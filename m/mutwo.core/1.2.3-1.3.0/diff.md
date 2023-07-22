# Comparing `tmp/mutwo.core-1.2.3.tar.gz` & `tmp/mutwo.core-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutwo.core-1.2.3.tar", last modified: Fri Mar 17 21:11:53 2023, max compression
+gzip compressed data, was "mutwo.core-1.3.0.tar", last modified: Sat Jul 22 15:45:11 2023, max compression
```

## Comparing `mutwo.core-1.2.3.tar` & `mutwo.core-1.3.0.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-17 21:11:53.312962 mutwo.core-1.2.3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1875 2023-03-17 21:11:53.312962 mutwo.core-1.2.3/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1011 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-17 21:11:53.308962 mutwo.core-1.2.3/mutwo/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-17 21:11:53.308962 mutwo.core-1.2.3/mutwo/core_constants/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1085 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_constants/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-17 21:11:53.308962 mutwo.core-1.2.3/mutwo/core_converters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_converters/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9365 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_converters/abc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      383 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_converters/configurations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9604 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_converters/parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13881 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_converters/tempos.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-17 21:11:53.312962 mutwo.core-1.2.3/mutwo/core_events/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      897 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_events/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43798 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_events/abc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    39347 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_events/basic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2964 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_events/configurations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    34846 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_events/envelopes.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-17 21:11:53.312962 mutwo.core-1.2.3/mutwo/core_generators/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_generators/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2320 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_generators/generic.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-17 21:11:53.312962 mutwo.core-1.2.3/mutwo/core_parameters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_parameters/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12600 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_parameters/abc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      771 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_parameters/configurations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_parameters/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      915 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_parameters/durations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2777 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_parameters/tempos.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-17 21:11:53.312962 mutwo.core-1.2.3/mutwo/core_utilities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_utilities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      230 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_utilities/configurations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5297 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_utilities/decorators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6467 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_utilities/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1226 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_utilities/tests.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17689 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_utilities/tools.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-17 21:11:53.312962 mutwo.core-1.2.3/mutwo/core_version/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/mutwo/core_version/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-17 21:11:53.308962 mutwo.core-1.2.3/mutwo.core.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1875 2023-03-17 21:11:53.000000 mutwo.core-1.2.3/mutwo.core.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1065 2023-03-17 21:11:53.000000 mutwo.core-1.2.3/mutwo.core.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-17 21:11:53.000000 mutwo.core-1.2.3/mutwo.core.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2023-03-17 21:11:53.000000 mutwo.core-1.2.3/mutwo.core.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-03-17 21:11:53.000000 mutwo.core-1.2.3/mutwo.core.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-03-17 21:11:53.312962 mutwo.core-1.2.3/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1610 2023-03-17 21:11:42.000000 mutwo.core-1.2.3/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-22 15:45:11.749225 mutwo.core-1.3.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1875 2023-07-22 15:45:11.749225 mutwo.core-1.3.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1011 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-22 15:45:11.741225 mutwo.core-1.3.0/mutwo/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-22 15:45:11.745225 mutwo.core-1.3.0/mutwo/core_configurations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_configurations/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-22 15:45:11.745225 mutwo.core-1.3.0/mutwo/core_constants/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1085 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_constants/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-22 15:45:11.745225 mutwo.core-1.3.0/mutwo/core_converters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_converters/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9365 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_converters/abc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      383 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_converters/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9604 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_converters/parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13946 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_converters/tempos.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-22 15:45:11.745225 mutwo.core-1.3.0/mutwo/core_events/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      919 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_events/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    46357 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_events/abc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    50443 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_events/basic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4872 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_events/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    37267 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_events/envelopes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      763 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_events/tempos.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-22 15:45:11.745225 mutwo.core-1.3.0/mutwo/core_generators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_generators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2320 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_generators/generic.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-22 15:45:11.749225 mutwo.core-1.3.0/mutwo/core_parameters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_parameters/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12600 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_parameters/abc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      771 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_parameters/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_parameters/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      915 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_parameters/durations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2777 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_parameters/tempos.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-22 15:45:11.749225 mutwo.core-1.3.0/mutwo/core_utilities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_utilities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      230 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_utilities/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5297 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_utilities/decorators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7168 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_utilities/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1226 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_utilities/tests.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18488 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_utilities/tools.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-22 15:45:11.749225 mutwo.core-1.3.0/mutwo/core_version/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/mutwo/core_version/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-22 15:45:11.745225 mutwo.core-1.3.0/mutwo.core.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1875 2023-07-22 15:45:11.000000 mutwo.core-1.3.0/mutwo.core.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1131 2023-07-22 15:45:11.000000 mutwo.core-1.3.0/mutwo.core.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-22 15:45:11.000000 mutwo.core-1.3.0/mutwo.core.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2023-07-22 15:45:11.000000 mutwo.core-1.3.0/mutwo.core.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-07-22 15:45:11.000000 mutwo.core-1.3.0/mutwo.core.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-22 15:45:11.749225 mutwo.core-1.3.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1610 2023-07-22 15:44:57.000000 mutwo.core-1.3.0/setup.py
```

### Comparing `mutwo.core-1.2.3/LICENSE` & `mutwo.core-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mutwo.core-1.2.3/PKG-INFO` & `mutwo.core-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutwo.core
-Version: 1.2.3
+Version: 1.3.0
 Summary: core library for event based framework mutwo
 Home-page: https://github.com/mutwo-org/mutwo
 Author: Tim Pauli, Levin Eric Zimmermann
 Author-email: tim.pauli@folkwang-uni.de, levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mutwo.core-1.2.3/README.md` & `mutwo.core-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mutwo.core-1.2.3/mutwo/core_constants/__init__.py` & `mutwo.core-1.3.0/mutwo/core_constants/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Definition of global variables which are used all over mutwo.
+"""Definition of global constants which are used all over mutwo.
 """
 
 import fractions
 import typing
 
 import quicktions
```

### Comparing `mutwo.core-1.2.3/mutwo/core_converters/abc.py` & `mutwo.core-1.3.0/mutwo/core_converters/abc.py`

 * *Files identical despite different names*

### Comparing `mutwo.core-1.2.3/mutwo/core_converters/parsers.py` & `mutwo.core-1.3.0/mutwo/core_converters/parsers.py`

 * *Files identical despite different names*

### Comparing `mutwo.core-1.2.3/mutwo/core_converters/tempos.py` & `mutwo.core-1.3.0/mutwo/core_converters/tempos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Apply tempo curve on any :class:`~mutwo.core_events.abc.Event` and convert :class:`~mutwo.core_parameters.abc.TempoPoint` to beat-length-in-seconds.
 
 """
 
 import functools
 import typing
-import warnings
 
 from mutwo import core_constants
 from mutwo import core_converters
 from mutwo import core_events
 from mutwo import core_parameters
 from mutwo import core_utilities
 
@@ -35,33 +34,35 @@
 
     >>> from mutwo import core_converters
     >>> tempo_point_converter = core_converters.TempoPointToBeatLengthInSeconds()
     """
 
     TempoPoint = core_parameters.abc.TempoPoint | core_constants.Real
 
+    def __init__(self):
+        self._logger = core_utilities.get_cls_logger(type(self))
+
     @staticmethod
     def _beats_per_minute_to_seconds_per_beat(
         beats_per_minute: core_constants.Real,
     ) -> float:
         return float(60 / beats_per_minute)
 
