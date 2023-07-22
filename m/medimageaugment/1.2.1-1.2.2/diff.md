# Comparing `tmp/medimageaugment-1.2.1.tar.gz` & `tmp/medimageaugment-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medimageaugment-1.2.1.tar", last modified: Sat Jul 22 06:54:43 2023, max compression
+gzip compressed data, was "medimageaugment-1.2.2.tar", last modified: Sat Jul 22 07:11:09 2023, max compression
```

## Comparing `medimageaugment-1.2.1.tar` & `medimageaugment-1.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 06:54:43.697354 medimageaugment-1.2.1/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1077 2023-07-22 06:45:25.000000 medimageaugment-1.2.1/LICENSE
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      798 2023-07-22 06:54:43.696391 medimageaugment-1.2.1/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    14911 2023-07-22 06:53:59.000000 medimageaugment-1.2.1/README.md
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 06:54:43.694018 medimageaugment-1.2.1/medimageaugment.egg-info/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      798 2023-07-22 06:54:43.000000 medimageaugment-1.2.1/medimageaugment.egg-info/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      220 2023-07-22 06:54:43.000000 medimageaugment-1.2.1/medimageaugment.egg-info/SOURCES.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 06:54:43.000000 medimageaugment-1.2.1/medimageaugment.egg-info/dependency_links.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 06:54:43.000000 medimageaugment-1.2.1/medimageaugment.egg-info/requires.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 06:54:43.000000 medimageaugment-1.2.1/medimageaugment.egg-info/top_level.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 06:54:43.697779 medimageaugment-1.2.1/setup.cfg
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      996 2023-07-22 06:54:40.000000 medimageaugment-1.2.1/setup.py
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 07:11:09.698321 medimageaugment-1.2.2/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1077 2023-07-22 06:45:25.000000 medimageaugment-1.2.2/LICENSE
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15751 2023-07-22 07:11:09.697313 medimageaugment-1.2.2/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    14911 2023-07-22 06:53:59.000000 medimageaugment-1.2.2/README.md
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 07:11:09.694632 medimageaugment-1.2.2/medimageaugment.egg-info/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15751 2023-07-22 07:11:09.000000 medimageaugment-1.2.2/medimageaugment.egg-info/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      220 2023-07-22 07:11:09.000000 medimageaugment-1.2.2/medimageaugment.egg-info/SOURCES.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 07:11:09.000000 medimageaugment-1.2.2/medimageaugment.egg-info/dependency_links.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 07:11:09.000000 medimageaugment-1.2.2/medimageaugment.egg-info/requires.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 07:11:09.000000 medimageaugment-1.2.2/medimageaugment.egg-info/top_level.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 07:11:09.698778 medimageaugment-1.2.2/setup.cfg
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1094 2023-07-22 07:11:05.000000 medimageaugment-1.2.2/setup.py
```

### Comparing `medimageaugment-1.2.1/LICENSE` & `medimageaugment-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medimageaugment-1.2.1/README.md` & `medimageaugment-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `medimageaugment-1.2.1/setup.py` & `medimageaugment-1.2.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medimageaugment',
-    version='1.2.1',
+    version='1.2.2',
     description='A Python class for image augmentation',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     author='Your Name',
     author_email='your.email@example.com',
     url='https://github.com/himanalot/medimageaugment',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scipy',
```

