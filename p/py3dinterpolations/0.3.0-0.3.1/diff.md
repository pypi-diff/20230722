# Comparing `tmp/py3dinterpolations-0.3.0.tar.gz` & `tmp/py3dinterpolations-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3dinterpolations-0.3.0.tar", last modified: Sat Jul 22 01:15:21 2023, max compression
+gzip compressed data, was "py3dinterpolations-0.3.1.tar", last modified: Sat Jul 22 01:15:39 2023, max compression
```

## Comparing `py3dinterpolations-0.3.0.tar` & `py3dinterpolations-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:15:21.135690 py3dinterpolations-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-22 01:15:08.000000 py3dinterpolations-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-22 01:15:21.135690 py3dinterpolations-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-22 01:15:08.000000 py3dinterpolations-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:15:21.135690 py3dinterpolations-0.3.0/py3dinterpolations/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-22 01:15:08.000000 py3dinterpolations-0.3.0/py3dinterpolations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:15:21.135690 py3dinterpolations-0.3.0/py3dinterpolations/core/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-22 01:15:08.000000 py3dinterpolations-0.3.0/py3dinterpolations/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-22 01:15:08.000000 py3dinterpolations-0.3.0/py3dinterpolations/core/grid3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-22 01:15:08.000000 py3dinterpolations-0.3.0/py3dinterpolations/core/griddata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:15:21.135690 py3dinterpolations-0.3.0/py3dinterpolations/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 01:15:08.000000 py3dinterpolations-0.3.0/py3dinterpolations/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-22 01:15:08.000000 py3dinterpolations-0.3.0/py3dinterpolations/plotting/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:15:21.135690 py3dinterpolations-0.3.0/py3dinterpolations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-22 01:15:21.000000 py3dinterpolations-0.3.0/py3dinterpolations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-22 01:15:21.000000 py3dinterpolations-0.3.0/py3dinterpolations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 01:15:21.000000 py3dinterpolations-0.3.0/py3dinterpolations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-22 01:15:21.000000 py3dinterpolations-0.3.0/py3dinterpolations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-22 01:15:21.000000 py3dinterpolations-0.3.0/py3dinterpolations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 01:15:21.135690 py3dinterpolations-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-22 01:15:08.000000 py3dinterpolations-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:15:38.996550 py3dinterpolations-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-22 01:15:29.000000 py3dinterpolations-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-22 01:15:38.996550 py3dinterpolations-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-22 01:15:29.000000 py3dinterpolations-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:15:38.996550 py3dinterpolations-0.3.1/py3dinterpolations/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-22 01:15:29.000000 py3dinterpolations-0.3.1/py3dinterpolations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:15:38.996550 py3dinterpolations-0.3.1/py3dinterpolations/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-22 01:15:29.000000 py3dinterpolations-0.3.1/py3dinterpolations/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-22 01:15:29.000000 py3dinterpolations-0.3.1/py3dinterpolations/core/grid3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-22 01:15:29.000000 py3dinterpolations-0.3.1/py3dinterpolations/core/griddata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:15:38.996550 py3dinterpolations-0.3.1/py3dinterpolations/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 01:15:29.000000 py3dinterpolations-0.3.1/py3dinterpolations/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-22 01:15:29.000000 py3dinterpolations-0.3.1/py3dinterpolations/plotting/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:15:38.996550 py3dinterpolations-0.3.1/py3dinterpolations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-22 01:15:38.000000 py3dinterpolations-0.3.1/py3dinterpolations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-22 01:15:38.000000 py3dinterpolations-0.3.1/py3dinterpolations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 01:15:38.000000 py3dinterpolations-0.3.1/py3dinterpolations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-22 01:15:38.000000 py3dinterpolations-0.3.1/py3dinterpolations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-22 01:15:38.000000 py3dinterpolations-0.3.1/py3dinterpolations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 01:15:38.996550 py3dinterpolations-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-22 01:15:29.000000 py3dinterpolations-0.3.1/setup.py
```

### Comparing `py3dinterpolations-0.3.0/LICENSE` & `py3dinterpolations-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py3dinterpolations-0.3.0/PKG-INFO` & `py3dinterpolations-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dinterpolations
-Version: 0.3.0
+Version: 0.3.1
 Summary: quick 3D interpolation with python
 Home-page: https://github.com/giocaizzi/py3dinterpolations
 Author: giocaizzi
 Author-email: giocaizzi@gmail.com
 License: MIT
 Project-URL: Documentation, https://giocaizzi.github.io/py3dinterpolations/
 Project-URL: Bug Reports, https://github.com/giocaizzi/py3dinterpolations/issues
```

### Comparing `py3dinterpolations-0.3.0/README.md` & `py3dinterpolations-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `py3dinterpolations-0.3.0/py3dinterpolations/core/__init__.py` & `py3dinterpolations-0.3.1/py3dinterpolations/core/__init__.py`

 * *Files identical despite different names*

### Comparing `py3dinterpolations-0.3.0/py3dinterpolations/core/grid3d.py` & `py3dinterpolations-0.3.1/py3dinterpolations/core/grid3d.py`

 * *Files identical despite different names*

### Comparing `py3dinterpolations-0.3.0/py3dinterpolations/core/griddata.py` & `py3dinterpolations-0.3.1/py3dinterpolations/core/griddata.py`

 * *Files identical despite different names*

### Comparing `py3dinterpolations-0.3.0/py3dinterpolations/plotting/plotting.py` & `py3dinterpolations-0.3.1/py3dinterpolations/plotting/plotting.py`

 * *Files identical despite different names*

### Comparing `py3dinterpolations-0.3.0/py3dinterpolations.egg-info/PKG-INFO` & `py3dinterpolations-0.3.1/py3dinterpolations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dinterpolations
-Version: 0.3.0
+Version: 0.3.1
 Summary: quick 3D interpolation with python
 Home-page: https://github.com/giocaizzi/py3dinterpolations
 Author: giocaizzi
 Author-email: giocaizzi@gmail.com
 License: MIT
 Project-URL: Documentation, https://giocaizzi.github.io/py3dinterpolations/
 Project-URL: Bug Reports, https://github.com/giocaizzi/py3dinterpolations/issues
```

### Comparing `py3dinterpolations-0.3.0/setup.py` & `py3dinterpolations-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="py3dinterpolations",
-    version="0.3.0",
+    version="0.3.1",
     description="quick 3D interpolation with python",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/giocaizzi/py3dinterpolations",
     author="giocaizzi",
     author_email="giocaizzi@gmail.com",
     license="MIT",
```

