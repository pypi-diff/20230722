# Comparing `tmp/scilint-0.2.0.tar.gz` & `tmp/scilint-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scilint-0.2.0.tar", last modified: Mon Jul 17 09:55:11 2023, max compression
+gzip compressed data, was "scilint-0.2.1.tar", last modified: Sat Jul 22 19:31:35 2023, max compression
```

## Comparing `scilint-0.2.0.tar` & `scilint-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:55:11.653639 scilint-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-07-17 09:53:13.000000 scilint-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-17 09:53:13.000000 scilint-0.2.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-07-17 09:55:11.653639 scilint-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17398 2023-07-17 09:54:49.000000 scilint-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-17 09:53:13.000000 scilint-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:55:11.649639 scilint-0.2.0/scilint/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 09:54:31.000000 scilint-0.2.0/scilint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28316 2023-07-17 09:54:49.000000 scilint-0.2.0/scilint/_modidx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:55:11.653639 scilint-0.2.0/scilint/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:54:31.000000 scilint-0.2.0/scilint/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-17 09:54:30.000000 scilint-0.2.0/scilint/experimental/test_nbdev.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:55:11.653639 scilint-0.2.0/scilint/exploratory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:54:31.000000 scilint-0.2.0/scilint/exploratory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-17 09:54:30.000000 scilint-0.2.0/scilint/exploratory/test_nbdev.py
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-07-17 09:54:30.000000 scilint-0.2.0/scilint/indicators.py
--rw-r--r--   0 runner    (1001) docker     (123)    16421 2023-07-17 09:54:31.000000 scilint-0.2.0/scilint/scilint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:55:11.653639 scilint-0.2.0/scilint/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:54:31.000000 scilint-0.2.0/scilint/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-17 09:54:30.000000 scilint-0.2.0/scilint/test/test_nbdev.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-17 09:54:31.000000 scilint-0.2.0/scilint/test/test_nbdev_high_quality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:55:11.653639 scilint-0.2.0/scilint/validated/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:54:31.000000 scilint-0.2.0/scilint/validated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-17 09:54:31.000000 scilint-0.2.0/scilint/validated/test_nbdev_high_quality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:55:11.653639 scilint-0.2.0/scilint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-07-17 09:55:11.000000 scilint-0.2.0/scilint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-17 09:55:11.000000 scilint-0.2.0/scilint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:55:11.000000 scilint-0.2.0/scilint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-17 09:55:11.000000 scilint-0.2.0/scilint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:53:31.000000 scilint-0.2.0/scilint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 09:55:11.000000 scilint-0.2.0/scilint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 09:55:11.000000 scilint-0.2.0/scilint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 09:55:11.653639 scilint-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-17 09:53:13.000000 scilint-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:31:35.857342 scilint-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-07-22 19:30:00.000000 scilint-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-22 19:30:00.000000 scilint-0.2.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-07-22 19:31:35.857342 scilint-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17398 2023-07-22 19:31:19.000000 scilint-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-22 19:30:00.000000 scilint-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:31:35.853342 scilint-0.2.1/scilint/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 19:31:04.000000 scilint-0.2.1/scilint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28355 2023-07-22 19:31:19.000000 scilint-0.2.1/scilint/_modidx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:31:35.857342 scilint-0.2.1/scilint/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:31:04.000000 scilint-0.2.1/scilint/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-22 19:31:03.000000 scilint-0.2.1/scilint/experimental/test_nbdev.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:31:35.857342 scilint-0.2.1/scilint/exploratory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:31:04.000000 scilint-0.2.1/scilint/exploratory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-22 19:31:03.000000 scilint-0.2.1/scilint/exploratory/test_nbdev.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-07-22 19:31:03.000000 scilint-0.2.1/scilint/indicators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-07-22 19:31:04.000000 scilint-0.2.1/scilint/scilint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:31:35.857342 scilint-0.2.1/scilint/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:31:04.000000 scilint-0.2.1/scilint/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-22 19:31:03.000000 scilint-0.2.1/scilint/test/test_nbdev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-22 19:31:03.000000 scilint-0.2.1/scilint/test/test_nbdev_high_quality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:31:35.857342 scilint-0.2.1/scilint/validated/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:31:04.000000 scilint-0.2.1/scilint/validated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-22 19:31:03.000000 scilint-0.2.1/scilint/validated/test_nbdev_high_quality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:31:35.857342 scilint-0.2.1/scilint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-07-22 19:31:35.000000 scilint-0.2.1/scilint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-22 19:31:35.000000 scilint-0.2.1/scilint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 19:31:35.000000 scilint-0.2.1/scilint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-22 19:31:35.000000 scilint-0.2.1/scilint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 19:30:14.000000 scilint-0.2.1/scilint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-22 19:31:35.000000 scilint-0.2.1/scilint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-22 19:31:35.000000 scilint-0.2.1/scilint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 19:31:35.857342 scilint-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-22 19:30:00.000000 scilint-0.2.1/setup.py
```

### Comparing `scilint-0.2.0/LICENSE` & `scilint-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scilint-0.2.0/NOTICE` & `scilint-0.2.1/NOTICE`

 * *Files identical despite different names*

### Comparing `scilint-0.2.0/PKG-INFO` & `scilint-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scilint
-Version: 0.2.0
+Version: 0.2.1
 Summary: infuse quality into notebook based workflows with a new type of build tool.
 Home-page: https://github.com/newday-data/scilint/tree/{branch}/
 Author: Donal Simmie
 Author-email: oss@newday.co.uk
 License: Apache Software License 2.0
 Project-URL: Documentation, https://newday-data.github.io/scilint/
 Keywords: research,production,exploration,CI/CD
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scilint Version: 0.2.0 Summary: infuse quality into
+Metadata-Version: 2.1 Name: scilint Version: 0.2.1 Summary: infuse quality into
 notebook based workflows with a new type of build tool. Home-page: https://
 github.com/newday-data/scilint/tree/{branch}/ Author: Donal Simmie Author-
 email: oss@newday.co.uk License: Apache Software License 2.0 Project-URL:
 Documentation, https://newday-data.github.io/scilint/ Keywords:
 research,production,exploration,CI/CD Platform: UNKNOWN Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Programming Language ::
