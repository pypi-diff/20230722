# Comparing `tmp/classroom_extensions-0.0.4.tar.gz` & `tmp/classroom_extensions-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classroom_extensions-0.0.4.tar", last modified: Wed Jul 19 23:28:47 2023, max compression
+gzip compressed data, was "classroom_extensions-0.0.6.tar", last modified: Fri Jul 21 22:34:11 2023, max compression
```

## Comparing `classroom_extensions-0.0.4.tar` & `classroom_extensions-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:28:47.598442 classroom_extensions-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-19 23:28:37.000000 classroom_extensions-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-07-19 23:28:47.598442 classroom_extensions-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-19 23:28:37.000000 classroom_extensions-0.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:28:47.594442 classroom_extensions-0.0.4/classroom_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-19 23:28:37.000000 classroom_extensions-0.0.4/classroom_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-19 23:28:37.000000 classroom_extensions-0.0.4/classroom_extensions/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-19 23:28:37.000000 classroom_extensions-0.0.4/classroom_extensions/mariadb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-19 23:28:37.000000 classroom_extensions-0.0.4/classroom_extensions/mariadb_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-07-19 23:28:37.000000 classroom_extensions-0.0.4/classroom_extensions/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-19 23:28:37.000000 classroom_extensions-0.0.4/classroom_extensions/mongodb_install.py
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-07-19 23:28:37.000000 classroom_extensions-0.0.4/classroom_extensions/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-19 23:28:37.000000 classroom_extensions-0.0.4/classroom_extensions/plantuml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-19 23:28:37.000000 classroom_extensions-0.0.4/classroom_extensions/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:28:47.594442 classroom_extensions-0.0.4/classroom_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-07-19 23:28:47.000000 classroom_extensions-0.0.4/classroom_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-19 23:28:47.000000 classroom_extensions-0.0.4/classroom_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 23:28:47.000000 classroom_extensions-0.0.4/classroom_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-19 23:28:47.000000 classroom_extensions-0.0.4/classroom_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 23:28:47.000000 classroom_extensions-0.0.4/classroom_extensions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-19 23:28:37.000000 classroom_extensions-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 23:28:47.598442 classroom_extensions-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:28:47.594442 classroom_extensions-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-19 23:28:37.000000 classroom_extensions-0.0.4/tests/test_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-19 23:28:37.000000 classroom_extensions-0.0.4/tests/test_mariadb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-19 23:28:37.000000 classroom_extensions-0.0.4/tests/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-19 23:28:37.000000 classroom_extensions-0.0.4/tests/test_nodejs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-07-19 23:28:37.000000 classroom_extensions-0.0.4/tests/test_plantuml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:34:11.209051 classroom_extensions-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-07-21 22:34:11.209051 classroom_extensions-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:34:11.209051 classroom_extensions-0.0.6/classroom_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/classroom_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/classroom_extensions/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/classroom_extensions/mariadb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/classroom_extensions/mariadb_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/classroom_extensions/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/classroom_extensions/mongodb_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/classroom_extensions/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/classroom_extensions/plantuml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/classroom_extensions/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:34:11.209051 classroom_extensions-0.0.6/classroom_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-07-21 22:34:11.000000 classroom_extensions-0.0.6/classroom_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-21 22:34:11.000000 classroom_extensions-0.0.6/classroom_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:34:11.000000 classroom_extensions-0.0.6/classroom_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-21 22:34:11.000000 classroom_extensions-0.0.6/classroom_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-21 22:34:11.000000 classroom_extensions-0.0.6/classroom_extensions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 22:34:11.209051 classroom_extensions-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:34:11.209051 classroom_extensions-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/tests/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/tests/test_mariadb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/tests/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/tests/test_nodejs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-07-21 22:34:02.000000 classroom_extensions-0.0.6/tests/test_plantuml.py
```

### Comparing `classroom_extensions-0.0.4/LICENSE` & `classroom_extensions-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.4/PKG-INFO` & `classroom_extensions-0.0.6/classroom_extensions.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: classroom_extensions
-Version: 0.0.4
+Name: classroom-extensions
+Version: 0.0.6
 Summary: IPython extensions used for teaching
 Author-email: Marcos Dias de Assuncao <assuncao@acm.org>
 Maintainer-email: Marcos Dias de Assuncao <assuncao@acm.org>
 License: MIT
 Project-URL: Homepage, https://github.com/assuncaomarcos/classroom_extensions
 Project-URL: Bug Reports, https://github.com/assuncaomarcos/classroom_extensions
 Project-URL: Say Thanks!, https://saythanks.io/to/assuncaomarcos
