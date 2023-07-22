# Comparing `tmp/dapplooker-0.0.1.tar.gz` & `tmp/dapplooker-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapplooker-0.0.1.tar", last modified: Sat Jul 22 20:15:25 2023, max compression
+gzip compressed data, was "dapplooker-0.0.3.tar", last modified: Sat Jul 22 21:00:35 2023, max compression
```

## Comparing `dapplooker-0.0.1.tar` & `dapplooker-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 20:15:25.663463 dapplooker-0.0.1/
--rw-rw-rw-   0        0        0      308 2023-07-22 20:15:25.661461 dapplooker-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-22 15:53:45.000000 dapplooker-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 20:15:25.596473 dapplooker-0.0.1/dapplooker/
--rw-rw-rw-   0        0        0       50 2023-07-22 20:07:29.000000 dapplooker-0.0.1/dapplooker/__init__.py
--rw-rw-rw-   0        0        0      456 2023-07-22 17:10:42.000000 dapplooker-0.0.1/dapplooker/chart_constants.py
--rw-rw-rw-   0        0        0     1947 2023-07-22 20:15:08.000000 dapplooker-0.0.1/dapplooker/dapplooker_charts.py
--rw-rw-rw-   0        0        0      747 2023-07-22 17:12:39.000000 dapplooker-0.0.1/dapplooker/interface.py
-drwxrwxrwx   0        0        0        0 2023-07-22 20:15:25.657462 dapplooker-0.0.1/dapplooker.egg-info/
--rw-rw-rw-   0        0        0      308 2023-07-22 20:15:24.000000 dapplooker-0.0.1/dapplooker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-07-22 20:15:25.000000 dapplooker-0.0.1/dapplooker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 20:15:24.000000 dapplooker-0.0.1/dapplooker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-22 19:56:55.000000 dapplooker-0.0.1/dapplooker.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-07-22 20:15:24.000000 dapplooker-0.0.1/dapplooker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-22 20:15:25.000000 dapplooker-0.0.1/dapplooker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-22 20:15:25.664466 dapplooker-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      872 2023-07-22 16:13:25.000000 dapplooker-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 21:00:35.275759 dapplooker-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-07-22 20:42:35.000000 dapplooker-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3646 2023-07-22 21:00:35.272740 dapplooker-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3317 2023-07-22 20:39:31.000000 dapplooker-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 21:00:35.174742 dapplooker-0.0.3/dapplooker/
+-rw-rw-rw-   0        0        0       50 2023-07-22 20:07:29.000000 dapplooker-0.0.3/dapplooker/__init__.py
+-rw-rw-rw-   0        0        0      456 2023-07-22 17:10:42.000000 dapplooker-0.0.3/dapplooker/chart_constants.py
+-rw-rw-rw-   0        0        0     1918 2023-07-22 20:18:31.000000 dapplooker-0.0.3/dapplooker/dapplooker_charts.py
+-rw-rw-rw-   0        0        0      747 2023-07-22 17:12:39.000000 dapplooker-0.0.3/dapplooker/interface.py
+drwxrwxrwx   0        0        0        0 2023-07-22 21:00:35.268738 dapplooker-0.0.3/dapplooker.egg-info/
+-rw-rw-rw-   0        0        0     3646 2023-07-22 21:00:33.000000 dapplooker-0.0.3/dapplooker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-07-22 21:00:34.000000 dapplooker-0.0.3/dapplooker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 21:00:34.000000 dapplooker-0.0.3/dapplooker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-22 19:56:55.000000 dapplooker-0.0.3/dapplooker.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-22 21:00:34.000000 dapplooker-0.0.3/dapplooker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-22 21:00:34.000000 dapplooker-0.0.3/dapplooker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-22 21:00:35.277753 dapplooker-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      928 2023-07-22 21:00:11.000000 dapplooker-0.0.3/setup.py
```

### Comparing `dapplooker-0.0.1/dapplooker/dapplooker_charts.py` & `dapplooker-0.0.3/dapplooker/dapplooker_charts.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,14 @@
             raise ValueError(
                 f"Invalid output format: {output_format}. Supported formats are: {ChartConstants.supported_format_type}"
             )
 
         # Build the API URL.
         chart_api_url = ChartConstants.get_chart_detail_url
         full_api_url = f"{chart_api_url}/{chart_uuid}?api_key={api_key}&output_format={format}"
-        print(full_api_url)
         # Call the API and get the response.
         res_object = requests.get(full_api_url)
 
         # Check the status code of the response.
         if res_object.status_code in [200, 201, 202, 203, 204]:
             return res_object.json()
         else:
```

### Comparing `dapplooker-0.0.1/dapplooker/interface.py` & `dapplooker-0.0.3/dapplooker/interface.py`

 * *Files identical despite different names*

### Comparing `dapplooker-0.0.1/setup.py` & `dapplooker-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 import os
 
 # Utility function to read the README file.
 # Used for the long_description.  It's nice, because now
 # 1) we have a top level README file, and 
 # 2) it's easier to type in the README file than to put a raw string in below.
 
-def read(*rnames):
-    return open(os.path.join(os.path.dirname(os.path.abspath(__file__)), *rnames)).read()
+# read the contents of  README file
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 setup(
     name="dapplooker",
-    version="0.0.1",
+    version="0.0.3",
     description="A minimal, complete, python API for DappLooker",
-    long_description=read("README.md"),
+    long_description=long_description,
     url="https://github.com/0xSumitBanik/dapplooker-py-sdk",
     long_description_content_type="text/markdown",
     author="Sumit Banik",
     license="MIT",
     packages=[
         "dapplooker"
     ],
```

