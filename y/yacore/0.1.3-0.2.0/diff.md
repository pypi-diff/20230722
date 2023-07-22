# Comparing `tmp/yacore-0.1.3.tar.gz` & `tmp/yacore-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yacore-0.1.3.tar", last modified: Sun Jan  8 11:19:14 2023, max compression
+gzip compressed data, was "yacore-0.2.0.tar", last modified: Sat Jul 22 21:32:51 2023, max compression
```

## Comparing `yacore-0.1.3.tar` & `yacore-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 11:19:14.272558 yacore-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-08 11:19:04.000000 yacore-0.1.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-01-08 11:19:04.000000 yacore-0.1.3/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-08 11:19:04.000000 yacore-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-01-08 11:19:14.272558 yacore-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-01-08 11:19:04.000000 yacore-0.1.3/history.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-01-08 11:19:04.000000 yacore-0.1.3/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-01-08 11:19:04.000000 yacore-0.1.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-01-08 11:19:04.000000 yacore-0.1.3/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-08 11:19:14.272558 yacore-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-01-08 11:19:04.000000 yacore-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 11:19:14.264558 yacore-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-01-08 11:19:04.000000 yacore-0.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-01-08 11:19:04.000000 yacore-0.1.3/tests/test_db_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-01-08 11:19:04.000000 yacore-0.1.3/tests/test_deepmerge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-01-08 11:19:04.000000 yacore-0.1.3/tests/test_executors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-01-08 11:19:04.000000 yacore-0.1.3/tests/test_net_http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 11:19:14.264558 yacore-0.1.3/yacore/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-01-08 11:19:04.000000 yacore-0.1.3/yacore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 11:19:14.268558 yacore-0.1.3/yacore/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 11:19:04.000000 yacore-0.1.3/yacore/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 11:19:14.268558 yacore-0.1.3/yacore/db/postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-08 11:19:04.000000 yacore-0.1.3/yacore/db/postgresql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-01-08 11:19:04.000000 yacore-0.1.3/yacore/db/postgresql/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-01-08 11:19:04.000000 yacore-0.1.3/yacore/db/postgresql/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-01-08 11:19:04.000000 yacore-0.1.3/yacore/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-08 11:19:04.000000 yacore-0.1.3/yacore/injector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 11:19:14.268558 yacore-0.1.3/yacore/log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 11:19:04.000000 yacore-0.1.3/yacore/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-01-08 11:19:04.000000 yacore-0.1.3/yacore/log/loguru.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-01-08 11:19:04.000000 yacore-0.1.3/yacore/log/stdlib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 11:19:14.268558 yacore-0.1.3/yacore/net/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 11:19:04.000000 yacore-0.1.3/yacore/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 11:19:14.272558 yacore-0.1.3/yacore/net/http/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-08 11:19:04.000000 yacore-0.1.3/yacore/net/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-01-08 11:19:04.000000 yacore-0.1.3/yacore/net/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-01-08 11:19:04.000000 yacore-0.1.3/yacore/net/http/server.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-08 11:19:04.000000 yacore-0.1.3/yacore/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 11:19:14.268558 yacore-0.1.3/yacore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-01-08 11:19:14.000000 yacore-0.1.3/yacore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-01-08 11:19:14.000000 yacore-0.1.3/yacore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-08 11:19:14.000000 yacore-0.1.3/yacore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-08 11:19:14.000000 yacore-0.1.3/yacore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-01-08 11:19:14.000000 yacore-0.1.3/yacore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-08 11:19:14.000000 yacore-0.1.3/yacore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:32:51.487054 yacore-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-22 21:32:35.000000 yacore-0.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-22 21:32:35.000000 yacore-0.2.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-22 21:32:35.000000 yacore-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-22 21:32:51.487054 yacore-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-22 21:32:35.000000 yacore-0.2.0/history.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-22 21:32:35.000000 yacore-0.2.0/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-22 21:32:35.000000 yacore-0.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-22 21:32:35.000000 yacore-0.2.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 21:32:51.487054 yacore-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-22 21:32:35.000000 yacore-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:32:51.487054 yacore-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-22 21:32:35.000000 yacore-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-07-22 21:32:35.000000 yacore-0.2.0/tests/test_db_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-22 21:32:35.000000 yacore-0.2.0/tests/test_deepmerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-22 21:32:35.000000 yacore-0.2.0/tests/test_executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-22 21:32:35.000000 yacore-0.2.0/tests/test_net_http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:32:51.487054 yacore-0.2.0/yacore/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-22 21:32:35.000000 yacore-0.2.0/yacore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:32:51.487054 yacore-0.2.0/yacore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 21:32:35.000000 yacore-0.2.0/yacore/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:32:51.487054 yacore-0.2.0/yacore/db/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-22 21:32:35.000000 yacore-0.2.0/yacore/db/postgresql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-22 21:32:35.000000 yacore-0.2.0/yacore/db/postgresql/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-07-22 21:32:35.000000 yacore-0.2.0/yacore/db/postgresql/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-22 21:32:35.000000 yacore-0.2.0/yacore/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-22 21:32:35.000000 yacore-0.2.0/yacore/injector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:32:51.487054 yacore-0.2.0/yacore/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 21:32:35.000000 yacore-0.2.0/yacore/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-22 21:32:35.000000 yacore-0.2.0/yacore/log/loguru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-22 21:32:35.000000 yacore-0.2.0/yacore/log/stdlib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:32:51.487054 yacore-0.2.0/yacore/net/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 21:32:35.000000 yacore-0.2.0/yacore/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:32:51.487054 yacore-0.2.0/yacore/net/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-22 21:32:35.000000 yacore-0.2.0/yacore/net/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-22 21:32:35.000000 yacore-0.2.0/yacore/net/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-22 21:32:35.000000 yacore-0.2.0/yacore/net/http/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 21:32:35.000000 yacore-0.2.0/yacore/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:32:51.487054 yacore-0.2.0/yacore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-22 21:32:51.000000 yacore-0.2.0/yacore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-22 21:32:51.000000 yacore-0.2.0/yacore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 21:32:51.000000 yacore-0.2.0/yacore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-22 21:32:51.000000 yacore-0.2.0/yacore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-22 21:32:51.000000 yacore-0.2.0/yacore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-22 21:32:51.000000 yacore-0.2.0/yacore.egg-info/top_level.txt
```

### Comparing `yacore-0.1.3/PKG-INFO` & `yacore-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: yacore
-Version: 0.1.3
+Version: 0.2.0
 Summary: yet another core library
 Home-page: https://github.com/pohmelie/yacore
 Author: pohmelie
 Author-email: multisosnooley@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >= 3.9
