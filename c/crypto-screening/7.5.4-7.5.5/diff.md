# Comparing `tmp/crypto-screening-7.5.4.tar.gz` & `tmp/crypto-screening-7.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-7.5.4.tar", last modified: Fri Jul 21 23:37:56 2023, max compression
+gzip compressed data, was "crypto-screening-7.5.5.tar", last modified: Fri Jul 21 23:40:08 2023, max compression
```

## Comparing `crypto-screening-7.5.4.tar` & `crypto-screening-7.5.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 23:37:56.352705 crypto-screening-7.5.4/
--rw-rw-rw-   0        0        0      196 2023-07-21 23:37:56.000000 crypto-screening-7.5.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-21 23:37:56.352705 crypto-screening-7.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-7.5.4/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-7.5.4/build.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:37:56.313706 crypto-screening-7.5.4/crypto_screening/
--rw-rw-rw-   0        0        0     1002 2023-07-21 10:49:22.000000 crypto-screening-7.5.4/crypto_screening/base.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:37:56.328707 crypto-screening-7.5.4/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-7.5.4/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-7.5.4/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:37:56.332705 crypto-screening-7.5.4/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-7.5.4/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-7.5.4/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-7.5.4/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-7.5.4/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:37:56.335722 crypto-screening-7.5.4/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-7.5.4/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24729 2023-07-20 08:01:55.000000 crypto-screening-7.5.4/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    16341 2023-07-21 10:15:56.000000 crypto-screening-7.5.4/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21717 2023-07-20 08:01:55.000000 crypto-screening-7.5.4/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-7.5.4/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    16799 2023-07-20 15:36:57.000000 crypto-screening-7.5.4/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19514 2023-07-21 10:12:10.000000 crypto-screening-7.5.4/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-7.5.4/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0     1007 2023-07-21 10:52:54.000000 crypto-screening-7.5.4/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-7.5.4/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:37:56.337706 crypto-screening-7.5.4/crypto_screening/market/
--rw-rw-rw-   0        0        0    14501 2023-07-21 23:37:45.000000 crypto-screening-7.5.4/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:37:56.340706 crypto-screening-7.5.4/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-7.5.4/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-7.5.4/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-7.5.4/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-7.5.4/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:37:56.347707 crypto-screening-7.5.4/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      519 2023-07-20 15:38:19.000000 crypto-screening-7.5.4/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    15448 2023-07-21 23:25:16.000000 crypto-screening-7.5.4/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    13798 2023-07-20 15:24:13.000000 crypto-screening-7.5.4/crypto_screening/market/screeners/callbacks.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:37:56.350707 crypto-screening-7.5.4/crypto_screening/market/screeners/collectors/
--rw-rw-rw-   0        0        0      217 2023-07-20 15:09:26.000000 crypto-screening-7.5.4/crypto_screening/market/screeners/collectors/__init__.py
--rw-rw-rw-   0        0        0     3602 2023-07-21 23:25:16.000000 crypto-screening-7.5.4/crypto_screening/market/screeners/collectors/base.py
--rw-rw-rw-   0        0        0     3988 2023-07-21 08:58:50.000000 crypto-screening-7.5.4/crypto_screening/market/screeners/collectors/database.py
--rw-rw-rw-   0        0        0     5952 2023-07-20 15:13:32.000000 crypto-screening-7.5.4/crypto_screening/market/screeners/collectors/sockets.py
--rw-rw-rw-   0        0        0    13450 2023-07-20 08:33:40.000000 crypto-screening-7.5.4/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    20177 2023-07-21 23:36:03.000000 crypto-screening-7.5.4/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    10983 2023-07-21 08:58:32.000000 crypto-screening-7.5.4/crypto_screening/market/screeners/database.py
--rw-rw-rw-   0        0        0    37526 2023-07-21 11:02:21.000000 crypto-screening-7.5.4/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    17713 2023-07-21 12:44:32.000000 crypto-screening-7.5.4/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    17240 2023-07-21 12:44:17.000000 crypto-screening-7.5.4/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    20611 2023-07-19 16:46:01.000000 crypto-screening-7.5.4/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0    17314 2023-07-21 12:44:28.000000 crypto-screening-7.5.4/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-7.5.4/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-7.5.4/crypto_screening/process.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:37:56.303692 crypto-screening-7.5.4/crypto_screening/source/
-drwxrwxrwx   0        0        0        0 2023-07-21 23:37:56.350707 crypto-screening-7.5.4/crypto_screening/source/data/
--rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-7.5.4/crypto_screening/source/data/all_exchanges_symbols.json
--rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-7.5.4/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-7.5.4/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:37:56.325714 crypto-screening-7.5.4/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-21 23:37:56.000000 crypto-screening-7.5.4/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2070 2023-07-21 23:37:56.000000 crypto-screening-7.5.4/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 23:37:56.000000 crypto-screening-7.5.4/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-21 23:37:56.000000 crypto-screening-7.5.4/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-21 23:37:56.000000 crypto-screening-7.5.4/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-21 23:37:56.000000 crypto-screening-7.5.4/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-7.5.4/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-7.5.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 23:37:56.352705 crypto-screening-7.5.4/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-07-21 23:37:53.000000 crypto-screening-7.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:40:08.023061 crypto-screening-7.5.5/
+-rw-rw-rw-   0        0        0      196 2023-07-21 23:40:07.000000 crypto-screening-7.5.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-21 23:40:08.023061 crypto-screening-7.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-7.5.5/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-7.5.5/build.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:40:07.985057 crypto-screening-7.5.5/crypto_screening/
+-rw-rw-rw-   0        0        0     1002 2023-07-21 10:49:22.000000 crypto-screening-7.5.5/crypto_screening/base.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:40:08.001057 crypto-screening-7.5.5/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-7.5.5/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-7.5.5/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:40:08.005057 crypto-screening-7.5.5/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-7.5.5/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-7.5.5/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-7.5.5/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-7.5.5/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:40:08.007057 crypto-screening-7.5.5/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-7.5.5/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24729 2023-07-20 08:01:55.000000 crypto-screening-7.5.5/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    16341 2023-07-21 10:15:56.000000 crypto-screening-7.5.5/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21717 2023-07-20 08:01:55.000000 crypto-screening-7.5.5/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-7.5.5/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    16799 2023-07-20 15:36:57.000000 crypto-screening-7.5.5/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19514 2023-07-21 10:12:10.000000 crypto-screening-7.5.5/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-7.5.5/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0     1007 2023-07-21 10:52:54.000000 crypto-screening-7.5.5/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-7.5.5/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:40:08.009057 crypto-screening-7.5.5/crypto_screening/market/
+-rw-rw-rw-   0        0        0    14279 2023-07-21 23:39:53.000000 crypto-screening-7.5.5/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:40:08.011057 crypto-screening-7.5.5/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-7.5.5/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-7.5.5/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-7.5.5/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-7.5.5/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:40:08.019057 crypto-screening-7.5.5/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      519 2023-07-20 15:38:19.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    15448 2023-07-21 23:25:16.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    13798 2023-07-20 15:24:13.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/callbacks.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:40:08.021057 crypto-screening-7.5.5/crypto_screening/market/screeners/collectors/
+-rw-rw-rw-   0        0        0      217 2023-07-20 15:09:26.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     3602 2023-07-21 23:25:16.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     3988 2023-07-21 08:58:50.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     5952 2023-07-20 15:13:32.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    13450 2023-07-20 08:33:40.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    20177 2023-07-21 23:36:03.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    10983 2023-07-21 08:58:32.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/database.py
+-rw-rw-rw-   0        0        0    37526 2023-07-21 11:02:21.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    17713 2023-07-21 12:44:32.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    17240 2023-07-21 12:44:17.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    20611 2023-07-19 16:46:01.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0    17314 2023-07-21 12:44:28.000000 crypto-screening-7.5.5/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-7.5.5/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-7.5.5/crypto_screening/process.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:40:07.975476 crypto-screening-7.5.5/crypto_screening/source/
+drwxrwxrwx   0        0        0        0 2023-07-21 23:40:08.022057 crypto-screening-7.5.5/crypto_screening/source/data/
+-rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-7.5.5/crypto_screening/source/data/all_exchanges_symbols.json
+-rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-7.5.5/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-7.5.5/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:40:07.998057 crypto-screening-7.5.5/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-21 23:40:07.000000 crypto-screening-7.5.5/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2070 2023-07-21 23:40:07.000000 crypto-screening-7.5.5/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 23:40:07.000000 crypto-screening-7.5.5/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-21 23:40:07.000000 crypto-screening-7.5.5/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-21 23:40:07.000000 crypto-screening-7.5.5/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-21 23:40:07.000000 crypto-screening-7.5.5/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-7.5.5/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-7.5.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 23:40:08.024061 crypto-screening-7.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-07-21 23:40:01.000000 crypto-screening-7.5.5/setup.py
```

### Comparing `crypto-screening-7.5.4/PKG-INFO` & `crypto-screening-7.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 7.5.4
+Version: 7.5.5
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-7.5.4/README.md` & `crypto-screening-7.5.5/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/build.py` & `crypto-screening-7.5.5/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/base.py` & `crypto-screening-7.5.5/crypto_screening/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/collect/assets.py` & `crypto-screening-7.5.5/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/collect/exchanges.py` & `crypto-screening-7.5.5/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-7.5.5/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/collect/market/orderbook.py` & `crypto-screening-7.5.5/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/collect/market/orders.py` & `crypto-screening-7.5.5/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/collect/market/state/assets.py` & `crypto-screening-7.5.5/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/collect/market/state/base.py` & `crypto-screening-7.5.5/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-7.5.5/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/collect/market/trades.py` & `crypto-screening-7.5.5/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/collect/screeners.py` & `crypto-screening-7.5.5/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/collect/symbols.py` & `crypto-screening-7.5.5/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/dataset.py` & `crypto-screening-7.5.5/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/exchanges.py` & `crypto-screening-7.5.5/crypto_screening/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/interval.py` & `crypto-screening-7.5.5/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/market/dynamic.py` & `crypto-screening-7.5.5/crypto_screening/market/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,20 +71,16 @@
         :param separator: The separator of the assets.
         :param included: The symbols to include.
         :param bases: The bases of the asset pairs.
 
         :return: The values of the assets.
         """
 
-        screeners = []
-        screeners.extend(self.orderbook_screeners)
-        screeners.extend(self.ohlcv_screeners)
-
         screeners = exchanges_symbols_screeners(
-            screeners=screeners, exchanges=exchanges,
+            screeners=self.orderbook_screeners, exchanges=exchanges,
             separator=separator, bases=bases, quotes=quotes,
             included=included, excluded=excluded, adjust=adjust
         )
 
         return assets_orderbook_market_state(
             screeners=screeners, separator=separator,
             length=length, adjust=adjust
@@ -114,20 +110,16 @@
         :param separator: The separator of the assets.
         :param included: The symbols to include.
         :param bases: The bases of the asset pairs.
 
         :return: The values of the assets.
         """
 
