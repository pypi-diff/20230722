# Comparing `tmp/focus-cfe-0.0.dev2.tar.gz` & `tmp/focus-cfe-0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/focus-cfe-0.0.dev2.tar", last modified: Sun Jul 16 21:02:47 2023, max compression
+gzip compressed data, was "dist/focus-cfe-0.0.dev3.tar", last modified: Sat Jul 22 18:20:54 2023, max compression
```

## Comparing `focus-cfe-0.0.dev2.tar` & `focus-cfe-0.0.dev3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-16 21:02:47.490738 focus-cfe-0.0.dev2/
--rw-r--r--   0 kyosuke    (501) staff       (20)     4737 2023-07-16 21:02:47.490905 focus-cfe-0.0.dev2/PKG-INFO
--rw-r--r--   0 kyosuke    (501) staff       (20)     3228 2023-07-16 20:26:06.000000 focus-cfe-0.0.dev2/README.rst
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-16 21:02:47.487327 focus-cfe-0.0.dev2/focus/
--rw-r--r--   0 kyosuke    (501) staff       (20)      597 2023-07-15 18:38:07.000000 focus-cfe-0.0.dev2/focus/__init__.py
--rw-r--r--   0 kyosuke    (501) staff       (20)    18455 2023-07-15 21:50:24.000000 focus-cfe-0.0.dev2/focus/core.py
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-16 21:02:47.488533 focus-cfe-0.0.dev2/focus/tests/
--rw-r--r--   0 kyosuke    (501) staff       (20)        0 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev2/focus/tests/__init__.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     3883 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev2/focus/tests/test_focus.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     4156 2023-07-15 18:42:01.000000 focus-cfe-0.0.dev2/focus/tests/test_utils.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     4643 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev2/focus/utils.py
--rw-r--r--   0 kyosuke    (501) staff       (20)      568 2023-07-16 21:01:59.000000 focus-cfe-0.0.dev2/focus/version.py
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-16 21:02:47.490493 focus-cfe-0.0.dev2/focus_cfe.egg-info/
--rw-r--r--   0 kyosuke    (501) staff       (20)     4737 2023-07-16 21:02:47.000000 focus-cfe-0.0.dev2/focus_cfe.egg-info/PKG-INFO
--rw-r--r--   0 kyosuke    (501) staff       (20)      301 2023-07-16 21:02:47.000000 focus-cfe-0.0.dev2/focus_cfe.egg-info/SOURCES.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)        1 2023-07-16 21:02:47.000000 focus-cfe-0.0.dev2/focus_cfe.egg-info/dependency_links.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)        6 2023-07-16 21:02:47.000000 focus-cfe-0.0.dev2/focus_cfe.egg-info/top_level.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)       80 2023-07-16 21:02:47.491325 focus-cfe-0.0.dev2/setup.cfg
--rw-r--r--   0 kyosuke    (501) staff       (20)     1543 2023-07-10 22:03:45.000000 focus-cfe-0.0.dev2/setup.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-22 18:20:54.272191 focus-cfe-0.0.dev3/
+-rw-r--r--   0 kyosuke    (501) staff       (20)     5123 2023-07-22 18:20:54.272471 focus-cfe-0.0.dev3/PKG-INFO
+-rw-r--r--   0 kyosuke    (501) staff       (20)     3646 2023-07-22 16:39:29.000000 focus-cfe-0.0.dev3/README.rst
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-22 18:20:54.267780 focus-cfe-0.0.dev3/focus/
+-rw-r--r--   0 kyosuke    (501) staff       (20)      597 2023-07-15 18:38:07.000000 focus-cfe-0.0.dev3/focus/__init__.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)    18455 2023-07-15 21:50:24.000000 focus-cfe-0.0.dev3/focus/core.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-22 18:20:54.269296 focus-cfe-0.0.dev3/focus/tests/
+-rw-r--r--   0 kyosuke    (501) staff       (20)        0 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev3/focus/tests/__init__.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     3883 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev3/focus/tests/test_focus.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4156 2023-07-15 18:42:01.000000 focus-cfe-0.0.dev3/focus/tests/test_utils.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4643 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev3/focus/utils.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)      568 2023-07-22 18:20:15.000000 focus-cfe-0.0.dev3/focus/version.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-22 18:20:54.271683 focus-cfe-0.0.dev3/focus_cfe.egg-info/
+-rw-r--r--   0 kyosuke    (501) staff       (20)     5123 2023-07-22 18:20:54.000000 focus-cfe-0.0.dev3/focus_cfe.egg-info/PKG-INFO
+-rw-r--r--   0 kyosuke    (501) staff       (20)      301 2023-07-22 18:20:54.000000 focus-cfe-0.0.dev3/focus_cfe.egg-info/SOURCES.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)        1 2023-07-22 18:20:54.000000 focus-cfe-0.0.dev3/focus_cfe.egg-info/dependency_links.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)        6 2023-07-22 18:20:54.000000 focus-cfe-0.0.dev3/focus_cfe.egg-info/top_level.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)       80 2023-07-22 18:20:54.273224 focus-cfe-0.0.dev3/setup.cfg
+-rw-r--r--   0 kyosuke    (501) staff       (20)     1543 2023-07-10 22:03:45.000000 focus-cfe-0.0.dev3/setup.py
```

### Comparing `focus-cfe-0.0.dev2/PKG-INFO` & `focus-cfe-0.0.dev3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: focus-cfe
-Version: 0.0.dev2
+Version: 0.0.dev3
 Summary: FOCUS is a python package for generating counterfactual explanations for a tree-based model
 Home-page: UNKNOWN
 Author: Kyosuke Morita
 Author-email: kq441morita@gmail.com
 License: UNKNOWN
 Description: FOCUS: Flexible Optimizable Counterfactual Explanations for Tree Ensembles
         ==========================================================================
