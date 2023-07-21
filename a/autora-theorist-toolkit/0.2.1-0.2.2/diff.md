# Comparing `tmp/autora-theorist-toolkit-0.2.1.tar.gz` & `tmp/autora-theorist-toolkit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-theorist-toolkit-0.2.1.tar", last modified: Fri Jul 21 22:43:59 2023, max compression
+gzip compressed data, was "autora-theorist-toolkit-0.2.2.tar", last modified: Fri Jul 21 23:04:31 2023, max compression
```

## Comparing `autora-theorist-toolkit-0.2.1.tar` & `autora-theorist-toolkit-0.2.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.517197 autora-theorist-toolkit-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.509197 autora-theorist-toolkit-0.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.509197 autora-theorist-toolkit-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.509197 autora-theorist-toolkit-0.2.1/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.idea/autora-theorist-toolkit.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.509197 autora-theorist-toolkit-0.2.1/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-21 22:43:59.517197 autora-theorist-toolkit-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/docs/Additional Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 22:43:59.517197 autora-theorist-toolkit-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/src/autora/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/src/autora/theorist/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/components/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/components/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/ddm_bms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/hybrid_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.513197 autora-theorist-toolkit-0.2.1/src/autora_theorist_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-21 22:43:59.000000 autora-theorist-toolkit-0.2.1/src/autora_theorist_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-21 22:43:59.000000 autora-theorist-toolkit-0.2.1/src/autora_theorist_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:43:59.000000 autora-theorist-toolkit-0.2.1/src/autora_theorist_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 22:43:59.000000 autora-theorist-toolkit-0.2.1/src/autora_theorist_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 22:43:59.000000 autora-theorist-toolkit-0.2.1/src/autora_theorist_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:59.517197 autora-theorist-toolkit-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/tests/test_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-21 22:43:49.000000 autora-theorist-toolkit-0.2.1/tests/test_visual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.599252 autora-theorist-toolkit-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.591251 autora-theorist-toolkit-0.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.591251 autora-theorist-toolkit-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.idea/autora-theorist-toolkit.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-21 23:04:31.599252 autora-theorist-toolkit-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/docs/Additional Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 23:04:31.599252 autora-theorist-toolkit-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/src/autora/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/src/autora/theorist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/components/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/components/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.599252 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/ddm_bms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/hybrid_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.599252 autora-theorist-toolkit-0.2.2/src/autora_theorist_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-21 23:04:31.000000 autora-theorist-toolkit-0.2.2/src/autora_theorist_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-21 23:04:31.000000 autora-theorist-toolkit-0.2.2/src/autora_theorist_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 23:04:31.000000 autora-theorist-toolkit-0.2.2/src/autora_theorist_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 23:04:31.000000 autora-theorist-toolkit-0.2.2/src/autora_theorist_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 23:04:31.000000 autora-theorist-toolkit-0.2.2/src/autora_theorist_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.599252 autora-theorist-toolkit-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/tests/test_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/tests/test_visual.py
```

### Comparing `autora-theorist-toolkit-0.2.1/.github/pull_request_template.md` & `autora-theorist-toolkit-0.2.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/.github/workflows/python-publish.yml` & `autora-theorist-toolkit-0.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/.gitignore` & `autora-theorist-toolkit-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/.idea/inspectionProfiles/Project_Default.xml` & `autora-theorist-toolkit-0.2.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/.pre-commit-config.yaml` & `autora-theorist-toolkit-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/PKG-INFO` & `autora-theorist-toolkit-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-toolkit
-Version: 0.2.1
+Version: 0.2.2
 Summary: Toolkit to build algorithms for model recovery
 Author-email: "Joshua T. S. Hewson" <joshua_hewson@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/TheLemonPig/autora-theorist-toolkit
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-toolkit-0.2.1/README.md` & `autora-theorist-toolkit-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/docs/Additional Example.ipynb` & `autora-theorist-toolkit-0.2.2/docs/Additional Example.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/docs/Basic Usage.ipynb` & `autora-theorist-toolkit-0.2.2/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/docs/index.md` & `autora-theorist-toolkit-0.2.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/mkdocs/base.yml` & `autora-theorist-toolkit-0.2.2/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/pyproject.toml` & `autora-theorist-toolkit-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/components/nodes.py` & `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/components/nodes.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/components/primitives.py` & `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/components/primitives.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import List
+
 import numpy as np
 import scipy
 
 
 class Operation:
     def __init__(self, operator):
         self._operator = operator
