# Comparing `tmp/lassen-0.1.3.tar.gz` & `tmp/lassen-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lassen-0.1.3.tar", max compression
+gzip compressed data, was "lassen-0.2.0.tar", max compression
```

## Comparing `lassen-0.1.3.tar` & `lassen-0.2.0.tar`

### file list

```diff
@@ -1,53 +1,76 @@
--rw-r--r--   0        0        0     1071 2023-06-06 18:13:43.336753 lassen-0.1.3/LICENSE
--rw-r--r--   0        0        0     2781 2023-06-15 21:16:27.733755 lassen-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986429 lassen-0.1.3/lassen/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986933 lassen-0.1.3/lassen/alembic/__init__.py
--rw-r--r--   0        0        0     3685 2023-06-06 23:14:20.987092 lassen-0.1.3/lassen/alembic/cli.py
--rw-r--r--   0        0        0     3601 2023-06-06 23:14:20.987203 lassen-0.1.3/lassen/alembic/io.py
--rw-r--r--   0        0        0     1043 2023-06-06 23:14:20.987305 lassen-0.1.3/lassen/alembic/runner.py
--rw-r--r--   0        0        0      174 2023-06-06 23:14:20.987414 lassen-0.1.3/lassen/assets/__init__.py
--rw-r--r--   0        0        0     1592 2023-06-06 23:14:20.987525 lassen-0.1.3/lassen/assets/alembic.ini
--rw-r--r--   0        0        0      494 2023-06-06 23:14:20.987634 lassen-0.1.3/lassen/assets/script.py.mako
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.987697 lassen-0.1.3/lassen/core/__init__.py
--rw-r--r--   0        0        0      153 2023-06-15 21:16:27.734730 lassen-0.1.3/lassen/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2487 2023-06-15 21:16:27.734981 lassen-0.1.3/lassen/core/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0     1862 2023-06-06 23:14:20.988497 lassen-0.1.3/lassen/core/config.py
--rw-r--r--   0        0        0        0 2023-06-15 21:16:27.735020 lassen-0.1.3/lassen/datasets/__init__.py
--rw-r--r--   0        0        0     2368 2023-06-15 22:39:22.170659 lassen-0.1.3/lassen/datasets/dataset_helpers.py
--rw-r--r--   0        0        0     3024 2023-06-15 22:26:02.922940 lassen-0.1.3/lassen/datasets/pyarrow_schemas.py
--rw-r--r--   0        0        0      240 2023-06-06 23:14:20.988685 lassen-0.1.3/lassen/db/__init__.py
--rw-r--r--   0        0        0      396 2023-06-15 21:16:27.735607 lassen-0.1.3/lassen/db/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      139 2023-06-06 23:14:20.989157 lassen-0.1.3/lassen/db/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      147 2023-06-06 23:14:20.989285 lassen-0.1.3/lassen/db/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0      293 2023-06-06 23:14:20.989436 lassen-0.1.3/lassen/db/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     1931 2023-06-15 21:16:27.735885 lassen-0.1.3/lassen/db/__pycache__/base_class.cpython-310.pyc
--rw-r--r--   0        0        0     2727 2023-06-06 23:14:20.989823 lassen-0.1.3/lassen/db/__pycache__/base_class.cpython-311.pyc
--rw-r--r--   0        0        0      839 2023-06-15 21:16:27.736092 lassen-0.1.3/lassen/db/__pycache__/session.cpython-310.pyc
--rw-r--r--   0        0        0     1271 2023-06-06 23:14:20.990178 lassen-0.1.3/lassen/db/__pycache__/session.cpython-311.pyc
--rw-r--r--   0        0        0     1909 2023-06-06 23:14:20.990303 lassen-0.1.3/lassen/db/base_class.py
--rw-r--r--   0        0        0      627 2023-06-06 23:14:20.990409 lassen-0.1.3/lassen/db/session.py
--rw-r--r--   0        0        0      210 2023-06-06 23:14:20.990522 lassen-0.1.3/lassen/schema.py
--rw-r--r--   0        0        0      227 2023-06-15 21:16:27.736193 lassen-0.1.3/lassen/shared.py
--rw-r--r--   0        0        0     9983 2023-06-06 23:14:20.990676 lassen-0.1.3/lassen/store.py
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.990727 lassen-0.1.3/lassen/tests/__init__.py
--rw-r--r--   0        0        0      154 2023-06-15 21:16:27.736415 lassen-0.1.3/lassen/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1973 2023-06-15 21:31:07.938752 lassen-0.1.3/lassen/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1220 2023-06-06 23:14:20.991368 lassen-0.1.3/lassen/tests/__pycache__/fixtures.cpython-310.pyc
--rw-r--r--   0        0        0     5734 2023-06-15 21:16:27.736953 lassen-0.1.3/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1901 2023-06-15 21:16:27.737091 lassen-0.1.3/lassen/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-15 21:16:27.737128 lassen-0.1.3/lassen/tests/datasets/__init__.py
--rw-r--r--   0        0        0     2243 2023-06-15 22:42:38.547093 lassen-0.1.3/lassen/tests/datasets/test_dataset_helpers.py
--rw-r--r--   0        0        0     1645 2023-06-15 22:26:02.923228 lassen-0.1.3/lassen/tests/datasets/test_pyarrow_schemas.py
--rw-r--r--   0        0        0      176 2023-06-06 23:14:20.991801 lassen-0.1.3/lassen/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      463 2023-06-06 23:14:20.991923 lassen-0.1.3/lassen/tests/fixtures/test_harness/README.md
--rw-r--r--   0        0        0      311 2023-06-06 23:14:20.992056 lassen-0.1.3/lassen/tests/fixtures/test_harness/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.992112 lassen-0.1.3/lassen/tests/fixtures/test_harness/test_harness/__init__.py
--rw-r--r--   0        0        0      691 2023-06-06 23:14:20.992321 lassen-0.1.3/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py
--rw-r--r--   0        0        0      653 2023-06-06 23:14:20.992456 lassen-0.1.3/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py
--rw-r--r--   0        0        0      217 2023-06-06 23:14:20.992593 lassen-0.1.3/lassen/tests/fixtures/test_harness/test_harness/models.py
--rw-r--r--   0        0        0      461 2023-06-06 23:14:20.992727 lassen-0.1.3/lassen/tests/model_fixtures.py
--rw-r--r--   0        0        0     2252 2023-06-06 23:14:20.992858 lassen-0.1.3/lassen/tests/test_alembic.py
--rw-r--r--   0        0        0     2799 2023-06-06 23:14:20.992986 lassen-0.1.3/lassen/tests/test_store.py
--rw-r--r--   0        0        0     1325 2023-06-17 18:38:20.916738 lassen-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4347 1970-01-01 00:00:00.000000 lassen-0.1.3/setup.py
--rw-r--r--   0        0        0     3763 1970-01-01 00:00:00.000000 lassen-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-06 18:13:43.336753 lassen-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3159 2023-07-22 17:00:28.388296 lassen-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986429 lassen-0.2.0/lassen/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986933 lassen-0.2.0/lassen/alembic/__init__.py
+-rw-r--r--   0        0        0     3685 2023-06-06 23:14:20.987092 lassen-0.2.0/lassen/alembic/cli.py
+-rw-r--r--   0        0        0     2839 2023-07-22 17:00:28.388594 lassen-0.2.0/lassen/alembic/io.py
+-rw-r--r--   0        0        0     1043 2023-06-06 23:14:20.987305 lassen-0.2.0/lassen/alembic/runner.py
+-rw-r--r--   0        0        0      174 2023-06-06 23:14:20.987414 lassen-0.2.0/lassen/assets/__init__.py
+-rw-r--r--   0        0        0     1592 2023-06-06 23:14:20.987525 lassen-0.2.0/lassen/assets/alembic.ini
+-rw-r--r--   0        0        0      494 2023-06-06 23:14:20.987634 lassen-0.2.0/lassen/assets/script.py.mako
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.987697 lassen-0.2.0/lassen/core/__init__.py
+-rw-r--r--   0        0        0      153 2023-06-15 21:16:27.734730 lassen-0.2.0/lassen/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2487 2023-06-15 21:16:27.734981 lassen-0.2.0/lassen/core/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0        0        0     1862 2023-06-06 23:14:20.988497 lassen-0.2.0/lassen/core/config.py
+-rw-r--r--   0        0        0        0 2023-06-15 21:16:27.735020 lassen-0.2.0/lassen/datasets/__init__.py
+-rw-r--r--   0        0        0     2368 2023-06-15 22:39:22.170659 lassen-0.2.0/lassen/datasets/dataset_helpers.py
+-rw-r--r--   0        0        0     3024 2023-06-15 22:26:02.922940 lassen-0.2.0/lassen/datasets/pyarrow_schemas.py
+-rw-r--r--   0        0        0      240 2023-06-06 23:14:20.988685 lassen-0.2.0/lassen/db/__init__.py
+-rw-r--r--   0        0        0      396 2023-06-15 21:16:27.735607 lassen-0.2.0/lassen/db/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      422 2023-07-22 17:00:28.388869 lassen-0.2.0/lassen/db/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      147 2023-06-06 23:14:20.989285 lassen-0.2.0/lassen/db/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0      293 2023-06-06 23:14:20.989436 lassen-0.2.0/lassen/db/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1931 2023-06-15 21:16:27.735885 lassen-0.2.0/lassen/db/__pycache__/base_class.cpython-310.pyc
+-rw-r--r--   0        0        0     2976 2023-07-22 17:00:28.389221 lassen-0.2.0/lassen/db/__pycache__/base_class.cpython-311.pyc
+-rw-r--r--   0        0        0      839 2023-06-15 21:16:27.736092 lassen-0.2.0/lassen/db/__pycache__/session.cpython-310.pyc
+-rw-r--r--   0        0        0     1296 2023-07-22 17:00:28.389524 lassen-0.2.0/lassen/db/__pycache__/session.cpython-311.pyc
+-rw-r--r--   0        0        0     1920 2023-07-22 17:00:28.389828 lassen-0.2.0/lassen/db/base_class.py
+-rw-r--r--   0        0        0      627 2023-06-06 23:14:20.990409 lassen-0.2.0/lassen/db/session.py
+-rw-r--r--   0        0        0     1272 2023-07-22 17:00:28.389917 lassen-0.2.0/lassen/io.py
+-rw-r--r--   0        0        0      210 2023-06-06 23:14:20.990522 lassen-0.2.0/lassen/schema.py
+-rw-r--r--   0        0        0      227 2023-06-15 21:16:27.736193 lassen-0.2.0/lassen/shared.py
+-rw-r--r--   0        0        0     9988 2023-07-22 17:00:28.390179 lassen-0.2.0/lassen/store.py
+-rw-r--r--   0        0        0      201 2023-07-22 17:00:28.390303 lassen-0.2.0/lassen/stubs/__init__.py
+-rw-r--r--   0        0        0     1170 2023-07-22 17:00:28.390398 lassen-0.2.0/lassen/stubs/base.py
+-rw-r--r--   0        0        0      147 2023-07-22 17:00:28.390482 lassen-0.2.0/lassen/stubs/definition.py
+-rw-r--r--   0        0        0     1892 2023-07-22 17:00:28.390588 lassen-0.2.0/lassen/stubs/field.py
+-rw-r--r--   0        0        0     3731 2023-07-22 17:00:28.390696 lassen-0.2.0/lassen/stubs/generate.py
+-rw-r--r--   0        0        0       96 2023-07-22 17:00:28.390790 lassen-0.2.0/lassen/stubs/generators/__init__.py
+-rw-r--r--   0        0        0     8487 2023-07-22 17:00:28.390910 lassen-0.2.0/lassen/stubs/generators/common.py
+-rw-r--r--   0        0        0     4165 2023-07-22 17:00:28.391026 lassen-0.2.0/lassen/stubs/generators/schema.py
+-rw-r--r--   0        0        0    12025 2023-07-22 17:00:28.391178 lassen-0.2.0/lassen/stubs/generators/store.py
+-rw-r--r--   0        0        0      177 2023-07-22 17:00:28.391343 lassen-0.2.0/lassen/stubs/templates/__init__.py
+-rw-r--r--   0        0        0     1052 2023-07-22 17:00:28.391457 lassen-0.2.0/lassen/stubs/templates/schema.py.j2
+-rw-r--r--   0        0        0      551 2023-07-22 17:00:28.391564 lassen-0.2.0/lassen/stubs/templates/sqlalchemy.py.j2
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.990727 lassen-0.2.0/lassen/tests/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-15 21:16:27.736415 lassen-0.2.0/lassen/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1973 2023-06-15 21:31:07.938752 lassen-0.2.0/lassen/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1220 2023-06-06 23:14:20.991368 lassen-0.2.0/lassen/tests/__pycache__/fixtures.cpython-310.pyc
+-rw-r--r--   0        0        0     5734 2023-06-15 21:16:27.736953 lassen-0.2.0/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1901 2023-06-15 21:16:27.737091 lassen-0.2.0/lassen/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-15 21:16:27.737128 lassen-0.2.0/lassen/tests/datasets/__init__.py
+-rw-r--r--   0        0        0     2243 2023-06-15 22:42:38.547093 lassen-0.2.0/lassen/tests/datasets/test_dataset_helpers.py
+-rw-r--r--   0        0        0     1645 2023-06-15 22:26:02.923228 lassen-0.2.0/lassen/tests/datasets/test_pyarrow_schemas.py
+-rw-r--r--   0        0        0      176 2023-06-06 23:14:20.991801 lassen-0.2.0/lassen/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     1215 2023-07-22 17:00:28.391699 lassen-0.2.0/lassen/tests/fixtures/stubs/expected_schema.py
+-rw-r--r--   0        0        0     1013 2023-07-22 17:00:28.391801 lassen-0.2.0/lassen/tests/fixtures/stubs/expected_schema_public.py
+-rw-r--r--   0        0        0      989 2023-07-22 17:00:28.391909 lassen-0.2.0/lassen/tests/fixtures/stubs/expected_store.py
+-rw-r--r--   0        0        0     1095 2023-07-22 17:00:28.392269 lassen-0.2.0/lassen/tests/fixtures/stubs/fixtures.py
+-rw-r--r--   0        0        0      463 2023-06-06 23:14:20.991923 lassen-0.2.0/lassen/tests/fixtures/test_harness/README.md
+-rw-r--r--   0        0        0      311 2023-06-06 23:14:20.992056 lassen-0.2.0/lassen/tests/fixtures/test_harness/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.992112 lassen-0.2.0/lassen/tests/fixtures/test_harness/test_harness/__init__.py
+-rw-r--r--   0        0        0      691 2023-06-06 23:14:20.992321 lassen-0.2.0/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py
+-rw-r--r--   0        0        0      653 2023-06-06 23:14:20.992456 lassen-0.2.0/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py
+-rw-r--r--   0        0        0      217 2023-06-06 23:14:20.992593 lassen-0.2.0/lassen/tests/fixtures/test_harness/test_harness/models.py
+-rw-r--r--   0        0        0      461 2023-06-06 23:14:20.992727 lassen-0.2.0/lassen/tests/model_fixtures.py
+-rw-r--r--   0        0        0        0 2023-07-22 17:00:28.392359 lassen-0.2.0/lassen/tests/stubs/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-22 17:00:28.392464 lassen-0.2.0/lassen/tests/stubs/generators/__init__.py
+-rw-r--r--   0        0        0     3828 2023-07-22 17:00:28.392630 lassen-0.2.0/lassen/tests/stubs/generators/test_common.py
+-rw-r--r--   0        0        0      712 2023-07-22 17:00:28.392845 lassen-0.2.0/lassen/tests/stubs/generators/test_schema.py
+-rw-r--r--   0        0        0     2671 2023-07-22 17:00:28.393035 lassen-0.2.0/lassen/tests/stubs/generators/test_store.py
+-rw-r--r--   0        0        0     2560 2023-07-22 17:00:28.393152 lassen-0.2.0/lassen/tests/stubs/test_generate.py
+-rw-r--r--   0        0        0     2252 2023-06-06 23:14:20.992858 lassen-0.2.0/lassen/tests/test_alembic.py
+-rw-r--r--   0        0        0     2842 2023-07-22 17:00:28.393357 lassen-0.2.0/lassen/tests/test_store.py
+-rw-r--r--   0        0        0     1423 2023-07-22 17:00:34.267205 lassen-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4987 1970-01-01 00:00:00.000000 lassen-0.2.0/setup.py
+-rw-r--r--   0        0        0     4129 1970-01-01 00:00:00.000000 lassen-0.2.0/PKG-INFO
```

### Comparing `lassen-0.1.3/LICENSE` & `lassen-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/README.md` & `lassen-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,26 @@
 
 Core utilities for MonkeySee web applications.
 
 Not guaranteed to be backwards compatible, use at your own risk.
 
 ## Structure
 