-    @staticmethod
     def _extract_beats_per_minute_and_reference_from_tempo_point(
-        tempo_point: TempoPoint,
+        self, tempo_point: TempoPoint
     ) -> tuple[core_constants.Real, core_constants.Real]:
         try:
             beats_per_minute = tempo_point.tempo_in_beats_per_minute  # type: ignore
         except AttributeError:
             beats_per_minute = float(tempo_point)  # type: ignore
 
         try:
             reference = tempo_point.reference  # type: ignore
         except AttributeError:
-            warnings.warn(core_utilities.UndefinedReferenceWarning(tempo_point))
+            self._logger.warn(core_utilities.UndefinedReferenceWarning(tempo_point))
             reference = 1
 
         return beats_per_minute, reference
 
     def convert(self, tempo_point_to_convert: TempoPoint) -> float:
         """Converts a :class:`TempoPoint` to beat-length-in-seconds.
```

### Comparing `mutwo.core-1.2.3/mutwo/core_events/__init__.py` & `mutwo.core-1.3.0/mutwo/core_events/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     - :class:`mutwo.core_events.SimultaneousEvent`
 """
 
 from . import configurations
 from . import abc
 
 from .basic import *
+from .tempos import *
 from .envelopes import *
 
 from . import basic, envelopes
 
 from mutwo import core_utilities
 
 __all__ = core_utilities.get_all(basic, envelopes)
```

### Comparing `mutwo.core-1.2.3/mutwo/core_events/abc.py` & `mutwo.core-1.3.0/mutwo/core_events/abc.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,19 @@
         """Helper method to make sure that start < end.
 
         Can be used within the different cut_out methods.
         """
         if not condition(start, end):
             raise core_utilities.InvalidStartAndEndValueError(start, end)
 
+    @staticmethod
+    def _assert_valid_absolute_time(t: core_parameters.abc.Duration):
+        if t < 0:
+            raise core_utilities.InvalidAbsoluteTime(t)
+
     @functools.cached_property
     def _event_to_metrized_event(self):
         # Import in method to avoid circular import error
         return __import__(
             "mutwo.core_converters"
         ).core_converters.EventToMetrizedEvent()
 
@@ -339,19 +344,19 @@
 
         **Example:**
 
         >>> from mutwo import core_events
         >>> simple_event = core_events.SimpleEvent(duration = 1)
         >>> simple_event.tempo_envelope[0].value = 100
         >>> simple_event.tempo_envelope
-        TempoEnvelope([SimpleEvent(curve_shape = 0, duration = DirectDuration(duration = 1), tempo_point = 60, value = 100), SimpleEvent(curve_shape = 0, duration = DirectDuration(duration = 0), tempo_point = 60)])
+        TempoEnvelope([TempoEvent(curve_shape = 0, duration = DirectDuration(duration = 1), tempo_point = DirectTempoPoint(BPM = 60, reference = 1), value = 100), TempoEvent(curve_shape = 0, duration = DirectDuration(duration = 0), tempo_point = DirectTempoPoint(BPM = 60, reference = 1))])
         >>> simple_event.reset_tempo_envelope()
         SimpleEvent(duration = DirectDuration(duration = 1))
         >>> simple_event.tempo_envelope
-        TempoEnvelope([SimpleEvent(curve_shape = 0, duration = DirectDuration(duration = 1), tempo_point = 60), SimpleEvent(curve_shape = 0, duration = DirectDuration(duration = 0), tempo_point = 60)])
+        TempoEnvelope([TempoEvent(curve_shape = 0, duration = DirectDuration(duration = 1), tempo_point = DirectTempoPoint(BPM = 60, reference = 1)), TempoEvent(curve_shape = 0, duration = DirectDuration(duration = 0), tempo_point = DirectTempoPoint(BPM = 60, reference = 1))])
         """
 
         self.tempo_envelope = core_events.TempoEnvelope([[0, 60], [1, 60]])
 
     @abc.abstractmethod
     def metrize(self) -> typing.Optional[Event]:
         """Apply tempo envelope of event on itself
@@ -408,39 +413,73 @@
         ...     [core_events.SimpleEvent(3), core_events.SimpleEvent(2)]
         ... )
         >>> sequential_event.cut_off(1, 3)
         SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 1)), SimpleEvent(duration = DirectDuration(duration = 2))])
         """
 
     def split_at(
-        self, absolute_time: core_parameters.abc.Duration
-    ) -> tuple[Event, Event]:
-        """Split event in two events at :attr:`absolute_time`.
-
-        :param absolute_time: where event shall be split
-        :return: Two events that result from splitting the present event.
+        self,
+        *absolute_time: core_parameters.abc.Duration,
+        ignore_invalid_split_point: bool = False,
+    ) -> tuple[Event, ...]:
+        """Split event into *n* events at :attr:`absolute_time`.
+
+        :param *absolute_time: where event shall be split
+        :param ignore_invalid_split_point: If set to `True` `split_at` won't raise
+            :class:`mutwo.core_utilities.SplitError` in case a split time isn't
+            inside the duration range of the event. Otherwise the exception is raised.
+            Default to ``False``.
+        :raises: :class:`mutwo.core_utilities.NoSplitTimeError` if no `absolute_time`
+            is given. Raises :class:`mutwo.core_utilities.InvalidAbsoluteTime` if any
+            absolute_time is smaller than 0. Raises :class:`mutwo.core_utilities.SplitError`
+            if any absolute_time is bigger than the events duration and
+            `ignore_invalid_split_point` is not set.
+        :return:  Tuple of events that result from splitting the present event.
+
+        **Hint:**
+
+        Calling ``split_at`` once with multiple split time arguments is much more efficient
+        than calling ``split_at`` multiple times with only one split time for
+        :class:`mutwo.core_events.SequentialEvent`.
 
         **Example:**
 
         >>> from mutwo import core_events
         >>> sequential_event = core_events.SequentialEvent([core_events.SimpleEvent(3)])
         >>> sequential_event.split_at(1)
         (SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 1))]), SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 2))]))
         >>> sequential_event[0].split_at(1)
         (SimpleEvent(duration = DirectDuration(duration = 1)), SimpleEvent(duration = DirectDuration(duration = 2)))
         """
+        if not absolute_time:
+            raise core_utilities.NoSplitTimeError()
 
-        absolute_time = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(
-            absolute_time
-        )
+        absolute_time_list = list(sorted(absolute_time))
+        # Already sorted => check if smallest t < 0
+        self._assert_valid_absolute_time(absolute_time_list[0])
+        if 0 not in absolute_time_list:
+            absolute_time_list.insert(0, core_parameters.DirectDuration(0))
+
+        if (duration := self.duration) > absolute_time_list[-1]:
+            absolute_time_list.append(duration)
+        elif duration < absolute_time_list[-1] and not ignore_invalid_split_point:
+            raise core_utilities.SplitError(absolute_time_list[-1])
 
-        return (
-            self.cut_out(0, absolute_time, mutate=False),  # type: ignore
-            self.cut_out(absolute_time, self.duration, mutate=False),  # type: ignore
-        )
+        split_event_list = []
+        for t0, t1 in zip(absolute_time_list, absolute_time_list[1:]):
+            try:
+                split_event_list.append(self.cut_out(t0, t1, mutate=False))
+            except (
+                core_utilities.InvalidStartAndEndValueError,
+                core_utilities.InvalidCutOutStartAndEndValuesError,
+            ):
+                if not ignore_invalid_split_point:
+                    raise core_utilities.SplitError(t0)
+
+        return tuple(split_event_list)
 
 
 T = typing.TypeVar("T", bound=Event)
 
 
 # FIXME(This Event can be initialised (no abstract error).
 # Please see the following issue for comparison:
