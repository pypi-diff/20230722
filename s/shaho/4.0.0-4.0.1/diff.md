# Comparing `tmp/shaho-4.0.0.tar.gz` & `tmp/shaho-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaho-4.0.0.tar", last modified: Sat Jul 22 11:52:53 2023, max compression
+gzip compressed data, was "shaho-4.0.1.tar", last modified: Sat Jul 22 13:34:01 2023, max compression
```

## Comparing `shaho-4.0.0.tar` & `shaho-4.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-22 11:52:52.993393 shaho-4.0.0/
--rw-rw----   0 root         (0) everybody  (9997)     1081 2023-06-19 22:22:31.000000 shaho-4.0.0/LICENCE
--rw-rw----   0 root         (0) everybody  (9997)      883 2023-07-22 11:52:52.973393 shaho-4.0.0/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)        8 2023-06-19 22:20:40.000000 shaho-4.0.0/README.md
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-22 11:52:52.993393 shaho-4.0.0/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1059 2023-07-22 11:49:07.000000 shaho-4.0.0/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-22 11:52:52.803393 shaho-4.0.0/shaho/
--rw-rw----   0 root         (0) everybody  (9997)      789 2023-07-19 14:40:37.000000 shaho-4.0.0/shaho/An_Wb.py
--rw-rw----   0 root         (0) everybody  (9997)     2412 2023-07-22 11:47:25.000000 shaho-4.0.0/shaho/Socket.py
--rw-rw----   0 root         (0) everybody  (9997)       14 2023-06-19 22:14:59.000000 shaho-4.0.0/shaho/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     4079 2023-07-19 14:40:37.000000 shaho-4.0.0/shaho/encryption.py
--rw-rw----   0 root         (0) everybody  (9997)    64261 2023-07-22 09:46:28.000000 shaho-4.0.0/shaho/mb.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-22 11:52:52.943393 shaho-4.0.0/shaho.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      883 2023-07-22 11:52:52.000000 shaho-4.0.0/shaho.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      223 2023-07-22 11:52:52.000000 shaho-4.0.0/shaho.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-22 11:52:52.000000 shaho-4.0.0/shaho.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        6 2023-07-22 11:52:52.000000 shaho-4.0.0/shaho.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-22 13:34:01.701634 shaho-4.0.1/
+-rw-rw----   0 root         (0) everybody  (9997)     1081 2023-06-19 22:22:31.000000 shaho-4.0.1/LICENCE
+-rw-rw----   0 root         (0) everybody  (9997)      883 2023-07-22 13:34:01.671634 shaho-4.0.1/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)        8 2023-06-19 22:20:40.000000 shaho-4.0.1/README.md
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-22 13:34:01.701634 shaho-4.0.1/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1059 2023-07-22 13:31:48.000000 shaho-4.0.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-22 13:34:01.521634 shaho-4.0.1/shaho/
+-rw-rw----   0 root         (0) everybody  (9997)      789 2023-07-19 14:40:37.000000 shaho-4.0.1/shaho/An_Wb.py
+-rw-rw----   0 root         (0) everybody  (9997)     2412 2023-07-22 11:47:25.000000 shaho-4.0.1/shaho/Socket.py
+-rw-rw----   0 root         (0) everybody  (9997)       14 2023-06-19 22:14:59.000000 shaho-4.0.1/shaho/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     4079 2023-07-19 14:40:37.000000 shaho-4.0.1/shaho/encryption.py
+-rw-rw----   0 root         (0) everybody  (9997)    64089 2023-07-22 13:30:21.000000 shaho-4.0.1/shaho/mb.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-22 13:34:01.651634 shaho-4.0.1/shaho.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      883 2023-07-22 13:34:00.000000 shaho-4.0.1/shaho.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      223 2023-07-22 13:34:01.000000 shaho-4.0.1/shaho.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-22 13:34:00.000000 shaho-4.0.1/shaho.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        6 2023-07-22 13:34:00.000000 shaho-4.0.1/shaho.egg-info/top_level.txt
```

### Comparing `shaho-4.0.0/LICENCE` & `shaho-4.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `shaho-4.0.0/PKG-INFO` & `shaho-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaho
-Version: 4.0.0
+Version: 4.0.1
 Summary:  library Robot
 Home-page: https://github.com
 Author: shaho
 Author-email: mbshahoorg@gmail.com
 License: MIT
 Keywords: shaho,Shaho
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `shaho-4.0.0/setup.py` & `shaho-4.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 from setuptools import setup
 
 _long_description = open('README.md').read()
 
 setup(
     name = "shaho",
-    version = "4.0.0",
+    version = "4.0.1",
     author = "shaho",
     author_email = "mbshahoorg@gmail.com",
     description = (" library Robot"),
     license = "MIT",
     keywords = ["shaho","Shaho"],
     url = "https://github.com",
     packages=['shaho'],
```

### Comparing `shaho-4.0.0/shaho/An_Wb.py` & `shaho-4.0.1/shaho/An_Wb.py`

 * *Files identical despite different names*

### Comparing `shaho-4.0.0/shaho/Socket.py` & `shaho-4.0.1/shaho/Socket.py`

 * *Files identical despite different names*

### Comparing `shaho-4.0.0/shaho/encryption.py` & `shaho-4.0.1/shaho/encryption.py`

 * *Files identical despite different names*

### Comparing `shaho-4.0.0/shaho/mb.py` & `shaho-4.0.1/shaho/mb.py`

 * *Files 1% similar despite different names*

```diff
@@ -721,15 +721,15 @@
 				"object_guid": chat_id
 			},
 			"client": SetClines.web
 		}
 
 		while 1:
 			try:
-				return loads(self.enc.decrypt(loads(self.send_post(inData))["data_enc"])).get("data").get("messages")
+				return loads(self.enc.decrypt(loads(self.send_post(inData))["data_enc"]))
 				break
 			except: continue
 
 
 	def setMembersAccess(self, chat_id, access_list):
 		inData = {
 			"method":"setGroupDefaultAccess",
@@ -738,15 +738,15 @@
 				"group_guid": chat_id
 			},
 			"client": SetClines.web
 		}
 
 		while 1:
 			try:
-				return loads(request.urlopen(request.Request(Bot._getURL(), data=dumps({"api_version":"5","auth": self.Auth,"data_enc":self.enc.encrypt(dumps(inData))}).encode(), headers={'Content-Type': 'application/json'})).read())
+				return loads(self.enc.decrypt(loads(self.send_post(inData))["data_enc"]))
 				break
 			except: continue
 
 	def getGroupMembers(self, chat_id, start_id=None):
 		inData = {
 			"method":"getGroupAllMembers",
 			"input":{
```

### Comparing `shaho-4.0.0/shaho.egg-info/PKG-INFO` & `shaho-4.0.1/shaho.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaho
-Version: 4.0.0
+Version: 4.0.1
 Summary:  library Robot
 Home-page: https://github.com
 Author: shaho
 Author-email: mbshahoorg@gmail.com
 License: MIT
 Keywords: shaho,Shaho
 Classifier: Development Status :: 3 - Alpha
```

