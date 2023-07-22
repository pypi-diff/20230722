# Comparing `tmp/pytest-xvirt-0.1.2.tar.gz` & `tmp/pytest-xvirt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/simone/Documents/python/pytest-xvirt/dist/.tmp-nhnm_wcq/pytest-xvirt-0.1.2.tar", last modified: Fri Jul 21 14:47:43 2023, max compression
+gzip compressed data, was "/home/simone/Documents/python/pytest-xvirt/dist/.tmp-9q0acwc2/pytest-xvirt-0.1.3.tar", last modified: Sat Jul 22 17:19:45 2023, max compression
```

## Comparing `pytest-xvirt-0.1.2.tar` & `pytest-xvirt-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/
--rw-rw-r--   0 simone    (1000) simone    (1000)     3248 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)     2046 2023-04-02 16:47:36.000000 pytest-xvirt-0.1.2/README.rst
--rw-rw-r--   0 simone    (1000) simone    (1000)      236 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/setup.cfg
--rw-rw-r--   0 simone    (1000) simone    (1000)     1708 2023-07-21 14:46:49.000000 pytest-xvirt-0.1.2/setup.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/
--rw-rw-r--   0 simone    (1000) simone    (1000)     3248 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)      578 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/SOURCES.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/dependency_links.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)       32 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/entry_points.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-15 17:04:00.000000 pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/not-zip-safe
--rw-rw-r--   0 simone    (1000) simone    (1000)       14 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/requires.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)       19 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/top_level.txt
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/xvirt/
--rw-rw-r--   0 simone    (1000) simone    (1000)      547 2023-07-20 14:54:06.000000 pytest-xvirt-0.1.2/src/xvirt/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      561 2023-05-14 17:39:36.000000 pytest-xvirt-0.1.2/src/xvirt/collectors.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/xvirt/empty/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-04-15 18:10:34.000000 pytest-xvirt-0.1.2/src/xvirt/empty/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1520 2023-05-14 17:23:30.000000 pytest-xvirt-0.1.2/src/xvirt/events.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1181 2023-07-21 14:31:51.000000 pytest-xvirt-0.1.2/src/xvirt/events_handler.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      202 2023-07-20 15:12:59.000000 pytest-xvirt-0.1.2/src/xvirt/newhooks.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2912 2023-07-21 14:29:29.000000 pytest-xvirt-0.1.2/src/xvirt/plugin.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/tests/
--rw-rw-r--   0 simone    (1000) simone    (1000)     1485 2023-05-21 16:30:01.000000 pytest-xvirt-0.1.2/tests/test_collectors.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      962 2023-07-21 14:34:52.000000 pytest-xvirt-0.1.2/tests/test_end2end.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1662 2023-07-20 15:12:59.000000 pytest-xvirt-0.1.2/tests/test_newhook_notify.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1705 2023-07-20 15:01:53.000000 pytest-xvirt-0.1.2/tests/test_newhook_setup.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-07-22 17:19:45.000000 pytest-xvirt-0.1.3/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3248 2023-07-22 17:19:45.000000 pytest-xvirt-0.1.3/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2046 2023-04-02 16:47:36.000000 pytest-xvirt-0.1.3/README.rst
+-rw-rw-r--   0 simone    (1000) simone    (1000)      236 2023-07-22 17:19:45.000000 pytest-xvirt-0.1.3/setup.cfg
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1708 2023-07-22 17:19:39.000000 pytest-xvirt-0.1.3/setup.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-07-22 17:19:45.000000 pytest-xvirt-0.1.3/src/
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-07-22 17:19:45.000000 pytest-xvirt-0.1.3/src/pytest_xvirt.egg-info/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3248 2023-07-22 17:19:45.000000 pytest-xvirt-0.1.3/src/pytest_xvirt.egg-info/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)      578 2023-07-22 17:19:45.000000 pytest-xvirt-0.1.3/src/pytest_xvirt.egg-info/SOURCES.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-07-22 17:19:45.000000 pytest-xvirt-0.1.3/src/pytest_xvirt.egg-info/dependency_links.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)       32 2023-07-22 17:19:45.000000 pytest-xvirt-0.1.3/src/pytest_xvirt.egg-info/entry_points.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-15 17:04:00.000000 pytest-xvirt-0.1.3/src/pytest_xvirt.egg-info/not-zip-safe
+-rw-rw-r--   0 simone    (1000) simone    (1000)       14 2023-07-22 17:19:45.000000 pytest-xvirt-0.1.3/src/pytest_xvirt.egg-info/requires.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)       19 2023-07-22 17:19:45.000000 pytest-xvirt-0.1.3/src/pytest_xvirt.egg-info/top_level.txt
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-07-22 17:19:45.000000 pytest-xvirt-0.1.3/src/xvirt/
+-rw-rw-r--   0 simone    (1000) simone    (1000)      547 2023-07-20 14:54:06.000000 pytest-xvirt-0.1.3/src/xvirt/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      561 2023-05-14 17:39:36.000000 pytest-xvirt-0.1.3/src/xvirt/collectors.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-07-22 17:19:45.000000 pytest-xvirt-0.1.3/src/xvirt/empty/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-04-15 18:10:34.000000 pytest-xvirt-0.1.3/src/xvirt/empty/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1520 2023-05-14 17:23:30.000000 pytest-xvirt-0.1.3/src/xvirt/events.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2319 2023-07-22 17:18:12.000000 pytest-xvirt-0.1.3/src/xvirt/events_handler.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      202 2023-07-20 15:12:59.000000 pytest-xvirt-0.1.3/src/xvirt/newhooks.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2912 2023-07-21 14:29:29.000000 pytest-xvirt-0.1.3/src/xvirt/plugin.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-07-22 17:19:45.000000 pytest-xvirt-0.1.3/tests/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1485 2023-05-21 16:30:01.000000 pytest-xvirt-0.1.3/tests/test_collectors.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      962 2023-07-21 14:34:52.000000 pytest-xvirt-0.1.3/tests/test_end2end.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1662 2023-07-20 15:12:59.000000 pytest-xvirt-0.1.3/tests/test_newhook_notify.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1705 2023-07-20 15:01:53.000000 pytest-xvirt-0.1.3/tests/test_newhook_setup.py
```

### Comparing `pytest-xvirt-0.1.2/PKG-INFO` & `pytest-xvirt-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-xvirt
-Version: 0.1.2
+Version: 0.1.3
 Summary: A pytest plugin to virtualize test. For example to transparently running them on a remote box.
 Home-page: https://github.com/www-py/pytest-xvirt
 Author: Simone Giacomelli, Fabrizio Lamarca
 Author-email: simone.giacomelli@gmail.com, lamarca.fabrizio@gmail.com
 Maintainer: Simone Giacomelli
 Maintainer-email: simone.giacomelli@gmail.com
 License: Apache 2.0
