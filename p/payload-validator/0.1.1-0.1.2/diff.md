# Comparing `tmp/payload-validator-0.1.1.tar.gz` & `tmp/payload-validator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\payload-validator-0.1.1.tar", last modified: Sat Jul 22 08:33:36 2023, max compression
+gzip compressed data, was "dist\payload-validator-0.1.2.tar", last modified: Sat Jul 22 08:37:06 2023, max compression
```

## Comparing `payload-validator-0.1.1.tar` & `payload-validator-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 08:33:36.000000 payload-validator-0.1.1/
--rw-rw-rw-   0        0        0       74 2023-07-22 08:07:09.000000 payload-validator-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0    11818 2023-07-22 08:33:36.000000 payload-validator-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    11050 2023-07-22 08:32:26.000000 payload-validator-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-22 08:33:36.000000 payload-validator-0.1.1/payload_validator/
--rw-rw-rw-   0        0        0        0 2023-07-22 07:50:18.000000 payload-validator-0.1.1/payload_validator/__init__.py
--rw-rw-rw-   0        0        0      837 2023-07-22 05:40:00.000000 payload-validator-0.1.1/payload_validator/exceptions.py
--rw-rw-rw-   0        0        0     5084 2023-07-22 08:22:01.000000 payload-validator-0.1.1/payload_validator/validators.py
-drwxrwxrwx   0        0        0        0 2023-07-22 08:33:36.000000 payload-validator-0.1.1/payload_validator.egg-info/
--rw-rw-rw-   0        0        0    11818 2023-07-22 08:33:36.000000 payload-validator-0.1.1/payload_validator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-07-22 08:33:36.000000 payload-validator-0.1.1/payload_validator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 08:33:36.000000 payload-validator-0.1.1/payload_validator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-22 08:33:36.000000 payload-validator-0.1.1/payload_validator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      796 2023-07-22 08:33:36.000000 payload-validator-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0       68 2023-07-22 07:54:29.000000 payload-validator-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:37:06.000000 payload-validator-0.1.2/
+-rw-rw-rw-   0        0        0       74 2023-07-22 08:07:09.000000 payload-validator-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    11818 2023-07-22 08:37:06.000000 payload-validator-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11050 2023-07-22 08:32:26.000000 payload-validator-0.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-22 08:37:06.000000 payload-validator-0.1.2/payload_validator/
+-rw-rw-rw-   0        0        0        0 2023-07-22 07:50:18.000000 payload-validator-0.1.2/payload_validator/__init__.py
+-rw-rw-rw-   0        0        0      837 2023-07-22 05:40:00.000000 payload-validator-0.1.2/payload_validator/exceptions.py
+-rw-rw-rw-   0        0        0     5102 2023-07-22 08:36:39.000000 payload-validator-0.1.2/payload_validator/validators.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:37:06.000000 payload-validator-0.1.2/payload_validator.egg-info/
+-rw-rw-rw-   0        0        0    11818 2023-07-22 08:37:06.000000 payload-validator-0.1.2/payload_validator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-22 08:37:06.000000 payload-validator-0.1.2/payload_validator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 08:37:06.000000 payload-validator-0.1.2/payload_validator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-22 08:37:06.000000 payload-validator-0.1.2/payload_validator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      796 2023-07-22 08:37:06.000000 payload-validator-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0       68 2023-07-22 07:54:29.000000 payload-validator-0.1.2/setup.py
```

### Comparing `payload-validator-0.1.1/PKG-INFO` & `payload-validator-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payload-validator
-Version: 0.1.1
+Version: 0.1.2
 Summary: Validating payload datas for Python
 Home-page: https://github.com/cwadven/payload-validator
 Author: cwadven
 Author-email: cwadven4@gmail.com
 Maintainer: cwadven
 License: MIT
 Keywords: django random
```

### Comparing `payload-validator-0.1.1/README.rst` & `payload-validator-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `payload-validator-0.1.1/payload_validator/exceptions.py` & `payload-validator-0.1.2/payload_validator/exceptions.py`

 * *Files identical despite different names*

### Comparing `payload-validator-0.1.1/payload_validator/validators.py` & `payload-validator-0.1.2/payload_validator/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     Iterable,
     Optional,
     TypeVar,
     Union,
 )
 from types import FunctionType
 
-from exceptions import (
+from payload_validator.exceptions import (
     InvalidValueError,
     ValidationException,
     ValidationNotRunException,
 )
 
 
 T = TypeVar('T')  # Use TypeVar for arbitrary object types
```

### Comparing `payload-validator-0.1.1/payload_validator.egg-info/PKG-INFO` & `payload-validator-0.1.2/payload_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payload-validator
-Version: 0.1.1
+Version: 0.1.2
 Summary: Validating payload datas for Python
 Home-page: https://github.com/cwadven/payload-validator
 Author: cwadven
 Author-email: cwadven4@gmail.com
 Maintainer: cwadven
 License: MIT
 Keywords: django random
```

### Comparing `payload-validator-0.1.1/setup.cfg` & `payload-validator-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6179 6c6f 6164 2d76 616c 6964   = payload-valid
 00000020: 6174 6f72 0d0a 7665 7273 696f 6e20 3d20  ator..version = 
-00000030: 302e 312e 310d 0a61 7574 686f 7220 3d20  0.1.1..author = 
+00000030: 302e 312e 320d 0a61 7574 686f 7220 3d20  0.1.2..author = 
 00000040: 6377 6164 7665 6e0d 0a61 7574 686f 725f  cwadven..author_
 00000050: 656d 6169 6c20 3d20 6377 6164 7665 6e34  email = cwadven4
 00000060: 4067 6d61 696c 2e63 6f6d 0d0a 6d61 696e  @gmail.com..main
 00000070: 7461 696e 6572 203d 2063 7761 6476 656e  tainer = cwadven
 00000080: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000090: 5661 6c69 6461 7469 6e67 2070 6179 6c6f  Validating paylo
 000000a0: 6164 2064 6174 6173 2066 6f72 2050 7974  ad datas for Pyt
```

