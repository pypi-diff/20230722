# Comparing `tmp/adafruit-circuitpython-wiznet5k-3.0.0.tar.gz` & `tmp/adafruit-circuitpython-wiznet5k-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-wiznet5k-3.0.0.tar", last modified: Tue Jun 27 17:30:01 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-wiznet5k-4.0.0.tar", last modified: Fri Jul 21 22:05:46 2023, max compression
```

## Comparing `adafruit-circuitpython-wiznet5k-3.0.0.tar` & `adafruit-circuitpython-wiznet5k-4.0.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.971476 adafruit-circuitpython-wiznet5k-3.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.967476 adafruit-circuitpython-wiznet5k-3.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.967476 adafruit-circuitpython-wiznet5k-3.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.967476 adafruit-circuitpython-wiznet5k-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.971476 adafruit-circuitpython-wiznet5k-3.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-27 17:30:01.971476 adafruit-circuitpython-wiznet5k-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.971476 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_circuitpython_wiznet5k.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-27 17:30:01.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-27 17:30:01.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:30:01.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 17:30:01.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 17:30:01.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.971476 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51329 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    27103 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py
--rw-r--r--   0 runner    (1001) docker     (123)    27015 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.971476 adafruit-circuitpython-wiznet5k-3.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.971476 adafruit-circuitpython-wiznet5k-3.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:30:01.971476 adafruit-circuitpython-wiznet5k-3.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_aio_post.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_cheerlights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_cpython_client_for_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_simpletest_manual_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_wsgiserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-27 17:29:54.000000 adafruit-circuitpython-wiznet5k-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-27 17:29:46.000000 adafruit-circuitpython-wiznet5k-3.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:30:01.971476 adafruit-circuitpython-wiznet5k-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:05:46.290364 adafruit-circuitpython-wiznet5k-4.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:05:46.286364 adafruit-circuitpython-wiznet5k-4.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:05:46.286364 adafruit-circuitpython-wiznet5k-4.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:05:46.286364 adafruit-circuitpython-wiznet5k-4.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:05:46.286364 adafruit-circuitpython-wiznet5k-4.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-07-21 22:05:46.290364 adafruit-circuitpython-wiznet5k-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:05:46.286364 adafruit-circuitpython-wiznet5k-4.0.0/adafruit_circuitpython_wiznet5k.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-07-21 22:05:46.000000 adafruit-circuitpython-wiznet5k-4.0.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-21 22:05:46.000000 adafruit-circuitpython-wiznet5k-4.0.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:05:46.000000 adafruit-circuitpython-wiznet5k-4.0.0/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-21 22:05:46.000000 adafruit-circuitpython-wiznet5k-4.0.0/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 22:05:46.000000 adafruit-circuitpython-wiznet5k-4.0.0/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:05:46.290364 adafruit-circuitpython-wiznet5k-4.0.0/adafruit_wiznet5k/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:05:38.000000 adafruit-circuitpython-wiznet5k-4.0.0/adafruit_wiznet5k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51695 2023-07-21 22:05:38.000000 adafruit-circuitpython-wiznet5k-4.0.0/adafruit_wiznet5k/adafruit_wiznet5k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-21 22:05:38.000000 adafruit-circuitpython-wiznet5k-4.0.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25760 2023-07-21 22:05:38.000000 adafruit-circuitpython-wiznet5k-4.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-07-21 22:05:38.000000 adafruit-circuitpython-wiznet5k-4.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-21 22:05:38.000000 adafruit-circuitpython-wiznet5k-4.0.0/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27015 2023-07-21 22:05:38.000000 adafruit-circuitpython-wiznet5k-4.0.0/adafruit_wiznet5k/adafruit_wiznet5k_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-21 22:05:38.000000 adafruit-circuitpython-wiznet5k-4.0.0/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:05:46.290364 adafruit-circuitpython-wiznet5k-4.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:05:46.290364 adafruit-circuitpython-wiznet5k-4.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:05:46.290364 adafruit-circuitpython-wiznet5k-4.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-21 22:05:38.000000 adafruit-circuitpython-wiznet5k-4.0.0/examples/wiznet5k_aio_post.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-07-21 22:05:38.000000 adafruit-circuitpython-wiznet5k-4.0.0/examples/wiznet5k_cheerlights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-07-21 22:05:38.000000 adafruit-circuitpython-wiznet5k-4.0.0/examples/wiznet5k_cpython_client_for_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-21 22:05:38.000000 adafruit-circuitpython-wiznet5k-4.0.0/examples/wiznet5k_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-21 22:05:38.000000 adafruit-circuitpython-wiznet5k-4.0.0/examples/wiznet5k_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-21 22:05:38.000000 adafruit-circuitpython-wiznet5k-4.0.0/examples/wiznet5k_simpletest_manual_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-21 22:05:38.000000 adafruit-circuitpython-wiznet5k-4.0.0/examples/wiznet5k_wsgiserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-21 22:05:38.000000 adafruit-circuitpython-wiznet5k-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-21 22:05:30.000000 adafruit-circuitpython-wiznet5k-4.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 22:05:46.290364 adafruit-circuitpython-wiznet5k-4.0.0/setup.cfg
```

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-wiznet5k-4.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/.gitignore` & `adafruit-circuitpython-wiznet5k-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/.pre-commit-config.yaml` & `adafruit-circuitpython-wiznet5k-4.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/.pylintrc` & `adafruit-circuitpython-wiznet5k-4.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-wiznet5k-4.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/LICENSE` & `adafruit-circuitpython-wiznet5k-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-wiznet5k-4.0.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/LICENSES/MIT.txt` & `adafruit-circuitpython-wiznet5k-4.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-wiznet5k-4.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/PKG-INFO` & `adafruit-circuitpython-wiznet5k-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wiznet5k
-Version: 3.0.0
+Version: 4.0.0
 Summary: Pure-Python interface for WIZNET 5k ethernet modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
 Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/README.rst` & `adafruit-circuitpython-wiznet5k-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO` & `adafruit-circuitpython-wiznet5k-4.0.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wiznet5k
-Version: 3.0.0
+Version: 4.0.0
 Summary: Pure-Python interface for WIZNET 5k ethernet modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
 Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt` & `adafruit-circuitpython-wiznet5k-4.0.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k.py` & `adafruit-circuitpython-wiznet5k-4.0.0/adafruit_wiznet5k/adafruit_wiznet5k.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         import digitalio
 
         IpAddress4Raw = Union[bytes, Tuple[int, int, int, int]]
         MacAddressRaw = Union[bytes, Tuple[int, int, int, int, int, int]]
 except ImportError:
     pass
 
-__version__ = "3.0.0"
+__version__ = "4.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k.git"
 
 from random import randint
 import time
 import gc
 from micropython import const
 
@@ -152,15 +152,15 @@
 _CH_SIZE = const(0x100)
 _SOCK_SIZE = const(0x800)  # MAX W5k socket size
 _SOCK_MASK = const(0x7FF)
 # Register commands
 _MR_RST = const(0x80)  # Mode Register RST
 # Socket mode register
 _SNMR_CLOSE = const(0x00)
-SNMR_TCP = const(0x21)
+_SNMR_TCP = const(0x21)
 SNMR_UDP = const(0x02)
 _SNMR_IPRAW = const(0x03)
 _SNMR_MACRAW = const(0x04)
 _SNMR_PPPOE = const(0x05)
 
 _MAX_PACKET = const(4000)
 _LOCAL_PORT = const(0x400)
@@ -488,15 +488,15 @@
         self._write(_REG_SUBR[self._chip_type], 0x04, bytes(subnet_mask))
         self._write(_REG_GAR[self._chip_type], 0x04, bytes(gateway_address))
 
         self._dns = bytes(dns_server)
 
     # *** Public Socket Methods ***
 
-    def socket_available(self, socket_num: int, sock_type: int = SNMR_TCP) -> int:
+    def socket_available(self, socket_num: int, sock_type: int = _SNMR_TCP) -> int:
         """
         Number of bytes available to be read from the socket.
 
         :param int socket_num: Socket to check for available bytes.
         :param int sock_type: Socket type. Use SNMR_TCP for TCP or SNMR_UDP for UDP,
             defaults to SNMR_TCP.
 
@@ -510,15 +510,15 @@
                 socket_num, sock_type
             ),
             self._debug,
         )
         self._sock_num_in_range(socket_num)
 
         number_of_bytes = self._get_rx_rcv_size(socket_num)
-        if self.read_snsr(socket_num) == SNMR_UDP:
+        if self._read_snsr(socket_num) == SNMR_UDP:
             number_of_bytes -= 8  # Subtract UDP header from packet size.
         if number_of_bytes < 0:
             raise ValueError("Negative number of bytes found on socket.")
         return number_of_bytes
 
     def socket_status(self, socket_num: int) -> int:
         """
@@ -529,22 +529,22 @@
         SNSR_SOCK_CLOSING, SNSR_SOCK_TIME_WAIT, SNSR_SOCK_CLOSE_WAIT, SNSR_LAST_ACK,
         SNSR_SOCK_UDP, SNSR_SOCK_IPRAW, SNSR_SOCK_MACRAW, SNSR_SOCK_PPOE.
 
         :param int socket_num: ID of socket to check.
 
         :return int: The connection status.
         """
-        return self.read_snsr(socket_num)
+        return self._read_snsr(socket_num)
 
     def socket_connect(
         self,
         socket_num: int,
         dest: IpAddress4Raw,
         port: int,
-        conn_mode: int = SNMR_TCP,
+        conn_mode: int = _SNMR_TCP,
     ) -> int:
         """
         Open and verify a connection from a socket to a destination IPv4 address
         or hostname. A TCP connection is made by default. A UDP connection can also
         be made.
 
         :param int socket_num: ID of the socket to be connected.
@@ -563,19 +563,19 @@
                 conn_mode, port, self.pretty_ip(dest)
             ),
             self._debug,
         )
         # initialize a socket and set the mode
         self.socket_open(socket_num, conn_mode=conn_mode)
         # set socket destination IP and port
-        self.write_sndipr(socket_num, dest)
-        self.write_sndport(socket_num, port)
-        self.write_sncr(socket_num, _CMD_SOCK_CONNECT)
+        self._write_sndipr(socket_num, dest)
+        self._write_sndport(socket_num, port)
+        self._write_sncr(socket_num, _CMD_SOCK_CONNECT)
 
-        if conn_mode == SNMR_TCP:
+        if conn_mode == _SNMR_TCP:
             # wait for tcp connection establishment
             while self.socket_status(socket_num) != SNSR_SOCK_ESTABLISHED:
                 time.sleep(0.001)
                 debug_msg(
                     "SNSR: {}".format(self.socket_status(socket_num)), self._debug
                 )
                 if self.socket_status(socket_num) == SNSR_SOCK_CLOSED:
@@ -634,15 +634,15 @@
 
         :raises ValueError: If the socket number is out of range.
         """
         self._sock_num_in_range(socket_number)
         WIZNET5K._sockets_reserved[socket_number - 1] = False
 
     def socket_listen(
-        self, socket_num: int, port: int, conn_mode: int = SNMR_TCP
+        self, socket_num: int, port: int, conn_mode: int = _SNMR_TCP
     ) -> None:
         """
         Listen on a socket's port.
 
         :param int socket_num: ID of socket to listen on.
         :param int port: Port to listen on (0 - 65,535).
         :param int conn_mode: Connection mode SNMR_TCP for TCP or SNMR_UDP for
@@ -661,23 +661,23 @@
             self._debug,
         )
         # Initialize a socket and set the mode
         self.src_port = port
         self.socket_open(socket_num, conn_mode=conn_mode)
         self.src_port = 0
         # Send listen command
-        self.write_sncr(socket_num, _CMD_SOCK_LISTEN)
+        self._write_sncr(socket_num, _CMD_SOCK_LISTEN)
         # Wait until ready
         status = SNSR_SOCK_CLOSED
         while status not in (
             SNSR_SOCK_LISTEN,
             SNSR_SOCK_ESTABLISHED,
             _SNSR_SOCK_UDP,
         ):
-            status = self.read_snsr(socket_num)
+            status = self._read_snsr(socket_num)
             if status == SNSR_SOCK_CLOSED:
                 raise RuntimeError("Listening socket closed.")
 
     def socket_accept(self, socket_num: int) -> Tuple[int, Tuple[str, int]]:
         """
         Destination IPv4 address and port from an incoming connection.
 
@@ -699,15 +699,15 @@
             "Dest is ({}, {}), Next listen socknum is #{}".format(
                 dest_ip, dest_port, next_socknum
             ),
             self._debug,
         )
         return next_socknum, (dest_ip, dest_port)
 
-    def socket_open(self, socket_num: int, conn_mode: int = SNMR_TCP) -> None:
+    def socket_open(self, socket_num: int, conn_mode: int = _SNMR_TCP) -> None:
         """
         Open an IP socket.
 
         The socket may connect via TCP or UDP protocols.
 
         :param int socket_num: The socket number to open.
         :param int conn_mode: The protocol to use. Use SNMR_TCP for TCP or SNMR_UDP for \
@@ -716,62 +716,62 @@
         :raises ValueError: If the socket number is out of range.
         :raises ConnectionError: If the Ethernet link is down or no connection to socket.
         :raises RuntimeError: If unable to open a socket in UDP or TCP mode.
         """
         self._sock_num_in_range(socket_num)
         self._check_link_status()
         debug_msg("*** Opening socket {}".format(socket_num), self._debug)
-        if self.read_snsr(socket_num) not in (
+        if self._read_snsr(socket_num) not in (
             SNSR_SOCK_CLOSED,
             SNSR_SOCK_TIME_WAIT,
             SNSR_SOCK_FIN_WAIT,
             SNSR_SOCK_CLOSE_WAIT,
             _SNSR_SOCK_CLOSING,
             _SNSR_SOCK_UDP,
         ):
             raise ConnectionError("Failed to initialize a connection with the socket.")
         debug_msg("* Opening W5k Socket, protocol={}".format(conn_mode), self._debug)
         time.sleep(0.00025)
 
-        self.write_snmr(socket_num, conn_mode)
+        self._write_snmr(socket_num, conn_mode)
         self.write_snir(socket_num, 0xFF)
 
         if self.src_port > 0:
             # write to socket source port
-            self.write_sock_port(socket_num, self.src_port)
+            self._write_sock_port(socket_num, self.src_port)
         else:
             s_port = randint(49152, 65535)
             while s_port in self._src_ports_in_use:
                 s_port = randint(49152, 65535)
-            self.write_sock_port(socket_num, s_port)
+            self._write_sock_port(socket_num, s_port)
             self._src_ports_in_use[socket_num] = s_port
 
         # open socket
-        self.write_sncr(socket_num, _CMD_SOCK_OPEN)
-        if self.read_snsr(socket_num) not in [_SNSR_SOCK_INIT, _SNSR_SOCK_UDP]:
+        self._write_sncr(socket_num, _CMD_SOCK_OPEN)
+        if self._read_snsr(socket_num) not in [_SNSR_SOCK_INIT, _SNSR_SOCK_UDP]:
             raise RuntimeError("Could not open socket in TCP or UDP mode.")
 
     def socket_close(self, socket_num: int) -> None:
         """
         Close a socket.
 
         :param int socket_num: The socket to close.
 
         :raises ValueError: If the socket number is out of range.
         """
         debug_msg("*** Closing socket {}".format(socket_num), self._debug)
         self._sock_num_in_range(socket_num)
-        self.write_sncr(socket_num, _CMD_SOCK_CLOSE)
+        self._write_sncr(socket_num, _CMD_SOCK_CLOSE)
         debug_msg("  Waiting for socket to close…", self._debug)
         timeout = time.monotonic() + 5.0
-        while self.read_snsr(socket_num) != SNSR_SOCK_CLOSED:
+        while self._read_snsr(socket_num) != SNSR_SOCK_CLOSED:
             if time.monotonic() > timeout:
                 raise RuntimeError(
                     "Wiznet5k failed to close socket, status = {}.".format(
-                        self.read_snsr(socket_num)
+                        self._read_snsr(socket_num)
                     )
                 )
             time.sleep(0.0001)
         debug_msg("  Socket has closed.", self._debug)
 
     def socket_disconnect(self, socket_num: int) -> None:
         """
@@ -779,15 +779,15 @@
 
         :param int socket_num: The socket to close.
 
         :raises ValueError: If the socket number is out of range.
         """
         debug_msg("*** Disconnecting socket {}".format(socket_num), self._debug)
         self._sock_num_in_range(socket_num)
-        self.write_sncr(socket_num, _CMD_SOCK_DISCON)
+        self._write_sncr(socket_num, _CMD_SOCK_DISCON)
 
     def socket_read(self, socket_num: int, length: int) -> Tuple[int, bytes]:
         """
         Read data from a hardware socket. Called directly by TCP socket objects and via
         read_udp() for UDP socket objects.
 
         :param int socket_num: The socket to read data from.
@@ -815,15 +815,15 @@
             # Read the starting save address of the received data.
             pointer = self._read_snrx_rd(socket_num)
             # Read data from the hardware socket.
             bytes_read = self._chip_socket_read(socket_num, pointer, bytes_on_socket)
             # After reading the received data, update Sn_RX_RD register.
             pointer = (pointer + bytes_on_socket) & 0xFFFF
             self._write_snrx_rd(socket_num, pointer)
-            self.write_sncr(socket_num, _CMD_SOCK_RECV)
+            self._write_sncr(socket_num, _CMD_SOCK_RECV)
         else:
             # no data on socket
             if self._read_snmr(socket_num) in (
                 SNSR_SOCK_LISTEN,
                 SNSR_SOCK_CLOSED,
                 SNSR_SOCK_CLOSE_WAIT,
             ):
@@ -902,15 +902,15 @@
         # Read the starting address for saving the transmitting data.
         pointer = self._read_sntx_wr(socket_num)
         offset = pointer & _SOCK_MASK
         self._chip_socket_write(socket_num, offset, bytes_to_write, buffer)
         # update sn_tx_wr to the value + data size
         pointer = (pointer + bytes_to_write) & 0xFFFF
         self._write_sntx_wr(socket_num, pointer)
-        self.write_sncr(socket_num, _CMD_SOCK_SEND)
+        self._write_sncr(socket_num, _CMD_SOCK_SEND)
 
         # check data was  transferred correctly
         while not self.read_snir(socket_num) & _SNIR_SEND_OK:
             if self.socket_status(socket_num) in (
                 SNSR_SOCK_CLOSED,
                 SNSR_SOCK_TIME_WAIT,
                 SNSR_SOCK_FIN_WAIT,
@@ -1053,14 +1053,19 @@
             raise ValueError("Socket number out of range.")
 
     def _check_link_status(self):
         """Raise an exception if the link is down."""
         if not self.link_status:
             raise ConnectionError("The Ethernet connection is down.")
 
+    @staticmethod
+    def _read_socket_reservations() -> list[int]:
+        """Return the list of reserved sockets."""
+        return WIZNET5K._sockets_reserved
+
     def _read_mr(self) -> int:
         """Read from the Mode Register (MR)."""
         return int.from_bytes(self._read(_REG_MR[self._chip_type], 0x00), "big")
 
     def _write_mr(self, data: int) -> None:
         """Write to the mode register (MR)."""
         self._write(_REG_MR[self._chip_type], 0x04, data)
@@ -1171,26 +1176,30 @@
         data = []
         for offset in range(4):
             data.append(
                 self._read_socket_register(sock, _REG_SNDIPR[self._chip_type] + offset)
             )
         return bytes(data)
 
-    def write_sndipr(self, sock: int, ip_addr: bytes) -> None:
+    def _write_sndipr(self, sock: int, ip_addr: bytes) -> None:
         """Write to socket destination IP Address."""
         for offset, value in enumerate(ip_addr):
             self._write_socket_register(
                 sock, _REG_SNDIPR[self._chip_type] + offset, value
             )
 
-    def write_sndport(self, sock: int, port: int) -> None:
+    def _read_sndport(self, sock: int) -> int:
+        """Read socket destination port."""
+        return self._read_two_byte_sock_reg(sock, _REG_SNDPORT[self._chip_type])
+
+    def _write_sndport(self, sock: int, port: int) -> None:
         """Write to socket destination port."""
         self._write_two_byte_sock_reg(sock, _REG_SNDPORT[self._chip_type], port)
 
-    def read_snsr(self, sock: int) -> int:
+    def _read_snsr(self, sock: int) -> int:
         """Read Socket n Status Register."""
         return self._read_socket_register(sock, _REG_SNSR[self._chip_type])
 
     def read_snir(self, sock: int) -> int:
         """Read Socket n Interrupt Register."""
         return self._read_socket_register(sock, _REG_SNIR[self._chip_type])
 
@@ -1198,23 +1207,23 @@
         """Write to Socket n Interrupt Register."""
         self._write_socket_register(sock, _REG_SNIR[self._chip_type], data)
 
     def _read_snmr(self, sock: int) -> int:
         """Read the socket MR register."""
         return self._read_socket_register(sock, _REG_SNMR)
 
-    def write_snmr(self, sock: int, protocol: int) -> None:
+    def _write_snmr(self, sock: int, protocol: int) -> None:
         """Write to Socket n Mode Register."""
         self._write_socket_register(sock, _REG_SNMR, protocol)
 
-    def write_sock_port(self, sock: int, port: int) -> None:
+    def _write_sock_port(self, sock: int, port: int) -> None:
         """Write to the socket port number."""
         self._write_two_byte_sock_reg(sock, _REG_SNPORT[self._chip_type], port)
 
-    def write_sncr(self, sock: int, data: int) -> None:
+    def _write_sncr(self, sock: int, data: int) -> None:
         """Write to socket command register."""
         self._write_socket_register(sock, _REG_SNCR[self._chip_type], data)
         # Wait for command to complete before continuing.
         while self._read_socket_register(sock, _REG_SNCR[self._chip_type]):
             pass
 
     @property
```

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py` & `adafruit-circuitpython-wiznet5k-4.0.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py` & `adafruit-circuitpython-wiznet5k-4.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py`

 * *Files 7% similar despite different names*

```diff
@@ -143,15 +143,14 @@
         # Prevent buffer overrun in send_dhcp_message()
         if len(mac_address) != 6:
             raise ValueError("MAC address must be 6 bytes.")
         self._mac_address = mac_address
 
         # Set socket interface
         self._eth = eth
