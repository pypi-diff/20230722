# Comparing `tmp/mg_fastpurge-0.1.3.tar.gz` & `tmp/mg_fastpurge-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mg_fastpurge-0.1.3.tar", max compression
+gzip compressed data, was "mg_fastpurge-0.1.4.tar", max compression
```

## Comparing `mg_fastpurge-0.1.3.tar` & `mg_fastpurge-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-07-19 02:42:42.924833 mg_fastpurge-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-07-22 07:11:33.680448 mg_fastpurge-0.1.3/mg_fastpurge/__init__.py
--rwxr-xr-x   0        0        0      852 2023-07-22 07:48:39.723321 mg_fastpurge-0.1.3/mg_fastpurge/purge.py
--rw-r--r--   0        0        0      650 2023-07-22 08:01:09.311326 mg_fastpurge-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      785 1970-01-01 00:00:00.000000 mg_fastpurge-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-19 02:42:42.924833 mg_fastpurge-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-22 07:11:33.680448 mg_fastpurge-0.1.4/mg_fastpurge/__init__.py
+-rwxr-xr-x   0        0        0      852 2023-07-22 07:48:39.723321 mg_fastpurge-0.1.4/mg_fastpurge/purge.py
+-rw-r--r--   0        0        0      650 2023-07-22 08:08:21.498782 mg_fastpurge-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      785 1970-01-01 00:00:00.000000 mg_fastpurge-0.1.4/PKG-INFO
```

### Comparing `mg_fastpurge-0.1.3/mg_fastpurge/purge.py` & `mg_fastpurge-0.1.4/mg_fastpurge/purge.py`

 * *Files identical despite different names*

### Comparing `mg_fastpurge-0.1.3/pyproject.toml` & `mg_fastpurge-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry] 
 name = "mg_fastpurge"
-version = "0.1.3" 
+version = "0.1.4" 
 description = "Marriott CDN Team Fastpurge POC script" 
 authors = ["Alan Janis <alan.janis@marriott.com>", "Raahi Chada <raahi.chada@marriott.com"]
 readme = "README.md"
 packages = [{include = "mg_fastpurge"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
```

### Comparing `mg_fastpurge-0.1.3/PKG-INFO` & `mg_fastpurge-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mg-fastpurge
-Version: 0.1.3
+Version: 0.1.4
 Summary: Marriott CDN Team Fastpurge POC script
 Author: Alan Janis
 Author-email: alan.janis@marriott.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

