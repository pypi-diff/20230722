# Comparing `tmp/unstac-0.0.3.tar.gz` & `tmp/unstac-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstac-0.0.3.tar", last modified: Sat Jul 22 13:33:12 2023, max compression
+gzip compressed data, was "unstac-0.0.4.tar", last modified: Sat Jul 22 14:56:36 2023, max compression
```

## Comparing `unstac-0.0.3.tar` & `unstac-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 luka      (1000) luka      (1000)        0 2023-07-22 13:33:12.534398 unstac-0.0.3/
--rw-r--r--   0 luka      (1000) luka      (1000)     1070 2023-07-22 12:32:34.000000 unstac-0.0.3/LICENSE
--rw-r--r--   0 luka      (1000) luka      (1000)     2183 2023-07-22 13:33:12.531065 unstac-0.0.3/PKG-INFO
--rw-r--r--   0 luka      (1000) luka      (1000)     1969 2023-07-22 13:30:55.000000 unstac-0.0.3/README.md
--rw-r--r--   0 luka      (1000) luka      (1000)      545 2023-07-22 13:33:08.000000 unstac-0.0.3/pyproject.toml
--rw-r--r--   0 luka      (1000) luka      (1000)       38 2023-07-22 13:33:12.534398 unstac-0.0.3/setup.cfg
--rw-r--r--   0 luka      (1000) luka      (1000)       38 2023-07-22 13:09:11.000000 unstac-0.0.3/setup.py
-drwxr-xr-x   0 luka      (1000) luka      (1000)        0 2023-07-22 13:33:12.531065 unstac-0.0.3/unstac/
--rw-r--r--   0 luka      (1000) luka      (1000)     4248 2023-07-22 12:35:41.000000 unstac-0.0.3/unstac/__init__.py
--rw-r--r--   0 luka      (1000) luka      (1000)       58 2023-07-22 12:09:07.000000 unstac-0.0.3/unstac/__main__.py
-drwxr-xr-x   0 luka      (1000) luka      (1000)        0 2023-07-22 13:33:12.531065 unstac-0.0.3/unstac.egg-info/
--rw-r--r--   0 luka      (1000) luka      (1000)     2183 2023-07-22 13:33:12.000000 unstac-0.0.3/unstac.egg-info/PKG-INFO
--rw-r--r--   0 luka      (1000) luka      (1000)      261 2023-07-22 13:33:12.000000 unstac-0.0.3/unstac.egg-info/SOURCES.txt
--rw-r--r--   0 luka      (1000) luka      (1000)        1 2023-07-22 13:33:12.000000 unstac-0.0.3/unstac.egg-info/dependency_links.txt
--rw-r--r--   0 luka      (1000) luka      (1000)       39 2023-07-22 13:33:12.000000 unstac-0.0.3/unstac.egg-info/entry_points.txt
--rw-r--r--   0 luka      (1000) luka      (1000)       44 2023-07-22 13:33:12.000000 unstac-0.0.3/unstac.egg-info/requires.txt
--rw-r--r--   0 luka      (1000) luka      (1000)        7 2023-07-22 13:33:12.000000 unstac-0.0.3/unstac.egg-info/top_level.txt
+drwxr-xr-x   0 luka      (1000) luka      (1000)        0 2023-07-22 14:56:36.855044 unstac-0.0.4/
+-rw-r--r--   0 luka      (1000) luka      (1000)     1070 2023-07-22 12:32:34.000000 unstac-0.0.4/LICENSE
+-rw-r--r--   0 luka      (1000) luka      (1000)     2235 2023-07-22 14:56:36.851710 unstac-0.0.4/PKG-INFO
+-rw-r--r--   0 luka      (1000) luka      (1000)     1969 2023-07-22 13:30:55.000000 unstac-0.0.4/README.md
+-rw-r--r--   0 luka      (1000) luka      (1000)      613 2023-07-22 14:56:30.000000 unstac-0.0.4/pyproject.toml
+-rw-r--r--   0 luka      (1000) luka      (1000)       38 2023-07-22 14:56:36.855044 unstac-0.0.4/setup.cfg
+-rw-r--r--   0 luka      (1000) luka      (1000)       38 2023-07-22 13:09:11.000000 unstac-0.0.4/setup.py
+drwxr-xr-x   0 luka      (1000) luka      (1000)        0 2023-07-22 14:56:36.851710 unstac-0.0.4/unstac/
+-rw-r--r--   0 luka      (1000) luka      (1000)     4248 2023-07-22 12:35:41.000000 unstac-0.0.4/unstac/__init__.py
+-rw-r--r--   0 luka      (1000) luka      (1000)       58 2023-07-22 12:09:07.000000 unstac-0.0.4/unstac/__main__.py
+drwxr-xr-x   0 luka      (1000) luka      (1000)        0 2023-07-22 14:56:36.851710 unstac-0.0.4/unstac.egg-info/
+-rw-r--r--   0 luka      (1000) luka      (1000)     2235 2023-07-22 14:56:36.000000 unstac-0.0.4/unstac.egg-info/PKG-INFO
+-rw-r--r--   0 luka      (1000) luka      (1000)      261 2023-07-22 14:56:36.000000 unstac-0.0.4/unstac.egg-info/SOURCES.txt
+-rw-r--r--   0 luka      (1000) luka      (1000)        1 2023-07-22 14:56:36.000000 unstac-0.0.4/unstac.egg-info/dependency_links.txt
+-rw-r--r--   0 luka      (1000) luka      (1000)       39 2023-07-22 14:56:36.000000 unstac-0.0.4/unstac.egg-info/entry_points.txt
+-rw-r--r--   0 luka      (1000) luka      (1000)       44 2023-07-22 14:56:36.000000 unstac-0.0.4/unstac.egg-info/requires.txt
+-rw-r--r--   0 luka      (1000) luka      (1000)        7 2023-07-22 14:56:36.000000 unstac-0.0.4/unstac.egg-info/top_level.txt
```

### Comparing `unstac-0.0.3/LICENSE` & `unstac-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unstac-0.0.3/PKG-INFO` & `unstac-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: unstac
-Version: 0.0.3
-Summary: Tool for unwrapping Spatiotemporal Asset Catalogs into tabular data
+Version: 0.0.4
+Summary: Tool for unwrapping Spatiotemporal Asset Catalogs into GeoPackage
+Author-email: Luka Antonić <luka.olegsson@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `unstac`
 
 CLI tool for making GeoPackages from static
```

### Comparing `unstac-0.0.3/README.md` & `unstac-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `unstac-0.0.3/pyproject.toml` & `unstac-0.0.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unstac"
-version = "0.0.3"
-authors = []
-description = "Tool for unwrapping Spatiotemporal Asset Catalogs into tabular data"
+version = "0.0.4"
+authors = [
+        {name = "Luka Antonić", email = "luka.olegsson@gmail.com"},
+]
+description = "Tool for unwrapping Spatiotemporal Asset Catalogs into GeoPackage"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = []
 dependencies = [
              "pystac[orjson]",
              "rich",
              "typer",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `unstac-0.0.3/unstac/__init__.py` & `unstac-0.0.4/unstac/__init__.py`

 * *Files identical despite different names*

### Comparing `unstac-0.0.3/unstac.egg-info/PKG-INFO` & `unstac-0.0.4/unstac.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: unstac
-Version: 0.0.3
-Summary: Tool for unwrapping Spatiotemporal Asset Catalogs into tabular data
+Version: 0.0.4
+Summary: Tool for unwrapping Spatiotemporal Asset Catalogs into GeoPackage
+Author-email: Luka Antonić <luka.olegsson@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `unstac`
 
 CLI tool for making GeoPackages from static
```