@@ -451,14 +490,15 @@
     def __init__(
         self,
         iterable: typing.Iterable[T] = [],
         tempo_envelope: typing.Optional[core_events.TempoEnvelope] = None,
     ):
         Event.__init__(self, tempo_envelope)
         list.__init__(self, iterable)
+        self._logger = core_utilities.get_cls_logger(type(self))
 
     def __init_subclass__(
         cls, class_specific_side_attribute_tuple: tuple[str, ...] = tuple([])
     ):
         # It's better to prove `class_specific_side_attribute_tuple`
         # as a class initialisation attribute instead of a simple class attribute,
         # because with a simple class attribute we have no guarantee that the
@@ -702,23 +742,32 @@
         but also the `concatenate_by...` methods of ``SimultaneousEvent``.
 
         It's important to first call this method before appending the
         child events of the other container, because we still need
         to know the original duration of the target event. Due to this
         difficulty this method is private.
         """
-        other_tempo_envelope = other.tempo_envelope.copy()
-        # We first set the duration of the tempo envelopes to the
-        # duration of the given event. This is necessary, because the
-        # tempo envelope duration is always relative to the events duration.
-        # If we don't set them to this absolute value, the inner
-        # relationships may be distorted after concatenation.
-        self.tempo_envelope.duration = self.duration
-        other_tempo_envelope.duration = other.duration
-        self.tempo_envelope.extend(other_tempo_envelope)
+        # We need to ensure the tempo envelope of the event
+        # is as long as it's duration, otherwise the others tempo
+        # envelope may be postponed (if our envelope is longer
+        # than the event) or may be too early (if our envelope
+        # is shorted than the event).
+        # We don't care here if the others event envelope is too
+        # short or too long, because the relationships are still
+        # the same.
+        if (d := self.duration) < (d_env := self.tempo_envelope.duration):
+            self._logger.warning(
+                f"Tempo envelope of '{str(self)[:35]}...' needed "
+                "to be truncated because the envelope was "
+                "longer than the actual event."
+            )
+            self.tempo_envelope.cut_out(0, d)
+        elif d > d_env:
+            self.tempo_envelope.extend_until(d)
+        self.tempo_envelope.extend(other.tempo_envelope.copy())
 
     # ###################################################################### #
     #                           public methods                               #
     # ###################################################################### #
 
     def destructive_copy(self) -> ComplexEvent[T]:
         empty_copy = self.empty_copy()
```

### Comparing `mutwo.core-1.2.3/mutwo/core_events/basic.py` & `mutwo.core-1.3.0/mutwo/core_events/basic.py`

 * *Files 20% similar despite different names*

```diff
@@ -242,14 +242,15 @@
         start: core_parameters.abc.Duration,
         end: core_parameters.abc.Duration,
     ) -> SimpleEvent:
         start, end = (
             core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
             for unknown_object in (start, end)
         )
+        self._assert_valid_absolute_time(start)
         self._assert_correct_start_and_end_values(
             start, end, condition=lambda start, end: start < end
         )
 
         duration = self.duration
 
         difference_to_duration: core_parameters.DirectDuration = (
@@ -275,14 +276,15 @@
         end: core_parameters.abc.Duration,
     ) -> SimpleEvent:
         start, end = (
             core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
             for unknown_object in (start, end)
         )
 
+        self._assert_valid_absolute_time(start)
         self._assert_correct_start_and_end_values(start, end)
 
         duration = self.duration
         if start < duration:
             if end > duration:
                 end = duration
 
@@ -370,14 +372,57 @@
                 event.cut_off(0, cut_off_duration - difference_to_event_start)
 
         for index in reversed(event_to_delete_list):
             del self[index]
 
         return self
 
+    def _split_child_at(
+        self,
+        absolute_time: core_parameters.abc.Duration | typing.Any,
+        absolute_time_in_floats_tuple: tuple[float, ...],
+        duration_in_floats: float,
+    ) -> int:
+        absolute_time = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(
+            absolute_time
+        )
+        self._assert_valid_absolute_time(absolute_time)
+        absolute_time_in_floats = absolute_time.duration_in_floats
+
+        event_index = SequentialEvent._get_index_at_from_absolute_time_tuple(
+            absolute_time_in_floats, absolute_time_in_floats_tuple, duration_in_floats
+        )
+
+        # If there is no event at the requested time, raise error
+        if event_index is None:
+            raise core_utilities.SplitUnavailableChildError(absolute_time)
+
+        # Only try to split child event at the requested time if there isn't
+        # a segregation already anyway
+        elif absolute_time_in_floats != absolute_time_in_floats_tuple[event_index]:
+            try:
+                end = absolute_time_in_floats_tuple[event_index + 1]
+            except IndexError:
+                end = duration_in_floats
+
+            difference = end - absolute_time_in_floats
+            split_event = self[event_index].split_at(difference)
+            split_event_count = len(split_event)
+            match split_event_count:
+                case 1:
+                    pass
+                case 2:
+                    self[event_index] = split_event[0]
+                    self.insert(event_index, split_event[1])
+                case _:
+                    raise RuntimeError("Unexpected event count!")
+
+            return event_index + 1
+        return event_index
+
     # ###################################################################### #
     #                        private   properties                            #
     # ###################################################################### #
 
     @property
     def _absolute_time_tuple_and_duration(
         self,
@@ -541,14 +586,15 @@
         start: core_constants.DurationType,
         end: core_constants.DurationType,
     ) -> SequentialEvent[T]:
         start, end = (
             core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
             for unknown_object in (start, end)
         )
+        self._assert_valid_absolute_time(start)
         self._assert_correct_start_and_end_values(start, end)
 
         event_to_remove_index_list = []
         for event_index, event_start, event in zip(
             range(len(self)), self.absolute_time_tuple, self
         ):
             event_duration = event.duration
@@ -584,29 +630,31 @@
         start: core_constants.DurationType,
         end: core_constants.DurationType,
     ) -> SequentialEvent[T]:
         start, end = (
             core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
             for unknown_object in (start, end)
         )
+        self._assert_valid_absolute_time(start)
+
         cut_off_duration = end - start
 
         # Avoid unnecessary iterations
         if cut_off_duration > 0:
             return self._cut_off(start, end, cut_off_duration)
 
     @core_utilities.add_copy_option
     def squash_in(  # type: ignore
         self,
         start: core_parameters.abc.Duration | typing.Any,
         event_to_squash_in: core_events.abc.Event,
     ) -> SequentialEvent[T]:
         start = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(start)
+        self._assert_valid_absolute_time(start)
         start_in_floats = start.duration_in_floats
-
         self._assert_start_in_range(start_in_floats)
 
         # Only run cut_off if necessary -> Improve performance
         if (event_to_squash_in_duration := event_to_squash_in.duration) > 0:
             cut_off_end = start + event_to_squash_in_duration
             self._cut_off(start, cut_off_end, event_to_squash_in_duration)
 
@@ -656,68 +704,99 @@
     @core_utilities.add_copy_option
     def slide_in(
         self,
         start: core_parameters.abc.Duration,
         event_to_slide_in: core_events.abc.Event,
     ) -> SequentialEvent[T]:
         start = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(start)
+        self._assert_valid_absolute_time(start)
         start_in_floats = start.duration_in_floats
+        if start_in_floats == 0:
+            self.insert(0, event_to_slide_in)
+            return self
         self._assert_start_in_range(start_in_floats)
-        self[:], b = self.split_at(start)
-        self.extend([event_to_slide_in] + b)
+        try:
+            self[:], b = self.split_at(start)
+        except ValueError:  # Only one event => start == duration.
+            self.append(event_to_slide_in)
+        else:
+            self.extend([event_to_slide_in] + b)
         return self
 
     @core_utilities.add_copy_option
     def split_child_at(
         self, absolute_time: core_parameters.abc.Duration | typing.Any
     ) -> SequentialEvent[T]:
-        absolute_time_in_floats = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(
-            absolute_time
-        ).duration_in_floats
         (
             absolute_time_in_floats_tuple,
             duration_in_floats,
         ) = self._absolute_time_in_floats_tuple_and_duration
 
-        event_index = SequentialEvent._get_index_at_from_absolute_time_tuple(
-            absolute_time_in_floats, absolute_time_in_floats_tuple, duration_in_floats
+        return self._split_child_at(
+            absolute_time, absolute_time_in_floats_tuple, duration_in_floats
         )
 
-        # If there is no event at the requested time, raise error
-        if event_index is None:
-            raise core_utilities.SplitUnavailableChildError(absolute_time)
+    def split_at(
+        self,
+        *absolute_time: core_parameters.abc.Duration,
+        ignore_invalid_split_point: bool = False,
+    ) -> tuple[SequentialEvent, ...]:
+        if not absolute_time:
+            raise core_utilities.NoSplitTimeError()
 
-        # Only try to split child event at the requested time if there isn't
-        # a segregation already anyway
-        elif absolute_time_in_floats != absolute_time_in_floats_tuple[event_index]:
+        (
+            absolute_time_in_floats_tuple,
+            duration_in_floats,
+        ) = self._absolute_time_in_floats_tuple_and_duration
+
+        absolute_time_list = list(absolute_time_in_floats_tuple)
+
+        # NOTE: maybe we can add a 'mutate=False' keyword in case
+        # someone doesn't care about keeping the old event and wants
+        # to save some seconds of expensive copy-operation?
+        c = self.copy()
+
+        index_list = []
+        is_first = True
+        for t in sorted(absolute_time):
+            if is_first:  # First is smallest, check if t < 0
+                self._assert_valid_absolute_time(t)
+                is_first = False
+            # Improve performance: don't try to split if we know it is
+            # already split here. We also need to be sure to not
+            # add any duplicates to 'absolute_time_list', so we need
+            # to check anyway.
+            if t in absolute_time_list:
+                index_list.append(absolute_time_list.index(t))
+                continue
+            # It's okay to ignore, this is still within the given event
+            # (if we don't continue 'split_child_at' raises an error).
+            if t == duration_in_floats:
+                continue
             try:
-                end = absolute_time_in_floats_tuple[event_index + 1]
-            except IndexError:
-                end = duration_in_floats
+                i = c._split_child_at(t, tuple(absolute_time_list), duration_in_floats)
+            except core_utilities.SplitUnavailableChildError:
+                if not ignore_invalid_split_point:
+                    raise core_utilities.SplitError(t)
+                # We can stop, because if there isn't any child at this time
+                # there won't be any child at a later time (remember: our
+                # absolute times are sorted).
+                break
+            index_list.append(i)
+            absolute_time_list.append(t)
+            absolute_time_list.sort()
+
+        # Add frame indices (if not already present)
+        if 0 not in index_list:
+            index_list.insert(0, 0)
 
-            difference = end - absolute_time_in_floats
-            first_event, second_event = self[event_index].split_at(difference)
-            self[event_index] = first_event
-            self.insert(event_index, second_event)
+        if (event_count := len(c)) not in index_list:
+            index_list.append(event_count)
 
-    def split_at(
-        self, absolute_time: core_parameters.abc.Duration
-    ) -> tuple[SequentialEvent, SequentialEvent]:
-        absolute_time = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(
-            absolute_time
-        )
-        absolute_time_tuple = self.absolute_time_tuple
-        # Only run expensive 'split_at' in case we can't simply
-        # split via slice.
-        try:
-            index = absolute_time_tuple.index(absolute_time)
-        except ValueError:
-            return super().split_at(absolute_time)
-        else:
-            return self[:index].copy(), self[index:].copy()
+        return tuple(c[i0:i1] for i0, i1 in zip(index_list, index_list[1:]))
 
     @core_utilities.add_copy_option
     def extend_until(
         self,
         duration: core_parameters.abc.Duration,
         duration_to_white_space: typing.Optional[
             typing.Callable[[core_parameters.abc.Duration], core_events.abc.Event]
@@ -759,14 +838,53 @@
             # This should already fail above, but if this strange object
             # somehow owned '_concatenate_tempo_envelope', it should
             # fail here.
             case _:
                 raise core_utilities.ConcatenationError(ancestor, event)
 
     # ###################################################################### #
+    #                           private methods                              #
+    # ###################################################################### #
+
+    def _make_event_slice_tuple(
+        self,
+        absolute_time_list: list[core_parameters.abc.Duration],
+        slice_tuple_to_event: typing.Callable[
+            [tuple[core_parameters.abc.Event, ...]], core_parameters.abc.Event
+        ],
+    ) -> tuple[core_events.abc.Event, ...]:
+        """Split at given times and cast split events into new events."""
+
+        # Slice all child events
+        slices = []
+        for e in self:
+            slices.append(
+                list(e.split_at(*absolute_time_list, ignore_invalid_split_point=True))
+            )
+
+        # Ensure all slices have the same amount of entries,
+        # because we use 'zip' later and if one of them is
+        # shorter we loose some parts of our event.
+        if slices:
+            slices_count_tuple = tuple(len(s) for s in slices)
+            max_slice_count = max(slices_count_tuple)
+            for s, c in zip(slices, slices_count_tuple):
+                if delta := max_slice_count - c:
+                    s.extend([None] * delta)
+
+        # Finally, build new sequence from event slices
+        event_list = []
+        for slice_tuple in zip(*slices):
+            if slice_tuple := tuple(filter(bool, slice_tuple)):
+                e = slice_tuple_to_event(slice_tuple)
+                event_list.append(e)
+
+        return tuple(event_list)
+
+    # ###################################################################### #
     #                           properties                                   #
     # ###################################################################### #
 
     @core_events.abc.ComplexEvent.duration.getter
     def duration(self) -> core_constants.DurationType:
         try:
             return max(event.duration for event in self)
@@ -784,37 +902,40 @@
         start: core_parameters.abc.Duration | typing.Any,
         end: core_parameters.abc.Duration | typing.Any,
     ) -> SimultaneousEvent[T]:
         start, end = (
             core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
             for unknown_object in (start, end)
         )
+        self._assert_valid_absolute_time(start)
         self._assert_correct_start_and_end_values(start, end)
         [event.cut_out(start, end) for event in self]
 
     @core_utilities.add_copy_option
     def cut_off(  # type: ignore
         self,
         start: core_constants.DurationType,
         end: core_constants.DurationType,
     ) -> SimultaneousEvent[T]:
         start, end = (
             core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
             for unknown_object in (start, end)
         )
+        self._assert_valid_absolute_time(start)
         self._assert_correct_start_and_end_values(start, end)
         [event.cut_off(start, end) for event in self]
 
     @core_utilities.add_copy_option
     def squash_in(  # type: ignore
         self,
         start: core_parameters.abc.Duration | typing.Any,
         event_to_squash_in: core_events.abc.Event,
     ) -> SimultaneousEvent[T]:
         start = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(start)
+        self._assert_valid_absolute_time(start)
         self._assert_start_in_range(start)
 
         for event in self:
             try:
                 event.squash_in(start, event_to_squash_in)  # type: ignore
             # Simple events don't have a 'squash_in' method.
             except AttributeError:
@@ -823,14 +944,15 @@
     @core_utilities.add_copy_option
     def slide_in(
         self,
         start: core_parameters.abc.Duration,
         event_to_slide_in: core_events.abc.Event,
     ) -> SimultaneousEvent[T]:
         start = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(start)
+        self._assert_valid_absolute_time(start)
         self._assert_start_in_range(start)
         for event in self:
             try:
                 event.slide_in(start, event_to_slide_in)  # type: ignore
             # Simple events don't have a 'slide_in' method.
             except AttributeError:
                 raise core_utilities.ImpossibleToSlideInError(self, event_to_slide_in)
@@ -851,15 +973,15 @@
     def extend_until(
         self,
         duration: typing.Optional[core_parameters.abc.Duration] = None,
         duration_to_white_space: typing.Optional[
             typing.Callable[[core_parameters.abc.Duration], core_events.abc.Event]
         ] = None,
         prolong_simple_event: bool = True,
-    ) -> SequentialEvent:
+    ) -> SimultaneousEvent[T]:
         duration = (
             self.duration
             if duration is None
             else core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(duration)
         )
         duration_to_white_space = (
             duration_to_white_space
@@ -897,31 +1019,43 @@
         :param mutate: If ``False`` the function will return a copy of the given object.
             If set to ``True`` the object itself will be changed and the function will
             return the changed object. Default to ``True``.
         :type mutate: bool
         :raises core_utilities.ConcatenationError: If there are any :class:`SimpleEvent`
             inside a :class:`SimultaneousEvent`.
 
+        **Hint:**
+
+        Similarly to Pythons ``list.extend`` the concatenation simply appends
+        the children of the other event to the sequence without copying them.
+        This means when changing the children in the new event, it also changes
+        the child event in the original sequence. If you want to avoid this,
+        call ``event.copy()`` before concatenating it to the host event.
+
         **Example:**
 
         >>> from mutwo import core_events
         >>> s = core_events.SimultaneousEvent(
         ...     [core_events.SequentialEvent([core_events.SimpleEvent(1)])]
         ... )
         >>> s.concatenate_by_index(s)
         SimultaneousEvent([SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 1)), SimpleEvent(duration = DirectDuration(duration = 1))])])
         """
         if (self_duration := self.duration) > 0:
             self.extend_until(self_duration)
