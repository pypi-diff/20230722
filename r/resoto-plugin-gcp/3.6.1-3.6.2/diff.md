# Comparing `tmp/resoto-plugin-gcp-3.6.1.tar.gz` & `tmp/resoto-plugin-gcp-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-gcp-3.6.1.tar", last modified: Fri Jul 14 17:02:09 2023, max compression
+gzip compressed data, was "resoto-plugin-gcp-3.6.2.tar", last modified: Fri Jul 21 22:18:56 2023, max compression
```

## Comparing `resoto-plugin-gcp-3.6.1.tar` & `resoto-plugin-gcp-3.6.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:02:09.617871 resoto-plugin-gcp-3.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-14 17:02:09.617871 resoto-plugin-gcp-3.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:02:09.617871 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/gcp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:02:09.617871 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25320 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)   284432 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    49819 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    40556 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:02:09.617871 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-14 17:02:09.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-14 17:02:09.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:02:09.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 17:02:09.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:57:50.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-14 17:02:09.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 17:02:09.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-14 17:02:09.621871 resoto-plugin-gcp-3.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:02:09.617871 resoto-plugin-gcp-3.6.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/random_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/test_billing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/test_sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:18:56.813373 resoto-plugin-gcp-3.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-21 22:18:56.813373 resoto-plugin-gcp-3.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:18:56.805373 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/gcp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:18:56.809373 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23211 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/resources/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)   284565 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/resources/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49819 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/resources/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40556 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/resources/sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/resources/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:18:56.809373 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-21 22:18:56.000000 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-21 22:18:56.000000 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:18:56.000000 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 22:18:56.000000 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:13:34.000000 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-21 22:18:56.000000 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 22:18:56.000000 resoto-plugin-gcp-3.6.2/resoto_plugin_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-21 22:18:56.813373 resoto-plugin-gcp-3.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:18:56.813373 resoto-plugin-gcp-3.6.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/test/random_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/test/test_billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/test/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/test/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/test/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/test/test_sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-21 22:11:55.000000 resoto-plugin-gcp-3.6.2/test/test_storage.py
```

### Comparing `resoto-plugin-gcp-3.6.1/PKG-INFO` & `resoto-plugin-gcp-3.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.6.1
+Version: 3.6.2
 Summary: Resoto GCP Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/gcp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-gcp-3.6.1/pyproject.toml` & `resoto-plugin-gcp-3.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-gcp"
 description = "Resoto GCP Collector Plugin"
-version = "3.6.1"
+version = "3.6.2"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.6.1",
+    "resotolib==3.6.2",
     "google-api-python-client",
     "oauth2client",
     "retrying",
     "tenacity",
 ]
 
 [project.entry-points."resoto.plugins"]
```

### Comparing `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/__init__.py` & `resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/collector.py` & `resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/config.py` & `resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/gcp_client.py` & `resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/gcp_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/base.py` & `resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/resources/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
-import concurrent
 import json
 import logging
-from concurrent.futures import Executor, Future
+from concurrent.futures import Future
 from threading import Lock
 from types import TracebackType
 from typing import Callable, List, ClassVar, Optional, TypeVar, Type, Any, Dict, Set
 
 from attr import define, field
 from google.auth.credentials import Credentials as GoogleAuthCredentials
 from googleapiclient.errors import HttpError
@@ -24,14 +23,15 @@
     ModelReference,
 )
 from resotolib.config import Config
 from resotolib.core.actions import CoreFeedback
 from resotolib.graph import Graph, EdgeKey
 from resotolib.json import from_json as from_js, value_in_path
 from resotolib.json_bender import bend, Bender, S, Bend, MapDict, F
+from resotolib.threading import ExecutorQueue
 from resotolib.types import Json
 
 log = logging.getLogger("resoto.plugins.gcp")
 
 
 T = TypeVar("T")
 
@@ -42,76 +42,14 @@
     return GcpClient(
         Credentials.get(project.id),
         project_id=project.id,
         region=resource.region().name if resource.region() else None,
     )
 
 
