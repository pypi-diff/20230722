# Comparing `tmp/tic-tac-toe-backend-1.7.1.tar.gz` & `tmp/tic-tac-toe-backend-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tic-tac-toe-backend-1.7.1.tar", last modified: Wed Jul 19 02:52:18 2023, max compression
+gzip compressed data, was "tic-tac-toe-backend-1.8.0.tar", last modified: Sat Jul 22 01:31:40 2023, max compression
```

## Comparing `tic-tac-toe-backend-1.7.1.tar` & `tic-tac-toe-backend-1.8.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:52:18.958446 tic-tac-toe-backend-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-19 02:52:18.958446 tic-tac-toe-backend-1.7.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1532 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 02:52:18.958446 tic-tac-toe-backend-1.7.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1182 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:52:18.954446 tic-tac-toe-backend-1.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:52:18.958446 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-19 02:52:18.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-19 02:52:18.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:52:18.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-19 02:52:18.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 02:52:18.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backend.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:52:18.958446 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:52:18.958446 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:52:18.958446 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/models/errors/
--rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/models/errors/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      700 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:52:18.958446 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)      215 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      474 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/models/operations/get_.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      481 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/models/operations/get_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/models/operations/put_games.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:52:18.958446 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2969 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/models/shared/move.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/models/shared/moveparameter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/models/shared/version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5630 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:52:18.958446 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-19 02:52:08.000000 tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:31:40.021401 tic-tac-toe-backend-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-22 01:31:40.021401 tic-tac-toe-backend-1.8.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1532 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 01:31:40.021401 tic-tac-toe-backend-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:31:40.017401 tic-tac-toe-backend-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:31:40.017401 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-22 01:31:39.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-22 01:31:39.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 01:31:39.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-22 01:31:39.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-22 01:31:39.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:31:40.021401 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:31:40.021401 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:31:40.021401 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:31:40.021401 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/models/operations/get_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/models/operations/get_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/models/operations/put_games.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:31:40.021401 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/models/shared/move.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/models/shared/moveparameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/models/shared/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:31:40.021401 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26032 2023-07-22 01:31:30.000000 tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/utils/utils.py
```

### Comparing `tic-tac-toe-backend-1.7.1/LICENSE.md` & `tic-tac-toe-backend-1.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.7.1/PKG-INFO` & `tic-tac-toe-backend-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tic-tac-toe-backend
-Version: 1.7.1
+Version: 1.8.0
 Summary: Tic Tac Toe Backend Python Client SDK
 Home-page: UNKNOWN
 Author: Shain Lafazan
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `tic-tac-toe-backend-1.7.1/README.md` & `tic-tac-toe-backend-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.7.1/setup.py` & `tic-tac-toe-backend-1.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="tic-tac-toe-backend",
-    version="1.7.1",
+    version="1.8.0",
     author="Shain Lafazan",
     description="Tic Tac Toe Backend Python Client SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi>=2022.12.7",
         "charset-normalizer>=2.1.1",
-        "dataclasses-json-speakeasy>=0.5.8",
+        "dataclasses-json>=0.5.12",
         "idna>=3.3",
         "jsonpath-python>=1.0.6 ",
         "marshmallow>=3.17.1",
         "marshmallow-enum>=1.5.1",
         "mypy-extensions>=0.4.3",
         "packaging>=21.3",
         "pyparsing>=3.0.9",
```

### Comparing `tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backend.egg-info/PKG-INFO` & `tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tic-tac-toe-backend
-Version: 1.7.1
+Version: 1.8.0
 Summary: Tic Tac Toe Backend Python Client SDK
 Home-page: UNKNOWN
 Author: Shain Lafazan
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backend.egg-info/SOURCES.txt` & `tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/models/errors/sdkerror.py` & `tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/models/shared/__init__.py` & `tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/models/shared/move.py` & `tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/models/shared/move.py`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/sdk.py` & `tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/sdk.py`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/sdkconfiguration.py` & `tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/sdkconfiguration.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 class SDKConfiguration:
     client: requests.Session
     security_client: requests.Session
     server_url: str = ''
     server_idx: int = 0
     language: str = 'python'
     openapi_doc_version: str = '1.0.0'
-    sdk_version: str = '1.7.1'
-    gen_version: str = '2.70.2'
+    sdk_version: str = '1.8.0'
+    gen_version: str = '2.71.0'
 
     def get_server_details(self) -> tuple[str, dict[str, str]]:
         if self.server_url:
             return self.server_url.removesuffix('/'), {}
         if self.server_idx is None:
             self.server_idx = 0
```

### Comparing `tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/utils/retries.py` & `tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/utils/retries.py`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.7.1/src/tic_tac_toe_backends/utils/utils.py` & `tic-tac-toe-backend-1.8.0/src/tic_tac_toe_backends/utils/utils.py`

 * *Files identical despite different names*

