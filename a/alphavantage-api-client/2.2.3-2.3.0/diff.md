# Comparing `tmp/alphavantage_api_client-2.2.3-py3-none-any.whl.zip` & `tmp/alphavantage_api_client-2.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,26 @@
-Zip file size: 29080 bytes, number of entries: 21
--rw-rw-r--  2.0 unx      241 b- defN 23-May-30 16:40 alphavantage_api_client/__init__.py
--rw-rw-r--  2.0 unx      800 b- defN 22-Jul-02 20:13 alphavantage_api_client/__main__.py
--rw-rw-r--  2.0 unx    20255 b- defN 23-Jun-26 17:01 alphavantage_api_client/client.py
--rw-rw-r--  2.0 unx     7951 b- defN 23-Jun-26 17:01 alphavantage_api_client/models.py
--rw-rw-r--  2.0 unx     7725 b- defN 22-Sep-01 17:05 alphavantage_api_client/response_validation_rules.py
--rw-rw-r--  2.0 unx    11793 b- defN 22-Jul-27 01:15 alphavantage_api_client/ticker.py
--rw-rw-r--  2.0 unx      260 b- defN 22-May-21 19:54 alphavantage_api_client/version.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-26 17:01 examples/__init__.py
--rw-rw-r--  2.0 unx     7031 b- defN 23-Jun-26 17:01 examples/getting_started.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Jun-30 16:06 tests/__init__.py
--rw-rw-r--  2.0 unx     3373 b- defN 23-Jun-26 13:20 tests/mock_client.py
--rw-rw-r--  2.0 unx     1948 b- defN 22-Sep-01 17:05 tests/test_evaluate_company.py
--rw-rw-r--  2.0 unx     7788 b- defN 23-Jun-26 13:20 tests/test_mock_client_unit.py
--rw-rw-r--  2.0 unx    19650 b- defN 23-Jun-26 18:00 tests/test_multi_client_integration.py
--rw-rw-r--  2.0 unx    18640 b- defN 23-Jun-26 18:08 tests/test_single_client_cache_integration.py
--rw-rw-r--  2.0 unx     2966 b- defN 22-Jul-27 01:15 tests/test_ticker.py
--rw-rw-r--  2.0 unx     1067 b- defN 23-Jun-26 18:11 alphavantage_api_client-2.2.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx    14032 b- defN 23-Jun-26 18:11 alphavantage_api_client-2.2.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-26 18:11 alphavantage_api_client-2.2.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       39 b- defN 23-Jun-26 18:11 alphavantage_api_client-2.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1876 b- defN 23-Jun-26 18:11 alphavantage_api_client-2.2.3.dist-info/RECORD
-21 files, 127527 bytes uncompressed, 25980 bytes compressed:  79.6%
+Zip file size: 39518 bytes, number of entries: 24
+-rw-r--r--  2.0 unx      495 b- defN 23-Jul-15 16:04 alphavantage_api_client/__init__.py
+-rw-r--r--  2.0 unx      800 b- defN 23-Jul-15 16:04 alphavantage_api_client/__main__.py
+-rw-r--r--  2.0 unx    98974 b- defN 23-Jul-22 16:11 alphavantage_api_client/client.py
+-rw-r--r--  2.0 unx    10372 b- defN 23-Jul-15 16:04 alphavantage_api_client/models.py
+-rw-r--r--  2.0 unx     7725 b- defN 23-Jul-15 16:04 alphavantage_api_client/response_validation_rules.py
+-rw-r--r--  2.0 unx    11793 b- defN 23-Jul-15 16:04 alphavantage_api_client/ticker.py
+-rw-r--r--  2.0 unx      260 b- defN 23-Jul-15 16:04 alphavantage_api_client/version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 16:04 examples/__init__.py
+-rw-r--r--  2.0 unx     7485 b- defN 23-Jul-16 14:22 examples/getting_started.py
+-rw-r--r--  2.0 unx      149 b- defN 23-Jul-15 16:04 tests/__init__.py
+-rw-r--r--  2.0 unx     2810 b- defN 23-Jul-15 16:04 tests/mock_client.py
+-rw-r--r--  2.0 unx   100355 b- defN 23-Jul-22 16:11 tests/test_all_free_endpoints.py
+-rw-r--r--  2.0 unx     3301 b- defN 23-Jul-15 16:04 tests/test_all_paid_endpoints.py
+-rw-r--r--  2.0 unx      226 b- defN 23-Jul-22 16:11 tests/test_base.py
+-rw-r--r--  2.0 unx      366 b- defN 23-Jul-15 16:04 tests/test_mock_client_units.py
+-rw-r--r--  2.0 unx      273 b- defN 23-Jul-15 16:04 tests/test_multi_client_integration.py
+-rw-r--r--  2.0 unx      284 b- defN 23-Jul-15 16:04 tests/test_multi_client_paid_integration.py
+-rw-r--r--  2.0 unx      598 b- defN 23-Jul-22 16:07 tests/test_single_client_integration.py
+-rw-r--r--  2.0 unx     1987 b- defN 23-Jul-15 16:04 tests/test_single_client_limit_reached.py
+-rw-rw-r--  2.0 unx     1067 b- defN 23-Jul-22 16:17 alphavantage_api_client-2.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14014 b- defN 23-Jul-22 16:17 alphavantage_api_client-2.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-22 16:17 alphavantage_api_client-2.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       39 b- defN 23-Jul-22 16:17 alphavantage_api_client-2.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2156 b- defN 23-Jul-22 16:17 alphavantage_api_client-2.3.0.dist-info/RECORD
+24 files, 265621 bytes uncompressed, 35968 bytes compressed:  86.5%
```

## zipnote {}

```diff
@@ -27,38 +27,47 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/mock_client.py
 Comment: 
 
-Filename: tests/test_evaluate_company.py
+Filename: tests/test_all_free_endpoints.py
 Comment: 
 
-Filename: tests/test_mock_client_unit.py
+Filename: tests/test_all_paid_endpoints.py
+Comment: 
+
+Filename: tests/test_base.py
+Comment: 
+
+Filename: tests/test_mock_client_units.py
 Comment: 
 
 Filename: tests/test_multi_client_integration.py
 Comment: 
 
-Filename: tests/test_single_client_cache_integration.py
+Filename: tests/test_multi_client_paid_integration.py
+Comment: 
+
+Filename: tests/test_single_client_integration.py
 Comment: 
 
-Filename: tests/test_ticker.py
+Filename: tests/test_single_client_limit_reached.py
 Comment: 
 
-Filename: alphavantage_api_client-2.2.3.dist-info/LICENSE
+Filename: alphavantage_api_client-2.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: alphavantage_api_client-2.2.3.dist-info/METADATA
+Filename: alphavantage_api_client-2.3.0.dist-info/METADATA
 Comment: 
 
-Filename: alphavantage_api_client-2.2.3.dist-info/WHEEL
+Filename: alphavantage_api_client-2.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: alphavantage_api_client-2.2.3.dist-info/top_level.txt
+Filename: alphavantage_api_client-2.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: alphavantage_api_client-2.2.3.dist-info/RECORD
+Filename: alphavantage_api_client-2.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## alphavantage_api_client/__init__.py

```diff
@@ -1,4 +1,6 @@
 from alphavantage_api_client.client import AlphavantageClient
-from alphavantage_api_client.models import GlobalQuote, Quote, AccountingReport, CompanyOverview, RealGDP, \
-    CsvNotSupported
+from alphavantage_api_client.models import GlobalQuote, Quote, AccountingReport, CompanyOverview, EconomicIndicator, \
+    CsvNotSupported, TickerSearch, MarketStatus, MarketMovers, NewsAndSentiment, EarningsCalendar\
+    , EarningsCalendarItem,IpoCalendarItem, IpoCalendar, CurrencyQuote, Commodity
 from alphavantage_api_client.ticker import Ticker
+from alphavantage_api_client.response_validation_rules import ValidationRuleChecks
```

## alphavantage_api_client/client.py

