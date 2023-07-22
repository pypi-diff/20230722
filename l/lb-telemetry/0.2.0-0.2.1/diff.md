# Comparing `tmp/lb-telemetry-0.2.0.tar.gz` & `tmp/lb-telemetry-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/lhcb/lb-telemetry/dist/.tmp-svmt_l_3/lb-telemetry-0.2.0.tar", last modified: Fri Jul  7 16:05:16 2023, max compression
+gzip compressed data, was "/builds/lhcb/lb-telemetry/dist/.tmp-5nd60wga/lb-telemetry-0.2.1.tar", last modified: Sat Jul 22 12:06:02 2023, max compression
```

## Comparing `lb-telemetry-0.2.0.tar` & `lb-telemetry-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     2191 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1967 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/.mypy.ini
--rw-r--r--   0 root         (0) root         (0)      594 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    18151 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/.pylintrc
--rw-r--r--   0 root         (0) root         (0)    35065 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1379 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      705 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1187 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/src/lb_telemetry/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/src/lb_telemetry/__init__.py
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/src/lb_telemetry/log_fetch_error.py
--rw-r--r--   0 root         (0) root         (0)     5447 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/src/lb_telemetry/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/src/lb_telemetry.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1379 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/src/lb_telemetry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      432 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/src/lb_telemetry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/src/lb_telemetry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       94 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/src/lb_telemetry.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/src/lb_telemetry.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/tests/
--rw-r--r--   0 root         (0) root         (0)       60 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5195 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/tests/test_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 12:06:02.000000 lb-telemetry-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-07-22 12:05:27.000000 lb-telemetry-0.2.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-07-22 12:05:27.000000 lb-telemetry-0.2.1/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-22 12:05:27.000000 lb-telemetry-0.2.1/.mypy.ini
+-rw-r--r--   0 root         (0) root         (0)      594 2023-07-22 12:05:27.000000 lb-telemetry-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    18151 2023-07-22 12:05:27.000000 lb-telemetry-0.2.1/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)    35065 2023-07-22 12:05:27.000000 lb-telemetry-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2214 2023-07-22 12:06:02.000000 lb-telemetry-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-07-22 12:05:27.000000 lb-telemetry-0.2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1210 2023-07-22 12:05:27.000000 lb-telemetry-0.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-22 12:06:02.000000 lb-telemetry-0.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 12:06:02.000000 lb-telemetry-0.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 12:06:02.000000 lb-telemetry-0.2.1/src/lb_telemetry/
+-rw-r--r--   0 root         (0) root         (0)     6374 2023-07-22 12:05:27.000000 lb-telemetry-0.2.1/src/lb_telemetry/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 12:06:02.000000 lb-telemetry-0.2.1/src/lb_telemetry.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2214 2023-07-22 12:06:02.000000 lb-telemetry-0.2.1/src/lb_telemetry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      369 2023-07-22 12:06:02.000000 lb-telemetry-0.2.1/src/lb_telemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-22 12:06:02.000000 lb-telemetry-0.2.1/src/lb_telemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-22 12:06:02.000000 lb-telemetry-0.2.1/src/lb_telemetry.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-22 12:06:02.000000 lb-telemetry-0.2.1/src/lb_telemetry.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 12:06:02.000000 lb-telemetry-0.2.1/tests/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-22 12:05:27.000000 lb-telemetry-0.2.1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6052 2023-07-22 12:05:27.000000 lb-telemetry-0.2.1/tests/test_logger.py
```

### Comparing `lb-telemetry-0.2.0/.gitignore` & `lb-telemetry-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.2.0/.gitlab-ci.yml` & `lb-telemetry-0.2.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.2.0/.pre-commit-config.yaml` & `lb-telemetry-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.2.0/.pylintrc` & `lb-telemetry-0.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.2.0/LICENSE` & `lb-telemetry-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.2.0/pyproject.toml` & `lb-telemetry-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
+    "LbPlatformUtils",
     "logzero",
     "requests",
 ]
 
 [tool.setuptools_scm]
 
 [project.urls]
