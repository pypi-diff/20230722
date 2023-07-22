# Comparing `tmp/apkpatcher-cli-1.3.3.tar.gz` & `tmp/apkpatcher-cli-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkpatcher-cli-1.3.3.tar", last modified: Sat Jul 22 11:40:32 2023, max compression
+gzip compressed data, was "apkpatcher-cli-1.3.4.tar", last modified: Sat Jul 22 13:11:09 2023, max compression
```

## Comparing `apkpatcher-cli-1.3.3.tar` & `apkpatcher-cli-1.3.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 11:40:32.312381 apkpatcher-cli-1.3.3/
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)    18046 2023-07-21 09:54:40.000000 apkpatcher-cli-1.3.3/LICENSE
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 11:40:32.312381 apkpatcher-cli-1.3.3/PKG-INFO
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)     7475 2023-07-22 11:38:19.000000 apkpatcher-cli-1.3.3/README.md
--rwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)    47047 2023-07-22 11:39:59.000000 apkpatcher-cli-1.3.3/apkpatcher
-drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 11:40:32.312381 apkpatcher-cli-1.3.3/apkpatcher_cli.egg-info/
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 11:40:32.000000 apkpatcher-cli-1.3.3/apkpatcher_cli.egg-info/PKG-INFO
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      226 2023-07-22 11:40:32.000000 apkpatcher-cli-1.3.3/apkpatcher_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 11:40:32.000000 apkpatcher-cli-1.3.3/apkpatcher_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       17 2023-07-22 11:40:32.000000 apkpatcher-cli-1.3.3/apkpatcher_cli.egg-info/requires.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 11:40:32.000000 apkpatcher-cli-1.3.3/apkpatcher_cli.egg-info/top_level.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       38 2023-07-22 11:40:32.312381 apkpatcher-cli-1.3.3/setup.cfg
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      804 2023-07-22 11:39:43.000000 apkpatcher-cli-1.3.3/setup.py
+drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 13:11:09.500093 apkpatcher-cli-1.3.4/
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)    18046 2023-07-21 09:54:40.000000 apkpatcher-cli-1.3.4/LICENSE
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 13:11:09.500093 apkpatcher-cli-1.3.4/PKG-INFO
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)     7006 2023-07-22 13:05:52.000000 apkpatcher-cli-1.3.4/README.md
+-rwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)    47992 2023-07-22 13:10:29.000000 apkpatcher-cli-1.3.4/apkpatcher
+drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 13:11:09.500093 apkpatcher-cli-1.3.4/apkpatcher_cli.egg-info/
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 13:11:09.000000 apkpatcher-cli-1.3.4/apkpatcher_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      226 2023-07-22 13:11:09.000000 apkpatcher-cli-1.3.4/apkpatcher_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 13:11:09.000000 apkpatcher-cli-1.3.4/apkpatcher_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       29 2023-07-22 13:11:09.000000 apkpatcher-cli-1.3.4/apkpatcher_cli.egg-info/requires.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 13:11:09.000000 apkpatcher-cli-1.3.4/apkpatcher_cli.egg-info/top_level.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       38 2023-07-22 13:11:09.500093 apkpatcher-cli-1.3.4/setup.cfg
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      826 2023-07-22 13:10:33.000000 apkpatcher-cli-1.3.4/setup.py
```

### Comparing `apkpatcher-cli-1.3.3/LICENSE` & `apkpatcher-cli-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `apkpatcher-cli-1.3.3/PKG-INFO` & `apkpatcher-cli-1.3.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher-cli
-Version: 1.3.3
+Version: 1.3.4
 Summary: Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher
 Home-page: https://github.com/nitanmarcel/apkpatcher
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkpatcher-cli-1.3.3/README.md` & `apkpatcher-cli-1.3.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,57 @@
 ## APK Patcher
 
-This tool was developed mainly to automatically insert Frida Gadget inside APKs, but helps also in other common tasks while reversing Android apps.
+This tool was developed mainly to automatically insert Frida Gadget inside APKs but helps also in other common tasks while reversing Android apps.
 
 Frida Website: https://frida.re/
 
 Frida Github: https://github.com/frida/frida
 
 
 #### Features
 - Automatically insert Frida gadget library in APK, so you can use Frida without root - [Reference](https://frida.re/docs/gadget/)
-- Configure Frida Gadget to automatically load hooks javascript file, without requiring to use frida client
+- Configure Frida Gadget to automatically load hooks javascript file, without requiring the use of Frida client
 - Insert a network configuration in APK that allows the application to use User Certificate Authorities - [Reference](https://android-developers.googleblog.com/2016/07/changes-to-trusted-certificate.html)
-- Help during the tedious tasks of decompile, modify code, repackage, resign, zipalign
+- Help during the tedious tasks of decompiling, modify code, repackaging, resign, zipalign
 
 #### How To Install
 ##### Dependencies
-Starting with 1.2.0 only `java` is a required dependencies, with `frida` and `adb` as optional dependencies.
+Starting with 1.2.0 only `java` is a required dependency, with `Frida` and `adb` as optional dependencies.
 
-- java (required)
+- java (optional and will be automatically installed if it doesn't exist)
 - adb (optional to automatically detect target architecture)
 
 ##### Termux
 
  Termux has 2 extra dependencies.
 
  - custom apktool - https://github.com/rendiix/termux-apktool
-    - install the apktool for your arch then pass if to `apkpatcher` with `--apktool /data/data/com.termux/files/usr/bin/apktool.jar`
+    - install the apktool for your arch then pass it to `apkpatcher` with `--apktool /data/data/com.termux/files/usr/bin/apktool.jar`
  
  - custom zipalign version - https://github.com/rendiix/termux-zipalign
-    - it should will be automatically detected and used by `apkpatcher`
+    - it should be automatically detected and used by `apkpatcher`
   
 
 ##### APK Patcher Installation
 `pip install apkpatcher-cli`
 
-#### Termux
- Termux require a custom apktool jar file then used with the app by calling `apkpatcher` with `--apktool /path/to/apktool.jar` argument
- 
-
 #### How To Use It
 For all usages, the output file will be something like <apkname>_patched.apk.
 
-**Before using apkpatcher, make sure you have the latest version of apktool**
-- ##### Downloading Gadgets
-  Before using APK Patcher, download frida gadgets running the following command
-  ```
-  apkpatcher --update-gadgets
-  ```
-
 - ##### Bundles
   apkpatcher supports bundles out of the box by just passing the bundle path.
 
 - ##### Inserting Frida Gadget
-  In order to insert Frida library in APK, **enable USB debugging in your device and connect it in your PC**. APK Patcher will **identify your device** architecture and **insert the right gadget**.
   ```
