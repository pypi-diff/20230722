# Comparing `tmp/unstac-0.0.2.tar.gz` & `tmp/unstac-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstac-0.0.2.tar", last modified: Sat Jul 22 13:09:16 2023, max compression
+gzip compressed data, was "unstac-0.0.3.tar", last modified: Sat Jul 22 13:33:12 2023, max compression
```

## Comparing `unstac-0.0.2.tar` & `unstac-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 luka      (1000) luka      (1000)        0 2023-07-22 13:09:16.437394 unstac-0.0.2/
--rw-r--r--   0 luka      (1000) luka      (1000)     1070 2023-07-22 12:32:34.000000 unstac-0.0.2/LICENSE
--rw-r--r--   0 luka      (1000) luka      (1000)     2177 2023-07-22 13:09:16.437394 unstac-0.0.2/PKG-INFO
--rw-r--r--   0 luka      (1000) luka      (1000)     1963 2023-07-22 12:53:09.000000 unstac-0.0.2/README.md
--rw-r--r--   0 luka      (1000) luka      (1000)      545 2023-07-22 12:40:30.000000 unstac-0.0.2/pyproject.toml
--rw-r--r--   0 luka      (1000) luka      (1000)       38 2023-07-22 13:09:16.437394 unstac-0.0.2/setup.cfg
--rw-r--r--   0 luka      (1000) luka      (1000)       38 2023-07-22 13:09:11.000000 unstac-0.0.2/setup.py
-drwxr-xr-x   0 luka      (1000) luka      (1000)        0 2023-07-22 13:09:16.437394 unstac-0.0.2/unstac/
--rw-r--r--   0 luka      (1000) luka      (1000)     4248 2023-07-22 12:35:41.000000 unstac-0.0.2/unstac/__init__.py
--rw-r--r--   0 luka      (1000) luka      (1000)       58 2023-07-22 12:09:07.000000 unstac-0.0.2/unstac/__main__.py
-drwxr-xr-x   0 luka      (1000) luka      (1000)        0 2023-07-22 13:09:16.437394 unstac-0.0.2/unstac.egg-info/
--rw-r--r--   0 luka      (1000) luka      (1000)     2177 2023-07-22 13:09:16.000000 unstac-0.0.2/unstac.egg-info/PKG-INFO
--rw-r--r--   0 luka      (1000) luka      (1000)      261 2023-07-22 13:09:16.000000 unstac-0.0.2/unstac.egg-info/SOURCES.txt
--rw-r--r--   0 luka      (1000) luka      (1000)        1 2023-07-22 13:09:16.000000 unstac-0.0.2/unstac.egg-info/dependency_links.txt
--rw-r--r--   0 luka      (1000) luka      (1000)       39 2023-07-22 13:09:16.000000 unstac-0.0.2/unstac.egg-info/entry_points.txt
--rw-r--r--   0 luka      (1000) luka      (1000)       44 2023-07-22 13:09:16.000000 unstac-0.0.2/unstac.egg-info/requires.txt
--rw-r--r--   0 luka      (1000) luka      (1000)        7 2023-07-22 13:09:16.000000 unstac-0.0.2/unstac.egg-info/top_level.txt
+drwxr-xr-x   0 luka      (1000) luka      (1000)        0 2023-07-22 13:33:12.534398 unstac-0.0.3/
+-rw-r--r--   0 luka      (1000) luka      (1000)     1070 2023-07-22 12:32:34.000000 unstac-0.0.3/LICENSE
+-rw-r--r--   0 luka      (1000) luka      (1000)     2183 2023-07-22 13:33:12.531065 unstac-0.0.3/PKG-INFO
+-rw-r--r--   0 luka      (1000) luka      (1000)     1969 2023-07-22 13:30:55.000000 unstac-0.0.3/README.md
+-rw-r--r--   0 luka      (1000) luka      (1000)      545 2023-07-22 13:33:08.000000 unstac-0.0.3/pyproject.toml
+-rw-r--r--   0 luka      (1000) luka      (1000)       38 2023-07-22 13:33:12.534398 unstac-0.0.3/setup.cfg
+-rw-r--r--   0 luka      (1000) luka      (1000)       38 2023-07-22 13:09:11.000000 unstac-0.0.3/setup.py
+drwxr-xr-x   0 luka      (1000) luka      (1000)        0 2023-07-22 13:33:12.531065 unstac-0.0.3/unstac/
+-rw-r--r--   0 luka      (1000) luka      (1000)     4248 2023-07-22 12:35:41.000000 unstac-0.0.3/unstac/__init__.py
+-rw-r--r--   0 luka      (1000) luka      (1000)       58 2023-07-22 12:09:07.000000 unstac-0.0.3/unstac/__main__.py
+drwxr-xr-x   0 luka      (1000) luka      (1000)        0 2023-07-22 13:33:12.531065 unstac-0.0.3/unstac.egg-info/
+-rw-r--r--   0 luka      (1000) luka      (1000)     2183 2023-07-22 13:33:12.000000 unstac-0.0.3/unstac.egg-info/PKG-INFO
+-rw-r--r--   0 luka      (1000) luka      (1000)      261 2023-07-22 13:33:12.000000 unstac-0.0.3/unstac.egg-info/SOURCES.txt
+-rw-r--r--   0 luka      (1000) luka      (1000)        1 2023-07-22 13:33:12.000000 unstac-0.0.3/unstac.egg-info/dependency_links.txt
+-rw-r--r--   0 luka      (1000) luka      (1000)       39 2023-07-22 13:33:12.000000 unstac-0.0.3/unstac.egg-info/entry_points.txt
+-rw-r--r--   0 luka      (1000) luka      (1000)       44 2023-07-22 13:33:12.000000 unstac-0.0.3/unstac.egg-info/requires.txt
+-rw-r--r--   0 luka      (1000) luka      (1000)        7 2023-07-22 13:33:12.000000 unstac-0.0.3/unstac.egg-info/top_level.txt
```

### Comparing `unstac-0.0.2/LICENSE` & `unstac-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unstac-0.0.2/PKG-INFO` & `unstac-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstac
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tool for unwrapping Spatiotemporal Asset Catalogs into tabular data
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `unstac`
 
