# Comparing `tmp/toRST-0.0.8.tar.gz` & `tmp/toRST-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toRST-0.0.8.tar", last modified: Fri Jul 21 03:16:50 2023, max compression
+gzip compressed data, was "toRST-0.0.9.tar", last modified: Sat Jul 22 02:25:20 2023, max compression
```

## Comparing `toRST-0.0.8.tar` & `toRST-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 03:16:50.984797 toRST-0.0.8/
--rw-r--r--   0 jreyno     (501) staff       (20)     1085 2023-07-18 19:42:12.000000 toRST-0.0.8/LICENSE
--rw-r--r--   0 jreyno     (501) staff       (20)     2617 2023-07-21 03:16:50.984857 toRST-0.0.8/PKG-INFO
--rw-r--r--   0 jreyno     (501) staff       (20)     1222 2023-07-21 02:00:59.000000 toRST-0.0.8/README.md
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 03:16:50.981690 toRST-0.0.8/csv2rst/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.8/csv2rst/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)      836 2023-07-21 03:11:50.000000 toRST-0.0.8/csv2rst/csv2rst.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 03:16:50.982472 toRST-0.0.8/funcs/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.8/funcs/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)     1179 2023-07-18 16:07:34.000000 toRST-0.0.8/funcs/command.py
--rw-r--r--   0 jreyno     (501) staff       (20)      434 2023-07-21 03:14:42.000000 toRST-0.0.8/funcs/funcs.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 03:16:50.982872 toRST-0.0.8/json2rst/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.8/json2rst/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)      385 2023-07-18 16:07:34.000000 toRST-0.0.8/json2rst/json2rst.py
--rw-r--r--   0 jreyno     (501) staff       (20)      103 2023-07-18 20:40:47.000000 toRST-0.0.8/pyproject.toml
--rw-r--r--   0 jreyno     (501) staff       (20)      678 2023-07-21 03:16:50.985086 toRST-0.0.8/setup.cfg
--rw-r--r--   0 jreyno     (501) staff       (20)     1535 2023-07-21 03:16:09.000000 toRST-0.0.8/setup.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 03:16:50.983142 toRST-0.0.8/tests/
--rw-r--r--   0 jreyno     (501) staff       (20)      790 2023-07-18 16:07:34.000000 toRST-0.0.8/tests/test_toRST_toRST.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 03:16:50.983840 toRST-0.0.8/toRST/
--rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.8/toRST/__init__.py
--rw-r--r--   0 jreyno     (501) staff       (20)     2606 2023-07-21 03:15:29.000000 toRST-0.0.8/toRST/toRST.py
--rw-r--r--   0 jreyno     (501) staff       (20)      332 2023-07-21 01:49:45.000000 toRST-0.0.8/toRST/write.py
-drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-21 03:16:50.984678 toRST-0.0.8/toRST.egg-info/
--rw-r--r--   0 jreyno     (501) staff       (20)     2617 2023-07-21 03:16:50.000000 toRST-0.0.8/toRST.egg-info/PKG-INFO
--rw-r--r--   0 jreyno     (501) staff       (20)      404 2023-07-21 03:16:50.000000 toRST-0.0.8/toRST.egg-info/SOURCES.txt
--rw-r--r--   0 jreyno     (501) staff       (20)        1 2023-07-21 03:16:50.000000 toRST-0.0.8/toRST.egg-info/dependency_links.txt
--rw-r--r--   0 jreyno     (501) staff       (20)       44 2023-07-21 03:16:50.000000 toRST-0.0.8/toRST.egg-info/entry_points.txt
--rw-r--r--   0 jreyno     (501) staff       (20)       29 2023-07-21 03:16:50.000000 toRST-0.0.8/toRST.egg-info/top_level.txt
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-22 02:25:20.261047 toRST-0.0.9/
+-rw-r--r--   0 jreyno     (501) staff       (20)     1085 2023-07-18 19:42:12.000000 toRST-0.0.9/LICENSE
+-rw-r--r--   0 jreyno     (501) staff       (20)     2702 2023-07-22 02:25:20.261107 toRST-0.0.9/PKG-INFO
+-rw-r--r--   0 jreyno     (501) staff       (20)     1305 2023-07-22 02:23:35.000000 toRST-0.0.9/README.md
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-22 02:25:20.258109 toRST-0.0.9/csv2rst/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.9/csv2rst/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      836 2023-07-21 03:11:50.000000 toRST-0.0.9/csv2rst/csv2rst.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-22 02:25:20.258920 toRST-0.0.9/funcs/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.9/funcs/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)     1179 2023-07-18 16:07:34.000000 toRST-0.0.9/funcs/command.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      898 2023-07-22 02:23:35.000000 toRST-0.0.9/funcs/funcs.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-22 02:25:20.259250 toRST-0.0.9/json2rst/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.9/json2rst/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      385 2023-07-18 16:07:34.000000 toRST-0.0.9/json2rst/json2rst.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      103 2023-07-18 20:40:47.000000 toRST-0.0.9/pyproject.toml
+-rw-r--r--   0 jreyno     (501) staff       (20)      678 2023-07-22 02:25:20.261369 toRST-0.0.9/setup.cfg
+-rw-r--r--   0 jreyno     (501) staff       (20)     1620 2023-07-22 02:23:35.000000 toRST-0.0.9/setup.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-22 02:25:20.259551 toRST-0.0.9/tests/
+-rw-r--r--   0 jreyno     (501) staff       (20)     1465 2023-07-22 02:23:35.000000 toRST-0.0.9/tests/test_toRST_toRST.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-22 02:25:20.260008 toRST-0.0.9/toRST/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-18 16:07:34.000000 toRST-0.0.9/toRST/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)     2654 2023-07-22 02:23:35.000000 toRST-0.0.9/toRST/toRST.py
+-rw-r--r--   0 jreyno     (501) staff       (20)      332 2023-07-21 01:49:45.000000 toRST-0.0.9/toRST/write.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-22 02:25:20.260929 toRST-0.0.9/toRST.egg-info/
+-rw-r--r--   0 jreyno     (501) staff       (20)     2702 2023-07-22 02:25:20.000000 toRST-0.0.9/toRST.egg-info/PKG-INFO
+-rw-r--r--   0 jreyno     (501) staff       (20)      404 2023-07-22 02:25:20.000000 toRST-0.0.9/toRST.egg-info/SOURCES.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)        1 2023-07-22 02:25:20.000000 toRST-0.0.9/toRST.egg-info/dependency_links.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)       44 2023-07-22 02:25:20.000000 toRST-0.0.9/toRST.egg-info/entry_points.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)       29 2023-07-22 02:25:20.000000 toRST-0.0.9/toRST.egg-info/top_level.txt
```

### Comparing `toRST-0.0.8/LICENSE` & `toRST-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `toRST-0.0.8/PKG-INFO` & `toRST-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toRST
-Version: 0.0.8
+Version: 0.0.9
 Summary: Command line tool for converting CSV and JSON files into reStructuredText Tables.
 Home-page: https://github.com/jrey999/toRST
 Author: John Reynolds
 Author-email: reynoldsjohngreg@gmail.com
 License: The MIT License (MIT)
         Copyright © 2023 John Reynolds
         
@@ -16,15 +16,15 @@
 Project-URL: Bug Tracker, https://github.com/jrey999/toRST/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-=====
+==========================================================================================
 <br>toRST
 =====
 
 Convert various data formats to reStructuredText tables.
 
 **Currently supports**:
 ----------------------
```

