# Comparing `tmp/robotframework_jupyterlibrary-0.5.0.tar.gz` & `tmp/robotframework_jupyterlibrary-0.5.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_jupyterlibrary-0.5.0.tar", last modified: Fri Jul 21 13:01:44 2023, max compression
+gzip compressed data, was "robotframework_jupyterlibrary-0.5.0a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `robotframework_jupyterlibrary-0.5.0.tar` & `robotframework_jupyterlibrary-0.5.0a0.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0       25 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.binder/apt.txt
--rw-r--r--   0        0        0       52 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.binder/labex.txt
--rw-r--r--   0        0        0      382 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.binder/postBuild
--rw-r--r--   0        0        0     2573 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      739 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/ISSUE_TEMPLATE/docs.md
--rw-r--r--   0        0        0      572 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      903 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/ISSUE_TEMPLATE/release.md
--rw-r--r--   0        0        0      275 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/env_specs/_base.yml
--rw-r--r--   0        0        0      240 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/env_specs/docs.yml
--rw-r--r--   0        0        0      339 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/env_specs/lab3.yml
--rw-r--r--   0        0        0      266 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/env_specs/lab4.yml
--rw-r--r--   0        0        0      122 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/env_specs/lint.yml
--rw-r--r--   0        0        0      259 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/env_specs/meta.yml
--rw-r--r--   0        0        0      122 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/env_specs/py3.11.yml
--rw-r--r--   0        0        0      155 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/env_specs/py3.8.yml
--rw-r--r--   0        0        0       56 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/env_specs/test-py3.7.yml
--rw-r--r--   0        0        0      116 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/env_specs/test.yml
--rw-r--r--   0        0        0    16455 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/docs/linux-64/conda.lock
--rw-r--r--   0        0        0    15689 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/docs/osx-64/conda.lock
--rw-r--r--   0        0        0    15622 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/docs/win-64/conda.lock
--rw-r--r--   0        0        0     9809 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/lint/linux-64/conda.lock
--rw-r--r--   0        0        0     8943 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/lint/osx-64/conda.lock
--rw-r--r--   0        0        0     9106 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/lint/win-64/conda.lock
--rw-r--r--   0        0        0    19778 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/meta/linux-64/conda.lock
--rw-r--r--   0        0        0    18602 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/meta/osx-64/conda.lock
--rw-r--r--   0        0        0    18567 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/meta/win-64/conda.lock
--rw-r--r--   0        0        0    19615 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/test/linux-64/py3.11/lab3/conda.lock
--rw-r--r--   0        0        0    18203 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/test/linux-64/py3.11/lab4/conda.lock
--rw-r--r--   0        0        0    18924 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/test/linux-64/py3.8/lab3/conda.lock
--rw-r--r--   0        0        0    17513 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/test/linux-64/py3.8/lab4/conda.lock
--rw-r--r--   0        0        0    18974 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/test/osx-64/py3.11/lab3/conda.lock
--rw-r--r--   0        0        0    17676 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/test/osx-64/py3.11/lab4/conda.lock
--rw-r--r--   0        0        0    18281 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/test/osx-64/py3.8/lab3/conda.lock
--rw-r--r--   0        0        0    16984 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/test/osx-64/py3.8/lab4/conda.lock
--rw-r--r--   0        0        0    18771 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/test/win-64/py3.11/lab3/conda.lock
--rw-r--r--   0        0        0    17473 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/test/win-64/py3.11/lab4/conda.lock
--rw-r--r--   0        0        0    18078 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/test/win-64/py3.8/lab3/conda.lock
--rw-r--r--   0        0        0    16781 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/locks/test/win-64/py3.8/lab4/conda.lock
--rw-r--r--   0        0        0      912 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/pull_request_template.md
--rw-r--r--   0        0        0     1158 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/recipe/meta.yaml.in
--rw-r--r--   0        0        0     5766 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      190 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.gitignore
--rw-r--r--   0        0        0      313 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/.readthedocs.yml
--rw-r--r--   0        0        0     3358 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1506 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/LICENSE
--rw-r--r--   0        0        0     3858 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/README.md
--rw-r--r--   0        0        0       27 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/_scripts/__init__.py
--rw-r--r--   0        0        0     4888 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/_scripts/atest.py
--rw-r--r--   0        0        0      905 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/_scripts/combine.py
--rw-r--r--   0        0        0     1082 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/_scripts/lint.py
--rw-r--r--   0        0        0     2426 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/_scripts/lock.py
--rw-r--r--   0        0        0     9959 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/_scripts/project.py
--rw-r--r--   0        0        0     1401 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/_scripts/reporter.py
--rw-r--r--   0        0        0      222 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/atest/00_smoke/00_import.robot
--rw-r--r--   0        0        0     3128 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/atest/01_server/00_basic.robot
--rw-r--r--   0        0        0      546 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/atest/__init__.robot
--rw-r--r--   0        0        0     1100 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/atest/classic/10_notebook.robot
--rw-r--r--   0        0        0      418 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/atest/classic/__init__.robot
--rw-r--r--   0        0        0      590 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/atest/lab/00_shell.robot
--rw-r--r--   0        0        0     2495 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/atest/lab/10_notebook.robot
--rw-r--r--   0        0        0     1565 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/atest/lab/20_magic.robot
--rw-r--r--   0        0        0      866 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/atest/lab/30_settings.robot
--rw-r--r--   0        0        0     2408 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/atest/lab/__init__.robot
--rw-r--r--   0        0        0     1035 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/atest/notebook/10_notebook.robot
--rw-r--r--   0        0        0      468 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/atest/notebook/__init__.robot
--rw-r--r--   0        0        0    10986 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/docs/CI.ipynb
--rw-r--r--   0        0        0     7686 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/docs/HISTORY.ipynb
--rw-r--r--   0        0        0     3808 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/docs/INSTALL.ipynb
--rw-r--r--   0        0        0     3750 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/docs/KEYWORDS.ipynb
--rw-r--r--   0        0        0     2163 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/docs/LIMITS.ipynb
--rw-r--r--   0        0        0     5020 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/docs/MAGIC.ipynb
--rw-r--r--   0        0        0     2387 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/docs/WHY.ipynb
--rw-r--r--   0        0        0     1175 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/docs/_static/anvil.svg
--rw-r--r--   0        0        0     1654 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/docs/_static/css/custom.css
--rw-r--r--   0        0        0     6452 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/docs/_static/fonts/OCRA.woff2
--rw-r--r--   0        0        0     9212 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/docs/conf.py
--rw-r--r--   0        0        0      881 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/docs/index.ipynb
--rw-r--r--   0        0        0    17199 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/docs/rtd.yml
--rw-r--r--   0        0        0    18176 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/dodo.py
--rw-r--r--   0        0        0      313 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/package.json
--rw-r--r--   0        0        0     3006 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      391 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/__init__.py
--rw-r--r--   0        0        0      131 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/_version.py
--rw-r--r--   0        0        0      485 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/README.md
--rw-r--r--   0        0        0      552 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/classic/Commands.resource
--rw-r--r--   0        0        0     1140 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/classic/Notebook.resource
--rw-r--r--   0        0        0     1946 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/classic/Output.resource
--rw-r--r--   0        0        0     1708 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/classic/Selectors.resource
--rw-r--r--   0        0        0     1735 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/classic/Tree.resource
--rw-r--r--   0        0        0     2028 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Commands.resource
--rw-r--r--   0        0        0     2068 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Icons.resource
--rw-r--r--   0        0        0     1146 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Launcher.resource
--rw-r--r--   0        0        0     2609 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Notebook.resource
--rw-r--r--   0        0        0     2087 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Output.resource
--rw-r--r--   0        0        0     2679 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/PageInfo.resource
--rw-r--r--   0        0        0     3864 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Selectors.resource
--rw-r--r--   0        0        0     3133 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Settings.resource
--rw-r--r--   0        0        0     4412 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Shell.resource
--rw-r--r--   0        0        0      705 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Shortcuts.resource
--rw-r--r--   0        0        0      712 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Sidebar.resource
--rw-r--r--   0        0        0     1219 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Version.resource
--rw-r--r--   0        0        0      546 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/notebook/Commands.resource
--rw-r--r--   0        0        0     1207 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/notebook/Notebook.resource
--rw-r--r--   0        0        0     1891 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/notebook/Output.resource
--rw-r--r--   0        0        0     2449 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/notebook/Selectors.resource
--rw-r--r--   0        0        0     2046 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/notebook/Tree.resource
--rw-r--r--   0        0        0     3556 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/common/CodeMirror.resource
--rw-r--r--   0        0        0      450 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/common/Lumino.resource
--rw-r--r--   0        0        0       94 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/constants.py
--rw-r--r--   0        0        0     2586 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/core.py
--rw-r--r--   0        0        0       75 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/keywords/__init__.py
--rw-r--r--   0        0        0    13787 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/keywords/server.py
--rw-r--r--   0        0        0     1224 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/keywords/webelements.py
--rw-r--r--   0        0        0     6948 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/magic.py
--rw-r--r--   0        0        0      342 2023-07-21 13:01:44.000000 robotframework_jupyterlibrary-0.5.0/yarn.lock
--rw-r--r--   0        0        0     5822 1970-01-01 00:00:00.000000 robotframework_jupyterlibrary-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.binder/apt.txt
+-rw-r--r--   0        0        0       52 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.binder/labex.txt
+-rw-r--r--   0        0        0      382 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.binder/postBuild
+-rw-r--r--   0        0        0     2573 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      739 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0        0        0      572 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      903 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/ISSUE_TEMPLATE/release.md
+-rw-r--r--   0        0        0      310 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/_base.yml
+-rw-r--r--   0        0        0      172 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/docs.yml
+-rw-r--r--   0        0        0      339 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/lab3.yml
+-rw-r--r--   0        0        0      268 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/lab4.yml
+-rw-r--r--   0        0        0      122 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/lint.yml
+-rw-r--r--   0        0        0      257 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/meta.yml
+-rw-r--r--   0        0        0      122 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/py3.11.yml
+-rw-r--r--   0        0        0      155 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/py3.8.yml
+-rw-r--r--   0        0        0       56 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/test-py3.7.yml
+-rw-r--r--   0        0        0      116 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/test.yml
+-rw-r--r--   0        0        0    16815 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/docs/linux-64/conda.lock
+-rw-r--r--   0        0        0    16034 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/docs/osx-64/conda.lock
+-rw-r--r--   0        0        0    15961 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/docs/win-64/conda.lock
+-rw-r--r--   0        0        0    10412 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/lint/linux-64/conda.lock
+-rw-r--r--   0        0        0     9531 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/lint/osx-64/conda.lock
+-rw-r--r--   0        0        0     9688 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/lint/win-64/conda.lock
+-rw-r--r--   0        0        0    19331 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/meta/linux-64/conda.lock
+-rw-r--r--   0        0        0    18146 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/meta/osx-64/conda.lock
+-rw-r--r--   0        0        0    18114 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/meta/win-64/conda.lock
+-rw-r--r--   0        0        0    19865 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/linux-64/py3.11/lab3/conda.lock
+-rw-r--r--   0        0        0    18584 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/linux-64/py3.11/lab4/conda.lock
+-rw-r--r--   0        0        0    19058 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/linux-64/py3.8/lab3/conda.lock
+-rw-r--r--   0        0        0    17778 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/linux-64/py3.8/lab4/conda.lock
+-rw-r--r--   0        0        0    19323 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/osx-64/py3.11/lab3/conda.lock
+-rw-r--r--   0        0        0    18046 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/osx-64/py3.11/lab4/conda.lock
+-rw-r--r--   0        0        0    18514 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/osx-64/py3.8/lab3/conda.lock
+-rw-r--r--   0        0        0    17238 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/osx-64/py3.8/lab4/conda.lock
+-rw-r--r--   0        0        0    19110 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/win-64/py3.11/lab3/conda.lock
+-rw-r--r--   0        0        0    17833 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/win-64/py3.11/lab4/conda.lock
+-rw-r--r--   0        0        0    18301 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/win-64/py3.8/lab3/conda.lock
+-rw-r--r--   0        0        0    17025 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/win-64/py3.8/lab4/conda.lock
+-rw-r--r--   0        0        0      912 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/pull_request_template.md
+-rw-r--r--   0        0        0      994 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/recipe/meta.yaml.in
+-rw-r--r--   0        0        0     5766 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      190 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.gitignore
+-rw-r--r--   0        0        0      313 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.readthedocs.yml
+-rw-r--r--   0        0        0     3358 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1506 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/LICENSE
+-rw-r--r--   0        0        0     3858 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/README.md
+-rw-r--r--   0        0        0       27 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/_scripts/__init__.py
+-rw-r--r--   0        0        0     4888 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/_scripts/atest.py
+-rw-r--r--   0        0        0      905 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/_scripts/combine.py
+-rw-r--r--   0        0        0     1082 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/_scripts/lint.py
+-rw-r--r--   0        0        0     2426 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/_scripts/lock.py
+-rw-r--r--   0        0        0     9650 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/_scripts/project.py
+-rw-r--r--   0        0        0     1324 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/_scripts/reporter.py
+-rw-r--r--   0        0        0      222 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/00_smoke/00_import.robot
+-rw-r--r--   0        0        0     3128 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/01_server/00_basic.robot
+-rw-r--r--   0        0        0      546 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/__init__.robot
+-rw-r--r--   0        0        0     1100 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/classic/10_notebook.robot
+-rw-r--r--   0        0        0      418 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/classic/__init__.robot
+-rw-r--r--   0        0        0      590 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/lab/00_shell.robot
+-rw-r--r--   0        0        0     2495 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/lab/10_notebook.robot
+-rw-r--r--   0        0        0     1565 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/lab/20_magic.robot
+-rw-r--r--   0        0        0      866 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/lab/30_settings.robot
+-rw-r--r--   0        0        0     2408 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/lab/__init__.robot
+-rw-r--r--   0        0        0     1035 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/notebook/10_notebook.robot
+-rw-r--r--   0        0        0      468 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/notebook/__init__.robot
+-rw-r--r--   0        0        0    10986 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/CI.ipynb
+-rw-r--r--   0        0        0     7065 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/HISTORY.ipynb
+-rw-r--r--   0        0        0     3808 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/INSTALL.ipynb
+-rw-r--r--   0        0        0     3750 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/KEYWORDS.ipynb
+-rw-r--r--   0        0        0     2163 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/LIMITS.ipynb
+-rw-r--r--   0        0        0     5020 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/MAGIC.ipynb
+-rw-r--r--   0        0        0     2387 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/WHY.ipynb
+-rw-r--r--   0        0        0     1175 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/_static/anvil.svg
+-rw-r--r--   0        0        0     1654 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/_static/css/custom.css
+-rw-r--r--   0        0        0     6452 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/_static/fonts/OCRA.woff2
+-rw-r--r--   0        0        0     9212 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/conf.py
+-rw-r--r--   0        0        0      881 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/index.ipynb
+-rw-r--r--   0        0        0    17571 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/rtd.yml
+-rw-r--r--   0        0        0    17991 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/dodo.py
+-rw-r--r--   0        0        0      313 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/package.json
+-rw-r--r--   0        0        0     3008 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/pyproject.toml
+-rw-r--r--   0        0        0      391 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/__init__.py
+-rw-r--r--   0        0        0      131 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/_version.py
+-rw-r--r--   0        0        0      485 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/README.md
+-rw-r--r--   0        0        0      593 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/classic/Commands.resource
+-rw-r--r--   0        0        0     1140 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/classic/Notebook.resource
+-rw-r--r--   0        0        0     1946 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/classic/Output.resource
+-rw-r--r--   0        0        0     1708 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/classic/Selectors.resource
+-rw-r--r--   0        0        0     1735 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/classic/Tree.resource
+-rw-r--r--   0        0        0     2028 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Commands.resource
+-rw-r--r--   0        0        0     2068 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Icons.resource
+-rw-r--r--   0        0        0     1146 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Launcher.resource
+-rw-r--r--   0        0        0     2609 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Notebook.resource
+-rw-r--r--   0        0        0     2087 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Output.resource
+-rw-r--r--   0        0        0     2679 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/PageInfo.resource
+-rw-r--r--   0        0        0     3864 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Selectors.resource
+-rw-r--r--   0        0        0     3133 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Settings.resource
+-rw-r--r--   0        0        0     4412 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Shell.resource
+-rw-r--r--   0        0        0      705 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Shortcuts.resource
+-rw-r--r--   0        0        0      712 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Sidebar.resource
+-rw-r--r--   0        0        0     1219 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Version.resource
+-rw-r--r--   0        0        0      587 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/notebook/Commands.resource
+-rw-r--r--   0        0        0     1207 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/notebook/Notebook.resource
+-rw-r--r--   0        0        0     1891 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/notebook/Output.resource
+-rw-r--r--   0        0        0     2394 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/notebook/Selectors.resource
+-rw-r--r--   0        0        0     1974 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/notebook/Tree.resource
+-rw-r--r--   0        0        0     3556 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/common/CodeMirror.resource
+-rw-r--r--   0        0        0      450 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/common/Lumino.resource
+-rw-r--r--   0        0        0       94 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/constants.py
+-rw-r--r--   0        0        0     2586 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/core.py
+-rw-r--r--   0        0        0       75 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/keywords/__init__.py
+-rw-r--r--   0        0        0    13479 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/keywords/server.py
+-rw-r--r--   0        0        0     1224 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/keywords/webelements.py
+-rw-r--r--   0        0        0     6948 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/magic.py
+-rw-r--r--   0        0        0      342 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/yarn.lock
+-rw-r--r--   0        0        0     5824 1970-01-01 00:00:00.000000 robotframework_jupyterlibrary-0.5.0a0/PKG-INFO
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `robotframework_jupyterlibrary-0.5.0a0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/ISSUE_TEMPLATE/docs.md` & `robotframework_jupyterlibrary-0.5.0a0/.github/ISSUE_TEMPLATE/docs.md`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md` & `robotframework_jupyterlibrary-0.5.0a0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/ISSUE_TEMPLATE/release.md` & `robotframework_jupyterlibrary-0.5.0a0/.github/ISSUE_TEMPLATE/release.md`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/docs/linux-64/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/docs/linux-64/conda.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,76 +1,81 @@
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
 https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.1.0-hfd8a6a1_0.conda#067bcc23164642f4c226da631f2a2e1d
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-12.2.0-h46fd767_19.tar.bz2#1030b1f38c129f2634eae026f704fe60
 https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.11-3_cp311.conda#c2e2630ddb68cf52eec74dc7dfab20b5
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-12.2.0-h65d4601_19.tar.bz2#cedcee7c064c01c403f962c9e8d3c373
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-12.2.0-h65d4601_19.tar.bz2#e4c94f80aef025c17ab0828cd85ef535
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
 https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2#9194c9bf9428035a05352d031462eae4
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
 https://conda.anaconda.org/conda-forge/linux-64/libuv-1.44.2-h166bdaf_0.tar.bz2#e5cb4fe581a18ca2185a016eb848fc00
-https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
-https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
+https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-h166bdaf_4.tar.bz2#f3f9de449d32ca9b9c66a22863c96f41
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h27087fc_1.tar.bz2#4acfc691e64342b9dae57cf2adc63238
 https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
 https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
 https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2#4ae4d7795d33e02bd20f6b23d91caf82
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2#04bac51ba35ea023dc48af73c1c88c25
 https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
-https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
-https://conda.anaconda.org/conda-forge/linux-64/nodejs-18.16.1-hf52ce11_0.conda#23ed78db48ed08c94e5449f6661d65e6
-https://conda.anaconda.org/conda-forge/linux-64/python-3.11.4-hab00c5b_0_cpython.conda#1c628861a2a126b9fc9363ca1b7d014e
+https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-h166bdaf_4.tar.bz2#4b11e365c0275b808be78b30f904e295
+https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2#e5613f2bc717e9945840ff474419b8e4
+https://conda.anaconda.org/conda-forge/linux-64/nodejs-18.15.0-h4abf6b9_1.conda#2aabafd88f6876a57c45c00598715ac4
+https://conda.anaconda.org/conda-forge/linux-64/python-3.11.3-h2755cc3_0_cpython.conda#37005ea5f68df6a8a381b70cf4d4a160
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
+https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.0.9-py311ha362b79_9.conda#ced5340f5dc6cff43a80deac8d0e398f
+https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_8.tar.bz2#2ff08978892a3e8b954397c461f18418
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
-https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-unix_pyh707e725_0.conda#64dbb3b205546691a61204d1cfb208e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
+https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py311hcafe171_0.conda#f4c810ad9d791c8df5ad900ed74b085b
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/linux-64/docutils-0.19-py311h38be061_1.tar.bz2#599159b0740e9b82e7eef0e8471be3c2
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/linux-64/greenlet-2.0.2-py311hb755f60_1.conda#82f9885f18cc7ba9bca6687ac97f1d65
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
-https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py311h459d7ec_0.conda#9904dc4adb5d547cb21e136f98cb24b0
+https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.2-py311h2582759_0.conda#adb20bd57069614552adac60a020c36d
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/port-for-0.7.1-pyhd8ed1ab_0.conda#911d5daac0d579dc7aa4d85050ccd548
+https://conda.anaconda.org/conda-forge/noarch/port-for-0.6.3-pyhd8ed1ab_0.conda#cfc0df39511f323ad3d999203d86fe8d
 https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py311h2582759_0.conda#a90f8e278c1cd7064b2713e6b7db87e6
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
+https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py311h2582759_0.conda#e53876b66dcc4ba8a0afa63cd8502ac3
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py311hd4cff14_5.tar.bz2#da8769492e423103c59f469f4f17f8d9
 https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py311h75c88c4_0.conda#db94a7a9e865fbfde8c023b6e8958bb2
-https://conda.anaconda.org/conda-forge/noarch/robotframework-6.1-pyhd8ed1ab_0.conda#e383bebdc0d8fea4ecf9c9e01d0959fe
-https://conda.anaconda.org/conda-forge/linux-64/rpds-py-0.9.2-py311h46250e7_0.conda#bcf66b5abaec47198b42cdd0bb968540
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/noarch/robotframework-6.0.2-pyhd8ed1ab_1.conda#b4dcead8c5a99a14733d9b1ba5b7db09
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.4-pyhd8ed1ab_0.conda#5a31a7d564f551d0e6dff52fd8cb5b16
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
@@ -79,64 +84,62 @@
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/tabulate-0.9.0-pyhd8ed1ab_1.tar.bz2#4759805cce2d914c38472f70bf4d8bcb
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py311h459d7ec_0.conda#12b1c374ee90a1aa11ea921858394dc8
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.30.0-pyhd8ed1ab_0.conda#13bf095e3ecd18999d65b4d3ac5b15d5
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.2.0-pyhd8ed1ab_0.conda#c9e9064ab45ffb46f7a96834d9e7626d
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.4-pyhd8ed1ab_0.conda#18badd8fa3648d1beb1fcc7f2e0f756e
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.2-pyhd8ed1ab_0.conda#81a763f3c64fe6d5f32e033b0325265d
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.7.1-pyhd8ed1ab_0.conda#7c27ea1bdbe520bb830dcadd59f55cbf
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.3.5-pyhd8ed1ab_0.conda#9eeb66a24c8f6d950eb55a9f1128da20
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-2.0.19-py311h459d7ec_0.conda#9970b757e599b1b845fedd25c8d6fc7a
+https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-2.0.15-py311h459d7ec_0.conda#d2199e4c33e24003103845ab9b07469e
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.2-py311h38be061_0.conda#dcbfe3a95e8b99ec743e26a75d8c9cf4
+https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.0-py311h38be061_1.tar.bz2#0564e63c41c0527f8085a572a931f1e6
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.18.4-pyhd8ed1ab_0.conda#7356151a32ebd9a20158d2f26d224bfa
-https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.1-py311h38be061_0.conda#0cf8259b01ede82c76007996f73f89ed
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
+https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.0-py311h38be061_0.conda#1dd43a18a75d59206019e2a2a28555e5
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
 https://conda.anaconda.org/conda-forge/noarch/sphinx-5.3.0-pyhd8ed1ab_0.tar.bz2#f9e1fcfe235d655900bfeb6aee426472
-https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
+https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.2-pyhd8ed1ab_0.conda#4ec732d2264373773a5feaea477128a8
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.8.0-pyhd8ed1ab_0.conda#1ca43103a08456b19222d93fd9d119ac
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
 https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2021.3.14-pyhd8ed1ab_0.tar.bz2#1909f784dc37b4ab97afe2c95aeeabaa
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
-https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh41d4057_0.conda#0a0b0d8177c4a209017b356439292db8
+https://conda.anaconda.org/conda-forge/noarch/ipython-8.13.2-pyh41d4057_0.conda#e8563c13eee80a5f1c7bdfc2a1b20077
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda#f7aa15f77d29b11caa1df1eb15383c59
-https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh71e2992_0.conda#cfafc9387c32a43a1b6d63633489cbc9
+https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_0.conda#15700afca8f7ab35542e9c1af63568f1
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh210e3f2_0.conda#4b57b688e22d094d1479a35543c18e93
 https://conda.anaconda.org/conda-forge/noarch/jupyter-cache-0.6.1-pyhd8ed1ab_0.conda#2e360820ae68e3d28e1a5a9d2714ca5c
 https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda#40190b7d06f86b63d28fa78aaa39c023
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/docs/osx-64/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/docs/win-64/conda.lock`

 * *Files 5% similar despite different names*

```diff
@@ -1,136 +1,138 @@
 @EXPLICIT
-https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
-https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
-https://conda.anaconda.org/conda-forge/osx-64/icu-72.1-h7336db1_0.conda#c9689510a50a4bb2ae978421671a125e
-https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
-https://conda.anaconda.org/conda-forge/osx-64/libexpat-2.5.0-hf0c8a7f_1.conda#6c81cb022780ee33435cca0127dd43c9
-https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
-https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2#24632c09ed931af617fe6d5292919cab
-https://conda.anaconda.org/conda-forge/osx-64/libuv-1.44.2-hac89ed1_0.tar.bz2#958fa9add5701462a6c91e3774425ea1
-https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
-https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
-https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.11-3_cp311.conda#5e0a069a585445333868d2c6651c3b3f
+https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2023.5.7-h56e8100_0.conda#604212634bd8c4d6f20d44b946e8eedb
+https://conda.anaconda.org/conda-forge/win-64/libexpat-2.5.0-h63175ca_1.conda#636cc3cbbd2e28bcfd2f73b2044aac2c
+https://conda.anaconda.org/conda-forge/win-64/nodejs-18.15.0-h57928b3_1.conda#d728bbdc9a650a5d503d657ce12c01ce
+https://conda.anaconda.org/conda-forge/win-64/python_abi-3.11-3_cp311.conda#fd1634ba85cfea9376e1fc02d6f592e9
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
-https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
-https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
-https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
-https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
-https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
-https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
-https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
-https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-h8a1eda9_5.conda#75a8a98b1c4671c5d2897975731da42d
-https://conda.anaconda.org/conda-forge/osx-64/nodejs-18.16.1-h46e3395_0.conda#e4c06702959edec36072a3d081af4587
-https://conda.anaconda.org/conda-forge/osx-64/python-3.11.4-h30d4d87_0_cpython.conda#e40b3075f85db0184d5f61d17c580ef7
+https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
+https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.34.31931-h5081d32_16.conda#22125178654c6a8a393f9743d585704b
+https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hb25d44b_16.conda#ea326b37e3bd6d2616988e09f3a9396c
+https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.34.31931-hed1258a_16.conda#0374eae69b6dbfb27c3dc27167109eb4
+https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
+https://conda.anaconda.org/conda-forge/win-64/libbrotlicommon-1.0.9-hcfcfb64_8.tar.bz2#e8078e37208cd7d3e1eb5053f370ded8
+https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
+https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2#5c1fb45b5e2912c19098750ae8a32604
+https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.42.0-hcfcfb64_0.conda#9a71d93deb99cc09d8939d5235b5909a
+https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_4.tar.bz2#0cc5c5cc64ee1637f37f8540a175854c
+https://conda.anaconda.org/conda-forge/win-64/openssl-3.1.1-hcfcfb64_1.conda#1d913a5de46c6b2f7e4cfbd26b106b8b
+https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2#c69a5047cc9291ae40afd4a1ad6f0c0f
+https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
+https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
+https://conda.anaconda.org/conda-forge/win-64/libbrotlidec-1.0.9-hcfcfb64_8.tar.bz2#99839d9d81f33afa173c0fa82a702038
+https://conda.anaconda.org/conda-forge/win-64/libbrotlienc-1.0.9-hcfcfb64_8.tar.bz2#88e62627120c20289bf8982b15e0a6a1
+https://conda.anaconda.org/conda-forge/win-64/python-3.11.3-h2628c8c_0_cpython.conda#8f82e0e0ba51bed311f28eb6450393f6
+https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.4-h0e60522_1.tar.bz2#e1aff0583dda5fb917eb3d2c1025aa80
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
-https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
+https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.0.9-py311h814d153_9.conda#034ddcc806d421524fbc46778447e87c
+https://conda.anaconda.org/conda-forge/win-64/brotli-bin-1.0.9-hcfcfb64_8.tar.bz2#e18b70ed349d96086fd60a9c642b1b58
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
-https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-unix_pyh707e725_0.conda#64dbb3b205546691a61204d1cfb208e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
-https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.7-py311h814d153_0.conda#c27802860b87fe024c9b6276205a56b5
+https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.7-py311h12c1d0e_0.conda#b056c7299be929b711016d2f4e48d303
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
-https://conda.anaconda.org/conda-forge/osx-64/docutils-0.19-py311h6eed73b_1.tar.bz2#268664c5447607a94cd67a0be91f83cd
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
+https://conda.anaconda.org/conda-forge/win-64/docutils-0.19-py311h1ea47a8_1.tar.bz2#52b2142036004451e1881d97e9d01e8a
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
-https://conda.anaconda.org/conda-forge/osx-64/greenlet-2.0.2-py311hdf8f085_1.conda#58ebad2ba8dc2225237ebd7d7c3111d2
+https://conda.anaconda.org/conda-forge/win-64/greenlet-2.0.2-py311h12c1d0e_1.conda#07ff18c128d8f3cea2d077a431658456
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
-https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.3-py311h2725bcf_0.conda#65b70928fcc2a81891ad1a8a6a7b085a
+https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.2-py311ha68e1ae_0.conda#96e7ffe6ea438ba4517152abe3b39874
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/port-for-0.7.1-pyhd8ed1ab_0.conda#911d5daac0d579dc7aa4d85050ccd548
-https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.5-py311h5547dcb_0.conda#d9b4565309f4f992b42bd99031044642
-https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
+https://conda.anaconda.org/conda-forge/noarch/port-for-0.6.3-pyhd8ed1ab_0.conda#cfc0df39511f323ad3d999203d86fe8d
+https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.5-py311ha68e1ae_0.conda#f1a1eecd1bb4f431df5b9b6d8a152efd
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
+https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
-https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
+https://conda.anaconda.org/conda-forge/win-64/pyrsistent-0.19.3-py311ha68e1ae_0.conda#3f2780a49f0b4bb2c622f7cf098e3d06
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
-https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py311h5547dcb_5.tar.bz2#8d1e456914ce961119b07f396187a564
-https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.0-py311h5dacc12_0.conda#1f65b37886e7cb8476d48ea8bb9d19c0
-https://conda.anaconda.org/conda-forge/noarch/robotframework-6.1-pyhd8ed1ab_0.conda#e383bebdc0d8fea4ecf9c9e01d0959fe
-https://conda.anaconda.org/conda-forge/osx-64/rpds-py-0.9.2-py311h299eb51_0.conda#bda1d1d8fce204234ed183b150dd51cc
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/win-64/pywin32-304-py311h12c1d0e_2.tar.bz2#20a2d8e73b0be8e27ca4096d4f3a7053
+https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py311ha68e1ae_5.tar.bz2#0c97d59d54eb52e170224b3de6ade906
+https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.0-py311h7b3f143_0.conda#b690f6e1878ccc98e96a33658867e8e1
+https://conda.anaconda.org/conda-forge/noarch/robotframework-6.0.2-pyhd8ed1ab_1.conda#b4dcead8c5a99a14733d9b1ba5b7db09
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.4-pyhd8ed1ab_0.conda#5a31a7d564f551d0e6dff52fd8cb5b16
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.1-pyhd8ed1ab_0.conda#6c8c4d6eb2325e59290ac6dbbeacd5f0
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/tabulate-0.9.0-pyhd8ed1ab_1.tar.bz2#4759805cce2d914c38472f70bf4d8bcb
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
-https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py311h2725bcf_0.conda#276fe4341e39dcd9d9d33ca18140d2e7
+https://conda.anaconda.org/conda-forge/win-64/tornado-6.3.2-py311ha68e1ae_0.conda#e2a6c106c1cff7e884d93351cdee3c3e
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
+https://conda.anaconda.org/conda-forge/win-64/brotli-1.0.9-hcfcfb64_8.tar.bz2#2e661f21e1741c11506bdc7226e6b0bc
+https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py311h7d9ee11_3.conda#a8524727eb956b4741e25a64af79edb8
+https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-win_pyhd8ed1ab_2.tar.bz2#6b58680207b526c42dcff68b543803dd
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
-https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.30.0-pyhd8ed1ab_0.conda#13bf095e3ecd18999d65b4d3ac5b15d5
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.2.0-pyhd8ed1ab_0.conda#c9e9064ab45ffb46f7a96834d9e7626d
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.4-pyhd8ed1ab_0.conda#18badd8fa3648d1beb1fcc7f2e0f756e
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.7.1-pyhd8ed1ab_0.conda#7c27ea1bdbe520bb830dcadd59f55cbf
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.3.5-pyhd8ed1ab_0.conda#9eeb66a24c8f6d950eb55a9f1128da20
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
-https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/osx-64/sqlalchemy-2.0.19-py311h2725bcf_0.conda#a7a513f1a4945836be346940b6229e88
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
+https://conda.anaconda.org/conda-forge/win-64/sqlalchemy-2.0.15-py311ha68e1ae_0.conda#2e9495eb648eb49ee000a535372187ff
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/osx-64/trio-0.22.2-py311h6eed73b_0.conda#6ceb2138c6038d75a92b06d3f8fd9ece
+https://conda.anaconda.org/conda-forge/win-64/trio-0.22.0-py311h1ea47a8_1.tar.bz2#1475d3775d4e2cc09c366720de842992
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.2-pyhd8ed1ab_0.conda#81a763f3c64fe6d5f32e033b0325265d
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
+https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.3.0-py311h1ea47a8_0.conda#2b81965b74e70b89053845d1bc287561
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
+https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.2-pyhd8ed1ab_0.conda#4ec732d2264373773a5feaea477128a8
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.18.4-pyhd8ed1ab_0.conda#7356151a32ebd9a20158d2f26d224bfa
-https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.1-py311h6eed73b_0.conda#2d45628b123595054093ff65996b98ae
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.8.0-pyhd8ed1ab_0.conda#1ca43103a08456b19222d93fd9d119ac
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
 https://conda.anaconda.org/conda-forge/noarch/sphinx-5.3.0-pyhd8ed1ab_0.tar.bz2#f9e1fcfe235d655900bfeb6aee426472
-https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
+https://conda.anaconda.org/conda-forge/noarch/ipython-8.13.2-pyh08f2357_0.conda#aebd5e79c0f354cdbceb055cdec53659
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
+https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda#f7aa15f77d29b11caa1df1eb15383c59
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
-https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
+https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_0.conda#15700afca8f7ab35542e9c1af63568f1
 https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2021.3.14-pyhd8ed1ab_0.tar.bz2#1909f784dc37b4ab97afe2c95aeeabaa
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
-https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyhd1c38e8_0.conda#f56fab4cea853c2248105b6cd7d79bf0
-https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda#f7aa15f77d29b11caa1df1eb15383c59
-https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh5fb750a_0.conda#2a8ffa559d393fea47237b9d23ddf74f
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh025b116_0.conda#d18e38ce1f195efa2d76f9dc33832bf5
 https://conda.anaconda.org/conda-forge/noarch/jupyter-cache-0.6.1-pyhd8ed1ab_0.conda#2e360820ae68e3d28e1a5a9d2714ca5c
 https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda#40190b7d06f86b63d28fa78aaa39c023
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/docs/win-64/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/win-64/py3.11/lab3/conda.lock`

 * *Files 9% similar despite different names*

