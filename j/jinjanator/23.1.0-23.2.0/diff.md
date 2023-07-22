# Comparing `tmp/jinjanator-23.1.0.tar.gz` & `tmp/jinjanator-23.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Jul 22 18:34:47 2023, max compression
+gzip compressed data, last modified: Sat Jul 22 21:18:09 2023, max compression
```

## Comparing `jinjanator-23.1.0.tar` & `jinjanator-23.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1022 2023-07-22 18:34:47.000000 jinjanator-23.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     5925 2023-07-22 18:34:47.000000 jinjanator-23.1.0/PLUGINS.md
--rw-r--r--   0        0        0     8755 2023-07-22 18:34:47.000000 jinjanator-23.1.0/README.md
--rw-r--r--   0        0        0     1120 2023-07-22 18:34:47.000000 jinjanator-23.1.0/plugin_example/jinjanator_plugin_example.py
--rw-r--r--   0        0        0      591 2023-07-22 18:34:47.000000 jinjanator-23.1.0/plugin_example/pyproject.toml
--rw-r--r--   0        0        0     1747 2023-07-22 18:34:47.000000 jinjanator-23.1.0/plugin_example/tests/test_plugin.py
--rw-r--r--   0        0        0       81 2023-07-22 18:34:47.000000 jinjanator-23.1.0/src/jinjanator/__init__.py
--rw-r--r--   0        0        0     9522 2023-07-22 18:34:47.000000 jinjanator-23.1.0/src/jinjanator/cli.py
--rw-r--r--   0        0        0      716 2023-07-22 18:34:47.000000 jinjanator-23.1.0/src/jinjanator/context.py
--rw-r--r--   0        0        0     1154 2023-07-22 18:34:47.000000 jinjanator-23.1.0/src/jinjanator/filters.py
--rw-r--r--   0        0        0     3509 2023-07-22 18:34:47.000000 jinjanator-23.1.0/src/jinjanator/formats.py
--rw-r--r--   0        0        0     2456 2023-07-22 18:34:47.000000 jinjanator-23.1.0/src/jinjanator/plugin.py
--rw-r--r--   0        0        0        0 2023-07-22 18:34:47.000000 jinjanator-23.1.0/src/jinjanator/py.typed
--rw-r--r--   0        0        0      162 2023-07-22 18:34:47.000000 jinjanator-23.1.0/src/jinjanator/version.py
--rw-r--r--   0        0        0     1614 2023-07-22 18:34:47.000000 jinjanator-23.1.0/tests/__init__.py
--rw-r--r--   0        0        0      675 2023-07-22 18:34:47.000000 jinjanator-23.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1580 2023-07-22 18:34:47.000000 jinjanator-23.1.0/tests/test_argparse.py
--rw-r--r--   0        0        0      661 2023-07-22 18:34:47.000000 jinjanator-23.1.0/tests/test_cli.py
--rw-r--r--   0        0        0     2723 2023-07-22 18:34:47.000000 jinjanator-23.1.0/tests/test_env.py
--rw-r--r--   0        0        0      248 2023-07-22 18:34:47.000000 jinjanator-23.1.0/tests/test_extension.py
--rw-r--r--   0        0        0      840 2023-07-22 18:34:47.000000 jinjanator-23.1.0/tests/test_invalid_data.py
--rw-r--r--   0        0        0     3749 2023-07-22 18:34:47.000000 jinjanator-23.1.0/tests/test_nginx_config.py
--rw-r--r--   0        0        0      780 2023-07-22 18:34:47.000000 jinjanator-23.1.0/tests/test_output_file.py
--rw-r--r--   0        0        0      435 2023-07-22 18:34:47.000000 jinjanator-23.1.0/tests/test_template_not_found.py
--rw-r--r--   0        0        0      501 2023-07-22 18:34:47.000000 jinjanator-23.1.0/tests/test_undefined.py
--rw-r--r--   0        0        0      731 2023-07-22 18:34:47.000000 jinjanator-23.1.0/tests/test_unicode.py
--rw-r--r--   0        0        0       58 2023-07-22 18:34:47.000000 jinjanator-23.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2023-07-22 18:34:47.000000 jinjanator-23.1.0/LICENSE.apache-2.0
--rw-r--r--   0        0        0     1321 2023-07-22 18:34:47.000000 jinjanator-23.1.0/LICENSE.bsd-2-clause
--rw-r--r--   0        0        0     6886 2023-07-22 18:34:47.000000 jinjanator-23.1.0/pyproject.toml
--rw-r--r--   0        0        0     7546 2023-07-22 18:34:47.000000 jinjanator-23.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1261 2023-07-22 21:18:09.000000 jinjanator-23.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5925 2023-07-22 21:18:09.000000 jinjanator-23.2.0/PLUGINS.md
+-rw-r--r--   0        0        0     8755 2023-07-22 21:18:09.000000 jinjanator-23.2.0/README.md
+-rw-r--r--   0        0        0     1120 2023-07-22 21:18:09.000000 jinjanator-23.2.0/plugin_example/jinjanator_plugin_example.py
+-rw-r--r--   0        0        0      591 2023-07-22 21:18:09.000000 jinjanator-23.2.0/plugin_example/pyproject.toml
+-rw-r--r--   0        0        0     1747 2023-07-22 21:18:09.000000 jinjanator-23.2.0/plugin_example/tests/test_plugin.py
+-rw-r--r--   0        0        0       81 2023-07-22 21:18:09.000000 jinjanator-23.2.0/src/jinjanator/__init__.py
+-rw-r--r--   0        0        0     9507 2023-07-22 21:18:09.000000 jinjanator-23.2.0/src/jinjanator/cli.py
+-rw-r--r--   0        0        0      716 2023-07-22 21:18:09.000000 jinjanator-23.2.0/src/jinjanator/context.py
+-rw-r--r--   0        0        0     1154 2023-07-22 21:18:09.000000 jinjanator-23.2.0/src/jinjanator/filters.py
+-rw-r--r--   0        0        0     3509 2023-07-22 21:18:09.000000 jinjanator-23.2.0/src/jinjanator/formats.py
+-rw-r--r--   0        0        0     2456 2023-07-22 21:18:09.000000 jinjanator-23.2.0/src/jinjanator/plugin.py
+-rw-r--r--   0        0        0        0 2023-07-22 21:18:09.000000 jinjanator-23.2.0/src/jinjanator/py.typed
+-rw-r--r--   0        0        0      162 2023-07-22 21:18:09.000000 jinjanator-23.2.0/src/jinjanator/version.py
+-rw-r--r--   0        0        0     1614 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      675 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     1580 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_argparse.py
+-rw-r--r--   0        0        0     1284 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_cli.py
+-rw-r--r--   0        0        0     2723 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_env.py
+-rw-r--r--   0        0        0      248 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_extension.py
+-rw-r--r--   0        0        0      840 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_invalid_data.py
+-rw-r--r--   0        0        0     3749 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_nginx_config.py
+-rw-r--r--   0        0        0      780 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_output_file.py
+-rw-r--r--   0        0        0      435 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_template_not_found.py
+-rw-r--r--   0        0        0      501 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_undefined.py
+-rw-r--r--   0        0        0      731 2023-07-22 21:18:09.000000 jinjanator-23.2.0/tests/test_unicode.py
+-rw-r--r--   0        0        0       58 2023-07-22 21:18:09.000000 jinjanator-23.2.0/.gitignore
+-rw-r--r--   0        0        0    35149 2023-07-22 21:18:09.000000 jinjanator-23.2.0/LICENSE.apache-2.0
+-rw-r--r--   0        0        0     1321 2023-07-22 21:18:09.000000 jinjanator-23.2.0/LICENSE.bsd-2-clause
+-rw-r--r--   0        0        0     6950 2023-07-22 21:18:09.000000 jinjanator-23.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7647 2023-07-22 21:18:09.000000 jinjanator-23.2.0/PKG-INFO
```

### Comparing `jinjanator-23.1.0/CHANGELOG.md` & `jinjanator-23.2.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -24,12 +24,20 @@
 This changelog is managed by towncrier and is compiled at release time.
 
 See https://github.com/kpfleming/jinjanator/blob/main/.github/CONTRIBUTING.md#changelog for details.
 -->
 
 <!-- towncrier release notes start -->
 