-        self._wiz_sock = None
 
         # DHCP state machine
         self._dhcp_state = _STATE_INIT
         self._transaction_id = randint(1, 0x7FFFFFFF)
         self._start_time = 0.0
         self._blocking = False
         self._renew = None
@@ -192,16 +191,14 @@
         debug_msg("Maintaining lease with blocking = {}".format(blocking), self._debug)
         self._dhcp_state_machine(blocking=blocking)
 
     def _dsm_reset(self) -> None:
         """Close the socket and set attributes to default values used by the
         state machine INIT state."""
         debug_msg("Resetting DHCP state machine.", self._debug)
-        self._socket_release()
-        self._dhcp_connection_setup()
         self.dhcp_server_ip = _BROADCAST_SERVER_ADDR
         self._eth.ifconfig = (
             _UNASSIGNED_IP_ADDR,
             _UNASSIGNED_IP_ADDR,
             _UNASSIGNED_IP_ADDR,
             _UNASSIGNED_IP_ADDR,
         )
@@ -209,53 +206,14 @@
         self.local_ip = _UNASSIGNED_IP_ADDR
         self.subnet_mask = _UNASSIGNED_IP_ADDR
         self.dns_server_ip = _UNASSIGNED_IP_ADDR
         self._renew = None
         self._increment_transaction_id()
         self._start_time = time.monotonic()
 
