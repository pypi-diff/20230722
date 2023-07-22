# Comparing `tmp/finterstellar-0.2.19.tar.gz` & `tmp/finterstellar-0.2.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finterstellar-0.2.19.tar", last modified: Sat Jul 22 08:21:43 2023, max compression
+gzip compressed data, was "finterstellar-0.2.20.tar", last modified: Sat Jul 22 08:40:15 2023, max compression
```

## Comparing `finterstellar-0.2.19.tar` & `finterstellar-0.2.20.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 08:21:43.215000 finterstellar-0.2.19/
--rw-rw-rw-   0        0        0     1089 2021-03-08 19:23:15.000000 finterstellar-0.2.19/License
--rw-rw-rw-   0        0        0      575 2023-07-22 08:21:43.210000 finterstellar-0.2.19/PKG-INFO
--rw-rw-rw-   0        0        0      105 2021-03-08 19:32:22.000000 finterstellar-0.2.19/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 08:21:43.101000 finterstellar-0.2.19/finterstellar/
--rw-rw-rw-   0        0        0      211 2023-07-22 08:19:20.000000 finterstellar-0.2.19/finterstellar/__init__.py
--rw-rw-rw-   0        0        0     4793 2023-07-22 06:05:37.000000 finterstellar-0.2.19/finterstellar/data_prep.py
--rw-rw-rw-   0        0        0    12206 2023-07-22 06:05:37.000000 finterstellar-0.2.19/finterstellar/financials.py
--rw-rw-rw-   0        0        0     3966 2023-07-22 08:19:33.000000 finterstellar-0.2.19/finterstellar/krx.py
--rw-rw-rw-   0        0        0     7919 2023-07-22 06:05:37.000000 finterstellar-0.2.19/finterstellar/trading.py
--rw-rw-rw-   0        0        0     3800 2023-07-22 06:05:37.000000 finterstellar-0.2.19/finterstellar/trend.py
--rw-rw-rw-   0        0        0     7332 2023-07-22 06:05:37.000000 finterstellar-0.2.19/finterstellar/visualization.py
-drwxrwxrwx   0        0        0        0 2023-07-22 08:21:43.137000 finterstellar-0.2.19/finterstellar.egg-info/
--rw-rw-rw-   0        0        0      575 2023-07-22 08:21:42.000000 finterstellar-0.2.19/finterstellar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      580 2023-07-22 08:21:42.000000 finterstellar-0.2.19/finterstellar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 08:21:42.000000 finterstellar-0.2.19/finterstellar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-22 08:21:42.000000 finterstellar-0.2.19/finterstellar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-07-22 08:21:42.000000 finterstellar-0.2.19/finterstellar.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-22 08:21:43.205000 finterstellar-0.2.19/finterstellar_/
--rw-rw-rw-   0        0        0      214 2023-02-12 02:23:43.000000 finterstellar-0.2.19/finterstellar_/__init__.py
--rw-rw-rw-   0        0        0     5336 2023-02-12 02:23:43.000000 finterstellar-0.2.19/finterstellar_/data_prep.py
--rw-rw-rw-   0        0        0    12206 2023-02-12 02:23:43.000000 finterstellar-0.2.19/finterstellar_/financials.py
--rw-rw-rw-   0        0        0     7722 2023-02-12 02:23:43.000000 finterstellar-0.2.19/finterstellar_/trading.py
--rw-rw-rw-   0        0        0     3706 2023-02-12 02:23:43.000000 finterstellar-0.2.19/finterstellar_/trend.py
--rw-rw-rw-   0        0        0     2374 2023-02-12 02:23:43.000000 finterstellar-0.2.19/finterstellar_/util.py
--rw-rw-rw-   0        0        0     7137 2023-02-12 02:23:43.000000 finterstellar-0.2.19/finterstellar_/visualization.py
--rw-rw-rw-   0        0        0       42 2023-07-22 08:21:43.214000 finterstellar-0.2.19/setup.cfg
--rw-rw-rw-   0        0        0      827 2023-07-22 08:20:31.000000 finterstellar-0.2.19/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:40:15.751000 finterstellar-0.2.20/
+-rw-rw-rw-   0        0        0     1089 2021-03-08 19:23:15.000000 finterstellar-0.2.20/License
+-rw-rw-rw-   0        0        0      575 2023-07-22 08:40:15.746000 finterstellar-0.2.20/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2021-03-08 19:32:22.000000 finterstellar-0.2.20/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 08:40:15.625000 finterstellar-0.2.20/finterstellar/
+-rw-rw-rw-   0        0        0      272 2023-07-22 08:39:38.000000 finterstellar-0.2.20/finterstellar/__init__.py
+-rw-rw-rw-   0        0        0     4793 2023-07-22 06:05:37.000000 finterstellar-0.2.20/finterstellar/data_prep.py
+-rw-rw-rw-   0        0        0    12206 2023-07-22 06:05:37.000000 finterstellar-0.2.20/finterstellar/financials.py
+-rw-rw-rw-   0        0        0     3966 2023-07-22 08:19:33.000000 finterstellar-0.2.20/finterstellar/krx.py
+-rw-rw-rw-   0        0        0     7919 2023-07-22 06:05:37.000000 finterstellar-0.2.20/finterstellar/trading.py
+-rw-rw-rw-   0        0        0     3800 2023-07-22 06:05:37.000000 finterstellar-0.2.20/finterstellar/trend.py
+-rw-rw-rw-   0        0        0     7332 2023-07-22 08:39:26.000000 finterstellar-0.2.20/finterstellar/visualization.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:40:15.674000 finterstellar-0.2.20/finterstellar.egg-info/
+-rw-rw-rw-   0        0        0      575 2023-07-22 08:40:15.000000 finterstellar-0.2.20/finterstellar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2023-07-22 08:40:15.000000 finterstellar-0.2.20/finterstellar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 08:40:15.000000 finterstellar-0.2.20/finterstellar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-22 08:40:15.000000 finterstellar-0.2.20/finterstellar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-07-22 08:40:15.000000 finterstellar-0.2.20/finterstellar.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 08:40:15.742000 finterstellar-0.2.20/finterstellar_/
+-rw-rw-rw-   0        0        0      214 2023-02-12 02:23:43.000000 finterstellar-0.2.20/finterstellar_/__init__.py
+-rw-rw-rw-   0        0        0     5336 2023-02-12 02:23:43.000000 finterstellar-0.2.20/finterstellar_/data_prep.py
+-rw-rw-rw-   0        0        0    12206 2023-02-12 02:23:43.000000 finterstellar-0.2.20/finterstellar_/financials.py
+-rw-rw-rw-   0        0        0     7722 2023-02-12 02:23:43.000000 finterstellar-0.2.20/finterstellar_/trading.py
+-rw-rw-rw-   0        0        0     3706 2023-02-12 02:23:43.000000 finterstellar-0.2.20/finterstellar_/trend.py
+-rw-rw-rw-   0        0        0     2374 2023-02-12 02:23:43.000000 finterstellar-0.2.20/finterstellar_/util.py
+-rw-rw-rw-   0        0        0     7137 2023-02-12 02:23:43.000000 finterstellar-0.2.20/finterstellar_/visualization.py
+-rw-rw-rw-   0        0        0       42 2023-07-22 08:40:15.749000 finterstellar-0.2.20/setup.cfg
+-rw-rw-rw-   0        0        0      827 2023-07-22 08:39:43.000000 finterstellar-0.2.20/setup.py
```

### Comparing `finterstellar-0.2.19/License` & `finterstellar-0.2.20/License`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.19/PKG-INFO` & `finterstellar-0.2.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finterstellar
-Version: 0.2.19
+Version: 0.2.20
 Summary: Quantitative analysis tools for investment
 Home-page: https://github.com/finterstellar/library
 Author: finterstellar
 Author-email: finterstellar@naver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `finterstellar-0.2.19/finterstellar/data_prep.py` & `finterstellar-0.2.20/finterstellar/data_prep.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.19/finterstellar/financials.py` & `finterstellar-0.2.20/finterstellar/financials.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.19/finterstellar/krx.py` & `finterstellar-0.2.20/finterstellar/krx.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.19/finterstellar/trading.py` & `finterstellar-0.2.20/finterstellar/trading.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.19/finterstellar/trend.py` & `finterstellar-0.2.20/finterstellar/trend.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.19/finterstellar/visualization.py` & `finterstellar-0.2.20/finterstellar/visualization.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.19/finterstellar.egg-info/PKG-INFO` & `finterstellar-0.2.20/finterstellar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finterstellar
-Version: 0.2.19
+Version: 0.2.20
 Summary: Quantitative analysis tools for investment
 Home-page: https://github.com/finterstellar/library
 Author: finterstellar
 Author-email: finterstellar@naver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `finterstellar-0.2.19/finterstellar.egg-info/SOURCES.txt` & `finterstellar-0.2.20/finterstellar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.19/finterstellar_/data_prep.py` & `finterstellar-0.2.20/finterstellar_/data_prep.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.19/finterstellar_/financials.py` & `finterstellar-0.2.20/finterstellar_/financials.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.19/finterstellar_/trading.py` & `finterstellar-0.2.20/finterstellar_/trading.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.19/finterstellar_/trend.py` & `finterstellar-0.2.20/finterstellar_/trend.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.19/finterstellar_/util.py` & `finterstellar-0.2.20/finterstellar_/util.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.19/finterstellar_/visualization.py` & `finterstellar-0.2.20/finterstellar_/visualization.py`

 * *Files identical despite different names*

