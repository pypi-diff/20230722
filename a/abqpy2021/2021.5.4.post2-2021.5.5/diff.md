# Comparing `tmp/abqpy2021-2021.5.4.post2.tar.gz` & `tmp/abqpy2021-2021.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abqpy2021-2021.5.4.post2.tar", last modified: Wed Jul 12 11:48:16 2023, max compression
+gzip compressed data, was "abqpy2021-2021.5.5.tar", last modified: Sat Jul 22 07:25:17 2023, max compression
```

## Comparing `abqpy2021-2021.5.4.post2.tar` & `abqpy2021-2021.5.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:48:16.162002 abqpy2021-2021.5.4.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-12 11:48:16.162002 abqpy2021-2021.5.4.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-12 11:48:04.000000 abqpy2021-2021.5.4.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:48:16.162002 abqpy2021-2021.5.4.post2/abqpy2021.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-12 11:48:16.000000 abqpy2021-2021.5.4.post2/abqpy2021.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-12 11:48:16.000000 abqpy2021-2021.5.4.post2/abqpy2021.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 11:48:16.000000 abqpy2021-2021.5.4.post2/abqpy2021.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 11:48:16.000000 abqpy2021-2021.5.4.post2/abqpy2021.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 11:48:16.000000 abqpy2021-2021.5.4.post2/abqpy2021.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-12 11:48:04.000000 abqpy2021-2021.5.4.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 11:48:16.162002 abqpy2021-2021.5.4.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-12 11:48:04.000000 abqpy2021-2021.5.4.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 07:25:17.253271 abqpy2021-2021.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-22 07:25:17.249271 abqpy2021-2021.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-22 07:25:04.000000 abqpy2021-2021.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 07:25:17.249271 abqpy2021-2021.5.5/abqpy2021.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-22 07:25:17.000000 abqpy2021-2021.5.5/abqpy2021.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-22 07:25:17.000000 abqpy2021-2021.5.5/abqpy2021.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 07:25:17.000000 abqpy2021-2021.5.5/abqpy2021.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-22 07:25:17.000000 abqpy2021-2021.5.5/abqpy2021.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 07:25:17.000000 abqpy2021-2021.5.5/abqpy2021.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-22 07:25:04.000000 abqpy2021-2021.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 07:25:17.253271 abqpy2021-2021.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-22 07:25:04.000000 abqpy2021-2021.5.5/setup.py
```

### Comparing `abqpy2021-2021.5.4.post2/PKG-INFO` & `abqpy2021-2021.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abqpy2021
-Version: 2021.5.4.post2
+Version: 2021.5.5
 Summary: Type hints for Abaqus/Python scripting
 Author-email: WANG Hailin <hailin.wang@connect.polyu.hk>
 Project-URL: Homepage, https://abqpy.com
 Project-URL: GitHub, https://github.com/haiiliin/abqpy
 Project-URL: Bug Tracker, https://github.com/haiiliin/abqpy/issues
 Project-URL: Read the Docs, https://readthedocs.org/projects/abqpy
 Project-URL: Documentation, https://docs.abqpy.com/en/stable/
```

### Comparing `abqpy2021-2021.5.4.post2/abqpy2021.egg-info/PKG-INFO` & `abqpy2021-2021.5.5/abqpy2021.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abqpy2021
-Version: 2021.5.4.post2
+Version: 2021.5.5
 Summary: Type hints for Abaqus/Python scripting
 Author-email: WANG Hailin <hailin.wang@connect.polyu.hk>
 Project-URL: Homepage, https://abqpy.com
 Project-URL: GitHub, https://github.com/haiiliin/abqpy
 Project-URL: Bug Tracker, https://github.com/haiiliin/abqpy/issues
 Project-URL: Read the Docs, https://readthedocs.org/projects/abqpy
 Project-URL: Documentation, https://docs.abqpy.com/en/stable/
```

### Comparing `abqpy2021-2021.5.4.post2/pyproject.toml` & `abqpy2021-2021.5.5/pyproject.toml`

 * *Files identical despite different names*

