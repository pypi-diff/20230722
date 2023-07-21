# Comparing `tmp/resotoworker-3.6.1.tar.gz` & `tmp/resotoworker-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoworker-3.6.1.tar", last modified: Fri Jul 14 17:02:11 2023, max compression
+gzip compressed data, was "resotoworker-3.6.2.tar", last modified: Fri Jul 21 22:16:17 2023, max compression
```

## Comparing `resotoworker-3.6.1.tar` & `resotoworker-3.6.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:02:10.993684 resotoworker-3.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 16:56:59.000000 resotoworker-3.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-14 17:02:10.993684 resotoworker-3.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-14 16:56:59.000000 resotoworker-3.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-14 16:56:59.000000 resotoworker-3.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:02:10.993684 resotoworker-3.6.1/resotoworker/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/pluginloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:02:10.993684 resotoworker-3.6.1/resotoworker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-14 17:02:10.000000 resotoworker-3.6.1/resotoworker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-14 17:02:10.000000 resotoworker-3.6.1/resotoworker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:02:10.000000 resotoworker-3.6.1/resotoworker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 17:02:10.000000 resotoworker-3.6.1/resotoworker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:58:37.000000 resotoworker-3.6.1/resotoworker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-14 17:02:10.000000 resotoworker-3.6.1/resotoworker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 17:02:10.000000 resotoworker-3.6.1/resotoworker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-14 17:02:10.993684 resotoworker-3.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:02:10.993684 resotoworker-3.6.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:56:59.000000 resotoworker-3.6.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-14 16:56:59.000000 resotoworker-3.6.1/test/fakeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-14 16:56:59.000000 resotoworker-3.6.1/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-14 16:56:59.000000 resotoworker-3.6.1/test/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-14 16:56:59.000000 resotoworker-3.6.1/test/test_resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-14 16:56:59.000000 resotoworker-3.6.1/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:16:17.538173 resotoworker-3.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 22:11:13.000000 resotoworker-3.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-21 22:16:17.538173 resotoworker-3.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-21 22:11:13.000000 resotoworker-3.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-21 22:11:13.000000 resotoworker-3.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:16:17.534173 resotoworker-3.6.2/resotoworker/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-21 22:11:13.000000 resotoworker-3.6.2/resotoworker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-07-21 22:11:13.000000 resotoworker-3.6.2/resotoworker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-21 22:11:13.000000 resotoworker-3.6.2/resotoworker/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-07-21 22:11:13.000000 resotoworker-3.6.2/resotoworker/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-21 22:11:13.000000 resotoworker-3.6.2/resotoworker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-21 22:11:13.000000 resotoworker-3.6.2/resotoworker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-21 22:11:13.000000 resotoworker-3.6.2/resotoworker/pluginloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-07-21 22:11:13.000000 resotoworker-3.6.2/resotoworker/resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-21 22:11:13.000000 resotoworker-3.6.2/resotoworker/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-21 22:11:13.000000 resotoworker-3.6.2/resotoworker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:16:17.534173 resotoworker-3.6.2/resotoworker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-21 22:16:17.000000 resotoworker-3.6.2/resotoworker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-21 22:16:17.000000 resotoworker-3.6.2/resotoworker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:16:17.000000 resotoworker-3.6.2/resotoworker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 22:16:17.000000 resotoworker-3.6.2/resotoworker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:12:43.000000 resotoworker-3.6.2/resotoworker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-21 22:16:17.000000 resotoworker-3.6.2/resotoworker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 22:16:17.000000 resotoworker-3.6.2/resotoworker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 22:16:17.538173 resotoworker-3.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:16:17.538173 resotoworker-3.6.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:11:13.000000 resotoworker-3.6.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-21 22:11:13.000000 resotoworker-3.6.2/test/fakeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-21 22:11:13.000000 resotoworker-3.6.2/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-21 22:11:13.000000 resotoworker-3.6.2/test/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-21 22:11:13.000000 resotoworker-3.6.2/test/test_resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-21 22:11:13.000000 resotoworker-3.6.2/test/test_utils.py
```

### Comparing `resotoworker-3.6.1/PKG-INFO` & `resotoworker-3.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.6.1
+Version: 3.6.2
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoworker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `resotoworker-3.6.1/README.md` & `resotoworker-3.6.2/README.md`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.1/pyproject.toml` & `resotoworker-3.6.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "resotoworker"
-version = "3.6.1"
+version = "3.6.2"
 authors = [{name="Some Engineering Inc."}]
 description = "Runs collector plugins and sends the result to resotocore."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [ "Programming Language :: Python :: 3" ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.6.1",
+    "resotolib==3.6.2",
     "tenacity",
     "CherryPy",
 ]
 
 [project.scripts]
 resotoworker = "resotoworker.__main__:main"
