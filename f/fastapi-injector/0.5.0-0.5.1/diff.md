# Comparing `tmp/fastapi_injector-0.5.0.tar.gz` & `tmp/fastapi_injector-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_injector-0.5.0.tar", max compression
+gzip compressed data, was "fastapi_injector-0.5.1.tar", max compression
```

## Comparing `fastapi_injector-0.5.0.tar` & `fastapi_injector-0.5.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1326 2021-11-29 20:05:35.155753 fastapi_injector-0.5.0/LICENSE
--rw-r--r--   0        0        0     6332 2023-05-19 18:58:07.855882 fastapi_injector-0.5.0/README.md
--rw-r--r--   0        0        0      673 2023-05-19 18:47:49.138684 fastapi_injector-0.5.0/fastapi_injector/__init__.py
--rw-r--r--   0        0        0      618 2022-06-17 17:58:35.653761 fastapi_injector-0.5.0/fastapi_injector/attach.py
--rw-r--r--   0        0        0      217 2022-06-17 17:58:35.653761 fastapi_injector-0.5.0/fastapi_injector/exceptions.py
--rw-r--r--   0        0        0      971 2023-02-01 19:17:45.406262 fastapi_injector-0.5.0/fastapi_injector/injected.py
--rw-r--r--   0        0        0        0 2022-06-06 16:52:41.573382 fastapi_injector-0.5.0/fastapi_injector/py.typed
--rw-r--r--   0        0        0     3440 2023-05-19 18:47:49.138684 fastapi_injector-0.5.0/fastapi_injector/request_scope.py
--rw-r--r--   0        0        0      894 2023-05-19 18:49:42.232117 fastapi_injector-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     7288 1970-01-01 00:00:00.000000 fastapi_injector-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1326 2021-11-29 20:05:35.155753 fastapi_injector-0.5.1/LICENSE
+-rw-r--r--   0        0        0     6332 2023-05-19 18:58:07.855882 fastapi_injector-0.5.1/README.md
+-rw-r--r--   0        0        0      673 2023-05-19 18:47:49.138684 fastapi_injector-0.5.1/fastapi_injector/__init__.py
+-rw-r--r--   0        0        0      618 2022-06-17 17:58:35.653761 fastapi_injector-0.5.1/fastapi_injector/attach.py
+-rw-r--r--   0        0        0      217 2022-06-17 17:58:35.653761 fastapi_injector-0.5.1/fastapi_injector/exceptions.py
+-rw-r--r--   0        0        0     1010 2023-07-22 15:41:46.719943 fastapi_injector-0.5.1/fastapi_injector/injected.py
+-rw-r--r--   0        0        0        0 2022-06-06 16:52:41.573382 fastapi_injector-0.5.1/fastapi_injector/py.typed
+-rw-r--r--   0        0        0     3440 2023-05-19 18:47:49.138684 fastapi_injector-0.5.1/fastapi_injector/request_scope.py
+-rw-r--r--   0        0        0      898 2023-07-22 15:42:54.076644 fastapi_injector-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7288 1970-01-01 00:00:00.000000 fastapi_injector-0.5.1/PKG-INFO
```

### Comparing `fastapi_injector-0.5.0/LICENSE` & `fastapi_injector-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_injector-0.5.0/README.md` & `fastapi_injector-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_injector-0.5.0/fastapi_injector/__init__.py` & `fastapi_injector-0.5.1/fastapi_injector/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_injector-0.5.0/fastapi_injector/attach.py` & `fastapi_injector-0.5.1/fastapi_injector/attach.py`

 * *Files identical despite different names*

### Comparing `fastapi_injector-0.5.0/fastapi_injector/injected.py` & `fastapi_injector-0.5.1/fastapi_injector/injected.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from typing import Any, TypeVar
 
-from fastapi import Depends, Request
+from fastapi import Depends
+from starlette.requests import HTTPConnection
 
 from fastapi_injector.attach import get_injector_instance
 
 BoundInterface = TypeVar("BoundInterface", bound=type)
 
 
 def Injected(interface: BoundInterface) -> Any:  # pylint: disable=invalid-name
     """
     Asks your injector instance for the specified type,
     allowing you to use it in the route.
     """
 
-    async def inject_into_route(request: Request) -> BoundInterface:
-        return get_injector_instance(request.app).get(interface)
+    async def inject_into_route(conn: HTTPConnection) -> BoundInterface:
+        return get_injector_instance(conn.app).get(interface)
 
     return Depends(inject_into_route)
 
 
 def SyncInjected(interface: BoundInterface) -> Any:  # pylint: disable=invalid-name
     """
     Asks your injector instance for the specified type,
     allowing you to use it in the route. Intended for use
     with synchronous interfaces.
     """
 
-    def inject_into_route(request: Request) -> BoundInterface:
-        return get_injector_instance(request.app).get(interface)
+    def inject_into_route(conn: HTTPConnection) -> BoundInterface:
+        return get_injector_instance(conn.app).get(interface)
 
     return Depends(inject_into_route)
```

### Comparing `fastapi_injector-0.5.0/fastapi_injector/request_scope.py` & `fastapi_injector-0.5.1/fastapi_injector/request_scope.py`

 * *Files identical despite different names*

### Comparing `fastapi_injector-0.5.0/pyproject.toml` & `fastapi_injector-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-injector"
-version = "0.5.0"
+version = "0.5.1"
 description = "python-injector integration for FastAPI"
 authors = ["Matyas Richter <matyas@mrichter.cz>"]
 license = "BSD"
 repository = "https://github.com/matyasrichter/fastapi-injector"
 packages = [
     {include = "fastapi_injector"},
 ]
@@ -23,13 +23,13 @@
 fastapi = ">=0.70.0"
 injector = ">=0.19.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-asyncio = ">=0.20.3,<0.22.0"
 pytest-cov = "^4.0.0"
-pre-commit = "^2.21.0"
+pre-commit = ">=2.21,<4.0"
 httpx = "^0.23.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fastapi_injector-0.5.0/PKG-INFO` & `fastapi_injector-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-injector
-Version: 0.5.0
+Version: 0.5.1
 Summary: python-injector integration for FastAPI
 Home-page: https://github.com/matyasrichter/fastapi-injector
 License: BSD
 Author: Matyas Richter
 Author-email: matyas@mrichter.cz
 Requires-Python: >=3.8,<3.12
 Classifier: Environment :: Web Environment
```

