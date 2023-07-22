# Comparing `tmp/photondemo-0.0.1.tar.gz` & `tmp/photondemo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/photondemo-0.0.1.tar", last modified: Sat Jul 22 13:59:50 2023, max compression
+gzip compressed data, was "dist/photondemo-0.0.2.tar", last modified: Sat Jul 22 15:01:03 2023, max compression
```

## Comparing `photondemo-0.0.1.tar` & `photondemo-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2023-07-22 13:59:50.000000 photondemo-0.0.1/
--rw-r--r--   0 charlie    (501) staff       (20)      239 2023-07-22 13:59:50.000000 photondemo-0.0.1/PKG-INFO
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2023-07-22 13:59:50.000000 photondemo-0.0.1/logger/
--rw-r--r--   0 charlie    (501) staff       (20)       33 2023-07-22 13:52:49.000000 photondemo-0.0.1/logger/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)      287 2023-07-22 13:52:53.000000 photondemo-0.0.1/logger/logger.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2023-07-22 13:59:50.000000 photondemo-0.0.1/photondemo.egg-info/
--rw-r--r--   0 charlie    (501) staff       (20)      239 2023-07-22 13:59:50.000000 photondemo-0.0.1/photondemo.egg-info/PKG-INFO
--rw-r--r--   0 charlie    (501) staff       (20)      260 2023-07-22 13:59:50.000000 photondemo-0.0.1/photondemo.egg-info/SOURCES.txt
--rw-r--r--   0 charlie    (501) staff       (20)        1 2023-07-22 13:59:50.000000 photondemo-0.0.1/photondemo.egg-info/dependency_links.txt
--rw-r--r--   0 charlie    (501) staff       (20)        9 2023-07-22 13:59:50.000000 photondemo-0.0.1/photondemo.egg-info/requires.txt
--rw-r--r--   0 charlie    (501) staff       (20)       18 2023-07-22 13:59:50.000000 photondemo-0.0.1/photondemo.egg-info/top_level.txt
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2023-07-22 13:59:50.000000 photondemo-0.0.1/processors/
--rw-r--r--   0 charlie    (501) staff       (20)       39 2023-07-22 13:52:24.000000 photondemo-0.0.1/processors/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)      958 2023-07-22 13:50:48.000000 photondemo-0.0.1/processors/processor.py
--rw-r--r--   0 charlie    (501) staff       (20)       38 2023-07-22 13:59:50.000000 photondemo-0.0.1/setup.cfg
--rw-r--r--   0 charlie    (501) staff       (20)      537 2023-07-22 13:59:09.000000 photondemo-0.0.1/setup.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2023-07-22 15:01:03.000000 photondemo-0.0.2/
+-rw-r--r--   0 charlie    (501) staff       (20)      239 2023-07-22 15:01:03.000000 photondemo-0.0.2/PKG-INFO
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2023-07-22 15:01:03.000000 photondemo-0.0.2/logger/
+-rw-r--r--   0 charlie    (501) staff       (20)       33 2023-07-22 13:52:49.000000 photondemo-0.0.2/logger/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)      287 2023-07-22 13:52:53.000000 photondemo-0.0.2/logger/logger.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2023-07-22 15:01:03.000000 photondemo-0.0.2/photondemo.egg-info/
+-rw-r--r--   0 charlie    (501) staff       (20)      239 2023-07-22 15:01:03.000000 photondemo-0.0.2/photondemo.egg-info/PKG-INFO
+-rw-r--r--   0 charlie    (501) staff       (20)      260 2023-07-22 15:01:03.000000 photondemo-0.0.2/photondemo.egg-info/SOURCES.txt
+-rw-r--r--   0 charlie    (501) staff       (20)        1 2023-07-22 15:01:03.000000 photondemo-0.0.2/photondemo.egg-info/dependency_links.txt
+-rw-r--r--   0 charlie    (501) staff       (20)        9 2023-07-22 15:01:03.000000 photondemo-0.0.2/photondemo.egg-info/requires.txt
+-rw-r--r--   0 charlie    (501) staff       (20)       18 2023-07-22 15:01:03.000000 photondemo-0.0.2/photondemo.egg-info/top_level.txt
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2023-07-22 15:01:03.000000 photondemo-0.0.2/processors/
+-rw-r--r--   0 charlie    (501) staff       (20)       39 2023-07-22 13:52:24.000000 photondemo-0.0.2/processors/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)      958 2023-07-22 13:50:48.000000 photondemo-0.0.2/processors/processor.py
+-rw-r--r--   0 charlie    (501) staff       (20)       38 2023-07-22 15:01:03.000000 photondemo-0.0.2/setup.cfg
+-rw-r--r--   0 charlie    (501) staff       (20)      537 2023-07-22 14:59:35.000000 photondemo-0.0.2/setup.py
```

### Comparing `photondemo-0.0.1/processors/processor.py` & `photondemo-0.0.2/processors/processor.py`

 * *Files identical despite different names*

### Comparing `photondemo-0.0.1/setup.py` & `photondemo-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 DESCRIPTION = ""
 LONG_DESCRIPTION = ""
 
 setup(
     name="photondemo",
     version=VERSION,
     author="Charlie Day",
```

