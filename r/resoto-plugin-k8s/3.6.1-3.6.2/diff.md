# Comparing `tmp/resoto-plugin-k8s-3.6.1.tar.gz` & `tmp/resoto-plugin-k8s-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-k8s-3.6.1.tar", last modified: Fri Jul 14 17:05:59 2023, max compression
+gzip compressed data, was "resoto-plugin-k8s-3.6.2.tar", last modified: Fri Jul 21 22:12:20 2023, max compression
```

## Comparing `resoto-plugin-k8s-3.6.1.tar` & `resoto-plugin-k8s-3.6.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:59.821883 resoto-plugin-k8s-3.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-14 17:05:59.821883 resoto-plugin-k8s-3.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:59.821883 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19406 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:59.821883 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/deferred_edges/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/deferred_edges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/deferred_edges/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/deferred_edges/digitalocean.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/deferred_edges/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   106651 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:59.821883 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-14 17:05:59.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-14 17:05:59.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:05:59.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 17:05:59.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:02:43.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 17:05:59.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 17:05:59.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-14 17:05:59.821883 resoto-plugin-k8s-3.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:12:20.122733 resoto-plugin-k8s-3.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 22:06:13.000000 resoto-plugin-k8s-3.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-21 22:12:20.122733 resoto-plugin-k8s-3.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 22:06:13.000000 resoto-plugin-k8s-3.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-21 22:06:13.000000 resoto-plugin-k8s-3.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:12:20.118733 resoto-plugin-k8s-3.6.2/resoto_plugin_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-21 22:06:13.000000 resoto-plugin-k8s-3.6.2/resoto_plugin_k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19406 2023-07-21 22:06:13.000000 resoto-plugin-k8s-3.6.2/resoto_plugin_k8s/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-21 22:06:13.000000 resoto-plugin-k8s-3.6.2/resoto_plugin_k8s/collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:12:20.122733 resoto-plugin-k8s-3.6.2/resoto_plugin_k8s/deferred_edges/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-21 22:06:13.000000 resoto-plugin-k8s-3.6.2/resoto_plugin_k8s/deferred_edges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-21 22:06:13.000000 resoto-plugin-k8s-3.6.2/resoto_plugin_k8s/deferred_edges/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-21 22:06:13.000000 resoto-plugin-k8s-3.6.2/resoto_plugin_k8s/deferred_edges/digitalocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-21 22:06:13.000000 resoto-plugin-k8s-3.6.2/resoto_plugin_k8s/deferred_edges/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106651 2023-07-21 22:06:13.000000 resoto-plugin-k8s-3.6.2/resoto_plugin_k8s/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:12:20.122733 resoto-plugin-k8s-3.6.2/resoto_plugin_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-21 22:12:20.000000 resoto-plugin-k8s-3.6.2/resoto_plugin_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-21 22:12:20.000000 resoto-plugin-k8s-3.6.2/resoto_plugin_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:12:20.000000 resoto-plugin-k8s-3.6.2/resoto_plugin_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-21 22:12:20.000000 resoto-plugin-k8s-3.6.2/resoto_plugin_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:08:02.000000 resoto-plugin-k8s-3.6.2/resoto_plugin_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 22:12:20.000000 resoto-plugin-k8s-3.6.2/resoto_plugin_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 22:12:20.000000 resoto-plugin-k8s-3.6.2/resoto_plugin_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-21 22:12:20.122733 resoto-plugin-k8s-3.6.2/setup.cfg
```

### Comparing `resoto-plugin-k8s-3.6.1/PKG-INFO` & `resoto-plugin-k8s-3.6.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-k8s
-Version: 3.6.1
+Version: 3.6.2
 Summary: Resoto Kubernetes Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-k8s-3.6.1/pyproject.toml` & `resoto-plugin-k8s-3.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-k8s"
 description = "Resoto Kubernetes Collector Plugin"
-version = "3.6.1"
+version = "3.6.2"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.6.1",
+    "resotolib==3.6.2",
     "kubernetes",
 ]
 
 [project.entry-points."resoto.plugins"]
 k8s_collector = "resoto_plugin_k8s:KubernetesCollectorPlugin"
 
 [project.urls]
```

### Comparing `resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/__init__.py` & `resoto-plugin-k8s-3.6.2/resoto_plugin_k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/base.py` & `resoto-plugin-k8s-3.6.2/resoto_plugin_k8s/base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/collector.py` & `resoto-plugin-k8s-3.6.2/resoto_plugin_k8s/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/deferred_edges/__init__.py` & `resoto-plugin-k8s-3.6.2/resoto_plugin_k8s/deferred_edges/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/deferred_edges/aws.py` & `resoto-plugin-k8s-3.6.2/resoto_plugin_k8s/deferred_edges/aws.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/deferred_edges/digitalocean.py` & `resoto-plugin-k8s-3.6.2/resoto_plugin_k8s/deferred_edges/digitalocean.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/resources.py` & `resoto-plugin-k8s-3.6.2/resoto_plugin_k8s/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.6.1/resoto_plugin_k8s.egg-info/PKG-INFO` & `resoto-plugin-k8s-3.6.2/resoto_plugin_k8s.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-k8s
-Version: 3.6.1
+Version: 3.6.2
 Summary: Resoto Kubernetes Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-k8s-3.6.1/resoto_plugin_k8s.egg-info/SOURCES.txt` & `resoto-plugin-k8s-3.6.2/resoto_plugin_k8s.egg-info/SOURCES.txt`

 * *Files identical despite different names*

