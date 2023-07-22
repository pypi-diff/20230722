# Comparing `tmp/ijson-3.2.2.tar.gz` & `tmp/ijson-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ijson-3.2.2.tar", last modified: Thu Jun 22 03:59:36 2023, max compression
+gzip compressed data, was "dist/ijson-3.2.3.tar", last modified: Sat Jul 22 05:17:12 2023, max compression
```

## Comparing `ijson-3.2.2.tar` & `ijson-3.2.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:59:36.000000 ijson-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-06-22 03:59:33.000000 ijson-3.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-22 03:59:33.000000 ijson-3.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-22 03:59:33.000000 ijson-3.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25721 2023-06-22 03:59:36.000000 ijson-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-06-22 03:59:33.000000 ijson-3.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:59:36.000000 ijson-3.2.2/ijson/
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:59:36.000000 ijson-3.2.2/ijson/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/_yajl2_ctypes_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:59:36.000000 ijson-3.2.2/ijson/backends/yajl2_c/
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/async_reading_generator.c
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/async_reading_generator.h
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/basic_parse.c
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/basic_parse.h
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/basic_parse_async.c
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/basic_parse_async.h
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/basic_parse_basecoro.c
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/basic_parse_basecoro.h
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/builder.h
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/coro_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/coro_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/items.c
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/items.h
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/items_async.c
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/items_async.h
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/items_basecoro.c
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/items_basecoro.h
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/kvitems.c
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/kvitems.h
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/kvitems_async.c
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/kvitems_async.h
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/kvitems_basecoro.c
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/kvitems_basecoro.h
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/module.c
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/parse.c
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/parse.h
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/parse_async.c
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/parse_async.h
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/parse_basecoro.c
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/parse_basecoro.h
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/reading_generator.c
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c/reading_generator.h
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_c.py
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/backends/yajl2_cffi.py
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/utils35.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 03:59:33.000000 ijson-3.2.2/ijson/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:59:36.000000 ijson-3.2.2/ijson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25721 2023-06-22 03:59:36.000000 ijson-3.2.2/ijson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-22 03:59:36.000000 ijson-3.2.2/ijson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 03:59:36.000000 ijson-3.2.2/ijson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 03:59:36.000000 ijson-3.2.2/ijson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 03:59:36.000000 ijson-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-06-22 03:59:33.000000 ijson-3.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:59:36.000000 ijson-3.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:59:33.000000 ijson-3.2.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-22 03:59:33.000000 ijson-3.2.2/test/_test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-22 03:59:33.000000 ijson-3.2.2/test/_test_async_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 03:59:33.000000 ijson-3.2.2/test/_test_async_types_coroutine.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-22 03:59:33.000000 ijson-3.2.2/test/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-22 03:59:33.000000 ijson-3.2.2/test/test_async_types_coroutines.py
--rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-06-22 03:59:33.000000 ijson-3.2.2/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-22 03:59:33.000000 ijson-3.2.2/test/test_coroutines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-22 03:59:33.000000 ijson-3.2.2/test/test_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-22 03:59:33.000000 ijson-3.2.2/test/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-22 03:59:33.000000 ijson-3.2.2/test/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-22 03:59:33.000000 ijson-3.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:17:12.000000 ijson-3.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-07-22 05:17:10.000000 ijson-3.2.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-22 05:17:10.000000 ijson-3.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-22 05:17:10.000000 ijson-3.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25721 2023-07-22 05:17:12.000000 ijson-3.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-07-22 05:17:10.000000 ijson-3.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:17:12.000000 ijson-3.2.3/ijson/
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:17:12.000000 ijson-3.2.3/ijson/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/_yajl2_ctypes_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:17:12.000000 ijson-3.2.3/ijson/backends/yajl2_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/async_reading_generator.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/async_reading_generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/basic_parse.c
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/basic_parse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/basic_parse_async.c
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/basic_parse_async.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/basic_parse_basecoro.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/basic_parse_basecoro.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/builder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/coro_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/coro_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/items.c
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/items.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/items_async.c
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/items_async.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/items_basecoro.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/items_basecoro.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/kvitems.c
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/kvitems.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/kvitems_async.c
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/kvitems_async.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/kvitems_basecoro.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/kvitems_basecoro.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/parse.c
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/parse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/parse_async.c
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/parse_async.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/parse_basecoro.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/parse_basecoro.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/reading_generator.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c/reading_generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/backends/yajl2_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/utils35.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 05:17:10.000000 ijson-3.2.3/ijson/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:17:12.000000 ijson-3.2.3/ijson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25721 2023-07-22 05:17:12.000000 ijson-3.2.3/ijson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-22 05:17:12.000000 ijson-3.2.3/ijson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 05:17:12.000000 ijson-3.2.3/ijson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 05:17:12.000000 ijson-3.2.3/ijson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 05:17:12.000000 ijson-3.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-22 05:17:10.000000 ijson-3.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:17:12.000000 ijson-3.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 05:17:10.000000 ijson-3.2.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-22 05:17:10.000000 ijson-3.2.3/test/_test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-22 05:17:10.000000 ijson-3.2.3/test/_test_async_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-22 05:17:10.000000 ijson-3.2.3/test/_test_async_types_coroutine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-22 05:17:10.000000 ijson-3.2.3/test/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-22 05:17:10.000000 ijson-3.2.3/test/test_async_types_coroutines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-07-22 05:17:10.000000 ijson-3.2.3/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-22 05:17:10.000000 ijson-3.2.3/test/test_coroutines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-22 05:17:10.000000 ijson-3.2.3/test/test_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-22 05:17:10.000000 ijson-3.2.3/test/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-22 05:17:10.000000 ijson-3.2.3/test/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-22 05:17:10.000000 ijson-3.2.3/tox.ini
```

### Comparing `ijson-3.2.2/CHANGELOG.md` & `ijson-3.2.3/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,26 @@
 # Changelog
 
