# Comparing `tmp/morch-1.0.2.tar.gz` & `tmp/morch-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morch-1.0.2.tar", last modified: Thu Jul 20 12:47:13 2023, max compression
+gzip compressed data, was "morch-1.0.3.tar", last modified: Sat Jul 22 05:24:56 2023, max compression
```

## Comparing `morch-1.0.2.tar` & `morch-1.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 12:47:13.340273 morch-1.0.2/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1086 2023-06-17 07:10:20.000000 morch-1.0.2/LICENSE
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1430 2023-07-20 12:47:13.340273 morch-1.0.2/PKG-INFO
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      800 2023-07-20 12:45:57.000000 morch-1.0.2/README.md
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 12:47:13.340273 morch-1.0.2/morch/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      126 2023-06-22 12:33:56.000000 morch-1.0.2/morch/__init__.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 12:47:13.340273 morch-1.0.2/morch/helpers/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      142 2023-06-22 12:33:56.000000 morch-1.0.2/morch/helpers/__init__.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     2259 2023-06-22 12:33:56.000000 morch-1.0.2/morch/helpers/asynch.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      640 2023-06-22 12:33:56.000000 morch-1.0.2/morch/helpers/celery_utils.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     2119 2023-06-22 12:33:56.000000 morch-1.0.2/morch/helpers/handlers.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     2388 2023-07-20 12:45:57.000000 morch-1.0.2/morch/helpers/repository.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      145 2023-06-22 12:33:56.000000 morch-1.0.2/morch/helpers/status.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1007 2023-06-22 12:33:56.000000 morch-1.0.2/morch/helpers/utils.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 12:47:13.340273 morch-1.0.2/morch/saga/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       66 2023-06-22 12:33:56.000000 morch-1.0.2/morch/saga/__init__.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     3687 2023-06-22 12:33:56.000000 morch-1.0.2/morch/saga/asynch.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     5218 2023-06-22 12:33:56.000000 morch-1.0.2/morch/saga/base.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     5578 2023-07-20 06:58:40.000000 morch-1.0.2/morch/saga/stateful.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 12:47:13.340273 morch-1.0.2/morch/steps/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       62 2023-06-22 12:33:56.000000 morch-1.0.2/morch/steps/__init__.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      563 2023-06-22 12:33:56.000000 morch-1.0.2/morch/steps/asynch.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      361 2023-06-22 12:33:56.000000 morch-1.0.2/morch/steps/base.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       88 2023-06-22 12:33:56.000000 morch-1.0.2/morch/steps/sync.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 12:47:13.340273 morch-1.0.2/morch.egg-info/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1430 2023-07-20 12:47:13.000000 morch-1.0.2/morch.egg-info/PKG-INFO
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      618 2023-07-20 12:47:13.000000 morch-1.0.2/morch.egg-info/SOURCES.txt
--rw-rw-r--   0 saeed     (1000) saeed     (1000)        1 2023-07-20 12:47:13.000000 morch-1.0.2/morch.egg-info/dependency_links.txt
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      107 2023-07-20 12:47:13.000000 morch-1.0.2/morch.egg-info/requires.txt
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       12 2023-07-20 12:47:13.000000 morch-1.0.2/morch.egg-info/top_level.txt
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      656 2023-07-20 12:47:13.340273 morch-1.0.2/setup.cfg
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1327 2023-07-20 12:46:33.000000 morch-1.0.2/setup.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 12:47:13.340273 morch-1.0.2/tests/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)        0 2023-06-19 07:46:44.000000 morch-1.0.2/tests/__init__.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     6615 2023-06-22 12:33:56.000000 morch-1.0.2/tests/test_async_saga.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     2086 2023-06-22 12:33:56.000000 morch-1.0.2/tests/test_sync_saga.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-22 05:24:56.460532 morch-1.0.3/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     1086 2023-06-17 07:10:20.000000 morch-1.0.3/LICENSE
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     1430 2023-07-22 05:24:56.460532 morch-1.0.3/PKG-INFO
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      800 2023-07-20 12:45:57.000000 morch-1.0.3/README.md
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-22 05:24:56.460532 morch-1.0.3/morch/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      126 2023-06-22 12:33:56.000000 morch-1.0.3/morch/__init__.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-22 05:24:56.460532 morch-1.0.3/morch/helpers/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      142 2023-06-22 12:33:56.000000 morch-1.0.3/morch/helpers/__init__.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     2259 2023-06-22 12:33:56.000000 morch-1.0.3/morch/helpers/asynch.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      640 2023-06-22 12:33:56.000000 morch-1.0.3/morch/helpers/celery_utils.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     2119 2023-06-22 12:33:56.000000 morch-1.0.3/morch/helpers/handlers.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     2386 2023-07-22 05:24:18.000000 morch-1.0.3/morch/helpers/repository.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      145 2023-06-22 12:33:56.000000 morch-1.0.3/morch/helpers/status.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     1007 2023-06-22 12:33:56.000000 morch-1.0.3/morch/helpers/utils.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-22 05:24:56.460532 morch-1.0.3/morch/saga/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)       66 2023-06-22 12:33:56.000000 morch-1.0.3/morch/saga/__init__.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     3687 2023-06-22 12:33:56.000000 morch-1.0.3/morch/saga/asynch.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     5218 2023-06-22 12:33:56.000000 morch-1.0.3/morch/saga/base.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     5576 2023-07-22 05:24:18.000000 morch-1.0.3/morch/saga/stateful.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-22 05:24:56.460532 morch-1.0.3/morch/steps/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)       62 2023-06-22 12:33:56.000000 morch-1.0.3/morch/steps/__init__.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      563 2023-06-22 12:33:56.000000 morch-1.0.3/morch/steps/asynch.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      361 2023-06-22 12:33:56.000000 morch-1.0.3/morch/steps/base.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)       88 2023-06-22 12:33:56.000000 morch-1.0.3/morch/steps/sync.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-22 05:24:56.460532 morch-1.0.3/morch.egg-info/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     1430 2023-07-22 05:24:56.000000 morch-1.0.3/morch.egg-info/PKG-INFO
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      618 2023-07-22 05:24:56.000000 morch-1.0.3/morch.egg-info/SOURCES.txt
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)        1 2023-07-22 05:24:56.000000 morch-1.0.3/morch.egg-info/dependency_links.txt
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      107 2023-07-22 05:24:56.000000 morch-1.0.3/morch.egg-info/requires.txt
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)       12 2023-07-22 05:24:56.000000 morch-1.0.3/morch.egg-info/top_level.txt
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      656 2023-07-22 05:24:56.460532 morch-1.0.3/setup.cfg
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     1327 2023-07-22 05:24:33.000000 morch-1.0.3/setup.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-22 05:24:56.460532 morch-1.0.3/tests/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)        0 2023-06-19 07:46:44.000000 morch-1.0.3/tests/__init__.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     6615 2023-06-22 12:33:56.000000 morch-1.0.3/tests/test_async_saga.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     2086 2023-06-22 12:33:56.000000 morch-1.0.3/tests/test_sync_saga.py
```

### Comparing `morch-1.0.2/LICENSE` & `morch-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `morch-1.0.2/PKG-INFO` & `morch-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morch
-Version: 1.0.2
+Version: 1.0.3
 Summary: SAGA Python Microservice Orchestrator
 Home-page: https://github.com/hasanisaeed/morch
 Author: Saeed Hasani Borzadaran
 Author-email: hassanisaeed19@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/hasanisaeed/morch/issues/new
 Keywords: microservice,saga,patterns,microservice patterns,saga pattern
```

