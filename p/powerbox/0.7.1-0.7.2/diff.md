# Comparing `tmp/powerbox-0.7.1.tar.gz` & `tmp/powerbox-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerbox-0.7.1.tar", last modified: Tue Dec 13 06:40:32 2022, max compression
+gzip compressed data, was "powerbox-0.7.2.tar", last modified: Fri Jul 21 23:23:20 2023, max compression
```

## Comparing `powerbox-0.7.1.tar` & `powerbox-0.7.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 06:40:32.828793 powerbox-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2022-12-13 06:40:20.000000 powerbox-0.7.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      700 2022-12-13 06:40:20.000000 powerbox-0.7.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 06:40:32.796792 powerbox-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 06:40:32.804793 powerbox-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2022-12-13 06:40:20.000000 powerbox-0.7.1/.github/workflows/deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      942 2022-12-13 06:40:20.000000 powerbox-0.7.1/.github/workflows/run-docs-code.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2022-12-13 06:40:20.000000 powerbox-0.7.1/.github/workflows/test-with-warnings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      853 2022-12-13 06:40:20.000000 powerbox-0.7.1/.github/workflows/testsuite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-13 06:40:20.000000 powerbox-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      284 2022-12-13 06:40:20.000000 powerbox-0.7.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2022-12-13 06:40:20.000000 powerbox-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      658 2022-12-13 06:40:20.000000 powerbox-0.7.1/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 06:40:32.804793 powerbox-0.7.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-13 06:40:20.000000 powerbox-0.7.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2022-12-13 06:40:20.000000 powerbox-0.7.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2022-12-13 06:40:20.000000 powerbox-0.7.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2022-12-13 06:40:20.000000 powerbox-0.7.1/CONTRIBUTORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2022-12-13 06:40:20.000000 powerbox-0.7.1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2022-12-13 06:40:32.824792 powerbox-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2022-12-13 06:40:20.000000 powerbox-0.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 06:40:32.804793 powerbox-0.7.1/devel/
--rw-r--r--   0 runner    (1001) docker     (123)   568645 2022-12-13 06:40:20.000000 powerbox-0.7.1/devel/hankel_transform_of_cosmo_power.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    55814 2022-12-13 06:40:20.000000 powerbox-0.7.1/devel/testing_angular_averaging.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 06:40:32.808792 powerbox-0.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2022-12-13 06:40:20.000000 powerbox-0.7.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 06:40:32.808792 powerbox-0.7.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2022-12-13 06:40:20.000000 powerbox-0.7.1/docs/api/dft.rst
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-13 06:40:20.000000 powerbox-0.7.1/docs/api/powerbox.rst
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-13 06:40:20.000000 powerbox-0.7.1/docs/api/tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-13 06:40:20.000000 powerbox-0.7.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-13 06:40:20.000000 powerbox-0.7.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-13 06:40:20.000000 powerbox-0.7.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2022-12-13 06:40:20.000000 powerbox-0.7.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-13 06:40:20.000000 powerbox-0.7.1/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 06:40:32.816793 powerbox-0.7.1/docs/demos/
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2022-12-13 06:40:20.000000 powerbox-0.7.1/docs/demos/algorithm.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1160970 2022-12-13 06:40:20.000000 powerbox-0.7.1/docs/demos/cosmological_fields.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   438752 2022-12-13 06:40:20.000000 powerbox-0.7.1/docs/demos/dft.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1067152 2022-12-13 06:40:20.000000 powerbox-0.7.1/docs/demos/getting_started.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      336 2022-12-13 06:40:20.000000 powerbox-0.7.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      463 2022-12-13 06:40:20.000000 powerbox-0.7.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-13 06:40:20.000000 powerbox-0.7.1/docs/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 06:40:32.816793 powerbox-0.7.1/docs/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2022-12-13 06:40:20.000000 powerbox-0.7.1/docs/templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      722 2022-12-13 06:40:20.000000 powerbox-0.7.1/docs/templates/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 06:40:32.824792 powerbox-0.7.1/paper/
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2022-12-13 06:40:20.000000 powerbox-0.7.1/paper/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    98285 2022-12-13 06:40:20.000000 powerbox-0.7.1/paper/joss-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2022-12-13 06:40:20.000000 powerbox-0.7.1/paper/latex.template
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2022-12-13 06:40:20.000000 powerbox-0.7.1/paper/paper.aux
--rw-r--r--   0 runner    (1001) docker     (123)    90028 2022-12-13 06:40:20.000000 powerbox-0.7.1/paper/paper.bcf
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2022-12-13 06:40:20.000000 powerbox-0.7.1/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)    59139 2022-12-13 06:40:20.000000 powerbox-0.7.1/paper/paper.log
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2022-12-13 06:40:20.000000 powerbox-0.7.1/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)      141 2022-12-13 06:40:20.000000 powerbox-0.7.1/paper/paper.out
--rw-r--r--   0 runner    (1001) docker     (123)   130296 2022-12-13 06:40:20.000000 powerbox-0.7.1/paper/paper.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2022-12-13 06:40:20.000000 powerbox-0.7.1/paper/paper.run.xml
--rw-r--r--   0 runner    (1001) docker     (123)    13924 2022-12-13 06:40:20.000000 powerbox-0.7.1/paper/paper.tex
--rw-r--r--   0 runner    (1001) docker     (123)   107445 2022-12-13 06:40:20.000000 powerbox-0.7.1/paper/paper.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2022-12-13 06:40:20.000000 powerbox-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-13 06:40:32.828793 powerbox-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 06:40:32.796792 powerbox-0.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 06:40:32.824792 powerbox-0.7.1/src/powerbox/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2022-12-13 06:40:20.000000 powerbox-0.7.1/src/powerbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-13 06:40:32.000000 powerbox-0.7.1/src/powerbox/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12451 2022-12-13 06:40:20.000000 powerbox-0.7.1/src/powerbox/dft.py
--rw-r--r--   0 runner    (1001) docker     (123)    14916 2022-12-13 06:40:20.000000 powerbox-0.7.1/src/powerbox/powerbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    20533 2022-12-13 06:40:20.000000 powerbox-0.7.1/src/powerbox/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 06:40:32.824792 powerbox-0.7.1/src/powerbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2022-12-13 06:40:32.000000 powerbox-0.7.1/src/powerbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2022-12-13 06:40:32.000000 powerbox-0.7.1/src/powerbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 06:40:32.000000 powerbox-0.7.1/src/powerbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2022-12-13 06:40:32.000000 powerbox-0.7.1/src/powerbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-13 06:40:32.000000 powerbox-0.7.1/src/powerbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 06:40:32.824792 powerbox-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2022-12-13 06:40:20.000000 powerbox-0.7.1/tests/test_direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2022-12-13 06:40:20.000000 powerbox-0.7.1/tests/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2022-12-13 06:40:20.000000 powerbox-0.7.1/tests/test_fft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2022-12-13 06:40:20.000000 powerbox-0.7.1/tests/test_lognormal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2022-12-13 06:40:20.000000 powerbox-0.7.1/tests/test_power.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2022-12-13 06:40:20.000000 powerbox-0.7.1/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2022-12-13 06:40:20.000000 powerbox-0.7.1/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:23:20.154286 powerbox-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-21 23:23:10.000000 powerbox-0.7.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-21 23:23:10.000000 powerbox-0.7.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:23:20.138286 powerbox-0.7.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:23:20.142286 powerbox-0.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-21 23:23:10.000000 powerbox-0.7.2/.github/workflows/deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-21 23:23:10.000000 powerbox-0.7.2/.github/workflows/run-docs-code.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-21 23:23:10.000000 powerbox-0.7.2/.github/workflows/test-with-warnings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-21 23:23:10.000000 powerbox-0.7.2/.github/workflows/testsuite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-21 23:23:10.000000 powerbox-0.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-21 23:23:10.000000 powerbox-0.7.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-21 23:23:10.000000 powerbox-0.7.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-21 23:23:10.000000 powerbox-0.7.2/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:23:20.142286 powerbox-0.7.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 23:23:10.000000 powerbox-0.7.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-07-21 23:23:10.000000 powerbox-0.7.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-21 23:23:10.000000 powerbox-0.7.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-21 23:23:10.000000 powerbox-0.7.2/CONTRIBUTORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-21 23:23:10.000000 powerbox-0.7.2/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-21 23:23:20.154286 powerbox-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-21 23:23:10.000000 powerbox-0.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:23:20.142286 powerbox-0.7.2/devel/
+-rw-r--r--   0 runner    (1001) docker     (123)   568645 2023-07-21 23:23:10.000000 powerbox-0.7.2/devel/hankel_transform_of_cosmo_power.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    55814 2023-07-21 23:23:10.000000 powerbox-0.7.2/devel/testing_angular_averaging.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:23:20.146286 powerbox-0.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-21 23:23:10.000000 powerbox-0.7.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:23:20.146286 powerbox-0.7.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-21 23:23:10.000000 powerbox-0.7.2/docs/api/dft.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-21 23:23:10.000000 powerbox-0.7.2/docs/api/powerbox.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-21 23:23:10.000000 powerbox-0.7.2/docs/api/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-21 23:23:10.000000 powerbox-0.7.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-21 23:23:10.000000 powerbox-0.7.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-21 23:23:10.000000 powerbox-0.7.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-07-21 23:23:10.000000 powerbox-0.7.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-21 23:23:10.000000 powerbox-0.7.2/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:23:20.146286 powerbox-0.7.2/docs/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-21 23:23:10.000000 powerbox-0.7.2/docs/demos/algorithm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1160970 2023-07-21 23:23:10.000000 powerbox-0.7.2/docs/demos/cosmological_fields.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   438752 2023-07-21 23:23:10.000000 powerbox-0.7.2/docs/demos/dft.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1067152 2023-07-21 23:23:10.000000 powerbox-0.7.2/docs/demos/getting_started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-21 23:23:10.000000 powerbox-0.7.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-21 23:23:10.000000 powerbox-0.7.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 23:23:10.000000 powerbox-0.7.2/docs/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:23:20.146286 powerbox-0.7.2/docs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-21 23:23:10.000000 powerbox-0.7.2/docs/templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-21 23:23:10.000000 powerbox-0.7.2/docs/templates/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:23:20.150286 powerbox-0.7.2/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-21 23:23:10.000000 powerbox-0.7.2/paper/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    98285 2023-07-21 23:23:10.000000 powerbox-0.7.2/paper/joss-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-07-21 23:23:10.000000 powerbox-0.7.2/paper/latex.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-21 23:23:10.000000 powerbox-0.7.2/paper/paper.aux
+-rw-r--r--   0 runner    (1001) docker     (123)    90028 2023-07-21 23:23:10.000000 powerbox-0.7.2/paper/paper.bcf
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-07-21 23:23:10.000000 powerbox-0.7.2/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)    59139 2023-07-21 23:23:10.000000 powerbox-0.7.2/paper/paper.log
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-07-21 23:23:10.000000 powerbox-0.7.2/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-21 23:23:10.000000 powerbox-0.7.2/paper/paper.out
+-rw-r--r--   0 runner    (1001) docker     (123)   130296 2023-07-21 23:23:10.000000 powerbox-0.7.2/paper/paper.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-21 23:23:10.000000 powerbox-0.7.2/paper/paper.run.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    13924 2023-07-21 23:23:10.000000 powerbox-0.7.2/paper/paper.tex
+-rw-r--r--   0 runner    (1001) docker     (123)   107445 2023-07-21 23:23:10.000000 powerbox-0.7.2/paper/paper.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-21 23:23:10.000000 powerbox-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 23:23:20.154286 powerbox-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:23:20.138286 powerbox-0.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:23:20.150286 powerbox-0.7.2/src/powerbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-21 23:23:10.000000 powerbox-0.7.2/src/powerbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-21 23:23:20.000000 powerbox-0.7.2/src/powerbox/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-07-21 23:23:10.000000 powerbox-0.7.2/src/powerbox/dft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14950 2023-07-21 23:23:10.000000 powerbox-0.7.2/src/powerbox/powerbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20533 2023-07-21 23:23:10.000000 powerbox-0.7.2/src/powerbox/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:23:20.150286 powerbox-0.7.2/src/powerbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-21 23:23:20.000000 powerbox-0.7.2/src/powerbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-21 23:23:20.000000 powerbox-0.7.2/src/powerbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 23:23:20.000000 powerbox-0.7.2/src/powerbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-21 23:23:20.000000 powerbox-0.7.2/src/powerbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 23:23:20.000000 powerbox-0.7.2/src/powerbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:23:20.154286 powerbox-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-21 23:23:10.000000 powerbox-0.7.2/tests/test_direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-21 23:23:10.000000 powerbox-0.7.2/tests/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-21 23:23:10.000000 powerbox-0.7.2/tests/test_fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-21 23:23:10.000000 powerbox-0.7.2/tests/test_lognormal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-21 23:23:10.000000 powerbox-0.7.2/tests/test_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-21 23:23:10.000000 powerbox-0.7.2/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-07-21 23:23:10.000000 powerbox-0.7.2/tests/test_tools.py
```

### Comparing `powerbox-0.7.1/.github/workflows/deploy.yaml` & `powerbox-0.7.2/.github/workflows/deploy.yaml`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/.github/workflows/run-docs-code.yaml` & `powerbox-0.7.2/.github/workflows/run-docs-code.yaml`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/.github/workflows/test-with-warnings.yaml` & `powerbox-0.7.2/.github/workflows/test-with-warnings.yaml`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/.github/workflows/testsuite.yaml` & `powerbox-0.7.2/.github/workflows/testsuite.yaml`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/.pre-commit-config.yaml` & `powerbox-0.7.2/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,57 @@
 exclude: '^docs/conf.py'
 
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.2.0
+  rev: v4.4.0
   hooks:
   - id: trailing-whitespace
   - id: check-added-large-files
   - id: check-ast
   - id: check-json
   - id: check-merge-conflict
   - id: check-xml
   - id: debug-statements
   - id: end-of-file-fixer
   - id: requirements-txt-fixer
   - id: mixed-line-ending
     args: ['--fix=no']
 
 - repo: https://github.com/PyCQA/flake8