```diff
@@ -1,442 +1,882 @@
 import time
 
 import requests
 import os
 import configparser
 from .response_validation_rules import ValidationRuleChecks
 import json
-from alphavantage_api_client.models import GlobalQuote, Quote, AccountingReport, CompanyOverview, RealGDP, \
-    CsvNotSupported
+from alphavantage_api_client.models import (
+    GlobalQuote,
+    Quote,
+    AccountingReport,
+    CompanyOverview,
+    EconomicIndicator,
+    CsvNotSupported,
+    TickerSearch,
+    MarketStatus,
+    NewsAndSentiment,
+    MarketMovers,
+    EarningsCalendar,
+    IpoCalendarItem,
+    IpoCalendar,
+    CurrencyQuote,
+    Commodity,
+)
 import copy
 import logging
 import hashlib
 from typing import Optional, Union
+import csv
 
 
 class ApiKeyNotFound(Exception):
-
     def __init__(self, message: str):
         super().__init__(message)
 
 
 class AlphavantageClient:
+    """Python wrapper around alpha vantage api
+
+    Create a simple python wrapper around alpha vantage api. Normalize responses so you have consistency across end points.
+    Provide direct access to each end point so customers who already use the API can have the flexibility. Make it easy
+    to debug, so users can track down issues quickly.
+
+        Typical usage example:
+
+            client = AlphavantageClient()
+            or
+            client = AlphavantageClient().should_retry_once().use_simple_cache()
+    """
+
     def __init__(self):
         self.__total_calls__ = 0
         self.__max_cache_size__ = 0
         self.__retry__ = False
         self.__first_successful_attempt__ = 0
         self.__use_cache__ = False
         self.__cache__ = {}
         # try to get api key from USER_PROFILE/.alphavantage
-        alphavantage_config_file_path = f'{os.path.expanduser("~")}{os.path.sep}.alphavantage'
-        msg = {"method": "__init__", "action": f"{alphavantage_config_file_path} config file found"}
+        alphavantage_config_file_path = (
+            f'{os.path.expanduser("~")}{os.path.sep}.alphavantage'
+        )
+        msg = {
+            "method": "__init__",
+            "action": f"{alphavantage_config_file_path} config file found",
+        }
         if os.path.exists(alphavantage_config_file_path):
             logging.info(json.dumps(msg))
             config = configparser.ConfigParser()
             config.read(alphavantage_config_file_path)
-            self.__api_key__ = config['access']['api_key']
+            self.__api_key__ = config["access"]["api_key"]
             return
         # try to get from an environment variable
-        elif os.environ.get('ALPHAVANTAGE_API_KEY') is not None:
-            self.__api_key__ = os.environ.get('ALPHAVANTAGE_API_KEY')
+        elif os.environ.get("ALPHAVANTAGE_API_KEY") is not None:
+            self.__api_key__ = os.environ.get("ALPHAVANTAGE_API_KEY")
             msg["action"] = f"api key found from environment"
             logging.info(json.dumps(msg))
             return
         else:
             self.__api_key__ = ""
 
     def __build_url_from_args__(self, event: dict):
-        """
+        """private method to construct a url from requested api configuration
 
         Args:
-            event:
+            event: the params
 
         Returns:
-            :rtype: str
+            a string in url format
         """
-        url = f'https://www.alphavantage.co/query?'
+        url = f"https://www.alphavantage.co/query?"
         # build url from event
         for property in event:
-            url += f'{property}={event[property]}&'
+            url += f"{property}={event[property]}&"
         url = url[:-1]
         return url
 
     def __inject_values__(self, default_values: dict, dest_obj: dict):
-        """
+        """private method: inserts values into the destination dict. This will not overwrite values
 
         Args:
-            default_values:
-            dest_obj:
+            default_values: The required values to be inserted into the dest_obj
+            dest_obj: the dict to be hydrated with the default_values
 
         Returns:
-            :rtype: None
+            None
 
         """
         # inject defaults for missing values
         for default_key in default_values:
             if default_key not in dest_obj or dest_obj[default_key] is None:
                 dest_obj[default_key] = default_values[default_key]
 
-    def __create_api_request_from__(self, defaults: dict, event: dict):
-        """
-
-        Args:
-            defaults:
-            event:
-
-        Returns:
-            :rtype: dict
-        """
-        if event is not None:
+    def __create_api_request_from__(self, defaults: dict, event: Union[str, dict]):
+        json_request = event
+        if isinstance(event, str):
+            json_request = {"symbol": event} #assume the symbol
+        elif json_request is not None:
             json_request = event.copy()
         else:
             json_request = {}
         self.__inject_values__(defaults, json_request)
 
         return json_request
 
     def should_retry_once(self, retry: bool = True):
+        """Retry api call when limit reached has been detected
+
+        At present the Alpha Vantage API only allows 5 calls per min with a free account. This means you would need to
+        build retry logic to maximize your calls.  We have already done that for you! As a result, the client
+        will calculate the time from the last call and pause up to a minute before making a subsequent call.
+
+        Args:
+            retry: Flag to indicate whether you want to retry when limit has been reached
+
+        Returns:
+            AlphavantageClient
+
+        """
         self.__retry__ = retry
 
         return self
 
     def use_simple_cache(self, use_cache: bool = True, max_cache_size: int = 100):
-        """
+        """First in / First Out Cache to reduce the amount of calls you need to make to the alpha vantage api
+
+        An In-Memory Caching mechanism where your parameters (i.e. symbol, function, interval, format, etc) are used as
+        a key into a dictionary. This is similar to how SQL uses the SQL statement to cache it's responses. If you
+        have already requested data with those attributes then it will simply return it from the cache. The cache will
+        continue to grow until you call the clear_cache()
+
+
         First in First Out Cache
         Args:
-            use_cache:
+            use_cache: Flag to indicate whether you want to turn on caching
             max_cache_size: Max size of the cache.
 
         Returns:
 
         """
         self.__use_cache__ = use_cache
         self.__max_cache_size__ = max_cache_size
 
         return self
 
     def get_internal_metrics(self) -> dict:
+        """Obtain the total calls, retry setting and the first successful attempt
+
+        We want to provide you will some usefull statistics that may help you troubleshoot or understand your usage.
+
+        Returns:
+            A dict of relevaant details about your usage
+            totals calls - how many total calls have been made by the client
+            retry - your retry flag
+            first_successful_attempt - the time as a float
+
+        """
         total_calls = self.__total_calls__
         retry = self.__retry__
         first_successful_attempt = self.__first_successful_attempt__
         metrics = {
             "total_calls": total_calls,
             "retry": retry,
-            "first_successful_attempt": first_successful_attempt
+            "first_successful_attempt": first_successful_attempt,
         }
         return metrics
 
     def with_api_key(self, api_key: str):
-        """Specify the API Key when you are storing it somewhere other than in ini file or environment variable
+        """Specify your alpha vantage API Key
+
+        There are a few ways you can specify your alpha vantage api key:
+        1. This method ;-)
+        2. ~/.alphavantage
+        3. ALPHAVANTAGE_API_KEY env variable
+        4. within each request event dict using the same key name as the api expects (i.e. apiKey)
 
-        When you are storing your api key somewhere other than ~/.alphavantage or ALPHAVANTAGE_API_KEY env variable
         Args:
-            api_key (str): Your api key from alphavantage
+            api_key (str): Your api key from alpha vantage
 
         Returns:
-            :rtype: AlphavantageClient
+            This AlphavantageClient
         """
         if api_key is None or len(api_key) == 0:
-            raise ApiKeyNotFound("API Key is null or empty. Please specify a valid api key")
+            raise ApiKeyNotFound(
+                "API Key is null or empty. Please specify a valid api key"
+            )
         self.__api_key__ = api_key
 
         return self
 
     def get_global_quote(self, event: Union[str, dict]) -> GlobalQuote:
-        """ Lightweight access to obtain stock quote data
+        """A lightweight alternative to the time series APIs
 
-        A lightweight alternative to the time series APIs, this service returns the price and volume information
-        for a token of your choice.
+        This service returns the price and volume information
+        for the equity of your choice.
         Args:
-            event (dict): A ``dict`` containing the parameters supported by the api.
-            Minimum required value is ``symbol (str)``
+            event: A ticker symbol str OR dict of parameters to be sent to the API
 
         Returns:
-            :rtype: GlobalQuote
+            A GlobalQuote for the requested equity
 
         """
-        event_dict = event
-        if isinstance(event, str):
-            event_dict = {
-                "symbol": event
-            }
+
+        defaults = {"function": "GLOBAL_QUOTE"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return GlobalQuote.model_validate(json_response)
+
+    def get_daily_quote(self, event: Union[str, dict]) -> Quote:
+        """As traded daily time series price history
+
+        Includes: date, daily open, daily high, daily low, daily close, daily
+        volume for your specified equity covering 20+ years of historical data. If you are also interested in
+        split/dividend-adjusted historical data, please use the get_daily_adjusted_quote(...), which covers adjusted
+        close values and historical split and dividend events.
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns:
+            The Quote for the requested equity
+
+        """
+        # default params
         defaults = {
-            "function": "GLOBAL_QUOTE"
+            "datatype": "json",
+            "function": "TIME_SERIES_DAILY",
+            "outputsize": "compact",
         }
-        json_request = self.__create_api_request_from__(defaults, event_dict)
+        json_request = self.__create_api_request_from__(defaults, event)
         json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
 
-        return GlobalQuote.parse_obj(json_response)
+        return Quote.model_validate(json_response)
+
+    def get_daily_adjusted_quote(self, event: Union[str, dict]) -> Quote:
+        """As-traded daily open/high/low/close/volume values
+
+        Daily adjusted close values, and historical split/dividend events of the global equity specified, covering
+        20+ years of historical data.
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns:
+            The Quote for the requested equity
 
-    def get_daily_quote(self, event: dict) -> Quote:
         """
-        This API returns raw (as-traded) daily time series (date, daily open, daily high, daily low, daily close, daily
-        volume) of the global equity specified, covering 20+ years of historical data. If you are also interested in
-        split/dividend-adjusted historical data, please use the Daily Adjusted API, which covers adjusted close values
-        and historical split and dividend events.
+        # default params
+        defaults = {
+            "datatype": "json",
+            "function": "TIME_SERIES_DAILY_ADJUSTED",
+            "outputsize": "compact",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_weekly_quote(self, event: Union[str, dict]) -> Quote:
+        """weekly time series trading data
+
+        This API returns weekly time series (last trading day of each week, weekly open, weekly high, weekly low,
+        weekly close, weekly volume) of the global equity specified, covering 20+ years of historical data.
+
         Args:
-            event: dict, required
+            event: A ticker symbol str OR dict of parameters to be sent to the API
 
-        Returns: Quote
+        Returns:
+            The Quote for the requested equity
 
         """
         # default params
-        defaults = {"datatype": "json", "function": "TIME_SERIES_DAILY",
-                    "outputsize": "compact"}
+        defaults = {
+            "datatype": "json",
+            "function": "TIME_SERIES_WEEKLY",
+            "outputsize": "compact",
+        }
         json_request = self.__create_api_request_from__(defaults, event)
         json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
 
-        return Quote.parse_obj(json_response)
+        return Quote.model_validate(json_response)
+
+    def get_weekly_adjusted_quote(self, event: Union[str, dict]) -> Quote:
+        """weekly adjusted time series trading data
 
-    def get_intraday_quote(self, event: dict) -> Quote:
-        """ Intraday time series data covering extened trading hours.
+        This API returns weekly adjusted time series (last trading day of each week, weekly open, weekly high,
+        weekly low, weekly close, weekly adjusted close, weekly volume, weekly dividend) of the global equity
+        specified, covering 20+ years of historical data.
 
-        This API returns intraday time series of the equity specified, covering extended trading hours where applicable
-        (e.g., 4:00am to 8:00pm Eastern Time for the US market). The intraday data is derived from the Securities
-        Information Processor (SIP) market-aggregated data. You can query both raw (as-traded) and
-        split/dividend-adjusted intraday data from this endpoint.  This API returns the most recent 1-2 months of
-        intraday data and is best suited for short-term/medium-term charting and trading strategy development.
-        If you are targeting a deeper intraday history, please use the Extended Intraday API.
         Args:
-            event (dict): A Dictionary of parameters that will be passed to the api.
-            Minimum required is ``symbol`` = ``str``
+            event: A ticker symbol str OR dict of parameters to be sent to the API
 
         Returns:
-            :rtype: Quote
+            The Quote for the requested equity
 
         """
         # default params
-        defaults = {"symbol": None, "datatype": "json", "function": "TIME_SERIES_INTRADAY",
-                    "interval": "60min", "slice": "year1month1",
-                    "outputsize": "compact"}
-        event_dict = event
-        if isinstance(event, str):
-            event_dict = {
-                "symbol": event
-            }
-        json_request = self.__create_api_request_from__(defaults, event_dict)
+        defaults = {"datatype": "json", "function": "TIME_SERIES_WEEKLY_ADJUSTED"}
+        json_request = self.__create_api_request_from__(defaults, event)
         json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
 
-        return Quote.parse_obj(json_response)
+        return Quote.model_validate(json_response)
+
+    def get_monthly_quote(self, event: Union[str, dict]) -> Quote:
+        """monthly time series trading data
+
+        This API returns monthly time series (last trading day of each month, monthly open, monthly high,
+        monthly low, monthly close, monthly volume) of the global equity specified, covering 20+ years
+        of historical data.
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns:
+            The Quote for the requested equity
 
-    def get_income_statement(self, event: dict) -> AccountingReport:
         """
-        This API returns the annual and quarterly income statements for the company of interest, with
-        normalized fields mapped to GAAP and IFRS taxonomies of the SEC. Data is generally refreshed on the same day
-        a company reports its latest earnings and financials.
+        # default params
+        defaults = {"datatype": "json", "function": "TIME_SERIES_MONTHLY"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_monthly_adjusted_quote(self, event: Union[str, dict]) -> Quote:
+        """monthly adjusted time series trading data
+
+        This API returns monthly adjusted time series (last trading day of each month, monthly open, monthly high,
+        monthly low, monthly close, monthly adjusted close, monthly volume, monthly dividend) of the equity specified,
+        covering 20+ years of historical data.
 
         Args:
-            event (dict): A Dictionary of parameters that will be passed to the api.
-            Minimum required is ``symbol`` = ``str``
+            event: A ticker symbol str OR dict of parameters to be sent to the API
 
         Returns:
-            :rtype: AccountingReport
+            The Quote for the requested equity
 
         """
+        # default params
+        defaults = {"datatype": "json", "function": "TIME_SERIES_MONTHLY_ADJUSTED"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_intraday_quote(self, event: Union[str, dict]) -> Quote:
+        """Intraday time series data covering extended trading hours.
 
+        Covering extended trading hours when applicable (e.g., 4:00am to 8:00pm Eastern Time for the US market).
+        The intraday data is derived from the Securities Information Processor (SIP) market-aggregated data.
+        You can query both raw (as-traded) and split/dividend-adjusted intraday data from this endpoint.
+        This API returns the most recent 1-2 months of intraday data and is best suited for short-term/medium-term
+        charting and trading strategy development.
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns:
+             The Quote for the requested equity
+
+        """
+        # default params
         defaults = {
-            "function": "INCOME_STATEMENT",
-            "datatype": "json"
+            "symbol": None,
+            "datatype": "json",
+            "function": "TIME_SERIES_INTRADAY",
+            "interval": "60min",
+            "outputsize": "compact"
         }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_income_statement(self, event: Union[str, dict]) -> AccountingReport:
+        """annual and quarterly income statements for the company of interest
+
+        Includes normalized fields mapped to GAAP and IFRS taxonomies of the SEC. Data is generally
+        refreshed on the same day a company reports its latest earnings and financials.
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns:
+            The AccountingReport for the requested equity
+
+        """
+
+        defaults = {"function": "INCOME_STATEMENT", "datatype": "json"}
         event_dict = event
         if isinstance(event, str):
-            event_dict = {
-                "symbol": event
-            }
+            event_dict = {"symbol": event}
         if event_dict.get("datatype") == "csv":
             raise CsvNotSupported(defaults.get("function"), event_dict)
         json_request = self.__create_api_request_from__(defaults, event_dict)
         json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
 
-        return AccountingReport.parse_obj(json_response)
+        return AccountingReport.model_validate(json_response)
 
-    def get_balance_sheet(self, event: dict) -> AccountingReport:
-        defaults = {
-            "function": "BALANCE_SHEET",
-            "datatype": "json"
-        }
+    def get_balance_sheet(self, event: Union[str, dict]) -> AccountingReport:
+        """annual and quarterly balance sheets for the company of interest
+
+        Includes normalized fields mapped to GAAP and IFRS taxonomies of the SEC. Data is generally refreshed on the
+        same day a company reports its latest earnings and financials.
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns:
+            The AccountingReport for the requested equity
+
+        """
+        defaults = {"function": "BALANCE_SHEET", "datatype": "json"}
         event_dict = event
         if isinstance(event, str):
-            event_dict = {
-                "symbol": event
-            }
+            event_dict = {"symbol": event}
         if event_dict.get("datatype") == "csv":
             raise CsvNotSupported(defaults.get("function"), event_dict)
 
         json_request = self.__create_api_request_from__(defaults, event_dict)
         json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
 
-        return AccountingReport.parse_obj(json_response)
+        return AccountingReport.model_validate(json_response)
 
-    def get_cash_flow(self, event: dict) -> AccountingReport:
-        """
-        This API returns the annual and quarterly cash flow for the company of interest, with normalized fields
-        mapped to GAAP and IFRS taxonomies of the SEC. Data is generally refreshed on the same day a company reports
-        its latest earnings and financials.
+    def get_cash_flow(self, event: Union[str, dict]) -> AccountingReport:
+        """annual and quarterly cash flow for the company of interest
+
+        Includes normalized fields mapped to GAAP and IFRS taxonomies of the SEC. Data is generally refreshed on
+        the same day a company reports its latest earnings and financials.
         Args:
-            event (dict): A Dictionary of parameters that will be passed to the api.
-            Minimum required is ``symbol`` = ``str``
+            event: A ticker symbol str OR dict of parameters to be sent to the API
 
         Returns:
-            :rtype: AccountingReport
+            The AccountingReport for the requested equity
 
         """
-        defaults = {
-            "function": "CASH_FLOW",
-            "datatype": "json"
-        }
+        defaults = {"function": "CASH_FLOW", "datatype": "json"}
         event_dict = event
         if isinstance(event, str):
-            event_dict = {
-                "symbol": event
-            }
+            event_dict = {"symbol": event}
         if event_dict.get("datatype") == "csv":
             raise CsvNotSupported(defaults.get("function"), event_dict)
         json_request = self.__create_api_request_from__(defaults, event_dict)
         json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
 
-        return AccountingReport.parse_obj(json_response)
+        return AccountingReport.model_validate(json_response)
 
-    def get_earnings(self, event: Union[str, dict]) -> AccountingReport:
-        """
-        This API returns the annual and quarterly earnings (EPS) for the company of interest. Quarterly data also
-        includes analyst estimates and surprise metrics.
+    def get_earnings(self, event: Union[str, Union[str, dict]]) -> AccountingReport:
+        """annual and quarterly earnings (EPS) for the company of interest
+
+        The quarterly data also includes analyst estimates and surprise metrics.
 
         Args:
-            event (dict): A Dictionary of parameters that will be passed to the api.
-            Minimum required is ``symbol`` = ``str``
+            event: A ticker symbol str OR dict of parameters to be sent to the API
 
         Returns:
-            :rtype: AccountingReport
+            The AccountingReport for the requested equity
 
         """
-        defaults = {
-            "function": "EARNINGS",
-            "datatype": "json"
-        }
+        defaults = {"function": "EARNINGS", "datatype": "json"}
         event_dict = event
         if isinstance(event, str):
-            event_dict = {
-                "symbol": event
-            }
+            event_dict = {"symbol": event}
 
         if event_dict.get("datatype") == "csv":
             raise CsvNotSupported(defaults.get("function"), event_dict)
         json_request = self.__create_api_request_from__(defaults, event_dict)
         json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
 
-        return AccountingReport.parse_obj(json_response)
+        return AccountingReport.model_validate(json_response)
+
+    def get_company_overview(self, event: Union[str, dict]) -> CompanyOverview:
+        """company information, financial ratios, and other key metrics for the equity specified.
 
-    def get_company_overview(self, event: dict) -> CompanyOverview:
-        """
-        This API returns the company information, financial ratios, and other key metrics for the equity specified.
         Data is generally refreshed on the same day a company reports its latest earnings and financials.
 
         Args:
-            event (dict): A Dictionary of parameters that will be passed to the api.
-            Minimum required is ``symbol`` = ``str``
+            event: A ticker symbol str OR dict of parameters to be sent to the API
 
         Returns:
-            Return a CompanyOverview Object
+            The CompanyOverview for the requested equity
 
         """
-        defaults = {
-            "function": "OVERVIEW"
-        }
+        defaults = {"function": "OVERVIEW"}
         event_dict = event
         if isinstance(event, str):
-            event_dict = {
-                "symbol": event
-            }
+            event_dict = {"symbol": event}
         if event_dict.get("datatype") == "csv":
             raise CsvNotSupported(defaults.get("function"), event_dict)
         json_request = self.__create_api_request_from__(defaults, event_dict)
         json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
 
-        return CompanyOverview.parse_obj(json_response)
+        return CompanyOverview.model_validate(json_response)
 
-    def get_crypto_intraday(self, event: dict) -> Quote:
-        """
-        This API returns intraday time series (timestamp, open, high, low, close, volume) of the cryptocurrency
-        specified, updated realtime.
+    def get_crypto_intraday(self, event: dict) -> CurrencyQuote:
+        """Returns crypto intraday time series price data
+
+        Includes: timestamp, open, high, low, close, volume of the cryptocurrency specified, updated realtime.
 
         Args:
-            event (dict): A Dictionary of parameters that will be passed to the api.
-            Minimum required is ``symbol`` = (``str``)
+            event: dict of parameters to be sent to the API
 
         Returns:
-            :rtype: Quote
+            The CurrencyQuote for the requested equity
 
         """
         defaults = {
             "function": "CRYPTO_INTRADAY",
-            "interval": "5min",
             "market": "USD",
-            "outputsize": "compact"
+            "interval": "60min",
+            "outputsize": "compact",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+        # print(json.dumps(json_response))
+        return CurrencyQuote.model_validate(json_response)
+
+    def get_crypto_daily(self, event: dict) -> CurrencyQuote:
+        """returns the daily historical time series for a digital currency (e.g., BTC)
+
+        refreshed daily at midnight (UTC). Prices and volumes are quoted in both the market-specific 
+        currency and USD traded on a specific market (e.g., CNY/Chinese Yuan)
+
+        Args:
+            event: A dict of parameters that will be passed to the api.
+
+        Returns:
+            The CurrencyQuote for the requested equity
+
+        """
+        defaults = {"function": "DIGITAL_CURRENCY_DAILY", "market": "CNY"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+        return CurrencyQuote.model_validate(json_response)
+
+    def get_crypto_weekly(self, event: dict) -> CurrencyQuote:
+        """Returns the daily historical time series for a digital currency (e.g., BTC)
+
+        As traded on a specific market (e.g., CNY/Chinese Yuan), refreshed daily at midnight (UTC). Prices and
+        volumes are quoted in both the market-specific currency and USD.
+
+        Args:
+            event: A dict of parameters that will be passed to the api.
+
+        Returns:
+            The CurrencyQuote for the requested equity
+
+        """
+        defaults = {"function": "DIGITAL_CURRENCY_WEEKLY", "market": "CNY"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+        return CurrencyQuote.model_validate(json_response)
+
+    def get_crypto_monthly(self, event: dict) -> CurrencyQuote:
+        """Returns the monthly historical time series for a digital currency (e.g., BTC)
+
+        Refreshed daily at midnight (UTC). Prices and volumes are quoted in both the market-specific currency and USD.
+
+        Args:
+            event: A dict of parameters that will be passed to the api.
+
+        Returns:
+            The CurrencyQuote for the requested equity
+
+        """
+        defaults = {"function": "DIGITAL_CURRENCY_MONTHLY", "market": "CNY"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+        return CurrencyQuote.model_validate(json_response)
+
+    def get_currency_exchange_rates(self, event: dict) -> CurrencyQuote:
+        """returns the exchange rate for any pair of digital currency (e.g., Bitcoin) or physical currency (e.g., USD).
+
+        Args:
+            event: A Dictionary of parameters that will be passed to the api.
+
+        Returns:
+            The CurrencyQuote for the requested equity
+
+        """
+        defaults = {"function": "CURRENCY_EXCHANGE_RATE"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+        return CurrencyQuote.model_validate(json_response)
+
+    def get_real_gdp(self, event: dict = None) -> EconomicIndicator:
+        """Returns the annual and quarterly Real GDP of the United States.
+
+        Source: U.S. Bureau of Economic Analysis, Real Gross Domestic Product, retrieved from FRED, Federal
+        Reserve Bank of St. Louis. This data feed uses the FRED® API but is not endorsed or certified by the Federal
+        Reserve Bank of St. Louis. By using this data feed, you agree to be bound by the FRED® API Terms of Use.
+
+        Args:
+            event: Not required. You can pass in any parameters supported by the api
+
+        Returns:
+            The EconomicIndicator for the requested equity
+
+        """
+        defaults = {"function": "REAL_GDP", "interval": "annual", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return EconomicIndicator.model_validate(json_response)
+
+    def get_treasury_yield(self, event: dict = None) -> EconomicIndicator:
+        """Returns the daily, weekly, and monthly US treasury yield of a given maturity timeline.
+
+        Source: Board of Governors of the Federal Reserve System (US), Market Yield on U.S. Treasury Securities
+        at 3-month, 2-year, 5-year, 7-year, 10-year, and 30-year Constant Maturities, Quoted on an Investment Basis,
+        retrieved from FRED, Federal Reserve Bank of St. Louis. This data feed uses the FRED® API but is not endorsed
+        or certified by the Federal Reserve Bank of St. Louis. By using this data feed, you agree to be bound by the
+        FRED® API Terms of Use.
+
+        Args:
+            event: Not required. You can pass in any parameters supported by the api
+
+        Returns:
+            The EconomicIndicator for the requested equity
+
+        """
+        defaults = {
+            "function": "TREASURY_YIELD",
+            "interval": "monthly",
+            "datatype": "json",
+            "maturity": "10year",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return EconomicIndicator.model_validate(json_response)
+
+    def get_federal_funds_rate(self, event: dict = None) -> EconomicIndicator:
+        """returns the daily, weekly, and monthly federal funds rate (interest rate) of the United States.
+
+        Source: Board of Governors of the Federal Reserve System (US), Federal Funds Effective Rate, retrieved from
+        FRED, Federal Reserve Bank of St. Louis (https://fred.stlouisfed.org/series/FEDFUNDS). This data feed uses the
+        FRED® API but is not endorsed or certified by the Federal Reserve Bank of St. Louis. By using this data feed,
+        you agree to be bound by the FRED® API Terms of Use.
+
+        Args:
+            event: Not required. You can pass in any parameters supported by the api
+
+        Returns:
+            The EconomicIndicator for the requested equity
+
+        """
+        defaults = {
+            "function": "FEDERAL_FUNDS_RATE",
+            "interval": "monthly",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return EconomicIndicator.model_validate(json_response)
+
+    def get_cpi(self, event: dict = None) -> EconomicIndicator:
+        """Returns the monthly and semiannual consumer price index (CPI) of the United States.
+
+        CPI is widely regarded as the barometer of inflation levels in the broader economy.
+        Source: U.S. Bureau of Labor Statistics, Consumer Price Index for All Urban Consumers: All Items in U.S. City
+        Average, retrieved from FRED, Federal Reserve Bank of St. Louis. This data feed uses the FRED® API but is not
+        endorsed or certified by the Federal Reserve Bank of St. Louis. By using this data feed, you agree to be
+        bound by the FRED® API Terms of Use.
+
+        Args:
+            event: Not required. You can pass in any parameters supported by the api
+
+        Returns:
+            The EconomicIndicator for the requested equity
+
+        """
+        defaults = {"function": "CPI", "interval": "monthly", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return EconomicIndicator.model_validate(json_response)
+
+    def get_inflation(self, event: dict = None) -> EconomicIndicator:
+        """Returns the annual inflation rates (consumer prices) of the United States.
+
+        Source: World Bank, Inflation, consumer prices for the United States, retrieved from FRED, Federal Reserve Bank
+        of St. Louis. This data feed uses the FRED® API but is not endorsed or certified by the Federal Reserve
+        Bank of St. Louis. By using this data feed, you agree to be bound by the FRED® API Terms of Use.
+
+        Args:
+            event: Not required. You can pass in any parameters supported by the api
+
+        Returns:
+            The EconomicIndicator for the requested equity
+
+        """
+        defaults = {
+            "function": "INFLATION",
+            "datatype": "json",
         }
         json_request = self.__create_api_request_from__(defaults, event)
         json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
 
-        return Quote.parse_obj(json_response)
+        return EconomicIndicator.model_validate(json_response)
+
+    def get_retails_sales(self, event: dict = None) -> EconomicIndicator:
+        """returns the monthly Advance Retail Sales: Retail Trade data of the United States.
+
+        Source: U.S. Census Bureau, Advance Retail Sales: Retail Trade, retrieved from FRED,
+        Federal Reserve Bank of St. Louis (https://fred.stlouisfed.org/series/RSXFSN). This data feed uses the FRED®
+        API but is not endorsed or certified by the Federal Reserve Bank of St. Louis. By using this data feed, you
+        agree to be bound by the FRED® API Terms of Use.
+
+        Args:
+            event: Not required. You can pass in any parameters supported by the api
+
+        Returns:
+            The EconomicIndicator for the requested equity
 
-    def get_real_gdp(self, event: dict = None) -> RealGDP:
         """
+        defaults = {
+            "function": "RETAIL_SALES",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return EconomicIndicator.model_validate(json_response)
+
+    def get_durable_goods_orders(self, event: dict = None) -> EconomicIndicator:
+        """Returns the monthly manufacturers' new orders of durable goods in the United States.
 
-        This API returns the annual and quarterly Real GDP of the United States.
+        Source: U.S. Census Bureau, Manufacturers' New Orders: Durable Goods, retrieved from FRED, Federal Reserve
+        Bank of St. Louis (https://fred.stlouisfed.org/series/UMDMNO). This data feed uses the FRED® API but is not
+        endorsed or certified by the Federal Reserve Bank of St. Louis. By using this data feed, you agree to be bound
+        by the FRED® API Terms of Use.
 
         Args:
             event (dict): Not required. You can pass in any parameters supported by the api
 
         Returns:
-            :rtype: RealGDP
+            The EconomicIndicator for the requested equity
+
+        """
+        defaults = {
+            "function": "DURABLES",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return EconomicIndicator.model_validate(json_response)
+
+    def get_unemployment(self, event: dict = None) -> EconomicIndicator:
+        """Returns the monthly unemployment data of the United States.
+
+        The unemployment rate represents the number of unemployed as a percentage of the labor force. Labor force
+        data are restricted to people 16 years of age and older, who currently reside in 1 of the 50 states or the
+        District of Columbia, who do not reside in institutions (e.g., penal and mental facilities, homes for the aged),
+        and who are not on active duty in the Armed Forces (source).
+
+        Source: U.S. Bureau of Labor Statistics, Unemployment Rate, retrieved from FRED, Federal Reserve Bank of
+        St. Louis. This data feed uses the FRED® API but is not endorsed or certified by the Federal Reserve Bank of
+        St. Louis. By using this data feed, you agree to be bound by the FRED® API Terms of Use.
+
+        Args:
+            event: Not required. You can pass in any parameters supported by the api
+
+        Returns:
+            The EconomicIndicator for the requested equity
+
+        """
+        defaults = {
+            "function": "UNEMPLOYMENT",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return EconomicIndicator.model_validate(json_response)
+
+    def get_nonfarm_payroll(self, event: dict = None) -> EconomicIndicator:
+        """Returns the monthly US All Employees Nonfarm, a measure of the number of U.S.
+
+        Workers in the economy that excludes proprietors, private household employees, unpaid volunteers,
+        farm employees, and the unincorporated self-employed.
+
+        Source: U.S. Bureau of Labor Statistics, All Employees, Total Nonfarm, retrieved from FRED, Federal Reserve
+        Bank of St. Louis. This data feed uses the FRED® API but is not endorsed or certified by the Federal Reserve
+        Bank of St. Louis. By using this data feed, you agree to be bound by the FRED® API Terms of Use.
+
+        Args:
+            event: Not required. You can pass in any parameters supported by the api
+
+        Returns:
+            The EconomicIndicator for the requested equity
 
         """
         defaults = {
-            "function": "REAL_GDP",
-            "interval": "annual",
-            "datatype": "json"
+            "function": "NONFARM_PAYROLL",
+            "datatype": "json",
         }
         json_request = self.__create_api_request_from__(defaults, event)
         json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
 
-        return RealGDP.parse_obj(json_response)
+        return EconomicIndicator.model_validate(json_response)
+
+    def get_real_gdp_per_capita(self, event: dict = None) -> EconomicIndicator:
+        """Returns the quarterly Real GDP per Capita data of the United States.
+
+        Source: U.S. Bureau of Economic Analysis, Real gross domestic product per capita, retrieved from FRED,
+        Federal Reserve Bank of St. Louis. This data feed uses the FRED® API but is not endorsed or certified by the
+        Federal Reserve Bank of St. Louis. By using this data feed, you agree to be bound by the FRED® API Terms of Use.
+
+        Args:
+            event: Not required. You can pass in any parameters supported by the api
+
+        Returns:
+            :rtype: EconomicIndicator
+
+        """
+        defaults = {"function": "REAL_GDP_PER_CAPITA", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return EconomicIndicator.model_validate(json_response)
 
     def get_technical_indicator(self, event: dict) -> Quote:
         """
         Default technical indicator is SMA. You can change this by passing in ``function`` = ``[your indicator]``
 
         Args:
             event (dict): Parameters supported by the API
 
         Returns:
             :rtype: Quote
 
         """
-        defaults = {
-            "function": "SMA",
-            "interval": "monthly",
-            "datatype": "json"
-        }
+        defaults = {"function": "SMA", "interval": "monthly", "datatype": "json"}
         json_request = self.__create_api_request_from__(defaults, event)
         json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
         json_response["indicator"] = event.get("function")
 
-        return Quote.parse_obj(json_response)
+        return Quote.model_validate(json_response)
 
-    def get_data_from_alpha_vantage(self, event: dict, should_retry: bool = False) -> dict:
-        """
-        This is the underlying function that talks to alphavantage api.  Feel free to pass in any parameters supported
-        by the api.  You will receive a dictionary with the response from the web api. In addition, you will obtain
-        the ``success``, ``error_message`` and ``limit_reached`` fields.
+    def get_data_from_alpha_vantage(
+        self, event: dict, should_retry: bool = False
+    ) -> dict:
+        """Underlying function that talks to alphavantage api.
+
+        Feel free to pass in any parameters supported by the api.  You will receive a dictionary with the response
+        from the web api. In addition, you will obtain the success, error_message and limit_reached fields.
         Args:
-            event (dictionary): The url parameters supported by the web api
+            event: dict of the url parameters supported by the web api
 
         Returns:
-            :rtype: dict
+            A dict of the response from alpha vantage api. success, error_message and limit_reached fields are injected
+            into the dict for your reference.
 
         """
         # validate api key and insert into the request if needed
         checks = ValidationRuleChecks().from_customer_request(event)
         self.__validate_api_key__(checks, event)
 
         # create a version of the event without api key
@@ -460,84 +900,1701 @@
         # retry once if allowed and needed
         if checks.expect_limit_not_reached().passed() and should_retry:
             self.__sleep__()
             result = self.get_data_from_alpha_vantage(event, False)
             self.__first_successful_attempt__ = time.perf_counter()
             return result
 
-        # not all calls will have a symbol in the call to alphavantage.... if so we can to capture it.
+        # not all calls will have a symbol in the call to alphavantage.... if so we can, capture it.
         if "symbol" in event:
-            requested_data['symbol'] = event['symbol']
+            requested_data["symbol"] = event["symbol"]
 
         # put into cache if allowed
         if self.__use_cache__:
             self.__put_item_into_cache__(loggable_event, requested_data)
 
-        logging.info(json.dumps({"method": "get_data_from_alpha_vantage"
-                                    , "action": "return_value", "data": requested_data, "event": loggable_event}))
+        logging.info(
+            json.dumps(
+                {
+                    "method": "get_data_from_alpha_vantage",
+                    "action": "return_value",
+                    "data": requested_data,
+                    "event": loggable_event,
+                }
+            )
+        )
 
         return requested_data
 
     def __put_item_into_cache__(self, event, results):
-
         if len(self.__cache__) >= self.__max_cache_size__:
             self.__cache__.clear()
 
         hash_str = json.dumps(event, sort_keys=True)
         self.__cache__[hash_str] = results
 
     def __get_item_from_cache__(self, event):
         hash_str = json.dumps(event, sort_keys=True)
         if hash_str in self.__cache__:
             return self.__cache__[hash_str]
 
         return None
 
-    def __hydrate_request__(self, requested_data: dict, checks: ValidationRuleChecks, event: dict, should_retry: bool):
+    def __hydrate_request__(
+        self,
+        requested_data: dict,
+        checks: ValidationRuleChecks,
+        event: dict,
+        should_retry: bool,
+    ):
         # verify request worked correctly and build response
         # gotta check if consumer request json or csv, so we can parse the output correctly
-        requested_data['success'] = checks.expect_successful_response().passed()  # successful csv response
-        if not requested_data['success']:
-            requested_data['Error Message'] = checks.get_error_message()
-        requested_data['limit_reached'] = checks.expect_limit_not_reached().passed()
-        requested_data['status_code'] = checks.get_status_code()
-
-        if checks.expect_json_datatype().expect_successful_response().passed():  # successful json response
+        requested_data[
+            "success"
+        ] = checks.expect_successful_response().passed()  # successful csv response
+        if not requested_data["success"]:
+            requested_data["Error Message"] = checks.get_error_message()
+        requested_data["limit_reached"] = checks.expect_limit_not_reached().passed()
+        requested_data["status_code"] = checks.get_status_code()
+
+        if (
+            checks.expect_json_datatype().expect_successful_response().passed()
+        ):  # successful json response
             json_response = checks.get_obj()
             for field in json_response:
                 requested_data[field] = json_response[field]
 
-        if checks.expect_csv_datatype().expect_successful_response().passed():  # successful csv response
-            requested_data['csv'] = checks.get_obj()
-
-    def __fetch_data__(self, checks: ValidationRuleChecks, event: dict, loggable_event: dict):
+        if (
+            checks.expect_csv_datatype().expect_successful_response().passed()
+        ):  # successful csv response
+            requested_data["csv"] = checks.get_obj()
+
+    def __fetch_data__(
+        self, checks: ValidationRuleChecks, event: dict, loggable_event: dict
+    ):
         url = self.__build_url_from_args__(event)
         r = requests.get(url)
         if self.__first_successful_attempt__ == 0:
             self.__first_successful_attempt__ = time.perf_counter()
         self.__total_calls__ += 1
         checks.with_response(r)
-        logging.info(json.dumps({"method": "get_data_from_alpha_vantage", "action": "response_from_alphavantage"
-                                    , "status_code": r.status_code, "data": r.text, "event": loggable_event}))
+        logging.info(
+            json.dumps(
+                {
+                    "method": "get_data_from_alpha_vantage",
+                    "action": "response_from_alphavantage",
+                    "status_code": r.status_code,
+                    "data": r.text,
+                    "event": loggable_event,
+                }
+            )
+        )
 
     def __validate_api_key__(self, checks: ValidationRuleChecks, event: dict):
         # get api key if not provided
         if checks.expect_api_key_in_event().failed():
             event["apikey"] = self.__api_key__  # assume they passed to builder method.
-        elif self.__api_key__ is None or len(self.__api_key__) == 0 or "apikey" not in event \
-                or not event.get("apikey"):  # consumer didn't tell me where to get api key
+        elif (
+            self.__api_key__ is None
+            or len(self.__api_key__) == 0
+            or "apikey" not in event
+            or not event.get("apikey")
+        ):  # consumer didn't tell me where to get api key
             raise ApiKeyNotFound(
-                "You must call client.with_api_key([api_key]), create config file in your profile (i.e. ~/.alphavantage) or event[api_key] = [your api key] before retrieving data from alphavantage")
+                "You must call client.with_api_key([api_key]), create config file in your profile (i.e. ~/.alphavantage) or event[api_key] = [your api key] before retrieving data from alphavantage"
+            )
 
     def __sleep__(self):
         then = self.__first_successful_attempt__
         now = time.perf_counter()
         diff = 60 - (now - then)
         logging.info(f"sleeping for {diff} seconds")
         if diff < 0:
             diff = 60
         time.sleep(diff)
 
     def clear_cache(self):
+        """Clear First in / First Out Cache
+
+        Returns:
+            Nothing
+
+        """
         self.__cache__.clear()
 
         return self
+
+    def search_ticker(self, event: dict) -> TickerSearch:
+        """The Search Endpoint returns the best-matching symbols and market information based on your keywords.
+
+        The search results also contain match scores that provide you with the full
+        flexibility to develop your own search and filtering logic.
+        Args:
+            event: dict
+
+        Returns:
+            TickerSearch
+
+        """
+        defaults = {"function": "SYMBOL_SEARCH", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return TickerSearch.model_validate(json_response)
+
+    def get_market_status(self) -> MarketStatus:
+        """Returns the current market status of major trading venues for equities, forex, and cryptocurrencies.
+
+        Returns:
+            The MarketStatus of your choice
+        """
+        json_request = {"function": "MARKET_STATUS"}
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return MarketStatus.model_validate(json_response)
+
+    def get_top_gainers_and_losers(self) -> MarketMovers:
+        """Returns the top 20 gainers, losers, and the most active traded tickers in the US market.
+
+        Returns:
+            The MarketMovers of your choice
+
+        """
+        json_request = {"function": "TOP_GAINERS_LOSERS"}
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return MarketMovers.model_validate(json_response)
+
+    def get_earnings_calendar(self, event: Union[str, dict]) -> EarningsCalendar:
+        """Returns a list of company earnings expected in the next 3, 6, or 12 months.
+
+        Returns:
+            The EarningsCalendar of your choice
+
+        """
+        defaults = {
+            "function": "EARNINGS_CALENDAR",
+            "horizon": "3month",
+            "datatype": "csv",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+        records = json_response["csv"].split("\n")
+        header = records.pop(0)
+        headers = header.split(",")
+        reader = csv.DictReader(records, delimiter=",")
+        reader.fieldnames = headers
+        items = list(reader)
+        json_response["data"] = items
+
+        return EarningsCalendar.model_validate(json_response)
+
+    def get_ipo_calendar(self) -> IpoCalendar:
+        """Returns a list of company earnings expected in the next 3, 6, or 12 months.
+
+        Returns:
+            The IpoCalendar of your choice
+
+        """
+        json_request = {"function": "IPO_CALENDAR", "datatype": "csv"}
+
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+        records = json_response["csv"].split("\n")
+        header = records.pop(0)
+        headers = header.split(",")
+        reader = csv.DictReader(records, delimiter=",")
+        reader.fieldnames = headers
+        items = list(reader)
+        json_response["data"] = items
+
+        return IpoCalendar.model_validate(json_response)
+
+    def get_news_and_sentiment(self, event: dict) -> NewsAndSentiment:
+        """Returns live and historical market news & sentiment data
+
+        This API returns live and historical market news & sentiment data derived from over 50 major financial news
+        outlets around the world, covering stocks, cryptocurrencies, forex, and a wide range of topics such as fiscal
+        policy, mergers & acquisitions, IPOs, etc.
+
+        Args:
+            event: dict
+
+        Returns:
+            The NewsAndSentiment of your choice
+
+        """
+        defaults = {"function": "NEWS_SENTIMENT", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return NewsAndSentiment.model_validate(json_response)
+
+    def get_forex_intraday(self, event: dict) -> CurrencyQuote:
+        """returns intraday time series (timestamp, open, high, low, close) of the FX currency pair specified.
+
+        Args:
+            event: dict containing your params to the api
+
+        Returns:
+            The CurrencyQuote of your choice
+
+        """
+        defaults = {
+            "function": "FX_INTRADAY",
+            "datatype": "json",
+            "interval": "60min",
+            "outputsize": "compact",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return CurrencyQuote.model_validate(json_response)
+
+    def get_forex_daily(self, event: dict) -> CurrencyQuote:
+        """returns the daily time series of the FX currency pair specified, updated realtime.
+
+        Included fields: (timestamp, open, high, low, close)
+
+        Args:
+            event: dict containing your params to the api
+
+        Returns:
+            The CurrencyQuote of your choice
+
+        """
+
+        defaults = {
+            "function": "FX_DAILY",
+            "datatype": "json",
+            "interval": "60min",
+            "outputsize": "compact",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return CurrencyQuote.model_validate(json_response)
+
+    def get_forex_weekly(self, event: dict) -> CurrencyQuote:
+        """returns the weekly time series of the FX currency pair specified
+
+        Included fields: (timestamp, open, high, low, close) updated in realtime.  The latest data point is the price
+        information for the week (or partial week) containing the current trading day, updated realtime.
+
+        Args:
+            event: dict containing your params to the api
+
+        Returns:
+            The CurrencyQuote of your choice
+        """
+        defaults = {
+            "function": "FX_WEEKLY",
+            "datatype": "json",
+            "interval": "60min",
+            "outputsize": "compact",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return CurrencyQuote.model_validate(json_response)
+
+    def get_forex_monthly(self, event: dict) -> CurrencyQuote:
+        """returns the monthly time series of the FX currency pair specified
+
+        Included fields: (timestamp, open, high, low, close) updated in realtime.  The latest data point is the prices
+        information for the month (or partial month containing the current trading day, updated realtime.
+
+        Args:
+            event: dict containing your params to the api
+
+        Returns:
+            The CurrencyQuote of your choice
+
+        """
+        defaults = {
+            "function": "FX_MONTHLY",
+            "datatype": "json",
+            "interval": "60min",
+            "outputsize": "compact",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return CurrencyQuote.model_validate(json_response)
+
+    def get_crude_oil_wti_prices(self, event: dict) -> Commodity:
+        """returns the West Texas Intermediate (WTI) crude oil prices in daily, weekly, and monthly horizons.
+
+        Source: U.S. Energy Information Administration, Crude Oil Prices: West Texas Intermediate (WTI) - Cushing,
+        Oklahoma, retrieved from FRED, Federal Reserve Bank of St. Louis. This data feed uses the FRED® API but is not
+        endorsed or certified by the Federal Reserve Bank of St. Louis. By using this data feed, you agree to be
+        bound by the FRED® API Terms of Use.
+
+        Args:
+            event: dict containing your params to the api
+
+        Returns:
+            The Commodity of your choice
+
+        """
+        defaults = {"function": "WTI", "interval": "monthly", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Commodity.model_validate(json_response)
+
+    def get_crude_oil_brent_prices(self, event: dict) -> Commodity:
+        """returns the Brent (Europe) crude oil prices in daily, weekly, and monthly horizons.
+
+        Source: U.S. Energy Information Administration, Crude Oil Prices: Brent - Europe, retrieved from FRED,
+        Federal Reserve Bank of St. Louis. This data feed uses the FRED® API but is not endorsed or certified by the
+        Federal Reserve Bank of St. Louis. By using this data feed, you agree to be bound by the FRED® API Terms of Use.
+
+        Args:
+            event: dict containing your params to the api
+
+        Returns:
+            The Commodity of your choice
+
+        """
+        defaults = {"function": "BRENT", "interval": "monthly", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Commodity.model_validate(json_response)
+
+    def get_natural_gas_prices(self, event: dict) -> Commodity:
+        """returns the Henry Hub natural gas spot prices in daily, weekly, and monthly horizons.
+
+        Source: U.S. Energy Information Administration, Henry Hub Natural Gas Spot Price, retrieved from FRED,
+        Federal Reserve Bank of St. Louis. This data feed uses the FRED® API but is not endorsed or certified by the
+        Federal Reserve Bank of St. Louis. By using this data feed, you agree to be bound by the FRED® API Terms of Use.
+
+        Args:
+            event: dict containing your params to the api
+
+        Returns:
+            The Commodity of your choice
+
+        """
+        defaults = {
+            "function": "NATURAL_GAS",
+            "interval": "monthly",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Commodity.model_validate(json_response)
+
+    def get_copper_prices(self, event: dict) -> Commodity:
+        """returns the global price of copper in monthly, quarterly, and annual horizons.
+
+        Source: International Monetary Fund (IMF Terms of Use), Global price of Copper, retrieved from FRED, Federal
+        Reserve Bank of St. Louis. This data feed uses the FRED® API but is not endorsed or certified by the Federal
+        Reserve Bank of St. Louis. By using this data feed, you agree to be bound by the FRED® API Terms of Use.
+
+        Args:
+            event: dict containing your params to the api
+
+        Returns:
+            The Commodity of your choice
+        """
+        defaults = {"function": "COPPER", "interval": "monthly", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Commodity.model_validate(json_response)
+
+    def get_aluminum_prices(self, event: dict) -> Commodity:
+        """returns the global price of aluminum in monthly, quarterly, and annual horizons.
+
+        Source: International Monetary Fund (IMF Terms of Use), Global price of Aluminum, retrieved from FRED, Federal
+        Reserve Bank of St. Louis. This data feed uses the FRED® API but is not endorsed or certified by the Federal
+        Reserve Bank of St. Louis. By using this data feed, you agree to be bound by the FRED® API Terms of Use.
+
+        Args:
+            event: dict containing your params to the api
+
+        Returns:
+            The Commodity of your choice
+
+        """
+        defaults = {"function": "ALUMINUM", "interval": "monthly", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Commodity.model_validate(json_response)
+
+    def get_wheat_prices(self, event: dict) -> Commodity:
+        """returns the global price of wheat in monthly, quarterly, and annual horizons.
+
+        Source: International Monetary Fund (IMF Terms of Use), Global price of Wheat, retrieved from FRED, Federal
+        Reserve Bank of St. Louis. This data feed uses the FRED® API but is not endorsed or certified by the Federal
+        Reserve Bank of St. Louis. By using this data feed, you agree to be bound by the FRED® API Terms of Use.
+
+        Args:
+            event: dict containing your params to the api
+
+        Returns:
+            The Commodity of your choice
+
+        """
+        defaults = {"function": "WHEAT", "interval": "monthly", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Commodity.model_validate(json_response)
+
+    def get_corn_prices(self, event: dict) -> Commodity:
+        """returns the global price of corn in monthly, quarterly, and annual horizons.
+
+        Source: International Monetary Fund (IMF Terms of Use), Global price of Corn, retrieved from FRED, Federal
+        Reserve Bank of St. Louis. This data feed uses the FRED® API but is not endorsed or certified by the Federal
+        Reserve Bank of St. Louis. By using this data feed, you agree to be bound by the FRED® API Terms of Use.
+
+        Args:
+            event: dict containing your params to the api
+
+        Returns:
+            The Commodity of your choice
+        """
+        defaults = {"function": "CORN", "interval": "monthly", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Commodity.model_validate(json_response)
+
+    def get_cotton_prices(self, event: dict) -> Commodity:
+        """returns the global price of cotton in monthly, quarterly, and annual horizons.
+
+        Source: International Monetary Fund (IMF Terms of Use), Global price of Cotton, retrieved from FRED, Federal
+        Reserve Bank of St. Louis. This data feed uses the FRED® API but is not endorsed or certified by the Federal
+        Reserve Bank of St. Louis. By using this data feed, you agree to be bound by the FRED® API Terms of Use.
+
+        Args:
+            event: dict containing your params to the api
+
+        Returns:
+            The Commodity of your choice
+
+        """
+        defaults = {"function": "COTTON", "interval": "monthly", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Commodity.model_validate(json_response)
+
+    def get_sugar_prices(self, event: dict) -> Commodity:
+        """returns the global price of sugar in monthly, quarterly, and annual horizons.
+
+        Source: International Monetary Fund (IMF Terms of Use), Global price of Sugar, No. 11, World, retrieved from
+        FRED, Federal Reserve Bank of St. Louis. This data feed uses the FRED® API but is not endorsed or certified by
+        the Federal Reserve Bank of St. Louis. By using this data feed, you agree to be bound
+        by the FRED® API Terms of Use.
+
+        Args:
+            event: dict containing your params to the api
+
+        Returns:
+            The Commodity of your choice
+
+        """
+        defaults = {"function": "SUGAR", "interval": "monthly", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Commodity.model_validate(json_response)
+
+    def get_coffee_prices(self, event: dict) -> Commodity:
+        """returns the global price of coffee in monthly, quarterly, and annual horizons.
+
+        Source: International Monetary Fund (IMF Terms of Use), Global price of Coffee, Other Mild Arabica,
+        retrieved from FRED, Federal Reserve Bank of St. Louis. This data feed uses the FRED® API but is not
+        endorsed or certified by the Federal Reserve Bank of St. Louis. By using this data feed, you agree to be
+        bound by the FRED® API Terms of Use.
+
+        Args:
+            event: dict containing your params to the api
+
+        Returns:
+            The Commodity of your choice
+
+        """
+        defaults = {"function": "COFFEE", "interval": "monthly", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Commodity.model_validate(json_response)
+
+    def get_all_commodity_prices(self, event: dict) -> Commodity:
+        """returns the global price index of all commodities in monthly, quarterly, and annual temporal dimensions.
+
+        Source: International Monetary Fund (IMF Terms of Use), Global Price Index of All Commodities, retrieved
+        from FRED, Federal Reserve Bank of St. Louis. This data feed uses the FRED® API but is not endorsed or
+        certified by the Federal Reserve Bank of St. Louis. By using this data feed, you agree to be bound by
+        the FRED® API Terms of Use.
+
+        Args:
+            event: dict containing your params to the api
+
+        Returns:
+            The Commodity of your choice
+
+        """
+        defaults = {
+            "function": "ALL_COMMODITIES",
+            "interval": "monthly",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Commodity.model_validate(json_response)
+
+    def get_sma(self, event: Union[str, dict]) -> Quote:
+        """Returns the simple moving average (SMA) values.
+
+        See also:   http://www.investopedia.com/articles/technical/052201.asp
+                    http://www.fmlabs.com/reference/default.htm?url=SimpleMA.htm
+        Args:
+            event:  A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns:
+            The Quote of your choice
+
+        """
+        defaults = {
+            "function": "SMA",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_ema(self, event: Union[str, dict]) -> Quote:
+        """returns the exponential moving average (EMA) values.
+
+        See also: http://www.fmlabs.com/reference/default.htm?url=ExpMA.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns:
+            The Quote of your choice
+
+        """
+        defaults = {
+            "function": "EMA",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_wma(self, event: Union[str, dict]) -> Quote:
+        """returns the exponential moving average (EMA) values.
+
+        See also: http://www.fmlabs.com/reference/default.htm?url=ExpMA.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns:
+            The Quote of your choice
+
+        """
+        defaults = {
+            "function": "WMA",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_dema(self, event: Union[str, dict]) -> Quote:
+        """returns the double exponential moving average (DEMA) values.
+
+        See also: http://www.investopedia.com/articles/trading/10/double-exponential-moving-average.asp
+                : http://www.fmlabs.com/reference/default.htm?url=DEMA.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns:
+            The Quote of your choice
+
+        """
+        defaults = {
+            "function": "DEMA",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_tema(self, event: Union[str, dict]) -> Quote:
+        """returns the triple exponential moving average (TEMA) values.
+
+        See also: http://www.fmlabs.com/reference/default.htm?url=TEMA.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns:
+            The Quote of your choice
+
+        """
+        defaults = {
+            "function": "TEMA",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_trima(self, event: Union[str, dict]) -> Quote:
+        """returns the triple exponential moving average (TEMA) values.
+
+        See also: http://www.fmlabs.com/reference/default.htm?url=TEMA.htm
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns:
+            The Quote of your choice
+
+        """
+        defaults = {
+            "function": "TRIMA",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_kama(self, event: Union[str, dict]) -> Quote:
+        """returns the Kaufman adaptive moving average (KAMA) values.
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns:
+            The Quote of your choice
+
+        """
+        defaults = {
+            "function": "KAMA",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_mama(self, event: Union[str, dict]) -> Quote:
+        """returns the MESA adaptive moving average (MAMA) values.
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns:
+            The Quote of your choice
+
+        """
+        defaults = {
+            "function": "MAMA",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_vwap(self, event: Union[str, dict]) -> Quote:
+        """returns the volume weighted average price (VWAP) for intraday time series.
+
+        See also: https://www.investopedia.com/terms/v/vwap.asp
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns:
+            The Quote of your choice
+
+        """
+        defaults = {"function": "VWAP", "interval": "60min", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_t3(self, event: Union[str, dict]) -> Quote:
+        """returns the triple exponential moving average (T3) values.
+
+        See also: http://www.fmlabs.com/reference/default.htm?url=T3.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns:
+            The Quote of your choice
+
+        """
+        defaults = {
+            "function": "T3",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_macd(self, event: Union[str, dict]) -> Quote:
+        """returns the moving average convergence / divergence (MACD) values.
+
+        See also: http://www.investopedia.com/articles/forex/05/macddiverge.asp
+                : http://www.fmlabs.com/reference/default.htm?url=MACD.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns:
+            The Quote of your choice
+
+        """
+        defaults = {
+            "function": "MACD",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_macdext(self, event: Union[str, dict]) -> Quote:
+        """returns the moving average convergence / divergence values with controllable moving average type.
+
+        See also: http://www.investopedia.com/articles/forex/05/macddiverge.asp
+                : http://www.fmlabs.com/reference/default.htm?url=MACD.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns:
+            The Quote of your choice
+
+        """
+        defaults = {
+            "function": "MACDEXT",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_stoch(self, event: Union[str, dict]) -> Quote:
+        """returns the stochastic oscillator (STOCH) values.
+
+        See also: https://www.investopedia.com/terms/s/stochasticoscillator.asp
+                : http://www.fmlabs.com/reference/default.htm?url=StochasticOscillator.htm
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns:
+            The Quote of your choice
+
+        """
+        defaults = {
+            "function": "STOCH",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_stockhf(self, event: Union[str, dict]) -> Quote:
+        """returns the stochastic fast (STOCHF) values.
+
+        See also: http://www.investopedia.com/university/indicator_oscillator/ind_osc8.asp
+                : http://www.fmlabs.com/reference/default.htm?url=StochasticOscillator.htm
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {"function": "STOCHF", "interval": "daily", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_rsi(self, event: Union[str, dict]) -> Quote:
+        """returns the relative strength index (RSI) values.
+
+        See also: http://www.investopedia.com/articles/technical/071601.asp
+                : http://www.fmlabs.com/reference/default.htm?url=RSI.htm
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "RSI",
+            "interval": "daily",
+            "time_period": "60",
+            "series_type": "close",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_stochrsi(self, event: Union[str, dict]) -> Quote:
+        """returns the stochastic relative strength index (STOCHRSI) values.
+
+        See also: http://www.fmlabs.com/reference/default.htm?url=StochRSI.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+        """
+        defaults = {
+            "function": "STOCHRSI",
+            "interval": "daily",
+            "time_period": "60",
+            "series_type": "close",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_willr(self, event: Union[str, dict]) -> Quote:
+        """returns the Williams' %R (WILLR) values.
+
+        See also: http://www.fmlabs.com/reference/default.htm?url=WilliamsR.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "WILLR",
+            "interval": "daily",
+            "time_period": "60",
+            "series_type": "close",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_adx(self, event: Union[str, dict]) -> Quote:
+        """ returns the average directional movement index (ADX) values.
+        
+        See also: http://www.investopedia.com/articles/trading/07/adx-trend-indicator.asp
+                : http://www.fmlabs.com/reference/default.htm?url=ADX.htm
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "ADX",
+            "interval": "daily",
+            "time_period": "60",
+            "series_type": "close",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_adxr(self, event: Union[str, dict]) -> Quote:
+        """ returns the average directional movement index rating (ADXR) values.
+        This API 
+        See also: http://www.fmlabs.com/reference/default.htm?url=ADXR.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "ADXR",
+            "interval": "daily",
+            "time_period": "60",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_apo(self, event: Union[str, dict]) -> Quote:
+        """ returns the absolute price oscillator (APO) values.
+        
+        See also: http://www.fmlabs.com/reference/default.htm?url=PriceOscillator.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "APO",
+            "interval": "daily",
+            "time_period": "60",
+            "series_type": "close",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_ppo(self, event: Union[str, dict]) -> Quote:
+        """ returns the percentage price oscillator (PPO) values.
+        
+        See also: http://www.investopedia.com/articles/investing/051214/use-percentage-price-oscillator-elegant-indicator-picking-stocks.asp
+                : http://www.fmlabs.com/reference/default.htm?url=PriceOscillatorPct.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "PPO",
+            "interval": "daily",
+            "series_type": "close",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_mom(self, event: Union[str, dict]) -> Quote:
+        """returns the momentum (MOM) values.
+        
+        See also: http://www.investopedia.com/articles/technical/03/070203.asp
+                : http://www.fmlabs.com/reference/default.htm?url=Momentum.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "MOM",
+            "interval": "daily",
+            "series_type": "close",
+            "time_period": "60",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_bop(self, event: Union[str, dict]) -> Quote:
+        """returns the balance of power (BOP) values.
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {"function": "BOP", "interval": "daily", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_cci(self, event: Union[str, dict]) -> Quote:
+        """returns the commodity channel index (CCI) values.
+        
+        See also: http://www.investopedia.com/articles/trading/05/041805.asp
+                : http://www.fmlabs.com/reference/default.htm?url=CCI.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "CCI",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_cmo(self, event: Union[str, dict]) -> Quote:
+        """returns the Chande momentum oscillator (CMO) values.
+        
+        See also: http://www.fmlabs.com/reference/default.htm?url=CMO.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "CMO",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_roc(self, event: Union[str, dict]) -> Quote:
+        """returns the rate of change (ROC) values.
+        
+        See also: http://www.investopedia.com/articles/technical/092401.asp
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "ROC",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_rocr(self, event: Union[str, dict]) -> Quote:
+        """returns the rate of change ratio (ROCR) values.
+        
+        See also: http://www.investopedia.com/articles/technical/092401.asp
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "ROCR",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_aroon(self, event: Union[str, dict]) -> Quote:
+        """returns the Aroon (AROON) values.
+        
+        See also: http://www.investopedia.com/articles/trading/06/aroon.asp
+                : http://www.fmlabs.com/reference/default.htm?url=Aroon.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "AROON",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_aroonosc(self, event: Union[str, dict]) -> Quote:
+        """returns the Aroon oscillator (AROONOSC) values.
+        
+        See also: http://www.fmlabs.com/reference/default.htm?url=AroonOscillator.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "AROONOSC",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_mfi(self, event: Union[str, dict]) -> Quote:
+        """returns the money flow index (MFI) values.
+        
+        See also: http://www.investopedia.com/articles/technical/03/072303.asp
+                : http://www.fmlabs.com/reference/default.htm?url=MoneyFlowIndex.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "MFI",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_trix(self, event: Union[str, dict]) -> Quote:
+        """returns the 1-day rate of change of a triple smooth exponential moving average (TRIX) values.
+        
+        See also: http://www.investopedia.com/articles/technical/02/092402.asp
+                : http://www.fmlabs.com/reference/default.htm?url=TRIX.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "TRIX",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_ultosc(self, event: Union[str, dict]) -> Quote:
+        """returns the ultimate oscillator (ULTOSC) values.
+        
+        See also: http://www.fmlabs.com/reference/default.htm?url=UltimateOsc.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {"function": "ULTOSC", "interval": "daily", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_dx(self, event: Union[str, dict]) -> Quote:
+        """returns the directional movement index (DX) values.
+        
+        See also: http://www.investopedia.com/articles/technical/02/050602.asp
+                : http://www.fmlabs.com/reference/default.htm?url=DX.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "DX",
+            "interval": "daily",
+            "time_period": "60",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_minus_di(self, event: Union[str, dict]) -> Quote:
+        """returns the minus directional indicator (MINUS_DI) values.
+        
+        See also: http://www.investopedia.com/articles/technical/02/050602.asp
+                : http://www.fmlabs.com/reference/default.htm?url=DI.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "MINUS_DI",
+            "interval": "daily",
+            "time_period": "60",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_plus_di(self, event: Union[str, dict]) -> Quote:
+        """returns the plus directional indicator (PLUS_DI) values.
+        
+        See also: http://www.investopedia.com/articles/technical/02/050602.asp
+                : http://www.fmlabs.com/reference/default.htm?url=DI.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "PLUS_DI",
+            "interval": "daily",
+            "time_period": "60",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_minus_dm(self, event: Union[str, dict]) -> Quote:
+        """returns the minus directional movement (MINUS_DM) values.
+        
+        See also: http://www.investopedia.com/articles/technical/02/050602.asp
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "MINUS_DM",
+            "interval": "daily",
+            "time_period": "60",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_plus_dm(self, event: Union[str, dict]) -> Quote:
+        """returns the plus directional movement (PLUS_DM) values.
+    
+        See also: http://www.investopedia.com/articles/technical/02/050602.asp
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "PLUS_DM",
+            "interval": "daily",
+            "time_period": "60",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_bbands(self, event: Union[str, dict]) -> Quote:
+        """returns the Bollinger bands (BBANDS) values.
+        
+        See also: http://www.investopedia.com/articles/technical/04/030304.asp
+                : http://www.fmlabs.com/reference/default.htm?url=Bollinger.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "BBANDS",
+            "interval": "daily",
+            "time_period": "60",
+            "series_type": "close",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_midpoint(self, event: Union[str, dict]) -> Quote:
+        """returns the midpoint (MIDPOINT) values. MIDPOINT = (highest value + lowest value)/2.
+        
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "MIDPOINT",
+            "interval": "daily",
+            "time_period": "60",
+            "series_type": "close",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_midprice(self, event: Union[str, dict]) -> Quote:
+        """returns the midpoint price (MIDPRICE) values. MIDPRICE = (highest high + lowest low)/2.
+        
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "MIDPRICE",
+            "interval": "daily",
+            "time_period": "60",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_sar(self, event: Union[str, dict]) -> Quote:
+        """returns the parabolic SAR (SAR) values. See also: Investopedia article and mathematical reference.
+        
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {"function": "SAR", "interval": "daily", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_trange(self, event: Union[str, dict]) -> Quote:
+        """returns the true range (TRANGE) values.
+        
+        See also: http://www.fmlabs.com/reference/default.htm?url=TR.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {"function": "TRANGE", "interval": "daily", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_atr(self, event: Union[str, dict]) -> Quote:
+        """returns the average true range (ATR) values.
+        
+        See also: http://www.investopedia.com/articles/trading/08/average-true-range.asp
+                : http://www.fmlabs.com/reference/default.htm?url=ATR.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "ATR",
+            "interval": "daily",
+            "datatype": "json",
+            "time_period": "60",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_natr(self, event: Union[str, dict]) -> Quote:
+        """returns the normalized average true range (NATR) values.
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "NATR",
+            "interval": "daily",
+            "time_period": "60",
+            "datatype": "json",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_ad(self, event: Union[str, dict]) -> Quote:
+        """returns the Chaikin A/D line (AD) values.
+        
+        See also: http://www.investopedia.com/articles/active-trading/031914/understanding-chaikin-oscillator.asp
+                : http://www.fmlabs.com/reference/default.htm?url=AccumDist.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {"function": "AD", "interval": "daily", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_adosc(self, event: Union[str, dict]) -> Quote:
+        """returns the Chaikin A/D oscillator (ADOSC) values.
+        
+        See also: http://www.investopedia.com/articles/active-trading/031914/understanding-chaikin-oscillator.asp
+                : http://www.fmlabs.com/reference/default.htm?url=AccumDist.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {"function": "ADOSC", "interval": "daily", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_obv(self, event: Union[str, dict]) -> Quote:
+        """returns the on balance volume (OBV) values.
+        
+        See also: http://www.investopedia.com/articles/technical/100801.asp
+                : http://www.fmlabs.com/reference/default.htm?url=OBV.htm
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {"function": "OBV", "interval": "daily", "datatype": "json"}
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_ht_trendline(self, event: Union[str, dict]) -> Quote:
+        """returns the Hilbert transform, instantaneous trendline (HT_TRENDLINE) values.
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "HT_TRENDLINE",
+            "interval": "daily",
+            "datatype": "json",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_ht_sine(self, event: Union[str, dict]) -> Quote:
+        """returns the Hilbert transform, sine wave (HT_SINE) values.
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "HT_SINE",
+            "interval": "daily",
+            "datatype": "json",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_ht_trendmode(self, event: Union[str, dict]) -> Quote:
+        """returns the Hilbert transform, trend vs cycle mode (HT_TRENDMODE) values.
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "HT_TRENDMODE",
+            "interval": "daily",
+            "datatype": "json",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_ht_dcperiod(self, event: Union[str, dict]) -> Quote:
+        """returns the Hilbert transform, dominant cycle period (HT_DCPERIOD) values.
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "HT_DCPERIOD",
+            "interval": "daily",
+            "datatype": "json",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_ht_dcphase(self, event: Union[str, dict]) -> Quote:
+        """returns the Hilbert transform, dominant cycle period (HT_DCPERIOD) values.
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "HT_DCPHASE",
+            "interval": "daily",
+            "datatype": "json",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
+
+    def get_ht_phasor(self, event: Union[str, dict]) -> Quote:
+        """returns the Hilbert transform, phasor components (HT_PHASOR) values.
+
+        Args:
+            event: A ticker symbol str OR dict of parameters to be sent to the API
+
+        Returns: Quote
+
+        """
+        defaults = {
+            "function": "HT_PHASOR",
+            "interval": "daily",
+            "datatype": "json",
+            "series_type": "close",
+        }
+        json_request = self.__create_api_request_from__(defaults, event)
+        json_response = self.get_data_from_alpha_vantage(json_request, self.__retry__)
+
+        return Quote.model_validate(json_response)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## alphavantage_api_client/models.py

```diff
@@ -1,9 +1,9 @@
 import pydantic
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, ValidationError, model_validator
 from typing import Optional
 import copy
 
 
 class CsvNotSupported(Exception):
     def __init__(self, function: str, event: dict):
         self.message = f"CSV Datatype is not supported by this function {function}"
