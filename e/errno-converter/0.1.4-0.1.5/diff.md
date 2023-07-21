# Comparing `tmp/errno_converter-0.1.4.tar.gz` & `tmp/errno_converter-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "errno_converter-0.1.4.tar", last modified: Tue Jul  4 20:48:17 2023, max compression
+gzip compressed data, was "errno_converter-0.1.5.tar", last modified: Fri Jul 21 22:09:29 2023, max compression
```

## Comparing `errno_converter-0.1.4.tar` & `errno_converter-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 poku      (1000) poku      (1000)        0 2023-07-04 20:48:17.293100 errno_converter-0.1.4/
--rw-r--r--   0 poku      (1000) poku      (1000)     7048 2021-10-29 23:27:48.000000 errno_converter-0.1.4/LICENSE
--rw-r--r--   0 poku      (1000) poku      (1000)    11081 2023-07-04 20:48:17.293100 errno_converter-0.1.4/PKG-INFO
--rw-r--r--   0 poku      (1000) poku      (1000)     2381 2022-08-24 23:08:46.000000 errno_converter-0.1.4/README.md
--rw-r--r--   0 poku      (1000) poku      (1000)      838 2023-07-04 20:38:56.000000 errno_converter-0.1.4/pyproject.toml
--rw-r--r--   0 poku      (1000) poku      (1000)       38 2023-07-04 20:48:17.293100 errno_converter-0.1.4/setup.cfg
-drwxr-xr-x   0 poku      (1000) poku      (1000)        0 2023-07-04 20:48:17.289767 errno_converter-0.1.4/src/
--rw-r--r--   0 poku      (1000) poku      (1000)        0 2022-08-24 23:08:46.000000 errno_converter-0.1.4/src/__init__.py
--rwxr-xr-x   0 poku      (1000) poku      (1000)     5005 2023-07-04 20:08:00.000000 errno_converter-0.1.4/src/converter_lib.py
-drwxr-xr-x   0 poku      (1000) poku      (1000)        0 2023-07-04 20:48:17.293100 errno_converter-0.1.4/src/errno_converter.egg-info/
--rw-r--r--   0 poku      (1000) poku      (1000)    11081 2023-07-04 20:48:17.000000 errno_converter-0.1.4/src/errno_converter.egg-info/PKG-INFO
--rw-r--r--   0 poku      (1000) poku      (1000)      356 2023-07-04 20:48:17.000000 errno_converter-0.1.4/src/errno_converter.egg-info/SOURCES.txt
--rw-r--r--   0 poku      (1000) poku      (1000)        1 2023-07-04 20:48:17.000000 errno_converter-0.1.4/src/errno_converter.egg-info/dependency_links.txt
--rw-r--r--   0 poku      (1000) poku      (1000)      135 2023-07-04 20:48:17.000000 errno_converter-0.1.4/src/errno_converter.egg-info/entry_points.txt
--rw-r--r--   0 poku      (1000) poku      (1000)       71 2023-07-04 20:48:17.000000 errno_converter-0.1.4/src/errno_converter.egg-info/top_level.txt
--rwxr-xr-x   0 poku      (1000) poku      (1000)      567 2023-07-04 20:08:00.000000 errno_converter-0.1.4/src/errno_converter.py
--rwxr-xr-x   0 poku      (1000) poku      (1000)      610 2023-07-04 20:08:00.000000 errno_converter-0.1.4/src/http_converter.py
--rwxr-xr-x   0 poku      (1000) poku      (1000)      611 2023-07-04 20:08:00.000000 errno_converter-0.1.4/src/signal_converter.py
+drwxr-xr-x   0 poku      (1000) poku      (1000)        0 2023-07-21 22:09:29.372821 errno_converter-0.1.5/
+-rw-r--r--   0 poku      (1000) poku      (1000)     7048 2021-10-29 23:27:48.000000 errno_converter-0.1.5/LICENSE
+-rw-r--r--   0 poku      (1000) poku      (1000)    11081 2023-07-21 22:09:29.372821 errno_converter-0.1.5/PKG-INFO
+-rw-r--r--   0 poku      (1000) poku      (1000)     2381 2022-08-24 23:08:46.000000 errno_converter-0.1.5/README.md
+-rw-r--r--   0 poku      (1000) poku      (1000)      838 2023-07-21 21:18:22.000000 errno_converter-0.1.5/pyproject.toml
+-rw-r--r--   0 poku      (1000) poku      (1000)       38 2023-07-21 22:09:29.372821 errno_converter-0.1.5/setup.cfg
+drwxr-xr-x   0 poku      (1000) poku      (1000)        0 2023-07-21 22:09:29.372821 errno_converter-0.1.5/src/
+-rw-r--r--   0 poku      (1000) poku      (1000)        0 2022-08-24 23:08:46.000000 errno_converter-0.1.5/src/__init__.py
+-rwxr-xr-x   0 poku      (1000) poku      (1000)     6048 2023-07-21 21:58:17.000000 errno_converter-0.1.5/src/converter_lib.py
+drwxr-xr-x   0 poku      (1000) poku      (1000)        0 2023-07-21 22:09:29.372821 errno_converter-0.1.5/src/errno_converter.egg-info/
+-rw-r--r--   0 poku      (1000) poku      (1000)    11081 2023-07-21 22:09:29.000000 errno_converter-0.1.5/src/errno_converter.egg-info/PKG-INFO
+-rw-r--r--   0 poku      (1000) poku      (1000)      356 2023-07-21 22:09:29.000000 errno_converter-0.1.5/src/errno_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 poku      (1000) poku      (1000)        1 2023-07-21 22:09:29.000000 errno_converter-0.1.5/src/errno_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 poku      (1000) poku      (1000)      135 2023-07-21 22:09:29.000000 errno_converter-0.1.5/src/errno_converter.egg-info/entry_points.txt
+-rw-r--r--   0 poku      (1000) poku      (1000)       71 2023-07-21 22:09:29.000000 errno_converter-0.1.5/src/errno_converter.egg-info/top_level.txt
+-rwxr-xr-x   0 poku      (1000) poku      (1000)      613 2023-07-21 21:50:37.000000 errno_converter-0.1.5/src/errno_converter.py
+-rwxr-xr-x   0 poku      (1000) poku      (1000)      691 2023-07-21 21:49:27.000000 errno_converter-0.1.5/src/http_converter.py
+-rwxr-xr-x   0 poku      (1000) poku      (1000)      686 2023-07-21 21:50:57.000000 errno_converter-0.1.5/src/signal_converter.py
```

### Comparing `errno_converter-0.1.4/LICENSE` & `errno_converter-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `errno_converter-0.1.4/PKG-INFO` & `errno_converter-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: errno_converter
-Version: 0.1.4
+Version: 0.1.5
 Summary: As simple command line tool to convert error numbers (of C errno.h), http status codes and signal numbers to human readable strings or back zu numbers.
 Author-email: Heinrich Kießling <heinrich@kiess.link>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
```

