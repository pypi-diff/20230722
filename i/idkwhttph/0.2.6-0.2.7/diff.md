# Comparing `tmp/idkwhttph-0.2.6.tar.gz` & `tmp/idkwhttph-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idkwhttph-0.2.6.tar", max compression
+gzip compressed data, was "idkwhttph-0.2.7.tar", max compression
```

## Comparing `idkwhttph-0.2.6.tar` & `idkwhttph-0.2.7.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    19022 2023-07-22 06:51:20.344386 idkwhttph-0.2.6/idkwhttph/__init__.py
--rw-r--r--   0        0        0      295 2023-07-22 06:51:26.552379 idkwhttph-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      492 2023-07-22 06:53:12.131276 idkwhttph-0.2.6/setup.py
--rw-r--r--   0        0        0      239 2023-07-22 06:53:12.131691 idkwhttph-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    19022 2023-07-22 06:55:02.008155 idkwhttph-0.2.7/idkwhttph/__init__.py
+-rw-r--r--   0        0        0      295 2023-07-22 06:55:05.448151 idkwhttph-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      492 2023-07-22 06:56:14.676338 idkwhttph-0.2.7/setup.py
+-rw-r--r--   0        0        0      239 2023-07-22 06:56:14.676620 idkwhttph-0.2.7/PKG-INFO
```

### Comparing `idkwhttph-0.2.6/idkwhttph/__init__.py` & `idkwhttph-0.2.7/idkwhttph/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 # Imports
 
 from getkey import getkey, keys
 from replit import clear
 from replit import db
 from time import sleep
 import cursor
```

