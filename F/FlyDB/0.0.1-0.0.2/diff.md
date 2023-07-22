# Comparing `tmp/FlyDB-0.0.1.tar.gz` & `tmp/FlyDB-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlyDB-0.0.1.tar", last modified: Sat Jul 22 12:04:06 2023, max compression
+gzip compressed data, was "FlyDB-0.0.2.tar", last modified: Sat Jul 22 12:07:59 2023, max compression
```

## Comparing `FlyDB-0.0.1.tar` & `FlyDB-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 adminonly  (1000) adminonly  (1000)        0 2023-07-22 12:04:06.100820 FlyDB-0.0.1/
-drwxrwxr-x   0 adminonly  (1000) adminonly  (1000)        0 2023-07-22 12:04:06.100820 FlyDB-0.0.1/FlyDB/
--rw-rw-r--   0 adminonly  (1000) adminonly  (1000)        0 2023-07-22 11:55:43.000000 FlyDB-0.0.1/FlyDB/__init__.py
-drwxrwxr-x   0 adminonly  (1000) adminonly  (1000)        0 2023-07-22 12:04:06.100820 FlyDB-0.0.1/FlyDB/client_grpc/
--rw-rw-r--   0 adminonly  (1000) adminonly  (1000)        0 2023-07-22 11:55:51.000000 FlyDB-0.0.1/FlyDB/client_grpc/__init__.py
--rw-rw-r--   0 adminonly  (1000) adminonly  (1000)    10426 2023-07-22 09:17:10.000000 FlyDB-0.0.1/FlyDB/client_grpc/db_pb2.py
--rw-rw-r--   0 adminonly  (1000) adminonly  (1000)    28497 2023-07-22 11:55:57.000000 FlyDB-0.0.1/FlyDB/client_grpc/db_pb2_grpc.py
--rw-rw-r--   0 adminonly  (1000) adminonly  (1000)     5454 2023-07-22 11:55:57.000000 FlyDB-0.0.1/FlyDB/db.py
-drwxrwxr-x   0 adminonly  (1000) adminonly  (1000)        0 2023-07-22 12:04:06.100820 FlyDB-0.0.1/FlyDB/example/
--rw-rw-r--   0 adminonly  (1000) adminonly  (1000)        0 2023-07-22 11:55:51.000000 FlyDB-0.0.1/FlyDB/example/__init__.py
--rw-rw-r--   0 adminonly  (1000) adminonly  (1000)      387 2023-07-22 12:02:27.000000 FlyDB-0.0.1/FlyDB/example/simple.py
-drwxrwxr-x   0 adminonly  (1000) adminonly  (1000)        0 2023-07-22 12:04:06.100820 FlyDB-0.0.1/FlyDB.egg-info/
--rw-rw-r--   0 adminonly  (1000) adminonly  (1000)      215 2023-07-22 12:04:06.000000 FlyDB-0.0.1/FlyDB.egg-info/PKG-INFO
--rw-rw-r--   0 adminonly  (1000) adminonly  (1000)      341 2023-07-22 12:04:06.000000 FlyDB-0.0.1/FlyDB.egg-info/SOURCES.txt
--rw-rw-r--   0 adminonly  (1000) adminonly  (1000)        1 2023-07-22 12:04:06.000000 FlyDB-0.0.1/FlyDB.egg-info/dependency_links.txt
--rw-rw-r--   0 adminonly  (1000) adminonly  (1000)       16 2023-07-22 12:04:06.000000 FlyDB-0.0.1/FlyDB.egg-info/requires.txt
--rw-rw-r--   0 adminonly  (1000) adminonly  (1000)        6 2023-07-22 12:04:06.000000 FlyDB-0.0.1/FlyDB.egg-info/top_level.txt
--rw-rw-r--   0 adminonly  (1000) adminonly  (1000)    11356 2023-07-22 09:57:00.000000 FlyDB-0.0.1/LICENSE
--rw-rw-r--   0 adminonly  (1000) adminonly  (1000)      215 2023-07-22 12:04:06.100820 FlyDB-0.0.1/PKG-INFO
--rw-rw-r--   0 adminonly  (1000) adminonly  (1000)     2656 2023-07-22 11:55:45.000000 FlyDB-0.0.1/README.md
--rw-rw-r--   0 adminonly  (1000) adminonly  (1000)       38 2023-07-22 12:04:06.100820 FlyDB-0.0.1/setup.cfg
--rw-rw-r--   0 adminonly  (1000) adminonly  (1000)      348 2023-07-22 11:57:29.000000 FlyDB-0.0.1/setup.py
+drwxrwxr-x   0 adminonly  (1000) adminonly  (1000)        0 2023-07-22 12:07:59.436335 FlyDB-0.0.2/
+drwxrwxr-x   0 adminonly  (1000) adminonly  (1000)        0 2023-07-22 12:07:59.432335 FlyDB-0.0.2/FlyDB/
+-rw-rw-r--   0 adminonly  (1000) adminonly  (1000)        0 2023-07-22 11:55:43.000000 FlyDB-0.0.2/FlyDB/__init__.py
+drwxrwxr-x   0 adminonly  (1000) adminonly  (1000)        0 2023-07-22 12:07:59.432335 FlyDB-0.0.2/FlyDB/client_grpc/
+-rw-rw-r--   0 adminonly  (1000) adminonly  (1000)        0 2023-07-22 11:55:51.000000 FlyDB-0.0.2/FlyDB/client_grpc/__init__.py
+-rw-rw-r--   0 adminonly  (1000) adminonly  (1000)    10426 2023-07-22 09:17:10.000000 FlyDB-0.0.2/FlyDB/client_grpc/db_pb2.py
+-rw-rw-r--   0 adminonly  (1000) adminonly  (1000)    28497 2023-07-22 11:55:57.000000 FlyDB-0.0.2/FlyDB/client_grpc/db_pb2_grpc.py
+-rw-rw-r--   0 adminonly  (1000) adminonly  (1000)     5453 2023-07-22 12:07:30.000000 FlyDB-0.0.2/FlyDB/db.py
+drwxrwxr-x   0 adminonly  (1000) adminonly  (1000)        0 2023-07-22 12:07:59.432335 FlyDB-0.0.2/FlyDB/example/
+-rw-rw-r--   0 adminonly  (1000) adminonly  (1000)        0 2023-07-22 11:55:51.000000 FlyDB-0.0.2/FlyDB/example/__init__.py
+-rw-rw-r--   0 adminonly  (1000) adminonly  (1000)      387 2023-07-22 12:02:27.000000 FlyDB-0.0.2/FlyDB/example/simple.py
+drwxrwxr-x   0 adminonly  (1000) adminonly  (1000)        0 2023-07-22 12:07:59.432335 FlyDB-0.0.2/FlyDB.egg-info/
+-rw-rw-r--   0 adminonly  (1000) adminonly  (1000)      215 2023-07-22 12:07:59.000000 FlyDB-0.0.2/FlyDB.egg-info/PKG-INFO
+-rw-rw-r--   0 adminonly  (1000) adminonly  (1000)      341 2023-07-22 12:07:59.000000 FlyDB-0.0.2/FlyDB.egg-info/SOURCES.txt
+-rw-rw-r--   0 adminonly  (1000) adminonly  (1000)        1 2023-07-22 12:07:59.000000 FlyDB-0.0.2/FlyDB.egg-info/dependency_links.txt
+-rw-rw-r--   0 adminonly  (1000) adminonly  (1000)       16 2023-07-22 12:07:59.000000 FlyDB-0.0.2/FlyDB.egg-info/requires.txt
+-rw-rw-r--   0 adminonly  (1000) adminonly  (1000)        6 2023-07-22 12:07:59.000000 FlyDB-0.0.2/FlyDB.egg-info/top_level.txt
+-rw-rw-r--   0 adminonly  (1000) adminonly  (1000)    11356 2023-07-22 09:57:00.000000 FlyDB-0.0.2/LICENSE
+-rw-rw-r--   0 adminonly  (1000) adminonly  (1000)      215 2023-07-22 12:07:59.436335 FlyDB-0.0.2/PKG-INFO
+-rw-rw-r--   0 adminonly  (1000) adminonly  (1000)     2656 2023-07-22 11:55:45.000000 FlyDB-0.0.2/README.md
+-rw-rw-r--   0 adminonly  (1000) adminonly  (1000)       38 2023-07-22 12:07:59.436335 FlyDB-0.0.2/setup.cfg
+-rw-rw-r--   0 adminonly  (1000) adminonly  (1000)      348 2023-07-22 12:07:54.000000 FlyDB-0.0.2/setup.py
```

### Comparing `FlyDB-0.0.1/FlyDB/client_grpc/db_pb2.py` & `FlyDB-0.0.2/FlyDB/client_grpc/db_pb2.py`

 * *Files identical despite different names*

### Comparing `FlyDB-0.0.1/FlyDB/client_grpc/db_pb2_grpc.py` & `FlyDB-0.0.2/FlyDB/client_grpc/db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `FlyDB-0.0.1/FlyDB/db.py` & `FlyDB-0.0.2/FlyDB/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Union
 import grpc
-from FlyDB2.client_grpc import db_pb2_grpc
+from FlyDB.client_grpc import db_pb2_grpc
 from FlyDB.client_grpc import db_pb2
 
 
 class FlyDB:
     def __init__(self):
         """
         Initializes a new instance of the client class.
```

### Comparing `FlyDB-0.0.1/LICENSE` & `FlyDB-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FlyDB-0.0.1/README.md` & `FlyDB-0.0.2/README.md`

 * *Files identical despite different names*

