# Comparing `tmp/ir_client-0.1.3.tar.gz` & `tmp/ir_client-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ir_client-0.1.3.tar", max compression
+gzip compressed data, was "ir_client-0.1.4.tar", max compression
```

## Comparing `ir_client-0.1.3.tar` & `ir_client-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1068 2023-07-09 09:40:09.015525 ir_client-0.1.3/LICENSE
--rw-r--r--   0        0        0     1064 2023-07-09 09:32:13.241585 ir_client-0.1.3/ir_client/__init__.py
--rw-r--r--   0        0        0     1167 2023-07-09 09:32:13.257593 ir_client-0.1.3/ir_client/endpoint_parameters.py
--rw-r--r--   0        0        0     1624 2023-07-09 09:33:00.701328 ir_client-0.1.3/ir_client/endpoint_types.py
--rw-r--r--   0        0        0      319 2023-07-09 09:32:13.257593 ir_client-0.1.3/ir_client/exceptions.py
--rw-r--r--   0        0        0     1611 2023-07-09 09:33:00.701328 ir_client-0.1.3/ir_client/iracing_client.py
--rw-r--r--   0        0        0        0 2023-07-09 09:32:13.289609 ir_client-0.1.3/ir_client/laps/__init__.py
--rw-r--r--   0        0        0      706 2023-07-09 09:33:00.701328 ir_client-0.1.3/ir_client/laps/mappers.py
--rw-r--r--   0        0        0      680 2023-07-09 09:33:00.705330 ir_client-0.1.3/ir_client/laps/models.py
--rw-r--r--   0        0        0        0 2023-07-09 09:32:13.305617 ir_client-0.1.3/ir_client/series_race_results/__init__.py
--rw-r--r--   0        0        0     1227 2023-07-09 13:51:03.543560 ir_client-0.1.3/ir_client/series_race_results/mappers.py
--rw-r--r--   0        0        0      332 2023-07-09 09:32:13.325627 ir_client-0.1.3/ir_client/series_race_results/models.py
--rw-r--r--   0        0        0      104 2023-07-09 09:32:13.333631 ir_client-0.1.3/ir_client/session_parameters.py
--rw-r--r--   0        0        0        0 2023-07-09 09:32:13.333631 ir_client-0.1.3/ir_client/subsession_results/__init__.py
--rw-r--r--   0        0        0     4790 2023-07-09 09:33:00.737346 ir_client-0.1.3/ir_client/subsession_results/mappers.py
--rw-r--r--   0        0        0     1462 2023-07-09 09:33:00.709332 ir_client-0.1.3/ir_client/subsession_results/models.py
--rw-r--r--   0        0        0        0 2023-07-09 09:32:13.337633 ir_client-0.1.3/ir_client/utils/__init__.py
--rw-r--r--   0        0        0      369 2023-07-09 13:50:23.083392 ir_client-0.1.3/ir_client/utils/collections.py
--rw-r--r--   0        0        0      344 2023-07-09 09:32:13.337633 ir_client-0.1.3/ir_client/utils/datetime_utils.py
--rw-r--r--   0        0        0     1510 2023-07-09 09:32:13.337633 ir_client-0.1.3/ir_client/utils/enum_utils.py
--rw-r--r--   0        0        0     1540 2023-07-09 09:32:13.337633 ir_client-0.1.3/ir_client/utils/url_utils.py
--rw-r--r--   0        0        0      393 2023-07-09 13:56:34.864902 ir_client-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 ir_client-0.1.3/setup.py
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 ir_client-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-22 21:56:26.482107 ir_client-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1064 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/__init__.py
+-rw-r--r--   0        0        0     1167 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/endpoint_parameters.py
+-rw-r--r--   0        0        0     1624 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/endpoint_types.py
+-rw-r--r--   0        0        0      319 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/exceptions.py
+-rw-r--r--   0        0        0     1564 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/iracing_client.py
+-rw-r--r--   0        0        0        0 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/laps/__init__.py
+-rw-r--r--   0        0        0      706 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/laps/mappers.py
+-rw-r--r--   0        0        0      680 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/laps/models.py
+-rw-r--r--   0        0        0        0 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/series_race_results/__init__.py
+-rw-r--r--   0        0        0     1356 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/series_race_results/mappers.py
+-rw-r--r--   0        0        0      340 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/series_race_results/models.py
+-rw-r--r--   0        0        0      104 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/session_parameters.py
+-rw-r--r--   0        0        0        0 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/subsession_results/__init__.py
+-rw-r--r--   0        0        0     4790 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/subsession_results/mappers.py
+-rw-r--r--   0        0        0     1462 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/subsession_results/models.py
+-rw-r--r--   0        0        0        0 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/utils/__init__.py
+-rw-r--r--   0        0        0      385 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/utils/collections.py
+-rw-r--r--   0        0        0      344 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/utils/datetime_utils.py
+-rw-r--r--   0        0        0     1510 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/utils/enum_utils.py
+-rw-r--r--   0        0        0      229 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/utils/iterutils.py
+-rw-r--r--   0        0        0     1540 2023-07-22 21:56:26.482107 ir_client-0.1.4/ir_client/utils/url_utils.py
+-rw-r--r--   0        0        0      612 2023-07-22 21:56:26.482107 ir_client-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 ir_client-0.1.4/PKG-INFO
```

### Comparing `ir_client-0.1.3/LICENSE` & `ir_client-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.3/ir_client/__init__.py` & `ir_client-0.1.4/ir_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.3/ir_client/endpoint_parameters.py` & `ir_client-0.1.4/ir_client/endpoint_parameters.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.3/ir_client/endpoint_types.py` & `ir_client-0.1.4/ir_client/endpoint_types.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.3/ir_client/iracing_client.py` & `ir_client-0.1.4/ir_client/iracing_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from json import JSONDecodeError
-from starlette import status
 
 import requests
 
 from ir_client.exceptions import AuthorizationFailedException, InvalidDataException, MappingException
 from ir_client.utils.url_utils import build_absolute_url
 
 
