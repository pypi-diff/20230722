# Comparing `tmp/ninjakiwi_api-1.2.0a0.tar.gz` & `tmp/ninjakiwi_api-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninjakiwi_api-1.2.0a0.tar", max compression
+gzip compressed data, was "ninjakiwi_api-1.2.1.tar", max compression
```

## Comparing `ninjakiwi_api-1.2.0a0.tar` & `ninjakiwi_api-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1072 2023-07-22 12:21:39.118850 ninjakiwi_api-1.2.0a0/LICENSE
--rw-r--r--   0        0        0     2618 2023-07-22 12:21:39.118850 ninjakiwi_api-1.2.0a0/README.md
--rw-r--r--   0        0        0       84 2023-07-22 12:21:39.118850 ninjakiwi_api-1.2.0a0/ninjakiwi_api/API/BTD6/__init__.py
--rw-r--r--   0        0        0     6151 2023-07-22 12:21:39.118850 ninjakiwi_api-1.2.0a0/ninjakiwi_api/API/BTD6/function.py
--rw-r--r--   0        0        0       85 2023-07-22 12:21:39.118850 ninjakiwi_api-1.2.0a0/ninjakiwi_api/API/BTDB2/__init__.py
--rw-r--r--   0        0        0     2087 2023-07-22 12:21:39.118850 ninjakiwi_api-1.2.0a0/ninjakiwi_api/API/BTDB2/function.py
--rw-r--r--   0        0        0      184 2023-07-22 12:21:39.118850 ninjakiwi_api-1.2.0a0/ninjakiwi_api/API/__init__.py
--rw-r--r--   0        0        0      116 2023-07-22 12:21:39.118850 ninjakiwi_api-1.2.0a0/ninjakiwi_api/FUNCTIONS/ERROR/__init__.py
--rw-r--r--   0        0        0     1753 2023-07-22 12:21:39.118850 ninjakiwi_api-1.2.0a0/ninjakiwi_api/FUNCTIONS/ERROR/function.py
--rw-r--r--   0        0        0      108 2023-07-22 12:21:39.118850 ninjakiwi_api-1.2.0a0/ninjakiwi_api/FUNCTIONS/FETCH/__init__.py
--rw-r--r--   0        0        0     1063 2023-07-22 12:21:39.118850 ninjakiwi_api-1.2.0a0/ninjakiwi_api/FUNCTIONS/FETCH/function.py
--rw-r--r--   0        0        0     4640 2023-07-22 12:21:39.118850 ninjakiwi_api-1.2.0a0/ninjakiwi_api/FUNCTIONS/FETCH/model.py
--rw-r--r--   0        0        0      157 2023-07-22 12:21:39.118850 ninjakiwi_api-1.2.0a0/ninjakiwi_api/FUNCTIONS/__init__.py
--rw-r--r--   0        0        0      185 2023-07-22 12:21:39.118850 ninjakiwi_api-1.2.0a0/ninjakiwi_api/__init__.py
--rw-r--r--   0        0        0     3875 2023-07-22 12:21:39.118850 ninjakiwi_api-1.2.0a0/ninjakiwi_api/main.py
--rw-r--r--   0        0        0     2265 2023-07-22 12:21:39.122850 ninjakiwi_api-1.2.0a0/pyproject.toml
--rw-r--r--   0        0        0       43 2023-07-22 12:21:39.122850 ninjakiwi_api-1.2.0a0/tests/__init__.py
--rw-r--r--   0        0        0     5479 2023-07-22 12:21:39.122850 ninjakiwi_api-1.2.0a0/tests/test_btd6.py
--rw-r--r--   0        0        0     1142 2023-07-22 12:21:39.122850 ninjakiwi_api-1.2.0a0/tests/test_btdb2.py
--rw-r--r--   0        0        0     3584 2023-07-22 12:21:39.122850 ninjakiwi_api-1.2.0a0/tests/test_error.py
--rw-r--r--   0        0        0     3655 2023-07-22 12:21:39.122850 ninjakiwi_api-1.2.0a0/tests/test_fetch.py
--rw-r--r--   0        0        0     4915 2023-07-22 12:21:39.122850 ninjakiwi_api-1.2.0a0/tests/test_model.py
--rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 ninjakiwi_api-1.2.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2618 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/README.md
+-rw-r--r--   0        0        0       84 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/ninjakiwi_api/API/BTD6/__init__.py
+-rw-r--r--   0        0        0     6151 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/ninjakiwi_api/API/BTD6/function.py
+-rw-r--r--   0        0        0       85 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/ninjakiwi_api/API/BTDB2/__init__.py
+-rw-r--r--   0        0        0     2087 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/ninjakiwi_api/API/BTDB2/function.py
+-rw-r--r--   0        0        0      184 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/ninjakiwi_api/API/__init__.py
+-rw-r--r--   0        0        0      116 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/ninjakiwi_api/FUNCTIONS/ERROR/__init__.py
+-rw-r--r--   0        0        0     1753 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/ninjakiwi_api/FUNCTIONS/ERROR/function.py
+-rw-r--r--   0        0        0      108 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/ninjakiwi_api/FUNCTIONS/FETCH/__init__.py
+-rw-r--r--   0        0        0     1080 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/ninjakiwi_api/FUNCTIONS/FETCH/function.py
+-rw-r--r--   0        0        0     5431 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/ninjakiwi_api/FUNCTIONS/FETCH/model.py
+-rw-r--r--   0        0        0      157 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/ninjakiwi_api/FUNCTIONS/__init__.py
+-rw-r--r--   0        0        0      185 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/ninjakiwi_api/__init__.py
+-rw-r--r--   0        0        0     3881 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/ninjakiwi_api/main.py
+-rw-r--r--   0        0        0     2263 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     5479 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/tests/test_btd6.py
+-rw-r--r--   0        0        0     1142 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/tests/test_btdb2.py
+-rw-r--r--   0        0        0     3584 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/tests/test_error.py
+-rw-r--r--   0        0        0     3655 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/tests/test_fetch.py
+-rw-r--r--   0        0        0     4964 2023-07-22 12:19:19.731328 ninjakiwi_api-1.2.1/tests/test_model.py
+-rw-r--r--   0        0        0     4353 1970-01-01 00:00:00.000000 ninjakiwi_api-1.2.1/PKG-INFO
```

### Comparing `ninjakiwi_api-1.2.0a0/LICENSE` & `ninjakiwi_api-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.2.0a0/README.md` & `ninjakiwi_api-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.2.0a0/ninjakiwi_api/API/BTD6/function.py` & `ninjakiwi_api-1.2.1/ninjakiwi_api/API/BTD6/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.2.0a0/ninjakiwi_api/API/BTDB2/function.py` & `ninjakiwi_api-1.2.1/ninjakiwi_api/API/BTDB2/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.2.0a0/ninjakiwi_api/FUNCTIONS/ERROR/function.py` & `ninjakiwi_api-1.2.1/ninjakiwi_api/FUNCTIONS/ERROR/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.2.0a0/ninjakiwi_api/FUNCTIONS/FETCH/function.py` & `ninjakiwi_api-1.2.1/ninjakiwi_api/FUNCTIONS/FETCH/function.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 import aiohttp
 
 from ninjakiwi_api.FUNCTIONS.ERROR import _error_handler
 from ninjakiwi_api.FUNCTIONS.FETCH.model import _handler, model
 
 
