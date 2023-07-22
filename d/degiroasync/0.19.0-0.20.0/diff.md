# Comparing `tmp/degiroasync-0.19.0.tar.gz` & `tmp/degiroasync-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degiroasync-0.19.0.tar", last modified: Mon Jul 17 18:16:16 2023, max compression
+gzip compressed data, was "degiroasync-0.20.0.tar", last modified: Sat Jul 22 08:29:25 2023, max compression
```

## Comparing `degiroasync-0.19.0.tar` & `degiroasync-0.20.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-17 18:16:16.624474 degiroasync-0.19.0/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1075 2022-01-20 21:38:48.000000 degiroasync-0.19.0/LICENSE
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     5039 2023-07-17 18:16:16.624474 degiroasync-0.19.0/PKG-INFO
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     4347 2023-07-08 15:05:00.000000 degiroasync-0.19.0/README.md
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-17 18:16:16.620474 degiroasync-0.19.0/degiroasync/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      692 2022-04-13 19:10:04.000000 degiroasync-0.19.0/degiroasync/__init__.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-17 18:16:16.620474 degiroasync-0.19.0/degiroasync/api/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     4330 2023-07-08 14:01:28.000000 degiroasync-0.19.0/degiroasync/api/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     8334 2022-05-12 19:40:07.000000 degiroasync-0.19.0/degiroasync/api/orders.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    35297 2023-07-13 13:06:08.000000 degiroasync-0.19.0/degiroasync/api/product.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     9298 2023-07-09 15:27:14.000000 degiroasync-0.19.0/degiroasync/api/session.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-17 18:16:16.620474 degiroasync-0.19.0/degiroasync/core/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1551 2023-03-13 17:53:33.000000 degiroasync-0.19.0/degiroasync/core/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     6565 2023-07-13 13:09:23.000000 degiroasync-0.19.0/degiroasync/core/constants.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    14341 2023-07-10 07:20:34.000000 degiroasync-0.19.0/degiroasync/core/core.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      547 2023-03-13 16:44:13.000000 degiroasync-0.19.0/degiroasync/core/exceptions.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    16450 2023-07-09 14:06:23.000000 degiroasync-0.19.0/degiroasync/core/helpers.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-17 18:16:16.620474 degiroasync-0.19.0/degiroasync/webapi/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1925 2023-07-08 14:01:46.000000 degiroasync-0.19.0/degiroasync/webapi/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     5967 2023-07-09 14:59:10.000000 degiroasync-0.19.0/degiroasync/webapi/login.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    12060 2023-07-02 17:18:26.000000 degiroasync-0.19.0/degiroasync/webapi/orders.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    29327 2023-07-10 07:36:11.000000 degiroasync-0.19.0/degiroasync/webapi/product.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-17 18:16:16.620474 degiroasync-0.19.0/degiroasync.egg-info/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     5039 2023-07-17 18:16:16.000000 degiroasync-0.19.0/degiroasync.egg-info/PKG-INFO
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      743 2023-07-17 18:16:16.000000 degiroasync-0.19.0/degiroasync.egg-info/SOURCES.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)        1 2023-07-17 18:16:16.000000 degiroasync-0.19.0/degiroasync.egg-info/dependency_links.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      270 2023-07-17 18:16:16.000000 degiroasync-0.19.0/degiroasync.egg-info/requires.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)       18 2023-07-17 18:16:16.000000 degiroasync-0.19.0/degiroasync.egg-info/top_level.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      108 2022-02-26 15:27:30.000000 degiroasync-0.19.0/pyproject.toml
--rw-rw-r--   0 laumas    (1000) laumas    (1000)       38 2023-07-17 18:16:16.624474 degiroasync-0.19.0/setup.cfg
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     2167 2023-07-09 16:49:30.000000 degiroasync-0.19.0/setup.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-17 18:16:16.624474 degiroasync-0.19.0/tests/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)        0 2023-07-02 12:58:48.000000 degiroasync-0.19.0/tests/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1504 2023-07-02 16:37:29.000000 degiroasync-0.19.0/tests/integration_login.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     4826 2023-07-08 08:25:07.000000 degiroasync-0.19.0/tests/test_core.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    37483 2023-07-09 16:16:22.000000 degiroasync-0.19.0/tests/test_degiroapi.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    18422 2023-07-09 16:53:26.000000 degiroasync-0.19.0/tests/test_degirowebapi.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      153 2022-01-27 15:50:02.000000 degiroasync-0.19.0/tests/test_setup.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 08:29:25.126965 degiroasync-0.20.0/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1075 2022-01-20 21:38:48.000000 degiroasync-0.20.0/LICENSE
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     5039 2023-07-22 08:29:25.126965 degiroasync-0.20.0/PKG-INFO
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4347 2023-07-08 15:05:00.000000 degiroasync-0.20.0/README.md
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 08:29:25.118965 degiroasync-0.20.0/degiroasync/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      692 2022-04-13 19:10:04.000000 degiroasync-0.20.0/degiroasync/__init__.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 08:29:25.122965 degiroasync-0.20.0/degiroasync/api/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4382 2023-07-21 19:06:29.000000 degiroasync-0.20.0/degiroasync/api/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     8334 2022-05-12 19:40:07.000000 degiroasync-0.20.0/degiroasync/api/orders.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    36107 2023-07-21 21:54:58.000000 degiroasync-0.20.0/degiroasync/api/product.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    14340 2023-07-21 19:48:47.000000 degiroasync-0.20.0/degiroasync/api/session.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 08:29:25.122965 degiroasync-0.20.0/degiroasync/core/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1551 2023-03-13 17:53:33.000000 degiroasync-0.20.0/degiroasync/core/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     6629 2023-07-21 18:43:03.000000 degiroasync-0.20.0/degiroasync/core/constants.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    14341 2023-07-10 07:20:34.000000 degiroasync-0.20.0/degiroasync/core/core.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      547 2023-03-13 16:44:13.000000 degiroasync-0.20.0/degiroasync/core/exceptions.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    16450 2023-07-09 14:06:23.000000 degiroasync-0.20.0/degiroasync/core/helpers.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 08:29:25.126965 degiroasync-0.20.0/degiroasync/webapi/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1925 2023-07-08 14:01:46.000000 degiroasync-0.20.0/degiroasync/webapi/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    17277 2023-07-21 14:22:18.000000 degiroasync-0.20.0/degiroasync/webapi/login.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    12060 2023-07-02 17:18:26.000000 degiroasync-0.20.0/degiroasync/webapi/orders.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    29667 2023-07-22 08:23:55.000000 degiroasync-0.20.0/degiroasync/webapi/product.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 08:29:25.118965 degiroasync-0.20.0/degiroasync.egg-info/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     5039 2023-07-22 08:29:25.000000 degiroasync-0.20.0/degiroasync.egg-info/PKG-INFO
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      743 2023-07-22 08:29:25.000000 degiroasync-0.20.0/degiroasync.egg-info/SOURCES.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)        1 2023-07-22 08:29:25.000000 degiroasync-0.20.0/degiroasync.egg-info/dependency_links.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      270 2023-07-22 08:29:25.000000 degiroasync-0.20.0/degiroasync.egg-info/requires.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)       18 2023-07-22 08:29:25.000000 degiroasync-0.20.0/degiroasync.egg-info/top_level.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      108 2022-02-26 15:27:30.000000 degiroasync-0.20.0/pyproject.toml
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)       38 2023-07-22 08:29:25.130965 degiroasync-0.20.0/setup.cfg
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     2167 2023-07-21 21:56:37.000000 degiroasync-0.20.0/setup.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 08:29:25.126965 degiroasync-0.20.0/tests/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)        0 2023-07-02 12:58:48.000000 degiroasync-0.20.0/tests/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1504 2023-07-02 16:37:29.000000 degiroasync-0.20.0/tests/integration_login.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4826 2023-07-08 08:25:07.000000 degiroasync-0.20.0/tests/test_core.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    45164 2023-07-21 21:56:03.000000 degiroasync-0.20.0/tests/test_degiroapi.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    19746 2023-07-22 08:24:06.000000 degiroasync-0.20.0/tests/test_degirowebapi.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      153 2022-01-27 15:50:02.000000 degiroasync-0.20.0/tests/test_setup.py
```

### Comparing `degiroasync-0.19.0/LICENSE` & `degiroasync-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `degiroasync-0.19.0/PKG-INFO` & `degiroasync-0.20.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degiroasync
-Version: 0.19.0
+Version: 0.20.0
 Summary: A Python asynchronous library for Degiro trading service.
 Home-page: https://github.com/OhMajesticLama/degiroasync
 Author-email: ohmajesticlama@gmail.com
 Project-URL: Documentation, https://ohmajesticlama.github.io/degiroasync/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `degiroasync-0.19.0/README.md` & `degiroasync-0.20.0/README.md`

 * *Files identical despite different names*

### Comparing `degiroasync-0.19.0/degiroasync/__init__.py` & `degiroasync-0.20.0/degiroasync/__init__.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.19.0/degiroasync/api/__init__.py` & `degiroasync-0.20.0/degiroasync/api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,16 +59,17 @@
 """
 from .orders import check_order
 from .orders import get_orders
 from .orders import get_transactions
 from .orders import Order
 from .orders import Transaction
 from .session import Session
+from .session import Index
 from .session import login
-from .session import get_exchange_dictionary
+from .session import get_dictionary
 from .session import ExchangeDictionary
 from .session import Exchange, Region, Country
 from .product import get_portfolio
 from .product import get_portfolio_total
 from .product import get_price_series
 from .product import get_price_data
 from .product import search_product
@@ -92,17 +93,20 @@
         # in object names are flagged by editor's tools and easier to catch
         # than typos in a string.
         obj.__name__ for obj in (  # type: ignore
             # Session
             login,
             Credentials,
             Session,
-            get_exchange_dictionary,
+            get_dictionary,
             ExchangeDictionary,
-            Exchange, Region, Country,
+            Exchange,
+            Region,
+            Country,
+            Index,
 
             # Product
             search_product,
             get_portfolio,
             get_price_data,
             get_price_series,
```

### Comparing `degiroasync-0.19.0/degiroasync/api/orders.py` & `degiroasync-0.20.0/degiroasync/api/orders.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.19.0/degiroasync/api/product.py` & `degiroasync-0.20.0/degiroasync/api/product.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 from ..core import ResponseError
 from ..core import Credentials, SessionCore, Config
 from ..core import check_session_client, check_session_config
 from ..core.helpers import dict_from_attr_list
 from ..core.helpers import camelcase_dict_to_snake
 from .session import Session
 from .session import Exchange
-from .session import check_session_exchange_dictionary
+from .session import Index
+from .session import check_session_dictionary
 
 
 LOGGER = logging.getLogger(LOGGER_NAME)
 
 
 class ProductBase:
     # Initial implementation of ProductBase included deferred populating of
@@ -254,15 +255,15 @@
                 if (
                         product_info.get('exchange_id')
                         and issubclass(inst_cls, Stock)
                         ):
                     # WARNING: There could be exchange_id key, but empty value,
                     # We don't want to set it here if that's the case
                     product_info['exchange'] = (
-                            session.exchange_dictionary.exchange_by(
+                            session.dictionary.exchange_by(
                                 id=product_info['exchange_id'])
                             )
                 # 2022.04 JSONclass poor compatibility with mypy
                 info = inst_cls.Info(product_info)  # type: ignore
                 instance = inst_cls(force_init=True)
                 # 2022.04 JSONclass poor compatibility with mypy
                 instance.base = inst_cls.Base(product_base)  # type: ignore
@@ -770,14 +771,15 @@
         session: Session,
         *,
         by_text: Optional[str] = None,
         by_isin: Optional[str] = None,
         by_symbol: Optional[str] = None,
         country_id: Optional[str] = None,
         exchange_id: Optional[Union[str, Exchange]] = None,
+        index_id: Optional[Union[str, Index]] = None,
         product_type_id: Optional[PRODUCT.TYPEID] = PRODUCT.TYPEID.STOCK,
         offset: int = 0,
         limit: int = 100,
         ) -> (Sequence[ProductBase], int, int):
     """
     Returns
     -------
