# Comparing `tmp/bizlogic-0.2.0.tar.gz` & `tmp/bizlogic-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bizlogic-0.2.0.tar", max compression
+gzip compressed data, was "bizlogic-0.2.1.tar", max compression
```

## Comparing `bizlogic-0.2.0.tar` & `bizlogic-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.2.0/LICENSE
--rw-r--r--   0        0        0     2182 2023-05-15 17:30:35.537449 bizlogic-0.2.0/README.md
--rw-r--r--   0        0        0      341 2023-07-22 00:26:07.576378 bizlogic-0.2.0/bizlogic/__init__.py
--rw-r--r--   0        0        0     5923 2023-05-15 17:30:35.537815 bizlogic-0.2.0/bizlogic/application.py
--rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.2.0/bizlogic/loan/__init__.py
--rw-r--r--   0        0        0     6216 2023-07-22 00:25:50.621225 bizlogic-0.2.0/bizlogic/loan/reader.py
--rw-r--r--   0        0        0     2742 2023-07-16 23:08:16.349583 bizlogic-0.2.0/bizlogic/loan/repayment.py
--rw-r--r--   0        0        0     1573 2023-07-22 00:23:39.725425 bizlogic-0.2.0/bizlogic/loan/status.py
--rw-r--r--   0        0        0     4269 2023-05-15 17:30:35.538679 bizlogic-0.2.0/bizlogic/loan/writer.py
--rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.2.0/bizlogic/protoc/__init__.py
--rw-r--r--   0        0        0     1053 2023-05-15 17:30:35.538935 bizlogic-0.2.0/bizlogic/protoc/loan_application_pb2.py
--rw-r--r--   0        0        0     1709 2023-05-14 16:41:31.172854 bizlogic-0.2.0/bizlogic/protoc/loan_pb2.py
--rw-r--r--   0        0        0      952 2023-05-15 17:30:35.539315 bizlogic-0.2.0/bizlogic/protoc/vouch_pb2.py
--rw-r--r--   0        0        0     3462 2023-07-21 23:57:34.968269 bizlogic-0.2.0/bizlogic/utils.py
--rw-r--r--   0        0        0     4165 2023-05-15 17:30:35.539612 bizlogic-0.2.0/bizlogic/vouch.py
--rw-r--r--   0        0        0      451 2023-07-22 00:26:01.357915 bizlogic-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 bizlogic-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2182 2023-05-15 17:30:35.537449 bizlogic-0.2.1/README.md
+-rw-r--r--   0        0        0      341 2023-07-22 00:29:04.167923 bizlogic-0.2.1/bizlogic/__init__.py
+-rw-r--r--   0        0        0     5923 2023-05-15 17:30:35.537815 bizlogic-0.2.1/bizlogic/application.py
+-rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.2.1/bizlogic/loan/__init__.py
+-rw-r--r--   0        0        0     6216 2023-07-22 00:25:50.621225 bizlogic-0.2.1/bizlogic/loan/reader.py
+-rw-r--r--   0        0        0     2742 2023-07-16 23:08:16.349583 bizlogic-0.2.1/bizlogic/loan/repayment.py
+-rw-r--r--   0        0        0     1136 2023-07-22 00:28:44.429947 bizlogic-0.2.1/bizlogic/loan/status.py
+-rw-r--r--   0        0        0     4269 2023-05-15 17:30:35.538679 bizlogic-0.2.1/bizlogic/loan/writer.py
+-rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.2.1/bizlogic/protoc/__init__.py
+-rw-r--r--   0        0        0     1053 2023-05-15 17:30:35.538935 bizlogic-0.2.1/bizlogic/protoc/loan_application_pb2.py
+-rw-r--r--   0        0        0     1709 2023-05-14 16:41:31.172854 bizlogic-0.2.1/bizlogic/protoc/loan_pb2.py
+-rw-r--r--   0        0        0      952 2023-05-15 17:30:35.539315 bizlogic-0.2.1/bizlogic/protoc/vouch_pb2.py
+-rw-r--r--   0        0        0     3462 2023-07-21 23:57:34.968269 bizlogic-0.2.1/bizlogic/utils.py
+-rw-r--r--   0        0        0     4165 2023-05-15 17:30:35.539612 bizlogic-0.2.1/bizlogic/vouch.py
+-rw-r--r--   0        0        0      451 2023-07-22 00:29:00.428181 bizlogic-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 bizlogic-0.2.1/PKG-INFO
```

### Comparing `bizlogic-0.2.0/LICENSE` & `bizlogic-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.0/README.md` & `bizlogic-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.0/bizlogic/application.py` & `bizlogic-0.2.1/bizlogic/application.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.0/bizlogic/loan/reader.py` & `bizlogic-0.2.1/bizlogic/loan/reader.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.0/bizlogic/loan/repayment.py` & `bizlogic-0.2.1/bizlogic/loan/repayment.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.0/bizlogic/loan/writer.py` & `bizlogic-0.2.1/bizlogic/loan/writer.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.0/bizlogic/protoc/loan_application_pb2.py` & `bizlogic-0.2.1/bizlogic/protoc/loan_application_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.0/bizlogic/protoc/loan_pb2.py` & `bizlogic-0.2.1/bizlogic/protoc/loan_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.0/bizlogic/protoc/vouch_pb2.py` & `bizlogic-0.2.1/bizlogic/protoc/vouch_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.0/bizlogic/utils.py` & `bizlogic-0.2.1/bizlogic/utils.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.0/bizlogic/vouch.py` & `bizlogic-0.2.1/bizlogic/vouch.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.0/PKG-INFO` & `bizlogic-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bizlogic
-Version: 0.2.0
+Version: 0.2.1
 Summary: web3 lending platform business logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipfsclient (==0.0.7)
```