-async def _api_fetch(url: str) -> Optional[model] | None:
+async def _api_fetch(url: str, game: str) -> Optional[model] | None:
     async with aiohttp.ClientSession() as session:
         async with session.get(url) as response:
             if response.status == 200:
                 data = await response.json()
                 if data is not None:
                     if data["success"]:
                         try:
-                            return await _handler(data, response)
+                            return await _handler(data, response, game)
                         except Exception:
                             return await _error_handler(act="http", response=response)
                     else:
                         return await _error_handler(act="http", response=response)
                 else:
                     return await _error_handler(act="http", response=response)
             else:
```

### Comparing `ninjakiwi_api-1.2.0a0/ninjakiwi_api/FUNCTIONS/FETCH/model.py` & `ninjakiwi_api-1.2.1/ninjakiwi_api/FUNCTIONS/FETCH/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -72,14 +72,27 @@
                 for item in data:
                     results.extend(traverse(item, target_name))
             return results
 
         results = traverse(self._data, name)
         return results if results else None
 
+
+class btd6_model(model):
+    def __init__(self, data: dict, response: aiohttp.ClientResponse):
+        super().__init__(data, response)
+
+    async def get_user(self):
+        pass
+
+
+class btdb2_model(model):
+    def __init__(self, data: dict, response: aiohttp.ClientResponse):
+        super().__init__(data, response)
+
     async def get_homid(self, number: int) -> Union[str, None]:
         """
         Get the 'homid' (hashed object ID) at the specified index.
 
         Parameters
         ----------
         number : int
@@ -148,13 +161,28 @@
         """
         try:
             return await self.get_homid(2)
         except KeyError:
             return None
 
 
+async def _model_handler(
+    data: dict | None, response: aiohttp.ClientResponse | None, game: str | None
+) -> Optional[model] | None:
+    classes = {
+        "BTD6": btd6_model,
+        "BTDB2": btdb2_model,
+    }
+    if data is None or response is None or game is None:
+        return None
+    for key, value in classes.items():
+        if key == game:
+            return value(data, response)
+    return None
+
+
 async def _handler(
-    data: dict | None, response: aiohttp.ClientResponse | None
+    data: dict | None, response: aiohttp.ClientResponse | None, game: str | None
 ) -> Optional[model] | None:
