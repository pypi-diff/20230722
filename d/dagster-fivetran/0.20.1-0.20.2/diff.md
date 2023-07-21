# Comparing `tmp/dagster-fivetran-0.20.1.tar.gz` & `tmp/dagster-fivetran-0.20.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-fivetran-0.20.1.tar", last modified: Fri Jul 21 15:38:57 2023, max compression
+gzip compressed data, was "dagster-fivetran-0.20.2.tar", last modified: Fri Jul 21 22:36:35 2023, max compression
```

## Comparing `dagster-fivetran-0.20.1.tar` & `dagster-fivetran-0.20.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:57.519079 dagster-fivetran-0.20.1/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-21 15:29:00.000000 dagster-fivetran-0.20.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       68 2023-07-21 15:29:00.000000 dagster-fivetran-0.20.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      648 2023-07-21 15:38:57.519079 dagster-fivetran-0.20.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      134 2023-07-21 15:29:00.000000 dagster-fivetran-0.20.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:57.515079 dagster-fivetran-0.20.1/dagster_fivetran/
--rw-r--r--   0 root         (0) root         (0)      854 2023-07-21 15:29:00.000000 dagster-fivetran-0.20.1/dagster_fivetran/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20478 2023-07-21 15:29:00.000000 dagster-fivetran-0.20.1/dagster_fivetran/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)      426 2023-07-21 15:29:00.000000 dagster-fivetran-0.20.1/dagster_fivetran/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:57.519079 dagster-fivetran-0.20.1/dagster_fivetran/managed/
--rw-r--r--   0 root         (0) root         (0)      212 2023-07-21 15:29:00.000000 dagster-fivetran-0.20.1/dagster_fivetran/managed/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14474 2023-07-21 15:29:00.000000 dagster-fivetran-0.20.1/dagster_fivetran/managed/reconciliation.py
--rw-r--r--   0 root         (0) root         (0)     3258 2023-07-21 15:29:00.000000 dagster-fivetran-0.20.1/dagster_fivetran/managed/types.py
--rw-r--r--   0 root         (0) root         (0)     7139 2023-07-21 15:29:00.000000 dagster-fivetran-0.20.1/dagster_fivetran/ops.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-21 15:29:00.000000 dagster-fivetran-0.20.1/dagster_fivetran/py.typed
--rw-r--r--   0 root         (0) root         (0)    18311 2023-07-21 15:29:00.000000 dagster-fivetran-0.20.1/dagster_fivetran/resources.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-07-21 15:29:00.000000 dagster-fivetran-0.20.1/dagster_fivetran/types.py
--rw-r--r--   0 root         (0) root         (0)     2994 2023-07-21 15:29:00.000000 dagster-fivetran-0.20.1/dagster_fivetran/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 15:29:00.000000 dagster-fivetran-0.20.1/dagster_fivetran/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:57.519079 dagster-fivetran-0.20.1/dagster_fivetran.egg-info/
--rw-r--r--   0 root         (0) root         (0)      648 2023-07-21 15:38:57.000000 dagster-fivetran-0.20.1/dagster_fivetran.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      687 2023-07-21 15:38:57.000000 dagster-fivetran-0.20.1/dagster_fivetran.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:38:57.000000 dagster-fivetran-0.20.1/dagster_fivetran.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-07-21 15:38:57.000000 dagster-fivetran-0.20.1/dagster_fivetran.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:38:57.000000 dagster-fivetran-0.20.1/dagster_fivetran.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-21 15:38:57.000000 dagster-fivetran-0.20.1/dagster_fivetran.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-21 15:38:57.000000 dagster-fivetran-0.20.1/dagster_fivetran.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-07-21 15:38:57.523079 dagster-fivetran-0.20.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1442 2023-07-21 15:29:00.000000 dagster-fivetran-0.20.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:36:35.722545 dagster-fivetran-0.20.2/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-21 22:28:10.000000 dagster-fivetran-0.20.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       68 2023-07-21 22:28:10.000000 dagster-fivetran-0.20.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      648 2023-07-21 22:36:35.722545 dagster-fivetran-0.20.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      134 2023-07-21 22:28:10.000000 dagster-fivetran-0.20.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:36:35.718546 dagster-fivetran-0.20.2/dagster_fivetran/
+-rw-r--r--   0 root         (0) root         (0)      854 2023-07-21 22:28:10.000000 dagster-fivetran-0.20.2/dagster_fivetran/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20478 2023-07-21 22:28:10.000000 dagster-fivetran-0.20.2/dagster_fivetran/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)      426 2023-07-21 22:28:10.000000 dagster-fivetran-0.20.2/dagster_fivetran/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:36:35.722545 dagster-fivetran-0.20.2/dagster_fivetran/managed/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-07-21 22:28:10.000000 dagster-fivetran-0.20.2/dagster_fivetran/managed/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14474 2023-07-21 22:28:10.000000 dagster-fivetran-0.20.2/dagster_fivetran/managed/reconciliation.py
+-rw-r--r--   0 root         (0) root         (0)     3258 2023-07-21 22:28:10.000000 dagster-fivetran-0.20.2/dagster_fivetran/managed/types.py
+-rw-r--r--   0 root         (0) root         (0)     7139 2023-07-21 22:28:10.000000 dagster-fivetran-0.20.2/dagster_fivetran/ops.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-21 22:28:10.000000 dagster-fivetran-0.20.2/dagster_fivetran/py.typed
+-rw-r--r--   0 root         (0) root         (0)    18311 2023-07-21 22:28:10.000000 dagster-fivetran-0.20.2/dagster_fivetran/resources.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-07-21 22:28:10.000000 dagster-fivetran-0.20.2/dagster_fivetran/types.py
+-rw-r--r--   0 root         (0) root         (0)     2994 2023-07-21 22:28:10.000000 dagster-fivetran-0.20.2/dagster_fivetran/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 22:28:10.000000 dagster-fivetran-0.20.2/dagster_fivetran/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:36:35.718546 dagster-fivetran-0.20.2/dagster_fivetran.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      648 2023-07-21 22:36:35.000000 dagster-fivetran-0.20.2/dagster_fivetran.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      687 2023-07-21 22:36:35.000000 dagster-fivetran-0.20.2/dagster_fivetran.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 22:36:35.000000 dagster-fivetran-0.20.2/dagster_fivetran.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-21 22:36:35.000000 dagster-fivetran-0.20.2/dagster_fivetran.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 22:36:35.000000 dagster-fivetran-0.20.2/dagster_fivetran.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-21 22:36:35.000000 dagster-fivetran-0.20.2/dagster_fivetran.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-21 22:36:35.000000 dagster-fivetran-0.20.2/dagster_fivetran.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-07-21 22:36:35.722545 dagster-fivetran-0.20.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-07-21 22:28:10.000000 dagster-fivetran-0.20.2/setup.py
```

### Comparing `dagster-fivetran-0.20.1/LICENSE` & `dagster-fivetran-0.20.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.20.1/PKG-INFO` & `dagster-fivetran-0.20.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-fivetran
-Version: 0.20.1
+Version: 0.20.2
 Summary: Package for integrating Fivetran with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-fivetran
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-fivetran-0.20.1/dagster_fivetran/__init__.py` & `dagster-fivetran-0.20.2/dagster_fivetran/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.20.1/dagster_fivetran/asset_defs.py` & `dagster-fivetran-0.20.2/dagster_fivetran/asset_defs.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.20.1/dagster_fivetran/managed/reconciliation.py` & `dagster-fivetran-0.20.2/dagster_fivetran/managed/reconciliation.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.20.1/dagster_fivetran/managed/types.py` & `dagster-fivetran-0.20.2/dagster_fivetran/managed/types.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.20.1/dagster_fivetran/ops.py` & `dagster-fivetran-0.20.2/dagster_fivetran/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.20.1/dagster_fivetran/resources.py` & `dagster-fivetran-0.20.2/dagster_fivetran/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.20.1/dagster_fivetran/types.py` & `dagster-fivetran-0.20.2/dagster_fivetran/types.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.20.1/dagster_fivetran/utils.py` & `dagster-fivetran-0.20.2/dagster_fivetran/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.20.1/dagster_fivetran.egg-info/PKG-INFO` & `dagster-fivetran-0.20.2/dagster_fivetran.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-fivetran
-Version: 0.20.1
+Version: 0.20.2
 Summary: Package for integrating Fivetran with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-fivetran
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-fivetran-0.20.1/dagster_fivetran.egg-info/SOURCES.txt` & `dagster-fivetran-0.20.2/dagster_fivetran.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.20.1/setup.py` & `dagster-fivetran-0.20.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,20 +28,20 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_fivetran_tests*"]),
-    install_requires=["dagster==1.4.1"],
+    install_requires=["dagster==1.4.2"],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "dagster-fivetran = dagster_fivetran.cli:main",
         ]
     },
     extras_require={
         "managed": [
-            "dagster-managed-elements==0.20.1",
+            "dagster-managed-elements==0.20.2",
         ],
     },
 )
```

