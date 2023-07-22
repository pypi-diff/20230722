# Comparing `tmp/pyote-5.3.4.tar.gz` & `tmp/pyote-5.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyote-5.3.4.tar", last modified: Tue Jul 18 18:20:08 2023, max compression
+gzip compressed data, was "pyote-5.3.5.tar", last modified: Sat Jul 22 13:58:18 2023, max compression
```

## Comparing `pyote-5.3.4.tar` & `pyote-5.3.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 18:20:08.025495 pyote-5.3.4/
--rw-rw-rw-   0        0        0     1072 2017-06-14 17:12:14.000000 pyote-5.3.4/LICENSE
--rw-rw-rw-   0        0        0      194 2023-01-09 22:51:18.000000 pyote-5.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1190 2023-07-18 18:20:08.025495 pyote-5.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      285 2017-06-17 03:33:59.000000 pyote-5.3.4/README.rst
--rw-rw-rw-   0        0        0       81 2023-07-18 18:20:08.025495 pyote-5.3.4/setup.cfg
--rw-rw-rw-   0        0        0     2931 2023-07-18 02:09:20.000000 pyote-5.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 18:19:17.026797 pyote-5.3.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 18:20:08.009863 pyote-5.3.4/src/pyote.egg-info/
--rw-rw-rw-   0        0        0     1190 2023-07-18 18:20:07.000000 pyote-5.3.4/src/pyote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1789 2023-07-18 18:20:07.000000 pyote-5.3.4/src/pyote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 18:20:07.000000 pyote-5.3.4/src/pyote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2017-06-17 17:07:51.000000 pyote-5.3.4/src/pyote.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      257 2023-07-18 18:20:07.000000 pyote-5.3.4/src/pyote.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-18 18:20:07.000000 pyote-5.3.4/src/pyote.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-18 18:20:08.025495 pyote-5.3.4/src/pyoteapp/
--rwxrwxrwx   0        0        0      345 2018-11-28 18:46:03.000000 pyote-5.3.4/src/pyoteapp/PYOTE.bat
--rw-rw-rw-   0        0        0     5930 2023-03-27 21:30:02.000000 pyote-5.3.4/src/pyoteapp/SER.py
--rw-rw-rw-   0        0        0        0 2017-06-16 00:35:17.000000 pyote-5.3.4/src/pyoteapp/__init__.py
--rw-rw-rw-   0        0        0     5044 2020-01-10 23:40:03.000000 pyote-5.3.4/src/pyoteapp/autocorrtools.py
--rw-rw-rw-   0        0        0     1251 2020-01-29 05:31:51.000000 pyote-5.3.4/src/pyoteapp/blockIntegrateUtils.py
--rw-rw-rw-   0        0        0     2687 2023-01-10 05:23:59.000000 pyote-5.3.4/src/pyoteapp/checkForNewerVersion.py
--rw-rw-rw-   0        0        0    12525 2023-06-30 14:42:34.000000 pyote-5.3.4/src/pyoteapp/csvreader.py
--rw-rw-rw-   0        0        0    48292 2020-02-09 15:46:46.000000 pyote-5.3.4/src/pyoteapp/diffraction-table.p
--rw-rw-rw-   0        0        0     7549 2022-03-09 14:54:19.000000 pyote-5.3.4/src/pyoteapp/errorBarUtils.py
--rw-rw-rw-   0        0        0     8127 2020-02-15 22:41:06.000000 pyote-5.3.4/src/pyoteapp/example-penumbral.csv
--rw-rw-rw-   0        0        0     3701 2022-01-29 16:31:21.000000 pyote-5.3.4/src/pyoteapp/exponentialEdgeUtilities.py
--rw-rw-rw-   0        0        0     6835 2023-07-16 03:05:04.000000 pyote-5.3.4/src/pyoteapp/false_positive.py
--rw-rw-rw-   0        0        0     1426 2017-06-14 19:28:56.000000 pyote-5.3.4/src/pyoteapp/fixedPrecision.py
--rw-rw-rw-   0        0        0     9761 2022-08-28 02:47:10.000000 pyote-5.3.4/src/pyoteapp/genDiffraction.py
--rw-rw-rw-   0        0        0   386870 2023-07-10 15:37:00.000000 pyote-5.3.4/src/pyoteapp/gui.py
--rw-rw-rw-   0        0        0     1907 2023-06-17 17:37:29.000000 pyote-5.3.4/src/pyoteapp/helpDialog.py
--rw-rw-rw-   0        0        0    25723 2023-07-07 20:15:46.000000 pyote-5.3.4/src/pyoteapp/iterative_logl_functions.py
--rw-rw-rw-   0        0        0     5508 2023-04-09 14:19:52.000000 pyote-5.3.4/src/pyoteapp/likelihood_calculations.py
-drwxrwxrwx   0        0        0        0 2023-07-18 18:20:08.025495 pyote-5.3.4/src/pyoteapp/model-examples/
--rw-rw-rw-   0        0        0     1209 2023-05-29 17:45:05.000000 pyote-5.3.4/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p
--rw-rw-rw-   0        0        0     1204 2023-05-29 18:25:21.000000 pyote-5.3.4/src/pyoteapp/model-examples/LCP_penumbral.p
--rw-rw-rw-   0        0        0    15259 2022-12-25 19:15:36.000000 pyote-5.3.4/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0    15274 2022-12-25 19:15:25.000000 pyote-5.3.4/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0    10519 2022-12-25 19:15:13.000000 pyote-5.3.4/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0     6640 2022-12-25 19:15:12.000000 pyote-5.3.4/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv
--rw-rw-rw-   0        0        0    27881 2022-12-25 19:15:10.000000 pyote-5.3.4/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0   130669 2023-01-08 14:07:02.000000 pyote-5.3.4/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0   882048 2023-01-03 23:22:32.000000 pyote-5.3.4/src/pyoteapp/model-help.pdf
--rw-rw-rw-   0        0        0     1926 2023-05-11 18:15:42.000000 pyote-5.3.4/src/pyoteapp/noiseUtils.py
--rw-rw-rw-   0        0        0   461059 2023-07-18 18:15:27.000000 pyote-5.3.4/src/pyoteapp/pyote-info.pdf
--rw-rw-rw-   0        0        0   451841 2023-07-18 18:10:03.000000 pyote-5.3.4/src/pyoteapp/pyote.py
--rw-rw-rw-   0        0        0    79636 2023-06-17 20:42:15.000000 pyote-5.3.4/src/pyoteapp/pyote_modelling_utility_functions.py
--rwxrwxrwx   0        0        0      321 2018-12-06 17:53:09.000000 pyote-5.3.4/src/pyoteapp/run-pyote-mac.bat
--rw-rw-rw-   0        0        0     6084 2020-04-07 15:06:10.000000 pyote-5.3.4/src/pyoteapp/showVideoFrames.py
--rw-rw-rw-   0        0        0    23501 2023-07-07 02:06:56.000000 pyote-5.3.4/src/pyoteapp/solverUtils.py
--rw-rw-rw-   0        0        0    21983 2022-12-27 20:16:10.000000 pyote-5.3.4/src/pyoteapp/subframe_timing_utilities.py
--rw-rw-rw-   0        0        0    13719 2019-02-01 18:32:12.000000 pyote-5.3.4/src/pyoteapp/timestampDialog.py
--rw-rw-rw-   0        0        0    14937 2023-04-29 22:36:35.000000 pyote-5.3.4/src/pyoteapp/timestampUtils.py
--rw-rw-rw-   0        0        0       34 2023-07-18 18:12:15.000000 pyote-5.3.4/src/pyoteapp/version.py
+drwxrwxrwx   0        0        0        0 2023-07-22 13:58:18.269115 pyote-5.3.5/
+-rw-rw-rw-   0        0        0     1072 2017-06-14 17:12:14.000000 pyote-5.3.5/LICENSE
+-rw-rw-rw-   0        0        0      194 2023-01-09 22:51:18.000000 pyote-5.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1190 2023-07-22 13:58:18.269115 pyote-5.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2017-06-17 03:33:59.000000 pyote-5.3.5/README.rst
+-rw-rw-rw-   0        0        0       81 2023-07-22 13:58:18.269115 pyote-5.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     2945 2023-07-22 13:57:05.000000 pyote-5.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 13:58:18.237864 pyote-5.3.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-22 13:58:18.253490 pyote-5.3.5/src/pyote.egg-info/
+-rw-rw-rw-   0        0        0     1190 2023-07-22 13:58:18.000000 pyote-5.3.5/src/pyote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1789 2023-07-22 13:58:18.000000 pyote-5.3.5/src/pyote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 13:58:18.000000 pyote-5.3.5/src/pyote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2017-06-17 17:07:51.000000 pyote-5.3.5/src/pyote.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      268 2023-07-22 13:58:18.000000 pyote-5.3.5/src/pyote.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-22 13:58:18.000000 pyote-5.3.5/src/pyote.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 13:58:18.269115 pyote-5.3.5/src/pyoteapp/
+-rwxrwxrwx   0        0        0      345 2018-11-28 18:46:03.000000 pyote-5.3.5/src/pyoteapp/PYOTE.bat
+-rw-rw-rw-   0        0        0     5930 2023-03-27 21:30:02.000000 pyote-5.3.5/src/pyoteapp/SER.py
+-rw-rw-rw-   0        0        0        0 2017-06-16 00:35:17.000000 pyote-5.3.5/src/pyoteapp/__init__.py
+-rw-rw-rw-   0        0        0     5044 2020-01-10 23:40:03.000000 pyote-5.3.5/src/pyoteapp/autocorrtools.py
+-rw-rw-rw-   0        0        0     1251 2020-01-29 05:31:51.000000 pyote-5.3.5/src/pyoteapp/blockIntegrateUtils.py
+-rw-rw-rw-   0        0        0     2687 2023-01-10 05:23:59.000000 pyote-5.3.5/src/pyoteapp/checkForNewerVersion.py
+-rw-rw-rw-   0        0        0    12525 2023-06-30 14:42:34.000000 pyote-5.3.5/src/pyoteapp/csvreader.py
+-rw-rw-rw-   0        0        0    48292 2020-02-09 15:46:46.000000 pyote-5.3.5/src/pyoteapp/diffraction-table.p
+-rw-rw-rw-   0        0        0     7549 2022-03-09 14:54:19.000000 pyote-5.3.5/src/pyoteapp/errorBarUtils.py
+-rw-rw-rw-   0        0        0     8127 2020-02-15 22:41:06.000000 pyote-5.3.5/src/pyoteapp/example-penumbral.csv
+-rw-rw-rw-   0        0        0     3701 2022-01-29 16:31:21.000000 pyote-5.3.5/src/pyoteapp/exponentialEdgeUtilities.py
+-rw-rw-rw-   0        0        0     6835 2023-07-16 03:05:04.000000 pyote-5.3.5/src/pyoteapp/false_positive.py
+-rw-rw-rw-   0        0        0     1426 2017-06-14 19:28:56.000000 pyote-5.3.5/src/pyoteapp/fixedPrecision.py
+-rw-rw-rw-   0        0        0     9761 2022-08-28 02:47:10.000000 pyote-5.3.5/src/pyoteapp/genDiffraction.py
+-rw-rw-rw-   0        0        0   386870 2023-07-10 15:37:00.000000 pyote-5.3.5/src/pyoteapp/gui.py
+-rw-rw-rw-   0        0        0     1907 2023-06-17 17:37:29.000000 pyote-5.3.5/src/pyoteapp/helpDialog.py
+-rw-rw-rw-   0        0        0    25723 2023-07-07 20:15:46.000000 pyote-5.3.5/src/pyoteapp/iterative_logl_functions.py
+-rw-rw-rw-   0        0        0     5508 2023-04-09 14:19:52.000000 pyote-5.3.5/src/pyoteapp/likelihood_calculations.py
+drwxrwxrwx   0        0        0        0 2023-07-22 13:58:18.269115 pyote-5.3.5/src/pyoteapp/model-examples/
+-rw-rw-rw-   0        0        0     1209 2023-05-29 17:45:05.000000 pyote-5.3.5/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p
+-rw-rw-rw-   0        0        0     1204 2023-05-29 18:25:21.000000 pyote-5.3.5/src/pyoteapp/model-examples/LCP_penumbral.p
+-rw-rw-rw-   0        0        0    15259 2022-12-25 19:15:36.000000 pyote-5.3.5/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0    15274 2022-12-25 19:15:25.000000 pyote-5.3.5/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0    10519 2022-12-25 19:15:13.000000 pyote-5.3.5/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0     6640 2022-12-25 19:15:12.000000 pyote-5.3.5/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv
+-rw-rw-rw-   0        0        0    27881 2022-12-25 19:15:10.000000 pyote-5.3.5/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0   130669 2023-01-08 14:07:02.000000 pyote-5.3.5/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0   882048 2023-01-03 23:22:32.000000 pyote-5.3.5/src/pyoteapp/model-help.pdf
+-rw-rw-rw-   0        0        0     1926 2023-05-11 18:15:42.000000 pyote-5.3.5/src/pyoteapp/noiseUtils.py
+-rw-rw-rw-   0        0        0   461059 2023-07-18 18:15:27.000000 pyote-5.3.5/src/pyoteapp/pyote-info.pdf
+-rw-rw-rw-   0        0        0   451987 2023-07-22 13:42:16.000000 pyote-5.3.5/src/pyoteapp/pyote.py
+-rw-rw-rw-   0        0        0    79636 2023-06-17 20:42:15.000000 pyote-5.3.5/src/pyoteapp/pyote_modelling_utility_functions.py
+-rwxrwxrwx   0        0        0      321 2018-12-06 17:53:09.000000 pyote-5.3.5/src/pyoteapp/run-pyote-mac.bat
+-rw-rw-rw-   0        0        0     6084 2020-04-07 15:06:10.000000 pyote-5.3.5/src/pyoteapp/showVideoFrames.py
+-rw-rw-rw-   0        0        0    23501 2023-07-07 02:06:56.000000 pyote-5.3.5/src/pyoteapp/solverUtils.py
+-rw-rw-rw-   0        0        0    21983 2022-12-27 20:16:10.000000 pyote-5.3.5/src/pyoteapp/subframe_timing_utilities.py
+-rw-rw-rw-   0        0        0    13719 2019-02-01 18:32:12.000000 pyote-5.3.5/src/pyoteapp/timestampDialog.py
+-rw-rw-rw-   0        0        0    14937 2023-04-29 22:36:35.000000 pyote-5.3.5/src/pyoteapp/timestampUtils.py
+-rw-rw-rw-   0        0        0       34 2023-07-22 01:41:50.000000 pyote-5.3.5/src/pyoteapp/version.py
```

### Comparing `pyote-5.3.4/LICENSE` & `pyote-5.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/PKG-INFO` & `pyote-5.3.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyote
-Version: 5.3.4
+Version: 5.3.5
 Summary: pyote is a simplified subset of R-OTE
 Home-page: https://github.com/bob-anderson-ok/py-ote
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pyote-5.3.4/setup.py` & `pyote-5.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 # This is borrowed from pymovie so that an installation of pyote following a new Anaconda3 install
 # makes no complaints about what pymovie needs, that way the order if intalling pymovie and pyote won't matter
 INSTALL_REQUIRES = ['pyqtgraph==0.12.4', 'opencv-python', 'astroquery', 'resource',
                     'scikit-image(>=0.15.0)', 'wheel', 'requests', 'pyephem',
                     'PyQt5', 'pandas',
                     'winshell;platform_system=="Windows"',
                     'pypiwin32;platform_system=="Windows"', 'matplotlib', 'numpy<=1.22', 'astropy', 'scikit-image',
-                    'scipy', 'numba>=0.41.0', 'Adv2>=1.2.0', 'PyQt5', 'openpyxl', 'xlrd']
+                    'scipy', 'numba>=0.41.0', 'Adv2>=1.2.0', 'PyQt5', 'openpyxl', 'xlrd', 'xlsxwriter']
 
 ###################################################################
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 
 def read(*parts):
