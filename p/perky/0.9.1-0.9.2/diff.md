# Comparing `tmp/perky-0.9.1.tar.gz` & `tmp/perky-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perky-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "perky-0.9.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `perky-0.9.1.tar` & `perky-0.9.2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0       39 2023-07-01 02:47:29.152522 perky-0.9.1/.gitignore
--rw-r--r--   0        0        0     1089 2023-07-01 02:47:29.152522 perky-0.9.1/LICENSE
--rw-r--r--   0        0        0    18661 2023-07-03 07:32:45.286025 perky-0.9.1/README.md
--rwxr-xr-x   0        0        0    12412 2023-07-03 07:34:45.666982 perky-0.9.1/perky/__init__.py
--rw-r--r--   0        0        0    13762 2023-07-03 07:25:22.474485 perky-0.9.1/perky/tokenize.py
--rw-r--r--   0        0        0     7224 2023-07-02 06:53:52.878781 perky-0.9.1/perky/transform.py
--rw-r--r--   0        0        0     4807 2023-07-02 07:03:33.843370 perky-0.9.1/perky/utility.py
--rw-r--r--   0        0        0      437 2023-07-01 02:47:29.152522 perky-0.9.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 02:47:29.156522 perky-0.9.1/tests/__init__.py
--rw-r--r--   0        0        0      969 2023-07-03 07:13:58.037000 perky-0.9.1/tests/benchmark_perky.py
--rw-r--r--   0        0        0        3 2023-07-01 02:47:29.156522 perky-0.9.1/tests/include_dict/included.pky
--rw-r--r--   0        0        0       33 2023-07-01 02:47:29.156522 perky-0.9.1/tests/include_dict/main.pky
--rw-r--r--   0        0        0        1 2023-07-01 02:47:29.156522 perky-0.9.1/tests/include_list/included.pky
--rw-r--r--   0        0        0       27 2023-07-01 02:47:29.156522 perky-0.9.1/tests/include_list/main.pky
--rw-r--r--   0        0        0      106 2023-07-01 02:47:29.156522 perky-0.9.1/tests/include_nested/included.pky
--rw-r--r--   0        0        0      190 2023-07-01 02:47:29.156522 perky-0.9.1/tests/include_nested/main.pky
--rw-r--r--   0        0        0       30 2023-07-01 02:47:29.156522 perky-0.9.1/tests/include_path/dir1/main.pky
--rw-r--r--   0        0        0        3 2023-07-01 02:47:29.156522 perky-0.9.1/tests/include_path/dir2/included.pky
--rw-r--r--   0        0        0      766 2023-07-01 02:47:29.156522 perky-0.9.1/tests/perkytestlib.py
--rw-r--r--   0        0        0      669 2023-07-01 02:49:14.953392 perky-0.9.1/tests/test_all.py
--rw-r--r--   0        0        0      214 2023-07-01 02:47:29.156522 perky-0.9.1/tests/test_input.txt
--rw-r--r--   0        0        0    13623 2023-07-03 07:38:01.608539 perky-0.9.1/tests/test_perky.py
--rw-r--r--   0        0        0     8281 2023-07-03 07:26:12.034882 perky-0.9.1/tests/test_tokenize.py
--rw-r--r--   0        0        0     2545 2023-07-02 09:36:43.836312 perky-0.9.1/tests/test_transform.py
--rw-r--r--   0        0        0     2200 2023-07-02 06:57:38.156560 perky-0.9.1/tests/test_utility.py
--rw-r--r--   0        0        0    19097 1970-01-01 00:00:00.000000 perky-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1269 2023-07-21 23:57:20.326235 perky-0.9.2/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1373 2023-07-21 23:57:20.326235 perky-0.9.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0       39 2023-07-01 02:47:29.152522 perky-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1089 2023-07-01 02:47:29.152522 perky-0.9.2/LICENSE
+-rw-r--r--   0        0        0    19920 2023-07-21 23:57:20.326235 perky-0.9.2/README.md
+-rwxr-xr-x   0        0        0    12412 2023-07-21 23:59:35.011608 perky-0.9.2/perky/__init__.py
+-rw-r--r--   0        0        0    13762 2023-07-03 07:25:22.474485 perky-0.9.2/perky/tokenize.py
+-rw-r--r--   0        0        0     7224 2023-07-02 06:53:52.878781 perky-0.9.2/perky/transform.py
+-rw-r--r--   0        0        0     4807 2023-07-02 07:03:33.843370 perky-0.9.2/perky/utility.py
+-rw-r--r--   0        0        0      747 2023-07-21 23:57:20.326235 perky-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 02:47:29.156522 perky-0.9.2/tests/__init__.py
+-rw-r--r--   0        0        0      969 2023-07-03 07:13:58.037000 perky-0.9.2/tests/benchmark_perky.py
+-rw-r--r--   0        0        0        3 2023-07-01 02:47:29.156522 perky-0.9.2/tests/include_dict/included.pky
+-rw-r--r--   0        0        0       33 2023-07-01 02:47:29.156522 perky-0.9.2/tests/include_dict/main.pky
+-rw-r--r--   0        0        0        1 2023-07-01 02:47:29.156522 perky-0.9.2/tests/include_list/included.pky
+-rw-r--r--   0        0        0       27 2023-07-01 02:47:29.156522 perky-0.9.2/tests/include_list/main.pky
+-rw-r--r--   0        0        0      106 2023-07-01 02:47:29.156522 perky-0.9.2/tests/include_nested/included.pky
+-rw-r--r--   0        0        0      190 2023-07-01 02:47:29.156522 perky-0.9.2/tests/include_nested/main.pky
+-rw-r--r--   0        0        0       30 2023-07-01 02:47:29.156522 perky-0.9.2/tests/include_path/dir1/main.pky
+-rw-r--r--   0        0        0        3 2023-07-01 02:47:29.156522 perky-0.9.2/tests/include_path/dir2/included.pky
+-rw-r--r--   0        0        0      766 2023-07-01 02:47:29.156522 perky-0.9.2/tests/perkytestlib.py
+-rw-r--r--   0        0        0      669 2023-07-01 02:49:14.953392 perky-0.9.2/tests/test_all.py
+-rw-r--r--   0        0        0      214 2023-07-01 02:47:29.156522 perky-0.9.2/tests/test_input.txt
+-rw-r--r--   0        0        0    13623 2023-07-03 07:38:01.608539 perky-0.9.2/tests/test_perky.py
+-rw-r--r--   0        0        0     8281 2023-07-03 07:26:12.034882 perky-0.9.2/tests/test_tokenize.py
+-rw-r--r--   0        0        0     2545 2023-07-02 09:36:43.836312 perky-0.9.2/tests/test_transform.py
+-rw-r--r--   0        0        0     2200 2023-07-02 06:57:38.156560 perky-0.9.2/tests/test_utility.py
+-rw-r--r--   0        0        0    20701 1970-01-01 00:00:00.000000 perky-0.9.2/PKG-INFO
```

### Comparing `perky-0.9.1/LICENSE` & `perky-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `perky-0.9.1/README.md` & `perky-0.9.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # perky
 
 ## A friendly, easy, Pythonic text file format
 
 ##### Copyright 2018-2023 by Larry Hastings
 
+[![# test badge](https://img.shields.io/github/actions/workflow/status/larryhastings/perky/test.yml?branch=master&label=test)](https://github.com/larryhastings/perky/actions/workflows/test.yml) [![# coverage badge](https://img.shields.io/github/actions/workflow/status/larryhastings/perky/coverage.yml?branch=master&label=coverage)](https://github.com/larryhastings/perky/actions/workflows/coverage.yml) [![# python versions badge](https://img.shields.io/pypi/pyversions/perky.svg?logo=python&logoColor=FBE072)](https://pypi.org/project/perky/)
 
 ### Overview
 
 Perky is a new, simple "rcfile" text file format for Python programs.
 It solves the same problem as "INI" files, "TOML" files, and "JSON"
 files, but with its own opinion about how to best solve the problem.
 
@@ -379,15 +380,17 @@
 
 Perky has a "transformation" submodule.
 The idea is, you load a Perky file,
 then run `transform` on that dictionary to
 convert the strings into native values.
 
 These functions are no longer maintained or supported,
-and will be removed before 1.0.
+are excluded from
+[coverage](https://github.com/nedbat/coveragepy)
+testing, and will be removed before 1.0.
 Why?  This part of Perky was always
 an experiment... and the experiment never really paid
 off.  There are better implementations of this idea,
 like [Marshmallow](https://marshmallow.readthedocs.io/)--you
 you should use those instead.  (If you're relying on
 this code in Perky, I encourage you to fork
 off a copy and maintain it yourself.  But I doubt
@@ -441,19 +444,37 @@
 
 ### TODO
 
 * Backslash quoting currently does "whatever your version of Python does".  Perhaps this should be explicit, and parsed by Perky itself?
 
 ### Changelog
 
+**0.9.2** *2023/07/22*
+
+Extremely minor release.  No new features or bug fixes.
+
+* Added GitHub Actions integration.  Tests and
+  coverage are run in the cloud after every checkin.
+  Thanks to [Dan Pope](https://github.com/lordmauve)
+  for gently walking me through this!
+* Fixed metadata in the `pyproject.toml` file.
+* Dropped support for Python 3.5.  (I assumed I already
+  had, but it was still listed as being supported
+  in the project metadata.)
+* Added badges for testing, coverage,
+  and supported Python versions.
+
+
 **0.9.1** *2023/07/03*
 
 * API change: the `Parser` attribute `breadcrumbs` has been
   renamed to `stack`.  It was previously undocumented anyway,
-  though has now been documented.
+  though as of 0.9.1 it's now documented.  The previous name
+  `breadcrumbs` has been kept as an alias for now, but will
+  be removed before 1.0.
 * Added the `line_number` and `source` attributes to the
   `Parser` object, for the convenience of pragma handlers.
 * Refactored `parser_include` slightly.  No change to
   functionality or behavior, just a small code cleanup pass.
 * Added a "lines per second" output metric to the
   benchmark program.
```

