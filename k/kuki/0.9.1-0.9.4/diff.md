# Comparing `tmp/kuki-0.9.1.tar.gz` & `tmp/kuki-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuki-0.9.1.tar", last modified: Fri Jul 21 15:48:40 2023, max compression
+gzip compressed data, was "kuki-0.9.4.tar", last modified: Sat Jul 22 11:33:48 2023, max compression
```

## Comparing `kuki-0.9.1.tar` & `kuki-0.9.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-21 15:48:40.747237 kuki-0.9.1/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    11357 2023-05-07 13:15:07.000000 kuki-0.9.1/LICENSE
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12044 2023-07-21 15:48:40.747237 kuki-0.9.1/PKG-INFO
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      459 2023-07-20 14:47:33.000000 kuki-0.9.1/README.md
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-21 15:48:40.745237 kuki-0.9.1/kuki/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:14:38.000000 kuki-0.9.1/kuki/__init__.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1176 2023-05-20 06:39:32.000000 kuki-0.9.1/kuki/config_util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1579 2023-07-19 15:39:03.000000 kuki-0.9.1/kuki/kest.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1994 2023-07-19 16:18:20.000000 kuki-0.9.1/kuki/ktrl.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4281 2023-07-19 16:30:54.000000 kuki-0.9.1/kuki/ktrl_util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4403 2023-07-21 09:51:39.000000 kuki-0.9.1/kuki/kuki.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3774 2023-07-21 15:41:07.000000 kuki-0.9.1/kuki/package_util.py
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-21 15:48:40.747237 kuki-0.9.1/kuki/q/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-03 12:47:22.000000 kuki-0.9.1/kuki/q/__init__.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4535 2023-07-03 16:51:49.000000 kuki-0.9.1/kuki/q/cli.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     7819 2023-07-15 09:03:13.000000 kuki-0.9.1/kuki/q/kest.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      219 2023-07-19 16:35:57.000000 kuki-0.9.1/kuki/q/ktrl.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1898 2023-07-21 09:56:43.000000 kuki-0.9.1/kuki/q/kuki.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     2187 2023-07-20 15:49:50.000000 kuki-0.9.1/kuki/q/log.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1435 2023-07-15 14:20:22.000000 kuki-0.9.1/kuki/q/path.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    14401 2023-07-21 15:19:15.000000 kuki-0.9.1/kuki/registry_util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3704 2023-07-19 16:32:47.000000 kuki-0.9.1/kuki/util.py
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-21 15:48:40.746237 kuki-0.9.1/kuki.egg-info/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12044 2023-07-21 15:48:40.000000 kuki-0.9.1/kuki.egg-info/PKG-INFO
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      554 2023-07-21 15:48:40.000000 kuki-0.9.1/kuki.egg-info/SOURCES.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-21 15:48:40.000000 kuki-0.9.1/kuki.egg-info/dependency_links.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       84 2023-07-21 15:48:40.000000 kuki-0.9.1/kuki.egg-info/entry_points.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-21 15:48:40.000000 kuki-0.9.1/kuki.egg-info/not-zip-safe
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       17 2023-07-21 15:48:40.000000 kuki-0.9.1/kuki.egg-info/requires.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       10 2023-07-21 15:48:40.000000 kuki-0.9.1/kuki.egg-info/top_level.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      470 2023-07-21 15:48:40.748237 kuki-0.9.1/setup.cfg
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      315 2023-07-03 15:40:17.000000 kuki-0.9.1/setup.py
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-21 15:48:40.747237 kuki-0.9.1/test/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.9.1/test/__init__.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.9.1/test/conftest.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1423 2023-07-19 15:39:03.000000 kuki-0.9.1/test/test_kest.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    15810 2023-07-21 15:26:05.000000 kuki-0.9.1/test/test_kuki.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-22 11:33:48.663136 kuki-0.9.4/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    11357 2023-05-07 13:15:07.000000 kuki-0.9.4/LICENSE
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12044 2023-07-22 11:33:48.664136 kuki-0.9.4/PKG-INFO
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      459 2023-07-20 14:47:33.000000 kuki-0.9.4/README.md
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-22 11:33:48.661136 kuki-0.9.4/kuki/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:14:38.000000 kuki-0.9.4/kuki/__init__.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1176 2023-05-20 06:39:32.000000 kuki-0.9.4/kuki/config_util.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1579 2023-07-19 15:39:03.000000 kuki-0.9.4/kuki/kest.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1994 2023-07-19 16:18:20.000000 kuki-0.9.4/kuki/ktrl.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4652 2023-07-22 06:51:24.000000 kuki-0.9.4/kuki/ktrl_util.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4577 2023-07-22 07:28:15.000000 kuki-0.9.4/kuki/kuki.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4031 2023-07-22 05:33:03.000000 kuki-0.9.4/kuki/package_util.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-22 11:33:48.663136 kuki-0.9.4/kuki/q/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-03 12:47:22.000000 kuki-0.9.4/kuki/q/__init__.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4535 2023-07-03 16:51:49.000000 kuki-0.9.4/kuki/q/cli.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     7819 2023-07-15 09:03:13.000000 kuki-0.9.4/kuki/q/kest.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      219 2023-07-19 16:35:57.000000 kuki-0.9.4/kuki/q/ktrl.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1898 2023-07-21 09:56:43.000000 kuki-0.9.4/kuki/q/kuki.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     2187 2023-07-20 15:49:50.000000 kuki-0.9.4/kuki/q/log.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1435 2023-07-15 14:20:22.000000 kuki-0.9.4/kuki/q/path.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    18538 2023-07-22 11:32:34.000000 kuki-0.9.4/kuki/registry_util.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3704 2023-07-19 16:32:47.000000 kuki-0.9.4/kuki/util.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-22 11:33:48.662136 kuki-0.9.4/kuki.egg-info/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12044 2023-07-22 11:33:48.000000 kuki-0.9.4/kuki.egg-info/PKG-INFO
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      554 2023-07-22 11:33:48.000000 kuki-0.9.4/kuki.egg-info/SOURCES.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-22 11:33:48.000000 kuki-0.9.4/kuki.egg-info/dependency_links.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       84 2023-07-22 11:33:48.000000 kuki-0.9.4/kuki.egg-info/entry_points.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-22 11:33:48.000000 kuki-0.9.4/kuki.egg-info/not-zip-safe
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       17 2023-07-22 11:33:48.000000 kuki-0.9.4/kuki.egg-info/requires.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       10 2023-07-22 11:33:48.000000 kuki-0.9.4/kuki.egg-info/top_level.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      470 2023-07-22 11:33:48.664136 kuki-0.9.4/setup.cfg
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      315 2023-07-03 15:40:17.000000 kuki-0.9.4/setup.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-22 11:33:48.663136 kuki-0.9.4/test/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.9.4/test/__init__.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.9.4/test/conftest.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1423 2023-07-19 15:39:03.000000 kuki-0.9.4/test/test_kest.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    15810 2023-07-21 15:26:05.000000 kuki-0.9.4/test/test_kuki.py
```

### Comparing `kuki-0.9.1/LICENSE` & `kuki-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kuki-0.9.1/PKG-INFO` & `kuki-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuki
-Version: 0.9.1
+Version: 0.9.4
 Summary: K Ultimate pacKage Installer
 Author: Jo Shinonome
 License: Apache-2.0
 Keywords: q,k
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `kuki-0.9.1/kuki/config_util.py` & `kuki-0.9.4/kuki/config_util.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.1/kuki/kest.py` & `kuki-0.9.4/kuki/kest.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.1/kuki/ktrl.py` & `kuki-0.9.4/kuki/ktrl.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.1/kuki/ktrl_util.py` & `kuki-0.9.4/kuki/ktrl_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from . import config_util
 from .util import PROCESS_DEFAULT, PROFILE_DEFAULT, generate_cmd, generate_process_options
 
 logger = logging.getLogger()
 
 KTRL_PROFILE = PROFILE_DEFAULT
 KTRL_INSTANCE = {
-    "module": "",
+    "package": "",
     "version": "",
     "file": "",
     "dbPath": "",
     "args": [],
 }
 KTRL_PROCESS = KTRL_INSTANCE.copy()
 KTRL_PROCESS.update(PROCESS_DEFAULT)
@@ -41,16 +41,19 @@
         config = KTRL_PROFILE
         all_keys = set(KTRL_PROFILE.keys())
     else:
         path = Path.joinpath(
             global_process_dir if globalMode else local_process_dir,
             name + ".process.json",
         )
-        config = KTRL_INSTANCE
+        config = KTRL_INSTANCE.copy()
         all_keys = set(KTRL_PROCESS.keys())
+        if not globalMode:
+            config.pop("package")
+            config.pop("version")
 
     default_keys = set(config.keys())
     path.parent.mkdir(parents=True, exist_ok=True)
     if path.exists():
         config.update(json.loads(path.read_text()))
         for key in config.keys():
             if key not in all_keys:
@@ -62,14 +65,17 @@
 
     for key in sorted(keys):
         current_value = config.get(key, "")
         input_value = input("{} ({}): ".format(key, current_value)).strip()
         if key == "args":
             input_value = input_value.split()
         config[key] = input_value if input_value else current_value
+        if key in ["file", "package", "version"] and not config[key]:
+            logger.error(key + " cannot be empty string")
+            return
 
     config_json = json.dumps(config, indent=2)
     logger.info("About to write to {}".format(path))
     logger.info("\n" + config_json)
     proceed = input("Is this OK? (YES/no) ").strip()
     if not proceed or proceed.lower() == "yes":
         dump_json(path, config_json)
@@ -103,27 +109,33 @@
     if process_path.exists():
         process_json: dict = json.loads(process_path.read_text())
     else:
         logger.error("Not such file - {}".format(process_path))
         return
 
     if globalMode:
-        module_path = Path.joinpath(
+        package_path = Path.joinpath(
             config_util.global_kuki_root,
-            process_json.get("module"),
+            process_json.get("package"),
             process_json.get("version"),
         )
-        if not module_path.exists():
-            logger.error("Not such folder - {}".format(module_path))
+        if not package_path.exists():
+            logger.error("Not such folder - {}".format(package_path))
             return
-        os.chdir(module_path)
+        os.chdir(package_path)
     else:
-        module_path = Path.cwd()
+        package_path = Path.cwd()
+
+    file_name: str = process_json.get("file")
 
-    file_path = Path.joinpath(module_path, "src", process_json.get("file"))
+    file_path = Path.joinpath(
+        package_path,
+        "src",
+        file_name[4:] if file_name.startswith("src/") else file_name,
+    )
 
     options = generate_process_options([], process_json)
     # generate run command
     options = (
         ["-kScriptType", "ktrl"]
         + ["-file", str(file_path)]
         + ["-dbPath", process_json.get("dbPath", [])]
```

