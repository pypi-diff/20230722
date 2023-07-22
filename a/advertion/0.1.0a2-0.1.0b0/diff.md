# Comparing `tmp/advertion-0.1.0a2.tar.gz` & `tmp/advertion-0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advertion-0.1.0a2.tar", max compression
+gzip compressed data, was "advertion-0.1.0b0.tar", max compression
```

## Comparing `advertion-0.1.0a2.tar` & `advertion-0.1.0b0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1496 2023-07-16 11:09:45.586284 advertion-0.1.0a2/README.md
--rw-r--r--   0        0        0       98 2023-07-16 11:09:45.586284 advertion-0.1.0a2/advertion/__init__.py
--rw-r--r--   0        0        0     6287 2023-07-16 11:09:45.586284 advertion-0.1.0a2/advertion/core.py
--rw-r--r--   0        0        0     1857 2023-07-16 11:09:45.586284 advertion-0.1.0a2/advertion/public.py
--rw-r--r--   0        0        0     1445 2023-07-16 11:09:45.590284 advertion-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     2959 1970-01-01 00:00:00.000000 advertion-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     2667 2023-07-19 21:22:16.718805 advertion-0.1.0b0/README.md
+-rw-r--r--   0        0        0      101 2023-07-19 21:22:16.718805 advertion-0.1.0b0/advertion/__init__.py
+-rw-r--r--   0        0        0     6762 2023-07-19 21:22:16.718805 advertion-0.1.0b0/advertion/core.py
+-rw-r--r--   0        0        0     1859 2023-07-19 21:22:16.718805 advertion-0.1.0b0/advertion/public.py
+-rw-r--r--   0        0        0      100 2023-07-19 21:22:16.718805 advertion-0.1.0b0/advertion/version.py
+-rw-r--r--   0        0        0     1969 2023-07-19 21:22:16.718805 advertion-0.1.0b0/pyproject.toml
+-rw-r--r--   0        0        0     4165 1970-01-01 00:00:00.000000 advertion-0.1.0b0/PKG-INFO
```

### Comparing `advertion-0.1.0a2/advertion/core.py` & `advertion-0.1.0b0/advertion/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,120 +2,114 @@
 from statistics import mean
 from typing import Iterable, Union
 
 import numpy as np
 import pandas as pd
 import xgboost as xgb
 from pydantic import validate_call
+from scipy import stats
 from sklearn import metrics, model_selection
 
+from .version import __version__
+
 
 class AdversarialValidation(object):
     """`AdversarialValidation` is an internal interface performing adversarial validation
     on your training and test datasets.
 
     **Note**: Any attributes or methods prefixed with _underscores are forming a so-called "private" API, and is
     for internal use only. They may be changed or removed at anytime.
     """
 
     @validate_call(config=dict(arbitrary_types_allowed=True))
     def __init__(
         self,
-        train: pd.DataFrame,
-        test: pd.DataFrame,
-        target: str,
         smart: bool = True,
         n_splits: int = 5,
         verbose: bool = True,
-        random_state: Union[int, np.random.RandomState] = None,
+        random_state: Union[int, np.random.RandomState, None] = None,
     ):
-        self._train = train
-        self._test = test
-        self._target = target
         self._smart = smart
         self._n_splits = n_splits
         self._verbose = verbose
         self._random_state = random_state
         self._av_target = "_av_target_"
-        self._feature_importance_threshold = 0.95
-        self._tol = 0.05
+        self._statistic_threshold = 0.1
+        self._p_value_threshold = 0.05
+        self._decision_tolerance = 0.05
 
-    def perform(self):
+    @validate_call(config=dict(arbitrary_types_allowed=True))
+    def perform(
+        self, trainset: pd.DataFrame, testset: pd.DataFrame, target: str
+    ) -> dict:
         """Orchestrates the adversarial validation process.
 
         - Creates a new feature in both the training and test datasets.
         - Sets the value of the new feature to 0.0 for the training dataset, and 1.0 for the test dataset.
         - Drops original target variable from training dataset.
         - Combines the training and test datasets into a single dataset - let's call it `meta-dataset`.
+        - Optionally, identifies and drops adversarial features in the design matrix.
         - Performs cross-validation on the meta-dataset, using the new feature as the target variable.
 
+        Args:
+            trainset (pd.DataFrame): The training dataset.
+            testset (pd.DataFrame): The test dataset.
+            target (str): The target column name.
+
         Returns:
-            bool: Whether the train & test datasets follow the same underlying distribution.
+            dict: An informative key-valued response.
         """
