# Comparing `tmp/ElisionPy-0.0.4.tar.gz` & `tmp/ElisionPy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ElisionPy-0.0.4.tar", last modified: Sat Jul 22 20:08:09 2023, max compression
+gzip compressed data, was "ElisionPy-0.0.5.tar", last modified: Sat Jul 22 20:11:32 2023, max compression
```

## Comparing `ElisionPy-0.0.4.tar` & `ElisionPy-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 20:08:09.969162 ElisionPy-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-07-22 20:08:09.967162 ElisionPy-0.0.4/ElisionPy.egg-info/
--rw-rw-rw-   0        0        0      552 2023-07-22 20:08:09.000000 ElisionPy-0.0.4/ElisionPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-07-22 20:08:09.000000 ElisionPy-0.0.4/ElisionPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 20:08:09.000000 ElisionPy-0.0.4/ElisionPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-22 20:08:09.000000 ElisionPy-0.0.4/ElisionPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-22 20:08:09.000000 ElisionPy-0.0.4/ElisionPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      552 2023-07-22 20:08:09.969162 ElisionPy-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-07-22 19:00:10.000000 ElisionPy-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 20:08:09.969162 ElisionPy-0.0.4/elision/
--rw-rw-rw-   0        0        0        0 2023-07-22 19:43:20.000000 ElisionPy-0.0.4/elision/__init__.py
--rw-rw-rw-   0        0        0      736 2023-07-22 19:35:24.000000 ElisionPy-0.0.4/elision/help.py
--rw-rw-rw-   0        0        0     2117 2023-07-22 18:28:16.000000 ElisionPy-0.0.4/elision/random.py
--rw-rw-rw-   0        0        0       42 2023-07-22 20:08:09.970163 ElisionPy-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      807 2023-07-22 20:07:27.000000 ElisionPy-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 20:11:32.942064 ElisionPy-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-07-22 20:11:32.939063 ElisionPy-0.0.5/ElisionPy.egg-info/
+-rw-rw-rw-   0        0        0      552 2023-07-22 20:11:32.000000 ElisionPy-0.0.5/ElisionPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-07-22 20:11:32.000000 ElisionPy-0.0.5/ElisionPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 20:11:32.000000 ElisionPy-0.0.5/ElisionPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-22 20:11:32.000000 ElisionPy-0.0.5/ElisionPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-22 20:11:32.000000 ElisionPy-0.0.5/ElisionPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      552 2023-07-22 20:11:32.942064 ElisionPy-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-07-22 19:00:10.000000 ElisionPy-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 20:11:32.941064 ElisionPy-0.0.5/elision/
+-rw-rw-rw-   0        0        0        0 2023-07-22 19:43:20.000000 ElisionPy-0.0.5/elision/__init__.py
+-rw-rw-rw-   0        0        0      736 2023-07-22 19:35:24.000000 ElisionPy-0.0.5/elision/help.py
+-rw-rw-rw-   0        0        0     2117 2023-07-22 18:28:16.000000 ElisionPy-0.0.5/elision/random.py
+-rw-rw-rw-   0        0        0       42 2023-07-22 20:11:32.942064 ElisionPy-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      805 2023-07-22 20:10:53.000000 ElisionPy-0.0.5/setup.py
```

### Comparing `ElisionPy-0.0.4/ElisionPy.egg-info/PKG-INFO` & `ElisionPy-0.0.5/ElisionPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ElisionPy
-Version: 0.0.4
+Version: 0.0.5
 Summary: This module is under development!
 Home-page: https://github.com/Ginji-Fox/ElisionPy
 Author: Ginji
 Author-email: bfire1999@gmail.com
 Project-URL: Documentation, https://github.com/Ginji-Fox/ElisionPy
 Keywords: ElisionPy Elision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `ElisionPy-0.0.4/PKG-INFO` & `ElisionPy-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ElisionPy
-Version: 0.0.4
+Version: 0.0.5
 Summary: This module is under development!
 Home-page: https://github.com/Ginji-Fox/ElisionPy
 Author: Ginji
 Author-email: bfire1999@gmail.com
 Project-URL: Documentation, https://github.com/Ginji-Fox/ElisionPy
 Keywords: ElisionPy Elision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `ElisionPy-0.0.4/elision/help.py` & `ElisionPy-0.0.5/elision/help.py`

 * *Files identical despite different names*

### Comparing `ElisionPy-0.0.4/elision/random.py` & `ElisionPy-0.0.5/elision/random.py`

 * *Files identical despite different names*

### Comparing `ElisionPy-0.0.4/setup.py` & `ElisionPy-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='ElisionPy',
-  version='0.0.4',
+  version='0.0.5',
   author='Ginji',
   author_email='bfire1999@gmail.com',
   description='This module is under development!',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Ginji-Fox/ElisionPy',
   packages=find_packages(),
-  install_requires=['requests>=2.25.1', 'datetime>=8.1.7'],
+  install_requires=['requests>=2.25.1', 'datetime>=5.2'],
   classifiers=[
     'Programming Language :: Python :: 3.11',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent'
   ],
   keywords='ElisionPy Elision',
   project_urls={
```

