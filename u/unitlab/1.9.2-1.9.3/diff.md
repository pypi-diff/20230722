# Comparing `tmp/unitlab-1.9.2.tar.gz` & `tmp/unitlab-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitlab-1.9.2.tar", last modified: Tue Jun 20 09:38:54 2023, max compression
+gzip compressed data, was "unitlab-1.9.3.tar", last modified: Sat Jul 22 07:59:06 2023, max compression
```

## Comparing `unitlab-1.9.2.tar` & `unitlab-1.9.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-20 09:38:54.479501 unitlab-1.9.2/
--rw-rw-r--   0 me        (1000) me        (1000)     1060 2022-11-07 13:04:44.000000 unitlab-1.9.2/LICENSE.md
--rw-rw-r--   0 me        (1000) me        (1000)       84 2023-02-15 09:26:00.000000 unitlab-1.9.2/MANIFEST.in
--rw-rw-r--   0 me        (1000) me        (1000)      654 2023-06-20 09:38:54.479501 unitlab-1.9.2/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)     1431 2023-06-13 08:13:23.000000 unitlab-1.9.2/README.md
--rw-rw-r--   0 me        (1000) me        (1000)      106 2023-06-20 09:38:54.479501 unitlab-1.9.2/setup.cfg
--rw-rw-r--   0 me        (1000) me        (1000)     1108 2023-06-20 09:38:32.000000 unitlab-1.9.2/setup.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-20 09:38:54.475513 unitlab-1.9.2/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-20 09:38:54.475513 unitlab-1.9.2/src/unitlab/
--rw-rw-r--   0 me        (1000) me        (1000)      214 2023-05-23 13:05:07.000000 unitlab-1.9.2/src/unitlab/__init__.py
--rw-rw-r--   0 me        (1000) me        (1000)     1631 2023-06-15 09:37:56.000000 unitlab-1.9.2/src/unitlab/cli.py
--rw-rw-r--   0 me        (1000) me        (1000)    11359 2023-06-20 09:34:47.000000 unitlab-1.9.2/src/unitlab/client.py
--rw-rw-r--   0 me        (1000) me        (1000)      656 2023-06-13 10:04:19.000000 unitlab-1.9.2/src/unitlab/exceptions.py
--rw-rw-r--   0 me        (1000) me        (1000)     1813 2023-06-20 09:36:47.000000 unitlab-1.9.2/src/unitlab/run.py
--rw-rw-r--   0 me        (1000) me        (1000)     1933 2023-06-15 09:38:00.000000 unitlab-1.9.2/src/unitlab/utils.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-20 09:38:54.479501 unitlab-1.9.2/src/unitlab.egg-info/
--rw-rw-r--   0 me        (1000) me        (1000)      654 2023-06-20 09:38:54.000000 unitlab-1.9.2/src/unitlab.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      394 2023-06-20 09:38:54.000000 unitlab-1.9.2/src/unitlab.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2023-06-20 09:38:54.000000 unitlab-1.9.2/src/unitlab.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)       44 2023-06-20 09:38:54.000000 unitlab-1.9.2/src/unitlab.egg-info/entry_points.txt
--rw-rw-r--   0 me        (1000) me        (1000)       55 2023-06-20 09:38:54.000000 unitlab-1.9.2/src/unitlab.egg-info/requires.txt
--rw-rw-r--   0 me        (1000) me        (1000)        8 2023-06-20 09:38:54.000000 unitlab-1.9.2/src/unitlab.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-07-22 07:59:06.137505 unitlab-1.9.3/
+-rw-rw-r--   0 me        (1000) me        (1000)     1060 2022-11-07 13:04:44.000000 unitlab-1.9.3/LICENSE.md
+-rw-rw-r--   0 me        (1000) me        (1000)       84 2023-02-15 09:26:00.000000 unitlab-1.9.3/MANIFEST.in
+-rw-rw-r--   0 me        (1000) me        (1000)      654 2023-07-22 07:59:06.137505 unitlab-1.9.3/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)     1431 2023-06-13 08:13:23.000000 unitlab-1.9.3/README.md
+-rw-rw-r--   0 me        (1000) me        (1000)      106 2023-07-22 07:59:06.137505 unitlab-1.9.3/setup.cfg
+-rw-rw-r--   0 me        (1000) me        (1000)     1108 2023-07-22 07:58:54.000000 unitlab-1.9.3/setup.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-07-22 07:59:06.133505 unitlab-1.9.3/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-07-22 07:59:06.137505 unitlab-1.9.3/src/unitlab/
+-rw-rw-r--   0 me        (1000) me        (1000)      214 2023-05-23 13:05:07.000000 unitlab-1.9.3/src/unitlab/__init__.py
+-rw-rw-r--   0 me        (1000) me        (1000)     1631 2023-06-15 09:37:56.000000 unitlab-1.9.3/src/unitlab/cli.py
+-rw-rw-r--   0 me        (1000) me        (1000)    11370 2023-07-22 07:58:10.000000 unitlab-1.9.3/src/unitlab/client.py
+-rw-rw-r--   0 me        (1000) me        (1000)      656 2023-06-13 10:04:19.000000 unitlab-1.9.3/src/unitlab/exceptions.py
+-rw-rw-r--   0 me        (1000) me        (1000)     1813 2023-06-27 06:41:01.000000 unitlab-1.9.3/src/unitlab/run.py
+-rw-rw-r--   0 me        (1000) me        (1000)     1933 2023-07-22 07:56:31.000000 unitlab-1.9.3/src/unitlab/utils.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-07-22 07:59:06.137505 unitlab-1.9.3/src/unitlab.egg-info/
+-rw-rw-r--   0 me        (1000) me        (1000)      654 2023-07-22 07:59:06.000000 unitlab-1.9.3/src/unitlab.egg-info/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)      394 2023-07-22 07:59:06.000000 unitlab-1.9.3/src/unitlab.egg-info/SOURCES.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        1 2023-07-22 07:59:06.000000 unitlab-1.9.3/src/unitlab.egg-info/dependency_links.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       44 2023-07-22 07:59:06.000000 unitlab-1.9.3/src/unitlab.egg-info/entry_points.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       55 2023-07-22 07:59:06.000000 unitlab-1.9.3/src/unitlab.egg-info/requires.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        8 2023-07-22 07:59:06.000000 unitlab-1.9.3/src/unitlab.egg-info/top_level.txt
```

### Comparing `unitlab-1.9.2/LICENSE.md` & `unitlab-1.9.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unitlab-1.9.2/PKG-INFO` & `unitlab-1.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 1.9.2
+Version: 1.9.3
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `unitlab-1.9.2/README.md` & `unitlab-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `unitlab-1.9.2/setup.py` & `unitlab-1.9.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="unitlab",
-    version="1.9.2",
+    version="1.9.3",
     license="MIT",
     author="Unitlab Inc.",
     author_email="team@unitlab.ai",
     packages=find_packages("src"),
     include_package_data=True,
     package_data={"static": ["*"], "Potato": ["*.so"]},
     classifiers=[
```

### Comparing `unitlab-1.9.2/src/unitlab/cli.py` & `unitlab-1.9.3/src/unitlab/cli.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.9.2/src/unitlab/client.py` & `unitlab-1.9.3/src/unitlab/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         if not os.path.isdir(directory):
             raise ValueError(f"Directory {directory} does not exist")
 
         # set correct host
         send_request(
             {
                 "method": "GET",
-                "endpoint": "check",
+                "endpoint": ENDPOINTS["check"],
                 "headers": self._get_headers(),
             },
             session=self.api_session,
         )
         URL = os.environ["UNITLAB_BASE_URL"] + ENDPOINTS["upload_data"]
 
         async def post_image(session: aiohttp.ClientSession, image: str, task_id: str):
```

### Comparing `unitlab-1.9.2/src/unitlab/exceptions.py` & `unitlab-1.9.3/src/unitlab/exceptions.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.9.2/src/unitlab/run.py` & `unitlab-1.9.3/src/unitlab/run.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.9.2/src/unitlab/utils.py` & `unitlab-1.9.3/src/unitlab/utils.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.9.2/src/unitlab.egg-info/PKG-INFO` & `unitlab-1.9.3/src/unitlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 1.9.2
+Version: 1.9.3
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