-        for index, event in enumerate(other.copy()):
+        for index, event in enumerate(other):
             try:
                 ancestor = self[index]
             except IndexError:
                 if self_duration > 0:
-                    event.slide_in(0, core_events.SimpleEvent(self_duration))
+                    # Shallow copy before 'slide_in': We use the same
+                    # events, but we don't want to change the other sequence.
+                    event_new = event.empty_copy()
+                    event_new.extend(event[:])
+                    event = event_new.slide_in(0, core_events.SimpleEvent(self_duration))
                 self.append(event)
             else:
                 self._extend_ancestor(ancestor, event)
 
     @core_utilities.add_copy_option
     def concatenate_by_tag(self, other: SimultaneousEvent) -> SimultaneousEvent:
         """Concatenate with other :class:`~mutwo.core_events.SimultaneousEvent` along their tags.
@@ -935,38 +1069,146 @@
         :type mutate: bool
         :return: Concatenated event.
         :raises core_utilities.NoTagError: If any child event doesn't have a 'tag'
             attribute.
         :raises core_utilities.ConcatenationError: If there are any :class:`SimpleEvent`
             inside a :class:`SimultaneousEvent`.
 
+        **Hint:**
+
+        Similarly to Pythons ``list.extend`` the concatenation simply appends
+        the children of the other event to the sequence without copying them.
+        This means when changing the children in the new event, it also changes
+        the child event in the original sequence. If you want to avoid this,
+        call ``event.copy()`` before concatenating it to the host event.
+
         **Example:**
 
         >>> from mutwo import core_events
         >>> s = core_events.SimultaneousEvent(
         ...      [core_events.TaggedSequentialEvent([core_events.SimpleEvent(1)], tag="test")]
         ...  )
         >>> s.concatenate_by_tag(s)
         SimultaneousEvent([TaggedSequentialEvent([SimpleEvent(duration = DirectDuration(duration = 1)), SimpleEvent(duration = DirectDuration(duration = 1))])])
         """
         if (self_duration := self.duration) > 0:
             self.extend_until(self_duration)
