# Comparing `tmp/scraid-0.11.tar.gz` & `tmp/scraid-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scraid-0.11.tar", last modified: Thu Jul 20 15:51:47 2023, max compression
+gzip compressed data, was "scraid-0.12.tar", last modified: Sat Jul 22 08:23:35 2023, max compression
```

## Comparing `scraid-0.11.tar` & `scraid-0.12.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 yamed     (1000) yamed     (1000)        0 2023-07-20 15:51:47.714409 scraid-0.11/
--rw-rw-r--   0 yamed     (1000) yamed     (1000)     1457 2023-07-20 15:51:47.714409 scraid-0.11/PKG-INFO
--rw-rw-r--   0 yamed     (1000) yamed     (1000)      822 2023-07-20 15:09:48.000000 scraid-0.11/README.md
-drwxrwxr-x   0 yamed     (1000) yamed     (1000)        0 2023-07-20 15:51:47.714409 scraid-0.11/scraid/
--rw-rw-r--   0 yamed     (1000) yamed     (1000)        0 2023-07-20 14:51:49.000000 scraid-0.11/scraid/__init__.py
--rw-rw-r--   0 yamed     (1000) yamed     (1000)      580 2023-07-20 14:52:50.000000 scraid-0.11/scraid/advanced_request.py
-drwxrwxr-x   0 yamed     (1000) yamed     (1000)        0 2023-07-20 15:51:47.714409 scraid-0.11/scraid.egg-info/
--rw-rw-r--   0 yamed     (1000) yamed     (1000)     1457 2023-07-20 15:51:47.000000 scraid-0.11/scraid.egg-info/PKG-INFO
--rw-rw-r--   0 yamed     (1000) yamed     (1000)      262 2023-07-20 15:51:47.000000 scraid-0.11/scraid.egg-info/SOURCES.txt
--rw-rw-r--   0 yamed     (1000) yamed     (1000)        1 2023-07-20 15:51:47.000000 scraid-0.11/scraid.egg-info/dependency_links.txt
--rw-rw-r--   0 yamed     (1000) yamed     (1000)       22 2023-07-20 15:51:47.000000 scraid-0.11/scraid.egg-info/requires.txt
--rw-rw-r--   0 yamed     (1000) yamed     (1000)       13 2023-07-20 15:51:47.000000 scraid-0.11/scraid.egg-info/top_level.txt
--rw-rw-r--   0 yamed     (1000) yamed     (1000)       38 2023-07-20 15:51:47.714409 scraid-0.11/setup.cfg
--rw-rw-r--   0 yamed     (1000) yamed     (1000)      888 2023-07-20 15:47:16.000000 scraid-0.11/setup.py
-drwxrwxr-x   0 yamed     (1000) yamed     (1000)        0 2023-07-20 15:51:47.714409 scraid-0.11/tests/
--rw-rw-r--   0 yamed     (1000) yamed     (1000)        0 2023-07-20 14:53:26.000000 scraid-0.11/tests/__init__.py
--rw-rw-r--   0 yamed     (1000) yamed     (1000)      364 2023-07-20 14:53:42.000000 scraid-0.11/tests/test_advanced_request.py
+drwxrwxr-x   0 egon      (1000) egon      (1000)        0 2023-07-22 08:23:35.871864 scraid-0.12/
+-rw-rw-r--   0 egon      (1000) egon      (1000)     1508 2023-07-22 08:23:35.871864 scraid-0.12/PKG-INFO
+-rw-rw-r--   0 egon      (1000) egon      (1000)      822 2023-07-22 08:18:07.000000 scraid-0.12/README.md
+drwxrwxr-x   0 egon      (1000) egon      (1000)        0 2023-07-22 08:23:35.871864 scraid-0.12/scraid/
+-rw-rw-r--   0 egon      (1000) egon      (1000)        0 2023-07-22 08:18:07.000000 scraid-0.12/scraid/__init__.py
+-rw-rw-r--   0 egon      (1000) egon      (1000)      578 2023-07-22 08:20:12.000000 scraid-0.12/scraid/advanced_request.py
+drwxrwxr-x   0 egon      (1000) egon      (1000)        0 2023-07-22 08:23:35.871864 scraid-0.12/scraid.egg-info/
+-rw-rw-r--   0 egon      (1000) egon      (1000)     1508 2023-07-22 08:23:35.000000 scraid-0.12/scraid.egg-info/PKG-INFO
+-rw-rw-r--   0 egon      (1000) egon      (1000)      262 2023-07-22 08:23:35.000000 scraid-0.12/scraid.egg-info/SOURCES.txt
+-rw-rw-r--   0 egon      (1000) egon      (1000)        1 2023-07-22 08:23:35.000000 scraid-0.12/scraid.egg-info/dependency_links.txt
+-rw-rw-r--   0 egon      (1000) egon      (1000)       22 2023-07-22 08:23:35.000000 scraid-0.12/scraid.egg-info/requires.txt
+-rw-rw-r--   0 egon      (1000) egon      (1000)       13 2023-07-22 08:23:35.000000 scraid-0.12/scraid.egg-info/top_level.txt
+-rw-rw-r--   0 egon      (1000) egon      (1000)       38 2023-07-22 08:23:35.871864 scraid-0.12/setup.cfg
+-rw-rw-r--   0 egon      (1000) egon      (1000)      939 2023-07-22 08:23:26.000000 scraid-0.12/setup.py
+drwxrwxr-x   0 egon      (1000) egon      (1000)        0 2023-07-22 08:23:35.871864 scraid-0.12/tests/
+-rw-rw-r--   0 egon      (1000) egon      (1000)        0 2023-07-22 08:18:07.000000 scraid-0.12/tests/__init__.py
+-rw-rw-r--   0 egon      (1000) egon      (1000)      419 2023-07-22 08:18:07.000000 scraid-0.12/tests/test_advanced_request.py
```

### Comparing `scraid-0.11/PKG-INFO` & `scraid-0.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: scraid
-Version: 0.11
+Version: 0.12
 Summary: A package for advanced Scrapy functionality and utilities.
 Home-page: https://github.com/na0495/scraid
 Author: na0495
 Author-email: saad.mrabet@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 # Scraid
 
 scraid is a Python library that provides advanced utilities for Scrapy, including an advanced features and utilities.
 
 ## Installation