```diff
@@ -1,135 +1,165 @@
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2023.5.7-h56e8100_0.conda#604212634bd8c4d6f20d44b946e8eedb
 https://conda.anaconda.org/conda-forge/win-64/libexpat-2.5.0-h63175ca_1.conda#636cc3cbbd2e28bcfd2f73b2044aac2c
-https://conda.anaconda.org/conda-forge/win-64/nodejs-18.16.1-h57928b3_0.conda#8ceddf0826beb0b7730e89b2065d5b7e
+https://conda.anaconda.org/conda-forge/win-64/nodejs-18.15.0-h57928b3_1.conda#d728bbdc9a650a5d503d657ce12c01ce
+https://conda.anaconda.org/conda-forge/win-64/pandoc-2.19.2-h57928b3_2.conda#c188f67e94153ddc7e4e10ae127cbb1a
 https://conda.anaconda.org/conda-forge/win-64/python_abi-3.11-3_cp311.conda#fd1634ba85cfea9376e1fc02d6f592e9
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
 https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
-https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.36.32532-hfdfe4a8_17.conda#91c1ecaf3996889532fc0456178b1058
-https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h64f974e_17.conda#67ff6791f235bb606659bf2a5c169191
-https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.36.32532-h05e6639_17.conda#4618046c39f7c81861e53ded842e738a
+https://conda.anaconda.org/conda-forge/win-64/winpty-0.4.3-4.tar.bz2#1cee351bf20b830d991dbe0bc8cd7dfe
+https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.34.31931-h5081d32_16.conda#22125178654c6a8a393f9743d585704b
+https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hb25d44b_16.conda#ea326b37e3bd6d2616988e09f3a9396c
+https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.34.31931-hed1258a_16.conda#0374eae69b6dbfb27c3dc27167109eb4
 https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
+https://conda.anaconda.org/conda-forge/win-64/firefox-113.0-h63175ca_0.conda#a2bd8315d1c49f718d4ffe0b7cf39e00
+https://conda.anaconda.org/conda-forge/win-64/geckodriver-0.33.0-h611cf2b_0.conda#e5ad5ec7f6140c1fdf9bd2a7927a4f91
+https://conda.anaconda.org/conda-forge/win-64/libbrotlicommon-1.0.9-hcfcfb64_8.tar.bz2#e8078e37208cd7d3e1eb5053f370ded8
 https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
 https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2#5c1fb45b5e2912c19098750ae8a32604
 https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.42.0-hcfcfb64_0.conda#9a71d93deb99cc09d8939d5235b5909a
-https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
+https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_4.tar.bz2#0cc5c5cc64ee1637f37f8540a175854c
 https://conda.anaconda.org/conda-forge/win-64/openssl-3.1.1-hcfcfb64_1.conda#1d913a5de46c6b2f7e4cfbd26b106b8b
 https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2#c69a5047cc9291ae40afd4a1ad6f0c0f
 https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
 https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
-https://conda.anaconda.org/conda-forge/win-64/python-3.11.4-h2628c8c_0_cpython.conda#3187a32fba79e835f099ecea054026f4
+https://conda.anaconda.org/conda-forge/win-64/libbrotlidec-1.0.9-hcfcfb64_8.tar.bz2#99839d9d81f33afa173c0fa82a702038
+https://conda.anaconda.org/conda-forge/win-64/libbrotlienc-1.0.9-hcfcfb64_8.tar.bz2#88e62627120c20289bf8982b15e0a6a1
+https://conda.anaconda.org/conda-forge/win-64/python-3.11.3-h2628c8c_0_cpython.conda#8f82e0e0ba51bed311f28eb6450393f6
 https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.4-h0e60522_1.tar.bz2#e1aff0583dda5fb917eb3d2c1025aa80
-https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
+https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
+https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/win-64/brotli-python-1.0.9-py311h12c1d0e_9.conda#e3f916714f59b88acb5d3c9d83b6f44a
+https://conda.anaconda.org/conda-forge/win-64/brotli-bin-1.0.9-hcfcfb64_8.tar.bz2#e18b70ed349d96086fd60a9c642b1b58
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.7-py311h12c1d0e_0.conda#b056c7299be929b711016d2f4e48d303
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
-https://conda.anaconda.org/conda-forge/win-64/docutils-0.19-py311h1ea47a8_1.tar.bz2#52b2142036004451e1881d97e9d01e8a
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
+https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
+https://conda.anaconda.org/conda-forge/win-64/docutils-0.20.1-py311h1ea47a8_0.conda#851f4c302cc7f5a617cc03a3c2090634
+https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
-https://conda.anaconda.org/conda-forge/win-64/greenlet-2.0.2-py311h12c1d0e_1.conda#07ff18c128d8f3cea2d077a431658456
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
-https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
-https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.3-py311ha68e1ae_0.conda#db2c2f72a83bdc5b70947964e1ddc8bb
-https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
+https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_robotmode-0.3.1-pyhd8ed1ab_0.tar.bz2#081f1505925bd5ff080864f4281c28a6
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.2-py311ha68e1ae_0.conda#96e7ffe6ea438ba4517152abe3b39874
+https://conda.anaconda.org/conda-forge/noarch/mistune-2.0.5-pyhd8ed1ab_0.conda#61a07195cfc935f1c1901d8ecf4af441
+https://conda.anaconda.org/conda-forge/noarch/natsort-8.3.1-pyhd8ed1ab_0.conda#8c53149aa69bfeb045f28c92a2b2ddc7
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
+https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/port-for-0.7.1-pyhd8ed1ab_0.conda#911d5daac0d579dc7aa4d85050ccd548
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
 https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.5-py311ha68e1ae_0.conda#f1a1eecd1bb4f431df5b9b6d8a152efd
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
+https://conda.anaconda.org/conda-forge/win-64/pyrsistent-0.19.3-py311ha68e1ae_0.conda#3f2780a49f0b4bb2c622f7cf098e3d06
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
+https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/win-64/pywin32-304-py311h12c1d0e_2.tar.bz2#20a2d8e73b0be8e27ca4096d4f3a7053
+https://conda.anaconda.org/conda-forge/win-64/pywinpty-2.0.10-py311h12c1d0e_0.conda#4d7e034dc93f50757cf039a2e3183343
 https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py311ha68e1ae_5.tar.bz2#0c97d59d54eb52e170224b3de6ade906
 https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.0-py311h7b3f143_0.conda#b690f6e1878ccc98e96a33658867e8e1
-https://conda.anaconda.org/conda-forge/noarch/robotframework-6.1-pyhd8ed1ab_0.conda#e383bebdc0d8fea4ecf9c9e01d0959fe
-https://conda.anaconda.org/conda-forge/win-64/rpds-py-0.9.2-py311hc37eb10_0.conda#d2d75b1d27bcd4f7b6d049b32b2f7530
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
+https://conda.anaconda.org/conda-forge/noarch/robotframework-6.0.2-pyhd8ed1ab_1.conda#b4dcead8c5a99a14733d9b1ba5b7db09
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
-https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
-https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.4-pyhd8ed1ab_0.conda#5a31a7d564f551d0e6dff52fd8cb5b16
-https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
-https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.1-pyhd8ed1ab_0.conda#6c8c4d6eb2325e59290ac6dbbeacd5f0
-https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
-https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
-https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
-https://conda.anaconda.org/conda-forge/noarch/tabulate-0.9.0-pyhd8ed1ab_1.tar.bz2#4759805cce2d914c38472f70bf4d8bcb
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
 https://conda.anaconda.org/conda-forge/win-64/tornado-6.3.2-py311ha68e1ae_0.conda#e2a6c106c1cff7e884d93351cdee3c3e
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
+https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
+https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.2-pyhd8ed1ab_0.conda#bfe7e7cd1476092f51efbcde15dfb110
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
 https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
-https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
+https://conda.anaconda.org/conda-forge/win-64/y-py-0.5.9-py311hc37eb10_0.conda#c16da06cd2c39bba7391076fd64024d8
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
+https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
+https://conda.anaconda.org/conda-forge/win-64/brotli-1.0.9-hcfcfb64_8.tar.bz2#2e661f21e1741c11506bdc7226e6b0bc
 https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py311h7d9ee11_3.conda#a8524727eb956b4741e25a64af79edb8
-https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-win_pyh7428d3b_0.conda#c1e57b6771510a3d2648ed6e76277391
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
+https://conda.anaconda.org/conda-forge/win-64/coverage-7.2.7-py311ha68e1ae_0.conda#b3a60b6bb264fe70896de40fa392edf6
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
-https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
+https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.30.0-pyhd8ed1ab_0.conda#13bf095e3ecd18999d65b4d3ac5b15d5
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.2.0-pyhd8ed1ab_0.conda#c9e9064ab45ffb46f7a96834d9e7626d
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
+https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
+https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
+https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh08f2357_0.conda#c00d32dfa733d381b6a1908d0d67e0d7
+https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.0-pyh08f2357_0.tar.bz2#0152a609d5748ed9887d195b1e61a6c9
+https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
+https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
+https://conda.anaconda.org/conda-forge/win-64/argon2-cffi-bindings-21.2.0-py311ha68e1ae_3.tar.bz2#c321cd825b72a2073dfb3f92ce1507fb
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.7.1-pyhd8ed1ab_0.conda#7c27ea1bdbe520bb830dcadd59f55cbf
-https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.3.5-pyhd8ed1ab_0.conda#9eeb66a24c8f6d950eb55a9f1128da20
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
-https://conda.anaconda.org/conda-forge/win-64/sqlalchemy-2.0.19-py311ha68e1ae_0.conda#944762d7af313330f06b0475b2cc4853
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.15.0-pyhd8ed1ab_0.conda#02e7912139fb64828d18d07c43dcbad0
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/win-64/trio-0.22.2-py311h1ea47a8_0.conda#621bba80ba8161029c356642c8b0080a
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.4-pyhd8ed1ab_0.conda#18badd8fa3648d1beb1fcc7f2e0f756e
+https://conda.anaconda.org/conda-forge/win-64/trio-0.22.0-py311h1ea47a8_1.tar.bz2#1475d3775d4e2cc09c366720de842992
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.2-pyhd8ed1ab_0.conda#81a763f3c64fe6d5f32e033b0325265d
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
+https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.18.4-pyhd8ed1ab_0.conda#7356151a32ebd9a20158d2f26d224bfa
-https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.3.1-py311h1ea47a8_0.conda#6754e6f5ead86225c8c78825ff0398c9
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
+https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.3.0-py311h1ea47a8_0.conda#2b81965b74e70b89053845d1bc287561
+https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
+https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
+https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.2-pyhd8ed1ab_0.conda#4ec732d2264373773a5feaea477128a8
+https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.8.0-pyhd8ed1ab_0.conda#1ca43103a08456b19222d93fd9d119ac
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
-https://conda.anaconda.org/conda-forge/noarch/sphinx-5.3.0-pyhd8ed1ab_0.tar.bz2#f9e1fcfe235d655900bfeb6aee426472
-https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh08f2357_0.conda#1fc684c1de5475383790ada5627c5430
-https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
-https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda#f7aa15f77d29b11caa1df1eb15383c59
-https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
-https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
-https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2021.3.14-pyhd8ed1ab_0.tar.bz2#1909f784dc37b4ab97afe2c95aeeabaa
-https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh6817e22_0.conda#b5cd11cf19c739548e968c12e020c54d
-https://conda.anaconda.org/conda-forge/noarch/jupyter-cache-0.6.1-pyhd8ed1ab_0.conda#2e360820ae68e3d28e1a5a9d2714ca5c
-https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda#40190b7d06f86b63d28fa78aaa39c023
+https://conda.anaconda.org/conda-forge/noarch/ipython-8.13.2-pyh08f2357_0.conda#aebd5e79c0f354cdbceb055cdec53659
+https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
+https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_0.conda#15700afca8f7ab35542e9c1af63568f1
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh025b116_0.conda#d18e38ce1f195efa2d76f9dc33832bf5
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.4.0-pyhd8ed1ab_0.conda#4456e6030a8309bdad57569b0170b6a3
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.4.0-pyhd8ed1ab_0.conda#127c702e1b1eff595be82bc6a78cfce0
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.22.1-pyhd8ed1ab_0.conda#fc7172a6742a7c3c4331ddd7ed463ffc
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.4.0-pyhd8ed1ab_0.conda#a86727968b41c20dd3d73b91632e77dc
+https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server_ydoc-0.8.0-pyhd8ed1ab_0.conda#780280d42fbcb2eaf654a6ba7a3e5bb5
+https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
+https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.4-pyhd8ed1ab_0.conda#e66d4a6e36fcc92fe266932bf85fd35a
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/lint/linux-64/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/lint/win-64/conda.lock`

 * *Files 6% similar despite different names*

```diff
@@ -1,86 +1,85 @@
 @EXPLICIT
-https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
-https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
-https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.1.0-hfd8a6a1_0.conda#067bcc23164642f4c226da631f2a2e1d
-https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.11-3_cp311.conda#c2e2630ddb68cf52eec74dc7dfab20b5
+https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2023.5.7-h56e8100_0.conda#604212634bd8c4d6f20d44b946e8eedb
+https://conda.anaconda.org/conda-forge/win-64/libexpat-2.5.0-h63175ca_1.conda#636cc3cbbd2e28bcfd2f73b2044aac2c
+https://conda.anaconda.org/conda-forge/win-64/nodejs-18.15.0-h57928b3_1.conda#d728bbdc9a650a5d503d657ce12c01ce
+https://conda.anaconda.org/conda-forge/win-64/python_abi-3.11-3_cp311.conda#fd1634ba85cfea9376e1fc02d6f592e9
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
-https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
-https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
-https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
-https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
-https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
-https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
-https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
-https://conda.anaconda.org/conda-forge/linux-64/libuv-1.44.2-h166bdaf_0.tar.bz2#e5cb4fe581a18ca2185a016eb848fc00
-https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
-https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
-https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
-https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
-https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
-https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
-https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
-https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
-https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
-https://conda.anaconda.org/conda-forge/linux-64/nodejs-18.16.1-hf52ce11_0.conda#23ed78db48ed08c94e5449f6661d65e6
-https://conda.anaconda.org/conda-forge/linux-64/python-3.11.4-hab00c5b_0_cpython.conda#1c628861a2a126b9fc9363ca1b7d014e
+https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
+https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.34.31931-h5081d32_16.conda#22125178654c6a8a393f9743d585704b
+https://conda.anaconda.org/conda-forge/win-64/yarn-1.22.19-h57928b3_0.tar.bz2#b08134bf44e3ee5aa63a5448cb923683
+https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hb25d44b_16.conda#ea326b37e3bd6d2616988e09f3a9396c
+https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.34.31931-hed1258a_16.conda#0374eae69b6dbfb27c3dc27167109eb4
+https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
+https://conda.anaconda.org/conda-forge/win-64/libbrotlicommon-1.0.9-hcfcfb64_8.tar.bz2#e8078e37208cd7d3e1eb5053f370ded8
+https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
+https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.42.0-hcfcfb64_0.conda#9a71d93deb99cc09d8939d5235b5909a
+https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_4.tar.bz2#0cc5c5cc64ee1637f37f8540a175854c
+https://conda.anaconda.org/conda-forge/win-64/openssl-3.1.1-hcfcfb64_1.conda#1d913a5de46c6b2f7e4cfbd26b106b8b
+https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2#c69a5047cc9291ae40afd4a1ad6f0c0f
+https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
+https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
+https://conda.anaconda.org/conda-forge/win-64/libbrotlidec-1.0.9-hcfcfb64_8.tar.bz2#99839d9d81f33afa173c0fa82a702038
+https://conda.anaconda.org/conda-forge/win-64/libbrotlienc-1.0.9-hcfcfb64_8.tar.bz2#88e62627120c20289bf8982b15e0a6a1
+https://conda.anaconda.org/conda-forge/win-64/python-3.11.3-h2628c8c_0_cpython.conda#8f82e0e0ba51bed311f28eb6450393f6
+https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
-https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.0.9-py311ha362b79_9.conda#ced5340f5dc6cff43a80deac8d0e398f
+https://conda.anaconda.org/conda-forge/win-64/brotli-bin-1.0.9-hcfcfb64_8.tar.bz2#e18b70ed349d96086fd60a9c642b1b58
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
-https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-unix_pyh707e725_0.conda#64dbb3b205546691a61204d1cfb208e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
-https://conda.anaconda.org/conda-forge/linux-64/docutils-0.20.1-py311h38be061_0.conda#207175b7d514d42f977ec505800d6824
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
+https://conda.anaconda.org/conda-forge/win-64/docutils-0.20.1-py311h1ea47a8_0.conda#851f4c302cc7f5a617cc03a3c2090634
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
-https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py311h459d7ec_0.conda#9904dc4adb5d547cb21e136f98cb24b0
+https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.2-py311ha68e1ae_0.conda#96e7ffe6ea438ba4517152abe3b39874
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda#dbb80d1e8dc2dba5c8b106dc0768ad45
+https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
-https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
-https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py311hd4cff14_5.tar.bz2#da8769492e423103c59f469f4f17f8d9
-https://conda.anaconda.org/conda-forge/noarch/robotframework-6.1-pyhd8ed1ab_0.conda#e383bebdc0d8fea4ecf9c9e01d0959fe
-https://conda.anaconda.org/conda-forge/linux-64/ruff-0.0.278-py311h7145743_0.conda#9de13e2ecc62f50a8dd30115e31b3290
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py311ha68e1ae_5.tar.bz2#0c97d59d54eb52e170224b3de6ade906
+https://conda.anaconda.org/conda-forge/noarch/robotframework-6.0.2-pyhd8ed1ab_1.conda#b4dcead8c5a99a14733d9b1ba5b7db09
+https://conda.anaconda.org/conda-forge/win-64/ruff-0.0.270-py311hc14472d_0.conda#f1004bafb79f5d9269eea7a2309948d1
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
-https://conda.anaconda.org/conda-forge/linux-64/yarn-1.22.19-ha770c72_0.tar.bz2#61598c43738c48fac9e01294ff3d8bdb
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/win-64/brotli-1.0.9-hcfcfb64_8.tar.bz2#2e661f21e1741c11506bdc7226e6b0bc
+https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py311h7d9ee11_3.conda#a8524727eb956b4741e25a64af79edb8
+https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-win_pyhd8ed1ab_2.tar.bz2#6b58680207b526c42dcff68b543803dd
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
+https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.2.0-pyhd8ed1ab_0.conda#c9e9064ab45ffb46f7a96834d9e7626d
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/ssort-0.11.6-pyhd8ed1ab_0.tar.bz2#53729b150f41dd6ae004ce5854904659
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.4-pyhd8ed1ab_0.conda#18badd8fa3648d1beb1fcc7f2e0f756e
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.1-pyhd8ed1ab_0.conda#e76070baecfaca6ecdb5fbd5af7c9309
-https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
-https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.2-py311h38be061_0.conda#dcbfe3a95e8b99ec743e26a75d8c9cf4
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
+https://conda.anaconda.org/conda-forge/noarch/rich-13.3.5-pyhd8ed1ab_0.conda#2e40a02ad28e34f26cee2a72042843db
+https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-3.1.1-pyhd8ed1ab_0.conda#085598f9bc7287ee92ac0fa6ecfcf522
+https://conda.anaconda.org/conda-forge/win-64/trio-0.22.0-py311h1ea47a8_1.tar.bz2#1475d3775d4e2cc09c366720de842992
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.2-pyhd8ed1ab_0.conda#81a763f3c64fe6d5f32e033b0325265d
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
-https://conda.anaconda.org/conda-forge/linux-64/black-23.7.0-py311h38be061_1.conda#9dc54d30b15760b58706ac840803f6b4
+https://conda.anaconda.org/conda-forge/win-64/black-23.3.0-py311h1ea47a8_1.conda#cff72d53d4ea05005adc2f478447a0a1
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
-https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
+https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/rich-click-1.6.1-pyhd8ed1ab_0.conda#59a168d82c582248859d8dc8075da6f6
-https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-4.0.1-pyhd8ed1ab_0.conda#8ae87b8a24e3167fe71a8703ed7b202b
-https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
-https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.4.0-pyhd8ed1ab_0.conda#e27606b585fe4780ffc3827f83c26b57
+https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.2-pyhd8ed1ab_0.conda#4ec732d2264373773a5feaea477128a8
+https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
+https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.3.0-pyhd8ed1ab_0.conda#f156c895a6c4d63805bb3999f0544fe8
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
-https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
+https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_0.conda#15700afca8f7ab35542e9c1af63568f1
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/lint/osx-64/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/lint/osx-64/conda.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,79 +1,84 @@
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
 https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
-https://conda.anaconda.org/conda-forge/osx-64/icu-72.1-h7336db1_0.conda#c9689510a50a4bb2ae978421671a125e
-https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_8.tar.bz2#37157d273eaf3bc7d6862104161d9ec9
+https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.4-hd57cbcb_0.conda#195236e2eeb3b108e3b8eee47ad074fd
 https://conda.anaconda.org/conda-forge/osx-64/libexpat-2.5.0-hf0c8a7f_1.conda#6c81cb022780ee33435cca0127dd43c9
 https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
 https://conda.anaconda.org/conda-forge/osx-64/libuv-1.44.2-hac89ed1_0.tar.bz2#958fa9add5701462a6c91e3774425ea1
-https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
-https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
+https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-hfd90126_4.tar.bz2#35eb3fce8d51ed3c1fd4122bad48250b
+https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.3-h96cf925_1.tar.bz2#76217ebfbb163ff2770a261f955a5861
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.11-3_cp311.conda#5e0a069a585445333868d2c6651c3b3f
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
 https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
+https://conda.anaconda.org/conda-forge/osx-64/icu-70.1-h96cf925_0.tar.bz2#376635049e9b9b0bb875efd39dcd7b3b
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_8.tar.bz2#7f952a036d9014b4dab96c6ea0f8c2a7
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_8.tar.bz2#b36a3bfe866d9127f25f286506982166
 https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
 https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
-https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-h8a1eda9_5.conda#75a8a98b1c4671c5d2897975731da42d
-https://conda.anaconda.org/conda-forge/osx-64/nodejs-18.16.1-h46e3395_0.conda#e4c06702959edec36072a3d081af4587
-https://conda.anaconda.org/conda-forge/osx-64/python-3.11.4-h30d4d87_0_cpython.conda#e40b3075f85db0184d5f61d17c580ef7
+https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-hfd90126_4.tar.bz2#be90e6223c74ea253080abae19b3bdb1
+https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_8.tar.bz2#aac5ad0d8f747ef7f871508146df75d9
+https://conda.anaconda.org/conda-forge/osx-64/nodejs-18.15.0-hd0c9b3c_0.conda#4c7eb1947ecaa10394cf1cbcca343131
+https://conda.anaconda.org/conda-forge/osx-64/python-3.11.3-h99528f9_0_cpython.conda#c3291f9411424fc587d53a2ea57fb075
+https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
-https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.0.9-py311h814d153_9.conda#034ddcc806d421524fbc46778447e87c
+https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_8.tar.bz2#55f612fe4a9b5f6ac76348b6de94aaeb
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
-https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-unix_pyh707e725_0.conda#64dbb3b205546691a61204d1cfb208e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
+https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/osx-64/docutils-0.20.1-py311h6eed73b_0.conda#0536cbe889e20101b7f8e6d6b1dbcbf4
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
-https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.3-py311h2725bcf_0.conda#65b70928fcc2a81891ad1a8a6a7b085a
+https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.2-py311h5547dcb_0.conda#13091519d55d667506aaf413cffaff10
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda#dbb80d1e8dc2dba5c8b106dc0768ad45
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py311h5547dcb_5.tar.bz2#8d1e456914ce961119b07f396187a564
-https://conda.anaconda.org/conda-forge/noarch/robotframework-6.1-pyhd8ed1ab_0.conda#e383bebdc0d8fea4ecf9c9e01d0959fe
-https://conda.anaconda.org/conda-forge/osx-64/ruff-0.0.278-py311hbf57787_0.conda#29574c8686dd4ca23349309a19b38355
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/noarch/robotframework-6.0.2-pyhd8ed1ab_1.conda#b4dcead8c5a99a14733d9b1ba5b7db09
+https://conda.anaconda.org/conda-forge/osx-64/ruff-0.0.270-py311hbf57787_0.conda#6c5985dd7bb8416badbf99b4a16203a0
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
 https://conda.anaconda.org/conda-forge/osx-64/yarn-1.22.19-h694c41f_0.tar.bz2#9f64d37f3aff1bb032a3cd76ab6ed1aa
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
+https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.2.0-pyhd8ed1ab_0.conda#c9e9064ab45ffb46f7a96834d9e7626d
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/ssort-0.11.6-pyhd8ed1ab_0.tar.bz2#53729b150f41dd6ae004ce5854904659
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.4-pyhd8ed1ab_0.conda#18badd8fa3648d1beb1fcc7f2e0f756e
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.2-pyhd8ed1ab_0.conda#81a763f3c64fe6d5f32e033b0325265d
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.1-pyhd8ed1ab_0.conda#e76070baecfaca6ecdb5fbd5af7c9309
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
-https://conda.anaconda.org/conda-forge/osx-64/trio-0.22.2-py311h6eed73b_0.conda#6ceb2138c6038d75a92b06d3f8fd9ece
+https://conda.anaconda.org/conda-forge/noarch/rich-13.3.5-pyhd8ed1ab_0.conda#2e40a02ad28e34f26cee2a72042843db
+https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-3.1.1-pyhd8ed1ab_0.conda#085598f9bc7287ee92ac0fa6ecfcf522
+https://conda.anaconda.org/conda-forge/osx-64/trio-0.22.0-py311h6eed73b_1.tar.bz2#71a739c4b0b1e17cfd27cfdf828d52a8
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
-https://conda.anaconda.org/conda-forge/osx-64/black-23.7.0-py311h6eed73b_1.conda#476e9030b804b5428b52e33e3f7bbecf
+https://conda.anaconda.org/conda-forge/osx-64/black-23.3.0-py311h6eed73b_1.conda#2783c68e84c0573fece0880488c7c001
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
 https://conda.anaconda.org/conda-forge/noarch/rich-click-1.6.1-pyhd8ed1ab_0.conda#59a168d82c582248859d8dc8075da6f6
-https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-4.0.1-pyhd8ed1ab_0.conda#8ae87b8a24e3167fe71a8703ed7b202b
-https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
-https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.4.0-pyhd8ed1ab_0.conda#e27606b585fe4780ffc3827f83c26b57
+https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.2-pyhd8ed1ab_0.conda#4ec732d2264373773a5feaea477128a8
+https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.3.0-pyhd8ed1ab_0.conda#f156c895a6c4d63805bb3999f0544fe8
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
-https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
+https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_0.conda#15700afca8f7ab35542e9c1af63568f1
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/lint/win-64/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/lint/linux-64/conda.lock`

 * *Files 14% similar despite different names*