-  apkpatcher -a base.apk
+  apkpatcher -a base.apk --arch device_architecture
   ```
 
-  If you can't connect the device in USB or if you want to select a **custom gadget**, see the *gadgets* folder and use the following syntax:
+  If you have adb installed and connected to your device you can ommit the `--arch` argument.
+
+  You can also install a custom gadget by specifying the path to it as:
   ```
   apkpatcher -a base.apk -g ~/Tools/apkpatcher/gadgets/12.5.9/frida-gadget-12.5.9-android-arm.so
   ```
 
   When you open the app, the Android screen will stay freezed. The frida gadget has started and is waiting for connection. Connect with the command `frida -U -n Gadget`
 
 - ##### Autoload Script
@@ -90,36 +80,36 @@
   ```
 
 - ##### Load a shared library instead of the frida gadget
   You may also load a custom shared library (e.g compiled with frida-deepfreeze-rs) instead of a frida gadget
   `apkpatcher -a base.apk --lib my_lib.so`
 
 - ##### Enable User Certificate Authorities
-  When analyzing android apps, you may want to intercept it's HTTPS traffic with some proxy like Burp Suite. Since Android 7 - Nougat, apps that the target API Level is 24 and above no longer trust in user-added CAs. In order to bypass this restriction, you can patch the APK to insert a network configuration. APK Patcher can do this automatically for you. Use the following command
+  When analyzing android apps, you may want to intercept it's HTTPS traffic with some proxy like Burp Suite. Since Android 7 - Nougat, apps that the target API Level is 24 and above no longer trust user-added CAs. In order to bypass this restriction, you can patch the APK to insert a network configuration. APK Patcher can do this automatically for you. Use the following command
 
   ```
   apkpatcher --enable-user-certificates --prevent-frida-gadget -a base.apk
   ```
   ~~
 
-  Note that we used the option `--prevent-frida-gadget`, so the frida gadget library is not inserted in application
+  Note that we used the option `--prevent-frida-gadget`, so the frida gadget library is not inserted in the application
 
   **Caution:** If the network_security_config.xml file already exists, apkpatcher will delete it, and this may cause some bug. APK Patcher will show you the original file content before deleting it.
 
 - ##### Force Extract Resources
   ~~APK Patcher will try the most it can to avoid extracting resource files, since this task may fail sometimes. So if you just want to insert frida gadget and the app already declares the usage of `android.permission.INTERNET`, apkpatcher will not extract AndroidManifest.xml and resource files. It will modify only some smali code.~~
   
