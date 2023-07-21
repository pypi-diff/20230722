# Comparing `tmp/pyopensprinkler-0.7.6.tar.gz` & `tmp/pyopensprinkler-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyopensprinkler-0.7.6.tar", last modified: Sat Feb 25 21:01:54 2023, max compression
+gzip compressed data, was "dist/pyopensprinkler-0.7.7.tar", last modified: Fri Jul 21 22:13:13 2023, max compression
```

## Comparing `pyopensprinkler-0.7.6.tar` & `pyopensprinkler-0.7.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2023-02-25 21:01:54.060000 pyopensprinkler-0.7.6/
--rw-r--r--   0 vincent   (1000) vincent   (1000)      475 2023-02-25 21:01:54.060000 pyopensprinkler-0.7.6/PKG-INFO
--rw-r--r--   0 vincent   (1000) vincent   (1000)     2135 2020-10-16 22:21:30.000000 pyopensprinkler-0.7.6/README.md
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2023-02-25 21:01:54.060000 pyopensprinkler-0.7.6/pyopensprinkler/
--rw-r--r--   0 vincent   (1000) vincent   (1000)    29175 2022-06-01 21:56:41.000000 pyopensprinkler-0.7.6/pyopensprinkler/__init__.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)     1504 2020-07-04 11:32:57.000000 pyopensprinkler-0.7.6/pyopensprinkler/const.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)     7134 2021-02-27 01:28:46.000000 pyopensprinkler-0.7.6/pyopensprinkler/program.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)     8743 2021-02-27 01:28:46.000000 pyopensprinkler-0.7.6/pyopensprinkler/station.py
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2023-02-25 21:01:54.060000 pyopensprinkler-0.7.6/pyopensprinkler.egg-info/
--rw-rw-rw-   0 vincent   (1000) vincent   (1000)      475 2023-02-25 21:01:53.000000 pyopensprinkler-0.7.6/pyopensprinkler.egg-info/PKG-INFO
--rw-rw-rw-   0 vincent   (1000) vincent   (1000)      329 2023-02-25 21:01:53.000000 pyopensprinkler-0.7.6/pyopensprinkler.egg-info/SOURCES.txt
--rw-rw-rw-   0 vincent   (1000) vincent   (1000)        1 2023-02-25 21:01:53.000000 pyopensprinkler-0.7.6/pyopensprinkler.egg-info/dependency_links.txt
--rw-rw-rw-   0 vincent   (1000) vincent   (1000)       30 2023-02-25 21:01:53.000000 pyopensprinkler-0.7.6/pyopensprinkler.egg-info/requires.txt
--rw-rw-rw-   0 vincent   (1000) vincent   (1000)       16 2023-02-25 21:01:53.000000 pyopensprinkler-0.7.6/pyopensprinkler.egg-info/top_level.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)      154 2023-02-25 21:01:54.060000 pyopensprinkler-0.7.6/setup.cfg
--rw-r--r--   0 vincent   (1000) vincent   (1000)      824 2023-02-25 21:01:21.000000 pyopensprinkler-0.7.6/setup.py
+drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-21 22:13:13.240000 pyopensprinkler-0.7.7/
+-rw-r--r--   0 vincent   (1000) vincent   (1000)      475 2023-07-21 22:13:13.240000 pyopensprinkler-0.7.7/PKG-INFO
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     2139 2023-07-20 22:16:07.000000 pyopensprinkler-0.7.7/README.md
+drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-21 22:13:13.240000 pyopensprinkler-0.7.7/pyopensprinkler/
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    29175 2022-06-01 21:56:41.000000 pyopensprinkler-0.7.7/pyopensprinkler/__init__.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     1504 2020-07-04 11:32:57.000000 pyopensprinkler-0.7.7/pyopensprinkler/const.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     8821 2023-07-21 22:12:35.000000 pyopensprinkler-0.7.7/pyopensprinkler/program.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     8743 2021-02-27 01:28:46.000000 pyopensprinkler-0.7.7/pyopensprinkler/station.py
+drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2023-07-21 22:13:13.240000 pyopensprinkler-0.7.7/pyopensprinkler.egg-info/
+-rw-rw-rw-   0 vincent   (1000) vincent   (1000)      475 2023-07-21 22:13:13.000000 pyopensprinkler-0.7.7/pyopensprinkler.egg-info/PKG-INFO
+-rw-rw-rw-   0 vincent   (1000) vincent   (1000)      329 2023-07-21 22:13:13.000000 pyopensprinkler-0.7.7/pyopensprinkler.egg-info/SOURCES.txt
+-rw-rw-rw-   0 vincent   (1000) vincent   (1000)        1 2023-07-21 22:13:13.000000 pyopensprinkler-0.7.7/pyopensprinkler.egg-info/dependency_links.txt
+-rw-rw-rw-   0 vincent   (1000) vincent   (1000)       30 2023-07-21 22:13:13.000000 pyopensprinkler-0.7.7/pyopensprinkler.egg-info/requires.txt
+-rw-rw-rw-   0 vincent   (1000) vincent   (1000)       16 2023-07-21 22:13:13.000000 pyopensprinkler-0.7.7/pyopensprinkler.egg-info/top_level.txt
+-rw-r--r--   0 vincent   (1000) vincent   (1000)      154 2023-07-21 22:13:13.240000 pyopensprinkler-0.7.7/setup.cfg
+-rw-r--r--   0 vincent   (1000) vincent   (1000)      824 2023-07-21 22:12:35.000000 pyopensprinkler-0.7.7/setup.py
```

### Comparing `pyopensprinkler-0.7.6/README.md` & `pyopensprinkler-0.7.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Python module for OpenSprinker API
 
 [![PyPI version](https://badge.fury.io/py/pyopensprinkler.svg)](https://badge.fury.io/py/pyopensprinkler)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyopensprinkler)
 ![Linting Status](https://github.com/vinteo/py-opensprinkler/workflows/Linting/badge.svg)
-[![Build Status](https://travis-ci.org/vinteo/py-opensprinkler.svg?branch=master)](https://travis-ci.org/vinteo/py-opensprinkler)
+[![Build Status](https://app.travis-ci.com/vinteo/py-opensprinkler.svg?branch=master)](https://travis-ci.org/vinteo/py-opensprinkler)
 [![codecov](https://codecov.io/gh/vinteo/py-opensprinkler/branch/master/graph/badge.svg)](https://codecov.io/gh/vinteo/py-opensprinkler)
 
 Tested against OpenSprinkler version 2.1.9.
 
 ## Installation
 
 ```bash
```

### Comparing `pyopensprinkler-0.7.6/pyopensprinkler/__init__.py` & `pyopensprinkler-0.7.7/pyopensprinkler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyopensprinkler-0.7.6/pyopensprinkler/const.py` & `pyopensprinkler-0.7.7/pyopensprinkler/const.py`

 * *Files identical despite different names*

### Comparing `pyopensprinkler-0.7.6/pyopensprinkler/program.py` & `pyopensprinkler-0.7.7/pyopensprinkler/program.py`

 * *Files 26% similar despite different names*

```diff
@@ -30,32 +30,15 @@
         return await self._set_variables({variable: value})
 
     async def _set_variables(self, params=None):
         if params is None:
             params = {}
         params["pid"] = self._index
 
-        # hacky garbage to make setting the name work
-        # NOTE: setting en and name in the same request results in the name parameter being ignored
-        v = ""
-        if "v" not in params:
-            dlist = self._get_program_data().copy()
-            if "name" in params:
-                dlist.pop(5)
-            v = json.dumps(dlist).replace(" ", "")
-
-        if "v" in params:
-            name = params["v"].pop(5)
-            if "name" not in params:
-                params["name"] = name
-            v = json.dumps(params.pop("v", None)).replace(" ", "")
-
-        v = v.strip()
-
-        content = await self._controller.request("/cp", params, f"v={v}")
+        content = await self._controller.request("/cp", params)
         return content["result"]
 
     async def _manual_run(self):
         """Run program"""
         params = {"pid": self._index, "uwt": 0}
         content = await self._controller.request("/mp", params)
         return content["result"]
@@ -64,14 +47,21 @@
         return list(
             reversed([int(x) for x in list("{0:08b}".format(self._get_variable(0)))])
         )
 
     def _bits_to_int(self, bits):
         return int("".join(map(str, list(reversed(bits)))), 2)
 
+    def _format_program_data(self, dlist):
+        """Move program name from 'v' to 'name' parameter and remove spaces."""
+        name = dlist.pop(5)
+        v = json.dumps(dlist).replace(" ", "")
+        params = {"v": v, "name": name}
+        return params
+
     async def enable(self):
         """Enable operation"""
         return await self.set_enabled(True)
 
     async def disable(self):
         """Disable operation"""
         return await self.set_enabled(False)
@@ -83,15 +73,18 @@
             return await self._set_variable("en", 0)
 
     async def run(self):
         """Run program"""
         return await self._manual_run()
 
     async def set_name(self, name):
-        return await self._set_variable("name", name)
+        dlist = self._get_program_data().copy()
+        dlist[5] = name
+        params = self._format_program_data(dlist)
+        return await self._set_variables(params)
 
     async def set_use_weather_adjustments(self, value):
         return await self._set_variable("uwt", int(value))
 
     async def set_odd_even_restriction(self, value):
         dlist = self._get_program_data().copy()
         bits = self._get_data_flag_bits()
@@ -111,16 +104,16 @@
 
         # even-days
         if value == 2:
             bits[2] = 0
             bits[3] = 1
 
         dlist[0] = self._bits_to_int(bits)
-
-        return await self._set_variable("v", dlist)
+        params = self._format_program_data(dlist)
+        return await self._set_variables(params)
 
     async def set_program_schedule_type(self, value):
         dlist = self._get_program_data().copy()
         bits = self._get_data_flag_bits()
 
         if value != 0 and value != 3:
             raise ValueError("value must be 0 or 3")
@@ -132,16 +125,16 @@
 
         # interval-day
         if value == 3:
             bits[4] = 1
             bits[5] = 1
 
         dlist[0] = self._bits_to_int(bits)
-
-        return await self._set_variable("v", dlist)
+        params = self._format_program_data(dlist)
+        return await self._set_variables(params)
 
     async def set_start_time_type(self, value):
         dlist = self._get_program_data().copy()
         bits = self._get_data_flag_bits()
 
         if value < 0 or value > 1:
             raise ValueError("value must be 0 or 1")
@@ -151,26 +144,54 @@
             bits[6] = 0
 
         # fixed-time
         if value == 1:
             bits[6] = 1
 
         dlist[0] = self._bits_to_int(bits)
+        params = self._format_program_data(dlist)
+        return await self._set_variables(params)
 
-        return await self._set_variable("v", dlist)
+    async def set_program_start_time(self, start_index, start_time):
+        dlist = self._get_program_data().copy()
+        dlist[3][start_index] = start_time
+        params = self._format_program_data(dlist)
+        return await self._set_variables(params)
+
+    async def set_program_start_times(self, start_times):
+        dlist = self._get_program_data().copy()
+        dlist[3] = start_times
+        params = self._format_program_data(dlist)
+        return await self._set_variables(params)
 
     async def set_station_duration(self, station_index, duration):
         dlist = self._get_program_data().copy()
         dlist[4][station_index] = duration
-        return await self._set_variable("v", dlist)
+        params = self._format_program_data(dlist)
+        return await self._set_variables(params)
 
     async def set_station_durations(self, durations):
         dlist = self._get_program_data().copy()
         dlist[4] = durations
-        return await self._set_variable("v", dlist)
+        params = self._format_program_data(dlist)
+        return await self._set_variables(params)
+
+    async def set_days0(self, value):
+        """Set days0 (weekday bits in Weekday mode, starting in days in Interval mode)"""
+        dlist = self._get_program_data().copy()
+        dlist[1] = value
+        params = self._format_program_data(dlist)
+        return await self._set_variables(params)
+
+    async def set_days1(self, value):
+        """Retrieve days1 (not used in Weekday mode, interval days in Interval mode)"""
+        dlist = self._get_program_data().copy()
+        dlist[2] = value
+        params = self._format_program_data(dlist)
+        return await self._set_variables(params)
 
     @property
     def name(self):
         """Program name"""
         return self._get_variable(5)
 
     @property
@@ -266,7 +287,27 @@
         value = self.start_time_type
 
         if value == 0:
             return SCHEDULE_START_TIME_REPEATING
 
         if value == 1:
             return SCHEDULE_START_TIME_FIXED
+
+    @property
+    def program_start_times(self):
+        """Retrieve station start times"""
+        return self._get_variable(3)
+
+    @property
+    def station_durations(self):
+        """Retrieve station durations"""
+        return self._get_variable(4)
+
+    @property
+    def days0(self):
+        """Retrieve days0 (weekday bits in Weekday mode, starting in days in Interval mode)"""
+        return self._get_variable(1)
+
+    @property
+    def days1(self):
+        """Retrieve days1 (not used in Weekday mode, interval days in Interval mode)"""
+        return self._get_variable(2)
```

### Comparing `pyopensprinkler-0.7.6/pyopensprinkler/station.py` & `pyopensprinkler-0.7.7/pyopensprinkler/station.py`

 * *Files identical despite different names*

### Comparing `pyopensprinkler-0.7.6/setup.py` & `pyopensprinkler-0.7.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """pyopensprinkler setup script."""
 from setuptools import setup
 
-version = "0.7.6"
+version = "0.7.7"
 
 github_username = "vinteo"
 github_repository = "py-opensprinkler"
 
 github_path = f"{github_username}/{github_repository}"
 github_url = f"https://github.com/{github_path}"
 
@@ -14,15 +14,15 @@
 
 setup(
     name="pyopensprinkler",
     version=version,
     author="Vincent Teo, Travis Glenn Hansen",
     author_email="vinteo@gmail.com, travisghansen@yahoo.com",
     packages=["pyopensprinkler"],
-    install_requires=["aiohttp==3.8.4", "backoff==2.2.1"],
+    install_requires=["aiohttp==3.8.5", "backoff==2.2.1"],
     url=github_url,
     download_url=download_url,
     project_urls=project_urls,
     license="MIT",
     description="A Python module for the OpenSprinkler API.",
     platforms="Cross Platform",
 )
```

