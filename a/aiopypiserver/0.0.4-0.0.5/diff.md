# Comparing `tmp/aiopypiserver-0.0.4.tar.gz` & `tmp/aiopypiserver-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopypiserver-0.0.4.tar", last modified: Fri Jul 21 17:09:38 2023, max compression
+gzip compressed data, was "aiopypiserver-0.0.5.tar", last modified: Sat Jul 22 02:37:43 2023, max compression
```

## Comparing `aiopypiserver-0.0.4.tar` & `aiopypiserver-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.387835 aiopypiserver-0.0.4/
--rw-rw-rw-   0        0        0    35149 2023-07-14 22:21:30.000000 aiopypiserver-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       31 2023-07-17 10:49:17.000000 aiopypiserver-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2471 2023-07-21 17:09:38.387835 aiopypiserver-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1786 2023-07-18 09:58:20.000000 aiopypiserver-0.0.4/README.md
--rw-rw-rw-   0        0        0      789 2023-07-21 17:07:58.000000 aiopypiserver-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-21 17:09:38.388836 aiopypiserver-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.331310 aiopypiserver-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.349308 aiopypiserver-0.0.4/src/aiopypiserver/
--rw-rw-rw-   0        0        0      109 2023-07-17 10:49:17.000000 aiopypiserver-0.0.4/src/aiopypiserver/__init__.py
--rw-rw-rw-   0        0        0      112 2023-07-17 10:49:17.000000 aiopypiserver-0.0.4/src/aiopypiserver/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.382834 aiopypiserver-0.0.4/src/aiopypiserver/assets/
--rw-rw-rw-   0        0        0        0 2023-07-18 09:58:20.000000 aiopypiserver-0.0.4/src/aiopypiserver/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.384835 aiopypiserver-0.0.4/src/aiopypiserver/assets/__pycache__/
--rw-rw-rw-   0        0        0      197 2023-07-18 09:58:20.000000 aiopypiserver-0.0.4/src/aiopypiserver/assets/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    14282 2023-07-21 16:03:22.000000 aiopypiserver-0.0.4/src/aiopypiserver/assets/grids-responsive-min.css
--rw-rw-rw-   0        0        0     2311 2023-07-21 17:02:47.000000 aiopypiserver-0.0.4/src/aiopypiserver/assets/index.html
--rw-rw-rw-   0        0        0      169 2023-07-17 10:49:17.000000 aiopypiserver-0.0.4/src/aiopypiserver/assets/list.html
--rw-rw-rw-   0        0        0    15721 2023-07-21 16:03:28.000000 aiopypiserver-0.0.4/src/aiopypiserver/assets/pure-min.css
--rw-rw-rw-   0        0        0     2192 2023-07-21 17:00:21.000000 aiopypiserver-0.0.4/src/aiopypiserver/assets/styles.css
--rw-rw-rw-   0        0        0    10554 2023-07-21 17:08:20.000000 aiopypiserver-0.0.4/src/aiopypiserver/webserver.py
-drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.373826 aiopypiserver-0.0.4/src/aiopypiserver.egg-info/
--rw-rw-rw-   0        0        0     2471 2023-07-21 17:09:38.000000 aiopypiserver-0.0.4/src/aiopypiserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      698 2023-07-21 17:09:38.000000 aiopypiserver-0.0.4/src/aiopypiserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 17:09:38.000000 aiopypiserver-0.0.4/src/aiopypiserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-21 17:09:38.000000 aiopypiserver-0.0.4/src/aiopypiserver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-07-21 17:09:38.000000 aiopypiserver-0.0.4/src/aiopypiserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-21 17:09:38.000000 aiopypiserver-0.0.4/src/aiopypiserver.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 17:09:38.386836 aiopypiserver-0.0.4/tests/
--rw-rw-rw-   0        0        0      941 2023-07-17 10:49:17.000000 aiopypiserver-0.0.4/tests/test_server.py
+drwxrwxrwx   0        0        0        0 2023-07-22 02:37:43.609187 aiopypiserver-0.0.5/
+-rw-rw-rw-   0        0        0    35149 2023-07-14 22:21:30.000000 aiopypiserver-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       31 2023-07-17 10:49:17.000000 aiopypiserver-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2468 2023-07-22 02:37:43.608188 aiopypiserver-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1786 2023-07-18 09:58:20.000000 aiopypiserver-0.0.5/README.md
+-rw-rw-rw-   0        0        0      786 2023-07-22 02:36:07.000000 aiopypiserver-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-22 02:37:43.609187 aiopypiserver-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-22 02:37:43.523184 aiopypiserver-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-22 02:37:43.540179 aiopypiserver-0.0.5/src/aiopypiserver/
+-rw-rw-rw-   0        0        0      109 2023-07-17 10:49:17.000000 aiopypiserver-0.0.5/src/aiopypiserver/__init__.py
+-rw-rw-rw-   0        0        0      112 2023-07-17 10:49:17.000000 aiopypiserver-0.0.5/src/aiopypiserver/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 02:37:43.603187 aiopypiserver-0.0.5/src/aiopypiserver/assets/
+-rw-rw-rw-   0        0        0        0 2023-07-18 09:58:20.000000 aiopypiserver-0.0.5/src/aiopypiserver/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 02:37:43.605188 aiopypiserver-0.0.5/src/aiopypiserver/assets/__pycache__/
+-rw-rw-rw-   0        0        0      197 2023-07-18 09:58:20.000000 aiopypiserver-0.0.5/src/aiopypiserver/assets/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    14282 2023-07-21 16:03:22.000000 aiopypiserver-0.0.5/src/aiopypiserver/assets/grids-responsive-min.css
+-rw-rw-rw-   0        0        0     2311 2023-07-21 17:02:47.000000 aiopypiserver-0.0.5/src/aiopypiserver/assets/index.html
+-rw-rw-rw-   0        0        0      169 2023-07-17 10:49:17.000000 aiopypiserver-0.0.5/src/aiopypiserver/assets/list.html
+-rw-rw-rw-   0        0        0    15721 2023-07-21 16:03:28.000000 aiopypiserver-0.0.5/src/aiopypiserver/assets/pure-min.css
+-rw-rw-rw-   0        0        0     2192 2023-07-21 17:00:21.000000 aiopypiserver-0.0.5/src/aiopypiserver/assets/styles.css
+-rw-rw-rw-   0        0        0    10554 2023-07-21 17:08:20.000000 aiopypiserver-0.0.5/src/aiopypiserver/webserver.py
+drwxrwxrwx   0        0        0        0 2023-07-22 02:37:43.567181 aiopypiserver-0.0.5/src/aiopypiserver.egg-info/
+-rw-rw-rw-   0        0        0     2468 2023-07-22 02:37:43.000000 aiopypiserver-0.0.5/src/aiopypiserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      698 2023-07-22 02:37:43.000000 aiopypiserver-0.0.5/src/aiopypiserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 02:37:43.000000 aiopypiserver-0.0.5/src/aiopypiserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-22 02:37:43.000000 aiopypiserver-0.0.5/src/aiopypiserver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-07-22 02:37:43.000000 aiopypiserver-0.0.5/src/aiopypiserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-22 02:37:43.000000 aiopypiserver-0.0.5/src/aiopypiserver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 02:37:43.607189 aiopypiserver-0.0.5/tests/
+-rw-rw-rw-   0        0        0      941 2023-07-17 10:49:17.000000 aiopypiserver-0.0.5/tests/test_server.py
```

### Comparing `aiopypiserver-0.0.4/LICENSE` & `aiopypiserver-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopypiserver-0.0.4/PKG-INFO` & `aiopypiserver-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: aiopypiserver
-Version: 0.0.4
+Version: 0.0.5
 Summary: Do what pypiserver does, but with aiohttp.
 Author: Jamie Walton
 Project-URL: Homepage, https://github.com/jamie0walton/aiopypiserver
 Project-URL: Bug Tracker, https://github.com/jamie0walton/aiopypiserver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aiopypiserver
 
 A basic PyPi server using aiohttp to serve web pages. Intended to work behind
