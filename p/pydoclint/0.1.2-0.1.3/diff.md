# Comparing `tmp/pydoclint-0.1.2.tar.gz` & `tmp/pydoclint-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoclint-0.1.2.tar", last modified: Fri Jul 21 02:42:21 2023, max compression
+gzip compressed data, was "pydoclint-0.1.3.tar", last modified: Fri Jul 21 22:08:33 2023, max compression
```

## Comparing `pydoclint-0.1.2.tar` & `pydoclint-0.1.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:42:21.789863 pydoclint-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-21 02:42:09.000000 pydoclint-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14506 2023-07-21 02:42:21.789863 pydoclint-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14059 2023-07-21 02:42:09.000000 pydoclint-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:42:21.781863 pydoclint-0.1.2/pydoclint/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/flake8_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/parse_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:42:21.789863 pydoclint-0.1.2/pydoclint/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/astTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/internal_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/method_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/return_anno.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/return_arg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/return_yield_raise.py
--rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/unparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/violation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/utils/walk.py
--rw-r--r--   0 runner    (1001) docker     (123)    24031 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pydoclint/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:42:21.785863 pydoclint-0.1.2/pydoclint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14506 2023-07-21 02:42:21.000000 pydoclint-0.1.2/pydoclint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-21 02:42:21.000000 pydoclint-0.1.2/pydoclint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 02:42:21.000000 pydoclint-0.1.2/pydoclint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-21 02:42:21.000000 pydoclint-0.1.2/pydoclint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-21 02:42:21.000000 pydoclint-0.1.2/pydoclint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 02:42:21.000000 pydoclint-0.1.2/pydoclint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-21 02:42:09.000000 pydoclint-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-21 02:42:21.789863 pydoclint-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-21 02:42:09.000000 pydoclint-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 02:42:21.789863 pydoclint-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-21 02:42:09.000000 pydoclint-0.1.2/tests/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    40645 2023-07-21 02:42:09.000000 pydoclint-0.1.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-21 02:42:09.000000 pydoclint-0.1.2/tests/test_parse_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:08:33.794436 pydoclint-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-21 22:08:21.000000 pydoclint-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14506 2023-07-21 22:08:33.794436 pydoclint-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14059 2023-07-21 22:08:21.000000 pydoclint-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:08:33.790436 pydoclint-0.1.3/pydoclint/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/flake8_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/parse_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:08:33.794436 pydoclint-0.1.3/pydoclint/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/astTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/internal_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/method_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/return_anno.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/return_arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/return_yield_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/unparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/violation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/utils/walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24031 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pydoclint/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:08:33.794436 pydoclint-0.1.3/pydoclint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14506 2023-07-21 22:08:33.000000 pydoclint-0.1.3/pydoclint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-21 22:08:33.000000 pydoclint-0.1.3/pydoclint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:08:33.000000 pydoclint-0.1.3/pydoclint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-21 22:08:33.000000 pydoclint-0.1.3/pydoclint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-21 22:08:33.000000 pydoclint-0.1.3/pydoclint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 22:08:33.000000 pydoclint-0.1.3/pydoclint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-21 22:08:21.000000 pydoclint-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-21 22:08:33.794436 pydoclint-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-21 22:08:21.000000 pydoclint-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:08:33.794436 pydoclint-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-21 22:08:21.000000 pydoclint-0.1.3/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40645 2023-07-21 22:08:21.000000 pydoclint-0.1.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-21 22:08:21.000000 pydoclint-0.1.3/tests/test_parse_config.py
```

### Comparing `pydoclint-0.1.2/LICENSE` & `pydoclint-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.2/PKG-INFO` & `pydoclint-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python docstring linter that checks arguments, returns, yields, and raises sections
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
```

### Comparing `pydoclint-0.1.2/README.md` & `pydoclint-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.2/pydoclint/flake8_entry.py` & `pydoclint-0.1.3/pydoclint/flake8_entry.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,14 +125,15 @@
             options.skip_checking_short_docstrings
         )
         cls.skip_checking_raises = options.skip_checking_raises
         cls.allow_init_docstring = options.allow_init_docstring
         cls.require_return_section_when_returning_none = (
             options.require_return_section_when_returning_none
         )
