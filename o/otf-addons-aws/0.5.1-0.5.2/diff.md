# Comparing `tmp/otf-addons-aws-0.5.1.tar.gz` & `tmp/otf-addons-aws-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otf-addons-aws-0.5.1.tar", last modified: Fri Jul 21 13:39:14 2023, max compression
+gzip compressed data, was "otf-addons-aws-0.5.2.tar", last modified: Sat Jul 22 19:25:15 2023, max compression
```

## Comparing `otf-addons-aws-0.5.1.tar` & `otf-addons-aws-0.5.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.816904 otf-addons-aws-0.5.1/
--rw-r--r--   0 adam       (501) staff       (20)       72 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/AUTHORS
--rw-r--r--   0 adam       (501) staff       (20)    35149 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/LICENSE
--rw-r--r--   0 adam       (501) staff       (20)       44 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)     5382 2023-07-21 13:39:14.816766 otf-addons-aws-0.5.1/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     4543 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/README.md
--rw-r--r--   0 adam       (501) staff       (20)    13202 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.1/pyproject.toml
--rw-r--r--   0 adam       (501) staff       (20)       38 2023-07-21 13:39:14.816941 otf-addons-aws-0.5.1/setup.cfg
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.810105 otf-addons-aws-0.5.1/src/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.809967 otf-addons-aws-0.5.1/src/opentaskpy/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.809470 otf-addons-aws-0.5.1/src/opentaskpy/addons/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.811627 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/
--rw-r--r--   0 adam       (501) staff       (20)        0 2023-07-20 13:18:56.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/__init__.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.812593 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/
--rw-r--r--   0 adam       (501) staff       (20)        0 2023-07-20 13:18:56.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)      942 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/creds.py
--rw-r--r--   0 adam       (501) staff       (20)     4580 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/lambda.py
--rw-r--r--   0 adam       (501) staff       (20)    12798 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/s3.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.809796 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.809735 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.812911 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/
--rw-r--r--   0 adam       (501) staff       (20)      542 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/lambda.json
--rw-r--r--   0 adam       (501) staff       (20)      506 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/protocol.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.813266 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/
--rw-r--r--   0 adam       (501) staff       (20)      503 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/protocol.json
--rw-r--r--   0 adam       (501) staff       (20)      429 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/s3.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.813764 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.814086 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/
--rw-r--r--   0 adam       (501) staff       (20)      279 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/flags.json
--rw-r--r--   0 adam       (501) staff       (20)      571 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/protocol.json
--rw-r--r--   0 adam       (501) staff       (20)      485 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.814431 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/
--rw-r--r--   0 adam       (501) staff       (20)      398 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/fileWatch.json
--rw-r--r--   0 adam       (501) staff       (20)      500 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/protocol.json
--rw-r--r--   0 adam       (501) staff       (20)      663 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.810007 otf-addons-aws-0.5.1/src/opentaskpy/plugins/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.810047 otf-addons-aws-0.5.1/src/opentaskpy/plugins/lookup/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.814586 otf-addons-aws-0.5.1/src/opentaskpy/plugins/lookup/aws/
--rw-r--r--   0 adam       (501) staff       (20)     2819 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/src/opentaskpy/plugins/lookup/aws/ssm.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.815304 otf-addons-aws-0.5.1/src/otf_addons_aws.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)     5382 2023-07-21 13:39:14.000000 otf-addons-aws-0.5.1/src/otf_addons_aws.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     1570 2023-07-21 13:39:14.000000 otf-addons-aws-0.5.1/src/otf_addons_aws.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-07-21 13:39:14.000000 otf-addons-aws-0.5.1/src/otf_addons_aws.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)      208 2023-07-21 13:39:14.000000 otf-addons-aws-0.5.1/src/otf_addons_aws.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)       11 2023-07-21 13:39:14.000000 otf-addons-aws-0.5.1/src/otf_addons_aws.egg-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-21 13:39:14.816578 otf-addons-aws-0.5.1/tests/
--rw-r--r--   0 adam       (501) staff       (20)      670 2023-07-20 13:18:56.000000 otf-addons-aws-0.5.1/tests/test_lambda_execution_schema_validate.py
--rw-r--r--   0 adam       (501) staff       (20)     2853 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/tests/test_plugin_ssm.py
--rw-r--r--   0 adam       (501) staff       (20)     9676 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/tests/test_remotehandler_lambda_execution.py
--rw-r--r--   0 adam       (501) staff       (20)     2113 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.1/tests/test_remotehandler_s3_execution.py
--rw-r--r--   0 adam       (501) staff       (20)    21869 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.1/tests/test_remotehandler_s3_transfer.py
--rw-r--r--   0 adam       (501) staff       (20)     2272 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.1/tests/test_s3_source_schema_validate.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.756633 otf-addons-aws-0.5.2/
+-rw-r--r--   0 adam       (501) staff       (20)       72 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/AUTHORS
+-rw-r--r--   0 adam       (501) staff       (20)    35149 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)       44 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/MANIFEST.in
+-rw-r--r--   0 adam       (501) staff       (20)     6050 2023-07-22 19:25:15.756496 otf-addons-aws-0.5.2/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     5211 2023-07-21 15:52:59.000000 otf-addons-aws-0.5.2/README.md
+-rw-r--r--   0 adam       (501) staff       (20)    13231 2023-07-22 19:25:03.000000 otf-addons-aws-0.5.2/pyproject.toml
+-rw-r--r--   0 adam       (501) staff       (20)       38 2023-07-22 19:25:15.756670 otf-addons-aws-0.5.2/setup.cfg
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.748048 otf-addons-aws-0.5.2/src/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.747906 otf-addons-aws-0.5.2/src/opentaskpy/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.747388 otf-addons-aws-0.5.2/src/opentaskpy/addons/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.749722 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/
+-rw-r--r--   0 adam       (501) staff       (20)        0 2023-07-22 14:47:19.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/__init__.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.750698 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/
+-rw-r--r--   0 adam       (501) staff       (20)        0 2023-07-20 13:18:56.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)      942 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/creds.py
+-rw-r--r--   0 adam       (501) staff       (20)     4685 2023-07-22 16:20:49.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/lambda.py
+-rw-r--r--   0 adam       (501) staff       (20)    13127 2023-07-22 16:28:21.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/s3.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.747726 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.747665 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.751298 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/
+-rw-r--r--   0 adam       (501) staff       (20)      542 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/lambda.json
+-rw-r--r--   0 adam       (501) staff       (20)      506 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/protocol.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.751712 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/
+-rw-r--r--   0 adam       (501) staff       (20)      503 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/protocol.json
+-rw-r--r--   0 adam       (501) staff       (20)      429 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/s3.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.753057 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.753502 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/
+-rw-r--r--   0 adam       (501) staff       (20)      279 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/flags.json
+-rw-r--r--   0 adam       (501) staff       (20)      571 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/protocol.json
+-rw-r--r--   0 adam       (501) staff       (20)      485 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.753839 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/
+-rw-r--r--   0 adam       (501) staff       (20)      398 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/fileWatch.json
+-rw-r--r--   0 adam       (501) staff       (20)      500 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/protocol.json
+-rw-r--r--   0 adam       (501) staff       (20)      663 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.747948 otf-addons-aws-0.5.2/src/opentaskpy/plugins/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.747988 otf-addons-aws-0.5.2/src/opentaskpy/plugins/lookup/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.753989 otf-addons-aws-0.5.2/src/opentaskpy/plugins/lookup/aws/
+-rw-r--r--   0 adam       (501) staff       (20)     2819 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/plugins/lookup/aws/ssm.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.754590 otf-addons-aws-0.5.2/src/otf_addons_aws.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)     6050 2023-07-22 19:25:15.000000 otf-addons-aws-0.5.2/src/otf_addons_aws.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     1570 2023-07-22 19:25:15.000000 otf-addons-aws-0.5.2/src/otf_addons_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-07-22 19:25:15.000000 otf-addons-aws-0.5.2/src/otf_addons_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)      228 2023-07-22 19:25:15.000000 otf-addons-aws-0.5.2/src/otf_addons_aws.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)       11 2023-07-22 19:25:15.000000 otf-addons-aws-0.5.2/src/otf_addons_aws.egg-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.756258 otf-addons-aws-0.5.2/tests/
+-rw-r--r--   0 adam       (501) staff       (20)      670 2023-07-20 13:18:56.000000 otf-addons-aws-0.5.2/tests/test_lambda_execution_schema_validate.py
+-rw-r--r--   0 adam       (501) staff       (20)     2413 2023-07-22 14:53:37.000000 otf-addons-aws-0.5.2/tests/test_plugin_ssm.py
+-rw-r--r--   0 adam       (501) staff       (20)    11598 2023-07-22 16:02:47.000000 otf-addons-aws-0.5.2/tests/test_remotehandler_lambda_execution.py
+-rw-r--r--   0 adam       (501) staff       (20)     1893 2023-07-22 14:53:16.000000 otf-addons-aws-0.5.2/tests/test_remotehandler_s3_execution.py
+-rw-r--r--   0 adam       (501) staff       (20)    22384 2023-07-22 19:15:25.000000 otf-addons-aws-0.5.2/tests/test_remotehandler_s3_transfer.py
+-rw-r--r--   0 adam       (501) staff       (20)     2272 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.2/tests/test_s3_source_schema_validate.py
```

### Comparing `otf-addons-aws-0.5.1/LICENSE` & `otf-addons-aws-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.1/README.md` & `otf-addons-aws-0.5.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-![unittest status](https://github.com/adammcdonagh/otf-addons-aws/actions/workflows/main.yml/badge.svg)
+[![PyPi](https://img.shields.io/pypi/v/otf-addons-aws.svg)](https://pypi.org/project/otf-addons-aws/)
+![unittest status](https://github.com/adammcdonagh/otf-addons-aws/actions/workflows/test.yml/badge.svg)
+[![Coverage](https://img.shields.io/codecov/c/github/adammcdonagh/otf-addons-aws.svg)](https://codecov.io/gh/adammcdonagh/otf-addons-aws)
+[![License](https://img.shields.io/github/license/adammcdonagh/otf-addons-aws.svg)](https://github.com/adammcdonagh/otf-addons-aws/blob/master/LICENSE)
+[![Issues](https://img.shields.io/github/issues/adammcdonagh/otf-addons-aws.svg)](https://github.com/adammcdonagh/otf-addons-aws/issues)
+[![Stars](https://img.shields.io/github/stars/adammcdonagh/otf-addons-aws.svg)](https://github.com/adammcdonagh/otf-addons-aws/stargazers)
 
 This repository contains addons to allow integration with AWS components via [Open Task Framework (OTF)](https://github.com/adammcdonagh/open-task-framework)
 
 Open Task Framework (OTF) is a Python based framework to make it easy to run predefined file transfers and scripts/commands on remote machines.
 
 These addons include several additional features:
```

### Comparing `otf-addons-aws-0.5.1/pyproject.toml` & `otf-addons-aws-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "otf-addons-aws"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
   { name="Adam McDonagh", email="adam@elitemonkey.net" },
 ]
 license = { text = "GPLv3" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: POSIX",
 ]
 keywords = ["automation", "task", "framework", "aws", "s3", "ssm", "otf"]
 dependencies = [
   "boto3 >= 1.26",
-  "opentaskpy >= 0.12.0",
+  "opentaskpy >= 0.12.1",
 ]
 description = "Addons for opentaskpy, giving it the ability to push/pull via AWS S3, and pull variables from AWS SSM Parameter Store."
 readme = "README.md"
 requires-python = ">=3.11"
 
 [project.optional-dependencies]
 dev = [
@@ -38,26 +38,28 @@
   "pytest-shell",
   "lovely-pytest-docker",
   "pre-commit",
   "pylint",
   "pydantic",
   "mypy",
   "ruff",
+  "coverage",
+  "pytest-cov"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/adammcdonagh/otf-addons-aws"
 "Bug Tracker" = "https://github.com/adammcdonagh/otf-addons-aws/issues"
 "Changelog" = "https://github.com/adammcdonagh/otf-addons-aws/blob/main/CHANGELOG.md"
 
 [tool.isort]
 profile = 'black'
 
 [tool.bumpver]
-current_version = "0.5.1"
+current_version = "0.5.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/creds.py` & `otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/creds.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/lambda.py` & `otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/lambda.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,21 +90,22 @@
         if "payload" in self.spec:
             payload = self.spec["payload"]
 
         try:
             invoke_response = self.lambda_client.invoke(
                 FunctionName=function_arn,
                 InvocationType=invocation_type,
+                LogType="Tail",
                 Payload=json.dumps(payload),
             )
 
             if (
                 invoke_response["StatusCode"] != 200
-                and invoke_response["StatusCode"] != 202
-            ):
+                and invocation_type == "RequestResponse"
+            ) or (invoke_response["StatusCode"] != 202 and invocation_type == "Event"):
                 self.logger.error(f"Failed to run lambda function: {function_arn}")
                 return False
 
             if "FunctionError" in invoke_response:
                 self.logger.error(
                     f"Lambda function returned an error: {function_arn} - AWS Exception"
                     f" message: {invoke_response['FunctionError']}"
```

### Comparing `otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/s3.py` & `otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,49 +119,53 @@
         """
         kwargs = {
             "Bucket": self.spec["bucket"],
             "MaxKeys": MAX_OBJECTS_PER_QUERY,
         }
         if directory:
             kwargs["Prefix"] = directory
-        elif str(self.spec["directory"]):
+        elif "directory" in self.spec and str(self.spec["directory"]):
             kwargs["Prefix"] = str(self.spec["directory"])
 
         remote_files = {}
 
-        while True:
-            response = self.s3_client.list_objects_v2(**kwargs)
-
-            if response["KeyCount"]:
-                for object_ in response["Contents"]:
-                    key = object_["Key"]
-                    # Get the filename from the key
-                    filename = key.split("/")[-1]  #
-                    self.logger.debug(f"Found file: {filename}")
-                    if file_pattern and not re.match(file_pattern, filename):
-                        continue
-
-                    # Get the size and modified time
-                    file_attr = self.s3_client.head_object(
-                        Bucket=self.spec["bucket"], Key=key
-                    )
-
-                    remote_files[key] = {
-                        "size": file_attr["ContentLength"],
-                        "modified_time": file_attr["LastModified"].timestamp(),
-                    }
-
-                # This handles the pagination
-                # if the NextContinuationToken doesn't exist, then we'll break out
-                # of the loop
-                try:
-                    kwargs["ContinuationToken"] = response["NextContinuationToken"]
-                except KeyError:
-                    break
-            break
+        try:
+            while True:
+                response = self.s3_client.list_objects_v2(**kwargs)
+
+                if response["KeyCount"]:
+                    for object_ in response["Contents"]:
+                        key = object_["Key"]
+                        # Get the filename from the key
+                        filename = key.split("/")[-1]  #
+                        self.logger.debug(f"Found file: {filename}")
+                        if file_pattern and not re.match(file_pattern, filename):
+                            continue
+
+                        # Get the size and modified time
+                        file_attr = self.s3_client.head_object(
+                            Bucket=self.spec["bucket"], Key=key
+                        )
+
+                        remote_files[key] = {
+                            "size": file_attr["ContentLength"],
+                            "modified_time": file_attr["LastModified"].timestamp(),
+                        }
+
+                    # This handles the pagination
+                    # if the NextContinuationToken doesn't exist, then we'll break out
+                    # of the loop
+                    try:
+                        kwargs["ContinuationToken"] = response["NextContinuationToken"]
+                    except KeyError:
+                        break
+                break
+        except Exception as e:  # pylint: disable=broad-exception-caught
+            self.logger.error(f"Error listing files: {self.spec['bucket']}")
+            self.logger.error(e)
 
         return remote_files
 
     def move_files_to_final_location(self, files: list[str]) -> None:
         """Not implemented for this handler."""
         raise NotImplementedError
```

### Comparing `otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/lambda.json` & `otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/lambda.json`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/protocol.json` & `otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/protocol.json`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.1/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source.json` & `otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source.json`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.1/src/opentaskpy/plugins/lookup/aws/ssm.py` & `otf-addons-aws-0.5.2/src/opentaskpy/plugins/lookup/aws/ssm.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.1/src/otf_addons_aws.egg-info/SOURCES.txt` & `otf-addons-aws-0.5.2/src/otf_addons_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.1/tests/test_lambda_execution_schema_validate.py` & `otf-addons-aws-0.5.2/tests/test_lambda_execution_schema_validate.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.1/tests/test_plugin_ssm.py` & `otf-addons-aws-0.5.2/tests/test_plugin_ssm.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,27 +23,21 @@
 
     assert (
         ex.value.args[0]
         == f"Missing kwarg: 'name' while trying to run lookup plugin '{PLUGIN_NAME}'"
     )
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
 def test_ssm_plugin_param_name_not_found(credentials):
     with pytest.raises(ClientError) as ex:
         run(name="does_not_exist")
 
     assert ex.value.response["Error"]["Code"] == "ParameterNotFound"
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
 def test_ssm_plugin_standard_string(ssm_client):
     expected = "test1234"
     # Populate the SSM parameter store with a test value
     ssm_client.put_parameter(
         Name="my_test_param",
         Value=expected,
         Type="String",
@@ -51,17 +45,14 @@
     )
 
     result = run(name="my_test_param")
 
     assert result == expected
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
 def test_ssm_plugin_secure_string(ssm_client):
     expected = "securetest1234"
     # Populate the SSM parameter store with a test value
     ssm_client.put_parameter(
         Name="my_secure_test_param",
         Value=expected,
         Type="SecureString",
@@ -69,17 +60,14 @@
     )
 
     result = run(name="my_secure_test_param")
 
     assert result == expected
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
 def test_config_loader_using_ssm_plugin(ssm_client, tmpdir):
     json_obj = {
         "testLookup": "{{ lookup('aws.ssm', name='my_test_param') }}",
     }
 
     fs.create_files(
         [
```

### Comparing `otf-addons-aws-0.5.1/tests/test_remotehandler_lambda_execution.py` & `otf-addons-aws-0.5.2/tests/test_remotehandler_lambda_execution.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import pytest
 from opentaskpy.config.loader import ConfigLoader
 from opentaskpy.taskhandlers import batch, execution
 from pytest_shell import fs
 
 from tests.fixtures.localstack import *  # noqa: F403, F405
 
-os.environ["OTF_NO_LOG"] = "0"
 os.environ["OTF_LOG_LEVEL"] = "DEBUG"
 
 BUCKET_NAME = "otf-addons-aws-lambda-execution-test"
 BUCKET_NAME_1 = "otf-addons-aws-lambda-execution-test-1"
 BUCKET_NAME_2 = "otf-addons-aws-lambda-execution-test-2"
 logger = opentaskpy.otflogging.init_logging(__name__)
 
@@ -78,28 +77,33 @@
         FunctionName="my-function",
         Runtime="python3.9",
         Code={
             "ZipFile": zip_buffer.read(),
         },
         Handler=f"{re.sub('.py', '', lambda_handler)}.lambda_handler",
         Role="arn:aws:iam::123456789012:role/lambda-role",
-        Timeout=300,
+        Timeout=10,
         MemorySize=128,
     )
     function_arn = lambda_response["FunctionArn"]
 
     # Wait for the function status to become Active, from Pending before proceeding
     counter = 0
     while True:
         lambda_response = lambda_client.get_function(FunctionName=function_arn)
         if lambda_response["Configuration"]["State"] == "Active":
             break
         counter += 1
         # If we get to 10, then fail the text
-        if counter >= 10:
+        limit = 10
+
+        # Give it more time if running in GitHub Actions
+        if github_actions():
+            limit = 30
+        if counter >= limit:
             raise Exception(
                 "Lambda function failed to become active in reasonable time"
             )
         time.sleep(1)
 
     # Manually call the function to check it's actually working
     if invoke:
@@ -124,31 +128,25 @@
     for bucket in buckets:
         subprocess.run(
             ["awslocal", "s3", "rb", f"s3://{bucket}", "--force"], check=False
         )
         subprocess.run(["awslocal", "s3", "mb", f"s3://{bucket}"], check=False)
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
 def test_remote_handler(credentials):
     execution_obj = execution.Execution(
         None, "call-lambda-function", lambda_execution_task_definition
     )
 
     execution_obj._set_remote_handlers()
 
     # Validate some things were set as expected
     assert execution_obj.remote_handlers[0].__class__.__name__ == "LambdaExecution"
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
 def test_run_lambda_function(credentials, lambda_client, s3_client, setup_bucket):
     function_arn = create_lambda_function(
         lambda_client,
         "lambda_write_to_s3.py",
         {
             "bucket_name": BUCKET_NAME,
             "file_name": "function_test.txt",
@@ -211,17 +209,64 @@
     lambda_execution_task_definition_copy["invocationType"] = "RequestResponse"
     execution_obj = execution.Execution(
         None, "call-lambda-function", lambda_execution_task_definition_copy
     )
     assert execution_obj.run()
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
+def test_run_lambda_function_with_failure(credentials, lambda_client):
+    function_arn = create_lambda_function(lambda_client, "lambda_failure.py", {})
+
+    # Update the task definition with the ARN of the function we just created
+    lambda_execution_task_definition_copy = lambda_execution_task_definition.copy()
+    lambda_execution_task_definition_copy["functionArn"] = function_arn
+    lambda_execution_task_definition_copy["invocationType"] = "RequestResponse"
+
+    # Call the execution and check whether the lambda function ran successfully
+    execution_obj = execution.Execution(
+        None, "call-lambda-function-failure", lambda_execution_task_definition_copy
+    )
+
+    logging.getLogger("boto3").setLevel(logging.DEBUG)
+    logging.getLogger("botocore").setLevel(logging.DEBUG)
+
+    # Wait a second for the lambda to finish
+    time.sleep(2)
+
+    assert not execution_obj.run()
+
+
+def test_run_non_existent_lambda_function(credentials):
+    # Update the task definition with the ARN of the function we just created
+    lambda_execution_task_definition_copy = lambda_execution_task_definition.copy()
+    lambda_execution_task_definition_copy["functionArn"] = "invalid-arn"
+
+    # Call the execution and check whether the lambda function ran successfully
+    execution_obj = execution.Execution(
+        None,
+        "call-non-existent-lambda-function-failure",
+        lambda_execution_task_definition_copy,
+    )
+
+    logging.getLogger("boto3").setLevel(logging.DEBUG)
+    logging.getLogger("botocore").setLevel(logging.DEBUG)
+
+    assert not execution_obj.run()
+
+
+def test_run_lambda_function_with_invalid_config():
+    lambda_execution_task_definition_copy = lambda_execution_task_definition.copy()
+    del lambda_execution_task_definition_copy["functionArn"]
+    execution_obj = execution.Execution(
+        None, "call-lambda-function-invalid", lambda_execution_task_definition_copy
+    )
+    with pytest.raises(opentaskpy.exceptions.InvalidConfigError):
+        execution_obj.run()
+
+
 def test_run_lambda_function_with_invalid_payload(lambda_client):
     # Create the lambda function
     function_arn = create_lambda_function(
         lambda_client,
         "lambda_write_to_s3.py",
         {
             "bucket_name": BUCKET_NAME_1,
@@ -253,35 +298,33 @@
         None, "call-lambda-function", lambda_execution_task_definition_invalid_payload
     )
 
     # This is expected to work, because there's no validation of the payload when invoked this way
     assert execution_obj.run()
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
 def test_lambda_execution_batch_timeout(tmpdir, lambda_client):
     # Create the function, but dont invoke it, as it runs too long
     function_arn = create_lambda_function(
         lambda_client, "lambda_sleep_60.py", None, invoke=False
     )
 
     # set the arn in lambda_execution_task_definition
     lambda_execution_task_definition["functionArn"] = function_arn
+    # Set invocationType to RequestResponse so that it blocks, and will timeout
+    lambda_execution_task_definition["invocationType"] = "RequestResponse"
 
     # We need to write the lambda execution definition to a file for the config_loader to read from
     with open(f"{tmpdir}/lambda_execution_task_definition.json", "w") as f:
         json.dump(lambda_execution_task_definition, f)
 
     # Write a dummy variables file
     fs.create_files([{f"{tmpdir}/variables.json": {"content": "{}"}}])
 
     config_loader = ConfigLoader(tmpdir)
 
-    # Enable logging
-    del os.environ["OTF_NO_LOG"]
-
     batch_obj = batch.Batch(
         None, "timeout", lambda_batch_task_definition, config_loader
     )
-    assert batch_obj.run()
+
+    # Batch is configured to timeout first, though since we cannot kill the actual lambda thread, it'll still block until the lambda function times out
+    assert not batch_obj.run()
```

### Comparing `otf-addons-aws-0.5.1/tests/test_remotehandler_s3_execution.py` & `otf-addons-aws-0.5.2/tests/test_remotehandler_s3_execution.py`

 * *Files 20% similar despite different names*

```diff
@@ -38,31 +38,25 @@
     for bucket in buckets:
         subprocess.run(
             ["awslocal", "s3", "rb", f"s3://{bucket}", "--force"], check=False
         )
         subprocess.run(["awslocal", "s3", "mb", f"s3://{bucket}"], check=False)
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
 def test_remote_handler():
     execution_obj = execution.Execution(
         None, "s3-flag-file", s3_execution_task_definition
     )
 
     execution_obj._set_remote_handlers()
 
     # Validate some things were set as expected
     assert execution_obj.remote_handlers[0].__class__.__name__ == "S3Execution"
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
 def test_s3_touch_file(setup_bucket):
     execution_obj = execution.Execution(
         None, "s3-flag-file", s3_execution_task_definition
     )
 
     assert execution_obj.run()
```

### Comparing `otf-addons-aws-0.5.1/tests/test_remotehandler_s3_transfer.py` & `otf-addons-aws-0.5.2/tests/test_remotehandler_s3_transfer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pylint: skip-file
 import datetime
 import os
 import shutil
 import subprocess
 import threading
+from copy import deepcopy
 
 import pytest
 from opentaskpy.taskhandlers import transfer
 from pytest_shell import fs
 
 from opentaskpy import exceptions
 from tests.fixtures.localstack import *  # noqa: F403, F405
@@ -362,18 +363,15 @@
     ]
     for host in ("ssh_1", "ssh_2"):
         for command in commands:
             docker_services.execute(host, *command)
 
 
 @pytest.fixture(scope="function")
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
-def setup_bucket(credentials):
+def setup_bucket(credentials, s3_client):
     # This all relies on docker container for the AWS stack being set up and running
     # The AWS CLI should also be installed
 
     buckets = [BUCKET_NAME, BUCKET_NAME_2]
     # Delete existing buckets and recreate
     for bucket in buckets:
         subprocess.run(
@@ -392,51 +390,55 @@
     # Validate some things were set as expected
     assert transfer_obj.source_remote_handler.__class__.__name__ == "S3Transfer"
 
     # dest_remote_handler should be None
     assert transfer_obj.dest_remote_handlers is None
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
-def test_s3_file_watch(setup_bucket, tmp_path):
+def test_s3_file_watch(s3_client, setup_bucket, tmp_path):
     transfer_obj = transfer.Transfer(
         None, "s3-file-watch", s3_file_watch_task_definition
     )
 
     # Create a file to watch for with the current date
     datestamp = datetime.datetime.now().strftime("%Y%m%d")
 
     # Write a test file locally
-    fs.create_files([{f"{tmp_path}/{datestamp}.txt": {"content": "test1234"}}])
-
-    # Write the dummy file to the test S3 bucket
+    fs.create_files(
+        [
+            {f"{tmp_path}/{datestamp}.txt": {"content": "test1234"}},
+            {f"{tmp_path}/{datestamp}1.csv": {"content": "test1234"}},
+            {f"{tmp_path}/{datestamp}2.pdf": {"content": "test1234"}},
+            {f"{tmp_path}/{datestamp}3.docx": {"content": "test1234"}},
+        ]
+    )
 
     with pytest.raises(exceptions.RemoteFileNotFoundError) as cm:
         transfer_obj.run()
     assert "No files found after " in cm.value.args[0]
 
+    # Upload the 3 non-matching files
+    for file in os.listdir(tmp_path):
+        if not file.endswith(".txt"):
+            create_s3_file(s3_client, f"{tmp_path}/{file}", f"src/{file}")
+
     # This time write the contents after 5 seconds
     t = threading.Timer(
         5,
         create_s3_file,
-        [f"{tmp_path}/{datestamp}.txt", "src/test.txt"],
+        [s3_client, f"{tmp_path}/{datestamp}.txt", "src/test.txt"],
     )
     t.start()
     print(  # noqa: T201
         "Started thread - Expect file in 5 seconds, starting task-run now..."
     )
 
     assert transfer_obj.run()
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
 def test_s3_age_conditions_size(setup_bucket, tmp_path, s3_client):
     transfer_obj = transfer.Transfer(
         None, "s3-age-conditions", s3_age_conditions_task_definition
     )
 
     # Write a test file locally
     files = [
@@ -445,196 +447,214 @@
         {f"{tmp_path}/too_new_file.txt": {"content": "123"}},
     ]
     fs.create_files(files)
     import time
 
     for file in files:
         file_name = os.path.basename(list(file.keys())[0])
-        create_s3_file(list(file.keys())[0], f"src/{file_name}")
+        create_s3_file(s3_client, list(file.keys())[0], f"src/{file_name}")
         # Sleep 6 seconds
         time.sleep(6)
 
     assert transfer_obj.run()
 
     objects = s3_client.list_objects(Bucket=BUCKET_NAME_2)
     # check that the correct_file.txt is in the bucket, and not the other 2
     assert len(objects["Contents"]) == 1
     assert objects["Contents"][0]["Key"] == "dest/correct_file.txt"
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
 def test_s3_file_conditions_size(setup_bucket, tmp_path, s3_client):
     transfer_obj = transfer.Transfer(
         None, "s3-file-size-conditions", s3_file_size_conditions_task_definition
     )
 
     # Write a test file locally
     files = [
         {f"{tmp_path}/too_small_file.txt": {"content": "1"}},
         {f"{tmp_path}/correct_file.txt": {"content": "test12345678"}},
         {f"{tmp_path}/too_large_file.txt": {"content": "test12345678901234567890"}},
     ]
     fs.create_files(files)
     for file in files:
         file_name = os.path.basename(list(file.keys())[0])
-        create_s3_file(list(file.keys())[0], f"src/{file_name}")
+        create_s3_file(s3_client, list(file.keys())[0], f"src/{file_name}")
 
     assert transfer_obj.run()
 
     objects = s3_client.list_objects(Bucket=BUCKET_NAME_2)
     # check that the correct_file.txt is in the bucket, and not the other 2
     assert len(objects["Contents"]) == 1
     assert objects["Contents"][0]["Key"] == "dest/correct_file.txt"
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
 def test_s3_to_s3_copy(setup_bucket, s3_client, tmp_path):
     transfer_obj = transfer.Transfer(None, "s3-to-s3", s3_to_s3_copy_task_definition)
 
     # Create a file to watch for with the current date
     datestamp = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
 
     # Write a test file locally
 
     fs.create_files([{f"{tmp_path}/{datestamp}.txt": {"content": "test1234"}}])
-    create_s3_file(f"{tmp_path}/{datestamp}.txt", "src/test.txt")
+    create_s3_file(s3_client, f"{tmp_path}/{datestamp}.txt", "src/test.txt")
 
     assert transfer_obj.run()
 
     # Check that the file is in the destination bucket
     s3_response = s3_client.head_object(
         Bucket=BUCKET_NAME_2,
         Key="dest/test.txt",
     )
     assert s3_response["ResponseMetadata"]["HTTPStatusCode"] == 200
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
+def test_s3_to_s3_invalid_source(setup_bucket, s3_client, tmp_path):
+    s3_to_s3_copy_task_definition_copy = deepcopy(s3_to_s3_copy_task_definition)
+
+    s3_to_s3_copy_task_definition_copy["source"]["bucket"] = "invalid-bucket"
+
+    transfer_obj = transfer.Transfer(
+        None, "s3-to-s3-invalid-source", s3_to_s3_copy_task_definition_copy
+    )
+
+    with pytest.raises(exceptions.FilesDoNotMeetConditionsError):
+        transfer_obj.run()
+
+
+def test_s3_to_s3_invalid_destination(credentials, setup_bucket, s3_client, tmp_path):
+    s3_to_s3_copy_task_definition_copy = deepcopy(s3_to_s3_copy_task_definition)
+
+    s3_to_s3_copy_task_definition_copy["destination"][0]["bucket"] = "invalid-bucket"
+
+    # Create a file to find
+    datestamp = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
+
+    # Write a test file locally
+
+    fs.create_files([{f"{tmp_path}/{datestamp}.txt": {"content": "test1234"}}])
+    create_s3_file(s3_client, f"{tmp_path}/{datestamp}.txt", "src/test.txt")
+
+    transfer_obj = transfer.Transfer(
+        None, "s3-to-s3-invalid-destination", s3_to_s3_copy_task_definition_copy
+    )
+
+    with pytest.raises(exceptions.RemoteTransferError):
+        transfer_obj.run()
+
+
 def test_s3_to_s3_with_fin_copy(setup_bucket, tmp_path, s3_client):
     transfer_obj = transfer.Transfer(
         None, "s3-to-s3-with-fin", s3_to_s3_copy_with_fin_task_definition
     )
 
     # Create a file to watch for with the current date
     datestamp = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
 
     # Write a test file locally
 
     fs.create_files([{f"{tmp_path}/{datestamp}.txt": {"content": "test1234"}}])
-    create_s3_file(f"{tmp_path}/{datestamp}.txt", "src/test.txt")
+    create_s3_file(s3_client, f"{tmp_path}/{datestamp}.txt", "src/test.txt")
 
     assert transfer_obj.run()
 
     objects = s3_client.list_objects(Bucket=BUCKET_NAME_2)
 
     assert len(objects["Contents"]) == 2
     # Check that the file and fin file are in the destination bucket
     object_keys = [obj["Key"] for obj in objects["Contents"]]
     assert "dest/test.txt" in object_keys
     assert "dest/my_fin.fin" in object_keys
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
 def test_s3_to_s3_copy_disable_bucket_owner_acl(setup_bucket, s3_client, tmp_path):
-    s3_to_s3_copy_task_definition["destination"][0]["protocol"][
+    s3_to_s3_copy_task_definition_copy = deepcopy(s3_to_s3_copy_task_definition)
+    s3_to_s3_copy_task_definition_copy["destination"][0]["protocol"][
         "disableBucketOwnerControlACL"
     ] = True
-    transfer_obj = transfer.Transfer(None, "s3-to-s3", s3_to_s3_copy_task_definition)
+    transfer_obj = transfer.Transfer(
+        None, "s3-to-s3", s3_to_s3_copy_task_definition_copy
+    )
 
     # Create a file to watch for with the current date
     datestamp = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
 
     # Write a test file locally
 
     fs.create_files([{f"{tmp_path}/{datestamp}.txt": {"content": "test1234"}}])
-    create_s3_file(f"{tmp_path}/{datestamp}.txt", "src/test.txt")
+    create_s3_file(s3_client, f"{tmp_path}/{datestamp}.txt", "src/test.txt")
 
     assert transfer_obj.run()
 
     # Can't really test this works with localstack, since there's no actual IAM permissions set on anything
     # Check that the file is in the destination bucket
     objects = s3_client.list_objects(Bucket=BUCKET_NAME_2)
     assert len(objects["Contents"]) == 1
     assert objects["Contents"][0]["Key"] == "dest/test.txt"
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
 def test_s3_to_s3_copy_pca_delete(setup_bucket, tmp_path, s3_client):
     transfer_obj = transfer.Transfer(
         None, "s3-to-s3-pca-delete", s3_to_s3_pca_delete_task_definition
     )
 
     # Create a file to watch for with the current date
     datestamp = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
 
     # Write a test file locally
 
     fs.create_files([{f"{tmp_path}/{datestamp}.txt": {"content": "test1234"}}])
-    create_s3_file(f"{tmp_path}/{datestamp}.txt", f"src/{datestamp}.txt")
+    create_s3_file(s3_client, f"{tmp_path}/{datestamp}.txt", f"src/{datestamp}.txt")
 
     assert transfer_obj.run()
 
     objects = s3_client.list_objects(Bucket=BUCKET_NAME_2)
     # check that the correct_file.txt is in the bucket, and not the other 2
     assert len(objects["Contents"]) == 1
     assert objects["Contents"][0]["Key"] == f"dest/{datestamp}.txt"
 
     # Check that the file is not in the source bucket
     objects = s3_client.list_objects(Bucket=BUCKET_NAME)
     assert "Contents" not in objects
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
 def test_s3_to_s3_copy_pca_move(setup_bucket, tmp_path, s3_client):
     transfer_obj = transfer.Transfer(
         None, "s3-to-s3-pca-move", s3_to_s3_pca_move_task_definition
     )
 
     # Write a test file locally
 
     fs.create_files([{f"{tmp_path}/pca-move.txt": {"content": "test1234"}}])
-    create_s3_file(f"{tmp_path}/pca-move.txt", "src/pca-move.txt")
+    create_s3_file(s3_client, f"{tmp_path}/pca-move.txt", "src/pca-move.txt")
 
     assert transfer_obj.run()
 
     # Check that the file is in the destination bucket
     objects = s3_client.list_objects(Bucket=BUCKET_NAME_2)
     assert len(objects["Contents"]) == 1
     assert objects["Contents"][0]["Key"] == "dest/pca-move.txt"
 
     # Check that the file has been moved to archive
     objects = s3_client.list_objects(Bucket=BUCKET_NAME)
     assert len(objects["Contents"]) == 1
     assert objects["Contents"][0]["Key"] == "src/archive/pca-move.txt"
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
 def test_s3_to_s3_copy_pca_rename(setup_bucket, tmp_path, s3_client):
     transfer_obj = transfer.Transfer(
         None, "s3-to-s3-pca-rename", s3_to_s3_pca_rename_task_definition
     )
 
     # Write a test file locally
     fs.create_files([{f"{tmp_path}/file-pca-rename-1234.txt": {"content": "test1234"}}])
     create_s3_file(
-        f"{tmp_path}/file-pca-rename-1234.txt", "src/file-pca-rename-1234.txt"
+        s3_client,
+        f"{tmp_path}/file-pca-rename-1234.txt",
+        "src/file-pca-rename-1234.txt",
     )
 
     assert transfer_obj.run()
 
     # Check that the file is in the destination bucket
     objects = s3_client.list_objects(Bucket=BUCKET_NAME_2)
     assert len(objects["Contents"]) == 1
@@ -643,30 +663,27 @@
     objects = s3_client.list_objects(Bucket=BUCKET_NAME)
     assert len(objects["Contents"]) == 1
     assert (
         objects["Contents"][0]["Key"] == "src/archive/file-pca-rename-1234-renamed.txt"
     )
 
 
-def test_s3_to_ssh_copy(setup_bucket, tmp_path, setup_ssh_keys):
+def test_s3_to_ssh_copy(setup_bucket, s3_client, tmp_path, setup_ssh_keys):
     transfer_obj = transfer.Transfer(None, "s3-to-ssh", s3_to_ssh_copy_task_definition)
 
     # Create a file to watch for with the current date
     datestamp = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
 
     # Write a test file locally
     fs.create_files([{f"{tmp_path}/{datestamp}.txt": {"content": "test1234"}}])
-    create_s3_file(f"{tmp_path}/{datestamp}.txt", "src/test.txt")
+    create_s3_file(s3_client, f"{tmp_path}/{datestamp}.txt", "src/test.txt")
 
     assert transfer_obj.run()
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
 def test_ssh_to_s3_copy(setup_bucket, root_dir, setup_ssh_keys):
     transfer_obj = transfer.Transfer(None, "ssh-to-s3", ssh_to_s3_copy_task_definition)
 
     # Create a file to watch for with the current date
     datestamp = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
 
     # Write a test file locally
@@ -686,40 +703,33 @@
         ],
         capture_output=True,
     )
     # Asset result.returncode is 0
     assert result.returncode == 0
 
 
-@pytest.mark.skipif(
-    condition=github_actions(), reason="cannot run localstack tests in github actions"
-)
 def test_s3_file_watch_custom_creds(
     setup_bucket,
     tmp_path,
-    cleanup_credentials,
+    s3_client,
 ):
     transfer_obj = transfer.Transfer(
         None, "s3-file-watch-custom-creds", s3_file_watch_custom_creds_task_definition
     )
 
     # Create a file to watch for with the current date
     datestamp = datetime.datetime.now().strftime("%Y%m%d")
 
     # Write a test file locally
     fs.create_files([{f"{tmp_path}/{datestamp}.txt": {"content": "test1234"}}])
     # Write the dummy file to the test S3 bucket
-    create_s3_file(f"{tmp_path}/{datestamp}.txt", "src/test.txt")
+    create_s3_file(s3_client, f"{tmp_path}/{datestamp}.txt", "src/test.txt")
 
     assert transfer_obj.run()
 
 
-def create_s3_file(local_file, object_key):
-    subprocess.run(
-        [
-            "awslocal",
-            "s3",
-            "cp",
-            local_file,
-            f"s3://{BUCKET_NAME}/{object_key}",
-        ]
+def create_s3_file(s3_client, local_file, object_key):
+    s3_client.put_object(
+        Bucket=BUCKET_NAME,
+        Key=object_key,
+        Body=open(local_file, "rb"),
     )
```

### Comparing `otf-addons-aws-0.5.1/tests/test_s3_source_schema_validate.py` & `otf-addons-aws-0.5.2/tests/test_s3_source_schema_validate.py`

 * *Files identical despite different names*

