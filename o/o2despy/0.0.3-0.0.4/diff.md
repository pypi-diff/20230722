# Comparing `tmp/o2despy-0.0.3.tar.gz` & `tmp/o2despy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "o2despy-0.0.3.tar", last modified: Wed Feb  1 14:46:31 2023, max compression
+gzip compressed data, was "o2despy-0.0.4.tar", last modified: Sat Jul 22 09:04:35 2023, max compression
```

## Comparing `o2despy-0.0.3.tar` & `o2despy-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-02-01 14:46:31.960699 o2despy-0.0.3/
--rw-rw-rw-   0        0        0     1117 2023-01-31 09:11:19.000000 o2despy-0.0.3/License.txt
--rw-rw-rw-   0        0        0      225 2023-02-01 14:46:31.956666 o2despy-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4947 2023-01-31 09:11:22.000000 o2despy-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-01 14:46:31.917666 o2despy-0.0.3/o2despy/
--rw-rw-rw-   0        0        0     3567 2023-02-01 12:42:55.000000 o2despy-0.0.3/o2despy/action.py
--rw-rw-rw-   0        0        0     1383 2023-02-01 12:43:01.000000 o2despy-0.0.3/o2despy/assets.py
--rw-rw-rw-   0        0        0     2636 2023-02-01 12:42:58.000000 o2despy-0.0.3/o2despy/event.py
--rw-rw-rw-   0        0        0    11980 2023-02-01 12:43:03.000000 o2despy-0.0.3/o2despy/hour_counter.py
--rw-rw-rw-   0        0        0    11129 2023-02-01 12:43:05.000000 o2despy-0.0.3/o2despy/sandbox.py
-drwxrwxrwx   0        0        0        0 2023-02-01 14:46:31.932667 o2despy-0.0.3/o2despy.egg-info/
--rw-rw-rw-   0        0        0      225 2023-02-01 14:46:31.000000 o2despy-0.0.3/o2despy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-02-01 14:46:31.000000 o2despy-0.0.3/o2despy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-01 14:46:31.000000 o2despy-0.0.3/o2despy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-02-01 14:46:31.000000 o2despy-0.0.3/o2despy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-01 14:46:31.961675 o2despy-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      297 2023-02-01 14:46:02.000000 o2despy-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-01 14:46:31.948668 o2despy-0.0.3/standard/
--rw-rw-rw-   0        0        0     3145 2023-02-01 12:44:43.000000 o2despy-0.0.3/standard/generator.py
--rw-rw-rw-   0        0        0     1599 2023-01-25 08:48:50.000000 o2despy-0.0.3/standard/load.py
--rw-rw-rw-   0        0        0     4052 2023-02-01 12:44:50.000000 o2despy-0.0.3/standard/queue.py
--rw-rw-rw-   0        0        0     6203 2023-02-01 13:05:08.000000 o2despy-0.0.3/standard/server.py
-drwxrwxrwx   0        0        0        0 2023-02-01 14:46:31.952676 o2despy-0.0.3/utils/
--rw-rw-rw-   0        0        0     3149 2023-01-25 08:48:50.000000 o2despy-0.0.3/utils/readonly.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:04:35.294366 o2despy-0.0.4/
+-rw-rw-rw-   0        0        0     1117 2023-01-31 09:11:19.000000 o2despy-0.0.4/License.txt
+-rw-rw-rw-   0        0        0      225 2023-07-22 09:04:35.294366 o2despy-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4947 2023-01-31 09:11:22.000000 o2despy-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 09:04:35.278843 o2despy-0.0.4/commons/
+-rw-rw-rw-   0        0        0     1985 2023-07-22 08:26:12.000000 o2despy-0.0.4/commons/duration_statistics_config.py
+-rw-rw-rw-   0        0        0     1057 2023-07-22 08:39:37.000000 o2despy-0.0.4/commons/file_config.py
+-rw-rw-rw-   0        0        0     1770 2023-07-22 08:26:12.000000 o2despy-0.0.4/commons/time_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:04:35.284930 o2despy-0.0.4/o2despy/
+-rw-rw-rw-   0        0        0     4515 2023-07-22 08:26:12.000000 o2despy-0.0.4/o2despy/action.py
+-rw-rw-rw-   0        0        0      230 2023-07-22 08:26:12.000000 o2despy-0.0.4/o2despy/assets.py
+-rw-rw-rw-   0        0        0     1227 2023-07-22 08:26:12.000000 o2despy-0.0.4/o2despy/entity.py
+-rw-rw-rw-   0        0        0     3131 2023-07-22 08:26:12.000000 o2despy-0.0.4/o2despy/event.py
+-rw-rw-rw-   0        0        0    17939 2023-07-22 08:39:12.000000 o2despy-0.0.4/o2despy/hour_counter.py
+-rw-rw-rw-   0        0        0    17350 2023-07-22 08:39:12.000000 o2despy-0.0.4/o2despy/sandbox.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:04:35.293366 o2despy-0.0.4/o2despy.egg-info/
+-rw-rw-rw-   0        0        0      225 2023-07-22 09:04:35.000000 o2despy-0.0.4/o2despy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-07-22 09:04:35.000000 o2despy-0.0.4/o2despy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 09:04:35.000000 o2despy-0.0.4/o2despy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-22 09:04:35.000000 o2despy-0.0.4/o2despy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-22 09:04:35.295367 o2despy-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      287 2023-07-22 09:04:32.000000 o2despy-0.0.4/setup.py
```

### Comparing `o2despy-0.0.3/License.txt` & `o2despy-0.0.4/License.txt`

 * *Files identical despite different names*

### Comparing `o2despy-0.0.3/README.md` & `o2despy-0.0.4/README.md`

 * *Files identical despite different names*

