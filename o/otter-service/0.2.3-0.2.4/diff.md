# Comparing `tmp/otter_service-0.2.3.tar.gz` & `tmp/otter_service-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otter_service-0.2.3.tar", last modified: Fri Jul 21 21:02:28 2023, max compression
+gzip compressed data, was "otter_service-0.2.4.tar", last modified: Fri Jul 21 22:48:36 2023, max compression
```

## Comparing `otter_service-0.2.3.tar` & `otter_service-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 21:02:28.432687 otter_service-0.2.3/
--rw-r--r--   0 sean       (501) staff       (20)     1498 2021-10-24 00:07:22.000000 otter_service-0.2.3/LICENSE
--rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-21 21:02:28.432941 otter_service-0.2.3/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)     7704 2023-07-21 17:54:42.000000 otter_service-0.2.3/README.md
--rw-r--r--   0 sean       (501) staff       (20)      103 2023-07-20 15:40:45.000000 otter_service-0.2.3/pyproject.toml
--rw-r--r--   0 sean       (501) staff       (20)      786 2023-07-21 21:02:28.434100 otter_service-0.2.3/setup.cfg
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 21:02:28.419700 otter_service-0.2.3/src/
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 21:02:28.425184 otter_service-0.2.3/src/otter_service/
--rw-r--r--   0 sean       (501) staff       (20)       22 2023-07-21 21:01:08.000000 otter_service-0.2.3/src/otter_service/__init__.py
--rw-r--r--   0 sean       (501) staff       (20)     1722 2023-07-21 17:51:59.000000 otter_service-0.2.3/src/otter_service/access_sops_keys.py
--rw-r--r--   0 sean       (501) staff       (20)     1035 2022-09-01 01:54:36.000000 otter_service-0.2.3/src/otter_service/firestore-test.py
--rw-r--r--   0 sean       (501) staff       (20)     5059 2023-07-21 21:00:48.000000 otter_service-0.2.3/src/otter_service/grade_assignment.py
--rw-r--r--   0 sean       (501) staff       (20)    19675 2023-07-21 21:01:08.000000 otter_service-0.2.3/src/otter_service/otter_nb.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 21:02:28.429137 otter_service-0.2.3/src/otter_service/secrets/
--rw-r--r--   0 sean       (501) staff       (20)      983 2023-07-21 17:51:59.000000 otter_service-0.2.3/src/otter_service/secrets/gh_key.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1229 2022-06-11 00:39:08.000000 otter_service-0.2.3/src/otter_service/secrets/gke_key.yaml
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 21:02:28.428120 otter_service-0.2.3/src/otter_service.egg-info/
--rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-21 21:02:28.000000 otter_service-0.2.3/src/otter_service.egg-info/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)      584 2023-07-21 21:02:28.000000 otter_service-0.2.3/src/otter_service.egg-info/SOURCES.txt
--rw-r--r--   0 sean       (501) staff       (20)        1 2023-07-21 21:02:28.000000 otter_service-0.2.3/src/otter_service.egg-info/dependency_links.txt
--rw-r--r--   0 sean       (501) staff       (20)       62 2023-07-21 21:02:28.000000 otter_service-0.2.3/src/otter_service.egg-info/entry_points.txt
--rw-r--r--   0 sean       (501) staff       (20)       14 2023-07-21 21:02:28.000000 otter_service-0.2.3/src/otter_service.egg-info/top_level.txt
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 21:02:28.432340 otter_service-0.2.3/tests/
--rw-r--r--   0 sean       (501) staff       (20)      895 2022-06-18 01:43:56.000000 otter_service-0.2.3/tests/test_access_sops_keys.py
--rw-r--r--   0 sean       (501) staff       (20)     1416 2023-07-21 17:51:59.000000 otter_service-0.2.3/tests/test_grade_assignment.py
--rw-r--r--   0 sean       (501) staff       (20)     2094 2023-07-21 21:00:48.000000 otter_service-0.2.3/tests/test_otter_nb.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 22:48:36.668910 otter_service-0.2.4/
+-rw-r--r--   0 sean       (501) staff       (20)     1498 2021-10-24 00:07:22.000000 otter_service-0.2.4/LICENSE
+-rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-21 22:48:36.669122 otter_service-0.2.4/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)     7704 2023-07-21 17:54:42.000000 otter_service-0.2.4/README.md
+-rw-r--r--   0 sean       (501) staff       (20)      103 2023-07-20 15:40:45.000000 otter_service-0.2.4/pyproject.toml
+-rw-r--r--   0 sean       (501) staff       (20)      786 2023-07-21 22:48:36.670053 otter_service-0.2.4/setup.cfg
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 22:48:36.653994 otter_service-0.2.4/src/
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 22:48:36.660045 otter_service-0.2.4/src/otter_service/
+-rw-r--r--   0 sean       (501) staff       (20)       22 2023-07-21 22:47:47.000000 otter_service-0.2.4/src/otter_service/__init__.py
+-rw-r--r--   0 sean       (501) staff       (20)     1722 2023-07-21 17:51:59.000000 otter_service-0.2.4/src/otter_service/access_sops_keys.py
+-rw-r--r--   0 sean       (501) staff       (20)     1025 2023-07-21 21:37:40.000000 otter_service-0.2.4/src/otter_service/firestore-test.py
+-rw-r--r--   0 sean       (501) staff       (20)     5059 2023-07-21 21:13:17.000000 otter_service-0.2.4/src/otter_service/grade_assignment.py
+-rw-r--r--   0 sean       (501) staff       (20)    19655 2023-07-21 22:47:47.000000 otter_service-0.2.4/src/otter_service/otter_nb.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 22:48:36.663850 otter_service-0.2.4/src/otter_service/secrets/
+-rw-r--r--   0 sean       (501) staff       (20)      983 2023-07-21 17:51:59.000000 otter_service-0.2.4/src/otter_service/secrets/gh_key.yaml
+-rw-r--r--   0 sean       (501) staff       (20)     1229 2022-06-11 00:39:08.000000 otter_service-0.2.4/src/otter_service/secrets/gke_key.yaml
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 22:48:36.662629 otter_service-0.2.4/src/otter_service.egg-info/
+-rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-21 22:48:36.000000 otter_service-0.2.4/src/otter_service.egg-info/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)      584 2023-07-21 22:48:36.000000 otter_service-0.2.4/src/otter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 sean       (501) staff       (20)        1 2023-07-21 22:48:36.000000 otter_service-0.2.4/src/otter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 sean       (501) staff       (20)       62 2023-07-21 22:48:36.000000 otter_service-0.2.4/src/otter_service.egg-info/entry_points.txt
+-rw-r--r--   0 sean       (501) staff       (20)       14 2023-07-21 22:48:36.000000 otter_service-0.2.4/src/otter_service.egg-info/top_level.txt
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 22:48:36.668444 otter_service-0.2.4/tests/
+-rw-r--r--   0 sean       (501) staff       (20)      895 2022-06-18 01:43:56.000000 otter_service-0.2.4/tests/test_access_sops_keys.py
+-rw-r--r--   0 sean       (501) staff       (20)     1416 2023-07-21 17:51:59.000000 otter_service-0.2.4/tests/test_grade_assignment.py
+-rw-r--r--   0 sean       (501) staff       (20)     2140 2023-07-21 22:47:47.000000 otter_service-0.2.4/tests/test_otter_nb.py
```

### Comparing `otter_service-0.2.3/LICENSE` & `otter_service-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.3/PKG-INFO` & `otter_service-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter_service
-Version: 0.2.3
+Version: 0.2.4
 Summary: Grading Service for Edx 8x courses
 Home-page: https://github.com/data-8/otter-service
 Author: Vincent Su and Sean Morris
 Author-email: sean.smorris@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `otter_service-0.2.3/README.md` & `otter_service-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.3/setup.cfg` & `otter_service-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.3/src/otter_service/access_sops_keys.py` & `otter_service-0.2.4/src/otter_service/access_sops_keys.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.3/src/otter_service/firestore-test.py` & `otter_service-0.2.4/src/otter_service/firestore-test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import firebase_admin
 from firebase_admin import credentials
 from firebase_admin import firestore
-import os
 from datetime import datetime
 from pytz import timezone
 import pytz
 
 # Use the application default credentials
 # cred = credentials.ApplicationDefault()
 # firebase_admin.initialize_app(cred, {
```