-class CancelOnFirstError(Exception):
-    pass
-
-
-@define
-class ExecutorQueue:
-    executor: Executor
-    name: str
-    fail_on_first_exception: bool = False
-    futures: List[Future[Any]] = field(factory=list)
-    _lock: Lock = Lock()
-    _exception: Optional[Exception] = None
-
-    def submit_work(self, fn: Callable[..., T], *args: Any, **kwargs: Any) -> Future[T]:
-        def do_work() -> T:
-            # in case of exception let's fail fast and do not execute the function
-            if self._exception is None:
-                try:
-                    return fn(*args, **kwargs)
-                except Exception as e:
-                    # only store the first exception if we should fail on first future
-                    if self._exception is None:
-                        self._exception = e
-                    raise e
-            else:
-                raise CancelOnFirstError(
-                    "Exception happened in another thread. Do not start work."
-                ) from self._exception
-
-        future = (
-            self.executor.submit(do_work) if self.fail_on_first_exception else self.executor.submit(fn, *args, **kwargs)
-        )
-
-        with self._lock:
-            self.futures.append(future)
-        return future
-
-    def wait_for_submitted_work(self) -> None:
-        def _wait_for_current_batch() -> None:
-            # wait until all futures are complete
-            with self._lock:
-                to_wait = self.futures
-                self.futures = []
-            for future in concurrent.futures.as_completed(to_wait):
-                try:
-                    future.result()
-                except CancelOnFirstError:
-                    pass
-                except Exception as ex:
-                    log.exception(f"Unhandled exception in project {self.name}: {ex}")
-                    raise
-
-        # Wait until all submitted work and their potential "children" work is done
-        with self._lock:
-            remaining = len(self.futures)
-
-        while not remaining == 0:
-            _wait_for_current_batch()
-            with self._lock:
-                remaining = len(self.futures)
-
-
 class GraphBuilder:
     def __init__(
         self,
         graph: Graph,
         cloud: Cloud,
         project: GcpProject,
         credentials: GoogleAuthCredentials,
@@ -140,15 +78,15 @@
         self.graph_edges_access = graph_edges_access or Lock()
 
     def submit_work(self, fn: Callable[..., T], *args: Any, **kwargs: Any) -> Future[T]:
         """
         Use this method for work that can be done in parallel.
         Example: fetching tags of a resource.
         """
-        return self.executor.submit_work(fn, *args, **kwargs)
+        return self.executor.submit_work(self.project.id, fn, *args, **kwargs)
 
     def prepare_region_zone_lookup(self) -> None:
         regions = self.resources_of(GcpRegion)
         zns = self.resources_of(GcpZone)
         self.region_by_name = {r.safe_name: r for r in regions}
         self.region_by_zone_name = {z.safe_name: self.region_by_name[z.safe_name.rsplit("-", 1)[0]] for z in zns}
         self.zone_by_name = {z.safe_name: z for z in zns}
```

### Comparing `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/billing.py` & `resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/resources/billing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/compute.py` & `resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/resources/compute.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     BaseVolumeType,
     ModelReference,
     BaseVolume,
     VolumeStatus,
     BaseInstance,
     InstanceStatus,
 )
-from resotolib.json_bender import Bender, S, Bend, ForallBend, MapDict, F, MapEnum
+from resotolib.json_bender import Bender, S, Bend, ForallBend, MapDict, F, MapEnum, AsInt
 from resotolib.types import Json
 
 log = logging.getLogger("resoto.plugins.gcp")
 
 
 # This service is called Compute Engine in the GCP API.
 # https://cloud.google.com/kubernetes-engine/docs
@@ -769,18 +769,18 @@
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
-        "default_disk_size_gb": S("defaultDiskSizeGb"),
+        "default_disk_size_gb": S("defaultDiskSizeGb") >> AsInt(),
         "valid_disk_size": S("validDiskSize"),
     }