```diff
@@ -1,80 +1,91 @@
 @EXPLICIT
-https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2023.5.7-h56e8100_0.conda#604212634bd8c4d6f20d44b946e8eedb
-https://conda.anaconda.org/conda-forge/win-64/libexpat-2.5.0-h63175ca_1.conda#636cc3cbbd2e28bcfd2f73b2044aac2c
-https://conda.anaconda.org/conda-forge/win-64/nodejs-18.16.1-h57928b3_0.conda#8ceddf0826beb0b7730e89b2065d5b7e
-https://conda.anaconda.org/conda-forge/win-64/python_abi-3.11-3_cp311.conda#fd1634ba85cfea9376e1fc02d6f592e9
+https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
+https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
+https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-12.2.0-h46fd767_19.tar.bz2#1030b1f38c129f2634eae026f704fe60
+https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.11-3_cp311.conda#c2e2630ddb68cf52eec74dc7dfab20b5
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
-https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
-https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.36.32532-hfdfe4a8_17.conda#91c1ecaf3996889532fc0456178b1058
-https://conda.anaconda.org/conda-forge/win-64/yarn-1.22.19-h57928b3_0.tar.bz2#b08134bf44e3ee5aa63a5448cb923683
-https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h64f974e_17.conda#67ff6791f235bb606659bf2a5c169191
-https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.36.32532-h05e6639_17.conda#4618046c39f7c81861e53ded842e738a
-https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
-https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
-https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.42.0-hcfcfb64_0.conda#9a71d93deb99cc09d8939d5235b5909a
-https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
-https://conda.anaconda.org/conda-forge/win-64/openssl-3.1.1-hcfcfb64_1.conda#1d913a5de46c6b2f7e4cfbd26b106b8b
-https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2#c69a5047cc9291ae40afd4a1ad6f0c0f
-https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
-https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
-https://conda.anaconda.org/conda-forge/win-64/python-3.11.4-h2628c8c_0_cpython.conda#3187a32fba79e835f099ecea054026f4
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-12.2.0-h65d4601_19.tar.bz2#cedcee7c064c01c403f962c9e8d3c373
+https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-12.2.0-h65d4601_19.tar.bz2#e4c94f80aef025c17ab0828cd85ef535
+https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
+https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2#9194c9bf9428035a05352d031462eae4
+https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
+https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
+https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
+https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
+https://conda.anaconda.org/conda-forge/linux-64/libuv-1.44.2-h166bdaf_0.tar.bz2#e5cb4fe581a18ca2185a016eb848fc00
+https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-h166bdaf_4.tar.bz2#f3f9de449d32ca9b9c66a22863c96f41
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h27087fc_1.tar.bz2#4acfc691e64342b9dae57cf2adc63238
+https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
+https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
+https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2#4ae4d7795d33e02bd20f6b23d91caf82
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2#04bac51ba35ea023dc48af73c1c88c25
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
+https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
+https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
+https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-h166bdaf_4.tar.bz2#4b11e365c0275b808be78b30f904e295
+https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2#e5613f2bc717e9945840ff474419b8e4
+https://conda.anaconda.org/conda-forge/linux-64/nodejs-18.15.0-h4abf6b9_1.conda#2aabafd88f6876a57c45c00598715ac4
+https://conda.anaconda.org/conda-forge/linux-64/python-3.11.3-h2755cc3_0_cpython.conda#37005ea5f68df6a8a381b70cf4d4a160
+https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
-https://conda.anaconda.org/conda-forge/win-64/brotli-python-1.0.9-py311h12c1d0e_9.conda#e3f916714f59b88acb5d3c9d83b6f44a
+https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_8.tar.bz2#2ff08978892a3e8b954397c461f18418
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
+https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
-https://conda.anaconda.org/conda-forge/win-64/docutils-0.20.1-py311h1ea47a8_0.conda#851f4c302cc7f5a617cc03a3c2090634
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
+https://conda.anaconda.org/conda-forge/linux-64/docutils-0.20.1-py311h38be061_0.conda#207175b7d514d42f977ec505800d6824
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
-https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.3-py311ha68e1ae_0.conda#db2c2f72a83bdc5b70947964e1ddc8bb
+https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.2-py311h2582759_0.conda#adb20bd57069614552adac60a020c36d
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda#dbb80d1e8dc2dba5c8b106dc0768ad45
-https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
-https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py311ha68e1ae_5.tar.bz2#0c97d59d54eb52e170224b3de6ade906
-https://conda.anaconda.org/conda-forge/noarch/robotframework-6.1-pyhd8ed1ab_0.conda#e383bebdc0d8fea4ecf9c9e01d0959fe
-https://conda.anaconda.org/conda-forge/win-64/ruff-0.0.278-py311hc14472d_0.conda#b08a88ea3efc302641e0b4463bbf6ed6
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py311hd4cff14_5.tar.bz2#da8769492e423103c59f469f4f17f8d9
+https://conda.anaconda.org/conda-forge/noarch/robotframework-6.0.2-pyhd8ed1ab_1.conda#b4dcead8c5a99a14733d9b1ba5b7db09
+https://conda.anaconda.org/conda-forge/linux-64/ruff-0.0.270-py311h7145743_0.conda#d3815827ba01af4a36bdeffe12c4717a
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
-https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
-https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py311h7d9ee11_3.conda#a8524727eb956b4741e25a64af79edb8
-https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-win_pyh7428d3b_0.conda#c1e57b6771510a3d2648ed6e76277391
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/linux-64/yarn-1.22.19-ha770c72_0.tar.bz2#61598c43738c48fac9e01294ff3d8bdb
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
+https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
-https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.2.0-pyhd8ed1ab_0.conda#c9e9064ab45ffb46f7a96834d9e7626d
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/ssort-0.11.6-pyhd8ed1ab_0.tar.bz2#53729b150f41dd6ae004ce5854904659
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.2-pyhd8ed1ab_0.conda#81a763f3c64fe6d5f32e033b0325265d
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.1-pyhd8ed1ab_0.conda#e76070baecfaca6ecdb5fbd5af7c9309
-https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
-https://conda.anaconda.org/conda-forge/win-64/trio-0.22.2-py311h1ea47a8_0.conda#621bba80ba8161029c356642c8b0080a
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.4-pyhd8ed1ab_0.conda#18badd8fa3648d1beb1fcc7f2e0f756e
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
+https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
+https://conda.anaconda.org/conda-forge/noarch/rich-13.3.5-pyhd8ed1ab_0.conda#2e40a02ad28e34f26cee2a72042843db
+https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-3.1.1-pyhd8ed1ab_0.conda#085598f9bc7287ee92ac0fa6ecfcf522
+https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.0-py311h38be061_1.tar.bz2#0564e63c41c0527f8085a572a931f1e6
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
-https://conda.anaconda.org/conda-forge/win-64/black-23.7.0-py311h1ea47a8_1.conda#335ab55360386db3b594370694d3a22c
+https://conda.anaconda.org/conda-forge/linux-64/black-23.3.0-py311h38be061_1.conda#b0d621848bfba5aacbdfc43dfdeabfec
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
-https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/rich-click-1.6.1-pyhd8ed1ab_0.conda#59a168d82c582248859d8dc8075da6f6
-https://conda.anaconda.org/conda-forge/noarch/robotframework-robocop-4.0.1-pyhd8ed1ab_0.conda#8ae87b8a24e3167fe71a8703ed7b202b
-https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
-https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.4.0-pyhd8ed1ab_0.conda#e27606b585fe4780ffc3827f83c26b57
+https://conda.anaconda.org/conda-forge/noarch/rich-click-1.6.1-pyhd8ed1ab_0.conda#59a168d82c582248859d8dc8075da6f6
+https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.2-pyhd8ed1ab_0.conda#4ec732d2264373773a5feaea477128a8
+https://conda.anaconda.org/conda-forge/noarch/robotframework-tidy-4.3.0-pyhd8ed1ab_0.conda#f156c895a6c4d63805bb3999f0544fe8
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
-https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
+https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_0.conda#15700afca8f7ab35542e9c1af63568f1
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/meta/linux-64/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/meta/linux-64/conda.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,172 +1,168 @@
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
 https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.1.0-hfd8a6a1_0.conda#067bcc23164642f4c226da631f2a2e1d
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-12.2.0-h46fd767_19.tar.bz2#1030b1f38c129f2634eae026f704fe60
 https://conda.anaconda.org/conda-forge/noarch/pybind11-abi-4-hd8ed1ab_3.tar.bz2#878f923dd6acc8aeb47a75da6c4098be
 https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.11-3_cp311.conda#c2e2630ddb68cf52eec74dc7dfab20b5
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-12.2.0-h65d4601_19.tar.bz2#cedcee7c064c01c403f962c9e8d3c373
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-12.2.0-h65d4601_19.tar.bz2#e4c94f80aef025c17ab0828cd85ef535
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
 https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.19.1-hd590300_0.conda#e8c18d865be43e2fb3f7a145b6adf1f5
 https://conda.anaconda.org/conda-forge/linux-64/fmt-9.1.0-h924138e_0.tar.bz2#b57864c85261a0fbc7132d2cc17478c7
 https://conda.anaconda.org/conda-forge/linux-64/gettext-0.21.1-h27087fc_0.tar.bz2#14947d8770185e5153fdd04d4673ed37
 https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
 https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2#30186d27e2c9fa62b45fb1476b7200e3
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-h516909a_1.tar.bz2#6f8720dff19e17ce5d48cfe7f3d2f0a3
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-h166bdaf_0.tar.bz2#b62b52da46c39ee2bc3c162ac7f1804d
 https://conda.anaconda.org/conda-forge/linux-64/liblief-0.12.3-h27087fc_0.tar.bz2#2ed926c822a091c21d467429d1eaa92c
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
-https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
+https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-h166bdaf_4.tar.bz2#f3f9de449d32ca9b9c66a22863c96f41
 https://conda.anaconda.org/conda-forge/linux-64/lz4-c-1.9.4-hcb278e6_0.conda#318b08df404f9c9be5712aaa5a6f0bb0
 https://conda.anaconda.org/conda-forge/linux-64/lzo-2.10-h516909a_1000.tar.bz2#bb14fcb13341b81d5eb386423b9d2bac
-https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h27087fc_1.tar.bz2#4acfc691e64342b9dae57cf2adc63238
 https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
 https://conda.anaconda.org/conda-forge/linux-64/patch-2.7.6-h7f98852_1002.tar.bz2#4c1bbbec45149a186b915c67d086ed3b
-https://conda.anaconda.org/conda-forge/linux-64/patchelf-0.17.2-h58526e2_0.conda#ba76a6a448819560b5f8b08a9c74f415
+https://conda.anaconda.org/conda-forge/linux-64/patchelf-0.18.0-h59595ed_0.conda#6cdb2b6d3bc02fc55f5e61ca95a3022b
 https://conda.anaconda.org/conda-forge/linux-64/reproc-14.2.4-h0b41bf4_0.conda#0f51393e019df1f0047ef864cd9ddeec
 https://conda.anaconda.org/conda-forge/linux-64/ripgrep-13.0.0-h2f28480_2.tar.bz2#15a0bf4a1260b0a08198eb683eb272fb
 https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
 https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
 https://conda.anaconda.org/conda-forge/linux-64/yaml-cpp-0.7.0-h27087fc_2.tar.bz2#0449d47d8457feaa3720d4779616dde2
 https://conda.anaconda.org/conda-forge/linux-64/expat-2.5.0-hcb278e6_1.conda#8b9b5aca60558d02ddaa09d599e55920
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
 https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.52.0-h61bc06f_0.conda#613955a50485812985c059e7b269f42e
-https://conda.anaconda.org/conda-forge/linux-64/libsolv-0.7.24-hfc55251_1.conda#9d2787f2fdcf65661e2416b2dffdb668
+https://conda.anaconda.org/conda-forge/linux-64/libsolv-0.7.23-h3eb15da_0.conda#122332e6deb4aea9eaf22021d2ecd256
 https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
-https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
+https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.10.0-hf14f497_3.tar.bz2#d85acad4b47dff4e3def14a769a97906
 https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.11.4-h0d562d8_0.conda#e46fad17d5fb57316b956f88dca765e4
 https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.40-hc3806b6_0.tar.bz2#69e2c796349cd9b273890bee0febfe1b
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/reproc-cpp-14.2.4-hcb278e6_0.conda#ede8e0f849f2fee2f78cb488b4ea3b33
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
-https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.2-hfc55251_7.conda#32ae18eb2a687912fc9e92a501c0a11b
-https://conda.anaconda.org/conda-forge/linux-64/krb5-1.21.1-h659d440_0.conda#1b5126ec25763eb17ef74c8763d26e84
+https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.2-h3eb15da_6.conda#6b63daed8feeca47be78f323e793d555
+https://conda.anaconda.org/conda-forge/linux-64/krb5-1.20.1-h81ceb04_0.conda#89a41adce7106749573d883b2f657d78
 https://conda.anaconda.org/conda-forge/linux-64/libarchive-3.6.2-h039dbb9_1.conda#29cf970521d30d113f3425b84cb250f6
-https://conda.anaconda.org/conda-forge/linux-64/libglib-2.76.4-hebfc3b9_0.conda#c6f951789c888f7bbd2dd6858eab69de
-https://conda.anaconda.org/conda-forge/linux-64/python-3.11.4-hab00c5b_0_cpython.conda#1c628861a2a126b9fc9363ca1b7d014e
+https://conda.anaconda.org/conda-forge/linux-64/libglib-2.76.3-hebfc3b9_0.conda#a64f11b244b2c112cd3fa1cbe9493999
+https://conda.anaconda.org/conda-forge/linux-64/python-3.11.3-h2755cc3_0_cpython.conda#37005ea5f68df6a8a381b70cf4d4a160
 https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2#5f095bc6454094e96f146491fd03633b
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/noarch/cachy-0.3.0-pyhd8ed1ab_1.tar.bz2#5dfee17f24e2dfd18d7392b48c9351e2
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/linux-64/chardet-5.1.0-py311h38be061_0.conda#9ad842c86331f98301ac1d3e4af26843
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
-https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-unix_pyh707e725_0.conda#64dbb3b205546691a61204d1cfb208e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
+https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/crashtest-0.4.1-pyhd8ed1ab_0.tar.bz2#709a2295dd907bb34afb57d54320642f
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/linux-64/dbus-1.13.6-h5008d03_3.tar.bz2#ecfff944ba3960ecb334b9a2663d708d
-https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.7-pyhd8ed1ab_0.conda#12d8aae6994f342618443a8f05c652a0
+https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2#b65b4d50dbd2d50fa0aeac367ec9eed7
 https://conda.anaconda.org/conda-forge/linux-64/docutils-0.20.1-py311h38be061_0.conda#207175b7d514d42f977ec505800d6824
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
-https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda#53522ec72e6adae42bd373ef58357230
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.0-pyhd8ed1ab_0.conda#650f18a56f366dbf419c15b543592c2d
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/glob2-0.7-py_0.tar.bz2#1f3a88e65e61216e1d475135922dbf6a
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2#9800ad1699b42612478755a2d26c722d
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
-https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.2.0-hca28451_0.conda#73d6b3c8d9a8f7f2703ef9163ab92b0e
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
+https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.1.2-h409715c_0.conda#50c873c9660ed116707ae15b663928d8
 https://conda.anaconda.org/conda-forge/noarch/lockfile-0.12.2-py_1.tar.bz2#c104d98e09c47519950cffb8dd5b4f10
-https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py311h459d7ec_0.conda#9904dc4adb5d547cb21e136f98cb24b0
+https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.2-py311h2582759_0.conda#adb20bd57069614552adac60a020c36d
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/more-itertools-9.1.0-pyhd8ed1ab_0.conda#1698a717f83cfecf644a877c174c84bd
 https://conda.anaconda.org/conda-forge/linux-64/msgpack-python-1.0.5-py311ha3edf6b_0.conda#7415f24f8c44e44152623d93c5015000
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2#a4eea5bff523f26442405bc5d1f52adb
 https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda#be1e9f1c65a1ed0f2ae9352fec99db64
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
 https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py311h2582759_0.conda#a90f8e278c1cd7064b2713e6b7db87e6
 https://conda.anaconda.org/conda-forge/linux-64/py-lief-0.12.3-py311ha362b79_0.tar.bz2#adbe6a080737fa9fa60fd655bd3afb39
 https://conda.anaconda.org/conda-forge/linux-64/pycosat-0.6.4-py311hd4cff14_1.tar.bz2#17399f8b68b4592f098ab18d4fdb0ac4
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
 https://conda.anaconda.org/conda-forge/noarch/pylev-1.4.0-pyhd8ed1ab_0.tar.bz2#edf8651c4379d9d1495ad6229622d150
+https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py311h2582759_0.conda#e53876b66dcc4ba8a0afa63cd8502ac3
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
-https://conda.anaconda.org/conda-forge/linux-64/python-libarchive-c-5.0-py311h38be061_1.conda#7ca450aa38981b17fd08c16f03660147
+https://conda.anaconda.org/conda-forge/linux-64/python-libarchive-c-4.0-py311h38be061_2.tar.bz2#1c3e2d22ddfb6ff2a0edd60e91e018db
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py311hd4cff14_5.tar.bz2#da8769492e423103c59f469f4f17f8d9
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-2.0.0-pyhd8ed1ab_0.tar.bz2#d337886e38f965bf97aaec382ff6db00
-https://conda.anaconda.org/conda-forge/linux-64/rpds-py-0.9.2-py311h46250e7_0.conda#bcf66b5abaec47198b42cdd0bb968540
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.7-py311h2582759_1.conda#5e997292429a22ad50c11af0a2cb0f08
 https://conda.anaconda.org/conda-forge/linux-64/ruamel_yaml-0.15.80-py311hd4cff14_1008.tar.bz2#cfc7aa9d4e13c267fb6531d4788f2ede
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/smmap-3.0.5-pyh44b312d_0.tar.bz2#3a8dc70789709aa315325d5df06fb7e4
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.8-pyha770c72_0.conda#75838e8556166263a82038b51d01d5f1
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2#92facfec94bc02d6ccf42e7173831a36
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
-https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.1-pyhd8ed1ab_0.conda#7b517e7a6f0790337906c055aa97ca49
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py311h409f033_3.conda#9025d0786dbbe4bc91fd8e85502decce
 https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2#72a46ffc25701c173932fd55cf0965d3
 https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyhd8ed1ab_2.conda#02abb7b66b02e8b9f5a9b05454400087
 https://conda.anaconda.org/conda-forge/noarch/gitdb-4.0.10-pyhd8ed1ab_0.conda#3706d2f3d7cb5dae600c833345a76132
 https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
-https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.3.0-pyhd8ed1ab_0.conda#e9f79248d30e942f7c358ff21a1790f5
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
+https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2#31e4a1506968d017229bdb64695013a1
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/noarch/joblib-1.3.0-pyhd8ed1ab_1.conda#fb4caf6da228ccc487350eade569abae
-https://conda.anaconda.org/conda-forge/linux-64/libmamba-1.4.9-h658169a_0.conda#903a241189a2fd9d7e6a33ee2505a49c
-https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.30.0-pyhd8ed1ab_0.conda#13bf095e3ecd18999d65b4d3ac5b15d5
-https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.32-py311h459d7ec_0.conda#628868dc17f9bd39a2eb77846e35980c
+https://conda.anaconda.org/conda-forge/noarch/joblib-1.2.0-pyhd8ed1ab_0.tar.bz2#7583652522d71ad78ba536bba06940eb
+https://conda.anaconda.org/conda-forge/linux-64/libmamba-1.4.2-hcea66bb_0.conda#0b3b4c833ea1ec555063479e2ac259dc
+https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
+https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.31-py311h459d7ec_0.conda#f0fc1409f49257fe5ec2d86d0595d9bc
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
-https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda#578ae086f225bc2380c79f3b551ff2f7
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
 https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py311hd4cff14_1005.tar.bz2#9bdac7084ecfc08338bae1b976535724
 https://conda.anaconda.org/conda-forge/linux-64/cmarkgfm-0.8.0-py311hd4cff14_2.tar.bz2#ed1a2dba3b53fcd450f2fe867af0ba3f
-https://conda.anaconda.org/conda-forge/linux-64/cryptography-41.0.2-py311h63ff55d_0.conda#90e9e96dd807c2613a163c197192da6c
+https://conda.anaconda.org/conda-forge/linux-64/cryptography-41.0.0-py311h63ff55d_0.conda#6bc48185b9486a8590a599e768cefb61
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.32-pyhd8ed1ab_0.conda#5809a12901d57388444c3293c975d0bb
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.7.1-pyhd8ed1ab_0.conda#7c27ea1bdbe520bb830dcadd59f55cbf
-https://conda.anaconda.org/conda-forge/linux-64/libmambapy-1.4.9-py311h527f279_0.conda#f16b9947a4614e335bdbcf17280989c5
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
-https://conda.anaconda.org/conda-forge/linux-64/pydantic-core-2.3.0-py311h46250e7_0.conda#99ca132ca705de6765df5e3c4c346572
-https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
+https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.31-pyhd8ed1ab_0.conda#f6e6b482110246a81c3f03e81c68752d
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
+https://conda.anaconda.org/conda-forge/linux-64/libmambapy-1.4.2-py311h1f88262_0.conda#178d22489c16ff3eefe33330ec9ccec9
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
+https://conda.anaconda.org/conda-forge/linux-64/pydantic-1.10.8-py311h459d7ec_0.conda#28c5d92548b5294b2726c89e91d68ac4
+https://conda.anaconda.org/conda-forge/noarch/rich-13.3.5-pyhd8ed1ab_0.conda#2e40a02ad28e34f26cee2a72042843db
 https://conda.anaconda.org/conda-forge/noarch/watchgod-0.8.2-pyhd8ed1ab_0.tar.bz2#8bf811791ff4ea8b6368b8ff451c6421
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
-https://conda.anaconda.org/conda-forge/linux-64/zstandard-0.19.0-py311haa97af0_2.conda#10b11630d87e0a1d4abce705bc4e0b55
+https://conda.anaconda.org/conda-forge/linux-64/zstandard-0.19.0-py311hbe0fcd7_1.conda#1f48d127dd18240505cba632b67f7931
 https://conda.anaconda.org/conda-forge/noarch/conda-package-streaming-0.8.0-pyhd8ed1ab_0.conda#ebe3230a4c1e135954eee4fb6ef8cded
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.18.4-pyhd8ed1ab_0.conda#7356151a32ebd9a20158d2f26d224bfa
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
-https://conda.anaconda.org/conda-forge/noarch/pydantic-2.0.3-pyhd8ed1ab_1.conda#77753c350c42e70dd3e9919dd8099fc7
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
 https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
-https://conda.anaconda.org/conda-forge/noarch/readme_renderer-40.0-pyhd8ed1ab_0.conda#9ba2b509f6fe88364512caa9089ea886
+https://conda.anaconda.org/conda-forge/noarch/readme_renderer-37.3-pyhd8ed1ab_0.tar.bz2#82e8ab317fe8f1d2a944688438dce868
 https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py311h38be061_1.tar.bz2#ec745aaae03cc47120c1f11ac7b7bcf5
-https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.24.1-pyhd8ed1ab_0.conda#428f6c7385636d72191cb4fa0e489503
+https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.23.0-pyhd8ed1ab_0.conda#a920e114c4c2ced2280e266da65ab5e6
 https://conda.anaconda.org/conda-forge/noarch/conda-package-handling-2.0.2-pyh38be061_0.conda#44800e9bd13143292097c65e57323038
-https://conda.anaconda.org/conda-forge/linux-64/keyring-24.2.0-py311h38be061_0.conda#b8eedb6181eff2dfeb34182330db1240
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
+https://conda.anaconda.org/conda-forge/linux-64/keyring-23.13.1-py311h38be061_0.conda#0dc0127b1daefefa5e2caa49dde5c230
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.13.0-pyhd8ed1ab_0.conda#9f0b2eb5f5dd2cec36d5342a80adfec0
+https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.12.11-pyhd8ed1ab_1.conda#e8f0410e0aa03342304357c5cc3bb75d
 https://conda.anaconda.org/conda-forge/linux-64/conda-22.9.0-py311h38be061_2.tar.bz2#d083486f8b405adad834ba22b9cd7340
 https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2#c99ae3abf501990769047b4b40a98f17
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
 https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda#99c98318c8646b08cc764f90ce98906e
-https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.13.0-pyhd8ed1ab_0.conda#3fd3d55ea862cc0736ac1cce6f44c2d1
+https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.12.11-pyhd8ed1ab_1.conda#9df660456c0076d27b802448f7ede78f
 https://conda.anaconda.org/conda-forge/linux-64/conda-build-3.24.0-py311h38be061_1.conda#729024de8c325a04a5632caefca4659e
-https://conda.anaconda.org/conda-forge/linux-64/mamba-1.4.9-py311h3072747_0.conda#f089b0415d7c4b26cb2f95eef2cefff0
+https://conda.anaconda.org/conda-forge/linux-64/mamba-1.4.2-py311h3072747_0.conda#e18f16d3d5b6c17edd412919da4ca559
 https://conda.anaconda.org/conda-forge/noarch/twine-4.0.2-pyhd8ed1ab_0.conda#e3a16168d6b9deefb8c1caa7943fb49e
 https://conda.anaconda.org/conda-forge/noarch/boa-0.14.0-pyhd8ed1ab_4.conda#58bd83f97618383b954808e3596bc202
-https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.1.1-pyhd8ed1ab_0.conda#492afee8c1d4e0d1fd314925a2a8dc89
+https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.0.0-pyhd8ed1ab_0.conda#b21d640094b5b8acb270334b5950cc74
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/meta/osx-64/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/meta/osx-64/conda.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,163 +1,159 @@
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
 https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.19.1-h0dc2134_0.conda#b3e62631b4e1b9801477523ce1d6f355
 https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
 https://conda.anaconda.org/conda-forge/osx-64/icu-72.1-h7336db1_0.conda#c9689510a50a4bb2ae978421671a125e
-https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
+https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.4-hd57cbcb_0.conda#195236e2eeb3b108e3b8eee47ad074fd
 https://conda.anaconda.org/conda-forge/osx-64/libev-4.33-haf1e3a3_1.tar.bz2#79dc2be110b2a3d1e97ec21f691c50ad
 https://conda.anaconda.org/conda-forge/osx-64/libexpat-2.5.0-hf0c8a7f_1.conda#6c81cb022780ee33435cca0127dd43c9
 https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
 https://conda.anaconda.org/conda-forge/osx-64/libiconv-1.17-hac89ed1_0.tar.bz2#691d103d11180486154af49c037b7ed9
-https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
+https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-hfd90126_4.tar.bz2#35eb3fce8d51ed3c1fd4122bad48250b
 https://conda.anaconda.org/conda-forge/osx-64/lzo-2.10-haf1e3a3_1000.tar.bz2#0b6bca372a95d6c602c7a922e928ce79
-https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
+https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.3-h96cf925_1.tar.bz2#76217ebfbb163ff2770a261f955a5861
 https://conda.anaconda.org/conda-forge/osx-64/patch-2.7.6-hbcf498f_1002.tar.bz2#6b43381b7baa13d12f7f8c1c5f815902
 https://conda.anaconda.org/conda-forge/noarch/pybind11-abi-4-hd8ed1ab_3.tar.bz2#878f923dd6acc8aeb47a75da6c4098be
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.11-3_cp311.conda#5e0a069a585445333868d2c6651c3b3f
 https://conda.anaconda.org/conda-forge/osx-64/reproc-14.2.4-hb7f2c08_0.conda#02b5e8cb2a08ac9c816a91b49070b8e2
 https://conda.anaconda.org/conda-forge/osx-64/ripgrep-13.0.0-hbbacdb1_2.tar.bz2#5ae3834efaaf5a666d45609fd51f85c5
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
 https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
 https://conda.anaconda.org/conda-forge/osx-64/fmt-9.1.0-hb8565cd_0.tar.bz2#310d897883dbdd88555d6321a4c2e6e8
 https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2#6016a8a1d0e63cac3de2c352cd40208b
 https://conda.anaconda.org/conda-forge/osx-64/liblief-0.12.3-hf0c8a7f_0.tar.bz2#82ccbb9725d912138cda0fa890146c55
-https://conda.anaconda.org/conda-forge/osx-64/libsolv-0.7.24-h7d26f99_1.conda#2e004cf14f0b4b458208362a4c54a056
+https://conda.anaconda.org/conda-forge/osx-64/libsolv-0.7.23-hbc0c0cd_0.conda#f032439375fa26ce944d8a70f81682a4
 https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
 https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.11.4-hd95e348_0.conda#681f8dda25e73a830d774a37b9839c85
 https://conda.anaconda.org/conda-forge/osx-64/lz4-c-1.9.4-hf0c8a7f_0.conda#aa04f7143228308662696ac24023f991
 https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/reproc-cpp-14.2.4-hf0c8a7f_0.conda#aef754e1111b466a15227427f65a1733
 https://conda.anaconda.org/conda-forge/osx-64/tapi-1100.0.11-h9ce4665_0.tar.bz2#f9ff42ccf809a21ba6f8607f8de36108
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
 https://conda.anaconda.org/conda-forge/osx-64/yaml-cpp-0.7.0-hf0c8a7f_2.tar.bz2#06c92b93b45ed2c842eb0893c5d2552a
-https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.2-h829000d_7.conda#b274ec4dbf15a6e20900e397610567a0
-https://conda.anaconda.org/conda-forge/osx-64/krb5-1.21.1-hb884880_0.conda#d4989bfe4cc9daec567a9935f5ad520b
+https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.2-hbc0c0cd_6.conda#40a188783d3c425bdccc9ae9104acbb8
+https://conda.anaconda.org/conda-forge/osx-64/krb5-1.20.1-h049b76e_0.conda#db11fa2968ef0837288fe2d7f5b77a50
 https://conda.anaconda.org/conda-forge/osx-64/libarchive-3.6.2-h0b5dc4a_1.conda#578c79bc28b8d1fa995e7cc0d3c7e965
-https://conda.anaconda.org/conda-forge/osx-64/libllvm16-16.0.6-he4b1e75_0.conda#23d9714cecfbe0b0493faac3dda4d18a
+https://conda.anaconda.org/conda-forge/osx-64/libllvm16-16.0.4-he4b1e75_0.conda#a61de681c7390e2571be3fd4475dc541
 https://conda.anaconda.org/conda-forge/osx-64/libnghttp2-1.52.0-he2ab024_0.conda#12ac7d100bf260263e30a019517f42a2
-https://conda.anaconda.org/conda-forge/osx-64/libssh2-1.11.0-hd019ec5_0.conda#ca3a72efba692c59a90d4b9fc0dfe774
-https://conda.anaconda.org/conda-forge/osx-64/python-3.11.4-h30d4d87_0_cpython.conda#e40b3075f85db0184d5f61d17c580ef7
+https://conda.anaconda.org/conda-forge/osx-64/libssh2-1.10.0-h47af595_3.tar.bz2#5a28624eeb7812b585b9e2d75f846ba2
+https://conda.anaconda.org/conda-forge/osx-64/python-3.11.3-h99528f9_0_cpython.conda#c3291f9411424fc587d53a2ea57fb075
 https://conda.anaconda.org/conda-forge/osx-64/sigtool-0.1.3-h88f4db0_0.tar.bz2#fbfb84b9de9a6939cb165c02c69b1865
 https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2#5f095bc6454094e96f146491fd03633b
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/noarch/cachy-0.3.0-pyhd8ed1ab_1.tar.bz2#5dfee17f24e2dfd18d7392b48c9351e2
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/osx-64/chardet-5.1.0-py311h6eed73b_0.conda#49dc5dea3f4dee3fd861b5da9a3241ed
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
-https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-unix_pyh707e725_0.conda#64dbb3b205546691a61204d1cfb208e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
+https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/crashtest-0.4.1-pyhd8ed1ab_0.tar.bz2#709a2295dd907bb34afb57d54320642f
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
-https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.7-pyhd8ed1ab_0.conda#12d8aae6994f342618443a8f05c652a0
+https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2#b65b4d50dbd2d50fa0aeac367ec9eed7
 https://conda.anaconda.org/conda-forge/osx-64/docutils-0.20.1-py311h6eed73b_0.conda#0536cbe889e20101b7f8e6d6b1dbcbf4
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
-https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda#53522ec72e6adae42bd373ef58357230
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.0-pyhd8ed1ab_0.conda#650f18a56f366dbf419c15b543592c2d
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/glob2-0.7-py_0.tar.bz2#1f3a88e65e61216e1d475135922dbf6a
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
 https://conda.anaconda.org/conda-forge/osx-64/ld64_osx-64-609-hbfe4790_13.conda#db5b18302e29e823656f2a7a69df7bd9
-https://conda.anaconda.org/conda-forge/osx-64/libcurl-8.2.0-h5f667d7_0.conda#d4a20b5cacc98af6020576836b408a82
+https://conda.anaconda.org/conda-forge/osx-64/libcurl-8.1.2-hbee3ae8_0.conda#d51e337da844262f9033c9a26452520f
 https://conda.anaconda.org/conda-forge/noarch/lockfile-0.12.2-py_1.tar.bz2#c104d98e09c47519950cffb8dd5b4f10
-https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.3-py311h2725bcf_0.conda#65b70928fcc2a81891ad1a8a6a7b085a
+https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.2-py311h5547dcb_0.conda#13091519d55d667506aaf413cffaff10
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/more-itertools-9.1.0-pyhd8ed1ab_0.conda#1698a717f83cfecf644a877c174c84bd
 https://conda.anaconda.org/conda-forge/osx-64/msgpack-python-1.0.5-py311hd2070f0_0.conda#d3a60c5422b7d61b2740c7c5df508c86
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2#a4eea5bff523f26442405bc5d1f52adb
 https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda#be1e9f1c65a1ed0f2ae9352fec99db64
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
 https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.5-py311h5547dcb_0.conda#d9b4565309f4f992b42bd99031044642
 https://conda.anaconda.org/conda-forge/osx-64/py-lief-0.12.3-py311h814d153_0.tar.bz2#cdd3df753cc25aebf41024db69bc585d
 https://conda.anaconda.org/conda-forge/osx-64/pycosat-0.6.4-py311h5547dcb_1.tar.bz2#229e642050372d50ebdc24e2265ce8b2
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
 https://conda.anaconda.org/conda-forge/noarch/pylev-1.4.0-pyhd8ed1ab_0.tar.bz2#edf8651c4379d9d1495ad6229622d150
+https://conda.anaconda.org/conda-forge/osx-64/pyrsistent-0.19.3-py311h5547dcb_0.conda#f114c0dab9f9c894b260297371124634
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
-https://conda.anaconda.org/conda-forge/osx-64/python-libarchive-c-5.0-py311h6eed73b_1.conda#3f3c0f0660f94687c02613f0dd3c4fb6
+https://conda.anaconda.org/conda-forge/osx-64/python-libarchive-c-4.0-py311h6eed73b_2.tar.bz2#3f638415e24cec2635e49949205c3d1a
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py311h5547dcb_5.tar.bz2#8d1e456914ce961119b07f396187a564
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-2.0.0-pyhd8ed1ab_0.tar.bz2#d337886e38f965bf97aaec382ff6db00
-https://conda.anaconda.org/conda-forge/osx-64/rpds-py-0.9.2-py311h299eb51_0.conda#bda1d1d8fce204234ed183b150dd51cc
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.7-py311h5547dcb_1.conda#fdae97fc41b9e4aa53d644cca8ba6c54
 https://conda.anaconda.org/conda-forge/osx-64/ruamel_yaml-0.15.80-py311h5547dcb_1008.tar.bz2#42c63993b1aaba9dc3c69a36e368d11c
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/smmap-3.0.5-pyh44b312d_0.tar.bz2#3a8dc70789709aa315325d5df06fb7e4
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.8-pyha770c72_0.conda#75838e8556166263a82038b51d01d5f1
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2#92facfec94bc02d6ccf42e7173831a36
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
-https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.1-pyhd8ed1ab_0.conda#7b517e7a6f0790337906c055aa97ca49
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/osx-64/cctools_osx-64-973.0.1-h5676edf_13.conda#86fa34ad281d649490b616b7026e8f7e
 https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py311ha86e640_3.conda#5967be4da33261eada7cc79593f71088
 https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2#72a46ffc25701c173932fd55cf0965d3
 https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyhd8ed1ab_2.conda#02abb7b66b02e8b9f5a9b05454400087
 https://conda.anaconda.org/conda-forge/noarch/gitdb-4.0.10-pyhd8ed1ab_0.conda#3706d2f3d7cb5dae600c833345a76132
 https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
-https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.3.0-pyhd8ed1ab_0.conda#e9f79248d30e942f7c358ff21a1790f5
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
+https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2#31e4a1506968d017229bdb64695013a1
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/noarch/joblib-1.3.0-pyhd8ed1ab_1.conda#fb4caf6da228ccc487350eade569abae
+https://conda.anaconda.org/conda-forge/noarch/joblib-1.2.0-pyhd8ed1ab_0.tar.bz2#7583652522d71ad78ba536bba06940eb
 https://conda.anaconda.org/conda-forge/osx-64/ld64-609-ha02d983_13.conda#019a988c615c39a44ebb92969fb2731f
-https://conda.anaconda.org/conda-forge/osx-64/libmamba-1.4.9-hc2ec11d_0.conda#24417139b9b9891af400f207132c36f3
-https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.30.0-pyhd8ed1ab_0.conda#13bf095e3ecd18999d65b4d3ac5b15d5
-https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.17.32-py311h2725bcf_0.conda#c5c5f7cf4ca556cfdb605e05cfbc8bec
+https://conda.anaconda.org/conda-forge/osx-64/libmamba-1.4.2-h9d281b0_0.conda#f7963359f4abf1ee8b569106aa5325e7
+https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
+https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.17.31-py311h2725bcf_0.conda#a81b5091605ed21fb00f03a110c14cf8
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
-https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda#578ae086f225bc2380c79f3b551ff2f7
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
 https://conda.anaconda.org/conda-forge/osx-64/brotlipy-0.7.0-py311h5547dcb_1005.tar.bz2#5f97ac938a90d06eebea42c321abe0d7
 https://conda.anaconda.org/conda-forge/osx-64/cctools-973.0.1-h40f6528_13.conda#846229d9e82b6db32fc37313f1306430
 https://conda.anaconda.org/conda-forge/osx-64/cmarkgfm-0.8.0-py311h5547dcb_2.tar.bz2#69cd422f24f98fb4f8a9a896798bff06
-https://conda.anaconda.org/conda-forge/osx-64/cryptography-41.0.2-py311h892b619_0.conda#f3975c6d2c0406f204760ac434e3b785
+https://conda.anaconda.org/conda-forge/osx-64/cryptography-41.0.0-py311h892b619_0.conda#ba40bc0ceacca822aab7c7f9a021198d
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.32-pyhd8ed1ab_0.conda#5809a12901d57388444c3293c975d0bb
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.7.1-pyhd8ed1ab_0.conda#7c27ea1bdbe520bb830dcadd59f55cbf
-https://conda.anaconda.org/conda-forge/osx-64/libmambapy-1.4.9-py311h266e549_0.conda#63ed56aa9922af8fe8899e8d60d28abc
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
-https://conda.anaconda.org/conda-forge/osx-64/pydantic-core-2.3.0-py311h299eb51_0.conda#4d627a3cb4e813bcc47256c9a01bf90f
-https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
+https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.31-pyhd8ed1ab_0.conda#f6e6b482110246a81c3f03e81c68752d
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
+https://conda.anaconda.org/conda-forge/osx-64/libmambapy-1.4.2-py311hcc19a12_0.conda#8c03cef57bc55e0153406fe89149fe9e
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
+https://conda.anaconda.org/conda-forge/osx-64/pydantic-1.10.8-py311h2725bcf_0.conda#90be10c21a9af4548c1bbf1e00dbb82a
+https://conda.anaconda.org/conda-forge/noarch/rich-13.3.5-pyhd8ed1ab_0.conda#2e40a02ad28e34f26cee2a72042843db
 https://conda.anaconda.org/conda-forge/noarch/watchgod-0.8.2-pyhd8ed1ab_0.tar.bz2#8bf811791ff4ea8b6368b8ff451c6421
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
-https://conda.anaconda.org/conda-forge/osx-64/zstandard-0.19.0-py311h26cfcfc_2.conda#864dbcdc4f7a00fee5a84d4655bc4799
+https://conda.anaconda.org/conda-forge/osx-64/zstandard-0.19.0-py311hebd4beb_1.conda#b0d4f55c803038fd429494acf684e6ef
 https://conda.anaconda.org/conda-forge/noarch/conda-package-streaming-0.8.0-pyhd8ed1ab_0.conda#ebe3230a4c1e135954eee4fb6ef8cded
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.18.4-pyhd8ed1ab_0.conda#7356151a32ebd9a20158d2f26d224bfa
-https://conda.anaconda.org/conda-forge/osx-64/keyring-24.2.0-py311h6eed73b_0.conda#8ba03d96e54958cd02110dc032d0bda2
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
-https://conda.anaconda.org/conda-forge/noarch/pydantic-2.0.3-pyhd8ed1ab_1.conda#77753c350c42e70dd3e9919dd8099fc7
+https://conda.anaconda.org/conda-forge/osx-64/keyring-23.13.1-py311h6eed73b_0.conda#ae2618c59c8f3481aa7014de862c6d57
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
 https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
-https://conda.anaconda.org/conda-forge/noarch/readme_renderer-40.0-pyhd8ed1ab_0.conda#9ba2b509f6fe88364512caa9089ea886
-https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.24.1-pyhd8ed1ab_0.conda#428f6c7385636d72191cb4fa0e489503
+https://conda.anaconda.org/conda-forge/noarch/readme_renderer-37.3-pyhd8ed1ab_0.tar.bz2#82e8ab317fe8f1d2a944688438dce868
+https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.23.0-pyhd8ed1ab_0.conda#a920e114c4c2ced2280e266da65ab5e6
 https://conda.anaconda.org/conda-forge/noarch/conda-package-handling-2.0.2-pyh38be061_0.conda#44800e9bd13143292097c65e57323038
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.13.0-pyhd8ed1ab_0.conda#9f0b2eb5f5dd2cec36d5342a80adfec0
+https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.12.11-pyhd8ed1ab_1.conda#e8f0410e0aa03342304357c5cc3bb75d
 https://conda.anaconda.org/conda-forge/osx-64/conda-22.9.0-py311h6eed73b_2.tar.bz2#d18ef2c39925384887a22371e00b1160
 https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2#c99ae3abf501990769047b4b40a98f17
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
 https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda#99c98318c8646b08cc764f90ce98906e
-https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.13.0-pyhd8ed1ab_0.conda#3fd3d55ea862cc0736ac1cce6f44c2d1
+https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.12.11-pyhd8ed1ab_1.conda#9df660456c0076d27b802448f7ede78f
 https://conda.anaconda.org/conda-forge/osx-64/conda-build-3.24.0-py311h6eed73b_1.conda#55ec148592ba46f0abd76f2743b71eb3
-https://conda.anaconda.org/conda-forge/osx-64/mamba-1.4.9-py311h8082e30_0.conda#fc8f6120311f278ae53dcccbd97c39fa
+https://conda.anaconda.org/conda-forge/osx-64/mamba-1.4.2-py311h8082e30_0.conda#ec6b2a4cd27737c34604c9faf5ac0f2e
 https://conda.anaconda.org/conda-forge/noarch/twine-4.0.2-pyhd8ed1ab_0.conda#e3a16168d6b9deefb8c1caa7943fb49e
 https://conda.anaconda.org/conda-forge/noarch/boa-0.14.0-pyhd8ed1ab_4.conda#58bd83f97618383b954808e3596bc202
-https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.1.1-pyhd8ed1ab_0.conda#492afee8c1d4e0d1fd314925a2a8dc89
+https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.0.0-pyhd8ed1ab_0.conda#b21d640094b5b8acb270334b5950cc74
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/meta/win-64/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/meta/win-64/conda.lock`

 * *Files 4% similar despite different names*

