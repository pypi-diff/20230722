# Comparing `tmp/crypto-screening-7.5.6.tar.gz` & `tmp/crypto-screening-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-7.5.6.tar", last modified: Sat Jul 22 09:34:07 2023, max compression
+gzip compressed data, was "crypto-screening-8.0.0.tar", last modified: Sat Jul 22 14:29:03 2023, max compression
```

## Comparing `crypto-screening-7.5.6.tar` & `crypto-screening-8.0.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.189436 crypto-screening-7.5.6/
--rw-rw-rw-   0        0        0      196 2023-07-22 09:34:06.000000 crypto-screening-7.5.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-22 09:34:07.189436 crypto-screening-7.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-7.5.6/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-7.5.6/build.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.011671 crypto-screening-7.5.6/crypto_screening/
--rw-rw-rw-   0        0        0     1002 2023-07-21 10:49:22.000000 crypto-screening-7.5.6/crypto_screening/base.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.049275 crypto-screening-7.5.6/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-7.5.6/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-7.5.6/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.079244 crypto-screening-7.5.6/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-7.5.6/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-7.5.6/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-7.5.6/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-7.5.6/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.101723 crypto-screening-7.5.6/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-7.5.6/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24729 2023-07-20 08:01:55.000000 crypto-screening-7.5.6/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    16341 2023-07-21 10:15:56.000000 crypto-screening-7.5.6/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21717 2023-07-20 08:01:55.000000 crypto-screening-7.5.6/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-7.5.6/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    16799 2023-07-20 15:36:57.000000 crypto-screening-7.5.6/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19514 2023-07-21 10:12:10.000000 crypto-screening-7.5.6/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-7.5.6/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0     1007 2023-07-21 10:52:54.000000 crypto-screening-7.5.6/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-7.5.6/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.112767 crypto-screening-7.5.6/crypto_screening/market/
--rw-rw-rw-   0        0        0    14279 2023-07-21 23:39:53.000000 crypto-screening-7.5.6/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.136276 crypto-screening-7.5.6/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10654 2023-07-18 21:40:34.000000 crypto-screening-7.5.6/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-7.5.6/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-7.5.6/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-7.5.6/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.181438 crypto-screening-7.5.6/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      519 2023-07-20 15:38:19.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    15448 2023-07-21 23:25:16.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    13798 2023-07-20 15:24:13.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/callbacks.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.187437 crypto-screening-7.5.6/crypto_screening/market/screeners/collectors/
--rw-rw-rw-   0        0        0      217 2023-07-20 15:09:26.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/collectors/__init__.py
--rw-rw-rw-   0        0        0     6340 2023-07-22 09:28:50.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/collectors/base.py
--rw-rw-rw-   0        0        0     4055 2023-07-22 09:26:50.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/collectors/database.py
--rw-rw-rw-   0        0        0     6116 2023-07-22 09:26:50.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/collectors/sockets.py
--rw-rw-rw-   0        0        0    13450 2023-07-20 08:33:40.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    20177 2023-07-21 23:36:03.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    10983 2023-07-21 08:58:32.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/database.py
--rw-rw-rw-   0        0        0    37526 2023-07-21 11:02:21.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    17713 2023-07-21 12:44:32.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    17240 2023-07-21 12:44:17.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    20611 2023-07-19 16:46:01.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0    17314 2023-07-21 12:44:28.000000 crypto-screening-7.5.6/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-7.5.6/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-7.5.6/crypto_screening/process.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:34:06.968784 crypto-screening-7.5.6/crypto_screening/source/
-drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.188437 crypto-screening-7.5.6/crypto_screening/source/data/
--rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-7.5.6/crypto_screening/source/data/all_exchanges_symbols.json
--rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-7.5.6/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-7.5.6/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:34:07.025706 crypto-screening-7.5.6/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-22 09:34:06.000000 crypto-screening-7.5.6/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2070 2023-07-22 09:34:06.000000 crypto-screening-7.5.6/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 09:34:06.000000 crypto-screening-7.5.6/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-22 09:34:06.000000 crypto-screening-7.5.6/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-22 09:34:06.000000 crypto-screening-7.5.6/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-22 09:34:06.000000 crypto-screening-7.5.6/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-7.5.6/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-7.5.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-22 09:34:07.189436 crypto-screening-7.5.6/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-07-22 09:33:58.000000 crypto-screening-7.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.450106 crypto-screening-8.0.0/
+-rw-rw-rw-   0        0        0      196 2023-07-22 14:29:01.000000 crypto-screening-8.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-22 14:29:03.450106 crypto-screening-8.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.0.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.0.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.324298 crypto-screening-8.0.0/crypto_screening/
+-rw-rw-rw-   0        0        0     1002 2023-07-21 10:49:22.000000 crypto-screening-8.0.0/crypto_screening/base.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.361270 crypto-screening-8.0.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-8.0.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-8.0.0/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.388298 crypto-screening-8.0.0/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      235 2023-07-16 14:00:25.000000 crypto-screening-8.0.0/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19623 2023-07-18 21:23:44.000000 crypto-screening-8.0.0/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17275 2023-07-17 09:43:58.000000 crypto-screening-8.0.0/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12533 2023-07-18 21:21:45.000000 crypto-screening-8.0.0/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.410295 crypto-screening-8.0.0/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      194 2023-07-16 14:00:21.000000 crypto-screening-8.0.0/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24729 2023-07-20 08:01:55.000000 crypto-screening-8.0.0/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    16341 2023-07-21 10:15:56.000000 crypto-screening-8.0.0/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21717 2023-07-20 08:01:55.000000 crypto-screening-8.0.0/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15133 2023-07-18 21:21:06.000000 crypto-screening-8.0.0/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    16799 2023-07-20 15:36:57.000000 crypto-screening-8.0.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19514 2023-07-21 10:12:10.000000 crypto-screening-8.0.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-8.0.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0     1007 2023-07-21 10:52:54.000000 crypto-screening-8.0.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-8.0.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.416298 crypto-screening-8.0.0/crypto_screening/market/
+-rw-rw-rw-   0        0        0    15126 2023-07-22 11:30:19.000000 crypto-screening-8.0.0/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.427097 crypto-screening-8.0.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10429 2023-07-22 11:56:59.000000 crypto-screening-8.0.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.0.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1200 2023-07-18 21:52:07.000000 crypto-screening-8.0.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6957 2023-07-18 21:40:34.000000 crypto-screening-8.0.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.440105 crypto-screening-8.0.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      519 2023-07-20 15:38:19.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    23442 2023-07-22 14:11:45.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    13798 2023-07-22 14:15:26.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/callbacks.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.448105 crypto-screening-8.0.0/crypto_screening/market/screeners/collectors/
+-rw-rw-rw-   0        0        0      217 2023-07-20 15:09:26.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     6285 2023-07-22 14:19:31.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     4055 2023-07-22 09:26:50.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     6116 2023-07-22 09:26:50.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    12295 2023-07-22 14:13:24.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    10848 2023-07-22 14:02:39.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    10983 2023-07-21 08:58:32.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/database.py
+-rw-rw-rw-   0        0        0    22098 2023-07-22 14:27:51.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    11807 2023-07-22 14:28:12.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    11409 2023-07-22 14:28:12.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    16923 2023-07-22 14:27:51.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0    11488 2023-07-22 14:28:12.000000 crypto-screening-8.0.0/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3832 2023-07-18 21:42:09.000000 crypto-screening-8.0.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-8.0.0/crypto_screening/process.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.282271 crypto-screening-8.0.0/crypto_screening/source/
+drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.449105 crypto-screening-8.0.0/crypto_screening/source/data/
+-rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.0.0/crypto_screening/source/data/all_exchanges_symbols.json
+-rw-rw-rw-   0        0        0    10361 2023-07-18 17:06:38.000000 crypto-screening-8.0.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3599 2023-07-18 22:07:23.000000 crypto-screening-8.0.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-22 14:29:03.338299 crypto-screening-8.0.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-22 14:29:03.000000 crypto-screening-8.0.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2070 2023-07-22 14:29:03.000000 crypto-screening-8.0.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 14:29:03.000000 crypto-screening-8.0.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-22 14:29:03.000000 crypto-screening-8.0.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-22 14:29:03.000000 crypto-screening-8.0.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-22 14:29:01.000000 crypto-screening-8.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.0.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-22 14:29:03.450106 crypto-screening-8.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-07-22 14:28:58.000000 crypto-screening-8.0.0/setup.py
```

### Comparing `crypto-screening-7.5.6/PKG-INFO` & `crypto-screening-8.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 7.5.6
+Version: 8.0.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-7.5.6/README.md` & `crypto-screening-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/build.py` & `crypto-screening-8.0.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/base.py` & `crypto-screening-8.0.0/crypto_screening/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/collect/assets.py` & `crypto-screening-8.0.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/collect/exchanges.py` & `crypto-screening-8.0.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-8.0.0/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/collect/market/orderbook.py` & `crypto-screening-8.0.0/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/collect/market/orders.py` & `crypto-screening-8.0.0/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/collect/market/state/assets.py` & `crypto-screening-8.0.0/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/collect/market/state/base.py` & `crypto-screening-8.0.0/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-8.0.0/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/collect/market/trades.py` & `crypto-screening-8.0.0/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/collect/screeners.py` & `crypto-screening-8.0.0/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/collect/symbols.py` & `crypto-screening-8.0.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/dataset.py` & `crypto-screening-8.0.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/exchanges.py` & `crypto-screening-8.0.0/crypto_screening/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/interval.py` & `crypto-screening-8.0.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/market/dynamic.py` & `crypto-screening-8.0.0/crypto_screening/market/dynamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,37 +15,40 @@
     assets_orders_market_state, symbols_orders_market_state,
     SymbolsOrdersMarketState, AssetsOrdersMarketState
 )
 from crypto_screening.collect.market.trades import (
     assets_trades_market_state, symbols_trades_market_state,
     SymbolsTradesMarketState, AssetsTradesMarketState
 )
-from crypto_screening.market.screeners.container import ScreenersContainer
+from crypto_screening.market.screeners.container import (
+    ScreenersContainer, FrozenScreenersContainer
+)
 
 __all__ = [
-    "ScreenersMarket"
+    "ScreenersMarket",
+    "FrozenScreenersMarket"
 ]
 
 ExchangesData = Union[Dict[str, Iterable[str]], Iterable[str]]
 
-class ScreenersMarket(ScreenersContainer):
+class FrozenScreenersMarket(FrozenScreenersContainer):
     """
     A class to represent a multi-exchange multi-pairs crypto data screener.
     Using this class enables extracting screener objects and screeners
     data by the exchange name and the symbol of the pair.
 
     parameters:
 
     - screeners:
         The screener objects to form a market.
 
-    >>> from crypto_screening.market.dynamic import ScreenersMarket
+    >>> from crypto_screening.market.dynamic import FrozenScreenersMarket
     >>> from crypto_screening.market.screeners.base import BaseScreener
     >>>
-    >>> market = ScreenersMarket(
+    >>> market = FrozenScreenersMarket(
     >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
     >>> )
     >>>
     >>> market.find_screener(exchange="binance", symbol="BTC/USDT"))
     """
 
     def assets_orderbook_market_state(
@@ -351,8 +354,30 @@
             included=included, excluded=excluded, adjust=adjust
         )
 
         return symbols_orders_market_state(
             screeners=screeners, length=length, adjust=adjust
         )
     # end symbols_orders_market_state
-# end DynamicScreenerContainer
+# end FrozenScreenersMarket
+
+class ScreenersMarket(ScreenersContainer, FrozenScreenersMarket):
+    """
+    A class to represent a multi-exchange multi-pairs crypto data screener.
+    Using this class enables extracting screener objects and screeners
+    data by the exchange name and the symbol of the pair.
+
+    parameters:
+
+    - screeners:
+        The screener objects to form a market.
+
+    >>> from crypto_screening.market.dynamic import ScreenersMarket
+    >>> from crypto_screening.market.screeners.base import BaseScreener
+    >>>
+    >>> market = ScreenersMarket(
+    >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
+    >>> )
+    >>>
+    >>> market.find_screener(exchange="binance", symbol="BTC/USDT"))
+    """
+# end ScreenersMarket
```

### Comparing `crypto-screening-7.5.6/crypto_screening/market/foundation/data.py` & `crypto-screening-8.0.0/crypto_screening/market/foundation/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,14 @@
     "DataCollector"
 ]
 
 @represent
 class DataCollector(metaclass=ABCMeta):
     """A class to represent an abstract parent class of data collectors."""
 
