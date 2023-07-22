# Comparing `tmp/sqlx-exec-1.1.0.tar.gz` & `tmp/sqlx-exec-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.1.0.tar", last modified: Sat Jul 22 01:53:04 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.1.1.tar", last modified: Sat Jul 22 02:05:38 2023, max compression
```

## Comparing `sqlx-exec-1.1.0.tar` & `sqlx-exec-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 01:53:04.000000 sqlx-exec-1.1.0/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2553 2023-07-22 01:53:04.000000 sqlx-exec-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2047 2023-07-21 22:36:53.000000 sqlx-exec-1.1.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-22 01:53:04.000000 sqlx-exec-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1161 2023-07-22 01:51:14.000000 sqlx-exec-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-22 01:53:04.000000 sqlx-exec-1.1.0/sqlexec/
--rw-rw-rw-   0        0        0     2457 2023-07-21 22:49:57.000000 sqlx-exec-1.1.0/sqlexec/engin.py
--rw-rw-rw-   0        0        0    10884 2023-07-21 23:56:22.000000 sqlx-exec-1.1.0/sqlexec/exec.py
--rw-rw-rw-   0        0        0     1030 2023-07-21 22:35:47.000000 sqlx-exec-1.1.0/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     2786 2023-07-21 16:37:12.000000 sqlx-exec-1.1.0/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     2421 2023-07-22 00:01:56.000000 sqlx-exec-1.1.0/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4275 2023-07-21 16:54:46.000000 sqlx-exec-1.1.0/sqlexec/support.py
--rw-rw-rw-   0        0        0      343 2023-07-21 21:37:31.000000 sqlx-exec-1.1.0/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 01:53:04.000000 sqlx-exec-1.1.0/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-22 01:53:04.000000 sqlx-exec-1.1.0/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-21 08:56:11.000000 sqlx-exec-1.1.0/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2553 2023-07-22 01:53:04.000000 sqlx-exec-1.1.0/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-07-22 01:53:04.000000 sqlx-exec-1.1.0/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-22 01:53:04.000000 sqlx-exec-1.1.0/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 02:05:38.000000 sqlx-exec-1.1.1/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2553 2023-07-22 02:05:38.000000 sqlx-exec-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2047 2023-07-21 22:36:53.000000 sqlx-exec-1.1.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-22 02:05:38.000000 sqlx-exec-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1161 2023-07-22 02:05:34.000000 sqlx-exec-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 02:05:38.000000 sqlx-exec-1.1.1/sqlexec/
+-rw-rw-rw-   0        0        0     2457 2023-07-21 22:49:57.000000 sqlx-exec-1.1.1/sqlexec/engin.py
+-rw-rw-rw-   0        0        0    10884 2023-07-21 23:56:22.000000 sqlx-exec-1.1.1/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     1030 2023-07-21 22:35:47.000000 sqlx-exec-1.1.1/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0     2786 2023-07-21 16:37:12.000000 sqlx-exec-1.1.1/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     2419 2023-07-22 02:04:44.000000 sqlx-exec-1.1.1/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4275 2023-07-21 16:54:46.000000 sqlx-exec-1.1.1/sqlexec/support.py
+-rw-rw-rw-   0        0        0      364 2023-07-22 02:04:16.000000 sqlx-exec-1.1.1/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 02:05:38.000000 sqlx-exec-1.1.1/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-22 02:05:38.000000 sqlx-exec-1.1.1/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-21 08:56:11.000000 sqlx-exec-1.1.1/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2553 2023-07-22 02:05:38.000000 sqlx-exec-1.1.1/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-07-22 02:05:38.000000 sqlx-exec-1.1.1/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-22 02:05:38.000000 sqlx-exec-1.1.1/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.1.0/LICENSE` & `sqlx-exec-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.0/PKG-INFO` & `sqlx-exec-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.1.0
+Version: 1.1.1
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
```

### Comparing `sqlx-exec-1.1.0/README.rst` & `sqlx-exec-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.0/setup.py` & `sqlx-exec-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.1.0',
+    version='1.1.1',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.1.0/sqlexec/engin.py` & `sqlx-exec-1.1.1/sqlexec/engin.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.0/sqlexec/exec.py` & `sqlx-exec-1.1.1/sqlexec/exec.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.0/sqlexec/log_support.py` & `sqlx-exec-1.1.1/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.0/sqlexec/pooling.py` & `sqlx-exec-1.1.1/sqlexec/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.0/sqlexec/sql_support.py` & `sqlx-exec-1.1.1/sqlexec/sql_support.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     return sql, args
 
 
 def get_batch_args(*args):
     return args[0] if isinstance(args, tuple) and len(args) == 1 and isinstance(args[0], Sequence) else args
 
 
-
 def batch_insert_sql_args(table: str, *args):
     args = get_batch_args(*args)
     args = [zip(*arg.items()) for arg in args]  # [(cols, args)]
     cols, args = zip(*args)  # (cols), (args)
     sql = _SQL_ENGIN.create_insert_sql(table, cols[0])
     return sql, args
```

### Comparing `sqlx-exec-1.1.0/sqlexec/support.py` & `sqlx-exec-1.1.1/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.0/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.1.1/sqlx_exec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.1.0
+Version: 1.1.1
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
```