```

### Comparing `resotoworker-3.6.1/resotoworker/__main__.py` & `resotoworker-3.6.2/resotoworker/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-import multiprocessing
 import os
 import sys
 import threading
+import multiprocessing
 import cherrypy  # type: ignore
 import time
+import requests
+import resotolib.proc
 from functools import partial
 from queue import Queue
 from signal import SIGTERM
 from typing import List, Dict, Type, Optional, Any, Callable
-
-import requests
-
-import resotolib.proc
+from multiprocessing.managers import SyncManager
 from resotolib.args import ArgumentParser
 from resotolib.baseplugin import BaseActionPlugin, BaseCollectorPlugin, PluginType
 from resotolib.config import Config
 from resotolib.core import add_args as core_add_args, resotocore, wait_for_resotocore
 from resotolib.core.actions import CoreActions, CoreFeedback
 from resotolib.core.ca import TLSData
 from resotolib.core.tasks import CoreTasks, CoreTaskHandler
@@ -23,15 +22,15 @@
     add_event_listener,
     Event,
     EventType,
 )
 from resotolib.jwt import add_args as jwt_add_args
 from resotolib.logger import log, setup_logger, add_args as logging_add_args
 from resotolib.core.custom_command import command_definitions
-from resotolib.proc import log_stats, increase_limits
+from resotolib.proc import log_stats
 from resotolib.types import Json
 from resotolib.web import WebServer
 from resotolib.web.metrics import WebApp
 from resotoworker.cleanup import cleanup
 from resotoworker.collect import Collector
 from resotoworker.config import add_config
 from resotoworker.utils import write_files_to_home_dir, write_utf8_file
@@ -111,26 +110,25 @@
         if tls_data:
             verify = tls_data.verify
         return s.send(request=prepared, verify=verify)
 
     core = Resotocore(send_request, config)
 
     # the multiprocessing manager is used to share data between processes
-    mp_manager = multiprocessing.Manager()
+    ctx = multiprocessing.get_context("spawn")
+    mp_manager = SyncManager(ctx=ctx)
+    mp_manager.start(initializer=resotolib.proc.increase_limits)
     core_messages: Queue[Json] = mp_manager.Queue()
 
     collector = Collector(config, core, core_messages)
 
     # Handle Ctrl+c and other means of termination/shutdown
     resotolib.proc.initializer()
     add_event_listener(EventType.SHUTDOWN, shutdown, blocking=False)
 
