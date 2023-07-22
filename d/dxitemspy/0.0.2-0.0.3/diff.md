# Comparing `tmp/dxitemspy-0.0.2.tar.gz` & `tmp/dxitemspy-0.0.3.tar.gz`

## Comparing `dxitemspy-0.0.2.tar` & `dxitemspy-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 dxitemspy-0.0.2/src/dxitemspy/__about__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 dxitemspy-0.0.2/src/dxitemspy/__init__.py
--rw-r--r--   0        0        0 21243725 2020-02-02 00:00:00.000000 dxitemspy-0.0.2/src/dxitemspy/dxi_mapping.json
--rw-r--r--   0        0        0   619732 2020-02-02 00:00:00.000000 dxitemspy-0.0.2/src/dxitemspy/dxi_metadata.json
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 dxitemspy-0.0.2/src/dxitemspy/dxitems.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 dxitemspy-0.0.2/src/dxitemspy/parse_dxi_mapping.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 dxitemspy-0.0.2/src/dxitemspy/parse_dxi_meta.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 dxitemspy-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 dxitemspy-0.0.2/tests/dxi_test.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 dxitemspy-0.0.2/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 dxitemspy-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 dxitemspy-0.0.2/README.md
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 dxitemspy-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 dxitemspy-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/src/dxitemspy/__about__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/src/dxitemspy/__init__.py
+-rw-r--r--   0        0        0 21243725 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/src/dxitemspy/dxi_mapping.json
+-rw-r--r--   0        0        0   619732 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/src/dxitemspy/dxi_metadata.json
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/src/dxitemspy/dxitems.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/src/dxitemspy/parse_dxi_mapping.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/src/dxitemspy/parse_dxi_meta.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/tests/dxi_test.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/README.md
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/PKG-INFO
```

### Comparing `dxitemspy-0.0.2/src/dxitemspy/dxi_mapping.json` & `dxitemspy-0.0.3/src/dxitemspy/dxi_mapping.json`

 * *Files identical despite different names*

### Comparing `dxitemspy-0.0.2/src/dxitemspy/dxi_metadata.json` & `dxitemspy-0.0.3/src/dxitemspy/dxi_metadata.json`

 * *Files identical despite different names*

### Comparing `dxitemspy-0.0.2/src/dxitemspy/dxitems.py` & `dxitemspy-0.0.3/src/dxitemspy/dxitems.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import csv
 import re
 
 class DXIEngine:
 
     def __init__(self):
 
-        fn_mapping = "src/dxitemspy/dxi_mapping.json"
-        fn_metadata = "src/dxitemspy/dxi_metadata.json"
+        fn_mapping = "dxitemspy/dxi_mapping.json"
+        fn_metadata = "dxitemspy/dxi_metadata.json"
         self.dxi_mapping = {}
         self.dxi_metadata = {}
         with open(fn_mapping, "r") as fp:
             self.dxi_mapping = json.load(fp)
         with open(fn_metadata, "r") as fp:
             self.dxi_metadata = json.load(fp)
```

### Comparing `dxitemspy-0.0.2/src/dxitemspy/parse_dxi_mapping.py` & `dxitemspy-0.0.3/src/dxitemspy/parse_dxi_mapping.py`

 * *Files identical despite different names*

### Comparing `dxitemspy-0.0.2/src/dxitemspy/parse_dxi_meta.py` & `dxitemspy-0.0.3/src/dxitemspy/parse_dxi_meta.py`

 * *Files identical despite different names*

### Comparing `dxitemspy-0.0.2/LICENSE.txt` & `dxitemspy-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dxitemspy-0.0.2/README.md` & `dxitemspy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dxitemspy-0.0.2/pyproject.toml` & `dxitemspy-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dxitemspy-0.0.2/PKG-INFO` & `dxitemspy-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxitemspy
-Version: 0.0.2
+Version: 0.0.3
 Project-URL: Documentation, https://github.com/yubin-park/dxitemspy#readme
 Project-URL: Issues, https://github.com/yubin-park/dxitemspy/issues
 Project-URL: Source, https://github.com/yubin-park/dxitemspy
 Author-email: yubin-park <yubin.park@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

