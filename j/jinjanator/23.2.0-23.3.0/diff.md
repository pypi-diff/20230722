# Comparing `tmp/jinjanator-23.2.0.tar.gz` & `tmp/jinjanator-23.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Jul 22 21:18:09 2023, max compression
+gzip compressed data, last modified: Sat Jul 22 21:49:54 2023, max compression
```

## Comparing `jinjanator-23.2.0.tar` & `jinjanator-23.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1261 2023-07-22 21:18:09.000000 jinjanator-23.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     5925 2023-07-22 21:18:09.000000 jinjanator-23.2.0/PLUGINS.md
--rw-r--r--   0        0        0     8755 2023-07-22 21:18:09.000000 jinjanator-23.2.0/README.md
--rw-r--r--   0        0        0     1120 2023-07-22 21:18:09.000000 jinjanator-23.2.0/plugin_example/jinjanator_plugin_example.py
--rw-r--r--   0        0        0      591 2023-07-22 21:18:09.000000 jinjanator-23.2.0/plugin_example/pyproject.toml
--rw-r--r--   0        0        0     1747 2023-07-22 21:18:09.000000 jinjanator-23.2.0/plugin_example/tests/test_plugin.py
--rw-r--r--   0        0        0       81 2023-07-22 21:18:09.000000 jinjanator-23.2.0/src/jinjanator/__init__.py
--rw-r--r--   0        0        0     9507 2023-07-22 21:18:09.000000 jinjanator-23.2.0/src/jinjanator/cli.py
--rw-r--r--   0        0        0      716 2023-07-22 21:18:09.000000 jinjanator-23.2.0/src/jinjanator/context.py
--rw-r--r--   0        0        0     1154 2023-07-22 21:18:09.000000 jinjanator-23.2.0/src/jinjanator/filters.py
--rw-r--r--   0        0        0     3509 2023-07-22 21:18:09.000000 jinjanator-23.2.0/src/jinjanator/formats.py
--rw-r--r--   0        0        0     2456 2023-07-22 21:18:09.000000 jinjanator-23.2.0/src/jinjanator/plugin.py
--rw-r--r--   0        0        0        0 2023-07-22 21:18:09.000000 jinjanator-23.2.0/src/jinjanator/py.typed
--rw-r--r--   0        0        0      162 2023-07-22 21:18:09.000000 jinjanator-23.2.0/src/jinjanator/version.py
--rw-r--r--   0        0        0     1614 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/__init__.py
--rw-r--r--   0        0        0      675 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/conftest.py
--rw-r--r--   0        0        0     1580 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_argparse.py
--rw-r--r--   0        0        0     1284 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_cli.py
--rw-r--r--   0        0        0     2723 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_env.py
--rw-r--r--   0        0        0      248 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_extension.py
--rw-r--r--   0        0        0      840 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_invalid_data.py
--rw-r--r--   0        0        0     3749 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_nginx_config.py
--rw-r--r--   0        0        0      780 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_output_file.py
--rw-r--r--   0        0        0      435 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_template_not_found.py
--rw-r--r--   0        0        0      501 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_undefined.py
--rw-r--r--   0        0        0      731 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_unicode.py
--rw-r--r--   0        0        0       58 2023-07-22 21:18:09.000000 jinjanator-23.2.0/.gitignore
--rw-r--r--   0        0        0    35149 2023-07-22 21:18:09.000000 jinjanator-23.2.0/LICENSE.apache-2.0
--rw-r--r--   0        0        0     1321 2023-07-22 21:18:09.000000 jinjanator-23.2.0/LICENSE.bsd-2-clause
--rw-r--r--   0        0        0     6950 2023-07-22 21:18:09.000000 jinjanator-23.2.0/pyproject.toml
--rw-r--r--   0        0        0     7647 2023-07-22 21:18:09.000000 jinjanator-23.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1600 2023-07-22 21:49:54.000000 jinjanator-23.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5925 2023-07-22 21:49:54.000000 jinjanator-23.3.0/PLUGINS.md
+-rw-r--r--   0        0        0     8755 2023-07-22 21:49:54.000000 jinjanator-23.3.0/README.md
+-rw-r--r--   0        0        0     1120 2023-07-22 21:49:54.000000 jinjanator-23.3.0/plugin_example/jinjanator_plugin_example.py
+-rw-r--r--   0        0        0      591 2023-07-22 21:49:54.000000 jinjanator-23.3.0/plugin_example/pyproject.toml
+-rw-r--r--   0        0        0     1747 2023-07-22 21:49:54.000000 jinjanator-23.3.0/plugin_example/tests/test_plugin.py
+-rw-r--r--   0        0        0       81 2023-07-22 21:49:54.000000 jinjanator-23.3.0/src/jinjanator/__init__.py
+-rw-r--r--   0        0        0     9522 2023-07-22 21:49:54.000000 jinjanator-23.3.0/src/jinjanator/cli.py
+-rw-r--r--   0        0        0      716 2023-07-22 21:49:54.000000 jinjanator-23.3.0/src/jinjanator/context.py
+-rw-r--r--   0        0        0     1154 2023-07-22 21:49:54.000000 jinjanator-23.3.0/src/jinjanator/filters.py
+-rw-r--r--   0        0        0     3509 2023-07-22 21:49:54.000000 jinjanator-23.3.0/src/jinjanator/formats.py
+-rw-r--r--   0        0        0     2456 2023-07-22 21:49:54.000000 jinjanator-23.3.0/src/jinjanator/plugin.py
+-rw-r--r--   0        0        0        0 2023-07-22 21:49:54.000000 jinjanator-23.3.0/src/jinjanator/py.typed
+-rw-r--r--   0        0        0      162 2023-07-22 21:49:54.000000 jinjanator-23.3.0/src/jinjanator/version.py
+-rw-r--r--   0        0        0     1614 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      675 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     1580 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_argparse.py
+-rw-r--r--   0        0        0     1284 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_cli.py
+-rw-r--r--   0        0        0     2723 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_env.py
+-rw-r--r--   0        0        0      248 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_extension.py
+-rw-r--r--   0        0        0      840 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_invalid_data.py
+-rw-r--r--   0        0        0     3749 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_nginx_config.py
+-rw-r--r--   0        0        0      780 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_output_file.py
+-rw-r--r--   0        0        0      435 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_template_not_found.py
+-rw-r--r--   0        0        0      501 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_undefined.py
+-rw-r--r--   0        0        0      731 2023-07-22 21:49:54.000000 jinjanator-23.3.0/tests/test_unicode.py
+-rw-r--r--   0        0        0       58 2023-07-22 21:49:54.000000 jinjanator-23.3.0/.gitignore
+-rw-r--r--   0        0        0    35149 2023-07-22 21:49:54.000000 jinjanator-23.3.0/LICENSE.apache-2.0
+-rw-r--r--   0        0        0     1321 2023-07-22 21:49:54.000000 jinjanator-23.3.0/LICENSE.bsd-2-clause
+-rw-r--r--   0        0        0     6908 2023-07-22 21:49:54.000000 jinjanator-23.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7820 2023-07-22 21:49:54.000000 jinjanator-23.3.0/PKG-INFO
```

### Comparing `jinjanator-23.2.0/CHANGELOG.md` & `jinjanator-23.3.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,24 @@
 This changelog is managed by towncrier and is compiled at release time.
 
 See https://github.com/kpfleming/jinjanator/blob/main/.github/CONTRIBUTING.md#changelog for details.
 -->
 
 <!-- towncrier release notes start -->
 