-    def _socket_release(self) -> None:
-        """Close the socket if it exists."""
-        debug_msg("Releasing socket.", self._debug)
-        if self._wiz_sock:
-            self._eth.socket_close(self._wiz_sock)
-            self._wiz_sock = None
-        debug_msg("  Socket released.", self._debug)
-
-    def _dhcp_connection_setup(self, timeout: float = 5.0) -> None:
-        """Initialise a UDP socket.
-
-        Attempt to initialise a UDP socket. If the finite state machine (FSM) is in
-        blocking mode, repeat failed attempts until a socket is initialised or
-        the operation times out, then raise an exception. If the FSM is in non-blocking
-        mode, ignore the error and return.
-
-        :param int timeout: Time to keep retrying if the FSM is in blocking mode.
-            Defaults to 5.
-
-        :raises TimeoutError: If the FSM is in blocking mode and a socket cannot be
-            initialised.
-        """
-        stop_time = time.monotonic() + timeout
-        debug_msg("Setting up connection for DHCP.", self._debug)
-        while self._wiz_sock is None and time.monotonic() < stop_time:
-            self._wiz_sock = self._eth.get_socket()
-            if self._wiz_sock == 0xFF:
-                self._wiz_sock = None
-        while time.monotonic() < stop_time:
-            self._eth.write_snmr(self._wiz_sock, 0x02)  # Set UDP connection
-            self._eth.write_sock_port(self._wiz_sock, 68)  # Set DHCP client port.
-            self._eth.write_sncr(self._wiz_sock, 0x01)  # Open the socket.
-            if self._eth.read_snsr(self._wiz_sock) == 0x22:
-                self._eth.write_sndport(2, _DHCP_SERVER_PORT)
-                debug_msg("+ Connection OK, port set.", self._debug)
-                return
-        self._wiz_sock = None
-        raise RuntimeError("Unable to initialize UDP socket.")
-
     def _increment_transaction_id(self) -> None:
         """Increment the transaction ID and roll over from 0x7fffffff to 0."""
         debug_msg("Incrementing transaction ID", self._debug)
         self._transaction_id = (self._transaction_id + 1) & 0x7FFFFFFF
 
     def _next_retry_time(self, *, attempt: int, interval: int = 4) -> float:
         """Calculate a retry stop time.
@@ -276,41 +234,40 @@
         """
         debug_msg("Calculating next retry time and incrementing retries.", self._debug)
         if interval <= 1:
             raise ValueError("Retry interval must be > 1 second.")
         delay = 2**attempt * interval + randint(-1, 1) + time.monotonic()
         return delay
 
