# Comparing `tmp/gen3_util-0.0.4rc6.tar.gz` & `tmp/gen3_util-0.0.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_util-0.0.4rc6.tar", last modified: Fri Jul 21 21:39:56 2023, max compression
+gzip compressed data, was "gen3_util-0.0.5rc1.tar", last modified: Wed Jul 19 18:49:30 2023, max compression
```

## Comparing `gen3_util-0.0.4rc6.tar` & `gen3_util-0.0.5rc1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-21 21:39:56.526562 gen3_util-0.0.4rc6/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.4rc6/LICENSE
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     9640 2023-07-21 21:39:56.526233 gen3_util-0.0.4rc6/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     8955 2023-07-19 00:41:02.000000 gen3_util-0.0.4rc6/README.md
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-21 21:39:56.334974 gen3_util-0.0.4rc6/gen3_util/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       71 2023-07-05 18:55:42.000000 gen3_util-0.0.4rc6/gen3_util/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-21 21:39:56.346976 gen3_util-0.0.4rc6/gen3_util/access/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2321 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc6/gen3_util/access/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4021 2023-07-21 21:17:57.000000 gen3_util-0.0.4rc6/gen3_util/access/cli.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-21 21:39:56.347730 gen3_util-0.0.4rc6/gen3_util/access/policies/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc6/gen3_util/access/policies/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5687 2023-07-19 00:41:02.000000 gen3_util-0.0.4rc6/gen3_util/access/requestor.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-21 21:39:56.354854 gen3_util-0.0.4rc6/gen3_util/buckets/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      803 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc6/gen3_util/buckets/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      629 2023-06-21 17:42:54.000000 gen3_util-0.0.4rc6/gen3_util/buckets/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      474 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc6/gen3_util/buckets/lister.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-21 21:39:56.357716 gen3_util-0.0.4rc6/gen3_util/cli/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4637 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc6/gen3_util/cli/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1667 2023-06-21 17:42:54.000000 gen3_util-0.0.4rc6/gen3_util/cli/cli.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-21 21:39:56.358443 gen3_util-0.0.4rc6/gen3_util/common/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5317 2023-07-21 21:17:57.000000 gen3_util-0.0.4rc6/gen3_util/common/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-21 21:39:56.364486 gen3_util-0.0.4rc6/gen3_util/config/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2824 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc6/gen3_util/config/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      433 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc6/gen3_util/config/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      503 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc6/gen3_util/config/config.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-21 21:39:56.392457 gen3_util-0.0.4rc6/gen3_util/files/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1285 2023-06-21 17:42:55.000000 gen3_util-0.0.4rc6/gen3_util/files/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2437 2023-07-17 22:26:17.000000 gen3_util-0.0.4rc6/gen3_util/files/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      938 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc6/gen3_util/files/downloader.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      192 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc6/gen3_util/files/lister.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      202 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc6/gen3_util/files/remover.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    13121 2023-07-19 00:41:02.000000 gen3_util-0.0.4rc6/gen3_util/files/uploader.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-21 21:39:56.479303 gen3_util-0.0.4rc6/gen3_util/meta/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4101 2023-07-07 00:01:20.000000 gen3_util-0.0.4rc6/gen3_util/meta/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2256 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc6/gen3_util/meta/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      323 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc6/gen3_util/meta/downloader.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    11295 2023-07-20 00:34:28.000000 gen3_util-0.0.4rc6/gen3_util/meta/importer.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      329 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc6/gen3_util/meta/lister.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      201 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc6/gen3_util/meta/remover.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3858 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc6/gen3_util/meta/uploader.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3299 2023-07-11 21:14:30.000000 gen3_util-0.0.4rc6/gen3_util/meta/validator.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-21 21:39:56.490264 gen3_util-0.0.4rc6/gen3_util/projects/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2247 2023-06-21 17:42:55.000000 gen3_util-0.0.4rc6/gen3_util/projects/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2769 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc6/gen3_util/projects/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1901 2023-06-30 03:26:36.000000 gen3_util-0.0.4rc6/gen3_util/projects/creator.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      793 2023-06-21 17:42:55.000000 gen3_util-0.0.4rc6/gen3_util/projects/lister.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1078 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc6/gen3_util/projects/remover.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-21 21:39:56.344233 gen3_util-0.0.4rc6/gen3_util.egg-info/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     9640 2023-07-21 21:39:56.000000 gen3_util-0.0.4rc6/gen3_util.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1687 2023-07-21 21:39:56.000000 gen3_util-0.0.4rc6/gen3_util.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        1 2023-07-21 21:39:56.000000 gen3_util-0.0.4rc6/gen3_util.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       53 2023-07-21 21:39:56.000000 gen3_util-0.0.4rc6/gen3_util.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      141 2023-07-21 21:39:56.000000 gen3_util-0.0.4rc6/gen3_util.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       16 2023-07-21 21:39:56.000000 gen3_util-0.0.4rc6/gen3_util.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       38 2023-07-21 21:39:56.526627 gen3_util-0.0.4rc6/setup.cfg
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5579 2023-07-21 21:39:32.000000 gen3_util-0.0.4rc6/setup.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-21 21:39:56.327253 gen3_util-0.0.4rc6/tests/
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-21 21:39:56.521710 gen3_util-0.0.4rc6/tests/integration/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc6/tests/integration/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      275 2023-07-19 00:41:02.000000 gen3_util-0.0.4rc6/tests/integration/conftest.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4358 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc6/tests/integration/test_access.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      454 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc6/tests/integration/test_buckets.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      243 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc6/tests/integration/test_config.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2089 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc6/tests/integration/test_files.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5134 2023-07-19 00:41:02.000000 gen3_util-0.0.4rc6/tests/integration/test_meta.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1237 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc6/tests/integration/test_project.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-21 21:39:56.525056 gen3_util-0.0.4rc6/tests/unit/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc6/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      322 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc6/tests/unit/conftest.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-21 21:39:56.525533 gen3_util-0.0.4rc6/tests/unit/plugins/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc6/tests/unit/plugins/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-21 21:39:56.525764 gen3_util-0.0.4rc6/tests/unit/plugins/gen3_util_plugin_foo/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1450 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc6/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3380 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc6/tests/unit/test_cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      565 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc6/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      551 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc6/tests/unit/test_config.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2350 2023-07-19 00:41:02.000000 gen3_util-0.0.4rc6/tests/unit/test_files.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4616 2023-07-07 18:51:14.000000 gen3_util-0.0.4rc6/tests/unit/test_meta.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc6/tests/unit/test_validate_directory.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 18:49:30.599085 gen3_util-0.0.5rc1/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.5rc1/LICENSE
+-rw-r--r--   0 walsbr   (320923486) 1971611142     9640 2023-07-19 18:49:30.598801 gen3_util-0.0.5rc1/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     8955 2023-07-19 00:41:02.000000 gen3_util-0.0.5rc1/README.md
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 18:49:30.567362 gen3_util-0.0.5rc1/gen3_util/
+-rw-r--r--   0 walsbr   (320923486) 1971611142       71 2023-07-05 18:55:42.000000 gen3_util-0.0.5rc1/gen3_util/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 18:49:30.579296 gen3_util-0.0.5rc1/gen3_util/access/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2321 2023-07-07 00:00:20.000000 gen3_util-0.0.5rc1/gen3_util/access/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4281 2023-07-07 00:45:48.000000 gen3_util-0.0.5rc1/gen3_util/access/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 18:49:30.580839 gen3_util-0.0.5rc1/gen3_util/access/policies/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:00:20.000000 gen3_util-0.0.5rc1/gen3_util/access/policies/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5687 2023-07-19 00:41:02.000000 gen3_util-0.0.5rc1/gen3_util/access/requestor.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 18:49:30.583483 gen3_util-0.0.5rc1/gen3_util/buckets/
+-rw-r--r--   0 walsbr   (320923486) 1971611142      803 2023-05-10 23:31:00.000000 gen3_util-0.0.5rc1/gen3_util/buckets/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      629 2023-06-21 17:42:54.000000 gen3_util-0.0.5rc1/gen3_util/buckets/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      474 2023-05-10 23:31:00.000000 gen3_util-0.0.5rc1/gen3_util/buckets/lister.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 18:49:30.584315 gen3_util-0.0.5rc1/gen3_util/cli/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4637 2023-07-07 00:00:20.000000 gen3_util-0.0.5rc1/gen3_util/cli/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1667 2023-06-21 17:42:54.000000 gen3_util-0.0.5rc1/gen3_util/cli/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 18:49:30.584619 gen3_util-0.0.5rc1/gen3_util/common/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5262 2023-07-07 00:45:48.000000 gen3_util-0.0.5rc1/gen3_util/common/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 18:49:30.585419 gen3_util-0.0.5rc1/gen3_util/config/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2824 2023-07-07 00:00:20.000000 gen3_util-0.0.5rc1/gen3_util/config/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      433 2023-06-28 20:29:46.000000 gen3_util-0.0.5rc1/gen3_util/config/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-10 23:31:00.000000 gen3_util-0.0.5rc1/gen3_util/config/config.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 18:49:30.587127 gen3_util-0.0.5rc1/gen3_util/files/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1285 2023-06-21 17:42:55.000000 gen3_util-0.0.5rc1/gen3_util/files/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2437 2023-07-17 22:26:17.000000 gen3_util-0.0.5rc1/gen3_util/files/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      938 2023-07-07 00:00:20.000000 gen3_util-0.0.5rc1/gen3_util/files/downloader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      192 2023-05-10 23:31:00.000000 gen3_util-0.0.5rc1/gen3_util/files/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      202 2023-05-10 23:31:00.000000 gen3_util-0.0.5rc1/gen3_util/files/remover.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    13121 2023-07-19 00:41:02.000000 gen3_util-0.0.5rc1/gen3_util/files/uploader.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 18:49:30.592952 gen3_util-0.0.5rc1/gen3_util/meta/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4101 2023-07-07 00:01:20.000000 gen3_util-0.0.5rc1/gen3_util/meta/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2256 2023-07-07 00:00:20.000000 gen3_util-0.0.5rc1/gen3_util/meta/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      323 2023-07-07 00:00:20.000000 gen3_util-0.0.5rc1/gen3_util/meta/downloader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    11615 2023-07-19 18:48:10.000000 gen3_util-0.0.5rc1/gen3_util/meta/importer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      329 2023-07-07 00:00:20.000000 gen3_util-0.0.5rc1/gen3_util/meta/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      201 2023-05-10 23:31:00.000000 gen3_util-0.0.5rc1/gen3_util/meta/remover.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3858 2023-07-07 00:00:20.000000 gen3_util-0.0.5rc1/gen3_util/meta/uploader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3299 2023-07-11 21:14:30.000000 gen3_util-0.0.5rc1/gen3_util/meta/validator.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 18:49:30.594147 gen3_util-0.0.5rc1/gen3_util/projects/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2247 2023-06-21 17:42:55.000000 gen3_util-0.0.5rc1/gen3_util/projects/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2769 2023-07-07 00:00:20.000000 gen3_util-0.0.5rc1/gen3_util/projects/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1901 2023-06-30 03:26:36.000000 gen3_util-0.0.5rc1/gen3_util/projects/creator.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      793 2023-06-21 17:42:55.000000 gen3_util-0.0.5rc1/gen3_util/projects/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1078 2023-06-28 20:29:46.000000 gen3_util-0.0.5rc1/gen3_util/projects/remover.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 18:49:30.572753 gen3_util-0.0.5rc1/gen3_util.egg-info/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     9640 2023-07-19 18:49:30.000000 gen3_util-0.0.5rc1/gen3_util.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1687 2023-07-19 18:49:30.000000 gen3_util-0.0.5rc1/gen3_util.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-07-19 18:49:30.000000 gen3_util-0.0.5rc1/gen3_util.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       53 2023-07-19 18:49:30.000000 gen3_util-0.0.5rc1/gen3_util.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142      141 2023-07-19 18:49:30.000000 gen3_util-0.0.5rc1/gen3_util.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       16 2023-07-19 18:49:30.000000 gen3_util-0.0.5rc1/gen3_util.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-07-19 18:49:30.599161 gen3_util-0.0.5rc1/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5579 2023-07-19 18:47:51.000000 gen3_util-0.0.5rc1/setup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 18:49:30.564822 gen3_util-0.0.5rc1/tests/
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 18:49:30.595894 gen3_util-0.0.5rc1/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.5rc1/tests/integration/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      275 2023-07-19 00:41:02.000000 gen3_util-0.0.5rc1/tests/integration/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4358 2023-07-07 00:45:48.000000 gen3_util-0.0.5rc1/tests/integration/test_access.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      454 2023-06-28 20:29:46.000000 gen3_util-0.0.5rc1/tests/integration/test_buckets.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      243 2023-06-28 20:29:46.000000 gen3_util-0.0.5rc1/tests/integration/test_config.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2089 2023-07-07 00:00:20.000000 gen3_util-0.0.5rc1/tests/integration/test_files.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5134 2023-07-19 00:41:02.000000 gen3_util-0.0.5rc1/tests/integration/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1237 2023-07-07 00:00:20.000000 gen3_util-0.0.5rc1/tests/integration/test_project.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 18:49:30.597962 gen3_util-0.0.5rc1/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.5rc1/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      322 2023-05-05 20:31:25.000000 gen3_util-0.0.5rc1/tests/unit/conftest.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 18:49:30.598263 gen3_util-0.0.5rc1/tests/unit/plugins/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:45:48.000000 gen3_util-0.0.5rc1/tests/unit/plugins/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 18:49:30.598502 gen3_util-0.0.5rc1/tests/unit/plugins/gen3_util_plugin_foo/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1450 2023-07-07 00:45:48.000000 gen3_util-0.0.5rc1/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3380 2023-07-07 00:00:20.000000 gen3_util-0.0.5rc1/tests/unit/test_cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_util-0.0.5rc1/tests/unit/test_coding_conventions.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      551 2023-05-05 20:31:25.000000 gen3_util-0.0.5rc1/tests/unit/test_config.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2350 2023-07-19 00:41:02.000000 gen3_util-0.0.5rc1/tests/unit/test_files.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4616 2023-07-07 18:51:14.000000 gen3_util-0.0.5rc1/tests/unit/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.5rc1/tests/unit/test_validate_directory.py
```

### Comparing `gen3_util-0.0.4rc6/LICENSE` & `gen3_util-0.0.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/PKG-INFO` & `gen3_util-0.0.5rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3_util
-Version: 0.0.4rc6
+Version: 0.0.5rc1
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
```

### Comparing `gen3_util-0.0.4rc6/README.md` & `gen3_util-0.0.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/access/__init__.py` & `gen3_util-0.0.5rc1/gen3_util/access/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/access/cli.py` & `gen3_util-0.0.5rc1/gen3_util/access/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 def access_group(config: Config):
     """Manage access requests."""
     pass
 
 
 @access_group.command(name="touch")
 @click.argument('user_name')
