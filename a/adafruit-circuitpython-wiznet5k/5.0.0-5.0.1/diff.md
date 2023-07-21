# Comparing `tmp/adafruit-circuitpython-wiznet5k-5.0.0.tar.gz` & `tmp/adafruit-circuitpython-wiznet5k-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-wiznet5k-5.0.0.tar", last modified: Fri Jul 21 22:24:25 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-wiznet5k-5.0.1.tar", last modified: Fri Jul 21 22:59:41 2023, max compression
```

## Comparing `adafruit-circuitpython-wiznet5k-5.0.0.tar` & `adafruit-circuitpython-wiznet5k-5.0.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:24:25.525205 adafruit-circuitpython-wiznet5k-5.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:24:25.513205 adafruit-circuitpython-wiznet5k-5.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:24:25.517205 adafruit-circuitpython-wiznet5k-5.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:24:25.517205 adafruit-circuitpython-wiznet5k-5.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:24:25.517205 adafruit-circuitpython-wiznet5k-5.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-07-21 22:24:25.525205 adafruit-circuitpython-wiznet5k-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:24:25.517205 adafruit-circuitpython-wiznet5k-5.0.0/adafruit_circuitpython_wiznet5k.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-07-21 22:24:25.000000 adafruit-circuitpython-wiznet5k-5.0.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-21 22:24:25.000000 adafruit-circuitpython-wiznet5k-5.0.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:24:25.000000 adafruit-circuitpython-wiznet5k-5.0.0/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-21 22:24:25.000000 adafruit-circuitpython-wiznet5k-5.0.0/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 22:24:25.000000 adafruit-circuitpython-wiznet5k-5.0.0/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:24:25.521205 adafruit-circuitpython-wiznet5k-5.0.0/adafruit_wiznet5k/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:24:14.000000 adafruit-circuitpython-wiznet5k-5.0.0/adafruit_wiznet5k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51695 2023-07-21 22:24:14.000000 adafruit-circuitpython-wiznet5k-5.0.0/adafruit_wiznet5k/adafruit_wiznet5k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-21 22:24:14.000000 adafruit-circuitpython-wiznet5k-5.0.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    25760 2023-07-21 22:24:14.000000 adafruit-circuitpython-wiznet5k-5.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-07-21 22:24:14.000000 adafruit-circuitpython-wiznet5k-5.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)    27015 2023-07-21 22:24:14.000000 adafruit-circuitpython-wiznet5k-5.0.0/adafruit_wiznet5k/adafruit_wiznet5k_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-21 22:24:14.000000 adafruit-circuitpython-wiznet5k-5.0.0/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:24:25.521205 adafruit-circuitpython-wiznet5k-5.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:24:25.521205 adafruit-circuitpython-wiznet5k-5.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:24:25.525205 adafruit-circuitpython-wiznet5k-5.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-21 22:24:14.000000 adafruit-circuitpython-wiznet5k-5.0.0/examples/wiznet5k_aio_post.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-07-21 22:24:14.000000 adafruit-circuitpython-wiznet5k-5.0.0/examples/wiznet5k_cheerlights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-07-21 22:24:14.000000 adafruit-circuitpython-wiznet5k-5.0.0/examples/wiznet5k_cpython_client_for_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-21 22:24:14.000000 adafruit-circuitpython-wiznet5k-5.0.0/examples/wiznet5k_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-21 22:24:14.000000 adafruit-circuitpython-wiznet5k-5.0.0/examples/wiznet5k_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-21 22:24:14.000000 adafruit-circuitpython-wiznet5k-5.0.0/examples/wiznet5k_simpletest_manual_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-21 22:24:14.000000 adafruit-circuitpython-wiznet5k-5.0.0/examples/wiznet5k_wsgiserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-21 22:24:14.000000 adafruit-circuitpython-wiznet5k-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-21 22:24:03.000000 adafruit-circuitpython-wiznet5k-5.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 22:24:25.525205 adafruit-circuitpython-wiznet5k-5.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:59:41.804372 adafruit-circuitpython-wiznet5k-5.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:59:41.788372 adafruit-circuitpython-wiznet5k-5.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:59:41.792372 adafruit-circuitpython-wiznet5k-5.0.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:59:41.796372 adafruit-circuitpython-wiznet5k-5.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:59:41.796372 adafruit-circuitpython-wiznet5k-5.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-07-21 22:59:41.804372 adafruit-circuitpython-wiznet5k-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:59:41.796372 adafruit-circuitpython-wiznet5k-5.0.1/adafruit_circuitpython_wiznet5k.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-07-21 22:59:41.000000 adafruit-circuitpython-wiznet5k-5.0.1/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-21 22:59:41.000000 adafruit-circuitpython-wiznet5k-5.0.1/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:59:41.000000 adafruit-circuitpython-wiznet5k-5.0.1/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-21 22:59:41.000000 adafruit-circuitpython-wiznet5k-5.0.1/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 22:59:41.000000 adafruit-circuitpython-wiznet5k-5.0.1/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:59:41.800372 adafruit-circuitpython-wiznet5k-5.0.1/adafruit_wiznet5k/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:59:33.000000 adafruit-circuitpython-wiznet5k-5.0.1/adafruit_wiznet5k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51695 2023-07-21 22:59:33.000000 adafruit-circuitpython-wiznet5k-5.0.1/adafruit_wiznet5k/adafruit_wiznet5k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-21 22:59:33.000000 adafruit-circuitpython-wiznet5k-5.0.1/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25760 2023-07-21 22:59:33.000000 adafruit-circuitpython-wiznet5k-5.0.1/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-07-21 22:59:33.000000 adafruit-circuitpython-wiznet5k-5.0.1/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27036 2023-07-21 22:59:33.000000 adafruit-circuitpython-wiznet5k-5.0.1/adafruit_wiznet5k/adafruit_wiznet5k_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-21 22:59:33.000000 adafruit-circuitpython-wiznet5k-5.0.1/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:59:41.800372 adafruit-circuitpython-wiznet5k-5.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:59:41.800372 adafruit-circuitpython-wiznet5k-5.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:59:41.804372 adafruit-circuitpython-wiznet5k-5.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-21 22:59:33.000000 adafruit-circuitpython-wiznet5k-5.0.1/examples/wiznet5k_aio_post.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-07-21 22:59:33.000000 adafruit-circuitpython-wiznet5k-5.0.1/examples/wiznet5k_cheerlights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-07-21 22:59:33.000000 adafruit-circuitpython-wiznet5k-5.0.1/examples/wiznet5k_cpython_client_for_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-21 22:59:33.000000 adafruit-circuitpython-wiznet5k-5.0.1/examples/wiznet5k_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-21 22:59:33.000000 adafruit-circuitpython-wiznet5k-5.0.1/examples/wiznet5k_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-21 22:59:33.000000 adafruit-circuitpython-wiznet5k-5.0.1/examples/wiznet5k_simpletest_manual_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-21 22:59:33.000000 adafruit-circuitpython-wiznet5k-5.0.1/examples/wiznet5k_wsgiserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-21 22:59:33.000000 adafruit-circuitpython-wiznet5k-5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-21 22:59:24.000000 adafruit-circuitpython-wiznet5k-5.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 22:59:41.804372 adafruit-circuitpython-wiznet5k-5.0.1/setup.cfg
```

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-wiznet5k-5.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/.gitignore` & `adafruit-circuitpython-wiznet5k-5.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/.pre-commit-config.yaml` & `adafruit-circuitpython-wiznet5k-5.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/.pylintrc` & `adafruit-circuitpython-wiznet5k-5.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-wiznet5k-5.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/LICENSE` & `adafruit-circuitpython-wiznet5k-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-wiznet5k-5.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/LICENSES/MIT.txt` & `adafruit-circuitpython-wiznet5k-5.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-wiznet5k-5.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/PKG-INFO` & `adafruit-circuitpython-wiznet5k-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wiznet5k
-Version: 5.0.0
+Version: 5.0.1
 Summary: Pure-Python interface for WIZNET 5k ethernet modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
 Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/README.rst` & `adafruit-circuitpython-wiznet5k-5.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO` & `adafruit-circuitpython-wiznet5k-5.0.1/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wiznet5k
-Version: 5.0.0
+Version: 5.0.1
 Summary: Pure-Python interface for WIZNET 5k ethernet modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
 Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt` & `adafruit-circuitpython-wiznet5k-5.0.1/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/adafruit_wiznet5k/adafruit_wiznet5k.py` & `adafruit-circuitpython-wiznet5k-5.0.1/adafruit_wiznet5k/adafruit_wiznet5k.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         import digitalio
 
         IpAddress4Raw = Union[bytes, Tuple[int, int, int, int]]
         MacAddressRaw = Union[bytes, Tuple[int, int, int, int, int, int]]
 except ImportError:
     pass
 
-__version__ = "5.0.0"
+__version__ = "5.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k.git"
 
 from random import randint
 import time
 import gc
 from micropython import const
```

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py` & `adafruit-circuitpython-wiznet5k-5.0.1/adafruit_wiznet5k/adafruit_wiznet5k_debug.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py` & `adafruit-circuitpython-wiznet5k-5.0.1/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py` & `adafruit-circuitpython-wiznet5k-5.0.1/adafruit_wiznet5k/adafruit_wiznet5k_dns.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/adafruit_wiznet5k/adafruit_wiznet5k_socket.py` & `adafruit-circuitpython-wiznet5k-5.0.1/adafruit_wiznet5k/adafruit_wiznet5k_socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,20 +402,20 @@
         ):
             if self._timeout and 0 < self._timeout < time.monotonic() - stamp:
                 raise TimeoutError("Failed to accept connection.")
             if self._status == wiznet5k.adafruit_wiznet5k.SNSR_SOCK_CLOSED:
                 self.close()
                 self.listen()
 
