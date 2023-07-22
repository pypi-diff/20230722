# Comparing `tmp/transformers_js_py-0.1.1.tar.gz` & `tmp/transformers_js_py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers_js_py-0.1.1.tar", max compression
+gzip compressed data, was "transformers_js_py-0.1.2.tar", max compression
```

## Comparing `transformers_js_py-0.1.1.tar` & `transformers_js_py-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-07-18 07:47:21.359134 transformers_js_py-0.1.1/LICENSE
--rw-r--r--   0        0        0       21 2023-07-18 07:57:53.172125 transformers_js_py-0.1.1/README.md
--rw-r--r--   0        0        0      579 2023-07-22 03:05:38.779906 transformers_js_py-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2389 2023-07-22 02:36:22.861114 transformers_js_py-0.1.1/transformers_js/__init__.py
--rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 transformers_js_py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-22 03:11:41.822904 transformers_js_py-0.1.2/LICENSE
+-rw-r--r--   0        0        0       21 2023-07-22 03:11:41.822904 transformers_js_py-0.1.2/README.md
+-rw-r--r--   0        0        0      579 2023-07-22 03:11:41.826904 transformers_js_py-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2389 2023-07-22 03:11:41.826904 transformers_js_py-0.1.2/transformers_js/__init__.py
+-rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 transformers_js_py-0.1.2/PKG-INFO
```

### Comparing `transformers_js_py-0.1.1/LICENSE` & `transformers_js_py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `transformers_js_py-0.1.1/pyproject.toml` & `transformers_js_py-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "transformers-js-py"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Yuichiro Tachibana (Tsuchiya) <t.yic.yt@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "transformers_js"}]
 
 [tool.poetry.dependencies]
```

### Comparing `transformers_js_py-0.1.1/transformers_js/__init__.py` & `transformers_js_py-0.1.2/transformers_js/__init__.py`

 * *Files identical despite different names*

