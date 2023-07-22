# Comparing `tmp/PyEasySQL-3.0.2.tar.gz` & `tmp/PyEasySQL-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEasySQL-3.0.2.tar", last modified: Wed Jul 12 13:10:09 2023, max compression
+gzip compressed data, was "PyEasySQL-3.0.3.tar", last modified: Sat Jul 22 15:24:08 2023, max compression
```

## Comparing `PyEasySQL-3.0.2.tar` & `PyEasySQL-3.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 13:10:09.478943 PyEasySQL-3.0.2/
-drwxrwxrwx   0        0        0        0 2023-07-12 13:10:09.450027 PyEasySQL-3.0.2/EasySQL/
--rw-rw-rw-   0        0        0     3452 2023-07-09 09:35:55.000000 PyEasySQL-3.0.2/EasySQL/ABC.py
--rw-rw-rw-   0        0        0     2887 2021-06-27 12:24:21.000000 PyEasySQL-3.0.2/EasySQL/Characters.py
--rw-rw-rw-   0        0        0    14208 2023-07-11 13:02:37.000000 PyEasySQL-3.0.2/EasySQL/Classes.py
--rw-rw-rw-   0        0        0     5655 2022-06-25 11:35:34.000000 PyEasySQL-3.0.2/EasySQL/Commands.py
--rw-rw-rw-   0        0        0      305 2023-07-11 12:44:34.000000 PyEasySQL-3.0.2/EasySQL/Decorators.py
--rw-rw-rw-   0        0        0     2097 2023-07-09 09:35:55.000000 PyEasySQL-3.0.2/EasySQL/EasyInstances.py
--rw-rw-rw-   0        0        0      757 2023-06-08 19:41:42.000000 PyEasySQL-3.0.2/EasySQL/Exceptions.py
--rw-rw-rw-   0        0        0      457 2021-04-04 16:17:30.000000 PyEasySQL-3.0.2/EasySQL/Logging.py
--rw-rw-rw-   0        0        0      134 2023-07-09 09:35:55.000000 PyEasySQL-3.0.2/EasySQL/Tags.py
--rw-rw-rw-   0        0        0     2602 2023-07-11 12:55:43.000000 PyEasySQL-3.0.2/EasySQL/Types.py
--rw-rw-rw-   0        0        0     2496 2022-04-15 06:15:51.000000 PyEasySQL-3.0.2/EasySQL/Where.py
--rw-rw-rw-   0        0        0      290 2023-07-09 11:50:43.000000 PyEasySQL-3.0.2/EasySQL/__init__.py
--rw-rw-rw-   0        0        0     6499 2023-07-12 13:10:09.477280 PyEasySQL-3.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 13:10:09.469844 PyEasySQL-3.0.2/PyEasySQL.egg-info/
--rw-rw-rw-   0        0        0     6499 2023-07-12 13:10:08.000000 PyEasySQL-3.0.2/PyEasySQL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-07-12 13:10:08.000000 PyEasySQL-3.0.2/PyEasySQL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 13:10:08.000000 PyEasySQL-3.0.2/PyEasySQL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-12 13:10:08.000000 PyEasySQL-3.0.2/PyEasySQL.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-12 13:10:08.000000 PyEasySQL-3.0.2/PyEasySQL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5119 2023-07-09 10:37:27.000000 PyEasySQL-3.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-12 13:10:09.479462 PyEasySQL-3.0.2/setup.cfg
--rw-rw-rw-   0        0        0      859 2023-07-11 12:35:42.000000 PyEasySQL-3.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 15:24:08.038012 PyEasySQL-3.0.3/
+drwxrwxrwx   0        0        0        0 2023-07-22 15:24:08.018067 PyEasySQL-3.0.3/EasySQL/
+-rw-rw-rw-   0        0        0     3452 2023-07-09 09:35:55.000000 PyEasySQL-3.0.3/EasySQL/ABC.py
+-rw-rw-rw-   0        0        0     2887 2021-06-27 12:24:21.000000 PyEasySQL-3.0.3/EasySQL/Characters.py
+-rw-rw-rw-   0        0        0    14303 2023-07-22 14:35:27.000000 PyEasySQL-3.0.3/EasySQL/Classes.py
+-rw-rw-rw-   0        0        0     5764 2023-07-18 13:18:56.000000 PyEasySQL-3.0.3/EasySQL/Commands.py
+-rw-rw-rw-   0        0        0      305 2023-07-11 12:44:34.000000 PyEasySQL-3.0.3/EasySQL/Decorators.py
+-rw-rw-rw-   0        0        0     2097 2023-07-09 09:35:55.000000 PyEasySQL-3.0.3/EasySQL/EasyInstances.py
+-rw-rw-rw-   0        0        0      757 2023-06-08 19:41:42.000000 PyEasySQL-3.0.3/EasySQL/Exceptions.py
+-rw-rw-rw-   0        0        0      457 2021-04-04 16:17:30.000000 PyEasySQL-3.0.3/EasySQL/Logging.py
+-rw-rw-rw-   0        0        0      134 2023-07-09 09:35:55.000000 PyEasySQL-3.0.3/EasySQL/Tags.py
+-rw-rw-rw-   0        0        0     2602 2023-07-11 12:55:43.000000 PyEasySQL-3.0.3/EasySQL/Types.py
+-rw-rw-rw-   0        0        0     2496 2022-04-15 06:15:51.000000 PyEasySQL-3.0.3/EasySQL/Where.py
+-rw-rw-rw-   0        0        0      290 2023-07-09 11:50:43.000000 PyEasySQL-3.0.3/EasySQL/__init__.py
+-rw-rw-rw-   0        0        0     6499 2023-07-22 15:24:08.037017 PyEasySQL-3.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-22 15:24:08.033026 PyEasySQL-3.0.3/PyEasySQL.egg-info/
+-rw-rw-rw-   0        0        0     6499 2023-07-22 15:24:05.000000 PyEasySQL-3.0.3/PyEasySQL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-07-22 15:24:05.000000 PyEasySQL-3.0.3/PyEasySQL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 15:24:05.000000 PyEasySQL-3.0.3/PyEasySQL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-22 15:24:05.000000 PyEasySQL-3.0.3/PyEasySQL.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-22 15:24:05.000000 PyEasySQL-3.0.3/PyEasySQL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5119 2023-07-09 10:37:27.000000 PyEasySQL-3.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-22 15:24:08.038012 PyEasySQL-3.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      859 2023-07-22 14:35:27.000000 PyEasySQL-3.0.3/setup.py
```

### Comparing `PyEasySQL-3.0.2/EasySQL/ABC.py` & `PyEasySQL-3.0.3/EasySQL/ABC.py`

 * *Files identical despite different names*

### Comparing `PyEasySQL-3.0.2/EasySQL/Characters.py` & `PyEasySQL-3.0.3/EasySQL/Characters.py`

 * *Files identical despite different names*

### Comparing `PyEasySQL-3.0.2/EasySQL/Classes.py` & `PyEasySQL-3.0.3/EasySQL/Classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 class EasyForeignColumn(EasyColumn):
     @staticmethod
     def of(column: EasyColumn, name: str = None, *tags: SQLTag, default: Any = None):
         if not isinstance(column.table, EasyTable):
             return TypeError('Version 3: To use this method, The table of column must be set')
 
         tags = (NOT_NULL, ) if NOT_NULL in tags else ()
