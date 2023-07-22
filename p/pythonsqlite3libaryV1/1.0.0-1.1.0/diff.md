# Comparing `tmp/pythonsqlite3libaryV1-1.0.0.tar.gz` & `tmp/pythonsqlite3libaryV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonsqlite3libaryV1-1.0.0.tar", last modified: Fri Jul 21 23:56:04 2023, max compression
+gzip compressed data, was "pythonsqlite3libaryV1-1.1.0.tar", last modified: Fri Jul 21 23:58:10 2023, max compression
```

## Comparing `pythonsqlite3libaryV1-1.0.0.tar` & `pythonsqlite3libaryV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 23:56:04.970889 pythonsqlite3libaryV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      354 2023-07-21 23:56:04.970889 pythonsqlite3libaryV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 23:56:04.970889 pythonsqlite3libaryV1-1.0.0/pythonsqlite3libaryV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-21 23:56:04.000000 pythonsqlite3libaryV1-1.0.0/pythonsqlite3libaryV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 23:56:04.970889 pythonsqlite3libaryV1-1.0.0/pythonsqlite3libaryV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      354 2023-07-21 23:56:04.000000 pythonsqlite3libaryV1-1.0.0/pythonsqlite3libaryV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      222 2023-07-21 23:56:04.000000 pythonsqlite3libaryV1-1.0.0/pythonsqlite3libaryV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 23:56:04.000000 pythonsqlite3libaryV1-1.0.0/pythonsqlite3libaryV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 23:56:04.000000 pythonsqlite3libaryV1-1.0.0/pythonsqlite3libaryV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 23:56:04.970889 pythonsqlite3libaryV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      567 2023-07-21 23:56:04.000000 pythonsqlite3libaryV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 23:58:10.210502 pythonsqlite3libaryV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-07-21 23:58:10.210502 pythonsqlite3libaryV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 23:58:10.210502 pythonsqlite3libaryV1-1.1.0/pythonsqlite3libaryV1/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-21 23:58:09.000000 pythonsqlite3libaryV1-1.1.0/pythonsqlite3libaryV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 23:58:10.210502 pythonsqlite3libaryV1-1.1.0/pythonsqlite3libaryV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-07-21 23:58:10.000000 pythonsqlite3libaryV1-1.1.0/pythonsqlite3libaryV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      222 2023-07-21 23:58:10.000000 pythonsqlite3libaryV1-1.1.0/pythonsqlite3libaryV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 23:58:10.000000 pythonsqlite3libaryV1-1.1.0/pythonsqlite3libaryV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 23:58:10.000000 pythonsqlite3libaryV1-1.1.0/pythonsqlite3libaryV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 23:58:10.210502 pythonsqlite3libaryV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      567 2023-07-21 23:58:09.000000 pythonsqlite3libaryV1-1.1.0/setup.py
```

### Comparing `pythonsqlite3libaryV1-1.0.0/setup.py` & `pythonsqlite3libaryV1-1.1.0/setup.py`

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
     name="pythonsqlite3libaryV1",
     version=VERSION,
```