-@click.argument('project_id')
+@click.option('--project_id', show_default=True, default=None, help='add a project id ex: --project_id aced-Alcoholism')
+@click.option('--resource_path',  show_default=True, default=None, help='add resource paths ex: --resource_path /programs/aced/projects/Alcoholism')
 @click.option('--roles', show_default=True, default=None, help='Add comma-delimited role permissions to the access request, ex: --roles "storage_writer,file_uploader"')
 @click.pass_obj
-def access_touch(config: Config,  user_name: str, project_id: str, roles: str):
+def access_touch(config: Config,  user_name: str, project_id: str, resource_path: str, roles: str):
     """Create a request for read access.
 
     \b
     USER_NAME (str): user's email
     PROJECT_ID or RESOURCE_PATH: <program-name>-<project-name> or /resource/path
 
     """
```

### Comparing `gen3_util-0.0.4rc6/gen3_util/access/requestor.py` & `gen3_util-0.0.5rc1/gen3_util/access/requestor.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/buckets/__init__.py` & `gen3_util-0.0.5rc1/gen3_util/buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/buckets/cli.py` & `gen3_util-0.0.5rc1/gen3_util/buckets/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/cli/__init__.py` & `gen3_util-0.0.5rc1/gen3_util/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/cli/cli.py` & `gen3_util-0.0.5rc1/gen3_util/cli/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/common/__init__.py` & `gen3_util-0.0.5rc1/gen3_util/common/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,11 +169,10 @@
     except EmailNotValidError as e:
         msgs.append(f"{email} is not a valid email address. {e}")
     return msgs
 
 
 def to_resource_path(project_id):
     """Canonical conversion of project_id to resource path."""
