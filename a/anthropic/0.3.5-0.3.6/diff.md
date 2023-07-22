# Comparing `tmp/anthropic-0.3.5.tar.gz` & `tmp/anthropic-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anthropic-0.3.5.tar", max compression
+gzip compressed data, was "anthropic-0.3.6.tar", max compression
```

## Comparing `anthropic-0.3.5.tar` & `anthropic-0.3.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1056 2023-06-26 21:50:36.624119 anthropic-0.3.5/LICENSE
--rw-r--r--   0        0        0     9665 2023-07-11 13:43:09.482168 anthropic-0.3.5/README.md
--rw-r--r--   0        0        0     1925 2023-07-20 00:08:54.643285 anthropic-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1999 2023-06-26 21:50:36.627612 anthropic-0.3.5/src/anthropic/__init__.py
--rw-r--r--   0        0        0    46809 2023-06-26 21:50:36.628016 anthropic-0.3.5/src/anthropic/_base_client.py
--rw-r--r--   0        0        0     3889 2023-06-26 21:50:36.628324 anthropic-0.3.5/src/anthropic/_base_exceptions.py
--rw-r--r--   0        0        0    15329 2023-06-26 21:50:36.628587 anthropic-0.3.5/src/anthropic/_client.py
--rw-r--r--   0        0        0      112 2023-06-26 21:50:36.628774 anthropic-0.3.5/src/anthropic/_constants.py
--rw-r--r--   0        0        0     1285 2023-06-26 21:50:36.628893 anthropic-0.3.5/src/anthropic/_exceptions.py
--rw-r--r--   0        0        0     7343 2023-06-26 21:50:36.629012 anthropic-0.3.5/src/anthropic/_models.py
--rw-r--r--   0        0        0     4846 2023-06-26 21:50:36.629146 anthropic-0.3.5/src/anthropic/_qs.py
--rw-r--r--   0        0        0      896 2023-06-26 21:50:36.629271 anthropic-0.3.5/src/anthropic/_resource.py
--rw-r--r--   0        0        0     7126 2023-06-26 21:50:36.629400 anthropic-0.3.5/src/anthropic/_streaming.py
--rw-r--r--   0        0        0     1186 2023-07-11 13:43:09.484957 anthropic-0.3.5/src/anthropic/_tokenizers.py
--rw-r--r--   0        0        0     4230 2023-06-26 21:50:36.629650 anthropic-0.3.5/src/anthropic/_types.py
--rw-r--r--   0        0        0     1277 2023-06-26 21:50:36.629824 anthropic-0.3.5/src/anthropic/_utils/__init__.py
--rw-r--r--   0        0        0     6710 2023-06-26 21:50:36.629952 anthropic-0.3.5/src/anthropic/_utils/_transform.py
--rw-r--r--   0        0        0     9411 2023-06-26 21:50:36.630107 anthropic-0.3.5/src/anthropic/_utils/_utils.py
--rw-r--r--   0        0        0      128 2023-07-20 00:08:54.643596 anthropic-0.3.5/src/anthropic/_version.py
--rw-r--r--   0        0        0      168 2023-06-26 21:50:36.630485 anthropic-0.3.5/src/anthropic/pagination.py
--rw-r--r--   0        0        0        0 2023-06-26 21:50:36.630566 anthropic-0.3.5/src/anthropic/py.typed
--rw-r--r--   0        0        0      156 2023-06-26 21:50:36.630819 anthropic-0.3.5/src/anthropic/resources/__init__.py
--rw-r--r--   0        0        0    21781 2023-07-19 23:00:27.618209 anthropic-0.3.5/src/anthropic/resources/completions.py
--rw-r--r--   0        0        0  1774213 2023-06-26 21:50:36.640575 anthropic-0.3.5/src/anthropic/tokenizer.json
--rw-r--r--   0        0        0      226 2023-06-26 21:50:36.640828 anthropic-0.3.5/src/anthropic/types/__init__.py
--rw-r--r--   0        0        0      664 2023-06-26 21:50:36.640952 anthropic-0.3.5/src/anthropic/types/completion.py
--rw-r--r--   0        0        0     7111 2023-07-19 23:00:27.618522 anthropic-0.3.5/src/anthropic/types/completion_create_params.py
--rw-r--r--   0        0        0    10618 1970-01-01 00:00:00.000000 anthropic-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-06-26 21:50:36.624119 anthropic-0.3.6/LICENSE
+-rw-r--r--   0        0        0     9649 2023-07-22 02:16:31.626443 anthropic-0.3.6/README.md
+-rw-r--r--   0        0        0     1925 2023-07-22 02:16:31.626782 anthropic-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     1999 2023-06-26 21:50:36.627612 anthropic-0.3.6/src/anthropic/__init__.py
+-rw-r--r--   0        0        0    46809 2023-06-26 21:50:36.628016 anthropic-0.3.6/src/anthropic/_base_client.py
+-rw-r--r--   0        0        0     3889 2023-06-26 21:50:36.628324 anthropic-0.3.6/src/anthropic/_base_exceptions.py
+-rw-r--r--   0        0        0    15329 2023-06-26 21:50:36.628587 anthropic-0.3.6/src/anthropic/_client.py
+-rw-r--r--   0        0        0      112 2023-06-26 21:50:36.628774 anthropic-0.3.6/src/anthropic/_constants.py
+-rw-r--r--   0        0        0     1285 2023-06-26 21:50:36.628893 anthropic-0.3.6/src/anthropic/_exceptions.py
+-rw-r--r--   0        0        0     7343 2023-06-26 21:50:36.629012 anthropic-0.3.6/src/anthropic/_models.py
+-rw-r--r--   0        0        0     4846 2023-06-26 21:50:36.629146 anthropic-0.3.6/src/anthropic/_qs.py
+-rw-r--r--   0        0        0      896 2023-06-26 21:50:36.629271 anthropic-0.3.6/src/anthropic/_resource.py
+-rw-r--r--   0        0        0     7126 2023-06-26 21:50:36.629400 anthropic-0.3.6/src/anthropic/_streaming.py
+-rw-r--r--   0        0        0     1186 2023-07-11 13:43:09.484957 anthropic-0.3.6/src/anthropic/_tokenizers.py
+-rw-r--r--   0        0        0     4230 2023-06-26 21:50:36.629650 anthropic-0.3.6/src/anthropic/_types.py
+-rw-r--r--   0        0        0     1277 2023-06-26 21:50:36.629824 anthropic-0.3.6/src/anthropic/_utils/__init__.py
+-rw-r--r--   0        0        0     6710 2023-06-26 21:50:36.629952 anthropic-0.3.6/src/anthropic/_utils/_transform.py
+-rw-r--r--   0        0        0     9411 2023-06-26 21:50:36.630107 anthropic-0.3.6/src/anthropic/_utils/_utils.py
+-rw-r--r--   0        0        0      128 2023-07-22 02:16:31.627239 anthropic-0.3.6/src/anthropic/_version.py
+-rw-r--r--   0        0        0      168 2023-06-26 21:50:36.630485 anthropic-0.3.6/src/anthropic/pagination.py
+-rw-r--r--   0        0        0        0 2023-06-26 21:50:36.630566 anthropic-0.3.6/src/anthropic/py.typed
+-rw-r--r--   0        0        0      156 2023-06-26 21:50:36.630819 anthropic-0.3.6/src/anthropic/resources/__init__.py
+-rw-r--r--   0        0        0    21781 2023-07-19 23:00:27.618209 anthropic-0.3.6/src/anthropic/resources/completions.py
+-rw-r--r--   0        0        0  1774213 2023-06-26 21:50:36.640575 anthropic-0.3.6/src/anthropic/tokenizer.json
+-rw-r--r--   0        0        0      226 2023-06-26 21:50:36.640828 anthropic-0.3.6/src/anthropic/types/__init__.py
+-rw-r--r--   0        0        0      664 2023-06-26 21:50:36.640952 anthropic-0.3.6/src/anthropic/types/completion.py
+-rw-r--r--   0        0        0     7111 2023-07-19 23:00:27.618522 anthropic-0.3.6/src/anthropic/types/completion_create_params.py
+-rw-r--r--   0        0        0    10602 1970-01-01 00:00:00.000000 anthropic-0.3.6/PKG-INFO
```

### Comparing `anthropic-0.3.5/LICENSE` & `anthropic-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.5/README.md` & `anthropic-0.3.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -176,21 +176,21 @@
 
 When the API returns a non-success status code (i.e., 4xx or 5xx
 response), a subclass of `anthropic.APIStatusError` will be raised, containing `status_code` and `response` properties.
 
 All errors inherit from `anthropic.APIError`.
 
 ```python
-from anthropic import Anthropic, HUMAN_PROMPT, AI_PROMPT
+import anthropic
 
-anthropic = Anthropic()
+client = anthropic.Anthropic()
 
 try:
-    anthropic.completions.create(
-        prompt=f"{HUMAN_PROMPT} Your prompt here {AI_PROMPT}",
+    client.completions.create(
+        prompt=f"{anthropic.HUMAN_PROMPT} Your prompt here {anthropic.AI_PROMPT}",
         max_tokens_to_sample=300,
         model="claude-2",
     )
 except anthropic.APIConnectionError as e:
     print("The server could not be reached")
     print(e.__cause__)  # an underlying Exception, likely raised within httpx.
 except anthropic.RateLimitError as e:
```

