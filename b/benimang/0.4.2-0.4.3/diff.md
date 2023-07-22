# Comparing `tmp/benimang-0.4.2.tar.gz` & `tmp/benimang-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benimang-0.4.2.tar", last modified: Fri Jul 21 01:41:29 2023, max compression
+gzip compressed data, was "benimang-0.4.3.tar", last modified: Sat Jul 22 01:58:01 2023, max compression
```

## Comparing `benimang-0.4.2.tar` & `benimang-0.4.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 01:41:29.180384 benimang-0.4.2/
--rw-rw-rw-   0        0        0       29 2023-07-19 08:32:47.000000 benimang-0.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0      237 2023-07-21 01:41:29.179382 benimang-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 01:41:29.173381 benimang-0.4.2/beni/
--rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/__init__.py
--rw-rw-rw-   0        0        0     6505 2023-07-20 01:41:22.000000 benimang-0.4.2/beni/bbyte.py
--rw-rw-rw-   0        0        0     6308 2023-07-20 02:52:57.000000 benimang-0.4.2/beni/bcache.py
--rw-rw-rw-   0        0        0     1906 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/bcolor.py
--rw-rw-rw-   0        0        0     2460 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/bexecute.py
--rw-rw-rw-   0        0        0     2139 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/bfile.py
--rw-rw-rw-   0        0        0     5047 2023-07-20 03:23:07.000000 benimang-0.4.2/beni/bfunc.py
--rw-rw-rw-   0        0        0     5855 2023-07-20 02:01:20.000000 benimang-0.4.2/beni/bhttp.py
--rw-rw-rw-   0        0        0     2347 2023-07-20 02:15:15.000000 benimang-0.4.2/beni/binput.py
--rw-rw-rw-   0        0        0     5663 2023-07-20 03:23:14.000000 benimang-0.4.2/beni/block.py
--rw-rw-rw-   0        0        0     4175 2023-07-20 02:15:15.000000 benimang-0.4.2/beni/blog.py
--rw-rw-rw-   0        0        0     5664 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/bpath.py
--rw-rw-rw-   0        0        0     2418 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/bplaywright.py
--rw-rw-rw-   0        0        0     1086 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/bprogress.py
--rw-rw-rw-   0        0        0     3845 2023-07-20 03:24:05.000000 benimang-0.4.2/beni/bqiniu.py
--rw-rw-rw-   0        0        0    10523 2023-07-20 01:45:35.000000 benimang-0.4.2/beni/bsqlite.py
--rw-rw-rw-   0        0        0      859 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/bstorage.py
--rw-rw-rw-   0        0        0     1974 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/btable.py
--rw-rw-rw-   0        0        0     4871 2023-07-21 01:29:06.000000 benimang-0.4.2/beni/btask.py
--rw-rw-rw-   0        0        0     1574 2023-07-19 08:32:47.000000 benimang-0.4.2/beni/btime.py
--rw-rw-rw-   0        0        0      390 2023-07-20 02:53:02.000000 benimang-0.4.2/beni/btype.py
--rw-rw-rw-   0        0        0     2391 2023-07-20 02:15:15.000000 benimang-0.4.2/beni/bzip.py
-drwxrwxrwx   0        0        0        0 2023-07-21 01:41:29.177382 benimang-0.4.2/benimang.egg-info/
--rw-rw-rw-   0        0        0      237 2023-07-21 01:41:29.000000 benimang-0.4.2/benimang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-07-21 01:41:29.000000 benimang-0.4.2/benimang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 01:41:29.000000 benimang-0.4.2/benimang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-21 01:41:29.000000 benimang-0.4.2/benimang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      346 2023-07-21 01:31:52.000000 benimang-0.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-21 01:41:29.180384 benimang-0.4.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-21 01:41:29.178382 benimang-0.4.2/test/
--rw-rw-rw-   0        0        0      638 2023-07-19 08:32:47.000000 benimang-0.4.2/test/test_sample.py
+drwxrwxrwx   0        0        0        0 2023-07-22 01:58:01.071961 benimang-0.4.3/
+-rw-rw-rw-   0        0        0       29 2023-07-19 08:32:47.000000 benimang-0.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      237 2023-07-22 01:58:01.070961 benimang-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 01:58:01.065960 benimang-0.4.3/beni/
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/__init__.py
+-rw-rw-rw-   0        0        0     6505 2023-07-20 01:41:22.000000 benimang-0.4.3/beni/bbyte.py
+-rw-rw-rw-   0        0        0     6308 2023-07-20 02:52:57.000000 benimang-0.4.3/beni/bcache.py
+-rw-rw-rw-   0        0        0     1906 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/bcolor.py
+-rw-rw-rw-   0        0        0     2460 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/bexecute.py
+-rw-rw-rw-   0        0        0     2139 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/bfile.py
+-rw-rw-rw-   0        0        0     5047 2023-07-20 03:23:07.000000 benimang-0.4.3/beni/bfunc.py
+-rw-rw-rw-   0        0        0     5855 2023-07-20 02:01:20.000000 benimang-0.4.3/beni/bhttp.py
+-rw-rw-rw-   0        0        0     2347 2023-07-20 02:15:15.000000 benimang-0.4.3/beni/binput.py
+-rw-rw-rw-   0        0        0     5663 2023-07-20 03:23:14.000000 benimang-0.4.3/beni/block.py
+-rw-rw-rw-   0        0        0     4175 2023-07-20 02:15:15.000000 benimang-0.4.3/beni/blog.py
+-rw-rw-rw-   0        0        0     5664 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/bpath.py
+-rw-rw-rw-   0        0        0     2418 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/bplaywright.py
+-rw-rw-rw-   0        0        0     1086 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/bprogress.py
+-rw-rw-rw-   0        0        0     3845 2023-07-20 03:24:05.000000 benimang-0.4.3/beni/bqiniu.py
+-rw-rw-rw-   0        0        0    10523 2023-07-20 01:45:35.000000 benimang-0.4.3/beni/bsqlite.py
+-rw-rw-rw-   0        0        0      859 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/bstorage.py
+-rw-rw-rw-   0        0        0     1974 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/btable.py
+-rw-rw-rw-   0        0        0     4467 2023-07-22 01:55:57.000000 benimang-0.4.3/beni/btask.py
+-rw-rw-rw-   0        0        0     1574 2023-07-19 08:32:47.000000 benimang-0.4.3/beni/btime.py
+-rw-rw-rw-   0        0        0      390 2023-07-20 02:53:02.000000 benimang-0.4.3/beni/btype.py
+-rw-rw-rw-   0        0        0     2391 2023-07-20 02:15:15.000000 benimang-0.4.3/beni/bzip.py
+drwxrwxrwx   0        0        0        0 2023-07-22 01:58:01.068961 benimang-0.4.3/benimang.egg-info/
+-rw-rw-rw-   0        0        0      237 2023-07-22 01:58:01.000000 benimang-0.4.3/benimang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2023-07-22 01:58:01.000000 benimang-0.4.3/benimang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 01:58:01.000000 benimang-0.4.3/benimang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-22 01:58:01.000000 benimang-0.4.3/benimang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      346 2023-07-22 01:57:09.000000 benimang-0.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-22 01:58:01.071961 benimang-0.4.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-22 01:58:01.069961 benimang-0.4.3/test/
+-rw-rw-rw-   0        0        0      638 2023-07-19 08:32:47.000000 benimang-0.4.3/test/test_sample.py
```

### Comparing `benimang-0.4.2/beni/bbyte.py` & `benimang-0.4.3/beni/bbyte.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/beni/bcache.py` & `benimang-0.4.3/beni/bcache.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/beni/bcolor.py` & `benimang-0.4.3/beni/bcolor.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/beni/bexecute.py` & `benimang-0.4.3/beni/bexecute.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/beni/bfile.py` & `benimang-0.4.3/beni/bfile.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/beni/bfunc.py` & `benimang-0.4.3/beni/bfunc.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/beni/bhttp.py` & `benimang-0.4.3/beni/bhttp.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/beni/binput.py` & `benimang-0.4.3/beni/binput.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/beni/block.py` & `benimang-0.4.3/beni/block.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/beni/blog.py` & `benimang-0.4.3/beni/blog.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/beni/bpath.py` & `benimang-0.4.3/beni/bpath.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/beni/bplaywright.py` & `benimang-0.4.3/beni/bplaywright.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/beni/bprogress.py` & `benimang-0.4.3/beni/bprogress.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/beni/bqiniu.py` & `benimang-0.4.3/beni/bqiniu.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/beni/bsqlite.py` & `benimang-0.4.3/beni/bsqlite.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/beni/bstorage.py` & `benimang-0.4.3/beni/bstorage.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/beni/btable.py` & `benimang-0.4.3/beni/btable.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/beni/btask.py` & `benimang-0.4.3/beni/btask.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,51 @@
 import asyncio
