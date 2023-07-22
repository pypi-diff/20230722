# Comparing `tmp/c_l_testing-0.0.6a0.tar.gz` & `tmp/c_l_testing-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c_l_testing-0.0.6a0.tar", last modified: Sat Jul 22 18:25:41 2023, max compression
+gzip compressed data, was "c_l_testing-0.0.8.tar", last modified: Sat Jul 22 18:58:44 2023, max compression
```

## Comparing `c_l_testing-0.0.6a0.tar` & `c_l_testing-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 justin.anzalone   (501) staff       (20)        0 2023-07-22 18:25:41.197940 c_l_testing-0.0.6a0/
--rw-r--r--   0 justin.anzalone   (501) staff       (20)    11343 2023-07-22 16:32:00.000000 c_l_testing-0.0.6a0/LICENSE
--rw-r--r--   0 justin.anzalone   (501) staff       (20)     7948 2023-07-22 18:25:41.197996 c_l_testing-0.0.6a0/PKG-INFO
--rw-r--r--   0 justin.anzalone   (501) staff       (20)     6911 2023-07-22 17:28:55.000000 c_l_testing-0.0.6a0/README.rst
-drwxr-xr-x   0 justin.anzalone   (501) staff       (20)        0 2023-07-22 18:25:41.195908 c_l_testing-0.0.6a0/c_l_testing.egg-info/
--rw-r--r--   0 justin.anzalone   (501) staff       (20)     7948 2023-07-22 18:25:41.000000 c_l_testing-0.0.6a0/c_l_testing.egg-info/PKG-INFO
--rw-r--r--   0 justin.anzalone   (501) staff       (20)      593 2023-07-22 18:25:41.000000 c_l_testing-0.0.6a0/c_l_testing.egg-info/SOURCES.txt
--rw-r--r--   0 justin.anzalone   (501) staff       (20)        1 2023-07-22 18:25:41.000000 c_l_testing-0.0.6a0/c_l_testing.egg-info/dependency_links.txt
--rw-r--r--   0 justin.anzalone   (501) staff       (20)       15 2023-07-22 18:25:41.000000 c_l_testing-0.0.6a0/c_l_testing.egg-info/requires.txt
--rw-r--r--   0 justin.anzalone   (501) staff       (20)       14 2023-07-22 18:25:41.000000 c_l_testing-0.0.6a0/c_l_testing.egg-info/top_level.txt
-drwxr-xr-x   0 justin.anzalone   (501) staff       (20)        0 2023-07-22 18:25:41.197147 c_l_testing-0.0.6a0/carson_living/
--rw-r--r--   0 justin.anzalone   (501) staff       (20)     1936 2023-07-22 16:32:00.000000 c_l_testing-0.0.6a0/carson_living/__init__.py
--rw-r--r--   0 justin.anzalone   (501) staff       (20)     6258 2023-07-22 18:22:08.000000 c_l_testing-0.0.6a0/carson_living/auth.py
--rw-r--r--   0 justin.anzalone   (501) staff       (20)     2461 2023-07-22 16:32:00.000000 c_l_testing-0.0.6a0/carson_living/carson.py
--rw-r--r--   0 justin.anzalone   (501) staff       (20)    12625 2023-07-22 16:32:00.000000 c_l_testing-0.0.6a0/carson_living/carson_entities.py
--rw-r--r--   0 justin.anzalone   (501) staff       (20)     1342 2023-07-22 16:32:00.000000 c_l_testing-0.0.6a0/carson_living/const.py
--rw-r--r--   0 justin.anzalone   (501) staff       (20)     5924 2023-07-22 16:32:00.000000 c_l_testing-0.0.6a0/carson_living/eagleeye.py
--rw-r--r--   0 justin.anzalone   (501) staff       (20)    11381 2023-07-22 16:32:00.000000 c_l_testing-0.0.6a0/carson_living/eagleeye_entities.py
--rw-r--r--   0 justin.anzalone   (501) staff       (20)     3616 2023-07-22 16:32:00.000000 c_l_testing-0.0.6a0/carson_living/entities.py
--rw-r--r--   0 justin.anzalone   (501) staff       (20)      475 2023-07-22 16:32:00.000000 c_l_testing-0.0.6a0/carson_living/error.py
--rw-r--r--   0 justin.anzalone   (501) staff       (20)     2970 2023-07-22 16:32:00.000000 c_l_testing-0.0.6a0/carson_living/util.py
--rw-r--r--   0 justin.anzalone   (501) staff       (20)      178 2023-07-22 18:25:41.198197 c_l_testing-0.0.6a0/setup.cfg
--rw-r--r--   0 justin.anzalone   (501) staff       (20)     1482 2023-07-22 18:25:13.000000 c_l_testing-0.0.6a0/setup.py
-drwxr-xr-x   0 justin.anzalone   (501) staff       (20)        0 2023-07-22 18:25:41.197832 c_l_testing-0.0.6a0/tests/
--rw-r--r--   0 justin.anzalone   (501) staff       (20)     7368 2023-07-22 16:32:00.000000 c_l_testing-0.0.6a0/tests/test_auth.py
--rw-r--r--   0 justin.anzalone   (501) staff       (20)     2244 2023-07-22 16:32:00.000000 c_l_testing-0.0.6a0/tests/test_base.py
--rw-r--r--   0 justin.anzalone   (501) staff       (20)    10427 2023-07-22 16:32:00.000000 c_l_testing-0.0.6a0/tests/test_camera.py
--rw-r--r--   0 justin.anzalone   (501) staff       (20)     6566 2023-07-22 16:32:00.000000 c_l_testing-0.0.6a0/tests/test_carson.py
--rw-r--r--   0 justin.anzalone   (501) staff       (20)     2822 2023-07-22 16:32:00.000000 c_l_testing-0.0.6a0/tests/test_door.py
--rw-r--r--   0 justin.anzalone   (501) staff       (20)     4207 2023-07-22 16:32:00.000000 c_l_testing-0.0.6a0/tests/test_eagleeye.py
+drwxr-xr-x   0 justin.anzalone   (501) staff       (20)        0 2023-07-22 18:58:44.297748 c_l_testing-0.0.8/
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)    11343 2023-07-22 16:32:00.000000 c_l_testing-0.0.8/LICENSE
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)     7946 2023-07-22 18:58:44.297808 c_l_testing-0.0.8/PKG-INFO
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)     6911 2023-07-22 17:28:55.000000 c_l_testing-0.0.8/README.rst
+drwxr-xr-x   0 justin.anzalone   (501) staff       (20)        0 2023-07-22 18:58:44.295519 c_l_testing-0.0.8/c_l_testing.egg-info/
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)     7946 2023-07-22 18:58:44.000000 c_l_testing-0.0.8/c_l_testing.egg-info/PKG-INFO
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)      593 2023-07-22 18:58:44.000000 c_l_testing-0.0.8/c_l_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)        1 2023-07-22 18:58:44.000000 c_l_testing-0.0.8/c_l_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)       15 2023-07-22 18:58:44.000000 c_l_testing-0.0.8/c_l_testing.egg-info/requires.txt
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)       14 2023-07-22 18:58:44.000000 c_l_testing-0.0.8/c_l_testing.egg-info/top_level.txt
+drwxr-xr-x   0 justin.anzalone   (501) staff       (20)        0 2023-07-22 18:58:44.296786 c_l_testing-0.0.8/carson_living/
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)     1936 2023-07-22 16:32:00.000000 c_l_testing-0.0.8/carson_living/__init__.py
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)     6604 2023-07-22 18:56:24.000000 c_l_testing-0.0.8/carson_living/auth.py
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)     2461 2023-07-22 16:32:00.000000 c_l_testing-0.0.8/carson_living/carson.py
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)    12625 2023-07-22 16:32:00.000000 c_l_testing-0.0.8/carson_living/carson_entities.py
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)     1342 2023-07-22 16:32:00.000000 c_l_testing-0.0.8/carson_living/const.py
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)     5924 2023-07-22 16:32:00.000000 c_l_testing-0.0.8/carson_living/eagleeye.py
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)    11381 2023-07-22 16:32:00.000000 c_l_testing-0.0.8/carson_living/eagleeye_entities.py
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)     3616 2023-07-22 16:32:00.000000 c_l_testing-0.0.8/carson_living/entities.py
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)      475 2023-07-22 16:32:00.000000 c_l_testing-0.0.8/carson_living/error.py
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)     2970 2023-07-22 16:32:00.000000 c_l_testing-0.0.8/carson_living/util.py
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)      178 2023-07-22 18:58:44.298007 c_l_testing-0.0.8/setup.cfg
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)     1481 2023-07-22 18:58:09.000000 c_l_testing-0.0.8/setup.py
+drwxr-xr-x   0 justin.anzalone   (501) staff       (20)        0 2023-07-22 18:58:44.297627 c_l_testing-0.0.8/tests/
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)     7368 2023-07-22 16:32:00.000000 c_l_testing-0.0.8/tests/test_auth.py
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)     2244 2023-07-22 16:32:00.000000 c_l_testing-0.0.8/tests/test_base.py
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)    10427 2023-07-22 16:32:00.000000 c_l_testing-0.0.8/tests/test_camera.py
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)     6566 2023-07-22 16:32:00.000000 c_l_testing-0.0.8/tests/test_carson.py
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)     2822 2023-07-22 16:32:00.000000 c_l_testing-0.0.8/tests/test_door.py
+-rw-r--r--   0 justin.anzalone   (501) staff       (20)     4207 2023-07-22 16:32:00.000000 c_l_testing-0.0.8/tests/test_eagleeye.py
```

### Comparing `c_l_testing-0.0.6a0/LICENSE` & `c_l_testing-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `c_l_testing-0.0.6a0/PKG-INFO` & `c_l_testing-0.0.8/c_l_testing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: c_l_testing
-Version: 0.0.6a0
+Name: c-l-testing
+Version: 0.0.8
 Summary: A Python library to communicate with Carson Living Residences (https://www.carson.live/)
 Home-page: https://github.com/justanz/python-carson-living-testing
 Author: Martin Riedel
 Author-email: web@riedel-it.de
 License: Apache License 2.0
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `c_l_testing-0.0.6a0/README.rst` & `c_l_testing-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `c_l_testing-0.0.6a0/c_l_testing.egg-info/PKG-INFO` & `c_l_testing-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: c-l-testing
-Version: 0.0.6a0
+Name: c_l_testing
+Version: 0.0.8
 Summary: A Python library to communicate with Carson Living Residences (https://www.carson.live/)
 Home-page: https://github.com/justanz/python-carson-living-testing
 Author: Martin Riedel
 Author-email: web@riedel-it.de
 License: Apache License 2.0
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `c_l_testing-0.0.6a0/c_l_testing.egg-info/SOURCES.txt` & `c_l_testing-0.0.8/c_l_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `c_l_testing-0.0.6a0/carson_living/__init__.py` & `c_l_testing-0.0.8/carson_living/__init__.py`

 * *Files identical despite different names*

