# Comparing `tmp/git_aggregator-3.0.1.tar.gz` & `tmp/git_aggregator-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_aggregator-3.0.1.tar", last modified: Wed Sep 21 12:40:43 2022, max compression
+gzip compressed data, was "git_aggregator-4.0.tar", last modified: Sat Jul 22 11:19:47 2023, max compression
```

## Comparing `git_aggregator-3.0.1.tar` & `git_aggregator-4.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 12:40:43.831548 git_aggregator-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 12:40:43.827548 git_aggregator-3.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 12:40:43.831548 git_aggregator-3.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      751 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/DEVELOP.rst
--rw-r--r--   0 runner    (1001) docker     (121)    34520 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10886 2022-09-21 12:40:43.831548 git_aggregator-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9971 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 12:40:43.831548 git_aggregator-3.0.1/git_aggregator/
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/git_aggregator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/git_aggregator/_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     6663 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/git_aggregator/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/git_aggregator/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     3302 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/git_aggregator/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     7752 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/git_aggregator/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    16428 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/git_aggregator/repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/git_aggregator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 12:40:43.831548 git_aggregator-3.0.1/git_aggregator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10886 2022-09-21 12:40:43.000000 git_aggregator-3.0.1/git_aggregator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-09-21 12:40:43.000000 git_aggregator-3.0.1/git_aggregator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 12:40:43.000000 git_aggregator-3.0.1/git_aggregator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-21 12:40:43.000000 git_aggregator-3.0.1/git_aggregator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-21 12:40:43.000000 git_aggregator-3.0.1/git_aggregator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-21 12:40:43.000000 git_aggregator-3.0.1/git_aggregator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 12:40:43.831548 git_aggregator-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1499 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 12:40:43.831548 git_aggregator-3.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14429 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (121)    13024 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/tests/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-09-21 12:40:34.000000 git_aggregator-3.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:19:47.801873 git_aggregator-4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-22 11:19:37.000000 git_aggregator-4.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:19:47.797873 git_aggregator-4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:19:47.797873 git_aggregator-4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-22 11:19:37.000000 git_aggregator-4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-22 11:19:37.000000 git_aggregator-4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-22 11:19:37.000000 git_aggregator-4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-22 11:19:37.000000 git_aggregator-4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-22 11:19:37.000000 git_aggregator-4.0/DEVELOP.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-07-22 11:19:37.000000 git_aggregator-4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-22 11:19:37.000000 git_aggregator-4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-07-22 11:19:47.801873 git_aggregator-4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-07-22 11:19:37.000000 git_aggregator-4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:19:47.801873 git_aggregator-4.0/git_aggregator/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-22 11:19:37.000000 git_aggregator-4.0/git_aggregator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-22 11:19:37.000000 git_aggregator-4.0/git_aggregator/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-07-22 11:19:37.000000 git_aggregator-4.0/git_aggregator/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-22 11:19:37.000000 git_aggregator-4.0/git_aggregator/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-22 11:19:37.000000 git_aggregator-4.0/git_aggregator/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-22 11:19:37.000000 git_aggregator-4.0/git_aggregator/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16436 2023-07-22 11:19:37.000000 git_aggregator-4.0/git_aggregator/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-22 11:19:37.000000 git_aggregator-4.0/git_aggregator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:19:47.801873 git_aggregator-4.0/git_aggregator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-07-22 11:19:47.000000 git_aggregator-4.0/git_aggregator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-22 11:19:47.000000 git_aggregator-4.0/git_aggregator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 11:19:47.000000 git_aggregator-4.0/git_aggregator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-22 11:19:47.000000 git_aggregator-4.0/git_aggregator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-22 11:19:47.000000 git_aggregator-4.0/git_aggregator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-22 11:19:47.000000 git_aggregator-4.0/git_aggregator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 11:19:47.801873 git_aggregator-4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-22 11:19:37.000000 git_aggregator-4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:19:47.801873 git_aggregator-4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-22 11:19:37.000000 git_aggregator-4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-07-22 11:19:37.000000 git_aggregator-4.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-22 11:19:37.000000 git_aggregator-4.0/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-07-22 11:19:37.000000 git_aggregator-4.0/tests/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-22 11:19:37.000000 git_aggregator-4.0/tox.ini
```

### Comparing `git_aggregator-3.0.1/.gitignore` & `git_aggregator-4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `git_aggregator-3.0.1/LICENSE` & `git_aggregator-4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git_aggregator-3.0.1/PKG-INFO` & `git_aggregator-4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: git_aggregator
-Version: 3.0.1
+Version: 4.0
 Summary: A program to aggregate git branches from different remotes into a consolidated one
 Home-page: http://github.com/acsone/git-aggregator
 Author: ACSONE SA/NV
 Author-email: info@acsone.eu
 License: AGPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Shells
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
 
 .. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. image:: https://github.com/acsone/git-aggregator/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/acsone/git-aggregator/actions/workflows/ci.yml
+.. image:: https://results.pre-commit.ci/badge/github/acsone/git-aggregator/master.svg
+   :target: https://results.pre-commit.ci/latest/github/acsone/git-aggregator/master
+   :alt: pre-commit.ci status
 .. image:: https://img.shields.io/pypi/pyversions/git-aggregator
 
 ==============
 git-aggregator
 ==============
 
 Manage the aggregation of git branches from different remotes to build a consolidated one.
@@ -240,14 +243,21 @@
    $ gitaggregate -c repos.yaml show-closed-prs
 
 .. _Github API token: https://github.com/settings/tokens
 
 Changes
 =======
 
+4.0 (2023-07-22)
+----------------
+
+* [BREAKING] drop support for other configuration file formats than yaml
+* Ensure git pull is always done in fast-forward mode
+* Drop support for python 3.6, test with python 3.11, stop testing with pypy
+
 3.0.1 (2022-09-21)
 ------------------
 
 * Fix git clone issue with git < 2.17
 
 3.0.0 (2022-09-20)
 ------------------
```

