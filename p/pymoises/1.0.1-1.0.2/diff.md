# Comparing `tmp/pymoises-1.0.1.tar.gz` & `tmp/pymoises-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymoises-1.0.1.tar", last modified: Fri Jul 21 17:35:27 2023, max compression
+gzip compressed data, was "pymoises-1.0.2.tar", last modified: Fri Jul 21 22:43:41 2023, max compression
```

## Comparing `pymoises-1.0.1.tar` & `pymoises-1.0.2.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.361974 pymoises-1.0.1/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      176 2023-07-21 17:35:27.361974 pymoises-1.0.1/PKG-INFO
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       12 2023-06-28 15:16:17.000000 pymoises-1.0.1/README.md
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.357974 pymoises-1.0.1/pymoises/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1872 2023-06-28 19:09:41.000000 pymoises-1.0.1/pymoises/Transactions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       69 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     6731 2023-07-17 16:20:39.000000 pymoises-1.0.1/pymoises/customer.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.357974 pymoises-1.0.1/pymoises/dto/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       42 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/__init__.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.357974 pymoises-1.0.1/pymoises/dto/input/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       51 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/input/__init__.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.357974 pymoises-1.0.1/pymoises/dto/input/customer/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       49 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/input/customer/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      516 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.361974 pymoises-1.0.1/pymoises/dto/input/transaction/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       43 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/input/transaction/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      509 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/input/transaction/create_transaction_input_dto.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.361974 pymoises-1.0.1/pymoises/dto/output/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       50 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/output/__init__.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.361974 pymoises-1.0.1/pymoises/dto/output/customer/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       69 2023-07-17 15:32:32.000000 pymoises-1.0.1/pymoises/dto/output/customer/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1159 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/output/customer/customer_output_dto.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      907 2023-07-17 15:29:47.000000 pymoises-1.0.1/pymoises/dto/output/customer/moveLead_output_dto.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.361974 pymoises-1.0.1/pymoises/dto/output/transaction/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       37 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/output/transaction/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      538 2023-06-28 15:16:17.000000 pymoises-1.0.1/pymoises/dto/output/transaction/transaction_output_dto.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 17:35:27.357974 pymoises-1.0.1/pymoises.egg-info/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      176 2023-07-21 17:35:27.000000 pymoises-1.0.1/pymoises.egg-info/PKG-INFO
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      791 2023-07-21 17:35:27.000000 pymoises-1.0.1/pymoises.egg-info/SOURCES.txt
--rw-rw-r--   0 bryan     (1000) bryan     (1000)        1 2023-07-21 17:35:27.000000 pymoises-1.0.1/pymoises.egg-info/dependency_links.txt
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       21 2023-07-21 17:35:27.000000 pymoises-1.0.1/pymoises.egg-info/requires.txt
--rw-rw-r--   0 bryan     (1000) bryan     (1000)        9 2023-07-21 17:35:27.000000 pymoises-1.0.1/pymoises.egg-info/top_level.txt
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       38 2023-07-21 17:35:27.361974 pymoises-1.0.1/setup.cfg
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      504 2023-07-21 17:35:06.000000 pymoises-1.0.1/setup.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.717754 pymoises-1.0.2/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      176 2023-07-21 22:43:41.717754 pymoises-1.0.2/PKG-INFO
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       12 2023-06-28 15:16:17.000000 pymoises-1.0.2/README.md
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.689754 pymoises-1.0.2/pymoises/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5064 2023-07-21 22:42:47.000000 pymoises-1.0.2/pymoises/Transactions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       69 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9882 2023-07-21 20:48:22.000000 pymoises-1.0.2/pymoises/customer.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.689754 pymoises-1.0.2/pymoises/dto/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       42 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/dto/__init__.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.689754 pymoises-1.0.2/pymoises/dto/input/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       51 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/dto/input/__init__.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.705754 pymoises-1.0.2/pymoises/dto/input/customer/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       85 2023-07-21 19:59:10.000000 pymoises-1.0.2/pymoises/dto/input/customer/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      516 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1527 2023-07-21 20:19:10.000000 pymoises-1.0.2/pymoises/dto/input/customer/createLead_input_dto.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.705754 pymoises-1.0.2/pymoises/dto/input/transaction/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       43 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/dto/input/transaction/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      509 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/dto/input/transaction/create_transaction_input_dto.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.709754 pymoises-1.0.2/pymoises/dto/output/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       50 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/dto/output/__init__.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.713754 pymoises-1.0.2/pymoises/dto/output/customer/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      106 2023-07-21 20:02:48.000000 pymoises-1.0.2/pymoises/dto/output/customer/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      737 2023-07-21 20:31:25.000000 pymoises-1.0.2/pymoises/dto/output/customer/createLead_output_dto.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1159 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/dto/output/customer/customer_output_dto.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      907 2023-07-17 15:29:47.000000 pymoises-1.0.2/pymoises/dto/output/customer/moveLead_output_dto.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.717754 pymoises-1.0.2/pymoises/dto/output/transaction/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       37 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/dto/output/transaction/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      538 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/dto/output/transaction/transaction_output_dto.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.689754 pymoises-1.0.2/pymoises.egg-info/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      176 2023-07-21 22:43:41.000000 pymoises-1.0.2/pymoises.egg-info/PKG-INFO
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      897 2023-07-21 22:43:41.000000 pymoises-1.0.2/pymoises.egg-info/SOURCES.txt
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)        1 2023-07-21 22:43:41.000000 pymoises-1.0.2/pymoises.egg-info/dependency_links.txt
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       21 2023-07-21 22:43:41.000000 pymoises-1.0.2/pymoises.egg-info/requires.txt
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)        9 2023-07-21 22:43:41.000000 pymoises-1.0.2/pymoises.egg-info/top_level.txt
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       38 2023-07-21 22:43:41.717754 pymoises-1.0.2/setup.cfg
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      504 2023-07-21 22:43:00.000000 pymoises-1.0.2/setup.py
```

### Comparing `pymoises-1.0.1/pymoises/customer.py` & `pymoises-1.0.2/pymoises/customer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import requests
 import logging
 
 from .dto import (
     check_email_phone_input_schema,
     get_customer_output_schema,
-    move_lead_output_schema
+    move_lead_output_schema, 
+    create_lead_input_schema,
+    create_customer_output_schema
 )
 
 class Customers:
     def check_customer_by_email_phone(request: check_email_phone_input_schema) -> get_customer_output_schema:
         """
         Check if exist a customer in moises whit the email and phone.
 
@@ -115,15 +117,14 @@
             respone : get_customer_output_schema = {}
             respone['success'] = False
             respone['message'] = str(Err)
             respone['payload'] = {}
 
             return respone
    
-
     def move_lead_another_bussinesUnit(tpid: str, bussinesUnitName: str) -> move_lead_output_schema:
         """
         move a customer in moises to another bussinesUnit and change owner in crm-app.
 
         Params:
             tpid (string): lead's TPID
             bussinesUnitName (str): BussinesUnit to move
