# Comparing `tmp/apkpatcher-cli-1.3.1.tar.gz` & `tmp/apkpatcher-cli-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkpatcher-cli-1.3.1.tar", last modified: Sat Jul 22 10:20:49 2023, max compression
+gzip compressed data, was "apkpatcher-cli-1.3.2.tar", last modified: Sat Jul 22 10:42:31 2023, max compression
```

## Comparing `apkpatcher-cli-1.3.1.tar` & `apkpatcher-cli-1.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 10:20:49.006232 apkpatcher-cli-1.3.1/
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)    18046 2023-07-21 09:54:40.000000 apkpatcher-cli-1.3.1/LICENSE
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 10:20:49.006232 apkpatcher-cli-1.3.1/PKG-INFO
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)     6930 2023-07-22 10:11:16.000000 apkpatcher-cli-1.3.1/README.md
--rwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)    46479 2023-07-22 10:20:08.000000 apkpatcher-cli-1.3.1/apkpatcher
-drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 10:20:49.006232 apkpatcher-cli-1.3.1/apkpatcher_cli.egg-info/
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 10:20:48.000000 apkpatcher-cli-1.3.1/apkpatcher_cli.egg-info/PKG-INFO
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      226 2023-07-22 10:20:48.000000 apkpatcher-cli-1.3.1/apkpatcher_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 10:20:48.000000 apkpatcher-cli-1.3.1/apkpatcher_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       28 2023-07-22 10:20:48.000000 apkpatcher-cli-1.3.1/apkpatcher_cli.egg-info/requires.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 10:20:48.000000 apkpatcher-cli-1.3.1/apkpatcher_cli.egg-info/top_level.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       38 2023-07-22 10:20:49.006232 apkpatcher-cli-1.3.1/setup.cfg
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      825 2023-07-22 10:20:10.000000 apkpatcher-cli-1.3.1/setup.py
+drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 10:42:31.022981 apkpatcher-cli-1.3.2/
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)    18046 2023-07-21 09:54:40.000000 apkpatcher-cli-1.3.2/LICENSE
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 10:42:31.022981 apkpatcher-cli-1.3.2/PKG-INFO
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)     6930 2023-07-22 10:11:16.000000 apkpatcher-cli-1.3.2/README.md
+-rwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)    46479 2023-07-22 10:41:51.000000 apkpatcher-cli-1.3.2/apkpatcher
+drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 10:42:31.022981 apkpatcher-cli-1.3.2/apkpatcher_cli.egg-info/
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 10:42:30.000000 apkpatcher-cli-1.3.2/apkpatcher_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      226 2023-07-22 10:42:30.000000 apkpatcher-cli-1.3.2/apkpatcher_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 10:42:30.000000 apkpatcher-cli-1.3.2/apkpatcher_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       17 2023-07-22 10:42:30.000000 apkpatcher-cli-1.3.2/apkpatcher_cli.egg-info/requires.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 10:42:30.000000 apkpatcher-cli-1.3.2/apkpatcher_cli.egg-info/top_level.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       38 2023-07-22 10:42:31.022981 apkpatcher-cli-1.3.2/setup.cfg
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      804 2023-07-22 10:41:54.000000 apkpatcher-cli-1.3.2/setup.py
```

### Comparing `apkpatcher-cli-1.3.1/LICENSE` & `apkpatcher-cli-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apkpatcher-cli-1.3.1/PKG-INFO` & `apkpatcher-cli-1.3.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher-cli
-Version: 1.3.1
+Version: 1.3.2
 Summary: Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher
 Home-page: https://github.com/nitanmarcel/apkpatcher
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkpatcher-cli-1.3.1/README.md` & `apkpatcher-cli-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `apkpatcher-cli-1.3.1/apkpatcher` & `apkpatcher-cli-1.3.2/apkpatcher`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import xml.etree.ElementTree as ET
 import zipfile
 from pathlib import Path
 
 import requests
 from appdirs import user_cache_dir, user_data_dir
 
-__version__ = '1.3.1'
+__version__ = '1.3.2'
 
 APK_TOOL_VERSION = '2.8.0'
 APK_SIGNER_VERSION = '1.3.0'
 
 # noinspection SpellCheckingInspection
```

### Comparing `apkpatcher-cli-1.3.1/apkpatcher_cli.egg-info/PKG-INFO` & `apkpatcher-cli-1.3.2/apkpatcher_cli.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher-cli
-Version: 1.3.1
+Version: 1.3.2
 Summary: Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher
 Home-page: https://github.com/nitanmarcel/apkpatcher
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkpatcher-cli-1.3.1/setup.py` & `apkpatcher-cli-1.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from setuptools import setup
 
 setup(
    name='apkpatcher-cli',
-   version='1.3.1',
+   version='1.3.2',
    description='Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher',
    author='Marcel Alexandru Nitan',
    author_email='nitan.marcel@gmail.com',
    url='https://github.com/nitanmarcel/apkpatcher',
    keywords=['FRIDA', 'APK'],
    scripts=['apkpatcher'],
    install_requires=[
        'requests',
-       'appdirs',
-       'androguard'
+       'appdirs'
    ],
    classifiers=[
     'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
```

