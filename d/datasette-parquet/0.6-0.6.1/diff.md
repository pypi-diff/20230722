# Comparing `tmp/datasette-parquet-0.6.tar.gz` & `tmp/datasette-parquet-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-parquet-0.6.tar", last modified: Sun Apr 23 03:48:30 2023, max compression
+gzip compressed data, was "datasette-parquet-0.6.1.tar", last modified: Sat Jul 22 01:02:10 2023, max compression
```

## Comparing `datasette-parquet-0.6.tar` & `datasette-parquet-0.6.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:48:30.944607 datasette-parquet-0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-23 03:48:14.000000 datasette-parquet-0.6/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-23 03:48:14.000000 datasette-parquet-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-04-23 03:48:30.944607 datasette-parquet-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-04-23 03:48:14.000000 datasette-parquet-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:48:30.944607 datasette-parquet-0.6/datasette_parquet/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-23 03:48:14.000000 datasette-parquet-0.6/datasette_parquet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-23 03:48:14.000000 datasette-parquet-0.6/datasette_parquet/ddl.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-23 03:48:14.000000 datasette-parquet-0.6/datasette_parquet/debounce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-23 03:48:14.000000 datasette-parquet-0.6/datasette_parquet/ducky.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-23 03:48:14.000000 datasette-parquet-0.6/datasette_parquet/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-23 03:48:14.000000 datasette-parquet-0.6/datasette_parquet/rewrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-23 03:48:14.000000 datasette-parquet-0.6/datasette_parquet/winging_it.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:48:30.944607 datasette-parquet-0.6/datasette_parquet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-04-23 03:48:30.000000 datasette-parquet-0.6/datasette_parquet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-23 03:48:30.000000 datasette-parquet-0.6/datasette_parquet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 03:48:30.000000 datasette-parquet-0.6/datasette_parquet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-23 03:48:30.000000 datasette-parquet-0.6/datasette_parquet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-23 03:48:30.000000 datasette-parquet-0.6/datasette_parquet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 03:48:30.000000 datasette-parquet-0.6/datasette_parquet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 03:48:30.944607 datasette-parquet-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-23 03:48:14.000000 datasette-parquet-0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:48:30.944607 datasette-parquet-0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-23 03:48:14.000000 datasette-parquet-0.6/tests/test_parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:02:10.435819 datasette-parquet-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-22 01:01:55.000000 datasette-parquet-0.6.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 01:01:55.000000 datasette-parquet-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-07-22 01:02:10.435819 datasette-parquet-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-07-22 01:01:55.000000 datasette-parquet-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:02:10.435819 datasette-parquet-0.6.1/datasette_parquet/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-22 01:01:55.000000 datasette-parquet-0.6.1/datasette_parquet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-22 01:01:55.000000 datasette-parquet-0.6.1/datasette_parquet/ddl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-22 01:01:55.000000 datasette-parquet-0.6.1/datasette_parquet/debounce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-22 01:01:55.000000 datasette-parquet-0.6.1/datasette_parquet/ducky.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-22 01:01:55.000000 datasette-parquet-0.6.1/datasette_parquet/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-22 01:01:55.000000 datasette-parquet-0.6.1/datasette_parquet/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-22 01:01:55.000000 datasette-parquet-0.6.1/datasette_parquet/rewrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-22 01:01:55.000000 datasette-parquet-0.6.1/datasette_parquet/winging_it.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:02:10.435819 datasette-parquet-0.6.1/datasette_parquet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-07-22 01:02:10.000000 datasette-parquet-0.6.1/datasette_parquet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-22 01:02:10.000000 datasette-parquet-0.6.1/datasette_parquet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 01:02:10.000000 datasette-parquet-0.6.1/datasette_parquet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-22 01:02:10.000000 datasette-parquet-0.6.1/datasette_parquet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-22 01:02:10.000000 datasette-parquet-0.6.1/datasette_parquet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-22 01:02:10.000000 datasette-parquet-0.6.1/datasette_parquet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 01:02:10.435819 datasette-parquet-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-22 01:01:55.000000 datasette-parquet-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:02:10.435819 datasette-parquet-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-22 01:01:55.000000 datasette-parquet-0.6.1/tests/test_parquet.py
```

### Comparing `datasette-parquet-0.6/COPYING` & `datasette-parquet-0.6.1/COPYING`

 * *Files identical despite different names*

### Comparing `datasette-parquet-0.6/LICENSE` & `datasette-parquet-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-parquet-0.6/PKG-INFO` & `datasette-parquet-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-parquet
-Version: 0.6
+Version: 0.6.1
 Summary: Read Parquet files in Datasette
 Home-page: https://github.com/cldellow/datasette-parquet
 Author: Colin Dellow
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/cldellow/datasette-parquet/issues
 Project-URL: CI, https://github.com/cldellow/datasette-parquet/actions
 Project-URL: Changelog, https://github.com/cldellow/datasette-parquet/releases
