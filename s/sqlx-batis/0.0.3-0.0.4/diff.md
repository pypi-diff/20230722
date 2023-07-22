# Comparing `tmp/sqlx-batis-0.0.3.tar.gz` & `tmp/sqlx-batis-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-batis-0.0.3.tar", last modified: Sat Jul 22 03:24:00 2023, max compression
+gzip compressed data, was "dist\sqlx-batis-0.0.4.tar", last modified: Sat Jul 22 18:34:09 2023, max compression
```

## Comparing `sqlx-batis-0.0.3.tar` & `sqlx-batis-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 03:24:00.000000 sqlx-batis-0.0.3/
--rw-rw-rw-   0        0        0     3430 2023-07-22 03:24:00.000000 sqlx-batis-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2948 2023-07-22 02:28:27.000000 sqlx-batis-0.0.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-22 03:24:00.000000 sqlx-batis-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-07-22 03:23:52.000000 sqlx-batis-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-22 03:24:00.000000 sqlx-batis-0.0.3/sqlxbatis/
--rw-rw-rw-   0        0        0      117 2023-07-22 00:07:56.000000 sqlx-batis-0.0.3/sqlxbatis/constant.py
--rw-rw-rw-   0        0        0     7010 2023-07-22 02:22:52.000000 sqlx-batis-0.0.3/sqlxbatis/dbx.py
--rw-rw-rw-   0        0        0      488 2023-07-22 00:16:38.000000 sqlx-batis-0.0.3/sqlxbatis/log_support.py
--rw-rw-rw-   0        0        0     7161 2023-07-22 01:21:23.000000 sqlx-batis-0.0.3/sqlxbatis/sql_holder.py
--rw-rw-rw-   0        0        0     4126 2023-07-22 02:22:52.000000 sqlx-batis-0.0.3/sqlxbatis/sql_mapper.py
--rw-rw-rw-   0        0        0     2340 2023-07-22 03:19:08.000000 sqlx-batis-0.0.3/sqlxbatis/sql_support.py
--rw-rw-rw-   0        0        0      242 2023-07-22 02:23:17.000000 sqlx-batis-0.0.3/sqlxbatis/support.py
--rw-rw-rw-   0        0        0      136 2023-07-22 02:12:40.000000 sqlx-batis-0.0.3/sqlxbatis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 03:23:59.000000 sqlx-batis-0.0.3/sqlx_batis.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-22 03:23:59.000000 sqlx-batis-0.0.3/sqlx_batis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-22 02:18:23.000000 sqlx-batis-0.0.3/sqlx_batis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3430 2023-07-22 03:23:59.000000 sqlx-batis-0.0.3/sqlx_batis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-07-22 03:23:59.000000 sqlx-batis-0.0.3/sqlx_batis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      401 2023-07-22 03:23:59.000000 sqlx-batis-0.0.3/sqlx_batis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2023-07-22 03:23:59.000000 sqlx-batis-0.0.3/sqlx_batis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 18:34:09.000000 sqlx-batis-0.0.4/
+-rw-rw-rw-   0        0        0     3430 2023-07-22 18:34:09.000000 sqlx-batis-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2948 2023-07-22 02:28:27.000000 sqlx-batis-0.0.4/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-22 18:34:09.000000 sqlx-batis-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-07-22 18:33:47.000000 sqlx-batis-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 18:34:09.000000 sqlx-batis-0.0.4/sqlxbatis/
+-rw-rw-rw-   0        0        0       64 2023-07-22 18:25:44.000000 sqlx-batis-0.0.4/sqlxbatis/constant.py
+-rw-rw-rw-   0        0        0     7033 2023-07-22 18:13:12.000000 sqlx-batis-0.0.4/sqlxbatis/dbx.py
+-rw-rw-rw-   0        0        0      818 2023-07-22 18:13:12.000000 sqlx-batis-0.0.4/sqlxbatis/exec_support.py
+-rw-rw-rw-   0        0        0      488 2023-07-22 18:24:31.000000 sqlx-batis-0.0.4/sqlxbatis/log_support.py
+-rw-rw-rw-   0        0        0     7056 2023-07-22 18:30:15.000000 sqlx-batis-0.0.4/sqlxbatis/sql_holder.py
+-rw-rw-rw-   0        0        0     4120 2023-07-22 18:31:21.000000 sqlx-batis-0.0.4/sqlxbatis/sql_mapper.py
+-rw-rw-rw-   0        0        0      616 2023-07-22 18:29:54.000000 sqlx-batis-0.0.4/sqlxbatis/sql_support.py
+-rw-rw-rw-   0        0        0      227 2023-07-22 03:49:33.000000 sqlx-batis-0.0.4/sqlxbatis/support.py
+-rw-rw-rw-   0        0        0      177 2023-07-22 03:49:33.000000 sqlx-batis-0.0.4/sqlxbatis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 18:34:09.000000 sqlx-batis-0.0.4/sqlx_batis.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-22 18:34:09.000000 sqlx-batis-0.0.4/sqlx_batis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-22 02:18:23.000000 sqlx-batis-0.0.4/sqlx_batis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3430 2023-07-22 18:34:09.000000 sqlx-batis-0.0.4/sqlx_batis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-07-22 18:34:09.000000 sqlx-batis-0.0.4/sqlx_batis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      427 2023-07-22 18:34:09.000000 sqlx-batis-0.0.4/sqlx_batis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2023-07-22 18:34:09.000000 sqlx-batis-0.0.4/sqlx_batis.egg-info/top_level.txt
```

### Comparing `sqlx-batis-0.0.3/PKG-INFO` & `sqlx-batis-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.0.3
+Version: 0.0.4
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `sqlx-batis-0.0.3/README.rst` & `sqlx-batis-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.0.3/setup.py` & `sqlx-batis-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     name='sqlx-batis',
     packages=['sqlxbatis'],
     description="sqlx-batis is a sql executor for Python like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
-        'sqlx-exec>=1.1.2',
+        'sqlx-exec>=1.1.3',
     ],
-    version='0.0.3',
+    version='0.0.4',
     url='https://gitee.com/summry/sqlx-batis',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-batis-0.0.3/sqlxbatis/dbx.py` & `sqlx-batis-0.0.4/sqlxbatis/dbx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import sqlexec
-from .sql_support import do_save, limit_one_sql_args
-from . import sql_holder as holder, Engin
-from .log_support import logger, sql_id_log, page_sql_id_log
+from .exec_support import do_save
+from . import Engin, sql_holder as holder
+from .sql_support import limit_one_sql_args
 from sqlexec.sql_support import get_batch_args
+from .log_support import logger, sql_id_log, page_sql_id_log
 
 
 def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, show_sql=False, mapper_path='mapper', engin=Engin.MySQL, **kwargs):
     holder.load_mapper(mapper_path)
-    sqlexec.init_engin(user=user, password=password, database=database, host=host, port=port, show_sql=show_sql, engin=engin, **kwargs)
+    sqlexec.init_db(user=user, password=password, database=database, host=host, port=port, show_sql=show_sql, engin=engin, **kwargs)
 
 
 def insert(table: str, **kwargs):
     """
     Insert data into table, return effect rowcount.
     :param table: table name
     :param kwargs: {'name': '张三', 'age': 20}
```

