# Comparing `tmp/pympipool-0.5.5.tar.gz` & `tmp/pympipool-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympipool-0.5.5.tar", last modified: Tue Jul 18 13:53:02 2023, max compression
+gzip compressed data, was "pympipool-0.5.6.tar", last modified: Fri Jul 21 22:29:49 2023, max compression
```

## Comparing `pympipool-0.5.5.tar` & `pympipool-0.5.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:53:02.749822 pympipool-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-18 13:52:59.000000 pympipool-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-18 13:52:59.000000 pympipool-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-18 13:53:02.749822 pympipool-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-07-18 13:52:59.000000 pympipool-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:53:02.749822 pympipool-0.5.5/pympipool/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-18 13:53:02.749822 pympipool-0.5.5/pympipool/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:53:02.745822 pympipool-0.5.5/pympipool/external_interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/external_interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/external_interfaces/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/external_interfaces/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/external_interfaces/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/external_interfaces/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:53:02.745822 pympipool-0.5.5/pympipool/parallel_executors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/parallel_executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/parallel_executors/mpiexec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/parallel_executors/mpipool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:53:02.745822 pympipool-0.5.5/pympipool/shared_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/shared_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/shared_functions/external_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/shared_functions/parallel_executors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:53:02.745822 pympipool-0.5.5/pympipool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-18 13:53:02.000000 pympipool-0.5.5/pympipool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-18 13:53:02.000000 pympipool-0.5.5/pympipool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:53:02.000000 pympipool-0.5.5/pympipool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 13:53:02.000000 pympipool-0.5.5/pympipool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 13:53:02.000000 pympipool-0.5.5/pympipool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-18 13:53:02.749822 pympipool-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-18 13:53:02.000000 pympipool-0.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:53:02.749822 pympipool-0.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_communicator_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_future.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_worker_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-18 13:52:59.000000 pympipool-0.5.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:49.739897 pympipool-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-21 22:29:46.000000 pympipool-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-21 22:29:46.000000 pympipool-0.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-21 22:29:49.739897 pympipool-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-07-21 22:29:46.000000 pympipool-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:49.739897 pympipool-0.5.6/pympipool/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-21 22:29:49.739897 pympipool-0.5.6/pympipool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:49.735897 pympipool-0.5.6/pympipool/external_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/external_interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/external_interfaces/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/external_interfaces/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/external_interfaces/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/external_interfaces/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:49.735897 pympipool-0.5.6/pympipool/parallel_executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/parallel_executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/parallel_executors/mpiexec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/parallel_executors/mpipool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:49.739897 pympipool-0.5.6/pympipool/shared_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/shared_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/shared_functions/external_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/shared_functions/parallel_executors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:49.735897 pympipool-0.5.6/pympipool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-21 22:29:49.000000 pympipool-0.5.6/pympipool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-21 22:29:49.000000 pympipool-0.5.6/pympipool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:29:49.000000 pympipool-0.5.6/pympipool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 22:29:49.000000 pympipool-0.5.6/pympipool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 22:29:49.000000 pympipool-0.5.6/pympipool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-21 22:29:49.739897 pympipool-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-21 22:29:49.000000 pympipool-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:49.739897 pympipool-0.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_communicator_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_worker_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-21 22:29:46.000000 pympipool-0.5.6/versioneer.py
```

### Comparing `pympipool-0.5.5/LICENSE` & `pympipool-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/PKG-INFO` & `pympipool-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.5.5
+Version: 0.5.6
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.5.5/README.md` & `pympipool-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/pympipool/__init__.py` & `pympipool-0.5.6/pympipool/__init__.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/pympipool/external_interfaces/communication.py` & `pympipool-0.5.6/pympipool/external_interfaces/communication.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/pympipool/external_interfaces/executor.py` & `pympipool-0.5.6/pympipool/external_interfaces/executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/pympipool/external_interfaces/pool.py` & `pympipool-0.5.6/pympipool/external_interfaces/pool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/pympipool/external_interfaces/thread.py` & `pympipool-0.5.6/pympipool/external_interfaces/thread.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/pympipool/parallel_executors/mpiexec.py` & `pympipool-0.5.6/pympipool/parallel_executors/mpiexec.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from os.path import abspath
 import pickle
 import sys
 
 import cloudpickle
 
 from pympipool.external_interfaces.communication import (
     connect_to_socket_interface,
@@ -29,14 +30,19 @@
             host=argument_dict["host"], port=argument_dict["zmqport"]
         )
     else:
         context = None
         socket = None
 
     memory = None
