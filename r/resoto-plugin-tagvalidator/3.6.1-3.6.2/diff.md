# Comparing `tmp/resoto-plugin-tagvalidator-3.6.1.tar.gz` & `tmp/resoto-plugin-tagvalidator-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-tagvalidator-3.6.1.tar", last modified: Fri Jul 14 17:00:57 2023, max compression
+gzip compressed data, was "resoto-plugin-tagvalidator-3.6.2.tar", last modified: Fri Jul 21 22:10:57 2023, max compression
```

## Comparing `resoto-plugin-tagvalidator-3.6.1.tar` & `resoto-plugin-tagvalidator-3.6.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:57.682255 resoto-plugin-tagvalidator-3.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 16:55:05.000000 resoto-plugin-tagvalidator-3.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-14 17:00:57.682255 resoto-plugin-tagvalidator-3.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-14 16:55:05.000000 resoto-plugin-tagvalidator-3.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-14 16:55:05.000000 resoto-plugin-tagvalidator-3.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:57.678255 resoto-plugin-tagvalidator-3.6.1/resoto_plugin_tagvalidator/
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-07-14 16:55:05.000000 resoto-plugin-tagvalidator-3.6.1/resoto_plugin_tagvalidator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-14 16:55:05.000000 resoto-plugin-tagvalidator-3.6.1/resoto_plugin_tagvalidator/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:57.678255 resoto-plugin-tagvalidator-3.6.1/resoto_plugin_tagvalidator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-14 17:00:57.000000 resoto-plugin-tagvalidator-3.6.1/resoto_plugin_tagvalidator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-14 17:00:57.000000 resoto-plugin-tagvalidator-3.6.1/resoto_plugin_tagvalidator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:00:57.000000 resoto-plugin-tagvalidator-3.6.1/resoto_plugin_tagvalidator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-14 17:00:57.000000 resoto-plugin-tagvalidator-3.6.1/resoto_plugin_tagvalidator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:56:56.000000 resoto-plugin-tagvalidator-3.6.1/resoto_plugin_tagvalidator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 17:00:57.000000 resoto-plugin-tagvalidator-3.6.1/resoto_plugin_tagvalidator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-14 17:00:57.000000 resoto-plugin-tagvalidator-3.6.1/resoto_plugin_tagvalidator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-14 17:00:57.682255 resoto-plugin-tagvalidator-3.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:57.682255 resoto-plugin-tagvalidator-3.6.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-14 16:55:05.000000 resoto-plugin-tagvalidator-3.6.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:57.221335 resoto-plugin-tagvalidator-3.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 22:06:12.000000 resoto-plugin-tagvalidator-3.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-21 22:10:57.221335 resoto-plugin-tagvalidator-3.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-21 22:06:12.000000 resoto-plugin-tagvalidator-3.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-21 22:06:12.000000 resoto-plugin-tagvalidator-3.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:57.217335 resoto-plugin-tagvalidator-3.6.2/resoto_plugin_tagvalidator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-07-21 22:06:12.000000 resoto-plugin-tagvalidator-3.6.2/resoto_plugin_tagvalidator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-21 22:06:12.000000 resoto-plugin-tagvalidator-3.6.2/resoto_plugin_tagvalidator/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:57.221335 resoto-plugin-tagvalidator-3.6.2/resoto_plugin_tagvalidator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-21 22:10:57.000000 resoto-plugin-tagvalidator-3.6.2/resoto_plugin_tagvalidator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-21 22:10:57.000000 resoto-plugin-tagvalidator-3.6.2/resoto_plugin_tagvalidator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:10:57.000000 resoto-plugin-tagvalidator-3.6.2/resoto_plugin_tagvalidator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-21 22:10:57.000000 resoto-plugin-tagvalidator-3.6.2/resoto_plugin_tagvalidator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:07:41.000000 resoto-plugin-tagvalidator-3.6.2/resoto_plugin_tagvalidator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 22:10:57.000000 resoto-plugin-tagvalidator-3.6.2/resoto_plugin_tagvalidator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-21 22:10:57.000000 resoto-plugin-tagvalidator-3.6.2/resoto_plugin_tagvalidator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 22:10:57.221335 resoto-plugin-tagvalidator-3.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:10:57.221335 resoto-plugin-tagvalidator-3.6.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-21 22:06:12.000000 resoto-plugin-tagvalidator-3.6.2/test/test_config.py
```

### Comparing `resoto-plugin-tagvalidator-3.6.1/PKG-INFO` & `resoto-plugin-tagvalidator-3.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-tagvalidator
-Version: 3.6.1
+Version: 3.6.2
 Summary: Resoto Tag Validator Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/tagvalidator
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-tagvalidator-3.6.1/README.md` & `resoto-plugin-tagvalidator-3.6.2/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-tagvalidator-3.6.1/pyproject.toml` & `resoto-plugin-tagvalidator-3.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-tagvalidator"
 description = "Resoto Tag Validator Plugin"
-version = "3.6.1"
+version = "3.6.2"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.6.1",
+    "resotolib==3.6.2",
 ]
 
 [project.entry-points."resoto.plugins"]
 tagvalidator = "resoto_plugin_tagvalidator:TagValidatorPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
```

### Comparing `resoto-plugin-tagvalidator-3.6.1/resoto_plugin_tagvalidator/__init__.py` & `resoto-plugin-tagvalidator-3.6.2/resoto_plugin_tagvalidator/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-tagvalidator-3.6.1/resoto_plugin_tagvalidator/config.py` & `resoto-plugin-tagvalidator-3.6.2/resoto_plugin_tagvalidator/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-tagvalidator-3.6.1/resoto_plugin_tagvalidator.egg-info/PKG-INFO` & `resoto-plugin-tagvalidator-3.6.2/resoto_plugin_tagvalidator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-tagvalidator
-Version: 3.6.1
+Version: 3.6.2
 Summary: Resoto Tag Validator Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/tagvalidator
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-tagvalidator-3.6.1/test/test_config.py` & `resoto-plugin-tagvalidator-3.6.2/test/test_config.py`

 * *Files identical despite different names*