-        for tagged_event in other.copy():
+        for tagged_event in other:
             if not hasattr(tagged_event, "tag"):
                 raise core_utilities.NoTagError(tagged_event)
             tag = tagged_event.tag
             try:
                 ancestor = self[tag]
             except KeyError:
                 if self_duration > 0:
-                    tagged_event.slide_in(0, core_events.SimpleEvent(self_duration))
+                    # Shallow copy before 'slide_in': We use the same
+                    # events, but we don't want to change the other sequence.
+                    event_new = tagged_event.empty_copy()
+                    event_new.extend(tagged_event[:])
+                    tagged_event = event_new.slide_in(0, core_events.SimpleEvent(self_duration))
                 self.append(tagged_event)
             else:
                 self._extend_ancestor(ancestor, tagged_event)
 
+    # NOTE: 'sequentalize' is very generic, it works for all type of child
+    # event structure. This is good, but in it's current form it's mostly
+    # only useful with rather long and complex user defined 'slice_tuple_to_event'
+    # definitions. For instance when sequentializing
+    # SimultaneousEvent[SequentialEvent[SimpleEvent]] the returned event will be
+    # SequentialEvent[SimultaneousEvent[SequentialEvent[SimpleEvent]]]. Here the
+    # inner sequential events are always pointless, since they will always only
+    # contain one simple event.
+    def sequentialize(
+        self,
+        slice_tuple_to_event: typing.Optional[
+            typing.Callable[
+                [tuple[core_parameters.abc.Event, ...]], core_parameters.abc.Event
+            ]
+        ] = None,
+    ) -> core_events.SequentialEvent:
+        """Convert parallel structure to a sequential structure.
+
+        :param slice_tuple_to_event: In order to sequentialize the event
+            `mutwo` splits each child event into small 'event slices'. These
+            'event slices' are simply events created by the `split_at` method.
+            Each of those parallel slice groups need to be bound together to
+            one new event. These new events are sequentially ordered to result
+            in a new sequential structure. The simplest and default way to
+            archive this is by simply putting all event parts into a new
+            :class:`SimultaneousEvent`, so the resulting :class:`SequentialEvent`
+            will be a sequence of `SimultaneousEvent`. This parameter is
+            available so that users can convert her/his parallel structure in
+            meaningful ways (for instance to imitate the ``.chordify``
+            `method from music21 <https://web.mit.edu/music21/doc/usersGuide/usersGuide_09_chordify.html>`
+            which transforms polyphonic music to a chord structure).
+            If ``None`` `slice_tuple_to_event` is set to
+            :class:`SimultaneousEvent`. Default to ``None``.
+        :type slice_tuple_to_event: typing.Optional[typing.Callable[[tuple[core_parameters.abc.Event, ...]], core_parameters.abc.Event]]
+
+        **Example:**
+
+        >>> from mutwo import core_events
+        >>> e = core_events.SimultaneousEvent(
+        ...     [
+        ...         core_events.SequentialEvent(
+        ...             [core_events.SimpleEvent(2), core_events.SimpleEvent(1)]
+        ...         ),
+        ...         core_events.SequentialEvent(
+        ...             [core_events.SimpleEvent(3)]
+        ...         ),
+        ...     ]
+        ... )
+        >>> e.sequentialize()
+        SequentialEvent([SimultaneousEvent([SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 2))]), SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 2))])]), SimultaneousEvent([SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 1))]), SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 1))])])])
+        """
+        if slice_tuple_to_event is None:
+            slice_tuple_to_event = SimultaneousEvent
+
+        # Find all start/end times
+        absolute_time_set = set([])
+        for e in self:
+            try:  # SequentialEvent
+                (
+                    absolute_time_tuple,
+                    duration,
+                ) = e._absolute_time_in_floats_tuple_and_duration
+            except AttributeError:  # SimpleEvent or SimultaneousEvent
+                absolute_time_tuple, duration = (0,), e.duration.duration_in_floats
+            for t in absolute_time_tuple + (duration,):
+                absolute_time_set.add(t)
+
+        # Sort, but also remove the last entry: we don't need
+        # to split at complete duration, because after duration
+        # there isn't any event left in any child.
+        absolute_time_list = sorted(absolute_time_set)[:-1]
+
+        return core_events.SequentialEvent(
+            self._make_event_slice_tuple(absolute_time_list, slice_tuple_to_event)
+        )
+
+    def split_at(
+        self,
+        *absolute_time: core_parameters.abc.Duration,
+        ignore_invalid_split_point: bool = False,
+    ) -> tuple[SimultaneousEvent, ...]:
+        if not absolute_time:
+            raise core_utilities.NoSplitTimeError()
+
+        absolute_time = sorted(absolute_time)
+        self._assert_valid_absolute_time(absolute_time[0])
+        if absolute_time[-1] > self.duration and not ignore_invalid_split_point:
+            raise core_utilities.SplitError(absolute_time[-1])
+
+        def slice_tuple_to_event(slice_tuple):
+            e = self.empty_copy()
+            e[:] = slice_tuple
+            return e
+
+        return self._make_event_slice_tuple(absolute_time, slice_tuple_to_event)
+
 
 @core_utilities.add_tag_to_class
 class TaggedSimpleEvent(SimpleEvent):
     """:class:`SimpleEvent` with tag."""
 
 
 @core_utilities.add_tag_to_class
