# Comparing `tmp/get-gecko-driver-1.3.8.tar.gz` & `tmp/get-gecko-driver-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get-gecko-driver-1.3.8.tar", last modified: Tue Oct  4 05:48:58 2022, max compression
+gzip compressed data, was "get-gecko-driver-1.3.9.tar", last modified: Tue Oct  4 06:21:08 2022, max compression
```

## Comparing `get-gecko-driver-1.3.8.tar` & `get-gecko-driver-1.3.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-10-04 05:48:58.458352 get-gecko-driver-1.3.8/
--rw-rw-rw-   0        0        0     1091 2022-10-03 02:34:50.000000 get-gecko-driver-1.3.8/LICENSE
--rw-rw-rw-   0        0        0     4219 2022-10-04 05:48:58.458352 get-gecko-driver-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     3436 2022-10-03 03:05:10.000000 get-gecko-driver-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2022-10-04 05:48:58.436355 get-gecko-driver-1.3.8/get_gecko_driver/
--rw-rw-rw-   0        0        0       65 2022-10-04 03:39:27.000000 get-gecko-driver-1.3.8/get_gecko_driver/__init__.py
--rw-rw-rw-   0        0        0     4788 2022-10-04 03:38:38.000000 get-gecko-driver-1.3.8/get_gecko_driver/app.py
--rw-rw-rw-   0        0        0      311 2022-09-27 00:28:38.000000 get-gecko-driver-1.3.8/get_gecko_driver/constants.py
--rw-rw-rw-   0        0        0     2492 2022-10-04 03:48:56.000000 get-gecko-driver-1.3.8/get_gecko_driver/downloader.py
-drwxrwxrwx   0        0        0        0 2022-10-04 05:48:58.449351 get-gecko-driver-1.3.8/get_gecko_driver/enums/
--rw-rw-rw-   0        0        0       32 2022-10-03 02:27:49.000000 get-gecko-driver-1.3.8/get_gecko_driver/enums/__init__.py
--rw-rw-rw-   0        0        0      248 2022-10-03 03:30:10.000000 get-gecko-driver-1.3.8/get_gecko_driver/enums/platform.py
--rw-rw-rw-   0        0        0      294 2022-09-23 03:18:54.000000 get-gecko-driver-1.3.8/get_gecko_driver/exceptions.py
--rw-rw-rw-   0        0        0     8963 2022-10-04 03:44:13.000000 get-gecko-driver-1.3.8/get_gecko_driver/get_driver.py
-drwxrwxrwx   0        0        0        0 2022-10-04 05:48:58.457362 get-gecko-driver-1.3.8/get_gecko_driver/test/
--rw-rw-rw-   0        0        0        0 2022-09-23 03:18:54.000000 get-gecko-driver-1.3.8/get_gecko_driver/test/__init__.py
--rw-rw-rw-   0        0        0     5184 2022-10-03 03:07:10.000000 get-gecko-driver-1.3.8/get_gecko_driver/test/test_app.py
-drwxrwxrwx   0        0        0        0 2022-10-04 05:48:58.446352 get-gecko-driver-1.3.8/get_gecko_driver.egg-info/
--rw-rw-rw-   0        0        0     4219 2022-10-04 05:48:58.000000 get-gecko-driver-1.3.8/get_gecko_driver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      592 2022-10-04 05:48:58.000000 get-gecko-driver-1.3.8/get_gecko_driver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-04 05:48:58.000000 get-gecko-driver-1.3.8/get_gecko_driver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2022-10-04 05:48:58.000000 get-gecko-driver-1.3.8/get_gecko_driver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       58 2022-10-04 05:48:58.000000 get-gecko-driver-1.3.8/get_gecko_driver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2022-10-04 05:48:58.000000 get-gecko-driver-1.3.8/get_gecko_driver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      133 2022-10-04 05:48:58.460355 get-gecko-driver-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1289 2022-10-04 03:39:27.000000 get-gecko-driver-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-04 06:21:08.678080 get-gecko-driver-1.3.9/
+-rw-rw-rw-   0        0        0     1091 2022-10-03 02:34:50.000000 get-gecko-driver-1.3.9/LICENSE
+-rw-rw-rw-   0        0        0     4219 2022-10-04 06:21:08.678080 get-gecko-driver-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3436 2022-10-03 03:05:10.000000 get-gecko-driver-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2022-10-04 06:21:08.655088 get-gecko-driver-1.3.9/get_gecko_driver/
+-rw-rw-rw-   0        0        0       65 2022-10-04 06:19:07.000000 get-gecko-driver-1.3.9/get_gecko_driver/__init__.py
+-rw-rw-rw-   0        0        0     4788 2022-10-04 03:38:38.000000 get-gecko-driver-1.3.9/get_gecko_driver/app.py
+-rw-rw-rw-   0        0        0      311 2022-09-27 00:28:38.000000 get-gecko-driver-1.3.9/get_gecko_driver/constants.py
+-rw-rw-rw-   0        0        0     2478 2022-10-04 06:18:32.000000 get-gecko-driver-1.3.9/get_gecko_driver/downloader.py
+drwxrwxrwx   0        0        0        0 2022-10-04 06:21:08.675078 get-gecko-driver-1.3.9/get_gecko_driver/enums/
+-rw-rw-rw-   0        0        0       32 2022-10-03 02:27:49.000000 get-gecko-driver-1.3.9/get_gecko_driver/enums/__init__.py
+-rw-rw-rw-   0        0        0      248 2022-10-03 03:30:10.000000 get-gecko-driver-1.3.9/get_gecko_driver/enums/platform.py
+-rw-rw-rw-   0        0        0      294 2022-09-23 03:18:54.000000 get-gecko-driver-1.3.9/get_gecko_driver/exceptions.py
+-rw-rw-rw-   0        0        0     8942 2022-10-04 06:18:32.000000 get-gecko-driver-1.3.9/get_gecko_driver/get_driver.py
+drwxrwxrwx   0        0        0        0 2022-10-04 06:21:08.677082 get-gecko-driver-1.3.9/get_gecko_driver/test/
+-rw-rw-rw-   0        0        0        0 2022-09-23 03:18:54.000000 get-gecko-driver-1.3.9/get_gecko_driver/test/__init__.py
+-rw-rw-rw-   0        0        0     5184 2022-10-03 03:07:10.000000 get-gecko-driver-1.3.9/get_gecko_driver/test/test_app.py
+drwxrwxrwx   0        0        0        0 2022-10-04 06:21:08.673079 get-gecko-driver-1.3.9/get_gecko_driver.egg-info/
+-rw-rw-rw-   0        0        0     4219 2022-10-04 06:21:08.000000 get-gecko-driver-1.3.9/get_gecko_driver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      592 2022-10-04 06:21:08.000000 get-gecko-driver-1.3.9/get_gecko_driver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-04 06:21:08.000000 get-gecko-driver-1.3.9/get_gecko_driver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2022-10-04 06:21:08.000000 get-gecko-driver-1.3.9/get_gecko_driver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       58 2022-10-04 06:21:08.000000 get-gecko-driver-1.3.9/get_gecko_driver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2022-10-04 06:21:08.000000 get-gecko-driver-1.3.9/get_gecko_driver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      133 2022-10-04 06:21:08.680080 get-gecko-driver-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1289 2022-10-04 06:19:07.000000 get-gecko-driver-1.3.9/setup.py
```

### Comparing `get-gecko-driver-1.3.8/LICENSE` & `get-gecko-driver-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `get-gecko-driver-1.3.8/PKG-INFO` & `get-gecko-driver-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: get-gecko-driver
-Version: 1.3.8
+Version: 1.3.9
 Summary: A tool to download and install GeckoDriver.
 Home-page: https://github.com/zaironjacobs/get-gecko-driver
-Download-URL: https://github.com/zaironjacobs/get-gecko-driver/archive/v1.3.8.tar.gz
+Download-URL: https://github.com/zaironjacobs/get-gecko-driver/archive/v1.3.9.tar.gz
 Author: Zairon Jacobs
 Author-email: zaironjacobs@gmail.com
 License: MIT
 Keywords: gecko,geckodriver,download,install,web,driver,tool
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `get-gecko-driver-1.3.8/README.md` & `get-gecko-driver-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `get-gecko-driver-1.3.8/get_gecko_driver/app.py` & `get-gecko-driver-1.3.9/get_gecko_driver/app.py`

 * *Files identical despite different names*