### Comparing `morch-1.0.2/README.md` & `morch-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `morch-1.0.2/morch/helpers/asynch.py` & `morch-1.0.3/morch/helpers/asynch.py`

 * *Files identical despite different names*

### Comparing `morch-1.0.2/morch/helpers/celery_utils.py` & `morch-1.0.3/morch/helpers/celery_utils.py`

 * *Files identical despite different names*

### Comparing `morch-1.0.2/morch/helpers/handlers.py` & `morch-1.0.3/morch/helpers/handlers.py`

 * *Files identical despite different names*

### Comparing `morch-1.0.2/morch/helpers/repository.py` & `morch-1.0.3/morch/helpers/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         # Update Saga record in saga table
         self.saga.objects.filter(pk=saga_state_filter.first().saga.id).update(status=_get_saga_status(status))
         return saga_state_filter.update(status=status)
 
     def update(self, saga_state_id: int, **fields_to_update: dict) -> object:
         return self.get_saga_state_filter(saga_state_id).update(**fields_to_update)
 
-    def create(self, **fields_to_create: dict) -> None:
+    def create(self, fields_to_create: dict) -> None:
         self.state.objects.create(**fields_to_create)
 
     def on_step_failure(self, saga_state_id: int, failed_step: BaseStep, initial_failure_payload: dict) -> object:
         return self.get_saga_state_filter(saga_state_id).update(failed_step=failed_step.name,
                                                                 failed_at=datetime.datetime.utcnow(),
                                                                 failure_details=initial_failure_payload
                                                                 )