### Comparing `errno_converter-0.1.4/README.md` & `errno_converter-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `errno_converter-0.1.4/pyproject.toml` & `errno_converter-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "errno_converter"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Heinrich Kießling", email="heinrich@kiess.link" },
 ]
 description = "As simple command line tool to convert error numbers (of C errno.h), http status codes and signal numbers to human readable strings or back zu numbers."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `errno_converter-0.1.4/src/converter_lib.py` & `errno_converter-0.1.5/src/converter_lib.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,160 +1,184 @@
-#!/usr/bin/env python3
-# coding=utf-8
-
-from enum import Enum
+import abc
 import logging
 import os
 import re
 import subprocess
 import sys
-
+from typing import Sequence
 
 logger = logging.getLogger(__name__)
 
 
-class Converter(object):
-    NAME = None
-    NUMBER_RANGE = ()
+class Converter(object, metaclass=abc.ABCMeta):
+    NAME: str = ""
+    NUMBER_RANGE: Sequence[int] = ()
 
     @staticmethod
-    def number2code(number):
-        raise NotImplementedError
+    @abc.abstractmethod
+    def number2code(number: int) -> str:
+        """Convert a single numerical code to its textual code, raise an Exception if impossible."""
 
     @staticmethod
-    def code2number(code):
-        raise NotImplementedError
+    @abc.abstractmethod
+    def code2number(code: str) -> int:
+        """Convert a textual code to its numerical code, raise an Exception if impossible."""
 
     @staticmethod
-    def number2description(number):
-        raise NotImplementedError
+    @abc.abstractmethod
+    def number2description(number: int) -> str:
+        """Convert a numerical code to its description (empty string if impossible)"""
 
     @staticmethod
-    def get_candidates():
-        raise NotImplementedError
+    @abc.abstractmethod
+    def get_candidates() -> list[str]:
+        """List all textual codes that can be converted."""
 
-    @classmethod
-    def print_version(cls):
-        """
-        Print Git project version by running ``git describe --tags`` in this project.
-        """
+
+class Parser:
+    @staticmethod
+    def _print_version():
+        """Print Git project version by running ``git describe --tags`` in this project."""
 
         project_dir = os.path.dirname(__file__)
         with open(os.devnull, "wb") as devnull:
             version = subprocess.check_output(
                 ["git", "describe", "--tags"], stderr=devnull, cwd=project_dir
             )
             version = version.rstrip()
         if hasattr(version, "decode"):
             version = version.decode("utf-8")
         print(f"{sys.argv[0]} version {version}")
 
-    @classmethod
-    def print_help(cls):
+    @staticmethod
+    def _print_help(converter: type[Converter]) -> None:
+        """Prints help text to cli."""
         print(
             "{cmd} [-v] list|<{name}-number>|<{name}-name>".format(
-                cmd=sys.argv[0], name=cls.NAME
+                cmd=sys.argv[0], name=converter.NAME
             )
         )
 
-    @classmethod
-    def convert(cls, number=None, code=None, verbose=False):
-        """
-        :param int number:
-        :param str code:
-        :param bool verbose:
-        :rtype: str
-        """
-        n = cls.code2number(code) if number is None else number
-        c = cls.number2code(number) if code is None else code
+    @staticmethod
+    def _convert(
+        converter: type[Converter],
+        number: int | None = None,
+        code: str | None = None,
+        verbose: bool = False,
+    ) -> str:
+        n = (
+            converter.code2number(code)
+            if number is None and code is not None
+            else number
+        )
+        c = (
+            converter.number2code(number)
+            if number is not None and code is None
+            else code
+        )
+
+        if n is None or c is None:
+            raise Exception("Either number or code must be provided.")
 
         if verbose:
-            return "{n:3d} - {c:15}: {d}".format(n=n, c=c, d=cls.number2description(n))
-        else:
-            if code is None:
-                return c
-            elif number is None:
-                return str(n)
-            else:
-                return "{n:3d} - {c}".format(n=n, c=c)
+            return f"{n:3d} - {c:15}: {converter.number2description(n)}"
+
+        if code is None:
+            return c
+
+        if number is None:
+            return str(n)
+
+        return f"{n:3d} - {c}"
 
     @classmethod
-    def parse(cls):
+    def parse(cls, converter: type[Converter]) -> None:
+        """Parse cli arguments, convert code and print result."""
+
         if len(sys.argv) < 2:
-            cls.print_help()
+            cls._print_help(converter)
             exit()
 
-        invalids = dict()
+        invalids = {}
         verbose_option = sys.argv[1]
         if verbose_option == "-v":
             if len(sys.argv) < 3:
                 try:
-                    cls.print_version()
+                    cls._print_version()
                 except Exception as exc:
                     logger.error(f"Printing version (git tag) ommited due to: {exc}")
-                    cls.print_help()
+                    cls._print_help(converter)
                 exit()
             code_or_number = sys.argv[2]
         else:
             verbose_option = ""
             code_or_number = sys.argv[1]
 
         if code_or_number.lower() == "list":
-            for n in cls.NUMBER_RANGE:
+            for n in converter.NUMBER_RANGE:
                 try:
                     print(
-                        cls.convert(
+                        cls._convert(
+                            converter=converter,
                             number=n,
-                            code=cls.number2code(n),
+                            code=converter.number2code(n),
                             verbose=bool(verbose_option),
                         )
                     )
                 except Exception as e:
                     invalids[n] = e
 
         elif code_or_number.isdigit():
+            number = int(code_or_number)
             try:
                 print(
-                    cls.convert(
-                        number=int(code_or_number), verbose=bool(verbose_option)
+                    cls._convert(
+                        converter=converter, number=number, verbose=bool(verbose_option)
                     )
                 )
             except Exception as e:
-                invalids[code_or_number] = e
+                invalids[number] = e
 
         else:
             try:
-                print(cls.convert(code=code_or_number, verbose=bool(verbose_option)))
+                print(
+                    cls._convert(
+                        converter=converter,
+                        code=code_or_number,
+                        verbose=bool(verbose_option),
+                    )
+                )
             except Exception as e:
                 if verbose_option:
                     print(
                         "No {name} matched the input {i!r} ({e}). Try to match as re:".format(
-                            name=cls.NAME, i=code_or_number, e=e
+                            name=converter.NAME, i=code_or_number, e=e
                         ),
                         file=sys.stderr,
                     )
                 search = re.compile(code_or_number, flags=re.IGNORECASE)
-                for att in cls.get_candidates():
+                for att in converter.get_candidates():
                     try:
-                        number = cls.code2number(att)
-                        desc = cls.number2description(number)
+                        number = converter.code2number(att)
+                        desc = converter.number2description(number)
                         if (
                             search.search(att)
                             or search.search(str(number))
                             or search.search(desc)
                             and bool(verbose_option)
                         ):
                             print(
-                                cls.convert(
+                                cls._convert(
+                                    converter=converter,
                                     number=number,
                                     code=att,
                                     verbose=bool(verbose_option),
                                 )
                             )
                     except:
                         pass
 
         if invalids and verbose_option:
             if all(isinstance(e, (ValueError, KeyError)) for e in invalids.values()):
-                print("invalids: {}".format(set(invalids.keys())), file=sys.stderr)
+                print(f"invalids: {set(invalids.keys())}", file=sys.stderr)
             else:
-                print("invalids: {}".format(invalids), file=sys.stderr)
+                print(f"invalids: {invalids}", file=sys.stderr)
```

