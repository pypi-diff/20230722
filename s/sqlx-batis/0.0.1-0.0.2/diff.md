# Comparing `tmp/sqlx-batis-0.0.1.tar.gz` & `tmp/sqlx-batis-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-batis-0.0.1.tar", last modified: Sat Jul 22 02:18:23 2023, max compression
+gzip compressed data, was "dist\sqlx-batis-0.0.2.tar", last modified: Sat Jul 22 02:29:35 2023, max compression
```

## Comparing `sqlx-batis-0.0.1.tar` & `sqlx-batis-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 02:18:23.000000 sqlx-batis-0.0.1/
--rw-rw-rw-   0        0        0     3421 2023-07-22 02:18:23.000000 sqlx-batis-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2939 2023-07-22 02:17:14.000000 sqlx-batis-0.0.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-22 02:18:23.000000 sqlx-batis-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-07-22 02:08:25.000000 sqlx-batis-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-22 02:18:23.000000 sqlx-batis-0.0.1/sqlxbatis/
--rw-rw-rw-   0        0        0      117 2023-07-22 00:07:56.000000 sqlx-batis-0.0.1/sqlxbatis/constant.py
--rw-rw-rw-   0        0        0     7030 2023-07-22 02:03:32.000000 sqlx-batis-0.0.1/sqlxbatis/dbx.py
--rw-rw-rw-   0        0        0      488 2023-07-22 00:16:38.000000 sqlx-batis-0.0.1/sqlxbatis/log_support.py
--rw-rw-rw-   0        0        0     7161 2023-07-22 01:21:23.000000 sqlx-batis-0.0.1/sqlxbatis/sql_holder.py
--rw-rw-rw-   0        0        0     4137 2023-07-22 01:48:11.000000 sqlx-batis-0.0.1/sqlxbatis/sql_mapper.py
--rw-rw-rw-   0        0        0     2345 2023-07-22 01:49:20.000000 sqlx-batis-0.0.1/sqlxbatis/sql_support.py
--rw-rw-rw-   0        0        0      244 2023-07-21 22:13:30.000000 sqlx-batis-0.0.1/sqlxbatis/support.py
--rw-rw-rw-   0        0        0      136 2023-07-22 02:12:40.000000 sqlx-batis-0.0.1/sqlxbatis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 02:18:23.000000 sqlx-batis-0.0.1/sqlx_batis.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-22 02:18:23.000000 sqlx-batis-0.0.1/sqlx_batis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-22 02:18:23.000000 sqlx-batis-0.0.1/sqlx_batis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3421 2023-07-22 02:18:23.000000 sqlx-batis-0.0.1/sqlx_batis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-07-22 02:18:23.000000 sqlx-batis-0.0.1/sqlx_batis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      401 2023-07-22 02:18:23.000000 sqlx-batis-0.0.1/sqlx_batis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2023-07-22 02:18:23.000000 sqlx-batis-0.0.1/sqlx_batis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 02:29:35.000000 sqlx-batis-0.0.2/
+-rw-rw-rw-   0        0        0     3430 2023-07-22 02:29:35.000000 sqlx-batis-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2948 2023-07-22 02:28:27.000000 sqlx-batis-0.0.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-22 02:29:35.000000 sqlx-batis-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-07-22 02:29:32.000000 sqlx-batis-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 02:29:35.000000 sqlx-batis-0.0.2/sqlxbatis/
+-rw-rw-rw-   0        0        0      117 2023-07-22 00:07:56.000000 sqlx-batis-0.0.2/sqlxbatis/constant.py
+-rw-rw-rw-   0        0        0     7010 2023-07-22 02:22:52.000000 sqlx-batis-0.0.2/sqlxbatis/dbx.py
+-rw-rw-rw-   0        0        0      488 2023-07-22 00:16:38.000000 sqlx-batis-0.0.2/sqlxbatis/log_support.py
+-rw-rw-rw-   0        0        0     7161 2023-07-22 01:21:23.000000 sqlx-batis-0.0.2/sqlxbatis/sql_holder.py
+-rw-rw-rw-   0        0        0     4126 2023-07-22 02:22:52.000000 sqlx-batis-0.0.2/sqlxbatis/sql_mapper.py
+-rw-rw-rw-   0        0        0     2325 2023-07-22 02:22:52.000000 sqlx-batis-0.0.2/sqlxbatis/sql_support.py
+-rw-rw-rw-   0        0        0      242 2023-07-22 02:23:17.000000 sqlx-batis-0.0.2/sqlxbatis/support.py
+-rw-rw-rw-   0        0        0      136 2023-07-22 02:12:40.000000 sqlx-batis-0.0.2/sqlxbatis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 02:29:35.000000 sqlx-batis-0.0.2/sqlx_batis.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-22 02:29:34.000000 sqlx-batis-0.0.2/sqlx_batis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-22 02:18:23.000000 sqlx-batis-0.0.2/sqlx_batis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3430 2023-07-22 02:29:34.000000 sqlx-batis-0.0.2/sqlx_batis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-07-22 02:29:34.000000 sqlx-batis-0.0.2/sqlx_batis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      401 2023-07-22 02:29:35.000000 sqlx-batis-0.0.2/sqlx_batis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2023-07-22 02:29:34.000000 sqlx-batis-0.0.2/sqlx_batis.egg-info/top_level.txt
```

### Comparing `sqlx-batis-0.0.1/PKG-INFO` & `sqlx-batis-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.0.1
+Version: 0.0.2
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -109,14 +109,14 @@
 
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 
-If you want to operate MySQL database, you may need MySqlx: https://pypi.org/project/mysqlx
+If you want to operate MySQL database, may be you need MySqlx: https://pypi.org/project/mysqlx
 
