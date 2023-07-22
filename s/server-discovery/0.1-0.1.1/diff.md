# Comparing `tmp/server-discovery-0.1.tar.gz` & `tmp/server-discovery-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "server-discovery-0.1.tar", last modified: Sat Jul 22 21:32:06 2023, max compression
+gzip compressed data, was "server-discovery-0.1.1.tar", last modified: Sat Jul 22 21:39:34 2023, max compression
```

## Comparing `server-discovery-0.1.tar` & `server-discovery-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-22 21:32:06.325369 server-discovery-0.1/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      119 2023-07-22 21:32:06.324369 server-discovery-0.1/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1259 2023-07-22 21:24:00.000000 server-discovery-0.1/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)      161 2023-07-22 18:44:41.000000 server-discovery-0.1/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-07-22 21:32:06.325369 server-discovery-0.1/setup.cfg
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-22 21:32:06.311369 server-discovery-0.1/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-22 21:32:06.319369 server-discovery-0.1/src/server_discovery/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      190 2023-07-22 20:48:39.000000 server-discovery-0.1/src/server_discovery/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      860 2023-07-22 21:17:29.000000 server-discovery-0.1/src/server_discovery/_broadcast.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1490 2023-07-22 21:12:56.000000 server-discovery-0.1/src/server_discovery/_client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      495 2023-07-22 20:22:02.000000 server-discovery-0.1/src/server_discovery/_info_model.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1432 2023-07-22 21:11:22.000000 server-discovery-0.1/src/server_discovery/_server.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-22 21:32:06.323369 server-discovery-0.1/src/server_discovery.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      119 2023-07-22 21:32:06.000000 server-discovery-0.1/src/server_discovery.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      411 2023-07-22 21:32:06.000000 server-discovery-0.1/src/server_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-22 21:32:06.000000 server-discovery-0.1/src/server_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       19 2023-07-22 21:32:06.000000 server-discovery-0.1/src/server_discovery.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       17 2023-07-22 21:32:06.000000 server-discovery-0.1/src/server_discovery.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-22 21:39:34.956735 server-discovery-0.1.1/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1502 2023-07-22 21:39:34.955735 server-discovery-0.1.1/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1259 2023-07-22 21:24:00.000000 server-discovery-0.1.1/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      262 2023-07-22 21:39:11.000000 server-discovery-0.1.1/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-07-22 21:39:34.956735 server-discovery-0.1.1/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-22 21:39:34.946735 server-discovery-0.1.1/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-22 21:39:34.951735 server-discovery-0.1.1/src/server_discovery/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      190 2023-07-22 20:48:39.000000 server-discovery-0.1.1/src/server_discovery/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      860 2023-07-22 21:17:29.000000 server-discovery-0.1.1/src/server_discovery/_broadcast.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1490 2023-07-22 21:12:56.000000 server-discovery-0.1.1/src/server_discovery/_client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      495 2023-07-22 20:22:02.000000 server-discovery-0.1.1/src/server_discovery/_info_model.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1432 2023-07-22 21:11:22.000000 server-discovery-0.1.1/src/server_discovery/_server.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-22 21:39:34.954735 server-discovery-0.1.1/src/server_discovery.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1502 2023-07-22 21:39:34.000000 server-discovery-0.1.1/src/server_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      411 2023-07-22 21:39:34.000000 server-discovery-0.1.1/src/server_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-22 21:39:34.000000 server-discovery-0.1.1/src/server_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       19 2023-07-22 21:39:34.000000 server-discovery-0.1.1/src/server_discovery.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       17 2023-07-22 21:39:34.000000 server-discovery-0.1.1/src/server_discovery.egg-info/top_level.txt
```

### Comparing `server-discovery-0.1/README.md` & `server-discovery-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `server-discovery-0.1/src/server_discovery/_broadcast.py` & `server-discovery-0.1.1/src/server_discovery/_broadcast.py`

 * *Files identical despite different names*

### Comparing `server-discovery-0.1/src/server_discovery/_client.py` & `server-discovery-0.1.1/src/server_discovery/_client.py`

 * *Files identical despite different names*

### Comparing `server-discovery-0.1/src/server_discovery/_server.py` & `server-discovery-0.1.1/src/server_discovery/_server.py`

 * *Files identical despite different names*