@@ -12,32 +12,101 @@
 
 
 class BaseResponse(BaseModel):
     success: bool
     limit_reached: bool
     status_code: int
     error_message: Optional[str] = Field(None, alias='Error Message')
-    csv: Optional[str]
+    csv: Optional[str] = None
 
 
 class BaseQuote(BaseResponse):
     symbol: str
 
 
+class TickerSearch(BaseResponse):
+    data: list[dict] = Field({}, alias='bestMatches')
+
+class MarketStatus(BaseResponse):
+    endpoint: str
+    data: list[dict] = Field({}, alias='markets')
+
+class NewsAndSentiment(BaseResponse):
+    items: int
+    sentiment_score_definition: str
+    relevance_score_definition: str
+    data: list[dict] = Field({}, alias='feed')
+
+class MarketMovers(BaseResponse):
+    top_gainers: list[dict]
+    top_losers: list[dict]
+    last_updated: str
+    meta_data: Optional[str] = Field(str, alias='metadata')
+    most_actively_traded: list[dict]
+
+class EarningsCalendarItem(BaseModel):
+    symbol: str
+    name: str
+    report_date: str = Field(str,alias='reportDate')
+    fiscal_date_ending: str = Field(str,alias='fiscalDateEnding')
+    estimate: Optional[float] = None
+    currency: Optional[str] = None
+
+class IpoCalendarItem(BaseModel):
+    symbol: str
+    name: str
+    ipo_date: str = Field(str,alias="ipoDate")
+    price_range_low: Optional[float] = Field(float, alias="priceRangeLow")
+    price_range_high: Optional[float] = Field(float, alias="priceRangeHigh")
+    currency: Optional[str] = None
+    exchange: Optional[str] = None
+
+class IpoCalendar(BaseResponse):
+    data: Optional[list[IpoCalendarItem]] = Field([])
+
+class EarningsCalendar(BaseResponse):
+    symbol: str
+    data: Optional[list[EarningsCalendarItem]] = Field([])
+
+class CurrencyQuote(BaseResponse):
+    data: Optional[dict] = Field({})
+    meta_data: Optional[dict] = Field({}, alias='Meta Data')
+
+    @model_validator(mode="before")
+    def normalize_fields(cls, values):
+        return {
+            "data" if k.startswith("Time Series FX (")
+                      or k.startswith("Crypto Intraday (")
+                      or k.startswith("Time Series Crypto (")
+                      or k.startswith("Time Series (Digital Currency")
+                      or k.startswith("Realtime Currency Exchange Rate") else k: v for k, v in values.items()
+        }
+
+class Commodity(BaseResponse):
+    name: str
+    interval: str
+    unit: str
+    data: list[dict]
+
 class Quote(BaseQuote):
     """
     data is this clients abstraction of the response from alpha vantage. Time Series, Technical Indicator
     """
     data: Optional[dict] = {}
     meta_data: Optional[dict] = Field({}, alias='Meta Data')
 
