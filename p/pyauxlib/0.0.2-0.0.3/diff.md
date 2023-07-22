# Comparing `tmp/pyauxlib-0.0.2.tar.gz` & `tmp/pyauxlib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyauxlib-0.0.2.tar", last modified: Fri Jun 30 03:59:28 2023, max compression
+gzip compressed data, was "pyauxlib-0.0.3.tar", last modified: Sat Jul 22 13:55:20 2023, max compression
```

## Comparing `pyauxlib-0.0.2.tar` & `pyauxlib-0.0.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/.cookiecutterrc
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.138184 pyauxlib-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.142184 pyauxlib-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/.github/workflows/github-actions.yml
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.142184 pyauxlib-0.0.2/ci/
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/ci/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/ci/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.138184 pyauxlib-0.0.2/ci/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.138184 pyauxlib-0.0.2/ci/templates/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.142184 pyauxlib-0.0.2/ci/templates/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.142184 pyauxlib-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.142184 pyauxlib-0.0.2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/reference/pyauxlib.rst
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.138184 pyauxlib-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.142184 pyauxlib-0.0.2/src/pyauxlib/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/src/pyauxlib/callables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/callables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/callables/callables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/src/pyauxlib/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/decorators/timing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/src/pyauxlib/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/experimental/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/experimental/get_caller_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/experimental/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/experimental/lists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/src/pyauxlib/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/io/filesfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/io/yamlio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/src/pyauxlib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/utils/deprecations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/utils/dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/src/pyauxlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-30 03:59:28.000000 pyauxlib-0.0.2/src/pyauxlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-30 03:59:28.000000 pyauxlib-0.0.2/src/pyauxlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 03:59:28.000000 pyauxlib-0.0.2/src/pyauxlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 03:59:27.000000 pyauxlib-0.0.2/src/pyauxlib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 03:59:28.000000 pyauxlib-0.0.2/src/pyauxlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 03:59:28.000000 pyauxlib-0.0.2/src/pyauxlib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/tests/test_pyauxlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:20.432047 pyauxlib-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/.cookiecutterrc
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:20.416046 pyauxlib-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:20.424046 pyauxlib-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/.github/workflows/github-actions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-22 13:55:20.432047 pyauxlib-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:20.424046 pyauxlib-0.0.3/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/ci/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/ci/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:20.416046 pyauxlib-0.0.3/ci/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:20.416046 pyauxlib-0.0.3/ci/templates/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:20.424046 pyauxlib-0.0.3/ci/templates/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:20.424046 pyauxlib-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:20.424046 pyauxlib-0.0.3/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/docs/reference/pyauxlib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 13:55:20.432047 pyauxlib-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:20.420046 pyauxlib-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:20.424046 pyauxlib-0.0.3/src/pyauxlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:20.428046 pyauxlib-0.0.3/src/pyauxlib/callables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/callables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/callables/callables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:20.428046 pyauxlib-0.0.3/src/pyauxlib/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/decorators/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:20.428046 pyauxlib-0.0.3/src/pyauxlib/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/experimental/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/experimental/get_caller_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/experimental/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/experimental/lists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:20.428046 pyauxlib-0.0.3/src/pyauxlib/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/io/filesfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/io/yamlio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:20.432047 pyauxlib-0.0.3/src/pyauxlib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/utils/deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/utils/dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/src/pyauxlib/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:20.428046 pyauxlib-0.0.3/src/pyauxlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-22 13:55:20.000000 pyauxlib-0.0.3/src/pyauxlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-22 13:55:20.000000 pyauxlib-0.0.3/src/pyauxlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 13:55:20.000000 pyauxlib-0.0.3/src/pyauxlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 13:55:20.000000 pyauxlib-0.0.3/src/pyauxlib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-22 13:55:20.000000 pyauxlib-0.0.3/src/pyauxlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 13:55:20.000000 pyauxlib-0.0.3/src/pyauxlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:55:20.432047 pyauxlib-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/tests/test_pyauxlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-22 13:55:05.000000 pyauxlib-0.0.3/tox.ini
```

### Comparing `pyauxlib-0.0.2/.bumpversion.cfg` & `pyauxlib-0.0.3/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.0.2
+current_version = 0.0.3
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `pyauxlib-0.0.2/.cookiecutterrc` & `pyauxlib-0.0.3/.cookiecutterrc`

 * *Files 0% similar despite different names*

