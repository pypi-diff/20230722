# Comparing `tmp/crypto-screening-7.5.0.tar.gz` & `tmp/crypto-screening-7.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-7.5.0.tar", last modified: Fri Jul 21 23:06:10 2023, max compression
+gzip compressed data, was "crypto-screening-7.5.1.tar", last modified: Fri Jul 21 23:15:45 2023, max compression
```

## Comparing `crypto-screening-7.5.0.tar` & `crypto-screening-7.5.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 23:06:10.167554 crypto-screening-7.5.0/
--rw-rw-rw-   0        0        0      196 2023-07-21 23:06:08.000000 crypto-screening-7.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-21 23:06:10.166554 crypto-screening-7.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-7.5.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-7.5.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:06:09.969439 crypto-screening-7.5.0/crypto_screening/
--rw-rw-rw-   0        0        0     1002 2023-07-21 10:49:22.000000 crypto-screening-7.5.0/crypto_screening/base.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:06:10.009010 crypto-screening-7.5.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-7.5.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-7.5.0/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:06:10.036014 crypto-screening-7.5.0/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-7.5.0/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-7.5.0/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-7.5.0/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-7.5.0/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:06:10.057980 crypto-screening-7.5.0/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-7.5.0/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24729 2023-07-20 08:01:55.000000 crypto-screening-7.5.0/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    16341 2023-07-21 10:15:56.000000 crypto-screening-7.5.0/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21717 2023-07-20 08:01:55.000000 crypto-screening-7.5.0/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-7.5.0/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    16799 2023-07-20 15:36:57.000000 crypto-screening-7.5.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19514 2023-07-21 10:12:10.000000 crypto-screening-7.5.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-7.5.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0     1007 2023-07-21 10:52:54.000000 crypto-screening-7.5.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-7.5.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:06:10.063010 crypto-screening-7.5.0/crypto_screening/market/
--rw-rw-rw-   0        0        0    18821 2023-07-21 23:02:29.000000 crypto-screening-7.5.0/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:06:10.085023 crypto-screening-7.5.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-7.5.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-7.5.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-7.5.0/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-7.5.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:06:10.145554 crypto-screening-7.5.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      519 2023-07-20 15:38:19.000000 crypto-screening-7.5.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    12013 2023-07-21 12:46:02.000000 crypto-screening-7.5.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    13798 2023-07-20 15:24:13.000000 crypto-screening-7.5.0/crypto_screening/market/screeners/callbacks.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:06:10.160584 crypto-screening-7.5.0/crypto_screening/market/screeners/collectors/
--rw-rw-rw-   0        0        0      217 2023-07-20 15:09:26.000000 crypto-screening-7.5.0/crypto_screening/market/screeners/collectors/__init__.py
--rw-rw-rw-   0        0        0     3630 2023-07-21 23:01:46.000000 crypto-screening-7.5.0/crypto_screening/market/screeners/collectors/base.py
--rw-rw-rw-   0        0        0     3988 2023-07-21 08:58:50.000000 crypto-screening-7.5.0/crypto_screening/market/screeners/collectors/database.py
--rw-rw-rw-   0        0        0     5952 2023-07-20 15:13:32.000000 crypto-screening-7.5.0/crypto_screening/market/screeners/collectors/sockets.py
--rw-rw-rw-   0        0        0    13450 2023-07-20 08:33:40.000000 crypto-screening-7.5.0/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    19042 2023-07-21 23:05:27.000000 crypto-screening-7.5.0/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    10983 2023-07-21 08:58:32.000000 crypto-screening-7.5.0/crypto_screening/market/screeners/database.py
--rw-rw-rw-   0        0        0    37526 2023-07-21 11:02:21.000000 crypto-screening-7.5.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    17713 2023-07-21 12:44:32.000000 crypto-screening-7.5.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    17240 2023-07-21 12:44:17.000000 crypto-screening-7.5.0/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    20611 2023-07-19 16:46:01.000000 crypto-screening-7.5.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0    17314 2023-07-21 12:44:28.000000 crypto-screening-7.5.0/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-7.5.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-7.5.0/crypto_screening/process.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:06:09.922486 crypto-screening-7.5.0/crypto_screening/source/
-drwxrwxrwx   0        0        0        0 2023-07-21 23:06:10.165586 crypto-screening-7.5.0/crypto_screening/source/data/
--rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-7.5.0/crypto_screening/source/data/all_exchanges_symbols.json
--rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-7.5.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-7.5.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-21 23:06:09.987446 crypto-screening-7.5.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-21 23:06:09.000000 crypto-screening-7.5.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2070 2023-07-21 23:06:09.000000 crypto-screening-7.5.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 23:06:09.000000 crypto-screening-7.5.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-21 23:06:09.000000 crypto-screening-7.5.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-21 23:06:09.000000 crypto-screening-7.5.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-21 23:06:08.000000 crypto-screening-7.5.0/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-7.5.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-7.5.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 23:06:10.167554 crypto-screening-7.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-07-21 23:05:57.000000 crypto-screening-7.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:15:45.006966 crypto-screening-7.5.1/
+-rw-rw-rw-   0        0        0      196 2023-07-21 23:15:44.000000 crypto-screening-7.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-21 23:15:45.006966 crypto-screening-7.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-7.5.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-7.5.1/build.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:15:44.965492 crypto-screening-7.5.1/crypto_screening/
+-rw-rw-rw-   0        0        0     1002 2023-07-21 10:49:22.000000 crypto-screening-7.5.1/crypto_screening/base.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:15:44.983520 crypto-screening-7.5.1/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-7.5.1/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-7.5.1/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:15:44.986992 crypto-screening-7.5.1/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-7.5.1/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-7.5.1/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-7.5.1/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-7.5.1/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:15:44.989987 crypto-screening-7.5.1/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-7.5.1/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24729 2023-07-20 08:01:55.000000 crypto-screening-7.5.1/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    16341 2023-07-21 10:15:56.000000 crypto-screening-7.5.1/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21717 2023-07-20 08:01:55.000000 crypto-screening-7.5.1/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-7.5.1/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    16799 2023-07-20 15:36:57.000000 crypto-screening-7.5.1/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19514 2023-07-21 10:12:10.000000 crypto-screening-7.5.1/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-7.5.1/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0     1007 2023-07-21 10:52:54.000000 crypto-screening-7.5.1/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-7.5.1/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:15:44.991966 crypto-screening-7.5.1/crypto_screening/market/
+-rw-rw-rw-   0        0        0    18821 2023-07-21 23:02:29.000000 crypto-screening-7.5.1/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:15:44.993967 crypto-screening-7.5.1/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-7.5.1/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-7.5.1/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-7.5.1/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-7.5.1/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:15:45.002966 crypto-screening-7.5.1/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      519 2023-07-20 15:38:19.000000 crypto-screening-7.5.1/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    12013 2023-07-21 12:46:02.000000 crypto-screening-7.5.1/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    13798 2023-07-20 15:24:13.000000 crypto-screening-7.5.1/crypto_screening/market/screeners/callbacks.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:15:45.004966 crypto-screening-7.5.1/crypto_screening/market/screeners/collectors/
+-rw-rw-rw-   0        0        0      217 2023-07-20 15:09:26.000000 crypto-screening-7.5.1/crypto_screening/market/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     3630 2023-07-21 23:01:46.000000 crypto-screening-7.5.1/crypto_screening/market/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     3988 2023-07-21 08:58:50.000000 crypto-screening-7.5.1/crypto_screening/market/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     5952 2023-07-20 15:13:32.000000 crypto-screening-7.5.1/crypto_screening/market/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    13450 2023-07-20 08:33:40.000000 crypto-screening-7.5.1/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    19304 2023-07-21 23:15:16.000000 crypto-screening-7.5.1/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    10983 2023-07-21 08:58:32.000000 crypto-screening-7.5.1/crypto_screening/market/screeners/database.py
+-rw-rw-rw-   0        0        0    37526 2023-07-21 11:02:21.000000 crypto-screening-7.5.1/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    17713 2023-07-21 12:44:32.000000 crypto-screening-7.5.1/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    17240 2023-07-21 12:44:17.000000 crypto-screening-7.5.1/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    20611 2023-07-19 16:46:01.000000 crypto-screening-7.5.1/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0    17314 2023-07-21 12:44:28.000000 crypto-screening-7.5.1/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-7.5.1/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-7.5.1/crypto_screening/process.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:15:44.953465 crypto-screening-7.5.1/crypto_screening/source/
+drwxrwxrwx   0        0        0        0 2023-07-21 23:15:45.005965 crypto-screening-7.5.1/crypto_screening/source/data/
+-rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-7.5.1/crypto_screening/source/data/all_exchanges_symbols.json
+-rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-7.5.1/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-7.5.1/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:15:44.979494 crypto-screening-7.5.1/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-21 23:15:44.000000 crypto-screening-7.5.1/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2070 2023-07-21 23:15:44.000000 crypto-screening-7.5.1/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 23:15:44.000000 crypto-screening-7.5.1/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-21 23:15:44.000000 crypto-screening-7.5.1/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-21 23:15:44.000000 crypto-screening-7.5.1/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-21 23:15:44.000000 crypto-screening-7.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-7.5.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-7.5.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 23:15:45.006966 crypto-screening-7.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-07-21 23:15:40.000000 crypto-screening-7.5.1/setup.py
```

### Comparing `crypto-screening-7.5.0/PKG-INFO` & `crypto-screening-7.5.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 7.5.0
+Version: 7.5.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-7.5.0/README.md` & `crypto-screening-7.5.1/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/build.py` & `crypto-screening-7.5.1/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/base.py` & `crypto-screening-7.5.1/crypto_screening/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/collect/assets.py` & `crypto-screening-7.5.1/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/collect/exchanges.py` & `crypto-screening-7.5.1/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-7.5.1/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/collect/market/orderbook.py` & `crypto-screening-7.5.1/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/collect/market/orders.py` & `crypto-screening-7.5.1/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/collect/market/state/assets.py` & `crypto-screening-7.5.1/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/collect/market/state/base.py` & `crypto-screening-7.5.1/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-7.5.1/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/collect/market/trades.py` & `crypto-screening-7.5.1/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/collect/screeners.py` & `crypto-screening-7.5.1/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/collect/symbols.py` & `crypto-screening-7.5.1/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/dataset.py` & `crypto-screening-7.5.1/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/exchanges.py` & `crypto-screening-7.5.1/crypto_screening/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/interval.py` & `crypto-screening-7.5.1/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/market/dynamic.py` & `crypto-screening-7.5.1/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/market/foundation/data.py` & `crypto-screening-7.5.1/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-7.5.1/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/market/foundation/state.py` & `crypto-screening-7.5.1/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-7.5.1/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/market/screeners/__init__.py` & `crypto-screening-7.5.1/crypto_screening/market/screeners/__init__.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/market/screeners/base.py` & `crypto-screening-7.5.1/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/market/screeners/callbacks.py` & `crypto-screening-7.5.1/crypto_screening/market/screeners/callbacks.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/market/screeners/collectors/base.py` & `crypto-screening-7.5.1/crypto_screening/market/screeners/collectors/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/market/screeners/collectors/database.py` & `crypto-screening-7.5.1/crypto_screening/market/screeners/collectors/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/market/screeners/collectors/sockets.py` & `crypto-screening-7.5.1/crypto_screening/market/screeners/collectors/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/market/screeners/combined.py` & `crypto-screening-7.5.1/crypto_screening/market/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/market/screeners/container.py` & `crypto-screening-7.5.1/crypto_screening/market/screeners/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,21 +240,23 @@
             if exchange is not None
         }
     # end structure
 
     def add(
             self,
             screeners: Iterable[BaseScreener],
-            adjust: Optional[bool] = True
+            adjust: Optional[bool] = True,
+            update: Optional[bool] = True
     ) -> None:
         """
         Updates the data with the new screeners.
 
         :param screeners: The new screeners to add.
         :param adjust: The value to adjust for screeners.
+        :param update: The value to update.
         """
 
         new_screeners = []
 
         for screener in screeners:
             if screener not in self._screeners:
                 new_screeners.append(screener)