-    @pydantic.root_validator(pre=True)
+    @model_validator(mode="before")
     def normalize_fields(cls, values):
         return {
-            "data" if k.startswith("Technical Analysis: ") or k.startswith("Time Series (")
+            "data" if k.startswith("Weekly Adjusted Time Series")
+                      or k.startswith("Monthly Adjusted Time Series")
+                      or k.startswith("Monthly Time Series")
+                      or k.startswith("Weekly Time Series")
+                      or k.startswith("Technical Analysis: ")
+                      or k.startswith("Time Series (")
                       or k.startswith("Time Series Crypto (") else k: v for k, v in values.items()
         }
 
     def get_most_recent_value(self) -> Optional[dict]:
         if len(self.data) > 0:
             for quote_date in self.data:
                 quotes = self.data[quote_date]
@@ -45,15 +114,15 @@
                 return quotes
 
         return None
 
     def get_oldest_value(self) -> Optional[dict]:
         if len(self.data) > 0:
             quote_dates = list(self.data.keys())
-            last_quote_date = quote_dates[len(quote_dates)-1]
+            last_quote_date = quote_dates[len(quote_dates) - 1]
             quote = self.data[last_quote_date]
             quote["query_date"] = last_quote_date
 
             return quote
 
         return None
 
@@ -103,15 +172,15 @@
         return self.get_data_value(field)
 
 
 class AccountingReport(BaseQuote):
     annualReports: list = Field(default=[], alias="annualReports")
     quarterlyReports: list = Field(default=[], alias="quarterlyReports")
 