-    if '-' not in project_id:
-        return project_id
+
     _ = project_id.split('-')
     return f"/programs/{_[0]}/projects/{_[1]}"
```

### Comparing `gen3_util-0.0.4rc6/gen3_util/config/__init__.py` & `gen3_util-0.0.5rc1/gen3_util/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/files/__init__.py` & `gen3_util-0.0.5rc1/gen3_util/files/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/files/cli.py` & `gen3_util-0.0.5rc1/gen3_util/files/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/files/downloader.py` & `gen3_util-0.0.5rc1/gen3_util/files/downloader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/files/uploader.py` & `gen3_util-0.0.5rc1/gen3_util/files/uploader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/meta/__init__.py` & `gen3_util-0.0.5rc1/gen3_util/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/meta/cli.py` & `gen3_util-0.0.5rc1/gen3_util/meta/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/meta/importer.py` & `gen3_util-0.0.5rc1/gen3_util/meta/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,21 +144,31 @@
 
         count = 0
         size = 0
         already_seen = set()
         for file in input_path.glob(pattern):
             if file.is_dir():
                 continue
+            if file.is_symlink():
+                logger.info(f"Skipping symlink {file}")
+                continue
+
+            try:
+                resources = _extract_fhir_resources(str(file).replace(remove_path_prefix, '', 1), input_path, plugin_path)
+            except ValueError:
+                # expected error if plugin does not want to process this file
+                logger.info(f"Skipping {file}")
+                continue
+
             stat = file.stat()
             modified = datetime.fromtimestamp(stat.st_mtime, tz=timezone.utc)
             mime, encoding = mimetypes.guess_type(file)
             if not mime:
                 mime = _magic.from_file(file)
 
