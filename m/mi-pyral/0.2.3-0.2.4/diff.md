# Comparing `tmp/mi-pyral-0.2.3.tar.gz` & `tmp/mi-pyral-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mi-pyral-0.2.3.tar", last modified: Wed Jul 12 15:53:06 2023, max compression
+gzip compressed data, was "mi-pyral-0.2.4.tar", last modified: Sat Jul 22 16:16:57 2023, max compression
```

## Comparing `mi-pyral-0.2.3.tar` & `mi-pyral-0.2.4.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 15:53:06.336936 mi-pyral-0.2.3/
--rw-r--r--   0 starr      (501) staff       (20)     1072 2023-07-12 13:36:46.000000 mi-pyral-0.2.3/LICENSE
--rw-r--r--   0 starr      (501) staff       (20)       72 2023-07-12 15:52:08.000000 mi-pyral-0.2.3/MANIFEST.in
--rw-r--r--   0 starr      (501) staff       (20)     2077 2023-07-12 15:53:06.336842 mi-pyral-0.2.3/PKG-INFO
--rw-r--r--   0 starr      (501) staff       (20)      210 2022-10-08 18:13:55.000000 mi-pyral-0.2.3/README.md
--rw-r--r--   0 starr      (501) staff       (20)      922 2023-07-12 15:52:56.000000 mi-pyral-0.2.3/pyproject.toml
--rw-r--r--   0 starr      (501) staff       (20)       38 2023-07-12 15:53:06.336969 mi-pyral-0.2.3/setup.cfg
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 15:53:06.334154 mi-pyral-0.2.3/src/
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 15:53:06.335367 mi-pyral-0.2.3/src/mi_pyral.egg-info/
--rw-r--r--   0 starr      (501) staff       (20)     2077 2023-07-12 15:53:06.000000 mi-pyral-0.2.3/src/mi_pyral.egg-info/PKG-INFO
--rw-r--r--   0 starr      (501) staff       (20)      517 2023-07-12 15:53:06.000000 mi-pyral-0.2.3/src/mi_pyral.egg-info/SOURCES.txt
--rw-r--r--   0 starr      (501) staff       (20)        1 2023-07-12 15:53:06.000000 mi-pyral-0.2.3/src/mi_pyral.egg-info/dependency_links.txt
--rw-r--r--   0 starr      (501) staff       (20)       47 2023-07-12 15:53:06.000000 mi-pyral-0.2.3/src/mi_pyral.egg-info/entry_points.txt
--rw-r--r--   0 starr      (501) staff       (20)       91 2023-07-12 15:53:06.000000 mi-pyral-0.2.3/src/mi_pyral.egg-info/requires.txt
--rw-r--r--   0 starr      (501) staff       (20)        6 2023-07-12 15:53:06.000000 mi-pyral-0.2.3/src/mi_pyral.egg-info/top_level.txt
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 15:53:06.336546 mi-pyral-0.2.3/src/pyral/
--rw-r--r--   0 starr      (501) staff       (20)       17 2023-07-12 15:52:56.000000 mi-pyral-0.2.3/src/pyral/__init__.py
--rw-r--r--   0 starr      (501) staff       (20)     1453 2023-07-12 13:36:46.000000 mi-pyral-0.2.3/src/pyral/__main__.py
--rw-r--r--   0 starr      (501) staff       (20)     1131 2023-07-12 13:36:46.000000 mi-pyral-0.2.3/src/pyral/command.py
--rw-r--r--   0 starr      (501) staff       (20)     2154 2023-07-12 15:52:08.000000 mi-pyral-0.2.3/src/pyral/database.py
--rw-r--r--   0 starr      (501) staff       (20)      726 2023-07-12 13:36:46.000000 mi-pyral-0.2.3/src/pyral/exceptions.py
--rw-r--r--   0 starr      (501) staff       (20)      807 2023-07-12 13:36:46.000000 mi-pyral-0.2.3/src/pyral/log.conf
--rw-r--r--   0 starr      (501) staff       (20)    25048 2023-07-12 15:32:41.000000 mi-pyral-0.2.3/src/pyral/relation.py
--rw-r--r--   0 starr      (501) staff       (20)    18368 2023-07-12 15:32:41.000000 mi-pyral-0.2.3/src/pyral/relvar.py
--rw-r--r--   0 starr      (501) staff       (20)      435 2023-07-12 13:36:46.000000 mi-pyral-0.2.3/src/pyral/rtypes.py
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-12 15:53:06.336668 mi-pyral-0.2.3/src/pyral/tcl_scripts/
--rw-r--r--   0 starr      (501) staff       (20)      387 2023-07-12 13:36:46.000000 mi-pyral-0.2.3/src/pyral/tcl_scripts/init_TclRAL.tcl
--rw-r--r--   0 starr      (501) staff       (20)     2110 2023-07-12 15:32:41.000000 mi-pyral-0.2.3/src/pyral/transaction.py
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-22 16:16:57.891190 mi-pyral-0.2.4/
+-rw-r--r--   0 starr      (501) staff       (20)     1072 2023-07-12 13:36:46.000000 mi-pyral-0.2.4/LICENSE
+-rw-r--r--   0 starr      (501) staff       (20)       72 2023-07-12 15:58:32.000000 mi-pyral-0.2.4/MANIFEST.in
+-rw-r--r--   0 starr      (501) staff       (20)     2077 2023-07-22 16:16:57.891095 mi-pyral-0.2.4/PKG-INFO
+-rw-r--r--   0 starr      (501) staff       (20)      210 2022-10-08 18:13:55.000000 mi-pyral-0.2.4/README.md
+-rw-r--r--   0 starr      (501) staff       (20)      922 2023-07-22 16:16:05.000000 mi-pyral-0.2.4/pyproject.toml
+-rw-r--r--   0 starr      (501) staff       (20)       38 2023-07-22 16:16:57.891221 mi-pyral-0.2.4/setup.cfg
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-22 16:16:57.888116 mi-pyral-0.2.4/src/
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-22 16:16:57.889199 mi-pyral-0.2.4/src/mi_pyral.egg-info/
+-rw-r--r--   0 starr      (501) staff       (20)     2077 2023-07-22 16:16:57.000000 mi-pyral-0.2.4/src/mi_pyral.egg-info/PKG-INFO
+-rw-r--r--   0 starr      (501) staff       (20)      562 2023-07-22 16:16:57.000000 mi-pyral-0.2.4/src/mi_pyral.egg-info/SOURCES.txt
+-rw-r--r--   0 starr      (501) staff       (20)        1 2023-07-22 16:16:57.000000 mi-pyral-0.2.4/src/mi_pyral.egg-info/dependency_links.txt
+-rw-r--r--   0 starr      (501) staff       (20)       47 2023-07-22 16:16:57.000000 mi-pyral-0.2.4/src/mi_pyral.egg-info/entry_points.txt
+-rw-r--r--   0 starr      (501) staff       (20)       91 2023-07-22 16:16:57.000000 mi-pyral-0.2.4/src/mi_pyral.egg-info/requires.txt
+-rw-r--r--   0 starr      (501) staff       (20)        6 2023-07-22 16:16:57.000000 mi-pyral-0.2.4/src/mi_pyral.egg-info/top_level.txt
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-22 16:16:57.890718 mi-pyral-0.2.4/src/pyral/
+-rw-r--r--   0 starr      (501) staff       (20)       17 2023-07-22 16:16:05.000000 mi-pyral-0.2.4/src/pyral/__init__.py
+-rw-r--r--   0 starr      (501) staff       (20)     1635 2023-07-22 16:16:05.000000 mi-pyral-0.2.4/src/pyral/__main__.py
+-rw-r--r--   0 starr      (501) staff       (20)     1131 2023-07-12 13:36:46.000000 mi-pyral-0.2.4/src/pyral/command.py
+-rw-r--r--   0 starr      (501) staff       (20)     2154 2023-07-12 15:58:32.000000 mi-pyral-0.2.4/src/pyral/database.py
+-rw-r--r--   0 starr      (501) staff       (20)      726 2023-07-12 13:36:46.000000 mi-pyral-0.2.4/src/pyral/exceptions.py
+-rw-r--r--   0 starr      (501) staff       (20)      807 2023-07-12 13:36:46.000000 mi-pyral-0.2.4/src/pyral/log.conf
+-rw-r--r--   0 starr      (501) staff       (20)      607 2023-07-22 16:16:05.000000 mi-pyral-0.2.4/src/pyral/print_table.py
+-rw-r--r--   0 starr      (501) staff       (20)    25316 2023-07-22 16:16:05.000000 mi-pyral-0.2.4/src/pyral/relation.py
+-rw-r--r--   0 starr      (501) staff       (20)    18368 2023-07-12 15:58:32.000000 mi-pyral-0.2.4/src/pyral/relvar.py
+-rw-r--r--   0 starr      (501) staff       (20)      435 2023-07-12 13:36:46.000000 mi-pyral-0.2.4/src/pyral/rtypes.py
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-22 16:16:57.890834 mi-pyral-0.2.4/src/pyral/tcl_scripts/
+-rw-r--r--   0 starr      (501) staff       (20)      387 2023-07-12 13:36:46.000000 mi-pyral-0.2.4/src/pyral/tcl_scripts/init_TclRAL.tcl
+-rw-r--r--   0 starr      (501) staff       (20)     2110 2023-07-12 15:58:32.000000 mi-pyral-0.2.4/src/pyral/transaction.py
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-22 16:16:57.890936 mi-pyral-0.2.4/tests/
+-rw-r--r--   0 starr      (501) staff       (20)      879 2023-07-22 16:16:05.000000 mi-pyral-0.2.4/tests/test_print.py
```

### Comparing `mi-pyral-0.2.3/LICENSE` & `mi-pyral-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mi-pyral-0.2.3/PKG-INFO` & `mi-pyral-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mi-pyral
-Version: 0.2.3
+Version: 0.2.4
 Summary: PyRAL Pythonic interface to TclRAL
 Author-email: Leon Starr <leon_starr@modelint.com>
 License: MIT License
         
         Copyright (c) 2019-2023 Leon Starr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mi-pyral-0.2.3/pyproject.toml` & `mi-pyral-0.2.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mi-pyral"
