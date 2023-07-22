# Comparing `tmp/gw3-0.6.1.tar.gz` & `tmp/gw3-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gw3-0.6.1.tar", last modified: Sat Jul 22 15:56:46 2023, max compression
+gzip compressed data, was "gw3-0.6.2.tar", last modified: Sat Jul 22 15:59:26 2023, max compression
```

## Comparing `gw3-0.6.1.tar` & `gw3-0.6.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-22 15:56:46.138880 gw3-0.6.1/
--rw-r--r--   0 colt       (501) staff       (20)      645 2023-07-22 15:56:46.138592 gw3-0.6.1/PKG-INFO
--rw-r--r--   0 colt       (501) staff       (20)     1436 2023-07-13 10:40:55.000000 gw3-0.6.1/README.md
-drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-22 15:56:46.136234 gw3-0.6.1/gw3/
--rw-r--r--   0 colt       (501) staff       (20)       46 2023-07-13 10:42:41.000000 gw3-0.6.1/gw3/__init__.py
--rw-r--r--   0 colt       (501) staff       (20)     5640 2023-07-22 15:55:12.000000 gw3-0.6.1/gw3/client.py
-drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-22 15:56:46.138073 gw3-0.6.1/gw3.egg-info/
--rw-r--r--   0 colt       (501) staff       (20)      645 2023-07-22 15:56:46.000000 gw3-0.6.1/gw3.egg-info/PKG-INFO
--rw-r--r--   0 colt       (501) staff       (20)      182 2023-07-22 15:56:46.000000 gw3-0.6.1/gw3.egg-info/SOURCES.txt
--rw-r--r--   0 colt       (501) staff       (20)        1 2023-07-22 15:56:46.000000 gw3-0.6.1/gw3.egg-info/dependency_links.txt
--rw-r--r--   0 colt       (501) staff       (20)        9 2023-07-22 15:56:46.000000 gw3-0.6.1/gw3.egg-info/requires.txt
--rw-r--r--   0 colt       (501) staff       (20)        4 2023-07-22 15:56:46.000000 gw3-0.6.1/gw3.egg-info/top_level.txt
--rw-r--r--   0 colt       (501) staff       (20)       38 2023-07-22 15:56:46.139000 gw3-0.6.1/setup.cfg
--rw-r--r--   0 colt       (501) staff       (20)      783 2023-07-22 15:56:25.000000 gw3-0.6.1/setup.py
+drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-22 15:59:26.474100 gw3-0.6.2/
+-rw-r--r--   0 colt       (501) staff       (20)      645 2023-07-22 15:59:26.473655 gw3-0.6.2/PKG-INFO
+-rw-r--r--   0 colt       (501) staff       (20)     1436 2023-07-13 10:40:55.000000 gw3-0.6.2/README.md
+drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-22 15:59:26.471368 gw3-0.6.2/gw3/
+-rw-r--r--   0 colt       (501) staff       (20)       46 2023-07-13 10:42:41.000000 gw3-0.6.2/gw3/__init__.py
+-rw-r--r--   0 colt       (501) staff       (20)     5645 2023-07-22 15:58:31.000000 gw3-0.6.2/gw3/client.py
+drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-22 15:59:26.473106 gw3-0.6.2/gw3.egg-info/
+-rw-r--r--   0 colt       (501) staff       (20)      645 2023-07-22 15:59:26.000000 gw3-0.6.2/gw3.egg-info/PKG-INFO
+-rw-r--r--   0 colt       (501) staff       (20)      182 2023-07-22 15:59:26.000000 gw3-0.6.2/gw3.egg-info/SOURCES.txt
+-rw-r--r--   0 colt       (501) staff       (20)        1 2023-07-22 15:59:26.000000 gw3-0.6.2/gw3.egg-info/dependency_links.txt
+-rw-r--r--   0 colt       (501) staff       (20)        9 2023-07-22 15:59:26.000000 gw3-0.6.2/gw3.egg-info/requires.txt
+-rw-r--r--   0 colt       (501) staff       (20)        4 2023-07-22 15:59:26.000000 gw3-0.6.2/gw3.egg-info/top_level.txt
+-rw-r--r--   0 colt       (501) staff       (20)       38 2023-07-22 15:59:26.474248 gw3-0.6.2/setup.cfg
+-rw-r--r--   0 colt       (501) staff       (20)      783 2023-07-22 15:58:35.000000 gw3-0.6.2/setup.py
```

### Comparing `gw3-0.6.1/PKG-INFO` & `gw3-0.6.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gw3
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Python client for the Gateway3 API
 Home-page: https://github.com/photon-storage/gw3-sdk-python
 Author: photon team
 Author-email: admin@photon.storage
 License: UNKNOWN
 Keywords: gw3,ipfs,gateway3
 Platform: UNKNOWN
```

### Comparing `gw3-0.6.1/README.md` & `gw3-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `gw3-0.6.1/gw3/client.py` & `gw3-0.6.2/gw3/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,14 +167,14 @@
         payload = {
             "name": name,
             "value": value,
             "secert_key": secert_key,
             "format": secert_format,
             "seq": seq,
         }
-        req = requests.Request("POST", data=json.dumps(payload))
+        req = requests.Request("POST", url, data=json.dumps(payload))
         response = self.send_request(req)
 
         if response.ok:
             return response.json()["msg"]
         else:
             raise Exception("import_ipns API call")
```

### Comparing `gw3-0.6.1/gw3.egg-info/PKG-INFO` & `gw3-0.6.2/gw3.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gw3
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Python client for the Gateway3 API
 Home-page: https://github.com/photon-storage/gw3-sdk-python
 Author: photon team
 Author-email: admin@photon.storage
 License: UNKNOWN
 Keywords: gw3,ipfs,gateway3
 Platform: UNKNOWN
```

### Comparing `gw3-0.6.1/setup.py` & `gw3-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gw3',
-    version='0.6.1',
+    version='0.6.2',
     description='A Python client for the Gateway3 API',
     keywords=["gw3", "ipfs", "gateway3"],
     author='photon team',
     author_email='admin@photon.storage',
     url='https://github.com/photon-storage/gw3-sdk-python',
     packages=find_packages(),
     install_requires=[
```

