# Comparing `tmp/sopel_modules.stocks-1.2.1.tar.gz` & `tmp/sopel_modules.stocks-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel_modules.stocks-1.2.1.tar", last modified: Sat Nov 12 18:40:48 2022, max compression
+gzip compressed data, was "sopel_modules.stocks-1.2.2.tar", last modified: Sat Jul 22 01:33:56 2023, max compression
```

## Comparing `sopel_modules.stocks-1.2.1.tar` & `sopel_modules.stocks-1.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 18:40:48.465999 sopel_modules.stocks-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-11-12 18:40:39.000000 sopel_modules.stocks-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-11-12 18:40:39.000000 sopel_modules.stocks-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 18:40:39.000000 sopel_modules.stocks-1.2.1/NEWS
--rw-r--r--   0 runner    (1001) docker     (121)     2271 2022-11-12 18:40:48.465999 sopel_modules.stocks-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-11-12 18:40:39.000000 sopel_modules.stocks-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-12 18:40:39.000000 sopel_modules.stocks-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-12 18:40:48.465999 sopel_modules.stocks-1.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1413 2022-11-12 18:40:39.000000 sopel_modules.stocks-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 18:40:48.461999 sopel_modules.stocks-1.2.1/sopel_modules/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-12 18:40:39.000000 sopel_modules.stocks-1.2.1/sopel_modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 18:40:48.461999 sopel_modules.stocks-1.2.1/sopel_modules/stocks/
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-11-12 18:40:39.000000 sopel_modules.stocks-1.2.1/sopel_modules/stocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 18:40:48.465999 sopel_modules.stocks-1.2.1/sopel_modules/stocks/providers/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 18:40:39.000000 sopel_modules.stocks-1.2.1/sopel_modules/stocks/providers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1687 2022-11-12 18:40:39.000000 sopel_modules.stocks-1.2.1/sopel_modules/stocks/providers/alphavantage.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      514 2022-11-12 18:40:39.000000 sopel_modules.stocks-1.2.1/sopel_modules/stocks/providers/iexcloud.py
--rw-r--r--   0 runner    (1001) docker     (121)     3433 2022-11-12 18:40:39.000000 sopel_modules.stocks-1.2.1/sopel_modules/stocks/stocks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 18:40:48.461999 sopel_modules.stocks-1.2.1/sopel_modules.stocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2271 2022-11-12 18:40:48.000000 sopel_modules.stocks-1.2.1/sopel_modules.stocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-11-12 18:40:48.000000 sopel_modules.stocks-1.2.1/sopel_modules.stocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-12 18:40:48.000000 sopel_modules.stocks-1.2.1/sopel_modules.stocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-12 18:40:48.000000 sopel_modules.stocks-1.2.1/sopel_modules.stocks.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-12 18:40:48.000000 sopel_modules.stocks-1.2.1/sopel_modules.stocks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-12 18:40:48.000000 sopel_modules.stocks-1.2.1/sopel_modules.stocks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 18:40:48.465999 sopel_modules.stocks-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-12 18:40:39.000000 sopel_modules.stocks-1.2.1/tests/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:33:56.377245 sopel_modules.stocks-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/NEWS
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-22 01:33:56.377245 sopel_modules.stocks-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 01:33:56.377245 sopel_modules.stocks-1.2.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1413 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:33:56.377245 sopel_modules.stocks-1.2.2/sopel_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/sopel_modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:33:56.377245 sopel_modules.stocks-1.2.2/sopel_modules/stocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/sopel_modules/stocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:33:56.377245 sopel_modules.stocks-1.2.2/sopel_modules/stocks/providers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/sopel_modules/stocks/providers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1781 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/sopel_modules/stocks/providers/alphavantage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/sopel_modules/stocks/providers/iexcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/sopel_modules/stocks/stocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:33:56.377245 sopel_modules.stocks-1.2.2/sopel_modules.stocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-22 01:33:56.000000 sopel_modules.stocks-1.2.2/sopel_modules.stocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-22 01:33:56.000000 sopel_modules.stocks-1.2.2/sopel_modules.stocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 01:33:56.000000 sopel_modules.stocks-1.2.2/sopel_modules.stocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-22 01:33:56.000000 sopel_modules.stocks-1.2.2/sopel_modules.stocks.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 01:33:56.000000 sopel_modules.stocks-1.2.2/sopel_modules.stocks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-22 01:33:56.000000 sopel_modules.stocks-1.2.2/sopel_modules.stocks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:33:56.377245 sopel_modules.stocks-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/tests/requirements.txt
```

### Comparing `sopel_modules.stocks-1.2.1/LICENSE` & `sopel_modules.stocks-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sopel_modules.stocks-1.2.1/PKG-INFO` & `sopel_modules.stocks-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel_modules.stocks
-Version: 1.2.1
+Version: 1.2.2
 Summary: Sopel Stocks Plugin
 Home-page: http://github.com/rustybower/sopel-stocks
 Author: Rusty Bower
 Author-email: rusty@rustybower.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sopel_modules.stocks-1.2.1/README.md` & `sopel_modules.stocks-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sopel_modules.stocks-1.2.1/setup.py` & `sopel_modules.stocks-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 with open('tests/requirements.txt') as dev_requirements_file:
     dev_requirements = [req for req in dev_requirements_file.readlines()]
 
 
 setup(
     name='sopel_modules.stocks',
-    version='1.2.1',
+    version='1.2.2',
     description='Sopel Stocks Plugin',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',  # This is important!
     author='Rusty Bower',
     author_email='rusty@rustybower.com',
     url='http://github.com/rustybower/sopel-stocks',
     packages=find_packages('.'),
```

### Comparing `sopel_modules.stocks-1.2.1/sopel_modules/stocks/providers/iexcloud.py` & `sopel_modules.stocks-1.2.2/sopel_modules/stocks/providers/iexcloud.py`

 * *Files identical despite different names*

### Comparing `sopel_modules.stocks-1.2.1/sopel_modules/stocks/stocks.py` & `sopel_modules.stocks-1.2.2/sopel_modules/stocks/stocks.py`

 * *Files identical despite different names*

### Comparing `sopel_modules.stocks-1.2.1/sopel_modules.stocks.egg-info/PKG-INFO` & `sopel_modules.stocks-1.2.2/sopel_modules.stocks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel-modules.stocks
-Version: 1.2.1
+Version: 1.2.2
 Summary: Sopel Stocks Plugin
 Home-page: http://github.com/rustybower/sopel-stocks
 Author: Rusty Bower
 Author-email: rusty@rustybower.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sopel_modules.stocks-1.2.1/sopel_modules.stocks.egg-info/SOURCES.txt` & `sopel_modules.stocks-1.2.2/sopel_modules.stocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

