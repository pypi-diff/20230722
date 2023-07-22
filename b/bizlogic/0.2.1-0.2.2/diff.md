# Comparing `tmp/bizlogic-0.2.1.tar.gz` & `tmp/bizlogic-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bizlogic-0.2.1.tar", max compression
+gzip compressed data, was "bizlogic-0.2.2.tar", max compression
```

## Comparing `bizlogic-0.2.1.tar` & `bizlogic-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.2.1/LICENSE
--rw-r--r--   0        0        0     2182 2023-05-15 17:30:35.537449 bizlogic-0.2.1/README.md
--rw-r--r--   0        0        0      341 2023-07-22 00:29:04.167923 bizlogic-0.2.1/bizlogic/__init__.py
--rw-r--r--   0        0        0     5923 2023-05-15 17:30:35.537815 bizlogic-0.2.1/bizlogic/application.py
--rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.2.1/bizlogic/loan/__init__.py
--rw-r--r--   0        0        0     6216 2023-07-22 00:25:50.621225 bizlogic-0.2.1/bizlogic/loan/reader.py
--rw-r--r--   0        0        0     2742 2023-07-16 23:08:16.349583 bizlogic-0.2.1/bizlogic/loan/repayment.py
--rw-r--r--   0        0        0     1136 2023-07-22 00:28:44.429947 bizlogic-0.2.1/bizlogic/loan/status.py
--rw-r--r--   0        0        0     4269 2023-05-15 17:30:35.538679 bizlogic-0.2.1/bizlogic/loan/writer.py
--rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.2.1/bizlogic/protoc/__init__.py
--rw-r--r--   0        0        0     1053 2023-05-15 17:30:35.538935 bizlogic-0.2.1/bizlogic/protoc/loan_application_pb2.py
--rw-r--r--   0        0        0     1709 2023-05-14 16:41:31.172854 bizlogic-0.2.1/bizlogic/protoc/loan_pb2.py
--rw-r--r--   0        0        0      952 2023-05-15 17:30:35.539315 bizlogic-0.2.1/bizlogic/protoc/vouch_pb2.py
--rw-r--r--   0        0        0     3462 2023-07-21 23:57:34.968269 bizlogic-0.2.1/bizlogic/utils.py
--rw-r--r--   0        0        0     4165 2023-05-15 17:30:35.539612 bizlogic-0.2.1/bizlogic/vouch.py
--rw-r--r--   0        0        0      451 2023-07-22 00:29:00.428181 bizlogic-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 bizlogic-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2182 2023-05-15 17:30:35.537449 bizlogic-0.2.2/README.md
+-rw-r--r--   0        0        0      341 2023-07-22 12:58:36.931514 bizlogic-0.2.2/bizlogic/__init__.py
+-rw-r--r--   0        0        0     5923 2023-05-15 17:30:35.537815 bizlogic-0.2.2/bizlogic/application.py
+-rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.2.2/bizlogic/loan/__init__.py
+-rw-r--r--   0        0        0     7493 2023-07-22 12:49:17.705921 bizlogic-0.2.2/bizlogic/loan/reader.py
+-rw-r--r--   0        0        0     2742 2023-07-16 23:08:16.349583 bizlogic-0.2.2/bizlogic/loan/repayment.py
+-rw-r--r--   0        0        0     1136 2023-07-22 00:28:44.429947 bizlogic-0.2.2/bizlogic/loan/status.py
+-rw-r--r--   0        0        0     4269 2023-05-15 17:30:35.538679 bizlogic-0.2.2/bizlogic/loan/writer.py
+-rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.2.2/bizlogic/protoc/__init__.py
+-rw-r--r--   0        0        0     1053 2023-05-15 17:30:35.538935 bizlogic-0.2.2/bizlogic/protoc/loan_application_pb2.py
+-rw-r--r--   0        0        0     1709 2023-05-14 16:41:31.172854 bizlogic-0.2.2/bizlogic/protoc/loan_pb2.py
+-rw-r--r--   0        0        0      952 2023-05-15 17:30:35.539315 bizlogic-0.2.2/bizlogic/protoc/vouch_pb2.py
+-rw-r--r--   0        0        0     3462 2023-07-21 23:57:34.968269 bizlogic-0.2.2/bizlogic/utils.py
+-rw-r--r--   0        0        0     4165 2023-05-15 17:30:35.539612 bizlogic-0.2.2/bizlogic/vouch.py
+-rw-r--r--   0        0        0      451 2023-07-22 12:58:31.631164 bizlogic-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 bizlogic-0.2.2/PKG-INFO
```

### Comparing `bizlogic-0.2.1/LICENSE` & `bizlogic-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.1/README.md` & `bizlogic-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.1/bizlogic/application.py` & `bizlogic-0.2.2/bizlogic/application.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.1/bizlogic/loan/reader.py` & `bizlogic-0.2.2/bizlogic/loan/reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 
-from typing import Self
+from typing import List, Self
+import json
+
+from google.protobuf.json_format import MessageToDict
 
 from bizlogic.loan import PREFIX
 from bizlogic.loan.status import LoanStatus, LoanStatusType
 from bizlogic.protoc.loan_pb2 import Loan
 from bizlogic.utils import GROUP_BY, PARSERS, ParserType, Utils
 
 from ipfsclient.ipfs import Ipfs
