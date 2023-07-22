# Comparing `tmp/py3settings-2.0.3.tar.gz` & `tmp/py3settings-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3settings-2.0.3.tar", last modified: Fri Jul 14 22:35:09 2023, max compression
+gzip compressed data, was "py3settings-2.1.0.tar", last modified: Sat Jul 22 15:35:16 2023, max compression
```

## Comparing `py3settings-2.0.3.tar` & `py3settings-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 22:35:09.151105 py3settings-2.0.3/
--rw-rw-rw-   0        0        0      588 2023-07-14 22:35:09.152104 py3settings-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-07-14 16:12:21.000000 py3settings-2.0.3/README.md
--rw-rw-rw-   0        0        0      108 2023-07-14 16:31:07.000000 py3settings-2.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      695 2023-07-14 22:35:09.156104 py3settings-2.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-14 22:35:09.132107 py3settings-2.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-14 22:35:09.139104 py3settings-2.0.3/src/py3Settings/
--rw-rw-rw-   0        0        0      114 2023-07-14 22:33:50.000000 py3settings-2.0.3/src/py3Settings/__init__.py
--rw-rw-rw-   0        0        0      616 2023-07-14 22:06:08.000000 py3settings-2.0.3/src/py3Settings/example.py
--rw-rw-rw-   0        0        0      353 2023-07-14 22:00:44.000000 py3settings-2.0.3/src/py3Settings/file.py
--rw-rw-rw-   0        0        0     6340 2023-07-14 22:34:47.000000 py3settings-2.0.3/src/py3Settings/main.py
-drwxrwxrwx   0        0        0        0 2023-07-14 22:35:09.150103 py3settings-2.0.3/src/py3settings.egg-info/
--rw-rw-rw-   0        0        0      588 2023-07-14 22:35:09.000000 py3settings-2.0.3/src/py3settings.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-07-14 22:35:09.000000 py3settings-2.0.3/src/py3settings.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 22:35:09.000000 py3settings-2.0.3/src/py3settings.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-14 22:35:09.000000 py3settings-2.0.3/src/py3settings.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 15:35:16.635970 py3settings-2.1.0/
+-rw-rw-rw-   0        0        0     1161 2023-07-22 14:34:20.000000 py3settings-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0      611 2023-07-22 15:35:16.635970 py3settings-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-07-14 16:12:21.000000 py3settings-2.1.0/README.md
+-rw-rw-rw-   0        0        0      108 2023-07-14 16:31:07.000000 py3settings-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      695 2023-07-22 15:35:16.636973 py3settings-2.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-22 15:35:16.609969 py3settings-2.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-22 15:35:16.621971 py3settings-2.1.0/src/py3Settings/
+-rw-rw-rw-   0        0        0      434 2023-07-22 14:34:20.000000 py3settings-2.1.0/src/py3Settings/__init__.py
+-rw-rw-rw-   0        0        0      353 2023-07-14 22:00:44.000000 py3settings-2.1.0/src/py3Settings/file.py
+-rw-rw-rw-   0        0        0     5973 2023-07-22 14:57:03.000000 py3settings-2.1.0/src/py3Settings/main.py
+-rw-rw-rw-   0        0        0     1005 2023-07-15 09:51:07.000000 py3settings-2.1.0/src/py3Settings/proxy.py
+-rw-rw-rw-   0        0        0      269 2023-07-15 09:51:22.000000 py3settings-2.1.0/src/py3Settings/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-22 15:35:16.633970 py3settings-2.1.0/src/py3settings.egg-info/
+-rw-rw-rw-   0        0        0      611 2023-07-22 15:35:16.000000 py3settings-2.1.0/src/py3settings.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-07-22 15:35:16.000000 py3settings-2.1.0/src/py3settings.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 15:35:16.000000 py3settings-2.1.0/src/py3settings.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-22 15:35:16.000000 py3settings-2.1.0/src/py3settings.egg-info/top_level.txt
```

### Comparing `py3settings-2.0.3/PKG-INFO` & `py3settings-2.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: py3settings
-Version: 2.0.3
+Version: 2.1.0
 Summary: A powerful json file settings manager for Python 3
 Home-page: https://github.com/acalasanzs/py3Settings
 Author: Albert Calasanz Sallen
 Author-email: acalasanzs@gmail.com
 Project-URL: Bug Tracker, https://github.com/acalasanzs/py3Settings/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 Hecho con mucho amor por Albert Calasanz Sallen
 v1.0
```

### Comparing `py3settings-2.0.3/setup.cfg` & `py3settings-2.1.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7933 7365 7474 696e 6773 0d0a   = py3settings..
-00000020: 7665 7273 696f 6e20 3d20 322e 302e 330d  version = 2.0.3.
+00000020: 7665 7273 696f 6e20 3d20 322e 312e 300d  version = 2.1.0.
 00000030: 0a61 7574 686f 7220 3d20 416c 6265 7274  .author = Albert
 00000040: 2043 616c 6173 616e 7a20 5361 6c6c 656e   Calasanz Sallen
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2061 6361 6c61 7361 6e7a 7340 676d 6169   acalasanzs@gmai
 00000070: 6c2e 636f 6d0d 0a64 6573 6372 6970 7469  l.com..descripti
 00000080: 6f6e 203d 2041 2070 6f77 6572 6675 6c20  on = A powerful 
 00000090: 6a73 6f6e 2066 696c 6520 7365 7474 696e  json file settin
