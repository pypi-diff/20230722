# Comparing `tmp/lemonbar-0.6.1.tar.gz` & `tmp/lemonbar-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemonbar-0.6.1.tar", last modified: Sat Jul 22 14:06:34 2023, max compression
+gzip compressed data, was "lemonbar-0.6.2.tar", last modified: Sat Jul 22 14:27:23 2023, max compression
```

## Comparing `lemonbar-0.6.1.tar` & `lemonbar-0.6.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:06:34.099579 lemonbar-0.6.1/
--rw-r--r--   0 ori       (1000) ori       (1000)     1066 2023-07-22 12:38:48.000000 lemonbar-0.6.1/LICENSE
--rw-r--r--   0 ori       (1000) ori       (1000)      766 2023-07-22 14:06:34.099579 lemonbar-0.6.1/PKG-INFO
--rw-r--r--   0 ori       (1000) ori       (1000)     4834 2023-07-22 13:48:25.000000 lemonbar-0.6.1/README.md
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:06:34.099579 lemonbar-0.6.1/lemonbar/
--rw-r--r--   0 ori       (1000) ori       (1000)      129 2023-07-22 13:46:23.000000 lemonbar-0.6.1/lemonbar/__init__.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1166 2023-07-22 12:58:07.000000 lemonbar-0.6.1/lemonbar/async_utils.py
--rw-r--r--   0 ori       (1000) ori       (1000)     6187 2023-07-22 13:46:54.000000 lemonbar-0.6.1/lemonbar/lemonbar.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1934 2023-07-22 13:25:07.000000 lemonbar-0.6.1/lemonbar/module.py
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:06:34.099579 lemonbar-0.6.1/lemonbar.egg-info/
--rw-r--r--   0 ori       (1000) ori       (1000)      766 2023-07-22 14:06:34.000000 lemonbar-0.6.1/lemonbar.egg-info/PKG-INFO
--rw-r--r--   0 ori       (1000) ori       (1000)      280 2023-07-22 14:06:34.000000 lemonbar-0.6.1/lemonbar.egg-info/SOURCES.txt
--rw-r--r--   0 ori       (1000) ori       (1000)        1 2023-07-22 14:06:34.000000 lemonbar-0.6.1/lemonbar.egg-info/dependency_links.txt
--rw-r--r--   0 ori       (1000) ori       (1000)       20 2023-07-22 14:06:34.000000 lemonbar-0.6.1/lemonbar.egg-info/requires.txt
--rw-r--r--   0 ori       (1000) ori       (1000)        9 2023-07-22 14:06:34.000000 lemonbar-0.6.1/lemonbar.egg-info/top_level.txt
--rw-r--r--   0 ori       (1000) ori       (1000)       79 2023-07-22 14:06:34.099579 lemonbar-0.6.1/setup.cfg
--rw-r--r--   0 ori       (1000) ori       (1000)      946 2023-07-22 14:06:32.000000 lemonbar-0.6.1/setup.py
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:27:23.038441 lemonbar-0.6.2/
+-rw-r--r--   0 ori       (1000) ori       (1000)     1066 2023-07-22 12:38:48.000000 lemonbar-0.6.2/LICENSE
+-rw-r--r--   0 ori       (1000) ori       (1000)     5641 2023-07-22 14:27:23.038441 lemonbar-0.6.2/PKG-INFO
+-rw-r--r--   0 ori       (1000) ori       (1000)     4834 2023-07-22 13:48:25.000000 lemonbar-0.6.2/README.md
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:27:23.037441 lemonbar-0.6.2/lemonbar/
+-rw-r--r--   0 ori       (1000) ori       (1000)      129 2023-07-22 13:46:23.000000 lemonbar-0.6.2/lemonbar/__init__.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1166 2023-07-22 12:58:07.000000 lemonbar-0.6.2/lemonbar/async_utils.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     6187 2023-07-22 13:46:54.000000 lemonbar-0.6.2/lemonbar/lemonbar.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1934 2023-07-22 13:25:07.000000 lemonbar-0.6.2/lemonbar/module.py
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:27:23.038441 lemonbar-0.6.2/lemonbar.egg-info/
+-rw-r--r--   0 ori       (1000) ori       (1000)     5641 2023-07-22 14:27:23.000000 lemonbar-0.6.2/lemonbar.egg-info/PKG-INFO
+-rw-r--r--   0 ori       (1000) ori       (1000)      280 2023-07-22 14:27:23.000000 lemonbar-0.6.2/lemonbar.egg-info/SOURCES.txt
+-rw-r--r--   0 ori       (1000) ori       (1000)        1 2023-07-22 14:27:23.000000 lemonbar-0.6.2/lemonbar.egg-info/dependency_links.txt
+-rw-r--r--   0 ori       (1000) ori       (1000)       20 2023-07-22 14:27:23.000000 lemonbar-0.6.2/lemonbar.egg-info/requires.txt
+-rw-r--r--   0 ori       (1000) ori       (1000)        9 2023-07-22 14:27:23.000000 lemonbar-0.6.2/lemonbar.egg-info/top_level.txt
+-rw-r--r--   0 ori       (1000) ori       (1000)       79 2023-07-22 14:27:23.038441 lemonbar-0.6.2/setup.cfg
+-rw-r--r--   0 ori       (1000) ori       (1000)     1074 2023-07-22 14:27:21.000000 lemonbar-0.6.2/setup.py
```

### Comparing `lemonbar-0.6.1/LICENSE` & `lemonbar-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.1/README.md` & `lemonbar-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.1/lemonbar/async_utils.py` & `lemonbar-0.6.2/lemonbar/async_utils.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.1/lemonbar/lemonbar.py` & `lemonbar-0.6.2/lemonbar/lemonbar.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.1/lemonbar/module.py` & `lemonbar-0.6.2/lemonbar/module.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.1/setup.py` & `lemonbar-0.6.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from distutils.core import setup
+from pathlib import Path
 
 setup(
     name='lemonbar',
     packages=['lemonbar'],
-    version='0.6.1',
+    version='0.6.2',
     license='MIT',
     description='A Python API for interacting with Lemonbar',
+    long_description=Path("README.md").read_text(),
+    long_description_content_type="text/markdown",
     author='Ori Harel',
     author_email='oeharel@gmail.com',
     url='https://github.com/Heknon/lemonbar-api',
     download_url='https://github.com/Heknon/lemonbar-api/archive/refs/tags/v0.6.1.tar.gz',
     keywords=['lemonbar', 'api', 'lemonbar-api', "arch", "linux"],
     install_requires=[
         'pydantic',
```