```

### Comparing `lb-telemetry-0.2.0/src/lb_telemetry/logger.py` & `lb-telemetry-0.2.1/src/lb_telemetry/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 ###############################################################################
-# (c) Copyright 2021 CERN for the benefit of the LHCb Collaboration           #
+# (c) Copyright 2023 CERN for the benefit of the LHCb Collaboration           #
 #                                                                             #
 # This software is distributed under the terms of the GNU General Public      #
 # Licence version 3 (GPL Version 3), copied verbatim in the file "COPYING".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
 
 import json
-import os
-import subprocess
+import platform
 import time
 from typing import Optional
 
+from LbPlatformUtils import inspect
 import requests
 from logzero import logger as logzero
 
 INFLUXDB_LEGAL_TYPES = [bool, int, float, str]
 
 
 class Logger:
@@ -26,25 +26,14 @@
         self,
         producer="lb-telemetry",
         datasource_id="10459",
         database="monit_production_lb_telemetry",
         send_url="http://monit-metrics.cern.ch:10012/",
     ):
         self.producer = producer
-        self.token = os.environ.get("LB_TELEMETRY_TOKEN")
-        if not self.token:
-            self.token = subprocess.check_output(
-                [
-                    "xrdfs",
-                    "root://eoslhcb.cern.ch/",
-                    "cat",
-                    "/eos/lhcb/wg/PID/lb-telemetry/token",
-                ],
-                text=True,
-            )
         self.datasource_id = datasource_id
         self.database = database
         self.send_url = send_url
 
     @staticmethod
     def is_data_valid(data: dict, tags: list) -> bool:
         """Verifies the validity of data for logger usage.
@@ -80,66 +69,99 @@
                 logzero.warning(
                     f"The tag {tag}: ({data[tag]}) has a value of type "
                     f"{type(data[tag])} so will be converted to a string"
                 )
 
         return True
 
-    def build_payload(self, table: str, data: dict, tags: list[str]) -> dict:
+    @staticmethod
+    def get_os_version() -> str:
+        system = platform.system()
+        if system == "Linux":
+            ver_name, ver_num = platform.libc_ver()
+            return f"{ver_name} {ver_num}"
+        elif system == "Darwin":
+            ver_num = platform.mac_ver()[0]
+            return ver_num
+        elif system == "Windows":
+            ver_num = platform.win32_ver()[0]
+            return ver_num
+        else:
+            return "N/A"
+
+    def build_payload(
+        self, table: str, data: dict, tags: list[str], include_host_info: bool
+    ) -> dict:
         """Builds a payload to be sent to MONIT.
 
         The payload timestamp is in ms.
 
         Args:
             table: The name of the calling package and ID for the
                      table the data should be sent to.
             data: The data (tags and fields with their values) to be sent to MONIT.
                   Should not be empty.
             tags: Which data entries are tags (the rest are assumed to be fields).
+            include_host_info: Whether information about the caller's system should
+                               be included in logging (Python version, OS, etc.)
         """
+        if include_host_info:
+            host_info = {
+                "python": f"{platform.python_implementation()} "
+                f"{platform.python_version()}",
+                "system": platform.system(),
+                "processor": inspect.architecture(),
+                "os_version": self.get_os_version(),
+            }
+        else:
+            host_info = {}
+
         payload = {
             "producer": self.producer,
             "type": table,
             "timestamp": int(time.time() * 1000),
-            "idb_tags": tags,
+            "idb_tags": tags + list(host_info.keys()),
         }
 
-        return {**payload, **data}
+        return {**payload, **host_info, **data}
 
-    def log_to_monit(self, package: str, data: dict, tags: list[str]) -> Optional[int]:
+    def log_to_monit(
+        self, package: str, data: dict, tags: list[str], include_host_info: bool = True
+    ) -> Optional[int]:
         """Sends the provided data to MONIT.
 
         The logged data is accessible via MONIT Grafana.
 
         Args:
             package: The name of the calling package and ID for the
                      database the data should be sent to.
             data: The data (tags and fields with their values) to be sent to MONIT.
             tags: Which data entries are tags (the rest are assumed to be fields).