-If you want to operate PostgreSQL database, you may need MySqlx: https://pypi.org/project/pgsqlx
+If you want to operate PostgreSQL database, may be you need MySqlx: https://pypi.org/project/pgsqlx
 
-If you just wanted a simple sql executor, you may need sqlx-exec: https://pypi.org/project/sqlx-exec
+If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
```

### Comparing `sqlx-batis-0.0.1/README.rst` & `sqlx-batis-0.0.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -96,12 +96,12 @@
 
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 
-If you want to operate MySQL database, you may need MySqlx: https://pypi.org/project/mysqlx
+If you want to operate MySQL database, may be you need MySqlx: https://pypi.org/project/mysqlx
 
-If you want to operate PostgreSQL database, you may need MySqlx: https://pypi.org/project/pgsqlx
+If you want to operate PostgreSQL database, may be you need MySqlx: https://pypi.org/project/pgsqlx
 
-If you just wanted a simple sql executor, you may need sqlx-exec: https://pypi.org/project/sqlx-exec
+If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
```

### Comparing `sqlx-batis-0.0.1/setup.py` & `sqlx-batis-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     name='sqlx-batis',
     packages=['sqlxbatis'],
     description="sqlx-batis is a sql executor for Python like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
-        'sqlx-exec>=1.1.0',
+        'sqlx-exec>=1.1.2',
     ],
-    version='0.0.1',
+    version='0.0.2',
     url='https://gitee.com/summry/sqlx-batis',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-batis-0.0.1/sqlxbatis/dbx.py` & `sqlx-batis-0.0.2/sqlxbatis/dbx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import sqlexec
-from sqlexec import Engin
 from .sql_support import do_save, limit_one_sql_args
-from . import sql_holder as holder
+from . import sql_holder as holder, Engin
 from .log_support import logger, sql_id_log, page_sql_id_log
 from sqlexec.sql_support import get_batch_args
 
 
 def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, show_sql=False, mapper_path='mapper', engin=Engin.MySQL, **kwargs):
     holder.load_mapper(mapper_path)
     sqlexec.init_engin(user=user, password=password, database=database, host=host, port=port, show_sql=show_sql, engin=engin, **kwargs)
```

### Comparing `sqlx-batis-0.0.1/sqlxbatis/sql_holder.py` & `sqlx-batis-0.0.2/sqlxbatis/sql_holder.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.0.1/sqlxbatis/sql_mapper.py` & `sqlx-batis-0.0.2/sqlxbatis/sql_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
-import re
 import sqlexec
 import functools
 from .support import SqlAction
 from .log_support import logger
-from .sql_support import simple_sql, do_save, do_save0
 from sqlexec.sql_support import get_named_sql_args
+from .sql_support import simple_sql, do_save, do_save0
 from .sql_holder import get_sql_model, do_get_sql, build_sql_id
 
 _UPDATE_ACTIONS = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.CALL.value)
 
 
 def mapper(namespace: str = None, sql_id: str = None, batch=False, return_pk=False):
     def _decorator(func):
```

### Comparing `sqlx-batis-0.0.1/sqlxbatis/sql_support.py` & `sqlx-batis-0.0.2/sqlxbatis/sql_support.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import re
 import sqlexec
-from sqlexec import Engin
 from jinja2 import Template
 from .support import SqlAction
 from .log_support import logger
 from functools import lru_cache
 from .support import MapperError
-from . import sql_holder as holder
+from . import sql_holder as holder, Engin
 from .constant import CACHE_SIZE, LIMIT_1, DYNAMIC_REGEX
 from sqlexec.sql_support import get_select_key, get_engin, require_limit, get_named_sql_args
 
 def simple_sql(sql: str, *args, **kwargs):
     return get_named_sql_args(sql, **kwargs) if kwargs else (sql, args)
```

### Comparing `sqlx-batis-0.0.1/sqlx_batis.egg-info/PKG-INFO` & `sqlx-batis-0.0.2/sqlx_batis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.0.1
+Version: 0.0.2
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -109,14 +109,14 @@
 
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 
-If you want to operate MySQL database, you may need MySqlx: https://pypi.org/project/mysqlx
+If you want to operate MySQL database, may be you need MySqlx: https://pypi.org/project/mysqlx
 
-If you want to operate PostgreSQL database, you may need MySqlx: https://pypi.org/project/pgsqlx
+If you want to operate PostgreSQL database, may be you need MySqlx: https://pypi.org/project/pgsqlx
 
-If you just wanted a simple sql executor, you may need sqlx-exec: https://pypi.org/project/sqlx-exec
+If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
```