-    def _receive_dhcp_response(self, timeout: float) -> int:
+    def _receive_dhcp_response(self, socket_num: int, timeout: float) -> int:
         """
         Receive data from the socket in response to a DHCP query.
 
         Reads data from the buffer until a viable minimum packet size has been
         received or the operation times out. If a viable packet is received, it is
         stored in the global buffer and the number of bytes received is returned.
         If the packet is too short, it is discarded and zero is returned. The
         maximum packet size is limited by the size of the global buffer.
 
-        :param float timeout: time.monotonic at which attempt should timeout.
+        :param int socket_num: Socket to read from.
+        :param float timeout: time.monotonic at which attempt should time out.
 
         :returns int: The number of bytes stored in the global buffer.
         """
         debug_msg("Receiving a DHCP response.", self._debug)
         while time.monotonic() < timeout:
             # DHCP returns the query plus additional data. The query length is 236 bytes.
-            if self._eth.socket_available(self._wiz_sock, _SNMR_UDP) > 236:
-                bytes_count, bytes_read = self._eth.read_udp(
-                    self._wiz_sock, _BUFF_LENGTH
-                )
+            if self._eth.socket_available(socket_num, _SNMR_UDP) > 236:
+                bytes_count, bytes_read = self._eth.read_udp(socket_num, _BUFF_LENGTH)
                 _BUFF[:bytes_count] = bytes_read
                 debug_msg("Received {} bytes".format(bytes_count), self._debug)
                 del bytes_read
                 gc.collect()
                 return bytes_count
