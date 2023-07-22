# Comparing `tmp/lemonbar-0.7.1.tar.gz` & `tmp/lemonbar-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemonbar-0.7.1.tar", last modified: Sat Jul 22 16:23:58 2023, max compression
+gzip compressed data, was "lemonbar-0.7.2.tar", last modified: Sat Jul 22 16:43:36 2023, max compression
```

## Comparing `lemonbar-0.7.1.tar` & `lemonbar-0.7.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 16:23:58.540671 lemonbar-0.7.1/
--rw-r--r--   0 ori       (1000) ori       (1000)     1066 2023-07-22 12:38:48.000000 lemonbar-0.7.1/LICENSE
--rw-r--r--   0 ori       (1000) ori       (1000)     5641 2023-07-22 16:23:58.540671 lemonbar-0.7.1/PKG-INFO
--rw-r--r--   0 ori       (1000) ori       (1000)     4834 2023-07-22 13:48:25.000000 lemonbar-0.7.1/README.md
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 16:23:58.538671 lemonbar-0.7.1/lemonbar/
--rw-r--r--   0 ori       (1000) ori       (1000)      187 2023-07-22 15:50:45.000000 lemonbar-0.7.1/lemonbar/__init__.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1166 2023-07-22 12:58:07.000000 lemonbar-0.7.1/lemonbar/async_utils.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1474 2023-07-22 15:56:32.000000 lemonbar-0.7.1/lemonbar/command_handler.py
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 16:23:58.539671 lemonbar-0.7.1/lemonbar/formatters/
--rw-r--r--   0 ori       (1000) ori       (1000)      110 2023-07-22 13:48:25.000000 lemonbar-0.7.1/lemonbar/formatters/__init__.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1078 2023-07-21 19:14:24.000000 lemonbar-0.7.1/lemonbar/formatters/_formatter.py
--rw-r--r--   0 ori       (1000) ori       (1000)      521 2023-07-22 13:36:40.000000 lemonbar-0.7.1/lemonbar/formatters/attributes.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1047 2023-07-22 13:36:40.000000 lemonbar-0.7.1/lemonbar/formatters/basic_formatters.py
--rw-r--r--   0 ori       (1000) ori       (1000)      369 2023-07-22 13:36:40.000000 lemonbar-0.7.1/lemonbar/formatters/button.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1324 2023-07-22 13:36:40.000000 lemonbar-0.7.1/lemonbar/formatters/change_monitor.py
--rw-r--r--   0 ori       (1000) ori       (1000)     6204 2023-07-22 16:21:52.000000 lemonbar-0.7.1/lemonbar/lemonbar.py
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 16:23:58.540671 lemonbar-0.7.1/lemonbar/models/
--rw-r--r--   0 ori       (1000) ori       (1000)      109 2023-07-22 13:38:31.000000 lemonbar-0.7.1/lemonbar/models/__init__.py
--rw-r--r--   0 ori       (1000) ori       (1000)      985 2023-07-22 13:48:25.000000 lemonbar-0.7.1/lemonbar/models/bar_geometry.py
--rw-r--r--   0 ori       (1000) ori       (1000)       99 2023-07-21 17:39:08.000000 lemonbar-0.7.1/lemonbar/models/bar_placement.py
--rw-r--r--   0 ori       (1000) ori       (1000)     3282 2023-07-22 13:39:01.000000 lemonbar-0.7.1/lemonbar/models/lemonbar_arguments.py
--rw-r--r--   0 ori       (1000) ori       (1000)      839 2023-07-22 14:53:04.000000 lemonbar-0.7.1/lemonbar/models/monitor.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1964 2023-07-22 15:16:48.000000 lemonbar-0.7.1/lemonbar/module.py
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 16:23:58.540671 lemonbar-0.7.1/lemonbar/modules/
--rw-r--r--   0 ori       (1000) ori       (1000)        0 2023-07-21 21:42:55.000000 lemonbar-0.7.1/lemonbar/modules/__init__.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1626 2023-07-22 15:56:32.000000 lemonbar-0.7.1/lemonbar/modules/clock.py
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 16:23:58.539671 lemonbar-0.7.1/lemonbar.egg-info/
--rw-r--r--   0 ori       (1000) ori       (1000)     5641 2023-07-22 16:23:58.000000 lemonbar-0.7.1/lemonbar.egg-info/PKG-INFO
--rw-r--r--   0 ori       (1000) ori       (1000)      729 2023-07-22 16:23:58.000000 lemonbar-0.7.1/lemonbar.egg-info/SOURCES.txt
--rw-r--r--   0 ori       (1000) ori       (1000)        1 2023-07-22 16:23:58.000000 lemonbar-0.7.1/lemonbar.egg-info/dependency_links.txt
--rw-r--r--   0 ori       (1000) ori       (1000)       41 2023-07-22 16:23:58.000000 lemonbar-0.7.1/lemonbar.egg-info/requires.txt
--rw-r--r--   0 ori       (1000) ori       (1000)        9 2023-07-22 16:23:58.000000 lemonbar-0.7.1/lemonbar.egg-info/top_level.txt
--rw-r--r--   0 ori       (1000) ori       (1000)       79 2023-07-22 16:23:58.541671 lemonbar-0.7.1/setup.cfg
--rw-r--r--   0 ori       (1000) ori       (1000)     1079 2023-07-22 16:22:35.000000 lemonbar-0.7.1/setup.py
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 16:43:36.927542 lemonbar-0.7.2/
+-rw-r--r--   0 ori       (1000) ori       (1000)     1066 2023-07-22 12:38:48.000000 lemonbar-0.7.2/LICENSE
+-rw-r--r--   0 ori       (1000) ori       (1000)     5641 2023-07-22 16:43:36.927542 lemonbar-0.7.2/PKG-INFO
+-rw-r--r--   0 ori       (1000) ori       (1000)     4834 2023-07-22 13:48:25.000000 lemonbar-0.7.2/README.md
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 16:43:36.925541 lemonbar-0.7.2/lemonbar/
+-rw-r--r--   0 ori       (1000) ori       (1000)      187 2023-07-22 15:50:45.000000 lemonbar-0.7.2/lemonbar/__init__.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1166 2023-07-22 12:58:07.000000 lemonbar-0.7.2/lemonbar/async_utils.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1474 2023-07-22 15:56:32.000000 lemonbar-0.7.2/lemonbar/command_handler.py
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 16:43:36.926542 lemonbar-0.7.2/lemonbar/formatters/
+-rw-r--r--   0 ori       (1000) ori       (1000)      110 2023-07-22 13:48:25.000000 lemonbar-0.7.2/lemonbar/formatters/__init__.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1078 2023-07-21 19:14:24.000000 lemonbar-0.7.2/lemonbar/formatters/_formatter.py
+-rw-r--r--   0 ori       (1000) ori       (1000)      521 2023-07-22 13:36:40.000000 lemonbar-0.7.2/lemonbar/formatters/attributes.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1119 2023-07-22 16:42:27.000000 lemonbar-0.7.2/lemonbar/formatters/basic_formatters.py
+-rw-r--r--   0 ori       (1000) ori       (1000)      369 2023-07-22 13:36:40.000000 lemonbar-0.7.2/lemonbar/formatters/button.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1324 2023-07-22 13:36:40.000000 lemonbar-0.7.2/lemonbar/formatters/change_monitor.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     6204 2023-07-22 16:21:52.000000 lemonbar-0.7.2/lemonbar/lemonbar.py
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 16:43:36.926542 lemonbar-0.7.2/lemonbar/models/
+-rw-r--r--   0 ori       (1000) ori       (1000)      109 2023-07-22 13:38:31.000000 lemonbar-0.7.2/lemonbar/models/__init__.py
+-rw-r--r--   0 ori       (1000) ori       (1000)      985 2023-07-22 13:48:25.000000 lemonbar-0.7.2/lemonbar/models/bar_geometry.py
+-rw-r--r--   0 ori       (1000) ori       (1000)       99 2023-07-21 17:39:08.000000 lemonbar-0.7.2/lemonbar/models/bar_placement.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     3282 2023-07-22 13:39:01.000000 lemonbar-0.7.2/lemonbar/models/lemonbar_arguments.py
+-rw-r--r--   0 ori       (1000) ori       (1000)      839 2023-07-22 14:53:04.000000 lemonbar-0.7.2/lemonbar/models/monitor.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1964 2023-07-22 15:16:48.000000 lemonbar-0.7.2/lemonbar/module.py
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 16:43:36.926542 lemonbar-0.7.2/lemonbar/modules/
+-rw-r--r--   0 ori       (1000) ori       (1000)        0 2023-07-21 21:42:55.000000 lemonbar-0.7.2/lemonbar/modules/__init__.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1626 2023-07-22 15:56:32.000000 lemonbar-0.7.2/lemonbar/modules/clock.py
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 16:43:36.925541 lemonbar-0.7.2/lemonbar.egg-info/
+-rw-r--r--   0 ori       (1000) ori       (1000)     5641 2023-07-22 16:43:36.000000 lemonbar-0.7.2/lemonbar.egg-info/PKG-INFO
+-rw-r--r--   0 ori       (1000) ori       (1000)      729 2023-07-22 16:43:36.000000 lemonbar-0.7.2/lemonbar.egg-info/SOURCES.txt
+-rw-r--r--   0 ori       (1000) ori       (1000)        1 2023-07-22 16:43:36.000000 lemonbar-0.7.2/lemonbar.egg-info/dependency_links.txt
+-rw-r--r--   0 ori       (1000) ori       (1000)       41 2023-07-22 16:43:36.000000 lemonbar-0.7.2/lemonbar.egg-info/requires.txt
+-rw-r--r--   0 ori       (1000) ori       (1000)        9 2023-07-22 16:43:36.000000 lemonbar-0.7.2/lemonbar.egg-info/top_level.txt
+-rw-r--r--   0 ori       (1000) ori       (1000)       79 2023-07-22 16:43:36.927542 lemonbar-0.7.2/setup.cfg
+-rw-r--r--   0 ori       (1000) ori       (1000)     1079 2023-07-22 16:42:57.000000 lemonbar-0.7.2/setup.py
```

### Comparing `lemonbar-0.7.1/LICENSE` & `lemonbar-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lemonbar-0.7.1/PKG-INFO` & `lemonbar-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lemonbar
-Version: 0.7.1
+Version: 0.7.2
 Summary: A Python API for interacting with Lemonbar
 Home-page: https://github.com/Heknon/lemonbar-api
