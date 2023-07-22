# Comparing `tmp/quickscope-0.1.3.tar.gz` & `tmp/quickscope-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickscope-0.1.3.tar", last modified: Thu Aug 11 18:52:16 2022, max compression
+gzip compressed data, was "quickscope-0.1.4.tar", last modified: Sat Jul 22 17:57:06 2023, max compression
```

## Comparing `quickscope-0.1.3.tar` & `quickscope-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2022-08-11 18:52:16.763047 quickscope-0.1.3/
--rw-rw-r--   0 audrey    (1000) audrey    (1000)     1714 2022-08-11 18:52:16.763047 quickscope-0.1.3/PKG-INFO
--rw-rw-r--   0 audrey    (1000) audrey    (1000)     1470 2022-08-11 18:50:20.000000 quickscope-0.1.3/README.md
--rw-rw-r--   0 audrey    (1000) audrey    (1000)       98 2022-07-28 05:50:42.000000 quickscope-0.1.3/pyproject.toml
-drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2022-08-11 18:52:16.759055 quickscope-0.1.3/quickscope/
--rw-rw-r--   0 audrey    (1000) audrey    (1000)       62 2022-08-11 18:51:29.000000 quickscope-0.1.3/quickscope/__init__.py
--rw-rw-r--   0 audrey    (1000) audrey    (1000)       34 2022-08-11 18:04:52.000000 quickscope-0.1.3/quickscope/__main__.py
--rw-rw-r--   0 audrey    (1000) audrey    (1000)     2482 2022-08-11 17:48:35.000000 quickscope-0.1.3/quickscope/common.py
--rw-rw-r--   0 audrey    (1000) audrey    (1000)    19026 2022-08-11 18:06:34.000000 quickscope-0.1.3/quickscope/shooter.py
--rw-rw-r--   0 audrey    (1000) audrey    (1000)    12729 2022-08-11 00:03:27.000000 quickscope-0.1.3/quickscope/statuspage.py
--rw-rw-r--   0 audrey    (1000) audrey    (1000)    11417 2022-08-11 18:33:36.000000 quickscope-0.1.3/quickscope/tracker.py
-drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2022-08-11 18:52:16.763047 quickscope-0.1.3/quickscope.egg-info/
--rw-rw-r--   0 audrey    (1000) audrey    (1000)     1714 2022-08-11 18:52:16.000000 quickscope-0.1.3/quickscope.egg-info/PKG-INFO
--rw-rw-r--   0 audrey    (1000) audrey    (1000)      376 2022-08-11 18:52:16.000000 quickscope-0.1.3/quickscope.egg-info/SOURCES.txt
--rw-rw-r--   0 audrey    (1000) audrey    (1000)        1 2022-08-11 18:52:16.000000 quickscope-0.1.3/quickscope.egg-info/dependency_links.txt
--rw-rw-r--   0 audrey    (1000) audrey    (1000)       55 2022-08-11 18:52:16.000000 quickscope-0.1.3/quickscope.egg-info/entry_points.txt
--rw-rw-r--   0 audrey    (1000) audrey    (1000)       30 2022-08-11 18:52:16.000000 quickscope-0.1.3/quickscope.egg-info/requires.txt
--rw-rw-r--   0 audrey    (1000) audrey    (1000)       11 2022-08-11 18:52:16.000000 quickscope-0.1.3/quickscope.egg-info/top_level.txt
--rw-rw-r--   0 audrey    (1000) audrey    (1000)      526 2022-08-11 18:52:16.763047 quickscope-0.1.3/setup.cfg
+drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2023-07-22 17:57:06.292819 quickscope-0.1.4/
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)     1714 2023-07-22 17:57:06.292819 quickscope-0.1.4/PKG-INFO
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)     1470 2022-08-11 18:50:20.000000 quickscope-0.1.4/README.md
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)       98 2022-07-28 05:50:42.000000 quickscope-0.1.4/pyproject.toml
+drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2023-07-22 17:57:06.292819 quickscope-0.1.4/quickscope/
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)       62 2023-07-22 17:41:56.000000 quickscope-0.1.4/quickscope/__init__.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)       34 2022-08-11 18:04:52.000000 quickscope-0.1.4/quickscope/__main__.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)     2576 2023-07-22 16:41:07.000000 quickscope-0.1.4/quickscope/common.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)    19251 2023-07-22 17:10:28.000000 quickscope-0.1.4/quickscope/shooter.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)    12729 2022-08-11 00:03:27.000000 quickscope-0.1.4/quickscope/statuspage.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)    11434 2022-08-11 18:57:26.000000 quickscope-0.1.4/quickscope/tracker.py
+drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2023-07-22 17:57:06.292819 quickscope-0.1.4/quickscope.egg-info/
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)     1714 2023-07-22 17:57:06.000000 quickscope-0.1.4/quickscope.egg-info/PKG-INFO
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)      376 2023-07-22 17:57:06.000000 quickscope-0.1.4/quickscope.egg-info/SOURCES.txt
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)        1 2023-07-22 17:57:06.000000 quickscope-0.1.4/quickscope.egg-info/dependency_links.txt
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)       55 2023-07-22 17:57:06.000000 quickscope-0.1.4/quickscope.egg-info/entry_points.txt
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)       30 2023-07-22 17:57:06.000000 quickscope-0.1.4/quickscope.egg-info/requires.txt
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)       11 2023-07-22 17:57:06.000000 quickscope-0.1.4/quickscope.egg-info/top_level.txt
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)      526 2023-07-22 17:57:06.292819 quickscope-0.1.4/setup.cfg
```

### Comparing `quickscope-0.1.3/PKG-INFO` & `quickscope-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickscope
-Version: 0.1.3
+Version: 0.1.4
 Summary: A lightweight and scalable A/D CTF exploit shooter
 Home-page: https://github.com/shellphish/quickscope
 License: zlib
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Quickscope
```

### Comparing `quickscope-0.1.3/README.md` & `quickscope-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `quickscope-0.1.3/quickscope/common.py` & `quickscope-0.1.4/quickscope/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict
+from typing import List, Dict, Optional
 import enum
 from dataclasses import dataclass, field
 from dataclasses_json import config, DataClassJsonMixin
 from collections import defaultdict
 import logging
 
 PORT = 3356
@@ -18,14 +18,15 @@
     port: int
 
 @dataclass(frozen=True)
 class Target(DataClassJsonMixin):
     team: Team
     service: Service
     flag_id: str
+    tick: Optional[int] = None
 
     def same_process(self, other: 'Target'):
         return self.team == other.team and self.service == other.service
 
 class SubmissionResult(enum.Enum):
     OK = 'OK'
     INVALID = 'INVALID'
@@ -79,15 +80,16 @@
     tick_timeout: int
     retry_timeout: int
     error_log: str
 
 def setup_logging():
     """installs logging configuration. run this before any other code"""
     root = logging.getLogger()
-    root.setLevel(logging.DEBUG)
+    root.setLevel(logging.INFO)
+    logging.getLogger('quickscope').setLevel('DEBUG')
     ch = logging.StreamHandler()
     ch.setLevel(logging.DEBUG)
     fm = logging.Formatter(
         "%(asctime)s - %(name)-25s - %(funcName)-10s - %(levelname)-5s"
         + " - %(message)s")
     ch.setFormatter(fm)
     root.addHandler(ch)
```