-        train = self.__keep_numeric_types(self._train)
-        test = self.__keep_numeric_types(self._test)
+        response = dict()
 
-        train[self._av_target] = 0.0
-        test[self._av_target] = 1.0
+        print(
+            "INFO: Working only with available numerical features, categorical features are not yet supported."
+        )
+        trainset = self.__preprocessing(trainset)
+        testset = self.__preprocessing(testset)
+
+        trainset[self._av_target] = 0.0
+        testset[self._av_target] = 1.0
 
-        train = train.drop(self._target, axis=1)
+        trainset = trainset.drop(target, axis=1)
 
-        combined = pd.concat([train, test], axis=0, ignore_index=True)
+        combined = pd.concat([trainset, testset], axis=0, ignore_index=True)
+
+        combined = combined.sample(frac=1)
 
         X = combined.drop(self._av_target, axis=1)
 
         y = combined[self._av_target]
 
         if self._smart:
-            X = self._prune_features(X, y)
+            adv_features = [*self._identify_adversarial_features(trainset, testset)]
+            X = X.drop(adv_features, axis=1)
+            response["adversarial_features"] = adv_features
 
         mean_roc_auc = mean([*self._cross_validate(X, y)])
 
-        no_better_than_random = isclose(0.5, mean_roc_auc, abs_tol=self._tol)
-
-        return (
-            self.datasets_are_similar(mean_roc_auc)
-            if no_better_than_random
-            else self.datasets_are_different(mean_roc_auc)
+        no_better_than_random = isclose(
+            0.5, mean_roc_auc, abs_tol=self._decision_tolerance
         )
 
-    def datasets_are_similar(self, metric: float) -> bool:
-        """Handles the response when the training and test datasets follow the same underlying distribution.
-
-        Args:
-            metric (float): The mean ROC AUC score.
-
-        Returns:
-            bool: Always returns True.
-        """
         if self._verbose:
-            print(
-                f"INFO: The training and test datasets are similar [mean ROC AUC: {round(metric, 3)}]."
-            )
-        return True
+            info = "INFO: training and test datasets "
+            info += "follow" if no_better_than_random else "do not follow"
+            info += " the same underlying distribution"
+            info += f" [mean ROC AUC: {round(mean_roc_auc, 3)}]."
 
-    def datasets_are_different(self, metric: float) -> bool:
-        """Handles the response when the training and test datasets follow different underlying distributions.
-
-        Args:
-            metric (float): The mean ROC AUC score.
-
-        Returns:
-            bool: Always returns False.
-        """
-        if self._verbose:
-            print(
-                f"INFO: The training and test datasets are similar [mean ROC AUC: {round(metric, 3)}]."
-            )
-
-            if metric < 0.4:
+            print(info)
+            if mean_roc_auc < 0.4:
                 print(
                     f"INFO: The reported ROC AUC value is very low, which may indicate a class confusion problem."
                 )
-        return False
+
+        response["datasets_follow_same_distribution"] = no_better_than_random
+        response["mean_roc_auc"] = mean_roc_auc
+
+        return response
 
     def _cross_validate(self, X: pd.DataFrame, y: pd.Series) -> Iterable[float]:
         """Performs cross-validation, calculating the
         Area Under the Receiver Operating Characteristic Curve (ROC AUC)
         from prediction scores.
 
         Args:
@@ -137,57 +131,66 @@
 
             clf.fit(X_train, y_train)
 
             y_pred = clf.predict_proba(X_test)[:, 1]
 
             yield metrics.roc_auc_score(y_test, y_pred)
 
-    def _prune_features(self, X: pd.DataFrame, y: pd.Series) -> pd.DataFrame:
+    def _identify_adversarial_features(
+        self, trainset: pd.DataFrame, testset: pd.DataFrame
+    ) -> Iterable[str]:
         """Prunes features from the design matrix, based on a feature importance scheme.
 
         Args:
-            X (pd.DataFrame): The design matrix.
-            y (pd.Series): The target variable.
+            trainset (pd.DataFrame): The training dataset.
+            testset (pd.DataFrame): The test dataset.
 
         Returns:
-            pd.DataFrame: The pruned design matrix.
+            Iterable[str]: An iterable of feature names.
         """
-        clf = self._classifier()
-
-        model = clf.fit(X, y)
+        print(
+            f"INFO: Will try to identify adv. features "
+            f"(see: https://advertion.readthedocs.io/en/{__version__}/adversarial-features)"
+        )
 
-        prunable_features = [
-            feature
-            for feature, importance in zip(X.columns, model.feature_importances_)
-            if importance >= self._feature_importance_threshold
-        ]
+        for feature in testset.columns:
+            if isinstance(feature, str) and feature == self._av_target:
+                continue
 
-        if self._verbose:
-            print(
-                f"INFO: The following features were pruned, based on feature importance: {prunable_features}"
+            statistic, p_value = stats.kstest(
+                trainset[feature].values, testset[feature].values
             )
 
-        return X.drop(prunable_features, axis=1)
+            if (
+                statistic > self._statistic_threshold
+                and p_value < self._p_value_threshold
+            ):
+                if self._verbose:
+                    print(
+                        f"INFO: Identified adversarial feature: "
+                        f"[name: {feature}, statistic: {statistic}, p-value: {p_value}]."
+                    )
+
+                yield feature
 
     @staticmethod
-    def __keep_numeric_types(df: pd.DataFrame) -> pd.DataFrame:
-        """Keeps only numeric columns in the `df`.
+    def __preprocessing(df: pd.DataFrame) -> pd.DataFrame:
+        """Performs sensible preprocessing on `df` (in a copy of it).
 
         Args:
             df (pd.DataFrame): A DataFrame.
 
         Returns:
             pd.DataFrame: A DataFrame with only numeric-type columns.
         """
         return df.select_dtypes(include=np.number).copy()
 
-    @staticmethod
-    def _classifier(**params):
+    def _classifier(self, **params):
         """Returns a classifier instance.
 
         Args:
             **params: Arbitrary keyword arguments.
 
         Returns:
             xgb.XGBClassifier: An XGBoost classifier instance.
         """
-        return xgb.XGBClassifier(**params)
+        return xgb.XGBClassifier(**params, random_state=self._random_state)
```

### Comparing `advertion-0.1.0a2/pyproject.toml` & `advertion-0.1.0b0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "advertion"
-version = "0.1.0-alpha2"
+version = "0.1.0-beta"
 description = "A tiny framework to perform adversarial validation of your training and test data."
 authors = ["Ilias Antonopoulos <ilias.antonopoulos@yahoo.gr>"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://pypi.org/project/advertion"
 repository = "https://github.com/ilias-ant/adversarial-validation"
 keywords = ["adversarial-validation", "data-drift", "machine-learning"]
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Science/Research",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -25,23 +25,53 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.6,<3.12"
 
 scikit-learn = "~1.3.0"
 pandas = "~2.0.3"
 pydantic = "~2.0.3"
+scipy = "~1.10.1"   # scipy v1.11+ requires Python <3.13,>=3.9, but we need for now Python 3.8 for readthedocs
 xgboost = "~1.7.6"
 
 [tool.poetry.group.dev.dependencies]
+autoflake = "^2.2.0"
+bandit = "^1.7.5"
 black = "^23.3.0"
 isort = "^5.12.0"
 mkdocs = "^1.4.3"
 mkdocs-material = "^9.1.18"
 mkdocstrings = {version = "^0.20.0", extras = ["python"]}
 notebook = "^6.5.4"
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 
+[tool.black]
+line-length = 88
+skip-string-normalization = true
+target-version = ['py38', 'py39', 'py310', 'py311']
+include = '\.pyi?$'
+exclude = '''
+/(
+    \.git
+  | \.hg
+  | \.mypy_cache
+  | \.tox
+  | \.venv
+  | \.pytest_cache
+  | \.test_coverage
+  | _build
+  | buck-out
+  | build
+  | dist
+)/
+'''
+
+[tool.isort]
+profile = "black"
+
+[tool.bandit]
+exclude_dirs = ["tests"]
+skips = []
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `advertion-0.1.0a2/PKG-INFO` & `advertion-0.1.0b0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,38 @@
-Metadata-Version: 2.1
-Name: advertion
-Version: 0.1.0a2
-Summary: A tiny framework to perform adversarial validation of your training and test data.
-Home-page: https://pypi.org/project/advertion
-License: Apache-2.0
-Keywords: adversarial-validation,data-drift,machine-learning
-Author: Ilias Antonopoulos
-Author-email: ilias.antonopoulos@yahoo.gr
-Requires-Python: >=3.8.6,<3.12
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: pandas (>=2.0.3,<2.1.0)
-Requires-Dist: pydantic (>=2.0.3,<2.1.0)
-Requires-Dist: scikit-learn (>=1.3.0,<1.4.0)
-Requires-Dist: xgboost (>=1.7.6,<1.8.0)
-Project-URL: Bug Tracker, https://github.com/ilias-ant/adversarial-validation/issues
-Project-URL: Repository, https://github.com/ilias-ant/adversarial-validation
-Description-Content-Type: text/markdown
-
 # adversarial-validation
 
 [![PyPI](https://img.shields.io/pypi/v/advertion?color=blue&label=PyPI&logo=PyPI&logoColor=white)](https://pypi.org/project/advertion/) 
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/advertion?logo=python&logoColor=white)](https://www.python.org/) 
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/advertion?logo=python&logoColor=white)](https://www.python.org/)
+[![codecov](https://codecov.io/gh/ilias-ant/adversarial-validation/branch/main/graph/badge.svg?token=WXJ66ACKTA)](https://codecov.io/gh/ilias-ant/adversarial-validation)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ilias-ant/adversarial-validation/ci.yml?branch=main)](https://github.com/ilias-ant/adversarial-validation/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/advertion/badge/?version=latest)](https://advertion.readthedocs.io/en/latest/?badge=latest)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/advertion?color=orange)](https://www.python.org/dev/peps/pep-0427/)
 
 A tiny framework to perform adversarial validation of your training and test data.
 
+<img src="https://raw.githubusercontent.com/ilias-ant/adversarial-validation/main/static/logo.png" width="95%" text="figjam">
+
+**What is adversarial validation?**
+
+A common workflow in machine learning projects (*especially in Kaggle competitions*) is to:
+
+1. train your ML model in a training dataset.
+2. tune and validate your ML model in a validation dataset (*which typically originates as a fraction of the training 
+dataset*). 
+3. finally, assess the actual generalization ability of your ML model in a held-out test dataset.
+
+This strategy is widely accepted, but it heavily relies on the assumption that the training and test datasets are drawn 
+from the same underlying distribution. This is often referred to as the “identically distributed” property in the 
+literature.
+
+This package helps you easily assert whether the "identically distributed" property holds true for your training and 
+test datasets or equivalently whether your validation dataset is a good proxy for your model's performance on the unseen 
+test instances.
+
 ## Install
 
 The recommended installation is via `pip`:
 
 ```bash
 pip install advertion
 ```
@@ -55,15 +43,19 @@
 
 ```python
 from advertion import validate
 
 train = pd.read_csv("...")
 test = pd.read_csv("...")
 
-are_similar = validate(
-    train=train,
-    test=test,
+validate(
+    trainset=train,
+    testset=test,
     target="label",
 )
-# are_similar = True: train and test are following the same underlying distribution.
-# are_similar = False: test dataset exhibits a different underlying distribution than train dataset.
-```
+
+# // {
+# //     "datasets_follow_same_distribution": True,
+# //     'mean_roc_auc': 0.5021320833333334,
+# //     "adversarial_features': ['id'],
+# // }
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

