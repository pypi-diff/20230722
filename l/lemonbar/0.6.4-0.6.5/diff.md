# Comparing `tmp/lemonbar-0.6.4.tar.gz` & `tmp/lemonbar-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemonbar-0.6.4.tar", last modified: Sat Jul 22 14:37:43 2023, max compression
+gzip compressed data, was "lemonbar-0.6.5.tar", last modified: Sat Jul 22 14:42:53 2023, max compression
```

## Comparing `lemonbar-0.6.4.tar` & `lemonbar-0.6.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:37:43.863373 lemonbar-0.6.4/
--rw-r--r--   0 ori       (1000) ori       (1000)     1066 2023-07-22 12:38:48.000000 lemonbar-0.6.4/LICENSE
--rw-r--r--   0 ori       (1000) ori       (1000)     5641 2023-07-22 14:37:43.863373 lemonbar-0.6.4/PKG-INFO
--rw-r--r--   0 ori       (1000) ori       (1000)     4834 2023-07-22 13:48:25.000000 lemonbar-0.6.4/README.md
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:37:43.862373 lemonbar-0.6.4/lemonbar/
--rw-r--r--   0 ori       (1000) ori       (1000)      129 2023-07-22 13:46:23.000000 lemonbar-0.6.4/lemonbar/__init__.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1166 2023-07-22 12:58:07.000000 lemonbar-0.6.4/lemonbar/async_utils.py
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:37:43.862373 lemonbar-0.6.4/lemonbar/formatters/
--rw-r--r--   0 ori       (1000) ori       (1000)      110 2023-07-22 13:48:25.000000 lemonbar-0.6.4/lemonbar/formatters/__init__.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1078 2023-07-21 19:14:24.000000 lemonbar-0.6.4/lemonbar/formatters/_formatter.py
--rw-r--r--   0 ori       (1000) ori       (1000)      521 2023-07-22 13:36:40.000000 lemonbar-0.6.4/lemonbar/formatters/attributes.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1047 2023-07-22 13:36:40.000000 lemonbar-0.6.4/lemonbar/formatters/basic_formatters.py
--rw-r--r--   0 ori       (1000) ori       (1000)      369 2023-07-22 13:36:40.000000 lemonbar-0.6.4/lemonbar/formatters/button.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1324 2023-07-22 13:36:40.000000 lemonbar-0.6.4/lemonbar/formatters/change_monitor.py
--rw-r--r--   0 ori       (1000) ori       (1000)     6187 2023-07-22 13:46:54.000000 lemonbar-0.6.4/lemonbar/lemonbar.py
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:37:43.863373 lemonbar-0.6.4/lemonbar/models/
--rw-r--r--   0 ori       (1000) ori       (1000)      109 2023-07-22 13:38:31.000000 lemonbar-0.6.4/lemonbar/models/__init__.py
--rw-r--r--   0 ori       (1000) ori       (1000)      985 2023-07-22 13:48:25.000000 lemonbar-0.6.4/lemonbar/models/bar_geometry.py
--rw-r--r--   0 ori       (1000) ori       (1000)       99 2023-07-21 17:39:08.000000 lemonbar-0.6.4/lemonbar/models/bar_placement.py
--rw-r--r--   0 ori       (1000) ori       (1000)     3282 2023-07-22 13:39:01.000000 lemonbar-0.6.4/lemonbar/models/lemonbar_arguments.py
--rw-r--r--   0 ori       (1000) ori       (1000)      818 2023-07-22 13:36:40.000000 lemonbar-0.6.4/lemonbar/models/monitor.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1934 2023-07-22 13:25:07.000000 lemonbar-0.6.4/lemonbar/module.py
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:37:43.863373 lemonbar-0.6.4/lemonbar/modules/
--rw-r--r--   0 ori       (1000) ori       (1000)        0 2023-07-21 21:42:55.000000 lemonbar-0.6.4/lemonbar/modules/__init__.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1692 2023-07-22 13:45:37.000000 lemonbar-0.6.4/lemonbar/modules/clock.py
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:37:43.862373 lemonbar-0.6.4/lemonbar.egg-info/
--rw-r--r--   0 ori       (1000) ori       (1000)     5641 2023-07-22 14:37:43.000000 lemonbar-0.6.4/lemonbar.egg-info/PKG-INFO
--rw-r--r--   0 ori       (1000) ori       (1000)      701 2023-07-22 14:37:43.000000 lemonbar-0.6.4/lemonbar.egg-info/SOURCES.txt
--rw-r--r--   0 ori       (1000) ori       (1000)        1 2023-07-22 14:37:43.000000 lemonbar-0.6.4/lemonbar.egg-info/dependency_links.txt
--rw-r--r--   0 ori       (1000) ori       (1000)       20 2023-07-22 14:37:43.000000 lemonbar-0.6.4/lemonbar.egg-info/requires.txt
--rw-r--r--   0 ori       (1000) ori       (1000)        9 2023-07-22 14:37:43.000000 lemonbar-0.6.4/lemonbar.egg-info/top_level.txt
--rw-r--r--   0 ori       (1000) ori       (1000)       79 2023-07-22 14:37:43.863373 lemonbar-0.6.4/setup.cfg
--rw-r--r--   0 ori       (1000) ori       (1000)     1047 2023-07-22 14:37:41.000000 lemonbar-0.6.4/setup.py
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:42:53.988339 lemonbar-0.6.5/
+-rw-r--r--   0 ori       (1000) ori       (1000)     1066 2023-07-22 12:38:48.000000 lemonbar-0.6.5/LICENSE
+-rw-r--r--   0 ori       (1000) ori       (1000)     5641 2023-07-22 14:42:53.988339 lemonbar-0.6.5/PKG-INFO
+-rw-r--r--   0 ori       (1000) ori       (1000)     4834 2023-07-22 13:48:25.000000 lemonbar-0.6.5/README.md
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:42:53.986339 lemonbar-0.6.5/lemonbar/
+-rw-r--r--   0 ori       (1000) ori       (1000)      129 2023-07-22 13:46:23.000000 lemonbar-0.6.5/lemonbar/__init__.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1166 2023-07-22 12:58:07.000000 lemonbar-0.6.5/lemonbar/async_utils.py
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:42:53.987339 lemonbar-0.6.5/lemonbar/formatters/
+-rw-r--r--   0 ori       (1000) ori       (1000)      110 2023-07-22 13:48:25.000000 lemonbar-0.6.5/lemonbar/formatters/__init__.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1078 2023-07-21 19:14:24.000000 lemonbar-0.6.5/lemonbar/formatters/_formatter.py
+-rw-r--r--   0 ori       (1000) ori       (1000)      521 2023-07-22 13:36:40.000000 lemonbar-0.6.5/lemonbar/formatters/attributes.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1047 2023-07-22 13:36:40.000000 lemonbar-0.6.5/lemonbar/formatters/basic_formatters.py
+-rw-r--r--   0 ori       (1000) ori       (1000)      369 2023-07-22 13:36:40.000000 lemonbar-0.6.5/lemonbar/formatters/button.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1324 2023-07-22 13:36:40.000000 lemonbar-0.6.5/lemonbar/formatters/change_monitor.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     6187 2023-07-22 13:46:54.000000 lemonbar-0.6.5/lemonbar/lemonbar.py
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:42:53.987339 lemonbar-0.6.5/lemonbar/models/
+-rw-r--r--   0 ori       (1000) ori       (1000)      109 2023-07-22 13:38:31.000000 lemonbar-0.6.5/lemonbar/models/__init__.py
+-rw-r--r--   0 ori       (1000) ori       (1000)      985 2023-07-22 13:48:25.000000 lemonbar-0.6.5/lemonbar/models/bar_geometry.py
+-rw-r--r--   0 ori       (1000) ori       (1000)       99 2023-07-21 17:39:08.000000 lemonbar-0.6.5/lemonbar/models/bar_placement.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     3282 2023-07-22 13:39:01.000000 lemonbar-0.6.5/lemonbar/models/lemonbar_arguments.py
+-rw-r--r--   0 ori       (1000) ori       (1000)      818 2023-07-22 13:36:40.000000 lemonbar-0.6.5/lemonbar/models/monitor.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1934 2023-07-22 13:25:07.000000 lemonbar-0.6.5/lemonbar/module.py
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:42:53.988339 lemonbar-0.6.5/lemonbar/modules/
+-rw-r--r--   0 ori       (1000) ori       (1000)        0 2023-07-21 21:42:55.000000 lemonbar-0.6.5/lemonbar/modules/__init__.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1692 2023-07-22 13:45:37.000000 lemonbar-0.6.5/lemonbar/modules/clock.py
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:42:53.987339 lemonbar-0.6.5/lemonbar.egg-info/
+-rw-r--r--   0 ori       (1000) ori       (1000)     5641 2023-07-22 14:42:53.000000 lemonbar-0.6.5/lemonbar.egg-info/PKG-INFO
+-rw-r--r--   0 ori       (1000) ori       (1000)      701 2023-07-22 14:42:53.000000 lemonbar-0.6.5/lemonbar.egg-info/SOURCES.txt
+-rw-r--r--   0 ori       (1000) ori       (1000)        1 2023-07-22 14:42:53.000000 lemonbar-0.6.5/lemonbar.egg-info/dependency_links.txt
+-rw-r--r--   0 ori       (1000) ori       (1000)       41 2023-07-22 14:42:53.000000 lemonbar-0.6.5/lemonbar.egg-info/requires.txt
+-rw-r--r--   0 ori       (1000) ori       (1000)        9 2023-07-22 14:42:53.000000 lemonbar-0.6.5/lemonbar.egg-info/top_level.txt
+-rw-r--r--   0 ori       (1000) ori       (1000)       79 2023-07-22 14:42:53.988339 lemonbar-0.6.5/setup.cfg
+-rw-r--r--   0 ori       (1000) ori       (1000)     1079 2023-07-22 14:41:31.000000 lemonbar-0.6.5/setup.py
```

### Comparing `lemonbar-0.6.4/LICENSE` & `lemonbar-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.4/PKG-INFO` & `lemonbar-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lemonbar
-Version: 0.6.4
+Version: 0.6.5
 Summary: A Python API for interacting with Lemonbar
 Home-page: https://github.com/Heknon/lemonbar-api
