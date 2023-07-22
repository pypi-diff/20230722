# Comparing `tmp/pathgenmap-0.0.9.tar.gz` & `tmp/pathgenmap-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathgenmap-0.0.9.tar", last modified: Fri Jul 14 00:10:14 2023, max compression
+gzip compressed data, was "pathgenmap-0.1.0.tar", last modified: Sat Jul 22 17:23:00 2023, max compression
```

## Comparing `pathgenmap-0.0.9.tar` & `pathgenmap-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-14 00:10:14.500530 pathgenmap-0.0.9/
--rw-r--r--   0 marcossousa   (501) staff       (20)     1083 2023-07-13 00:05:25.000000 pathgenmap-0.0.9/LICENSE
--rw-r--r--   0 marcossousa   (501) staff       (20)      422 2023-07-14 00:10:14.499904 pathgenmap-0.0.9/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)      740 2023-07-13 21:56:31.000000 pathgenmap-0.0.9/README.md
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-14 00:10:14.493083 pathgenmap-0.0.9/pathgenmap/
--rw-r--r--   0 marcossousa   (501) staff       (20)     1307 2023-07-13 00:07:52.000000 pathgenmap-0.0.9/pathgenmap/EggAnnot.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     3014 2023-07-14 00:10:06.000000 pathgenmap-0.0.9/pathgenmap/Integration.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     1889 2023-07-13 11:28:07.000000 pathgenmap-0.0.9/pathgenmap/PathAnalys.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     1140 2023-07-14 00:06:16.000000 pathgenmap-0.0.9/pathgenmap/PathGenMap.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     1205 2023-07-13 11:46:42.000000 pathgenmap-0.0.9/pathgenmap/SpeciesAbundance.py
--rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-07-13 00:03:39.000000 pathgenmap-0.0.9/pathgenmap/__init__.py
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-14 00:10:14.498015 pathgenmap-0.0.9/pathgenmap.egg-info/
--rw-r--r--   0 marcossousa   (501) staff       (20)      422 2023-07-14 00:10:14.000000 pathgenmap-0.0.9/pathgenmap.egg-info/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)      385 2023-07-14 00:10:14.000000 pathgenmap-0.0.9/pathgenmap.egg-info/SOURCES.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-07-14 00:10:14.000000 pathgenmap-0.0.9/pathgenmap.egg-info/dependency_links.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       59 2023-07-14 00:10:14.000000 pathgenmap-0.0.9/pathgenmap.egg-info/entry_points.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       27 2023-07-14 00:10:14.000000 pathgenmap-0.0.9/pathgenmap.egg-info/requires.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       11 2023-07-14 00:10:14.000000 pathgenmap-0.0.9/pathgenmap.egg-info/top_level.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-07-14 00:10:14.500755 pathgenmap-0.0.9/setup.cfg
--rw-r--r--   0 marcossousa   (501) staff       (20)      655 2023-07-14 00:10:06.000000 pathgenmap-0.0.9/setup.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:23:00.367612 pathgenmap-0.1.0/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1083 2023-07-22 17:15:46.000000 pathgenmap-0.1.0/LICENSE
+-rw-r--r--   0 marcossousa   (501) staff       (20)      394 2023-07-22 17:23:00.366692 pathgenmap-0.1.0/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      739 2023-07-22 17:22:11.000000 pathgenmap-0.1.0/README.md
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:23:00.354339 pathgenmap-0.1.0/pathgenmap/
+-rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:09:59.000000 pathgenmap-0.1.0/pathgenmap/__init__.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)      788 2023-07-22 17:10:43.000000 pathgenmap-0.1.0/pathgenmap/pathgenmap.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     2939 2023-07-22 15:45:28.000000 pathgenmap-0.1.0/pathgenmap/pathprocess.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-22 17:23:00.364104 pathgenmap-0.1.0/pathgenmap.egg-info/
+-rw-r--r--   0 marcossousa   (501) staff       (20)      394 2023-07-22 17:23:00.000000 pathgenmap-0.1.0/pathgenmap.egg-info/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      306 2023-07-22 17:23:00.000000 pathgenmap-0.1.0/pathgenmap.egg-info/SOURCES.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-07-22 17:23:00.000000 pathgenmap-0.1.0/pathgenmap.egg-info/dependency_links.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       58 2023-07-22 17:23:00.000000 pathgenmap-0.1.0/pathgenmap.egg-info/entry_points.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       45 2023-07-22 17:23:00.000000 pathgenmap-0.1.0/pathgenmap.egg-info/requires.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       11 2023-07-22 17:23:00.000000 pathgenmap-0.1.0/pathgenmap.egg-info/top_level.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-07-22 17:23:00.368243 pathgenmap-0.1.0/setup.cfg
+-rw-r--r--   0 marcossousa   (501) staff       (20)      694 2023-07-22 17:21:32.000000 pathgenmap-0.1.0/setup.py
```

### Comparing `pathgenmap-0.0.9/LICENSE` & `pathgenmap-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.9/README.md` & `pathgenmap-0.1.0/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 python PathGenMap.py <pathway_file> <annotation_file> <species_abundance_file>
 ```
 
 The output will be written to an output file in the same directory.
 
 ```
 Please replace <pathway_file>, <annotation_file>, and <species_abundance_file> with your actual file paths.
-```
+```
```

### Comparing `pathgenmap-0.0.9/setup.py` & `pathgenmap-0.1.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pathgenmap",
-    version="0.0.9",
+    version="0.1.0",
     packages=find_packages(),
-    install_requires=["pandas>=1.1.0", "tqdm>=4.48.0"],
+    install_requires=["pandas>=1.1.0", "tqdm>=4.48.0", "matplotlib>=3.1.1"],
     author="Marcos Paulo Alves de Sousa",
     author_email="msousa@museu-goeldi.br",
-    description="PathGenMap is a comprehensive Python application designed to integrate pathway, annotation, and species abundance data.",
+    description="PathGenMap is a comprehensive Python application designed to integrate pathway, annotation, "
+                "and species abundance data.",
     license="MIT",
     keywords="pathway annotation species abundance",
     url="http://github.com/marcos-de-sousa/pathgenmap",
     entry_points={
         'console_scripts': [
-            'pathgenmap=pathgenmap.PathGenMap:main',
+            'pathgenmap=pathgenmap.pathgenmap:main',
         ],
     },
-)
+)
```

