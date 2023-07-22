# Comparing `tmp/eclair-cli-1.0.1.tar.gz` & `tmp/eclair-cli-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eclair-cli-1.0.1.tar", last modified: Sat Jul 22 12:14:50 2023, max compression
+gzip compressed data, was "eclair-cli-1.0.2.tar", last modified: Sat Jul 22 13:37:13 2023, max compression
```

## Comparing `eclair-cli-1.0.1.tar` & `eclair-cli-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-22 12:14:50.977448 eclair-cli-1.0.1/
--rw-r--r--   0 abhinavmir   (501) staff       (20)     2765 2023-07-22 12:14:50.977316 eclair-cli-1.0.1/PKG-INFO
--rw-r--r--   0 abhinavmir   (501) staff       (20)     2537 2023-07-22 11:27:21.000000 eclair-cli-1.0.1/README.md
-drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-22 12:14:50.976047 eclair-cli-1.0.1/eclair_cli.egg-info/
--rw-r--r--   0 abhinavmir   (501) staff       (20)     2765 2023-07-22 12:14:50.000000 eclair-cli-1.0.1/eclair_cli.egg-info/PKG-INFO
--rw-r--r--   0 abhinavmir   (501) staff       (20)      357 2023-07-22 12:14:50.000000 eclair-cli-1.0.1/eclair_cli.egg-info/SOURCES.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)        1 2023-07-22 12:14:50.000000 eclair-cli-1.0.1/eclair_cli.egg-info/dependency_links.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)       54 2023-07-22 12:14:50.000000 eclair-cli-1.0.1/eclair_cli.egg-info/entry_points.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)       12 2023-07-22 12:14:50.000000 eclair-cli-1.0.1/eclair_cli.egg-info/requires.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)        4 2023-07-22 12:14:50.000000 eclair-cli-1.0.1/eclair_cli.egg-info/top_level.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)       38 2023-07-22 12:14:50.977487 eclair-cli-1.0.1/setup.cfg
--rw-r--r--   0 abhinavmir   (501) staff       (20)      704 2023-07-22 12:14:47.000000 eclair-cli-1.0.1/setup.py
-drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-22 12:14:50.977116 eclair-cli-1.0.1/src/
--rw-r--r--   0 abhinavmir   (501) staff       (20)     4560 2023-07-17 15:40:38.000000 eclair-cli-1.0.1/src/ABI_class.py
--rw-r--r--   0 abhinavmir   (501) staff       (20)        0 2023-07-20 16:30:21.000000 eclair-cli-1.0.1/src/__init__.py
--rw-r--r--   0 abhinavmir   (501) staff       (20)     1714 2023-07-22 07:56:10.000000 eclair-cli-1.0.1/src/agg.py
--rw-r--r--   0 abhinavmir   (501) staff       (20)     2117 2023-07-22 00:04:46.000000 eclair-cli-1.0.1/src/entry.py
--rw-r--r--   0 abhinavmir   (501) staff       (20)      355 2023-07-08 15:29:28.000000 eclair-cli-1.0.1/src/get_all_files.py
--rw-r--r--   0 abhinavmir   (501) staff       (20)     3867 2023-07-22 11:58:38.000000 eclair-cli-1.0.1/src/main.py
--rw-r--r--   0 abhinavmir   (501) staff       (20)      416 2023-07-11 18:11:51.000000 eclair-cli-1.0.1/src/sol_to_json.py
--rw-r--r--   0 abhinavmir   (501) staff       (20)    10985 2023-07-22 11:31:45.000000 eclair-cli-1.0.1/src/templating_logic.py
+drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-22 13:37:13.345680 eclair-cli-1.0.2/
+-rw-r--r--   0 abhinavmir   (501) staff       (20)     2765 2023-07-22 13:37:13.345538 eclair-cli-1.0.2/PKG-INFO
+-rw-r--r--   0 abhinavmir   (501) staff       (20)     2537 2023-07-22 11:27:21.000000 eclair-cli-1.0.2/README.md
+drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-22 13:37:13.344360 eclair-cli-1.0.2/eclair_cli.egg-info/
+-rw-r--r--   0 abhinavmir   (501) staff       (20)     2765 2023-07-22 13:37:13.000000 eclair-cli-1.0.2/eclair_cli.egg-info/PKG-INFO
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      333 2023-07-22 13:37:13.000000 eclair-cli-1.0.2/eclair_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)        1 2023-07-22 13:37:13.000000 eclair-cli-1.0.2/eclair_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)       54 2023-07-22 13:37:13.000000 eclair-cli-1.0.2/eclair_cli.egg-info/entry_points.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)       12 2023-07-22 13:37:13.000000 eclair-cli-1.0.2/eclair_cli.egg-info/requires.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)        4 2023-07-22 13:37:13.000000 eclair-cli-1.0.2/eclair_cli.egg-info/top_level.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)       38 2023-07-22 13:37:13.345723 eclair-cli-1.0.2/setup.cfg
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      704 2023-07-22 13:35:17.000000 eclair-cli-1.0.2/setup.py
+drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-22 13:37:13.345336 eclair-cli-1.0.2/src/
+-rw-r--r--   0 abhinavmir   (501) staff       (20)     4560 2023-07-17 15:40:38.000000 eclair-cli-1.0.2/src/ABI_class.py
+-rw-r--r--   0 abhinavmir   (501) staff       (20)        0 2023-07-20 16:30:21.000000 eclair-cli-1.0.2/src/__init__.py
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      355 2023-07-08 15:29:28.000000 eclair-cli-1.0.2/src/get_all_files.py
+-rw-r--r--   0 abhinavmir   (501) staff       (20)     3555 2023-07-22 13:37:11.000000 eclair-cli-1.0.2/src/main.py
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      416 2023-07-11 18:11:51.000000 eclair-cli-1.0.2/src/sol_to_json.py
+-rw-r--r--   0 abhinavmir   (501) staff       (20)    10985 2023-07-22 11:31:45.000000 eclair-cli-1.0.2/src/templating_logic.py
```

### Comparing `eclair-cli-1.0.1/PKG-INFO` & `eclair-cli-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eclair-cli
-Version: 1.0.1
+Version: 1.0.2
 Summary: A tool to create library wrappers for Blockchain Business Logic code.
 Author: August Radjoe
 Author-email: atg271@gmail.com
 Description-Content-Type: text/markdown
 
 # Eclair CLI Tool
