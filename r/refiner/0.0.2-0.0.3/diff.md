# Comparing `tmp/refiner-0.0.2.tar.gz` & `tmp/refiner-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refiner-0.0.2.tar", last modified: Sun Jul  2 08:00:57 2023, max compression
+gzip compressed data, was "refiner-0.0.3.tar", last modified: Sat Jul 22 03:26:29 2023, max compression
```

## Comparing `refiner-0.0.2.tar` & `refiner-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-02 08:00:57.002089 refiner-0.0.2/
--rw-r--r--   0 adaro      (501) staff       (20)     1066 2023-04-22 07:38:04.000000 refiner-0.0.2/LICENSE
--rw-r--r--   0 adaro      (501) staff       (20)     1881 2023-07-02 08:00:57.001794 refiner-0.0.2/PKG-INFO
--rw-r--r--   0 adaro      (501) staff       (20)     1272 2023-07-02 07:49:51.000000 refiner-0.0.2/README.md
--rw-r--r--   0 adaro      (501) staff       (20)      752 2023-07-02 07:59:44.000000 refiner-0.0.2/pyproject.toml
--rw-r--r--   0 adaro      (501) staff       (20)       38 2023-07-02 08:00:57.002174 refiner-0.0.2/setup.cfg
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-02 08:00:56.995429 refiner-0.0.2/src/
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-02 08:00:56.997432 refiner-0.0.2/src/refiner/
--rw-r--r--   0 adaro      (501) staff       (20)        0 2023-04-28 14:32:48.000000 refiner-0.0.2/src/refiner/__init__.py
--rw-r--r--   0 adaro      (501) staff       (20)     5197 2023-06-20 10:25:14.000000 refiner-0.0.2/src/refiner/embeddings.py
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-02 08:00:57.001102 refiner-0.0.2/src/refiner/integrations/
--rw-r--r--   0 adaro      (501) staff       (20)       86 2023-06-09 07:17:42.000000 refiner-0.0.2/src/refiner/integrations/__init__.py
--rw-r--r--   0 adaro      (501) staff       (20)      356 2023-06-09 09:24:33.000000 refiner-0.0.2/src/refiner/integrations/refiner_openai.py
--rw-r--r--   0 adaro      (501) staff       (20)     2668 2023-06-20 10:06:14.000000 refiner-0.0.2/src/refiner/integrations/refiner_pinecone.py
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-02 08:00:56.999348 refiner-0.0.2/src/refiner.egg-info/
--rw-r--r--   0 adaro      (501) staff       (20)     1881 2023-07-02 08:00:56.000000 refiner-0.0.2/src/refiner.egg-info/PKG-INFO
--rw-r--r--   0 adaro      (501) staff       (20)      381 2023-07-02 08:00:56.000000 refiner-0.0.2/src/refiner.egg-info/SOURCES.txt
--rw-r--r--   0 adaro      (501) staff       (20)        1 2023-07-02 08:00:56.000000 refiner-0.0.2/src/refiner.egg-info/dependency_links.txt
--rw-r--r--   0 adaro      (501) staff       (20)       87 2023-07-02 08:00:56.000000 refiner-0.0.2/src/refiner.egg-info/requires.txt
--rw-r--r--   0 adaro      (501) staff       (20)        8 2023-07-02 08:00:56.000000 refiner-0.0.2/src/refiner.egg-info/top_level.txt
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 03:26:29.503605 refiner-0.0.3/
+-rw-r--r--   0 adaro      (501) staff       (20)     1066 2023-04-22 07:38:04.000000 refiner-0.0.3/LICENSE
+-rw-r--r--   0 adaro      (501) staff       (20)     2095 2023-07-22 03:26:29.503265 refiner-0.0.3/PKG-INFO
+-rw-r--r--   0 adaro      (501) staff       (20)     1486 2023-07-11 08:25:57.000000 refiner-0.0.3/README.md
+-rw-r--r--   0 adaro      (501) staff       (20)      752 2023-07-22 03:21:34.000000 refiner-0.0.3/pyproject.toml
+-rw-r--r--   0 adaro      (501) staff       (20)       38 2023-07-22 03:26:29.503691 refiner-0.0.3/setup.cfg
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 03:26:29.494997 refiner-0.0.3/src/
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 03:26:29.497972 refiner-0.0.3/src/refiner/
+-rw-r--r--   0 adaro      (501) staff       (20)        0 2023-04-28 14:32:48.000000 refiner-0.0.3/src/refiner/__init__.py
+-rw-r--r--   0 adaro      (501) staff       (20)     3894 2023-07-22 03:17:48.000000 refiner-0.0.3/src/refiner/embeddings.py
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 03:26:29.502297 refiner-0.0.3/src/refiner/integrations/
+-rw-r--r--   0 adaro      (501) staff       (20)       86 2023-06-09 07:17:42.000000 refiner-0.0.3/src/refiner/integrations/__init__.py
+-rw-r--r--   0 adaro      (501) staff       (20)      508 2023-07-22 03:20:39.000000 refiner-0.0.3/src/refiner/integrations/refiner_openai.py
+-rw-r--r--   0 adaro      (501) staff       (20)     2807 2023-07-22 03:21:07.000000 refiner-0.0.3/src/refiner/integrations/refiner_pinecone.py
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 03:26:29.500234 refiner-0.0.3/src/refiner.egg-info/
+-rw-r--r--   0 adaro      (501) staff       (20)     2095 2023-07-22 03:26:29.000000 refiner-0.0.3/src/refiner.egg-info/PKG-INFO
+-rw-r--r--   0 adaro      (501) staff       (20)      381 2023-07-22 03:26:29.000000 refiner-0.0.3/src/refiner.egg-info/SOURCES.txt
+-rw-r--r--   0 adaro      (501) staff       (20)        1 2023-07-22 03:26:29.000000 refiner-0.0.3/src/refiner.egg-info/dependency_links.txt
+-rw-r--r--   0 adaro      (501) staff       (20)       87 2023-07-22 03:26:29.000000 refiner-0.0.3/src/refiner.egg-info/requires.txt
+-rw-r--r--   0 adaro      (501) staff       (20)        8 2023-07-22 03:26:29.000000 refiner-0.0.3/src/refiner.egg-info/top_level.txt
```

### Comparing `refiner-0.0.2/LICENSE` & `refiner-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `refiner-0.0.2/PKG-INFO` & `refiner-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: refiner
-Version: 0.0.2
+Version: 0.0.3
 Summary: Refiner is a python package that allows you to store text as vectors in Pinecone and then search for similar text. It uses OpenAI to generate embeddings and then uses Pinecone to store and search for similar text.
 Author-email: Alex Daro <gmx2267@gmail.com>
 Project-URL: Homepage, https://github.com/adaro/ai-refiner
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AI-Refiner
 
-The [Refiner](https://pypi.org/project/refiner/) python package can be used to convert and store text and metadata as vector embeddings. Embeddings are generated using [OpenAI](https://openai.com/) and stored as vectors in [Pinecone](https://www.pinecone.io/). Stored embeddings can then be "queried" using the `search` method. Matched embeddings contain contextually relavant metadata that can be used for AI chatbots, semnatic search APIs, and can also be used for training and tuning large language models.
-
+The [Refiner](https://pypi.org/project/refiner/) Python package can be used to convert and store text and metadata as vector embeddings. Embeddings are generated using [OpenAI](https://openai.com/) and stored as vectors in [Pinecone](https://www.pinecone.io/). Stored embeddings can then be "queried" using the `search` method. Matched embeddings contain contextually relevant metadata that can be used for AI chatbots, and semantic search APIs, etc.
 ## Installation
 
 ```shell
 pip install refiner
 ```
 
 ## OpenAI and Pinecone API Keys.
@@ -44,10 +43,22 @@
 
 ```shell
 PINECONE_API_KEY="API_KEY"
 PINECONE_ENVIRONMENT_NAME="ENV_NAME"
 OPENAI_API_KEY="API_KEY"
 ```
 
-## API Docs
+## CLI
+
+You can install the [CLI](https://pypi.org/project/refiner-cli/) to `create` and `search` your vectors.
+
+```shell
+pip install refiner-cli
+```
+
+The --help option can be used to learn about the create and search commands.
 
-Comming soon.
+```shell
+refiner --help
+refiner create --help
+refiner search --help
+```
```

