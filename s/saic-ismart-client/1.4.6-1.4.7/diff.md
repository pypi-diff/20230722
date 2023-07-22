# Comparing `tmp/saic_ismart_client-1.4.6.tar.gz` & `tmp/saic_ismart_client-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saic_ismart_client-1.4.6.tar", last modified: Fri Jul 21 15:29:59 2023, max compression
+gzip compressed data, was "saic_ismart_client-1.4.7.tar", last modified: Sat Jul 22 12:28:47 2023, max compression
```

## Comparing `saic_ismart_client-1.4.6.tar` & `saic_ismart_client-1.4.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.854666 saic_ismart_client-1.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-21 15:29:59.854666 saic_ismart_client-1.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:29:59.854666 saic_ismart_client-1.4.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.846666 saic_ismart_client-1.4.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.850666 saic_ismart_client-1.4.6/src/saic_ismart_client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.846666 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.850666 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.850666 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.850666 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24328 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/common_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/message_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.850666 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v1_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v1_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v1_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.850666 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v2_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v2_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v2_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.850666 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v3_0/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v3_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23497 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v3_0/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    44396 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/src/saic_ismart_client/saic_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.850666 saic_ismart_client-1.4.6/src/saic_ismart_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-21 15:29:59.000000 saic_ismart_client-1.4.6/src/saic_ismart_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-21 15:29:59.000000 saic_ismart_client-1.4.6/src/saic_ismart_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:29:59.000000 saic_ismart_client-1.4.6/src/saic_ismart_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-21 15:29:59.000000 saic_ismart_client-1.4.6/src/saic_ismart_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 15:29:59.000000 saic_ismart_client-1.4.6/src/saic_ismart_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:29:59.854666 saic_ismart_client-1.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/tests/test_Message_v1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/tests/test_Message_v2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/tests/test_Message_v3_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/tests/test_abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-07-21 15:29:50.000000 saic_ismart_client-1.4.6/tests/test_saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:28:47.674455 saic_ismart_client-1.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-22 12:28:47.674455 saic_ismart_client-1.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 12:28:47.674455 saic_ismart_client-1.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:28:47.666455 saic_ismart_client-1.4.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:28:47.670455 saic_ismart_client-1.4.7/src/saic_ismart_client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:28:47.666455 saic_ismart_client-1.4.7/src/saic_ismart_client/ASN.1_schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:28:47.670455 saic_ismart_client-1.4.7/src/saic_ismart_client/ASN.1_schema/v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:28:47.670455 saic_ismart_client-1.4.7/src/saic_ismart_client/ASN.1_schema/v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:28:47.670455 saic_ismart_client-1.4.7/src/saic_ismart_client/ASN.1_schema/v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24328 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/common_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/message_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:28:47.670455 saic_ismart_client-1.4.7/src/saic_ismart_client/ota_v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/ota_v1_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/ota_v1_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/ota_v1_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:28:47.670455 saic_ismart_client-1.4.7/src/saic_ismart_client/ota_v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/ota_v2_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/ota_v2_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/ota_v2_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:28:47.670455 saic_ismart_client-1.4.7/src/saic_ismart_client/ota_v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/ota_v3_0/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/ota_v3_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23497 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/ota_v3_0/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44453 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/src/saic_ismart_client/saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:28:47.670455 saic_ismart_client-1.4.7/src/saic_ismart_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-22 12:28:47.000000 saic_ismart_client-1.4.7/src/saic_ismart_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-22 12:28:47.000000 saic_ismart_client-1.4.7/src/saic_ismart_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 12:28:47.000000 saic_ismart_client-1.4.7/src/saic_ismart_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-22 12:28:47.000000 saic_ismart_client-1.4.7/src/saic_ismart_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-22 12:28:47.000000 saic_ismart_client-1.4.7/src/saic_ismart_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:28:47.670455 saic_ismart_client-1.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/tests/test_Message_v1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/tests/test_Message_v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/tests/test_Message_v3_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/tests/test_abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-07-22 12:28:35.000000 saic_ismart_client-1.4.7/tests/test_saic_api.py
```

### Comparing `saic_ismart_client-1.4.6/LICENSE` & `saic_ismart_client-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/PKG-INFO` & `saic_ismart_client-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic_ismart_client
-Version: 1.4.6
+Version: 1.4.7
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.4.6/README.md` & `saic_ismart_client-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/pyproject.toml` & `saic_ismart_client-1.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saic_ismart_client"
-version = "1.4.6"
+version = "1.4.7"
 authors = [
     { name = "Thomas Salm", email="saic-python-client@devtom.de"},
 ]
 dependencies = [
     "asn1tools >= 0.166.0",
     "requests >= 2.31.0",
     "urllib3 >= 2.0.3",
```

### Comparing `saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1` & `saic_ismart_client-1.4.7/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.7/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1` & `saic_ismart_client-1.4.7/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.7/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1` & `saic_ismart_client-1.4.7/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.7/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/src/saic_ismart_client/abrp_api.py` & `saic_ismart_client-1.4.7/src/saic_ismart_client/abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/src/saic_ismart_client/common_model.py` & `saic_ismart_client-1.4.7/src/saic_ismart_client/common_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/src/saic_ismart_client/message_decoder.py` & `saic_ismart_client-1.4.7/src/saic_ismart_client/message_decoder.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v1_1/Message.py` & `saic_ismart_client-1.4.7/src/saic_ismart_client/ota_v1_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v1_1/data_model.py` & `saic_ismart_client-1.4.7/src/saic_ismart_client/ota_v1_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v2_1/Message.py` & `saic_ismart_client-1.4.7/src/saic_ismart_client/ota_v2_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v2_1/data_model.py` & `saic_ismart_client-1.4.7/src/saic_ismart_client/ota_v2_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v3_0/Message.py` & `saic_ismart_client-1.4.7/src/saic_ismart_client/ota_v3_0/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/src/saic_ismart_client/ota_v3_0/data_model.py` & `saic_ismart_client-1.4.7/src/saic_ismart_client/ota_v3_0/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/src/saic_ismart_client/saic_api.py` & `saic_ismart_client-1.4.7/src/saic_ismart_client/saic_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,14 +171,15 @@
         vehicle_status_req = OtaRvmVehicleStatusReq()
         vehicle_status_req.veh_status_req_type = 2
         vehicle_status_req_msg = MessageV2(MessageBodyV2(), vehicle_status_req)
         application_id = '511'
         application_data_protocol_version = 25857
         self.message_V2_1_coder.initialize_message(self.uid, self.get_token(), vin_info.vin, application_id,
                                                    application_data_protocol_version, 1, vehicle_status_req_msg)
+        vehicle_status_req_msg.body.ack_required = False
         if event_id is not None:
             vehicle_status_req_msg.body.event_id = event_id
         self.publish_json_request(application_id, application_data_protocol_version, vehicle_status_req_msg.get_data())
         vehicle_status_req_hex = self.message_V2_1_coder.encode_request(vehicle_status_req_msg)
         self.publish_raw_request(application_id, application_data_protocol_version, vehicle_status_req_hex)
         vehicle_status_rsp_hex = self.send_request(vehicle_status_req_hex,
                                                    urllib.parse.urljoin(self.saic_uri, '/TAP.Web/ota.mpv21'))
```

### Comparing `saic_ismart_client-1.4.6/src/saic_ismart_client.egg-info/PKG-INFO` & `saic_ismart_client-1.4.7/src/saic_ismart_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic-ismart-client
-Version: 1.4.6
+Version: 1.4.7
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.4.6/src/saic_ismart_client.egg-info/SOURCES.txt` & `saic_ismart_client-1.4.7/src/saic_ismart_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/tests/test_Message_v1_1.py` & `saic_ismart_client-1.4.7/tests/test_Message_v1_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/tests/test_Message_v2_1.py` & `saic_ismart_client-1.4.7/tests/test_Message_v2_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/tests/test_Message_v3_0.py` & `saic_ismart_client-1.4.7/tests/test_Message_v3_0.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/tests/test_abrp_api.py` & `saic_ismart_client-1.4.7/tests/test_abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.6/tests/test_saic_api.py` & `saic_ismart_client-1.4.7/tests/test_saic_api.py`

 * *Files identical despite different names*