-**Stores:** Each model is expected to have its own store. Base classes that provide standard logic are provided by `lassen.store`
+**Stores:** Each datamodel is expected to have its own store. Base classes that provide standard logic are provided by `lassen.store`
 - StoreBase: Base class for all stores
 - StoreFilterMixin: Mixin for filtering stores that specify an additional schema to use to filter
 
+**Schemas:** Each datamodel should define a Model class (SQLAlchemy base object) and a series of Schema objects (Pydantic) that allow the Store to serialize the models. These schemas are also often used for direct CRUD referencing in the API layer.
+
+We use a base `Stub` file to generate these schemas from a centralized definition.
+
+```bash
+poetry run generate-lassen
+```
+
 **Datasets:** Optional huggingface `datasets` processing utilities. Only installed under the `lassen[datasets]` extra. These provide support for:
 
 - batch_to_examples: Iterate and manipulate each example separately, versus over nested key-based lists.
 - examples_to_batch: Takes the output of a typehinted element-wise batch and converts into the format needed for dataset insertion. If datasets can't automatically interpret the type of the fields, also provide automatic casting based on the typehinted dataclass.
 
 ```python
 from lassen.datasets import batch_to_examples, examples_to_batch
```

### Comparing `lassen-0.1.3/lassen/alembic/cli.py` & `lassen-0.2.0/lassen/alembic/cli.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/lassen/alembic/runner.py` & `lassen-0.2.0/lassen/alembic/runner.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/lassen/assets/alembic.ini` & `lassen-0.2.0/lassen/assets/alembic.ini`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/lassen/core/__pycache__/config.cpython-310.pyc` & `lassen-0.2.0/lassen/core/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/lassen/core/config.py` & `lassen-0.2.0/lassen/core/config.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/lassen/datasets/dataset_helpers.py` & `lassen-0.2.0/lassen/datasets/dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/lassen/datasets/pyarrow_schemas.py` & `lassen-0.2.0/lassen/datasets/pyarrow_schemas.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/lassen/db/__pycache__/base_class.cpython-310.pyc` & `lassen-0.2.0/lassen/db/__pycache__/base_class.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/lassen/db/__pycache__/base_class.cpython-311.pyc` & `lassen-0.2.0/lassen/db/__pycache__/base_class.cpython-311.pyc`

 * *Files 19% similar despite different names*

