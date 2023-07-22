# Comparing `tmp/custodian-2023.6.5.tar.gz` & `tmp/custodian-2023.7.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custodian-2023.6.5.tar", last modified: Mon Jun  5 15:24:27 2023, max compression
+gzip compressed data, was "custodian-2023.7.22.tar", last modified: Sat Jul 22 15:25:19 2023, max compression
```

## Comparing `custodian-2023.6.5.tar` & `custodian-2023.7.22.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.789778 custodian-2023.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-05 15:20:36.000000 custodian-2023.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-05 15:20:36.000000 custodian-2023.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-05 15:24:27.789778 custodian-2023.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-05 15:20:36.000000 custodian-2023.6.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.785778 custodian-2023.6.5/custodian/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.785778 custodian-2023.6.5/custodian/ansible/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/ansible/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/ansible/interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.785778 custodian-2023.6.5/custodian/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3653 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cli/converge_geometry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4538 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cli/converge_kpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3486 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cli/cstdn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2337 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cli/run_nwchem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12410 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cli/run_vasp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.785778 custodian-2023.6.5/custodian/cp2k/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cp2k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44267 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cp2k/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cp2k/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cp2k/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cp2k/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/cp2k/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    36611 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/custodian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.785778 custodian-2023.6.5/custodian/feff/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/feff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/feff/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/feff/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/feff/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.789778 custodian-2023.6.5/custodian/lobster/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/lobster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/lobster/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/lobster/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.789778 custodian-2023.6.5/custodian/nwchem/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/nwchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/nwchem/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/nwchem/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.789778 custodian-2023.6.5/custodian/qchem/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20599 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/qchem/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    31904 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/qchem/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/qchem/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.789778 custodian-2023.6.5/custodian/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/tests/test_custodian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.789778 custodian-2023.6.5/custodian/vasp/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76553 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/vasp/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/vasp/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)    39455 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/vasp/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-06-05 15:20:36.000000 custodian-2023.6.5/custodian/vasp/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:24:27.785778 custodian-2023.6.5/custodian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-05 15:24:27.000000 custodian-2023.6.5/custodian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-05 15:24:27.000000 custodian-2023.6.5/custodian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:24:27.000000 custodian-2023.6.5/custodian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-05 15:24:27.000000 custodian-2023.6.5/custodian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-05 15:24:27.000000 custodian-2023.6.5/custodian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 15:24:27.000000 custodian-2023.6.5/custodian.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-05 15:20:36.000000 custodian-2023.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-05 15:20:36.000000 custodian-2023.6.5/requirements-ci.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-05 15:20:36.000000 custodian-2023.6.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-05 15:24:27.789778 custodian-2023.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-05 15:20:36.000000 custodian-2023.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:25:19.642495 custodian-2023.7.22/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-22 15:21:31.000000 custodian-2023.7.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-22 15:21:31.000000 custodian-2023.7.22/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-22 15:25:19.642495 custodian-2023.7.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-22 15:21:31.000000 custodian-2023.7.22/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:25:19.630494 custodian-2023.7.22/custodian/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:25:19.634494 custodian-2023.7.22/custodian/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/ansible/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/ansible/interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:25:19.634494 custodian-2023.7.22/custodian/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3653 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/cli/converge_geometry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4538 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/cli/converge_kpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3486 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/cli/cstdn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2337 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/cli/run_nwchem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12410 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/cli/run_vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:25:19.638494 custodian-2023.7.22/custodian/cp2k/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/cp2k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44267 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/cp2k/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/cp2k/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/cp2k/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/cp2k/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/cp2k/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37284 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/custodian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:25:19.638494 custodian-2023.7.22/custodian/feff/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/feff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/feff/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/feff/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/feff/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:25:19.638494 custodian-2023.7.22/custodian/lobster/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/lobster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/lobster/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/lobster/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:25:19.642495 custodian-2023.7.22/custodian/nwchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/nwchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/nwchem/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/nwchem/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:25:19.642495 custodian-2023.7.22/custodian/qchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20599 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/qchem/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31904 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/qchem/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/qchem/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:25:19.642495 custodian-2023.7.22/custodian/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/tests/test_custodian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:25:19.642495 custodian-2023.7.22/custodian/vasp/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76925 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/vasp/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/vasp/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39733 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/vasp/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-07-22 15:21:31.000000 custodian-2023.7.22/custodian/vasp/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:25:19.634494 custodian-2023.7.22/custodian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-22 15:25:19.000000 custodian-2023.7.22/custodian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-22 15:25:19.000000 custodian-2023.7.22/custodian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 15:25:19.000000 custodian-2023.7.22/custodian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-22 15:25:19.000000 custodian-2023.7.22/custodian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-22 15:25:19.000000 custodian-2023.7.22/custodian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-22 15:25:19.000000 custodian-2023.7.22/custodian.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-22 15:21:31.000000 custodian-2023.7.22/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-22 15:21:31.000000 custodian-2023.7.22/requirements-ci.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-22 15:21:31.000000 custodian-2023.7.22/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-22 15:25:19.642495 custodian-2023.7.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-22 15:21:31.000000 custodian-2023.7.22/setup.py
```

### Comparing `custodian-2023.6.5/LICENSE` & `custodian-2023.7.22/LICENSE`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/PKG-INFO` & `custodian-2023.7.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custodian
-Version: 2023.6.5
+Version: 2023.7.22
 Summary: A simple JIT job management framework in Python.
 Home-page: https://github.com/materialsproject/custodian
 Author: Shyue Ping Ong, William Davidson Richards, Stephen Dacek, Xiaohui Qu, Matthew Horton, Samuel M. Blau
 Author-email: ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 License: MIT
 Keywords: jit,just-in-time,job,management,vasp
```

