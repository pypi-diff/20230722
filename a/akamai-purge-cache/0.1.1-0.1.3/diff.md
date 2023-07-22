# Comparing `tmp/akamai_purge_cache-0.1.1.tar.gz` & `tmp/akamai_purge_cache-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akamai_purge_cache-0.1.1.tar", max compression
+gzip compressed data, was "akamai_purge_cache-0.1.3.tar", max compression
```

## Comparing `akamai_purge_cache-0.1.1.tar` & `akamai_purge_cache-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-07-19 02:42:42.924833 akamai_purge_cache-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-22 07:11:33.680448 akamai_purge_cache-0.1.1/akamai_purge_cache/__init__.py
--rwxr-xr-x   0        0        0      844 2023-07-22 07:01:37.281113 akamai_purge_cache-0.1.1/akamai_purge_cache/purge.py
--rw-r--r--   0        0        0      581 2023-07-22 07:23:47.754092 akamai_purge_cache-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 akamai_purge_cache-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-19 02:42:42.924833 akamai_purge_cache-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-22 07:11:33.680448 akamai_purge_cache-0.1.3/akamai_purge_cache/__init__.py
+-rwxr-xr-x   0        0        0      844 2023-07-22 07:01:37.281113 akamai_purge_cache-0.1.3/akamai_purge_cache/purge.py
+-rw-r--r--   0        0        0      582 2023-07-22 07:37:40.614569 akamai_purge_cache-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 akamai_purge_cache-0.1.3/PKG-INFO
```

### Comparing `akamai_purge_cache-0.1.1/akamai_purge_cache/purge.py` & `akamai_purge_cache-0.1.3/akamai_purge_cache/purge.py`

 * *Files identical despite different names*

### Comparing `akamai_purge_cache-0.1.1/pyproject.toml` & `akamai_purge_cache-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "akamai-purge-cache"
-version = "0.1.1"
+version = "0.1.3"
 description = ""
 authors = ["Alan Janis <alan.janis@marriott.com>"]
 readme = "README.md"
 packages = [{include = "akamai_purge_cache"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.10"
 fastpurge = "^1.0.4"
 edgegrid-python = "^1.3.1"
 monotonic = "^1.6"
 more-executors = "^2.11.4"
 click = "^8.1.6"
 awslambdaric = "^2.0.4"
```

### Comparing `akamai_purge_cache-0.1.1/PKG-INFO` & `akamai_purge_cache-0.1.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: akamai-purge-cache
-Version: 0.1.1
+Version: 0.1.3
 Summary: 
 Author: Alan Janis
 Author-email: alan.janis@marriott.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: awslambdaric (>=2.0.4,<3.0.0)
 Requires-Dist: click (>=8.1.6,<9.0.0)
 Requires-Dist: edgegrid-python (>=1.3.1,<2.0.0)
 Requires-Dist: fastpurge (>=1.0.4,<2.0.0)
```

