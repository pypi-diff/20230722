# Comparing `tmp/sightvision-0.1.1.tar.gz` & `tmp/sightvision-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sightvision-0.1.1.tar", last modified: Sat Jul 22 16:08:35 2023, max compression
+gzip compressed data, was "sightvision-0.1.4.tar", last modified: Sat Jul 22 21:13:23 2023, max compression
```

## Comparing `sightvision-0.1.1.tar` & `sightvision-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dragon    (1000) dragon    (1000)        0 2023-07-22 16:08:35.290095 sightvision-0.1.1/
--rw-r--r--   0 dragon    (1000) dragon    (1000)     1065 2023-07-21 19:53:53.000000 sightvision-0.1.1/LICENSE.txt
--rw-r--r--   0 dragon    (1000) dragon    (1000)      990 2023-07-22 16:08:35.290095 sightvision-0.1.1/PKG-INFO
--rw-r--r--   0 dragon    (1000) dragon    (1000)      987 2023-07-22 15:23:42.000000 sightvision-0.1.1/README.md
--rw-r--r--   0 dragon    (1000) dragon    (1000)       79 2023-07-22 16:08:35.290095 sightvision-0.1.1/setup.cfg
--rw-r--r--   0 dragon    (1000) dragon    (1000)     1895 2023-07-22 16:08:11.000000 sightvision-0.1.1/setup.py
-drwxr-xr-x   0 dragon    (1000) dragon    (1000)        0 2023-07-22 16:08:35.286762 sightvision-0.1.1/sightvision/
--rw-r--r--   0 dragon    (1000) dragon    (1000)     2265 2023-07-22 02:25:31.000000 sightvision-0.1.1/sightvision/ClassificationModule.py.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     3756 2023-07-22 02:24:49.000000 sightvision-0.1.1/sightvision/ColorModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     1559 2023-07-22 15:47:17.000000 sightvision-0.1.1/sightvision/FPS.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     2361 2023-07-22 02:20:18.000000 sightvision-0.1.1/sightvision/FaceDetectionModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     3607 2023-07-21 23:32:34.000000 sightvision-0.1.1/sightvision/FaceMeshModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     7350 2023-07-22 02:19:49.000000 sightvision-0.1.1/sightvision/HandTrackingModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     2235 2023-07-22 16:03:23.000000 sightvision-0.1.1/sightvision/PIDModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     3423 2023-07-22 02:22:52.000000 sightvision-0.1.1/sightvision/PlotModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     5536 2023-07-22 02:22:27.000000 sightvision-0.1.1/sightvision/PoseModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     1670 2023-07-22 02:21:53.000000 sightvision-0.1.1/sightvision/SelfiSegmentationModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     2213 2023-07-22 02:21:28.000000 sightvision-0.1.1/sightvision/SerialModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     6541 2023-07-22 02:20:48.000000 sightvision-0.1.1/sightvision/Utils.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)      272 2023-07-22 15:24:14.000000 sightvision-0.1.1/sightvision/__init__.py
-drwxr-xr-x   0 dragon    (1000) dragon    (1000)        0 2023-07-22 16:08:35.290095 sightvision-0.1.1/sightvision.egg-info/
--rw-r--r--   0 dragon    (1000) dragon    (1000)      990 2023-07-22 16:08:35.000000 sightvision-0.1.1/sightvision.egg-info/PKG-INFO
--rw-r--r--   0 dragon    (1000) dragon    (1000)      587 2023-07-22 16:08:35.000000 sightvision-0.1.1/sightvision.egg-info/SOURCES.txt
--rw-r--r--   0 dragon    (1000) dragon    (1000)        1 2023-07-22 16:08:35.000000 sightvision-0.1.1/sightvision.egg-info/dependency_links.txt
--rw-r--r--   0 dragon    (1000) dragon    (1000)       24 2023-07-22 16:08:35.000000 sightvision-0.1.1/sightvision.egg-info/requires.txt
--rw-r--r--   0 dragon    (1000) dragon    (1000)       12 2023-07-22 16:08:35.000000 sightvision-0.1.1/sightvision.egg-info/top_level.txt
+drwxr-xr-x   0 dragon    (1000) dragon    (1000)        0 2023-07-22 21:13:23.116717 sightvision-0.1.4/
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     1065 2023-07-21 19:53:53.000000 sightvision-0.1.4/LICENSE.txt
+-rw-r--r--   0 dragon    (1000) dragon    (1000)      914 2023-07-22 21:13:23.116717 sightvision-0.1.4/PKG-INFO
+-rw-r--r--   0 dragon    (1000) dragon    (1000)      987 2023-07-22 15:23:42.000000 sightvision-0.1.4/README.md
+-rw-r--r--   0 dragon    (1000) dragon    (1000)       79 2023-07-22 21:13:23.116717 sightvision-0.1.4/setup.cfg
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     1960 2023-07-22 21:13:02.000000 sightvision-0.1.4/setup.py
+drwxr-xr-x   0 dragon    (1000) dragon    (1000)        0 2023-07-22 21:13:23.113384 sightvision-0.1.4/sightvision/
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     2265 2023-07-22 02:25:31.000000 sightvision-0.1.4/sightvision/ClassificationModule.py.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     3756 2023-07-22 02:24:49.000000 sightvision-0.1.4/sightvision/ColorModule.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     1559 2023-07-22 15:47:17.000000 sightvision-0.1.4/sightvision/FPS.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     2361 2023-07-22 02:20:18.000000 sightvision-0.1.4/sightvision/FaceDetectionModule.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     3607 2023-07-21 23:32:34.000000 sightvision-0.1.4/sightvision/FaceMeshModule.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     7350 2023-07-22 02:19:49.000000 sightvision-0.1.4/sightvision/HandTrackingModule.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     2235 2023-07-22 16:03:23.000000 sightvision-0.1.4/sightvision/PIDModule.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     3423 2023-07-22 02:22:52.000000 sightvision-0.1.4/sightvision/PlotModule.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     5536 2023-07-22 02:22:27.000000 sightvision-0.1.4/sightvision/PoseModule.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     1670 2023-07-22 02:21:53.000000 sightvision-0.1.4/sightvision/SelfiSegmentationModule.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     2213 2023-07-22 02:21:28.000000 sightvision-0.1.4/sightvision/SerialModule.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)     6541 2023-07-22 02:20:48.000000 sightvision-0.1.4/sightvision/Utils.py
+-rw-r--r--   0 dragon    (1000) dragon    (1000)      637 2023-07-22 21:10:19.000000 sightvision-0.1.4/sightvision/__init__.py
+drwxr-xr-x   0 dragon    (1000) dragon    (1000)        0 2023-07-22 21:13:23.113384 sightvision-0.1.4/sightvision.egg-info/
+-rw-r--r--   0 dragon    (1000) dragon    (1000)      914 2023-07-22 21:13:22.000000 sightvision-0.1.4/sightvision.egg-info/PKG-INFO
+-rw-r--r--   0 dragon    (1000) dragon    (1000)      587 2023-07-22 21:13:23.000000 sightvision-0.1.4/sightvision.egg-info/SOURCES.txt
+-rw-r--r--   0 dragon    (1000) dragon    (1000)        1 2023-07-22 21:13:22.000000 sightvision-0.1.4/sightvision.egg-info/dependency_links.txt
+-rw-r--r--   0 dragon    (1000) dragon    (1000)       48 2023-07-22 21:13:22.000000 sightvision-0.1.4/sightvision.egg-info/requires.txt
+-rw-r--r--   0 dragon    (1000) dragon    (1000)       12 2023-07-22 21:13:22.000000 sightvision-0.1.4/sightvision.egg-info/top_level.txt
```

### Comparing `sightvision-0.1.1/LICENSE.txt` & `sightvision-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sightvision-0.1.1/README.md` & `sightvision-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sightvision-0.1.1/setup.py` & `sightvision-0.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from distutils.core import setup
 setup(
   name = 'sightvision',         # How you named your package folder (MyLib)
   packages = ['sightvision'],   # Chose the same as "name"
-  version = '0.1.1',      # Start with a small number and increase it with every change you make
+  version = '0.1.4',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'This is a Computer vision package that makes its easy to run Image processing and AI functions.',   # Give a short description about your library
   author = 'Leonardi Melo',                   # Type in your name
   author_email = 'opensource.leonardi@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/rexionmars/SightVision',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/rexionmars/SightVision/archive/v_01.tar.gz',    # I explain this later on
+  #download_url = 'https://github.com/rexionmars/SightVision/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['Computervision', 'Imageutils', 'Imageprocessing'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'opencv-python',
           'mediapipe',
+          'tensorflow',
+          'serial',
+          'numpy',
+
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
```

### Comparing `sightvision-0.1.1/sightvision/ClassificationModule.py.py` & `sightvision-0.1.4/sightvision/ClassificationModule.py.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1.1/sightvision/ColorModule.py` & `sightvision-0.1.4/sightvision/ColorModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1.1/sightvision/FPS.py` & `sightvision-0.1.4/sightvision/FPS.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1.1/sightvision/FaceDetectionModule.py` & `sightvision-0.1.4/sightvision/FaceDetectionModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1.1/sightvision/FaceMeshModule.py` & `sightvision-0.1.4/sightvision/FaceMeshModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1.1/sightvision/HandTrackingModule.py` & `sightvision-0.1.4/sightvision/HandTrackingModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1.1/sightvision/PIDModule.py` & `sightvision-0.1.4/sightvision/PIDModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1.1/sightvision/PlotModule.py` & `sightvision-0.1.4/sightvision/PlotModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1.1/sightvision/PoseModule.py` & `sightvision-0.1.4/sightvision/PoseModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1.1/sightvision/SelfiSegmentationModule.py` & `sightvision-0.1.4/sightvision/SelfiSegmentationModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1.1/sightvision/SerialModule.py` & `sightvision-0.1.4/sightvision/SerialModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1.1/sightvision/Utils.py` & `sightvision-0.1.4/sightvision/Utils.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.1.1/sightvision.egg-info/SOURCES.txt` & `sightvision-0.1.4/sightvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

