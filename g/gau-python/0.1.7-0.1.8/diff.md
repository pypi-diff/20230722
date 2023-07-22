# Comparing `tmp/gau-python-0.1.7.tar.gz` & `tmp/gau-python-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gau-python-0.1.7.tar", last modified: Thu Jan  5 01:37:42 2023, max compression
+gzip compressed data, was "gau-python-0.1.8.tar", last modified: Sat Jul 22 04:10:18 2023, max compression
```

## Comparing `gau-python-0.1.7.tar` & `gau-python-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 01:37:42.583654 gau-python-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-05 01:37:29.000000 gau-python-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-01-05 01:37:42.583654 gau-python-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-01-05 01:37:29.000000 gau-python-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 01:37:42.583654 gau-python-0.1.7/gau_python/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-01-05 01:37:29.000000 gau-python-0.1.7/gau_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-01-05 01:37:29.000000 gau-python-0.1.7/gau_python/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 01:37:42.583654 gau-python-0.1.7/gau_python/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 01:37:29.000000 gau-python-0.1.7/gau_python/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-01-05 01:37:29.000000 gau-python-0.1.7/gau_python/providers/commoncrawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-01-05 01:37:29.000000 gau-python-0.1.7/gau_python/providers/otx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-01-05 01:37:29.000000 gau-python-0.1.7/gau_python/providers/wayback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 01:37:42.583654 gau-python-0.1.7/gau_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-01-05 01:37:42.000000 gau-python-0.1.7/gau_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-01-05 01:37:42.000000 gau-python-0.1.7/gau_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 01:37:42.000000 gau-python-0.1.7/gau_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-05 01:37:42.000000 gau-python-0.1.7/gau_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-01-05 01:37:29.000000 gau-python-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 01:37:42.583654 gau-python-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:10:18.244298 gau-python-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-22 04:10:06.000000 gau-python-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-22 04:10:18.244298 gau-python-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-22 04:10:06.000000 gau-python-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:10:18.244298 gau-python-0.1.8/gau_python/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-22 04:10:06.000000 gau-python-0.1.8/gau_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-22 04:10:06.000000 gau-python-0.1.8/gau_python/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:10:18.244298 gau-python-0.1.8/gau_python/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 04:10:06.000000 gau-python-0.1.8/gau_python/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-22 04:10:06.000000 gau-python-0.1.8/gau_python/providers/commoncrawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-22 04:10:06.000000 gau-python-0.1.8/gau_python/providers/otx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-22 04:10:06.000000 gau-python-0.1.8/gau_python/providers/wayback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 04:10:18.244298 gau-python-0.1.8/gau_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-22 04:10:18.000000 gau-python-0.1.8/gau_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-22 04:10:18.000000 gau-python-0.1.8/gau_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 04:10:18.000000 gau-python-0.1.8/gau_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-22 04:10:18.000000 gau-python-0.1.8/gau_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-22 04:10:06.000000 gau-python-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 04:10:18.244298 gau-python-0.1.8/setup.cfg
```

### Comparing `gau-python-0.1.7/LICENSE` & `gau-python-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gau-python-0.1.7/PKG-INFO` & `gau-python-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gau-python
-Version: 0.1.7
+Version: 0.1.8
 Summary: Source: https://github.com/connor-marchand/gau-python
 Author-email: Connor Marchand <connor@connormarchand.com>
 Project-URL: Homepage, https://github.com/connor-marchand/gau-python
 Project-URL: Bug Tracker, https://github.com/connor-marchand/gau-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gau-python-0.1.7/README.md` & `gau-python-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `gau-python-0.1.7/gau_python/main.py` & `gau-python-0.1.8/gau_python/main.py`

 * *Files identical despite different names*

### Comparing `gau-python-0.1.7/gau_python/providers/commoncrawl.py` & `gau-python-0.1.8/gau_python/providers/commoncrawl.py`

 * *Files identical despite different names*

### Comparing `gau-python-0.1.7/gau_python/providers/otx.py` & `gau-python-0.1.8/gau_python/providers/wayback.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import json
 import logging
 
 import requests
 
-base_url = 'https://otx.alienvault.com/api/v1/indicators/hostname'
+base_url = "https://web.archive.org/cdx/search/cdx"
 
 
-def get_urls_otx(domain):
+def get_urls_wayback(domain):
     urls = []
-    page = 1
+    page = 0
     try:
         while True:
-            request_url = base_url + f'/{domain}/url_list?limit=100&page={str(page)}'
+            request_url = base_url + f'?url={domain}/*&output=json&collapse=urlkey&fl=original&page={page}'
             logging.info(f'GET {request_url}')
             response = requests.get(url=request_url)
-            response_json = json.loads(response.text)
-
-            for url_item in response_json["url_list"]:
-                urls.append(str(url_item["url"]))
-            if response_json['has_next']:
+            if len(response.text) > 0:
+                response_json = json.loads(response.text)
+                for url in response_json:
+                    urls.append(str(url[0]))
                 page += 1
             else:
                 break
 
     except requests.exceptions.Timeout:
         logging.error("requests.exceptions.Timeout: Timeout")
     except requests.exceptions.TooManyRedirects:
```

### Comparing `gau-python-0.1.7/gau_python/providers/wayback.py` & `gau-python-0.1.8/gau_python/providers/otx.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 import json
 import logging
 
 import requests
 
-base_url = "https://web.archive.org/cdx/search/cdx"
+base_urls = ['https://otx.alienvault.com/api/v1/indicators/hostname',
+             'https://otx.alienvault.com/api/v1/indicators/url',
+             'https://otx.alienvault.com/api/v1/indicators/domain']
 
 
-def get_urls_wayback(domain):
+def get_urls_otx(domain):
     urls = []
-    page = 0
     try:
-        while True:
-            request_url = base_url + f'?url={domain}/*&output=json&collapse=urlkey&fl=original&page={page}'
-            logging.info(f'GET {request_url}')
-            response = requests.get(url=request_url)
-            if len(response.text) > 0:
+        for base_url in base_urls:
+            page = 1
+            while True:
+                request_url = base_url + f'/{domain}/url_list?limit=100&page={str(page)}'
+                logging.info(f'GET {request_url}')
+                response = requests.get(url=request_url)
                 response_json = json.loads(response.text)
-                for url in response_json:
-                    urls.append(str(url[0]))
-                page += 1
-            else:
+
+                if 'url_list' not in response_json:
+                    for url_item in response_json["url_list"]:
+                        urls.append(str(url_item["url"]))
+                    if response_json['has_next']:
+                        page += 1
+                    else:
+                        break
                 break
 
     except requests.exceptions.Timeout:
         logging.error("requests.exceptions.Timeout: Timeout")
     except requests.exceptions.TooManyRedirects:
         logging.error("requests.exceptions.TooManyRedirects: Too many redirects. Try a different URL.")
     except requests.exceptions.RequestException:
```

### Comparing `gau-python-0.1.7/gau_python.egg-info/PKG-INFO` & `gau-python-0.1.8/gau_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gau-python
-Version: 0.1.7
+Version: 0.1.8
 Summary: Source: https://github.com/connor-marchand/gau-python
 Author-email: Connor Marchand <connor@connormarchand.com>
 Project-URL: Homepage, https://github.com/connor-marchand/gau-python
 Project-URL: Bug Tracker, https://github.com/connor-marchand/gau-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gau-python-0.1.7/pyproject.toml` & `gau-python-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["requests", "setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gau-python"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Connor Marchand", email="connor@connormarchand.com" },
 ]
 description = "Source: https://github.com/connor-marchand/gau-python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

