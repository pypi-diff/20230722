# Comparing `tmp/medimageaugment-1.0.0.tar.gz` & `tmp/medimageaugment-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medimageaugment-1.0.0.tar", last modified: Sat Jul 22 05:31:33 2023, max compression
+gzip compressed data, was "medimageaugment-1.0.1.tar", last modified: Sat Jul 22 05:34:51 2023, max compression
```

## Comparing `medimageaugment-1.0.0.tar` & `medimageaugment-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 05:31:33.727492 medimageaugment-1.0.0/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1077 2023-07-22 05:26:51.000000 medimageaugment-1.0.0/LICENSE
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      798 2023-07-22 05:31:33.726607 medimageaugment-1.0.0/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15124 2023-07-22 05:26:40.000000 medimageaugment-1.0.0/README.md
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 05:31:33.725653 medimageaugment-1.0.0/medimageaugment.egg-info/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      798 2023-07-22 05:31:33.000000 medimageaugment-1.0.0/medimageaugment.egg-info/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      220 2023-07-22 05:31:33.000000 medimageaugment-1.0.0/medimageaugment.egg-info/SOURCES.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 05:31:33.000000 medimageaugment-1.0.0/medimageaugment.egg-info/dependency_links.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 05:31:33.000000 medimageaugment-1.0.0/medimageaugment.egg-info/requires.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 05:31:33.000000 medimageaugment-1.0.0/medimageaugment.egg-info/top_level.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 05:31:33.728033 medimageaugment-1.0.0/setup.cfg
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      996 2023-07-22 05:27:18.000000 medimageaugment-1.0.0/setup.py
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 05:34:51.580158 medimageaugment-1.0.1/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1077 2023-07-22 05:26:51.000000 medimageaugment-1.0.1/LICENSE
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      798 2023-07-22 05:34:51.579577 medimageaugment-1.0.1/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)    15124 2023-07-22 05:26:40.000000 medimageaugment-1.0.1/README.md
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-22 05:34:51.578259 medimageaugment-1.0.1/medimageaugment.egg-info/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      798 2023-07-22 05:34:51.000000 medimageaugment-1.0.1/medimageaugment.egg-info/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      220 2023-07-22 05:34:51.000000 medimageaugment-1.0.1/medimageaugment.egg-info/SOURCES.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 05:34:51.000000 medimageaugment-1.0.1/medimageaugment.egg-info/dependency_links.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 05:34:51.000000 medimageaugment-1.0.1/medimageaugment.egg-info/requires.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-22 05:34:51.000000 medimageaugment-1.0.1/medimageaugment.egg-info/top_level.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-22 05:34:51.580543 medimageaugment-1.0.1/setup.cfg
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      996 2023-07-22 05:32:28.000000 medimageaugment-1.0.1/setup.py
```

### Comparing `medimageaugment-1.0.0/LICENSE` & `medimageaugment-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medimageaugment-1.0.0/PKG-INFO` & `medimageaugment-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medimageaugment
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python class for image augmentation
 Home-page: https://github.com/himanalot/medimageaugment
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
```

### Comparing `medimageaugment-1.0.0/README.md` & `medimageaugment-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `medimageaugment-1.0.0/medimageaugment.egg-info/PKG-INFO` & `medimageaugment-1.0.1/medimageaugment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medimageaugment
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python class for image augmentation
 Home-page: https://github.com/himanalot/medimageaugment
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
```

### Comparing `medimageaugment-1.0.0/setup.py` & `medimageaugment-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medimageaugment',
-    version='1.0.0',
+    version='1.0.1',
     description='A Python class for image augmentation',
     author='Your Name',
     author_email='your.email@example.com',
     url='https://github.com/himanalot/medimageaugment',
     packages=find_packages(),
     install_requires=[
         'numpy',
```

