# Comparing `tmp/plemmy-0.3.2.tar.gz` & `tmp/plemmy-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plemmy-0.3.2.tar", last modified: Thu Jul 20 23:47:13 2023, max compression
+gzip compressed data, was "plemmy-0.3.3.tar", last modified: Sat Jul 22 19:39:57 2023, max compression
```

## Comparing `plemmy-0.3.2.tar` & `plemmy-0.3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-20 23:47:13.810187 plemmy-0.3.2/
--rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-07-20 23:46:22.000000 plemmy-0.3.2/LICENSE
--rw-r--r--   0 tjkessler   (501) staff       (20)     2658 2023-07-20 23:47:13.810017 plemmy-0.3.2/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)     2372 2023-07-20 23:46:22.000000 plemmy-0.3.2/README.md
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-20 23:47:13.808878 plemmy-0.3.2/plemmy/
--rw-r--r--   0 tjkessler   (501) staff       (20)      209 2023-07-20 23:46:22.000000 plemmy-0.3.2/plemmy/__init__.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    71480 2023-07-20 23:46:22.000000 plemmy-0.3.2/plemmy/lemmyhttp.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    13987 2023-07-20 23:46:22.000000 plemmy-0.3.2/plemmy/objects.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    19231 2023-07-20 23:46:22.000000 plemmy-0.3.2/plemmy/responses.py
--rw-r--r--   0 tjkessler   (501) staff       (20)     2866 2023-07-20 23:46:22.000000 plemmy-0.3.2/plemmy/utils.py
--rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-07-20 23:46:37.000000 plemmy-0.3.2/plemmy/version.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    16980 2023-07-20 23:46:22.000000 plemmy-0.3.2/plemmy/views.py
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-20 23:47:13.809794 plemmy-0.3.2/plemmy.egg-info/
--rw-r--r--   0 tjkessler   (501) staff       (20)     2658 2023-07-20 23:47:13.000000 plemmy-0.3.2/plemmy.egg-info/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)      331 2023-07-20 23:47:13.000000 plemmy-0.3.2/plemmy.egg-info/SOURCES.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-20 23:47:13.000000 plemmy-0.3.2/plemmy.egg-info/dependency_links.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-20 23:47:13.000000 plemmy-0.3.2/plemmy.egg-info/not-zip-safe
--rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-07-20 23:47:13.000000 plemmy-0.3.2/plemmy.egg-info/requires.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-07-20 23:47:13.000000 plemmy-0.3.2/plemmy.egg-info/top_level.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-07-20 23:47:13.810240 plemmy-0.3.2/setup.cfg
--rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-07-20 23:46:22.000000 plemmy-0.3.2/setup.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-22 19:39:57.227370 plemmy-0.3.3/
+-rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-07-20 23:46:22.000000 plemmy-0.3.3/LICENSE
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2704 2023-07-22 19:39:57.227148 plemmy-0.3.3/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2418 2023-07-22 19:39:18.000000 plemmy-0.3.3/README.md
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-22 19:39:57.225731 plemmy-0.3.3/plemmy/
+-rw-r--r--   0 tjkessler   (501) staff       (20)      209 2023-07-20 23:46:22.000000 plemmy-0.3.3/plemmy/__init__.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    71480 2023-07-20 23:46:22.000000 plemmy-0.3.3/plemmy/lemmyhttp.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    13987 2023-07-20 23:46:22.000000 plemmy-0.3.3/plemmy/objects.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    19231 2023-07-20 23:46:22.000000 plemmy-0.3.3/plemmy/responses.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2907 2023-07-22 19:36:24.000000 plemmy-0.3.3/plemmy/utils.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-07-22 19:38:24.000000 plemmy-0.3.3/plemmy/version.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    16980 2023-07-20 23:46:22.000000 plemmy-0.3.3/plemmy/views.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-22 19:39:57.226833 plemmy-0.3.3/plemmy.egg-info/
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2704 2023-07-22 19:39:57.000000 plemmy-0.3.3/plemmy.egg-info/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)      331 2023-07-22 19:39:57.000000 plemmy-0.3.3/plemmy.egg-info/SOURCES.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-22 19:39:57.000000 plemmy-0.3.3/plemmy.egg-info/dependency_links.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-22 19:39:57.000000 plemmy-0.3.3/plemmy.egg-info/not-zip-safe
+-rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-07-22 19:39:57.000000 plemmy-0.3.3/plemmy.egg-info/requires.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-07-22 19:39:57.000000 plemmy-0.3.3/plemmy.egg-info/top_level.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-07-22 19:39:57.227424 plemmy-0.3.3/setup.cfg
+-rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-07-20 23:46:22.000000 plemmy-0.3.3/setup.py
```

### Comparing `plemmy-0.3.2/LICENSE` & `plemmy-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.2/PKG-INFO` & `plemmy-0.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: plemmy
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python API for LemmyHttp
 Home-page: https://github.com/tjkessler/plemmy
 Author: Travis Kessler
 Author-email: travis.j.kessler@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Plemmy: a Python package for accessing the Lemmy API
 
