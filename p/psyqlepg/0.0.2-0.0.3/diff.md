# Comparing `tmp/psyqlepg-0.0.2.tar.gz` & `tmp/psyqlepg-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyqlepg-0.0.2.tar", last modified: Wed Jul 19 09:24:10 2023, max compression
+gzip compressed data, was "psyqlepg-0.0.3.tar", last modified: Sat Jul 22 06:29:06 2023, max compression
```

## Comparing `psyqlepg-0.0.2.tar` & `psyqlepg-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-19 09:24:10.113987 psyqlepg-0.0.2/
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)     1515 2023-07-19 09:19:30.000000 psyqlepg-0.0.2/LICENSE
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      565 2023-07-19 09:24:10.112987 psyqlepg-0.0.2/PKG-INFO
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)       49 2023-07-19 09:20:45.000000 psyqlepg-0.0.2/README.md
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      502 2023-07-19 09:21:34.000000 psyqlepg-0.0.2/pyproject.toml
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)       38 2023-07-19 09:24:10.113987 psyqlepg-0.0.2/setup.cfg
-drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-19 09:24:10.107987 psyqlepg-0.0.2/src/
-drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-19 09:24:10.111987 psyqlepg-0.0.2/src/psyqlepg/
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)     4177 2023-07-19 09:22:09.000000 psyqlepg-0.0.2/src/psyqlepg/__init__.py
-drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-19 09:24:10.112987 psyqlepg-0.0.2/src/psyqlepg.egg-info/
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      565 2023-07-19 09:24:10.000000 psyqlepg-0.0.2/src/psyqlepg.egg-info/PKG-INFO
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      201 2023-07-19 09:24:10.000000 psyqlepg-0.0.2/src/psyqlepg.egg-info/SOURCES.txt
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)        1 2023-07-19 09:24:10.000000 psyqlepg-0.0.2/src/psyqlepg.egg-info/dependency_links.txt
--rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)        9 2023-07-19 09:24:10.000000 psyqlepg-0.0.2/src/psyqlepg.egg-info/top_level.txt
+drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-22 06:29:06.829032 psyqlepg-0.0.3/
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)     1515 2023-07-19 09:19:30.000000 psyqlepg-0.0.3/LICENSE
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      735 2023-07-22 06:29:06.829032 psyqlepg-0.0.3/PKG-INFO
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      219 2023-07-19 09:40:34.000000 psyqlepg-0.0.3/README.md
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      502 2023-07-22 06:13:44.000000 psyqlepg-0.0.3/pyproject.toml
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)       38 2023-07-22 06:29:06.829032 psyqlepg-0.0.3/setup.cfg
+drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-22 06:29:06.826032 psyqlepg-0.0.3/src/
+drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-22 06:29:06.828032 psyqlepg-0.0.3/src/psyqlepg/
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)     4193 2023-07-22 06:22:32.000000 psyqlepg-0.0.3/src/psyqlepg/__init__.py
+drwxr-xr-x   0 dbezborodov  (1001) dbezborodov  (1001)        0 2023-07-22 06:29:06.829032 psyqlepg-0.0.3/src/psyqlepg.egg-info/
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      735 2023-07-22 06:29:06.000000 psyqlepg-0.0.3/src/psyqlepg.egg-info/PKG-INFO
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)      201 2023-07-22 06:29:06.000000 psyqlepg-0.0.3/src/psyqlepg.egg-info/SOURCES.txt
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)        1 2023-07-22 06:29:06.000000 psyqlepg-0.0.3/src/psyqlepg.egg-info/dependency_links.txt
+-rw-r--r--   0 dbezborodov  (1001) dbezborodov  (1001)        9 2023-07-22 06:29:06.000000 psyqlepg-0.0.3/src/psyqlepg.egg-info/top_level.txt
```

### Comparing `psyqlepg-0.0.2/LICENSE` & `psyqlepg-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psyqlepg-0.0.2/PKG-INFO` & `psyqlepg-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 Metadata-Version: 2.1
 Name: psyqlepg
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple SQL library for psycopg3.
 Author-email: Damien Bezborodov <dbezborodov@gmail.com>
 Project-URL: Homepage, https://github.com/bezborodow/psyqlepg
 Project-URL: Bug Tracker, https://github.com/bezborodow/psyqlepg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Psysqlpg: Basic Common SQL Queries for Psycopg
