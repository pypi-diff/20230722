# Comparing `tmp/redmage-0.3.1.tar.gz` & `tmp/redmage-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redmage-0.3.1.tar", max compression
+gzip compressed data, was "redmage-0.4.2.tar", max compression
```

## Comparing `redmage-0.3.1.tar` & `redmage-0.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.3.1/LICENSE
--rw-r--r--   0        0        0    15237 2023-07-11 04:23:19.514090 redmage-0.3.1/README.md
--rw-r--r--   0        0        0      660 2023-07-11 04:29:40.809276 redmage-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      328 2023-05-15 02:04:21.318232 redmage-0.3.1/redmage/__init__.py
--rw-r--r--   0        0        0     6832 2023-07-11 04:29:40.810276 redmage-0.3.1/redmage/components.py
--rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.3.1/redmage/convertors.py
--rw-r--r--   0        0        0     7832 2023-07-11 04:19:56.895119 redmage-0.3.1/redmage/core.py
--rw-r--r--   0        0        0     9782 2023-07-11 00:57:08.841340 redmage-0.3.1/redmage/elements.py
--rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.3.1/redmage/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.3.1/redmage/py.typed
--rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.3.1/redmage/targets.py
--rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.3.1/redmage/triggers.py
--rw-r--r--   0        0        0     1722 2023-07-11 01:12:10.164710 redmage-0.3.1/redmage/types.py
--rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.3.1/redmage/utils.py
--rw-r--r--   0        0        0    15938 1970-01-01 00:00:00.000000 redmage-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.4.2/LICENSE
+-rw-r--r--   0        0        0    15297 2023-07-22 17:27:13.140258 redmage-0.4.2/README.md
+-rw-r--r--   0        0        0      687 2023-07-22 17:27:13.149299 redmage-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-05-15 02:04:21.318232 redmage-0.4.2/redmage/__init__.py
+-rw-r--r--   0        0        0     6936 2023-07-22 17:32:00.355849 redmage-0.4.2/redmage/components.py
+-rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.4.2/redmage/convertors.py
+-rw-r--r--   0        0        0     7977 2023-07-22 17:32:27.359979 redmage-0.4.2/redmage/core.py
+-rw-r--r--   0        0        0     9364 2023-07-22 17:27:13.157467 redmage-0.4.2/redmage/elements.py
+-rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.4.2/redmage/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.4.2/redmage/py.typed
+-rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.4.2/redmage/targets.py
+-rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.4.2/redmage/triggers.py
+-rw-r--r--   0        0        0     1722 2023-07-13 21:46:22.902130 redmage-0.4.2/redmage/types.py
+-rw-r--r--   0        0        0      644 2023-07-22 17:27:13.158467 redmage-0.4.2/redmage/utils.py
+-rw-r--r--   0        0        0    15998 1970-01-01 00:00:00.000000 redmage-0.4.2/PKG-INFO
```

### Comparing `redmage-0.3.1/LICENSE` & `redmage-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redmage-0.3.1/README.md` & `redmage-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class Counter(Component, routes=("/",)):
     count: int
 
     def __init__(self):
         self.count = 0
 
