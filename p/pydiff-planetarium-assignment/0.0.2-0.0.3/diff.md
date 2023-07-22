# Comparing `tmp/pydiff-planetarium-assignment-0.0.2.tar.gz` & `tmp/pydiff-planetarium-assignment-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiff-planetarium-assignment-0.0.2.tar", last modified: Sat Jul 22 14:59:27 2023, max compression
+gzip compressed data, was "pydiff-planetarium-assignment-0.0.3.tar", last modified: Sat Jul 22 15:28:00 2023, max compression
```

## Comparing `pydiff-planetarium-assignment-0.0.2.tar` & `pydiff-planetarium-assignment-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 14:59:27.578586 pydiff-planetarium-assignment-0.0.2/
--rw-r--r--   0 channprj   (501) staff       (20)     1866 2023-07-22 14:59:27.578480 pydiff-planetarium-assignment-0.0.2/PKG-INFO
--rw-r--r--   0 channprj   (501) staff       (20)     1435 2023-07-22 14:57:37.000000 pydiff-planetarium-assignment-0.0.2/README.md
-drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 14:59:27.577467 pydiff-planetarium-assignment-0.0.2/pydiff_planetarium_assignment/
-drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 14:59:27.578317 pydiff-planetarium-assignment-0.0.2/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/
--rw-r--r--   0 channprj   (501) staff       (20)     1866 2023-07-22 14:59:27.000000 pydiff-planetarium-assignment-0.0.2/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/PKG-INFO
--rw-r--r--   0 channprj   (501) staff       (20)      365 2023-07-22 14:59:27.000000 pydiff-planetarium-assignment-0.0.2/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/SOURCES.txt
--rw-r--r--   0 channprj   (501) staff       (20)        1 2023-07-22 14:59:27.000000 pydiff-planetarium-assignment-0.0.2/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/dependency_links.txt
--rw-r--r--   0 channprj   (501) staff       (20)        1 2023-07-22 14:59:27.000000 pydiff-planetarium-assignment-0.0.2/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/top_level.txt
--rw-r--r--   0 channprj   (501) staff       (20)      104 2023-07-22 14:45:33.000000 pydiff-planetarium-assignment-0.0.2/pyproject.toml
--rw-r--r--   0 channprj   (501) staff       (20)       38 2023-07-22 14:59:27.578618 pydiff-planetarium-assignment-0.0.2/setup.cfg
--rw-r--r--   0 channprj   (501) staff       (20)      789 2023-07-22 14:59:23.000000 pydiff-planetarium-assignment-0.0.2/setup.py
+drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 15:28:00.300201 pydiff-planetarium-assignment-0.0.3/
+-rw-r--r--   0 channprj   (501) staff       (20)     2291 2023-07-22 15:28:00.300100 pydiff-planetarium-assignment-0.0.3/PKG-INFO
+-rw-r--r--   0 channprj   (501) staff       (20)     1860 2023-07-22 15:27:00.000000 pydiff-planetarium-assignment-0.0.3/README.md
+drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 15:28:00.299208 pydiff-planetarium-assignment-0.0.3/pydiff_planetarium_assignment/
+drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 15:28:00.299960 pydiff-planetarium-assignment-0.0.3/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/
+-rw-r--r--   0 channprj   (501) staff       (20)     2291 2023-07-22 15:28:00.000000 pydiff-planetarium-assignment-0.0.3/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/PKG-INFO
+-rw-r--r--   0 channprj   (501) staff       (20)      365 2023-07-22 15:28:00.000000 pydiff-planetarium-assignment-0.0.3/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/SOURCES.txt
+-rw-r--r--   0 channprj   (501) staff       (20)        1 2023-07-22 15:28:00.000000 pydiff-planetarium-assignment-0.0.3/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/dependency_links.txt
+-rw-r--r--   0 channprj   (501) staff       (20)        1 2023-07-22 15:28:00.000000 pydiff-planetarium-assignment-0.0.3/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/top_level.txt
+-rw-r--r--   0 channprj   (501) staff       (20)      104 2023-07-22 14:45:33.000000 pydiff-planetarium-assignment-0.0.3/pyproject.toml
+-rw-r--r--   0 channprj   (501) staff       (20)       38 2023-07-22 15:28:00.300229 pydiff-planetarium-assignment-0.0.3/setup.cfg
+-rw-r--r--   0 channprj   (501) staff       (20)      789 2023-07-22 15:27:27.000000 pydiff-planetarium-assignment-0.0.3/setup.py
```

### Comparing `pydiff-planetarium-assignment-0.0.2/setup.py` & `pydiff-planetarium-assignment-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pydiff-planetarium-assignment',
-    version='0.0.2',
+    version='0.0.3',
     author='channprj',
     author_email='chann@chann.dev',
     description='Simple implementation of unix diff',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/planetarium/take-home-2023-channprj',
     project_urls={
```