### Comparing `custodian-2023.6.5/README.rst` & `custodian-2023.7.22/README.rst`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/ansible/actions.py` & `custodian-2023.7.22/custodian/ansible/actions.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/ansible/interpreter.py` & `custodian-2023.7.22/custodian/ansible/interpreter.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/cli/converge_geometry.py` & `custodian-2023.7.22/custodian/cli/converge_geometry.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/cli/converge_kpoints.py` & `custodian-2023.7.22/custodian/cli/converge_kpoints.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/cli/cstdn.py` & `custodian-2023.7.22/custodian/cli/cstdn.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/cli/run_nwchem.py` & `custodian-2023.7.22/custodian/cli/run_nwchem.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/cli/run_vasp.py` & `custodian-2023.7.22/custodian/cli/run_vasp.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/cp2k/handlers.py` & `custodian-2023.7.22/custodian/cp2k/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/cp2k/interpreter.py` & `custodian-2023.7.22/custodian/cp2k/interpreter.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/cp2k/jobs.py` & `custodian-2023.7.22/custodian/cp2k/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/cp2k/utils.py` & `custodian-2023.7.22/custodian/cp2k/utils.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/cp2k/validators.py` & `custodian-2023.7.22/custodian/cp2k/validators.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/custodian.py` & `custodian-2023.7.22/custodian/custodian.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     # will set for True, true, TRUE, etc.
     if literal_eval(os.environ.get("CUSTODIAN_REPORTING_OPT_IN", "False").title()):
         SENTRY_DSN = "https://0f7291738eb042a3af671df9fc68ae2a@sentry.io/1470881"
 
 if SENTRY_DSN:
     import sentry_sdk
 
-    sentry_sdk.init(dsn=SENTRY_DSN)
+    sentry_sdk.init(dsn=SENTRY_DSN)  # pylint: disable=E0110
 
     with sentry_sdk.configure_scope() as scope:
         from getpass import getuser
 
         try:
             scope.user = {"username": getuser()}
         except Exception:
@@ -455,29 +455,39 @@
 
             p = job.run()
             # Check for errors using the error handlers and perform
             # corrections.
             has_error = False
             zero_return_code = True
 
