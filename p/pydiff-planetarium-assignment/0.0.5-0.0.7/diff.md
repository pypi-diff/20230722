# Comparing `tmp/pydiff-planetarium-assignment-0.0.5.tar.gz` & `tmp/pydiff-planetarium-assignment-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiff-planetarium-assignment-0.0.5.tar", last modified: Sat Jul 22 15:38:28 2023, max compression
+gzip compressed data, was "pydiff-planetarium-assignment-0.0.7.tar", last modified: Sat Jul 22 16:44:58 2023, max compression
```

## Comparing `pydiff-planetarium-assignment-0.0.5.tar` & `pydiff-planetarium-assignment-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 15:38:28.428897 pydiff-planetarium-assignment-0.0.5/
--rw-r--r--   0 channprj   (501) staff       (20)     2298 2023-07-22 15:38:28.428780 pydiff-planetarium-assignment-0.0.5/PKG-INFO
--rw-r--r--   0 channprj   (501) staff       (20)     1860 2023-07-22 15:36:32.000000 pydiff-planetarium-assignment-0.0.5/README.md
--rw-r--r--   0 channprj   (501) staff       (20)      104 2023-07-22 14:45:33.000000 pydiff-planetarium-assignment-0.0.5/pyproject.toml
--rw-r--r--   0 channprj   (501) staff       (20)       38 2023-07-22 15:38:28.428929 pydiff-planetarium-assignment-0.0.5/setup.cfg
--rw-r--r--   0 channprj   (501) staff       (20)      770 2023-07-22 15:38:24.000000 pydiff-planetarium-assignment-0.0.5/setup.py
-drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 15:38:28.427117 pydiff-planetarium-assignment-0.0.5/src/
-drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 15:38:28.428077 pydiff-planetarium-assignment-0.0.5/src/pydiff_planetarium_assignment/
--rw-r--r--   0 channprj   (501) staff       (20)        0 2023-07-22 09:09:07.000000 pydiff-planetarium-assignment-0.0.5/src/pydiff_planetarium_assignment/__init__.py
--rw-r--r--   0 channprj   (501) staff       (20)      372 2023-07-22 13:17:36.000000 pydiff-planetarium-assignment-0.0.5/src/pydiff_planetarium_assignment/diff.py
--rw-r--r--   0 channprj   (501) staff       (20)     1418 2023-07-22 15:27:00.000000 pydiff-planetarium-assignment-0.0.5/src/pydiff_planetarium_assignment/print.py
--rwxrwxrwx   0 channprj   (501) staff       (20)     1422 2023-07-22 15:20:21.000000 pydiff-planetarium-assignment-0.0.5/src/pydiff_planetarium_assignment/pydiff.py
-drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 15:38:28.428615 pydiff-planetarium-assignment-0.0.5/src/pydiff_planetarium_assignment.egg-info/
--rw-r--r--   0 channprj   (501) staff       (20)     2298 2023-07-22 15:38:28.000000 pydiff-planetarium-assignment-0.0.5/src/pydiff_planetarium_assignment.egg-info/PKG-INFO
--rw-r--r--   0 channprj   (501) staff       (20)      436 2023-07-22 15:38:28.000000 pydiff-planetarium-assignment-0.0.5/src/pydiff_planetarium_assignment.egg-info/SOURCES.txt
--rw-r--r--   0 channprj   (501) staff       (20)        1 2023-07-22 15:38:28.000000 pydiff-planetarium-assignment-0.0.5/src/pydiff_planetarium_assignment.egg-info/dependency_links.txt
--rw-r--r--   0 channprj   (501) staff       (20)       30 2023-07-22 15:38:28.000000 pydiff-planetarium-assignment-0.0.5/src/pydiff_planetarium_assignment.egg-info/top_level.txt
+drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 16:44:58.171752 pydiff-planetarium-assignment-0.0.7/
+-rw-r--r--   0 channprj   (501) staff       (20)     2785 2023-07-22 16:44:58.171655 pydiff-planetarium-assignment-0.0.7/PKG-INFO
+-rw-r--r--   0 channprj   (501) staff       (20)     2347 2023-07-22 16:32:23.000000 pydiff-planetarium-assignment-0.0.7/README.md
+-rw-r--r--   0 channprj   (501) staff       (20)      104 2023-07-22 14:45:33.000000 pydiff-planetarium-assignment-0.0.7/pyproject.toml
+-rw-r--r--   0 channprj   (501) staff       (20)       38 2023-07-22 16:44:58.171781 pydiff-planetarium-assignment-0.0.7/setup.cfg
+-rw-r--r--   0 channprj   (501) staff       (20)      770 2023-07-22 16:44:42.000000 pydiff-planetarium-assignment-0.0.7/setup.py
+drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 16:44:58.170369 pydiff-planetarium-assignment-0.0.7/src/
+drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 16:44:58.171093 pydiff-planetarium-assignment-0.0.7/src/pydiff_planetarium_assignment/
+-rw-r--r--   0 channprj   (501) staff       (20)        0 2023-07-22 09:09:07.000000 pydiff-planetarium-assignment-0.0.7/src/pydiff_planetarium_assignment/__init__.py
+-rw-r--r--   0 channprj   (501) staff       (20)     1733 2023-07-22 16:43:08.000000 pydiff-planetarium-assignment-0.0.7/src/pydiff_planetarium_assignment/diff.py
+-rw-r--r--   0 channprj   (501) staff       (20)     1467 2023-07-22 16:41:47.000000 pydiff-planetarium-assignment-0.0.7/src/pydiff_planetarium_assignment/print.py
+-rwxrwxrwx   0 channprj   (501) staff       (20)     1511 2023-07-22 16:32:46.000000 pydiff-planetarium-assignment-0.0.7/src/pydiff_planetarium_assignment/pydiff.py
+drwxr-xr-x   0 channprj   (501) staff       (20)        0 2023-07-22 16:44:58.171507 pydiff-planetarium-assignment-0.0.7/src/pydiff_planetarium_assignment.egg-info/
+-rw-r--r--   0 channprj   (501) staff       (20)     2785 2023-07-22 16:44:58.000000 pydiff-planetarium-assignment-0.0.7/src/pydiff_planetarium_assignment.egg-info/PKG-INFO
+-rw-r--r--   0 channprj   (501) staff       (20)      436 2023-07-22 16:44:58.000000 pydiff-planetarium-assignment-0.0.7/src/pydiff_planetarium_assignment.egg-info/SOURCES.txt
+-rw-r--r--   0 channprj   (501) staff       (20)        1 2023-07-22 16:44:58.000000 pydiff-planetarium-assignment-0.0.7/src/pydiff_planetarium_assignment.egg-info/dependency_links.txt
+-rw-r--r--   0 channprj   (501) staff       (20)       30 2023-07-22 16:44:58.000000 pydiff-planetarium-assignment-0.0.7/src/pydiff_planetarium_assignment.egg-info/top_level.txt
```

### Comparing `pydiff-planetarium-assignment-0.0.5/PKG-INFO` & `pydiff-planetarium-assignment-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,67 @@
 Metadata-Version: 2.1
 Name: pydiff-planetarium-assignment
