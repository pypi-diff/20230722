# Comparing `tmp/refiner-cli-0.0.1.tar.gz` & `tmp/refiner-cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refiner-cli-0.0.1.tar", last modified: Tue Jul 11 08:04:50 2023, max compression
+gzip compressed data, was "refiner-cli-0.0.2.tar", last modified: Sat Jul 22 05:54:37 2023, max compression
```

## Comparing `refiner-cli-0.0.1.tar` & `refiner-cli-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-11 08:04:50.385631 refiner-cli-0.0.1/
--rw-r--r--   0 adaro      (501) staff       (20)     1067 2023-07-02 08:16:02.000000 refiner-cli-0.0.1/LICENSE
--rw-r--r--   0 adaro      (501) staff       (20)     1872 2023-07-11 08:04:50.385734 refiner-cli-0.0.1/PKG-INFO
--rw-r--r--   0 adaro      (501) staff       (20)     1274 2023-07-11 08:03:57.000000 refiner-cli-0.0.1/README.md
--rw-r--r--   0 adaro      (501) staff       (20)      682 2023-07-11 07:56:37.000000 refiner-cli-0.0.1/pyproject.toml
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-11 08:04:50.382662 refiner-cli-0.0.1/refiner_cli/
--rw-r--r--   0 adaro      (501) staff       (20)        0 2023-07-02 10:19:04.000000 refiner-cli-0.0.1/refiner_cli/__init__.py
--rw-r--r--   0 adaro      (501) staff       (20)     2631 2023-07-02 11:34:10.000000 refiner-cli-0.0.1/refiner_cli/cli.py
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-11 08:04:50.385272 refiner-cli-0.0.1/refiner_cli.egg-info/
--rw-r--r--   0 adaro      (501) staff       (20)     1872 2023-07-11 08:04:50.000000 refiner-cli-0.0.1/refiner_cli.egg-info/PKG-INFO
--rw-r--r--   0 adaro      (501) staff       (20)      306 2023-07-11 08:04:50.000000 refiner-cli-0.0.1/refiner_cli.egg-info/SOURCES.txt
--rw-r--r--   0 adaro      (501) staff       (20)        1 2023-07-11 08:04:50.000000 refiner-cli-0.0.1/refiner_cli.egg-info/dependency_links.txt
--rw-r--r--   0 adaro      (501) staff       (20)       48 2023-07-11 08:04:50.000000 refiner-cli-0.0.1/refiner_cli.egg-info/entry_points.txt
--rw-r--r--   0 adaro      (501) staff       (20)       14 2023-07-11 08:04:50.000000 refiner-cli-0.0.1/refiner_cli.egg-info/requires.txt
--rw-r--r--   0 adaro      (501) staff       (20)       12 2023-07-11 08:04:50.000000 refiner-cli-0.0.1/refiner_cli.egg-info/top_level.txt
--rw-r--r--   0 adaro      (501) staff       (20)      190 2023-07-11 08:04:50.386298 refiner-cli-0.0.1/setup.cfg
--rw-r--r--   0 adaro      (501) staff       (20)       38 2023-07-02 08:24:31.000000 refiner-cli-0.0.1/setup.py
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 05:54:37.209401 refiner-cli-0.0.2/
+-rw-r--r--   0 adaro      (501) staff       (20)     1067 2023-07-02 08:16:02.000000 refiner-cli-0.0.2/LICENSE
+-rw-r--r--   0 adaro      (501) staff       (20)     1913 2023-07-22 05:54:37.209574 refiner-cli-0.0.2/PKG-INFO
+-rw-r--r--   0 adaro      (501) staff       (20)     1315 2023-07-11 08:21:41.000000 refiner-cli-0.0.2/README.md
+-rw-r--r--   0 adaro      (501) staff       (20)      682 2023-07-22 05:54:04.000000 refiner-cli-0.0.2/pyproject.toml
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 05:54:37.206914 refiner-cli-0.0.2/refiner_cli/
+-rw-r--r--   0 adaro      (501) staff       (20)        0 2023-07-02 10:19:04.000000 refiner-cli-0.0.2/refiner_cli/__init__.py
+-rw-r--r--   0 adaro      (501) staff       (20)     4862 2023-07-22 05:50:09.000000 refiner-cli-0.0.2/refiner_cli/cli.py
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 05:54:37.209061 refiner-cli-0.0.2/refiner_cli.egg-info/
+-rw-r--r--   0 adaro      (501) staff       (20)     1913 2023-07-22 05:54:37.000000 refiner-cli-0.0.2/refiner_cli.egg-info/PKG-INFO
+-rw-r--r--   0 adaro      (501) staff       (20)      306 2023-07-22 05:54:37.000000 refiner-cli-0.0.2/refiner_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 adaro      (501) staff       (20)        1 2023-07-22 05:54:37.000000 refiner-cli-0.0.2/refiner_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 adaro      (501) staff       (20)       48 2023-07-22 05:54:37.000000 refiner-cli-0.0.2/refiner_cli.egg-info/entry_points.txt
+-rw-r--r--   0 adaro      (501) staff       (20)       14 2023-07-22 05:54:37.000000 refiner-cli-0.0.2/refiner_cli.egg-info/requires.txt
+-rw-r--r--   0 adaro      (501) staff       (20)       12 2023-07-22 05:54:37.000000 refiner-cli-0.0.2/refiner_cli.egg-info/top_level.txt
+-rw-r--r--   0 adaro      (501) staff       (20)      190 2023-07-22 05:54:37.210200 refiner-cli-0.0.2/setup.cfg
+-rw-r--r--   0 adaro      (501) staff       (20)       38 2023-07-02 08:24:31.000000 refiner-cli-0.0.2/setup.py
```

### Comparing `refiner-cli-0.0.1/LICENSE` & `refiner-cli-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `refiner-cli-0.0.1/PKG-INFO` & `refiner-cli-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: refiner-cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: Refiner CLI allows you to store text as vectors in Pinecone and then search for similar text. It uses OpenAI to generate embeddings and then uses Pinecone to store and search for similar text.
 Author-email: Alex Daro <gmx2267@gmail.com>
 Project-URL: Homepage, https://github.com/AI-Refiner/refiner-cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # refiner-cli
 
-CLI for the [Refiner](https://pypi.org/project/refiner/) python package convert and store text and metadata as vector embeddings. Embeddings are generated using [OpenAI](https://openai.com/) and stored as vectors in [Pinecone](https://www.pinecone.io/). Stored embeddings can then be "queried" using the `search` command. Matched embeddings contain contextually relavant metadata that can be used for AI chatbots, semnatic search APIs, and can also be used for training and tuning large language models.
+[CLI](https://pypi.org/project/refiner-cli/) for the [Refiner](https://pypi.org/project/refiner/) python package convert and store text and metadata as vector embeddings. Embeddings are generated using [OpenAI](https://openai.com/) and stored as vectors in [Pinecone](https://www.pinecone.io/). Stored embeddings can then be "queried" using the `search` command. Matched embeddings contain contextually relavant metadata that can be used for AI chatbots, semnatic search APIs, and can also be used for training and tuning large language models.
 
 ## Installation
 
 ```shell
 pip install refiner-cli
 ```
```

