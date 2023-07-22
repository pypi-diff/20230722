# Comparing `tmp/marketwatchdata-0.0.3.tar.gz` & `tmp/marketwatchdata-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marketwatchdata-0.0.3.tar", last modified: Sat Jul 22 14:56:08 2023, max compression
+gzip compressed data, was "marketwatchdata-0.0.4.tar", last modified: Sat Jul 22 15:04:49 2023, max compression
```

## Comparing `marketwatchdata-0.0.3.tar` & `marketwatchdata-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:56:08.821562 marketwatchdata-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 14:55:41.000000 marketwatchdata-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-22 14:55:41.000000 marketwatchdata-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-22 14:56:08.821562 marketwatchdata-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-22 14:55:41.000000 marketwatchdata-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:56:08.821562 marketwatchdata-0.0.3/marketwatchdata/
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-22 14:55:41.000000 marketwatchdata-0.0.3/marketwatchdata/MarketWatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-22 14:55:41.000000 marketwatchdata-0.0.3/marketwatchdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:56:08.821562 marketwatchdata-0.0.3/marketwatchdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-22 14:56:08.000000 marketwatchdata-0.0.3/marketwatchdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-22 14:56:08.000000 marketwatchdata-0.0.3/marketwatchdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 14:56:08.000000 marketwatchdata-0.0.3/marketwatchdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-22 14:56:08.000000 marketwatchdata-0.0.3/marketwatchdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 14:56:08.000000 marketwatchdata-0.0.3/marketwatchdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-22 14:55:41.000000 marketwatchdata-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 14:56:08.821562 marketwatchdata-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-22 14:55:41.000000 marketwatchdata-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:56:08.821562 marketwatchdata-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-22 14:55:41.000000 marketwatchdata-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-22 14:55:41.000000 marketwatchdata-0.0.3/tests/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:04:49.163262 marketwatchdata-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 15:04:09.000000 marketwatchdata-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-22 15:04:09.000000 marketwatchdata-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-22 15:04:49.163262 marketwatchdata-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-22 15:04:09.000000 marketwatchdata-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:04:49.163262 marketwatchdata-0.0.4/marketwatchdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-22 15:04:09.000000 marketwatchdata-0.0.4/marketwatchdata/MarketWatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-22 15:04:09.000000 marketwatchdata-0.0.4/marketwatchdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:04:49.163262 marketwatchdata-0.0.4/marketwatchdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-22 15:04:49.000000 marketwatchdata-0.0.4/marketwatchdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-22 15:04:49.000000 marketwatchdata-0.0.4/marketwatchdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 15:04:49.000000 marketwatchdata-0.0.4/marketwatchdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-22 15:04:49.000000 marketwatchdata-0.0.4/marketwatchdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 15:04:49.000000 marketwatchdata-0.0.4/marketwatchdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-22 15:04:09.000000 marketwatchdata-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 15:04:49.163262 marketwatchdata-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-22 15:04:09.000000 marketwatchdata-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:04:49.163262 marketwatchdata-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-22 15:04:09.000000 marketwatchdata-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-22 15:04:09.000000 marketwatchdata-0.0.4/tests/test_func.py
```

### Comparing `marketwatchdata-0.0.3/LICENSE` & `marketwatchdata-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `marketwatchdata-0.0.3/PKG-INFO` & `marketwatchdata-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marketwatchdata
-Version: 0.0.3
+Version: 0.0.4
 Summary: retrieve data from MarketWatch.com
 Home-page: https://github.com/yacper/marketwatchdata
 Author: yacper
 Author-email: yacper@gmail.com
 License: MIT
 Keywords: stock,option,futures,fund,bond,index,air,finance,spider,quant,quantitative,investment,trading,algotrading,data
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `marketwatchdata-0.0.3/marketwatchdata/MarketWatch.py` & `marketwatchdata-0.0.4/marketwatchdata/MarketWatch.py`

 * *Files identical despite different names*

### Comparing `marketwatchdata-0.0.3/marketwatchdata.egg-info/PKG-INFO` & `marketwatchdata-0.0.4/marketwatchdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marketwatchdata
-Version: 0.0.3
+Version: 0.0.4
 Summary: retrieve data from MarketWatch.com
 Home-page: https://github.com/yacper/marketwatchdata
 Author: yacper
 Author-email: yacper@gmail.com
 License: MIT
 Keywords: stock,option,futures,fund,bond,index,air,finance,spider,quant,quantitative,investment,trading,algotrading,data
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `marketwatchdata-0.0.3/setup.py` & `marketwatchdata-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `marketwatchdata-0.0.3/tests/test_func.py` & `marketwatchdata-0.0.4/tests/test_func.py`

 * *Files identical despite different names*

