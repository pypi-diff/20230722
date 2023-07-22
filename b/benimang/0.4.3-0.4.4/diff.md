# Comparing `tmp/benimang-0.4.3.tar.gz` & `tmp/benimang-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benimang-0.4.3.tar", last modified: Sat Jul 22 01:58:01 2023, max compression
+gzip compressed data, was "benimang-0.4.4.tar", last modified: Sat Jul 22 06:35:41 2023, max compression
```

## Comparing `benimang-0.4.3.tar` & `benimang-0.4.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 01:58:01.071961 benimang-0.4.3/
--rw-rw-rw-   0        0        0       29 2023-07-19 08:32:47.000000 benimang-0.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0      237 2023-07-22 01:58:01.070961 benimang-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 01:58:01.065960 benimang-0.4.3/beni/
--rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/__init__.py
--rw-rw-rw-   0        0        0     6505 2023-07-20 01:41:22.000000 benimang-0.4.3/beni/bbyte.py
--rw-rw-rw-   0        0        0     6308 2023-07-20 02:52:57.000000 benimang-0.4.3/beni/bcache.py
--rw-rw-rw-   0        0        0     1906 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/bcolor.py
--rw-rw-rw-   0        0        0     2460 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/bexecute.py
--rw-rw-rw-   0        0        0     2139 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/bfile.py
--rw-rw-rw-   0        0        0     5047 2023-07-20 03:23:07.000000 benimang-0.4.3/beni/bfunc.py
--rw-rw-rw-   0        0        0     5855 2023-07-20 02:01:20.000000 benimang-0.4.3/beni/bhttp.py
--rw-rw-rw-   0        0        0     2347 2023-07-20 02:15:15.000000 benimang-0.4.3/beni/binput.py
--rw-rw-rw-   0        0        0     5663 2023-07-20 03:23:14.000000 benimang-0.4.3/beni/block.py
--rw-rw-rw-   0        0        0     4175 2023-07-20 02:15:15.000000 benimang-0.4.3/beni/blog.py
--rw-rw-rw-   0        0        0     5664 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/bpath.py
--rw-rw-rw-   0        0        0     2418 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/bplaywright.py
--rw-rw-rw-   0        0        0     1086 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/bprogress.py
--rw-rw-rw-   0        0        0     3845 2023-07-20 03:24:05.000000 benimang-0.4.3/beni/bqiniu.py
--rw-rw-rw-   0        0        0    10523 2023-07-20 01:45:35.000000 benimang-0.4.3/beni/bsqlite.py
--rw-rw-rw-   0        0        0      859 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/bstorage.py
--rw-rw-rw-   0        0        0     1974 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/btable.py
--rw-rw-rw-   0        0        0     4467 2023-07-22 01:55:57.000000 benimang-0.4.3/beni/btask.py
--rw-rw-rw-   0        0        0     1574 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/btime.py
--rw-rw-rw-   0        0        0      390 2023-07-20 02:53:02.000000 benimang-0.4.3/beni/btype.py
--rw-rw-rw-   0        0        0     2391 2023-07-20 02:15:15.000000 benimang-0.4.3/beni/bzip.py
-drwxrwxrwx   0        0        0        0 2023-07-22 01:58:01.068961 benimang-0.4.3/benimang.egg-info/
--rw-rw-rw-   0        0        0      237 2023-07-22 01:58:01.000000 benimang-0.4.3/benimang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-07-22 01:58:01.000000 benimang-0.4.3/benimang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 01:58:01.000000 benimang-0.4.3/benimang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-22 01:58:01.000000 benimang-0.4.3/benimang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      346 2023-07-22 01:57:09.000000 benimang-0.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-22 01:58:01.071961 benimang-0.4.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-22 01:58:01.069961 benimang-0.4.3/test/
--rw-rw-rw-   0        0        0      638 2023-07-19 08:32:47.000000 benimang-0.4.3/test/test_sample.py
+drwxrwxrwx   0        0        0        0 2023-07-22 06:35:41.918487 benimang-0.4.4/
+-rw-rw-rw-   0        0        0       29 2023-07-19 08:32:47.000000 benimang-0.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      237 2023-07-22 06:35:41.918487 benimang-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 06:35:41.912421 benimang-0.4.4/beni/
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.4/beni/__init__.py
+-rw-rw-rw-   0        0        0     6505 2023-07-20 01:41:22.000000 benimang-0.4.4/beni/bbyte.py
+-rw-rw-rw-   0        0        0     6308 2023-07-20 02:52:57.000000 benimang-0.4.4/beni/bcache.py
+-rw-rw-rw-   0        0        0     1906 2023-07-19 08:32:47.000000 benimang-0.4.4/beni/bcolor.py
+-rw-rw-rw-   0        0        0     2460 2023-07-19 08:32:47.000000 benimang-0.4.4/beni/bexecute.py
+-rw-rw-rw-   0        0        0     2139 2023-07-19 08:32:47.000000 benimang-0.4.4/beni/bfile.py
+-rw-rw-rw-   0        0        0     5047 2023-07-20 03:23:07.000000 benimang-0.4.4/beni/bfunc.py
+-rw-rw-rw-   0        0        0     5855 2023-07-20 02:01:20.000000 benimang-0.4.4/beni/bhttp.py
+-rw-rw-rw-   0        0        0     2347 2023-07-20 02:15:15.000000 benimang-0.4.4/beni/binput.py
+-rw-rw-rw-   0        0        0     5663 2023-07-20 03:23:14.000000 benimang-0.4.4/beni/block.py
+-rw-rw-rw-   0        0        0     4175 2023-07-20 02:15:15.000000 benimang-0.4.4/beni/blog.py
+-rw-rw-rw-   0        0        0     5664 2023-07-19 08:32:47.000000 benimang-0.4.4/beni/bpath.py
+-rw-rw-rw-   0        0        0     2418 2023-07-19 08:32:47.000000 benimang-0.4.4/beni/bplaywright.py
+-rw-rw-rw-   0        0        0     1086 2023-07-19 08:32:47.000000 benimang-0.4.4/beni/bprogress.py
+-rw-rw-rw-   0        0        0     3845 2023-07-20 03:24:05.000000 benimang-0.4.4/beni/bqiniu.py
+-rw-rw-rw-   0        0        0    10523 2023-07-20 01:45:35.000000 benimang-0.4.4/beni/bsqlite.py
+-rw-rw-rw-   0        0        0      859 2023-07-19 08:32:47.000000 benimang-0.4.4/beni/bstorage.py
+-rw-rw-rw-   0        0        0     1974 2023-07-19 08:32:47.000000 benimang-0.4.4/beni/btable.py
+-rw-rw-rw-   0        0        0     4460 2023-07-22 06:33:48.000000 benimang-0.4.4/beni/btask.py
+-rw-rw-rw-   0        0        0     1574 2023-07-22 06:33:25.000000 benimang-0.4.4/beni/btime.py
+-rw-rw-rw-   0        0        0      390 2023-07-20 02:53:02.000000 benimang-0.4.4/beni/btype.py
+-rw-rw-rw-   0        0        0     2391 2023-07-20 02:15:15.000000 benimang-0.4.4/beni/bzip.py
+drwxrwxrwx   0        0        0        0 2023-07-22 06:35:41.916422 benimang-0.4.4/benimang.egg-info/
+-rw-rw-rw-   0        0        0      237 2023-07-22 06:35:41.000000 benimang-0.4.4/benimang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2023-07-22 06:35:41.000000 benimang-0.4.4/benimang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 06:35:41.000000 benimang-0.4.4/benimang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-22 06:35:41.000000 benimang-0.4.4/benimang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      346 2023-07-22 06:34:38.000000 benimang-0.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-22 06:35:41.918487 benimang-0.4.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-22 06:35:41.917422 benimang-0.4.4/test/
+-rw-rw-rw-   0        0        0      638 2023-07-19 08:32:47.000000 benimang-0.4.4/test/test_sample.py
```

### Comparing `benimang-0.4.3/beni/bbyte.py` & `benimang-0.4.4/beni/bbyte.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/beni/bcache.py` & `benimang-0.4.4/beni/bcache.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/beni/bcolor.py` & `benimang-0.4.4/beni/bcolor.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/beni/bexecute.py` & `benimang-0.4.4/beni/bexecute.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/beni/bfile.py` & `benimang-0.4.4/beni/bfile.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/beni/bfunc.py` & `benimang-0.4.4/beni/bfunc.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/beni/bhttp.py` & `benimang-0.4.4/beni/bhttp.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/beni/binput.py` & `benimang-0.4.4/beni/binput.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/beni/block.py` & `benimang-0.4.4/beni/block.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/beni/blog.py` & `benimang-0.4.4/beni/blog.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/beni/bpath.py` & `benimang-0.4.4/beni/bpath.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/beni/bplaywright.py` & `benimang-0.4.4/beni/bplaywright.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/beni/bprogress.py` & `benimang-0.4.4/beni/bprogress.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/beni/bqiniu.py` & `benimang-0.4.4/beni/bqiniu.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/beni/bsqlite.py` & `benimang-0.4.4/beni/bsqlite.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/beni/bstorage.py` & `benimang-0.4.4/beni/bstorage.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/beni/btable.py` & `benimang-0.4.4/beni/btable.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/beni/btask.py` & `benimang-0.4.4/beni/btask.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import sys
 from contextlib import asynccontextmanager
 from dataclasses import dataclass
 from datetime import datetime as Datetime
 from pathlib import Path