@@ -807,14 +809,15 @@
         return True
 
     resp_json = await webapi.search_product(
         session,
         by_text,
         product_type_id=product_type_id,
         country_id=country_id,
+        index_id=index_id,
         limit=limit,
         offset=offset)
     LOGGER.debug("api.search_product response| %s",
                  pprint.pformat(resp_json))
     # Calls with more than one page could be parallelized:
     # First page is needed first to get the total answers, but
     # further pages could be fetched several at a time.
@@ -845,14 +848,15 @@
         session: Session,
         *,
         by_text: Optional[str] = None,
         by_isin: Optional[str] = None,
         by_symbol: Optional[str] = None,
         by_country: Optional[str] = None,
         by_exchange: Optional[Union[str, Exchange]] = None,
+        by_index: Optional[Union[str, Index]] = None,
         product_type_id: Optional[PRODUCT.TYPEID] = PRODUCT.TYPEID.STOCK,
         max_iter: Optional[int] = 1000
         ) -> List[ProductBase]:
     """
     Access `product_search` endpoint.
 
     Exactly one of `by_text`, `by_isin`, `by_symbol` be set.
@@ -876,18 +880,22 @@
             2 letters code.
 
         product_type_id
             Restricts search to one type of products.
             See :class:`~degiroasync.core.PRODUCT.TYPEID`
 
         by_exchange
-            Restricts results to products in a exchange. Can be either an
+            Restricts results to products in an exchange. Can be either an
             Exchange instance or an `hiq_abbr` str (e.g. EPA for Paris, AEX
             for Amsterdam)
 
+        by_index
+            Restricts results to products in an index. Can be either an
+            Index instance or an index `name` str.
+
         product_type_id
             Restricts search to one type of products.
 
         max_iter
             Pull `max_iter` pages of results. If `None`, don't stop until end
             is reached. Default value: 1000.
 
@@ -908,65 +916,81 @@
         # We've checked above that we only have one not-None search parameter.
         if by_symbol is not None:
             by_text = by_symbol
         elif by_isin is not None:
             by_text = by_isin
         elif by_country is not None:
             pass  # Could also be set without text deal with it after
+        elif by_index is not None:
+            pass  # Manage below
         else:
             raise AssertionError(
                     "by_text is None and no search parameters was set or "
                     "found. Have you set a search parameters to "
                     "search_product?"
                     "\n If yes, this shouldn't be happening, please open a bug"
                     " report."
                     )
 
     country_id = None
     if by_country is not None:
-        country = session.exchange_dictionary.country_by(
+        country = session.dictionary.country_by(
             name=by_country
                 )
         country_id = country.id
 
     exchange_id = None
     if by_exchange is not None:
         if isinstance(by_exchange, Exchange):
             exchange_id = by_exchange.id
         elif isinstance(by_exchange, str):
-            check_session_exchange_dictionary(session)
-            exchange = session.exchange_dictionary.exchange_by(
+            check_session_dictionary(session)
+            exchange = session.dictionary.exchange_by(
                 hiq_abbr=by_exchange)
             exchange_id = exchange.id
         else:
             raise TypeError(
                 "Only Exchange or str types supported for 'by_exchange'.")
 
+    index_id = None
+    if by_index is not None:
+        if isinstance(by_index, Index):
+            index_id = by_index.id
+        elif isinstance(by_index, str):
+            check_session_dictionary(session)
+            index = session.dictionary.index_by(name=by_index)
+            index_id = index.id
+        else:
+            raise TypeError(
+                "Only Index or str types supported for 'by_index'.")
+
     limit = 100
     products = []
 
     # trigger first call to get total:
     products, n_unfiltered, total = await _search_one(
             session,
             by_text=by_text,
             by_isin=by_isin,
             by_symbol=by_symbol,
             country_id=country_id,
             exchange_id=exchange_id,
+            index_id=index_id,
             offset=0,
             limit=limit
             )
 
     if n_unfiltered < total:
         # Generate args
         args = ({
             'session': session,
             'by_text': by_text,
             'by_isin': by_isin,
             'by_symbol': by_symbol,
+            'index_id': index_id,
             'country_id': country_id,
             'exchange_id': exchange_id,
             'offset': offset,
             'limit': limit,
             } for offset in range(n_unfiltered, total, limit)
             )
         # The use of _search_one and gather improves performance over
```

### Comparing `degiroasync-0.19.0/degiroasync/core/__init__.py` & `degiroasync-0.20.0/degiroasync/core/__init__.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.19.0/degiroasync/core/constants.py` & `degiroasync-0.20.0/degiroasync/core/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,28 +228,31 @@
 
         CURRENCY
             Currencies. This is used by endpoint for account balances for
             instance.
 
         """
         STOCK = 1
