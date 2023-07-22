# Comparing `tmp/refiner-0.0.3.tar.gz` & `tmp/refiner-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refiner-0.0.3.tar", last modified: Sat Jul 22 03:26:29 2023, max compression
+gzip compressed data, was "refiner-0.0.4.tar", last modified: Sat Jul 22 05:40:19 2023, max compression
```

## Comparing `refiner-0.0.3.tar` & `refiner-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 03:26:29.503605 refiner-0.0.3/
--rw-r--r--   0 adaro      (501) staff       (20)     1066 2023-04-22 07:38:04.000000 refiner-0.0.3/LICENSE
--rw-r--r--   0 adaro      (501) staff       (20)     2095 2023-07-22 03:26:29.503265 refiner-0.0.3/PKG-INFO
--rw-r--r--   0 adaro      (501) staff       (20)     1486 2023-07-11 08:25:57.000000 refiner-0.0.3/README.md
--rw-r--r--   0 adaro      (501) staff       (20)      752 2023-07-22 03:21:34.000000 refiner-0.0.3/pyproject.toml
--rw-r--r--   0 adaro      (501) staff       (20)       38 2023-07-22 03:26:29.503691 refiner-0.0.3/setup.cfg
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 03:26:29.494997 refiner-0.0.3/src/
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 03:26:29.497972 refiner-0.0.3/src/refiner/
--rw-r--r--   0 adaro      (501) staff       (20)        0 2023-04-28 14:32:48.000000 refiner-0.0.3/src/refiner/__init__.py
--rw-r--r--   0 adaro      (501) staff       (20)     3894 2023-07-22 03:17:48.000000 refiner-0.0.3/src/refiner/embeddings.py
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 03:26:29.502297 refiner-0.0.3/src/refiner/integrations/
--rw-r--r--   0 adaro      (501) staff       (20)       86 2023-06-09 07:17:42.000000 refiner-0.0.3/src/refiner/integrations/__init__.py
--rw-r--r--   0 adaro      (501) staff       (20)      508 2023-07-22 03:20:39.000000 refiner-0.0.3/src/refiner/integrations/refiner_openai.py
--rw-r--r--   0 adaro      (501) staff       (20)     2807 2023-07-22 03:21:07.000000 refiner-0.0.3/src/refiner/integrations/refiner_pinecone.py
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 03:26:29.500234 refiner-0.0.3/src/refiner.egg-info/
--rw-r--r--   0 adaro      (501) staff       (20)     2095 2023-07-22 03:26:29.000000 refiner-0.0.3/src/refiner.egg-info/PKG-INFO
--rw-r--r--   0 adaro      (501) staff       (20)      381 2023-07-22 03:26:29.000000 refiner-0.0.3/src/refiner.egg-info/SOURCES.txt
--rw-r--r--   0 adaro      (501) staff       (20)        1 2023-07-22 03:26:29.000000 refiner-0.0.3/src/refiner.egg-info/dependency_links.txt
--rw-r--r--   0 adaro      (501) staff       (20)       87 2023-07-22 03:26:29.000000 refiner-0.0.3/src/refiner.egg-info/requires.txt
--rw-r--r--   0 adaro      (501) staff       (20)        8 2023-07-22 03:26:29.000000 refiner-0.0.3/src/refiner.egg-info/top_level.txt
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 05:40:19.025943 refiner-0.0.4/
+-rw-r--r--   0 adaro      (501) staff       (20)     1066 2023-04-22 07:38:04.000000 refiner-0.0.4/LICENSE
+-rw-r--r--   0 adaro      (501) staff       (20)     2095 2023-07-22 05:40:19.025519 refiner-0.0.4/PKG-INFO
+-rw-r--r--   0 adaro      (501) staff       (20)     1486 2023-07-11 08:25:57.000000 refiner-0.0.4/README.md
+-rw-r--r--   0 adaro      (501) staff       (20)      752 2023-07-22 05:37:54.000000 refiner-0.0.4/pyproject.toml
+-rw-r--r--   0 adaro      (501) staff       (20)       38 2023-07-22 05:40:19.026067 refiner-0.0.4/setup.cfg
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 05:40:19.019662 refiner-0.0.4/src/
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 05:40:19.021509 refiner-0.0.4/src/refiner/
+-rw-r--r--   0 adaro      (501) staff       (20)        0 2023-04-28 14:32:48.000000 refiner-0.0.4/src/refiner/__init__.py
+-rw-r--r--   0 adaro      (501) staff       (20)     3866 2023-07-22 05:29:05.000000 refiner-0.0.4/src/refiner/embeddings.py
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 05:40:19.024915 refiner-0.0.4/src/refiner/integrations/
+-rw-r--r--   0 adaro      (501) staff       (20)       86 2023-06-09 07:17:42.000000 refiner-0.0.4/src/refiner/integrations/__init__.py
+-rw-r--r--   0 adaro      (501) staff       (20)      508 2023-07-22 03:20:39.000000 refiner-0.0.4/src/refiner/integrations/refiner_openai.py
+-rw-r--r--   0 adaro      (501) staff       (20)     3265 2023-07-22 05:37:20.000000 refiner-0.0.4/src/refiner/integrations/refiner_pinecone.py
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 05:40:19.023687 refiner-0.0.4/src/refiner.egg-info/
+-rw-r--r--   0 adaro      (501) staff       (20)     2095 2023-07-22 05:40:19.000000 refiner-0.0.4/src/refiner.egg-info/PKG-INFO
+-rw-r--r--   0 adaro      (501) staff       (20)      381 2023-07-22 05:40:19.000000 refiner-0.0.4/src/refiner.egg-info/SOURCES.txt
+-rw-r--r--   0 adaro      (501) staff       (20)        1 2023-07-22 05:40:19.000000 refiner-0.0.4/src/refiner.egg-info/dependency_links.txt
+-rw-r--r--   0 adaro      (501) staff       (20)       87 2023-07-22 05:40:19.000000 refiner-0.0.4/src/refiner.egg-info/requires.txt
+-rw-r--r--   0 adaro      (501) staff       (20)        8 2023-07-22 05:40:19.000000 refiner-0.0.4/src/refiner.egg-info/top_level.txt
```

### Comparing `refiner-0.0.3/LICENSE` & `refiner-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `refiner-0.0.3/PKG-INFO` & `refiner-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refiner
-Version: 0.0.3
+Version: 0.0.4
 Summary: Refiner is a python package that allows you to store text as vectors in Pinecone and then search for similar text. It uses OpenAI to generate embeddings and then uses Pinecone to store and search for similar text.
 Author-email: Alex Daro <gmx2267@gmail.com>
 Project-URL: Homepage, https://github.com/adaro/ai-refiner
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `refiner-0.0.3/README.md` & `refiner-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `refiner-0.0.3/pyproject.toml` & `refiner-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "refiner"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Alex Daro", email="gmx2267@gmail.com" },
 ]
 description = "Refiner is a python package that allows you to store text as vectors in Pinecone and then search for similar text. It uses OpenAI to generate embeddings and then uses Pinecone to store and search for similar text."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `refiner-0.0.3/src/refiner/embeddings.py` & `refiner-0.0.4/src/refiner/embeddings.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,33 +14,32 @@
     Embeddings are created using OpenAI. Uses Pinecone for storing and searching embeddings.
     """
 
     def __init__(self, config_file=None, openai_api_key=None, pinecone_api_key=None, pinecone_environment_name=None):
         """
         Initialize the Refiner class.
         """
-        self.config_file = config_file
-        _dotenv_path = Path(self.config_file or '.env')
+        _dotenv_path = Path(config_file or '.env')
         if _dotenv_path.exists():
             load_dotenv(dotenv_path=_dotenv_path)
 
-        self.openai_api_key = openai_api_key or os.getenv("OPENAI_API_KEY")
-        self.pinecone_api_key = pinecone_api_key or os.getenv(
+        self.__openai_api_key = openai_api_key or os.getenv("OPENAI_API_KEY")
+        self.__pinecone_api_key = pinecone_api_key or os.getenv(
             "PINECONE_API_KEY")
         self.pinecone_environment_name = pinecone_environment_name or os.getenv(
             "PINECONE_ENVIRONMENT_NAME")
         self.openai_ada_200_default_dimension = 1536
 
     def __validate_env(self):
         """
         Validate the environment variables.
         """
-        if not self.openai_api_key:
+        if not self.__openai_api_key:
             return {"error": "OPENAI_API_KEY environment variable not set in .env file or passed in as an argument."}
-        if not self.pinecone_api_key:
+        if not self.__pinecone_api_key:
             return {"error": "PINECONE_API_KEY environment variable not set in .env file or passed in as an argument."}
         if not self.pinecone_environment_name:
             return {"error": "PINECONE_ENVIRONMENT_NAME environment variable not set in .env file or passed in as an argument."}
         return {"success": True}
 
     def __validate_payload(self, payload):
         """