-<img src="img/plemmy.png" alt="drawing" width="325"/>
+<img src="https://github.com/tjkessler/plemmy/blob/main/img/plemmy.png" alt="drawing" width="325"/>
 
 [![GitHub version](https://badge.fury.io/gh/tjkessler%2Fplemmy.svg)](https://badge.fury.io/gh/tjkessler%2Fplemmy)
 [![PyPI version](https://badge.fury.io/py/plemmy.svg)](https://badge.fury.io/py/plemmy)
 [![GitHub license](https://img.shields.io/badge/license-Apache-blue.svg)](https://raw.githubusercontent.com/tjkessler/plemmy/master/LICENSE.txt)
 
 Plemmy allows you to interact with any Lemmy instance using Python and the [LemmyHttp API](https://join-lemmy.org/api/classes/LemmyHttp.html).
```

### Comparing `plemmy-0.3.2/README.md` & `plemmy-0.3.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Plemmy: a Python package for accessing the Lemmy API
 
-<img src="img/plemmy.png" alt="drawing" width="325"/>
+<img src="https://github.com/tjkessler/plemmy/blob/main/img/plemmy.png" alt="drawing" width="325"/>
 
 [![GitHub version](https://badge.fury.io/gh/tjkessler%2Fplemmy.svg)](https://badge.fury.io/gh/tjkessler%2Fplemmy)
 [![PyPI version](https://badge.fury.io/py/plemmy.svg)](https://badge.fury.io/py/plemmy)
 [![GitHub license](https://img.shields.io/badge/license-Apache-blue.svg)](https://raw.githubusercontent.com/tjkessler/plemmy/master/LICENSE.txt)
 
 Plemmy allows you to interact with any Lemmy instance using Python and the [LemmyHttp API](https://join-lemmy.org/api/classes/LemmyHttp.html).
```

### Comparing `plemmy-0.3.2/plemmy/lemmyhttp.py` & `plemmy-0.3.3/plemmy/lemmyhttp.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.2/plemmy/objects.py` & `plemmy-0.3.3/plemmy/objects.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.2/plemmy/responses.py` & `plemmy-0.3.3/plemmy/responses.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.2/plemmy/utils.py` & `plemmy-0.3.3/plemmy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,10 +80,9 @@
 
     Args:
         arguments (dict): function arguments supplied with locals()
 
     Returns:
         dict: constructed dictionary/form
     """
-
-    return {k: v for k, v in arguments.items()
+    return {k: str(v).lower() if isinstance(v, bool) else v for k, v in arguments.items()
             if v is not None and k != "self"}
```

### Comparing `plemmy-0.3.2/plemmy/views.py` & `plemmy-0.3.3/plemmy/views.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.2/plemmy.egg-info/PKG-INFO` & `plemmy-0.3.3/plemmy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: plemmy
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python API for LemmyHttp
 Home-page: https://github.com/tjkessler/plemmy
 Author: Travis Kessler
 Author-email: travis.j.kessler@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Plemmy: a Python package for accessing the Lemmy API
 
-<img src="img/plemmy.png" alt="drawing" width="325"/>
+<img src="https://github.com/tjkessler/plemmy/blob/main/img/plemmy.png" alt="drawing" width="325"/>
 
 [![GitHub version](https://badge.fury.io/gh/tjkessler%2Fplemmy.svg)](https://badge.fury.io/gh/tjkessler%2Fplemmy)
 [![PyPI version](https://badge.fury.io/py/plemmy.svg)](https://badge.fury.io/py/plemmy)
 [![GitHub license](https://img.shields.io/badge/license-Apache-blue.svg)](https://raw.githubusercontent.com/tjkessler/plemmy/master/LICENSE.txt)
 
 Plemmy allows you to interact with any Lemmy instance using Python and the [LemmyHttp API](https://join-lemmy.org/api/classes/LemmyHttp.html).
```

### Comparing `plemmy-0.3.2/setup.py` & `plemmy-0.3.3/setup.py`

 * *Files identical despite different names*