```

### Comparing `scilint-0.2.0/README.md` & `scilint-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `scilint-0.2.0/scilint/_modidx.py` & `scilint-0.2.1/scilint/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,40 +59,40 @@
                                                                                                'scilint/exploratory/test_nbdev.py'),
                                                 'scilint.exploratory.test_nbdev.serve_num_topics': ( 'example_nbs/exploratory/nbdev.html#serve_num_topics',
                                                                                                      'scilint/exploratory/test_nbdev.py'),
                                                 'scilint.exploratory.test_nbdev.something': ( 'example_nbs/exploratory/nbdev.html#something',
                                                                                               'scilint/exploratory/test_nbdev.py')},
             'scilint.indicators': { 'scilint.indicators._check_for_function_asserts': ( 'indicators.html#_check_for_function_asserts',
                                                                                         'scilint/indicators.py'),
+                                    'scilint.indicators._count_func_calls': ('indicators.html#_count_func_calls', 'scilint/indicators.py'),
                                     'scilint.indicators._count_func_ret_asserts': ( 'indicators.html#_count_func_ret_asserts',
                                                                                     'scilint/indicators.py'),
                                     'scilint.indicators._count_inline_asserts': ( 'indicators.html#_count_inline_asserts',
                                                                                   'scilint/indicators.py'),
+                                    'scilint.indicators._get_cell_code': ('indicators.html#_get_cell_code', 'scilint/indicators.py'),
+                                    'scilint.indicators._get_func_defs': ('indicators.html#_get_func_defs', 'scilint/indicators.py'),
                                     'scilint.indicators._incr_assert_count': ( 'indicators.html#_incr_assert_count',
                                                                                'scilint/indicators.py'),
                                     'scilint.indicators._tests_per_function_code': ( 'indicators.html#_tests_per_function_code',
                                                                                      'scilint/indicators.py'),
                                     'scilint.indicators._update_ret_vals': ('indicators.html#_update_ret_vals', 'scilint/indicators.py'),
                                     'scilint.indicators.calc_ifp': ('indicators.html#calc_ifp', 'scilint/indicators.py'),
                                     'scilint.indicators.calls_per_func': ('indicators.html#calls_per_func', 'scilint/indicators.py'),
                                     'scilint.indicators.calls_per_func_mean': ( 'indicators.html#calls_per_func_mean',
                                                                                 'scilint/indicators.py'),
                                     'scilint.indicators.calls_per_func_median': ( 'indicators.html#calls_per_func_median',
                                                                                   'scilint/indicators.py'),
-                                    'scilint.indicators.count_func_calls': ('indicators.html#count_func_calls', 'scilint/indicators.py'),
-                                    'scilint.indicators.get_cell_code': ('indicators.html#get_cell_code', 'scilint/indicators.py'),
-                                    'scilint.indicators.get_func_defs': ('indicators.html#get_func_defs', 'scilint/indicators.py'),
                                     'scilint.indicators.get_project_root': ('indicators.html#get_project_root', 'scilint/indicators.py'),
                                     'scilint.indicators.iaf': ('indicators.html#iaf', 'scilint/indicators.py'),
                                     'scilint.indicators.in_func_pct': ('indicators.html#in_func_pct', 'scilint/indicators.py'),
                                     'scilint.indicators.loc_per_md_section': ( 'indicators.html#loc_per_md_section',
                                                                                'scilint/indicators.py'),
                                     'scilint.indicators.markdown_code_pct': ('indicators.html#markdown_code_pct', 'scilint/indicators.py'),
-                                    'scilint.indicators.replace_ipython_magics': ( 'indicators.html#replace_ipython_magics',
-                                                                                   'scilint/indicators.py'),
+                                    'scilint.indicators.remove_ipython_special_directives': ( 'indicators.html#remove_ipython_special_directives',
+                                                                                              'scilint/indicators.py'),
                                     'scilint.indicators.safe_div': ('indicators.html#safe_div', 'scilint/indicators.py'),
                                     'scilint.indicators.tests_func_coverage_pct': ( 'indicators.html#tests_func_coverage_pct',
                                                                                     'scilint/indicators.py'),
                                     'scilint.indicators.tests_per_func_mean': ( 'indicators.html#tests_per_func_mean',
                                                                                 'scilint/indicators.py'),
                                     'scilint.indicators.tests_per_function': ( 'indicators.html#tests_per_function',
                                                                                'scilint/indicators.py'),
```

