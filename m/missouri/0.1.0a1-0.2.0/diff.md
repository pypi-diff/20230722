# Comparing `tmp/missouri-0.1.0a1.tar.gz` & `tmp/missouri-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "missouri-0.1.0a1.tar", max compression
+gzip compressed data, was "missouri-0.2.0.tar", max compression
```

## Comparing `missouri-0.1.0a1.tar` & `missouri-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0       54 2023-03-25 21:50:43.355256 missouri-0.1.0a1/CHANGELOG.md
--rw-r--r--   0        0        0      640 2023-03-25 21:50:43.355970 missouri-0.1.0a1/LICENSE
--rw-r--r--   0        0        0        0 2023-03-25 21:50:43.357350 missouri-0.1.0a1/missouri/__init__.py
--rw-r--r--   0        0        0     4328 2023-03-27 16:24:53.159792 missouri-0.1.0a1/missouri/coding.py
--rw-r--r--   0        0        0      150 2023-03-25 21:50:43.358310 missouri-0.1.0a1/missouri/common_types.py
--rw-r--r--   0        0        0     1845 2023-03-27 16:24:39.133716 missouri-0.1.0a1/missouri/json.py
--rw-r--r--   0        0        0     2072 2023-03-27 16:26:06.746805 missouri-0.1.0a1/missouri/numpylib.py
--rw-r--r--   0        0        0      796 2023-03-27 22:10:36.781449 missouri-0.1.0a1/missouri/openlib.py
--rw-r--r--   0        0        0        0 2023-03-30 17:39:19.308761 missouri-0.1.0a1/missouri/py.typed
--rw-r--r--   0        0        0     1312 2023-03-30 17:40:37.254819 missouri-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 missouri-0.1.0a1/setup.py
--rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 missouri-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0      133 2023-07-22 16:24:28.536948 missouri-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      640 2023-03-30 20:36:15.928421 missouri-0.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-03-30 20:36:15.931890 missouri-0.2.0/missouri/__init__.py
+-rw-r--r--   0        0        0     4197 2023-07-22 16:24:28.537366 missouri-0.2.0/missouri/coding.py
+-rw-r--r--   0        0        0     1824 2023-07-22 16:24:28.537779 missouri-0.2.0/missouri/json.py
+-rw-r--r--   0        0        0     2094 2023-07-22 16:24:28.538132 missouri-0.2.0/missouri/numpylib.py
+-rw-r--r--   0        0        0      820 2023-07-22 16:24:28.538482 missouri-0.2.0/missouri/openlib.py
+-rw-r--r--   0        0        0        0 2023-03-30 20:36:15.935088 missouri-0.2.0/missouri/py.typed
+-rw-r--r--   0        0        0     1309 2023-07-22 16:24:28.538818 missouri-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 missouri-0.2.0/setup.py
+-rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 missouri-0.2.0/PKG-INFO
```

### Comparing `missouri-0.1.0a1/LICENSE` & `missouri-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `missouri-0.1.0a1/missouri/coding.py` & `missouri-0.2.0/missouri/coding.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Adapted from
 # https://github.com/metabolize-forks/baiji-serialization/tree/8b77f19685555e1bab03e75a433d00ce6fa4bea5
 # Apache 2.0
 
 import typing as t
-from .common_types import JsonType
 from .numpylib import decode_numpy as _decode_numpy, encode_numpy as _encode_numpy
 
 if t.TYPE_CHECKING:  # pragma: no cover
     import numpy as np
 
 
 class MethodListCaller:
@@ -24,27 +23,27 @@
             index = len(self.method_list)
         self.method_list.insert(index, method)
 
     def clear(self) -> None:
         # be defensive if someone forgets to call super pylint: disable=attribute-defined-outside-init
         self.method_list = []
 
-    def __call__(self, obj: t.Any) -> t.Optional[JsonType]:
+    def __call__(self, obj: t.Any) -> t.Any:
         """
         Call the methods in method_list until one of them returns something other than None
         and return that as the result of the call.
         """
         try:
             return next(
                 filter(lambda x: x is not None, (f(obj) for f in self.method_list))
             )
         except StopIteration:
             return self.default(obj)
 
-    def default(self, x: t.Any) -> t.Optional[JsonType]:
+    def default(self, x: t.Any) -> t.Any:
         """
         If none of the methods returned something, then return this default
         """
         return x
 
 
 class JSONEncoder(MethodListCaller):
@@ -74,25 +73,25 @@
     def __init__(self, encode_as_primitives: t.Optional[bool] = None):
         self.encode_as_primitives = (
             False if encode_as_primitives is None else encode_as_primitives
         )
         self.register(self.encode)
         self.register(self.encode_numpy)
 
-    def default(self, obj: t.Any) -> t.Optional[JsonType]:
+    def default(self, obj: t.Any) -> t.Any:
         raise ValueError(f"Object of type {type(obj)} is not JSON-serializable")
 
-    def encode(self, obj: t.Any) -> t.Optional[JsonType]:
+    def encode(self, obj: t.Any) -> t.Any:
         """
         In a subclass, either override this or add some encode functions and
         override __init__ to register them.
         """
         pass
 
-    def encode_numpy(self, obj: "np.ndarray") -> t.Optional[JsonType]:
+    def encode_numpy(self, obj: "np.ndarray") -> t.Any:
         return _encode_numpy(obj, as_primitives=self.encode_as_primitives)
 
 
 class JSONDecoder(MethodListCaller):
     """
     Instances may be passed to simplejson as object_hook to decode json objects.
     The decoders will be called in order. The first one to return something other
@@ -115,16 +114,16 @@
     MethodListCaller.
     """
 
     def __init__(self) -> None:
         self.register(self.decode)
         self.register(self.decode_numpy)
 
-    def decode(self, obj: JsonType) -> t.Optional[JsonType]:
+    def decode(self, obj: t.Any) -> t.Any:
         """
         In a subclass, either override this or add some decode functions and
         override __init__ to register them
         """
         pass
 
-    def decode_numpy(self, obj: JsonType) -> t.Optional["np.ndarray"]:
+    def decode_numpy(self, obj: t.Any) -> t.Optional["np.ndarray"]:
         return _decode_numpy(obj)
```

