# Comparing `tmp/thunno2-2.2.2.tar.gz` & `tmp/thunno2-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.2.2.tar", last modified: Sun Jul  2 13:19:57 2023, max compression
+gzip compressed data, was "thunno2-2.2.3.tar", last modified: Sat Jul 22 09:30:10 2023, max compression
```

## Comparing `thunno2-2.2.2.tar` & `thunno2-2.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-02 13:19:57.759678 thunno2-2.2.2/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-07-02 13:19:57.759568 thunno2-2.2.2/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-07-02 13:19:57.759756 thunno2-2.2.2/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-05-30 13:16:32.000000 thunno2-2.2.2/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-02 13:19:57.758922 thunno2-2.2.2/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-05-01 12:43:53.000000 thunno2-2.2.2/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)     3268 2023-05-14 14:05:01.000000 thunno2-2.2.2/thunno2/autoexplanation.py
--rw-r--r--   0 nayak      (501) staff       (20)     1491 2023-05-11 17:22:25.000000 thunno2-2.2.2/thunno2/canvas.py
--rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.2.2/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    57155 2023-07-02 13:06:12.000000 thunno2-2.2.2/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     3046 2023-05-14 17:13:03.000000 thunno2-2.2.2/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.2.2/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     7303 2023-06-03 14:35:27.000000 thunno2-2.2.2/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    58798 2023-07-02 13:06:12.000000 thunno2-2.2.2/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    33291 2023-06-24 09:12:25.000000 thunno2-2.2.2/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    25968 2023-06-24 14:02:54.000000 thunno2-2.2.2/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     3440 2023-07-02 13:16:10.000000 thunno2-2.2.2/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    86444 2023-07-02 13:06:12.000000 thunno2-2.2.2/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     4505 2023-06-24 09:12:25.000000 thunno2-2.2.2/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-07-02 13:18:12.000000 thunno2-2.2.2/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-02 13:19:57.759423 thunno2-2.2.2/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-07-02 13:19:57.000000 thunno2-2.2.2/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      459 2023-07-02 13:19:57.000000 thunno2-2.2.2/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-07-02 13:19:57.000000 thunno2-2.2.2/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       54 2023-07-02 13:19:57.000000 thunno2-2.2.2/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-07-02 13:19:57.000000 thunno2-2.2.2/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-22 09:30:10.409415 thunno2-2.2.3/
+-rw-r--r--   0 nayak      (501) staff       (20)      940 2023-07-22 09:30:10.409199 thunno2-2.2.3/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-07-22 09:30:10.409471 thunno2-2.2.3/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-05-30 13:16:32.000000 thunno2-2.2.3/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-22 09:30:10.407814 thunno2-2.2.3/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-05-01 12:43:53.000000 thunno2-2.2.3/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3268 2023-05-14 14:05:01.000000 thunno2-2.2.3/thunno2/autoexplanation.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1491 2023-05-11 17:22:25.000000 thunno2-2.2.3/thunno2/canvas.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.2.3/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    57155 2023-07-02 13:06:12.000000 thunno2-2.2.3/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3046 2023-05-14 17:13:03.000000 thunno2-2.2.3/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.2.3/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     7303 2023-06-03 14:35:27.000000 thunno2-2.2.3/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    58811 2023-07-13 18:38:48.000000 thunno2-2.2.3/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    33317 2023-07-22 09:29:18.000000 thunno2-2.2.3/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    25968 2023-07-22 09:29:18.000000 thunno2-2.2.3/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3440 2023-07-02 13:16:10.000000 thunno2-2.2.3/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    86420 2023-07-13 18:37:15.000000 thunno2-2.2.3/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     4505 2023-06-24 09:12:25.000000 thunno2-2.2.3/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-07-22 09:29:12.000000 thunno2-2.2.3/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-22 09:30:10.408927 thunno2-2.2.3/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      940 2023-07-22 09:30:10.000000 thunno2-2.2.3/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      459 2023-07-22 09:30:10.000000 thunno2-2.2.3/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-07-22 09:30:10.000000 thunno2-2.2.3/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       53 2023-07-22 09:30:10.000000 thunno2-2.2.3/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-07-22 09:30:10.000000 thunno2-2.2.3/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.2.2/PKG-INFO` & `thunno2-2.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.2.2
+Version: 2.2.3
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.3.tar.gz
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.2.tar.gz
 Keywords: golfing,code-golf,language
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 
 Thunno is a golfing language written in Python. Learn more at https://github.com/Thunno/Thunno2
