# Comparing `tmp/abqpy2016-2016.5.4.post2.tar.gz` & `tmp/abqpy2016-2016.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abqpy2016-2016.5.4.post2.tar", last modified: Wed Jul 12 11:48:50 2023, max compression
+gzip compressed data, was "abqpy2016-2016.5.5.tar", last modified: Sat Jul 22 07:24:24 2023, max compression
```

## Comparing `abqpy2016-2016.5.4.post2.tar` & `abqpy2016-2016.5.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:48:50.610791 abqpy2016-2016.5.4.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-12 11:48:50.610791 abqpy2016-2016.5.4.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-12 11:48:38.000000 abqpy2016-2016.5.4.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:48:50.610791 abqpy2016-2016.5.4.post2/abqpy2016.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-12 11:48:50.000000 abqpy2016-2016.5.4.post2/abqpy2016.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-12 11:48:50.000000 abqpy2016-2016.5.4.post2/abqpy2016.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 11:48:50.000000 abqpy2016-2016.5.4.post2/abqpy2016.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 11:48:50.000000 abqpy2016-2016.5.4.post2/abqpy2016.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 11:48:50.000000 abqpy2016-2016.5.4.post2/abqpy2016.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-12 11:48:38.000000 abqpy2016-2016.5.4.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 11:48:50.610791 abqpy2016-2016.5.4.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-12 11:48:38.000000 abqpy2016-2016.5.4.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 07:24:24.071047 abqpy2016-2016.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-22 07:24:24.071047 abqpy2016-2016.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-22 07:24:07.000000 abqpy2016-2016.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 07:24:24.071047 abqpy2016-2016.5.5/abqpy2016.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-22 07:24:23.000000 abqpy2016-2016.5.5/abqpy2016.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-22 07:24:24.000000 abqpy2016-2016.5.5/abqpy2016.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 07:24:23.000000 abqpy2016-2016.5.5/abqpy2016.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-22 07:24:23.000000 abqpy2016-2016.5.5/abqpy2016.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 07:24:23.000000 abqpy2016-2016.5.5/abqpy2016.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-22 07:24:07.000000 abqpy2016-2016.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 07:24:24.071047 abqpy2016-2016.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-22 07:24:07.000000 abqpy2016-2016.5.5/setup.py
```

### Comparing `abqpy2016-2016.5.4.post2/PKG-INFO` & `abqpy2016-2016.5.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abqpy2016
-Version: 2016.5.4.post2
+Version: 2016.5.5
 Summary: Type hints for Abaqus/Python scripting
 Author-email: WANG Hailin <hailin.wang@connect.polyu.hk>
 Project-URL: Homepage, https://abqpy.com
 Project-URL: GitHub, https://github.com/haiiliin/abqpy
 Project-URL: Bug Tracker, https://github.com/haiiliin/abqpy/issues
 Project-URL: Read the Docs, https://readthedocs.org/projects/abqpy
 Project-URL: Documentation, https://docs.abqpy.com/en/stable/
```

### Comparing `abqpy2016-2016.5.4.post2/abqpy2016.egg-info/PKG-INFO` & `abqpy2016-2016.5.5/abqpy2016.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abqpy2016
-Version: 2016.5.4.post2
+Version: 2016.5.5
 Summary: Type hints for Abaqus/Python scripting
 Author-email: WANG Hailin <hailin.wang@connect.polyu.hk>
 Project-URL: Homepage, https://abqpy.com
 Project-URL: GitHub, https://github.com/haiiliin/abqpy
 Project-URL: Bug Tracker, https://github.com/haiiliin/abqpy/issues
 Project-URL: Read the Docs, https://readthedocs.org/projects/abqpy
 Project-URL: Documentation, https://docs.abqpy.com/en/stable/
```

### Comparing `abqpy2016-2016.5.4.post2/pyproject.toml` & `abqpy2016-2016.5.5/pyproject.toml`

 * *Files identical despite different names*