+            # Choose the terminate function to run. If a terminate_func exists, this
+            # should take priority, followed by Job.terminate if implemented, and finally
+            # subprocess.Popen.terminate if neither of the former exist.
+            terminate = self.terminate_func or job.terminate or p.terminate
+
             # While the job is running, we use the handlers that are
             # monitors to monitor the job.
             if isinstance(p, subprocess.Popen):
                 if self.monitors:
                     n = 0
                     while True:
                         n += 1
                         time.sleep(self.polling_time_step)
+                        # We poll the process p to check if it is still running.
+                        # Note that the process here is not the actual calculation
+                        # but whatever is used to control the execution of the
+                        # calculation executable. For instance; mpirun, srun, and so on.
                         if p.poll() is not None:
                             break
-                        terminate = self.terminate_func or p.terminate
                         if n % self.monitor_freq == 0:
+                            # At every self.polling_time_step * self.monitor_freq seconds,
+                            # we check the job for errors using handlers that are monitors.
+                            # In order to properly kill a running calculation, we use
+                            # the appropriate implementation of terminate.
                             has_error = self._do_check(self.monitors, terminate)
-                        if terminate is not None and terminate != p.terminate:
-                            time.sleep(self.polling_time_step)
                 else:
                     p.wait()
                     if self.terminate_func is not None and self.terminate_func != p.terminate:
                         self.terminate_func()
                         time.sleep(self.polling_time_step)
 
                 zero_return_code = p.returncode == 0
@@ -487,18 +497,14 @@
             # handlers fix the problems detected by monitors
             # if an error has been found, not all handlers need to run
             if has_error:
                 self._do_check([h for h in self.handlers if not h.is_monitor])
             else:
                 has_error = self._do_check(self.handlers)
 
-            if has_error:
-                # This makes sure the job is killed cleanly for certain systems.
-                job.terminate()
-
             # If there are no errors detected, perform
             # postprocessing and exit.
             if not has_error:
                 for v in self.validators:
                     if v.check():
                         self.run_log[-1]["validator"] = v
                         s = f"Validation failed: {v.__class__.__name__}"
```

### Comparing `custodian-2023.6.5/custodian/feff/handlers.py` & `custodian-2023.7.22/custodian/feff/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/feff/interpreter.py` & `custodian-2023.7.22/custodian/feff/interpreter.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/feff/jobs.py` & `custodian-2023.7.22/custodian/feff/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/lobster/handlers.py` & `custodian-2023.7.22/custodian/lobster/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/lobster/jobs.py` & `custodian-2023.7.22/custodian/lobster/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/nwchem/handlers.py` & `custodian-2023.7.22/custodian/nwchem/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/nwchem/jobs.py` & `custodian-2023.7.22/custodian/nwchem/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/qchem/handlers.py` & `custodian-2023.7.22/custodian/qchem/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/qchem/jobs.py` & `custodian-2023.7.22/custodian/qchem/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/qchem/utils.py` & `custodian-2023.7.22/custodian/qchem/utils.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/tests/test_custodian.py` & `custodian-2023.7.22/custodian/tests/test_custodian.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/utils.py` & `custodian-2023.7.22/custodian/utils.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/vasp/handlers.py` & `custodian-2023.7.22/custodian/vasp/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,29 +120,29 @@
         Args:
             output_filename (str): This is the file where the stdout for vasp
                 is being redirected. The error messages that are checked are
                 present in the stdout. Defaults to "vasp.out", which is the
                 default redirect used by :class:`custodian.vasp.jobs.VaspJob`.
             errors_subset_to_detect (list): A subset of errors to catch. The
                 default is None, which means all supported errors are detected.
-                Use this to only catch only a subset of supported errors.
-                E.g., ["eddrrm", "zheev"] will only catch the eddrmm and zheev
-                errors, and not others. If you wish to only excluded one or
+                Use this to catch only a subset of supported errors.
+                E.g., ["eddrmm", "zheev"] will only catch the eddrmm and zheev
+                errors, and not others. If you wish to only exclude one or
                 two of the errors, you can create this list by the following
                 lines:
-            vtst_fixes (bool): Whether to consider VTST optimizers. Defaults to
-                False for compatibility purposes, but if you have VTST, you
-                would likely benefit from setting this to True.
 
                 ```
-                subset = list(VaspErrorHandler.error_msgs.keys())
-                subset.pop("eddrrm")
+                subset = list(VaspErrorHandler().error_msgs.keys())
+                subset.remove("eddrmm")
 
                 handler = VaspErrorHandler(errors_subset_to_catch=subset)
                 ```
+            vtst_fixes (bool): Whether to consider VTST optimizers. Defaults to
+                False for compatibility purposes, but if you have VTST, you
+                would likely benefit from setting this to True.
         """
         self.output_filename = output_filename
         self.errors = set()
         self.error_count = Counter()
         self.errors_subset_to_catch = errors_subset_to_catch or list(VaspErrorHandler.error_msgs.keys())
         self.vtst_fixes = vtst_fixes
         self.logger = logging.getLogger(self.__class__.__name__)
@@ -1247,15 +1247,15 @@
         incar = Incar.from_file("INCAR")
         try:
             outcar = Outcar("OUTCAR")
         except Exception:
             # Can't perform check if Outcar not valid
             return False
 
-        if incar.get("ISMEAR", 0) > 0:
+        if incar.get("ISMEAR", 1) > 0:
             # Read the latest entropy term.
             outcar.read_pattern(
                 {"entropy": r"entropy T\*S.*= *(\D\d*\.\d*)"}, postprocess=float, reverse=True, terminate_on_match=True
             )
             n_atoms = Structure.from_file("POSCAR").num_sites
             if outcar.data.get("entropy", []):
                 entropy_per_atom = abs(np.max(outcar.data.get("entropy"))) / n_atoms
@@ -1281,14 +1281,23 @@
         if sigma > 0.08:
             actions.append(
                 {
                     "dict": "INCAR",
                     "action": {"_set": {"SIGMA": sigma - 0.06}},
                 }
             )
+        else:
+            # https://vasp.at/wiki/index.php/ISMEAR recommends ISMEAR = 0 if you have
+            # no a priori knowledge of your system ("then always use Gaussian smearing"
+            actions.append(
+                {
+                    "dict": "INCAR",
+                    "action": {"_set": {"ISMEAR": 0, "SIGMA": 0.05}},
+                }
+            )
 
         VaspModder(vi=vi).apply_actions(actions)
         return {"errors": ["LargeSigma"], "actions": actions}
 
 
 class PotimErrorHandler(ErrorHandler):
     """
```

### Comparing `custodian-2023.6.5/custodian/vasp/interpreter.py` & `custodian-2023.7.22/custodian/vasp/interpreter.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian/vasp/jobs.py` & `custodian-2023.7.22/custodian/vasp/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,24 +135,24 @@
                 where the CHGCAR and WAVECAR are sometimes deleted (due to
                 changes in fft grid, etc.). Only applies to non-final runs.
             auto_continue (bool): Whether to automatically continue a run
                 if a STOPCAR is present. This is very useful if using the
                 wall-time handler which will write a read-only STOPCAR to
                 prevent VASP from deleting it once it finishes
         """
-        self.vasp_cmd = vasp_cmd
+        self.vasp_cmd = tuple(vasp_cmd)
         self.output_file = output_file
         self.stderr_file = stderr_file
         self.final = final
         self.backup = backup
         self.suffix = suffix
         self.settings_override = settings_override
         self.auto_npar = auto_npar
         self.auto_gamma = auto_gamma
-        self.gamma_vasp_cmd = gamma_vasp_cmd
+        self.gamma_vasp_cmd = tuple(gamma_vasp_cmd) if gamma_vasp_cmd else None
         self.copy_magmom = copy_magmom
         self.auto_continue = auto_continue
 
         if SENTRY_DSN:
             # if using Sentry logging, add specific VASP executable to scope
             from sentry_sdk import configure_scope
 
@@ -242,15 +242,15 @@
         """
         cmd = list(self.vasp_cmd)
         if self.auto_gamma:
             vi = VaspInput.from_directory(".")
             kpts = vi["KPOINTS"]
             if kpts is not None:
                 if kpts.style == Kpoints.supported_modes.Gamma and tuple(kpts.kpts[0]) == (1, 1, 1):