+        cls.check_return_types = options.check_return_types
         cls.style = options.style
 
     def run(self) -> Generator[Tuple[int, int, str, Any], None, None]:
         """Run the linter and yield the violation information"""
         if self.type_hints_in_docstring != 'None':  # user supplies this option
             raise ValueError(
                 'The option `--type-hints-in-docstring` has been renamed;'
@@ -166,28 +167,33 @@
             '--allow-init-docstring',
             self.allow_init_docstring,
         )
         requireReturnSectionWhenReturningNone = self._bool(
             '--require-return-section-when-returning-none',
             self.require_return_section_when_returning_none,
         )
+        checkReturnTypes = self._bool(
+            '--check-return-types',
+            self.check_return_types,
+        )
 
         if self.style not in {'numpy', 'google', 'sphinx'}:
             raise ValueError(
                 'Invalid value for "--style": must be "numpy", "google", or "sphinx"'
             )
 
         v = Visitor(
             argTypeHintsInSignature=argTypeHintsInSignature,
             argTypeHintsInDocstring=argTypeHintsInDocstring,
             checkArgOrder=checkArgOrder,
             skipCheckingShortDocstrings=skipCheckingShortDocstrings,
             skipCheckingRaises=skipCheckingRaises,
             allowInitDocstring=allowInitDocstring,
             requireReturnSectionWhenReturningNone=requireReturnSectionWhenReturningNone,
+            checkReturnTypes=checkReturnTypes,
             style=self.style,
         )
         v.visit(self._tree)
         violationInfo = [_.getInfoForFlake8() for _ in v.violations]
         for line, colOffset, msg in violationInfo:
             yield line, colOffset, msg, type(self)
```

### Comparing `pydoclint-0.1.2/pydoclint/main.py` & `pydoclint-0.1.3/pydoclint/main.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.2/pydoclint/parse_config.py` & `pydoclint-0.1.3/pydoclint/parse_config.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.2/pydoclint/utils/annotation.py` & `pydoclint-0.1.3/pydoclint/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.2/pydoclint/utils/arg.py` & `pydoclint-0.1.3/pydoclint/utils/arg.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.2/pydoclint/utils/astTypes.py` & `pydoclint-0.1.3/pydoclint/utils/astTypes.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.2/pydoclint/utils/doc.py` & `pydoclint-0.1.3/pydoclint/utils/doc.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.2/pydoclint/utils/generic.py` & `pydoclint-0.1.3/pydoclint/utils/generic.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.2/pydoclint/utils/return_anno.py` & `pydoclint-0.1.3/pydoclint/utils/return_anno.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.2/pydoclint/utils/return_yield_raise.py` & `pydoclint-0.1.3/pydoclint/utils/return_yield_raise.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.2/pydoclint/utils/unparser.py` & `pydoclint-0.1.3/pydoclint/utils/unparser.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.2/pydoclint/utils/violation.py` & `pydoclint-0.1.3/pydoclint/utils/violation.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.2/pydoclint/utils/walk.py` & `pydoclint-0.1.3/pydoclint/utils/walk.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.2/pydoclint/visitor.py` & `pydoclint-0.1.3/pydoclint/visitor.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.2/pydoclint.egg-info/PKG-INFO` & `pydoclint-0.1.3/pydoclint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python docstring linter that checks arguments, returns, yields, and raises sections
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
```

### Comparing `pydoclint-0.1.2/pydoclint.egg-info/SOURCES.txt` & `pydoclint-0.1.3/pydoclint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.2/setup.cfg` & `pydoclint-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydoclint
-version = 0.1.2
+version = 0.1.3
 description = A Python docstring linter that checks arguments, returns, yields, and raises sections
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jsh9/pydoclint
 license = MIT
 license_file = LICENSE
 classifiers =
```

### Comparing `pydoclint-0.1.2/tests/test_generic.py` & `pydoclint-0.1.3/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.2/tests/test_main.py` & `pydoclint-0.1.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.2/tests/test_parse_config.py` & `pydoclint-0.1.3/tests/test_parse_config.py`

 * *Files identical despite different names*

