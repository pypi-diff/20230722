# Comparing `tmp/aiochris-0.3.0rc2.tar.gz` & `tmp/aiochris-0.3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiochris-0.3.0rc2.tar", max compression
+gzip compressed data, was "aiochris-0.3.0rc3.tar", max compression
```

## Comparing `aiochris-0.3.0rc2.tar` & `aiochris-0.3.0rc3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1069 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/LICENSE
--rw-r--r--   0        0        0     1738 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/README.md
--rw-r--r--   0        0        0      594 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/client/__init__.py
--rw-r--r--   0        0        0     6161 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/client/admin.py
--rw-r--r--   0        0        0     1335 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/client/anon.py
--rw-r--r--   0        0        0     9615 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/client/authed.py
--rw-r--r--   0        0        0     3718 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/client/base.py
--rw-r--r--   0        0        0     1695 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/client/normal.py
--rw-r--r--   0        0        0      644 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/enums.py
--rw-r--r--   0        0        0      698 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/errors.py
--rw-r--r--   0        0        0     2284 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/examples.md
--rw-r--r--   0        0        0     4811 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/home.md
--rw-r--r--   0        0        0       97 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/link/__init__.py
--rw-r--r--   0        0        0     1143 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/link/collection_client.py
--rw-r--r--   0        0        0     5027 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/link/http.py
--rw-r--r--   0        0        0     4659 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/link/linked.py
--rw-r--r--   0        0        0     1450 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/link/metaprog.py
--rw-r--r--   0        0        0        0 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/models/__init__.py
--rw-r--r--   0        0        0     1631 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/models/collection_links.py
--rw-r--r--   0        0        0     2898 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/models/data.py
--rw-r--r--   0        0        0     5047 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/models/logged_in.py
--rw-r--r--   0        0        0     1129 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/models/public.py
--rw-r--r--   0        0        0     3118 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/types.py
--rw-r--r--   0        0        0       31 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/util/__init__.py
--rw-r--r--   0        0        0     6932 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/aiochris/util/search.py
--rw-r--r--   0        0        0      785 2023-07-12 21:45:17.766044 aiochris-0.3.0rc2/pyproject.toml
--rw-r--r--   0        0        0     2364 1970-01-01 00:00:00.000000 aiochris-0.3.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/LICENSE
+-rw-r--r--   0        0        0     1738 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/README.md
+-rw-r--r--   0        0        0      594 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/client/__init__.py
+-rw-r--r--   0        0        0     6161 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/client/admin.py
+-rw-r--r--   0        0        0     1335 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/client/anon.py
+-rw-r--r--   0        0        0     9615 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/client/authed.py
+-rw-r--r--   0        0        0     3718 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/client/base.py
+-rw-r--r--   0        0        0     1695 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/client/normal.py
+-rw-r--r--   0        0        0      644 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/enums.py
+-rw-r--r--   0        0        0      788 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/errors.py
+-rw-r--r--   0        0        0     2284 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/examples.md
+-rw-r--r--   0        0        0     4811 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/home.md
+-rw-r--r--   0        0        0       97 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/link/__init__.py
+-rw-r--r--   0        0        0     1143 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/link/collection_client.py
+-rw-r--r--   0        0        0     5027 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/link/http.py
+-rw-r--r--   0        0        0     4659 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/link/linked.py
+-rw-r--r--   0        0        0     1450 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/link/metaprog.py
+-rw-r--r--   0        0        0        0 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/models/__init__.py
+-rw-r--r--   0        0        0     1631 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/models/collection_links.py
+-rw-r--r--   0        0        0     2898 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/models/data.py
+-rw-r--r--   0        0        0     5047 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/models/logged_in.py
+-rw-r--r--   0        0        0     1129 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/models/public.py
+-rw-r--r--   0        0        0     3118 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/types.py
+-rw-r--r--   0        0        0       31 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/util/__init__.py
+-rw-r--r--   0        0        0     6932 2023-07-13 00:03:54.280780 aiochris-0.3.0rc3/aiochris/util/search.py
+-rw-r--r--   0        0        0      785 2023-07-13 00:03:54.284780 aiochris-0.3.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     2364 1970-01-01 00:00:00.000000 aiochris-0.3.0rc3/PKG-INFO
```

### Comparing `aiochris-0.3.0rc2/LICENSE` & `aiochris-0.3.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/README.md` & `aiochris-0.3.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/aiochris/__init__.py` & `aiochris-0.3.0rc3/aiochris/__init__.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/aiochris/client/admin.py` & `aiochris-0.3.0rc3/aiochris/client/admin.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/aiochris/client/anon.py` & `aiochris-0.3.0rc3/aiochris/client/anon.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/aiochris/client/authed.py` & `aiochris-0.3.0rc3/aiochris/client/authed.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/aiochris/client/base.py` & `aiochris-0.3.0rc3/aiochris/client/base.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/aiochris/client/normal.py` & `aiochris-0.3.0rc3/aiochris/client/normal.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/aiochris/enums.py` & `aiochris-0.3.0rc3/aiochris/enums.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/aiochris/errors.py` & `aiochris-0.3.0rc3/aiochris/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,18 @@
     """
     Raises custom exceptions.
     """
     if res.status < 400:
         res.raise_for_status()
         return
     exception = BadRequestError if res.status < 500 else InternalServerError
-    raise exception(res.status, res.url, await res.json())
+    try:
+        raise exception(res.status, res.url, await res.json())
+    except aiohttp.ClientError:
+        raise exception(res.status, res.url)
 
 
 class BaseClientError(Exception):
     pass
 
 
 class ResponseError(BaseClientError):
```

### Comparing `aiochris-0.3.0rc2/aiochris/examples.md` & `aiochris-0.3.0rc3/aiochris/examples.md`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/aiochris/home.md` & `aiochris-0.3.0rc3/aiochris/home.md`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/aiochris/link/collection_client.py` & `aiochris-0.3.0rc3/aiochris/link/collection_client.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/aiochris/link/http.py` & `aiochris-0.3.0rc3/aiochris/link/http.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/aiochris/link/linked.py` & `aiochris-0.3.0rc3/aiochris/link/linked.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/aiochris/link/metaprog.py` & `aiochris-0.3.0rc3/aiochris/link/metaprog.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/aiochris/models/collection_links.py` & `aiochris-0.3.0rc3/aiochris/models/collection_links.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/aiochris/models/data.py` & `aiochris-0.3.0rc3/aiochris/models/data.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/aiochris/models/logged_in.py` & `aiochris-0.3.0rc3/aiochris/models/logged_in.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/aiochris/models/public.py` & `aiochris-0.3.0rc3/aiochris/models/public.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/aiochris/types.py` & `aiochris-0.3.0rc3/aiochris/types.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/aiochris/util/search.py` & `aiochris-0.3.0rc3/aiochris/util/search.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.3.0rc2/pyproject.toml` & `aiochris-0.3.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiochris"
-version = "0.3.0rc2"
+version = "0.3.0rc3"
 description = "ChRIS client built on aiohttp"
 authors = ["FNNDSC <dev@babyMRI.org>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `aiochris-0.3.0rc2/PKG-INFO` & `aiochris-0.3.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiochris
-Version: 0.3.0rc2
+Version: 0.3.0rc3
 Summary: ChRIS client built on aiohttp
 License: MIT
 Author: FNNDSC
 Author-email: dev@babyMRI.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