@@ -977,7 +1219,11 @@
 
 
 @core_utilities.add_tag_to_class
 class TaggedSimultaneousEvent(
     SimultaneousEvent, typing.Generic[T], class_specific_side_attribute_tuple=("tag",)
 ):
     """:class:`SimultaneousEvent` with tag."""
+
+    def sequentialize(self, *args, **kwargs):
+        sequential_event = super().sequentialize(*args, **kwargs)
+        return TaggedSequentialEvent(sequential_event, tag=self.tag)
```

### Comparing `mutwo.core-1.2.3/mutwo/core_events/configurations.py` & `mutwo.core-1.3.0/mutwo/core_events/configurations.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 import functools
 import typing
 
 import quicktions
 
 # We can't set core_converters.UnknownObjectToObject
 # directly because it would raise a circular import error.
-def __unknown_object_to_duration(unknown_object):
+@functools.cache
+def __unknown_object_to_duration():
     from mutwo import core_converters
     from mutwo import core_parameters
 
     return core_converters.UnknownObjectToObject[core_parameters.abc.Duration](
         (
             (
                 (float, int, fractions.Fraction, quicktions.Fraction),
                 core_parameters.DirectDuration,
             ),
         )
-    )(unknown_object)
+    )
 
 
 # We don't define the function with `def UNKNOWN_OBJECT_TO_DURATION`
 # because this is and should look like a global variable and not like
 # a function.
-UNKNOWN_OBJECT_TO_DURATION = __unknown_object_to_duration
+UNKNOWN_OBJECT_TO_DURATION = lambda o: __unknown_object_to_duration()(o)
 """Global definition of callable to parse objects to :class:`mutwo.core_parameters.abc.Duration`.
 
 This function is used in almost all objects which inherit from
 :class:`mutwo.core_events.abc.Event`. It implements syntactic sugar
 so that users can parse buildin types (or other objects) to mutwo callables
 which expect :class:`mutwo.core_parameters.abc.Duration` objects.
 
@@ -78,8 +79,60 @@
 
 DEFAULT_DURATION_TO_WHITE_SPACE = lambda duration: __simpleEvent()(duration)
 """Default conversion for parameter `duration_to_white_space` in
 :func:`mutwo.core_events.abc.ComplexEvent.extend_until`. This simply
 returns a :class:`mutwo.core_events.SimpleEvent` with the given
 duration."""
 
+
+# We can't set core_converters.UnknownObjectToObject
+# directly because it would raise a circular import error.
+@functools.cache
+def __unknown_object_to_tempo_point():
+    from mutwo import core_converters
+    from mutwo import core_parameters
+
+    return core_converters.UnknownObjectToObject[core_parameters.abc.TempoPoint](
+        (
+            (
+                (float, int, fractions.Fraction, quicktions.Fraction),
+                core_parameters.DirectTempoPoint,
+            ),
+        )
+    )
+
+
+# We don't define the function with `def UNKNOWN_OBJECT_TO_DURATION`
+# because this is and should look like a global variable and not like
+# a function.
+UNKNOWN_OBJECT_TO_TEMPO_POINT = lambda o: __unknown_object_to_tempo_point()(o)
+"""Global definition of callable to parse objects to :class:`mutwo.core_parameters.abc.TempoPoint`.
+
+It implements syntactic sugar so that users can parse buildin types
+(or other objects) to mutwo callables which expect
+:class:`mutwo.core_parameters.abc.TempoPoint` objects.
+
+This global variable is the reason why the following
+code prints a :class:`mutwo.core_parameters.DirectTempoPoint`:
+
+    >>> from mutwo import core_events
+    >>> t = core_events.TempoEvent(tempo_point=60, duration=1)
+    >>> t.tempo_point
+    DirectTempoPoint(BPM = 60, reference = 1)
+
+Without this function...
+
+    1. It wouldn't be certain that `tempo_point` returns an instance
+    of :class:`mutwo.core_parameters.abc.TempoPoint`.
+
+    2. Or the code would raise a ``TypeError`` and users would be forced
+    to write:
+
+        >>> core_events.TempoEvent(tempo_point=core_parameters.DirectTempoPoint(60), duration=1)
+
+Because the syntactic sugar partially violates the Python Zen
+"Explicit is better than implicit" this function is publicly defined
+in the `configurations` module (and not in private class methods),
+so that users are encouraged to override the variable if desired.
+"""
+
 del functools, typing
```

### Comparing `mutwo.core-1.2.3/mutwo/core_events/envelopes.py` & `mutwo.core-1.3.0/mutwo/core_events/envelopes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Envelope events"""
 
 from __future__ import annotations
 
 import bisect
 import typing
-import warnings
 
 from scipy import integrate
 
 from mutwo import core_constants
 from mutwo import core_events
 from mutwo import core_parameters
 from mutwo import core_utilities
