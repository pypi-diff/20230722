# Comparing `tmp/fondat_hubspot-4.1a1.tar.gz` & `tmp/fondat_hubspot-4.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fondat_hubspot-4.1a1.tar", max compression
+gzip compressed data, was "fondat_hubspot-4.1a2.tar", max compression
```

## Comparing `fondat_hubspot-4.1a1.tar` & `fondat_hubspot-4.1a2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1055 2023-03-23 00:18:59.445824 fondat_hubspot-4.1a1/LICENSE
--rw-r--r--   0        0        0      824 2023-03-23 00:16:09.583074 fondat_hubspot-4.1a1/README.md
--rw-r--r--   0        0        0       38 2023-03-23 00:20:20.218975 fondat_hubspot-4.1a1/fondat/hubspot/__init__.py
--rw-r--r--   0        0        0     4200 2023-06-02 03:39:50.424788 fondat_hubspot-4.1a1/fondat/hubspot/auth.py
--rw-r--r--   0        0        0     7603 2023-06-02 23:52:12.107015 fondat_hubspot-4.1a1/fondat/hubspot/client.py
--rw-r--r--   0        0        0      201 2023-06-02 19:41:42.605756 fondat_hubspot-4.1a1/fondat/hubspot/contacts/__init__.py
--rw-r--r--   0        0        0     4420 2023-06-03 00:00:58.858321 fondat_hubspot-4.1a1/fondat/hubspot/contacts/lists.py
--rw-r--r--   0        0        0      555 2023-05-30 05:35:22.827943 fondat_hubspot-4.1a1/fondat/hubspot/crm/__init__.py
--rw-r--r--   0        0        0    13080 2023-06-02 19:47:24.577196 fondat_hubspot-4.1a1/fondat/hubspot/crm/exports.py
--rw-r--r--   0        0        0     2253 2023-06-02 16:09:55.071083 fondat_hubspot-4.1a1/fondat/hubspot/crm/model.py
--rw-r--r--   0        0        0     5480 2023-06-03 00:00:58.851654 fondat_hubspot-4.1a1/fondat/hubspot/crm/objects.py
--rw-r--r--   0        0        0     1493 2023-06-02 15:59:10.268143 fondat_hubspot-4.1a1/fondat/hubspot/crm/owners.py
--rw-r--r--   0        0        0     3225 2023-06-02 19:47:24.500529 fondat_hubspot-4.1a1/fondat/hubspot/crm/pipelines.py
--rw-r--r--   0        0        0     1610 2023-06-02 18:03:10.729064 fondat_hubspot-4.1a1/fondat/hubspot/crm/properties.py
--rw-r--r--   0        0        0     1264 2023-06-02 18:30:15.700352 fondat_hubspot-4.1a1/fondat/hubspot/crm/schemas.py
--rw-r--r--   0        0        0      201 2023-05-16 22:20:53.537415 fondat_hubspot-4.1a1/fondat/hubspot/settings/__init__.py
--rw-r--r--   0        0        0     2313 2023-06-02 23:46:00.486675 fondat_hubspot-4.1a1/fondat/hubspot/settings/users.py
--rw-r--r--   0        0        0     1132 2023-06-03 02:48:40.285899 fondat_hubspot-4.1a1/pyproject.toml
--rw-r--r--   0        0        0     1683 1970-01-01 00:00:00.000000 fondat_hubspot-4.1a1/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-03-23 00:18:59.445824 fondat_hubspot-4.1a2/LICENSE
+-rw-r--r--   0        0        0      824 2023-03-23 00:16:09.583074 fondat_hubspot-4.1a2/README.md
+-rw-r--r--   0        0        0       38 2023-03-23 00:20:20.218975 fondat_hubspot-4.1a2/fondat/hubspot/__init__.py
+-rw-r--r--   0        0        0     7603 2023-07-22 00:07:34.629495 fondat_hubspot-4.1a2/fondat/hubspot/client.py
+-rw-r--r--   0        0        0      201 2023-06-02 19:41:42.605756 fondat_hubspot-4.1a2/fondat/hubspot/contacts/__init__.py
+-rw-r--r--   0        0        0     4420 2023-06-03 00:00:58.858321 fondat_hubspot-4.1a2/fondat/hubspot/contacts/lists.py
+-rw-r--r--   0        0        0      555 2023-05-30 05:35:22.827943 fondat_hubspot-4.1a2/fondat/hubspot/crm/__init__.py
+-rw-r--r--   0        0        0    13080 2023-06-02 19:47:24.577196 fondat_hubspot-4.1a2/fondat/hubspot/crm/exports.py
+-rw-r--r--   0        0        0     2253 2023-06-02 16:09:55.071083 fondat_hubspot-4.1a2/fondat/hubspot/crm/model.py
+-rw-r--r--   0        0        0     5480 2023-06-03 00:00:58.851654 fondat_hubspot-4.1a2/fondat/hubspot/crm/objects.py
+-rw-r--r--   0        0        0     1493 2023-06-02 15:59:10.268143 fondat_hubspot-4.1a2/fondat/hubspot/crm/owners.py
+-rw-r--r--   0        0        0     3225 2023-06-02 19:47:24.500529 fondat_hubspot-4.1a2/fondat/hubspot/crm/pipelines.py
+-rw-r--r--   0        0        0     1610 2023-06-02 18:03:10.729064 fondat_hubspot-4.1a2/fondat/hubspot/crm/properties.py
+-rw-r--r--   0        0        0     1264 2023-06-02 18:30:15.700352 fondat_hubspot-4.1a2/fondat/hubspot/crm/schemas.py
+-rw-r--r--   0        0        0     4188 2023-07-21 23:40:21.285524 fondat_hubspot-4.1a2/fondat/hubspot/oauth.py
+-rw-r--r--   0        0        0      201 2023-05-16 22:20:53.537415 fondat_hubspot-4.1a2/fondat/hubspot/settings/__init__.py
+-rw-r--r--   0        0        0     2313 2023-06-02 23:46:00.486675 fondat_hubspot-4.1a2/fondat/hubspot/settings/users.py
+-rw-r--r--   0        0        0     1132 2023-07-22 00:12:25.870989 fondat_hubspot-4.1a2/pyproject.toml
+-rw-r--r--   0        0        0     1632 1970-01-01 00:00:00.000000 fondat_hubspot-4.1a2/PKG-INFO
```

### Comparing `fondat_hubspot-4.1a1/LICENSE` & `fondat_hubspot-4.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1a1/README.md` & `fondat_hubspot-4.1a2/README.md`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1a1/fondat/hubspot/auth.py` & `fondat_hubspot-4.1a2/fondat/hubspot/oauth.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from urllib.parse import urlencode
 
 
 _AUTH_ENDPOINT = "https://app.hubspot.com/oauth/authorize"
 _TOKEN_ENDPOINT = "https://api.hubapi.com/oauth/v1/token"
 
 
-def generate_oauth_authorization_url(
+def generate_authorization_url(
     *,
     endpoint: str = _AUTH_ENDPOINT,
     client_id: str,
     scopes: list[str],
     redirect_uri: str,
     optional_scopes: list[str] | None = None,
     state: str | None = None,
@@ -42,15 +42,15 @@
     return (
         endpoint.rstrip("/")
         + "?"
         + urlencode({k: v for k, v in params.items() if v is not None})
     )
 
 
-async def request_oauth_refresh_token(
+async def request_refresh_token(
     *,
     session: aiohttp.ClientSession,
     endpoint: str = _TOKEN_ENDPOINT,
     client_id: str,
     client_secret: str,
     redirect_uri: str,
     code: str,
```