```diff
@@ -5,158 +5,154 @@
 https://conda.anaconda.org/conda-forge/noarch/pybind11-abi-4-hd8ed1ab_3.tar.bz2#878f923dd6acc8aeb47a75da6c4098be
 https://conda.anaconda.org/conda-forge/win-64/python_abi-3.11-3_cp311.conda#fd1634ba85cfea9376e1fc02d6f592e9
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
 https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
 https://conda.anaconda.org/conda-forge/win-64/m2-msys2-runtime-2.5.0.17080.65c939c-3.tar.bz2#ce25c58bc90071bf71f3d472cb8dfbce
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gmp-6.1.0-2.tar.bz2#53a1c73e1e3d185516d7e3af177596d9
 https://conda.anaconda.org/conda-forge/win-64/m2w64-libwinpthread-git-5.0.0.4634.697f757-2.tar.bz2#774130a326dee16f1ceb05cc687ee4f0
-https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.36.32532-hfdfe4a8_17.conda#91c1ecaf3996889532fc0456178b1058
+https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.34.31931-h5081d32_16.conda#22125178654c6a8a393f9743d585704b
 https://conda.anaconda.org/conda-forge/win-64/m2-patch-2.7.5-2.tar.bz2#f5159110837c3e221146e623f3c44f1c
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-core-5.3.0-7.tar.bz2#4289d80fb4d272f1f3b56cfe87ac90bd
-https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h64f974e_17.conda#67ff6791f235bb606659bf2a5c169191
-https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.36.32532-h05e6639_17.conda#4618046c39f7c81861e53ded842e738a
+https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hb25d44b_16.conda#ea326b37e3bd6d2616988e09f3a9396c
+https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.34.31931-hed1258a_16.conda#0374eae69b6dbfb27c3dc27167109eb4
 https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
 https://conda.anaconda.org/conda-forge/win-64/fmt-9.1.0-h181d51b_0.tar.bz2#31a20cf261b2bd0a76d670db1b3e6fa1
 https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
 https://conda.anaconda.org/conda-forge/win-64/libiconv-1.17-h8ffe710_0.tar.bz2#050119977a86e4856f0416e2edcf81bb
 https://conda.anaconda.org/conda-forge/win-64/liblief-0.12.3-h63175ca_0.tar.bz2#37f670590cc40b69393894cca459e346
 https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.42.0-hcfcfb64_0.conda#9a71d93deb99cc09d8939d5235b5909a
-https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
+https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_4.tar.bz2#0cc5c5cc64ee1637f37f8540a175854c
 https://conda.anaconda.org/conda-forge/win-64/lz4-c-1.9.4-hcfcfb64_0.conda#e34720eb20a33fc3bfb8451dd837ab7a
 https://conda.anaconda.org/conda-forge/win-64/lzo-2.10-he774522_1000.tar.bz2#d5cf4b7eaa52316f135eed9e8548ad57
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libgfortran-5.3.0-6.tar.bz2#066552ac6b907ec6d72c0ddab29050dc
 https://conda.anaconda.org/conda-forge/win-64/openssl-3.1.1-hcfcfb64_1.conda#1d913a5de46c6b2f7e4cfbd26b106b8b
 https://conda.anaconda.org/conda-forge/win-64/reproc-14.2.4-hcfcfb64_0.conda#059e1351c1affff15b16aec51c6967a6
 https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2#c69a5047cc9291ae40afd4a1ad6f0c0f
 https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
 https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
 https://conda.anaconda.org/conda-forge/win-64/yaml-cpp-0.7.0-h63175ca_2.tar.bz2#27c8a78ba0cd18268cfc7b04c5512162
-https://conda.anaconda.org/conda-forge/win-64/krb5-1.21.1-heb0366b_0.conda#66fdc07e563f5ae3f6d82c58f492f776
-https://conda.anaconda.org/conda-forge/win-64/libsolv-0.7.24-h12be248_1.conda#9b9e1559d74271bff7ac4eb51cfe56c4
-https://conda.anaconda.org/conda-forge/win-64/libssh2-1.11.0-h7dfc565_0.conda#dc262d03aae04fe26825062879141a41
+https://conda.anaconda.org/conda-forge/win-64/krb5-1.20.1-heb0366b_0.conda#a07b05ee8f451ab15698397185efe989
+https://conda.anaconda.org/conda-forge/win-64/libsolv-0.7.23-h12be248_0.conda#4955aac5971a11e1b79c47912645b9e2
+https://conda.anaconda.org/conda-forge/win-64/libssh2-1.10.0-h9a1e1f7_3.tar.bz2#c2b344e960a173c777bb3ed172c38cd8
 https://conda.anaconda.org/conda-forge/win-64/libxml2-2.11.4-hc3477c8_0.conda#586627982a63815637f871a6360fe3f9
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-5.3.0-7.tar.bz2#fe759119b8b3bfa720b8762c6fdc35de
-https://conda.anaconda.org/conda-forge/win-64/python-3.11.4-h2628c8c_0_cpython.conda#3187a32fba79e835f099ecea054026f4
+https://conda.anaconda.org/conda-forge/win-64/python-3.11.3-h2628c8c_0_cpython.conda#8f82e0e0ba51bed311f28eb6450393f6
 https://conda.anaconda.org/conda-forge/win-64/reproc-cpp-14.2.4-h63175ca_0.conda#a9ee9bbbbda9b32ec690c4909146770d
-https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.2-h12be248_7.conda#f3c3879d8cda1c5a6885435dd48a470e
+https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.2-h12be248_6.conda#62826565682d013b3e2346aaf7bded0e
 https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2#5f095bc6454094e96f146491fd03633b
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/noarch/cachy-0.3.0-pyhd8ed1ab_1.tar.bz2#5dfee17f24e2dfd18d7392b48c9351e2
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
 https://conda.anaconda.org/conda-forge/win-64/chardet-5.1.0-py311h1ea47a8_0.conda#bb0899c06c1df8fc7802caab197b0963
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/crashtest-0.4.1-pyhd8ed1ab_0.tar.bz2#709a2295dd907bb34afb57d54320642f
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
-https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.7-pyhd8ed1ab_0.conda#12d8aae6994f342618443a8f05c652a0
+https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2#b65b4d50dbd2d50fa0aeac367ec9eed7
 https://conda.anaconda.org/conda-forge/win-64/docutils-0.20.1-py311h1ea47a8_0.conda#851f4c302cc7f5a617cc03a3c2090634
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
-https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda#53522ec72e6adae42bd373ef58357230
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.0-pyhd8ed1ab_0.conda#650f18a56f366dbf419c15b543592c2d
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/glob2-0.7-py_0.tar.bz2#1f3a88e65e61216e1d475135922dbf6a
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
 https://conda.anaconda.org/conda-forge/win-64/libarchive-3.6.2-h6f8411a_1.conda#314124476882f64abc20b76148d2909b
-https://conda.anaconda.org/conda-forge/win-64/libcurl-8.2.0-hd5e4a3a_0.conda#af51ef2e3436c62039fdbb6c8116ec7e
+https://conda.anaconda.org/conda-forge/win-64/libcurl-8.1.2-h68f0423_0.conda#94b9b7d0e882461fdb72d8d4e7441746
 https://conda.anaconda.org/conda-forge/noarch/lockfile-0.12.2-py_1.tar.bz2#c104d98e09c47519950cffb8dd5b4f10
-https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.3-py311ha68e1ae_0.conda#db2c2f72a83bdc5b70947964e1ddc8bb
+https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.2-py311ha68e1ae_0.conda#96e7ffe6ea438ba4517152abe3b39874
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/win-64/menuinst-1.4.19-py311h1ea47a8_1.tar.bz2#8eb00075c8acb7dd264c4a8537b89549
 https://conda.anaconda.org/conda-forge/noarch/more-itertools-9.1.0-pyhd8ed1ab_0.conda#1698a717f83cfecf644a877c174c84bd
 https://conda.anaconda.org/conda-forge/win-64/msgpack-python-1.0.5-py311h005e61a_0.conda#01a252f384a5d1ad338cff1184d9a9c0
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2#a4eea5bff523f26442405bc5d1f52adb
 https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda#be1e9f1c65a1ed0f2ae9352fec99db64
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
 https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.5-py311ha68e1ae_0.conda#f1a1eecd1bb4f431df5b9b6d8a152efd
 https://conda.anaconda.org/conda-forge/win-64/py-lief-0.12.3-py311h12c1d0e_0.tar.bz2#e3bbee7381ef4ed51db5832641c26893
 https://conda.anaconda.org/conda-forge/win-64/pycosat-0.6.4-py311ha68e1ae_1.tar.bz2#c7af04cd8a66f6d782982751200239d0
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
 https://conda.anaconda.org/conda-forge/noarch/pylev-1.4.0-pyhd8ed1ab_0.tar.bz2#edf8651c4379d9d1495ad6229622d150
+https://conda.anaconda.org/conda-forge/win-64/pyrsistent-0.19.3-py311ha68e1ae_0.conda#3f2780a49f0b4bb2c622f7cf098e3d06
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
-https://conda.anaconda.org/conda-forge/win-64/pywin32-ctypes-0.2.2-py311h1ea47a8_0.conda#93204e67d63d9ea4ef2b878172222b74
+https://conda.anaconda.org/conda-forge/win-64/pywin32-ctypes-0.2.0-py311h1ea47a8_1006.tar.bz2#86ee973a16f5449d9ded34b512331dce
 https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py311ha68e1ae_5.tar.bz2#0c97d59d54eb52e170224b3de6ade906
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-2.0.0-pyhd8ed1ab_0.tar.bz2#d337886e38f965bf97aaec382ff6db00
 https://conda.anaconda.org/conda-forge/win-64/ripgrep-13.0.0-h7f3b576_2.tar.bz2#8f37f34d42c5675df21caf041597e792
-https://conda.anaconda.org/conda-forge/win-64/rpds-py-0.9.2-py311hc37eb10_0.conda#d2d75b1d27bcd4f7b6d049b32b2f7530
 https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml.clib-0.2.7-py311ha68e1ae_1.conda#654fbe603c79490699cd7447e4627aee
 https://conda.anaconda.org/conda-forge/win-64/ruamel_yaml-0.15.80-py311ha68e1ae_1008.tar.bz2#c1c3cca1078977cfa12d36f32eb58fbe
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/smmap-3.0.5-pyh44b312d_0.tar.bz2#3a8dc70789709aa315325d5df06fb7e4
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.8-pyha770c72_0.conda#75838e8556166263a82038b51d01d5f1
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2#92facfec94bc02d6ccf42e7173831a36
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
 https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
-https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.1-pyhd8ed1ab_0.conda#7b517e7a6f0790337906c055aa97ca49
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py311h7d9ee11_3.conda#a8524727eb956b4741e25a64af79edb8
-https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-win_pyh7428d3b_0.conda#c1e57b6771510a3d2648ed6e76277391
+https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-win_pyhd8ed1ab_2.tar.bz2#6b58680207b526c42dcff68b543803dd
 https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyhd8ed1ab_2.conda#02abb7b66b02e8b9f5a9b05454400087
 https://conda.anaconda.org/conda-forge/noarch/gitdb-4.0.10-pyhd8ed1ab_0.conda#3706d2f3d7cb5dae600c833345a76132
 https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
-https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.3.0-pyhd8ed1ab_0.conda#e9f79248d30e942f7c358ff21a1790f5
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
+https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2#31e4a1506968d017229bdb64695013a1
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/noarch/joblib-1.3.0-pyhd8ed1ab_1.conda#fb4caf6da228ccc487350eade569abae
-https://conda.anaconda.org/conda-forge/win-64/libmamba-1.4.9-ha24f096_0.conda#c632423ab1fd294a174f4324cc47614c
-https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda#93a8e71256479c62074356ef6ebf501b
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
+https://conda.anaconda.org/conda-forge/noarch/joblib-1.2.0-pyhd8ed1ab_0.tar.bz2#7583652522d71ad78ba536bba06940eb
+https://conda.anaconda.org/conda-forge/win-64/libmamba-1.4.2-h8a7d157_0.conda#beac6b9e25bbaf8d22b13df786891192
+https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
-https://conda.anaconda.org/conda-forge/win-64/python-libarchive-c-5.0-py311h1ea47a8_1.conda#659bc6061b6dc9ef0436ee22d64e8ac2
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.30.0-pyhd8ed1ab_0.conda#13bf095e3ecd18999d65b4d3ac5b15d5
-https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml-0.17.32-py311ha68e1ae_0.conda#1a51f29331338bfde51127db204d7757
+https://conda.anaconda.org/conda-forge/win-64/python-libarchive-c-4.0-py311h1ea47a8_2.tar.bz2#587f3af8e6a1d545a1b3b5a2617435f7
+https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml-0.17.31-py311ha68e1ae_0.conda#211e024535a77ae712ad05d2ec7ac4fe
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
-https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.5.0-pyhd8ed1ab_0.conda#578ae086f225bc2380c79f3b551ff2f7
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
 https://conda.anaconda.org/conda-forge/win-64/brotlipy-0.7.0-py311ha68e1ae_1005.tar.bz2#dd9604ece454103e7210110c6d343e37
 https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2#72a46ffc25701c173932fd55cf0965d3
 https://conda.anaconda.org/conda-forge/win-64/cmarkgfm-0.8.0-py311ha68e1ae_2.tar.bz2#206cb594ef199270b7e0d3d17aa87cbe
-https://conda.anaconda.org/conda-forge/win-64/cryptography-41.0.2-py311h28e9c30_0.conda#ea9fc978bfef9ceeb950687f0063c460
+https://conda.anaconda.org/conda-forge/win-64/cryptography-41.0.0-py311h28e9c30_0.conda#0ce847348dc2b7127a1046701a06190c
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.32-pyhd8ed1ab_0.conda#5809a12901d57388444c3293c975d0bb
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.7.1-pyhd8ed1ab_0.conda#7c27ea1bdbe520bb830dcadd59f55cbf
-https://conda.anaconda.org/conda-forge/win-64/libmambapy-1.4.9-py311h29ee5fe_0.conda#7c0314b43476618fefcbfff8f58c4e87
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
-https://conda.anaconda.org/conda-forge/win-64/pydantic-core-2.3.0-py311hc37eb10_0.conda#9259b7da3dde8b3c247e944cfbe13b87
-https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
+https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.31-pyhd8ed1ab_0.conda#f6e6b482110246a81c3f03e81c68752d
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
+https://conda.anaconda.org/conda-forge/win-64/libmambapy-1.4.2-py311h29ee5fe_0.conda#1d07b16b07e0b3fa5d2e145b221e4f1d
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
+https://conda.anaconda.org/conda-forge/win-64/pydantic-1.10.8-py311ha68e1ae_0.conda#db03940169f3c8ac02330ddbfe02be35
+https://conda.anaconda.org/conda-forge/noarch/rich-13.3.5-pyhd8ed1ab_0.conda#2e40a02ad28e34f26cee2a72042843db
 https://conda.anaconda.org/conda-forge/noarch/watchgod-0.8.2-pyhd8ed1ab_0.tar.bz2#8bf811791ff4ea8b6368b8ff451c6421
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
-https://conda.anaconda.org/conda-forge/win-64/zstandard-0.19.0-py311he5d195f_2.conda#7ef609e9bfd58d18962d7b7c0c529638
+https://conda.anaconda.org/conda-forge/win-64/zstandard-0.19.0-py311he5d195f_1.conda#af889af78c5389e344392e305b4d7bc7
 https://conda.anaconda.org/conda-forge/noarch/conda-package-streaming-0.8.0-pyhd8ed1ab_0.conda#ebe3230a4c1e135954eee4fb6ef8cded
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.18.4-pyhd8ed1ab_0.conda#7356151a32ebd9a20158d2f26d224bfa
-https://conda.anaconda.org/conda-forge/win-64/keyring-24.2.0-py311h1ea47a8_0.conda#6a5239529cb5af3437bdd24c1082c2eb
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
-https://conda.anaconda.org/conda-forge/noarch/pydantic-2.0.3-pyhd8ed1ab_1.conda#77753c350c42e70dd3e9919dd8099fc7
+https://conda.anaconda.org/conda-forge/win-64/keyring-23.13.1-py311h1ea47a8_0.conda#ff14a49b769ea59ee6709a890e17f317
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
 https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
-https://conda.anaconda.org/conda-forge/noarch/readme_renderer-40.0-pyhd8ed1ab_0.conda#9ba2b509f6fe88364512caa9089ea886
-https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.24.1-pyhd8ed1ab_0.conda#428f6c7385636d72191cb4fa0e489503
+https://conda.anaconda.org/conda-forge/noarch/readme_renderer-37.3-pyhd8ed1ab_0.tar.bz2#82e8ab317fe8f1d2a944688438dce868
+https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.23.0-pyhd8ed1ab_0.conda#a920e114c4c2ced2280e266da65ab5e6
 https://conda.anaconda.org/conda-forge/noarch/conda-package-handling-2.0.2-pyh38be061_0.conda#44800e9bd13143292097c65e57323038
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.13.0-pyhd8ed1ab_0.conda#9f0b2eb5f5dd2cec36d5342a80adfec0
+https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.12.11-pyhd8ed1ab_1.conda#e8f0410e0aa03342304357c5cc3bb75d
 https://conda.anaconda.org/conda-forge/win-64/conda-22.9.0-py311h1ea47a8_2.tar.bz2#b10f47d78cb51f295ee9e6f3a611fa17
 https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2#c99ae3abf501990769047b4b40a98f17
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
 https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda#99c98318c8646b08cc764f90ce98906e
-https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.13.0-pyhd8ed1ab_0.conda#3fd3d55ea862cc0736ac1cce6f44c2d1
+https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.12.11-pyhd8ed1ab_1.conda#9df660456c0076d27b802448f7ede78f
 https://conda.anaconda.org/conda-forge/win-64/conda-build-3.24.0-py311h1ea47a8_1.conda#7ea047a304cca9c56288743ec167607c
-https://conda.anaconda.org/conda-forge/win-64/mamba-1.4.9-py311h8cb466b_0.conda#289b9796d4d827835bf1e32e14cf64dd
+https://conda.anaconda.org/conda-forge/win-64/mamba-1.4.2-py311h8cb466b_0.conda#5eea8bf32794bfd136e989e12dd5a908
 https://conda.anaconda.org/conda-forge/noarch/twine-4.0.2-pyhd8ed1ab_0.conda#e3a16168d6b9deefb8c1caa7943fb49e
 https://conda.anaconda.org/conda-forge/noarch/boa-0.14.0-pyhd8ed1ab_4.conda#58bd83f97618383b954808e3596bc202
-https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.1.1-pyhd8ed1ab_0.conda#492afee8c1d4e0d1fd314925a2a8dc89
+https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.0.0-pyhd8ed1ab_0.conda#b21d640094b5b8acb270334b5950cc74
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/test/linux-64/py3.11/lab3/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/linux-64/py3.11/lab3/conda.lock`

 * *Files 6% similar despite different names*

```diff
@@ -1,169 +1,171 @@
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
 https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.1.0-hfd8a6a1_0.conda#067bcc23164642f4c226da631f2a2e1d
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-12.2.0-h46fd767_19.tar.bz2#1030b1f38c129f2634eae026f704fe60
 https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.11-3_cp311.conda#c2e2630ddb68cf52eec74dc7dfab20b5
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-12.2.0-h65d4601_19.tar.bz2#cedcee7c064c01c403f962c9e8d3c373
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-12.2.0-h65d4601_19.tar.bz2#e4c94f80aef025c17ab0828cd85ef535
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
-https://conda.anaconda.org/conda-forge/linux-64/firefox-115.0-hd3aeb46_0.conda#816707575d8de0052347e2fa5a19c5f7
+https://conda.anaconda.org/conda-forge/linux-64/firefox-113.0-h59595ed_0.conda#262f91a0dfca92813a3d469cc5453f61
 https://conda.anaconda.org/conda-forge/linux-64/geckodriver-0.33.0-hd2f7af9_0.conda#83664049f2b276cc23bd67d41eb9a4ee
-https://conda.anaconda.org/conda-forge/linux-64/gmp-6.2.1-h58526e2_0.tar.bz2#b94cf2db16066b242ebd26db2facbd56
 https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2#9194c9bf9428035a05352d031462eae4
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
 https://conda.anaconda.org/conda-forge/linux-64/libuv-1.44.2-h166bdaf_0.tar.bz2#e5cb4fe581a18ca2185a016eb848fc00
-https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
-https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
+https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-h166bdaf_4.tar.bz2#f3f9de449d32ca9b9c66a22863c96f41
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h27087fc_1.tar.bz2#4acfc691e64342b9dae57cf2adc63238
 https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
 https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
 https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2#4ae4d7795d33e02bd20f6b23d91caf82
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2#04bac51ba35ea023dc48af73c1c88c25
 https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
+https://conda.anaconda.org/conda-forge/linux-64/pandoc-2.19.2-h32600fe_2.conda#326f46f36d15c44cff5f81d505cb717f
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
-https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
-https://conda.anaconda.org/conda-forge/linux-64/nodejs-18.16.1-hf52ce11_0.conda#23ed78db48ed08c94e5449f6661d65e6
-https://conda.anaconda.org/conda-forge/linux-64/pandoc-3.1.3-h32600fe_0.conda#8287aeb8462e2d4b235eff788e75919d
-https://conda.anaconda.org/conda-forge/linux-64/python-3.11.4-hab00c5b_0_cpython.conda#1c628861a2a126b9fc9363ca1b7d014e
+https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-h166bdaf_4.tar.bz2#4b11e365c0275b808be78b30f904e295
+https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2#e5613f2bc717e9945840ff474419b8e4
+https://conda.anaconda.org/conda-forge/linux-64/nodejs-18.15.0-h4abf6b9_1.conda#2aabafd88f6876a57c45c00598715ac4
+https://conda.anaconda.org/conda-forge/linux-64/python-3.11.3-h2755cc3_0_cpython.conda#37005ea5f68df6a8a381b70cf4d4a160
 https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
+https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.0.9-py311ha362b79_9.conda#ced5340f5dc6cff43a80deac8d0e398f
+https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_8.tar.bz2#2ff08978892a3e8b954397c461f18418
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py311hcafe171_0.conda#f4c810ad9d791c8df5ad900ed74b085b
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/linux-64/docutils-0.20.1-py311h38be061_0.conda#207175b7d514d42f977ec505800d6824
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_robotmode-0.3.1-pyhd8ed1ab_0.tar.bz2#081f1505925bd5ff080864f4281c28a6
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
-https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py311h459d7ec_0.conda#9904dc4adb5d547cb21e136f98cb24b0
-https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
-https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.2-py311h2582759_0.conda#adb20bd57069614552adac60a020c36d
+https://conda.anaconda.org/conda-forge/noarch/mistune-2.0.5-pyhd8ed1ab_0.conda#61a07195cfc935f1c1901d8ecf4af441
+https://conda.anaconda.org/conda-forge/noarch/natsort-8.3.1-pyhd8ed1ab_0.conda#8c53149aa69bfeb045f28c92a2b2ddc7
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda#02153b6b760bbec00cfe9e4c97993d06
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
 https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py311h2582759_0.conda#a90f8e278c1cd7064b2713e6b7db87e6
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
+https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py311h2582759_0.conda#e53876b66dcc4ba8a0afa63cd8502ac3
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py311hd4cff14_5.tar.bz2#da8769492e423103c59f469f4f17f8d9
 https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py311h75c88c4_0.conda#db94a7a9e865fbfde8c023b6e8958bb2
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
-https://conda.anaconda.org/conda-forge/noarch/robotframework-6.1-pyhd8ed1ab_0.conda#e383bebdc0d8fea4ecf9c9e01d0959fe
-https://conda.anaconda.org/conda-forge/linux-64/rpds-py-0.9.2-py311h46250e7_0.conda#bcf66b5abaec47198b42cdd0bb968540
+https://conda.anaconda.org/conda-forge/noarch/robotframework-6.0.2-pyhd8ed1ab_1.conda#b4dcead8c5a99a14733d9b1ba5b7db09
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh41d4057_0.conda#ada5a17adcd10be4fc7e37e4166ba0e2
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py311h459d7ec_0.conda#12b1c374ee90a1aa11ea921858394dc8
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.2-pyhd8ed1ab_0.conda#bfe7e7cd1476092f51efbcde15dfb110
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
 https://conda.anaconda.org/conda-forge/linux-64/y-py-0.5.9-py311hfe55011_0.conda#216fb67bd1016b05fe33672bd71937a8
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py311h409f033_3.conda#9025d0786dbbe4bc91fd8e85502decce
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
 https://conda.anaconda.org/conda-forge/linux-64/coverage-7.2.7-py311h459d7ec_0.conda#3c2c65575c28b23afc5e4ff721a2fc9f
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.30.0-pyhd8ed1ab_0.conda#13bf095e3ecd18999d65b4d3ac5b15d5
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.2.0-pyhd8ed1ab_0.conda#c9e9064ab45ffb46f7a96834d9e7626d
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.4-pyhd8ed1ab_0.conda#18badd8fa3648d1beb1fcc7f2e0f756e
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.2-pyhd8ed1ab_0.conda#81a763f3c64fe6d5f32e033b0325265d
 https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
 https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py311hd4cff14_3.tar.bz2#5159e874f65ac382773d2b534a1d7b80
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.7.1-pyhd8ed1ab_0.conda#7c27ea1bdbe520bb830dcadd59f55cbf
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.15.0-pyhd8ed1ab_0.conda#02e7912139fb64828d18d07c43dcbad0
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.2-py311h38be061_0.conda#dcbfe3a95e8b99ec743e26a75d8c9cf4
+https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.0-py311h38be061_1.tar.bz2#0564e63c41c0527f8085a572a931f1e6
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.18.4-pyhd8ed1ab_0.conda#7356151a32ebd9a20158d2f26d224bfa
-https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.1-py311h38be061_0.conda#0cf8259b01ede82c76007996f73f89ed
+https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.0-py311h38be061_0.conda#1dd43a18a75d59206019e2a2a28555e5
+https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
-https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.2-pyhd8ed1ab_0.conda#4ec732d2264373773a5feaea477128a8
 https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
-https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.8.0-pyhd8ed1ab_0.conda#1ca43103a08456b19222d93fd9d119ac
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
-https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh41d4057_0.conda#0a0b0d8177c4a209017b356439292db8
+https://conda.anaconda.org/conda-forge/noarch/ipython-8.13.2-pyh41d4057_0.conda#e8563c13eee80a5f1c7bdfc2a1b20077
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
-https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh71e2992_0.conda#cfafc9387c32a43a1b6d63633489cbc9
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda#32dde1678bb003c90d4bc0c2dbd21814
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.1-pyhd8ed1ab_1.conda#796b056965d7146bcac082fa2a83943d
+https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_0.conda#15700afca8f7ab35542e9c1af63568f1
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh210e3f2_0.conda#4b57b688e22d094d1479a35543c18e93
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.4.0-pyhd8ed1ab_0.conda#4456e6030a8309bdad57569b0170b6a3
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.4.0-pyhd8ed1ab_0.conda#127c702e1b1eff595be82bc6a78cfce0
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.1-pyhd8ed1ab_1.conda#95d9d1523df069792cd059f412be0d6e
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.22.1-pyhd8ed1ab_0.conda#fc7172a6742a7c3c4331ddd7ed463ffc
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.4.0-pyhd8ed1ab_0.conda#a86727968b41c20dd3d73b91632e77dc
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_ydoc-0.8.0-pyhd8ed1ab_0.conda#780280d42fbcb2eaf654a6ba7a3e5bb5
 https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
 https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.5-pyhd8ed1ab_0.conda#82299e1d33c6f130688f90880e6b3b4f
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.4-pyhd8ed1ab_0.conda#e66d4a6e36fcc92fe266932bf85fd35a
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/test/linux-64/py3.11/lab4/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/linux-64/py3.8/lab4/conda.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,157 +1,153 @@
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
 https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.1.0-hfd8a6a1_0.conda#067bcc23164642f4c226da631f2a2e1d
-https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.11-3_cp311.conda#c2e2630ddb68cf52eec74dc7dfab20b5
-https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-12.2.0-h46fd767_19.tar.bz2#1030b1f38c129f2634eae026f704fe60
+https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.8-3_cp38.conda#2f3f7af062b42d664117662612022204
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-12.2.0-h65d4601_19.tar.bz2#cedcee7c064c01c403f962c9e8d3c373
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-12.2.0-h65d4601_19.tar.bz2#e4c94f80aef025c17ab0828cd85ef535
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
-https://conda.anaconda.org/conda-forge/linux-64/firefox-115.0-hd3aeb46_0.conda#816707575d8de0052347e2fa5a19c5f7
+https://conda.anaconda.org/conda-forge/linux-64/firefox-113.0-h59595ed_0.conda#262f91a0dfca92813a3d469cc5453f61
 https://conda.anaconda.org/conda-forge/linux-64/geckodriver-0.33.0-hd2f7af9_0.conda#83664049f2b276cc23bd67d41eb9a4ee
 https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
-https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2#9194c9bf9428035a05352d031462eae4
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
 https://conda.anaconda.org/conda-forge/linux-64/libuv-1.44.2-h166bdaf_0.tar.bz2#e5cb4fe581a18ca2185a016eb848fc00
-https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
-https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
+https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-h166bdaf_4.tar.bz2#f3f9de449d32ca9b9c66a22863c96f41
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h27087fc_1.tar.bz2#4acfc691e64342b9dae57cf2adc63238
 https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
 https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
 https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2#4ae4d7795d33e02bd20f6b23d91caf82
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2#04bac51ba35ea023dc48af73c1c88c25
 https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
-https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
-https://conda.anaconda.org/conda-forge/linux-64/nodejs-18.16.1-hf52ce11_0.conda#23ed78db48ed08c94e5449f6661d65e6
-https://conda.anaconda.org/conda-forge/linux-64/python-3.11.4-hab00c5b_0_cpython.conda#1c628861a2a126b9fc9363ca1b7d014e
+https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-h166bdaf_4.tar.bz2#4b11e365c0275b808be78b30f904e295
+https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2#e5613f2bc717e9945840ff474419b8e4
+https://conda.anaconda.org/conda-forge/linux-64/nodejs-18.15.0-h4abf6b9_1.conda#2aabafd88f6876a57c45c00598715ac4
+https://conda.anaconda.org/conda-forge/linux-64/python-3.8.16-he550d4f_1_cpython.conda#9de84cccfbc5f8350a3667bb6ef6fc30
+https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.0.9-py311ha362b79_9.conda#ced5340f5dc6cff43a80deac8d0e398f
+https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_8.tar.bz2#2ff08978892a3e8b954397c461f18418
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
-https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py311hcafe171_0.conda#f4c810ad9d791c8df5ad900ed74b085b
+https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py38h8dc9893_0.conda#e3c2cc835cf3223d585d1d25d56fd3de
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
-https://conda.anaconda.org/conda-forge/linux-64/docutils-0.20.1-py311h38be061_0.conda#207175b7d514d42f977ec505800d6824
+https://conda.anaconda.org/conda-forge/linux-64/docutils-0.20.1-py38h578d9bd_0.conda#3657a5b59c232b89f21b82d27e12d636
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
-https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
-https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py311h459d7ec_0.conda#9904dc4adb5d547cb21e136f98cb24b0
-https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
-https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.2-py38h1de0b5d_0.conda#6d97b5d6f06933ab653f1862ddf6e33e
+https://conda.anaconda.org/conda-forge/noarch/mistune-2.0.5-pyhd8ed1ab_0.conda#61a07195cfc935f1c1901d8ecf4af441
+https://conda.anaconda.org/conda-forge/noarch/natsort-8.3.1-pyhd8ed1ab_0.conda#8c53149aa69bfeb045f28c92a2b2ddc7
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda#02153b6b760bbec00cfe9e4c97993d06
-https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py311h2582759_0.conda#a90f8e278c1cd7064b2713e6b7db87e6
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
+https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py38h1de0b5d_0.conda#92e899e7b0ed27c793014d1fa54f9b7b
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
-https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
+https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py38h1de0b5d_0.conda#a33157288d499397a2a56da4d724948d
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
-https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py311hd4cff14_5.tar.bz2#da8769492e423103c59f469f4f17f8d9
-https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py311h75c88c4_0.conda#db94a7a9e865fbfde8c023b6e8958bb2
+https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py38h0a891b7_5.tar.bz2#0856c59f9ddb710c640dc0428d66b1b7
+https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py38h509eb50_0.conda#33872b6650886eba869408b76c96994c
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
-https://conda.anaconda.org/conda-forge/noarch/robotframework-6.1-pyhd8ed1ab_0.conda#e383bebdc0d8fea4ecf9c9e01d0959fe
-https://conda.anaconda.org/conda-forge/linux-64/rpds-py-0.9.2-py311h46250e7_0.conda#bcf66b5abaec47198b42cdd0bb968540
+https://conda.anaconda.org/conda-forge/noarch/robotframework-5.0.1-pyhd8ed1ab_0.tar.bz2#325df82f1bdd5175bb7b16d0c96e7d5e
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh41d4057_0.conda#ada5a17adcd10be4fc7e37e4166ba0e2
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
-https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py311h459d7ec_0.conda#12b1c374ee90a1aa11ea921858394dc8
+https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py38h01eb140_0.conda#3db869202b0e523d606d13e81ca79ab6
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
-https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
-https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
-https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.3-pyhd8ed1ab_0.conda#a3d2d43b74e042567cc4b5e328534885
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.2-pyhd8ed1ab_0.conda#bfe7e7cd1476092f51efbcde15dfb110
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
+https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.2-pyhd8ed1ab_0.conda#41221f97a0c82e5a60b21716a3d7469c
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
-https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py311h409f033_3.conda#9025d0786dbbe4bc91fd8e85502decce
+https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py38h4a40e3a_3.conda#3ac112151c6b6cfe457e976de41af0c5
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
-https://conda.anaconda.org/conda-forge/linux-64/coverage-7.2.7-py311h459d7ec_0.conda#3c2c65575c28b23afc5e4ff721a2fc9f
+https://conda.anaconda.org/conda-forge/linux-64/coverage-7.2.7-py38h01eb140_0.conda#08ec729e43c468bf658e8795dbf7fb22
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.30.0-pyhd8ed1ab_0.conda#13bf095e3ecd18999d65b4d3ac5b15d5
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.2.0-pyhd8ed1ab_0.conda#c9e9064ab45ffb46f7a96834d9e7626d
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-2.2.0-pyhd8ed1ab_0.tar.bz2#29a329f0b817038d27d7bdfb2ca04b5a
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.4-pyhd8ed1ab_0.conda#18badd8fa3648d1beb1fcc7f2e0f756e
-https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py311hd4cff14_3.tar.bz2#5159e874f65ac382773d2b534a1d7b80
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.2-pyhd8ed1ab_0.conda#81a763f3c64fe6d5f32e033b0325265d
+https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py38h0a891b7_3.tar.bz2#efcaa056d265a3138d2038a4b6b68791
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.7.1-pyhd8ed1ab_0.conda#7c27ea1bdbe520bb830dcadd59f55cbf
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
-https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.2-py311h38be061_0.conda#dcbfe3a95e8b99ec743e26a75d8c9cf4
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.15.0-pyhd8ed1ab_0.conda#02e7912139fb64828d18d07c43dcbad0
+https://conda.anaconda.org/conda-forge/linux-64/trio-0.21.0-py38h578d9bd_0.tar.bz2#635bfc42b4cdcbf54112fb7d7cd0165d
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.18.4-pyhd8ed1ab_0.conda#7356151a32ebd9a20158d2f26d224bfa
-https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.1-py311h38be061_0.conda#0cf8259b01ede82c76007996f73f89ed
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
-https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
+https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.0-py38h578d9bd_0.conda#d75b783a348cf33c6d3d75480300fecd
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.2-pyhd8ed1ab_0.conda#4ec732d2264373773a5feaea477128a8
+https://conda.anaconda.org/conda-forge/linux-64/ipython-7.33.0-py38h578d9bd_0.tar.bz2#e5974f3989600330818d1bc921549bae
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
-https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh41d4057_0.conda#0a0b0d8177c4a209017b356439292db8
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh210e3f2_0.conda#4b57b688e22d094d1479a35543c18e93
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
-https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh71e2992_0.conda#cfafc9387c32a43a1b6d63633489cbc9
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda#32dde1678bb003c90d4bc0c2dbd21814
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
+https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-5.1.3-pyhd8ed1ab_0.tar.bz2#464fdfebe1a1ffb41b031d8bbfb6041f
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.4.0-pyhd8ed1ab_0.conda#4456e6030a8309bdad57569b0170b6a3
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
 https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.0-pyhd8ed1ab_0.conda#38589f4104d11f2a59ff01a9f4e3bfb3
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.22.1-pyhd8ed1ab_0.conda#fc7172a6742a7c3c4331ddd7ed463ffc
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.0.3-pyhd8ed1ab_0.conda#c861cae50ac4cbc6d573a947f67a2d0c
-https://conda.anaconda.org/conda-forge/noarch/notebook-7.0.0-pyhd8ed1ab_0.conda#a8aa205f2b275a786cf6e55bb60a2d1a
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.0.1-pyhd8ed1ab_0.conda#93cc832cb8e18caa52c7b36ea6ce7f3d
+https://conda.anaconda.org/conda-forge/label/notebook_beta/noarch/notebook-7.0.0b3-pyhb537eac_0.conda#a654d4b1443e5f3ac52d3a3dc1b19b17
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/test/linux-64/py3.8/lab3/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/linux-64/py3.8/lab3/conda.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,163 +1,164 @@
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
 https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.1.0-hfd8a6a1_0.conda#067bcc23164642f4c226da631f2a2e1d
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-12.2.0-h46fd767_19.tar.bz2#1030b1f38c129f2634eae026f704fe60
 https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.8-3_cp38.conda#2f3f7af062b42d664117662612022204
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-12.2.0-h65d4601_19.tar.bz2#cedcee7c064c01c403f962c9e8d3c373
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-12.2.0-h65d4601_19.tar.bz2#e4c94f80aef025c17ab0828cd85ef535
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
-https://conda.anaconda.org/conda-forge/linux-64/firefox-115.0-hd3aeb46_0.conda#816707575d8de0052347e2fa5a19c5f7
+https://conda.anaconda.org/conda-forge/linux-64/firefox-113.0-h59595ed_0.conda#262f91a0dfca92813a3d469cc5453f61
 https://conda.anaconda.org/conda-forge/linux-64/geckodriver-0.33.0-hd2f7af9_0.conda#83664049f2b276cc23bd67d41eb9a4ee
-https://conda.anaconda.org/conda-forge/linux-64/gmp-6.2.1-h58526e2_0.tar.bz2#b94cf2db16066b242ebd26db2facbd56
 https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2#9194c9bf9428035a05352d031462eae4
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
 https://conda.anaconda.org/conda-forge/linux-64/libuv-1.44.2-h166bdaf_0.tar.bz2#e5cb4fe581a18ca2185a016eb848fc00
-https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
-https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
+https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-h166bdaf_4.tar.bz2#f3f9de449d32ca9b9c66a22863c96f41
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h27087fc_1.tar.bz2#4acfc691e64342b9dae57cf2adc63238
 https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
 https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
 https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2#4ae4d7795d33e02bd20f6b23d91caf82
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2#04bac51ba35ea023dc48af73c1c88c25
 https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
+https://conda.anaconda.org/conda-forge/linux-64/pandoc-2.19.2-h32600fe_2.conda#326f46f36d15c44cff5f81d505cb717f
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
-https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
-https://conda.anaconda.org/conda-forge/linux-64/nodejs-18.16.1-hf52ce11_0.conda#23ed78db48ed08c94e5449f6661d65e6
-https://conda.anaconda.org/conda-forge/linux-64/pandoc-3.1.3-h32600fe_0.conda#8287aeb8462e2d4b235eff788e75919d
-https://conda.anaconda.org/conda-forge/linux-64/python-3.8.17-he550d4f_0_cpython.conda#72d038de0a228e4f0ef4011940641293
+https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-h166bdaf_4.tar.bz2#4b11e365c0275b808be78b30f904e295
+https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2#e5613f2bc717e9945840ff474419b8e4
+https://conda.anaconda.org/conda-forge/linux-64/nodejs-18.15.0-h4abf6b9_1.conda#2aabafd88f6876a57c45c00598715ac4
+https://conda.anaconda.org/conda-forge/linux-64/python-3.8.16-he550d4f_1_cpython.conda#9de84cccfbc5f8350a3667bb6ef6fc30
 https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
 https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.0.9-py38hfa26641_9.conda#d056745008e5ed73210a31dcfd4d183a
+https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_8.tar.bz2#2ff08978892a3e8b954397c461f18418
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py38h8dc9893_0.conda#e3c2cc835cf3223d585d1d25d56fd3de
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/linux-64/docutils-0.20.1-py38h578d9bd_0.conda#3657a5b59c232b89f21b82d27e12d636
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_robotmode-0.3.1-pyhd8ed1ab_0.tar.bz2#081f1505925bd5ff080864f4281c28a6
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
-https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py38h01eb140_0.conda#17d2a5314adf0f25220eeebb312d00a4
-https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
-https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.2-py38h1de0b5d_0.conda#6d97b5d6f06933ab653f1862ddf6e33e
+https://conda.anaconda.org/conda-forge/noarch/mistune-2.0.5-pyhd8ed1ab_0.conda#61a07195cfc935f1c1901d8ecf4af441
+https://conda.anaconda.org/conda-forge/noarch/natsort-8.3.1-pyhd8ed1ab_0.conda#8c53149aa69bfeb045f28c92a2b2ddc7
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda#02153b6b760bbec00cfe9e4c97993d06
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
 https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py38h1de0b5d_0.conda#92e899e7b0ed27c793014d1fa54f9b7b
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
+https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py38h1de0b5d_0.conda#a33157288d499397a2a56da4d724948d
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py38h0a891b7_5.tar.bz2#0856c59f9ddb710c640dc0428d66b1b7
 https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py38h509eb50_0.conda#33872b6650886eba869408b76c96994c
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/noarch/robotframework-5.0.1-pyhd8ed1ab_0.tar.bz2#325df82f1bdd5175bb7b16d0c96e7d5e
-https://conda.anaconda.org/conda-forge/linux-64/rpds-py-0.9.2-py38h0cc4f7c_0.conda#b735f2645ae63f01a36d8615a49acff7
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh41d4057_0.conda#ada5a17adcd10be4fc7e37e4166ba0e2
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py38h01eb140_0.conda#3db869202b0e523d606d13e81ca79ab6
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.2-pyhd8ed1ab_0.conda#bfe7e7cd1476092f51efbcde15dfb110
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
 https://conda.anaconda.org/conda-forge/linux-64/y-py-0.5.9-py38h9fda977_0.conda#18517ed6c99222252a7409b9e128015c
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
-https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.1-pyhd8ed1ab_0.conda#7b517e7a6f0790337906c055aa97ca49
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py38h4a40e3a_3.conda#3ac112151c6b6cfe457e976de41af0c5
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
 https://conda.anaconda.org/conda-forge/linux-64/coverage-7.2.7-py38h01eb140_0.conda#08ec729e43c468bf658e8795dbf7fb22
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.30.0-pyhd8ed1ab_0.conda#13bf095e3ecd18999d65b4d3ac5b15d5
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-2.2.0-pyhd8ed1ab_0.tar.bz2#29a329f0b817038d27d7bdfb2ca04b5a
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.4-pyhd8ed1ab_0.conda#18badd8fa3648d1beb1fcc7f2e0f756e
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.2-pyhd8ed1ab_0.conda#81a763f3c64fe6d5f32e033b0325265d
 https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
 https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py38h0a891b7_3.tar.bz2#efcaa056d265a3138d2038a4b6b68791
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.7.1-pyhd8ed1ab_0.conda#7c27ea1bdbe520bb830dcadd59f55cbf
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.15.0-pyhd8ed1ab_0.conda#02e7912139fb64828d18d07c43dcbad0
 https://conda.anaconda.org/conda-forge/linux-64/trio-0.21.0-py38h578d9bd_0.tar.bz2#635bfc42b4cdcbf54112fb7d7cd0165d
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.18.4-pyhd8ed1ab_0.conda#7356151a32ebd9a20158d2f26d224bfa
 https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.0-py38h578d9bd_0.conda#d75b783a348cf33c6d3d75480300fecd
+https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
-https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.2-pyhd8ed1ab_0.conda#4ec732d2264373773a5feaea477128a8
 https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/linux-64/ipython-7.33.0-py38h578d9bd_0.tar.bz2#e5974f3989600330818d1bc921549bae
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
-https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.8.0-pyhd8ed1ab_0.conda#1ca43103a08456b19222d93fd9d119ac
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh71e2992_0.conda#cfafc9387c32a43a1b6d63633489cbc9
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh210e3f2_0.conda#4b57b688e22d094d1479a35543c18e93
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
 https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-5.1.3-pyhd8ed1ab_0.tar.bz2#464fdfebe1a1ffb41b031d8bbfb6041f
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda#32dde1678bb003c90d4bc0c2dbd21814
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.1-pyhd8ed1ab_1.conda#796b056965d7146bcac082fa2a83943d
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.4.0-pyhd8ed1ab_0.conda#4456e6030a8309bdad57569b0170b6a3
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.4.0-pyhd8ed1ab_0.conda#127c702e1b1eff595be82bc6a78cfce0
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.1-pyhd8ed1ab_1.conda#95d9d1523df069792cd059f412be0d6e
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.22.1-pyhd8ed1ab_0.conda#fc7172a6742a7c3c4331ddd7ed463ffc
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.4.0-pyhd8ed1ab_0.conda#a86727968b41c20dd3d73b91632e77dc
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_ydoc-0.8.0-pyhd8ed1ab_0.conda#780280d42fbcb2eaf654a6ba7a3e5bb5
 https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
 https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.5-pyhd8ed1ab_0.conda#82299e1d33c6f130688f90880e6b3b4f
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.4-pyhd8ed1ab_0.conda#e66d4a6e36fcc92fe266932bf85fd35a
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/test/linux-64/py3.8/lab4/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/docs/rtd.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,151 +1,155 @@
-@EXPLICIT
-https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
-https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
-https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.1.0-hfd8a6a1_0.conda#067bcc23164642f4c226da631f2a2e1d
-https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.8-3_cp38.conda#2f3f7af062b42d664117662612022204
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
-https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
-https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
-https://conda.anaconda.org/conda-forge/linux-64/firefox-115.0-hd3aeb46_0.conda#816707575d8de0052347e2fa5a19c5f7
-https://conda.anaconda.org/conda-forge/linux-64/geckodriver-0.33.0-hd2f7af9_0.conda#83664049f2b276cc23bd67d41eb9a4ee
-https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
-https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
-https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
-https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
-https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
-https://conda.anaconda.org/conda-forge/linux-64/libuv-1.44.2-h166bdaf_0.tar.bz2#e5cb4fe581a18ca2185a016eb848fc00
-https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
-https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
-https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
-https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
-https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
-https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
-https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
-https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
-https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
-https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
-https://conda.anaconda.org/conda-forge/linux-64/nodejs-18.16.1-hf52ce11_0.conda#23ed78db48ed08c94e5449f6661d65e6
-https://conda.anaconda.org/conda-forge/linux-64/python-3.8.17-he550d4f_0_cpython.conda#72d038de0a228e4f0ef4011940641293
-https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
-https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
-https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
-https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.0.9-py38hfa26641_9.conda#d056745008e5ed73210a31dcfd4d183a
-https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
-https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
-https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py38h8dc9893_0.conda#e3c2cc835cf3223d585d1d25d56fd3de
-https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
-https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
-https://conda.anaconda.org/conda-forge/linux-64/docutils-0.20.1-py38h578d9bd_0.conda#3657a5b59c232b89f21b82d27e12d636
-https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
-https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
-https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
-https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py38h01eb140_0.conda#17d2a5314adf0f25220eeebb312d00a4
-https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
-https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
-https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
-https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
-https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
-https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
-https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
-https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda#02153b6b760bbec00cfe9e4c97993d06
-https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py38h1de0b5d_0.conda#92e899e7b0ed27c793014d1fa54f9b7b
-https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
-https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
-https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
-https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
-https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
-https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
-https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
-https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py38h0a891b7_5.tar.bz2#0856c59f9ddb710c640dc0428d66b1b7
-https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py38h509eb50_0.conda#33872b6650886eba869408b76c96994c
-https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
-https://conda.anaconda.org/conda-forge/noarch/robotframework-5.0.1-pyhd8ed1ab_0.tar.bz2#325df82f1bdd5175bb7b16d0c96e7d5e
-https://conda.anaconda.org/conda-forge/linux-64/rpds-py-0.9.2-py38h0cc4f7c_0.conda#b735f2645ae63f01a36d8615a49acff7
-https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh41d4057_0.conda#ada5a17adcd10be4fc7e37e4166ba0e2
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
-https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
-https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
-https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
-https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
-https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
-https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
-https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py38h01eb140_0.conda#3db869202b0e523d606d13e81ca79ab6
-https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
-https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
-https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
-https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.1-pyhd8ed1ab_0.conda#7b517e7a6f0790337906c055aa97ca49
-https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.3-pyhd8ed1ab_0.conda#a3d2d43b74e042567cc4b5e328534885
-https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
-https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
-https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
-https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py38h4a40e3a_3.conda#3ac112151c6b6cfe457e976de41af0c5
-https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
-https://conda.anaconda.org/conda-forge/linux-64/coverage-7.2.7-py38h01eb140_0.conda#08ec729e43c468bf658e8795dbf7fb22
-https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
-https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
-https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
-https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
-https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
-https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
-https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
-https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.30.0-pyhd8ed1ab_0.conda#13bf095e3ecd18999d65b4d3ac5b15d5
-https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-2.2.0-pyhd8ed1ab_0.tar.bz2#29a329f0b817038d27d7bdfb2ca04b5a
-https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
-https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
-https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.4-pyhd8ed1ab_0.conda#18badd8fa3648d1beb1fcc7f2e0f756e
-https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py38h0a891b7_3.tar.bz2#efcaa056d265a3138d2038a4b6b68791
-https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.7.1-pyhd8ed1ab_0.conda#7c27ea1bdbe520bb830dcadd59f55cbf
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
-https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
-https://conda.anaconda.org/conda-forge/linux-64/trio-0.21.0-py38h578d9bd_0.tar.bz2#635bfc42b4cdcbf54112fb7d7cd0165d
-https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
-https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
-https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
-https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
-https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.18.4-pyhd8ed1ab_0.conda#7356151a32ebd9a20158d2f26d224bfa
-https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.0-py38h578d9bd_0.conda#d75b783a348cf33c6d3d75480300fecd
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
-https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
-https://conda.anaconda.org/conda-forge/linux-64/ipython-7.33.0-py38h578d9bd_0.tar.bz2#e5974f3989600330818d1bc921549bae
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
-https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
-https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh71e2992_0.conda#cfafc9387c32a43a1b6d63633489cbc9
-https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
-https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-5.1.3-pyhd8ed1ab_0.tar.bz2#464fdfebe1a1ffb41b031d8bbfb6041f
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda#32dde1678bb003c90d4bc0c2dbd21814
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
-https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.0-pyhd8ed1ab_0.conda#38589f4104d11f2a59ff01a9f4e3bfb3
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
-https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.0.3-pyhd8ed1ab_0.conda#c861cae50ac4cbc6d573a947f67a2d0c
-https://conda.anaconda.org/conda-forge/noarch/notebook-7.0.0-pyhd8ed1ab_0.conda#a8aa205f2b275a786cf6e55bb60a2d1a
+# Probably don't edit by hand!
+#
+# This was generated from .github/locks/docs/linux-64/conda.lock
+#
+#   doit docs:rtd:env
+#
+channels:
+  - conda-forge
+  - nodefaults
+dependencies:
+  - https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
+  - https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
+  - https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
+  - https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-12.2.0-h46fd767_19.tar.bz2#1030b1f38c129f2634eae026f704fe60
+  - https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.11-3_cp311.conda#c2e2630ddb68cf52eec74dc7dfab20b5
+  - https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
+  - https://conda.anaconda.org/conda-forge/linux-64/libgomp-12.2.0-h65d4601_19.tar.bz2#cedcee7c064c01c403f962c9e8d3c373
+  - https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
+  - https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-12.2.0-h65d4601_19.tar.bz2#e4c94f80aef025c17ab0828cd85ef535
+  - https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
+  - https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
+  - https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2#9194c9bf9428035a05352d031462eae4
+  - https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
+  - https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
+  - https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
+  - https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
+  - https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
+  - https://conda.anaconda.org/conda-forge/linux-64/libuv-1.44.2-h166bdaf_0.tar.bz2#e5cb4fe581a18ca2185a016eb848fc00
+  - https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-h166bdaf_4.tar.bz2#f3f9de449d32ca9b9c66a22863c96f41
+  - https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h27087fc_1.tar.bz2#4acfc691e64342b9dae57cf2adc63238
+  - https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
+  - https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
+  - https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
+  - https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2#4ae4d7795d33e02bd20f6b23d91caf82
+  - https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2#04bac51ba35ea023dc48af73c1c88c25
+  - https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
+  - https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
+  - https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
+  - https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
+  - https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-h166bdaf_4.tar.bz2#4b11e365c0275b808be78b30f904e295
+  - https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2#e5613f2bc717e9945840ff474419b8e4
+  - https://conda.anaconda.org/conda-forge/linux-64/nodejs-18.15.0-h4abf6b9_1.conda#2aabafd88f6876a57c45c00598715ac4
+  - https://conda.anaconda.org/conda-forge/linux-64/python-3.11.3-h2755cc3_0_cpython.conda#37005ea5f68df6a8a381b70cf4d4a160
+  - https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
+  - https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
+  - https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
+  - https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
+  - https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
+  - https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_8.tar.bz2#2ff08978892a3e8b954397c461f18418
+  - https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
+  - https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
+  - https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
+  - https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
+  - https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
+  - https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py311hcafe171_0.conda#f4c810ad9d791c8df5ad900ed74b085b
+  - https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
+  - https://conda.anaconda.org/conda-forge/linux-64/docutils-0.19-py311h38be061_1.tar.bz2#599159b0740e9b82e7eef0e8471be3c2
+  - https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+  - https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
+  - https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
+  - https://conda.anaconda.org/conda-forge/linux-64/greenlet-2.0.2-py311hb755f60_1.conda#82f9885f18cc7ba9bca6687ac97f1d65
+  - https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
+  - https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
+  - https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.2-py311h2582759_0.conda#adb20bd57069614552adac60a020c36d
+  - https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
+  - https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
+  - https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
+  - https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
+  - https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
+  - https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
+  - https://conda.anaconda.org/conda-forge/noarch/port-for-0.6.3-pyhd8ed1ab_0.conda#cfc0df39511f323ad3d999203d86fe8d
+  - https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py311h2582759_0.conda#a90f8e278c1cd7064b2713e6b7db87e6
+  - https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
+  - https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
+  - https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
+  - https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py311h2582759_0.conda#e53876b66dcc4ba8a0afa63cd8502ac3
+  - https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
+  - https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
+  - https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
+  - https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py311hd4cff14_5.tar.bz2#da8769492e423103c59f469f4f17f8d9
+  - https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py311h75c88c4_0.conda#db94a7a9e865fbfde8c023b6e8958bb2
+  - https://conda.anaconda.org/conda-forge/noarch/robotframework-6.0.2-pyhd8ed1ab_1.conda#b4dcead8c5a99a14733d9b1ba5b7db09
+  - https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
+  - https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
+  - https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
+  - https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
+  - https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
+  - https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
+  - https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.4-pyhd8ed1ab_0.conda#5a31a7d564f551d0e6dff52fd8cb5b16
+  - https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
+  - https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.1-pyhd8ed1ab_0.conda#6c8c4d6eb2325e59290ac6dbbeacd5f0
+  - https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
+  - https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
+  - https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
+  - https://conda.anaconda.org/conda-forge/noarch/tabulate-0.9.0-pyhd8ed1ab_1.tar.bz2#4759805cce2d914c38472f70bf4d8bcb
+  - https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
+  - https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
+  - https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py311h459d7ec_0.conda#12b1c374ee90a1aa11ea921858394dc8
+  - https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
+  - https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
+  - https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+  - https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+  - https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
+  - https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
+  - https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
+  - https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
+  - https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
+  - https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
+  - https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
+  - https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+  - https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
+  - https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
+  - https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
+  - https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
+  - https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
+  - https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
+  - https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
+  - https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
+  - https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
+  - https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
+  - https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
+  - https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
+  - https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.2-pyhd8ed1ab_0.conda#81a763f3c64fe6d5f32e033b0325265d
+  - https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
+  - https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+  - https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
+  - https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.3.5-pyhd8ed1ab_0.conda#9eeb66a24c8f6d950eb55a9f1128da20
+  - https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
+  - https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
+  - https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-2.0.15-py311h459d7ec_0.conda#d2199e4c33e24003103845ab9b07469e
+  - https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
+  - https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.0-py311h38be061_1.tar.bz2#0564e63c41c0527f8085a572a931f1e6
+  - https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
+  - https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
+  - https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
+  - https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
+  - https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.0-py311h38be061_0.conda#1dd43a18a75d59206019e2a2a28555e5
+  - https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+  - https://conda.anaconda.org/conda-forge/noarch/sphinx-5.3.0-pyhd8ed1ab_0.tar.bz2#f9e1fcfe235d655900bfeb6aee426472
+  - https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.2-pyhd8ed1ab_0.conda#4ec732d2264373773a5feaea477128a8
+  - https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+  - https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
+  - https://conda.anaconda.org/conda-forge/noarch/nbformat-5.8.0-pyhd8ed1ab_0.conda#1ca43103a08456b19222d93fd9d119ac
+  - https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+  - https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
+  - https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
+  - https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2021.3.14-pyhd8ed1ab_0.tar.bz2#1909f784dc37b4ab97afe2c95aeeabaa
+  - https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
+  - https://conda.anaconda.org/conda-forge/noarch/ipython-8.13.2-pyh41d4057_0.conda#e8563c13eee80a5f1c7bdfc2a1b20077
+  - https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda#f7aa15f77d29b11caa1df1eb15383c59
+  - https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_0.conda#15700afca8f7ab35542e9c1af63568f1
+  - https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh210e3f2_0.conda#4b57b688e22d094d1479a35543c18e93
+  - https://conda.anaconda.org/conda-forge/noarch/jupyter-cache-0.6.1-pyhd8ed1ab_0.conda#2e360820ae68e3d28e1a5a9d2714ca5c
+  - https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda#40190b7d06f86b63d28fa78aaa39c023
+name: rtd
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/test/osx-64/py3.11/lab3/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/docs/osx-64/conda.lock`

 * *Files 8% similar despite different names*

