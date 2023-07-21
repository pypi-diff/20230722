# Comparing `tmp/microSWIFTtelemetry-0.3.1.tar.gz` & `tmp/microSWIFTtelemetry-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microSWIFTtelemetry-0.3.1.tar", last modified: Tue Jul 11 00:23:58 2023, max compression
+gzip compressed data, was "microSWIFTtelemetry-0.3.2.tar", last modified: Fri Jul 21 22:05:27 2023, max compression
```

## Comparing `microSWIFTtelemetry-0.3.1.tar` & `microSWIFTtelemetry-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-11 00:23:58.374210 microSWIFTtelemetry-0.3.1/
--rw-r--r--   0 jacob      (501) staff       (20)     1068 2022-11-06 06:16:28.000000 microSWIFTtelemetry-0.3.1/LICENSE
--rw-r--r--   0 jacob      (501) staff       (20)     1362 2023-07-11 00:23:58.374073 microSWIFTtelemetry-0.3.1/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)     3636 2022-12-22 16:21:15.000000 microSWIFTtelemetry-0.3.1/README.md
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-11 00:23:58.372474 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/
--rw-r--r--   0 jacob      (501) staff       (20)      137 2022-12-04 19:59:27.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/__init__.py
--rw-r--r--   0 jacob      (501) staff       (20)     9144 2023-07-11 00:09:58.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/pull_telemetry.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-11 00:23:58.373864 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/sbd/
--rw-r--r--   0 jacob      (501) staff       (20)       78 2022-12-04 20:17:51.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/sbd/__init__.py
--rw-r--r--   0 jacob      (501) staff       (20)     4301 2023-07-11 00:09:58.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/sbd/compile_sbd.py
--rw-r--r--   0 jacob      (501) staff       (20)     3012 2023-07-11 00:09:58.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/sbd/definitions.py
--rw-r--r--   0 jacob      (501) staff       (20)     6227 2023-07-11 00:09:58.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/sbd/read_sbd.py
--rw-r--r--   0 jacob      (501) staff       (20)     2386 2023-07-11 00:23:33.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/version.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-11 00:23:58.372999 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     1362 2023-07-11 00:23:58.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      506 2023-07-11 00:23:58.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-07-11 00:23:58.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       31 2023-07-11 00:23:58.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)       20 2023-07-11 00:23:58.000000 microSWIFTtelemetry-0.3.1/microSWIFTtelemetry.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)      145 2022-11-06 01:29:54.000000 microSWIFTtelemetry-0.3.1/pyproject.toml
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-07-11 00:23:58.374249 microSWIFTtelemetry-0.3.1/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1373 2022-11-06 20:48:39.000000 microSWIFTtelemetry-0.3.1/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-21 22:05:27.293690 microSWIFTtelemetry-0.3.2/
+-rw-r--r--   0 jacob      (501) staff       (20)     1068 2022-11-06 06:16:28.000000 microSWIFTtelemetry-0.3.2/LICENSE
+-rw-r--r--   0 jacob      (501) staff       (20)     1362 2023-07-21 22:05:27.293521 microSWIFTtelemetry-0.3.2/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)     3636 2022-12-22 16:21:15.000000 microSWIFTtelemetry-0.3.2/README.md
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-21 22:05:27.291394 microSWIFTtelemetry-0.3.2/microSWIFTtelemetry/
+-rw-r--r--   0 jacob      (501) staff       (20)      137 2022-12-04 19:59:27.000000 microSWIFTtelemetry-0.3.2/microSWIFTtelemetry/__init__.py
+-rw-r--r--   0 jacob      (501) staff       (20)     9144 2023-07-11 00:09:58.000000 microSWIFTtelemetry-0.3.2/microSWIFTtelemetry/pull_telemetry.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-21 22:05:27.293178 microSWIFTtelemetry-0.3.2/microSWIFTtelemetry/sbd/
+-rw-r--r--   0 jacob      (501) staff       (20)       78 2022-12-04 20:17:51.000000 microSWIFTtelemetry-0.3.2/microSWIFTtelemetry/sbd/__init__.py
+-rw-r--r--   0 jacob      (501) staff       (20)     4453 2023-07-21 22:01:02.000000 microSWIFTtelemetry-0.3.2/microSWIFTtelemetry/sbd/compile_sbd.py
+-rw-r--r--   0 jacob      (501) staff       (20)     3012 2023-07-11 00:09:58.000000 microSWIFTtelemetry-0.3.2/microSWIFTtelemetry/sbd/definitions.py
+-rw-r--r--   0 jacob      (501) staff       (20)     6227 2023-07-11 00:09:58.000000 microSWIFTtelemetry-0.3.2/microSWIFTtelemetry/sbd/read_sbd.py
+-rw-r--r--   0 jacob      (501) staff       (20)     2386 2023-07-21 22:04:15.000000 microSWIFTtelemetry-0.3.2/microSWIFTtelemetry/version.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-21 22:05:27.292203 microSWIFTtelemetry-0.3.2/microSWIFTtelemetry.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     1362 2023-07-21 22:05:27.000000 microSWIFTtelemetry-0.3.2/microSWIFTtelemetry.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      506 2023-07-21 22:05:27.000000 microSWIFTtelemetry-0.3.2/microSWIFTtelemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-07-21 22:05:27.000000 microSWIFTtelemetry-0.3.2/microSWIFTtelemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       31 2023-07-21 22:05:27.000000 microSWIFTtelemetry-0.3.2/microSWIFTtelemetry.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       20 2023-07-21 22:05:27.000000 microSWIFTtelemetry-0.3.2/microSWIFTtelemetry.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)      145 2022-11-06 01:29:54.000000 microSWIFTtelemetry-0.3.2/pyproject.toml
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-07-21 22:05:27.293741 microSWIFTtelemetry-0.3.2/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1373 2022-11-06 20:48:39.000000 microSWIFTtelemetry-0.3.2/setup.py
```

### Comparing `microSWIFTtelemetry-0.3.1/LICENSE` & `microSWIFTtelemetry-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `microSWIFTtelemetry-0.3.1/PKG-INFO` & `microSWIFTtelemetry-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microSWIFTtelemetry
-Version: 0.3.1
+Version: 0.3.2
 Summary: microSWIFTtelemetry: Python-based functionality for pulling telemetry from the microSWIFT wave buoy.
 Home-page: https://github.com/SASlabgroup/microSWIFTtelemetry
 Download-URL: 
 Author: Jacob Davis
 Author-email: davisjr@uw.edu
 Maintainer: Jacob Davis
 Maintainer-email: davisjr@uw.edu
```