+## [23.3.0](https://github.com/kpfleming/jinjanator/tree/23.3.0) - 2023-07-22
+
+### Fixes
+
+- Disabled Jinja2 'autoescape' feature since it can produce incorrect output.
+  [#8](https://github.com/kpfleming/jinjanator/issues/8)
+- Add missing 'attrs' package to project dependencies.
+  [#9](https://github.com/kpfleming/jinjanator/issues/9)
+
+
 ## [23.2.0](https://github.com/kpfleming/jinjanator/tree/23.2.0) - 2023-07-22
 
 ### Fixes
 
 - Resolved crash when writing final output. Increased test coverage to avoid regressions.
   [#7](https://github.com/kpfleming/jinjanator/issues/7)
```

### Comparing `jinjanator-23.2.0/PLUGINS.md` & `jinjanator-23.3.0/PLUGINS.md`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/README.md` & `jinjanator-23.3.0/README.md`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/plugin_example/jinjanator_plugin_example.py` & `jinjanator-23.3.0/plugin_example/jinjanator_plugin_example.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/plugin_example/pyproject.toml` & `jinjanator-23.3.0/plugin_example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/plugin_example/tests/test_plugin.py` & `jinjanator-23.3.0/plugin_example/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/src/jinjanator/cli.py` & `jinjanator-23.3.0/src/jinjanator/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         j2_env_params.setdefault(
             "undefined",
             jinja2.Undefined if allow_undefined else jinja2.StrictUndefined,
         )
         j2_env_params.setdefault("extensions", self.ENABLED_EXTENSIONS)
         j2_env_params.setdefault("loader", FilePathLoader(cwd))
 
-        self._env = jinja2.Environment(**j2_env_params, autoescape=True)
+        self._env = jinja2.Environment(**j2_env_params, autoescape=False)  # noqa: S701
 
         for plugin_globals in plugin_hook_callers.plugin_globals():
             self._env.globals.update(plugin_globals)
 
         for plugin_filters in plugin_hook_callers.plugin_filters():
             self._env.filters.update(plugin_filters)
```

### Comparing `jinjanator-23.2.0/src/jinjanator/context.py` & `jinjanator-23.3.0/src/jinjanator/context.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/src/jinjanator/filters.py` & `jinjanator-23.3.0/src/jinjanator/filters.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/src/jinjanator/formats.py` & `jinjanator-23.3.0/src/jinjanator/formats.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/src/jinjanator/plugin.py` & `jinjanator-23.3.0/src/jinjanator/plugin.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/tests/__init__.py` & `jinjanator-23.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/tests/conftest.py` & `jinjanator-23.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/tests/test_argparse.py` & `jinjanator-23.3.0/tests/test_argparse.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/tests/test_cli.py` & `jinjanator-23.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/tests/test_env.py` & `jinjanator-23.3.0/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/tests/test_invalid_data.py` & `jinjanator-23.3.0/tests/test_invalid_data.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/tests/test_nginx_config.py` & `jinjanator-23.3.0/tests/test_nginx_config.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/tests/test_output_file.py` & `jinjanator-23.3.0/tests/test_output_file.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/tests/test_unicode.py` & `jinjanator-23.3.0/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/LICENSE.apache-2.0` & `jinjanator-23.3.0/LICENSE.apache-2.0`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/LICENSE.bsd-2-clause` & `jinjanator-23.3.0/LICENSE.bsd-2-clause`

 * *Files identical despite different names*

### Comparing `jinjanator-23.2.0/pyproject.toml` & `jinjanator-23.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
   "Typing :: Typed",
 ]
 dynamic = [
   "readme",
   "version",
 ]
 dependencies = [
+  "attrs",
   "jinja2>=2.7.2",
   "pluggy",
   "PyYAML",
   "typing-extensions",
 ]
 [project.urls]
 "Bug Tracker" = "https://github.com/kpfleming/jinjanator/issues"
@@ -49,19 +50,19 @@
 skip-install = true
 dependencies = [
   "towncrier",
 ]
 
 [tool.hatch.envs.changelog.scripts]
 draft = [
-  "rm changelog.d/*~",
+  "rm -f changelog.d/*~",
   "towncrier build --version main --draft",
 ]
 release = [
-  "rm changelog.d/*~",
+  "rm -f changelog.d/*~",
   "towncrier build --version {args}",
 ]
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
@@ -90,15 +91,14 @@
 ]
 
 [tool.hatch.envs.default]
 python = "3.11"
 
 [tool.hatch.envs.lint]
 dependencies = [
-    "attrs", # needed for type-checking tests
     "black",
     "ruff",
     "mypy",
     "pytest", # needed for type-checking tests
     "types-PyYAML",
 ]
 
@@ -118,15 +118,14 @@
      "mypy tests",
      "mypy plugin_example/*.py",
      "shellcheck workflow-support/*.sh",
 ]
 
 [tool.hatch.envs.ci]
 dependencies = [
-    "attrs",
     "coverage[toml]",
     "pytest",
     "pytest-cov",
     "pytest-icdiff",
     "PyYAML",
 ]