-        name = f'{column.name} of {column.table}' if name is None else name
+        name = f'{column.name} of {column.table.name}' if name is None else name
         return EasyForeignColumn(name, column.table, column, *tags, default=default)
 
     def __init__(self, name: str, table: 'EasyTable', reference: Union[EasyColumn, str], *tags: SQLTag, default: Any = None):
         column = table.get_column(reference)
         if column is None:
             raise ValueError(f'Unable to find `{reference}` in the table')
 
@@ -365,11 +365,11 @@
         from .Commands import Delete
 
         assert self.prepared, 'Unable to perform action before preparing the table'
         return Delete(self._database, self, where).execute()
 
     def set(self, columns: SOS_ECOS, values: SOS[Any], where: Where = None):
         selection = self.select(columns, where)
-        if selection:
+        if selection is not None and len(selection) > 0:
             self.update(columns, values, where)
         else:
-            self.insert(columns, values)
+            self.insert(self.columns if columns is None or columns == '*' else columns, values)
```

### Comparing `PyEasySQL-3.0.2/EasySQL/Commands.py` & `PyEasySQL-3.0.3/EasySQL/Commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,26 +26,32 @@
             raise ValueError(f'Unable to find `{column}` in data')
 
         return self._data[col]
 
     def __iter__(self):
         return iter([self])
 
