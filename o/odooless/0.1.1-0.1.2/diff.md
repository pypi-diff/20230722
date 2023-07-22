# Comparing `tmp/odooless-0.1.1.tar.gz` & `tmp/odooless-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odooless-0.1.1.tar", last modified: Sat Jul 22 16:42:08 2023, max compression
+gzip compressed data, was "odooless-0.1.2.tar", last modified: Sat Jul 22 16:49:36 2023, max compression
```

## Comparing `odooless-0.1.1.tar` & `odooless-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:42:08.303784 odooless-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-22 16:42:08.303784 odooless-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-22 16:41:57.000000 odooless-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:42:08.303784 odooless-0.1.1/odooless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-22 16:42:08.000000 odooless-0.1.1/odooless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-22 16:42:08.000000 odooless-0.1.1/odooless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:42:08.000000 odooless-0.1.1/odooless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 16:42:08.000000 odooless-0.1.1/odooless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:42:08.000000 odooless-0.1.1/odooless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 16:42:08.303784 odooless-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-22 16:41:57.000000 odooless-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:49:36.611178 odooless-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-22 16:49:36.607178 odooless-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-22 16:49:26.000000 odooless-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:49:36.607178 odooless-0.1.2/odooless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-22 16:49:36.000000 odooless-0.1.2/odooless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-22 16:49:36.000000 odooless-0.1.2/odooless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:49:36.000000 odooless-0.1.2/odooless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 16:49:36.000000 odooless-0.1.2/odooless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:49:36.000000 odooless-0.1.2/odooless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 16:49:36.611178 odooless-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-22 16:49:26.000000 odooless-0.1.2/setup.py
```

### Comparing `odooless-0.1.1/PKG-INFO` & `odooless-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: odooless
-Version: 0.1.1
+Version: 0.1.2
 Summary: A DynamoDB ORM inspired by Odoo
-Home-page: https://github.com/Barameg/odooless
+Home-page: https://github.com/Barameg/odooless.git
 Author: Sam Hasan
 Author-email: sam@barameg.co
 Keywords: odooless
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `odooless-0.1.1/README.md` & `odooless-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `odooless-0.1.1/odooless.egg-info/PKG-INFO` & `odooless-0.1.2/odooless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: odooless
-Version: 0.1.1
+Version: 0.1.2
 Summary: A DynamoDB ORM inspired by Odoo
-Home-page: https://github.com/Barameg/odooless
+Home-page: https://github.com/Barameg/odooless.git
 Author: Sam Hasan
 Author-email: sam@barameg.co
 Keywords: odooless
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `odooless-0.1.1/setup.py` & `odooless-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='odooless',
-    version='0.1.1',
+    version='0.1.2',
     description='A DynamoDB ORM inspired by Odoo',
     long_description='A DynamoDB ORM inspired by Odoo',
     author='Sam Hasan',
     author_email='sam@barameg.co',
-    url='https://github.com/Barameg/odooless',
+    url='https://github.com/Barameg/odooless.git',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