### Comparing `quickscope-0.1.3/quickscope/shooter.py` & `quickscope-0.1.4/quickscope/shooter.py`

 * *Files 2% similar despite different names*

```diff
@@ -362,24 +362,24 @@
 
     if not os.access(script, os.X_OK):
         if script.endswith('.py'):
             cmd.insert(0, 'python3')
 
     def preexec_limits():
         size_bytes = int(mem_limit * 1024 * 1024 * 1024)
-        resource.setrlimit(resource.RLIMIT_STACK, (size_bytes, size_bytes))
+        #resource.setrlimit(resource.RLIMIT_STACK, (size_bytes, size_bytes))
         resource.setrlimit(resource.RLIMIT_DATA, (size_bytes, size_bytes))
         os.setpgrp()
 
     proc = subprocess.Popen(
         cmd,
         stdin=subprocess.PIPE,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
-        cwd=os.path.dirname(script),
+        cwd=os.path.dirname(os.path.realpath(script)),
         preexec_fn=preexec_limits,
         env=env,
     )
     assert proc.stdout is not None
     LIVE_PROCESSES.add(proc)
     head_buf: List[bytes] = []
     tail_buf: List[bytes] = []
@@ -416,16 +416,23 @@
                     logger.warning("Submission queue is full")
                     time.sleep(5)
                 else:
                     break
 
     try:
         proc.wait(deadline - time.time())
+        try:
+            os.killpg(proc.pid, signal.SIGKILL)
+        except ProcessLookupError:
+            pass
     except subprocess.TimeoutExpired:
-        proc.kill()
+        try:
+            os.killpg(proc.pid, signal.SIGKILL)
+        except ProcessLookupError:
+            pass
         proc.wait()
     LIVE_PROCESSES.remove(proc)
 
     if logdir is not None:
         log_filename = os.path.join(logdir, script + '-' + datetime.datetime.now().isoformat())
         pathlib.Path(log_filename).parent.mkdir(parents=True, exist_ok=True)
         with open(log_filename, 'wb') as fp:
```

