# Comparing `tmp/crypto-screening-7.5.5.tar.gz` & `tmp/crypto-screening-7.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-7.5.5.tar", last modified: Fri Jul 21 23:40:08 2023, max compression
+gzip compressed data, was "crypto-screening-7.5.6.tar", last modified: Sat Jul 22 09:34:07 2023, max compression
```

## Comparing `crypto-screening-7.5.5.tar` & `crypto-screening-7.5.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 23:40:08.023061 crypto-screening-7.5.5/
--rw-rw-rw-   0        0        0      196 2023-07-21 23:40:07.000000 crypto-screening-7.5.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-21 23:40:08.023061 crypto-screening-7.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-7.5.5/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-7.5.5/build.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:40:07.985057 crypto-screening-7.5.5/crypto_screening/
--rw-rw-rw-   0        0        0     1002 2023-07-21 10:49:22.000000 crypto-screening-7.5.5/crypto_screening/base.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:40:08.001057 crypto-screening-7.5.5/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-7.5.5/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-7.5.5/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:40:08.005057 crypto-screening-7.5.5/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-7.5.5/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-7.5.5/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-7.5.5/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-7.5.5/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:40:08.007057 crypto-screening-7.5.5/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-7.5.5/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24729 2023-07-20 08:01:55.000000 crypto-screening-7.5.5/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    16341 2023-07-21 10:15:56.000000 crypto-screening-7.5.5/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21717 2023-07-20 08:01:55.000000 crypto-screening-7.5.5/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-7.5.5/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    16799 2023-07-20 15:36:57.000000 crypto-screening-7.5.5/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19514 2023-07-21 10:12:10.000000 crypto-screening-7.5.5/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-7.5.5/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0     1007 2023-07-21 10:52:54.000000 crypto-screening-7.5.5/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-7.5.5/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:40:08.009057 crypto-screening-7.5.5/crypto_screening/market/
--rw-rw-rw-   0        0        0    14279 2023-07-21 23:39:53.000000 crypto-screening-7.5.5/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:40:08.011057 crypto-screening-7.5.5/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-7.5.5/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-7.5.5/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-7.5.5/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-7.5.5/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:40:08.019057 crypto-screening-7.5.5/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      519 2023-07-20 15:38:19.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    15448 2023-07-21 23:25:16.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    13798 2023-07-20 15:24:13.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/callbacks.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:40:08.021057 crypto-screening-7.5.5/crypto_screening/market/screeners/collectors/
--rw-rw-rw-   0        0        0      217 2023-07-20 15:09:26.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/collectors/__init__.py
--rw-rw-rw-   0        0        0     3602 2023-07-21 23:25:16.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/collectors/base.py
--rw-rw-rw-   0        0        0     3988 2023-07-21 08:58:50.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/collectors/database.py
--rw-rw-rw-   0        0        0     5952 2023-07-20 15:13:32.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/collectors/sockets.py
--rw-rw-rw-   0        0        0    13450 2023-07-20 08:33:40.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    20177 2023-07-21 23:36:03.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    10983 2023-07-21 08:58:32.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/database.py
--rw-rw-rw-   0        0        0    37526 2023-07-21 11:02:21.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    17713 2023-07-21 12:44:32.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    17240 2023-07-21 12:44:17.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    20611 2023-07-19 16:46:01.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0    17314 2023-07-21 12:44:28.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-7.5.5/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-7.5.5/crypto_screening/process.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:40:07.975476 crypto-screening-7.5.5/crypto_screening/source/
-drwxrwxrwx   0        0        0        0 2023-07-21 23:40:08.022057 crypto-screening-7.5.5/crypto_screening/source/data/
--rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-7.5.5/crypto_screening/source/data/all_exchanges_symbols.json
--rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-7.5.5/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-7.5.5/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:40:07.998057 crypto-screening-7.5.5/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-21 23:40:07.000000 crypto-screening-7.5.5/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2070 2023-07-21 23:40:07.000000 crypto-screening-7.5.5/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 23:40:07.000000 crypto-screening-7.5.5/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-21 23:40:07.000000 crypto-screening-7.5.5/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-21 23:40:07.000000 crypto-screening-7.5.5/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-21 23:40:07.000000 crypto-screening-7.5.5/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-7.5.5/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-7.5.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 23:40:08.024061 crypto-screening-7.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-07-21 23:40:01.000000 crypto-screening-7.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.189436 crypto-screening-7.5.6/
+-rw-rw-rw-   0        0        0      196 2023-07-22 09:34:06.000000 crypto-screening-7.5.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-22 09:34:07.189436 crypto-screening-7.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-7.5.6/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-7.5.6/build.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.011671 crypto-screening-7.5.6/crypto_screening/
+-rw-rw-rw-   0        0        0     1002 2023-07-21 10:49:22.000000 crypto-screening-7.5.6/crypto_screening/base.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.049275 crypto-screening-7.5.6/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-7.5.6/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-7.5.6/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.079244 crypto-screening-7.5.6/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-7.5.6/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-7.5.6/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-7.5.6/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-7.5.6/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.101723 crypto-screening-7.5.6/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-7.5.6/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24729 2023-07-20 08:01:55.000000 crypto-screening-7.5.6/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    16341 2023-07-21 10:15:56.000000 crypto-screening-7.5.6/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21717 2023-07-20 08:01:55.000000 crypto-screening-7.5.6/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-7.5.6/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    16799 2023-07-20 15:36:57.000000 crypto-screening-7.5.6/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19514 2023-07-21 10:12:10.000000 crypto-screening-7.5.6/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-7.5.6/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0     1007 2023-07-21 10:52:54.000000 crypto-screening-7.5.6/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-7.5.6/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.112767 crypto-screening-7.5.6/crypto_screening/market/
+-rw-rw-rw-   0        0        0    14279 2023-07-21 23:39:53.000000 crypto-screening-7.5.6/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.136276 crypto-screening-7.5.6/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-7.5.6/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-7.5.6/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-7.5.6/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-7.5.6/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.181438 crypto-screening-7.5.6/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      519 2023-07-20 15:38:19.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    15448 2023-07-21 23:25:16.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    13798 2023-07-20 15:24:13.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/callbacks.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.187437 crypto-screening-7.5.6/crypto_screening/market/screeners/collectors/
+-rw-rw-rw-   0        0        0      217 2023-07-20 15:09:26.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     6340 2023-07-22 09:28:50.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     4055 2023-07-22 09:26:50.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     6116 2023-07-22 09:26:50.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    13450 2023-07-20 08:33:40.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    20177 2023-07-21 23:36:03.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    10983 2023-07-21 08:58:32.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/database.py
+-rw-rw-rw-   0        0        0    37526 2023-07-21 11:02:21.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    17713 2023-07-21 12:44:32.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    17240 2023-07-21 12:44:17.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    20611 2023-07-19 16:46:01.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0    17314 2023-07-21 12:44:28.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-7.5.6/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-7.5.6/crypto_screening/process.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:34:06.968784 crypto-screening-7.5.6/crypto_screening/source/
+drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.188437 crypto-screening-7.5.6/crypto_screening/source/data/
+-rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-7.5.6/crypto_screening/source/data/all_exchanges_symbols.json
+-rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-7.5.6/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-7.5.6/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.025706 crypto-screening-7.5.6/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-22 09:34:06.000000 crypto-screening-7.5.6/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2070 2023-07-22 09:34:06.000000 crypto-screening-7.5.6/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 09:34:06.000000 crypto-screening-7.5.6/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-22 09:34:06.000000 crypto-screening-7.5.6/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-22 09:34:06.000000 crypto-screening-7.5.6/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-22 09:34:06.000000 crypto-screening-7.5.6/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-7.5.6/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-7.5.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-22 09:34:07.189436 crypto-screening-7.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-07-22 09:33:58.000000 crypto-screening-7.5.6/setup.py
```

### Comparing `crypto-screening-7.5.5/PKG-INFO` & `crypto-screening-7.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 7.5.5
+Version: 7.5.6
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-7.5.5/README.md` & `crypto-screening-7.5.6/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/build.py` & `crypto-screening-7.5.6/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/base.py` & `crypto-screening-7.5.6/crypto_screening/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/collect/assets.py` & `crypto-screening-7.5.6/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/collect/exchanges.py` & `crypto-screening-7.5.6/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-7.5.6/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/collect/market/orderbook.py` & `crypto-screening-7.5.6/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/collect/market/orders.py` & `crypto-screening-7.5.6/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/collect/market/state/assets.py` & `crypto-screening-7.5.6/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/collect/market/state/base.py` & `crypto-screening-7.5.6/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-7.5.6/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/collect/market/trades.py` & `crypto-screening-7.5.6/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/collect/screeners.py` & `crypto-screening-7.5.6/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/collect/symbols.py` & `crypto-screening-7.5.6/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/dataset.py` & `crypto-screening-7.5.6/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/exchanges.py` & `crypto-screening-7.5.6/crypto_screening/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/interval.py` & `crypto-screening-7.5.6/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/market/dynamic.py` & `crypto-screening-7.5.6/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/market/foundation/data.py` & `crypto-screening-7.5.6/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/market/foundation/protocols.py` & `crypto-screening-7.5.6/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/market/foundation/state.py` & `crypto-screening-7.5.6/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/market/foundation/waiting.py` & `crypto-screening-7.5.6/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/market/screeners/__init__.py` & `crypto-screening-7.5.6/crypto_screening/market/screeners/__init__.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/market/screeners/base.py` & `crypto-screening-7.5.6/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/market/screeners/callbacks.py` & `crypto-screening-7.5.6/crypto_screening/market/screeners/callbacks.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/market/screeners/collectors/base.py` & `crypto-screening-7.5.6/crypto_screening/market/waiting.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,120 +1,114 @@
-# base.py
+# waiting.py
 