### Comparing `errno_converter-0.1.4/src/errno_converter.egg-info/PKG-INFO` & `errno_converter-0.1.5/src/errno_converter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: errno-converter
-Version: 0.1.4
+Version: 0.1.5
 Summary: As simple command line tool to convert error numbers (of C errno.h), http status codes and signal numbers to human readable strings or back zu numbers.
 Author-email: Heinrich Kießling <heinrich@kiess.link>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
```

### Comparing `errno_converter-0.1.4/src/errno_converter.py` & `errno_converter-0.1.5/src/errno_converter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-#!/usr/bin/env python3
-# coding=utf-8
 import os
 import errno
-from converter_lib import Converter
+
+from converter_lib import Converter, Parser
 
 
 class ErrnoConverter(Converter):
-    NAME = "errno"
-    NUMBER_RANGE = range(1, 132)
+    NAME: str = "errno"
+    NUMBER_RANGE: range = range(1, 132)
 
     @staticmethod
-    def number2code(number):
+    def number2code(number: int) -> str:
         return errno.errorcode[int(number)]
 
     @staticmethod
-    def code2number(code):
+    def code2number(code: str) -> int:
         return getattr(errno, code)
 
     @staticmethod
-    def get_candidates():
+    def get_candidates() -> list[str]:
         return dir(errno)
 
     @staticmethod
