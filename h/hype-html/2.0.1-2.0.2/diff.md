# Comparing `tmp/hype_html-2.0.1.tar.gz` & `tmp/hype_html-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hype_html-2.0.1.tar", max compression
+gzip compressed data, was "hype_html-2.0.2.tar", max compression
```

## Comparing `hype_html-2.0.1.tar` & `hype_html-2.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1060 2023-04-29 15:04:42.318609 hype_html-2.0.1/LICENSE
--rw-r--r--   0        0        0     3362 2023-07-21 01:05:21.615529 hype_html-2.0.1/README.md
--rw-r--r--   0        0        0     1060 2023-04-29 15:04:42.319608 hype_html-2.0.1/hype/LICENSE
--rw-r--r--   0        0        0     1196 2023-07-21 03:40:06.266196 hype_html-2.0.1/hype/__init__.py
--rw-r--r--   0        0        0     1426 2023-07-21 03:40:06.306296 hype_html-2.0.1/hype/asyncio/__init__.py
--rw-r--r--   0        0        0   185102 2023-07-21 03:36:07.261516 hype_html-2.0.1/hype/asyncio/element.py
--rw-r--r--   0        0        0   185077 2023-07-21 03:22:33.145794 hype_html-2.0.1/hype/element.py
--rw-r--r--   0        0        0        0 2023-04-29 16:08:45.852021 hype_html-2.0.1/hype/py.typed
--rw-r--r--   0        0        0      529 2023-07-21 03:40:19.296414 hype_html-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     3956 1970-01-01 00:00:00.000000 hype_html-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-29 15:04:42.318609 hype_html-2.0.2/LICENSE
+-rw-r--r--   0        0        0     3362 2023-07-21 01:05:21.615529 hype_html-2.0.2/README.md
+-rw-r--r--   0        0        0     1060 2023-04-29 15:04:42.319608 hype_html-2.0.2/hype/LICENSE
+-rw-r--r--   0        0        0     1196 2023-07-21 03:40:06.266196 hype_html-2.0.2/hype/__init__.py
+-rw-r--r--   0        0        0     1426 2023-07-21 03:40:06.306296 hype_html-2.0.2/hype/asyncio/__init__.py
+-rw-r--r--   0        0        0   185084 2023-07-21 04:26:44.258682 hype_html-2.0.2/hype/asyncio/element.py
+-rw-r--r--   0        0        0   185077 2023-07-21 03:22:33.145794 hype_html-2.0.2/hype/element.py
+-rw-r--r--   0        0        0        0 2023-04-29 16:08:45.852021 hype_html-2.0.2/hype/py.typed
+-rw-r--r--   0        0        0      569 2023-07-21 22:56:04.516979 hype_html-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3956 1970-01-01 00:00:00.000000 hype_html-2.0.2/PKG-INFO
```

### Comparing `hype_html-2.0.1/LICENSE` & `hype_html-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hype_html-2.0.1/README.md` & `hype_html-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hype_html-2.0.1/hype/LICENSE` & `hype_html-2.0.2/hype/LICENSE`

 * *Files identical despite different names*

### Comparing `hype_html-2.0.1/hype/__init__.py` & `hype_html-2.0.2/hype/__init__.py`

 * *Files identical despite different names*

### Comparing `hype_html-2.0.1/hype/asyncio/__init__.py` & `hype_html-2.0.2/hype/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `hype_html-2.0.1/hype/asyncio/element.py` & `hype_html-2.0.2/hype/asyncio/element.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 class Element:
     self_closing = False
 
     @property
     def tag(self) -> str:
         raise RuntimeError("Element requires tag property to render.")
 
-    def __init__(self, *args: Union[str, "Element"], **kwargs: Optional[str]):
+    def __init__(self, *args: Any, **kwargs: Optional[str]):
         if self.self_closing and len(args):
             raise RuntimeError("Self closing elements cannot have inner elements.")
 
         self.inner_elements = list(args)
         self.props = {}
         for k, v in kwargs.items():
             key, val = self._process_attr(k, v)
```

### Comparing `hype_html-2.0.1/hype/element.py` & `hype_html-2.0.2/hype/element.py`

 * *Files identical despite different names*

### Comparing `hype_html-2.0.1/pyproject.toml` & `hype_html-2.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 [tool.poetry]
 name = "hype-html"
-version = "2.0.1"
+version = "2.0.2"
 description = "A minimal python dsl for generating html."
 authors = ["Scott Russell <me@scottrussell.net>"]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "hype"}]
+packages = [
+    {include = "hype"},
+    {include = "hype/py.typed"},
+]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 
 [tool.poetry.group.dev.dependencies]
 jinja2 = "^3.1.2"
```

### Comparing `hype_html-2.0.1/PKG-INFO` & `hype_html-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hype-html
-Version: 2.0.1
+Version: 2.0.2
 Summary: A minimal python dsl for generating html.
 License: MIT
 Author: Scott Russell
 Author-email: me@scottrussell.net
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

