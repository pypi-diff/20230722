# Comparing `tmp/odooless-0.1.5.tar.gz` & `tmp/odooless-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odooless-0.1.5.tar", last modified: Sat Jul 22 17:12:36 2023, max compression
+gzip compressed data, was "odooless-0.1.6.tar", last modified: Sat Jul 22 17:32:02 2023, max compression
```

## Comparing `odooless-0.1.5.tar` & `odooless-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:12:36.545587 odooless-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-22 17:12:36.545587 odooless-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-22 17:12:25.000000 odooless-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:12:36.545587 odooless-0.1.5/odooless/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 17:12:25.000000 odooless-0.1.5/odooless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-22 17:12:25.000000 odooless-0.1.5/odooless/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)    35379 2023-07-22 17:12:25.000000 odooless-0.1.5/odooless/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:12:36.545587 odooless-0.1.5/odooless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-22 17:12:36.000000 odooless-0.1.5/odooless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-22 17:12:36.000000 odooless-0.1.5/odooless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 17:12:36.000000 odooless-0.1.5/odooless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 17:12:36.000000 odooless-0.1.5/odooless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 17:12:36.000000 odooless-0.1.5/odooless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 17:12:36.545587 odooless-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-22 17:12:25.000000 odooless-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:32:02.446915 odooless-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-22 17:32:02.446915 odooless-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-22 17:31:49.000000 odooless-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:32:02.446915 odooless-0.1.6/odooless/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 17:31:49.000000 odooless-0.1.6/odooless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-22 17:31:49.000000 odooless-0.1.6/odooless/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35379 2023-07-22 17:31:49.000000 odooless-0.1.6/odooless/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:32:02.446915 odooless-0.1.6/odooless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-22 17:32:02.000000 odooless-0.1.6/odooless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-22 17:32:02.000000 odooless-0.1.6/odooless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 17:32:02.000000 odooless-0.1.6/odooless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 17:32:02.000000 odooless-0.1.6/odooless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 17:32:02.000000 odooless-0.1.6/odooless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 17:32:02.446915 odooless-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-22 17:31:49.000000 odooless-0.1.6/setup.py
```

### Comparing `odooless-0.1.5/PKG-INFO` & `odooless-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odooless
-Version: 0.1.5
+Version: 0.1.6
 Summary: A DynamoDB ORM inspired by Odoo
 Home-page: https://github.com/Barameg/odooless.git
 Author: Sam Hasan
 Author-email: sam@barameg.co
 Keywords: odooless
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `odooless-0.1.5/odooless/models.py` & `odooless-0.1.6/odooless/models.py`

 * *Files identical despite different names*

### Comparing `odooless-0.1.5/odooless.egg-info/PKG-INFO` & `odooless-0.1.6/odooless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odooless
-Version: 0.1.5
+Version: 0.1.6
 Summary: A DynamoDB ORM inspired by Odoo
 Home-page: https://github.com/Barameg/odooless.git
 Author: Sam Hasan
 Author-email: sam@barameg.co
 Keywords: odooless
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `odooless-0.1.5/setup.py` & `odooless-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='odooless',
-    version='0.1.5',
+    version='0.1.6',
     description='A DynamoDB ORM inspired by Odoo',
     long_description='A DynamoDB ORM inspired by Odoo',
     author='Sam Hasan',
     author_email='sam@barameg.co',
     url='https://github.com/Barameg/odooless.git',
     packages=find_packages(),
     classifiers=[
```