-    default_disk_size_gb: Optional[str] = field(default=None)
+    default_disk_size_gb: Optional[int] = field(default=None)
     valid_disk_size: Optional[str] = field(default=None)
 
     resource_group_map: ClassVar[Dict[str, str]] = {
         "local-ssd": "LocalSSD",
         "pd-balanced": "SSD",
         "pd-ssd": "SSD",
         "pd-standard": "PDStandard",
@@ -889,15 +889,15 @@
         "last_detach_timestamp": S("lastDetachTimestamp"),
         "license_codes": S("licenseCodes", default=[]),
         "licenses": S("licenses", default=[]),
         "location_hint": S("locationHint"),
         "options": S("options"),
         "disk_params": S("params", default={}) >> Bend(GcpDiskParams.mapping),
         "physical_block_size_bytes": S("physicalBlockSizeBytes"),
-        "provisioned_iops": S("provisionedIops"),
+        "provisioned_iops": S("provisionedIops") >> AsInt(),
         "replica_zones": S("replicaZones", default=[]),
         "resource_policies": S("resourcePolicies", default=[]),
         "satisfies_pzs": S("satisfiesPzs"),
         "size_gb": S("sizeGb"),
         "source_disk": S("sourceDisk"),
         "source_disk_id": S("sourceDiskId"),
         "source_image": S("sourceImage"),
@@ -937,15 +937,15 @@
     last_detach_timestamp: Optional[datetime] = field(default=None)
     license_codes: Optional[List[str]] = field(default=None)
     licenses: Optional[List[str]] = field(default=None)
     location_hint: Optional[str] = field(default=None)
     options: Optional[str] = field(default=None)
     disk_params: Optional[GcpDiskParams] = field(default=None)
     physical_block_size_bytes: Optional[str] = field(default=None)
-    provisioned_iops: Optional[str] = field(default=None)
+    provisioned_iops: Optional[int] = field(default=None)
     replica_zones: Optional[List[str]] = field(default=None)
     resource_policies: Optional[List[str]] = field(default=None)
     satisfies_pzs: Optional[bool] = field(default=None)
     size_gb: Optional[str] = field(default=None)
     source_disk: Optional[str] = field(default=None)
     source_disk_id: Optional[str] = field(default=None)
     source_image: Optional[str] = field(default=None)
@@ -1964,15 +1964,15 @@
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "architecture": S("architecture"),
         "archive_size_bytes": S("archiveSizeBytes"),
-        "disk_size_gb": S("diskSizeGb"),
+        "disk_size_gb": S("diskSizeGb") >> AsInt(),
         "family": S("family"),
         "guest_os_features": S("guestOsFeatures", default=[]) >> ForallBend(S("type")),
         "image_encryption_key": S("imageEncryptionKey", default={}) >> Bend(GcpCustomerEncryptionKey.mapping),
         "license_codes": S("licenseCodes", default=[]),
         "licenses": S("licenses", default=[]),
         "raw_disk": S("rawDisk", default={}) >> Bend(GcpRawdisk.mapping),
         "satisfies_pzs": S("satisfiesPzs"),
@@ -1992,15 +1992,15 @@
         "source_snapshot_id": S("sourceSnapshotId"),
         "source_type": S("sourceType"),
         "status": S("status"),
         "storage_locations": S("storageLocations", default=[]),
     }
     architecture: Optional[str] = field(default=None)
     archive_size_bytes: Optional[str] = field(default=None)
-    disk_size_gb: Optional[str] = field(default=None)
+    disk_size_gb: Optional[int] = field(default=None)
     family: Optional[str] = field(default=None)
     guest_os_features: Optional[List[str]] = field(default=None)
     image_encryption_key: Optional[GcpCustomerEncryptionKey] = field(default=None)
     license_codes: Optional[List[str]] = field(default=None)
     licenses: Optional[List[str]] = field(default=None)
     raw_disk: Optional[GcpRawdisk] = field(default=None)
     satisfies_pzs: Optional[bool] = field(default=None)
@@ -2313,38 +2313,38 @@
 @define(eq=False, slots=False)
 class GcpAttachedDiskInitializeParams:
     kind: ClassVar[str] = "gcp_attached_disk_initialize_params"
     mapping: ClassVar[Dict[str, Bender]] = {
         "architecture": S("architecture"),
         "description": S("description"),
         "disk_name": S("diskName"),
-        "disk_size_gb": S("diskSizeGb"),
+        "disk_size_gb": S("diskSizeGb") >> AsInt(),
         "disk_type": S("diskType"),
         "labels": S("labels"),
         "licenses": S("licenses", default=[]),
         "on_update_action": S("onUpdateAction"),
-        "provisioned_iops": S("provisionedIops"),
+        "provisioned_iops": S("provisionedIops") >> AsInt(),
         "resource_manager_tags": S("resourceManagerTags"),
         "resource_policies": S("resourcePolicies", default=[]),
         "source_image": S("sourceImage"),
         "source_image_encryption_key": S("sourceImageEncryptionKey", default={})
         >> Bend(GcpCustomerEncryptionKey.mapping),
         "source_snapshot": S("sourceSnapshot"),
         "source_snapshot_encryption_key": S("sourceSnapshotEncryptionKey", default={})
         >> Bend(GcpCustomerEncryptionKey.mapping),
     }
     architecture: Optional[str] = field(default=None)
     description: Optional[str] = field(default=None)
     disk_name: Optional[str] = field(default=None)