```diff
@@ -50,12 +50,12 @@
     scrutinizer: "no"
     setup_py_uses_setuptools_scm: "no"
     sphinx_docs: "yes"
     sphinx_docs_hosting: "https://pyauxlib.readthedocs.io/"
     sphinx_doctest: "no"
     sphinx_theme: "sphinx-rtd-theme"
     test_matrix_separate_coverage: "no"
-    version: 0.0.2
+    version: 0.0.3
     version_manager: "bump2version"
     website: "https://github.com/psolsfer"
     year_from: "2023"
     year_to: "2023"
```

### Comparing `pyauxlib-0.0.2/.github/workflows/github-actions.yml` & `pyauxlib-0.0.3/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.2/.pre-commit-config.yaml` & `pyauxlib-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.2/CONTRIBUTING.rst` & `pyauxlib-0.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.2/LICENSE` & `pyauxlib-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.2/PKG-INFO` & `pyauxlib-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyauxlib
-Version: 0.0.2
+Version: 0.0.3
 Summary: Auxiliary library for python.
 Home-page: https://github.com/psolsfer/pyauxlib
 Author: Pablo Solís Fernández
 Author-email: pablosolisfernandez@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://pyauxlib.readthedocs.io/
 Project-URL: Changelog, https://pyauxlib.readthedocs.io/en/latest/changelog.html
```

### Comparing `pyauxlib-0.0.2/README.rst` & `pyauxlib-0.0.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/pyauxlib
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/pyauxlib.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/pyauxlib
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/psolsfer/pyauxlib/v0.0.2.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/psolsfer/pyauxlib/v0.0.3.svg
     :alt: Commits since latest release
-    :target: https://github.com/psolsfer/pyauxlib/compare/v0.0.2...main
+    :target: https://github.com/psolsfer/pyauxlib/compare/v0.0.3...main
 
 
 
 .. end-badges
 
 Auxiliary library for python.
```

### Comparing `pyauxlib-0.0.2/ci/bootstrap.py` & `pyauxlib-0.0.3/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.2/ci/templates/.github/workflows/github-actions.yml` & `pyauxlib-0.0.3/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.2/docs/conf.py` & `pyauxlib-0.0.3/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "PyAuxLib"
 year = "2023"
 author = "Pablo Solís Fernández"
 copyright = f"{year}, {author}"
-version = release = "0.0.2"
+version = release = "0.0.3"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/psolsfer/pyauxlib/issues/%s", "#"),
     "pr": ("https://github.com/psolsfer/pyauxlib/pull/%s", "PR #"),
 }
```

### Comparing `pyauxlib-0.0.2/pyproject.toml` & `pyauxlib-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,12 +42,12 @@
 
 [tool.ruff.flake8-pytest-style]
 fixture-parentheses = false
 mark-parentheses = false
 
 [tool.ruff.isort]
 forced-separate = ["conftest"]
-force-single-line = true
+force-single-line = false
 
 [tool.black]
 line-length = 140
 target-version = ["py310"]
```

### Comparing `pyauxlib-0.0.2/pytest.ini` & `pyauxlib-0.0.3/pytest.ini`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.2/setup.py` & `pyauxlib-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 #!/usr/bin/env python
 import re
 from pathlib import Path
 
-from setuptools import find_packages
-from setuptools import setup
+from setuptools import find_packages, setup
 
 
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 requirements = ["deprecated", "wrapt"]
 test_requirements = [
     "pytest>=3",
 ]
 
 setup(
     name="pyauxlib",
-    version="0.0.2",
+    version="0.0.3",
     license="BSD-3-Clause",
     description="Auxiliary library for python.",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
     author="Pablo Solís Fernández",
     author_email="pablosolisfernandez@gmail.com",
     url="https://github.com/psolsfer/pyauxlib",
     packages=find_packages("src"),
+    package_data={"pyauxlib": ["py.typed"]},
     package_dir={"": "src"},
     py_modules=[path.stem for path in Path("src").glob("*.py")],
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
         "Development Status :: 2 - Pre-Alpha",
```

### Comparing `pyauxlib-0.0.2/src/pyauxlib/callables/callables.py` & `pyauxlib-0.0.3/src/pyauxlib/callables/callables.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.2/src/pyauxlib/experimental/decorator.py` & `pyauxlib-0.0.3/src/pyauxlib/experimental/decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import functools
 import inspect
 import warnings
