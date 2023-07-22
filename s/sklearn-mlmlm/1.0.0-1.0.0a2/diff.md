# Comparing `tmp/sklearn_mlmlm-1.0.0.tar.gz` & `tmp/sklearn_mlmlm-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_mlmlm-1.0.0.tar", max compression
+gzip compressed data, was "sklearn_mlmlm-1.0.0a2.tar", max compression
```

## Comparing `sklearn_mlmlm-1.0.0.tar` & `sklearn_mlmlm-1.0.0a2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1556 2023-07-22 18:15:10.600704 sklearn_mlmlm-1.0.0/LICENSE
--rw-r--r--   0        0        0      844 2023-07-22 18:15:10.600704 sklearn_mlmlm-1.0.0/README.rst
--rw-r--r--   0        0        0     1084 2023-07-22 18:16:09.717231 sklearn_mlmlm-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     8685 2023-07-22 18:15:10.608704 sklearn_mlmlm-1.0.0/src/sklearn_mlmlm/classifiers.py
--rw-r--r--   0        0        0     1749 1970-01-01 00:00:00.000000 sklearn_mlmlm-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1556 2023-07-22 18:24:53.386052 sklearn_mlmlm-1.0.0a2/LICENSE
+-rw-r--r--   0        0        0      844 2023-07-22 18:24:53.386052 sklearn_mlmlm-1.0.0a2/README.rst
+-rw-r--r--   0        0        0     1086 2023-07-22 18:25:41.910696 sklearn_mlmlm-1.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     8685 2023-07-22 18:24:53.390052 sklearn_mlmlm-1.0.0a2/src/sklearn_mlmlm/classifiers.py
+-rw-r--r--   0        0        0     1751 1970-01-01 00:00:00.000000 sklearn_mlmlm-1.0.0a2/PKG-INFO
```

### Comparing `sklearn_mlmlm-1.0.0/LICENSE` & `sklearn_mlmlm-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_mlmlm-1.0.0/README.rst` & `sklearn_mlmlm-1.0.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `sklearn_mlmlm-1.0.0/pyproject.toml` & `sklearn_mlmlm-1.0.0a2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 [tool.poetry]
 name = "sklearn_mlmlm"
-version = "1.0.0"
+version = "1.0.0a2"
 authors = ["Daniel E Fredriksen <dfredriksen@quantyra.org>"]
 description = "A python and sklearn compatible implementation of ML-MLM."
 readme = "README.rst"
 classifiers = [
     'Intended Audience :: Science/Research',
     'Programming Language :: Python',
     'Topic :: Software Development',
```

### Comparing `sklearn_mlmlm-1.0.0/src/sklearn_mlmlm/classifiers.py` & `sklearn_mlmlm-1.0.0a2/src/sklearn_mlmlm/classifiers.py`

 * *Files identical despite different names*

### Comparing `sklearn_mlmlm-1.0.0/PKG-INFO` & `sklearn_mlmlm-1.0.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn-mlmlm
-Version: 1.0.0
+Version: 1.0.0a2
 Summary: A python and sklearn compatible implementation of ML-MLM.
 Author: Daniel E Fredriksen
 Author-email: dfredriksen@quantyra.org
 Requires-Python: >=3.10,<3.13
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
```

