# Comparing `tmp/codefast-23.7.14.11.tar.gz` & `tmp/codefast-23.7.22.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/codefast-23.7.14.11.tar", last modified: Fri Jul 14 03:06:57 2023, max compression
+gzip compressed data, was "codefast-23.7.22.4.tar", last modified: Sat Jul 22 04:24:09 2023, max compression
```

## Comparing `codefast-23.7.14.11.tar` & `codefast-23.7.22.4.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-14 03:06:57.342090 codefast-23.7.14.11/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1074 2021-08-14 02:45:04.000000 codefast-23.7.14.11/LICENSE
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     1486 2023-07-14 03:06:57.342090 codefast-23.7.14.11/PKG-INFO
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1115 2021-08-14 02:45:04.000000 codefast-23.7.14.11/README.md
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-14 03:06:57.330090 codefast-23.7.14.11/codefast/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1791 2023-07-14 03:06:33.000000 codefast-23.7.14.11/codefast/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     6075 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/argparser.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-14 03:06:57.330090 codefast-23.7.14.11/codefast/asyncio/
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1368 2023-04-19 05:45:01.000000 codefast-23.7.14.11/codefast/asyncio/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1777 2023-05-04 16:26:49.000000 codefast-23.7.14.11/codefast/asyncio/rabbitmq.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-14 03:06:57.330090 codefast-23.7.14.11/codefast/axe/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       34 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/axe/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2232 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/axe/axe.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1029 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/axe.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-14 03:06:57.330090 codefast-23.7.14.11/codefast/base/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       31 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/base/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3880 2022-12-25 13:22:03.000000 codefast-23.7.14.11/codefast/base/format_print.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-14 03:06:57.330090 codefast-23.7.14.11/codefast/betterargs/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       71 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/betterargs/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     4719 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/betterargs/abstractclient.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      692 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/cn.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2646 2022-11-19 16:15:49.000000 codefast-23.7.14.11/codefast/concurrency.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-14 03:06:57.334090 codefast-23.7.14.11/codefast/concurrent/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)        0 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/concurrent/__init__.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     2891 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/concurrent/fastapi_demo.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     4328 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/concurrent/scheduler.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2108 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/constants.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      592 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/core.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-14 03:06:57.334090 codefast-23.7.14.11/codefast/decorators/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3105 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/decorators/__init__.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)      440 2022-12-15 06:35:33.000000 codefast-23.7.14.11/codefast/decorators/log.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     2886 2023-04-28 12:37:33.000000 codefast-23.7.14.11/codefast/decorators/retry.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)    12000 2023-05-10 08:10:23.000000 codefast-23.7.14.11/codefast/ds.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      112 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/exception.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-14 03:06:57.334090 codefast-23.7.14.11/codefast/experimental/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)        0 2023-01-10 00:15:53.000000 codefast-23.7.14.11/codefast/experimental/__init__.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)      581 2023-01-10 02:42:34.000000 codefast-23.7.14.11/codefast/experimental/nsq.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-14 03:06:57.334090 codefast-23.7.14.11/codefast/fio/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       23 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/fio/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     5951 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/fio/ffpb.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-14 03:06:57.334090 codefast-23.7.14.11/codefast/frameworks/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1103 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/frameworks/__init__.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-14 03:06:57.334090 codefast-23.7.14.11/codefast/functools/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       75 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/functools/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      485 2023-01-02 02:54:54.000000 codefast-23.7.14.11/codefast/functools/random.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1042 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/functools/subroutine.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-14 03:06:57.338090 codefast-23.7.14.11/codefast/io/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      174 2023-02-05 03:01:40.000000 codefast-23.7.14.11/codefast/io/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3912 2023-05-07 07:55:23.000000 codefast-23.7.14.11/codefast/io/_json.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     3328 2022-12-04 12:10:17.000000 codefast-23.7.14.11/codefast/io/dblite.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     7952 2023-06-01 03:02:06.000000 codefast-23.7.14.11/codefast/io/file.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     4411 2023-04-12 12:05:54.000000 codefast-23.7.14.11/codefast/io/osdb.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     3857 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/io/sqlite.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3310 2022-12-28 09:45:27.000000 codefast-23.7.14.11/codefast/logger.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1708 2023-05-22 11:40:05.000000 codefast-23.7.14.11/codefast/math.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-14 03:06:57.338090 codefast-23.7.14.11/codefast/network/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      135 2023-04-07 06:18:56.000000 codefast-23.7.14.11/codefast/network/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1213 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/network/curl.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      587 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/network/factory.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2681 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/network/richdownloader.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3841 2023-05-15 04:15:33.000000 codefast-23.7.14.11/codefast/network/tools.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-14 03:06:57.338090 codefast-23.7.14.11/codefast/patterns/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       70 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/patterns/__init__.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1223 2022-12-10 01:39:19.000000 codefast-23.7.14.11/codefast/patterns/factory_method.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     3320 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/patterns/observer.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1884 2023-05-23 04:08:38.000000 codefast-23.7.14.11/codefast/patterns/pipeline.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      773 2022-12-27 13:57:07.000000 codefast-23.7.14.11/codefast/patterns/responsibility_chain.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      395 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/patterns/singleton.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1303 2022-12-15 06:38:07.000000 codefast-23.7.14.11/codefast/reader.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-14 03:06:57.338090 codefast-23.7.14.11/codefast/supercell/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       21 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/supercell/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      124 2022-11-19 13:54:17.000000 codefast-23.7.14.11/codefast/tmp.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-14 03:06:57.338090 codefast-23.7.14.11/codefast/types/
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1064 2022-11-23 05:27:16.000000 codefast-23.7.14.11/codefast/types/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)    12126 2023-05-05 12:49:16.000000 codefast-23.7.14.11/codefast/utils.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-14 03:06:57.330090 codefast-23.7.14.11/codefast.egg-info/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     1486 2023-07-14 03:06:57.000000 codefast-23.7.14.11/codefast.egg-info/PKG-INFO
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     1676 2023-07-14 03:06:57.000000 codefast-23.7.14.11/codefast.egg-info/SOURCES.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        1 2023-07-14 03:06:57.000000 codefast-23.7.14.11/codefast.egg-info/dependency_links.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       96 2023-07-14 03:06:57.000000 codefast-23.7.14.11/codefast.egg-info/requires.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       15 2023-07-14 03:06:57.000000 codefast-23.7.14.11/codefast.egg-info/top_level.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       38 2023-07-14 03:06:57.342090 codefast-23.7.14.11/setup.cfg
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      878 2023-04-07 08:56:08.000000 codefast-23.7.14.11/setup.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-14 03:06:57.338090 codefast-23.7.14.11/tests/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-04-18 12:52:35.000000 codefast-23.7.14.11/tests/__init__.py
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      825 2023-04-18 13:01:02.000000 codefast-23.7.14.11/tests/test_unique_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:24:09.734828 codefast-23.7.22.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-22 04:23:55.000000 codefast-23.7.22.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-22 04:24:09.734828 codefast-23.7.22.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-22 04:23:55.000000 codefast-23.7.22.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:24:09.730828 codefast-23.7.22.4/codefast/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:24:09.730828 codefast-23.7.22.4/codefast/asyncio/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1368 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/asyncio/rabbitmq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:24:09.730828 codefast-23.7.22.4/codefast/axe/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/axe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/axe/axe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/axe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:24:09.730828 codefast-23.7.22.4/codefast/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/base/format_print.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:24:09.734828 codefast-23.7.22.4/codefast/betterargs/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/betterargs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/betterargs/abstractclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/cn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/concurrency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:24:09.734828 codefast-23.7.22.4/codefast/concurrent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/concurrent/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2891 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/concurrent/fastapi_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/concurrent/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:24:09.734828 codefast-23.7.22.4/codefast/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/decorators/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      440 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/decorators/log.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2886 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/decorators/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:24:09.734828 codefast-23.7.22.4/codefast/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/experimental/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      581 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/experimental/nsq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:24:09.734828 codefast-23.7.22.4/codefast/fio/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/fio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/fio/ffpb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:24:09.734828 codefast-23.7.22.4/codefast/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/frameworks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:24:09.734828 codefast-23.7.22.4/codefast/functools/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/functools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/functools/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/functools/subroutine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:24:09.734828 codefast-23.7.22.4/codefast/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/io/_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3328 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/io/dblite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/io/file.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4411 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/io/osdb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3857 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/io/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:24:09.734828 codefast-23.7.22.4/codefast/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/network/curl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/network/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/network/richdownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/network/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:24:09.734828 codefast-23.7.22.4/codefast/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/patterns/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1223 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/patterns/factory_method.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3320 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/patterns/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/patterns/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/patterns/responsibility_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/patterns/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:24:09.734828 codefast-23.7.22.4/codefast/supercell/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/supercell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/tmp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:24:09.734828 codefast-23.7.22.4/codefast/types/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-07-22 04:23:55.000000 codefast-23.7.22.4/codefast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:24:09.730828 codefast-23.7.22.4/codefast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-22 04:24:09.000000 codefast-23.7.22.4/codefast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-22 04:24:09.000000 codefast-23.7.22.4/codefast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 04:24:09.000000 codefast-23.7.22.4/codefast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-22 04:24:09.000000 codefast-23.7.22.4/codefast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-22 04:24:09.000000 codefast-23.7.22.4/codefast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 04:24:09.734828 codefast-23.7.22.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-22 04:23:55.000000 codefast-23.7.22.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:24:09.734828 codefast-23.7.22.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 04:23:55.000000 codefast-23.7.22.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-22 04:23:55.000000 codefast-23.7.22.4/tests/test_unique_session.py
```

### Comparing `codefast-23.7.14.11/LICENSE` & `codefast-23.7.22.4/LICENSE`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/README.md` & `codefast-23.7.22.4/README.md`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/__init__.py` & `codefast-23.7.22.4/codefast/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,23 @@
 
 # ---------------------------- Math methods
 def round4(number:float)->float:
     return round(number, 4)
 
 def round2(number:float)->float:
     return round(number, 2)
