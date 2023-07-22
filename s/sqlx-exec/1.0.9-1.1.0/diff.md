# Comparing `tmp/sqlx-exec-1.0.9.tar.gz` & `tmp/sqlx-exec-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.0.9.tar", last modified: Fri Jul 21 21:29:43 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.1.0.tar", last modified: Sat Jul 22 01:53:04 2023, max compression
```

## Comparing `sqlx-exec-1.0.9.tar` & `sqlx-exec-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 21:29:43.000000 sqlx-exec-1.0.9/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.0.9/LICENSE
--rw-rw-rw-   0        0        0     2537 2023-07-21 21:29:43.000000 sqlx-exec-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2031 2023-07-21 18:34:31.000000 sqlx-exec-1.0.9/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-21 21:29:43.000000 sqlx-exec-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1161 2023-07-21 21:29:09.000000 sqlx-exec-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 21:29:43.000000 sqlx-exec-1.0.9/sqlexec/
--rw-rw-rw-   0        0        0     2441 2023-07-21 20:40:15.000000 sqlx-exec-1.0.9/sqlexec/engin.py
--rw-rw-rw-   0        0        0    10749 2023-07-21 21:06:09.000000 sqlx-exec-1.0.9/sqlexec/exec.py
--rw-rw-rw-   0        0        0     1018 2023-07-21 18:10:23.000000 sqlx-exec-1.0.9/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     2786 2023-07-21 16:37:12.000000 sqlx-exec-1.0.9/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     1608 2023-07-21 21:27:49.000000 sqlx-exec-1.0.9/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4275 2023-07-21 16:54:46.000000 sqlx-exec-1.0.9/sqlexec/support.py
--rw-rw-rw-   0        0        0      324 2023-07-21 18:17:34.000000 sqlx-exec-1.0.9/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 21:29:43.000000 sqlx-exec-1.0.9/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-21 21:29:43.000000 sqlx-exec-1.0.9/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-21 08:56:11.000000 sqlx-exec-1.0.9/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2537 2023-07-21 21:29:43.000000 sqlx-exec-1.0.9/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-07-21 21:29:43.000000 sqlx-exec-1.0.9/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-21 21:29:43.000000 sqlx-exec-1.0.9/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 01:53:04.000000 sqlx-exec-1.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2553 2023-07-22 01:53:04.000000 sqlx-exec-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2047 2023-07-21 22:36:53.000000 sqlx-exec-1.1.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-22 01:53:04.000000 sqlx-exec-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1161 2023-07-22 01:51:14.000000 sqlx-exec-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 01:53:04.000000 sqlx-exec-1.1.0/sqlexec/
+-rw-rw-rw-   0        0        0     2457 2023-07-21 22:49:57.000000 sqlx-exec-1.1.0/sqlexec/engin.py
+-rw-rw-rw-   0        0        0    10884 2023-07-21 23:56:22.000000 sqlx-exec-1.1.0/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     1030 2023-07-21 22:35:47.000000 sqlx-exec-1.1.0/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0     2786 2023-07-21 16:37:12.000000 sqlx-exec-1.1.0/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     2421 2023-07-22 00:01:56.000000 sqlx-exec-1.1.0/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4275 2023-07-21 16:54:46.000000 sqlx-exec-1.1.0/sqlexec/support.py
+-rw-rw-rw-   0        0        0      343 2023-07-21 21:37:31.000000 sqlx-exec-1.1.0/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 01:53:04.000000 sqlx-exec-1.1.0/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-22 01:53:04.000000 sqlx-exec-1.1.0/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-21 08:56:11.000000 sqlx-exec-1.1.0/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2553 2023-07-22 01:53:04.000000 sqlx-exec-1.1.0/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-07-22 01:53:04.000000 sqlx-exec-1.1.0/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-22 01:53:04.000000 sqlx-exec-1.1.0/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.0.9/LICENSE` & `sqlx-exec-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.9/PKG-INFO` & `sqlx-exec-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.0.9
+Version: 1.1.0
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
@@ -19,17 +19,17 @@
 
    import sqlexec
    from sqlexec import Engin
 
    if __name__ == '__main__':
        sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, engin=Engin.PostgreSQL)
 