+## [23.2.0](https://github.com/kpfleming/jinjanator/tree/23.2.0) - 2023-07-22
+
+### Fixes
+
+- Resolved crash when writing final output. Increased test coverage to avoid regressions.
+  [#7](https://github.com/kpfleming/jinjanator/issues/7)
+
+
 ## [23.1.0](https://github.com/kpfleming/jinjanator/tree/23.1.0) - 2023-07-22
 
 ### Added
 
 - Initial release!
```

### Comparing `jinjanator-23.1.0/PLUGINS.md` & `jinjanator-23.2.0/PLUGINS.md`

 * *Files identical despite different names*

### Comparing `jinjanator-23.1.0/README.md` & `jinjanator-23.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jinjanator-23.1.0/plugin_example/jinjanator_plugin_example.py` & `jinjanator-23.2.0/plugin_example/jinjanator_plugin_example.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.1.0/plugin_example/pyproject.toml` & `jinjanator-23.2.0/plugin_example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jinjanator-23.1.0/plugin_example/tests/test_plugin.py` & `jinjanator-23.2.0/plugin_example/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.1.0/src/jinjanator/cli.py` & `jinjanator-23.2.0/src/jinjanator/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
             suffix = args.data.suffix
             for k, v in available_formats.items():
                 if suffix in v.suffixes:
                     args.format = k
                     break
             if args.format == "?":
                 msg = f"no format which can read '{suffix}' files available"
-                raise ValueError(msg)
+                raise SystemExit(msg)
 
     # We always expect a file;
     # unless the user wants 'env', and there's no input file provided.
     if args.format == "env":
         """
         With the "env" format, if no dotenv filename is provided,
         we have two options: 1. The user wants to use the current
@@ -307,20 +307,19 @@
             f.write(result)
             f.close()
         return ""
 
     return result
 
 
-def main() -> int | None:
+def main(args: list[str] | None = None) -> int | None:
     try:
-        output = render_command(
-            Path.cwd(),
-            os.environ,
-            sys.stdin,
-            sys.argv,
-        )
+        if args is None:  # pragma: no cover
+            args = sys.argv
+
+        output = render_command(Path.cwd(), os.environ, sys.stdin, args)
     except SystemExit:
         return 1
-    outstream = getattr(sys.stdout, "buffer", sys.stdout)
-    outstream.write(output)
+
+    sys.stdout.write(output)
+
     return None
```

### Comparing `jinjanator-23.1.0/src/jinjanator/context.py` & `jinjanator-23.2.0/src/jinjanator/context.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.1.0/src/jinjanator/filters.py` & `jinjanator-23.2.0/src/jinjanator/filters.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.1.0/src/jinjanator/formats.py` & `jinjanator-23.2.0/src/jinjanator/formats.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.1.0/src/jinjanator/plugin.py` & `jinjanator-23.2.0/src/jinjanator/plugin.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.1.0/tests/__init__.py` & `jinjanator-23.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.1.0/tests/conftest.py` & `jinjanator-23.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.1.0/tests/test_argparse.py` & `jinjanator-23.2.0/tests/test_argparse.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.1.0/tests/test_cli.py` & `jinjanator-23.2.0/tests/test_cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 from typing import Any
 
 import pytest
 
+import jinjanator.cli
+
 from . import (
     FilePairFactory,
     render_file,
 )
 
 
 def test_quiet(make_file_pair: FilePairFactory, capsys: Any) -> None:
@@ -16,11 +18,29 @@
     captured = capsys.readouterr()
     assert len(captured.err) == 0
 
 
 def test_unavailable_suffix(make_file_pair: FilePairFactory) -> None:
     files = make_file_pair("Hello {{name}}!", "name=Blart", "xyz")
     with pytest.raises(
-        ValueError,
+        SystemExit,
         match="no format which can read '.xyz' files available",
     ):
         render_file(files, [])
+
+
+def test_main_normal(make_file_pair: FilePairFactory, capsys: Any) -> None:
+    files = make_file_pair("Hello {{name}}!", "name=Blart", "env")
+    assert (
+        jinjanator.cli.main(["--quiet", str(files.template_file), str(files.data_file)])
+        is None
+    )
+    captured = capsys.readouterr()
+    assert captured.out == "Hello Blart!"
+
+
+def test_main_failure(make_file_pair: FilePairFactory) -> None:
+    files = make_file_pair("Hello {{name}}!", "name=Blart", "xyz")
+    assert (
+        jinjanator.cli.main(["--quiet", str(files.template_file), str(files.data_file)])
+        == 1
+    )
```

### Comparing `jinjanator-23.1.0/tests/test_env.py` & `jinjanator-23.2.0/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.1.0/tests/test_invalid_data.py` & `jinjanator-23.2.0/tests/test_invalid_data.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.1.0/tests/test_nginx_config.py` & `jinjanator-23.2.0/tests/test_nginx_config.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.1.0/tests/test_output_file.py` & `jinjanator-23.2.0/tests/test_output_file.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.1.0/tests/test_unicode.py` & `jinjanator-23.2.0/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.1.0/LICENSE.apache-2.0` & `jinjanator-23.2.0/LICENSE.apache-2.0`

 * *Files identical despite different names*

### Comparing `jinjanator-23.1.0/LICENSE.bsd-2-clause` & `jinjanator-23.2.0/LICENSE.bsd-2-clause`

 * *Files identical despite different names*

### Comparing `jinjanator-23.1.0/pyproject.toml` & `jinjanator-23.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -42,23 +42,26 @@
 [project.urls]
 "Bug Tracker" = "https://github.com/kpfleming/jinjanator/issues"
 "Homepage" = "https://github.com/kpfleming/jinjanator"
 [project.scripts]
 jinjanate = "jinjanator.cli:main"
 
 [tool.hatch.envs.changelog]
+skip-install = true
 dependencies = [
   "towncrier",
 ]
 
 [tool.hatch.envs.changelog.scripts]
 draft = [
+  "rm changelog.d/*~",
   "towncrier build --version main --draft",
 ]
 release = [
+  "rm changelog.d/*~",
   "towncrier build --version {args}",
 ]
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
@@ -137,15 +140,15 @@
 ]
 
 [tool.hatch.envs.ci.scripts]
 ci = [
     "pip install ./plugin_example",
     "rm -f .coverage",
     # run tests
-    "pytest --verbose --cov-append  --cov-branch --cov-fail-under=96 --cov=jinjanator",
+    "pytest --verbose --cov-append  --cov-branch --cov-fail-under=98 --cov=jinjanator",
     # produce a coverage report with 'missing' lines indicated
     "coverage report -m",
 ]
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 
@@ -164,15 +167,15 @@
 text = """
 ## Release Information
 """
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "CHANGELOG.md"
 start-after = "<!-- towncrier release notes start -->"
-# pattern = "\n(###.+?\n)## "
+pattern = "\n(###.+?\n)## "
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 text = """
 ---
 [→ Full Changelog](https://github.com/kpfleming/jinjanator/blob/main/CHANGELOG.md)
 """
```

### Comparing `jinjanator-23.1.0/PKG-INFO` & `jinjanator-23.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjanator
-Version: 23.1.0
+Version: 23.2.0
 Summary: Command-line interface to Jinja2 for templating in shell scripts.
 Project-URL: Bug Tracker, https://github.com/kpfleming/jinjanator/issues
 Project-URL: Homepage, https://github.com/kpfleming/jinjanator
 Author-email: "Kevin P. Fleming" <jinjanator@kevin.km6g.us>, Mark Vartanyan <kolypto@gmail.com>
 License: Apache-2.0
 License-File: LICENSE.apache-2.0
 License-File: LICENSE.bsd-2-clause
@@ -310,16 +310,15 @@
 Pass: {{ env("USER_PASSWORD") }}
 ```
 
 Notice that there must be quotes around the environment variable name
 when it is a literal string.
 
 ## Release Information
+### Fixes
 
+- Resolved crash when writing final output. Increased test coverage to avoid regressions.
+  [[#7](https://github.com/kpfleming/jinjanator/issues/7)](https://github.com/kpfleming/jinjanator/issues/7)
 
-## [23.1.0](https://github.com/kpfleming/jinjanator/tree/23.1.0) - 2023-07-22
 
-### Added
-
-- Initial release!
 ---
 [→ Full Changelog](https://github.com/kpfleming/jinjanator/blob/main/CHANGELOG.md)
```

