# Comparing `tmp/finterstellar-0.2.18.tar.gz` & `tmp/finterstellar-0.2.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finterstellar-0.2.18.tar", last modified: Sat Jul 22 08:14:02 2023, max compression
+gzip compressed data, was "finterstellar-0.2.19.tar", last modified: Sat Jul 22 08:21:43 2023, max compression
```

## Comparing `finterstellar-0.2.18.tar` & `finterstellar-0.2.19.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 08:14:02.415000 finterstellar-0.2.18/
--rw-rw-rw-   0        0        0     1089 2021-03-08 19:23:15.000000 finterstellar-0.2.18/License
--rw-rw-rw-   0        0        0      575 2023-07-22 08:14:02.410000 finterstellar-0.2.18/PKG-INFO
--rw-rw-rw-   0        0        0      105 2021-03-08 19:32:22.000000 finterstellar-0.2.18/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 08:14:02.293000 finterstellar-0.2.18/finterstellar/
--rw-rw-rw-   0        0        0      213 2023-07-22 08:12:41.000000 finterstellar-0.2.18/finterstellar/__init__.py
--rw-rw-rw-   0        0        0     4793 2023-07-22 06:05:37.000000 finterstellar-0.2.18/finterstellar/data_prep.py
--rw-rw-rw-   0        0        0    12206 2023-07-22 06:05:37.000000 finterstellar-0.2.18/finterstellar/financials.py
--rw-rw-rw-   0        0        0     3962 2023-07-22 07:55:07.000000 finterstellar-0.2.18/finterstellar/krx.py
--rw-rw-rw-   0        0        0     7919 2023-07-22 06:05:37.000000 finterstellar-0.2.18/finterstellar/trading.py
--rw-rw-rw-   0        0        0     3800 2023-07-22 06:05:37.000000 finterstellar-0.2.18/finterstellar/trend.py
--rw-rw-rw-   0        0        0     7332 2023-07-22 06:05:37.000000 finterstellar-0.2.18/finterstellar/visualization.py
-drwxrwxrwx   0        0        0        0 2023-07-22 08:14:02.332000 finterstellar-0.2.18/finterstellar.egg-info/
--rw-rw-rw-   0        0        0      575 2023-07-22 08:14:02.000000 finterstellar-0.2.18/finterstellar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      580 2023-07-22 08:14:02.000000 finterstellar-0.2.18/finterstellar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 08:14:02.000000 finterstellar-0.2.18/finterstellar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-22 08:14:02.000000 finterstellar-0.2.18/finterstellar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-07-22 08:14:02.000000 finterstellar-0.2.18/finterstellar.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-22 08:14:02.405000 finterstellar-0.2.18/finterstellar_/
--rw-rw-rw-   0        0        0      214 2023-02-12 02:23:43.000000 finterstellar-0.2.18/finterstellar_/__init__.py
--rw-rw-rw-   0        0        0     5336 2023-02-12 02:23:43.000000 finterstellar-0.2.18/finterstellar_/data_prep.py
--rw-rw-rw-   0        0        0    12206 2023-02-12 02:23:43.000000 finterstellar-0.2.18/finterstellar_/financials.py
--rw-rw-rw-   0        0        0     7722 2023-02-12 02:23:43.000000 finterstellar-0.2.18/finterstellar_/trading.py
--rw-rw-rw-   0        0        0     3706 2023-02-12 02:23:43.000000 finterstellar-0.2.18/finterstellar_/trend.py
--rw-rw-rw-   0        0        0     2374 2023-02-12 02:23:43.000000 finterstellar-0.2.18/finterstellar_/util.py
--rw-rw-rw-   0        0        0     7137 2023-02-12 02:23:43.000000 finterstellar-0.2.18/finterstellar_/visualization.py
--rw-rw-rw-   0        0        0       42 2023-07-22 08:14:02.414000 finterstellar-0.2.18/setup.cfg
--rw-rw-rw-   0        0        0      827 2023-07-22 08:13:36.000000 finterstellar-0.2.18/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:21:43.215000 finterstellar-0.2.19/
+-rw-rw-rw-   0        0        0     1089 2021-03-08 19:23:15.000000 finterstellar-0.2.19/License
+-rw-rw-rw-   0        0        0      575 2023-07-22 08:21:43.210000 finterstellar-0.2.19/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2021-03-08 19:32:22.000000 finterstellar-0.2.19/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 08:21:43.101000 finterstellar-0.2.19/finterstellar/
+-rw-rw-rw-   0        0        0      211 2023-07-22 08:19:20.000000 finterstellar-0.2.19/finterstellar/__init__.py
+-rw-rw-rw-   0        0        0     4793 2023-07-22 06:05:37.000000 finterstellar-0.2.19/finterstellar/data_prep.py
+-rw-rw-rw-   0        0        0    12206 2023-07-22 06:05:37.000000 finterstellar-0.2.19/finterstellar/financials.py
+-rw-rw-rw-   0        0        0     3966 2023-07-22 08:19:33.000000 finterstellar-0.2.19/finterstellar/krx.py
+-rw-rw-rw-   0        0        0     7919 2023-07-22 06:05:37.000000 finterstellar-0.2.19/finterstellar/trading.py
+-rw-rw-rw-   0        0        0     3800 2023-07-22 06:05:37.000000 finterstellar-0.2.19/finterstellar/trend.py
+-rw-rw-rw-   0        0        0     7332 2023-07-22 06:05:37.000000 finterstellar-0.2.19/finterstellar/visualization.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:21:43.137000 finterstellar-0.2.19/finterstellar.egg-info/
+-rw-rw-rw-   0        0        0      575 2023-07-22 08:21:42.000000 finterstellar-0.2.19/finterstellar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2023-07-22 08:21:42.000000 finterstellar-0.2.19/finterstellar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 08:21:42.000000 finterstellar-0.2.19/finterstellar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-22 08:21:42.000000 finterstellar-0.2.19/finterstellar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-07-22 08:21:42.000000 finterstellar-0.2.19/finterstellar.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 08:21:43.205000 finterstellar-0.2.19/finterstellar_/
+-rw-rw-rw-   0        0        0      214 2023-02-12 02:23:43.000000 finterstellar-0.2.19/finterstellar_/__init__.py
+-rw-rw-rw-   0        0        0     5336 2023-02-12 02:23:43.000000 finterstellar-0.2.19/finterstellar_/data_prep.py
+-rw-rw-rw-   0        0        0    12206 2023-02-12 02:23:43.000000 finterstellar-0.2.19/finterstellar_/financials.py
+-rw-rw-rw-   0        0        0     7722 2023-02-12 02:23:43.000000 finterstellar-0.2.19/finterstellar_/trading.py
+-rw-rw-rw-   0        0        0     3706 2023-02-12 02:23:43.000000 finterstellar-0.2.19/finterstellar_/trend.py
+-rw-rw-rw-   0        0        0     2374 2023-02-12 02:23:43.000000 finterstellar-0.2.19/finterstellar_/util.py
+-rw-rw-rw-   0        0        0     7137 2023-02-12 02:23:43.000000 finterstellar-0.2.19/finterstellar_/visualization.py
+-rw-rw-rw-   0        0        0       42 2023-07-22 08:21:43.214000 finterstellar-0.2.19/setup.cfg
+-rw-rw-rw-   0        0        0      827 2023-07-22 08:20:31.000000 finterstellar-0.2.19/setup.py
```

### Comparing `finterstellar-0.2.18/License` & `finterstellar-0.2.19/License`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.18/PKG-INFO` & `finterstellar-0.2.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finterstellar
-Version: 0.2.18
+Version: 0.2.19
 Summary: Quantitative analysis tools for investment
 Home-page: https://github.com/finterstellar/library
 Author: finterstellar
 Author-email: finterstellar@naver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `finterstellar-0.2.18/finterstellar/data_prep.py` & `finterstellar-0.2.19/finterstellar/data_prep.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.18/finterstellar/financials.py` & `finterstellar-0.2.19/finterstellar/financials.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.18/finterstellar/krx.py` & `finterstellar-0.2.19/finterstellar/krx.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 df_elw = pd.DataFrame.from_dict(rst)
 
 # 종합
 df_master = pd.concat([df_equity, df_etf, df_etn, df_elw])
 df_master = df_master[['ISU_CD', 'ISU_SRT_CD', 'ISU_ABBRV']]
 
 
