# Comparing `tmp/pysqlilibery-1.0.0.tar.gz` & `tmp/pysqlilibery-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqlilibery-1.0.0.tar", last modified: Fri Jul 21 23:05:59 2023, max compression
+gzip compressed data, was "pysqlilibery-1.1.0.tar", last modified: Fri Jul 21 23:08:05 2023, max compression
```

## Comparing `pysqlilibery-1.0.0.tar` & `pysqlilibery-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 23:05:59.064431 pysqlilibery-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      345 2023-07-21 23:05:59.064431 pysqlilibery-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 23:05:59.064431 pysqlilibery-1.0.0/pysqlilibery/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-21 23:05:58.000000 pysqlilibery-1.0.0/pysqlilibery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 23:05:59.064431 pysqlilibery-1.0.0/pysqlilibery.egg-info/
--rw-r--r--   0 root         (0) root         (0)      345 2023-07-21 23:05:58.000000 pysqlilibery-1.0.0/pysqlilibery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      177 2023-07-21 23:05:59.000000 pysqlilibery-1.0.0/pysqlilibery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 23:05:58.000000 pysqlilibery-1.0.0/pysqlilibery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 23:05:58.000000 pysqlilibery-1.0.0/pysqlilibery.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 23:05:59.064431 pysqlilibery-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      558 2023-07-21 23:05:58.000000 pysqlilibery-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 23:08:05.056020 pysqlilibery-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-07-21 23:08:05.056020 pysqlilibery-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 23:08:05.052020 pysqlilibery-1.1.0/pysqlilibery/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-21 23:08:04.000000 pysqlilibery-1.1.0/pysqlilibery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 23:08:05.056020 pysqlilibery-1.1.0/pysqlilibery.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-07-21 23:08:04.000000 pysqlilibery-1.1.0/pysqlilibery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      177 2023-07-21 23:08:05.000000 pysqlilibery-1.1.0/pysqlilibery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 23:08:04.000000 pysqlilibery-1.1.0/pysqlilibery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-21 23:08:04.000000 pysqlilibery-1.1.0/pysqlilibery.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 23:08:05.056020 pysqlilibery-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      558 2023-07-21 23:08:04.000000 pysqlilibery-1.1.0/setup.py
```

### Comparing `pysqlilibery-1.0.0/setup.py` & `pysqlilibery-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pysqlilibery",
     version=VERSION,
```

