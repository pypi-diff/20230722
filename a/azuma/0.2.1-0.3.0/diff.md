# Comparing `tmp/azuma-0.2.1.tar.gz` & `tmp/azuma-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azuma-0.2.1.tar", max compression
+gzip compressed data, was "azuma-0.3.0.tar", max compression
```

## Comparing `azuma-0.2.1.tar` & `azuma-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1070 2023-07-07 23:02:32.195212 azuma-0.2.1/LICENSE
--rw-r--r--   0        0        0      560 2023-07-07 23:02:32.195212 azuma-0.2.1/README.md
--rw-r--r--   0        0        0      128 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/__init__.py
--rw-r--r--   0        0        0     1483 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/cli.py
--rw-r--r--   0        0        0      212 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/exceptions.py
--rw-r--r--   0        0        0      952 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/grammar.lark
--rw-r--r--   0        0        0     5226 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/matchers.py
--rw-r--r--   0        0        0      129 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/parsers/__init__.py
--rw-r--r--   0        0        0     3452 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/parsers/condition.py
--rw-r--r--   0        0        0     5451 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/parsers/detection.py
--rw-r--r--   0        0        0      144 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/schemas/__init__.py
--rw-r--r--   0        0        0     1882 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/schemas/detection.py
--rw-r--r--   0        0        0      256 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/schemas/log_source.py
--rw-r--r--   0        0        0      206 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/schemas/related.py
--rw-r--r--   0        0        0     3937 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/schemas/rule.py
--rw-r--r--   0        0        0     1098 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/schemas/rule_set.py
--rw-r--r--   0        0        0     1249 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/schemas/yaml_model.py
--rw-r--r--   0        0        0      318 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/types.py
--rw-r--r--   0        0        0      638 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/utils.py
--rw-r--r--   0        0        0      182 2023-07-07 23:02:32.195212 azuma-0.2.1/azuma/validators.py
--rw-r--r--   0        0        0     1351 2023-07-07 23:02:52.367235 azuma-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 azuma-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-22 00:07:35.509229 azuma-0.3.0/LICENSE
+-rw-r--r--   0        0        0      560 2023-07-22 00:07:35.509229 azuma-0.3.0/README.md
+-rw-r--r--   0        0        0      128 2023-07-22 00:07:35.509229 azuma-0.3.0/azuma/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-22 00:07:35.509229 azuma-0.3.0/azuma/cli.py
+-rw-r--r--   0        0        0      212 2023-07-22 00:07:35.509229 azuma-0.3.0/azuma/exceptions.py
+-rw-r--r--   0        0        0      952 2023-07-22 00:07:35.509229 azuma-0.3.0/azuma/grammar.lark
+-rw-r--r--   0        0        0     5226 2023-07-22 00:07:35.509229 azuma-0.3.0/azuma/matchers.py
+-rw-r--r--   0        0        0      129 2023-07-22 00:07:35.509229 azuma-0.3.0/azuma/parsers/__init__.py
+-rw-r--r--   0        0        0     3440 2023-07-22 00:07:35.509229 azuma-0.3.0/azuma/parsers/condition.py
+-rw-r--r--   0        0        0     5451 2023-07-22 00:07:35.509229 azuma-0.3.0/azuma/parsers/detection.py
+-rw-r--r--   0        0        0      144 2023-07-22 00:07:35.509229 azuma-0.3.0/azuma/schemas/__init__.py
+-rw-r--r--   0        0        0     1882 2023-07-22 00:07:35.509229 azuma-0.3.0/azuma/schemas/detection.py
+-rw-r--r--   0        0        0      256 2023-07-22 00:07:35.509229 azuma-0.3.0/azuma/schemas/log_source.py
+-rw-r--r--   0        0        0      206 2023-07-22 00:07:35.509229 azuma-0.3.0/azuma/schemas/related.py
+-rw-r--r--   0        0        0     3937 2023-07-22 00:07:35.509229 azuma-0.3.0/azuma/schemas/rule.py
+-rw-r--r--   0        0        0     1098 2023-07-22 00:07:35.509229 azuma-0.3.0/azuma/schemas/rule_set.py
+-rw-r--r--   0        0        0     1249 2023-07-22 00:07:35.509229 azuma-0.3.0/azuma/schemas/yaml_model.py
+-rw-r--r--   0        0        0      318 2023-07-22 00:07:35.509229 azuma-0.3.0/azuma/types.py
+-rw-r--r--   0        0        0      638 2023-07-22 00:07:35.509229 azuma-0.3.0/azuma/utils.py
+-rw-r--r--   0        0        0      182 2023-07-22 00:07:35.509229 azuma-0.3.0/azuma/validators.py
+-rw-r--r--   0        0        0     1376 2023-07-22 00:07:52.089803 azuma-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1321 1970-01-01 00:00:00.000000 azuma-0.3.0/PKG-INFO
```

### Comparing `azuma-0.2.1/LICENSE` & `azuma-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `azuma-0.2.1/README.md` & `azuma-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `azuma-0.2.1/azuma/cli.py` & `azuma-0.3.0/azuma/cli.py`

 * *Files identical despite different names*

### Comparing `azuma-0.2.1/azuma/grammar.lark` & `azuma-0.3.0/azuma/grammar.lark`

 * *Files identical despite different names*

### Comparing `azuma-0.2.1/azuma/matchers.py` & `azuma-0.3.0/azuma/matchers.py`

 * *Files identical despite different names*

### Comparing `azuma-0.2.1/azuma/parsers/condition.py` & `azuma-0.3.0/azuma/parsers/condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     @staticmethod
     def near_aggregation(args):
         raise UnsupportedFeature("Near operation not supported.")
 
 
 # Create & initialize Lark class instance
 factory_parser = Lark(
-    grammar, parser="lalr", transformer=FactoryTransformer(), maybe_placeholders=True
+    grammar, parser="lalr", transformer=FactoryTransformer(), strict=True
 )
 
 
 def prepare_condition(raw_condition: str | list) -> Tree:
     if isinstance(raw_condition, list):
         raw_condition = "(" + ") or (".join(raw_condition) + ")"