### Comparing `missouri-0.1.0a1/missouri/json.py` & `missouri-0.2.0/missouri/json.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # Adapted from
 # https://github.com/metabolize-forks/baiji-serialization/tree/8b77f19685555e1bab03e75a433d00ce6fa4bea5
 # Apache 2.0
 
 import typing as t
 import simplejson as json
 from .coding import JSONDecoder, JSONEncoder
-from .common_types import JsonType
-from .openlib import ensure_text_file_open
+from .openlib import FileLike, ensure_text_file_open
 
 
 def _dump_args(kwargs: dict) -> dict:
     if "default" in kwargs:
         raise ValueError(
             "Instead of explicitly setting default, subclass missouri.coding.JSONEncoder and pass it as encoder"
         )
@@ -23,15 +22,15 @@
         )
     if "encode_as_primitives" in kwargs:
         del kwargs["encode_as_primitives"]
     kwargs["for_json"] = True
     return kwargs
 
 
-def dump(obj: t.Any, path: str, *args: object, **kwargs: object) -> None:
+def dump(obj: t.Any, path: FileLike, *args: object, **kwargs: object) -> None:
     with ensure_text_file_open(path, "w") as f:
         json.dump(obj, f, *args, **_dump_args(kwargs))
 
 
 def dumps(obj: t.Any, **kwargs: object) -> str:
     return json.dumps(obj, **_dump_args(kwargs))
 
@@ -45,14 +44,14 @@
         kwargs["object_hook"] = kwargs["decoder"]
         del kwargs["decoder"]
     else:
         kwargs["object_hook"] = JSONDecoder()
     return kwargs
 
 
-def load(path: str, *args: object, **kwargs: object) -> JsonType:
+def load(path: FileLike, *args: object, **kwargs: object) -> t.Any:
     with ensure_text_file_open(path, "r") as f:
         return json.load(f, *args, **_load_args(kwargs))
 
 
