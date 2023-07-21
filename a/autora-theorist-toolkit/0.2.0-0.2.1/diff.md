# Comparing `tmp/autora-theorist-toolkit-0.2.0.tar.gz` & `tmp/autora-theorist-toolkit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-theorist-toolkit-0.2.0.tar", last modified: Fri Jul 21 18:46:24 2023, max compression
+gzip compressed data, was "autora-theorist-toolkit-0.2.1.tar", last modified: Fri Jul 21 22:43:59 2023, max compression
```

## Comparing `autora-theorist-toolkit-0.2.0.tar` & `autora-theorist-toolkit-0.2.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.142157 autora-theorist-toolkit-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.130157 autora-theorist-toolkit-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.130157 autora-theorist-toolkit-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.134157 autora-theorist-toolkit-0.2.0/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.idea/autora-theorist-toolkit.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.134157 autora-theorist-toolkit-0.2.0/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-21 18:46:24.142157 autora-theorist-toolkit-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.134157 autora-theorist-toolkit-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/docs/Additional Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.134157 autora-theorist-toolkit-0.2.0/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.134157 autora-theorist-toolkit-0.2.0/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 18:46:24.142157 autora-theorist-toolkit-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.134157 autora-theorist-toolkit-0.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.134157 autora-theorist-toolkit-0.2.0/src/autora/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.134157 autora-theorist-toolkit-0.2.0/src/autora/theorist/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.134157 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.138157 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/components/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/components/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.138157 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.142157 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/ddm_bms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/hybrid_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.142157 autora-theorist-toolkit-0.2.0/src/autora_theorist_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-21 18:46:24.000000 autora-theorist-toolkit-0.2.0/src/autora_theorist_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-21 18:46:24.000000 autora-theorist-toolkit-0.2.0/src/autora_theorist_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 18:46:24.000000 autora-theorist-toolkit-0.2.0/src/autora_theorist_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 18:46:24.000000 autora-theorist-toolkit-0.2.0/src/autora_theorist_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 18:46:24.000000 autora-theorist-toolkit-0.2.0/src/autora_theorist_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:24.142157 autora-theorist-toolkit-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/tests/test_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-21 18:46:11.000000 autora-theorist-toolkit-0.2.0/tests/test_visual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.517197 autora-theorist-toolkit-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.509197 autora-theorist-toolkit-0.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.509197 autora-theorist-toolkit-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.509197 autora-theorist-toolkit-0.2.1/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.idea/autora-theorist-toolkit.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.509197 autora-theorist-toolkit-0.2.1/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-21 22:43:59.517197 autora-theorist-toolkit-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/docs/Additional Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 22:43:59.517197 autora-theorist-toolkit-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/src/autora/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/src/autora/theorist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/components/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/components/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/ddm_bms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/hybrid_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/src/autora_theorist_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-21 22:43:59.000000 autora-theorist-toolkit-0.2.1/src/autora_theorist_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-21 22:43:59.000000 autora-theorist-toolkit-0.2.1/src/autora_theorist_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:43:59.000000 autora-theorist-toolkit-0.2.1/src/autora_theorist_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 22:43:59.000000 autora-theorist-toolkit-0.2.1/src/autora_theorist_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 22:43:59.000000 autora-theorist-toolkit-0.2.1/src/autora_theorist_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.517197 autora-theorist-toolkit-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/tests/test_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/tests/test_visual.py
```

### Comparing `autora-theorist-toolkit-0.2.0/.github/pull_request_template.md` & `autora-theorist-toolkit-0.2.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/.github/workflows/python-publish.yml` & `autora-theorist-toolkit-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/.gitignore` & `autora-theorist-toolkit-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/.idea/inspectionProfiles/Project_Default.xml` & `autora-theorist-toolkit-0.2.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/.pre-commit-config.yaml` & `autora-theorist-toolkit-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/PKG-INFO` & `autora-theorist-toolkit-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-toolkit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Toolkit to build algorithms for model recovery
 Author-email: "Joshua T. S. Hewson" <joshua_hewson@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/TheLemonPig/autora-theorist-toolkit
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-toolkit-0.2.0/README.md` & `autora-theorist-toolkit-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/docs/Additional Example.ipynb` & `autora-theorist-toolkit-0.2.1/docs/Additional Example.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/docs/Basic Usage.ipynb` & `autora-theorist-toolkit-0.2.1/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/docs/index.md` & `autora-theorist-toolkit-0.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/mkdocs/base.yml` & `autora-theorist-toolkit-0.2.1/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/pyproject.toml` & `autora-theorist-toolkit-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/components/nodes.py` & `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/components/nodes.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/components/primitives.py` & `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/components/primitives.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 from typing import List
+import numpy as np
+import scipy
 
 
 class Operation:
     def __init__(self, operator):
         self._operator = operator
 
     def __repr__(self):
         return self._operator
 
     def __call__(self, *args):
         ...
 
 
 class SimpleFunction(Operation):