-            resources = _extract_fhir_resources(str(file).replace(remove_path_prefix, '', 1), input_path, plugin_path)
             subject_reference = f"ResearchStudy/{research_study['id']}"  # Who/what is the subject of the document
 
             for resource in resources:
                 if resource.id in already_seen:
                     continue
 
                 if resource.resource_type == 'Patient':
```

### Comparing `gen3_util-0.0.4rc6/gen3_util/meta/uploader.py` & `gen3_util-0.0.5rc1/gen3_util/meta/uploader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/meta/validator.py` & `gen3_util-0.0.5rc1/gen3_util/meta/validator.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/projects/__init__.py` & `gen3_util-0.0.5rc1/gen3_util/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/projects/cli.py` & `gen3_util-0.0.5rc1/gen3_util/projects/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/projects/creator.py` & `gen3_util-0.0.5rc1/gen3_util/projects/creator.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/projects/lister.py` & `gen3_util-0.0.5rc1/gen3_util/projects/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util/projects/remover.py` & `gen3_util-0.0.5rc1/gen3_util/projects/remover.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/gen3_util.egg-info/PKG-INFO` & `gen3_util-0.0.5rc1/gen3_util.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3-util
-Version: 0.0.4rc6
+Version: 0.0.5rc1
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
```

### Comparing `gen3_util-0.0.4rc6/gen3_util.egg-info/SOURCES.txt` & `gen3_util-0.0.5rc1/gen3_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/setup.py` & `gen3_util-0.0.5rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='gen3_util',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.4rc6',  # Required
+    version='0.0.5rc1',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Commons utilities',
     # Optional
