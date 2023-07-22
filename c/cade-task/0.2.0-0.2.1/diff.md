# Comparing `tmp/cade_task-0.2.0.tar.gz` & `tmp/cade_task-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cade_task-0.2.0.tar", max compression
+gzip compressed data, was "cade_task-0.2.1.tar", max compression
```

## Comparing `cade_task-0.2.0.tar` & `cade_task-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-06-22 21:56:01.797435 cade_task-0.2.0/LICENSE
--rw-r--r--   0        0        0        0 2023-07-18 17:17:25.645802 cade_task-0.2.0/cade_task/__init__.py
--rw-r--r--   0        0        0       61 2023-07-18 17:17:25.646114 cade_task-0.2.0/cade_task/__main__.py
--rw-r--r--   0        0        0     3889 2023-07-18 17:17:25.646439 cade_task-0.2.0/cade_task/cli.py
--rw-r--r--   0        0        0     2772 2023-07-18 17:17:25.646697 cade_task-0.2.0/cade_task/lib.py
--rw-r--r--   0        0        0      443 2023-07-18 17:17:25.647301 cade_task-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 cade_task-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-22 21:56:01.797435 cade_task-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3129 2023-07-18 17:48:03.192515 cade_task-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-18 17:17:25.645802 cade_task-0.2.1/cade_task/__init__.py
+-rw-r--r--   0        0        0       61 2023-07-18 17:17:25.646114 cade_task-0.2.1/cade_task/__main__.py
+-rw-r--r--   0        0        0     3889 2023-07-18 17:17:25.646439 cade_task-0.2.1/cade_task/cli.py
+-rw-r--r--   0        0        0     2772 2023-07-18 17:17:25.646697 cade_task-0.2.1/cade_task/lib.py
+-rw-r--r--   0        0        0      535 2023-07-19 02:12:15.658884 cade_task-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 cade_task-0.2.1/PKG-INFO
```

### Comparing `cade_task-0.2.0/LICENSE` & `cade_task-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cade_task-0.2.0/cade_task/cli.py` & `cade_task-0.2.1/cade_task/cli.py`

 * *Files identical despite different names*

### Comparing `cade_task-0.2.0/cade_task/lib.py` & `cade_task-0.2.1/cade_task/lib.py`

 * *Files identical despite different names*