#### Python bytecode

```diff
@@ -1,24 +1,24 @@
 magic:    0xa70d0d0a
-moddate:  0x95e26764 (Fri May 19 20:56:53 2023 UTC)
-files sz: 1749
+moddate:  0x73f8ba64 (Fri Jul 21 21:28:19 2023 UTC)
+files sz: 1920
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c046d055a056d065a066d075a076d085a080100640064046c096d0a5a
-      0a6d0b5a0b6d0c5a0c6d0d5a0d6d0e5a0e0100650c020047006405840064
-      06a6020000ab020000000000000000a6000000ab0000000000000000005a
-      0f02004700640784006408a6020000ab0200000000000000005a10020065
-      0ba6000000ab0000000000000000005a11020065076a1200000000000000
-      00650a6409a6020000ab020000000000000000640a8400a6000000ab0000
-      000000000000005a13640b5300
+      0a6d0b5a0b6d0c5a0c6d0d5a0d6d0e5a0e6d0f5a0f0100650d0200470064
+      0584006406a6020000ab020000000000000000a6000000ab000000000000
+      0000005a1002004700640784006408a6020000ab0200000000000000005a
+      110200470064098400640a650aa6030000ab0300000000000000005a1202
+      0065076a130000000000000000650c640ba6020000ab0200000000000000
+      00640c8400a6000000ab0000000000000000005a14640d5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Any',))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Any)
                 10 STORE_NAME               1 (Any)
@@ -41,177 +41,188 @@
                 40 IMPORT_FROM              7 (event)
                 42 STORE_NAME               7 (event)
                 44 IMPORT_FROM              8 (false)
                 46 STORE_NAME               8 (false)
                 48 POP_TOP
    
      5          50 LOAD_CONST               0 (0)
-                52 LOAD_CONST               4 (('Session', 'declarative_base', 'declarative_mixin', 'declared_attr', 'with_loader_criteria'))
+                52 LOAD_CONST               4 (('DeclarativeBase', 'Mapped', 'Session', 'declarative_mixin', 'declared_attr', 'with_loader_criteria'))
                 54 IMPORT_NAME              9 (sqlalchemy.orm)
-                56 IMPORT_FROM             10 (Session)
-                58 STORE_NAME              10 (Session)
-                60 IMPORT_FROM             11 (declarative_base)
-                62 STORE_NAME              11 (declarative_base)
-                64 IMPORT_FROM             12 (declarative_mixin)
-                66 STORE_NAME              12 (declarative_mixin)
-                68 IMPORT_FROM             13 (declared_attr)
-                70 STORE_NAME              13 (declared_attr)
-                72 IMPORT_FROM             14 (with_loader_criteria)
-                74 STORE_NAME              14 (with_loader_criteria)
-                76 POP_TOP
-   
-    14          78 LOAD_NAME               12 (declarative_mixin)
-   
-    15          80 PUSH_NULL
-                82 LOAD_BUILD_CLASS
-                84 LOAD_CONST               5 (<code object MainMixin, file "/code/selectify/db/base_class.py", line 14>)
-                86 MAKE_FUNCTION            0
-                88 LOAD_CONST               6 ('MainMixin')
-                90 PRECALL                  2
-                94 CALL                     2
-   
-    14         104 PRECALL                  0
-               108 CALL                     0
-   
-    15         118 STORE_NAME              15 (MainMixin)
-   
-    25         120 PUSH_NULL
-               122 LOAD_BUILD_CLASS
-               124 LOAD_CONST               7 (<code object ArchivedMixin, file "/code/selectify/db/base_class.py", line 25>)
-               126 MAKE_FUNCTION            0
-               128 LOAD_CONST               8 ('ArchivedMixin')
-               130 PRECALL                  2
-               134 CALL                     2
-               144 STORE_NAME              16 (ArchivedMixin)
-   
-    29         146 PUSH_NULL
-               148 LOAD_NAME               11 (declarative_base)
-               150 PRECALL                  0
-               154 CALL                     0
-               164 STORE_NAME              17 (Base)
-   
-    33         166 PUSH_NULL
-               168 LOAD_NAME                7 (event)
-               170 LOAD_ATTR               18 (listens_for)
-               180 LOAD_NAME               10 (Session)
-               182 LOAD_CONST               9 ('do_orm_execute')
-               184 PRECALL                  2
-               188 CALL                     2
-   
-    34         198 LOAD_CONST              10 (<code object _add_filtering_criteria, file "/code/selectify/db/base_class.py", line 33>)
-               200 MAKE_FUNCTION            0
-   
-    33         202 PRECALL                  0
-               206 CALL                     0
-   
-    34         216 STORE_NAME              19 (_add_filtering_criteria)
-               218 LOAD_CONST              11 (None)
-               220 RETURN_VALUE
+                56 IMPORT_FROM             10 (DeclarativeBase)
+                58 STORE_NAME              10 (DeclarativeBase)
+                60 IMPORT_FROM             11 (Mapped)
+                62 STORE_NAME              11 (Mapped)
+                64 IMPORT_FROM             12 (Session)
+                66 STORE_NAME              12 (Session)
+                68 IMPORT_FROM             13 (declarative_mixin)
+                70 STORE_NAME              13 (declarative_mixin)
+                72 IMPORT_FROM             14 (declared_attr)
+                74 STORE_NAME              14 (declared_attr)
+                76 IMPORT_FROM             15 (with_loader_criteria)
+                78 STORE_NAME              15 (with_loader_criteria)
+                80 POP_TOP
+   
+    15          82 LOAD_NAME               13 (declarative_mixin)
+   
+    16          84 PUSH_NULL
+                86 LOAD_BUILD_CLASS
+                88 LOAD_CONST               5 (<code object MainMixin, file "/Users/piercefreeman/projects/lassen/lassen/db/base_class.py", line 15>)
+                90 MAKE_FUNCTION            0
+                92 LOAD_CONST               6 ('MainMixin')
+                94 PRECALL                  2
+                98 CALL                     2
+   
+    15         108 PRECALL                  0
+               112 CALL                     0
+   
+    16         122 STORE_NAME              16 (MainMixin)
+   
+    27         124 PUSH_NULL
+               126 LOAD_BUILD_CLASS
+               128 LOAD_CONST               7 (<code object ArchivedMixin, file "/Users/piercefreeman/projects/lassen/lassen/db/base_class.py", line 27>)
+               130 MAKE_FUNCTION            0
+               132 LOAD_CONST               8 ('ArchivedMixin')
+               134 PRECALL                  2
+               138 CALL                     2
+               148 STORE_NAME              17 (ArchivedMixin)
+   
+    31         150 PUSH_NULL
+               152 LOAD_BUILD_CLASS
+               154 LOAD_CONST               9 (<code object Base, file "/Users/piercefreeman/projects/lassen/lassen/db/base_class.py", line 31>)
+               156 MAKE_FUNCTION            0
+               158 LOAD_CONST              10 ('Base')
+               160 LOAD_NAME               10 (DeclarativeBase)
+               162 PRECALL                  3
+               166 CALL                     3
+               176 STORE_NAME              18 (Base)
+   
+    36         178 PUSH_NULL
+               180 LOAD_NAME                7 (event)
+               182 LOAD_ATTR               19 (listens_for)
+               192 LOAD_NAME               12 (Session)
+               194 LOAD_CONST              11 ('do_orm_execute')
+               196 PRECALL                  2
+               200 CALL                     2
+   
+    37         210 LOAD_CONST              12 (<code object _add_filtering_criteria, file "/Users/piercefreeman/projects/lassen/lassen/db/base_class.py", line 36>)
+               212 MAKE_FUNCTION            0
+   
+    36         214 PRECALL                  0
+               218 CALL                     0
+   
+    37         228 STORE_NAME              20 (_add_filtering_criteria)
+               230 LOAD_CONST              13 (None)
+               232 RETURN_VALUE
    consts
       0
       ('Any',)
       ('underscore',)
       ('Boolean', 'Column', 'event', 'false')
-      ('Session', 'declarative_base', 'declarative_mixin', 'declared_attr', 'with_loader_criteria')
+      ('DeclarativeBase', 'Mapped', 'Session', 'declarative_mixin', 'declared_attr', 'with_loader_criteria')
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 3
+         stacksize : 6
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c0000006505650464023c
-            000000650664036505660264048404a6000000ab0000000000000000005a
-            0764055300
-          14           0 RESUME                   0
+            000000650664036400640465076505190000000000000000006604640584
+            04a6000000ab0000000000000000005a0864065300
+          15           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('MainMixin')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          16          12 LOAD_NAME                3 (Any)
+          17          12 LOAD_NAME                3 (Any)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('id')
                       18 STORE_SUBSCR
          
-          17          22 LOAD_NAME                5 (str)
+          18          22 LOAD_NAME                5 (str)
                       24 LOAD_NAME                4 (__annotations__)
                       26 LOAD_CONST               2 ('__name__')
                       28 STORE_SUBSCR
          
-          20          32 LOAD_NAME                6 (declared_attr)
+          22          32 LOAD_NAME                6 (declared_attr)
          
-          21          34 LOAD_CONST               3 ('return')
-                      36 LOAD_NAME                5 (str)
-                      38 BUILD_TUPLE              2
-                      40 LOAD_CONST               4 (<code object __tablename__, file "/code/selectify/db/base_class.py", line 20>)
-                      42 MAKE_FUNCTION            4 (annotations)
-         
-          20          44 PRECALL                  0
-                      48 CALL                     0
-         
-          21          58 STORE_NAME               7 (__tablename__)
-                      60 LOAD_CONST               5 (None)
-                      62 RETURN_VALUE
+          23          34 LOAD_CONST               3 ('cls')
+                      36 LOAD_CONST               0 ('MainMixin')
+                      38 LOAD_CONST               4 ('return')
+                      40 LOAD_NAME                7 (Mapped)
+                      42 LOAD_NAME                5 (str)
+                      44 BINARY_SUBSCR
+                      54 BUILD_TUPLE              4
+                      56 LOAD_CONST               5 (<code object __tablename__, file "/Users/piercefreeman/projects/lassen/lassen/db/base_class.py", line 22>)
+                      58 MAKE_FUNCTION            4 (annotations)
+         
+          22          60 PRECALL                  0
+                      64 CALL                     0
+         
+          23          74 STORE_NAME               8 (__tablename__)
+                      76 LOAD_CONST               6 (None)
+                      78 RETURN_VALUE
          consts
             'MainMixin'
             'id'
             '__name__'
+            'cls'
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000005300
-                20           0 RESUME                   0
+                22           0 RESUME                   0
                
-                22           2 LOAD_GLOBAL              1 (NULL + underscore)
+                24           2 LOAD_GLOBAL              1 (NULL + underscore)
                             14 LOAD_FAST                0 (cls)
                             16 LOAD_ATTR                1 (__name__)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 RETURN_VALUE
                consts
                   None
                names      ('underscore', '__name__')
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
-               filename   '/code/selectify/db/base_class.py'
+               filename   '/Users/piercefreeman/projects/lassen/lassen/db/base_class.py'
                name       '__tablename__'
-               firstlineno 20
+               firstlineno 22
                lnotab 0x0202
             None
-         names      ('__name__', '__module__', '__qualname__', 'Any', '__annotations__', 'str', 'declared_attr', '__tablename__')
+         names      ('__name__', '__module__', '__qualname__', 'Any', '__annotations__', 'str', 'declared_attr', 'Mapped', '__tablename__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/code/selectify/db/base_class.py'
+         filename   '/Users/piercefreeman/projects/lassen/lassen/db/base_class.py'
          name       'MainMixin'
-         firstlineno 14
-         lnotab 0x0c020a010a0302010aff0e01
+         firstlineno 15
+         lnotab 0x0c020a010a0402011aff0e01
       'MainMixin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a0202006503650464016401ac02a6030000ab0300
             000000000000005a0564035300
-          25           0 RESUME                   0
+          27           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ArchivedMixin')
                        8 STORE_NAME               2 (__qualname__)
          
-          26          10 PUSH_NULL
+          28          10 PUSH_NULL
                       12 LOAD_NAME                3 (Column)
                       14 LOAD_NAME                4 (Boolean)
                       16 LOAD_CONST               1 (False)
                       18 LOAD_CONST               1 (False)
                       20 KW_NAMES                 2
                       22 PRECALL                  3
                       26 CALL                     3
@@ -223,80 +234,106 @@
             False
             ('default', 'nullable')
             None
          names      ('__name__', '__module__', '__qualname__', 'Column', 'Boolean', 'archived')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/code/selectify/db/base_class.py'
+         filename   '/Users/piercefreeman/projects/lassen/lassen/db/base_class.py'
          name       'ArchivedMixin'
-         firstlineno 25
+         firstlineno 27
          lnotab 0x0a01
       'ArchivedMixin'
+      code
+         argcount  : 0
+         nlocals   : 0
+         stacksize : 1
+         flags     : 0
+         code 0x970065005a0164005a0264015300
+          31           0 RESUME                   0
+                       2 LOAD_NAME                0 (__name__)
+                       4 STORE_NAME               1 (__module__)
+                       6 LOAD_CONST               0 ('Base')
+                       8 STORE_NAME               2 (__qualname__)
+         
+          32          10 LOAD_CONST               1 (None)
+                      12 RETURN_VALUE
+         consts
+            'Base'
+            None
+         names      ('__name__', '__module__', '__qualname__')
+         varnames   ()
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/piercefreeman/projects/lassen/lassen/db/base_class.py'
+         name       'Base'
+         firstlineno 31
+         lnotab 0x0a01
+      'Base'
       'do_orm_execute'
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 7
          flags     : 3
          code
             0x97007c006a00000000000000000073597c006a01000000000000000073
             547c006a020000000000000000a003000000000000000000000000000000
             000000000064016402a6020000ab020000000000000000733b7c006a0400
             00000000000000a005000000000000000000000000000000000000000074
             0d00000000000000000000740e00000000000000000000640384006404ac
             05a6030000ab030000000000000000a6010000ab0100000000000000007c
             005f04000000000000000064065300640653006406530064065300
-          33           0 RESUME                   0
+          36           0 RESUME                   0
          
-          50           2 LOAD_FAST                0 (execute_state)
+          53           2 LOAD_FAST                0 (execute_state)
                        4 LOAD_ATTR                0 (is_column_load)
          
-          49          14 POP_JUMP_FORWARD_IF_TRUE    89 (to 194)
+          52          14 POP_JUMP_FORWARD_IF_TRUE    89 (to 194)
          
-          51          16 LOAD_FAST                0 (execute_state)
+          54          16 LOAD_FAST                0 (execute_state)
                       18 LOAD_ATTR                1 (is_relationship_load)
          
-          49          28 POP_JUMP_FORWARD_IF_TRUE    84 (to 198)
+          52          28 POP_JUMP_FORWARD_IF_TRUE    84 (to 198)
          
-          52          30 LOAD_FAST                0 (execute_state)
+          55          30 LOAD_FAST                0 (execute_state)
                       32 LOAD_ATTR                2 (execution_options)
                       42 LOAD_METHOD              3 (get)
                       64 LOAD_CONST               1 ('include_archived')
                       66 LOAD_CONST               2 (False)
                       68 PRECALL                  2
                       72 CALL                     2
          
-          49          82 POP_JUMP_FORWARD_IF_TRUE    59 (to 202)
+          52          82 POP_JUMP_FORWARD_IF_TRUE    59 (to 202)
          
-          55          84 LOAD_FAST                0 (execute_state)
+          58          84 LOAD_FAST                0 (execute_state)
                       86 LOAD_ATTR                4 (statement)
                       96 LOAD_METHOD              5 (options)
          
-          56         118 LOAD_GLOBAL             13 (NULL + with_loader_criteria)
+          59         118 LOAD_GLOBAL             13 (NULL + with_loader_criteria)
          
-          57         130 LOAD_GLOBAL             14 (ArchivedMixin)
+          60         130 LOAD_GLOBAL             14 (ArchivedMixin)
          
-          58         142 LOAD_CONST               3 (<code object <lambda>, file "/code/selectify/db/base_class.py", line 58>)
+          61         142 LOAD_CONST               3 (<code object <lambda>, file "/Users/piercefreeman/projects/lassen/lassen/db/base_class.py", line 61>)
                      144 MAKE_FUNCTION            0
          
-          59         146 LOAD_CONST               4 (True)
+          62         146 LOAD_CONST               4 (True)
          
-          56         148 KW_NAMES                 5
+          59         148 KW_NAMES                 5
                      150 PRECALL                  3
                      154 CALL                     3
          
-          55         164 PRECALL                  1
+          58         164 PRECALL                  1
                      168 CALL                     1
                      178 LOAD_FAST                0 (execute_state)
                      180 STORE_ATTR               4 (statement)
                      190 LOAD_CONST               6 (None)
                      192 RETURN_VALUE
          
-          49     >>  194 LOAD_CONST               6 (None)
+          52     >>  194 LOAD_CONST               6 (None)
                      196 RETURN_VALUE
                  >>  198 LOAD_CONST               6 (None)
                      200 RETURN_VALUE
                  >>  202 LOAD_CONST               6 (None)
                      204 RETURN_VALUE
          consts
             'Intercept all ORM queries.   Add a with_loader_criteria option to all\n    of them.\n\n    This option applies to SELECT queries and adds a global WHERE criteria\n    (or as appropriate ON CLAUSE criteria for join targets)\n    to all objects of a certain class or superclass.\n\n    '
@@ -306,47 +343,47 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 19
                code
                   0x97007c006a000000000000000000740300000000000000000000a60000
                   00ab0000000000000000006b02000000005300
-                58           0 RESUME                   0
+                61           0 RESUME                   0
                              2 LOAD_FAST                0 (cls)
                              4 LOAD_ATTR                0 (archived)
                             14 LOAD_GLOBAL              3 (NULL + false)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 COMPARE_OP               2 (==)
                             46 RETURN_VALUE
                consts
                   None
                names      ('archived', 'false')
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
-               filename   '/code/selectify/db/base_class.py'
+               filename   '/Users/piercefreeman/projects/lassen/lassen/db/base_class.py'
                name       '<lambda>'
-               firstlineno 58
+               firstlineno 61
                lnotab 0x
             True
             ('include_aliases',)
             None
          names      ('is_column_load', 'is_relationship_load', 'execution_options', 'get', 'statement', 'options', 'with_loader_criteria', 'ArchivedMixin')
          varnames   ('execute_state',)
          freevars   ()
          cellvars   ()
-         filename   '/code/selectify/db/base_class.py'
+         filename   '/Users/piercefreeman/projects/lassen/lassen/db/base_class.py'
          name       '_add_filtering_criteria'
-         firstlineno 33
+         firstlineno 36
          lnotab 0x02110cff02020cfe020334fd020622010c010c01040102fd10ff1efa
       None
-   names      ('typing', 'Any', 'inflection', 'underscore', 'sqlalchemy', 'Boolean', 'Column', 'event', 'false', 'sqlalchemy.orm', 'Session', 'declarative_base', 'declarative_mixin', 'declared_attr', 'with_loader_criteria', 'MainMixin', 'ArchivedMixin', 'Base', 'listens_for', '_add_filtering_criteria')
+   names      ('typing', 'Any', 'inflection', 'underscore', 'sqlalchemy', 'Boolean', 'Column', 'event', 'false', 'sqlalchemy.orm', 'DeclarativeBase', 'Mapped', 'Session', 'declarative_mixin', 'declared_attr', 'with_loader_criteria', 'MainMixin', 'ArchivedMixin', 'Base', 'listens_for', '_add_filtering_criteria')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/code/selectify/db/base_class.py'
+   filename   '/Users/piercefreeman/projects/lassen/lassen/db/base_class.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c020c0118011c09020118ff0e01020a1a041404200104ff0e
+      0x00ff02010c020c011801200a020118ff0e01020b1a041c05200104ff0e
       01
```

