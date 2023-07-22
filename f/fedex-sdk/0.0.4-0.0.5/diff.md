# Comparing `tmp/fedex-sdk-0.0.4.tar.gz` & `tmp/fedex-sdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedex-sdk-0.0.4.tar", last modified: Fri Jul 21 14:09:21 2023, max compression
+gzip compressed data, was "fedex-sdk-0.0.5.tar", last modified: Sat Jul 22 09:14:54 2023, max compression
```

## Comparing `fedex-sdk-0.0.4.tar` & `fedex-sdk-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 14:09:21.165813 fedex-sdk-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-07-21 14:09:21.118943 fedex-sdk-0.0.4/FedexSDK/
--rw-rw-rw-   0        0        0     3231 2023-07-21 14:09:04.000000 fedex-sdk-0.0.4/FedexSDK/FedExSDK.py
--rw-rw-rw-   0        0        0       55 2023-07-21 14:09:11.000000 fedex-sdk-0.0.4/FedexSDK/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 14:09:21.134566 fedex-sdk-0.0.4/FedexSDK/models/
--rw-rw-rw-   0        0        0       79 2023-07-20 14:07:03.000000 fedex-sdk-0.0.4/FedexSDK/models/AccountNumber.py
--rw-rw-rw-   0        0        0     1400 2023-07-20 14:15:22.000000 fedex-sdk-0.0.4/FedexSDK/models/Address.py
--rw-rw-rw-   0        0        0     2163 2023-07-20 13:11:54.000000 fedex-sdk-0.0.4/FedexSDK/models/Contact.py
--rw-rw-rw-   0        0        0      297 2023-07-20 14:00:52.000000 fedex-sdk-0.0.4/FedexSDK/models/Recipient.py
--rw-rw-rw-   0        0        0     1345 2023-07-20 14:16:51.000000 fedex-sdk-0.0.4/FedexSDK/models/Request.py
--rw-rw-rw-   0        0        0     6754 2023-07-21 08:19:24.000000 fedex-sdk-0.0.4/FedexSDK/models/RequestedShipment.py
--rw-rw-rw-   0        0        0      263 2023-07-20 13:49:03.000000 fedex-sdk-0.0.4/FedexSDK/models/Shipper.py
--rw-rw-rw-   0        0        0      316 2023-07-20 14:00:05.000000 fedex-sdk-0.0.4/FedexSDK/models/SoldTo.py
--rw-rw-rw-   0        0        0      581 2023-07-20 13:08:42.000000 fedex-sdk-0.0.4/FedexSDK/models/Tin.py
--rw-rw-rw-   0        0        0      300 2023-07-20 13:07:32.000000 fedex-sdk-0.0.4/FedexSDK/models/TotalDeclaredValue.py
--rw-rw-rw-   0        0        0      969 2023-07-21 08:43:43.000000 fedex-sdk-0.0.4/FedexSDK/models/__init__.py
--rw-rw-rw-   0        0        0      326 2023-07-21 14:09:21.150191 fedex-sdk-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 14:09:21.150191 fedex-sdk-0.0.4/fedex_sdk.egg-info/
--rw-rw-rw-   0        0        0      326 2023-07-21 14:09:20.000000 fedex-sdk-0.0.4/fedex_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-21 14:09:21.000000 fedex-sdk-0.0.4/fedex_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 14:09:20.000000 fedex-sdk-0.0.4/fedex_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 14:09:20.000000 fedex-sdk-0.0.4/fedex_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 14:09:21.165813 fedex-sdk-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      559 2023-07-21 08:44:20.000000 fedex-sdk-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:14:54.486441 fedex-sdk-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-07-22 09:14:54.439586 fedex-sdk-0.0.5/FedexSDK/
+-rw-rw-rw-   0        0        0     3984 2023-07-22 09:13:16.000000 fedex-sdk-0.0.5/FedexSDK/FedExSDK.py
+-rw-rw-rw-   0        0        0       55 2023-07-22 09:14:46.000000 fedex-sdk-0.0.5/FedexSDK/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:14:54.455194 fedex-sdk-0.0.5/FedexSDK/models/
+-rw-rw-rw-   0        0        0       79 2023-07-20 14:07:03.000000 fedex-sdk-0.0.5/FedexSDK/models/AccountNumber.py
+-rw-rw-rw-   0        0        0     1400 2023-07-20 14:15:22.000000 fedex-sdk-0.0.5/FedexSDK/models/Address.py
+-rw-rw-rw-   0        0        0     2163 2023-07-20 13:11:54.000000 fedex-sdk-0.0.5/FedexSDK/models/Contact.py
+-rw-rw-rw-   0        0        0      297 2023-07-20 14:00:52.000000 fedex-sdk-0.0.5/FedexSDK/models/Recipient.py
+-rw-rw-rw-   0        0        0     1345 2023-07-20 14:16:51.000000 fedex-sdk-0.0.5/FedexSDK/models/Request.py
+-rw-rw-rw-   0        0        0     6754 2023-07-21 08:19:24.000000 fedex-sdk-0.0.5/FedexSDK/models/RequestedShipment.py
+-rw-rw-rw-   0        0        0      263 2023-07-20 13:49:03.000000 fedex-sdk-0.0.5/FedexSDK/models/Shipper.py
+-rw-rw-rw-   0        0        0      316 2023-07-20 14:00:05.000000 fedex-sdk-0.0.5/FedexSDK/models/SoldTo.py
+-rw-rw-rw-   0        0        0      581 2023-07-20 13:08:42.000000 fedex-sdk-0.0.5/FedexSDK/models/Tin.py
+-rw-rw-rw-   0        0        0      300 2023-07-20 13:07:32.000000 fedex-sdk-0.0.5/FedexSDK/models/TotalDeclaredValue.py
+-rw-rw-rw-   0        0        0      969 2023-07-21 08:43:43.000000 fedex-sdk-0.0.5/FedexSDK/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:14:54.470831 fedex-sdk-0.0.5/FedexSDK/models/tracking/
+-rw-rw-rw-   0        0        0      127 2023-07-22 07:14:07.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/AdditionalTrackingInfo.py
+-rw-rw-rw-   0        0        0      214 2023-07-22 07:04:34.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/Address.py
+-rw-rw-rw-   0        0        0       97 2023-07-22 08:23:17.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/DateAndTime.py
+-rw-rw-rw-   0        0        0      119 2023-07-22 08:29:51.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/DelayDetail.py
+-rw-rw-rw-   0        0        0      308 2023-07-22 08:22:00.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/DeliveryDetails.py
+-rw-rw-rw-   0        0        0      124 2023-07-22 08:21:44.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/DeliveryOptionEligiblityDetail.py
+-rw-rw-rw-   0        0        0      385 2023-07-22 07:04:54.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/Destination.py
+-rw-rw-rw-   0        0        0      294 2023-07-22 08:17:20.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/LatestStatusDetail.py
+-rw-rw-rw-   0        0        0      131 2023-07-22 07:04:47.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/LocationContactAndAddress.py
+-rw-rw-rw-   0        0        0      213 2023-07-22 07:05:30.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/OriginLocation.py
+-rw-rw-rw-   0        0        0      387 2023-07-22 08:28:05.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/PackageDetails.py
+-rw-rw-rw-   0        0        0      183 2023-07-22 08:17:51.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/RecipientInformation.py
+-rw-rw-rw-   0        0        0      481 2023-07-22 06:57:13.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/ScanEvent.py
+-rw-rw-rw-   0        0        0      355 2023-07-22 08:29:12.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/ScanLocation.py
+-rw-rw-rw-   0        0        0      105 2023-07-22 08:22:58.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/ServiceCommitMessage.py
+-rw-rw-rw-   0        0        0      131 2023-07-22 07:02:59.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/ServiceDetail.py
+-rw-rw-rw-   0        0        0      199 2023-07-22 07:01:06.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/ShipmentDetails.py
+-rw-rw-rw-   0        0        0      181 2023-07-22 08:27:55.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/ShipperInformation.py
+-rw-rw-rw-   0        0        0      126 2023-07-22 08:22:37.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/SpecialHandling.py
+-rw-rw-rw-   0        0        0     2130 2023-07-22 08:25:22.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/TrackResult.py
+-rw-rw-rw-   0        0        0      150 2023-07-22 07:13:21.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/TrackingNumberInfo.py
+-rw-rw-rw-   0        0        0      319 2023-07-22 07:00:07.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/WeightAndDimensions.py
+-rw-rw-rw-   0        0        0      251 2023-07-22 07:02:26.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/Window.py
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:48:10.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/__init__.py
+-rw-rw-rw-   0        0        0      326 2023-07-22 09:14:54.486441 fedex-sdk-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-22 09:14:54.486441 fedex-sdk-0.0.5/fedex_sdk.egg-info/
+-rw-rw-rw-   0        0        0      326 2023-07-22 09:14:54.000000 fedex-sdk-0.0.5/fedex_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1562 2023-07-22 09:14:54.000000 fedex-sdk-0.0.5/fedex_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 09:14:54.000000 fedex-sdk-0.0.5/fedex_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-22 09:14:54.000000 fedex-sdk-0.0.5/fedex_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-22 09:14:54.486441 fedex-sdk-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      559 2023-07-21 08:44:20.000000 fedex-sdk-0.0.5/setup.py
```

### Comparing `fedex-sdk-0.0.4/FedexSDK/FedExSDK.py` & `fedex-sdk-0.0.5/FedexSDK/FedExSDK.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import json
 import os
 from dataclasses import dataclass
 from requests_oauthlib import OAuth2Session
 import requests
 from FedexSDK.models import Request
 