-        raise TimeoutError("No DHCP response received.")
+        return 0  # No bytes received.
 
     def _process_messaging_states(self, *, message_type: int):
         """
         Process a message while the FSM is in SELECTING or REQUESTING state.
 
         Check the message and update the FSM state if it is a valid type.
 
@@ -353,68 +310,85 @@
             or renewing states.
 
         :raises ValueError: If the function is not called from SELECTING or BLOCKING FSM
             states.
         :raises TimeoutError: If the FSM is in blocking mode and no valid response has
             been received before the timeout expires.
         """
+        # pylint: disable=too-many-branches
         debug_msg("Processing SELECTING or REQUESTING state.", self._debug)
         if self._dhcp_state == _STATE_SELECTING:
             msg_type_out = _DHCP_DISCOVER
         elif self._dhcp_state == _STATE_REQUESTING:
             msg_type_out = _DHCP_REQUEST
         else:
             raise ValueError(
                 "FSM can only send messages while in SELECTING or REQUESTING states."
             )
-        for attempt in range(4):  # Initial attempt plus 3 retries.
-            message_length = self._generate_dhcp_message(message_type=msg_type_out)
+        debug_msg("Setting up connection for DHCP.", self._debug)
+        if self._renew:
+            dhcp_server = self.dhcp_server_ip
+        else:
+            dhcp_server = _BROADCAST_SERVER_ADDR
+        sock_num = None
+        deadline = time.monotonic() + 5.0
+        try:
+            while sock_num is None:
+                sock_num = self._eth.get_socket()
+                if sock_num == 0xFF:
+                    sock_num = None
+                if time.monotonic() > deadline:
+                    raise RuntimeError("Unable to initialize UDP socket.")
+
+            self._eth.src_port = 68
+            self._eth.socket_connect(
+                sock_num, dhcp_server, _DHCP_SERVER_PORT, conn_mode=0x02
+            )
+            self._eth.src_port = 0
 