-  As of 1.2.0 the tool will extract resources by default so the app can install: https://github.com/iBotPeaches/Apktool/issues/1626
+  As of 1.2.0 the tool will extract resources by default so the app can install on the device: https://github.com/iBotPeaches/Apktool/issues/1626
 
 - ##### Help during package modification
-  Every time you have to modify an APK, it is a tedious task to decompile, modify, repackage, sign (and generate a key if you don't have one) and zipalign it. APK Patcher will help you during this task. You can use the `--wait-before-repackage`, and APK Patcher will wait you make any change you want. Then you just instruct APK Patcher to continue, and it will automatically repack the APK, sign it with a random generated key and zipalign it. You can use this option with combination of other APK Patcher flags.
+  Every time you have to modify an APK, it is a tedious task to decompile, modify, repackage, sign (and generate a key if you don't have one), and zipalign it. APK Patcher will help you during this task. You can use the `--wait-before-repackage`, and APK Patcher will wait for you to make any change you want. Then you just instruct APK Patcher to continue, and it will automatically repack the APK, sign it with a randomly generated key, and zipalign it. You can use this option with a combination of other APK Patcher flags.
 
   - Just decompile and wait for me:
   ```
-  apkpatcher -a base.apk --prevent-frida-gadget --force-extract-resources -w
+  apkpatcher -a base.apk --prevent-frida-gadget -w
   ```
   The output will be something like the following:
   ```
   [*] Extracting base.apk (with resources) to /tmp/apkptmp/base
   [*] Some errors may occur while decoding resources that have framework dependencies
   [*] Apkpatcher is waiting for your OK to repackage the apk...
   [*] Are you ready? (y/N):
```

### Comparing `apkpatcher-cli-1.3.3/apkpatcher` & `apkpatcher-cli-1.3.4/apkpatcher`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import argparse
 import json
 import lzma
 import os
+import glob
 import shutil
 import signal
 import subprocess
 import sys
 import tempfile
 import time
 import xml.etree.ElementTree as ET
 import zipfile
 from pathlib import Path
 
 import requests
 from appdirs import user_cache_dir, user_data_dir
 
-__version__ = '1.3.3'
+import jdk
+
+__version__ = '1.3.4'
 
 APK_TOOL_VERSION = '2.8.0'
 APK_SIGNER_VERSION = '1.3.0'
+JAVA_JDK_VERSION = 17
 
 # noinspection SpellCheckingInspection
 
 
 class BColors:
     COLOR_BLUE = '\033[94m'
     COLOR_RED_BG = '\033[101m'
@@ -172,26 +176,26 @@
             os.makedirs(target_folder)
 
         downloaded_files = []
         for gadget in list_gadgets:
             gadget_file_path = os.path.join(target_folder, gadget['name'])
 
             if os.path.isfile(gadget_file_path.replace('.xz', '')):
-                print(f'{gadget["name"]} already exists. Skipping.')
+                self.print_info(f'{gadget["name"]} already exists. Skipping.')
             else:
                 self.download_file(gadget['url'], gadget_file_path)
                 downloaded_files.append(gadget_file_path)
 
-        print('Extracting downloaded files...')
+        self.print_info('Extracting downloaded files...')
 
         for downloaded_file in downloaded_files:
             with lzma.open(downloaded_file) as f, open(downloaded_file.replace(".xz", ""), "wb") as outfile:
                 outfile.write(f.read())
 
-        print('Done! Gadgets were updated')
+        self.print_done('Done! Gadgets were updated')
 
         return True
 
     def download_file(self, url, target_path):
         file_name = target_path.split('/')[-1]
         response = requests.get(url, stream=True)
         response.raise_for_status()
@@ -219,15 +223,38 @@
                         sys.stdout.flush()
 
                     f.write(chunk)
 
         if self.VERBOSITY >= self.VERBOSITY_HIGH:
             sys.stdout.write('\n')
 
+    def find_java(self):
+        base_path = self.dependencies_manager.java
+        if not os.path.exists(base_path):
+            return None
+        else:
+            if os.path.isfile(base_path):
+                return base_path
+            else:
+                pattern = os.path.join(base_path, "jdk-17*", "bin", "java")
+                java_paths = glob.glob(pattern)
+                if java_paths:
+                    return java_paths[-0]
+            return None
+        
+
+
     def check_and_download_tools(self, apktool_path=None):
+        java_path = self.find_java()
+        if not java_path:
+            self.print_info('Downloading java. This might take a while...')
+            jdk.install(17, path=self.dependencies_manager.java)
+        java_path = self.find_java()
+        self.dependencies_manager.add_depedency('java', java_path)
+
         if not apktool_path:
             apktool_path = os.path.join(
                 self.data_dir, 'apktool_{0}.jar'.format(APK_TOOL_VERSION))
         if not os.path.isfile(apktool_path):
             old_apktool = Path(self.data_dir).glob('apktool*.jar')
             for i in old_apktool:
                 self.print_info(
@@ -566,15 +593,15 @@
         self.print_info(
             'Frida loader was injected in the entrypoint smali file!')
 
         return True
 
     def set_extract_native_libs(self, manifest_path):
         if not os.path.isfile(manifest_path):
-            print("Couldn't find the Manifest file. Something is wrong with the apk!")
+            self.print_warn("Couldn't find the Manifest file. Something is wrong with the apk!")
             return
 
         tree = ET.parse(manifest_path)
         root = tree.getroot()
 
         namespaces = {'android': 'http://schemas.android.com/apk/res/android'}
 
@@ -589,15 +616,15 @@
                 application_node.set('{%s}extractNativeLibs' %
                                      namespaces['android'], 'true')
                 tree.write(manifest_path, encoding='utf-8',
                            xml_declaration=True)
 
     def fix_target_sdk(self, apk_path, manifest_path):
         if not os.path.isfile(manifest_path):
-            print("Couldn't find the Manifest file. Something is wrong with the apk!")
+            self.print_warn("Couldn't find the Manifest file. Something is wrong with the apk!")
             return
 
     def get_arch_by_gadget(self, gadget_path):
         if 'arm' in gadget_path and '64' not in gadget_path:
             return self.ARCH_ARM
 
         elif 'arm64' in gadget_path:
@@ -1080,37 +1107,38 @@
 
     if args.version:
         patcher.set_verbosity(patcher.VERBOSITY_HIGH)
         patcher.print_done('apkpatcher {0}'.format(__version__))
         return 1
 
     if not dependencies_manager.add_depedency('java'):
-        patcher.print_warn('java is not installed')
-        return 1
+        java_path = os.path.join(patcher.data_dir, 'jdk')
+        dependencies_manager.add_depedency('java', path=java_path)
 
     dependencies_manager.add_depedency('frida', required=False)
     dependencies_manager.add_depedency('adb', required=False)
 
     # Fix on termux
     dependencies_manager.add_depedency('zipalign', required=False)
 
-    if not dependencies_manager.has_satisfied_required_dependencies():
-        patcher.print_warn('One or more dependencies were not satisfied.')
-        return
-
     patcher.dependencies_manager = dependencies_manager
 
     if args.verbosity:
         patcher.set_verbosity(int(args.verbosity))
     else:
         patcher.set_verbosity(patcher.VERBOSITY_HIGH)
 
+    patcher.check_and_download_tools(apktool_path=args.apktool)
+
+    if not dependencies_manager.has_satisfied_required_dependencies():
+        patcher.print_warn('One or more dependencies were not satisfied.')
+        return
+    
     if args.update_gadgets:
         patcher.update_apkpatcher_gadgets()
-
         return 0
 
     if not args.apk:
         parser.print_help()
 
         return 1
 
@@ -1130,16 +1158,14 @@
             gadget_to_use = patcher.get_recommended_gadget(abi=args.arch)
 
         if gadget_to_use is None or not os.path.isfile(gadget_to_use):
             patcher.print_warn('Could not identify the gadget!')
 
             return 1
 
-    patcher.check_and_download_tools(apktool_path=args.apktool)
-
     # THE APK PATCHING STARTS HERE
 
     apk_file_path = args.apk
     apk_file_name = os.path.basename(apk_file_path)
     if apk_file_path.endswith('.xapk'):
         patcher.is_bundle = True
         apk_file_path = patcher.extract_bundle(apk_file_path)
```

### Comparing `apkpatcher-cli-1.3.3/apkpatcher_cli.egg-info/PKG-INFO` & `apkpatcher-cli-1.3.4/apkpatcher_cli.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher-cli
-Version: 1.3.3
+Version: 1.3.4
 Summary: Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher
 Home-page: https://github.com/nitanmarcel/apkpatcher
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkpatcher-cli-1.3.3/setup.py` & `apkpatcher-cli-1.3.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup
 
 setup(
    name='apkpatcher-cli',
-   version='1.3.3',
+   version='1.3.4',
    description='Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher',
    author='Marcel Alexandru Nitan',
    author_email='nitan.marcel@gmail.com',
    url='https://github.com/nitanmarcel/apkpatcher',
    keywords=['FRIDA', 'APK'],
    scripts=['apkpatcher'],
    install_requires=[
        'requests',
-       'appdirs'
+       'appdirs',
+       'install-jdk'
    ],
    classifiers=[
     'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
```

