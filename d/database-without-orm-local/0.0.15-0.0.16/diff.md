# Comparing `tmp/database-without-orm-local-0.0.15.tar.gz` & `tmp/database-without-orm-local-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-without-orm-local-0.0.15.tar", last modified: Fri Jul 21 11:59:01 2023, max compression
+gzip compressed data, was "database-without-orm-local-0.0.16.tar", last modified: Sat Jul 22 09:52:29 2023, max compression
```

## Comparing `database-without-orm-local-0.0.15.tar` & `database-without-orm-local-0.0.16.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:59:01.054879 database-without-orm-local-0.0.15/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:58:40.000000 database-without-orm-local-0.0.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-21 11:59:01.054879 database-without-orm-local-0.0.15/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:59:01.054879 database-without-orm-local-0.0.15/circles_local_database_python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:58:40.000000 database-without-orm-local-0.0.15/circles_local_database_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-21 11:58:40.000000 database-without-orm-local-0.0.15/circles_local_database_python/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:59:01.054879 database-without-orm-local-0.0.15/database_without_orm_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-21 11:59:01.000000 database-without-orm-local-0.0.15/database_without_orm_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-21 11:59:01.000000 database-without-orm-local-0.0.15/database_without_orm_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:59:01.000000 database-without-orm-local-0.0.15/database_without_orm_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-21 11:59:01.000000 database-without-orm-local-0.0.15/database_without_orm_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-21 11:58:40.000000 database-without-orm-local-0.0.15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 11:59:01.054879 database-without-orm-local-0.0.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-21 11:58:40.000000 database-without-orm-local-0.0.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:52:29.645074 database-without-orm-local-0.0.16/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:52:06.000000 database-without-orm-local-0.0.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-22 09:52:29.645074 database-without-orm-local-0.0.16/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:52:29.645074 database-without-orm-local-0.0.16/circles_local_database_python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:52:06.000000 database-without-orm-local-0.0.16/circles_local_database_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-22 09:52:06.000000 database-without-orm-local-0.0.16/circles_local_database_python/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:52:29.645074 database-without-orm-local-0.0.16/database_without_orm_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-22 09:52:29.000000 database-without-orm-local-0.0.16/database_without_orm_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-22 09:52:29.000000 database-without-orm-local-0.0.16/database_without_orm_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 09:52:29.000000 database-without-orm-local-0.0.16/database_without_orm_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-22 09:52:29.000000 database-without-orm-local-0.0.16/database_without_orm_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-22 09:52:06.000000 database-without-orm-local-0.0.16/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 09:52:29.645074 database-without-orm-local-0.0.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-22 09:52:06.000000 database-without-orm-local-0.0.16/setup.py
```

### Comparing `database-without-orm-local-0.0.15/circles_local_database_python/database.py` & `database-without-orm-local-0.0.16/circles_local_database_python/database.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import mysql.connector
 import os
 from dotenv import load_dotenv
-from logger_local_python_package.LocalLogger import logger_local
+from logger_local_python_package.LoggerLocal import logger_local
 load_dotenv()
 
-component_id=112
+COMPONENT_ID=112
 
 
 class database():
 
     def connect_to_database(self):
+        logger_local.init(object={'component_id' :COMPONENT_ID})
         try:
             host=os.getenv("RDS_HOSTNAME")if os.getenv("RDS_HOSTNAME") else " "
             user=os.getenv("RDS_USERNAME")if os.getenv("RDS_USERNAME") else " "
             password=os.getenv("RDS_PASSWORD")if os.getenv("RDS_PASSWORD") else " "
             object1={
                 'host':os.getenv("RDS_HOSTNAME"),
                 'user':os.getenv("RDS_USERNAME"),
-                'password':os.getenv("RDS_PASSWORD"),
-                'component_id' :component_id
+                'password':os.getenv("RDS_PASSWORD")          
             }
             logger_local.start(object=object1)
             mydb = mysql.connector.connect(
             host=os.getenv("RDS_HOSTNAME"),
             user=os.getenv("RDS_USERNAME"),
             password=os.getenv("RDS_PASSWORD")
         )
-            logger_local.end(object={'component_id' :component_id})
+            logger_local.end(object={})
             return mydb
         except Exception as e:
             logger_local.exception(str(host+" "+user+" "+password),object=e)
```

### Comparing `database-without-orm-local-0.0.15/setup.py` & `database-without-orm-local-0.0.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 # used by python -m build
 setuptools.setup(
      name='database-without-orm-local',  
-     version='0.0.15', # https://pypi.org/project/database-without-orm-local/
+     version='0.0.16', # https://pypi.org/project/database-without-orm-local/
      author="Circles",
      author_email="info@circles.life",
      description="Circles Local Database without ORM Python PyPI Package",
      long_description="This is a package for sharing common Database methods",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