-Download-URL: https://github.com/Heknon/lemonbar-api/archive/refs/tags/v0.7.1.tar.gz
+Download-URL: https://github.com/Heknon/lemonbar-api/archive/refs/tags/v0.7.2.tar.gz
 Author: Ori Harel
 Author-email: oeharel@gmail.com
 License: MIT
 Keywords: lemonbar,api,lemonbar-api,arch,linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `lemonbar-0.7.1/README.md` & `lemonbar-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `lemonbar-0.7.1/lemonbar/async_utils.py` & `lemonbar-0.7.2/lemonbar/async_utils.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.7.1/lemonbar/command_handler.py` & `lemonbar-0.7.2/lemonbar/command_handler.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.7.1/lemonbar/formatters/_formatter.py` & `lemonbar-0.7.2/lemonbar/formatters/_formatter.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.7.1/lemonbar/formatters/attributes.py` & `lemonbar-0.7.2/lemonbar/formatters/attributes.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.7.1/lemonbar/formatters/basic_formatters.py` & `lemonbar-0.7.2/lemonbar/formatters/basic_formatters.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 
 
 @make_formatter('R')
 def swap_background_and_foreground(message: str) -> str:
     return message
 
 
-@make_formatter('l')
 def align_left(message: str) -> str:
-    return message
+    return "%{l}" + message + "%{l}"
+
+
+def align_center(message: str) -> str:
+    return "%{c}" + message + "%{l}"
 
 
-@make_formatter('r')
 def align_right(message: str) -> str:
-    return message
+    return "%{r}" + message + "%{l}"
 
 
 def offset_x(pixels: int, message: str) -> str:
     return lemon_formatting(message, 'O', str(pixels))
 
 
 def background_color(color: Color, message: str) -> str:
```

### Comparing `lemonbar-0.7.1/lemonbar/formatters/change_monitor.py` & `lemonbar-0.7.2/lemonbar/formatters/change_monitor.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.7.1/lemonbar/lemonbar.py` & `lemonbar-0.7.2/lemonbar/lemonbar.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.7.1/lemonbar/models/bar_geometry.py` & `lemonbar-0.7.2/lemonbar/models/bar_geometry.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.7.1/lemonbar/models/lemonbar_arguments.py` & `lemonbar-0.7.2/lemonbar/models/lemonbar_arguments.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.7.1/lemonbar/models/monitor.py` & `lemonbar-0.7.2/lemonbar/models/monitor.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.7.1/lemonbar/module.py` & `lemonbar-0.7.2/lemonbar/module.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.7.1/lemonbar/modules/clock.py` & `lemonbar-0.7.2/lemonbar/modules/clock.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.7.1/lemonbar.egg-info/PKG-INFO` & `lemonbar-0.7.2/lemonbar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lemonbar
-Version: 0.7.1
+Version: 0.7.2
 Summary: A Python API for interacting with Lemonbar
 Home-page: https://github.com/Heknon/lemonbar-api
-Download-URL: https://github.com/Heknon/lemonbar-api/archive/refs/tags/v0.7.1.tar.gz
+Download-URL: https://github.com/Heknon/lemonbar-api/archive/refs/tags/v0.7.2.tar.gz
 Author: Ori Harel
 Author-email: oeharel@gmail.com
 License: MIT
 Keywords: lemonbar,api,lemonbar-api,arch,linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `lemonbar-0.7.1/lemonbar.egg-info/SOURCES.txt` & `lemonbar-0.7.2/lemonbar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lemonbar-0.7.1/setup.py` & `lemonbar-0.7.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from distutils.core import setup
 from pathlib import Path
 
 setup(
     name='lemonbar',
-    version='0.7.1',
+    version='0.7.2',
     license='MIT',
     description='A Python API for interacting with Lemonbar',
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     author='Ori Harel',
     author_email='oeharel@gmail.com',
     url='https://github.com/Heknon/lemonbar-api',
-    download_url='https://github.com/Heknon/lemonbar-api/archive/refs/tags/v0.7.1.tar.gz',
+    download_url='https://github.com/Heknon/lemonbar-api/archive/refs/tags/v0.7.2.tar.gz',
     keywords=['lemonbar', 'api', 'lemonbar-api', "arch", "linux"],
     install_requires=[
         'pydantic',
         'screeninfo',
         'pydantic_extra_types',
     ],
     classifiers=[
```