-                    if self.gamma_vasp_cmd is not None and which(self.gamma_vasp_cmd[-1]):
+                    if self.gamma_vasp_cmd is not None and which(self.gamma_vasp_cmd[-1]):  # pylint: disable=E1136
                         cmd = self.gamma_vasp_cmd
                     elif which(cmd[-1] + ".gamma"):
                         cmd[-1] += ".gamma"
         logger.info(f"Running {' '.join(cmd)}")
         with open(self.output_file, "w") as f_std, open(self.stderr_file, "w", buffering=1) as f_err:
             # use line buffering for stderr
             return subprocess.Popen(cmd, stdout=f_std, stderr=f_err, start_new_session=True)  # pylint: disable=R1732
@@ -661,43 +661,47 @@
         with open("EOS.txt", "w") as f:
             f.write(f"# {lattice_direction} energy\n")
             for k in sorted(energies.keys()):
                 f.write(f"{k} {energies[k]}\n")
 
     def terminate(self):
         """
-        Kill all vasp processes associated with the current job.
+        Kill all VASP processes associated with the current job.
         This is done by looping over all processes and selecting the ones
-        that contain "vasp" as well as access files (CHGCAR in particular)
+        that contain "vasp" as well as access files (vasprun.xml in particular)
         in the custodian working directory.
-        There is also a safety that kills all vasp processes if non of the
-        processes can be killed (This is bad if more than one vasp runs are
+        There is also a safety that kills all VASP processes if none of the
+        processes can be killed (This is bad if more than one VASP runs are
         simultaneously executed on the same node). However, this should never
         happen.
         """
         workdir = os.getcwd()
-        logger.info(f"kill vasp processes in work dir {workdir}")
-        is_killed = False
+        logger.info(f"Killing VASP processes in workdir {workdir}.")
         for proc in psutil.process_iter():
             try:
                 if "vasp" in proc.name().lower():
-                    for file in proc.open_files():
-                        if workdir + "/CHGCAR" == file.path and psutil.pid_exists(proc.pid):
-                            proc.kill()
-                            is_killed = True
-            except (psutil.NoSuchProcess, psutil.AccessDenied):
+                    open_paths = [file.path for file in proc.open_files()]
+                    vasprun_path = os.path.join(workdir, "vasprun.xml")
+                    if (vasprun_path in open_paths) and psutil.pid_exists(proc.pid):
+                        proc.kill()
+                        return
+            except (psutil.NoSuchProcess, psutil.AccessDenied) as e:
+                logger.warning(f"Exception {e} encountered while killing VASP.")
                 continue
-        if not is_killed:
-            logger.warning(f"killing vasp processes in work dir {workdir} failed. Resorting to 'killall'.")
-            cmds = self.vasp_cmd
-            if self.gamma_vasp_cmd:
-                cmds += self.gamma_vasp_cmd
-                for k in cmds:
-                    if "vasp" in k:
-                        subprocess.run(["killall", f"{k}"])
+
+        logger.warning(
+            f"Killing VASP processes in workdir {workdir} failed with subprocess.Popen.terminate(). "
+            "Resorting to 'killall'."
+        )
+        cmds = self.vasp_cmd
+        if self.gamma_vasp_cmd:
+            cmds += self.gamma_vasp_cmd
+        for k in cmds:
+            if "vasp" in k:
+                subprocess.run(["killall", f"{k}"])
 
 
 class VaspNEBJob(VaspJob):
     """
     A NEB vasp job, especially for CI-NEB running at PBS clusters.
     The class is added for the purpose of handling a different folder
     arrangement in NEB calculation.
@@ -766,24 +770,24 @@
                 runs and to copy the CONTCAR to the POSCAR, you will provide::
 
                     [{"dict": "INCAR", "action": {"_set": {"ISTART": 1}}},
                      {"file": "CONTCAR",
                       "action": {"_file_copy": {"dest": "POSCAR"}}}]
         """
 