### Comparing `lassen-0.1.3/lassen/db/__pycache__/session.cpython-310.pyc` & `lassen-0.2.0/lassen/db/__pycache__/session.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/lassen/db/__pycache__/session.cpython-311.pyc` & `lassen-0.2.0/lassen/db/__pycache__/session.cpython-311.pyc`

 * *Files 25% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x36cf6e64 (Thu May 25 03:00:06 2023 UTC)
-files sz: 630
+moddate:  0xccbd7f64 (Tue Jun  6 23:14:20 2023 UTC)
+files sz: 627
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -31,29 +31,29 @@
                 30 IMPORT_NAME              4 (sqlalchemy.orm)
                 32 IMPORT_FROM              5 (sessionmaker)
                 34 STORE_NAME               5 (sessionmaker)
                 36 POP_TOP
    
      6          38 LOAD_CONST               0 (0)
                 40 LOAD_CONST               4 (('get_settings',))
-                42 IMPORT_NAME              6 (selectify.core.config)
+                42 IMPORT_NAME              6 (lassen.core.config)
                 44 IMPORT_FROM              7 (get_settings)
                 46 STORE_NAME               7 (get_settings)
                 48 POP_TOP
    
      8          50 LOAD_CONST               5 (None)
                 52 STORE_GLOBAL             8 (SessionLocal)
    
