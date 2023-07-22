# Comparing `tmp/python_jsonpath-0.8.1.tar.gz` & `tmp/python_jsonpath-0.9.0.tar.gz`

## Comparing `python_jsonpath-0.8.1.tar` & `python_jsonpath-0.9.0.tar`

### file list

```diff
@@ -1,30 +1,33 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/__about__.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/__init__.py
--rw-r--r--   0        0        0    16812 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/env.py
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/exceptions.py
--rw-r--r--   0        0        0    19524 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/filter.py
--rw-r--r--   0        0        0    11063 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/lex.py
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/match.py
--rw-r--r--   0        0        0    20477 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/parse.py
--rw-r--r--   0        0        0    21596 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/patch.py
--rw-r--r--   0        0        0    13672 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/path.py
--rw-r--r--   0        0        0    12518 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/pointer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/py.typed
--rw-r--r--   0        0        0    24303 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/selectors.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/stream.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/token.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/__init__.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/arguments.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/count.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/is_instance.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/keys.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/length.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/match.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/search.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/typeof.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/jsonpath/function_extensions/value.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/LICENSE.txt
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/README.md
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 python_jsonpath-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/__about__.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/__main__.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/_data.py
+-rw-r--r--   0        0        0     9819 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/cli.py
+-rw-r--r--   0        0        0    17421 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/env.py
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/exceptions.py
+-rw-r--r--   0        0        0    19524 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/filter.py
+-rw-r--r--   0        0        0    11063 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/lex.py
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/match.py
+-rw-r--r--   0        0        0    20636 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/parse.py
+-rw-r--r--   0        0        0    21349 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/patch.py
+-rw-r--r--   0        0        0    13676 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/path.py
+-rw-r--r--   0        0        0    22229 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/pointer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/py.typed
+-rw-r--r--   0        0        0    26458 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/selectors.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/stream.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/token.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/function_extensions/__init__.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/function_extensions/arguments.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/function_extensions/count.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/function_extensions/is_instance.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/function_extensions/keys.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/function_extensions/length.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/function_extensions/match.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/function_extensions/search.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/function_extensions/typeof.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/jsonpath/function_extensions/value.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/README.md
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 python_jsonpath-0.9.0/PKG-INFO
```

### Comparing `python_jsonpath-0.8.1/jsonpath/__init__.py` & `python_jsonpath-0.9.0/jsonpath/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,22 +9,26 @@
 from .exceptions import JSONPathSyntaxError
 from .exceptions import JSONPathTypeError
 from .exceptions import JSONPointerError
 from .exceptions import JSONPointerIndexError
 from .exceptions import JSONPointerKeyError
 from .exceptions import JSONPointerResolutionError
 from .exceptions import JSONPointerTypeError
+from .exceptions import RelativeJSONPointerError
+from .exceptions import RelativeJSONPointerIndexError
+from .exceptions import RelativeJSONPointerSyntaxError
 from .filter import UNDEFINED
 from .lex import Lexer
 from .match import JSONPathMatch
 from .parse import Parser
 from .patch import JSONPatch
 from .path import CompoundJSONPath
 from .path import JSONPath
 from .pointer import JSONPointer
+from .pointer import RelativeJSONPointer
 from .pointer import resolve
 
 __all__ = (
     "compile",
     "CompoundJSONPath",
     "findall_async",
     "findall",
@@ -44,14 +48,18 @@
     "JSONPointerIndexError",
     "JSONPointerKeyError",
     "JSONPointerResolutionError",
     "JSONPointerTypeError",
     "Lexer",
     "match",
     "Parser",
+    "RelativeJSONPointer",
+    "RelativeJSONPointerError",
+    "RelativeJSONPointerIndexError",
+    "RelativeJSONPointerSyntaxError",
     "resolve",
     "UNDEFINED",
 )
 
 
 # For convenience
 DEFAULT_ENV = JSONPathEnvironment()
```

### Comparing `python_jsonpath-0.8.1/jsonpath/env.py` & `python_jsonpath-0.9.0/jsonpath/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,16 +66,18 @@
       `setup_function_extensions()`
     - Hook in to mapping and sequence item getting by overriding `getitem()`.
     - Change filter comparison operator behavior by overriding `compare()`.
 
     ## Class attributes
 
     Arguments:
-        filter_caching (bool): If `True`, filter expressions will be cached where
-            possible.
+        filter_caching (bool): If `True`, filter expressions will be cached
+            where possible.
+        unicode_escape: If `True`, decode UTF-16 escape sequences found in
+            JSONPath string literals.
 
     Attributes:
         filter_context_token (str): The pattern used to select extra filter context
             data. Defaults to `"_"`.
         intersection_token (str): The pattern used as the intersection operator.
             Defaults to `"&"`.
         key_token (str): The pattern used to identify the current key or index when
@@ -109,16 +111,26 @@
     min_int_index = -(2**53) + 1
 
     # Override these to customize path tokenization and parsing.
     lexer_class: Type[Lexer] = Lexer
     parser_class: Type[Parser] = Parser
     match_class: Type[JSONPathMatch] = JSONPathMatch
 
-    def __init__(self, *, filter_caching: bool = True) -> None:
-        self.filter_caching = filter_caching
+    def __init__(
+        self,
+        *,
+        filter_caching: bool = True,
+        unicode_escape: bool = True,
+    ) -> None:
+        self.filter_caching: bool = filter_caching
+        """Enable or disable filter expression caching."""
+
+        self.unicode_escape: bool = unicode_escape
+        """Enable or disable decoding of UTF-16 escape sequences found in
+        JSONPath string literals."""
 
         self.lexer: Lexer = self.lexer_class(env=self)
         """The lexer bound to this environment."""
 
         self.parser: Parser = self.parser_class(env=self)
         """The parser bound to this environment."""
 
@@ -133,14 +145,19 @@
         Arguments:
             path: A JSONPath as a string.
 
         Returns:
             A `JSONPath` or `CompoundJSONPath`, ready to match against some data.
                 Expect a `CompoundJSONPath` if the path string uses the _union_ or
                 _intersection_ operators.