-    def __init__(self, operator):
+    def __init__(self, operator, func):
         super().__init__(operator)
+        self._func = func
 
     def __call__(self, a):
-        return exec(f"{self._operator}{a}")
+        return exec(f"{self._operator}{a}", {self._operator: self._func})
 
 
 class Arithmetic(Operation):
     def __init__(self, operator):
         super().__init__(operator)
 
     def __call__(self, a, b):
         return eval(f"{a} {self._operator} {b}")
 
 
 default_primitives: List = [
     Arithmetic(operator) for operator in ["+", "-", "*", "/", "**"]
 ]
 default_primitives += [
-    SimpleFunction(operator)
-    for operator in [
-        "np.sin",
-        "np.cos",
-        "np.exp",
-        "np.log",
-        "np.heaviside",
-        "scipy.expit",
-    ]
+    SimpleFunction(operator[0], operator[1])
+    for operator in {
+        "sin": np.sin,
+        "cos": np.cos,
+        "exp": np.exp,
+        "log": np.log,
+        "heaviside": np.heaviside,
+        "expit": scipy.expit,
+        }
 ]
```

### Comparing `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/fitting.py` & `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/fitting.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/metrics.py` & `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/metrics.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/regression.py` & `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/regression.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,21 +20,19 @@
             except (FittingError, TypeError, ValueError, ZeroDivisionError):
                 obj.back_step()
 
     return handler
 
 
 def canonical(expr_str: str):
-    expr_str = expr_str.replace("np.", "")
     expr_sym = sympify(expr_str)
     expr_str = str(expr_sym)
     while "__a" in expr_str:
         start = expr_str.index("__a")
         stop = expr_str.index("__", start + 1) + 2
         expr_str = expr_str[:start] + "__c__" + expr_str[stop:]
     return expr_str
 
 
 def clean_equation(expr_str):
-    expr_str = expr_str.replace("np.", "")
     expr_sym = sympify(expr_str)
     return str(expr_sym)
```

### Comparing `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/methods/rules.py` & `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/rules.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py` & `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py` & `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py` & `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,81 @@
-import numpy as np
-import pandas as pd
-import scipy
-from sklearn.metrics import mean_squared_error
-
-from autora.theorist.toolkit.methods.fitting import scipy_curve_fit
-from autora.theorist.toolkit.methods.rules import less_than
-from autora.theorist.toolkit.models.symbolic_regression import SymbolicRegressor
-
-
 class HierarchicalSymbolicRegressor(SymbolicRegressor):
-    def __init__(self):
-        super().__init__()
+
+    def __init__(self, primitives=None):
+        super().__init__(primitives=primitives)
         self.ids = list()
         self.id_parameters = dict()
+        self.parameter_cache = Stack()
 
     def load_data(self, x, y, g):
         if isinstance(x, pd.DataFrame) and isinstance(y, pd.DataFrame):
             dv_variables, iv_variables = x.columns, y.columns
         elif isinstance(x, np.ndarray):