+        INDEX = 180
         BONDS = 2
         FUTURES = 7
         OPTIONS = 8
         FUNDS = 13
         LEVERAGE_PRODUCTS = 14
         ETFS = 131
         CFDS = 535
         WARRANTS = 536
         CURRENCY = 311
 
     class TYPE(StrEnum):
         STOCK = 'STOCK'
+        INDEX = 'INDEX'
         FUND = 'FUND'
         CASH = 'CASH'
+        CFD = 'CFD'
         CURRENCY = 'CURRENCY'
 
 
 class SORT(StrEnum):
     """
     Used by some endpoints to provide sorted results.
```

### Comparing `degiroasync-0.19.0/degiroasync/core/core.py` & `degiroasync-0.20.0/degiroasync/core/core.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.19.0/degiroasync/core/exceptions.py` & `degiroasync-0.20.0/degiroasync/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.19.0/degiroasync/core/helpers.py` & `degiroasync-0.20.0/degiroasync/core/helpers.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.19.0/degiroasync/webapi/__init__.py` & `degiroasync-0.20.0/degiroasync/webapi/__init__.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.19.0/degiroasync/webapi/orders.py` & `degiroasync-0.20.0/degiroasync/webapi/orders.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.19.0/degiroasync/webapi/product.py` & `degiroasync-0.20.0/degiroasync/webapi/product.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,21 @@
 LOGGER = logging.getLogger(LOGGER_NAME)
 
 
 async def get_portfolio(session: SessionCore) -> Dict[str, Any]:
     """
     Get portfolio web call.
 