### Comparing `microSWIFTtelemetry-0.3.1/README.md` & `microSWIFTtelemetry-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/pull_telemetry.py` & `microSWIFTtelemetry-0.3.2/microSWIFTtelemetry/pull_telemetry.py`

 * *Files identical despite different names*

### Comparing `microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/sbd/compile_sbd.py` & `microSWIFTtelemetry-0.3.2/microSWIFTtelemetry/sbd/compile_sbd.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 __all__ = [
     "to_pandas_datetime_index",
     "sort_dict",
     "compile_sbd",
 ]
 
+import os
 import warnings
 from collections import defaultdict
 from typing import Any
 
 import numpy as np
 import pandas
 import xarray
@@ -28,14 +29,16 @@
     var_type: str,
     from_memory: bool = False
 ) -> Any:
     """
     Compile contents of short burst data files into the specified
     variable type or output.
 
+    Valid variable types: 'dict' or 'pandas'
+
     Args:
         sbd_folder (str): directory containing.sbd files
         var_type (str): variable type to be returned
         from_memory (bool, optional): flag to indicate whether
                 sbd_folder was loaded from memory (True) or a local file
                 (False); defaults to False.
 
@@ -52,17 +55,21 @@
     if from_memory:
         for file in sbd_folder.namelist():
             swift_data, error_message = read_sbd(sbd_folder.open(file))
             if swift_data:
                 data.append(swift_data)
             errors.append(error_message)
 
-    else: #TODO: support reading from a folder of SBDs
-        raise NotImplementedError('Reading from a folder on the local '
-                                  'machine is not supported yet.')
+    else:
+        for file in os.listdir(sbd_folder):
+            with open(os.path.join(sbd_folder, file), 'rb') as file:
+                swift_data, error_message = read_sbd(file)
+            if swift_data:
+                data.append(swift_data)
+            errors.append(error_message)
 
     errors = _combine_dict_list(errors)
 
     if var_type == 'dict':
         d = _combine_dict_list(data)
         if d:
             d = sort_dict(d)
```

### Comparing `microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/sbd/definitions.py` & `microSWIFTtelemetry-0.3.2/microSWIFTtelemetry/sbd/definitions.py`

 * *Files identical despite different names*

### Comparing `microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/sbd/read_sbd.py` & `microSWIFTtelemetry-0.3.2/microSWIFTtelemetry/sbd/read_sbd.py`

 * *Files identical despite different names*

### Comparing `microSWIFTtelemetry-0.3.1/microSWIFTtelemetry/version.py` & `microSWIFTtelemetry-0.3.2/microSWIFTtelemetry/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import absolute_import, division, print_function
 from os.path import join as pjoin
 
 # Format expected by setup.py and doc/source/conf.py: string of form "X.Y.Z"
 _version_major = 0
 _version_minor = 3
-_version_micro = 1  # use '' for first of series, number for 1 and above
+_version_micro = 2  # use '' for first of series, number for 1 and above
 # _version_extra = 'dev'
 _version_extra = ''  # TODO: Uncomment this for full releases
 
 # Construct full version string from these.
 _ver = [_version_major, _version_minor]
 if _version_micro:
     _ver.append(_version_micro)
```

### Comparing `microSWIFTtelemetry-0.3.1/microSWIFTtelemetry.egg-info/PKG-INFO` & `microSWIFTtelemetry-0.3.2/microSWIFTtelemetry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microSWIFTtelemetry
-Version: 0.3.1
+Version: 0.3.2
 Summary: microSWIFTtelemetry: Python-based functionality for pulling telemetry from the microSWIFT wave buoy.
 Home-page: https://github.com/SASlabgroup/microSWIFTtelemetry
 Download-URL: 
 Author: Jacob Davis
 Author-email: davisjr@uw.edu
 Maintainer: Jacob Davis
 Maintainer-email: davisjr@uw.edu
```

### Comparing `microSWIFTtelemetry-0.3.1/setup.py` & `microSWIFTtelemetry-0.3.2/setup.py`

 * *Files identical despite different names*

