# Comparing `tmp/apkpatcher-cli-1.2.0.tar.gz` & `tmp/apkpatcher-cli-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkpatcher-cli-1.2.0.tar", last modified: Sat Jul 22 00:43:04 2023, max compression
+gzip compressed data, was "apkpatcher-cli-1.3.1.tar", last modified: Sat Jul 22 10:20:49 2023, max compression
```

## Comparing `apkpatcher-cli-1.2.0.tar` & `apkpatcher-cli-1.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 00:43:04.921554 apkpatcher-cli-1.2.0/
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)    18046 2023-07-21 09:54:40.000000 apkpatcher-cli-1.2.0/LICENSE
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 00:43:04.921554 apkpatcher-cli-1.2.0/PKG-INFO
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)     7059 2023-07-21 22:59:45.000000 apkpatcher-cli-1.2.0/README.md
--rwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)    44789 2023-07-22 00:37:29.000000 apkpatcher-cli-1.2.0/apkpatcher
-drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 00:43:04.921554 apkpatcher-cli-1.2.0/apkpatcher_cli.egg-info/
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 00:43:04.000000 apkpatcher-cli-1.2.0/apkpatcher_cli.egg-info/PKG-INFO
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      226 2023-07-22 00:43:04.000000 apkpatcher-cli-1.2.0/apkpatcher_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 00:43:04.000000 apkpatcher-cli-1.2.0/apkpatcher_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       28 2023-07-22 00:43:04.000000 apkpatcher-cli-1.2.0/apkpatcher_cli.egg-info/requires.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 00:43:04.000000 apkpatcher-cli-1.2.0/apkpatcher_cli.egg-info/top_level.txt
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       38 2023-07-22 00:43:04.921554 apkpatcher-cli-1.2.0/setup.cfg
--rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      825 2023-07-22 00:42:38.000000 apkpatcher-cli-1.2.0/setup.py
+drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 10:20:49.006232 apkpatcher-cli-1.3.1/
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)    18046 2023-07-21 09:54:40.000000 apkpatcher-cli-1.3.1/LICENSE
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 10:20:49.006232 apkpatcher-cli-1.3.1/PKG-INFO
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)     6930 2023-07-22 10:11:16.000000 apkpatcher-cli-1.3.1/README.md
+-rwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)    46479 2023-07-22 10:20:08.000000 apkpatcher-cli-1.3.1/apkpatcher
+drwxr-xr-x   0 nitanmarcel  (1000) nitanmarcel  (1000)        0 2023-07-22 10:20:49.006232 apkpatcher-cli-1.3.1/apkpatcher_cli.egg-info/
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      692 2023-07-22 10:20:48.000000 apkpatcher-cli-1.3.1/apkpatcher_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      226 2023-07-22 10:20:48.000000 apkpatcher-cli-1.3.1/apkpatcher_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 10:20:48.000000 apkpatcher-cli-1.3.1/apkpatcher_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       28 2023-07-22 10:20:48.000000 apkpatcher-cli-1.3.1/apkpatcher_cli.egg-info/requires.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)        1 2023-07-22 10:20:48.000000 apkpatcher-cli-1.3.1/apkpatcher_cli.egg-info/top_level.txt
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)       38 2023-07-22 10:20:49.006232 apkpatcher-cli-1.3.1/setup.cfg
+-rw-r--r--   0 nitanmarcel  (1000) nitanmarcel  (1000)      825 2023-07-22 10:20:10.000000 apkpatcher-cli-1.3.1/setup.py
```

### Comparing `apkpatcher-cli-1.2.0/LICENSE` & `apkpatcher-cli-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apkpatcher-cli-1.2.0/PKG-INFO` & `apkpatcher-cli-1.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher-cli
-Version: 1.2.0
+Version: 1.3.1
 Summary: Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher
 Home-page: https://github.com/nitanmarcel/apkpatcher
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkpatcher-cli-1.2.0/README.md` & `apkpatcher-cli-1.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 #### How To Install
 ##### Dependencies
 Starting with 1.2.0 only `java` is a required dependencies, with `frida` and `adb` as optional dependencies.
 
 
 - java (required)
-- frida and frida-tools: `pip3 install frida frida-tools` (optional to install frida gadget/scripts into the target application)
 - adb (optional to automatically detect target architecture)
 
 ##### APK Patcher Installation
 `pip install apkpatcher-cli`
 
 #### How To Use It
 For all usages, the output file will be something like <apkname>_patched.apk.