```

### Comparing `scraid-0.11/README.md` & `scraid-0.12/README.md`

 * *Files identical despite different names*

### Comparing `scraid-0.11/scraid/advanced_request.py` & `scraid-0.12/scraid/advanced_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-
 from scrapy import Request
 from fake_useragent import UserAgent
 
-# ----------------------------------------------------------    
+# ----------------------------------------------------------
+
 
 class AdvancedRequest(Request):
     """
         AdvancedRequest is a subclass of scrapy.Request that sets a random User-Agent header for each request,
         using the fake-useragent package, to avoid being blocked by websites that detect and block spiders.
     """
+
     def __init__(self, *args, **kwargs):
         headers = {'User-Agent': UserAgent().random}
         kwargs.setdefault('headers', headers)
-        super().__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
```

### Comparing `scraid-0.11/scraid.egg-info/PKG-INFO` & `scraid-0.12/scraid.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: scraid
-Version: 0.11
+Version: 0.12
 Summary: A package for advanced Scrapy functionality and utilities.
 Home-page: https://github.com/na0495/scraid
 Author: na0495
 Author-email: saad.mrabet@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 # Scraid
 
 scraid is a Python library that provides advanced utilities for Scrapy, including an advanced features and utilities.
 
 ## Installation
```

### Comparing `scraid-0.11/setup.py` & `scraid-0.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
-# ----------------------------------------- 
+# -----------------------------------------
 
 setup(
     name='scraid',
-    version='0.11',
+    version='0.12',
     packages=find_packages(),
     install_requires=[
         'scrapy',
         'fake_useragent',
     ],
     author='na0495',
     author_email='saad.mrabet@example.com',
@@ -20,9 +20,11 @@
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+
     ],
-)
+)
```

