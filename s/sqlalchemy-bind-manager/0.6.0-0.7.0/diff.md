# Comparing `tmp/sqlalchemy_bind_manager-0.6.0.tar.gz` & `tmp/sqlalchemy_bind_manager-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_bind_manager-0.6.0.tar", max compression
+gzip compressed data, was "sqlalchemy_bind_manager-0.7.0.tar", max compression
```

## Comparing `sqlalchemy_bind_manager-0.6.0.tar` & `sqlalchemy_bind_manager-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1073 2023-07-08 11:01:18.572363 sqlalchemy_bind_manager-0.6.0/LICENSE
--rw-r--r--   0        0        0     8778 2023-07-08 11:01:18.572363 sqlalchemy_bind_manager-0.6.0/README.md
--rw-r--r--   0        0        0     2375 2023-07-08 11:01:31.344604 sqlalchemy_bind_manager-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      107 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/__init__.py
--rw-r--r--   0        0        0     5241 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_bind_manager.py
--rw-r--r--   0        0        0      197 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/__init__.py
--rw-r--r--   0        0        0     6080 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/async_.py
--rw-r--r--   0        0        0    11340 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/base_repository.py
--rw-r--r--   0        0        0     1099 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/common.py
--rw-r--r--   0        0        0     7429 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/result_presenters.py
--rw-r--r--   0        0        0     5376 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/sync.py
--rw-r--r--   0        0        0     3118 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_session_handler.py
--rw-r--r--   0        0        0     2507 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_unit_of_work/__init__.py
--rw-r--r--   0        0        0      358 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/exceptions.py
--rw-r--r--   0        0        0    11155 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/protocols.py
--rw-r--r--   0        0        0        0 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/py.typed
--rw-r--r--   0        0        0      242 2023-07-08 11:01:18.576363 sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/repository.py
--rw-r--r--   0        0        0    10171 1970-01-01 00:00:00.000000 sqlalchemy_bind_manager-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-22 13:57:50.372797 sqlalchemy_bind_manager-0.7.0/LICENSE
+-rw-r--r--   0        0        0     8784 2023-07-22 13:57:50.372797 sqlalchemy_bind_manager-0.7.0/README.md
+-rw-r--r--   0        0        0     2375 2023-07-22 13:58:04.136861 sqlalchemy_bind_manager-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-07-22 13:57:50.372797 sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/__init__.py
+-rw-r--r--   0        0        0     5241 2023-07-22 13:57:50.372797 sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/_bind_manager.py
+-rw-r--r--   0        0        0      197 2023-07-22 13:57:50.372797 sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/_repository/__init__.py
+-rw-r--r--   0        0        0     6274 2023-07-22 13:57:50.372797 sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/_repository/async_.py
+-rw-r--r--   0        0        0    11569 2023-07-22 13:57:50.372797 sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/_repository/base_repository.py
+-rw-r--r--   0        0        0     1099 2023-07-22 13:57:50.372797 sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/_repository/common.py
+-rw-r--r--   0        0        0     7429 2023-07-22 13:57:50.372797 sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/_repository/result_presenters.py
+-rw-r--r--   0        0        0     5570 2023-07-22 13:57:50.372797 sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/_repository/sync.py
+-rw-r--r--   0        0        0     3118 2023-07-22 13:57:50.372797 sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/_session_handler.py
+-rw-r--r--   0        0        0     2507 2023-07-22 13:57:50.372797 sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/_unit_of_work/__init__.py
+-rw-r--r--   0        0        0      358 2023-07-22 13:57:50.372797 sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/exceptions.py
+-rw-r--r--   0        0        0    11155 2023-07-22 13:57:50.372797 sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/protocols.py
+-rw-r--r--   0        0        0        0 2023-07-22 13:57:50.372797 sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/py.typed
+-rw-r--r--   0        0        0      242 2023-07-22 13:57:50.372797 sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/repository.py
+-rw-r--r--   0        0        0    10177 1970-01-01 00:00:00.000000 sqlalchemy_bind_manager-0.7.0/PKG-INFO
```

### Comparing `sqlalchemy_bind_manager-0.6.0/LICENSE` & `sqlalchemy_bind_manager-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.6.0/README.md` & `sqlalchemy_bind_manager-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 ```
 
 This will make sure we have an `AsyncEngine` and an `AsyncSession` are initialised, as an asynchronous context manager.
 
 ```python
 async with sa_manager.get_session() as session:
     session.add(o)
-    session.commit()
+    await session.commit()
 ```
 
 Note that async implementation has several differences from the sync one, make sure
 to check [SQLAlchemy asyncio documentation](https://docs.sqlalchemy.org/en/20/orm/extensions/asyncio.html)
 
 ## Repository / Unit of work
```

### Comparing `sqlalchemy_bind_manager-0.6.0/pyproject.toml` & `sqlalchemy_bind_manager-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlalchemy-bind-manager"
-version = "0.6.0"
+version = "0.7.0"
 description = "A manager to easily handle multiple SQLAlchemy configurations"
 license = "MIT"
 authors = ["Federico Busetti <729029+febus982@users.noreply.github.com>"]
 repository = "https://github.com/febus982/sqlalchemy-bind-manager"
 homepage = "https://febus982.github.io/sqlalchemy-bind-manager"
 readme = "README.md"
 packages = [{include = "sqlalchemy_bind_manager"}]