```diff
@@ -1,164 +1,139 @@
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
 https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
-https://conda.anaconda.org/conda-forge/osx-64/icu-72.1-h7336db1_0.conda#c9689510a50a4bb2ae978421671a125e
-https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_8.tar.bz2#37157d273eaf3bc7d6862104161d9ec9
+https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.4-hd57cbcb_0.conda#195236e2eeb3b108e3b8eee47ad074fd
 https://conda.anaconda.org/conda-forge/osx-64/libexpat-2.5.0-hf0c8a7f_1.conda#6c81cb022780ee33435cca0127dd43c9
 https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
 https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2#24632c09ed931af617fe6d5292919cab
 https://conda.anaconda.org/conda-forge/osx-64/libuv-1.44.2-hac89ed1_0.tar.bz2#958fa9add5701462a6c91e3774425ea1
-https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
-https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
+https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-hfd90126_4.tar.bz2#35eb3fce8d51ed3c1fd4122bad48250b
+https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.3-h96cf925_1.tar.bz2#76217ebfbb163ff2770a261f955a5861
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.11-3_cp311.conda#5e0a069a585445333868d2c6651c3b3f
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
 https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
-https://conda.anaconda.org/conda-forge/osx-64/firefox-115.0-he965462_0.conda#89398dd53b5dacf0f0651b78a0ca01a9
-https://conda.anaconda.org/conda-forge/osx-64/geckodriver-0.33.0-hf46a32e_0.conda#897200360380560ac85cf0756161dd78
+https://conda.anaconda.org/conda-forge/osx-64/icu-70.1-h96cf925_0.tar.bz2#376635049e9b9b0bb875efd39dcd7b3b
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_8.tar.bz2#7f952a036d9014b4dab96c6ea0f8c2a7
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_8.tar.bz2#b36a3bfe866d9127f25f286506982166
 https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
 https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
-https://conda.anaconda.org/conda-forge/osx-64/pandoc-3.1.3-h9d075a6_0.conda#e86a3d5c966a09b6129354114483f7a7
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
 https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
-https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-h8a1eda9_5.conda#75a8a98b1c4671c5d2897975731da42d
-https://conda.anaconda.org/conda-forge/osx-64/nodejs-18.16.1-h46e3395_0.conda#e4c06702959edec36072a3d081af4587
-https://conda.anaconda.org/conda-forge/osx-64/python-3.11.4-h30d4d87_0_cpython.conda#e40b3075f85db0184d5f61d17c580ef7
-https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
+https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-hfd90126_4.tar.bz2#be90e6223c74ea253080abae19b3bdb1
+https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_8.tar.bz2#aac5ad0d8f747ef7f871508146df75d9
+https://conda.anaconda.org/conda-forge/osx-64/nodejs-18.15.0-hd0c9b3c_0.conda#4c7eb1947ecaa10394cf1cbcca343131
+https://conda.anaconda.org/conda-forge/osx-64/python-3.11.3-h99528f9_0_cpython.conda#c3291f9411424fc587d53a2ea57fb075
+https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
 https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
+https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.0.9-py311h814d153_9.conda#034ddcc806d421524fbc46778447e87c
+https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_8.tar.bz2#55f612fe4a9b5f6ac76348b6de94aaeb
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
+https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
+https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.7-py311h814d153_0.conda#c27802860b87fe024c9b6276205a56b5
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
-https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
-https://conda.anaconda.org/conda-forge/osx-64/docutils-0.20.1-py311h6eed73b_0.conda#0536cbe889e20101b7f8e6d6b1dbcbf4
-https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
+https://conda.anaconda.org/conda-forge/osx-64/docutils-0.19-py311h6eed73b_1.tar.bz2#268664c5447607a94cd67a0be91f83cd
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
+https://conda.anaconda.org/conda-forge/osx-64/greenlet-2.0.2-py311hdf8f085_1.conda#58ebad2ba8dc2225237ebd7d7c3111d2
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
-https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_robotmode-0.3.1-pyhd8ed1ab_0.tar.bz2#081f1505925bd5ff080864f4281c28a6
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
-https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.3-py311h2725bcf_0.conda#65b70928fcc2a81891ad1a8a6a7b085a
-https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
-https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
+https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
+https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.2-py311h5547dcb_0.conda#13091519d55d667506aaf413cffaff10
+https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
-https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda#02153b6b760bbec00cfe9e4c97993d06
+https://conda.anaconda.org/conda-forge/noarch/port-for-0.6.3-pyhd8ed1ab_0.conda#cfc0df39511f323ad3d999203d86fe8d
 https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.5-py311h5547dcb_0.conda#d9b4565309f4f992b42bd99031044642
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
-https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
+https://conda.anaconda.org/conda-forge/osx-64/pyrsistent-0.19.3-py311h5547dcb_0.conda#f114c0dab9f9c894b260297371124634
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
-https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py311h5547dcb_5.tar.bz2#8d1e456914ce961119b07f396187a564
 https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.0-py311h5dacc12_0.conda#1f65b37886e7cb8476d48ea8bb9d19c0
-https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
-https://conda.anaconda.org/conda-forge/noarch/robotframework-6.1-pyhd8ed1ab_0.conda#e383bebdc0d8fea4ecf9c9e01d0959fe
-https://conda.anaconda.org/conda-forge/osx-64/rpds-py-0.9.2-py311h299eb51_0.conda#bda1d1d8fce204234ed183b150dd51cc
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/noarch/robotframework-6.0.2-pyhd8ed1ab_1.conda#b4dcead8c5a99a14733d9b1ba5b7db09
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
+https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
+https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.4-pyhd8ed1ab_0.conda#5a31a7d564f551d0e6dff52fd8cb5b16
+https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
+https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.1-pyhd8ed1ab_0.conda#6c8c4d6eb2325e59290ac6dbbeacd5f0
+https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
+https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
+https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
+https://conda.anaconda.org/conda-forge/noarch/tabulate-0.9.0-pyhd8ed1ab_1.tar.bz2#4759805cce2d914c38472f70bf4d8bcb
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py311h2725bcf_0.conda#276fe4341e39dcd9d9d33ca18140d2e7
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
-https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
-https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
-https://conda.anaconda.org/conda-forge/osx-64/y-py-0.5.9-py311h890d03e_0.conda#d333683779e7145d5fe8bb18e08a7623
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
-https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
-https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
-https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py311ha86e640_3.conda#5967be4da33261eada7cc79593f71088
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
-https://conda.anaconda.org/conda-forge/osx-64/coverage-7.2.7-py311h2725bcf_0.conda#afba3a3f74c5f71ebd9f400871e8c4de
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
+https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
+https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
-https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
-https://conda.anaconda.org/conda-forge/osx-64/pyobjc-core-9.2-py311hf110eff_0.conda#460e6d2c254ec4aa4299cd9bffa3b7f8
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.30.0-pyhd8ed1ab_0.conda#13bf095e3ecd18999d65b4d3ac5b15d5
-https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.2.0-pyhd8ed1ab_0.conda#c9e9064ab45ffb46f7a96834d9e7626d
-https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
-https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyhd1c38e8_0.conda#046120b71d8896cb7faef78bfdbfee1e
-https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.4-pyhd8ed1ab_0.conda#18badd8fa3648d1beb1fcc7f2e0f756e
-https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
-https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py311h5547dcb_3.tar.bz2#c09459e349fa61afc352f473766de109
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.2-pyhd8ed1ab_0.conda#81a763f3c64fe6d5f32e033b0325265d
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.7.1-pyhd8ed1ab_0.conda#7c27ea1bdbe520bb830dcadd59f55cbf
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
-https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-9.2-py311hf110eff_0.conda#6ba4637fa1ed0a1e829b1f278c12274a
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
+https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.3.5-pyhd8ed1ab_0.conda#9eeb66a24c8f6d950eb55a9f1128da20
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
+https://conda.anaconda.org/conda-forge/osx-64/sqlalchemy-2.0.15-py311h2725bcf_0.conda#0a917fc9f67ca0f9fbcaa917cf8caf98
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/osx-64/trio-0.22.2-py311h6eed73b_0.conda#6ceb2138c6038d75a92b06d3f8fd9ece
+https://conda.anaconda.org/conda-forge/osx-64/trio-0.22.0-py311h6eed73b_1.tar.bz2#71a739c4b0b1e17cfd27cfdf828d52a8
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
-https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.18.4-pyhd8ed1ab_0.conda#7356151a32ebd9a20158d2f26d224bfa
-https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.1-py311h6eed73b_0.conda#2d45628b123595054093ff65996b98ae
-https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
-https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyhd1c38e8_0.conda#2657c3de5371c571aef6678afb4aaadd
-https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
-https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
-https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
+https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.0-py311h6eed73b_0.conda#e0e5cfb36ece6eae9c355eed1e90ff9d
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/sphinx-5.3.0-pyhd8ed1ab_0.tar.bz2#f9e1fcfe235d655900bfeb6aee426472
+https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.2-pyhd8ed1ab_0.conda#4ec732d2264373773a5feaea477128a8
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.8.0-pyhd8ed1ab_0.conda#1ca43103a08456b19222d93fd9d119ac
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
-https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyhd1c38e8_0.conda#f56fab4cea853c2248105b6cd7d79bf0
-https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
-https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh5fb750a_0.conda#2a8ffa559d393fea47237b9d23ddf74f
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda#32dde1678bb003c90d4bc0c2dbd21814
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.1-pyhd8ed1ab_1.conda#796b056965d7146bcac082fa2a83943d
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.1-pyhd8ed1ab_1.conda#95d9d1523df069792cd059f412be0d6e
-https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server_ydoc-0.8.0-pyhd8ed1ab_0.conda#780280d42fbcb2eaf654a6ba7a3e5bb5
-https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
-https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.5-pyhd8ed1ab_0.conda#82299e1d33c6f130688f90880e6b3b4f
+https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2021.3.14-pyhd8ed1ab_0.tar.bz2#1909f784dc37b4ab97afe2c95aeeabaa
+https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
+https://conda.anaconda.org/conda-forge/noarch/ipython-8.13.2-pyhd1c38e8_0.conda#30960117dd6bd242aec8428a1004b167
+https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda#f7aa15f77d29b11caa1df1eb15383c59
+https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_0.conda#15700afca8f7ab35542e9c1af63568f1
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh736e0ef_0.conda#d5aa7d2cc9fe03f62cf6e7bcc8e1a8df
+https://conda.anaconda.org/conda-forge/noarch/jupyter-cache-0.6.1-pyhd8ed1ab_0.conda#2e360820ae68e3d28e1a5a9d2714ca5c
+https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda#40190b7d06f86b63d28fa78aaa39c023
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/test/osx-64/py3.11/lab4/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/win-64/py3.11/lab4/conda.lock`

 * *Files 8% similar despite different names*

```diff
@@ -1,153 +1,154 @@
 @EXPLICIT
-https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
-https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
-https://conda.anaconda.org/conda-forge/osx-64/icu-72.1-h7336db1_0.conda#c9689510a50a4bb2ae978421671a125e
-https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
-https://conda.anaconda.org/conda-forge/osx-64/libexpat-2.5.0-hf0c8a7f_1.conda#6c81cb022780ee33435cca0127dd43c9
-https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
-https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2#24632c09ed931af617fe6d5292919cab
-https://conda.anaconda.org/conda-forge/osx-64/libuv-1.44.2-hac89ed1_0.tar.bz2#958fa9add5701462a6c91e3774425ea1
-https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
-https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
-https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.11-3_cp311.conda#5e0a069a585445333868d2c6651c3b3f
+https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2023.5.7-h56e8100_0.conda#604212634bd8c4d6f20d44b946e8eedb
+https://conda.anaconda.org/conda-forge/win-64/libexpat-2.5.0-h63175ca_1.conda#636cc3cbbd2e28bcfd2f73b2044aac2c
+https://conda.anaconda.org/conda-forge/win-64/nodejs-18.15.0-h57928b3_1.conda#d728bbdc9a650a5d503d657ce12c01ce
+https://conda.anaconda.org/conda-forge/win-64/python_abi-3.11-3_cp311.conda#fd1634ba85cfea9376e1fc02d6f592e9
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
-https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
-https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
-https://conda.anaconda.org/conda-forge/osx-64/firefox-115.0-he965462_0.conda#89398dd53b5dacf0f0651b78a0ca01a9
-https://conda.anaconda.org/conda-forge/osx-64/geckodriver-0.33.0-hf46a32e_0.conda#897200360380560ac85cf0756161dd78
-https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
-https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
-https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
-https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
-https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
-https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-h8a1eda9_5.conda#75a8a98b1c4671c5d2897975731da42d
-https://conda.anaconda.org/conda-forge/osx-64/nodejs-18.16.1-h46e3395_0.conda#e4c06702959edec36072a3d081af4587
-https://conda.anaconda.org/conda-forge/osx-64/python-3.11.4-h30d4d87_0_cpython.conda#e40b3075f85db0184d5f61d17c580ef7
-https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
+https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
+https://conda.anaconda.org/conda-forge/win-64/winpty-0.4.3-4.tar.bz2#1cee351bf20b830d991dbe0bc8cd7dfe
+https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.34.31931-h5081d32_16.conda#22125178654c6a8a393f9743d585704b
+https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hb25d44b_16.conda#ea326b37e3bd6d2616988e09f3a9396c
+https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.34.31931-hed1258a_16.conda#0374eae69b6dbfb27c3dc27167109eb4
+https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
+https://conda.anaconda.org/conda-forge/win-64/firefox-113.0-h63175ca_0.conda#a2bd8315d1c49f718d4ffe0b7cf39e00
+https://conda.anaconda.org/conda-forge/win-64/geckodriver-0.33.0-h611cf2b_0.conda#e5ad5ec7f6140c1fdf9bd2a7927a4f91
+https://conda.anaconda.org/conda-forge/win-64/libbrotlicommon-1.0.9-hcfcfb64_8.tar.bz2#e8078e37208cd7d3e1eb5053f370ded8
+https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
+https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2#5c1fb45b5e2912c19098750ae8a32604
+https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.42.0-hcfcfb64_0.conda#9a71d93deb99cc09d8939d5235b5909a
+https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_4.tar.bz2#0cc5c5cc64ee1637f37f8540a175854c
+https://conda.anaconda.org/conda-forge/win-64/openssl-3.1.1-hcfcfb64_1.conda#1d913a5de46c6b2f7e4cfbd26b106b8b
+https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2#c69a5047cc9291ae40afd4a1ad6f0c0f
+https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
+https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
+https://conda.anaconda.org/conda-forge/win-64/libbrotlidec-1.0.9-hcfcfb64_8.tar.bz2#99839d9d81f33afa173c0fa82a702038
+https://conda.anaconda.org/conda-forge/win-64/libbrotlienc-1.0.9-hcfcfb64_8.tar.bz2#88e62627120c20289bf8982b15e0a6a1
+https://conda.anaconda.org/conda-forge/win-64/python-3.11.3-h2628c8c_0_cpython.conda#8f82e0e0ba51bed311f28eb6450393f6
+https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.4-h0e60522_1.tar.bz2#e1aff0583dda5fb917eb3d2c1025aa80
+https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.0.9-py311h814d153_9.conda#034ddcc806d421524fbc46778447e87c
+https://conda.anaconda.org/conda-forge/win-64/brotli-bin-1.0.9-hcfcfb64_8.tar.bz2#e18b70ed349d96086fd60a9c642b1b58
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
-https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.7-py311h814d153_0.conda#c27802860b87fe024c9b6276205a56b5
+https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
+https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.7-py311h12c1d0e_0.conda#b056c7299be929b711016d2f4e48d303
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
-https://conda.anaconda.org/conda-forge/osx-64/docutils-0.20.1-py311h6eed73b_0.conda#0536cbe889e20101b7f8e6d6b1dbcbf4
+https://conda.anaconda.org/conda-forge/win-64/docutils-0.20.1-py311h1ea47a8_0.conda#851f4c302cc7f5a617cc03a3c2090634
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
-https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.3-py311h2725bcf_0.conda#65b70928fcc2a81891ad1a8a6a7b085a
-https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
-https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.2-py311ha68e1ae_0.conda#96e7ffe6ea438ba4517152abe3b39874
+https://conda.anaconda.org/conda-forge/noarch/mistune-2.0.5-pyhd8ed1ab_0.conda#61a07195cfc935f1c1901d8ecf4af441
+https://conda.anaconda.org/conda-forge/noarch/natsort-8.3.1-pyhd8ed1ab_0.conda#8c53149aa69bfeb045f28c92a2b2ddc7
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda#02153b6b760bbec00cfe9e4c97993d06
-https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.5-py311h5547dcb_0.conda#d9b4565309f4f992b42bd99031044642
-https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
+https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.5-py311ha68e1ae_0.conda#f1a1eecd1bb4f431df5b9b6d8a152efd
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
-https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
+https://conda.anaconda.org/conda-forge/win-64/pyrsistent-0.19.3-py311ha68e1ae_0.conda#3f2780a49f0b4bb2c622f7cf098e3d06
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
-https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py311h5547dcb_5.tar.bz2#8d1e456914ce961119b07f396187a564
-https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.0-py311h5dacc12_0.conda#1f65b37886e7cb8476d48ea8bb9d19c0
+https://conda.anaconda.org/conda-forge/win-64/pywin32-304-py311h12c1d0e_2.tar.bz2#20a2d8e73b0be8e27ca4096d4f3a7053
+https://conda.anaconda.org/conda-forge/win-64/pywinpty-2.0.10-py311h12c1d0e_0.conda#4d7e034dc93f50757cf039a2e3183343
+https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py311ha68e1ae_5.tar.bz2#0c97d59d54eb52e170224b3de6ade906
+https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.0-py311h7b3f143_0.conda#b690f6e1878ccc98e96a33658867e8e1
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
-https://conda.anaconda.org/conda-forge/noarch/robotframework-6.1-pyhd8ed1ab_0.conda#e383bebdc0d8fea4ecf9c9e01d0959fe
-https://conda.anaconda.org/conda-forge/osx-64/rpds-py-0.9.2-py311h299eb51_0.conda#bda1d1d8fce204234ed183b150dd51cc
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/noarch/robotframework-6.0.2-pyhd8ed1ab_1.conda#b4dcead8c5a99a14733d9b1ba5b7db09
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
-https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py311h2725bcf_0.conda#276fe4341e39dcd9d9d33ca18140d2e7
+https://conda.anaconda.org/conda-forge/win-64/tornado-6.3.2-py311ha68e1ae_0.conda#e2a6c106c1cff7e884d93351cdee3c3e
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.2-pyhd8ed1ab_0.conda#bfe7e7cd1476092f51efbcde15dfb110
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
-https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.3-pyhd8ed1ab_0.conda#a3d2d43b74e042567cc4b5e328534885
+https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.2-pyhd8ed1ab_0.conda#41221f97a0c82e5a60b21716a3d7469c
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
-https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py311ha86e640_3.conda#5967be4da33261eada7cc79593f71088
+https://conda.anaconda.org/conda-forge/win-64/brotli-1.0.9-hcfcfb64_8.tar.bz2#2e661f21e1741c11506bdc7226e6b0bc
+https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py311h7d9ee11_3.conda#a8524727eb956b4741e25a64af79edb8
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
-https://conda.anaconda.org/conda-forge/osx-64/coverage-7.2.7-py311h2725bcf_0.conda#afba3a3f74c5f71ebd9f400871e8c4de
+https://conda.anaconda.org/conda-forge/win-64/coverage-7.2.7-py311ha68e1ae_0.conda#b3a60b6bb264fe70896de40fa392edf6
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
-https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
-https://conda.anaconda.org/conda-forge/osx-64/pyobjc-core-9.2-py311hf110eff_0.conda#460e6d2c254ec4aa4299cd9bffa3b7f8
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.30.0-pyhd8ed1ab_0.conda#13bf095e3ecd18999d65b4d3ac5b15d5
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.2.0-pyhd8ed1ab_0.conda#c9e9064ab45ffb46f7a96834d9e7626d
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
-https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyhd1c38e8_0.conda#046120b71d8896cb7faef78bfdbfee1e
+https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh08f2357_0.conda#c00d32dfa733d381b6a1908d0d67e0d7
+https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.0-pyh08f2357_0.tar.bz2#0152a609d5748ed9887d195b1e61a6c9
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.4-pyhd8ed1ab_0.conda#18badd8fa3648d1beb1fcc7f2e0f756e
-https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py311h5547dcb_3.tar.bz2#c09459e349fa61afc352f473766de109
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
+https://conda.anaconda.org/conda-forge/win-64/argon2-cffi-bindings-21.2.0-py311ha68e1ae_3.tar.bz2#c321cd825b72a2073dfb3f92ce1507fb
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.7.1-pyhd8ed1ab_0.conda#7c27ea1bdbe520bb830dcadd59f55cbf
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
-https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-9.2-py311hf110eff_0.conda#6ba4637fa1ed0a1e829b1f278c12274a
-https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.15.0-pyhd8ed1ab_0.conda#02e7912139fb64828d18d07c43dcbad0
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/osx-64/trio-0.22.2-py311h6eed73b_0.conda#6ceb2138c6038d75a92b06d3f8fd9ece
+https://conda.anaconda.org/conda-forge/win-64/trio-0.22.0-py311h1ea47a8_1.tar.bz2#1475d3775d4e2cc09c366720de842992
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.2-pyhd8ed1ab_0.conda#81a763f3c64fe6d5f32e033b0325265d
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
-https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.18.4-pyhd8ed1ab_0.conda#7356151a32ebd9a20158d2f26d224bfa
-https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.1-py311h6eed73b_0.conda#2d45628b123595054093ff65996b98ae
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
-https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyhd1c38e8_0.conda#2657c3de5371c571aef6678afb4aaadd
-https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
+https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.3.0-py311h1ea47a8_0.conda#2b81965b74e70b89053845d1bc287561
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
+https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.2-pyhd8ed1ab_0.conda#4ec732d2264373773a5feaea477128a8
+https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
-https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyhd1c38e8_0.conda#f56fab4cea853c2248105b6cd7d79bf0
+https://conda.anaconda.org/conda-forge/noarch/ipython-8.13.2-pyh08f2357_0.conda#aebd5e79c0f354cdbceb055cdec53659
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
-https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh5fb750a_0.conda#2a8ffa559d393fea47237b9d23ddf74f
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda#32dde1678bb003c90d4bc0c2dbd21814
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
+https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_0.conda#15700afca8f7ab35542e9c1af63568f1
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh025b116_0.conda#d18e38ce1f195efa2d76f9dc33832bf5
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.4.0-pyhd8ed1ab_0.conda#4456e6030a8309bdad57569b0170b6a3
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
 https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.0-pyhd8ed1ab_0.conda#38589f4104d11f2a59ff01a9f4e3bfb3
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.22.1-pyhd8ed1ab_0.conda#fc7172a6742a7c3c4331ddd7ed463ffc
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.0.3-pyhd8ed1ab_0.conda#c861cae50ac4cbc6d573a947f67a2d0c
-https://conda.anaconda.org/conda-forge/noarch/notebook-7.0.0-pyhd8ed1ab_0.conda#a8aa205f2b275a786cf6e55bb60a2d1a
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.0.1-pyhd8ed1ab_0.conda#93cc832cb8e18caa52c7b36ea6ce7f3d
+https://conda.anaconda.org/conda-forge/label/notebook_beta/noarch/notebook-7.0.0b3-pyhb537eac_0.conda#a654d4b1443e5f3ac52d3a3dc1b19b17
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/test/osx-64/py3.8/lab3/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/win-64/py3.8/lab3/conda.lock`

 * *Files 7% similar despite different names*