+Requires-Python: >= 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: db.postgresql
 Provides-Extra: log.loguru
 Provides-Extra: log.std
 Provides-Extra: net.http
 License-File: license.txt
```

### Comparing `yacore-0.1.3/license.txt` & `yacore-0.2.0/license.txt`

 * *Files identical despite different names*

### Comparing `yacore-0.1.3/readme.md` & `yacore-0.2.0/readme.md`

 * *Files identical despite different names*

### Comparing `yacore-0.1.3/setup.py` & `yacore-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 PACKAGE_ROOT = Path(__file__).parent
 VERSION = PACKAGE_ROOT / "yacore" / "version.txt"
 
 
 extras_require = {
-    "dev": ["flake8", "pytest", "pytest-asyncio", "pytest-cov", "testcontainers"],
+    "dev": ["ruff", "pytest", "pytest-asyncio", "pytest-cov", "testcontainers"],
     "db.postgresql": ["asyncpg", "yarl"],
     "log.loguru": ["loguru"],
     "log.std": ["pyyaml"],
     "net.http": ["async-timeout", "fastapi >= 0.89.0", "httpx", "hypercorn", "yarl"],
 }
 
 extras_dev = set()
@@ -23,15 +23,15 @@
 setup(
     name="yacore",
     version=VERSION.read_text().strip(),
     packages=find_packages(include=["yacore*"]),
     package_data={
         "": ["*.txt"],
     },
-    python_requires=">= 3.9",
+    python_requires=">= 3.11",
     install_requires=[
         "cock >= 0.11.0",
         "facet >= 0.9.1",
         "giveme",
     ],
     extras_require=extras_require,
     entry_points={
```

### Comparing `yacore-0.1.3/tests/conftest.py` & `yacore-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `yacore-0.1.3/tests/test_db_postgresql.py` & `yacore-0.2.0/tests/test_db_postgresql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import time
-from typing import List, Optional
 from unittest.mock import AsyncMock, patch
 
 import pytest
 
-from yacore.db.postgresql.postgresql import (DbPostgresql, DatabaseMigrator, Migration,
-                                             MigrationError, db_postgresql_from_config,
-                                             migrate_using_config)
+from yacore.db.postgresql.postgresql import (
+    DatabaseMigrator,
+    DbPostgresql,
+    Migration,
+    MigrationError,
+    db_postgresql_from_config,
+    migrate_using_config,
+)
 
 
 @pytest.mark.asyncio
 async def test_database_connection(database):
     async with database.get_connection() as conn:
         await conn.execute("CREATE TABLE test ()")
         await conn.execute("DROP TABLE test")
@@ -46,15 +50,15 @@
         db_postgresql_from_config()
 
     core_config["db_postgresql_database"] = database_name
     database = db_postgresql_from_config()
     assert str(database.url) == "postgresql://user:password@some_host:2345/some_database"
 
 
-async def case(database, current: Optional[str], target: Optional[str], expected: str, expected_calls: List[int]):
+async def case(database, current: str | None, target: str | None, expected: str, expected_calls: list[int]):
     calls = []
     migrations = [
         Migration("002", "001", AsyncMock(side_effect=lambda _: calls.append(2))),
         Migration("001", None, AsyncMock(side_effect=lambda _: calls.append(1))),
         Migration("003", "002", AsyncMock(side_effect=lambda _: calls.append(3))),
     ]
     if current is not None:
```

### Comparing `yacore-0.1.3/tests/test_deepmerge.py` & `yacore-0.2.0/tests/test_deepmerge.py`

 * *Files identical despite different names*

### Comparing `yacore-0.1.3/tests/test_executors.py` & `yacore-0.2.0/tests/test_executors.py`

 * *Files identical despite different names*

### Comparing `yacore-0.1.3/tests/test_net_http.py` & `yacore-0.2.0/tests/test_net_http.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,19 +39,23 @@
 async def test_handler_validation_error(web_client, web_server: NetHttpServer):
     web_server.add_post("/handle", handler)
 
     response = await web_client.post("handle")
     assert response.status_code == 422
     data = response.json()
     assert data["code"] == "common.validation_error"
-    assert data["data"] == [{
+    data = data["data"]
+    assert len(data) == 1
+    expected = {
         "loc": ["body", "value"],
-        "msg": "field required",
-        "type": "value_error.missing",
-    }]
+        "msg": "Field required",
+        "type": "missing",
+    }
+    for k, v in expected.items():
+        assert data[0][k] == v
 
 
 @pytest.mark.asyncio
 async def test_handler_error(web_client, web_server: NetHttpServer):
     web_server.add_post("/handle", handler)
 
     response = await web_client.post("handle", json={"value": "error"})
```

### Comparing `yacore-0.1.3/yacore/db/postgresql/fixtures.py` & `yacore-0.2.0/yacore/db/postgresql/fixtures.py`

 * *Files identical despite different names*

### Comparing `yacore-0.1.3/yacore/db/postgresql/postgresql.py` & `yacore-0.2.0/yacore/db/postgresql/postgresql.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 import importlib
 import logging
 import time
+from collections.abc import Callable, Coroutine
 from dataclasses import dataclass
 from importlib import resources
-from typing import Any, Callable, Coroutine, Dict, List, Optional, Set
+from typing import Any
 
 import asyncpg
 from asyncpg import Connection
 from asyncpg.pool import Pool, PoolAcquireContext
 from cock import Option, build_options_from_dict
 from facet import ServiceMixin
 from yarl import URL
@@ -46,15 +47,15 @@
                  pool_min_size: int = 2, pool_max_size: int = 10):
         self._url = connection_url.with_scheme("postgresql")
         self._attempts = conn_attempts
         self._interval = conn_interval
         self._pool_min_size = pool_min_size
         self._pool_max_size = pool_max_size
 
-        self._pool: Optional[Pool] = None
+        self._pool: Pool | None = None
 
     async def start(self):
         for _ in range(self._attempts):
             start = time.monotonic()
             try:
                 self._pool = await self._create_pool()
             except (OSError,
@@ -71,15 +72,16 @@
                 logger.debug("Successfully connected to database")
                 break
         else:
             raise RuntimeError("Can't connect to db, attempts gone")
 
     async def _create_pool(self) -> Pool:
         return await asyncpg.create_pool(
-            dsn=str(self._url), min_size=self._pool_min_size, max_size=self._pool_max_size
+            dsn=str(self._url), min_size=self._pool_min_size, max_size=self._pool_max_size,
+            timeout=self._interval
         )
 
     async def stop(self):
         await self._pool.close()
         self._pool = None
 
     def get_connection(self) -> PoolAcquireContext:
@@ -94,15 +96,15 @@
         return self._pool
 
     async def clear_schema(self):
         async with self.get_connection() as conn:
             await conn.execute("DROP SCHEMA public CASCADE")
             await conn.execute("CREATE SCHEMA public")
 
-    async def migrate(self, migration_script_location: str, migration_target_revision: Optional[str] = None):
+    async def migrate(self, migration_script_location: str, migration_target_revision: str | None = None):
         migrator = DatabaseMigrator(migration_script_location)
         async with self.get_connection() as conn:
             await migrator.migrate(conn, target=migration_target_revision)
 
 
 @register(name="db_postgresql", singleton=True)
 @inject
@@ -124,15 +126,15 @@
         pool_max_size=config.db_postgresql_pool_max_size,
     )
 
 
 @dataclass(frozen=True)
 class Migration:
     revision: str
-    depends_on: Optional[str]
+    depends_on: str | None
     migrate: Callable[[Connection], Coroutine]
 
     @classmethod
     def from_module(cls, module: Any):
         return cls(module.revision, module.depends_on, module.migrate)
 
 
@@ -140,15 +142,15 @@
     pass
 
 
 class DatabaseMigrator:
     def __init__(self, script_location: str):
         self._script_location = script_location
 
-    async def migrate(self, conn: Connection, *, target: Optional[str] = None):
+    async def migrate(self, conn: Connection, *, target: str | None = None):
         migrations = self.collect_migrations()
 
         await conn.execute("CREATE TABLE IF NOT EXISTS revision (id TEXT PRIMARY KEY)")
         current = await conn.fetchval("SELECT id FROM revision")
 
         target_text = target or "<head>"
         current_text = current or "<empty>"
@@ -176,18 +178,18 @@
                     break
 
             q = "UPDATE revision SET id = $1" if current else "INSERT INTO revision VALUES ($1)"
             await conn.execute(q, migration.revision)
 
         logger.info("Database is migrated to %s", migration.revision)
 
-    def collect_migrations(self) -> List[Migration]:
-        collected_revs: Set[str] = set()
-        prerequisites: Dict[Optional[str], Migration] = {}
-        result: List[Migration] = []
+    def collect_migrations(self) -> list[Migration]:
+        collected_revs: set[str] = set()
+        prerequisites: dict[str | None, Migration] = {}
+        result: list[Migration] = []
         for migration in self.load_modules():
             if migration.depends_on in prerequisites:
                 raise MigrationError(f"Multiple revisions depend on {migration.depends_on}")
             prerequisites[migration.depends_on] = migration
 
             if migration.revision in collected_revs:
                 raise MigrationError(f"Found multiple revisions {migration.revision}")
@@ -203,15 +205,15 @@
             dependent_rev = prerequisites.pop(last_rev, None)
             if dependent_rev is None:
                 raise MigrationError(f"Migration chain is broken after {last_rev}")
             result.append(dependent_rev)
 
         return result
 
-    def load_modules(self) -> List[Migration]:
+    def load_modules(self) -> list[Migration]:
         result = []
         for path in resources.files(self._script_location).iterdir():
             if path.suffix == ".py" and path.stem != "__init__":
                 module = importlib.import_module(f"{self._script_location}.{path.stem}")
                 result.append(Migration.from_module(module))
         return result
```

### Comparing `yacore-0.1.3/yacore/executors.py` & `yacore-0.2.0/yacore/executors.py`

 * *Files identical despite different names*

### Comparing `yacore-0.1.3/yacore/log/loguru.py` & `yacore-0.2.0/yacore/log/loguru.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import logging
 import sys
 
-from cock import Option, build_options_from_dict
 from click import Choice
+from cock import Option, build_options_from_dict
 from loguru import logger
 
 from yacore.injector import inject
 
 log_options = build_options_from_dict({
     "log-level": Option(default="debug", type=Choice(["debug", "info", "warning", "error"])),
 })
 
 
 class InterceptHandler(logging.Handler):
     def emit(self, record):
-        # Get corresponding Loguru level if it exists
+        # Get corresponding Loguru level if it exists.
         try:
             level = logger.level(record.levelname).name
         except ValueError:
             level = record.levelno
 
-        # Find caller from where originated the logged message
-        frame, depth = logging.currentframe(), 2
-        while frame.f_code.co_filename == logging.__file__:
+        # Find caller from where originated the logged message.
+        frame, depth = sys._getframe(6), 6
+        while frame and frame.f_code.co_filename == logging.__file__:
             frame = frame.f_back
             depth += 1
 
         logger.opt(depth=depth, exception=record.exc_info).log(level, record.getMessage())
 
 
 def configure_logging(log_level):
@@ -35,13 +35,13 @@
             dict(
                 sink=sys.stderr,
                 # format="{time} {level:<8} {message}",
                 level=log_level.upper(),
             ),
         ],
     )