@@ -38,15 +41,15 @@
             recent_only (bool, optional): Include previous updates or
                 only get the most recent. Defaults to True.
 
         Returns:
             pd.DataFrame: The open loan offers for the borrower.
         """
         return self.query_for_status(
-            status=LoanStatus.PENDING_ACCEPTANCE,
+            status=LoanStatusType.PENDING_ACCEPTANCE,
             index=Index(
                 prefix=PREFIX,
                 index={
                     "borrower": borrower
                 },
                 size=3
             ),
@@ -205,7 +208,45 @@
             return df
 
         # filter for most recent applications per loan_id
         if recent_only:
             df = Utils.get_most_recent(df, GROUP_BY[ParserType.LOAN])
 
         return df
+
+    def query_for_loan_details(
+            self: Self,
+            loan_id: str,
+            recent_only: bool = True) -> List[Loan]:
+        """Query for a specific loan and return all the loan data.
+
+        Args:
+            loan_id (str): The loan to query for.
+            recent_only (bool, optional): Include previous updates or
+                only get the most recent. Defaults to True.
+
+        Returns:
+            str: The loan with the specified id in JSON format.
+        """
+        loans = Store.query(
+            query_index=Index(
+                prefix=PREFIX,
+                index={
+                    "loan": loan_id
+                },
+                size=3
+            ),
+            ipfs=self.ipfsclient,
+            reader=Loan()
+        )
+
+        loan_data = []
+        for loan in loans:
+            # convert the protobuf message to a Python dict
+            loan_dict = MessageToDict(loan.reader)
+            loan_data.append(loan_dict)
+
+        # if recent_only is set to True, only return the most recent loan data
+        if recent_only and loan_data:
+            loan_data = [max(loan_data, key=lambda x: x['updateTime'])]
+
+        return json.dumps(loan_data)
```

### Comparing `bizlogic-0.2.1/bizlogic/loan/repayment.py` & `bizlogic-0.2.2/bizlogic/loan/repayment.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.1/bizlogic/loan/status.py` & `bizlogic-0.2.2/bizlogic/loan/status.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.1/bizlogic/loan/writer.py` & `bizlogic-0.2.2/bizlogic/loan/writer.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.1/bizlogic/protoc/loan_application_pb2.py` & `bizlogic-0.2.2/bizlogic/protoc/loan_application_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.1/bizlogic/protoc/loan_pb2.py` & `bizlogic-0.2.2/bizlogic/protoc/loan_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.1/bizlogic/protoc/vouch_pb2.py` & `bizlogic-0.2.2/bizlogic/protoc/vouch_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.1/bizlogic/utils.py` & `bizlogic-0.2.2/bizlogic/utils.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.1/bizlogic/vouch.py` & `bizlogic-0.2.2/bizlogic/vouch.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.2.1/PKG-INFO` & `bizlogic-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bizlogic
-Version: 0.2.1
+Version: 0.2.2
 Summary: web3 lending platform business logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipfsclient (==0.0.7)
```

