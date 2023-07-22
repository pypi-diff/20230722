# Comparing `tmp/pox-0.3.2.tar.gz` & `tmp/pox-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pox-0.3.2.tar", last modified: Sun Oct 23 20:05:55 2022, max compression
+gzip compressed data, was "pox-0.3.3.tar", last modified: Sat Jul 22 20:28:55 2023, max compression
```

## Comparing `pox-0.3.2.tar` & `pox-0.3.3.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxr-xr-x   0 mmckerns   (501) staff       (20)        0 2022-10-23 20:05:55.597947 pox-0.3.2/
--rw-r--r--   0 mmckerns   (501) staff       (20)      829 2022-05-16 22:36:47.000000 pox-0.3.2/.codecov.yml
--rw-r--r--   0 mmckerns   (501) staff       (20)      540 2022-05-16 22:36:47.000000 pox-0.3.2/.coveragerc
--rw-r--r--   0 mmckerns   (501) staff       (20)       32 2016-12-29 19:33:18.000000 pox-0.3.2/.gitignore
--rw-r--r--   0 mmckerns   (501) staff       (20)      285 2022-05-16 22:37:05.000000 pox-0.3.2/.readthedocs.yml
--rw-r--r--   0 mmckerns   (501) staff       (20)     1143 2022-07-02 18:09:45.000000 pox-0.3.2/.travis.yml
--rw-r--r--   0 mmckerns   (501) staff       (20)     1790 2022-01-01 16:19:30.000000 pox-0.3.2/LICENSE
--rw-r--r--   0 mmckerns   (501) staff       (20)      219 2022-07-05 23:17:21.000000 pox-0.3.2/MANIFEST.in
--rw-r--r--   0 mmckerns   (501) staff       (20)     7945 2022-10-23 20:05:55.598204 pox-0.3.2/PKG-INFO
--rw-r--r--   0 mmckerns   (501) staff       (20)     7378 2022-05-25 17:58:38.000000 pox-0.3.2/README.md
-drwxr-xr-x   0 mmckerns   (501) staff       (20)        0 2022-10-23 20:05:55.570624 pox-0.3.2/docs/
--rw-r--r--   0 mmckerns   (501) staff       (20)      667 2022-05-16 22:36:47.000000 pox-0.3.2/docs/Makefile
--rw-r--r--   0 mmckerns   (501) staff       (20)      430 2022-05-17 16:10:16.000000 pox-0.3.2/docs/requirements.txt
-drwxr-xr-x   0 mmckerns   (501) staff       (20)        0 2022-10-23 20:05:55.577365 pox-0.3.2/docs/source/
--rw-r--r--   0 mmckerns   (501) staff       (20)     7328 2022-07-06 19:25:25.000000 pox-0.3.2/docs/source/conf.py
--rw-r--r--   0 mmckerns   (501) staff       (20)      376 2017-08-23 20:59:24.000000 pox-0.3.2/docs/source/index.rst
--rw-r--r--   0 mmckerns   (501) staff       (20)    78646 2017-08-11 19:09:08.000000 pox-0.3.2/docs/source/pathos.png
--rw-r--r--   0 mmckerns   (501) staff       (20)      609 2017-08-22 19:38:59.000000 pox-0.3.2/docs/source/pox.rst
--rw-r--r--   0 mmckerns   (501) staff       (20)      121 2018-05-26 14:51:35.000000 pox-0.3.2/docs/source/scripts.rst
-drwxr-xr-x   0 mmckerns   (501) staff       (20)        0 2022-10-23 20:05:55.584025 pox-0.3.2/pox/
--rw-r--r--   0 mmckerns   (501) staff       (20)     8781 2022-10-23 20:05:55.000000 pox-0.3.2/pox/__info__.py
--rw-r--r--   0 mmckerns   (501) staff       (20)     1631 2022-07-06 21:24:44.000000 pox-0.3.2/pox/__init__.py
--rw-r--r--   0 mmckerns   (501) staff       (20)     1673 2022-01-01 16:19:30.000000 pox-0.3.2/pox/__main__.py
--rw-r--r--   0 mmckerns   (501) staff       (20)     4269 2022-01-01 16:19:30.000000 pox-0.3.2/pox/_disk.py
--rw-r--r--   0 mmckerns   (501) staff       (20)    17985 2022-06-26 21:12:46.000000 pox-0.3.2/pox/shutils.py
-drwxr-xr-x   0 mmckerns   (501) staff       (20)        0 2022-10-23 20:05:55.591595 pox-0.3.2/pox/tests/
--rw-r--r--   0 mmckerns   (501) staff       (20)      498 2022-01-01 16:19:30.000000 pox-0.3.2/pox/tests/__init__.py
--rw-r--r--   0 mmckerns   (501) staff       (20)      839 2022-07-09 10:33:58.000000 pox-0.3.2/pox/tests/__main__.py
--rw-r--r--   0 mmckerns   (501) staff       (20)     3850 2022-05-25 18:04:42.000000 pox-0.3.2/pox/tests/test_shutils.py
--rw-r--r--   0 mmckerns   (501) staff       (20)     4781 2022-01-01 16:19:30.000000 pox-0.3.2/pox/tests/test_utils.py
--rw-r--r--   0 mmckerns   (501) staff       (20)    20679 2022-01-01 16:19:30.000000 pox-0.3.2/pox/utils.py
-drwxr-xr-x   0 mmckerns   (501) staff       (20)        0 2022-10-23 20:05:55.588291 pox-0.3.2/pox.egg-info/
--rw-r--r--   0 mmckerns   (501) staff       (20)     7945 2022-10-23 20:05:55.000000 pox-0.3.2/pox.egg-info/PKG-INFO
--rw-r--r--   0 mmckerns   (501) staff       (20)      721 2022-10-23 20:05:55.000000 pox-0.3.2/pox.egg-info/SOURCES.txt
--rw-r--r--   0 mmckerns   (501) staff       (20)        1 2022-10-23 20:05:55.000000 pox-0.3.2/pox.egg-info/dependency_links.txt
--rw-r--r--   0 mmckerns   (501) staff       (20)        1 2022-10-23 20:05:55.000000 pox-0.3.2/pox.egg-info/not-zip-safe
--rw-r--r--   0 mmckerns   (501) staff       (20)        4 2022-10-23 20:05:55.000000 pox-0.3.2/pox.egg-info/top_level.txt
--rw-r--r--   0 mmckerns   (501) staff       (20)      166 2022-05-20 09:49:08.000000 pox-0.3.2/pyproject.toml
-drwxr-xr-x   0 mmckerns   (501) staff       (20)        0 2022-10-23 20:05:55.592394 pox-0.3.2/scripts/
--rw-r--r--   0 mmckerns   (501) staff       (20)      692 2022-01-01 16:19:30.000000 pox-0.3.2/scripts/pox
--rw-r--r--   0 mmckerns   (501) staff       (20)       62 2022-10-23 20:05:55.599166 pox-0.3.2/setup.cfg
--rw-r--r--   0 mmckerns   (501) staff       (20)     3926 2022-08-10 11:33:35.000000 pox-0.3.2/setup.py
-drwxr-xr-x   0 mmckerns   (501) staff       (20)        0 2022-10-23 20:05:55.597313 pox-0.3.2/tools/
--rw-r--r--   0 mmckerns   (501) staff       (20)     1155 2013-11-22 21:24:26.000000 pox-0.3.2/tools/README
--rw-r--r--   0 mmckerns   (501) staff       (20)      590 2022-01-01 16:19:30.000000 pox-0.3.2/tools/bash_profile
--rw-r--r--   0 mmckerns   (501) staff       (20)      773 2022-01-01 16:19:30.000000 pox-0.3.2/tools/pathosrc
--rw-r--r--   0 mmckerns   (501) staff       (20)     1801 2022-01-01 16:19:30.000000 pox-0.3.2/tools/pythonstartup
--rw-r--r--   0 mmckerns   (501) staff       (20)      849 2022-01-01 16:19:30.000000 pox-0.3.2/tools/ssh_agent
--rw-r--r--   0 mmckerns   (501) staff       (20)      394 2022-01-01 16:19:30.000000 pox-0.3.2/tools/ssh_config
--rw-r--r--   0 mmckerns   (501) staff       (20)      354 2022-07-09 10:40:22.000000 pox-0.3.2/tox.ini
--rw-r--r--   0 mmckerns   (501) staff       (20)     2730 2022-10-23 20:04:38.000000 pox-0.3.2/version.py
+drwxr-xr-x   0 mmckerns   (501) staff       (20)        0 2023-07-22 20:28:55.462035 pox-0.3.3/
+-rw-r--r--   0 mmckerns   (501) staff       (20)      829 2022-05-16 22:36:47.000000 pox-0.3.3/.codecov.yml
+-rw-r--r--   0 mmckerns   (501) staff       (20)      540 2022-05-16 22:36:47.000000 pox-0.3.3/.coveragerc
+-rw-r--r--   0 mmckerns   (501) staff       (20)       32 2016-12-29 19:33:18.000000 pox-0.3.3/.gitignore
+-rw-r--r--   0 mmckerns   (501) staff       (20)      285 2022-05-16 22:37:05.000000 pox-0.3.3/.readthedocs.yml
+-rw-r--r--   0 mmckerns   (501) staff       (20)     1571 2023-07-07 03:02:11.000000 pox-0.3.3/.travis.yml
+-rw-r--r--   0 mmckerns   (501) staff       (20)     1790 2023-02-08 18:06:12.000000 pox-0.3.3/LICENSE
+-rw-r--r--   0 mmckerns   (501) staff       (20)      219 2022-07-05 23:17:21.000000 pox-0.3.3/MANIFEST.in
+-rw-r--r--   0 mmckerns   (501) staff       (20)     7996 2023-07-22 20:28:55.462922 pox-0.3.3/PKG-INFO
+-rw-r--r--   0 mmckerns   (501) staff       (20)     7514 2023-03-10 04:03:24.000000 pox-0.3.3/README.md
+drwxr-xr-x   0 mmckerns   (501) staff       (20)        0 2023-07-22 20:28:55.428036 pox-0.3.3/docs/
+-rw-r--r--   0 mmckerns   (501) staff       (20)      667 2022-05-16 22:36:47.000000 pox-0.3.3/docs/Makefile
+-rw-r--r--   0 mmckerns   (501) staff       (20)      430 2023-07-22 01:39:02.000000 pox-0.3.3/docs/requirements.txt
+drwxr-xr-x   0 mmckerns   (501) staff       (20)        0 2023-07-22 20:28:55.438051 pox-0.3.3/docs/source/
+drwxr-xr-x   0 mmckerns   (501) staff       (20)        0 2023-07-22 20:28:55.412718 pox-0.3.3/docs/source/_static/
+drwxr-xr-x   0 mmckerns   (501) staff       (20)        0 2023-07-22 20:28:55.440838 pox-0.3.3/docs/source/_static/css/
+-rw-r--r--   0 mmckerns   (501) staff       (20)       85 2023-07-05 04:39:45.000000 pox-0.3.3/docs/source/_static/css/custom.css
+-rw-r--r--   0 mmckerns   (501) staff       (20)     7917 2023-07-05 04:58:37.000000 pox-0.3.3/docs/source/conf.py
+-rw-r--r--   0 mmckerns   (501) staff       (20)      297 2023-07-05 05:54:29.000000 pox-0.3.3/docs/source/index.rst
+-rw-r--r--   0 mmckerns   (501) staff       (20)    78646 2017-08-11 19:09:08.000000 pox-0.3.3/docs/source/pathos.png
+-rw-r--r--   0 mmckerns   (501) staff       (20)      362 2023-02-05 00:04:37.000000 pox-0.3.3/docs/source/pox.rst
+-rw-r--r--   0 mmckerns   (501) staff       (20)      130 2023-02-05 00:04:43.000000 pox-0.3.3/docs/source/scripts.rst
+drwxr-xr-x   0 mmckerns   (501) staff       (20)        0 2023-07-22 20:28:55.446637 pox-0.3.3/pox/
+-rw-r--r--   0 mmckerns   (501) staff       (20)     8781 2023-07-22 20:28:55.000000 pox-0.3.3/pox/__info__.py
+-rw-r--r--   0 mmckerns   (501) staff       (20)     1631 2023-01-01 13:06:47.000000 pox-0.3.3/pox/__init__.py
+-rw-r--r--   0 mmckerns   (501) staff       (20)     1673 2023-01-01 13:06:47.000000 pox-0.3.3/pox/__main__.py
+-rw-r--r--   0 mmckerns   (501) staff       (20)     4270 2023-02-19 21:15:48.000000 pox-0.3.3/pox/_disk.py
+-rw-r--r--   0 mmckerns   (501) staff       (20)    17985 2023-01-01 13:06:47.000000 pox-0.3.3/pox/shutils.py
+drwxr-xr-x   0 mmckerns   (501) staff       (20)        0 2023-07-22 20:28:55.454482 pox-0.3.3/pox/tests/
+-rw-r--r--   0 mmckerns   (501) staff       (20)      498 2023-01-01 13:06:47.000000 pox-0.3.3/pox/tests/__init__.py
+-rw-r--r--   0 mmckerns   (501) staff       (20)      839 2023-01-01 13:06:47.000000 pox-0.3.3/pox/tests/__main__.py
+-rw-r--r--   0 mmckerns   (501) staff       (20)     3850 2023-01-01 13:06:47.000000 pox-0.3.3/pox/tests/test_shutils.py
+-rw-r--r--   0 mmckerns   (501) staff       (20)     4781 2023-01-01 13:06:47.000000 pox-0.3.3/pox/tests/test_utils.py
+-rw-r--r--   0 mmckerns   (501) staff       (20)    20679 2023-01-01 13:06:47.000000 pox-0.3.3/pox/utils.py
+drwxr-xr-x   0 mmckerns   (501) staff       (20)        0 2023-07-22 20:28:55.450843 pox-0.3.3/pox.egg-info/
+-rw-r--r--   0 mmckerns   (501) staff       (20)     7996 2023-07-22 20:28:55.000000 pox-0.3.3/pox.egg-info/PKG-INFO
+-rw-r--r--   0 mmckerns   (501) staff       (20)      756 2023-07-22 20:28:55.000000 pox-0.3.3/pox.egg-info/SOURCES.txt
+-rw-r--r--   0 mmckerns   (501) staff       (20)        1 2023-07-22 20:28:55.000000 pox-0.3.3/pox.egg-info/dependency_links.txt
+-rw-r--r--   0 mmckerns   (501) staff       (20)        1 2023-07-22 20:28:55.000000 pox-0.3.3/pox.egg-info/not-zip-safe
+-rw-r--r--   0 mmckerns   (501) staff       (20)        4 2023-07-22 20:28:55.000000 pox-0.3.3/pox.egg-info/top_level.txt
+-rw-r--r--   0 mmckerns   (501) staff       (20)      166 2022-05-20 09:49:08.000000 pox-0.3.3/pyproject.toml
+drwxr-xr-x   0 mmckerns   (501) staff       (20)        0 2023-07-22 20:28:55.455387 pox-0.3.3/scripts/
+-rw-r--r--   0 mmckerns   (501) staff       (20)      692 2023-01-01 13:06:47.000000 pox-0.3.3/scripts/pox
+-rw-r--r--   0 mmckerns   (501) staff       (20)       62 2023-07-22 20:28:55.464341 pox-0.3.3/setup.cfg
+-rw-r--r--   0 mmckerns   (501) staff       (20)     3976 2023-01-01 13:06:52.000000 pox-0.3.3/setup.py
+drwxr-xr-x   0 mmckerns   (501) staff       (20)        0 2023-07-22 20:28:55.460890 pox-0.3.3/tools/
+-rw-r--r--   0 mmckerns   (501) staff       (20)     1155 2013-11-22 21:24:26.000000 pox-0.3.3/tools/README
+-rw-r--r--   0 mmckerns   (501) staff       (20)      590 2023-01-01 13:06:47.000000 pox-0.3.3/tools/bash_profile
+-rw-r--r--   0 mmckerns   (501) staff       (20)      773 2023-01-01 13:06:47.000000 pox-0.3.3/tools/pathosrc
+-rw-r--r--   0 mmckerns   (501) staff       (20)     1801 2023-01-01 13:06:47.000000 pox-0.3.3/tools/pythonstartup
+-rw-r--r--   0 mmckerns   (501) staff       (20)      849 2023-01-01 13:06:47.000000 pox-0.3.3/tools/ssh_agent
+-rw-r--r--   0 mmckerns   (501) staff       (20)      394 2023-01-01 13:06:47.000000 pox-0.3.3/tools/ssh_config
+-rw-r--r--   0 mmckerns   (501) staff       (20)      376 2023-07-07 02:30:54.000000 pox-0.3.3/tox.ini
+-rw-r--r--   0 mmckerns   (501) staff       (20)     3168 2023-07-22 20:27:36.000000 pox-0.3.3/version.py
```

### Comparing `pox-0.3.2/.codecov.yml` & `pox-0.3.3/.codecov.yml`

 * *Files identical despite different names*

### Comparing `pox-0.3.2/.coveragerc` & `pox-0.3.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `pox-0.3.2/LICENSE` & `pox-0.3.3/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Copyright (c) 2004-2016 California Institute of Technology.
-Copyright (c) 2016-2022 The Uncertainty Quantification Foundation.
+Copyright (c) 2016-2023 The Uncertainty Quantification Foundation.
 All rights reserved.
 
 This software is available subject to the conditions and terms laid
 out below. By downloading and using this software you are agreeing
 to the following conditions.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
-are met::
+are met:
 
-    - Redistribution of source code must retain the above copyright
+    - Redistributions of source code must retain the above copyright
       notice, this list of conditions and the following disclaimer.
 
-    - Redistribution in binary form must reproduce the above copyright
+    - Redistributions in binary form must reproduce the above copyright
       notice, this list of conditions and the following disclaimer in the
-      documentations and/or other materials provided with the distribution.
+      documentation and/or other materials provided with the distribution.
 
     - Neither the names of the copyright holders nor the names of any of
       the contributors may be used to endorse or promote products derived
       from this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
 "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
```

