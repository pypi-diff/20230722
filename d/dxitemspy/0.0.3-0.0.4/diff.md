# Comparing `tmp/dxitemspy-0.0.3.tar.gz` & `tmp/dxitemspy-0.0.4.tar.gz`

## Comparing `dxitemspy-0.0.3.tar` & `dxitemspy-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/src/dxitemspy/__about__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/src/dxitemspy/__init__.py
--rw-r--r--   0        0        0 21243725 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/src/dxitemspy/dxi_mapping.json
--rw-r--r--   0        0        0   619732 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/src/dxitemspy/dxi_metadata.json
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/src/dxitemspy/dxitems.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/src/dxitemspy/parse_dxi_mapping.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/src/dxitemspy/parse_dxi_meta.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/tests/dxi_test.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/README.md
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 dxitemspy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 dxitemspy-0.0.4/src/dxitemspy/__about__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 dxitemspy-0.0.4/src/dxitemspy/__init__.py
+-rw-r--r--   0        0        0 21243725 2020-02-02 00:00:00.000000 dxitemspy-0.0.4/src/dxitemspy/dxi_mapping.json
+-rw-r--r--   0        0        0   619732 2020-02-02 00:00:00.000000 dxitemspy-0.0.4/src/dxitemspy/dxi_metadata.json
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 dxitemspy-0.0.4/src/dxitemspy/dxitems.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 dxitemspy-0.0.4/src/dxitemspy/parse_dxi_mapping.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 dxitemspy-0.0.4/src/dxitemspy/parse_dxi_meta.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 dxitemspy-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 dxitemspy-0.0.4/tests/dxi_test.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 dxitemspy-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 dxitemspy-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 dxitemspy-0.0.4/README.md
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 dxitemspy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 dxitemspy-0.0.4/PKG-INFO
```

### Comparing `dxitemspy-0.0.3/src/dxitemspy/dxi_mapping.json` & `dxitemspy-0.0.4/src/dxitemspy/dxi_mapping.json`

 * *Files identical despite different names*

### Comparing `dxitemspy-0.0.3/src/dxitemspy/dxi_metadata.json` & `dxitemspy-0.0.4/src/dxitemspy/dxi_metadata.json`

 * *Files identical despite different names*

### Comparing `dxitemspy-0.0.3/src/dxitemspy/dxitems.py` & `dxitemspy-0.0.4/src/dxitemspy/dxitems.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import json
 import csv
 import re
-
+from pkg_resources import resource_filename as rscfn
 class DXIEngine:
 
     def __init__(self):
 
-        fn_mapping = "dxitemspy/dxi_mapping.json"
-        fn_metadata = "dxitemspy/dxi_metadata.json"
         self.dxi_mapping = {}
         self.dxi_metadata = {}
+        fn_mapping = rscfn(__name__, 'dxi_mapping.json')
         with open(fn_mapping, "r") as fp:
-            self.dxi_mapping = json.load(fp)
+            self.dxi_mapping = json.load(fp)   
+        fn_metadata = rscfn(__name__, 'dxi_mapping.json')
         with open(fn_metadata, "r") as fp:
-            self.dxi_metadata = json.load(fp)
+            self.dxi_metadata = json.load(fp)   
 
     def get_dxi(self, dx_lst):
 
         dx2dxi = {} 
         labels = []
         for dx in set(dx_lst):
             if dx in self.dxi_mapping:
```

### Comparing `dxitemspy-0.0.3/src/dxitemspy/parse_dxi_mapping.py` & `dxitemspy-0.0.4/src/dxitemspy/parse_dxi_mapping.py`

 * *Files identical despite different names*

### Comparing `dxitemspy-0.0.3/src/dxitemspy/parse_dxi_meta.py` & `dxitemspy-0.0.4/src/dxitemspy/parse_dxi_meta.py`

 * *Files identical despite different names*

### Comparing `dxitemspy-0.0.3/LICENSE.txt` & `dxitemspy-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dxitemspy-0.0.3/README.md` & `dxitemspy-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dxitemspy-0.0.3/pyproject.toml` & `dxitemspy-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dxitemspy-0.0.3/PKG-INFO` & `dxitemspy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxitemspy
-Version: 0.0.3
+Version: 0.0.4
 Project-URL: Documentation, https://github.com/yubin-park/dxitemspy#readme
 Project-URL: Issues, https://github.com/yubin-park/dxitemspy/issues
 Project-URL: Source, https://github.com/yubin-park/dxitemspy
 Author-email: yubin-park <yubin.park@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

