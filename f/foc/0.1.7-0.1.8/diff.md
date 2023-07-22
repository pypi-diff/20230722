# Comparing `tmp/foc-0.1.7.tar.gz` & `tmp/foc-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foc-0.1.7.tar", last modified: Fri Jul 21 00:55:26 2023, max compression
+gzip compressed data, was "foc-0.1.8.tar", last modified: Sat Jul 22 15:28:12 2023, max compression
```

## Comparing `foc-0.1.7.tar` & `foc-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-21 00:55:26.150616 foc-0.1.7/
--rw-r--r--   0 thyeem     (501) staff       (20)      618 2023-07-21 00:54:37.000000 foc-0.1.7/ChangeLog.md
--rw-r--r--   0 thyeem     (501) staff       (20)     1068 2023-05-15 21:22:31.000000 foc-0.1.7/LICENSE
--rw-r--r--   0 thyeem     (501) staff       (20)       55 2023-06-06 23:18:02.000000 foc-0.1.7/MANIFEST.in
--rw-r--r--   0 thyeem     (501) staff       (20)    17346 2023-07-21 00:55:26.150961 foc-0.1.7/PKG-INFO
--rw-r--r--   0 thyeem     (501) staff       (20)    16885 2023-07-15 21:05:41.000000 foc-0.1.7/README.md
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-21 00:55:26.148212 foc-0.1.7/foc/
--rw-r--r--   0 thyeem     (501) staff       (20)    19825 2023-07-21 00:53:53.000000 foc-0.1.7/foc/__init__.py
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-21 00:55:26.149707 foc-0.1.7/foc.egg-info/
--rw-r--r--   0 thyeem     (501) staff       (20)    17346 2023-07-21 00:55:26.000000 foc-0.1.7/foc.egg-info/PKG-INFO
--rw-r--r--   0 thyeem     (501) staff       (20)      221 2023-07-21 00:55:26.000000 foc-0.1.7/foc.egg-info/SOURCES.txt
--rw-r--r--   0 thyeem     (501) staff       (20)        1 2023-07-21 00:55:26.000000 foc-0.1.7/foc.egg-info/dependency_links.txt
--rw-r--r--   0 thyeem     (501) staff       (20)       10 2023-07-21 00:55:26.000000 foc-0.1.7/foc.egg-info/top_level.txt
--rw-r--r--   0 thyeem     (501) staff       (20)      102 2023-07-21 00:55:26.151477 foc-0.1.7/setup.cfg
--rw-r--r--   0 thyeem     (501) staff       (20)      700 2023-07-21 00:54:54.000000 foc-0.1.7/setup.py
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-21 00:55:26.150183 foc-0.1.7/tests/
--rw-r--r--   0 thyeem     (501) staff       (20)        0 2023-06-11 20:28:50.000000 foc-0.1.7/tests/__init__.py
--rw-r--r--   0 thyeem     (501) staff       (20)     8338 2023-07-19 17:13:12.000000 foc-0.1.7/tests/test_foc.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-22 15:28:12.977149 foc-0.1.8/
+-rw-r--r--   0 thyeem     (501) staff       (20)      644 2023-07-22 15:22:35.000000 foc-0.1.8/ChangeLog.md
+-rw-r--r--   0 thyeem     (501) staff       (20)     1068 2023-06-07 00:06:02.000000 foc-0.1.8/LICENSE
+-rw-r--r--   0 thyeem     (501) staff       (20)       55 2023-06-07 00:06:02.000000 foc-0.1.8/MANIFEST.in
+-rw-r--r--   0 thyeem     (501) staff       (20)    17346 2023-07-22 15:28:12.977217 foc-0.1.8/PKG-INFO
+-rw-r--r--   0 thyeem     (501) staff       (20)    16885 2023-07-18 12:48:54.000000 foc-0.1.8/README.md
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-22 15:28:12.976268 foc-0.1.8/foc/
+-rw-r--r--   0 thyeem     (501) staff       (20)    20370 2023-07-22 15:19:41.000000 foc-0.1.8/foc/__init__.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-22 15:28:12.976733 foc-0.1.8/foc.egg-info/
+-rw-r--r--   0 thyeem     (501) staff       (20)    17346 2023-07-22 15:28:12.000000 foc-0.1.8/foc.egg-info/PKG-INFO
+-rw-r--r--   0 thyeem     (501) staff       (20)      221 2023-07-22 15:28:12.000000 foc-0.1.8/foc.egg-info/SOURCES.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)        1 2023-07-22 15:28:12.000000 foc-0.1.8/foc.egg-info/dependency_links.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)       10 2023-07-22 15:28:12.000000 foc-0.1.8/foc.egg-info/top_level.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)      102 2023-07-22 15:28:12.977448 foc-0.1.8/setup.cfg
+-rw-r--r--   0 thyeem     (501) staff       (20)      700 2023-07-22 15:22:53.000000 foc-0.1.8/setup.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-22 15:28:12.976922 foc-0.1.8/tests/
+-rw-r--r--   0 thyeem     (501) staff       (20)        0 2023-06-15 10:03:02.000000 foc-0.1.8/tests/__init__.py
+-rw-r--r--   0 thyeem     (501) staff       (20)     8338 2023-07-18 12:57:28.000000 foc-0.1.8/tests/test_foc.py
```

### Comparing `foc-0.1.7/ChangeLog.md` & `foc-0.1.8/ChangeLog.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,7 +21,10 @@
 # 0.1.6
 - Remove the unnecessary caching (possible memory leak)
 - Added `shuffle`
 - Improved `random_int`
 
 # 0.1.7
 - Added `const`, `until`, and `apply`
