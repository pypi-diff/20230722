# Comparing `tmp/sightvision-0.1.tar.gz` & `tmp/sightvision-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sightvision-0.1.tar", last modified: Sat Jul 22 02:34:07 2023, max compression
+gzip compressed data, was "sightvision-0.1.3.tar", last modified: Sat Jul 22 15:31:25 2023, max compression
```

## Comparing `sightvision-0.1.tar` & `sightvision-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dragon    (1000) dragon    (1000)        0 2023-07-22 02:34:07.880635 sightvision-0.1/
--rw-r--r--   0 dragon    (1000) dragon    (1000)     1065 2023-07-21 19:53:53.000000 sightvision-0.1/LICENSE.txt
--rw-r--r--   0 dragon    (1000) dragon    (1000)      988 2023-07-22 02:34:07.880635 sightvision-0.1/PKG-INFO
--rw-r--r--   0 dragon    (1000) dragon    (1000)       12 2023-07-21 23:49:15.000000 sightvision-0.1/README.md
--rw-r--r--   0 dragon    (1000) dragon    (1000)       79 2023-07-22 02:34:07.883968 sightvision-0.1/setup.cfg
--rw-r--r--   0 dragon    (1000) dragon    (1000)     1893 2023-07-22 02:33:47.000000 sightvision-0.1/setup.py
-drwxr-xr-x   0 dragon    (1000) dragon    (1000)        0 2023-07-22 02:34:07.877302 sightvision-0.1/sightvision/
--rw-r--r--   0 dragon    (1000) dragon    (1000)     2265 2023-07-22 02:25:31.000000 sightvision-0.1/sightvision/ClassificationModule.py.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     3756 2023-07-22 02:24:49.000000 sightvision-0.1/sightvision/ColorModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     1558 2023-07-21 23:34:40.000000 sightvision-0.1/sightvision/FPS.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     2361 2023-07-22 02:20:18.000000 sightvision-0.1/sightvision/FaceDetectionModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     3607 2023-07-21 23:32:34.000000 sightvision-0.1/sightvision/FaceMeshModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     7350 2023-07-22 02:19:49.000000 sightvision-0.1/sightvision/HandTrackingModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     2230 2023-07-22 02:23:11.000000 sightvision-0.1/sightvision/PIDModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     3423 2023-07-22 02:22:52.000000 sightvision-0.1/sightvision/PlotModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     5536 2023-07-22 02:22:27.000000 sightvision-0.1/sightvision/PoseModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     1670 2023-07-22 02:21:53.000000 sightvision-0.1/sightvision/SelfiSegmentationModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     2213 2023-07-22 02:21:28.000000 sightvision-0.1/sightvision/SerialModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     6541 2023-07-22 02:20:48.000000 sightvision-0.1/sightvision/Utils.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)      272 2023-07-22 02:16:51.000000 sightvision-0.1/sightvision/__init__.py
-drwxr-xr-x   0 dragon    (1000) dragon    (1000)        0 2023-07-22 02:34:07.880635 sightvision-0.1/sightvision.egg-info/
--rw-r--r--   0 dragon    (1000) dragon    (1000)      988 2023-07-22 02:34:07.000000 sightvision-0.1/sightvision.egg-info/PKG-INFO
--rw-r--r--   0 dragon    (1000) dragon    (1000)      587 2023-07-22 02:34:07.000000 sightvision-0.1/sightvision.egg-info/SOURCES.txt
--rw-r--r--   0 dragon    (1000) dragon    (1000)        1 2023-07-22 02:34:07.000000 sightvision-0.1/sightvision.egg-info/dependency_links.txt
--rw-r--r--   0 dragon    (1000) dragon    (1000)       24 2023-07-22 02:34:07.000000 sightvision-0.1/sightvision.egg-info/requires.txt
--rw-r--r--   0 dragon    (1000) dragon    (1000)       12 2023-07-22 02:34:07.000000 sightvision-0.1/sightvision.egg-info/top_level.txt
+drwxr-xr-x   0 dragon    (1000) dragon    (1000)        0 2023-07-22 15:31:25.723381 sightvision-0.1.3/
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     1065 2023-07-21 19:53:53.000000 sightvision-0.1.3/LICENSE.txt
+-rw-r--r--   0 dragon    (1000) dragon    (1000)      990 2023-07-22 15:31:25.723381 sightvision-0.1.3/PKG-INFO
+-rw-r--r--   0 dragon    (1000) dragon    (1000)      987 2023-07-22 15:23:42.000000 sightvision-0.1.3/README.md
+-rw-r--r--   0 dragon    (1000) dragon    (1000)       79 2023-07-22 15:31:25.723381 sightvision-0.1.3/setup.cfg
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     1895 2023-07-22 15:29:13.000000 sightvision-0.1.3/setup.py
+drwxr-xr-x   0 dragon    (1000) dragon    (1000)        0 2023-07-22 15:31:25.720047 sightvision-0.1.3/sightvision/
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     2265 2023-07-22 02:25:31.000000 sightvision-0.1.3/sightvision/ClassificationModule.py.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     3756 2023-07-22 02:24:49.000000 sightvision-0.1.3/sightvision/ColorModule.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     1558 2023-07-21 23:34:40.000000 sightvision-0.1.3/sightvision/FPS.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     2361 2023-07-22 02:20:18.000000 sightvision-0.1.3/sightvision/FaceDetectionModule.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     3607 2023-07-21 23:32:34.000000 sightvision-0.1.3/sightvision/FaceMeshModule.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     7350 2023-07-22 02:19:49.000000 sightvision-0.1.3/sightvision/HandTrackingModule.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     2230 2023-07-22 02:23:11.000000 sightvision-0.1.3/sightvision/PIDModule.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     3423 2023-07-22 02:22:52.000000 sightvision-0.1.3/sightvision/PlotModule.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     5536 2023-07-22 02:22:27.000000 sightvision-0.1.3/sightvision/PoseModule.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     1670 2023-07-22 02:21:53.000000 sightvision-0.1.3/sightvision/SelfiSegmentationModule.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     2213 2023-07-22 02:21:28.000000 sightvision-0.1.3/sightvision/SerialModule.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     6541 2023-07-22 02:20:48.000000 sightvision-0.1.3/sightvision/Utils.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)      272 2023-07-22 15:24:14.000000 sightvision-0.1.3/sightvision/__init__.py
+drwxr-xr-x   0 dragon    (1000) dragon    (1000)        0 2023-07-22 15:31:25.723381 sightvision-0.1.3/sightvision.egg-info/
+-rw-r--r--   0 dragon    (1000) dragon    (1000)      990 2023-07-22 15:31:25.000000 sightvision-0.1.3/sightvision.egg-info/PKG-INFO
+-rw-r--r--   0 dragon    (1000) dragon    (1000)      587 2023-07-22 15:31:25.000000 sightvision-0.1.3/sightvision.egg-info/SOURCES.txt
+-rw-r--r--   0 dragon    (1000) dragon    (1000)        1 2023-07-22 15:31:25.000000 sightvision-0.1.3/sightvision.egg-info/dependency_links.txt
+-rw-r--r--   0 dragon    (1000) dragon    (1000)       24 2023-07-22 15:31:25.000000 sightvision-0.1.3/sightvision.egg-info/requires.txt
+-rw-r--r--   0 dragon    (1000) dragon    (1000)       12 2023-07-22 15:31:25.000000 sightvision-0.1.3/sightvision.egg-info/top_level.txt
```

### Comparing `sightvision-0.1/LICENSE.txt` & `sightvision-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sightvision-0.1/PKG-INFO` & `sightvision-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sightvision
-Version: 0.1
+Version: 0.1.3
 Summary: This is a Computer vision package that makes its easy to run Image processing and AI functions.
 Home-page: https://github.com/rexionmars/SightVision
 Download-URL: https://github.com/rexionmars/SightVision/archive/v_01.tar.gz
 Author: Leonardi Melo
 Author-email: opensource.leonardi@gmail.com
 License: MIT
 Keywords: Computervision,Imageutils,Imageprocessing