-    Example return:
+
+    Returns
+    -------
+
+    Example dictionary portfolio:
+
+    .. code-block:: python
 
         {'portfolio': {'isAdded': True,
          'lastUpdated': 1088,
          'name': 'portfolio',
          'value': [
             {'id': '8614787',
              'isAdded': True,
@@ -565,15 +571,15 @@
         except Exception:
             LOGGER.error('get_products_info response| %s', response)
             LOGGER.error('get_products_info url| %s', url)
             LOGGER.error('get_products_info products_ids| %s', products_ids)
             LOGGER.error('get_products_info products_ids| %s', products_ids)
             raise
         resp_json = response.json()
-        LOGGER.debug('get_products_info|', resp_json)
+        LOGGER.debug('get_products_info| %s', resp_json)
     return resp_json
 
 
 async def get_company_profile(
         session: SessionCore,
         isin: str) -> Dict[str, Any]:
     """
@@ -821,17 +827,20 @@
         country_id: Optional[str] = None,
         index_id: Optional[str] = None,
         limit: int = 50,
         offset: int = 0) -> Dict[str, Any]:
     """
     Access `product_search` endpoint.
 
-    Example response:
+    Returns
+    -------
+
+    Example JSON response below, will be returned as a Python dict.
 
-    .. code-block:: python
+    .. code-block:: JSON
 
         {
             "offset": 0,
             "products": [
                 {
                     "active": true,
                     "buyOrderTypes": [
@@ -892,22 +901,26 @@
     params = dict(
         offset=offset,
         limit=limit,
         intAccount=session.client.int_account,
         sessionId=session.config.session_id,
         requireTotal=True
     )
-    if search_txt is not None:
-        params['searchText'] = search_txt
     if product_type_id is not None:
         params['productTypeId'] = product_type_id
     if country_id is not None:
         params['stockCountryId'] = country_id
     if index_id is not None:
         params['indexId'] = index_id
+        if search_txt is None:
+            # 202307: Searching by indexId with no 'searchTxt' triggers
+            # internal server error. We must provide an empty string
+            search_txt = ''
+    if search_txt is not None:
+        params['searchText'] = search_txt
     LOGGER.debug("webapi.search_product params| %s", params)
     async with session as client:
         response = await client.get(url,
                                     cookies=session._cookies,
                                     params=params)
     check_response(response)
     LOGGER.debug("webapi.search_product response| %s", response.json())
```

### Comparing `degiroasync-0.19.0/degiroasync.egg-info/PKG-INFO` & `degiroasync-0.20.0/degiroasync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degiroasync
-Version: 0.19.0
+Version: 0.20.0
 Summary: A Python asynchronous library for Degiro trading service.
 Home-page: https://github.com/OhMajesticLama/degiroasync
 Author-email: ohmajesticlama@gmail.com
 Project-URL: Documentation, https://ohmajesticlama.github.io/degiroasync/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `degiroasync-0.19.0/degiroasync.egg-info/SOURCES.txt` & `degiroasync-0.20.0/degiroasync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `degiroasync-0.19.0/setup.py` & `degiroasync-0.20.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     description = "A Python asynchronous library for Degiro trading service."
     readme_path = os.path.join(os.path.dirname(__file__), 'README.md')
     with open(readme_path, "r") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name="degiroasync",
-        version="0.19.0",
+        version="0.20.0",
         author_email="ohmajesticlama@gmail.com",
         description=description,
         long_description=long_description,
         long_description_content_type='text/markdown',
         url="https://github.com/OhMajesticLama/degiroasync",
         project_urls={
             'Documentation':
```

### Comparing `degiroasync-0.19.0/tests/integration_login.py` & `degiroasync-0.20.0/tests/integration_login.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.19.0/tests/test_core.py` & `degiroasync-0.20.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.19.0/tests/test_degiroapi.py` & `degiroasync-0.20.0/tests/test_degiroapi.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,22 +13,23 @@
 import degiroasync
 import degiroasync.webapi
 import degiroasync.api
 import degiroasync.webapi
 import degiroasync.core
 import degiroasync.core.helpers
 from degiroasync.core import Credentials
-#from degiroasync.api.product import convert_time_series
 from degiroasync.api import ProductFactory
 from degiroasync.api import Order
 from degiroasync.api import ORDER
 from degiroasync.api import Exchange
+from degiroasync.api import Index
 from degiroasync.core.constants import PRODUCT
 from degiroasync.core.constants import PRICE
 from degiroasync.core import BadCredentialsError
+from degiroasync.core import camelcase_dict_to_snake
 
 from tests.integration_login import _get_credentials
 from tests.integration_login import _IntegrationLogin
 
 
 LOGGER = logging.getLogger(degiroasync.core.LOGGER_NAME)
 LOGGER.setLevel(logging.DEBUG)
@@ -235,56 +236,228 @@
                         'id': 710, 'code': 'XPAR', 'hiqAbbr': 'EPA',
                         'country': 'FR', 'city': 'Paris', 'micCode': 'XPAR',
                         'name': 'Euronext Paris'},
                     {
                         'id': 200, 'code': 'XAMS', 'hiqAbbr': 'EAM',
                         'country': 'NL', 'city': 'Amsterdam',
                         'micCode': 'XAMS', 'name': 'Euronext Amsterdam'}
-                    ]
+                    ],
+                'indices': [{'id': '106002', 'name': 'SDAX'},
+                            {'id': '106001', 'name': 'MDAX'},
+                            {'id': '5',
+                             'name': 'CAC 40',
+                             'productId': 4824940},
+                            {'id': '121003',
+                             'name': 'SMIM',
+                             'productId': 11875105},
+                            {'id': 114003, 'name': 'ISEQ Overall'},
+                            {'id': 121002, 'name': 'SLI',
+                             'productId': 11875104}],
             }
         self.get_product_dictionary_mock = resp_mock
 
     @unittest.mock.patch('degiroasync.webapi.get_product_dictionary')
-    async def test_exchange_dictionary_attributes(self, get_dict_mock):
+    async def test_dictionary_attributes(self, get_dict_mock):
         # Mock webapi.get_product_dictionary
         get_dict_mock.return_value = self._product_dictionary_dummy
         session = object()  # dummy is enough, we mocked the class
         dictionary = await degiroasync.api.ExchangeDictionary(session)
 
         regions = dictionary.regions
         self.assertIn('Europe', (r.name for r in regions))
         countries = dictionary.countries
         self.assertIn('NL', (c.name for c in countries))
         exchanges = dictionary.exchanges
         self.assertIn('XAMS', (e.mic_code for e in exchanges))
 
     @unittest.mock.patch('degiroasync.webapi.get_product_dictionary')
-    async def test_exchange_dictionary_exchange(self, get_dict_mock):
+    async def test_dictionary_exchange(self, get_dict_mock):
         # Mock webapi.get_product_dictionary
         get_dict_mock.return_value = self._product_dictionary_dummy
         session = object()  # dummy is enough, we mocked the class
         dictionary = await degiroasync.api.ExchangeDictionary(session)
 
         eam_exc = dictionary.exchange_by(hiq_abbr='EAM')
         self.assertEqual(eam_exc.mic_code, 'XAMS')
         self.assertEqual(eam_exc.country_name, 'NL')
 
     @unittest.mock.patch('degiroasync.webapi.get_product_dictionary')
-    async def test_exchange_dictionary_country(self, get_dict_mock):
+    async def test_dictionary_country(self, get_dict_mock):
         # Mock webapi.get_product_dictionary
         get_dict_mock.return_value = self._product_dictionary_dummy
         session = object()  # dummy is enough, we mocked the class
         dictionary = await degiroasync.api.ExchangeDictionary(session)
 
         country = dictionary.country_by(name='FR')
         self.assertEqual(country.region.name, 'Europe')
 
         country = dictionary.country_by(name='NL')
         self.assertEqual(country.region.name, 'Europe')
 
+    @unittest.mock.patch('degiroasync.webapi.get_product_dictionary')
+    async def test_dictionary_index(self, get_dict_mock):
+        # Mock webapi.get_product_dictionary
+        get_dict_mock.return_value = self._product_dictionary_dummy
+        session = object()  # dummy is enough, we mocked the class
+        dictionary = await degiroasync.api.ExchangeDictionary(session)
+
+        index = dictionary.index_by(name='CAC 40')
+        self.assertEqual(index.name, 'CAC 40')
+        index = dictionary.index_by(id='5')
+        self.assertEqual(index.name, 'CAC 40')
+
+    @unittest.mock.patch('degiroasync.webapi.get_products_info')
+    async def test_dictionary_index_info(
+            self,
+            get_products_info_mock):
+        # Mock webapi.get_product_dictionary
+        get_products_info_mock.return_value = {
+              "data": {
+                "4824940": {
+                  "id": "4824940",
+                  "name": "CAC 40",
+                  "isin": "FR0003500008",
+                  "symbol": "CAC INDEX",
+                  "contractSize": 1,
+                  "productType": "INDEX",
+                  "productTypeId": 180,
+                  "tradable": False,
+                  "category": "H",
+                  "currency": "EUR",
+                  "active": True,
+                  "exchangeId": "710",
+                  "onlyEodPrices": False,
+                  "orderTimeTypes": [],
+                  "buyOrderTypes": [],
+                  "sellOrderTypes": [],
+                  "productBitTypes": [],
+                  "closePrice": 7384.91,
+                  "closePriceDate": "2023-07-20",
+                  "feedQuality": "R",
+                  "orderBookDepth": 0,
+                  "vwdIdentifierType": "issueid",
+                  "vwdId": "360015511",
+                  "qualitySwitchable": False,
+                  "qualitySwitchFree": False,
+                  "vwdModuleId": 1
+                }
+              }
+            }
+
+        session = MagicMock()  # dummy is enough, the call is mocked
+        session.dictionary = MagicMock()
+        session.dictionary.exchange_by = MagicMock(
+                return_value=Exchange(dict(
+                    id='id',
+                    name='name',
+                    country_name='COUNTRYCODE',
+                    hiq_abbr='TDG'
+                    ))
+                )
+        data = self._product_dictionary_dummy['indices'][2]
+        data['productId'] = str(data['productId'])
+        data = camelcase_dict_to_snake(data)
+        index = Index(data)
+
+        self.assertEqual(index.name, 'CAC 40')
+        await index.get_info(session)
+        self.assertEqual(index.info.isin, "FR0003500008")
+
+
+class TestSearchProduct(unittest.IsolatedAsyncioTestCase):
+    @unittest.mock.patch('degiroasync.webapi.get_products_info')
+    @unittest.mock.patch('degiroasync.webapi.search_product')
+    async def test_search_by_index(
+            self,
+            search_product_m,
+            get_products_info_m,
+            ):
+        get_products_info_m.return_value = {'data': {
+                '123': {
+                    'id': '123',
+                    'productTypeId': 99,
+                    'name': 'foo',
+                    'symbol': 'FOO',
+                    'currency': 'EUR',
+                    'exchangeId': 'exid',
+                    'tradable': True,
+                    'isin': 'isinexample',
+                }
+            }
+        }
+        session = MagicMock()
+        session.dictionary = MagicMock()
+        index = MagicMock()
+        index.id = '123'
+        index.name = 'CAC 40'
+        session.dictionary.index_by = MagicMock(return_value=index)
+
+        search_product_m.return_value = {
+            "total": 1,
+            "offset": 0,
+            "products": [
+                {
+                    "active": True,
+                    "buyOrderTypes": [
+                        "LIMIT",
+                        "MARKET",
+                        "STOPLOSS",
+                        "STOPLIMIT"
+                    ],
+                    "category": "B",
+                    "closePrice": 113.3,
+                    "closePriceDate": "2022-02-02",
+                    "contractSize": 1.0,
+                    "currency": "EUR",
+                    "exchangeId": "710",
+                    "feedQuality": "R",
+                    "feedQualitySecondary": "CX",
+                    "id": "123",
+                    "isin": "NL0000235190",
+                    "name": "AIRBUS",
+                    "onlyEodPrices": False,
+                    "orderBookDepth": 0,
+                    "orderBookDepthSecondary": 0,
+                    "orderTimeTypes": [
+                        "DAY",
+                        "GTC"
+                    ],
+                    "productBitTypes": [],
+                    "productType": "STOCK",
+                    "productTypeId": 1,
+                    "qualitySwitchFree": False,
+                    "qualitySwitchFreeSecondary": False,
+                    "qualitySwitchable": False,
+                    "qualitySwitchableSecondary": False,
+                    "sellOrderTypes": [
+                        "LIMIT",
+                        "MARKET",
+                        "STOPLOSS",
+                        "STOPLIMIT"
+                    ],
+                    "strikePrice": -0.0001,
+                    "symbol": "AIR",
+                    "tradable": True,
+                    "vwdId": "360114899",
+                    "vwdIdSecondary": "955000256",
+                    "vwdIdentifierType": "issueid",
+                    "vwdIdentifierTypeSecondary": "issueid",
+                    "vwdModuleId": 1,
+                    "vwdModuleIdSecondary": 2
+                }
+            ]
+        }
+
+        products = await degiroasync.api.search_product(
+                session,
+                by_index='CAC 40'
+                )
+        # There should be only one product returned by the mock
+        self.assertGreaterEqual(len(products), 1)
+
 
 class TestProduct(unittest.IsolatedAsyncioTestCase):
     """
     Local tests for Product.
     """
     @unittest.mock.patch('degiroasync.webapi.get_products_info')
     async def test_product(self, wapi_prodinfo_m):
@@ -299,25 +472,24 @@
                     'tradable': True,
                     'isin': 'isinexample',
                 }
             }
         }
 
         session = MagicMock()  # Don't care
-        session.exchange_dictionary = MagicMock()
-        session.exchange_dictionary.exchange_by = MagicMock(
+        session.dictionary = MagicMock()
+        session.dictionary.exchange_by = MagicMock(
                 return_value=Exchange(dict(
                     id='exid',
                     name='EuroNext',
                     country_name='France',
                     hiq_abbr='EPA',
-            )
-        )
-
+                    )
                 )
+        )
 
         # Test that degiroasync.api returns properly initiated products
         products_gen = ProductFactory.init_batch(
                 session,
                 (
                     {
                         'id': '123',
@@ -344,16 +516,16 @@
                     'exchangeId': 'exid',
                     'tradable': True,
                     'isin': 'isinexample',
                 }
             }
         }
         session = MagicMock()  # Don't care
-        session.exchange_dictionary = MagicMock()
-        session.exchange_dictionary.exchange_by = MagicMock(
+        session.dictionary = MagicMock()
+        session.dictionary.exchange_by = MagicMock(
                 return_value=Exchange(dict(
                     id='exid',
                     name='EuroNext',
                     country_name='France',
                     hiq_abbr='EPA',
                         )
                     )
@@ -373,14 +545,15 @@
         self.assertEqual(len(products), 1)
         self.assertEqual(products[0].base.id, '123')
         self.assertEqual(products[0].base.additional, 123)
         self.assertEqual(products[0].info.name, 'foo')
         self.assertEqual(products[0].info.symbol, 'FOO')
 
 
+
 class TestDegiroasyncPrice(
         unittest.IsolatedAsyncioTestCase):
 
     def test_priceseries_items(self):
         resp_json = {
                 'requestid': '1',
                 'start': '2023-06-29T00:00:00',
@@ -813,21 +986,33 @@
                     )
             # The point of implementing filtering on symbol and exchange
             # is to target one specific product. Raise an error if it doesn't
             # work.
             self.assertGreaterEqual(len(products), 1)
             for product in products:
                 self.assertEqual(
-                        session.exchange_dictionary.exchange_by(
+                        session.dictionary.exchange_by(
                             id=product.info.exchange_id).country_name,
                         'FR'
                         )
 
+        async def test_search_product_index(self):
+            session = await _IntegrationLogin._login()
+            products = await degiroasync.api.search_product(
+                    session,
+                    by_index='CAC 40',
+                    max_iter=1,  # We don't need every product for this test.
+                    )
+            LOGGER.debug("Integration Test search_product_index| %s", products)
+            # The point of implementing filtering on symbol and exchange
+            # is to target one specific product. Raise an error if it doesn't
+            # work.
+            self.assertEqual(len(products), 40)
+
     class TestDegiroasyncIntegrationExchangeDictionary(
-            _IntegrationLogin,
             unittest.IsolatedAsyncioTestCase):
         async def test_product_dictionary_attributes(self):
             session = await _IntegrationLogin._login()
             dictionary = await degiroasync.api.ExchangeDictionary(session)
 
             regions = dictionary.regions
             self.assertIn('Europe', (r.name for r in regions))
@@ -839,16 +1024,29 @@
         async def test_product_dictionary_exchange_by(self):
             session = await _IntegrationLogin._login()
             dictionary = await degiroasync.api.ExchangeDictionary(session)
             eam_exc = dictionary.exchange_by(hiq_abbr='EAM')
             self.assertEqual(eam_exc.mic_code, 'XAMS')
             self.assertEqual(eam_exc.country_name, 'NL')
 
+        async def test_index_populate_indices(self):
+            session = await _IntegrationLogin._login()
+            await session.dictionary.populate_indices_info(session)
+
+            index = session.dictionary.index_by(name='CAC 40')
+            self.assertEqual(index.info.symbol, 'CAC INDEX')
+
+        async def test_index_info(self):
+            session = await _IntegrationLogin._login()
+            index = session.dictionary.index_by(name='CAC 40')
+            await index.get_info(session)
+
+            self.assertEqual(index.info.symbol, 'CAC INDEX')
+
     class TestDegiroasyncIntegrationOrders(
-            _IntegrationLogin,
             unittest.IsolatedAsyncioTestCase):
         async def test_get_orders(self):
             session = await _IntegrationLogin._login()
             orders, orders_hist = await degiroasync.api.get_orders(session)
             LOGGER.debug("test_get_orders orders| %s", orders)
             LOGGER.debug("test_get_orders orders hist| %s", orders_hist)
             for o in itertools.chain(orders, orders_hist):
@@ -898,14 +1096,15 @@
                     time_type=ORDER.TIME.DAY,
                     order_type=ORDER.TYPE.LIMITED,
                     size=1,
                     price=80
             )
             self.assertIn('confirmation_id', order_check)
 
+
 if __name__ == '__main__':
     handler = logging.StreamHandler()
     handler.setLevel(logging.DEBUG)
     formatter = logging.Formatter(
             "%(asctime)s-%(name)s-%(levelname)s-%(message)",
             "%Y%m%d"
             )
```

### Comparing `degiroasync-0.19.0/tests/test_degirowebapi.py` & `degiroasync-0.20.0/tests/test_degirowebapi.py`

 * *Files 18% similar despite different names*

```diff
@@ -244,14 +244,45 @@
                     search)
             self.assertIn('products', resp_json, resp_json)
             self.assertGreaterEqual(len(resp_json['products']), 1)
             self.assertIn('id', resp_json['products'][0], resp_json)
             self.assertIn('isin', resp_json['products'][0], resp_json)
             self.assertIn('name', resp_json['products'][0], resp_json)
 
+        #async def test_search_product_exchange(self):
+        #    raise NotImplementedError()
+        #    session = await _IntegrationLogin._login()
+
+        #    search = "AIRBUS"
+        #    resp_json = await degiroasync.webapi.search_product(
+        #            session,
+        #            search)
+        #    self.assertIn('products', resp_json, resp_json)
+        #    self.assertGreaterEqual(len(resp_json['products']), 1)
+        #    self.assertIn('id', resp_json['products'][0], resp_json)
+        #    self.assertIn('isin', resp_json['products'][0], resp_json)
+        #    self.assertIn('name', resp_json['products'][0], resp_json)
+
+        async def test_search_product_by_index(self):
+            session = await _IntegrationLogin._login()
+            resp_json = await degiroasync.webapi.get_product_dictionary(
+                    session,
+                    )
+
+            index = session.dictionary.index_by(name='CAC 40')
+            LOGGER.debug("test_search_product_by_index| Index: %s", index)
+            resp_json = await degiroasync.webapi.search_product(
+                    session,
+                    index_id=index.id,
+                    limit=100
+                    )
+            self.assertIn('products', resp_json, resp_json)
+            # We should have 40 products in CAC 40
+            self.assertGreaterEqual(len(resp_json['products']), 40)
+
         async def test_product_dictionary(self):
             session = await _IntegrationLogin._login()
 
             resp_json = await degiroasync.webapi.get_product_dictionary(
                     session
                     )
 
@@ -287,15 +318,15 @@
 
             # Leverage api.search_product to get a specific product_id
             # as example for integration testing of check_order.
             # This is introducing a dependency on api module, but is easier
             # to manage. Future improvement opportunit for this test: implement
             # required query and filter here using only webapi.
             from degiroasync import api
-            session.exchange_dictionary = await api.get_exchange_dictionary(
+            session.dictionary = await api.get_dictionary(
                     session)
             products = await api.search_product(
                     session,
                     by_symbol="AIR",
                     by_exchange="EPA",
                     product_type_id=PRODUCT.TYPEID.STOCK
                     )
@@ -367,15 +398,14 @@
                     )
             LOGGER.debug("test_get_orders_history| response: %s", resp_json)
 
             self.assertIn('data', resp_json)
             data = resp_json['data']
             for order in data:
                 self.assertIn('created', order)
-                self.assertIn('orderId', order)
                 self.assertIn('productId', order)
                 self.assertIn('size', order)
                 self.assertIn('price', order)
                 self.assertIn('buysell', order)
                 self.assertIn(order['buysell'], ('B', 'S'))
                 self.assertIn('orderTypeId', order)
                 self.assertIn('orderTimeTypeId', order)
```