-Version: 0.0.5
+Version: 0.0.7
 Summary: Simple implementation of unix diff
 Home-page: https://github.com/planetarium/take-home-2023-channprj
 Author: channprj
 Author-email: chann@chann.dev
 Project-URL: Bug Tracker, https://github.com/planetarium/take-home-2023-channprj/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # take-home-2023-channprj
 
+## To do
+
+- [x] Init projects
+- [x] Split and refine codes
+- [x] Wrap as a python packages using `pyproject.toml`
+- [ ] Write pure implementation of diff
+- [x] Add more documentation
+- [ ] Refine code and structure
+- [ ] Add more options and defensive logics
+
 ## TLDR;
 
 Install package and import this.
 
 ```sh
+# Link: https://pypi.org/project/pydiff-planetarium-assignment/
 pip install pydiff-planetarium-assignment
 ```
 
 ```py
 from pydiff_planetarium_assignment.diff import new_diff
 from pydiff_planetarium_assignment.print import diff_print
 
 
-old_data = '''this
-is
-old
-sentence'''
-new_data = '''this
-is
-new
-sentence'''
+old_list = ['this\n', 'is\n', 'old\n', 'message']
+new_list = ['this\n', 'is\n', 'new\n', 'message']
 
-output = new_diff(old=old_data, new=new_data)
+output = new_diff(old_list=old_list, new_list=new_list)
 diff_print(output)  # ...or print(output)
+```
 