-    # Try to increase nofile and nproc limits
-    increase_limits()
-
     web_server_args = {}
     if tls_data and not Config.resotoworker.no_tls:
         web_server_args = {
             "ssl_cert": tls_data.cert_path,
             "ssl_key": tls_data.key_path,
         }
     web_server = WebServer(
@@ -207,14 +205,15 @@
             log.exception(f"Caught unhandled persistent Plugin exception {e}")
 
     # We wait for the shutdown Event to be set() and then end the program
     # While doing so we print the list of active threads once per 15 minutes
     shutdown_event.wait()
     web_server.shutdown()
     time.sleep(1)  # everything gets 1000ms to shutdown gracefully before we force it
+    mp_manager.shutdown()
     resotolib.proc.kill_children(SIGTERM, ensure_death=True)
     log.info("Shutdown complete")
     os._exit(0)
 
 
 def core_actions_processor(
     config: Config,
```

### Comparing `resotoworker-3.6.1/resotoworker/cleanup.py` & `resotoworker-3.6.2/resotoworker/cleanup.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.1/resotoworker/collect.py` & `resotoworker-3.6.2/resotoworker/collect.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from tempfile import mkdtemp
 from shutil import rmtree
 from queue import Queue
 import resotolib.proc
 from time import time
 from concurrent import futures
 from threading import Lock
+from multiprocessing.managers import SyncManager
 from resotoworker.exceptions import DuplicateMessageError
 from resotoworker.resotocore import Resotocore
 from resotolib.baseplugin import BaseCollectorPlugin
 from resotolib.baseresources import GraphRoot, BaseCloud, BaseAccount, BaseResource
 from resotolib.core.actions import CoreFeedback
 from resotolib.graph import Graph, sanitize, GraphMergeKind
 from resotolib.logger import log, setup_logger
@@ -130,15 +131,17 @@
         processing_id = f"{task_id}:{step_name}"
         try:
             with self.processing_lock:
                 if processing_id in self.processing:
                     raise DuplicateMessageError(f"Already processing {processing_id} - ignoring message")
                 self.processing.add(processing_id)
 
-            mp_manager = multiprocessing.Manager()
+            ctx = multiprocessing.get_context("spawn")
+            mp_manager = SyncManager(ctx=ctx)
+            mp_manager.start(initializer=resotolib.proc.increase_limits)
             graph_queue: Queue[Optional[Graph]] = mp_manager.Queue()
             graph_sender_threads = []
             graph_sender_pool_size = self._config.resotoworker.graph_sender_pool_size
             tempdir = mkdtemp(prefix=f"resoto-{task_id}", dir=self._config.resotoworker.tempdir)
             try:
                 for i in range(graph_sender_pool_size):
                     graph_sender_t = threading.Thread(
@@ -153,18 +156,18 @@
                 self._resotocore.create_graph_and_update_model(tempdir=tempdir)
                 collect(collectors, graph_queue, task_data)
             finally:
                 log.debug("Telling graph sender threads to end")
                 for _ in range(graph_sender_pool_size):
                     graph_queue.put(None)
                 for t in graph_sender_threads:
-                    t.join(self._config.resotoworker.timeout)
+                    t.join(300)
+                mp_manager.shutdown()
                 if not self._config.resotoworker.debug_dump_json:
                     rmtree(tempdir, ignore_errors=True)
-
         finally:
             with self.processing_lock:
                 if processing_id in self.processing:
                     self.processing.remove(processing_id)
 
 
 def collect_plugin_graph(
```

### Comparing `resotoworker-3.6.1/resotoworker/config.py` & `resotoworker-3.6.2/resotoworker/config.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.1/resotoworker/pluginloader.py` & `resotoworker-3.6.2/resotoworker/pluginloader.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.1/resotoworker/resotocore.py` & `resotoworker-3.6.2/resotoworker/resotocore.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.1/resotoworker/tag.py` & `resotoworker-3.6.2/resotoworker/tag.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.1/resotoworker/utils.py` & `resotoworker-3.6.2/resotoworker/utils.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.1/resotoworker.egg-info/PKG-INFO` & `resotoworker-3.6.2/resotoworker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.6.1
+Version: 3.6.2
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoworker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `resotoworker-3.6.1/resotoworker.egg-info/SOURCES.txt` & `resotoworker-3.6.2/resotoworker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.1/test/test_args.py` & `resotoworker-3.6.2/test/test_args.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.1/test/test_collect.py` & `resotoworker-3.6.2/test/test_collect.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.1/test/test_resotocore.py` & `resotoworker-3.6.2/test/test_resotocore.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.1/test/test_utils.py` & `resotoworker-3.6.2/test/test_utils.py`

 * *Files identical despite different names*