-    def render(self):
+    async def render(self):
         return Div(
             H1(f"Clicked {self.count} times."),
             Button(
                 "Add 1",
                 click=self.add_one(),
             ),
             Script(src="https://unpkg.com/htmx.org@1.9.2"),
@@ -90,15 +90,15 @@
 
 
 app = Redmage()
 
 
 class Index(Component, routes=("/",)):
 
-    def render(self):
+    async def render(self):
         return Doc(
             Html(
                 Head(
                     Title("Example"),
                 ),
                 Body(
                     H1("Hello Redmage"),
@@ -176,15 +176,15 @@
 
 
 app = Redmage()
 
 
 class Index(Component, routes=("/",)):
 
-    def render(self):
+    async def render(self):
         return Doc(
             Html(
                 Head(
                     Title("Todo App"),
                 ),
                 Body(
                     ChildComponent(),
@@ -192,15 +192,15 @@
                 ),
             )
         )
 
 
 class ChildComponent(Component):
 
-    def render(self):
+    async def render(self):
         return H1("Child Component")
 
 ```
 
 > In the following examples I'm going to assume that the components we write are rendered in an **Index** component like above so it will be ommited.
 
 
@@ -225,15 +225,15 @@
 
 
 class ClickComponent(Component):
 
     def __init__(self):
         self.count = 0
 
-    def render(self):
+    async def render(self):
         return Button(
             self.count,
             target=self.set_count(self.count + 1)
         )
 
     @Target.post
     def set_count(self, count: int):
@@ -257,15 +257,15 @@
 
 
 class Message(Component):
 
     def __init__(self, content):
         self.content = content
 
-    def render(self):
+    async def render(self):
         return Div(
             P(f"{self.content=}"),
             Form(
                 Input(
                     type="text",
                     id="content",
                     name="content",
@@ -300,15 +300,15 @@
     content: str
     count: int
 
     def __init__(self, content, count):
         self.content = content
         self.count = count
 
-    def render(self):
+    async def render(self):
         return Div(
             P(f"{self.content=}"),
             Form(
                 Input(
                     type="text",
                     id="content",
                     name="content",
@@ -338,15 +338,15 @@
 Redmage provides a very thin abstraction over _hx-trigger_ attributes. An element's **trigger** keyword argument can be used to tell Redamge which event type should trigger a component update. You can just pass a string value of the [event](https://developer.mozilla.org/en-US/docs/Web/Events) name.
 
 ```
 class HoverCount(Component):
     def __init__(self):
         self.count = 0
 
-    def render(self):
+    async def render(self):
         return Div(
             self.count,
             target=self.set_count(self.count + 1),
             trigger="mouseover",
         )
 
     @Target.post
@@ -372,15 +372,15 @@
 from redmage.types import HTMXTrigger
 
 
 class HoverCount(Component):
     def __init__(self):
         self.count = 0
 
-    def render(self):
+    async def render(self):
         trigger = Trigger(HTMXTrigger.MOUSEOVER, DelayTriggerModifier(1000))
 
         return Div(
             self.count, target=self.set_count(self.count + 1), trigger=trigger
         )
 
     @Target.post
@@ -395,15 +395,15 @@
 The **Element** class has a number of keyword arguments associated with events that we can pass **Target** objects too. This can simplify our code by not having to add both target and trigger keyword arguments. Below is an example.
 
 ```
 class HoverCount(Component):
     def __init__(self):
         self.count = 0
 
-    def render(self):
+    async def render(self):
         return Div(
             self.count,
             mouse_over=self.set_count(self.count + 1),
         )
 
     @Target.post
     def set_count(self, count: int):
```

### Comparing `redmage-0.3.1/pyproject.toml` & `redmage-0.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "redmage"
-version = "0.3.1"
+version = "0.4.2"
 description = "A component based library for building htmx powered applications."
 authors = ["Scott Russell <me@scottrussell.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 starlette = "^0.26.1"
-hype-html = "^1.1.3"
+hype-html = "^2.0.3"
 python-multipart = "^0.0.6"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 pycodestyle = "^2.10.0"
 black = "^23.3.0"
 isort = "^5.12.0"
 httpx = "^0.24.0"
 jinja2 = "^3.1.2"
 mypy = "^1.2.0"
 uvicorn = "^0.22.0"
+pytest-asyncio = "^0.21.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `redmage-0.3.1/redmage/components.py` & `redmage-0.4.2/redmage/components.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,32 +4,31 @@
 from inspect import Parameter, signature
 from typing import Any, Dict, Optional
 from typing import OrderedDict as OrderedDictType
 from typing import Tuple
 from uuid import uuid1
 
 from starlette.convertors import CONVERTOR_TYPES as starlette_convertors
+from starlette.requests import Request
 from starlette.responses import HTMLResponse
 
-from .utils import group_signature_param_by_kind
+from .utils import astr, group_signature_param_by_kind
 
 logger = logging.getLogger("redmage")
 
 
 class Component(ABC):
     app: "Redmage"  # type: ignore
+    request = None  # type: ignore
     render_extensions: Dict[str, Any] = {}
 
     def __init_subclass__(cls, routes: Optional[Tuple[str]] = None, **kwargs: Any):
         super().__init_subclass__(**kwargs)
         cls.app.register_component(cls, routes=routes)
 
-    def build_response(self, content: Any) -> HTMLResponse:
-        return HTMLResponse(content)
-
     @classmethod
     def set_app(cls, app: "Redmage") -> None:  # type: ignore
         cls.app = app
 
     @classmethod
     def add_render_extension(cls, **kwargs: Any) -> None:
         for key, value in kwargs.items():
@@ -153,15 +152,15 @@
     @property
     def id(self) -> str:
         if not hasattr(self, "_id"):
             self._id = f"{self.__class__.__name__}-{str(uuid1())}"
         return self._id
 
     @abstractmethod
-    def render(self, **exts: Any) -> "Element":  # type: ignore
+    async def render(self, **exts: Any) -> "Element":  # type: ignore
         ...  # pragma: no cover
 
     def _filter_render_extensions(self) -> OrderedDictType[str, Any]:
         args = OrderedDict()
         params = signature(self.render).parameters
         for param in params.values():
             if param.name in self.render_extensions.keys():
@@ -169,12 +168,15 @@
             if param.kind == Parameter.VAR_KEYWORD:
                 args.update(self.render_extensions)
         return args
 
     def set_element_id(self, el: "Element") -> None:  # type: ignore
         el.attrs(_id=self.id)
 
-    def __str__(self) -> str:
+    def build_response(self, content: Any) -> HTMLResponse:
+        return HTMLResponse(content)
+
+    async def _astr_(self) -> str:
         render_extentions = self._filter_render_extensions()
-        el = self.render(**render_extentions)
+        el = await self.render(**render_extentions)
         self.set_element_id(el)
-        return str(el)
+        return await astr(el)
```

### Comparing `redmage-0.3.1/redmage/convertors.py` & `redmage-0.4.2/redmage/convertors.py`

 * *Files identical despite different names*

### Comparing `redmage-0.3.1/redmage/core.py` & `redmage-0.4.2/redmage/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from starlette.routing import Route
 
 from redmage.exceptions import RedmageError
 
 from .components import Component
 from .targets import Target
 from .types import HTTPMethod
+from .utils import astr
 
 logger = logging.getLogger("redmage")
 
 
 ComponentClass = Type[Component]
 
 
@@ -59,15 +60,16 @@
     ) -> None:
         self.components.append((cls, routes))
 
     def _get_explicit_route_function(self, cls: ComponentClass) -> Callable:
         async def route_function(request: Request) -> HTMLResponse:
             attrs = {**request.path_params, **request.query_params}
             instance = cls(**attrs)
-            return instance.build_response(str(instance))
+            instance.request = request  # type: ignore
+            return instance.build_response(await astr(instance))
 
         return route_function
 
     def _get_route_function(
         self, cls: ComponentClass, name: str, fn: Callable
     ) -> Callable:
         async def route_function(request: Request) -> HTMLResponse:
@@ -101,18 +103,20 @@
                 )
             else:
                 components = fn(
                     instance,
                     **{**comp_params, **comp_query_params},
                 )
             if isinstance(components, tuple):
-                return instance.build_response("\n".join([str(c) for c in components]))
+                return instance.build_response(
+                    "\n".join([await astr(c) for c in components])
+                )
             elif components:
-                return instance.build_response(str(components))
-            return instance.build_response(str(instance))
+                return instance.build_response(await astr(components))
+            return instance.build_response(await astr(instance))
 
         return route_function
 
     def _convert_value(self, key: str, value: str, fn: Callable) -> Any:
         params = signature(fn).parameters
         if key in params:
             ann = (
```

### Comparing `redmage-0.3.1/redmage/targets.py` & `redmage-0.4.2/redmage/targets.py`

 * *Files identical despite different names*

### Comparing `redmage-0.3.1/redmage/triggers.py` & `redmage-0.4.2/redmage/triggers.py`

 * *Files identical despite different names*

### Comparing `redmage-0.3.1/redmage/types.py` & `redmage-0.4.2/redmage/types.py`

 * *Files identical despite different names*

### Comparing `redmage-0.3.1/redmage/utils.py` & `redmage-0.4.2/redmage/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import inspect
 from inspect import Parameter, _ParameterKind
-from typing import Dict, List
+from typing import Any, Dict, List
 
 
 def group_signature_param_by_kind(
     sig: inspect.Signature,
 ) -> Dict[_ParameterKind, List[Parameter]]:
     # TODO fix type hints here
     # Need VAR_POSITIONAL and VAR_KEYWORD?
@@ -12,7 +12,11 @@
         Parameter.POSITIONAL_ONLY: [],
         Parameter.POSITIONAL_OR_KEYWORD: [],
         Parameter.KEYWORD_ONLY: [],
     }
     for param in sig.parameters.values():
         grouped[param.kind].append(param)
     return grouped
+
+
+async def astr(astringable: Any) -> str:
+    return await astringable._astr_()
```

### Comparing `redmage-0.3.1/PKG-INFO` & `redmage-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: redmage
-Version: 0.3.1
+Version: 0.4.2
 Summary: A component based library for building htmx powered applications.
 License: MIT
 Author: Scott Russell
 Author-email: me@scottrussell.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hype-html (>=1.1.3,<2.0.0)
+Requires-Dist: hype-html (>=2.0.3,<3.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: starlette (>=0.26.1,<0.27.0)
 Description-Content-Type: text/markdown
 
 # redmage
 
 [![run-tests](https://github.com/redmage-labs/redmage/actions/workflows/main.yaml/badge.svg)](https://github.com/redmage-labs/redmage/actions/workflows/main.yaml)
@@ -41,15 +41,15 @@
 
 class Counter(Component, routes=("/",)):
     count: int
 
     def __init__(self):
         self.count = 0
 
-    def render(self):
+    async def render(self):
         return Div(
             H1(f"Clicked {self.count} times."),
             Button(
                 "Add 1",
                 click=self.add_one(),
             ),
             Script(src="https://unpkg.com/htmx.org@1.9.2"),
@@ -109,15 +109,15 @@
 
 
 app = Redmage()
 
 
 class Index(Component, routes=("/",)):
 
-    def render(self):
+    async def render(self):
         return Doc(
             Html(
                 Head(
                     Title("Example"),
                 ),
                 Body(
                     H1("Hello Redmage"),
@@ -195,15 +195,15 @@
 
 
 app = Redmage()
 
 
 class Index(Component, routes=("/",)):
 
-    def render(self):
+    async def render(self):
         return Doc(
             Html(
                 Head(
                     Title("Todo App"),
                 ),
                 Body(
                     ChildComponent(),
@@ -211,15 +211,15 @@
                 ),
             )
         )
 
 
 class ChildComponent(Component):
 
-    def render(self):
+    async def render(self):
         return H1("Child Component")
 
 ```
 
 > In the following examples I'm going to assume that the components we write are rendered in an **Index** component like above so it will be ommited.
 
 
@@ -244,15 +244,15 @@
 
 
 class ClickComponent(Component):
 
     def __init__(self):
         self.count = 0
 
-    def render(self):
+    async def render(self):
         return Button(
             self.count,
             target=self.set_count(self.count + 1)
         )
 
     @Target.post
     def set_count(self, count: int):
@@ -276,15 +276,15 @@
 
 
 class Message(Component):
 
     def __init__(self, content):
         self.content = content
 
-    def render(self):
+    async def render(self):
         return Div(
             P(f"{self.content=}"),
             Form(
                 Input(
                     type="text",
                     id="content",
                     name="content",
@@ -319,15 +319,15 @@
     content: str
     count: int
 
     def __init__(self, content, count):
         self.content = content
         self.count = count
 
-    def render(self):
+    async def render(self):
         return Div(
             P(f"{self.content=}"),
             Form(
                 Input(
                     type="text",
                     id="content",
                     name="content",
@@ -357,15 +357,15 @@
 Redmage provides a very thin abstraction over _hx-trigger_ attributes. An element's **trigger** keyword argument can be used to tell Redamge which event type should trigger a component update. You can just pass a string value of the [event](https://developer.mozilla.org/en-US/docs/Web/Events) name.
 
 ```
 class HoverCount(Component):
     def __init__(self):
         self.count = 0
 
-    def render(self):
+    async def render(self):
         return Div(
             self.count,
             target=self.set_count(self.count + 1),
             trigger="mouseover",
         )
 
     @Target.post
@@ -391,15 +391,15 @@
 from redmage.types import HTMXTrigger
 
 
 class HoverCount(Component):
     def __init__(self):
         self.count = 0
 
-    def render(self):
+    async def render(self):
         trigger = Trigger(HTMXTrigger.MOUSEOVER, DelayTriggerModifier(1000))
 
         return Div(
             self.count, target=self.set_count(self.count + 1), trigger=trigger
         )
 
     @Target.post
@@ -414,15 +414,15 @@
 The **Element** class has a number of keyword arguments associated with events that we can pass **Target** objects too. This can simplify our code by not having to add both target and trigger keyword arguments. Below is an example.
 
 ```
 class HoverCount(Component):
     def __init__(self):
         self.count = 0
 
-    def render(self):
+    async def render(self):
         return Div(
             self.count,
             mouse_over=self.set_count(self.count + 1),
         )
 
     @Target.post
     def set_count(self, count: int):
```

