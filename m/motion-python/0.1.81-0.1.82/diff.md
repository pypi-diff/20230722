# Comparing `tmp/motion_python-0.1.81.tar.gz` & `tmp/motion_python-0.1.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.81.tar", max compression
+gzip compressed data, was "motion_python-0.1.82.tar", max compression
```

## Comparing `motion_python-0.1.81.tar` & `motion_python-0.1.82.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3344 2023-07-14 23:09:36.657246 motion_python-0.1.81/README.md
--rw-r--r--   0        0        0      344 2023-07-14 23:09:36.657246 motion_python-0.1.81/motion/__init__.py
--rw-r--r--   0        0        0     3867 2023-07-14 23:09:36.657246 motion_python-0.1.81/motion/cli.py
--rw-r--r--   0        0        0    24251 2023-07-14 23:09:36.657246 motion_python-0.1.81/motion/component.py
--rw-r--r--   0        0        0     4623 2023-07-14 23:09:36.657246 motion_python-0.1.81/motion/dicts.py
--rw-r--r--   0        0        0    17368 2023-07-14 23:09:36.657246 motion_python-0.1.81/motion/execute.py
--rw-r--r--   0        0        0    13681 2023-07-14 23:09:36.657246 motion_python-0.1.81/motion/instance.py
--rw-r--r--   0        0        0     4882 2023-07-14 23:09:36.661246 motion_python-0.1.81/motion/migrate.py
--rw-r--r--   0        0        0    13660 2023-07-14 23:09:36.661246 motion_python-0.1.81/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0     1153 2023-07-14 23:09:36.661246 motion_python-0.1.81/motion/route.py
--rw-r--r--   0        0        0     4953 2023-07-14 23:09:36.661246 motion_python-0.1.81/motion/server/update_task.py
--rw-r--r--   0        0        0     8661 2023-07-14 23:09:36.661246 motion_python-0.1.81/motion/utils.py
--rw-r--r--   0        0        0     1736 2023-07-14 23:10:02.405441 motion_python-0.1.81/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.81/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-07-21 23:34:21.661643 motion_python-0.1.82/README.md
+-rw-r--r--   0        0        0      344 2023-07-21 23:34:21.661643 motion_python-0.1.82/motion/__init__.py
+-rw-r--r--   0        0        0     3867 2023-07-21 23:34:21.661643 motion_python-0.1.82/motion/cli.py
+-rw-r--r--   0        0        0    24251 2023-07-21 23:34:21.661643 motion_python-0.1.82/motion/component.py
+-rw-r--r--   0        0        0     4623 2023-07-21 23:34:21.665644 motion_python-0.1.82/motion/dicts.py
+-rw-r--r--   0        0        0    17498 2023-07-21 23:34:21.665644 motion_python-0.1.82/motion/execute.py
+-rw-r--r--   0        0        0    13682 2023-07-21 23:34:21.665644 motion_python-0.1.82/motion/instance.py
+-rw-r--r--   0        0        0     4897 2023-07-21 23:34:21.665644 motion_python-0.1.82/motion/migrate.py
+-rw-r--r--   0        0        0    13660 2023-07-21 23:34:21.665644 motion_python-0.1.82/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0     1153 2023-07-21 23:34:21.665644 motion_python-0.1.82/motion/route.py
+-rw-r--r--   0        0        0     4953 2023-07-21 23:34:21.665644 motion_python-0.1.82/motion/server/update_task.py
+-rw-r--r--   0        0        0     9966 2023-07-21 23:34:21.665644 motion_python-0.1.82/motion/utils.py
+-rw-r--r--   0        0        0     1782 2023-07-21 23:34:46.301750 motion_python-0.1.82/pyproject.toml
+-rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 motion_python-0.1.82/PKG-INFO
```

### Comparing `motion_python-0.1.81/README.md` & `motion_python-0.1.82/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.81/motion/cli.py` & `motion_python-0.1.82/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.81/motion/component.py` & `motion_python-0.1.82/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.81/motion/dicts.py` & `motion_python-0.1.82/motion/dicts.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.81/motion/execute.py` & `motion_python-0.1.82/motion/execute.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from motion.dicts import Properties, State
 from motion.route import Route
 from motion.server.update_task import UpdateTask
 from motion.utils import (
     RedisParams,
     UpdateEvent,
     UpdateEventGroup,
+    get_redis_params,
     hash_object,
     loadState,
     logger,
     saveState,
 )
 
 
