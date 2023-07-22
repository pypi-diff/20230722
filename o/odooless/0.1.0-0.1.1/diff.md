# Comparing `tmp/odooless-0.1.0.tar.gz` & `tmp/odooless-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odooless-0.1.0.tar", last modified: Sat Jul 22 16:31:46 2023, max compression
+gzip compressed data, was "odooless-0.1.1.tar", last modified: Sat Jul 22 16:42:08 2023, max compression
```

## Comparing `odooless-0.1.0.tar` & `odooless-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:31:46.085465 odooless-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-22 16:31:46.085465 odooless-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-22 16:31:35.000000 odooless-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:31:46.085465 odooless-0.1.0/odooless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-22 16:31:46.000000 odooless-0.1.0/odooless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-22 16:31:46.000000 odooless-0.1.0/odooless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:31:46.000000 odooless-0.1.0/odooless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 16:31:46.000000 odooless-0.1.0/odooless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:31:46.000000 odooless-0.1.0/odooless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 16:31:46.085465 odooless-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-22 16:31:35.000000 odooless-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:42:08.303784 odooless-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-22 16:42:08.303784 odooless-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-22 16:41:57.000000 odooless-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:42:08.303784 odooless-0.1.1/odooless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-22 16:42:08.000000 odooless-0.1.1/odooless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-22 16:42:08.000000 odooless-0.1.1/odooless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:42:08.000000 odooless-0.1.1/odooless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 16:42:08.000000 odooless-0.1.1/odooless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:42:08.000000 odooless-0.1.1/odooless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 16:42:08.303784 odooless-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-22 16:41:57.000000 odooless-0.1.1/setup.py
```

### Comparing `odooless-0.1.0/PKG-INFO` & `odooless-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odooless
-Version: 0.1.0
+Version: 0.1.1
 Summary: A DynamoDB ORM inspired by Odoo
 Home-page: https://github.com/Barameg/odooless
 Author: Sam Hasan
 Author-email: sam@barameg.co
 Keywords: odooless
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `odooless-0.1.0/README.md` & `odooless-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `odooless-0.1.0/odooless.egg-info/PKG-INFO` & `odooless-0.1.1/odooless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odooless
-Version: 0.1.0
+Version: 0.1.1
 Summary: A DynamoDB ORM inspired by Odoo
 Home-page: https://github.com/Barameg/odooless
 Author: Sam Hasan
 Author-email: sam@barameg.co
 Keywords: odooless
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `odooless-0.1.0/setup.py` & `odooless-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='odooless',
-    version='0.1.0',
+    version='0.1.1',
     description='A DynamoDB ORM inspired by Odoo',
     long_description='A DynamoDB ORM inspired by Odoo',
     author='Sam Hasan',
     author_email='sam@barameg.co',
     url='https://github.com/Barameg/odooless',
     packages=find_packages(),
     classifiers=[
```