### Comparing `kuki-0.9.1/kuki/kuki.py` & `kuki-0.9.4/kuki/kuki.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,21 @@
     "--publish",
     action="store_true",
     default=False,
     help="publish a q/k package using kuki.json",
 )
 
 group.add_argument(
+    "--unpublish",
+    type=str,
+    help="unpublish a q/k package",
+)
+
+
+group.add_argument(
     "--pack",
     action="store_true",
     default=False,
     help="pack a q/k package using kuki.json",
 )
 
 group.add_argument(
@@ -140,14 +147,16 @@
         user = input("Username: ")
         password = getpass.getpass("Password: ")
         registry_util.login(user, password)
     elif args.search:
         registry_util.search_package(args.search)
     elif args.download:
         registry_util.download_entry(args.download)
+    elif args.unpublish:
+        registry_util.unpublish_package(args.unpublish)
     else:
         if args.globalMode:
             if isinstance(args.install, list):
                 registry_util.install_packages(args.install, False, True)
                 registry_util.dump_global_index()
         elif not package_util.exits():
             logger.error("kuki.json not found, use 'kuki --init' to init the package first")
```

### Comparing `kuki-0.9.1/kuki/package_util.py` & `kuki-0.9.4/kuki/package_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import logging
 import os
+import re
 from pathlib import Path
 from typing import Dict, List, TypedDict
 
 logger = logging.getLogger()
 config_file = "kuki.json"
 index_file = "kuki_index.json"
 readme_file = "README.md"
@@ -49,17 +50,20 @@
         readme_path.touch()
         readme_path.write_text("# {name}\n\n- author: {author}\n- git: {git}\n".format(**kuki))
         src_path.mkdir(parents=True, exist_ok=True)
 
 
 def init():
     dir = os.path.basename(os.getcwd())
-    package = input("package name: ({}) ".format(dir)).strip()
+    package = input("package name: ({}) ".format(dir.lower())).strip()
     if not package:
-        package = dir
+        package = dir.lower()
+
+    is_valid_name(package)
+
     description = input("description: ").strip()
     author = input("author: ").strip()
     git = input("git repository: ").strip()
     package_type = input("package type: (q)").strip()
     if not package_type:
         package_type = "q"
     if package_type not in ["q", "k", "k9"]:
@@ -127,7 +131,13 @@
     else:
         return {}
 
 
 def dump_pkg_index(kuki_index: Dict[str, Kuki]):
     with open(package_index_path, "w") as file:
         json.dump(kuki_index, file, indent=2)
+
+
+def is_valid_name(name: str) -> bool:
+    if re.fullmatch(r"(@[a-z-]+/)?[a-z-]+", name) is None:
+        logger.error("only allows lower cases(a-z) and hyphen(-) as the package name")
+        exit(1)
```

### Comparing `kuki-0.9.1/kuki/q/cli.q` & `kuki-0.9.4/kuki/q/cli.q`

 * *Files identical despite different names*

### Comparing `kuki-0.9.1/kuki/q/kest.q` & `kuki-0.9.4/kuki/q/kest.q`

 * *Files identical despite different names*

### Comparing `kuki-0.9.1/kuki/q/kuki.q` & `kuki-0.9.4/kuki/q/kuki.q`

 * *Files identical despite different names*

### Comparing `kuki-0.9.1/kuki/q/log.q` & `kuki-0.9.4/kuki/q/log.q`

 * *Files identical despite different names*

### Comparing `kuki-0.9.1/kuki/q/path.q` & `kuki-0.9.4/kuki/q/path.q`

 * *Files identical despite different names*

### Comparing `kuki-0.9.1/kuki/registry_util.py` & `kuki-0.9.4/kuki/registry_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 urllib3.disable_warnings()
 
 logger = logging.getLogger()
 config = config_util.load_config()
 registry = config.get("registry", "https://kuki.ninja/")
 token = config.get("token", "")
+user = config.get("user", "")
 
 global_cache_dir = Path.joinpath(config_util.global_kuki_root, "_cache")
 global_index_path = Path.joinpath(config_util.global_kuki_root, ".index")
 
 kuki_json = package_util.load_kuki()
 
 if global_cache_dir.exists() and not global_cache_dir.is_dir():
@@ -62,14 +63,15 @@
     headers = {"Accept": "application/json", "Content-Type": "application/json"}
     res = requests.put(user_url + user, json.dumps(payload), headers=headers, verify=False)
 
     if res.status_code == 201:
         logger.info("the user '{}' has been added".format(user))
         token = res.json()["token"]
         config_util.update_config("token", token)
+        config_util.update_config("user", user)
     else:
         logger.error("failed to add user: " + user)
         logger.error("status code: {}, error: {}".format(res.status_code, res.json()["error"]))
 
 
 def login(user: str, password: str):
     basic_auth = HTTPBasicAuth(user, password)
@@ -78,14 +80,15 @@
     res = requests.put(
         user_url + user, json.dumps(payload), headers=headers, auth=basic_auth, verify=False
     )
     if res.status_code == 201:
         logger.info("you are authenticated as '{}'".format(user))
         token = res.json()["token"]
         config_util.update_config("token", token)
+        config_util.update_config("user", user)
     else:
         logger.error("failed to authenticated as '{}'".format(user))
         logger.error("status code: {}, error: {}".format(res.status_code, res.json()["error"]))
 
 
 def search_package(package: str):
     res = requests.get(search_url.format(package), verify=False)
@@ -104,16 +107,34 @@
                 pkg["time"]["modified"],
                 pkg["dist-tags"]["latest"],
                 " ".join(pkg.get("keywords", "")),
             )
         )
 
 
