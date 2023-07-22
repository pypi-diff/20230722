# Comparing `tmp/elias-0.2.7.tar.gz` & `tmp/elias-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/Projects/elias/dist/.tmp-0dxmdpgg/elias-0.2.7.tar", last modified: Wed Jul  5 09:30:07 2023, max compression
+gzip compressed data, was "/mnt/d/Projects/elias/dist/.tmp-6y2w3wi1/elias-0.2.9.tar", last modified: Sat Jul 22 12:46:38 2023, max compression
```

## Comparing `elias-0.2.7.tar` & `elias-0.2.9.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-05 09:30:07.519194 elias-0.2.7/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.7/LICENSE
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-07-05 09:30:07.519194 elias-0.2.7/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1736 2022-04-27 09:37:39.000000 elias-0.2.7/README.md
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      110 2022-04-27 09:37:39.000000 elias-0.2.7/pyproject.toml
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      707 2023-07-05 09:30:07.529264 elias-0.2.7/setup.cfg
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       98 2022-04-27 09:37:39.000000 elias-0.2.7/setup.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-05 09:30:05.821378 elias-0.2.7/src/
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-05 09:30:05.984124 elias-0.2.7/src/elias/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.7/src/elias/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    24491 2023-07-05 09:24:37.000000 elias-0.2.7/src/elias/config.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-05 09:30:06.364177 elias-0.2.7/src/elias/data/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.7/src/elias/data/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8439 2022-04-27 09:37:39.000000 elias-0.2.7/src/elias/data/combined.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4507 2022-04-27 09:37:39.000000 elias-0.2.7/src/elias/data/loader.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4987 2022-04-27 09:37:39.000000 elias-0.2.7/src/elias/data/sampling.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1047 2022-04-27 09:37:39.000000 elias-0.2.7/src/elias/data/stop_criterion.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-05 09:30:06.659326 elias-0.2.7/src/elias/folder/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      156 2022-04-27 09:37:39.000000 elias-0.2.7/src/elias/folder/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1355 2022-04-27 09:37:39.000000 elias-0.2.7/src/elias/folder/analysis.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8126 2022-05-13 11:41:20.000000 elias-0.2.7/src/elias/folder/data.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13271 2022-12-23 10:38:59.000000 elias-0.2.7/src/elias/folder/folder.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1491 2022-12-23 10:15:28.000000 elias-0.2.7/src/elias/folder/model.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4983 2023-05-29 14:26:02.000000 elias-0.2.7/src/elias/folder/run.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-05 09:30:07.013561 elias-0.2.7/src/elias/manager/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      294 2022-04-27 09:37:39.000000 elias-0.2.7/src/elias/manager/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2705 2022-04-27 09:37:39.000000 elias-0.2.7/src/elias/manager/analysis.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1594 2022-04-27 09:37:39.000000 elias-0.2.7/src/elias/manager/artifact.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    12045 2022-04-27 09:37:39.000000 elias-0.2.7/src/elias/manager/buffered.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13104 2022-10-23 15:43:10.000000 elias-0.2.7/src/elias/manager/data.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    22291 2022-12-23 10:55:00.000000 elias-0.2.7/src/elias/manager/model.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2918 2023-05-29 14:22:02.000000 elias-0.2.7/src/elias/manager/run.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-05 09:30:07.477496 elias-0.2.7/src/elias/util/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      361 2022-06-24 14:37:22.000000 elias-0.2.7/src/elias/util/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6870 2023-04-28 12:57:24.000000 elias-0.2.7/src/elias/util/fs.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     7919 2022-06-24 13:43:08.000000 elias-0.2.7/src/elias/util/io.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      333 2023-06-21 14:23:03.000000 elias-0.2.7/src/elias/util/random.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4690 2023-03-21 10:20:42.000000 elias-0.2.7/src/elias/util/range.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1248 2022-10-24 10:11:39.000000 elias-0.2.7/src/elias/util/timing.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1218 2023-07-04 15:24:59.000000 elias-0.2.7/src/elias/util/typing.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5512 2022-05-11 08:27:09.000000 elias-0.2.7/src/elias/util/version.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-05 09:30:06.128363 elias-0.2.7/src/elias.egg-info/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-07-05 09:30:05.000000 elias-0.2.7/src/elias.egg-info/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      948 2023-07-05 09:30:05.000000 elias-0.2.7/src/elias.egg-info/SOURCES.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-07-05 09:30:05.000000 elias-0.2.7/src/elias.egg-info/dependency_links.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      100 2023-07-05 09:30:05.000000 elias-0.2.7/src/elias.egg-info/requires.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        6 2023-07-05 09:30:05.000000 elias-0.2.7/src/elias.egg-info/top_level.txt
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-22 12:46:38.215965 elias-0.2.9/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.9/LICENSE
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-07-22 12:46:38.215965 elias-0.2.9/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1736 2022-04-27 09:37:39.000000 elias-0.2.9/README.md
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      110 2022-04-27 09:37:39.000000 elias-0.2.9/pyproject.toml
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      729 2023-07-22 12:46:38.223196 elias-0.2.9/setup.cfg
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       98 2022-04-27 09:37:39.000000 elias-0.2.9/setup.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-22 12:46:36.681436 elias-0.2.9/src/
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-22 12:46:36.875149 elias-0.2.9/src/elias/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.9/src/elias/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    25208 2023-07-21 13:42:03.000000 elias-0.2.9/src/elias/config.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-22 12:46:37.256555 elias-0.2.9/src/elias/data/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.9/src/elias/data/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8439 2022-04-27 09:37:39.000000 elias-0.2.9/src/elias/data/combined.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4507 2022-04-27 09:37:39.000000 elias-0.2.9/src/elias/data/loader.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4987 2022-04-27 09:37:39.000000 elias-0.2.9/src/elias/data/sampling.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1047 2022-04-27 09:37:39.000000 elias-0.2.9/src/elias/data/stop_criterion.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-22 12:46:37.497125 elias-0.2.9/src/elias/folder/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      156 2022-04-27 09:37:39.000000 elias-0.2.9/src/elias/folder/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1355 2022-04-27 09:37:39.000000 elias-0.2.9/src/elias/folder/analysis.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8126 2022-05-13 11:41:20.000000 elias-0.2.9/src/elias/folder/data.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13271 2022-12-23 10:38:59.000000 elias-0.2.9/src/elias/folder/folder.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1491 2022-12-23 10:15:28.000000 elias-0.2.9/src/elias/folder/model.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4983 2023-05-29 14:26:02.000000 elias-0.2.9/src/elias/folder/run.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-22 12:46:37.794513 elias-0.2.9/src/elias/manager/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      294 2022-04-27 09:37:39.000000 elias-0.2.9/src/elias/manager/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2705 2022-04-27 09:37:39.000000 elias-0.2.9/src/elias/manager/analysis.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1594 2022-04-27 09:37:39.000000 elias-0.2.9/src/elias/manager/artifact.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    12045 2022-04-27 09:37:39.000000 elias-0.2.9/src/elias/manager/buffered.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13104 2022-10-23 15:43:10.000000 elias-0.2.9/src/elias/manager/data.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    23482 2023-07-22 00:14:10.000000 elias-0.2.9/src/elias/manager/model.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2918 2023-05-29 14:22:02.000000 elias-0.2.9/src/elias/manager/run.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-22 12:46:38.181143 elias-0.2.9/src/elias/util/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      361 2022-06-24 14:37:22.000000 elias-0.2.9/src/elias/util/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6870 2023-04-28 12:57:24.000000 elias-0.2.9/src/elias/util/fs.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     9994 2023-07-19 17:19:47.000000 elias-0.2.9/src/elias/util/io.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      333 2023-06-21 14:23:03.000000 elias-0.2.9/src/elias/util/random.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4690 2023-03-21 10:20:42.000000 elias-0.2.9/src/elias/util/range.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1248 2022-10-24 10:11:39.000000 elias-0.2.9/src/elias/util/timing.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1218 2023-07-04 15:24:59.000000 elias-0.2.9/src/elias/util/typing.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5512 2022-05-11 08:27:09.000000 elias-0.2.9/src/elias/util/version.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3055 2023-07-22 12:32:06.000000 elias-0.2.9/src/elias/util/wandb_images.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-07-22 12:46:37.050645 elias-0.2.9/src/elias.egg-info/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-07-22 12:46:36.000000 elias-0.2.9/src/elias.egg-info/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      979 2023-07-22 12:46:36.000000 elias-0.2.9/src/elias.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-07-22 12:46:36.000000 elias-0.2.9/src/elias.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      122 2023-07-22 12:46:36.000000 elias-0.2.9/src/elias.egg-info/requires.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        6 2023-07-22 12:46:36.000000 elias-0.2.9/src/elias.egg-info/top_level.txt
```

### Comparing `elias-0.2.7/PKG-INFO` & `elias-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elias
-Version: 0.2.7
+Version: 0.2.9
 Summary: ELIAS experiment library for facilitating machine learning projects
 Home-page: https://github.com/tobias-kirschstein/elias
 Author: Tobias Kirschstein
 Author-email: tobias.kirschstein@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `elias-0.2.7/README.md` & `elias-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias/config.py` & `elias-0.2.9/src/elias/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import inspect
 from abc import ABC, abstractmethod
-from dataclasses import dataclass, asdict, fields, field
+from collections import defaultdict
+from dataclasses import dataclass, asdict, fields, field, replace, is_dataclass
 from enum import Enum, EnumMeta, auto
 from importlib import import_module
 from pydoc import locate
 from typing import List, Tuple, Any, Type, get_type_hints, Generic, TypeVar, Dict, Iterator, Callable, Optional
 
 import dacite
 import numpy as np
@@ -158,15 +159,30 @@
         are represented by their intrinsic value instead. When deserializing the stored JSON with :meth:`from_json`
         the enum values can be parsed into proper enums again thanks to the type annotation in the underlying dataclass.
 
         Returns
         -------
             a Python dictionary representing this dataclass
         """
-        return asdict(self, dict_factory=self._serialize_enums_and_numpy)
+
+        config = replace(self)
+
+        # Python's asdict() cannot deal with defaultdict instances "TypeError: first argument must be callable or None"
+        # Hence, we silently replace defaultdicts with regular dicts here
+        def _cast_defaultdict_rec(inner_config: Config):
+            for field in fields(inner_config):
+                value = getattr(inner_config, field.name)
+                if isinstance(value, defaultdict):
+                    setattr(inner_config, field.name, dict(value))
+                elif is_dataclass(value):
+                    _cast_defaultdict_rec(value)
+
+        _cast_defaultdict_rec(config)
+
+        return asdict(config, dict_factory=config._serialize_enums_and_numpy)
 
     def __post_init__(self):
         """
         Overrides the post initialization hook of Python's dataclasses.
         This default implementation scans for fields in the dataclass that have an enum type hint.
         Any of these attributes that are not proper enums of their type will then be automatically instantiated.
         This comes handy when initializing a Config from command line values as these are often only strings hinting
```