+
+        Raises:
+            JSONPathSyntaxError: If _path_ is invalid.
+            JSONPathTypeError: If filter functions are given arguments of an
+                unacceptable type.
         """
         tokens = self.lexer.tokenize(path)
         stream = TokenStream(tokens)
         _path: Union[JSONPath, CompoundJSONPath] = JSONPath(
             env=self, selectors=self.parser.parse(stream)
         )
 
@@ -152,23 +169,23 @@
                     raise JSONPathSyntaxError(
                         f"expected a path after {stream.current.value!r}",
                         token=stream.current,
                     )
 
                 if stream.current.kind == TOKEN_UNION:
                     stream.next_token()
-                    _path.union(
+                    _path = _path.union(
                         JSONPath(
                             env=self,
                             selectors=self.parser.parse(stream),
                         )
                     )
                 elif stream.current.kind == TOKEN_INTERSECTION:
                     stream.next_token()
-                    _path.intersection(
+                    _path = _path.intersection(
                         JSONPath(
                             env=self,
                             selectors=self.parser.parse(stream),
                         )
                     )
                 else:  # pragma: no cover
                     # Parser.parse catches this too
```

### Comparing `python_jsonpath-0.8.1/jsonpath/exceptions.py` & `python_jsonpath-0.9.0/jsonpath/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -87,22 +87,56 @@
 class JSONPointerResolutionError(JSONPointerError):
     """Base exception for those that can be raised during pointer resolution."""
 
 
 class JSONPointerIndexError(JSONPointerResolutionError, IndexError):
     """An exception raised when an array index is out of range."""
 
+    def __str__(self) -> str:
+        return f"pointer index error {super().__str__()}"
+
 
 class JSONPointerKeyError(JSONPointerResolutionError, KeyError):
     """An exception raised when a pointer references a mapping with a missing key."""
 
+    def __str__(self) -> str:
+        return f"pointer key error {super().__str__()}"
+
 
 class JSONPointerTypeError(JSONPointerResolutionError, TypeError):
     """An exception raised when a pointer resolves a string against a sequence."""
 
+    def __str__(self) -> str:
+        return f"pointer type error {super().__str__()}"
+
+
+class RelativeJSONPointerError(Exception):
+    """Base class for all Relative JSON Pointer errors."""
+
+
+class RelativeJSONPointerIndexError(RelativeJSONPointerError):
+    """An exception raised when modifying a pointer index out of range."""
+
+
+class RelativeJSONPointerSyntaxError(RelativeJSONPointerError):
+    """An exception raised when we fail to parse a relative JSON Pointer."""
+
+    def __init__(self, msg: str, rel: str) -> None:
+        super().__init__(msg)
+        self.rel = rel
+
+    def __str__(self) -> str:
+        if not self.rel:
+            return super().__str__()
+
+        msg = self.rel[:7]
+        if len(msg) == 6:  # noqa: PLR2004
+            msg += ".."
+        return f"{super().__str__()} {msg!r}"
+
 
 class JSONPatchError(Exception):
     """Base class for all JSON Patch errors."""
 
 
 class JSONPatchTestFailure(JSONPatchError):  # noqa: N818
     """An exception raised when a JSON Patch _test_ op fails."""
```

### Comparing `python_jsonpath-0.8.1/jsonpath/filter.py` & `python_jsonpath-0.9.0/jsonpath/filter.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.1/jsonpath/lex.py` & `python_jsonpath-0.9.0/jsonpath/lex.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.1/jsonpath/match.py` & `python_jsonpath-0.9.0/jsonpath/match.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.1/jsonpath/parse.py` & `python_jsonpath-0.9.0/jsonpath/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -343,15 +343,15 @@
             env=self.env,
             token=start_token,
             start=start,
             stop=stop,
             step=step,
         )
 
-    def parse_selector_list(self, stream: TokenStream) -> ListSelector:
+    def parse_selector_list(self, stream: TokenStream) -> ListSelector:  # noqa: PLR0912
         """Parse a comma separated list JSONPath selectors from a stream of tokens."""
         tok = stream.next_token()
         list_items: List[
             Union[
                 IndexSelector,
                 KeysSelector,
                 PropertySelector,
@@ -387,21 +387,24 @@
             elif stream.current.kind == TOKEN_STRING:
                 if self.RE_INVALID_NAME_SELECTOR.search(stream.current.value):
                     raise JSONPathSyntaxError(
                         f"invalid name selector {stream.current.value!r}",
                         token=stream.current,
                     )
 
-                name = (
-                    codecs.decode(
-                        stream.current.value.replace("\\/", "/"), "unicode-escape"
+                if self.env.unicode_escape:
+                    name = (
+                        codecs.decode(
+                            stream.current.value.replace("\\/", "/"), "unicode-escape"
+                        )
+                        .encode("utf-16", "surrogatepass")
+                        .decode("utf-16")
                     )
-                    .encode("utf-16", "surrogatepass")
-                    .decode("utf-16")
-                )
+                else:
+                    name = stream.current.value
 
                 list_items.append(
                     PropertySelector(
                         env=self.env,
                         token=stream.current,
                         name=name,
                     ),
```

### Comparing `python_jsonpath-0.8.1/jsonpath/patch.py` & `python_jsonpath-0.9.0/jsonpath/patch.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 from typing import List
 from typing import Mapping
 from typing import MutableMapping
 from typing import MutableSequence
 from typing import TypeVar
 from typing import Union
 
-from .exceptions import JSONPatchError
-from .exceptions import JSONPatchTestFailure
-from .exceptions import JSONPointerError
-from .exceptions import JSONPointerIndexError
-from .exceptions import JSONPointerKeyError
-from .exceptions import JSONPointerTypeError
-from .pointer import UNDEFINED
-from .pointer import JSONPointer
+from jsonpath._data import load_data
+from jsonpath.exceptions import JSONPatchError
+from jsonpath.exceptions import JSONPatchTestFailure
+from jsonpath.exceptions import JSONPointerError
+from jsonpath.exceptions import JSONPointerIndexError
+from jsonpath.exceptions import JSONPointerKeyError
+from jsonpath.exceptions import JSONPointerTypeError
+from jsonpath.pointer import UNDEFINED
+from jsonpath.pointer import JSONPointer
 
 
 class Op(ABC):
     """One of the JSON Patch operations."""
 
     name = "base"
 
@@ -378,17 +379,20 @@
         if not isinstance(pointer, str):
             raise JSONPatchError(
                 f"expected a JSON Pointer string for {key!r}, "
                 f"found {pointer.__class__.__name__!r} "
                 f"({op}:{i})"
             )
 
-        return JSONPointer(
-            pointer, unicode_escape=self.unicode_escape, uri_decode=self.uri_decode
-        )
+        try:
+            return JSONPointer(
+                pointer, unicode_escape=self.unicode_escape, uri_decode=self.uri_decode
+            )
+        except JSONPointerError as err:
+            raise JSONPatchError(f"{err} ({op}:{i})") from err
 
     def _op_value(
         self, operation: Mapping[str, object], key: str, op: str, i: int
     ) -> object:
         try:
             return operation[key]
         except KeyError as err:
@@ -506,15 +510,15 @@
         pointer = self._ensure_pointer(path)
         self.ops.append(OpTest(path=pointer, value=value))
         return self
 
     def apply(
         self,
         data: Union[str, IOBase, MutableSequence[object], MutableMapping[str, object]],
-    ) -> Union[MutableSequence[object], MutableMapping[str, object]]:
+    ) -> object:
         """Apply all operations from this patch to _data_.
 
         If _data_ is a string or file-like object, it will be loaded with
         _json.loads_. Otherwise _data_ should be a JSON-like data structure and
         will be modified in place.
 
         When modifying _data_ in place, we return modified data too. This is