```

### Comparing `sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_bind_manager.py` & `sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/_bind_manager.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/async_.py` & `sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/_repository/async_.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,22 +62,24 @@
         if not self._external_session:
             async with self._session_handler.get_session(not commit) as _session:
                 yield _session
         else:
             yield self._external_session
 
     async def save(self, instance: MODEL) -> MODEL:
+        self._fail_if_invalid_models([instance])
         async with self._get_session() as session:
             session.add(instance)
         return instance
 
     async def save_many(
         self,
         instances: Iterable[MODEL],
     ) -> Iterable[MODEL]:
+        self._fail_if_invalid_models(instances)
         async with self._get_session() as session:
             session.add_all(instances)
         return instances
 
     async def get(self, identifier: PRIMARY_KEY) -> MODEL:
         async with self._get_session(commit=False) as session:
             model = await session.get(self._model, identifier)
@@ -90,18 +92,20 @@
             getattr(self._model, self._model_pk()).in_(identifiers)
         )
 
         async with self._get_session(commit=False) as session:
             return [x for x in (await session.execute(stmt)).scalars()]
 
     async def delete(self, instance: MODEL) -> None:
+        self._fail_if_invalid_models([instance])
         async with self._get_session() as session:
             await session.delete(instance)
 
     async def delete_many(self, instances: Iterable[MODEL]) -> None:
+        self._fail_if_invalid_models(instances)
         async with self._get_session() as session:
             for instance in instances:
                 await session.delete(instance)
 
     async def find(
         self,
         search_params: Union[None, Mapping[str, Any]] = None,
```

### Comparing `sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/base_repository.py` & `sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/_repository/base_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,7 +314,11 @@
         :return:
         """
         primary_keys = inspect(self._model).primary_key  # type: ignore
         if len(primary_keys) > 1:
             raise NotImplementedError("Composite primary keys are not supported.")
 
         return primary_keys[0].name
+
+    def _fail_if_invalid_models(self, objects: Iterable[MODEL]) -> None:
+        if [x for x in objects if not isinstance(x, self._model)]:
+            raise InvalidModel("Cannot handle models not belonging to this repository")
```

### Comparing `sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/common.py` & `sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/_repository/common.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/result_presenters.py` & `sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/_repository/result_presenters.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_repository/sync.py` & `sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/_repository/sync.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,19 +54,21 @@
         if not self._external_session:
             with self._session_handler.get_session(not commit) as _session:
                 yield _session
         else:
             yield self._external_session
 
     def save(self, instance: MODEL) -> MODEL:
+        self._fail_if_invalid_models([instance])
         with self._get_session() as session:
             session.add(instance)
         return instance
 
     def save_many(self, instances: Iterable[MODEL]) -> Iterable[MODEL]:
+        self._fail_if_invalid_models(instances)
         with self._get_session() as session:
             session.add_all(instances)
         return instances
 
     def get(self, identifier: PRIMARY_KEY) -> MODEL:
         with self._get_session(commit=False) as session:
             model = session.get(self._model, identifier)
@@ -79,18 +81,20 @@
             getattr(self._model, self._model_pk()).in_(identifiers)
         )
 
         with self._get_session(commit=False) as session:
             return [x for x in session.execute(stmt).scalars()]
 
     def delete(self, instance: MODEL) -> None:
+        self._fail_if_invalid_models([instance])
         with self._get_session() as session:
             session.delete(instance)
 
     def delete_many(self, instances: Iterable[MODEL]) -> None:
+        self._fail_if_invalid_models(instances)
         with self._get_session() as session:
             for model in instances:
                 session.delete(model)
 
     def find(
         self,
         search_params: Union[None, Mapping[str, Any]] = None,
```

### Comparing `sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_session_handler.py` & `sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/_session_handler.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/_unit_of_work/__init__.py` & `sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/_unit_of_work/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.6.0/sqlalchemy_bind_manager/protocols.py` & `sqlalchemy_bind_manager-0.7.0/sqlalchemy_bind_manager/protocols.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.6.0/PKG-INFO` & `sqlalchemy_bind_manager-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-bind-manager
-Version: 0.6.0
+Version: 0.7.0
 Summary: A manager to easily handle multiple SQLAlchemy configurations
 Home-page: https://febus982.github.io/sqlalchemy-bind-manager
 License: MIT
 Keywords: sqlalchemy,config,manager
 Author: Federico Busetti
 Author-email: 729029+febus982@users.noreply.github.com
 Requires-Python: >=3.8,<3.12
@@ -159,15 +159,15 @@
 ```
 
 This will make sure we have an `AsyncEngine` and an `AsyncSession` are initialised, as an asynchronous context manager.
 
 ```python
 async with sa_manager.get_session() as session:
     session.add(o)
-    session.commit()
+    await session.commit()
 ```
 
 Note that async implementation has several differences from the sync one, make sure
 to check [SQLAlchemy asyncio documentation](https://docs.sqlalchemy.org/en/20/orm/extensions/asyncio.html)
 
 ## Repository / Unit of work
```