-    11          54 LOAD_CONST               6 (<code object get_session_local, file "/code/selectify/db/session.py", line 11>)
+    11          54 LOAD_CONST               6 (<code object get_session_local, file "/Users/piercefreeman/projects/lassen/lassen/db/session.py", line 11>)
                 56 MAKE_FUNCTION            0
                 58 STORE_NAME               9 (get_session_local)
    
     20          60 LOAD_NAME                1 (contextmanager)
    
-    21          62 LOAD_CONST               7 (<code object get_db_context, file "/code/selectify/db/session.py", line 20>)
+    21          62 LOAD_CONST               7 (<code object get_db_context, file "/Users/piercefreeman/projects/lassen/lassen/db/session.py", line 20>)
                 64 MAKE_FUNCTION            0
    
     20          66 PRECALL                  0
                 70 CALL                     0
    
     21          80 STORE_NAME              10 (get_db_context)
                 82 LOAD_CONST               5 (None)
@@ -109,15 +109,15 @@
             ('pool_pre_ping',)
             False
             ('autocommit', 'autoflush', 'bind')
          names      ('get_settings', 'create_engine', 'SQLALCHEMY_DATABASE_URI', 'sessionmaker', 'SessionLocal')
          varnames   ('settings', 'engine')
          freevars   ()
          cellvars   ()
