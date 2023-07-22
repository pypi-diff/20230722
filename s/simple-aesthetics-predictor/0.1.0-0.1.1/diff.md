# Comparing `tmp/simple_aesthetics_predictor-0.1.0.tar.gz` & `tmp/simple_aesthetics_predictor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_aesthetics_predictor-0.1.0.tar", max compression
+gzip compressed data, was "simple_aesthetics_predictor-0.1.1.tar", max compression
```

## Comparing `simple_aesthetics_predictor-0.1.0.tar` & `simple_aesthetics_predictor-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2023-07-22 07:27:34.538768 simple_aesthetics_predictor-0.1.0/LICENSE
--rw-r--r--   0        0        0     2428 2023-07-22 07:27:34.538768 simple_aesthetics_predictor-0.1.0/README.md
--rw-r--r--   0        0        0      178 2023-07-22 07:27:34.538768 simple_aesthetics_predictor-0.1.0/aesthetics_predictor/__init__.py
--rw-r--r--   0        0        0      525 2023-07-22 07:27:34.538768 simple_aesthetics_predictor-0.1.0/aesthetics_predictor/utils.py
--rw-r--r--   0        0        0     2338 2023-07-22 07:27:34.542768 simple_aesthetics_predictor-0.1.0/aesthetics_predictor/v1.py
--rw-r--r--   0        0        0     4467 2023-07-22 07:27:34.542768 simple_aesthetics_predictor-0.1.0/aesthetics_predictor/v2.py
--rw-r--r--   0        0        0      685 2023-07-22 07:27:47.678723 simple_aesthetics_predictor-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3010 1970-01-01 00:00:00.000000 simple_aesthetics_predictor-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-22 08:03:10.192359 simple_aesthetics_predictor-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2428 2023-07-22 08:03:10.192359 simple_aesthetics_predictor-0.1.1/README.md
+-rw-r--r--   0        0        0      178 2023-07-22 08:03:10.192359 simple_aesthetics_predictor-0.1.1/aesthetics_predictor/__init__.py
+-rw-r--r--   0        0        0      525 2023-07-22 08:03:10.192359 simple_aesthetics_predictor-0.1.1/aesthetics_predictor/utils.py
+-rw-r--r--   0        0        0     2338 2023-07-22 08:03:10.192359 simple_aesthetics_predictor-0.1.1/aesthetics_predictor/v1.py
+-rw-r--r--   0        0        0     4467 2023-07-22 08:03:10.196359 simple_aesthetics_predictor-0.1.1/aesthetics_predictor/v2.py
+-rw-r--r--   0        0        0      685 2023-07-22 08:03:26.540563 simple_aesthetics_predictor-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3010 1970-01-01 00:00:00.000000 simple_aesthetics_predictor-0.1.1/PKG-INFO
```

### Comparing `simple_aesthetics_predictor-0.1.0/LICENSE` & `simple_aesthetics_predictor-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_aesthetics_predictor-0.1.0/README.md` & `simple_aesthetics_predictor-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `simple_aesthetics_predictor-0.1.0/aesthetics_predictor/utils.py` & `simple_aesthetics_predictor-0.1.1/aesthetics_predictor/utils.py`

 * *Files identical despite different names*

### Comparing `simple_aesthetics_predictor-0.1.0/aesthetics_predictor/v1.py` & `simple_aesthetics_predictor-0.1.1/aesthetics_predictor/v1.py`

 * *Files identical despite different names*

### Comparing `simple_aesthetics_predictor-0.1.0/aesthetics_predictor/v2.py` & `simple_aesthetics_predictor-0.1.1/aesthetics_predictor/v2.py`

 * *Files identical despite different names*

### Comparing `simple_aesthetics_predictor-0.1.0/pyproject.toml` & `simple_aesthetics_predictor-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simple-aesthetics-predictor"
-version = "0.1.0" # specified by poetry-dynamic-versioning
+version = "0.1.1" # specified by poetry-dynamic-versioning
 description = ""
 authors = ["Shunsuke KITADA <shunsuke.kitada.0831@gmail.com>"]
 readme = "README.md"
 packages = [{include = "aesthetics_predictor"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `simple_aesthetics_predictor-0.1.0/PKG-INFO` & `simple_aesthetics_predictor-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-aesthetics-predictor
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Shunsuke KITADA
 Author-email: shunsuke.kitada.0831@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