@@ -15,29 +15,24 @@
            :target: https://pypi.org/project/focus-cfe/
            :alt: PyPI version
         
         .. image:: https://readthedocs.org/projects/focus-cfe/badge/?version=latest
            :target: https://focus-cfe.readthedocs.io/en/latest/?badge=latest
            :alt: Documentation status
         
-        .. image:: https://img.shields.io/github/stars/kyosek/focus.svg
-           :target: https://github.com/kyosek/focus/stargazers
-           :alt: GitHub stars
-        
-        .. image:: https://img.shields.io/github/forks/kyosek/focus.svg?color=blue
-           :target: https://github.com/kyosek/focus/network
-           :alt: GitHub forks
-        
         .. image:: https://pepy.tech/badge/focus-cfe
            :target: https://pepy.tech/project/focus-cfe
            :alt: Downloads
         
-        .. image:: https://coveralls.io/repos/github/kyosek/focus/badge.svg
-           :target: https://coveralls.io/github/kyosek/focus
-           :alt: Coverage Status
+        .. image:: https://codecov.io/gh/kyosek/focus/branch/master/graph/badge.svg?token=G5I7TJR0JQ
+            :target: https://codecov.io/gh/kyosek/focus
+        
+        .. image:: https://dl.circleci.com/status-badge/img/gh/kyosek/focus/tree/master.svg?style=svg
+            :target: https://dl.circleci.com/status-badge/redirect/gh/kyosek/focus/tree/master
+            :alt: Circle CI
         
         .. image:: https://api.codeclimate.com/v1/badges/93840d29606abb212051/maintainability
            :target: https://codeclimate.com/github/kyosek/focus-cfe/maintainability
            :alt: Maintainability
         
         .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
            :target: https://github.com/kyosek/focus-cfe
@@ -72,19 +67,20 @@
         
         .. image:: docs/plot.png
             :width: 200px
             :height: 100px
             :scale: 50 %
             :alt: Before and After FOCUS was applied to the features from above example.
         
-        **Note**\:
+        **Limitations**\:
         
