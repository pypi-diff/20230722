# Comparing `tmp/ninjakiwi_api-0.0.7.tar.gz` & `tmp/ninjakiwi_api-1.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninjakiwi_api-0.0.7.tar", max compression
+gzip compressed data, was "ninjakiwi_api-1.1.0a0.tar", max compression
```

## Comparing `ninjakiwi_api-0.0.7.tar` & `ninjakiwi_api-1.1.0a0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
--rw-r--r--   0        0        0     1072 2023-07-19 16:03:17.395151 ninjakiwi_api-0.0.7/LICENSE
--rw-r--r--   0        0        0      825 2023-07-20 12:55:39.295946 ninjakiwi_api-0.0.7/README.md
--rw-r--r--   0        0        0       84 2023-07-20 11:13:18.959090 ninjakiwi_api-0.0.7/ninjakiwi_api/API/BTD6/__init__.py
--rw-r--r--   0        0        0     3002 2023-07-20 11:13:18.975757 ninjakiwi_api-0.0.7/ninjakiwi_api/API/BTD6/function.py
--rw-r--r--   0        0        0       85 2023-07-20 11:13:18.942423 ninjakiwi_api-0.0.7/ninjakiwi_api/API/BTDB2/__init__.py
--rw-r--r--   0        0        0     1085 2023-07-20 11:13:18.939090 ninjakiwi_api-0.0.7/ninjakiwi_api/API/BTDB2/function.py
--rw-r--r--   0        0        0      184 2023-07-20 11:13:18.949090 ninjakiwi_api-0.0.7/ninjakiwi_api/API/__init__.py
--rw-r--r--   0        0        0      116 2023-07-20 11:38:30.257333 ninjakiwi_api-0.0.7/ninjakiwi_api/FUNCTIONS/ERROR/__init__.py
--rw-r--r--   0        0        0     1807 2023-07-20 10:44:10.487649 ninjakiwi_api-0.0.7/ninjakiwi_api/FUNCTIONS/ERROR/function.py
--rw-r--r--   0        0        0      108 2023-07-20 11:38:30.260666 ninjakiwi_api-0.0.7/ninjakiwi_api/FUNCTIONS/FETCH/__init__.py
--rw-r--r--   0        0        0      746 2023-07-20 11:43:09.057477 ninjakiwi_api-0.0.7/ninjakiwi_api/FUNCTIONS/FETCH/function.py
--rw-r--r--   0        0        0     1985 2023-07-20 13:13:15.256860 ninjakiwi_api-0.0.7/ninjakiwi_api/FUNCTIONS/FETCH/model.py
--rw-r--r--   0        0        0      157 2023-07-20 11:38:30.267333 ninjakiwi_api-0.0.7/ninjakiwi_api/FUNCTIONS/__init__.py
--rw-r--r--   0        0        0      185 2023-07-20 11:13:18.952423 ninjakiwi_api-0.0.7/ninjakiwi_api/__init__.py
--rw-r--r--   0        0        0     3109 2023-07-20 12:43:41.544888 ninjakiwi_api-0.0.7/ninjakiwi_api/main.py
--rw-r--r--   0        0        0     2158 2023-07-20 13:00:29.983891 ninjakiwi_api-0.0.7/pyproject.toml
--rw-r--r--   0        0        0       43 2023-07-19 16:03:17.421818 ninjakiwi_api-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0      806 2023-07-20 12:39:33.825683 ninjakiwi_api-0.0.7/tests/test_main.py
--rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 ninjakiwi_api-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/LICENSE
+-rw-r--r--   0        0        0     2618 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/README.md
+-rw-r--r--   0        0        0       84 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/API/BTD6/__init__.py
+-rw-r--r--   0        0        0     6151 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/API/BTD6/function.py
+-rw-r--r--   0        0        0       85 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/API/BTDB2/__init__.py
+-rw-r--r--   0        0        0     2087 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/API/BTDB2/function.py
+-rw-r--r--   0        0        0      184 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/API/__init__.py
+-rw-r--r--   0        0        0      116 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/FUNCTIONS/ERROR/__init__.py
+-rw-r--r--   0        0        0     1753 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/FUNCTIONS/ERROR/function.py
+-rw-r--r--   0        0        0      108 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/FUNCTIONS/FETCH/__init__.py
+-rw-r--r--   0        0        0     1063 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/FUNCTIONS/FETCH/function.py
+-rw-r--r--   0        0        0     4640 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/FUNCTIONS/FETCH/model.py
+-rw-r--r--   0        0        0      157 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/FUNCTIONS/__init__.py
+-rw-r--r--   0        0        0      185 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/__init__.py
+-rw-r--r--   0        0        0     3875 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/main.py
+-rw-r--r--   0        0        0     2265 2023-07-22 11:39:10.152446 ninjakiwi_api-1.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-07-22 11:39:10.152446 ninjakiwi_api-1.1.0a0/tests/__init__.py
+-rw-r--r--   0        0        0     5479 2023-07-22 11:39:10.152446 ninjakiwi_api-1.1.0a0/tests/test_btd6.py
+-rw-r--r--   0        0        0     1142 2023-07-22 11:39:10.152446 ninjakiwi_api-1.1.0a0/tests/test_btdb2.py
+-rw-r--r--   0        0        0     3584 2023-07-22 11:39:10.152446 ninjakiwi_api-1.1.0a0/tests/test_error.py
+-rw-r--r--   0        0        0     3655 2023-07-22 11:39:10.152446 ninjakiwi_api-1.1.0a0/tests/test_fetch.py
+-rw-r--r--   0        0        0     4915 2023-07-22 11:39:10.152446 ninjakiwi_api-1.1.0a0/tests/test_model.py
+-rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 ninjakiwi_api-1.1.0a0/PKG-INFO
```

### Comparing `ninjakiwi_api-0.0.7/LICENSE` & `ninjakiwi_api-1.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.7/ninjakiwi_api/FUNCTIONS/FETCH/function.py` & `ninjakiwi_api-1.1.0a0/ninjakiwi_api/FUNCTIONS/FETCH/function.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 """FUNCTION-level package for NinjaKiwi API."""
 
 from typing import Optional
 
 import aiohttp
 
 from ninjakiwi_api.FUNCTIONS.ERROR import _error_handler