@@ -41,21 +42,20 @@
 
         self._init_state_func = init_state_func
         self._init_state_params = init_state_params
         self._load_state_func = load_state_func
         self._save_state_func = save_state_func
 
         self.running: Any = multiprocessing.Value("b", False)
-        self._redis_con = self._connectToRedis()
+        self._redis_params, self._redis_con = self._connectToRedis()
         try:
             self._redis_con.ping()
         except redis.exceptions.ConnectionError:
-            rp = RedisParams()
             raise ConnectionError(
-                f"Could not connect to a Redis backend {rp}. "
+                f"Could not connect to a Redis backend {self._redis_params}. "
                 + "Please set environment variables MOTION_REDIS_HOST, "
                 + "MOTION_REDIS_PORT, MOTION_REDIS_DB, and/or "
                 + "MOTION_REDIS_PASSWORD to your Redis params."
             )
         self.running.value = True
 
         # Set up state
@@ -93,23 +93,23 @@
         # self._shutdown_event = threading.Event()
 
         # Set up update queues, batch sizes, and threads
         self.disabled = disabled
         if not disabled:
             self._build_fit_jobs()
 
-    def _connectToRedis(self) -> redis.Redis:
-        rp = RedisParams()
+    def _connectToRedis(self) -> Tuple[RedisParams, redis.Redis]:
+        rp = get_redis_params()
         r = redis.Redis(
             host=rp.host,
             port=rp.port,
             password=rp.password,
             db=rp.db,
         )
-        return r
+        return rp, r
 
     def _loadState(self) -> State:
         return loadState(self._redis_con, self._instance_name, self._load_state_func)
 
     def setUp(self, **kwargs: Any) -> Dict[str, Any]:
         # Set up initial state
         if self._init_state_func is not None:
@@ -118,15 +118,14 @@
                 raise TypeError(f"{self._instance_name} init should return a dict.")
             return initial_state
 
         return {}
 
     def _build_fit_jobs(self) -> None:
         """Builds update job."""
-        rp = RedisParams()
         # self.worker_states = {}
 
         # Set up update task
         self.route_dict_for_fit = {}
         self.channel_dict_for_fit = {}
         self.queue_ids_for_fit = []
         for rkey, routes in self._update_routes.items():
@@ -143,18 +142,18 @@
             self.worker_task = UpdateTask(
                 self._instance_name,
                 routes=self.route_dict_for_fit,
                 save_state_func=self._save_state_func,
                 load_state_func=self._load_state_func,
                 queue_identifiers=self.queue_ids_for_fit,
                 channel_identifiers=self.channel_dict_for_fit,
-                redis_host=rp.host,
-                redis_port=rp.port,
-                redis_db=rp.db,
-                redis_password=rp.password,  # type: ignore
+                redis_host=self._redis_params.host,
+                redis_port=self._redis_params.port,
+                redis_db=self._redis_params.db,
+                redis_password=self._redis_params.password,  # type: ignore
                 running=self.running,
             )
             self.worker_task.start()
 
         # Set up a monitor thread
         self.stop_event = threading.Event()
         self.monitor_thread = threading.Thread(
@@ -162,15 +161,14 @@
         )
         self.monitor_thread.start()
 
     def _monitor_process(self) -> None:
         if not self.worker_task:
             return
 
-        rp = RedisParams()
         while not self.stop_event.is_set():
             # See if the update task is alive
             if not self.worker_task.is_alive():
                 logger.debug(
                     f"Failed to detect heartbeat for {self.worker_task.name}."
                     + " Restarting the task in the background."
                 )