@@ -18,14 +19,22 @@
     def __init__(self, operator, func):
         super().__init__(operator)
         self._func = func
 
     def __call__(self, a):
         return exec(f"{self._operator}{a}", {self._operator: self._func})
 
+    def __getitem__(self, item):
+        if item == 0:
+            return self._operator
+        elif item == 1:
+            return self._func
+        else:
+            raise KeyError(f"Invalid key to {self.__class__.__name__}")
+
 
 class Arithmetic(Operation):
     def __init__(self, operator):
         super().__init__(operator)
 
     def __call__(self, a, b):
         return eval(f"{a} {self._operator} {b}")
@@ -38,10 +47,10 @@
     SimpleFunction(operator[0], operator[1])
     for operator in {
         "sin": np.sin,
         "cos": np.cos,
         "exp": np.exp,
         "log": np.log,
         "heaviside": np.heaviside,
-        "expit": scipy.expit,
-        }
+        "expit": scipy.special.expit,
+    }
 ]
```

### Comparing `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/fitting.py` & `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/fitting.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/metrics.py` & `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/metrics.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/regression.py` & `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/methods/rules.py` & `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/rules.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py` & `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py` & `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py` & `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,88 @@
+import logging
+import random
+
+import numpy as np
+from tqdm import tqdm
+
+from autora.theorist.toolkit.methods.metrics import MinimumDescriptionLength
+from autora.theorist.toolkit.methods.rules import replace_node
+from autora.theorist.toolkit.models.hierarchical_symbolic_regressor import (
+    HierarchicalSymbolicRegressor,
+)
+
+logging.basicConfig(level=logging.INFO)
+_logger = logging.getLogger(__name__)
+
+prior_dict_ = {
+    "+": 3.0,
+    "-": 3.0,
+    "*": 3.0,
+    "/": 3.0,
+    "**": 3.0,
+    "sin": 10.0,
+    "exp": 10.0,
+    "log": 10.0,
+}
+
+temperatures_ = [1.04**n for n in range(20)]
+
+
 class HierarchicalBayesianSymbolicRegression:
+    def __init__(self, temperatures=None, prior_dict=None, primitives=None):
+        self.primitives = primitives
+        self.temperatures = temperatures_ if temperatures is None else temperatures
+        self.prior_dict = prior_dict_ if prior_dict is None else prior_dict
+        self.theorists = [
+            HierarchicalSymbolicRegressor(primitives=primitives)
+            for _ in self.temperatures
+        ]
+
+    def fit(self, x, y, g, epochs=100, verbose=False):
+        n_swaps = 0
+        for theorist in self.theorists:
+            theorist.load_data(x, y, g)
+        for n in tqdm(range(epochs)):
+            for i, theorist in enumerate(self.theorists):
+                metric = MinimumDescriptionLength(
+                    n=x.shape[0],
+                    k=len(theorist.model_.get_parameters()),
+                    prior_dict=self.prior_dict,
+                    expr_str=str(theorist.model_),
+                    bic_temp=self.temperatures[i],
+                )
+                theorist.hierarchical_fit_step(X=x, y=y, g=g, metric=metric)
+                _logger.debug("Finish iteration {}".format(n))
+            n_swaps += int(self.tree_swap(x, y, g))
+        if verbose:
+            print(f"Number of tree swaps: {n_swaps} swaps out of {epochs} epochs")
 