-    logging.basicConfig(handlers=[InterceptHandler()], level=0)
+    logging.basicConfig(handlers=[InterceptHandler()], level=0, force=True)
 
 
 @inject
 def configure_logging_from_config(config):
     configure_logging(config.log_level)
```

### Comparing `yacore-0.1.3/yacore/log/stdlib.py` & `yacore-0.2.0/yacore/log/stdlib.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import collections
 import copy
 import itertools
 import logging
 import logging.config
 from pathlib import Path
 
-from click import Choice, Path as ClickPath
-from cock import Option, build_options_from_dict
 import yaml
+from click import Choice
+from click import Path as ClickPath
+from cock import Option, build_options_from_dict
 
 from yacore.injector import inject
 
 log_options = build_options_from_dict({
     "log-level": Option(default="debug", type=Choice(["debug", "info", "warning", "error"])),
     "log-config": Option(default=None, type=ClickPath(exists=True, dir_okay=False))
 })
@@ -39,20 +40,20 @@
     elif isinstance(source, collections.abc.Set):
         if isinstance(target, collections.abc.MutableSet):
             target |= source
         elif isinstance(target, collections.abc.Set):
             return target | source
         else:
             return copy.deepcopy(source)
-    elif not isinstance(source, (str, collections.abc.ByteString)) and \
+    elif not isinstance(source, str | collections.abc.ByteString) and \
             isinstance(source, collections.abc.Sequence):
         if isinstance(target, collections.abc.MutableSequence):
             for v in source:
                 target.append(v)