```

### Comparing `morch-1.0.2/morch/helpers/utils.py` & `morch-1.0.3/morch/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `morch-1.0.2/morch/saga/asynch.py` & `morch-1.0.3/morch/saga/asynch.py`

 * *Files identical despite different names*

### Comparing `morch-1.0.2/morch/saga/base.py` & `morch-1.0.3/morch/saga/base.py`

 * *Files identical despite different names*

### Comparing `morch-1.0.2/morch/saga/stateful.py` & `morch-1.0.3/morch/saga/stateful.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         raise NotImplementedError
 
     @abc.abstractmethod
     def update(self, saga_id: int, **fields_to_update: dict) -> object:
         raise NotImplementedError
 
     @abc.abstractmethod
-    def create(self, **fields_to_create: dict) -> object:
+    def create(self, fields_to_create: dict) -> object:
         raise NotImplementedError
 
     @abc.abstractmethod
     def on_step_failure(self, saga_id: int, failed_step: BaseStep, initial_failure_payload: dict) -> object:
         pass
 
     @abc.abstractmethod
```

### Comparing `morch-1.0.2/morch/steps/asynch.py` & `morch-1.0.3/morch/steps/asynch.py`

 * *Files identical despite different names*

### Comparing `morch-1.0.2/morch.egg-info/PKG-INFO` & `morch-1.0.3/morch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morch
-Version: 1.0.2
+Version: 1.0.3
 Summary: SAGA Python Microservice Orchestrator
 Home-page: https://github.com/hasanisaeed/morch
 Author: Saeed Hasani Borzadaran
 Author-email: hassanisaeed19@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/hasanisaeed/morch/issues/new
 Keywords: microservice,saga,patterns,microservice patterns,saga pattern
```

### Comparing `morch-1.0.2/morch.egg-info/SOURCES.txt` & `morch-1.0.3/morch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `morch-1.0.2/setup.cfg` & `morch-1.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = morch
-version = 1.0.2
+version = 1.0.3
 author = Saeed Hasani Borzadaran
 author_email = hassanisaeed19@gmail.com
 description = Python Microservice Orchestrator
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/hasanisaeed/morch
 project_urls =
```

### Comparing `morch-1.0.2/setup.py` & `morch-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 setuptools.setup(name="morch",
-                 version="1.0.2",
+                 version="1.0.3",
                  author="Saeed Hasani Borzadaran",
                  author_email="hassanisaeed19@gmail.com",
                  description="SAGA Python Microservice Orchestrator",
                  long_description_content_type="text/markdown",
                  url="https://github.com/hasanisaeed/morch",
                  keywords='microservice, saga, patterns, microservice patterns, saga pattern',
                  python_requires='>=3.9',
```

### Comparing `morch-1.0.2/tests/test_async_saga.py` & `morch-1.0.3/tests/test_async_saga.py`

 * *Files identical despite different names*

### Comparing `morch-1.0.2/tests/test_sync_saga.py` & `morch-1.0.3/tests/test_sync_saga.py`

 * *Files identical despite different names*