```

### Comparing `sightvision-0.1/setup.py` & `sightvision-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'sightvision',         # How you named your package folder (MyLib)
   packages = ['sightvision'],   # Chose the same as "name"
-  version = '0.1',      # Start with a small number and increase it with every change you make
+  version = '0.1.3',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'This is a Computer vision package that makes its easy to run Image processing and AI functions.',   # Give a short description about your library
   author = 'Leonardi Melo',                   # Type in your name
   author_email = 'opensource.leonardi@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/rexionmars/SightVision',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/rexionmars/SightVision/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['Computervision', 'Imageutils', 'Imageprocessing'],   # Keywords that define your package best
```

### Comparing `sightvision-0.1/sightvision/ClassificationModule.py.py` & `sightvision-0.1.3/sightvision/ClassificationModule.py.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1/sightvision/ColorModule.py` & `sightvision-0.1.3/sightvision/ColorModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1/sightvision/FPS.py` & `sightvision-0.1.3/sightvision/FPS.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1/sightvision/FaceDetectionModule.py` & `sightvision-0.1.3/sightvision/FaceDetectionModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1/sightvision/FaceMeshModule.py` & `sightvision-0.1.3/sightvision/FaceMeshModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1/sightvision/HandTrackingModule.py` & `sightvision-0.1.3/sightvision/HandTrackingModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1/sightvision/PIDModule.py` & `sightvision-0.1.3/sightvision/PIDModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1/sightvision/PlotModule.py` & `sightvision-0.1.3/sightvision/PlotModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1/sightvision/PoseModule.py` & `sightvision-0.1.3/sightvision/PoseModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1/sightvision/SelfiSegmentationModule.py` & `sightvision-0.1.3/sightvision/SelfiSegmentationModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1/sightvision/SerialModule.py` & `sightvision-0.1.3/sightvision/SerialModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1/sightvision/Utils.py` & `sightvision-0.1.3/sightvision/Utils.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1/sightvision.egg-info/PKG-INFO` & `sightvision-0.1.3/sightvision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sightvision
-Version: 0.1
+Version: 0.1.3
 Summary: This is a Computer vision package that makes its easy to run Image processing and AI functions.
 Home-page: https://github.com/rexionmars/SightVision
 Download-URL: https://github.com/rexionmars/SightVision/archive/v_01.tar.gz
 Author: Leonardi Melo
 Author-email: opensource.leonardi@gmail.com
 License: MIT
 Keywords: Computervision,Imageutils,Imageprocessing
```

### Comparing `sightvision-0.1/sightvision.egg-info/SOURCES.txt` & `sightvision-0.1.3/sightvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

