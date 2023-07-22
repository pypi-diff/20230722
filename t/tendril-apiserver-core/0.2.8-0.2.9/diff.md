# Comparing `tmp/tendril-apiserver-core-0.2.8.tar.gz` & `tmp/tendril-apiserver-core-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-apiserver-core-0.2.8.tar", last modified: Wed Dec 14 20:03:00 2022, max compression
+gzip compressed data, was "dist/tendril-apiserver-core-0.2.9.tar", last modified: Mon Feb 27 21:09:45 2023, max compression
```

## Comparing `tendril-apiserver-core-0.2.8.tar` & `tendril-apiserver-core-0.2.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:03:00.443401 tendril-apiserver-core-0.2.8/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2020-03-20 07:52:32.000000 tendril-apiserver-core-0.2.8/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2020-03-20 07:52:33.000000 tendril-apiserver-core-0.2.8/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2020-03-20 07:52:32.000000 tendril-apiserver-core-0.2.8/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-03-20 07:52:32.000000 tendril-apiserver-core-0.2.8/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2020-03-20 07:52:33.000000 tendril-apiserver-core-0.2.8/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2020-03-20 07:52:31.000000 tendril-apiserver-core-0.2.8/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4070 2022-12-14 20:03:00.443401 tendril-apiserver-core-0.2.8/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2302 2022-11-25 03:24:33.000000 tendril-apiserver-core-0.2.8/README.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2022-12-14 20:03:00.443401 tendril-apiserver-core-0.2.8/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3431 2022-12-14 16:38:03.000000 tendril-apiserver-core-0.2.8/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:03:00.439401 tendril-apiserver-core-0.2.8/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:03:00.439401 tendril-apiserver-core-0.2.8/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-08-23 15:59:56.000000 tendril-apiserver-core-0.2.8/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:03:00.439401 tendril-apiserver-core-0.2.8/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-25 03:24:33.000000 tendril-apiserver-core-0.2.8/src/tendril/apiserver/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       52 2022-12-13 06:20:04.000000 tendril-apiserver-core-0.2.8/src/tendril/apiserver/core.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:03:00.439401 tendril-apiserver-core-0.2.8/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-07 14:54:45.000000 tendril-apiserver-core-0.2.8/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2051 2022-12-07 13:19:39.000000 tendril-apiserver-core-0.2.8/src/tendril/apiserver/routers/diagnostics.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1043 2022-12-07 13:19:39.000000 tendril-apiserver-core-0.2.8/src/tendril/apiserver/routers/system.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3600 2022-12-14 17:32:58.000000 tendril-apiserver-core-0.2.8/src/tendril/apiserver/server.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:03:00.439401 tendril-apiserver-core-0.2.8/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-27 05:30:09.000000 tendril-apiserver-core-0.2.8/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:03:00.439401 tendril-apiserver-core-0.2.8/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      212 2022-11-27 05:30:09.000000 tendril-apiserver-core-0.2.8/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      153 2022-11-27 05:33:56.000000 tendril-apiserver-core-0.2.8/src/tendril/authz/scopes/system.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:03:00.439401 tendril-apiserver-core-0.2.8/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-03-20 07:52:30.000000 tendril-apiserver-core-0.2.8/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2745 2022-11-27 08:00:04.000000 tendril-apiserver-core-0.2.8/src/tendril/config/server.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:03:00.439401 tendril-apiserver-core-0.2.8/src/tendril/resources/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1302 2022-08-08 11:28:48.000000 tendril-apiserver-core-0.2.8/src/tendril/resources/test_certificate.pem
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1704 2022-08-08 11:28:48.000000 tendril-apiserver-core-0.2.8/src/tendril/resources/test_key.pem
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-12-14 20:03:00.443401 tendril-apiserver-core-0.2.8/src/tendril_apiserver_core.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4070 2022-12-14 20:03:00.000000 tendril-apiserver-core-0.2.8/src/tendril_apiserver_core.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      900 2022-12-14 20:03:00.000000 tendril-apiserver-core-0.2.8/src/tendril_apiserver_core.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2022-12-14 20:03:00.000000 tendril-apiserver-core-0.2.8/src/tendril_apiserver_core.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       67 2022-12-14 20:03:00.000000 tendril-apiserver-core-0.2.8/src/tendril_apiserver_core.egg-info/entry_points.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      731 2022-12-14 20:03:00.000000 tendril-apiserver-core-0.2.8/src/tendril_apiserver_core.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2022-12-14 20:03:00.000000 tendril-apiserver-core-0.2.8/src/tendril_apiserver_core.egg-info/top_level.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      829 2022-11-25 03:24:49.000000 tendril-apiserver-core-0.2.8/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-02-27 21:09:45.940628 tendril-apiserver-core-0.2.9/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.2.9/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.2.9/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.2.9/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.2.9/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.2.9/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.2.9/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4070 2023-02-27 21:09:45.940628 tendril-apiserver-core-0.2.9/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2302 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.2.9/README.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-02-27 21:09:45.944629 tendril-apiserver-core-0.2.9/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3431 2023-02-24 08:35:00.000000 tendril-apiserver-core-0.2.9/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-02-27 21:09:45.916628 tendril-apiserver-core-0.2.9/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-02-27 21:09:45.924629 tendril-apiserver-core-0.2.9/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.2.9/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-02-27 21:09:45.924629 tendril-apiserver-core-0.2.9/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.2.9/src/tendril/apiserver/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       52 2023-02-18 23:08:41.000000 tendril-apiserver-core-0.2.9/src/tendril/apiserver/core.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-02-27 21:09:45.928629 tendril-apiserver-core-0.2.9/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 20:27:06.000000 tendril-apiserver-core-0.2.9/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2051 2022-12-09 20:27:06.000000 tendril-apiserver-core-0.2.9/src/tendril/apiserver/routers/diagnostics.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1043 2022-12-09 20:27:06.000000 tendril-apiserver-core-0.2.9/src/tendril/apiserver/routers/system.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3600 2023-02-24 08:35:00.000000 tendril-apiserver-core-0.2.9/src/tendril/apiserver/server.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-02-27 21:09:45.928629 tendril-apiserver-core-0.2.9/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:36:13.000000 tendril-apiserver-core-0.2.9/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-02-27 21:09:45.932628 tendril-apiserver-core-0.2.9/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 21:00:43.000000 tendril-apiserver-core-0.2.9/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      153 2022-11-28 19:36:13.000000 tendril-apiserver-core-0.2.9/src/tendril/authz/scopes/system.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-02-27 21:09:45.932628 tendril-apiserver-core-0.2.9/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.2.9/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2745 2022-11-28 19:36:13.000000 tendril-apiserver-core-0.2.9/src/tendril/config/server.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-02-27 21:09:45.936628 tendril-apiserver-core-0.2.9/src/tendril/resources/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1302 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.2.9/src/tendril/resources/test_certificate.pem
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1704 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.2.9/src/tendril/resources/test_key.pem
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-02-27 21:09:45.940628 tendril-apiserver-core-0.2.9/src/tendril_apiserver_core.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4070 2023-02-27 21:09:45.000000 tendril-apiserver-core-0.2.9/src/tendril_apiserver_core.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      900 2023-02-27 21:09:45.000000 tendril-apiserver-core-0.2.9/src/tendril_apiserver_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-02-27 21:09:45.000000 tendril-apiserver-core-0.2.9/src/tendril_apiserver_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       67 2023-02-27 21:09:45.000000 tendril-apiserver-core-0.2.9/src/tendril_apiserver_core.egg-info/entry_points.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      731 2023-02-27 21:09:45.000000 tendril-apiserver-core-0.2.9/src/tendril_apiserver_core.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-02-27 21:09:45.000000 tendril-apiserver-core-0.2.9/src/tendril_apiserver_core.egg-info/top_level.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      829 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.2.9/tox.ini
```

### Comparing `tendril-apiserver-core-0.2.8/.gitignore` & `tendril-apiserver-core-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.2.8/.readthedocs.yml` & `tendril-apiserver-core-0.2.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.2.8/.travis.yml` & `tendril-apiserver-core-0.2.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.2.8/LICENSE` & `tendril-apiserver-core-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.2.8/PKG-INFO` & `tendril-apiserver-core-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-apiserver-core
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tendril API Server Core Infrastructure
 Home-page: https://github.com/tendril-framework/tendril-apiserver-core
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 License: UNKNOWN
 Project-URL: Documentation, https://tendril-apiserver-core.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-apiserver-core/issues
