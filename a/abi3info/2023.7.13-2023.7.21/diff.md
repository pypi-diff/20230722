# Comparing `tmp/abi3info-2023.7.13.tar.gz` & `tmp/abi3info-2023.7.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abi3info-2023.7.13.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "abi3info-2023.7.21.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `abi3info-2023.7.13.tar` & `abi3info-2023.7.21.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1109 2023-07-13 05:01:38.633352 abi3info-2023.7.13/LICENSE
--rw-r--r--   0        0        0     1915 2023-07-13 05:01:38.633352 abi3info-2023.7.13/README.md
--rw-r--r--   0        0        0     1038 2023-07-13 05:01:38.633352 abi3info-2023.7.13/abi3info/__init__.py
--rw-r--r--   0        0        0   191351 2023-07-13 05:01:38.633352 abi3info-2023.7.13/abi3info/_internal.py
--rw-r--r--   0        0        0     7791 2023-07-13 05:01:38.633352 abi3info-2023.7.13/abi3info/models.py
--rw-r--r--   0        0        0     1885 2023-07-13 05:01:38.633352 abi3info-2023.7.13/pyproject.toml
--rw-r--r--   0        0        0     3462 1970-01-01 00:00:00.000000 abi3info-2023.7.13/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-07-22 03:23:25.607255 abi3info-2023.7.21/LICENSE
+-rw-r--r--   0        0        0     1915 2023-07-22 03:23:25.607255 abi3info-2023.7.21/README.md
+-rw-r--r--   0        0        0     1038 2023-07-22 03:23:25.607255 abi3info-2023.7.21/abi3info/__init__.py
+-rw-r--r--   0        0        0   191533 2023-07-22 03:23:25.607255 abi3info-2023.7.21/abi3info/_internal.py
+-rw-r--r--   0        0        0     7791 2023-07-22 03:23:25.607255 abi3info-2023.7.21/abi3info/models.py
+-rw-r--r--   0        0        0     1885 2023-07-22 03:23:25.607255 abi3info-2023.7.21/pyproject.toml
+-rw-r--r--   0        0        0     3462 1970-01-01 00:00:00.000000 abi3info-2023.7.21/PKG-INFO
```

### Comparing `abi3info-2023.7.13/LICENSE` & `abi3info-2023.7.21/LICENSE`

 * *Files identical despite different names*

### Comparing `abi3info-2023.7.13/README.md` & `abi3info-2023.7.21/README.md`

 * *Files identical despite different names*

### Comparing `abi3info-2023.7.13/abi3info/__init__.py` & `abi3info-2023.7.21/abi3info/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Function,
     Macro,
     Struct,
     Symbol,
     Typedef,
 )
 
-__version__ = "2023.07.13"
+__version__ = "2023.07.21"
 """
 The current version of abi3info.
 """
 
 DATAS: Final[dict[Symbol, Data]] = _DATAS
 """
 Data object members of the limited API and stable ABI.
```

### Comparing `abi3info-2023.7.13/abi3info/_internal.py` & `abi3info-2023.7.21/abi3info/_internal.py`

 * *Files 0% similar despite different names*

```diff
@@ -4481,14 +4481,20 @@
     ),
     Symbol(name="PyMapping_GetOptionalItemString"): Function(
         symbol=Symbol(name="PyMapping_GetOptionalItemString"),
         added=PyVersion(major=3, minor=13),
         ifdef=None,
         abi_only=False,
     ),
+    Symbol(name="PyModule_Add"): Function(
+        symbol=Symbol(name="PyModule_Add"),
+        added=PyVersion(major=3, minor=13),
+        ifdef=None,
+        abi_only=False,
+    ),
 }
 _MACROS: Final[dict[str, Macro]] = {
     "Py_tp_dealloc": Macro(name="Py_tp_dealloc", added=PyVersion(major=3, minor=2)),
     "Py_tp_getattr": Macro(name="Py_tp_getattr", added=PyVersion(major=3, minor=2)),
     "Py_tp_setattr": Macro(name="Py_tp_setattr", added=PyVersion(major=3, minor=2)),
     "Py_tp_repr": Macro(name="Py_tp_repr", added=PyVersion(major=3, minor=2)),
     "Py_tp_hash": Macro(name="Py_tp_hash", added=PyVersion(major=3, minor=2)),
```

### Comparing `abi3info-2023.7.13/abi3info/models.py` & `abi3info-2023.7.21/abi3info/models.py`

 * *Files identical despite different names*

### Comparing `abi3info-2023.7.13/pyproject.toml` & `abi3info-2023.7.21/pyproject.toml`

 * *Files identical despite different names*

### Comparing `abi3info-2023.7.13/PKG-INFO` & `abi3info-2023.7.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abi3info
-Version: 2023.7.13
+Version: 2023.7.21
 Summary: A library for abi3 and other CPython API information
 Author-email: William Woodruff <william@yossarian.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
```

