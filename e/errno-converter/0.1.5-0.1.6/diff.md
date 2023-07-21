# Comparing `tmp/errno_converter-0.1.5.tar.gz` & `tmp/errno_converter-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "errno_converter-0.1.5.tar", last modified: Fri Jul 21 22:09:29 2023, max compression
+gzip compressed data, was "errno_converter-0.1.6.tar", last modified: Fri Jul 21 23:21:39 2023, max compression
```

## Comparing `errno_converter-0.1.5.tar` & `errno_converter-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 poku      (1000) poku      (1000)        0 2023-07-21 22:09:29.372821 errno_converter-0.1.5/
--rw-r--r--   0 poku      (1000) poku      (1000)     7048 2021-10-29 23:27:48.000000 errno_converter-0.1.5/LICENSE
--rw-r--r--   0 poku      (1000) poku      (1000)    11081 2023-07-21 22:09:29.372821 errno_converter-0.1.5/PKG-INFO
--rw-r--r--   0 poku      (1000) poku      (1000)     2381 2022-08-24 23:08:46.000000 errno_converter-0.1.5/README.md
--rw-r--r--   0 poku      (1000) poku      (1000)      838 2023-07-21 21:18:22.000000 errno_converter-0.1.5/pyproject.toml
--rw-r--r--   0 poku      (1000) poku      (1000)       38 2023-07-21 22:09:29.372821 errno_converter-0.1.5/setup.cfg
-drwxr-xr-x   0 poku      (1000) poku      (1000)        0 2023-07-21 22:09:29.372821 errno_converter-0.1.5/src/
--rw-r--r--   0 poku      (1000) poku      (1000)        0 2022-08-24 23:08:46.000000 errno_converter-0.1.5/src/__init__.py
--rwxr-xr-x   0 poku      (1000) poku      (1000)     6048 2023-07-21 21:58:17.000000 errno_converter-0.1.5/src/converter_lib.py
-drwxr-xr-x   0 poku      (1000) poku      (1000)        0 2023-07-21 22:09:29.372821 errno_converter-0.1.5/src/errno_converter.egg-info/
--rw-r--r--   0 poku      (1000) poku      (1000)    11081 2023-07-21 22:09:29.000000 errno_converter-0.1.5/src/errno_converter.egg-info/PKG-INFO
--rw-r--r--   0 poku      (1000) poku      (1000)      356 2023-07-21 22:09:29.000000 errno_converter-0.1.5/src/errno_converter.egg-info/SOURCES.txt
--rw-r--r--   0 poku      (1000) poku      (1000)        1 2023-07-21 22:09:29.000000 errno_converter-0.1.5/src/errno_converter.egg-info/dependency_links.txt
--rw-r--r--   0 poku      (1000) poku      (1000)      135 2023-07-21 22:09:29.000000 errno_converter-0.1.5/src/errno_converter.egg-info/entry_points.txt
--rw-r--r--   0 poku      (1000) poku      (1000)       71 2023-07-21 22:09:29.000000 errno_converter-0.1.5/src/errno_converter.egg-info/top_level.txt
--rwxr-xr-x   0 poku      (1000) poku      (1000)      613 2023-07-21 21:50:37.000000 errno_converter-0.1.5/src/errno_converter.py
--rwxr-xr-x   0 poku      (1000) poku      (1000)      691 2023-07-21 21:49:27.000000 errno_converter-0.1.5/src/http_converter.py
--rwxr-xr-x   0 poku      (1000) poku      (1000)      686 2023-07-21 21:50:57.000000 errno_converter-0.1.5/src/signal_converter.py
+drwxr-xr-x   0 poku      (1000) poku      (1000)        0 2023-07-21 23:21:39.249889 errno_converter-0.1.6/
+-rw-r--r--   0 poku      (1000) poku      (1000)     7048 2021-10-29 23:27:48.000000 errno_converter-0.1.6/LICENSE
+-rw-r--r--   0 poku      (1000) poku      (1000)    11081 2023-07-21 23:21:39.249889 errno_converter-0.1.6/PKG-INFO
+-rw-r--r--   0 poku      (1000) poku      (1000)     2381 2022-08-24 23:08:46.000000 errno_converter-0.1.6/README.md
+-rw-r--r--   0 poku      (1000) poku      (1000)      838 2023-07-21 23:20:00.000000 errno_converter-0.1.6/pyproject.toml
+-rw-r--r--   0 poku      (1000) poku      (1000)       38 2023-07-21 23:21:39.249889 errno_converter-0.1.6/setup.cfg
+drwxr-xr-x   0 poku      (1000) poku      (1000)        0 2023-07-21 23:21:39.249889 errno_converter-0.1.6/src/
+drwxr-xr-x   0 poku      (1000) poku      (1000)        0 2023-07-21 23:21:39.249889 errno_converter-0.1.6/src/errno_converter.egg-info/
+-rw-r--r--   0 poku      (1000) poku      (1000)    11081 2023-07-21 23:21:39.000000 errno_converter-0.1.6/src/errno_converter.egg-info/PKG-INFO
+-rw-r--r--   0 poku      (1000) poku      (1000)      378 2023-07-21 23:21:39.000000 errno_converter-0.1.6/src/errno_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 poku      (1000) poku      (1000)        1 2023-07-21 23:21:39.000000 errno_converter-0.1.6/src/errno_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 poku      (1000) poku      (1000)      135 2023-07-21 23:21:39.000000 errno_converter-0.1.6/src/errno_converter.egg-info/entry_points.txt
+-rw-r--r--   0 poku      (1000) poku      (1000)       52 2023-07-21 23:21:39.000000 errno_converter-0.1.6/src/errno_converter.egg-info/top_level.txt
+-rwxr-xr-x   0 poku      (1000) poku      (1000)      635 2023-07-21 23:19:31.000000 errno_converter-0.1.6/src/errno_converter.py
+-rwxr-xr-x   0 poku      (1000) poku      (1000)      713 2023-07-21 23:19:31.000000 errno_converter-0.1.6/src/http_converter.py
+drwxr-xr-x   0 poku      (1000) poku      (1000)        0 2023-07-21 23:21:39.249889 errno_converter-0.1.6/src/lib/
+-rw-r--r--   0 poku      (1000) poku      (1000)        0 2023-07-21 22:24:54.000000 errno_converter-0.1.6/src/lib/__init__.py
+-rwxr-xr-x   0 poku      (1000) poku      (1000)      826 2023-07-21 22:22:31.000000 errno_converter-0.1.6/src/lib/converter.py
+-rw-r--r--   0 poku      (1000) poku      (1000)     5468 2023-07-21 22:49:41.000000 errno_converter-0.1.6/src/lib/parser.py
+-rwxr-xr-x   0 poku      (1000) poku      (1000)      708 2023-07-21 23:19:31.000000 errno_converter-0.1.6/src/signal_converter.py
```

### Comparing `errno_converter-0.1.5/LICENSE` & `errno_converter-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `errno_converter-0.1.5/PKG-INFO` & `errno_converter-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: errno_converter
-Version: 0.1.5
+Version: 0.1.6
 Summary: As simple command line tool to convert error numbers (of C errno.h), http status codes and signal numbers to human readable strings or back zu numbers.
 Author-email: Heinrich Kießling <heinrich@kiess.link>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
```

