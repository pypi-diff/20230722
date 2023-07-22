# Comparing `tmp/odooless-0.1.2.tar.gz` & `tmp/odooless-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odooless-0.1.2.tar", last modified: Sat Jul 22 16:49:36 2023, max compression
+gzip compressed data, was "odooless-0.1.3.tar", last modified: Sat Jul 22 16:59:50 2023, max compression
```

## Comparing `odooless-0.1.2.tar` & `odooless-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:49:36.611178 odooless-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-22 16:49:36.607178 odooless-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-22 16:49:26.000000 odooless-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:49:36.607178 odooless-0.1.2/odooless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-22 16:49:36.000000 odooless-0.1.2/odooless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-22 16:49:36.000000 odooless-0.1.2/odooless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:49:36.000000 odooless-0.1.2/odooless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 16:49:36.000000 odooless-0.1.2/odooless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:49:36.000000 odooless-0.1.2/odooless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 16:49:36.611178 odooless-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-22 16:49:26.000000 odooless-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:59:50.017040 odooless-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-22 16:59:50.017040 odooless-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-22 16:59:31.000000 odooless-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:59:50.017040 odooless-0.1.3/odooless/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:59:31.000000 odooless-0.1.3/odooless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-22 16:59:31.000000 odooless-0.1.3/odooless/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35379 2023-07-22 16:59:31.000000 odooless-0.1.3/odooless/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:59:50.017040 odooless-0.1.3/odooless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-22 16:59:49.000000 odooless-0.1.3/odooless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-22 16:59:49.000000 odooless-0.1.3/odooless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:59:49.000000 odooless-0.1.3/odooless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 16:59:49.000000 odooless-0.1.3/odooless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 16:59:49.000000 odooless-0.1.3/odooless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 16:59:50.017040 odooless-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-22 16:59:31.000000 odooless-0.1.3/setup.py
```

### Comparing `odooless-0.1.2/PKG-INFO` & `odooless-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odooless
-Version: 0.1.2
+Version: 0.1.3
 Summary: A DynamoDB ORM inspired by Odoo
 Home-page: https://github.com/Barameg/odooless.git
 Author: Sam Hasan
 Author-email: sam@barameg.co
 Keywords: odooless
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `odooless-0.1.2/README.md` & `odooless-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `odooless-0.1.2/odooless.egg-info/PKG-INFO` & `odooless-0.1.3/odooless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odooless
-Version: 0.1.2
+Version: 0.1.3
 Summary: A DynamoDB ORM inspired by Odoo
 Home-page: https://github.com/Barameg/odooless.git
 Author: Sam Hasan
 Author-email: sam@barameg.co
 Keywords: odooless
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `odooless-0.1.2/setup.py` & `odooless-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='odooless',
-    version='0.1.2',
+    version='0.1.3',
     description='A DynamoDB ORM inspired by Odoo',
     long_description='A DynamoDB ORM inspired by Odoo',
     author='Sam Hasan',
     author_email='sam@barameg.co',
     url='https://github.com/Barameg/odooless.git',
     packages=find_packages(),
     classifiers=[
```