### Comparing `fondat_hubspot-4.1a1/fondat/hubspot/client.py` & `fondat_hubspot-4.1a2/fondat/hubspot/client.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1a1/fondat/hubspot/contacts/lists.py` & `fondat_hubspot-4.1a2/fondat/hubspot/contacts/lists.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1a1/fondat/hubspot/crm/__init__.py` & `fondat_hubspot-4.1a2/fondat/hubspot/crm/__init__.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1a1/fondat/hubspot/crm/exports.py` & `fondat_hubspot-4.1a2/fondat/hubspot/crm/exports.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1a1/fondat/hubspot/crm/model.py` & `fondat_hubspot-4.1a2/fondat/hubspot/crm/model.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1a1/fondat/hubspot/crm/objects.py` & `fondat_hubspot-4.1a2/fondat/hubspot/crm/objects.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1a1/fondat/hubspot/crm/owners.py` & `fondat_hubspot-4.1a2/fondat/hubspot/crm/owners.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1a1/fondat/hubspot/crm/pipelines.py` & `fondat_hubspot-4.1a2/fondat/hubspot/crm/pipelines.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1a1/fondat/hubspot/crm/properties.py` & `fondat_hubspot-4.1a2/fondat/hubspot/crm/properties.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1a1/fondat/hubspot/crm/schemas.py` & `fondat_hubspot-4.1a2/fondat/hubspot/crm/schemas.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1a1/fondat/hubspot/settings/users.py` & `fondat_hubspot-4.1a2/fondat/hubspot/settings/users.py`

 * *Files identical despite different names*

### Comparing `fondat_hubspot-4.1a1/pyproject.toml` & `fondat_hubspot-4.1a2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.black]
 line-length = 96
 target-version = ['py310']
 
 [tool.poetry]
 name = "fondat-hubspot"
-version = "4.1a1"
+version = "4.1a2"
 description = "Fondat package for HubSpot."
 readme = "README.md"
 authors = ["fondat-hubspot authors"]
 homepage = "https://github.com/fondat/fondat-hubspot/"
 documentation = "https://github.com/fondat/fondat-hubspot/wiki"
 license = "MIT"
 keywords = ["asgi", "framework", "resource", "openapi"]
@@ -22,24 +22,24 @@
     "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
 packages = [
     { include = "fondat" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.11"
 aiodns = "^3.0"
 aiohttp = "^3.8"
-fondat = "^4.1.3"
+fondat = "^4.1.9"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3"
 isort = "^5.12"
 pre-commit = "^3.3"
-pytest = "^7.3"
+pytest = "^7.4"
 pytest-asyncio = "^0.21"
 pytest-cov = "^4.1"
 
 [tool.isort]
 profile = "black"
 lexicographical = true
 lines_after_imports = 2
```

### Comparing `fondat_hubspot-4.1a1/PKG-INFO` & `fondat_hubspot-4.1a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: fondat-hubspot
-Version: 4.1a1
+Version: 4.1a2
 Summary: Fondat package for HubSpot.
 Home-page: https://github.com/fondat/fondat-hubspot/
 License: MIT
 Keywords: asgi,framework,resource,openapi
 Author: fondat-hubspot authors
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Dist: aiodns (>=3.0,<4.0)
 Requires-Dist: aiohttp (>=3.8,<4.0)
-Requires-Dist: fondat (>=4.1.3,<5.0.0)
+Requires-Dist: fondat (>=4.1.9,<5.0.0)
 Project-URL: Documentation, https://github.com/fondat/fondat-hubspot/wiki
 Description-Content-Type: text/markdown
 
 # fondat-hubspot
 
 [![PyPI](https://badge.fury.io/py/fondat-hubspot.svg)](https://badge.fury.io/py/fondat-hubspot)
 [![Python](https://img.shields.io/pypi/pyversions/fondat-hubspot)](https://python.org/)
```