-            if self._renew:
-                dhcp_server_address = self.dhcp_server_ip
-            else:
-                dhcp_server_address = _BROADCAST_SERVER_ADDR
-            self._eth.write_sndipr(self._wiz_sock, dhcp_server_address)
-            self._eth.write_sndport(self._wiz_sock, _DHCP_SERVER_PORT)
-            self._eth.socket_write(self._wiz_sock, _BUFF[:message_length])
-            next_resend = self._next_retry_time(attempt=attempt)
-            while time.monotonic() < next_resend:
-                if self._receive_dhcp_response(next_resend):
-                    try:
-                        msg_type_in = self._parse_dhcp_response()
+            message_length = self._generate_dhcp_message(message_type=msg_type_out)
+            for attempt in range(4):  # Initial attempt plus 3 retries.
+                self._eth.socket_write(sock_num, _BUFF[:message_length])
+                next_resend = self._next_retry_time(attempt=attempt)
+                while time.monotonic() < next_resend:
+                    if self._receive_dhcp_response(sock_num, next_resend):
+                        try:
+                            msg_type_in = self._parse_dhcp_response()
+                            debug_msg(
+                                "Received message type {}".format(msg_type_in),
+                                self._debug,
+                            )
+                            return msg_type_in
+                        except ValueError as error:
+                            debug_msg(error, self._debug)
+                    if not self._blocking or self._renew:
                         debug_msg(
-                            "Received message type {}".format(msg_type_in), self._debug
+                            "No message, FSM is nonblocking or renewing, exiting loop.",
+                            self._debug,
                         )