+# Psyqlepg: Basic Common SQL Queries for Psycopg
+
+ * [Psycopg Documentation](https://www.psycopg.org/psycopg3/docs/)
+
+## Development
+
+ * [Packaging](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
```

### Comparing `psyqlepg-0.0.2/src/psyqlepg/__init__.py` & `psyqlepg-0.0.3/src/psyqlepg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,54 @@
 from psycopg import sql
 import re
 
 
+class Where:
+    def __init__(self, name=None, value=None):
+        self.params = []
+        self.args = []
+        if (name):
+            self.append(name, value)
+
+
+    def append(self, name, value=None):
+        if isinstance(name, sql.Composable):
+            self.params.append(name)
+        else:
+            self.params.append(sql.SQL('{} = %s').format(sql.Identifier(name)))
+            self.args.append(value)
+        return self
+
+    def clause(self):
+        if not self.params:
+            return sql.SQL('true').format()
+
+        return sql.SQL('{params}').format(
+            params=sql.SQL(' and ').join(self.params))
+
+
+    def as_string(self, context):
+        return self.clause().as_string(context)
+
+
 def selectone(conn, table, primary_key, identifier):
     query = sql.SQL('''
         select *
         from {table}
         where {primary_key} = %s
         limit 1
     ''').format(
             table=sql.Identifier(table),
             primary_key=sql.Identifier(primary_key))
 
     cur = conn.execute(query, [identifier])
     return cur.fetchone()
 
 
-def selectall(conn, table, where):
+def selectall(conn, table, where=Where()):
     query = sql.SQL('''
         select *
         from {table}
         where {where}
     ''').format(
             where=where.clause(),
             table=sql.Identifier(table))
@@ -83,51 +111,23 @@
                     queries[name] = line
                 else:
                     queries[name] += line
 
         return queries
 
 
-class Where:
-    def __init__(self, name=None, value=None):
-        self.params = []
-        self.args = []
-        if (name):
-            self.append(name, value)
-
-
-    def append(self, name, value=None):
-        if isinstance(name, sql.Composable):
-            self.params.append(name)
-        else:
-            self.params.append(sql.SQL('{} = %s').format(sql.Identifier(name)))
-            self.args.append(value)
-        return self
-
-    def clause(self):
-        if not self.params:
-            return sql.SQL('true').format()
-
-        return sql.SQL('{params}').format(
-            params=sql.SQL(' and ').join(self.params))
-
-
-    def as_string(self, context):
-        return self.clause().as_string(context)
-
-
 class Table:
     queries = None
 
     @classmethod
     def get(cls, conn, identifier, key=None):
         return selectone(conn, cls.table, key or cls.primary_key, identifier)
 
     @classmethod
-    def find(cls, conn, where):
+    def find(cls, conn, where=Where()):
         return selectall(conn, cls.table, where)
 
     @classmethod
     def insert(cls, conn, **kwargs):
         return insert(conn, cls.table, cls.primary_key, **kwargs)
 
     @classmethod
```

### Comparing `psyqlepg-0.0.2/src/psyqlepg.egg-info/PKG-INFO` & `psyqlepg-0.0.3/src/psyqlepg.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 Metadata-Version: 2.1
 Name: psyqlepg
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple SQL library for psycopg3.
 Author-email: Damien Bezborodov <dbezborodov@gmail.com>
 Project-URL: Homepage, https://github.com/bezborodow/psyqlepg
 Project-URL: Bug Tracker, https://github.com/bezborodow/psyqlepg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Psysqlpg: Basic Common SQL Queries for Psycopg
+# Psyqlepg: Basic Common SQL Queries for Psycopg
+
+ * [Psycopg Documentation](https://www.psycopg.org/psycopg3/docs/)
+
+## Development
+
+ * [Packaging](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
```