### Comparing `pox-0.3.2/PKG-INFO` & `pox-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pox
-Version: 0.3.2
+Version: 0.3.3
 Summary: utilities for filesystem exploration and automated builds
 Home-page: https://github.com/uqfoundation/pox
 Download-URL: https://pypi.org/project/pox/#files
 Author: Mike McKerns
 Author-email: mmckerns@uqfoundation.org
 Maintainer: Mike McKerns
 Maintainer-email: mmckerns@uqfoundation.org
@@ -20,14 +20,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 License-File: LICENSE
 
@@ -44,31 +45,31 @@
 on a remote host, where queries such as *"what is the root of the filesystem?"*,
 *"what is the user's name?"*, and *"what login shell is preferred?"* become
 essential in allowing a remote user to function as if they were logged in
 locally. While ``pox`` is in the same vein of both the ``os`` and ``shutil``
 builtin modules, the majority of its functionality is unique and compliments
 these two modules.
 
-``pox`` provides python equivalents of several unix shell commands such as
+``pox`` provides Python equivalents of several unix shell commands such as
 ``which`` and ``find``. These commands allow automated discovery of what has
 been installed on an operating system, and where the essential tools are
 located. This capability is useful not only for exploring remote hosts,
 but also locally as a helper utility for automated build and installation.
 
 Several high-level operations on files and filesystems are also provided.
