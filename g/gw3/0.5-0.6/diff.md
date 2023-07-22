# Comparing `tmp/gw3-0.5.tar.gz` & `tmp/gw3-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gw3-0.5.tar", last modified: Thu Jul 13 10:14:43 2023, max compression
+gzip compressed data, was "gw3-0.6.tar", last modified: Sat Jul 22 15:49:05 2023, max compression
```

## Comparing `gw3-0.5.tar` & `gw3-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-13 10:14:43.267149 gw3-0.5/
--rw-r--r--   0 colt       (501) staff       (20)      643 2023-07-13 10:14:43.266664 gw3-0.5/PKG-INFO
--rw-r--r--   0 colt       (501) staff       (20)     1447 2023-07-13 09:18:18.000000 gw3-0.5/README.md
-drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-13 10:14:43.264538 gw3-0.5/gw3/
--rw-r--r--   0 colt       (501) staff       (20)       45 2023-07-13 10:10:43.000000 gw3-0.5/gw3/__init__.py
--rw-r--r--   0 colt       (501) staff       (20)     5084 2023-07-13 09:18:18.000000 gw3-0.5/gw3/client.py
-drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-13 10:14:43.266147 gw3-0.5/gw3.egg-info/
--rw-r--r--   0 colt       (501) staff       (20)      643 2023-07-13 10:14:43.000000 gw3-0.5/gw3.egg-info/PKG-INFO
--rw-r--r--   0 colt       (501) staff       (20)      182 2023-07-13 10:14:43.000000 gw3-0.5/gw3.egg-info/SOURCES.txt
--rw-r--r--   0 colt       (501) staff       (20)        1 2023-07-13 10:14:43.000000 gw3-0.5/gw3.egg-info/dependency_links.txt
--rw-r--r--   0 colt       (501) staff       (20)        9 2023-07-13 10:14:43.000000 gw3-0.5/gw3.egg-info/requires.txt
--rw-r--r--   0 colt       (501) staff       (20)        4 2023-07-13 10:14:43.000000 gw3-0.5/gw3.egg-info/top_level.txt
--rw-r--r--   0 colt       (501) staff       (20)       38 2023-07-13 10:14:43.267309 gw3-0.5/setup.cfg
--rw-r--r--   0 colt       (501) staff       (20)      781 2023-07-13 10:14:27.000000 gw3-0.5/setup.py
+drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-22 15:49:05.517461 gw3-0.6/
+-rw-r--r--   0 colt       (501) staff       (20)      643 2023-07-22 15:49:05.517175 gw3-0.6/PKG-INFO
+-rw-r--r--   0 colt       (501) staff       (20)     1436 2023-07-13 10:40:55.000000 gw3-0.6/README.md
+drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-22 15:49:05.514797 gw3-0.6/gw3/
+-rw-r--r--   0 colt       (501) staff       (20)       46 2023-07-13 10:42:41.000000 gw3-0.6/gw3/__init__.py
+-rw-r--r--   0 colt       (501) staff       (20)     5628 2023-07-22 15:45:08.000000 gw3-0.6/gw3/client.py
+drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-22 15:49:05.516684 gw3-0.6/gw3.egg-info/
+-rw-r--r--   0 colt       (501) staff       (20)      643 2023-07-22 15:49:05.000000 gw3-0.6/gw3.egg-info/PKG-INFO
+-rw-r--r--   0 colt       (501) staff       (20)      182 2023-07-22 15:49:05.000000 gw3-0.6/gw3.egg-info/SOURCES.txt
+-rw-r--r--   0 colt       (501) staff       (20)        1 2023-07-22 15:49:05.000000 gw3-0.6/gw3.egg-info/dependency_links.txt
+-rw-r--r--   0 colt       (501) staff       (20)        9 2023-07-22 15:49:05.000000 gw3-0.6/gw3.egg-info/requires.txt
+-rw-r--r--   0 colt       (501) staff       (20)        4 2023-07-22 15:49:05.000000 gw3-0.6/gw3.egg-info/top_level.txt
+-rw-r--r--   0 colt       (501) staff       (20)       38 2023-07-22 15:49:05.517577 gw3-0.6/setup.cfg
+-rw-r--r--   0 colt       (501) staff       (20)      781 2023-07-22 15:47:57.000000 gw3-0.6/setup.py
```

### Comparing `gw3-0.5/PKG-INFO` & `gw3-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gw3
-Version: 0.5
+Version: 0.6
 Summary: A Python client for the Gateway3 API
 Home-page: https://github.com/photon-storage/gw3-sdk-python
 Author: photon team
 Author-email: admin@photon.storage
 License: UNKNOWN
 Keywords: gw3,ipfs,gateway3
 Platform: UNKNOWN
```

### Comparing `gw3-0.5/README.md` & `gw3-0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 ```
 
 ### Usage
 
 Here's a simple example demonstrating the usage of the Gateway3 IPFS Gateway SDK:
 
 ```python
-from gw3 import GW3Client
+import gw3
 
-client = GW3Client(
+client = gw3.GW3Client(
     "YOUR-ACCESS-KEY",
     "YOUR-ACCESS-SECRET",
 )
 
 data = b"The Times 03/Jan/2009 Chancellor on brink of second bailout for banks"
 
 # Post the data to the IPFS network, receiving a CID as a result
```

### Comparing `gw3-0.5/gw3/client.py` & `gw3-0.6/gw3/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -155,8 +155,25 @@
         url = f"{ENDPOINT}/api/v0/name/publish?arg={cid}&key={name}"
         req = requests.Request("POST", url)
         response = self.send_request(req)
 
         if response.ok:
             return response.json()["msg"]
         else:
-            raise Exception("update_ipns API call")
+            raise Exception("update_ipns API call")
+
+    def import_ipns(self, name, value, secert_key, secert_format, seq):
+        url = f"{ENDPOINT}/api/v0/name/import"
+        payload = {
+            "name": name,
+            "value": value,
+            "secert_key": secert_key,
+            "format": secert_format,
+            "seq": seq,
+        }
+        req = requests.Request("POST", data=json.dumps(payload))
+        response = self.send_request(req)
+
+        if response.ok:
+            return response.json()["msg"]
+        else:
+            raise Exception("import_ipns API call")
```

### Comparing `gw3-0.5/gw3.egg-info/PKG-INFO` & `gw3-0.6/gw3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gw3
-Version: 0.5
+Version: 0.6
 Summary: A Python client for the Gateway3 API
 Home-page: https://github.com/photon-storage/gw3-sdk-python
 Author: photon team
 Author-email: admin@photon.storage
 License: UNKNOWN
 Keywords: gw3,ipfs,gateway3
 Platform: UNKNOWN
```

### Comparing `gw3-0.5/setup.py` & `gw3-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gw3',
-    version='0.5',
+    version='0.6',
     description='A Python client for the Gateway3 API',
     keywords=["gw3", "ipfs", "gateway3"],
     author='photon team',
     author_email='admin@photon.storage',
     url='https://github.com/photon-storage/gw3-sdk-python',
     packages=find_packages(),
     install_requires=[
```

