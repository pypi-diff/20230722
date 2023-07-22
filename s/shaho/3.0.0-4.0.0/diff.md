# Comparing `tmp/shaho-3.0.0.tar.gz` & `tmp/shaho-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaho-3.0.0.tar", last modified: Tue Jul  4 18:57:42 2023, max compression
+gzip compressed data, was "shaho-4.0.0.tar", last modified: Sat Jul 22 11:52:53 2023, max compression
```

## Comparing `shaho-3.0.0.tar` & `shaho-4.0.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-04 18:57:42.433614 shaho-3.0.0/
--rw-rw----   0 root         (0) everybody  (9997)     1081 2023-06-19 22:22:31.000000 shaho-3.0.0/LICENCE
--rw-rw----   0 root         (0) everybody  (9997)      902 2023-07-04 18:57:42.413614 shaho-3.0.0/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)        8 2023-06-19 22:20:40.000000 shaho-3.0.0/README.md
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-04 18:57:42.433614 shaho-3.0.0/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1059 2023-07-04 18:45:18.000000 shaho-3.0.0/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-04 18:57:42.253614 shaho-3.0.0/shaho/
--rw-rw----   0 root         (0) everybody  (9997)       14 2023-06-19 22:14:59.000000 shaho-3.0.0/shaho/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    22222 2023-07-04 18:44:18.000000 shaho-3.0.0/shaho/mb.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-04 18:57:42.393614 shaho-3.0.0/shaho.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      902 2023-07-04 18:57:41.000000 shaho-3.0.0/shaho.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      172 2023-07-04 18:57:42.000000 shaho-3.0.0/shaho.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-04 18:57:41.000000 shaho-3.0.0/shaho.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        6 2023-07-04 18:57:42.000000 shaho-3.0.0/shaho.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-22 11:52:52.993393 shaho-4.0.0/
+-rw-rw----   0 root         (0) everybody  (9997)     1081 2023-06-19 22:22:31.000000 shaho-4.0.0/LICENCE
+-rw-rw----   0 root         (0) everybody  (9997)      883 2023-07-22 11:52:52.973393 shaho-4.0.0/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)        8 2023-06-19 22:20:40.000000 shaho-4.0.0/README.md
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-22 11:52:52.993393 shaho-4.0.0/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1059 2023-07-22 11:49:07.000000 shaho-4.0.0/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-22 11:52:52.803393 shaho-4.0.0/shaho/
+-rw-rw----   0 root         (0) everybody  (9997)      789 2023-07-19 14:40:37.000000 shaho-4.0.0/shaho/An_Wb.py
+-rw-rw----   0 root         (0) everybody  (9997)     2412 2023-07-22 11:47:25.000000 shaho-4.0.0/shaho/Socket.py
+-rw-rw----   0 root         (0) everybody  (9997)       14 2023-06-19 22:14:59.000000 shaho-4.0.0/shaho/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     4079 2023-07-19 14:40:37.000000 shaho-4.0.0/shaho/encryption.py
+-rw-rw----   0 root         (0) everybody  (9997)    64261 2023-07-22 09:46:28.000000 shaho-4.0.0/shaho/mb.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-22 11:52:52.943393 shaho-4.0.0/shaho.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      883 2023-07-22 11:52:52.000000 shaho-4.0.0/shaho.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      223 2023-07-22 11:52:52.000000 shaho-4.0.0/shaho.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-22 11:52:52.000000 shaho-4.0.0/shaho.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        6 2023-07-22 11:52:52.000000 shaho-4.0.0/shaho.egg-info/top_level.txt
```

### Comparing `shaho-3.0.0/LICENCE` & `shaho-4.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `shaho-3.0.0/PKG-INFO` & `shaho-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: shaho
-Version: 3.0.0
+Version: 4.0.0
 Summary:  library Robot
 Home-page: https://github.com
 Author: shaho
 Author-email: mbshahoorg@gmail.com
 License: MIT
 Keywords: shaho,Shaho
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
@@ -20,8 +19,7 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENCE
 
 Mb ShAhO
-
```

### Comparing `shaho-3.0.0/setup.py` & `shaho-4.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 from setuptools import setup
 
 _long_description = open('README.md').read()
 
 setup(
     name = "shaho",
-    version = "3.0.0",
+    version = "4.0.0",
     author = "shaho",
     author_email = "mbshahoorg@gmail.com",
     description = (" library Robot"),
     license = "MIT",
     keywords = ["shaho","Shaho"],
     url = "https://github.com",
     packages=['shaho'],
```

### Comparing `shaho-3.0.0/shaho.egg-info/PKG-INFO` & `shaho-4.0.0/shaho.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: shaho
-Version: 3.0.0
+Version: 4.0.0
 Summary:  library Robot
 Home-page: https://github.com
 Author: shaho
 Author-email: mbshahoorg@gmail.com
 License: MIT
 Keywords: shaho,Shaho
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
@@ -20,8 +19,7 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENCE
 
 Mb ShAhO
-
```

