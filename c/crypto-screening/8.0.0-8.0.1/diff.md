# Comparing `tmp/crypto-screening-8.0.0.tar.gz` & `tmp/crypto-screening-8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-8.0.0.tar", last modified: Sat Jul 22 14:29:03 2023, max compression
+gzip compressed data, was "crypto-screening-8.0.1.tar", last modified: Sat Jul 22 14:34:03 2023, max compression
```

## Comparing `crypto-screening-8.0.0.tar` & `crypto-screening-8.0.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.450106 crypto-screening-8.0.0/
--rw-rw-rw-   0        0        0      196 2023-07-22 14:29:01.000000 crypto-screening-8.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-22 14:29:03.450106 crypto-screening-8.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.0.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.0.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.324298 crypto-screening-8.0.0/crypto_screening/
--rw-rw-rw-   0        0        0     1002 2023-07-21 10:49:22.000000 crypto-screening-8.0.0/crypto_screening/base.py
-drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.361270 crypto-screening-8.0.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-8.0.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-8.0.0/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.388298 crypto-screening-8.0.0/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-8.0.0/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-8.0.0/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-8.0.0/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-8.0.0/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.410295 crypto-screening-8.0.0/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-8.0.0/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24729 2023-07-20 08:01:55.000000 crypto-screening-8.0.0/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    16341 2023-07-21 10:15:56.000000 crypto-screening-8.0.0/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21717 2023-07-20 08:01:55.000000 crypto-screening-8.0.0/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-8.0.0/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    16799 2023-07-20 15:36:57.000000 crypto-screening-8.0.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19514 2023-07-21 10:12:10.000000 crypto-screening-8.0.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-8.0.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0     1007 2023-07-21 10:52:54.000000 crypto-screening-8.0.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-8.0.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.416298 crypto-screening-8.0.0/crypto_screening/market/
--rw-rw-rw-   0        0        0    15126 2023-07-22 11:30:19.000000 crypto-screening-8.0.0/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.427097 crypto-screening-8.0.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10429 2023-07-22 11:56:59.000000 crypto-screening-8.0.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.0.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-8.0.0/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-8.0.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.440105 crypto-screening-8.0.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      519 2023-07-20 15:38:19.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    23442 2023-07-22 14:11:45.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    13798 2023-07-22 14:15:26.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/callbacks.py
-drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.448105 crypto-screening-8.0.0/crypto_screening/market/screeners/collectors/
--rw-rw-rw-   0        0        0      217 2023-07-20 15:09:26.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/collectors/__init__.py
--rw-rw-rw-   0        0        0     6285 2023-07-22 14:19:31.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/collectors/base.py
--rw-rw-rw-   0        0        0     4055 2023-07-22 09:26:50.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/collectors/database.py
--rw-rw-rw-   0        0        0     6116 2023-07-22 09:26:50.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/collectors/sockets.py
--rw-rw-rw-   0        0        0    12295 2023-07-22 14:13:24.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    10848 2023-07-22 14:02:39.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    10983 2023-07-21 08:58:32.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/database.py
--rw-rw-rw-   0        0        0    22098 2023-07-22 14:27:51.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    11807 2023-07-22 14:28:12.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    11409 2023-07-22 14:28:12.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    16923 2023-07-22 14:27:51.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0    11488 2023-07-22 14:28:12.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-8.0.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-8.0.0/crypto_screening/process.py
-drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.282271 crypto-screening-8.0.0/crypto_screening/source/
-drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.449105 crypto-screening-8.0.0/crypto_screening/source/data/
--rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.0.0/crypto_screening/source/data/all_exchanges_symbols.json
--rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-8.0.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-8.0.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.338299 crypto-screening-8.0.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-22 14:29:03.000000 crypto-screening-8.0.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2070 2023-07-22 14:29:03.000000 crypto-screening-8.0.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 14:29:03.000000 crypto-screening-8.0.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-22 14:29:03.000000 crypto-screening-8.0.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-22 14:29:03.000000 crypto-screening-8.0.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-22 14:29:01.000000 crypto-screening-8.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.0.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-22 14:29:03.450106 crypto-screening-8.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-07-22 14:28:58.000000 crypto-screening-8.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:34:03.541463 crypto-screening-8.0.1/
+-rw-rw-rw-   0        0        0      196 2023-07-22 14:34:03.000000 crypto-screening-8.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-22 14:34:03.541463 crypto-screening-8.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.0.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.0.1/build.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:34:03.497429 crypto-screening-8.0.1/crypto_screening/
+-rw-rw-rw-   0        0        0     1002 2023-07-21 10:49:22.000000 crypto-screening-8.0.1/crypto_screening/base.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:34:03.518463 crypto-screening-8.0.1/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-8.0.1/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-8.0.1/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:34:03.522459 crypto-screening-8.0.1/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-8.0.1/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-8.0.1/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-8.0.1/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-8.0.1/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:34:03.525455 crypto-screening-8.0.1/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-8.0.1/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24729 2023-07-20 08:01:55.000000 crypto-screening-8.0.1/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    16341 2023-07-21 10:15:56.000000 crypto-screening-8.0.1/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21717 2023-07-20 08:01:55.000000 crypto-screening-8.0.1/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-8.0.1/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    16799 2023-07-20 15:36:57.000000 crypto-screening-8.0.1/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19514 2023-07-21 10:12:10.000000 crypto-screening-8.0.1/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-8.0.1/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0     1007 2023-07-21 10:52:54.000000 crypto-screening-8.0.1/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-8.0.1/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:34:03.527429 crypto-screening-8.0.1/crypto_screening/market/
+-rw-rw-rw-   0        0        0    15126 2023-07-22 11:30:19.000000 crypto-screening-8.0.1/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:34:03.530460 crypto-screening-8.0.1/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10459 2023-07-22 14:33:35.000000 crypto-screening-8.0.1/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.0.1/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-8.0.1/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-8.0.1/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:34:03.537459 crypto-screening-8.0.1/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      519 2023-07-20 15:38:19.000000 crypto-screening-8.0.1/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    23442 2023-07-22 14:11:45.000000 crypto-screening-8.0.1/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    13798 2023-07-22 14:15:26.000000 crypto-screening-8.0.1/crypto_screening/market/screeners/callbacks.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:34:03.539462 crypto-screening-8.0.1/crypto_screening/market/screeners/collectors/
+-rw-rw-rw-   0        0        0      217 2023-07-20 15:09:26.000000 crypto-screening-8.0.1/crypto_screening/market/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     6285 2023-07-22 14:19:31.000000 crypto-screening-8.0.1/crypto_screening/market/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     4055 2023-07-22 09:26:50.000000 crypto-screening-8.0.1/crypto_screening/market/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     6116 2023-07-22 09:26:50.000000 crypto-screening-8.0.1/crypto_screening/market/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    12295 2023-07-22 14:13:24.000000 crypto-screening-8.0.1/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    10848 2023-07-22 14:02:39.000000 crypto-screening-8.0.1/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    10983 2023-07-21 08:58:32.000000 crypto-screening-8.0.1/crypto_screening/market/screeners/database.py
+-rw-rw-rw-   0        0        0    22098 2023-07-22 14:27:51.000000 crypto-screening-8.0.1/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    11807 2023-07-22 14:28:12.000000 crypto-screening-8.0.1/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    11409 2023-07-22 14:28:12.000000 crypto-screening-8.0.1/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    16923 2023-07-22 14:27:51.000000 crypto-screening-8.0.1/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0    11488 2023-07-22 14:28:12.000000 crypto-screening-8.0.1/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-8.0.1/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-8.0.1/crypto_screening/process.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:34:03.488457 crypto-screening-8.0.1/crypto_screening/source/
+drwxrwxrwx   0        0        0        0 2023-07-22 14:34:03.540460 crypto-screening-8.0.1/crypto_screening/source/data/
+-rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.0.1/crypto_screening/source/data/all_exchanges_symbols.json
+-rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-8.0.1/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-8.0.1/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:34:03.515460 crypto-screening-8.0.1/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-22 14:34:03.000000 crypto-screening-8.0.1/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2070 2023-07-22 14:34:03.000000 crypto-screening-8.0.1/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 14:34:03.000000 crypto-screening-8.0.1/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-22 14:34:03.000000 crypto-screening-8.0.1/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-22 14:34:03.000000 crypto-screening-8.0.1/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-22 14:34:03.000000 crypto-screening-8.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.0.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-22 14:34:03.542459 crypto-screening-8.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-07-22 14:34:00.000000 crypto-screening-8.0.1/setup.py
```

### Comparing `crypto-screening-8.0.0/PKG-INFO` & `crypto-screening-8.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.0.0
+Version: 8.0.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.0.0/README.md` & `crypto-screening-8.0.1/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/build.py` & `crypto-screening-8.0.1/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/base.py` & `crypto-screening-8.0.1/crypto_screening/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/collect/assets.py` & `crypto-screening-8.0.1/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/collect/exchanges.py` & `crypto-screening-8.0.1/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-8.0.1/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/collect/market/orderbook.py` & `crypto-screening-8.0.1/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/collect/market/orders.py` & `crypto-screening-8.0.1/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/collect/market/state/assets.py` & `crypto-screening-8.0.1/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/collect/market/state/base.py` & `crypto-screening-8.0.1/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-8.0.1/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/collect/market/trades.py` & `crypto-screening-8.0.1/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/collect/screeners.py` & `crypto-screening-8.0.1/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/collect/symbols.py` & `crypto-screening-8.0.1/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/dataset.py` & `crypto-screening-8.0.1/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/exchanges.py` & `crypto-screening-8.0.1/crypto_screening/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/interval.py` & `crypto-screening-8.0.1/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/market/dynamic.py` & `crypto-screening-8.0.1/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/market/foundation/data.py` & `crypto-screening-8.0.1/crypto_screening/market/foundation/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -173,29 +173,29 @@
         """
     # end base_wait_for_update
 
     def start_blocking(self) -> None:
         """Starts the blocking process."""
 
         if self.saving:
-            warnings.warn(f"Blocking process of {self} is already running.")
+            warnings.warn(f"Blocking process of {repr(self)} is already running.")
         # end if
 
         self._blocking = True
 
         while self.blocking:
             time.sleep(0.005)
         # end while
     # end start_blocking
 
     def start_screening(self) -> None:
         """Starts the screening process."""
 
         if self.screening:
-            warnings.warn(f"Screening process of {self} is already running.")
+            warnings.warn(f"Screening process of {repr(self)} is already running.")
 
             return
         # end if
 
         self._screening = True
 
         self._screening_process = threading.Thread(
@@ -205,15 +205,15 @@
         self._screening_process.start()
     # end start_screening
 
     def start_saving(self) -> None:
         """Starts the saving process."""
 
         if self.saving:
-            warnings.warn(f"Saving process of {self} is already running.")
+            warnings.warn(f"Saving process of {repr(self)} is already running.")
         # end if
 
         self._saving = True
 
         self._saving_process = threading.Thread(
             target=self.saving_loop
         )
@@ -221,15 +221,15 @@
         self._saving_process.start()
     # end start_saving
 
     def start_updating(self) -> None:
         """Starts the updating process."""
 
         if self.updating:
-            warnings.warn(f"Updating process of {self} is already running.")
+            warnings.warn(f"Updating process of {repr(self)} is already running.")
         # end if
 
         self._updating = True
 
         self._update_process = threading.Thread(
             target=self.update_loop
         )
@@ -275,15 +275,15 @@
         :return: The start_timeout process.
         """
 
         if (
             isinstance(self._timeout_process, threading.Thread) and
             self._timeout_process.is_alive()
         ):
