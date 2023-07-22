# Comparing `tmp/apkpatcher-cli-1.3.5.tar.gz` & `tmp/apkpatcher-cli-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkpatcher-cli-1.3.5.tar", last modified: Sat Jul 22 14:05:33 2023, max compression
+gzip compressed data, was "apkpatcher-cli-1.3.6.tar", last modified: Sat Jul 22 14:19:56 2023, max compression
```

## Comparing `apkpatcher-cli-1.3.5.tar` & `apkpatcher-cli-1.3.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 14:05:33.472257 apkpatcher-cli-1.3.5/
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)    18046 2023-07-21 09:54:40.000000 apkpatcher-cli-1.3.5/LICENSE
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 14:05:33.472257 apkpatcher-cli-1.3.5/PKG-INFO
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)     7006 2023-07-22 13:05:52.000000 apkpatcher-cli-1.3.5/README.md
--rwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)    47996 2023-07-22 14:05:04.000000 apkpatcher-cli-1.3.5/apkpatcher
-drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 14:05:33.472257 apkpatcher-cli-1.3.5/apkpatcher_cli.egg-info/
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 14:05:33.000000 apkpatcher-cli-1.3.5/apkpatcher_cli.egg-info/PKG-INFO
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      226 2023-07-22 14:05:33.000000 apkpatcher-cli-1.3.5/apkpatcher_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 14:05:33.000000 apkpatcher-cli-1.3.5/apkpatcher_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       29 2023-07-22 14:05:33.000000 apkpatcher-cli-1.3.5/apkpatcher_cli.egg-info/requires.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 14:05:33.000000 apkpatcher-cli-1.3.5/apkpatcher_cli.egg-info/top_level.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       38 2023-07-22 14:05:33.472257 apkpatcher-cli-1.3.5/setup.cfg
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      826 2023-07-22 14:05:18.000000 apkpatcher-cli-1.3.5/setup.py
+drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 14:19:56.395604 apkpatcher-cli-1.3.6/
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)    18046 2023-07-21 09:54:40.000000 apkpatcher-cli-1.3.6/LICENSE
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 14:19:56.395604 apkpatcher-cli-1.3.6/PKG-INFO
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)     7006 2023-07-22 13:05:52.000000 apkpatcher-cli-1.3.6/README.md
+-rwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)    48000 2023-07-22 14:19:35.000000 apkpatcher-cli-1.3.6/apkpatcher
+drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 14:19:56.395604 apkpatcher-cli-1.3.6/apkpatcher_cli.egg-info/
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 14:19:56.000000 apkpatcher-cli-1.3.6/apkpatcher_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      226 2023-07-22 14:19:56.000000 apkpatcher-cli-1.3.6/apkpatcher_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 14:19:56.000000 apkpatcher-cli-1.3.6/apkpatcher_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       29 2023-07-22 14:19:56.000000 apkpatcher-cli-1.3.6/apkpatcher_cli.egg-info/requires.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        4 2023-07-22 14:19:56.000000 apkpatcher-cli-1.3.6/apkpatcher_cli.egg-info/top_level.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       38 2023-07-22 14:19:56.395604 apkpatcher-cli-1.3.6/setup.cfg
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      826 2023-07-22 14:19:38.000000 apkpatcher-cli-1.3.6/setup.py
```

### Comparing `apkpatcher-cli-1.3.5/LICENSE` & `apkpatcher-cli-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `apkpatcher-cli-1.3.5/PKG-INFO` & `apkpatcher-cli-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher-cli
-Version: 1.3.5
+Version: 1.3.6
 Summary: Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher
 Home-page: https://github.com/nitanmarcel/apkpatcher
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkpatcher-cli-1.3.5/README.md` & `apkpatcher-cli-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `apkpatcher-cli-1.3.5/apkpatcher` & `apkpatcher-cli-1.3.6/apkpatcher`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 
 import requests
 from appdirs import user_cache_dir, user_data_dir
 
 import jdk
 
-__version__ = '1.3.5'
+__version__ = '1.3.6'
 
 APK_TOOL_VERSION = '2.8.0'
 APK_SIGNER_VERSION = '1.3.0'
 JAVA_JDK_VERSION = 17
 
 # noinspection SpellCheckingInspection
 
@@ -307,17 +307,17 @@
             abi = subprocess.check_output(
                 ['adb', 'shell', 'getprop ro.product.cpu.abi']).decode('utf-8').strip()
         elif not abi:
             self.print_warn(
                 'Can\'t automatically detect device architecture. Use the --arch argument instead. (missing adb command)')
             sys.exit(1)
         else:
-            if abi not in ['arm64-v8a', 'arm64', 'x86', 'x86_64']:
+            if abi not in ['armeabi-v7a', 'arm64', 'x86', 'x86_64']:
                 self.print_warn(
-                    'Architecture {0} if not one of the supported architectures arm64-v8a, arm64, x86, x86_64'.format(abi))
+                    'Architecture {0} if not one of the supported architectures armeabi-v7a, arm64, x86, x86_64'.format(abi))
                 sys.exit(0)
 
         self.print_info('The abi is {0}'.format(abi))
 
         frida_version = self.get_frida_version()
         gadgets_folder = os.path.join(self.data_dir, 'gadgets')
         target_folder = os.path.join(gadgets_folder, frida_version)
```

### Comparing `apkpatcher-cli-1.3.5/apkpatcher_cli.egg-info/PKG-INFO` & `apkpatcher-cli-1.3.6/apkpatcher_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher-cli
-Version: 1.3.5
+Version: 1.3.6
 Summary: Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher
 Home-page: https://github.com/nitanmarcel/apkpatcher
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkpatcher-cli-1.3.5/setup.py` & `apkpatcher-cli-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
    name='apkpatcher-cli',
-   version='1.3.5',
+   version='1.3.6',
    description='Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher',
    author='Marcel Alexandru Nitan',
    author_email='nitan.marcel@gmail.com',
    url='https://github.com/nitanmarcel/apkpatcher',
    keywords=['FRIDA', 'APK'],
    scripts=['apkpatcher'],
    install_requires=[
```