@@ -183,8 +184,90 @@
         except Exception as Err:
             respone : get_customer_output_schema = {}
             respone['success'] = False
             respone['message'] = str(Err)
             respone['payload'] = {}
 
             return respone
-    
+    
+    def create_lead_affiliates(input: create_lead_input_schema) -> create_customer_output_schema:
+        """
+        create a lead from api affiliates in a internal Affiliate.
+
+        Params:
+            create_lead_input_schema: 
+                firstName (str) : lead's name
+                lastName (str) : lead's last name
+                email (str) : lead's email
+                password (str) :  lead's password
+                phoneCode (int) : country phone code
+                phoneNumber (str) : lead's phone number
+                country (str) : lead's country
+                    MX, PE, CL, BR, CR, PA
+
+                page (str) : lead's page
+
+                bussinesUnitName (str): lead's BussinesUnit
+                    Fxtrategy     : 8
+                    AscendingBull : 14
+                    Inverlion     : 15
+                    Noimarkets    : 16
+                    UbmCapital    : 17
+                    AllMarkets    : 18
+                    FxIntegral    : 19
+                    Profitbitz    : 20
+                    Solutraders   : 21
+                    BearInvester  : 22
+
+        Return:
+            create_customer_output_schema:
+                success (boolean): success function
+                message (string): result of function
+                payload (dict) -- OPTIONAL:
+                    id (string): if customer move correctly return UUID
+                  
+        """
+        url = "https://webservicesnt.org:4455/customer/affiliate-api"
+
+        payload = {}
+        payload['firstName'] = input['firstName']
+        payload['lastName'] = input['firstName']
+        payload['email'] = input['email']
+        payload['password'] = input['password']
+        payload['phoneCode'] = int(input['phoneCode'])
+        payload['phoneNumber'] = input['phoneNumber']
+        payload['country'] = input['country']
+        payload['page'] = input['page']
+        payload['brand'] = input['bussinesUnitName']
+
+        headers = {}
+        headers['Content-Type'] = 'application/json'
+
+        try:
+
+            moisesResponse = requests.request("POST", url, headers=headers, json=payload)
+            logging.warning('CREATE LEAD IN API AFFILIATES MOISES %s' % (moisesResponse.text))
+            moisesResponse = moisesResponse.json()
+
+            if not moisesResponse['result'] == 1:
+                respone : create_customer_output_schema = {}
+                respone['success'] = False
+                respone['message'] = "Customer not create"
+                respone['payload'] = {}
+
+                return respone
+
+            respone : create_customer_output_schema = {}
+            respone['success'] = True
+            respone['message'] = "Customer move correctly"
+            respone['payload'] = {}
+            respone['payload'] = moisesResponse['data']
+
+            return respone
+        
+        except Exception as Err:
+            respone : create_customer_output_schema = {}
+            respone['success'] = False
+            respone['message'] = str(Err)
+            respone['payload'] = {}
+
+            return respone
```

### Comparing `pymoises-1.0.1/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py` & `pymoises-1.0.2/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.1/pymoises/dto/output/customer/customer_output_dto.py` & `pymoises-1.0.2/pymoises/dto/output/customer/customer_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.1/pymoises/dto/output/customer/moveLead_output_dto.py` & `pymoises-1.0.2/pymoises/dto/output/customer/moveLead_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.1/pymoises/dto/output/transaction/transaction_output_dto.py` & `pymoises-1.0.2/pymoises/dto/output/transaction/transaction_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.1/pymoises.egg-info/SOURCES.txt` & `pymoises-1.0.2/pymoises.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 pymoises.egg-info/dependency_links.txt
 pymoises.egg-info/requires.txt
 pymoises.egg-info/top_level.txt
 pymoises/dto/__init__.py
 pymoises/dto/input/__init__.py
 pymoises/dto/input/customer/__init__.py
 pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py
+pymoises/dto/input/customer/createLead_input_dto.py
 pymoises/dto/input/transaction/__init__.py
 pymoises/dto/input/transaction/create_transaction_input_dto.py
 pymoises/dto/output/__init__.py
 pymoises/dto/output/customer/__init__.py
+pymoises/dto/output/customer/createLead_output_dto.py
 pymoises/dto/output/customer/customer_output_dto.py
 pymoises/dto/output/customer/moveLead_output_dto.py
 pymoises/dto/output/transaction/__init__.py
 pymoises/dto/output/transaction/transaction_output_dto.py
```

