# Comparing `tmp/types-s2clientprotocol-5.0.0.0.tar.gz` & `tmp/types-s2clientprotocol-5.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-s2clientprotocol-5.0.0.0.tar", last modified: Fri Jul 21 18:19:05 2023, max compression
+gzip compressed data, was "types-s2clientprotocol-5.0.0.1.tar", last modified: Sat Jul 22 21:12:13 2023, max compression
```

## Comparing `types-s2clientprotocol-5.0.0.0.tar` & `types-s2clientprotocol-5.0.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:19:05.846898 types-s2clientprotocol-5.0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-21 18:19:03.000000 types-s2clientprotocol-5.0.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-21 18:19:03.000000 types-s2clientprotocol-5.0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-21 18:19:05.846898 types-s2clientprotocol-5.0.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:19:05.846898 types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-21 18:19:03.000000 types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-21 18:18:46.000000 types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/build.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-21 18:18:46.000000 types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-07-21 18:18:46.000000 types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/data_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18423 2023-07-21 18:18:46.000000 types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/debug_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24184 2023-07-21 18:18:46.000000 types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/error_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-07-21 18:18:46.000000 types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/query_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    31822 2023-07-21 18:18:46.000000 types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/raw_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    96186 2023-07-21 18:18:46.000000 types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/sc2api_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15558 2023-07-21 18:18:46.000000 types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/score_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23431 2023-07-21 18:18:46.000000 types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/spatial_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24710 2023-07-21 18:18:46.000000 types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/ui_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 18:19:05.846898 types-s2clientprotocol-5.0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-21 18:19:03.000000 types-s2clientprotocol-5.0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:19:05.846898 types-s2clientprotocol-5.0.0.0/types_s2clientprotocol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-21 18:19:05.000000 types-s2clientprotocol-5.0.0.0/types_s2clientprotocol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-21 18:19:05.000000 types-s2clientprotocol-5.0.0.0/types_s2clientprotocol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 18:19:05.000000 types-s2clientprotocol-5.0.0.0/types_s2clientprotocol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 18:19:05.000000 types-s2clientprotocol-5.0.0.0/types_s2clientprotocol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 18:19:05.000000 types-s2clientprotocol-5.0.0.0/types_s2clientprotocol.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:12:13.717752 types-s2clientprotocol-5.0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-22 21:12:12.000000 types-s2clientprotocol-5.0.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-22 21:12:12.000000 types-s2clientprotocol-5.0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-22 21:12:13.717752 types-s2clientprotocol-5.0.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:12:13.713752 types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-22 21:12:12.000000 types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-22 21:11:45.000000 types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-22 21:11:45.000000 types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-07-22 21:11:45.000000 types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/data_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18423 2023-07-22 21:11:45.000000 types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/debug_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24184 2023-07-22 21:11:45.000000 types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/error_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-07-22 21:11:45.000000 types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/query_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    31822 2023-07-22 21:11:45.000000 types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/raw_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    96186 2023-07-22 21:11:45.000000 types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/sc2api_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15558 2023-07-22 21:11:45.000000 types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/score_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23431 2023-07-22 21:11:45.000000 types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/spatial_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24710 2023-07-22 21:11:45.000000 types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/ui_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 21:12:13.717752 types-s2clientprotocol-5.0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-22 21:12:12.000000 types-s2clientprotocol-5.0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:12:13.713752 types-s2clientprotocol-5.0.0.1/types_s2clientprotocol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-22 21:12:13.000000 types-s2clientprotocol-5.0.0.1/types_s2clientprotocol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-22 21:12:13.000000 types-s2clientprotocol-5.0.0.1/types_s2clientprotocol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 21:12:13.000000 types-s2clientprotocol-5.0.0.1/types_s2clientprotocol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-22 21:12:13.000000 types-s2clientprotocol-5.0.0.1/types_s2clientprotocol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-22 21:12:13.000000 types-s2clientprotocol-5.0.0.1/types_s2clientprotocol.egg-info/top_level.txt
```

### Comparing `types-s2clientprotocol-5.0.0.0/PKG-INFO` & `types-s2clientprotocol-5.0.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-s2clientprotocol
-Version: 5.0.0.0
+Version: 5.0.0.1
 Summary: Typing stubs for s2clientprotocol
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/s2clientprotocol.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,10 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `s2clientprotocol`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/s2clientprotocol. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `33588c79080ab81afe207c55af82243aeda11203` and was tested
+This package was generated from typeshed commit `7d33060e6ae3ebe54462a891f0c566c97371915b` and was tested
 with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+pytype 2023.7.21.
```

### Comparing `types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/common_pb2.pyi` & `types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/data_pb2.pyi` & `types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/debug_pb2.pyi` & `types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/debug_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/error_pb2.pyi` & `types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/query_pb2.pyi` & `types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/raw_pb2.pyi` & `types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/raw_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/sc2api_pb2.pyi` & `types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/sc2api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/score_pb2.pyi` & `types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/score_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/spatial_pb2.pyi` & `types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/spatial_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-s2clientprotocol-5.0.0.0/s2clientprotocol-stubs/ui_pb2.pyi` & `types-s2clientprotocol-5.0.0.1/s2clientprotocol-stubs/ui_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-s2clientprotocol-5.0.0.0/setup.py` & `types-s2clientprotocol-5.0.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `s2clientprotocol`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/s2clientprotocol. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `33588c79080ab81afe207c55af82243aeda11203` and was tested
+This package was generated from typeshed commit `7d33060e6ae3ebe54462a891f0c566c97371915b` and was tested
 with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+pytype 2023.7.21.
 '''.lstrip()
 
 setup(name=name,
-      version="5.0.0.0",
+      version="5.0.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/s2clientprotocol.md",
```

### Comparing `types-s2clientprotocol-5.0.0.0/types_s2clientprotocol.egg-info/PKG-INFO` & `types-s2clientprotocol-5.0.0.1/types_s2clientprotocol.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-s2clientprotocol
-Version: 5.0.0.0
+Version: 5.0.0.1
 Summary: Typing stubs for s2clientprotocol
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/s2clientprotocol.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,10 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `s2clientprotocol`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/s2clientprotocol. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `33588c79080ab81afe207c55af82243aeda11203` and was tested
+This package was generated from typeshed commit `7d33060e6ae3ebe54462a891f0c566c97371915b` and was tested
 with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+pytype 2023.7.21.
```

### Comparing `types-s2clientprotocol-5.0.0.0/types_s2clientprotocol.egg-info/SOURCES.txt` & `types-s2clientprotocol-5.0.0.1/types_s2clientprotocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

