# Comparing `tmp/abqpy2023-0.0.1.tar.gz` & `tmp/abqpy2023-2023.5.4.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abqpy2023-0.0.1.tar", last modified: Wed Jul 12 04:38:30 2023, max compression
+gzip compressed data, was "abqpy2023-2023.5.4.post2.tar", last modified: Wed Jul 12 11:41:51 2023, max compression
```

## Comparing `abqpy2023-0.0.1.tar` & `abqpy2023-2023.5.4.post2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:38:30.300686 abqpy2023-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-12 04:38:30.300686 abqpy2023-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-12 04:38:18.000000 abqpy2023-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:38:30.300686 abqpy2023-0.0.1/abqpy2023.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-12 04:38:30.000000 abqpy2023-0.0.1/abqpy2023.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-12 04:38:30.000000 abqpy2023-0.0.1/abqpy2023.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 04:38:30.000000 abqpy2023-0.0.1/abqpy2023.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 04:38:30.000000 abqpy2023-0.0.1/abqpy2023.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 04:38:30.000000 abqpy2023-0.0.1/abqpy2023.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-12 04:38:18.000000 abqpy2023-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 04:38:30.300686 abqpy2023-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:41:51.775436 abqpy2023-2023.5.4.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-12 11:41:51.775436 abqpy2023-2023.5.4.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-12 11:41:39.000000 abqpy2023-2023.5.4.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:41:51.775436 abqpy2023-2023.5.4.post2/abqpy2023.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-12 11:41:51.000000 abqpy2023-2023.5.4.post2/abqpy2023.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-12 11:41:51.000000 abqpy2023-2023.5.4.post2/abqpy2023.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 11:41:51.000000 abqpy2023-2023.5.4.post2/abqpy2023.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 11:41:51.000000 abqpy2023-2023.5.4.post2/abqpy2023.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 11:41:51.000000 abqpy2023-2023.5.4.post2/abqpy2023.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-12 11:41:39.000000 abqpy2023-2023.5.4.post2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 11:41:51.775436 abqpy2023-2023.5.4.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-12 11:41:39.000000 abqpy2023-2023.5.4.post2/setup.py
```

### Comparing `abqpy2023-0.0.1/PKG-INFO` & `abqpy2023-2023.5.4.post2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 Metadata-Version: 2.1
 Name: abqpy2023
-Version: 0.0.1
+Version: 2023.5.4.post2
 Summary: Type hints for Abaqus/Python scripting
 Author-email: WANG Hailin <hailin.wang@connect.polyu.hk>
+Project-URL: Homepage, https://abqpy.com
+Project-URL: GitHub, https://github.com/haiiliin/abqpy
+Project-URL: Bug Tracker, https://github.com/haiiliin/abqpy/issues
+Project-URL: Read the Docs, https://readthedocs.org/projects/abqpy
+Project-URL: Documentation, https://docs.abqpy.com/en/stable/
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abqpy2023-0.0.1/abqpy2023.egg-info/PKG-INFO` & `abqpy2023-2023.5.4.post2/abqpy2023.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 Metadata-Version: 2.1
 Name: abqpy2023
-Version: 0.0.1
+Version: 2023.5.4.post2
 Summary: Type hints for Abaqus/Python scripting
 Author-email: WANG Hailin <hailin.wang@connect.polyu.hk>
+Project-URL: Homepage, https://abqpy.com
+Project-URL: GitHub, https://github.com/haiiliin/abqpy
+Project-URL: Bug Tracker, https://github.com/haiiliin/abqpy/issues
+Project-URL: Read the Docs, https://readthedocs.org/projects/abqpy
+Project-URL: Documentation, https://docs.abqpy.com/en/stable/
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