```

### Comparing `eclair-cli-1.0.1/README.md` & `eclair-cli-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `eclair-cli-1.0.1/eclair_cli.egg-info/PKG-INFO` & `eclair-cli-1.0.2/eclair_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eclair-cli
-Version: 1.0.1
+Version: 1.0.2
 Summary: A tool to create library wrappers for Blockchain Business Logic code.
 Author: August Radjoe
 Author-email: atg271@gmail.com
 Description-Content-Type: text/markdown
 
 # Eclair CLI Tool
```

### Comparing `eclair-cli-1.0.1/setup.py` & `eclair-cli-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the content of the README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='eclair-cli',
-    version='1.0.1',
+    version='1.0.2',
     author='August Radjoe',
     author_email='atg271@gmail.com',
     description='A tool to create library wrappers for Blockchain Business Logic code.',
     long_description=long_description,
     long_description_content_type="text/markdown",  # or "text/x-rst" for RST format
     packages=['src'],
     entry_points={
```

### Comparing `eclair-cli-1.0.1/src/ABI_class.py` & `eclair-cli-1.0.2/src/ABI_class.py`

 * *Files identical despite different names*

### Comparing `eclair-cli-1.0.1/src/main.py` & `eclair-cli-1.0.2/src/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -78,30 +78,25 @@
     print(conf_data)
 
 def process_arguments():
     parser = argparse.ArgumentParser(prog='eclair', description='A tool to create library wrappers for Blockchain Business Logic code.')
 
     subparsers = parser.add_subparsers(dest='command')
     init_parser = subparsers.add_parser('init', help='Initialize a new project')
+    wrap_parser = subparsers.add_parser('wrap', help='Wrap all contracts in the contracts directory into Python classes and deployers')
+    help_parser = subparsers.add_parser('help', help='Show this help message')
+
     # Add more subparsers for different commands if needed
 
     args = parser.parse_args()
 
     if args.command == 'init':
         initialize_project()
     elif args.command == '--help' or args.command == 'help' or args.command == "-h" or args.command == "--h":
-        print("Usage: eclair [optional command]")
-        print("Commands:")
-        print("  wrap\t\t\tWrap all contracts in the contracts directory into Python classes and deployers")
-        print("  init\t\t\tInitialize a new project")
-        print("  help\t\t\tShow this help message")
+        parser.print_help()
     elif args.command == "wrap":
         process_files()
     else:
-        print("Usage: eclair [optional command]")
-        print("Commands:")
-        print("  wrap\t\t\tWrap all contracts in the contracts directory into Python classes and deployers")
-        print("  init\t\t\tInitialize a new project")
-        print("  help\t\t\tShow this help message")
+        parser.print_help()
 
 if __name__ == '__main__':
     sys.exit(process_arguments())
```

### Comparing `eclair-cli-1.0.1/src/templating_logic.py` & `eclair-cli-1.0.2/src/templating_logic.py`

 * *Files identical despite different names*

