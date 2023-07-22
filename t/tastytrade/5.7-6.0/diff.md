# Comparing `tmp/tastytrade-5.7.tar.gz` & `tmp/tastytrade-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-5.7.tar", last modified: Sat Jul  8 03:39:01 2023, max compression
+gzip compressed data, was "tastytrade-6.0.tar", last modified: Sat Jul 22 02:53:52 2023, max compression
```

## Comparing `tastytrade-5.7.tar` & `tastytrade-6.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:39:01.782328 tastytrade-5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-08 03:38:47.000000 tastytrade-5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-07-08 03:39:01.782328 tastytrade-5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-07-08 03:38:47.000000 tastytrade-5.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 03:39:01.782328 tastytrade-5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-08 03:38:47.000000 tastytrade-5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:39:01.778328 tastytrade-5.7/tastytrade/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35213 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:39:01.782328 tastytrade-5.7/tastytrade/dxfeed/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/candle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/greeks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/theoprice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/timeandsale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/dxfeed/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    33222 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    19825 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-08 03:38:47.000000 tastytrade-5.7/tastytrade/watchlists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 03:39:01.782328 tastytrade-5.7/tastytrade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-07-08 03:39:01.000000 tastytrade-5.7/tastytrade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-08 03:39:01.000000 tastytrade-5.7/tastytrade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 03:39:01.000000 tastytrade-5.7/tastytrade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-08 03:39:01.000000 tastytrade-5.7/tastytrade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 03:39:01.000000 tastytrade-5.7/tastytrade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:53:52.341702 tastytrade-6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-22 02:53:43.000000 tastytrade-6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-07-22 02:53:52.337702 tastytrade-6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-22 02:53:43.000000 tastytrade-6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 02:53:52.341702 tastytrade-6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-22 02:53:43.000000 tastytrade-6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:53:52.333702 tastytrade-6.0/tastytrade/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35162 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:53:52.337702 tastytrade-6.0/tastytrade/dxfeed/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/candle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/greeks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/theoprice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/timeandsale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/dxfeed/underlying.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33234 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21256 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-07-22 02:53:43.000000 tastytrade-6.0/tastytrade/watchlists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 02:53:52.337702 tastytrade-6.0/tastytrade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-07-22 02:53:52.000000 tastytrade-6.0/tastytrade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-22 02:53:52.000000 tastytrade-6.0/tastytrade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 02:53:52.000000 tastytrade-6.0/tastytrade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-22 02:53:52.000000 tastytrade-6.0/tastytrade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-22 02:53:52.000000 tastytrade-6.0/tastytrade.egg-info/top_level.txt
```

### Comparing `tastytrade-5.7/LICENSE` & `tastytrade-6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tastytrade-5.7/PKG-INFO` & `tastytrade-6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 5.7
+Version: 6.0
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -20,91 +20,90 @@
 .. image:: https://static.pepy.tech/badge/tastytrade
    :target: https://pepy.tech/project/tastytrade
    :alt: PyPI Downloads
 
 Tastytrade Python SDK
 =====================
 
-.. inclusion-marker
-
 A simple, reverse-engineered SDK for Tastytrade built on their (now mostly public) API. This will allow you to create trading algorithms for whatever strategies you may have quickly and painlessly in Python.
 
 Installation
 ------------
 
-.. code-block:: bash
+::
 
    $ pip install tastytrade
 
 Creating a session
 ------------------
 
 A session object is required to authenticate your requests to the Tastytrade API.
 You can create a real session using your normal login, or a certification (test) session using your certification login.
 
 .. code-block:: python
 
-   from tastytrade.session import Session
-   session = Session('username', 'password')
+   from tastytrade import ProductionSession
+   session = ProductionSession('username', 'password')
 
 Using the streamer
 ------------------
 
-The streamer is a websocket connection to the Tastytrade API that allows you to subscribe to real-time data for Quotes, Greeks, and more.
+The streamer is a websocket connection to dxfeed (the Tastytrade data provider) that allows you to subscribe to real-time data for quotes, greeks, and more.
 
 .. code-block:: python
 
-   from tastytrade.streamer import DataStreamer, EventType
+   from tastytrade import DataStreamer
+   from tastytrade.dxfeed import EventType
 
    streamer = await DataStreamer.create(session)
    subs_list = ['SPY', 'SPX']
 
-   # this function fetches quotes once, then closes the subscription
    await streamer.subscribe(EventType.QUOTE, subs_list)
+   # this example fetches quotes once, then exits
    quotes = []
    async for quote in streamer.listen():
       quotes.append(quote)
       if len(quotes) >= len(subs_list):
          break
    print(quotes)
 
 >>> [Quote(eventSymbol='SPY', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='Q', bidPrice=411.58, bidSize=400.0, askTime=0, askExchangeCode='Q', askPrice=411.6, askSize=1313.0), Quote(eventSymbol='SPX', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='\x00', bidPrice=4122.49, bidSize='NaN', askTime=0, askExchangeCode='\x00', askPrice=4123.65, askSize='NaN')]
 
 Getting current positions
 -------------------------
 
 .. code-block:: python
    
-   from tastytrade.account import Account
+   from tastytrade import Account
 
    account = Account.get_accounts(session)[0]
    positions = account.get_positions(session)
    print(positions[0])
 
 >>> CurrentPosition(account_number='5WV69754', symbol='IAU', instrument_type=<InstrumentType.EQUITY: 'Equity'>, underlying_symbol='IAU', quantity=Decimal('20'), quantity_direction='Long', close_price=Decimal('37.09'), average_open_price=Decimal('37.51'), average_yearly_market_close_price=Decimal('37.51'), average_daily_market_close_price=Decimal('37.51'), multiplier=1, cost_effect='Credit', is_suppressed=False, is_frozen=False, realized_day_gain=Decimal('7.888'), realized_day_gain_effect='Credit', realized_day_gain_date=datetime.date(2023, 5, 19), realized_today=Decimal('0.512'), realized_today_effect='Debit', realized_today_date=datetime.date(2023, 5, 19), created_at=datetime.datetime(2023, 3, 31, 14, 38, 32, 58000, tzinfo=datetime.timezone.utc), updated_at=datetime.datetime(2023, 5, 19, 16, 56, 51, 920000, tzinfo=datetime.timezone.utc), mark=None, mark_price=None, restricted_quantity=Decimal('0'), expires_at=None, fixing_price=None, deliverable_type=None)
 
 Symbol search
 -------------
 
 .. code-block:: python
 
-   from tastytrade.search import symbol_search
+   from tastytrade import symbol_search
 
    results = symbol_search(session, 'AAP')
    print(results)
 
 >>> [SymbolData(symbol='AAP', description='Advance Auto Parts Inc.'), SymbolData(symbol='AAPD', description='Direxion Daily AAPL Bear 1X Shares'), SymbolData(symbol='AAPL', description='Apple Inc. - Common Stock'), SymbolData(symbol='AAPB', description='GraniteShares 1.75x Long AAPL Daily ETF'), SymbolData(symbol='AAPU', description='Direxion Daily AAPL Bull 1.5X Shares')]
 
 Placing an order
 ----------------
 
 .. code-block:: python
 
    from decimal import Decimal
-   from tastytrade.account import Account
+   from tastytrade import Account
    from tastytrade.instruments import Equity
    from tastytrade.order import NewOrder, OrderAction, OrderTimeInForce, OrderType, PriceEffect
 
    account = Account.get_account(session, '5WV69754')
    symbol = Equity.get_equity(session, 'USO')
    leg = symbol.build_leg(Decimal('5'), OrderAction.BUY_TO_OPEN)  # buy to open 5 shares
```

### Comparing `tastytrade-5.7/README.rst` & `tastytrade-6.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,91 +9,90 @@
 .. image:: https://static.pepy.tech/badge/tastytrade
    :target: https://pepy.tech/project/tastytrade
    :alt: PyPI Downloads
 
 Tastytrade Python SDK
 =====================
 
-.. inclusion-marker
-
 A simple, reverse-engineered SDK for Tastytrade built on their (now mostly public) API. This will allow you to create trading algorithms for whatever strategies you may have quickly and painlessly in Python.
 
 Installation
 ------------
 
-.. code-block:: bash
+::
 
    $ pip install tastytrade
 
 Creating a session
 ------------------
 
 A session object is required to authenticate your requests to the Tastytrade API.
 You can create a real session using your normal login, or a certification (test) session using your certification login.
 
 .. code-block:: python
 
-   from tastytrade.session import Session
-   session = Session('username', 'password')
+   from tastytrade import ProductionSession
+   session = ProductionSession('username', 'password')
 
 Using the streamer
 ------------------
 
-The streamer is a websocket connection to the Tastytrade API that allows you to subscribe to real-time data for Quotes, Greeks, and more.
+The streamer is a websocket connection to dxfeed (the Tastytrade data provider) that allows you to subscribe to real-time data for quotes, greeks, and more.
 
 .. code-block:: python
 
-   from tastytrade.streamer import DataStreamer, EventType
+   from tastytrade import DataStreamer
+   from tastytrade.dxfeed import EventType
 
    streamer = await DataStreamer.create(session)
    subs_list = ['SPY', 'SPX']
 
-   # this function fetches quotes once, then closes the subscription
    await streamer.subscribe(EventType.QUOTE, subs_list)