-        self.vasp_cmd = vasp_cmd
+        self.vasp_cmd = tuple(vasp_cmd)
         self.output_file = output_file
         self.stderr_file = stderr_file
         self.final = final
         self.backup = backup
         self.suffix = suffix
         self.auto_npar = auto_npar
         self.half_kpts = half_kpts
         self.auto_gamma = auto_gamma
-        self.gamma_vasp_cmd = gamma_vasp_cmd
+        self.gamma_vasp_cmd = tuple(gamma_vasp_cmd) if gamma_vasp_cmd else None
         self.auto_continue = auto_continue
         self.settings_override = settings_override
         self.neb_dirs = []  # 00, 01, etc.
         self.neb_sub = []  # 01, 02, etc.
 
         for path in os.listdir("."):
             if os.path.isdir(path) and path.isdigit():
@@ -860,15 +864,15 @@
         if self.auto_gamma:
             kpts = Kpoints.from_file("KPOINTS")
             if kpts.style == Kpoints.supported_modes.Gamma and tuple(kpts.kpts[0]) == (
                 1,
                 1,
                 1,
             ):
-                if self.gamma_vasp_cmd is not None and which(self.gamma_vasp_cmd[-1]):
+                if self.gamma_vasp_cmd is not None and which(self.gamma_vasp_cmd[-1]):  # pylint: disable=E1136
                     cmd = self.gamma_vasp_cmd
                 elif which(cmd[-1] + ".gamma"):
                     cmd[-1] += ".gamma"
         logger.info(f"Running {' '.join(cmd)}")
         with open(self.output_file, "w") as f_std, open(self.stderr_file, "w", buffering=1) as f_err:
             # Use line buffering for stderr
             return subprocess.Popen(cmd, stdout=f_std, stderr=f_err, start_new_session=True)  # pylint: disable=R1732
```

### Comparing `custodian-2023.6.5/custodian/vasp/validators.py` & `custodian-2023.7.22/custodian/vasp/validators.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/custodian.egg-info/PKG-INFO` & `custodian-2023.7.22/custodian.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custodian
-Version: 2023.6.5
+Version: 2023.7.22
 Summary: A simple JIT job management framework in Python.
 Home-page: https://github.com/materialsproject/custodian
 Author: Shyue Ping Ong, William Davidson Richards, Stephen Dacek, Xiaohui Qu, Matthew Horton, Samuel M. Blau
 Author-email: ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 License: MIT
 Keywords: jit,just-in-time,job,management,vasp
```

### Comparing `custodian-2023.6.5/custodian.egg-info/SOURCES.txt` & `custodian-2023.7.22/custodian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/setup.cfg` & `custodian-2023.7.22/setup.cfg`

 * *Files identical despite different names*

### Comparing `custodian-2023.6.5/setup.py` & `custodian-2023.7.22/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     long_desc = f.read()
     ind = long_desc.find("\n")
     long_desc = long_desc[ind + 1 :]
 
 setup(
     name="custodian",
     packages=find_packages(),
-    version="2023.6.5",
-    install_requires=["monty>=2.0.6", "ruamel.yaml>=0.15.6", "sentry-sdk>=0.8.0"],
+    version="2023.7.22",
+    install_requires=["monty>=2.0.6", "ruamel.yaml>=0.15.6", "sentry-sdk>=0.8.0", "psutil"],
     extras_require={"vasp, nwchem, qchem": ["pymatgen>=2019.8.23"]},
     package_data={},
     author="Shyue Ping Ong, William Davidson Richards, Stephen Dacek, Xiaohui Qu, Matthew Horton, Samuel M. Blau",
     author_email="ongsp@ucsd.edu",
     maintainer="Shyue Ping Ong",
     url="https://github.com/materialsproject/custodian",
     license="MIT",
```