+## [3.2.3]
+
+* Fixed several issues in the ``yajl2_c`` backend
+  and its async generators
+  that were only made apparent
+  when running it with PyPy
+  and/or a CPython debug build (#101).
+  As part of that,
+  an issue was found and fixed in PyPy itself
+  affecting all versions up to 7.3.12,
+  so users will need to wait until the next version is released
+  to be able to use async generators
+  (https://foss.heptapod.net/pypy/pypy/-/issues/3956).
+* Adapted ``yajl2_c`` async generators
+  to work against PyPy shortcomings
+  (https://foss.heptapod.net/pypy/pypy/-/issues/3965).
+
 ## [3.2.2]
 
 * Fixed compilation and ``async`` support
   of the ``yajl2_c`` backend in pyhthon 3.12 (#98).
 * Check ``IJSON_BUILD_YAJL2C`` environment variable
   when building ijson
   to force/skip building the ``yajl2_c`` backend (#102).
@@ -313,7 +330,8 @@
 [3.1.2.post0]: https://github.com/ICRAR/ijson/releases/tag/v3.1.2.post0
 [3.1.3]: https://github.com/ICRAR/ijson/releases/tag/v3.1.3
 [3.1.4]: https://github.com/ICRAR/ijson/releases/tag/v3.1.4
 [3.2.0]: https://github.com/ICRAR/ijson/releases/tag/v3.2.0
 [3.2.0.post0]: https://github.com/ICRAR/ijson/releases/tag/v3.2.0.post0
 [3.2.1]: https://github.com/ICRAR/ijson/releases/tag/v3.2.1
 [3.2.2]: https://github.com/ICRAR/ijson/releases/tag/v3.2.2
+[3.2.3]: https://github.com/ICRAR/ijson/releases/tag/v3.2.3
```

### Comparing `ijson-3.2.2/LICENSE.txt` & `ijson-3.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/PKG-INFO` & `ijson-3.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ijson
-Version: 3.2.2
+Version: 3.2.3
 Summary: Iterative JSON parser with standard Python iterator interfaces
 Home-page: https://github.com/ICRAR/ijson
 Author: Rodrigo Tobar, Ivan Sagalaev
 Author-email: rtobar@icrar.org, maniac@softwaremaniacs.org
 License: BSD
 Description: .. image:: https://github.com/ICRAR/ijson/actions/workflows/deploy-to-pypi.yml/badge.svg
             :target: https://github.com/ICRAR/ijson/actions/workflows/deploy-to-pypi.yml
```

### Comparing `ijson-3.2.2/README.rst` & `ijson-3.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/__init__.py` & `ijson-3.2.3/ijson/__init__.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/__init__.py` & `ijson-3.2.3/ijson/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/_yajl2_ctypes_common.py` & `ijson-3.2.3/ijson/backends/_yajl2_ctypes_common.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/python.py` & `ijson-3.2.3/ijson/backends/python.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl.py` & `ijson-3.2.3/ijson/backends/yajl.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2.py` & `ijson-3.2.3/ijson/backends/yajl2.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/async_reading_generator.c` & `ijson-3.2.3/ijson/backends/yajl2_c/async_reading_generator.c`

 * *Files 10% similar despite different names*

```diff
@@ -50,31 +50,46 @@
 	Py_XDECREF(self->buf_size);
 	Py_XDECREF(self->read_func);
 	Py_XDECREF(self->file);
 	Py_XDECREF(self->coro);
 	Py_TYPE(self)->tp_free((PyObject*)self);
 }
 
+static void raise_stopiteration(PyObject *value)
+{
+#if defined(PYPY_VERSION)
+	// PyPy doesn't seem to support normalised exceptions for coroutines,
+	// see https://foss.heptapod.net/pypy/pypy/-/issues/3965
+	PyObject *ex_value = PyObject_CallFunctionObjArgs(PyExc_StopIteration, value, NULL);
+	PyErr_SetObject(PyExc_StopIteration, ex_value);
+	Py_DECREF(ex_value);
+#else
+	PyObject *stop_iteration_args = PyTuple_New(1);
+	PyTuple_SET_ITEM(stop_iteration_args, 0, value);
+	PyErr_SetObject(PyExc_StopIteration, stop_iteration_args);
+	Py_DECREF(stop_iteration_args);
+#endif
+}
+
 static PyObject *maybe_pop_event(async_reading_generator *self)
 {
 	PyObject *events = self->events;
 	Py_ssize_t nevents = PyList_Size(events);
 	if (nevents == 0) {
 		return NULL;
 	}
 	PyObject *event = PyList_GET_ITEM(events, self->index++);
-	PyObject *res = PyTuple_New(2);
 	Py_INCREF(event);
-	PyTuple_SET_ITEM(res, 0, event);
-	PyErr_SetObject(PyExc_StopIteration, res);
-	Py_DECREF(res);
 	if (self->index == nevents) {
-		PySequence_DelSlice(events, 0, self->index);
+		if (PySequence_DelSlice(events, 0, self->index) == -1) {
+			Py_RETURN_NONE;
+		}
 		self->index = 0;
 	}
+	raise_stopiteration(event);
 	return event;
 }
 
 static int is_gen_coroutine(PyObject *o)
 {
 	if (PyGen_CheckExact(o)) {
 		PyCodeObject *code = (PyCodeObject *)PyObject_GetAttrString(o, "gi_code");
```

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/async_reading_generator.h` & `ijson-3.2.3/ijson/backends/yajl2_c/async_reading_generator.h`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/basic_parse.c` & `ijson-3.2.3/ijson/backends/yajl2_c/basic_parse.c`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/basic_parse.h` & `ijson-3.2.3/ijson/backends/yajl2_c/basic_parse.h`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/basic_parse_async.c` & `ijson-3.2.3/ijson/backends/yajl2_c/basic_parse_async.c`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/basic_parse_async.h` & `ijson-3.2.3/ijson/backends/yajl2_c/basic_parse_async.h`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/basic_parse_basecoro.c` & `ijson-3.2.3/ijson/backends/yajl2_c/basic_parse_basecoro.c`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/basic_parse_basecoro.h` & `ijson-3.2.3/ijson/backends/yajl2_c/basic_parse_basecoro.h`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/builder.h` & `ijson-3.2.3/ijson/backends/yajl2_c/builder.h`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/common.h` & `ijson-3.2.3/ijson/backends/yajl2_c/common.h`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/coro_utils.c` & `ijson-3.2.3/ijson/backends/yajl2_c/coro_utils.c`

 * *Files 7% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 
 #include "common.h"
 #include "coro_utils.h"
 
 PyObject *chain(PyObject *sink, pipeline_node *coro_pipeline)
 {
 	PyObject *coro = sink;
+	Py_INCREF(coro);
 	int element = 0;
 	while (1) {
 		pipeline_node node = coro_pipeline[element++];
 		if (node.type == NULL) {
 			break;
 		}
 		PyObject *coro_args;
 		if (node.args) {
 			int nargs = PyTuple_Size(node.args);
 			N_N(coro_args = PyTuple_New(nargs + 1));
+			Py_INCREF(coro);
 			PyTuple_SET_ITEM(coro_args, 0, coro);
 			int i;
 			for (i = 0; i != nargs; i++) {
 				PyTuple_SET_ITEM(coro_args, i + 1, PySequence_GetItem(node.args, i));
 			}
 		}
 		else {
 			N_N(coro_args = PyTuple_Pack(1, coro));
 		}
-		if (coro != sink) {
-			Py_DECREF(coro);
-		}
+		Py_DECREF(coro);
 		N_N(coro = PyObject_Call((PyObject *)node.type, coro_args, node.kwargs));
 		Py_DECREF(coro_args);
 	}
 	return coro;
 }
```

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/coro_utils.h` & `ijson-3.2.3/ijson/backends/yajl2_c/coro_utils.h`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/items.c` & `ijson-3.2.3/ijson/backends/yajl2_c/items.c`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/items.h` & `ijson-3.2.3/ijson/backends/yajl2_c/items.h`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/items_async.c` & `ijson-3.2.3/ijson/backends/yajl2_c/items_async.c`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/items_async.h` & `ijson-3.2.3/ijson/backends/yajl2_c/items_async.h`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/items_basecoro.c` & `ijson-3.2.3/ijson/backends/yajl2_c/items_basecoro.c`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/items_basecoro.h` & `ijson-3.2.3/ijson/backends/yajl2_c/items_basecoro.h`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/kvitems.c` & `ijson-3.2.3/ijson/backends/yajl2_c/kvitems.c`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/kvitems.h` & `ijson-3.2.3/ijson/backends/yajl2_c/kvitems.h`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/kvitems_async.c` & `ijson-3.2.3/ijson/backends/yajl2_c/kvitems_async.c`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/kvitems_async.h` & `ijson-3.2.3/ijson/backends/yajl2_c/kvitems_async.h`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/kvitems_basecoro.c` & `ijson-3.2.3/ijson/backends/yajl2_c/kvitems_basecoro.c`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/kvitems_basecoro.h` & `ijson-3.2.3/ijson/backends/yajl2_c/kvitems_basecoro.h`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/module.c` & `ijson-3.2.3/ijson/backends/yajl2_c/module.c`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/parse.c` & `ijson-3.2.3/ijson/backends/yajl2_c/parse.c`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/parse.h` & `ijson-3.2.3/ijson/backends/yajl2_c/parse.h`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/parse_async.c` & `ijson-3.2.3/ijson/backends/yajl2_c/parse_async.c`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/parse_async.h` & `ijson-3.2.3/ijson/backends/yajl2_c/parse_async.h`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/parse_basecoro.c` & `ijson-3.2.3/ijson/backends/yajl2_c/parse_basecoro.c`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/parse_basecoro.h` & `ijson-3.2.3/ijson/backends/yajl2_c/parse_basecoro.h`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/reading_generator.c` & `ijson-3.2.3/ijson/backends/yajl2_c/reading_generator.c`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c/reading_generator.h` & `ijson-3.2.3/ijson/backends/yajl2_c/reading_generator.h`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_c.py` & `ijson-3.2.3/ijson/backends/yajl2_c.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/backends/yajl2_cffi.py` & `ijson-3.2.3/ijson/backends/yajl2_cffi.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/common.py` & `ijson-3.2.3/ijson/common.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/compat.py` & `ijson-3.2.3/ijson/compat.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/dump.py` & `ijson-3.2.3/ijson/dump.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/utils.py` & `ijson-3.2.3/ijson/utils.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson/utils35.py` & `ijson-3.2.3/ijson/utils35.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/ijson.egg-info/PKG-INFO` & `ijson-3.2.3/ijson.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ijson
-Version: 3.2.2
+Version: 3.2.3
 Summary: Iterative JSON parser with standard Python iterator interfaces
 Home-page: https://github.com/ICRAR/ijson
 Author: Rodrigo Tobar, Ivan Sagalaev
 Author-email: rtobar@icrar.org, maniac@softwaremaniacs.org
 License: BSD
 Description: .. image:: https://github.com/ICRAR/ijson/actions/workflows/deploy-to-pypi.yml/badge.svg
             :target: https://github.com/ICRAR/ijson/actions/workflows/deploy-to-pypi.yml
```

### Comparing `ijson-3.2.2/ijson.egg-info/SOURCES.txt` & `ijson-3.2.3/ijson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/setup.py` & `ijson-3.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/test/_test_async_common.py` & `ijson-3.2.3/test/_test_async_common.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/test/_test_async_types_coroutine.py` & `ijson-3.2.3/test/_test_async_types_coroutine.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/test/test_base.py` & `ijson-3.2.3/test/test_base.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/test/test_coroutines.py` & `ijson-3.2.3/test/test_coroutines.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/test/test_dump.py` & `ijson-3.2.3/test/test_dump.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/test/test_generators.py` & `ijson-3.2.3/test/test_generators.py`

 * *Files identical despite different names*

### Comparing `ijson-3.2.2/test/test_misc.py` & `ijson-3.2.3/test/test_misc.py`

 * *Files identical despite different names*