@@ -28,14 +28,20 @@
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+.. image:: https://coveralls.io/repos/github/assuncaomarcos/classroom_extensions/badge.svg?branch=main
+    :target: https://coveralls.io/github/assuncaomarcos/classroom_extensions?branch=main
+
+
 IPython Extensions for Teaching
 ===============================
 
 This project provides a set of IPython extensions used for teaching at the
 Ecole de Technologie Superieure (ETS) of Montreal. The extensions work on
 Google Colab, and Jupyter notebooks with some effort, and provide a set of
 magics (e.g., `%%sql`) while customizing existing ones (e.g., `%%javascript`)
```

### Comparing `classroom_extensions-0.0.4/README.rst` & `classroom_extensions-0.0.6/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+.. image:: https://coveralls.io/repos/github/assuncaomarcos/classroom_extensions/badge.svg?branch=main
+    :target: https://coveralls.io/github/assuncaomarcos/classroom_extensions?branch=main
+
+
 IPython Extensions for Teaching
 ===============================
 
 This project provides a set of IPython extensions used for teaching at the
 Ecole de Technologie Superieure (ETS) of Montreal. The extensions work on
 Google Colab, and Jupyter notebooks with some effort, and provide a set of
 magics (e.g., `%%sql`) while customizing existing ones (e.g., `%%javascript`)
```

### Comparing `classroom_extensions-0.0.4/classroom_extensions/html.py` & `classroom_extensions-0.0.6/classroom_extensions/html.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.4/classroom_extensions/mariadb.py` & `classroom_extensions-0.0.6/classroom_extensions/mariadb.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.4/classroom_extensions/mariadb_install.py` & `classroom_extensions-0.0.6/classroom_extensions/mariadb_install.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,23 +58,24 @@
 
     @staticmethod
     def _meet_requirements() -> bool:
         """
         Check if running on Colab with the right Ubuntu release
 
         Returns:
-            True if running on Google Colab on Ubuntu 20.xx container
+            True if running on Google Colab on Ubuntu 2x.xx container
         """
-        return is_colab() and get_os_release().startswith("20.")
+        return is_colab() and get_os_release().startswith("2")
 
     @classmethod
     def _start_mariadb(cls) -> None:
         """Starts MariaDB"""
 
-        get_ipython().system_raw("service mysql start &")
+        service_name = "mariadb" if get_os_release().startswith("22") else "mysql"
+        get_ipython().system_raw(f"service {service_name} start &")
         print("Waiting for a few seconds for MariaDB server to start...")
         time.sleep(START_DB_TIMEOUT)
 
     @line_magic
     def install_mariadb(self, line: str):
         """Install MariaDB, mariadb_kernel, sqlparse, etc"""
