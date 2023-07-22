# Comparing `tmp/mkdocs_file_filter_plugin-0.0.8.tar.gz` & `tmp/mkdocs_file_filter_plugin-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_file_filter_plugin-0.0.8.tar", max compression
+gzip compressed data, was "mkdocs_file_filter_plugin-0.1.0.tar", max compression
```

## Comparing `mkdocs_file_filter_plugin-0.0.8.tar` & `mkdocs_file_filter_plugin-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-05-16 02:18:36.738991 mkdocs_file_filter_plugin-0.0.8/LICENSE
--rw-r--r--   0        0        0    17036 2023-05-16 02:18:36.738991 mkdocs_file_filter_plugin-0.0.8/README.md
--rw-r--r--   0        0        0       11 2023-05-16 02:18:36.738991 mkdocs_file_filter_plugin-0.0.8/mkdocs_file_filter_plugin/__init__.py
--rw-r--r--   0        0        0     1824 2023-05-16 02:18:36.738991 mkdocs_file_filter_plugin-0.0.8/mkdocs_file_filter_plugin/external_config.py
--rw-r--r--   0        0        0     4658 2023-05-16 02:18:36.738991 mkdocs_file_filter_plugin-0.0.8/mkdocs_file_filter_plugin/judger.py
--rw-r--r--   0        0        0      974 2023-05-16 02:18:36.738991 mkdocs_file_filter_plugin-0.0.8/mkdocs_file_filter_plugin/logger.py
--rw-r--r--   0        0        0     4899 2023-05-16 02:18:36.738991 mkdocs_file_filter_plugin-0.0.8/mkdocs_file_filter_plugin/plugin.py
--rw-r--r--   0        0        0     1169 2023-05-16 02:18:36.738991 mkdocs_file_filter_plugin-0.0.8/mkdocs_file_filter_plugin/plugin_config.py
--rw-r--r--   0        0        0     6574 2023-05-16 02:19:00.467415 mkdocs_file_filter_plugin-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    18996 1970-01-01 00:00:00.000000 mkdocs_file_filter_plugin-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-22 18:06:33.473317 mkdocs_file_filter_plugin-0.1.0/LICENSE
+-rw-r--r--   0        0        0    17036 2023-07-22 18:06:33.473317 mkdocs_file_filter_plugin-0.1.0/README.md
+-rw-r--r--   0        0        0       11 2023-07-22 18:06:33.473317 mkdocs_file_filter_plugin-0.1.0/mkdocs_file_filter_plugin/__init__.py
+-rw-r--r--   0        0        0     1824 2023-07-22 18:06:33.473317 mkdocs_file_filter_plugin-0.1.0/mkdocs_file_filter_plugin/external_config.py
+-rw-r--r--   0        0        0     4658 2023-07-22 18:06:33.473317 mkdocs_file_filter_plugin-0.1.0/mkdocs_file_filter_plugin/judger.py
+-rw-r--r--   0        0        0      974 2023-07-22 18:06:33.473317 mkdocs_file_filter_plugin-0.1.0/mkdocs_file_filter_plugin/logger.py
+-rw-r--r--   0        0        0     4899 2023-07-22 18:06:33.473317 mkdocs_file_filter_plugin-0.1.0/mkdocs_file_filter_plugin/plugin.py
+-rw-r--r--   0        0        0     1169 2023-07-22 18:06:33.473317 mkdocs_file_filter_plugin-0.1.0/mkdocs_file_filter_plugin/plugin_config.py
+-rw-r--r--   0        0        0     6578 2023-07-22 18:07:00.301979 mkdocs_file_filter_plugin-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    18794 1970-01-01 00:00:00.000000 mkdocs_file_filter_plugin-0.1.0/PKG-INFO
```

### Comparing `mkdocs_file_filter_plugin-0.0.8/LICENSE` & `mkdocs_file_filter_plugin-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_file_filter_plugin-0.0.8/README.md` & `mkdocs_file_filter_plugin-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_file_filter_plugin-0.0.8/mkdocs_file_filter_plugin/external_config.py` & `mkdocs_file_filter_plugin-0.1.0/mkdocs_file_filter_plugin/external_config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_file_filter_plugin-0.0.8/mkdocs_file_filter_plugin/judger.py` & `mkdocs_file_filter_plugin-0.1.0/mkdocs_file_filter_plugin/judger.py`

 * *Files identical despite different names*

### Comparing `mkdocs_file_filter_plugin-0.0.8/mkdocs_file_filter_plugin/logger.py` & `mkdocs_file_filter_plugin-0.1.0/mkdocs_file_filter_plugin/logger.py`

 * *Files identical despite different names*

### Comparing `mkdocs_file_filter_plugin-0.0.8/mkdocs_file_filter_plugin/plugin.py` & `mkdocs_file_filter_plugin-0.1.0/mkdocs_file_filter_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_file_filter_plugin-0.0.8/mkdocs_file_filter_plugin/plugin_config.py` & `mkdocs_file_filter_plugin-0.1.0/mkdocs_file_filter_plugin/plugin_config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_file_filter_plugin-0.0.8/pyproject.toml` & `mkdocs_file_filter_plugin-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-file-filter-plugin"
-version = "0.0.8"
+version = "0.1.0"
 description = 'A MkDocs plugin that lets you exclude/include docs files using globs, regexes, gitignore-style file and Markdown/Frontmatter tags metadata.'
 authors = [
   "Dariusz Porowski <3431813+dariuszporowski@users.noreply.github.com>",
 ]
 homepage = "https://github.com/DariuszPorowski/mkdocs-file-filter-plugin"
 repository = "https://github.com/DariuszPorowski/mkdocs-file-filter-plugin"
 documentation = "https://github.com/DariuszPorowski/mkdocs-file-filter-plugin/blob/main/README.md"