### Comparing `toRST-0.0.8/README.md` & `toRST-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-=====
+==========================================================================================
 <br>toRST
 =====
 
 Convert various data formats to reStructuredText tables.
 
 **Currently supports**:
 ----------------------
@@ -12,15 +12,15 @@
 
 **Planned formats**:
 
 
 - Excel<br><br>
 
 **installation**
-[PyPI](https://pypi.org/project/toRST/0.0.1/)<br>
+[PyPI](https://pypi.org/project/toRST/)<br>
 ```bash
 pip install toRST
 ```
 <br>
 
 **CLI Usage**
 -------------
@@ -49,14 +49,14 @@
   
 Import Table class
 ```python
 from toRST.toRST import Table
 ```
 Convert file1.csv into RST string
 ```python
-rst_table = Table('file1').build_table()
+rst_table = Table('file1.csv').build_table()
 ```
 
 **What toRST was built for**
 ----------------------------
 
 While building [mlb-positive-ev](https://github.com/jrey999/mlb-positive-ev), I wanted a quick and readable output of a SQLite query and couldn't find anything suitable.
```

### Comparing `toRST-0.0.8/csv2rst/csv2rst.py` & `toRST-0.0.9/csv2rst/csv2rst.py`

 * *Files identical despite different names*

### Comparing `toRST-0.0.8/funcs/command.py` & `toRST-0.0.9/funcs/command.py`

 * *Files identical despite different names*

### Comparing `toRST-0.0.8/setup.cfg` & `toRST-0.0.9/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = torst
-version = 0.0.8
+version = 0.0.9
 author = John Reynolds
 author_email = reynoldsjohngreg@gmail.com
 description = Convert various data formats to reStructuredText tables.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jrey999/toRST
 project_urls =
```

### Comparing `toRST-0.0.8/setup.py` & `toRST-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 
 readme = """
-=====
+==========================================================================================
 <br>toRST
 =====
 
 Convert various data formats to reStructuredText tables.
 
 **Currently supports**:
 ----------------------
@@ -61,15 +61,15 @@
 ```
 """.strip()
 
 with open('LICENSE') as f:
     license = f.read()
 setup(
     name='toRST',
-    version='0.0.8',
+    version='0.0.9',
     description='Command line tool for converting CSV and JSON files into reStructuredText Tables.',
     long_description=readme,
     author='John Reynolds',
     author_email='reynoldsjohngreg@gmail.com',
     url='https://github.com/jrey999/toRST',
     license=license,
     packages=find_packages(exclude=('tests',)),
```

### Comparing `toRST-0.0.8/toRST/toRST.py` & `toRST-0.0.9/toRST/toRST.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from funcs.funcs import get_extension, handle_file
+from funcs.funcs import handle_file, handle_raw
 
 
 class Table:
 
-    def __init__(self, file) -> None:
+    def __init__(self, input) -> None:
         
-        self.data = handle_file(file)
+        self.data = handle_file(input) if isinstance(input, str) else handle_raw(input)
         self.headers = self.data[0]
         self.column_widths = self.get_column_widths()
         self.page_info = self.get_page_info()
 
     def get_column_widths(self) -> dict[int, int]:
         """
         Get the maximum width for each column.
```

### Comparing `toRST-0.0.8/toRST.egg-info/PKG-INFO` & `toRST-0.0.9/toRST.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toRST
-Version: 0.0.8
+Version: 0.0.9
 Summary: Command line tool for converting CSV and JSON files into reStructuredText Tables.
 Home-page: https://github.com/jrey999/toRST
 Author: John Reynolds
 Author-email: reynoldsjohngreg@gmail.com
 License: The MIT License (MIT)
         Copyright © 2023 John Reynolds
         
@@ -16,15 +16,15 @@
 Project-URL: Bug Tracker, https://github.com/jrey999/toRST/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-=====
+==========================================================================================
 <br>toRST
 =====
 
 Convert various data formats to reStructuredText tables.
 
 **Currently supports**:
 ----------------------
```