```

### Comparing `pyote-5.3.4/src/pyote.egg-info/PKG-INFO` & `pyote-5.3.5/src/pyote.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyote
-Version: 5.3.4
+Version: 5.3.5
 Summary: pyote is a simplified subset of R-OTE
 Home-page: https://github.com/bob-anderson-ok/py-ote
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pyote-5.3.4/src/pyote.egg-info/SOURCES.txt` & `pyote-5.3.5/src/pyote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/SER.py` & `pyote-5.3.5/src/pyoteapp/SER.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/autocorrtools.py` & `pyote-5.3.5/src/pyoteapp/autocorrtools.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/blockIntegrateUtils.py` & `pyote-5.3.5/src/pyoteapp/blockIntegrateUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/checkForNewerVersion.py` & `pyote-5.3.5/src/pyoteapp/checkForNewerVersion.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/csvreader.py` & `pyote-5.3.5/src/pyoteapp/csvreader.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/diffraction-table.p` & `pyote-5.3.5/src/pyoteapp/diffraction-table.p`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/errorBarUtils.py` & `pyote-5.3.5/src/pyoteapp/errorBarUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/example-penumbral.csv` & `pyote-5.3.5/src/pyoteapp/example-penumbral.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/exponentialEdgeUtilities.py` & `pyote-5.3.5/src/pyoteapp/exponentialEdgeUtilities.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/false_positive.py` & `pyote-5.3.5/src/pyoteapp/false_positive.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/fixedPrecision.py` & `pyote-5.3.5/src/pyoteapp/fixedPrecision.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/genDiffraction.py` & `pyote-5.3.5/src/pyoteapp/genDiffraction.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/gui.py` & `pyote-5.3.5/src/pyoteapp/gui.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/helpDialog.py` & `pyote-5.3.5/src/pyoteapp/helpDialog.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/iterative_logl_functions.py` & `pyote-5.3.5/src/pyoteapp/iterative_logl_functions.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/likelihood_calculations.py` & `pyote-5.3.5/src/pyoteapp/likelihood_calculations.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p` & `pyote-5.3.5/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/model-examples/LCP_penumbral.p` & `pyote-5.3.5/src/pyoteapp/model-examples/LCP_penumbral.p`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.3.5/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.3.5/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.3.5/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv` & `pyote-5.3.5/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv` & `pyote-5.3.5/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv` & `pyote-5.3.5/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/model-help.pdf` & `pyote-5.3.5/src/pyoteapp/model-help.pdf`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/noiseUtils.py` & `pyote-5.3.5/src/pyoteapp/noiseUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/pyote-info.pdf` & `pyote-5.3.5/src/pyoteapp/pyote-info.pdf`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/pyote.py` & `pyote-5.3.5/src/pyoteapp/pyote.py`

 * *Files 0% similar despite different names*

```diff
@@ -4853,27 +4853,27 @@
     def clearFitMetricTxtFile(self):
         if self.csvFilePath is None:
             self.showInfo(f'A light curve has not been selected yet\n\n'
                           f'so there is no fit metrics file to remove.')
             return
 
         lightCurveDir = os.path.dirname(self.csvFilePath)  # This gets the folder where the light-curve.csv is located
