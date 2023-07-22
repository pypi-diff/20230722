# Comparing `tmp/ubox-0.0.1.tar.gz` & `tmp/ubox-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubox-0.0.1.tar", last modified: Sat Jul 22 12:53:54 2023, max compression
+gzip compressed data, was "ubox-0.0.1.2.tar", last modified: Sat Jul 22 13:03:45 2023, max compression
```

## Comparing `ubox-0.0.1.tar` & `ubox-0.0.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-22 12:53:54.533424 ubox-0.0.1/
--rw-r--r--   0 tek        (501) staff       (20)     1060 2023-07-22 12:39:24.000000 ubox-0.0.1/LICENSE
--rw-r--r--   0 tek        (501) staff       (20)      534 2023-07-22 12:53:54.533209 ubox-0.0.1/PKG-INFO
--rw-r--r--   0 tek        (501) staff       (20)       25 2023-07-22 12:44:39.000000 ubox-0.0.1/README.md
--rw-r--r--   0 tek        (501) staff       (20)       38 2023-07-22 12:53:54.533493 ubox-0.0.1/setup.cfg
--rw-r--r--   0 tek        (501) staff       (20)     1216 2023-07-22 12:53:36.000000 ubox-0.0.1/setup.py
-drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-22 12:53:54.531920 ubox-0.0.1/ubox/
--rw-r--r--   0 tek        (501) staff       (20)      107 2023-07-22 12:47:22.000000 ubox-0.0.1/ubox/__init__.py
--rw-r--r--   0 tek        (501) staff       (20)     1643 2023-07-22 12:50:59.000000 ubox-0.0.1/ubox/crypto.py
--rw-r--r--   0 tek        (501) staff       (20)      593 2023-07-22 12:50:47.000000 ubox-0.0.1/ubox/random.py
-drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-22 12:53:54.532931 ubox-0.0.1/ubox.egg-info/
--rw-r--r--   0 tek        (501) staff       (20)      534 2023-07-22 12:53:54.000000 ubox-0.0.1/ubox.egg-info/PKG-INFO
--rw-r--r--   0 tek        (501) staff       (20)      185 2023-07-22 12:53:54.000000 ubox-0.0.1/ubox.egg-info/SOURCES.txt
--rw-r--r--   0 tek        (501) staff       (20)        1 2023-07-22 12:53:54.000000 ubox-0.0.1/ubox.egg-info/dependency_links.txt
--rw-r--r--   0 tek        (501) staff       (20)        5 2023-07-22 12:53:54.000000 ubox-0.0.1/ubox.egg-info/top_level.txt
+drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-22 13:03:45.529380 ubox-0.0.1.2/
+-rw-r--r--   0 tek        (501) staff       (20)     1060 2023-07-22 12:39:24.000000 ubox-0.0.1.2/LICENSE
+-rw-r--r--   0 tek        (501) staff       (20)      536 2023-07-22 13:03:45.529172 ubox-0.0.1.2/PKG-INFO
+-rw-r--r--   0 tek        (501) staff       (20)       25 2023-07-22 12:44:39.000000 ubox-0.0.1.2/README.md
+-rw-r--r--   0 tek        (501) staff       (20)       38 2023-07-22 13:03:45.529450 ubox-0.0.1.2/setup.cfg
+-rw-r--r--   0 tek        (501) staff       (20)     1218 2023-07-22 13:03:33.000000 ubox-0.0.1.2/setup.py
+drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-22 13:03:45.527891 ubox-0.0.1.2/ubox/
+-rw-r--r--   0 tek        (501) staff       (20)      169 2023-07-22 13:02:22.000000 ubox-0.0.1.2/ubox/__init__.py
+-rw-r--r--   0 tek        (501) staff       (20)     1643 2023-07-22 12:50:59.000000 ubox-0.0.1.2/ubox/crypto.py
+-rw-r--r--   0 tek        (501) staff       (20)      793 2023-07-22 13:03:05.000000 ubox-0.0.1.2/ubox/identifiers.py
+-rw-r--r--   0 tek        (501) staff       (20)      593 2023-07-22 12:50:47.000000 ubox-0.0.1.2/ubox/random.py
+drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-22 13:03:45.528867 ubox-0.0.1.2/ubox.egg-info/
+-rw-r--r--   0 tek        (501) staff       (20)      536 2023-07-22 13:03:45.000000 ubox-0.0.1.2/ubox.egg-info/PKG-INFO
+-rw-r--r--   0 tek        (501) staff       (20)      205 2023-07-22 13:03:45.000000 ubox-0.0.1.2/ubox.egg-info/SOURCES.txt
+-rw-r--r--   0 tek        (501) staff       (20)        1 2023-07-22 13:03:45.000000 ubox-0.0.1.2/ubox.egg-info/dependency_links.txt
+-rw-r--r--   0 tek        (501) staff       (20)        5 2023-07-22 13:03:45.000000 ubox-0.0.1.2/ubox.egg-info/top_level.txt
```

### Comparing `ubox-0.0.1/LICENSE` & `ubox-0.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ubox-0.0.1/PKG-INFO` & `ubox-0.0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubox
-Version: 0.0.1
+Version: 0.0.1.2
 Summary: Python Utils Box for Botting/Spoofing (encryption, random, etc)
 Author: Tekky
 Author-email: <support@g4f.ai>
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `ubox-0.0.1/setup.py` & `ubox-0.0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.1.2'
 DESCRIPTION = 'Python Utils Box for Botting/Spoofing (encryption, random, etc)'
 
 # Setting up
 setup(
     name="ubox",
     version=VERSION,
     author="Tekky",
```

### Comparing `ubox-0.0.1/ubox/crypto.py` & `ubox-0.0.1.2/ubox/crypto.py`

 * *Files identical despite different names*

### Comparing `ubox-0.0.1/ubox/random.py` & `ubox-0.0.1.2/ubox/random.py`

 * *Files identical despite different names*

### Comparing `ubox-0.0.1/ubox.egg-info/PKG-INFO` & `ubox-0.0.1.2/ubox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubox
-Version: 0.0.1
+Version: 0.0.1.2
 Summary: Python Utils Box for Botting/Spoofing (encryption, random, etc)
 Author: Tekky
 Author-email: <support@g4f.ai>
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

