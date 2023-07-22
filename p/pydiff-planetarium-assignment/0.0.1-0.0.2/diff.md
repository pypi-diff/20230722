# Comparing `tmp/pydiff-planetarium-assignment-0.0.1.tar.gz` & `tmp/pydiff-planetarium-assignment-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiff-planetarium-assignment-0.0.1.tar", last modified: Sat Jul 22 14:48:06 2023, max compression
+gzip compressed data, was "pydiff-planetarium-assignment-0.0.2.tar", last modified: Sat Jul 22 14:59:27 2023, max compression
```

## Comparing `pydiff-planetarium-assignment-0.0.1.tar` & `pydiff-planetarium-assignment-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 14:48:06.557519 pydiff-planetarium-assignment-0.0.1/
--rw-r--r--   0 channprj   (501) staff       (20)     1784 2023-07-22 14:48:06.557421 pydiff-planetarium-assignment-0.0.1/PKG-INFO
--rw-r--r--   0 channprj   (501) staff       (20)     1354 2023-07-22 14:47:22.000000 pydiff-planetarium-assignment-0.0.1/README.md
-drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 14:48:06.557277 pydiff-planetarium-assignment-0.0.1/pydiff_planetarium_assignment.egg-info/
--rw-r--r--   0 channprj   (501) staff       (20)     1784 2023-07-22 14:48:06.000000 pydiff-planetarium-assignment-0.0.1/pydiff_planetarium_assignment.egg-info/PKG-INFO
--rw-r--r--   0 channprj   (501) staff       (20)      245 2023-07-22 14:48:06.000000 pydiff-planetarium-assignment-0.0.1/pydiff_planetarium_assignment.egg-info/SOURCES.txt
--rw-r--r--   0 channprj   (501) staff       (20)        1 2023-07-22 14:48:06.000000 pydiff-planetarium-assignment-0.0.1/pydiff_planetarium_assignment.egg-info/dependency_links.txt
--rw-r--r--   0 channprj   (501) staff       (20)        1 2023-07-22 14:48:06.000000 pydiff-planetarium-assignment-0.0.1/pydiff_planetarium_assignment.egg-info/top_level.txt
--rw-r--r--   0 channprj   (501) staff       (20)      104 2023-07-22 14:45:33.000000 pydiff-planetarium-assignment-0.0.1/pyproject.toml
--rw-r--r--   0 channprj   (501) staff       (20)       38 2023-07-22 14:48:06.557548 pydiff-planetarium-assignment-0.0.1/setup.cfg
--rw-r--r--   0 channprj   (501) staff       (20)      760 2023-07-22 14:48:02.000000 pydiff-planetarium-assignment-0.0.1/setup.py
+drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 14:59:27.578586 pydiff-planetarium-assignment-0.0.2/
+-rw-r--r--   0 channprj   (501) staff       (20)     1866 2023-07-22 14:59:27.578480 pydiff-planetarium-assignment-0.0.2/PKG-INFO
+-rw-r--r--   0 channprj   (501) staff       (20)     1435 2023-07-22 14:57:37.000000 pydiff-planetarium-assignment-0.0.2/README.md
+drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 14:59:27.577467 pydiff-planetarium-assignment-0.0.2/pydiff_planetarium_assignment/
+drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 14:59:27.578317 pydiff-planetarium-assignment-0.0.2/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/
+-rw-r--r--   0 channprj   (501) staff       (20)     1866 2023-07-22 14:59:27.000000 pydiff-planetarium-assignment-0.0.2/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/PKG-INFO
+-rw-r--r--   0 channprj   (501) staff       (20)      365 2023-07-22 14:59:27.000000 pydiff-planetarium-assignment-0.0.2/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/SOURCES.txt
+-rw-r--r--   0 channprj   (501) staff       (20)        1 2023-07-22 14:59:27.000000 pydiff-planetarium-assignment-0.0.2/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/dependency_links.txt
+-rw-r--r--   0 channprj   (501) staff       (20)        1 2023-07-22 14:59:27.000000 pydiff-planetarium-assignment-0.0.2/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/top_level.txt
+-rw-r--r--   0 channprj   (501) staff       (20)      104 2023-07-22 14:45:33.000000 pydiff-planetarium-assignment-0.0.2/pyproject.toml
+-rw-r--r--   0 channprj   (501) staff       (20)       38 2023-07-22 14:59:27.578618 pydiff-planetarium-assignment-0.0.2/setup.cfg
+-rw-r--r--   0 channprj   (501) staff       (20)      789 2023-07-22 14:59:23.000000 pydiff-planetarium-assignment-0.0.2/setup.py
```

### Comparing `pydiff-planetarium-assignment-0.0.1/PKG-INFO` & `pydiff-planetarium-assignment-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pydiff-planetarium-assignment
-Version: 0.0.1
-Summary: Simple implementation of unixdiff
+Version: 0.0.2
+Summary: Simple implementation of unix diff
 Home-page: https://github.com/planetarium/take-home-2023-channprj
 Author: channprj
 Author-email: chann@chann.dev
 Project-URL: Bug Tracker, https://github.com/planetarium/take-home-2023-channprj/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -20,29 +20,36 @@
 - [x] Split and refine codes
 - [x] Wrap as a python packages using `pyproject.toml`
 - [ ] Write pure implementation of diff
 - [x] Add more documentation
 
 ## TLDR;
 