-  rev: 4.0.1
+  rev: 6.0.0
   hooks:
   - id: flake8
     additional_dependencies:
-      - flake8-comprehensions
-      - flake8-logging-format
       - flake8-builtins
-      - flake8-eradicate
+#      - flake8-eradicate  # flake8 6 incompatible
       - pep8-naming
       - flake8-pytest
       - flake8-docstrings
       - flake8-rst-docstrings
       - flake8-rst
-      - flake8-copyright
+#      - flake8-copyright  # flake8 6 incompatible
       - flake8-markdown
       - flake8-bugbear
-      - flake8-comprehensions
+ #     - flake8-comprehensions  # flake8 6 incompatible
       - flake8-print
 
 
 - repo: https://github.com/psf/black
-  rev: 22.3.0
+  rev: 23.7.0
   hooks:
   - id: black
 
 - repo: https://github.com/PyCQA/isort
-  rev: 5.10.1
+  rev: 5.12.0
   hooks:
   - id: isort
 
 - repo: https://github.com/pre-commit/pygrep-hooks
-  rev: v1.9.0
+  rev: v1.10.0
   hooks:
     - id: rst-backticks
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v2.32.0
+  rev: v3.9.0
   hooks:
   -   id: pyupgrade
       args: [--py38-plus]
```

### Comparing `powerbox-0.7.1/.readthedocs.yml` & `powerbox-0.7.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/CHANGELOG.rst` & `powerbox-0.7.2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/CONTRIBUTING.rst` & `powerbox-0.7.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/LICENSE.rst` & `powerbox-0.7.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/PKG-INFO` & `powerbox-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerbox
-Version: 0.7.1
+Version: 0.7.2
 Summary: Create arbitrary boxes with isotropic power spectra
 Author-email: Steven Murray <steven.g.murray@asu.edu>
 License: MIT
 Project-URL: repository, https://github.com/steven-murray/powerbox
 Project-URL: documentation, https://powerbox.readthedocs.io
 Keywords: power-spectrum,signal processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `powerbox-0.7.1/README.rst` & `powerbox-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/devel/hankel_transform_of_cosmo_power.ipynb` & `powerbox-0.7.2/devel/hankel_transform_of_cosmo_power.ipynb`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/devel/testing_angular_averaging.ipynb` & `powerbox-0.7.2/devel/testing_angular_averaging.ipynb`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/docs/Makefile` & `powerbox-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/docs/conf.py` & `powerbox-0.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/docs/demos/algorithm.ipynb` & `powerbox-0.7.2/docs/demos/algorithm.ipynb`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/docs/demos/cosmological_fields.ipynb` & `powerbox-0.7.2/docs/demos/cosmological_fields.ipynb`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/docs/demos/dft.ipynb` & `powerbox-0.7.2/docs/demos/dft.ipynb`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/docs/demos/getting_started.ipynb` & `powerbox-0.7.2/docs/demos/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/docs/templates/class.rst` & `powerbox-0.7.2/docs/templates/class.rst`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/docs/templates/modules.rst` & `powerbox-0.7.2/docs/templates/modules.rst`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/paper/Makefile` & `powerbox-0.7.2/paper/Makefile`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/paper/joss-logo.png` & `powerbox-0.7.2/paper/joss-logo.png`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/paper/latex.template` & `powerbox-0.7.2/paper/latex.template`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/paper/paper.aux` & `powerbox-0.7.2/paper/paper.aux`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/paper/paper.bcf` & `powerbox-0.7.2/paper/paper.bcf`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/paper/paper.bib` & `powerbox-0.7.2/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/paper/paper.log` & `powerbox-0.7.2/paper/paper.log`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/paper/paper.md` & `powerbox-0.7.2/paper/paper.md`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/paper/paper.pdf` & `powerbox-0.7.2/paper/paper.pdf`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/paper/paper.run.xml` & `powerbox-0.7.2/paper/paper.run.xml`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/paper/paper.tex` & `powerbox-0.7.2/paper/paper.tex`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/paper/paper.zip` & `powerbox-0.7.2/paper/paper.zip`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/pyproject.toml` & `powerbox-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/src/powerbox/__init__.py` & `powerbox-0.7.2/src/powerbox/__init__.py`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/src/powerbox/dft.py` & `powerbox-0.7.2/src/powerbox/dft.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 """
 import warnings
 
 __all__ = ["fft", "ifft", "fftfreq", "fftshift", "ifftshift"]
 
 # Try importing the pyFFTW interface
 try:
-
     from multiprocessing import cpu_count
 
     THREADS = cpu_count()
 
     from pyfftw.interfaces.cache import enable, set_keepalive_time
     from pyfftw.interfaces.numpy_fft import fftfreq as _fftfreq
     from pyfftw.interfaces.numpy_fft import fftn as _fftn
@@ -133,16 +132,16 @@
     else:
         if np.isscalar(Lk):
             Lk = Lk * np.ones(len(axes))
         L = N * 2 * np.pi / (Lk * b)  # Take account of the fourier convention.
 
     left_edge = _set_left_edge(left_edge, axes, L)
 
-    V = float(np.product(L))  # Volume of box
-    Vx = V / np.product(N)  # Volume of cell
+    V = float(np.prod(L))  # Volume of box
+    Vx = V / np.prod(N)  # Volume of cell
 
     ft = (
         Vx
         * fftshift(fftn(X, axes=axes), axes=axes)
         * np.sqrt(np.abs(b) / (2 * np.pi) ** (1 - a)) ** len(axes)
     )
 
@@ -229,25 +228,25 @@
 
     elif np.isscalar(Lk):
         Lk = [Lk] * len(axes)
 
     Lk = np.array(Lk)
     left_edge = _set_left_edge(left_edge, axes, Lk)
 
-    V = np.product(Lk)
+    V = np.prod(Lk)
     dk = np.array([float(lk) / float(n) for lk, n in zip(Lk, N)])
 
     ft = (
         V
         * ifftn(X, axes=axes)
         * np.sqrt(np.abs(b) / (2 * np.pi) ** (1 + a)) ** len(axes)
     )
     ft = ifftshift(ft, axes=axes)
 
-    freq = np.array([fftfreq(n, d=d, b=b) for n, d in zip(N, dk)])
+    freq = [fftfreq(n, d=d, b=b) for n, d in zip(N, dk)]
 
     ft = _adjust_phase(ft, left_edge, freq, axes, -b)
     return _retfunc(ft, freq, axes, ret_cubegrid)
 
 
 def _adjust_phase(ft, left_edge, freq, axes, b):
     for i, (l, f) in enumerate(zip(left_edge, freq)):
```

### Comparing `powerbox-0.7.1/src/powerbox/powerbox.py` & `powerbox-0.7.2/src/powerbox/powerbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,14 @@
         boxlength=1.0,
         ensure_physical=False,
         a=1.0,
         b=1.0,
         vol_normalised_power=True,
         seed=None,
     ):
-
         self.N = N
         self.dim = dim
         self.boxlength = boxlength
         self.L = boxlength
         self.fourier_a = a
         self.fourier_b = b
         self.vol_normalised_power = vol_normalised_power
@@ -292,15 +291,16 @@
             dimensions. Each row represents a single tracer's co-ordinates.
         """
         if delta_x is None:
             if self.seed is None:
                 warnings.warn(
                     "You Should provide `seed` at initialization if one"
                     " wants a correspondence between parent field and"
-                    " discrete samples."
+                    " discrete samples.",
+                    stacklevel=2,
                 )
             dx = self.delta_x()
         else:
             dx = delta_x
 
         dx = (dx + 1) * self.dx**self.dim * nbar
         n = dx