```

### Comparing `classroom_extensions-0.0.4/classroom_extensions/mongodb.py` & `classroom_extensions-0.0.6/classroom_extensions/mongodb.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.4/classroom_extensions/mongodb_install.py` & `classroom_extensions-0.0.6/classroom_extensions/mongodb_install.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,31 +6,36 @@
 
 Note: This extension assumes that you are working in Google Colab
 running Ubuntu 20.04.
 """
 from os import path
 import os
 import glob
+import time
 from argparse import ArgumentParser
+from IPython.core.getipython import get_ipython
 from IPython.core.magic import magics_class, line_magic, Magics
 from .util import exec_cmd, get_os_release, is_colab
 
-_SOFTWARE_DESC = {"mongodb": "MongoDB", "mongodb_shell": "MongoDB Shell"}
+_START_DB_TIMEOUT = 5  # Timeout for starting MariaDB
+_SOFTWARE_DESC = {"mongo": "MongoDB"}
 
 _INSTALL_CMDS = {
-    "mongodb": ["apt update", "apt install mongodb", "service mongodb start"],
-    "mongodb_shell": [
-        "wget -qO- https://www.mongodb.org/static/pgp/server-6.0.asc |"
-        "sudo tee /etc/apt/trusted.gpg.d/server-6.0.asc",
+    "mongo": [
+        "apt update -y",
+        "apt-get install gnupg curl",
+        """curl -fsSL https://pgp.mongodb.com/server-6.0.asc | \
+             gpg -o /usr/share/keyrings/mongodb-server-6.0.gpg \
+             --dearmor""",
         "sudo apt-get install gnupg",
-        "echo 'deb [ arch=amd64,arm64 ] "
-        "https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/6.0 multiverse' | "
-        "sudo tee /etc/apt/sources.list.d/mongodb-org-6.0.list",
+        "echo 'deb [ arch=amd64,arm64 signed-by=/usr/share/keyrings/mongodb-server-6.0.gpg ] "
+        "https://repo.mongodb.org/apt/ubuntu jammy/mongodb-org/6.0 multiverse' "
+        "| tee /etc/apt/sources.list.d/mongodb-org-6.0.list",
         "sudo apt update",
-        "sudo apt install -y mongodb-mongosh",
+        "apt-get install -y mongodb-org",
     ],
 }
 
 _SAMPLE_DBS_URL = "https://github.com/neelabalan/mongodb-sample-dataset.git"
 
 
 @magics_class
@@ -61,17 +66,17 @@
 
     @staticmethod
     def _meet_requirements() -> bool:
         """
         Check if running on Colab with the right Ubuntu release
 
         Returns:
-            True if running on Google Colab on Ubuntu 20.xx container
+            True if running on Google Colab on Ubuntu 2x.xx container
         """
-        return is_colab() and get_os_release().startswith("20.")
+        return is_colab() and get_os_release().startswith("2")
 
     @staticmethod
     def install_software(software: str) -> None:
         """Installs a given software"""
         description = _SOFTWARE_DESC.get(software)
         commands = _INSTALL_CMDS.get(software)
 
@@ -90,46 +95,56 @@
         print("Cloning git repository with the sample datasets...")
         clone_path = path.join(os.getcwd(), local_clone)
         try:
             if not path.exists(clone_path):
                 exec_cmd(f"git clone {_SAMPLE_DBS_URL} {local_clone}")
             else:
                 print("Skipping git clone as local repository seems to exist.")
-                datasets = [
-                    f
-                    for f in os.listdir(local_clone)
-                    if not path.isfile(path.join(local_clone, f))
-                ]
-                for dataset in datasets:
-                    dataset_path = path.join(clone_path, dataset)
-                    print(f"Importing dataset {dataset}...")
-                    for json_file in glob.glob(f"{dataset_path}/*.json"):
-                        collection = path.splitext(path.basename(json_file))[0]
-                        cmd = (
-                            f"mongoimport --drop --host localhost --port 27017 "
-                            f"--db {dataset} --collection {collection} --file {json_file}"
-                        )
-                        exec_cmd(cmd)
+
+            datasets = [
+                f
+                for f in os.listdir(local_clone)
+                if not path.isfile(path.join(local_clone, f))
+            ]
+            for dataset in datasets:
+                dataset_path = path.join(clone_path, dataset)
+                print(f"Importing dataset {dataset}...")
+                for json_file in glob.glob(f"{dataset_path}/*.json"):
+                    collection = path.splitext(path.basename(json_file))[0]
+                    cmd = (
+                        f"mongoimport --drop --host localhost --port 27017 "
+                        f"--db {dataset} --collection {collection} --file {json_file}"
+                    )
+                    exec_cmd(cmd)
             print("Finished importing the sample datasets.")
         except RuntimeError as runtime_error:
             print(f"Error importing sample databases: {runtime_error}")
 
+    @staticmethod
+    def _start_mongodb() -> None:
+        """Starts MongoDB"""
+
+        get_ipython().system_raw("mongod --config /etc/mongod.conf &")
+        print("Waiting for a few seconds for MongoDB server to start...")
+        time.sleep(_START_DB_TIMEOUT)
+
     @line_magic
     def install_mongodb(self, line: str):
         """Install MongoDB and MongoDB Shell"""
 
         if not self._meet_requirements():
             print(
                 "Note: the magics for installing and configuring "
                 "MongoDB may not work outside Google Colab"
             )
 
         args = self._arg_parser.parse_args(line.split() if line else "")
-        self.install_software("mongodb")
-        self.install_software("mongodb_shell")
+        self.install_software("mongo")
+        self._start_mongodb()
+
         if args.sample_dbs:
             self.import_sample_datasets()
 
 
 def load_ipython_extension(ipython):
     """
     Loads the ipython extension
