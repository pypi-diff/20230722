# Comparing `tmp/cdk-ecs-service-extensions-2.0.1a92.tar.gz` & `tmp/cdk-ecs-service-extensions-2.0.1a93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-ecs-service-extensions-2.0.1a92.tar", last modified: Thu Jul 20 00:31:49 2023, max compression
+gzip compressed data, was "cdk-ecs-service-extensions-2.0.1a93.tar", last modified: Fri Jul 21 00:29:37 2023, max compression
```

## Comparing `cdk-ecs-service-extensions-2.0.1a92.tar` & `cdk-ecs-service-extensions-2.0.1a93.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:31:49.301456 cdk-ecs-service-extensions-2.0.1a92/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-20 00:31:33.000000 cdk-ecs-service-extensions-2.0.1a92/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 00:31:33.000000 cdk-ecs-service-extensions-2.0.1a92/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-20 00:31:33.000000 cdk-ecs-service-extensions-2.0.1a92/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    25295 2023-07-20 00:31:49.301456 cdk-ecs-service-extensions-2.0.1a92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24273 2023-07-20 00:31:33.000000 cdk-ecs-service-extensions-2.0.1a92/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-20 00:31:33.000000 cdk-ecs-service-extensions-2.0.1a92/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 00:31:49.301456 cdk-ecs-service-extensions-2.0.1a92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-20 00:31:33.000000 cdk-ecs-service-extensions-2.0.1a92/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:31:49.297456 cdk-ecs-service-extensions-2.0.1a92/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:31:49.301456 cdk-ecs-service-extensions-2.0.1a92/src/cdk_ecs_service_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)   295093 2023-07-20 00:31:33.000000 cdk-ecs-service-extensions-2.0.1a92/src/cdk_ecs_service_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:31:49.301456 cdk-ecs-service-extensions-2.0.1a92/src/cdk_ecs_service_extensions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-20 00:31:33.000000 cdk-ecs-service-extensions-2.0.1a92/src/cdk_ecs_service_extensions/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   172615 2023-07-20 00:31:33.000000 cdk-ecs-service-extensions-2.0.1a92/src/cdk_ecs_service_extensions/_jsii/ecs-service-extensions@2.0.1-alpha.92.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 00:31:33.000000 cdk-ecs-service-extensions-2.0.1a92/src/cdk_ecs_service_extensions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 00:31:49.301456 cdk-ecs-service-extensions-2.0.1a92/src/cdk_ecs_service_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25295 2023-07-20 00:31:49.000000 cdk-ecs-service-extensions-2.0.1a92/src/cdk_ecs_service_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-20 00:31:49.000000 cdk-ecs-service-extensions-2.0.1a92/src/cdk_ecs_service_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 00:31:49.000000 cdk-ecs-service-extensions-2.0.1a92/src/cdk_ecs_service_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 00:31:49.000000 cdk-ecs-service-extensions-2.0.1a92/src/cdk_ecs_service_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-20 00:31:49.000000 cdk-ecs-service-extensions-2.0.1a92/src/cdk_ecs_service_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:29:37.277577 cdk-ecs-service-extensions-2.0.1a93/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-21 00:29:25.000000 cdk-ecs-service-extensions-2.0.1a93/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 00:29:25.000000 cdk-ecs-service-extensions-2.0.1a93/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-21 00:29:25.000000 cdk-ecs-service-extensions-2.0.1a93/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    25295 2023-07-21 00:29:37.277577 cdk-ecs-service-extensions-2.0.1a93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24273 2023-07-21 00:29:25.000000 cdk-ecs-service-extensions-2.0.1a93/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-21 00:29:25.000000 cdk-ecs-service-extensions-2.0.1a93/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 00:29:37.277577 cdk-ecs-service-extensions-2.0.1a93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-21 00:29:25.000000 cdk-ecs-service-extensions-2.0.1a93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:29:37.277577 cdk-ecs-service-extensions-2.0.1a93/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:29:37.277577 cdk-ecs-service-extensions-2.0.1a93/src/cdk_ecs_service_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)   295093 2023-07-21 00:29:25.000000 cdk-ecs-service-extensions-2.0.1a93/src/cdk_ecs_service_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:29:37.277577 cdk-ecs-service-extensions-2.0.1a93/src/cdk_ecs_service_extensions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-21 00:29:25.000000 cdk-ecs-service-extensions-2.0.1a93/src/cdk_ecs_service_extensions/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   172611 2023-07-21 00:29:25.000000 cdk-ecs-service-extensions-2.0.1a93/src/cdk_ecs_service_extensions/_jsii/ecs-service-extensions@2.0.1-alpha.93.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 00:29:25.000000 cdk-ecs-service-extensions-2.0.1a93/src/cdk_ecs_service_extensions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:29:37.277577 cdk-ecs-service-extensions-2.0.1a93/src/cdk_ecs_service_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25295 2023-07-21 00:29:37.000000 cdk-ecs-service-extensions-2.0.1a93/src/cdk_ecs_service_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-21 00:29:37.000000 cdk-ecs-service-extensions-2.0.1a93/src/cdk_ecs_service_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 00:29:37.000000 cdk-ecs-service-extensions-2.0.1a93/src/cdk_ecs_service_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-21 00:29:37.000000 cdk-ecs-service-extensions-2.0.1a93/src/cdk_ecs_service_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-21 00:29:37.000000 cdk-ecs-service-extensions-2.0.1a93/src/cdk_ecs_service_extensions.egg-info/top_level.txt
```

### Comparing `cdk-ecs-service-extensions-2.0.1a92/LICENSE` & `cdk-ecs-service-extensions-2.0.1a93/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-ecs-service-extensions-2.0.1a92/PKG-INFO` & `cdk-ecs-service-extensions-2.0.1a93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-ecs-service-extensions
-Version: 2.0.1a92
+Version: 2.0.1a93
 Summary: The CDK Construct Library that helps you build ECS services using simple extensions
 Home-page: https://github.com/cdklabs/cdk-ecs-service-extensions.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-ecs-service-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-ecs-service-extensions-2.0.1a92/README.md` & `cdk-ecs-service-extensions-2.0.1a93/README.md`

 * *Files identical despite different names*

