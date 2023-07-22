# Comparing `tmp/suanpan-sprt-0.6.5.tar.gz` & `tmp/suanpan-sprt-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/suanpan-sprt-0.6.5.tar", last modified: Tue Jul 18 09:03:50 2023, max compression
+gzip compressed data, was "dist/suanpan-sprt-0.6.6.tar", last modified: Sat Jul 22 10:21:55 2023, max compression
```

## Comparing `suanpan-sprt-0.6.5.tar` & `suanpan-sprt-0.6.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      129 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/README.md
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/setup.cfg
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/setup.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/sprt/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/sprt/__init__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4337 2023-07-18 09:03:49.000000 suanpan-sprt-0.6.5/sprt/__main__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/sprt/arguments.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1251 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/sprt/envs.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/sprt/exceptions.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5737 2023-07-18 07:58:15.000000 suanpan-sprt-0.6.5/sprt/loader.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2087 2023-07-17 07:00:31.000000 suanpan-sprt-0.6.5/sprt/log.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/sprt/master.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6876 2023-07-18 08:32:10.000000 suanpan-sprt-0.6.5/sprt/server.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6419 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/sprt/storage.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3261 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/sprt/testing.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1290 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/sprt/utils.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-07-18 09:03:49.000000 suanpan-sprt-0.6.5/sprt/version.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/suanpan_sprt.egg-info/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/suanpan_sprt.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/suanpan_sprt.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/suanpan_sprt.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/suanpan_sprt.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/suanpan_sprt.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/suanpan_sprt.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-22 10:21:55.000000 suanpan-sprt-0.6.6/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-22 10:21:55.000000 suanpan-sprt-0.6.6/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      129 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.6/README.md
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-07-22 10:21:55.000000 suanpan-sprt-0.6.6/setup.cfg
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.6/setup.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-22 10:21:55.000000 suanpan-sprt-0.6.6/sprt/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.6/sprt/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4337 2023-07-18 09:03:49.000000 suanpan-sprt-0.6.6/sprt/__main__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.6/sprt/arguments.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1251 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.6/sprt/envs.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.6/sprt/exceptions.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6021 2023-07-22 10:21:55.000000 suanpan-sprt-0.6.6/sprt/loader.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2087 2023-07-17 07:00:31.000000 suanpan-sprt-0.6.6/sprt/log.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      903 2023-07-22 10:21:55.000000 suanpan-sprt-0.6.6/sprt/master.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6917 2023-07-22 10:21:55.000000 suanpan-sprt-0.6.6/sprt/server.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6419 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.6/sprt/storage.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3261 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.6/sprt/testing.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1290 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.6/sprt/utils.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-07-22 10:21:55.000000 suanpan-sprt-0.6.6/sprt/version.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-22 10:21:55.000000 suanpan-sprt-0.6.6/suanpan_sprt.egg-info/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-22 10:21:55.000000 suanpan-sprt-0.6.6/suanpan_sprt.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-07-22 10:21:55.000000 suanpan-sprt-0.6.6/suanpan_sprt.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-07-22 10:21:55.000000 suanpan-sprt-0.6.6/suanpan_sprt.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-07-22 10:21:55.000000 suanpan-sprt-0.6.6/suanpan_sprt.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-07-22 10:21:55.000000 suanpan-sprt-0.6.6/suanpan_sprt.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-07-22 10:21:55.000000 suanpan-sprt-0.6.6/suanpan_sprt.egg-info/top_level.txt
```

### Comparing `suanpan-sprt-0.6.5/setup.py` & `suanpan-sprt-0.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.5/sprt/__main__.py` & `suanpan-sprt-0.6.6/sprt/__main__.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.5/sprt/arguments.py` & `suanpan-sprt-0.6.6/sprt/arguments.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.5/sprt/envs.py` & `suanpan-sprt-0.6.6/sprt/envs.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.5/sprt/loader.py` & `suanpan-sprt-0.6.6/sprt/loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import logging
 import inspect
 import pathlib
 import importlib
 import importlib.util