-from typing import Final
+from typing import Any, Final
 
 import nest_asyncio
 from colorama import Fore
 from typer import Typer
 
 from beni import bcolor, bfunc, block, blog, bpath, btime
 from beni.btype import Null
@@ -54,21 +54,21 @@
                     # 2 - Error: Missing command.
                     pass
                 else:
                     raise
     asyncio.run(func())
 
 
-def dev(name: str):
+def dev(name: str, *args: Any, **kwargs: Any):
     '例：db.reverse'
     async def func():
         async with _task():
             module, cmd = name.split('.')
             exec(f'from {options.package} import {module}')
-            exec(f'{module}.{cmd}()')
+            eval(f'{module}.{cmd}')(*args, **kwargs)
     asyncio.run(func())
 
 
 @asynccontextmanager
 async def _task():
     _checkVscodeVenv()
     bfunc.sysUtf8()
@@ -98,29 +98,27 @@
                 color = Fore.LIGHTMAGENTA_EX
             elif errorNum:
                 color = Fore.LIGHTRED_EX
             elif warningNum:
                 color = Fore.YELLOW
             else:
                 color = Fore.LIGHTGREEN_EX
-            bcolor.set(color)
-            blog.info('-' * 75)
-            msgAry = ['任务结束']
+            msgAry = ['', '-' * 75]
             if criticalNum:
-                msgAry.append(f'critical({criticalNum})')
+                msgAry.append(f'critical：{criticalNum}')
             if errorNum:
-                msgAry.append(f'error({errorNum})')
+                msgAry.append(f'error：{errorNum}')
             if warningNum:
-                msgAry.append(f'warning({warningNum})')
+                msgAry.append(f'warning：{warningNum}')
             duration = str(Datetime.now() - start_time)
             if duration.startswith('0:'):
                 duration = '0' + duration
-            msgAry.append(f'\n用时: {duration}')
+            msgAry.append(f'任务结束（{duration}）')
             bcolor.set(color)
-            blog.info(' '.join(msgAry))
+            blog.info('\n'.join(msgAry))
 
             # 删除多余的日志
             try:
                 if logFile:
                     logFileAry = list(logFile.parent.glob('*.log'))
                     logFileAry.remove(logFile)
                     logFileAry.sort()
```

### Comparing `benimang-0.4.3/beni/btime.py` & `benimang-0.4.4/beni/btime.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/beni/bzip.py` & `benimang-0.4.4/beni/bzip.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/benimang.egg-info/SOURCES.txt` & `benimang-0.4.4/benimang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `benimang-0.4.3/test/test_sample.py` & `benimang-0.4.4/test/test_sample.py`

 * *Files identical despite different names*