@@ -267,27 +269,31 @@
             # end if
         # end for
 
         self._screeners.extend(new_screeners)
 
         screeners_table(new_screeners, table=self._table)
 
-        self.update()
+        if update:
+            self.update()
+        # end if
     # end update
 
     def remove(
             self,
             screeners: Iterable[BaseScreener],
-            adjust: Optional[bool] = True
+            adjust: Optional[bool] = True,
+            update: Optional[bool] = True
     ) -> None:
         """
         Updates the data with the new screeners.
 
         :param screeners: The new screeners to add.
         :param adjust: The value to adjust for screeners.
+        :param update: The value to update.
         """
 
         for screener in screeners:
             if screener in self._screeners:
                 self._screeners.remove(screener)
 
             elif not adjust:
@@ -298,15 +304,17 @@
             # end if
         # end for
 
         self._table.clear()
 
         screeners_table(self._screeners, table=self._table)
 
-        self.update()
+        if update:
+            self.update()
+        # end if
     # end remove
 
     def find_screeners(
             self,
             exchange: Optional[str] = None,
             symbol: Optional[str] = None,
             base: Optional[Type[_S]] = None,
```

### Comparing `crypto-screening-7.5.0/crypto_screening/market/screeners/database.py` & `crypto-screening-7.5.1/crypto_screening/market/screeners/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-7.5.1/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-7.5.1/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/market/screeners/orders.py` & `crypto-screening-7.5.1/crypto_screening/market/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-7.5.1/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/market/screeners/trades.py` & `crypto-screening-7.5.1/crypto_screening/market/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/market/waiting.py` & `crypto-screening-7.5.1/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/process.py` & `crypto-screening-7.5.1/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/source/data/all_exchanges_symbols.json` & `crypto-screening-7.5.1/crypto_screening/source/data/all_exchanges_symbols.json`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/symbols.py` & `crypto-screening-7.5.1/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening/validate.py` & `crypto-screening-7.5.1/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-7.5.1/crypto_screening.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 7.5.0
+Version: 7.5.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-7.5.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-7.5.1/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.0/pyproject.toml` & `crypto-screening-7.5.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '7.5.0'
+version = '7.5.1'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-7.5.0/setup.py` & `crypto-screening-7.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "crypto_screening/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='7.5.0',
+        version='7.5.1',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