-import warnings
-import threading
 import datetime as dt
-from typing import List, Tuple, Optional, Iterable, Union, Dict
-
-from crypto_screening.market.screeners.base import BaseScreener, BaseMarketController
-from crypto_screening.market.screeners.container import ScreenersContainer
-from crypto_screening.collect.market.state.base import index_to_datetime
+from typing import (
+    Optional, Union, Iterable
+)
+
+from crypto_screening.collect.screeners import gather_screeners
+from crypto_screening.market.screeners import BaseScreener, BaseMarketScreener
+from crypto_screening.market.foundation.state import WaitingState
+from crypto_screening.market.foundation.waiting import (
+    base_await_update, base_await_dynamic_initialization,
+    base_await_initialization, base_await_dynamic_update
+)
 
 __all__ = [
-    "ScreenersDataCollector"
+    "await_dynamic_initialization",
+    "await_update",
+    "await_initialization",
+    "await_dynamic_update",
+    "WaitingState"
 ]
 
-Data = List[Tuple[Union[str, float, dt.datetime], Dict[str, Optional[Union[str, float, bool]]]]]
+def await_dynamic_initialization(
+        screeners: Iterable[Union[BaseScreener, BaseMarketScreener]],
+        stop: Optional[bool] = None,
+        delay: Optional[Union[float, dt.timedelta]] = None,
+        cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
+) -> WaitingState:
+    """
+    Waits for all the create_screeners to update.
+
+    :param screeners: The create_screeners to wait for them to update.
+    :param delay: The delay for the waiting.
+    :param stop: The value to stop the screener objects.
+    :param cancel: The time to cancel the waiting.
+
+    :returns: The total delay.
+    """
+
+    return base_await_dynamic_initialization(
+        screeners=screeners, stop=stop, delay=delay,
+        cancel=cancel, gatherer=gather_screeners
+    )
+# end await_dynamic_initialization
+
+def await_initialization(
+        *screeners: Union[BaseScreener, BaseMarketScreener],
+        stop: Optional[bool] = False,
+        delay: Optional[Union[float, dt.timedelta]] = None,
+        cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
+) -> WaitingState:
+    """
+    Waits for all the create_screeners to update.
+
+    :param screeners: The create_screeners to wait for them to update.
+    :param delay: The delay for the waiting.
+    :param stop: The value to stop the screener objects.
+    :param cancel: The time to cancel the waiting.
+
+    :returns: The total delay.
+    """
+
+    return base_await_initialization(
+        *screeners, stop=stop, delay=delay,
+        cancel=cancel, gatherer=gather_screeners
+    )
+# end await_initialization
+
+def await_dynamic_update(
+        screeners: Iterable[Union[BaseScreener, BaseMarketScreener]],
+        stop: Optional[bool] = False,
+        delay: Optional[Union[float, dt.timedelta]] = None,
+        cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
+) -> WaitingState:
+    """
+    Waits for all the create_screeners to update.
+
+    :param screeners: The create_screeners to wait for them to update.
+    :param delay: The delay for the waiting.
+    :param stop: The value to stop the screener objects.
+    :param cancel: The time to cancel the waiting.
+
+    :returns: The total delay.
+    """
+
+    return base_await_dynamic_update(
+        screeners=screeners, stop=stop, delay=delay,
+        cancel=cancel, gatherer=gather_screeners
+    )
+# end await_dynamic_update
+
+def await_update(
+        *screeners: Union[BaseScreener, BaseMarketScreener],
+        stop: Optional[bool] = False,
+        delay: Optional[Union[float, dt.timedelta]] = None,
+        cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
+) -> WaitingState:
+    """
+    Waits for all the create_screeners to update.
+
+    :param screeners: The create_screeners to wait for them to update.
+    :param delay: The delay for the waiting.
+    :param stop: The value to stop the screener objects.
+    :param cancel: The time to cancel the waiting.
 
-class ScreenersDataCollector(ScreenersContainer, BaseMarketController):
+    :returns: The total delay.
     """