+```diff
+# Sample output
+---
++++
+@@ -1,4 +1,4 @@
+ this
+ is
+-old
++new
+ message
 ```
 
 ## Prerequisites
 
-- Python 3 (>= 3.11)
+- Python 3 (>= 3.8, Recommend >= 3.11)
 
 ## How to use
 
 Install Python according to your preferences. Recommend to use direnv and pyenv.
 
 And then, install dependencies like below.
 
@@ -63,44 +79,41 @@
 # ... or like this
 python ./pydiff_planetarium_assignment/pydiff.py --old_file ./samples/test.txt --new_file ./samples/test2.txt
 ```
 
 #### Arguments
 
 ```sh
-channprj@CHANN-M2:~/workspace/take-home-2023-channprj(main⚡) » ./pydiff --help
+$ ./pydiff --help
 Usage: pydiff [OPTIONS]
 
+  Reference Application for pydiff
+
 Options:
   --old_file TEXT  Original file.
   --new_file TEXT  Compare target file.
-  --experimental   Use new diff. If not set, default to use python built-in function.
+  --builtin        Use python built-in function.
   --help           Show this message and exit.
 ```
 
 ### Packages
 
 ```python
 from pydiff_planetarium_assignment.diff import new_diff
 from pydiff_planetarium_assignment.print import diff_print
 
 
-old_data = '''this
-is
-old
-sentence'''
-new_data = '''this
-is
-new
-sentence'''
+old_list = ['this\n', 'is\n', 'old\n', 'message']
+new_list = ['this\n', 'is\n', 'new\n', 'message']
 
-output = new_diff(old=old_data, new=new_data)
+output = new_diff(old_list=old_list, new_list=new_list)
 diff_print(output)  # ...or print(output)
 ```
 
 ## Reference
 
 - https://en.wikipedia.org/wiki/Diff
 - https://devocean.sk.com/blog/techBoardDetail.do?ID=163566
 - https://click.palletsprojects.com/
 - https://docs.python.org/3/library/difflib.html
 - https://stackoverflow.com/a/70599663/5254829
+- https://github.com/python/cpython/blob/main/Lib/difflib.py
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pydiff-planetarium-assignment-0.0.5/setup.py` & `pydiff-planetarium-assignment-0.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pydiff-planetarium-assignment',
-    version='0.0.5',
+    version='0.0.7',
     author='channprj',
     author_email='chann@chann.dev',
     description='Simple implementation of unix diff',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/planetarium/take-home-2023-channprj',
     project_urls={
```