-    @pydantic.root_validator(pre=True)
+    @model_validator(mode="before")
     def normalize_fields(cls, values):
         annual_report_fields = ["annualEarnings"]
         quarterly_report_fields = ["quarterlyEarnings"]
         new_values = copy.deepcopy(values)
         for field in new_values:
             new_field = field
             if field in annual_report_fields:
@@ -134,19 +203,19 @@
         if len(self.quarterlyReports) > 0:
             for index, quarterly_report in enumerate(self.quarterlyReports):
                 return quarterly_report
 
         return None
 
 
-class RealGDP(BaseResponse):
-    name: Optional[str]
-    interval: Optional[str]
-    unit: Optional[str]
-    data: Optional[list]
+class EconomicIndicator(BaseResponse):
+    name: Optional[str] = None
+    interval: Optional[str] = None
+    unit: Optional[str] = None
+    data: Optional[list] = None
 
 
 class CompanyOverview(BaseQuote):
     symbol: str = Field(default=None, alias='Symbol')
     asset_type: str = Field(default=None, alias='AssetType')
     name: str = Field(default=None, alias='Name')
     description: str = Field(default=None, alias='Description')
```

## examples/getting_started.py

```diff
@@ -1,17 +1,17 @@
 from alphavantage_api_client import AlphavantageClient, GlobalQuote, Quote, AccountingReport, CompanyOverview, Ticker