### Comparing `refiner-cli-0.0.1/README.md` & `refiner-cli-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # refiner-cli
 
-CLI for the [Refiner](https://pypi.org/project/refiner/) python package convert and store text and metadata as vector embeddings. Embeddings are generated using [OpenAI](https://openai.com/) and stored as vectors in [Pinecone](https://www.pinecone.io/). Stored embeddings can then be "queried" using the `search` command. Matched embeddings contain contextually relavant metadata that can be used for AI chatbots, semnatic search APIs, and can also be used for training and tuning large language models.
+[CLI](https://pypi.org/project/refiner-cli/) for the [Refiner](https://pypi.org/project/refiner/) python package convert and store text and metadata as vector embeddings. Embeddings are generated using [OpenAI](https://openai.com/) and stored as vectors in [Pinecone](https://www.pinecone.io/). Stored embeddings can then be "queried" using the `search` command. Matched embeddings contain contextually relavant metadata that can be used for AI chatbots, semnatic search APIs, and can also be used for training and tuning large language models.
 
 ## Installation
 
 ```shell
 pip install refiner-cli
 ```
```

### Comparing `refiner-cli-0.0.1/pyproject.toml` & `refiner-cli-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "refiner-cli"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Alex Daro", email="gmx2267@gmail.com" },
 ]
 description = "Refiner CLI allows you to store text as vectors in Pinecone and then search for similar text. It uses OpenAI to generate embeddings and then uses Pinecone to store and search for similar text."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `refiner-cli-0.0.1/refiner_cli.egg-info/PKG-INFO` & `refiner-cli-0.0.2/refiner_cli.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: refiner-cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: Refiner CLI allows you to store text as vectors in Pinecone and then search for similar text. It uses OpenAI to generate embeddings and then uses Pinecone to store and search for similar text.
 Author-email: Alex Daro <gmx2267@gmail.com>
 Project-URL: Homepage, https://github.com/AI-Refiner/refiner-cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # refiner-cli
 
-CLI for the [Refiner](https://pypi.org/project/refiner/) python package convert and store text and metadata as vector embeddings. Embeddings are generated using [OpenAI](https://openai.com/) and stored as vectors in [Pinecone](https://www.pinecone.io/). Stored embeddings can then be "queried" using the `search` command. Matched embeddings contain contextually relavant metadata that can be used for AI chatbots, semnatic search APIs, and can also be used for training and tuning large language models.
+[CLI](https://pypi.org/project/refiner-cli/) for the [Refiner](https://pypi.org/project/refiner/) python package convert and store text and metadata as vector embeddings. Embeddings are generated using [OpenAI](https://openai.com/) and stored as vectors in [Pinecone](https://www.pinecone.io/). Stored embeddings can then be "queried" using the `search` command. Matched embeddings contain contextually relavant metadata that can be used for AI chatbots, semnatic search APIs, and can also be used for training and tuning large language models.
 
 ## Installation
 
 ```shell
 pip install refiner-cli
 ```
```