-Examples of which are: finding the location of an installed python package,
+Examples of which are: finding the location of an installed Python package,
 determining if and where the source code resides on the filesystem, and
 determining what version the installed package is.
 
 ``pox`` also provides utilities to enable the abstraction of commands sent
 to a remote filesystem.  In conjunction with a registry of environment
 variables and installed utilites, ``pox`` enables the user to interact with
 a remote filesystem as if they were logged in locally. 
 
-``pox`` is part of ``pathos``, a python framework for heterogeneous computing.
+``pox`` is part of ``pathos``, a Python framework for heterogeneous computing.
 ``pox`` is in active development, so any user feedback, bug reports, comments,
 or suggestions are highly appreciated.  A list of issues is located at https://github.com/uqfoundation/pox/issues, with a legacy list maintained at https://uqfoundation.github.io/project/pathos/query.
 
 
 Major Features
 ==============
 
@@ -151,15 +152,15 @@
 and perform some basic search functions::
 
     >>> pox.find('python3.9', recurse=5, root='/opt')
     ['/opt/local/bin/python3.9']
     >>> pox.which('python3.9')
     '/opt/local/bin/python3.9'
 
-``pox`` also has a specialized `which` command just for python::
+``pox`` also has a specialized `which` command just for Python::
 
     >>> pox.which_python()
     '/opt/local/bin/python3.9'
     >>> pox.which_python(lazy=True, version=True)
     '`which python3.9`'
 
 Any of the ``pox`` functions can be launched from the command line,