### Comparing `scilint-0.2.0/scilint/experimental/test_nbdev.py` & `scilint-0.2.1/scilint/experimental/test_nbdev.py`

 * *Files identical despite different names*

### Comparing `scilint-0.2.0/scilint/exploratory/test_nbdev.py` & `scilint-0.2.1/scilint/exploratory/test_nbdev.py`

 * *Files identical despite different names*

### Comparing `scilint-0.2.0/scilint/indicators.py` & `scilint-0.2.1/scilint/indicators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/indicators.ipynb.
 
 # %% auto 0
-__all__ = ['indicator_funcs', 'get_project_root', 'count_func_calls', 'replace_ipython_magics', 'safe_div', 'get_cell_code',
-           'get_func_defs', 'calls_per_func', 'calls_per_func_mean', 'calls_per_func_median', 'iaf',
-           'tests_per_function', 'tests_per_func_mean', 'tests_func_coverage_pct', 'calc_ifp', 'in_func_pct',
-           'markdown_code_pct', 'total_code_len', 'loc_per_md_section']
+__all__ = ['indicator_funcs', 'get_project_root', 'remove_ipython_special_directives', 'safe_div', 'calls_per_func',
+           'calls_per_func_mean', 'calls_per_func_median', 'iaf', 'tests_per_function', 'tests_per_func_mean',
+           'tests_func_coverage_pct', 'calc_ifp', 'in_func_pct', 'markdown_code_pct', 'total_code_len',
+           'loc_per_md_section']
 
 # %% ../nbs/indicators.ipynb 2
 import ast
-import re
 import warnings
 from collections import Counter
 from pathlib import Path
 
 import nbformat
 import numpy as np
 import pandas as pd
 from execnb.nbio import read_nb
 
 # %% ../nbs/indicators.ipynb 7
 def get_project_root(path: Path = Path(".").resolve()):
     return find_project_root(tuple([str()]))
 
 # %% ../nbs/indicators.ipynb 9
-def count_func_calls(code, func_defs):
+def _count_func_calls(code, func_defs):
     func_calls = Counter({k: 0 for k in func_defs})
     for stmt in ast.walk(ast.parse(code)):
         if isinstance(stmt, ast.Call):
             if type(stmt.func) == ast.Subscript:
                 func_name = stmt.func.value.id
             else:
                 func_name = (
@@ -35,53 +34,56 @@
                 )
             if func_name in func_defs:
                 if func_name in func_calls:
                     func_calls[func_name] += 1
     return func_calls
 
 # %% ../nbs/indicators.ipynb 13
