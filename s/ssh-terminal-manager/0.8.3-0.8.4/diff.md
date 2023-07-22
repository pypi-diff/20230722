# Comparing `tmp/ssh_terminal_manager-0.8.3.tar.gz` & `tmp/ssh_terminal_manager-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_terminal_manager-0.8.3.tar", last modified: Wed Jul 19 07:59:00 2023, max compression
+gzip compressed data, was "ssh_terminal_manager-0.8.4.tar", last modified: Sat Jul 22 01:49:38 2023, max compression
```

## Comparing `ssh_terminal_manager-0.8.3.tar` & `ssh_terminal_manager-0.8.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-19 07:59:00.682728 ssh_terminal_manager-0.8.3/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.8.3/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-19 07:59:00.682728 ssh_terminal_manager-0.8.3/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      223 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.8.3/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      802 2023-07-19 07:58:10.000000 ssh_terminal_manager-0.8.3/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-19 07:59:00.682728 ssh_terminal_manager-0.8.3/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-19 07:59:00.678728 ssh_terminal_manager-0.8.3/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-19 07:59:00.682728 ssh_terminal_manager-0.8.3/src/ssh_terminal_manager/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8726 2023-07-17 08:57:09.000000 ssh_terminal_manager-0.8.3/src/ssh_terminal_manager/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      393 2023-07-17 08:57:09.000000 ssh_terminal_manager-0.8.3/src/ssh_terminal_manager/errors.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-19 07:59:00.682728 ssh_terminal_manager-0.8.3/src/ssh_terminal_manager.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-19 07:59:00.000000 ssh_terminal_manager-0.8.3/src/ssh_terminal_manager.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      343 2023-07-19 07:59:00.000000 ssh_terminal_manager-0.8.3/src/ssh_terminal_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-19 07:59:00.000000 ssh_terminal_manager-0.8.3/src/ssh_terminal_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       70 2023-07-19 07:59:00.000000 ssh_terminal_manager-0.8.3/src/ssh_terminal_manager.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       21 2023-07-19 07:59:00.000000 ssh_terminal_manager-0.8.3/src/ssh_terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-22 01:49:38.595806 ssh_terminal_manager-0.8.4/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.8.4/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-22 01:49:38.595806 ssh_terminal_manager-0.8.4/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      223 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.8.4/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      802 2023-07-22 01:47:50.000000 ssh_terminal_manager-0.8.4/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-22 01:49:38.595806 ssh_terminal_manager-0.8.4/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-22 01:49:38.591807 ssh_terminal_manager-0.8.4/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-22 01:49:38.595806 ssh_terminal_manager-0.8.4/src/ssh_terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8748 2023-07-21 08:58:13.000000 ssh_terminal_manager-0.8.4/src/ssh_terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      393 2023-07-19 08:12:41.000000 ssh_terminal_manager-0.8.4/src/ssh_terminal_manager/errors.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-22 01:49:38.595806 ssh_terminal_manager-0.8.4/src/ssh_terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-22 01:49:38.000000 ssh_terminal_manager-0.8.4/src/ssh_terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      343 2023-07-22 01:49:38.000000 ssh_terminal_manager-0.8.4/src/ssh_terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-22 01:49:38.000000 ssh_terminal_manager-0.8.4/src/ssh_terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       70 2023-07-22 01:49:38.000000 ssh_terminal_manager-0.8.4/src/ssh_terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       21 2023-07-22 01:49:38.000000 ssh_terminal_manager-0.8.4/src/ssh_terminal_manager.egg-info/top_level.txt
```

### Comparing `ssh_terminal_manager-0.8.3/LICENSE` & `ssh_terminal_manager-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.8.3/PKG-INFO` & `ssh_terminal_manager-0.8.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh_terminal_manager
-Version: 0.8.3
+Version: 0.8.4
 Summary: Use terminal commands to control and monitor remote devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
 Keywords: ssh,terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssh_terminal_manager-0.8.3/pyproject.toml` & `ssh_terminal_manager-0.8.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_terminal_manager"
-version = "0.8.3"
+version = "0.8.4"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Use terminal commands to control and monitor remote devices"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -20,14 +20,14 @@
   "ssh", 
   "terminal", 
   "command line",
 ]
 dependencies = [
   "icmplib >= 3.0",
   "paramiko >= 3.2.0",
-  "terminal-manager >= 0.8.3",
+  "terminal-manager >= 0.8.4",
   "wakeonlan >= 3.0.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/zhbjsh/ssh-terminal-manager"
 "Bug Tracker" = "https://github.com/zhbjsh/ssh-terminal-manager/issues"
```

### Comparing `ssh_terminal_manager-0.8.3/src/ssh_terminal_manager/__init__.py` & `ssh_terminal_manager-0.8.4/src/ssh_terminal_manager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import icmplib
 import paramiko
 import wakeonlan
 from terminal_manager import (
     DEFAULT_ALLOW_TURN_OFF,
     DEFAULT_COMMAND_TIMEOUT,
+    PLACEHOLDER_KEY,
     ActionCommand,
     BinarySensor,
     Collection,
     Command,
     CommandError,
     CommandOutput,
     Event,
```

### Comparing `ssh_terminal_manager-0.8.3/src/ssh_terminal_manager.egg-info/PKG-INFO` & `ssh_terminal_manager-0.8.4/src/ssh_terminal_manager.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-terminal-manager
-Version: 0.8.3
+Version: 0.8.4
 Summary: Use terminal commands to control and monitor remote devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
 Keywords: ssh,terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

