# Comparing `tmp/resoto-plugin-cleanup-aws-vpcs-3.6.1.tar.gz` & `tmp/resoto-plugin-cleanup-aws-vpcs-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-aws-vpcs-3.6.1.tar", last modified: Fri Jul 14 17:04:01 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-aws-vpcs-3.6.2.tar", last modified: Fri Jul 21 22:10:19 2023, max compression
```

## Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.1.tar` & `resoto-plugin-cleanup-aws-vpcs-3.6.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:04:01.250792 resoto-plugin-cleanup-aws-vpcs-3.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 17:00:19.000000 resoto-plugin-cleanup-aws-vpcs-3.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-14 17:04:01.250792 resoto-plugin-cleanup-aws-vpcs-3.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-14 17:00:19.000000 resoto-plugin-cleanup-aws-vpcs-3.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-14 17:00:19.000000 resoto-plugin-cleanup-aws-vpcs-3.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:04:01.250792 resoto-plugin-cleanup-aws-vpcs-3.6.1/resoto_plugin_cleanup_aws_vpcs/
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-14 17:00:19.000000 resoto-plugin-cleanup-aws-vpcs-3.6.1/resoto_plugin_cleanup_aws_vpcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-14 17:00:19.000000 resoto-plugin-cleanup-aws-vpcs-3.6.1/resoto_plugin_cleanup_aws_vpcs/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:04:01.250792 resoto-plugin-cleanup-aws-vpcs-3.6.1/resoto_plugin_cleanup_aws_vpcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-14 17:04:01.000000 resoto-plugin-cleanup-aws-vpcs-3.6.1/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-14 17:04:01.000000 resoto-plugin-cleanup-aws-vpcs-3.6.1/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:04:01.000000 resoto-plugin-cleanup-aws-vpcs-3.6.1/resoto_plugin_cleanup_aws_vpcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-14 17:04:01.000000 resoto-plugin-cleanup-aws-vpcs-3.6.1/resoto_plugin_cleanup_aws_vpcs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:01:50.000000 resoto-plugin-cleanup-aws-vpcs-3.6.1/resoto_plugin_cleanup_aws_vpcs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-14 17:04:01.000000 resoto-plugin-cleanup-aws-vpcs-3.6.1/resoto_plugin_cleanup_aws_vpcs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-14 17:04:01.000000 resoto-plugin-cleanup-aws-vpcs-3.6.1/resoto_plugin_cleanup_aws_vpcs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-14 17:04:01.254792 resoto-plugin-cleanup-aws-vpcs-3.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:04:01.250792 resoto-plugin-cleanup-aws-vpcs-3.6.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-14 17:00:19.000000 resoto-plugin-cleanup-aws-vpcs-3.6.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:19.520438 resoto-plugin-cleanup-aws-vpcs-3.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 22:06:10.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-21 22:10:19.520438 resoto-plugin-cleanup-aws-vpcs-3.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-21 22:06:10.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-21 22:06:10.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:19.516438 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-21 22:06:10.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-21 22:06:10.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:19.520438 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-21 22:10:19.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-21 22:10:19.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:10:19.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-21 22:10:19.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:07:50.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-21 22:10:19.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-21 22:10:19.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 22:10:19.520438 resoto-plugin-cleanup-aws-vpcs-3.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:19.520438 resoto-plugin-cleanup-aws-vpcs-3.6.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-21 22:06:10.000000 resoto-plugin-cleanup-aws-vpcs-3.6.2/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.1/PKG-INFO` & `resoto-plugin-cleanup-aws-vpcs-3.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-vpcs
-Version: 3.6.1
+Version: 3.6.2
 Summary: AWS VPC Cleaner Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_vpcs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.1/README.md` & `resoto-plugin-cleanup-aws-vpcs-3.6.2/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.1/pyproject.toml` & `resoto-plugin-cleanup-aws-vpcs-3.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-cleanup-aws-vpcs"
 description = "AWS VPC Cleaner Plugin"
-version = "3.6.1"
+version = "3.6.2"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,16 +23,16 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.6.1",
-    "resoto-plugin-aws==3.6.1"
+    "resotolib==3.6.2",
+    "resoto-plugin-aws==3.6.2"
 ]
 
 [project.entry-points."resoto.plugins"]
 cleanup_aws_vpcs = "resoto_plugin_cleanup_aws_vpcs:CleanupAWSVPCsPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.1/resoto_plugin_cleanup_aws_vpcs/__init__.py` & `resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.1/resoto_plugin_cleanup_aws_vpcs/config.py` & `resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.1/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO` & `resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-vpcs
-Version: 3.6.1
+Version: 3.6.2
 Summary: AWS VPC Cleaner Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_vpcs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-vpcs-3.6.1/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-aws-vpcs-3.6.2/resoto_plugin_cleanup_aws_vpcs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

