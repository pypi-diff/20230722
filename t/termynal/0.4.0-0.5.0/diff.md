# Comparing `tmp/termynal-0.4.0.tar.gz` & `tmp/termynal-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termynal-0.4.0.tar", max compression
+gzip compressed data, was "termynal-0.5.0.tar", max compression
```

## Comparing `termynal-0.4.0.tar` & `termynal-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1092 2023-07-06 12:49:35.725065 termynal-0.4.0/LICENSE
--rw-r--r--   0        0        0     1067 2023-07-06 12:49:35.725065 termynal-0.4.0/README.md
--rw-r--r--   0        0        0     2388 2023-07-06 12:49:35.725065 termynal-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-06 12:49:35.725065 termynal-0.4.0/termynal/__init__.py
--rw-r--r--   0        0        0     2281 2023-07-06 12:49:35.725065 termynal-0.4.0/termynal/assets/termynal.css
--rw-r--r--   0        0        0     9704 2023-07-06 12:49:35.725065 termynal-0.4.0/termynal/assets/termynal.js
--rw-r--r--   0        0        0     4617 2023-07-06 12:49:35.725065 termynal-0.4.0/termynal/markdown.py
--rw-r--r--   0        0        0     1121 2023-07-06 12:49:35.725065 termynal-0.4.0/termynal/plugin.py
--rw-r--r--   0        0        0     2091 1970-01-01 00:00:00.000000 termynal-0.4.0/setup.py
--rw-r--r--   0        0        0     1732 1970-01-01 00:00:00.000000 termynal-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-22 16:51:35.582324 termynal-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1758 2023-07-22 16:51:35.582324 termynal-0.5.0/README.md
+-rw-r--r--   0        0        0     2415 2023-07-22 16:51:35.582324 termynal-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-22 16:51:35.582324 termynal-0.5.0/termynal/__init__.py
+-rw-r--r--   0        0        0     2281 2023-07-22 16:51:35.582324 termynal-0.5.0/termynal/assets/termynal.css
+-rw-r--r--   0        0        0     9704 2023-07-22 16:51:35.582324 termynal-0.5.0/termynal/assets/termynal.js
+-rw-r--r--   0        0        0     5541 2023-07-22 16:51:35.582324 termynal-0.5.0/termynal/markdown.py
+-rw-r--r--   0        0        0     1121 2023-07-22 16:51:35.582324 termynal-0.5.0/termynal/plugin.py
+-rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 termynal-0.5.0/PKG-INFO
```

### Comparing `termynal-0.4.0/LICENSE` & `termynal-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `termynal-0.4.0/pyproject.toml` & `termynal-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.4.0"
+version = "0.5.0"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version"
 ]
 bump_message = "chore(release): version $current_version → $new_version"
 update_changelog_on_bump = true
 
 [tool.poetry]
 name = "termynal"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["Danil Akhtarov <daxartio@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/daxartio/termynal"
 homepage = "https://pypi.org/project/termynal"
 keywords = []
@@ -39,19 +39,20 @@
 pytest-deadfixtures = "*"
 pytest-mock = "*"
 ruff = "*"
 toml = "*"
 types-Markdown = "*"
 
 [tool.poetry.group.docs.dependencies]
+markdown-include = "^0.8.1"
 mkdocs = "*"
 mkdocs-material = "*"
 
 [tool.poetry.group.git.dependencies]
-commitizen = "^2.39.1"
+commitizen = "^3.5.3"
 
 [tool.poetry.extras]
 mkdocs = ["mkdocs"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `termynal-0.4.0/termynal/assets/termynal.css` & `termynal-0.5.0/termynal/assets/termynal.css`

 * *Files identical despite different names*

### Comparing `termynal-0.4.0/termynal/assets/termynal.js` & `termynal-0.5.0/termynal/assets/termynal.js`

 * *Files identical despite different names*

### Comparing `termynal-0.4.0/termynal/markdown.py` & `termynal-0.5.0/termynal/markdown.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,29 +8,47 @@
     from markdown import core
 
 
 class Termynal:
     progress_literal_start = "---&gt; 100%"
     custom_literal_start = "# "
 
-    def __init__(self, prompt_literal_start: tuple = ("$ ",)):
+    def __init__(
+        self,
+        prompt_literal_start: tuple = ("$ ",),
+        promt_in_multiline: bool = False,
+    ):
         """Initialize."""
         self.prompt_literal_start = "|".join(re.escape(p) for p in prompt_literal_start)
         self.regex_prompts = re.compile(f"^({self.prompt_literal_start})")
+        self.promt_in_multiline = promt_in_multiline
 
     def convert(self, code: str) -> List[str]:
         code_lines = []
         code_lines.append('<div class="termy" data-termynal>')
