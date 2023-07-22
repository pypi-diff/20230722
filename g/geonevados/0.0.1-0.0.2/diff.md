# Comparing `tmp/geonevados-0.0.1.tar.gz` & `tmp/geonevados-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geonevados-0.0.1.tar", last modified: Tue Jul 18 22:34:06 2023, max compression
+gzip compressed data, was "geonevados-0.0.2.tar", last modified: Sat Jul 22 15:08:42 2023, max compression
```

## Comparing `geonevados-0.0.1.tar` & `geonevados-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 josedanielvelezcastano   (501) staff       (20)        0 2023-07-18 22:34:06.015836 geonevados-0.0.1/
--rw-r--r--   0 josedanielvelezcastano   (501) staff       (20)     1074 2023-07-18 22:21:47.000000 geonevados-0.0.1/LICENSE
--rw-r--r--   0 josedanielvelezcastano   (501) staff       (20)      122 2023-07-18 22:21:47.000000 geonevados-0.0.1/MANIFEST.in
--rw-r--r--   0 josedanielvelezcastano   (501) staff       (20)     1069 2023-07-18 22:34:06.015908 geonevados-0.0.1/PKG-INFO
--rw-r--r--   0 josedanielvelezcastano   (501) staff       (20)      371 2023-07-18 22:21:47.000000 geonevados-0.0.1/README.md
-drwxr-xr-x   0 josedanielvelezcastano   (501) staff       (20)        0 2023-07-18 22:34:06.015050 geonevados-0.0.1/geonevados/
--rw-r--r--   0 josedanielvelezcastano   (501) staff       (20)      128 2023-07-18 22:21:48.000000 geonevados-0.0.1/geonevados/__init__.py
--rw-r--r--   0 josedanielvelezcastano   (501) staff       (20)      188 2023-07-18 22:21:48.000000 geonevados-0.0.1/geonevados/common.py
--rw-r--r--   0 josedanielvelezcastano   (501) staff       (20)       19 2023-07-18 22:21:48.000000 geonevados-0.0.1/geonevados/geonevados.py
-drwxr-xr-x   0 josedanielvelezcastano   (501) staff       (20)        0 2023-07-18 22:34:06.015712 geonevados-0.0.1/geonevados.egg-info/
--rw-r--r--   0 josedanielvelezcastano   (501) staff       (20)     1069 2023-07-18 22:34:05.000000 geonevados-0.0.1/geonevados.egg-info/PKG-INFO
--rw-r--r--   0 josedanielvelezcastano   (501) staff       (20)      303 2023-07-18 22:34:05.000000 geonevados-0.0.1/geonevados.egg-info/SOURCES.txt
--rw-r--r--   0 josedanielvelezcastano   (501) staff       (20)        1 2023-07-18 22:34:05.000000 geonevados-0.0.1/geonevados.egg-info/dependency_links.txt
--rw-r--r--   0 josedanielvelezcastano   (501) staff       (20)        1 2023-07-18 22:34:05.000000 geonevados-0.0.1/geonevados.egg-info/not-zip-safe
--rw-r--r--   0 josedanielvelezcastano   (501) staff       (20)       11 2023-07-18 22:34:05.000000 geonevados-0.0.1/geonevados.egg-info/top_level.txt
--rw-r--r--   0 josedanielvelezcastano   (501) staff       (20)        0 2023-07-18 22:21:47.000000 geonevados-0.0.1/requirements.txt
--rw-r--r--   0 josedanielvelezcastano   (501) staff       (20)      393 2023-07-18 22:34:06.016231 geonevados-0.0.1/setup.cfg
--rw-r--r--   0 josedanielvelezcastano   (501) staff       (20)     1683 2023-07-18 22:21:47.000000 geonevados-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:08:42.240999 geonevados-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-22 15:08:27.000000 geonevados-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-22 15:08:27.000000 geonevados-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-22 15:08:42.240999 geonevados-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-22 15:08:27.000000 geonevados-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:08:42.236999 geonevados-0.0.2/geonevados/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-22 15:08:27.000000 geonevados-0.0.2/geonevados/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-22 15:08:27.000000 geonevados-0.0.2/geonevados/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-22 15:08:27.000000 geonevados-0.0.2/geonevados/geonevados.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:08:42.240999 geonevados-0.0.2/geonevados.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-22 15:08:42.000000 geonevados-0.0.2/geonevados.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-22 15:08:42.000000 geonevados-0.0.2/geonevados.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 15:08:42.000000 geonevados-0.0.2/geonevados.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 15:08:42.000000 geonevados-0.0.2/geonevados.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-22 15:08:42.000000 geonevados-0.0.2/geonevados.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:08:27.000000 geonevados-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-22 15:08:42.240999 geonevados-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-22 15:08:27.000000 geonevados-0.0.2/setup.py
```

### Comparing `geonevados-0.0.1/LICENSE` & `geonevados-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geonevados-0.0.1/PKG-INFO` & `geonevados-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geonevados
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tracking nevados.
 Home-page: https://github.com/jdavecas/geonevados
 Author: J. Daniel Velez
 Author-email: davelez@unc.edu
 License: MIT license
 Keywords: geonevados
 Classifier: Intended Audience :: Developers
```

### Comparing `geonevados-0.0.1/geonevados.egg-info/PKG-INFO` & `geonevados-0.0.2/geonevados.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geonevados
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tracking nevados.
 Home-page: https://github.com/jdavecas/geonevados
 Author: J. Daniel Velez
 Author-email: davelez@unc.edu
 License: MIT license
 Keywords: geonevados
 Classifier: Intended Audience :: Developers
```

### Comparing `geonevados-0.0.1/setup.py` & `geonevados-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='geonevados',
     name='geonevados',
     packages=find_packages(include=['geonevados', 'geonevados.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/jdavecas/geonevados',
-    version='0.0.1',
+    version='0.0.2',
     zip_safe=False,
 )
```