-    if data is None or response is None:
+    if data is None or response is None or game is None:
         return None
-    return model(data, response)
+    return await _model_handler(data, response, game)
```

### Comparing `ninjakiwi_api-1.2.0a0/ninjakiwi_api/main.py` & `ninjakiwi_api-1.2.1/ninjakiwi_api/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,10 +93,10 @@
             print(f"Successfully fetched HOM leaderboard: {leaderboard}")
         else:
             print("Failed to fetch HOM leaderboard.")
     """
 
     url = await _game_to_func(game, data, **options)
     if url is not None:
-        return await _api_fetch(url)
+        return await _api_fetch(url, game)
     else:
         return None
```

### Comparing `ninjakiwi_api-1.2.0a0/pyproject.toml` & `ninjakiwi_api-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "ninjakiwi_api"
-version = "1.2.0a0"
+version = "1.2.1"
 homepage = "https://github.com/GustavoSchip/ninjakiwi-api"
 description = "NinjaKiwi API (Open Data) for Python! (My first library)"
 authors = [
     "Gustavo Schip <gustavoschip@proton.me>",
 ]
 maintainers = [
     "Gustavo Schip <gustavoschip@proton.me>",
```

### Comparing `ninjakiwi_api-1.2.0a0/tests/test_btd6.py` & `ninjakiwi_api-1.2.1/tests/test_btd6.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.2.0a0/tests/test_btdb2.py` & `ninjakiwi_api-1.2.1/tests/test_btdb2.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.2.0a0/tests/test_error.py` & `ninjakiwi_api-1.2.1/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.2.0a0/tests/test_fetch.py` & `ninjakiwi_api-1.2.1/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.2.0a0/tests/test_model.py` & `ninjakiwi_api-1.2.1/tests/test_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 """Tests for `ninjakiwi_api` package."""
 # pylint: disable=redefined-outer-name
 
 import pytest
 from aiohttp import test_utils
 
-from ninjakiwi_api.FUNCTIONS.FETCH.model import model
+from ninjakiwi_api.FUNCTIONS.FETCH.model import model, btd6_model, btdb2_model
 
 
 @pytest.mark.asyncio
 async def test_get_raw_data():
     """Test for get_raw_data"""
     data = {
         "name": "Test User",
@@ -67,15 +67,15 @@
         "leaderboard": "https://data.ninjakiwi.com/battles2/homs/season_12/leaderboard",
     }
 
     request = test_utils.make_mocked_request("GET", "/test")
     request.json = test_utils.make_mocked_coro(return_value=data)
     request.status = 200
 
-    my_model = model(data, request)
+    my_model = btdb2_model(data, request)
 
     homid_1 = await my_model.get_homid(0)
     assert homid_1 == "season_13"
 
     homid_2 = await my_model.get_homid(1)
     assert homid_2 is None
 
@@ -92,15 +92,15 @@
         "leaderboard": "https://data.ninjakiwi.com/battles2/homs/season_12/leaderboard",
     }
 
     request = test_utils.make_mocked_request("GET", "/test")
     request.json = test_utils.make_mocked_coro(return_value=data)
     request.status = 200
 
-    my_model = model(data, request)
+    my_model = btdb2_model(data, request)
 
     future_season = await my_model.get_next_season()
     assert future_season == "season_13"
 
 
 @pytest.mark.asyncio
 async def test_get_current_season():
@@ -124,15 +124,15 @@
         },
     ]
 
     request = test_utils.make_mocked_request("GET", "/test")
     request.json = test_utils.make_mocked_coro(return_value=data)
     request.status = 200
 
-    my_model = model(data, request)
+    my_model = btdb2_model(data, request)
 
     future_season = await my_model.get_current_season()
     assert future_season == "season_12"
 
 
 @pytest.mark.asyncio
 async def test_get_previous_season():
@@ -164,11 +164,11 @@
         },
     ]
 
     request = test_utils.make_mocked_request("GET", "/test")
     request.json = test_utils.make_mocked_coro(return_value=data)
     request.status = 200
 
-    my_model = model(data, request)
+    my_model = btdb2_model(data, request)
 
     future_season = await my_model.get_previous_season()
     assert future_season == "season_11"
```

### Comparing `ninjakiwi_api-1.2.0a0/PKG-INFO` & `ninjakiwi_api-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjakiwi-api
-Version: 1.2.0a0
+Version: 1.2.1
 Summary: NinjaKiwi API (Open Data) for Python! (My first library)
 Home-page: https://github.com/GustavoSchip/ninjakiwi-api
 License: MIT
 Keywords: API,NinjaKiwi
 Author: Gustavo Schip
 Author-email: gustavoschip@proton.me
 Maintainer: Gustavo Schip
```