-    disk_size_gb: Optional[str] = field(default=None)
+    disk_size_gb: Optional[int] = field(default=None)
     disk_type: Optional[str] = field(default=None)
     labels: Optional[Dict[str, str]] = field(default=None)
     licenses: Optional[List[str]] = field(default=None)
     on_update_action: Optional[str] = field(default=None)
-    provisioned_iops: Optional[str] = field(default=None)
+    provisioned_iops: Optional[int] = field(default=None)
     resource_manager_tags: Optional[Dict[str, str]] = field(default=None)
     resource_policies: Optional[List[str]] = field(default=None)
     source_image: Optional[str] = field(default=None)
     source_image_encryption_key: Optional[GcpCustomerEncryptionKey] = field(default=None)
     source_snapshot: Optional[str] = field(default=None)
     source_snapshot_encryption_key: Optional[GcpCustomerEncryptionKey] = field(default=None)
 
@@ -2354,15 +2354,15 @@
     kind: ClassVar[str] = "gcp_attached_disk"
     mapping: ClassVar[Dict[str, Bender]] = {
         "architecture": S("architecture"),
         "auto_delete": S("autoDelete"),
         "boot": S("boot"),
         "device_name": S("deviceName"),
         "disk_encryption_key": S("diskEncryptionKey", default={}) >> Bend(GcpCustomerEncryptionKey.mapping),
-        "disk_size_gb": S("diskSizeGb"),
+        "disk_size_gb": S("diskSizeGb") >> AsInt(),
         "force_attach": S("forceAttach"),
         "guest_os_features": S("guestOsFeatures", default=[]) >> ForallBend(S("type")),
         "index": S("index"),
         "initialize_params": S("initializeParams", default={}) >> Bend(GcpAttachedDiskInitializeParams.mapping),
         "interface": S("interface"),
         "licenses": S("licenses", default=[]),
         "mode": S("mode"),
@@ -2372,15 +2372,15 @@
         "type": S("type"),
     }
     architecture: Optional[str] = field(default=None)
     auto_delete: Optional[bool] = field(default=None)
     boot: Optional[bool] = field(default=None)
     device_name: Optional[str] = field(default=None)
     disk_encryption_key: Optional[GcpCustomerEncryptionKey] = field(default=None)
-    disk_size_gb: Optional[str] = field(default=None)
+    disk_size_gb: Optional[int] = field(default=None)
     force_attach: Optional[bool] = field(default=None)
     guest_os_features: Optional[List[str]] = field(default=None)
     index: Optional[int] = field(default=None)
     initialize_params: Optional[GcpAttachedDiskInitializeParams] = field(default=None)
     interface: Optional[str] = field(default=None)
     licenses: Optional[List[str]] = field(default=None)
     mode: Optional[str] = field(default=None)
@@ -2660,24 +2660,24 @@
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
-        "properties": S("properties", default={}) >> Bend(GcpInstanceProperties.mapping),
+        "template_properties": S("properties", default={}) >> Bend(GcpInstanceProperties.mapping),
         "source_instance": S("sourceInstance"),
         "source_instance_params": S("sourceInstanceParams", default={}) >> Bend(GcpSourceInstanceParams.mapping),
     }
-    properties: Optional[GcpInstanceProperties] = field(default=None)
+    template_properties: Optional[GcpInstanceProperties] = field(default=None)
     source_instance: Optional[str] = field(default=None)
     source_instance_params: Optional[GcpSourceInstanceParams] = field(default=None)
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
-        if p := self.properties:
+        if p := self.template_properties:
             if p.machine_type:
                 builder.add_edge(self, reverse=True, clazz=GcpMachineType, link=p.machine_type)
 
 
 @define(eq=False, slots=False)
 class GcpInstanceParams:
     kind: ClassVar[str] = "gcp_instance_params"