-        Currently FOCUS can be applied to scikit-learn `DecisionTreeClassifier`, `RandomForestClassifier` and `AdaBoostClassifier`.
+        - Currently, FOCUS can only be applied to scikit-learn `DecisionTreeClassifier`, `RandomForestClassifier` and `AdaBoostClassifier`.
+        - While categorical features may be included in the feature set, it is important to note that the interpretation of changes in categorical features, such as transitioning from age 40 to 20, may not provide meaningful insights.
+        - The input features should be scaled to the range of 0 and 1 before applying FOCUS. Therefore, it is necessary to transform the features prior to using FOCUS. However, this scaling process may introduce some additional complexity when interpreting the features after applying FOCUS.
         
-        Installation
         ^^^^^^^^^^^^
         
         It is recommended to use **pip** or **conda** for installation. Please make sure
         **the latest version** is installed:
         
         .. code-block:: bash
```

### Comparing `focus-cfe-0.0.dev2/README.rst` & `focus-cfe-0.0.dev3/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -7,29 +7,24 @@
    :target: https://pypi.org/project/focus-cfe/
    :alt: PyPI version
 
 .. image:: https://readthedocs.org/projects/focus-cfe/badge/?version=latest
    :target: https://focus-cfe.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation status
 
-.. image:: https://img.shields.io/github/stars/kyosek/focus.svg
-   :target: https://github.com/kyosek/focus/stargazers
-   :alt: GitHub stars
-
-.. image:: https://img.shields.io/github/forks/kyosek/focus.svg?color=blue
-   :target: https://github.com/kyosek/focus/network
-   :alt: GitHub forks
-
 .. image:: https://pepy.tech/badge/focus-cfe
    :target: https://pepy.tech/project/focus-cfe
    :alt: Downloads
 
-.. image:: https://coveralls.io/repos/github/kyosek/focus/badge.svg
-   :target: https://coveralls.io/github/kyosek/focus
-   :alt: Coverage Status
+.. image:: https://codecov.io/gh/kyosek/focus/branch/master/graph/badge.svg?token=G5I7TJR0JQ
+    :target: https://codecov.io/gh/kyosek/focus
+
+.. image:: https://dl.circleci.com/status-badge/img/gh/kyosek/focus/tree/master.svg?style=svg
+    :target: https://dl.circleci.com/status-badge/redirect/gh/kyosek/focus/tree/master
+    :alt: Circle CI
 
 .. image:: https://api.codeclimate.com/v1/badges/93840d29606abb212051/maintainability
    :target: https://codeclimate.com/github/kyosek/focus-cfe/maintainability
    :alt: Maintainability
 
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
    :target: https://github.com/kyosek/focus-cfe
@@ -64,19 +59,20 @@
 
 .. image:: docs/plot.png
     :width: 200px
     :height: 100px
     :scale: 50 %
     :alt: Before and After FOCUS was applied to the features from above example.
 
-**Note**\:
+**Limitations**\:
 
-Currently FOCUS can be applied to scikit-learn `DecisionTreeClassifier`, `RandomForestClassifier` and `AdaBoostClassifier`.
+- Currently, FOCUS can only be applied to scikit-learn `DecisionTreeClassifier`, `RandomForestClassifier` and `AdaBoostClassifier`.
+- While categorical features may be included in the feature set, it is important to note that the interpretation of changes in categorical features, such as transitioning from age 40 to 20, may not provide meaningful insights.
+- The input features should be scaled to the range of 0 and 1 before applying FOCUS. Therefore, it is necessary to transform the features prior to using FOCUS. However, this scaling process may introduce some additional complexity when interpreting the features after applying FOCUS.
 
-Installation
 ^^^^^^^^^^^^
 
 It is recommended to use **pip** or **conda** for installation. Please make sure
 **the latest version** is installed:
 
 .. code-block:: bash
```

### Comparing `focus-cfe-0.0.dev2/focus/__init__.py` & `focus-cfe-0.0.dev3/focus/__init__.py`

 * *Files identical despite different names*

### Comparing `focus-cfe-0.0.dev2/focus/core.py` & `focus-cfe-0.0.dev3/focus/core.py`

 * *Files identical despite different names*

### Comparing `focus-cfe-0.0.dev2/focus/tests/test_focus.py` & `focus-cfe-0.0.dev3/focus/tests/test_focus.py`

 * *Files identical despite different names*

### Comparing `focus-cfe-0.0.dev2/focus/tests/test_utils.py` & `focus-cfe-0.0.dev3/focus/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `focus-cfe-0.0.dev2/focus/utils.py` & `focus-cfe-0.0.dev3/focus/utils.py`

 * *Files identical despite different names*