### Comparing `sqlx-batis-0.0.3/sqlxbatis/sql_holder.py` & `sqlx-batis-0.0.4/sqlxbatis/sql_holder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 import os
 import re
 from typing import List
 from typing import Mapping
 from jinja2 import Template
 from .log_support import logger
 from .support import MapperError, SqlAction
-from sqlexec.sql_support import get_named_sql_args
-from .constant import DYNAMIC_REGEX
+from .sql_support import is_dynamic_sql, get_named_sql_args
 
 try:
     import xml.etree.cElementTree as ET
 except ImportError:
     import xml.etree.ElementTree as ET
 
 _SQL_CONTAINER = dict()
 _valid_sql_actions = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.SELECT.value)
 
 
-
 class SqlModel:
     def __init__(self, sql: str, action: str, namespace: str, dynamic=False, includes: List[str] = None, pk_seq: str = None, select_key: str=None):
         self.sql = sql
         self.action = action
         self.namespace = namespace
         self.dynamic = dynamic
         self.includes = includes
         self.pk_seq = pk_seq
         self.select_key = select_key
         self.mapping = True if dynamic else ':' in sql
         self.placeholder = False if self.mapping else '?' in sql
 
-def is_dynamic_sql(sql: str):
-    return re.search(DYNAMIC_REGEX, sql)
-
 
 def get_sql(sql_id: str, *args, **kwargs):
     sql_model = get_sql_model(sql_id)
     return do_get_sql(sql_model, False, None, *args, **kwargs)
 
 
 def do_get_sql(sql_model, batch, param_names, *args, **kwargs):
```

### Comparing `sqlx-batis-0.0.3/sqlxbatis/sql_mapper.py` & `sqlx-batis-0.0.4/sqlxbatis/sql_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sqlexec
 import functools
 from .support import SqlAction
 from .log_support import logger
-from sqlexec.sql_support import get_named_sql_args
-from .sql_support import simple_sql, do_save, do_save0
+from .exec_support import do_save, do_save0
+from .sql_support import simple_sql, get_named_sql_args
 from .sql_holder import get_sql_model, do_get_sql, build_sql_id
 
 _UPDATE_ACTIONS = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.CALL.value)
 
 
 def mapper(namespace: str = None, sql_id: str = None, batch=False, return_pk=False):
     def _decorator(func):
```

### Comparing `sqlx-batis-0.0.3/sqlx_batis.egg-info/PKG-INFO` & `sqlx-batis-0.0.4/sqlx_batis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.0.3
+Version: 0.0.4
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

