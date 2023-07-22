# Comparing `tmp/medimageaugment-1.3.4.1.tar.gz` & `tmp/medimageaugment-1.3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medimageaugment-1.3.4.1.tar", last modified: Sat Jul 22 21:38:59 2023, max compression
+gzip compressed data, was "medimageaugment-1.3.4.2.tar", last modified: Sat Jul 22 21:40:37 2023, max compression
```

## Comparing `medimageaugment-1.3.4.1.tar` & `medimageaugment-1.3.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 21:38:59.877336 medimageaugment-1.3.4.1/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1077 2023-07-22 07:27:55.000000 medimageaugment-1.3.4.1/LICENSE
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15765 2023-07-22 21:38:59.876246 medimageaugment-1.3.4.1/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    14911 2023-07-22 07:27:59.000000 medimageaugment-1.3.4.1/README.md
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 21:38:59.875041 medimageaugment-1.3.4.1/medimageaugment.egg-info/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15765 2023-07-22 21:38:59.000000 medimageaugment-1.3.4.1/medimageaugment.egg-info/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      220 2023-07-22 21:38:59.000000 medimageaugment-1.3.4.1/medimageaugment.egg-info/SOURCES.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 21:38:59.000000 medimageaugment-1.3.4.1/medimageaugment.egg-info/dependency_links.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 21:38:59.000000 medimageaugment-1.3.4.1/medimageaugment.egg-info/requires.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 21:38:59.000000 medimageaugment-1.3.4.1/medimageaugment.egg-info/top_level.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 21:38:59.877645 medimageaugment-1.3.4.1/setup.cfg
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1108 2023-07-22 21:38:56.000000 medimageaugment-1.3.4.1/setup.py
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 21:40:37.749238 medimageaugment-1.3.4.2/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1077 2023-07-22 07:27:55.000000 medimageaugment-1.3.4.2/LICENSE
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15765 2023-07-22 21:40:37.748290 medimageaugment-1.3.4.2/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    14911 2023-07-22 07:27:59.000000 medimageaugment-1.3.4.2/README.md
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 21:40:37.747177 medimageaugment-1.3.4.2/medimageaugment.egg-info/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15765 2023-07-22 21:40:37.000000 medimageaugment-1.3.4.2/medimageaugment.egg-info/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      220 2023-07-22 21:40:37.000000 medimageaugment-1.3.4.2/medimageaugment.egg-info/SOURCES.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 21:40:37.000000 medimageaugment-1.3.4.2/medimageaugment.egg-info/dependency_links.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 21:40:37.000000 medimageaugment-1.3.4.2/medimageaugment.egg-info/requires.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 21:40:37.000000 medimageaugment-1.3.4.2/medimageaugment.egg-info/top_level.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 21:40:37.749523 medimageaugment-1.3.4.2/setup.cfg
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1108 2023-07-22 21:40:34.000000 medimageaugment-1.3.4.2/setup.py
```

### Comparing `medimageaugment-1.3.4.1/LICENSE` & `medimageaugment-1.3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medimageaugment-1.3.4.1/PKG-INFO` & `medimageaugment-1.3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medimageaugment
-Version: 1.3.4.1
+Version: 1.3.4.2
 Summary: A Python class for image augmentation
 Home-page: https://github.com/himanalot/medimageaugment
 Author: Ishan Ramrakhiani
 Author-email: ishanramrakhiani@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
```

### Comparing `medimageaugment-1.3.4.1/README.md` & `medimageaugment-1.3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `medimageaugment-1.3.4.1/medimageaugment.egg-info/PKG-INFO` & `medimageaugment-1.3.4.2/medimageaugment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medimageaugment
-Version: 1.3.4.1
+Version: 1.3.4.2
 Summary: A Python class for image augmentation
 Home-page: https://github.com/himanalot/medimageaugment
 Author: Ishan Ramrakhiani
 Author-email: ishanramrakhiani@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
```

### Comparing `medimageaugment-1.3.4.1/setup.py` & `medimageaugment-1.3.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medimageaugment',
-    version='1.3.4.1',
+    version='1.3.4.2',
     description='A Python class for image augmentation',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Ishan Ramrakhiani',
     author_email='ishanramrakhiani@gmail.com',
     url='https://github.com/himanalot/medimageaugment',
     packages=find_packages(),
```