### Comparing `elias-0.2.7/src/elias/data/combined.py` & `elias-0.2.9/src/elias/data/combined.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias/data/loader.py` & `elias-0.2.9/src/elias/data/loader.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias/data/sampling.py` & `elias-0.2.9/src/elias/data/sampling.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias/data/stop_criterion.py` & `elias-0.2.9/src/elias/data/stop_criterion.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias/folder/analysis.py` & `elias-0.2.9/src/elias/folder/analysis.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias/folder/data.py` & `elias-0.2.9/src/elias/folder/data.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias/folder/folder.py` & `elias-0.2.9/src/elias/folder/folder.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias/folder/model.py` & `elias-0.2.9/src/elias/folder/model.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias/folder/run.py` & `elias-0.2.9/src/elias/folder/run.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias/manager/analysis.py` & `elias-0.2.9/src/elias/manager/analysis.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias/manager/artifact.py` & `elias-0.2.9/src/elias/manager/artifact.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias/manager/buffered.py` & `elias-0.2.9/src/elias/manager/buffered.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias/manager/data.py` & `elias-0.2.9/src/elias/manager/data.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias/manager/model.py` & `elias-0.2.9/src/elias/manager/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,23 +183,35 @@
         """
 
         try:
             if localize_via_run_name:
                 new_model_manager = cls(run_name)
             else:
                 new_model_manager = cls(model_store_path, run_name)
-        except TypeError:
+        except TypeError as e:
             raise NotImplementedError(f"Could not construct model manager {cls} with location and run name parameter. "
-                                      f"Please override from_location() to match the class __init__() method")
+                                      f"Please override from_location() to match the class __init__() method"
+                                      f"Other possible error: {e}")
         return new_model_manager
 
     # -------------------------------------------------------------------------
     # Building/Storing/Loading Models
     # -------------------------------------------------------------------------
 
+    def get_checkpoint_path(self, checkpoint_name_or_id: Union[str, int]):
+        assert self._checkpoint_name_format is not None, "Cannot get checkpoint path, no file name format specified"
+
+        checkpoint_id = self._resolve_checkpoint_id(checkpoint_name_or_id)
+        self._checkpoints_folder.substitute(self._checkpoint_name_format, checkpoint_id)
+        checkpoint_file_name = self._checkpoints_folder.get_file_name_by_numbering(self._checkpoint_name_format,
+                                                                                   checkpoint_id)
+
+        checkpoint_path = f"{self._checkpoints_folder.get_location()}/{checkpoint_file_name}"
+        return checkpoint_path
+
     def list_checkpoints(self) -> List[str]:
         assert self._checkpoint_name_format is not None, "Cannot list checkpoints, no file name format specified"
 
         checkpoint_ids_and_names = self._checkpoints_folder.list_file_numbering(self._checkpoint_name_format)
         if len(checkpoint_ids_and_names) == 0:
             return []
 
@@ -214,38 +226,41 @@
             checkpoint_names = checkpoint_names[last_neg_id + 1:] + checkpoint_names[:last_neg_id + 1]
 
         return checkpoint_names
 
     def list_checkpoint_ids(self) -> List[int]:
         assert self._checkpoint_name_format is not None, "Cannot list checkpoints, no file name format specified"
 
-        checkpoint_ids = self._checkpoints_folder.list_file_numbering(self._checkpoint_name_format, return_only_numbering=True)
+        checkpoint_ids = self._checkpoints_folder.list_file_numbering(self._checkpoint_name_format,
+                                                                      return_only_numbering=True)
         last_neg_id = None
         for idx, checkpoint_id in enumerate(checkpoint_ids):
             if checkpoint_id < 0:
                 last_neg_id = idx
 
         if last_neg_id is not None:
             checkpoint_ids = checkpoint_ids[last_neg_id + 1:] + checkpoint_ids[:last_neg_id + 1]
 
         return checkpoint_ids
 
     def store_checkpoint(self, model: _ModelType, checkpoint_name_or_id: Union[str, int], **kwargs):
         if isinstance(checkpoint_name_or_id, int):
             assert self._checkpoint_name_format is not None, \
                 f"Cannot store checkpoint with id {checkpoint_name_or_id} since no checkpoint name format was specified"
-            checkpoint_file_name = self._checkpoints_folder.substitute(self._checkpoint_name_format, checkpoint_name_or_id)
+            checkpoint_file_name = self._checkpoints_folder.substitute(self._checkpoint_name_format,
+                                                                       checkpoint_name_or_id)
         else:
             checkpoint_file_name = checkpoint_name_or_id
 
         self._store_checkpoint(model, checkpoint_file_name, **kwargs)
 
     def load_checkpoint(self, checkpoint_name_or_id: Union[str, int], **kwargs) -> _ModelType:
         checkpoint_id = self._resolve_checkpoint_id(checkpoint_name_or_id)
-        checkpoint_file_name = self._checkpoints_folder.get_file_name_by_numbering(self._checkpoint_name_format, checkpoint_id)
+        checkpoint_file_name = self._checkpoints_folder.get_file_name_by_numbering(self._checkpoint_name_format,
+                                                                                   checkpoint_id)
 
         return self._load_checkpoint(checkpoint_file_name, **kwargs)
 
     def delete_checkpoint(self, checkpoint_name_or_id: Union[str, int]):
         checkpoint_id = self._resolve_checkpoint_id(checkpoint_name_or_id)
         checkpoint_file_name = self._checkpoints_folder.get_file_name_by_numbering(self._checkpoint_name_format,
                                                                                    checkpoint_id)
@@ -403,14 +418,17 @@
     # -------------------------------------------------------------------------
     # Getters
     # -------------------------------------------------------------------------
 
     def get_run_name(self) -> str:
         return self._run_name
 
+    def get_location(self) -> str:
+        return self._folder.get_location()
+
     def get_model_store_path(self) -> str:
         return self._folder.get_location()
 
     # -------------------------------------------------------------------------
     # Helper Methods
     # -------------------------------------------------------------------------
 
@@ -428,23 +446,25 @@
             assert self._checkpoint_name_format is not None, \
                 "Cannot resolve checkpoint by id, no file name format specified"
             if checkpoint_name_or_id < 0:
                 # Find latest checkpoint
                 assert checkpoint_name_or_id == -1, \
                     f"Only -1 is allowed as negative checkpoint id, got `{checkpoint_name_or_id}`"
 
-                checkpoint_ids, checkpoint_names = zip(*self._checkpoints_folder.list_file_numbering(self._checkpoint_name_format))
+                checkpoint_ids, checkpoint_names = zip(
+                    *self._checkpoints_folder.list_file_numbering(self._checkpoint_name_format))
                 if -1 in checkpoint_ids:
                     checkpoint_id = -1
                 else:
                     # No checkpoint with id -1 present => Take checkpoint with largest ID instead
                     assert len(checkpoint_ids) > 0, \
                         f"Cannot find latest checkpoint, no checkpoints found in {self._checkpoints_folder.get_location()}"
                     checkpoint_id = checkpoint_ids[-1]
             else:
                 # Find corresponding name for checkpoint id
                 checkpoint_id = checkpoint_name_or_id
 
             return checkpoint_id
         else:
-            checkpoint_id = self._checkpoints_folder.get_numbering_by_file_name(self._checkpoint_name_format, checkpoint_name_or_id)
+            checkpoint_id = self._checkpoints_folder.get_numbering_by_file_name(self._checkpoint_name_format,
+                                                                                checkpoint_name_or_id)
             return checkpoint_id
```

### Comparing `elias-0.2.7/src/elias/manager/run.py` & `elias-0.2.9/src/elias/manager/run.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias/util/fs.py` & `elias-0.2.9/src/elias/util/fs.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias/util/io.py` & `elias-0.2.9/src/elias/util/io.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,16 +5,19 @@
     - pickled Python objects (+gzip)
 """
 
 import gzip
 import json
 import pickle
 from pathlib import Path
