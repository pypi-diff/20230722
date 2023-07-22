# Comparing `tmp/hedgesql-1.3.1.tar.gz` & `tmp/hedgesql-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hedgesql-1.3.1.tar", last modified: Sun Jul 16 09:00:00 2023, max compression
+gzip compressed data, was "hedgesql-1.3.2.tar", last modified: Sat Jul 22 18:38:16 2023, max compression
```

## Comparing `hedgesql-1.3.1.tar` & `hedgesql-1.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-07-16 09:00:00.248837 hedgesql-1.3.1/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 hedgesql-1.3.1/LICENSE
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      616 2023-07-16 09:00:00.248837 hedgesql-1.3.1/PKG-INFO
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-07-16 09:00:00.248837 hedgesql-1.3.1/hedgesql/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)       96 2023-06-18 17:46:31.000000 hedgesql-1.3.1/hedgesql/__init__.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     5214 2023-06-23 17:25:05.000000 hedgesql-1.3.1/hedgesql/datatypes.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     9711 2023-07-16 08:59:16.000000 hedgesql-1.3.1/hedgesql/hedge_sql.py
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-07-16 09:00:00.248837 hedgesql-1.3.1/hedgesql.egg-info/
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      616 2023-07-16 08:59:59.000000 hedgesql-1.3.1/hedgesql.egg-info/PKG-INFO
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      240 2023-07-16 09:00:00.000000 hedgesql-1.3.1/hedgesql.egg-info/SOURCES.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-07-16 08:59:59.000000 hedgesql-1.3.1/hedgesql.egg-info/dependency_links.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-07-16 08:59:59.000000 hedgesql-1.3.1/hedgesql.egg-info/requires.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        9 2023-07-16 08:59:59.000000 hedgesql-1.3.1/hedgesql.egg-info/top_level.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-07-16 09:00:00.248837 hedgesql-1.3.1/setup.cfg
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      761 2023-07-16 08:59:34.000000 hedgesql-1.3.1/setup.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-07-22 18:38:16.909311 hedgesql-1.3.2/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 hedgesql-1.3.2/LICENSE
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      616 2023-07-22 18:38:16.909311 hedgesql-1.3.2/PKG-INFO
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-07-22 18:38:16.909311 hedgesql-1.3.2/hedgesql/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)       96 2023-06-18 17:46:31.000000 hedgesql-1.3.2/hedgesql/__init__.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     5214 2023-06-23 17:25:05.000000 hedgesql-1.3.2/hedgesql/datatypes.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     9835 2023-07-22 18:37:23.000000 hedgesql-1.3.2/hedgesql/hedge_sql.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-07-22 18:38:16.909311 hedgesql-1.3.2/hedgesql.egg-info/
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      616 2023-07-22 18:38:16.000000 hedgesql-1.3.2/hedgesql.egg-info/PKG-INFO
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      240 2023-07-22 18:38:16.000000 hedgesql-1.3.2/hedgesql.egg-info/SOURCES.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-07-22 18:38:16.000000 hedgesql-1.3.2/hedgesql.egg-info/dependency_links.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-07-22 18:38:16.000000 hedgesql-1.3.2/hedgesql.egg-info/requires.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        9 2023-07-22 18:38:16.000000 hedgesql-1.3.2/hedgesql.egg-info/top_level.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-07-22 18:38:16.909311 hedgesql-1.3.2/setup.cfg
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      761 2023-07-22 18:37:50.000000 hedgesql-1.3.2/setup.py
```

### Comparing `hedgesql-1.3.1/LICENSE` & `hedgesql-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hedgesql-1.3.1/PKG-INFO` & `hedgesql-1.3.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hedgesql
-Version: 1.3.1
+Version: 1.3.2
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/I-HedgeDev/litesqlite
 Author: HedgeDev
 Author-email: hedge_dev@mail.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `hedgesql-1.3.1/hedgesql/datatypes.py` & `hedgesql-1.3.2/hedgesql/datatypes.py`

 * *Files identical despite different names*

### Comparing `hedgesql-1.3.1/hedgesql/hedge_sql.py` & `hedgesql-1.3.2/hedgesql/hedge_sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,18 +73,19 @@
                     table_name: str,
                     set_data: Dict[str, Union[str, int, float]],
                     where: Optional[List[Dict[str, Union[str, int, float]]]] = None) -> None:
         values = []
         set_clause_parts = []
 
         for col, value in set_data.items():
-            if isinstance(value, str) and value.startswith('+'):
+            if isinstance(value, str) and value.startswith('+') or value.startswith('-'):
                 col_name = col
                 col_value = value[1:]
-                set_clause_parts.append(f"{col_name}={col_name}+?")
+                sign = value[0]
+                set_clause_parts.append(f"{col_name}={col_name}{sign}?")
                 values.append(col_value)
             else:
                 set_clause_parts.append(f"{col}=?")
                 values.append(value)
 
         set_clause = ', '.join(set_clause_parts)
 
@@ -197,18 +198,19 @@
                           table_name: str,
                           set_data: Dict[str, Union[str, int, float]],
                           where: Optional[List[Dict[str, Union[str, int, float]]]] = None) -> None:
         values = []
         set_clause_parts = []
 
         for col, value in set_data.items():
-            if isinstance(value, str) and value.startswith('+'):
+            if isinstance(value, str) and value.startswith('+') or value.startswith('-'):
                 col_name = col
                 col_value = value[1:]
-                set_clause_parts.append(f"{col_name}={col_name}+?")
+                sign = value[0]
+                set_clause_parts.append(f"{col_name}={col_name}{sign}?")
                 values.append(col_value)
             else:
                 set_clause_parts.append(f"{col}=?")
                 values.append(value)
 
         set_clause = ', '.join(set_clause_parts)
```

### Comparing `hedgesql-1.3.1/hedgesql.egg-info/PKG-INFO` & `hedgesql-1.3.2/hedgesql.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hedgesql
-Version: 1.3.1
+Version: 1.3.2
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/I-HedgeDev/litesqlite
 Author: HedgeDev
 Author-email: hedge_dev@mail.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `hedgesql-1.3.1/setup.py` & `hedgesql-1.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='hedgesql',
-    version='1.3.1',
+    version='1.3.2',
     description='Convenient work with sqlite3 and aiosqlite',
     url='https://github.com/I-HedgeDev/litesqlite',
     author='HedgeDev',
     author_email='hedge_dev@mail.ru',
     packages=['hedgesql'],
     install_requires=[
         'aiosqlite'
```