-    A class to represent an asset price screener.
 
-    Using this class, you can create a screener object to
-    screen the market ask and bid data for a specific asset in
-    a specific exchange at real time.
-
-    Parameters:
-
-    - screeners:
-        The screener object to control and fill with data.
-
-    - location:
-        The saving location for the saved data of the screener.
-
-    - cancel:
-        The time to cancel screening process after no new data is fetched.
-
-    - delay:
-        The delay to wait between each data fetching.
-
-    - screeners:
-        The screener object to control and fill with data.
-    """
-
-    def __init__(
-            self,
-            screeners: Optional[Iterable[BaseScreener]] = None,
-            location: Optional[str] = None,
-            cancel: Optional[Union[float, dt.timedelta]] = None,
-            delay: Optional[Union[float, dt.timedelta]] = None
-    ) -> None:
-        """
-        Defines the class attributes.
-
-        :param location: The saving location for the data.
-        :param delay: The delay for the process.
-        :param cancel: The cancel time for the loops.
-        """
-
-        BaseMarketController.__init__(
-            self, location=location, cancel=cancel, delay=delay
-        )
-
-        ScreenersContainer.__init__(self, screeners=screeners)
-    # end __init__
-
-    def handle(
-            self,
-            name: str,
-            exchange: str,
-            symbol: str,
-            interval: str,
-            data: Data
-    ) -> None:
-        """
-        Handles the data received from the connection.
-
-        :param data: The data to handle.
-        :param name: The name of the data.
-        :param exchange: The exchange of the screener.
-        :param symbol: The symbol of the screener.
-        :param interval: The interval of the screener.
-        """
-
-        screeners = self.find_screeners(
-            base=BaseScreener.SCREENER_NAME_TYPE_MATCHES[name],
-            exchange=exchange, symbol=symbol,
-            interval=interval
-        )
-
-        for screener in screeners:
-            for index, row in data:
-                index = index_to_datetime(index)
-
-                if index not in screener.market.index:
-                    screener.market.loc[index] = row
-                # end if
-            # end for
-        # end for
-    # end handle
-
-    def screening_loop(self) -> None:
-        """Runs the process of the price screening."""
-    # end screening_loop
-
-    def start_screening(self) -> None:
-        """Starts the screening process."""
-
-        if self.screening:
-            warnings.warn(f"Timeout screening of {self} is already running.")
-
-            return
-        # end if
-
-        self._screening_process = threading.Thread(
-            target=lambda: self.screening_loop()
-        )
-
-        self._screening_process.start()
-    # end start_screening
-# end ScreenersDataCollector
+    return base_await_update(
+        *screeners, stop=stop, delay=delay,
+        cancel=cancel, gatherer=gather_screeners
+    )
+# end await_update
```

### Comparing `crypto-screening-7.5.5/crypto_screening/market/screeners/collectors/database.py` & `crypto-screening-7.5.6/crypto_screening/market/screeners/collectors/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,17 +109,19 @@
 
                     # noinspection PyTypeChecker
                     data: Data = list(
                         (index, row.to_dict())
                         for index, row in dataset.iterrows()
                     )
 
-                    self.handle(
-                        data=data, name=name, exchange=exchange,
-                        symbol=symbol, interval=interval
+                    self.collect(
+                        dict(
+                            data=data, name=name, exchange=exchange,
+                            symbol=symbol, interval=interval
+                        )
                     )
 
                 except Exception as e:
                     self.failed_tables.setdefault(table, []).append(e)
                 # end try
             # end for
         # end while
```

### Comparing `crypto-screening-7.5.5/crypto_screening/market/screeners/collectors/sockets.py` & `crypto-screening-7.5.6/crypto_screening/market/screeners/collectors/sockets.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,14 @@
 
         self.address = address
         self.port = port
 
         self.loop: Optional[asyncio.AbstractEventLoop] = None
 
         self.chunks: Dict[float, List[Dict[str, Any]]] = {}
-
         self.fail_record: Dict[str, List[Tuple[bytes, Exception]]] = {}
     # end __init__
 
     async def receive(
             self, reader: asyncio.StreamReader, writer: asyncio.StreamWriter
     ) -> None:
         """
