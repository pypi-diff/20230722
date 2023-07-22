# Comparing `tmp/aiotaskq-0.0.3.tar.gz` & `tmp/aiotaskq-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotaskq-0.0.3.tar", last modified: Sun Mar 20 16:44:45 2022, max compression
+gzip compressed data, was "aiotaskq-0.0.4.tar", last modified: Fri Mar 25 03:24:36 2022, max compression
```

## Comparing `aiotaskq-0.0.3.tar` & `aiotaskq-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxr-x   0 in-gote   (1000) in-gote   (1000)        0 2022-03-20 16:44:45.844864 aiotaskq-0.0.3/
--rw-rw-r--   0 in-gote   (1000) in-gote   (1000)     1606 2022-03-20 16:44:45.844864 aiotaskq-0.0.3/PKG-INFO
--rw-rw-r--   0 in-gote   (1000) in-gote   (1000)     1079 2022-03-20 16:41:08.000000 aiotaskq-0.0.3/README.md
--rw-rw-r--   0 in-gote   (1000) in-gote   (1000)      299 2022-03-20 16:27:56.000000 aiotaskq-0.0.3/pyproject.toml
--rw-rw-r--   0 in-gote   (1000) in-gote   (1000)      637 2022-03-20 16:44:45.844864 aiotaskq-0.0.3/setup.cfg
-drwxrwxr-x   0 in-gote   (1000) in-gote   (1000)        0 2022-03-20 16:44:45.840865 aiotaskq-0.0.3/src/
-drwxrwxr-x   0 in-gote   (1000) in-gote   (1000)        0 2022-03-20 16:44:45.840865 aiotaskq-0.0.3/src/aiotaskq/
--rw-rw-r--   0 in-gote   (1000) in-gote   (1000)      731 2022-03-20 16:39:41.000000 aiotaskq-0.0.3/src/aiotaskq/__init__.py
--rw-rw-r--   0 in-gote   (1000) in-gote   (1000)      254 2022-03-20 15:57:25.000000 aiotaskq-0.0.3/src/aiotaskq/constants.py
--rw-rw-r--   0 in-gote   (1000) in-gote   (1000)      121 2022-03-20 14:12:34.000000 aiotaskq-0.0.3/src/aiotaskq/exceptions.py
--rw-rw-r--   0 in-gote   (1000) in-gote   (1000)     2767 2022-03-20 15:58:36.000000 aiotaskq-0.0.3/src/aiotaskq/main.py
--rw-rw-r--   0 in-gote   (1000) in-gote   (1000)     1352 2022-03-20 16:00:19.000000 aiotaskq-0.0.3/src/aiotaskq/worker.py
-drwxrwxr-x   0 in-gote   (1000) in-gote   (1000)        0 2022-03-20 16:44:45.844864 aiotaskq-0.0.3/src/aiotaskq.egg-info/
--rw-rw-r--   0 in-gote   (1000) in-gote   (1000)     1606 2022-03-20 16:44:45.000000 aiotaskq-0.0.3/src/aiotaskq.egg-info/PKG-INFO
--rw-rw-r--   0 in-gote   (1000) in-gote   (1000)      300 2022-03-20 16:44:45.000000 aiotaskq-0.0.3/src/aiotaskq.egg-info/SOURCES.txt
--rw-rw-r--   0 in-gote   (1000) in-gote   (1000)        1 2022-03-20 16:44:45.000000 aiotaskq-0.0.3/src/aiotaskq.egg-info/dependency_links.txt
--rw-rw-r--   0 in-gote   (1000) in-gote   (1000)        9 2022-03-20 16:44:45.000000 aiotaskq-0.0.3/src/aiotaskq.egg-info/top_level.txt
+drwxrwxr-x   0 in-gote   (1000) in-gote   (1000)        0 2022-03-25 03:24:36.701284 aiotaskq-0.0.4/
+-rw-rw-r--   0 in-gote   (1000) in-gote   (1000)     2242 2022-03-25 03:24:36.701284 aiotaskq-0.0.4/PKG-INFO
+-rw-rw-r--   0 in-gote   (1000) in-gote   (1000)     1693 2022-03-25 03:21:01.000000 aiotaskq-0.0.4/README.md
+-rw-rw-r--   0 in-gote   (1000) in-gote   (1000)      358 2022-03-25 03:21:01.000000 aiotaskq-0.0.4/pyproject.toml
+-rw-rw-r--   0 in-gote   (1000) in-gote   (1000)      714 2022-03-25 03:24:36.701284 aiotaskq-0.0.4/setup.cfg
+drwxrwxr-x   0 in-gote   (1000) in-gote   (1000)        0 2022-03-25 03:24:36.697284 aiotaskq-0.0.4/src/
+drwxrwxr-x   0 in-gote   (1000) in-gote   (1000)        0 2022-03-25 03:24:36.697284 aiotaskq-0.0.4/src/aiotaskq/
+-rw-rw-r--   0 in-gote   (1000) in-gote   (1000)      725 2022-03-25 03:21:01.000000 aiotaskq-0.0.4/src/aiotaskq/__init__.py
+-rwxrwxr-x   0 in-gote   (1000) in-gote   (1000)      419 2022-03-25 03:21:01.000000 aiotaskq-0.0.4/src/aiotaskq/__main__.py
+-rw-rw-r--   0 in-gote   (1000) in-gote   (1000)      255 2022-03-25 03:21:01.000000 aiotaskq-0.0.4/src/aiotaskq/constants.py
+-rw-rw-r--   0 in-gote   (1000) in-gote   (1000)      121 2022-03-20 14:12:34.000000 aiotaskq-0.0.4/src/aiotaskq/exceptions.py
+-rw-rw-r--   0 in-gote   (1000) in-gote   (1000)     2848 2022-03-25 03:21:01.000000 aiotaskq-0.0.4/src/aiotaskq/main.py
+-rwxrwxr-x   0 in-gote   (1000) in-gote   (1000)     2096 2022-03-25 03:21:01.000000 aiotaskq-0.0.4/src/aiotaskq/worker.py
+drwxrwxr-x   0 in-gote   (1000) in-gote   (1000)        0 2022-03-25 03:24:36.701284 aiotaskq-0.0.4/src/aiotaskq.egg-info/
+-rw-rw-r--   0 in-gote   (1000) in-gote   (1000)     2242 2022-03-25 03:24:36.000000 aiotaskq-0.0.4/src/aiotaskq.egg-info/PKG-INFO
+-rw-rw-r--   0 in-gote   (1000) in-gote   (1000)      399 2022-03-25 03:24:36.000000 aiotaskq-0.0.4/src/aiotaskq.egg-info/SOURCES.txt
+-rw-rw-r--   0 in-gote   (1000) in-gote   (1000)        1 2022-03-25 03:24:36.000000 aiotaskq-0.0.4/src/aiotaskq.egg-info/dependency_links.txt
+-rw-rw-r--   0 in-gote   (1000) in-gote   (1000)       51 2022-03-25 03:24:36.000000 aiotaskq-0.0.4/src/aiotaskq.egg-info/entry_points.txt
+-rw-rw-r--   0 in-gote   (1000) in-gote   (1000)      125 2022-03-25 03:24:36.000000 aiotaskq-0.0.4/src/aiotaskq.egg-info/requires.txt
+-rw-rw-r--   0 in-gote   (1000) in-gote   (1000)        9 2022-03-25 03:24:36.000000 aiotaskq-0.0.4/src/aiotaskq.egg-info/top_level.txt
```

### Comparing `aiotaskq-0.0.3/PKG-INFO` & `aiotaskq-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 Metadata-Version: 2.1
 Name: aiotaskq
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple asynchronous task queue
 Home-page: https://github.com/imranariffin/aiotaskq
 Author: Imran Ariffin
 Author-email: ariffin.imran@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/imranariffin/aiotaskq/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 
 # aiotask
 
 A simple asynchronous task queue
 
 ## Motivation
 