+
+# 0.1.8
+- Added `choice`
```

### Comparing `foc-0.1.7/LICENSE` & `foc-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `foc-0.1.7/PKG-INFO` & `foc-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foc
-Version: 0.1.7
+Version: 0.1.8
 Summary: A collection of python functions for somebody's sanity
 Home-page: https://github.com/thyeem/foc
 Author: Francis Lim
 Author-email: thyeem@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `foc-0.1.7/README.md` & `foc-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `foc-0.1.7/foc/__init__.py` & `foc-0.1.8/foc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,15 @@
     "basename",
     "mkdir",
     "rmdir",
     "bytes_to_int",
     "int_to_bytes",
     "random_bytes",
     "random_int",
+    "choice",
     "shuffle",
     "dmap",
     "fn_args",
     "singleton",
     "polling",
     "neatly",
     "nprint",
@@ -796,15 +797,15 @@
 
 def random_bytes(n):
     """generate cryptographically secure random bytes"""
     return os.urandom(n)
 
 
 def random_int(*args):
-    """generate random integer cryptographically secure and fast.
+    """generate random integer cryptographically secure and faster than numpy.
     return random integer(s) in range of [low, high)"""
 
     def rint(high, low=0):
         assert high > low, "Error, low >= high"
         x = high - low
         return low + (
             bytes_to_int(
@@ -828,14 +829,32 @@
     x = list(x)
     for i in range(len(x) - 1, 0, -1):
         j = random_int(0, i)
         x[i], x[j] = x[j], x[i]
     return x
 
 
+def choice(x, size=None, replace=False):
+    """Generate a sample with/without replacement from a given iterable"""
+    x = list(x)
+    if size is None:
+        return x[random_int(len(x))]
+    else:
+        size = int(len(x) * size) if 0 < size < 1 else size
+        replace = True if len(x) < size else replace
+        return [
+            x[i]
+            for i in (
+                random_int(0, len(x), size)
+                if replace
+                else shuffle(range(len(x)))[:size]
+            )
+        ]
+
+
 class dmap(dict):
     """dot-accessible dict(map)"""
 
     __delattr__ = dict.__delitem__
 
     def __getattr__(self, key):
         if key not in self and key != "_ipython_canary_method_should_not_exist_":
```

### Comparing `foc-0.1.7/foc.egg-info/PKG-INFO` & `foc-0.1.8/foc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foc
-Version: 0.1.7
+Version: 0.1.8
 Summary: A collection of python functions for somebody's sanity
 Home-page: https://github.com/thyeem/foc
 Author: Francis Lim
 Author-email: thyeem@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `foc-0.1.7/setup.py` & `foc-0.1.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="foc",
-    version="0.1.7",
+    version="0.1.8",
     author="Francis Lim",
     author_email="thyeem@gmail.com",
     description="A collection of python functions for somebody's sanity",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[],
     url="https://github.com/thyeem/foc",
```

### Comparing `foc-0.1.7/tests/test_foc.py` & `foc-0.1.8/tests/test_foc.py`

 * *Files identical despite different names*

