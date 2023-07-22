# Comparing `tmp/sixth-python-0.1.7.tar.gz` & `tmp/sixth-python-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sixth-python-0.1.7.tar", last modified: Wed Jul 12 01:03:25 2023, max compression
+gzip compressed data, was "dist/sixth-python-0.1.8.tar", last modified: Sat Jul 22 02:44:06 2023, max compression
```

## Comparing `sixth-python-0.1.7.tar` & `sixth-python-0.1.8.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-12 01:03:25.000000 sixth-python-0.1.7/
--rw-r--r--   0 mac        (501) staff       (20)     3101 2023-07-12 01:03:25.000000 sixth-python-0.1.7/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1899 2023-06-23 11:48:40.000000 sixth-python-0.1.7/README.md
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-12 01:03:25.000000 sixth-python-0.1.7/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     3760 2023-07-12 01:02:01.000000 sixth-python-0.1.7/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-12 01:03:25.000000 sixth-python-0.1.7/sixth/
--rw-r--r--   0 mac        (501) staff       (20)       27 2023-06-23 22:29:11.000000 sixth-python-0.1.7/sixth/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-12 01:03:25.000000 sixth-python-0.1.7/sixth/middlewares/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-python-0.1.7/sixth/middlewares/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3703 2023-07-11 23:56:33.000000 sixth-python-0.1.7/sixth/middlewares/encryption_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-python-0.1.7/sixth/middlewares/six_base_http_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     3924 2023-07-11 23:56:33.000000 sixth-python-0.1.7/sixth/middlewares/six_independent_rate_limiter.py
--rw-r--r--   0 mac        (501) staff       (20)     8153 2023-07-12 00:56:52.000000 sixth-python-0.1.7/sixth/middlewares/six_rate_limiter_middleware.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-12 01:03:25.000000 sixth-python-0.1.7/sixth/pen_test/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-python-0.1.7/sixth/pen_test/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      143 2023-07-09 17:50:41.000000 sixth-python-0.1.7/sixth/pen_test/auto_pen_test.py
--rw-r--r--   0 mac        (501) staff       (20)     1201 2023-07-11 23:10:12.000000 sixth-python-0.1.7/sixth/schemas.py
--rw-r--r--   0 mac        (501) staff       (20)     4246 2023-07-11 23:56:33.000000 sixth-python-0.1.7/sixth/sdk.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-12 01:03:25.000000 sixth-python-0.1.7/sixth/utils/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-python-0.1.7/sixth/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-python-0.1.7/sixth/utils/encryption_utils.py
--rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-python-0.1.7/sixth/utils/time_utils.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-12 01:03:25.000000 sixth-python-0.1.7/sixth_python.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     3101 2023-07-12 01:03:25.000000 sixth-python-0.1.7/sixth_python.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      604 2023-07-12 01:03:25.000000 sixth-python-0.1.7/sixth_python.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-12 01:03:25.000000 sixth-python-0.1.7/sixth_python.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      610 2023-07-12 01:03:25.000000 sixth-python-0.1.7/sixth_python.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        6 2023-07-12 01:03:25.000000 sixth-python-0.1.7/sixth_python.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-22 02:44:06.000000 sixth-python-0.1.8/
+-rw-r--r--   0 mac        (501) staff       (20)     3101 2023-07-22 02:44:06.000000 sixth-python-0.1.8/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1899 2023-06-23 11:48:40.000000 sixth-python-0.1.8/README.md
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-22 02:44:06.000000 sixth-python-0.1.8/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     3776 2023-07-22 02:43:43.000000 sixth-python-0.1.8/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-22 02:44:06.000000 sixth-python-0.1.8/sixth/
+-rw-r--r--   0 mac        (501) staff       (20)       27 2023-06-23 22:29:11.000000 sixth-python-0.1.8/sixth/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-22 02:44:06.000000 sixth-python-0.1.8/sixth/middlewares/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-python-0.1.8/sixth/middlewares/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3703 2023-07-22 02:37:28.000000 sixth-python-0.1.8/sixth/middlewares/encryption_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-python-0.1.8/sixth/middlewares/six_base_http_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     3924 2023-07-22 02:37:28.000000 sixth-python-0.1.8/sixth/middlewares/six_independent_rate_limiter.py
+-rw-r--r--   0 mac        (501) staff       (20)     8144 2023-07-22 02:40:39.000000 sixth-python-0.1.8/sixth/middlewares/six_rate_limiter_middleware.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-22 02:44:06.000000 sixth-python-0.1.8/sixth/pen_test/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-python-0.1.8/sixth/pen_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      143 2023-07-09 17:50:41.000000 sixth-python-0.1.8/sixth/pen_test/auto_pen_test.py
+-rw-r--r--   0 mac        (501) staff       (20)     1216 2023-07-14 11:44:21.000000 sixth-python-0.1.8/sixth/schemas.py
+-rw-r--r--   0 mac        (501) staff       (20)     4246 2023-07-22 02:37:28.000000 sixth-python-0.1.8/sixth/sdk.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-22 02:44:06.000000 sixth-python-0.1.8/sixth/utils/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-python-0.1.8/sixth/utils/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-python-0.1.8/sixth/utils/encryption_utils.py
+-rw-r--r--   0 mac        (501) staff       (20)      525 2023-07-22 02:40:45.000000 sixth-python-0.1.8/sixth/utils/pickle_db_with_lock.py
+-rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-python-0.1.8/sixth/utils/time_utils.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-22 02:44:06.000000 sixth-python-0.1.8/sixth_python.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     3101 2023-07-22 02:44:06.000000 sixth-python-0.1.8/sixth_python.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      639 2023-07-22 02:44:06.000000 sixth-python-0.1.8/sixth_python.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-22 02:44:06.000000 sixth-python-0.1.8/sixth_python.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      619 2023-07-22 02:44:06.000000 sixth-python-0.1.8/sixth_python.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        6 2023-07-22 02:44:06.000000 sixth-python-0.1.8/sixth_python.egg-info/top_level.txt
```

### Comparing `sixth-python-0.1.7/PKG-INFO` & `sixth-python-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sixth-python
-Version: 0.1.7
+Version: 0.1.8
 Summary: Sixth offical python package
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: 
         # **Sixth**