-def replace_ipython_magics(code):
-    # Replace Ipython magic and shell command symbol with comment
-    code = code.replace("%", "#")
-    code = re.sub(r"^!", "#", code)
-    return re.sub(r"\n\W?!", "\n#", code)
+def remove_ipython_special_directives(code):
+    lines = code.split("\n")
+    lines = [
+        line
+        for line in lines
+        if not line.strip().startswith("%") and not line.strip().startswith("!")
+    ]
+    return "\n".join(lines)
 
 # %% ../nbs/indicators.ipynb 15
 def safe_div(numer, denom):
     return 0 if denom == 0 else numer / denom
 
 # %% ../nbs/indicators.ipynb 18
-def get_cell_code(nb):
+def _get_cell_code(nb):
     pnb = nbformat.from_dict(nb)
     nb_cell_code = "\n".join(
         [
-            replace_ipython_magics(c["source"])
+            remove_ipython_special_directives(c["source"])
             for c in pnb.cells
             if c["cell_type"] == "code"
         ]
     )
     return nb_cell_code
 
 # %% ../nbs/indicators.ipynb 20
-def get_func_defs(code, ignore_private_prefix=True):
+def _get_func_defs(code, ignore_private_prefix=True):
     func_names = []
     for stmt in ast.walk(ast.parse(code)):
         if isinstance(stmt, ast.FunctionDef):
             inner_cond = (
                 False if ignore_private_prefix and stmt.name.startswith("_") else True
             )
             if inner_cond:
                 func_names.append(stmt.name)
     return func_names
 
 # %% ../nbs/indicators.ipynb 24
 def calls_per_func(nb):
-    nb_cell_code = get_cell_code(nb)
-    func_defs = get_func_defs(nb_cell_code)
-    func_calls = count_func_calls(nb_cell_code, func_defs)
+    nb_cell_code = _get_cell_code(nb)
+    func_defs = _get_func_defs(nb_cell_code)
+    func_calls = _count_func_calls(nb_cell_code, func_defs)
     return func_calls
 
 # %% ../nbs/indicators.ipynb 26
 def calls_per_func_mean(nb):
     return pd.Series(calls_per_func(nb)).mean()
 
 # %% ../nbs/indicators.ipynb 28
@@ -105,24 +107,24 @@
                     )
                     if func_name in inline_func_asserts:
                         inline_func_asserts[func_name] += 1
     return inline_func_asserts
 
 # %% ../nbs/indicators.ipynb 38
 def iaf(nb):
-    nb_cell_code = get_cell_code(nb)
+    nb_cell_code = _get_cell_code(nb)
     if nb_cell_code == "":
         return np.nan
-    func_defs = get_func_defs(nb_cell_code)
+    func_defs = _get_func_defs(nb_cell_code)
     return _count_inline_asserts(nb_cell_code, func_defs)
 
 # %% ../nbs/indicators.ipynb 44
 def _count_func_ret_asserts(nb_cell_code):
     ret_vals = {}
-    func_defs = get_func_defs(nb_cell_code)
+    func_defs = _get_func_defs(nb_cell_code)
     func_ret_asserts = Counter({k: 0 for k in func_defs})
     assert_func_counts = {}
     for stmt in ast.walk(ast.parse(nb_cell_code)):
         if isinstance(stmt, ast.Assign) and isinstance(stmt.value, ast.Call):
             _update_ret_vals(stmt, ret_vals)
 
         if isinstance(stmt, ast.Assert):
@@ -133,46 +135,46 @@
 
     return func_ret_asserts
 
 # %% ../nbs/indicators.ipynb 45
 def _check_for_function_asserts(
     stmt: ast.AST, ret_vals, func_ret_asserts, assert_func_counts
 ):
-    if "left" in stmt.test.__dict__:
-        if "id" in stmt.test.left.__dict__:
+    if hasattr(stmt.test, "left"):
+        if hasattr(stmt.test.left, "id"):
             _incr_assert_count(
                 id(stmt),
                 ret_vals,
                 func_ret_asserts,
                 assert_func_counts,
                 stmt.test.left.id,
             )
         for comp in stmt.test.comparators:
-            if "id" in comp.__dict__:
+            if hasattr(comp, "id"):
                 _incr_assert_count(
                     id(stmt), ret_vals, func_ret_asserts, assert_func_counts, comp.id
                 )
     elif isinstance(stmt.test, ast.Name):
-        if "id" in stmt.test.__dict__:
+        if hasattr(stmt.test, "id"):
             _incr_assert_count(
                 id(stmt), ret_vals, func_ret_asserts, assert_func_counts, stmt.test.id
             )
     elif isinstance(stmt.test, ast.BoolOp):
         for val in stmt.test.values:
-            if "left" in val.__dict__:
-                if "id" in val.left.__dict__:
+            if hasattr(val, "left"):
+                if hasattr(val.left, "id"):
                     _incr_assert_count(
                         id(stmt),
                         ret_vals,
                         func_ret_asserts,
                         assert_func_counts,
                         val.left.id,
                     )
                 for comp in val.comparators:
-                    if "id" in comp.__dict__:
+                    if hasattr(comp, "id"):
                         _incr_assert_count(
                             id(stmt),
                             ret_vals,
                             func_ret_asserts,
                             assert_func_counts,
                             comp.id,
                         )
@@ -187,60 +189,44 @@
     ):
         assert_func_counts[assert_id].append(ret_vals[return_var])
         if return_var in ret_vals:
             func_ret_asserts[ret_vals[return_var]] += 1
 
 # %% ../nbs/indicators.ipynb 47
 def _update_ret_vals(stmt, ret_vals):
-    if type(stmt.value.func) == ast.Subscript:
+    if isinstance(stmt.value.func, ast.Subscript):
         func_name = stmt.func.value.id
+    elif isinstance(stmt.value.func, ast.Attribute):
+        func_name = stmt.value.func.attr
     else:
-        if isinstance(stmt.value.func, ast.Attribute):
-            if (
-                "func" in stmt.value.func.value.__dict__
-                and "id" in stmt.value.func.value.func.__dict__
-            ):
-                func_name = stmt.value.func.value.func.id
-            else:
-                if "attr" in stmt.value.func.__dict__:
-                    func_name = stmt.value.func.attr
-                elif "value" in stmt.value.func.__dict__:
-                    if "id" in stmt.value.func.value.__dict__:
-                        func_name = stmt.value.func.value.id
-                    elif "attr" in stmt.value.func.value.__dict__:
-                        func_name = stmt.value.func.value.attr
-                else:
-                    raise ValueError(f"{stmt.value.func.__dict__}")
-        else:
-            func_name = (
-                stmt.value.func.id
-                if "id" in stmt.value.func.__dict__
-                else stmt.func.attr
-            )
+        func_name = (
+            stmt.value.func.id if hasattr(stmt.value.func, "id") else stmt.func.attr
+        )
+
     if isinstance(stmt.targets[0], ast.Name):
         ret_vals[stmt.targets[0].id] = func_name
     elif isinstance(stmt.targets[0], ast.Tuple):
         for elts in stmt.targets[0].elts:
             ret_vals[elts.id] = func_name
 
 # %% ../nbs/indicators.ipynb 49
 def tests_per_function(nb):
     nb_cell_code = "\n".join(
         [
-            replace_ipython_magics(c["source"])
+            remove_ipython_special_directives(c["source"])
             for c in nb.cells
             if c["cell_type"] == "code"
         ]
     )
     return _tests_per_function_code(nb_cell_code)
 
 
 def _tests_per_function_code(nb_cell_code):
     func_ret_asserts = _count_func_ret_asserts(nb_cell_code)
-    inline_asserts = _count_inline_asserts(nb_cell_code, get_func_defs(nb_cell_code))
+    inline_asserts = _count_inline_asserts(nb_cell_code, _get_func_defs(nb_cell_code))
 
     func_ret_asserts.update(inline_asserts)
     return pd.Series(func_ret_asserts)
 
 # %% ../nbs/indicators.ipynb 52
 def tests_per_func_mean(nb):
     return tests_per_function(nb).mean()
@@ -249,60 +235,60 @@
 def tests_func_coverage_pct(nb):
     return tests_per_function(nb).clip(upper=1).mean() * 100
 
 # %% ../nbs/indicators.ipynb 59
 def calc_ifp(nb_cell_code):
     stmts_in_func = 0
     stmts_outside_func = 0