-from typing import Union
+from typing import Union, Tuple, Literal
 
+import PIL.Image
+import cv2
+import imageio
 import numpy as np
 import yaml
 from PIL import Image
 
 from elias.util.fs import ensure_file_ending, ensure_directory_exists_for_file
 
 PathType = Union[str, Path]
@@ -243,19 +246,74 @@
 # =========================================================================
 # Images
 # =========================================================================
 
 def save_img(img: np.ndarray, path: PathType):
     ensure_directory_exists_for_file(path)
 
-    if img.dtype == np.float32:
-        # If float array was passed, have to transform [0.0, 1.0] -> [0, ..., 255)
-        assert 0 <= img.min() and img.max() <= 1, \
-            "passed float array should have values between 0 and 1 to be interpreted as image"
-        img = (img * 255).astype(np.uint8)
+    if Path(path).suffix == '.exr':
+        imageio.imwrite(path, img)
+    else:
+        if img.dtype == np.float32:
+            # TODO: Do we really want to quantize without asking?
+            # If float array was passed, have to transform [0.0, 1.0] -> [0, ..., 255)
+            assert 0 <= img.min() and img.max() <= 1, \
+                "passed float array should have values between 0 and 1 to be interpreted as image"
+            img = (img * 255).astype(np.uint8)
 