-
+import logging
 
 def sample_global_quote():
     client = AlphavantageClient()
 
     global_quote = client.get_global_quote("TSLA")
     if not global_quote.success:
         raise ValueError(f"{global_quote.error_message}")
-    print(global_quote.json())  # convenience method that will convert to json
+    print(global_quote.model_dump_json())  # convenience method that will convert to json
     print(f"stock price: ${global_quote.get_price()}")  # convenience method to get stock price
     print(f"trade volume: {global_quote.get_volume()}")  # convenience method to get volume
     print(f"low price: ${global_quote.get_low_price()}")  # convenience method to get low price for the day
 
 
 def sample_balance_sheet():
     client = AlphavantageClient()
@@ -54,27 +54,27 @@
     income_statement = client.get_income_statement("TSLA")
     reports = [earnings, cash_flow, balance_sheet, income_statement]
 
     # show that each report is in the same type and how to access the annual and quarterly reports
     for accounting_report in reports:
         if not accounting_report.success:
             raise ValueError(f"{accounting_report.error_message}")
-        print(accounting_report.json())
+        print(accounting_report.model_dump_json())
         print(accounting_report.quarterlyReports)  # array of  all quarterly report
         print(accounting_report.annualReports)  # array of all annual reports
         print(accounting_report.get_most_recent_annual_report())  # get the most recent annual report
         print(accounting_report.get_most_recent_quarterly_report())  # get the most recent quarterly report;
 
 
 def sample_intraday_quote():
     client = AlphavantageClient()
     quote = client.get_intraday_quote("TSLA")
     if not quote.success:
         raise ValueError(f"{quote.error_message}")
-    print(quote.json())
+    print(quote.model_dump_json())
     print(f"success: {quote.success}")  # injected by this library to show success
     print(quote.data)  # all data from alpha vantage
     print(quote.get_most_recent_value())  # most recent quote
     print(quote.get_oldest_value())  # get the oldest quote
 
 
 def sample_company_overview():
