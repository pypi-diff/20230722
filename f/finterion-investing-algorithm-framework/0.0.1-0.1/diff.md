# Comparing `tmp/finterion investing algorithm framework-0.0.1.tar.gz` & `tmp/finterion investing algorithm framework-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finterion investing algorithm framework-0.0.1.tar", last modified: Wed Jul 19 21:19:54 2023, max compression
+gzip compressed data, was "finterion investing algorithm framework-0.1.tar", last modified: Sat Jul 22 20:37:52 2023, max compression
```

## Comparing `finterion investing algorithm framework-0.0.1.tar` & `finterion investing algorithm framework-0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 21:19:54.426500 finterion investing algorithm framework-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-19 21:19:21.000000 finterion investing algorithm framework-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-19 21:19:54.426500 finterion investing algorithm framework-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-19 21:19:21.000000 finterion investing algorithm framework-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 21:19:54.426500 finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-19 21:19:21.000000 finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 21:19:54.426500 finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-19 21:19:21.000000 finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-19 21:19:21.000000 finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework/configuration/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-19 21:19:21.000000 finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework/create_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-19 21:19:21.000000 finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-19 21:19:21.000000 finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework/market_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 21:19:54.426500 finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework/models/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-19 21:19:21.000000 finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-19 21:19:21.000000 finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework/models/portfolio_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 21:19:54.426500 finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-19 21:19:54.000000 finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-19 21:19:54.000000 finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 21:19:54.000000 finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-19 21:19:54.000000 finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-19 21:19:54.000000 finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 21:19:54.426500 finterion investing algorithm framework-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-19 21:19:21.000000 finterion investing algorithm framework-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:37:52.330790 finterion investing algorithm framework-0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-22 20:37:18.000000 finterion investing algorithm framework-0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-22 20:37:52.330790 finterion investing algorithm framework-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-22 20:37:18.000000 finterion investing algorithm framework-0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:37:52.330790 finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-22 20:37:18.000000 finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:37:52.330790 finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-22 20:37:18.000000 finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-22 20:37:18.000000 finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework/configuration/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-22 20:37:18.000000 finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework/create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-22 20:37:18.000000 finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-22 20:37:18.000000 finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework/market_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:37:52.330790 finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-22 20:37:18.000000 finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-22 20:37:18.000000 finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework/models/portfolio_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:37:52.330790 finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-22 20:37:52.000000 finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-22 20:37:52.000000 finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 20:37:52.000000 finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-22 20:37:52.000000 finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-22 20:37:52.000000 finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 20:37:52.330790 finterion investing algorithm framework-0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-22 20:37:18.000000 finterion investing algorithm framework-0.1/setup.py
```

### Comparing `finterion investing algorithm framework-0.0.1/LICENSE` & `finterion investing algorithm framework-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `finterion investing algorithm framework-0.0.1/PKG-INFO` & `finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: finterion investing algorithm framework
-Version: 0.0.1
+Name: finterion-investing-algorithm-framework
+Version: 0.1
 Summary: Official Finterion plugin for the investing algorithm framework
 Home-page: https://github.com/finterion/finterion-investing-algorithm-framework.git
 Author: Finterion
 License: Apache License 2.0
 Keywords: Finterion,finterion,investing-algorithm,investing-algorithm-framework,INVESTING,BOT,ALGORITHM,FRAMEWORK,investing-bots,trading-bots
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -28,25 +28,32 @@
 ```
 
 ## Usage 
 In order to use the plugin you must use the 'create_app' function provided 
 by the plugin. This function will return an instance of the investing 
 algorithm framework configured with the finterion platform.
 
+> **Note:** You must provide the API key of your algorithm in order to use 
+> the plugin. You can find your API keys in the developer dashboard of
+> your algorithm on the finterion platform.
+
 ```python
 import os
 import pathlib
 from datetime import datetime, timedelta
 
 from finterion_investing_algorithm_framework import create_app
 from investing_algorithm_framework import RESOURCE_DIRECTORY, TimeUnit, \
     TradingTimeFrame, TradingDataType, OrderSide
 
 dir_path = os.path.abspath(os.path.join(os.path.realpath(__file__), os.pardir))
-app = create_app({RESOURCE_DIRECTORY: pathlib.Path(__file__).parent.resolve()})
+app = create_app(
+    api_key="<your_api_key>", 
+    config={RESOURCE_DIRECTORY: pathlib.Path(__file__).parent.resolve()}
+)
 
 
 @app.strategy(
     time_unit=TimeUnit.SECOND, # Algorithm will be executed every 5 seconds
     interval=5,
     market="binance", # Will retrieve trading data from binance
     symbols=["BTC/USDT", "ETH/USDT", ["DOT/USDT"]], # Symbols must be in the format of TARGET/TRADE symbol (e.g. BTC/USDT)
```