```

### Comparing `gen3_util-0.0.4rc6/tests/integration/test_access.py` & `gen3_util-0.0.5rc1/tests/integration/test_access.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/tests/integration/test_files.py` & `gen3_util-0.0.5rc1/tests/integration/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/tests/integration/test_meta.py` & `gen3_util-0.0.5rc1/tests/integration/test_meta.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/tests/integration/test_project.py` & `gen3_util-0.0.5rc1/tests/integration/test_project.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/tests/unit/plugins/gen3_util_plugin_foo/__init__.py` & `gen3_util-0.0.5rc1/tests/unit/plugins/gen3_util_plugin_foo/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/tests/unit/test_cli.py` & `gen3_util-0.0.5rc1/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/tests/unit/test_coding_conventions.py` & `gen3_util-0.0.5rc1/tests/unit/test_coding_conventions.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/tests/unit/test_config.py` & `gen3_util-0.0.5rc1/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/tests/unit/test_files.py` & `gen3_util-0.0.5rc1/tests/unit/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/tests/unit/test_meta.py` & `gen3_util-0.0.5rc1/tests/unit/test_meta.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc6/tests/unit/test_validate_directory.py` & `gen3_util-0.0.5rc1/tests/unit/test_validate_directory.py`

 * *Files identical despite different names*

