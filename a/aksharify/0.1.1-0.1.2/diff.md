# Comparing `tmp/aksharify-0.1.1.tar.gz` & `tmp/aksharify-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-0.1.1.tar", max compression
+gzip compressed data, was "aksharify-0.1.2.tar", max compression
```

## Comparing `aksharify-0.1.1.tar` & `aksharify-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1094 2023-07-22 05:33:48.477839 aksharify-0.1.1/LICENSE.md
--rw-r--r--   0        0        0      681 2023-07-22 05:36:53.148738 aksharify-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5988 2023-07-22 03:57:31.621402 aksharify-0.1.1/README.md
--rw-r--r--   0        0        0       55 2023-07-21 04:56:00.214997 aksharify-0.1.1/src/aksharify/__init__.py
--rw-r--r--   0        0        0     3473 2023-07-20 03:47:20.468936 aksharify-0.1.1/src/aksharify/aksharify.py
--rw-r--r--   0        0        0     5274 2023-07-20 14:19:37.279133 aksharify-0.1.1/src/aksharify/distributions.py
--rw-r--r--   0        0        0     1556 2023-07-18 11:04:22.323563 aksharify-0.1.1/src/aksharify/image.py
--rw-r--r--   0        0        0     4711 2023-07-18 04:15:13.427078 aksharify-0.1.1/src/aksharify/outputs.py
--rw-r--r--   0        0        0     6665 1970-01-01 00:00:00.000000 aksharify-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-07-22 05:33:48.477839 aksharify-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0      674 2023-07-22 05:41:38.335539 aksharify-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5988 2023-07-22 03:57:31.621402 aksharify-0.1.2/README.md
+-rw-r--r--   0        0        0       55 2023-07-21 04:56:00.214997 aksharify-0.1.2/src/aksharify/__init__.py
+-rw-r--r--   0        0        0     3473 2023-07-20 03:47:20.468936 aksharify-0.1.2/src/aksharify/aksharify.py
+-rw-r--r--   0        0        0     5274 2023-07-20 14:19:37.279133 aksharify-0.1.2/src/aksharify/distributions.py
+-rw-r--r--   0        0        0     1556 2023-07-18 11:04:22.323563 aksharify-0.1.2/src/aksharify/image.py
+-rw-r--r--   0        0        0     4711 2023-07-18 04:15:13.427078 aksharify-0.1.2/src/aksharify/outputs.py
+-rw-r--r--   0        0        0     6660 1970-01-01 00:00:00.000000 aksharify-0.1.2/PKG-INFO
```

### Comparing `aksharify-0.1.1/LICENSE.md` & `aksharify-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.1/pyproject.toml` & `aksharify-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "aksharify"
-version = "0.1.1"
+version = "0.1.2"
 description = "Ascii Art + Emoji Art python Package"
 authors = ["Prime Patel <primespatel@gmail.com>"]
 readme = "README.md"
 packages = [{include = "aksharify", from = "src"}]
-license = "LICENSE.md"
+license = "MIT"
 homepage = "https://primepatel.github.io/aksharify/"
 repository = "https://github.com/primepatel/aksharify"
 keywords = ["Ascii Art","Emoji Art","Prime Patel","primepatel"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pillow = "^9.3.0"
```

### Comparing `aksharify-0.1.1/README.md` & `aksharify-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.1/src/aksharify/aksharify.py` & `aksharify-0.1.2/src/aksharify/aksharify.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.1/src/aksharify/distributions.py` & `aksharify-0.1.2/src/aksharify/distributions.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.1/src/aksharify/image.py` & `aksharify-0.1.2/src/aksharify/image.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.1/src/aksharify/outputs.py` & `aksharify-0.1.2/src/aksharify/outputs.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.1/PKG-INFO` & `aksharify-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 0.1.1
+Version: 0.1.2
 Summary: Ascii Art + Emoji Art python Package
 Home-page: https://primepatel.github.io/aksharify/
-License: LICENSE.md
+License: MIT
 Keywords: Ascii Art,Emoji Art,Prime Patel,primepatel
 Author: Prime Patel
 Author-email: primespatel@gmail.com
 Requires-Python: >=3.10,<4.0
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cairosvg (>=2.7.0,<3.0.0)
 Requires-Dist: ipython (>=8.14.0,<9.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: pillow (>=9.3.0,<10.0.0)
```

