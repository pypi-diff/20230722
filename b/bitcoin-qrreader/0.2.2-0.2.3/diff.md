# Comparing `tmp/bitcoin_qrreader-0.2.2.tar.gz` & `tmp/bitcoin_qrreader-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitcoin_qrreader-0.2.2.tar", last modified: Fri Jul 21 19:40:57 2023, max compression
+gzip compressed data, was "bitcoin_qrreader-0.2.3.tar", last modified: Sat Jul 22 09:27:39 2023, max compression
```

## Comparing `bitcoin_qrreader-0.2.2.tar` & `bitcoin_qrreader-0.2.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-21 19:40:57.101949 bitcoin_qrreader-0.2.2/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    35149 2023-06-09 17:54:40.000000 bitcoin_qrreader-0.2.2/LICENSE
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2854 2023-07-21 11:50:05.000000 bitcoin_qrreader-0.2.2/LICENSE_UR
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1291 2023-07-21 19:40:57.101949 bitcoin_qrreader-0.2.2/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      784 2023-07-21 17:29:28.000000 bitcoin_qrreader-0.2.2/README.md
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-21 19:40:57.097949 bitcoin_qrreader-0.2.2/bitcoin_qrreader/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2023-07-20 11:25:47.000000 bitcoin_qrreader-0.2.2/bitcoin_qrreader/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    21558 2023-07-21 17:53:15.000000 bitcoin_qrreader-0.2.2/bitcoin_qrreader/bitcoin_qr.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1366 2023-07-21 11:27:49.000000 bitcoin_qrreader-0.2.2/bitcoin_qrreader/bitcoin_qr_gui.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     3849 2023-07-21 19:33:23.000000 bitcoin_qrreader-0.2.2/bitcoin_qrreader/qr_qui.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-21 19:40:57.097949 bitcoin_qrreader-0.2.2/bitcoin_qrreader.egg-info/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1291 2023-07-21 19:40:57.000000 bitcoin_qrreader-0.2.2/bitcoin_qrreader.egg-info/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1001 2023-07-21 19:40:57.000000 bitcoin_qrreader-0.2.2/bitcoin_qrreader.egg-info/SOURCES.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-07-21 19:40:57.000000 bitcoin_qrreader-0.2.2/bitcoin_qrreader.egg-info/dependency_links.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       47 2023-07-21 19:40:57.000000 bitcoin_qrreader-0.2.2/bitcoin_qrreader.egg-info/requires.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       28 2023-07-21 19:40:57.000000 bitcoin_qrreader-0.2.2/bitcoin_qrreader.egg-info/top_level.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2023-07-21 19:40:57.101949 bitcoin_qrreader-0.2.2/setup.cfg
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1075 2023-07-21 19:33:53.000000 bitcoin_qrreader-0.2.2/setup.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-21 19:40:57.097949 bitcoin_qrreader-0.2.2/ur/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2023-07-21 11:50:05.000000 bitcoin_qrreader-0.2.2/ur/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4940 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.2/ur/bytewords.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    11377 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.2/ur/cbor_lite.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      179 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.2/ur/constants.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      729 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.2/ur/crc32.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     9669 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.2/ur/fountain_decoder.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4978 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.2/ur/fountain_encoder.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1603 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.2/ur/fountain_utils.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1568 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.2/ur/random_sampler.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      491 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.2/ur/ur.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     5115 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.2/ur/ur_decoder.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2038 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.2/ur/ur_encoder.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1638 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.2/ur/utils.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4440 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.2/ur/xoshiro256.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-21 19:40:57.097949 bitcoin_qrreader-0.2.2/urtypes/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1157 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.2/urtypes/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1580 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.2/urtypes/bytes.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-21 19:40:57.097949 bitcoin_qrreader-0.2.2/urtypes/cbor/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1247 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.2/urtypes/cbor/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2213 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.2/urtypes/cbor/data.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     6660 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.2/urtypes/cbor/decoder.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4937 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.2/urtypes/cbor/encoder.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-21 19:40:57.101949 bitcoin_qrreader-0.2.2/urtypes/crypto/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1315 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.2/urtypes/crypto/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2370 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.2/urtypes/crypto/account.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1842 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.2/urtypes/crypto/bip39.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1951 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.2/urtypes/crypto/coin_info.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2238 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.2/urtypes/crypto/ec_key.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     9315 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.2/urtypes/crypto/hd_key.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     3747 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.2/urtypes/crypto/keypath.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2467 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.2/urtypes/crypto/multi_key.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     6360 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.2/urtypes/crypto/output.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1293 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.2/urtypes/crypto/psbt.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2288 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.2/urtypes/registry.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-22 09:27:39.837497 bitcoin_qrreader-0.2.3/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    35149 2023-06-09 17:54:40.000000 bitcoin_qrreader-0.2.3/LICENSE
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2854 2023-07-21 11:50:05.000000 bitcoin_qrreader-0.2.3/LICENSE_UR
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1291 2023-07-22 09:27:39.837497 bitcoin_qrreader-0.2.3/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      784 2023-07-21 17:29:28.000000 bitcoin_qrreader-0.2.3/README.md
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-22 09:27:39.833497 bitcoin_qrreader-0.2.3/bitcoin_qrreader/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2023-07-20 11:25:47.000000 bitcoin_qrreader-0.2.3/bitcoin_qrreader/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    21500 2023-07-22 08:17:29.000000 bitcoin_qrreader-0.2.3/bitcoin_qrreader/bitcoin_qr.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1366 2023-07-21 11:27:49.000000 bitcoin_qrreader-0.2.3/bitcoin_qrreader/bitcoin_qr_gui.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     3849 2023-07-21 19:33:23.000000 bitcoin_qrreader-0.2.3/bitcoin_qrreader/qr_qui.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-22 09:27:39.833497 bitcoin_qrreader-0.2.3/bitcoin_qrreader.egg-info/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1291 2023-07-22 09:27:39.000000 bitcoin_qrreader-0.2.3/bitcoin_qrreader.egg-info/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1001 2023-07-22 09:27:39.000000 bitcoin_qrreader-0.2.3/bitcoin_qrreader.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-07-22 09:27:39.000000 bitcoin_qrreader-0.2.3/bitcoin_qrreader.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       47 2023-07-22 09:27:39.000000 bitcoin_qrreader-0.2.3/bitcoin_qrreader.egg-info/requires.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       28 2023-07-22 09:27:39.000000 bitcoin_qrreader-0.2.3/bitcoin_qrreader.egg-info/top_level.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2023-07-22 09:27:39.837497 bitcoin_qrreader-0.2.3/setup.cfg
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1075 2023-07-22 09:27:05.000000 bitcoin_qrreader-0.2.3/setup.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-22 09:27:39.837497 bitcoin_qrreader-0.2.3/ur/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        0 2023-07-21 11:50:05.000000 bitcoin_qrreader-0.2.3/ur/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4940 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.3/ur/bytewords.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    11377 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.3/ur/cbor_lite.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      179 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.3/ur/constants.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      729 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.3/ur/crc32.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     9669 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.3/ur/fountain_decoder.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4978 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.3/ur/fountain_encoder.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1603 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.3/ur/fountain_utils.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1568 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.3/ur/random_sampler.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      491 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.3/ur/ur.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     5115 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.3/ur/ur_decoder.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2038 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.3/ur/ur_encoder.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1638 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.3/ur/utils.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4440 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.2.3/ur/xoshiro256.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-22 09:27:39.837497 bitcoin_qrreader-0.2.3/urtypes/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1157 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.3/urtypes/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1580 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.3/urtypes/bytes.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-22 09:27:39.837497 bitcoin_qrreader-0.2.3/urtypes/cbor/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1247 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.3/urtypes/cbor/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2213 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.3/urtypes/cbor/data.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     6660 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.3/urtypes/cbor/decoder.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4937 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.3/urtypes/cbor/encoder.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-07-22 09:27:39.837497 bitcoin_qrreader-0.2.3/urtypes/crypto/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1315 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.3/urtypes/crypto/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2370 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.3/urtypes/crypto/account.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1842 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.3/urtypes/crypto/bip39.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1951 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.3/urtypes/crypto/coin_info.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2238 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.3/urtypes/crypto/ec_key.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     9315 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.3/urtypes/crypto/hd_key.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     3747 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.3/urtypes/crypto/keypath.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2467 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.3/urtypes/crypto/multi_key.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     6360 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.3/urtypes/crypto/output.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1293 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.3/urtypes/crypto/psbt.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2288 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.2.3/urtypes/registry.py
```

### Comparing `bitcoin_qrreader-0.2.2/LICENSE` & `bitcoin_qrreader-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/LICENSE_UR` & `bitcoin_qrreader-0.2.3/LICENSE_UR`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/PKG-INFO` & `bitcoin_qrreader-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitcoin_qrreader
-Version: 0.2.2
+Version: 0.2.3
 Summary: Bitcoin qr reader
 Home-page: https://github.com/andreasgriffin/bitcoin-qrreader
 Author: Andreas Griffin
 Author-email: andreasgriffin@proton.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `bitcoin_qrreader-0.2.2/README.md` & `bitcoin_qrreader-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/bitcoin_qrreader/bitcoin_qr.py` & `bitcoin_qrreader-0.2.3/bitcoin_qrreader/bitcoin_qr.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,21 +366,20 @@
         if self.data_type == DataType.Descriptor:
             return self.data.as_string_private() if self.data else self.data
         if self.data_type == DataType.KeyStoreInfo:
             return str(self.data)
         if self.data_type == DataType.PSBT:
             return str(self.data.serialize())
         if self.data_type == DataType.Tx:
-            return str(self.data.serialize())
+            return str(serialized_to_hex(self.data.serialize()))
 
-    def __str__(self) -> str:
-        if self.data_type == DataType.Descriptor:
-            return f"{self.data_type.name}: {self.data_as_string()}"
+        return str(self.data)
 
-        return f"{self.data_type.name}: {self.data}"
+    def __str__(self) -> str:
+        return f"{self.data_type.name}: {self.data_as_string()}"
 
     @classmethod
     def from_str(cls, s, network: bdk.Network):
         s = s.strip()
 
         # try is it is an bip21 uri
         # this also handles addresses without a prefix
```

### Comparing `bitcoin_qrreader-0.2.2/bitcoin_qrreader/bitcoin_qr_gui.py` & `bitcoin_qrreader-0.2.3/bitcoin_qrreader/bitcoin_qr_gui.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/bitcoin_qrreader/qr_qui.py` & `bitcoin_qrreader-0.2.3/bitcoin_qrreader/qr_qui.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/bitcoin_qrreader.egg-info/PKG-INFO` & `bitcoin_qrreader-0.2.3/bitcoin_qrreader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitcoin-qrreader
-Version: 0.2.2
+Version: 0.2.3
 Summary: Bitcoin qr reader
 Home-page: https://github.com/andreasgriffin/bitcoin-qrreader
 Author: Andreas Griffin
 Author-email: andreasgriffin@proton.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `bitcoin_qrreader-0.2.2/bitcoin_qrreader.egg-info/SOURCES.txt` & `bitcoin_qrreader-0.2.3/bitcoin_qrreader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/setup.py` & `bitcoin_qrreader-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="bitcoin_qrreader",
-    version="0.2.2",
+    version="0.2.3",
     author="Andreas Griffin",
     author_email="andreasgriffin@proton.me",
     description="Bitcoin qr reader",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andreasgriffin/bitcoin-qrreader",
     packages=find_packages(),
```