-                        return msg_type_in
-                    except ValueError as error:
-                        debug_msg(error, self._debug)
-                if not self._blocking or self._renew:
-                    debug_msg(
-                        "No message, FSM is nonblocking or renewing, exiting loop.",
-                        self._debug,
-                    )
-                    return 0  # Did not receive a response in a single attempt.
-        raise TimeoutError(
-            "No response from DHCP server after {} retries.".format(attempt)
-        )
+                        return 0  # Did not receive a response in a single attempt.
+            raise TimeoutError(
+                "No response from DHCP server after {} retries.".format(attempt)
+            )
+        finally:
+            self._eth.socket_close(sock_num)  # Close the socket whatever happens.
 
     def _dhcp_state_machine(self, *, blocking: bool = False) -> None:
         """
         A finite state machine to allow the DHCP lease to be managed without blocking
         the main program. The initial lease...
         """
         debug_msg("DHCP FSM called with blocking = {}".format(blocking), self._debug)
         debug_msg("FSM initial state is {}".format(self._dhcp_state), self._debug)
         self._blocking = blocking
         while True:
             if self._dhcp_state == _STATE_BOUND:
                 now = time.monotonic()
                 if now < self._t1:
                     debug_msg("No timers have expired. Exiting FSM.", self._debug)
-                    self._socket_release()
                     return
                 if now > self._lease:
                     debug_msg(
                         "Lease has expired, switching state to INIT.", self._debug
                     )
                     self._blocking = True
                     self._dhcp_state = _STATE_INIT