+def get_publisher(pkg_name: str) -> str:
+    headers = {
+        "Authorization": "Bearer {}".format(token),
+    }
+    res = requests.get(registry + pkg_name, headers=headers, verify=False)
+    if res.status_code == 404:
+        return ""
+    else:
+        pkg = res.json()
+        latest_version = pkg["dist-tags"]["latest"]
+        return pkg["versions"][latest_version]["publisher"]
+
+
 def publish_entry():
     try:
+        if not user:
+            logger.error(
+                "run 'kuki --adduser' or 'kuki --login' first and then publish the package"
+            )
+            return
         publish_package()
     except Exception as e:
         logger.error("failed to publish")
         logger.error(e)
 
 
 def pack_package(pkg_name: str, version: str):
@@ -160,14 +181,21 @@
 
 
 def publish_package():
     kuki = package_util.load_kuki()
     pkg_name = kuki.get("name")
     version = kuki.get("version")
 
+    publisher = get_publisher(pkg_name)
+    if publisher != user:
+        logger.error("not allow to publish to other user's package")
+        return
+
+    package_util.is_valid_name(pkg_name)
+
     tar_name, tar_packed_size = pack_package(pkg_name, version)
 
     logger.info("publishing to {} with tag latest and default access".format(registry))
 
     headers = {
         "Accept": "application/json",
         "Content-Type": "application/json",
@@ -193,14 +221,15 @@
         "readme": package_util.load_readme(),
         "versions": {
             version: {
                 "_id": "{}@{}".format(pkg_name, version),
                 "name": pkg_name,
                 "description": kuki.get("package", ""),
                 "author": {"name": kuki.get("author", "unknown")},
+                "publisher": user,
                 "version": version,
                 "readme": package_util.load_readme(),
                 "dependencies": kuki.get("dependencies", {}),
                 "dist": {
                     "shasum": shasum.hexdigest(),
                     "tarball": "{}{}/-/{}".format(registry, pkg_name, tar_name),
                 },
@@ -217,14 +246,100 @@
     res = requests.put(registry + pkg_name, data=json.dumps(data), headers=headers, verify=False)
     if res.status_code != 201:
         raise Exception(
             "failed to publish package '{}' with error: {}".format(pkg_name, res.json()["error"])
         )
 
 
+def unpublish_package(pkg_id: str):
+    pkg_name, version = (pkg_id if "@" in pkg_id else pkg_id + "@").split("@")
+
+    headers = {
+        "Authorization": "Bearer {}".format(token),
+    }
+
+    res = requests.get(registry + pkg_name, headers=headers, verify=False)
+    pkg: dict = res.json()
+    if res.status_code != 200:
+        raise Exception(pkg.get("error"))
+    dist_tags: Dict[str, str] = pkg["dist-tags"]
+    latest_version = dist_tags["latest"]
+    publisher = pkg["versions"][latest_version]["publisher"]
+    if user != publisher:
+        logger.error("not allowed to unpublish other user's package")
+        return
+    all_version = pkg.get("versions", {})
+    only_version = len(all_version) == 1
+    no_version = len(all_version) == 0
+
+    if not version or no_version or (only_version and version in all_version):
+        logger.info("unpublishing package '{}'".format(pkg_name))
+        res = requests.delete(
+            registry + pkg_name + "/-rev/" + pkg.get("_rev"),
+            headers=headers,
+            verify=False,
+        )
+        if res.status_code != 201:
+            raise Exception(
+                "failed to unpublish package '{}' with error: {}, status code: {}".format(
+                    pkg_name,
+                    res.json()["error"],
+                    res.status_code,
+                )
+            )
+        logger.info("successfully unpublish package '{}'".format(pkg_name))
+    else:
+        logger.info("unpublishing package '{}@{}'".format(pkg_name, version))
+        if version not in all_version:
+            logger.error("no version:{} available".format(version))
+            return
+        dist = all_version[version]["dist"]
+        all_version.pop(version)
+
+        for tag in list(dist_tags.keys()):
+            if dist_tags[tag] == version:
+                dist_tags.pop(tag)
+        if latest_version == version:
+            dist_tags["latest"] = max(all_version)
+        pkg.pop("_revisions", None)
+        pkg.pop("_attachments", None)
+        pkg["dist-tags"] = dist_tags
+        pkg["versions"] = all_version
+        res = requests.put(
+            registry + pkg_name + "/-rev/" + pkg.get("_rev"),
+            json=pkg,
+            headers=headers,
+            verify=False,
+        )
+        if res.status_code != 201:
+            raise Exception(
+                "failed to unpublish package '{}' with error: {}, status code: {}".format(
+                    pkg_name,
+                    res.json()["error"],
+                    res.status_code,
+                )
+            )
+        new_pkg: dict = requests.get(registry + pkg_name, headers=headers, verify=False).json()
+        tarball_url = dist["tarball"]
+        res = requests.delete(
+            tarball_url + "/-rev/" + new_pkg.get("_rev"),
+            headers=headers,
+            verify=False,
+        )
+        if res.status_code != 201:
+            raise Exception(
+                "failed to unpublish package '{}' with error: {}, status code: {}".format(
+                    pkg_name,
+                    res.json()["error"],
+                    res.status_code,
+                )
+            )
+        logger.info("successfully unpublishing package '{}@{}'".format(pkg_name, version))
+
+
 def get_tar_name(name: str, version: str):
     return "{}-v{}.tgz".format(name, version)
 
 
 def get_pkg_path(name: str, version: str):
     return Path.joinpath(config_util.global_kuki_root, name, version)
```

### Comparing `kuki-0.9.1/kuki/util.py` & `kuki-0.9.4/kuki/util.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.1/kuki.egg-info/PKG-INFO` & `kuki-0.9.4/kuki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuki
-Version: 0.9.1
+Version: 0.9.4
 Summary: K Ultimate pacKage Installer
 Author: Jo Shinonome
 License: Apache-2.0
 Keywords: q,k
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `kuki-0.9.1/kuki.egg-info/SOURCES.txt` & `kuki-0.9.4/kuki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kuki-0.9.1/test/test_kest.py` & `kuki-0.9.4/test/test_kest.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.1/test/test_kuki.py` & `kuki-0.9.4/test/test_kuki.py`

 * *Files identical despite different names*

