# Comparing `tmp/alfred-workflow-packager-2.0.1.tar.gz` & `tmp/alfred-workflow-packager-3.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred-workflow-packager-2.0.1.tar", last modified: Sat May  7 02:38:31 2022, max compression
+gzip compressed data, was "alfred-workflow-packager-3.0.0b5.tar", last modified: Sat Jul 22 20:26:18 2023, max compression
```

## Comparing `alfred-workflow-packager-2.0.1.tar` & `alfred-workflow-packager-3.0.0b5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 caleb      (501) staff       (20)        0 2022-05-07 02:38:31.823876 alfred-workflow-packager-2.0.1/
--rw-r--r--   0 caleb      (501) staff       (20)     1083 2022-03-26 23:32:11.000000 alfred-workflow-packager-2.0.1/LICENSE.txt
--rw-r--r--   0 caleb      (501) staff       (20)     4804 2022-05-07 02:38:31.823928 alfred-workflow-packager-2.0.1/PKG-INFO
--rw-r--r--   0 caleb      (501) staff       (20)     4409 2022-03-26 23:47:40.000000 alfred-workflow-packager-2.0.1/README.md
-drwxr-xr-x   0 caleb      (501) staff       (20)        0 2022-05-07 02:38:31.823322 alfred-workflow-packager-2.0.1/alfred_workflow_packager.egg-info/
--rw-r--r--   0 caleb      (501) staff       (20)     4804 2022-05-07 02:38:31.000000 alfred-workflow-packager-2.0.1/alfred_workflow_packager.egg-info/PKG-INFO
--rw-r--r--   0 caleb      (501) staff       (20)      419 2022-05-07 02:38:31.000000 alfred-workflow-packager-2.0.1/alfred_workflow_packager.egg-info/SOURCES.txt
--rw-r--r--   0 caleb      (501) staff       (20)        1 2022-05-07 02:38:31.000000 alfred-workflow-packager-2.0.1/alfred_workflow_packager.egg-info/dependency_links.txt
--rw-r--r--   0 caleb      (501) staff       (20)       39 2022-05-07 02:38:31.000000 alfred-workflow-packager-2.0.1/alfred_workflow_packager.egg-info/entry_points.txt
--rw-r--r--   0 caleb      (501) staff       (20)       17 2022-05-07 02:38:31.000000 alfred-workflow-packager-2.0.1/alfred_workflow_packager.egg-info/requires.txt
--rw-r--r--   0 caleb      (501) staff       (20)        4 2022-05-07 02:38:31.000000 alfred-workflow-packager-2.0.1/alfred_workflow_packager.egg-info/top_level.txt
-drwxr-xr-x   0 caleb      (501) staff       (20)        0 2022-05-07 02:38:31.823690 alfred-workflow-packager-2.0.1/awp/
--rw-r--r--   0 caleb      (501) staff       (20)       38 2022-03-26 23:32:11.000000 alfred-workflow-packager-2.0.1/awp/__init__.py
-drwxr-xr-x   0 caleb      (501) staff       (20)        0 2022-05-07 02:38:31.823789 alfred-workflow-packager-2.0.1/awp/data/
--rw-r--r--   0 caleb      (501) staff       (20)      843 2021-01-17 04:52:27.000000 alfred-workflow-packager-2.0.1/awp/data/config-schema.json
--rw-r--r--   0 caleb      (501) staff       (20)     1335 2022-03-26 23:32:11.000000 alfred-workflow-packager-2.0.1/awp/main.py
--rwxr-xr-x   0 caleb      (501) staff       (20)     9021 2022-05-07 02:33:10.000000 alfred-workflow-packager-2.0.1/awp/packager.py
--rw-r--r--   0 caleb      (501) staff       (20)      399 2022-03-26 23:32:11.000000 alfred-workflow-packager-2.0.1/awp/validator.py
--rw-r--r--   0 caleb      (501) staff       (20)       79 2022-05-07 02:38:31.824105 alfred-workflow-packager-2.0.1/setup.cfg
--rw-r--r--   0 caleb      (501) staff       (20)      918 2022-05-07 02:37:00.000000 alfred-workflow-packager-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:26:18.967415 alfred-workflow-packager-3.0.0b5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-22 20:26:03.000000 alfred-workflow-packager-3.0.0b5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-22 20:26:18.967415 alfred-workflow-packager-3.0.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-22 20:26:03.000000 alfred-workflow-packager-3.0.0b5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:26:18.967415 alfred-workflow-packager-3.0.0b5/alfred_workflow_packager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-22 20:26:18.000000 alfred-workflow-packager-3.0.0b5/alfred_workflow_packager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-22 20:26:18.000000 alfred-workflow-packager-3.0.0b5/alfred_workflow_packager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 20:26:18.000000 alfred-workflow-packager-3.0.0b5/alfred_workflow_packager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 20:26:18.000000 alfred-workflow-packager-3.0.0b5/alfred_workflow_packager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-22 20:26:18.000000 alfred-workflow-packager-3.0.0b5/alfred_workflow_packager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-22 20:26:18.000000 alfred-workflow-packager-3.0.0b5/alfred_workflow_packager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:26:18.967415 alfred-workflow-packager-3.0.0b5/awp/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 20:26:03.000000 alfred-workflow-packager-3.0.0b5/awp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-22 20:26:03.000000 alfred-workflow-packager-3.0.0b5/awp/argparse_extras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-22 20:26:03.000000 alfred-workflow-packager-3.0.0b5/awp/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9375 2023-07-22 20:26:03.000000 alfred-workflow-packager-3.0.0b5/awp/packager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-22 20:26:03.000000 alfred-workflow-packager-3.0.0b5/awp/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-22 20:26:03.000000 alfred-workflow-packager-3.0.0b5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 20:26:18.967415 alfred-workflow-packager-3.0.0b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-22 20:26:03.000000 alfred-workflow-packager-3.0.0b5/setup.py
```

### Comparing `alfred-workflow-packager-2.0.1/LICENSE.txt` & `alfred-workflow-packager-3.0.0b5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alfred-workflow-packager-2.0.1/PKG-INFO` & `alfred-workflow-packager-3.0.0b5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: alfred-workflow-packager
-Version: 2.0.1
-Summary: A CLI utility for packaging and exporting Alfred workflows
-Home-page: https://github.com/caleb531/alfred-workflow-packager
-Author: Caleb Evans
-Author-email: caleb@calebevans.me
-License: MIT
-Keywords: alfred workflow package export
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Alfred Workflow Packager
 
 *Copyright 2016-2022 Caleb Evans*  
 *Released under the MIT license*
 
 Alfred Workflow Packager is a command-line utility which makes the process of
 packaging and exporting an [Alfred](https://www.alfredapp.com/) workflow
@@ -215,9 +202,7 @@
 ```
 /usr/bin/php fruit/orange.php "$@"
 ```
 
 ```
 /usr/bin/php fruit/orange.php "{query}"
 ```
-
-
```

### Comparing `alfred-workflow-packager-2.0.1/README.md` & `alfred-workflow-packager-3.0.0b5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,44 @@
+Metadata-Version: 2.1
+Name: alfred-workflow-packager
+Version: 3.0.0b5
+Summary: A CLI utility for packaging and exporting Alfred workflows
+Author-email: Caleb Evans <caleb@calebevans.me>
+Maintainer-email: Caleb Evans <caleb@calebevans.me>
+License: The MIT License (MIT)
+        
+        Copyright (c) 2016-2022 Caleb Evans
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in
+        all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+        THE SOFTWARE.
+        
+Project-URL: homepage, https://github.com/caleb531/alfred-workflow-packager
+Project-URL: documentation, https://github.com/caleb531/alfred-workflow-packager#readme
+Project-URL: repository, https://github.com/caleb531/alfred-workflow-packager
+Project-URL: changelog, https://github.com/caleb531/alfred-workflow-packager/releases
+Keywords: alfred,workflow,package,export
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Alfred Workflow Packager
 
 *Copyright 2016-2022 Caleb Evans*  
 *Released under the MIT license*
 
 Alfred Workflow Packager is a command-line utility which makes the process of
 packaging and exporting an [Alfred](https://www.alfredapp.com/) workflow
```

### Comparing `alfred-workflow-packager-2.0.1/alfred_workflow_packager.egg-info/PKG-INFO` & `alfred-workflow-packager-3.0.0b5/alfred_workflow_packager.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,41 @@
 Metadata-Version: 2.1
 Name: alfred-workflow-packager
-Version: 2.0.1
+Version: 3.0.0b5
 Summary: A CLI utility for packaging and exporting Alfred workflows
-Home-page: https://github.com/caleb531/alfred-workflow-packager
-Author: Caleb Evans
-Author-email: caleb@calebevans.me
-License: MIT
-Keywords: alfred workflow package export
-Platform: UNKNOWN
+Author-email: Caleb Evans <caleb@calebevans.me>
+Maintainer-email: Caleb Evans <caleb@calebevans.me>
+License: The MIT License (MIT)
+        
+        Copyright (c) 2016-2022 Caleb Evans
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in
+        all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+        THE SOFTWARE.
+        
+Project-URL: homepage, https://github.com/caleb531/alfred-workflow-packager
+Project-URL: documentation, https://github.com/caleb531/alfred-workflow-packager#readme
+Project-URL: repository, https://github.com/caleb531/alfred-workflow-packager
+Project-URL: changelog, https://github.com/caleb531/alfred-workflow-packager/releases
+Keywords: alfred,workflow,package,export
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Alfred Workflow Packager
 
 *Copyright 2016-2022 Caleb Evans*  
 *Released under the MIT license*
@@ -215,9 +239,7 @@
 ```
 /usr/bin/php fruit/orange.php "$@"
 ```
 
 ```
 /usr/bin/php fruit/orange.php "{query}"
 ```
-
-
```

### Comparing `alfred-workflow-packager-2.0.1/awp/main.py` & `alfred-workflow-packager-3.0.0b5/awp/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,25 +4,31 @@
 import argparse
 import json
 
 import jsonschema
 
 import awp.packager
 import awp.validator
+from awp.argparse_extras import constForNargsStar
 
 
 # Parse arguments given via command-line interface
 def parse_cli_args():
 
     parser = argparse.ArgumentParser()
     parser.add_argument(
-        '--force', '-f', action='store_true',
+        '--force', '-f',
+        action='store_true',
         help='forces the copying of all files and directories')
     parser.add_argument(
-        '--export', '-e', nargs='?', const='', default=None,
+        '--export', '-e',
+        nargs='*',
+        action=constForNargsStar,
+        const=[],
+        default=None,
         help='exports the installed workflow to the local project directory')
     parser.add_argument(
         '--version', '-v',
         help='the new version number to use for the workflow')
     return parser.parse_args()
 
 
@@ -38,15 +44,15 @@
     config = get_utility_config()
 
     try:
         awp.validator.validate_config(config)
         awp.packager.package_workflow(
             config,
             version=cli_args.version,
-            export_file=cli_args.export,
+            export_files=cli_args.export,
             force=cli_args.force)
     except jsonschema.exceptions.ValidationError as error:
         print('awp (from packager.json): {}'.format(error.message))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `alfred-workflow-packager-2.0.1/awp/packager.py` & `alfred-workflow-packager-3.0.0b5/awp/packager.py`

 * *Files 4% similar despite different names*

```diff
@@ -229,28 +229,35 @@
     create_parent_dirs(archive_path)
     with ZipFile(archive_path, 'w', compression=ZIP_DEFLATED) as zip_file:
         zip_workflow_dirs(workflow_path, zip_file)
 
 
 # Package installed workflow by copying resources from project, updating
 # README, and optionally exporting workflow
-def package_workflow(config, version, export_file, force=False):
+def package_workflow(config, version, export_files, force=False):
 
     workflow_path, info = get_installed_workflow(config['bundle_id'])
 
     copy_pkg_resources(workflow_path, config['resources'], force=force)
     if 'readme' in config:
         update_workflow_readme(info, config['readme'])
     update_workflow_version(info, version)
     plist_path = os.path.join(workflow_path, 'info.plist')
     with open(plist_path, 'rb+') as plist_file:
         plistlib.dump(info, plist_file)
 
-    if export_file == '':
-        export_file = config['export_file']
+    # Do not export anything if --export/-e option is not supplied
+    if export_files is None:
+        return
+
+    # If --export/-e is supplied but without any arguments, default to the
+    # export_files list defined in packager.json (this must match the 'const'
+    # parameter in the argument definition for --export/-e)
+    if export_files == []:
+        export_files = config.get('export_files', [])
 
-    if export_file:
+    for export_file in export_files:
         project_path = os.getcwd()
         export_workflow(workflow_path, os.path.join(
             project_path, export_file))
         print('Exported installed workflow successfully (v{})'.format(
             info['version']))
```