```

### Comparing `powerbox-0.7.1/src/powerbox/tools.py` & `powerbox-0.7.2/src/powerbox/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         coords = _magnitude_grid(coords)
 
     indx, bins, sumweight = _get_binweights(
         coords, weights, bins, average, bin_ave=bin_ave, log_bins=log_bins
     )
 
     if np.any(sumweight == 0):
-        warnings.warn("One or more radial bins had no cells within it.")
+        warnings.warn("One or more radial bins had no cells within it.", stacklevel=2)
 
     res = _field_average(indx, field, weights, sumweight)
 
     if get_variance:
         var = _field_variance(indx, field, res, weights, sumweight)
         return res, bins, var
     else:
@@ -131,15 +131,14 @@
     if dim is not None:
         return np.sqrt(np.sum(np.meshgrid(*([x**2] * dim)), axis=0))
     else:
         return np.sqrt(np.sum(np.meshgrid(*([X**2 for X in x])), axis=0))
 
 
 def _get_binweights(coords, weights, bins, average=True, bin_ave=True, log_bins=False):
-
     # Get a vector of bin edges
     bins = _getbins(bins, coords, log_bins)
 
     indx = np.digitize(coords.flatten(), bins)
 
     if average or bin_ave:
         if not np.isscalar(weights):