-            dv_variables = ["_x" + str(i) + "_" for i in range(x.shape[1])]
-            iv_variables = ["_y" + str(i) + "_" for i in range(y.shape[1])]
+            dv_variables = ['_x' + str(i) + '_' for i in range(x.shape[1])]
+            iv_variables = ['_y' + str(i) + '_' for i in range(y.shape[1])]
         else:
-            raise TypeError(
-                "Only valid types for x and y are pandas DataFrames and Numpy nd-arrays"
-            )
-        self.DVs = {
-            dv_variables[i]: np.array(x[:, i]) for i in range(len(dv_variables))
-        }
-        self.IVs = {
-            iv_variables[i]: np.array(y[:, i]) for i in range(len(iv_variables))
-        }
+            raise TypeError('Only valid types for x and y are pandas DataFrames and Numpy nd-arrays')
+        self.DVs = {dv_variables[i]: np.array(x[:, i]) for i in range(len(dv_variables))}
+        self.IVs = {iv_variables[i]: np.array(y[:, i]) for i in range(len(iv_variables))}
         self.ids = np.unique(g)
-        self.id_parameters = dict.fromkeys(self.ids, None)
+        self.id_parameters = dict.fromkeys(self.ids, [0.])
         self._variables = dv_variables
 
-    def get_id_data(self, x, y, g, id):
-        x, y = x[g == id], y[g == id]
-        if len(x.shape) == 1:
-            x = x.reshape(-1, 1)
-        if len(y.shape) == 1:
-            x = y.reshape(-1, 1)
-        return x, y
+    def cache(self):
+        self.parameter_cache.push(deepcopy(self.id_parameters))
+        super().cache()
+
+    def back_step(self):
+        self.id_parameters = self.parameter_cache.pop()
+        super().back_step()
+
+    def get_id_data(self, g, id, x, y=None):
+        id_x = x[g == id]
+        if len(id_x.shape) == 1:
+            id_x = id_x.reshape((-1, 1))
+        if y is None:
+            id_y = None
+        else:
+            id_y = y[g == id]
+            if len(id_y.shape) == 1:
+                id_y = id_y.reshape((-1, 1))
+        return id_x, id_y
 
     def update_dict(self, id, parameters):
         self.id_parameters.update({id: parameters})
 
-    def hierarchical_fit_step(
-        self,
-        X,
-        y,
-        g,
-        fitter=scipy_curve_fit,
-        metric=mean_squared_error,
-        accept=less_than,
-        *args,
-        **kwargs,
-    ):
-        self.load_data(X, y, g)
+    @regression_handler
+    def hierarchical_fit_step(self, X, y, g,
+                              fitter=scipy_curve_fit, metric=mean_squared_error, accept=less_than, *args, **kwargs):
         self.step()
         if not self.visited():
             self.optimize_parameters(X, y, g, fitter)
             self._record_visit()
-            y_pred = self.predict(X)
+            y_pred = self.predict(X, g)
             error = metric(y, y_pred, *args, **kwargs)
             if accept(error, self._error):
                 self._error = error
             else:
                 self.back_step()
         else:
             self.back_step()
+        return True
+
+    def predict(self, X, g):
+        y_predict = []
+        for id in np.unique(g):
+            id_x, _ = self.get_id_data(g, id, X, None)
+            parameters = self.id_parameters[id]
+            self.model_.set_parameters(parameters)
+            self._compile()
+            y_predict += super().predict(id_x).tolist()
+        return np.array(y_predict).reshape((-1, 1))
 
     def optimize_parameters(self, x, y, g, fitter):
-        if len(self.model_.get_parameters()) > 0:
-            for id in self.ids:
-                id_x, id_y = self.get_id_data(x, y, g, id)
+        for id in self.ids:
+            if len(self.model_.get_parameters()) > 0:
+                id_x, id_y = self.get_id_data(g, id, x, y)
                 fitted_parameters = fitter(id_x, id_y, self.get_expression())
                 self.update_dict(id, fitted_parameters)
