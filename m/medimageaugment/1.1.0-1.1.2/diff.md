# Comparing `tmp/medimageaugment-1.1.0.tar.gz` & `tmp/medimageaugment-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medimageaugment-1.1.0.tar", last modified: Sat Jul 22 06:20:21 2023, max compression
+gzip compressed data, was "medimageaugment-1.1.2.tar", last modified: Sat Jul 22 06:29:56 2023, max compression
```

## Comparing `medimageaugment-1.1.0.tar` & `medimageaugment-1.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 06:20:21.138333 medimageaugment-1.1.0/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1077 2023-07-22 06:19:31.000000 medimageaugment-1.1.0/LICENSE
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      798 2023-07-22 06:20:21.137699 medimageaugment-1.1.0/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15277 2023-07-22 06:19:55.000000 medimageaugment-1.1.0/README.md
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 06:20:21.136724 medimageaugment-1.1.0/medimageaugment.egg-info/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      798 2023-07-22 06:20:20.000000 medimageaugment-1.1.0/medimageaugment.egg-info/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      220 2023-07-22 06:20:20.000000 medimageaugment-1.1.0/medimageaugment.egg-info/SOURCES.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 06:20:20.000000 medimageaugment-1.1.0/medimageaugment.egg-info/dependency_links.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 06:20:20.000000 medimageaugment-1.1.0/medimageaugment.egg-info/requires.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 06:20:20.000000 medimageaugment-1.1.0/medimageaugment.egg-info/top_level.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 06:20:21.138599 medimageaugment-1.1.0/setup.cfg
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      996 2023-07-22 06:19:47.000000 medimageaugment-1.1.0/setup.py
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 06:29:56.000575 medimageaugment-1.1.2/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1077 2023-07-22 06:19:31.000000 medimageaugment-1.1.2/LICENSE
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      798 2023-07-22 06:29:55.999903 medimageaugment-1.1.2/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15277 2023-07-22 06:24:59.000000 medimageaugment-1.1.2/README.md
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 06:29:55.998892 medimageaugment-1.1.2/medimageaugment.egg-info/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      798 2023-07-22 06:29:55.000000 medimageaugment-1.1.2/medimageaugment.egg-info/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      220 2023-07-22 06:29:55.000000 medimageaugment-1.1.2/medimageaugment.egg-info/SOURCES.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 06:29:55.000000 medimageaugment-1.1.2/medimageaugment.egg-info/dependency_links.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 06:29:55.000000 medimageaugment-1.1.2/medimageaugment.egg-info/requires.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 06:29:55.000000 medimageaugment-1.1.2/medimageaugment.egg-info/top_level.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 06:29:56.000853 medimageaugment-1.1.2/setup.cfg
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      996 2023-07-22 06:29:31.000000 medimageaugment-1.1.2/setup.py
```

### Comparing `medimageaugment-1.1.0/LICENSE` & `medimageaugment-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medimageaugment-1.1.0/PKG-INFO` & `medimageaugment-1.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medimageaugment
-Version: 1.1.0
+Version: 1.1.2
 Summary: A Python class for image augmentation
 Home-page: https://github.com/himanalot/medimageaugment
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
```

### Comparing `medimageaugment-1.1.0/README.md` & `medimageaugment-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `medimageaugment-1.1.0/medimageaugment.egg-info/PKG-INFO` & `medimageaugment-1.1.2/medimageaugment.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medimageaugment
-Version: 1.1.0
+Version: 1.1.2
 Summary: A Python class for image augmentation
 Home-page: https://github.com/himanalot/medimageaugment
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
```

### Comparing `medimageaugment-1.1.0/setup.py` & `medimageaugment-1.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medimageaugment',
-    version='1.1.0',
+    version='1.1.2',
     description='A Python class for image augmentation',
     author='Your Name',
     author_email='your.email@example.com',
     url='https://github.com/himanalot/medimageaugment',
     packages=find_packages(),
     install_requires=[
         'numpy',
```