-Download-URL: https://github.com/Heknon/lemonbar-api/archive/refs/tags/v0.6.1.tar.gz
+Download-URL: https://github.com/Heknon/lemonbar-api/archive/refs/tags/v0.6.5.tar.gz
 Author: Ori Harel
 Author-email: oeharel@gmail.com
 License: MIT
 Keywords: lemonbar,api,lemonbar-api,arch,linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `lemonbar-0.6.4/README.md` & `lemonbar-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.4/lemonbar/async_utils.py` & `lemonbar-0.6.5/lemonbar/async_utils.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.4/lemonbar/formatters/_formatter.py` & `lemonbar-0.6.5/lemonbar/formatters/_formatter.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.4/lemonbar/formatters/attributes.py` & `lemonbar-0.6.5/lemonbar/formatters/attributes.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.4/lemonbar/formatters/basic_formatters.py` & `lemonbar-0.6.5/lemonbar/formatters/basic_formatters.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.4/lemonbar/formatters/change_monitor.py` & `lemonbar-0.6.5/lemonbar/formatters/change_monitor.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.4/lemonbar/lemonbar.py` & `lemonbar-0.6.5/lemonbar/lemonbar.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.4/lemonbar/models/bar_geometry.py` & `lemonbar-0.6.5/lemonbar/models/bar_geometry.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.4/lemonbar/models/lemonbar_arguments.py` & `lemonbar-0.6.5/lemonbar/models/lemonbar_arguments.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.4/lemonbar/models/monitor.py` & `lemonbar-0.6.5/lemonbar/models/monitor.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.4/lemonbar/module.py` & `lemonbar-0.6.5/lemonbar/module.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.4/lemonbar/modules/clock.py` & `lemonbar-0.6.5/lemonbar/modules/clock.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.4/lemonbar.egg-info/PKG-INFO` & `lemonbar-0.6.5/lemonbar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lemonbar
-Version: 0.6.4
+Version: 0.6.5
 Summary: A Python API for interacting with Lemonbar
 Home-page: https://github.com/Heknon/lemonbar-api
-Download-URL: https://github.com/Heknon/lemonbar-api/archive/refs/tags/v0.6.1.tar.gz
+Download-URL: https://github.com/Heknon/lemonbar-api/archive/refs/tags/v0.6.5.tar.gz
 Author: Ori Harel
 Author-email: oeharel@gmail.com
 License: MIT
 Keywords: lemonbar,api,lemonbar-api,arch,linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `lemonbar-0.6.4/lemonbar.egg-info/SOURCES.txt` & `lemonbar-0.6.5/lemonbar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.4/setup.py` & `lemonbar-0.6.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from distutils.core import setup
 from pathlib import Path
 
 setup(
     name='lemonbar',
-    version='0.6.4',
+    version='0.6.5',
     license='MIT',
     description='A Python API for interacting with Lemonbar',
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     author='Ori Harel',
     author_email='oeharel@gmail.com',
     url='https://github.com/Heknon/lemonbar-api',
-    download_url='https://github.com/Heknon/lemonbar-api/archive/refs/tags/v0.6.1.tar.gz',
+    download_url='https://github.com/Heknon/lemonbar-api/archive/refs/tags/v0.6.5.tar.gz',
     keywords=['lemonbar', 'api', 'lemonbar-api', "arch", "linux"],
     install_requires=[
         'pydantic',
         'screeninfo',
+        'pydantic_extra_types',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