-from ninjakiwi_api.FUNCTIONS.FETCH.model import _handler, _model
+from ninjakiwi_api.FUNCTIONS.FETCH.model import _handler, model
 
 
-async def _api_fetch(url: str) -> Optional[_model] | None:
+async def _api_fetch(url: str) -> Optional[model] | None:
     async with aiohttp.ClientSession() as session:
         async with session.get(url) as response:
             if response.status == 200:
                 data = await response.json()
-                try:
-                    return await _handler(data, response)
-                except Exception:
+                if data is not None:
+                    if data["success"]:
+                        try:
+                            return await _handler(data, response)
+                        except Exception:
+                            return await _error_handler(act="http", response=response)
+                    else:
+                        return await _error_handler(act="http", response=response)
+                else:
                     return await _error_handler(act="http", response=response)
             else:
                 return await _error_handler(act="http", response=response)
```

### Comparing `ninjakiwi_api-0.0.7/pyproject.toml` & `ninjakiwi_api-1.1.0a0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool]
 [tool.poetry]
 name = "ninjakiwi_api"
-version = "0.0.7"
-homepage = "https://github.com/GustavoSchip/ninjakiwi_api"
-description = "NinjaKiwi API (OpenDATA) for Python! (My first library)"
+version = "1.1.0a0"
+homepage = "https://github.com/GustavoSchip/ninjakiwi-api"
+description = "NinjaKiwi API (Open Data) for Python! (My first library)"
 authors = [
     "Gustavo Schip <gustavoschip@proton.me>",
 ]
 maintainers = [
     "Gustavo Schip <gustavoschip@proton.me>",
 ]
 readme = "README.md"
@@ -16,53 +16,55 @@
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Natural Language :: English',
     'Programming Language :: Python :: 3.11',
 ]
 keywords = [
-    "NinjaKiwi",
     "API",
+    "NinjaKiwi",
 ]
 packages = [
     { include = "ninjakiwi_api" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<4.0.0"
 
 asyncio  = {version = "^3.4.3"}
 aiohttp  = { version = "^3.8.1"}
-black  = { version = "^22.3.0", optional = true}
-isort  = { version = "5.10.1", optional = true}
-flake8  = { version = "4.0.1", optional = true}
+black  = { version = ">=22.3,<24.0", optional = true}
+isort  = { version = "5.12.0", optional = true}
+flake8  = { version = "6.0.0", optional = true}
 flake8-docstrings = { version = "^1.6.0", optional = true }
 pytest  = { version = "^7.0.1", optional = true}
 pytest-asyncio  = {version = "^0.21.1", optional = true}
-pytest-cov  = { version = "^3.0.0", optional = true}
-tox  = { version = "^3.24.5", optional = true}
+pytest-cov  = { version = ">=3,<5", optional = true}
+pytest-mock  = { version = "^3.11.1", optional = true}
+tox  = { version = ">=3.24.5,<5.0.0", optional = true}
 virtualenv  = { version = "^20.13.1", optional = true}
-pip  = { version = "^22.0.3"}
-twine  = { version = "^3.8.0", optional = true}
-pre-commit = {version = "^2.17.0", optional = true}
+pip  = { version = ">=22.0.3,<24.0.0"}
+twine  = { version = ">=3.8,<5.0", optional = true}
+pre-commit = {version = ">=2.17,<4.0", optional = true}
 toml = {version = "^0.10.2", optional = true}
 livereload = {version = "^2.6.3", optional = true}
 pyreadline = {version = "^2.1", optional = true}
 tornado = {version = "^6.2", optional = true}
 
 [tool.poetry.extras]
 test = [
     "pytest",
     "black",
     "isort",
     "flake8",
     "flake8-docstrings",
     "pytest-cov",
-    "pytest-asyncio"
+    "pytest-asyncio",
+    "pytest-mock"
     ]
 
 dev = ["tox", "pre-commit", "virtualenv", "pip", "twine", "toml"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

