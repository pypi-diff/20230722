# Comparing `tmp/cirq-1.3.0.dev20230720000937-py3-none-any.whl.zip` & `tmp/cirq-1.3.0.dev20230722062259-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 8379 bytes, number of entries: 6
--rw-r--r--  2.0 unx      292 b- defN 23-Jul-20 00:09 cirq-1.3.0.dev20230720000937.dist-info/AUTHORS
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-20 00:09 cirq-1.3.0.dev20230720000937.dist-info/LICENSE
--rw-r--r--  2.0 unx     7790 b- defN 23-Jul-20 00:09 cirq-1.3.0.dev20230720000937.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 00:09 cirq-1.3.0.dev20230720000937.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-20 00:09 cirq-1.3.0.dev20230720000937.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      563 b- defN 23-Jul-20 00:09 cirq-1.3.0.dev20230720000937.dist-info/RECORD
-6 files, 20095 bytes uncompressed, 7341 bytes compressed:  63.5%
+Zip file size: 8380 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      292 b- defN 23-Jul-22 06:23 cirq-1.3.0.dev20230722062259.dist-info/AUTHORS
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-22 06:23 cirq-1.3.0.dev20230722062259.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7798 b- defN 23-Jul-22 06:23 cirq-1.3.0.dev20230722062259.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-22 06:23 cirq-1.3.0.dev20230722062259.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-22 06:23 cirq-1.3.0.dev20230722062259.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      563 b- defN 23-Jul-22 06:23 cirq-1.3.0.dev20230722062259.dist-info/RECORD
+6 files, 20103 bytes uncompressed, 7342 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: cirq-1.3.0.dev20230720000937.dist-info/AUTHORS
+Filename: cirq-1.3.0.dev20230722062259.dist-info/AUTHORS
 Comment: 
 
-Filename: cirq-1.3.0.dev20230720000937.dist-info/LICENSE
+Filename: cirq-1.3.0.dev20230722062259.dist-info/LICENSE
 Comment: 
 
-Filename: cirq-1.3.0.dev20230720000937.dist-info/METADATA
+Filename: cirq-1.3.0.dev20230722062259.dist-info/METADATA
 Comment: 
 
-Filename: cirq-1.3.0.dev20230720000937.dist-info/WHEEL
+Filename: cirq-1.3.0.dev20230722062259.dist-info/WHEEL
 Comment: 
 
-Filename: cirq-1.3.0.dev20230720000937.dist-info/top_level.txt
+Filename: cirq-1.3.0.dev20230722062259.dist-info/top_level.txt
 Comment: 
 
-Filename: cirq-1.3.0.dev20230720000937.dist-info/RECORD
+Filename: cirq-1.3.0.dev20230722062259.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cirq-1.3.0.dev20230720000937.dist-info/LICENSE` & `cirq-1.3.0.dev20230722062259.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cirq-1.3.0.dev20230720000937.dist-info/METADATA` & `cirq-1.3.0.dev20230722062259.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: cirq
-Version: 1.3.0.dev20230720000937
+Version: 1.3.0.dev20230722062259
 Summary: A framework for creating, editing, and invoking Noisy Intermediate Scale Quantum (NISQ) circuits.
 Home-page: http://github.com/quantumlib/cirq
 Author: The Cirq Developers
 Author-email: cirq-dev@googlegroups.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.9.0
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: cirq-aqt (==1.3.0.dev20230720000937)
-Requires-Dist: cirq-core (==1.3.0.dev20230720000937)
-Requires-Dist: cirq-ft (==1.3.0.dev20230720000937)
-Requires-Dist: cirq-google (==1.3.0.dev20230720000937)
-Requires-Dist: cirq-ionq (==1.3.0.dev20230720000937)
-Requires-Dist: cirq-pasqal (==1.3.0.dev20230720000937)
-Requires-Dist: cirq-rigetti (==1.3.0.dev20230720000937)
-Requires-Dist: cirq-web (==1.3.0.dev20230720000937)
+Requires-Dist: cirq-aqt (==1.3.0.dev20230722062259)
+Requires-Dist: cirq-core (==1.3.0.dev20230722062259)
+Requires-Dist: cirq-ft (==1.3.0.dev20230722062259)
+Requires-Dist: cirq-google (==1.3.0.dev20230722062259)
+Requires-Dist: cirq-ionq (==1.3.0.dev20230722062259)
+Requires-Dist: cirq-pasqal (==1.3.0.dev20230722062259)
+Requires-Dist: cirq-rigetti (==1.3.0.dev20230722062259)
+Requires-Dist: cirq-web (==1.3.0.dev20230722062259)
 Provides-Extra: dev_env
 Requires-Dist: mypy (==1.2.0) ; extra == 'dev_env'
 Requires-Dist: types-backports (==0.1.3) ; extra == 'dev_env'
 Requires-Dist: types-cachetools ; extra == 'dev_env'
 Requires-Dist: types-protobuf (==3.19.22) ; extra == 'dev_env'
 Requires-Dist: types-requests (==2.28.1) ; extra == 'dev_env'
 Requires-Dist: types-setuptools (==62.6.1) ; extra == 'dev_env'
 Requires-Dist: pytest ; extra == 'dev_env'
 Requires-Dist: pytest-asyncio ; extra == 'dev_env'
-Requires-Dist: pytest-cov ; extra == 'dev_env'
+Requires-Dist: pytest-cov (~=3.0) ; extra == 'dev_env'
 Requires-Dist: pytest-randomly ; extra == 'dev_env'
 Requires-Dist: coverage (<=6.2) ; extra == 'dev_env'
 Requires-Dist: pytest-xdist (~=2.2.0) ; extra == 'dev_env'
 Requires-Dist: filelock (~=3.0.12) ; extra == 'dev_env'
 Requires-Dist: freezegun (~=0.3.15) ; extra == 'dev_env'
 Requires-Dist: importlib-metadata ; extra == 'dev_env'
 Requires-Dist: virtualenv ; extra == 'dev_env'
```

