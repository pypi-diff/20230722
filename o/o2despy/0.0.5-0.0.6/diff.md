# Comparing `tmp/o2despy-0.0.5.tar.gz` & `tmp/o2despy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "o2despy-0.0.5.tar", last modified: Sat Jul 22 09:23:22 2023, max compression
+gzip compressed data, was "o2despy-0.0.6.tar", last modified: Sat Jul 22 09:33:00 2023, max compression
```

## Comparing `o2despy-0.0.5.tar` & `o2despy-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 09:23:22.006911 o2despy-0.0.5/
--rw-rw-rw-   0        0        0     1117 2023-01-31 09:11:19.000000 o2despy-0.0.5/License.txt
--rw-rw-rw-   0        0        0      225 2023-07-22 09:23:22.006911 o2despy-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4947 2023-01-31 09:11:22.000000 o2despy-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 09:23:21.983832 o2despy-0.0.5/commons/
--rw-rw-rw-   0        0        0     1985 2023-07-22 08:26:12.000000 o2despy-0.0.5/commons/duration_statistics_config.py
--rw-rw-rw-   0        0        0     1057 2023-07-22 08:39:37.000000 o2despy-0.0.5/commons/file_config.py
--rw-rw-rw-   0        0        0     1770 2023-07-22 08:26:12.000000 o2despy-0.0.5/commons/time_tools.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:23:21.989331 o2despy-0.0.5/o2despy/
--rw-rw-rw-   0        0        0     4515 2023-07-22 08:26:12.000000 o2despy-0.0.5/o2despy/action.py
--rw-rw-rw-   0        0        0      230 2023-07-22 08:26:12.000000 o2despy-0.0.5/o2despy/assets.py
--rw-rw-rw-   0        0        0     1227 2023-07-22 08:26:12.000000 o2despy-0.0.5/o2despy/entity.py
--rw-rw-rw-   0        0        0     3131 2023-07-22 08:26:12.000000 o2despy-0.0.5/o2despy/event.py
--rw-rw-rw-   0        0        0    17939 2023-07-22 08:39:12.000000 o2despy-0.0.5/o2despy/hour_counter.py
--rw-rw-rw-   0        0        0    17350 2023-07-22 08:39:12.000000 o2despy-0.0.5/o2despy/sandbox.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:23:22.005693 o2despy-0.0.5/o2despy.egg-info/
--rw-rw-rw-   0        0        0      225 2023-07-22 09:23:21.000000 o2despy-0.0.5/o2despy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-07-22 09:23:21.000000 o2despy-0.0.5/o2despy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 09:23:21.000000 o2despy-0.0.5/o2despy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-22 09:23:21.000000 o2despy-0.0.5/o2despy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-22 09:23:22.007912 o2despy-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      287 2023-07-22 09:23:06.000000 o2despy-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:33:00.368685 o2despy-0.0.6/
+-rw-rw-rw-   0        0        0     1117 2023-01-31 09:11:19.000000 o2despy-0.0.6/License.txt
+-rw-rw-rw-   0        0        0      225 2023-07-22 09:33:00.367680 o2despy-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4947 2023-01-31 09:11:22.000000 o2despy-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 09:33:00.352556 o2despy-0.0.6/commons/
+-rw-rw-rw-   0        0        0     1985 2023-07-22 08:26:12.000000 o2despy-0.0.6/commons/duration_statistics_config.py
+-rw-rw-rw-   0        0        0     1057 2023-07-22 08:39:37.000000 o2despy-0.0.6/commons/file_config.py
+-rw-rw-rw-   0        0        0     1770 2023-07-22 08:26:12.000000 o2despy-0.0.6/commons/time_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:33:00.358573 o2despy-0.0.6/o2despy/
+-rw-rw-rw-   0        0        0     4515 2023-07-22 08:26:12.000000 o2despy-0.0.6/o2despy/action.py
+-rw-rw-rw-   0        0        0      230 2023-07-22 08:26:12.000000 o2despy-0.0.6/o2despy/assets.py
+-rw-rw-rw-   0        0        0     1227 2023-07-22 08:26:12.000000 o2despy-0.0.6/o2despy/entity.py
+-rw-rw-rw-   0        0        0     3131 2023-07-22 08:26:12.000000 o2despy-0.0.6/o2despy/event.py
+-rw-rw-rw-   0        0        0    17939 2023-07-22 08:39:12.000000 o2despy-0.0.6/o2despy/hour_counter.py
+-rw-rw-rw-   0        0        0    17350 2023-07-22 08:39:12.000000 o2despy-0.0.6/o2despy/sandbox.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:33:00.366673 o2despy-0.0.6/o2despy.egg-info/
+-rw-rw-rw-   0        0        0      225 2023-07-22 09:33:00.000000 o2despy-0.0.6/o2despy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-07-22 09:33:00.000000 o2despy-0.0.6/o2despy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 09:33:00.000000 o2despy-0.0.6/o2despy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-22 09:33:00.000000 o2despy-0.0.6/o2despy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-22 09:33:00.368685 o2despy-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      287 2023-07-22 09:32:58.000000 o2despy-0.0.6/setup.py
```

### Comparing `o2despy-0.0.5/License.txt` & `o2despy-0.0.6/License.txt`

 * *Files identical despite different names*

### Comparing `o2despy-0.0.5/README.md` & `o2despy-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `o2despy-0.0.5/commons/duration_statistics_config.py` & `o2despy-0.0.6/commons/duration_statistics_config.py`

 * *Files identical despite different names*

### Comparing `o2despy-0.0.5/commons/file_config.py` & `o2despy-0.0.6/commons/file_config.py`

 * *Files identical despite different names*

### Comparing `o2despy-0.0.5/commons/time_tools.py` & `o2despy-0.0.6/commons/time_tools.py`

 * *Files identical despite different names*

### Comparing `o2despy-0.0.5/o2despy/action.py` & `o2despy-0.0.6/o2despy/action.py`

 * *Files identical despite different names*

### Comparing `o2despy-0.0.5/o2despy/entity.py` & `o2despy-0.0.6/o2despy/entity.py`

 * *Files identical despite different names*

### Comparing `o2despy-0.0.5/o2despy/event.py` & `o2despy-0.0.6/o2despy/event.py`

 * *Files identical despite different names*

### Comparing `o2despy-0.0.5/o2despy/hour_counter.py` & `o2despy-0.0.6/o2despy/hour_counter.py`

 * *Files identical despite different names*

### Comparing `o2despy-0.0.5/o2despy/sandbox.py` & `o2despy-0.0.6/o2despy/sandbox.py`

 * *Files identical despite different names*