### Comparing `quickscope-0.1.3/quickscope/statuspage.py` & `quickscope-0.1.4/quickscope/statuspage.py`

 * *Files identical despite different names*

### Comparing `quickscope-0.1.3/quickscope/tracker.py` & `quickscope-0.1.4/quickscope/tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
 import concurrent.futures
 import threading
 import nclib
 import io
 import time
-from typing import Optional
+from typing import Optional, Set
 
 from .common import *
 
 
 logger = logging.getLogger(__name__)
 
 class Tracker:
@@ -134,18 +134,18 @@
 
     def process_successful_submissions(
             self,
             submissions: List[Submission],
             results: List[SubmissionLog],
             sock: Optional[nclib.Netcat]=None
     ) -> None:
-        submissions = set(submissions)
+        submissions_set = set(submissions)
         for result in results:
             try:
-                submissions.remove(result.submission)
+                submissions_set.remove(result.submission)
             except KeyError:
                 pass
             if result.result == SubmissionResult.SELF:
                 self.untarget_host_port(result.submission.target)
             elif result.result == SubmissionResult.OK:
                 logger.info(
                     "Got points on %s:%s",
@@ -168,15 +168,15 @@
             elif result.result == SubmissionResult.TOO_OLD:
                 pass
             else:
                 logger.error("Bad submission result: %s (is your submitter misbehaving?)",
                              result.result)
 
         with self.submit_buffer_lock:
-            self.submit_buffer.extend(submissions)
+            self.submit_buffer.extend(submissions_set)
 
     def serve_getregex(self, sock: nclib.Netcat):
         sock.sendln(self.FLAG_REGEX)
 
     def serve_gettargets(self, sock: nclib.Netcat):
         script_id = sock.readln(max_size=100, timeout=1).strip().decode()
         script_name = sock.readln(max_size=100, timeout=1).strip().decode()
```

### Comparing `quickscope-0.1.3/quickscope.egg-info/PKG-INFO` & `quickscope-0.1.4/quickscope.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickscope
-Version: 0.1.3
+Version: 0.1.4
 Summary: A lightweight and scalable A/D CTF exploit shooter
 Home-page: https://github.com/shellphish/quickscope
 License: zlib
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Quickscope
```

### Comparing `quickscope-0.1.3/setup.cfg` & `quickscope-0.1.4/setup.cfg`

 * *Files identical despite different names*