@@ -428,23 +402,21 @@
                         "T1 has expired, switching state to RENEWING.", self._debug
                     )
                     self._dhcp_state = _STATE_RENEWING
 
             if self._dhcp_state == _STATE_RENEWING:
                 debug_msg("FSM state is RENEWING.", self._debug)
                 self._renew = "renew"
-                self._dhcp_connection_setup()
                 self._start_time = time.monotonic()
                 self._dhcp_state = _STATE_REQUESTING
 
             if self._dhcp_state == _STATE_REBINDING:
                 debug_msg("FSM state is REBINDING.", self._debug)
                 self._renew = "rebind"
                 self.dhcp_server_ip = _BROADCAST_SERVER_ADDR
-                self._dhcp_connection_setup()
                 self._start_time = time.monotonic()
                 self._dhcp_state = _STATE_REQUESTING
 
             if self._dhcp_state == _STATE_INIT:
                 debug_msg("FSM state is INIT.", self._debug)
                 self._dsm_reset()
                 self._dhcp_state = _STATE_SELECTING
```

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py` & `adafruit-circuitpython-wiznet5k-4.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py` & `adafruit-circuitpython-wiznet5k-4.0.0/adafruit_wiznet5k/adafruit_wiznet5k_ntp.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     if TYPE_CHECKING:
         from adafruit_wiznet5k.adafruit_wiznet5k import WIZNET5K
 except ImportError:
     pass
 import time
 import adafruit_wiznet5k.adafruit_wiznet5k_socket as socket
 
-# __version__ = "3.0.0"
+# __version__ = "4.0.0"
 # __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_NTP.git"
 
 
 class NTP:
     """Wiznet5k NTP Client."""
 
     def __init__(
```

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_socket.py` & `adafruit-circuitpython-wiznet5k-4.0.0/adafruit_wiznet5k/adafruit_wiznet5k_socket.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py` & `adafruit-circuitpython-wiznet5k-4.0.0/adafruit_wiznet5k/adafruit_wiznet5k_wsgiserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/docs/_static/favicon.ico` & `adafruit-circuitpython-wiznet5k-4.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/docs/api.rst` & `adafruit-circuitpython-wiznet5k-4.0.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/docs/conf.py` & `adafruit-circuitpython-wiznet5k-4.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/docs/index.rst` & `adafruit-circuitpython-wiznet5k-4.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_aio_post.py` & `adafruit-circuitpython-wiznet5k-4.0.0/examples/wiznet5k_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_cheerlights.py` & `adafruit-circuitpython-wiznet5k-4.0.0/examples/wiznet5k_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_cpython_client_for_simpleserver.py` & `adafruit-circuitpython-wiznet5k-4.0.0/examples/wiznet5k_cpython_client_for_simpleserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_simpleserver.py` & `adafruit-circuitpython-wiznet5k-4.0.0/examples/wiznet5k_simpleserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_simpletest.py` & `adafruit-circuitpython-wiznet5k-4.0.0/examples/wiznet5k_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_simpletest_manual_network.py` & `adafruit-circuitpython-wiznet5k-4.0.0/examples/wiznet5k_simpletest_manual_network.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/examples/wiznet5k_wsgiserver.py` & `adafruit-circuitpython-wiznet5k-4.0.0/examples/wiznet5k_wsgiserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wiznet5k-3.0.0/pyproject.toml` & `adafruit-circuitpython-wiznet5k-4.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-wiznet5k"
 description = "Pure-Python interface for WIZNET 5k ethernet modules."
-version = "3.0.0"
+version = "4.0.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k"}
 keywords = [
     "adafruit",
```