+from quart import current_app
 from .arguments import init_arg_from_arg_spec, init_return_from_value, DEFAULT_DATA_SUBTYPE_ARGS_MAP
 from .storage import Storage
 from .exceptions import ParamsArgError, InvocationFunctionError
 from .log import NodeStreamHandler, LogkitHandler
 
 
 class NodeFunction(object):
@@ -96,19 +97,20 @@
             self._logkit.removeHandler(self._logkit_handler)
         else:
             if self._logkit_handler and logkit.uri != self._logkit_handler.uri:
                 self._logkit.removeHandler(self._logkit_handler)
                 self._logkit_handler = None
 
             if self._logkit_handler is None:
+                logging.info('setup logkit handler: %s', logkit.uri)
                 lh = LogkitHandler(logkit.uri, logkit.namespace, logkit.path, logkit.events_append)
-                lh.setLevel('INFO')
+                lh.setLevel(logkit.logs_level.upper())
                 self._logkit.addHandler(lh)
                 self._logkit_handler = lh
-                self._logkit.setLevel(logkit.logs_level.upper())
+                # self._logkit.setLevel(logkit.logs_level.upper())
 
     @staticmethod
     def _init_logkit(app_id, node_id):
         name = f'logkit_{app_id}_{node_id}'
         logger = logging.getLogger(name)
         logger.propagate = False
 
@@ -121,14 +123,17 @@
         sh.setFormatter(formatter)
         logger.addHandler(sh)
 
         return logger
 
     def __del__(self):
         # os.remove(self.location)
+        if self._logkit_handler:
+            current_app.logger.info('close logkit handler: %s', self._logkit_handler.uri)
+            self._logkit_handler.close()
         self._logkit.handlers.clear()
         del self.module
 
 
 class RuntimeContext(object):
     def __init__(self, user_id, app_id, node_id):
         self.request_id = None
```

### Comparing `suanpan-sprt-0.6.5/sprt/log.py` & `suanpan-sprt-0.6.6/sprt/log.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.5/sprt/master.py` & `suanpan-sprt-0.6.6/sprt/master.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         envs.userSignatureHeaderField: signature_v1(envs.accessSecret, envs.userId),
         envs.userSignVersionHeaderField: "v1",
     }
 
 
 def sio(*args, **kwargs):
     kwargs["headers"] = {**default_headers(), **kwargs.pop("headers", {})}
-    client = socketio.Client()
+    client = socketio.Client(reconnection_attempts=3)
     client.connect(*args, **kwargs)
 
     return client
 
 
 def get_token():
     # TODO: add for oss
```

### Comparing `suanpan-sprt-0.6.5/sprt/server.py` & `suanpan-sprt-0.6.6/sprt/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import gc
 import json
 import logging
 import typing
 import pathlib
 import dataclasses
 import pydantic
+from quart import current_app
 from contextlib import redirect_stdout, redirect_stderr, contextmanager
 from quart import Quart
 from quart_schema import QuartSchema, validate_request, validate_response, RequestSchemaValidationError
 from quart_schema import validation
 from . import loader, envs, exceptions, utils
 
 
@@ -158,15 +159,15 @@
 async def background_garbage_collection(app_id):
     del_nodes = []
     for node_id, node_function in module_imported.items():
         if node_function.context.app_id == app_id:
             del_nodes.append(node_id)
 
     for node_id in del_nodes:
-        logging.info(f'node {node_id} release')
+        current_app.logger.info(f'node {node_id} release')
         del module_imported[node_id]
 
     gc.collect()
 
 module_imported = {}
```

### Comparing `suanpan-sprt-0.6.5/sprt/storage.py` & `suanpan-sprt-0.6.6/sprt/storage.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.5/sprt/testing.py` & `suanpan-sprt-0.6.6/sprt/testing.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.5/sprt/utils.py` & `suanpan-sprt-0.6.6/sprt/utils.py`

 * *Files identical despite different names*