```diff
@@ -1,158 +1,158 @@
 @EXPLICIT
-https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
-https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
-https://conda.anaconda.org/conda-forge/osx-64/icu-72.1-h7336db1_0.conda#c9689510a50a4bb2ae978421671a125e
-https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
-https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
-https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2#24632c09ed931af617fe6d5292919cab
-https://conda.anaconda.org/conda-forge/osx-64/libuv-1.44.2-hac89ed1_0.tar.bz2#958fa9add5701462a6c91e3774425ea1
-https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
-https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
-https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.8-3_cp38.conda#ff192f59f7fe23555612030493a079f8
-https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
-https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
-https://conda.anaconda.org/conda-forge/osx-64/firefox-115.0-he965462_0.conda#89398dd53b5dacf0f0651b78a0ca01a9
-https://conda.anaconda.org/conda-forge/osx-64/geckodriver-0.33.0-hf46a32e_0.conda#897200360380560ac85cf0756161dd78
-https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
-https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
-https://conda.anaconda.org/conda-forge/osx-64/pandoc-3.1.3-h9d075a6_0.conda#e86a3d5c966a09b6129354114483f7a7
-https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
-https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
-https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
-https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-h8a1eda9_5.conda#75a8a98b1c4671c5d2897975731da42d
-https://conda.anaconda.org/conda-forge/osx-64/nodejs-18.16.1-h46e3395_0.conda#e4c06702959edec36072a3d081af4587
-https://conda.anaconda.org/conda-forge/osx-64/python-3.8.17-hf9b03c3_0_cpython.conda#f613b663d3829f325b4ffb626bf612b6
+https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2023.5.7-h56e8100_0.conda#604212634bd8c4d6f20d44b946e8eedb
+https://conda.anaconda.org/conda-forge/win-64/nodejs-18.15.0-h57928b3_1.conda#d728bbdc9a650a5d503d657ce12c01ce
+https://conda.anaconda.org/conda-forge/win-64/pandoc-2.19.2-h57928b3_2.conda#c188f67e94153ddc7e4e10ae127cbb1a
+https://conda.anaconda.org/conda-forge/win-64/python_abi-3.8-3_cp38.conda#c6df946723dadd4a5830a8ff8c6b9a20
+https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
+https://conda.anaconda.org/conda-forge/win-64/winpty-0.4.3-4.tar.bz2#1cee351bf20b830d991dbe0bc8cd7dfe
+https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.34.31931-h5081d32_16.conda#22125178654c6a8a393f9743d585704b
+https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hb25d44b_16.conda#ea326b37e3bd6d2616988e09f3a9396c
+https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.34.31931-hed1258a_16.conda#0374eae69b6dbfb27c3dc27167109eb4
+https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
+https://conda.anaconda.org/conda-forge/win-64/firefox-113.0-h63175ca_0.conda#a2bd8315d1c49f718d4ffe0b7cf39e00
+https://conda.anaconda.org/conda-forge/win-64/geckodriver-0.33.0-h611cf2b_0.conda#e5ad5ec7f6140c1fdf9bd2a7927a4f91
+https://conda.anaconda.org/conda-forge/win-64/libbrotlicommon-1.0.9-hcfcfb64_8.tar.bz2#e8078e37208cd7d3e1eb5053f370ded8
+https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
+https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2#5c1fb45b5e2912c19098750ae8a32604
+https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.42.0-hcfcfb64_0.conda#9a71d93deb99cc09d8939d5235b5909a
+https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_4.tar.bz2#0cc5c5cc64ee1637f37f8540a175854c
+https://conda.anaconda.org/conda-forge/win-64/openssl-3.1.1-hcfcfb64_1.conda#1d913a5de46c6b2f7e4cfbd26b106b8b
+https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2#c69a5047cc9291ae40afd4a1ad6f0c0f
+https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
+https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
+https://conda.anaconda.org/conda-forge/win-64/libbrotlidec-1.0.9-hcfcfb64_8.tar.bz2#99839d9d81f33afa173c0fa82a702038
+https://conda.anaconda.org/conda-forge/win-64/libbrotlienc-1.0.9-hcfcfb64_8.tar.bz2#88e62627120c20289bf8982b15e0a6a1
+https://conda.anaconda.org/conda-forge/win-64/python-3.8.16-h4de0772_1_cpython.conda#461d9fc92cfde68f2ca7ef0988f6326a
+https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.4-h0e60522_1.tar.bz2#e1aff0583dda5fb917eb3d2c1025aa80
 https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
-https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
 https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.0.9-py38h4cd09af_9.conda#f958e25488ff7e044031bca8a6c5267b
+https://conda.anaconda.org/conda-forge/win-64/brotli-bin-1.0.9-hcfcfb64_8.tar.bz2#e18b70ed349d96086fd60a9c642b1b58
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
-https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.7-py38h4cd09af_0.conda#32626ffd5cd7eaad3036d7dca808ddc7
+https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
+https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.7-py38hd3f51b4_0.conda#de2533e0a4ad84a4e5c5d6ad196f8e14
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
-https://conda.anaconda.org/conda-forge/osx-64/docutils-0.20.1-py38h50d1736_0.conda#5722ca19ba9d5601032fd4dd5262b12a
+https://conda.anaconda.org/conda-forge/win-64/docutils-0.20.1-py38haa244fe_0.conda#8f4292bb1a13ed095a725c137843da5f
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_robotmode-0.3.1-pyhd8ed1ab_0.tar.bz2#081f1505925bd5ff080864f4281c28a6
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
-https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.3-py38hcafd530_0.conda#e8ee9933dc3749c889baccb1c4b4f014
-https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
-https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.2-py38h91455d4_0.conda#962b32c8c11df005d9e225ecde549e57
+https://conda.anaconda.org/conda-forge/noarch/mistune-2.0.5-pyhd8ed1ab_0.conda#61a07195cfc935f1c1901d8ecf4af441
+https://conda.anaconda.org/conda-forge/noarch/natsort-8.3.1-pyhd8ed1ab_0.conda#8c53149aa69bfeb045f28c92a2b2ddc7
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda#02153b6b760bbec00cfe9e4c97993d06
-https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.5-py38hef030d1_0.conda#20b4cc7adae881327b943c883be6335e
-https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
+https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.5-py38h91455d4_0.conda#091a6bc808bfd07c97be1eb316440070
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
-https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
+https://conda.anaconda.org/conda-forge/win-64/pyrsistent-0.19.3-py38h91455d4_0.conda#fb4aa6d774c3a286a8561af24ff87185
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
-https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py38hef030d1_5.tar.bz2#e27d698dc29c6d5b49f1385bcd1d50f9
-https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.0-py38h3b70857_0.conda#a48761bc98b3bc22d209e9bb2f3dc5c1
+https://conda.anaconda.org/conda-forge/win-64/pywin32-304-py38hd3f51b4_2.tar.bz2#cfefffaad808b61f2932f64c079417b8
+https://conda.anaconda.org/conda-forge/win-64/pywinpty-2.0.10-py38hd3f51b4_0.conda#cc93c5fe55b8a7bdd719ce74bfbe819c
+https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py38h91455d4_5.tar.bz2#f62ab7e18711e3cbc068319448ecf771
+https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.0-py38ha85f68a_0.conda#5e97b9e91fc8cb7ec32647d5bec74030
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/noarch/robotframework-5.0.1-pyhd8ed1ab_0.tar.bz2#325df82f1bdd5175bb7b16d0c96e7d5e
-https://conda.anaconda.org/conda-forge/osx-64/rpds-py-0.9.2-py38h7510fb3_0.conda#bbd51a20bd2a5ad644516f860b9570aa
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
-https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py38hcafd530_0.conda#afefcf665a5049b030efb084a51e3935
+https://conda.anaconda.org/conda-forge/win-64/tornado-6.3.2-py38h91455d4_0.conda#3e625e06e8892112acb47695eaf22b47
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
-https://conda.anaconda.org/conda-forge/osx-64/y-py-0.5.9-py38he94b92c_0.conda#433e9f376d8b2295c16dcc9e97e0fea3
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
-https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.1-pyhd8ed1ab_0.conda#7b517e7a6f0790337906c055aa97ca49
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.2-pyhd8ed1ab_0.conda#bfe7e7cd1476092f51efbcde15dfb110
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
+https://conda.anaconda.org/conda-forge/win-64/y-py-0.5.9-py38h4900a04_0.conda#4ba79cbf620ff0cd934fee88bb9c7713
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
-https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py38hb368cf1_3.conda#a2b3ae2a1fd2aea0b4433d9e7fff8cf3
+https://conda.anaconda.org/conda-forge/win-64/brotli-1.0.9-hcfcfb64_8.tar.bz2#2e661f21e1741c11506bdc7226e6b0bc
+https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py38h57701bc_3.conda#9b94af390cfdf924a063302a2ddb3860
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
-https://conda.anaconda.org/conda-forge/osx-64/coverage-7.2.7-py38hcafd530_0.conda#868ae7c3c94b2fffbe28687a64646f53
+https://conda.anaconda.org/conda-forge/win-64/coverage-7.2.7-py38h91455d4_0.conda#2fa3faef0a7b6a5da2bff0faddbfbc68
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
-https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
-https://conda.anaconda.org/conda-forge/osx-64/pyobjc-core-9.2-py38h095c2e5_0.conda#8dbb4798b2066b678d8da47734d1c763
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.30.0-pyhd8ed1ab_0.conda#13bf095e3ecd18999d65b4d3ac5b15d5
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-2.2.0-pyhd8ed1ab_0.tar.bz2#29a329f0b817038d27d7bdfb2ca04b5a
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
-https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyhd1c38e8_0.conda#046120b71d8896cb7faef78bfdbfee1e
+https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh08f2357_0.conda#c00d32dfa733d381b6a1908d0d67e0d7
+https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.0-pyh08f2357_0.tar.bz2#0152a609d5748ed9887d195b1e61a6c9
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.4-pyhd8ed1ab_0.conda#18badd8fa3648d1beb1fcc7f2e0f756e
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
 https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
-https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py38hef030d1_3.tar.bz2#fc1bc20add8eff07c367973bba25e8eb
+https://conda.anaconda.org/conda-forge/win-64/argon2-cffi-bindings-21.2.0-py38h91455d4_3.tar.bz2#a262d1c7aaf5a93a02b33dd985c27831
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.7.1-pyhd8ed1ab_0.conda#7c27ea1bdbe520bb830dcadd59f55cbf
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
-https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-9.2-py38h095c2e5_0.conda#fa3e3307ff143e7a9e823ce7bbc916ad
-https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
-https://conda.anaconda.org/conda-forge/osx-64/trio-0.21.0-py38h50d1736_0.tar.bz2#1e91102a7512cb5094ebe9818a361376
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.15.0-pyhd8ed1ab_0.conda#02e7912139fb64828d18d07c43dcbad0
+https://conda.anaconda.org/conda-forge/win-64/trio-0.21.0-py38haa244fe_0.tar.bz2#0fe81ab845eea9441bc9a025d47577be
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.2-pyhd8ed1ab_0.conda#81a763f3c64fe6d5f32e033b0325265d
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
-https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.18.4-pyhd8ed1ab_0.conda#7356151a32ebd9a20158d2f26d224bfa
-https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.1-py38h50d1736_0.conda#03a3619e222793567b29b5966c2a821d
+https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.3.0-py38haa244fe_0.conda#ff05e328ef5915b4a8176844f5effddd
+https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
-https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyhd1c38e8_0.conda#2657c3de5371c571aef6678afb4aaadd
-https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
+https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.2-pyhd8ed1ab_0.conda#4ec732d2264373773a5feaea477128a8
 https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
-https://conda.anaconda.org/conda-forge/osx-64/ipython-7.33.0-py38h50d1736_0.tar.bz2#3bba83a6f445cccddfa5076ddbdd9467
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
-https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
+https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
+https://conda.anaconda.org/conda-forge/win-64/ipython-7.33.0-py38haa244fe_0.tar.bz2#1185ff9399904ccd14f2eadbbca1aeab
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.8.0-pyhd8ed1ab_0.conda#1ca43103a08456b19222d93fd9d119ac
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh5fb750a_0.conda#2a8ffa559d393fea47237b9d23ddf74f
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh025b116_0.conda#d18e38ce1f195efa2d76f9dc33832bf5
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
 https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-5.1.3-pyhd8ed1ab_0.tar.bz2#464fdfebe1a1ffb41b031d8bbfb6041f
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda#32dde1678bb003c90d4bc0c2dbd21814
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.1-pyhd8ed1ab_1.conda#796b056965d7146bcac082fa2a83943d
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.4.0-pyhd8ed1ab_0.conda#4456e6030a8309bdad57569b0170b6a3
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.4.0-pyhd8ed1ab_0.conda#127c702e1b1eff595be82bc6a78cfce0
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.1-pyhd8ed1ab_1.conda#95d9d1523df069792cd059f412be0d6e
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.22.1-pyhd8ed1ab_0.conda#fc7172a6742a7c3c4331ddd7ed463ffc
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.4.0-pyhd8ed1ab_0.conda#a86727968b41c20dd3d73b91632e77dc
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_ydoc-0.8.0-pyhd8ed1ab_0.conda#780280d42fbcb2eaf654a6ba7a3e5bb5
 https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
 https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.5-pyhd8ed1ab_0.conda#82299e1d33c6f130688f90880e6b3b4f
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.4-pyhd8ed1ab_0.conda#e66d4a6e36fcc92fe266932bf85fd35a
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/test/osx-64/py3.8/lab4/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/osx-64/py3.8/lab3/conda.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,147 +1,160 @@
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
 https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
-https://conda.anaconda.org/conda-forge/osx-64/icu-72.1-h7336db1_0.conda#c9689510a50a4bb2ae978421671a125e
-https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_8.tar.bz2#37157d273eaf3bc7d6862104161d9ec9
+https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.4-hd57cbcb_0.conda#195236e2eeb3b108e3b8eee47ad074fd
 https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
 https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2#24632c09ed931af617fe6d5292919cab
 https://conda.anaconda.org/conda-forge/osx-64/libuv-1.44.2-hac89ed1_0.tar.bz2#958fa9add5701462a6c91e3774425ea1
-https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
-https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
+https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-hfd90126_4.tar.bz2#35eb3fce8d51ed3c1fd4122bad48250b
+https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.3-h96cf925_1.tar.bz2#76217ebfbb163ff2770a261f955a5861
+https://conda.anaconda.org/conda-forge/osx-64/pandoc-2.19.2-h694c41f_2.conda#de3014568ff5004048dd09ba73990430
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.8-3_cp38.conda#ff192f59f7fe23555612030493a079f8
 https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
-https://conda.anaconda.org/conda-forge/osx-64/firefox-115.0-he965462_0.conda#89398dd53b5dacf0f0651b78a0ca01a9
+https://conda.anaconda.org/conda-forge/osx-64/firefox-113.0-he965462_0.conda#6730ed9d9f8ff58391adf5fe00c984c4
 https://conda.anaconda.org/conda-forge/osx-64/geckodriver-0.33.0-hf46a32e_0.conda#897200360380560ac85cf0756161dd78
+https://conda.anaconda.org/conda-forge/osx-64/icu-70.1-h96cf925_0.tar.bz2#376635049e9b9b0bb875efd39dcd7b3b
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_8.tar.bz2#7f952a036d9014b4dab96c6ea0f8c2a7
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_8.tar.bz2#b36a3bfe866d9127f25f286506982166
 https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
 https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
 https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
-https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-h8a1eda9_5.conda#75a8a98b1c4671c5d2897975731da42d
-https://conda.anaconda.org/conda-forge/osx-64/nodejs-18.16.1-h46e3395_0.conda#e4c06702959edec36072a3d081af4587
-https://conda.anaconda.org/conda-forge/osx-64/python-3.8.17-hf9b03c3_0_cpython.conda#f613b663d3829f325b4ffb626bf612b6
+https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-hfd90126_4.tar.bz2#be90e6223c74ea253080abae19b3bdb1
+https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_8.tar.bz2#aac5ad0d8f747ef7f871508146df75d9
+https://conda.anaconda.org/conda-forge/osx-64/nodejs-18.15.0-hd0c9b3c_0.conda#4c7eb1947ecaa10394cf1cbcca343131
+https://conda.anaconda.org/conda-forge/osx-64/python-3.8.16-hf9b03c3_1_cpython.conda#96d23d997c18a90efde924d9ca6dd5b3
+https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
 https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
 https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.0.9-py38h4cd09af_9.conda#f958e25488ff7e044031bca8a6c5267b
+https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_8.tar.bz2#55f612fe4a9b5f6ac76348b6de94aaeb
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.7-py38h4cd09af_0.conda#32626ffd5cd7eaad3036d7dca808ddc7
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/osx-64/docutils-0.20.1-py38h50d1736_0.conda#5722ca19ba9d5601032fd4dd5262b12a
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
-https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.3-py38hcafd530_0.conda#e8ee9933dc3749c889baccb1c4b4f014
-https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
-https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
+https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_robotmode-0.3.1-pyhd8ed1ab_0.tar.bz2#081f1505925bd5ff080864f4281c28a6
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.2-py38hef030d1_0.conda#011ae40b08362bc2b0b549f4fc0bd79f
+https://conda.anaconda.org/conda-forge/noarch/mistune-2.0.5-pyhd8ed1ab_0.conda#61a07195cfc935f1c1901d8ecf4af441
+https://conda.anaconda.org/conda-forge/noarch/natsort-8.3.1-pyhd8ed1ab_0.conda#8c53149aa69bfeb045f28c92a2b2ddc7
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda#02153b6b760bbec00cfe9e4c97993d06
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
 https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.5-py38hef030d1_0.conda#20b4cc7adae881327b943c883be6335e
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
+https://conda.anaconda.org/conda-forge/osx-64/pyrsistent-0.19.3-py38hef030d1_0.conda#01ca11f08679d88fc881a19902a0a008
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py38hef030d1_5.tar.bz2#e27d698dc29c6d5b49f1385bcd1d50f9
 https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.0-py38h3b70857_0.conda#a48761bc98b3bc22d209e9bb2f3dc5c1
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/noarch/robotframework-5.0.1-pyhd8ed1ab_0.tar.bz2#325df82f1bdd5175bb7b16d0c96e7d5e
-https://conda.anaconda.org/conda-forge/osx-64/rpds-py-0.9.2-py38h7510fb3_0.conda#bbd51a20bd2a5ad644516f860b9570aa
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py38hcafd530_0.conda#afefcf665a5049b030efb084a51e3935
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
-https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.1-pyhd8ed1ab_0.conda#7b517e7a6f0790337906c055aa97ca49
-https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.3-pyhd8ed1ab_0.conda#a3d2d43b74e042567cc4b5e328534885
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.2-pyhd8ed1ab_0.conda#bfe7e7cd1476092f51efbcde15dfb110
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/osx-64/y-py-0.5.9-py38he94b92c_0.conda#433e9f376d8b2295c16dcc9e97e0fea3
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py38hb368cf1_3.conda#a2b3ae2a1fd2aea0b4433d9e7fff8cf3
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
 https://conda.anaconda.org/conda-forge/osx-64/coverage-7.2.7-py38hcafd530_0.conda#868ae7c3c94b2fffbe28687a64646f53
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
-https://conda.anaconda.org/conda-forge/osx-64/pyobjc-core-9.2-py38h095c2e5_0.conda#8dbb4798b2066b678d8da47734d1c763
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
+https://conda.anaconda.org/conda-forge/osx-64/pyobjc-core-9.1.1-py38h8f2a8f7_0.conda#e8cdf74d4a128a7bdd574d6c06b3b994
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.30.0-pyhd8ed1ab_0.conda#13bf095e3ecd18999d65b4d3ac5b15d5
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-2.2.0-pyhd8ed1ab_0.tar.bz2#29a329f0b817038d27d7bdfb2ca04b5a
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyhd1c38e8_0.conda#046120b71d8896cb7faef78bfdbfee1e
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.4-pyhd8ed1ab_0.conda#18badd8fa3648d1beb1fcc7f2e0f756e
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.2-pyhd8ed1ab_0.conda#81a763f3c64fe6d5f32e033b0325265d
+https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
 https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py38hef030d1_3.tar.bz2#fc1bc20add8eff07c367973bba25e8eb
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.7.1-pyhd8ed1ab_0.conda#7c27ea1bdbe520bb830dcadd59f55cbf
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
-https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-9.2-py38h095c2e5_0.conda#fa3e3307ff143e7a9e823ce7bbc916ad
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
+https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-9.1.1-py38h8f2a8f7_0.conda#eaea41f1de16d95ce4de1fdd1b4bb295
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.15.0-pyhd8ed1ab_0.conda#02e7912139fb64828d18d07c43dcbad0
 https://conda.anaconda.org/conda-forge/osx-64/trio-0.21.0-py38h50d1736_0.tar.bz2#1e91102a7512cb5094ebe9818a361376
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.18.4-pyhd8ed1ab_0.conda#7356151a32ebd9a20158d2f26d224bfa
-https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.1-py38h50d1736_0.conda#03a3619e222793567b29b5966c2a821d
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
+https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.0-py38h50d1736_0.conda#c342b82641ef032fa8b256eb4f0a5649
+https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
+https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyhd1c38e8_0.conda#2657c3de5371c571aef6678afb4aaadd
-https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
+https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.2-pyhd8ed1ab_0.conda#4ec732d2264373773a5feaea477128a8
+https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/osx-64/ipython-7.33.0-py38h50d1736_0.tar.bz2#3bba83a6f445cccddfa5076ddbdd9467
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
-https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.8.0-pyhd8ed1ab_0.conda#1ca43103a08456b19222d93fd9d119ac
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh5fb750a_0.conda#2a8ffa559d393fea47237b9d23ddf74f
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh736e0ef_0.conda#d5aa7d2cc9fe03f62cf6e7bcc8e1a8df
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
 https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-5.1.3-pyhd8ed1ab_0.tar.bz2#464fdfebe1a1ffb41b031d8bbfb6041f
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda#32dde1678bb003c90d4bc0c2dbd21814
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
-https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.0-pyhd8ed1ab_0.conda#38589f4104d11f2a59ff01a9f4e3bfb3
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.4.0-pyhd8ed1ab_0.conda#4456e6030a8309bdad57569b0170b6a3
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.4.0-pyhd8ed1ab_0.conda#127c702e1b1eff595be82bc6a78cfce0
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.22.1-pyhd8ed1ab_0.conda#fc7172a6742a7c3c4331ddd7ed463ffc
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.4.0-pyhd8ed1ab_0.conda#a86727968b41c20dd3d73b91632e77dc
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.0.3-pyhd8ed1ab_0.conda#c861cae50ac4cbc6d573a947f67a2d0c
-https://conda.anaconda.org/conda-forge/noarch/notebook-7.0.0-pyhd8ed1ab_0.conda#a8aa205f2b275a786cf6e55bb60a2d1a
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server_ydoc-0.8.0-pyhd8ed1ab_0.conda#780280d42fbcb2eaf654a6ba7a3e5bb5
+https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
+https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.4-pyhd8ed1ab_0.conda#e66d4a6e36fcc92fe266932bf85fd35a
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/test/win-64/py3.11/lab3/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/linux-64/py3.11/lab4/conda.lock`

 * *Files 9% similar despite different names*

```diff
@@ -1,162 +1,160 @@
 @EXPLICIT
-https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2023.5.7-h56e8100_0.conda#604212634bd8c4d6f20d44b946e8eedb
-https://conda.anaconda.org/conda-forge/win-64/libexpat-2.5.0-h63175ca_1.conda#636cc3cbbd2e28bcfd2f73b2044aac2c
-https://conda.anaconda.org/conda-forge/win-64/nodejs-18.16.1-h57928b3_0.conda#8ceddf0826beb0b7730e89b2065d5b7e
-https://conda.anaconda.org/conda-forge/win-64/pandoc-3.1.3-h57928b3_0.conda#5185086e0662a98ae366212b5bef1af0
-https://conda.anaconda.org/conda-forge/win-64/python_abi-3.11-3_cp311.conda#fd1634ba85cfea9376e1fc02d6f592e9
+https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
+https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
+https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-12.2.0-h46fd767_19.tar.bz2#1030b1f38c129f2634eae026f704fe60
+https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.11-3_cp311.conda#c2e2630ddb68cf52eec74dc7dfab20b5
 https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
-https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
-https://conda.anaconda.org/conda-forge/win-64/winpty-0.4.3-4.tar.bz2#1cee351bf20b830d991dbe0bc8cd7dfe
-https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.36.32532-hfdfe4a8_17.conda#91c1ecaf3996889532fc0456178b1058
-https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h64f974e_17.conda#67ff6791f235bb606659bf2a5c169191
-https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.36.32532-h05e6639_17.conda#4618046c39f7c81861e53ded842e738a
-https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
-https://conda.anaconda.org/conda-forge/win-64/firefox-115.0-h63175ca_0.conda#e4e73664dd6be2e19a749b7c21da5d27
-https://conda.anaconda.org/conda-forge/win-64/geckodriver-0.33.0-h611cf2b_0.conda#e5ad5ec7f6140c1fdf9bd2a7927a4f91
-https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
-https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2#5c1fb45b5e2912c19098750ae8a32604
-https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.42.0-hcfcfb64_0.conda#9a71d93deb99cc09d8939d5235b5909a
-https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
-https://conda.anaconda.org/conda-forge/win-64/openssl-3.1.1-hcfcfb64_1.conda#1d913a5de46c6b2f7e4cfbd26b106b8b
-https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2#c69a5047cc9291ae40afd4a1ad6f0c0f
-https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
-https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
-https://conda.anaconda.org/conda-forge/win-64/python-3.11.4-h2628c8c_0_cpython.conda#3187a32fba79e835f099ecea054026f4
-https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.4-h0e60522_1.tar.bz2#e1aff0583dda5fb917eb3d2c1025aa80
-https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-12.2.0-h65d4601_19.tar.bz2#cedcee7c064c01c403f962c9e8d3c373
+https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-12.2.0-h65d4601_19.tar.bz2#e4c94f80aef025c17ab0828cd85ef535
+https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
+https://conda.anaconda.org/conda-forge/linux-64/firefox-113.0-h59595ed_0.conda#262f91a0dfca92813a3d469cc5453f61
+https://conda.anaconda.org/conda-forge/linux-64/geckodriver-0.33.0-hd2f7af9_0.conda#83664049f2b276cc23bd67d41eb9a4ee
+https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2#9194c9bf9428035a05352d031462eae4
+https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
+https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
+https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
+https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
+https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
+https://conda.anaconda.org/conda-forge/linux-64/libuv-1.44.2-h166bdaf_0.tar.bz2#e5cb4fe581a18ca2185a016eb848fc00
+https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-h166bdaf_4.tar.bz2#f3f9de449d32ca9b9c66a22863c96f41
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h27087fc_1.tar.bz2#4acfc691e64342b9dae57cf2adc63238
+https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
+https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
+https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2#4ae4d7795d33e02bd20f6b23d91caf82
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2#04bac51ba35ea023dc48af73c1c88c25
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
+https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
+https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
+https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
+https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-h166bdaf_4.tar.bz2#4b11e365c0275b808be78b30f904e295
+https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2#e5613f2bc717e9945840ff474419b8e4
+https://conda.anaconda.org/conda-forge/linux-64/nodejs-18.15.0-h4abf6b9_1.conda#2aabafd88f6876a57c45c00598715ac4
+https://conda.anaconda.org/conda-forge/linux-64/python-3.11.3-h2755cc3_0_cpython.conda#37005ea5f68df6a8a381b70cf4d4a160
+https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/win-64/brotli-python-1.0.9-py311h12c1d0e_9.conda#e3f916714f59b88acb5d3c9d83b6f44a
+https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_8.tar.bz2#2ff08978892a3e8b954397c461f18418
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
-https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
-https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.7-py311h12c1d0e_0.conda#b056c7299be929b711016d2f4e48d303
+https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py311hcafe171_0.conda#f4c810ad9d791c8df5ad900ed74b085b
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
-https://conda.anaconda.org/conda-forge/win-64/docutils-0.20.1-py311h1ea47a8_0.conda#851f4c302cc7f5a617cc03a3c2090634
+https://conda.anaconda.org/conda-forge/linux-64/docutils-0.20.1-py311h38be061_0.conda#207175b7d514d42f977ec505800d6824
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
-https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_robotmode-0.3.1-pyhd8ed1ab_0.tar.bz2#081f1505925bd5ff080864f4281c28a6
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
-https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.3-py311ha68e1ae_0.conda#db2c2f72a83bdc5b70947964e1ddc8bb
-https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
-https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.2-py311h2582759_0.conda#adb20bd57069614552adac60a020c36d
+https://conda.anaconda.org/conda-forge/noarch/mistune-2.0.5-pyhd8ed1ab_0.conda#61a07195cfc935f1c1901d8ecf4af441
+https://conda.anaconda.org/conda-forge/noarch/natsort-8.3.1-pyhd8ed1ab_0.conda#8c53149aa69bfeb045f28c92a2b2ddc7
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda#02153b6b760bbec00cfe9e4c97993d06
-https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.5-py311ha68e1ae_0.conda#f1a1eecd1bb4f431df5b9b6d8a152efd
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
+https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py311h2582759_0.conda#a90f8e278c1cd7064b2713e6b7db87e6
+https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
+https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py311h2582759_0.conda#e53876b66dcc4ba8a0afa63cd8502ac3
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
-https://conda.anaconda.org/conda-forge/win-64/pywin32-304-py311h12c1d0e_2.tar.bz2#20a2d8e73b0be8e27ca4096d4f3a7053
-https://conda.anaconda.org/conda-forge/win-64/pywinpty-2.0.11-py311h12c1d0e_0.conda#dd979ef7f5a96b0a607dbfe6d5028fef
-https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py311ha68e1ae_5.tar.bz2#0c97d59d54eb52e170224b3de6ade906
-https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.0-py311h7b3f143_0.conda#b690f6e1878ccc98e96a33658867e8e1
+https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py311hd4cff14_5.tar.bz2#da8769492e423103c59f469f4f17f8d9
+https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py311h75c88c4_0.conda#db94a7a9e865fbfde8c023b6e8958bb2
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
-https://conda.anaconda.org/conda-forge/noarch/robotframework-6.1-pyhd8ed1ab_0.conda#e383bebdc0d8fea4ecf9c9e01d0959fe
-https://conda.anaconda.org/conda-forge/win-64/rpds-py-0.9.2-py311hc37eb10_0.conda#d2d75b1d27bcd4f7b6d049b32b2f7530
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/noarch/robotframework-6.0.2-pyhd8ed1ab_1.conda#b4dcead8c5a99a14733d9b1ba5b7db09
+https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh41d4057_0.conda#ada5a17adcd10be4fc7e37e4166ba0e2
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
-https://conda.anaconda.org/conda-forge/win-64/tornado-6.3.2-py311ha68e1ae_0.conda#e2a6c106c1cff7e884d93351cdee3c3e
+https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py311h459d7ec_0.conda#12b1c374ee90a1aa11ea921858394dc8
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
-https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
-https://conda.anaconda.org/conda-forge/win-64/y-py-0.5.9-py311hc37eb10_0.conda#c16da06cd2c39bba7391076fd64024d8
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.2-pyhd8ed1ab_0.conda#bfe7e7cd1476092f51efbcde15dfb110
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
+https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.2-pyhd8ed1ab_0.conda#41221f97a0c82e5a60b21716a3d7469c
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
-https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py311h7d9ee11_3.conda#a8524727eb956b4741e25a64af79edb8
+https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py311h409f033_3.conda#9025d0786dbbe4bc91fd8e85502decce
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
-https://conda.anaconda.org/conda-forge/win-64/coverage-7.2.7-py311ha68e1ae_0.conda#b3a60b6bb264fe70896de40fa392edf6
+https://conda.anaconda.org/conda-forge/linux-64/coverage-7.2.7-py311h459d7ec_0.conda#3c2c65575c28b23afc5e4ff721a2fc9f
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
-https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
+https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.30.0-pyhd8ed1ab_0.conda#13bf095e3ecd18999d65b4d3ac5b15d5
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.2.0-pyhd8ed1ab_0.conda#c9e9064ab45ffb46f7a96834d9e7626d
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
-https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh08f2357_0.conda#c00d32dfa733d381b6a1908d0d67e0d7
-https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.0-pyh08f2357_0.tar.bz2#0152a609d5748ed9887d195b1e61a6c9
+https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
-https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
-https://conda.anaconda.org/conda-forge/win-64/argon2-cffi-bindings-21.2.0-py311ha68e1ae_3.tar.bz2#c321cd825b72a2073dfb3f92ce1507fb
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.2-pyhd8ed1ab_0.conda#81a763f3c64fe6d5f32e033b0325265d
+https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py311hd4cff14_3.tar.bz2#5159e874f65ac382773d2b534a1d7b80
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.7.1-pyhd8ed1ab_0.conda#7c27ea1bdbe520bb830dcadd59f55cbf
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
+https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.15.0-pyhd8ed1ab_0.conda#02e7912139fb64828d18d07c43dcbad0
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/win-64/trio-0.22.2-py311h1ea47a8_0.conda#621bba80ba8161029c356642c8b0080a
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.4-pyhd8ed1ab_0.conda#18badd8fa3648d1beb1fcc7f2e0f756e
+https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.0-py311h38be061_1.tar.bz2#0564e63c41c0527f8085a572a931f1e6
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.18.4-pyhd8ed1ab_0.conda#7356151a32ebd9a20158d2f26d224bfa
-https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.3.1-py311h1ea47a8_0.conda#6754e6f5ead86225c8c78825ff0398c9
-https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
-https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
-https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
+https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.0-py311h38be061_0.conda#1dd43a18a75d59206019e2a2a28555e5
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.2-pyhd8ed1ab_0.conda#4ec732d2264373773a5feaea477128a8
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
-https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh08f2357_0.conda#1fc684c1de5475383790ada5627c5430
+https://conda.anaconda.org/conda-forge/noarch/ipython-8.13.2-pyh41d4057_0.conda#e8563c13eee80a5f1c7bdfc2a1b20077
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
-https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh6817e22_0.conda#b5cd11cf19c739548e968c12e020c54d
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda#32dde1678bb003c90d4bc0c2dbd21814
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.1-pyhd8ed1ab_1.conda#796b056965d7146bcac082fa2a83943d
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.1-pyhd8ed1ab_1.conda#95d9d1523df069792cd059f412be0d6e
+https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_0.conda#15700afca8f7ab35542e9c1af63568f1
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh210e3f2_0.conda#4b57b688e22d094d1479a35543c18e93
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.4.0-pyhd8ed1ab_0.conda#4456e6030a8309bdad57569b0170b6a3
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
+https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.0-pyhd8ed1ab_0.conda#38589f4104d11f2a59ff01a9f4e3bfb3
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.22.1-pyhd8ed1ab_0.conda#fc7172a6742a7c3c4331ddd7ed463ffc
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server_ydoc-0.8.0-pyhd8ed1ab_0.conda#780280d42fbcb2eaf654a6ba7a3e5bb5
-https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
-https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.5-pyhd8ed1ab_0.conda#82299e1d33c6f130688f90880e6b3b4f
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.0.1-pyhd8ed1ab_0.conda#93cc832cb8e18caa52c7b36ea6ce7f3d
+https://conda.anaconda.org/conda-forge/label/notebook_beta/noarch/notebook-7.0.0b3-pyhb537eac_0.conda#a654d4b1443e5f3ac52d3a3dc1b19b17
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/test/win-64/py3.11/lab4/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/win-64/py3.8/lab4/conda.lock`

 * *Files 13% similar despite different names*