+
+    cwd = abspath(".")
+    if cwd not in sys.path:
+        sys.path.insert(1, cwd)
+
     while True:
         # Read from socket
         if mpi_rank_zero:
             input_dict = receive_instruction(socket=socket)
         else:
             input_dict = None
         input_dict = MPI.COMM_WORLD.bcast(input_dict, root=0)
```

### Comparing `pympipool-0.5.5/pympipool/parallel_executors/mpipool.py` & `pympipool-0.5.6/pympipool/parallel_executors/mpipool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from os.path import abspath
 import pickle
 import sys
 
 import cloudpickle
 
 from pympipool.external_interfaces.communication import (
     connect_to_socket_interface,
@@ -23,14 +24,19 @@
         cloudpickle.loads,
         pickle.HIGHEST_PROTOCOL,
     )
     from mpi4py.futures import MPIPoolExecutor
 
     future_dict = {}
     argument_dict = parse_arguments(argument_lst=sys.argv)
+
+    cwd = abspath(".")
+    if cwd not in sys.path:
+        sys.path.insert(1, cwd)
+
     with MPIPoolExecutor(int(argument_dict["total_cores"])) as executor:
         if executor is not None:
             context, socket = connect_to_socket_interface(
                 host=argument_dict["host"], port=argument_dict["zmqport"]
             )
             while True:
                 output = parse_socket_communication(
```

### Comparing `pympipool-0.5.5/pympipool/shared_functions/external_interfaces.py` & `pympipool-0.5.6/pympipool/shared_functions/external_interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,15 +245,19 @@
         task_dict = future_queue.get()
         if "shutdown" in task_dict.keys() and task_dict["shutdown"]:
             interface.shutdown(wait=task_dict["wait"])
             break
         elif "fn" in task_dict.keys() and "future" in task_dict.keys():
             f = task_dict.pop("future")
             if f.set_running_or_notify_cancel():
-                f.set_result(interface.send_and_receive_dict(input_dict=task_dict))
+                try:
+                    f.set_result(interface.send_and_receive_dict(input_dict=task_dict))
+                except Exception as thread_exeception:
+                    f.set_exception(exception=thread_exeception)
+                    raise thread_exeception
         elif "fn" in task_dict.keys() and "init" in task_dict.keys():
             interface.send_dict(input_dict=task_dict)
 
 
 def _execute_serial_tasks_loop(
     interface, future_queue, future_dict, sleep_interval=0.1
 ):
```

### Comparing `pympipool-0.5.5/pympipool/shared_functions/parallel_executors.py` & `pympipool-0.5.6/pympipool/shared_functions/parallel_executors.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/pympipool.egg-info/PKG-INFO` & `pympipool-0.5.6/pympipool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.5.5
+Version: 0.5.6
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.5.5/pympipool.egg-info/SOURCES.txt` & `pympipool-0.5.6/pympipool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/setup.py` & `pympipool-0.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/tests/test_communicator_split.py` & `pympipool-0.5.6/tests/test_communicator_split.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/tests/test_executor.py` & `pympipool-0.5.6/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/tests/test_future.py` & `pympipool-0.5.6/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/tests/test_interface.py` & `pympipool-0.5.6/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/tests/test_multitask.py` & `pympipool-0.5.6/tests/test_multitask.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/tests/test_parse.py` & `pympipool-0.5.6/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/tests/test_pool.py` & `pympipool-0.5.6/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/tests/test_queue.py` & `pympipool-0.5.6/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/tests/test_task.py` & `pympipool-0.5.6/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/tests/test_worker.py` & `pympipool-0.5.6/tests/test_worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,14 +58,20 @@
         self.assertEqual(list(output), [np.array(1), np.array(4), np.array(9)])
 
     def test_executor_exception(self):
         with self.assertRaises(RuntimeError):
             with Executor(cores=1) as p:
                 p.submit(raise_error)
 
+    def test_executor_exception_future(self):
+        with self.assertRaises(RuntimeError):
+            with Executor(cores=1) as p:
+                fs = p.submit(raise_error)
+                fs.result()
+
     def test_pool_multi_core(self):
         with Executor(cores=2) as p:
             output = p.submit(mpi_funct, i=2)
             self.assertEqual(len(p), 1)
             self.assertTrue(isinstance(output, Future))
             self.assertFalse(output.done())
             sleep(1)
```

### Comparing `pympipool-0.5.5/tests/test_worker_memory.py` & `pympipool-0.5.6/tests/test_worker_memory.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/tests/test_zmq.py` & `pympipool-0.5.6/tests/test_zmq.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.5/versioneer.py` & `pympipool-0.5.6/versioneer.py`

 * *Files identical despite different names*