-    Image.fromarray(img).save(path)
+        Image.fromarray(img).save(path)
 
 
 def load_img(path: PathType) -> np.ndarray:
-    img = Image.open(path)
+    if Path(path).suffix == '.exr':
+        img = imageio.imread_v2(path)
+    else:
+        img = Image.open(path)
+
     return np.asarray(img)
+
+
+InterpolationType = Literal['nearest', 'bilinear', 'bicubic', 'lanczos']
+
+
+def resize_img(img: np.ndarray,
+               scale: Union[float, Tuple[float, float]],
+               interpolation: InterpolationType = 'bilinear',
+               use_opencv: bool = False) -> np.ndarray:
+    try:
+        iter(scale)
+    except TypeError:
+        scale_x = scale
+        scale_y = scale
+    else:
+        scale_x, scale_y = scale
+
+    if use_opencv:
+        if interpolation == 'nearest':
+            interpolation = cv2.INTER_NEAREST
+        elif interpolation == 'bilinear':
+            interpolation = cv2.INTER_LINEAR
+        elif interpolation == 'bicubic':
+            interpolation = cv2.INTER_CUBIC
+        elif interpolation == 'lanczos':
+            interpolation = cv2.INTER_LANCZOS4
+        else:
+            raise ValueError(f"Invalid interpolation type: {interpolation}")
+
+        img = cv2.resize(img, (int(img.shape[1] * scale_x), int(img.shape[0] * scale_y)), interpolation=interpolation)
+    else:
+        if interpolation == 'nearest':
+            interpolation = PIL.Image.Resampling.NEAREST
+        elif interpolation == 'bilinear':
+            interpolation = PIL.Image.Resampling.BILINEAR
+        elif interpolation == 'bicubic':
+            interpolation = PIL.Image.Resampling.BICUBIC
+        elif interpolation == 'lanczos':
+            interpolation = PIL.Image.Resampling.LANCZOS
+        else:
+            raise ValueError(f"Invalid interpolation type: {interpolation}")
+
+        img_pil = Image.fromarray(img)
+        img_pil = img_pil.resize((int(img.shape[1] * scale_x), int(img.shape[0] * scale_y)), resample=interpolation)
+        img = np.array(img_pil)
+
+    return img
```

### Comparing `elias-0.2.7/src/elias/util/range.py` & `elias-0.2.9/src/elias/util/range.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias/util/timing.py` & `elias-0.2.9/src/elias/util/timing.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias/util/typing.py` & `elias-0.2.9/src/elias/util/typing.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias/util/version.py` & `elias-0.2.9/src/elias/util/version.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.7/src/elias.egg-info/PKG-INFO` & `elias-0.2.9/src/elias.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elias
-Version: 0.2.7
+Version: 0.2.9
 Summary: ELIAS experiment library for facilitating machine learning projects
 Home-page: https://github.com/tobias-kirschstein/elias
 Author: Tobias Kirschstein
 Author-email: tobias.kirschstein@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `elias-0.2.7/src/elias.egg-info/SOURCES.txt` & `elias-0.2.9/src/elias.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -31,8 +31,9 @@
 src/elias/util/__init__.py
 src/elias/util/fs.py
 src/elias/util/io.py
 src/elias/util/random.py
 src/elias/util/range.py
 src/elias/util/timing.py
 src/elias/util/typing.py
-src/elias/util/version.py
+src/elias/util/version.py
+src/elias/util/wandb_images.py
```