### Comparing `bitcoin_qrreader-0.2.2/ur/bytewords.py` & `bitcoin_qrreader-0.2.3/ur/bytewords.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/ur/cbor_lite.py` & `bitcoin_qrreader-0.2.3/ur/cbor_lite.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/ur/crc32.py` & `bitcoin_qrreader-0.2.3/ur/crc32.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/ur/fountain_decoder.py` & `bitcoin_qrreader-0.2.3/ur/fountain_decoder.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/ur/fountain_encoder.py` & `bitcoin_qrreader-0.2.3/ur/fountain_encoder.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/ur/fountain_utils.py` & `bitcoin_qrreader-0.2.3/ur/fountain_utils.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/ur/random_sampler.py` & `bitcoin_qrreader-0.2.3/ur/random_sampler.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/ur/ur_decoder.py` & `bitcoin_qrreader-0.2.3/ur/ur_decoder.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/ur/ur_encoder.py` & `bitcoin_qrreader-0.2.3/ur/ur_encoder.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/ur/utils.py` & `bitcoin_qrreader-0.2.3/ur/utils.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/ur/xoshiro256.py` & `bitcoin_qrreader-0.2.3/ur/xoshiro256.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/urtypes/__init__.py` & `bitcoin_qrreader-0.2.3/urtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/urtypes/bytes.py` & `bitcoin_qrreader-0.2.3/urtypes/bytes.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/urtypes/cbor/__init__.py` & `bitcoin_qrreader-0.2.3/urtypes/cbor/__init__.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/urtypes/cbor/data.py` & `bitcoin_qrreader-0.2.3/urtypes/cbor/data.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/urtypes/cbor/decoder.py` & `bitcoin_qrreader-0.2.3/urtypes/cbor/decoder.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/urtypes/cbor/encoder.py` & `bitcoin_qrreader-0.2.3/urtypes/cbor/encoder.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/urtypes/crypto/__init__.py` & `bitcoin_qrreader-0.2.3/urtypes/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/urtypes/crypto/account.py` & `bitcoin_qrreader-0.2.3/urtypes/crypto/account.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/urtypes/crypto/bip39.py` & `bitcoin_qrreader-0.2.3/urtypes/crypto/bip39.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/urtypes/crypto/coin_info.py` & `bitcoin_qrreader-0.2.3/urtypes/crypto/coin_info.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/urtypes/crypto/ec_key.py` & `bitcoin_qrreader-0.2.3/urtypes/crypto/ec_key.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/urtypes/crypto/hd_key.py` & `bitcoin_qrreader-0.2.3/urtypes/crypto/hd_key.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/urtypes/crypto/keypath.py` & `bitcoin_qrreader-0.2.3/urtypes/crypto/keypath.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/urtypes/crypto/multi_key.py` & `bitcoin_qrreader-0.2.3/urtypes/crypto/multi_key.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/urtypes/crypto/output.py` & `bitcoin_qrreader-0.2.3/urtypes/crypto/output.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/urtypes/crypto/psbt.py` & `bitcoin_qrreader-0.2.3/urtypes/crypto/psbt.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.2.2/urtypes/registry.py` & `bitcoin_qrreader-0.2.3/urtypes/registry.py`

 * *Files identical despite different names*

