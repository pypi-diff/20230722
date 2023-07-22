# Comparing `tmp/nsj_queue_lib-0.0.2.tar.gz` & `tmp/nsj_queue_lib-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_queue_lib-0.0.2.tar", last modified: Sat Jul 22 18:40:15 2023, max compression
+gzip compressed data, was "nsj_queue_lib-0.1.0.tar", last modified: Sat Jul 22 20:31:06 2023, max compression
```

## Comparing `nsj_queue_lib-0.0.2.tar` & `nsj_queue_lib-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 18:40:15.777039 nsj_queue_lib-0.0.2/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2542 2023-07-22 18:40:15.777039 nsj_queue_lib-0.0.2/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1976 2023-07-21 22:40:47.000000 nsj_queue_lib-0.0.2/README.md
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 18:40:15.777039 nsj_queue_lib-0.0.2/nsj_queue_lib/
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 18:40:15.777039 nsj_queue_lib-0.0.2/nsj_queue_lib/nsj_queue_lib.egg-info/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2542 2023-07-22 18:40:15.000000 nsj_queue_lib-0.0.2/nsj_queue_lib/nsj_queue_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      320 2023-07-22 18:40:15.000000 nsj_queue_lib-0.0.2/nsj_queue_lib/nsj_queue_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-22 18:40:15.000000 nsj_queue_lib-0.0.2/nsj_queue_lib/nsj_queue_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       64 2023-07-22 18:40:15.000000 nsj_queue_lib-0.0.2/nsj_queue_lib/nsj_queue_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-22 18:40:15.000000 nsj_queue_lib-0.0.2/nsj_queue_lib/nsj_queue_lib.egg-info/top_level.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 22:32:09.000000 nsj_queue_lib-0.0.2/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      808 2023-07-22 18:40:15.777039 nsj_queue_lib-0.0.2/setup.cfg
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 18:40:15.777039 nsj_queue_lib-0.0.2/tests/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1284 2023-07-19 18:24:10.000000 nsj_queue_lib-0.0.2/tests/test_push_notification.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 20:31:06.088917 nsj_queue_lib-0.1.0/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2542 2023-07-22 20:31:06.088917 nsj_queue_lib-0.1.0/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1976 2023-07-21 22:40:47.000000 nsj_queue_lib-0.1.0/README.md
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 20:31:06.084917 nsj_queue_lib-0.1.0/nsj_queue_lib/
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 20:31:06.088917 nsj_queue_lib-0.1.0/nsj_queue_lib/nsj_queue_lib.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2542 2023-07-22 20:31:06.000000 nsj_queue_lib-0.1.0/nsj_queue_lib/nsj_queue_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      320 2023-07-22 20:31:06.000000 nsj_queue_lib-0.1.0/nsj_queue_lib/nsj_queue_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-22 20:31:06.000000 nsj_queue_lib-0.1.0/nsj_queue_lib/nsj_queue_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       64 2023-07-22 20:31:06.000000 nsj_queue_lib-0.1.0/nsj_queue_lib/nsj_queue_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-22 20:31:06.000000 nsj_queue_lib-0.1.0/nsj_queue_lib/nsj_queue_lib.egg-info/top_level.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 22:32:09.000000 nsj_queue_lib-0.1.0/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      808 2023-07-22 20:31:06.088917 nsj_queue_lib-0.1.0/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 20:31:06.088917 nsj_queue_lib-0.1.0/tests/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1284 2023-07-19 18:24:10.000000 nsj_queue_lib-0.1.0/tests/test_push_notification.py
```

### Comparing `nsj_queue_lib-0.0.2/PKG-INFO` & `nsj_queue_lib-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_queue_lib
-Version: 0.0.2
+Version: 0.1.0
 Summary: Biblioteca para facilitar a implementação de filas e workers.
 Home-page: https://github.com/Nasajon/nsj-queue-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-queue-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_queue_lib-0.0.2/README.md` & `nsj_queue_lib-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.0.2/nsj_queue_lib/nsj_queue_lib.egg-info/PKG-INFO` & `nsj_queue_lib-0.1.0/nsj_queue_lib/nsj_queue_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-queue-lib
-Version: 0.0.2
+Version: 0.1.0
 Summary: Biblioteca para facilitar a implementação de filas e workers.
 Home-page: https://github.com/Nasajon/nsj-queue-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-queue-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_queue_lib-0.0.2/setup.cfg` & `nsj_queue_lib-0.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_queue_lib
-version = 0.0.2
+version = 0.1.0
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para facilitar a implementação de filas e workers.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj-queue-lib
 project_urls =
```

### Comparing `nsj_queue_lib-0.0.2/tests/test_push_notification.py` & `nsj_queue_lib-0.1.0/tests/test_push_notification.py`

 * *Files identical despite different names*