-        elif not isinstance(target, (str, collections.abc.ByteString)) and \
+        elif not isinstance(target, str | collections.abc.ByteString) and \
                 isinstance(target, collections.abc.Sequence):
             return tuple(itertools.chain(target, source))
         else:
             return copy.deepcopy(source)
     elif source is not None or allow_none:
         return source
```

### Comparing `yacore-0.1.3/yacore/net/http/client.py` & `yacore-0.2.0/yacore/net/http/client.py`

 * *Files identical despite different names*

### Comparing `yacore-0.1.3/yacore/net/http/server.py` & `yacore-0.2.0/yacore/net/http/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncio
-from typing import Any, Optional
+from typing import Any
 
 from cock import Option, build_options_from_dict
 from facet import ServiceMixin
 from fastapi import FastAPI
 from fastapi.exceptions import RequestValidationError
 from fastapi.responses import JSONResponse
 from hypercorn.asyncio import serve
@@ -30,15 +30,15 @@
 class HealthCheck(BaseModel):
     ok: bool
     name: str
     version: str
     build_info: str
 
 
-def _api_error(status_code: int, code: str, message: Optional[str] = None, data: Optional[Any] = None):
+def _api_error(status_code: int, code: str, message: str | None = None, data: Any | None = None):
     return JSONResponse(
         status_code=status_code,
         content={
             "code": code,
             "message": message,
             "data": data,
         },
```

### Comparing `yacore-0.1.3/yacore.egg-info/PKG-INFO` & `yacore-0.2.0/yacore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: yacore
-Version: 0.1.3
+Version: 0.2.0
 Summary: yet another core library
 Home-page: https://github.com/pohmelie/yacore
 Author: pohmelie
 Author-email: multisosnooley@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >= 3.9
+Requires-Python: >= 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: db.postgresql
 Provides-Extra: log.loguru
 Provides-Extra: log.std
 Provides-Extra: net.http
 License-File: license.txt
```

### Comparing `yacore-0.1.3/yacore.egg-info/SOURCES.txt` & `yacore-0.2.0/yacore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

