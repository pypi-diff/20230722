# Comparing `tmp/openai_function_call-0.2.0.tar.gz` & `tmp/openai_function_call-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_function_call-0.2.0.tar", max compression
+gzip compressed data, was "openai_function_call-0.2.1.tar", max compression
```

## Comparing `openai_function_call-0.2.0.tar` & `openai_function_call-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1066 2023-07-17 13:01:37.119032 openai_function_call-0.2.0/LICENSE
--rw-r--r--   0        0        0     8394 2023-07-17 13:01:37.119032 openai_function_call-0.2.0/README.md
--rw-r--r--   0        0        0      187 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/openai_function_call/__init__.py
--rw-r--r--   0        0        0      151 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/openai_function_call/dsl/__init__.py
--rw-r--r--   0        0        0     5799 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/openai_function_call/dsl/completion.py
--rw-r--r--   0        0        0      505 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/openai_function_call/dsl/messages/__init__.py
--rw-r--r--   0        0        0     1669 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/openai_function_call/dsl/messages/base.py
--rw-r--r--   0        0        0     3260 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/openai_function_call/dsl/messages/messages.py
--rw-r--r--   0        0        0     1486 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/openai_function_call/dsl/messages/user.py
--rw-r--r--   0        0        0     2210 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/openai_function_call/dsl/multitask.py
--rw-r--r--   0        0        0     6330 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/openai_function_call/function_calls.py
--rw-r--r--   0        0        0      662 2023-07-17 13:01:37.127032 openai_function_call-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     9127 1970-01-01 00:00:00.000000 openai_function_call-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-22 16:07:42.134784 openai_function_call-0.2.1/LICENSE
+-rw-r--r--   0        0        0     8394 2023-07-22 16:07:42.134784 openai_function_call-0.2.1/README.md
+-rw-r--r--   0        0        0      187 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/openai_function_call/__init__.py
+-rw-r--r--   0        0        0      151 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/openai_function_call/dsl/__init__.py
+-rw-r--r--   0        0        0     5799 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/openai_function_call/dsl/completion.py
+-rw-r--r--   0        0        0      505 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/openai_function_call/dsl/messages/__init__.py
+-rw-r--r--   0        0        0     1669 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/openai_function_call/dsl/messages/base.py
+-rw-r--r--   0        0        0     3260 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/openai_function_call/dsl/messages/messages.py
+-rw-r--r--   0        0        0     1486 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/openai_function_call/dsl/messages/user.py
+-rw-r--r--   0        0        0     3698 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/openai_function_call/dsl/multitask.py
+-rw-r--r--   0        0        0     6330 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/openai_function_call/function_calls.py
+-rw-r--r--   0        0        0      662 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     9127 1970-01-01 00:00:00.000000 openai_function_call-0.2.1/PKG-INFO
```

### Comparing `openai_function_call-0.2.0/LICENSE` & `openai_function_call-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.2.0/README.md` & `openai_function_call-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Pydantic is all you need, for openai function calls.
 
 Check out the [docs](https://openai-function-call.onrender.com/)!
 
 We try to provides a powerful and efficient approach to output parsing when interacting with OpenAI's Function Call API. One that is framework agnostic and minimizes any dependencies. It leverages the data validation capabilities of the Pydantic library to handle output parsing in a more structured and reliable manner.
 If you have any feedback, leave an issue or hit me up on [twitter](https://twitter.com/jxnlco).
 
-This repo also contains a range of examples I've used in experimetnation and in production and I welcome new contributions for different types of schemas.
+This repo also contains a range of examples I've used in experimentation and in production and I welcome new contributions for different types of schemas.
 
 ## Support
 
 Follow me on twitter and consider helping pay for openai tokens!
 
 [![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/jxnlco.svg?style=social&label=Follow%20%40jxnlco)](https://twitter.com/jxnlco) [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/jxnl)
```

### Comparing `openai_function_call-0.2.0/openai_function_call/dsl/completion.py` & `openai_function_call-0.2.1/openai_function_call/dsl/completion.py`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.2.0/openai_function_call/dsl/messages/base.py` & `openai_function_call-0.2.1/openai_function_call/dsl/messages/base.py`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.2.0/openai_function_call/dsl/messages/messages.py` & `openai_function_call-0.2.1/openai_function_call/dsl/messages/messages.py`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.2.0/openai_function_call/dsl/messages/user.py` & `openai_function_call-0.2.1/openai_function_call/dsl/messages/user.py`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.2.0/openai_function_call/function_calls.py` & `openai_function_call-0.2.1/openai_function_call/function_calls.py`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.2.0/pyproject.toml` & `openai_function_call-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-function-call"
-version = "0.2.0"
+version = "0.2.1"
 description = "Helper functions that allow us to improve openai's function_call ergonomics"
 authors = ["Jason <jason@jxnl.co>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "openai_function_call"}]
 repository = "https://github.com/jxnl/openai_function_call"
```

### Comparing `openai_function_call-0.2.0/PKG-INFO` & `openai_function_call-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-function-call
-Version: 0.2.0
+Version: 0.2.1
 Summary: Helper functions that allow us to improve openai's function_call ergonomics
 Home-page: https://github.com/jxnl/openai_function_call
 License: MIT
 Author: Jason
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,15 @@
 # Pydantic is all you need, for openai function calls.
 
 Check out the [docs](https://openai-function-call.onrender.com/)!
 
 We try to provides a powerful and efficient approach to output parsing when interacting with OpenAI's Function Call API. One that is framework agnostic and minimizes any dependencies. It leverages the data validation capabilities of the Pydantic library to handle output parsing in a more structured and reliable manner.
 If you have any feedback, leave an issue or hit me up on [twitter](https://twitter.com/jxnlco).
 
-This repo also contains a range of examples I've used in experimetnation and in production and I welcome new contributions for different types of schemas.
+This repo also contains a range of examples I've used in experimentation and in production and I welcome new contributions for different types of schemas.
 
 ## Support
 
 Follow me on twitter and consider helping pay for openai tokens!
 
 [![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/jxnlco.svg?style=social&label=Follow%20%40jxnlco)](https://twitter.com/jxnlco) [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/jxnl)
```

