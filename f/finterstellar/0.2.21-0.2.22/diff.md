# Comparing `tmp/finterstellar-0.2.21.tar.gz` & `tmp/finterstellar-0.2.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finterstellar-0.2.21.tar", last modified: Sat Jul 22 08:51:03 2023, max compression
+gzip compressed data, was "finterstellar-0.2.22.tar", last modified: Sat Jul 22 09:03:53 2023, max compression
```

## Comparing `finterstellar-0.2.21.tar` & `finterstellar-0.2.22.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 08:51:03.084000 finterstellar-0.2.21/
--rw-rw-rw-   0        0        0     1089 2021-03-08 19:23:15.000000 finterstellar-0.2.21/License
--rw-rw-rw-   0        0        0      575 2023-07-22 08:51:03.079000 finterstellar-0.2.21/PKG-INFO
--rw-rw-rw-   0        0        0      105 2021-03-08 19:32:22.000000 finterstellar-0.2.21/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 08:51:02.979000 finterstellar-0.2.21/finterstellar/
--rw-rw-rw-   0        0        0      211 2023-07-22 08:50:10.000000 finterstellar-0.2.21/finterstellar/__init__.py
--rw-rw-rw-   0        0        0     4793 2023-07-22 06:05:37.000000 finterstellar-0.2.21/finterstellar/data_prep.py
--rw-rw-rw-   0        0        0    12206 2023-07-22 06:05:37.000000 finterstellar-0.2.21/finterstellar/financials.py
--rw-rw-rw-   0        0        0     3966 2023-07-22 08:19:33.000000 finterstellar-0.2.21/finterstellar/krx.py
--rw-rw-rw-   0        0        0     7919 2023-07-22 06:05:37.000000 finterstellar-0.2.21/finterstellar/trading.py
--rw-rw-rw-   0        0        0     3800 2023-07-22 06:05:37.000000 finterstellar-0.2.21/finterstellar/trend.py
--rw-rw-rw-   0        0        0     7355 2023-07-22 08:50:24.000000 finterstellar-0.2.21/finterstellar/visualization.py
-drwxrwxrwx   0        0        0        0 2023-07-22 08:51:03.012000 finterstellar-0.2.21/finterstellar.egg-info/
--rw-rw-rw-   0        0        0      575 2023-07-22 08:51:02.000000 finterstellar-0.2.21/finterstellar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      580 2023-07-22 08:51:02.000000 finterstellar-0.2.21/finterstellar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 08:51:02.000000 finterstellar-0.2.21/finterstellar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-22 08:51:02.000000 finterstellar-0.2.21/finterstellar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-07-22 08:51:02.000000 finterstellar-0.2.21/finterstellar.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-22 08:51:03.075000 finterstellar-0.2.21/finterstellar_/
--rw-rw-rw-   0        0        0      214 2023-02-12 02:23:43.000000 finterstellar-0.2.21/finterstellar_/__init__.py
--rw-rw-rw-   0        0        0     5336 2023-02-12 02:23:43.000000 finterstellar-0.2.21/finterstellar_/data_prep.py
--rw-rw-rw-   0        0        0    12206 2023-02-12 02:23:43.000000 finterstellar-0.2.21/finterstellar_/financials.py
--rw-rw-rw-   0        0        0     7722 2023-02-12 02:23:43.000000 finterstellar-0.2.21/finterstellar_/trading.py
--rw-rw-rw-   0        0        0     3706 2023-02-12 02:23:43.000000 finterstellar-0.2.21/finterstellar_/trend.py
--rw-rw-rw-   0        0        0     2374 2023-02-12 02:23:43.000000 finterstellar-0.2.21/finterstellar_/util.py
--rw-rw-rw-   0        0        0     7137 2023-02-12 02:23:43.000000 finterstellar-0.2.21/finterstellar_/visualization.py
--rw-rw-rw-   0        0        0       42 2023-07-22 08:51:03.083000 finterstellar-0.2.21/setup.cfg
--rw-rw-rw-   0        0        0      827 2023-07-22 08:50:30.000000 finterstellar-0.2.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:03:53.756000 finterstellar-0.2.22/
+-rw-rw-rw-   0        0        0     1089 2021-03-08 19:23:15.000000 finterstellar-0.2.22/License
+-rw-rw-rw-   0        0        0      575 2023-07-22 09:03:53.752000 finterstellar-0.2.22/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2021-03-08 19:32:22.000000 finterstellar-0.2.22/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 09:03:53.652000 finterstellar-0.2.22/finterstellar/
+-rw-rw-rw-   0        0        0      211 2023-07-22 08:50:10.000000 finterstellar-0.2.22/finterstellar/__init__.py
+-rw-rw-rw-   0        0        0     4793 2023-07-22 06:05:37.000000 finterstellar-0.2.22/finterstellar/data_prep.py
+-rw-rw-rw-   0        0        0    12206 2023-07-22 06:05:37.000000 finterstellar-0.2.22/finterstellar/financials.py
+-rw-rw-rw-   0        0        0     3966 2023-07-22 08:19:33.000000 finterstellar-0.2.22/finterstellar/krx.py
+-rw-rw-rw-   0        0        0     7919 2023-07-22 06:05:37.000000 finterstellar-0.2.22/finterstellar/trading.py
+-rw-rw-rw-   0        0        0     3800 2023-07-22 06:05:37.000000 finterstellar-0.2.22/finterstellar/trend.py
+-rw-rw-rw-   0        0        0     7304 2023-07-22 09:02:21.000000 finterstellar-0.2.22/finterstellar/visualization.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:03:53.685000 finterstellar-0.2.22/finterstellar.egg-info/
+-rw-rw-rw-   0        0        0      575 2023-07-22 09:03:53.000000 finterstellar-0.2.22/finterstellar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2023-07-22 09:03:53.000000 finterstellar-0.2.22/finterstellar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 09:03:53.000000 finterstellar-0.2.22/finterstellar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-22 09:03:53.000000 finterstellar-0.2.22/finterstellar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-07-22 09:03:53.000000 finterstellar-0.2.22/finterstellar.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 09:03:53.747000 finterstellar-0.2.22/finterstellar_/
+-rw-rw-rw-   0        0        0      214 2023-02-12 02:23:43.000000 finterstellar-0.2.22/finterstellar_/__init__.py
+-rw-rw-rw-   0        0        0     5336 2023-02-12 02:23:43.000000 finterstellar-0.2.22/finterstellar_/data_prep.py
+-rw-rw-rw-   0        0        0    12206 2023-02-12 02:23:43.000000 finterstellar-0.2.22/finterstellar_/financials.py
+-rw-rw-rw-   0        0        0     7722 2023-02-12 02:23:43.000000 finterstellar-0.2.22/finterstellar_/trading.py
+-rw-rw-rw-   0        0        0     3706 2023-02-12 02:23:43.000000 finterstellar-0.2.22/finterstellar_/trend.py
+-rw-rw-rw-   0        0        0     2374 2023-02-12 02:23:43.000000 finterstellar-0.2.22/finterstellar_/util.py
+-rw-rw-rw-   0        0        0     7137 2023-02-12 02:23:43.000000 finterstellar-0.2.22/finterstellar_/visualization.py
+-rw-rw-rw-   0        0        0       42 2023-07-22 09:03:53.755000 finterstellar-0.2.22/setup.cfg
+-rw-rw-rw-   0        0        0      827 2023-07-22 09:03:18.000000 finterstellar-0.2.22/setup.py
```

### Comparing `finterstellar-0.2.21/License` & `finterstellar-0.2.22/License`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.21/PKG-INFO` & `finterstellar-0.2.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finterstellar
-Version: 0.2.21
+Version: 0.2.22
 Summary: Quantitative analysis tools for investment
 Home-page: https://github.com/finterstellar/library
 Author: finterstellar
 Author-email: finterstellar@naver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `finterstellar-0.2.21/finterstellar/data_prep.py` & `finterstellar-0.2.22/finterstellar/data_prep.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.21/finterstellar/financials.py` & `finterstellar-0.2.22/finterstellar/financials.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.21/finterstellar/krx.py` & `finterstellar-0.2.22/finterstellar/krx.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.21/finterstellar/trading.py` & `finterstellar-0.2.22/finterstellar/trading.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.21/finterstellar/trend.py` & `finterstellar-0.2.22/finterstellar/trend.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.21/finterstellar/visualization.py` & `finterstellar-0.2.22/finterstellar/visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from . import data_prep
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.ticker import ScalarFormatter, FixedLocator
-import warnings
-
-warnings.filterwarnings('ignore')
 
 
 ScalarFormatter().set_scientific(False)
