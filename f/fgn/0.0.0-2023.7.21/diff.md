# Comparing `tmp/fgn-0.0.0.tar.gz` & `tmp/fgn-2023.7.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgn-0.0.0.tar", last modified: Fri Jul 21 19:13:24 2023, max compression
+gzip compressed data, was "fgn-2023.7.21.tar", last modified: Sat Jul 22 00:39:58 2023, max compression
```

## Comparing `fgn-0.0.0.tar` & `fgn-2023.7.21.tar`

### file list

```diff
@@ -1,48 +1,223 @@
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-21 19:13:24.188977 fgn-0.0.0/
--rw-r--r--   0 candacechatman   (501) staff       (20)      586 2023-07-21 16:52:47.000000 fgn-0.0.0/.coveragerc
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-21 19:13:24.182110 fgn-0.0.0/.github/
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-21 19:13:24.185103 fgn-0.0.0/.github/workflows/
--rw-r--r--   0 candacechatman   (501) staff       (20)     4382 2023-07-21 18:56:18.000000 fgn-0.0.0/.github/workflows/ci.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)      566 2023-07-21 16:52:47.000000 fgn-0.0.0/.gitignore
--rw-r--r--   0 candacechatman   (501) staff       (20)       51 2023-07-21 16:52:47.000000 fgn-0.0.0/.isort.cfg
--rw-r--r--   0 candacechatman   (501) staff       (20)     1670 2023-07-21 16:55:22.000000 fgn-0.0.0/.pre-commit-config.yaml
--rw-r--r--   0 candacechatman   (501) staff       (20)      530 2023-07-21 16:52:47.000000 fgn-0.0.0/.readthedocs.yml
--rw-r--r--   0 candacechatman   (501) staff       (20)       77 2023-07-21 16:52:47.000000 fgn-0.0.0/AUTHORS.rst
--rw-r--r--   0 candacechatman   (501) staff       (20)      134 2023-07-21 17:25:04.000000 fgn-0.0.0/CHANGELOG.rst
--rw-r--r--   0 candacechatman   (501) staff       (20)    13762 2023-07-21 16:52:47.000000 fgn-0.0.0/CONTRIBUTING.rst
--rw-r--r--   0 candacechatman   (501) staff       (20)     1079 2023-07-21 16:52:47.000000 fgn-0.0.0/LICENSE.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)     2440 2023-07-21 19:13:24.189063 fgn-0.0.0/PKG-INFO
--rw-r--r--   0 candacechatman   (501) staff       (20)     1982 2023-07-21 16:52:47.000000 fgn-0.0.0/README.rst
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-21 19:13:24.186611 fgn-0.0.0/docs/
--rw-r--r--   0 candacechatman   (501) staff       (20)     1154 2023-07-21 16:52:47.000000 fgn-0.0.0/docs/Makefile
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-21 19:13:24.186739 fgn-0.0.0/docs/_static/
--rw-r--r--   0 candacechatman   (501) staff       (20)       18 2023-07-21 16:52:47.000000 fgn-0.0.0/docs/_static/.gitignore
--rw-r--r--   0 candacechatman   (501) staff       (20)       41 2023-07-21 16:52:47.000000 fgn-0.0.0/docs/authors.rst
--rw-r--r--   0 candacechatman   (501) staff       (20)       43 2023-07-21 16:52:47.000000 fgn-0.0.0/docs/changelog.rst
--rw-r--r--   0 candacechatman   (501) staff       (20)     9714 2023-07-21 16:52:47.000000 fgn-0.0.0/docs/conf.py
--rw-r--r--   0 candacechatman   (501) staff       (20)       33 2023-07-21 16:52:47.000000 fgn-0.0.0/docs/contributing.rst
--rw-r--r--   0 candacechatman   (501) staff       (20)     2297 2023-07-21 16:52:47.000000 fgn-0.0.0/docs/index.rst
--rw-r--r--   0 candacechatman   (501) staff       (20)       67 2023-07-21 16:52:47.000000 fgn-0.0.0/docs/license.rst
--rw-r--r--   0 candacechatman   (501) staff       (20)       39 2023-07-21 16:52:47.000000 fgn-0.0.0/docs/readme.rst
--rw-r--r--   0 candacechatman   (501) staff       (20)      233 2023-07-21 16:52:47.000000 fgn-0.0.0/docs/requirements.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)      346 2023-07-21 16:52:47.000000 fgn-0.0.0/pyproject.toml
--rw-r--r--   0 candacechatman   (501) staff       (20)     1235 2023-07-21 19:13:24.189429 fgn-0.0.0/setup.cfg
--rw-r--r--   0 candacechatman   (501) staff       (20)      698 2023-07-21 16:52:47.000000 fgn-0.0.0/setup.py
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-21 19:13:24.182465 fgn-0.0.0/src/
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-21 19:13:24.187383 fgn-0.0.0/src/fgn/
--rw-r--r--   0 candacechatman   (501) staff       (20)      577 2023-07-21 16:52:47.000000 fgn-0.0.0/src/fgn/__init__.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      422 2023-07-21 18:43:35.000000 fgn-0.0.0/src/fgn/cli.py
--rw-r--r--   0 candacechatman   (501) staff       (20)     4192 2023-07-21 16:52:47.000000 fgn-0.0.0/src/fgn/skeleton.py
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-21 19:13:24.188268 fgn-0.0.0/src/fgn.egg-info/
--rw-r--r--   0 candacechatman   (501) staff       (20)     2440 2023-07-21 19:13:24.000000 fgn-0.0.0/src/fgn.egg-info/PKG-INFO
--rw-r--r--   0 candacechatman   (501) staff       (20)      718 2023-07-21 19:13:24.000000 fgn-0.0.0/src/fgn.egg-info/SOURCES.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        1 2023-07-21 19:13:24.000000 fgn-0.0.0/src/fgn.egg-info/dependency_links.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)       37 2023-07-21 19:13:24.000000 fgn-0.0.0/src/fgn.egg-info/entry_points.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        1 2023-07-21 16:56:59.000000 fgn-0.0.0/src/fgn.egg-info/not-zip-safe
--rw-r--r--   0 candacechatman   (501) staff       (20)      102 2023-07-21 19:13:24.000000 fgn-0.0.0/src/fgn.egg-info/requires.txt
--rw-r--r--   0 candacechatman   (501) staff       (20)        4 2023-07-21 19:13:24.000000 fgn-0.0.0/src/fgn.egg-info/top_level.txt
-drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-21 19:13:24.188790 fgn-0.0.0/tests/
--rw-r--r--   0 candacechatman   (501) staff       (20)      271 2023-07-21 16:52:47.000000 fgn-0.0.0/tests/conftest.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      855 2023-07-21 18:47:03.000000 fgn-0.0.0/tests/test_cli.py
--rw-r--r--   0 candacechatman   (501) staff       (20)      599 2023-07-21 17:15:32.000000 fgn-0.0.0/tests/test_skeleton.py
--rw-r--r--   0 candacechatman   (501) staff       (20)     2851 2023-07-21 16:52:47.000000 fgn-0.0.0/tox.ini
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.839191 fgn-2023.7.21/
+-rw-r--r--   0 candacechatman   (501) staff       (20)      586 2023-07-21 16:52:47.000000 fgn-2023.7.21/.coveragerc
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.811812 fgn-2023.7.21/.github/
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.816058 fgn-2023.7.21/.github/workflows/
+-rw-r--r--   0 candacechatman   (501) staff       (20)     4382 2023-07-21 18:56:18.000000 fgn-2023.7.21/.github/workflows/ci.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)      566 2023-07-21 16:52:47.000000 fgn-2023.7.21/.gitignore
+-rw-r--r--   0 candacechatman   (501) staff       (20)       51 2023-07-21 16:52:47.000000 fgn-2023.7.21/.isort.cfg
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1670 2023-07-21 16:55:22.000000 fgn-2023.7.21/.pre-commit-config.yaml
+-rw-r--r--   0 candacechatman   (501) staff       (20)      530 2023-07-21 16:52:47.000000 fgn-2023.7.21/.readthedocs.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)       77 2023-07-21 16:52:47.000000 fgn-2023.7.21/AUTHORS.rst
+-rw-r--r--   0 candacechatman   (501) staff       (20)      134 2023-07-21 17:25:04.000000 fgn-2023.7.21/CHANGELOG.rst
+-rw-r--r--   0 candacechatman   (501) staff       (20)    13762 2023-07-21 16:52:47.000000 fgn-2023.7.21/CONTRIBUTING.rst
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1079 2023-07-21 16:52:47.000000 fgn-2023.7.21/LICENSE.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)       37 2023-07-22 00:10:12.000000 fgn-2023.7.21/MANIFEST.in
+-rw-r--r--   0 candacechatman   (501) staff       (20)     7038 2023-07-22 00:39:58.839273 fgn-2023.7.21/PKG-INFO
+-rw-r--r--   0 candacechatman   (501) staff       (20)     6538 2023-07-22 00:38:10.000000 fgn-2023.7.21/README.rst
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.817669 fgn-2023.7.21/docs/
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1154 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/Makefile
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.817807 fgn-2023.7.21/docs/_static/
+-rw-r--r--   0 candacechatman   (501) staff       (20)       18 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/_static/.gitignore
+-rw-r--r--   0 candacechatman   (501) staff       (20)       41 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/authors.rst
+-rw-r--r--   0 candacechatman   (501) staff       (20)       43 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/changelog.rst
+-rw-r--r--   0 candacechatman   (501) staff       (20)     9714 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/conf.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)       33 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/contributing.rst
+-rw-r--r--   0 candacechatman   (501) staff       (20)     2297 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/index.rst
+-rw-r--r--   0 candacechatman   (501) staff       (20)       67 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/license.rst
+-rw-r--r--   0 candacechatman   (501) staff       (20)       39 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/readme.rst
+-rw-r--r--   0 candacechatman   (501) staff       (20)      233 2023-07-21 16:52:47.000000 fgn-2023.7.21/docs/requirements.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)      346 2023-07-21 16:52:47.000000 fgn-2023.7.21/pyproject.toml
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1398 2023-07-22 00:39:58.839694 fgn-2023.7.21/setup.cfg
+-rw-r--r--   0 candacechatman   (501) staff       (20)      693 2023-07-22 00:34:27.000000 fgn-2023.7.21/setup.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.812082 fgn-2023.7.21/src/
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.818286 fgn-2023.7.21/src/fgn/
+-rw-r--r--   0 candacechatman   (501) staff       (20)      577 2023-07-21 16:52:47.000000 fgn-2023.7.21/src/fgn/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      532 2023-07-21 21:57:44.000000 fgn-2023.7.21/src/fgn/cli.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.820542 fgn-2023.7.21/src/fgn/core/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-30 20:42:36.000000 fgn-2023.7.21/src/fgn/core/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     5894 2023-07-21 22:06:39.000000 fgn-2023.7.21/src/fgn/core/chat_agent.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1336 2023-07-22 00:08:39.000000 fgn-2023.7.21/src/fgn/core/command_context.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.820779 fgn-2023.7.21/src/fgn/core/commands/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-01 20:36:22.000000 fgn-2023.7.21/src/fgn/core/commands/__init__.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.821757 fgn-2023.7.21/src/fgn/core/commands/blog/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 01:45:16.000000 fgn-2023.7.21/src/fgn/core/commands/blog/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      401 2023-07-22 00:08:39.000000 fgn-2023.7.21/src/fgn/core/commands/blog/blog_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      284 2023-03-29 22:12:51.000000 fgn-2023.7.21/src/fgn/core/commands/blog/blog_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 01:45:16.000000 fgn-2023.7.21/src/fgn/core/commands/blog/blog_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 01:45:16.000000 fgn-2023.7.21/src/fgn/core/commands/blog/blog_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1932 2023-04-19 20:56:19.000000 fgn-2023.7.21/src/fgn/core/commands/blog/blog_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 01:45:16.000000 fgn-2023.7.21/src/fgn/core/commands/blog/blog_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.822664 fgn-2023.7.21/src/fgn/core/commands/chain/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 01:31:14.000000 fgn-2023.7.21/src/fgn/core/commands/chain/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1522 2023-07-22 00:14:45.000000 fgn-2023.7.21/src/fgn/core/commands/chain/chain_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      268 2023-04-14 01:31:14.000000 fgn-2023.7.21/src/fgn/core/commands/chain/chain_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 00:34:48.000000 fgn-2023.7.21/src/fgn/core/commands/chain/chain_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 01:31:14.000000 fgn-2023.7.21/src/fgn/core/commands/chain/chain_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)    10183 2023-04-19 23:20:50.000000 fgn-2023.7.21/src/fgn/core/commands/chain/chain_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 01:31:14.000000 fgn-2023.7.21/src/fgn/core/commands/chain/chain_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.823434 fgn-2023.7.21/src/fgn/core/commands/code/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 00:16:54.000000 fgn-2023.7.21/src/fgn/core/commands/code/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      452 2023-04-23 07:52:01.000000 fgn-2023.7.21/src/fgn/core/commands/code/code_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      293 2023-04-21 18:43:00.000000 fgn-2023.7.21/src/fgn/core/commands/code/code_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 00:16:54.000000 fgn-2023.7.21/src/fgn/core/commands/code/code_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-29 00:16:54.000000 fgn-2023.7.21/src/fgn/core/commands/code/code_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-21 18:42:58.000000 fgn-2023.7.21/src/fgn/core/commands/code/code_schema.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     4092 2023-04-29 20:34:41.000000 fgn-2023.7.21/src/fgn/core/commands/code/code_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)      275 2023-03-29 00:19:20.000000 fgn-2023.7.21/src/fgn/core/commands/code/code_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.823648 fgn-2023.7.21/src/fgn/core/commands/core/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 01:07:18.000000 fgn-2023.7.21/src/fgn/core/commands/core/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      377 2023-04-14 01:38:20.000000 fgn-2023.7.21/src/fgn/core/commands/core/core_cmd.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.825024 fgn-2023.7.21/src/fgn/core/commands/dsl/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-11 03:26:13.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      415 2023-04-14 03:12:15.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/dsl_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      256 2023-04-11 19:24:14.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/dsl_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)     6522 2023-04-11 19:24:14.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/dsl_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-11 03:26:13.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/dsl_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)      634 2023-04-11 19:31:02.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/dsl_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)      931 2023-04-11 19:31:02.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/dsl_template.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)      367 2023-04-08 03:58:38.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/main.yaml
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1697 2023-04-08 21:49:12.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/newsletter.yaml
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1674 2023-04-08 04:35:12.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/newsletter2.yaml
+-rw-r--r--   0 candacechatman   (501) staff       (20)      265 2023-04-08 03:58:15.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/sub.yaml
+-rw-r--r--   0 candacechatman   (501) staff       (20)     2811 2023-04-08 20:38:17.000000 fgn-2023.7.21/src/fgn/core/commands/dsl/switch.yaml
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.825904 fgn-2023.7.21/src/fgn/core/commands/feedback/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 22:37:07.000000 fgn-2023.7.21/src/fgn/core/commands/feedback/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      438 2023-05-01 01:46:44.000000 fgn-2023.7.21/src/fgn/core/commands/feedback/feedback_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      286 2023-04-19 22:37:07.000000 fgn-2023.7.21/src/fgn/core/commands/feedback/feedback_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 22:37:07.000000 fgn-2023.7.21/src/fgn/core/commands/feedback/feedback_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     4244 2023-04-19 23:06:06.000000 fgn-2023.7.21/src/fgn/core/commands/feedback/feedback_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1996 2023-04-19 22:47:50.000000 fgn-2023.7.21/src/fgn/core/commands/feedback/feedback_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 22:37:07.000000 fgn-2023.7.21/src/fgn/core/commands/feedback/feedback_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.826846 fgn-2023.7.21/src/fgn/core/commands/fun/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-06-22 18:48:42.000000 fgn-2023.7.21/src/fgn/core/commands/fun/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      575 2023-07-22 00:08:39.000000 fgn-2023.7.21/src/fgn/core/commands/fun/fun_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      256 2023-06-22 18:48:42.000000 fgn-2023.7.21/src/fgn/core/commands/fun/fun_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-06-22 18:48:42.000000 fgn-2023.7.21/src/fgn/core/commands/fun/fun_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-06-22 18:48:42.000000 fgn-2023.7.21/src/fgn/core/commands/fun/fun_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     7750 2023-06-22 18:53:35.000000 fgn-2023.7.21/src/fgn/core/commands/fun/fun_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-06-22 18:48:42.000000 fgn-2023.7.21/src/fgn/core/commands/fun/fun_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.827733 fgn-2023.7.21/src/fgn/core/commands/guide/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 01:30:55.000000 fgn-2023.7.21/src/fgn/core/commands/guide/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      407 2023-07-22 00:14:45.000000 fgn-2023.7.21/src/fgn/core/commands/guide/guide_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      268 2023-04-12 01:30:55.000000 fgn-2023.7.21/src/fgn/core/commands/guide/guide_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 01:30:55.000000 fgn-2023.7.21/src/fgn/core/commands/guide/guide_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 01:30:55.000000 fgn-2023.7.21/src/fgn/core/commands/guide/guide_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     4999 2023-04-19 23:13:20.000000 fgn-2023.7.21/src/fgn/core/commands/guide/guide_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 01:30:55.000000 fgn-2023.7.21/src/fgn/core/commands/guide/guide_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.828913 fgn-2023.7.21/src/fgn/core/commands/help/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-13 20:52:14.000000 fgn-2023.7.21/src/fgn/core/commands/help/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)    10159 2023-04-17 03:25:54.000000 fgn-2023.7.21/src/fgn/core/commands/help/help-in.md
+-rw-r--r--   0 candacechatman   (501) staff       (20)      405 2023-04-14 03:12:15.000000 fgn-2023.7.21/src/fgn/core/commands/help/help_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      228 2023-04-14 00:53:18.000000 fgn-2023.7.21/src/fgn/core/commands/help/help_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)     3063 2023-04-17 02:37:56.000000 fgn-2023.7.21/src/fgn/core/commands/help/help_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-13 20:52:14.000000 fgn-2023.7.21/src/fgn/core/commands/help/help_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)    10220 2023-06-26 18:00:16.000000 fgn-2023.7.21/src/fgn/core/commands/help/help_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-13 20:52:14.000000 fgn-2023.7.21/src/fgn/core/commands/help/help_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.829717 fgn-2023.7.21/src/fgn/core/commands/howto/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 00:38:05.000000 fgn-2023.7.21/src/fgn/core/commands/howto/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      585 2023-05-10 21:54:04.000000 fgn-2023.7.21/src/fgn/core/commands/howto/howto_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      268 2023-04-12 00:38:05.000000 fgn-2023.7.21/src/fgn/core/commands/howto/howto_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 00:38:05.000000 fgn-2023.7.21/src/fgn/core/commands/howto/howto_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 00:38:05.000000 fgn-2023.7.21/src/fgn/core/commands/howto/howto_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     3781 2023-06-13 17:15:14.000000 fgn-2023.7.21/src/fgn/core/commands/howto/howto_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-12 00:38:05.000000 fgn-2023.7.21/src/fgn/core/commands/howto/howto_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.830578 fgn-2023.7.21/src/fgn/core/commands/lts/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 00:07:58.000000 fgn-2023.7.21/src/fgn/core/commands/lts/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      477 2023-04-29 20:31:50.000000 fgn-2023.7.21/src/fgn/core/commands/lts/lts_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      256 2023-04-19 00:07:58.000000 fgn-2023.7.21/src/fgn/core/commands/lts/lts_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 00:07:58.000000 fgn-2023.7.21/src/fgn/core/commands/lts/lts_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 00:07:58.000000 fgn-2023.7.21/src/fgn/core/commands/lts/lts_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1657 2023-04-19 00:16:44.000000 fgn-2023.7.21/src/fgn/core/commands/lts/lts_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 00:07:58.000000 fgn-2023.7.21/src/fgn/core/commands/lts/lts_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.831369 fgn-2023.7.21/src/fgn/core/commands/nano/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-13 20:15:56.000000 fgn-2023.7.21/src/fgn/core/commands/nano/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      407 2023-04-14 03:36:47.000000 fgn-2023.7.21/src/fgn/core/commands/nano/nano_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      262 2023-04-13 20:15:56.000000 fgn-2023.7.21/src/fgn/core/commands/nano/nano_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)      529 2023-04-13 20:45:30.000000 fgn-2023.7.21/src/fgn/core/commands/nano/nano_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-13 20:15:56.000000 fgn-2023.7.21/src/fgn/core/commands/nano/nano_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     2022 2023-07-01 06:04:22.000000 fgn-2023.7.21/src/fgn/core/commands/nano/nano_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-13 20:15:56.000000 fgn-2023.7.21/src/fgn/core/commands/nano/nano_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.832064 fgn-2023.7.21/src/fgn/core/commands/plan/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-24 17:00:38.000000 fgn-2023.7.21/src/fgn/core/commands/plan/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      406 2023-04-19 21:13:19.000000 fgn-2023.7.21/src/fgn/core/commands/plan/plan_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      259 2023-03-28 22:04:20.000000 fgn-2023.7.21/src/fgn/core/commands/plan/plan_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-24 23:39:15.000000 fgn-2023.7.21/src/fgn/core/commands/plan/plan_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-24 15:13:22.000000 fgn-2023.7.21/src/fgn/core/commands/plan/plan_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     4708 2023-04-19 21:30:40.000000 fgn-2023.7.21/src/fgn/core/commands/plan/plan_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)      440 2023-04-12 01:04:03.000000 fgn-2023.7.21/src/fgn/core/commands/plan/plan_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.832732 fgn-2023.7.21/src/fgn/core/commands/prompt/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-24 17:00:38.000000 fgn-2023.7.21/src/fgn/core/commands/prompt/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      482 2023-05-01 02:54:17.000000 fgn-2023.7.21/src/fgn/core/commands/prompt/prompt_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      257 2023-03-27 16:12:16.000000 fgn-2023.7.21/src/fgn/core/commands/prompt/prompt_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-19 20:57:09.000000 fgn-2023.7.21/src/fgn/core/commands/prompt/prompt_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     3738 2023-04-19 21:00:08.000000 fgn-2023.7.21/src/fgn/core/commands/prompt/prompt_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1691 2023-04-13 23:44:53.000000 fgn-2023.7.21/src/fgn/core/commands/prompt/prompt_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.833493 fgn-2023.7.21/src/fgn/core/commands/shell/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-28 23:04:20.000000 fgn-2023.7.21/src/fgn/core/commands/shell/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1369 2023-04-29 21:38:36.000000 fgn-2023.7.21/src/fgn/core/commands/shell/shell_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      268 2023-03-28 23:04:20.000000 fgn-2023.7.21/src/fgn/core/commands/shell/shell_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-28 23:04:20.000000 fgn-2023.7.21/src/fgn/core/commands/shell/shell_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-28 23:04:20.000000 fgn-2023.7.21/src/fgn/core/commands/shell/shell_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)      535 2023-06-26 17:56:46.000000 fgn-2023.7.21/src/fgn/core/commands/shell/shell_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-28 23:04:20.000000 fgn-2023.7.21/src/fgn/core/commands/shell/shell_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.834375 fgn-2023.7.21/src/fgn/core/commands/summary/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 00:08:40.000000 fgn-2023.7.21/src/fgn/core/commands/summary/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      402 2023-07-22 00:14:45.000000 fgn-2023.7.21/src/fgn/core/commands/summary/summary_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      280 2023-04-14 00:08:40.000000 fgn-2023.7.21/src/fgn/core/commands/summary/summary_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 00:08:40.000000 fgn-2023.7.21/src/fgn/core/commands/summary/summary_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 00:08:40.000000 fgn-2023.7.21/src/fgn/core/commands/summary/summary_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     2674 2023-04-20 19:37:14.000000 fgn-2023.7.21/src/fgn/core/commands/summary/summary_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-14 00:08:40.000000 fgn-2023.7.21/src/fgn/core/commands/summary/summary_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.834956 fgn-2023.7.21/src/fgn/core/commands/template/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-24 17:00:38.000000 fgn-2023.7.21/src/fgn/core/commands/template/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     2038 2023-04-30 00:43:45.000000 fgn-2023.7.21/src/fgn/core/commands/template/template_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      259 2023-03-28 22:28:18.000000 fgn-2023.7.21/src/fgn/core/commands/template/template_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-28 22:28:18.000000 fgn-2023.7.21/src/fgn/core/commands/template/template_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-28 22:28:18.000000 fgn-2023.7.21/src/fgn/core/commands/template/template_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)      435 2023-03-28 22:28:18.000000 fgn-2023.7.21/src/fgn/core/commands/template/template_template.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.835873 fgn-2023.7.21/src/fgn/core/commands/yaml/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-20 20:56:12.000000 fgn-2023.7.21/src/fgn/core/commands/yaml/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     3116 2023-04-21 01:44:04.000000 fgn-2023.7.21/src/fgn/core/commands/yaml/product-information-schema.yaml
+-rw-r--r--   0 candacechatman   (501) staff       (20)      408 2023-04-30 02:01:51.000000 fgn-2023.7.21/src/fgn/core/commands/yaml/yaml_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      262 2023-04-20 20:56:12.000000 fgn-2023.7.21/src/fgn/core/commands/yaml/yaml_config.yml
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-20 20:56:12.000000 fgn-2023.7.21/src/fgn/core/commands/yaml/yaml_example.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-20 20:56:12.000000 fgn-2023.7.21/src/fgn/core/commands/yaml/yaml_history.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)      879 2023-04-21 01:54:46.000000 fgn-2023.7.21/src/fgn/core/commands/yaml/yaml_system_prompt.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-20 20:56:12.000000 fgn-2023.7.21/src/fgn/core/commands/yaml/yaml_template.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)     2635 2023-05-01 02:30:56.000000 fgn-2023.7.21/src/fgn/core/core_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1607 2023-05-21 21:11:46.000000 fgn-2023.7.21/src/fgn/core/default_sub_cmd.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     3762 2023-04-13 23:44:53.000000 fgn-2023.7.21/src/fgn/core/dsl_parser.py
+-rwxr-xr-x   0 candacechatman   (501) staff       (20)     4277 2023-07-21 22:01:54.000000 fgn-2023.7.21/src/fgn/core/fgn_cli.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.836065 fgn-2023.7.21/src/fgn/models/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-04-06 19:32:18.000000 fgn-2023.7.21/src/fgn/models/__init__.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.836467 fgn-2023.7.21/src/fgn/models/dsl/
+-rw-r--r--   0 candacechatman   (501) staff       (20)      270 2023-04-08 04:05:38.000000 fgn-2023.7.21/src/fgn/models/dsl/fgn_dsl_schema.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      355 2023-04-08 04:05:52.000000 fgn-2023.7.21/src/fgn/models/dsl/step.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      242 2023-04-08 04:18:36.000000 fgn-2023.7.21/src/fgn/models/dsl/task.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      373 2023-03-23 03:55:38.000000 fgn-2023.7.21/src/fgn/models/message.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     4192 2023-07-21 16:52:47.000000 fgn-2023.7.21/src/fgn/skeleton.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.837532 fgn-2023.7.21/src/fgn/utils/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-03-30 20:42:36.000000 fgn-2023.7.21/src/fgn/utils/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     3254 2023-04-29 21:10:53.000000 fgn-2023.7.21/src/fgn/utils/chat_agent_configuration.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      227 2023-03-31 00:51:25.000000 fgn-2023.7.21/src/fgn/utils/clipboard.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     3336 2023-07-21 22:05:11.000000 fgn-2023.7.21/src/fgn/utils/file_operations.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     5655 2023-07-21 21:38:30.000000 fgn-2023.7.21/src/fgn/utils/openai_operations.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1820 2023-07-21 21:49:15.000000 fgn-2023.7.21/src/fgn/utils/output_manager.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.819243 fgn-2023.7.21/src/fgn.egg-info/
+-rw-r--r--   0 candacechatman   (501) staff       (20)     7038 2023-07-22 00:39:58.000000 fgn-2023.7.21/src/fgn.egg-info/PKG-INFO
+-rw-r--r--   0 candacechatman   (501) staff       (20)     7078 2023-07-22 00:39:58.000000 fgn-2023.7.21/src/fgn.egg-info/SOURCES.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        1 2023-07-22 00:39:58.000000 fgn-2023.7.21/src/fgn.egg-info/dependency_links.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)       45 2023-07-22 00:39:58.000000 fgn-2023.7.21/src/fgn.egg-info/entry_points.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        1 2023-07-21 16:56:59.000000 fgn-2023.7.21/src/fgn.egg-info/not-zip-safe
+-rw-r--r--   0 candacechatman   (501) staff       (20)      206 2023-07-22 00:39:58.000000 fgn-2023.7.21/src/fgn.egg-info/requires.txt
+-rw-r--r--   0 candacechatman   (501) staff       (20)        4 2023-07-22 00:39:58.000000 fgn-2023.7.21/src/fgn.egg-info/top_level.txt
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.838237 fgn-2023.7.21/tests/
+-rw-r--r--   0 candacechatman   (501) staff       (20)        0 2023-07-21 20:21:09.000000 fgn-2023.7.21/tests/__init__.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      271 2023-07-21 20:59:55.000000 fgn-2023.7.21/tests/conftest.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      855 2023-07-21 18:47:03.000000 fgn-2023.7.21/tests/test_cli.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)      599 2023-07-21 17:15:32.000000 fgn-2023.7.21/tests/test_skeleton.py
+drwxr-xr-x   0 candacechatman   (501) staff       (20)        0 2023-07-22 00:39:58.838971 fgn-2023.7.21/tests/utils/
+-rw-r--r--   0 candacechatman   (501) staff       (20)     1852 2023-07-21 21:40:26.000000 fgn-2023.7.21/tests/utils/test_file_operations.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     3737 2023-07-21 21:48:33.000000 fgn-2023.7.21/tests/utils/test_openai_operations.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     2750 2023-07-21 21:52:30.000000 fgn-2023.7.21/tests/utils/test_output_manager.py
+-rw-r--r--   0 candacechatman   (501) staff       (20)     2926 2023-07-21 20:26:23.000000 fgn-2023.7.21/tox.ini
```

### Comparing `fgn-0.0.0/.coveragerc` & `fgn-2023.7.21/.coveragerc`

 * *Files identical despite different names*

### Comparing `fgn-0.0.0/.github/workflows/ci.yml` & `fgn-2023.7.21/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fgn-0.0.0/.gitignore` & `fgn-2023.7.21/.gitignore`

 * *Files identical despite different names*

### Comparing `fgn-0.0.0/.pre-commit-config.yaml` & `fgn-2023.7.21/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fgn-0.0.0/.readthedocs.yml` & `fgn-2023.7.21/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `fgn-0.0.0/CONTRIBUTING.rst` & `fgn-2023.7.21/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `fgn-0.0.0/LICENSE.txt` & `fgn-2023.7.21/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fgn-0.0.0/docs/Makefile` & `fgn-2023.7.21/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fgn-0.0.0/docs/conf.py` & `fgn-2023.7.21/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fgn-0.0.0/docs/index.rst` & `fgn-2023.7.21/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fgn-0.0.0/setup.cfg` & `fgn-2023.7.21/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fgn
-description = Add a short description here!
+description = FGN: An AI-powered command-line tool for automated file generation.
 author = Sean Chatman
 author_email = info@chatmangpt.com
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/seanchatmangpt/fgn
@@ -21,29 +21,42 @@
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.11"
 	click
 	pyfakefs
