# Comparing `tmp/ElisionPy-0.0.5.tar.gz` & `tmp/ElisionPy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ElisionPy-0.0.5.tar", last modified: Sat Jul 22 20:11:32 2023, max compression
+gzip compressed data, was "ElisionPy-0.0.6.tar", last modified: Sat Jul 22 20:17:27 2023, max compression
```

## Comparing `ElisionPy-0.0.5.tar` & `ElisionPy-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 20:11:32.942064 ElisionPy-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-07-22 20:11:32.939063 ElisionPy-0.0.5/ElisionPy.egg-info/
--rw-rw-rw-   0        0        0      552 2023-07-22 20:11:32.000000 ElisionPy-0.0.5/ElisionPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-07-22 20:11:32.000000 ElisionPy-0.0.5/ElisionPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 20:11:32.000000 ElisionPy-0.0.5/ElisionPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-22 20:11:32.000000 ElisionPy-0.0.5/ElisionPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-22 20:11:32.000000 ElisionPy-0.0.5/ElisionPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      552 2023-07-22 20:11:32.942064 ElisionPy-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-07-22 19:00:10.000000 ElisionPy-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 20:11:32.941064 ElisionPy-0.0.5/elision/
--rw-rw-rw-   0        0        0        0 2023-07-22 19:43:20.000000 ElisionPy-0.0.5/elision/__init__.py
--rw-rw-rw-   0        0        0      736 2023-07-22 19:35:24.000000 ElisionPy-0.0.5/elision/help.py
--rw-rw-rw-   0        0        0     2117 2023-07-22 18:28:16.000000 ElisionPy-0.0.5/elision/random.py
--rw-rw-rw-   0        0        0       42 2023-07-22 20:11:32.942064 ElisionPy-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      805 2023-07-22 20:10:53.000000 ElisionPy-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 20:17:27.448048 ElisionPy-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-07-22 20:17:27.445047 ElisionPy-0.0.6/ElisionPy.egg-info/
+-rw-rw-rw-   0        0        0      552 2023-07-22 20:17:27.000000 ElisionPy-0.0.6/ElisionPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-07-22 20:17:27.000000 ElisionPy-0.0.6/ElisionPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 20:17:27.000000 ElisionPy-0.0.6/ElisionPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-22 20:17:27.000000 ElisionPy-0.0.6/ElisionPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-22 20:17:27.000000 ElisionPy-0.0.6/ElisionPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      552 2023-07-22 20:17:27.448048 ElisionPy-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-07-22 19:00:10.000000 ElisionPy-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 20:17:27.448048 ElisionPy-0.0.6/elision/
+-rw-rw-rw-   0        0        0        0 2023-07-22 19:43:20.000000 ElisionPy-0.0.6/elision/__init__.py
+-rw-rw-rw-   0        0        0    94642 2023-04-04 21:04:10.000000 ElisionPy-0.0.6/elision/datetime.py
+-rw-rw-rw-   0        0        0      736 2023-07-22 19:35:24.000000 ElisionPy-0.0.6/elision/help.py
+-rw-rw-rw-   0        0        0     2117 2023-07-22 18:28:16.000000 ElisionPy-0.0.6/elision/random.py
+-rw-rw-rw-   0        0        0       42 2023-07-22 20:17:27.449048 ElisionPy-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      805 2023-07-22 20:16:34.000000 ElisionPy-0.0.6/setup.py
```

### Comparing `ElisionPy-0.0.5/ElisionPy.egg-info/PKG-INFO` & `ElisionPy-0.0.6/ElisionPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ElisionPy
-Version: 0.0.5
+Version: 0.0.6
 Summary: This module is under development!
 Home-page: https://github.com/Ginji-Fox/ElisionPy
 Author: Ginji
 Author-email: bfire1999@gmail.com
 Project-URL: Documentation, https://github.com/Ginji-Fox/ElisionPy
 Keywords: ElisionPy Elision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `ElisionPy-0.0.5/PKG-INFO` & `ElisionPy-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ElisionPy
-Version: 0.0.5
+Version: 0.0.6
 Summary: This module is under development!
 Home-page: https://github.com/Ginji-Fox/ElisionPy
 Author: Ginji
 Author-email: bfire1999@gmail.com
 Project-URL: Documentation, https://github.com/Ginji-Fox/ElisionPy
 Keywords: ElisionPy Elision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `ElisionPy-0.0.5/elision/help.py` & `ElisionPy-0.0.6/elision/help.py`

 * *Files identical despite different names*

### Comparing `ElisionPy-0.0.5/elision/random.py` & `ElisionPy-0.0.6/elision/random.py`

 * *Files identical despite different names*

### Comparing `ElisionPy-0.0.5/setup.py` & `ElisionPy-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='ElisionPy',
-  version='0.0.5',
+  version='0.0.6',
   author='Ginji',
   author_email='bfire1999@gmail.com',
   description='This module is under development!',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Ginji-Fox/ElisionPy',
   packages=find_packages(),
```