-font = 'Malgun Gothic, DejaVu Sans'
+font = 'NanumBarunGothic, DejaVu Sans'
 plt.style.use('bmh')
 plt.rcParams['font.family'] = font
 plt.rcParams['axes.unicode_minus'] = False
 plt.rcParams['axes.grid'] = True
 plt.rcParams['lines.linewidth'] = 1.5
 plt.rcParams['grid.linestyle'] = '--'
 plt.rcParams['grid.alpha'] = 0.7
```

### Comparing `finterstellar-0.2.21/finterstellar.egg-info/PKG-INFO` & `finterstellar-0.2.22/finterstellar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finterstellar
-Version: 0.2.21
+Version: 0.2.22
 Summary: Quantitative analysis tools for investment
 Home-page: https://github.com/finterstellar/library
 Author: finterstellar
 Author-email: finterstellar@naver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `finterstellar-0.2.21/finterstellar.egg-info/SOURCES.txt` & `finterstellar-0.2.22/finterstellar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.21/finterstellar_/data_prep.py` & `finterstellar-0.2.22/finterstellar_/data_prep.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.21/finterstellar_/financials.py` & `finterstellar-0.2.22/finterstellar_/financials.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.21/finterstellar_/trading.py` & `finterstellar-0.2.22/finterstellar_/trading.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.21/finterstellar_/trend.py` & `finterstellar-0.2.22/finterstellar_/trend.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.21/finterstellar_/util.py` & `finterstellar-0.2.22/finterstellar_/util.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.21/finterstellar_/visualization.py` & `finterstellar-0.2.22/finterstellar_/visualization.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.21/setup.py` & `finterstellar-0.2.22/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="finterstellar",
-    version="0.2.21",
+    version="0.2.22",
     author="finterstellar",
     author_email="finterstellar@naver.com",
     description="Quantitative analysis tools for investment",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/finterstellar/library",
     packages=setuptools.find_packages(),
```

