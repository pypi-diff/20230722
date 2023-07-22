# Comparing `tmp/xapi-python-0.1.3.tar.gz` & `tmp/xapi-python-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xapi-python-0.1.3.tar", last modified: Thu May  4 10:12:39 2023, max compression
+gzip compressed data, was "xapi-python-0.1.4.tar", last modified: Sat Jul 22 08:34:57 2023, max compression
```

## Comparing `xapi-python-0.1.3.tar` & `xapi-python-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-05-04 10:12:39.830490 xapi-python-0.1.3/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1071 2023-04-25 04:51:26.000000 xapi-python-0.1.3/LICENSE
--rw-r--r--   0 pawel     (1000) pawel     (1000)     8203 2023-05-04 10:12:39.830490 xapi-python-0.1.3/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5898 2023-05-03 10:23:56.000000 xapi-python-0.1.3/README.md
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1131 2023-05-03 10:40:10.000000 xapi-python-0.1.3/pyproject.toml
--rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2023-05-04 10:12:39.830490 xapi-python-0.1.3/setup.cfg
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1027 2023-05-03 10:38:51.000000 xapi-python-0.1.3/setup.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-05-04 10:12:39.830490 xapi-python-0.1.3/tests/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5121 2023-05-02 15:09:32.000000 xapi-python-0.1.3/tests/test_connect.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     7958 2023-04-26 11:15:10.000000 xapi-python-0.1.3/tests/test_socket.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4014 2023-04-27 05:35:22.000000 xapi-python-0.1.3/tests/test_stream.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1566 2023-04-29 10:20:03.000000 xapi-python-0.1.3/tests/test_xapi.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-05-04 10:12:39.830490 xapi-python-0.1.3/xapi/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      338 2023-05-03 10:39:00.000000 xapi-python-0.1.3/xapi/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2228 2023-05-03 10:23:56.000000 xapi-python-0.1.3/xapi/connection.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1464 2023-04-24 14:52:49.000000 xapi-python-0.1.3/xapi/enums.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      205 2023-04-29 11:41:41.000000 xapi-python-0.1.3/xapi/exceptions.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     6640 2023-04-29 11:38:37.000000 xapi-python-0.1.3/xapi/socket.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2947 2023-04-29 11:39:31.000000 xapi-python-0.1.3/xapi/stream.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2209 2023-05-03 10:23:56.000000 xapi-python-0.1.3/xapi/xapi.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-05-04 10:12:39.830490 xapi-python-0.1.3/xapi_python.egg-info/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     8203 2023-05-04 10:12:39.000000 xapi-python-0.1.3/xapi_python.egg-info/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)      410 2023-05-04 10:12:39.000000 xapi-python-0.1.3/xapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2023-05-04 10:12:39.000000 xapi-python-0.1.3/xapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       19 2023-05-04 10:12:39.000000 xapi-python-0.1.3/xapi_python.egg-info/requires.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        5 2023-05-04 10:12:39.000000 xapi-python-0.1.3/xapi_python.egg-info/top_level.txt
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-07-22 08:34:57.284159 xapi-python-0.1.4/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1071 2023-04-25 04:51:26.000000 xapi-python-0.1.4/LICENSE
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     8259 2023-07-22 08:34:57.284159 xapi-python-0.1.4/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5954 2023-06-18 12:21:54.000000 xapi-python-0.1.4/README.md
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1131 2023-07-22 07:56:03.000000 xapi-python-0.1.4/pyproject.toml
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2023-07-22 08:34:57.284159 xapi-python-0.1.4/setup.cfg
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1027 2023-07-22 07:55:48.000000 xapi-python-0.1.4/setup.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-07-22 08:34:57.284159 xapi-python-0.1.4/tests/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5564 2023-07-22 08:34:28.000000 xapi-python-0.1.4/tests/test_connect.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     7958 2023-04-26 11:15:10.000000 xapi-python-0.1.4/tests/test_socket.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4014 2023-04-27 05:35:22.000000 xapi-python-0.1.4/tests/test_stream.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1566 2023-04-29 10:20:03.000000 xapi-python-0.1.4/tests/test_xapi.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-07-22 08:34:57.284159 xapi-python-0.1.4/xapi/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      338 2023-07-22 07:58:35.000000 xapi-python-0.1.4/xapi/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2355 2023-07-22 08:29:02.000000 xapi-python-0.1.4/xapi/connection.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1464 2023-04-24 14:52:49.000000 xapi-python-0.1.4/xapi/enums.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      205 2023-04-29 11:41:41.000000 xapi-python-0.1.4/xapi/exceptions.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     6640 2023-04-29 11:38:37.000000 xapi-python-0.1.4/xapi/socket.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2947 2023-04-29 11:39:31.000000 xapi-python-0.1.4/xapi/stream.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2209 2023-05-03 10:23:56.000000 xapi-python-0.1.4/xapi/xapi.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-07-22 08:34:57.284159 xapi-python-0.1.4/xapi_python.egg-info/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     8259 2023-07-22 08:34:57.000000 xapi-python-0.1.4/xapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      410 2023-07-22 08:34:57.000000 xapi-python-0.1.4/xapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2023-07-22 08:34:57.000000 xapi-python-0.1.4/xapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       19 2023-07-22 08:34:57.000000 xapi-python-0.1.4/xapi_python.egg-info/requires.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        5 2023-07-22 08:34:57.000000 xapi-python-0.1.4/xapi_python.egg-info/top_level.txt
```

### Comparing `xapi-python-0.1.3/LICENSE` & `xapi-python-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.3/PKG-INFO` & `xapi-python-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xapi-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: The xStation5 API Python library
 Home-page: https://github.com/pawelkn/xapi-python
 Author: Paweł Knioła
 Author-email: Paweł Knioła <pawel.kn@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Paweł Knioła