-                print(f"{id}")
-                self._hier_compile()
-
-    def _hier_compile(self, x_type=tuple):
-        self.model_.catalog()
-        str_repr = self._sub_in_x(self.model_.__repr__(), x_type=x_type)
-        func_str = "def func(X,id):" + "\n"
-        func_str += "\t" + ",".join(
-            str(parameter) for parameter in self.model_.get_parameters()
-        )
-        func_str += "\t" + "= dic[id]" + "\n"
-        func_str += "\t" + "return " + str_repr
-        namespace = {}
-        exec(func_str, {"np": np, "scipy": scipy, "dic": self.id_parameters}, namespace)
-        self._expression = namespace["func"]
-        return "func", namespace
+            else:
+                self.update_dict(id, [])
+        self._compile()
```

### Comparing `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/hybrid_regression.py` & `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/hybrid_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/memory.py` & `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/memory.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py` & `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/symbolic_regression.py` & `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/symbolic_regression.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 from copy import deepcopy
 from inspect import signature
 from typing import List
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import scipy
 from sklearn.base import BaseEstimator
 from sklearn.metrics import mean_squared_error
 from tqdm import tqdm
 
 from autora.theorist.toolkit.components.nodes import Operator, Parameter, Variable
-from autora.theorist.toolkit.components.primitives import default_primitives
+from autora.theorist.toolkit.components.primitives import default_primitives, SimpleFunction
 from autora.theorist.toolkit.methods.fitting import scipy_curve_fit
 from autora.theorist.toolkit.methods.regression import canonical, regression_handler
 from autora.theorist.toolkit.methods.rules import less_than
 from autora.theorist.toolkit.models.memory import Stack
 from autora.theorist.toolkit.models.tree import Tree
 
 
@@ -25,14 +24,16 @@
     # TODO: replace tree=None with expression=None once build_tree() is made
     def __init__(self, tree=None, moves=None, primitives=None, metric=None):
         self.DVs = dict()  # currently unused
         self.IVs = dict()  # currently unused
         self.model_ = Tree() if tree is None else tree
         self.metric = mean_squared_error if metric is None else metric
         self._primitives = default_primitives if primitives is None else primitives
+        self._custom_primitives = {primitive[0]:primitive[1] for primitive in default_primitives
+                                   if isinstance(primitive, SimpleFunction)]
         self._expression = None
         self._value = None
         self._cache: Stack = Stack()
         self._moves: List[str] = (
             [
                 "Root/None",
                 "None/Root",
@@ -264,15 +265,15 @@
             + "): "
         )
         func_str += "return " + str_repr
         namespace = {
             str(parameter): parameter.get_value()
             for parameter in self.model_.get_parameters()
         }
-        exec(func_str, {"np": np, "scipy": scipy}, namespace)
+        exec(func_str, self._custom_primitives, namespace)
         self._expression = namespace["func"]
         return "func", namespace
 
     def visited(self):
         return canonical(str(self.model_)) in self._visit_list
 
     def get_parameters(self):
```

### Comparing `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/models/tree.py` & `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/tree.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/src/autora/theorist/toolkit/utils.py` & `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/utils.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/src/autora_theorist_toolkit.egg-info/PKG-INFO` & `autora-theorist-toolkit-0.2.1/src/autora_theorist_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-toolkit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Toolkit to build algorithms for model recovery
 Author-email: "Joshua T. S. Hewson" <joshua_hewson@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/TheLemonPig/autora-theorist-toolkit
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-toolkit-0.2.0/src/autora_theorist_toolkit.egg-info/SOURCES.txt` & `autora-theorist-toolkit-0.2.1/src/autora_theorist_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/tests/README.md` & `autora-theorist-toolkit-0.2.1/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/tests/test_toolkit.py` & `autora-theorist-toolkit-0.2.1/tests/test_toolkit.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.0/tests/test_visual.py` & `autora-theorist-toolkit-0.2.1/tests/test_visual.py`

 * *Files identical despite different names*