-         filename   '/code/selectify/db/session.py'
+         filename   '/Users/piercefreeman/projects/lassen/lassen/db/session.py'
          name       'get_session_local'
          firstlineno 11
          lnotab 0x02031c012c012401
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 4
@@ -184,19 +184,19 @@
            116 to 164 -> 166 [1] lasti
          consts
             None
          names      ('get_session_local', 'close')
          varnames   ('db',)
          freevars   ()
          cellvars   ()
-         filename   '/code/selectify/db/session.py'
+         filename   '/Users/piercefreeman/projects/lassen/lassen/db/session.py'
          name       'get_db_context'
          firstlineno 20
          lnotab 0x0602040102012c01080204012cff0a012aff
-   names      ('contextlib', 'contextmanager', 'sqlalchemy', 'create_engine', 'sqlalchemy.orm', 'sessionmaker', 'selectify.core.config', 'get_settings', 'SessionLocal', 'get_session_local', 'get_db_context')
+   names      ('contextlib', 'contextmanager', 'sqlalchemy', 'create_engine', 'sqlalchemy.orm', 'sessionmaker', 'lassen.core.config', 'get_settings', 'SessionLocal', 'get_session_local', 'get_db_context')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/code/selectify/db/session.py'
+   filename   '/Users/piercefreeman/projects/lassen/lassen/db/session.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c020c010c020c0204030609020104ff0e01
```

### Comparing `lassen-0.1.3/lassen/db/base_class.py` & `lassen-0.2.0/lassen/db/base_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any
 
 from inflection import underscore
 from sqlalchemy import Boolean, Column, event, false
 from sqlalchemy.orm import (
+    DeclarativeBase,
     Mapped,
     Session,
-    declarative_base,
     declarative_mixin,
     declared_attr,
     with_loader_criteria,
 )
 
 
 @declarative_mixin
@@ -24,15 +24,16 @@
         return underscore(cls.__name__)  # type: ignore
 
 
 class ArchivedMixin:
     archived = Column(Boolean, default=False, nullable=False)
 
 
