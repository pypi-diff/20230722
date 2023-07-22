# Comparing `tmp/terminal_manager-0.8.4.tar.gz` & `tmp/terminal_manager-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_manager-0.8.4.tar", last modified: Sat Jul 22 01:45:41 2023, max compression
+gzip compressed data, was "terminal_manager-0.8.5.tar", last modified: Sat Jul 22 08:23:49 2023, max compression
```

## Comparing `terminal_manager-0.8.4.tar` & `terminal_manager-0.8.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-22 01:45:41.178071 terminal_manager-0.8.4/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.8.4/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-22 01:45:41.178071 terminal_manager-0.8.4/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.8.4/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      706 2023-07-22 01:43:23.000000 terminal_manager-0.8.4/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-22 01:45:41.178071 terminal_manager-0.8.4/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-22 01:45:41.174071 terminal_manager-0.8.4/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-22 01:45:41.178071 terminal_manager-0.8.4/src/terminal_manager/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     7023 2023-07-21 08:57:24.000000 terminal_manager-0.8.4/src/terminal_manager/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-19 08:12:41.000000 terminal_manager-0.8.4/src/terminal_manager/collection.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     6319 2023-07-19 08:12:41.000000 terminal_manager-0.8.4/src/terminal_manager/command.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-22 01:45:41.178071 terminal_manager-0.8.4/src/terminal_manager/default_collections/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-19 08:12:41.000000 terminal_manager-0.8.4/src/terminal_manager/default_collections/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1084 2023-07-21 07:29:28.000000 terminal_manager-0.8.4/src/terminal_manager/default_collections/const.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4371 2023-07-19 08:12:41.000000 terminal_manager-0.8.4/src/terminal_manager/default_collections/linux.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5206 2023-07-19 08:12:41.000000 terminal_manager-0.8.4/src/terminal_manager/default_collections/windows_cmd.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5368 2023-07-19 08:12:41.000000 terminal_manager-0.8.4/src/terminal_manager/default_collections/windows_ps.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-19 08:12:41.000000 terminal_manager-0.8.4/src/terminal_manager/errors.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-19 08:12:41.000000 terminal_manager-0.8.4/src/terminal_manager/event.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-19 08:12:41.000000 terminal_manager-0.8.4/src/terminal_manager/helpers.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8379 2023-07-22 01:20:47.000000 terminal_manager-0.8.4/src/terminal_manager/sensor.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-07-19 08:12:41.000000 terminal_manager-0.8.4/src/terminal_manager/synchronizer.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-22 01:45:41.178071 terminal_manager-0.8.4/src/terminal_manager.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-22 01:45:41.000000 terminal_manager-0.8.4/src/terminal_manager.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-07-22 01:45:41.000000 terminal_manager-0.8.4/src/terminal_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-22 01:45:41.000000 terminal_manager-0.8.4/src/terminal_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-07-22 01:45:41.000000 terminal_manager-0.8.4/src/terminal_manager.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-07-22 01:45:41.000000 terminal_manager-0.8.4/src/terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-22 08:23:49.878153 terminal_manager-0.8.5/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.8.5/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-22 08:23:49.878153 terminal_manager-0.8.5/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.8.5/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      706 2023-07-22 08:01:52.000000 terminal_manager-0.8.5/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-22 08:23:49.878153 terminal_manager-0.8.5/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-22 08:23:49.870154 terminal_manager-0.8.5/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-22 08:23:49.874153 terminal_manager-0.8.5/src/terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     7023 2023-07-22 07:37:31.000000 terminal_manager-0.8.5/src/terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-22 07:37:35.000000 terminal_manager-0.8.5/src/terminal_manager/collection.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     6319 2023-07-22 07:37:39.000000 terminal_manager-0.8.5/src/terminal_manager/command.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-22 08:23:49.878153 terminal_manager-0.8.5/src/terminal_manager/default_collections/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-22 07:38:24.000000 terminal_manager-0.8.5/src/terminal_manager/default_collections/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1084 2023-07-22 07:38:26.000000 terminal_manager-0.8.5/src/terminal_manager/default_collections/const.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4371 2023-07-22 07:38:30.000000 terminal_manager-0.8.5/src/terminal_manager/default_collections/linux.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5206 2023-07-22 07:38:33.000000 terminal_manager-0.8.5/src/terminal_manager/default_collections/windows_cmd.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5368 2023-07-22 07:38:37.000000 terminal_manager-0.8.5/src/terminal_manager/default_collections/windows_ps.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-22 07:37:41.000000 terminal_manager-0.8.5/src/terminal_manager/errors.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-22 07:37:44.000000 terminal_manager-0.8.5/src/terminal_manager/event.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-22 07:38:08.000000 terminal_manager-0.8.5/src/terminal_manager/helpers.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8379 2023-07-22 07:38:13.000000 terminal_manager-0.8.5/src/terminal_manager/sensor.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-07-22 07:38:18.000000 terminal_manager-0.8.5/src/terminal_manager/synchronizer.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-22 08:23:49.874153 terminal_manager-0.8.5/src/terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-22 08:23:49.000000 terminal_manager-0.8.5/src/terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-07-22 08:23:49.000000 terminal_manager-0.8.5/src/terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-22 08:23:49.000000 terminal_manager-0.8.5/src/terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-07-22 08:23:49.000000 terminal_manager-0.8.5/src/terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-07-22 08:23:49.000000 terminal_manager-0.8.5/src/terminal_manager.egg-info/top_level.txt
```

### Comparing `terminal_manager-0.8.4/LICENSE` & `terminal_manager-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.4/PKG-INFO` & `terminal_manager-0.8.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal_manager
-Version: 0.8.4
+Version: 0.8.5
 Summary: Use terminal commands to control and monitor devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `terminal_manager-0.8.4/pyproject.toml` & `terminal_manager-0.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terminal_manager"
-version = "0.8.4"
+version = "0.8.5"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Use terminal commands to control and monitor devices"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `terminal_manager-0.8.4/src/terminal_manager/__init__.py` & `terminal_manager-0.8.5/src/terminal_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.4/src/terminal_manager/collection.py` & `terminal_manager-0.8.5/src/terminal_manager/collection.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.4/src/terminal_manager/command.py` & `terminal_manager-0.8.5/src/terminal_manager/command.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.4/src/terminal_manager/default_collections/const.py` & `terminal_manager-0.8.5/src/terminal_manager/default_collections/const.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.4/src/terminal_manager/default_collections/linux.py` & `terminal_manager-0.8.5/src/terminal_manager/default_collections/linux.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.4/src/terminal_manager/default_collections/windows_cmd.py` & `terminal_manager-0.8.5/src/terminal_manager/default_collections/windows_cmd.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.4/src/terminal_manager/default_collections/windows_ps.py` & `terminal_manager-0.8.5/src/terminal_manager/default_collections/windows_ps.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.4/src/terminal_manager/event.py` & `terminal_manager-0.8.5/src/terminal_manager/event.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.4/src/terminal_manager/sensor.py` & `terminal_manager-0.8.5/src/terminal_manager/sensor.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.4/src/terminal_manager/synchronizer.py` & `terminal_manager-0.8.5/src/terminal_manager/synchronizer.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.4/src/terminal_manager.egg-info/PKG-INFO` & `terminal_manager-0.8.5/src/terminal_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-manager
-Version: 0.8.4
+Version: 0.8.5
 Summary: Use terminal commands to control and monitor devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `terminal_manager-0.8.4/src/terminal_manager.egg-info/SOURCES.txt` & `terminal_manager-0.8.5/src/terminal_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