### Comparing `get-gecko-driver-1.3.8/get_gecko_driver/downloader.py` & `get-gecko-driver-1.3.9/get_gecko_driver/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from urllib3.util.retry import Retry
 from requests.adapters import HTTPAdapter
 from urllib.parse import urlparse
 from requests.exceptions import RequestException
 from requests.exceptions import HTTPError
 
 
-def download(url: str, output_path: str | None = None, file_name: str | None = None):
+def download(url: str, output_path: str = None, file_name: str = None):
     """
     Download a file from url
     If output_path is None, the file will be downloaded directly at the current directory
     If file_name is None, the file name from the url will be used
     """
 
     session = __retry_session(retries=3,
```

### Comparing `get-gecko-driver-1.3.8/get_gecko_driver/get_driver.py` & `get-gecko-driver-1.3.9/get_gecko_driver/get_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from .exceptions import UnknownPlatformError
 from .exceptions import VersionUrlError
 from .exceptions import UnknownVersionError
 from .exceptions import DownloadError
 
 
 class GetGeckoDriver:
-    def __init__(self, platform: Platform | None = None):
+    def __init__(self, platform: Platform = None):
         if not platform:
             if pl.system() == 'Windows':
                 self.__system_platform = self.__check_platform(Platform.win)
             elif pl.system() == 'Linux':
                 self.__system_platform = self.__check_platform(Platform.linux)
             elif pl.system() == 'Darwin':
                 self.__system_platform = self.__check_platform(Platform.macos)
@@ -102,26 +102,26 @@
                     # No 64 bit, get 32 bit
                     pass
             # 32bit
             url = constants.url_download.format(version, version, Platform.macos) + tar_gz_ext
             self.__check_if_url_is_valid(url)
             return url
 
-    def download_latest_version(self, output_path: str | None = None, extract: bool = False):
+    def download_latest_version(self, output_path: str = None, extract: bool = False):
         """
         Download the latest geckodriver version
 
         :param output_path: Path to download the driver to
         :param extract: Extract the downloaded driver or not
         """
 
         version = self.latest_version()
         self.download_version(version=version, output_path=output_path, extract=extract)
 
-    def download_version(self, version: str, output_path: str | None = None, extract: bool = False) -> str:
+    def download_version(self, version: str, output_path: str = None, extract: bool = False) -> str:
         """
         Download a geckodriver version
 
         :param version: Geckodriver version
         :param output_path: Path to download the driver to
         :param extract: Extract the downloaded driver or not
         """
```

### Comparing `get-gecko-driver-1.3.8/get_gecko_driver/test/test_app.py` & `get-gecko-driver-1.3.9/get_gecko_driver/test/test_app.py`

 * *Files identical despite different names*

### Comparing `get-gecko-driver-1.3.8/get_gecko_driver.egg-info/PKG-INFO` & `get-gecko-driver-1.3.9/get_gecko_driver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: get-gecko-driver
-Version: 1.3.8
+Version: 1.3.9
 Summary: A tool to download and install GeckoDriver.
 Home-page: https://github.com/zaironjacobs/get-gecko-driver
-Download-URL: https://github.com/zaironjacobs/get-gecko-driver/archive/v1.3.8.tar.gz
+Download-URL: https://github.com/zaironjacobs/get-gecko-driver/archive/v1.3.9.tar.gz
 Author: Zairon Jacobs
 Author-email: zaironjacobs@gmail.com
 License: MIT
 Keywords: gecko,geckodriver,download,install,web,driver,tool
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `get-gecko-driver-1.3.8/get_gecko_driver.egg-info/SOURCES.txt` & `get-gecko-driver-1.3.9/get_gecko_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `get-gecko-driver-1.3.8/setup.py` & `get-gecko-driver-1.3.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 
 name = 'get-gecko-driver'
-version = '1.3.8'
+version = '1.3.9'
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 requires = [
     'bs4>=0.0.1',
     'requests>=2.28.1',
```

