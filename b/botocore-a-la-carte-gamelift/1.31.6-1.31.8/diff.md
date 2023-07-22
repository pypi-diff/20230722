# Comparing `tmp/botocore-a-la-carte-gamelift-1.31.6.tar.gz` & `tmp/botocore-a-la-carte-gamelift-1.31.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-gamelift-1.31.6.tar", last modified: Thu Jul 20 01:20:25 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-gamelift-1.31.8.tar", last modified: Fri Jul 21 01:21:35 2023, max compression
```

## Comparing `botocore-a-la-carte-gamelift-1.31.6.tar` & `botocore-a-la-carte-gamelift-1.31.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:25.918731 botocore-a-la-carte-gamelift-1.31.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-20 01:20:25.000000 botocore-a-la-carte-gamelift-1.31.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-20 01:20:25.918731 botocore-a-la-carte-gamelift-1.31.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:25.914731 botocore-a-la-carte-gamelift-1.31.6/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:25.914731 botocore-a-la-carte-gamelift-1.31.6/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:25.914731 botocore-a-la-carte-gamelift-1.31.6/botocore/data/gamelift/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:25.914731 botocore-a-la-carte-gamelift-1.31.6/botocore/data/gamelift/2015-10-01/
--rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-07-20 01:19:55.000000 botocore-a-la-carte-gamelift-1.31.6/botocore/data/gamelift/2015-10-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 01:19:55.000000 botocore-a-la-carte-gamelift-1.31.6/botocore/data/gamelift/2015-10-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-20 01:19:55.000000 botocore-a-la-carte-gamelift-1.31.6/botocore/data/gamelift/2015-10-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   530402 2023-07-20 01:19:55.000000 botocore-a-la-carte-gamelift-1.31.6/botocore/data/gamelift/2015-10-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:25.918731 botocore-a-la-carte-gamelift-1.31.6/botocore_a_la_carte_gamelift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-20 01:20:25.000000 botocore-a-la-carte-gamelift-1.31.6/botocore_a_la_carte_gamelift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-20 01:20:25.000000 botocore-a-la-carte-gamelift-1.31.6/botocore_a_la_carte_gamelift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 01:20:25.000000 botocore-a-la-carte-gamelift-1.31.6/botocore_a_la_carte_gamelift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 01:20:25.000000 botocore-a-la-carte-gamelift-1.31.6/botocore_a_la_carte_gamelift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 01:20:25.918731 botocore-a-la-carte-gamelift-1.31.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-20 01:20:25.000000 botocore-a-la-carte-gamelift-1.31.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:35.327177 botocore-a-la-carte-gamelift-1.31.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:35.000000 botocore-a-la-carte-gamelift-1.31.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-21 01:21:35.327177 botocore-a-la-carte-gamelift-1.31.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:35.327177 botocore-a-la-carte-gamelift-1.31.8/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:35.327177 botocore-a-la-carte-gamelift-1.31.8/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:35.327177 botocore-a-la-carte-gamelift-1.31.8/botocore/data/gamelift/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:35.327177 botocore-a-la-carte-gamelift-1.31.8/botocore/data/gamelift/2015-10-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-07-21 01:21:06.000000 botocore-a-la-carte-gamelift-1.31.8/botocore/data/gamelift/2015-10-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 01:21:06.000000 botocore-a-la-carte-gamelift-1.31.8/botocore/data/gamelift/2015-10-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-21 01:21:06.000000 botocore-a-la-carte-gamelift-1.31.8/botocore/data/gamelift/2015-10-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   530402 2023-07-21 01:21:06.000000 botocore-a-la-carte-gamelift-1.31.8/botocore/data/gamelift/2015-10-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:35.327177 botocore-a-la-carte-gamelift-1.31.8/botocore_a_la_carte_gamelift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-21 01:21:35.000000 botocore-a-la-carte-gamelift-1.31.8/botocore_a_la_carte_gamelift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-21 01:21:35.000000 botocore-a-la-carte-gamelift-1.31.8/botocore_a_la_carte_gamelift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:35.000000 botocore-a-la-carte-gamelift-1.31.8/botocore_a_la_carte_gamelift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:35.000000 botocore-a-la-carte-gamelift-1.31.8/botocore_a_la_carte_gamelift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:35.327177 botocore-a-la-carte-gamelift-1.31.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-21 01:21:35.000000 botocore-a-la-carte-gamelift-1.31.8/setup.py
```

### Comparing `botocore-a-la-carte-gamelift-1.31.6/LICENSE.txt` & `botocore-a-la-carte-gamelift-1.31.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-gamelift-1.31.6/PKG-INFO` & `botocore-a-la-carte-gamelift-1.31.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-gamelift
-Version: 1.31.6
+Version: 1.31.8
 Summary: gamelift data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-gamelift-1.31.6/botocore/data/gamelift/2015-10-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-gamelift-1.31.8/botocore/data/gamelift/2015-10-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-gamelift-1.31.6/botocore/data/gamelift/2015-10-01/paginators-1.json` & `botocore-a-la-carte-gamelift-1.31.8/botocore/data/gamelift/2015-10-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-gamelift-1.31.6/botocore/data/gamelift/2015-10-01/service-2.json` & `botocore-a-la-carte-gamelift-1.31.8/botocore/data/gamelift/2015-10-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-gamelift-1.31.6/botocore_a_la_carte_gamelift.egg-info/PKG-INFO` & `botocore-a-la-carte-gamelift-1.31.8/botocore_a_la_carte_gamelift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-gamelift
-Version: 1.31.6
+Version: 1.31.8
 Summary: gamelift data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-gamelift-1.31.6/setup.py` & `botocore-a-la-carte-gamelift-1.31.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-gamelift',
-    version="1.31.6",
+    version="1.31.8",
     description='gamelift data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/gamelift/*/*.json'],
```