```

### Comparing `pytest-xvirt-0.1.2/README.rst` & `pytest-xvirt-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.2/setup.py` & `pytest-xvirt-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding='utf-8').read()
 
 
 setup(
     name='pytest-xvirt',
-    version='0.1.2',
+    version='0.1.3',
     author='Simone Giacomelli, Fabrizio Lamarca',
     author_email='simone.giacomelli@gmail.com, lamarca.fabrizio@gmail.com',
     maintainer='Simone Giacomelli',
     maintainer_email='simone.giacomelli@gmail.com',
     license='Apache 2.0',
     url='https://github.com/www-py/pytest-xvirt',
     description='A pytest plugin to virtualize test. For example to transparently running them on a remote box.',
```

### Comparing `pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/PKG-INFO` & `pytest-xvirt-0.1.3/src/pytest_xvirt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-xvirt
-Version: 0.1.2
+Version: 0.1.3
 Summary: A pytest plugin to virtualize test. For example to transparently running them on a remote box.
 Home-page: https://github.com/www-py/pytest-xvirt
 Author: Simone Giacomelli, Fabrizio Lamarca
 Author-email: simone.giacomelli@gmail.com, lamarca.fabrizio@gmail.com
 Maintainer: Simone Giacomelli
 Maintainer-email: simone.giacomelli@gmail.com
 License: Apache 2.0
```

### Comparing `pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/SOURCES.txt` & `pytest-xvirt-0.1.3/src/pytest_xvirt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.2/src/xvirt/__init__.py` & `pytest-xvirt-0.1.3/src/xvirt/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.2/src/xvirt/collectors.py` & `pytest-xvirt-0.1.3/src/xvirt/collectors.py`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.2/src/xvirt/events.py` & `pytest-xvirt-0.1.3/src/xvirt/events.py`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.2/src/xvirt/plugin.py` & `pytest-xvirt-0.1.3/src/xvirt/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.2/tests/test_collectors.py` & `pytest-xvirt-0.1.3/tests/test_collectors.py`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.2/tests/test_end2end.py` & `pytest-xvirt-0.1.3/tests/test_end2end.py`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.2/tests/test_newhook_notify.py` & `pytest-xvirt-0.1.3/tests/test_newhook_notify.py`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.2/tests/test_newhook_setup.py` & `pytest-xvirt-0.1.3/tests/test_newhook_setup.py`

 * *Files identical despite different names*