-    for stmt in ast.walk(ast.parse(replace_ipython_magics(nb_cell_code))):
+    for stmt in ast.walk(ast.parse(remove_ipython_special_directives(nb_cell_code))):
         if isinstance(stmt, ast.FunctionDef) and not stmt.name.startswith("_"):
             for body_item in stmt.body:
                 stmts_in_func += 1
         elif isinstance(stmt, ast.Module):
             for body_item in stmt.body:
                 if not isinstance(body_item, ast.FunctionDef):
                     stmts_outside_func += 1
     return (
         0
         if stmts_outside_func + stmts_in_func == 0
         else (stmts_in_func / (stmts_outside_func + stmts_in_func)) * 100
     )
 
-# %% ../nbs/indicators.ipynb 61
+# %% ../nbs/indicators.ipynb 62
 def in_func_pct(nb):
     nb_cell_code = "\n".join(
         [
-            replace_ipython_magics(c["source"])
+            remove_ipython_special_directives(c["source"])
             for c in nb.cells
             if c["cell_type"] == "code"
         ]
     )
     if nb_cell_code == "":
         return np.nan
     return calc_ifp(nb_cell_code)
 
-# %% ../nbs/indicators.ipynb 64
+# %% ../nbs/indicators.ipynb 66
 def markdown_code_pct(nb):
     md_cells = [c for c in nb.cells if c["cell_type"] == "markdown"]
     code_cells = [c for c in nb.cells if c["cell_type"] == "code"]
     num_code_cells = len(code_cells)
     if num_code_cells == 0:
         return np.nan
     num_md_cells = len(md_cells)
     return (
         100
         if num_code_cells == 0
         else (num_md_cells / (num_md_cells + num_code_cells)) * 100
     )
 
-# %% ../nbs/indicators.ipynb 67
+# %% ../nbs/indicators.ipynb 70
 def total_code_len(nb):
     return sum([len(c["source"]) for c in nb.cells if c["cell_type"] == "code"])
 
