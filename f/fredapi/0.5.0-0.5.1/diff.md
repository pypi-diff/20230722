# Comparing `tmp/fredapi-0.5.0.tar.gz` & `tmp/fredapi-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fredapi-0.5.0.tar", last modified: Tue Mar 15 14:12:33 2022, max compression
+gzip compressed data, was "fredapi-0.5.1.tar", last modified: Sat Jul 22 10:32:26 2023, max compression
```

## Comparing `fredapi-0.5.0.tar` & `fredapi-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mortadamehyar   (501) staff       (20)        0 2022-03-15 14:12:33.579931 fredapi-0.5.0/
--rw-r--r--   0 mortadamehyar   (501) staff       (20)     4088 2015-03-02 17:50:16.000000 fredapi-0.5.0/DESCRIPTION.rst
--rw-r--r--   0 mortadamehyar   (501) staff       (20)    11324 2014-09-14 21:07:19.000000 fredapi-0.5.0/LICENSE
--rw-r--r--   0 mortadamehyar   (501) staff       (20)       43 2019-01-19 06:53:28.000000 fredapi-0.5.0/MANIFEST.in
--rw-r--r--   0 mortadamehyar   (501) staff       (20)     6138 2022-03-15 14:12:33.579559 fredapi-0.5.0/PKG-INFO
--rw-r--r--   0 mortadamehyar   (501) staff       (20)     8508 2019-01-19 06:53:28.000000 fredapi-0.5.0/README.md
-drwxr-xr-x   0 mortadamehyar   (501) staff       (20)        0 2022-03-15 14:12:33.576717 fredapi-0.5.0/fredapi/
--rw-r--r--   0 mortadamehyar   (501) staff       (20)       82 2015-05-20 16:41:21.000000 fredapi-0.5.0/fredapi/__init__.py
--rw-r--r--   0 mortadamehyar   (501) staff       (20)    19652 2022-03-15 13:57:52.000000 fredapi-0.5.0/fredapi/fred.py
--rw-r--r--   0 mortadamehyar   (501) staff       (20)       19 2022-03-15 14:07:08.000000 fredapi-0.5.0/fredapi/version.py
-drwxr-xr-x   0 mortadamehyar   (501) staff       (20)        0 2022-03-15 14:12:33.578947 fredapi-0.5.0/fredapi.egg-info/
--rw-r--r--   0 mortadamehyar   (501) staff       (20)     6138 2022-03-15 14:12:33.000000 fredapi-0.5.0/fredapi.egg-info/PKG-INFO
--rw-r--r--   0 mortadamehyar   (501) staff       (20)      263 2022-03-15 14:12:33.000000 fredapi-0.5.0/fredapi.egg-info/SOURCES.txt
--rw-r--r--   0 mortadamehyar   (501) staff       (20)        1 2022-03-15 14:12:33.000000 fredapi-0.5.0/fredapi.egg-info/dependency_links.txt
--rw-r--r--   0 mortadamehyar   (501) staff       (20)        7 2022-03-15 14:12:33.000000 fredapi-0.5.0/fredapi.egg-info/requires.txt
--rw-r--r--   0 mortadamehyar   (501) staff       (20)        8 2022-03-15 14:12:33.000000 fredapi-0.5.0/fredapi.egg-info/top_level.txt
--rw-r--r--   0 mortadamehyar   (501) staff       (20)       38 2022-03-15 14:12:33.580042 fredapi-0.5.0/setup.cfg
--rw-r--r--   0 mortadamehyar   (501) staff       (20)     1387 2017-09-03 02:31:48.000000 fredapi-0.5.0/setup.py
+drwxr-xr-x   0 mortadamehyar   (501) staff       (20)        0 2023-07-22 10:32:26.211425 fredapi-0.5.1/
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)     4088 2015-03-02 17:50:16.000000 fredapi-0.5.1/DESCRIPTION.rst
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)    11324 2014-09-14 21:07:19.000000 fredapi-0.5.1/LICENSE
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)       43 2019-01-19 06:53:28.000000 fredapi-0.5.1/MANIFEST.in
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)     5004 2023-07-22 10:32:26.211296 fredapi-0.5.1/PKG-INFO
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)     8508 2019-01-19 06:53:28.000000 fredapi-0.5.1/README.md
+drwxr-xr-x   0 mortadamehyar   (501) staff       (20)        0 2023-07-22 10:32:26.210383 fredapi-0.5.1/fredapi/
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)       82 2015-05-20 16:41:21.000000 fredapi-0.5.1/fredapi/__init__.py
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)    19658 2023-07-22 09:55:59.000000 fredapi-0.5.1/fredapi/fred.py
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)       19 2023-07-22 09:55:59.000000 fredapi-0.5.1/fredapi/version.py
+drwxr-xr-x   0 mortadamehyar   (501) staff       (20)        0 2023-07-22 10:32:26.211104 fredapi-0.5.1/fredapi.egg-info/
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)     5004 2023-07-22 10:32:26.000000 fredapi-0.5.1/fredapi.egg-info/PKG-INFO
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)      263 2023-07-22 10:32:26.000000 fredapi-0.5.1/fredapi.egg-info/SOURCES.txt
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)        1 2023-07-22 10:32:26.000000 fredapi-0.5.1/fredapi.egg-info/dependency_links.txt
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)        7 2023-07-22 10:32:26.000000 fredapi-0.5.1/fredapi.egg-info/requires.txt
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)        8 2023-07-22 10:32:26.000000 fredapi-0.5.1/fredapi.egg-info/top_level.txt
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)       38 2023-07-22 10:32:26.211458 fredapi-0.5.1/setup.cfg
+-rw-r--r--   0 mortadamehyar   (501) staff       (20)     1387 2017-09-03 02:31:48.000000 fredapi-0.5.1/setup.py
```

### Comparing `fredapi-0.5.0/DESCRIPTION.rst` & `fredapi-0.5.1/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `fredapi-0.5.0/LICENSE` & `fredapi-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fredapi-0.5.0/README.md` & `fredapi-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fredapi-0.5.0/fredapi/fred.py` & `fredapi-0.5.1/fredapi/fred.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,15 +349,15 @@
         else:
             max_results_needed = limit
 
         if max_results_needed > self.max_results_per_request:
             for i in range(1, max_results_needed // self.max_results_per_request + 1):
                 offset = i * self.max_results_per_request
                 next_data, _ = self.__do_series_search(url + '&offset=' + str(offset))
-                data = data.append(next_data)
+                data = pd.concat([data, next_data])
         return data.head(max_results_needed)
 
     def search(self, text, limit=1000, order_by=None, sort_order=None, filter=None):
         """
         Do a fulltext search for series in the Fred dataset. Returns information about matching series in a DataFrame.
 
         Parameters
```

### Comparing `fredapi-0.5.0/setup.py` & `fredapi-0.5.1/setup.py`

 * *Files identical despite different names*