-Base = declarative_base()
+class Base(DeclarativeBase):
+    pass
 
 
 # https://docs.sqlalchemy.org/en/14/_modules/examples/extending_query/filter_public.html
 @event.listens_for(Session, "do_orm_execute")
 def _add_filtering_criteria(execute_state):
     """Intercept all ORM queries.   Add a with_loader_criteria option to all
     of them.
```

### Comparing `lassen-0.1.3/lassen/db/session.py` & `lassen-0.2.0/lassen/db/session.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/lassen/store.py` & `lassen-0.2.0/lassen/store.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
             static_value = obj_in_data[relationship]
             static_value_original = (
                 obj_in[relationship]
                 if isinstance(obj_in, dict)
                 else getattr(obj_in, relationship)
             )
-            database_value = None
+            database_value: Any = None
 
             # Determine if we should create a list
             # Otherwise assume this is an object
             if isinstance(static_value, list):
                 database_value = []
                 for value, original_value in zip(static_value, static_value_original):
                     # print("ORIGINAL", original_value)
```

### Comparing `lassen-0.1.3/lassen/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc` & `lassen-0.2.0/lassen/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/lassen/tests/__pycache__/fixtures.cpython-310.pyc` & `lassen-0.2.0/lassen/tests/__pycache__/fixtures.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc` & `lassen-0.2.0/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/lassen/tests/conftest.py` & `lassen-0.2.0/lassen/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/lassen/tests/datasets/test_dataset_helpers.py` & `lassen-0.2.0/lassen/tests/datasets/test_dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/lassen/tests/datasets/test_pyarrow_schemas.py` & `lassen-0.2.0/lassen/tests/datasets/test_pyarrow_schemas.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py` & `lassen-0.2.0/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py` & `lassen-0.2.0/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/lassen/tests/test_alembic.py` & `lassen-0.2.0/lassen/tests/test_alembic.py`

 * *Files identical despite different names*

### Comparing `lassen-0.1.3/lassen/tests/test_store.py` & `lassen-0.2.0/lassen/tests/test_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import pytest
 from sqlalchemy.orm import Session
 
 from lassen.store import StoreBase
-from lassen.tests.model_fixtures import (
-    TestModel,
-    TestSchema,
-    TestSchemaCreate,
-    TestSchemaUpdate,
-)
+from lassen.tests.model_fixtures import TestModel, TestSchemaCreate, TestSchemaUpdate
 
 
 @pytest.fixture
 def use_fixture_models(db_session: Session):
+    if not db_session.bind:
+        raise ValueError("No database connection")
+
     from lassen.db.base_class import Base
 
     Base.metadata.create_all(bind=db_session.bind)
 
 
 def create_batch(db_session: Session, quantity: int = 1):
     create_identifiers = []
@@ -27,29 +25,29 @@
         create_identifiers.append(test_model.id)
     return create_identifiers
 
 
 def test_store_base_get(db_session: Session, use_fixture_models):
     test_model_id = create_batch(db_session, quantity=1)[0]
 
-    store = StoreBase[TestSchema, TestSchemaCreate, TestSchemaUpdate](TestModel)
+    store = StoreBase[TestModel, TestSchemaCreate, TestSchemaUpdate](TestModel)
     # Test with a valid ID
     retrieved = store.get(db_session, id=test_model_id)
     assert retrieved is not None
     assert retrieved.id == test_model_id
     assert retrieved.name == f"Test Model 0"
 
     # Test with an invalid ID
     assert store.get(db_session, id=9999) == None
 
 
 def test_store_base_get_multi(db_session: Session, use_fixture_models):
     create_batch(db_session, quantity=5)
 
-    store = StoreBase[TestSchema, TestSchemaCreate, TestSchemaUpdate](TestModel)
+    store = StoreBase[TestModel, TestSchemaCreate, TestSchemaUpdate](TestModel)
     # Test without skip and limit
     retrieved = store.get_multi(db_session)
     assert len(retrieved) == 5
 
     # Test with skip
     retrieved = store.get_multi(db_session, skip=2)
     assert len(retrieved) == 3
@@ -62,27 +60,27 @@
     retrieved = store.get_multi(db_session, skip=1, limit=2)
     assert len(retrieved) == 2
 
 
 def test_store_base_update(db_session: Session, use_fixture_models):
     test_model_id = create_batch(db_session, quantity=1)[0]
 
-    store = StoreBase[TestSchema, TestSchemaCreate, TestSchemaUpdate](TestModel)
+    store = StoreBase[TestModel, TestSchemaCreate, TestSchemaUpdate](TestModel)
     update_schema = TestSchemaUpdate(id=test_model_id, name="Updated Name")
     db_obj = store.get(db_session, id=test_model_id)
     assert db_obj is not None
 
     updated = store.update(db_session, db_obj=db_obj, obj_in=update_schema)
     db_session.commit()
     assert updated.id == test_model_id
     assert updated.name == "Updated Name"
 
 
 def test_store_base_remove(db_session: Session, use_fixture_models):
     test_model_id = create_batch(db_session, quantity=1)[0]
 
-    store = StoreBase[TestSchema, TestSchemaCreate, TestSchemaUpdate](TestModel)
+    store = StoreBase[TestModel, TestSchemaCreate, TestSchemaUpdate](TestModel)
     store.remove(db_session, id=test_model_id)
     db_session.commit()
 
     # Test that the model instance has been removed
     assert store.get(db_session, id=test_model_id) is None
```

### Comparing `lassen-0.1.3/pyproject.toml` & `lassen-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [tool.poetry]
 name = "lassen"
-version = "0.1.3"
+version = "0.2.0"
 description = "Common webapp scaffolding."
 authors = ["Pierce Freeman <pierce@freeman.vc>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10"
-fastapi = "^0.96.0"
-pydantic = "^1.10.8"
+python = "^3.11"
+fastapi = "^0.95.1"
+pydantic = "^1.10.2"
 inflection = "^0.5.1"
 click = "^8.1.3"
 alembic = "^1.11.1"
 alembic-autogenerate-enums = "^0.1.1"
 python-dotenv = "^1.0.0"
 
 datasets = { version = "^2.13.0", optional = true }
 numpy = { version = "^1.24.3", optional = true }
 pandas = { version = "^2.0.2", optional = true }
 
 SQLAlchemy = { version = "^2.0.15", optional = true }
 psycopg2 = { version = "^2.9.6", optional = true }
+Jinja2 = "^3.1.2"
 
 [tool.poetry.extras]
 datasets = ["datasets", "numpy", "pandas"]
 database = ["SQLAlchemy", "psycopg2"]
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
@@ -38,20 +39,24 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 migrate = "lassen.alembic.cli:main"
+generate-lassen = "lassen.stubs.generate:cli"
 
 [tool.isort]
 profile = "black"
 known_first_party = "lassen"
 multi_line_output=3
 
+[tool.mypy]
+exclude = "fixtures"
+
 [[tool.mypy.overrides]]
 module = "pyarrow.*"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "datasets.*"
 ignore_missing_imports = true
```

### Comparing `lassen-0.1.3/setup.py` & `lassen-0.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,54 +4,62 @@
 packages = \
 ['lassen',
  'lassen.alembic',
  'lassen.assets',
  'lassen.core',
  'lassen.datasets',
  'lassen.db',
+ 'lassen.stubs',
+ 'lassen.stubs.generators',
+ 'lassen.stubs.templates',
  'lassen.tests',
  'lassen.tests.datasets',
  'lassen.tests.fixtures',
+ 'lassen.tests.fixtures.stubs',
  'lassen.tests.fixtures.test_harness.test_harness',
- 'lassen.tests.fixtures.test_harness.test_harness.migrations']
+ 'lassen.tests.fixtures.test_harness.test_harness.migrations',
+ 'lassen.tests.stubs',
+ 'lassen.tests.stubs.generators']
 
 package_data = \
 {'': ['*'], 'lassen.tests.fixtures': ['test_harness/*']}
 
 install_requires = \
-['alembic-autogenerate-enums>=0.1.1,<0.2.0',
+['Jinja2>=3.1.2,<4.0.0',
+ 'alembic-autogenerate-enums>=0.1.1,<0.2.0',
  'alembic>=1.11.1,<2.0.0',
  'click>=8.1.3,<9.0.0',
- 'fastapi>=0.96.0,<0.97.0',
+ 'fastapi>=0.95.1,<0.96.0',
  'inflection>=0.5.1,<0.6.0',
- 'pydantic>=1.10.8,<2.0.0',
+ 'pydantic>=1.10.2,<2.0.0',
  'python-dotenv>=1.0.0,<2.0.0']
 
 extras_require = \
 {'database': ['SQLAlchemy>=2.0.15,<3.0.0', 'psycopg2>=2.9.6,<3.0.0'],
  'datasets': ['datasets>=2.13.0,<3.0.0',
               'numpy>=1.24.3,<2.0.0',
               'pandas>=2.0.2,<3.0.0']}
 
 entry_points = \
-{'console_scripts': ['migrate = lassen.alembic.cli:main']}
+{'console_scripts': ['generate-lassen = lassen.stubs.generate:cli',
+                     'migrate = lassen.alembic.cli:main']}
 
 setup_kwargs = {
     'name': 'lassen',
-    'version': '0.1.3',
+    'version': '0.2.0',
     'description': 'Common webapp scaffolding.',
-    'long_description': '# lassen\n\n**40.4881° N, 121.5049° W**\n\nCore utilities for MonkeySee web applications.\n\nNot guaranteed to be backwards compatible, use at your own risk.\n\n## Structure\n\n**Stores:** Each model is expected to have its own store. Base classes that provide standard logic are provided by `lassen.store`\n- StoreBase: Base class for all stores\n- StoreFilterMixin: Mixin for filtering stores that specify an additional schema to use to filter\n\n**Datasets:** Optional huggingface `datasets` processing utilities. Only installed under the `lassen[datasets]` extra. These provide support for:\n\n- batch_to_examples: Iterate and manipulate each example separately, versus over nested key-based lists.\n- examples_to_batch: Takes the output of a typehinted element-wise batch and converts into the format needed for dataset insertion. If datasets can\'t automatically interpret the type of the fields, also provide automatic casting based on the typehinted dataclass.\n\n```python\nfrom lassen.datasets import batch_to_examples, examples_to_batch\nimport pandas as pd\n\n@dataclass\nclass BatchInsertion:\n    texts: list[str]\n\ndef batch_process(examples):\n    new_examples : list[BatchInsertion] = []\n    for example in batch_to_examples(examples):\n        new_examples.append(\n            BatchInsertion(\n                example["raw_text"].split()\n            )\n        )\n\n    # datasets won\'t be able to typehint a dataset that starts with an empty example, so we use our explicit schema to cast the data\n    return examples_to_batch(new_examples, BatchInsertion, explicit_schema=True)\n\ndf = pd.DataFrame(\n    [\n        {"raw_text": ""},\n        {"raw_text": "This is a test"},\n        {"raw_text": "This is another test"},\n    ]\n)\n\ndataset = Dataset.from_pandas(df)\n\ndataset = dataset.map(\n    batch_process,\n    batched=True,\n    batch_size=1,\n    num_proc=1,\n    remove_columns=dataset.column_names,\n)\n```\n\n**Migrations:** Lassen includes a templated alembic.init and env.py file. Client applications just need to have a `migrations` folder within their project root. After this you can swap `poetry run alembic` with `poetry run migrate`.\n\n```sh\npoetry run migrate upgrade head\n```\n\n**Settings:** Application settings should subclass our core settings. This provides a standard way to load settings from environment variables and includes common database keys.\n\n```python\nfrom lassen.core.config import CoreSettings, register_settings\n\n@register_settings\nclass ClientSettings(CoreSettings):\n    pass\n```\n\n**Schemas:** For helper schemas when returning results via API, see [lassen.schema](./lassen/schema.py).\n\n## Development\n\n```sh\npoetry install --extras "datasets"\n\ncreateuser lassen\ncreatedb -O lassen lassen_db\ncreatedb -O lassen lassen_test_db\n```\n\nUnit Tests:\n\n```sh\npoetry run pytest\n```\n',
+    'long_description': '# lassen\n\n**40.4881° N, 121.5049° W**\n\nCore utilities for MonkeySee web applications.\n\nNot guaranteed to be backwards compatible, use at your own risk.\n\n## Structure\n\n**Stores:** Each datamodel is expected to have its own store. Base classes that provide standard logic are provided by `lassen.store`\n- StoreBase: Base class for all stores\n- StoreFilterMixin: Mixin for filtering stores that specify an additional schema to use to filter\n\n**Schemas:** Each datamodel should define a Model class (SQLAlchemy base object) and a series of Schema objects (Pydantic) that allow the Store to serialize the models. These schemas are also often used for direct CRUD referencing in the API layer.\n\nWe use a base `Stub` file to generate these schemas from a centralized definition.\n\n```bash\npoetry run generate-lassen\n```\n\n**Datasets:** Optional huggingface `datasets` processing utilities. Only installed under the `lassen[datasets]` extra. These provide support for:\n\n- batch_to_examples: Iterate and manipulate each example separately, versus over nested key-based lists.\n- examples_to_batch: Takes the output of a typehinted element-wise batch and converts into the format needed for dataset insertion. If datasets can\'t automatically interpret the type of the fields, also provide automatic casting based on the typehinted dataclass.\n\n```python\nfrom lassen.datasets import batch_to_examples, examples_to_batch\nimport pandas as pd\n\n@dataclass\nclass BatchInsertion:\n    texts: list[str]\n\ndef batch_process(examples):\n    new_examples : list[BatchInsertion] = []\n    for example in batch_to_examples(examples):\n        new_examples.append(\n            BatchInsertion(\n                example["raw_text"].split()\n            )\n        )\n\n    # datasets won\'t be able to typehint a dataset that starts with an empty example, so we use our explicit schema to cast the data\n    return examples_to_batch(new_examples, BatchInsertion, explicit_schema=True)\n\ndf = pd.DataFrame(\n    [\n        {"raw_text": ""},\n        {"raw_text": "This is a test"},\n        {"raw_text": "This is another test"},\n    ]\n)\n\ndataset = Dataset.from_pandas(df)\n\ndataset = dataset.map(\n    batch_process,\n    batched=True,\n    batch_size=1,\n    num_proc=1,\n    remove_columns=dataset.column_names,\n)\n```\n\n**Migrations:** Lassen includes a templated alembic.init and env.py file. Client applications just need to have a `migrations` folder within their project root. After this you can swap `poetry run alembic` with `poetry run migrate`.\n\n```sh\npoetry run migrate upgrade head\n```\n\n**Settings:** Application settings should subclass our core settings. This provides a standard way to load settings from environment variables and includes common database keys.\n\n```python\nfrom lassen.core.config import CoreSettings, register_settings\n\n@register_settings\nclass ClientSettings(CoreSettings):\n    pass\n```\n\n**Schemas:** For helper schemas when returning results via API, see [lassen.schema](./lassen/schema.py).\n\n## Development\n\n```sh\npoetry install --extras "datasets"\n\ncreateuser lassen\ncreatedb -O lassen lassen_db\ncreatedb -O lassen lassen_test_db\n```\n\nUnit Tests:\n\n```sh\npoetry run pytest\n```\n',
     'author': 'Pierce Freeman',
     'author_email': 'pierce@freeman.vc',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.11,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `lassen-0.1.3/PKG-INFO` & `lassen-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 Metadata-Version: 2.1
 Name: lassen
-Version: 0.1.3
+Version: 0.2.0
 Summary: Common webapp scaffolding.
 Author: Pierce Freeman
 Author-email: pierce@freeman.vc
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: database
 Provides-Extra: datasets
+Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: SQLAlchemy (>=2.0.15,<3.0.0); extra == "database"
 Requires-Dist: alembic (>=1.11.1,<2.0.0)
 Requires-Dist: alembic-autogenerate-enums (>=0.1.1,<0.2.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: datasets (>=2.13.0,<3.0.0); extra == "datasets"
-Requires-Dist: fastapi (>=0.96.0,<0.97.0)
+Requires-Dist: fastapi (>=0.95.1,<0.96.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0); extra == "datasets"
 Requires-Dist: pandas (>=2.0.2,<3.0.0); extra == "datasets"
 Requires-Dist: psycopg2 (>=2.9.6,<3.0.0); extra == "database"
-Requires-Dist: pydantic (>=1.10.8,<2.0.0)
+Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # lassen
 
 **40.4881° N, 121.5049° W**
 
 Core utilities for MonkeySee web applications.
 
 Not guaranteed to be backwards compatible, use at your own risk.
 
 ## Structure
 
-**Stores:** Each model is expected to have its own store. Base classes that provide standard logic are provided by `lassen.store`
+**Stores:** Each datamodel is expected to have its own store. Base classes that provide standard logic are provided by `lassen.store`
 - StoreBase: Base class for all stores
 - StoreFilterMixin: Mixin for filtering stores that specify an additional schema to use to filter
 
+**Schemas:** Each datamodel should define a Model class (SQLAlchemy base object) and a series of Schema objects (Pydantic) that allow the Store to serialize the models. These schemas are also often used for direct CRUD referencing in the API layer.
+
+We use a base `Stub` file to generate these schemas from a centralized definition.
+
+```bash
+poetry run generate-lassen
+```
+
 **Datasets:** Optional huggingface `datasets` processing utilities. Only installed under the `lassen[datasets]` extra. These provide support for:
 
 - batch_to_examples: Iterate and manipulate each example separately, versus over nested key-based lists.
 - examples_to_batch: Takes the output of a typehinted element-wise batch and converts into the format needed for dataset insertion. If datasets can't automatically interpret the type of the fields, also provide automatic casting based on the typehinted dataclass.
 
 ```python
 from lassen.datasets import batch_to_examples, examples_to_batch
```

