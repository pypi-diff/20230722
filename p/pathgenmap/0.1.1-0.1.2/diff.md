# Comparing `tmp/pathgenmap-0.1.1.tar.gz` & `tmp/pathgenmap-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathgenmap-0.1.1.tar", last modified: Sat Jul 22 17:40:59 2023, max compression
+gzip compressed data, was "pathgenmap-0.1.2.tar", last modified: Sat Jul 22 17:48:00 2023, max compression
```

## Comparing `pathgenmap-0.1.1.tar` & `pathgenmap-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:40:59.248585 pathgenmap-0.1.1/
--rw-r--r--   0 marcossousa   (501) staff       (20)     1083 2023-07-22 17:15:46.000000 pathgenmap-0.1.1/LICENSE
--rw-r--r--   0 marcossousa   (501) staff       (20)      394 2023-07-22 17:40:59.247425 pathgenmap-0.1.1/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)      739 2023-07-22 17:22:11.000000 pathgenmap-0.1.1/README.md
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:40:59.239211 pathgenmap-0.1.1/pathgenmap/
--rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:09:59.000000 pathgenmap-0.1.1/pathgenmap/__init__.py
--rw-r--r--   0 marcossousa   (501) staff       (20)      788 2023-07-22 17:10:43.000000 pathgenmap-0.1.1/pathgenmap/pathgenmap.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     2939 2023-07-22 15:45:28.000000 pathgenmap-0.1.1/pathgenmap/pathprocess.py
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:40:59.246418 pathgenmap-0.1.1/pathgenmap.egg-info/
--rw-r--r--   0 marcossousa   (501) staff       (20)      394 2023-07-22 17:40:59.000000 pathgenmap-0.1.1/pathgenmap.egg-info/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)      306 2023-07-22 17:40:59.000000 pathgenmap-0.1.1/pathgenmap.egg-info/SOURCES.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-07-22 17:40:59.000000 pathgenmap-0.1.1/pathgenmap.egg-info/dependency_links.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       58 2023-07-22 17:40:59.000000 pathgenmap-0.1.1/pathgenmap.egg-info/entry_points.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       45 2023-07-22 17:40:59.000000 pathgenmap-0.1.1/pathgenmap.egg-info/requires.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       11 2023-07-22 17:40:59.000000 pathgenmap-0.1.1/pathgenmap.egg-info/top_level.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-07-22 17:40:59.249369 pathgenmap-0.1.1/setup.cfg
--rw-r--r--   0 marcossousa   (501) staff       (20)      694 2023-07-22 17:40:26.000000 pathgenmap-0.1.1/setup.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:48:00.322236 pathgenmap-0.1.2/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1083 2023-07-22 17:15:46.000000 pathgenmap-0.1.2/LICENSE
+-rw-r--r--   0 marcossousa   (501) staff       (20)      394 2023-07-22 17:48:00.321172 pathgenmap-0.1.2/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      739 2023-07-22 17:22:11.000000 pathgenmap-0.1.2/README.md
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:48:00.314067 pathgenmap-0.1.2/pathgenmap/
+-rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:09:59.000000 pathgenmap-0.1.2/pathgenmap/__init__.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)      788 2023-07-22 17:10:43.000000 pathgenmap-0.1.2/pathgenmap/pathgenmap.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     2939 2023-07-22 15:45:28.000000 pathgenmap-0.1.2/pathgenmap/pathprocess.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:48:00.319883 pathgenmap-0.1.2/pathgenmap.egg-info/
+-rw-r--r--   0 marcossousa   (501) staff       (20)      394 2023-07-22 17:48:00.000000 pathgenmap-0.1.2/pathgenmap.egg-info/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      306 2023-07-22 17:48:00.000000 pathgenmap-0.1.2/pathgenmap.egg-info/SOURCES.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-07-22 17:48:00.000000 pathgenmap-0.1.2/pathgenmap.egg-info/dependency_links.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       58 2023-07-22 17:48:00.000000 pathgenmap-0.1.2/pathgenmap.egg-info/entry_points.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       61 2023-07-22 17:48:00.000000 pathgenmap-0.1.2/pathgenmap.egg-info/requires.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       11 2023-07-22 17:48:00.000000 pathgenmap-0.1.2/pathgenmap.egg-info/top_level.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-07-22 17:48:00.322527 pathgenmap-0.1.2/setup.cfg
+-rw-r--r--   0 marcossousa   (501) staff       (20)      752 2023-07-22 17:47:45.000000 pathgenmap-0.1.2/setup.py
```

### Comparing `pathgenmap-0.1.1/LICENSE` & `pathgenmap-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.1.1/README.md` & `pathgenmap-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.1.1/pathgenmap/pathgenmap.py` & `pathgenmap-0.1.2/pathgenmap/pathgenmap.py`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.1.1/pathgenmap/pathprocess.py` & `pathgenmap-0.1.2/pathgenmap/pathprocess.py`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.1.1/setup.py` & `pathgenmap-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pathgenmap",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
-    install_requires=["pandas>=1.1.0", "tqdm>=4.48.0", "matplotlib>=3.1.1"],
+    install_requires=[
+        "pandas>=1.1.0",
+        "tqdm>=4.48.0",
+        "matplotlib>=3.1.1",
+        "biopython>=1.78"
+    ],
     author="Marcos Paulo Alves de Sousa",
     author_email="msousa@museu-goeldi.br",
     description="PathGenMap is a comprehensive Python application designed to integrate pathway, annotation, "
                 "and species abundance data.",
     license="MIT",
     keywords="pathway annotation species abundance",
     url="http://github.com/marcos-de-sousa/pathgenmap",
     entry_points={
         'console_scripts': [
             'pathgenmap=pathgenmap.pathgenmap:main',
         ],
     },
-)
+)
```

