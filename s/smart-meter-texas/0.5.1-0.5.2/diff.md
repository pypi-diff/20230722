# Comparing `tmp/smart_meter_texas-0.5.1.tar.gz` & `tmp/smart_meter_texas-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_meter_texas-0.5.1.tar", last modified: Sun May 29 00:38:18 2022, max compression
+gzip compressed data, was "smart_meter_texas-0.5.2.tar", last modified: Sat Jul 22 12:38:05 2023, max compression
```

## Comparing `smart_meter_texas-0.5.1.tar` & `smart_meter_texas-0.5.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 00:38:18.907906 smart_meter_texas-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3638 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1863 2022-05-29 00:38:18.907906 smart_meter_texas-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 00:38:18.903906 smart_meter_texas-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     4974 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      779 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/docs/smart_meter_texas.rst
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-05-29 00:38:18.907906 smart_meter_texas-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1436 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 00:38:18.903906 smart_meter_texas-0.5.1/smart_meter_texas/
--rw-r--r--   0 runner    (1001) docker     (121)    16500 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/smart_meter_texas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/smart_meter_texas/const.py
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-05-29 00:38:00.000000 smart_meter_texas-0.5.1/smart_meter_texas/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 00:38:18.907906 smart_meter_texas-0.5.1/smart_meter_texas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1863 2022-05-29 00:38:18.000000 smart_meter_texas-0.5.1/smart_meter_texas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-05-29 00:38:18.000000 smart_meter_texas-0.5.1/smart_meter_texas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-29 00:38:18.000000 smart_meter_texas-0.5.1/smart_meter_texas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-29 00:38:18.000000 smart_meter_texas-0.5.1/smart_meter_texas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-05-29 00:38:18.000000 smart_meter_texas-0.5.1/smart_meter_texas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-05-29 00:38:18.000000 smart_meter_texas-0.5.1/smart_meter_texas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:38:05.848132 smart_meter_texas-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-22 12:38:05.848132 smart_meter_texas-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:38:05.848132 smart_meter_texas-0.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4974 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/docs/smart_meter_texas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-22 12:38:05.848132 smart_meter_texas-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:38:05.848132 smart_meter_texas-0.5.2/smart_meter_texas/
+-rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/smart_meter_texas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/smart_meter_texas/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-22 12:37:53.000000 smart_meter_texas-0.5.2/smart_meter_texas/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:38:05.848132 smart_meter_texas-0.5.2/smart_meter_texas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-22 12:38:05.000000 smart_meter_texas-0.5.2/smart_meter_texas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-22 12:38:05.000000 smart_meter_texas-0.5.2/smart_meter_texas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 12:38:05.000000 smart_meter_texas-0.5.2/smart_meter_texas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 12:38:05.000000 smart_meter_texas-0.5.2/smart_meter_texas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-22 12:38:05.000000 smart_meter_texas-0.5.2/smart_meter_texas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-22 12:38:05.000000 smart_meter_texas-0.5.2/smart_meter_texas.egg-info/top_level.txt
```

### Comparing `smart_meter_texas-0.5.1/CONTRIBUTING.rst` & `smart_meter_texas-0.5.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `smart_meter_texas-0.5.1/LICENSE` & `smart_meter_texas-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_meter_texas-0.5.1/PKG-INFO` & `smart_meter_texas-0.5.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart_meter_texas
-Version: 0.5.1
+Version: 0.5.2
 Summary: Package to connect to and retrieve data from the unofficial Smart Meter Texas API
 Home-page: https://github.com/grahamwetzler/smart-meter-texas
 Author: Graham Wetzler
 Author-email: graham@wetzler.dev
 License: MIT license
 Keywords: smart_meter_texas
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `smart_meter_texas-0.5.1/README.rst` & `smart_meter_texas-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `smart_meter_texas-0.5.1/docs/Makefile` & `smart_meter_texas-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `smart_meter_texas-0.5.1/docs/conf.py` & `smart_meter_texas-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `smart_meter_texas-0.5.1/docs/installation.rst` & `smart_meter_texas-0.5.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `smart_meter_texas-0.5.1/docs/make.bat` & `smart_meter_texas-0.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `smart_meter_texas-0.5.1/setup.py` & `smart_meter_texas-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     keywords="smart_meter_texas",
     name="smart_meter_texas",
     packages=find_packages(include=["smart_meter_texas", "smart_meter_texas.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/grahamwetzler/smart-meter-texas",
-    version="0.5.1",
+    version="0.5.2",
     zip_safe=False,
 )
```

### Comparing `smart_meter_texas-0.5.1/smart_meter_texas/__init__.py` & `smart_meter_texas-0.5.2/smart_meter_texas/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     SmartMeterTexasAuthError,
     SmartMeterTexasAuthExpired,
     SmartMeterTexasRateLimitError,
 )
 
 __author__ = "Graham Wetzler"
 __email__ = "graham@wetzler.dev"
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Meter:
     def __init__(self, meter: str, esiid: str, address: str):
         self.meter = meter
```

### Comparing `smart_meter_texas-0.5.1/smart_meter_texas/const.py` & `smart_meter_texas-0.5.2/smart_meter_texas/const.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 
-BASE_HOSTNAME = "www.smartmetertexas.com"
+BASE_HOSTNAME = "smartmetertexas.com"
 BASE_URL = "https://" + BASE_HOSTNAME + "/"
 BASE_ENDPOINT = BASE_URL + "api"
 AUTH_ENDPOINT = "/user/authenticate"
 DASHBOARD_ENDPOINT = "/dashboard"
 LATEST_OD_READ_ENDPOINT = "/usage/latestodrread"
 METER_ENDPOINT = "/meter"
 OD_READ_ENDPOINT = "/ondemandread"
```

### Comparing `smart_meter_texas-0.5.1/smart_meter_texas/exceptions.py` & `smart_meter_texas-0.5.2/smart_meter_texas/exceptions.py`

 * *Files identical despite different names*

### Comparing `smart_meter_texas-0.5.1/smart_meter_texas.egg-info/PKG-INFO` & `smart_meter_texas-0.5.2/smart_meter_texas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-meter-texas
-Version: 0.5.1
+Version: 0.5.2
 Summary: Package to connect to and retrieve data from the unofficial Smart Meter Texas API
 Home-page: https://github.com/grahamwetzler/smart-meter-texas
 Author: Graham Wetzler
 Author-email: graham@wetzler.dev
 License: MIT license
 Keywords: smart_meter_texas
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `smart_meter_texas-0.5.1/smart_meter_texas.egg-info/SOURCES.txt` & `smart_meter_texas-0.5.2/smart_meter_texas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

