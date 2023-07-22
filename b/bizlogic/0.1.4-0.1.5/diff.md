# Comparing `tmp/bizlogic-0.1.4.tar.gz` & `tmp/bizlogic-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bizlogic-0.1.4.tar", max compression
+gzip compressed data, was "bizlogic-0.1.5.tar", max compression
```

## Comparing `bizlogic-0.1.4.tar` & `bizlogic-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.1.4/LICENSE
--rw-r--r--   0        0        0     2182 2023-05-15 17:30:35.537449 bizlogic-0.1.4/README.md
--rw-r--r--   0        0        0      341 2023-07-17 01:39:01.940531 bizlogic-0.1.4/bizlogic/__init__.py
--rw-r--r--   0        0        0     5923 2023-05-15 17:30:35.537815 bizlogic-0.1.4/bizlogic/application.py
--rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.1.4/bizlogic/loan/__init__.py
--rw-r--r--   0        0        0     6063 2023-07-17 01:35:25.436885 bizlogic-0.1.4/bizlogic/loan/reader.py
--rw-r--r--   0        0        0     2742 2023-07-16 23:08:16.349583 bizlogic-0.1.4/bizlogic/loan/repayment.py
--rw-r--r--   0        0        0     1573 2023-07-17 01:38:32.073711 bizlogic-0.1.4/bizlogic/loan/status.py
--rw-r--r--   0        0        0     4269 2023-05-15 17:30:35.538679 bizlogic-0.1.4/bizlogic/loan/writer.py
--rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.1.4/bizlogic/protoc/__init__.py
--rw-r--r--   0        0        0     1053 2023-05-15 17:30:35.538935 bizlogic-0.1.4/bizlogic/protoc/loan_application_pb2.py
--rw-r--r--   0        0        0     1709 2023-05-14 16:41:31.172854 bizlogic-0.1.4/bizlogic/protoc/loan_pb2.py
--rw-r--r--   0        0        0      952 2023-05-15 17:30:35.539315 bizlogic-0.1.4/bizlogic/protoc/vouch_pb2.py
--rw-r--r--   0        0        0     3337 2023-05-15 17:30:35.539448 bizlogic-0.1.4/bizlogic/utils.py
--rw-r--r--   0        0        0     4165 2023-05-15 17:30:35.539612 bizlogic-0.1.4/bizlogic/vouch.py
--rw-r--r--   0        0        0      451 2023-07-17 01:38:58.342660 bizlogic-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 bizlogic-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2182 2023-05-15 17:30:35.537449 bizlogic-0.1.5/README.md
+-rw-r--r--   0        0        0      341 2023-07-21 23:58:05.619345 bizlogic-0.1.5/bizlogic/__init__.py
+-rw-r--r--   0        0        0     5923 2023-05-15 17:30:35.537815 bizlogic-0.1.5/bizlogic/application.py
+-rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.1.5/bizlogic/loan/__init__.py
+-rw-r--r--   0        0        0     6063 2023-07-17 01:35:25.436885 bizlogic-0.1.5/bizlogic/loan/reader.py
+-rw-r--r--   0        0        0     2742 2023-07-16 23:08:16.349583 bizlogic-0.1.5/bizlogic/loan/repayment.py
+-rw-r--r--   0        0        0     1573 2023-07-17 01:38:32.073711 bizlogic-0.1.5/bizlogic/loan/status.py
+-rw-r--r--   0        0        0     4269 2023-05-15 17:30:35.538679 bizlogic-0.1.5/bizlogic/loan/writer.py
+-rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.1.5/bizlogic/protoc/__init__.py
+-rw-r--r--   0        0        0     1053 2023-05-15 17:30:35.538935 bizlogic-0.1.5/bizlogic/protoc/loan_application_pb2.py
+-rw-r--r--   0        0        0     1709 2023-05-14 16:41:31.172854 bizlogic-0.1.5/bizlogic/protoc/loan_pb2.py
+-rw-r--r--   0        0        0      952 2023-05-15 17:30:35.539315 bizlogic-0.1.5/bizlogic/protoc/vouch_pb2.py
+-rw-r--r--   0        0        0     3462 2023-07-21 23:57:34.968269 bizlogic-0.1.5/bizlogic/utils.py
+-rw-r--r--   0        0        0     4165 2023-05-15 17:30:35.539612 bizlogic-0.1.5/bizlogic/vouch.py
+-rw-r--r--   0        0        0      451 2023-07-21 23:58:01.374410 bizlogic-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 bizlogic-0.1.5/PKG-INFO
```

### Comparing `bizlogic-0.1.4/LICENSE` & `bizlogic-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.4/README.md` & `bizlogic-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.4/bizlogic/application.py` & `bizlogic-0.1.5/bizlogic/application.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.4/bizlogic/loan/reader.py` & `bizlogic-0.1.5/bizlogic/loan/reader.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.4/bizlogic/loan/repayment.py` & `bizlogic-0.1.5/bizlogic/loan/repayment.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.4/bizlogic/loan/status.py` & `bizlogic-0.1.5/bizlogic/loan/status.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.4/bizlogic/loan/writer.py` & `bizlogic-0.1.5/bizlogic/loan/writer.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.4/bizlogic/protoc/loan_application_pb2.py` & `bizlogic-0.1.5/bizlogic/protoc/loan_application_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.4/bizlogic/protoc/loan_pb2.py` & `bizlogic-0.1.5/bizlogic/protoc/loan_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.4/bizlogic/protoc/vouch_pb2.py` & `bizlogic-0.1.5/bizlogic/protoc/vouch_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.4/bizlogic/utils.py` & `bizlogic-0.1.5/bizlogic/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import datetime
 
 from ipfskvs.store import Store
 
 import pandas as pd
 
+import logging
+
+LOG = logging.getLogger(__name__)
+LOG.setLevel(logging.DEBUG)
+
 
 class ParserType:
     """The type of protobuf object."""
 
     LOAN_APPLICATION = 1
     LOAN = 2
     VOUCH = 3
@@ -80,14 +85,15 @@
 
         Args:
             store (Store): The store object to parse
 
         Returns:
             datetime.date: The offer expiry
         """
+        LOG.debug(f"Parsing: {store.reader}")
         return datetime.datetime.fromtimestamp(
             store.reader.offer_expiry.seconds + store.reader.offer_expiry.nanos / 1e9  # noqa: E501
         )
 
 
 PARSERS = {
     ParserType.LOAN_APPLICATION: {
```

### Comparing `bizlogic-0.1.4/bizlogic/vouch.py` & `bizlogic-0.1.5/bizlogic/vouch.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.4/PKG-INFO` & `bizlogic-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bizlogic
-Version: 0.1.4
+Version: 0.1.5
 Summary: web3 lending platform business logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipfsclient (==0.0.7)
```