-        metric_file_path = lightCurveDir + r'\fit_metrics.txt'
+        metric_file_path = os.path.join(lightCurveDir, 'fit_metrics.txt')
         if os.path.exists(metric_file_path):
             os.remove(metric_file_path)
             self.showInfo(f'The fit metrics file has been cleared.')
         return
 
     def renameFitMetricFile(self):
         if self.csvFilePath is None:
             self.showInfo('No lightcurve file selected yet.')
             return
 
         lightCurveDir = os.path.dirname(self.csvFilePath)
-        current_metric_filepath = lightCurveDir + '\\fit_metrics.txt'
+        current_metric_filepath = os.path.join(lightCurveDir, 'fit_metrics.txt')
 
         if not os.path.exists(current_metric_filepath):
             self.showInfo(f'There is no metrics file yet.')
             return
 
         inp = QtWidgets.QInputDialog(self)
         inp.setInputMode(QtWidgets.QInputDialog.InputMode.TextInput)
@@ -4888,20 +4888,21 @@
         head, tail = os.path.split(lightCurveDir)
 
         inp.setTextValue(tail)
 
         if inp.exec_() == QtWidgets.QDialog.DialogCode.Accepted:
             # This gets the folder where the light-curve.csv is located
             lightCurveDir = os.path.dirname(self.csvFilePath)
