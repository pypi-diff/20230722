# Comparing `tmp/pydiff-planetarium-assignment-0.0.3.tar.gz` & `tmp/pydiff-planetarium-assignment-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiff-planetarium-assignment-0.0.3.tar", last modified: Sat Jul 22 15:28:00 2023, max compression
+gzip compressed data, was "pydiff-planetarium-assignment-0.0.4.tar", last modified: Sat Jul 22 15:30:43 2023, max compression
```

## Comparing `pydiff-planetarium-assignment-0.0.3.tar` & `pydiff-planetarium-assignment-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 15:28:00.300201 pydiff-planetarium-assignment-0.0.3/
--rw-r--r--   0 channprj   (501) staff       (20)     2291 2023-07-22 15:28:00.300100 pydiff-planetarium-assignment-0.0.3/PKG-INFO
--rw-r--r--   0 channprj   (501) staff       (20)     1860 2023-07-22 15:27:00.000000 pydiff-planetarium-assignment-0.0.3/README.md
-drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 15:28:00.299208 pydiff-planetarium-assignment-0.0.3/pydiff_planetarium_assignment/
-drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 15:28:00.299960 pydiff-planetarium-assignment-0.0.3/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/
--rw-r--r--   0 channprj   (501) staff       (20)     2291 2023-07-22 15:28:00.000000 pydiff-planetarium-assignment-0.0.3/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/PKG-INFO
--rw-r--r--   0 channprj   (501) staff       (20)      365 2023-07-22 15:28:00.000000 pydiff-planetarium-assignment-0.0.3/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/SOURCES.txt
--rw-r--r--   0 channprj   (501) staff       (20)        1 2023-07-22 15:28:00.000000 pydiff-planetarium-assignment-0.0.3/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/dependency_links.txt
--rw-r--r--   0 channprj   (501) staff       (20)        1 2023-07-22 15:28:00.000000 pydiff-planetarium-assignment-0.0.3/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/top_level.txt
--rw-r--r--   0 channprj   (501) staff       (20)      104 2023-07-22 14:45:33.000000 pydiff-planetarium-assignment-0.0.3/pyproject.toml
--rw-r--r--   0 channprj   (501) staff       (20)       38 2023-07-22 15:28:00.300229 pydiff-planetarium-assignment-0.0.3/setup.cfg
--rw-r--r--   0 channprj   (501) staff       (20)      789 2023-07-22 15:27:27.000000 pydiff-planetarium-assignment-0.0.3/setup.py
+drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 15:30:43.031307 pydiff-planetarium-assignment-0.0.4/
+-rw-r--r--   0 channprj   (501) staff       (20)     2291 2023-07-22 15:30:43.031209 pydiff-planetarium-assignment-0.0.4/PKG-INFO
+-rw-r--r--   0 channprj   (501) staff       (20)     1860 2023-07-22 15:27:00.000000 pydiff-planetarium-assignment-0.0.4/README.md
+drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 15:30:43.030314 pydiff-planetarium-assignment-0.0.4/pydiff_planetarium_assignment/
+drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 15:30:43.031069 pydiff-planetarium-assignment-0.0.4/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/
+-rw-r--r--   0 channprj   (501) staff       (20)     2291 2023-07-22 15:30:43.000000 pydiff-planetarium-assignment-0.0.4/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/PKG-INFO
+-rw-r--r--   0 channprj   (501) staff       (20)      365 2023-07-22 15:30:43.000000 pydiff-planetarium-assignment-0.0.4/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/SOURCES.txt
+-rw-r--r--   0 channprj   (501) staff       (20)        1 2023-07-22 15:30:43.000000 pydiff-planetarium-assignment-0.0.4/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/dependency_links.txt
+-rw-r--r--   0 channprj   (501) staff       (20)        1 2023-07-22 15:30:43.000000 pydiff-planetarium-assignment-0.0.4/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/top_level.txt
+-rw-r--r--   0 channprj   (501) staff       (20)      104 2023-07-22 14:45:33.000000 pydiff-planetarium-assignment-0.0.4/pyproject.toml
+-rw-r--r--   0 channprj   (501) staff       (20)       38 2023-07-22 15:30:43.031339 pydiff-planetarium-assignment-0.0.4/setup.cfg
+-rw-r--r--   0 channprj   (501) staff       (20)      815 2023-07-22 15:30:26.000000 pydiff-planetarium-assignment-0.0.4/setup.py
```

### Comparing `pydiff-planetarium-assignment-0.0.3/PKG-INFO` & `pydiff-planetarium-assignment-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydiff-planetarium-assignment
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple implementation of unix diff
 Home-page: https://github.com/planetarium/take-home-2023-channprj
 Author: channprj
 Author-email: chann@chann.dev
 Project-URL: Bug Tracker, https://github.com/planetarium/take-home-2023-channprj/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
```

### Comparing `pydiff-planetarium-assignment-0.0.3/README.md` & `pydiff-planetarium-assignment-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pydiff-planetarium-assignment-0.0.3/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/PKG-INFO` & `pydiff-planetarium-assignment-0.0.4/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydiff-planetarium-assignment
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple implementation of unix diff
 Home-page: https://github.com/planetarium/take-home-2023-channprj
 Author: channprj
 Author-email: chann@chann.dev
 Project-URL: Bug Tracker, https://github.com/planetarium/take-home-2023-channprj/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
```

### Comparing `pydiff-planetarium-assignment-0.0.3/setup.py` & `pydiff-planetarium-assignment-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pydiff-planetarium-assignment',
-    version='0.0.3',
+    version='0.0.4',
     author='channprj',
     author_email='chann@chann.dev',
     description='Simple implementation of unix diff',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/planetarium/take-home-2023-channprj',
     project_urls={
         'Bug Tracker':
         'https://github.com/planetarium/take-home-2023-channprj/issues',
     },
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
     package_dir={'': 'pydiff_planetarium_assignment'},
-    packages=setuptools.find_packages(where='src'),
+    packages=setuptools.find_packages(where='pydiff_planetarium_assignment'),
     python_requires='>=3.11',
 )
```

