# Comparing `tmp/redmage-0.4.2.tar.gz` & `tmp/redmage-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redmage-0.4.2.tar", max compression
+gzip compressed data, was "redmage-0.4.3.tar", max compression
```

## Comparing `redmage-0.4.2.tar` & `redmage-0.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.4.2/LICENSE
--rw-r--r--   0        0        0    15297 2023-07-22 17:27:13.140258 redmage-0.4.2/README.md
--rw-r--r--   0        0        0      687 2023-07-22 17:27:13.149299 redmage-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      328 2023-05-15 02:04:21.318232 redmage-0.4.2/redmage/__init__.py
--rw-r--r--   0        0        0     6936 2023-07-22 17:32:00.355849 redmage-0.4.2/redmage/components.py
--rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.4.2/redmage/convertors.py
--rw-r--r--   0        0        0     7977 2023-07-22 17:32:27.359979 redmage-0.4.2/redmage/core.py
--rw-r--r--   0        0        0     9364 2023-07-22 17:27:13.157467 redmage-0.4.2/redmage/elements.py
--rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.4.2/redmage/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.4.2/redmage/py.typed
--rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.4.2/redmage/targets.py
--rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.4.2/redmage/triggers.py
--rw-r--r--   0        0        0     1722 2023-07-13 21:46:22.902130 redmage-0.4.2/redmage/types.py
--rw-r--r--   0        0        0      644 2023-07-22 17:27:13.158467 redmage-0.4.2/redmage/utils.py
--rw-r--r--   0        0        0    15998 1970-01-01 00:00:00.000000 redmage-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.4.3/LICENSE
+-rw-r--r--   0        0        0    15297 2023-07-22 17:27:13.140258 redmage-0.4.3/README.md
+-rw-r--r--   0        0        0      687 2023-07-22 19:10:56.271201 redmage-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-05-15 02:04:21.318232 redmage-0.4.3/redmage/__init__.py
+-rw-r--r--   0        0        0     6901 2023-07-22 19:10:56.275803 redmage-0.4.3/redmage/components.py
+-rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.4.3/redmage/convertors.py
+-rw-r--r--   0        0        0     7624 2023-07-22 19:10:56.280766 redmage-0.4.3/redmage/core.py
+-rw-r--r--   0        0        0     9364 2023-07-22 17:27:13.157467 redmage-0.4.3/redmage/elements.py
+-rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.4.3/redmage/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.4.3/redmage/py.typed
+-rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.4.3/redmage/targets.py
+-rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.4.3/redmage/triggers.py
+-rw-r--r--   0        0        0     1722 2023-07-13 21:46:22.902130 redmage-0.4.3/redmage/types.py
+-rw-r--r--   0        0        0      644 2023-07-22 17:27:13.158467 redmage-0.4.3/redmage/utils.py
+-rw-r--r--   0        0        0    15998 1970-01-01 00:00:00.000000 redmage-0.4.3/PKG-INFO
```

### Comparing `redmage-0.4.2/LICENSE` & `redmage-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `redmage-0.4.2/README.md` & `redmage-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `redmage-0.4.2/pyproject.toml` & `redmage-0.4.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redmage"
-version = "0.4.2"
+version = "0.4.3"
 description = "A component based library for building htmx powered applications."
 authors = ["Scott Russell <me@scottrussell.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `redmage-0.4.2/redmage/components.py` & `redmage-0.4.3/redmage/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from .utils import astr, group_signature_param_by_kind
 
 logger = logging.getLogger("redmage")
 
 
 class Component(ABC):
     app: "Redmage"  # type: ignore
-    request = None  # type: ignore
     render_extensions: Dict[str, Any] = {}
 
     def __init_subclass__(cls, routes: Optional[Tuple[str]] = None, **kwargs: Any):
         super().__init_subclass__(**kwargs)
         cls.app.register_component(cls, routes=routes)
 
     @classmethod
```

### Comparing `redmage-0.4.2/redmage/convertors.py` & `redmage-0.4.3/redmage/convertors.py`

 * *Files identical despite different names*

### Comparing `redmage-0.4.2/redmage/core.py` & `redmage-0.4.3/redmage/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,36 +21,26 @@
 logger = logging.getLogger("redmage")
 
 
 ComponentClass = Type[Component]
 
 
 class Redmage:
-    def __init__(
-        self, middleware: Optional[Sequence[Middleware]] = None, debug: bool = False
-    ):
-        self.debug = debug
-        self.middleware = middleware
+    def __init__(self, **kwargs: Any):
+        self.kwargs = kwargs
         self.routes: List[Route] = []
         self.components: List[Tuple[ComponentClass, Optional[Tuple[str]]]] = []
         # Could cause problems if multiple apps are created
         Component.set_app(self)
 
     @property
     def starlette(self) -> Starlette:
         if not hasattr(self, "_starlette"):
             self.create_routes()
-            if self.middleware:
-                self._starlette = Starlette(
-                    debug=self.debug,
-                    routes=self.routes,
-                    middleware=self.middleware,
-                )
-            else:
-                self._starlette = Starlette(debug=self.debug, routes=self.routes)
+            self._starlette = Starlette(routes=self.routes, **self.kwargs)
         return self._starlette
 
     def create_routes(self) -> None:
         for cls, routes in self.components:
             if routes:
                 self._register_routes(cls, routes)
             self._register_targets(cls)
@@ -60,15 +50,15 @@
     ) -> None:
         self.components.append((cls, routes))
 
     def _get_explicit_route_function(self, cls: ComponentClass) -> Callable:
         async def route_function(request: Request) -> HTMLResponse:
             attrs = {**request.path_params, **request.query_params}
             instance = cls(**attrs)
-            instance.request = request  # type: ignore
+            cls.add_render_extension(request=request)
             return instance.build_response(await astr(instance))
 
         return route_function
 
     def _get_route_function(
         self, cls: ComponentClass, name: str, fn: Callable
     ) -> Callable:
```

### Comparing `redmage-0.4.2/redmage/elements.py` & `redmage-0.4.3/redmage/elements.py`

 * *Files identical despite different names*

### Comparing `redmage-0.4.2/redmage/targets.py` & `redmage-0.4.3/redmage/targets.py`

 * *Files identical despite different names*

### Comparing `redmage-0.4.2/redmage/triggers.py` & `redmage-0.4.3/redmage/triggers.py`

 * *Files identical despite different names*

### Comparing `redmage-0.4.2/redmage/types.py` & `redmage-0.4.3/redmage/types.py`

 * *Files identical despite different names*

### Comparing `redmage-0.4.2/redmage/utils.py` & `redmage-0.4.3/redmage/utils.py`

 * *Files identical despite different names*

### Comparing `redmage-0.4.2/PKG-INFO` & `redmage-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redmage
-Version: 0.4.2
+Version: 0.4.3
 Summary: A component based library for building htmx powered applications.
 License: MIT
 Author: Scott Russell
 Author-email: me@scottrussell.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