```

### Comparing `azuma-0.2.1/azuma/parsers/detection.py` & `azuma-0.3.0/azuma/parsers/detection.py`

 * *Files identical despite different names*

### Comparing `azuma-0.2.1/azuma/schemas/detection.py` & `azuma-0.3.0/azuma/schemas/detection.py`

 * *Files identical despite different names*

### Comparing `azuma-0.2.1/azuma/schemas/rule.py` & `azuma-0.3.0/azuma/schemas/rule.py`

 * *Files identical despite different names*

### Comparing `azuma-0.2.1/azuma/schemas/rule_set.py` & `azuma-0.3.0/azuma/schemas/rule_set.py`

 * *Files identical despite different names*

### Comparing `azuma-0.2.1/azuma/schemas/yaml_model.py` & `azuma-0.3.0/azuma/schemas/yaml_model.py`

 * *Files identical despite different names*

### Comparing `azuma-0.2.1/azuma/utils.py` & `azuma-0.3.0/azuma/utils.py`

 * *Files identical despite different names*

### Comparing `azuma-0.2.1/pyproject.toml` & `azuma-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 [tool.poetry]
 name = "azuma"
-version = "0.2.1"
+version = "0.3.0"
 description = "Yet another Sigma library for Python"
 authors = ["Manabu Niseki <manabu.niseki@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ninoseki/azuma"
 repository = "https://github.com/ninoseki/azuma"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-lark-parser = ">=0.12,<1.0"
+lark = { extras = ["interegular"], version = ">=1.1,<2.0" }
 loguru = ">=0.7,<1.0"
 pydantic = ">=2.0,<3.0"
 pyyaml = ">=6.0,<7.0"
-regex = ">=2022"
+regex = ">=2023"
 typer = ">=0.9,<1.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.3"
-ci-py = "^1.0.0"
+black = "^23.7"
+ci-py = "^1.0"
 gitpython = "^3.1"
 mypy = "^1.4"
 pre-commit = "^3.3"
 pytest = "^7.4"
 pytest-pretty = "^1.2"
-pytest-randomly = "^3.12"
-pyupgrade = "^3.7"
+pytest-randomly = "^3.13"
+pyupgrade = "^3.9"
 ruff = "^0.0"
 types-pyyaml = "^6.0"
 urllib3 = "^1.0"
 
 [tool.poetry.group.doc.dependencies]
 mkdocs = "^1.4"
 mkdocs-material = "^9.1"
-mkdocstrings = {extras = ["python"], version = "^0.22"}
+mkdocstrings = { extras = ["python"], version = "^0.22" }
 
 [tool.poetry.scripts]
 azuma = "azuma.cli:app"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.ruff]
 select = [
-    "E",    # pycodestyle errors
-    "W",    # pycodestyle warnings
-    "F",    # pyflakes
-    "C",    # flake8-comprehensions
-    "B",    # flake8-bugbear
-    "T20",  # flake8-print
+    "E",   # pycodestyle errors
+    "W",   # pycodestyle warnings
+    "F",   # pyflakes
+    "C",   # flake8-comprehensions
+    "B",   # flake8-bugbear
+    "T20", # flake8-print
 ]
 ignore = [
-    "E501",  # line too long, handled by black
+    "E501", # line too long, handled by black
 ]
```

### Comparing `azuma-0.2.1/PKG-INFO` & `azuma-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: azuma
-Version: 0.2.1
+Version: 0.3.0
 Summary: Yet another Sigma library for Python
 Home-page: https://github.com/ninoseki/azuma
 License: MIT
 Author: Manabu Niseki
 Author-email: manabu.niseki@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: lark-parser (>=0.12,<1.0)
+Requires-Dist: lark[interegular] (>=1.1,<2.0)
 Requires-Dist: loguru (>=0.7,<1.0)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: regex (>=2022)
+Requires-Dist: regex (>=2023)
 Requires-Dist: typer (>=0.9,<1.0)
 Project-URL: Repository, https://github.com/ninoseki/azuma
 Description-Content-Type: text/markdown
 
 # azuma
 
 [![PyPI version](https://badge.fury.io/py/azuma.svg)](https://badge.fury.io/py/azuma)
```