-# ----------------------------End of Math methods
+
+# ---------------------------- pandas read files
+
+import pandas as pd
+def csv(csv_file)->pd.DataFrame:
+    return pd.read_csv(csv_file)
+
+def excel(excel_file)->pd.DataFrame:
+    return pd.read_excel(excel_file)
 
 
 def date_file(prefix: str, file_ext: str) -> str:
     import datetime
     return f"{prefix}_{datetime.datetime.now().strftime('%Y%m%d%H%M')}.{file_ext}"
```

### Comparing `codefast-23.7.14.11/codefast/argparser.py` & `codefast-23.7.22.4/codefast/argparser.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/asyncio/__init__.py` & `codefast-23.7.22.4/codefast/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/asyncio/rabbitmq.py` & `codefast-23.7.22.4/codefast/asyncio/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/axe/axe.py` & `codefast-23.7.22.4/codefast/axe/axe.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/axe.py` & `codefast-23.7.22.4/codefast/axe.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/base/format_print.py` & `codefast-23.7.22.4/codefast/base/format_print.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/betterargs/abstractclient.py` & `codefast-23.7.22.4/codefast/betterargs/abstractclient.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/cn.py` & `codefast-23.7.22.4/codefast/cn.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/concurrency.py` & `codefast-23.7.22.4/codefast/concurrency.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/concurrent/fastapi_demo.py` & `codefast-23.7.22.4/codefast/concurrent/fastapi_demo.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/concurrent/scheduler.py` & `codefast-23.7.22.4/codefast/concurrent/scheduler.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/constants.py` & `codefast-23.7.22.4/codefast/constants.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/core.py` & `codefast-23.7.22.4/codefast/core.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/decorators/__init__.py` & `codefast-23.7.22.4/codefast/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/decorators/retry.py` & `codefast-23.7.22.4/codefast/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/ds.py` & `codefast-23.7.22.4/codefast/ds.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/experimental/nsq.py` & `codefast-23.7.22.4/codefast/experimental/nsq.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/fio/ffpb.py` & `codefast-23.7.22.4/codefast/fio/ffpb.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/frameworks/__init__.py` & `codefast-23.7.22.4/codefast/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/functools/subroutine.py` & `codefast-23.7.22.4/codefast/functools/subroutine.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/io/_json.py` & `codefast-23.7.22.4/codefast/io/_json.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/io/dblite.py` & `codefast-23.7.22.4/codefast/io/dblite.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/io/file.py` & `codefast-23.7.22.4/codefast/io/file.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/io/osdb.py` & `codefast-23.7.22.4/codefast/io/osdb.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/io/sqlite.py` & `codefast-23.7.22.4/codefast/io/sqlite.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/logger.py` & `codefast-23.7.22.4/codefast/logger.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/math.py` & `codefast-23.7.22.4/codefast/math.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/network/curl.py` & `codefast-23.7.22.4/codefast/network/curl.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/network/factory.py` & `codefast-23.7.22.4/codefast/network/factory.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/network/richdownloader.py` & `codefast-23.7.22.4/codefast/network/richdownloader.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/network/tools.py` & `codefast-23.7.22.4/codefast/network/tools.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/patterns/factory_method.py` & `codefast-23.7.22.4/codefast/patterns/factory_method.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/patterns/observer.py` & `codefast-23.7.22.4/codefast/patterns/observer.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/patterns/pipeline.py` & `codefast-23.7.22.4/codefast/patterns/pipeline.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/patterns/responsibility_chain.py` & `codefast-23.7.22.4/codefast/patterns/responsibility_chain.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/reader.py` & `codefast-23.7.22.4/codefast/reader.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/types/__init__.py` & `codefast-23.7.22.4/codefast/types/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast/utils.py` & `codefast-23.7.22.4/codefast/utils.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/codefast.egg-info/SOURCES.txt` & `codefast-23.7.22.4/codefast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/setup.py` & `codefast-23.7.22.4/setup.py`

 * *Files identical despite different names*

### Comparing `codefast-23.7.14.11/tests/test_unique_session.py` & `codefast-23.7.22.4/tests/test_unique_session.py`

 * *Files identical despite different names*

