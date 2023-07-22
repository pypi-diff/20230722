# Comparing `tmp/aiopypiserver-0.0.5.tar.gz` & `tmp/aiopypiserver-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopypiserver-0.0.5.tar", last modified: Sat Jul 22 02:37:43 2023, max compression
+gzip compressed data, was "aiopypiserver-0.0.6.tar", last modified: Sat Jul 22 08:38:48 2023, max compression
```

## Comparing `aiopypiserver-0.0.5.tar` & `aiopypiserver-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 02:37:43.609187 aiopypiserver-0.0.5/
--rw-rw-rw-   0        0        0    35149 2023-07-14 22:21:30.000000 aiopypiserver-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       31 2023-07-17 10:49:17.000000 aiopypiserver-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2468 2023-07-22 02:37:43.608188 aiopypiserver-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1786 2023-07-18 09:58:20.000000 aiopypiserver-0.0.5/README.md
--rw-rw-rw-   0        0        0      786 2023-07-22 02:36:07.000000 aiopypiserver-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-22 02:37:43.609187 aiopypiserver-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-22 02:37:43.523184 aiopypiserver-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-22 02:37:43.540179 aiopypiserver-0.0.5/src/aiopypiserver/
--rw-rw-rw-   0        0        0      109 2023-07-17 10:49:17.000000 aiopypiserver-0.0.5/src/aiopypiserver/__init__.py
--rw-rw-rw-   0        0        0      112 2023-07-17 10:49:17.000000 aiopypiserver-0.0.5/src/aiopypiserver/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 02:37:43.603187 aiopypiserver-0.0.5/src/aiopypiserver/assets/
--rw-rw-rw-   0        0        0        0 2023-07-18 09:58:20.000000 aiopypiserver-0.0.5/src/aiopypiserver/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 02:37:43.605188 aiopypiserver-0.0.5/src/aiopypiserver/assets/__pycache__/
--rw-rw-rw-   0        0        0      197 2023-07-18 09:58:20.000000 aiopypiserver-0.0.5/src/aiopypiserver/assets/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    14282 2023-07-21 16:03:22.000000 aiopypiserver-0.0.5/src/aiopypiserver/assets/grids-responsive-min.css
--rw-rw-rw-   0        0        0     2311 2023-07-21 17:02:47.000000 aiopypiserver-0.0.5/src/aiopypiserver/assets/index.html
--rw-rw-rw-   0        0        0      169 2023-07-17 10:49:17.000000 aiopypiserver-0.0.5/src/aiopypiserver/assets/list.html
--rw-rw-rw-   0        0        0    15721 2023-07-21 16:03:28.000000 aiopypiserver-0.0.5/src/aiopypiserver/assets/pure-min.css
--rw-rw-rw-   0        0        0     2192 2023-07-21 17:00:21.000000 aiopypiserver-0.0.5/src/aiopypiserver/assets/styles.css
--rw-rw-rw-   0        0        0    10554 2023-07-21 17:08:20.000000 aiopypiserver-0.0.5/src/aiopypiserver/webserver.py
-drwxrwxrwx   0        0        0        0 2023-07-22 02:37:43.567181 aiopypiserver-0.0.5/src/aiopypiserver.egg-info/
--rw-rw-rw-   0        0        0     2468 2023-07-22 02:37:43.000000 aiopypiserver-0.0.5/src/aiopypiserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      698 2023-07-22 02:37:43.000000 aiopypiserver-0.0.5/src/aiopypiserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 02:37:43.000000 aiopypiserver-0.0.5/src/aiopypiserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-22 02:37:43.000000 aiopypiserver-0.0.5/src/aiopypiserver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-07-22 02:37:43.000000 aiopypiserver-0.0.5/src/aiopypiserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-22 02:37:43.000000 aiopypiserver-0.0.5/src/aiopypiserver.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-22 02:37:43.607189 aiopypiserver-0.0.5/tests/
--rw-rw-rw-   0        0        0      941 2023-07-17 10:49:17.000000 aiopypiserver-0.0.5/tests/test_server.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:38:48.932686 aiopypiserver-0.0.6/
+-rw-rw-rw-   0        0        0    35149 2023-07-14 22:21:30.000000 aiopypiserver-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       31 2023-07-17 10:49:17.000000 aiopypiserver-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2468 2023-07-22 08:38:48.930167 aiopypiserver-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1786 2023-07-18 09:58:20.000000 aiopypiserver-0.0.6/README.md
+-rw-rw-rw-   0        0        0      786 2023-07-22 08:35:36.000000 aiopypiserver-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-22 08:38:48.933686 aiopypiserver-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-22 08:38:48.889463 aiopypiserver-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-22 08:38:48.899978 aiopypiserver-0.0.6/src/aiopypiserver/
+-rw-rw-rw-   0        0        0      109 2023-07-17 10:49:17.000000 aiopypiserver-0.0.6/src/aiopypiserver/__init__.py
+-rw-rw-rw-   0        0        0      112 2023-07-17 10:49:17.000000 aiopypiserver-0.0.6/src/aiopypiserver/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:38:48.926170 aiopypiserver-0.0.6/src/aiopypiserver/assets/
+-rw-rw-rw-   0        0        0        0 2023-07-18 09:58:20.000000 aiopypiserver-0.0.6/src/aiopypiserver/assets/__init__.py
+-rw-rw-rw-   0        0        0     2205 2023-07-22 08:34:56.000000 aiopypiserver-0.0.6/src/aiopypiserver/assets/index.html
+-rw-rw-rw-   0        0        0      169 2023-07-17 10:49:17.000000 aiopypiserver-0.0.6/src/aiopypiserver/assets/list.html
+-rw-rw-rw-   0        0        0     3678 2023-07-22 08:34:04.000000 aiopypiserver-0.0.6/src/aiopypiserver/assets/pure.css
+-rw-rw-rw-   0        0        0    10554 2023-07-21 17:08:20.000000 aiopypiserver-0.0.6/src/aiopypiserver/webserver.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:38:48.913637 aiopypiserver-0.0.6/src/aiopypiserver.egg-info/
+-rw-rw-rw-   0        0        0     2468 2023-07-22 08:38:48.000000 aiopypiserver-0.0.6/src/aiopypiserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      546 2023-07-22 08:38:48.000000 aiopypiserver-0.0.6/src/aiopypiserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 08:38:48.000000 aiopypiserver-0.0.6/src/aiopypiserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-22 08:38:48.000000 aiopypiserver-0.0.6/src/aiopypiserver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-07-22 08:38:48.000000 aiopypiserver-0.0.6/src/aiopypiserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-22 08:38:48.000000 aiopypiserver-0.0.6/src/aiopypiserver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 08:38:48.928169 aiopypiserver-0.0.6/tests/
+-rw-rw-rw-   0        0        0      941 2023-07-17 10:49:17.000000 aiopypiserver-0.0.6/tests/test_server.py
```

### Comparing `aiopypiserver-0.0.5/LICENSE` & `aiopypiserver-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopypiserver-0.0.5/PKG-INFO` & `aiopypiserver-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopypiserver
-Version: 0.0.5
+Version: 0.0.6
 Summary: Do what pypiserver does, but with aiohttp.
 Author: Jamie Walton
 Project-URL: Homepage, https://github.com/jamie0walton/aiopypiserver
 Project-URL: Bug Tracker, https://github.com/jamie0walton/aiopypiserver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `aiopypiserver-0.0.5/README.md` & `aiopypiserver-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aiopypiserver-0.0.5/pyproject.toml` & `aiopypiserver-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aiopypiserver"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     {name="Jamie Walton"}
 ]
 description = "Do what pypiserver does, but with aiohttp."
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
```

### Comparing `aiopypiserver-0.0.5/src/aiopypiserver/assets/index.html` & `aiopypiserver-0.0.6/src/aiopypiserver/assets/index.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
   <meta charset="utf-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <title>Welcome to aiopypiserver</title>