@@ -113,32 +112,36 @@
                     if len(chunks) == payload[SocketCallback.CHUNKS]:
                         payload = json.loads(''.join(chunks[key]))
 
                         chunks.pop(key)
 
                         packet = payload[Callback.DATA]
 
-                        self.handle(
-                            name=payload[SocketCallback.KEY],
-                            data=packet[Callback.DATA],
-                            exchange=packet[Callback.EXCHANGE],
-                            symbol=packet[Callback.SYMBOL],
-                            interval=packet[Callback.INTERVAL]
+                        self.collect(
+                            dict(
+                                name=payload[SocketCallback.KEY],
+                                data=packet[Callback.DATA],
+                                exchange=packet[Callback.EXCHANGE],
+                                symbol=packet[Callback.SYMBOL],
+                                interval=packet[Callback.INTERVAL]
+                            )
                         )
                     # end if
 
                 else:
                     packet = payload[Callback.DATA]
 
-                    self.handle(
-                        name=payload[SocketCallback.KEY],
-                        data=packet[Callback.DATA],
-                        exchange=packet[Callback.EXCHANGE],
-                        symbol=packet[Callback.SYMBOL],
-                        interval=packet[Callback.INTERVAL]
+                    self.collect(
+                        dict(
+                            name=payload[SocketCallback.KEY],
+                            data=packet[Callback.DATA],
+                            exchange=packet[Callback.EXCHANGE],
+                            symbol=packet[Callback.SYMBOL],
+                            interval=packet[Callback.INTERVAL]
+                        )
                     )
                 # end for
             # end for
 
         except Exception as e:
             self.fail_record.setdefault(
                 writer.get_extra_info('peername'), []
```

### Comparing `crypto-screening-7.5.5/crypto_screening/market/screeners/combined.py` & `crypto-screening-7.5.6/crypto_screening/market/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/market/screeners/container.py` & `crypto-screening-7.5.6/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/market/screeners/database.py` & `crypto-screening-7.5.6/crypto_screening/market/screeners/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-7.5.6/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-7.5.6/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/market/screeners/orders.py` & `crypto-screening-7.5.6/crypto_screening/market/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/market/screeners/recorder.py` & `crypto-screening-7.5.6/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/market/screeners/trades.py` & `crypto-screening-7.5.6/crypto_screening/market/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/process.py` & `crypto-screening-7.5.6/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/source/data/all_exchanges_symbols.json` & `crypto-screening-7.5.6/crypto_screening/source/data/all_exchanges_symbols.json`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/symbols.py` & `crypto-screening-7.5.6/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening/validate.py` & `crypto-screening-7.5.6/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-7.5.6/crypto_screening.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 7.5.5
+Version: 7.5.6
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-7.5.5/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-7.5.6/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.5/pyproject.toml` & `crypto-screening-7.5.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '7.5.5'
+version = '7.5.6'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-7.5.5/setup.py` & `crypto-screening-7.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "crypto_screening/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='7.5.5',
+        version='7.5.6',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