### Comparing `cdk-ecs-service-extensions-2.0.1a92/setup.py` & `cdk-ecs-service-extensions-2.0.1a93/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-ecs-service-extensions",
-    "version": "2.0.1.a92",
+    "version": "2.0.1.a93",
     "description": "The CDK Construct Library that helps you build ECS services using simple extensions",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-ecs-service-extensions.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_ecs_service_extensions",
         "cdk_ecs_service_extensions._jsii"
     ],
     "package_data": {
         "cdk_ecs_service_extensions._jsii": [
-            "ecs-service-extensions@2.0.1-alpha.92.jsii.tgz"
+            "ecs-service-extensions@2.0.1-alpha.93.jsii.tgz"
         ],
         "cdk_ecs_service_extensions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-ecs-service-extensions-2.0.1a92/src/cdk_ecs_service_extensions/__init__.py` & `cdk-ecs-service-extensions-2.0.1a93/src/cdk_ecs_service_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-ecs-service-extensions-2.0.1a92/src/cdk_ecs_service_extensions.egg-info/PKG-INFO` & `cdk-ecs-service-extensions-2.0.1a93/src/cdk_ecs_service_extensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-ecs-service-extensions
-Version: 2.0.1a92
+Version: 2.0.1a93
 Summary: The CDK Construct Library that helps you build ECS services using simple extensions
 Home-page: https://github.com/cdklabs/cdk-ecs-service-extensions.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-ecs-service-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-ecs-service-extensions-2.0.1a92/src/cdk_ecs_service_extensions.egg-info/SOURCES.txt` & `cdk-ecs-service-extensions-2.0.1a93/src/cdk_ecs_service_extensions.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/cdk_ecs_service_extensions/py.typed
 src/cdk_ecs_service_extensions.egg-info/PKG-INFO
 src/cdk_ecs_service_extensions.egg-info/SOURCES.txt
 src/cdk_ecs_service_extensions.egg-info/dependency_links.txt
 src/cdk_ecs_service_extensions.egg-info/requires.txt
 src/cdk_ecs_service_extensions.egg-info/top_level.txt
 src/cdk_ecs_service_extensions/_jsii/__init__.py
-src/cdk_ecs_service_extensions/_jsii/ecs-service-extensions@2.0.1-alpha.92.jsii.tgz
+src/cdk_ecs_service_extensions/_jsii/ecs-service-extensions@2.0.1-alpha.93.jsii.tgz
```

