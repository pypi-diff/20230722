# Comparing `tmp/pathgenmap-0.1.0.tar.gz` & `tmp/pathgenmap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathgenmap-0.1.0.tar", last modified: Sat Jul 22 17:23:00 2023, max compression
+gzip compressed data, was "pathgenmap-0.1.1.tar", last modified: Sat Jul 22 17:40:59 2023, max compression
```

## Comparing `pathgenmap-0.1.0.tar` & `pathgenmap-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:23:00.367612 pathgenmap-0.1.0/
--rw-r--r--   0 marcossousa   (501) staff       (20)     1083 2023-07-22 17:15:46.000000 pathgenmap-0.1.0/LICENSE
--rw-r--r--   0 marcossousa   (501) staff       (20)      394 2023-07-22 17:23:00.366692 pathgenmap-0.1.0/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)      739 2023-07-22 17:22:11.000000 pathgenmap-0.1.0/README.md
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:23:00.354339 pathgenmap-0.1.0/pathgenmap/
--rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:09:59.000000 pathgenmap-0.1.0/pathgenmap/__init__.py
--rw-r--r--   0 marcossousa   (501) staff       (20)      788 2023-07-22 17:10:43.000000 pathgenmap-0.1.0/pathgenmap/pathgenmap.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     2939 2023-07-22 15:45:28.000000 pathgenmap-0.1.0/pathgenmap/pathprocess.py
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:23:00.364104 pathgenmap-0.1.0/pathgenmap.egg-info/
--rw-r--r--   0 marcossousa   (501) staff       (20)      394 2023-07-22 17:23:00.000000 pathgenmap-0.1.0/pathgenmap.egg-info/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)      306 2023-07-22 17:23:00.000000 pathgenmap-0.1.0/pathgenmap.egg-info/SOURCES.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-07-22 17:23:00.000000 pathgenmap-0.1.0/pathgenmap.egg-info/dependency_links.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       58 2023-07-22 17:23:00.000000 pathgenmap-0.1.0/pathgenmap.egg-info/entry_points.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       45 2023-07-22 17:23:00.000000 pathgenmap-0.1.0/pathgenmap.egg-info/requires.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       11 2023-07-22 17:23:00.000000 pathgenmap-0.1.0/pathgenmap.egg-info/top_level.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-07-22 17:23:00.368243 pathgenmap-0.1.0/setup.cfg
--rw-r--r--   0 marcossousa   (501) staff       (20)      694 2023-07-22 17:21:32.000000 pathgenmap-0.1.0/setup.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:40:59.248585 pathgenmap-0.1.1/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1083 2023-07-22 17:15:46.000000 pathgenmap-0.1.1/LICENSE
+-rw-r--r--   0 marcossousa   (501) staff       (20)      394 2023-07-22 17:40:59.247425 pathgenmap-0.1.1/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      739 2023-07-22 17:22:11.000000 pathgenmap-0.1.1/README.md
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:40:59.239211 pathgenmap-0.1.1/pathgenmap/
+-rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:09:59.000000 pathgenmap-0.1.1/pathgenmap/__init__.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)      788 2023-07-22 17:10:43.000000 pathgenmap-0.1.1/pathgenmap/pathgenmap.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     2939 2023-07-22 15:45:28.000000 pathgenmap-0.1.1/pathgenmap/pathprocess.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:40:59.246418 pathgenmap-0.1.1/pathgenmap.egg-info/
+-rw-r--r--   0 marcossousa   (501) staff       (20)      394 2023-07-22 17:40:59.000000 pathgenmap-0.1.1/pathgenmap.egg-info/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      306 2023-07-22 17:40:59.000000 pathgenmap-0.1.1/pathgenmap.egg-info/SOURCES.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-07-22 17:40:59.000000 pathgenmap-0.1.1/pathgenmap.egg-info/dependency_links.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       58 2023-07-22 17:40:59.000000 pathgenmap-0.1.1/pathgenmap.egg-info/entry_points.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       45 2023-07-22 17:40:59.000000 pathgenmap-0.1.1/pathgenmap.egg-info/requires.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       11 2023-07-22 17:40:59.000000 pathgenmap-0.1.1/pathgenmap.egg-info/top_level.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-07-22 17:40:59.249369 pathgenmap-0.1.1/setup.cfg
+-rw-r--r--   0 marcossousa   (501) staff       (20)      694 2023-07-22 17:40:26.000000 pathgenmap-0.1.1/setup.py
```

### Comparing `pathgenmap-0.1.0/LICENSE` & `pathgenmap-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.1.0/README.md` & `pathgenmap-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.1.0/pathgenmap/pathgenmap.py` & `pathgenmap-0.1.1/pathgenmap/pathgenmap.py`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.1.0/pathgenmap/pathprocess.py` & `pathgenmap-0.1.1/pathgenmap/pathprocess.py`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.1.0/setup.py` & `pathgenmap-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pathgenmap",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=["pandas>=1.1.0", "tqdm>=4.48.0", "matplotlib>=3.1.1"],
     author="Marcos Paulo Alves de Sousa",
     author_email="msousa@museu-goeldi.br",
     description="PathGenMap is a comprehensive Python application designed to integrate pathway, annotation, "
                 "and species abundance data.",
     license="MIT",
```