```

### Comparing `pox-0.3.2/README.md` & `pox-0.3.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 on a remote host, where queries such as *"what is the root of the filesystem?"*,
 *"what is the user's name?"*, and *"what login shell is preferred?"* become
 essential in allowing a remote user to function as if they were logged in
 locally. While ``pox`` is in the same vein of both the ``os`` and ``shutil``
 builtin modules, the majority of its functionality is unique and compliments
 these two modules.
 
-``pox`` provides python equivalents of several unix shell commands such as
+``pox`` provides Python equivalents of several unix shell commands such as
 ``which`` and ``find``. These commands allow automated discovery of what has
 been installed on an operating system, and where the essential tools are
 located. This capability is useful not only for exploring remote hosts,
 but also locally as a helper utility for automated build and installation.
 
 Several high-level operations on files and filesystems are also provided.
-Examples of which are: finding the location of an installed python package,
+Examples of which are: finding the location of an installed Python package,
 determining if and where the source code resides on the filesystem, and
 determining what version the installed package is.
 
 ``pox`` also provides utilities to enable the abstraction of commands sent
 to a remote filesystem.  In conjunction with a registry of environment
 variables and installed utilites, ``pox`` enables the user to interact with
 a remote filesystem as if they were logged in locally. 
 
-``pox`` is part of ``pathos``, a python framework for heterogeneous computing.
+``pox`` is part of ``pathos``, a Python framework for heterogeneous computing.
 ``pox`` is in active development, so any user feedback, bug reports, comments,
 or suggestions are highly appreciated.  A list of issues is located at https://github.com/uqfoundation/pox/issues, with a legacy list maintained at https://uqfoundation.github.io/project/pathos/query.
 
 
 Major Features
 --------------
 ``pox`` provides utilities for discovering the user's environment:
@@ -50,14 +50,15 @@
 * parse operating system commands for remote shell invocation
 * convert text files to platform-specific formatting
 
 
 Current Release
 [![Downloads](https://static.pepy.tech/personalized-badge/pox?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads)](https://pepy.tech/project/pox)
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/pox?color=blue&label=conda%20downloads)](https://anaconda.org/conda-forge/pox)
+[![Stack Overflow](https://img.shields.io/badge/stackoverflow-get%20help-black.svg)](https://stackoverflow.com/questions/tagged/pathos)
 ---------------
 The latest released version of ``pox`` is available from:
     https://pypi.org/project/pox
 
 ``pox`` is distributed under a 3-clause BSD license.
 
 
@@ -115,15 +116,15 @@
 and perform some basic search functions::
 
     >>> pox.find('python3.9', recurse=5, root='/opt')
     ['/opt/local/bin/python3.9']
     >>> pox.which('python3.9')
     '/opt/local/bin/python3.9'
 
-``pox`` also has a specialized `which` command just for python::
+``pox`` also has a specialized `which` command just for Python::
 
     >>> pox.which_python()
     '/opt/local/bin/python3.9'
     >>> pox.which_python(lazy=True, version=True)
     '`which python3.9`'
 
 Any of the ``pox`` functions can be launched from the command line,
```

### Comparing `pox-0.3.2/docs/Makefile` & `pox-0.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pox-0.3.2/docs/source/conf.py` & `pox-0.3.3/docs/source/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,24 +53,42 @@
 # source_suffix = ['.rst', '.md']
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = u'pox'
+project = 'pox'
 year = datetime.now().year
-copyright = u'%d, The Uncertainty Quantification Foundation' % year
-author = u'Mike McKerns'
+copyright = '%d, The Uncertainty Quantification Foundation' % year
+author = 'Mike McKerns'
 
 # extension config
 github_project_url = "https://github.com/uqfoundation/pox"
 autoclass_content = 'both'
+autodoc_default_options = {
+    'members': True,
+    'undoc-members': True,
+    'private-members': True,
+    'special-members': True,
+    'show-inheritance': True,
+    'imported-members': True,
+    'exclude-members': (
+        '__dict__,'
+        '__slots__,'
+        '__weakref__,'
+        '__module__,'
+        '_abc_impl,'
+        '__init__,'
+        '__annotations__,'
+        '__dataclass_fields__,'
+    )
+}
 autodoc_typehints = 'description'
-napoleon_include_init_with_doc = True
+autodoc_typehints_format = 'short'
 napoleon_include_private_with_doc = False
 napoleon_include_special_with_doc = True
 napoleon_use_ivar = True
 napoleon_use_param = True
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
@@ -82,15 +100,15 @@
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
@@ -110,57 +128,63 @@
 on_rtd = os.environ.get('READTHEDOCS', None) == 'True'
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 if not on_rtd:
     html_theme = 'alabaster' #'bizstyle'
+    html_css_files = ['css/custom.css',]
    #import sphinx_rtd_theme
    #html_theme = 'sphinx_rtd_theme'
    #html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 html_theme_options = {
     'github_user': 'uqfoundation',
     'github_repo': 'pox',
     'github_button': False,
     'github_banner': True,
     'travis_button': True,
+    'codecov_button': True,
+    'donate_url': 'http://uqfoundation.org/pages/donate.html',
     'gratipay_user': False,  # username
     'extra_nav_links': {'Module Index': 'py-modindex.html'},
 #   'show_related': True,
+#   'globaltoc_collapse': True,
+    'globaltoc_maxdepth': 4,
     'show_powered_by': False
 }
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
 # Custom sidebar templates, must be a dictionary that maps document names
 # to template names.
 #
 # This is required for the alabaster theme
 # refs: http://alabaster.readthedocs.io/en/latest/installation.html#sidebars
-#if html_theme == 'alabaster':
+if on_rtd:
+    toc_style = 'localtoc.html', # display the toctree
+else:
+    toc_style = 'globaltoc.html', # collapse the toctree
 html_sidebars = {
     '**': [
         'about.html',
+        'donate.html',
+        'searchbox.html',
 #       'navigation.html',
-        'localtoc.html', # display the toctree
+        toc_style, # defined above
         'relations.html', # needs 'show_related':True option to display
-        'searchbox.html',
-        'donate.html', # needs 'gratipay_user':<uname> option to display
     ]
 }
-#FIXME: donate / UQFoundation (home/github)
-
 
 # -- Options for HTMLHelp output ------------------------------------------
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = 'poxdoc'
 
 # Logo for sidebar
@@ -187,45 +211,45 @@
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'pox.tex', u'pox Documentation',
-     u'Mike McKerns', 'manual'),
+    (master_doc, 'pox.tex', 'pox Documentation',
+     'Mike McKerns', 'manual'),
 ]
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    (master_doc, 'pox', u'pox Documentation',
+    (master_doc, 'pox', 'pox Documentation',
      [author], 1)
 ]
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'pox', u'pox Documentation',
+    (master_doc, 'pox', 'pox Documentation',
      author, 'pox', 'Utilities for filesystem exploration and automated builds.',
      'Miscellaneous'),
 ]
 
 
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'https://docs.python.org/': None}
+intersphinx_mapping = {'https://docs.python.org/3/': None}
 #    {'python': {'https://docs.python.org/': None},
 #     'mystic': {'https://mystic.readthedocs.io/en/latest/', None},
 #     'pathos': {'https://pathos.readthedocs.io/en/latest/', None},
 #     'klepto': {'https://klepto.readthedocs.io/en/latest/', None},
 #     'dill': {'https://dill.readthedocs.io/en/latest/', None},
 #     'multiprocess': {'https://multiprocess.readthedocs.io/en/latest/', None},
 #     'ppft': {'https://ppft.readthedocs.io/en/latest/', None},
```

### Comparing `pox-0.3.2/docs/source/pathos.png` & `pox-0.3.3/docs/source/pathos.png`

 * *Files identical despite different names*

### Comparing `pox-0.3.2/pox/__info__.py` & `pox-0.3.3/pox/__info__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 #
 # Author: Mike McKerns (mmckerns @caltech and @uqfoundation)
-# Copyright (c) 2022 The Uncertainty Quantification Foundation.
+# Copyright (c) 2023 The Uncertainty Quantification Foundation.
 # License: 3-clause BSD.  The full license text is available at:
 #  - https://github.com/uqfoundation/pox/blob/master/LICENSE
 '''
 --------------------------------------------------------------
 pox: utilities for filesystem exploration and automated builds
 --------------------------------------------------------------
 
@@ -18,31 +18,31 @@
 on a remote host, where queries such as *"what is the root of the filesystem?"*,
 *"what is the user's name?"*, and *"what login shell is preferred?"* become
 essential in allowing a remote user to function as if they were logged in
 locally. While ``pox`` is in the same vein of both the ``os`` and ``shutil``
 builtin modules, the majority of its functionality is unique and compliments
 these two modules.
 
-``pox`` provides python equivalents of several unix shell commands such as
+``pox`` provides Python equivalents of several unix shell commands such as
 ``which`` and ``find``. These commands allow automated discovery of what has
 been installed on an operating system, and where the essential tools are
 located. This capability is useful not only for exploring remote hosts,
 but also locally as a helper utility for automated build and installation.
 
 Several high-level operations on files and filesystems are also provided.
-Examples of which are: finding the location of an installed python package,
+Examples of which are: finding the location of an installed Python package,
 determining if and where the source code resides on the filesystem, and
 determining what version the installed package is.
 
 ``pox`` also provides utilities to enable the abstraction of commands sent
 to a remote filesystem.  In conjunction with a registry of environment
 variables and installed utilites, ``pox`` enables the user to interact with
 a remote filesystem as if they were logged in locally. 
 
-``pox`` is part of ``pathos``, a python framework for heterogeneous computing.
+``pox`` is part of ``pathos``, a Python framework for heterogeneous computing.
 ``pox`` is in active development, so any user feedback, bug reports, comments,
 or suggestions are highly appreciated.  A list of issues is located at https://github.com/uqfoundation/pox/issues, with a legacy list maintained at https://uqfoundation.github.io/project/pathos/query.
 
 
 Major Features
 ==============
 
@@ -125,15 +125,15 @@
 and perform some basic search functions::
 
     >>> pox.find('python3.9', recurse=5, root='/opt')
     ['/opt/local/bin/python3.9']
     >>> pox.which('python3.9')
     '/opt/local/bin/python3.9'
 
-``pox`` also has a specialized `which` command just for python::
+``pox`` also has a specialized `which` command just for Python::
 
     >>> pox.which_python()
     '/opt/local/bin/python3.9'
     >>> pox.which_python(lazy=True, version=True)
     '`which python3.9`'
 
 Any of the ``pox`` functions can be launched from the command line,
@@ -185,36 +185,36 @@
     https://uqfoundation.github.io/project/pathos
 
 Please see https://uqfoundation.github.io/project/pathos or
 http://arxiv.org/pdf/1202.1056 for further information.
 
 '''
 