@@ -528,40 +532,27 @@
             Modified input data.
 
         Raises:
             JSONPatchError: When a patch operation fails.
             JSONPatchTestFailure: When a _test_ operation does not pass.
                 `JSONPatchTestFailure` is a subclass of `JSONPatchError`.
         """
-        if isinstance(data, str):
-            _data: Union[
-                MutableSequence[object], MutableMapping[str, object]
-            ] = json.loads(data)
-        elif isinstance(data, IOBase):
-            _data = json.loads(data.read())
-        else:
-            _data = data
+        _data = load_data(data)
 
         for i, op in enumerate(self.ops):
             try:
                 _data = op.apply(_data)
             except JSONPatchTestFailure as err:
                 raise JSONPatchTestFailure(f"test failed ({op.name}:{i})") from err
             except JSONPointerKeyError as err:
-                raise JSONPatchError(
-                    f"pointer key error {err} ({op.name}:{i})"
-                ) from err
+                raise JSONPatchError(f"{err} ({op.name}:{i})") from err
             except JSONPointerIndexError as err:
-                raise JSONPatchError(
-                    f"pointer index error {err} ({op.name}:{i})"
-                ) from err
+                raise JSONPatchError(f"{err} ({op.name}:{i})") from err
             except JSONPointerTypeError as err:
-                raise JSONPatchError(
-                    f"pointer type error {err} ({op.name}:{i})"
-                ) from err
+                raise JSONPatchError(f"{err} ({op.name}:{i})") from err
             except (JSONPointerError, JSONPatchError) as err:
                 raise JSONPatchError(f"{err} ({op.name}:{i})") from err
         return _data
 
     def asdicts(self) -> List[Dict[str, object]]:
         """Return a list of this patch's operations as dictionaries."""
         return [op.asdict() for op in self.ops]
```

### Comparing `python_jsonpath-0.8.1/jsonpath/path.py` & `python_jsonpath-0.9.0/jsonpath/path.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # noqa: D100
 from __future__ import annotations
 
 import itertools
-import json
-from io import IOBase
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import AsyncIterable
 from typing import Iterable
 from typing import List
 from typing import Mapping
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import TypeVar
 from typing import Union
 
-from .match import FilterContextVars
-from .match import JSONPathMatch
+from jsonpath._data import load_data
+from jsonpath.match import FilterContextVars
+from jsonpath.match import JSONPathMatch
 
 if TYPE_CHECKING:
+    from io import IOBase
+
     from .env import JSONPathEnvironment
     from .selectors import JSONPathSelector
 
 
 class JSONPath:
     """A compiled JSONPath ready to be applied to a JSON string or Python object.
 
@@ -49,14 +50,20 @@
         self.selectors = tuple(selectors)
 
     def __str__(self) -> str:
         return self.env.root_token + "".join(
             str(selector) for selector in self.selectors
         )
 
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, JSONPath) and self.selectors == __value.selectors
+
+    def __hash__(self) -> int:
+        return hash(self.selectors)
+
     def findall(
         self,
         data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
         *,
         filter_context: Optional[FilterContextVars] = None,
     ) -> List[object]:
         """Find all objects in `data` matching the given JSONPath `path`.
@@ -75,22 +82,16 @@
             be empty.
 
         Raises:
             JSONPathSyntaxError: If the path is invalid.
             JSONPathTypeError: If a filter expression attempts to use types in
                 an incompatible way.
         """
-        if isinstance(data, str):
-            _data = json.loads(data)
-        elif isinstance(data, IOBase):
-            _data = json.loads(data.read())
-        else:
-            _data = data
         return [
-            match.obj for match in self.finditer(_data, filter_context=filter_context)
+            match.obj for match in self.finditer(data, filter_context=filter_context)
         ]
 
     def finditer(
         self,
         data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
         *,
         filter_context: Optional[FilterContextVars] = None,
@@ -110,21 +111,15 @@
             An iterator yielding `JSONPathMatch` objects for each match.
 
         Raises:
             JSONPathSyntaxError: If the path is invalid.
             JSONPathTypeError: If a filter expression attempts to use types in
                 an incompatible way.
         """