### Comparing `finterion investing algorithm framework-0.0.1/README.md` & `finterion investing algorithm framework-0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -8,25 +8,32 @@
 ```
 
 ## Usage 
 In order to use the plugin you must use the 'create_app' function provided 
 by the plugin. This function will return an instance of the investing 
 algorithm framework configured with the finterion platform.
 
+> **Note:** You must provide the API key of your algorithm in order to use 
+> the plugin. You can find your API keys in the developer dashboard of
+> your algorithm on the finterion platform.
+
 ```python
 import os
 import pathlib
 from datetime import datetime, timedelta
 
 from finterion_investing_algorithm_framework import create_app
 from investing_algorithm_framework import RESOURCE_DIRECTORY, TimeUnit, \
     TradingTimeFrame, TradingDataType, OrderSide
 
 dir_path = os.path.abspath(os.path.join(os.path.realpath(__file__), os.pardir))
-app = create_app({RESOURCE_DIRECTORY: pathlib.Path(__file__).parent.resolve()})
+app = create_app(
+    api_key="<your_api_key>", 
+    config={RESOURCE_DIRECTORY: pathlib.Path(__file__).parent.resolve()}
+)
 
 
 @app.strategy(
     time_unit=TimeUnit.SECOND, # Algorithm will be executed every 5 seconds
     interval=5,
     market="binance", # Will retrieve trading data from binance
     symbols=["BTC/USDT", "ETH/USDT", ["DOT/USDT"]], # Symbols must be in the format of TARGET/TRADE symbol (e.g. BTC/USDT)
```

### Comparing `finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework/create_app.py` & `finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework/create_app.py`

 * *Files identical despite different names*

### Comparing `finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework/market_service.py` & `finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework/market_service.py`

 * *Files identical despite different names*

### Comparing `finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework/models/portfolio_configuration.py` & `finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework/models/portfolio_configuration.py`

 * *Files identical despite different names*

### Comparing `finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework.egg-info/PKG-INFO` & `finterion investing algorithm framework-0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: finterion-investing-algorithm-framework
-Version: 0.0.1
+Name: finterion investing algorithm framework
+Version: 0.1
 Summary: Official Finterion plugin for the investing algorithm framework
 Home-page: https://github.com/finterion/finterion-investing-algorithm-framework.git
 Author: Finterion
 License: Apache License 2.0
 Keywords: Finterion,finterion,investing-algorithm,investing-algorithm-framework,INVESTING,BOT,ALGORITHM,FRAMEWORK,investing-bots,trading-bots
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -28,25 +28,32 @@
 ```
 
 ## Usage 
 In order to use the plugin you must use the 'create_app' function provided 
 by the plugin. This function will return an instance of the investing 
 algorithm framework configured with the finterion platform.
 
+> **Note:** You must provide the API key of your algorithm in order to use 
+> the plugin. You can find your API keys in the developer dashboard of
+> your algorithm on the finterion platform.
+
 ```python
 import os
 import pathlib
 from datetime import datetime, timedelta
 
 from finterion_investing_algorithm_framework import create_app
 from investing_algorithm_framework import RESOURCE_DIRECTORY, TimeUnit, \
     TradingTimeFrame, TradingDataType, OrderSide
 
 dir_path = os.path.abspath(os.path.join(os.path.realpath(__file__), os.pardir))
-app = create_app({RESOURCE_DIRECTORY: pathlib.Path(__file__).parent.resolve()})
+app = create_app(
+    api_key="<your_api_key>", 
+    config={RESOURCE_DIRECTORY: pathlib.Path(__file__).parent.resolve()}
+)
 
 
 @app.strategy(
     time_unit=TimeUnit.SECOND, # Algorithm will be executed every 5 seconds
     interval=5,
     market="binance", # Will retrieve trading data from binance
     symbols=["BTC/USDT", "ETH/USDT", ["DOT/USDT"]], # Symbols must be in the format of TARGET/TRADE symbol (e.g. BTC/USDT)
```

### Comparing `finterion investing algorithm framework-0.0.1/finterion_investing_algorithm_framework.egg-info/SOURCES.txt` & `finterion investing algorithm framework-0.1/finterion_investing_algorithm_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finterion investing algorithm framework-0.0.1/setup.py` & `finterion investing algorithm framework-0.1/setup.py`

 * *Files identical despite different names*

