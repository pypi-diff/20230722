# Comparing `tmp/autora-theorist-toolkit-0.2.2.tar.gz` & `tmp/autora-theorist-toolkit-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-theorist-toolkit-0.2.2.tar", last modified: Fri Jul 21 23:04:31 2023, max compression
+gzip compressed data, was "autora-theorist-toolkit-0.2.3.tar", last modified: Sat Jul 22 00:09:02 2023, max compression
```

## Comparing `autora-theorist-toolkit-0.2.2.tar` & `autora-theorist-toolkit-0.2.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.599252 autora-theorist-toolkit-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.591251 autora-theorist-toolkit-0.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.591251 autora-theorist-toolkit-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.idea/autora-theorist-toolkit.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-21 23:04:31.599252 autora-theorist-toolkit-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/docs/Additional Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 23:04:31.599252 autora-theorist-toolkit-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/src/autora/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/src/autora/theorist/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/components/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/components/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.595252 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.599252 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/ddm_bms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/hybrid_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.599252 autora-theorist-toolkit-0.2.2/src/autora_theorist_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-21 23:04:31.000000 autora-theorist-toolkit-0.2.2/src/autora_theorist_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-21 23:04:31.000000 autora-theorist-toolkit-0.2.2/src/autora_theorist_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 23:04:31.000000 autora-theorist-toolkit-0.2.2/src/autora_theorist_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 23:04:31.000000 autora-theorist-toolkit-0.2.2/src/autora_theorist_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 23:04:31.000000 autora-theorist-toolkit-0.2.2/src/autora_theorist_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:31.599252 autora-theorist-toolkit-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/tests/test_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-21 23:04:20.000000 autora-theorist-toolkit-0.2.2/tests/test_visual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.232451 autora-theorist-toolkit-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.idea/autora-theorist-toolkit.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-22 00:09:02.232451 autora-theorist-toolkit-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/docs/Additional Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 00:09:02.232451 autora-theorist-toolkit-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/src/autora/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/src/autora/theorist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.228451 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.232451 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/components/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/components/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.232451 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.232451 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/ddm_bms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/hybrid_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.232451 autora-theorist-toolkit-0.2.3/src/autora_theorist_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-22 00:09:02.000000 autora-theorist-toolkit-0.2.3/src/autora_theorist_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-22 00:09:02.000000 autora-theorist-toolkit-0.2.3/src/autora_theorist_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 00:09:02.000000 autora-theorist-toolkit-0.2.3/src/autora_theorist_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-22 00:09:02.000000 autora-theorist-toolkit-0.2.3/src/autora_theorist_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-22 00:09:02.000000 autora-theorist-toolkit-0.2.3/src/autora_theorist_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:09:02.232451 autora-theorist-toolkit-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/tests/test_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-22 00:08:51.000000 autora-theorist-toolkit-0.2.3/tests/test_visual.py
```

### Comparing `autora-theorist-toolkit-0.2.2/.github/pull_request_template.md` & `autora-theorist-toolkit-0.2.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/.github/workflows/python-publish.yml` & `autora-theorist-toolkit-0.2.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/.gitignore` & `autora-theorist-toolkit-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/.idea/inspectionProfiles/Project_Default.xml` & `autora-theorist-toolkit-0.2.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/.pre-commit-config.yaml` & `autora-theorist-toolkit-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/PKG-INFO` & `autora-theorist-toolkit-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-toolkit
-Version: 0.2.2
+Version: 0.2.3
 Summary: Toolkit to build algorithms for model recovery
 Author-email: "Joshua T. S. Hewson" <joshua_hewson@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/TheLemonPig/autora-theorist-toolkit
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-toolkit-0.2.2/README.md` & `autora-theorist-toolkit-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/docs/Additional Example.ipynb` & `autora-theorist-toolkit-0.2.3/docs/Additional Example.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/docs/Basic Usage.ipynb` & `autora-theorist-toolkit-0.2.3/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/docs/index.md` & `autora-theorist-toolkit-0.2.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/mkdocs/base.yml` & `autora-theorist-toolkit-0.2.3/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/pyproject.toml` & `autora-theorist-toolkit-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/components/nodes.py` & `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/components/nodes.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/components/primitives.py` & `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/components/primitives.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,9 +48,9 @@
     for operator in {
         "sin": np.sin,
         "cos": np.cos,
         "exp": np.exp,
         "log": np.log,
         "heaviside": np.heaviside,
         "expit": scipy.special.expit,
-    }
+    }.items()
 ]
```

### Comparing `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/fitting.py` & `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/fitting.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/metrics.py` & `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/metrics.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/regression.py` & `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/methods/rules.py` & `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/methods/rules.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py` & `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py` & `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py` & `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import random
 
 import numpy as np
 from tqdm import tqdm
 
