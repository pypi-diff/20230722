# Comparing `tmp/fedex-sdk-0.0.5.tar.gz` & `tmp/fedex-sdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedex-sdk-0.0.5.tar", last modified: Sat Jul 22 09:14:54 2023, max compression
+gzip compressed data, was "fedex-sdk-0.0.6.tar", last modified: Sat Jul 22 09:26:42 2023, max compression
```

## Comparing `fedex-sdk-0.0.5.tar` & `fedex-sdk-0.0.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 09:14:54.486441 fedex-sdk-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-07-22 09:14:54.439586 fedex-sdk-0.0.5/FedexSDK/
--rw-rw-rw-   0        0        0     3984 2023-07-22 09:13:16.000000 fedex-sdk-0.0.5/FedexSDK/FedExSDK.py
--rw-rw-rw-   0        0        0       55 2023-07-22 09:14:46.000000 fedex-sdk-0.0.5/FedexSDK/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:14:54.455194 fedex-sdk-0.0.5/FedexSDK/models/
--rw-rw-rw-   0        0        0       79 2023-07-20 14:07:03.000000 fedex-sdk-0.0.5/FedexSDK/models/AccountNumber.py
--rw-rw-rw-   0        0        0     1400 2023-07-20 14:15:22.000000 fedex-sdk-0.0.5/FedexSDK/models/Address.py
--rw-rw-rw-   0        0        0     2163 2023-07-20 13:11:54.000000 fedex-sdk-0.0.5/FedexSDK/models/Contact.py
--rw-rw-rw-   0        0        0      297 2023-07-20 14:00:52.000000 fedex-sdk-0.0.5/FedexSDK/models/Recipient.py
--rw-rw-rw-   0        0        0     1345 2023-07-20 14:16:51.000000 fedex-sdk-0.0.5/FedexSDK/models/Request.py
--rw-rw-rw-   0        0        0     6754 2023-07-21 08:19:24.000000 fedex-sdk-0.0.5/FedexSDK/models/RequestedShipment.py
--rw-rw-rw-   0        0        0      263 2023-07-20 13:49:03.000000 fedex-sdk-0.0.5/FedexSDK/models/Shipper.py
--rw-rw-rw-   0        0        0      316 2023-07-20 14:00:05.000000 fedex-sdk-0.0.5/FedexSDK/models/SoldTo.py
--rw-rw-rw-   0        0        0      581 2023-07-20 13:08:42.000000 fedex-sdk-0.0.5/FedexSDK/models/Tin.py
--rw-rw-rw-   0        0        0      300 2023-07-20 13:07:32.000000 fedex-sdk-0.0.5/FedexSDK/models/TotalDeclaredValue.py
--rw-rw-rw-   0        0        0      969 2023-07-21 08:43:43.000000 fedex-sdk-0.0.5/FedexSDK/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:14:54.470831 fedex-sdk-0.0.5/FedexSDK/models/tracking/
--rw-rw-rw-   0        0        0      127 2023-07-22 07:14:07.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/AdditionalTrackingInfo.py
--rw-rw-rw-   0        0        0      214 2023-07-22 07:04:34.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/Address.py
--rw-rw-rw-   0        0        0       97 2023-07-22 08:23:17.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/DateAndTime.py
--rw-rw-rw-   0        0        0      119 2023-07-22 08:29:51.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/DelayDetail.py
--rw-rw-rw-   0        0        0      308 2023-07-22 08:22:00.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/DeliveryDetails.py
--rw-rw-rw-   0        0        0      124 2023-07-22 08:21:44.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/DeliveryOptionEligiblityDetail.py
--rw-rw-rw-   0        0        0      385 2023-07-22 07:04:54.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/Destination.py
--rw-rw-rw-   0        0        0      294 2023-07-22 08:17:20.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/LatestStatusDetail.py
--rw-rw-rw-   0        0        0      131 2023-07-22 07:04:47.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/LocationContactAndAddress.py
--rw-rw-rw-   0        0        0      213 2023-07-22 07:05:30.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/OriginLocation.py
--rw-rw-rw-   0        0        0      387 2023-07-22 08:28:05.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/PackageDetails.py
--rw-rw-rw-   0        0        0      183 2023-07-22 08:17:51.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/RecipientInformation.py
--rw-rw-rw-   0        0        0      481 2023-07-22 06:57:13.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/ScanEvent.py
--rw-rw-rw-   0        0        0      355 2023-07-22 08:29:12.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/ScanLocation.py
--rw-rw-rw-   0        0        0      105 2023-07-22 08:22:58.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/ServiceCommitMessage.py
--rw-rw-rw-   0        0        0      131 2023-07-22 07:02:59.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/ServiceDetail.py
--rw-rw-rw-   0        0        0      199 2023-07-22 07:01:06.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/ShipmentDetails.py
--rw-rw-rw-   0        0        0      181 2023-07-22 08:27:55.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/ShipperInformation.py
--rw-rw-rw-   0        0        0      126 2023-07-22 08:22:37.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/SpecialHandling.py
--rw-rw-rw-   0        0        0     2130 2023-07-22 08:25:22.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/TrackResult.py
--rw-rw-rw-   0        0        0      150 2023-07-22 07:13:21.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/TrackingNumberInfo.py
--rw-rw-rw-   0        0        0      319 2023-07-22 07:00:07.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/WeightAndDimensions.py
--rw-rw-rw-   0        0        0      251 2023-07-22 07:02:26.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/Window.py
--rw-rw-rw-   0        0        0        0 2023-07-22 06:48:10.000000 fedex-sdk-0.0.5/FedexSDK/models/tracking/__init__.py
--rw-rw-rw-   0        0        0      326 2023-07-22 09:14:54.486441 fedex-sdk-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-22 09:14:54.486441 fedex-sdk-0.0.5/fedex_sdk.egg-info/
--rw-rw-rw-   0        0        0      326 2023-07-22 09:14:54.000000 fedex-sdk-0.0.5/fedex_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1562 2023-07-22 09:14:54.000000 fedex-sdk-0.0.5/fedex_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 09:14:54.000000 fedex-sdk-0.0.5/fedex_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-22 09:14:54.000000 fedex-sdk-0.0.5/fedex_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-22 09:14:54.486441 fedex-sdk-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      559 2023-07-21 08:44:20.000000 fedex-sdk-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:26:42.851204 fedex-sdk-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-07-22 09:26:42.774203 fedex-sdk-0.0.6/FedexSDK/
+-rw-rw-rw-   0        0        0     3984 2023-07-22 09:13:16.000000 fedex-sdk-0.0.6/FedexSDK/FedExSDK.py
+-rw-rw-rw-   0        0        0       66 2023-07-22 09:26:34.000000 fedex-sdk-0.0.6/FedexSDK/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:26:42.789202 fedex-sdk-0.0.6/FedexSDK/models/
+-rw-rw-rw-   0        0        0       79 2023-07-20 14:07:03.000000 fedex-sdk-0.0.6/FedexSDK/models/AccountNumber.py
+-rw-rw-rw-   0        0        0     1400 2023-07-20 14:15:22.000000 fedex-sdk-0.0.6/FedexSDK/models/Address.py
+-rw-rw-rw-   0        0        0     2163 2023-07-20 13:11:54.000000 fedex-sdk-0.0.6/FedexSDK/models/Contact.py
+-rw-rw-rw-   0        0        0      297 2023-07-20 14:00:52.000000 fedex-sdk-0.0.6/FedexSDK/models/Recipient.py
+-rw-rw-rw-   0        0        0     1345 2023-07-20 14:16:51.000000 fedex-sdk-0.0.6/FedexSDK/models/Request.py
+-rw-rw-rw-   0        0        0     6754 2023-07-21 08:19:24.000000 fedex-sdk-0.0.6/FedexSDK/models/RequestedShipment.py
+-rw-rw-rw-   0        0        0      263 2023-07-20 13:49:03.000000 fedex-sdk-0.0.6/FedexSDK/models/Shipper.py
+-rw-rw-rw-   0        0        0      316 2023-07-20 14:00:05.000000 fedex-sdk-0.0.6/FedexSDK/models/SoldTo.py
+-rw-rw-rw-   0        0        0      581 2023-07-20 13:08:42.000000 fedex-sdk-0.0.6/FedexSDK/models/Tin.py
+-rw-rw-rw-   0        0        0      300 2023-07-20 13:07:32.000000 fedex-sdk-0.0.6/FedexSDK/models/TotalDeclaredValue.py
+-rw-rw-rw-   0        0        0      969 2023-07-21 08:43:43.000000 fedex-sdk-0.0.6/FedexSDK/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:26:42.824203 fedex-sdk-0.0.6/FedexSDK/models/tracking/
+-rw-rw-rw-   0        0        0      127 2023-07-22 07:14:07.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/AdditionalTrackingInfo.py
+-rw-rw-rw-   0        0        0      214 2023-07-22 07:04:34.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/Address.py
+-rw-rw-rw-   0        0        0       97 2023-07-22 08:23:17.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/DateAndTime.py
+-rw-rw-rw-   0        0        0      119 2023-07-22 08:29:51.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/DelayDetail.py
+-rw-rw-rw-   0        0        0      328 2023-07-22 09:24:39.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/DeliveryDetails.py
+-rw-rw-rw-   0        0        0      124 2023-07-22 08:21:44.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/DeliveryOptionEligiblityDetail.py
+-rw-rw-rw-   0        0        0      385 2023-07-22 07:04:54.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/Destination.py
+-rw-rw-rw-   0        0        0      333 2023-07-22 09:23:39.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/LatestStatusDetail.py
+-rw-rw-rw-   0        0        0      131 2023-07-22 07:04:47.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/LocationContactAndAddress.py
+-rw-rw-rw-   0        0        0      213 2023-07-22 07:05:30.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/OriginLocation.py
+-rw-rw-rw-   0        0        0      387 2023-07-22 08:28:05.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/PackageDetails.py
+-rw-rw-rw-   0        0        0      183 2023-07-22 08:17:51.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/RecipientInformation.py
+-rw-rw-rw-   0        0        0      481 2023-07-22 06:57:13.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/ScanEvent.py
+-rw-rw-rw-   0        0        0      355 2023-07-22 08:29:12.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/ScanLocation.py
+-rw-rw-rw-   0        0        0      105 2023-07-22 08:22:58.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/ServiceCommitMessage.py
+-rw-rw-rw-   0        0        0      131 2023-07-22 07:02:59.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/ServiceDetail.py
+-rw-rw-rw-   0        0        0      199 2023-07-22 07:01:06.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/ShipmentDetails.py
+-rw-rw-rw-   0        0        0      181 2023-07-22 08:27:55.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/ShipperInformation.py
+-rw-rw-rw-   0        0        0      126 2023-07-22 08:22:37.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/SpecialHandling.py
+-rw-rw-rw-   0        0        0     2150 2023-07-22 09:25:14.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/TrackResult.py
+-rw-rw-rw-   0        0        0      150 2023-07-22 07:13:21.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/TrackingNumberInfo.py
+-rw-rw-rw-   0        0        0      319 2023-07-22 07:00:07.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/WeightAndDimensions.py
+-rw-rw-rw-   0        0        0      251 2023-07-22 07:02:26.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/Window.py
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:48:10.000000 fedex-sdk-0.0.6/FedexSDK/models/tracking/__init__.py
+-rw-rw-rw-   0        0        0      326 2023-07-22 09:26:42.850203 fedex-sdk-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-22 09:26:42.849286 fedex-sdk-0.0.6/fedex_sdk.egg-info/
+-rw-rw-rw-   0        0        0      326 2023-07-22 09:26:42.000000 fedex-sdk-0.0.6/fedex_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1562 2023-07-22 09:26:42.000000 fedex-sdk-0.0.6/fedex_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 09:26:42.000000 fedex-sdk-0.0.6/fedex_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-22 09:26:42.000000 fedex-sdk-0.0.6/fedex_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-22 09:26:42.852203 fedex-sdk-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      559 2023-07-21 08:44:20.000000 fedex-sdk-0.0.6/setup.py
```

### Comparing `fedex-sdk-0.0.5/FedexSDK/FedExSDK.py` & `fedex-sdk-0.0.6/FedexSDK/FedExSDK.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.5/FedexSDK/models/Address.py` & `fedex-sdk-0.0.6/FedexSDK/models/Address.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.5/FedexSDK/models/Contact.py` & `fedex-sdk-0.0.6/FedexSDK/models/Contact.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.5/FedexSDK/models/Request.py` & `fedex-sdk-0.0.6/FedexSDK/models/Request.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.5/FedexSDK/models/RequestedShipment.py` & `fedex-sdk-0.0.6/FedexSDK/models/RequestedShipment.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.5/FedexSDK/models/Tin.py` & `fedex-sdk-0.0.6/FedexSDK/models/Tin.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.5/FedexSDK/models/__init__.py` & `fedex-sdk-0.0.6/FedexSDK/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.5/FedexSDK/models/tracking/TrackResult.py` & `fedex-sdk-0.0.6/FedexSDK/models/tracking/TrackResult.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict, Any
+from typing import List, Dict, Any, Optional
 from pydantic import BaseModel
 from .ServiceCommitMessage import ServiceCommitMessage
 from .Destination import DestinationLocation, LastUpdatedDestinationAddress
 from .OriginLocation import OriginLocation
 from .DeliveryDetails import DeliveryDetails
 from .SpecialHandling import SpecialHandling
 from .DateAndTime import DateAndTime
@@ -30,15 +30,15 @@
     shipmentDetails: ShipmentDetails
     scanEvents: List[ScanEvent]
     availableNotifications: List[str]
     deliveryDetails: DeliveryDetails
     originLocation: OriginLocation
     destinationLocation: DestinationLocation
     lastUpdatedDestinationAddress: LastUpdatedDestinationAddress
-    serviceCommitMessage: ServiceCommitMessage
+    serviceCommitMessage: Optional[ServiceCommitMessage]
     serviceDetail: ServiceDetail
     standardTransitTimeWindow: StandardTransitTimeWindow
     estimatedDeliveryTimeWindow: EstimatedDeliveryTimeWindow
     goodsClassificationCode: str
     returnDetail: Dict[str, Any]
 
 class CompleteTrackResult(BaseModel):
```

### Comparing `fedex-sdk-0.0.5/fedex_sdk.egg-info/SOURCES.txt` & `fedex-sdk-0.0.6/fedex_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fedex-sdk-0.0.5/setup.py` & `fedex-sdk-0.0.6/setup.py`

 * *Files identical despite different names*

