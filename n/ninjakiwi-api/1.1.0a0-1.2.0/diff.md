# Comparing `tmp/ninjakiwi_api-1.1.0a0.tar.gz` & `tmp/ninjakiwi_api-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninjakiwi_api-1.1.0a0.tar", max compression
+gzip compressed data, was "ninjakiwi_api-1.2.0.tar", max compression
```

## Comparing `ninjakiwi_api-1.1.0a0.tar` & `ninjakiwi_api-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1072 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/LICENSE
--rw-r--r--   0        0        0     2618 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/README.md
--rw-r--r--   0        0        0       84 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/API/BTD6/__init__.py
--rw-r--r--   0        0        0     6151 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/API/BTD6/function.py
--rw-r--r--   0        0        0       85 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/API/BTDB2/__init__.py
--rw-r--r--   0        0        0     2087 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/API/BTDB2/function.py
--rw-r--r--   0        0        0      184 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/API/__init__.py
--rw-r--r--   0        0        0      116 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/FUNCTIONS/ERROR/__init__.py
--rw-r--r--   0        0        0     1753 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/FUNCTIONS/ERROR/function.py
--rw-r--r--   0        0        0      108 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/FUNCTIONS/FETCH/__init__.py
--rw-r--r--   0        0        0     1063 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/FUNCTIONS/FETCH/function.py
--rw-r--r--   0        0        0     4640 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/FUNCTIONS/FETCH/model.py
--rw-r--r--   0        0        0      157 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/FUNCTIONS/__init__.py
--rw-r--r--   0        0        0      185 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/__init__.py
--rw-r--r--   0        0        0     3875 2023-07-22 11:39:10.148445 ninjakiwi_api-1.1.0a0/ninjakiwi_api/main.py
--rw-r--r--   0        0        0     2265 2023-07-22 11:39:10.152446 ninjakiwi_api-1.1.0a0/pyproject.toml
--rw-r--r--   0        0        0       43 2023-07-22 11:39:10.152446 ninjakiwi_api-1.1.0a0/tests/__init__.py
--rw-r--r--   0        0        0     5479 2023-07-22 11:39:10.152446 ninjakiwi_api-1.1.0a0/tests/test_btd6.py
--rw-r--r--   0        0        0     1142 2023-07-22 11:39:10.152446 ninjakiwi_api-1.1.0a0/tests/test_btdb2.py
--rw-r--r--   0        0        0     3584 2023-07-22 11:39:10.152446 ninjakiwi_api-1.1.0a0/tests/test_error.py
--rw-r--r--   0        0        0     3655 2023-07-22 11:39:10.152446 ninjakiwi_api-1.1.0a0/tests/test_fetch.py
--rw-r--r--   0        0        0     4915 2023-07-22 11:39:10.152446 ninjakiwi_api-1.1.0a0/tests/test_model.py
--rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 ninjakiwi_api-1.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2618 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/README.md
+-rw-r--r--   0        0        0       84 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/ninjakiwi_api/API/BTD6/__init__.py
+-rw-r--r--   0        0        0     6151 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/ninjakiwi_api/API/BTD6/function.py
+-rw-r--r--   0        0        0       85 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/ninjakiwi_api/API/BTDB2/__init__.py
+-rw-r--r--   0        0        0     2087 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/ninjakiwi_api/API/BTDB2/function.py
+-rw-r--r--   0        0        0      184 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/ninjakiwi_api/API/__init__.py
+-rw-r--r--   0        0        0      116 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/ninjakiwi_api/FUNCTIONS/ERROR/__init__.py
+-rw-r--r--   0        0        0     1753 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/ninjakiwi_api/FUNCTIONS/ERROR/function.py
+-rw-r--r--   0        0        0      108 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/ninjakiwi_api/FUNCTIONS/FETCH/__init__.py
+-rw-r--r--   0        0        0     1063 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/ninjakiwi_api/FUNCTIONS/FETCH/function.py
+-rw-r--r--   0        0        0     4640 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/ninjakiwi_api/FUNCTIONS/FETCH/model.py
+-rw-r--r--   0        0        0      157 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/ninjakiwi_api/FUNCTIONS/__init__.py
+-rw-r--r--   0        0        0      185 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/ninjakiwi_api/__init__.py
+-rw-r--r--   0        0        0     3875 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/ninjakiwi_api/main.py
+-rw-r--r--   0        0        0     2263 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     5479 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/tests/test_btd6.py
+-rw-r--r--   0        0        0     1142 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/tests/test_btdb2.py
+-rw-r--r--   0        0        0     3584 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/tests/test_error.py
+-rw-r--r--   0        0        0     3655 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/tests/test_fetch.py
+-rw-r--r--   0        0        0     4915 2023-07-22 12:14:09.735289 ninjakiwi_api-1.2.0/tests/test_model.py
+-rw-r--r--   0        0        0     4353 1970-01-01 00:00:00.000000 ninjakiwi_api-1.2.0/PKG-INFO
```

### Comparing `ninjakiwi_api-1.1.0a0/LICENSE` & `ninjakiwi_api-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.1.0a0/README.md` & `ninjakiwi_api-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.1.0a0/ninjakiwi_api/API/BTD6/function.py` & `ninjakiwi_api-1.2.0/ninjakiwi_api/API/BTD6/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.1.0a0/ninjakiwi_api/API/BTDB2/function.py` & `ninjakiwi_api-1.2.0/ninjakiwi_api/API/BTDB2/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.1.0a0/ninjakiwi_api/FUNCTIONS/ERROR/function.py` & `ninjakiwi_api-1.2.0/ninjakiwi_api/FUNCTIONS/ERROR/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.1.0a0/ninjakiwi_api/FUNCTIONS/FETCH/function.py` & `ninjakiwi_api-1.2.0/ninjakiwi_api/FUNCTIONS/FETCH/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.1.0a0/ninjakiwi_api/FUNCTIONS/FETCH/model.py` & `ninjakiwi_api-1.2.0/ninjakiwi_api/FUNCTIONS/FETCH/model.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.1.0a0/ninjakiwi_api/main.py` & `ninjakiwi_api-1.2.0/ninjakiwi_api/main.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.1.0a0/pyproject.toml` & `ninjakiwi_api-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "ninjakiwi_api"
-version = "1.1.0a0"
+version = "1.2.0"
 homepage = "https://github.com/GustavoSchip/ninjakiwi-api"
 description = "NinjaKiwi API (Open Data) for Python! (My first library)"
 authors = [
     "Gustavo Schip <gustavoschip@proton.me>",
 ]
 maintainers = [
     "Gustavo Schip <gustavoschip@proton.me>",
```

### Comparing `ninjakiwi_api-1.1.0a0/tests/test_btd6.py` & `ninjakiwi_api-1.2.0/tests/test_btd6.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.1.0a0/tests/test_btdb2.py` & `ninjakiwi_api-1.2.0/tests/test_btdb2.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.1.0a0/tests/test_error.py` & `ninjakiwi_api-1.2.0/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.1.0a0/tests/test_fetch.py` & `ninjakiwi_api-1.2.0/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.1.0a0/tests/test_model.py` & `ninjakiwi_api-1.2.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-1.1.0a0/PKG-INFO` & `ninjakiwi_api-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjakiwi-api
-Version: 1.1.0a0
+Version: 1.2.0
 Summary: NinjaKiwi API (Open Data) for Python! (My first library)
 Home-page: https://github.com/GustavoSchip/ninjakiwi-api
 License: MIT
 Keywords: API,NinjaKiwi
 Author: Gustavo Schip
 Author-email: gustavoschip@proton.me
 Maintainer: Gustavo Schip
```