### Comparing `otter_service-0.2.3/src/otter_service/grade_assignment.py` & `otter_service-0.2.4/src/otter_service/grade_assignment.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.3/src/otter_service/otter_nb.py` & `otter_service-0.2.4/src/otter_service/otter_nb.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import signal
 from functools import partial
 import traceback
 from datetime import datetime
 import os
 from hashlib import sha1
 from oauthlib.oauth1.rfc5849 import signature, parameters
-import pandas as pd
 import pytz
 from pytz import timezone
 from jupyterhub.services.auth import HubOAuthenticated
 from lxml import etree
 import aiohttp
 import async_timeout
 import tornado.web
```

### Comparing `otter_service-0.2.3/src/otter_service/secrets/gh_key.yaml` & `otter_service-0.2.4/src/otter_service/secrets/gh_key.yaml`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.3/src/otter_service/secrets/gke_key.yaml` & `otter_service-0.2.4/src/otter_service/secrets/gke_key.yaml`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.3/src/otter_service.egg-info/PKG-INFO` & `otter_service-0.2.4/src/otter_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-service
-Version: 0.2.3
+Version: 0.2.4
 Summary: Grading Service for Edx 8x courses
 Home-page: https://github.com/data-8/otter-service
 Author: Vincent Su and Sean Morris
 Author-email: sean.smorris@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `otter_service-0.2.3/src/otter_service.egg-info/SOURCES.txt` & `otter_service-0.2.4/src/otter_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.3/tests/test_access_sops_keys.py` & `otter_service-0.2.4/tests/test_access_sops_keys.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.3/tests/test_grade_assignment.py` & `otter_service-0.2.4/tests/test_grade_assignment.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.3/tests/test_otter_nb.py` & `otter_service-0.2.4/tests/test_otter_nb.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,21 +18,22 @@
     channel = grpc.insecure_channel("localhost:8080")
     transport = firestore_grpc_transport.FirestoreGrpcTransport(channel=channel)
     db = firestore.client()
     db._firestore_api_internal = firestore_client.FirestoreClient(transport=transport)
     yield db
 
 
-@pytest.mark.skip(reason="test oauth2 now")
+@pytest.mark.skip(reason="test oauth2")
 async def test_http_client(http_server_client):
     resp = await http_server_client.fetch('/services/otter_grade/')
     assert resp.code == 302
     http_server_client.close()
 
 
+@pytest.mark.skip(reason="tests local firestore")
 def test_write_grade(firebase_local):
     grade_info = {"userid": "WRITE_TEST", "course": "8x-test", "grade": 88.0, "section": "1", "assignment": "lab99"}
     doc = gn.write_grade(grade_info)[1]
     doc_ref = firebase_local.collection(f'{os.environ.get("ENVIRONMENT")}-grades').document(f'{doc.id}')
     doc_obj = doc_ref.get()
     doc_dict = doc_obj.to_dict()
```