```

### Comparing `aiopypiserver-0.0.4/README.md` & `aiopypiserver-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aiopypiserver-0.0.4/pyproject.toml` & `aiopypiserver-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aiopypiserver"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     {name="Jamie Walton"}
 ]
 description = "Do what pypiserver does, but with aiohttp."
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
     "aiohttp == 3.8.*"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Environment :: Console",
-    "Development Status :: 1 - Planning",
+    "Development Status :: 3 - Alpha",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/jamie0walton/aiopypiserver"
 "Bug Tracker" = "https://github.com/jamie0walton/aiopypiserver/issues"
 
 [project.scripts]
```

### Comparing `aiopypiserver-0.0.4/src/aiopypiserver/assets/grids-responsive-min.css` & `aiopypiserver-0.0.5/src/aiopypiserver/assets/grids-responsive-min.css`

 * *Files identical despite different names*

### Comparing `aiopypiserver-0.0.4/src/aiopypiserver/assets/index.html` & `aiopypiserver-0.0.5/src/aiopypiserver/assets/index.html`

 * *Files identical despite different names*

### Comparing `aiopypiserver-0.0.4/src/aiopypiserver/assets/pure-min.css` & `aiopypiserver-0.0.5/src/aiopypiserver/assets/pure-min.css`

 * *Files identical despite different names*

### Comparing `aiopypiserver-0.0.4/src/aiopypiserver/assets/styles.css` & `aiopypiserver-0.0.5/src/aiopypiserver/assets/styles.css`

 * *Files identical despite different names*

### Comparing `aiopypiserver-0.0.4/src/aiopypiserver/webserver.py` & `aiopypiserver-0.0.5/src/aiopypiserver/webserver.py`

 * *Files identical despite different names*

### Comparing `aiopypiserver-0.0.4/src/aiopypiserver.egg-info/PKG-INFO` & `aiopypiserver-0.0.5/src/aiopypiserver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: aiopypiserver
-Version: 0.0.4
+Version: 0.0.5
 Summary: Do what pypiserver does, but with aiohttp.
 Author: Jamie Walton
 Project-URL: Homepage, https://github.com/jamie0walton/aiopypiserver
 Project-URL: Bug Tracker, https://github.com/jamie0walton/aiopypiserver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aiopypiserver
 
 A basic PyPi server using aiohttp to serve web pages. Intended to work behind
```

### Comparing `aiopypiserver-0.0.4/src/aiopypiserver.egg-info/SOURCES.txt` & `aiopypiserver-0.0.5/src/aiopypiserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiopypiserver-0.0.4/tests/test_server.py` & `aiopypiserver-0.0.5/tests/test_server.py`

 * *Files identical despite different names*