+from autora.theorist.toolkit.components.primitives import default_primitives
 from autora.theorist.toolkit.methods.metrics import MinimumDescriptionLength
 from autora.theorist.toolkit.methods.rules import replace_node
 from autora.theorist.toolkit.models.hierarchical_symbolic_regressor import (
     HierarchicalSymbolicRegressor,
 )
 
 logging.basicConfig(level=logging.INFO)
@@ -25,19 +26,24 @@
 }
 
 temperatures_ = [1.04**n for n in range(20)]
 
 
 class HierarchicalBayesianSymbolicRegression:
     def __init__(self, temperatures=None, prior_dict=None, primitives=None):
-        self.primitives = primitives
         self.temperatures = temperatures_ if temperatures is None else temperatures
         self.prior_dict = prior_dict_ if prior_dict is None else prior_dict
+        primitives_ = default_primitives if primitives is None else primitives
+        self.primitives = [
+            primitive
+            for primitive in primitives_
+            if str(primitive) in list(self.prior_dict.keys())
+        ]
         self.theorists = [
-            HierarchicalSymbolicRegressor(primitives=primitives)
+            HierarchicalSymbolicRegressor(primitives=self.primitives)
             for _ in self.temperatures
         ]
 
     def fit(self, x, y, g, epochs=100, verbose=False):
         n_swaps = 0
         for theorist in self.theorists:
             theorist.load_data(x, y, g)
```

### Comparing `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py` & `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/hybrid_regression.py` & `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/hybrid_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/memory.py` & `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/memory.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py` & `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/symbolic_regression.py` & `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/symbolic_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/models/tree.py` & `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/models/tree.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/src/autora/theorist/toolkit/utils.py` & `autora-theorist-toolkit-0.2.3/src/autora/theorist/toolkit/utils.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/src/autora_theorist_toolkit.egg-info/PKG-INFO` & `autora-theorist-toolkit-0.2.3/src/autora_theorist_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-toolkit
-Version: 0.2.2
+Version: 0.2.3
 Summary: Toolkit to build algorithms for model recovery
 Author-email: "Joshua T. S. Hewson" <joshua_hewson@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/TheLemonPig/autora-theorist-toolkit
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-toolkit-0.2.2/src/autora_theorist_toolkit.egg-info/SOURCES.txt` & `autora-theorist-toolkit-0.2.3/src/autora_theorist_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/tests/README.md` & `autora-theorist-toolkit-0.2.3/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.2/tests/test_toolkit.py` & `autora-theorist-toolkit-0.2.3/tests/test_toolkit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import scipy
 
 from autora.theorist.toolkit.models.bayesian_machine_scientist import (
     BayesianMachineScientist,
 )
 from autora.theorist.toolkit.models.bayesian_symbolic_regression import (
     BayesianSymbolicRegressor,
 )
@@ -46,17 +47,33 @@
 
 
 def test_bayesian_machine_scientist_initialization():
     theorist = BayesianMachineScientist()
     assert theorist is not None
 
 
-def test_hbsr_running():
-    theorist = HierarchicalBayesianSymbolicRegression()
-    assert theorist is not None
+def test_hsbr_prior_restriction_and_fitting():
+    prior_dict_ = {"+": 1.0, "expit": 1.0}
+    hsbr = HierarchicalBayesianSymbolicRegression(prior_dict=prior_dict_)
+    assert len(hsbr.theorists[-1]._primitives) > 0
+    x = scipy.special.expit(np.linspace(0, 1, 100)).reshape((-1, 1))
+    y = 1 + x
+    g = np.ones_like(x)
+    hsbr.fit(x, y, g, epochs=30)
+    assert "-" not in hsbr.theorists[-1].model_
+    assert "*" not in hsbr.theorists[-1].model_
+    assert "**" not in hsbr.theorists[-1].model_
+    assert "/" not in hsbr.theorists[-1].model_
+    assert "cos" not in hsbr.theorists[-1].model_
+    assert "exp" not in hsbr.theorists[-1].model_
+    assert "log" not in hsbr.theorists[-1].model_
+    assert "sin" not in hsbr.theorists[-1].model_
+    assert (
+        np.sum(hsbr.theorists[-1].predict(x, g) - y) == 0
+    ), f"{hsbr.theorists[-1].model_} but should be 1+expit(x)"
 
 
 if __name__ == "__main__":
     test_symbolic_regression_initialization()
     test_bayesian_symbolic_regression_initialization()
     test_parallel_symbolic_regression_initialization()
     test_bayesian_machine_scientist_initialization()
```

### Comparing `autora-theorist-toolkit-0.2.2/tests/test_visual.py` & `autora-theorist-toolkit-0.2.3/tests/test_visual.py`

 * *Files identical despite different names*