-  def __init__(self, temperatures, prior_dict, primitives=None):
-    self.primitives = primitives
-    self.temperatures = temperatures
-    self.prior_dict = prior_dict
-    self.theorists = [HierarchicalSymbolicRegressor(primitives=primitives) for _ in self.temperatures]
-
-  def fit(self, x, y, g, epochs=100):
-    n_swaps = 0
-    for theorist in self.theorists:
-      theorist.load_data(x, y, g)
-    for n in tqdm(range(epochs)):
-        for i, theorist in enumerate(self.theorists):
-            metric = MinimumDescriptionLength(n=x.shape[0], k=len(theorist.model_.get_parameters()),
-                                              prior_dict=self.prior_dict, expr_str=str(theorist.model_),
-                                              bic_temp=self.temperatures[i])
-            theorist.hierarchical_fit_step(X=x, y=y,g=g, metric=metric)
-            _logger.debug("Finish iteration {}".format(n))
-        self.tree_swap(x, y, g)
-
-  def tree_swap(self, x, y, g):
-      j = random.choice(range(len(self.temperatures)-1))
-      temp1, temp2 = self.temperatures[j:j+2]
-      theorist1, theorist2 = self.theorists[j:j+2]
-      y_pred1 = theorist1.predict(x, g)
-      if isinstance(y_pred1, float):
-          y_pred1 = np.ones(y.shape) * y_pred1
-      y_pred2 = theorist2.predict(x, g)
-      if isinstance(y_pred2, float):
-          y_pred2 = np.ones(y.shape) * y_pred2
-      loss1 = MinimumDescriptionLength(n=x.shape[0], k=len(theorist1.model_.get_parameters()),
-                                        prior_dict=self.prior_dict, expr_str=str(theorist1.model_),
-                                        bic_temp=temp1)(y, y_pred1)
-      loss2 = MinimumDescriptionLength(n=x.shape[0], k=len(theorist2.model_.get_parameters()),
-                                        prior_dict=self.prior_dict, expr_str=str(theorist2.model_),
-                                        bic_temp=temp2)(y, y_pred2)
-      mdl_change = loss1*(1/temp2-1/temp1) + loss2*(1/temp1-1/temp2)
-      if replace_node(-mdl_change):
-          self.theorists[j:j+2] = theorist2, theorist1
-          return True
-      else:
-          return False
+    def tree_swap(self, x, y, g):
+        j = random.choice(range(len(self.temperatures) - 1))
+        temp1, temp2 = self.temperatures[j : j + 2]
+        theorist1, theorist2 = self.theorists[j : j + 2]
+        y_pred1 = theorist1.predict(x, g)
+        if isinstance(y_pred1, float):
+            y_pred1 = np.ones(y.shape) * y_pred1
+        y_pred2 = theorist2.predict(x, g)
+        if isinstance(y_pred2, float):
+            y_pred2 = np.ones(y.shape) * y_pred2
+        loss1 = MinimumDescriptionLength(
+            n=x.shape[0],
+            k=len(theorist1.model_.get_parameters()),
+            prior_dict=self.prior_dict,
+            expr_str=str(theorist1.model_),
+            bic_temp=temp1,
+        )(y, y_pred1)
+        loss2 = MinimumDescriptionLength(
+            n=x.shape[0],
+            k=len(theorist2.model_.get_parameters()),
+            prior_dict=self.prior_dict,
+            expr_str=str(theorist2.model_),
+            bic_temp=temp2,
+        )(y, y_pred2)
+        mdl_change = loss1 * (1 / temp2 - 1 / temp1) + loss2 * (1 / temp1 - 1 / temp2)
+        if replace_node(-mdl_change):
+            self.theorists[j : j + 2] = theorist2, theorist1
+            return True
+        else:
+            return False
```

### Comparing `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/hybrid_regression.py` & `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/hybrid_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/memory.py` & `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/memory.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py` & `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/symbolic_regression.py` & `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/symbolic_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 import numpy as np
 import pandas as pd
 from sklearn.base import BaseEstimator
 from sklearn.metrics import mean_squared_error
 from tqdm import tqdm
 
 from autora.theorist.toolkit.components.nodes import Operator, Parameter, Variable