@@ -344,17 +343,18 @@
         >>> e.value_at(0)
         0
         >>> e.value_at(1)
         2
         >>> e.value_at(0.5)
         1.0
         """
-        absolute_time_in_floats = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(
+        absolute_time = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(
             absolute_time
-        ).duration_in_floats
+        )
+        absolute_time_in_floats = absolute_time.duration_in_floats
 
         (
             absolute_time_in_floats_tuple,
             duration_in_floats,
         ) = self._absolute_time_in_floats_tuple_and_duration
 
         try:
@@ -474,14 +474,16 @@
             raise core_utilities.EmptyEnvelopeError(self, "sample_at")
 
         absolute_time, append_duration = (
             core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
             for unknown_object in (absolute_time, append_duration)
         )
 
+        self._assert_valid_absolute_time(absolute_time)
+
         # We only add a new event in case there isn't any event yet at
         # given point in time.
         if absolute_time not in (absolute_time_tuple := self.absolute_time_tuple):
             envelope_duration = absolute_time_tuple[-1] + self[-1].duration
             event = self._make_event(
                 find_duration(absolute_time, absolute_time_tuple),
                 self.parameter_at(absolute_time),
@@ -544,15 +546,15 @@
         start, end = (
             core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
             for unknown_object in (start, end)
         )
 
         duration = end - start
         if duration == 0:
-            warnings.warn(core_utilities.InvalidAverageValueStartAndEndWarning())
+            self._logger.warn(core_utilities.InvalidAverageValueStartAndEndWarning())
             return self.value_at(start)
         return self.integrate_interval(start, end) / duration.duration
 
     def get_average_parameter(
         self,
         start: typing.Optional[core_constants.DurationType] = None,
         end: typing.Optional[core_constants.DurationType] = None,
@@ -585,14 +587,16 @@
         start: core_parameters.abc.Duration | typing.Any,
         end: core_parameters.abc.Duration | typing.Any,
     ) -> Envelope[T]:
         start, end = (
             core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
             for unknown_object in (start, end)
         )
+        # _assert_correct_start_and_end_values and _assert_valid_absolute_time
+        # is called when super().cut_out is called later.
 
         self.sample_at(start, append_duration=end - start)
         self.sample_at(end)
 
         last_point = self.get_event_at(end)
 
         # In case last_point.duration == 0 "get_event_at" won't return
@@ -616,14 +620,18 @@
         start: core_parameters.abc.Duration | typing.Any,
         end: core_parameters.abc.Duration | typing.Any,
     ) -> Envelope[T]:
         start, end = (
             core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
             for unknown_object in (start, end)
         )
+        self._assert_valid_absolute_time(start)
+        self._assert_correct_start_and_end_values(
+            start, end, condition=lambda start, end: start < end
+        )
 
         if (cut_off_duration := end - start) > 0:
             # It is sufficient to find the first control point
             # by simply using "parameter_at" instead of "sample_at":
             # We don't need an accurate curve_shape or duration,
             # because this point only exists in an infinitely short
             # moment in time anyway (or better: its main function is
@@ -644,25 +652,63 @@
         self,
         duration: core_parameters.abc.Duration,
         duration_to_white_space: typing.Optional[
             typing.Callable[[core_parameters.abc.Duration], core_events.abc.Event]
         ] = None,
         prolong_simple_event: bool = True,
     ) -> Envelope[T]:
-        self_duration = self.duration
-        super().extend_until(
-            duration,
-            duration_to_white_space=duration_to_white_space
-            or (
-                lambda duration: self._make_event(
-                    duration, self.parameter_at(self_duration), 0
-                )
-            ),
-            prolong_simple_event=prolong_simple_event,
-        )
+        if not self:
+            raise core_utilities.EmptyEnvelopeError(self, "extend_until")
+        self.sample_at(duration)
+
+    def split_at(
+        self,
+        *absolute_time: core_parameters.abc.Duration,
+        ignore_invalid_split_point: bool = False,
+    ) -> tuple[Envelope, ...]:
+        if not absolute_time:
+            raise core_utilities.NoSplitTimeError()
+
+        absolute_time = sorted(absolute_time)
+        if absolute_time[-1] > self.duration and not ignore_invalid_split_point:
+            raise core_utilities.SplitError(absolute_time[-1])
+
+        # We copy, because the 'sample_at' calls would change our envelope.
+        self = self.copy()
+
+        for t in absolute_time:
+            self.sample_at(t)
+
+        def add(s, value):
+            s.append(s._make_event(0, s.value_to_parameter(value), 0))
+
+        segment_tuple = super().split_at(
+            *absolute_time, ignore_invalid_split_point=ignore_invalid_split_point
+        )
+
+        # We already added the interpolation points with 'self.sample_at(*t)',
+        # but they are always only available in the segments after the split
+        # point (because for each segment the start is included, but the end
+        # duration isn't included anymore). So we need to add them to the
+        # segments before the split points, otherwise 'value_at' returns wrong
+        # values.
+        for segment0, segment1 in zip(segment_tuple, segment_tuple[1:]):
+            add(segment0, segment1.value_at(0))
+
+        if segment_tuple:
+            s = segment_tuple[-1]
+            v = self.value_at(self.duration)
+            # Only add control point, if it isn't present
+            # yet anyway (minimal changes).
+            # This condition is 'true' if we only split at
+            # start time ('env.split_at(0)').
+            if s.value_at(s.duration) != v:
+                add(s, v)
+
+        return segment_tuple
 
 
 class RelativeEnvelope(Envelope, typing.Generic[T]):
     __parent_doc_string = Envelope.__doc__.split("\n")[2:]  # type: ignore
     __after_parameter_text_index = __parent_doc_string.index("")
     __doc__ = "\n".join(
         ["Envelope with relative durations and values / parameters.\n"]
@@ -773,14 +819,21 @@
         ] = None,
         parameter_to_value: typing.Optional[
             typing.Callable[[core_constants.ParameterType], core_events.Envelope.Value]
         ] = None,
         apply_parameter_on_event: typing.Optional[
             typing.Callable[[core_events.abc.Event, core_constants.ParameterType], None]
         ] = None,
+        default_event_class: type[core_events.abc.Event] = core_events.TempoEvent,
+        initialise_default_event_class: typing.Callable[
+            [type[core_events.abc.Event], core_constants.DurationType],
+            core_events.abc.Event,
+        ] = lambda simple_event_class, duration: simple_event_class(
+            tempo_point=1, duration=duration
+        ),
         **kwargs,
     ):
         def default_event_to_parameter(event: core_events.abc.Event) -> TempoPoint:
             return getattr(
                 event,
                 core_events.configurations.DEFAULT_TEMPO_ENVELOPE_PARAMETER_NAME,
             )
@@ -810,14 +863,16 @@
         super().__init__(
             *args,
             event_to_parameter=event_to_parameter or default_event_to_parameter,
             value_to_parameter=value_to_parameter or default_value_to_parameter,
             parameter_to_value=parameter_to_value or default_parameter_to_value,
             apply_parameter_on_event=apply_parameter_on_event
             or default_apply_parameter_on_event,
+            default_event_class=default_event_class,
+            initialise_default_event_class=initialise_default_event_class,
             **kwargs,
         )
 
     def __eq__(self, other: typing.Any):
         # TempoEnvelope can't use the default '__eq__' method inherited
         # from list, because this would create endless recursion
         # (because every event has a TempoEnvelope, so Python would forever
```

### Comparing `mutwo.core-1.2.3/mutwo/core_generators/__init__.py` & `mutwo.core-1.3.0/mutwo/core_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `mutwo.core-1.2.3/mutwo/core_generators/generic.py` & `mutwo.core-1.3.0/mutwo/core_generators/generic.py`

 * *Files identical despite different names*

### Comparing `mutwo.core-1.2.3/mutwo/core_parameters/abc.py` & `mutwo.core-1.3.0/mutwo/core_parameters/abc.py`

 * *Files identical despite different names*

### Comparing `mutwo.core-1.2.3/mutwo/core_parameters/configurations.py` & `mutwo.core-1.3.0/mutwo/core_parameters/configurations.py`

 * *Files identical despite different names*

### Comparing `mutwo.core-1.2.3/mutwo/core_parameters/constants.py` & `mutwo.core-1.3.0/mutwo/core_parameters/constants.py`

 * *Files identical despite different names*

### Comparing `mutwo.core-1.2.3/mutwo/core_parameters/durations.py` & `mutwo.core-1.3.0/mutwo/core_parameters/durations.py`

 * *Files identical despite different names*

### Comparing `mutwo.core-1.2.3/mutwo/core_parameters/tempos.py` & `mutwo.core-1.3.0/mutwo/core_parameters/tempos.py`

 * *Files identical despite different names*

### Comparing `mutwo.core-1.2.3/mutwo/core_utilities/decorators.py` & `mutwo.core-1.3.0/mutwo/core_utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `mutwo.core-1.2.3/mutwo/core_utilities/exceptions.py` & `mutwo.core-1.3.0/mutwo/core_utilities/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,19 +19,22 @@
     "InvalidCutOutStartAndEndValuesError",
     "SplitUnavailableChildError",
     "NoSolutionFoundError",
     "EmptyEnvelopeError",
     "UndefinedReferenceWarning",
     "ConcatenationError",
     "NoTagError",
+    "SplitError",
+    "InvalidAbsoluteTime",
+    "NoSplitTimeError",
 )
 
 
 class CannotSetDurationOfEmptyComplexEvent(Exception):
-    def __init__(self, cls):
+    def __init__(self):
         super().__init__(
             "You tried to set the duration of a complex "
             "event (e.g. 'SequentialEvent' or 'SimultaneousEvent') "
             "which doesn't have any child events. This"
             " is impossible, because the duration of a 'ComplexEvent'"
             " is simply the sum of its sequentially ordered child events."
         )
@@ -132,14 +135,19 @@
         super().__init__(
             f"Can't cut out SimpleEvent '{simple_event}' with "
             f"duration '{duration}' from"
             f" (start = {start} to end = {end})."
         )
 
 
+class SplitError(Exception):
+    def __init__(self, absolute_time: core_constants.DurationType):
+        super().__init__(f"Can't split event at absolute time '{absolute_time}'.")
+
+
 class SplitUnavailableChildError(Exception):
     def __init__(self, absolute_time: core_constants.DurationType):
         super().__init__(
             f"Can't split child at absolute time '{absolute_time}'. There is no child"
             " event available at the requested time."
         )
 
@@ -180,7 +188,21 @@
         super().__init__(
             "It's not possible to concatenate an event "
             "with the 'concatenate_by_tag' method if not "
             "all child events have tags. Here 'mutwo' detected the "
             f"child event '{str(event_without_tag)[:50]}...' "
             "which doesn't have any 'tag' attribute."
         )
+
+
+class InvalidAbsoluteTime(Exception):
+    def __init__(self, t):
+        super().__init__(
+            f"Duration '{t}' is smaller than 0 and can therefore not "
+            "represent an absolute time. The absolute time line starts "
+            "from 0 until +inf and therefore the smallest absolute time is 0."
+        )
+
+
+class NoSplitTimeError(Exception):
+    def __init__(self):
+        super().__init__("Nothing to split (no split time given)!")
```

### Comparing `mutwo.core-1.2.3/mutwo/core_utilities/tests.py` & `mutwo.core-1.3.0/mutwo/core_utilities/tests.py`

 * *Files identical despite different names*

### Comparing `mutwo.core-1.2.3/mutwo/core_utilities/tools.py` & `mutwo.core-1.3.0/mutwo/core_utilities/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Generic utility functions."""
 
 import bisect
 import copy
 import functools
 import itertools