-version = "0.2.3"
+version = "0.2.4"
 description = "PyRAL Pythonic interface to TclRAL"
 readme = "README.md"
 authors = [{ name = "Leon Starr", email = "leon_starr@modelint.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `mi-pyral-0.2.3/src/mi_pyral.egg-info/PKG-INFO` & `mi-pyral-0.2.4/src/mi_pyral.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mi-pyral
-Version: 0.2.3
+Version: 0.2.4
 Summary: PyRAL Pythonic interface to TclRAL
 Author-email: Leon Starr <leon_starr@modelint.com>
 License: MIT License
         
         Copyright (c) 2019-2023 Leon Starr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mi-pyral-0.2.3/src/mi_pyral.egg-info/SOURCES.txt` & `mi-pyral-0.2.4/src/mi_pyral.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -10,12 +10,14 @@
 src/mi_pyral.egg-info/top_level.txt
 src/pyral/__init__.py
 src/pyral/__main__.py
 src/pyral/command.py
 src/pyral/database.py
 src/pyral/exceptions.py
 src/pyral/log.conf
+src/pyral/print_table.py
 src/pyral/relation.py
 src/pyral/relvar.py
 src/pyral/rtypes.py
 src/pyral/transaction.py
-src/pyral/tcl_scripts/init_TclRAL.tcl
+src/pyral/tcl_scripts/init_TclRAL.tcl
+tests/test_print.py
```

### Comparing `mi-pyral-0.2.3/src/pyral/__main__.py` & `mi-pyral-0.2.4/src/pyral/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     logging.config.fileConfig(fname=log_conf_path, disable_existing_loggers=False)
     return logging.getLogger(__name__)  # Create a logger for this module
 
 
 # Configure the expected parameters and actions for the argparse module
 def parse(cl_input):
     parser = argparse.ArgumentParser(description='PyRAL')
+    parser.add_argument('-T', '--test', action='store_true',
+                        help='Run print test'),
     parser.add_argument('-R', '--rebuild', action='store_true',
                         help='Rebuild the database.'),
     parser.add_argument('-D', '--debug', action='store_true',
                         help='Debug mode'),
     parser.add_argument('-V', '--version', action='store_true',
                         help='Print the current version of PyRAL')
     return parser.parse_args(cl_input)
@@ -38,15 +40,18 @@
 
     # Parse the command line args
     args = parse(sys.argv[1:])
 
     if args.version:
         # Just print the version and quit
         print(f'PyRAL version: {version}')
-        sys.exit(0)
+
+    if args.test:
+        from print_table import TableTest
+        TableTest.print_table()
 
 
     logger.info("No problemo")  # We didn't die on an exception, basically
     print("\nNo problemo")
 
 
 if __name__ == "__main__":
```

### Comparing `mi-pyral-0.2.3/src/pyral/command.py` & `mi-pyral-0.2.4/src/pyral/command.py`

 * *Files identical despite different names*

### Comparing `mi-pyral-0.2.3/src/pyral/database.py` & `mi-pyral-0.2.4/src/pyral/database.py`

 * *Files identical despite different names*

### Comparing `mi-pyral-0.2.3/src/pyral/exceptions.py` & `mi-pyral-0.2.4/src/pyral/exceptions.py`

 * *Files identical despite different names*

### Comparing `mi-pyral-0.2.3/src/pyral/log.conf` & `mi-pyral-0.2.4/src/pyral/log.conf`

 * *Files identical despite different names*

### Comparing `mi-pyral-0.2.3/src/pyral/relation.py` & `mi-pyral-0.2.4/src/pyral/relation.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,24 +303,28 @@
 
         # Construct the header dictionary
         h_items = h.strip('{').split()  # Remove the open brace and split on spaces (no spaces in TclRAL attr names)
         header = dict(zip(h_items[::2], h_items[1::2]))  # Attribute names for keys and TclRAL types for values
 
         # Construct the body list
         # Each tuple is surrounded by brackets so our first stop is to split them all out into distinct tuple strings
-        body = b.split('} {')
-        body[0] = body[0].lstrip(' {')  # Remove any preceding space or brackets from the first tuple
+        # Remove leading space and enclosing brackets from entire body
+        # 2/-2 skips over leading space and first bracket and truncates final bracket surrounding body
+        body = b[2:-2].split('} {')
+        body[0] = body[0].lstrip('{')  # Remove preceding bracket from the first tuple
+
         # Each tuple alternates with the attribute name and the attribute value
         # We want to extract just the values to create the table rows
         # To complicate matters, values may contain spaces. TclRAL attribute names do not.
         # A multi-word value is surrounded by brackets
         # So you might see a tuple like this: Floor_height 32.6 Name {Lower lobby}
         # We need a regex component that will extract the bracketed space delimited values
         # As well as the non-bracketed single word values
-        value_pattern = r"([{}<>\w ]*)"  # Grab a string of any combination of brackets, word characters and spaces
+        # value_pattern = r"([{}<>\w ]*)"  # Grab a string of any combination of brackets, word characters and spaces
+        value_pattern = r"(.*)"  # Grab the whole value string. We'll strip the brackets out later.
         # Now we build this component into an alternating pattern of attribute and value items
         # for the attributes in our relation header
         tuple_pattern = ""
         for a in header.keys():
             tuple_pattern += f"{a} {value_pattern} "
         tuple_pattern = tuple_pattern.rstrip(' ')  # Removes the final trailing space
         # Now we can use the constructed tuple pattern regex to extract a list of values
```

### Comparing `mi-pyral-0.2.3/src/pyral/relvar.py` & `mi-pyral-0.2.4/src/pyral/relvar.py`

 * *Files identical despite different names*

### Comparing `mi-pyral-0.2.3/src/pyral/transaction.py` & `mi-pyral-0.2.4/src/pyral/transaction.py`

 * *Files identical despite different names*