-import inspect
 import sys
 from contextlib import asynccontextmanager
+from dataclasses import dataclass
 from datetime import datetime as Datetime
 from pathlib import Path
+from typing import Final
 
 import nest_asyncio
 from colorama import Fore
 from typer import Typer
 
 from beni import bcolor, bfunc, block, blog, bpath, btime
 from beni.btype import Null
 
 app = Typer()
-_LOGFILE_COUNT = 100
-_TASKS = 'tasks'
 
 nest_asyncio.apply()
 
-_key: str = 'btask'
-_logDir: Path = Null
-_binDir: Path = Null
-
-
-@bfunc.onceCall
-def init(
-    *,
-    key: str = '',
-    logDir: Path | str = '',
-    binDir: Path | str = ''
-):
-    global _key, _logDir, _binDir
-    if key:
-        _key = key
-    if logDir:
-        _logDir = bpath.get(logDir)
-    if binDir:
-        _binDir = bpath.get(binDir)
+
+@dataclass
+class _Options:
+    tasksPath: Path = Null
+    lock: str = 'btask'
+    package: str = 'tasks'
+    logPath: Path = Null
+    binPath: Path = Null
+    logFilesLimit: int = 100
+
+
+options: Final = _Options()
 
 
 def main():
+    assert options.tasksPath, '请先设置 options.mainFile'
+
     async def func():
         async with _task():
             try:
-                tasksDir = _getRootDir() / _TASKS
-                files = tasksDir.glob('*.py')
+                files = options.tasksPath.glob('*.py')
                 files = filter(lambda x: not x.name.startswith('_'), files)
                 for moduleName in [x.stem for x in files]:
-                    exec(f'import {_TASKS}.{moduleName}')
-                    module = eval(f'{_TASKS}.{moduleName}')
+                    exec(f'import {options.package}.{moduleName}')
+                    module = eval(f'{options.package}.{moduleName}')
                     if hasattr(module, 'app'):
                         sub: Typer = getattr(module, 'app')
                         if sub is not app:
                             sub.info.name = moduleName.replace('_', '-')
                             app.add_typer(sub, name=sub.info.name)
                 app()
             except BaseException as ex:
@@ -66,30 +59,30 @@
 
 
 def dev(name: str):
     '例：db.reverse'
     async def func():
         async with _task():
             module, cmd = name.split('.')
-            exec(f'from {_TASKS} import {module}')
+            exec(f'from {options.package} import {module}')
             exec(f'{module}.{cmd}()')
     asyncio.run(func())
 
 
 @asynccontextmanager
 async def _task():
     _checkVscodeVenv()
     bfunc.sysUtf8()
-    if _binDir:
-        bfunc.addEnvPath(_binDir)
-    async with block.useFileLock(_key):
+    if options.binPath:
+        bfunc.addEnvPath(options.binPath)
+    async with block.useFileLock(options.lock):
         start_time = Datetime.now()
         bfunc.initErrorFormat()
-        if _logDir:
-            logFile = bpath.get(_logDir, btime.datetimeStr('%Y%m%d_%H%M%S.log'))
+        if options.logPath:
+            logFile = bpath.get(options.logPath, btime.datetimeStr('%Y%m%d_%H%M%S.log'))
             assert logFile.is_file(), f'日志文件创建失败（已存在） {logFile}'
         else:
             logFile = None
         try:
             blog.init(logFile=logFile)
             yield
         except BaseException as ex:
@@ -127,31 +120,19 @@
 
             # 删除多余的日志
             try:
                 if logFile:
                     logFileAry = list(logFile.parent.glob('*.log'))
                     logFileAry.remove(logFile)
                     logFileAry.sort()
-                    logFileAry = logFileAry[_LOGFILE_COUNT:]
+                    logFileAry = logFileAry[options.logFilesLimit:]
                     await bpath.remove(*logFileAry)
             except:
                 pass
 
 
-def _getRootDir():
-    frametype = inspect.currentframe()
-    target = frametype
-    while True:
-        assert target and target.f_back
-        target = target.f_back
-        if target.f_locals.get('__name__') == '__main__':
-            file = target.f_locals.get('__file__')
-            if type(file) is str:
-                return bpath.get(file).parent
-
-
 def _checkVscodeVenv():
     par = '--vscode-venv'
     if par in sys.argv:
         sys.argv.remove(par)
         sys.orig_argv.remove(par)
         input('回车后继续（为了兼容vscode venv问题）...')
```

### Comparing `benimang-0.4.2/beni/btime.py` & `benimang-0.4.3/beni/btime.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/beni/bzip.py` & `benimang-0.4.3/beni/bzip.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/benimang.egg-info/SOURCES.txt` & `benimang-0.4.3/benimang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `benimang-0.4.2/test/test_sample.py` & `benimang-0.4.3/test/test_sample.py`

 * *Files identical despite different names*