@@ -220,8 +220,8 @@
 git clone https://github.com/pawelkn/xapi-python.git
 cd xapi-python
 python3 -m unittest discover tests
 ```
 
 ## Buy Me A Coffee! ☕
 
-If you find the project beneficial and would like to support me, please consider showing your appreciation by buying me a coffee on [BuyMeACoffee](https://www.buymeacoffee.com/pawelkn)
+If you find the project beneficial and would like to support me, please consider showing your appreciation by buying me a coffee on [Buy Me A Coffee](https://www.buymeacoffee.com/pawelkn) or [Buy Coffee Poland](https://buycoffee.to/pawelkn)
```

### Comparing `xapi-python-0.1.3/README.md` & `xapi-python-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -176,8 +176,8 @@
 git clone https://github.com/pawelkn/xapi-python.git
 cd xapi-python
 python3 -m unittest discover tests
 ```
 
 ## Buy Me A Coffee! ☕
 
-If you find the project beneficial and would like to support me, please consider showing your appreciation by buying me a coffee on [BuyMeACoffee](https://www.buymeacoffee.com/pawelkn)
+If you find the project beneficial and would like to support me, please consider showing your appreciation by buying me a coffee on [Buy Me A Coffee](https://www.buymeacoffee.com/pawelkn) or [Buy Coffee Poland](https://buycoffee.to/pawelkn)
```

### Comparing `xapi-python-0.1.3/pyproject.toml` & `xapi-python-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xapi-python"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Paweł Knioła", email="pawel.kn@gmail.com" },
 ]
 description = "The xStation5 API Python library"
 keywords = [
   "python", "python3", "bitcoin", "trading", "websocket", "trading-api", "forex", "xapi", "forex-trading",
   "exchange-api", "forex-data", "xstation", "xstation5", "xtb", "xopenhub", "forex-api", "xopenhub-api",
```

### Comparing `xapi-python-0.1.3/setup.py` & `xapi-python-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,10 +16,10 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12"
     ],
     python_requires='>=3.7',
-    version="0.1.3",
+    version="0.1.4",
     packages=['xapi'],
 )
```

### Comparing `xapi-python-0.1.3/tests/test_connect.py` & `xapi-python-0.1.4/tests/test_connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,22 @@
 import json
 import asyncio
 
 from xapi import Connection, ConnectionClosed
 
 class TestConnection(unittest.IsolatedAsyncioTestCase):
 
+    async def test_connect_websocket_exception(self):
+        c = Connection()
+        with patch("websockets.client.connect", new_callable=AsyncMock) as mocked_connect:
+            mocked_connect.side_effect = websockets.exceptions.WebSocketException()
+            with self.assertRaises(ConnectionClosed) as cm:
+                await c.connect("ws://127.0.0.1:9000")
+            self.assertEqual(str(cm.exception), "WebSocket exception: ")
+
     async def test_connect_socket_gaierror(self):
         c = Connection()
         with patch("websockets.client.connect", new_callable=AsyncMock) as mocked_connect:
             mocked_connect.side_effect = socket.gaierror()
             with self.assertRaises(ConnectionClosed) as cm:
                 await c.connect("ws://127.0.0.1:9000")
             self.assertEqual(str(cm.exception), "Hostname cannot be resolved")
```

### Comparing `xapi-python-0.1.3/tests/test_socket.py` & `xapi-python-0.1.4/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.3/tests/test_stream.py` & `xapi-python-0.1.4/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.3/tests/test_xapi.py` & `xapi-python-0.1.4/tests/test_xapi.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.3/xapi/connection.py` & `xapi-python-0.1.4/xapi/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,17 @@
         self._conn = None
         self._lock = asyncio.Lock()
 
     async def connect(self, url):
         try:
             self._conn = await websockets.client.connect(url, close_timeout=0, max_size=None)
 
+        except websockets.exceptions.WebSocketException as e:
+            raise ConnectionClosed(f"WebSocket exception: {e}")
+
         except socket.gaierror:
             raise ConnectionClosed("Hostname cannot be resolved")
 
         except asyncio.exceptions.TimeoutError:
             raise ConnectionClosed("Connection timed out")
 
         except ConnectionRefusedError:
```

### Comparing `xapi-python-0.1.3/xapi/enums.py` & `xapi-python-0.1.4/xapi/enums.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.3/xapi/socket.py` & `xapi-python-0.1.4/xapi/socket.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.3/xapi/stream.py` & `xapi-python-0.1.4/xapi/stream.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.3/xapi/xapi.py` & `xapi-python-0.1.4/xapi/xapi.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.3/xapi_python.egg-info/PKG-INFO` & `xapi-python-0.1.4/xapi_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xapi-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: The xStation5 API Python library
 Home-page: https://github.com/pawelkn/xapi-python
 Author: Paweł Knioła
 Author-email: Paweł Knioła <pawel.kn@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Paweł Knioła
@@ -220,8 +220,8 @@
 git clone https://github.com/pawelkn/xapi-python.git
 cd xapi-python
 python3 -m unittest discover tests
 ```
 
 ## Buy Me A Coffee! ☕
 
-If you find the project beneficial and would like to support me, please consider showing your appreciation by buying me a coffee on [BuyMeACoffee](https://www.buymeacoffee.com/pawelkn)
+If you find the project beneficial and would like to support me, please consider showing your appreciation by buying me a coffee on [Buy Me A Coffee](https://www.buymeacoffee.com/pawelkn) or [Buy Coffee Poland](https://buycoffee.to/pawelkn)
```

