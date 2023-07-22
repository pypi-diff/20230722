# Comparing `tmp/types-protobuf-4.23.0.1.tar.gz` & `tmp/types-protobuf-4.23.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-protobuf-4.23.0.1.tar", last modified: Wed May 10 15:22:27 2023, max compression
+gzip compressed data, was "types-protobuf-4.23.0.2.tar", last modified: Sat Jul 22 15:13:31 2023, max compression
```

## Comparing `types-protobuf-4.23.0.1.tar` & `types-protobuf-4.23.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:27.012899 types-protobuf-4.23.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-10 15:22:26.000000 types-protobuf-4.23.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:22:26.000000 types-protobuf-4.23.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-10 15:22:27.012899 types-protobuf-4.23.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:27.004899 types-protobuf-4.23.0.1/google-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-10 15:22:26.000000 types-protobuf-4.23.0.1/google-stubs/METADATA.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:27.008899 types-protobuf-4.23.0.1/google-stubs/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/any_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/api_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:27.012899 types-protobuf-4.23.0.1/google-stubs/protobuf/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/compiler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/compiler/plugin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/descriptor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    76549 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/descriptor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/descriptor_pool.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/duration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/empty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/field_mask_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:27.012899 types-protobuf-4.23.0.1/google-stubs/protobuf/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/internal/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/internal/api_implementation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/internal/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/internal/decoder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/internal/encoder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/internal/enum_type_wrapper.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/internal/extension_dict.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/internal/message_listener.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/internal/python_message.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/internal/type_checkers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/internal/well_known_types.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/internal/wire_format.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/json_format.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/message.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/message_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/reflection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/source_context_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/struct_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/symbol_database.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/text_format.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/timestamp_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16140 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/type_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:27.012899 types-protobuf-4.23.0.1/google-stubs/protobuf/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/util/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-10 15:19:44.000000 types-protobuf-4.23.0.1/google-stubs/protobuf/wrappers_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:22:27.016899 types-protobuf-4.23.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-10 15:22:26.000000 types-protobuf-4.23.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:27.012899 types-protobuf-4.23.0.1/types_protobuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-10 15:22:26.000000 types-protobuf-4.23.0.1/types_protobuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-10 15:22:26.000000 types-protobuf-4.23.0.1/types_protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:22:26.000000 types-protobuf-4.23.0.1/types_protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 15:22:26.000000 types-protobuf-4.23.0.1/types_protobuf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:31.595401 types-protobuf-4.23.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-22 15:13:29.000000 types-protobuf-4.23.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-22 15:13:29.000000 types-protobuf-4.23.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-22 15:13:31.595401 types-protobuf-4.23.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:31.591401 types-protobuf-4.23.0.2/google-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-22 15:13:29.000000 types-protobuf-4.23.0.2/google-stubs/METADATA.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:31.595401 types-protobuf-4.23.0.2/google-stubs/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/any_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/api_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:31.595401 types-protobuf-4.23.0.2/google-stubs/protobuf/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/compiler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/compiler/plugin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/descriptor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    76549 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/descriptor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/descriptor_pool.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/duration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/empty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/field_mask_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:31.595401 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/api_implementation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/decoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/encoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/enum_type_wrapper.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/extension_dict.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/message_listener.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/python_message.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/type_checkers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/well_known_types.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/wire_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/json_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/message.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/message_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/reflection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/source_context_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/struct_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/symbol_database.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/text_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/timestamp_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16140 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/type_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:31.595401 types-protobuf-4.23.0.2/google-stubs/protobuf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/util/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/wrappers_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 15:13:31.595401 types-protobuf-4.23.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-22 15:13:29.000000 types-protobuf-4.23.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:31.595401 types-protobuf-4.23.0.2/types_protobuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-22 15:13:31.000000 types-protobuf-4.23.0.2/types_protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-22 15:13:31.000000 types-protobuf-4.23.0.2/types_protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 15:13:31.000000 types-protobuf-4.23.0.2/types_protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-22 15:13:31.000000 types-protobuf-4.23.0.2/types_protobuf.egg-info/top_level.txt
```

### Comparing `types-protobuf-4.23.0.1/CHANGELOG.md` & `types-protobuf-4.23.0.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 4.23.0.2 (2023-07-22)
+
+Pretend `_EnumTypeWrapper` inherits from `type` (#10203)
+
+Pretend `google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper` inherits from `type`. It doesn't really, but this makes type checkers stop complaining when you use it as a metaclass, which is the only reason the class exists.
+
 ## 4.23.0.1 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
 
 ## 4.23.0.0 (2023-05-09)
 
 [stubsabot] Bump protobuf to 4.23.* (#10158)
```

### Comparing `types-protobuf-4.23.0.1/PKG-INFO` & `types-protobuf-4.23.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-protobuf
-Version: 4.23.0.1
+Version: 4.23.0.2
 Summary: Typing stubs for protobuf
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/protobuf.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -23,9 +23,15 @@
 PyCharm, etc. to check code that uses
 `protobuf`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/protobuf. All fixes for
 types and metadata should be contributed there.
 
 Generated with aid from mypy-protobuf v3.4.0
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `53a893279713c8abcc970a578d6f28e97efdd68f` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.7.21.
```

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/any_pb2.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/any_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/api_pb2.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/compiler/plugin_pb2.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/compiler/plugin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/descriptor.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/descriptor.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/descriptor_pb2.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/descriptor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/descriptor_pool.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/descriptor_pool.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/duration_pb2.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/duration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/empty_pb2.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/empty_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/field_mask_pb2.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/field_mask_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/internal/containers.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/internal/containers.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/internal/decoder.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/internal/decoder.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/internal/encoder.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/internal/encoder.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/internal/enum_type_wrapper.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/internal/enum_type_wrapper.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 
 from google.protobuf.descriptor import EnumDescriptor
 
 _V = TypeVar("_V", bound=int)
 
 # Expose a generic version so that those using mypy-protobuf
 # can get autogenerated NewType wrapper around the int values
-class _EnumTypeWrapper(Generic[_V]):
+# NOTE: this doesn't actually inherit from type,
+# but mypy doesn't support metaclasses that don't inherit from type,
+# so we pretend it does in the stubs...
+class _EnumTypeWrapper(type, Generic[_V]):
     DESCRIPTOR: EnumDescriptor
     def __init__(self, enum_type: EnumDescriptor) -> None: ...
     def Name(self, number: _V) -> str: ...
     def Value(self, name: str | bytes) -> _V: ...
     def keys(self) -> list[str]: ...
     def values(self) -> list[_V]: ...
     def items(self) -> list[tuple[str, _V]]: ...
```

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/internal/extension_dict.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/internal/extension_dict.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/internal/well_known_types.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/internal/well_known_types.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/internal/wire_format.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/internal/wire_format.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/json_format.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/json_format.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/message.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/message.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/message_factory.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/message_factory.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/service.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/service.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/source_context_pb2.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/source_context_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/struct_pb2.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/struct_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/symbol_database.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/symbol_database.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/text_format.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/text_format.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/timestamp_pb2.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/timestamp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/type_pb2.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/google-stubs/protobuf/wrappers_pb2.pyi` & `types-protobuf-4.23.0.2/google-stubs/protobuf/wrappers_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.1/setup.py` & `types-protobuf-4.23.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,33 +13,39 @@
 PyCharm, etc. to check code that uses
 `protobuf`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/protobuf. All fixes for
 types and metadata should be contributed there.
 
 Generated with aid from mypy-protobuf v3.4.0
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `53a893279713c8abcc970a578d6f28e97efdd68f` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.7.21.
 '''.lstrip()
 
 setup(name=name,
-      version="4.23.0.1",
+      version="4.23.0.2",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/protobuf.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['google-stubs'],
-      package_data={'google-stubs': ['protobuf/__init__.pyi', 'protobuf/any_pb2.pyi', 'protobuf/api_pb2.pyi', 'protobuf/compiler/__init__.pyi', 'protobuf/compiler/plugin_pb2.pyi', 'protobuf/descriptor.pyi', 'protobuf/descriptor_pb2.pyi', 'protobuf/descriptor_pool.pyi', 'protobuf/duration_pb2.pyi', 'protobuf/empty_pb2.pyi', 'protobuf/field_mask_pb2.pyi', 'protobuf/internal/__init__.pyi', 'protobuf/internal/api_implementation.pyi', 'protobuf/internal/containers.pyi', 'protobuf/internal/decoder.pyi', 'protobuf/internal/encoder.pyi', 'protobuf/internal/enum_type_wrapper.pyi', 'protobuf/internal/extension_dict.pyi', 'protobuf/internal/message_listener.pyi', 'protobuf/internal/python_message.pyi', 'protobuf/internal/type_checkers.pyi', 'protobuf/internal/well_known_types.pyi', 'protobuf/internal/wire_format.pyi', 'protobuf/json_format.pyi', 'protobuf/message.pyi', 'protobuf/message_factory.pyi', 'protobuf/reflection.pyi', 'protobuf/service.pyi', 'protobuf/source_context_pb2.pyi', 'protobuf/struct_pb2.pyi', 'protobuf/symbol_database.pyi', 'protobuf/text_format.pyi', 'protobuf/timestamp_pb2.pyi', 'protobuf/type_pb2.pyi', 'protobuf/util/__init__.pyi', 'protobuf/wrappers_pb2.pyi', 'METADATA.toml']},
+      package_data={'google-stubs': ['protobuf/__init__.pyi', 'protobuf/any_pb2.pyi', 'protobuf/api_pb2.pyi', 'protobuf/compiler/__init__.pyi', 'protobuf/compiler/plugin_pb2.pyi', 'protobuf/descriptor.pyi', 'protobuf/descriptor_pb2.pyi', 'protobuf/descriptor_pool.pyi', 'protobuf/duration_pb2.pyi', 'protobuf/empty_pb2.pyi', 'protobuf/field_mask_pb2.pyi', 'protobuf/internal/__init__.pyi', 'protobuf/internal/api_implementation.pyi', 'protobuf/internal/containers.pyi', 'protobuf/internal/decoder.pyi', 'protobuf/internal/encoder.pyi', 'protobuf/internal/enum_type_wrapper.pyi', 'protobuf/internal/extension_dict.pyi', 'protobuf/internal/message_listener.pyi', 'protobuf/internal/python_message.pyi', 'protobuf/internal/type_checkers.pyi', 'protobuf/internal/well_known_types.pyi', 'protobuf/internal/wire_format.pyi', 'protobuf/json_format.pyi', 'protobuf/message.pyi', 'protobuf/message_factory.pyi', 'protobuf/reflection.pyi', 'protobuf/service.pyi', 'protobuf/source_context_pb2.pyi', 'protobuf/struct_pb2.pyi', 'protobuf/symbol_database.pyi', 'protobuf/text_format.pyi', 'protobuf/timestamp_pb2.pyi', 'protobuf/type_pb2.pyi', 'protobuf/util/__init__.pyi', 'protobuf/wrappers_pb2.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-protobuf-4.23.0.1/types_protobuf.egg-info/PKG-INFO` & `types-protobuf-4.23.0.2/types_protobuf.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-protobuf
-Version: 4.23.0.1
+Version: 4.23.0.2
 Summary: Typing stubs for protobuf
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/protobuf.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -23,9 +23,15 @@
 PyCharm, etc. to check code that uses
 `protobuf`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/protobuf. All fixes for
 types and metadata should be contributed there.
 
 Generated with aid from mypy-protobuf v3.4.0
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `53a893279713c8abcc970a578d6f28e97efdd68f` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.7.21.
```

### Comparing `types-protobuf-4.23.0.1/types_protobuf.egg-info/SOURCES.txt` & `types-protobuf-4.23.0.2/types_protobuf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