```

### Comparing `apkpatcher-cli-1.2.0/apkpatcher` & `apkpatcher-cli-1.3.1/apkpatcher`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
-import xml.etree.ElementTree as ET
-import os
-from pathlib import Path
-from androguard.core.bytecodes.apk import APK
+import argparse
+import json
 import lzma
+import os
+import shutil
+import signal
+import subprocess
 import sys
-import json
+import tempfile
 import time
-import signal
-import shutil
-import argparse
-import requests
+import xml.etree.ElementTree as ET
 import zipfile
-from appdirs import user_data_dir, user_cache_dir
-import tempfile
-import subprocess
+from pathlib import Path
 
-__version__ = '1.2.0'
+import requests
+from appdirs import user_cache_dir, user_data_dir
+
+__version__ = '1.3.1'
 
 APK_TOOL_VERSION = '2.8.0'
 APK_SIGNER_VERSION = '1.3.0'
 
 # noinspection SpellCheckingInspection
+
+
 class BColors:
     COLOR_BLUE = '\033[94m'
     COLOR_RED_BG = '\033[101m'
     COLOR_RED = '\033[91m'
     COLOR_GREEN = '\033[92m'
     COLOR_BOLD = '\033[1m'
     COLOR_ENDC = '\033[0m'
@@ -52,36 +54,35 @@
         path = path or shutil.which(name)
         if required:
             self.required_dependencies[name] = bool(path)
         if not path:
             return None
         self.dependencies[name] = path
         return path
-    
+
     def get_depedency(self, name):
         if name not in self.dependencies:
             return None
         return self.dependencies[name]
-    
+
     def has_satisfied_required_dependencies(self):
         for i in self.required_dependencies.values():
             if not i:
                 return False
         return True
-    
+
     def __getattr__(self, name):
         return self.get_depedency(name.replace('_', '-'))
 
 
 # noinspection PyBroadException,SpellCheckingInspection
 class Patcher:
 
     dependencies_manager = None
 
-
     apk_file_path = None
     apk_tmp_dir = None
 
     appname = 'apkpatcher'
     appauthor = 'nitanmarcel'
 
     data_dir = user_data_dir(appname, appauthor)
@@ -116,31 +117,31 @@
         self.apk_file_path = apk_file_path
 
     def set_verbosity(self, verbosity_level):
         self.VERBOSITY = verbosity_level
 
     def print_info(self, msg):
         if self.VERBOSITY >= self.VERBOSITY_HIGH:
-            sys.stdout.write(BColors.COLOR_BLUE + '[*] {0}\n'.format(msg) + BColors.ENDC)
+            sys.stdout.write(BColors.COLOR_BLUE +
+                             '[*] {0}\n'.format(msg) + BColors.ENDC)
 
     def print_done(self, msg):
         if self.VERBOSITY >= self.VERBOSITY_LOW:
-            sys.stdout.write(BColors.COLOR_GREEN + '[+] {0}\n'.format(msg) + BColors.ENDC)
+            sys.stdout.write(BColors.COLOR_GREEN +
+                             '[+] {0}\n'.format(msg) + BColors.ENDC)
 
     def print_warn(self, msg):
         if self.VERBOSITY >= self.VERBOSITY_LOW:
-            sys.stdout.write(BColors.COLOR_RED + '[-] {0}\n'.format(msg) + BColors.ENDC)
+            sys.stdout.write(BColors.COLOR_RED +
+                             '[-] {0}\n'.format(msg) + BColors.ENDC)
 
     def update_apkpatcher_gadgets(self):
-        if not self.has_satisfied_dependencies():
-            self.print_warn('One or more dependencies are missing!')
-            return False
-
-        frida_version = subprocess.check_output([self.dependencies_manager.frida, '--version']).decode('utf-8').strip()
-        self.print_info('Updating frida gadgets according to your frida version: {0}'.format(frida_version))
+        frida_version = self.get_frida_version()
+        self.print_info(
+            'Updating frida gadgets according to your frida version: {0}'.format(frida_version))
 
         github_link = 'https://api.github.com/repos/frida/frida/releases'
 
         response = requests.get(github_link).text
         releases = json.loads(response)
 
         release_link = None
@@ -219,40 +220,49 @@
 
                     f.write(chunk)
 
         if self.VERBOSITY >= self.VERBOSITY_HIGH:
             sys.stdout.write('\n')
 
     def check_and_download_tools(self):
-        apktool_path = os.path.join(self.data_dir, 'apktool_{0}.jar'.format(APK_TOOL_VERSION))
+        apktool_path = os.path.join(
+            self.data_dir, 'apktool_{0}.jar'.format(APK_TOOL_VERSION))
         if not os.path.isfile(apktool_path):
             old_apktool = Path(self.data_dir).glob('apktool*.jar')
             for i in old_apktool:
-                self.print_info('Remove outdated apktool {0}'.format(os.path.basename(i)))
-            apktool_uri = 'https://github.com/iBotPeaches/Apktool/releases/download/v{0}/apktool_{1}.jar'.format(APK_TOOL_VERSION, APK_TOOL_VERSION)
+                self.print_info(
+                    'Remove outdated apktool {0}'.format(os.path.basename(i)))
+            apktool_uri = 'https://github.com/iBotPeaches/Apktool/releases/download/v{0}/apktool_{1}.jar'.format(
+                APK_TOOL_VERSION, APK_TOOL_VERSION)
             self.download_file(apktool_uri, apktool_path)
         self.dependencies_manager.add_depedency('apktool', apktool_path)
-        
-        apksigner_path = os.path.join(self.data_dir, 'uber-apk-signer-{0}.jar'.format(APK_SIGNER_VERSION))
+
+        apksigner_path = os.path.join(
+            self.data_dir, 'uber-apk-signer-{0}.jar'.format(APK_SIGNER_VERSION))
         if not os.path.isfile(apksigner_path):
             old_apksigner = Path(self.data_dir).glob('uber-apk-signer-*.jar')
             for i in old_apksigner:
-                self.print_info('Remove outdated uber-apk-signer {0}'.format(os.path.basename(i)))
-            apksigner_uri = 'https://github.com/patrickfav/uber-apk-signer/releases/download/v{0}/uber-apk-signer-{1}.jar'.format(APK_SIGNER_VERSION, APK_SIGNER_VERSION)
+                self.print_info(
+                    'Remove outdated uber-apk-signer {0}'.format(os.path.basename(i)))
+            apksigner_uri = 'https://github.com/patrickfav/uber-apk-signer/releases/download/v{0}/uber-apk-signer-{1}.jar'.format(
+                APK_SIGNER_VERSION, APK_SIGNER_VERSION)
             self.download_file(apksigner_uri, apksigner_path)
-        self.dependencies_manager.add_depedency('uber-apk-signer', apksigner_path)
+        self.dependencies_manager.add_depedency(
+            'uber-apk-signer', apksigner_path)
 
     def get_arch(self, abi=None):
         if self.dependencies_manager.adb and abi is None:
             self.print_info('Trying to identify the right frida-gadget...')
             self.print_info('Waiting for device...')
             os.system('adb wait-for-device')
-            abi = subprocess.check_output(['adb', 'shell', 'getprop ro.product.cpu.abi']).decode('utf-8').strip()
+            abi = subprocess.check_output(
+                ['adb', 'shell', 'getprop ro.product.cpu.abi']).decode('utf-8').strip()
         if abi not in ['armeabi-v7a', 'arm64', 'x86', 'x86_64']:
-            self.print_warn('Architecture {0} if not one of the supported architectures arm64-v8a, arm64, x86, x86_64'.format(abi))
+            self.print_warn(
+                'Architecture {0} if not one of the supported architectures arm64-v8a, arm64, x86, x86_64'.format(abi))
             sys.exit(0)
         if abi in ['armeabi-v7a']:
             return self.ARCH_ARM
         if abi in ['arm64']:
             return self.ARCH_ARM64
         if abi in ['x86']:
             return self.ARCH_X86
@@ -262,33 +272,37 @@
     def get_recommended_gadget(self, abi=None):
         ret = None
 
         if self.dependencies_manager.adb and abi is None:
             self.print_info('Trying to identify the right frida-gadget...')
             self.print_info('Waiting for device...')
             os.system('adb wait-for-device')
-            abi = subprocess.check_output(['adb', 'shell', 'getprop ro.product.cpu.abi']).decode('utf-8').strip()
+            abi = subprocess.check_output(
+                ['adb', 'shell', 'getprop ro.product.cpu.abi']).decode('utf-8').strip()
         elif not abi:
-            self.print_warn('Can\'t automatically detect device architecture. Use the --arch argument instead. (missing adb command)')
+            self.print_warn(
+                'Can\'t automatically detect device architecture. Use the --arch argument instead. (missing adb command)')
             sys.exit(1)
         else:
             if abi not in ['arm64-v8a', 'arm64', 'x86', 'x86_64']:
-                self.print_warn('Architecture {0} if not one of the supported architectures arm64-v8a, arm64, x86, x86_64'.format(abi))
+                self.print_warn(
+                    'Architecture {0} if not one of the supported architectures arm64-v8a, arm64, x86, x86_64'.format(abi))
                 sys.exit(0)
 
         self.print_info('The abi is {0}'.format(abi))
 
-        frida_version = subprocess.check_output([self.dependencies_manager.frida, '--version']).strip().decode('utf-8')
+        frida_version = self.get_frida_version()
         gadgets_folder = os.path.join(self.data_dir, 'gadgets')
         target_folder = os.path.join(gadgets_folder, frida_version)
 
         if not os.path.isdir(target_folder):
             self.update_apkpatcher_gadgets()
         dir_list = os.listdir(target_folder)
-        gadget_files = [f for f in dir_list if os.path.isfile(os.path.join(target_folder, f))]
+        gadget_files = [f for f in dir_list if os.path.isfile(
+            os.path.join(target_folder, f))]
         if abi in ['armeabi', 'armeabi-v7a']:
             for gadget_file in gadget_files:
                 if 'arm' in gadget_file and '64' not in gadget_file:
                     full_path = os.path.join(target_folder, gadget_file)
                     ret = full_path
                     break
 
@@ -312,95 +326,129 @@
                     full_path = os.path.join(target_folder, gadget_file)
                     ret = full_path
                     break
 
         if ret is None:
             self.print_warn('No recommended gadget file was found.')
         else:
-            self.print_info('Architecture identified ({0}). Gadget was selected.' .format(abi))
+            self.print_info(
+                'Architecture identified ({0}). Gadget was selected.' .format(abi))
 
         return ret
 
     def extract_apk(self, apk_path, destination_path, extract_resources=True):
         if extract_resources:
-            self.print_info('Extracting {0} (with resources) to {1}'.format(apk_path, destination_path))
-            subprocess.check_output([self.dependencies_manager.java, '-jar', self.dependencies_manager.apktool, '-f', 'd', apk_path, '-o', destination_path])
+            self.print_info('Extracting {0} (with resources) to {1}'.format(
+                apk_path, destination_path))
+            subprocess.check_output([self.dependencies_manager.java, '-jar',
+                                    self.dependencies_manager.apktool, '-f', 'd', apk_path, '-o', destination_path])
         else:
-            self.print_info('Extracting {0} (without resources) to {1}'.format(apk_path, destination_path))
-            subprocess.check_output([self.dependencies_manager.java, '-jar', self.dependencies_manager.apktool, '-f', '-r', 'd', apk_path, '-o', destination_path])
+            self.print_info('Extracting {0} (without resources) to {1}'.format(
+                apk_path, destination_path))
+            subprocess.check_output([self.dependencies_manager.java, '-jar',
+                                    self.dependencies_manager.apktool, '-f', '-r', 'd', apk_path, '-o', destination_path])
 
     def extract_bundle(self, xapk_path):
         tmp_dir = tempfile.gettempdir()
         xapk_name = os.path.basename(xapk_path)
         tmp_path = os.path.join(tmp_dir, xapk_name)
         manifest_path = os.path.join(tmp_path, 'manifest.json')
         base_apk = None
         if not os.path.exists(tmp_path):
             os.mkdir(tmp_path)
-        self.print_info('Extracting bundle {0} to {1}'.format(xapk_path, tmp_path))
+        self.print_info(
+            'Extracting bundle {0} to {1}'.format(xapk_path, tmp_path))
         with zipfile.ZipFile(xapk_path) as zip:
             zip.extractall(tmp_path)
         with open(manifest_path, 'r') as manifest_file:
             manifest = json.load(manifest_file)
             for apk in manifest['split_apks']:
                 if apk['id'] == 'base':
                     base_apk = os.path.join(tmp_path, apk['file'])
         if not base_apk:
             self.print_warn('Failed to find base apk')
             os.rmdir(tmp_path)
             sys.exit(1)
 
-        self.print_info('Found base apk {0}'.format(os.path.basename(base_apk)))
+        self.print_info('Found base apk {0}'.format(
+            os.path.basename(base_apk)))
         return base_apk
 
-    def has_permission(self, apk_path, permission_name):
-        apk_file = APK(apk_path)
+    def has_permission(self, manifest_path, permission_name):
+        if not os.path.isfile(manifest_path):
+            self.print_warn(
+                "Couldn't find the Manifest file. Something is wrong with the apk!")
 
-        if permission_name in apk_file.get_permissions():
-            self.print_info(f'The app {apk_path} has the permission "{permission_name}"')
-            return True
-        else:
-            self.print_info(f"The app {apk_path} doesn't have the permission '{permission_name}'")
             return False
+        tree = ET.parse(manifest_path)
+        root = tree.getroot()
 
-    def get_entrypoint_class_name(self, apk_path):
-        apk_file = APK(apk_path)
-        entrypoint_class = apk_file.get_main_activity()
+        namespaces = {'android': 'http://schemas.android.com/apk/res/android'}
 
-        if entrypoint_class is None:
-            print('Something was wrong while getting launchable-activity')
+        for elem in root.findall('uses-permission', namespaces):
+            permission = elem.get('{%s}name' % namespaces['android'])
+            if permission == permission_name:
+                self.print_info(
+                    f'The apk has the permission "{permission_name}"')
+                return True
+        self.print_info(
+            f"The apk doesn't have the permission '{permission_name}'")
+        return False
 
-        return entrypoint_class
+    def get_entrypoint_class_name(self, manifest_path):
+        if not os.path.isfile(manifest_path):
+            self.print_warn(
+                "Couldn't find the Manifest file. Something is wrong with the apk!")
+
+            return None
+        tree = ET.parse(manifest_path)
+        root = tree.getroot()
+
+        namespaces = {'android': 'http://schemas.android.com/apk/res/android'}
+
+        main_action = "android.intent.action.MAIN"
+
+        for activity in root.findall("./application/activity", namespaces):
+            for intent_filter in activity.findall("intent-filter", namespaces):
+                for action in intent_filter.findall("action", namespaces):
+                    if action.get("{%s}name" % namespaces["android"]) == main_action:
+                        return activity.get("{%s}name" % namespaces["android"])
+        self.print_warn(
+            'Something was wrong, couldn\'t find the launchable-activity.')
+        return None
 
     def get_entrypoint_smali_path(self, base_path, entrypoint_class):
         files_at_path = os.listdir(base_path)
         entrypoint_final_path = None
 
         for file in files_at_path:
             if file.startswith('smali'):
-                entrypoint_tmp = os.path.join(base_path, file, entrypoint_class.replace('.', '/') + '.smali')
+                entrypoint_tmp = os.path.join(
+                    base_path, file, entrypoint_class.replace('.', '/') + '.smali')
 
                 if os.path.isfile(entrypoint_tmp):
                     entrypoint_final_path = entrypoint_tmp
                     break
 
         if entrypoint_final_path is None:
             self.print_warn('Couldn\'t find the application entrypoint')
         else:
-            self.print_info('Found application entrypoint at {0}'.format(entrypoint_final_path))
+            self.print_info('Found application entrypoint at {0}'.format(
+                entrypoint_final_path))
 
         return entrypoint_final_path
 
     def create_temp_folder_for_apk(self, apk_path):
         system_tmp_dir = tempfile.gettempdir()
         apkpatcher_tmp_dir = os.path.join(system_tmp_dir, 'apkptmp')
 
         apk_name = apk_path.split('/')[-1]
 
-        final_tmp_dir = os.path.join(apkpatcher_tmp_dir, apk_name.replace('.apk', '').replace('.', '_'))
+        final_tmp_dir = os.path.join(
+            apkpatcher_tmp_dir, apk_name.replace('.apk', '').replace('.', '_'))
 
         if os.path.isdir(final_tmp_dir):
             self.print_info('App temp dir already exists. Removing it...')
             shutil.rmtree(final_tmp_dir)
 
         os.makedirs(final_tmp_dir)
 
@@ -427,15 +475,16 @@
 .end method
         '''.replace('<LIBFRIDA>', frida_lib_name)
 
         with open(entrypoint_smali_path, 'r') as smali_file:
             content = smali_file.read()
 
             if 'frida-gadget' in content:
-                self.print_info('The frida-gadget is already in the entrypoint. Skipping...')
+                self.print_info(
+                    'The frida-gadget is already in the entrypoint. Skipping...')
                 return False
 
             direct_methods_start_index = content.find('# direct methods')
             direct_methods_end_index = content.find('# virtual methods')
 
             if direct_methods_start_index == -1 or direct_methods_end_index == -1:
                 self.print_warn('Could not find direct methods.')
@@ -468,24 +517,26 @@
             if has_class_constructor and prologue_start_index == -1:
                 no_prologue_case = True
 
                 locals_start_index = content.find('.locals ',
                                                   class_constructor_start_index, class_constructor_end_index)
 
             if no_prologue_case and locals_start_index == -1:
-                self.print_warn('Has class constructor. No prologue case, but no "locals 0" found.')
+                self.print_warn(
+                    'Has class constructor. No prologue case, but no "locals 0" found.')
                 return False
 
             locals_end_index = -1
             if no_prologue_case:
                 locals_end_index = locals_start_index + len('locals X')
 
             prologue_end_index = -1
             if has_class_constructor and prologue_start_index > -1:
-                prologue_end_index = prologue_start_index + len('.prologue') + 1
+                prologue_end_index = prologue_start_index + \
+                    len('.prologue') + 1
 
             if has_class_constructor:
                 if no_prologue_case:
                     new_content = content[0:locals_end_index]
 
                     if content[locals_end_index] == '0':
                         new_content += '1'
@@ -496,25 +547,27 @@
                     new_content += partial_injection_code
                     new_content += content[locals_end_index+1:]
                 else:
                     new_content = content[0:prologue_end_index]
                     new_content += partial_injection_code
                     new_content += content[prologue_end_index:]
             else:
-                tmp_index = direct_methods_start_index + len('# direct methods') + 1
+                tmp_index = direct_methods_start_index + \
+                    len('# direct methods') + 1
                 new_content = content[0:tmp_index]
                 new_content += full_injection_code
                 new_content += content[tmp_index:]
 
         # The newContent is ready to be saved
-        
+
         with open(entrypoint_smali_path, 'w') as smali_file:
             smali_file.write(new_content)
 
-        self.print_info('Frida loader was injected in the entrypoint smali file!')
+        self.print_info(
+            'Frida loader was injected in the entrypoint smali file!')
 
         return True
 
     def set_extract_native_libs(self, manifest_path):
         if not os.path.isfile(manifest_path):
             print("Couldn't find the Manifest file. Something is wrong with the apk!")
             return
@@ -523,25 +576,28 @@
         root = tree.getroot()
 
         namespaces = {'android': 'http://schemas.android.com/apk/res/android'}
 
         application_node = root.find('application', namespaces)
 
         if application_node is not None:
-            extract_native_libs = application_node.get('{%s}extractNativeLibs' % namespaces['android'])
+            extract_native_libs = application_node.get(
+                '{%s}extractNativeLibs' % namespaces['android'])
             if extract_native_libs is not None and extract_native_libs == "false":
-                self.print_info('Setting extractNativeLibs to true. https://github.com/iBotPeaches/Apktool/issues/3081')
-                application_node.set('{%s}extractNativeLibs' % namespaces['android'], 'true')
-                tree.write(manifest_path, encoding='utf-8', xml_declaration=True)
+                self.print_info(
+                    'Setting extractNativeLibs to true. https://github.com/iBotPeaches/Apktool/issues/3081')
+                application_node.set('{%s}extractNativeLibs' %
+                                     namespaces['android'], 'true')
+                tree.write(manifest_path, encoding='utf-8',
+                           xml_declaration=True)
 
     def fix_target_sdk(self, apk_path, manifest_path):
         if not os.path.isfile(manifest_path):
             print("Couldn't find the Manifest file. Something is wrong with the apk!")
             return
-        
 
     def get_arch_by_gadget(self, gadget_path):
         if 'arm' in gadget_path and '64' not in gadget_path:
             return self.ARCH_ARM
 
         elif 'arm64' in gadget_path:
             return self.ARCH_ARM64
@@ -576,15 +632,16 @@
         elif arch == self.ARCH_X86:
             sub_dir = os.path.join(libs_path, 'x86')
 
         elif arch == self.ARCH_X64:
             sub_dir = os.path.join(libs_path, 'x86_64')
 
         else:
-            self.print_warn("Couldn't create the appropriate folder with the given arch.")
+            self.print_warn(
+                "Couldn't create the appropriate folder with the given arch.")
             return []
 
         if not os.path.isdir(sub_dir):
             self.print_info('Creating folder {0}'.format(sub_dir))
             os.makedirs(sub_dir)
 
         if arch == self.ARCH_ARM:
@@ -601,100 +658,117 @@
     def delete_existing_gadget(self, arch_folder, delete_custom_files=0):
         gadget_path = os.path.join(arch_folder, self.DEFAULT_GADGET_NAME)
 
         if os.path.isfile(gadget_path):
             os.remove(gadget_path)
 
         if delete_custom_files & self.CONFIG_BIT:
-            config_file_path = os.path.join(arch_folder, self.DEFAULT_CONFIG_NAME)
+            config_file_path = os.path.join(
+                arch_folder, self.DEFAULT_CONFIG_NAME)
 
             if os.path.isfile(config_file_path):
                 os.remove(config_file_path)
 
         if delete_custom_files & self.AUTOLOAD_BIT:
-            hookfile_path = os.path.join(arch_folder, self.DEFAULT_HOOKFILE_NAME)
+            hookfile_path = os.path.join(
+                arch_folder, self.DEFAULT_HOOKFILE_NAME)
 
             if os.path.isfile(hookfile_path):
                 os.remove(hookfile_path)
 
     def insert_shared_lib(self, base_path, lib_path, lib_name, arch):
         arch_folders = self.create_lib_arch_folders(base_path, arch)
         if not arch_folders:
-            self.print_warn('Some error occurred while creating the libs folders')
+            self.print_warn(
+                'Some error occurred while creating the libs folders')
             return False
         for folder in arch_folders:
             target_path = os.path.join(folder, lib_name)
             self.print_info('Copying shared library to {}'.format(target_path))
             shutil.copyfile(lib_path, target_path)
         return True
 
     def insert_frida_lib(self, base_path, gadget_path, config_file_path=None, auto_load_script_path=None):
         arch = self.get_arch_by_gadget(gadget_path)
         arch_folders = self.create_lib_arch_folders(base_path, arch)
 
         if not arch_folders:
-            self.print_warn('Some error occurred while creating the libs folders')
+            self.print_warn(
+                'Some error occurred while creating the libs folders')
             return False
 
         for folder in arch_folders:
             if config_file_path and auto_load_script_path:
-                self.delete_existing_gadget(folder, delete_custom_files=self.CONFIG_BIT | self.AUTOLOAD_BIT)
+                self.delete_existing_gadget(
+                    folder, delete_custom_files=self.CONFIG_BIT | self.AUTOLOAD_BIT)
 
             elif config_file_path and not auto_load_script_path:
-                self.delete_existing_gadget(folder, delete_custom_files=self.CONFIG_BIT)
+                self.delete_existing_gadget(
+                    folder, delete_custom_files=self.CONFIG_BIT)
 
             elif auto_load_script_path and not config_file_path:
-                self.delete_existing_gadget(folder, delete_custom_files=self.AUTOLOAD_BIT)
+                self.delete_existing_gadget(
+                    folder, delete_custom_files=self.AUTOLOAD_BIT)
 
             else:
                 self.delete_existing_gadget(folder, delete_custom_files=0)
 
             target_gadget_path = os.path.join(folder, self.DEFAULT_GADGET_NAME)
 
             self.print_info('Copying gadget to {0}'.format(target_gadget_path))
 
             shutil.copyfile(gadget_path, target_gadget_path)
 
             if config_file_path:
-                target_config_path = target_gadget_path.replace('.so', '.config.so')
+                target_config_path = target_gadget_path.replace(
+                    '.so', '.config.so')
 
-                self.print_info('Copying config file to {0}'.format(target_config_path))
+                self.print_info(
+                    'Copying config file to {0}'.format(target_config_path))
                 shutil.copyfile(config_file_path, target_config_path)
 
             if auto_load_script_path:
-                target_autoload_path = target_gadget_path.replace(self.DEFAULT_GADGET_NAME, self.DEFAULT_HOOKFILE_NAME)
+                target_autoload_path = target_gadget_path.replace(
+                    self.DEFAULT_GADGET_NAME, self.DEFAULT_HOOKFILE_NAME)
 
-                self.print_info('Copying auto load script file to {0}'.format(target_autoload_path))
+                self.print_info(
+                    'Copying auto load script file to {0}'.format(target_autoload_path))
                 shutil.copyfile(auto_load_script_path, target_autoload_path)
 
         return True
 
     def repackage_apk(self, base_apk_path, apk_name, target_file=None, bundle_path=None, use_aapt2=False):
         if target_file is None:
             current_path = os.getcwd()
             if bundle_path:
-                target_file = os.path.join(current_path, apk_name.replace('.xapk', '_patched.xapk'))
+                target_file = os.path.join(
+                    current_path, apk_name.replace('.xapk', '_patched.xapk'))
             else:
-                target_file = os.path.join(current_path, apk_name.replace('.apk', '_patched.apk'))
+                target_file = os.path.join(
+                    current_path, apk_name.replace('.apk', '_patched.apk'))
 
             if os.path.isfile(target_file):
                 timestamp = str(time.time()).replace('.', '')
                 if bundle_path:
-                    new_file_name = target_file.replace('.xapk', '_{0}.xapk'.format(timestamp))
+                    new_file_name = target_file.replace(
+                        '.xapk', '_{0}.xapk'.format(timestamp))
                 else:
-                    new_file_name = target_file.replace('.apk', '_{0}.apk'.format(timestamp))
+                    new_file_name = target_file.replace(
+                        '.apk', '_{0}.apk'.format(timestamp))
                 target_file = new_file_name
 
         self.print_info('Repackaging apk to {0}'.format(target_file))
         self.print_info('This may take some time...')
 
         if bundle_path:
-            apktool_build_cmd = [self.dependencies_manager.java, '-jar', self.dependencies_manager.apktool, 'b', '-o', bundle_path, base_apk_path, '-f']
+            apktool_build_cmd = [self.dependencies_manager.java, '-jar',
+                                 self.dependencies_manager.apktool, 'b', '-o', bundle_path, base_apk_path, '-f']
         else:
-            apktool_build_cmd = [self.dependencies_manager.java, '-jar', self.dependencies_manager.apktool, 'b', '-o', target_file, base_apk_path, '-f']
+            apktool_build_cmd = [self.dependencies_manager.java, '-jar',
+                                 self.dependencies_manager.apktool, 'b', '-o', target_file, base_apk_path, '-f']
         if use_aapt2:
             apktool_build_cmd.append('--use-aapt2')
 
         subprocess.check_output(apktool_build_cmd)
         if bundle_path:
             bundle_dir = os.path.dirname(bundle_path)
             self.sign_and_zipalign(bundle_dir)
@@ -703,16 +777,18 @@
 
         if bundle_path:
             bundle_dir_path = os.path.dirname(bundle_path)
             with zipfile.ZipFile(target_file, 'w', zipfile.ZIP_DEFLATED) as zip:
                 for foldername, subfolders, filenames in os.walk(bundle_dir_path):
                     for filename in filenames:
                         absolute_path = os.path.join(foldername, filename)
-                        relative_path = os.path.relpath(absolute_path, bundle_dir_path)  # use relative path
-                        zip.write(absolute_path, arcname=relative_path)  # remove folder hierarchy
+                        relative_path = os.path.relpath(
+                            absolute_path, bundle_dir_path)  # use relative path
+                        # remove folder hierarchy
+                        zip.write(absolute_path, arcname=relative_path)
 
         return target_file
 
     def create_security_config_xml(self, base_path):
         res_path = os.path.join(base_path, 'res')
 
         # Probably this if statement will never be reached
@@ -727,20 +803,23 @@
             self.print_info('res/xml path not found. Creating one...')
 
             os.makedirs(xml_path)
 
         netsec_path = os.path.join(xml_path, 'network_security_config.xml')
 
         if os.path.isfile(netsec_path):
-            self.print_warn('The network_security_config.xml file already exists!')
-            self.print_warn('I will try to delete it and create a new one. This can introduce some bug!')
+            self.print_warn(
+                'The network_security_config.xml file already exists!')
+            self.print_warn(
+                'I will try to delete it and create a new one. This can introduce some bug!')
 
             with open(netsec_path, 'r') as netsec_file:
                 contents = netsec_file.read()
-                self.print_warn('Original network_security_config.xml file content:\n{0}'.format(contents))
+                self.print_warn(
+                    'Original network_security_config.xml file content:\n{0}'.format(contents))
 
             os.remove(netsec_path)
 
         with open(netsec_path, 'w') as netsec_file:
             security_content = '''<?xml version="1.0" encoding="utf-8"?>
 <network-security-config>
 <base-config cleartextTrafficPermitted="true">
@@ -753,67 +832,75 @@
             '''
 
             netsec_file.write(security_content)
 
         self.print_info('The network_security_config.xml file was created!')
 
     def inject_user_certificates_label(self, base_dir):
-        self.print_info('Injecting Network Security label to accept user certificates...')
+        self.print_info(
+            'Injecting Network Security label to accept user certificates...')
 
         manifest_path = os.path.join(base_dir, 'AndroidManifest.xml')
 
         if not os.path.isfile(manifest_path):
-            self.print_warn("Couldn't find the Manifest file. Something is wrong with the apk!")
+            self.print_warn(
+                "Couldn't find the Manifest file. Something is wrong with the apk!")
 
             return False
 
         with open(manifest_path, 'r') as manifest_file:
             manifest_content = manifest_file.read()
 
             start_application_tag = manifest_content.find('<application ')
-            end_application_tag = manifest_content.find('>', start_application_tag)
+            end_application_tag = manifest_content.find(
+                '>', start_application_tag)
 
         new_manifest = manifest_content[:end_application_tag]
         new_manifest += ' android:networkSecurityConfig="@xml/network_security_config"'
         new_manifest += manifest_content[end_application_tag:]
 
         with open(manifest_path, 'w') as manifest_file:
             manifest_file.write(new_manifest)
 
         self.print_info('The Network Security label was added!')
 
     def has_user_certificates_label(self, base_path):
         manifest_path = os.path.join(base_path, 'AndroidManifest.xml')
 
         if not os.path.isfile(manifest_path):
-            self.print_warn("Couldn't find the Manifest file. Something is wrong with the apk!")
+            self.print_warn(
+                "Couldn't find the Manifest file. Something is wrong with the apk!")
 
             return False
 
         with open(manifest_path, 'r') as manifest_file:
             manifest_content = manifest_file.read()
 
-            has_netsec_label = manifest_content.find('network_security_config') != -1
+            has_netsec_label = manifest_content.find(
+                'network_security_config') != -1
 
         return has_netsec_label
 
     def enable_user_certificates(self, base_path):
         if not self.has_user_certificates_label(base_path):
             self.inject_user_certificates_label(base_path)
 
         self.create_security_config_xml(base_path)
 
     def inject_permission_manifest(self, base_dir, permission):
-        self.print_info('Injecting permission {0} in Manifest...'.format(permission))
+        self.print_info(
+            'Injecting permission {0} in Manifest...'.format(permission))
 
-        permission_tag = '<uses-permission android:name="{0}"/>'.format(permission)
+        permission_tag = '<uses-permission android:name="{0}"/>'.format(
+            permission)
         manifest_path = os.path.join(base_dir, 'AndroidManifest.xml')
 
         if not os.path.isfile(manifest_path):
-            self.print_warn("Couldn't find the Manifest file. Something is wrong with the apk!")
+            self.print_warn(
+                "Couldn't find the Manifest file. Something is wrong with the apk!")
 
             return False
 
         f = open(manifest_path, 'r')
         manifest_content = f.read()
         f.close()
 
@@ -837,57 +924,71 @@
         new_manifest += manifest_content[end_manifest_tag + 1:]
 
         f = open(manifest_path, 'w')
         f.write(new_manifest)
         f.close()
 
     def get_codeshare(self, uri):
+        if uri.endswith('/'):
+            uri = uri[:len(uri) - 1]
         project_url = f"https://codeshare.frida.re/api/project/{uri}/"
-        target_path = os.path.join(tempfile.gettempdir(), uri.split('/', 1)[-1  ] + '.js')
+        target_path = os.path.join(
+            tempfile.gettempdir(), uri.split('/', 1)[-1] + '.js')
         self.download_file(project_url, target_path)
         with open(target_path, 'r') as js:
             content = json.loads(js.read())
         with open(target_path, 'w') as js:
             js.write(content['source'])
         return target_path
-    
+
     def remove_old_signature(self, apkfile):
         tmp_zip = os.path.join(os.path.dirname(apkfile), 'tmp.zip')
         with zipfile.ZipFile(apkfile, 'r') as zin:
             with zipfile.ZipFile(tmp_zip, 'w') as zout:
                 for item in zin.infolist():
                     if not str(item.filename).startswith('META-INF'):
                         zout.writestr(item.filename, zin.read(item))
         os.remove(apkfile)
         os.rename(tmp_zip, apkfile)
 
     def sign_and_zipalign(self, apk_path):
-        self.print_info('Signing apk files...')  
+        self.print_info('Signing apk files...')
 
-        subprocess.call('{0} -jar {1} -a {2} --allowResign --overwrite'.format(self.dependencies_manager.java, self.dependencies_manager.uber_apk_signer, apk_path), shell=True, stdout=subprocess.DEVNULL)
+        subprocess.call('{0} -jar {1} -a {2} --allowResign --overwrite'.format(self.dependencies_manager.java,
+                        self.dependencies_manager.uber_apk_signer, apk_path), shell=True, stdout=subprocess.DEVNULL)
         idsig_files = Path(apk_path).glob('*.idsig')
         for i in idsig_files:
             os.remove(i)
 
         self.print_info('The APK files were signed and optimized!')
 
+    def get_frida_version(self):
+        if self.dependencies_manager.frida:
+            return subprocess.check_output([self.dependencies_manager.frida, '--version']).strip().decode('utf-8')
+        self.print_info(
+            'Frida not installed. Using latest version from github')
+        release_uri = f"https://api.github.com/repos/frida/frida/releases/latest"
+        response = requests.get(release_uri)
+        json = response.json()
+        return json['tag_name']
+
     @staticmethod
     def get_int_frida_version(str_version):
         version_split = str_version.split('.')
 
         if len(version_split) > 3:
             version_split = version_split[0:3]
 
         while len(version_split) < 3:
             version_split.append('0')
 
         return int(''.join(["{num:03d}".format(num=int(i)) for i in version_split]))
 
     def min_frida_version(self, min_version):
-        frida_version = subprocess.check_output([self.dependencies_manager.frida, '--version']).strip().decode('utf-8')
+        frida_version = self.get_frida_version()
 
         if self.get_int_frida_version(frida_version) < self.get_int_frida_version(min_version):
             return False
 
         return True
 
     def get_default_config_file(self):
@@ -908,234 +1009,240 @@
         f.write(config)
         f.close()
 
         return path
 
 
 def signal_handler(_signal_id, _frame):
-    print('\n' + BColors.COLOR_RED + 'YOU PRESSED CTRL+C! Exiting now...' + BColors.ENDC)
+    print('\n' + BColors.COLOR_RED +
+          'YOU PRESSED CTRL+C! Exiting now...' + BColors.ENDC)
 
     sys.exit(1)
 
 
 # noinspection SpellCheckingInspection
 def main():
     patcher = Patcher()
 
     parser = argparse.ArgumentParser()
-    parser.add_argument('-a', '--apk', help='Specify the apk you want to patch')
+    parser.add_argument(
+        '-a', '--apk', help='Specify the apk you want to patch')
     parser.add_argument('-g', '--gadget', help='Specify the frida-gadget file')
-    parser.add_argument('--arch', help='Force architecture to inject frida gadget for. Supported arches: arm64-v8a, arm64, x86, x86_64')
+    parser.add_argument(
+        '--arch', help='Force architecture to inject frida gadget for. Supported arches: arm64-v8a, arm64, x86, x86_64')
     parser.add_argument('--autoload-script', help='Auto load script')
     parser.add_argument("--codeshare", help='Auto load script from codeshare')
-    parser.add_argument('-v', '--verbosity', help='Verbosity level (0 to 3). Default is 3')
-    parser.add_argument('--update-gadgets', help='Update frida-gadgets', action='store_true')
-    parser.add_argument('-r', '--no-resources', help='Do not extract resources',
-                        action='store_true')
+    parser.add_argument('-v', '--verbosity',
+                        help='Verbosity level (0 to 3). Default is 3')
+    parser.add_argument('--update-gadgets',
+                        help='Update frida-gadgets', action='store_true')
     parser.add_argument('--use-aapt2', help='Use aapt2 with apktool',
                         action='store_true')
 
     parser.add_argument('-e', '--enable-user-certificates', help='Add some configs in apk to accept user certificates',
                         action='store_true')
 
-    parser.add_argument('--prevent-frida-gadget', help='Does not insert frida gadget', action='store_true')
-    parser.add_argument('-l', '--lib', help="Inject a shared library in place of frida gadget")
+    parser.add_argument('--prevent-frida-gadget',
+                        help='Does not insert frida gadget', action='store_true')
+    parser.add_argument(
+        '-l', '--lib', help="Inject a shared library in place of frida gadget")
     parser.add_argument('-w', '--wait-before-repackage', help='Waits for your OK before repackage the apk',
                         action='store_true')
 
-    parser.add_argument('-o', '--output-file', help='Specify the output file (patched)')
+    parser.add_argument('-o', '--output-file',
+                        help='Specify the output file (patched)')
 
-    parser.add_argument('--version', help='Display information about the version', action='store_true')
+    parser.add_argument(
+        '--version', help='Display information about the version', action='store_true')
 
     group = parser.add_argument_group('Execute command before repackage')
-    group.add_argument('-x', '--exec-before-repackage', help='Specify a command to execute before repackage')
+    group.add_argument('-x', '--exec-before-repackage',
+                       help='Specify a command to execute before repackage')
 
     group.add_argument('--pass-temp-path', help='Should I pass the apk folder as parameter to your command?',
                        action='store_true')
 
     args = parser.parse_args()
 
     if len(sys.argv) == 1:
         parser.print_help()
 
         return 1
-    
+
     dependencies_manager = ExternalDependencies()
-    
+
     if args.version:
         patcher.set_verbosity(patcher.VERBOSITY_HIGH)
         patcher.print_done('apkpatcher {0}'.format(__version__))
         return 1
-    
+
     if not dependencies_manager.add_depedency('java'):
         patcher.print_warn('java is not installed')
         return 1
-    
+
     dependencies_manager.add_depedency('frida', required=False)
     dependencies_manager.add_depedency('adb', required=False)
-    
+
     if not dependencies_manager.has_satisfied_required_dependencies():
         patcher.print_warn('One or more dependencies were not satisfied.')
         return
-        
-    
+
     patcher.dependencies_manager = dependencies_manager
 
     if args.verbosity:
         patcher.set_verbosity(int(args.verbosity))
     else:
         patcher.set_verbosity(patcher.VERBOSITY_HIGH)
 
     if args.update_gadgets:
-        if dependencies_manager.frida:
-            patcher.update_apkpatcher_gadgets()
-        else:
-            patcher.print_warn('--update-gadgets disabled. (missing frida command)')
+        patcher.update_apkpatcher_gadgets()
 
         return 0
 
     if not args.apk:
         parser.print_help()
 
         return 1
 
     else:
         if not os.path.isfile(args.apk):
-            patcher.print_warn("The file {0} couldn't be found!".format(args.apk))
+            patcher.print_warn(
+                "The file {0} couldn't be found!".format(args.apk))
 
             return 1
 
     gadget_to_use = None
-    if not args.prevent_frida_gadget and dependencies_manager.frida:
+    if not args.prevent_frida_gadget:
         if args.gadget:
             gadget_to_use = args.gadget
 
         else:
             gadget_to_use = patcher.get_recommended_gadget(abi=args.arch)
 
         if gadget_to_use is None or not os.path.isfile(gadget_to_use):
             patcher.print_warn('Could not identify the gadget!')
 
             return 1
-        
+
     patcher.check_and_download_tools()
 
     # THE APK PATCHING STARTS HERE
 
     apk_file_path = args.apk
     apk_file_name = os.path.basename(apk_file_path)
     if apk_file_path.endswith('.xapk'):
         patcher.is_bundle = True
         apk_file_path = patcher.extract_bundle(apk_file_path)
     temporary_path = patcher.create_temp_folder_for_apk(apk_file_path)
 
-    has_internet_permission = False
-    if not args.prevent_frida_gadget:
-        has_internet_permission = patcher.has_permission(apk_file_path, patcher.INTERNET_PERMISSION)
+    patcher.extract_apk(apk_file_path, temporary_path, extract_resources=True)
 
-    if args.no_resources:
-        if not args.prevent_frida_gadget or args.lib:
-            patcher.print_warn('Can\'t inject frida or libraries without extracting resources. https://github.com/iBotPeaches/Apktool/issues/3081')
-            sys.exit(1)
-        if args.enable_user_certificates:
-            patcher.print_warn('Can\'t enable user certificates without extracting resources. https://github.com/iBotPeaches/Apktool/issues/3081')
-            sys.exit(1)
-        patcher.extract_apk(apk_file_path, temporary_path, extract_resources=False)
+    manifest_path = os.path.join(temporary_path, 'AndroidManifest.xml')
 
-    else:
-        patcher.extract_apk(apk_file_path, temporary_path, extract_resources=True)
+    has_internet_permission = False
+    if not args.prevent_frida_gadget:
+        has_internet_permission = patcher.has_permission(
+            manifest_path, patcher.INTERNET_PERMISSION)
 
     if not args.prevent_frida_gadget and not has_internet_permission:
-        patcher.inject_permission_manifest(temporary_path, patcher.INTERNET_PERMISSION)
+        patcher.inject_permission_manifest(
+            temporary_path, patcher.INTERNET_PERMISSION)
 
     if args.enable_user_certificates:
         patcher.enable_user_certificates(temporary_path)
 
     if not args.prevent_frida_gadget and not args.lib:
-        if not dependencies_manager.frida:
-            patcher.print_warn('Frida patching disabled. (missing frida command).')
-        else:
-            # START --[ INJECTING FRIDA LIB FILE AND SMALI CODE ]--
-            entrypoint_class = patcher.get_entrypoint_class_name(apk_file_path)
-            entrypoint_smali_path = patcher.get_entrypoint_smali_path(temporary_path, entrypoint_class)
-
-            patcher.insert_frida_loader(entrypoint_smali_path)
-
-            if args.autoload_script or args.codeshare:
-                if dependencies_manager.frida:
-                    if not patcher.min_frida_version('10.6.33'):
-                        patcher.print_warn('Autoload is not supported in this version of frida. Update it!')
-                        return 1
-                    else:
-                        patcher.print_warn('Couldn\'t fetch frida version. Autoload might not be supported on the device')
-
-                script_file = args.autoload_script or patcher.get_codeshare(args.codeshare)
-
-                if not os.path.isfile(script_file):
-                    patcher.print_warn('The script {0} was not found.'.format(script_file))
-
-                    return 1
+        # START --[ INJECTING FRIDA LIB FILE AND SMALI CODE ]--
+        entrypoint_class = patcher.get_entrypoint_class_name(manifest_path)
+        entrypoint_smali_path = patcher.get_entrypoint_smali_path(
+            temporary_path, entrypoint_class)
+
+        patcher.insert_frida_loader(entrypoint_smali_path)
+
+        if args.autoload_script or args.codeshare:
+            if not patcher.min_frida_version('10.6.33'):
+                patcher.print_warn(
+                    'Autoload is not supported in this version of frida. Update it!')
+                return 1
+
+            script_file = args.autoload_script or patcher.get_codeshare(
+                args.codeshare)
+
+            if not os.path.isfile(script_file):
+                patcher.print_warn(
+                    'The script {0} was not found.'.format(script_file))
+
+                return 1
+
+            default_config_file = patcher.get_default_config_file()
+            patcher.insert_frida_lib(temporary_path, gadget_to_use,
+                                     config_file_path=default_config_file, auto_load_script_path=script_file)
 
-                default_config_file = patcher.get_default_config_file()
-                patcher.insert_frida_lib(temporary_path, gadget_to_use,
-                                        config_file_path=default_config_file, auto_load_script_path=script_file)
-
-            else:
-                patcher.insert_frida_lib(temporary_path, gadget_to_use)
+        else:
+            patcher.insert_frida_lib(temporary_path, gadget_to_use)
             # END --[ INJECTING FRIDA LIB FILE AND SMALI CODE ]--
 
     elif args.lib:
         lib_file = args.lib
         if not os.path.isfile(lib_file):
             patcher.print_warn('Library {0} was not found.'.format(lib_file))
         lib_name, lib_ext = os.path.basename(lib_file).rsplit('.', 1)
         lib_path = os.path.abspath(args.lib)
-        entrypoint_class = patcher.get_entrypoint_class_name(apk_file_path)
+        entrypoint_class = patcher.get_entrypoint_class_name(manifest_path)
 
-        entrypoint_smali_path = patcher.get_entrypoint_smali_path(temporary_path, entrypoint_class)
+        entrypoint_smali_path = patcher.get_entrypoint_smali_path(
+            temporary_path, entrypoint_class)
         arch = patcher.get_arch(abi=args.arch)
-        patcher.insert_shared_lib(temporary_path, lib_path, lib_name + '.' + lib_ext, arch)
+        patcher.insert_shared_lib(
+            temporary_path, lib_path, lib_name + '.' + lib_ext, arch)
         patcher.insert_frida_loader(entrypoint_smali_path, lib_name)
 
     if args.wait_before_repackage:
-        patcher.print_info('Apkpatcher is waiting for your OK to repackage the apk...')
+        patcher.print_info(
+            'Apkpatcher is waiting for your OK to repackage the apk...')
 
-        answer = input(BColors.COLOR_BLUE + '[*] Are you ready? (y/N): ' + BColors.ENDC)
+        answer = input(BColors.COLOR_BLUE +
+                       '[*] Are you ready? (y/N): ' + BColors.ENDC)
 
         while answer.lower() != 'y':
-            answer = input(BColors.COLOR_BLUE + '[*] Are you ready? (y/N): ' + BColors.ENDC)
+            answer = input(BColors.COLOR_BLUE +
+                           '[*] Are you ready? (y/N): ' + BColors.ENDC)
 
     if args.exec_before_repackage:
         if args.pass_temp_path:
             if 'TMP_PATH_HERE' in args.exec_before_repackage:
-                command_to_execute = args.exec_before_repackage.replace('TMP_PATH_HERE', temporary_path)
+                command_to_execute = args.exec_before_repackage.replace(
+                    'TMP_PATH_HERE', temporary_path)
 
             else:
-                command_to_execute = '{0} {1}'.format(args.exec_before_repackage, temporary_path)
+                command_to_execute = '{0} {1}'.format(
+                    args.exec_before_repackage, temporary_path)
         else:
             command_to_execute = '{0}'.format(args.exec_before_repackage)
 
-        print(BColors.COLOR_RED + '[!] Provided shell command: {0}'.format(command_to_execute) + BColors.COLOR_ENDC)
-        answer = input(BColors.COLOR_RED + '[!] Are you sure you want to execute it? (y/N) ' + BColors.ENDC)
+        print(BColors.COLOR_RED + '[!] Provided shell command: {0}'.format(
+            command_to_execute) + BColors.COLOR_ENDC)
+        answer = input(
+            BColors.COLOR_RED + '[!] Are you sure you want to execute it? (y/N) ' + BColors.ENDC)
 
         if answer.lower() == 'y':
             patcher.print_info('Executing -> {0}'.format(command_to_execute))
             os.system(command_to_execute)
 
-
-    if not args.no_resources:
-        manifest_path = os.path.join(temporary_path, 'AndroidManifest.xml')
-        patcher.set_extract_native_libs(manifest_path)
+    patcher.set_extract_native_libs(manifest_path)
 
     if patcher.is_bundle:
-        output_file_path = patcher.repackage_apk(temporary_path, apk_file_name, target_file=args.output_file, bundle_path=apk_file_path, use_aapt2=args.use_aapt2)
+        output_file_path = patcher.repackage_apk(
+            temporary_path, apk_file_name, target_file=args.output_file, bundle_path=apk_file_path, use_aapt2=args.use_aapt2)
     else:
-        output_file_path = patcher.repackage_apk(temporary_path, apk_file_name, target_file=args.output_file, use_aapt2=args.use_aapt2)
+        output_file_path = patcher.repackage_apk(
+            temporary_path, apk_file_name, target_file=args.output_file, use_aapt2=args.use_aapt2)
 
-    patcher.print_done('The temporary folder was not deleted. Find it at {0}'.format(temporary_path))
+    patcher.print_done(
+        'The temporary folder was not deleted. Find it at {0}'.format(temporary_path))
     patcher.print_done('Your file is located at {0}.'.format(output_file_path))
 
     return 0
 
 
 if __name__ == '__main__':
     signal.signal(signal.SIGINT, signal_handler)
```

### Comparing `apkpatcher-cli-1.2.0/apkpatcher_cli.egg-info/PKG-INFO` & `apkpatcher-cli-1.3.1/apkpatcher_cli.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher-cli
-Version: 1.2.0
+Version: 1.3.1
 Summary: Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher
 Home-page: https://github.com/nitanmarcel/apkpatcher
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkpatcher-cli-1.2.0/setup.py` & `apkpatcher-cli-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
    name='apkpatcher-cli',
-   version='1.2.0',
+   version='1.3.1',
    description='Automate the task of patching an apk with frida-gadget. fork of badadaf/apkpatcher',
    author='Marcel Alexandru Nitan',
    author_email='nitan.marcel@gmail.com',
    url='https://github.com/nitanmarcel/apkpatcher',
    keywords=['FRIDA', 'APK'],
    scripts=['apkpatcher'],
    install_requires=[
```