-        screeners = []
-        screeners.extend(self.orderbook_screeners)
-        screeners.extend(self.ohlcv_screeners)
-
         screeners = exchanges_symbols_screeners(
-            screeners=screeners, exchanges=exchanges,
+            screeners=self.orderbook_screeners, exchanges=exchanges,
             separator=separator, bases=bases, quotes=quotes,
             included=included, excluded=excluded, adjust=adjust
         )
 
         return symbols_orderbook_market_state(
             screeners=screeners, length=length, adjust=adjust
         )
```

### Comparing `crypto-screening-7.5.4/crypto_screening/market/foundation/data.py` & `crypto-screening-7.5.5/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/market/foundation/protocols.py` & `crypto-screening-7.5.5/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/market/foundation/state.py` & `crypto-screening-7.5.5/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/market/foundation/waiting.py` & `crypto-screening-7.5.5/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/market/screeners/__init__.py` & `crypto-screening-7.5.5/crypto_screening/market/screeners/__init__.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/market/screeners/base.py` & `crypto-screening-7.5.5/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/market/screeners/callbacks.py` & `crypto-screening-7.5.5/crypto_screening/market/screeners/callbacks.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/market/screeners/collectors/base.py` & `crypto-screening-7.5.5/crypto_screening/market/screeners/collectors/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/market/screeners/collectors/database.py` & `crypto-screening-7.5.5/crypto_screening/market/screeners/collectors/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/market/screeners/collectors/sockets.py` & `crypto-screening-7.5.5/crypto_screening/market/screeners/collectors/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/market/screeners/combined.py` & `crypto-screening-7.5.5/crypto_screening/market/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/market/screeners/container.py` & `crypto-screening-7.5.5/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/market/screeners/database.py` & `crypto-screening-7.5.5/crypto_screening/market/screeners/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-7.5.5/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-7.5.5/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/market/screeners/orders.py` & `crypto-screening-7.5.5/crypto_screening/market/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/market/screeners/recorder.py` & `crypto-screening-7.5.5/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/market/screeners/trades.py` & `crypto-screening-7.5.5/crypto_screening/market/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/market/waiting.py` & `crypto-screening-7.5.5/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/process.py` & `crypto-screening-7.5.5/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/source/data/all_exchanges_symbols.json` & `crypto-screening-7.5.5/crypto_screening/source/data/all_exchanges_symbols.json`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/symbols.py` & `crypto-screening-7.5.5/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening/validate.py` & `crypto-screening-7.5.5/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-7.5.5/crypto_screening.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 7.5.4
+Version: 7.5.5
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-7.5.4/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-7.5.5/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.4/pyproject.toml` & `crypto-screening-7.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '7.5.4'
+version = '7.5.5'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-7.5.4/setup.py` & `crypto-screening-7.5.5/setup.py`

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
-        version='7.5.4',
+        version='7.5.5',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

