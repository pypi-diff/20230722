# Comparing `tmp/bizlogic-0.2.3.tar.gz` & `tmp/bizlogic-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bizlogic-0.2.3.tar", max compression
+gzip compressed data, was "bizlogic-0.2.4.tar", max compression
```

## Comparing `bizlogic-0.2.3.tar` & `bizlogic-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.2.3/LICENSE
--rw-r--r--   0        0        0     2182 2023-05-15 17:30:35.537449 bizlogic-0.2.3/README.md
--rw-r--r--   0        0        0      341 2023-07-22 13:06:56.529003 bizlogic-0.2.3/bizlogic/__init__.py
--rw-r--r--   0        0        0     5923 2023-05-15 17:30:35.537815 bizlogic-0.2.3/bizlogic/application.py
--rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.2.3/bizlogic/loan/__init__.py
--rw-r--r--   0        0        0     7494 2023-07-22 13:06:44.579916 bizlogic-0.2.3/bizlogic/loan/reader.py
--rw-r--r--   0        0        0     2742 2023-07-22 13:03:29.399551 bizlogic-0.2.3/bizlogic/loan/repayment.py
--rw-r--r--   0        0        0     1136 2023-07-22 13:03:29.400196 bizlogic-0.2.3/bizlogic/loan/status.py
--rw-r--r--   0        0        0     4269 2023-05-15 17:30:35.538679 bizlogic-0.2.3/bizlogic/loan/writer.py
--rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.2.3/bizlogic/protoc/__init__.py
--rw-r--r--   0        0        0     1053 2023-05-15 17:30:35.538935 bizlogic-0.2.3/bizlogic/protoc/loan_application_pb2.py
--rw-r--r--   0        0        0     1709 2023-05-14 16:41:31.172854 bizlogic-0.2.3/bizlogic/protoc/loan_pb2.py
--rw-r--r--   0        0        0      952 2023-05-15 17:30:35.539315 bizlogic-0.2.3/bizlogic/protoc/vouch_pb2.py
--rw-r--r--   0        0        0     3462 2023-07-22 13:03:29.401263 bizlogic-0.2.3/bizlogic/utils.py
--rw-r--r--   0        0        0     4165 2023-05-15 17:30:35.539612 bizlogic-0.2.3/bizlogic/vouch.py
--rw-r--r--   0        0        0      451 2023-07-22 13:06:51.076642 bizlogic-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 bizlogic-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2182 2023-05-15 17:30:35.537449 bizlogic-0.2.4/README.md
+-rw-r--r--   0        0        0      341 2023-07-22 13:08:48.995848 bizlogic-0.2.4/bizlogic/__init__.py
+-rw-r--r--   0        0        0     5923 2023-05-15 17:30:35.537815 bizlogic-0.2.4/bizlogic/application.py
+-rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.2.4/bizlogic/loan/__init__.py
+-rw-r--r--   0        0        0     7543 2023-07-22 13:08:38.469609 bizlogic-0.2.4/bizlogic/loan/reader.py
+-rw-r--r--   0        0        0     2742 2023-07-22 13:03:29.399551 bizlogic-0.2.4/bizlogic/loan/repayment.py
+-rw-r--r--   0        0        0     1136 2023-07-22 13:03:29.400196 bizlogic-0.2.4/bizlogic/loan/status.py
+-rw-r--r--   0        0        0     4269 2023-05-15 17:30:35.538679 bizlogic-0.2.4/bizlogic/loan/writer.py
+-rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.2.4/bizlogic/protoc/__init__.py
+-rw-r--r--   0        0        0     1053 2023-05-15 17:30:35.538935 bizlogic-0.2.4/bizlogic/protoc/loan_application_pb2.py
+-rw-r--r--   0        0        0     1709 2023-05-14 16:41:31.172854 bizlogic-0.2.4/bizlogic/protoc/loan_pb2.py
+-rw-r--r--   0        0        0      952 2023-05-15 17:30:35.539315 bizlogic-0.2.4/bizlogic/protoc/vouch_pb2.py
+-rw-r--r--   0        0        0     3462 2023-07-22 13:03:29.401263 bizlogic-0.2.4/bizlogic/utils.py
+-rw-r--r--   0        0        0     4165 2023-05-15 17:30:35.539612 bizlogic-0.2.4/bizlogic/vouch.py
+-rw-r--r--   0        0        0      451 2023-07-22 13:08:45.373041 bizlogic-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 bizlogic-0.2.4/PKG-INFO
```

### Comparing `bizlogic-0.2.3/LICENSE` & `bizlogic-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.3/README.md` & `bizlogic-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.3/bizlogic/application.py` & `bizlogic-0.2.4/bizlogic/application.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.3/bizlogic/loan/reader.py` & `bizlogic-0.2.4/bizlogic/loan/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,11 +242,12 @@
         loan_data = []
         for loan in loans:
             # convert the protobuf message to a Python dict
             loan_dict = MessageToDict(loan.reader)
             loan_data.append(loan_dict)
 
         # if recent_only is set to True, only return the most recent loan data
+        LOG.debug("Loan details: %s", loan_data)
         if recent_only and loan_data:
             loan_data = [max(loan_data, key=lambda row: row['created'])]
 
         return json.dumps(loan_data)
```

### Comparing `bizlogic-0.2.3/bizlogic/loan/repayment.py` & `bizlogic-0.2.4/bizlogic/loan/repayment.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.3/bizlogic/loan/status.py` & `bizlogic-0.2.4/bizlogic/loan/status.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.3/bizlogic/loan/writer.py` & `bizlogic-0.2.4/bizlogic/loan/writer.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.3/bizlogic/protoc/loan_application_pb2.py` & `bizlogic-0.2.4/bizlogic/protoc/loan_application_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.3/bizlogic/protoc/loan_pb2.py` & `bizlogic-0.2.4/bizlogic/protoc/loan_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.3/bizlogic/protoc/vouch_pb2.py` & `bizlogic-0.2.4/bizlogic/protoc/vouch_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.3/bizlogic/utils.py` & `bizlogic-0.2.4/bizlogic/utils.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.3/bizlogic/vouch.py` & `bizlogic-0.2.4/bizlogic/vouch.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.3/PKG-INFO` & `bizlogic-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bizlogic
-Version: 0.2.3
+Version: 0.2.4
 Summary: web3 lending platform business logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipfsclient (==0.0.7)
```