@@ -47,36 +47,36 @@
 [tool.poetry.plugins."mkdocs.plugins"]
 file-filter = "mkdocs_file_filter_plugin.plugin:FileFilter"
 file_filter = "mkdocs_file_filter_plugin.plugin:FileFilter"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 mkdocs = "^1.4.3"
-igittigitt = "^2.1.2"
+igittigitt = "^2.1.4"
 schema = "^0.7.5"
-pyyaml = "^6.0"
+pyyaml = ">=5.1,<7"
 pyyaml-env-tag = "^0.1"
 
 [tool.poetry.group.dev.dependencies]
-mkdocs-material = "^9.1.12"
+mkdocs-material = "^9.1.19"
 mkdocs-awesome-pages-plugin = "^2.9.1"
-mkdocs-exclude-unused-files = "^1.1.0"
+mkdocs-exclude-unused-files = "^1.2.1"
 isort = "^5.12.0"
-black = "^23.3.0"
+black = "^23.7.0"
 pylint = "^2.17.4"
 flake8 = "^6.0.0"
-mypy = "^1.3.0"
+mypy = "^1.4.1"
 mypy-extensions = "^1.0.0"
 pydocstyle = "^6.3.0"
 bandit = "^1.7.5"
-pytest = "^7.3.1"
-pytest-cov = "^4.0.0"
-pre-commit = "^3.3.1"
-ruff = "^0.0.267"
-pyupgrade = "^3.4.0"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
+pre-commit = "^3.3.3"
+ruff = "^0.0.280"
+pyupgrade = "^3.9.0"
 
 [tool.poetry.plugins."poetry-plugin-up"]
 # https://github.com/MousaZeidBaker/poetry-plugin-up#usage
 
 [tool.poetry-dynamic-versioning]
 # https://github.com/mtkennerly/poetry-dynamic-versioning#configuration
 enable = false
```

### Comparing `mkdocs_file_filter_plugin-0.0.8/PKG-INFO` & `mkdocs_file_filter_plugin-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-file-filter-plugin
-Version: 0.0.8
+Version: 0.1.0
 Summary: A MkDocs plugin that lets you exclude/include docs files using globs, regexes, gitignore-style file and Markdown/Frontmatter tags metadata.
 Home-page: https://github.com/DariuszPorowski/mkdocs-file-filter-plugin
 License: MIT
 Keywords: mkdocs,plugin,exclude,include,glob,regex,gitignore,markdown,frontmatter,metadata,tags
 Author: Dariusz Porowski
 Author-email: 3431813+dariuszporowski@users.noreply.github.com
 Requires-Python: >=3.8.1,<4.0
@@ -14,24 +14,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Documentation
-Requires-Dist: igittigitt (>=2.1.2,<3.0.0)
+Requires-Dist: igittigitt (>=2.1.4,<3.0.0)
 Requires-Dist: mkdocs (>=1.4.3,<2.0.0)
-Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: pyyaml (>=5.1,<7)
 Requires-Dist: pyyaml-env-tag (>=0.1,<0.2)
 Requires-Dist: schema (>=0.7.5,<0.8.0)
 Project-URL: Documentation, https://github.com/DariuszPorowski/mkdocs-file-filter-plugin/blob/main/README.md
 Project-URL: History, https://github.com/DariuszPorowski/mkdocs-file-filter-plugin/releases
 Project-URL: Issues, https://github.com/DariuszPorowski/mkdocs-file-filter-plugin/issues
 Project-URL: Repository, https://github.com/DariuszPorowski/mkdocs-file-filter-plugin
 Description-Content-Type: text/markdown
```

