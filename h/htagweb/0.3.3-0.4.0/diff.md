# Comparing `tmp/htagweb-0.3.3.tar.gz` & `tmp/htagweb-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagweb-0.3.3.tar", max compression
+gzip compressed data, was "htagweb-0.4.0.tar", max compression
```

## Comparing `htagweb-0.3.3.tar` & `htagweb-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0     1065 2023-07-18 07:00:12.071597 htagweb-0.3.3/LICENSE
--rw-r--r--   0        0        0     3148 2023-07-18 07:00:12.071597 htagweb-0.3.3/README.md
--rw-r--r--   0        0        0     9938 2023-07-18 07:00:12.351596 htagweb-0.3.3/htagweb/__init__.py
--rw-r--r--   0        0        0     2225 2023-07-18 07:00:12.071597 htagweb-0.3.3/htagweb/crypto.py
--rw-r--r--   0        0        0     3794 2023-07-18 07:00:12.071597 htagweb-0.3.3/htagweb/manager.py
--rw-r--r--   0        0        0     5541 2023-07-18 07:00:12.071597 htagweb-0.3.3/htagweb/uidprocess.py
--rw-r--r--   0        0        0     1124 2023-07-18 07:00:12.351596 htagweb-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     4350 1970-01-01 00:00:00.000000 htagweb-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-22 08:59:17.604581 htagweb-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3148 2023-07-22 08:59:17.604581 htagweb-0.4.0/README.md
+-rw-r--r--   0        0        0      518 2023-07-22 08:59:18.008585 htagweb-0.4.0/htagweb/__init__.py
+-rw-r--r--   0        0        0      421 2023-07-22 08:59:17.604581 htagweb-0.4.0/htagweb/__main__.py
+-rw-r--r--   0        0        0     2521 2023-07-22 08:59:17.604581 htagweb-0.4.0/htagweb/crypto.py
+-rw-r--r--   0        0        0    10107 2023-07-22 08:59:17.608581 htagweb-0.4.0/htagweb/htagserver.py
+-rw-r--r--   0        0        0     3797 2023-07-22 08:59:17.608581 htagweb-0.4.0/htagweb/manager.py
+-rw-r--r--   0        0        0     5543 2023-07-22 08:59:17.608581 htagweb-0.4.0/htagweb/uidprocess.py
+-rw-r--r--   0        0        0     9904 2023-07-22 08:59:17.608581 htagweb-0.4.0/htagweb/webbase.py
+-rw-r--r--   0        0        0     1124 2023-07-22 08:59:18.008585 htagweb-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4350 1970-01-01 00:00:00.000000 htagweb-0.4.0/PKG-INFO
```

### Comparing `htagweb-0.3.3/LICENSE` & `htagweb-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `htagweb-0.3.3/README.md` & `htagweb-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `htagweb-0.3.3/htagweb/__init__.py` & `htagweb-0.4.0/htagweb/webbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 # #############################################################################
 # Copyright (C) 2023 manatlan manatlan[at]gmail(dot)com
 #
 # MIT licence
 #
-# https://github.com/manatlan/htag
+# https://github.com/manatlan/htagweb
 # #############################################################################
 
-__version__ = "0.3.3" # auto updated
 
 """
 WebServer & WebServerWS
 ~~~~~~~~~~~~~~~~~~~~~~~~
 - new versions of oldest WebHTTP & WebWS (nearly compatibles)
 - concept of an htag app application server (manager), which communicate with child process, with queue
 - Htag Apps runned in a process, per user (real isolation!)
```

### Comparing `htagweb-0.3.3/htagweb/crypto.py` & `htagweb-0.4.0/htagweb/crypto.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# -*- coding: utf-8 -*-
+# #############################################################################
+# Copyright (C) 2023 manatlan manatlan[at]gmail(dot)com
+#
+# MIT licence
+#
+# https://github.com/manatlan/htagweb
+# #############################################################################
 from Cryptodome.Cipher import AES # pip3 install pycryptodomex
 import hashlib
 import base64,os
 # https://hackernoon.com/how-to-use-aes-256-cipher-python-cryptography-examples-6tbh37cr
 
 def decrypt(b64:bytes,key:str) -> bytes:   # text
     data=base64.b64decode(b64)
```

### Comparing `htagweb-0.3.3/htagweb/manager.py` & `htagweb-0.4.0/htagweb/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # #############################################################################
 # Copyright (C) 2023 manatlan manatlan[at]gmail(dot)com
 #
 # MIT licence
 #
-# https://github.com/manatlan/htag
+# https://github.com/manatlan/htagweb
 # #############################################################################
 import asyncio
 import logging,pickle
 
 logger = logging.getLogger(__name__)
 
 async def manager_server(reader, writer):
```

### Comparing `htagweb-0.3.3/htagweb/uidprocess.py` & `htagweb-0.4.0/htagweb/uidprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # #############################################################################
 # Copyright (C) 2023 manatlan manatlan[at]gmail(dot)com
 #
 # MIT licence
 #
-# https://github.com/manatlan/htag
+# https://github.com/manatlan/htagweb
 # #############################################################################
 import asyncio,sys
 import multiprocessing
 import logging,importlib
 from htag.render import HRenderer
 from shared_memory_dict import SharedMemoryDict
 
@@ -39,15 +39,15 @@
                 names = fqn.split(".")
                 modulename,name=".".join(names[:-1]), names[-1]
                 if modulename in sys.modules:
                     module=sys.modules[modulename]
                     try:
                         module=importlib.reload( module )
                     except ModuleNotFoundError:
-                        """ can't be (really) reloaded if the component is in the 
+                        """ can't be (really) reloaded if the component is in the
                         same module as the instance htag server"""
                         pass
                 else:
                     module=importlib.import_module(modulename)
                 #---------------------------
                 htClass = getattr(module,name)
```

### Comparing `htagweb-0.3.3/pyproject.toml` & `htagweb-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagweb"
-version = "0.3.3" # auto-updated
+version = "0.4.0" # auto-updated
 description = "It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','webserver']
 homepage = "https://github.com/manatlan/htagweb"
 repository = "https://github.com/manatlan/htagweb"
```

### Comparing `htagweb-0.3.3/PKG-INFO` & `htagweb-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagweb
-Version: 0.3.3
+Version: 0.4.0
 Summary: It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)
 Home-page: https://github.com/manatlan/htagweb
 License: MIT
 Keywords: htag,webserver
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.8,<4.0
```