@@ -3182,15 +3182,15 @@
 class GcpSavedAttachedDisk:
     kind: ClassVar[str] = "gcp_saved_attached_disk"
     mapping: ClassVar[Dict[str, Bender]] = {
         "auto_delete": S("autoDelete"),
         "boot": S("boot"),
         "device_name": S("deviceName"),
         "disk_encryption_key": S("diskEncryptionKey", default={}) >> Bend(GcpCustomerEncryptionKey.mapping),
-        "disk_size_gb": S("diskSizeGb"),
+        "disk_size_gb": S("diskSizeGb") >> AsInt(),
         "disk_type": S("diskType"),
         "guest_os_features": S("guestOsFeatures", default=[]) >> ForallBend(S("type")),
         "index": S("index"),
         "interface": S("interface"),
         "licenses": S("licenses", default=[]),
         "mode": S("mode"),
         "source": S("source"),
@@ -3198,15 +3198,15 @@
         "storage_bytes_status": S("storageBytesStatus"),
         "type": S("type"),
     }
     auto_delete: Optional[bool] = field(default=None)
     boot: Optional[bool] = field(default=None)
     device_name: Optional[str] = field(default=None)
     disk_encryption_key: Optional[GcpCustomerEncryptionKey] = field(default=None)
-    disk_size_gb: Optional[str] = field(default=None)
+    disk_size_gb: Optional[int] = field(default=None)
     disk_type: Optional[str] = field(default=None)
     guest_os_features: Optional[List[str]] = field(default=None)
     index: Optional[int] = field(default=None)
     interface: Optional[str] = field(default=None)
     licenses: Optional[List[str]] = field(default=None)
     mode: Optional[str] = field(default=None)
     source: Optional[str] = field(default=None)
@@ -3983,16 +3983,16 @@
     cores_per_license: Optional[str] = field(default=None)
     license: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpAllocationSpecificSKUAllocationAllocatedInstancePropertiesReservedDisk:
     kind: ClassVar[str] = "gcp_allocation_specific_sku_allocation_allocated_instance_properties_reserved_disk"
-    mapping: ClassVar[Dict[str, Bender]] = {"disk_size_gb": S("diskSizeGb"), "interface": S("interface")}
-    disk_size_gb: Optional[str] = field(default=None)
+    mapping: ClassVar[Dict[str, Bender]] = {"disk_size_gb": S("diskSizeGb") >> AsInt(), "interface": S("interface")}
+    disk_size_gb: Optional[int] = field(default=None)
     interface: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpAllocationSpecificSKUAllocationReservedInstanceProperties:
     kind: ClassVar[str] = "gcp_allocation_specific_sku_allocation_reserved_instance_properties"
     mapping: ClassVar[Dict[str, Bender]] = {
@@ -5651,15 +5651,15 @@
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "snapshot_architecture": S("architecture"),
         "snapshot_auto_created": S("autoCreated"),
         "snapshot_chain_name": S("chainName"),
         "snapshot_creation_size_bytes": S("creationSizeBytes"),
-        "snapshot_disk_size_gb": S("diskSizeGb"),
+        "snapshot_disk_size_gb": S("diskSizeGb") >> AsInt(),
         "snapshot_download_bytes": S("downloadBytes"),
         "snapshot_license_codes": S("licenseCodes", default=[]),
         "snapshot_licenses": S("licenses", default=[]),
         "snapshot_location_hint": S("locationHint"),
         "snapshot_satisfies_pzs": S("satisfiesPzs"),
         "snapshot_snapshot_encryption_key": S("snapshotEncryptionKey", default={})
         >> Bend(GcpCustomerEncryptionKey.mapping),
@@ -5675,15 +5675,15 @@
         "snapshot_storage_bytes_status": S("storageBytesStatus"),
         "snapshot_storage_locations": S("storageLocations", default=[]),
     }
     snapshot_architecture: Optional[str] = field(default=None)
     snapshot_auto_created: Optional[bool] = field(default=None)
     snapshot_chain_name: Optional[str] = field(default=None)
     snapshot_creation_size_bytes: Optional[str] = field(default=None)