### Comparing `focus-cfe-0.0.dev2/focus/version.py` & `focus-cfe-0.0.dev3/focus/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = "0.0.dev2"  # pragma: no cover
+__version__ = "0.0.dev3"  # pragma: no cover
```

### Comparing `focus-cfe-0.0.dev2/focus_cfe.egg-info/PKG-INFO` & `focus-cfe-0.0.dev3/focus_cfe.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: focus-cfe
-Version: 0.0.dev2
+Version: 0.0.dev3
 Summary: FOCUS is a python package for generating counterfactual explanations for a tree-based model
 Home-page: UNKNOWN
 Author: Kyosuke Morita
 Author-email: kq441morita@gmail.com
 License: UNKNOWN
 Description: FOCUS: Flexible Optimizable Counterfactual Explanations for Tree Ensembles
         ==========================================================================
@@ -15,29 +15,24 @@
            :target: https://pypi.org/project/focus-cfe/
            :alt: PyPI version
         
         .. image:: https://readthedocs.org/projects/focus-cfe/badge/?version=latest
            :target: https://focus-cfe.readthedocs.io/en/latest/?badge=latest
            :alt: Documentation status
         
-        .. image:: https://img.shields.io/github/stars/kyosek/focus.svg
-           :target: https://github.com/kyosek/focus/stargazers
-           :alt: GitHub stars
-        
-        .. image:: https://img.shields.io/github/forks/kyosek/focus.svg?color=blue
-           :target: https://github.com/kyosek/focus/network
-           :alt: GitHub forks
-        
         .. image:: https://pepy.tech/badge/focus-cfe
            :target: https://pepy.tech/project/focus-cfe
            :alt: Downloads
         
-        .. image:: https://coveralls.io/repos/github/kyosek/focus/badge.svg
-           :target: https://coveralls.io/github/kyosek/focus
-           :alt: Coverage Status
+        .. image:: https://codecov.io/gh/kyosek/focus/branch/master/graph/badge.svg?token=G5I7TJR0JQ
+            :target: https://codecov.io/gh/kyosek/focus
+        
+        .. image:: https://dl.circleci.com/status-badge/img/gh/kyosek/focus/tree/master.svg?style=svg
+            :target: https://dl.circleci.com/status-badge/redirect/gh/kyosek/focus/tree/master
+            :alt: Circle CI
         
         .. image:: https://api.codeclimate.com/v1/badges/93840d29606abb212051/maintainability
            :target: https://codeclimate.com/github/kyosek/focus-cfe/maintainability
            :alt: Maintainability
         
         .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
            :target: https://github.com/kyosek/focus-cfe
@@ -72,19 +67,20 @@
         
         .. image:: docs/plot.png
             :width: 200px
             :height: 100px
             :scale: 50 %
             :alt: Before and After FOCUS was applied to the features from above example.
         
-        **Note**\:
+        **Limitations**\:
         
-        Currently FOCUS can be applied to scikit-learn `DecisionTreeClassifier`, `RandomForestClassifier` and `AdaBoostClassifier`.
+        - Currently, FOCUS can only be applied to scikit-learn `DecisionTreeClassifier`, `RandomForestClassifier` and `AdaBoostClassifier`.
+        - While categorical features may be included in the feature set, it is important to note that the interpretation of changes in categorical features, such as transitioning from age 40 to 20, may not provide meaningful insights.
+        - The input features should be scaled to the range of 0 and 1 before applying FOCUS. Therefore, it is necessary to transform the features prior to using FOCUS. However, this scaling process may introduce some additional complexity when interpreting the features after applying FOCUS.
         
-        Installation
         ^^^^^^^^^^^^
         
         It is recommended to use **pip** or **conda** for installation. Please make sure
         **the latest version** is installed:
         
         .. code-block:: bash
```

### Comparing `focus-cfe-0.0.dev2/setup.py` & `focus-cfe-0.0.dev3/setup.py`

 * *Files identical despite different names*