+        multiline = False
+        used_prompt = None
         for line in code.split("\n"):
             if match := self.regex_prompts.match(line):
                 used_prompt = match.group()
                 code_lines.append(
                     f'<span data-ty="input" data-ty-prompt="{used_prompt.strip()}">'
-                    f"{line.rsplit(used_prompt)[1]}</span>",
+                    f"{line.rsplit(used_prompt)[1].replace(' ', '&nbsp;')}</span>",
+                )
+                multiline = bool(line.endswith("\\"))
+            elif multiline:
+                used_prompt = used_prompt or ""
+                if not self.promt_in_multiline:
+                    used_prompt = ""
+                code_lines.append(
+                    f'<span data-ty="input" data-ty-prompt="{used_prompt.strip()}">'
+                    f'{line.replace(" ", "&nbsp;")}</span>',
                 )
+                multiline = bool(line.endswith("\\"))
+
             elif line.startswith(self.custom_literal_start):
                 code_lines.append(
                     f'<span class="termynal-comment" data-ty>{line}</span>',
                 )
             elif line.startswith(self.progress_literal_start):
                 code_lines.append('<span data-ty="progress"></span>')
             else:
@@ -43,14 +61,15 @@
     rexep = re.compile("(<code.*>)((.|\n)*?)(</code>)")
     comment = "<!-- termynal -->"
     language_class = 'class="language-console"'
 
     def __init__(self, config: dict, md: "core.Markdown"):
         """Initialize."""
         self.prompt_literal_start = config.get("prompt_literal_start", ("$ ",))
+        self.promt_in_multiline = config.get("promt_in_multiline", False)
 
         super(TermynalPreprocessor, self).__init__(md=md)
 
     def run(self, lines: List):
         content_by_placeholder = {}
         for i in range(self.md.htmlStash.html_counter):
             placeholder = self.md.htmlStash.get_placeholder(i)
@@ -68,15 +87,18 @@
         return new_lines
 
     def _get_lines(
         self,
         lines: List,
         content_by_placeholder: Dict,
     ):  # pylint:disable=too-many-nested-blocks
-        termynal_obj = Termynal(prompt_literal_start=self.prompt_literal_start)
+        termynal_obj = Termynal(
+            prompt_literal_start=self.prompt_literal_start,
+            promt_in_multiline=self.promt_in_multiline,
+        )
         lines_by_placeholder = {}
         is_termynal_code = False
         for line in lines:
             if line in content_by_placeholder:
                 (content, i) = content_by_placeholder[line]
 
                 if not isinstance(content, str):
@@ -113,14 +135,18 @@
             "prompt_literal_start": [
                 [
                     "$ ",
                 ],
                 "A list of prompt characters start to consider as console - "
                 "Default: ['$ ',]",
             ],
+            "promt_in_multiline": [
+                False,
+                "Default: False",
+            ],
         }
 
         super(TermynalExtension, self).__init__(*args, **kwargs)
 
     def extendMarkdown(self, md: "core.Markdown"):  # noqa:N802
         """Register the extension."""
         md.registerExtension(self)
```

### Comparing `termynal-0.4.0/termynal/plugin.py` & `termynal-0.5.0/termynal/plugin.py`

 * *Files identical despite different names*

### Comparing `termynal-0.4.0/PKG-INFO` & `termynal-0.5.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termynal
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Home-page: https://pypi.org/project/termynal
 License: MIT
 Author: Danil Akhtarov
 Author-email: daxartio@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,22 @@
 Requires-Dist: markdown
 Requires-Dist: mkdocs (>=1.4,<2.0) ; extra == "mkdocs"
 Project-URL: Repository, https://github.com/daxartio/termynal
 Description-Content-Type: text/markdown
 
 # Termynal
 
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/daxartio/termynal/check.yml)
+[![PyPI](https://img.shields.io/pypi/v/termynal)](https://pypi.org/project/termynal/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/termynal)](https://www.python.org/downloads/)
+[![Docs](https://img.shields.io/badge/docs-latest-blue)](https://daxartio.github.io/termynal/)
+![GitHub](https://img.shields.io/github/license/daxartio/termynal)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/termynal)
+![GitHub last commit](https://img.shields.io/github/last-commit/daxartio/termynal)
+
 A lightweight and modern animated terminal window.
 Built for [mkdocs](https://www.mkdocs.org/).
 
 ## Installation
 
 <!-- termynal -->
 
@@ -117,7 +125,11 @@
 
 ````
 
 ## Credits
 
 Thanks [ines](https://github.com/ines/termynal)
 
+## Contribution
+
+[Contribution guidelines for this project](CONTRIBUTING.md)
+
```

