# Comparing `tmp/webdriver_manager-3.8.6.tar.gz` & `tmp/webdriver_manager-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webdriver_manager-3.8.6.tar", last modified: Thu Apr 13 20:11:36 2023, max compression
+gzip compressed data, was "dist/webdriver_manager-3.9.0.tar", last modified: Sat Jul 22 15:06:22 2023, max compression
```

## Comparing `webdriver_manager-3.8.6.tar` & `webdriver_manager-3.9.0.tar`

### file list

```diff
@@ -1,59 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:36.435014 webdriver_manager-3.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-04-13 20:11:36.435014 webdriver_manager-3.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10136 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-13 20:11:36.439015 webdriver_manager-3.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:36.435014 webdriver_manager-3.8.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_brave_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_chrome_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_chromium_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_custom_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_custom_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_edge_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_firefox_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_ie_driver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2742 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_opera_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_silent_global_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:36.435014 webdriver_manager-3.8.6/tests_negative/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests_negative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests_negative/test_browsers_not_installed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:36.435014 webdriver_manager-3.8.6/tests_xdist/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests_xdist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests_xdist/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests_xdist/test_cuncurent_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests_xdist/test_cuncurent_2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:36.435014 webdriver_manager-3.8.6/webdriver_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/chrome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:36.435014 webdriver_manager-3.8.6/webdriver_manager/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/download_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/driver_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:36.435014 webdriver_manager-3.8.6/webdriver_manager/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/drivers/chrome.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/drivers/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/drivers/firefox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/drivers/ie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/drivers/opera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/firefox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/microsoft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1743 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/opera.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:36.435014 webdriver_manager-3.8.6/webdriver_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-04-13 20:11:36.000000 webdriver_manager-3.8.6/webdriver_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-13 20:11:36.000000 webdriver_manager-3.8.6/webdriver_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:11:36.000000 webdriver_manager-3.8.6/webdriver_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:11:36.000000 webdriver_manager-3.8.6/webdriver_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-13 20:11:36.000000 webdriver_manager-3.8.6/webdriver_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:06:22.000000 webdriver_manager-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-07-22 15:06:22.000000 webdriver_manager-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10136 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-22 15:06:22.000000 webdriver_manager-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:06:22.000000 webdriver_manager-3.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/tests/test_brave_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/tests/test_chrome_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/tests/test_chromium_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/tests/test_custom_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/tests/test_custom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/tests/test_edge_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/tests/test_firefox_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/tests/test_ie_driver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2742 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/tests/test_opera_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/tests/test_silent_global_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:06:22.000000 webdriver_manager-3.9.0/webdriver_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/chrome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:06:22.000000 webdriver_manager-3.9.0/webdriver_manager/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/core/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/core/download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/core/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/core/driver_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/core/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/core/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12151 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:06:22.000000 webdriver_manager-3.9.0/webdriver_manager/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/drivers/chrome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/drivers/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/drivers/firefox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/drivers/ie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/drivers/opera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/firefox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/microsoft.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1743 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/opera.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:05:57.000000 webdriver_manager-3.9.0/webdriver_manager/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:06:22.000000 webdriver_manager-3.9.0/webdriver_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-07-22 15:06:22.000000 webdriver_manager-3.9.0/webdriver_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-22 15:06:22.000000 webdriver_manager-3.9.0/webdriver_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 15:06:22.000000 webdriver_manager-3.9.0/webdriver_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 15:06:22.000000 webdriver_manager-3.9.0/webdriver_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-22 15:06:22.000000 webdriver_manager-3.9.0/webdriver_manager.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `webdriver_manager-3.8.6/LICENSE` & `webdriver_manager-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/PKG-INFO` & `webdriver_manager-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdriver_manager
-Version: 3.8.6
+Version: 3.9.0
 Summary: Library provides the way to automatically manage drivers for different browsers
 Home-page: https://github.com/SergeyPirogov/webdriver_manager
 Author: Sergey Pirogov
 Author-email: automationremarks@gmail.com
 Keywords: testing,selenium,driver,test automation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Information Technology
```