-
```

### Comparing `thunno2-2.2.2/setup.py` & `thunno2-2.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.2/thunno2/autoexplanation.py` & `thunno2-2.2.3/thunno2/autoexplanation.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.2/thunno2/canvas.py` & `thunno2-2.2.3/thunno2/canvas.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.2/thunno2/codepage.py` & `thunno2-2.2.3/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.2/thunno2/commands.py` & `thunno2-2.2.3/thunno2/commands.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.2/thunno2/constants.py` & `thunno2-2.2.3/thunno2/constants.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.2/thunno2/dictionary.py` & `thunno2-2.2.3/thunno2/dictionary.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.2/thunno2/flags.py` & `thunno2-2.2.3/thunno2/flags.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.2/thunno2/helpers.py` & `thunno2-2.2.3/thunno2/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1316,14 +1316,15 @@
 def vectorised_index_of(x, y):
     r = []
     for i in x:
         if isinstance(y, (str, list)):
             r.append(index_of(i, y))
         else:
             r.append(num_index_of(i, y))
+    return r
 
 
 def cartesian_product(x, y):
     return list(map(list, itertools.product(y, x)))
 
 
 def range_product1(n, y):
```

### Comparing `thunno2-2.2.2/thunno2/interpreter.py` & `thunno2-2.2.3/thunno2/interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -683,18 +683,18 @@
             r = []
             f1, f2 = info
             ctx.stack.push(a)
             k = f1()
             if k:
                 r.append(k[-1])
             ctx.stack = Stack(copy.deepcopy(old_stack))
-            ctx.stack.push(a)
             k = f2()
             if k:
                 r.append(k[-1])
+            ctx.stack = Stack(copy.deepcopy(old_stack))
             ctx.stack.push(r)
         elif desc == "recursive environment":
             a = next(ctx.stack.rmv(1))
             if isinstance(a, list):
                 x = copy.deepcopy(a)
             else:
                 x = [a]
```

### Comparing `thunno2-2.2.2/thunno2/lexer.py` & `thunno2-2.2.3/thunno2/lexer.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.2/thunno2/run.py` & `thunno2-2.2.3/thunno2/run.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.2/thunno2/tests.py` & `thunno2-2.2.3/thunno2/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,14 @@
 
 assert_eq(call("A", "abc"), 1)
 assert_eq(call("A", "123"), 0)
 assert_eq(call("A", ""), 0)
 assert_eq(call("A", ["a", ["b", ["1", ["2"]]]]), [1, [1, [0, [0]]]])
 
 assert_eq(call("A", ["abc", 123, "123", -0.123]), [1, 123, 0, 0.123])
-assert_eq(call("A"), 0)
 
 # B
 
 assert_eq(call("B", 2, 12), [1, 1, 0, 0])
 assert_eq(call("B", [100, 1000], 12345), [[1, 23, 45], [12, 345]])
 assert_eq(
     call("B", [0, 1, 2], [5, 10, 15]),
```

### Comparing `thunno2-2.2.2/thunno2/tokens.py` & `thunno2-2.2.3/thunno2/tokens.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.2/thunno2.egg-info/PKG-INFO` & `thunno2-2.2.3/thunno2.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.2.2
+Version: 2.2.3
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.3.tar.gz
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.2.tar.gz
 Keywords: golfing,code-golf,language
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 
 Thunno is a golfing language written in Python. Learn more at https://github.com/Thunno/Thunno2
-
```

