# Comparing `tmp/septem-circumstantiae-0.0.2.tar.gz` & `tmp/septem-circumstantiae-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "septem-circumstantiae-0.0.2.tar", last modified: Mon Jul 10 19:39:08 2023, max compression
+gzip compressed data, was "septem-circumstantiae-0.0.3.tar", last modified: Sat Jul 22 00:39:47 2023, max compression
```

## Comparing `septem-circumstantiae-0.0.2.tar` & `septem-circumstantiae-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-10 19:39:08.369584 septem-circumstantiae-0.0.2/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1078 2023-07-09 23:53:45.000000 septem-circumstantiae-0.0.2/LICENSE
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      657 2023-07-10 19:39:08.369584 septem-circumstantiae-0.0.2/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       91 2023-07-09 23:53:45.000000 septem-circumstantiae-0.0.2/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      647 2023-07-10 19:35:51.000000 septem-circumstantiae-0.0.2/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-07-10 19:39:08.369584 septem-circumstantiae-0.0.2/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-10 19:39:08.369584 septem-circumstantiae-0.0.2/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-10 19:39:08.369584 septem-circumstantiae-0.0.2/src/septem-circumstantiae/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      322 2023-07-10 19:35:51.000000 septem-circumstantiae-0.0.2/src/septem-circumstantiae/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      625 2023-07-10 19:16:43.000000 septem-circumstantiae-0.0.2/src/septem-circumstantiae/human_events.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      586 2023-07-10 19:16:43.000000 septem-circumstantiae-0.0.2/src/septem-circumstantiae/natural_events.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-10 19:39:08.369584 septem-circumstantiae-0.0.2/src/septem_circumstantiae.egg-info/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      657 2023-07-10 19:39:08.000000 septem-circumstantiae-0.0.2/src/septem_circumstantiae.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      352 2023-07-10 19:39:08.000000 septem-circumstantiae-0.0.2/src/septem_circumstantiae.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-07-10 19:39:08.000000 septem-circumstantiae-0.0.2/src/septem_circumstantiae.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       22 2023-07-10 19:39:08.000000 septem-circumstantiae-0.0.2/src/septem_circumstantiae.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-22 00:39:47.963298 septem-circumstantiae-0.0.3/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1078 2023-07-09 23:53:45.000000 septem-circumstantiae-0.0.3/LICENSE
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      657 2023-07-22 00:39:47.963298 septem-circumstantiae-0.0.3/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       91 2023-07-09 23:53:45.000000 septem-circumstantiae-0.0.3/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      647 2023-07-22 00:37:34.000000 septem-circumstantiae-0.0.3/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-07-22 00:39:47.963298 septem-circumstantiae-0.0.3/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-22 00:39:47.959298 septem-circumstantiae-0.0.3/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-22 00:39:47.963298 septem-circumstantiae-0.0.3/src/septem-circumstantiae/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      322 2023-07-10 19:35:51.000000 septem-circumstantiae-0.0.3/src/septem-circumstantiae/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      620 2023-07-22 00:37:34.000000 septem-circumstantiae-0.0.3/src/septem-circumstantiae/events.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-22 00:39:47.963298 septem-circumstantiae-0.0.3/src/septem_circumstantiae.egg-info/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      657 2023-07-22 00:39:47.000000 septem-circumstantiae-0.0.3/src/septem_circumstantiae.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      302 2023-07-22 00:39:47.000000 septem-circumstantiae-0.0.3/src/septem_circumstantiae.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-07-22 00:39:47.000000 septem-circumstantiae-0.0.3/src/septem_circumstantiae.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       22 2023-07-22 00:39:47.000000 septem-circumstantiae-0.0.3/src/septem_circumstantiae.egg-info/top_level.txt
```

### Comparing `septem-circumstantiae-0.0.2/LICENSE` & `septem-circumstantiae-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `septem-circumstantiae-0.0.2/PKG-INFO` & `septem-circumstantiae-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: septem-circumstantiae
-Version: 0.0.2
+Version: 0.0.3
 Summary: Septem Circumstantiae
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/septem-circumstantiae/septem-circumstantiae
 Project-URL: Bug Tracker, https://github.com/septem-circumstantiae/septem-circumstantiae/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `septem-circumstantiae-0.0.2/pyproject.toml` & `septem-circumstantiae-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "septem-circumstantiae"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "Septem Circumstantiae"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
```

### Comparing `septem-circumstantiae-0.0.2/src/septem-circumstantiae/human_events.py` & `septem-circumstantiae-0.0.3/src/septem-circumstantiae/events.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 This source code is licensed under the license found in the
 LICENSE file in the root directory of this source tree.
 """
 
 # https://alxfed.github.io/blog/posts/2019/02/22/Septem-Circumstantiae.html
 
 
-class HumanEvent:
+class Event:
     """"""
     who: str    = ''  # quis
     what: str   = ''  # quid
     when: str   = ''  # quando
     where: str  = ''  # ubi
     why: str    = ''  # cur (for the sake of what?)
     how: str    = ''  # quem ad modum (in what way?)
```

### Comparing `septem-circumstantiae-0.0.2/src/septem_circumstantiae.egg-info/PKG-INFO` & `septem-circumstantiae-0.0.3/src/septem_circumstantiae.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: septem-circumstantiae
-Version: 0.0.2
+Version: 0.0.3
 Summary: Septem Circumstantiae
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/septem-circumstantiae/septem-circumstantiae
 Project-URL: Bug Tracker, https://github.com/septem-circumstantiae/septem-circumstantiae/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

