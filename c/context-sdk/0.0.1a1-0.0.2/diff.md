# Comparing `tmp/context-sdk-0.0.1a1.tar.gz` & `tmp/context-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "context-sdk-0.0.1a1.tar", last modified: Fri Jul 21 23:00:53 2023, max compression
+gzip compressed data, was "context-sdk-0.0.2.tar", last modified: Fri Jul 21 23:02:09 2023, max compression
```

## Comparing `context-sdk-0.0.1a1.tar` & `context-sdk-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ibrahimahmed   (501) staff       (20)        0 2023-07-21 23:00:53.943032 context-sdk-0.0.1a1/
--rw-r--r--   0 ibrahimahmed   (501) staff       (20)      599 2023-07-21 23:00:53.942869 context-sdk-0.0.1a1/PKG-INFO
--rw-r--r--   0 ibrahimahmed   (501) staff       (20)     1273 2023-07-21 22:59:45.000000 context-sdk-0.0.1a1/README.md
-drwxr-xr-x   0 ibrahimahmed   (501) staff       (20)        0 2023-07-21 23:00:53.941988 context-sdk-0.0.1a1/context/
--rw-r--r--   0 ibrahimahmed   (501) staff       (20)     1895 2023-07-21 22:48:58.000000 context-sdk-0.0.1a1/context/__init__.py
-drwxr-xr-x   0 ibrahimahmed   (501) staff       (20)        0 2023-07-21 23:00:53.942529 context-sdk-0.0.1a1/context_sdk.egg-info/
--rw-r--r--   0 ibrahimahmed   (501) staff       (20)      599 2023-07-21 23:00:53.000000 context-sdk-0.0.1a1/context_sdk.egg-info/PKG-INFO
--rw-r--r--   0 ibrahimahmed   (501) staff       (20)      199 2023-07-21 23:00:53.000000 context-sdk-0.0.1a1/context_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahimahmed   (501) staff       (20)        1 2023-07-21 23:00:53.000000 context-sdk-0.0.1a1/context_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahimahmed   (501) staff       (20)        8 2023-07-21 23:00:53.000000 context-sdk-0.0.1a1/context_sdk.egg-info/top_level.txt
--rw-r--r--   0 ibrahimahmed   (501) staff       (20)       38 2023-07-21 23:00:53.943071 context-sdk-0.0.1a1/setup.cfg
--rw-r--r--   0 ibrahimahmed   (501) staff       (20)      737 2023-07-21 23:00:51.000000 context-sdk-0.0.1a1/setup.py
-drwxr-xr-x   0 ibrahimahmed   (501) staff       (20)        0 2023-07-21 23:00:53.942669 context-sdk-0.0.1a1/tests/
--rw-r--r--   0 ibrahimahmed   (501) staff       (20)      562 2023-07-21 22:48:47.000000 context-sdk-0.0.1a1/tests/test_search.py
+drwxr-xr-x   0 ibrahimahmed   (501) staff       (20)        0 2023-07-21 23:02:09.019326 context-sdk-0.0.2/
+-rw-r--r--   0 ibrahimahmed   (501) staff       (20)      597 2023-07-21 23:02:09.019174 context-sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 ibrahimahmed   (501) staff       (20)     1273 2023-07-21 22:59:45.000000 context-sdk-0.0.2/README.md
+drwxr-xr-x   0 ibrahimahmed   (501) staff       (20)        0 2023-07-21 23:02:09.018303 context-sdk-0.0.2/context/
+-rw-r--r--   0 ibrahimahmed   (501) staff       (20)     1895 2023-07-21 22:48:58.000000 context-sdk-0.0.2/context/__init__.py
+drwxr-xr-x   0 ibrahimahmed   (501) staff       (20)        0 2023-07-21 23:02:09.018850 context-sdk-0.0.2/context_sdk.egg-info/
+-rw-r--r--   0 ibrahimahmed   (501) staff       (20)      597 2023-07-21 23:02:08.000000 context-sdk-0.0.2/context_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahimahmed   (501) staff       (20)      199 2023-07-21 23:02:09.000000 context-sdk-0.0.2/context_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahimahmed   (501) staff       (20)        1 2023-07-21 23:02:08.000000 context-sdk-0.0.2/context_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahimahmed   (501) staff       (20)        8 2023-07-21 23:02:08.000000 context-sdk-0.0.2/context_sdk.egg-info/top_level.txt
+-rw-r--r--   0 ibrahimahmed   (501) staff       (20)       38 2023-07-21 23:02:09.019369 context-sdk-0.0.2/setup.cfg
+-rw-r--r--   0 ibrahimahmed   (501) staff       (20)      734 2023-07-21 23:01:57.000000 context-sdk-0.0.2/setup.py
+drwxr-xr-x   0 ibrahimahmed   (501) staff       (20)        0 2023-07-21 23:02:09.018985 context-sdk-0.0.2/tests/
+-rw-r--r--   0 ibrahimahmed   (501) staff       (20)      562 2023-07-21 22:48:47.000000 context-sdk-0.0.2/tests/test_search.py
```

### Comparing `context-sdk-0.0.1a1/PKG-INFO` & `context-sdk-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: context-sdk
-Version: 0.0.1a1
+Version: 0.0.2
 Summary: Context SDK
 Home-page: https://usecontext.com
 Author: Context
 Author-email: sam@usecontext.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `context-sdk-0.0.1a1/README.md` & `context-sdk-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `context-sdk-0.0.1a1/context/__init__.py` & `context-sdk-0.0.2/context/__init__.py`

 * *Files identical despite different names*

### Comparing `context-sdk-0.0.1a1/context_sdk.egg-info/PKG-INFO` & `context-sdk-0.0.2/context_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: context-sdk
-Version: 0.0.1a1
+Version: 0.0.2
 Summary: Context SDK
 Home-page: https://usecontext.com
 Author: Context
 Author-email: sam@usecontext.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `context-sdk-0.0.1a1/setup.py` & `context-sdk-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="context-sdk",
-    version="0.0.1-a1",
+    version="0.0.2",
     description="Context SDK",
     author="Context",
     author_email="sam@usecontext.com",
     url="https://usecontext.com",
     packages=find_packages(),
     install_requires=[],
     classifiers=[
```

### Comparing `context-sdk-0.0.1a1/tests/test_search.py` & `context-sdk-0.0.2/tests/test_search.py`

 * *Files identical despite different names*