@@ -63,25 +62,25 @@
         if validated_env.get('error', None):
             return validated_env
 
         validated_payload = self.__validate_payload(payload)
         if validated_payload.get('error', None):
             return validated_payload
 
-        openai_client = OpenAIClient(self.openai_api_key)
+        openai_client = OpenAIClient(self.__openai_api_key)
         embeddings = openai_client.create_embeddings(payload['text'])
 
         metadata = payload.get('metadata', None)
         if metadata:
             metadata = json.loads(metadata)
 
         vector = (str(payload['id']), embeddings, metadata)
 
         pinecone_client = PineconeClient(
-            self.pinecone_api_key, self.pinecone_environment_name)
+            self.__pinecone_api_key, self.pinecone_environment_name)
         response = pinecone_client.store_embeddings(
             [vector], index_id, dimension=self.openai_ada_200_default_dimension, namespace=namespace,
             batch_size=batch_size, pool_threads=pool_threads)
 
         return response
 
     def search(self, query, index_id, limit, namespace=None):
@@ -89,13 +88,13 @@
         Search embeddings from text.
         """
         validated_env = self.__validate_env()
         if validated_env.get('error', None):
             return validated_env
 
         pinecone_client = PineconeClient(
-            self.pinecone_api_key, self.pinecone_environment_name)
-        openai_client = OpenAIClient(self.openai_api_key)
+            self.__pinecone_api_key, self.pinecone_environment_name)
+        openai_client = OpenAIClient(self.__openai_api_key)
         embeddings = openai_client.create_embeddings(query)
         results = pinecone_client.search(
             embeddings, index_id, limit, namespace=namespace)
         return results
```

### Comparing `refiner-0.0.3/src/refiner/integrations/refiner_pinecone.py` & `refiner-0.0.4/src/refiner/integrations/refiner_pinecone.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,30 @@
+import os
 import pinecone
 import itertools
+from pathlib import Path
+from dotenv import load_dotenv
 
 
 class PineconeClient(object):
 
-    def __init__(self, api_key, environment_name):
+    def __init__(self, api_key=None, environment_name=None, config_file=None):
+
+        self.config_file = config_file
+        _dotenv_path = Path(self.config_file or '.env')
+        if _dotenv_path.exists():
+            load_dotenv(dotenv_path=_dotenv_path)
+
+        self.__api_key = api_key or os.getenv("PINECONE_API_KEY")
+        self.environment_name = environment_name or os.getenv(
+            "PINECONE_ENVIRONMENT_NAME")
+
         # Init Pinecone
         pinecone.init(
-            api_key=api_key, environment=environment_name)
+            api_key=self.__api_key, environment=self.environment_name)
 
         # Set pinecone on class. Consumers of this class can use it to call pinecone API directly.
         self.pinecone = pinecone
 
     def chunks(self, iterable, batch_size=100):
         """A helper function to break an iterable into chunks of size batch_size."""
         it = iter(iterable)
```

### Comparing `refiner-0.0.3/src/refiner.egg-info/PKG-INFO` & `refiner-0.0.4/src/refiner.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refiner
-Version: 0.0.3
+Version: 0.0.4
 Summary: Refiner is a python package that allows you to store text as vectors in Pinecone and then search for similar text. It uses OpenAI to generate embeddings and then uses Pinecone to store and search for similar text.
 Author-email: Alex Daro <gmx2267@gmail.com>
 Project-URL: Homepage, https://github.com/adaro/ai-refiner
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