+Install package and import this.
+
 ```sh
-pip install pydiff
+pip install pydiff-planetarium-assignment
+```
+
+```py
+import pydiff
+
 ```
 
 ## Prerequisites
 
 - Python 3 (>= 3.11)
 
 ## How to use
 
 Install Python according to your preferences. Recommend to use direnv and pyenv.
 
 And then, install dependencies like below.
 
-```sh
+```
 pip install -r requirements.txt
 ```
 
 ### Reference Application
 
 If you're prepared, you can use it like below.
```

### Comparing `pydiff-planetarium-assignment-0.0.1/README.md` & `pydiff-planetarium-assignment-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,29 +8,36 @@
 - [x] Split and refine codes
 - [x] Wrap as a python packages using `pyproject.toml`
 - [ ] Write pure implementation of diff
 - [x] Add more documentation
 
 ## TLDR;
 
+Install package and import this.
+
 ```sh
-pip install pydiff
+pip install pydiff-planetarium-assignment
+```
+
+```py
+import pydiff
+
 ```
 
 ## Prerequisites
 
 - Python 3 (>= 3.11)
 
 ## How to use
 
 Install Python according to your preferences. Recommend to use direnv and pyenv.
 
 And then, install dependencies like below.
 
-```sh
+```
 pip install -r requirements.txt
 ```
 
 ### Reference Application
 
 If you're prepared, you can use it like below.
```

### Comparing `pydiff-planetarium-assignment-0.0.1/pydiff_planetarium_assignment.egg-info/PKG-INFO` & `pydiff-planetarium-assignment-0.0.2/pydiff_planetarium_assignment/pydiff_planetarium_assignment.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pydiff-planetarium-assignment
-Version: 0.0.1
-Summary: Simple implementation of unixdiff
+Version: 0.0.2
+Summary: Simple implementation of unix diff
 Home-page: https://github.com/planetarium/take-home-2023-channprj
 Author: channprj
 Author-email: chann@chann.dev
 Project-URL: Bug Tracker, https://github.com/planetarium/take-home-2023-channprj/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -20,29 +20,36 @@
 - [x] Split and refine codes
 - [x] Wrap as a python packages using `pyproject.toml`
 - [ ] Write pure implementation of diff
 - [x] Add more documentation
 
 ## TLDR;
 
+Install package and import this.
+
 ```sh
-pip install pydiff
+pip install pydiff-planetarium-assignment
+```
+
+```py
+import pydiff
+
 ```
 
 ## Prerequisites
 
 - Python 3 (>= 3.11)
 
 ## How to use
 
 Install Python according to your preferences. Recommend to use direnv and pyenv.
 
 And then, install dependencies like below.
 
-```sh
+```
 pip install -r requirements.txt
 ```
 
 ### Reference Application
 
 If you're prepared, you can use it like below.
```

### Comparing `pydiff-planetarium-assignment-0.0.1/setup.py` & `pydiff-planetarium-assignment-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pydiff-planetarium-assignment',
-    version='0.0.1',
+    version='0.0.2',
     author='channprj',
     author_email='chann@chann.dev',
-    description='Simple implementation of unixdiff',
+    description='Simple implementation of unix diff',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/planetarium/take-home-2023-channprj',
     project_urls={
         'Bug Tracker':
         'https://github.com/planetarium/take-home-2023-channprj/issues',
     },
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
-    package_dir={'': '.'},
+    package_dir={'': 'pydiff_planetarium_assignment'},
     packages=setuptools.find_packages(where='src'),
     python_requires='>=3.11',
 )
```