@@ -100,16 +100,17 @@
     print(cash_flow.get_most_recent_quarterly_report())  # get the newest quarterly statement
     print(cash_flow.get_most_recent_annual_report())  # get the most recent annual report
     print(cash_flow.quarterlyReports)  # get [] quarterly reports
     print(cash_flow.annualReports)  # get [] annual reports
 
 
 def sample_retry_when_limit_reached():
+    logging.basicConfig(level=logging.INFO)
     client = AlphavantageClient().use_simple_cache().should_retry_once()
-    symbols = ["TSLA", "F", "C", "WFC", "ZIM", "PXD", "PXD", "POOL", "INTC", "INTU"]  # more than 5 calls so should fail
+    symbols = ["TSLA", "F", "C", "WFC", "ZIM", "PXD", "PXD", "POOL", "INTC", "INTU", "AAPL"]  # more than 5 calls so should fail
     for symbol in symbols:
         event = {
             "symbol": symbol
         }
         global_quote = client.get_global_quote(event)
         if not global_quote.success:
             raise ValueError(f"{global_quote.error_message}")
@@ -146,10 +147,20 @@
     # get the combined financial statements and iterate easy
     correlated_financial_statements = aapl.get_correlated_reports() # both quarterly and annually
 
     for fiscal_date_ending in correlated_financial_statements:
         combined_financial_statements = correlated_financial_statements[fiscal_date_ending]
         print(f"{fiscal_date_ending} = {combined_financial_statements}")
 
+def sample_direct_access():
+    client = AlphavantageClient()
+    event = {
+        "symbol" : "AAPL",
+        "function" : "GLOBAL_QUOTE"
+    } # EACH ATTRIBUTE IS EXACTLY SUPPORTED BY END POINTS
+
+    response = client.get_data_from_alpha_vantage(event)
+    print(response) # a dictionary with exact response from Alpha Vantage End point you requested
+
 
 if __name__ == "__main__":
-    sample_ticker_usage()
+    sample_direct_access()
```

## tests/__init__.py

```diff
@@ -0,0 +1,10 @@
+00000000: 6672 6f6d 202e 7465 7374 5f62 6173 6520  from .test_base 
+00000010: 696d 706f 7274 2042 6173 6554 6573 7453  import BaseTestS
+00000020: 7569 7465 0a66 726f 6d20 2e74 6573 745f  uite.from .test_
+00000030: 616c 6c5f 6672 6565 5f65 6e64 706f 696e  all_free_endpoin
+00000040: 7473 2069 6d70 6f72 7420 416c 6c45 6e64  ts import AllEnd
+00000050: 506f 696e 7454 6573 7473 0a66 726f 6d20  PointTests.from 
+00000060: 2e74 6573 745f 616c 6c5f 7061 6964 5f65  .test_all_paid_e
+00000070: 6e64 706f 696e 7473 2069 6d70 6f72 7420  ndpoints import 
+00000080: 416c 6c50 6169 6445 6e64 506f 696e 7454  AllPaidEndPointT
+00000090: 6573 7473 0a                             ests.
```

## tests/mock_client.py

```diff
@@ -1,74 +1,72 @@
-import logging
+import time
 
-from alphavantage_api_client import AlphavantageClient
-import json
+import requests
 import os
-from os.path import exists
+import configparser
+from alphavantage_api_client import ValidationRuleChecks, AlphavantageClient
+import json
+import copy
+import logging
 
 
 class MockAlphavantageClient(AlphavantageClient):
 
     def __init__(self):
         super().__init__()
         path = os.getcwd()
         logging.info(f"current path = {path}")
         self.base_path = f"{path}/tests/mocks"
-        if not exists(self.base_path):
+        if not os.path.exists(self.base_path):
             logging.info(f"I must be running from pycharm as a test since cwd is {self.base_path}, need to fix")
             path = os.path.dirname(os.getcwd())
             os.chdir(path) # go up a directory
             path = os.getcwd()
             self.base_path = f"{path}/tests/mocks"
 
         logging.info(f"self.base_path = {self.base_path}")
+        self.load_cache_from_disk()
 
-    def get_data_from_alpha_vantage(self, event, context=None):
-        '''
-        Get all data from alpha vantage
-        :param event:
-        :param context:
-        :return:
-        :rtype: dict
-        '''
-        if event is None:
-            raise ValueError("Event property isn't define")
-
-        text_file = None
-        if event.get("function") == "GLOBAL_QUOTE":
-            text_file = open(f"{self.base_path}/mock_stock_quote.json", "r")
-        elif event.get("function") == "BALANCE_SHEET":
-            text_file = open(f"{self.base_path}/mock_balance_sheet.json", "r")
-        elif event.get("function") == "INCOME_STATEMENT":
-            text_file = open(f"{self.base_path}/mock_income_statement.json", "r")
-        elif event.get("function") == "CASH_FLOW":
-            text_file = open(f"{self.base_path}/mock_cash_flow.json", "r")
-        elif event.get("function") == "EARNINGS":
-            text_file = open(f"{self.base_path}/mock_earnings.json", "r")
-        elif event.get("function") == "OVERVIEW":
-            text_file = open(f"{self.base_path}/mock_company_profile.json", "r")
-        elif event.get("function") == "CRYPTO_INTRADAY" and event.get("outputsize") == "full":
-            text_file = open(f"{self.base_path}/mock_crypto_full.json", "r")
-        elif event.get("function") == "REAL_GDP":
-            text_file = open(f"{self.base_path}/mock_real_gdp.json", "r")
-        elif event.get("function") == "EMA":
-            text_file = open(f"{self.base_path}/mock_technical_indicator_ema.json")
-        elif event.get("function") == "SMA":
-            text_file = open(f"{self.base_path}/mock_technical_indicator_sma_equity.json", "r")
-        elif event.get("function") == "TIME_SERIES_DAILY" and event.get("outputsize") == "compact":
-            text_file = open(f"{self.base_path}/mock_stock_price_full.json", "r")
-        elif event.get("function") == "TIME_SERIES_INTRADAY" and event.get("interval") == "5min":
-            text_file = open(f"{self.base_path}/mock_intraday_series_quote.json", "r")
-        elif event.get("function") == "NEWS_SENTIMENT":
-            text_file = open(f"{self.base_path}/mock_news_an_sentiment.json", "r")
-        else:
-            raise ValueError(f"We don't have a mock data file for your request {json.dumps(event)}")
-
-        data = text_file.read()
-        text_file.close()
-        json_response = json.loads(data)
-        json_response["success"] = True
+    def load_cache_from_disk(self):
+        self.use_simple_cache()
+        with open(f"{self.base_path}/mock_data.json",'r') as file:
+            json_string = file.read()
+        cache = json.loads(json_string)
+        self.__cache__ = cache
+
+    def get_data_from_alpha_vantage(self, event: dict, should_retry: bool = False) -> dict:
+        """
+        This is the underlying function that talks to alphavantage api.  Feel free to pass in any parameters supported
+        by the api.  You will receive a dictionary with the response from the web api. In addition, you will obtain
+        the ``success``, ``error_message`` and ``limit_reached`` fields.
+        Args:
+            event (dictionary): The url parameters supported by the web api
+
+        Returns:
+            :rtype: dict
+
+        """
+        # validate api key and insert into the request if needed
+        checks = ValidationRuleChecks().from_customer_request(event)
+        self.__validate_api_key__(checks, event)
+
+        # create a version of the event without api key
+        loggable_event = copy.deepcopy(event)
+        loggable_event.pop("apikey")
+
+        # check cache if allowed
+        if self.__use_cache__:
+            results = self.__get_item_from_cache__(loggable_event)
+            logging.info(f"Found item in cache: {results}")
+            if results is not None:
+                logging.info(json.dumps({"method": "mock.get_data_from_alpha_vantage"
+                                            , "action": "return_value", "data": results,
+                                         "event": loggable_event}))
+                return results
+        json_response = dict()
+        json_response["success"] = False
         json_response["limit_reached"] = False
         json_response["status_code"] = 200
         if "symbol" in event:
             json_response["symbol"] = event["symbol"]
+        json_response["error_message"] = "Could not find requested data"
         return json_response
```

## tests/test_multi_client_integration.py

```diff
@@ -1,499 +1,8 @@
-import pytest
-import time
-from alphavantage_api_client import AlphavantageClient, CsvNotSupported
-import logging
-import json
+from alphavantage_api_client import AlphavantageClient
+from .test_all_free_endpoints import AllEndPointTests
 
 
-# https://intellij-support.jetbrains.com/hc/en-us/community/posts/360000218290-Configure-google-docstring
-# above is reference for setting google docstring in pycharm
-def setup_function(function):
-    pass
+class TestMultiClientIntegrationSuite(AllEndPointTests):
 
