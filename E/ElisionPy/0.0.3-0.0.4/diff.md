# Comparing `tmp/ElisionPy-0.0.3.tar.gz` & `tmp/ElisionPy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ElisionPy-0.0.3.tar", last modified: Sat Jul 22 19:43:51 2023, max compression
+gzip compressed data, was "ElisionPy-0.0.4.tar", last modified: Sat Jul 22 20:08:09 2023, max compression
```

## Comparing `ElisionPy-0.0.3.tar` & `ElisionPy-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 19:43:51.469944 ElisionPy-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-07-22 19:43:51.467944 ElisionPy-0.0.3/ElisionPy.egg-info/
--rw-rw-rw-   0        0        0      552 2023-07-22 19:43:51.000000 ElisionPy-0.0.3/ElisionPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-07-22 19:43:51.000000 ElisionPy-0.0.3/ElisionPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 19:43:51.000000 ElisionPy-0.0.3/ElisionPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-22 19:43:51.000000 ElisionPy-0.0.3/ElisionPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-22 19:43:51.000000 ElisionPy-0.0.3/ElisionPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      552 2023-07-22 19:43:51.469944 ElisionPy-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-07-22 19:00:10.000000 ElisionPy-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 19:43:51.468944 ElisionPy-0.0.3/elision/
--rw-rw-rw-   0        0        0        0 2023-07-22 19:43:20.000000 ElisionPy-0.0.3/elision/__init__.py
--rw-rw-rw-   0        0        0      736 2023-07-22 19:35:24.000000 ElisionPy-0.0.3/elision/help.py
--rw-rw-rw-   0        0        0     2117 2023-07-22 18:28:16.000000 ElisionPy-0.0.3/elision/random.py
--rw-rw-rw-   0        0        0       42 2023-07-22 19:43:51.470946 ElisionPy-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      788 2023-07-22 19:43:46.000000 ElisionPy-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 20:08:09.969162 ElisionPy-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-07-22 20:08:09.967162 ElisionPy-0.0.4/ElisionPy.egg-info/
+-rw-rw-rw-   0        0        0      552 2023-07-22 20:08:09.000000 ElisionPy-0.0.4/ElisionPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-07-22 20:08:09.000000 ElisionPy-0.0.4/ElisionPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 20:08:09.000000 ElisionPy-0.0.4/ElisionPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-22 20:08:09.000000 ElisionPy-0.0.4/ElisionPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-22 20:08:09.000000 ElisionPy-0.0.4/ElisionPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      552 2023-07-22 20:08:09.969162 ElisionPy-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-07-22 19:00:10.000000 ElisionPy-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 20:08:09.969162 ElisionPy-0.0.4/elision/
+-rw-rw-rw-   0        0        0        0 2023-07-22 19:43:20.000000 ElisionPy-0.0.4/elision/__init__.py
+-rw-rw-rw-   0        0        0      736 2023-07-22 19:35:24.000000 ElisionPy-0.0.4/elision/help.py
+-rw-rw-rw-   0        0        0     2117 2023-07-22 18:28:16.000000 ElisionPy-0.0.4/elision/random.py
+-rw-rw-rw-   0        0        0       42 2023-07-22 20:08:09.970163 ElisionPy-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      807 2023-07-22 20:07:27.000000 ElisionPy-0.0.4/setup.py
```

### Comparing `ElisionPy-0.0.3/elision/help.py` & `ElisionPy-0.0.4/elision/help.py`

 * *Files identical despite different names*

### Comparing `ElisionPy-0.0.3/elision/random.py` & `ElisionPy-0.0.4/elision/random.py`

 * *Files identical despite different names*

### Comparing `ElisionPy-0.0.3/setup.py` & `ElisionPy-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='ElisionPy',
-  version='0.0.3',
+  version='0.0.4',
   author='Ginji',
   author_email='bfire1999@gmail.com',
   description='This module is under development!',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Ginji-Fox/ElisionPy',
   packages=find_packages(),
-  install_requires=['requests>=2.25.1'],
+  install_requires=['requests>=2.25.1', 'datetime>=8.1.7'],
   classifiers=[
     'Programming Language :: Python :: 3.11',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent'
   ],
   keywords='ElisionPy Elision',
   project_urls={
```