### Comparing `perky-0.9.1/perky/__init__.py` & `perky-0.9.2/perky/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
 OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 import ast
 from collections.abc import MutableMapping, MutableSequence, Sequence
 import os.path
 from os.path import isfile, join, normpath
 import re
 import shlex
```

### Comparing `perky-0.9.1/perky/tokenize.py` & `perky-0.9.2/perky/tokenize.py`

 * *Files identical despite different names*

### Comparing `perky-0.9.1/perky/transform.py` & `perky-0.9.2/perky/transform.py`

 * *Files identical despite different names*

### Comparing `perky-0.9.1/perky/utility.py` & `perky-0.9.2/perky/utility.py`

 * *Files identical despite different names*

### Comparing `perky-0.9.1/tests/benchmark_perky.py` & `perky-0.9.2/tests/benchmark_perky.py`

 * *Files identical despite different names*

### Comparing `perky-0.9.1/tests/perkytestlib.py` & `perky-0.9.2/tests/perkytestlib.py`

 * *Files identical despite different names*

### Comparing `perky-0.9.1/tests/test_all.py` & `perky-0.9.2/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `perky-0.9.1/tests/test_perky.py` & `perky-0.9.2/tests/test_perky.py`

 * *Files identical despite different names*

### Comparing `perky-0.9.1/tests/test_tokenize.py` & `perky-0.9.2/tests/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `perky-0.9.1/tests/test_transform.py` & `perky-0.9.2/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `perky-0.9.1/tests/test_utility.py` & `perky-0.9.2/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `perky-0.9.1/PKG-INFO` & `perky-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 Metadata-Version: 2.1
 Name: perky