+    def __len__(self):
+        return len(self._data.keys())
+
     @property
     def data(self):
         return self._data.copy()
 
 
 class EmptySelectData(SelectData):
     def __init__(self, table: EasyTable):
         super().__init__(table, [], [])
 
     def __iter__(self):
         return iter([])
 
+    def __len__(self):
+        return 0
+
     def __repr__(self):
         return f'<EmptySelectData source="{self._table.name}">'
 
 
 class Select(SQLCommandExecutable):
     def __init__(self, database: EasyDatabase, table: EasyTable = None, columns: Sequence[EasyColumn] = None, where: Where = None, limit: int = None, offset: int = None, order: Iterable[EasyColumn] = None, descending: bool = False, force_one: bool = False):
         self._database = database
```

### Comparing `PyEasySQL-3.0.2/EasySQL/EasyInstances.py` & `PyEasySQL-3.0.3/EasySQL/EasyInstances.py`

 * *Files identical despite different names*

### Comparing `PyEasySQL-3.0.2/EasySQL/Exceptions.py` & `PyEasySQL-3.0.3/EasySQL/Exceptions.py`

 * *Files identical despite different names*

### Comparing `PyEasySQL-3.0.2/EasySQL/Types.py` & `PyEasySQL-3.0.3/EasySQL/Types.py`

 * *Files identical despite different names*

### Comparing `PyEasySQL-3.0.2/EasySQL/Where.py` & `PyEasySQL-3.0.3/EasySQL/Where.py`

 * *Files identical despite different names*

### Comparing `PyEasySQL-3.0.2/PKG-INFO` & `PyEasySQL-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyEasySQL
-Version: 3.0.2
+Version: 3.0.3
 Summary: SQL Database management without even a SQL line
 Home-page: https://github.com/ashenguard/easysql
 Author: Ashenguard
 Author-email: Ashenguard@agmdev.xyz
 License: MIT License
 Description: # EasySQL
         ![Downloads](https://pepy.tech/badge/pyeasysql)
```

### Comparing `PyEasySQL-3.0.2/PyEasySQL.egg-info/PKG-INFO` & `PyEasySQL-3.0.3/PyEasySQL.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyEasySQL
-Version: 3.0.2
+Version: 3.0.3
 Summary: SQL Database management without even a SQL line
 Home-page: https://github.com/ashenguard/easysql
 Author: Ashenguard
 Author-email: Ashenguard@agmdev.xyz
 License: MIT License
 Description: # EasySQL
         ![Downloads](https://pepy.tech/badge/pyeasysql)
```

### Comparing `PyEasySQL-3.0.2/README.md` & `PyEasySQL-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `PyEasySQL-3.0.2/setup.py` & `PyEasySQL-3.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyEasySQL",
-    version="3.0.2",
+    version="3.0.3",
     license='MIT License',
     author="Ashenguard",
     author_email="Ashenguard@agmdev.xyz",
     description="SQL Database management without even a SQL line",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ashenguard/easysql",
```