-    snapshot_disk_size_gb: Optional[str] = field(default=None)
+    snapshot_disk_size_gb: Optional[int] = field(default=None)
     snapshot_download_bytes: Optional[str] = field(default=None)
     snapshot_license_codes: Optional[List[str]] = field(default=None)
     snapshot_licenses: Optional[List[str]] = field(default=None)
     snapshot_location_hint: Optional[str] = field(default=None)
     snapshot_satisfies_pzs: Optional[bool] = field(default=None)
     snapshot_snapshot_encryption_key: Optional[GcpCustomerEncryptionKey] = field(default=None)
     snapshot_snapshot_type: Optional[str] = field(default=None)
```

### Comparing `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/container.py` & `resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/resources/container.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/sqladmin.py` & `resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/resources/sqladmin.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/storage.py` & `resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/resources/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 @define(eq=False, slots=False)
 class GcpAutoclass:
     kind: ClassVar[str] = "gcp_autoclass"
     mapping: ClassVar[Dict[str, Bender]] = {"enabled": S("enabled"), "toggle_time": S("toggleTime")}
     enabled: Optional[bool] = field(default=None)
-    toggle_time: Optional[str] = field(default=None)
+    toggle_time: Optional[datetime] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpCors:
     kind: ClassVar[str] = "gcp_cors"
     mapping: ClassVar[Dict[str, Bender]] = {
         "max_age_seconds": S("maxAgeSeconds"),
@@ -103,23 +103,23 @@
 
 
 @define(eq=False, slots=False)
 class GcpBucketpolicyonly:
     kind: ClassVar[str] = "gcp_bucketpolicyonly"
     mapping: ClassVar[Dict[str, Bender]] = {"enabled": S("enabled"), "locked_time": S("lockedTime")}
     enabled: Optional[bool] = field(default=None)
-    locked_time: Optional[str] = field(default=None)
+    locked_time: Optional[datetime] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpUniformbucketlevelaccess:
     kind: ClassVar[str] = "gcp_uniformbucketlevelaccess"
     mapping: ClassVar[Dict[str, Bender]] = {"enabled": S("enabled"), "locked_time": S("lockedTime")}
     enabled: Optional[bool] = field(default=None)
-    locked_time: Optional[str] = field(default=None)
+    locked_time: Optional[datetime] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpIamconfiguration:
     kind: ClassVar[str] = "gcp_iamconfiguration"
     mapping: ClassVar[Dict[str, Bender]] = {
         "bucket_policy_only": S("bucketPolicyOnly", default={}) >> Bend(GcpBucketpolicyonly.mapping),
@@ -202,15 +202,15 @@
 class GcpRetentionpolicy:
     kind: ClassVar[str] = "gcp_retentionpolicy"
     mapping: ClassVar[Dict[str, Bender]] = {
         "effective_time": S("effectiveTime"),
         "is_locked": S("isLocked"),
         "retention_period": S("retentionPeriod"),
     }
-    effective_time: Optional[str] = field(default=None)
+    effective_time: Optional[datetime] = field(default=None)
     is_locked: Optional[bool] = field(default=None)
     retention_period: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpWebsite:
     kind: ClassVar[str] = "gcp_website"
@@ -260,14 +260,15 @@
         mutate_iam_permissions=["storage.buckets.update", "storage.buckets.delete"],
     )
     mapping: ClassVar[Dict[str, Bender]] = {
         "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
+        "mtime": S("updated"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "acl": S("acl", default=[]) >> ForallBend(GcpBucketAccessControl.mapping),
         "autoclass": S("autoclass", default={}) >> Bend(GcpAutoclass.mapping),
         "requester_pays": S("billing", "requesterPays"),
@@ -309,16 +310,16 @@
     metageneration: Optional[str] = field(default=None)
     bucket_owner: Optional[GcpOwner] = field(default=None)
     project_number: Optional[str] = field(default=None)
     retention_policy: Optional[GcpRetentionpolicy] = field(default=None)
     rpo: Optional[str] = field(default=None)
     satisfies_pzs: Optional[bool] = field(default=None)
     storage_class: Optional[str] = field(default=None)
-    time_created: Optional[str] = field(default=None)
-    updated: Optional[str] = field(default=None)
+    time_created: Optional[datetime] = field(default=None)
+    updated: Optional[datetime] = field(default=None)
     bucket_website: Optional[GcpWebsite] = field(default=None)
     requester_pays: Optional[bool] = field(default=None)
     versioning_enabled: Optional[bool] = field(default=None)
     lifecycle_rule: List[GcpRule] = field(factory=list)
 
     def pre_delete(self, graph: Graph) -> bool:
         client = get_client(self)
```

### Comparing `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/utils.py` & `resoto-plugin-gcp-3.6.2/resoto_plugin_gcp/utils.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/PKG-INFO` & `resoto-plugin-gcp-3.6.2/resoto_plugin_gcp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.6.1
+Version: 3.6.2
 Summary: Resoto GCP Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/gcp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/SOURCES.txt` & `resoto-plugin-gcp-3.6.2/resoto_plugin_gcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.1/test/conftest.py` & `resoto-plugin-gcp-3.6.2/test/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,43 @@
-from concurrent.futures import Executor, Future
+from concurrent.futures import ThreadPoolExecutor
 from queue import Queue
-from typing import Any, Callable, Iterator
+from typing import Iterator
 
 from google.auth.credentials import AnonymousCredentials
 from googleapiclient import discovery
 from pytest import fixture
 
 from resoto_plugin_gcp import gcp_client
 from resoto_plugin_gcp.config import GcpConfig
-from resoto_plugin_gcp.resources.base import ExecutorQueue, GcpRegion, GraphBuilder, GcpProject
+from resoto_plugin_gcp.resources.base import GcpRegion, GraphBuilder, GcpProject
 from resotolib.baseresources import Cloud
 from resotolib.config import Config
 from resotolib.core.actions import CoreFeedback
 from resotolib.graph import Graph
+from resotolib.threading import ExecutorQueue
 from .random_client import build_random_data_client, random_predefined
 
 
-class DummyExecutor(Executor):
-    def submit(self, fn: Callable[..., Any], *args: Any, **kwargs: Any) -> Future[Any]:  # type: ignore
-        result = fn(*args, **kwargs)
-        f: Future[Any] = Future()
-        f.set_result(result)
-        return f
-
-
 @fixture
 def random_builder() -> Iterator[GraphBuilder]:
-    # Initialise config
-    Config.add_config(GcpConfig)
-    Config.init_default_config()
-    # change discovery function factory for tests
-    gcp_client._discovery_function = build_random_data_client
-    queue = ExecutorQueue(DummyExecutor(), "dummy")
-    feedback = CoreFeedback("test", "test", "test", Queue())
-    project = GcpProject(id="test")
-    project_global_region = GcpRegion.fallback_global_region(project)
-    builder = GraphBuilder(
-        Graph(), Cloud(id="gcp"), project, AnonymousCredentials(), queue, feedback, project_global_region
-    )
-    builder.add_node(project_global_region, {})
-    # add predefined regions and zones
-    for predefined in random_predefined:
-        builder.add_node(predefined)
-    builder.prepare_region_zone_lookup()
-    # provide the builder to the test method
-    yield builder
-    # rest the original discovery function
-    gcp_client._discovery_function = discovery.build
+    with ThreadPoolExecutor(1) as executor:
+        # Initialise config
+        Config.add_config(GcpConfig)
+        Config.init_default_config()
+        # change discovery function factory for tests
+        gcp_client._discovery_function = build_random_data_client
+        queue = ExecutorQueue(executor, "dummy")
+        feedback = CoreFeedback("test", "test", "test", Queue())
+        project = GcpProject(id="test")
+        project_global_region = GcpRegion.fallback_global_region(project)
+        builder = GraphBuilder(
+            Graph(), Cloud(id="gcp"), project, AnonymousCredentials(), queue, feedback, project_global_region
+        )
+        builder.add_node(project_global_region, {})
+        # add predefined regions and zones
+        for predefined in random_predefined:
+            builder.add_node(predefined)
+        builder.prepare_region_zone_lookup()
+        # provide the builder to the test method
+        yield builder
+        # rest the original discovery function
+        gcp_client._discovery_function = discovery.build
```

### Comparing `resoto-plugin-gcp-3.6.1/test/random_client.py` & `resoto-plugin-gcp-3.6.2/test/random_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,19 @@
                 keys = PredefinedDictKeys.get(path, [random_string() for _ in range(random_int(1, 3))])
                 return {key: value_for(schema["additionalProperties"], level + 1, f"{path}.{key}") for key in keys}
             elif schema["type"] == "array":
                 count = random_int(1, 3)
                 return [value_for(schema["items"], level + 1, f"{path}[]") for _ in range(count)]
             elif schema["type"] == "string" and "enum" in schema:
                 return random_choice(schema["enum"])  # type: ignore
-            elif schema["type"] == "string" and "in RFC3339 text format" in schema.get("description", ""):
+            elif schema["type"] == "string" and (
+                schema.get("format") == "date-time"
+                or schema.get("format") == "google-datetime"
+                or "in RFC3339 text format" in schema.get("description", "")
+            ):
                 return random_datetime()
             elif schema["type"] == "string" and "URL" in schema.get("description", ""):
                 return f"https://example.{random_string()}.{random_choice(['com', 'org', 'net'])}"
             elif schema["type"] == "string" and "IPv4" in schema.get("description", ""):
                 return random_ipv4()
             elif schema["type"] == "string" and "int" in schema.get("format", ""):
                 return str(random_int())
```

### Comparing `resoto-plugin-gcp-3.6.1/test/test_base.py` & `resoto-plugin-gcp-3.6.2/test/test_base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.1/test/test_billing.py` & `resoto-plugin-gcp-3.6.2/test/test_billing.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,10 +18,11 @@
     SERVICE_NAME = "Compute Engine"
     fixture_replies = {
         "Service": {"serviceId": lambda: SERVICE_ID, "displayName": lambda: SERVICE_NAME},
         "Sku": {"name": lambda: SERVICE_ID},
     }
     with FixturedClient(random_builder, fixture_replies) as random_builder:
         services = GcpService.collect_resources(random_builder)
+        random_builder.executor.wait_for_submitted_work()
         for service in services:
             service.connect_in_graph(random_builder, {"Dummy": "Source"})
         assert len(random_builder.edges_of(GcpService, GcpSku)) > 0
```

### Comparing `resoto-plugin-gcp-3.6.1/test/test_collector.py` & `resoto-plugin-gcp-3.6.2/test/test_collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.1/test/test_compute.py` & `resoto-plugin-gcp-3.6.2/test/test_compute.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 
     for price in known_prices_per_gig:
         region = next((obj for obj in regions if obj.id == price[1]), None)
         disk_type = next((obj for obj in disk_types if obj.name == price[0]), None)
         assert disk_type
         disk_type._region = region
         disk_type.connect_in_graph(random_builder, {"Dummy": "Source"})
+        assert disk_type.ondemand_cost is not None
         assert disk_type.ondemand_cost > 0.0
         assert round(disk_type.ondemand_cost, 5) == price[2]
 
 
 def test_gcp_disk(random_builder: GraphBuilder) -> None:
     disk = roundtrip(GcpDisk, random_builder)
     connect_resource(random_builder, disk, GcpDiskType, selfLink=disk.volume_type)
@@ -150,14 +151,15 @@
         "Instance": {"machineType": lambda: CUSTOM_MACHINE_TYPE_PART},
         "MachineType": {"selfLink": lambda: CUSTOM_MACHINE_TYPE_FULL},
     }
     assert len(random_builder.resources_of(GcpMachineType)) == 0
 
     with FixturedClient(random_builder, fixture_replies) as random_builder:
         res: List[GcpInstance] = GcpInstance.collect_resources(random_builder)  # type: ignore
+        random_builder.executor.wait_for_submitted_work()
         for node, data in random_builder.graph.nodes(data=True):
             node.connect_in_graph(random_builder, data.get("source") or {})
         first_instance: GcpInstance = res[0]
 
     assert len(random_builder.resources_of(GcpMachineType)) == 1
     only_machine_type = random_builder.resources_of(GcpMachineType)[0]
     assert first_instance.instance_cores == only_machine_type.instance_cores
```

### Comparing `resoto-plugin-gcp-3.6.1/test/test_config.py` & `resoto-plugin-gcp-3.6.2/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.1/test/test_container.py` & `resoto-plugin-gcp-3.6.2/test/test_container.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.1/test/test_sqladmin.py` & `resoto-plugin-gcp-3.6.2/test/test_sqladmin.py`

 * *Files identical despite different names*

