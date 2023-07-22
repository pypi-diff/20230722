# Comparing `tmp/lsstream-0.0.7.tar.gz` & `tmp/lsstream-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsstream-0.0.7.tar", last modified: Sat Jul 22 16:41:06 2023, max compression
+gzip compressed data, was "lsstream-0.1.0.tar", last modified: Sat Jul 22 16:57:56 2023, max compression
```

## Comparing `lsstream-0.0.7.tar` & `lsstream-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:41:06.578504 lsstream-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-22 16:40:55.000000 lsstream-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-22 16:41:06.578504 lsstream-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-22 16:40:55.000000 lsstream-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-22 16:40:55.000000 lsstream-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 16:41:06.578504 lsstream-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:41:06.574504 lsstream-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:41:06.578504 lsstream-0.0.7/src/lsstream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:40:55.000000 lsstream-0.0.7/src/lsstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-22 16:40:55.000000 lsstream-0.0.7/src/lsstream/file_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-22 16:40:55.000000 lsstream-0.0.7/src/lsstream/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-22 16:40:55.000000 lsstream-0.0.7/src/lsstream/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-22 16:40:55.000000 lsstream-0.0.7/src/lsstream/style.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-22 16:40:55.000000 lsstream-0.0.7/src/lsstream/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-22 16:40:55.000000 lsstream-0.0.7/src/lsstream/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:41:06.578504 lsstream-0.0.7/src/lsstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-22 16:41:06.000000 lsstream-0.0.7/src/lsstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-22 16:41:06.000000 lsstream-0.0.7/src/lsstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:41:06.000000 lsstream-0.0.7/src/lsstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-22 16:41:06.000000 lsstream-0.0.7/src/lsstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 16:41:06.000000 lsstream-0.0.7/src/lsstream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:57:56.196497 lsstream-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-22 16:57:45.000000 lsstream-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-22 16:57:56.196497 lsstream-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-22 16:57:45.000000 lsstream-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-22 16:57:45.000000 lsstream-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 16:57:56.196497 lsstream-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:57:56.196497 lsstream-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:57:56.196497 lsstream-0.1.0/src/lsstream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:57:45.000000 lsstream-0.1.0/src/lsstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-22 16:57:45.000000 lsstream-0.1.0/src/lsstream/file_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-22 16:57:45.000000 lsstream-0.1.0/src/lsstream/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-22 16:57:45.000000 lsstream-0.1.0/src/lsstream/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-22 16:57:45.000000 lsstream-0.1.0/src/lsstream/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-22 16:57:45.000000 lsstream-0.1.0/src/lsstream/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-22 16:57:45.000000 lsstream-0.1.0/src/lsstream/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:57:56.196497 lsstream-0.1.0/src/lsstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-22 16:57:56.000000 lsstream-0.1.0/src/lsstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-22 16:57:56.000000 lsstream-0.1.0/src/lsstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:57:56.000000 lsstream-0.1.0/src/lsstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-22 16:57:56.000000 lsstream-0.1.0/src/lsstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 16:57:56.000000 lsstream-0.1.0/src/lsstream.egg-info/top_level.txt
```

### Comparing `lsstream-0.0.7/LICENSE` & `lsstream-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lsstream-0.0.7/PKG-INFO` & `lsstream-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsstream
-Version: 0.0.7
+Version: 0.1.0
 Summary: To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
 Author-email: Wermutton <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/Wermutton/lsstream
 Project-URL: Bug Tracker, https://github.com/Wermutton/lsstream/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lsstream-0.0.7/pyproject.toml` & `lsstream-0.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lsstream"
-version = "0.0.7"
+version = "0.1.0"
 authors = [
   { name="Wermutton", email="redacted@redacted.redacted" },
 ]
 description = "To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   "pyfiglet",
-  "termcolor"
+  "termcolor",
+  "colorama"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `lsstream-0.0.7/src/lsstream/file_generation.py` & `lsstream-0.1.0/src/lsstream/file_generation.py`

 * *Files identical despite different names*

### Comparing `lsstream-0.0.7/src/lsstream/main.py` & `lsstream-0.1.0/src/lsstream/main.py`

 * *Files identical despite different names*

### Comparing `lsstream-0.0.7/src/lsstream/prompts.py` & `lsstream-0.1.0/src/lsstream/prompts.py`

 * *Files identical despite different names*

### Comparing `lsstream-0.0.7/src/lsstream.egg-info/PKG-INFO` & `lsstream-0.1.0/src/lsstream.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsstream
-Version: 0.0.7
+Version: 0.1.0
 Summary: To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
 Author-email: Wermutton <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/Wermutton/lsstream
 Project-URL: Bug Tracker, https://github.com/Wermutton/lsstream/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