+from collections.abc import Callable
+from typing import Any
 
 import wrapt
 from deprecated.classic import ClassicAdapter
 
 _routine_stacklevel = 2
 string_types = (bytes, str)
 
 
 # TODO: see also how they handle the deprecated decorator in sklearn:
 # sklearn.utils.deprecation
-def experimental(*args, **kwargs):
+def experimental(*args: Any, **kwargs: Any) -> functools.partial[Callable[..., Any]]:
     # REFERENCE: "adapted" from deprecated method of deprecated library
     # TODO: probably a simpler decorator can be used, w/o ClassicAdapted, ...
     """
     This is a decorator which can be used to mark functions
     as experimental. It will result in a warning being emitted
     when the function is used.
```

### Comparing `pyauxlib-0.0.2/src/pyauxlib/experimental/get_caller_path.py` & `pyauxlib-0.0.3/src/pyauxlib/experimental/get_caller_path.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from inspect import currentframe
-from inspect import getframeinfo
+from inspect import currentframe, getframeinfo
 from pathlib import Path
 from types import FrameType
 
 
 def get_caller_path() -> Path | None:
     # FIXME: Does this work as intended? Is it useful?
     """Gets the path of the caller script.
```

### Comparing `pyauxlib-0.0.2/src/pyauxlib/experimental/kwargs.py` & `pyauxlib-0.0.3/src/pyauxlib/experimental/kwargs.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.2/src/pyauxlib/experimental/lists.py` & `pyauxlib-0.0.3/src/pyauxlib/experimental/lists.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Any
+
 from pyauxlib.experimental.decorator import experimental
 
 
 @experimental
 def list_elements_to_numeric(lst: list) -> list:
     """Converts to numeric values all the possible elements of a list.
     First try to convert to int, and then to float. Elements that cannot be converted
@@ -21,15 +23,15 @@
     for ele in lst:
         new_list.append(is_number(ele))
 
     return new_list
 
 
 @experimental
-def is_number(ele):
+def is_number(ele: Any) -> int | float | Any:
     """Returns an object converted to int. If it cannot be converted to int, it will
     try to convert to float.
 
     Parameters
     ----------
     ele : _type_
         object
@@ -41,15 +43,15 @@
     try:
         return int(ele)
     except ValueError:
         return is_float(ele)
 
 
 @experimental