-__version__ = '0.3.2'
+__version__ = '0.3.3'
 __author__ = 'Mike McKerns'
 
 __license__ = '''
 Copyright (c) 2004-2016 California Institute of Technology.
-Copyright (c) 2016-2022 The Uncertainty Quantification Foundation.
+Copyright (c) 2016-2023 The Uncertainty Quantification Foundation.
 All rights reserved.
 
 This software is available subject to the conditions and terms laid
 out below. By downloading and using this software you are agreeing
 to the following conditions.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
-are met::
+are met:
 
-    - Redistribution of source code must retain the above copyright
+    - Redistributions of source code must retain the above copyright
       notice, this list of conditions and the following disclaimer.
 
-    - Redistribution in binary form must reproduce the above copyright
+    - Redistributions in binary form must reproduce the above copyright
       notice, this list of conditions and the following disclaimer in the
-      documentations and/or other materials provided with the distribution.
+      documentation and/or other materials provided with the distribution.
 
     - Neither the names of the copyright holders nor the names of any of
       the contributors may be used to endorse or promote products derived
       from this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
 "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
```

### Comparing `pox-0.3.2/pox/__init__.py` & `pox-0.3.3/pox/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # Author: Mike McKerns (mmckerns @caltech and @uqfoundation)
 # Copyright (c) 1997-2016 California Institute of Technology.
-# Copyright (c) 2016-2022 The Uncertainty Quantification Foundation.
+# Copyright (c) 2016-2023 The Uncertainty Quantification Foundation.
 # License: 3-clause BSD.  The full license text is available at:
 #  - https://github.com/uqfoundation/pox/blob/master/LICENSE
 
 # author, version, license, and long description
 try: # the package is installed
     from .__info__ import __version__, __author__, __doc__, __license__
 except: # pragma: no cover
```

### Comparing `pox-0.3.2/pox/__main__.py` & `pox-0.3.3/pox/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # Author: Mike McKerns (mmckerns @caltech and @uqfoundation)
 # Copyright (c) 1997-2016 California Institute of Technology.
-# Copyright (c) 2016-2022 The Uncertainty Quantification Foundation.
+# Copyright (c) 2016-2023 The Uncertainty Quantification Foundation.
 # License: 3-clause BSD.  The full license text is available at:
 #  - https://github.com/uqfoundation/pox/blob/master/LICENSE
 """
 run any of the pox commands from the command shell prompt
 
 Notes:
     - To get help, type ``$ pox`` at a shell terminal prompt.
```

### Comparing `pox-0.3.2/pox/_disk.py` & `pox-0.3.3/pox/_disk.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #          Lars Buitinck <L.J.Buitinck@uva.nl>
 # Copyright (c) 2010 Gael Varoquaux
 # License: BSD Style, 3 clauses.
 
 # Forked by: Mike McKerns (December 2013)
 # Author: Mike McKerns (mmckerns @caltech and @uqfoundation)
 # Copyright (c) 2013-2016 California Institute of Technology.
-# Copyright (c) 2016-2022 The Uncertainty Quantification Foundation.
+# Copyright (c) 2016-2023 The Uncertainty Quantification Foundation.
 # License: 3-clause BSD.  The full license text is available at:
 #  - https://github.com/uqfoundation/pox/blob/master/LICENSE
 """
 Disk management utilities.
 """
 
 import os
@@ -88,15 +88,16 @@
     Returns:
         None
 
     Notes:
         If self=False, the directory indicated by path is left in place,
         and its subdirectories are erased. If self=True, path is also removed.
 
-        If ignore_errors=True, errors are ignored. Otherwise, onerror is called        to handle the error with arguments ``(func, path, exc_info)``, where
+        If ignore_errors=True, errors are ignored. Otherwise, onerror is called
+        to handle the error with arguments ``(func, path, exc_info)``, where
         *func* is ``os.listdir``, ``os.remove``, or ``os.rmdir``; *path* is the
         argument to the function that caused it to fail; and *exc_info* is a
         tuple returned by ``sys.exc_info()``. If ignore_errors=False and
         onerror=None, an exception is raised.
     """
     names = []
     try:
```

### Comparing `pox-0.3.2/pox/shutils.py` & `pox-0.3.3/pox/shutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # Author: Mike McKerns (mmckerns @caltech and @uqfoundation)
 # Copyright (c) 1997-2016 California Institute of Technology.
-# Copyright (c) 2016-2022 The Uncertainty Quantification Foundation.
+# Copyright (c) 2016-2023 The Uncertainty Quantification Foundation.
 # License: 3-clause BSD.  The full license text is available at:
 #  - https://github.com/uqfoundation/pox/blob/master/LICENSE
 #
 # adapted from Mike McKerns' gsl.infect.shutils
 """
 shell utilities for user environment and filesystem exploration
 """
```

### Comparing `pox-0.3.2/pox/tests/__main__.py` & `pox-0.3.3/pox/tests/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 #
 # Author: Mike McKerns (mmckerns @caltech and @uqfoundation)
-# Copyright (c) 2018-2022 The Uncertainty Quantification Foundation.
+# Copyright (c) 2018-2023 The Uncertainty Quantification Foundation.
 # License: 3-clause BSD.  The full license text is available at:
 #  - https://github.com/uqfoundation/pox/blob/master/LICENSE
 
 import glob
 import os
 import sys
 import subprocess as sp
```

### Comparing `pox-0.3.2/pox/tests/test_shutils.py` & `pox-0.3.3/pox/tests/test_shutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # Author: Mike McKerns (mmckerns @caltech and @uqfoundation)
 # Copyright (c) 1997-2016 California Institute of Technology.
-# Copyright (c) 2016-2022 The Uncertainty Quantification Foundation.
+# Copyright (c) 2016-2023 The Uncertainty Quantification Foundation.
 # License: 3-clause BSD.  The full license text is available at:
 #  - https://github.com/uqfoundation/pox/blob/master/LICENSE
 """
 test pox's shell utilities
 """
 import os
```

### Comparing `pox-0.3.2/pox/tests/test_utils.py` & `pox-0.3.3/pox/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # Author: Mike McKerns (mmckerns @caltech and @uqfoundation)
 # Copyright (c) 1997-2016 California Institute of Technology.
-# Copyright (c) 2016-2022 The Uncertainty Quantification Foundation.
+# Copyright (c) 2016-2023 The Uncertainty Quantification Foundation.
 # License: 3-clause BSD.  The full license text is available at:
 #  - https://github.com/uqfoundation/pox/blob/master/LICENSE
 """
 test pox's higher-level shell utilities
 """
 import os
 import sys
```

### Comparing `pox-0.3.2/pox/utils.py` & `pox-0.3.3/pox/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # Author: Mike McKerns (mmckerns @caltech and @uqfoundation)
 # Copyright (c) 1997-2016 California Institute of Technology.
-# Copyright (c) 2016-2022 The Uncertainty Quantification Foundation.
+# Copyright (c) 2016-2023 The Uncertainty Quantification Foundation.
 # License: 3-clause BSD.  The full license text is available at:
 #  - https://github.com/uqfoundation/pox/blob/master/LICENSE
 #
 # adapted from Mike McKerns' gsl.infect.utils
 """
 higher-level shell utilities for user environment and filesystem exploration
 """
```

### Comparing `pox-0.3.2/pox.egg-info/PKG-INFO` & `pox-0.3.3/pox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pox
-Version: 0.3.2
+Version: 0.3.3
 Summary: utilities for filesystem exploration and automated builds
 Home-page: https://github.com/uqfoundation/pox
 Download-URL: https://pypi.org/project/pox/#files
 Author: Mike McKerns
 Author-email: mmckerns@uqfoundation.org
 Maintainer: Mike McKerns
 Maintainer-email: mmckerns@uqfoundation.org
@@ -20,14 +20,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 License-File: LICENSE
 
@@ -44,31 +45,31 @@
 on a remote host, where queries such as *"what is the root of the filesystem?"*,
 *"what is the user's name?"*, and *"what login shell is preferred?"* become
 essential in allowing a remote user to function as if they were logged in
 locally. While ``pox`` is in the same vein of both the ``os`` and ``shutil``
 builtin modules, the majority of its functionality is unique and compliments
 these two modules.
 
-``pox`` provides python equivalents of several unix shell commands such as
+``pox`` provides Python equivalents of several unix shell commands such as
 ``which`` and ``find``. These commands allow automated discovery of what has
 been installed on an operating system, and where the essential tools are
 located. This capability is useful not only for exploring remote hosts,
 but also locally as a helper utility for automated build and installation.
 
 Several high-level operations on files and filesystems are also provided.
-Examples of which are: finding the location of an installed python package,
+Examples of which are: finding the location of an installed Python package,
 determining if and where the source code resides on the filesystem, and
 determining what version the installed package is.
 
 ``pox`` also provides utilities to enable the abstraction of commands sent
 to a remote filesystem.  In conjunction with a registry of environment
 variables and installed utilites, ``pox`` enables the user to interact with
 a remote filesystem as if they were logged in locally. 
 
-``pox`` is part of ``pathos``, a python framework for heterogeneous computing.
+``pox`` is part of ``pathos``, a Python framework for heterogeneous computing.
 ``pox`` is in active development, so any user feedback, bug reports, comments,
 or suggestions are highly appreciated.  A list of issues is located at https://github.com/uqfoundation/pox/issues, with a legacy list maintained at https://uqfoundation.github.io/project/pathos/query.
 
 
 Major Features
 ==============
 
@@ -151,15 +152,15 @@
 and perform some basic search functions::
 
     >>> pox.find('python3.9', recurse=5, root='/opt')
     ['/opt/local/bin/python3.9']
     >>> pox.which('python3.9')
     '/opt/local/bin/python3.9'
 
-``pox`` also has a specialized `which` command just for python::
+``pox`` also has a specialized `which` command just for Python::
 
     >>> pox.which_python()
     '/opt/local/bin/python3.9'
     >>> pox.which_python(lazy=True, version=True)
     '`which python3.9`'
 
 Any of the ``pox`` functions can be launched from the command line,
```

### Comparing `pox-0.3.2/pox.egg-info/SOURCES.txt` & `pox-0.3.3/pox.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 docs/Makefile
 docs/requirements.txt
 docs/source/conf.py
 docs/source/index.rst
 docs/source/pathos.png
 docs/source/pox.rst
 docs/source/scripts.rst
+docs/source/_static/css/custom.css
 pox/__info__.py
 pox/__init__.py
 pox/__main__.py
 pox/_disk.py
 pox/shutils.py
 pox/utils.py
 pox.egg-info/PKG-INFO
```

### Comparing `pox-0.3.2/scripts/pox` & `pox-0.3.3/scripts/pox`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 #
 # Author: Mike McKerns (mmckerns @caltech and @uqfoundation)
-# Copyright (c) 2018-2022 The Uncertainty Quantification Foundation.
+# Copyright (c) 2018-2023 The Uncertainty Quantification Foundation.
 # License: 3-clause BSD.  The full license text is available at:
 #  - https://github.com/uqfoundation/pox/blob/master/LICENSE
 
 import pox.__main__
 from pox.__main__ import *
 __doc__ = pox.__main__.__doc__
```

### Comparing `pox-0.3.2/setup.py` & `pox-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # Author: Mike McKerns (mmckerns @caltech and @uqfoundation)
 # Copyright (c) 1997-2016 California Institute of Technology.
-# Copyright (c) 2016-2022 The Uncertainty Quantification Foundation.
+# Copyright (c) 2016-2023 The Uncertainty Quantification Foundation.
 # License: 3-clause BSD.  The full license text is available at:
 #  - https://github.com/uqfoundation/pox/blob/master/LICENSE
 
 import os
 import sys
 # drop support for older python
 if sys.version_info < (3, 7):
@@ -62,14 +62,15 @@
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
     ],
     packages = ['pox','pox.tests'],
     package_dir = {'pox':'pox','pox.tests':'pox/tests'},
```

### Comparing `pox-0.3.2/tools/README` & `pox-0.3.3/tools/README`

 * *Files identical despite different names*

### Comparing `pox-0.3.2/tools/bash_profile` & `pox-0.3.3/tools/bash_profile`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # .bash_profile (additions)
 #
 # Author: Mike McKerns (mmckerns @caltech and @uqfoundation)
 # Copyright (c) 1997-2016 California Institute of Technology.
-# Copyright (c) 2016-2022 The Uncertainty Quantification Foundation.
+# Copyright (c) 2016-2023 The Uncertainty Quantification Foundation.
 # License: 3-clause BSD.  The full license text is available at:
 #  - https://github.com/uqfoundation/pox/blob/master/LICENSE
 
 # Get standard aliases and functions
 if [ -f ~/.bashrc ]; then
 	. ~/.bashrc
 fi
```

### Comparing `pox-0.3.2/tools/pathosrc` & `pox-0.3.3/tools/pathosrc`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # .pathosrc
 #
 # Author: Mike McKerns (mmckerns @caltech and @uqfoundation)
 # Copyright (c) 1997-2016 California Institute of Technology.
-# Copyright (c) 2016-2022 The Uncertainty Quantification Foundation.
+# Copyright (c) 2016-2023 The Uncertainty Quantification Foundation.
 # License: 3-clause BSD.  The full license text is available at:
 #  - https://github.com/uqfoundation/pox/blob/master/LICENSE
 
 # user environment
 PATH=$PATH:.:$HOME/bin
 LD_LIBRARY_PATH=$LD_LIBRARY_PATH:.:$HOME/lib
 MYPYTHON = $HOME/python
```

### Comparing `pox-0.3.2/tools/pythonstartup` & `pox-0.3.3/tools/pythonstartup`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # to activate, run the following in your command shell:
 #   export PYTHONSTARTUP=$HOME/.python
 #   export PYTHONHISTORY=$HOME/.pyhistory
 #   cp ./pythonstartup $PYTHONSTARTUP
 #
 # Author: Mike McKerns (mmckerns @caltech and @uqfoundation)
 # Copyright (c) 1997-2016 California Institute of Technology.
-# Copyright (c) 2016-2022 The Uncertainty Quantification Foundation.
+# Copyright (c) 2016-2023 The Uncertainty Quantification Foundation.
 # License: 3-clause BSD.  The full license text is available at:
 #  - https://github.com/uqfoundation/pox/blob/master/LICENSE
 
 try:
   import readline
 except ImportError:
   print ("Module readline not available.")
```

### Comparing `pox-0.3.2/tools/ssh_agent` & `pox-0.3.3/tools/ssh_agent`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # .ssh_agent
 #
 # Author: Mike McKerns (mmckerns @caltech and @uqfoundation)
 # Copyright (c) 1997-2016 California Institute of Technology.
-# Copyright (c) 2016-2022 The Uncertainty Quantification Foundation.
+# Copyright (c) 2016-2023 The Uncertainty Quantification Foundation.
 # License: 3-clause BSD.  The full license text is available at:
 #  - https://github.com/uqfoundation/pox/blob/master/LICENSE
 
 # --- ssh-agent ---
 # If this shell is interactive, restart it within an ssh-agent.  This
 # depends on ssh-agent and ssh-add being on the user's default PATH, which
 # should be the case if they're in /usr/bin where they should be.
```

### Comparing `pox-0.3.2/version.py` & `pox-0.3.3/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #
 # Author: Mike McKerns (mmckerns @caltech and @uqfoundation)
-# Copyright (c) 2022 The Uncertainty Quantification Foundation.
+# Copyright (c) 2022-2023 The Uncertainty Quantification Foundation.
 # License: 3-clause BSD.  The full license text is available at:
 #  - https://github.com/uqfoundation/pox/blob/master/LICENSE
 
-__version__ = '0.3.2'
+__version__ = '0.3.3'
 __author__ = 'Mike McKerns'
 __contact__ = 'mmckerns@uqfoundation.org'
 
 
 def get_license_text(filepath):
     "open the LICENSE file and read the contents"
     try:
@@ -34,14 +34,21 @@
                 continue
             elif skip and line.startswith('    http'):
                 README += '\n' + line
             elif line.startswith('* '):
                 README += line.replace('* ','    - ',1)
             elif line.startswith('-'):
                 README += line.replace('-','=') + '\n'
+            elif line.startswith('!['): # image
+                alt,img = line.split('](',1)
+                if img.startswith('docs'): # relative path
+                    img = img.split('docs/source/',1)[-1] # make is in docs
+                README += '.. image:: ' + img.replace(')','')
+                README += '   :alt: ' + alt.replace('![','') + '\n'
+            #elif ')[http' in line: # alt text link (`text <http://url>`_)
             else:
                 README += line
                 skip = line.endswith(':\n')
         fh.close()
     except:
         README = ''
     return README
@@ -57,15 +64,15 @@
         license: the module's license contents
     """
     import os
     infofile = os.path.join(dirpath, '%s/__info__.py' % modulename)
     header = '''#!/usr/bin/env python
 #
 # Author: Mike McKerns (mmckerns @caltech and @uqfoundation)
-# Copyright (c) 2022 The Uncertainty Quantification Foundation.
+# Copyright (c) 2023 The Uncertainty Quantification Foundation.
 # License: 3-clause BSD.  The full license text is available at:
 #  - https://github.com/uqfoundation/%s/blob/master/LICENSE
 ''' % modulename #XXX: author and email are hardwired in the header
     doc = info.get('doc', None)
     version = info.get('version', None)
     author = info.get('author', None)
     license = info.get('license', None)
```