```

### Comparing `tendril-apiserver-core-0.2.8/README.rst` & `tendril-apiserver-core-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.2.8/setup.py` & `tendril-apiserver-core-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.2.8/src/tendril/apiserver/routers/diagnostics.py` & `tendril-apiserver-core-0.2.9/src/tendril/apiserver/routers/diagnostics.py`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.2.8/src/tendril/apiserver/routers/system.py` & `tendril-apiserver-core-0.2.9/src/tendril/apiserver/routers/system.py`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.2.8/src/tendril/apiserver/server.py` & `tendril-apiserver-core-0.2.9/src/tendril/apiserver/server.py`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.2.8/src/tendril/config/__init__.py` & `tendril-apiserver-core-0.2.9/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.2.8/src/tendril/config/server.py` & `tendril-apiserver-core-0.2.9/src/tendril/config/server.py`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.2.8/src/tendril/resources/test_certificate.pem` & `tendril-apiserver-core-0.2.9/src/tendril/resources/test_certificate.pem`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.2.8/src/tendril/resources/test_key.pem` & `tendril-apiserver-core-0.2.9/src/tendril/resources/test_key.pem`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.2.8/src/tendril_apiserver_core.egg-info/PKG-INFO` & `tendril-apiserver-core-0.2.9/src/tendril_apiserver_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-apiserver-core
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tendril API Server Core Infrastructure
 Home-page: https://github.com/tendril-framework/tendril-apiserver-core
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 License: UNKNOWN
 Project-URL: Documentation, https://tendril-apiserver-core.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-apiserver-core/issues
```

### Comparing `tendril-apiserver-core-0.2.8/src/tendril_apiserver_core.egg-info/SOURCES.txt` & `tendril-apiserver-core-0.2.9/src/tendril_apiserver_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.2.8/src/tendril_apiserver_core.egg-info/requires.txt` & `tendril-apiserver-core-0.2.9/src/tendril_apiserver_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.2.8/tox.ini` & `tendril-apiserver-core-0.2.9/tox.ini`

 * *Files identical despite different names*

