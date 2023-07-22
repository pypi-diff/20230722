# Comparing `tmp/apkpatcher-cli-1.1.0.tar.gz` & `tmp/apkpatcher-cli-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkpatcher-cli-1.1.0.tar", last modified: Fri Jul 21 15:58:50 2023, max compression
+gzip compressed data, was "apkpatcher-cli-1.2.0.tar", last modified: Sat Jul 22 00:43:04 2023, max compression
```

## Comparing `apkpatcher-cli-1.1.0.tar` & `apkpatcher-cli-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-21 15:58:50.211125 apkpatcher-cli-1.1.0/
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)    18046 2023-07-21 09:54:40.000000 apkpatcher-cli-1.1.0/LICENSE
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-21 15:58:50.211125 apkpatcher-cli-1.1.0/PKG-INFO
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)     7642 2023-07-21 15:48:01.000000 apkpatcher-cli-1.1.0/README.md
--rwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)    42638 2023-07-21 15:57:24.000000 apkpatcher-cli-1.1.0/apkpatcher
-drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-21 15:58:50.211125 apkpatcher-cli-1.1.0/apkpatcher_cli.egg-info/
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-21 15:58:50.000000 apkpatcher-cli-1.1.0/apkpatcher_cli.egg-info/PKG-INFO
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      226 2023-07-21 15:58:50.000000 apkpatcher-cli-1.1.0/apkpatcher_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-21 15:58:50.000000 apkpatcher-cli-1.1.0/apkpatcher_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       17 2023-07-21 15:58:50.000000 apkpatcher-cli-1.1.0/apkpatcher_cli.egg-info/requires.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-21 15:58:50.000000 apkpatcher-cli-1.1.0/apkpatcher_cli.egg-info/top_level.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       38 2023-07-21 15:58:50.211125 apkpatcher-cli-1.1.0/setup.cfg
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      804 2023-07-21 15:57:10.000000 apkpatcher-cli-1.1.0/setup.py
+drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 00:43:04.921554 apkpatcher-cli-1.2.0/
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)    18046 2023-07-21 09:54:40.000000 apkpatcher-cli-1.2.0/LICENSE
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 00:43:04.921554 apkpatcher-cli-1.2.0/PKG-INFO
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)     7059 2023-07-21 22:59:45.000000 apkpatcher-cli-1.2.0/README.md
+-rwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)    44789 2023-07-22 00:37:29.000000 apkpatcher-cli-1.2.0/apkpatcher
+drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 00:43:04.921554 apkpatcher-cli-1.2.0/apkpatcher_cli.egg-info/
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 00:43:04.000000 apkpatcher-cli-1.2.0/apkpatcher_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      226 2023-07-22 00:43:04.000000 apkpatcher-cli-1.2.0/apkpatcher_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 00:43:04.000000 apkpatcher-cli-1.2.0/apkpatcher_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       28 2023-07-22 00:43:04.000000 apkpatcher-cli-1.2.0/apkpatcher_cli.egg-info/requires.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 00:43:04.000000 apkpatcher-cli-1.2.0/apkpatcher_cli.egg-info/top_level.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       38 2023-07-22 00:43:04.921554 apkpatcher-cli-1.2.0/setup.cfg
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      825 2023-07-22 00:42:38.000000 apkpatcher-cli-1.2.0/setup.py
```

### Comparing `apkpatcher-cli-1.1.0/LICENSE` & `apkpatcher-cli-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apkpatcher-cli-1.1.0/PKG-INFO` & `apkpatcher-cli-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher-cli
-Version: 1.1.0
+Version: 1.2.0
 Summary: Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher
 Home-page: https://github.com/nitanmarcel/apkpatcher
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkpatcher-cli-1.1.0/README.md` & `apkpatcher-cli-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,32 +11,20 @@
 - Automatically insert Frida gadget library in APK, so you can use Frida without root - [Reference](https://frida.re/docs/gadget/)
 - Configure Frida Gadget to automatically load hooks javascript file, without requiring to use frida client
 - Insert a network configuration in APK that allows the application to use User Certificate Authorities - [Reference](https://android-developers.googleblog.com/2016/07/changes-to-trusted-certificate.html)
 - Help during the tedious tasks of decompile, modify code, repackage, resign, zipalign
 
 #### How To Install
 ##### Dependencies
-The only Python dependency is `requests`, that is used to parse Github API in order to download Frida Gadgets.
+Starting with 1.2.0 only `java` is a required dependencies, with `frida` and `adb` as optional dependencies.
 
-But in order to make the script work properly, some other tools are required.
 
-Make sure the following tools are **installed** and **properly configured in your PATH** environment variable:
-
-- frida and frida-tools: `pip3 install frida frida-tools`
-- apktool - https://ibotpeaches.github.io/Apktool/install/
-- unxz
-- aapt
-- zipalign
-- adb
-- keytool
-- jarsigner
-
-If you have Android Studio installed, you will find aapt, zipalign and adb inside `~/Android/Sdk/build-tools/` or `~/Android/Sdk/build-tools/platform-tools/`
-
-A lot of tools used by APK Patcher require Java, so I suppose you will have it installed. Both `jarsigner` and `keytool` will probably come with your java installation. In my case I can find both tools in `/usr/lib/jvm/default/bin/` 
+- java (required)
+- frida and frida-tools: `pip3 install frida frida-tools` (optional to install frida gadget/scripts into the target application)
+- adb (optional to automatically detect target architecture)
 
 ##### APK Patcher Installation
 `pip install apkpatcher-cli`
 
 #### How To Use It
 For all usages, the output file will be something like <apkname>_patched.apk.
 
@@ -94,26 +82,24 @@
 
 - ##### Enable User Certificate Authorities
   When analyzing android apps, you may want to intercept it's HTTPS traffic with some proxy like Burp Suite. Since Android 7 - Nougat, apps that the target API Level is 24 and above no longer trust in user-added CAs. In order to bypass this restriction, you can patch the APK to insert a network configuration. APK Patcher can do this automatically for you. Use the following command
 
   ```
   apkpatcher --enable-user-certificates --prevent-frida-gadget -a base.apk
   ```
+  ~~
 
   Note that we used the option `--prevent-frida-gadget`, so the frida gadget library is not inserted in application
 
   **Caution:** If the network_security_config.xml file already exists, apkpatcher will delete it, and this may cause some bug. APK Patcher will show you the original file content before deleting it.
 
 - ##### Force Extract Resources
-  APK Patcher will try the most it can to avoid extracting resource files, since this task may fail sometimes. So if you just want to insert frida gadget and the app already declares the usage of `android.permission.INTERNET`, apkpatcher will not extract AndroidManifest.xml and resource files. It will modify only some smali code.
+  ~~APK Patcher will try the most it can to avoid extracting resource files, since this task may fail sometimes. So if you just want to insert frida gadget and the app already declares the usage of `android.permission.INTERNET`, apkpatcher will not extract AndroidManifest.xml and resource files. It will modify only some smali code.~~
   
-  If you want to force APK Patcher to extract resources even when it its not required, use the following command
-  ```
-  apkpatcher -a base.apk --force-extract-resources
-  ```
+  As of 1.2.0 the tool will extract resources by default so the app can install: https://github.com/iBotPeaches/Apktool/issues/1626
 
 - ##### Help during package modification
   Every time you have to modify an APK, it is a tedious task to decompile, modify, repackage, sign (and generate a key if you don't have one) and zipalign it. APK Patcher will help you during this task. You can use the `--wait-before-repackage`, and APK Patcher will wait you make any change you want. Then you just instruct APK Patcher to continue, and it will automatically repack the APK, sign it with a random generated key and zipalign it. You can use this option with combination of other APK Patcher flags.
 
   - Just decompile and wait for me:
   ```
   apkpatcher -a base.apk --prevent-frida-gadget --force-extract-resources -w
```

### Comparing `apkpatcher-cli-1.1.0/apkpatcher` & `apkpatcher-cli-1.2.0/apkpatcher`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
-
-from cgi import print_environ
-from fileinput import filename
+import xml.etree.ElementTree as ET
 import os
+from pathlib import Path
+from androguard.core.bytecodes.apk import APK
+import lzma
 import sys
 import json
 import time
 import signal
 import shutil
 import argparse
 import requests
 import zipfile
 from appdirs import user_data_dir, user_cache_dir
 import tempfile
 import subprocess
 
-__version__ = '1.1.0'
+__version__ = '1.2.0'
 
+APK_TOOL_VERSION = '2.8.0'
+APK_SIGNER_VERSION = '1.3.0'
 
 # noinspection SpellCheckingInspection
 class BColors:
     COLOR_BLUE = '\033[94m'
     COLOR_RED_BG = '\033[101m'
     COLOR_RED = '\033[91m'
     COLOR_GREEN = '\033[92m'
@@ -36,15 +39,49 @@
     FAIL = '\033[91m'
     ENDC = '\033[0m'
     BOLD = '\033[1m'
     UNDERLINE = '\033[4m'
 
 
 # noinspection PyBroadException,SpellCheckingInspection
+class ExternalDependencies:
+    def __init__(self) -> None:
+        self.dependencies = {}
+        self.required_dependencies = {}
+
+    def add_depedency(self, name, path=None, required=True):
+        path = path or shutil.which(name)
+        if required:
+            self.required_dependencies[name] = bool(path)
+        if not path:
+            return None
+        self.dependencies[name] = path
+        return path
+    
+    def get_depedency(self, name):
+        if name not in self.dependencies:
+            return None
+        return self.dependencies[name]
+    
+    def has_satisfied_required_dependencies(self):
+        for i in self.required_dependencies.values():
+            if not i:
+                return False
+        return True
+    
+    def __getattr__(self, name):
+        return self.get_depedency(name.replace('_', '-'))
+
+
+# noinspection PyBroadException,SpellCheckingInspection
 class Patcher:
+
+    dependencies_manager = None
+
+
     apk_file_path = None
     apk_tmp_dir = None
 
     appname = 'apkpatcher'
     appauthor = 'nitanmarcel'
 
     data_dir = user_data_dir(appname, appauthor)
@@ -89,95 +126,20 @@
         if self.VERBOSITY >= self.VERBOSITY_LOW:
             sys.stdout.write(BColors.COLOR_GREEN + '[+] {0}\n'.format(msg) + BColors.ENDC)
 
     def print_warn(self, msg):
         if self.VERBOSITY >= self.VERBOSITY_LOW:
             sys.stdout.write(BColors.COLOR_RED + '[-] {0}\n'.format(msg) + BColors.ENDC)
 
-    def has_satisfied_dependencies(self, action='all'):
-        flag = True
-        self.print_info('Checking dependencies...')
-
-        # Check Frida
-        try:
-            subprocess.check_output(['frida', '--version'])
-        except Exception:
-            flag = False
-            self.print_warn('Frida is not installed')
-
-        # Check aapt
-        if action in ['all']:
-            try:
-                subprocess.check_output(['aapt', 'version'])
-            except Exception:
-                flag = False
-                self.print_warn('aapt is not installed')
-
-        # Check adb
-        if action in ['all']:
-            try:
-                subprocess.check_output(['adb', '--version'])
-            except Exception:
-                flag = False
-                self.print_warn('adb is not installed')
-
-        # Check apktool
-        if action in ['all']:
-            try:
-                subprocess.check_output(['apktool', '--version'])
-            except Exception:
-                self.print_warn('Apktool is not installed')
-                flag = False
-
-        # Check unxz
-        if action in ['all']:
-            try:
-                subprocess.check_output(['unxz', '--version'])
-            except Exception:
-                flag = False
-                self.print_warn('unxz is not installed')
-
-        # Check keytool
-        if action in ['all']:
-            try:
-                cmd_output = subprocess.check_output(['keytool;echo'], stderr=subprocess.STDOUT, shell=True)
-
-                if b'Key and Certificate' not in cmd_output:
-                    flag = False
-                    self.print_warn('keytool is not installed')
-
-            except Exception:
-                flag = False
-                self.print_warn('keytool is not installed')
-
-        # Check jarsigner
-        if action in ['all']:
-            try:
-                subprocess.check_output(['jarsigner', '-h'], stderr=subprocess.STDOUT)
-            except Exception:
-                flag = False
-                self.print_warn('jarsigner is not installed')
-
-        # Check Zipalign
-        if action in ['all']:
-            cmd_output = subprocess.check_output(['zipalign;echo'],
-                                                 stderr=subprocess.STDOUT, shell=True).decode('utf-8')
-
-            if 'zip alignment' not in cmd_output.lower():
-                flag = False
-                self.print_warn('zipalign is not installed')
-
-        return flag
-
     def update_apkpatcher_gadgets(self):
         if not self.has_satisfied_dependencies():
             self.print_warn('One or more dependencies are missing!')
             return False
 
-        frida_version = subprocess.check_output(['frida', '--version']).decode('utf-8').strip()
+        frida_version = subprocess.check_output([self.dependencies_manager.frida, '--version']).decode('utf-8').strip()
         self.print_info('Updating frida gadgets according to your frida version: {0}'.format(frida_version))
 
         github_link = 'https://api.github.com/repos/frida/frida/releases'
 
         response = requests.get(github_link).text
         releases = json.loads(response)
 
@@ -209,25 +171,26 @@
             os.makedirs(target_folder)
 
         downloaded_files = []
         for gadget in list_gadgets:
             gadget_file_path = os.path.join(target_folder, gadget['name'])
 
             if os.path.isfile(gadget_file_path.replace('.xz', '')):
-                self.print_info('{0} already exists. Skipping.'.format(gadget['name']))
+                print(f'{gadget["name"]} already exists. Skipping.')
             else:
                 self.download_file(gadget['url'], gadget_file_path)
                 downloaded_files.append(gadget_file_path)
 
-        self.print_info('Extracting downloaded files...')
+        print('Extracting downloaded files...')
 
         for downloaded_file in downloaded_files:
-            subprocess.check_output(['unxz', downloaded_file])
+            with lzma.open(downloaded_file) as f, open(downloaded_file.replace(".xz", ""), "wb") as outfile:
+                outfile.write(f.read())
 
-        self.print_done('Done! Gadgets were updated')
+        print('Done! Gadgets were updated')
 
         return True
 
     def download_file(self, url, target_path):
         file_name = target_path.split('/')[-1]
         response = requests.get(url, stream=True)
         response.raise_for_status()
@@ -255,25 +218,70 @@
                         sys.stdout.flush()
 
                     f.write(chunk)
 
         if self.VERBOSITY >= self.VERBOSITY_HIGH:
             sys.stdout.write('\n')
 
-    def get_recommended_gadget(self):
+    def check_and_download_tools(self):
+        apktool_path = os.path.join(self.data_dir, 'apktool_{0}.jar'.format(APK_TOOL_VERSION))
+        if not os.path.isfile(apktool_path):
+            old_apktool = Path(self.data_dir).glob('apktool*.jar')
+            for i in old_apktool:
+                self.print_info('Remove outdated apktool {0}'.format(os.path.basename(i)))
+            apktool_uri = 'https://github.com/iBotPeaches/Apktool/releases/download/v{0}/apktool_{1}.jar'.format(APK_TOOL_VERSION, APK_TOOL_VERSION)
+            self.download_file(apktool_uri, apktool_path)
+        self.dependencies_manager.add_depedency('apktool', apktool_path)
+        
+        apksigner_path = os.path.join(self.data_dir, 'uber-apk-signer-{0}.jar'.format(APK_SIGNER_VERSION))
+        if not os.path.isfile(apksigner_path):
+            old_apksigner = Path(self.data_dir).glob('uber-apk-signer-*.jar')
+            for i in old_apksigner:
+                self.print_info('Remove outdated uber-apk-signer {0}'.format(os.path.basename(i)))
+            apksigner_uri = 'https://github.com/patrickfav/uber-apk-signer/releases/download/v{0}/uber-apk-signer-{1}.jar'.format(APK_SIGNER_VERSION, APK_SIGNER_VERSION)
+            self.download_file(apksigner_uri, apksigner_path)
+        self.dependencies_manager.add_depedency('uber-apk-signer', apksigner_path)
+
+    def get_arch(self, abi=None):
+        if self.dependencies_manager.adb and abi is None:
+            self.print_info('Trying to identify the right frida-gadget...')
+            self.print_info('Waiting for device...')
+            os.system('adb wait-for-device')
+            abi = subprocess.check_output(['adb', 'shell', 'getprop ro.product.cpu.abi']).decode('utf-8').strip()
+        if abi not in ['armeabi-v7a', 'arm64', 'x86', 'x86_64']:
+            self.print_warn('Architecture {0} if not one of the supported architectures arm64-v8a, arm64, x86, x86_64'.format(abi))
+            sys.exit(0)
+        if abi in ['armeabi-v7a']:
+            return self.ARCH_ARM
+        if abi in ['arm64']:
+            return self.ARCH_ARM64
+        if abi in ['x86']:
+            return self.ARCH_X86
+        if abi in ['x64']:
+            return self.ARCH_X64
+
+    def get_recommended_gadget(self, abi=None):
         ret = None
 
-        self.print_info('Trying to identify the right frida-gadget...')
-        self.print_info('Waiting for device...')
-        os.system('adb wait-for-device')
-        abi = subprocess.check_output(['adb', 'shell', 'getprop ro.product.cpu.abi']).decode('utf-8').strip()
+        if self.dependencies_manager.adb and abi is None:
+            self.print_info('Trying to identify the right frida-gadget...')
+            self.print_info('Waiting for device...')
+            os.system('adb wait-for-device')
+            abi = subprocess.check_output(['adb', 'shell', 'getprop ro.product.cpu.abi']).decode('utf-8').strip()
+        elif not abi:
+            self.print_warn('Can\'t automatically detect device architecture. Use the --arch argument instead. (missing adb command)')
+            sys.exit(1)
+        else:
+            if abi not in ['arm64-v8a', 'arm64', 'x86', 'x86_64']:
+                self.print_warn('Architecture {0} if not one of the supported architectures arm64-v8a, arm64, x86, x86_64'.format(abi))
+                sys.exit(0)
 
         self.print_info('The abi is {0}'.format(abi))
 
-        frida_version = subprocess.check_output(['frida', '--version']).strip().decode('utf-8')
+        frida_version = subprocess.check_output([self.dependencies_manager.frida, '--version']).strip().decode('utf-8')
         gadgets_folder = os.path.join(self.data_dir, 'gadgets')
         target_folder = os.path.join(gadgets_folder, frida_version)
 
         if not os.path.isdir(target_folder):
             self.update_apkpatcher_gadgets()
         dir_list = os.listdir(target_folder)
         gadget_files = [f for f in dir_list if os.path.isfile(os.path.join(target_folder, f))]
@@ -311,20 +319,18 @@
             self.print_info('Architecture identified ({0}). Gadget was selected.' .format(abi))
 
         return ret
 
     def extract_apk(self, apk_path, destination_path, extract_resources=True):
         if extract_resources:
             self.print_info('Extracting {0} (with resources) to {1}'.format(apk_path, destination_path))
-            self.print_info('Some errors may occur while decoding resources that have framework dependencies')
-
-            subprocess.check_output(['apktool', '-f', 'd', '-o', destination_path, apk_path])
+            subprocess.check_output([self.dependencies_manager.java, '-jar', self.dependencies_manager.apktool, '-f', 'd', apk_path, '-o', destination_path])
         else:
             self.print_info('Extracting {0} (without resources) to {1}'.format(apk_path, destination_path))
-            subprocess.check_output(['apktool', '-f', '-r', 'd', '-o', destination_path, apk_path])
+            subprocess.check_output([self.dependencies_manager.java, '-jar', self.dependencies_manager.apktool, '-f', '-r', 'd', apk_path, '-o', destination_path])
 
     def extract_bundle(self, xapk_path):
         tmp_dir = tempfile.gettempdir()
         xapk_name = os.path.basename(xapk_path)
         tmp_path = os.path.join(tmp_dir, xapk_name)
         manifest_path = os.path.join(tmp_path, 'manifest.json')
         base_apk = None
@@ -343,37 +349,29 @@
             os.rmdir(tmp_path)
             sys.exit(1)
 
         self.print_info('Found base apk {0}'.format(os.path.basename(base_apk)))
         return base_apk
 
     def has_permission(self, apk_path, permission_name):
-        permissions = subprocess.check_output(['aapt', 'dump', 'permissions', apk_path]).decode('utf-8')
+        apk_file = APK(apk_path)
 
-        if permission_name in permissions:
-            self.print_info('The app {0} has the permission "{1}"'.format(apk_path, permission_name))
+        if permission_name in apk_file.get_permissions():
+            self.print_info(f'The app {apk_path} has the permission "{permission_name}"')
             return True
         else:
-            self.print_info("The app {0} doesn't have the permission '{1}'".format(apk_path, permission_name))
+            self.print_info(f"The app {apk_path} doesn't have the permission '{permission_name}'")
             return False
 
     def get_entrypoint_class_name(self, apk_path):
-        dump_lines = subprocess.check_output(['aapt', 'dump', 'badging', apk_path]).decode('utf-8').split('\n')
-        entrypoint_class = None
-
-        for line in dump_lines:
-            if 'launchable-activity:' in line:
-                name_start = line.find('name=')
-                entrypoint_class = line[name_start:].split(' ')[0]\
-                    .replace('name=', '').replace('\'', '').replace('"', '')
-
-                break
+        apk_file = APK(apk_path)
+        entrypoint_class = apk_file.get_main_activity()
 
         if entrypoint_class is None:
-            self.print_warn('Something was wrong while getting launchable-activity')
+            print('Something was wrong while getting launchable-activity')
 
         return entrypoint_class
 
     def get_entrypoint_smali_path(self, base_path, entrypoint_class):
         files_at_path = os.listdir(base_path)
         entrypoint_final_path = None
 
@@ -512,14 +510,39 @@
         with open(entrypoint_smali_path, 'w') as smali_file:
             smali_file.write(new_content)
 
         self.print_info('Frida loader was injected in the entrypoint smali file!')
 
         return True
 
+    def set_extract_native_libs(self, manifest_path):
+        if not os.path.isfile(manifest_path):
+            print("Couldn't find the Manifest file. Something is wrong with the apk!")
+            return
+
+        tree = ET.parse(manifest_path)
+        root = tree.getroot()
+
+        namespaces = {'android': 'http://schemas.android.com/apk/res/android'}
+
+        application_node = root.find('application', namespaces)
+
+        if application_node is not None:
+            extract_native_libs = application_node.get('{%s}extractNativeLibs' % namespaces['android'])
+            if extract_native_libs is not None and extract_native_libs == "false":
+                self.print_info('Setting extractNativeLibs to true. https://github.com/iBotPeaches/Apktool/issues/3081')
+                application_node.set('{%s}extractNativeLibs' % namespaces['android'], 'true')
+                tree.write(manifest_path, encoding='utf-8', xml_declaration=True)
+
+    def fix_target_sdk(self, apk_path, manifest_path):
+        if not os.path.isfile(manifest_path):
+            print("Couldn't find the Manifest file. Something is wrong with the apk!")
+            return
+        
+
     def get_arch_by_gadget(self, gadget_path):
         if 'arm' in gadget_path and '64' not in gadget_path:
             return self.ARCH_ARM
 
         elif 'arm64' in gadget_path:
             return self.ARCH_ARM64
 
@@ -641,15 +664,15 @@
                 target_autoload_path = target_gadget_path.replace(self.DEFAULT_GADGET_NAME, self.DEFAULT_HOOKFILE_NAME)
 
                 self.print_info('Copying auto load script file to {0}'.format(target_autoload_path))
                 shutil.copyfile(auto_load_script_path, target_autoload_path)
 
         return True
 
-    def repackage_apk(self, base_apk_path, apk_name, target_file=None, bundle_path=None, use_aapt2=False, keep_keystore=True):
+    def repackage_apk(self, base_apk_path, apk_name, target_file=None, bundle_path=None, use_aapt2=False):
         if target_file is None:
             current_path = os.getcwd()
             if bundle_path:
                 target_file = os.path.join(current_path, apk_name.replace('.xapk', '_patched.xapk'))
             else:
                 target_file = os.path.join(current_path, apk_name.replace('.apk', '_patched.apk'))
 
@@ -661,26 +684,26 @@
                     new_file_name = target_file.replace('.apk', '_{0}.apk'.format(timestamp))
                 target_file = new_file_name
 
         self.print_info('Repackaging apk to {0}'.format(target_file))
         self.print_info('This may take some time...')
 
         if bundle_path:
-            apktool_build_cmd = ['apktool', 'b', '-o', bundle_path, base_apk_path, '-f']
+            apktool_build_cmd = [self.dependencies_manager.java, '-jar', self.dependencies_manager.apktool, 'b', '-o', bundle_path, base_apk_path, '-f']
         else:
-            apktool_build_cmd = ['apktool', 'b', '-o', target_file, base_apk_path, '-f']
+            apktool_build_cmd = [self.dependencies_manager.java, '-jar', self.dependencies_manager.apktool, 'b', '-o', target_file, base_apk_path, '-f']
         if use_aapt2:
-            apktool_build_cmd.insert(1, "--use-aapt2") 
+            apktool_build_cmd.append('--use-aapt2')
 
         subprocess.check_output(apktool_build_cmd)
         if bundle_path:
             bundle_dir = os.path.dirname(bundle_path)
-            self.sign_and_zipalign([os.path.join(bundle_dir, f) for f in os.listdir(bundle_dir) if f.endswith('.apk')], keep_keystore)
+            self.sign_and_zipalign(bundle_dir)
         else:
-            self.sign_and_zipalign([target_file,],keep_keystore)
+            self.sign_and_zipalign(target_file)
 
         if bundle_path:
             bundle_dir_path = os.path.dirname(bundle_path)
             with zipfile.ZipFile(target_file, 'w', zipfile.ZIP_DEFLATED) as zip:
                 for foldername, subfolders, filenames in os.walk(bundle_dir_path):
                     for filename in filenames:
                         absolute_path = os.path.join(foldername, filename)
@@ -833,45 +856,21 @@
             with zipfile.ZipFile(tmp_zip, 'w') as zout:
                 for item in zin.infolist():
                     if not str(item.filename).startswith('META-INF'):
                         zout.writestr(item.filename, zin.read(item))
         os.remove(apkfile)
         os.rename(tmp_zip, apkfile)
 
-    def sign_and_zipalign(self, apk_paths, keep_keystore):
-        keystorepath = os.path.join(self.cache_dir, 'apkpatcherkeystore')
-        if not os.path.isfile(keystorepath):
-            self.print_info('Generating a random key...')
-            subprocess.call(
-                'keytool -genkey -keyalg RSA -keysize 2048 -validity 700 -noprompt -alias apkpatcheralias1 -dname '
-                '"CN=apk.patcher.com, OU=ID, O=APK, L=Patcher, S=Patch, C=BR" -keystore {0} '
-                '-storepass password -keypass password'.format(keystorepath),
-                shell=True)
-        
-        for apk in apk_paths:
-            self.print_info('Removing any existing signatures in {0}...'.format(apk))
-            self.remove_old_signature(apk)
-
-            self.print_info('Signing {0}...'.format(apk))
-            subprocess.call(
-                'jarsigner -sigalg SHA1withRSA -digestalg SHA1 -keystore {0} '
-                '-storepass password {1} apkpatcheralias1'.format(keystorepath, apk),
-                shell=True)
-
-            self.print_info('The apk was signed!')
-            self.print_info('Optimizing with zipalign...')
-            tmp_target_file = apk.replace('.apk', '_tmp.apk')
-            shutil.move(apk, tmp_target_file)
-            subprocess.call('zipalign 4 {0} {1}'.format(tmp_target_file, apk), stderr=subprocess.STDOUT, shell=True)
-
-            os.remove(tmp_target_file)
-            self.print_info('The file was optimized!')
-            
-        if not keep_keystore:
-            os.remove(keystorepath)
+    def sign_and_zipalign(self, apk_path):
+        self.print_info('Signing apk files...')  
+
+        subprocess.call('{0} -jar {1} -a {2} --allowResign --overwrite'.format(self.dependencies_manager.java, self.dependencies_manager.uber_apk_signer, apk_path), shell=True, stdout=subprocess.DEVNULL)
+        idsig_files = Path(apk_path).glob('*.idsig')
+        for i in idsig_files:
+            os.remove(i)
 
         self.print_info('The APK files were signed and optimized!')
 
     @staticmethod
     def get_int_frida_version(str_version):
         version_split = str_version.split('.')
 
@@ -880,15 +879,15 @@
 
         while len(version_split) < 3:
             version_split.append('0')
 
         return int(''.join(["{num:03d}".format(num=int(i)) for i in version_split]))
 
     def min_frida_version(self, min_version):
-        frida_version = subprocess.check_output(['frida', '--version']).strip().decode('utf-8')
+        frida_version = subprocess.check_output([self.dependencies_manager.frida, '--version']).strip().decode('utf-8')
 
         if self.get_int_frida_version(frida_version) < self.get_int_frida_version(min_version):
             return False
 
         return True
 
     def get_default_config_file(self):
@@ -921,32 +920,31 @@
 # noinspection SpellCheckingInspection
 def main():
     patcher = Patcher()
 
     parser = argparse.ArgumentParser()
     parser.add_argument('-a', '--apk', help='Specify the apk you want to patch')
     parser.add_argument('-g', '--gadget', help='Specify the frida-gadget file')
+    parser.add_argument('--arch', help='Force architecture to inject frida gadget for. Supported arches: arm64-v8a, arm64, x86, x86_64')
     parser.add_argument('--autoload-script', help='Auto load script')
     parser.add_argument("--codeshare", help='Auto load script from codeshare')
     parser.add_argument('-v', '--verbosity', help='Verbosity level (0 to 3). Default is 3')
     parser.add_argument('--update-gadgets', help='Update frida-gadgets', action='store_true')
-    parser.add_argument('-f', '--force-extract-resources', help='Force extract resources and manifest',
+    parser.add_argument('-r', '--no-resources', help='Do not extract resources',
                         action='store_true')
     parser.add_argument('--use-aapt2', help='Use aapt2 with apktool',
                         action='store_true')
 
     parser.add_argument('-e', '--enable-user-certificates', help='Add some configs in apk to accept user certificates',
                         action='store_true')
 
     parser.add_argument('--prevent-frida-gadget', help='Does not insert frida gadget', action='store_true')
     parser.add_argument('-l', '--lib', help="Inject a shared library in place of frida gadget")
     parser.add_argument('-w', '--wait-before-repackage', help='Waits for your OK before repackage the apk',
                         action='store_true')
-    parser.add_argument('-k', '--keep-keystore', help='Keeps generated keystore for future use',
-                        action='store_true')
 
     parser.add_argument('-o', '--output-file', help='Specify the output file (patched)')
 
     parser.add_argument('--version', help='Display information about the version', action='store_true')
 
     group = parser.add_argument_group('Execute command before repackage')
     group.add_argument('-x', '--exec-before-repackage', help='Specify a command to execute before repackage')
@@ -957,128 +955,148 @@
     args = parser.parse_args()
 
     if len(sys.argv) == 1:
         parser.print_help()
 
         return 1
     
+    dependencies_manager = ExternalDependencies()
+    
     if args.version:
         patcher.set_verbosity(patcher.VERBOSITY_HIGH)
-
-        frida_version = subprocess.check_output(['frida', '--version']).strip().decode('utf-8')
-        patcher.print_info('frida {0}'.format(frida_version))
         patcher.print_done('apkpatcher {0}'.format(__version__))
         return 1
+    
+    if not dependencies_manager.add_depedency('java'):
+        patcher.print_warn('java is not installed')
+        return 1
+    
+    dependencies_manager.add_depedency('frida', required=False)
+    dependencies_manager.add_depedency('adb', required=False)
+    
+    if not dependencies_manager.has_satisfied_required_dependencies():
+        patcher.print_warn('One or more dependencies were not satisfied.')
+        return
+        
+    
+    patcher.dependencies_manager = dependencies_manager
 
     if args.verbosity:
         patcher.set_verbosity(int(args.verbosity))
     else:
         patcher.set_verbosity(patcher.VERBOSITY_HIGH)
 
     if args.update_gadgets:
-        patcher.update_apkpatcher_gadgets()
+        if dependencies_manager.frida:
+            patcher.update_apkpatcher_gadgets()
+        else:
+            patcher.print_warn('--update-gadgets disabled. (missing frida command)')
 
         return 0
 
     if not args.apk:
         parser.print_help()
 
         return 1
 
     else:
         if not os.path.isfile(args.apk):
             patcher.print_warn("The file {0} couldn't be found!".format(args.apk))
 
             return 1
 
-    if not patcher.has_satisfied_dependencies('all'):
-        patcher.print_warn('One or more dependencies were not satisfied.')
-
-        return 1
-
     gadget_to_use = None
-    if not args.prevent_frida_gadget:
+    if not args.prevent_frida_gadget and dependencies_manager.frida:
         if args.gadget:
             gadget_to_use = args.gadget
 
         else:
-            gadget_to_use = patcher.get_recommended_gadget()
+            gadget_to_use = patcher.get_recommended_gadget(abi=args.arch)
 
         if gadget_to_use is None or not os.path.isfile(gadget_to_use):
             patcher.print_warn('Could not identify the gadget!')
 
             return 1
+        
+    patcher.check_and_download_tools()
 
     # THE APK PATCHING STARTS HERE
 
     apk_file_path = args.apk
     apk_file_name = os.path.basename(apk_file_path)
     if apk_file_path.endswith('.xapk'):
         patcher.is_bundle = True
         apk_file_path = patcher.extract_bundle(apk_file_path)
     temporary_path = patcher.create_temp_folder_for_apk(apk_file_path)
 
     has_internet_permission = False
     if not args.prevent_frida_gadget:
         has_internet_permission = patcher.has_permission(apk_file_path, patcher.INTERNET_PERMISSION)
 
-    # Will extract the resources when needed or when forced
-    if (not args.prevent_frida_gadget and not has_internet_permission) \
-            or args.enable_user_certificates or args.force_extract_resources:
-
-        patcher.extract_apk(apk_file_path, temporary_path, extract_resources=True)
+    if args.no_resources:
+        if not args.prevent_frida_gadget or args.lib:
+            patcher.print_warn('Can\'t inject frida or libraries without extracting resources. https://github.com/iBotPeaches/Apktool/issues/3081')
+            sys.exit(1)
+        if args.enable_user_certificates:
+            patcher.print_warn('Can\'t enable user certificates without extracting resources. https://github.com/iBotPeaches/Apktool/issues/3081')
+            sys.exit(1)
+        patcher.extract_apk(apk_file_path, temporary_path, extract_resources=False)
 
     else:
-        patcher.extract_apk(apk_file_path, temporary_path, extract_resources=False)
+        patcher.extract_apk(apk_file_path, temporary_path, extract_resources=True)
 
     if not args.prevent_frida_gadget and not has_internet_permission:
         patcher.inject_permission_manifest(temporary_path, patcher.INTERNET_PERMISSION)
 
     if args.enable_user_certificates:
         patcher.enable_user_certificates(temporary_path)
 
     if not args.prevent_frida_gadget and not args.lib:
-        # START --[ INJECTING FRIDA LIB FILE AND SMALI CODE ]--
-        entrypoint_class = patcher.get_entrypoint_class_name(apk_file_path)
-        entrypoint_smali_path = patcher.get_entrypoint_smali_path(temporary_path, entrypoint_class)
-
-        patcher.insert_frida_loader(entrypoint_smali_path)
-
-        if args.autoload_script or args.codeshare:
-            if not patcher.min_frida_version('10.6.33'):
-                patcher.print_warn('Autoload is not supported in this version of frida. Update it!')
-
-                return 1
+        if not dependencies_manager.frida:
+            patcher.print_warn('Frida patching disabled. (missing frida command).')
+        else:
+            # START --[ INJECTING FRIDA LIB FILE AND SMALI CODE ]--
+            entrypoint_class = patcher.get_entrypoint_class_name(apk_file_path)
+            entrypoint_smali_path = patcher.get_entrypoint_smali_path(temporary_path, entrypoint_class)
+
+            patcher.insert_frida_loader(entrypoint_smali_path)
+
+            if args.autoload_script or args.codeshare:
+                if dependencies_manager.frida:
+                    if not patcher.min_frida_version('10.6.33'):
+                        patcher.print_warn('Autoload is not supported in this version of frida. Update it!')
+                        return 1
+                    else:
+                        patcher.print_warn('Couldn\'t fetch frida version. Autoload might not be supported on the device')
 
-            script_file = args.autoload_script or patcher.get_codeshare(args.codeshare)
+                script_file = args.autoload_script or patcher.get_codeshare(args.codeshare)
 
-            if not os.path.isfile(script_file):
-                patcher.print_warn('The script {0} was not found.'.format(script_file))
+                if not os.path.isfile(script_file):
+                    patcher.print_warn('The script {0} was not found.'.format(script_file))
 
-                return 1
+                    return 1
 
-            default_config_file = patcher.get_default_config_file()
-            patcher.insert_frida_lib(temporary_path, gadget_to_use,
-                                     config_file_path=default_config_file, auto_load_script_path=script_file)
+                default_config_file = patcher.get_default_config_file()
+                patcher.insert_frida_lib(temporary_path, gadget_to_use,
+                                        config_file_path=default_config_file, auto_load_script_path=script_file)
 
-        else:
-            patcher.insert_frida_lib(temporary_path, gadget_to_use)
-        # END --[ INJECTING FRIDA LIB FILE AND SMALI CODE ]--
+            else:
+                patcher.insert_frida_lib(temporary_path, gadget_to_use)
+            # END --[ INJECTING FRIDA LIB FILE AND SMALI CODE ]--
 
     elif args.lib:
         lib_file = args.lib
         if not os.path.isfile(lib_file):
             patcher.print_warn('Library {0} was not found.'.format(lib_file))
         lib_name, lib_ext = os.path.basename(lib_file).rsplit('.', 1)
         lib_path = os.path.abspath(args.lib)
         entrypoint_class = patcher.get_entrypoint_class_name(apk_file_path)
 
         entrypoint_smali_path = patcher.get_entrypoint_smali_path(temporary_path, entrypoint_class)
-        recommended_gadget = patcher.get_recommended_gadget()
-        arch = patcher.get_arch_by_gadget(recommended_gadget)
+        arch = patcher.get_arch(abi=args.arch)
         patcher.insert_shared_lib(temporary_path, lib_path, lib_name + '.' + lib_ext, arch)
         patcher.insert_frida_loader(entrypoint_smali_path, lib_name)
 
     if args.wait_before_repackage:
         patcher.print_info('Apkpatcher is waiting for your OK to repackage the apk...')
 
         answer = input(BColors.COLOR_BLUE + '[*] Are you ready? (y/N): ' + BColors.ENDC)
@@ -1099,18 +1117,23 @@
         print(BColors.COLOR_RED + '[!] Provided shell command: {0}'.format(command_to_execute) + BColors.COLOR_ENDC)
         answer = input(BColors.COLOR_RED + '[!] Are you sure you want to execute it? (y/N) ' + BColors.ENDC)
 
         if answer.lower() == 'y':
             patcher.print_info('Executing -> {0}'.format(command_to_execute))
             os.system(command_to_execute)
 
+
+    if not args.no_resources:
+        manifest_path = os.path.join(temporary_path, 'AndroidManifest.xml')
+        patcher.set_extract_native_libs(manifest_path)
+
     if patcher.is_bundle:
-        output_file_path = patcher.repackage_apk(temporary_path, apk_file_name, target_file=args.output_file, bundle_path=apk_file_path, use_aapt2=args.use_aapt2, keep_keystore=args.keep_keystore)
+        output_file_path = patcher.repackage_apk(temporary_path, apk_file_name, target_file=args.output_file, bundle_path=apk_file_path, use_aapt2=args.use_aapt2)
     else:
-        output_file_path = patcher.repackage_apk(temporary_path, apk_file_name, target_file=args.output_file, use_aapt2=args.use_aapt2, keep_keystore=args.keep_keystore)
+        output_file_path = patcher.repackage_apk(temporary_path, apk_file_name, target_file=args.output_file, use_aapt2=args.use_aapt2)
 
     patcher.print_done('The temporary folder was not deleted. Find it at {0}'.format(temporary_path))
     patcher.print_done('Your file is located at {0}.'.format(output_file_path))
 
     return 0
```

### Comparing `apkpatcher-cli-1.1.0/apkpatcher_cli.egg-info/PKG-INFO` & `apkpatcher-cli-1.2.0/apkpatcher_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher-cli
-Version: 1.1.0
+Version: 1.2.0
 Summary: Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher
 Home-page: https://github.com/nitanmarcel/apkpatcher
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkpatcher-cli-1.1.0/setup.py` & `apkpatcher-cli-1.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from setuptools import setup
 
 setup(
    name='apkpatcher-cli',
-   version='1.1.0',
+   version='1.2.0',
    description='Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher',
    author='Marcel Alexandru Nitan',
    author_email='nitan.marcel@gmail.com',
    url='https://github.com/nitanmarcel/apkpatcher',
    keywords=['FRIDA', 'APK'],
    scripts=['apkpatcher'],
    install_requires=[
        'requests',
        'appdirs',
+       'androguard'
    ],
    classifiers=[
     'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
 
    ]
-)
+)
```

