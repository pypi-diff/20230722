# Comparing `tmp/dropchain-sdk-0.1.2.tar.gz` & `tmp/dropchain-sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dropchain-sdk-0.1.2.tar", last modified: Wed May 31 23:28:13 2023, max compression
+gzip compressed data, was "dist/dropchain-sdk-0.2.0.tar", last modified: Sat Jul 22 00:00:00 2023, max compression
```

## Comparing `dropchain-sdk-0.1.2.tar` & `dropchain-sdk-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 crazink    (501) staff       (20)        0 2023-05-31 23:28:13.000000 dropchain-sdk-0.1.2/
--rw-r--r--   0 crazink    (501) staff       (20)      935 2023-05-31 23:28:13.000000 dropchain-sdk-0.1.2/PKG-INFO
--rw-r--r--   0 crazink    (501) staff       (20)     1069 2023-03-03 02:58:53.000000 dropchain-sdk-0.1.2/LICENSE.md
-drwxr-xr-x   0 crazink    (501) staff       (20)        0 2023-05-31 23:28:13.000000 dropchain-sdk-0.1.2/dropchain_sdk/
--rw-r--r--   0 crazink    (501) staff       (20)    25071 2023-05-31 22:44:27.000000 dropchain-sdk-0.1.2/dropchain_sdk/__init__.py
--rw-r--r--   0 crazink    (501) staff       (20)      436 2023-03-04 00:06:46.000000 dropchain-sdk-0.1.2/README.md
--rw-r--r--   0 crazink    (501) staff       (20)      580 2023-05-31 23:27:14.000000 dropchain-sdk-0.1.2/setup.py
-drwxr-xr-x   0 crazink    (501) staff       (20)        0 2023-05-31 23:28:13.000000 dropchain-sdk-0.1.2/dropchain_sdk.egg-info/
--rw-r--r--   0 crazink    (501) staff       (20)      935 2023-05-31 23:28:13.000000 dropchain-sdk-0.1.2/dropchain_sdk.egg-info/PKG-INFO
--rw-r--r--   0 crazink    (501) staff       (20)      239 2023-05-31 23:28:13.000000 dropchain-sdk-0.1.2/dropchain_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 crazink    (501) staff       (20)        9 2023-05-31 23:28:13.000000 dropchain-sdk-0.1.2/dropchain_sdk.egg-info/requires.txt
--rw-r--r--   0 crazink    (501) staff       (20)       14 2023-05-31 23:28:13.000000 dropchain-sdk-0.1.2/dropchain_sdk.egg-info/top_level.txt
--rw-r--r--   0 crazink    (501) staff       (20)        1 2023-05-31 23:28:13.000000 dropchain-sdk-0.1.2/dropchain_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 crazink    (501) staff       (20)       38 2023-05-31 23:28:13.000000 dropchain-sdk-0.1.2/setup.cfg
+drwxr-xr-x   0 crazink    (501) staff       (20)        0 2023-07-22 00:00:00.000000 dropchain-sdk-0.2.0/
+-rw-r--r--   0 crazink    (501) staff       (20)      935 2023-07-22 00:00:00.000000 dropchain-sdk-0.2.0/PKG-INFO
+-rw-r--r--   0 crazink    (501) staff       (20)     1069 2023-03-03 02:58:53.000000 dropchain-sdk-0.2.0/LICENSE.md
+drwxr-xr-x   0 crazink    (501) staff       (20)        0 2023-07-22 00:00:00.000000 dropchain-sdk-0.2.0/dropchain_sdk/
+-rw-r--r--   0 crazink    (501) staff       (20)    24496 2023-07-21 23:55:08.000000 dropchain-sdk-0.2.0/dropchain_sdk/__init__.py
+-rw-r--r--   0 crazink    (501) staff       (20)      436 2023-03-04 00:06:46.000000 dropchain-sdk-0.2.0/README.md
+-rw-r--r--   0 crazink    (501) staff       (20)      580 2023-07-21 22:58:55.000000 dropchain-sdk-0.2.0/setup.py
+drwxr-xr-x   0 crazink    (501) staff       (20)        0 2023-07-22 00:00:00.000000 dropchain-sdk-0.2.0/dropchain_sdk.egg-info/
+-rw-r--r--   0 crazink    (501) staff       (20)      935 2023-07-22 00:00:00.000000 dropchain-sdk-0.2.0/dropchain_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 crazink    (501) staff       (20)      239 2023-07-22 00:00:00.000000 dropchain-sdk-0.2.0/dropchain_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 crazink    (501) staff       (20)        9 2023-07-22 00:00:00.000000 dropchain-sdk-0.2.0/dropchain_sdk.egg-info/requires.txt
+-rw-r--r--   0 crazink    (501) staff       (20)       14 2023-07-22 00:00:00.000000 dropchain-sdk-0.2.0/dropchain_sdk.egg-info/top_level.txt
+-rw-r--r--   0 crazink    (501) staff       (20)        1 2023-07-22 00:00:00.000000 dropchain-sdk-0.2.0/dropchain_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 crazink    (501) staff       (20)       38 2023-07-22 00:00:00.000000 dropchain-sdk-0.2.0/setup.cfg
```

### Comparing `dropchain-sdk-0.1.2/PKG-INFO` & `dropchain-sdk-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dropchain-sdk
-Version: 0.1.2
+Version: 0.2.0
 Summary: Build robust web3 applications seamlessly using Python with existing frameworks.
 Home-page: https://github.com/cRazink/py_dropchain_sdk
 Author: DropChain Inc
 Author-email: carter@dropchain.network
 License: MIT
 Description: # Python DropChain SDK
