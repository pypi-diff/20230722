# Comparing `tmp/botocore-a-la-carte-macie2-1.31.6.tar.gz` & `tmp/botocore-a-la-carte-macie2-1.31.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-macie2-1.31.6.tar", last modified: Thu Jul 20 01:20:33 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-macie2-1.31.8.tar", last modified: Fri Jul 21 01:21:43 2023, max compression
```

## Comparing `botocore-a-la-carte-macie2-1.31.6.tar` & `botocore-a-la-carte-macie2-1.31.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:33.366806 botocore-a-la-carte-macie2-1.31.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-20 01:20:33.000000 botocore-a-la-carte-macie2-1.31.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-20 01:20:33.366806 botocore-a-la-carte-macie2-1.31.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:33.366806 botocore-a-la-carte-macie2-1.31.6/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:33.366806 botocore-a-la-carte-macie2-1.31.6/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:33.366806 botocore-a-la-carte-macie2-1.31.6/botocore/data/macie2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:33.366806 botocore-a-la-carte-macie2-1.31.6/botocore/data/macie2/2020-01-01/
--rw-r--r--   0 runner    (1001) docker     (123)    17624 2023-07-20 01:19:55.000000 botocore-a-la-carte-macie2-1.31.6/botocore/data/macie2/2020-01-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-20 01:19:55.000000 botocore-a-la-carte-macie2-1.31.6/botocore/data/macie2/2020-01-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   484586 2023-07-20 01:19:55.000000 botocore-a-la-carte-macie2-1.31.6/botocore/data/macie2/2020-01-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-20 01:19:55.000000 botocore-a-la-carte-macie2-1.31.6/botocore/data/macie2/2020-01-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:33.366806 botocore-a-la-carte-macie2-1.31.6/botocore_a_la_carte_macie2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-20 01:20:33.000000 botocore-a-la-carte-macie2-1.31.6/botocore_a_la_carte_macie2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-20 01:20:33.000000 botocore-a-la-carte-macie2-1.31.6/botocore_a_la_carte_macie2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 01:20:33.000000 botocore-a-la-carte-macie2-1.31.6/botocore_a_la_carte_macie2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 01:20:33.000000 botocore-a-la-carte-macie2-1.31.6/botocore_a_la_carte_macie2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 01:20:33.366806 botocore-a-la-carte-macie2-1.31.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-20 01:20:33.000000 botocore-a-la-carte-macie2-1.31.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:43.023325 botocore-a-la-carte-macie2-1.31.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:42.000000 botocore-a-la-carte-macie2-1.31.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-21 01:21:43.023325 botocore-a-la-carte-macie2-1.31.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:43.023325 botocore-a-la-carte-macie2-1.31.8/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:43.023325 botocore-a-la-carte-macie2-1.31.8/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:43.023325 botocore-a-la-carte-macie2-1.31.8/botocore/data/macie2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:43.023325 botocore-a-la-carte-macie2-1.31.8/botocore/data/macie2/2020-01-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    17624 2023-07-21 01:21:06.000000 botocore-a-la-carte-macie2-1.31.8/botocore/data/macie2/2020-01-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-21 01:21:06.000000 botocore-a-la-carte-macie2-1.31.8/botocore/data/macie2/2020-01-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   484586 2023-07-21 01:21:06.000000 botocore-a-la-carte-macie2-1.31.8/botocore/data/macie2/2020-01-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-21 01:21:06.000000 botocore-a-la-carte-macie2-1.31.8/botocore/data/macie2/2020-01-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:43.023325 botocore-a-la-carte-macie2-1.31.8/botocore_a_la_carte_macie2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-21 01:21:42.000000 botocore-a-la-carte-macie2-1.31.8/botocore_a_la_carte_macie2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-21 01:21:42.000000 botocore-a-la-carte-macie2-1.31.8/botocore_a_la_carte_macie2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:42.000000 botocore-a-la-carte-macie2-1.31.8/botocore_a_la_carte_macie2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:42.000000 botocore-a-la-carte-macie2-1.31.8/botocore_a_la_carte_macie2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:43.023325 botocore-a-la-carte-macie2-1.31.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-21 01:21:42.000000 botocore-a-la-carte-macie2-1.31.8/setup.py
```

### Comparing `botocore-a-la-carte-macie2-1.31.6/LICENSE.txt` & `botocore-a-la-carte-macie2-1.31.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-macie2-1.31.6/PKG-INFO` & `botocore-a-la-carte-macie2-1.31.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-macie2
-Version: 1.31.6
+Version: 1.31.8
 Summary: macie2 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-macie2-1.31.6/botocore/data/macie2/2020-01-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-macie2-1.31.8/botocore/data/macie2/2020-01-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-macie2-1.31.6/botocore/data/macie2/2020-01-01/paginators-1.json` & `botocore-a-la-carte-macie2-1.31.8/botocore/data/macie2/2020-01-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-macie2-1.31.6/botocore/data/macie2/2020-01-01/service-2.json` & `botocore-a-la-carte-macie2-1.31.8/botocore/data/macie2/2020-01-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-macie2-1.31.6/botocore/data/macie2/2020-01-01/waiters-2.json` & `botocore-a-la-carte-macie2-1.31.8/botocore/data/macie2/2020-01-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-macie2-1.31.6/botocore_a_la_carte_macie2.egg-info/PKG-INFO` & `botocore-a-la-carte-macie2-1.31.8/botocore_a_la_carte_macie2.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-macie2
-Version: 1.31.6
+Version: 1.31.8
 Summary: macie2 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-macie2-1.31.6/setup.py` & `botocore-a-la-carte-macie2-1.31.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-macie2',
-    version="1.31.6",
+    version="1.31.8",
     description='macie2 data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/macie2/*/*.json'],
```

