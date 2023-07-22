# Comparing `tmp/refiner-0.0.4.tar.gz` & `tmp/refiner-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refiner-0.0.4.tar", last modified: Sat Jul 22 05:40:19 2023, max compression
+gzip compressed data, was "refiner-0.0.5.tar", last modified: Sat Jul 22 05:47:14 2023, max compression
```

## Comparing `refiner-0.0.4.tar` & `refiner-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 05:40:19.025943 refiner-0.0.4/
--rw-r--r--   0 adaro      (501) staff       (20)     1066 2023-04-22 07:38:04.000000 refiner-0.0.4/LICENSE
--rw-r--r--   0 adaro      (501) staff       (20)     2095 2023-07-22 05:40:19.025519 refiner-0.0.4/PKG-INFO
--rw-r--r--   0 adaro      (501) staff       (20)     1486 2023-07-11 08:25:57.000000 refiner-0.0.4/README.md
--rw-r--r--   0 adaro      (501) staff       (20)      752 2023-07-22 05:37:54.000000 refiner-0.0.4/pyproject.toml
--rw-r--r--   0 adaro      (501) staff       (20)       38 2023-07-22 05:40:19.026067 refiner-0.0.4/setup.cfg
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 05:40:19.019662 refiner-0.0.4/src/
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 05:40:19.021509 refiner-0.0.4/src/refiner/
--rw-r--r--   0 adaro      (501) staff       (20)        0 2023-04-28 14:32:48.000000 refiner-0.0.4/src/refiner/__init__.py
--rw-r--r--   0 adaro      (501) staff       (20)     3866 2023-07-22 05:29:05.000000 refiner-0.0.4/src/refiner/embeddings.py
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 05:40:19.024915 refiner-0.0.4/src/refiner/integrations/
--rw-r--r--   0 adaro      (501) staff       (20)       86 2023-06-09 07:17:42.000000 refiner-0.0.4/src/refiner/integrations/__init__.py
--rw-r--r--   0 adaro      (501) staff       (20)      508 2023-07-22 03:20:39.000000 refiner-0.0.4/src/refiner/integrations/refiner_openai.py
--rw-r--r--   0 adaro      (501) staff       (20)     3265 2023-07-22 05:37:20.000000 refiner-0.0.4/src/refiner/integrations/refiner_pinecone.py
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 05:40:19.023687 refiner-0.0.4/src/refiner.egg-info/
--rw-r--r--   0 adaro      (501) staff       (20)     2095 2023-07-22 05:40:19.000000 refiner-0.0.4/src/refiner.egg-info/PKG-INFO
--rw-r--r--   0 adaro      (501) staff       (20)      381 2023-07-22 05:40:19.000000 refiner-0.0.4/src/refiner.egg-info/SOURCES.txt
--rw-r--r--   0 adaro      (501) staff       (20)        1 2023-07-22 05:40:19.000000 refiner-0.0.4/src/refiner.egg-info/dependency_links.txt
--rw-r--r--   0 adaro      (501) staff       (20)       87 2023-07-22 05:40:19.000000 refiner-0.0.4/src/refiner.egg-info/requires.txt
--rw-r--r--   0 adaro      (501) staff       (20)        8 2023-07-22 05:40:19.000000 refiner-0.0.4/src/refiner.egg-info/top_level.txt
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 05:47:14.219096 refiner-0.0.5/
+-rw-r--r--   0 adaro      (501) staff       (20)     1066 2023-04-22 07:38:04.000000 refiner-0.0.5/LICENSE
+-rw-r--r--   0 adaro      (501) staff       (20)     2095 2023-07-22 05:47:14.218714 refiner-0.0.5/PKG-INFO
+-rw-r--r--   0 adaro      (501) staff       (20)     1486 2023-07-11 08:25:57.000000 refiner-0.0.5/README.md
+-rw-r--r--   0 adaro      (501) staff       (20)      752 2023-07-22 05:46:57.000000 refiner-0.0.5/pyproject.toml
+-rw-r--r--   0 adaro      (501) staff       (20)       38 2023-07-22 05:47:14.219272 refiner-0.0.5/setup.cfg
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 05:47:14.212169 refiner-0.0.5/src/
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 05:47:14.214117 refiner-0.0.5/src/refiner/
+-rw-r--r--   0 adaro      (501) staff       (20)        0 2023-04-28 14:32:48.000000 refiner-0.0.5/src/refiner/__init__.py
+-rw-r--r--   0 adaro      (501) staff       (20)     3866 2023-07-22 05:29:05.000000 refiner-0.0.5/src/refiner/embeddings.py
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 05:47:14.218222 refiner-0.0.5/src/refiner/integrations/
+-rw-r--r--   0 adaro      (501) staff       (20)       86 2023-06-09 07:17:42.000000 refiner-0.0.5/src/refiner/integrations/__init__.py
+-rw-r--r--   0 adaro      (501) staff       (20)      508 2023-07-22 03:20:39.000000 refiner-0.0.5/src/refiner/integrations/refiner_openai.py
+-rw-r--r--   0 adaro      (501) staff       (20)     3265 2023-07-22 05:37:20.000000 refiner-0.0.5/src/refiner/integrations/refiner_pinecone.py
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-22 05:47:14.216156 refiner-0.0.5/src/refiner.egg-info/
+-rw-r--r--   0 adaro      (501) staff       (20)     2095 2023-07-22 05:47:14.000000 refiner-0.0.5/src/refiner.egg-info/PKG-INFO
+-rw-r--r--   0 adaro      (501) staff       (20)      381 2023-07-22 05:47:14.000000 refiner-0.0.5/src/refiner.egg-info/SOURCES.txt
+-rw-r--r--   0 adaro      (501) staff       (20)        1 2023-07-22 05:47:14.000000 refiner-0.0.5/src/refiner.egg-info/dependency_links.txt
+-rw-r--r--   0 adaro      (501) staff       (20)       87 2023-07-22 05:47:14.000000 refiner-0.0.5/src/refiner.egg-info/requires.txt
+-rw-r--r--   0 adaro      (501) staff       (20)        8 2023-07-22 05:47:14.000000 refiner-0.0.5/src/refiner.egg-info/top_level.txt
```

### Comparing `refiner-0.0.4/LICENSE` & `refiner-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `refiner-0.0.4/PKG-INFO` & `refiner-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refiner
-Version: 0.0.4
+Version: 0.0.5
 Summary: Refiner is a python package that allows you to store text as vectors in Pinecone and then search for similar text. It uses OpenAI to generate embeddings and then uses Pinecone to store and search for similar text.
 Author-email: Alex Daro <gmx2267@gmail.com>
 Project-URL: Homepage, https://github.com/adaro/ai-refiner
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `refiner-0.0.4/README.md` & `refiner-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `refiner-0.0.4/pyproject.toml` & `refiner-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "refiner"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Alex Daro", email="gmx2267@gmail.com" },
 ]
 description = "Refiner is a python package that allows you to store text as vectors in Pinecone and then search for similar text. It uses OpenAI to generate embeddings and then uses Pinecone to store and search for similar text."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `refiner-0.0.4/src/refiner/embeddings.py` & `refiner-0.0.5/src/refiner/embeddings.py`

 * *Files identical despite different names*

### Comparing `refiner-0.0.4/src/refiner/integrations/refiner_pinecone.py` & `refiner-0.0.5/src/refiner/integrations/refiner_pinecone.py`

 * *Files identical despite different names*

### Comparing `refiner-0.0.4/src/refiner.egg-info/PKG-INFO` & `refiner-0.0.5/src/refiner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refiner
-Version: 0.0.4
+Version: 0.0.5
 Summary: Refiner is a python package that allows you to store text as vectors in Pinecone and then search for similar text. It uses OpenAI to generate embeddings and then uses Pinecone to store and search for similar text.
 Author-email: Alex Daro <gmx2267@gmail.com>
 Project-URL: Homepage, https://github.com/adaro/ai-refiner
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

