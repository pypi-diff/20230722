# Comparing `tmp/idkwhttph-0.2.4.tar.gz` & `tmp/idkwhttph-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idkwhttph-0.2.4.tar", max compression
+gzip compressed data, was "idkwhttph-0.2.5.tar", max compression
```

## Comparing `idkwhttph-0.2.4.tar` & `idkwhttph-0.2.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    18949 2023-07-22 06:19:20.459694 idkwhttph-0.2.4/idkwhttph/__init__.py
--rw-r--r--   0        0        0      295 2023-07-22 06:19:23.251690 idkwhttph-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      492 2023-07-22 06:19:58.446846 idkwhttph-0.2.4/setup.py
--rw-r--r--   0        0        0      239 2023-07-22 06:19:58.447285 idkwhttph-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    18949 2023-07-22 06:41:49.852980 idkwhttph-0.2.5/idkwhttph/__init__.py
+-rw-r--r--   0        0        0      295 2023-07-22 06:41:59.128970 idkwhttph-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      492 2023-07-22 06:42:23.264938 idkwhttph-0.2.5/setup.py
+-rw-r--r--   0        0        0      239 2023-07-22 06:42:23.265171 idkwhttph-0.2.5/PKG-INFO
```

### Comparing `idkwhttph-0.2.4/idkwhttph/__init__.py` & `idkwhttph-0.2.5/idkwhttph/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 # Imports
 
 from getkey import getkey, keys
 from replit import clear
 from replit import db
 from time import sleep
 import cursor
```

