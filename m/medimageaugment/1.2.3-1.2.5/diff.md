# Comparing `tmp/medimageaugment-1.2.3.tar.gz` & `tmp/medimageaugment-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medimageaugment-1.2.3.tar", last modified: Sat Jul 22 07:28:15 2023, max compression
+gzip compressed data, was "medimageaugment-1.2.5.tar", last modified: Sat Jul 22 19:23:48 2023, max compression
```

## Comparing `medimageaugment-1.2.3.tar` & `medimageaugment-1.2.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 07:28:15.906401 medimageaugment-1.2.3/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1077 2023-07-22 07:27:55.000000 medimageaugment-1.2.3/LICENSE
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15763 2023-07-22 07:28:15.905561 medimageaugment-1.2.3/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    14911 2023-07-22 07:27:59.000000 medimageaugment-1.2.3/README.md
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 07:28:15.904434 medimageaugment-1.2.3/medimageaugment.egg-info/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15763 2023-07-22 07:28:15.000000 medimageaugment-1.2.3/medimageaugment.egg-info/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      220 2023-07-22 07:28:15.000000 medimageaugment-1.2.3/medimageaugment.egg-info/SOURCES.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 07:28:15.000000 medimageaugment-1.2.3/medimageaugment.egg-info/dependency_links.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 07:28:15.000000 medimageaugment-1.2.3/medimageaugment.egg-info/requires.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 07:28:15.000000 medimageaugment-1.2.3/medimageaugment.egg-info/top_level.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 07:28:15.906729 medimageaugment-1.2.3/setup.cfg
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1106 2023-07-22 07:28:10.000000 medimageaugment-1.2.3/setup.py
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 19:23:48.774292 medimageaugment-1.2.5/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1077 2023-07-22 07:27:55.000000 medimageaugment-1.2.5/LICENSE
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15763 2023-07-22 19:23:48.773007 medimageaugment-1.2.5/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    14911 2023-07-22 07:27:59.000000 medimageaugment-1.2.5/README.md
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 19:23:48.771206 medimageaugment-1.2.5/medimageaugment.egg-info/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15763 2023-07-22 19:23:48.000000 medimageaugment-1.2.5/medimageaugment.egg-info/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      220 2023-07-22 19:23:48.000000 medimageaugment-1.2.5/medimageaugment.egg-info/SOURCES.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 19:23:48.000000 medimageaugment-1.2.5/medimageaugment.egg-info/dependency_links.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 19:23:48.000000 medimageaugment-1.2.5/medimageaugment.egg-info/requires.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 19:23:48.000000 medimageaugment-1.2.5/medimageaugment.egg-info/top_level.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 19:23:48.775017 medimageaugment-1.2.5/setup.cfg
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1106 2023-07-22 19:23:31.000000 medimageaugment-1.2.5/setup.py
```

### Comparing `medimageaugment-1.2.3/LICENSE` & `medimageaugment-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `medimageaugment-1.2.3/PKG-INFO` & `medimageaugment-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medimageaugment
-Version: 1.2.3
+Version: 1.2.5
 Summary: A Python class for image augmentation
 Home-page: https://github.com/himanalot/medimageaugment
 Author: Ishan Ramrakhiani
 Author-email: ishanramrakhiani@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
```

### Comparing `medimageaugment-1.2.3/README.md` & `medimageaugment-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `medimageaugment-1.2.3/medimageaugment.egg-info/PKG-INFO` & `medimageaugment-1.2.5/medimageaugment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medimageaugment
-Version: 1.2.3
+Version: 1.2.5
 Summary: A Python class for image augmentation
 Home-page: https://github.com/himanalot/medimageaugment
 Author: Ishan Ramrakhiani
 Author-email: ishanramrakhiani@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
```

### Comparing `medimageaugment-1.2.3/setup.py` & `medimageaugment-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medimageaugment',
-    version='1.2.3',
+    version='1.2.5',
     description='A Python class for image augmentation',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Ishan Ramrakhiani',
     author_email='ishanramrakhiani@gmail.com',
     url='https://github.com/himanalot/medimageaugment',
     packages=find_packages(),
```

