# Comparing `tmp/thunno2-2.2.3.tar.gz` & `tmp/thunno2-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.2.3.tar", last modified: Sat Jul 22 09:30:10 2023, max compression
+gzip compressed data, was "thunno2-2.2.4.tar", last modified: Sat Jul 22 09:35:31 2023, max compression
```

## Comparing `thunno2-2.2.3.tar` & `thunno2-2.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-22 09:30:10.409415 thunno2-2.2.3/
--rw-r--r--   0 nayak      (501) staff       (20)      940 2023-07-22 09:30:10.409199 thunno2-2.2.3/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-07-22 09:30:10.409471 thunno2-2.2.3/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-05-30 13:16:32.000000 thunno2-2.2.3/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-22 09:30:10.407814 thunno2-2.2.3/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-05-01 12:43:53.000000 thunno2-2.2.3/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)     3268 2023-05-14 14:05:01.000000 thunno2-2.2.3/thunno2/autoexplanation.py
--rw-r--r--   0 nayak      (501) staff       (20)     1491 2023-05-11 17:22:25.000000 thunno2-2.2.3/thunno2/canvas.py
--rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.2.3/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    57155 2023-07-02 13:06:12.000000 thunno2-2.2.3/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     3046 2023-05-14 17:13:03.000000 thunno2-2.2.3/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.2.3/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     7303 2023-06-03 14:35:27.000000 thunno2-2.2.3/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    58811 2023-07-13 18:38:48.000000 thunno2-2.2.3/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    33317 2023-07-22 09:29:18.000000 thunno2-2.2.3/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    25968 2023-07-22 09:29:18.000000 thunno2-2.2.3/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     3440 2023-07-02 13:16:10.000000 thunno2-2.2.3/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    86420 2023-07-13 18:37:15.000000 thunno2-2.2.3/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     4505 2023-06-24 09:12:25.000000 thunno2-2.2.3/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-07-22 09:29:12.000000 thunno2-2.2.3/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-22 09:30:10.408927 thunno2-2.2.3/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      940 2023-07-22 09:30:10.000000 thunno2-2.2.3/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      459 2023-07-22 09:30:10.000000 thunno2-2.2.3/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-07-22 09:30:10.000000 thunno2-2.2.3/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       53 2023-07-22 09:30:10.000000 thunno2-2.2.3/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-07-22 09:30:10.000000 thunno2-2.2.3/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-22 09:35:31.115307 thunno2-2.2.4/
+-rw-r--r--   0 nayak      (501) staff       (20)      940 2023-07-22 09:35:31.115200 thunno2-2.2.4/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-07-22 09:35:31.115340 thunno2-2.2.4/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-05-30 13:16:32.000000 thunno2-2.2.4/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-22 09:35:31.114532 thunno2-2.2.4/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-05-01 12:43:53.000000 thunno2-2.2.4/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3268 2023-05-14 14:05:01.000000 thunno2-2.2.4/thunno2/autoexplanation.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1491 2023-05-11 17:22:25.000000 thunno2-2.2.4/thunno2/canvas.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.2.4/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    57155 2023-07-02 13:06:12.000000 thunno2-2.2.4/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3046 2023-05-14 17:13:03.000000 thunno2-2.2.4/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.2.4/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     7303 2023-06-03 14:35:27.000000 thunno2-2.2.4/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    58811 2023-07-13 18:38:48.000000 thunno2-2.2.4/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    33317 2023-07-22 09:29:18.000000 thunno2-2.2.4/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    25968 2023-07-22 09:29:18.000000 thunno2-2.2.4/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3440 2023-07-02 13:16:10.000000 thunno2-2.2.4/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    86420 2023-07-13 18:37:15.000000 thunno2-2.2.4/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     4505 2023-06-24 09:12:25.000000 thunno2-2.2.4/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-07-22 09:34:42.000000 thunno2-2.2.4/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-07-22 09:35:31.115059 thunno2-2.2.4/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      940 2023-07-22 09:35:31.000000 thunno2-2.2.4/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      459 2023-07-22 09:35:31.000000 thunno2-2.2.4/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-07-22 09:35:31.000000 thunno2-2.2.4/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       53 2023-07-22 09:35:31.000000 thunno2-2.2.4/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-07-22 09:35:31.000000 thunno2-2.2.4/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.2.3/PKG-INFO` & `thunno2-2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.2.3
+Version: 2.2.4
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.3.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.4.tar.gz
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
 Keywords: golfing,code-golf,language
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `thunno2-2.2.3/setup.py` & `thunno2-2.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.3/thunno2/autoexplanation.py` & `thunno2-2.2.4/thunno2/autoexplanation.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.3/thunno2/canvas.py` & `thunno2-2.2.4/thunno2/canvas.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.3/thunno2/codepage.py` & `thunno2-2.2.4/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.3/thunno2/commands.py` & `thunno2-2.2.4/thunno2/commands.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.3/thunno2/constants.py` & `thunno2-2.2.4/thunno2/constants.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.3/thunno2/dictionary.py` & `thunno2-2.2.4/thunno2/dictionary.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.3/thunno2/flags.py` & `thunno2-2.2.4/thunno2/flags.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.3/thunno2/helpers.py` & `thunno2-2.2.4/thunno2/helpers.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.3/thunno2/interpreter.py` & `thunno2-2.2.4/thunno2/interpreter.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.3/thunno2/lexer.py` & `thunno2-2.2.4/thunno2/lexer.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.3/thunno2/run.py` & `thunno2-2.2.4/thunno2/run.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.3/thunno2/tests.py` & `thunno2-2.2.4/thunno2/tests.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.3/thunno2/tokens.py` & `thunno2-2.2.4/thunno2/tokens.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.2.3/thunno2.egg-info/PKG-INFO` & `thunno2-2.2.4/thunno2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.2.3
+Version: 2.2.4
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.3.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.2.4.tar.gz
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
 Keywords: golfing,code-golf,language
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