### Comparing `anthropic-0.3.5/pyproject.toml` & `anthropic-0.3.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anthropic"
-version = "0.3.5"
+version = "0.3.6"
 description = "Client library for the anthropic API"
 readme = "README.md"
 authors = ["Anthropic <support@anthropic.com>"]
 license = "MIT"
 repository = "https://github.com/anthropics/anthropic-sdk-python"
 packages = [
   { include = "anthropic", from = "src" }
```

### Comparing `anthropic-0.3.5/src/anthropic/__init__.py` & `anthropic-0.3.6/src/anthropic/__init__.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.5/src/anthropic/_base_client.py` & `anthropic-0.3.6/src/anthropic/_base_client.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.5/src/anthropic/_base_exceptions.py` & `anthropic-0.3.6/src/anthropic/_base_exceptions.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.5/src/anthropic/_client.py` & `anthropic-0.3.6/src/anthropic/_client.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.5/src/anthropic/_exceptions.py` & `anthropic-0.3.6/src/anthropic/_exceptions.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.5/src/anthropic/_models.py` & `anthropic-0.3.6/src/anthropic/_models.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.5/src/anthropic/_qs.py` & `anthropic-0.3.6/src/anthropic/_qs.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.5/src/anthropic/_resource.py` & `anthropic-0.3.6/src/anthropic/_resource.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.5/src/anthropic/_streaming.py` & `anthropic-0.3.6/src/anthropic/_streaming.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.5/src/anthropic/_tokenizers.py` & `anthropic-0.3.6/src/anthropic/_tokenizers.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.5/src/anthropic/_types.py` & `anthropic-0.3.6/src/anthropic/_types.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.5/src/anthropic/_utils/__init__.py` & `anthropic-0.3.6/src/anthropic/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.5/src/anthropic/_utils/_transform.py` & `anthropic-0.3.6/src/anthropic/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.5/src/anthropic/_utils/_utils.py` & `anthropic-0.3.6/src/anthropic/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.5/src/anthropic/resources/completions.py` & `anthropic-0.3.6/src/anthropic/resources/completions.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.5/src/anthropic/tokenizer.json` & `anthropic-0.3.6/src/anthropic/tokenizer.json`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.5/src/anthropic/types/completion.py` & `anthropic-0.3.6/src/anthropic/types/completion.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.5/src/anthropic/types/completion_create_params.py` & `anthropic-0.3.6/src/anthropic/types/completion_create_params.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.5/PKG-INFO` & `anthropic-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anthropic
-Version: 0.3.5
+Version: 0.3.6
 Summary: Client library for the anthropic API
 Home-page: https://github.com/anthropics/anthropic-sdk-python
 License: MIT
 Author: Anthropic
 Author-email: support@anthropic.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -201,21 +201,21 @@
 
 When the API returns a non-success status code (i.e., 4xx or 5xx
 response), a subclass of `anthropic.APIStatusError` will be raised, containing `status_code` and `response` properties.
 
 All errors inherit from `anthropic.APIError`.
 
 ```python
-from anthropic import Anthropic, HUMAN_PROMPT, AI_PROMPT
+import anthropic
 
-anthropic = Anthropic()
+client = anthropic.Anthropic()
 
 try:
-    anthropic.completions.create(
-        prompt=f"{HUMAN_PROMPT} Your prompt here {AI_PROMPT}",
+    client.completions.create(
+        prompt=f"{anthropic.HUMAN_PROMPT} Your prompt here {anthropic.AI_PROMPT}",
         max_tokens_to_sample=300,
         model="claude-2",
     )
 except anthropic.APIConnectionError as e:
     print("The server could not be reached")
     print(e.__cause__)  # an underlying Exception, likely raised within httpx.
 except anthropic.RateLimitError as e:
```

