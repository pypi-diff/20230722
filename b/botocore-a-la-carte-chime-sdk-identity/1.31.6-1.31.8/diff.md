# Comparing `tmp/botocore-a-la-carte-chime-sdk-identity-1.31.6.tar.gz` & `tmp/botocore-a-la-carte-chime-sdk-identity-1.31.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-chime-sdk-identity-1.31.6.tar", last modified: Thu Jul 20 01:20:12 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-chime-sdk-identity-1.31.8.tar", last modified: Fri Jul 21 01:21:20 2023, max compression
```

## Comparing `botocore-a-la-carte-chime-sdk-identity-1.31.6.tar` & `botocore-a-la-carte-chime-sdk-identity-1.31.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:12.246615 botocore-a-la-carte-chime-sdk-identity-1.31.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-20 01:20:12.000000 botocore-a-la-carte-chime-sdk-identity-1.31.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-20 01:20:12.246615 botocore-a-la-carte-chime-sdk-identity-1.31.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:12.242614 botocore-a-la-carte-chime-sdk-identity-1.31.6/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:12.242614 botocore-a-la-carte-chime-sdk-identity-1.31.6/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:12.242614 botocore-a-la-carte-chime-sdk-identity-1.31.6/botocore/data/chime-sdk-identity/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:12.242614 botocore-a-la-carte-chime-sdk-identity-1.31.6/botocore/data/chime-sdk-identity/2021-04-20/
--rw-r--r--   0 runner    (1001) docker     (123)    17656 2023-07-20 01:19:55.000000 botocore-a-la-carte-chime-sdk-identity-1.31.6/botocore/data/chime-sdk-identity/2021-04-20/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 01:19:55.000000 botocore-a-la-carte-chime-sdk-identity-1.31.6/botocore/data/chime-sdk-identity/2021-04-20/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 01:19:55.000000 botocore-a-la-carte-chime-sdk-identity-1.31.6/botocore/data/chime-sdk-identity/2021-04-20/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    80477 2023-07-20 01:19:55.000000 botocore-a-la-carte-chime-sdk-identity-1.31.6/botocore/data/chime-sdk-identity/2021-04-20/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:12.246615 botocore-a-la-carte-chime-sdk-identity-1.31.6/botocore_a_la_carte_chime_sdk_identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-20 01:20:12.000000 botocore-a-la-carte-chime-sdk-identity-1.31.6/botocore_a_la_carte_chime_sdk_identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-20 01:20:12.000000 botocore-a-la-carte-chime-sdk-identity-1.31.6/botocore_a_la_carte_chime_sdk_identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 01:20:12.000000 botocore-a-la-carte-chime-sdk-identity-1.31.6/botocore_a_la_carte_chime_sdk_identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 01:20:12.000000 botocore-a-la-carte-chime-sdk-identity-1.31.6/botocore_a_la_carte_chime_sdk_identity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 01:20:12.246615 botocore-a-la-carte-chime-sdk-identity-1.31.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-20 01:20:12.000000 botocore-a-la-carte-chime-sdk-identity-1.31.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:20.934918 botocore-a-la-carte-chime-sdk-identity-1.31.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:20.000000 botocore-a-la-carte-chime-sdk-identity-1.31.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-21 01:21:20.934918 botocore-a-la-carte-chime-sdk-identity-1.31.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:20.930918 botocore-a-la-carte-chime-sdk-identity-1.31.8/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:20.930918 botocore-a-la-carte-chime-sdk-identity-1.31.8/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:20.930918 botocore-a-la-carte-chime-sdk-identity-1.31.8/botocore/data/chime-sdk-identity/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:20.934918 botocore-a-la-carte-chime-sdk-identity-1.31.8/botocore/data/chime-sdk-identity/2021-04-20/
+-rw-r--r--   0 runner    (1001) docker     (123)    17656 2023-07-21 01:21:06.000000 botocore-a-la-carte-chime-sdk-identity-1.31.8/botocore/data/chime-sdk-identity/2021-04-20/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 01:21:06.000000 botocore-a-la-carte-chime-sdk-identity-1.31.8/botocore/data/chime-sdk-identity/2021-04-20/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 01:21:06.000000 botocore-a-la-carte-chime-sdk-identity-1.31.8/botocore/data/chime-sdk-identity/2021-04-20/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    80477 2023-07-21 01:21:06.000000 botocore-a-la-carte-chime-sdk-identity-1.31.8/botocore/data/chime-sdk-identity/2021-04-20/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:20.934918 botocore-a-la-carte-chime-sdk-identity-1.31.8/botocore_a_la_carte_chime_sdk_identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-21 01:21:20.000000 botocore-a-la-carte-chime-sdk-identity-1.31.8/botocore_a_la_carte_chime_sdk_identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-21 01:21:20.000000 botocore-a-la-carte-chime-sdk-identity-1.31.8/botocore_a_la_carte_chime_sdk_identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:20.000000 botocore-a-la-carte-chime-sdk-identity-1.31.8/botocore_a_la_carte_chime_sdk_identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:20.000000 botocore-a-la-carte-chime-sdk-identity-1.31.8/botocore_a_la_carte_chime_sdk_identity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:20.934918 botocore-a-la-carte-chime-sdk-identity-1.31.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-21 01:21:20.000000 botocore-a-la-carte-chime-sdk-identity-1.31.8/setup.py
```

### Comparing `botocore-a-la-carte-chime-sdk-identity-1.31.6/LICENSE.txt` & `botocore-a-la-carte-chime-sdk-identity-1.31.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-chime-sdk-identity-1.31.6/PKG-INFO` & `botocore-a-la-carte-chime-sdk-identity-1.31.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-chime-sdk-identity
-Version: 1.31.6
+Version: 1.31.8
 Summary: chime-sdk-identity data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-chime-sdk-identity-1.31.6/botocore/data/chime-sdk-identity/2021-04-20/endpoint-rule-set-1.json` & `botocore-a-la-carte-chime-sdk-identity-1.31.8/botocore/data/chime-sdk-identity/2021-04-20/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-chime-sdk-identity-1.31.6/botocore/data/chime-sdk-identity/2021-04-20/service-2.json` & `botocore-a-la-carte-chime-sdk-identity-1.31.8/botocore/data/chime-sdk-identity/2021-04-20/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-chime-sdk-identity-1.31.6/botocore_a_la_carte_chime_sdk_identity.egg-info/PKG-INFO` & `botocore-a-la-carte-chime-sdk-identity-1.31.8/botocore_a_la_carte_chime_sdk_identity.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-chime-sdk-identity
-Version: 1.31.6
+Version: 1.31.8
 Summary: chime-sdk-identity data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-chime-sdk-identity-1.31.6/botocore_a_la_carte_chime_sdk_identity.egg-info/SOURCES.txt` & `botocore-a-la-carte-chime-sdk-identity-1.31.8/botocore_a_la_carte_chime_sdk_identity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-chime-sdk-identity-1.31.6/setup.py` & `botocore-a-la-carte-chime-sdk-identity-1.31.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-chime-sdk-identity',
-    version="1.31.6",
+    version="1.31.8",
     description='chime-sdk-identity data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/chime-sdk-identity/*/*.json'],
```