```

### Comparing `sixth-python-0.1.7/README.md` & `sixth-python-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.7/setup.py` & `sixth-python-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from pip._internal.req import parse_requirements
 
 
 
 
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 DESCRIPTION = 'Sixth offical python package'
 LONG_DESCRIPTION = '''
 # **Sixth**
 
 
 [![N|Solid](https://firebasestorage.googleapis.com/v0/b/test-103bf.appspot.com/o/waves.png?alt=media&token=0fa4c489-d9c9-4a3b-9178-593b2b018613)](https://nodesource.com/products/nsolid)
 
@@ -141,15 +141,16 @@
     "six",
     "sniffio",
     "starlette",
     "typing_extensions",
     "uritemplate",
     "urllib3",
     "uvicorn",
-    "zipp"
+    "zipp",
+    "pickleDB"
     ],
     keywords=['python', 'cybersecurity', 'pentesting', 'encryption', 'rate limiting', 'xss prevention'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

### Comparing `sixth-python-0.1.7/sixth/middlewares/encryption_middleware.py` & `sixth-python-0.1.8/sixth/middlewares/encryption_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.7/sixth/middlewares/six_base_http_middleware.py` & `sixth-python-0.1.8/sixth/middlewares/six_base_http_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.7/sixth/middlewares/six_independent_rate_limiter.py` & `sixth-python-0.1.8/sixth/middlewares/six_independent_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.7/sixth/middlewares/six_rate_limiter_middleware.py` & `sixth-python-0.1.8/sixth/middlewares/six_rate_limiter_middleware.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,66 +8,66 @@
 from starlette.middleware import Middleware
 from starlette.datastructures import MutableHeaders
 import time
 import json
 from sixth import schemas
 import re
 import requests
-from dotenv import load_dotenv
-import os
+import pickledb
 import ast
 
 
 class SixRateLimiterMiddleware(BaseHTTPMiddleware):
     def __init__(self, app: ASGIApp, apikey: str, fastapi_app: FastAPI, project_config: schemas.ProjectConfig):
         super().__init__(app)
         self._config = project_config
         self._log_dict = {}
         self._app = app
         self._apikey = apikey
         self._route_last_updated = {}
         self._rate_limit_logs_sent = {}
+        self.db = pickledb.load(f'{apikey}_db.db', auto_dump=True)
         
         for route in fastapi_app.router.routes:
-            if type(route.app )== FastAPI:
+            if type(route.app) == FastAPI:
                 for new_route in route.app.routes:
                     path = "/v"+str(route.app.version)+new_route.path
                     edited_route = re.sub(r'\W+', '~', path)
                     self._log_dict[str(edited_route)] = {}
                     self._route_last_updated[str(edited_route)] = time.time()
                     self._rate_limit_logs_sent[str(edited_route)] = 0
             else:
                 edited_route = re.sub(r'\W+', '~', route.path)
                 self._log_dict[str(edited_route)] = {}
                 self._route_last_updated[str(edited_route)] = time.time()
-                self._rate_limit_logs_sent[str(edited_route)] = 0
-                
+                self._rate_limit_logs_sent[str(edited_route)] = 0                
 
     async def set_body(self, request: Request, body: bytes):
         async def receive() -> Message:
             return {'type': 'http.request', 'body': body}
         request._receive = receive
         
     def _is_rate_limit_reached(self, uid, route):
-        timestamp = time.time()
-        requests = self._log_dict[route].get(uid, None)
         rate_limit = self._config.rate_limiter[route].rate_limit
         interval = self._config.rate_limiter[route].interval
-        if requests == None:
-            self._log_dict[route][uid] = []
-        if len(self._log_dict[route].get(uid)) < rate_limit:
-            self._log_dict[route].get(uid, []).append(timestamp)
-            return True
-            
-        new_req = [new_req for new_req in self._log_dict[route][uid] if new_req > timestamp-interval]
-        if len(new_req) < rate_limit:
-            self._log_dict[route][uid].append(timestamp)
-            return True
-        else: 
+        body = {
+            "route": route, 
+            "interval": interval, 
+            "rate_limit": rate_limit, 
+            "unique_id": uid.replace(".","~"), 
+            "user_id": self._apikey,
+            "is_active":True
+        }
+        resp = requests.post("https://backend.withsix.co/rate-limit/enquire-has-reached-rate_limit", json=body)
+        if resp.status_code == 200:
+            body =  resp.json()
+            return body["response"]
+        else:
             return False
+
         
     async def _parse_bools(self, string: bytes)-> str:
         '''
             used  to parse boolean values in string format and convert it to Python's boolean format
         '''
         string = string.decode("utf-8")
         string = string.replace(' ', "")
@@ -87,15 +87,16 @@
                 user_id=self._apikey, 
                 body=str(body), 
                 query_args=str(query), 
                 timestamp=timestamp, 
                 attack_type="No Rate Limit Attack", 
                 cwe_link="https://cwe.mitre.org/data/definitions/770.html", 
                 status="MITIGATED", 
-                learn_more_link="https://en.wikipedia.org/wiki/Rate_limiting"
+                learn_more_link="https://en.wikipedia.org/wiki/Rate_limiting", 
+                route=route
             ).dict())
             self._rate_limit_logs_sent[route]=timestamp
             
 
         
     async def dispatch(self,request: Request,call_next) -> None:
         host = request.client.host
@@ -106,18 +107,19 @@
         rate_limit_resp = None
         status_code = 200
 
         
         
         #fail safe if there is an internal server error our servers are currenly in maintnance
         try:
-            if time.time() - self._route_last_updated[route] >60:
+            update_time = time.time()
+            if update_time - self._route_last_updated[route] >60:
                 #update rate limit details every 60 seconds
                 rate_limit_resp = requests.get("https://backend.withsix.co/project-config/config/get-route-rate-limit/"+self._apikey+"/"+route)
-                self._route_last_updated[route] = time.time()
+                self._route_last_updated[route] = update_time
                 status_code = rate_limit_resp.status_code
             body = None
 
             try:
                 body = await request.body()
                 await self.set_body(request, body)
                 body = await self._parse_bools(body)
@@ -145,36 +147,34 @@
                                 preferred_id = headers[preferred_id]
                             elif rate_limit.rate_limit_type == "args":
                                 preferred_id = query_params[preferred_id]
                             else:
                                 preferred_id = host
                         
 
-                        if self._is_rate_limit_reached(preferred_id, route): 
+                        if not self._is_rate_limit_reached(preferred_id, route): 
                             _response = await call_next(request)
                             return _response
                         else:
                             await self._send_logs(route=route, header=headers, body=body, query=query_params)
                             temp_payload = rate_limit.error_payload.values()
                             final = {}
                             for c in temp_payload:
                                 for keys in c:
                                     if keys != "uid":
                                         final[keys] = c[keys]
                             output= final
                             headers = MutableHeaders(headers={"content-length": str(len(str(output).encode())), 'content-type': 'application/json'})
                             return Response(json.dumps(output), status_code=420, headers=headers)
                     else:
-                       
                         _response = await call_next(request)
                         return _response
                 except Exception as e:
                     _response = await call_next(request)
                     return _response
             else:
                 #fail safe if there is an internal server error our servers are currenly in maintnance
                 _response = await call_next(request)
                 return _response
         except Exception as e:
-            
             _response = await call_next(request)
             return _response
```

### Comparing `sixth-python-0.1.7/sixth/schemas.py` & `sixth-python-0.1.8/sixth/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,8 +43,9 @@
     user_id:str
     body:object
     query_args: object = None
     timestamp: float 
     attack_type: str
     cwe_link: str
     status: str 
-    learn_more_link: str    
+    learn_more_link: str    
+    route: str
```

### Comparing `sixth-python-0.1.7/sixth/sdk.py` & `sixth-python-0.1.8/sixth/sdk.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.7/sixth/utils/encryption_utils.py` & `sixth-python-0.1.8/sixth/utils/encryption_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.7/sixth/utils/time_utils.py` & `sixth-python-0.1.8/sixth/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.7/sixth_python.egg-info/PKG-INFO` & `sixth-python-0.1.8/sixth_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sixth-python
-Version: 0.1.7
+Version: 0.1.8
 Summary: Sixth offical python package
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: 
         # **Sixth**
```

### Comparing `sixth-python-0.1.7/sixth_python.egg-info/requires.txt` & `sixth-python-0.1.8/sixth_python.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,7 +47,8 @@
 sniffio
 starlette
 typing_extensions
 uritemplate
 urllib3
 uvicorn
 zipp
+pickleDB
```

