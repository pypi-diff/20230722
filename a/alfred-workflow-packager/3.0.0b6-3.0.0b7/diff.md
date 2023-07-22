# Comparing `tmp/alfred-workflow-packager-3.0.0b6.tar.gz` & `tmp/alfred-workflow-packager-3.0.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred-workflow-packager-3.0.0b6.tar", last modified: Sat Jul 22 20:35:53 2023, max compression
+gzip compressed data, was "alfred-workflow-packager-3.0.0b7.tar", last modified: Sat Jul 22 20:39:22 2023, max compression
```

## Comparing `alfred-workflow-packager-3.0.0b6.tar` & `alfred-workflow-packager-3.0.0b7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:35:53.508929 alfred-workflow-packager-3.0.0b6/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-22 20:35:40.000000 alfred-workflow-packager-3.0.0b6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-22 20:35:53.508929 alfred-workflow-packager-3.0.0b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-22 20:35:40.000000 alfred-workflow-packager-3.0.0b6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:35:53.504929 alfred-workflow-packager-3.0.0b6/alfred_workflow_packager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-22 20:35:53.000000 alfred-workflow-packager-3.0.0b6/alfred_workflow_packager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-22 20:35:53.000000 alfred-workflow-packager-3.0.0b6/alfred_workflow_packager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 20:35:53.000000 alfred-workflow-packager-3.0.0b6/alfred_workflow_packager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 20:35:53.000000 alfred-workflow-packager-3.0.0b6/alfred_workflow_packager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-22 20:35:53.000000 alfred-workflow-packager-3.0.0b6/alfred_workflow_packager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-22 20:35:53.000000 alfred-workflow-packager-3.0.0b6/alfred_workflow_packager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:35:53.508929 alfred-workflow-packager-3.0.0b6/awp/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 20:35:40.000000 alfred-workflow-packager-3.0.0b6/awp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-22 20:35:40.000000 alfred-workflow-packager-3.0.0b6/awp/argparse_extras.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-22 20:35:40.000000 alfred-workflow-packager-3.0.0b6/awp/main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9375 2023-07-22 20:35:40.000000 alfred-workflow-packager-3.0.0b6/awp/packager.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-22 20:35:40.000000 alfred-workflow-packager-3.0.0b6/awp/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-22 20:35:40.000000 alfred-workflow-packager-3.0.0b6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 20:35:53.508929 alfred-workflow-packager-3.0.0b6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-22 20:35:40.000000 alfred-workflow-packager-3.0.0b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:39:22.331221 alfred-workflow-packager-3.0.0b7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-22 20:39:07.000000 alfred-workflow-packager-3.0.0b7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-22 20:39:22.331221 alfred-workflow-packager-3.0.0b7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-22 20:39:07.000000 alfred-workflow-packager-3.0.0b7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:39:22.331221 alfred-workflow-packager-3.0.0b7/alfred_workflow_packager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-22 20:39:22.000000 alfred-workflow-packager-3.0.0b7/alfred_workflow_packager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-22 20:39:22.000000 alfred-workflow-packager-3.0.0b7/alfred_workflow_packager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 20:39:22.000000 alfred-workflow-packager-3.0.0b7/alfred_workflow_packager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 20:39:22.000000 alfred-workflow-packager-3.0.0b7/alfred_workflow_packager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-22 20:39:22.000000 alfred-workflow-packager-3.0.0b7/alfred_workflow_packager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-22 20:39:22.000000 alfred-workflow-packager-3.0.0b7/alfred_workflow_packager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:39:22.331221 alfred-workflow-packager-3.0.0b7/awp/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 20:39:07.000000 alfred-workflow-packager-3.0.0b7/awp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-22 20:39:07.000000 alfred-workflow-packager-3.0.0b7/awp/argparse_extras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-22 20:39:07.000000 alfred-workflow-packager-3.0.0b7/awp/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9375 2023-07-22 20:39:07.000000 alfred-workflow-packager-3.0.0b7/awp/packager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-22 20:39:07.000000 alfred-workflow-packager-3.0.0b7/awp/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-22 20:39:07.000000 alfred-workflow-packager-3.0.0b7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 20:39:22.331221 alfred-workflow-packager-3.0.0b7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-22 20:39:07.000000 alfred-workflow-packager-3.0.0b7/setup.py
```

### Comparing `alfred-workflow-packager-3.0.0b6/LICENSE.txt` & `alfred-workflow-packager-3.0.0b7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alfred-workflow-packager-3.0.0b6/PKG-INFO` & `alfred-workflow-packager-3.0.0b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred-workflow-packager
-Version: 3.0.0b6
+Version: 3.0.0b7
 Summary: A CLI utility for packaging and exporting Alfred workflows
 Author-email: Caleb Evans <caleb@calebevans.me>
 Maintainer-email: Caleb Evans <caleb@calebevans.me>
 License: The MIT License (MIT)
         
         Copyright (c) 2016-2022 Caleb Evans
```

### Comparing `alfred-workflow-packager-3.0.0b6/README.md` & `alfred-workflow-packager-3.0.0b7/README.md`

 * *Files identical despite different names*

### Comparing `alfred-workflow-packager-3.0.0b6/alfred_workflow_packager.egg-info/PKG-INFO` & `alfred-workflow-packager-3.0.0b7/alfred_workflow_packager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred-workflow-packager
-Version: 3.0.0b6
+Version: 3.0.0b7
 Summary: A CLI utility for packaging and exporting Alfred workflows
 Author-email: Caleb Evans <caleb@calebevans.me>
 Maintainer-email: Caleb Evans <caleb@calebevans.me>
 License: The MIT License (MIT)
         
         Copyright (c) 2016-2022 Caleb Evans
```

### Comparing `alfred-workflow-packager-3.0.0b6/awp/argparse_extras.py` & `alfred-workflow-packager-3.0.0b7/awp/argparse_extras.py`

 * *Files identical despite different names*

### Comparing `alfred-workflow-packager-3.0.0b6/awp/main.py` & `alfred-workflow-packager-3.0.0b7/awp/main.py`

 * *Files identical despite different names*

### Comparing `alfred-workflow-packager-3.0.0b6/awp/packager.py` & `alfred-workflow-packager-3.0.0b7/awp/packager.py`

 * *Files identical despite different names*

### Comparing `alfred-workflow-packager-3.0.0b6/pyproject.toml` & `alfred-workflow-packager-3.0.0b7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "alfred-workflow-packager"
-version = "3.0.0-beta.6"
+version = "3.0.0-beta.7"
 description = "A CLI utility for packaging and exporting Alfred workflows"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
     { name = "Caleb Evans", email = "caleb@calebevans.me" }
 ]
 maintainers = [
```