```

### Comparing `py3settings-2.0.3/src/py3Settings/main.py` & `py3settings-2.1.0/src/py3Settings/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import os
-from typing import Any, Callable, List
-from . import file
+from typing import Any, Callable, Iterator, List
+import file
+from proxy import *
+from utils import *
+from collections.abc import Mapping
 # from packages.AppSettings.utils import staticinstance
-import re
 class Attribute:
     def __init__ (self, attr: str, typ : Any | None = None, validate:  Callable[[object], bool] | None = None, default: bool = False, getter: Callable[[], Any] = None):
         self.attr = attr
         if typ is None and validate is Callable[[object], bool]:
             self.validate = validate
         elif validate is None and typ is not None:
             self.typ = typ
             self.validate = lambda a: isinstance(a, typ) if not hasattr(self, 'get') else self.get
             if getter is not None:
                 self.get = getter
         else:
             raise SystemExit("No type!")
         self.default = default
-def printObjProps(theObject):
-    for property, value in vars(theObject).items():
-        print(property, ":", value)
 class Option():
     def __init__(self, name: str, optionName: str = "name", optionID: str | None = None):
         self.name = name
         self.optionName = optionName
         self.attributes = []
         self.default = None
         if optionID is None:
@@ -30,54 +29,45 @@
         self.optionID = optionID
     def append(self, attribute: Attribute):
         if self.default is None:
             self.default = attribute
         if attribute.default:
             self.default = attribute
         self.attributes.append(attribute)
-def getWithAttr(list: list, attr: str, name: str):
-    for x in list:
-        if getattr(x, name) == attr:
-            return x
-    return False
-def handle(format, dict:dict):
-    ins = Handler(format)
-    ins.init(**dict)
-    return ins
-class Handler:
-    invalid = r'[<>:"/\|?* ]'
-    def __init__(self, format: str):
-        self.format = format
-    def init(self, load: Callable[[str,str], dict], save: Callable[[dict], str | bool]):
-        self.load = Handler.safeCheck(load)
-        self.save = Handler.safeCheck(save)
-    @staticmethod
-    def safeCheck(fun):
-        def wrapper(*args, **kwargs):
-            assert Handler.fileStr(kwargs.get('filename') or args[0])
-            return fun(*args, **kwargs)
-        return wrapper
-    @classmethod
-    def fileStr(cls, file: str) -> bool:
-        file = file.split(".")
-        if(len(file) != 2):
-            return False
-        filename = file[0]
-        original = file[0]
-        if re.search(cls.invalid, filename):
-            return False
-        if original != filename:
-            return False
-        return True
 formats = [handle('.json',file.JSON)]
-class AppSettings():
+
+def addFormatSupport(Handler: Handler):
+    formats.append(Handler)
+def showFileDefs():
+    return file
+class AppSettings(Mapping):
     def __init__(self, options: List[Option]):
         self.options = options
         self.dict = dict()
         self.defaults = dict()
+        self.i = 0
+    def __getitem__(self, __key: str | int) -> Option:
+        for i,x in enumerate(self.options):
+            if __key == x.name or i == __key:
+                return x
+    def __delitem__(self, __key: str | int) -> None:
+        for i,x in enumerate(self.options):
+            if __key == x.name or i == __key:
+                self.options.remove(x)
+                return
+    def __iter__(self):
+        return self
+    def __len__(self) -> int:
+        return self.options.__len__()
+    def __next__(self):
+        if self.__len__()  == self.i:
+            raise StopIteration
+        x = self.options[self.i]
+        self.i += 1
+        return x
     @staticmethod
     def _loadFile(filename:str, path = os.getcwd()):
         type = "."+filename.split(".")[1]
         for x in formats:
             if x.format == type:
                 if(len(filename) == 0):
                     filename = f"settings{x.format}"
@@ -97,15 +87,15 @@
         if data is False:
             raise SystemExit("Format not supported")
         return self.load(data)
     def saveFile(self, *args,**kwargs):
         return AppSettings._saveFile(AppSettings.preProcess(self.dict), *args,**kwargs)
     @staticmethod
     def preProcess(data: dict):
-        return [x for x in data.values()]
+        return list(data.values())
     def validateAll(self):
         i = 0
         for key, value in self.dict.items():
             for option in self.options:
                 if option.optionName in value and value[option.optionName] == option.optionID:
                     for attr in [y for y in list(value.keys()) if y != option.optionName]:
                         attr_get = getWithAttr(option.attributes, attr, 'attr')
```

### Comparing `py3settings-2.0.3/src/py3settings.egg-info/PKG-INFO` & `py3settings-2.1.0/src/py3settings.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: py3settings
-Version: 2.0.3
+Version: 2.1.0
 Summary: A powerful json file settings manager for Python 3
 Home-page: https://github.com/acalasanzs/py3Settings
 Author: Albert Calasanz Sallen
 Author-email: acalasanzs@gmail.com
 Project-URL: Bug Tracker, https://github.com/acalasanzs/py3Settings/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 Hecho con mucho amor por Albert Calasanz Sallen
 v1.0
```

