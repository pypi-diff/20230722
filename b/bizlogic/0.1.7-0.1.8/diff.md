# Comparing `tmp/bizlogic-0.1.7.tar.gz` & `tmp/bizlogic-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bizlogic-0.1.7.tar", max compression
+gzip compressed data, was "bizlogic-0.1.8.tar", max compression
```

## Comparing `bizlogic-0.1.7.tar` & `bizlogic-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.1.7/LICENSE
--rw-r--r--   0        0        0     2182 2023-05-15 17:30:35.537449 bizlogic-0.1.7/README.md
--rw-r--r--   0        0        0      341 2023-07-22 00:16:54.421205 bizlogic-0.1.7/bizlogic/__init__.py
--rw-r--r--   0        0        0     5923 2023-05-15 17:30:35.537815 bizlogic-0.1.7/bizlogic/application.py
--rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.1.7/bizlogic/loan/__init__.py
--rw-r--r--   0        0        0     6253 2023-07-22 00:16:36.706205 bizlogic-0.1.7/bizlogic/loan/reader.py
--rw-r--r--   0        0        0     2742 2023-07-16 23:08:16.349583 bizlogic-0.1.7/bizlogic/loan/repayment.py
--rw-r--r--   0        0        0     1573 2023-07-17 01:38:32.073711 bizlogic-0.1.7/bizlogic/loan/status.py
--rw-r--r--   0        0        0     4269 2023-05-15 17:30:35.538679 bizlogic-0.1.7/bizlogic/loan/writer.py
--rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.1.7/bizlogic/protoc/__init__.py
--rw-r--r--   0        0        0     1053 2023-05-15 17:30:35.538935 bizlogic-0.1.7/bizlogic/protoc/loan_application_pb2.py
--rw-r--r--   0        0        0     1709 2023-05-14 16:41:31.172854 bizlogic-0.1.7/bizlogic/protoc/loan_pb2.py
--rw-r--r--   0        0        0      952 2023-05-15 17:30:35.539315 bizlogic-0.1.7/bizlogic/protoc/vouch_pb2.py
--rw-r--r--   0        0        0     3462 2023-07-21 23:57:34.968269 bizlogic-0.1.7/bizlogic/utils.py
--rw-r--r--   0        0        0     4165 2023-05-15 17:30:35.539612 bizlogic-0.1.7/bizlogic/vouch.py
--rw-r--r--   0        0        0      451 2023-07-22 00:16:49.364972 bizlogic-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 bizlogic-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2182 2023-05-15 17:30:35.537449 bizlogic-0.1.8/README.md
+-rw-r--r--   0        0        0      341 2023-07-22 00:20:18.673992 bizlogic-0.1.8/bizlogic/__init__.py
+-rw-r--r--   0        0        0     5923 2023-05-15 17:30:35.537815 bizlogic-0.1.8/bizlogic/application.py
+-rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.1.8/bizlogic/loan/__init__.py
+-rw-r--r--   0        0        0     6253 2023-07-22 00:16:36.706205 bizlogic-0.1.8/bizlogic/loan/reader.py
+-rw-r--r--   0        0        0     2742 2023-07-16 23:08:16.349583 bizlogic-0.1.8/bizlogic/loan/repayment.py
+-rw-r--r--   0        0        0     1561 2023-07-22 00:20:01.546093 bizlogic-0.1.8/bizlogic/loan/status.py
+-rw-r--r--   0        0        0     4269 2023-05-15 17:30:35.538679 bizlogic-0.1.8/bizlogic/loan/writer.py
+-rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.1.8/bizlogic/protoc/__init__.py
+-rw-r--r--   0        0        0     1053 2023-05-15 17:30:35.538935 bizlogic-0.1.8/bizlogic/protoc/loan_application_pb2.py
+-rw-r--r--   0        0        0     1709 2023-05-14 16:41:31.172854 bizlogic-0.1.8/bizlogic/protoc/loan_pb2.py
+-rw-r--r--   0        0        0      952 2023-05-15 17:30:35.539315 bizlogic-0.1.8/bizlogic/protoc/vouch_pb2.py
+-rw-r--r--   0        0        0     3462 2023-07-21 23:57:34.968269 bizlogic-0.1.8/bizlogic/utils.py
+-rw-r--r--   0        0        0     4165 2023-05-15 17:30:35.539612 bizlogic-0.1.8/bizlogic/vouch.py
+-rw-r--r--   0        0        0      451 2023-07-22 00:20:14.990636 bizlogic-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 bizlogic-0.1.8/PKG-INFO
```

### Comparing `bizlogic-0.1.7/LICENSE` & `bizlogic-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.7/README.md` & `bizlogic-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.7/bizlogic/application.py` & `bizlogic-0.1.8/bizlogic/application.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.7/bizlogic/loan/reader.py` & `bizlogic-0.1.8/bizlogic/loan/reader.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.7/bizlogic/loan/repayment.py` & `bizlogic-0.1.8/bizlogic/loan/repayment.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.7/bizlogic/loan/status.py` & `bizlogic-0.1.8/bizlogic/loan/status.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,19 +38,19 @@
         Args:
             loan: the loan
 
         Returns:
             LoanStatusType: the status of the loan
         """
         now = datetime.now()
-        expiry = LoanStatus._timestamp_to_datetime(loan['offer_expiry'])
+        expiry = LoanStatus._timestamp_to_datetime(loan.offer_expiry)
 
-        if expiry > now and not loan['accepted']:  # if the loan has not expired and is not accepted
+        if expiry > now and not loan.accepted:  # if the loan has not expired and is not accepted
             return LoanStatusType.PENDING_ACCEPTANCE
 
-        elif expiry <= now and not loan['accepted']:  # if the loan has expired and is not accepted
+        elif expiry <= now and not loan.accepted:  # if the loan has expired and is not accepted
             return LoanStatusType.EXPIRED_UNACCEPTED
 
-        elif loan['accepted']:  # if the loan is accepted, regardless of expiry
+        elif loan.accepted:  # if the loan is accepted, regardless of expiry
             return LoanStatusType.ACCEPTED
 
         raise ValueError("Unable to determine loan status")
```

### Comparing `bizlogic-0.1.7/bizlogic/loan/writer.py` & `bizlogic-0.1.8/bizlogic/loan/writer.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.7/bizlogic/protoc/loan_application_pb2.py` & `bizlogic-0.1.8/bizlogic/protoc/loan_application_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.7/bizlogic/protoc/loan_pb2.py` & `bizlogic-0.1.8/bizlogic/protoc/loan_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.7/bizlogic/protoc/vouch_pb2.py` & `bizlogic-0.1.8/bizlogic/protoc/vouch_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.7/bizlogic/utils.py` & `bizlogic-0.1.8/bizlogic/utils.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.7/bizlogic/vouch.py` & `bizlogic-0.1.8/bizlogic/vouch.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.7/PKG-INFO` & `bizlogic-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bizlogic
-Version: 0.1.7
+Version: 0.1.8
 Summary: web3 lending platform business logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipfsclient (==0.0.7)
```