### Comparing `git_aggregator-3.0.1/README.rst` & `git_aggregator-4.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 .. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. image:: https://github.com/acsone/git-aggregator/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/acsone/git-aggregator/actions/workflows/ci.yml
+.. image:: https://results.pre-commit.ci/badge/github/acsone/git-aggregator/master.svg
+   :target: https://results.pre-commit.ci/latest/github/acsone/git-aggregator/master
+   :alt: pre-commit.ci status
 .. image:: https://img.shields.io/pypi/pyversions/git-aggregator
 
 ==============
 git-aggregator
 ==============
 
 Manage the aggregation of git branches from different remotes to build a consolidated one.
@@ -217,14 +220,21 @@
    $ gitaggregate -c repos.yaml show-closed-prs
 
 .. _Github API token: https://github.com/settings/tokens
 
 Changes
 =======
 
+4.0 (2023-07-22)
+----------------
+
+* [BREAKING] drop support for other configuration file formats than yaml
+* Ensure git pull is always done in fast-forward mode
+* Drop support for python 3.6, test with python 3.11, stop testing with pypy
+
 3.0.1 (2022-09-21)
 ------------------
 
 * Fix git clone issue with git < 2.17
 
 3.0.0 (2022-09-20)
 ------------------
```

### Comparing `git_aggregator-3.0.1/git_aggregator/_compat.py` & `git_aggregator-4.0/git_aggregator/_compat.py`

 * *Files identical despite different names*

### Comparing `git_aggregator-3.0.1/git_aggregator/config.py` & `git_aggregator-4.0/git_aggregator/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # © 2015 ACSONE SA/NV
 # License AGPLv3 (http://www.gnu.org/licenses/agpl-3.0-standalone.html)
 
 import logging
 import os
 from string import Template
 
-import kaptan
+import yaml
+
 from .exception import ConfigException
 from ._compat import string_types
 
 
 log = logging.getLogger(__name__)
 
 