-        if isinstance(data, str):
-            _data = json.loads(data)
-        elif isinstance(data, IOBase):
-            _data = json.loads(data.read())
-        else:
-            _data = data
-
+        _data = load_data(data)
         matches: Iterable[JSONPathMatch] = [
             JSONPathMatch(
                 filter_context=filter_context or {},
                 obj=_data,
                 parent=None,
                 path=self.env.root_token,
                 parts=(),
@@ -140,40 +135,29 @@
     async def findall_async(
         self,
         data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
         *,
         filter_context: Optional[FilterContextVars] = None,
     ) -> List[object]:
         """An async version of `findall()`."""
-        if isinstance(data, str):
-            _data = json.loads(data)
-        elif isinstance(data, IOBase):
-            _data = json.loads(data.read())
-        else:
-            _data = data
         return [
             match.obj
             async for match in await self.finditer_async(
-                _data, filter_context=filter_context
+                data, filter_context=filter_context
             )
         ]
 
     async def finditer_async(
         self,
         data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
         *,
         filter_context: Optional[FilterContextVars] = None,
     ) -> AsyncIterable[JSONPathMatch]:
         """An async version of `finditer()`."""
-        if isinstance(data, str):
-            _data = json.loads(data)
-        elif isinstance(data, IOBase):
-            _data = json.loads(data.read())
-        else:
-            _data = data
+        _data = load_data(data)
 
         async def root_iter() -> AsyncIterable[JSONPathMatch]:
             yield self.env.match_class(
                 filter_context=filter_context or {},
                 obj=_data,
                 parent=None,
                 path=self.env.root_token,
@@ -229,26 +213,37 @@
     __slots__ = ("env", "path", "paths")
 
     def __init__(
         self,
         *,
         env: JSONPathEnvironment,
         path: Union[JSONPath, CompoundJSONPath],
+        paths: Iterable[Tuple[str, JSONPath]] = (),
     ) -> None:
         self.env = env
         self.path = path
-        self.paths: List[Tuple[(str, JSONPath)]] = []
+        self.paths = tuple(paths)
 
     def __str__(self) -> str:
         buf: List[str] = [str(self.path)]
         for op, path in self.paths:
             buf.append(f" {op} ")
             buf.append(str(path))
         return "".join(buf)
 
+    def __eq__(self, __value: object) -> bool:
+        return (
+            isinstance(__value, CompoundJSONPath)
+            and self.path == __value.path
+            and self.paths == __value.paths
+        )
+
+    def __hash__(self) -> int:
+        return hash((self.path, self.paths))
+
     def findall(
         self,
         data: Union[str, IOBase, Sequence[Any], Mapping[str, Any]],
         *,
         filter_context: Optional[FilterContextVars] = None,
     ) -> List[object]:
         """Find all objects in `data` matching the given JSONPath `path`.
@@ -387,22 +382,28 @@
                 assert op == self.env.intersection_token
                 _objs = [match.obj async for match in _matches]
                 matches = (match async for match in matches if match.obj in _objs)
 
         return matches
 
     def union(self, path: JSONPath) -> CompoundJSONPath:
-        """In-place union of this path and another path."""
-        self.paths.append((self.env.union_token, path))
-        return self
+        """Union of this path and another path."""
+        return self.__class__(
+            env=self.env,
+            path=self.path,
+            paths=self.paths + ((self.env.union_token, path),),
+        )
 
     def intersection(self, path: JSONPath) -> CompoundJSONPath:
-        """In-place intersection of this path and another path."""
-        self.paths.append((self.env.intersection_token, path))
-        return self
+        """Intersection of this path and another path."""
+        return self.__class__(
+            env=self.env,
+            path=self.path,
+            paths=self.paths + ((self.env.intersection_token, path),),
+        )
 
 
 T = TypeVar("T")
 
 
 async def _achain(*iterables: AsyncIterable[T]) -> AsyncIterable[T]:
     for it in iterables:
```

### Comparing `python_jsonpath-0.8.1/jsonpath/selectors.py` & `python_jsonpath-0.9.0/jsonpath/selectors.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,24 @@
     ) -> None:
         super().__init__(env=env, token=token)
         self.name = name
 
     def __str__(self) -> str:
         return f"['{self.name}']"
 
+    def __eq__(self, __value: object) -> bool:
+        return (
+            isinstance(__value, PropertySelector)
+            and self.name == __value.name
+            and self.token == __value.token
+        )
+
+    def __hash__(self) -> int:
+        return hash((self.name, self.token))
+
     def resolve(self, matches: Iterable[JSONPathMatch]) -> Iterable[JSONPathMatch]:
         for match in matches:
             if not isinstance(match.obj, Mapping):
                 continue
 
             with suppress(KeyError):
                 _match = self.env.match_class(
@@ -120,14 +130,24 @@
         super().__init__(env=env, token=token)
         self.index = index
         self._as_key = str(self.index)
 
     def __str__(self) -> str:
         return f"[{self.index}]"
 
+    def __eq__(self, __value: object) -> bool:
+        return (
+            isinstance(__value, IndexSelector)
+            and self.index == __value.index
+            and self.token == __value.token
+        )
+
+    def __hash__(self) -> int:
+        return hash((self.index, self.token))
+
     def _normalized_index(self, obj: Sequence[object]) -> int:
         if self.index < 0 and len(obj) >= abs(self.index):
             return len(obj) + self.index
         return self.index
 
     def resolve(self, matches: Iterable[JSONPathMatch]) -> Iterable[JSONPathMatch]:
         for match in matches:
@@ -140,15 +160,15 @@
                         parent=match,
                         parts=match.parts + (self._as_key,),
                         path=f"{match.path}['{self.index}']",
                         root=match.root,
                     )
                     match.add_child(_match)
                     yield _match
-            elif isinstance(match.obj, Sequence):
+            elif isinstance(match.obj, Sequence) and not isinstance(match.obj, str):
                 norm_index = self._normalized_index(match.obj)
                 with suppress(IndexError):
                     _match = self.env.match_class(
                         filter_context=match.filter_context(),
                         obj=self.env.getitem(match.obj, self.index),
                         parent=match,
                         parts=match.parts + (norm_index,),
@@ -171,15 +191,15 @@
                         parent=match,
                         parts=match.parts + (self._as_key,),
                         path=f"{match.path}['{self.index}']",
                         root=match.root,
                     )
                     match.add_child(_match)
                     yield _match
-            elif isinstance(match.obj, Sequence):
+            elif isinstance(match.obj, Sequence) and not isinstance(match.obj, str):
                 norm_index = self._normalized_index(match.obj)
                 with suppress(IndexError):
                     _match = self.env.match_class(
                         filter_context=match.filter_context(),
                         obj=await self.env.getitem_async(match.obj, self.index),
                         parent=match,
                         parts=match.parts + (norm_index,),
@@ -194,14 +214,20 @@
     """Select an mapping's keys/properties."""
 
     __slots__ = ()
 
     def __str__(self) -> str:
         return f"[{self.env.keys_selector_token}]"
 
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, KeysSelector) and self.token == __value.token
+
+    def __hash__(self) -> int:
+        return hash(self.token)
+
     def _keys(self, match: JSONPathMatch) -> Iterable[JSONPathMatch]:
         if isinstance(match.obj, Mapping):
             for i, key in enumerate(match.obj.keys()):
                 _match = self.env.match_class(
                     filter_context=match.filter_context(),
                     obj=key,
                     parent=match,
@@ -244,14 +270,24 @@
 
     def __str__(self) -> str:
         stop = self.slice.stop if self.slice.stop is not None else ""
         start = self.slice.start if self.slice.start is not None else ""
         step = self.slice.step if self.slice.step is not None else "1"
         return f"[{start}:{stop}:{step}]"
 
+    def __eq__(self, __value: object) -> bool:
+        return (
+            isinstance(__value, SliceSelector)
+            and self.slice == __value.slice
+            and self.token == __value.token
+        )
+
+    def __hash__(self) -> int:
+        return hash((str(self), self.token))
+
     def _check_range(self, *indices: Optional[int]) -> None:
         for i in indices:
             if i is not None and (
                 i < self.env.min_int_index or i > self.env.max_int_index
             ):
                 raise JSONPathIndexError("index out of range", token=self.token)
 
@@ -307,14 +343,20 @@
 
 class WildSelector(JSONPathSelector):
     """Wildcard expansion selector."""
 
     def __str__(self) -> str:
         return "[*]"
 
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, WildSelector) and self.token == __value.token
+
+    def __hash__(self) -> int:
+        return hash(self.token)
+
     def resolve(self, matches: Iterable[JSONPathMatch]) -> Iterable[JSONPathMatch]:
         for match in matches:
             if isinstance(match.obj, str):
                 continue
             if isinstance(match.obj, Mapping):
                 for key, val in match.obj.items():
                     _match = self.env.match_class(
@@ -372,14 +414,23 @@
 
 class RecursiveDescentSelector(JSONPathSelector):
     """A JSONPath selector that visits all objects recursively."""
 
     def __str__(self) -> str:
         return ".."
 
+    def __eq__(self, __value: object) -> bool:
+        return (
+            isinstance(__value, RecursiveDescentSelector)
+            and self.token == __value.token
+        )
+
+    def __hash__(self) -> int:
+        return hash(self.token)
+
     def _expand(self, match: JSONPathMatch) -> Iterable[JSONPathMatch]:
         if isinstance(match.obj, Mapping):
             for key, val in match.obj.items():
                 if isinstance(val, str):
                     pass
                 elif isinstance(val, (Mapping, Sequence)):
                     _match = self.env.match_class(
@@ -449,15 +500,15 @@
                 IndexSelector,
                 PropertySelector,
                 WildSelector,
             ]
         ],
     ) -> None:
         super().__init__(env=env, token=token)
-        self.items = items
+        self.items = tuple(items)
 
     def __str__(self) -> str:
         buf: List[str] = []
         for item in self.items:
             if isinstance(item, SliceSelector):
                 stop = item.slice.stop if item.slice.stop is not None else ""
                 start = item.slice.start if item.slice.start is not None else ""
@@ -469,14 +520,24 @@
                 buf.append("*")
             elif isinstance(item, KeysSelector):
                 buf.append(self.env.keys_selector_token)
             else:
                 buf.append(str(item.index))
         return f"[{', '.join(buf)}]"
 
+    def __eq__(self, __value: object) -> bool:
+        return (
+            isinstance(__value, ListSelector)
+            and self.items == __value.items
+            and self.token == __value.token
+        )
+
+    def __hash__(self) -> int:
+        return hash((self.items, self.token))
+
     def resolve(self, matches: Iterable[JSONPathMatch]) -> Iterable[JSONPathMatch]:
         _matches = list(matches)
         for item in self.items:
             yield from item.resolve(_matches)
 
     async def resolve_async(
         self, matches: AsyncIterable[JSONPathMatch]
@@ -503,14 +564,24 @@
         self.expression = expression
         # Compile-time check for cacheable nodes.
         self.cacheable_nodes = self.expression.cacheable_nodes()
 
     def __str__(self) -> str:
         return f"[?({self.expression})]"
 
+    def __eq__(self, __value: object) -> bool:
+        return (
+            isinstance(__value, Filter)
+            and self.expression == __value.expression
+            and self.token == __value.token
+        )
+
+    def __hash__(self) -> int:
+        return hash((str(self.expression), self.token))
+
     def resolve(  # noqa: PLR0912
         self, matches: Iterable[JSONPathMatch]
     ) -> Iterable[JSONPathMatch]:
         if self.cacheable_nodes and self.env.filter_caching:
             expr = self.expression.cache_tree()
         else:
             expr = self.expression
```

### Comparing `python_jsonpath-0.8.1/jsonpath/stream.py` & `python_jsonpath-0.9.0/jsonpath/stream.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.1/jsonpath/token.py` & `python_jsonpath-0.9.0/jsonpath/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,12 +114,15 @@
             isinstance(other, Token)
             and self.kind == other.kind
             and self.value == other.value
             and self.index == other.index
             and self.path == other.path
         )
 
+    def __hash__(self) -> int:
+        return hash((self.kind, self.value, self.index, self.path))
+
     def position(self) -> Tuple[int, int]:
         """Return the line and column number for the start of this token."""
         line_number = self.value.count("\n", 0, self.index) + 1
         column_number = self.index - self.value.rfind("\n", 0, self.index)
-        return (line_number, column_number)
+        return (line_number, column_number - 1)
```

### Comparing `python_jsonpath-0.8.1/jsonpath/function_extensions/arguments.py` & `python_jsonpath-0.9.0/jsonpath/function_extensions/arguments.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import inspect
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Callable
 from typing import List
 
 if TYPE_CHECKING:
-    from ..env import JSONPathEnvironment
-    from ..token import Token
+    from jsonpath.env import JSONPathEnvironment
+    from jsonpath.token import Token
 
-from ..exceptions import JSONPathTypeError
+from jsonpath.exceptions import JSONPathTypeError
 
 
 def validate(
     _: "JSONPathEnvironment",
     func: Callable[..., Any],
     args: List[Any],
     token: "Token",
```

### Comparing `python_jsonpath-0.8.1/jsonpath/function_extensions/count.py` & `python_jsonpath-0.9.0/jsonpath/function_extensions/count.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """The standard `count` function extension."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from typing import List
 
-from ..exceptions import JSONPathTypeError
-from ..filter import Literal
-from ..filter import Nil
+from jsonpath.exceptions import JSONPathTypeError
+from jsonpath.filter import Literal
+from jsonpath.filter import Nil
 
 if TYPE_CHECKING:
-    from ..env import JSONPathEnvironment
-    from ..match import NodeList
-    from ..token import Token
+    from jsonpath.env import JSONPathEnvironment
+    from jsonpath.match import NodeList
+    from jsonpath.token import Token
 
 
 class Count:
     """The built-in `count` function."""
 
     with_node_lists = True
```

### Comparing `python_jsonpath-0.8.1/jsonpath/function_extensions/is_instance.py` & `python_jsonpath-0.9.0/jsonpath/function_extensions/is_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """A non-standard "isinstance" filter function."""
 
 from typing import Mapping
 from typing import Sequence
 
-from ..filter import UNDEFINED
-from ..filter import UNDEFINED_LITERAL
+from jsonpath.filter import UNDEFINED
+from jsonpath.filter import UNDEFINED_LITERAL
 
 
 class IsInstance:
     """A non-standard "isinstance" filter function."""
 
     def __call__(self, obj: object, t: str) -> bool:  # noqa: PLR0911
         """Return `True` if the type of _obj_ matches _t_.
```

### Comparing `python_jsonpath-0.8.1/jsonpath/function_extensions/match.py` & `python_jsonpath-0.9.0/jsonpath/function_extensions/search.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-"""The standard `match` function extension."""
+"""The standard `search` function extension."""
 
 import re
 from typing import TYPE_CHECKING
 from typing import List
 from typing import Pattern
 from typing import Union
 
-from ..exceptions import JSONPathTypeError
-from ..filter import RegexArgument
-from ..filter import StringLiteral
+from jsonpath.exceptions import JSONPathTypeError
+from jsonpath.filter import RegexArgument
+from jsonpath.filter import StringLiteral
 
 if TYPE_CHECKING:
-    from ..env import JSONPathEnvironment
-    from ..token import Token
+    from jsonpath.env import JSONPathEnvironment
+    from jsonpath.token import Token
 
 
-class Match:
-    """The built-in `match` function.
+class Search:
+    """The built-in `search` function.
 
     This implementation uses the standard _re_ module, without attempting to map
     I-Regexps to Python regex.
     """
 
     def __call__(self, string: str, pattern: Union[str, Pattern[str], None]) -> bool:
-        """Return `True` if _pattern_ matches the given string, `False` otherwise."""
+        """Return `True` if the given string contains _pattern_, `False` otherwise."""
         # The IETF JSONPath draft requires us to return `False` if the pattern was
         # invalid. We use `None` to indicate the pattern could not be compiled.
         if string is None or pattern is None:
             return False
 
         try:
-            return bool(re.fullmatch(pattern, string))
+            return bool(re.search(pattern, string))
         except (TypeError, re.error):
             return False
 
     def validate(
         self,
         _: "JSONPathEnvironment",
         args: List[object],
```

### Comparing `python_jsonpath-0.8.1/jsonpath/function_extensions/search.py` & `python_jsonpath-0.9.0/jsonpath/function_extensions/match.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-"""The standard `search` function extension."""
+"""The standard `match` function extension."""
 
 import re
 from typing import TYPE_CHECKING
 from typing import List
 from typing import Pattern
 from typing import Union
 
-from ..exceptions import JSONPathTypeError
-from ..filter import RegexArgument
-from ..filter import StringLiteral
+from jsonpath.exceptions import JSONPathTypeError
+from jsonpath.filter import RegexArgument
+from jsonpath.filter import StringLiteral
 
 if TYPE_CHECKING:
-    from ..env import JSONPathEnvironment
-    from ..token import Token
+    from jsonpath.env import JSONPathEnvironment
+    from jsonpath.token import Token
 
 
-class Search:
-    """The built-in `search` function.
+class Match:
+    """The built-in `match` function.
 
     This implementation uses the standard _re_ module, without attempting to map
     I-Regexps to Python regex.
     """
 
     def __call__(self, string: str, pattern: Union[str, Pattern[str], None]) -> bool:
-        """Return `True` if the given string contains _pattern_, `False` otherwise."""
+        """Return `True` if _pattern_ matches the given string, `False` otherwise."""
         # The IETF JSONPath draft requires us to return `False` if the pattern was
         # invalid. We use `None` to indicate the pattern could not be compiled.
         if string is None or pattern is None:
             return False
 
         try:
-            return bool(re.search(pattern, string))
+            return bool(re.fullmatch(pattern, string))
         except (TypeError, re.error):
             return False
 
     def validate(
         self,
         _: "JSONPathEnvironment",
         args: List[object],
```

### Comparing `python_jsonpath-0.8.1/jsonpath/function_extensions/typeof.py` & `python_jsonpath-0.9.0/jsonpath/function_extensions/typeof.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """A non-standard "typeof" filter function."""
 
 from typing import Mapping
 from typing import Sequence
 
-from ..filter import UNDEFINED
-from ..filter import UNDEFINED_LITERAL
+from jsonpath.filter import UNDEFINED
+from jsonpath.filter import UNDEFINED_LITERAL
 
 
 class TypeOf:
     """A non-standard "typeof" filter function.
 
     Arguments:
         single_number_type: If True, will return "number" for ints and floats,
```

### Comparing `python_jsonpath-0.8.1/.gitignore` & `python_jsonpath-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.1/LICENSE.txt` & `python_jsonpath-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.8.1/pyproject.toml` & `python_jsonpath-0.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python-jsonpath"
-description = 'Another JSONPath implementation for Python.'
+description = 'JSONPath, JSON Pointer and JSON Patch for Python.'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [{ name = "James Prior", email = "jamesgr.prior@gmail.com" }]
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -30,14 +30,17 @@
 Documentation = "https://jg-rp.github.io/python-jsonpath/"
 Issues = "https://github.com/jg-rp/python-jsonpath/issues"
 Source = "https://github.com/jg-rp/python-jsonpath"
 
 [tool.hatch.version]
 path = "jsonpath/__about__.py"
 
+[project.scripts]
+json = "jsonpath.cli:main"
+
 [tool.hatch.build.targets.sdist]
 include = ["/jsonpath"]
 
 [tool.hatch.build.targets.wheel]
 include = ["/jsonpath"]
 
 [tool.hatch.envs.default]
@@ -123,17 +126,18 @@
   "RSE",
   "S",
   "SIM",
   "SLF",
   "T10",
   "T20",
   "TCH",
+  "TID",
   "YTT",
 ]
-ignore = ["S105", "S101", "D107", "D105", "PLR0913"]
+ignore = ["S105", "S101", "D107", "D105", "PLR0913", "SIM108"]
 
 fixable = ["I"]
 unfixable = []
 
 # Exclude a variety of commonly ignored directories.
 exclude = [
   ".bzr",
```

### Comparing `python_jsonpath-0.8.1/PKG-INFO` & `python_jsonpath-0.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: python-jsonpath
-Version: 0.8.1
-Summary: Another JSONPath implementation for Python.
+Version: 0.9.0
+Summary: JSONPath, JSON Pointer and JSON Patch for Python.
 Project-URL: Documentation, https://jg-rp.github.io/python-jsonpath/
 Project-URL: Issues, https://github.com/jg-rp/python-jsonpath/issues
 Project-URL: Source, https://github.com/jg-rp/python-jsonpath
 Author-email: James Prior <jamesgr.prior@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 <h1 align="center">Python JSONPath</h1>
 
 <p align="center">
-A flexible JSONPath engine for Python.
+A flexible JSONPath engine for Python with JSON Pointer and JSON Patch.
 </p>
 
 <p align="center">
   <a href="https://github.com/jg-rp/python-jsonpath/blob/main/LICENSE.txt">
     <img src="https://img.shields.io/pypi/l/python-jsonpath?style=flat-square" alt="License">
   </a>
   <a href="https://github.com/jg-rp/python-jsonpath/actions">
@@ -87,68 +87,64 @@
 ### JSONPath
 
 ```python
 import jsonpath
 
 data = {
     "users": [
-        {
-            "name": "Sue",
-            "score": 100,
-        },
-        {
-            "name": "John",
-            "score": 86,
-        },
-        {
-            "name": "Sally",
-            "score": 84,
-        },
-        {
-            "name": "Jane",
-            "score": 55,
-        },
+        {"name": "Sue", "score": 100},
+        {"name": "John", "score": 86},
+        {"name": "Sally", "score": 84},
+        {"name": "Jane", "score": 55},
     ]
 }
 
 user_names = jsonpath.findall("$.users[?@.score < 100].name", data)
 print(user_names) # ['John', 'Sally', 'Jane']
 ```
 
 ### JSON Pointer
 
-Since version 0.8.0, we also include an [RFC 6901](https://datatracker.ietf.org/doc/html/rfc6901) compliant implementation of JSON Pointer.
+Since version 0.8.0, we include an [RFC 6901](https://datatracker.ietf.org/doc/html/rfc6901) compliant implementation of JSON Pointer. See JSON Pointer [quick start](https://jg-rp.github.io/python-jsonpath/quickstart/#pointerresolvepointer-data), [guide](https://jg-rp.github.io/python-jsonpath/pointers/) and [API reference](https://jg-rp.github.io/python-jsonpath/api/#jsonpath.JSONPointer)
 
 ```python
 from jsonpath import pointer
 
 data = {
     "users": [
-        {
-            "name": "Sue",
-            "score": 100,
-        },
-        {
-            "name": "John",
-            "score": 86,
-        },
-        {
-            "name": "Sally",
-            "score": 84,
-        },
-        {
-            "name": "Jane",
-            "score": 55,
-        },
+        {"name": "Sue", "score": 100},
+        {"name": "John", "score": 86},
+        {"name": "Sally", "score": 84},
+        {"name": "Jane", "score": 55},
     ]
 }
 
 sue_score = pointer.resolve("/users/0/score", data)
 print(sue_score)  # 100
 
 jane_score = pointer.resolve(["users", 3, "score"], data)
 print(jane_score)  # 55
 ```
 
+### JSON Patch
+
+Since version 0.8.0, we also include an [RFC 6902](https://datatracker.ietf.org/doc/html/rfc6902) compliant implementation of JSON Patch. See JSON Patch [quick start](https://jg-rp.github.io/python-jsonpath/quickstart/#patchapplypatch-data) and [API reference](https://jg-rp.github.io/python-jsonpath/api/#jsonpath.JSONPatch)
+
+```python
+from jsonpath import patch
+
+patch_operations = [
+    {"op": "add", "path": "/some/foo", "value": {"foo": {}}},
+    {"op": "add", "path": "/some/foo", "value": {"bar": []}},
+    {"op": "copy", "from": "/some/other", "path": "/some/foo/else"},
+    {"op": "add", "path": "/some/foo/bar/-", "value": 1},
+]
+
+data = {"some": {"other": "thing"}}
+patch.apply(patch_operations, data)
+print(data) # {'some': {'other': 'thing', 'foo': {'bar': [1], 'else': 'thing'}}}
+
+```
+
 ## License
 
 `python-jsonpath` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

#### html2text {}

```diff
@@ -1,43 +1,57 @@
-Metadata-Version: 2.1 Name: python-jsonpath Version: 0.8.1 Summary: Another
-JSONPath implementation for Python. Project-URL: Documentation, https://jg-
+Metadata-Version: 2.1 Name: python-jsonpath Version: 0.9.0 Summary: JSONPath,
+JSON Pointer and JSON Patch for Python. Project-URL: Documentation, https://jg-
 rp.github.io/python-jsonpath/ Project-URL: Issues, https://github.com/jg-rp/
 python-jsonpath/issues Project-URL: Source, https://github.com/jg-rp/python-
 jsonpath Author-email: James Prior
 prior@gmail.com> License-Expression: MIT License-File: LICENSE.txt Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
 Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown
                          ****** Python JSONPath ******
-                    A flexible JSONPath engine for Python.
+    A flexible JSONPath engine for Python with JSON Pointer and JSON Patch.
                               [License] [Tests]
                       [PyPi_-_Version] [Python_versions]
 --- **Table of Contents** - [Install](#install) - [Links](#links) - [Examples]
 (#examples) - [License](#license) ## Install Install Python JSONPath using
 [pip](https://pip.pypa.io/en/stable/getting-started/): ```console pip install
 python-jsonpath ``` Or [Pipenv](https://pipenv.pypa.io/en/latest/): ```console
 pipenv install -u python-jsonpath ``` Or from [conda-forge](https://
 anaconda.org/conda-forge/python-jsonpath): ```console conda install -c conda-
 forge python-jsonpath ``` ## Links - Documentation: https://jg-rp.github.io/
 python-jsonpath/. - JSONPath Syntax: https://jg-rp.github.io/python-jsonpath/
 syntax/ - Change log: https://github.com/jg-rp/python-jsonpath/blob/main/
 CHANGELOG.md - PyPi: https://pypi.org/project/python-jsonpath - Source code:
 https://github.com/jg-rp/python-jsonpath - Issue tracker: https://github.com/
 jg-rp/python-jsonpath/issues ## Examples ### JSONPath ```python import jsonpath
-data = { "users": [ { "name": "Sue", "score": 100, }, { "name": "John",
-"score": 86, }, { "name": "Sally", "score": 84, }, { "name": "Jane", "score":
-55, }, ] } user_names = jsonpath.findall("$.users[?@.score < 100].name", data)
-print(user_names) # ['John', 'Sally', 'Jane'] ``` ### JSON Pointer Since
-version 0.8.0, we also include an [RFC 6901](https://datatracker.ietf.org/doc/
-html/rfc6901) compliant implementation of JSON Pointer. ```python from jsonpath
-import pointer data = { "users": [ { "name": "Sue", "score": 100, }, { "name":
-"John", "score": 86, }, { "name": "Sally", "score": 84, }, { "name": "Jane",
-"score": 55, }, ] } sue_score = pointer.resolve("/users/0/score", data) print
+data = { "users": [ {"name": "Sue", "score": 100}, {"name": "John", "score":
+86}, {"name": "Sally", "score": 84}, {"name": "Jane", "score": 55}, ] }
+user_names = jsonpath.findall("$.users[?@.score < 100].name", data) print
+(user_names) # ['John', 'Sally', 'Jane'] ``` ### JSON Pointer Since version
+0.8.0, we include an [RFC 6901](https://datatracker.ietf.org/doc/html/rfc6901)
+compliant implementation of JSON Pointer. See JSON Pointer [quick start](https:
+//jg-rp.github.io/python-jsonpath/quickstart/#pointerresolvepointer-data),
+[guide](https://jg-rp.github.io/python-jsonpath/pointers/) and [API reference]
+(https://jg-rp.github.io/python-jsonpath/api/#jsonpath.JSONPointer) ```python
+from jsonpath import pointer data = { "users": [ {"name": "Sue", "score": 100},
+{"name": "John", "score": 86}, {"name": "Sally", "score": 84}, {"name": "Jane",
+"score": 55}, ] } sue_score = pointer.resolve("/users/0/score", data) print
 (sue_score) # 100 jane_score = pointer.resolve(["users", 3, "score"], data)
-print(jane_score) # 55 ``` ## License `python-jsonpath` is distributed under
-the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+print(jane_score) # 55 ``` ### JSON Patch Since version 0.8.0, we also include
+an [RFC 6902](https://datatracker.ietf.org/doc/html/rfc6902) compliant
+implementation of JSON Patch. See JSON Patch [quick start](https://jg-
+rp.github.io/python-jsonpath/quickstart/#patchapplypatch-data) and [API
+reference](https://jg-rp.github.io/python-jsonpath/api/#jsonpath.JSONPatch)
+```python from jsonpath import patch patch_operations = [ {"op": "add", "path":
+"/some/foo", "value": {"foo": {}}}, {"op": "add", "path": "/some/foo", "value":
+{"bar": []}}, {"op": "copy", "from": "/some/other", "path": "/some/foo/else"},
+{"op": "add", "path": "/some/foo/bar/-", "value": 1}, ] data = {"some":
+{"other": "thing"}} patch.apply(patch_operations, data) print(data) # {'some':
+{'other': 'thing', 'foo': {'bar': [1], 'else': 'thing'}}} ``` ## License
+`python-jsonpath` is distributed under the terms of the [MIT](https://spdx.org/
+licenses/MIT.html) license.
```