```

### Comparing `dropchain-sdk-0.1.2/LICENSE.md` & `dropchain-sdk-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dropchain-sdk-0.1.2/dropchain_sdk/__init__.py` & `dropchain-sdk-0.2.0/dropchain_sdk/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import requests
 
 class DropChainSDK:
-    def __init__(self, rapidapi_key, app_id):
-        self.rapidapi_key = rapidapi_key
+    def __init__(self, api_key, app_id):
+        self.api_key = api_key
         self.app_id = app_id
         self.headers = {
             "content-type": "application/json",
-            "X-RapidAPI-Key": rapidapi_key,
-            "X-RapidAPI-Host": "dropchain1.p.rapidapi.com"
+            "X-API-Key": api_key
         }
 
     def asset_mint_testnet(self, created_asset_amount_int, created_asset_decimals, created_asset_name, created_asset_unit_name, created_asset_url, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/asset_mint_testnet"
+        url = "https://api.dropchain.network/v1/asset_mint_testnet"
 
         payload = {
             "app_id": self.app_id,
             "created_asset_amount_int": created_asset_amount_int,
             "created_asset_decimals": created_asset_decimals,
             "created_asset_name": created_asset_name,
             "created_asset_unit_name": created_asset_unit_name,
@@ -27,15 +26,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def asset_mint_dropnet(self, created_asset_amount_int, created_asset_decimals, created_asset_name, created_asset_unit_name, created_asset_url, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/asset_mint_dropnet"
+        url = "https://api.dropchain.network/v1/asset_mint_dropnet"
 
         payload = {
             "app_id": self.app_id,
             "created_asset_amount_int": created_asset_amount_int,
             "created_asset_decimals": created_asset_decimals,
             "created_asset_name": created_asset_name,
             "created_asset_unit_name": created_asset_unit_name,
@@ -47,30 +46,30 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def get_algo_address_from_uid(self, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/get_algo_address_from_uid"
+        url = "https://api.dropchain.network/v1/get_algo_address_from_uid"
 
         payload = {
             "app_id": self.app_id,
             "user1_uid": user1_uid
         }
 
         if session1_token is not None:
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def freeze_asset_testnet(self, asset1_id, receiver1_uid, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/freeze_asset_testnet"
+        url = "https://api.dropchain.network/v1/freeze_asset_testnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_id": asset1_id,
             "receiver1_uid": receiver1_uid,
             "user1_uid": user1_uid
         }
@@ -79,15 +78,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def freeze_asset_dropnet(self, asset1_id, receiver1_uid, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/freeze_asset_dropnet"
+        url = "https://api.dropchain.network/v1/freeze_asset_dropnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_id": asset1_id,
             "receiver1_uid": receiver1_uid,
             "user1_uid": user1_uid
         }
@@ -96,15 +95,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def get_transaction_info_dropnet(self, transaction1_id, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/get_transaction_info_dropnet"
+        url = "https://api.dropchain.network/v1/get_transaction_info_dropnet"
 
         payload = {
             "app_id": self.app_id,
             "transaction1_id": transaction1_id,
             "user1_uid": user1_uid
         }
 
@@ -112,15 +111,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def get_transaction_info_testnet(self, transaction1_id, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/get_transaction_info_testnet"
+        url = "https://api.dropchain.network/v1/get_transaction_info_testnet"
 
         payload = {
             "app_id": self.app_id,
             "transaction1_id": transaction1_id,
             "user1_uid": user1_uid
         }
 
@@ -128,15 +127,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def get_note_from_txid_testnet(self, transaction1_id, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/get_note_from_txid_testnet"
+        url = "https://api.dropchain.network/v1/get_note_from_txid_testnet"
 
         payload = {
             "app_id": self.app_id,
             "transaction1_id": transaction1_id,
             "user1_uid": user1_uid
         }
 
@@ -144,15 +143,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def get_note_from_txid_dropnet(self, transaction1_id, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/get_note_from_txid_dropnet"
+        url = "https://api.dropchain.network/v1/get_note_from_txid_dropnet"
 
         payload = {
             "app_id": self.app_id,
             "transaction1_id": transaction1_id,
             "user1_uid": user1_uid
         }
         
@@ -160,15 +159,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def get_asset_info_testnet(self, asset1_id, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/get_asset_info_testnet"
+        url = "https://api.dropchain.network/v1/get_asset_info_testnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_id": asset1_id,
             "user1_uid": user1_uid
         }
         
@@ -176,15 +175,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def get_asset_info_dropnet(self, asset1_id, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/get_asset_info_dropnet"
+        url = "https://api.dropchain.network/v1/get_asset_info_dropnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_id": asset1_id,
             "user1_uid": user1_uid
         }
 
@@ -193,15 +192,15 @@
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
 
     def send_asset_dropnet(self, asset1_amount_int, asset1_id, receiver1_uid, transaction1_note, session1_token, user1_uid): 
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/send_asset_dropnet"
+        url = "https://api.dropchain.network/v1/send_asset_dropnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_amount_int": asset1_amount_int,
             "asset1_id": asset1_id,
             "receiver1_uid": receiver1_uid,
             "transaction1_note": transaction1_note,
@@ -212,15 +211,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
        
     def send_asset_testnet(self, asset1_amount_int, asset1_id, receiver1_uid, transaction1_note, session1_token, user1_uid): 
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/send_asset_testnet"
+        url = "https://api.dropchain.network/v1/send_asset_testnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_amount_int": asset1_amount_int,
             "asset1_id": asset1_id,
             "receiver1_uid": receiver1_uid,
             "transaction1_note": transaction1_note,
@@ -232,15 +231,15 @@
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
 
     def send_algo_testnet(self, asset1_amount_int, receiver1_uid, transaction1_note, session1_token, user1_uid): 
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/send_algo_testnet"
+        url = "https://api.dropchain.network/v1/send_algo_testnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_amount_int": asset1_amount_int,
             "receiver1_uid": receiver1_uid,
             "transaction1_note": transaction1_note,
             "user1_uid": user1_uid
@@ -250,15 +249,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def send_drop_dropnet(self, asset1_amount_int, receiver1_uid, transaction1_note, session1_token, user1_uid): 
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/send_drop_dropnet"
+        url = "https://api.dropchain.network/v1/send_drop_dropnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_amount_int": asset1_amount_int,
             "receiver1_uid": receiver1_uid,
             "transaction1_note": transaction1_note,
             "user1_uid": user1_uid
@@ -268,15 +267,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def atomic_swap_algo_testnet(self, asset1_amount_int, asset2_amount_int, receiver1_uid, receiver2_uid, transaction1_note, transaction2_note, session1_token, session2_token, user1_uid, user2_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/atomic_swap_algo_testnet"
+        url = "https://api.dropchain.network/v1/atomic_swap_algo_testnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_amount_int": asset1_amount_int,
             "asset2_amount_int": asset2_amount_int,
             "receiver1_uid": receiver1_uid,
             "receiver2_uid": receiver2_uid,
@@ -293,15 +292,15 @@
             payload["session2_token"] = session2_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def atomic_swap_drop_dropnet(self, asset1_amount_int, asset2_amount_int, receiver1_uid, receiver2_uid, transaction1_note, transaction2_note, session1_token, session2_token, user1_uid, user2_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/atomic_swap_drop_dropnet"
+        url = "https://api.dropchain.network/v1/atomic_swap_drop_dropnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_amount_int": asset1_amount_int,
             "asset2_amount_int": asset2_amount_int,
             "receiver1_uid": receiver1_uid,
             "receiver2_uid": receiver2_uid,
@@ -318,15 +317,15 @@
             payload["session2_token"] = session2_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def get_metadata_from_hash(self, asset_metadata_hash, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/get_metadata_from_hash"
+        url = "https://api.dropchain.network/v1/get_metadata_from_hash"
 
         payload = {
             "app_id": self.app_id,
             "asset_metadata_hash": asset_metadata_hash,
             "user1_uid": user1_uid
         }
 
@@ -334,30 +333,30 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def asset_indexer_testnet(self, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/asset_indexer_testnet"
+        url = "https://api.dropchain.network/v1/asset_indexer_testnet"
 
         payload = {
             "app_id": self.app_id,
             "user1_uid": user1_uid
         }
 
         if session1_token is not None:
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def asset_indexer_lookup_testnet(self, receiver1_uid, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/asset_indexer_lookup_testnet"
+        url = "https://api.dropchain.network/v1/asset_indexer_lookup_testnet"
 
         payload = {
             "app_id": self.app_id,
             "user1_uid": user1_uid,
             "receiver1_uid": receiver1_uid
         }
 
@@ -365,30 +364,30 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def asset_indexer_dropnet(self, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/asset_indexer_dropnet"
+        url = "https://api.dropchain.network/v1/asset_indexer_dropnet"
 
         payload = {
             "app_id": self.app_id,
             "user1_uid": user1_uid
         }
 
         if session1_token is not None:
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def asset_indexer_lookup_dropnet(self, receiver1_uid, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/asset_indexer_lookup_dropnet"
+        url = "https://api.dropchain.network/v1/asset_indexer_lookup_dropnet"
 
         payload = {
             "app_id": self.app_id,
             "user1_uid": user1_uid,
             "receiver1_uid": receiver1_uid
         }
 
@@ -396,15 +395,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def atomic_swap_testnet(self, asset1_amount_int, asset1_id, asset2_amount_int, asset2_id, receiver1_uid, receiver2_uid, transaction1_note, transaction2_note, session1_token, session2_token, user1_uid, user2_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/atomic_swap_testnet"
+        url = "https://api.dropchain.network/v1/atomic_swap_testnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_amount_int": asset1_amount_int,
             "asset1_id": asset1_id,
             "asset2_amount_int": asset2_amount_int,
             "asset2_id": asset2_id,
@@ -423,15 +422,15 @@
             payload["session2_token"] = session2_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def atomic_swap_dropnet(self, asset1_amount_int, asset1_id, asset2_amount_int, asset2_id, receiver1_uid, receiver2_uid, transaction1_note, transaction2_note, session1_token, session2_token, user1_uid, user2_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/atomic_swap_dropnet"
+        url = "https://api.dropchain.network/v1/atomic_swap_dropnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_amount_int": asset1_amount_int,
             "asset1_id": asset1_id,
             "asset2_amount_int": asset2_amount_int,
             "asset2_id": asset2_id,
@@ -450,15 +449,15 @@
             payload["session2_token"] = session2_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def asset_optin_dropnet(self, asset1_id, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/asset_optin_dropnet"
+        url = "https://api.dropchain.network/v1/asset_optin_dropnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_id": asset1_id,
             "user1_uid": user1_uid
         }
 
@@ -466,15 +465,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def asset_optin_testnet(self, asset1_id, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/asset_optin_testnet"
+        url = "https://api.dropchain.network/v1/asset_optin_testnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_id": asset1_id,
             "user1_uid": user1_uid
         }
 
@@ -482,27 +481,27 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def redeem_session_token(self, session1_token):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/redeem_session_token"
+        url = "https://api.dropchain.network/v1/redeem_session_token"
 
         payload = {
             "app_id": self.app_id,
             "session1_token": session1_token
         }
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def create_asset_metadata(self, asset_metadata_description, asset_metadata_external_url, asset_metadata_has_traits, asset_metadata_image_url, asset_metadata_name, asset_metadata_trait_type1, asset_metadata_trait_type2, asset_metadata_trait_type3, asset_metadata_trait_type4, asset_metadata_trait_type5, asset_metadata_trait_type6,asset_metadata_trait_type7, asset_metadata_trait_type8, asset_metadata_value1, asset_metadata_value2, asset_metadata_value3, asset_metadata_value4, asset_metadata_value5, asset_metadata_value6, asset_metadata_value7, asset_metadata_value8, user1_uid, session1_token):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/create_asset_metadata"
+        url = "https://api.dropchain.network/v1/create_asset_metadata"
 
         payload = {
             "app_id": self.app_id,
             "asset_metadata_description": asset_metadata_description,
             "asset_metadata_external_url": asset_metadata_external_url,
             "asset_metadata_has_traits": asset_metadata_has_traits,
             "asset_metadata_image_url": asset_metadata_image_url,
@@ -530,15 +529,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def unfreeze_asset_testnet(self, asset1_id, receiver1_uid, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/unfreeze_asset_testnet"
+        url = "https://api.dropchain.network/v1/unfreeze_asset_testnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_id": asset1_id,
             "receiver1_uid": receiver1_uid,
             "user1_uid": user1_uid
         }
@@ -547,15 +546,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def unfreeze_asset_dropnet(self, asset1_id, receiver1_uid, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/unfreeze_asset_dropnet"
+        url = "https://api.dropchain.network/v1/unfreeze_asset_dropnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_id": asset1_id,
             "receiver1_uid": receiver1_uid,
             "user1_uid": user1_uid
         }
@@ -564,15 +563,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def clawback_asset_testnet(self, asset1_amount_int, asset1_id, receiver1_uid, transaction1_note, session1_token, clawback_uid, user1_uid): 
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/clawback_asset_testnet"
+        url = "https://api.dropchain.network/v1/clawback_asset_testnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_amount_int": asset1_amount_int,
             "asset1_id": asset1_id,
             "receiver1_uid": receiver1_uid,
             "transaction1_note": transaction1_note,
@@ -584,15 +583,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def clawback_asset_dropnet(self, asset1_amount_int, asset1_id, receiver1_uid, transaction1_note, session1_token, clawback_uid, user1_uid): 
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/clawback_asset_dropnet"
+        url = "https://api.dropchain.network/v1/clawback_asset_dropnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_amount_int": asset1_amount_int,
             "asset1_id": asset1_id,
             "receiver1_uid": receiver1_uid,
             "transaction1_note": transaction1_note,
@@ -604,15 +603,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def create_listing(self, product_title, product_description, product_media_url, product_usd_price, sold_asset_ids, quantity_to_send_after_purchase, session1_token, fulfillment_uid, user1_uid): 
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/create_listing"
+        url = "https://api.dropchain.network/v1/create_listing"
 
         payload = {
             "app_id": self.app_id,
             "user1_uid":user1_uid,
             "product_title":product_title,
             "product_description":product_description,
             "product_media_url":product_media_url,
@@ -626,15 +625,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def update_asset_metadata_dropnet(self, asset1_id, metadata_hash, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/update_asset_metadata_dropnet"
+        url = "https://api.dropchain.network/v1/update_asset_metadata_dropnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_id": asset1_id,
             "user1_uid": user1_uid,
             "metadata_hash": metadata_hash
         }
@@ -643,15 +642,15 @@
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def update_asset_metadata_testnet(self, asset1_id, metadata_hash, session1_token, user1_uid):
-        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/update_asset_metadata_testnet"
+        url = "https://api.dropchain.network/v1/update_asset_metadata_testnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_id": asset1_id,
             "user1_uid": user1_uid,
             "metadata_hash": metadata_hash
         }
```

### Comparing `dropchain-sdk-0.1.2/setup.py` & `dropchain-sdk-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
   
 with open("README.md", "r") as fh:
     description = fh.read()
   
 setuptools.setup(
     name="dropchain-sdk",
-    version="0.1.2",
+    version="0.2.0",
     author="DropChain Inc",
     author_email="carter@dropchain.network",
     packages=["dropchain_sdk"],
     description="Build robust web3 applications seamlessly using Python with existing frameworks.",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/cRazink/py_dropchain_sdk",
```

### Comparing `dropchain-sdk-0.1.2/dropchain_sdk.egg-info/PKG-INFO` & `dropchain-sdk-0.2.0/dropchain_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dropchain-sdk
-Version: 0.1.2
+Version: 0.2.0
 Summary: Build robust web3 applications seamlessly using Python with existing frameworks.
 Home-page: https://github.com/cRazink/py_dropchain_sdk
 Author: DropChain Inc
 Author-email: carter@dropchain.network
 License: MIT
 Description: # Python DropChain SDK
```