@@ -16,15 +16,15 @@
 ```
 pip install unstac
 ```
 
 or
 
 ```
-git clone https://gitlab.com/m1/unstac.git
+git clone https://gitlab.com/multione/unstac.git
 pip install .
 ```
 
 ## Usage
 
 ```
 $ unstac --help
```

### Comparing `unstac-0.0.2/README.md` & `unstac-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ```
 pip install unstac
 ```
 
 or
 
 ```
-git clone https://gitlab.com/m1/unstac.git
+git clone https://gitlab.com/multione/unstac.git
 pip install .
 ```
 
 ## Usage
 
 ```
 $ unstac --help
```

### Comparing `unstac-0.0.2/pyproject.toml` & `unstac-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unstac"
-version = "0.0.2"
+version = "0.0.3"
 authors = []
 description = "Tool for unwrapping Spatiotemporal Asset Catalogs into tabular data"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = []
 dependencies = [
              "pystac[orjson]",
```

### Comparing `unstac-0.0.2/unstac/__init__.py` & `unstac-0.0.3/unstac/__init__.py`

 * *Files identical despite different names*

### Comparing `unstac-0.0.2/unstac.egg-info/PKG-INFO` & `unstac-0.0.3/unstac.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstac
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tool for unwrapping Spatiotemporal Asset Catalogs into tabular data
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `unstac`
 
@@ -16,15 +16,15 @@
 ```
 pip install unstac
 ```
 
 or
 
 ```
-git clone https://gitlab.com/m1/unstac.git
+git clone https://gitlab.com/multione/unstac.git
 pip install .
 ```
 
 ## Usage
 
 ```
 $ unstac --help
```