-            current_metric_filepath = lightCurveDir + '\\fit_metrics.txt'
+            current_metric_filepath = os.path.join(lightCurveDir, 'fit_metrics.txt')
             name_given = inp.textValue()
             if '.xlsx' in name_given:
-                new_metric_filepath = lightCurveDir + f'\\{name_given}'
+                new_metric_filepath = os.path.join(lightCurveDir, f'{name_given}')
             else:
-                new_metric_filepath = lightCurveDir + f'\\{name_given}.xlsx'
+                # new_metric_filepath = lightCurveDir + f'\\{name_given}.xlsx'
+                new_metric_filepath = os.path.join(lightCurveDir, f'{name_given}.xlsx' )
 
             # Make a Pandas data frame from the csv file
             df = pd.read_csv(current_metric_filepath)
 
             # Create a Pandas Excel writer using xlswriter as the engine
             writer = pd.ExcelWriter(new_metric_filepath, engine='xlsxwriter')
 
@@ -7258,15 +7259,15 @@
         self.updateFitMetricTxtFile()
 
         if error_bar_plots_available:
             self.showHelp(self.helpLabelForFalsePositive)
 
     def updateFitMetricTxtFile(self):
         lightCurveDir = os.path.dirname(self.csvFilePath)  # This gets the folder where the light-curve.csv is located
-        metric_file_path = lightCurveDir + r'\fit_metrics.txt'
+        metric_file_path = os.path.join(lightCurveDir, 'fit_metrics.txt')
 
         if os.path.exists(metric_file_path):
             # self.showInfo('We will append to an existing fit_metric.csv file')
             pass
         else:
             # self.showInfo('We fill create a new fit_metric.csv file')
             with open(metric_file_path, 'w') as fileObject:
```

### Comparing `pyote-5.3.4/src/pyoteapp/pyote_modelling_utility_functions.py` & `pyote-5.3.5/src/pyoteapp/pyote_modelling_utility_functions.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/showVideoFrames.py` & `pyote-5.3.5/src/pyoteapp/showVideoFrames.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/solverUtils.py` & `pyote-5.3.5/src/pyoteapp/solverUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/subframe_timing_utilities.py` & `pyote-5.3.5/src/pyoteapp/subframe_timing_utilities.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/timestampDialog.py` & `pyote-5.3.5/src/pyoteapp/timestampDialog.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.4/src/pyoteapp/timestampUtils.py` & `pyote-5.3.5/src/pyoteapp/timestampUtils.py`

 * *Files identical despite different names*