-    def number2description(number):
+    def number2description(number: int) -> str:
         return os.strerror(number)
 
 
-def main():
-    return ErrnoConverter.parse()
+def main() -> None:
+    return Parser.parse(ErrnoConverter)
```

### Comparing `errno_converter-0.1.4/src/http_converter.py` & `errno_converter-0.1.5/src/signal_converter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-#!/usr/bin/env python3
-# coding=utf-8
-import http
+import signal
+from typing import Sequence
 
-from converter_lib import Converter
+from converter_lib import Converter, Parser
 
 
-class HttpConverter(Converter):
-    NAME = "http"
-    NUMBER_RANGE = range(100, 600)
+class SignalConverter(Converter):
+    NAME: str = "signal"
+    NUMBER_RANGE: Sequence[int] = range(1, 65)
 
     @staticmethod
-    def number2code(number):
-        return http.HTTPStatus(int(number)).phrase
+    def number2code(number: int) -> str:
+        return signal.Signals(int(number)).name
 
     @staticmethod
-    def code2number(code):
-        return getattr(http.HTTPStatus, code).value
+    def code2number(code: str) -> int:
+        return getattr(signal, code).value
 
     @staticmethod
-    def get_candidates():
-        return dir(http.HTTPStatus)
+    def get_candidates() -> list[str]:
+        return dir(signal)
 
     @staticmethod
-    def number2description(number):
-        return http.HTTPStatus(int(number)).description
+    def number2description(number: int) -> str:
+        return signal.strsignal(signal.Signals(int(number))) or ""
 
 
-def main():
-    return HttpConverter.parse()
+def main() -> None:
+    return Parser.parse(SignalConverter)
```