```

### Comparing `classroom_extensions-0.0.4/classroom_extensions/node.py` & `classroom_extensions-0.0.6/classroom_extensions/node.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.4/classroom_extensions/plantuml.py` & `classroom_extensions-0.0.6/classroom_extensions/plantuml.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.4/classroom_extensions/util.py` & `classroom_extensions-0.0.6/classroom_extensions/util.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.4/classroom_extensions.egg-info/PKG-INFO` & `classroom_extensions-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: classroom-extensions
-Version: 0.0.4
+Name: classroom_extensions
+Version: 0.0.6
 Summary: IPython extensions used for teaching
 Author-email: Marcos Dias de Assuncao <assuncao@acm.org>
 Maintainer-email: Marcos Dias de Assuncao <assuncao@acm.org>
 License: MIT
 Project-URL: Homepage, https://github.com/assuncaomarcos/classroom_extensions
 Project-URL: Bug Reports, https://github.com/assuncaomarcos/classroom_extensions
 Project-URL: Say Thanks!, https://saythanks.io/to/assuncaomarcos
@@ -28,14 +28,20 @@
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+.. image:: https://coveralls.io/repos/github/assuncaomarcos/classroom_extensions/badge.svg?branch=main
+    :target: https://coveralls.io/github/assuncaomarcos/classroom_extensions?branch=main
+
+
 IPython Extensions for Teaching
 ===============================
 
 This project provides a set of IPython extensions used for teaching at the
 Ecole de Technologie Superieure (ETS) of Montreal. The extensions work on
 Google Colab, and Jupyter notebooks with some effort, and provide a set of
 magics (e.g., `%%sql`) while customizing existing ones (e.g., `%%javascript`)
```

### Comparing `classroom_extensions-0.0.4/classroom_extensions.egg-info/SOURCES.txt` & `classroom_extensions-0.0.6/classroom_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.4/pyproject.toml` & `classroom_extensions-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.4/tests/test_html.py` & `classroom_extensions-0.0.6/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.4/tests/test_mariadb.py` & `classroom_extensions-0.0.6/tests/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.4/tests/test_mongodb.py` & `classroom_extensions-0.0.6/tests/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.4/tests/test_nodejs.py` & `classroom_extensions-0.0.6/tests/test_nodejs.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.4/tests/test_plantuml.py` & `classroom_extensions-0.0.6/tests/test_plantuml.py`

 * *Files identical despite different names*