-def is_float(ele):
+def is_float(ele: Any) -> float | Any:
     """Returns an object converted to float, or the original object if it cannot be
     converted
 
     Parameters
     ----------
     ele : _type_
         original object
```

### Comparing `pyauxlib-0.0.2/src/pyauxlib/io/filesfolders.py` & `pyauxlib-0.0.3/src/pyauxlib/io/filesfolders.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.2/src/pyauxlib/io/yamlio.py` & `pyauxlib-0.0.3/src/pyauxlib/io/yamlio.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.2/src/pyauxlib/utils/deprecations.py` & `pyauxlib-0.0.3/src/pyauxlib/utils/deprecations.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     # Warns of a deprecated argument.
     # To be called from within the method, when the deprecated argument is being used
     # method : method name
     # argument: argument to be deprecated
     # version: in which will be removed
     # additional_msg: e.g. "Use 'other_arg' instead"
     # TODO: PROBABLY it can be improved quite a lot...
-    # TODO: Is it possible to convert it in a decorator?
+    # TODO: Is it possible to convert it to a decorator?
 
     if not any([method, argument, version]):
         msg = "Used argument from method"
     if method:
         method = f"from method '{method}' "
     if argument:
         argument = f"'{argument}' "
```

### Comparing `pyauxlib-0.0.2/src/pyauxlib/utils/dictionaries.py` & `pyauxlib-0.0.3/src/pyauxlib/utils/dictionaries.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.2/src/pyauxlib/utils/encoding.py` & `pyauxlib-0.0.3/src/pyauxlib/utils/encoding.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,9 @@
 import logging
-from codecs import BOM_UTF8
-from codecs import BOM_UTF16
-from codecs import BOM_UTF16_BE
-from codecs import BOM_UTF16_LE
-from codecs import BOM_UTF32
-from codecs import BOM_UTF32_BE
-from codecs import BOM_UTF32_LE
+from codecs import BOM_UTF8, BOM_UTF16, BOM_UTF16_BE, BOM_UTF16_LE, BOM_UTF32, BOM_UTF32_BE, BOM_UTF32_LE
 from pathlib import Path
 
 try:
     import chardet
 except ImportError:
     chardet = None
 
@@ -35,15 +29,15 @@
         BOM_UTF16: "utf_16",
         BOM_UTF16_BE: "utf_16_be",
         BOM_UTF16_LE: "utf_16_le",
         BOM_UTF32: "utf_32",
         BOM_UTF32_BE: "utf_32_be",
         BOM_UTF32_LE: "utf_32_le",
     }
-
+    file = Path(file) if isinstance(file, str) else file
     try:
         with Path.open(file, "rb") as f:
             # Reads the first 5 bytes
             beginning = f.read(5)
 
             if beginning[0:2] in codecs:
                 encoding = codecs[beginning[0:2]]
@@ -53,31 +47,29 @@
                 encoding = codecs[beginning[0:4]]
             elif beginning[0:5] in codecs:
                 encoding = codecs[beginning[0:5]]
             else:
                 encoding = "utf-8"
             return encoding
     except FileNotFoundError as err:
-        # TODO: how to use the logger in a module???
-        print(f"Error loading file: {file}")
-        print(err)
+        logger.warning(f"Error {err} loading file: {file}")
         return None
 
 
 def detect_encoding_chardet(file: str | Path) -> str | None:
     """Detects the encoding of the file using the chardet library. This library uses
     heuristics to make an educated guess about the encoding of a file. However, this
     method is not always accurate and may be slow for large files.
     Use in cases where `detect_encoding` fails."""
+    file = Path(file) if isinstance(file, str) else file
     try:
         with Path.open(file, "rb") as f:
             raw_data = f.read()
             result = chardet.detect(raw_data)
             encoding = result["encoding"]
             return encoding
     except AttributeError:
         logger.warning("Install package 'chardet' for additional encoding detection.")
         return None
     except FileNotFoundError as err:
-        print(f"Error loading file: {file}")
-        print(err)
+        logger.warning(f"Error {err} loading file: {file}")
         return None
```

### Comparing `pyauxlib-0.0.2/src/pyauxlib/utils/logger.py` & `pyauxlib-0.0.3/src/pyauxlib/utils/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,18 +21,17 @@
     The level as an int
     """
 
     if level is None:
         return _set_level(default_level)
 
     if isinstance(level, str):
-        level: int = logging.getLevelName(level.upper())
+        return logging.getLevelName(level.upper())
     elif not isinstance(level, int):
-        level = logging.INFO
-
+        return logging.INFO
     return level
 
 
 def init_logger(
     name: str,
     level: int | str = "INFO",
     level_console: int | str | None = None,
```

### Comparing `pyauxlib-0.0.2/src/pyauxlib/utils/timer.py` & `pyauxlib-0.0.3/src/pyauxlib/utils/timer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import csv
 import logging
 import time
 import warnings
 from pathlib import Path
+from typing import Any
 
 
 class Timer:
     """Timer class to measure execution times.
 
     The timer can be managed manually, calling the start, stop,... methods.
     It can also be used as a context manager:
@@ -55,15 +56,15 @@
         self.reset()
 
     def __enter__(self):
         """Start a new timer as a context manager"""
         self.start()
         return self
 
-    def __exit__(self, *exc_info):
+    def __exit__(self, *exc_info: Any):
         """Stop the context manager timer"""
         self.stop()
 
     def start(self):
         """Starts the timer."""
         if self.stop_time is not None:
             self.logger("Timer has not been resetted.")
```

### Comparing `pyauxlib-0.0.2/src/pyauxlib.egg-info/PKG-INFO` & `pyauxlib-0.0.3/src/pyauxlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyauxlib
-Version: 0.0.2
+Version: 0.0.3
 Summary: Auxiliary library for python.
 Home-page: https://github.com/psolsfer/pyauxlib
 Author: Pablo Solís Fernández
 Author-email: pablosolisfernandez@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://pyauxlib.readthedocs.io/
 Project-URL: Changelog, https://pyauxlib.readthedocs.io/en/latest/changelog.html
```

### Comparing `pyauxlib-0.0.2/src/pyauxlib.egg-info/SOURCES.txt` & `pyauxlib-0.0.3/src/pyauxlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.2/tests/test_pyauxlib.py` & `pyauxlib-0.0.3/tests/test_pyauxlib.py`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.2/tox.ini` & `pyauxlib-0.0.3/tox.ini`

 * *Files identical despite different names*