@@ -336,16 +335,16 @@
 
     coords = _magnitude_grid([c for i, c in enumerate(coords) if i < n])
 
     indx, bins, sumweights = _get_binweights(
         coords, weights, bins, average, bin_ave=bin_ave, log_bins=log_bins
     )
 
-    n1 = np.product(field.shape[:n])
-    n2 = np.product(field.shape[n:])
+    n1 = np.prod(field.shape[:n])
+    n2 = np.prod(field.shape[n:])
 
     res = np.zeros((len(sumweights), n2), dtype=field.dtype)
     if get_variance:
         var = np.zeros_like(res)
 
     for i, fld in enumerate(field.reshape((n1, n2)).T):
         try:
@@ -468,15 +467,14 @@
     >>> plt.plot(k,p)
     >>> plt.plot(k,k**-2.)
     >>> plt.xscale('log')
     >>> plt.yscale('log')
     """
     # Check if the input data is in sampled particle format
     if N is not None:
-
         if deltax.shape[1] > deltax.shape[0]:
             raise ValueError(
                 "It seems that there are more dimensions than particles! "
                 "Try transposing deltax."
             )
 
         if deltax2 is not None and deltax2.shape[1] > deltax2.shape[0]:
@@ -531,15 +529,15 @@
 
         if deltax2 is not None and deltax.shape != deltax2.shape:
             raise ValueError("deltax and deltax2 must have the same shape!")
 
         N = deltax.shape
         Npart1 = None
 
-    V = np.product(boxlength)
+    V = np.prod(boxlength)
 
     # Calculate the n-D power spectrum and align it with the k from powerbox.
     FT, freq, k = dft.fft(deltax, L=boxlength, a=a, b=b, ret_cubegrid=True)
 
     FT2 = dft.fft(deltax2, L=boxlength, a=a, b=b)[0] if deltax2 is not None else FT
     P = np.real(FT * np.conj(FT2) / V**2)
 
@@ -547,15 +545,15 @@
         P *= V
 
     if res_ndim is None:
         res_ndim = dim
 
     # Determine a nice number of bins.
     if bins is None:
-        bins = int(np.product(N[:res_ndim]) ** (1.0 / res_ndim) / 2.2)
+        bins = int(np.prod(N[:res_ndim]) ** (1.0 / res_ndim) / 2.2)
 
     # Set k_weights so that k=0 mode is ignore if desired.
     if ignore_zero_mode:
         kmag = _magnitude_grid([c for i, c in enumerate(freq) if i < res_ndim])
         if np.isscalar(k_weights):
             k_weights = np.ones_like(kmag)
```

### Comparing `powerbox-0.7.1/src/powerbox.egg-info/PKG-INFO` & `powerbox-0.7.2/src/powerbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerbox
-Version: 0.7.1
+Version: 0.7.2
 Summary: Create arbitrary boxes with isotropic power spectra
 Author-email: Steven Murray <steven.g.murray@asu.edu>
 License: MIT
 Project-URL: repository, https://github.com/steven-murray/powerbox
 Project-URL: documentation, https://powerbox.readthedocs.io
 Keywords: power-spectrum,signal processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `powerbox-0.7.1/src/powerbox.egg-info/SOURCES.txt` & `powerbox-0.7.2/src/powerbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/tests/test_direct.py` & `powerbox-0.7.2/tests/test_direct.py`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/tests/test_discrete.py` & `powerbox-0.7.2/tests/test_discrete.py`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/tests/test_fft.py` & `powerbox-0.7.2/tests/test_fft.py`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/tests/test_lognormal.py` & `powerbox-0.7.2/tests/test_lognormal.py`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/tests/test_power.py` & `powerbox-0.7.2/tests/test_power.py`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/tests/test_stats.py` & `powerbox-0.7.2/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `powerbox-0.7.1/tests/test_tools.py` & `powerbox-0.7.2/tests/test_tools.py`

 * *Files identical despite different names*