### Comparing `c_l_testing-0.0.6a0/carson_living/auth.py` & `c_l_testing-0.0.8/carson_living/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,15 +99,23 @@
         """
         if token is None:
             self._token = None
             self._token_payload = None
             self._token_expiration_time = None
             return
         try:
-            self._token_payload = jwt.decode(token, key=public_key, algorithms=["ES256"])
+            self._token_payload = jwt.decode(
+                token,
+                key="",  # The key used for signature verification. This should be provided by the service provider.
+                algorithms=["HS256"],  # The algorithm used for signature verification.
+                options={
+                    "verify_signature": False,  # This is equivalent to the old `verify=False` option.
+                }
+            )
+
             self._token_expiration_time = self._token_payload.get('exp')
 
             self._token = token
 
             if self._token_update_cb is not None:
                 self._token_update_cb(token)
             _LOGGER.info('Set access Token for %s',
```

### Comparing `c_l_testing-0.0.6a0/carson_living/carson.py` & `c_l_testing-0.0.8/carson_living/carson.py`

 * *Files identical despite different names*

### Comparing `c_l_testing-0.0.6a0/carson_living/carson_entities.py` & `c_l_testing-0.0.8/carson_living/carson_entities.py`

 * *Files identical despite different names*

### Comparing `c_l_testing-0.0.6a0/carson_living/const.py` & `c_l_testing-0.0.8/carson_living/const.py`

 * *Files identical despite different names*

### Comparing `c_l_testing-0.0.6a0/carson_living/eagleeye.py` & `c_l_testing-0.0.8/carson_living/eagleeye.py`

 * *Files identical despite different names*

### Comparing `c_l_testing-0.0.6a0/carson_living/eagleeye_entities.py` & `c_l_testing-0.0.8/carson_living/eagleeye_entities.py`

 * *Files identical despite different names*

### Comparing `c_l_testing-0.0.6a0/carson_living/entities.py` & `c_l_testing-0.0.8/carson_living/entities.py`

 * *Files identical despite different names*

### Comparing `c_l_testing-0.0.6a0/carson_living/util.py` & `c_l_testing-0.0.8/carson_living/util.py`

 * *Files identical despite different names*

### Comparing `c_l_testing-0.0.6a0/setup.py` & `c_l_testing-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding=utf-8
 """Python Carson Living setup script."""
 from setuptools import setup
 
-_VERSION = '0.0.6a'
+_VERSION = '0.0.8'
 
 
 def readme():
     """Pipe README.rst"""
     with open('README.rst') as desc:
         return desc.read()
```

### Comparing `c_l_testing-0.0.6a0/tests/test_auth.py` & `c_l_testing-0.0.8/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `c_l_testing-0.0.6a0/tests/test_base.py` & `c_l_testing-0.0.8/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `c_l_testing-0.0.6a0/tests/test_camera.py` & `c_l_testing-0.0.8/tests/test_camera.py`

 * *Files identical despite different names*

### Comparing `c_l_testing-0.0.6a0/tests/test_carson.py` & `c_l_testing-0.0.8/tests/test_carson.py`

 * *Files identical despite different names*

### Comparing `c_l_testing-0.0.6a0/tests/test_door.py` & `c_l_testing-0.0.8/tests/test_door.py`

 * *Files identical despite different names*

### Comparing `c_l_testing-0.0.6a0/tests/test_eagleeye.py` & `c_l_testing-0.0.8/tests/test_eagleeye.py`

 * *Files identical despite different names*