### Comparing `refiner-0.0.2/README.md` & `refiner-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # AI-Refiner
 
-The [Refiner](https://pypi.org/project/refiner/) python package can be used to convert and store text and metadata as vector embeddings. Embeddings are generated using [OpenAI](https://openai.com/) and stored as vectors in [Pinecone](https://www.pinecone.io/). Stored embeddings can then be "queried" using the `search` method. Matched embeddings contain contextually relavant metadata that can be used for AI chatbots, semnatic search APIs, and can also be used for training and tuning large language models.
-
+The [Refiner](https://pypi.org/project/refiner/) Python package can be used to convert and store text and metadata as vector embeddings. Embeddings are generated using [OpenAI](https://openai.com/) and stored as vectors in [Pinecone](https://www.pinecone.io/). Stored embeddings can then be "queried" using the `search` method. Matched embeddings contain contextually relevant metadata that can be used for AI chatbots, and semantic search APIs, etc.
 ## Installation
 
 ```shell
 pip install refiner
 ```
 
 ## OpenAI and Pinecone API Keys.
@@ -31,10 +30,22 @@
 
 ```shell
 PINECONE_API_KEY="API_KEY"
 PINECONE_ENVIRONMENT_NAME="ENV_NAME"
 OPENAI_API_KEY="API_KEY"
 ```
 
-## API Docs
+## CLI
+
+You can install the [CLI](https://pypi.org/project/refiner-cli/) to `create` and `search` your vectors.
+
+```shell
+pip install refiner-cli
+```
+
+The --help option can be used to learn about the create and search commands.
 
-Comming soon.
+```shell
+refiner --help
+refiner create --help
+refiner search --help
+```
```

### Comparing `refiner-0.0.2/pyproject.toml` & `refiner-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "refiner"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Alex Daro", email="gmx2267@gmail.com" },
 ]
 description = "Refiner is a python package that allows you to store text as vectors in Pinecone and then search for similar text. It uses OpenAI to generate embeddings and then uses Pinecone to store and search for similar text."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `refiner-0.0.2/src/refiner/embeddings.py` & `refiner-0.0.3/src/refiner/embeddings.py`

 * *Files 19% similar despite different names*

```diff
@@ -95,52 +95,7 @@
         pinecone_client = PineconeClient(
             self.pinecone_api_key, self.pinecone_environment_name)
         openai_client = OpenAIClient(self.openai_api_key)
         embeddings = openai_client.create_embeddings(query)
         results = pinecone_client.search(
             embeddings, index_id, limit, namespace=namespace)
         return results
-
-    def delete(self, id):
-        """
-        Delete embeddings from text.
-        """
-        pass
-
-    def get(self, id):
-        """
-        Get embeddings from text.
-        """
-        pass
-
-    def update(self, id):
-        """
-        Update embeddings from text.
-        """
-        pass
-
-    # def upload_file(self, payload, index_id, namespace=None, batch_size=None, pool_threads=None):
-    #     """
-    #     Upload embeddings from file.
-    #     """
-    #     # Read file contents
-    #     # Create embeddings from file contents
-    #     # Store embeddings in Pinecone
-    #     # Return response
-
-    #     # read file in chunks if it's too big:
-    #     with open(file, 'r') as f:
-    #         if chunk_size:
-    #             while True:
-    #                 chunk = f.read(1024)
-    #                 if not chunk:
-    #                     break
-    #                 # create embeddings from chunk:
-    #                 openai_client = OpenAIClient(self.openai_api_key)
-    #                 embeddings = openai_client.create_embeddings(chunk)
-    #                 vector = (str(payload['id']), embeddings, metadata)
-
-    #                 # store embeddings in Pinecone
-
-    #     # read file contents:
-    #     with open(file, 'r') as f:
-    #         contents = f.read()
```

### Comparing `refiner-0.0.2/src/refiner/integrations/refiner_pinecone.py` & `refiner-0.0.3/src/refiner/integrations/refiner_pinecone.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 import pinecone
 import itertools
 
 
 class PineconeClient(object):
 
     def __init__(self, api_key, environment_name):
-        # Connect to Pinecone
-        pinecone.init(api_key=api_key, environment=environment_name)
+        # Init Pinecone
+        pinecone.init(
+            api_key=api_key, environment=environment_name)
+
+        # Set pinecone on class. Consumers of this class can use it to call pinecone API directly.
+        self.pinecone = pinecone
 
     def chunks(self, iterable, batch_size=100):
         """A helper function to break an iterable into chunks of size batch_size."""
         it = iter(iterable)
         chunk = tuple(itertools.islice(it, batch_size))
         while chunk:
             yield chunk
             chunk = tuple(itertools.islice(it, batch_size))
 
     def store_embeddings(self, embeddings, index_name, dimension, namespace=None, batch_size=None, pool_threads=None):
 
         # only create index if it doesn't exist
-        if index_name not in pinecone.list_indexes():
+        if index_name not in self.pinecone.list_indexes():
             print('Creating Pinecone index...')
-            pinecone.create_index(
+            self.pinecone.create_index(
                 name=index_name,
                 dimension=dimension
             )
+            print('Pinecone index created: {}'.format(index_name))
 
         # Add embeddings to Pinecone index
-        pinecone_index = pinecone.Index(index_name)
+        pinecone_index = self.pinecone.Index(index_name)
 
         # If pool_threads, use the pool_threads
         if pool_threads:
-            with pinecone.Index(index_name, pool_threads=pool_threads) as pinecone_index:
+            with self.pinecone.Index(index_name, pool_threads=pool_threads) as pinecone_index:
                 # Send requests in parallel
                 async_results = [
                     pinecone_index.upsert(
                         vectors=ids_vectors_chunk, async_req=True)
                     for ids_vectors_chunk in self.chunks(embeddings, batch_size=batch_size)
                 ]
                 # Wait for and retrieve responses (this raises in case of error)
@@ -54,18 +59,14 @@
         response = pinecone_index.upsert(
             vectors=embeddings, namespace=namespace)
         return response
 
     def search(self, embeddings, index_name, limit, namespace=None):
 
         # Connect to the Pinecone index
-        index = pinecone.Index(index_name)
+        index = self.pinecone.Index(index_name)
 
         # Perform a nearest neighbor search in Pinecone
         query_results = index.query(vector=embeddings, namespace=namespace,
                                     top_k=limit, include_values=False, include_metadata=True)
 
         return query_results
-
-    def delete(self, index_name, namespace=None):
-        # Delete pinecone id
-        pass
```

### Comparing `refiner-0.0.2/src/refiner.egg-info/PKG-INFO` & `refiner-0.0.3/src/refiner.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: refiner
-Version: 0.0.2
+Version: 0.0.3
 Summary: Refiner is a python package that allows you to store text as vectors in Pinecone and then search for similar text. It uses OpenAI to generate embeddings and then uses Pinecone to store and search for similar text.
 Author-email: Alex Daro <gmx2267@gmail.com>
 Project-URL: Homepage, https://github.com/adaro/ai-refiner
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AI-Refiner
 
-The [Refiner](https://pypi.org/project/refiner/) python package can be used to convert and store text and metadata as vector embeddings. Embeddings are generated using [OpenAI](https://openai.com/) and stored as vectors in [Pinecone](https://www.pinecone.io/). Stored embeddings can then be "queried" using the `search` method. Matched embeddings contain contextually relavant metadata that can be used for AI chatbots, semnatic search APIs, and can also be used for training and tuning large language models.
-
+The [Refiner](https://pypi.org/project/refiner/) Python package can be used to convert and store text and metadata as vector embeddings. Embeddings are generated using [OpenAI](https://openai.com/) and stored as vectors in [Pinecone](https://www.pinecone.io/). Stored embeddings can then be "queried" using the `search` method. Matched embeddings contain contextually relevant metadata that can be used for AI chatbots, and semantic search APIs, etc.
 ## Installation
 
 ```shell
 pip install refiner
 ```
 
 ## OpenAI and Pinecone API Keys.
@@ -44,10 +43,22 @@
 
 ```shell
 PINECONE_API_KEY="API_KEY"
 PINECONE_ENVIRONMENT_NAME="ENV_NAME"
 OPENAI_API_KEY="API_KEY"
 ```
 
-## API Docs
+## CLI
+
+You can install the [CLI](https://pypi.org/project/refiner-cli/) to `create` and `search` your vectors.
+
+```shell
+pip install refiner-cli
+```
+
+The --help option can be used to learn about the create and search commands.
 
-Comming soon.
+```shell
+refiner --help
+refiner create --help
+refiner search --help
+```
```

