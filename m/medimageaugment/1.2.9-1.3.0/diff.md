# Comparing `tmp/medimageaugment-1.2.9.tar.gz` & `tmp/medimageaugment-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medimageaugment-1.2.9.tar", last modified: Sat Jul 22 19:37:48 2023, max compression
+gzip compressed data, was "medimageaugment-1.3.0.tar", last modified: Sat Jul 22 19:45:37 2023, max compression
```

## Comparing `medimageaugment-1.2.9.tar` & `medimageaugment-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 19:37:48.907117 medimageaugment-1.2.9/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1077 2023-07-22 07:27:55.000000 medimageaugment-1.2.9/LICENSE
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15763 2023-07-22 19:37:48.906112 medimageaugment-1.2.9/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    14911 2023-07-22 07:27:59.000000 medimageaugment-1.2.9/README.md
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 19:37:48.904860 medimageaugment-1.2.9/medimageaugment.egg-info/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15763 2023-07-22 19:37:48.000000 medimageaugment-1.2.9/medimageaugment.egg-info/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      220 2023-07-22 19:37:48.000000 medimageaugment-1.2.9/medimageaugment.egg-info/SOURCES.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 19:37:48.000000 medimageaugment-1.2.9/medimageaugment.egg-info/dependency_links.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 19:37:48.000000 medimageaugment-1.2.9/medimageaugment.egg-info/requires.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 19:37:48.000000 medimageaugment-1.2.9/medimageaugment.egg-info/top_level.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 19:37:48.907581 medimageaugment-1.2.9/setup.cfg
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1106 2023-07-22 19:37:37.000000 medimageaugment-1.2.9/setup.py
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 19:45:37.799732 medimageaugment-1.3.0/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1077 2023-07-22 07:27:55.000000 medimageaugment-1.3.0/LICENSE
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15763 2023-07-22 19:45:37.797821 medimageaugment-1.3.0/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    14911 2023-07-22 07:27:59.000000 medimageaugment-1.3.0/README.md
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 19:45:37.795254 medimageaugment-1.3.0/medimageaugment.egg-info/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15763 2023-07-22 19:45:37.000000 medimageaugment-1.3.0/medimageaugment.egg-info/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      220 2023-07-22 19:45:37.000000 medimageaugment-1.3.0/medimageaugment.egg-info/SOURCES.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 19:45:37.000000 medimageaugment-1.3.0/medimageaugment.egg-info/dependency_links.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 19:45:37.000000 medimageaugment-1.3.0/medimageaugment.egg-info/requires.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 19:45:37.000000 medimageaugment-1.3.0/medimageaugment.egg-info/top_level.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 19:45:37.800369 medimageaugment-1.3.0/setup.cfg
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1106 2023-07-22 19:45:33.000000 medimageaugment-1.3.0/setup.py
```

### Comparing `medimageaugment-1.2.9/LICENSE` & `medimageaugment-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `medimageaugment-1.2.9/PKG-INFO` & `medimageaugment-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medimageaugment
-Version: 1.2.9
+Version: 1.3.0
 Summary: A Python class for image augmentation
 Home-page: https://github.com/himanalot/medimageaugment
 Author: Ishan Ramrakhiani
 Author-email: ishanramrakhiani@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
```

### Comparing `medimageaugment-1.2.9/README.md` & `medimageaugment-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `medimageaugment-1.2.9/medimageaugment.egg-info/PKG-INFO` & `medimageaugment-1.3.0/medimageaugment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medimageaugment
-Version: 1.2.9
+Version: 1.3.0
 Summary: A Python class for image augmentation
 Home-page: https://github.com/himanalot/medimageaugment
 Author: Ishan Ramrakhiani
 Author-email: ishanramrakhiani@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
```

### Comparing `medimageaugment-1.2.9/setup.py` & `medimageaugment-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medimageaugment',
-    version='1.2.9',
+    version='1.3.0',
     description='A Python class for image augmentation',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Ishan Ramrakhiani',
     author_email='ishanramrakhiani@gmail.com',
     url='https://github.com/himanalot/medimageaugment',
     packages=find_packages(),
```