-import operator
+import logging
 import math
+import operator
 import types
 import typing
 
+from mutwo import core_configurations
 from mutwo import core_constants
 
 
 __all__ = (
     "scale",
     "scale_sequence_to_sum",
     "accumulate_from_n",
@@ -26,14 +28,15 @@
     "set_nested_item_from_index_sequence",
     "find_numbers_which_sums_up_to",
     "call_function_except_attribute_error",
     "round_floats",
     "camel_case_to_snake_case",
     "test_if_objects_are_equal_by_parameter_tuple",
     "get_all",
+    "get_cls_logger",
 )
 
 
 def scale(
     value: core_constants.Real,
     old_min: core_constants.Real,
     old_max: core_constants.Real,
@@ -542,7 +545,28 @@
     """
     return functools.reduce(
         operator.add,
         map(
             lambda submodule: getattr(submodule, "__all__", tuple([])), submodule_tuple
         ),
     )
+
+
+def get_cls_logger(
+    cls: typing.Type, level: typing.Optional[int] = None
+) -> logging.Logger:
+    """Get the local logger of your class.
+
+    :param cls: The class for which the logger should be returned. Simply call
+        `type(o)` if you only have the instance.
+    :type cls: typing.Type
+    :param level: The logging level of the logger. If ``None`` the level
+        defined in `mutwo.core_configurations.LOGGING_LEVEL` is used. Default
+        to ``None``.
+    :type level: int
+    :return: A :class:`logging.Logger`.
+    """
+    if level is None:
+        level = core_configurations.LOGGING_LEVEL
+    logger = logging.getLogger(f"{cls.__module__}.{cls.__name__}")
+    logger.setLevel(level)
+    return logger
```

### Comparing `mutwo.core-1.2.3/mutwo.core.egg-info/PKG-INFO` & `mutwo.core-1.3.0/mutwo.core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutwo.core
-Version: 1.2.3
+Version: 1.3.0
 Summary: core library for event based framework mutwo
 Home-page: https://github.com/mutwo-org/mutwo
 Author: Tim Pauli, Levin Eric Zimmermann
 Author-email: tim.pauli@folkwang-uni.de, levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mutwo.core-1.2.3/mutwo.core.egg-info/SOURCES.txt` & `mutwo.core-1.3.0/mutwo.core.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 pyproject.toml
 setup.py
 mutwo.core.egg-info/PKG-INFO
 mutwo.core.egg-info/SOURCES.txt
 mutwo.core.egg-info/dependency_links.txt
 mutwo.core.egg-info/requires.txt
 mutwo.core.egg-info/top_level.txt
+mutwo/core_configurations/__init__.py
 mutwo/core_constants/__init__.py
 mutwo/core_converters/__init__.py
 mutwo/core_converters/abc.py
 mutwo/core_converters/configurations.py
 mutwo/core_converters/parsers.py
 mutwo/core_converters/tempos.py
 mutwo/core_events/__init__.py
 mutwo/core_events/abc.py
 mutwo/core_events/basic.py
 mutwo/core_events/configurations.py
 mutwo/core_events/envelopes.py
+mutwo/core_events/tempos.py
 mutwo/core_generators/__init__.py
 mutwo/core_generators/generic.py
 mutwo/core_parameters/__init__.py
 mutwo/core_parameters/abc.py
 mutwo/core_parameters/configurations.py
 mutwo/core_parameters/constants.py
 mutwo/core_parameters/durations.py
```

### Comparing `mutwo.core-1.2.3/setup.py` & `mutwo.core-1.3.0/setup.py`

 * *Files identical despite different names*