-       pk_sql = "SELECT currval('person_id_seq')"
-       id = sqlexec.save(pk_sql=pk_sql, table='person', name='zhangsan', age=15)
-       id = sqlexec.save_sql(pk_sql, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
+       select_key = "SELECT currval('person_id_seq')"
+       id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
+       id = sqlexec.save_sql(select_key, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
 
        count = sqlexec.get('select count(1) from person')
        # result: 3
 
        persons = sqlexec.select('select id, name, age from person')
        # result:
```

### Comparing `sqlx-exec-1.0.9/README.rst` & `sqlx-exec-1.1.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
    import sqlexec
    from sqlexec import Engin
 
    if __name__ == '__main__':
        sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, engin=Engin.PostgreSQL)
 
-       pk_sql = "SELECT currval('person_id_seq')"
-       id = sqlexec.save(pk_sql=pk_sql, table='person', name='zhangsan', age=15)
-       id = sqlexec.save_sql(pk_sql, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
+       select_key = "SELECT currval('person_id_seq')"
+       id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
+       id = sqlexec.save_sql(select_key, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
 
        count = sqlexec.get('select count(1) from person')
        # result: 3
 
        persons = sqlexec.select('select id, name, age from person')
        # result:
```

### Comparing `sqlx-exec-1.0.9/setup.py` & `sqlx-exec-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.0.9',
+    version='1.1.0',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.0.9/sqlexec/engin.py` & `sqlx-exec-1.1.0/sqlexec/engin.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     def page_sql_args(require_limit, sql: str, start, page_size, *args):
         if require_limit(sql):
             sql = '{} limit ?, ?'.format(sql)
         args = [*args, start, page_size]
         return sql, args
 
     @staticmethod
-    def pk_sql(*args):
+    def get_select_key(*args):
         return "SELECT LAST_INSERT_ID()"
 
 
 class PostgresEngin(SqlEngin):
 
     def __init__(self, logger, show_sql):
         super().__init__(logger, show_sql)
@@ -66,9 +66,9 @@
     def page_sql_args(require_limit, sql: str, start, page_size, *args):
         if require_limit(sql):
             sql = '{} LIMIT ? OFFSET ?'.format(sql)
         args = [*args, page_size, start]
         return sql, args
 
     @staticmethod
-    def pk_sql(pk_seq, *args):
+    def get_select_key(pk_seq, *args):
         return  "SELECT currval('{}')".format(pk_seq)
```

### Comparing `sqlx-exec-1.0.9/sqlexec/exec.py` & `sqlx-exec-1.1.0/sqlexec/exec.py`

 * *Files 3% similar despite different names*

```diff
@@ -148,44 +148,44 @@
     return: Effect rowcount
     """
     insert_log('insert', table, **kwargs)
     sql, args = sql_support.insert_sql_args(table.strip(), **kwargs)
     return execute(sql, *args)
 
 
-def save(pk_sql: str, table: str, **kwargs):
+def save(select_key: str, table: str, **kwargs):
     """
     Insert data into table, return primary key.
-    :param pk_sql: sql for getting primary key
+    :param select_key: sql for select primary key
     :param table: table
     :param kwargs:
     :return: Primary key
     """
-    save_log('save', pk_sql, table, **kwargs)
+    save_log('save', select_key, table, **kwargs)
     sql, args = sql_support.insert_sql_args(table.strip(), **kwargs)
-    return save_sql(pk_sql, sql, *args)
+    return save_sql(select_key, sql, *args)
 
 
 @with_connection
-def save_sql(pk_sql: str, sql: str, *args):
+def save_sql(select_key: str, sql: str, *args):
     """
     Insert data into table, return primary key.
-    :param pk_sql: sql for getting primary key
+    :param select_key: sql for select primary key
     :param sql: table
     :param args:
     :return: Primary key
     """
     global _DB_CTX
     cursor = None
-    logger.debug("Exec func 'sqlexec.%s', 'pk_sql': %s \n\t sql: %s \n\t args: %s" % ('save_sql', pk_sql, sql, args))
+    logger.debug("Exec func 'sqlexec.%s', 'select_key': %s \n\t sql: %s \n\t args: %s" % ('save_sql', select_key, sql, args))
     sql = sql_support.before_execute('save_sql', sql, *args)
     try:
         cursor = _DB_CTX.connection.cursor()
         cursor.execute(sql, args)
-        cursor.execute(pk_sql)
+        cursor.execute(select_key)
         result = cursor.fetchone()
         try_commit(_DB_CTX)
         return result[0]
     finally:
         if cursor:
             cursor.close()
 
@@ -209,14 +209,16 @@
     Batch execute sql return effect rowcount
     :param sql: insert into person(name, age) values(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
     :param args: All number must have same size.
     :return: Effect rowcount
     """
     global _DB_CTX
     cursor = None
+    if isinstance(args[0], dict):
+        sql, args = sql_support.batch_named_sql_args(sql, *args)
     sql = sql_support.before_execute('batch_execute', sql.strip(), *args)
     args = sql_support.get_batch_args(*args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.executemany(sql, args)
         effect_rowcount = cursor.rowcount
         try_commit(_DB_CTX)
```

### Comparing `sqlx-exec-1.0.9/sqlexec/log_support.py` & `sqlx-exec-1.1.0/sqlexec/log_support.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 basicConfig(level=INFO, format='[%(levelname)s]: %(asctime)s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
 
 
 def insert_log(function: str, table: str, **kwargs):
     logger.debug("Exec func 'sqlexec.%s' \n\t Table: '%s', kwargs: %s" % (function, table, kwargs))
 
 
-def save_log(function: str, pk_sql: str, table: str, **kwargs):
-    logger.debug("Exec func 'sqlexec.%s', 'pk_sql': %s \n\t Table: '%s', kwargs: %s" % (function, pk_sql, table, kwargs))
+def save_log(function: str, select_key: str, table: str, **kwargs):
+    logger.debug("Exec func 'sqlexec.%s', 'select_key': %s \n\t Table: '%s', kwargs: %s" % (function, select_key, table, kwargs))
 
 
 def get_log(function: str, sql: str, *args):
     logger.debug("Exec func 'sqlexec.%s' \n\t sql: %s \n\t args: %s" % (function, sql, args))
 
 
 def page_log(function: str, sql: str, page_num, page_size, *args):
```

### Comparing `sqlx-exec-1.0.9/sqlexec/pooling.py` & `sqlx-exec-1.1.0/sqlexec/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.9/sqlexec/sql_support.py` & `sqlx-exec-1.1.0/sqlexec/sql_support.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,98 @@
+import re
 from typing import Sequence
 from .log_support import logger
+from functools import lru_cache
 from .engin import Engin, MySqlEngin, PostgresEngin
 
 CACHE_SIZE = 256
+NAMED_REGEX = r':[\w|\d]*'
+_ENGIN = None
 _SQL_ENGIN = None
 before_execute = None
 
 
 def insert_sql_args(table: str, **kwargs):
     cols, args = zip(*kwargs.items())
     sql = _SQL_ENGIN.create_insert_sql(table, cols)
     return sql, args
 
 
 def get_batch_args(*args):
     return args[0] if isinstance(args, tuple) and len(args) == 1 and isinstance(args[0], Sequence) else args
 
 
+
 def batch_insert_sql_args(table: str, *args):
     args = get_batch_args(*args)
     args = [zip(*arg.items()) for arg in args]  # [(cols, args)]
     cols, args = zip(*args)  # (cols), (args)
-    sql = _SQL_ENGIN.create_insert_sql(table, cols)
+    sql = _SQL_ENGIN.create_insert_sql(table, cols[0])
     return sql, args
 
 
+def batch_named_sql_args(sql: str, *args):
+    args = get_batch_args(*args)
+    args = [get_named_args(sql, **arg) for arg in args]
+    sql = get_named_sql(sql)
+    return sql, args
+
+
+def get_named_sql_args(sql: str, **kwargs):
+    args = get_named_args(sql, **kwargs)
+    return get_named_sql(sql), args
+
+
+@lru_cache(maxsize=CACHE_SIZE)
+def get_named_sql(sql: str):
+    return re.sub(NAMED_REGEX, '?', sql)
+
+
+def get_named_args(sql: str, **kwargs):
+    return [kwargs[r[1:]] for r in re.findall(NAMED_REGEX, sql)]
+
+
 def page_sql_args(sql: str, page_num=1, page_size=10, *args):
     global _SQL_ENGIN
     start = (page_num - 1) * page_size
     return _SQL_ENGIN.page_sql_args(require_limit, sql, start, page_size, *args)
 
 
-def get_pk_sql(*args):
+def get_select_key(*args):
     global _SQL_ENGIN
-    return _SQL_ENGIN.pk_sql(*args)
+    return _SQL_ENGIN.get_select_key(*args)
 
 
 def require_limit(sql: str):
     lower_sql = sql.lower()
     if 'limit' not in lower_sql:
         return True
     idx = lower_sql.rindex('limit')
     if idx > 0 and ')' in lower_sql[idx:]:
         return True
     return False
 
 
 def set_config(engin, show_sql):
+    global _ENGIN
     global _SQL_ENGIN
     global before_execute
+    _ENGIN = engin
     if engin == Engin.MySQL:
         _SQL_ENGIN = MySqlEngin(logger, show_sql)
     elif engin == Engin.PostgreSQL:
         _SQL_ENGIN = PostgresEngin(logger, show_sql)
     before_execute = _SQL_ENGIN.before_execute
 
 
+def get_engin():
+    global _ENGIN
+    return _ENGIN
+
+
+def get_sql_engin():
+    global _SQL_ENGIN
+    return _SQL_ENGIN
+
+
```

### Comparing `sqlx-exec-1.0.9/sqlexec/support.py` & `sqlx-exec-1.1.0/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.0.9/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.1.0/sqlx_exec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.0.9
+Version: 1.1.0
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
@@ -19,17 +19,17 @@
 
    import sqlexec
    from sqlexec import Engin
 
    if __name__ == '__main__':
        sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, engin=Engin.PostgreSQL)
 
-       pk_sql = "SELECT currval('person_id_seq')"
-       id = sqlexec.save(pk_sql=pk_sql, table='person', name='zhangsan', age=15)
-       id = sqlexec.save_sql(pk_sql, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
+       select_key = "SELECT currval('person_id_seq')"
+       id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
+       id = sqlexec.save_sql(select_key, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
 
        count = sqlexec.get('select count(1) from person')
        # result: 3
 
        persons = sqlexec.select('select id, name, age from person')
        # result:
```