-    __slots__ = (
-        '_screening_process', '_timeout_process',
-        '_saving_process', '_update_process',
-        '_updating', '_saving', '_blocking',
-        '_screening', "location", "delay", "cancel"
-    )
-
     LOCATION = "datasets"
 
     DELAY = 0
     CANCEL = 0
 
     def __init__(
             self,
```

### Comparing `crypto-screening-7.5.6/crypto_screening/market/foundation/protocols.py` & `crypto-screening-8.0.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/market/foundation/state.py` & `crypto-screening-8.0.0/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/market/foundation/waiting.py` & `crypto-screening-8.0.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/market/screeners/__init__.py` & `crypto-screening-8.0.0/crypto_screening/market/screeners/__init__.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/market/screeners/base.py` & `crypto-screening-8.0.0/crypto_screening/market/screeners/orderbook.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,52 @@
-# base.py
+# orderbook.py
 
 import datetime as dt
-import time
-from abc import ABCMeta
 from typing import (
-    Optional, Union, Iterable, Any, List, Dict
+    Dict, Optional, Iterable, Union, List, Callable
 )
 
 import pandas as pd
 
-from represent import Modifiers
+from cryptofeed.types import OrderBook
+from cryptofeed.defines import L2_BOOK
 
-from multithreading import Caller, multi_threaded_call
-
-from crypto_screening.dataset import save_dataset, load_dataset, create_dataset
 from crypto_screening.symbols import adjust_symbol
-from crypto_screening.validate import validate_exchange, validate_symbol
-from crypto_screening.collect.symbols import all_exchange_symbols
-from crypto_screening.market.foundation.state import WaitingState
-from crypto_screening.market.foundation.data import DataCollector
-from crypto_screening.market.foundation.protocols import BaseScreenerProtocol
-from crypto_screening.market.foundation.waiting import (
-    base_await_initialization, base_await_dynamic_initialization,
-    base_await_dynamic_update, base_await_update
+from crypto_screening.dataset import (
+    BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME, create_dataset, ORDERBOOK_COLUMNS
+)
+from crypto_screening.market.screeners.base import BaseScreener
+from crypto_screening.market.screeners.callbacks import Callback, callback_data
+from crypto_screening.market.screeners.recorder import (
+    MarketScreener, MarketRecorder, MarketHandler
 )
 
 __all__ = [
-    "BaseScreener",
-    "BaseMarketScreener",
-    "BaseMarketController"
+    "OrderbookMarketScreener",
+    "OrderbookMarketRecorder",
+    "OrderbookScreener",
+    "orderbook_market_screener",
+    "create_orderbook_market_dataset",
+    "record_orderbook",
+    "create_orderbook_screeners"
 ]
 
-class BaseScreener(DataCollector):
+def create_orderbook_market_dataset() -> pd.DataFrame:
+    """
+    Creates a dataframe for the order book data.
+
+    :return: The dataframe.
+    """
+
+    return create_dataset(
+        columns=OrderbookMarketRecorder.COLUMNS
+    )
+# end create_orderbook_market_dataset
+
+class OrderbookScreener(BaseScreener):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
@@ -53,343 +64,166 @@
     - cancel:
         The time to cancel screening process after no new data is fetched.
 
     - delay:
         The delay to wait between each data fetching.
 
     - market:
-        The dataset of the market data.
+        The dataset of the market data as BID/ASK spread.
     """
 
-    __modifiers__ = Modifiers(**DataCollector.__modifiers__)
-    __modifiers__.hidden.append("market")
-
-    MINIMUM_DELAY = 1
-
-    NAME: Optional[str] = "BASE"
-    COLUMNS: Iterable[str] = []
-
-    __slots__ = "symbol", "exchange", "market"
-
-    SCREENER_NAME_TYPE_MATCHES: Dict[str, Any] = {}
-    SCREENER_TYPE_NAME_MATCHES: Dict[Any, str] = {}
-
-    def __init__(
-            self,
-            symbol: str,
-            exchange: str,
-            location: Optional[str] = None,
-            cancel: Optional[Union[float, dt.timedelta]] = None,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            market: Optional[pd.DataFrame] = None,
-    ) -> None:
-        """
-        Defines the class attributes.
-
-        :param symbol: The symbol of the asset.
-        :param exchange: The exchange to get source data from.
-        :param location: The saving location for the data.
-        :param delay: The delay for the process.
-        :param cancel: The cancel time for the loops.
-        :param market: The data for the market.
-        """
-
-        if not self.COLUMNS:
-            raise ValueError(
-                f"{repr(self)} must define a non-empty "
-                f"'COLUMNS' instance or class attribute."
-            )
-        # end if
-
-        super().__init__(location=location, cancel=cancel, delay=delay)
-
-        self.SCREENER_NAME_TYPE_MATCHES.setdefault(self.NAME, type(self))
-        self.SCREENER_TYPE_NAME_MATCHES.setdefault(type(self), self.NAME)
-
-        self.exchange = self.validate_exchange(exchange=exchange)
-        self.symbol = self.validate_symbol(exchange=self.exchange, symbol=symbol)
+    NAME = "ORDERBOOK"
 
-        if market is None:
-            market = create_dataset(self.COLUMNS)
-        # end if
-
-        self.market = market
-    # end __init__
+    COLUMNS = ORDERBOOK_COLUMNS
 
-    def await_initialization(
-            self,
-            stop: Optional[Union[bool, int]] = False,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
-    ) -> WaitingState[BaseScreenerProtocol]:
+    @property
+    def orderbook_market(self) -> pd.DataFrame:
         """
-        Waits for all the create_screeners to update.
+        Returns the market to hold the recorder data.
 
-        :param delay: The delay for the waiting.
-        :param stop: The value to stop the screener objects.
-        :param cancel: The time to cancel the waiting.
-
-        :returns: The total delay.
+        :return: The market object.
         """
 
-        self: Union[BaseScreener, BaseScreenerProtocol]
-
-        return base_await_initialization(
-            self, stop=stop, delay=delay, cancel=cancel
-        )
-    # end await_initialization
+        return self.market
+    # end orderbook_market
+# end OrderbookScreener
 
-    def await_update(
-            self,
-            stop: Optional[Union[bool, int]] = False,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
-    ) -> WaitingState[BaseScreenerProtocol]:
-        """
-        Waits for all the create_screeners to update.
-
-        :param delay: The delay for the waiting.
-        :param stop: The value to stop the screener objects.
-        :param cancel: The time to cancel the waiting.
-
-        :returns: The total delay.
-        """
-
-        self: Union[BaseScreener, BaseScreenerProtocol]
-
-        return base_await_update(
-            self, stop=stop, delay=delay, cancel=cancel
-        )
-    # end await_update
-
-    @staticmethod
-    def validate_exchange(exchange: str) -> str:
-        """
-        Validates the symbol value.
-
-        :param exchange: The exchange key.
-
-        :return: The validates symbol.
-        """
-
-        return validate_exchange(exchange=exchange)
-    # end validate_exchange
-
-    @staticmethod
-    def validate_symbol(exchange: str, symbol: Any) -> str:
-        """
-        Validates the symbol value.
-
-        :param exchange: The exchange key.
-        :param symbol: The key of the symbol.
-
-        :return: The validates symbol.
-        """
-
-        return validate_symbol(
-            exchange=exchange, symbol=symbol,
-            symbols=all_exchange_symbols(exchange=exchange)
-        )
-    # end validate_symbol
+async def record_orderbook(
+        screeners: Iterable[OrderbookScreener],
+        data: OrderBook,
+        timestamp: float,
+        callbacks: Optional[Iterable[Callback]] = None
+) -> bool:
+    """
+    Records the data from the crypto feed into the dataset.
 
-    def dataset_path(self, location: Optional[str] = None) -> str:
-        """
-        Creates the path to the saving file for the screener object.
+    :param screeners: The market structure.
+    :param data: The data from the exchange.
+    :param timestamp: The time of the request.
+    :param callbacks: The callbacks for the service.
 
-        :param location: The saving location of the dataset.
+    :return: The validation value.
+    """
 
-        :return: The saving path for the dataset.
-        """
+    exchange = data.exchange.lower()
+    symbol = adjust_symbol(symbol=data.symbol)
 
-        location = location or self.location
+    try:
+        index = dt.datetime.fromtimestamp(timestamp)
 
-        if location is None:
-            location = "."
-        # end if
+        bids = data.book.bids.to_list()
+        asks = data.book.asks.to_list()
 
-        return (
-            f"{location}/"
-            f"{self.exchange.lower()}/"
-            f"{self.NAME}-"
-            f"{adjust_symbol(self.symbol, separator='-')}.csv"
-        )
-    # end dataset_path
+        data = {
+            BIDS: float(bids[0][0]),
+            ASKS: float(asks[0][0]),
+            BIDS_VOLUME: float(bids[0][1]),
+            ASKS_VOLUME: float(asks[0][1])
+        }
 
-    def save_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
+        valid = False
 
-        :param location: The saving location of the dataset.
-        """
+        for screener in screeners:
+            if index in screener.market.index:
+                continue
+            # end if
 
-        if len(self.market) == 0:
-            return
-        # end if
+            valid = True
 
-        save_dataset(
-            dataset=self.market,
-            path=self.dataset_path(location=location)
-        )
-    # end save_dataset
-
-    def load_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
-
-        :param location: The saving location of the dataset.
-        """
-
-        data = load_dataset(path=self.dataset_path(location=location))
-
-        for index, data in zip(data.index[:], data.loc[:]):
-            self.market.loc[index] = data
+            screener.market.loc[index] = data
         # end for
-    # end load_dataset
-
-    def saving_loop(self) -> None:
-        """Runs the process of the price screening."""
 
-        self._saving = True
-
-        delay = self.delay
+        if valid:
+            for callback in callbacks or []:
+                payload = callback_data(
+                    data=[(timestamp, data)],
+                    exchange=exchange, symbol=symbol
+                )
 
-        if isinstance(self.delay, dt.timedelta):
-            delay = delay.total_seconds()
+                await callback.record(
+                    payload, timestamp, key=OrderbookScreener.NAME
+                )
+            # end if
         # end if
 
-        while self.saving:
-            start = time.time()
-
-            self.save_dataset()
+        return True
 
-            end = time.time()
+    except IndexError:
+        return False
+    # end try
+# end record_orderbook
 
-            time.sleep(max([delay - (end - start), self.MINIMUM_DELAY]))
-        # end while
-    # end saving_loop
-# end BaseScreener
+RecorderParameters = Dict[str, Union[Iterable[str], Dict[str, Callable]]]
 
-class BaseMarketController(DataCollector, metaclass=ABCMeta):
+class OrderbookMarketRecorder(MarketRecorder):
     """
-    A class to represent an asset price screener.
-
-    Using this class, you can create a screener object to
-    screen the market ask and bid data for a specific asset in
-    a specific exchange at real time.
+    A class to represent a crypto data feed recorder.
+    This object passes the record method to the handler object to record
+    the data fetched by the handler.
 
     Parameters:
 
-    - location:
-        The saving location for the saved data of the screener.
-
-    - cancel:
-        The time to cancel screening process after no new data is fetched.
+    - screeners:
+        The screeners to record data into their market datasets.
 
-    - delay:
-        The delay to wait between each data fetching.
+    - callbacks:
+        The callbacks to run when collecting new data.
 
-    - screeners:
-        The screener object to control and fill with data.
+    >>> from crypto_screening.market.screeners import OrderbookMarketRecorder
+    >>>
+    >>> recorder = OrderbookMarketRecorder(...)
     """
 
-    __modifiers__ = Modifiers(**DataCollector.__modifiers__)
-    __modifiers__.hidden.append("screeners")
-
-    screeners: List[BaseScreener]
+    COLUMNS = OrderbookScreener.COLUMNS
 
-    def await_initialization(
-            self,
-            stop: Optional[Union[bool, int]] = False,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
-    ) -> WaitingState[BaseScreener]:
+    @property
+    def orderbook_screeners(self) -> List[OrderbookScreener]:
         """
-        Waits for all the create_screeners to update.
+        Returns a list of all the order-book screeners.
 
-        :param delay: The delay for the waiting.
-        :param stop: The value to stop the screener objects.
-        :param cancel: The time to cancel the waiting.
-
-        :returns: The total delay.
+        :return: The order-book screeners.
         """
 
-        return base_await_dynamic_initialization(
-            self.screeners, stop=stop, delay=delay, cancel=cancel
-        )
-    # end await_initialization
+        return self.find_screeners(base=OrderbookScreener)
+    # end orderbook_screeners
 
-    def await_update(
-            self,
-            stop: Optional[Union[bool, int]] = False,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
-    ) -> WaitingState[BaseScreener]:
+    def parameters(self) -> RecorderParameters:
         """
-        Waits for all the create_screeners to update.
-
-        :param delay: The delay for the waiting.
-        :param stop: The value to stop the screener objects.
-        :param cancel: The time to cancel the waiting.
+        Returns the order book parameters.
 
-        :returns: The total delay.
+        :return: The order book parameters.
         """
 
-        return base_await_dynamic_update(
-            self.screeners, stop=stop, delay=delay, cancel=cancel
+        return dict(
+            channels=[L2_BOOK],
+            callbacks={L2_BOOK: self.record},
+            max_depth=1
         )
-    # end await_update
-
-    def save_datasets(self, location: Optional[str] = None) -> None:
-        """
-        Runs the data handling loop.
-
-        :param location: The saving location.
-        """
-
-        callers = []
+    # end parameters
 
-        for screener in self.screeners:
-            location = location or screener.location or self.location
-
-            callers.append(
-                Caller(
-                    target=screener.save_dataset,
-                    kwargs=dict(location=location)
-                )
-            )
-        # end for
-
-        multi_threaded_call(callers=callers)
-    # end save_datasets
-
-    def load_datasets(self, location: Optional[str] = None) -> None:
+    async def process(self, data: OrderBook, timestamp: float) -> bool:
         """
-        Runs the data handling loop.
+        Records the data from the crypto feed into the dataset.
 
-        :param location: The saving location.
+        :param data: The data from the exchange.
+        :param timestamp: The time of the request.
         """
 
-        callers = []
-
-        for screener in self.screeners:
-            location = location or screener.location or self.location
+        exchange = data.exchange.lower()
+        symbol = adjust_symbol(symbol=data.symbol)
 
-            callers.append(
-                Caller(
-                    target=screener.load_dataset,
-                    kwargs=dict(location=location)
-                )
-            )
-        # end for
-
-        multi_threaded_call(callers=callers)
-    # end load_datasets
-# end BaseScreener
+        return await record_orderbook(
+            screeners=self.find_screeners(
+                base=OrderbookScreener, exchange=exchange, symbol=symbol
+            ), data=data, callbacks=self.callbacks, timestamp=timestamp
+        )
+    # end process
+# end MarketOrderbookRecorder
 
-class BaseMarketScreener(BaseMarketController):
+class OrderbookMarketScreener(MarketScreener):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
@@ -400,121 +234,156 @@
 
     - cancel:
         The time to cancel screening process after no new data is fetched.
 
     - delay:
         The delay to wait between each data fetching.
 
+    - handler:
+        The handler object to handle the data feed.
+
+    - recorder:
+        The recorder object to record the data of the market from the feed.
+
     - screeners:
         The screener object to control and fill with data.
+
+    - refresh:
+        The duration of time between each refresh. 0 means no refresh.
+
+    - amount:
+        The amount of symbols for each symbols group for an exchange.
+
+    - limited:
+        The value to limit the running screeners to active exchanges.
+
+    >>> from crypto_screening.market.screeners import orderbook_market_screener
+    >>>
+    >>> structure = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
+    >>>
+    >>> screener = orderbook_market_screener(data=structure)
+    >>> screener.run()
     """
 
-    screeners: List[BaseScreener]
+    screeners: List[OrderbookScreener]
+    recorder: OrderbookMarketRecorder
+
+    COLUMNS = OrderbookMarketRecorder.COLUMNS
 
     def __init__(
             self,
-            screeners: Optional[Iterable[BaseScreener]] = None,
+            recorder: OrderbookMarketRecorder,
+            screeners: Optional[Iterable[OrderbookScreener]] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
-            delay: Optional[Union[float, dt.timedelta]] = None
+            delay: Optional[Union[float, dt.timedelta]] = None,
+            refresh: Optional[Union[float, dt.timedelta, bool]] = None,
+            limited: Optional[bool] = None,
+            handler: Optional[MarketHandler] = None,
+            amount: Optional[int] = None
     ) -> None:
         """
-        Defines the class attributes.
+        Creates the class attributes.
 
         :param location: The saving location for the data.
         :param delay: The delay for the process.
         :param cancel: The cancel time for the loops.
+        :param limited: The value to limit the screeners to active only.
+        :param refresh: The refresh time for rerunning.
+        :param handler: The handler object for the market data.
+        :param amount: The maximum amount of symbols for each feed.
+        :param recorder: The recorder object for recording the data.
         """
 
-        super().__init__(location=location, cancel=cancel, delay=delay)
-
-        self.screeners = list(screeners or [])
-    # end __init__
-
-    def await_initialization(
-            self,
-            stop: Optional[Union[bool, int]] = False,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
-    ) -> WaitingState[BaseScreener]:
-        """
-        Waits for all the create_screeners to update.
-
-        :param delay: The delay for the waiting.
-        :param stop: The value to stop the screener objects.
-        :param cancel: The time to cancel the waiting.
-
-        :returns: The total delay.
-        """
-
-        return base_await_dynamic_initialization(
-            self.screeners, stop=stop, delay=delay, cancel=cancel
+        super().__init__(
+            location=location, cancel=cancel,
+            delay=delay, recorder=recorder,
+            screeners=screeners, handler=handler, limited=limited,
+            amount=amount, refresh=refresh
         )
-    # end await_initialization
+    # end __init__
 
-    def await_update(
-            self,
-            stop: Optional[Union[bool, int]] = False,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
-    ) -> WaitingState[BaseScreener]:
+    @property
+    def orderbook_screeners(self) -> List[OrderbookScreener]:
         """
-        Waits for all the create_screeners to update.
+        Returns a list of all the order-book screeners.
 
-        :param delay: The delay for the waiting.
-        :param stop: The value to stop the screener objects.
-        :param cancel: The time to cancel the waiting.
-
-        :returns: The total delay.
+        :return: The order-book screeners.
         """
 
-        return base_await_dynamic_update(
-            self.screeners, stop=stop, delay=delay, cancel=cancel
-        )
-    # end await_update
-
-    def save_datasets(self, location: Optional[str] = None) -> None:
-        """
-        Runs the data handling loop.
+        return self.find_screeners(base=OrderbookScreener)
+    # end orderbook_screeners
+# end MarketOrderbookScreener
 
-        :param location: The saving location.
-        """
+def create_orderbook_screeners(
+        data: Dict[str, Iterable[str]],
+        location: Optional[str] = None,
+        cancel: Optional[Union[float, dt.timedelta]] = None,
+        delay: Optional[Union[float, dt.timedelta]] = None,
+) -> List[OrderbookScreener]:
+    """
+    Defines the class attributes.
 
-        callers = []
+    :param data: The data for the screeners.
+    :param location: The saving location for the data.
+    :param cancel: The time to cancel the waiting.
+    :param delay: The delay for the process.
+    """
 
-        for screener in self.screeners:
-            location = location or screener.location or self.location
+    screeners = []
 
-            callers.append(
-                Caller(
-                    target=screener.save_dataset,
-                    kwargs=dict(location=location)
+    for exchange, symbols in data.items():
+        for symbol in symbols:
+            screeners.append(
+                OrderbookScreener(
+                    symbol=symbol, exchange=exchange, delay=delay,
+                    location=location, cancel=cancel
                 )
             )
         # end for
+    # end for
 
-        multi_threaded_call(callers=callers)
-    # end save_datasets
+    return screeners
+# end create_orderbook_screeners
 
-    def load_datasets(self, location: Optional[str] = None) -> None:
-        """
-        Runs the data handling loop.
-
-        :param location: The saving location.
-        """
-
-        callers = []
+def orderbook_market_screener(
+        data: Dict[str, Iterable[str]],
+        location: Optional[str] = None,
+        cancel: Optional[Union[float, dt.timedelta]] = None,
+        delay: Optional[Union[float, dt.timedelta]] = None,
+        limited: Optional[bool] = None,
+        handler: Optional[MarketHandler] = None,
+        amount: Optional[int] = None,
+        callbacks: Optional[Iterable[Callback]] = None,
+        refresh: Optional[Union[float, dt.timedelta, bool]] = None,
+        recorder: Optional[OrderbookMarketRecorder] = None
+) -> OrderbookMarketScreener:
+    """
+    Creates the market screener object for the data.
 
-        for screener in self.screeners:
-            location = location or screener.location or self.location
+    :param data: The market data.
+    :param handler: The handler object for the market data.
+    :param limited: The value to limit the screeners to active only.
+    :param refresh: The refresh time for rerunning.
+    :param amount: The maximum amount of symbols for each feed.
+    :param recorder: The recorder object for recording the data.
+    :param location: The saving location for the data.
+    :param delay: The delay for the process.
+    :param cancel: The cancel time for the loops.
+    :param callbacks: The callbacks for the service.
 
-            callers.append(
-                Caller(
-                    target=screener.load_dataset,
-                    kwargs=dict(location=location)
-                )
-            )
-        # end for
+    :return: The market screener object.
+    """
 
-        multi_threaded_call(callers=callers)
-    # end load_datasets
-# end BaseScreener
+    screeners = create_orderbook_screeners(
+        data=data, location=location,
+        cancel=cancel, delay=delay
+    )
+
+    return OrderbookMarketScreener(
+        recorder=recorder or OrderbookMarketRecorder(
+            screeners=screeners, callbacks=callbacks
+        ), screeners=screeners,
+        handler=handler, location=location, amount=amount,
+        cancel=cancel, delay=delay, limited=limited, refresh=refresh
+    )
+# end orderbook_market_recorder
```

### Comparing `crypto-screening-7.5.6/crypto_screening/market/screeners/callbacks.py` & `crypto-screening-8.0.0/crypto_screening/market/screeners/callbacks.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/market/screeners/collectors/base.py` & `crypto-screening-8.0.0/crypto_screening/market/screeners/collectors/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # base.py
 
 import threading
 import datetime as dt
 import time
 from typing import List, Tuple, Optional, Iterable, Union, Dict, Any
 
-from crypto_screening.market.screeners.base import BaseScreener, BaseMarketController
 from crypto_screening.market.screeners.container import ScreenersContainer
+from crypto_screening.market.screeners.base import BaseScreener, BaseMarketScreener
 from crypto_screening.collect.market.state.base import index_to_datetime
 
 __all__ = [
     "ScreenersDataCollector"
 ]
 
 Data = List[Tuple[Union[str, float, dt.datetime], Dict[str, Optional[Union[str, float, bool]]]]]
 
-class ScreenersDataCollector(ScreenersContainer, BaseMarketController):
+class ScreenersDataCollector(BaseMarketScreener, ScreenersContainer):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
@@ -52,20 +52,19 @@
         Defines the class attributes.
 
         :param location: The saving location for the data.
         :param delay: The delay for the process.
         :param cancel: The cancel time for the loops.
         """
 
-        BaseMarketController.__init__(
-            self, location=location, cancel=cancel, delay=delay
+        super().__init__(
+            location=location, cancel=cancel,
+            delay=delay, screeners=screeners
         )
 
-        ScreenersContainer.__init__(self, screeners=screeners)
-
         self._handling_processes: List[threading.Thread] = []
         self.awaiting: List[Dict[str, Any]] = []
 
         self._handling = False
     # end __init__
 
     @property
@@ -202,15 +201,15 @@
         :param wait: The value to wait after starting to run the process.
         :param block: The value to block the execution.
         :param update: The value to update the screeners.
         :param timeout: The valur to add a start_timeout to the process.
         """
 
         if handlers is None:
-            handlers = 1
+            handlers = 0
         # end if
 
         if handlers:
             self._handling = True
         # end if
 
         for _ in range(handlers):
```

### Comparing `crypto-screening-7.5.6/crypto_screening/market/screeners/collectors/database.py` & `crypto-screening-8.0.0/crypto_screening/market/screeners/collectors/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/market/screeners/collectors/sockets.py` & `crypto-screening-8.0.0/crypto_screening/market/screeners/collectors/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/market/screeners/combined.py` & `crypto-screening-8.0.0/crypto_screening/market/screeners/combined.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,44 @@
 # combined.py
 
 import datetime as dt
 from typing import (
-    Dict, Optional, Iterable, Any,
-    Union, List, Callable, Type
+    Dict, Optional, Iterable, Any, Union, List, Type, Callable
 )
 
-import pandas as pd
-
-from sqlalchemy import Engine
-
-from cryptofeed import FeedHandler
-
 from crypto_screening.market.screeners.orderbook import (
-    orderbook_market_screener, OrderbookScreener,
-    OrderbookMarketRecorder
+    orderbook_market_screener
 )
 from crypto_screening.market.screeners.ohlcv import (
-    ohlcv_market_screener, OHLCVScreener,
-    OHLCVMarketRecorder
+    ohlcv_market_screener
 )
 from crypto_screening.market.screeners.trades import (
-    trades_market_screener, TradesScreener,
-    TradesMarketRecorder
+    trades_market_screener
 )
 from crypto_screening.market.screeners.orders import (
-    orders_market_screener, OrdersScreener,
-    OrdersMarketRecorder
+    orders_market_screener
 )
+from crypto_screening.market.screeners.container import ScreenersContainer
 from crypto_screening.market.screeners.callbacks import Callback
 from crypto_screening.market.screeners.recorder import (
-    MarketScreener
+    MarketScreener, MarketRecorder, MarketHandler
 )
 
 __all__ = [
     "CombinedMarketRecorder",
     "CombinedMarketScreener",
     "combined_market_screener",
     "CATEGORIES",
-    "RECORDERS",
     "Category",
     "OrderbookCategory",
     "TradesCategory",
     "OrdersCategory",
     "OHLCVCategory"
 ]
 
-Market = Dict[str, Dict[str, pd.DataFrame]]
-
 RecorderParameters = Dict[str, Union[Iterable[str], Dict[str, Callable]]]
 
 class Category:
     """A class to represent a category."""
 
     __slots__ = ()
 # end Category
@@ -76,34 +63,26 @@
 
 class OHLCVCategory(Category):
     """A class to represent a category."""
 
     __slots__ = ()
 # end OHLCVCategory
 
-RECORDERS = (
-    OHLCVMarketRecorder,
-    TradesMarketRecorder,
-    OrderbookMarketRecorder,
-    OrdersMarketRecorder
-)
 CATEGORIES = (
     OHLCVCategory,
     TradesCategory,
     OrdersCategory,
     OrderbookCategory
 )
 
-Recorder = Union[*RECORDERS]
-CategoryBase = Union[*CATEGORIES]
-
-MarketRecorders = Union[
-    Iterable[Type[CategoryBase]],
-    Iterable[Recorder],
-    Dict[Type[CategoryBase], Iterable[Recorder]]
+CategoryBase = Union[
+    OHLCVCategory,
+    TradesCategory,
+    OrdersCategory,
+    OrderbookCategory
 ]
 
 def gather(recorders: Iterable):
     """
     Gathers the functions to record the data.
 
     :param recorders: The data recorders.
@@ -127,15 +106,15 @@
 
         return True
     # end record
 
     return record
 # end gather
 
-class CombinedMarketRecorder:
+class CombinedMarketRecorder(MarketRecorder, ScreenersContainer):
     """
     A class to represent a crypto data feed recorder.
     This object passes the record method to the handler object to record
     the data fetched by the handler.
 
     Parameters:
 
@@ -143,31 +122,47 @@
         The Recorder objects to contron and collect data from, into the markets.
 
     >>> from crypto_screening.market.screeners import CombinedMarketRecorder
     >>>
     >>> recorder = CombinedMarketRecorder(...)
     """
 
-    def __init__(self, recorders: Iterable[Recorder]) -> None:
+    def __init__(self, recorders: Iterable[MarketRecorder]) -> None:
         """
         Defines the class attributes.
 
         :param recorders: The categories for the market screener.
         """
 
+        screeners = []
         structure: Dict[str, List[str]] = {}
 
         for recorder in recorders:
             structure.update(recorder.structure())
+            screeners.extend(recorder.screeners)
         # end for
 
+        screeners = list(set(screeners))
+
+        super().__init__(screeners=screeners)
+
         self.recorders = list(recorders)
         self._structure = structure
     # end __init__
 
+    def update_screeners(self) -> None:
+        """Updates the records of the object."""
+
+        super().update_screeners()
+
+        for recorder in self.recorders:
+            recorder.update_screeners()
+        # end for
+    # end update_screeners
+
     def structure(self) -> Dict[str, List[str]]:
         """
         Returns the structure of the market data.
 
         :return: The structure of the market.
         """
 
@@ -208,17 +203,15 @@
             channels=list(set(channels)),
             callbacks=callbacks,
             max_depth=1
         )
     # end parameters
 # end CombinedMarketRecorder
 
-Screener = Union[OrderbookScreener, OHLCVScreener, TradesScreener, OrdersScreener]
-
-class CombinedMarketScreener(MarketScreener):
+class CombinedMarketScreener(MarketScreener, ScreenersContainer):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
@@ -266,15 +259,15 @@
             markets: Iterable[MarketScreener],
             recorder: CombinedMarketRecorder,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None,
             refresh: Optional[Union[float, dt.timedelta, bool]] = None,
             limited: Optional[bool] = None,
-            handler: Optional[FeedHandler] = None,
+            handler: Optional[MarketHandler] = None,
             amount: Optional[int] = None
     ) -> None:
         """
         Creates the class attributes.
 
         :param location: The saving location for the data.
         :param markets: The market screeners.
@@ -296,131 +289,68 @@
         super().__init__(
             location=location, cancel=cancel,
             delay=delay, recorder=recorder,
             screeners=screeners, handler=handler, limited=limited,
             amount=amount, refresh=refresh
         )
 
-        self.markets = list(markets)
-        self.screeners = list(screeners)
+        self.markets = markets
     # end __init__
 
-    @property
-    def orderbook_screeners(self) -> List[OrderbookScreener]:
-        """
-        Returns a list of all the order-book screeners.
-
-        :return: The order-book screeners.
-        """
-
-        return [
-            screener for screener in self.screeners
-            if isinstance(screener, OrderbookScreener)
-        ]
-    # end orderbook_screeners
-
-    @property
-    def orders_screeners(self) -> List[OrdersScreener]:
-        """
-        Returns a list of all the order-book screeners.
+    def update_screeners(self) -> None:
+        """Updates the records of the object."""
 
-        :return: The orders screeners.
-        """
+        super().update_screeners()
 
-        return [
-            screener for screener in self.screeners
-            if isinstance(screener, OrdersScreener)
-        ]
-    # end orders_screeners
-
-    @property
-    def ohlcv_screeners(self) -> List[OHLCVScreener]:
-        """
-        Returns a list of all the order-book screeners.
-
-        :return: The OHLCV screeners.
-        """
-
-        return [
-            screener for screener in self.screeners
-            if isinstance(screener, OHLCVScreener)
-        ]
-    # end ohlcv_screeners
-
-    @property
-    def trades_screeners(self) -> List[TradesScreener]:
-        """
-        Returns a list of all the order-book screeners.
-
-        :return: The trades screeners.
-        """
-
-        return [
-            screener for screener in self.screeners
-            if isinstance(screener, TradesScreener)
-        ]
-    # end trades_screeners
-
-    def connect_screeners(self) -> None:
-        """Connects the screeners to the recording object."""
-
-        for market in self.markets:
-            market.connect_screeners()
-        # end for
-    # end connect_screeners
+        self.recorder.update_screeners()
+    # end update_screeners
 
     def merge_screeners(self) -> None:
         """Connects the screeners to the recording object."""
 
         for ohlcv_screener in self.ohlcv_screeners:
             for orderbook_screener in self.orderbook_screeners:
                 if (
                     (ohlcv_screener.exchange == orderbook_screener.exchange) and
                     (ohlcv_screener.symbol == orderbook_screener.symbol)
                 ):
-                    orderbook_screener.market = ohlcv_screener.orderbook_market
+                    ohlcv_screener.orderbook_market = orderbook_screener.market
                 # end if
             # end for
         # end for
     # end merge_screeners
 # end CombinedMarketScreener
 
-CATEGORY_RECORDER_CONSTRUCTOR_MATCHES = {
+CATEGORY_MARKET_SCREENER_CONSTRUCTOR_MATCHES = {
     OrderbookCategory: orderbook_market_screener,
     OHLCVCategory: ohlcv_market_screener,
     TradesCategory: trades_market_screener,
     OrdersCategory: orders_market_screener
 }
 
-Databases = Union[Iterable[str], Dict[str, Engine]]
-
 def combined_market_screener(
         data: Dict[str, Iterable[str]],
         categories: Optional[Type[CategoryBase]] = None,
         location: Optional[str] = None,
         cancel: Optional[Union[float, dt.timedelta]] = None,
         delay: Optional[Union[float, dt.timedelta]] = None,
         limited: Optional[bool] = None,
-        handler: Optional[FeedHandler] = None,
+        handler: Optional[MarketHandler] = None,
         amount: Optional[int] = None,
         callbacks: Optional[Iterable[Callback]] = None,
         refresh: Optional[Union[float, dt.timedelta, bool]] = None,
-        recorder: Optional[OrderbookMarketRecorder] = None,
-        fixed: Optional[bool] = True,
-        parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
+        recorder: Optional[CombinedMarketRecorder] = None,
 ) -> CombinedMarketScreener:
     """
     Creates the market screener object for the data.
 
     :param data: The market data.
     :param categories: The categories for the markets.
     :param handler: The handler object for the market data.
     :param limited: The value to limit the screeners to active only.
-    :param parameters: The parameters for the exchanges.
-    :param fixed: The value for fixed parameters to all exchanges.
     :param refresh: The refresh time for rerunning.
     :param amount: The maximum amount of symbols for each feed.
     :param recorder: The recorder object for recording the data.
     :param location: The saving location for the data.
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
     :param callbacks: The callbacks for the service.
@@ -428,31 +358,53 @@
     :return: The market screener object.
     """
 
     if categories is None:
         categories = CATEGORIES
     # end if
 
-    markets = [
-        CATEGORY_RECORDER_CONSTRUCTOR_MATCHES[category](
-            recorder=recorder, handler=handler, data=data,
+    categories = list(categories)
+
+    markets = []
+
+    if (OHLCVCategory in categories) and (OrderbookCategory in categories):
+        categories.remove(OHLCVCategory)
+        categories.remove(OrderbookCategory)
+
+        orderbook_market = orderbook_market_screener(
+            handler=handler, data=data, callbacks=callbacks,
+            location=location, amount=amount, cancel=cancel,
+            delay=delay, limited=limited, refresh=refresh
+        )
+
+        orderbook_market.recorder.disable()
+
+        ohlcv_market = ohlcv_market_screener(
+            handler=handler, data=data, callbacks=callbacks,
             location=location, amount=amount, cancel=cancel,
             delay=delay, limited=limited, refresh=refresh,
-            fixed=fixed, parameters=parameters, callbacks=callbacks
+            screeners=orderbook_market.screeners
+        )
+
+        ohlcv_market.merge_screeners()
+
+        markets.append(orderbook_market)
+        markets.append(ohlcv_market)
+    # end if
+
+    markets.extend(
+        CATEGORY_MARKET_SCREENER_CONSTRUCTOR_MATCHES[category](
+            handler=handler, data=data, callbacks=callbacks,
+            location=location, amount=amount, cancel=cancel,
+            delay=delay, limited=limited, refresh=refresh
         ) for category in set(categories)
-    ]
+    )
 
-    screener = CombinedMarketScreener(
+    market = CombinedMarketScreener(
         markets=markets, recorder=recorder or CombinedMarketRecorder(
             recorders=[market.recorder for market in markets]
         ), handler=handler, location=location, amount=amount, cancel=cancel,
         delay=delay, limited=limited, refresh=refresh
     )
 
-    screener.merge_screeners()
-    screener.add_feeds(
-        data=screener.recorder.structure(),
-        fixed=fixed, parameters=parameters
-    )
-
-    return screener
+    return market
 # end combined_market_screener
```

### Comparing `crypto-screening-7.5.6/crypto_screening/market/screeners/container.py` & `crypto-screening-8.0.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,683 +1,713 @@
-# container.py
+# ohlcv.py
 
-from typing import Iterable, List, Type, TypeVar, Optional, Dict
+import datetime as dt
+from typing import (
+    Dict, Optional, Iterable, Any,
+    Union, List, Callable, Tuple
+)
+
+import pandas as pd
 
-from represent import represent
+from cryptofeed.types import OrderBook
+from cryptofeed.defines import L2_BOOK
 
-from crypto_screening.market.screeners.ohlcv import OHLCVScreener
-from crypto_screening.market.screeners.orderbook import OrderbookScreener
-from crypto_screening.market.screeners.trades import TradesScreener
-from crypto_screening.market.screeners.orders import OrdersScreener
+from crypto_screening.interval import interval_to_total_time
+from crypto_screening.dataset import (
+    OHLCV_COLUMNS, bid_ask_to_ohlcv,
+    load_dataset, save_dataset, create_dataset
+)
+from crypto_screening.validate import validate_interval
+from crypto_screening.symbols import adjust_symbol
 from crypto_screening.market.screeners.base import BaseScreener
+from crypto_screening.market.screeners.callbacks import Callback, callback_data
+from crypto_screening.market.screeners.recorder import (
+    MarketScreener, MarketRecorder, MarketHandler
+)
+from crypto_screening.market.screeners.orderbook import (
+    OrderbookScreener, record_orderbook, create_orderbook_screeners
+)
 
 __all__ = [
-    "screeners_table",
-    "ScreenersContainer"
+    "OHLCVMarketScreener",
+    "OHLCVMarketRecorder",
+    "OHLCVScreener",
+    "ohlcv_market_screener",
+    "create_ohlcv_market_dataset",
+    "create_ohlcv_screeners"
 ]
 
-_S = TypeVar(
-    "_S",
-    BaseScreener,
-    OHLCVScreener,
-    OrderbookScreener,
-    TradesScreener,
-    OrdersScreener
-)
+Indexes = Dict[str, Dict[str, Dict[str, int]]]
 
-ScreenersTable = Dict[
-    Optional[Type[BaseScreener]],
-    Dict[
-        Optional[str],
-        Dict[Optional[str], Dict[Optional[str], List[BaseScreener]]]
-    ]
-]
+def create_ohlcv_market_dataset() -> pd.DataFrame:
+    """
+    Creates a dataframe for the order book data.
 
-def screeners_table(
-        screeners: Iterable[BaseScreener],
-        table: Optional[ScreenersTable] = None
-) -> ScreenersTable:
+    :return: The dataframe.
     """
-    Inserts all the screeners into the table.
 
-    :param screeners: The screeners to insert into the table.
-    :param table: The table to use for the data.
+    return create_dataset(
+        columns=OHLCVMarketRecorder.COLUMNS
+    )
+# end create_ohlcv_market_dataset
 
-    :return: The screeners table.
+class OHLCVScreener(BaseScreener):
     """
+    A class to represent an asset price screener.
 
-    if table is None:
-        table = {}
-    # end if
+    Using this class, you can create a screener object to
+    screen the market ask and bid data for a specific asset in
+    a specific exchange at real time.
 
-    for screener in screeners:
-        for interval in {
-            (
-                screener.interval
-                if isinstance(screener, OHLCVScreener) else
-                None
-            ), None
-        }:
-            lists = [
-                (
-                    table.
-                    setdefault(type(screener), {}).
-                    setdefault(screener.exchange, {}).
-                    setdefault(screener.symbol, {}).
-                    setdefault(interval, [])
-                ),
-                (
-                    table.
-                    setdefault(type(screener), {}).
-                    setdefault(screener.exchange, {}).
-                    setdefault(None, {}).
-                    setdefault(interval, [])
-                ),
-                (
-                    table.
-                    setdefault(type(screener), {}).
-                    setdefault(None, {}).
-                    setdefault(screener.symbol, {}).
-                    setdefault(interval, [])
-                ),
-                (
-                    table.
-                    setdefault(type(screener), {}).
-                    setdefault(None, {}).
-                    setdefault(None, {}).
-                    setdefault(interval, [])
-                ),
-                (
-                    table.
-                    setdefault(type(screener), {}).
-                    setdefault(None, {}).
-                    setdefault(None, {}).
-                    setdefault(None, [])
-                ),
-                (
-                    table.
-                    setdefault(None, {}).
-                    setdefault(screener.exchange, {}).
-                    setdefault(screener.symbol, {}).
-                    setdefault(interval, [])
-                ),
-                (
-                    table.
-                    setdefault(None, {}).
-                    setdefault(screener.exchange, {}).
-                    setdefault(None, {}).
-                    setdefault(interval, [])
-                ),
-                (
-                    table.
-                    setdefault(None, {}).
-                    setdefault(None, {}).
-                    setdefault(screener.symbol, {}).
-                    setdefault(interval, [])
-                ),
-                (
-                    table.
-                    setdefault(None, {}).
-                    setdefault(None, {}).
-                    setdefault(None, {}).
-                    setdefault(interval, [])
-                )
-            ]
+    Parameters:
 
-            for screeners_list in lists:
-                if screener not in screeners_list:
-                    screeners_list.append(screener)
-                # end if
-            # end for
-        # end for
-    # end for
+    - symbol:
+        The symbol of an asset to screen.
 
-    return table
-# end screeners_table
+    - exchange:
+        The key of the exchange platform to screen data from.
 
-@represent
-class ScreenersContainer:
-    """
-    A class to represent a multi-exchange multi-pairs crypto data screener.
-    Using this class enables extracting screener objects and screeners
-    data by the exchange name and the symbol of the pair.
+    - location:
+        The saving location for the saved data of the screener.
 
-    parameters:
+    - cancel:
+        The time to cancel screening process after no new data is fetched.
 
-    - screeners:
-        The screener objects to form a market.
+    - delay:
+        The delay to wait between each data fetching.
 
-    >>> from crypto_screening.market.screeners.container import ScreenersContainer
-    >>> from crypto_screening.market.screeners.base import BaseScreener
-    >>>
-    >>> container = ScreenersContainer(
-    >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
-    >>> )
+    - interval:
+        The interval for the data structure of OHLCV.
+
+    - market:
+        The dataset of the market data as OHLCV.
+
+    - base_market:
+        The dataset of the market data as BID/ASK spread.
     """
 
-    def __init__(self, screeners: Iterable[BaseScreener]) -> None:
+    INTERVAL = "1m"
+    NAME = "OHLCV"
+
+    COLUMNS = OHLCV_COLUMNS
+
+    def __init__(
+            self,
+            symbol: str,
+            exchange: str,
+            interval: Optional[str] = None,
+            location: Optional[str] = None,
+            cancel: Optional[Union[float, dt.timedelta]] = None,
+            delay: Optional[Union[float, dt.timedelta]] = None,
+            market: Optional[pd.DataFrame] = None,
+            orderbook_market: Optional[pd.DataFrame] = None
+    ) -> None:
         """
         Defines the class attributes.
 
-        :param screeners: The data screener object.
+        :param symbol: The symbol of the asset.
+        :param interval: The interval for the data.
+        :param exchange: The exchange to get source data from.
+        :param location: The saving location for the data.
+        :param delay: The delay for the process.
+        :param cancel: The cancel time for the loops.
+        :param market: The data for the market.
+        :param orderbook_market: The base market dataset.
         """
 
-        self._screeners = list(screeners)
+        super().__init__(
+            symbol=symbol, exchange=exchange, location=location,
+            cancel=cancel, delay=delay, market=market
+        )
+
+        self.interval = self.validate_interval(interval or self.INTERVAL)
 
-        self._table = screeners_table(self.screeners)
+        self.orderbook_market = orderbook_market
     # end __init__
 
-    @property
-    def screeners(self) -> List[BaseScreener]:
+    @staticmethod
+    def validate_interval(interval: str) -> str:
         """
-        Returns a list of all the screeners.
+        Validates the symbol value.
+
+        :param interval: The interval for the data.
 
-        :return: The screeners.
+        :return: The validates symbol.
         """
 
-        return list(self._screeners)
-    # end screeners
+        return validate_interval(interval=interval)
+    # end validate_symbol
 
     @property
-    def orderbook_screeners(self) -> List[OrderbookScreener]:
+    def ohlcv_market(self) -> pd.DataFrame:
         """
-        Returns a list of all the order-book screeners.
+        Returns the market to hold the recorder data.
 
-        :return: The order-book screeners.
+        :return: The market object.
         """
 
-        return self.find_screeners(base=OrderbookScreener)
-    # end orderbook_screeners
+        return self.market
+    # end ohlcv_market
 
-    @property
-    def orders_screeners(self) -> List[OrdersScreener]:
+    def orderbook_dataset_path(self, location: Optional[str] = None) -> str:
         """
-        Returns a list of all the order-book screeners.
+        Creates the path to the saving file for the screener object.
 
-        :return: The orders screeners.
+        :param location: The saving location of the dataset.
+
+        :return: The saving path for the dataset.
         """
 
-        return self.find_screeners(base=OrdersScreener)
-    # end orders_screeners
+        return (
+            self.dataset_path(location=location).
+            replace(self.NAME, OrderbookScreener.NAME)
+        )
+    # end orderbook_dataset_path
 
-    @property
-    def ohlcv_screeners(self) -> List[OHLCVScreener]:
+    def save_orderbook_dataset(self, location: Optional[str] = None) -> None:
         """
-        Returns a list of all the order-book screeners.
+        Saves the data of the screener.
 
-        :return: The OHLCV screeners.
+        :param location: The saving location of the dataset.
         """
 
-        return self.find_screeners(base=OHLCVScreener)
-    # end ohlcv_screeners
+        if len(self.orderbook_market) > 0:
+            save_dataset(
+                dataset=self.orderbook_market,
+                path=self.orderbook_dataset_path(location=location)
+            )
+        # end if
+    # end save_orderbook_dataset
 
-    @property
-    def trades_screeners(self) -> List[TradesScreener]:
+    def ohlcv_dataset_path(self, location: Optional[str] = None) -> str:
         """
-        Returns a list of all the order-book screeners.
+        Creates the path to the saving file for the screener object.
+
+        :param location: The saving location of the dataset.
 
-        :return: The trades screeners.
+        :return: The saving path for the dataset.
         """
 
-        return self.find_screeners(base=TradesScreener)
-    # end trades_screeners
+        return self.dataset_path(location=location)
+    # end ohlcv_dataset_path
 
-    def update(self) -> None:
-        """Updates the records of the object."""
-    # end update
+    def save_ohlcv_dataset(self, location: Optional[str] = None) -> None:
+        """
+        Saves the data of the screener.
 
-    def structure(self) -> Dict[str, List[str]]:
+        :param location: The saving location of the dataset.
         """
-        Returns the structure of the market data.
 
-        :return: The structure of the market.
+        if len(self.ohlcv_market) > 0:
+            save_dataset(
+                dataset=self.ohlcv_market,
+                path=self.ohlcv_dataset_path(location=location)
+            )
+        # end if
+    # end save_ohlcv_dataset
+
+    def save_datasets(self, location: Optional[str] = None) -> None:
         """
+        Saves the data of the screener.
 
-        return {
-            exchange: list([symbol for symbol in symbols if symbol is not None])
-            for exchange, symbols in self._table[None].items()
-            if exchange is not None
-        }
-    # end structure
+        :param location: The saving location of the dataset.
+        """
 
-    def add(
-            self,
-            screeners: Iterable[BaseScreener],
-            adjust: Optional[bool] = True,
-            update: Optional[bool] = True
-    ) -> None:
+        self.save_ohlcv_dataset(location=location)
+        self.save_orderbook_dataset(location=location)
+    # end save_datasets
+
+    def load_ohlcv_dataset(self, location: Optional[str] = None) -> None:
         """
-        Updates the data with the new screeners.
+        Saves the data of the screener.
 
-        :param screeners: The new screeners to add.
-        :param adjust: The value to adjust for screeners.
-        :param update: The value to update.
+        :param location: The saving location of the dataset.
         """
 
-        new_screeners = []
+        data = load_dataset(path=self.ohlcv_dataset_path(location=location))
 
-        for screener in screeners:
-            if screener not in self._screeners:
-                new_screeners.append(screener)
+        for index, data in zip(data.index[:], data.loc[:]):
+            self.ohlcv_market.loc[index] = data
+        # end for
+    # end load_ohlcv_dataset
 
-            elif not adjust:
-                raise ValueError(
-                    f"Cannot add screener {repr(screener)} to "
-                    f"{repr(self)} because it is already present."
-                )
-            # end if
+    def load_orderbook_dataset(self, location: Optional[str] = None) -> None:
+        """
+        Saves the data of the screener.
+
+        :param location: The saving location of the dataset.
+        """
+
+        data = load_dataset(path=self.orderbook_dataset_path(location=location))
+
+        for index, data in zip(data.index[:], data.loc[:]):
+            self.orderbook_market.loc[index] = data
         # end for
+    # end load_orderbook_dataset
 
-        self._screeners.extend(new_screeners)
+    def load_datasets(self, location: Optional[str] = None) -> None:
+        """
+        Saves the data of the screener.
 
-        screeners_table(new_screeners, table=self._table)
+        :param location: The saving location of the dataset.
+        """
 
-        if update:
-            self.update()
-        # end if
-    # end update
+        self.load_ohlcv_dataset(location=location)
+        self.load_orderbook_dataset(location=location)
+    # end load_datasets
 
-    def remove(
-            self,
-            screeners: Iterable[BaseScreener],
-            adjust: Optional[bool] = True,
-            update: Optional[bool] = True
-    ) -> None:
+    def orderbook_screener(self) -> OrderbookScreener:
         """
-        Updates the data with the new screeners.
+        Creates the orderbook screener object.
 
-        :param screeners: The new screeners to add.
-        :param adjust: The value to adjust for screeners.
-        :param update: The value to update.
+        :return: The orderbook screener.
         """
 
-        for screener in screeners:
-            if screener in self._screeners:
-                self._screeners.remove(screener)
+        return OrderbookScreener(
+            symbol=self.symbol, exchange=self.exchange, location=self.location,
+            cancel=self.cancel, delay=self.delay, market=self.orderbook_market
+        )
+    # end orderbook_screener
+# end OHLCVScreener
 
-            elif not adjust:
-                raise ValueError(
-                    f"Cannot remove screener {repr(screener)} from "
-                    f"{repr(self)} because it is not present."
-                )
-            # end if
-        # end for
+async def record_ohlcv(
+        screeners: Iterable[Union[OrderbookScreener, OHLCVScreener]],
+        indexes: Indexes,
+        data: OrderBook,
+        timestamp: float,
+        callbacks: Optional[Iterable[Callback]] = None
+) -> bool:
+    """
+    Records the data from the crypto feed into the dataset.
+
+    :param screeners: The screeners.
+    :param indexes: The indexes of the OHLCV market.
+    :param data: The data from the exchange.
+    :param timestamp: The time of the request.
+    :param callbacks: The callbacks for the service.
+
+    :return: The validation value.
+    """
+
+    orderbook_screeners: List[OrderbookScreener] = [
+        screener for screener in screeners
+        if isinstance(screener, OrderbookScreener)
+    ]
+
+    if not orderbook_screeners:
+        return False
+    # end if
+
+    if not await record_orderbook(
+        screeners=orderbook_screeners, callbacks=callbacks,
+        data=data, timestamp=timestamp
+    ):
+        return False
+    # end if
 
-        self._table.clear()
+    exchange = data.exchange.lower()
+    symbol = adjust_symbol(symbol=data.symbol)
 
-        screeners_table(self._screeners, table=self._table)
+    ohlcv_screeners: Dict[str, List[OHLCVScreener]] = {}
+    ohlcv_datasets: Dict[str, pd.DataFrame] = {}
 
-        if update:
-            self.update()
+    for screener in screeners:
+        if isinstance(screener, OHLCVScreener):
+            (
+                ohlcv_screeners.
+                setdefault(screener.interval, []).
+                append(screener)
+            )
         # end if
-    # end remove
+    # end for
 
-    def find_screeners(
-            self,
-            exchange: Optional[str] = None,
-            symbol: Optional[str] = None,
-            base: Optional[Type[_S]] = None,
-            interval: Optional[str] = None,
-            adjust: Optional[bool] = True
-    ) -> List[_S]:
-        """
-        Returns the data by according to the parameters.
+    if not ohlcv_screeners:
+        return False
+    # end if
 
-        :param base: The base type of the screener.
-        :param exchange: The exchange name.
-        :param symbol: The symbol name.
-        :param interval: The interval for the search.
-        :param adjust: The value to adjust for the screeners.
-
-        :return: The data.
-        """
-
-        try:
-            return list(self._table[base][exchange][symbol][interval])
-
-        except KeyError:
-            if not adjust:
-                raise ValueError(
-                    f"Cannot find screeners  matching to "
-                    f"type - {base}, exchange - {exchange}, "
-                    f"symbol - {symbol}, interval - {interval} "
-                    f"inside {repr(self)}"
-                )
-            # end if
-        # end try
-    # end find_screeners
+    spread = orderbook_screeners[0].market
 
-    def find_screener(
-            self,
-            exchange: Optional[str] = None,
-            symbol: Optional[str] = None,
-            base: Optional[Type[_S]] = None,
-            interval: Optional[str] = None,
-            index: Optional[int] = None,
-            adjust: Optional[bool] = True
-    ) -> _S:
-        """
-        Returns the data by according to the parameters.
-
-        :param base: The base type of the screener.
-        :param exchange: The exchange name.
-        :param symbol: The symbol name.
-        :param interval: The interval for the search.
-        :param index: The index of the screener in the list.
-        :param adjust: The value to adjust for the screeners.
-
-        :return: The data.
-        """
-
-        try:
-            return self.find_screeners(
-                exchange=exchange, symbol=symbol,
-                base=base, interval=interval, adjust=adjust
-            )[index or 0]
-
-        except IndexError:
-            if not adjust:
-                raise IndexError(
-                    f"Cannot find screeners matching to "
-                    f"type - {base}, exchange - {exchange}, "
-                    f"symbol - {symbol}, interval - {interval}, "
-                    f"index - {index} inside {repr(self)}"
-                )
-            # end if
-        # end try
-    # end find_orderbook_screener
+    for interval, screeners in ohlcv_screeners.items():
+        dataset_index = (
+            indexes.
+            setdefault(exchange, {}).
+            setdefault(symbol, {}).
+            setdefault(interval, 0)
+        )
 
-    def screener_in_market(
-            self,
-            exchange: Optional[str] = None,
-            symbol: Optional[str] = None,
-            base: Optional[Type[_S]] = None,
-            interval: Optional[str] = None
-    ) -> bool:
-        """
-        Returns the data by according to the parameters.
-
-        :param base: The base type of the screener.
-        :param exchange: The exchange name.
-        :param symbol: The symbol name.
-        :param interval: The interval to search.
-
-        :return: The data.
-        """
-
-        try:
-            self.find_screener(
-                exchange=exchange, symbol=symbol,
-                base=base, interval=interval
+        span: dt.timedelta = spread.index[-1] - spread.index[dataset_index]
+
+        interval_total_time = interval_to_total_time(interval)
+
+        if (span >= interval_total_time) or (dataset_index == 0):
+            ohlcv = bid_ask_to_ohlcv(
+                dataset=spread.iloc[dataset_index:], interval=interval
             )
 
-            return True
+            ohlcv_datasets[interval] = ohlcv
+        # end for
+    # end for
 
-        except ValueError:
-            return False
-        # end try
-    # end screener_in_market
+    for interval, ohlcv in ohlcv_datasets.items():
+        data: Dict[dt.datetime, Tuple[float, Dict[str, Any]]] = {}
 
-    def orderbook_screener_in_market(
-            self,
-            exchange: Optional[str] = None,
-            symbol: Optional[str] = None
-    ) -> bool:
-        """
-        Returns the data by according to the parameters.
+        for screener in ohlcv_screeners[interval]:
+            for index, row in ohlcv.iterrows():
+                index: dt.datetime
 
-        :param exchange: The exchange name.
-        :param symbol: The symbol name.
+                if index not in screener.ohlcv_market.index:
+                    screener.ohlcv_market.loc[index] = row
+                # end if
 
-        :return: The data.
-        """
+                data.setdefault(index, (index.timestamp(), row.to_dict()))
+            # end for
+        # end for
 
-        return self.screener_in_market(
-            exchange=exchange, symbol=symbol, base=OrderbookScreener
-        )
-    # end orderbook_screener_in_market
+        indexes[exchange][symbol][interval] = len(spread)
 
-    def orders_screener_in_market(
-            self,
-            exchange: Optional[str] = None,
-            symbol: Optional[str] = None
-    ) -> bool:
-        """
-        Returns the data by according to the parameters.
+        for callback in callbacks or []:
+            payload = callback_data(
+                data=list(data.values()), exchange=exchange,
+                symbol=symbol, interval=interval
+            )
 
-        :param exchange: The exchange name.
-        :param symbol: The symbol name.
+            await callback.record(payload, timestamp, key=OHLCVScreener.NAME)
+        # end if
 
-        :return: The data.
-        """
+    return True
+# end record_ohlcv
 
-        return self.screener_in_market(
-            exchange=exchange, symbol=symbol, base=OrdersScreener
-        )
-    # end orders_screener_in_market
+RecorderParameters = Dict[str, Union[Iterable[str], Dict[str, Callable]]]
 
-    def find_orderbook_screener(
-            self,
-            exchange: Optional[str] = None,
-            symbol: Optional[str] = None,
-            index: Optional[int] = None
-    ) -> OrderbookScreener:
-        """
-        Returns the data by according to the parameters.
+class OHLCVMarketRecorder(MarketRecorder):
+    """
+    A class to represent a crypto data feed recorder.
+    This object passes the record method to the handler object to record
+    the data fetched by the handler.
 
-        :param exchange: The exchange name.
-        :param symbol: The symbol name.
-        :param index: The index of the screener in the list.
+    Parameters:
 
-        :return: The data.
-        """
+    - screeners:
+        The screeners to record data into their market datasets.
 
-        return self.find_screener(
-            exchange=exchange, symbol=symbol,
-            base=OrderbookScreener, index=index
-        )
-    # end find_orderbook_screener
+    - callbacks:
+        The callbacks to run when collecting new data.
 
-    def find_orders_screener(
+    >>> from crypto_screening.market.screeners import OHLCVMarketRecorder
+    >>>
+    >>> recorder = OHLCVMarketRecorder(...)
+    """
+
+    COLUMNS = OHLCVScreener.COLUMNS
+
+    def __init__(
             self,
-            exchange: Optional[str] = None,
-            symbol: Optional[str] = None,
-            index: Optional[int] = None
-    ) -> OrdersScreener:
+            screeners: Iterable[BaseScreener],
+            callbacks: Optional[Iterable[Callback]] = None,
+    ) -> None:
         """
-        Returns the data by according to the parameters.
-
-        :param exchange: The exchange name.
-        :param symbol: The symbol name.
-        :param index: The index of the screener in the list.
+        Defines the class attributes.
 
-        :return: The data.
+        :param screeners: The screener objects.
+        :param callbacks: The callbacks for the service.
         """
 
-        return self.find_screener(
-            exchange=exchange, symbol=symbol,
-            base=OrdersScreener, index=index
-        )
-    # end find_orders_screener
+        super().__init__(screeners=screeners, callbacks=callbacks)
 
-    def find_orderbook_screeners(
-            self,
-            exchange: Optional[str] = None,
-            symbol: Optional[str] = None,
-            adjust: Optional[bool] = True
-    ) -> List[OrderbookScreener]:
-        """
-        Returns the data by according to the parameters.
+        self._indexes: Indexes = {}
+    # end __init__
 
-        :param exchange: The exchange name.
-        :param symbol: The symbol name.
-        :param adjust: The value to adjust for the screeners.
+    @property
+    def ohlcv_screeners(self) -> List[OHLCVScreener]:
+        """
+        Returns a list of all the order-book screeners.
 
-        :return: The data.
+        :return: The order-book screeners.
         """
 
-        return self.find_screeners(
-            exchange=exchange, symbol=symbol,
-            base=OrderbookScreener, adjust=adjust
-        )
-    # end find_orderbook_screener
+        return self.find_screeners(base=OHLCVScreener)
+    # end ohlcv_screeners
 
-    def find_orders_screeners(
-            self,
-            exchange: Optional[str] = None,
-            symbol: Optional[str] = None,
-            adjust: Optional[bool] = True
-    ) -> List[OrdersScreener]:
+    @property
+    def orderbook_screeners(self) -> List[OrderbookScreener]:
         """
-        Returns the data by according to the parameters.
+        Returns a list of all the ohlcv screeners.
+
+        :return: The ohlcv screeners.
+        """
+
+        return self.find_screeners(base=OrderbookScreener)
+    # end orderbook_screeners
 
-        :param exchange: The exchange name.
-        :param symbol: The symbol name.
-        :param adjust: The value to adjust for the screeners.
+    def parameters(self) -> RecorderParameters:
+        """
+        Returns the order book parameters.
 
-        :return: The data.
+        :return: The order book parameters.
         """
 
-        return self.find_screeners(
-            exchange=exchange, symbol=symbol,
-            base=OrdersScreener, adjust=adjust
+        return dict(
+            channels=[L2_BOOK],
+            callbacks={L2_BOOK: self.record},
+            max_depth=1
         )
-    # end find_orders_screeners
+    # end parameters
 
-    def ohlcv_screener_in_market(
-            self,
-            exchange: Optional[str] = None,
-            symbol: Optional[str] = None,
-            interval: Optional[str] = None
-    ) -> bool:
+    async def process(self, data: OrderBook, timestamp: float) -> bool:
         """
-        Returns the data by according to the parameters.
+        Records the data from the crypto feed into the dataset.
 
-        :param exchange: The exchange name.
-        :param symbol: The symbol name.
-        :param interval: The interval for the dataset.
-
-        :return: The data.
+        :param data: The data from the exchange.
+        :param timestamp: The time of the request.
         """
 
-        try:
-            self.find_ohlcv_screener(
-                exchange=exchange, symbol=symbol, interval=interval
+        exchange = data.exchange.lower()
+        symbol = adjust_symbol(symbol=data.symbol)
+
+        screeners = []
+
+        screeners.extend(
+            self.find_screeners(
+                base=OrderbookScreener, exchange=exchange, symbol=symbol
             )
+        )
+        screeners.extend(
+            self.find_screeners(
+                base=OHLCVScreener, exchange=exchange, symbol=symbol
+            )
+        )
 
-            return True
+        return await record_ohlcv(
+            screeners=screeners, data=data, indexes=self._indexes,
+            callbacks=self.callbacks, timestamp=timestamp
+        )
+    # end process
+# end MarketOHLCVRecorder
 
-        except ValueError:
-            return False
-    # end ohlcv_screener_in_market
+class OHLCVMarketScreener(MarketScreener):
+    """
+    A class to represent an asset price screener.
 
-    def trades_screener_in_market(
-            self,
-            exchange: Optional[str] = None,
-            symbol: Optional[str] = None
-    ) -> bool:
-        """
-        Returns the data by according to the parameters.
+    Using this class, you can create a screener object to
+    screen the market ask and bid data for a specific asset in
+    a specific exchange at real time.
 
-        :param exchange: The exchange name.
-        :param symbol: The symbol name.
+    Parameters:
 
-        :return: The data.
-        """
+    - screeners:
+        The screeners to connect to the market screener.
 
-        return self.screener_in_market(
-            exchange=exchange, symbol=symbol, base=TradesScreener
-        )
-    # end trades_screener_in_market
+    - intervals:
+        The structure to set a specific interval to the dataset
+        of each symbol in each exchange, matching the market data.
 
-    def find_ohlcv_screener(
-            self,
-            exchange: Optional[str] = None,
-            symbol: Optional[str] = None,
-            interval: Optional[str] = None,
-            index: Optional[int] = None
-    ) -> OHLCVScreener:
-        """
-        Returns the data by according to the parameters.
+    - location:
+        The saving location for the saved data of the screener.
 
-        :param exchange: The exchange name.
-        :param symbol: The symbol name.
-        :param interval: The interval for the dataset.
-        :param index: The index for the screener.
+    - cancel:
+        The time to cancel screening process after no new data is fetched.
 
-        :return: The data.
-        """
+    - delay:
+        The delay to wait between each data fetching.
 
-        return self.find_screener(
-            exchange=exchange, symbol=symbol, base=OHLCVScreener,
-            interval=interval, index=index
-        )
-    # end find_screeners
+    - handler:
+        The handler object to handle the data feed.
 
-    def find_trades_screener(
-            self,
-            exchange: Optional[str] = None,
-            symbol: Optional[str] = None,
-            index: Optional[int] = None
-    ) -> TradesScreener:
-        """
-        Returns the data by according to the parameters.
+    - recorder:
+        The recorder object to record the data of the market from the feed.
 
-        :param exchange: The exchange name.
-        :param symbol: The symbol name.
-        :param index: The index for the screener.
+    - screeners:
+        The screener object to control and fill with data.
 
-        :return: The data.
-        """
+    - refresh:
+        The duration of time between each refresh. 0 means no refresh.
 
-        return self.find_screener(
-            exchange=exchange, symbol=symbol, base=TradesScreener,
-            index=index
-        )
-    # end find_trades_screener
+    - amount:
+        The amount of symbols for each symbols group for an exchange.
 
-    def find_ohlcv_screeners(
-            self,
-            exchange: Optional[str] = None,
-            symbol: Optional[str] = None,
-            interval: Optional[str] = None,
-            adjust: Optional[bool] = True
-    ) -> List[OHLCVScreener]:
-        """
-        Returns the data by according to the parameters.
+    - limited:
+        The value to limit the running screeners to active exchanges.
+
+    >>> from crypto_screening.market.screeners import ohlcv_market_screener
+    >>>
+    >>> structure = {'1m': {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}}
+    >>>
+    >>> screener = ohlcv_market_screener(data=structure)
+    >>> screener.run()
+    """
+
+    screeners: List[Union[OHLCVScreener, OrderbookScreener]]
+    recorder: OHLCVMarketRecorder
 
-        :param exchange: The exchange name.
-        :param symbol: The symbol name.
-        :param interval: The interval for the datasets.
-        :param adjust: The value to adjust for the screeners.
+    COLUMNS = OHLCVMarketRecorder.COLUMNS
 
-        :return: The data.
+    def __init__(
+            self,
+            recorder: OHLCVMarketRecorder,
+            screeners: Optional[Iterable[Union[OHLCVScreener, OrderbookScreener]]] = None,
+            location: Optional[str] = None,
+            cancel: Optional[Union[float, dt.timedelta]] = None,
+            delay: Optional[Union[float, dt.timedelta]] = None,
+            refresh: Optional[Union[float, dt.timedelta, bool]] = None,
+            limited: Optional[bool] = None,
+            handler: Optional[MarketHandler] = None,
+            amount: Optional[int] = None
+    ) -> None:
         """
+        Creates the class attributes.
 
-        return self.find_screeners(
-            exchange=exchange, symbol=symbol, base=OHLCVScreener,
-            interval=interval, adjust=adjust
+        :param location: The saving location for the data.
+        :param delay: The delay for the process.
+        :param cancel: The cancel time for the loops.
+        :param limited: The value to limit the screeners to active only.
+        :param refresh: The refresh time for rerunning.
+        :param handler: The handler object for the market data.
+        :param amount: The maximum amount of symbols for each feed.
+        :param recorder: The recorder object for recording the data.
+        """
+
+        super().__init__(
+            location=location, cancel=cancel,
+            delay=delay, recorder=recorder,
+            screeners=screeners, handler=handler, limited=limited,
+            amount=amount, refresh=refresh
         )
-    # end find_ohlcv_screeners
+    # end __init__
 
-    def find_trades_screeners(
-            self,
-            exchange: Optional[str] = None,
-            symbol: Optional[str] = None,
-            adjust: Optional[bool] = True
-    ) -> List[TradesScreener]:
+    @property
+    def ohlcv_screeners(self) -> List[OHLCVScreener]:
+        """
+        Returns a list of all the ohlcv screeners.
+
+        :return: The ohlcv screeners.
         """
-        Returns the data by according to the parameters.
 
-        :param exchange: The exchange name.
-        :param symbol: The symbol name.
-        :param adjust: The value to adjust for the screeners.
+        return self.find_screeners(base=OHLCVScreener)
+    # end ohlcv_screeners
 
-        :return: The data.
+    @property
+    def orderbook_screeners(self) -> List[OrderbookScreener]:
         """
+        Returns a list of all the ohlcv screeners.
 
-        return self.find_screeners(
-            exchange=exchange, symbol=symbol, base=TradesScreener,
-            adjust=adjust
-        )
-    # end find_trades_screeners
-# end MappedScreenersContainer
+        :return: The ohlcv screeners.
+        """
+
+        return self.find_screeners(base=OrderbookScreener)
+    # end orderbook_screeners
+
+    def merge_screeners(self) -> None:
+        """Connects the screeners to the recording object."""
+
+        for ohlcv_screener in self.ohlcv_screeners:
+            for orderbook_screener in self.orderbook_screeners:
+                if (
+                    (ohlcv_screener.exchange == orderbook_screener.exchange) and
+                    (ohlcv_screener.symbol == orderbook_screener.symbol)
+                ):
+                    ohlcv_screener.orderbook_market = orderbook_screener.market
+                # end if
+            # end for
+        # end for
+    # end merge_screeners
+# end MarketOHLCVRecorder
+
+def create_ohlcv_screeners(
+        data: Dict[str, Union[Iterable[str], Dict[str, Iterable[str]]]],
+        location: Optional[str] = None,
+        cancel: Optional[Union[float, dt.timedelta]] = None,
+        delay: Optional[Union[float, dt.timedelta]] = None,
+) -> List[OHLCVScreener]:
+    """
+    Defines the class attributes.
+
+    :param data: The data for the screeners.
+    :param location: The saving location for the data.
+    :param cancel: The time to cancel the waiting.
+    :param delay: The delay for the process.
+    """
+
+    screeners = []
+
+    for exchange, symbols in data.items():
+        if isinstance(symbols, dict):
+            for symbol, intervals in symbols.items():
+                for interval in intervals:
+                    screeners.append(
+                        OHLCVScreener(
+                            symbol=symbol, exchange=exchange, delay=delay,
+                            location=location, cancel=cancel, interval=interval
+                        )
+                    )
+            # end for
+
+        else:
+            for symbol in symbols:
+                screeners.append(
+                    OHLCVScreener(
+                        symbol=symbol, exchange=exchange, delay=delay,
+                        location=location, cancel=cancel,
+                    )
+                )
+        # end if
+    # end for
+
+    return screeners
+# end create_ohlcv_screeners
+
+def ohlcv_market_screener(
+        data: Dict[str, Union[Iterable[str], Dict[str, Iterable[str]]]],
+        screeners: Optional[Iterable[OrderbookScreener]] = None,
+        location: Optional[str] = None,
+        cancel: Optional[Union[float, dt.timedelta]] = None,
+        delay: Optional[Union[float, dt.timedelta]] = None,
+        limited: Optional[bool] = None,
+        handler: Optional[MarketHandler] = None,
+        amount: Optional[int] = None,
+        callbacks: Optional[Iterable[Callback]] = None,
+        refresh: Optional[Union[float, dt.timedelta, bool]] = None,
+        recorder: Optional[OHLCVMarketRecorder] = None
+) -> OHLCVMarketScreener:
+    """
+    Creates the market screener object for the data.
+
+    :param data: The market data.
+    :param screeners: The base screeners.
+    :param handler: The handler object for the market data.
+    :param limited: The value to limit the screeners to active only.
+    :param refresh: The refresh time for rerunning.
+    :param amount: The maximum amount of symbols for each feed.
+    :param recorder: The recorder object for recording the data.
+    :param location: The saving location for the data.
+    :param delay: The delay for the process.
+    :param cancel: The cancel time for the loops.
+    :param callbacks: The callbacks for the service.
+
+    :return: The market screener object.
+    """
+
+    orderbook_screeners = (screeners or []) or create_orderbook_screeners(
+        data=data, location=location,
+        cancel=cancel, delay=delay
+    )
+
+    ohlcv_screeners = create_ohlcv_screeners(
+        data=data, location=location,
+        cancel=cancel, delay=delay
+    )
+
+    screeners = []
+    screeners.extend(orderbook_screeners)
+    screeners.extend(ohlcv_screeners)
+
+    market = OHLCVMarketScreener(
+        recorder=recorder or OHLCVMarketRecorder(
+            screeners=screeners, callbacks=callbacks
+        ), screeners=screeners,
+        handler=handler, location=location, amount=amount,
+        cancel=cancel, delay=delay, limited=limited, refresh=refresh
+    )
+
+    market.merge_screeners()
+
+    return market
+# end orderbook_market_recorder
```

### Comparing `crypto-screening-7.5.6/crypto_screening/market/screeners/database.py` & `crypto-screening-8.0.0/crypto_screening/market/screeners/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-8.0.0/crypto_screening/market/screeners/recorder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,285 +1,246 @@
-# orderbook.py
+# recorder.py
 
+import warnings
+import threading
+import time
+from abc import ABCMeta, abstractmethod
 import datetime as dt
 from typing import (
-    Dict, Optional, Iterable, Any, Union, List, Callable
+    Optional, Dict, Any, List,
+    Iterable, Type, Union
 )
+from functools import partial
+import asyncio
 
-import pandas as pd
-
-from sqlalchemy import Engine
+from represent import Modifiers, represent
 
 from cryptofeed import FeedHandler
-from cryptofeed.types import OrderBook
-from cryptofeed.defines import L2_BOOK
+from cryptofeed.feed import Feed
 
-from crypto_screening.symbols import adjust_symbol
 from crypto_screening.process import find_string_value
-from crypto_screening.dataset import (
-    BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME, create_dataset, ORDERBOOK_COLUMNS
+from crypto_screening.exchanges import EXCHANGES, EXCHANGE_NAMES
+from crypto_screening.symbols import adjust_symbol
+from crypto_screening.market.screeners.base import (
+    BaseMarketScreener, BaseScreener, BaseScreenersContainer
 )
-from crypto_screening.market.screeners.base import BaseScreener
-from crypto_screening.market.screeners.callbacks import Callback, callback_data
-from crypto_screening.market.screeners.recorder import MarketScreener, MarketRecorder
+from crypto_screening.market.screeners.callbacks import Callback
 
 __all__ = [
-    "OrderbookMarketScreener",
-    "OrderbookMarketRecorder",
-    "OrderbookScreener",
-    "create_orderbook_market",
-    "orderbook_market_screener",
-    "orderbook_market_recorder",
-    "create_orderbook_market_dataset",
-    "record_orderbook"
+    "MarketHandler",
+    "ExchangeFeed",
+    "FEED_GROUP_SIZE",
+    "add_feeds",
+    "MarketScreener",
+    "MarketRecorder"
 ]
 
-Market = Dict[str, Dict[str, pd.DataFrame]]
+class MarketHandler(FeedHandler):
+    """A class to handle the market data feed."""
 
-def create_orderbook_market_dataset() -> pd.DataFrame:
-    """
-    Creates a dataframe for the order book data.
+    def __init__(self) -> None:
+        """Defines the class attributes."""
 
-    :return: The dataframe.
-    """
+        super().__init__(
+            config={'uvloop': False, 'log': {'disabled': True}}
+        )
+    # end __init__
+# end MarketHandler
 
-    return create_dataset(
-        columns=OrderbookMarketRecorder.COLUMNS
-    )
-# end create_orderbook_market_dataset
+class ExchangeFeed(Feed):
+    """A class to represent an exchange feed object."""
 
-def create_orderbook_market(data: Dict[str, Iterable[str]]) -> Market:
-    """
-    Creates the dataframes of the market data.
+    handler: Optional[MarketHandler] = None
 
-    :param data: The market data.
+    running: bool = False
 
-    :return: The dataframes of the market data.
-    """
+    def stop(self) -> None:
+        """Stops the process."""
 
-    return {
-        exchange.lower(): {
-            symbol.upper(): create_orderbook_market_dataset()
-            for symbol in data[exchange]
-        } for exchange in data
-    }
-# end create_orderbook_market
+        self.running = False
 
-class OrderbookScreener(BaseScreener):
-    """
-    A class to represent an asset price screener.
+        Feed.stop(self)
+    # end stop
 
-    Using this class, you can create a screener object to
-    screen the market ask and bid data for a specific asset in
-    a specific exchange at real time.
+    def start(self, loop: asyncio.AbstractEventLoop) -> None:
+        """
+        Create tasks for exchange interfaces and backends.
 
-    Parameters:
+        :param loop: The event loop for the process.
+        """
 
-    - symbol:
-        The symbol of an asset to screen.
+        self.running = True
 
-    - exchange:
-        The key of the exchange platform to screen data from.
+        Feed.start(self, loop=loop)
+    # end start
+# end ExchangeFeed
 
-    - location:
-        The saving location for the saved data of the screener.
 
-    - cancel:
-        The time to cancel screening process after no new data is fetched.
+FEED_GROUP_SIZE = 20
 
-    - delay:
-        The delay to wait between each data fetching.
+def add_feeds(
+        handler: MarketHandler,
+        data: Dict[str, Iterable[str]],
+        fixed: Optional[bool] = False,
+        amount: Optional[int] = FEED_GROUP_SIZE,
+        parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
+) -> None:
+    """
+    Adds the symbols to the handler for each exchange.
 
-    - market:
-        The dataset of the market data as BID/ASK spread.
+    :param handler: The handler object.
+    :param data: The data of the exchanges and symbols to add.
+    :param parameters: The parameters for the exchanges.
+    :param fixed: The value for fixed parameters to all exchanges.
+    :param amount: The maximum amount of symbols for each feed.
     """
 
-    NAME = "ORDERBOOK"
+    base_parameters = None
 
-    COLUMNS = ORDERBOOK_COLUMNS
+    if not fixed:
+        parameters = parameters or {}
 
-    @property
-    def orderbook_market(self) -> pd.DataFrame:
-        """
-        Returns the market to hold the recorder data.
+    else:
+        base_parameters = parameters or {}
+        parameters = {}
+    # end if
 
-        :return: The market object.
-        """
+    for exchange, symbols in data.items():
+        exchange = find_string_value(value=exchange, values=EXCHANGE_NAMES)
 
-        return self.market
-    # end orderbook_market
-# end OrderbookScreener
+        symbols = [adjust_symbol(symbol, separator='-') for symbol in symbols]
 
-async def record_orderbook(
-        market: Market,
-        data: OrderBook,
-        timestamp: float,
-        callbacks: Optional[Iterable[Callback]] = None
-) -> bool:
-    """
-    Records the data from the crypto feed into the dataset.
+        if fixed:
+            parameters.setdefault(exchange, base_parameters)
+        # end if
 
-    :param market: The market structure.
-    :param data: The data from the exchange.
-    :param timestamp: The time of the request.
-    :param callbacks: The callbacks for the service.
+        EXCHANGES[exchange]: Type[ExchangeFeed]
 
-    :return: The validation value.
-    """
+        groups = []
 
-    exchange = find_string_value(
-        value=data.exchange, values=market.keys()
-    )
-    symbol = find_string_value(
-        value=adjust_symbol(symbol=data.symbol),
-        values=exchange
-    )
-
-    dataset = (
-        market.
-        setdefault(exchange, {}).
-        setdefault(symbol, create_orderbook_market_dataset())
-    )
-
-    try:
-        index = dt.datetime.fromtimestamp(timestamp)
-
-        if index in dataset.index:
-            return False
-        # end if
-
-        bids = data.book.bids.to_list()
-        asks = data.book.asks.to_list()
-
-        data = {
-            BIDS: float(bids[0][0]),
-            ASKS: float(asks[0][0]),
-            BIDS_VOLUME: float(bids[0][1]),
-            ASKS_VOLUME: float(asks[0][1])
-        }
-
-        dataset.loc[index] = data
-
-        for callback in callbacks or []:
-            payload = callback_data(
-                data=[(timestamp, data)], exchange=exchange, symbol=symbol
-            )
+        for i in range(0, int(len(symbols) / amount) + len(symbols) % amount, amount):
+            groups.append(symbols[i:])
+        # end for
 
-            await callback.record(payload, timestamp, key=OrderbookScreener.NAME)
-        # end if
+        for symbols_packet in groups:
+            exchange_parameters = (
+                parameters[exchange]
+                if (
+                    (exchange in parameters) and
+                    isinstance(parameters[exchange], dict) and
+                    all(isinstance(key, str) for key in parameters)
+                ) else {}
+            )
 
-        return True
+            feed = EXCHANGES[exchange](symbols=symbols_packet, **exchange_parameters)
 
-    except IndexError:
-        return False
-    # end try
-# end record_orderbook
+            feed.start = partial(ExchangeFeed.start, feed)
+            feed.stop = partial(ExchangeFeed.stop, feed)
+            feed.handler = handler
+            feed.running = False
 
-RecorderParameters = Dict[str, Union[Iterable[str], Dict[str, Callable]]]
+            handler.add_feed(feed)
+        # end for
+    # end for
+# end add_feeds
 
-class OrderbookMarketRecorder(MarketRecorder):
+@represent
+class MarketRecorder(BaseScreenersContainer, metaclass=ABCMeta):
     """
     A class to represent a crypto data feed recorder.
     This object passes the record method to the handler object to record
     the data fetched by the handler.
 
     Parameters:
 
-    - market:
-        The market structure of the data to store the fetched data in.
-        This structure is a dictionary with exchange names as keys
-        and dictionaries as values, where their keys are symbols,
-        and their values are the dataframes to record the data.
+    - screeners:
+        The screeners to record data into their market datasets.
 
-    - databases:
-        The databases and their engines for storing data in databases.
+    - callbacks:
+        The callbacks to run when collecting new data.
 
-    >>> from crypto_screening.market.screeners import orderbook_market_recorder
+    >>> from crypto_screening.market.screeners.recorder import MarketRecorder
     >>>
     >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
-    >>> recorder = orderbook_market_recorder(data=market)
-    """
+    >>> recorder = MarketRecorder(data=market)
 
-    COLUMNS = OrderbookScreener.COLUMNS
+    """
 
-    @property
-    def orderbook_market(self) -> Market:
+    def __init__(
+            self,
+            screeners: Iterable[BaseScreener],
+            callbacks: Optional[Iterable[Callback]] = None
+    ) -> None:
         """
-        Returns the market to hold the recorder data.
+        Defines the class attributes.
 
-        :return: The market object.
+        :param screeners: The screeners to record.
+        :param callbacks: The callbacks for the service.
         """
 
-        return self.market
-    # end orderbook_market
+        super().__init__(screeners=screeners)
+
+        self.callbacks = callbacks or []
+
+        self._disabled = False
+    # end __init__
+
+    @property
+    def disabled(self) -> bool:
+        """Returns the value for the recorder to run."""
+
+        return self._disabled
+    # end disabled
 
-    def parameters(self) -> RecorderParameters:
+    @abstractmethod
+    def parameters(self) -> Dict[str, Any]:
         """
         Returns the order book parameters.
 
         :return: The order book parameters.
         """
-
-        return dict(
-            channels=[L2_BOOK],
-            callbacks={L2_BOOK: self.record},
-            max_depth=1
-        )
     # end parameters
 
-    def orderbook(self, exchange: str, symbol: str) -> pd.DataFrame:
-        """
-        Returns the market data of the symbol from the exchange.
+    def disable(self) -> None:
+        """Stops the recorder."""
 
-        :param exchange: The source key of the exchange.
-        :param symbol: The symbol of the pair.
+        self._disabled = True
+    # end disable
 
-        :return: The dataset of the spread data.
-        """
+    def enable(self) -> None:
+        """Starts the recorder."""
 
-        return self.data(exchange=exchange, symbol=symbol)
-    # end orderbook
+        self._disabled = False
+    # end disable
 
-    def orderbook_in_market(self, exchange: str, symbol: str) -> bool:
+    async def process(self, data: Any, timestamp: float) -> bool:
         """
-        Returns the market data of the symbol from the exchange.
-
-        :param exchange: The source key of the exchange.
-        :param symbol: The symbol of the pair.
+        Records the data from the crypto feed into the dataset.
 
-        :return: The dataset of the spread data.
+        :param data: The data from the exchange.
+        :param timestamp: The time of the request.
         """
+    # end process
 
-        try:
-            self.orderbook(exchange=exchange, symbol=symbol)
-
-            return True
-
-        except ValueError:
-            return False
-        # end try
-    # end orderbook_in_market
-
-    async def record(self, data: OrderBook, timestamp: float) -> bool:
+    async def record(self, data: Any, timestamp: float):
         """
         Records the data from the crypto feed into the dataset.
 
         :param data: The data from the exchange.
         :param timestamp: The time of the request.
         """
 
-        return await record_orderbook(
-            market=self.market, data=data,
-            callbacks=self.callbacks, timestamp=timestamp
-        )
+        if not self.disabled:
+            await self.process(data=data, timestamp=timestamp)
+        # end if
     # end record
-# end MarketOrderbookRecorder
+# end MarketRecorder
 
-class OrderbookMarketScreener(MarketScreener):
+class MarketScreener(BaseMarketScreener):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
@@ -307,38 +268,37 @@
         The duration of time between each refresh. 0 means no refresh.
 
     - amount:
         The amount of symbols for each symbols group for an exchange.
 
     - limited:
         The value to limit the running screeners to active exchanges.
-
-    >>> from crypto_screening.market.screeners import orderbook_market_screener
-    >>>
-    >>> structure = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
-    >>>
-    >>> screener = orderbook_market_screener(data=structure)
-    >>> screener.run()
     """
 
-    screeners: List[OrderbookScreener]
-    recorder: OrderbookMarketRecorder
+    __modifiers__ = Modifiers()
+    __modifiers__.excluded.append('handler')
 
-    COLUMNS = OrderbookMarketRecorder.COLUMNS
+    screeners: List[BaseScreener]
+    recorder: MarketRecorder
+
+    DELAY = 1
+    AMOUNT = FEED_GROUP_SIZE
+
+    REFRESH = dt.timedelta(minutes=10)
 
     def __init__(
             self,
-            recorder: OrderbookMarketRecorder,
-            screeners: Optional[Iterable[OrderbookScreener]] = None,
+            recorder: MarketRecorder,
+            screeners: Optional[Iterable[BaseScreener]] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None,
             refresh: Optional[Union[float, dt.timedelta, bool]] = None,
             limited: Optional[bool] = None,
-            handler: Optional[FeedHandler] = None,
+            handler: Optional[MarketHandler] = None,
             amount: Optional[int] = None
     ) -> None:
         """
         Creates the class attributes.
 
         :param location: The saving location for the data.
         :param delay: The delay for the process.
@@ -348,224 +308,291 @@
         :param handler: The handler object for the market data.
         :param amount: The maximum amount of symbols for each feed.
         :param recorder: The recorder object for recording the data.
         """
 
         super().__init__(
             location=location, cancel=cancel,
-            delay=delay, recorder=recorder,
-            screeners=screeners, handler=handler, limited=limited,
-            amount=amount, refresh=refresh
+            delay=delay, screeners=screeners
         )
 
-        self.screeners[:] = screeners or self.create_orderbook_screeners()
+        if refresh is True:
+            refresh = self.REFRESH
+        # end if
+
+        self.recorder = recorder
+        self.handler = handler or MarketHandler()
+        self.limited = limited or False
+        self.amount = amount or self.AMOUNT
+        self.refresh = refresh
+
+        self.loop: Optional[asyncio.AbstractEventLoop] = None
+
+        self._feeds_parameters: Optional[Dict[str, Any]] = None
+        self._run_parameters: Optional[Dict[str, Any]] = None
     # end __init__
 
-    @property
-    def orderbook_market(self) -> Market:
-        """
-        Returns the market to hold the recorder data.
+    def update_screeners(self) -> None:
+        """Updates the records of the object."""
 
-        :return: The market object.
-        """
+        super().update_screeners()
 
-        return self.recorder.orderbook_market
-    # end orderbook_market
+        self.recorder.update_screeners()
+    # end update_screeners
 
-    @property
-    def orderbook_screeners(self) -> List[OrderbookScreener]:
+    def add_feeds(
+            self,
+            data: Optional[Dict[str, Iterable[str]]] = None,
+            fixed: Optional[bool] = True,
+            amount: Optional[int] = None,
+            parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
+    ) -> None:
         """
-        Returns a list of all the order-book screeners.
+        Adds the symbols to the handler for each exchange.
 
-        :return: The order-book screeners.
+        :param data: The data of the exchanges and symbols to add.
+        :param parameters: The parameters for the exchanges.
+        :param fixed: The value for fixed parameters to all exchanges.
+        :param amount: The maximum amount of symbols for each feed.
         """
 
-        return [
-            screener for screener in self.screeners
-            if isinstance(screener, OrderbookScreener)
-        ]
-    # end orderbook_screeners
+        if data is None:
+            data = self.structure()
+        # end if
 
-    def connect_screeners(self) -> None:
-        """Connects the screeners to the recording object."""
+        self._feeds_parameters = dict(
+            data=data, fixed=fixed, parameters=parameters, amount=amount
+        )
 
-        for screener in self.screeners:
-            if isinstance(screener, OrderbookScreener):
-                screener.market = self.orderbook(
-                    exchange=screener.exchange, symbol=screener.symbol
-                )
-            # end if
-        # end for
-    # end connect_screeners
+        feed_params = self.recorder.parameters()
+        feed_params.update(parameters or {})
 
-    def orderbook(self, exchange: str, symbol: str) -> pd.DataFrame:
-        """
-        Returns the market data of the symbol from the exchange.
+        add_feeds(
+            self.handler, data=data, fixed=fixed,
+            parameters=feed_params, amount=amount or self.amount
+        )
+    # end add_feeds
 
-        :param exchange: The source key of the exchange.
-        :param symbol: The symbol of the pair.
+    def refresh_feeds(self) -> None:
+        """Refreshes the feed objects."""
 
-        :return: The dataset of the spread data.
-        """
+        if self._feeds_parameters is None:
+            warnings.warn(
+                "Cannot refresh feeds as there was "
+                "no feeds initialization to repeat."
+            )
 
-        return self.recorder.orderbook(exchange=exchange, symbol=symbol)
-    # end orderbook
+            return
+        # end if
 
-    def orderbook_in_market(self, exchange: str, symbol: str) -> bool:
-        """
-        Returns the market data of the symbol from the exchange.
+        self.handler.feeds.clear()
 
-        :param exchange: The source key of the exchange.
-        :param symbol: The symbol of the pair.
+        self.add_feeds(**self._feeds_parameters)
+    # end refresh
 
-        :return: The dataset of the spread data.
-        """
+    def rerun(self) -> None:
+        """Refreshes the process."""
+
+        if self._run_parameters is None:
+            warnings.warn(
+                "Cannot rerun as there was "
+                "no initial process to repeat."
+            )
+
+            return
+        # end if
 
-        return self.recorder.orderbook_in_market(exchange=exchange, symbol=symbol)
-    # end orderbook_in_market
+        self.terminate()
+        self.refresh_feeds()
+        self.run(**self._run_parameters)
+    # end rerun
 
-    def create_orderbook_screener(
+    def screening_loop(
             self,
-            symbol: str,
-            exchange: str,
-            location: Optional[str] = None,
-            cancel: Optional[Union[float, dt.timedelta]] = None,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            container: Optional[Dict[str, Dict[str, OrderbookScreener]]] = None
-    ) -> OrderbookScreener:
+            start: Optional[bool] = True,
+            loop: Optional[asyncio.AbstractEventLoop] = None
+    ) -> None:
         """
-        Defines the class attributes.
+        Runs the process of the price screening.
 
-        :param symbol: The symbol of the asset.
-        :param exchange: The exchange to get source data from.
-        :param location: The saving location for the data.
-        :param cancel: The time to cancel the waiting.
-        :param delay: The delay for the process.
-        :param container: The container to contain the new screener.
+        :param start: The value to start the loop.
+        :param loop: The event loop.
         """
 
-        if container is None:
-            container = {}
+        if loop is None:
+            loop = asyncio.new_event_loop()
         # end if
 
-        if cancel is None:
-            cancel = self.cancel
-        # end if
+        self.loop = loop
 
-        if delay is None:
-            delay = self.delay
+        asyncio.set_event_loop(loop)
+
+        self._screening = True
+
+        for screener in self.screeners:
+            screener._screening = True
+        # end for
+
+        if self._feeds_parameters is None:
+            self.add_feeds()
         # end if
 
-        screener = OrderbookScreener(
-            symbol=symbol, exchange=exchange, delay=delay,
-            location=location, cancel=cancel, market=(
-                self.orderbook(exchange=exchange, symbol=symbol)
-                if self.orderbook_in_market(symbol=symbol, exchange=exchange)
-                else None
-            )
+        self.handler.run(
+            start_loop=start and (not loop.is_running()),
+            install_signal_handlers=False
         )
+    # end screening_loop
 
-        container.setdefault(exchange, {})[symbol] = screener
+    def saving_loop(self) -> None:
+        """Runs the process of the price screening."""
 
-        return screener
-    # end create_orderbook_screener
+        for screener in self.screeners:
+            screener._saving_process = threading.Thread(
+                target=screener.saving_loop
+            )
+            screener._saving_process.start()
+        # end for
+    # end saving_loop
 
-    def create_orderbook_screeners(
-            self,
-            location: Optional[str] = None,
-            cancel: Optional[Union[float, dt.timedelta]] = None,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            container: Optional[Dict[str, Dict[str, OrderbookScreener]]] = None
-    ) -> List[OrderbookScreener]:
-        """
-        Defines the class attributes.
+    def update_loop(self) -> None:
+        """Updates the state of the screeners."""
 
-        :param location: The saving location for the data.
-        :param cancel: The time to cancel the waiting.
-        :param delay: The delay for the process.
-        :param container: The container to contain the new screeners.
-        """
+        self._updating = True
+
+        refresh = self.refresh
+
+        if isinstance(refresh, dt.timedelta):
+            refresh = refresh.total_seconds()
+        # end if
 
-        screeners = []
+        start = time.time()
 
-        for exchange, symbols in self.structure().items():
-            for symbol in symbols:
-                screeners.append(
-                    self.create_orderbook_screener(
-                        symbol=symbol, exchange=exchange, delay=delay,
-                        location=location, cancel=cancel, container=container
-                    )
-                )
+        while self.updating:
+            s = time.time()
+
+            if self.screening:
+                self.update()
+
+                current = time.time()
+
+                if refresh and ((current - start) >= refresh):
+                    self.rerun()
+
+                    start = current
+                # end if
+            # end if
+
+            time.sleep(max([self.delay - (time.time() - s), 0]))
+        # end while
+    # end update_loop
+
+    def update(self) -> None:
+        """Updates the state of the screeners."""
+
+        for screener in self.screeners:
+            for feed in self.handler.feeds:
+                feed: ExchangeFeed
+
+                if (
+                    self.limited and
+                    (screener.exchange.lower() == feed.id.lower()) and
+                    (not feed.running)
+                ):
+                    screener.stop()
+                # end if
             # end for
         # end for
+    # end update
 
-        return screeners
-    # end create_orderbook_screeners
-# end MarketOrderbookScreener
+    def stop_screening(self) -> None:
+        """Stops the screening process."""
 
-Databases = Union[Iterable[str], Dict[str, Engine]]
+        super().stop_screening()
 
-def orderbook_market_recorder(data: Dict[str, Iterable[str]]) -> OrderbookMarketRecorder:
-    """
-    Creates the market recorder object for the data.
+        self.loop: asyncio.AbstractEventLoop
 
-    :param data: The market data.
+        async def stop() -> None:
+            """Stops the handler."""
 
-    :return: The market recorder object.
-    """
+            self.handler.stop(self.loop)
+            self.handler.close(self.loop)
+        # end stop
 
-    return OrderbookMarketRecorder(
-        market=create_orderbook_market(data=data)
-    )
-# end orderbook_market_recorder
+        self.loop.create_task(stop())
 
-def orderbook_market_screener(
-        data: Dict[str, Iterable[str]],
-        location: Optional[str] = None,
-        cancel: Optional[Union[float, dt.timedelta]] = None,
-        delay: Optional[Union[float, dt.timedelta]] = None,
-        limited: Optional[bool] = None,
-        handler: Optional[FeedHandler] = None,
-        market: Optional[Market] = None,
-        amount: Optional[int] = None,
-        callbacks: Optional[Iterable[Callback]] = None,
-        refresh: Optional[Union[float, dt.timedelta, bool]] = None,
-        recorder: Optional[OrderbookMarketRecorder] = None,
-        fixed: Optional[bool] = True,
-        parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
-) -> OrderbookMarketScreener:
-    """
-    Creates the market screener object for the data.
+        for task in asyncio.all_tasks(self.loop):
+            task.cancel()
+        # end for
 
-    :param data: The market data.
-    :param handler: The handler object for the market data.
-    :param limited: The value to limit the screeners to active only.
-    :param parameters: The parameters for the exchanges.
-    :param market: The object to fill with the crypto feed record.
-    :param fixed: The value for fixed parameters to all exchanges.
-    :param refresh: The refresh time for rerunning.
-    :param amount: The maximum amount of symbols for each feed.
-    :param recorder: The recorder object for recording the data.
-    :param location: The saving location for the data.
-    :param delay: The delay for the process.
-    :param cancel: The cancel time for the loops.
-    :param callbacks: The callbacks for the service.
+        self.loop = None
 
-    :return: The market screener object.
-    """
+        self.handler.running = False
+    # end stop_screening
+
+    def start_screening(
+            self,
+            start: Optional[bool] = True,
+            loop: Optional[asyncio.AbstractEventLoop] = None
+    ) -> None:
+        """
+        Starts the screening process.
 
-    screener = OrderbookMarketScreener(
-        recorder=recorder or OrderbookMarketRecorder(
-            market=market or create_orderbook_market(data=data),
-            callbacks=callbacks
-        ),
-        handler=handler, location=location, amount=amount,
-        cancel=cancel, delay=delay, limited=limited, refresh=refresh
-    )
-
-    screener.add_feeds(
-        data=screener.recorder.structure(),
-        fixed=fixed, parameters=parameters
-    )
+        :param start: The value to start the loop.
+        :param loop: The event loop.
+        """
+
+        if self.screening:
+            warnings.warn(f"Timeout screening of {self} is already running.")
 
-    return screener
-# end orderbook_market_recorder
+            return
+        # end if
+
+        self._screening_process = threading.Thread(
+            target=lambda: self.screening_loop(loop=loop, start=start)
+        )
+
+        self._screening_process.start()
+    # end start_screening
+
+    def run(
+            self,
+            save: Optional[bool] = True,
+            block: Optional[bool] = False,
+            update: Optional[bool] = True,
+            screen: Optional[bool] = True,
+            loop: Optional[asyncio.AbstractEventLoop] = None,
+            wait: Optional[Union[bool, float, dt.timedelta, dt.datetime]] = False,
+            timeout: Optional[Union[float, dt.timedelta, dt.datetime]] = None,
+    ) -> None:
+        """
+        Runs the program.
+
+        :param save: The value to save the data.
+        :param wait: The value to wait after starting to run the process.
+        :param block: The value to block the execution.
+        :param timeout: The valur to add a start_timeout to the process.
+        :param update: The value to update the screeners.
+        :param screen: The value to start the loop.
+        :param loop: The event loop.
+
+        :return: The start_timeout process.
+        """
+
+        self._run_parameters = dict(
+            save=save, block=block, update=update, screen=screen,
+            loop=loop, wait=wait, timeout=timeout,
+        )
+
+        if not block:
+            self.start_screening(loop=loop, start=screen)
+        # end if
+
+        super().run(
+            screen=False, block=False, wait=wait,
+            timeout=timeout, update=update, save=save
+        )
+
+        if block:
+            self.screening_loop(loop=loop, start=screen)
+        # end if
+    # end run
+# end MarketScreener
```

### Comparing `crypto-screening-7.5.6/crypto_screening/market/screeners/recorder.py` & `crypto-screening-8.0.0/crypto_screening/market/screeners/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,739 +1,774 @@
-# recorder.py
+# base.py
 
-import warnings
-import threading
-import time
 import datetime as dt
-from typing import (
-    Optional, Dict, Any, List,
-    Iterable, Type, Union
-)
-from functools import partial
-import asyncio
+import time
+from abc import ABCMeta
+from typing import Iterable, List, Type, TypeVar, Optional, Dict, Union, Any
 
 import pandas as pd
 
 from represent import Modifiers, represent
 
-from cryptofeed import FeedHandler
-from cryptofeed.feed import Feed
+from multithreading import Caller, multi_threaded_call
 
-from crypto_screening.validate import validate_exchange, validate_symbol
-from crypto_screening.process import find_string_value
-from crypto_screening.exchanges import EXCHANGES, EXCHANGE_NAMES
+from crypto_screening.dataset import save_dataset, load_dataset, create_dataset
 from crypto_screening.symbols import adjust_symbol
-from crypto_screening.market.screeners.base import BaseMarketScreener, BaseScreener
-from crypto_screening.market.screeners.callbacks import Callback
+from crypto_screening.validate import validate_exchange, validate_symbol
+from crypto_screening.collect.symbols import all_exchange_symbols
+from crypto_screening.market.foundation.state import WaitingState
+from crypto_screening.market.foundation.data import DataCollector
+from crypto_screening.market.foundation.protocols import BaseScreenerProtocol
+from crypto_screening.market.foundation.waiting import (
+    base_await_initialization, base_await_dynamic_initialization,
+    base_await_dynamic_update, base_await_update
+)
 
 __all__ = [
-    "MarketHandler",
-    "ExchangeFeed",
-    "FEED_GROUP_SIZE",
-    "add_feeds",
-    "MarketScreener",
-    "structure_screeners_datasets",
-    "structure_screener_datasets",
-    "MarketRecorder",
-    "validate_market"
+    "BaseScreener",
+    "BaseMarketScreener",
+    "BaseScreenersContainer",
+    "screeners_table",
+    "BaseFrozenScreenersContainer"
 ]
 
-class MarketHandler(FeedHandler):
-    """A class to handle the market data feed."""
-
-    def __init__(self) -> None:
-        """Defines the class attributes."""
-
-        super().__init__(
-            config={'uvloop': False, 'log': {'disabled': True}}
-        )
-    # end __init__
-# end MarketHandler
-
-class ExchangeFeed(Feed):
-    """A class to represent an exchange feed object."""
-
-    handler: Optional[FeedHandler] = None
-
-    running: bool = False
-
-    def stop(self) -> None:
-        """Stops the process."""
-
-        self.running = False
-
-        Feed.stop(self)
-    # end stop
+class BaseScreener(DataCollector):
+    """
+    A class to represent an asset price screener.
 
-    def start(self, loop: asyncio.AbstractEventLoop) -> None:
-        """
-        Create tasks for exchange interfaces and backends.
+    Using this class, you can create a screener object to
+    screen the market ask and bid data for a specific asset in
+    a specific exchange at real time.
 
-        :param loop: The event loop for the process.
-        """
+    Parameters:
 
-        self.running = True
+    - symbol:
+        The symbol of an asset to screen.
 
-        Feed.start(self, loop=loop)
-    # end start
-# end ExchangeFeed
+    - exchange:
+        The key of the exchange platform to screen data from.
 
+    - location:
+        The saving location for the saved data of the screener.
 
-FEED_GROUP_SIZE = 20
+    - cancel:
+        The time to cancel screening process after no new data is fetched.
 
-def add_feeds(
-        handler: FeedHandler,
-        data: Dict[str, Iterable[str]],
-        fixed: Optional[bool] = False,
-        amount: Optional[int] = FEED_GROUP_SIZE,
-        parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
-) -> None:
-    """
-    Adds the symbols to the handler for each exchange.
+    - delay:
+        The delay to wait between each data fetching.
 
-    :param handler: The handler object.
-    :param data: The data of the exchanges and symbols to add.
-    :param parameters: The parameters for the exchanges.
-    :param fixed: The value for fixed parameters to all exchanges.
-    :param amount: The maximum amount of symbols for each feed.
+    - market:
+        The dataset of the market data.
     """
 
-    base_parameters = None
-
-    if not fixed:
-        parameters = parameters or {}
-
-    else:
-        base_parameters = parameters or {}
-        parameters = {}
-    # end if
-
-    for exchange, symbols in data.items():
-        exchange = find_string_value(value=exchange, values=EXCHANGE_NAMES)
+    __modifiers__ = Modifiers()
+    __modifiers__.hidden.append("market")
 
-        symbols = [adjust_symbol(symbol, separator='-') for symbol in symbols]
+    MINIMUM_DELAY = 1
 
-        if fixed:
-            parameters.setdefault(exchange, base_parameters)
-        # end if
+    NAME: Optional[str] = "BASE"
+    COLUMNS: Iterable[str] = []
 
-        EXCHANGES[exchange]: Type[ExchangeFeed]
+    SCREENER_NAME_TYPE_MATCHES: Dict[str, Any] = {}
+    SCREENER_TYPE_NAME_MATCHES: Dict[Any, str] = {}
 
-        packets = []
+    def __init__(
+            self,
+            symbol: str,
+            exchange: str,
+            location: Optional[str] = None,
+            cancel: Optional[Union[float, dt.timedelta]] = None,
+            delay: Optional[Union[float, dt.timedelta]] = None,
+            market: Optional[pd.DataFrame] = None,
+    ) -> None:
+        """
+        Defines the class attributes.
 
-        for i in range(0, int(len(symbols) / amount) + len(symbols) % amount, amount):
-            packets.append(symbols[i:])
-        # end for
+        :param symbol: The symbol of the asset.
+        :param exchange: The exchange to get source data from.
+        :param location: The saving location for the data.
+        :param delay: The delay for the process.
+        :param cancel: The cancel time for the loops.
+        :param market: The data for the market.
+        """
 
-        for symbols_packet in packets:
-            exchange_parameters = (
-                parameters[exchange]
-                if (
-                    (exchange in parameters) and
-                    isinstance(parameters[exchange], dict) and
-                    all(isinstance(key, str) for key in parameters)
-                ) else {}
+        if not self.COLUMNS:
+            raise ValueError(
+                f"{repr(self)} must define a non-empty "
+                f"'COLUMNS' instance or class attribute."
             )
-
-            feed = EXCHANGES[exchange](symbols=symbols_packet, **exchange_parameters)
-
-            feed.start = partial(ExchangeFeed.start, feed)
-            feed.stop = partial(ExchangeFeed.stop, feed)
-            feed.handler = handler
-            feed.running = False
-
-            handler.add_feed(feed)
-        # end for
-    # end for
-# end add_feeds
-
-Market = Dict[str, Dict[str, Any]]
-
-def validate_market(data: Any) -> Market:
-    """
-    Validates the data.
-
-    :param data: The data to validate.
-
-    :return: The valid data.
-    """
-
-    try:
-        if not isinstance(data, dict):
-            raise ValueError
         # end if
 
-        for exchange, values in data.items():
-            if not (
-                isinstance(exchange, str) and
-                (
-                    isinstance(values, dict) and
-                    all(
-                        isinstance(symbol, str)
-                        for symbol, _ in values.items()
-                    )
-                )
-            ):
-                raise ValueError
-            # end if
-        # end for
-
-    except (TypeError, ValueError):
-        raise ValueError(
-            f"Data must be of type {Market}, not: {data}."
-        )
-    # end try
+        super().__init__(location=location, cancel=cancel, delay=delay)
 
-    return data
-# end validate_market
+        self.SCREENER_NAME_TYPE_MATCHES.setdefault(self.NAME, type(self))
+        self.SCREENER_TYPE_NAME_MATCHES.setdefault(type(self), self.NAME)
 
-@represent
-class MarketRecorder:
-    """
-    A class to represent a crypto data feed recorder.
-    This object passes the record method to the handler object to record
-    the data fetched by the handler.
+        self.exchange = self.validate_exchange(exchange=exchange)
+        self.symbol = self.validate_symbol(exchange=self.exchange, symbol=symbol)
 
-    Parameters:
+        if market is None:
+            market = create_dataset(self.COLUMNS)
+        # end if
 
-    - market:
-        The market structure of the data to store the fetched data in.
-        This structure is a dictionary with exchange names as keys
-        and dictionaries as values, where their keys are symbols,
-        and their values are the dataframes to record the data.
+        self.market = market
+    # end __init__
 
-    - databases:
-        The databases and their engines for storing data in databases.
+    def await_initialization(
+            self,
+            stop: Optional[Union[bool, int]] = False,
+            delay: Optional[Union[float, dt.timedelta]] = None,
+            cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
+    ) -> WaitingState[BaseScreenerProtocol]:
+        """
+        Waits for all the create_screeners to update.
 
-    >>> from crypto_screening.market.screeners.recorder import MarketRecorder
-    >>>
-    >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
-    >>>
-    >>> recorder = MarketRecorder(data=market)
+        :param delay: The delay for the waiting.
+        :param stop: The value to stop the screener objects.
+        :param cancel: The time to cancel the waiting.
 
-    """
+        :returns: The total delay.
+        """
 
-    __modifiers__ = Modifiers()
-    __modifiers__.hidden.append("market")
+        self: Union[BaseScreener, BaseScreenerProtocol]
 
-    __slots__ = "market", "databases", 'callbacks'
+        return base_await_initialization(
+            self, stop=stop, delay=delay, cancel=cancel
+        )
+    # end await_initialization
 
-    def __init__(
+    def await_update(
             self,
-            market: Market,
-            callbacks: Optional[Iterable[Callback]] = None
-    ) -> None:
+            stop: Optional[Union[bool, int]] = False,
+            delay: Optional[Union[float, dt.timedelta]] = None,
+            cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
+    ) -> WaitingState[BaseScreenerProtocol]:
         """
-        Defines the class attributes.
+        Waits for all the create_screeners to update.
 
-        :param market: The object to fill with the crypto feed record.
-        :param callbacks: The callbacks for the service.
+        :param delay: The delay for the waiting.
+        :param stop: The value to stop the screener objects.
+        :param cancel: The time to cancel the waiting.
+
+        :returns: The total delay.
         """
 
-        self.market = self.validate_market(data=market)
+        self: Union[BaseScreener, BaseScreenerProtocol]
 
-        self.callbacks = callbacks or []
-    # end __init__
+        return base_await_update(
+            self, stop=stop, delay=delay, cancel=cancel
+        )
+    # end await_update
 
     @staticmethod
-    def validate_market(data: Any) -> Market:
+    def validate_exchange(exchange: str) -> str:
         """
-        Validates the data.
+        Validates the symbol value.
 
-        :param data: The data to validate.
+        :param exchange: The exchange key.
 
-        :return: The valid data.
+        :return: The validates symbol.
         """
 
-        return validate_market(data=data)
-    # end validate_market
+        return validate_exchange(exchange=exchange)
+    # end validate_exchange
 
-    def parameters(self) -> Dict[str, Any]:
+    @staticmethod
+    def validate_symbol(exchange: str, symbol: Any) -> str:
         """
-        Returns the order book parameters.
+        Validates the symbol value.
+
+        :param exchange: The exchange key.
+        :param symbol: The key of the symbol.
 
-        :return: The order book parameters.
+        :return: The validates symbol.
         """
 
-        raise NotImplemented
-    # end parameters
+        return validate_symbol(
+            exchange=exchange, symbol=symbol,
+            symbols=all_exchange_symbols(exchange=exchange)
+        )
+    # end validate_symbol
 
-    def structure(self) -> Dict[str, List[str]]:
+    def dataset_path(self, location: Optional[str] = None) -> str:
         """
-        Returns the structure of the market data.
+        Creates the path to the saving file for the screener object.
 
-        :return: The structure of the market.
+        :param location: The saving location of the dataset.
+
+        :return: The saving path for the dataset.
         """
 
-        return {
-            exchange: list(symbols.keys())
-            for exchange, symbols in self.market.items()
-        }
-    # end structure
+        location = location or self.location
 
-    def data(self, exchange: str, symbol: str) -> Any:
-        """
-        Returns the market data of the symbol from the exchange.
+        if location is None:
+            location = "."
+        # end if
 
-        :param exchange: The source key of the exchange.
-        :param symbol: The symbol of the pair.
+        return (
+            f"{location}/"
+            f"{self.exchange.lower()}/"
+            f"{self.NAME}-"
+            f"{adjust_symbol(self.symbol, separator='-')}.csv"
+        )
+    # end dataset_path
 
-        :return: The dataset of the spread data.
+    def save_dataset(self, location: Optional[str] = None) -> None:
         """
+        Saves the data of the screener.
 
-        exchange = find_string_value(
-            value=exchange, values=self.market.keys()
-        )
+        :param location: The saving location of the dataset.
+        """
 
-        validate_exchange(
-            exchange=exchange,
-            exchanges=self.market.keys(),
-            provider=self
-        )
+        if len(self.market) == 0:
+            return
+        # end if
 
-        validate_symbol(
-            symbol=symbol,
-            exchange=exchange,
-            exchanges=self.market.keys(),
-            symbols=self.market[exchange],
-            provider=self
+        save_dataset(
+            dataset=self.market,
+            path=self.dataset_path(location=location)
         )
+    # end save_dataset
 
-        return self.market[exchange][symbol]
-    # end data
-
-    def in_market(self, exchange: str, symbol: str) -> bool:
+    def load_dataset(self, location: Optional[str] = None) -> None:
         """
-        Returns the market data of the symbol from the exchange.
-
-        :param exchange: The source key of the exchange.
-        :param symbol: The symbol of the pair.
+        Saves the data of the screener.
 
-        :return: The dataset of the spread data.
+        :param location: The saving location of the dataset.
         """
 
-        try:
-            self.data(exchange=exchange, symbol=symbol)
+        data = load_dataset(path=self.dataset_path(location=location))
 
-            return True
+        for index, data in zip(data.index[:], data.loc[:]):
+            self.market.loc[index] = data
+        # end for
+    # end load_dataset
 
-        except ValueError:
-            return False
-        # end try
-    # end in_market
-# end MarketRecorder
+    def saving_loop(self) -> None:
+        """Runs the process of the price screening."""
 
-class MarketScreener(BaseMarketScreener):
-    """
-    A class to represent an asset price screener.
+        self._saving = True
 
-    Using this class, you can create a screener object to
-    screen the market ask and bid data for a specific asset in
-    a specific exchange at real time.
+        delay = self.delay
 
-    Parameters:
+        if isinstance(self.delay, dt.timedelta):
+            delay = delay.total_seconds()
+        # end if
 
-    - location:
-        The saving location for the saved data of the screener.
+        while self.saving:
+            start = time.time()
 
-    - cancel:
-        The time to cancel screening process after no new data is fetched.
+            self.save_dataset()
 
-    - delay:
-        The delay to wait between each data fetching.
+            end = time.time()
 
-    - handler:
-        The handler object to handle the data feed.
+            time.sleep(max([delay - (end - start), self.MINIMUM_DELAY]))
+        # end while
+    # end saving_loop
+# end BaseScreener
 
-    - recorder:
-        The recorder object to record the data of the market from the feed.
+_S = TypeVar("_S")
 
-    - screeners:
-        The screener object to control and fill with data.
+ScreenersTable = Dict[
+    Optional[Type[BaseScreener]],
+    Dict[
+        Optional[str],
+        Dict[Optional[str], Dict[Optional[str], List[BaseScreener]]]
+    ]
+]
 
-    - refresh:
-        The duration of time between each refresh. 0 means no refresh.
+def screeners_table(
+        screeners: Iterable[BaseScreener],
+        table: Optional[ScreenersTable] = None
+) -> ScreenersTable:
+    """
+    Inserts all the screeners into the table.
 
-    - amount:
-        The amount of symbols for each symbols group for an exchange.
+    :param screeners: The screeners to insert into the table.
+    :param table: The table to use for the data.
 
-    - limited:
-        The value to limit the running screeners to active exchanges.
+    :return: The screeners table.
     """
 
-    __modifiers__ = Modifiers(**BaseMarketScreener.__modifiers__)
-    __modifiers__.excluded.append('handler')
+    if table is None:
+        table = {}
+    # end if
 
-    __slots__ = (
-        "handler", 'amount', "loop", "limited", "_feeds_parameters",
-        "_run_parameters", 'refresh', 'recorder'
-    )
+    for screener in screeners:
+        for interval in {
+            (
+                screener.interval
+                if hasattr(screener, "interval") else
+                None
+            ), None
+        }:
+            lists = [
+                (
+                    table.
+                    setdefault(type(screener), {}).
+                    setdefault(screener.exchange, {}).
+                    setdefault(screener.symbol, {}).
+                    setdefault(interval, [])
+                ),
+                (
+                    table.
+                    setdefault(type(screener), {}).
+                    setdefault(screener.exchange, {}).
+                    setdefault(None, {}).
+                    setdefault(interval, [])
+                ),
+                (
+                    table.
+                    setdefault(type(screener), {}).
+                    setdefault(None, {}).
+                    setdefault(screener.symbol, {}).
+                    setdefault(interval, [])
+                ),
+                (
+                    table.
+                    setdefault(type(screener), {}).
+                    setdefault(None, {}).
+                    setdefault(None, {}).
+                    setdefault(interval, [])
+                ),
+                (
+                    table.
+                    setdefault(type(screener), {}).
+                    setdefault(None, {}).
+                    setdefault(None, {}).
+                    setdefault(None, [])
+                ),
+                (
+                    table.
+                    setdefault(None, {}).
+                    setdefault(screener.exchange, {}).
+                    setdefault(screener.symbol, {}).
+                    setdefault(interval, [])
+                ),
+                (
+                    table.
+                    setdefault(None, {}).
+                    setdefault(screener.exchange, {}).
+                    setdefault(None, {}).
+                    setdefault(interval, [])
+                ),
+                (
+                    table.
+                    setdefault(None, {}).
+                    setdefault(None, {}).
+                    setdefault(screener.symbol, {}).
+                    setdefault(interval, [])
+                ),
+                (
+                    table.
+                    setdefault(None, {}).
+                    setdefault(None, {}).
+                    setdefault(None, {}).
+                    setdefault(interval, [])
+                )
+            ]
 
-    screeners: List[BaseScreener]
-    recorder: MarketRecorder
+            for screeners_list in lists:
+                if screener not in screeners_list:
+                    screeners_list.append(screener)
+                # end if
+            # end for
+        # end for
+    # end for
 
-    DELAY = 1
-    AMOUNT = FEED_GROUP_SIZE
+    return table
+# end screeners_table
 
-    REFRESH = dt.timedelta(minutes=5)
+@represent
+class BaseFrozenScreenersContainer:
+    """
+    A class to represent a multi-exchange multi-pairs crypto data screener.
+    Using this class enables extracting screener objects and screeners
+    data by the exchange name and the symbol of the pair.
 
-    def __init__(
-            self,
-            recorder: Union[MarketRecorder, Any],
-            screeners: Optional[Iterable[BaseScreener]] = None,
-            location: Optional[str] = None,
-            cancel: Optional[Union[float, dt.timedelta]] = None,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            refresh: Optional[Union[float, dt.timedelta, bool]] = None,
-            limited: Optional[bool] = None,
-            handler: Optional[FeedHandler] = None,
-            amount: Optional[int] = None
-    ) -> None:
-        """
-        Creates the class attributes.
+    parameters:
 
-        :param location: The saving location for the data.
-        :param delay: The delay for the process.
-        :param cancel: The cancel time for the loops.
-        :param limited: The value to limit the screeners to active only.
-        :param refresh: The refresh time for rerunning.
-        :param handler: The handler object for the market data.
-        :param amount: The maximum amount of symbols for each feed.
-        :param recorder: The recorder object for recording the data.
-        """
+    - screeners:
+        The screener objects to form a market.
 
-        super().__init__(
-            location=location, cancel=cancel,
-            delay=delay, screeners=screeners
-        )
+    >>> from crypto_screening.market.screeners.base import BaseFrozenScreenersContainer
+    >>> from crypto_screening.market.screeners.base import BaseScreener
+    >>>
+    >>> container = BaseFrozenScreenersContainer(
+    >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
+    >>> )
+    """
 
-        if refresh is True:
-            refresh = self.REFRESH
-        # end if
+    def __init__(self, screeners: Iterable[BaseScreener]) -> None:
+        """
+        Defines the class attributes.
 
-        self.recorder = recorder
-        self.handler = handler or MarketHandler()
-        self.limited = limited or False
-        self.amount = amount or self.AMOUNT
-        self.refresh = refresh
+        :param screeners: The data screener object.
+        """
 
-        self.loop: Optional[asyncio.AbstractEventLoop] = None
+        self._screeners = list(screeners)
 
-        self._feeds_parameters: Optional[Dict[str, Any]] = None
-        self._run_parameters: Optional[Dict[str, Any]] = None
+        self._table = screeners_table(self.screeners)
     # end __init__
 
-    def connect_screeners(self) -> None:
-        """Connects the screeners to the recording object."""
-    # end connect_screeners
+    @property
+    def screeners(self) -> List[BaseScreener]:
+        """
+        Returns a list of all the screeners.
+
+        :return: The screeners.
+        """
+
+        return list(self._screeners)
+    # end screeners
 
     def structure(self) -> Dict[str, List[str]]:
         """
         Returns the structure of the market data.
 
         :return: The structure of the market.
         """
 
-        return self.recorder.structure()
+        return {
+            exchange: list([symbol for symbol in symbols if symbol is not None])
+            for exchange, symbols in self._table[None].items()
+            if exchange is not None
+        }
     # end structure
 
-    def add_feeds(
+    def find_screeners(
             self,
-            data: Optional[Dict[str, Iterable[str]]] = None,
-            fixed: Optional[bool] = True,
-            amount: Optional[int] = None,
-            parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
-    ) -> None:
-        """
-        Adds the symbols to the handler for each exchange.
+            exchange: Optional[str] = None,
+            symbol: Optional[str] = None,
+            base: Optional[Type[_S]] = None,
+            interval: Optional[str] = None,
+            adjust: Optional[bool] = True
+    ) -> List[_S]:
+        """
+        Returns the data by according to the parameters.
+
+        :param base: The base type of the screener.
+        :param exchange: The exchange name.
+        :param symbol: The symbol name.
+        :param interval: The interval for the search.
+        :param adjust: The value to adjust for the screeners.
 
-        :param data: The data of the exchanges and symbols to add.
-        :param parameters: The parameters for the exchanges.
-        :param fixed: The value for fixed parameters to all exchanges.
-        :param amount: The maximum amount of symbols for each feed.
+        :return: The data.
         """
 
-        if data is None:
-            data = self.structure()
-        # end if
+        try:
+            return list(self._table[base][exchange][symbol][interval])
 
-        self._feeds_parameters = dict(
-            data=data, fixed=fixed, parameters=parameters
-        )
+        except KeyError:
+            if not adjust:
+                raise ValueError(
+                    f"Cannot find screeners  matching to "
+                    f"type - {base}, exchange - {exchange}, "
+                    f"symbol - {symbol}, interval - {interval} "
+                    f"inside {repr(self)}"
+                )
+            # end if
+        # end try
 
-        feed_params = self.recorder.parameters()
-        feed_params.update(parameters or {})
+        return []
+    # end find_screeners
 
-        add_feeds(
-            self.handler, data=data, fixed=fixed,
-            parameters=feed_params, amount=amount or self.amount
-        )
-    # end add_feeds
+    def find_screener(
+            self,
+            exchange: Optional[str] = None,
+            symbol: Optional[str] = None,
+            base: Optional[Type[_S]] = None,
+            interval: Optional[str] = None,
+            index: Optional[int] = None,
+            adjust: Optional[bool] = True
+    ) -> _S:
+        """
+        Returns the data by according to the parameters.
+
+        :param base: The base type of the screener.
+        :param exchange: The exchange name.
+        :param symbol: The symbol name.
+        :param interval: The interval for the search.
+        :param index: The index of the screener in the list.
+        :param adjust: The value to adjust for the screeners.
+
+        :return: The data.
+        """
+
+        try:
+            return self.find_screeners(
+                exchange=exchange, symbol=symbol,
+                base=base, interval=interval, adjust=adjust
+            )[index or 0]
+
+        except IndexError:
+            if not adjust:
+                raise IndexError(
+                    f"Cannot find screeners matching to "
+                    f"type - {base}, exchange - {exchange}, "
+                    f"symbol - {symbol}, interval - {interval}, "
+                    f"index - {index} inside {repr(self)}"
+                )
+            # end if
+        # end try
+    # end find_orderbook_screener
 
-    def refresh_feeds(self) -> None:
-        """Refreshes the feed objects."""
+    def screener_in_market(
+            self,
+            exchange: Optional[str] = None,
+            symbol: Optional[str] = None,
+            base: Optional[Type[_S]] = None,
+            interval: Optional[str] = None
+    ) -> bool:
+        """
+        Returns the data by according to the parameters.
+
+        :param base: The base type of the screener.
+        :param exchange: The exchange name.
+        :param symbol: The symbol name.
+        :param interval: The interval to search.
 
-        if self._feeds_parameters is None:
-            warnings.warn(
-                "Cannot refresh feeds as there was "
-                "no feeds initialization to repeat."
+        :return: The data.
+        """
+
+        try:
+            self.find_screener(
+                exchange=exchange, symbol=symbol,
+                base=base, interval=interval
             )
 
-            return
-        # end if
+            return True
 
-        self.handler.feeds.clear()
+        except ValueError:
+            return False
+        # end try
+    # end screener_in_market
+# end MappedScreenersContainer
 
-        self.add_feeds(**self._feeds_parameters)
-    # end refresh
+@represent
+class BaseScreenersContainer(BaseFrozenScreenersContainer):
+    """
+    A class to represent a multi-exchange multi-pairs crypto data screener.
+    Using this class enables extracting screener objects and screeners
+    data by the exchange name and the symbol of the pair.
 
-    def rerun(self) -> None:
-        """Refreshes the process."""
+    parameters:
 
-        if self._run_parameters is None:
-            warnings.warn(
-                "Cannot rerun as there was "
-                "no initial process to repeat."
-            )
+    - screeners:
+        The screener objects to form a market.
 
-            return
-        # end if
+    >>> from crypto_screening.market.screeners.base import BaseScreenersContainer
+    >>> from crypto_screening.market.screeners.base import BaseScreener
+    >>>
+    >>> container = BaseScreenersContainer(
+    >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
+    >>> )
+    """
 
-        self.terminate()
-        self.refresh_feeds()
-        self.run(**self._run_parameters)
-    # end rerun
+    def update_screeners(self) -> None:
+        """Updates the records of the object."""
+    # end update_screeners
 
-    def screening_loop(
+    def add(
             self,
-            start: Optional[bool] = True,
-            loop: Optional[asyncio.AbstractEventLoop] = None
+            screeners: Iterable[BaseScreener],
+            adjust: Optional[bool] = True,
+            update: Optional[bool] = True
     ) -> None:
         """
-        Runs the process of the price screening.
+        Updates the data with the new screeners.
 
-        :param start: The value to start the loop.
-        :param loop: The event loop.
+        :param screeners: The new screeners to add.
+        :param adjust: The value to adjust for screeners.
+        :param update: The value to update.
         """
 
-        if loop is None:
-            loop = asyncio.new_event_loop()
-        # end if
-
-        self.loop = loop
-
-        asyncio.set_event_loop(loop)
-
-        self._screening = True
-
-        for screener in self.screeners:
-            screener._screening = True
-        # end for
-
-        self.handler.run(
-            start_loop=start and (not loop.is_running()),
-            install_signal_handlers=False
-        )
-    # end screening_loop
+        new_screeners = []
 
-    def saving_loop(self) -> None:
-        """Runs the process of the price screening."""
+        for screener in screeners:
+            if screener not in self._screeners:
+                new_screeners.append(screener)
 
-        for screener in self.screeners:
-            screener._saving_process = threading.Thread(
-                target=screener.saving_loop
-            )
-            screener._saving_process.start()
+            elif not adjust:
+                raise ValueError(
+                    f"Cannot add screener {repr(screener)} to "
+                    f"{repr(self)} because it is already present."
+                )
+            # end if
         # end for
-    # end saving_loop
 
-    def update_loop(self) -> None:
-        """Updates the state of the screeners."""
+        self._screeners.extend(new_screeners)
 
-        self._updating = True
+        screeners_table(new_screeners, table=self._table)
 
-        refresh = self.refresh
-
-        if isinstance(refresh, dt.timedelta):
-            refresh = refresh.total_seconds()
+        if update:
+            self.update_screeners()
         # end if
+    # end update
 
-        start = time.time()
-
-        while self.updating:
-            s = time.time()
-
-            if self.screening:
-                self.update()
+    def remove(
+            self,
+            screeners: Iterable[BaseScreener],
+            adjust: Optional[bool] = True,
+            update: Optional[bool] = True
+    ) -> None:
+        """
+        Updates the data with the new screeners.
 
-                current = time.time()
+        :param screeners: The new screeners to add.
+        :param adjust: The value to adjust for screeners.
+        :param update: The value to update.
+        """
 
-                if refresh and ((current - start) >= refresh):
-                    self.rerun()
+        for screener in screeners:
+            if screener in self._screeners:
+                self._screeners.remove(screener)
 
-                    start = current
-                # end if
+            elif not adjust:
+                raise ValueError(
+                    f"Cannot remove screener {repr(screener)} from "
+                    f"{repr(self)} because it is not present."
+                )
             # end if
-
-            time.sleep(max([self.delay - (time.time() - s), 0]))
-        # end while
-    # end update_loop
-
-    def update(self) -> None:
-        """Updates the state of the screeners."""
-
-        for screener in self.screeners:
-            for feed in self.handler.feeds:
-                feed: ExchangeFeed
-
-                if (
-                    self.limited and
-                    (screener.exchange.lower() == feed.id.lower()) and
-                    (not feed.running)
-                ):
-                    screener.stop()
-                # end if
-            # end for
         # end for
-    # end update
 
-    def stop_screening(self) -> None:
-        """Stops the screening process."""
+        self._table.clear()
+
+        screeners_table(self._screeners, table=self._table)
 
-        super().stop_screening()
+        if update:
+            self.update_screeners()
+        # end if
+    # end remove
+# end BaseScreenersContainer
 
-        self.loop: asyncio.AbstractEventLoop
+class BaseMarketScreener(DataCollector, BaseScreenersContainer, metaclass=ABCMeta):
+    """
+    A class to represent an asset price screener.
 
-        async def stop() -> None:
-            """Stops the handler."""
+    Using this class, you can create a screener object to
+    screen the market ask and bid data for a specific asset in
+    a specific exchange at real time.
 
-            self.handler.stop(self.loop)
-            self.handler.close(self.loop)
-        # end stop
+    Parameters:
 
-        self.loop.create_task(stop())
+    - location:
+        The saving location for the saved data of the screener.
 
-        for task in asyncio.all_tasks(self.loop):
-            task.cancel()
-        # end for
+    - cancel:
+        The time to cancel screening process after no new data is fetched.
 
-        self.loop = None
+    - delay:
+        The delay to wait between each data fetching.
 
-        self.handler.running = False
-    # end stop_screening
+    - screeners:
+        The screener object to control and fill with data.
+    """
 
-    def start_screening(
+    def __init__(
             self,
-            start: Optional[bool] = True,
-            loop: Optional[asyncio.AbstractEventLoop] = None
+            screeners: Optional[Iterable[BaseScreener]] = None,
+            location: Optional[str] = None,
+            cancel: Optional[Union[float, dt.timedelta]] = None,
+            delay: Optional[Union[float, dt.timedelta]] = None
     ) -> None:
         """
-        Starts the screening process.
+        Defines the class attributes.
 
-        :param start: The value to start the loop.
-        :param loop: The event loop.
+        :param location: The saving location for the data.
+        :param delay: The delay for the process.
+        :param cancel: The cancel time for the loops.
         """
 
-        if self.screening:
-            warnings.warn(f"Timeout screening of {self} is already running.")
+        DataCollector.__init__(self, location=location, cancel=cancel, delay=delay)
 
-            return
-        # end if
+        BaseScreenersContainer.__init__(self, screeners=screeners)
+    # end __init__
 
-        self._screening_process = threading.Thread(
-            target=lambda: self.screening_loop(loop=loop, start=start)
-        )
+    def await_initialization(
+            self,
+            stop: Optional[Union[bool, int]] = False,
+            delay: Optional[Union[float, dt.timedelta]] = None,
+            cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
+    ) -> WaitingState[BaseScreener]:
+        """
+        Waits for all the create_screeners to update.
 
-        self._screening_process.start()
-    # end start_screening
+        :param delay: The delay for the waiting.
+        :param stop: The value to stop the screener objects.
+        :param cancel: The time to cancel the waiting.
 
-    def run(
-            self,
-            save: Optional[bool] = True,
-            block: Optional[bool] = False,
-            update: Optional[bool] = True,
-            screen: Optional[bool] = True,
-            loop: Optional[asyncio.AbstractEventLoop] = None,
-            wait: Optional[Union[bool, float, dt.timedelta, dt.datetime]] = False,
-            timeout: Optional[Union[float, dt.timedelta, dt.datetime]] = None,
-    ) -> None:
+        :returns: The total delay.
         """
-        Runs the program.
 
-        :param save: The value to save the data.
-        :param wait: The value to wait after starting to run the process.
-        :param block: The value to block the execution.
-        :param timeout: The valur to add a start_timeout to the process.
-        :param update: The value to update the screeners.
-        :param screen: The value to start the loop.
-        :param loop: The event loop.
-
-        :return: The start_timeout process.
-        """
-
-        self._run_parameters = dict(
-            save=save, block=block, update=update, screen=screen,
-            loop=loop, wait=wait, timeout=timeout,
+        return base_await_dynamic_initialization(
+            self.screeners, stop=stop, delay=delay, cancel=cancel
         )
+    # end await_initialization
 
-        if not block:
-            self.start_screening(loop=loop, start=screen)
-        # end if
+    def await_update(
+            self,
+            stop: Optional[Union[bool, int]] = False,
+            delay: Optional[Union[float, dt.timedelta]] = None,
+            cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
+    ) -> WaitingState[BaseScreener]:
+        """
+        Waits for all the create_screeners to update.
 
-        super().run(
-            screen=False, block=False, wait=wait,
-            timeout=timeout, update=update, save=save
-        )
+        :param delay: The delay for the waiting.
+        :param stop: The value to stop the screener objects.
+        :param cancel: The time to cancel the waiting.
 
-        if block:
-            self.screening_loop(loop=loop, start=screen)
-        # end if
-    # end run
-# end MarketScreener
+        :returns: The total delay.
+        """
 
-def structure_screeners_datasets(
-        screeners: Iterable[BaseScreener]
-) -> Dict[str, Dict[str, List[pd.DataFrame]]]:
-    """
-    Structures the screener objects by exchanges and symbols
+        return base_await_dynamic_update(
+            self.screeners, stop=stop, delay=delay, cancel=cancel
+        )
+    # end await_update
 
-    :param screeners: The screeners to structure.
+    def save_datasets(self, location: Optional[str] = None) -> None:
+        """
+        Runs the data handling loop.
 
-    :return: The structure of the screeners.
-    """
+        :param location: The saving location.
+        """
 
-    structure = {}
+        callers = []
 
-    for screener in screeners:
-        (
-            structure.
-            setdefault(screener.exchange, {}).
-            setdefault(screener.symbol, [])
-        ).append(screener.market)
-    # end for
+        for screener in self.screeners:
+            location = location or screener.location or self.location
 
-    return structure
-# end structure_screeners_datasets
+            callers.append(
+                Caller(
+                    target=screener.save_dataset,
+                    kwargs=dict(location=location)
+                )
+            )
+        # end for
 
-def structure_screener_datasets(
-        screeners: Iterable[BaseScreener]
-) -> Dict[str, Dict[str, pd.DataFrame]]:
-    """
-    Structures the screener objects by exchanges and symbols
+        multi_threaded_call(callers=callers)
+    # end save_datasets
 
-    :param screeners: The screeners to structure.
+    def load_datasets(self, location: Optional[str] = None) -> None:
+        """
+        Runs the data handling loop.
 
-    :return: The structure of the screeners.
-    """
+        :param location: The saving location.
+        """
 
-    structure = {}
+        callers = []
 
-    for screener in screeners:
-        (
-            structure.
-            setdefault(screener.exchange, {}).
-            setdefault(screener.symbol, screener.market)
-        )
-    # end for
+        for screener in self.screeners:
+            location = location or screener.location or self.location
+
+            callers.append(
+                Caller(
+                    target=screener.load_dataset,
+                    kwargs=dict(location=location)
+                )
+            )
+        # end for
 
-    return structure
-# end structure_screener_datasets
+        multi_threaded_call(callers=callers)
+    # end load_datasets
+# end BaseMarketScreener
```

### Comparing `crypto-screening-7.5.6/crypto_screening/market/screeners/trades.py` & `crypto-screening-8.0.0/crypto_screening/market/screeners/trades.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,51 @@
 # trades.py
 
 import datetime as dt
 from typing import (
-    Dict, Optional, Iterable, Any, Union, List, Callable
+    Dict, Optional, Iterable, Union, List, Callable
 )
 
 import pandas as pd
 
-from sqlalchemy import Engine
-
-from cryptofeed import FeedHandler
 from cryptofeed.types import Trade
 from cryptofeed.defines import TRADES
 
 from crypto_screening.symbols import adjust_symbol
-from crypto_screening.process import find_string_value
 from crypto_screening.dataset import (
     TRADES_COLUMNS, create_dataset, AMOUNT, PRICE, SIDE
 )
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.callbacks import Callback, callback_data
-from crypto_screening.market.screeners.recorder import MarketScreener, MarketRecorder
+from crypto_screening.market.screeners.recorder import (
+    MarketScreener, MarketRecorder, MarketHandler
+)
 
 __all__ = [
     "TradesMarketScreener",
     "TradesMarketRecorder",
     "TradesScreener",
-    "create_trades_market",
     "trades_market_screener",
-    "trades_market_recorder",
     "create_trades_market_dataset",
-    "record_trades"
+    "record_trades",
+    "create_trades_screeners"
 ]
 
-Market = Dict[str, Dict[str, pd.DataFrame]]
-
 def create_trades_market_dataset() -> pd.DataFrame:
     """
     Creates a dataframe for the order book data.
 
     :return: The dataframe.
     """
 
     return create_dataset(
         columns=TradesMarketRecorder.COLUMNS
     )
 # end create_trades_market_dataset
 
-def create_trades_market(data: Dict[str, Iterable[str]]) -> Market:
-    """
-    Creates the dataframes of the market data.
-
-    :param data: The market data.
-
-    :return: The dataframes of the market data.
-    """
-
-    return {
-        exchange.lower(): {
-            symbol.upper(): create_trades_market_dataset()
-            for symbol in data[exchange]
-        } for exchange in data
-    }
-# end create_trades_market
-
 class TradesScreener(BaseScreener):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
@@ -106,65 +84,65 @@
         """
 
         return self.market
     # end trades_market
 # end TradesScreener
 
 async def record_trades(
-        market: Market,
+        screeners: Iterable[TradesScreener],
         data: Trade,
         timestamp: float,
         callbacks: Optional[Iterable[Callback]] = None
 ) -> bool:
     """
     Records the data from the crypto feed into the dataset.
 
-    :param market: The market structure.
+    :param screeners: The screeners.
     :param data: The data from the exchange.
     :param timestamp: The time of the request.
     :param callbacks: The callbacks for the service.
 
     :return: The validation value.
     """
 
-    exchange = find_string_value(
-        value=data.exchange, values=market.keys()
-    )
-    symbol = find_string_value(
-        value=adjust_symbol(symbol=data.symbol),
-        values=exchange
-    )
-
-    dataset = (
-        market.
-        setdefault(exchange, {}).
-        setdefault(symbol, create_trades_market_dataset())
-    )
+    exchange = data.exchange.lower()
+    symbol = adjust_symbol(symbol=data.symbol)
 
     try:
         index = dt.datetime.fromtimestamp(timestamp)
 
-        if index in dataset.index:
-            return False
-        # end if
-
         data = {
             AMOUNT: float(data.amount),
             PRICE: float(data.price),
             SIDE: data.side
         }
 
-        dataset.loc[index] = data
+        valid = False
 
-        for callback in callbacks or []:
-            payload = callback_data(
-                data=[(timestamp, data)], exchange=exchange, symbol=symbol
-            )
+        for screener in screeners:
+            if index in screener.market.index:
+                continue
+            # end if
+
+            valid = True
+
+            screener.market.loc[index] = data
+        # end for
 
-            await callback.record(payload, timestamp, key=TradesScreener.NAME)
+        if valid:
+            for callback in callbacks or []:
+                payload = callback_data(
+                    data=[(timestamp, data)],
+                    exchange=exchange, symbol=symbol
+                )
+
+                await callback.record(
+                    payload, timestamp, key=TradesScreener.NAME
+                )
+            # end if
         # end if
 
         return True
 
     except IndexError:
         return False
     # end try
@@ -176,42 +154,37 @@
     """
     A class to represent a crypto data feed recorder.
     This object passes the record method to the handler object to record
     the data fetched by the handler.
 
     Parameters:
 
-    - market:
-        The market structure of the data to store the fetched data in.
-        This structure is a dictionary with exchange names as keys
-        and dictionaries as values, where their keys are symbols,
-        and their values are the dataframes to record the data.
+    - screeners:
+        The screeners to record data into their market datasets.
 
-    - databases:
-        The databases and their engines for storing data in databases.
+    - callbacks:
+        The callbacks to run when collecting new data.
 
-    >>> from crypto_screening.market.screeners import orderbook_market_recorder
+    >>> from crypto_screening.market.screeners import TradesMarketRecorder
     >>>
-    >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
-    >>>
-    >>> recorder = orderbook_market_recorder(data=market)
+    >>> recorder = TradesMarketRecorder(...)
     """
 
     COLUMNS = TradesScreener.COLUMNS
 
     @property
-    def trades_market(self) -> Market:
+    def trades_screeners(self) -> List[TradesScreener]:
         """
-        Returns the market to hold the recorder data.
+        Returns a list of all the order-book screeners.
 
-        :return: The market object.
+        :return: The order-book screeners.
         """
 
-        return self.market
-    # end trades_market
+        return self.find_screeners(base=TradesScreener)
+    # end trades_screeners
 
     def parameters(self) -> RecorderParameters:
         """
         Returns the order book parameters.
 
         :return: The order book parameters.
         """
@@ -219,62 +192,33 @@
         return dict(
             channels=[TRADES],
             callbacks={TRADES: self.record},
             max_depth=1
         )
     # end parameters
 
-    def trades(self, exchange: str, symbol: str) -> pd.DataFrame:
-        """
-        Returns the market data of the symbol from the exchange.
-
-        :param exchange: The source key of the exchange.
-        :param symbol: The symbol of the pair.
-
-        :return: The dataset of the spread data.
-        """
-
-        return self.data(exchange=exchange, symbol=symbol)
-    # end trades
-
-    def trades_in_market(self, exchange: str, symbol: str) -> bool:
-        """
-        Returns the market data of the symbol from the exchange.
-
-        :param exchange: The source key of the exchange.
-        :param symbol: The symbol of the pair.
-
-        :return: The dataset of the spread data.
-        """
-
-        try:
-            self.trades(exchange=exchange, symbol=symbol)
-
-            return True
-
-        except ValueError:
-            return False
-        # end try
-    # end trades_in_market
-
-    async def record(self, data: Trade, timestamp: float) -> bool:
+    async def process(self, data: Trade, timestamp: float) -> bool:
         """
         Records the data from the crypto feed into the dataset.
 
         :param data: The data from the exchange.
         :param timestamp: The time of the request.
 
         :return: The validation value.
         """
 
+        exchange = data.exchange.lower()
+        symbol = adjust_symbol(symbol=data.symbol)
+
         return await record_trades(
-            market=self.market, data=data, timestamp=timestamp,
-            callbacks=self.callbacks
+            screeners=self.find_screeners(
+                base=TradesScreener, exchange=exchange, symbol=symbol
+            ), data=data, timestamp=timestamp, callbacks=self.callbacks
         )
-    # end record
+    # end process
 # end TradesRecorder
 
 class TradesMarketScreener(MarketScreener):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
@@ -328,15 +272,15 @@
             recorder: TradesMarketRecorder,
             screeners: Optional[Iterable[TradesScreener]] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None,
             refresh: Optional[Union[float, dt.timedelta, bool]] = None,
             limited: Optional[bool] = None,
-            handler: Optional[FeedHandler] = None,
+            handler: Optional[MarketHandler] = None,
             amount: Optional[int] = None
     ) -> None:
         """
         Creates the class attributes.
 
         :param location: The saving location for the data.
         :param delay: The delay for the process.
@@ -350,220 +294,94 @@
 
         super().__init__(
             location=location, cancel=cancel,
             delay=delay, recorder=recorder,
             screeners=screeners, handler=handler, limited=limited,
             amount=amount, refresh=refresh
         )
-
-        self.screeners[:] = screeners or self.create_trades_screeners()
     # end __init__
 
     @property
-    def trades_market(self) -> Market:
-        """
-        Returns the market to hold the recorder data.
-
-        :return: The market object.
-        """
-
-        return self.recorder.trades_market
-    # end trades_market
-
-    @property
     def trades_screeners(self) -> List[TradesScreener]:
         """
         Returns a list of all the order-book screeners.
 
         :return: The order-book screeners.
         """
 
-        return [
-            screener for screener in self.screeners
-            if isinstance(screener, TradesScreener)
-        ]
+        return self.find_screeners(base=TradesScreener)
     # end trades_screeners
-
-    def connect_screeners(self) -> None:
-        """Connects the screeners to the recording object."""
-
-        for screener in self.screeners:
-            if isinstance(screener, TradesScreener):
-                screener.market = self.trades(
-                    exchange=screener.exchange, symbol=screener.symbol
-                )
-            # end if
-        # end for
-    # end connect_screeners
-
-    def trades(self, exchange: str, symbol: str) -> pd.DataFrame:
-        """
-        Returns the market data of the symbol from the exchange.
-
-        :param exchange: The source key of the exchange.
-        :param symbol: The symbol of the pair.
-
-        :return: The dataset of the spread data.
-        """
-
-        return self.recorder.trades(exchange=exchange, symbol=symbol)
-    # end trades
-
-    def trades_in_market(self, exchange: str, symbol: str) -> bool:
-        """
-        Returns the market data of the symbol from the exchange.
-
-        :param exchange: The source key of the exchange.
-        :param symbol: The symbol of the pair.
-
-        :return: The dataset of the spread data.
-        """
-
-        return self.recorder.trades_in_market(exchange=exchange, symbol=symbol)
-    # end trades_in_market
-
-    def create_trades_screener(
-            self,
-            symbol: str,
-            exchange: str,
-            location: Optional[str] = None,
-            cancel: Optional[Union[float, dt.timedelta]] = None,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            container: Optional[Dict[str, Dict[str, TradesScreener]]] = None
-    ) -> TradesScreener:
-        """
-        Defines the class attributes.
-
-        :param symbol: The symbol of the asset.
-        :param exchange: The exchange to get source data from.
-        :param location: The saving location for the data.
-        :param cancel: The time to cancel the waiting.
-        :param delay: The delay for the process.
-        :param container: The container to contain the new screener.
-        """
-
-        if container is None:
-            container = {}
-        # end if
-
-        if cancel is None:
-            cancel = self.cancel
-        # end if
-
-        if delay is None:
-            delay = self.delay
-        # end if
-
-        screener = TradesScreener(
-            symbol=symbol, exchange=exchange, delay=delay,
-            location=location, cancel=cancel, market=(
-                self.trades(exchange=exchange, symbol=symbol)
-                if self.trades_in_market(symbol=symbol, exchange=exchange)
-                else None
-            )
-        )
-
-        container.setdefault(exchange, {})[symbol] = screener
-
-        return screener
-    # end create_trades_screener
-
-    def create_trades_screeners(
-            self,
-            location: Optional[str] = None,
-            cancel: Optional[Union[float, dt.timedelta]] = None,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            container: Optional[Dict[str, Dict[str, TradesScreener]]] = None
-    ) -> List[TradesScreener]:
-        """
-        Defines the class attributes.
-
-        :param location: The saving location for the data.
-        :param cancel: The time to cancel the waiting.
-        :param delay: The delay for the process.
-        :param container: The container to contain the new screeners.
-        """
-
-        screeners = []
-
-        for exchange, symbols in self.structure().items():
-            for symbol in symbols:
-                screeners.append(
-                    self.create_trades_screener(
-                        symbol=symbol, exchange=exchange, delay=delay,
-                        location=location, cancel=cancel, container=container
-                    )
-                )
-            # end for
-        # end for
-
-        return screeners
-    # end create_trades_screeners
 # end MarketOrderbookScreener
 
-Databases = Union[Iterable[str], Dict[str, Engine]]
+def create_trades_screeners(
+        data: Dict[str, Iterable[str]],
+        location: Optional[str] = None,
+        cancel: Optional[Union[float, dt.timedelta]] = None,
+        delay: Optional[Union[float, dt.timedelta]] = None,
+) -> List[TradesScreener]:
+    """
+    Defines the class attributes.
 
-def trades_market_recorder(data: Dict[str, Iterable[str]]) -> TradesMarketRecorder:
+    :param data: The data for the screeners.
+    :param location: The saving location for the data.
+    :param cancel: The time to cancel the waiting.
+    :param delay: The delay for the process.
     """
-    Creates the market recorder object for the data.
 
-    :param data: The market data.
+    screeners = []
 
-    :return: The market recorder object.
-    """
+    for exchange, symbols in data.items():
+        for symbol in symbols:
+            screeners.append(
+                TradesScreener(
+                    symbol=symbol, exchange=exchange, delay=delay,
+                    location=location, cancel=cancel
+                )
+            )
+        # end for
+    # end for
 
-    return TradesMarketRecorder(
-        market=create_trades_market(data=data)
-    )
-# end trades_market_recorder
+    return screeners
+# end create_trades_screeners
 
 def trades_market_screener(
         data: Dict[str, Iterable[str]],
         location: Optional[str] = None,
         cancel: Optional[Union[float, dt.timedelta]] = None,
         delay: Optional[Union[float, dt.timedelta]] = None,
         limited: Optional[bool] = None,
-        handler: Optional[FeedHandler] = None,
-        market: Optional[Market] = None,
+        handler: Optional[MarketHandler] = None,
         amount: Optional[int] = None,
         callbacks: Optional[Iterable[Callback]] = None,
         refresh: Optional[Union[float, dt.timedelta, bool]] = None,
-        recorder: Optional[TradesMarketRecorder] = None,
-        fixed: Optional[bool] = True,
-        parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
+        recorder: Optional[TradesMarketRecorder] = None
 ) -> TradesMarketScreener:
     """
     Creates the market screener object for the data.
 
     :param data: The market data.
     :param handler: The handler object for the market data.
     :param limited: The value to limit the screeners to active only.
-    :param parameters: The parameters for the exchanges.
-    :param market: The object to fill with the crypto feed record.
-    :param fixed: The value for fixed parameters to all exchanges.
     :param refresh: The refresh time for rerunning.
     :param amount: The maximum amount of symbols for each feed.
     :param recorder: The recorder object for recording the data.
     :param location: The saving location for the data.
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
     :param callbacks: The callbacks for the service.
 
     :return: The market screener object.
     """
 
-    screener = TradesMarketScreener(
+    screeners = create_trades_screeners(
+        data=data, location=location,
+        cancel=cancel, delay=delay
+    )
+
+    return TradesMarketScreener(
         recorder=recorder or TradesMarketRecorder(
-            market=market or create_trades_market(data=data),
-            callbacks=callbacks
-        ),
+            screeners=screeners, callbacks=callbacks
+        ), screeners=screeners,
         handler=handler, location=location, amount=amount,
         cancel=cancel, delay=delay, limited=limited, refresh=refresh
     )
-
-    screener.add_feeds(
-        data=screener.recorder.structure(),
-        fixed=fixed, parameters=parameters
-    )
-
-    return screener
 # end trades_market_screener
```

### Comparing `crypto-screening-7.5.6/crypto_screening/market/waiting.py` & `crypto-screening-8.0.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/process.py` & `crypto-screening-8.0.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/source/data/all_exchanges_symbols.json` & `crypto-screening-8.0.0/crypto_screening/source/data/all_exchanges_symbols.json`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/symbols.py` & `crypto-screening-8.0.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening/validate.py` & `crypto-screening-8.0.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-8.0.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 7.5.6
+Version: 8.0.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-7.5.6/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-8.0.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-7.5.6/pyproject.toml` & `crypto-screening-8.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '7.5.6'
+version = '8.0.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-7.5.6/setup.py` & `crypto-screening-8.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "crypto_screening/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='7.5.6',
+        version='8.0.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

