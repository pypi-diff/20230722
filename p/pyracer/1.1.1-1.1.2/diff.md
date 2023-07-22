# Comparing `tmp/pyracer-1.1.1.tar.gz` & `tmp/pyracer-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracer-1.1.1.tar", last modified: Fri Jul 21 07:59:28 2023, max compression
+gzip compressed data, was "pyracer-1.1.2.tar", last modified: Sat Jul 22 08:57:20 2023, max compression
```

## Comparing `pyracer-1.1.1.tar` & `pyracer-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:59:28.475448 pyracer-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-21 07:59:13.000000 pyracer-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-21 07:59:28.475448 pyracer-1.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:59:28.471449 pyracer-1.1.1/RACER/
--rw-r--r--   0 runner    (1001) docker     (123)    14422 2023-07-21 07:59:13.000000 pyracer-1.1.1/RACER/RACER.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-21 07:59:13.000000 pyracer-1.1.1/RACER/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-21 07:59:13.000000 pyracer-1.1.1/RACER/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 07:59:13.000000 pyracer-1.1.1/RACER/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-21 07:59:13.000000 pyracer-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:59:28.475448 pyracer-1.1.1/pyracer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-21 07:59:28.000000 pyracer-1.1.1/pyracer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-21 07:59:28.000000 pyracer-1.1.1/pyracer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:59:28.000000 pyracer-1.1.1/pyracer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 07:59:28.000000 pyracer-1.1.1/pyracer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 07:59:28.000000 pyracer-1.1.1/pyracer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 07:59:28.475448 pyracer-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-21 07:59:13.000000 pyracer-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:20.837439 pyracer-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-22 08:57:12.000000 pyracer-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-22 08:57:20.837439 pyracer-1.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:20.837439 pyracer-1.1.2/RACER/
+-rw-r--r--   0 runner    (1001) docker     (123)    14422 2023-07-22 08:57:12.000000 pyracer-1.1.2/RACER/RACER.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-22 08:57:12.000000 pyracer-1.1.2/RACER/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-22 08:57:12.000000 pyracer-1.1.2/RACER/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 08:57:12.000000 pyracer-1.1.2/RACER/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-22 08:57:12.000000 pyracer-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:20.837439 pyracer-1.1.2/pyracer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-22 08:57:20.000000 pyracer-1.1.2/pyracer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-22 08:57:20.000000 pyracer-1.1.2/pyracer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 08:57:20.000000 pyracer-1.1.2/pyracer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-22 08:57:20.000000 pyracer-1.1.2/pyracer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 08:57:20.000000 pyracer-1.1.2/pyracer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 08:57:20.837439 pyracer-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-22 08:57:12.000000 pyracer-1.1.2/setup.py
```

### Comparing `pyracer-1.1.1/LICENSE` & `pyracer-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyracer-1.1.1/PKG-INFO` & `pyracer-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracer
-Version: 1.1.1
+Version: 1.1.2
 Summary: Unofficial Python implementation of the RACER classification algorithm.
 Home-page: https://github.com/Adversarian/RACER
 Author: Arian Tashakkor, Mohammad Safaiyan
 Author-email: a77physics@gmail.com
 License: MIT
 Keywords: machine learning,classification,RACER
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyracer-1.1.1/RACER/RACER.py` & `pyracer-1.1.2/RACER/RACER.py`

 * *Files identical despite different names*

### Comparing `pyracer-1.1.1/RACER/preprocessing.py` & `pyracer-1.1.2/RACER/preprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             y (Union[pd.DataFrame, np.ndarray]): Targets vector
 
         Returns:
             Tuple[Union[pd.DataFrame, np.ndarray], Union[pd.DataFrame, np.ndarray]]: Transformed features and targets vectors.
         """
         X, y = pd.DataFrame(X), pd.DataFrame(y)
         if self._quantizer == "infer":
-            uniques = y.nunique()
+            uniques = y.nunique().values
             if uniques > 2:
                 self._quantizer = MOB(max_candidates=self._max_num_splits)
             else:
                 self._quantizer = MDLP(max_n_bins=self._max_n_bins)
         numerics_X = X.select_dtypes(include=[np.number]).columns.tolist()
         if numerics_X:
             for col in numerics_X:
```

### Comparing `pyracer-1.1.1/README.md` & `pyracer-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyracer-1.1.1/pyracer.egg-info/PKG-INFO` & `pyracer-1.1.2/pyracer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracer
-Version: 1.1.1
+Version: 1.1.2
 Summary: Unofficial Python implementation of the RACER classification algorithm.
 Home-page: https://github.com/Adversarian/RACER
 Author: Arian Tashakkor, Mohammad Safaiyan
 Author-email: a77physics@gmail.com
 License: MIT
 Keywords: machine learning,classification,RACER
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyracer-1.1.1/setup.py` & `pyracer-1.1.2/setup.py`

 * *Files identical despite different names*