```diff
@@ -1,151 +1,147 @@
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2023.5.7-h56e8100_0.conda#604212634bd8c4d6f20d44b946e8eedb
-https://conda.anaconda.org/conda-forge/win-64/libexpat-2.5.0-h63175ca_1.conda#636cc3cbbd2e28bcfd2f73b2044aac2c
-https://conda.anaconda.org/conda-forge/win-64/nodejs-18.16.1-h57928b3_0.conda#8ceddf0826beb0b7730e89b2065d5b7e
-https://conda.anaconda.org/conda-forge/win-64/python_abi-3.11-3_cp311.conda#fd1634ba85cfea9376e1fc02d6f592e9
-https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
+https://conda.anaconda.org/conda-forge/win-64/nodejs-18.15.0-h57928b3_1.conda#d728bbdc9a650a5d503d657ce12c01ce
+https://conda.anaconda.org/conda-forge/win-64/python_abi-3.8-3_cp38.conda#c6df946723dadd4a5830a8ff8c6b9a20
 https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
 https://conda.anaconda.org/conda-forge/win-64/winpty-0.4.3-4.tar.bz2#1cee351bf20b830d991dbe0bc8cd7dfe
-https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.36.32532-hfdfe4a8_17.conda#91c1ecaf3996889532fc0456178b1058
-https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h64f974e_17.conda#67ff6791f235bb606659bf2a5c169191
-https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.36.32532-h05e6639_17.conda#4618046c39f7c81861e53ded842e738a
+https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.34.31931-h5081d32_16.conda#22125178654c6a8a393f9743d585704b
+https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hb25d44b_16.conda#ea326b37e3bd6d2616988e09f3a9396c
+https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.34.31931-hed1258a_16.conda#0374eae69b6dbfb27c3dc27167109eb4
 https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
-https://conda.anaconda.org/conda-forge/win-64/firefox-115.0-h63175ca_0.conda#e4e73664dd6be2e19a749b7c21da5d27
+https://conda.anaconda.org/conda-forge/win-64/firefox-113.0-h63175ca_0.conda#a2bd8315d1c49f718d4ffe0b7cf39e00
 https://conda.anaconda.org/conda-forge/win-64/geckodriver-0.33.0-h611cf2b_0.conda#e5ad5ec7f6140c1fdf9bd2a7927a4f91
+https://conda.anaconda.org/conda-forge/win-64/libbrotlicommon-1.0.9-hcfcfb64_8.tar.bz2#e8078e37208cd7d3e1eb5053f370ded8
 https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
 https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2#5c1fb45b5e2912c19098750ae8a32604
 https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.42.0-hcfcfb64_0.conda#9a71d93deb99cc09d8939d5235b5909a
-https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
+https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_4.tar.bz2#0cc5c5cc64ee1637f37f8540a175854c
 https://conda.anaconda.org/conda-forge/win-64/openssl-3.1.1-hcfcfb64_1.conda#1d913a5de46c6b2f7e4cfbd26b106b8b
 https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2#c69a5047cc9291ae40afd4a1ad6f0c0f
 https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
 https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
-https://conda.anaconda.org/conda-forge/win-64/python-3.11.4-h2628c8c_0_cpython.conda#3187a32fba79e835f099ecea054026f4
+https://conda.anaconda.org/conda-forge/win-64/libbrotlidec-1.0.9-hcfcfb64_8.tar.bz2#99839d9d81f33afa173c0fa82a702038
+https://conda.anaconda.org/conda-forge/win-64/libbrotlienc-1.0.9-hcfcfb64_8.tar.bz2#88e62627120c20289bf8982b15e0a6a1
+https://conda.anaconda.org/conda-forge/win-64/python-3.8.16-h4de0772_1_cpython.conda#461d9fc92cfde68f2ca7ef0988f6326a
 https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.4-h0e60522_1.tar.bz2#e1aff0583dda5fb917eb3d2c1025aa80
+https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/win-64/brotli-python-1.0.9-py311h12c1d0e_9.conda#e3f916714f59b88acb5d3c9d83b6f44a
+https://conda.anaconda.org/conda-forge/win-64/brotli-bin-1.0.9-hcfcfb64_8.tar.bz2#e18b70ed349d96086fd60a9c642b1b58
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
-https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.7-py311h12c1d0e_0.conda#b056c7299be929b711016d2f4e48d303
+https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.7-py38hd3f51b4_0.conda#de2533e0a4ad84a4e5c5d6ad196f8e14
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
-https://conda.anaconda.org/conda-forge/win-64/docutils-0.20.1-py311h1ea47a8_0.conda#851f4c302cc7f5a617cc03a3c2090634
+https://conda.anaconda.org/conda-forge/win-64/docutils-0.20.1-py38haa244fe_0.conda#8f4292bb1a13ed095a725c137843da5f
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
-https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
-https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.3-py311ha68e1ae_0.conda#db2c2f72a83bdc5b70947964e1ddc8bb
-https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
-https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.2-py38h91455d4_0.conda#962b32c8c11df005d9e225ecde549e57
+https://conda.anaconda.org/conda-forge/noarch/mistune-2.0.5-pyhd8ed1ab_0.conda#61a07195cfc935f1c1901d8ecf4af441
+https://conda.anaconda.org/conda-forge/noarch/natsort-8.3.1-pyhd8ed1ab_0.conda#8c53149aa69bfeb045f28c92a2b2ddc7
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda#02153b6b760bbec00cfe9e4c97993d06
-https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.5-py311ha68e1ae_0.conda#f1a1eecd1bb4f431df5b9b6d8a152efd
-https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
+https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.5-py38h91455d4_0.conda#091a6bc808bfd07c97be1eb316440070
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
+https://conda.anaconda.org/conda-forge/win-64/pyrsistent-0.19.3-py38h91455d4_0.conda#fb4aa6d774c3a286a8561af24ff87185
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
-https://conda.anaconda.org/conda-forge/win-64/pywin32-304-py311h12c1d0e_2.tar.bz2#20a2d8e73b0be8e27ca4096d4f3a7053
-https://conda.anaconda.org/conda-forge/win-64/pywinpty-2.0.11-py311h12c1d0e_0.conda#dd979ef7f5a96b0a607dbfe6d5028fef
-https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py311ha68e1ae_5.tar.bz2#0c97d59d54eb52e170224b3de6ade906
-https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.0-py311h7b3f143_0.conda#b690f6e1878ccc98e96a33658867e8e1
+https://conda.anaconda.org/conda-forge/win-64/pywin32-304-py38hd3f51b4_2.tar.bz2#cfefffaad808b61f2932f64c079417b8
+https://conda.anaconda.org/conda-forge/win-64/pywinpty-2.0.10-py38hd3f51b4_0.conda#cc93c5fe55b8a7bdd719ce74bfbe819c
+https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py38h91455d4_5.tar.bz2#f62ab7e18711e3cbc068319448ecf771
+https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.0-py38ha85f68a_0.conda#5e97b9e91fc8cb7ec32647d5bec74030
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
-https://conda.anaconda.org/conda-forge/noarch/robotframework-6.1-pyhd8ed1ab_0.conda#e383bebdc0d8fea4ecf9c9e01d0959fe
-https://conda.anaconda.org/conda-forge/win-64/rpds-py-0.9.2-py311hc37eb10_0.conda#d2d75b1d27bcd4f7b6d049b32b2f7530
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/noarch/robotframework-5.0.1-pyhd8ed1ab_0.tar.bz2#325df82f1bdd5175bb7b16d0c96e7d5e
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
-https://conda.anaconda.org/conda-forge/win-64/tornado-6.3.2-py311ha68e1ae_0.conda#e2a6c106c1cff7e884d93351cdee3c3e
+https://conda.anaconda.org/conda-forge/win-64/tornado-6.3.2-py38h91455d4_0.conda#3e625e06e8892112acb47695eaf22b47
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.2-pyhd8ed1ab_0.conda#bfe7e7cd1476092f51efbcde15dfb110
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
 https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
-https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
-https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
-https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.3-pyhd8ed1ab_0.conda#a3d2d43b74e042567cc4b5e328534885
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
+https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.2-pyhd8ed1ab_0.conda#41221f97a0c82e5a60b21716a3d7469c
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
-https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py311h7d9ee11_3.conda#a8524727eb956b4741e25a64af79edb8
+https://conda.anaconda.org/conda-forge/win-64/brotli-1.0.9-hcfcfb64_8.tar.bz2#2e661f21e1741c11506bdc7226e6b0bc
+https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py38h57701bc_3.conda#9b94af390cfdf924a063302a2ddb3860
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
-https://conda.anaconda.org/conda-forge/win-64/coverage-7.2.7-py311ha68e1ae_0.conda#b3a60b6bb264fe70896de40fa392edf6
+https://conda.anaconda.org/conda-forge/win-64/coverage-7.2.7-py38h91455d4_0.conda#2fa3faef0a7b6a5da2bff0faddbfbc68
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.30.0-pyhd8ed1ab_0.conda#13bf095e3ecd18999d65b4d3ac5b15d5
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.2.0-pyhd8ed1ab_0.conda#c9e9064ab45ffb46f7a96834d9e7626d
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-2.2.0-pyhd8ed1ab_0.tar.bz2#29a329f0b817038d27d7bdfb2ca04b5a
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh08f2357_0.conda#c00d32dfa733d381b6a1908d0d67e0d7
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.0-pyh08f2357_0.tar.bz2#0152a609d5748ed9887d195b1e61a6c9
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
-https://conda.anaconda.org/conda-forge/win-64/argon2-cffi-bindings-21.2.0-py311ha68e1ae_3.tar.bz2#c321cd825b72a2073dfb3f92ce1507fb
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
+https://conda.anaconda.org/conda-forge/win-64/argon2-cffi-bindings-21.2.0-py38h91455d4_3.tar.bz2#a262d1c7aaf5a93a02b33dd985c27831
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.7.1-pyhd8ed1ab_0.conda#7c27ea1bdbe520bb830dcadd59f55cbf
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
-https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-https://conda.anaconda.org/conda-forge/win-64/trio-0.22.2-py311h1ea47a8_0.conda#621bba80ba8161029c356642c8b0080a
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.4-pyhd8ed1ab_0.conda#18badd8fa3648d1beb1fcc7f2e0f756e
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.15.0-pyhd8ed1ab_0.conda#02e7912139fb64828d18d07c43dcbad0
+https://conda.anaconda.org/conda-forge/win-64/trio-0.21.0-py38haa244fe_0.tar.bz2#0fe81ab845eea9441bc9a025d47577be
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.2-pyhd8ed1ab_0.conda#81a763f3c64fe6d5f32e033b0325265d
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.18.4-pyhd8ed1ab_0.conda#7356151a32ebd9a20158d2f26d224bfa
-https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.3.1-py311h1ea47a8_0.conda#6754e6f5ead86225c8c78825ff0398c9
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
+https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.3.0-py38haa244fe_0.conda#ff05e328ef5915b4a8176844f5effddd
+https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
+https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.2-pyhd8ed1ab_0.conda#4ec732d2264373773a5feaea477128a8
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
-https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
-https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
+https://conda.anaconda.org/conda-forge/win-64/ipython-7.33.0-py38haa244fe_0.tar.bz2#1185ff9399904ccd14f2eadbbca1aeab
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
-https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh08f2357_0.conda#1fc684c1de5475383790ada5627c5430
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh025b116_0.conda#d18e38ce1f195efa2d76f9dc33832bf5
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
-https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh6817e22_0.conda#b5cd11cf19c739548e968c12e020c54d
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda#32dde1678bb003c90d4bc0c2dbd21814
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
+https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-5.1.3-pyhd8ed1ab_0.tar.bz2#464fdfebe1a1ffb41b031d8bbfb6041f
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.4.0-pyhd8ed1ab_0.conda#4456e6030a8309bdad57569b0170b6a3
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
 https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.0-pyhd8ed1ab_0.conda#38589f4104d11f2a59ff01a9f4e3bfb3
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.22.1-pyhd8ed1ab_0.conda#fc7172a6742a7c3c4331ddd7ed463ffc
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.0.3-pyhd8ed1ab_0.conda#c861cae50ac4cbc6d573a947f67a2d0c
-https://conda.anaconda.org/conda-forge/noarch/notebook-7.0.0-pyhd8ed1ab_0.conda#a8aa205f2b275a786cf6e55bb60a2d1a
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.0.1-pyhd8ed1ab_0.conda#93cc832cb8e18caa52c7b36ea6ce7f3d
+https://conda.anaconda.org/conda-forge/label/notebook_beta/noarch/notebook-7.0.0b3-pyhb537eac_0.conda#a654d4b1443e5f3ac52d3a3dc1b19b17
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/test/win-64/py3.8/lab3/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/osx-64/py3.11/lab3/conda.lock`

 * *Files 6% similar despite different names*

```diff
@@ -1,156 +1,167 @@
 @EXPLICIT
-https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2023.5.7-h56e8100_0.conda#604212634bd8c4d6f20d44b946e8eedb
-https://conda.anaconda.org/conda-forge/win-64/nodejs-18.16.1-h57928b3_0.conda#8ceddf0826beb0b7730e89b2065d5b7e
-https://conda.anaconda.org/conda-forge/win-64/pandoc-3.1.3-h57928b3_0.conda#5185086e0662a98ae366212b5bef1af0
-https://conda.anaconda.org/conda-forge/win-64/python_abi-3.8-3_cp38.conda#c6df946723dadd4a5830a8ff8c6b9a20
-https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
-https://conda.anaconda.org/conda-forge/win-64/winpty-0.4.3-4.tar.bz2#1cee351bf20b830d991dbe0bc8cd7dfe
-https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.36.32532-hfdfe4a8_17.conda#91c1ecaf3996889532fc0456178b1058
-https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h64f974e_17.conda#67ff6791f235bb606659bf2a5c169191
-https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.36.32532-h05e6639_17.conda#4618046c39f7c81861e53ded842e738a
-https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
-https://conda.anaconda.org/conda-forge/win-64/firefox-115.0-h63175ca_0.conda#e4e73664dd6be2e19a749b7c21da5d27
-https://conda.anaconda.org/conda-forge/win-64/geckodriver-0.33.0-h611cf2b_0.conda#e5ad5ec7f6140c1fdf9bd2a7927a4f91
-https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
-https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2#5c1fb45b5e2912c19098750ae8a32604
-https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.42.0-hcfcfb64_0.conda#9a71d93deb99cc09d8939d5235b5909a
-https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
-https://conda.anaconda.org/conda-forge/win-64/openssl-3.1.1-hcfcfb64_1.conda#1d913a5de46c6b2f7e4cfbd26b106b8b
-https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2#c69a5047cc9291ae40afd4a1ad6f0c0f
-https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
-https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
-https://conda.anaconda.org/conda-forge/win-64/python-3.8.17-h4de0772_0_cpython.conda#be2296eaf70eeb1cb83c4e95136e694a
-https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.4-h0e60522_1.tar.bz2#e1aff0583dda5fb917eb3d2c1025aa80
+https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
+https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_8.tar.bz2#37157d273eaf3bc7d6862104161d9ec9
+https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.4-hd57cbcb_0.conda#195236e2eeb3b108e3b8eee47ad074fd
+https://conda.anaconda.org/conda-forge/osx-64/libexpat-2.5.0-hf0c8a7f_1.conda#6c81cb022780ee33435cca0127dd43c9
+https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
+https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2#24632c09ed931af617fe6d5292919cab
+https://conda.anaconda.org/conda-forge/osx-64/libuv-1.44.2-hac89ed1_0.tar.bz2#958fa9add5701462a6c91e3774425ea1
+https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-hfd90126_4.tar.bz2#35eb3fce8d51ed3c1fd4122bad48250b
+https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.3-h96cf925_1.tar.bz2#76217ebfbb163ff2770a261f955a5861
+https://conda.anaconda.org/conda-forge/osx-64/pandoc-2.19.2-h694c41f_2.conda#de3014568ff5004048dd09ba73990430
+https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.11-3_cp311.conda#5e0a069a585445333868d2c6651c3b3f
+https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
+https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
+https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
+https://conda.anaconda.org/conda-forge/osx-64/firefox-113.0-he965462_0.conda#6730ed9d9f8ff58391adf5fe00c984c4
+https://conda.anaconda.org/conda-forge/osx-64/geckodriver-0.33.0-hf46a32e_0.conda#897200360380560ac85cf0756161dd78
+https://conda.anaconda.org/conda-forge/osx-64/icu-70.1-h96cf925_0.tar.bz2#376635049e9b9b0bb875efd39dcd7b3b
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_8.tar.bz2#7f952a036d9014b4dab96c6ea0f8c2a7
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_8.tar.bz2#b36a3bfe866d9127f25f286506982166
+https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
+https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
+https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
+https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
+https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
+https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-hfd90126_4.tar.bz2#be90e6223c74ea253080abae19b3bdb1
+https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_8.tar.bz2#aac5ad0d8f747ef7f871508146df75d9
+https://conda.anaconda.org/conda-forge/osx-64/nodejs-18.15.0-hd0c9b3c_0.conda#4c7eb1947ecaa10394cf1cbcca343131
+https://conda.anaconda.org/conda-forge/osx-64/python-3.11.3-h99528f9_0_cpython.conda#c3291f9411424fc587d53a2ea57fb075
 https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
+https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
 https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/win-64/brotli-python-1.0.9-py38hd3f51b4_9.conda#b451fb48b1337ceb34b7b39de0bc09c8
+https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_8.tar.bz2#55f612fe4a9b5f6ac76348b6de94aaeb
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
-https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
-https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.7-py38hd3f51b4_0.conda#de2533e0a4ad84a4e5c5d6ad196f8e14
+https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.7-py311h814d153_0.conda#c27802860b87fe024c9b6276205a56b5
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
-https://conda.anaconda.org/conda-forge/win-64/docutils-0.20.1-py38haa244fe_0.conda#8f4292bb1a13ed095a725c137843da5f
+https://conda.anaconda.org/conda-forge/osx-64/docutils-0.20.1-py311h6eed73b_0.conda#0536cbe889e20101b7f8e6d6b1dbcbf4
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_robotmode-0.3.1-pyhd8ed1ab_0.tar.bz2#081f1505925bd5ff080864f4281c28a6
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
-https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.3-py38h91455d4_0.conda#a674b0be89418013ffa8f92c89d08640
-https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
-https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.2-py311h5547dcb_0.conda#13091519d55d667506aaf413cffaff10
+https://conda.anaconda.org/conda-forge/noarch/mistune-2.0.5-pyhd8ed1ab_0.conda#61a07195cfc935f1c1901d8ecf4af441
+https://conda.anaconda.org/conda-forge/noarch/natsort-8.3.1-pyhd8ed1ab_0.conda#8c53149aa69bfeb045f28c92a2b2ddc7
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda#02153b6b760bbec00cfe9e4c97993d06
-https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.5-py38h91455d4_0.conda#091a6bc808bfd07c97be1eb316440070
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
+https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.5-py311h5547dcb_0.conda#d9b4565309f4f992b42bd99031044642
+https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
+https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
+https://conda.anaconda.org/conda-forge/osx-64/pyrsistent-0.19.3-py311h5547dcb_0.conda#f114c0dab9f9c894b260297371124634
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
-https://conda.anaconda.org/conda-forge/win-64/pywin32-304-py38hd3f51b4_2.tar.bz2#cfefffaad808b61f2932f64c079417b8
-https://conda.anaconda.org/conda-forge/win-64/pywinpty-2.0.11-py38hd3f51b4_0.conda#6d7d5d94ab48044490f8934923074ba2
-https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py38h91455d4_5.tar.bz2#f62ab7e18711e3cbc068319448ecf771
-https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.0-py38ha85f68a_0.conda#5e97b9e91fc8cb7ec32647d5bec74030
+https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py311h5547dcb_5.tar.bz2#8d1e456914ce961119b07f396187a564
+https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.0-py311h5dacc12_0.conda#1f65b37886e7cb8476d48ea8bb9d19c0
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
-https://conda.anaconda.org/conda-forge/noarch/robotframework-5.0.1-pyhd8ed1ab_0.tar.bz2#325df82f1bdd5175bb7b16d0c96e7d5e
-https://conda.anaconda.org/conda-forge/win-64/rpds-py-0.9.2-py38h4900a04_0.conda#222e659fb9e09325b23979c70c87784b
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/noarch/robotframework-6.0.2-pyhd8ed1ab_1.conda#b4dcead8c5a99a14733d9b1ba5b7db09
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
-https://conda.anaconda.org/conda-forge/win-64/tornado-6.3.2-py38h91455d4_0.conda#3e625e06e8892112acb47695eaf22b47
+https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py311h2725bcf_0.conda#276fe4341e39dcd9d9d33ca18140d2e7
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
-https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
-https://conda.anaconda.org/conda-forge/win-64/y-py-0.5.9-py38h4900a04_0.conda#4ba79cbf620ff0cd934fee88bb9c7713
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
-https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.1-pyhd8ed1ab_0.conda#7b517e7a6f0790337906c055aa97ca49
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.2-pyhd8ed1ab_0.conda#bfe7e7cd1476092f51efbcde15dfb110
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/osx-64/y-py-0.5.9-py311h890d03e_0.conda#d333683779e7145d5fe8bb18e08a7623
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
+https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
-https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py38h57701bc_3.conda#9b94af390cfdf924a063302a2ddb3860
+https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py311ha86e640_3.conda#5967be4da33261eada7cc79593f71088
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
-https://conda.anaconda.org/conda-forge/win-64/coverage-7.2.7-py38h91455d4_0.conda#2fa3faef0a7b6a5da2bff0faddbfbc68
+https://conda.anaconda.org/conda-forge/osx-64/coverage-7.2.7-py311h2725bcf_0.conda#afba3a3f74c5f71ebd9f400871e8c4de
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
-https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
+https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
+https://conda.anaconda.org/conda-forge/osx-64/pyobjc-core-9.1.1-py311hfd07503_0.conda#ba333461302daaea2dfce2d5223c876e
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.30.0-pyhd8ed1ab_0.conda#13bf095e3ecd18999d65b4d3ac5b15d5
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-2.2.0-pyhd8ed1ab_0.tar.bz2#29a329f0b817038d27d7bdfb2ca04b5a
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
-https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh08f2357_0.conda#c00d32dfa733d381b6a1908d0d67e0d7
-https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.0-pyh08f2357_0.tar.bz2#0152a609d5748ed9887d195b1e61a6c9
+https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyhd1c38e8_0.conda#046120b71d8896cb7faef78bfdbfee1e
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.2-pyhd8ed1ab_0.conda#81a763f3c64fe6d5f32e033b0325265d
 https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
-https://conda.anaconda.org/conda-forge/win-64/argon2-cffi-bindings-21.2.0-py38h91455d4_3.tar.bz2#a262d1c7aaf5a93a02b33dd985c27831
+https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py311h5547dcb_3.tar.bz2#c09459e349fa61afc352f473766de109
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.7.1-pyhd8ed1ab_0.conda#7c27ea1bdbe520bb830dcadd59f55cbf
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
-https://conda.anaconda.org/conda-forge/win-64/trio-0.21.0-py38haa244fe_0.tar.bz2#0fe81ab845eea9441bc9a025d47577be
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.4-pyhd8ed1ab_0.conda#18badd8fa3648d1beb1fcc7f2e0f756e
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
+https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-9.1.1-py311hfd07503_0.conda#d8c5226abc26b750ebdc5d40d00e7b35
+https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.15.0-pyhd8ed1ab_0.conda#02e7912139fb64828d18d07c43dcbad0
+https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
+https://conda.anaconda.org/conda-forge/osx-64/trio-0.22.0-py311h6eed73b_1.tar.bz2#71a739c4b0b1e17cfd27cfdf828d52a8
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.18.4-pyhd8ed1ab_0.conda#7356151a32ebd9a20158d2f26d224bfa
-https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.3.1-py38haa244fe_0.conda#15542a4c949a848b768a9e3b8ce3dd30
-https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
-https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
-https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
-https://conda.anaconda.org/conda-forge/win-64/ipython-7.33.0-py38haa244fe_0.tar.bz2#1185ff9399904ccd14f2eadbbca1aeab
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
+https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.0-py311h6eed73b_0.conda#e0e5cfb36ece6eae9c355eed1e90ff9d
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
+https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyhd1c38e8_0.conda#2657c3de5371c571aef6678afb4aaadd
+https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.2-pyhd8ed1ab_0.conda#4ec732d2264373773a5feaea477128a8
+https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.8.0-pyhd8ed1ab_0.conda#1ca43103a08456b19222d93fd9d119ac
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh6817e22_0.conda#b5cd11cf19c739548e968c12e020c54d
+https://conda.anaconda.org/conda-forge/noarch/ipython-8.13.2-pyhd1c38e8_0.conda#30960117dd6bd242aec8428a1004b167
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
-https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-5.1.3-pyhd8ed1ab_0.tar.bz2#464fdfebe1a1ffb41b031d8bbfb6041f
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda#32dde1678bb003c90d4bc0c2dbd21814
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.1-pyhd8ed1ab_1.conda#796b056965d7146bcac082fa2a83943d
+https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_0.conda#15700afca8f7ab35542e9c1af63568f1
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh736e0ef_0.conda#d5aa7d2cc9fe03f62cf6e7bcc8e1a8df
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.4.0-pyhd8ed1ab_0.conda#4456e6030a8309bdad57569b0170b6a3
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.4.0-pyhd8ed1ab_0.conda#127c702e1b1eff595be82bc6a78cfce0
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.1-pyhd8ed1ab_1.conda#95d9d1523df069792cd059f412be0d6e
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.22.1-pyhd8ed1ab_0.conda#fc7172a6742a7c3c4331ddd7ed463ffc
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.4.0-pyhd8ed1ab_0.conda#a86727968b41c20dd3d73b91632e77dc
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_ydoc-0.8.0-pyhd8ed1ab_0.conda#780280d42fbcb2eaf654a6ba7a3e5bb5
 https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
 https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.5-pyhd8ed1ab_0.conda#82299e1d33c6f130688f90880e6b3b4f
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.4-pyhd8ed1ab_0.conda#e66d4a6e36fcc92fe266932bf85fd35a
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/locks/test/win-64/py3.8/lab4/conda.lock` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/osx-64/py3.8/lab4/conda.lock`

 * *Files 5% similar despite different names*

```diff
@@ -1,145 +1,149 @@
 @EXPLICIT
-https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2023.5.7-h56e8100_0.conda#604212634bd8c4d6f20d44b946e8eedb
-https://conda.anaconda.org/conda-forge/win-64/nodejs-18.16.1-h57928b3_0.conda#8ceddf0826beb0b7730e89b2065d5b7e
-https://conda.anaconda.org/conda-forge/win-64/python_abi-3.8-3_cp38.conda#c6df946723dadd4a5830a8ff8c6b9a20
-https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2#72608f6cd3e5898229c3ea16deb1ac43
-https://conda.anaconda.org/conda-forge/win-64/winpty-0.4.3-4.tar.bz2#1cee351bf20b830d991dbe0bc8cd7dfe
-https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.36.32532-hfdfe4a8_17.conda#91c1ecaf3996889532fc0456178b1058
-https://conda.anaconda.org/conda-forge/win-64/vc-14.3-h64f974e_17.conda#67ff6791f235bb606659bf2a5c169191
-https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.36.32532-h05e6639_17.conda#4618046c39f7c81861e53ded842e738a
-https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
-https://conda.anaconda.org/conda-forge/win-64/firefox-115.0-h63175ca_0.conda#e4e73664dd6be2e19a749b7c21da5d27
-https://conda.anaconda.org/conda-forge/win-64/geckodriver-0.33.0-h611cf2b_0.conda#e5ad5ec7f6140c1fdf9bd2a7927a4f91
-https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2#2c96d1b6915b408893f9472569dee135
-https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2#5c1fb45b5e2912c19098750ae8a32604
-https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.42.0-hcfcfb64_0.conda#9a71d93deb99cc09d8939d5235b5909a
-https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda#5fdb9c6a113b6b6cb5e517fd972d5f41
-https://conda.anaconda.org/conda-forge/win-64/openssl-3.1.1-hcfcfb64_1.conda#1d913a5de46c6b2f7e4cfbd26b106b8b
-https://conda.anaconda.org/conda-forge/win-64/tk-8.6.12-h8ffe710_0.tar.bz2#c69a5047cc9291ae40afd4a1ad6f0c0f
-https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2#515d77642eaa3639413c6b1bc3f94219
-https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2#adbfb9f45d1004a26763652246a33764
-https://conda.anaconda.org/conda-forge/win-64/python-3.8.17-h4de0772_0_cpython.conda#be2296eaf70eeb1cb83c4e95136e694a
-https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.4-h0e60522_1.tar.bz2#e1aff0583dda5fb917eb3d2c1025aa80
+https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
+https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_8.tar.bz2#37157d273eaf3bc7d6862104161d9ec9
+https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.4-hd57cbcb_0.conda#195236e2eeb3b108e3b8eee47ad074fd
+https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
+https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2#24632c09ed931af617fe6d5292919cab
+https://conda.anaconda.org/conda-forge/osx-64/libuv-1.44.2-hac89ed1_0.tar.bz2#958fa9add5701462a6c91e3774425ea1
+https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-hfd90126_4.tar.bz2#35eb3fce8d51ed3c1fd4122bad48250b
+https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.3-h96cf925_1.tar.bz2#76217ebfbb163ff2770a261f955a5861
+https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.8-3_cp38.conda#ff192f59f7fe23555612030493a079f8
+https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
+https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
+https://conda.anaconda.org/conda-forge/osx-64/firefox-113.0-he965462_0.conda#6730ed9d9f8ff58391adf5fe00c984c4
+https://conda.anaconda.org/conda-forge/osx-64/geckodriver-0.33.0-hf46a32e_0.conda#897200360380560ac85cf0756161dd78
+https://conda.anaconda.org/conda-forge/osx-64/icu-70.1-h96cf925_0.tar.bz2#376635049e9b9b0bb875efd39dcd7b3b
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_8.tar.bz2#7f952a036d9014b4dab96c6ea0f8c2a7
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_8.tar.bz2#b36a3bfe866d9127f25f286506982166
+https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
+https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
+https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
+https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
+https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
+https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-hfd90126_4.tar.bz2#be90e6223c74ea253080abae19b3bdb1
+https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_8.tar.bz2#aac5ad0d8f747ef7f871508146df75d9
+https://conda.anaconda.org/conda-forge/osx-64/nodejs-18.15.0-hd0c9b3c_0.conda#4c7eb1947ecaa10394cf1cbcca343131
+https://conda.anaconda.org/conda-forge/osx-64/python-3.8.16-hf9b03c3_1_cpython.conda#96d23d997c18a90efde924d9ca6dd5b3
+https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
 https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-https://conda.anaconda.org/conda-forge/win-64/brotli-python-1.0.9-py38hd3f51b4_9.conda#b451fb48b1337ceb34b7b39de0bc09c8
+https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_8.tar.bz2#55f612fe4a9b5f6ac76348b6de94aaeb
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
 https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
-https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
-https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.7-py38hd3f51b4_0.conda#de2533e0a4ad84a4e5c5d6ad196f8e14
+https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.7-py38h4cd09af_0.conda#32626ffd5cd7eaad3036d7dca808ddc7
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
-https://conda.anaconda.org/conda-forge/win-64/docutils-0.20.1-py38haa244fe_0.conda#8f4292bb1a13ed095a725c137843da5f
+https://conda.anaconda.org/conda-forge/osx-64/docutils-0.20.1-py38h50d1736_0.conda#5722ca19ba9d5601032fd4dd5262b12a
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
-https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
-https://conda.anaconda.org/conda-forge/noarch/json5-0.9.14-pyhd8ed1ab_0.conda#dac1dabba2b5a9d1aee175c5fcc7b436
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
-https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.3-py38h91455d4_0.conda#a674b0be89418013ffa8f92c89d08640
-https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
-https://conda.anaconda.org/conda-forge/noarch/natsort-8.4.0-pyhd8ed1ab_0.conda#70959cd1db3cf77b2a27a0836cfd08a7
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.2-py38hef030d1_0.conda#011ae40b08362bc2b0b549f4fc0bd79f
+https://conda.anaconda.org/conda-forge/noarch/mistune-2.0.5-pyhd8ed1ab_0.conda#61a07195cfc935f1c1901d8ecf4af441
+https://conda.anaconda.org/conda-forge/noarch/natsort-8.3.1-pyhd8ed1ab_0.conda#8c53149aa69bfeb045f28c92a2b2ddc7
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda#02153b6b760bbec00cfe9e4c97993d06
-https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.5-py38h91455d4_0.conda#091a6bc808bfd07c97be1eb316440070
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
+https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.5-py38hef030d1_0.conda#20b4cc7adae881327b943c883be6335e
+https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
+https://conda.anaconda.org/conda-forge/osx-64/pyrsistent-0.19.3-py38hef030d1_0.conda#01ca11f08679d88fc881a19902a0a008
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
-https://conda.anaconda.org/conda-forge/win-64/pywin32-304-py38hd3f51b4_2.tar.bz2#cfefffaad808b61f2932f64c079417b8
-https://conda.anaconda.org/conda-forge/win-64/pywinpty-2.0.11-py38hd3f51b4_0.conda#6d7d5d94ab48044490f8934923074ba2
-https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py38h91455d4_5.tar.bz2#f62ab7e18711e3cbc068319448ecf771
-https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.0-py38ha85f68a_0.conda#5e97b9e91fc8cb7ec32647d5bec74030
+https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py38hef030d1_5.tar.bz2#e27d698dc29c6d5b49f1385bcd1d50f9
+https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.0-py38h3b70857_0.conda#a48761bc98b3bc22d209e9bb2f3dc5c1
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/noarch/robotframework-5.0.1-pyhd8ed1ab_0.tar.bz2#325df82f1bdd5175bb7b16d0c96e7d5e
-https://conda.anaconda.org/conda-forge/win-64/rpds-py-0.9.2-py38h4900a04_0.conda#222e659fb9e09325b23979c70c87784b
-https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
-https://conda.anaconda.org/conda-forge/win-64/tornado-6.3.2-py38h91455d4_0.conda#3e625e06e8892112acb47695eaf22b47
+https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py38hcafd530_0.conda#afefcf665a5049b030efb084a51e3935
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
-https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
-https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
-https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.1-pyhd8ed1ab_0.conda#7b517e7a6f0790337906c055aa97ca49
-https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.3-pyhd8ed1ab_0.conda#a3d2d43b74e042567cc4b5e328534885
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.2-pyhd8ed1ab_0.conda#bfe7e7cd1476092f51efbcde15dfb110
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
+https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.2-pyhd8ed1ab_0.conda#41221f97a0c82e5a60b21716a3d7469c
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
-https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py38h57701bc_3.conda#9b94af390cfdf924a063302a2ddb3860
+https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py38hb368cf1_3.conda#a2b3ae2a1fd2aea0b4433d9e7fff8cf3
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
-https://conda.anaconda.org/conda-forge/win-64/coverage-7.2.7-py38h91455d4_0.conda#2fa3faef0a7b6a5da2bff0faddbfbc68
+https://conda.anaconda.org/conda-forge/osx-64/coverage-7.2.7-py38hcafd530_0.conda#868ae7c3c94b2fffbe28687a64646f53
 https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
 https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
 https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