-Existing famously used asynchronous worker library (Celery) doesn't support asyncio and is hard to use. This library aims to help users compose tasks in a very native async-await manner. It is also full-typed for better productivity and correctness.
-
-## Simple Usage
+Existing famous asynchronous worker library (Celery) doesn't support asyncio and is hard to use. This library aims to help users compose tasks in a very native async-await manner. It is also full-typed for better productivity and correctness.
 
+## Example Usage
+Install aiotaskq
+```bash
+python -m pip install --upgrade pip
+pip install aiotaskq
+```
+Define simple app like the following:
+```bash
+tree .
+.
+└── app
+    └── app.py
+```
+Where `app.py` contains the following:
 ```python
 import asyncio
 
 import aiotaskq
 
 
 @aiotaskq.register_task
@@ -35,24 +48,40 @@
     # Some task with high cpu usage
     def _naive_fib(n: int) -> int:
         if n <= 1:
             return 1
         elif n <= 2:
             return 2
         return _naive_fib(n - 1) + _naive_fib(n - 2)
-    return _naove_fib(b)
+    return _naive_fib(b)
 
 
 async def main():
     async_result = await some_task.apply_async(42)
     sync_result = some_task(42)
     assert async_result == sync_result
+    print(f"sync_result == async_result == 165580141. Awesome!")
+
 
 if __name__ == "__main__":
-    asyncio.run_until_complete(main())
+    loop = asyncio.get_event_loop()
+    loop.run_until_complete(main())
+```
+Start redis
+```bash
+docker run --publish 127.0.0.1:6379:6379 redis
+```
+In a different terminal, start the aiotaskq worker
+```bash
+python -m aiotaskq worker app.app
+```
+Then in another different terminal, run your app
+```bash
+python ./app.py
+# Output: sync_result == async_result == {42}. Awesome!
 ```
 
 ## Advance usage
 
 ```python
 # TODO: Example of composing chain of tasks (chord + chain in Celery terms)
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aiotaskq-0.0.3/setup.cfg` & `aiotaskq-0.0.4/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aiotaskq
-version = 0.0.3
+version = 0.0.4
 author = Imran Ariffin
 author_email = ariffin.imran@gmail.com
 description = A simple asynchronous task queue
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/imranariffin/aiotaskq
 project_urls = 
@@ -19,11 +19,15 @@
 	= src
 packages = find:
 python_requires = >=3.9
 
 [options.packages.find]
 where = src
 
+[options.entry_points]
+console_scripts = 
+	aiotaskq = aiotaskq.__main__:cli
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `aiotaskq-0.0.3/src/aiotaskq/__init__.py` & `aiotaskq-0.0.4/src/aiotaskq/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,10 +28,8 @@
         asyncio.run_until_complete(main())
 
 """
 
 from .main import register_task
 
 
-__all__ = [
-    "register_task"
-]
+__all__ = ["register_task"]
```

### Comparing `aiotaskq-0.0.3/src/aiotaskq/main.py` & `aiotaskq-0.0.4/src/aiotaskq/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,86 +1,91 @@
 import asyncio
 import json
+import logging
 import typing as t
 import uuid
 
 from aiotaskq.constants import REDIS_URL, RESULTS_CHANNEL_TEMPLATE, TASKS_CHANNEL
 from aiotaskq.exceptions import WorkerNotReady
 
 import aioredis
 
-
-
 RT = t.TypeVar("RT")
 P = t.ParamSpec("P")
 
+logging.basicConfig(level=logging.DEBUG)
+logger = logging.getLogger(__name__)
+
 
 class AsyncResult(t.Generic[RT]):
     _result: RT
     _completed: bool = False
     _task_id: str
 
     def __init__(self, task_id: str) -> None:
         self._task_id = task_id
-    
+
     async def get(self) -> RT:
         redis_client = aioredis.from_url(REDIS_URL)
         async with redis_client.pubsub() as pubsub:
-            # await pubsub.subscribe(RESULTS_CHANNEL_TEMPLATE.format(task_id=self._task_id))
-            _result: RT
-            result = None
-            while result is None:
-                await pubsub.subscribe(RESULTS_CHANNEL_TEMPLATE.format(task_id=self._task_id))
-                result = await pubsub.get_message(ignore_subscribe_messages=True)
+            message: t.Optional[dict] = None
+            while message is None:
+                await pubsub.subscribe(
+                    RESULTS_CHANNEL_TEMPLATE.format(task_id=self._task_id)
+                )
+                message = await pubsub.get_message(ignore_subscribe_messages=True)
                 await asyncio.sleep(0.1)
-            print(result)
-            _result = json.loads(result["data"])
+            logger.debug("Message: %s", message)
+            _result: RT = json.loads(message["data"])
         return _result
 
 
 class Task(t.Generic[P, RT]):
 
     __qualname__: str
 
     def __init__(self, f: t.Callable[P, RT]) -> None:
         self._f = f
         self._id = uuid.uuid4()
 
     def __call__(self, *args, **kwargs) -> RT:
         return self._f(*args, **kwargs)
-    
+
     def get_task_id(self) -> str:
         return f"{self.__qualname__}:{self._id}"
 
     async def apply_async(self, *args: P.args, **kwargs: P.kwargs) -> RT:
         task_id = self.get_task_id()
         message = json.dumps(
             {
                 "task_id": task_id,
-                "args": args, 
+                "args": args,
                 "kwargs": kwargs,
             }
         )
         publisher = _get_redis_client()
 
         is_worker_ready = (await publisher.pubsub_numsub(TASKS_CHANNEL))[0][1] > 0
         if not is_worker_ready:
-            raise WorkerNotReady("No worker is ready to pick up tasks. Have you run your workers?")
-    
+            raise WorkerNotReady(
+                "No worker is ready to pick up tasks. Have you run your workers?"
+            )
+
         await publisher.publish(TASKS_CHANNEL, message=message)
         async_result: AsyncResult[RT] = AsyncResult(task_id=task_id)
         result = await async_result.get()
         return result
 
 
 def register_task(f: t.Callable[P, RT]) -> Task[P, RT]:
     import inspect
+
     func_module = inspect.getmodule(f)
     module_path = ".".join(
-        [p.split(".py")[0] for p in func_module.__file__.strip("./").split("/") if p != "src"] # type: ignore
+        [p.split(".py")[0] for p in func_module.__file__.strip("./").split("/") if p != "src"]  # type: ignore
     )
     task = Task[P, RT](f)
     task.__qualname__ = f"{module_path}.{f.__name__}"
     task.__module__ = module_path
     return task
```

### Comparing `aiotaskq-0.0.3/src/aiotaskq.egg-info/PKG-INFO` & `aiotaskq-0.0.4/src/aiotaskq.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 Metadata-Version: 2.1
 Name: aiotaskq
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple asynchronous task queue
 Home-page: https://github.com/imranariffin/aiotaskq
 Author: Imran Ariffin
 Author-email: ariffin.imran@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/imranariffin/aiotaskq/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 
 # aiotask
 
 A simple asynchronous task queue
 
 ## Motivation
 
-Existing famously used asynchronous worker library (Celery) doesn't support asyncio and is hard to use. This library aims to help users compose tasks in a very native async-await manner. It is also full-typed for better productivity and correctness.
-
-## Simple Usage
+Existing famous asynchronous worker library (Celery) doesn't support asyncio and is hard to use. This library aims to help users compose tasks in a very native async-await manner. It is also full-typed for better productivity and correctness.
 
+## Example Usage
+Install aiotaskq
+```bash
+python -m pip install --upgrade pip
+pip install aiotaskq
+```
+Define simple app like the following:
+```bash
+tree .
+.
+└── app
+    └── app.py
+```
+Where `app.py` contains the following:
 ```python
 import asyncio
 
 import aiotaskq
 
 
 @aiotaskq.register_task
@@ -35,24 +48,40 @@
     # Some task with high cpu usage
     def _naive_fib(n: int) -> int:
         if n <= 1:
             return 1
         elif n <= 2:
             return 2
         return _naive_fib(n - 1) + _naive_fib(n - 2)
-    return _naove_fib(b)
+    return _naive_fib(b)
 
 
 async def main():
     async_result = await some_task.apply_async(42)
     sync_result = some_task(42)
     assert async_result == sync_result
+    print(f"sync_result == async_result == 165580141. Awesome!")
+
 
 if __name__ == "__main__":
-    asyncio.run_until_complete(main())
+    loop = asyncio.get_event_loop()
+    loop.run_until_complete(main())
+```
+Start redis
+```bash
+docker run --publish 127.0.0.1:6379:6379 redis
+```
+In a different terminal, start the aiotaskq worker
+```bash
+python -m aiotaskq worker app.app
+```
+Then in another different terminal, run your app
+```bash
+python ./app.py
+# Output: sync_result == async_result == {42}. Awesome!
 ```
 
 ## Advance usage
 
 ```python
 # TODO: Example of composing chain of tasks (chord + chain in Celery terms)
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