-Version: 0.9.1
+Version: 0.9.2
 Summary: A simple, Pythonic file format.  Same interface as the
 Home-page: https://github.com/larryhastings/perky/
 Author: Larry Hastings
 Author-email: larry@hastings.org
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 
 # perky
 
 ## A friendly, easy, Pythonic text file format
 
 ##### Copyright 2018-2023 by Larry Hastings
 
+[![# test badge](https://img.shields.io/github/actions/workflow/status/larryhastings/perky/test.yml?branch=master&label=test)](https://github.com/larryhastings/perky/actions/workflows/test.yml) [![# coverage badge](https://img.shields.io/github/actions/workflow/status/larryhastings/perky/coverage.yml?branch=master&label=coverage)](https://github.com/larryhastings/perky/actions/workflows/coverage.yml) [![# python versions badge](https://img.shields.io/pypi/pyversions/perky.svg?logo=python&logoColor=FBE072)](https://pypi.org/project/perky/)
 
 ### Overview
 
 Perky is a new, simple "rcfile" text file format for Python programs.
 It solves the same problem as "INI" files, "TOML" files, and "JSON"
 files, but with its own opinion about how to best solve the problem.
 
@@ -392,15 +400,17 @@
 
 Perky has a "transformation" submodule.
 The idea is, you load a Perky file,
 then run `transform` on that dictionary to
 convert the strings into native values.
 
 These functions are no longer maintained or supported,
-and will be removed before 1.0.
+are excluded from
+[coverage](https://github.com/nedbat/coveragepy)
+testing, and will be removed before 1.0.
 Why?  This part of Perky was always
 an experiment... and the experiment never really paid
 off.  There are better implementations of this idea,
 like [Marshmallow](https://marshmallow.readthedocs.io/)--you
 you should use those instead.  (If you're relying on
 this code in Perky, I encourage you to fork
 off a copy and maintain it yourself.  But I doubt
@@ -454,19 +464,37 @@
 
 ### TODO
 
 * Backslash quoting currently does "whatever your version of Python does".  Perhaps this should be explicit, and parsed by Perky itself?
 
 ### Changelog
 
+**0.9.2** *2023/07/22*
+
+Extremely minor release.  No new features or bug fixes.
+
+* Added GitHub Actions integration.  Tests and
+  coverage are run in the cloud after every checkin.
+  Thanks to [Dan Pope](https://github.com/lordmauve)
+  for gently walking me through this!
+* Fixed metadata in the `pyproject.toml` file.
+* Dropped support for Python 3.5.  (I assumed I already
+  had, but it was still listed as being supported
+  in the project metadata.)
+* Added badges for testing, coverage,
+  and supported Python versions.
+
+
 **0.9.1** *2023/07/03*
 
 * API change: the `Parser` attribute `breadcrumbs` has been
   renamed to `stack`.  It was previously undocumented anyway,
-  though has now been documented.
+  though as of 0.9.1 it's now documented.  The previous name
+  `breadcrumbs` has been kept as an alias for now, but will
+  be removed before 1.0.
 * Added the `line_number` and `source` attributes to the
   `Parser` object, for the convenience of pragma handlers.
 * Refactored `parser_include` slightly.  No change to
   functionality or behavior, just a small code cleanup pass.
 * Added a "lines per second" output metric to the
   benchmark program.
```