### Comparing `errno_converter-0.1.5/README.md` & `errno_converter-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `errno_converter-0.1.5/pyproject.toml` & `errno_converter-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "errno_converter"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Heinrich Kießling", email="heinrich@kiess.link" },
 ]
 description = "As simple command line tool to convert error numbers (of C errno.h), http status codes and signal numbers to human readable strings or back zu numbers."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `errno_converter-0.1.5/src/converter_lib.py` & `errno_converter-0.1.6/src/lib/parser.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,36 @@
-import abc
 import logging
 import os
 import re
 import subprocess
 import sys
-from typing import Sequence
+from importlib.metadata import version as get_version, PackageNotFoundError
 
-logger = logging.getLogger(__name__)
-
-
-class Converter(object, metaclass=abc.ABCMeta):
-    NAME: str = ""
-    NUMBER_RANGE: Sequence[int] = ()
-
-    @staticmethod
-    @abc.abstractmethod
-    def number2code(number: int) -> str:
-        """Convert a single numerical code to its textual code, raise an Exception if impossible."""
+from .converter import Converter
 
-    @staticmethod
-    @abc.abstractmethod
-    def code2number(code: str) -> int:
-        """Convert a textual code to its numerical code, raise an Exception if impossible."""
-
-    @staticmethod
-    @abc.abstractmethod
-    def number2description(number: int) -> str:
-        """Convert a numerical code to its description (empty string if impossible)"""
 
-    @staticmethod
-    @abc.abstractmethod
-    def get_candidates() -> list[str]:
-        """List all textual codes that can be converted."""
+logger = logging.getLogger(__name__)
 
 
 class Parser:
     @staticmethod
     def _print_version():
         """Print Git project version by running ``git describe --tags`` in this project."""
 
-        project_dir = os.path.dirname(__file__)
-        with open(os.devnull, "wb") as devnull:
-            version = subprocess.check_output(
-                ["git", "describe", "--tags"], stderr=devnull, cwd=project_dir
-            )
-            version = version.rstrip()
-        if hasattr(version, "decode"):
-            version = version.decode("utf-8")
+        try:
+            version = get_version("errno-converter")
+        except PackageNotFoundError:
+            project_dir = os.path.dirname(__file__)
+            with open(os.devnull, "wb") as devnull:
+                version = subprocess.check_output(
+                    ["git", "describe", "--tags"], stderr=devnull, cwd=project_dir
+                )
+                version = version.rstrip()
+            if hasattr(version, "decode"):
+                version = version.decode("utf-8")
         print(f"{sys.argv[0]} version {version}")
 
     @staticmethod
     def _print_help(converter: type[Converter]) -> None:
         """Prints help text to cli."""
         print(
             "{cmd} [-v] list|<{name}-number>|<{name}-name>".format(
```

### Comparing `errno_converter-0.1.5/src/errno_converter.egg-info/PKG-INFO` & `errno_converter-0.1.6/src/errno_converter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: errno-converter
-Version: 0.1.5
+Version: 0.1.6
 Summary: As simple command line tool to convert error numbers (of C errno.h), http status codes and signal numbers to human readable strings or back zu numbers.
 Author-email: Heinrich Kießling <heinrich@kiess.link>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
```

### Comparing `errno_converter-0.1.5/src/errno_converter.py` & `errno_converter-0.1.6/src/errno_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import errno
 
-from converter_lib import Converter, Parser
+from lib.converter import Converter
+from lib.parser import Parser
 
 
 class ErrnoConverter(Converter):
     NAME: str = "errno"
     NUMBER_RANGE: range = range(1, 132)
 
     @staticmethod
```

### Comparing `errno_converter-0.1.5/src/http_converter.py` & `errno_converter-0.1.6/src/http_converter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import http
 from typing import Sequence
 
-from converter_lib import Converter, Parser
+from lib.converter import Converter
+from lib.parser import Parser
 
 
 class HttpConverter(Converter):
     NAME: str = "http"
     NUMBER_RANGE: Sequence[int] = range(100, 600)
 
     @staticmethod
```