-def get_price(symbol='000660', start_date=None, end_date=None):
+def get_krx_price(symbol='000660', start_date=None, end_date=None):
     # 종목정보 선택
     stock = df_master[df_master['ISU_SRT_CD']==symbol] if len(df_master[df_master['ISU_ABBRV']==symbol.upper()])<1 else df_master[df_master['ISU_ABBRV']==symbol.upper()]
     print(stock[['ISU_SRT_CD', 'ISU_ABBRV']])
     if len(stock) > 0:
         # 입력인자 세팅
         start_date = pd.to_datetime(start_date).strftime('%Y%m%d') if start_date else (pd.Timestamp.today()-pd.DateOffset(days=7)).strftime('%Y%m%d')
         end_date = pd.to_datetime(end_date).strftime('%Y%m%d') if end_date else pd.Timestamp.today().strftime('%Y%m%d')
```

### Comparing `finterstellar-0.2.18/finterstellar/trading.py` & `finterstellar-0.2.19/finterstellar/trading.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.18/finterstellar/trend.py` & `finterstellar-0.2.19/finterstellar/trend.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.18/finterstellar/visualization.py` & `finterstellar-0.2.19/finterstellar/visualization.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.18/finterstellar.egg-info/PKG-INFO` & `finterstellar-0.2.19/finterstellar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finterstellar
-Version: 0.2.18
+Version: 0.2.19
 Summary: Quantitative analysis tools for investment
 Home-page: https://github.com/finterstellar/library
 Author: finterstellar
 Author-email: finterstellar@naver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `finterstellar-0.2.18/finterstellar.egg-info/SOURCES.txt` & `finterstellar-0.2.19/finterstellar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.18/finterstellar_/data_prep.py` & `finterstellar-0.2.19/finterstellar_/data_prep.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.18/finterstellar_/financials.py` & `finterstellar-0.2.19/finterstellar_/financials.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.18/finterstellar_/trading.py` & `finterstellar-0.2.19/finterstellar_/trading.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.18/finterstellar_/trend.py` & `finterstellar-0.2.19/finterstellar_/trend.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.18/finterstellar_/util.py` & `finterstellar-0.2.19/finterstellar_/util.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.18/finterstellar_/visualization.py` & `finterstellar-0.2.19/finterstellar_/visualization.py`

 * *Files identical despite different names*

### Comparing `finterstellar-0.2.18/setup.py` & `finterstellar-0.2.19/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="finterstellar",
-    version="0.2.18",
+    version="0.2.19",
     author="finterstellar",
     author_email="finterstellar@naver.com",
     description="Quantitative analysis tools for investment",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/finterstellar/library",
     packages=setuptools.find_packages(),
```