+from FedexSDK.models.tracking.TrackResult import TrackResponse
+
 @dataclass
 class APIType:
     Production: str = "Production"
     Test: str = "Test"
 
 @dataclass
 class ImageType:
@@ -23,29 +25,46 @@
             raise Exception("Please Requests Session")
         
         self.session = session
         self.headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {session.access_token}"
         }
+        
+        self.api_url = "https://apis.fedex.com/track/v1"
 
     def create_shipment(self, request: Request, output_json_path: str):
-        url = "https://apis.fedex.com/ship/v1/shipments"
-
-        res = self.session.post(url, json=request.dict(), headers=self.headers)
+        res = self.session.post(f"{self.api_url}/shipments", json=request.dict(), headers=self.headers)
         
         now_date = datetime.datetime.now()
         with open(f"{now_date.strftime('%d_%m_%Y_tracking_numbers.txt')}", "a") as f:
             f.write(
                 f"{res.json()['output']['transactionShipments'][0]['shipmentDocuments'][0]['trackingNumber']}:{request.requestedShipment.recipients[0].contact.personName}\n"
             )
         
         json.dump(res.json(), open(output_json_path, "w", encoding="utf-8"), ensure_ascii=False)
 
     
+    def track_shipment_by_tracking_number(self, tracking_number: str, ship_date_begin: str, ship_date_end: str):
+        
+        data = {
+            "includeDetailedScans": True,
+            "trackingInfo": [
+                {
+                    "trackingNumberInfo": {
+                    "trackingNumber": tracking_number,
+                    },
+                    "shipDateBegin": ship_date_begin,
+                    "shipDateEnd": ship_date_end
+                }
+            ]
+        }
+        res = self.session.post(f"{self.api_url}/trackingnumbers", json=data, headers=self.headers)
+        return TrackResponse(**res.json())
+    
     def add_image(self, reference_id: str, image_name: str, image_index: str, image_type: ImageType, image_path: str):
         name, ext = os.path.splitext(image_path)
         data = {
             "document": {
                 "referenceId": reference_id,
                 "name": image_name,
                 "contentType": f"image/{ext}",
@@ -83,10 +102,8 @@
         data = {
             "grant_type": "client_credentials",
             "client_id": client_id,
             "client_secret": client_secret
         }
 
         response = requests.request("POST", url, data=data, headers=headers)
-        return OAuth2Session(client_id=client_id, token=response.json())
-
-
+        return OAuth2Session(client_id=client_id, token=response.json())
```

### Comparing `fedex-sdk-0.0.4/FedexSDK/models/Address.py` & `fedex-sdk-0.0.5/FedexSDK/models/Address.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.4/FedexSDK/models/Contact.py` & `fedex-sdk-0.0.5/FedexSDK/models/Contact.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.4/FedexSDK/models/Request.py` & `fedex-sdk-0.0.5/FedexSDK/models/Request.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.4/FedexSDK/models/RequestedShipment.py` & `fedex-sdk-0.0.5/FedexSDK/models/RequestedShipment.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.4/FedexSDK/models/Tin.py` & `fedex-sdk-0.0.5/FedexSDK/models/Tin.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.4/FedexSDK/models/__init__.py` & `fedex-sdk-0.0.5/FedexSDK/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.4/setup.py` & `fedex-sdk-0.0.5/setup.py`

 * *Files identical despite different names*