```

### Comparing `datasette-parquet-0.6/README.md` & `datasette-parquet-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `datasette-parquet-0.6/datasette_parquet/__init__.py` & `datasette-parquet-0.6.1/datasette_parquet/__init__.py`

 * *Files identical despite different names*

### Comparing `datasette-parquet-0.6/datasette_parquet/ddl.py` & `datasette-parquet-0.6.1/datasette_parquet/ddl.py`

 * *Files identical despite different names*

### Comparing `datasette-parquet-0.6/datasette_parquet/debounce.py` & `datasette-parquet-0.6.1/datasette_parquet/debounce.py`

 * *Files identical despite different names*

### Comparing `datasette-parquet-0.6/datasette_parquet/ducky.py` & `datasette-parquet-0.6.1/datasette_parquet/ducky.py`

 * *Files identical despite different names*

### Comparing `datasette-parquet-0.6/datasette_parquet/patches.py` & `datasette-parquet-0.6.1/datasette_parquet/patches.py`

 * *Files identical despite different names*

### Comparing `datasette-parquet-0.6/datasette_parquet/rewrite.py` & `datasette-parquet-0.6.1/datasette_parquet/rewrite.py`

 * *Files identical despite different names*

### Comparing `datasette-parquet-0.6/datasette_parquet.egg-info/PKG-INFO` & `datasette-parquet-0.6.1/datasette_parquet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-parquet
-Version: 0.6
+Version: 0.6.1
 Summary: Read Parquet files in Datasette
 Home-page: https://github.com/cldellow/datasette-parquet
 Author: Colin Dellow
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/cldellow/datasette-parquet/issues
 Project-URL: CI, https://github.com/cldellow/datasette-parquet/actions
 Project-URL: Changelog, https://github.com/cldellow/datasette-parquet/releases
```

### Comparing `datasette-parquet-0.6/setup.py` & `datasette-parquet-0.6.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.6"
+VERSION = "0.6.1"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `datasette-parquet-0.6/tests/test_parquet.py` & `datasette-parquet-0.6.1/tests/test_parquet.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from datasette.app import Datasette
 from .create_db import create_dbs
 import pytest
 import duckdb
 from datasette_parquet.winging_it import ProxyConnection
+from datasette_parquet import exceptions
 
 @pytest.fixture(scope="session")
 def datasette():
     create_dbs('./fixtures')
     metadata = {
         'plugins': {
             'datasette-parquet': {
@@ -67,7 +68,20 @@
     assert response.status_code == 200
 
 def test_fetchone():
     raw_conn = duckdb.connect()
     conn = ProxyConnection(raw_conn)
     fetched = conn.execute('SELECT 1 AS col').fetchone()
     assert fetched['col'] == 1
+
+
+@pytest.mark.asyncio
+def test_catch_double_quote_usage_for_literal(datasette):
+
+    raw_conn = duckdb.connect()
+    conn = ProxyConnection(raw_conn)
+
+    # try reading the parquet file in trove/userdata1.parquet
+    explodey_string_with_double_quotes = 'SELECT * from "./trove/userdata1.parquet" WHERE first_name = "Amanda"'
+
+    with pytest.raises(exceptions.DoubleQuoteForLiteraValue):
+        result = conn.execute(explodey_string_with_double_quotes).fetchall()
```

