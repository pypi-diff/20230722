# Comparing `tmp/pipedrive-wrapper-1.0.3.tar.gz` & `tmp/pipedrive-wrapper-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipedrive-wrapper-1.0.3.tar", last modified: Sat Jul 22 15:19:50 2023, max compression
+gzip compressed data, was "pipedrive-wrapper-1.0.4.tar", last modified: Sat Jul 22 15:22:49 2023, max compression
```

## Comparing `pipedrive-wrapper-1.0.3.tar` & `pipedrive-wrapper-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 15:19:50.374375 pipedrive-wrapper-1.0.3/
--rw-rw-rw-   0        0        0     1092 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      705 2023-07-22 15:19:50.374375 pipedrive-wrapper-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       65 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 15:19:50.345051 pipedrive-wrapper-1.0.3/pipedrive/
--rw-rw-rw-   0        0        0        0 2023-05-07 15:48:01.000000 pipedrive-wrapper-1.0.3/pipedrive/__init__.py
--rw-rw-rw-   0        0        0     3628 2023-07-16 14:41:55.000000 pipedrive-wrapper-1.0.3/pipedrive/activity.py
--rw-rw-rw-   0        0        0     2915 2023-07-16 14:41:50.000000 pipedrive-wrapper-1.0.3/pipedrive/client.py
--rw-rw-rw-   0        0        0     6459 2023-07-22 15:16:43.000000 pipedrive-wrapper-1.0.3/pipedrive/deal.py
--rw-rw-rw-   0        0        0      627 2023-07-22 15:14:59.000000 pipedrive-wrapper-1.0.3/pipedrive/deal_field.py
--rw-rw-rw-   0        0        0      855 2023-06-06 19:39:27.000000 pipedrive-wrapper-1.0.3/pipedrive/exceptions.py
--rw-rw-rw-   0        0        0     5541 2023-07-16 14:42:13.000000 pipedrive-wrapper-1.0.3/pipedrive/person.py
--rw-rw-rw-   0        0        0     3319 2023-06-06 19:04:08.000000 pipedrive-wrapper-1.0.3/pipedrive/util.py
-drwxrwxrwx   0        0        0        0 2023-07-22 15:19:50.372974 pipedrive-wrapper-1.0.3/pipedrive_wrapper.egg-info/
--rw-rw-rw-   0        0        0      705 2023-07-22 15:19:50.000000 pipedrive-wrapper-1.0.3/pipedrive_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-07-22 15:19:50.000000 pipedrive-wrapper-1.0.3/pipedrive_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 15:19:50.000000 pipedrive-wrapper-1.0.3/pipedrive_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-22 15:19:50.000000 pipedrive-wrapper-1.0.3/pipedrive_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-22 15:19:50.000000 pipedrive-wrapper-1.0.3/pipedrive_wrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-22 15:19:50.374375 pipedrive-wrapper-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-07-22 15:16:58.000000 pipedrive-wrapper-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 15:22:49.281206 pipedrive-wrapper-1.0.4/
+-rw-rw-rw-   0        0        0     1092 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      705 2023-07-22 15:22:49.280203 pipedrive-wrapper-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       65 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 15:22:49.262123 pipedrive-wrapper-1.0.4/pipedrive/
+-rw-rw-rw-   0        0        0        0 2023-05-07 15:48:01.000000 pipedrive-wrapper-1.0.4/pipedrive/__init__.py
+-rw-rw-rw-   0        0        0     3628 2023-07-16 14:41:55.000000 pipedrive-wrapper-1.0.4/pipedrive/activity.py
+-rw-rw-rw-   0        0        0     2993 2023-07-22 15:22:11.000000 pipedrive-wrapper-1.0.4/pipedrive/client.py
+-rw-rw-rw-   0        0        0     6459 2023-07-22 15:16:43.000000 pipedrive-wrapper-1.0.4/pipedrive/deal.py
+-rw-rw-rw-   0        0        0      627 2023-07-22 15:14:59.000000 pipedrive-wrapper-1.0.4/pipedrive/deal_field.py
+-rw-rw-rw-   0        0        0      855 2023-06-06 19:39:27.000000 pipedrive-wrapper-1.0.4/pipedrive/exceptions.py
+-rw-rw-rw-   0        0        0     5541 2023-07-16 14:42:13.000000 pipedrive-wrapper-1.0.4/pipedrive/person.py
+-rw-rw-rw-   0        0        0     3319 2023-06-06 19:04:08.000000 pipedrive-wrapper-1.0.4/pipedrive/util.py
+drwxrwxrwx   0        0        0        0 2023-07-22 15:22:49.279203 pipedrive-wrapper-1.0.4/pipedrive_wrapper.egg-info/
+-rw-rw-rw-   0        0        0      705 2023-07-22 15:22:49.000000 pipedrive-wrapper-1.0.4/pipedrive_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-07-22 15:22:49.000000 pipedrive-wrapper-1.0.4/pipedrive_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 15:22:49.000000 pipedrive-wrapper-1.0.4/pipedrive_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-22 15:22:49.000000 pipedrive-wrapper-1.0.4/pipedrive_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-22 15:22:49.000000 pipedrive-wrapper-1.0.4/pipedrive_wrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-22 15:22:49.281206 pipedrive-wrapper-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-07-22 15:22:26.000000 pipedrive-wrapper-1.0.4/setup.py
```

### Comparing `pipedrive-wrapper-1.0.3/LICENSE` & `pipedrive-wrapper-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.3/PKG-INFO` & `pipedrive-wrapper-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipedrive-wrapper
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python wrapper for the Pipedrive API
 Home-page: https://github.com/ppcantidio/pipedrive.py
 Author: Pedro Cantidio
 Author-email: ppcantidio@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pipedrive-wrapper-1.0.3/pipedrive/activity.py` & `pipedrive-wrapper-1.0.4/pipedrive/activity.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.3/pipedrive/client.py` & `pipedrive-wrapper-1.0.4/pipedrive/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import requests
 
 from .activity import Activity
 from .deal import Deal