-from autora.theorist.toolkit.components.primitives import default_primitives, SimpleFunction
+from autora.theorist.toolkit.components.primitives import (
+    SimpleFunction,
+    default_primitives,
+)
 from autora.theorist.toolkit.methods.fitting import scipy_curve_fit
 from autora.theorist.toolkit.methods.regression import canonical, regression_handler
 from autora.theorist.toolkit.methods.rules import less_than
 from autora.theorist.toolkit.models.memory import Stack
 from autora.theorist.toolkit.models.tree import Tree
 
 
@@ -24,16 +27,19 @@
     # TODO: replace tree=None with expression=None once build_tree() is made
     def __init__(self, tree=None, moves=None, primitives=None, metric=None):
         self.DVs = dict()  # currently unused
         self.IVs = dict()  # currently unused
         self.model_ = Tree() if tree is None else tree
         self.metric = mean_squared_error if metric is None else metric
         self._primitives = default_primitives if primitives is None else primitives
-        self._custom_primitives = {primitive[0]:primitive[1] for primitive in default_primitives
-                                   if isinstance(primitive, SimpleFunction)]
+        self._custom_primitives = {
+            primitive[0]: primitive[1]
+            for primitive in default_primitives
+            if isinstance(primitive, SimpleFunction)
+        }
         self._expression = None
         self._value = None
         self._cache: Stack = Stack()
         self._moves: List[str] = (
             [
                 "Root/None",
                 "None/Root",
```

### Comparing `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/models/tree.py` & `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/tree.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/src/autora/theorist/toolkit/utils.py` & `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/utils.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/src/autora_theorist_toolkit.egg-info/PKG-INFO` & `autora-theorist-toolkit-0.2.2/src/autora_theorist_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-toolkit
-Version: 0.2.1
+Version: 0.2.2
 Summary: Toolkit to build algorithms for model recovery
 Author-email: "Joshua T. S. Hewson" <joshua_hewson@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/TheLemonPig/autora-theorist-toolkit
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-toolkit-0.2.1/src/autora_theorist_toolkit.egg-info/SOURCES.txt` & `autora-theorist-toolkit-0.2.2/src/autora_theorist_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/tests/README.md` & `autora-theorist-toolkit-0.2.2/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.1/tests/test_toolkit.py` & `autora-theorist-toolkit-0.2.2/tests/test_toolkit.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 from autora.theorist.toolkit.models.bayesian_machine_scientist import (
     BayesianMachineScientist,
 )
 from autora.theorist.toolkit.models.bayesian_symbolic_regression import (
     BayesianSymbolicRegressor,
 )
+from autora.theorist.toolkit.models.hierarchical_bayesian_symbolic_regression import (
+    HierarchicalBayesianSymbolicRegression,
+)
 from autora.theorist.toolkit.models.memory import Stack
 from autora.theorist.toolkit.models.parallel_symbolic_regression import (
     ParallelSymbolicRegressor,
 )
 from autora.theorist.toolkit.models.symbolic_regression import SymbolicRegressor
 from autora.theorist.toolkit.models.tree import Tree
 
@@ -39,19 +42,20 @@
     theorist = ParallelSymbolicRegressor(
         temperatures=temperatures_, prior_dict=prior_dict_
     )
     assert theorist is not None
 
 
 def test_bayesian_machine_scientist_initialization():
-    prior_dict_ = {"+": 1.0}
-    temperatures_ = [1.04**t for t in range(20)]
-    theorist = BayesianMachineScientist(
-        temperatures=temperatures_, prior_dict=prior_dict_
-    )
+    theorist = BayesianMachineScientist()
+    assert theorist is not None
+
+
+def test_hbsr_running():
+    theorist = HierarchicalBayesianSymbolicRegression()
     assert theorist is not None
 
 
 if __name__ == "__main__":
     test_symbolic_regression_initialization()
     test_bayesian_symbolic_regression_initialization()
     test_parallel_symbolic_regression_initialization()
```

### Comparing `autora-theorist-toolkit-0.2.1/tests/test_visual.py` & `autora-theorist-toolkit-0.2.2/tests/test_visual.py`

 * *Files identical despite different names*