+   # this example fetches quotes once, then exits
    quotes = []
    async for quote in streamer.listen():
       quotes.append(quote)
       if len(quotes) >= len(subs_list):
          break
    print(quotes)
 
 >>> [Quote(eventSymbol='SPY', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='Q', bidPrice=411.58, bidSize=400.0, askTime=0, askExchangeCode='Q', askPrice=411.6, askSize=1313.0), Quote(eventSymbol='SPX', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='\x00', bidPrice=4122.49, bidSize='NaN', askTime=0, askExchangeCode='\x00', askPrice=4123.65, askSize='NaN')]
 
 Getting current positions
 -------------------------
 
 .. code-block:: python
    
-   from tastytrade.account import Account
+   from tastytrade import Account
 
    account = Account.get_accounts(session)[0]
    positions = account.get_positions(session)
    print(positions[0])
 
 >>> CurrentPosition(account_number='5WV69754', symbol='IAU', instrument_type=<InstrumentType.EQUITY: 'Equity'>, underlying_symbol='IAU', quantity=Decimal('20'), quantity_direction='Long', close_price=Decimal('37.09'), average_open_price=Decimal('37.51'), average_yearly_market_close_price=Decimal('37.51'), average_daily_market_close_price=Decimal('37.51'), multiplier=1, cost_effect='Credit', is_suppressed=False, is_frozen=False, realized_day_gain=Decimal('7.888'), realized_day_gain_effect='Credit', realized_day_gain_date=datetime.date(2023, 5, 19), realized_today=Decimal('0.512'), realized_today_effect='Debit', realized_today_date=datetime.date(2023, 5, 19), created_at=datetime.datetime(2023, 3, 31, 14, 38, 32, 58000, tzinfo=datetime.timezone.utc), updated_at=datetime.datetime(2023, 5, 19, 16, 56, 51, 920000, tzinfo=datetime.timezone.utc), mark=None, mark_price=None, restricted_quantity=Decimal('0'), expires_at=None, fixing_price=None, deliverable_type=None)
 
 Symbol search
 -------------
 
 .. code-block:: python
 
-   from tastytrade.search import symbol_search
+   from tastytrade import symbol_search
 
    results = symbol_search(session, 'AAP')
    print(results)
 
 >>> [SymbolData(symbol='AAP', description='Advance Auto Parts Inc.'), SymbolData(symbol='AAPD', description='Direxion Daily AAPL Bear 1X Shares'), SymbolData(symbol='AAPL', description='Apple Inc. - Common Stock'), SymbolData(symbol='AAPB', description='GraniteShares 1.75x Long AAPL Daily ETF'), SymbolData(symbol='AAPU', description='Direxion Daily AAPL Bull 1.5X Shares')]
 
 Placing an order
 ----------------
 
 .. code-block:: python
 
    from decimal import Decimal
-   from tastytrade.account import Account
+   from tastytrade import Account
    from tastytrade.instruments import Equity
    from tastytrade.order import NewOrder, OrderAction, OrderTimeInForce, OrderType, PriceEffect
 
    account = Account.get_account(session, '5WV69754')
    symbol = Equity.get_equity(session, 'USO')
    leg = symbol.build_leg(Decimal('5'), OrderAction.BUY_TO_OPEN)  # buy to open 5 shares
```

### Comparing `tastytrade-5.7/setup.py` & `tastytrade-6.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from setuptools import find_packages, setup
 