-
-def teardown_function(function):
-    pass
-
-
-def setup_module(module):
-    pass
-
-
-def teardown_module(module):
-    pass
-
-
-@pytest.mark.integration
-def test_can_query_from_cache():
-    event = {
-        "symbol": "tsla"
-    }
-    client = AlphavantageClient().use_simple_cache()
-
-    for i in range(200):
-        global_quote = client.get_global_quote(event)
-        assert global_quote.success, f"success was found to be {global_quote.success}: {global_quote.error_message}"
-        assert global_quote.symbol == event.get("symbol"), "Response symbol doesn't matched requested symbol"
-        assert not global_quote.limit_reached, f"{global_quote.error_message}"
-        assert len(global_quote.data) > 0, "Response should have data but contains zero"
-
-    logging.warning(f" Can quote stock symbol in JSON using cache: {event.get('symbol', None)}")
-
-
-@pytest.mark.integration
-def test_can_get_global_quote_json():
-    event = {
-        "symbol": "tsla"
-    }
-    client = AlphavantageClient().should_retry_once()
-
-    global_quote = client.get_global_quote(event)
-    assert global_quote.success, f"success was found to be {global_quote.success}: {global_quote.error_message}"
-    assert global_quote.symbol == event.get("symbol"), "Response symbol doesn't matched requested symbol"
-    assert not global_quote.limit_reached, f"{global_quote.error_message}"
-    assert len(global_quote.data) > 0, "Response should have data but contains zero"
-    logging.warning(f" Can quote stock symbol in JSON {event.get('symbol', None)}")
-
-
-@pytest.mark.integration
-def test_can_not_get_global_quote_json():
-    event = {
-        "symbol": "tsla2"
-    }
-    client = AlphavantageClient().should_retry_once()
-
-    global_quote = client.get_global_quote(event)
-    assert not global_quote.success, f"success was found to be {global_quote.success}: {global_quote.error_message}"
-    assert global_quote.symbol == event.get("symbol"), "Response symbol doesn't matched requested symbol"
-    assert not global_quote.limit_reached, f"{global_quote.error_message}"
-    assert not len(global_quote.data), "Response should have data but contains zero"
-    logging.warning(f" Can Not quote stock symbol in JSON {event.get('symbol', None)}")
-
-
-@pytest.mark.integration
-def test_can_get_global_quote_csv():
-    event = {
-        "symbol": "tsla",
-        "datatype": "csv"
-    }
-    client = AlphavantageClient().should_retry_once()
-    global_quote = client.get_global_quote(event)
-    assert global_quote.success, f"success was found to be {global_quote.success}: {global_quote.error_message}"
-    assert global_quote.symbol == event.get("symbol"), "Response symbol doesn't matched requested symbol"
-    assert not global_quote.limit_reached, f"{global_quote.error_message}"
-    assert len(global_quote.csv) > 0, "Response should have data but contains zero"
-    logging.warning(f" Can quote stock symbol in CSV {event.get('symbol', None)}")
-
-
-@pytest.mark.integration
-def test_can_not_global_quote_wrong_symbol_json():
-    event = {
-        "symbol": "tsla2323"
-    }
-    client = AlphavantageClient().should_retry_once()
-    global_quote = client.get_global_quote(event)
-    assert not global_quote.success, f"success was found to be {global_quote.success}: {global_quote.error_message}"
-    assert global_quote.symbol == event.get("symbol"), "Response symbol doesn't matched requested symbol"
-    # assert not global_quote.limit_reached, f"{global_quote.error_message}"
-    assert not len(global_quote.data), "Response should have data but contains zero"
-    logging.warning(f" Can NOT quote stock symbol in JSON {event.get('symbol', None)}")
-
-
-@pytest.mark.integration
-def test_can_not_global_quote_wrong_symbol_csv():
-    event = {
-        "symbol": "tsla2233",
-        "datatype": "csv"
-    }
-    client = AlphavantageClient().should_retry_once()
-    global_quote = client.get_global_quote(event)
-    assert not global_quote.success, f"success: {global_quote.success}, msg: {global_quote.error_message}"
-    assert global_quote.symbol == event.get("symbol"), "Response symbol doesn't matched requested symbol"
-    # assert not global_quote.limit_reached, f"{global_quote.error_message}"
-    assert global_quote.csv is None, "Response should have data but contains zero"
-    logging.warning(f" Can NOT quote stock symbol in csv {event.get('symbol', None)} : {global_quote.error_message}")
-
-
-@pytest.mark.limit
-def test_can_reach_limit_json():
-    client = AlphavantageClient()
-    event = {
-        "symbol": "tsla"
-    }
-    limit_reached = False
-    results = None
-    # force limit reached
-    # my api key is free, so 5 calls per min and total of 500 per day
-    for i in range(20):
-        results = client.get_global_quote(event)
-        if results.limit_reached:
-            limit_reached = True
-            break
-
-    assert limit_reached, "Failed to reach limit"
-    assert results.symbol == event['symbol'], f" Expected symbol doesn't match given: {event.get('symbol', None)}"
-    logging.warning(f" Can Reach Limit while quoting for symbol {event.get('symbol', None)} in JSON")
-
-
-@pytest.mark.limit
-def test_can_reach_limit_csv():
-    client = AlphavantageClient()
-    event = {
-        "symbol": "tsla",
-        "datatype": "csv"
-    }
-    limit_reached = False
-    # force limit reached
-    # my api key is free, so 5 calls per min and total of 500 per day
-    results = None
-    for i in range(20):
-        results = client.get_global_quote(event)
-        if results.limit_reached:
-            limit_reached = True
-            break
-
-    assert limit_reached, "Failed to reach limit"
-    assert results.symbol == event['symbol'], f" Expected symbol doesn't match given: {event.get('symbol', None)}"
-
-    logging.warning(f" Can Reach Limit while quoting for symbol {event.get('symbol', None)} in JSON")
-
-
-@pytest.mark.integration
-def test_can_quote_intraday():
-    event = {
-        "symbol": "TSLA",
-        "interval": "5min"
-    }
-    client = AlphavantageClient().should_retry_once()
-    intra_day_quote = client.get_intraday_quote(event)
-    assert not intra_day_quote.limit_reached, f"limit_reached should not be true {intra_day_quote.error_message}"
-    assert intra_day_quote.success, f"success is false {intra_day_quote.error_message}"
-    assert len(intra_day_quote.data), f"Did not return data for this symbol {intra_day_quote.symbol}"
-    logging.warning(f" Successfully quoted cryptocurrency symbol {event['symbol']} in JSON")
-
-
-@pytest.mark.integration_paid
-def test_can_quote_daily():
-    event = {
-        "symbol": "VZ"
-    }
-    client = AlphavantageClient().should_retry_once()
-    daily_quote = client.get_daily_quote(event)
-    print(daily_quote.json())
-    assert not daily_quote.limit_reached, f"limit_reached should not be true {daily_quote.error_message}"
-    assert daily_quote.success, f"success is false {daily_quote.error_message}"
-    assert len(daily_quote.data), f"Did not return data for this symbol {daily_quote.symbol}"
-    logging.warning(f" Successfully quoted symbol {event['symbol']} in JSON")
-
-
-@pytest.mark.integrationn_paid
-def test_can_quote_crypto():
-    event = {
-        "function": "CRYPTO_INTRADAY",
-        "symbol": "ETH",
-        "market": "USD",
-        "interval": "5min"
-    }
-    client = AlphavantageClient().should_retry_once()
-    results = client.get_crypto_intraday(event)
-    assert not results.limit_reached, f"limit_reached should not be true {results.error_message}"
-    assert results.success, f"success is false {results.error_message}"
-    assert len(results.data), "Data{} property is empty but should have information"
-    logging.warning(f" Successfully quoted cryptocurrency symbol {event['symbol']} in JSON")
-
-
-@pytest.mark.integration_paid
-def test_can_quote_crypto_csv():
-    event = {
-        "function": "CRYPTO_INTRADAY",
-        "symbol": "ETH",
-        "market": "USD",
-        "interval": "5min",
-        "datatype": "csv"
-    }
-    client = AlphavantageClient().should_retry_once()
-    results = client.get_crypto_intraday(event)
-    assert not results.limit_reached, f"limit_reached should not be true {results.error_message}"
-    assert results.success, f"success is false {results.error_message}"
-    assert len(results.csv), "Data{} property is empty but should have information"
-    logging.warning(f" Successfully quoted cryptocurrency symbol {event['symbol']} in CSV")
-
-
-@pytest.mark.integration
-def test_can_quote_real_gdp():
-    client = AlphavantageClient().should_retry_once()
-    real_gdp = client.get_real_gdp()
-    assert not real_gdp.limit_reached, f"limit_reached is not present in results {real_gdp.error_message}"
-    assert real_gdp.success, f"Success=False but expected true  {real_gdp.error_message}"
-    assert len(real_gdp.data), "Data{} is empty but expected results"
-    logging.warning(" Can quote Real GDP")
-
-
-@pytest.mark.integration
-def test_can_quote_real_csv():
-    event = {
-        "function": "REAL_GDP",
-        "interval": "annual",
-        "datatype": "csv"
-    }
-    client = AlphavantageClient().should_retry_once()
-    real_gdp = client.get_real_gdp(event)
-    assert not real_gdp.limit_reached, f"limit_reached is not present in results {real_gdp.error_message}"
-    assert real_gdp.success, f"Success=False but expected true  {real_gdp.error_message}"
-    assert real_gdp.data is None, "Data{} is empty but expected results"
-    assert len(real_gdp.csv), "CSV data is not present"
-    logging.warning(" Can quote Real GDP")
-
-
-@pytest.mark.integration
-def test_can_quote_technical_indicator():
-    event = {
-        "function": "EMA",
-        "symbol": "IBM",
-        "interval": "weekly",
-        "time_period": "10",
-        "series_type": "open"
-    }
-    client = AlphavantageClient().should_retry_once()
-    technical_indicator = client.get_technical_indicator(event)
-    assert not technical_indicator.limit_reached, f"limit_reached is True {technical_indicator.error_message}"
-    assert technical_indicator.success, f"Success is False {technical_indicator.error_message}"
-    logging.warning(" Can quote IBM EMA technical indicator")
-
-
-@pytest.mark.integration
-def test_can_quote_technical_indicator_csv():
-    event = {
-        "function": "EMA",
-        "symbol": "IBM",
-        "interval": "weekly",
-        "time_period": "10",
-        "series_type": "open",
-        "datatype": "csv"
-    }
-    client = AlphavantageClient().should_retry_once()
-    technical_indicator = client.get_technical_indicator(event)
-    assert not technical_indicator.limit_reached, f"limit_reached is True {technical_indicator.error_message}"
-    assert technical_indicator.success, f"Success is False {technical_indicator.error_message}"
-    assert len(technical_indicator.csv), "Csv field is empty"
-    logging.warning(" Can quote IBM EMA technical indicator")
-
-
-@pytest.mark.integration
-def test_can_query_company_overview():
-    client = AlphavantageClient().should_retry_once()
-    event = {
-        "symbol": "TSLA"
-    }
-
-    company_overview = client.get_company_overview(event)
-    assert company_overview.success, f"Unable to get comapny overview {company_overview.error_message}"
-    assert company_overview.symbol == event.get(
-        "symbol"), f"Symbols are not equal {company_overview.symbol} : {event.get('symbol')}"
-    assert not company_overview.limit_reached, "unexpected limit_reached"
-    logging.warning(f" Can query company overview {event.get('symbol', None)}")
-
-
-@pytest.mark.integration
-def test_can_not_quote_company_overview():
-    client = AlphavantageClient().should_retry_once()
-    event = {
-        "symbol": "TSLA2"
-    }
-
-    company_overview = client.get_company_overview(event)
-    assert not company_overview.success, f"{event.get('symbol')} should not have been successful"
-    assert company_overview.symbol != event.get(
-        "symbol"), f"Symbols are equal {company_overview.symbol} : {event.get('symbol')} but shouldn't be"
-    assert not company_overview.limit_reached, "unexpected limit_reached"
-    logging.warning(f" Can not query company overview: {company_overview.error_message}")
-
-
-@pytest.mark.integration
-def test_can_not_query_csv_company_overview():
-    with pytest.raises(CsvNotSupported):
-        client = AlphavantageClient()
-        event = {
-            "symbol": "tsla",
-            "datatype": "csv"
-        }
-        client.get_company_overview(event)
-
-
-@pytest.mark.integration
-def test_can_not_query_income_statement():
-
-    event = {
-        "symbol": "tsla22354q2354"
-    }
-    client = AlphavantageClient()
-    accounting_report = client.get_income_statement(event)
-    assert not accounting_report.success, f"success was found to be True: {accounting_report.error_message}"
-    assert accounting_report.symbol == event.get("symbol", None), f"Symbols don't match " \
-                                                                  f"{accounting_report.symbol} : {event.get('symbol')}"
-    logging.warning(f" Can not query  income statement {accounting_report.error_message}")
-
-
-@pytest.mark.integration
-def test_can_query_income_statement():
-    client = AlphavantageClient().should_retry_once()
-    event = {
-        "symbol": "tsla"
-    }
-
-    accounting_report = client.get_income_statement(event)
-    assert accounting_report.success, f"success was found to be false: {accounting_report.error_message}"
-    assert not accounting_report.limit_reached, f'{accounting_report.error_message}'
-    assert accounting_report.symbol == event.get("symbol", None), f"Symbols don't match " \
-                                                                  f"{accounting_report.symbol} : {event.get('symbol')}"
-    logging.warning(f" Can query  income statement {event.get('symbol', None)}")
-
-
-@pytest.mark.integration
-def test_can_not_query_income_statement_csv():
-    with pytest.raises(CsvNotSupported):
-        client = AlphavantageClient()
-        event = {
-            "symbol": "tsla",
-            "datatype": "csv"
-        }
-        client.get_income_statement(event)
-
-
-@pytest.mark.integration
-def can_query_earnings():
-    client = AlphavantageClient().should_retry_once()
-    event = {
-        "symbol": "tsla"
-    }
-
-    earnings = client.get_earnings(event)
-    assert earnings.success, f"success was found to be false: {earnings.error_message}"
-    assert not earnings.limit_reached, f'{earnings.error_message}'
-    assert len(earnings.quarterlyReports), "quarterlyReports is empty"
-    assert len(earnings.annualReports), "annualReports is empty"
-    assert earnings.symbol == event.get("symbol"), f"Symbols not equal {earnings.symbol} : {event.get('symbol')}"
-    logging.warning(f" Can query  earnings {event.get('symbol', None)}")
-
-
-@pytest.mark.integration
-def test_can_query_income_statement():
-    client = AlphavantageClient().should_retry_once()
-    event = {
-        "symbol": "tsla"
-    }
-
-    income = client.get_income_statement(event)
-    assert income.success, f"Unable to get income {income.error_message}"
-    assert income.symbol == event.get("symbol"), f"Symbols are not equal {income.symbol} : {event.get('symbol')}"
-    assert not income.limit_reached, "limit_reached but should not have"
-    logging.warning(f" Can query income statement {event.get('symbol', None)}")
-
-
-@pytest.mark.integration
-def test_can_query_earnings():
-    client = AlphavantageClient().should_retry_once()
-    event = {
-        "symbol": "tsla"
-    }
-
-    earnings = client.get_earnings(event)
-    assert earnings.success, f"success was found to be false: {earnings.error_message}"
-    assert not earnings.limit_reached, f"limit_reached is not present in results {earnings.error_message}"
-    assert earnings.symbol == event.get("symbol"), f"Symbols not equal {earnings.symbol} : {event.get('symbol')}"
-    logging.warning(f" Can query earnings {event.get('symbol', None)}")
-
-
-@pytest.mark.integration
-def test_can_not_query_earnings():
-    client = AlphavantageClient().should_retry_once()
-    event = {
-        "symbol": "tsla22"
-    }
-
-    earnings = client.get_earnings(event)
-    assert not earnings.success, f"success was found to be false: {earnings.error_message}"
-    assert not earnings.limit_reached, f"limit_reached is not present in results {earnings.error_message}"
-    assert earnings.symbol == event.get("symbol"), f"Symbols not equal {earnings.symbol} : {event.get('symbol')}"
-    logging.warning(f" Can not query earnings: {earnings.error_message}")
-
-
-@pytest.mark.integration
-def test_can_not_query_earnings_csv():
-    with pytest.raises(CsvNotSupported):
-        client = AlphavantageClient()
-        event = {
-            "symbol": "tsla",
-            "datatype": "csv"
-        }
-        client.get_earnings(event)
-
-
-@pytest.mark.integration
-def test_can_query_cash_flow():
-    client = AlphavantageClient().should_retry_once()
-    event = {
-        "symbol": "tsla"
-    }
-
-    cash_flow = client.get_cash_flow(event)
-    assert cash_flow.success, f"success was found to be false: {cash_flow.error_message}"
-    assert not cash_flow.limit_reached, f"limit_reached is true {cash_flow.error_message}"
-    assert cash_flow.symbol == event.get("symbol"), f"Symbols do not match {cash_flow.symbol} : {event.get('symbol')}"
-    assert len(cash_flow.annualReports), "annualReports is empty"
-    assert len(cash_flow.quarterlyReports), "quarterlyReports are empty"
-    logging.warning(f" Can query  cash flow {event.get('symbol', None)}")
-
-
-@pytest.mark.integration
-def test_can_not_query_cash_flow():
-    client = AlphavantageClient().should_retry_once()
-    event = {
-        "symbol": "tsla22"
-    }
-
-    cash_flow = client.get_cash_flow(event)
-    assert not cash_flow.success, f"success was found to be True which is unexpected: {cash_flow.error_message}"
-    assert not cash_flow.limit_reached, f"limit_reached is true {cash_flow.error_message}"
-    assert cash_flow.symbol == event.get("symbol"), f"Symbols do not match {cash_flow.symbol} : {event.get('symbol')}"
-    assert not len(cash_flow.annualReports), "annualReports are not empty"
-    assert not len(cash_flow.quarterlyReports), "quarterlyReports are not empty"
-    logging.warning(f" Can not query  cash flow {cash_flow.error_message}")
-
-
-@pytest.mark.integration
-def test_can_not_query_cash_flow_csv():
-    with pytest.raises(CsvNotSupported):
-        client = AlphavantageClient()
-        event = {
-            "symbol": "tsla",
-            "datatype": "csv"
-        }
-        client.get_cash_flow(event)
-        logging.warning(f"Querying  cash flow as CSV threw error as expected {event.get('symbol', None)}")
-
-
-@pytest.mark.integration
-def test_get_data_from_alpha_vantage():
-    event = {
-        "function": "EMA"
-    }
-    client = AlphavantageClient().should_retry_once()
-    results = client.get_data_from_alpha_vantage(event)
-    assert type(results) is dict, "Results object should be a dictionary"
-    assert len(results) > 0, "There should be data in the results"
-
-    logging.warning("Successfully queried data using get_data_from_alpha_vantage")
-
-
-@pytest.mark.integration_paid
-def test_get_fx_currency_data():
-    event = {
-        "function" : "CURRENCY_EXCHANGE_RATE",
-        "from_currency" : "JPY",
-        "to_currency" : "USD"
-    }
-    client = AlphavantageClient().should_retry_once()
-    results = client.get_data_from_alpha_vantage(event)
-    print(results)
-    assert results["success"], f"FX Exchange call failed{results}"
+    def get_client(self) -> AlphavantageClient:
+        return AlphavantageClient().should_retry_once()
```

## Comparing `alphavantage_api_client-2.2.3.dist-info/LICENSE` & `alphavantage_api_client-2.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `alphavantage_api_client-2.2.3.dist-info/METADATA` & `alphavantage_api_client-2.3.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: alphavantage-api-client
-Version: 2.2.3
-Summary: Interact with Alphavantage REST API
+Version: 2.3.0
+Summary: Interact with Alpha Vantage REST API
 Home-page: https://github.com/xrgarcia/alphavantage-api-client
 Author: Slashbin, LLC
 Author-email: support@slashbin.us
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
@@ -312,8 +311,7 @@
 
 Process finished with exit code 0
 ```
 
 ## More!
 
 Check out our [wiki](https://github.com/xrgarcia/alphavantage_api_client/wiki) for more info!
-
```