+from .deal_field import DealField
 from .exceptions import BadRequest, Forbidden, InternalServerError, NotFound, TooManyRequests, Unauthorized
 from .person import Person
 
 
 class Client:
     def __init__(self, token: str) -> None:
         self.base_url = "https://api.pipedrive.com/v1"
         self.token = token
         self.headers = {"Accept": "application/json"}
         self.activity = Activity(self)
         self.person = Person(self)
         self.deal = Deal(self)
+        self.deal_field = DealField(self)
 
     def _post(self, url_context: str, body: dict):
         url_to_request = self.__generate_url_to_request(url_context)
 
         body = self.__check_values_of_dict(body)
 
         response = requests.post(
```

### Comparing `pipedrive-wrapper-1.0.3/pipedrive/deal.py` & `pipedrive-wrapper-1.0.4/pipedrive/deal.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.3/pipedrive/deal_field.py` & `pipedrive-wrapper-1.0.4/pipedrive/deal_field.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.3/pipedrive/exceptions.py` & `pipedrive-wrapper-1.0.4/pipedrive/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.3/pipedrive/person.py` & `pipedrive-wrapper-1.0.4/pipedrive/person.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.3/pipedrive/util.py` & `pipedrive-wrapper-1.0.4/pipedrive/util.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.3/pipedrive_wrapper.egg-info/PKG-INFO` & `pipedrive-wrapper-1.0.4/pipedrive_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipedrive-wrapper
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python wrapper for the Pipedrive API
 Home-page: https://github.com/ppcantidio/pipedrive.py
 Author: Pedro Cantidio
 Author-email: ppcantidio@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pipedrive-wrapper-1.0.3/setup.py` & `pipedrive-wrapper-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="pipedrive-wrapper",
-    version="1.0.3",
+    version="1.0.4",
     author="Pedro Cantidio",
     author_email="ppcantidio@gmail.com",
     description="A Python wrapper for the Pipedrive API",
     long_description="A Python wrapper that simplifies interaction with the Pipedrive API",
     url="https://github.com/ppcantidio/pipedrive.py",
     packages=find_packages(exclude=["tests"]),
     classifiers=[
```