-            warnings.warn(f"Timeout process of {self} is already running.")
+            warnings.warn(f"Timeout process of {repr(self)} is already running.")
 
             return
         # end if
 
         if isinstance(duration, dt.datetime):
             duration = duration - dt.datetime.now()
         # end if
```

### Comparing `crypto-screening-8.0.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-8.0.1/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/market/foundation/state.py` & `crypto-screening-8.0.1/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-8.0.1/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/market/screeners/__init__.py` & `crypto-screening-8.0.1/crypto_screening/market/screeners/__init__.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/market/screeners/base.py` & `crypto-screening-8.0.1/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/market/screeners/callbacks.py` & `crypto-screening-8.0.1/crypto_screening/market/screeners/callbacks.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/market/screeners/collectors/base.py` & `crypto-screening-8.0.1/crypto_screening/market/screeners/collectors/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/market/screeners/collectors/database.py` & `crypto-screening-8.0.1/crypto_screening/market/screeners/collectors/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/market/screeners/collectors/sockets.py` & `crypto-screening-8.0.1/crypto_screening/market/screeners/collectors/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/market/screeners/combined.py` & `crypto-screening-8.0.1/crypto_screening/market/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/market/screeners/container.py` & `crypto-screening-8.0.1/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/market/screeners/database.py` & `crypto-screening-8.0.1/crypto_screening/market/screeners/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-8.0.1/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-8.0.1/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/market/screeners/orders.py` & `crypto-screening-8.0.1/crypto_screening/market/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-8.0.1/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/market/screeners/trades.py` & `crypto-screening-8.0.1/crypto_screening/market/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/market/waiting.py` & `crypto-screening-8.0.1/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/process.py` & `crypto-screening-8.0.1/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/source/data/all_exchanges_symbols.json` & `crypto-screening-8.0.1/crypto_screening/source/data/all_exchanges_symbols.json`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/symbols.py` & `crypto-screening-8.0.1/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening/validate.py` & `crypto-screening-8.0.1/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-8.0.1/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.0.0
+Version: 8.0.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.0.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-8.0.1/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.0.0/pyproject.toml` & `crypto-screening-8.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '8.0.0'
+version = '8.0.1'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-8.0.0/setup.py` & `crypto-screening-8.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "crypto_screening/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='8.0.0',
+        version='8.0.1',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

