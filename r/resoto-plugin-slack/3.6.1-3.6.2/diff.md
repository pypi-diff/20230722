# Comparing `tmp/resoto-plugin-slack-3.6.1.tar.gz` & `tmp/resoto-plugin-slack-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-slack-3.6.1.tar", last modified: Fri Jul 14 17:00:06 2023, max compression
+gzip compressed data, was "resoto-plugin-slack-3.6.2.tar", last modified: Fri Jul 21 22:15:51 2023, max compression
```

## Comparing `resoto-plugin-slack-3.6.1.tar` & `resoto-plugin-slack-3.6.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:06.174583 resoto-plugin-slack-3.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 16:56:01.000000 resoto-plugin-slack-3.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-14 17:00:06.174583 resoto-plugin-slack-3.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 16:56:01.000000 resoto-plugin-slack-3.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-14 16:56:01.000000 resoto-plugin-slack-3.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:06.174583 resoto-plugin-slack-3.6.1/resoto_plugin_slack/
--rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-07-14 16:56:01.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-14 16:56:01.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-07-14 16:56:01.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:06.174583 resoto-plugin-slack-3.6.1/resoto_plugin_slack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-14 17:00:06.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-14 17:00:06.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:00:06.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-14 17:00:06.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:57:38.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-14 17:00:06.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 17:00:06.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-14 17:00:06.178583 resoto-plugin-slack-3.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:06.174583 resoto-plugin-slack-3.6.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-14 16:56:01.000000 resoto-plugin-slack-3.6.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:15:51.359304 resoto-plugin-slack-3.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 22:11:07.000000 resoto-plugin-slack-3.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-21 22:15:51.359304 resoto-plugin-slack-3.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-21 22:11:07.000000 resoto-plugin-slack-3.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-21 22:11:07.000000 resoto-plugin-slack-3.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:15:51.359304 resoto-plugin-slack-3.6.2/resoto_plugin_slack/
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-07-21 22:11:07.000000 resoto-plugin-slack-3.6.2/resoto_plugin_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-21 22:11:07.000000 resoto-plugin-slack-3.6.2/resoto_plugin_slack/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-07-21 22:11:07.000000 resoto-plugin-slack-3.6.2/resoto_plugin_slack/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:15:51.359304 resoto-plugin-slack-3.6.2/resoto_plugin_slack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-21 22:15:51.000000 resoto-plugin-slack-3.6.2/resoto_plugin_slack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-21 22:15:51.000000 resoto-plugin-slack-3.6.2/resoto_plugin_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:15:51.000000 resoto-plugin-slack-3.6.2/resoto_plugin_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-21 22:15:51.000000 resoto-plugin-slack-3.6.2/resoto_plugin_slack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:13:01.000000 resoto-plugin-slack-3.6.2/resoto_plugin_slack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-21 22:15:51.000000 resoto-plugin-slack-3.6.2/resoto_plugin_slack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-21 22:15:51.000000 resoto-plugin-slack-3.6.2/resoto_plugin_slack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 22:15:51.359304 resoto-plugin-slack-3.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:15:51.359304 resoto-plugin-slack-3.6.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-21 22:11:07.000000 resoto-plugin-slack-3.6.2/test/test_config.py
```

### Comparing `resoto-plugin-slack-3.6.1/PKG-INFO` & `resoto-plugin-slack-3.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-slack
-Version: 3.6.1
+Version: 3.6.2
 Summary: Resoto Slack Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/slack
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-slack-3.6.1/pyproject.toml` & `resoto-plugin-slack-3.6.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-slack"
 description = "Resoto Slack Plugin"
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
     "slack-sdk",
     "retrying",
 ]
 
 [project.entry-points."resoto.plugins"]
 slack_bot = "resoto_plugin_slack:SlackBotPlugin"
 slack_collector = "resoto_plugin_slack:SlackCollectorPlugin"
```

### Comparing `resoto-plugin-slack-3.6.1/resoto_plugin_slack/__init__.py` & `resoto-plugin-slack-3.6.2/resoto_plugin_slack/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-slack-3.6.1/resoto_plugin_slack/resources.py` & `resoto-plugin-slack-3.6.2/resoto_plugin_slack/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-slack-3.6.1/resoto_plugin_slack.egg-info/PKG-INFO` & `resoto-plugin-slack-3.6.2/resoto_plugin_slack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-slack
-Version: 3.6.1
+Version: 3.6.2
 Summary: Resoto Slack Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/slack
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

