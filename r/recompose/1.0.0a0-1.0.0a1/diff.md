# Comparing `tmp/recompose-1.0.0a0-py3-none-any.whl.zip` & `tmp/recompose-1.0.0a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,10 @@
-Zip file size: 1817 bytes, number of entries: 6
--rw-rw-r--  2.0 unx       30 b- defN 23-Jul-22 06:31 recompose/__init__.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jul-22 06:32 recompose/py.typed
--rw-rw-r--  2.0 unx     1036 b- defN 23-Jul-22 06:32 recompose-1.0.0a0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-22 06:32 recompose-1.0.0a0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jul-22 06:32 recompose-1.0.0a0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      462 b- defN 23-Jul-22 06:32 recompose-1.0.0a0.dist-info/RECORD
-6 files, 1630 bytes uncompressed, 973 bytes compressed:  40.3%
+Zip file size: 2943 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-22 06:59 recompose/VERSION
+-rw-r--r--  2.0 unx      200 b- defN 23-Jul-22 06:59 recompose/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-22 06:59 recompose/py.typed
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jul-22 06:59 recompose-1.0.0a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1058 b- defN 23-Jul-22 06:59 recompose-1.0.0a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-22 06:59 recompose-1.0.0a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-22 06:59 recompose-1.0.0a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      627 b- defN 23-Jul-22 06:59 recompose-1.0.0a1.dist-info/RECORD
+8 files, 3074 bytes uncompressed, 1843 bytes compressed:  40.0%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
+Filename: recompose/VERSION
+Comment: 
+
 Filename: recompose/__init__.py
 Comment: 
 
 Filename: recompose/py.typed
 Comment: 
 
-Filename: recompose-1.0.0a0.dist-info/METADATA
+Filename: recompose-1.0.0a1.dist-info/LICENSE
+Comment: 
+
+Filename: recompose-1.0.0a1.dist-info/METADATA
 Comment: 
 
-Filename: recompose-1.0.0a0.dist-info/WHEEL
+Filename: recompose-1.0.0a1.dist-info/WHEEL
 Comment: 
 
-Filename: recompose-1.0.0a0.dist-info/top_level.txt
+Filename: recompose-1.0.0a1.dist-info/top_level.txt
 Comment: 
 
-Filename: recompose-1.0.0a0.dist-info/RECORD
+Filename: recompose-1.0.0a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## recompose/__init__.py

```diff
@@ -1 +1,8 @@
-__version__ = "1.0.0-alpha.0"
+"""
+Recompose is a Python package for templated data recomposition.
+"""
+
+from importlib.resources import open_text
+
+with open_text(__package__, "VERSION") as t:
+    __version__ = t.readline().strip()
```

## Comparing `recompose-1.0.0a0.dist-info/METADATA` & `recompose-1.0.0a1.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: recompose
-Version: 1.0.0a0
+Version: 1.0.0a1
 Summary: Templated data recomposition
 Home-page: https://github.com/cariad/recompose
 Author: Cariad Eccleston
 Author-email: cariad@cariad.earth
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # recompose
 
 **recompose** is a Python package for templated data recomposition.
 
 ## Author
```