+            include_host_info: Whether information about the caller's system should
+                               be included in logging (Python version, OS, etc.)
 
         Returns:
             The timestamp of the created log entry.
         """
         if not Logger.is_data_valid(data, tags):
             return None
 
-        payload = self.build_payload(package, data, tags)
+        payload = self.build_payload(package, data, tags, include_host_info)
 
         # Send the data to MONIT
         try:
             response = requests.post(
                 self.send_url,
                 headers={
                     "Content-Type": "application/json",
                 },
                 data=json.dumps(payload),
-                verify=False,
             )
         except requests.exceptions.RequestException as e:
-            logzero.warning(
+            logzero.debug(
                 f"An error occurred while logging telemetry "
                 f"(this can happen when running from outside "
                 f"the CERN network): {e}"
             )
             return None
 
         if response.status_code != 200:
```

### Comparing `lb-telemetry-0.2.0/tests/test_logger.py` & `lb-telemetry-0.2.1/tests/test_logger.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,57 +5,77 @@
 # Licence version 3 (GPL Version 3), copied verbatim in the file "COPYING".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
 import json
+import os
 import time
 from typing import Optional
 
+import pytest
 import requests
-from logzero import logger as logzero
 
-from lb_telemetry.log_fetch_error import LogFetchError
-from lb_telemetry.logger import INFLUXDB_LEGAL_TYPES, Logger
+from lb_telemetry import INFLUXDB_LEGAL_TYPES, Logger
 
-TEST_TABLE = "testing"
+TEST_TABLE = "testing_032"
 TEST_DATA = {
     "test_field1": "test_value",
     "test_field2": False,
     "test_field3": 0,
     "test_field4": 3.5,
     "test_tag1": "some_tag",
 }
 TEST_TAGS = ["test_tag1"]
 
 
+class LogFetchError(Exception):
+    pass
+
+
 def test_build_payload_valid():
     logger = Logger()
-    payload: dict = logger.build_payload(
-        table=TEST_TABLE,
-        data=TEST_DATA,
-        tags=TEST_TAGS,
-    )
-
-    # Ensure payload has mandatory fields
-    mandatory_keys = ["producer", "type", "idb_tags"]
-    assert all(key in payload for key in mandatory_keys)
-
-    assert payload["producer"] == logger.producer
-    assert payload["type"] == TEST_TABLE
-    assert payload["idb_tags"] == TEST_TAGS
-
-    # Ensure that all tags declared appear in the payload
-    for tag in payload["idb_tags"]:
-        assert tag in payload
-
-    # Ensure value types are compatible with InfluxDB
-    tags_and_fields = {k: payload[k] for k in payload if k not in mandatory_keys}
-    assert all([type(value) in INFLUXDB_LEGAL_TYPES for value in tags_and_fields])
+
+    for include_host_info in [False, True]:
+        payload: dict = logger.build_payload(
+            table=TEST_TABLE,
+            data=TEST_DATA,
+            tags=TEST_TAGS,
+            include_host_info=include_host_info,
+        )
+
+        # Ensure payload has mandatory fields
+        mandatory_keys = ["producer", "type", "idb_tags"]
+        assert all(key in payload for key in mandatory_keys)
+
+        assert payload["producer"] == logger.producer
+        assert payload["type"] == TEST_TABLE
+
+        # Ensure that all tags we defined appear in the list of tags
+        for tag in TEST_TAGS:
+            assert tag in payload["idb_tags"]
+
+        # Ensure that all tags declared appear in the payload
+        for tag in payload["idb_tags"]:
+            assert tag in payload
+
+        # Ensure value types are compatible with InfluxDB
+        tags_and_fields = {k: payload[k] for k in payload if k not in mandatory_keys}
+        assert all([type(value) in INFLUXDB_LEGAL_TYPES for value in tags_and_fields])
+
+        if include_host_info:
+            payload_without_host_info: dict = logger.build_payload(
+                table=TEST_TABLE,
+                data=TEST_DATA,
+                tags=TEST_TAGS,
+                include_host_info=False,
+            )
+
+            assert len(payload) > len(payload_without_host_info)
 
 
 def test_is_data_valid():
     invalid = [
         ({}, []),
         ({"some_field": ["arrays are", "not allowed"]}, []),
         ({"some_field": {"sets are", "not allowed"}}, []),
@@ -69,60 +89,72 @@
         ({"some_field": "some_value"}, []),
         ({"some_tag": "some_value"}, ["some_tag"]),
         ({"some_field": False, "some_tag": 3.5}, ["some_tag"]),
     ]
     assert all([Logger.is_data_valid(data, tags) for data, tags in valid])
 
 
-def fetch_test_log(logger: Logger, ts: int) -> Optional[dict]:
+@pytest.fixture
+def token() -> str:
+    token = os.environ.get("LB_TELEMETRY_TOKEN")
+    if not token:
+        pytest.skip("LB_TELEMETRY_TOKEN variable not set")
+
+    return token
+
+
+def fetch_test_log(logger: Logger, ts: int, token: str) -> Optional[dict]:
     base_url = "https://monit-grafana.cern.ch/api/datasources"
     path = f"proxy/{logger.datasource_id}/query?db={logger.database}"
     query = f"select * from {TEST_TABLE} where time = {ts}ms"  # noqa
 
     try:
         response = requests.post(
             f"{base_url}/{path}",
             headers={
-                "Authorization": f"Bearer {logger.token}",
+                "Authorization": f"Bearer {token}",
             },
             files={"q": query.encode("utf-8")},
         )
     except requests.exceptions.RequestException as e:
         raise LogFetchError(f"An error occurred while verifying the test log: {e}")
 
     if response.status_code != 200:
         raise LogFetchError(
             f"Unexpected status code {response.status_code}: " f"{response.text}"
         )
 
     results: dict = json.loads(response.text)["results"][0]
 
     if "error" in results:
-        logzero.debug(f"Request path: {path}")
-        logzero.debug(f"Query: {query}")
-        raise LogFetchError(f"An error appeared in the results: {results}")
+        raise LogFetchError(
+            f"An error appeared in the results: {results}\n\n"
+            f"Request path: {path}\n\n"
+            f"Query: {query}"
+        )
     elif "series" in results:
         return results["series"][0]
 
     return None
 
 
-def test_log_to_monit():
+def test_log_to_monit(token):
     # Send valid log
     logger = Logger()
-    ts = logger.log_to_monit(TEST_TABLE, TEST_DATA, TEST_TAGS)
+    ts = logger.log_to_monit(TEST_TABLE, TEST_DATA, TEST_TAGS, include_host_info=False)
     if ts is None:
         raise ValueError("Timestamp of log is None")
 
-    # Check if it can be fetched
-    max_attempts = 10
-    for i in range(max_attempts):
-        fetch_result = fetch_test_log(logger, ts)
+    # Check if the log can be fetched
+    MAX_ATTEMPTS = 10
+    for i in range(MAX_ATTEMPTS):
+        fetch_result = fetch_test_log(logger, ts, token)
 
-        if i == 9:
+        is_final_attempt = i == MAX_ATTEMPTS - 1
+        if is_final_attempt:
             raise AssertionError(
                 "Could not find test measurement "
                 "(there must've been an error posting it)"
             )
 
         if fetch_result is None:
             # Wait a bit
@@ -138,16 +170,16 @@
     for i, field in enumerate(fetch_result["columns"]):
         if field == "time":
             continue
 
         assert TEST_DATA[field] == fetch_result["values"][0][i]
 
 
-def test_log_to_monit_fail():
+def test_log_to_monit_fail(token):
     # Ensure we cannot fetch a fake timestamp
     logger = Logger()
     fake_ts = 10000000
-    assert fetch_test_log(logger, fake_ts) is None
+    assert fetch_test_log(logger, fake_ts, token) is None
 
     invalid_logger = Logger(send_url="invalid")
     ts = invalid_logger.log_to_monit(TEST_TABLE, TEST_DATA, TEST_TAGS)
     assert ts is None
```

