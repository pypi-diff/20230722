# Comparing `tmp/python-ria-0.0.3.tar.gz` & `tmp/python-ria-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-ria-0.0.3.tar", last modified: Sun Jun  5 12:38:16 2022, max compression
+gzip compressed data, was "python-ria-0.0.4.tar", last modified: Sat Jul 22 19:35:45 2023, max compression
```

## Comparing `python-ria-0.0.3.tar` & `python-ria-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-05 12:38:16.489088 python-ria-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-06-05 12:37:46.000000 python-ria-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3695 2022-06-05 12:38:16.489088 python-ria-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3131 2022-06-05 12:37:46.000000 python-ria-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-06-05 12:37:46.000000 python-ria-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-05 12:38:16.489088 python-ria-0.0.3/python_ria.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3695 2022-06-05 12:38:15.000000 python-ria-0.0.3/python_ria.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-06-05 12:38:16.000000 python-ria-0.0.3/python_ria.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-05 12:38:16.000000 python-ria-0.0.3/python_ria.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-05 12:38:16.000000 python-ria-0.0.3/python_ria.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-06-05 12:38:16.000000 python-ria-0.0.3/python_ria.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-05 12:38:16.489088 python-ria-0.0.3/ria/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-05 12:37:46.000000 python-ria-0.0.3/ria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-06-05 12:37:46.000000 python-ria-0.0.3/ria/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-05 12:38:16.489088 python-ria-0.0.3/ria/callback/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-05 12:37:46.000000 python-ria-0.0.3/ria/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-06-05 12:37:46.000000 python-ria-0.0.3/ria/callback/http_get_callback.py
--rw-r--r--   0 runner    (1001) docker     (121)     5506 2022-06-05 12:37:46.000000 python-ria-0.0.3/ria/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    13074 2022-06-05 12:37:46.000000 python-ria-0.0.3/ria/main.py
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-06-05 12:38:16.489088 python-ria-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-06-05 12:37:46.000000 python-ria-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:35:45.630142 python-ria-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 19:35:21.000000 python-ria-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-22 19:35:45.630142 python-ria-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-22 19:35:21.000000 python-ria-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-22 19:35:21.000000 python-ria-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:35:45.626142 python-ria-0.0.4/python_ria.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-22 19:35:45.000000 python-ria-0.0.4/python_ria.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-22 19:35:45.000000 python-ria-0.0.4/python_ria.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 19:35:45.000000 python-ria-0.0.4/python_ria.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-22 19:35:45.000000 python-ria-0.0.4/python_ria.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-22 19:35:45.000000 python-ria-0.0.4/python_ria.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:35:45.626142 python-ria-0.0.4/ria/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-22 19:35:21.000000 python-ria-0.0.4/ria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-22 19:35:21.000000 python-ria-0.0.4/ria/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:35:45.630142 python-ria-0.0.4/ria/callback/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:35:21.000000 python-ria-0.0.4/ria/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-22 19:35:21.000000 python-ria-0.0.4/ria/callback/http_get_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-22 19:35:21.000000 python-ria-0.0.4/ria/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-07-22 19:35:21.000000 python-ria-0.0.4/ria/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-22 19:35:45.630142 python-ria-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-22 19:35:21.000000 python-ria-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:35:45.630142 python-ria-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-22 19:35:21.000000 python-ria-0.0.4/tests/test_datos_diarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-22 19:35:21.000000 python-ria-0.0.4/tests/test_datos_mensuales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-22 19:35:21.000000 python-ria-0.0.4/tests/test_estaciones.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-22 19:35:21.000000 python-ria-0.0.4/tests/test_provincias.py
```

### Comparing `python-ria-0.0.3/LICENSE` & `python-ria-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-ria-0.0.3/PKG-INFO` & `python-ria-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ria
-Version: 0.0.3
+Version: 0.0.4
 Author: Francisco Puig
 Keywords: weather,RIA,Red de Información Agroclimática de Andalucía
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `python-ria-0.0.3/README.md` & `python-ria-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `python-ria-0.0.3/python_ria.egg-info/PKG-INFO` & `python-ria-0.0.4/python_ria.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ria
-Version: 0.0.3
+Version: 0.0.4
 Author: Francisco Puig
 Keywords: weather,RIA,Red de Información Agroclimática de Andalucía
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `python-ria-0.0.3/ria/_typing.py` & `python-ria-0.0.4/ria/_typing.py`

 * *Files identical despite different names*

### Comparing `python-ria-0.0.3/ria/constants.py` & `python-ria-0.0.4/ria/constants.py`

 * *Files identical despite different names*

### Comparing `python-ria-0.0.3/ria/main.py` & `python-ria-0.0.4/ria/main.py`

 * *Files identical despite different names*

### Comparing `python-ria-0.0.3/setup.cfg` & `python-ria-0.0.4/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-ria
-version = 0.0.3
+version = 0.0.4
 author = Francisco Puig
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = weather, RIA, Red de Información Agroclimática de Andalucía
 classifiers = 
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
```