### Comparing `pydiff-planetarium-assignment-0.0.5/src/pydiff_planetarium_assignment/print.py` & `pydiff-planetarium-assignment-0.0.7/src/pydiff_planetarium_assignment/print.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,16 @@
     Args:
         output (str): diff text
     '''
     for line in output:
         if line and line[0] == '+':
             print(GREEN_COLOR, end='')
             print(line, end='')
-            print(DEFAULT_COLOR)
+            print(DEFAULT_COLOR, end='')
         elif line and line[0] == '-':
             print(RED_COLOR, end='')
             print(line, end='')
-            print(DEFAULT_COLOR)
+            print(DEFAULT_COLOR, end='')
         else:
-            print(line)
+            if line:
+                print(line, end='')
     return
```

### Comparing `pydiff-planetarium-assignment-0.0.5/src/pydiff_planetarium_assignment/pydiff.py` & `pydiff-planetarium-assignment-0.0.7/src/pydiff_planetarium_assignment/pydiff.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,36 +22,43 @@
 @click.option(
     '--new_file',
     prompt='New file',
     type=str,
     help='Compare target file.',
 )
 @click.option(
-    '--experimental',
+    '--builtin',
     is_flag=True,
     type=bool,
-    help='Use new diff. If not set, default to use python built-in function.',
+    help='Use python built-in function.',
 )
 def command(
     old_file: str,
     new_file: str,
-    experimental: bool,
+    builtin: bool,
 ) -> None:
     '''Reference Application for pydiff'''
     try:
         old_file_data = ''
+        new_file_data = ''
         with open(old_file, 'r', encoding='utf-8') as _old_file:
             old_file_data = _old_file.readlines()
         with open(new_file, 'r', encoding='utf-8') as _new_file:
             new_file_data = _new_file.readlines()
 
-        if experimental:
-            output = new_diff(old=old_file_data, new=new_file_data)
+        if builtin:
+            output = built_in_diff(
+                old_list=old_file_data,
+                new_list=new_file_data,
+            )
         else:
-            output = built_in_diff(old=old_file_data, new=new_file_data)
+            output = new_diff(
+                old_list=old_file_data,
+                new_list=new_file_data,
+            )
 
         diff_print(output=output)
     except Exception as error:  # pylint: disable=broad-exception-caught
         # TODO: Use specific exceptions
         print(f'Failed to load files: {error}')
 
     return
```

### Comparing `pydiff-planetarium-assignment-0.0.5/src/pydiff_planetarium_assignment.egg-info/PKG-INFO` & `pydiff-planetarium-assignment-0.0.7/src/pydiff_planetarium_assignment.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,67 @@
 Metadata-Version: 2.1
 Name: pydiff-planetarium-assignment
-Version: 0.0.5
+Version: 0.0.7
 Summary: Simple implementation of unix diff
 Home-page: https://github.com/planetarium/take-home-2023-channprj
 Author: channprj
 Author-email: chann@chann.dev
 Project-URL: Bug Tracker, https://github.com/planetarium/take-home-2023-channprj/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # take-home-2023-channprj
 
+## To do
+
+- [x] Init projects
+- [x] Split and refine codes
+- [x] Wrap as a python packages using `pyproject.toml`
+- [ ] Write pure implementation of diff
+- [x] Add more documentation
+- [ ] Refine code and structure
+- [ ] Add more options and defensive logics
+
 ## TLDR;
 
 Install package and import this.
 
 ```sh
+# Link: https://pypi.org/project/pydiff-planetarium-assignment/
 pip install pydiff-planetarium-assignment
 ```
 
 ```py
 from pydiff_planetarium_assignment.diff import new_diff
 from pydiff_planetarium_assignment.print import diff_print
 
 
-old_data = '''this
-is
-old
-sentence'''
-new_data = '''this
-is
-new
-sentence'''
+old_list = ['this\n', 'is\n', 'old\n', 'message']
+new_list = ['this\n', 'is\n', 'new\n', 'message']
 
-output = new_diff(old=old_data, new=new_data)
+output = new_diff(old_list=old_list, new_list=new_list)
 diff_print(output)  # ...or print(output)
+```
 
+```diff
+# Sample output
+---
++++
+@@ -1,4 +1,4 @@
+ this
+ is
+-old
++new
+ message
 ```
 
 ## Prerequisites
 
-- Python 3 (>= 3.11)
+- Python 3 (>= 3.8, Recommend >= 3.11)
 
 ## How to use
 
 Install Python according to your preferences. Recommend to use direnv and pyenv.
 
 And then, install dependencies like below.
 
@@ -63,44 +79,41 @@
 # ... or like this
 python ./pydiff_planetarium_assignment/pydiff.py --old_file ./samples/test.txt --new_file ./samples/test2.txt
 ```
 
 #### Arguments
 
 ```sh
-channprj@CHANN-M2:~/workspace/take-home-2023-channprj(main⚡) » ./pydiff --help
+$ ./pydiff --help
 Usage: pydiff [OPTIONS]
 
+  Reference Application for pydiff
+
 Options:
   --old_file TEXT  Original file.
   --new_file TEXT  Compare target file.
-  --experimental   Use new diff. If not set, default to use python built-in function.
+  --builtin        Use python built-in function.
   --help           Show this message and exit.
 ```
 
 ### Packages
 
 ```python
 from pydiff_planetarium_assignment.diff import new_diff
 from pydiff_planetarium_assignment.print import diff_print
 
 
-old_data = '''this
-is
-old
-sentence'''
-new_data = '''this
-is
-new
-sentence'''
+old_list = ['this\n', 'is\n', 'old\n', 'message']
+new_list = ['this\n', 'is\n', 'new\n', 'message']
 
-output = new_diff(old=old_data, new=new_data)
+output = new_diff(old_list=old_list, new_list=new_list)
 diff_print(output)  # ...or print(output)
 ```
 
 ## Reference
 
 - https://en.wikipedia.org/wiki/Diff
 - https://devocean.sk.com/blog/techBoardDetail.do?ID=163566
 - https://click.palletsprojects.com/
 - https://docs.python.org/3/library/difflib.html
 - https://stackoverflow.com/a/70599663/5254829
+- https://github.com/python/cpython/blob/main/Lib/difflib.py
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