-from tastytrade import VERSION
-
 
 f = open('README.rst', 'r')
 LONG_DESCRIPTION = f.read()
 f.close()
 
 setup(
     name='tastytrade',
-    version=VERSION,
+    version='6.0',
     description='An unofficial SDK for Tastytrade!',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/x-rst',
     author='Graeme Holliday',
     author_email='graeme.holliday@pm.me',
     url='https://github.com/tastyware/tastytrade',
     license='MIT',
```

### Comparing `tastytrade-5.7/tastytrade/account.py` & `tastytrade-6.0/tastytrade/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import date, datetime
 from decimal import Decimal
-from typing import Any, Optional
+from typing import Any, Dict, List, Optional
 
 import requests
 
 from tastytrade.order import (InstrumentType, NewOrder, OrderStatus,
                               PlacedOrder, PlacedOrderResponse, PriceEffect)
 from tastytrade.session import Session
 from tastytrade.utils import (TastytradeError, TastytradeJsonDataclass,
@@ -176,15 +176,15 @@
     margin_requirement_effect: PriceEffect
     initial_requirement: Decimal
     initial_requirement_effect: PriceEffect
     maintenance_requirement: Decimal
     maintenance_requirement_effect: PriceEffect
     buying_power: Decimal
     buying_power_effect: PriceEffect
-    groups: list[dict[str, Any]]
+    groups: List[Dict[str, Any]]
     price_increase_percent: Decimal
     price_decrease_percent: Decimal
 
 
 class MarginReport(TastytradeJsonDataclass):
     """
     Dataclass containing an overall portfolio margin report.
@@ -203,15 +203,15 @@
     option_buying_power_effect: PriceEffect
     reg_t_margin_requirement: Decimal
     reg_t_margin_requirement_effect: PriceEffect
     reg_t_option_buying_power: Decimal
     reg_t_option_buying_power_effect: PriceEffect
     maintenance_excess: Decimal
     maintenance_excess_effect: PriceEffect
-    groups: list[MarginReportEntry]
+    groups: List[MarginReportEntry]
     last_state_timestamp: int
     initial_requirement: Optional[Decimal] = None
     initial_requirement_effect: Optional[PriceEffect] = None
 
 
 class MarginRequirement(TastytradeJsonDataclass):
     """
@@ -351,15 +351,15 @@
     leg_count: Optional[int] = None
     destination_venue: Optional[str] = None
     other_charge: Optional[Decimal] = None
     other_charge_effect: Optional[PriceEffect] = None
     other_charge_description: Optional[str] = None
     reverses_id: Optional[int] = None
     cost_basis_reconciliation_date: Optional[date] = None
-    lots: Optional[list[Lot]] = None
+    lots: Optional[List[Lot]] = None
     agency_price: Optional[Decimal] = None
     principal_price: Optional[Decimal] = None
 
 
 class Account(TastytradeJsonDataclass):
     """
     Dataclass that represents a Tastytrade account object, containing
@@ -392,15 +392,15 @@
     submitting_user_id: Optional[str] = None
 
     @classmethod
     def get_accounts(
         cls,
         session: Session,
         include_closed=False
-    ) -> list['Account']:
+    ) -> List['Account']:
         """
         Gets all trading accounts from the Tastyworks platform. By default
         excludes closed accounts from the results.
 
         :param session: the session to use for the request.
 
         :return: a list of :class:`Account` objects.
@@ -469,22 +469,24 @@
         """
         response = requests.get(
             f'{session.base_url}/accounts/{self.account_number}/balances',
             headers=session.headers
         )
         validate_response(response)  # throws exception if not 200
 
-        return response.json()['data']
+        data = response.json()['data']
+
+        return AccountBalance(**data)
 
     def get_balance_snapshots(
         self,
         session: Session,
         snapshot_date: Optional[date] = None,
         time_of_day: Optional[str] = None
-    ) -> list[AccountBalanceSnapshot]:
+    ) -> List[AccountBalanceSnapshot]:
         """
         Returns a list of two balance snapshots. The first one is the
         specified date, or, if not provided, the oldest snapshot available.
         The second one is the most recent snapshot.
 
         If you provide the snapshot date, you must also provide the time of
         day.
@@ -493,15 +495,15 @@
         :param snapshot_date: the date of the snapshot to get.
         :param time_of_day:
             the time of day of the snapshot to get, either 'EOD' or 'BOD'.
 
         :return:
             a list of two Tastytrade 'AccountBalanceSnapshot' in JSON format.
         """
-        params: dict[str, Any] = {
+        params: Dict[str, Any] = {
             'snapshot-date': snapshot_date,
             'time-of-day': time_of_day
         }
 
         response = requests.get(
             f'{session.base_url}/accounts/{self.account_number}/balance-snapshots',  # noqa: E501
             headers=session.headers,
@@ -512,23 +514,23 @@
         data = response.json()['data']['items']
 
         return [AccountBalanceSnapshot(**entry) for entry in data]
 
     def get_positions(
         self,
         session: Session,
-        underlying_symbols: Optional[list[str]] = None,
+        underlying_symbols: Optional[List[str]] = None,
         symbol: Optional[str] = None,
         instrument_type: Optional[InstrumentType] = None,
         include_closed: bool = False,
         underlying_product_code: Optional[str] = None,
-        partition_keys: Optional[list[str]] = None,
+        partition_keys: Optional[List[str]] = None,
         net_positions: bool = False,
         include_marks: bool = False
-    ) -> list[CurrentPosition]:
+    ) -> List[CurrentPosition]:
         """
         Get the current positions of the account.
 
         :param session: the session to use for the request.
         :param underlying_symbols:
             an array of underlying symbols for positions.
         :param symbol: a single symbol.
@@ -540,15 +542,15 @@
         :param net_positions:
             returns net positions grouped by instrument type and symbol.
         :param include_marks:
             include current quote mark (note: can decrease performance).
 
         :return: a list of Tastytrade 'CurrentPosition' objects in JSON format.
         """
-        params: dict[str, Any] = {
+        params: Dict[str, Any] = {
             'underlying-symbol[]': underlying_symbols,
             'symbol': symbol,
             'instrument-type': instrument_type,
             'include-closed-positions': include_closed,
             'underlying-product-code': underlying_product_code,
             'partition-keys[]': partition_keys,
             'net-positions': net_positions,
@@ -568,27 +570,27 @@
     def get_history(
         self,
         session: Session,
         per_page: int = 250,
         page_offset: Optional[int] = None,
         sort: str = 'Desc',
         type: Optional[str] = None,
-        types: Optional[list[str]] = None,
-        sub_types: Optional[list[str]] = None,
+        types: Optional[List[str]] = None,
+        sub_types: Optional[List[str]] = None,
         start_date: Optional[date] = None,
         end_date: date = date.today(),
         instrument_type: Optional[InstrumentType] = None,
         symbol: Optional[str] = None,
         underlying_symbol: Optional[str] = None,
         action: Optional[str] = None,
         partition_key: Optional[str] = None,
         futures_symbol: Optional[str] = None,
         start_at: Optional[datetime] = None,
         end_at: Optional[datetime] = None
-    ) -> list[Transaction]:
+    ) -> List[Transaction]:
         """
         Get transaction history of the account.
 
         :param session: the session to use for the request.
         :param per_page: the number of results to return per page.
         :param page_offset:
             provide a specific page to get; if not provided, get all pages
@@ -615,15 +617,15 @@
         """
         # if a specific page is provided, we just get that page;
         # otherwise, we loop through all pages
         paginate = False
         if page_offset is None:
             page_offset = 0
             paginate = True
-        params: dict[str, Any] = {
+        params: Dict[str, Any] = {
             'per-page': per_page,
             'page-offset': page_offset,
             'sort': sort,
             'type': type,
             'types[]': types,
             'sub-type[]': sub_types,
             'start-date': start_date,
@@ -679,39 +681,39 @@
 
         return Transaction(**data)
 
     def get_total_fees(
         self,
         session: Session,
         date: date = date.today()
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         """
         Get the total fees for a given date.
 
         :param session: the session to use for the request.
         :param date: the date to get fees for.
 
         :return: a dict containing the total fees and the price effect.
         """
-        params: dict[str, Any] = {'date': date}
+        params: Dict[str, Any] = {'date': date}
         response = requests.get(
             f'{session.base_url}/accounts/{self.account_number}/transactions/total-fees',  # noqa: E501
             headers=session.headers,
             params=params
         )
         validate_response(response)
 
         return response.json()['data']
 
     def get_net_liquidating_value_history(
         self,
         session: Session,
         time_back: Optional[str] = None,
         start_time: Optional[datetime] = None
-    ) -> list[NetLiqOhlc]:
+    ) -> List[NetLiqOhlc]:
         """
         Returns a list of account net liquidating value snapshots over the
         specified time period.
 
         :param session: the session to use for the request.
         :param time_back:
             the time period to get net liquidating value snapshots for. This
@@ -719,21 +721,18 @@
             '1d', '1m', '3m', '6m', '1y', 'all'.
         :param start_time:
             the start point for the query. This param is required is time-back
             is not given. If given, will take precedence over time-back.
 
         :return: a list of Tastytrade 'NetLiqOhlc' objects in JSON format.
         """
-        params: dict[str, Any] = {}
+        params: Dict[str, Any] = {}
         if start_time:
             # format to Tastytrade DateTime format
-            start_time = str(start_time) \
-                .replace(' ', 'T') \
-                .split('.')[0] + 'Z'  # type: ignore
-            params = {'start-time': start_time}
+            params = {'start-time': start_time.strftime('%Y-%m-%dT%H:%M:%SZ')}
         elif not time_back:
             msg = 'Either time_back or start_time must be specified.'
             raise TastytradeError(msg)
         else:
             params = {'time-back': time_back}
 
         response = requests.get(
@@ -805,15 +804,15 @@
         )
         validate_response(response)
 
         data = response.json()['data']
 
         return MarginReport(**data)
 
-    def get_live_orders(self, session: Session) -> list[PlacedOrder]:
+    def get_live_orders(self, session: Session) -> List[PlacedOrder]:
         """
         Get all live orders for the account.
 
         :param session: the session to use for the request.
 
         :return: a list of :class:`Order` objects.
         """
@@ -862,21 +861,21 @@
         self,
         session: Session,
         per_page: int = 50,
         page_offset: Optional[int] = None,
         start_date: Optional[date] = None,
         end_date: Optional[date] = None,
         underlying_symbol: Optional[str] = None,
-        statuses: Optional[list[OrderStatus]] = None,
+        statuses: Optional[List[OrderStatus]] = None,
         futures_symbol: Optional[str] = None,
         underlying_instrument_type: Optional[InstrumentType] = None,
         sort: str = 'Desc',
         start_at: Optional[datetime] = None,
         end_at: Optional[datetime] = None
-    ) -> list[PlacedOrder]:
+    ) -> List[PlacedOrder]:
         """
         Get order history of the account.
 
         :param session: the session to use for the request.
         :param per_page: the number of results to return per page.
         :param page_offset:
             provide a specific page to get; if not provided, get all pages
@@ -897,15 +896,15 @@
         """
         # if a specific page is provided, we just get that page;
         # otherwise, we loop through all pages
         paginate = False
         if page_offset is None:
             page_offset = 0
             paginate = True
-        params: dict[str, Any] = {
+        params: Dict[str, Any] = {
             'per-page': per_page,
             'page-offset': page_offset,
             'start-date': start_date,
             'end-date': end_date,
             'underlying-symbol': underlying_symbol,
             'status[]': statuses,
             'futures-symbol': futures_symbol,
```

### Comparing `tastytrade-5.7/tastytrade/dxfeed/candle.py` & `tastytrade-6.0/tastytrade/dxfeed/candle.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.7/tastytrade/dxfeed/event.py` & `tastytrade-6.0/tastytrade/dxfeed/event.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from abc import ABC
 from enum import Enum
+from typing import List
 
 
 class EventType(str, Enum):
     """
-    This is an :class:`~enum.Enum` that contains the valid subscription types for
-    the quote streamer.
+    This is an :class:`~enum.Enum` that contains the valid subscription types
+    for the data streamer.
 
-    Information on different types of events, their uses and their properties can be
-    found at the `dxfeed Knowledge Base <https://kb.dxfeed.com/en/data-model/dxfeed-api-market-events.html>`_.  # noqa: E501
+    Information on different types of events, their uses and their properties
+    can be found at the `dxfeed Knowledge Base
+    <https://kb.dxfeed.com/en/data-model/dxfeed-api-market-events.html>`_.
     """
     CANDLE = 'Candle'
     GREEKS = 'Greeks'
     PROFILE = 'Profile'
     QUOTE = 'Quote'
     SUMMARY = 'Summary'
     THEO_PRICE = 'TheoPrice'
     TIME_AND_SALE = 'TimeAndSale'
     TRADE = 'Trade'
+    UNDERLYING = 'Underlying'
 
 
 class Event(ABC):
     @classmethod
-    def from_stream(cls, data: list) -> list['Event']:
+    def from_stream(cls, data: list) -> List['Event']:
         """
         Makes a list of event objects from a list of raw trade data fetched by
         a :class:`~tastyworks.streamer.DataStreamer`.
 
         :param data: list of raw quote data from streamer
 
         :return: list of event objects from data
```

### Comparing `tastytrade-5.7/tastytrade/dxfeed/greeks.py` & `tastytrade-6.0/tastytrade/dxfeed/greeks.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.7/tastytrade/dxfeed/profile.py` & `tastytrade-6.0/tastytrade/dxfeed/profile.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.7/tastytrade/dxfeed/quote.py` & `tastytrade-6.0/tastytrade/dxfeed/quote.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.7/tastytrade/dxfeed/summary.py` & `tastytrade-6.0/tastytrade/dxfeed/summary.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.7/tastytrade/dxfeed/theoprice.py` & `tastytrade-6.0/tastytrade/dxfeed/theoprice.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.7/tastytrade/dxfeed/timeandsale.py` & `tastytrade-6.0/tastytrade/dxfeed/timeandsale.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.7/tastytrade/dxfeed/trade.py` & `tastytrade-6.0/tastytrade/dxfeed/trade.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.7/tastytrade/instruments.py` & `tastytrade-6.0/tastytrade/instruments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import date, datetime
 from decimal import Decimal
 from enum import Enum
-from typing import Any, Optional
+from typing import Any, Dict, List, Optional
 
 import requests
 
 from tastytrade.order import InstrumentType, TradeableTastytradeJsonDataclass
 from tastytrade.session import Session
 from tastytrade.utils import TastytradeJsonDataclass, validate_response
 
@@ -101,15 +101,15 @@
     """
     Dataclass representing an expiration in a nested options chain.
     """
     expiration_type: str
     expiration_date: date
     days_to_expiration: int
     settlement_type: str
-    strikes: list[Strike]
+    strikes: List[Strike]
 
 
 class NestedFutureOptionChainExpiration(TastytradeJsonDataclass):
     """
     Dataclass representing an expiration in a nested future options chain.
     """
     root_symbol: str
@@ -122,16 +122,16 @@
     expires_at: datetime
     asset: str
     expiration_type: str
     display_factor: Decimal
     option_contract_symbol: str
     stops_trading_at: datetime
     settlement_type: str
-    strikes: list[Strike]
-    tick_sizes: list[TickSize]
+    strikes: List[Strike]
+    tick_sizes: List[TickSize]
 
 
 class NestedFutureOptionFuture(TastytradeJsonDataclass):
     """
     Dataclass representing an underlying future in a nested future options
     chain.
     """
@@ -174,21 +174,21 @@
     """
     id: int
     short_description: str
     description: str
     is_closing_only: bool
     active: bool
     tick_size: Decimal
-    destination_venue_symbols: list[DestinationVenueSymbol]
+    destination_venue_symbols: List[DestinationVenueSymbol]
     streamer_symbol: Optional[str] = None
 
     @classmethod
     def get_cryptocurrencies(
-        cls, session: Session, symbols: list[str] = []
-    ) -> list['Cryptocurrency']:
+        cls, session: Session, symbols: List[str] = []
+    ) -> List['Cryptocurrency']:
         """
         Returns a list of cryptocurrency objects from the given symbols.
 
         :param session: the session to use for the request.
         :param symbols: the symbols to get the cryptocurrencies for.
 
         :return: a list of cryptocurrency objects.
@@ -250,25 +250,25 @@
     streamer_symbol: str
     borrow_rate: Optional[Decimal] = None
     cusip: Optional[str] = None
     short_description: Optional[str] = None
     halted_at: Optional[datetime] = None
     stops_trading_at: Optional[datetime] = None
     is_fractional_quantity_eligible: Optional[bool] = None
-    tick_sizes: Optional[list[TickSize]] = None
-    option_tick_sizes: Optional[list[TickSize]] = None
+    tick_sizes: Optional[List[TickSize]] = None
+    option_tick_sizes: Optional[List[TickSize]] = None
 
     @classmethod
     def get_active_equities(
         cls,
         session: Session,
         per_page: int = 1000,
         page_offset: Optional[int] = None,
         lendability: Optional[str] = None
-    ) -> list['Equity']:
+    ) -> List['Equity']:
         """
         Returns a list of actively traded :class:`Equity` objects.
 
         :param session: the session to use for the request.
         :param per_page: the number of equities to get per page.
         :param page_offset:
             provide a specific page to get; if not provided, get all pages
@@ -280,15 +280,15 @@
         """
         # if a specific page is provided, we just get that page;
         # otherwise, we loop through all pages
         paginate = False
         if page_offset is None:
             page_offset = 0
             paginate = True
-        params: dict[str, Any] = {
+        params: Dict[str, Any] = {
             'per-page': per_page,
             'page-offset': page_offset,
             'lendability': lendability
         }
 
         # loop through pages and get all active equities
         equities = []
@@ -313,33 +313,33 @@
 
         return equities
 
     @classmethod
     def get_equities(
         cls,
         session: Session,
-        symbols: Optional[list[str]] = None,
+        symbols: Optional[List[str]] = None,
         lendability: Optional[str] = None,
         is_index: Optional[bool] = None,
         is_etf: Optional[bool] = None
-    ) -> list['Equity']:
+    ) -> List['Equity']:
         """
         Returns a list of :class:`Equity` objects from the given symbols.
 
         :param session: the session to use for the request.
         :param symbols: the symbols to get the equities for.
         :param lendability:
             the lendability of the equities; e.g. 'Easy To Borrow',
             'Locate Required', 'Preborrow'
         :param is_index: whether the equities are indexes.
         :param is_etf: whether the equities are ETFs.
 
         :return: a list of :class:`Equity` objects.
         """
-        params: dict[str, Any] = {
+        params: Dict[str, Any] = {
             'symbol[]': symbols,
             'lendability': lendability,
             'is-index': is_index,
             'is-etf': is_etf
         }
         response = requests.get(
             f'{session.base_url}/instruments/equities',
@@ -405,29 +405,29 @@
         if not self.streamer_symbol:
             self._set_streamer_symbol()
 
     @classmethod
     def get_options(
         cls,
         session: Session,
-        symbols: Optional[list[str]] = None,
+        symbols: Optional[List[str]] = None,
         active: Optional[bool] = None,
         with_expired: Optional[bool] = None
-    ) -> list['Option']:
+    ) -> List['Option']:
         """
         Returns a list of :class:`Option` objects from the given symbols.
 
         :param session: the session to use for the request.
         :param symbols: the OCC symbols to get the options for.
         :param active: whether the options are active.
         :param with_expired: whether to include expired options.
 
         :return: a list of :class:`Option` objects.
         """
-        params: dict[str, Any] = {
+        params: Dict[str, Any] = {
             'symbol[]': symbols,
             'active': active,
             'with-expired': with_expired
         }
         response = requests.get(
             f'{session.base_url}/instruments/equity-options',
             headers=session.headers,
@@ -490,17 +490,17 @@
     create actual :class:`Option` objects you'll need to make an extra API
     request or two.
     """
     underlying_symbol: str
     root_symbol: str
     option_chain_type: str
     shares_per_contract: int
-    tick_sizes: list[TickSize]
-    deliverables: list[Deliverable]
-    expirations: list[NestedOptionChainExpiration]
+    tick_sizes: List[TickSize]
+    deliverables: List[Deliverable]
+    expirations: List[NestedOptionChainExpiration]
 
     @classmethod
     def get_chain(cls, session: Session, symbol: str) -> 'NestedOptionChain':
         """
         Gets the option chain for the given symbol in nested format.
 
         :param session: the session to use for the request.
@@ -530,16 +530,16 @@
     knowing the specific expirations or symbols.
     """
     root_symbol: str
     code: str
     description: str
     exchange: str
     product_type: str
-    listed_months: list[FutureMonthCode]
-    active_months: list[FutureMonthCode]
+    listed_months: List[FutureMonthCode]
+    active_months: List[FutureMonthCode]
     notional_multiplier: Decimal
     tick_size: Decimal
     display_factor: Decimal
     streamer_exchange_code: str
     small_notional: bool
     back_month_first_calendar_symbol: bool
     first_notice: bool
@@ -553,21 +553,21 @@
     contract_limit: Optional[int] = None
     product_subtype: Optional[str] = None
     security_group: Optional[str] = None
     true_underlying_code: Optional[str] = None
     clearport_code: Optional[str] = None
     legacy_code: Optional[str] = None
     legacy_exchange_code: Optional[str] = None
-    option_products: Optional[list['FutureOptionProduct']] = None
+    option_products: Optional[List['FutureOptionProduct']] = None
 
     @classmethod
     def get_future_products(
         cls,
         session: Session
-    ) -> list['FutureProduct']:
+    ) -> List['FutureProduct']:
         """
         Returns a list of :class:`FutureProduct` objects available.
 
         :param session: the session to use for the request.
 
         :return: a list of :class:`FutureProduct` objects.
         """
@@ -639,39 +639,39 @@
     contract_size: Optional[Decimal] = None
     main_fraction: Optional[Decimal] = None
     sub_fraction: Optional[Decimal] = None
     first_notice_date: Optional[date] = None
     roll_target_symbol: Optional[str] = None
     true_underlying_symbol: Optional[str] = None
     future_etf_equivalent: Optional[FutureEtfEquivalent] = None
-    tick_sizes: Optional[list[TickSize]] = None
-    option_tick_sizes: Optional[list[TickSize]] = None
-    spread_tick_sizes: Optional[list[TickSize]] = None
+    tick_sizes: Optional[List[TickSize]] = None
+    option_tick_sizes: Optional[List[TickSize]] = None
+    spread_tick_sizes: Optional[List[TickSize]] = None
 
     @classmethod
     def get_futures(
         cls,
         session: Session,
-        symbols: Optional[list[str]] = None,
-        product_codes: Optional[list[str]] = None
-    ) -> list['Future']:
+        symbols: Optional[List[str]] = None,
+        product_codes: Optional[List[str]] = None
+    ) -> List['Future']:
         """
         Returns a list of :class:`Future` objects from the given symbols
         or product codes.
 
         :param session: the session to use for the request.
         :param symbols:
             symbols of the futures, e.g. 'ESZ9', '/ESZ9'.
         :param product_codes:
             the product codes of the futures, e.g. 'ES', '6A'. Ignored if
             symbols are provided.
 
         :return: a list of :class:`Future` objects.
         """
-        params: dict[str, Any] = {
+        params: Dict[str, Any] = {
             'symbol[]': symbols,
             'product-code[]': product_codes
         }
         response = requests.get(
             f'{session.base_url}/instruments/futures',
             headers=session.headers,
             params={k: v for k, v in params.items() if v is not None}
@@ -728,15 +728,15 @@
     legacy_code: Optional[str] = None
     clearport_code: Optional[str] = None
 
     @classmethod
     def get_future_option_products(
         cls,
         session: Session
-    ) -> list['FutureOptionProduct']:
+    ) -> List['FutureOptionProduct']:
         """
         Returns a list of :class:`FutureOptionProduct` objects available.
 
         :param session: the session to use for the request.
 
         :return: a list of :class:`FutureOptionProduct` objects.
         """
@@ -817,20 +817,20 @@
     instrument_type: InstrumentType = InstrumentType.FUTURE_OPTION
     future_option_product: Optional['FutureOptionProduct'] = None
 
     @classmethod
     def get_future_options(
         cls,
         session: Session,
-        symbols: Optional[list[str]] = None,
+        symbols: Optional[List[str]] = None,
         root_symbol: Optional[str] = None,
         expiration_date: Optional[date] = None,
         option_type: Optional[OptionType] = None,
         strike_price: Optional[Decimal] = None
-    ) -> list['FutureOption']:
+    ) -> List['FutureOption']:
         """
         Returns a list of :class:`FutureOption` objects from the given symbols.
 
         NOTE: As far as I can tell, all of the parameters are bugged except
         for `symbols`.
 
         :param session: the session to use for the request.
@@ -839,15 +839,15 @@
             the root symbol to get the future options for, e.g. 'EW3', 'SO'
         :param expiration_date: the expiration date for the future options.
         :param option_type: the option type to filter by.
         :param strike_price: the strike price to filter by.
 
         :return: a list of :class:`FutureOption` objects.
         """
-        params: dict[str, Any] = {
+        params: Dict[str, Any] = {
             'symbol[]': symbols,
             'option-root-symbol': root_symbol,
             'expiration-date': expiration_date,
             'option-type': option_type,
             'strike-price': strike_price
         }
         response = requests.get(
@@ -891,28 +891,28 @@
     """
     Dataclass that represents a Tastytrade nested future option chain for a
     specific futures underlying symbol.
     """
     underlying_symbol: str
     root_symbol: str
     exercise_style: str
-    expirations: list[NestedFutureOptionChainExpiration]
+    expirations: List[NestedFutureOptionChainExpiration]
 
 
 class NestedFutureOptionChain(TastytradeJsonDataclass):
     """
     Dataclass that represents a Tastytrade nested option chain object. Contains
     information about the option chain and a method to fetch one for a symbol.
 
     This is cleaner than calling :meth:`get_future_option_chain` but if you
     want to create actual :class:`FutureOption` objects you'll need to make an
     extra API request or two.
     """
-    futures: list[NestedFutureOptionFuture]
-    option_chains: list[NestedFutureOptionSubchain]
+    futures: List[NestedFutureOptionFuture]
+    option_chains: List[NestedFutureOptionSubchain]
 
     @classmethod
     def get_chain(
         cls,
         session: Session,
         symbol: str
     ) -> 'NestedFutureOptionChain':
@@ -949,16 +949,16 @@
     active: bool
     cusip: Optional[str] = None
 
     @classmethod
     def get_warrants(
         cls,
         session: Session,
-        symbols: Optional[list[str]] = None
-    ) -> list['Warrant']:
+        symbols: Optional[List[str]] = None
+    ) -> List['Warrant']:
         """
         Returns a list of :class:`Warrant` objects from the given symbols.
 
         :param session: the session to use for the request.
         :param symbols: symbols of the warrants, e.g. 'NKLAW'
 
         :return: a list of :class:`Warrant` objects.
@@ -998,15 +998,15 @@
 
 # fix pydantic forward references
 FutureProduct.update_forward_refs()
 
 
 def get_quantity_decimal_precisions(
     session: Session
-) -> list[QuantityDecimalPrecision]:
+) -> List[QuantityDecimalPrecision]:
     """
     Returns a list of :class:`QuantityDecimalPrecision` objects for different
     types of instruments.
 
     :param session: the session to use for the request.
 
     :return: a list of :class:`QuantityDecimalPrecision` objects.
@@ -1021,15 +1021,15 @@
 
     return [QuantityDecimalPrecision(**entry) for entry in data]
 
 
 def get_option_chain(
     session: Session,
     symbol: str
-) -> dict[date, list[Option]]:
+) -> Dict[date, List[Option]]:
     """
     Returns a mapping of expiration date to a list of option objects
     representing the options chain for the given symbol.
 
     In the case that there are two expiries on the same day (e.g. SPXW
     and SPX AM options), both will be returned in the same list. If you
     just want one expiry, you'll need to filter the list yourself, or use
@@ -1058,15 +1058,15 @@
 
     return chain
 
 
 def get_future_option_chain(
     session: Session,
     symbol: str
-) -> dict[date, list[FutureOption]]:
+) -> Dict[date, List[FutureOption]]:
     """
     Returns a mapping of expiration date to a list of futures options
     objects representing the options chain for the given symbol.
 
     In the case that there are two expiries on the same day (e.g. EW
     and ES options), both will be returned in the same list. If you
     just want one expiry, you'll need to filter the list yourself, or
```

### Comparing `tastytrade-5.7/tastytrade/metrics.py` & `tastytrade-6.0/tastytrade/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import date, datetime
 from decimal import Decimal
-from typing import Any, Optional
+from typing import Any, Dict, List, Optional
 
 import requests
 
 from tastytrade.session import Session
 from tastytrade.utils import TastytradeJsonDataclass, validate_response
 
 
@@ -61,15 +61,15 @@
     implied_volatility_index_rank_source: str
     implied_volatility_percentile: Decimal
     implied_volatility_updated_at: datetime
     liquidity_value: Decimal
     liquidity_rank: Decimal
     liquidity_rating: int
     updated_at: datetime
-    option_expiration_implied_volatilities: list[OptionExpirationImpliedVolatility]  # noqa: E501
+    option_expiration_implied_volatilities: List[OptionExpirationImpliedVolatility]  # noqa: E501
     liquidity_running_state: Liquidity
     beta: Decimal
     beta_updated_at: datetime
     corr_spy_3month: Decimal
     dividend_rate_per_share: Decimal
     dividend_yield: Decimal
     listed_market: str
@@ -88,16 +88,16 @@
     dividend_next_date: Optional[date] = None
     dividend_pay_date: Optional[date] = None
     dividend_updated_at: Optional[datetime] = None
 
 
 def get_market_metrics(
     session: Session,
-    symbols: list[str]
-) -> list[MarketMetricInfo]:
+    symbols: List[str]
+) -> List[MarketMetricInfo]:
     """
     Retrieves market metrics for the given symbols.
 
     :param session: active user session to use
     :param symbols: list of symbols to retrieve metrics for
 
     :return: a list of Tastytrade 'MarketMetricInfo' objects in JSON format.
@@ -110,15 +110,15 @@
     validate_response(response)
 
     data = response.json()['data']['items']
 
     return [MarketMetricInfo(**entry) for entry in data]
 
 
-def get_dividends(session: Session, symbol: str) -> list[DividendInfo]:
+def get_dividends(session: Session, symbol: str) -> List[DividendInfo]:
     """
     Retrieves dividend information for the given symbol.
 
     :param session: active user session to use
     :param symbol: symbol to retrieve dividend information for
 
     :return: a list of Tastytrade 'DividendInfo' objects in JSON format.
@@ -135,26 +135,26 @@
     return [DividendInfo(**entry) for entry in data]
 
 
 def get_earnings(
     session: Session,
     symbol: str,
     start_date: date
-) -> list[EarningsInfo]:
+) -> List[EarningsInfo]:
     """
     Retrieves earnings information for the given symbol.
 
     :param session: active user session to use
     :param symbol: symbol to retrieve earnings information for
     :param start_date: limits earnings to those on or after the given date
 
     :return: a list of Tastytrade 'EarningsInfo' objects in JSON format.
     """
     symbol = symbol.replace('/', '%2F')
-    params: dict[str, Any] = {'start-date': start_date}
+    params: Dict[str, Any] = {'start-date': start_date}
     response = requests.get(
         f'{session.base_url}/market-metrics/historic-corporate-events/earnings-reports/{symbol}',  # noqa: E501
         headers=session.headers,
         params=params
     )
     validate_response(response)
```

### Comparing `tastytrade-5.7/tastytrade/order.py` & `tastytrade-6.0/tastytrade/order.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import date, datetime
 from decimal import Decimal
 from enum import Enum
-from typing import Optional
+from typing import Dict, List, Optional
 
 from tastytrade import VERSION
 from tastytrade.utils import TastytradeJsonDataclass
 
 
 class InstrumentType(str, Enum):
     """
@@ -116,15 +116,15 @@
     call :meth:`build_leg` to build a leg from the dataclass.
     """
     instrument_type: InstrumentType
     symbol: str
     action: OrderAction
     quantity: Decimal
     remaining_quantity: Optional[Decimal] = None
-    fills: Optional[list[FillInfo]] = None
+    fills: Optional[List[FillInfo]] = None
 
 
 class TradeableTastytradeJsonDataclass(TastytradeJsonDataclass):
     """
     Dataclass that represents a tradeable instrument.
 
     Classes that inherit from this class can call :meth:`build_leg` to build a
@@ -183,37 +183,37 @@
     instrument_type: InstrumentType
     indicator: str
     comparator: str
     threshold: Decimal
     is_threshold_based_on_notional: bool
     triggered_at: datetime
     triggered_value: Decimal
-    price_components: list[OrderConditionPriceComponent]
+    price_components: List[OrderConditionPriceComponent]
 
 
 class OrderRule(TastytradeJsonDataclass):
     """
     Dataclass that represents an order rule for a complex order.
     """
     route_after: datetime
     routed_at: datetime
     cancel_at: datetime
     cancelled_at: datetime
-    order_conditions: list[OrderCondition]
+    order_conditions: List[OrderCondition]
 
 
 class NewOrder(TastytradeJsonDataclass):
     """
     Dataclass containing information about a new order. Also used for
     modifying existing orders.
     """
     time_in_force: OrderTimeInForce
     order_type: OrderType
     source: str = f'tastyware/tastytrade:v{VERSION}'
-    legs: list[Leg]
+    legs: List[Leg]
     gtc_date: Optional[date] = None
     stop_trigger: Optional[Decimal] = None
     price: Optional[Decimal] = None  # optional for market orders
     price_effect: Optional[PriceEffect] = None
     value: Optional[Decimal] = None
     value_effect: Optional[PriceEffect] = None
     partition_key: Optional[str] = None
@@ -233,15 +233,15 @@
     underlying_symbol: str
     underlying_instrument_type: InstrumentType
     status: OrderStatus
     cancellable: bool
     editable: bool
     edited: bool
     updated_at: datetime
-    legs: list[Leg]
+    legs: List[Leg]
     id: Optional[str] = None
     price: Optional[Decimal] = None
     price_effect: Optional[PriceEffect] = None
     gtc_date: Optional[date] = None
     value: Optional[Decimal] = None
     value_effect: Optional[PriceEffect] = None
     stop_trigger: Optional[str] = None
@@ -272,16 +272,16 @@
     id: str
     account_number: str
     type: str
     terminal_at: str
     ratio_price_threshold: Decimal
     ratio_price_comparator: str
     ratio_price_is_threshold_based_on_notional: bool
-    related_orders: list[dict[str, str]]
-    orders: list[PlacedOrder]
+    related_orders: List[Dict[str, str]]
+    orders: List[PlacedOrder]
     trigger_order: PlacedOrder
 
 
 class BuyingPowerEffect(TastytradeJsonDataclass):
     """
     Dataclass containing information about the effect of a trade on buying
     power.
@@ -321,16 +321,16 @@
     """
     Dataclass grouping together information about a placed order.
     """
     buying_power_effect: BuyingPowerEffect
     fee_calculation: FeeCalculation
     order: Optional[PlacedOrder] = None
     complex_order: Optional[ComplexOrder] = None
-    warnings: Optional[list[Message]] = None
-    errors: Optional[list[Message]] = None
+    warnings: Optional[List[Message]] = None
+    errors: Optional[List[Message]] = None
 
 
 class OrderChainEntry(TastytradeJsonDataclass):
     """
     Dataclass containing information about a single order in an order chain.
     """
     symbol: str
@@ -365,16 +365,16 @@
     total_fill_cost: Optional[Decimal] = None
     total_fill_cost_effect: Optional[PriceEffect] = None
     gcd_quantity: Optional[Decimal] = None
     fill_cost_per_quantity: Optional[Decimal] = None
     fill_cost_per_quantity_effect: Optional[PriceEffect] = None
     order_fill_count: Optional[int] = None
     roll: Optional[bool] = None
-    legs: Optional[list[OrderChainLeg]] = None
-    entries: Optional[list[OrderChainEntry]] = None
+    legs: Optional[List[OrderChainLeg]] = None
+    entries: Optional[List[OrderChainEntry]] = None
 
 
 class ComputedData(TastytradeJsonDataclass):
     """
     Dataclass containing computed data about an order chain.
     """
     open: bool
@@ -399,15 +399,15 @@
     total_opening_cost_effect: PriceEffect
     total_closing_cost: Decimal
     total_closing_cost_effect: PriceEffect
     total_cost: Decimal
     total_cost_effect: PriceEffect
     gcd_open_quantity: Decimal
     fees_missing: bool
-    open_entries: list[OrderChainEntry]
+    open_entries: List[OrderChainEntry]
     total_cost_per_unit: Optional[Decimal] = None
     total_cost_per_unit_effect: Optional[PriceEffect] = None
 
 
 class OrderChain(TastytradeJsonDataclass):
     """
     Dataclass containing information about an order chain: a group of orders
@@ -418,8 +418,8 @@
     updated_at: datetime
     created_at: datetime
     account_number: str
     description: str
     underlying_symbol: str
     computed_data: ComputedData
     lite_nodes_sizes: int
-    lite_nodes: list[OrderChainNode]
+    lite_nodes: List[OrderChainNode]
```

### Comparing `tastytrade-5.7/tastytrade/search.py` & `tastytrade-6.0/tastytrade/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from typing import List
+
 import requests
 
 from tastytrade.session import Session
 from tastytrade.utils import TastytradeJsonDataclass
 
 
 class SymbolData(TastytradeJsonDataclass):
     """
     Dataclass holding search results for an individual item.
     """
     symbol: str
     description: str
 
 
-def symbol_search(session: Session, symbol: str) -> list[SymbolData]:
+def symbol_search(session: Session, symbol: str) -> List[SymbolData]:
     """
     Performs a symbol search using the Tastytrade API and returns a
     list of symbols that are similar to the given search phrase.
 
     :param session: active user session to use
     :param symbol: search phrase
```

### Comparing `tastytrade-5.7/tastytrade/streamer.py` & `tastytrade-6.0/tastytrade/streamer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,27 @@
 import asyncio
 import json
 from asyncio import Lock, Queue
 from datetime import datetime
 from decimal import Decimal
 from enum import Enum
-from typing import Any, AsyncIterator, Optional, Union
+from typing import Any, AsyncIterator, Dict, List, Optional, Union
 
-import requests
 import websockets
 
 from tastytrade import logger
 from tastytrade.account import (Account, AccountBalance, CurrentPosition,
                                 TradingStatus)
-from tastytrade.dxfeed import Channel
-from tastytrade.dxfeed.candle import Candle
-from tastytrade.dxfeed.event import Event, EventType
-from tastytrade.dxfeed.greeks import Greeks
-from tastytrade.dxfeed.profile import Profile
-from tastytrade.dxfeed.quote import Quote
-from tastytrade.dxfeed.summary import Summary
-from tastytrade.dxfeed.theoprice import TheoPrice
-from tastytrade.dxfeed.timeandsale import TimeAndSale
-from tastytrade.dxfeed.trade import Trade
+from tastytrade.dxfeed import (Candle, Channel, Event, EventType, Greeks,
+                               Profile, Quote, Summary, TheoPrice, TimeAndSale,
+                               Trade, Underlying)
 from tastytrade.order import (InstrumentType, OrderChain, PlacedOrder,
                               PriceEffect)
-from tastytrade.session import Session
-from tastytrade.utils import (TastytradeError, TastytradeJsonDataclass,
-                              validate_response)
+from tastytrade.session import CertificationSession, ProductionSession, Session
+from tastytrade.utils import TastytradeError, TastytradeJsonDataclass
 from tastytrade.watchlists import Watchlist
 
 CERT_STREAMER_URL = 'wss://streamer.cert.tastyworks.com'
 STREAMER_URL = 'wss://streamer.tastyworks.com'
 
 
 class QuoteAlert(TastytradeJsonDataclass):
@@ -87,15 +78,16 @@
     Used to subscribe to account-level updates (balances, orders, positions),
     public watchlist updates, quote alerts, and user-level messages. It should
     always be initialized using the :meth:`create` function, since the object
     cannot be fully instantiated without using async.
 
     Example usage::
 
-        session = Session('user', 'pass')
+        from tastytrade import Account, AlertStreamer
+
         streamer = await AlertStreamer.create(session)
         accounts = Account.get_accounts(session)
 
         await streamer.account_subscribe(accounts)
         await streamer.public_watchlists_subscribe()
         await streamer.quote_alerts_subscribe()
 
@@ -103,16 +95,17 @@
             print(data)
 
     """
     def __init__(self, session: Session):
         #: The active session used to initiate the streamer or make requests
         self.token: str = session.session_token
         #: The base url for the streamer websocket
+        is_certification = isinstance(session, CertificationSession)
         self.base_url: str = \
-            CERT_STREAMER_URL if session.is_certification else STREAMER_URL
+            CERT_STREAMER_URL if is_certification else STREAMER_URL
 
         self._queue: Queue = Queue()
         self._websocket = None
 
         self._connect_task = asyncio.create_task(self._connect())
 
     @classmethod
@@ -185,15 +178,15 @@
         elif type_str == 'UnderlyingYearGainSummary':
             return UnderlyingYearGainSummary(**data)
         elif type_str == 'PublicWatchlists':
             return Watchlist(**data)
         else:
             raise TastytradeError(f'Unknown message type: {type_str}\n{data}')
 
-    async def account_subscribe(self, accounts: list[Account]) -> None:
+    async def account_subscribe(self, accounts: List[Account]) -> None:
         """
         Subscribes to account-level updates (balances, orders, positions).
 
         :param accounts: list of :class:`Account` to subscribe to updates for
         """
         await self._subscribe(
             SubscriptionType.ACCOUNT,
@@ -235,21 +228,21 @@
             await self._subscribe(SubscriptionType.HEARTBEAT, '')
             # send the heartbeat every 10 seconds
             await asyncio.sleep(10)
 
     async def _subscribe(
         self,
         subscription: SubscriptionType,
-        value: Union[Optional[str], list[str]] = ''
+        value: Union[Optional[str], List[str]] = ''
     ) -> None:
         """
         Subscribes to a :class:`SubscriptionType`. Depending on the kind of
         subscription, the value parameter may be required.
         """
-        message: dict[str, Any] = {
+        message: Dict[str, Any] = {
             'auth-token': self.token,
             'action': subscription
         }
         if value:
             message['value'] = value
         logger.debug('sending alert subscription: %s', message)
         await self._websocket.send(json.dumps(message))  # type: ignore
@@ -260,58 +253,58 @@
     A :class:`DataStreamer` object is used to fetch quotes or greeks
     for a given symbol or list of symbols. It should always be
     initialized using the :meth:`create` function, since the object
     cannot be fully instantiated without using async.
 
     Example usage::
 
-        session = Session('user', 'pass')
+        from tastytrade import DataStreamer
+        from tastytrade.dxfeed import EventType
+
+        # must be a production session
         streamer = await DataStreamer.create(session)
 
         subs = ['SPY', 'GLD']  # list of quotes to fetch
         await streamer.subscribe(EventType.QUOTE, subs)
         quotes = []
-        async for quote in streamer.listen():
+        async for quote in streamer.listen(EventType.QUOTE):
             quotes.append(quote)
             if len(quotes) >= len(subs):
                 break
 
     """
-    def __init__(self, session: Session):
-        #: The active session used to initiate the streamer or make requests
-        self.session: Session = session
-
+    def __init__(self, session: ProductionSession):
         self._counter = 0
         self._lock: Lock = Lock()
-        self._queue: Queue = Queue()
-        self._queue_candle: Queue = Queue()
+        self._queues: Dict[str, Queue] = {
+            EventType.CANDLE: Queue(),
+            EventType.GREEKS: Queue(),
+            EventType.PROFILE: Queue(),
+            EventType.QUOTE: Queue(),
+            EventType.SUMMARY: Queue(),
+            EventType.THEO_PRICE: Queue(),
+            EventType.TIME_AND_SALE: Queue(),
+            EventType.TRADE: Queue(),
+            EventType.UNDERLYING: Queue()
+        }
         #: The unique client identifier received from the server
         self.client_id: Optional[str] = None
 
-        response = requests.get(
-            f'{session.base_url}/quote-streamer-tokens',
-            headers=session.headers
-        )
-        validate_response(response)
-        logger.debug('response %s', json.dumps(response.json()))
-        self._auth_token = response.json()['data']['token']
-        url = response.json()['data']['websocket-url'] + '/cometd'
-        self._wss_url = url.replace('https', 'wss')
+        self._auth_token = session.streamer_token
+        self._wss_url = session.streamer_url
 
         self._connect_task = asyncio.create_task(self._connect())
 
     @classmethod
-    async def create(cls, session: Session) -> 'DataStreamer':
+    async def create(cls, session: ProductionSession) -> 'DataStreamer':
         """
         Factory method for the :class:`DataStreamer` object.
         Simply calls the constructor and performs the asynchronous
         setup tasks. This should be used instead of the constructor.
 
-        Setup time is around 10-15 seconds.
-
         :param session: active user session to use
         """
         self = cls(session)
         while not self.client_id:
             await asyncio.sleep(0.1)
 
         return self
@@ -349,20 +342,18 @@
                         raise TastytradeError('Handshake failed')
 
             # main loop
             while True:
                 raw_message = await self._websocket.recv()
                 message = json.loads(raw_message)[0]
 
-                if message['channel'] == Channel.DATA:
+                if (message['channel'] == Channel.DATA or
+                        message['channel'] == Channel.TIME_SERIES):
                     logger.debug('data received: %s', message)
-                    await self._queue.put(message['data'])
-                elif message['channel'] == Channel.CANDLE:
-                    logger.debug('candle received: %s', message)
-                    await self._queue_candle.put(message['data'])
+                    await self._map_message(message['data'])
                 elif message['channel'] == Channel.SUBSCRIPTION:
                     logger.debug('sub received: %s', message)
 
     async def _handshake(self) -> None:
         """
         Sends a handshake message to the specified WebSocket
         connection. The handshake message is sent as a JSON
@@ -384,36 +375,27 @@
             'advice': {
                 'timeout': 60000,
                 'interval': 0
             }
         }
         await self._websocket.send(json.dumps([message]))
 
-    async def listen(self) -> AsyncIterator[Event]:
-        """
-        Using the existing subscriptions, pulls events and yield returns
-        them. Never exits unless there's an error or the channel is closed.
+    async def listen(
+        self,
+        event_type: EventType
+    ) -> AsyncIterator[Event]:
         """
-        while True:
-            raw_data = await self._queue.get()
-            messages = self._map_message(raw_data)
-            for message in messages:
-                yield message
-
-    async def listen_candle(self) -> AsyncIterator[Candle]:
-        """
-        Using the existing subscriptions, pulls candles and yield
-        returns them.
-        Never exits unless there's an error or the channel is closed.
+        Using the existing subscriptions, pulls events of the given type and
+        yield returns them. Never exits unless there's an error or the channel
+        is closed.
+
+        :param event_type: the type of event to listen for
         """
         while True:
-            raw_data = await self._queue_candle.get()
-            messages = self._map_message(raw_data)
-            for message in messages:
-                yield message  # type: ignore
+            yield await self._queues[event_type].get()
 
     def close(self) -> None:
         """
         Closes the websocket connection and cancels the heartbeat task.
         """
         self._connect_task.cancel()
         self._heartbeat_task.cancel()
@@ -435,20 +417,21 @@
             await self._websocket.send(json.dumps([message]))
             # send the heartbeat every 10 seconds
             await asyncio.sleep(10)
 
     async def subscribe(
         self,
         event_type: EventType,
-        symbols: list[str],
+        symbols: List[str],
         reset: bool = False
     ) -> None:
         """
         Subscribes to quotes for given list of symbols. Used for recurring data
         feeds.
+        For candles, use :meth:`subscribe_candle` instead.
 
         :param event_type: type of subscription to add
         :param symbols: list of symbols to subscribe for
         :param reset:
             whether to reset the subscription list (remove all other
             subscriptions of all types)
         """
@@ -464,111 +447,156 @@
         }
         logger.debug('sending subscription: %s', message)
         await self._websocket.send(json.dumps([message]))
 
     async def unsubscribe(
         self,
         event_type: EventType,
-        symbols: list[str]
+        symbols: List[str]
     ) -> None:
         """
         Removes existing subscription for given list of symbols.
+        For candles, use :meth:`unsubscribe_candle` instead.
 
         :param event_type: type of subscription to remove
         :param symbols: list of symbols to unsubscribe from
         """
         id = await self._next_id()
         message = {
             'id': id,
             'channel': Channel.SUBSCRIPTION,
-            'data': {
-                'reset': False,
-                'remove': {event_type: symbols}
-            },
+            'data': {'remove': {event_type: symbols}},
             'clientId': self.client_id
         }
         logger.debug('sending unsubscription: %s', message)
         await self._websocket.send(json.dumps([message]))
 
     async def subscribe_candle(
         self,
-        ticker: str,
+        symbols: List[str],
+        interval: str,
         start_time: datetime,
-        interval: str
+        end_time: Optional[datetime] = None,
+        extended_trading_hours: bool = False,
+        reset: bool = False
     ) -> None:
         """
-        Subscribes to candle-style 'OHLC' data for the given symbol.
+        Subscribes to time series data for the given symbol.
 
-        :param ticker: symbol to get date for
-        :param start_time: starting time for the data range
+        :param symbols: list of symbols to get data for
         :param interval:
-            the width of each candle in time, e.g. '5m', '1h', '3d',
+            the width of each candle in time, e.g. '15s', '5m', '1h', '3d',
             '1w', '1mo'
+        :param start_time: starting time for the data range
+        :param end_time: ending time for the data range
+        :param extended_trading_hours: whether to include extended trading
+        :param reset: whether to reset the subscription list
         """
         id = await self._next_id()
+        key = EventType.CANDLE
         message = {
             'id': id,
             'channel': Channel.SUBSCRIPTION,
             'data': {
+                'reset': reset,
                 'addTimeSeries': {
-                    'Candle': [{
-                        'eventSymbol': f'{ticker}{{={interval}}}',
+                    key: [{
+                        'eventSymbol': f'{ticker}{{={interval},tho=true}}'
+                        if extended_trading_hours
+                        else f'{ticker}{{={interval}}}',
                         'fromTime': int(start_time.timestamp() * 1000)
-                    }]
+                    } for ticker in symbols]
                 }
             },
             'clientId': self.client_id
         }
-        logger.debug('sending subscription: %s', message)
+        if end_time is not None:
+            message['data']['addTimeSeries'][key][0]['toTime'] = \
+                int(end_time.timestamp() * 1000)
         await self._websocket.send(json.dumps([message]))
 
-    async def unsubscribe_candle(self, ticker: str, interval: str) -> None:
+    async def unsubscribe_candle(
+        self,
+        ticker: str,
+        interval: Optional[str] = None,
+        extended_trading_hours: bool = False
+    ) -> None:
         """
-        Removes existing candle subscription for given list of symbols.
+        Removes existing subscription for a candle.
 
         :param ticker: symbol to unsubscribe from
         :param interval: candle width to unsubscribe from
+        :param extended_trading_hours:
+            whether candle to unsubscribe from contains extended trading hours
         """
         id = await self._next_id()
         message = {
             'id': id,
             'channel': Channel.SUBSCRIPTION,
             'data': {
-                'removeTimeSeries': {'Candle': [f'{ticker}{{={interval}}}']}
+                'removeTimeSeries': {
+                    EventType.CANDLE: [
+                        f'{ticker}{{={interval},tho=true}}'
+                        if extended_trading_hours
+                        else f'{ticker}{{={interval}}}'
+                    ]
+                }
             },
             'clientId': self.client_id
         }
         logger.debug('sending unsubscription: %s', message)
         await self._websocket.send(json.dumps([message]))
 
-    def _map_message(self, message) -> list[Event]:
+    async def _map_message(self, message) -> None:
         """
-        Takes the raw JSON data and returns a list of parsed event objects.
+        Takes the raw JSON data, parses the events and places them into their
+        respective queues.
+
+        :param message: raw JSON data from the websocket
         """
         # the first time around, types are shown
         if isinstance(message[0], str):
             msg_type = message[0]
         else:
             msg_type = message[0][0]
         # regardless, the second element will be the raw data
         data = message[1]
 
         # parse type or warn for unknown type
         if msg_type == EventType.CANDLE:
-            return Candle.from_stream(data)
+            candles = Candle.from_stream(data)
+            for candle in candles:
+                await self._queues[EventType.CANDLE].put(candle)
         elif msg_type == EventType.GREEKS:
-            return Greeks.from_stream(data)
+            greeks = Greeks.from_stream(data)
+            for greek in greeks:
+                await self._queues[EventType.GREEKS].put(greek)
         elif msg_type == EventType.PROFILE:
-            return Profile.from_stream(data)
+            profiles = Profile.from_stream(data)
+            for profile in profiles:
+                await self._queues[EventType.PROFILE].put(profile)
         elif msg_type == EventType.QUOTE:
-            return Quote.from_stream(data)
+            quotes = Quote.from_stream(data)
+            for quote in quotes:
+                await self._queues[EventType.QUOTE].put(quote)
         elif msg_type == EventType.SUMMARY:
-            return Summary.from_stream(data)
+            summaries = Summary.from_stream(data)
+            for summary in summaries:
+                await self._queues[EventType.SUMMARY].put(summary)
         elif msg_type == EventType.THEO_PRICE:
-            return TheoPrice.from_stream(data)
+            theo_prices = TheoPrice.from_stream(data)
+            for theo_price in theo_prices:
+                await self._queues[EventType.THEO_PRICE].put(theo_price)
         elif msg_type == EventType.TIME_AND_SALE:
-            return TimeAndSale.from_stream(data)
+            time_and_sales = TimeAndSale.from_stream(data)
+            for tas in time_and_sales:
+                await self._queues[EventType.TIME_AND_SALE].put(tas)
         elif msg_type == EventType.TRADE:
-            return Trade.from_stream(data)
+            trades = Trade.from_stream(data)
+            for trade in trades:
+                await self._queues[EventType.TRADE].put(trade)
+        elif msg_type == EventType.UNDERLYING:
+            underlyings = Underlying.from_stream(data)
+            for underlying in underlyings:
+                await self._queues[EventType.UNDERLYING].put(underlying)
         else:
-            msg = f'Unknown message type received from streamer: {message}'
-            raise TastytradeError(msg)
+            raise TastytradeError(f'Unknown message type received: {message}')
```

### Comparing `tastytrade-5.7/tastytrade/utils.py` & `tastytrade-6.0/tastytrade/utils.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.7/tastytrade/watchlists.py` & `tastytrade-6.0/tastytrade/watchlists.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import Dict, List, Optional
 
 import requests
 
 from tastytrade.instruments import InstrumentType
 from tastytrade.session import Session
 from tastytrade.utils import TastytradeJsonDataclass, validate_response
 
@@ -21,18 +21,18 @@
 
 class PairsWatchlist(TastytradeJsonDataclass):
     """
     Dataclass that represents a pairs watchlist object.
     """
     name: str
     order_index: int
-    pairs_equations: list[Pair]
+    pairs_equations: List[Pair]
 
     @classmethod
-    def get_pairs_watchlists(cls, session: Session) -> list['PairsWatchlist']:
+    def get_pairs_watchlists(cls, session: Session) -> List['PairsWatchlist']:
         """
         Fetches a list of all Tastytrade public pairs watchlists.
 
         :param session: the session to use for the request.
 
         :return: a list of :class:`PairsWatchlist` objects.
         """
@@ -72,24 +72,24 @@
 
 class Watchlist(TastytradeJsonDataclass):
     """
     Dataclass that represents a watchlist object (public or private),
     with functions to update, publish, modify and remove watchlists.
     """
     name: str
-    watchlist_entries: Optional[list[dict[str, str]]] = None
+    watchlist_entries: Optional[List[Dict[str, str]]] = None
     group_name: str = 'default'
     order_index: int = 9999
 
     @classmethod
     def get_public_watchlists(
         cls,
         session: Session,
         counts_only: bool = False
-    ) -> list['Watchlist']:
+    ) -> List['Watchlist']:
         """
         Fetches a list of all Tastytrade public watchlists.
 
         :param session: the session to use for the request.
         :param counts_only: whether to only fetch the counts of the watchlists.
 
         :return: a list of :class:`Watchlist` objects.
@@ -122,15 +122,15 @@
         validate_response(response)
 
         data = response.json()['data']
 
         return cls(**data)
 
     @classmethod
-    def get_private_watchlists(cls, session: Session) -> list['Watchlist']:
+    def get_private_watchlists(cls, session: Session) -> List['Watchlist']:
         """
         Fetches a the user's private watchlists.
 
         :param session: the session to use for the request.
 
         :return: a list of :class:`Watchlist` objects.
         """
```

### Comparing `tastytrade-5.7/tastytrade.egg-info/PKG-INFO` & `tastytrade-6.0/tastytrade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 5.7
+Version: 6.0
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -20,91 +20,90 @@
 .. image:: https://static.pepy.tech/badge/tastytrade
    :target: https://pepy.tech/project/tastytrade
    :alt: PyPI Downloads
 
 Tastytrade Python SDK
 =====================
 
-.. inclusion-marker
-
 A simple, reverse-engineered SDK for Tastytrade built on their (now mostly public) API. This will allow you to create trading algorithms for whatever strategies you may have quickly and painlessly in Python.
 
 Installation
 ------------
 
-.. code-block:: bash
+::
 
    $ pip install tastytrade
 
 Creating a session
 ------------------
 
 A session object is required to authenticate your requests to the Tastytrade API.
 You can create a real session using your normal login, or a certification (test) session using your certification login.
 
 .. code-block:: python
 
-   from tastytrade.session import Session
-   session = Session('username', 'password')
+   from tastytrade import ProductionSession
+   session = ProductionSession('username', 'password')
 
 Using the streamer
 ------------------
 
-The streamer is a websocket connection to the Tastytrade API that allows you to subscribe to real-time data for Quotes, Greeks, and more.
+The streamer is a websocket connection to dxfeed (the Tastytrade data provider) that allows you to subscribe to real-time data for quotes, greeks, and more.
 
 .. code-block:: python
 
-   from tastytrade.streamer import DataStreamer, EventType
+   from tastytrade import DataStreamer
+   from tastytrade.dxfeed import EventType
 
    streamer = await DataStreamer.create(session)
    subs_list = ['SPY', 'SPX']
 
-   # this function fetches quotes once, then closes the subscription
    await streamer.subscribe(EventType.QUOTE, subs_list)
+   # this example fetches quotes once, then exits
    quotes = []
    async for quote in streamer.listen():
       quotes.append(quote)
       if len(quotes) >= len(subs_list):
          break
    print(quotes)
 
 >>> [Quote(eventSymbol='SPY', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='Q', bidPrice=411.58, bidSize=400.0, askTime=0, askExchangeCode='Q', askPrice=411.6, askSize=1313.0), Quote(eventSymbol='SPX', eventTime=0, sequence=0, timeNanoPart=0, bidTime=0, bidExchangeCode='\x00', bidPrice=4122.49, bidSize='NaN', askTime=0, askExchangeCode='\x00', askPrice=4123.65, askSize='NaN')]
 
 Getting current positions
 -------------------------
 
 .. code-block:: python
    
-   from tastytrade.account import Account
+   from tastytrade import Account
 
    account = Account.get_accounts(session)[0]
    positions = account.get_positions(session)
    print(positions[0])
 
 >>> CurrentPosition(account_number='5WV69754', symbol='IAU', instrument_type=<InstrumentType.EQUITY: 'Equity'>, underlying_symbol='IAU', quantity=Decimal('20'), quantity_direction='Long', close_price=Decimal('37.09'), average_open_price=Decimal('37.51'), average_yearly_market_close_price=Decimal('37.51'), average_daily_market_close_price=Decimal('37.51'), multiplier=1, cost_effect='Credit', is_suppressed=False, is_frozen=False, realized_day_gain=Decimal('7.888'), realized_day_gain_effect='Credit', realized_day_gain_date=datetime.date(2023, 5, 19), realized_today=Decimal('0.512'), realized_today_effect='Debit', realized_today_date=datetime.date(2023, 5, 19), created_at=datetime.datetime(2023, 3, 31, 14, 38, 32, 58000, tzinfo=datetime.timezone.utc), updated_at=datetime.datetime(2023, 5, 19, 16, 56, 51, 920000, tzinfo=datetime.timezone.utc), mark=None, mark_price=None, restricted_quantity=Decimal('0'), expires_at=None, fixing_price=None, deliverable_type=None)
 
 Symbol search
 -------------
 
 .. code-block:: python
 
-   from tastytrade.search import symbol_search
+   from tastytrade import symbol_search
 
    results = symbol_search(session, 'AAP')
    print(results)
 
 >>> [SymbolData(symbol='AAP', description='Advance Auto Parts Inc.'), SymbolData(symbol='AAPD', description='Direxion Daily AAPL Bear 1X Shares'), SymbolData(symbol='AAPL', description='Apple Inc. - Common Stock'), SymbolData(symbol='AAPB', description='GraniteShares 1.75x Long AAPL Daily ETF'), SymbolData(symbol='AAPU', description='Direxion Daily AAPL Bull 1.5X Shares')]
 
 Placing an order
 ----------------
 
 .. code-block:: python
 
    from decimal import Decimal
-   from tastytrade.account import Account
+   from tastytrade import Account
    from tastytrade.instruments import Equity
    from tastytrade.order import NewOrder, OrderAction, OrderTimeInForce, OrderType, PriceEffect
 
    account = Account.get_account(session, '5WV69754')
    symbol = Equity.get_equity(session, 'USO')
    leg = symbol.build_leg(Decimal('5'), OrderAction.BUY_TO_OPEN)  # buy to open 5 shares
```

### Comparing `tastytrade-5.7/tastytrade.egg-info/SOURCES.txt` & `tastytrade-6.0/tastytrade.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 tastytrade/dxfeed/event.py
 tastytrade/dxfeed/greeks.py
 tastytrade/dxfeed/profile.py
 tastytrade/dxfeed/quote.py
 tastytrade/dxfeed/summary.py
 tastytrade/dxfeed/theoprice.py
 tastytrade/dxfeed/timeandsale.py
-tastytrade/dxfeed/trade.py
+tastytrade/dxfeed/trade.py
+tastytrade/dxfeed/underlying.py
```

