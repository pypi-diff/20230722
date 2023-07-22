# Comparing `tmp/apkpatcher-cli-1.3.4.tar.gz` & `tmp/apkpatcher-cli-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkpatcher-cli-1.3.4.tar", last modified: Sat Jul 22 13:11:09 2023, max compression
+gzip compressed data, was "apkpatcher-cli-1.3.5.tar", last modified: Sat Jul 22 14:05:33 2023, max compression
```

## Comparing `apkpatcher-cli-1.3.4.tar` & `apkpatcher-cli-1.3.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 13:11:09.500093 apkpatcher-cli-1.3.4/
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)    18046 2023-07-21 09:54:40.000000 apkpatcher-cli-1.3.4/LICENSE
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 13:11:09.500093 apkpatcher-cli-1.3.4/PKG-INFO
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)     7006 2023-07-22 13:05:52.000000 apkpatcher-cli-1.3.4/README.md
--rwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)    47992 2023-07-22 13:10:29.000000 apkpatcher-cli-1.3.4/apkpatcher
-drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 13:11:09.500093 apkpatcher-cli-1.3.4/apkpatcher_cli.egg-info/
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 13:11:09.000000 apkpatcher-cli-1.3.4/apkpatcher_cli.egg-info/PKG-INFO
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      226 2023-07-22 13:11:09.000000 apkpatcher-cli-1.3.4/apkpatcher_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 13:11:09.000000 apkpatcher-cli-1.3.4/apkpatcher_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       29 2023-07-22 13:11:09.000000 apkpatcher-cli-1.3.4/apkpatcher_cli.egg-info/requires.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 13:11:09.000000 apkpatcher-cli-1.3.4/apkpatcher_cli.egg-info/top_level.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       38 2023-07-22 13:11:09.500093 apkpatcher-cli-1.3.4/setup.cfg
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      826 2023-07-22 13:10:33.000000 apkpatcher-cli-1.3.4/setup.py
+drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 14:05:33.472257 apkpatcher-cli-1.3.5/
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)    18046 2023-07-21 09:54:40.000000 apkpatcher-cli-1.3.5/LICENSE
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 14:05:33.472257 apkpatcher-cli-1.3.5/PKG-INFO
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)     7006 2023-07-22 13:05:52.000000 apkpatcher-cli-1.3.5/README.md
+-rwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)    47996 2023-07-22 14:05:04.000000 apkpatcher-cli-1.3.5/apkpatcher
+drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 14:05:33.472257 apkpatcher-cli-1.3.5/apkpatcher_cli.egg-info/
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 14:05:33.000000 apkpatcher-cli-1.3.5/apkpatcher_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      226 2023-07-22 14:05:33.000000 apkpatcher-cli-1.3.5/apkpatcher_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 14:05:33.000000 apkpatcher-cli-1.3.5/apkpatcher_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       29 2023-07-22 14:05:33.000000 apkpatcher-cli-1.3.5/apkpatcher_cli.egg-info/requires.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 14:05:33.000000 apkpatcher-cli-1.3.5/apkpatcher_cli.egg-info/top_level.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       38 2023-07-22 14:05:33.472257 apkpatcher-cli-1.3.5/setup.cfg
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      826 2023-07-22 14:05:18.000000 apkpatcher-cli-1.3.5/setup.py
```

### Comparing `apkpatcher-cli-1.3.4/LICENSE` & `apkpatcher-cli-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `apkpatcher-cli-1.3.4/PKG-INFO` & `apkpatcher-cli-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher-cli
-Version: 1.3.4
+Version: 1.3.5
 Summary: Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher
 Home-page: https://github.com/nitanmarcel/apkpatcher
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkpatcher-cli-1.3.4/README.md` & `apkpatcher-cli-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `apkpatcher-cli-1.3.4/apkpatcher` & `apkpatcher-cli-1.3.5/apkpatcher`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 
 import requests
 from appdirs import user_cache_dir, user_data_dir
 
 import jdk
 
-__version__ = '1.3.4'
+__version__ = '1.3.5'
 
 APK_TOOL_VERSION = '2.8.0'
 APK_SIGNER_VERSION = '1.3.0'
 JAVA_JDK_VERSION = 17
 
 # noinspection SpellCheckingInspection
 
@@ -282,15 +282,15 @@
             self.print_info('Trying to identify the right frida-gadget...')
             self.print_info('Waiting for device...')
             os.system('adb wait-for-device')
             abi = subprocess.check_output(
                 ['adb', 'shell', 'getprop ro.product.cpu.abi']).decode('utf-8').strip()
         if abi not in ['armeabi-v7a', 'arm64', 'x86', 'x86_64']:
             self.print_warn(
-                'Architecture {0} if not one of the supported architectures arm64-v8a, arm64, x86, x86_64'.format(abi))
+                'Architecture {0} if not one of the supported architectures armeabi-v7a, arm64, x86, x86_64'.format(abi))
             sys.exit(0)
         if abi in ['armeabi-v7a']:
             return self.ARCH_ARM
         if abi in ['arm64']:
             return self.ARCH_ARM64
         if abi in ['x86']:
             return self.ARCH_X86
@@ -1057,15 +1057,15 @@
     patcher = Patcher()
 
     parser = argparse.ArgumentParser()
     parser.add_argument(
         '-a', '--apk', help='Specify the apk you want to patch')
     parser.add_argument('-g', '--gadget', help='Specify the frida-gadget file')
     parser.add_argument(
-        '--arch', help='Force architecture to inject frida gadget for. Supported arches: arm64-v8a, arm64, x86, x86_64')
+        '--arch', help='Force architecture to inject frida gadget for. Supported arches: armeabi-v7a, arm64, x86, x86_64')
     parser.add_argument('--autoload-script', help='Auto load script')
     parser.add_argument("--codeshare", help='Auto load script from codeshare')
     parser.add_argument('-v', '--verbosity',
                         help='Verbosity level (0 to 3). Default is 3')
     parser.add_argument('--update-gadgets',
                         help='Update frida-gadgets', action='store_true')
     parser.add_argument('--use-aapt2', help='Use aapt2 with apktool',
```

### Comparing `apkpatcher-cli-1.3.4/apkpatcher_cli.egg-info/PKG-INFO` & `apkpatcher-cli-1.3.5/apkpatcher_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher-cli
-Version: 1.3.4
+Version: 1.3.5
 Summary: Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher
 Home-page: https://github.com/nitanmarcel/apkpatcher
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkpatcher-cli-1.3.4/setup.py` & `apkpatcher-cli-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
    name='apkpatcher-cli',
-   version='1.3.4',
+   version='1.3.5',
    description='Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher',
    author='Marcel Alexandru Nitan',
    author_email='nitan.marcel@gmail.com',
    url='https://github.com/nitanmarcel/apkpatcher',
    keywords=['FRIDA', 'APK'],
    scripts=['apkpatcher'],
    install_requires=[
```

