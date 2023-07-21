# Comparing `tmp/gncxml-0.6.9.tar.gz` & `tmp/gncxml-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gncxml-0.6.9.tar", max compression
+gzip compressed data, was "gncxml-0.7.0.tar", max compression
```

## Comparing `gncxml-0.6.9.tar` & `gncxml-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2017-12-17 01:02:32.000000 gncxml-0.6.9/LICENSE
--rw-r--r--   0        0        0     1124 2022-01-22 02:05:23.252599 gncxml-0.6.9/README.md
--rw-r--r--   0        0        0      121 2017-11-23 20:24:39.000000 gncxml-0.6.9/gncxml/__init__.py
--rw-r--r--   0        0        0       90 2021-12-27 13:53:45.410909 gncxml-0.6.9/gncxml/__main__.py
--rw-r--r--   0        0        0     2871 2022-08-24 00:28:47.978154 gncxml-0.6.9/gncxml/_cli.py
--rw-r--r--   0        0        0    10398 2023-07-20 00:33:06.893294 gncxml-0.6.9/gncxml/_iso4217.py
--rw-r--r--   0        0        0    11085 2021-12-27 13:53:45.413612 gncxml-0.6.9/gncxml/book.py
--rw-r--r--   0        0        0      618 2023-07-20 16:09:15.147061 gncxml-0.6.9/pyproject.toml
--rw-r--r--   0        0        0     1876 1970-01-01 00:00:00.000000 gncxml-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2017-12-17 01:02:32.000000 gncxml-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1124 2023-07-21 23:23:00.931331 gncxml-0.7.0/README.md
+-rw-r--r--   0        0        0      121 2017-11-23 20:24:39.000000 gncxml-0.7.0/gncxml/__init__.py
+-rw-r--r--   0        0        0       90 2021-12-27 13:53:45.410909 gncxml-0.7.0/gncxml/__main__.py
+-rw-r--r--   0        0        0     2871 2022-08-24 00:28:47.978154 gncxml-0.7.0/gncxml/_cli.py
+-rw-r--r--   0        0        0    10398 2023-07-20 00:33:06.893294 gncxml-0.7.0/gncxml/_iso4217.py
+-rw-r--r--   0        0        0    11085 2021-12-27 13:53:45.413612 gncxml-0.7.0/gncxml/book.py
+-rw-r--r--   0        0        0      614 2023-07-21 23:14:01.735880 gncxml-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 gncxml-0.7.0/PKG-INFO
```

### Comparing `gncxml-0.6.9/LICENSE` & `gncxml-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gncxml-0.6.9/README.md` & `gncxml-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 try:
     book = gncxml.Book("mybook.gnucash")
 except OSError as err:
     sys.exit(err)
 
 # Extract splits as pandas.DataFrame
 df = book.list_splits()
-print(df[df["trn_date"] >= "2017-10-01"].to_csv())
+print(df[df["trn_date"] >= "2023-07-01"].to_csv())
 ```
 
 See also: [examples/module_usage.ipynb](https://github.com/LiosK/gncxml/blob/master/examples/module_usage.ipynb)
 
 ## License
 
 Copyright 2017-2022 LiosK
```

### Comparing `gncxml-0.6.9/gncxml/_cli.py` & `gncxml-0.7.0/gncxml/_cli.py`

 * *Files identical despite different names*

### Comparing `gncxml-0.6.9/gncxml/_iso4217.py` & `gncxml-0.7.0/gncxml/_iso4217.py`

 * *Files identical despite different names*

### Comparing `gncxml-0.6.9/gncxml/book.py` & `gncxml-0.7.0/gncxml/book.py`

 * *Files identical despite different names*

### Comparing `gncxml-0.6.9/pyproject.toml` & `gncxml-0.7.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gncxml"
-version = "0.6.9"
+version = "0.7.0"
 description = "Extract entries from GnuCash data file to pandas.DataFrame."
 license = "Apache-2.0"
 authors = ["LiosK <contact@mail.liosk.net>"]
 readme = "README.md"
 homepage = "https://github.com/LiosK/gncxml"
 classifiers = [
   "Operating System :: OS Independent",
@@ -12,15 +12,15 @@
 ]
 
 [tool.poetry.scripts]
 gncxml = "gncxml._cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pandas = "^1.5.3"
+pandas = "^2.0"
 
 [tool.poetry.dev-dependencies]
-jupyterlab = "^3.6.5"
+jupyterlab = "^4.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gncxml-0.6.9/PKG-INFO` & `gncxml-0.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: gncxml
-Version: 0.6.9
+Version: 0.7.0
 Summary: Extract entries from GnuCash data file to pandas.DataFrame.
 Home-page: https://github.com/LiosK/gncxml
 License: Apache-2.0
 Author: LiosK
 Author-email: contact@mail.liosk.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business :: Financial
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pandas (>=2.0,<3.0)
 Description-Content-Type: text/markdown
 
 # gncxml
 
 [![PyPI](https://img.shields.io/pypi/v/gncxml)](https://pypi.org/project/gncxml/)
 
 gncxml - extract entries from GnuCash data file to pandas.DataFrame
@@ -57,15 +57,15 @@
 try:
     book = gncxml.Book("mybook.gnucash")
 except OSError as err:
     sys.exit(err)
 
 # Extract splits as pandas.DataFrame
 df = book.list_splits()
-print(df[df["trn_date"] >= "2017-10-01"].to_csv())
+print(df[df["trn_date"] >= "2023-07-01"].to_csv())
 ```
 
 See also: [examples/module_usage.ipynb](https://github.com/LiosK/gncxml/blob/master/examples/module_usage.ipynb)
 
 ## License
 
 Copyright 2017-2022 LiosK
```