```

### Comparing `jinjanator-23.2.0/PKG-INFO` & `jinjanator-23.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjanator
-Version: 23.2.0
+Version: 23.3.0
 Summary: Command-line interface to Jinja2 for templating in shell scripts.
 Project-URL: Bug Tracker, https://github.com/kpfleming/jinjanator/issues
 Project-URL: Homepage, https://github.com/kpfleming/jinjanator
 Author-email: "Kevin P. Fleming" <jinjanator@kevin.km6g.us>, Mark Vartanyan <kolypto@gmail.com>
 License: Apache-2.0
 License-File: LICENSE.apache-2.0
 License-File: LICENSE.bsd-2-clause
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
+Requires-Dist: attrs
 Requires-Dist: jinja2>=2.7.2
 Requires-Dist: pluggy
 Requires-Dist: pyyaml
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # *jinjanator*: CLI tool for rendering Jinja2 templates
@@ -312,13 +313,15 @@
 
 Notice that there must be quotes around the environment variable name
 when it is a literal string.
 
 ## Release Information
 ### Fixes
 
-- Resolved crash when writing final output. Increased test coverage to avoid regressions.
-  [[#7](https://github.com/kpfleming/jinjanator/issues/7)](https://github.com/kpfleming/jinjanator/issues/7)
+- Disabled Jinja2 'autoescape' feature since it can produce incorrect output.
+  [[#8](https://github.com/kpfleming/jinjanator/issues/8)](https://github.com/kpfleming/jinjanator/issues/8)
+- Add missing 'attrs' package to project dependencies.
+  [[#9](https://github.com/kpfleming/jinjanator/issues/9)](https://github.com/kpfleming/jinjanator/issues/9)
 
 
 ---
 [→ Full Changelog](https://github.com/kpfleming/jinjanator/blob/main/CHANGELOG.md)
```