-        new_listen_socknum, addr = _the_interface.socket_accept(self._socknum)
+        _, addr = _the_interface.socket_accept(self._socknum)
         current_socknum = self._socknum
         # Create a new socket object and swap socket nums, so we can continue listening
         client_sock = socket()
+        self._socknum = client_sock._socknum  # pylint: disable=protected-access
         client_sock._socknum = current_socknum  # pylint: disable=protected-access
-        self._socknum = new_listen_socknum
         self._bind((None, self._listen_port))
         self.listen()
         while self._status != wiznet5k.adafruit_wiznet5k.SNSR_SOCK_LISTEN:
             raise RuntimeError("Failed to open new listening socket")
         return client_sock, addr
 
     @_check_socket_closed
```

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py` & `adafruit-circuitpython-wiznet5k-5.0.1/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/docs/_static/favicon.ico` & `adafruit-circuitpython-wiznet5k-5.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/docs/api.rst` & `adafruit-circuitpython-wiznet5k-5.0.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/docs/conf.py` & `adafruit-circuitpython-wiznet5k-5.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/docs/index.rst` & `adafruit-circuitpython-wiznet5k-5.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/examples/wiznet5k_aio_post.py` & `adafruit-circuitpython-wiznet5k-5.0.1/examples/wiznet5k_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/examples/wiznet5k_cheerlights.py` & `adafruit-circuitpython-wiznet5k-5.0.1/examples/wiznet5k_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/examples/wiznet5k_cpython_client_for_simpleserver.py` & `adafruit-circuitpython-wiznet5k-5.0.1/examples/wiznet5k_cpython_client_for_simpleserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/examples/wiznet5k_simpleserver.py` & `adafruit-circuitpython-wiznet5k-5.0.1/examples/wiznet5k_simpleserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/examples/wiznet5k_simpletest.py` & `adafruit-circuitpython-wiznet5k-5.0.1/examples/wiznet5k_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/examples/wiznet5k_simpletest_manual_network.py` & `adafruit-circuitpython-wiznet5k-5.0.1/examples/wiznet5k_simpletest_manual_network.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/examples/wiznet5k_wsgiserver.py` & `adafruit-circuitpython-wiznet5k-5.0.1/examples/wiznet5k_wsgiserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-5.0.0/pyproject.toml` & `adafruit-circuitpython-wiznet5k-5.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-wiznet5k"
 description = "Pure-Python interface for WIZNET 5k ethernet modules."
-version = "5.0.0"
+version = "5.0.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k"}
 keywords = [
     "adafruit",
```