+	rich
+	openai
+	watchdog
+	pyperclip
+	PyGithub
+	pytest
+	PyYAML
+	distro
+	markdown2
+	lxml
+	requests
+	openai
+	pytest-mock
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
 testing = 
 	setuptools
 	pytest
 	pytest-cov
 
 [options.entry_points]
 console_scripts = 
-	fgn = fgn.cli:main
+	fgn = fgn.core.fgn_cli:fgn
 
 [tool:pytest]
 addopts = 
 	--cov fgn --cov-report term-missing
 	--verbose
 norecursedirs = 
 	dist
```

### Comparing `fgn-0.0.0/setup.py` & `fgn-2023.7.21/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,15 +6,16 @@
     PyScaffold helps you to put up the scaffold of your new Python project.
     Learn more under: https://pyscaffold.org/
 """
 from setuptools import setup
 
 if __name__ == "__main__":
     try:
-        setup(use_scm_version={"version_scheme": "no-guess-dev"})
+        version = "2023.7.21"
+        setup(version=version)
     except:  # noqa
         print(
             "\n\nAn error occurred while building the project, "
             "please ensure you have the most updated version of setuptools, "
             "setuptools_scm and wheel with:\n"
             "   pip install -U setuptools setuptools_scm wheel\n\n"
         )
```

### Comparing `fgn-0.0.0/src/fgn/__init__.py` & `fgn-2023.7.21/src/fgn/__init__.py`

 * *Files identical despite different names*

### Comparing `fgn-0.0.0/src/fgn/skeleton.py` & `fgn-2023.7.21/src/fgn/skeleton.py`

 * *Files identical despite different names*

### Comparing `fgn-0.0.0/tests/test_cli.py` & `fgn-2023.7.21/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `fgn-0.0.0/tests/test_skeleton.py` & `fgn-2023.7.21/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `fgn-0.0.0/tox.ini` & `fgn-2023.7.21/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 isolated_build = True
 
 
 [testenv]
 description = Invoke pytest to run automated tests
 setenv =
     TOXINIDIR = {toxinidir}
+    OPENAI_API_KEY = "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"
 passenv =
     HOME
     SETUPTOOLS_*
 extras =
     testing
 commands =
     pytest {posargs}
```