@@ -144,15 +145,19 @@
     :returns: expanded config dict item
     :rtype: iter(dict)
     """
     if not os.path.exists(config):
         raise ConfigException('Unable to find configuration file: %s' % config)
 
     file_extension = os.path.splitext(config)[1][1:]
-    conf = kaptan.Kaptan(handler=kaptan.HANDLER_EXT.get(file_extension))
+    if file_extension not in ("yaml", "yml"):
+        raise ConfigException(
+            "Only .yaml and .yml configuration files are supported "
+            "(got %s)" % file_extension
+        )
 
     if expand_env:
         environment = {}
         if env_file is not None and os.path.isfile(env_file):
             with open(env_file) as env_file_handler:
                 for line in env_file_handler:
                     line = line.strip()
@@ -161,10 +166,13 @@
                     if '=' in line:
                         key, value = line.split('=')
                         environment.update({key.strip(): value.strip()})
         environment.update(os.environ)
         with open(config, 'r') as file_handler:
             config = Template(file_handler.read())
             config = config.substitute(environment)
+    else:
+        config = open(config, 'r').read()
+
+    conf = yaml.load(config, Loader=yaml.SafeLoader)
 
-    conf.import_config(config)
-    return get_repos(conf.export('dict') or {}, force)
+    return get_repos(conf or {}, force)
```

### Comparing `git_aggregator-3.0.1/git_aggregator/log.py` & `git_aggregator-4.0/git_aggregator/log.py`

 * *Files identical despite different names*

### Comparing `git_aggregator-3.0.1/git_aggregator/main.py` & `git_aggregator-4.0/git_aggregator/main.py`

 * *Files identical despite different names*

### Comparing `git_aggregator-3.0.1/git_aggregator/repo.py` & `git_aggregator-4.0/git_aggregator/repo.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,15 @@
     def _execute_shell_command_after(self):
         logger.info('Execute shell after commands')
         for cmd in self.shell_command_after:
             self.log_call(cmd, shell=True, cwd=self.cwd)
 
     def _merge(self, merge):
         logger.info("Pull %s, %s", merge["remote"], merge["ref"])
-        cmd = ("git", "pull", "--no-rebase")
+        cmd = ("git", "pull", "--ff", "--no-rebase")
         if self.git_version >= (1, 7, 10):
             # --edit and --no-edit appear with Git 1.7.10
             # see Documentation/RelNotes/1.7.10.txt of Git
             # (https://git.kernel.org/cgit/git/git.git/tree)
             cmd += ('--no-edit',)
         if logger.getEffectiveLevel() != logging.DEBUG:
             cmd += ('--quiet',)
```

### Comparing `git_aggregator-3.0.1/git_aggregator/utils.py` & `git_aggregator-4.0/git_aggregator/utils.py`

 * *Files identical despite different names*

### Comparing `git_aggregator-3.0.1/git_aggregator.egg-info/PKG-INFO` & `git_aggregator-4.0/git_aggregator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: git-aggregator
-Version: 3.0.1
+Version: 4.0
 Summary: A program to aggregate git branches from different remotes into a consolidated one
 Home-page: http://github.com/acsone/git-aggregator
 Author: ACSONE SA/NV
 Author-email: info@acsone.eu
 License: AGPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Shells
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
 
 .. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. image:: https://github.com/acsone/git-aggregator/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/acsone/git-aggregator/actions/workflows/ci.yml
+.. image:: https://results.pre-commit.ci/badge/github/acsone/git-aggregator/master.svg
+   :target: https://results.pre-commit.ci/latest/github/acsone/git-aggregator/master
+   :alt: pre-commit.ci status
 .. image:: https://img.shields.io/pypi/pyversions/git-aggregator
 
 ==============
 git-aggregator
 ==============
 
 Manage the aggregation of git branches from different remotes to build a consolidated one.
@@ -240,14 +243,21 @@
    $ gitaggregate -c repos.yaml show-closed-prs
 
 .. _Github API token: https://github.com/settings/tokens
 
 Changes
 =======
 
+4.0 (2023-07-22)
+----------------
+
+* [BREAKING] drop support for other configuration file formats than yaml
+* Ensure git pull is always done in fast-forward mode
+* Drop support for python 3.6, test with python 3.11, stop testing with pypy
+
 3.0.1 (2022-09-21)
 ------------------
 
 * Fix git clone issue with git < 2.17
 
 3.0.0 (2022-09-20)
 ------------------
```

### Comparing `git_aggregator-3.0.1/git_aggregator.egg-info/SOURCES.txt` & `git_aggregator-4.0/git_aggregator.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 DEVELOP.rst
 LICENSE
 MANIFEST.in
 README.rst
 setup.py
 tox.ini
 .github/workflows/ci.yml
+.github/workflows/release.yml
 git_aggregator/__init__.py
 git_aggregator/_compat.py
 git_aggregator/config.py
 git_aggregator/exception.py
 git_aggregator/log.py
 git_aggregator/main.py
 git_aggregator/repo.py
```

### Comparing `git_aggregator-3.0.1/setup.py` & `git_aggregator-4.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,36 +13,36 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: '
         'GNU Affero General Public License v3 or later (AGPLv3+)',
         'Operating System :: POSIX',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         "Topic :: Utilities",
         "Topic :: System :: Shells",
     ],
     license="AGPLv3+",
     author='ACSONE SA/NV',
     author_email='info@acsone.eu',
     url='http://github.com/acsone/git-aggregator',
     packages=[
         'git_aggregator',
     ],
     setup_requires=[
         'setuptools_scm',
     ],
     install_requires=[
-        'kaptan',
+        'PyYAML>=5',
         'argcomplete',
         'colorama',
         'requests',
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     entry_points=dict(
         console_scripts=['gitaggregate=git_aggregator.main:main']),
     test_suite='tests',
 )
```

### Comparing `git_aggregator-3.0.1/tests/test_config.py` & `git_aggregator-4.0/tests/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # -*- coding: utf-8 -*-
 # © 2015 ACSONE SA/NV
 # License AGPLv3 (http://www.gnu.org/licenses/agpl-3.0-standalone.html)
 import os
 import tempfile
 import unittest
-import kaptan
 from textwrap import dedent
 
+import yaml
+
 from git_aggregator import config
 from git_aggregator.exception import ConfigException
 from git_aggregator._compat import PY2
 
 
 class TestConfig(unittest.TestCase):
 
     def _parse_config(self, config_str):
-        conf = kaptan.Kaptan(handler='yaml')
-        conf.import_config(config_str)
-        return conf.export('dict')
+        return yaml.load(config_str, Loader=yaml.SafeLoader)
 
     def test_load(self):
         config_yaml = """
 /product_attribute:
     remotes:
         oca: https://github.com/OCA/product-attribute.git
         acsone: git+ssh://git@github.com/acsone/product-attribute.git
```

### Comparing `git_aggregator-3.0.1/tests/test_log.py` & `git_aggregator-4.0/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `git_aggregator-3.0.1/tests/test_repo.py` & `git_aggregator-4.0/tests/test_repo.py`

 * *Files identical despite different names*