-# %% ../nbs/indicators.ipynb 70
+# %% ../nbs/indicators.ipynb 74
 def loc_per_md_section(nb):
     num_md_sections = len(
         [
             c["source"]
             for c in nb.cells
             if c["cell_type"] == "markdown" and c["source"].strip().startswith("#")
         ]
@@ -310,15 +296,15 @@
     tcl = total_code_len(nb)
     if tcl == 0 or num_md_sections == 0:
         result = np.nan
     else:
         result = total_code_len(nb) / num_md_sections
     return result
 
-# %% ../nbs/indicators.ipynb 73
+# %% ../nbs/indicators.ipynb 77
 indicator_funcs = {
     "calls_per_func_mean": calls_per_func_mean,
     "calls_per_func_median": calls_per_func_median,
     "tests_per_func_mean": tests_per_func_mean,
     "tests_func_coverage_pct": tests_func_coverage_pct,
     "in_func_pct": in_func_pct,
     "markdown_code_pct": markdown_code_pct,
```

### Comparing `scilint-0.2.0/scilint/scilint.py` & `scilint-0.2.1/scilint/scilint.py`

 * *Files 4% similar despite different names*

```diff
@@ -204,15 +204,15 @@
 ):
     if nb_paths is None:
         nb_paths = [Path(p).absolute() for p in nbglob(nb_glob)]
     else:
         nb_paths = [Path(p).absolute() for p in nb_paths]
 
     if len(nb_paths) == 0:
-        return None, None, None
+        raise ValueError("Attempt to lint notebooks but no files found")
 
     excluded_paths = None
     exclusions = conf["exclusions"]
     if exclusions is not None:
         excluded_paths = _get_excluded_paths(nb_paths, exclude_pattern=exclusions)
 
     results = []
@@ -236,15 +236,28 @@
 
     scoring_report = lint_report[lint_report.include_in_scoring].copy()
     all_warns, num_warnings = _calculate_warnings(spec_name, scoring_report, conf)
     return lint_report, all_warns, num_warnings
 
 # %% ../nbs/scilint.ipynb 32
 def _map_paths_specs(nb_glob: Path = None, specs_glob: Path = Path(".").resolve()):
-    nbs = nbglob(nb_glob)
+    if is_nbdev_project():
+        nbs = nbglob(nb_glob)
+    else:
+        nb_glob = Path(".") if nb_glob is None else nb_glob
+        nbs = [
+            p.absolute()
+            for p in globtastic(
+                path=Path("."),
+                skip_folder_re="^[_.]",
+                file_glob="*.ipynb",
+                skip_file_re="^[_.]",
+            ).map(Path)
+        ]
+        nbs = [str(p) for p in nbs]
     spec_files = [
         Path(p)
         for p in globtastic(
             specs_glob,
             file_glob="scilint-*.yaml",
             skip_folder_re="ipynb_checkpoints|_proc",
         )
@@ -268,38 +281,38 @@
                 fallback_path = Path("scilint-default")
                 if fallback_path not in spec_nbs:
                     spec_nbs[fallback_path] = []
                 spec_nbs[fallback_path].append(nb)
 
     return spec_nbs
 
-# %% ../nbs/scilint.ipynb 47
+# %% ../nbs/scilint.ipynb 48
 def display_warning_report(all_warns: pd.DataFrame):
     print(
         "\n******************************************Begin Scilint Warning Report*****************************************"
     )
     print(all_warns.to_markdown(tablefmt="grid", index=False))
     print(
         "\n******************************************End Scilint Warning Report*******************************************\n"
     )
 
-# %% ../nbs/scilint.ipynb 49
+# %% ../nbs/scilint.ipynb 50
 def _persist_results(
     lint_report: pd.DataFrame, all_warns: pd.DataFrame, conf: Dict[str, Any]
 ):
     out_dir = Path(conf["out_dir"])
     conf_to_persist = {k: v for k, v in conf.items() if k != "indicators"}
     if not out_dir.exists():
         Path(out_dir).mkdir()
     with open(Path(out_dir, "scilint_config.json"), "w") as outfile:
         json.dump(conf_to_persist, outfile)
     all_warns.to_csv(Path(out_dir, "scilint_warnings.csv"), index=False)
     lint_report.to_csv(Path(out_dir, "scilint_report.csv"))
 
-# %% ../nbs/scilint.ipynb 52
+# %% ../nbs/scilint.ipynb 53
 def _load_conf(
     conf_path: str = None,
     exclusions: str = None,
     fail_over: int = None,
     out_dir: int = None,
     precision: int = None,
     print_syntax_errors: bool = None,
@@ -321,30 +334,36 @@
     )
     overrides = (exclusions, fail_over, out_dir, precision, print_syntax_errors)
     for override in zip(override_names, overrides):
         if override[1] is not None:
             conf[override[0]] = override[1]
     return conf
 
-# %% ../nbs/scilint.ipynb 56
+# %% ../nbs/scilint.ipynb 57
 def lint(
     display_report: bool = True,
     nb_glob: Path = None,
     specs_glob: Path = Path(".").resolve(),
     exclusions: str = None,
     fail_over: int = None,
     out_dir: int = None,
     precision: int = None,
     print_syntax_errors: bool = None,
 ):
     spec_nbs = _map_paths_specs(nb_glob, specs_glob)
     lint_reports = []
     all_warns = []
     warns_count = []
+    linting_failure = False
     for spec, nbs in spec_nbs.items():
+        if len(nbs) == 0:
+            print(
+                f"Linting skipped for: {spec.name} as no notebooks found matching path expression"
+            )
+            continue
         if spec == "scilint-default":
             conf = get_default_spec()
         else:
             conf = _load_conf(
                 spec, exclusions, fail_over, out_dir, precision, print_syntax_errors
             )
         if conf["evaluate"] == False:
@@ -366,33 +385,37 @@
             print(
                 f"Linting success for: {spec.name}, warnings ({num_warnings}) <= than threshold ({fail_over_conf}) "
             )
         else:
             print(
                 f"Linting failed for: {spec.name}, total warnings ({num_warnings}) exceeded threshold ({fail_over_conf})"
             )
-            sys.exit(num_warnings)
+            linting_failure = True
+            continue
 
     lint_report = pd.concat(lint_reports) if len(lint_reports) > 0 else lint_report
     all_warns = pd.concat(all_warns) if len(all_warns) > 0 else report_warns
     num_warnings = sum(warns_count)
 
+    _persist_results(lint_report, all_warns, conf)
+
     if num_warnings > 0:
-        print(
-            f"{num_warnings} warnings founds, within tolerated thresholds for all specs"
-        )
         if display_report:
             display_warning_report(all_warns)
+        if not linting_failure:
+            print(
+                f"{num_warnings} warnings founds, within tolerated thresholds for all specs"
+            )
+        else:
+            sys.exit(num_warnings)
     elif num_warnings == 0:
         print("No issues found during linting")
-
-    _persist_results(lint_report, all_warns, conf)
     print("Linting completed")
 
-# %% ../nbs/scilint.ipynb 59
+# %% ../nbs/scilint.ipynb 60
 def build(
     display_report: bool = True,
     nb_glob: Path = None,
     specs_glob: Path = Path(".").resolve(),
     exclusions: str = None,
     fail_over: int = None,
     out_dir: int = None,
@@ -417,20 +440,20 @@
         precision,
         print_syntax_errors,
     )
     if is_nbdev_project():
         nbdev_clean.__wrapped__()
         print("Cleaned notebooks")
 
-# %% ../nbs/scilint.ipynb 62
+# %% ../nbs/scilint.ipynb 63
 @call_parse
 def scilint_tidy():
     tidy()
 
-# %% ../nbs/scilint.ipynb 64
+# %% ../nbs/scilint.ipynb 65
 @call_parse
 def scilint_lint(
     display_report: Param("Print the lint report", store_false) = False,
     nb_glob: Path = None,
     specs_glob: Path = Path(".").resolve(),
     exclusions: str = None,
     fail_over: int = None,
@@ -445,15 +468,15 @@
         exclusions,
         fail_over,
         out_dir,
         precision,
         print_syntax_errors,
     )
 
-# %% ../nbs/scilint.ipynb 67
+# %% ../nbs/scilint.ipynb 68
 @call_parse
 def scilint_build(
     display_report: Param("Print the lint report", store_false) = False,
     nb_glob: Path = None,
     specs_glob: Path = Path(".").resolve(),
     exclusions: str = None,
     fail_over: int = None,
@@ -468,15 +491,15 @@
         exclusions,
         fail_over,
         out_dir,
         precision,
         print_syntax_errors,
     )
 
-# %% ../nbs/scilint.ipynb 69
+# %% ../nbs/scilint.ipynb 70
 @call_parse
 def scilint_ci(
     display_report: Param("Print the lint report", store_false) = False,
     nb_glob: Path = None,
     specs_glob: Path = Path(".").resolve(),
     exclusions: str = None,
     fail_over: int = None,
```

### Comparing `scilint-0.2.0/scilint/test/test_nbdev.py` & `scilint-0.2.1/scilint/test/test_nbdev.py`

 * *Files identical despite different names*

### Comparing `scilint-0.2.0/scilint/test/test_nbdev_high_quality.py` & `scilint-0.2.1/scilint/test/test_nbdev_high_quality.py`

 * *Files identical despite different names*

### Comparing `scilint-0.2.0/scilint/validated/test_nbdev_high_quality.py` & `scilint-0.2.1/scilint/validated/test_nbdev_high_quality.py`

 * *Files identical despite different names*

### Comparing `scilint-0.2.0/scilint.egg-info/PKG-INFO` & `scilint-0.2.1/scilint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scilint
-Version: 0.2.0
+Version: 0.2.1
 Summary: infuse quality into notebook based workflows with a new type of build tool.
 Home-page: https://github.com/newday-data/scilint/tree/{branch}/
 Author: Donal Simmie
 Author-email: oss@newday.co.uk
 License: Apache Software License 2.0
 Project-URL: Documentation, https://newday-data.github.io/scilint/
 Keywords: research,production,exploration,CI/CD
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scilint Version: 0.2.0 Summary: infuse quality into
+Metadata-Version: 2.1 Name: scilint Version: 0.2.1 Summary: infuse quality into
 notebook based workflows with a new type of build tool. Home-page: https://
 github.com/newday-data/scilint/tree/{branch}/ Author: Donal Simmie Author-
 email: oss@newday.co.uk License: Apache Software License 2.0 Project-URL:
 Documentation, https://newday-data.github.io/scilint/ Keywords:
 research,production,exploration,CI/CD Platform: UNKNOWN Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Programming Language ::
```

### Comparing `scilint-0.2.0/scilint.egg-info/SOURCES.txt` & `scilint-0.2.1/scilint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scilint-0.2.0/setup.py` & `scilint-0.2.1/setup.py`

 * *Files identical despite different names*

