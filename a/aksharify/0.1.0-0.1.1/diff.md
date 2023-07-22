# Comparing `tmp/aksharify-0.1.0.tar.gz` & `tmp/aksharify-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-0.1.0.tar", max compression
+gzip compressed data, was "aksharify-0.1.1.tar", max compression
```

## Comparing `aksharify-0.1.0.tar` & `aksharify-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      446 2023-07-22 05:21:16.818911 aksharify-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5988 2023-07-22 03:57:31.621402 aksharify-0.1.0/README.md
--rw-r--r--   0        0        0       55 2023-07-21 04:56:00.214997 aksharify-0.1.0/src/aksharify/__init__.py
--rw-r--r--   0        0        0     3473 2023-07-20 03:47:20.468936 aksharify-0.1.0/src/aksharify/aksharify.py
--rw-r--r--   0        0        0     5274 2023-07-20 14:19:37.279133 aksharify-0.1.0/src/aksharify/distributions.py
--rw-r--r--   0        0        0     1556 2023-07-18 11:04:22.323563 aksharify-0.1.0/src/aksharify/image.py
--rw-r--r--   0        0        0     4711 2023-07-18 04:15:13.427078 aksharify-0.1.0/src/aksharify/outputs.py
--rw-r--r--   0        0        0     6391 1970-01-01 00:00:00.000000 aksharify-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-07-22 05:33:48.477839 aksharify-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0      681 2023-07-22 05:36:53.148738 aksharify-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5988 2023-07-22 03:57:31.621402 aksharify-0.1.1/README.md
+-rw-r--r--   0        0        0       55 2023-07-21 04:56:00.214997 aksharify-0.1.1/src/aksharify/__init__.py
+-rw-r--r--   0        0        0     3473 2023-07-20 03:47:20.468936 aksharify-0.1.1/src/aksharify/aksharify.py
+-rw-r--r--   0        0        0     5274 2023-07-20 14:19:37.279133 aksharify-0.1.1/src/aksharify/distributions.py
+-rw-r--r--   0        0        0     1556 2023-07-18 11:04:22.323563 aksharify-0.1.1/src/aksharify/image.py
+-rw-r--r--   0        0        0     4711 2023-07-18 04:15:13.427078 aksharify-0.1.1/src/aksharify/outputs.py
+-rw-r--r--   0        0        0     6665 1970-01-01 00:00:00.000000 aksharify-0.1.1/PKG-INFO
```

### Comparing `aksharify-0.1.0/README.md` & `aksharify-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.0/src/aksharify/aksharify.py` & `aksharify-0.1.1/src/aksharify/aksharify.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.0/src/aksharify/distributions.py` & `aksharify-0.1.1/src/aksharify/distributions.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.0/src/aksharify/image.py` & `aksharify-0.1.1/src/aksharify/image.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.0/src/aksharify/outputs.py` & `aksharify-0.1.1/src/aksharify/outputs.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.0/PKG-INFO` & `aksharify-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: Ascii Art + Emoji Art python Package
+Home-page: https://primepatel.github.io/aksharify/
+License: LICENSE.md
+Keywords: Ascii Art,Emoji Art,Prime Patel,primepatel
 Author: Prime Patel
 Author-email: primespatel@gmail.com
 Requires-Python: >=3.10,<4.0
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cairosvg (>=2.7.0,<3.0.0)
 Requires-Dist: ipython (>=8.14.0,<9.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: pillow (>=9.3.0,<10.0.0)
 Requires-Dist: scikit-image (>=0.21.0,<0.22.0)
+Project-URL: Repository, https://github.com/primepatel/aksharify
 Description-Content-Type: text/markdown
 
 <a name="readme-top"></a>
 
 # __Aksharify__
 
 [![Contributors][contributors-shield]][contributors-url]
```

