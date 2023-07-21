# Comparing `tmp/dagster-mysql-0.20.1.tar.gz` & `tmp/dagster-mysql-0.20.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-mysql-0.20.1.tar", last modified: Fri Jul 21 15:38:28 2023, max compression
+gzip compressed data, was "dagster-mysql-0.20.2.tar", last modified: Fri Jul 21 22:39:01 2023, max compression
```

## Comparing `dagster-mysql-0.20.1.tar` & `dagster-mysql-0.20.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:28.455168 dagster-mysql-0.20.1/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-21 15:29:00.000000 dagster-mysql-0.20.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      126 2023-07-21 15:29:00.000000 dagster-mysql-0.20.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      552 2023-07-21 15:38:28.455168 dagster-mysql-0.20.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      125 2023-07-21 15:29:00.000000 dagster-mysql-0.20.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:28.447168 dagster-mysql-0.20.1/dagster_mysql/
--rw-r--r--   0 root         (0) root         (0)      434 2023-07-21 15:29:00.000000 dagster-mysql-0.20.1/dagster_mysql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:28.447168 dagster-mysql-0.20.1/dagster_mysql/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 15:29:00.000000 dagster-mysql-0.20.1/dagster_mysql/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1064 2023-07-21 15:29:00.000000 dagster-mysql-0.20.1/dagster_mysql/alembic/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:28.451168 dagster-mysql-0.20.1/dagster_mysql/event_log/
--rw-r--r--   0 root         (0) root         (0)       68 2023-07-21 15:29:00.000000 dagster-mysql-0.20.1/dagster_mysql/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8796 2023-07-21 15:29:00.000000 dagster-mysql-0.20.1/dagster_mysql/event_log/event_log.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-21 15:29:00.000000 dagster-mysql-0.20.1/dagster_mysql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:28.451168 dagster-mysql-0.20.1/dagster_mysql/run_storage/
--rw-r--r--   0 root         (0) root         (0)       60 2023-07-21 15:29:00.000000 dagster-mysql-0.20.1/dagster_mysql/run_storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7887 2023-07-21 15:29:00.000000 dagster-mysql-0.20.1/dagster_mysql/run_storage/run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:28.451168 dagster-mysql-0.20.1/dagster_mysql/schedule_storage/
--rw-r--r--   0 root         (0) root         (0)       75 2023-07-21 15:29:00.000000 dagster-mysql-0.20.1/dagster_mysql/schedule_storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6281 2023-07-21 15:29:00.000000 dagster-mysql-0.20.1/dagster_mysql/schedule_storage/schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     3730 2023-07-21 15:29:00.000000 dagster-mysql-0.20.1/dagster_mysql/storage.py
--rw-r--r--   0 root         (0) root         (0)     6435 2023-07-21 15:29:00.000000 dagster-mysql-0.20.1/dagster_mysql/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 15:29:00.000000 dagster-mysql-0.20.1/dagster_mysql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:38:28.447168 dagster-mysql-0.20.1/dagster_mysql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      552 2023-07-21 15:38:28.000000 dagster-mysql-0.20.1/dagster_mysql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      704 2023-07-21 15:38:28.000000 dagster-mysql-0.20.1/dagster_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:38:28.000000 dagster-mysql-0.20.1/dagster_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:38:28.000000 dagster-mysql-0.20.1/dagster_mysql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 15:38:28.000000 dagster-mysql-0.20.1/dagster_mysql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-21 15:38:28.000000 dagster-mysql-0.20.1/dagster_mysql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      148 2023-07-21 15:38:28.455168 dagster-mysql-0.20.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1244 2023-07-21 15:29:00.000000 dagster-mysql-0.20.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:01.624656 dagster-mysql-0.20.2/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-21 22:28:10.000000 dagster-mysql-0.20.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      126 2023-07-21 22:28:10.000000 dagster-mysql-0.20.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      552 2023-07-21 22:39:01.624656 dagster-mysql-0.20.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      125 2023-07-21 22:28:10.000000 dagster-mysql-0.20.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:01.616655 dagster-mysql-0.20.2/dagster_mysql/
+-rw-r--r--   0 root         (0) root         (0)      434 2023-07-21 22:28:10.000000 dagster-mysql-0.20.2/dagster_mysql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:01.616655 dagster-mysql-0.20.2/dagster_mysql/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:10.000000 dagster-mysql-0.20.2/dagster_mysql/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-07-21 22:28:10.000000 dagster-mysql-0.20.2/dagster_mysql/alembic/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:01.620655 dagster-mysql-0.20.2/dagster_mysql/event_log/
+-rw-r--r--   0 root         (0) root         (0)       68 2023-07-21 22:28:10.000000 dagster-mysql-0.20.2/dagster_mysql/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8796 2023-07-21 22:28:10.000000 dagster-mysql-0.20.2/dagster_mysql/event_log/event_log.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-21 22:28:10.000000 dagster-mysql-0.20.2/dagster_mysql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:01.620655 dagster-mysql-0.20.2/dagster_mysql/run_storage/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-21 22:28:10.000000 dagster-mysql-0.20.2/dagster_mysql/run_storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7887 2023-07-21 22:28:10.000000 dagster-mysql-0.20.2/dagster_mysql/run_storage/run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:01.620655 dagster-mysql-0.20.2/dagster_mysql/schedule_storage/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-07-21 22:28:10.000000 dagster-mysql-0.20.2/dagster_mysql/schedule_storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6281 2023-07-21 22:28:10.000000 dagster-mysql-0.20.2/dagster_mysql/schedule_storage/schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3730 2023-07-21 22:28:10.000000 dagster-mysql-0.20.2/dagster_mysql/storage.py
+-rw-r--r--   0 root         (0) root         (0)     6435 2023-07-21 22:28:10.000000 dagster-mysql-0.20.2/dagster_mysql/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 22:28:10.000000 dagster-mysql-0.20.2/dagster_mysql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:39:01.616655 dagster-mysql-0.20.2/dagster_mysql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-07-21 22:39:01.000000 dagster-mysql-0.20.2/dagster_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      704 2023-07-21 22:39:01.000000 dagster-mysql-0.20.2/dagster_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 22:39:01.000000 dagster-mysql-0.20.2/dagster_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 22:39:01.000000 dagster-mysql-0.20.2/dagster_mysql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 22:39:01.000000 dagster-mysql-0.20.2/dagster_mysql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-21 22:39:01.000000 dagster-mysql-0.20.2/dagster_mysql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-21 22:39:01.624656 dagster-mysql-0.20.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1244 2023-07-21 22:28:10.000000 dagster-mysql-0.20.2/setup.py
```

### Comparing `dagster-mysql-0.20.1/LICENSE` & `dagster-mysql-0.20.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.20.1/PKG-INFO` & `dagster-mysql-0.20.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mysql
-Version: 0.20.1
+Version: 0.20.2
 Summary: A Dagster integration for MySQL
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mysql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-mysql-0.20.1/dagster_mysql/alembic/alembic.ini` & `dagster-mysql-0.20.2/dagster_mysql/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.20.1/dagster_mysql/event_log/event_log.py` & `dagster-mysql-0.20.2/dagster_mysql/event_log/event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.20.1/dagster_mysql/run_storage/run_storage.py` & `dagster-mysql-0.20.2/dagster_mysql/run_storage/run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.20.1/dagster_mysql/schedule_storage/schedule_storage.py` & `dagster-mysql-0.20.2/dagster_mysql/schedule_storage/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.20.1/dagster_mysql/storage.py` & `dagster-mysql-0.20.2/dagster_mysql/storage.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.20.1/dagster_mysql/utils.py` & `dagster-mysql-0.20.2/dagster_mysql/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.20.1/dagster_mysql.egg-info/PKG-INFO` & `dagster-mysql-0.20.2/dagster_mysql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mysql
-Version: 0.20.1
+Version: 0.20.2
 Summary: A Dagster integration for MySQL
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mysql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-mysql-0.20.1/dagster_mysql.egg-info/SOURCES.txt` & `dagster-mysql-0.20.2/dagster_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.20.1/setup.py` & `dagster-mysql-0.20.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,10 +32,10 @@
     packages=find_packages(exclude=["dagster_mysql_tests*"]),
     package_data={
         "dagster-mysql": [
             "dagster_mysql/alembic/*",
         ]
     },
     include_package_data=True,
-    install_requires=["dagster==1.4.1", "mysql-connector-python"],
+    install_requires=["dagster==1.4.2", "mysql-connector-python"],
     zip_safe=False,
 )
```