-def loads(s: str, **kwargs: object) -> JsonType:
+def loads(s: str, **kwargs: object) -> t.Any:
     return json.loads(s, **_load_args(kwargs))
```

### Comparing `missouri-0.1.0a1/missouri/numpylib.py` & `missouri-0.2.0/missouri/numpylib.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import typing as t
 
-from .common_types import JsonType
-
 if t.TYPE_CHECKING:  # pragma: no cover
     try:
         import numpy as np
     except ImportError:
+        # This might generate type errors, but that is okay.
         pass
 
 
-def encode_numpy(obj: t.Any, as_primitives: bool) -> JsonType:
+def encode_numpy(obj: t.Any, as_primitives: bool) -> t.Any:
     try:
         import numpy as np
     except ImportError:
         # Clearly there won't be any numpy arrays to encode...
         return None
 
     if isinstance(obj, np.ndarray):
```

### Comparing `missouri-0.1.0a1/missouri/openlib.py` & `missouri-0.2.0/missouri/openlib.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import typing as t
 from contextlib import contextmanager
-from typing import TYPE_CHECKING
 
 
-if TYPE_CHECKING:  # pragma: no cover
+if t.TYPE_CHECKING:  # pragma: no cover
     from _typeshed import FileDescriptorOrPath
 
+FileLike = t.Union["FileDescriptorOrPath", t.IO[str]]
+
 
 @contextmanager
 def ensure_text_file_open(
     path_or_fp: t.Union["FileDescriptorOrPath", t.IO[str]], mode: t.Literal["r", "w"]
 ) -> t.Generator[t.IO[str], None, None]:
     import io
```

### Comparing `missouri-0.1.0a1/pyproject.toml` & `missouri-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "missouri"
-version = "0.1.0a1"
+version = "0.2.0"
 description = "Read and write JSON in one line"
 authors = ["Paul Melnikow <github@paulmelnikow.com>", "Body Labs, Metabolize, and other contributors"]
 license = "Apache-2.0"
 include = ["CHANGELOG.md"]
 exclude = ["*/test_*.py"]
 repository = "https://github.com/metabolize/missouri"
 classifiers = [
@@ -17,29 +17,29 @@
 
 
 [tool.poetry.dependencies]
 python = ">= 3.8, < 4"
 simplejson = ">= 3, < 4"
 
 [tool.poetry.dev-dependencies]
-black = "22.10.0"
+black = "23.3.0"
 click = "8.1.3"
-coverage = "6.5.0"
+coverage = "7.2.7"
 executor = "23.2"
 flake8 = "5.0.4"
 flake8-import-order = "0.18.2"
-mypy = "1.1.1"
+mypy = "1.4.1"
 myst-parser = "0.18.1"
-numpy = "1.23.4"
-pytest = "7.2.0"
-pytest-cov = "4.0.0"
-pytest-mock = "3.10.0"
-Sphinx = "4.3.2"
+numpy = "1.24.4"
+pytest = "7.4.0"
+pytest-cov = "4.1.0"
+pytest-mock = "3.11.1"
+Sphinx = "5.3.0"
 sphinxcontrib-apidoc = "0.3.0"
-types-simplejson = "3.18.0.1"
+types-simplejson = "3.19.0.1"
 
 [build-system]
 # Lint requires setuptools.
 requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.report]
```

### Comparing `missouri-0.1.0a1/setup.py` & `missouri-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['simplejson>=3,<4']
 
 setup_kwargs = {
     'name': 'missouri',
-    'version': '0.1.0a1',
+    'version': '0.2.0',
     'description': 'Read and write JSON in one line',
     'long_description': 'None',
     'author': 'Paul Melnikow',
     'author_email': 'github@paulmelnikow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/metabolize/missouri',
```

### Comparing `missouri-0.1.0a1/PKG-INFO` & `missouri-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: missouri
-Version: 0.1.0a1
+Version: 0.2.0
 Summary: Read and write JSON in one line
 Home-page: https://github.com/metabolize/missouri
 License: Apache-2.0
 Author: Paul Melnikow
 Author-email: github@paulmelnikow.com
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 3 - Alpha
```