### Comparing `webdriver_manager-3.8.6/README.md` & `webdriver_manager-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/setup.py` & `webdriver_manager-3.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     readme = readme_file.read()
 
 setuptools.setup(
     name='webdriver_manager',
     python_requires=">=3.7",
     long_description=readme,
     long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(exclude=['tests']),
+    packages=setuptools.find_packages(include=['webdriver_manager*']),
     include_package_data=True,
-    version='3.8.6',
+    version='3.9.0',
     description='Library provides the way to automatically manage drivers for different browsers',
     author='Sergey Pirogov',
     author_email='automationremarks@gmail.com',
     url='https://github.com/SergeyPirogov/webdriver_manager',
     keywords=['testing', 'selenium', 'driver', 'test automation'],
     classifiers=[
         'License :: OSI Approved :: Apache Software License',
```

### Comparing `webdriver_manager-3.8.6/tests/test_brave_driver.py` & `webdriver_manager-3.9.0/tests/test_brave_driver.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 
 def test_brave_manager_with_specific_version():
     bin_path = ChromeDriverManager("87.0.4280.88", chrome_type=ChromeType.BRAVE).install()
     assert os.path.exists(bin_path)
 
 
+@pytest.mark.skip(reason='Brave version is strange on CI')
 def test_brave_manager_with_selenium():
     binary_location = {
         OSType.LINUX: "/usr/bin/brave-browser",
         OSType.MAC: "/Applications/Brave Browser.app/Contents/MacOS/Brave Browser",
         OSType.WIN: f"{os.getenv('LOCALAPPDATA')}\\BraveSoftware\\Brave-Browser\\Application\\brave.exe",
     }[os_name()]
     log(binary_location)
@@ -41,23 +42,14 @@
     driver_path = ChromeDriverManager(chrome_type=ChromeType.BRAVE).install()
     driver = webdriver.Chrome(driver_path, options=option)
 
     driver.get("http://automation-remarks.com")
     driver.close()
 
 
-def test_driver_can_be_saved_to_custom_path():
-    custom_path = os.path.join(os.path.dirname(os.path.dirname(__file__)), "custom")
-
-    path = ChromeDriverManager(version="87.0.4280.88", path=custom_path,
-                               chrome_type=ChromeType.BRAVE).install()
-    assert os.path.exists(path)
-    assert custom_path in path
-
-
 def test_brave_manager_with_wrong_version():
     with pytest.raises(ValueError) as ex:
         ChromeDriverManager("0.2", chrome_type=ChromeType.BRAVE).install()
     assert "There is no such driver by url" in ex.value.args[0]
 
 
 @pytest.mark.parametrize('os_type', ['win32', 'win64'])
```

### Comparing `webdriver_manager-3.8.6/tests/test_chrome_driver.py` & `webdriver_manager-3.9.0/tests/test_chrome_driver.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,37 +2,40 @@
 import os
 
 import pytest
 from selenium import webdriver
 
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.core.constants import ROOT_FOLDER_NAME
+from selenium.webdriver.chrome.service import Service as ChromeService
+
+os.environ.setdefault("WDM_LOCAL", "true")
 
 
 def test_chrome_manager_with_cache(delete_drivers_dir):
     ChromeDriverManager().install()
-    bin = ChromeDriverManager().install()
-    assert os.path.exists(bin)
+    driver_binary = ChromeDriverManager().install()
+    assert os.path.exists(driver_binary)
 
 
 def test_chrome_manager_with_specific_version(delete_drivers_dir):
-    bin = ChromeDriverManager("87.0.4280.88").install()
-    assert os.path.exists(bin)
+    driver_binary = ChromeDriverManager("87.0.4280.88").install()
+    assert os.path.exists(driver_binary)
 
 
 def test_106_0_5249_61_chrome_version(delete_drivers_dir):
-    bin = ChromeDriverManager("106.0.5249.61").install()
-    assert os.path.exists(bin)
+    driver_binary = ChromeDriverManager("106.0.5249.61").install()
+    assert os.path.exists(driver_binary)
 
 
 def test_chrome_manager_with_project_root_local_folder(delete_drivers_dir):
     os.environ['WDM_LOCAL'] = "1"
-    bin = ChromeDriverManager("87.0.4280.88").install()
+    driver_binary = ChromeDriverManager("87.0.4280.88").install()
     os.environ['WDM_LOCAL'] = "0"
-    assert os.path.exists(bin)
+    assert os.path.exists(driver_binary)
 
 
 def test_driver_can_be_saved_to_custom_path():
     custom_path = os.path.join(os.path.dirname(os.path.dirname(__file__)), "custom")
     path = ChromeDriverManager(version="87.0.4280.88", path=custom_path).install()
     assert os.path.exists(path)
     assert custom_path in path
@@ -42,15 +45,15 @@
     with pytest.raises(ValueError) as ex:
         ChromeDriverManager("0.2").install()
     assert "There is no such driver by url" in ex.value.args[0]
 
 
 def test_chrome_manager_with_selenium():
     driver_path = ChromeDriverManager().install()
-    driver = webdriver.Chrome(driver_path)
+    driver = webdriver.Chrome(service=ChromeService(driver_path))
     driver.get("http://automation-remarks.com")
     driver.close()
 
 
 def test_driver_with_ssl_verify_disabled_can_be_downloaded(ssl_verify_enable):
     os.environ['WDM_SSL_VERIFY'] = '0'
     custom_path = os.path.join(os.path.dirname(
@@ -79,10 +82,10 @@
     with open(metadata_file, 'w') as outfile:
         json.dump(data, outfile)
 
     ChromeDriverManager(path=custom_path).install()
 
 
 @pytest.mark.parametrize('os_type', ['win32', 'win64', 'mac64', 'mac64_m1'])
-def test_can_get_chrome_for_win(os_type):
+def test_can_get_chrome_for_os(os_type):
     path = ChromeDriverManager(os_type=os_type).install()
     assert os.path.exists(path)
```

### Comparing `webdriver_manager-3.8.6/tests/test_chromium_driver.py` & `webdriver_manager-3.9.0/tests/test_chromium_driver.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/tests/test_custom_http_client.py` & `webdriver_manager-3.9.0/tests/test_custom_http_client.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/tests/test_custom_logger.py` & `webdriver_manager-3.9.0/tests/test_custom_logger.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/tests/test_downloader.py` & `webdriver_manager-3.9.0/tests/test_downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,33 +9,33 @@
 from webdriver_manager.drivers.chrome import ChromeDriver
 
 download_manager = WDMDownloadManager()
 
 
 def test_can_download_driver_as_zip_file(delete_drivers_dir):
     file = download_manager.download_file("http://chromedriver.storage.googleapis.com/2.26/chromedriver_win32.zip")
-    assert file.filename == "driver.zip"
+    assert file.filename == "chromedriver_win32.zip"
     archive = save_file(file, DEFAULT_PROJECT_ROOT_CACHE_PATH)
     assert archive.file_path == f"{DEFAULT_PROJECT_ROOT_CACHE_PATH}{os.sep}{file.filename}"
     assert archive.unpack(DEFAULT_PROJECT_ROOT_CACHE_PATH) == ["chromedriver.exe"]
 
 
 def test_can_download_driver_as_tar_gz(delete_drivers_dir):
     file = download_manager.download_file(
         "https://github.com/mozilla/geckodriver/releases/download/v0.26.0/geckodriver-v0.26.0-linux32.tar.gz")
     assert file.filename == 'geckodriver-v0.26.0-linux32.tar.gz'
     archive = save_file(file, DEFAULT_PROJECT_ROOT_CACHE_PATH)
     assert archive.file_path == f"{DEFAULT_PROJECT_ROOT_CACHE_PATH}{os.sep}{file.filename}"
     assert archive.unpack(DEFAULT_PROJECT_ROOT_CACHE_PATH) == ["geckodriver"]
 
 
-@pytest.mark.parametrize('version', ["2.26", None])
+@pytest.mark.parametrize('version', ["2.26"])
 def test_can_download_chrome_driver(delete_drivers_dir, version):
     driver = ChromeDriver(name="chromedriver", version=version, os_type="win32",
                           url="http://chromedriver.storage.googleapis.com",
                           latest_release_url="http://chromedriver.storage.googleapis.com/LATEST_RELEASE",
                           chrome_type=ChromeType.GOOGLE, http_client=WDMHttpClient())
 
     file = download_manager.download_file(driver.get_driver_download_url())
-    assert file.filename == "driver.zip"
+    assert file.filename == "chromedriver_win32.zip"
     archive = save_file(file, DEFAULT_PROJECT_ROOT_CACHE_PATH)
     assert "chromedriver.exe" in archive.unpack(DEFAULT_PROJECT_ROOT_CACHE_PATH)
```

### Comparing `webdriver_manager-3.8.6/tests/test_edge_driver.py` & `webdriver_manager-3.9.0/tests/test_edge_driver.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/tests/test_firefox_manager.py` & `webdriver_manager-3.9.0/tests/test_firefox_manager.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/tests/test_ie_driver.py` & `webdriver_manager-3.9.0/tests/test_ie_driver.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/tests/test_opera_manager.py` & `webdriver_manager-3.9.0/tests/test_opera_manager.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/tests/test_utils.py` & `webdriver_manager-3.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/webdriver_manager/chrome.py` & `webdriver_manager-3.9.0/webdriver_manager/chrome.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,9 +33,10 @@
             latest_release_url=latest_release_url,
             chrome_type=chrome_type,
             http_client=self.http_client,
         )
 
     def install(self) -> str:
         driver_path = self._get_driver_path(self.driver)
-        os.chmod(driver_path, 0o755)
+        if all(test_os not in driver_path for test_os in ["mac_arm64", "mac_x64"]):
+            os.chmod(driver_path, 0o755)
         return driver_path
```

### Comparing `webdriver_manager-3.8.6/webdriver_manager/core/archive.py` & `webdriver_manager-3.9.0/webdriver_manager/core/archive.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,14 +39,26 @@
             archive.extractall(to_directory)
         except Exception as e:
             if e.args[0] not in [26, 13] and e.args[1] not in [
                 "Text file busy",
                 "Permission denied",
             ]:
                 raise e
+            file_names = []
+            for n in archive.namelist():
+                if "/" not in n:
+                    file_names.append(n)
+                else:
+                    file_path, file_name = n.split("/")
+                    full_file_path = os.path.join(to_directory, file_path)
+                    source = os.path.join(full_file_path, file_name)
+                    destination = os.path.join(to_directory, file_name)
+                    os.rename(source, destination)
+                    file_names.append(file_name)
+            return sorted(file_names, key=lambda x: x.lower())
         return archive.namelist()
 
     def __extract_tar_file(self, to_directory):
         try:
             tar = tarfile.open(self.file_path, mode="r:gz")
         except tarfile.ReadError:
             tar = tarfile.open(self.file_path, mode="r:bz2")
```

### Comparing `webdriver_manager-3.8.6/webdriver_manager/core/config.py` & `webdriver_manager-3.9.0/webdriver_manager/core/config.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/webdriver_manager/core/driver.py` & `webdriver_manager-3.9.0/webdriver_manager/core/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,16 @@
     def get_driver_version_to_download(self):
         """
         Downloads version from parameter if version not None or "latest".
         Downloads latest, if version is "latest" or browser could not been determined.
         Downloads determined browser version driver in all other ways as a bonus fallback for lazy users.
         """
         if not self._driver_to_download_version:
-            self._driver_to_download_version = self._version if self._version not in (None, "latest") else self.get_latest_release_version()
+            self._driver_to_download_version = self._version if self._version not in (None, "latest") \
+                else self.get_latest_release_version()
         return self._driver_to_download_version
 
     def get_latest_release_version(self):
         # type: () -> str
         raise NotImplementedError("Please implement this method")
 
     def get_browser_version_from_os(self):
```

### Comparing `webdriver_manager-3.8.6/webdriver_manager/core/driver_cache.py` & `webdriver_manager-3.9.0/webdriver_manager/core/driver_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,18 +42,23 @@
         binary = self.__get_binary(files, driver.get_name())
         binary_path = os.path.join(path, binary)
         self.__save_metadata(driver, binary_path)
         log(f"Driver has been saved in cache [{path}]")
         return binary_path
 
     def __get_binary(self, files, driver_name):
+        if not files:
+            raise Exception(f"Can't find binary for {driver_name} among {files}")
+
         if len(files) == 1:
             return files[0]
 
         for f in files:
+            if 'LICENSE' in f:
+                continue
             if driver_name in f:
                 return f
 
         raise Exception(f"Can't find binary for {driver_name} among {files}")
 
     def __save_metadata(self, driver: Driver, binary_path, date=None):
         if date is None:
```

### Comparing `webdriver_manager-3.8.6/webdriver_manager/core/http.py` & `webdriver_manager-3.9.0/webdriver_manager/core/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,11 +31,9 @@
     def get(self, url, **kwargs) -> Response:
         try:
             resp = requests.get(
                 url=url, verify=self._ssl_verify, stream=True, **kwargs)
         except exceptions.ConnectionError:
             raise ConnectionError(f"Could not reach host. Are you offline?")
         self.validate_response(resp)
-        if wdm_progress_bar():
-            show_download_progress(resp)
         return resp
```

### Comparing `webdriver_manager-3.8.6/webdriver_manager/core/logger.py` & `webdriver_manager-3.9.0/webdriver_manager/core/logger.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/webdriver_manager/core/manager.py` & `webdriver_manager-3.9.0/webdriver_manager/core/manager.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/webdriver_manager/core/utils.py` & `webdriver_manager-3.9.0/webdriver_manager/core/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,32 +4,37 @@
 import re
 import subprocess
 import sys
 
 from tqdm import tqdm
 
 from webdriver_manager.core.archive import Archive
-from webdriver_manager.core.logger import log
 
 
 class File(object):
-    def __init__(self, stream):
+    def __init__(self, stream, file_name):
         self.content = stream.content
         self.__stream = stream
+        self.file_name = file_name
         self.__temp_name = "driver"
+        self.__regex_filename = r"""filename.+"(.+)"|filename.+''(.+)|filename=([\w.-]+)"""
 
     @property
     def filename(self) -> str:
+        if self.file_name:
+            return self.file_name
         try:
-            filename = re.findall(
-                "filename=(.+)", self.__stream.headers["content-disposition"]
-            )[0]
+            content = self.__stream.headers["content-disposition"]
+
+            content_disposition_list = re.split(";", content)
+            filenames = [re.findall(self.__regex_filename, element) for element in content_disposition_list]
+            filename = next(filter(None, next(filter(None, next(filter(None, filenames))))))
         except KeyError:
             filename = f"{self.__temp_name}.zip"
-        except IndexError:
+        except (IndexError, StopIteration):
             filename = f"{self.__temp_name}.exe"
 
         if '"' in filename:
             filename = filename.replace('"', "")
 
         return filename
 
@@ -56,17 +61,17 @@
     CHROMIUM = "chromium"
     BRAVE = "brave-browser"
     MSEDGE = "edge"
 
 
 PATTERN = {
     ChromeType.CHROMIUM: r"\d+\.\d+\.\d+",
-    ChromeType.GOOGLE: r"\d+\.\d+\.\d+",
+    ChromeType.GOOGLE: r"\d+\.\d+\.\d+(\.\d+)?",
     ChromeType.MSEDGE: r"\d+\.\d+\.\d+",
-    "brave-browser": r"(\d+)",
+    "brave-browser": r"\d+\.\d+\.\d+(\.\d+)?",
     "firefox": r"(\d+.\d+)",
 }
 
 
 def os_name():
     pl = sys.platform
     if pl == "linux" or pl == "linux2":
```

### Comparing `webdriver_manager-3.8.6/webdriver_manager/drivers/chrome.py` & `webdriver_manager-3.9.0/webdriver_manager/drivers/chrome.py`

 * *Files 19% similar despite different names*

```diff
@@ -41,23 +41,49 @@
         os_type = self._os_type
         # For Mac ARM CPUs after version 106.0.5249.61 the format of OS type changed
         # to more unified "mac_arm64". For newer versions, it'll be "mac_arm64"
         # by default, for lower versions we replace "mac_arm64" to old format - "mac64_m1".
         if version.parse(driver_version_to_download) < version.parse("106.0.5249.61"):
             os_type = os_type.replace("mac_arm64", "mac64_m1")
 
+        if version.parse(driver_version_to_download) >= version.parse("113"):
+            if os_type == "mac64":
+                os_type = "mac-x64"
+            if os_type in ["mac_64", "mac64_m1", "mac_arm64"]:
+                os_type = "mac-arm64"
+
+            modern_version_url = self.get_url_for_version_and_platform(driver_version_to_download, os_type)
+            log(f"Modern chrome version {modern_version_url}")
+            return modern_version_url
+
         return f"{self._url}/{driver_version_to_download}/{self.get_name()}_{os_type}.zip"
 
     def get_browser_type(self):
         return self._browser_type
 
     def get_latest_release_version(self):
         determined_browser_version = self.get_browser_version_from_os()
-
         log(f"Get LATEST {self._name} version for {self._browser_type}")
+        if version.parse(determined_browser_version) >= version.parse("113"):
+            return determined_browser_version
+
         latest_release_url = (
             self._latest_release_url
             if (self._version == "latest" or determined_browser_version is None)
             else f"{self._latest_release_url}_{determined_browser_version}"
         )
         resp = self._http_client.get(url=latest_release_url)
         return resp.text.rstrip()
+
+    def get_url_for_version_and_platform(self, browser_version, platform):
+        url = "https://googlechromelabs.github.io/chrome-for-testing/known-good-versions-with-downloads.json"
+        response = self._http_client.get(url)
+        data = response.json()
+        versions = data["versions"]
+        for v in versions:
+            if v["version"] == browser_version:
+                downloads = v["downloads"]["chromedriver"]
+                for d in downloads:
+                    if d["platform"] == platform:
+                        return d["url"]
+
+        raise Exception(f"No such driver version {browser_version} for {platform}")
```

### Comparing `webdriver_manager-3.8.6/webdriver_manager/drivers/edge.py` & `webdriver_manager-3.9.0/webdriver_manager/drivers/edge.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/webdriver_manager/drivers/firefox.py` & `webdriver_manager-3.9.0/webdriver_manager/drivers/firefox.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/webdriver_manager/drivers/ie.py` & `webdriver_manager-3.9.0/webdriver_manager/drivers/ie.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/webdriver_manager/drivers/opera.py` & `webdriver_manager-3.9.0/webdriver_manager/drivers/opera.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/webdriver_manager/firefox.py` & `webdriver_manager-3.9.0/webdriver_manager/firefox.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/webdriver_manager/microsoft.py` & `webdriver_manager-3.9.0/webdriver_manager/microsoft.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/webdriver_manager/opera.py` & `webdriver_manager-3.9.0/webdriver_manager/opera.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.6/webdriver_manager.egg-info/PKG-INFO` & `webdriver_manager-3.9.0/webdriver_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdriver-manager
-Version: 3.8.6
+Version: 3.9.0
 Summary: Library provides the way to automatically manage drivers for different browsers
 Home-page: https://github.com/SergeyPirogov/webdriver_manager
 Author: Sergey Pirogov
 Author-email: automationremarks@gmail.com
 Keywords: testing,selenium,driver,test automation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Information Technology
```