@@ -179,18 +177,18 @@
                 self.worker_task = UpdateTask(
                     self._instance_name,
                     routes=self.route_dict_for_fit,
                     save_state_func=self._save_state_func,
                     load_state_func=self._load_state_func,
                     queue_identifiers=self.queue_ids_for_fit,
                     channel_identifiers=self.channel_dict_for_fit,
-                    redis_host=rp.host,
-                    redis_port=rp.port,
-                    redis_db=rp.db,
-                    redis_password=rp.password,  # type: ignore
+                    redis_host=self._redis_params.host,
+                    redis_port=self._redis_params.port,
+                    redis_db=self._redis_params.db,
+                    redis_password=self._redis_params.password,  # type: ignore
                     running=self.running,
                 )
                 self.worker_task.start()
 
             if self.stop_event.is_set():
                 break
```

### Comparing `motion_python-0.1.81/motion/instance.py` & `motion_python-0.1.82/motion/instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import atexit
 import logging
+
 from typing import Any, Awaitable, Callable, Dict, List, Optional
 
 from motion.execute import Executor
 from motion.route import Route
 from motion.utils import DEFAULT_KEY_TTL, configureLogging, logger
```

### Comparing `motion_python-0.1.81/motion/migrate.py` & `motion_python-0.1.82/motion/migrate.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 from typing import Callable, List, Optional, Tuple
 
 import redis
 from pydantic import BaseConfig, BaseModel, Field
 
 from motion.component import Component
 from motion.dicts import State
-from motion.utils import RedisParams, loadState, logger, saveState
+from motion.utils import get_redis_params, loadState, logger, saveState
 
 
 def process_migration(
     instance_name: str,
     migrate_func: Callable,
     load_state_fn: Callable,
     save_state_fn: Callable,
 ) -> Tuple[str, Optional[Exception]]:
     try:
-        rp = RedisParams()
+        rp = get_redis_params()
         redis_con = redis.Redis(
             host=rp.host, port=rp.port, password=rp.password, db=rp.db
         )
         state = loadState(redis_con, instance_name, load_state_fn)
         new_state = migrate_func(state)
         assert isinstance(new_state, dict), (
             "Migration function must return a dict."
@@ -97,15 +97,15 @@
             List[MigrationResult]:
                 List of objects with instance_id and exception keys, where
                 exception is None if the migration was successful for that
                 instance name.
         """
         # Read all the states
 
-        rp = RedisParams()
+        rp = get_redis_params()
         redis_con = redis.Redis(
             host=rp.host, port=rp.port, password=rp.password, db=rp.db
         )
         instance_names = [
             self.component.name + "__" + iid if "__" not in iid else iid
             for iid in instance_ids
         ]
```

### Comparing `motion_python-0.1.81/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.82/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.81/motion/route.py` & `motion_python-0.1.82/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.81/motion/server/update_task.py` & `motion_python-0.1.82/motion/server/update_task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.81/motion/utils.py` & `motion_python-0.1.82/motion/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import random
 from pathlib import Path
 from typing import Any, Callable, Dict, Optional
 
 import cloudpickle
 import colorlog
 import redis
+import yaml
 from pydantic import BaseModel
 
 from motion.dicts import CustomDict, State
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_KEY_TTL = 60 * 60 * 24  # 1 day
@@ -34,22 +35,65 @@
 class RedisParams(BaseModel):
     host: str
     port: int
     db: int
     password: Optional[str] = None
 
     def __init__(self, **kwargs: Any) -> None:
-        kwargs.setdefault("host", os.getenv("MOTION_REDIS_HOST", "localhost"))
-        kwargs.setdefault("port", int(os.getenv("MOTION_REDIS_PORT", "6379")))
-        kwargs.setdefault("db", int(os.getenv("MOTION_REDIS_DB", "0")))
-        kwargs.setdefault("password", os.getenv("MOTION_REDIS_PASSWORD", None))
+        config = kwargs.get("config")
+
+        if config is not None:
+            kwargs.setdefault(
+                "host",
+                config.get(
+                    "MOTION_REDIS_HOST",
+                    os.getenv("MOTION_REDIS_HOST", "localhost"),
+                ),
+            )
+            kwargs.setdefault(
+                "port",
+                config.get(
+                    "MOTION_REDIS_PORT",
+                    int(os.getenv("MOTION_REDIS_PORT", "6379")),
+                ),
+            )
+            kwargs.setdefault(
+                "db",
+                config.get("MOTION_REDIS_DB", int(os.getenv("MOTION_REDIS_DB", "0"))),
+            )
+            kwargs.setdefault(
+                "password",
+                config.get(
+                    "MOTION_REDIS_PASSWORD",
+                    os.getenv("MOTION_REDIS_PASSWORD", None),
+                ),
+            )
+        else:
+            kwargs.setdefault("host", os.getenv("MOTION_REDIS_HOST", "localhost"))
+            kwargs.setdefault("port", int(os.getenv("MOTION_REDIS_PORT", "6379")))
+            kwargs.setdefault("db", int(os.getenv("MOTION_REDIS_DB", "0")))
+            kwargs.setdefault("password", os.getenv("MOTION_REDIS_PASSWORD", None))
 
         super().__init__(**kwargs)
 
 
+def get_redis_params(
+    config_file: str = "mconfig.yaml",
+) -> RedisParams:
+    config = None
+    if os.path.isfile(config_file):
+        with open(config_file, "r") as file:
+            config = yaml.safe_load(file)
+    else:
+        logger.info("No mconfig file found, using environment variables.")
+
+    rp = RedisParams(config=config)
+    return rp
+
+
 def clear_instance(instance_name: str) -> bool:
     """Clears the state and cached results associated with a component instance.
 
     Usage:
     ```python
     from motion import clear_instance
 
@@ -67,15 +111,15 @@
 
     Returns:
         bool: True if the instance existed, False otherwise.
     """
     if "__" not in instance_name:
         raise ValueError("Instance must be in the form `componentname__instanceid`.")
 
-    rp = RedisParams()
+    rp = get_redis_params()
     redis_con = redis.Redis(host=rp.host, port=rp.port, password=rp.password, db=rp.db)
 
     # Check if the instance exists
     if not redis_con.exists(f"MOTION_VERSION:{instance_name}"):
         return False
 
     # Delete the instance state, version, and cached results
@@ -116,15 +160,15 @@
 
     Returns:
         Dict[str, Any]: The state of the component instance.
     """
     if "__" not in instance_name:
         raise ValueError("Instance must be in the form `componentname__instanceid`.")
 
-    rp = RedisParams()
+    rp = get_redis_params()
     redis_con = redis.Redis(host=rp.host, port=rp.port, password=rp.password, db=rp.db)
 
     # Check if the instance exists
     if not redis_con.exists(f"MOTION_VERSION:{instance_name}"):
         raise ValueError(f"Instance {instance_name} does not exist.")
 
     # Get the state
```

### Comparing `motion_python-0.1.81/pyproject.toml` & `motion_python-0.1.82/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.81"
+version = "0.1.82"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1.3"
 colorlog = "^6.7.0"
 pydantic = "^1.10.7"
 cloudpickle = "^2.0"
 redis = "^4.5.5"
 psutil = "^5.9.5"
 rich = "^13.4.1"
+pyyaml = "^6.0.1"
 
 [tool.poetry.group.dev.dependencies]
 poetry-types = "^0.3.5"
 pytest = "^7.2.2"
 mypy = "^1.1.1"
 coverage = {extras = ["toml"], version = "^7.2.3"}
 pre-commit = "^3.2.1"
@@ -35,14 +36,15 @@
 mike = "^1.1.2"
 scikit-learn = "^1.2.2"
 types-redis = "^4.5.5.2"
 fastapi = "^0.95.2"
 httpx = "^0.24.1"
 pytest-asyncio = "^0.21.0"
 pytest-timeout = "^2.1.0"
+types-pyyaml = "^6.0.12.10"
 
 [tool.poetry.scripts]
 motion = "motion.cli:motioncli"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = "--basetemp=/tmp/pytest"
```

### Comparing `motion_python-0.1.81/PKG-INFO` & `motion_python-0.1.82/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.81
+Version: 0.1.82
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cloudpickle (>=2.0,<3.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: redis (>=4.5.5,<5.0.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0)
 Description-Content-Type: text/markdown
 
 # Motion
 
 [![motion](https://github.com/dm4ml/motion/workflows/motion/badge.svg)](https://github.com/dm4ml/motion/actions?query=workflow:"motion")
```