-  <link rel="stylesheet" href="pure-min.css">
-  <link rel="stylesheet" href="grids-responsive-min.css">
-  <link rel="stylesheet" href="styles.css">
+  <link rel="stylesheet" href="pure.css">
 </head>
 <body>
 
 <div id="layout" class="pure-g">
 <div class="sidebar pure-u-1 pure-u-md-1-4">
   <div class="header">
     <h2 class="brand-title">PyPI Server</h2>
```

#### html2text {}

```diff
@@ -1,10 +1,8 @@
 
-
-
 ***** PyPI Server *****
 ****** Welcome ******
 
 ***** aiopypiserver *****
 Your PyPI server.
 Relative hrefs behind a web proxy work.
```

### Comparing `aiopypiserver-0.0.5/src/aiopypiserver/webserver.py` & `aiopypiserver-0.0.6/src/aiopypiserver/webserver.py`

 * *Files identical despite different names*

### Comparing `aiopypiserver-0.0.5/src/aiopypiserver.egg-info/PKG-INFO` & `aiopypiserver-0.0.6/src/aiopypiserver.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopypiserver
-Version: 0.0.5
+Version: 0.0.6
 Summary: Do what pypiserver does, but with aiohttp.
 Author: Jamie Walton
 Project-URL: Homepage, https://github.com/jamie0walton/aiopypiserver
 Project-URL: Bug Tracker, https://github.com/jamie0walton/aiopypiserver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `aiopypiserver-0.0.5/src/aiopypiserver.egg-info/SOURCES.txt` & `aiopypiserver-0.0.6/src/aiopypiserver.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,11 @@
 src/aiopypiserver.egg-info/PKG-INFO
 src/aiopypiserver.egg-info/SOURCES.txt
 src/aiopypiserver.egg-info/dependency_links.txt
 src/aiopypiserver.egg-info/entry_points.txt
 src/aiopypiserver.egg-info/requires.txt
 src/aiopypiserver.egg-info/top_level.txt
 src/aiopypiserver/assets/__init__.py
-src/aiopypiserver/assets/grids-responsive-min.css
 src/aiopypiserver/assets/index.html
 src/aiopypiserver/assets/list.html
-src/aiopypiserver/assets/pure-min.css
-src/aiopypiserver/assets/styles.css
-src/aiopypiserver/assets/__pycache__/__init__.cpython-311.pyc
+src/aiopypiserver/assets/pure.css
 tests/test_server.py
```

### Comparing `aiopypiserver-0.0.5/tests/test_server.py` & `aiopypiserver-0.0.6/tests/test_server.py`

 * *Files identical despite different names*