-https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
-https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2#56cd9fe388baac0e90c7149cfac95b60
+https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
+https://conda.anaconda.org/conda-forge/osx-64/pyobjc-core-9.1.1-py38h8f2a8f7_0.conda#e8cdf74d4a128a7bdd574d6c06b3b994
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/noarch/referencing-0.30.0-pyhd8ed1ab_0.conda#13bf095e3ecd18999d65b4d3ac5b15d5
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-2.2.0-pyhd8ed1ab_0.tar.bz2#29a329f0b817038d27d7bdfb2ca04b5a
 https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
-https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh08f2357_0.conda#c00d32dfa733d381b6a1908d0d67e0d7
-https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.0-pyh08f2357_0.tar.bz2#0152a609d5748ed9887d195b1e61a6c9
+https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyhd1c38e8_0.conda#046120b71d8896cb7faef78bfdbfee1e
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
-https://conda.anaconda.org/conda-forge/win-64/argon2-cffi-bindings-21.2.0-py38h91455d4_3.tar.bz2#a262d1c7aaf5a93a02b33dd985c27831
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.2-pyhd8ed1ab_0.conda#81a763f3c64fe6d5f32e033b0325265d
+https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py38hef030d1_3.tar.bz2#fc1bc20add8eff07c367973bba25e8eb
 https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.7.1-pyhd8ed1ab_0.conda#7c27ea1bdbe520bb830dcadd59f55cbf
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
-https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.16.0-pyhd8ed1ab_0.conda#d5cef1ba9df784f3d4633134a5e23b4e
-https://conda.anaconda.org/conda-forge/win-64/trio-0.21.0-py38haa244fe_0.tar.bz2#0fe81ab845eea9441bc9a025d47577be
-https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.4-pyhd8ed1ab_0.conda#18badd8fa3648d1beb1fcc7f2e0f756e
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
+https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-9.1.1-py38h8f2a8f7_0.conda#eaea41f1de16d95ce4de1fdd1b4bb295
+https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.15.0-pyhd8ed1ab_0.conda#02e7912139fb64828d18d07c43dcbad0
+https://conda.anaconda.org/conda-forge/osx-64/trio-0.21.0-py38h50d1736_0.tar.bz2#1e91102a7512cb5094ebe9818a361376
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.18.4-pyhd8ed1ab_0.conda#7356151a32ebd9a20158d2f26d224bfa
-https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.3.1-py38haa244fe_0.conda#15542a4c949a848b768a9e3b8ce3dd30
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
-https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
 https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
-https://conda.anaconda.org/conda-forge/win-64/ipython-7.33.0-py38haa244fe_0.tar.bz2#1185ff9399904ccd14f2eadbbca1aeab
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
+https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.0-py38h50d1736_0.conda#c342b82641ef032fa8b256eb4f0a5649
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyhd1c38e8_0.conda#2657c3de5371c571aef6678afb4aaadd
+https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.2-pyhd8ed1ab_0.conda#4ec732d2264373773a5feaea477128a8
+https://conda.anaconda.org/conda-forge/osx-64/ipython-7.33.0-py38h50d1736_0.tar.bz2#3bba83a6f445cccddfa5076ddbdd9467
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
 https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh6817e22_0.conda#b5cd11cf19c739548e968c12e020c54d
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh736e0ef_0.conda#d5aa7d2cc9fe03f62cf6e7bcc8e1a8df
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
 https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-5.1.3-pyhd8ed1ab_0.tar.bz2#464fdfebe1a1ffb41b031d8bbfb6041f
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda#32dde1678bb003c90d4bc0c2dbd21814
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.4.0-pyhd8ed1ab_0.conda#4456e6030a8309bdad57569b0170b6a3
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
 https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.0-pyhd8ed1ab_0.conda#38589f4104d11f2a59ff01a9f4e3bfb3
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.22.1-pyhd8ed1ab_0.conda#fc7172a6742a7c3c4331ddd7ed463ffc
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.0.3-pyhd8ed1ab_0.conda#c861cae50ac4cbc6d573a947f67a2d0c
-https://conda.anaconda.org/conda-forge/noarch/notebook-7.0.0-pyhd8ed1ab_0.conda#a8aa205f2b275a786cf6e55bb60a2d1a
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.0.1-pyhd8ed1ab_0.conda#93cc832cb8e18caa52c7b36ea6ce7f3d
+https://conda.anaconda.org/conda-forge/label/notebook_beta/noarch/notebook-7.0.0b3-pyhb537eac_0.conda#a654d4b1443e5f3ac52d3a3dc1b19b17
```

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/pull_request_template.md` & `robotframework_jupyterlibrary-0.5.0a0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/.github/workflows/ci.yml` & `robotframework_jupyterlibrary-0.5.0a0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/CONTRIBUTING.md` & `robotframework_jupyterlibrary-0.5.0a0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/LICENSE` & `robotframework_jupyterlibrary-0.5.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/README.md` & `robotframework_jupyterlibrary-0.5.0a0/README.md`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/_scripts/atest.py` & `robotframework_jupyterlibrary-0.5.0a0/_scripts/atest.py`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/_scripts/combine.py` & `robotframework_jupyterlibrary-0.5.0a0/_scripts/combine.py`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/_scripts/lint.py` & `robotframework_jupyterlibrary-0.5.0a0/_scripts/lint.py`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/_scripts/lock.py` & `robotframework_jupyterlibrary-0.5.0a0/_scripts/lock.py`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/_scripts/project.py` & `robotframework_jupyterlibrary-0.5.0a0/_scripts/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """project paths, files and utilities, used by `dodo.py` and `_scripts/`."""
 import contextlib
 import os
 import platform
 import shutil
-import subprocess
 import sys
 from pathlib import Path
 
 try:
     import tomllib
 except ImportError:
     import tomli as tomllib
@@ -270,16 +269,14 @@
 ROBOCOP_ARGS = [
     "robocop",
     *("--configure", "empty-lines-between-sections:empty_lines:2"),
     *("--exclude", "deprecated-statement"),
     *("--exclude", "deprecated-with-name"),
     *("--exclude", "if-can-be-used"),
     *("--exclude", "too-many-calls-in-keyword"),
-    *("--exclude", "unnecessary-string-conversion"),
-    *("--exclude", "unused-variable"),
 ]
 
 
 class OK:
     ok = BUILD / "ok"
     atest = ok / "atest.txt"
     ssort = ok / "ssort.txt"
@@ -360,15 +357,7 @@
 
 def get_ok_actions(p: Path):
     """Create a pair of doit `actions` for working with a canary/ok file."""
     return [
         lambda: p.unlink() if p.exists() else None,
         lambda: [p.parent.mkdir(exist_ok=True, parents=True), p.touch(), None][-1],
     ]
-
-
-def get_source_date_epoch():
-    """Get the SOURCE_DATE_EPOCH from git."""
-    return subprocess.check_output(
-        ["git", "log", "-1", "--format=%ct"],
-        encoding="utf-8",
-    ).strip()
```

### Comparing `robotframework_jupyterlibrary-0.5.0/_scripts/reporter.py` & `robotframework_jupyterlibrary-0.5.0a0/_scripts/reporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from datetime import datetime
-from typing import ClassVar, Dict, List
 
 from doit.reporter import ConsoleReporter
 
 from . import project as P
 
 START = "::group::" if P.CI else ""
 END = "::endgroup::" if P.CI else ""
 
 TIMEFMT = "%H:%M:%S"
 SKIP = "--------"
 
 
 class GithubActionsReporter(ConsoleReporter):
-    _gh_timings: ClassVar[Dict[str, List[datetime]]] = {}
+    _gh_timings = {}
 
     def skip_uptodate(self, task):
         self.outstream.write(f"{START}[{SKIP}] ⏩  {task.title()}{END}\n")
 
     skip_ignore = skip_uptodate
 
     def execute_task(self, task):
```

### Comparing `robotframework_jupyterlibrary-0.5.0/atest/01_server/00_basic.robot` & `robotframework_jupyterlibrary-0.5.0a0/atest/01_server/00_basic.robot`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/atest/__init__.robot` & `robotframework_jupyterlibrary-0.5.0a0/atest/__init__.robot`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/atest/classic/10_notebook.robot` & `robotframework_jupyterlibrary-0.5.0a0/atest/classic/10_notebook.robot`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/atest/lab/00_shell.robot` & `robotframework_jupyterlibrary-0.5.0a0/atest/lab/00_shell.robot`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/atest/lab/10_notebook.robot` & `robotframework_jupyterlibrary-0.5.0a0/atest/lab/10_notebook.robot`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/atest/lab/20_magic.robot` & `robotframework_jupyterlibrary-0.5.0a0/atest/lab/20_magic.robot`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/atest/lab/30_settings.robot` & `robotframework_jupyterlibrary-0.5.0a0/atest/lab/30_settings.robot`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/atest/lab/__init__.robot` & `robotframework_jupyterlibrary-0.5.0a0/atest/lab/__init__.robot`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/atest/notebook/10_notebook.robot` & `robotframework_jupyterlibrary-0.5.0a0/atest/notebook/10_notebook.robot`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/docs/CI.ipynb` & `robotframework_jupyterlibrary-0.5.0a0/docs/CI.ipynb`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/docs/HISTORY.ipynb` & `robotframework_jupyterlibrary-0.5.0a0/docs/HISTORY.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9886363636363636%*

 * *Differences: {"'cells'": '{delete: [1]}'}*

```diff
@@ -7,30 +7,14 @@
                 "# HISTORY"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## 0.5.0\n",
-                "\n",
-                "| Products under test         | Versions              |\n",
-                "|-----------------------------|-----------------------|\n",
-                "| Python                      | `3.8.17`<br/>`3.11.4` |\n",
-                "| CodeMirror                  | `5`<br/>`6`           |\n",
-                "| Robot Framework             | `5.0.1`<br/>`6.1.0`   |\n",
-                "| Jupyter Notebook            | `6.5.4`<br/>`7.0.0`   |\n",
-                "| JupyterLab                  | `3.6.5`<br/>`4.0.3`   |\n",
-                "| Jupyter Server              | `2.7.0`               |"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
                 "## 0.5.0a0\n",
                 "\n",
                 "| Products under test         | Versions              |\n",
                 "|-----------------------------|-----------------------|\n",
                 "| Python                      | `3.8.16`<br/>`3.11.3` |\n",
                 "| CodeMirror                  | `5`<br/>`6`           |\n",
                 "| Robot Framework             | `5.0.1`<br/>`6.0.2`   |\n",
```

### Comparing `robotframework_jupyterlibrary-0.5.0/docs/INSTALL.ipynb` & `robotframework_jupyterlibrary-0.5.0a0/docs/INSTALL.ipynb`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/docs/KEYWORDS.ipynb` & `robotframework_jupyterlibrary-0.5.0a0/docs/KEYWORDS.ipynb`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/docs/LIMITS.ipynb` & `robotframework_jupyterlibrary-0.5.0a0/docs/LIMITS.ipynb`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/docs/MAGIC.ipynb` & `robotframework_jupyterlibrary-0.5.0a0/docs/MAGIC.ipynb`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/docs/WHY.ipynb` & `robotframework_jupyterlibrary-0.5.0a0/docs/WHY.ipynb`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/docs/_static/anvil.svg` & `robotframework_jupyterlibrary-0.5.0a0/docs/_static/anvil.svg`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/docs/_static/css/custom.css` & `robotframework_jupyterlibrary-0.5.0a0/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/docs/_static/fonts/OCRA.woff2` & `robotframework_jupyterlibrary-0.5.0a0/docs/_static/fonts/OCRA.woff2`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/docs/conf.py` & `robotframework_jupyterlibrary-0.5.0a0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/docs/index.ipynb` & `robotframework_jupyterlibrary-0.5.0a0/docs/index.ipynb`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/docs/rtd.yml` & `robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/osx-64/py3.11/lab4/conda.lock`

 * *Files 15% similar despite different names*

```diff
@@ -1,152 +1,156 @@
-# Probably don't edit by hand!
-#
-# This was generated from .github/locks/docs/linux-64/conda.lock
-#
-#   doit docs:rtd:env
-#
-channels:
-  - conda-forge
-  - nodefaults
-dependencies:
-  - https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
-  - https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
-  - https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
-  - https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.1.0-hfd8a6a1_0.conda#067bcc23164642f4c226da631f2a2e1d
-  - https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.11-3_cp311.conda#c2e2630ddb68cf52eec74dc7dfab20b5
-  - https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
-  - https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
-  - https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
-  - https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
-  - https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
-  - https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
-  - https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
-  - https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
-  - https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
-  - https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
-  - https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
-  - https://conda.anaconda.org/conda-forge/linux-64/libuv-1.44.2-h166bdaf_0.tar.bz2#e5cb4fe581a18ca2185a016eb848fc00
-  - https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
-  - https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
-  - https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
-  - https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
-  - https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
-  - https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
-  - https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
-  - https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
-  - https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
-  - https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
-  - https://conda.anaconda.org/conda-forge/linux-64/nodejs-18.16.1-hf52ce11_0.conda#23ed78db48ed08c94e5449f6661d65e6
-  - https://conda.anaconda.org/conda-forge/linux-64/python-3.11.4-hab00c5b_0_cpython.conda#1c628861a2a126b9fc9363ca1b7d014e
-  - https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
-  - https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
-  - https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
-  - https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
-  - https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.0.9-py311ha362b79_9.conda#ced5340f5dc6cff43a80deac8d0e398f
-  - https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-  - https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
-  - https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-unix_pyh707e725_0.conda#64dbb3b205546691a61204d1cfb208e3
-  - https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
-  - https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
-  - https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py311hcafe171_0.conda#f4c810ad9d791c8df5ad900ed74b085b
-  - https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
-  - https://conda.anaconda.org/conda-forge/linux-64/docutils-0.19-py311h38be061_1.tar.bz2#599159b0740e9b82e7eef0e8471be3c2
-  - https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
-  - https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
-  - https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
-  - https://conda.anaconda.org/conda-forge/linux-64/greenlet-2.0.2-py311hb755f60_1.conda#82f9885f18cc7ba9bca6687ac97f1d65
-  - https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
-  - https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
-  - https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py311h459d7ec_0.conda#9904dc4adb5d547cb21e136f98cb24b0
-  - https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
-  - https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
-  - https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
-  - https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
-  - https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
-  - https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-  - https://conda.anaconda.org/conda-forge/noarch/port-for-0.7.1-pyhd8ed1ab_0.conda#911d5daac0d579dc7aa4d85050ccd548
-  - https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py311h2582759_0.conda#a90f8e278c1cd7064b2713e6b7db87e6
-  - https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
-  - https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
-  - https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
-  - https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
-  - https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
-  - https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
-  - https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py311hd4cff14_5.tar.bz2#da8769492e423103c59f469f4f17f8d9
-  - https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py311h75c88c4_0.conda#db94a7a9e865fbfde8c023b6e8958bb2
-  - https://conda.anaconda.org/conda-forge/noarch/robotframework-6.1-pyhd8ed1ab_0.conda#e383bebdc0d8fea4ecf9c9e01d0959fe
-  - https://conda.anaconda.org/conda-forge/linux-64/rpds-py-0.9.2-py311h46250e7_0.conda#bcf66b5abaec47198b42cdd0bb968540
-  - https://conda.anaconda.org/conda-forge/noarch/setuptools-68.0.0-pyhd8ed1ab_0.conda#5a7739d0f57ee64133c9d32e6507c46d
-  - https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
-  - https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
-  - https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
-  - https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
-  - https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
-  - https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.4-pyhd8ed1ab_0.conda#5a31a7d564f551d0e6dff52fd8cb5b16
-  - https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
-  - https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.1-pyhd8ed1ab_0.conda#6c8c4d6eb2325e59290ac6dbbeacd5f0
-  - https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
-  - https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
-  - https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
-  - https://conda.anaconda.org/conda-forge/noarch/tabulate-0.9.0-pyhd8ed1ab_1.tar.bz2#4759805cce2d914c38472f70bf4d8bcb
-  - https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
-  - https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
-  - https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py311h459d7ec_0.conda#12b1c374ee90a1aa11ea921858394dc8
-  - https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-  - https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
-  - https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
-  - https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
-  - https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
-  - https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
-  - https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
-  - https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
-  - https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
-  - https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
-  - https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
-  - https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
-  - https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
-  - https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
-  - https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
-  - https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
-  - https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
-  - https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
-  - https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
-  - https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
-  - https://conda.anaconda.org/conda-forge/noarch/pip-23.2-pyhd8ed1ab_0.conda#fb90dfe13ce16c0a3374e3d34e3291c5
-  - https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-  - https://conda.anaconda.org/conda-forge/noarch/referencing-0.30.0-pyhd8ed1ab_0.conda#13bf095e3ecd18999d65b4d3ac5b15d5
-  - https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.2.0-pyhd8ed1ab_0.conda#c9e9064ab45ffb46f7a96834d9e7626d
-  - https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
-  - https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.4-pyhd8ed1ab_0.conda#18badd8fa3648d1beb1fcc7f2e0f756e
-  - https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
-  - https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
-  - https://conda.anaconda.org/conda-forge/noarch/jsonschema-specifications-2023.7.1-pyhd8ed1ab_0.conda#7c27ea1bdbe520bb830dcadd59f55cbf
-  - https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.3.5-pyhd8ed1ab_0.conda#9eeb66a24c8f6d950eb55a9f1128da20
-  - https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
-  - https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
-  - https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-2.0.19-py311h459d7ec_0.conda#9970b757e599b1b845fedd25c8d6fc7a
-  - https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
-  - https://conda.anaconda.org/conda-forge/linux-64/trio-0.22.2-py311h38be061_0.conda#dcbfe3a95e8b99ec743e26a75d8c9cf4
-  - https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
-  - https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
-  - https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
-  - https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
-  - https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.18.4-pyhd8ed1ab_0.conda#7356151a32ebd9a20158d2f26d224bfa
-  - https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.1-py311h38be061_0.conda#0cf8259b01ede82c76007996f73f89ed
-  - https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
-  - https://conda.anaconda.org/conda-forge/noarch/sphinx-5.3.0-pyhd8ed1ab_0.tar.bz2#f9e1fcfe235d655900bfeb6aee426472
-  - https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.3-pyhd8ed1ab_0.conda#51338d1133d8fed41796a581e974b22d
-  - https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
-  - https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
-  - https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
-  - https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
-  - https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
-  - https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
-  - https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2021.3.14-pyhd8ed1ab_0.tar.bz2#1909f784dc37b4ab97afe2c95aeeabaa
-  - https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
-  - https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh41d4057_0.conda#0a0b0d8177c4a209017b356439292db8
-  - https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda#f7aa15f77d29b11caa1df1eb15383c59
-  - https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_1.conda#108e78e654611c3a35890ceee3b354fa
-  - https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.24.0-pyh71e2992_0.conda#cfafc9387c32a43a1b6d63633489cbc9
-  - https://conda.anaconda.org/conda-forge/noarch/jupyter-cache-0.6.1-pyhd8ed1ab_0.conda#2e360820ae68e3d28e1a5a9d2714ca5c
-  - https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda#40190b7d06f86b63d28fa78aaa39c023
-name: rtd
+@EXPLICIT
+https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
+https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_8.tar.bz2#37157d273eaf3bc7d6862104161d9ec9
+https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.4-hd57cbcb_0.conda#195236e2eeb3b108e3b8eee47ad074fd
+https://conda.anaconda.org/conda-forge/osx-64/libexpat-2.5.0-hf0c8a7f_1.conda#6c81cb022780ee33435cca0127dd43c9
+https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
+https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2#24632c09ed931af617fe6d5292919cab
+https://conda.anaconda.org/conda-forge/osx-64/libuv-1.44.2-hac89ed1_0.tar.bz2#958fa9add5701462a6c91e3774425ea1
+https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-hfd90126_4.tar.bz2#35eb3fce8d51ed3c1fd4122bad48250b
+https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.3-h96cf925_1.tar.bz2#76217ebfbb163ff2770a261f955a5861
+https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.11-3_cp311.conda#5e0a069a585445333868d2c6651c3b3f
+https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
+https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
+https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
+https://conda.anaconda.org/conda-forge/osx-64/firefox-113.0-he965462_0.conda#6730ed9d9f8ff58391adf5fe00c984c4
+https://conda.anaconda.org/conda-forge/osx-64/geckodriver-0.33.0-hf46a32e_0.conda#897200360380560ac85cf0756161dd78
+https://conda.anaconda.org/conda-forge/osx-64/icu-70.1-h96cf925_0.tar.bz2#376635049e9b9b0bb875efd39dcd7b3b
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_8.tar.bz2#7f952a036d9014b4dab96c6ea0f8c2a7
+https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_8.tar.bz2#b36a3bfe866d9127f25f286506982166
+https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
+https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
+https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
+https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
+https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
+https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-hfd90126_4.tar.bz2#be90e6223c74ea253080abae19b3bdb1
+https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_8.tar.bz2#aac5ad0d8f747ef7f871508146df75d9
+https://conda.anaconda.org/conda-forge/osx-64/nodejs-18.15.0-hd0c9b3c_0.conda#4c7eb1947ecaa10394cf1cbcca343131
+https://conda.anaconda.org/conda-forge/osx-64/python-3.11.3-h99528f9_0_cpython.conda#c3291f9411424fc587d53a2ea57fb075
+https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
+https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
+https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
+https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
+https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
+https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_8.tar.bz2#55f612fe4a9b5f6ac76348b6de94aaeb
+https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
+https://conda.anaconda.org/conda-forge/noarch/cloudpickle-2.2.1-pyhd8ed1ab_0.conda#b325bfc4cff7d7f8a868f1f7ecc4ed16
+https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.7-py311h814d153_0.conda#c27802860b87fe024c9b6276205a56b5
+https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
+https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
+https://conda.anaconda.org/conda-forge/osx-64/docutils-0.20.1-py311h6eed73b_0.conda#0536cbe889e20101b7f8e6d6b1dbcbf4
+https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
+https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
+https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
+https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.2-py311h5547dcb_0.conda#13091519d55d667506aaf413cffaff10
+https://conda.anaconda.org/conda-forge/noarch/mistune-2.0.5-pyhd8ed1ab_0.conda#61a07195cfc935f1c1901d8ecf4af441
+https://conda.anaconda.org/conda-forge/noarch/natsort-8.3.1-pyhd8ed1ab_0.conda#8c53149aa69bfeb045f28c92a2b2ddc7
+https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
+https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
+https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
+https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
+https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
+https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
+https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.5-py311h5547dcb_0.conda#d9b4565309f4f992b42bd99031044642
+https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
+https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
+https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
+https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
+https://conda.anaconda.org/conda-forge/osx-64/pyrsistent-0.19.3-py311h5547dcb_0.conda#f114c0dab9f9c894b260297371124634
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
+https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
+https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
+https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
+https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py311h5547dcb_5.tar.bz2#8d1e456914ce961119b07f396187a564
+https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.0-py311h5dacc12_0.conda#1f65b37886e7cb8476d48ea8bb9d19c0
+https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
+https://conda.anaconda.org/conda-forge/noarch/robotframework-6.0.2-pyhd8ed1ab_1.conda#b4dcead8c5a99a14733d9b1ba5b7db09
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
+https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
+https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
+https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
+https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
+https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
+https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2#73506d1ab4202481841c68c169b7ef6c
+https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py311h2725bcf_0.conda#276fe4341e39dcd9d9d33ca18140d2e7
+https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.2-pyha770c72_0.conda#5a4a270e5a3f93846d6bade2f71fa440
+https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
+https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.2-pyhd8ed1ab_0.conda#bfe7e7cd1476092f51efbcde15dfb110
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.1-pyhd8ed1ab_1.tar.bz2#d65ef75084f8adbadb696dfd91148e79
+https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
+https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.2-pyhd8ed1ab_0.conda#41221f97a0c82e5a60b21716a3d7469c
+https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
+https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
+https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
+https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
+https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py311ha86e640_3.conda#5967be4da33261eada7cc79593f71088
+https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
+https://conda.anaconda.org/conda-forge/osx-64/coverage-7.2.7-py311h2725bcf_0.conda#afba3a3f74c5f71ebd9f400871e8c4de
+https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2#b21ed0883505ba1910994f1df031a428
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
+https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
+https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
+https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
+https://conda.anaconda.org/conda-forge/noarch/outcome-1.2.0-pyhd8ed1ab_0.tar.bz2#3dbb9ece72652131f12d66e889da7c0a
+https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
+https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
+https://conda.anaconda.org/conda-forge/osx-64/pyobjc-core-9.1.1-py311hfd07503_0.conda#ba333461302daaea2dfce2d5223c876e
+https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
+https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pythonlibcore-4.1.2-pyhd8ed1ab_0.conda#3af043636b92ad0317a234544b30a4a8
+https://conda.anaconda.org/conda-forge/noarch/robotframework-stacktrace-0.4.1-pyhd8ed1ab_0.tar.bz2#3dc788e294fd159537c931dbb964511e
+https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyhd1c38e8_0.conda#046120b71d8896cb7faef78bfdbfee1e
+https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.2-hd8ed1ab_0.conda#f676553904bb8f7c1dfe71c9db0d9ba7
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.2-pyhd8ed1ab_0.conda#81a763f3c64fe6d5f32e033b0325265d
+https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py311h5547dcb_3.tar.bz2#c09459e349fa61afc352f473766de109
+https://conda.anaconda.org/conda-forge/noarch/doit-0.36.0-pyhd8ed1ab_0.tar.bz2#fc5e53d070f1ee7bb38c2ece282dcb82
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
+https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-9.1.1-py311hfd07503_0.conda#d8c5226abc26b750ebdc5d40d00e7b35
+https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
+https://conda.anaconda.org/conda-forge/noarch/robotframework-pabot-2.15.0-pyhd8ed1ab_0.conda#02e7912139fb64828d18d07c43dcbad0
+https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
+https://conda.anaconda.org/conda-forge/osx-64/trio-0.22.0-py311h6eed73b_1.tar.bz2#71a739c4b0b1e17cfd27cfdf828d52a8
+https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
+https://conda.anaconda.org/conda-forge/noarch/wsproto-1.2.0-pyhd8ed1ab_0.tar.bz2#00ba804b54f451d102f6a7615f08470d
+https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
+https://conda.anaconda.org/conda-forge/noarch/doit-with-toml-0.36.0-pyhd8ed1ab_0.tar.bz2#593faaa546937cfa071928c9127fcb12
+https://conda.anaconda.org/conda-forge/noarch/flit-3.9.0-pyhd8ed1ab_0.conda#269513333bb3c273108404b7e618d827
+https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.0-py311h6eed73b_0.conda#e0e5cfb36ece6eae9c355eed1e90ff9d
+https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyhd1c38e8_0.conda#2657c3de5371c571aef6678afb4aaadd
+https://conda.anaconda.org/conda-forge/noarch/trio-websocket-0.10.2-pyhd8ed1ab_0.conda#4ec732d2264373773a5feaea477128a8
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/selenium-4.9.1-pyhd8ed1ab_0.conda#b3daee1b09922328cfa11b4761cf1adf
+https://conda.anaconda.org/conda-forge/noarch/ipython-8.13.2-pyhd1c38e8_0.conda#30960117dd6bd242aec8428a1004b167
+https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
+https://conda.anaconda.org/conda-forge/noarch/robotframework-seleniumlibrary-6.1.0-pyhd8ed1ab_0.conda#15700afca8f7ab35542e9c1af63568f1
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh736e0ef_0.conda#d5aa7d2cc9fe03f62cf6e7bcc8e1a8df
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.4.0-pyhd8ed1ab_0.conda#4456e6030a8309bdad57569b0170b6a3
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
+https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.0-pyhd8ed1ab_0.conda#38589f4104d11f2a59ff01a9f4e3bfb3
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.22.1-pyhd8ed1ab_0.conda#fc7172a6742a7c3c4331ddd7ed463ffc
+https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.0.1-pyhd8ed1ab_0.conda#93cc832cb8e18caa52c7b36ea6ce7f3d
+https://conda.anaconda.org/conda-forge/label/notebook_beta/noarch/notebook-7.0.0b3-pyhb537eac_0.conda#a654d4b1443e5f3ac52d3a3dc1b19b17
```

### Comparing `robotframework_jupyterlibrary-0.5.0/dodo.py` & `robotframework_jupyterlibrary-0.5.0a0/dodo.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,23 +56,18 @@
 
 def task_build():
     """Build packages."""
     env = "meta"
     env_lock = P.CONDA_LISTS[env]
     run_in = P.RUN_IN[env]
 
-    def _flit_build():
-        env = dict(os.environ, SOURCE_DATE_EPOCH=P.get_source_date_epoch())
-        rc = subprocess.call([*run_in, "flit", "--debug", "build"], env=env)
-        return rc == 0
-
     yield {
         "name": "pypi",
         "doc": "build the pypi sdist/wheel",
-        "actions": [_flit_build],
+        "actions": [[*run_in, "flit", "build"]],
         "targets": [P.SDIST, P.WHEEL],
         "file_dep": [*P.PY_SRC, *P.ROBOT_SRC, *P.SETUP_CRUFT, env_lock],
     }
 
     def _update_hash():
         # mimic sha256sum CLI
         if P.SHA256SUMS.exists():
```

### Comparing `robotframework_jupyterlibrary-0.5.0/pyproject.toml` & `robotframework_jupyterlibrary-0.5.0a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = ["flit_core >=3.9,<4"]
 
 [tool.flit.module]
 name = "JupyterLibrary"
 
 [project]
 name = "robotframework-jupyterlibrary"
-version = "0.5.0"
+version = "0.5.0a0"
 description = "A Robot Framework library for automating (testing of) Jupyter end-user applications and extensions."
 readme = "README.md"
 authors = [{name = "JupyterLibrary contributors", email = "robots-from-jupyter@googlegroups.com"}]
 requires-python = ">=3.8"
 classifiers = [
     "Framework :: Jupyter",
     "Framework :: Jupyter :: JupyterLab",
```

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/classic/Commands.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/notebook/Commands.resource`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 *** Settings ***
-Documentation       Command keywords for Jupyter Classic
+Documentation       Command keywords for Jupyter Notebook
 
-Resource            JupyterLibrary/clients/classic/Selectors.resource
+Resource            JupyterLibrary/clients/notebook/Selectors.resource
 
 
 *** Keywords ***
-Execute Notebook Classic Command
-    [Documentation]    Use the Notebook Classic Command Pop-up
+Execute Notebook Command
+    [Documentation]    Use the Jupyter Notebook Command Pop-up
     ...    to run a command and ``accept`` any resulting dialogs, then ``close``
     ...    the Command Palette.
-    [Arguments]    ${command}
-    Click Element    css:${JNC CSS CMD BUTTON}
-    Input Text    css:${JNC CSS CMD INPUT}    ${command}
-    Click Element    css:${JNC CSS CMD ITEM}
+    [Arguments]    ${command}    ${accept}=${True}    ${close}=${True}
+    Click Element    css:${JNB CSS CMD BUTTON}
+    Input Text    css:${JNB CSS CMD INPUT}    ${command}
+    Click Element    css:${JNB CSS CMD ITEM}
```

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/classic/Notebook.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/classic/Notebook.resource`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/classic/Output.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/classic/Output.resource`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/classic/Selectors.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/classic/Selectors.resource`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/classic/Tree.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/classic/Tree.resource`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Commands.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Commands.resource`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Icons.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Icons.resource`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Launcher.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Launcher.resource`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Notebook.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Notebook.resource`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Output.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Output.resource`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/PageInfo.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/PageInfo.resource`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Selectors.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Selectors.resource`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Settings.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Settings.resource`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Shell.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Shell.resource`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Shortcuts.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Shortcuts.resource`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Sidebar.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Sidebar.resource`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/jupyterlab/Version.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Version.resource`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/notebook/Notebook.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/notebook/Notebook.resource`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/notebook/Output.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/notebook/Output.resource`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/notebook/Selectors.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/notebook/Selectors.resource`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 *** Variables ***
 # imports from jupyterlab
 ${JNB CSS CELL}                         ${JLAB CSS CELL}
 ${JNB CSS ACCEPT}                       ${JLAB CSS MOD ACCEPT}
 
 # css selectors
-${JNB CSS TREE}                         .jp-DirListing
 ${JNB CSS TREE LIST}                    .jp-DirListing-content
 ${JNB CSS TREE LIST ITEM}               ${JNB CSS TREE LIST} .jp-DirListing-item
 ${JNB CSS TREE NEW MENU}                ${LM CSS MENU}
 ${JNB CSS TREE NEW NOTEBOOK}            ${JNB CSS TREE NEW MENU} li[data-command="notebook:create-new"]
 ${JNB CSS TREE MENU ITEM LABEL}         ${LM CSS MENU ITEM LABEL}
 ${JNB CSS KERNEL DIALOG SELECT}         .jp-Dialog select
 ${JNB CSS NB KERNEL BUSY}               .kernel_budy_icon
```

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/clients/notebook/Tree.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/notebook/Tree.resource`

 * *Files 10% similar despite different names*

```diff
@@ -14,16 +14,15 @@
     ...    Extra ``configuration`` is passed on to SeleniumLibrary's *Open Browser*.
     [Arguments]    ${browser}=headlessfirefox    ${nbserver}=${None}    ${url}=${EMPTY}    &{configuration}
     ${nbserver_url} =    Run Keyword If    not "${url}"    Get Jupyter Server URL    ${nbserver}
     ${token} =    Run Keyword If    not "${url}"    Get Jupyter Server Token    ${nbserver}
     ${final_url} =    Set Variable If    "${url}"    ${url}    ${nbserver_url}tree?token=${token}
     Open Browser    url=${final_url}    browser=${browser}    &{configuration}
     Update Globals For JupyterLab 4
-    Wait Until Element Is Visible    css:${JNB CSS TREE}
-    Wait Until Element Is Visible    css:${JNB CSS TREE LIST}    timeout=10s
+    Wait Until Element Is Visible    css:${JNB CSS TREE LIST}
 
 Launch A New Notebook
     [Documentation]    Use the Jupyter Notebook tree to launch a Notebook with the
     ...    given ``kernel``
     [Arguments]    ${kernel}=Python 3 (ipykernel)
     Click Element    xpath:${JNB XP TREE NEW BUTTON}
     Wait Until Element Is Visible    css:${JNB CSS TREE NEW MENU}
```

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/common/CodeMirror.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/common/CodeMirror.resource`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/core.py` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/core.py`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/keywords/server.py` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/keywords/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,32 +14,22 @@
 from SeleniumLibrary.base import LibraryComponent, keyword
 
 
 class ServerKeywords(LibraryComponent):
 
     """A component that extends the core with Jupyter server management."""
 
-    _handles: typing.List[subprocess.Popen]
-    _tmpdirs: typing.Dict[subprocess.Popen, str]
-    _notebook_dirs: typing.Dict[subprocess.Popen, str]
-    _ports: typing.Dict[subprocess.Popen, int]
-    _base_urls: typing.Dict[subprocess.Popen, str]
-    _tokens: typing.Dict[subprocess.Popen, str]
-    _app_name: typing.Optional[str]
-
-    def __init__(self, *args, **kwargs):
-        """Initialize a library with jupyter server keywords."""
-        super().__init__(*args, **kwargs)
-        self._handles = []
-        self._tmpdirs = {}
-        self._notebook_dirs = {}
-        self._ports = {}
-        self._base_urls = {}
-        self._tokens = {}
-        self._app_name = None
+    _handles: typing.List[subprocess.Popen] = []
+    _tmpdirs: typing.Dict[subprocess.Popen, str] = {}
+    _notebook_dirs: typing.Dict[subprocess.Popen, str] = {}
+    _ports: typing.Dict[subprocess.Popen, int] = {}
+    _base_urls: typing.Dict[subprocess.Popen, str] = {}
+    _tokens: typing.Dict[subprocess.Popen, str] = {}
+
+    _app_name: typing.Optional[str] = None
 
     @keyword
     def set_default_jupyter_app_name(
         self,
         app_name: typing.Optional[str] = None,
     ) -> typing.Optional[str]:
         """Set the current ``traitlets.Configurable`` Jupyter Server application, returning the previous value.
```

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/keywords/webelements.py` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/keywords/webelements.py`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/src/JupyterLibrary/magic.py` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/magic.py`

 * *Files identical despite different names*

### Comparing `robotframework_jupyterlibrary-0.5.0/PKG-INFO` & `robotframework_jupyterlibrary-0.5.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-jupyterlibrary
-Version: 0.5.0
+Version: 0.5.0a0
 Summary: A Robot Framework library for automating (testing of) Jupyter end-user applications and extensions.
 Keywords: Interactive,Jupyter,notebook,Testing,Web
 Author-email: JupyterLibrary contributors <robots-from-jupyter@googlegroups.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
```