@@ -30,10 +29,10 @@
 
         try:
             return endpoint_type.map_data(results.json())
         except (JSONDecodeError, MappingException) as e:
             raise InvalidDataException(endpoint_type_cls, endpoint_parameters, results.text) from e
     
     def _has_authorization_failed(self, response: requests.Response):
-        return response.status_code == status.HTTP_302_FOUND and (
+        return response.status_code == 302 and (
             "login.jsp" in response.headers['Location'] or "notauthed.jsp" in response.headers['Location']
         )
```

### Comparing `ir_client-0.1.3/ir_client/laps/mappers.py` & `ir_client-0.1.4/ir_client/laps/mappers.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.3/ir_client/laps/models.py` & `ir_client-0.1.4/ir_client/laps/models.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.3/ir_client/series_race_results/mappers.py` & `ir_client-0.1.4/ir_client/series_race_results/mappers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import List
 from ir_client.utils.collections import defaultordereddict #TODO extract different lib
 from more_itertools import unique_everseen
+from datetime import datetime, timezone
 
 from ir_client.exceptions import MappingException
 from ir_client.series_race_results.models import (
     SeriesRaceResult,
     SeriesRaceResultsSlot,
     SeriesRaceResultCollection
 )
@@ -12,15 +13,16 @@
 def map_series_race_results(data) -> SeriesRaceResultCollection:
     try:
         headers = {name: pos for (pos, name) in data['m'].items()}
         slots = defaultordereddict(lambda: SeriesRaceResultsSlot())
         races = _get_races(data, headers)
         for race in races:
             start_time = race[headers["start_time"]]
-            slots[start_time].results.append(_map_single_race(race, headers))
+            dt_start_time = datetime.fromtimestamp(start_time / 1e3, tz=timezone.utc)
+            slots[dt_start_time].results.append(_map_single_race(race, headers))
         return SeriesRaceResultCollection(slots=slots)
     except KeyError:
         raise InvalidSeriesRaceResultsDataException()
 
 def _get_races(data, headers):
     return unique_everseen(
         data['d'],
```

### Comparing `ir_client-0.1.3/ir_client/subsession_results/mappers.py` & `ir_client-0.1.4/ir_client/subsession_results/mappers.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.3/ir_client/subsession_results/models.py` & `ir_client-0.1.4/ir_client/subsession_results/models.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.3/ir_client/utils/enum_utils.py` & `ir_client-0.1.4/ir_client/utils/enum_utils.py`

 * *Files identical despite different names*

### Comparing `ir_client-0.1.3/ir_client/utils/url_utils.py` & `ir_client-0.1.4/ir_client/utils/url_utils.py`

 * *Files identical despite different names*

