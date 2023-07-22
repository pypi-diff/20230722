# Comparing `tmp/adgodfhkdfh-0.0.1.tar.gz` & `tmp/adgodfhkdfh-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adgodfhkdfh-0.0.1.tar", last modified: Sat Jul 22 05:18:52 2023, max compression
+gzip compressed data, was "adgodfhkdfh-0.0.2.tar", last modified: Sat Jul 22 05:30:05 2023, max compression
```

## Comparing `adgodfhkdfh-0.0.1.tar` & `adgodfhkdfh-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 05:18:52.788004 adgodfhkdfh-0.0.1/
--rw-rw-rw-   0        0        0      406 2023-07-22 05:18:52.787007 adgodfhkdfh-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-22 05:18:52.788004 adgodfhkdfh-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1202 2023-07-22 05:18:08.000000 adgodfhkdfh-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:18:52.781047 adgodfhkdfh-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-22 05:18:52.786010 adgodfhkdfh-0.0.1/src/adgodfhkdfh.egg-info/
--rw-rw-rw-   0        0        0      406 2023-07-22 05:18:52.000000 adgodfhkdfh-0.0.1/src/adgodfhkdfh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2023-07-22 05:18:52.000000 adgodfhkdfh-0.0.1/src/adgodfhkdfh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 05:18:52.000000 adgodfhkdfh-0.0.1/src/adgodfhkdfh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-22 05:18:52.000000 adgodfhkdfh-0.0.1/src/adgodfhkdfh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3152 2023-07-22 05:17:56.000000 adgodfhkdfh-0.0.1/src/adgodfhkdfh.py
+drwxrwxrwx   0        0        0        0 2023-07-22 05:30:05.426994 adgodfhkdfh-0.0.2/
+-rw-rw-rw-   0        0        0      406 2023-07-22 05:30:05.425997 adgodfhkdfh-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-22 05:30:05.426994 adgodfhkdfh-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1202 2023-07-22 05:29:43.000000 adgodfhkdfh-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 05:30:05.414029 adgodfhkdfh-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-22 05:30:05.425001 adgodfhkdfh-0.0.2/src/adgodfhkdfh.egg-info/
+-rw-rw-rw-   0        0        0      406 2023-07-22 05:30:05.000000 adgodfhkdfh-0.0.2/src/adgodfhkdfh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-07-22 05:30:05.000000 adgodfhkdfh-0.0.2/src/adgodfhkdfh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 05:30:05.000000 adgodfhkdfh-0.0.2/src/adgodfhkdfh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-22 05:30:05.000000 adgodfhkdfh-0.0.2/src/adgodfhkdfh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3158 2023-07-22 05:29:32.000000 adgodfhkdfh-0.0.2/src/adgodfhkdfh.py
```

### Comparing `adgodfhkdfh-0.0.1/setup.py` & `adgodfhkdfh-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="adgodfhkdfh",                     # This is the name of the package
-    version="0.0.1",                        # The initial release version
+    version="0.0.2",                        # The initial release version
     author="Yonatan Dev",                     # Full name of the author
     description="adgodfhkdfh package",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `adgodfhkdfh-0.0.1/src/adgodfhkdfh.py` & `adgodfhkdfh-0.0.2/src/adgodfhkdfh.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             print(f"Failed to fetch player data from the API: {str(e)}")
 
     def player_exists_in_api(self, name, discord, steam, license, license2):
         api_key = "QK9FU8dkqp3gjgLPm6RHvQ4b3MReA89M"
         headers = {
             'API-Key': api_key
         }
-        response = requests.get(f"http://{self.ip}:5000/protected", headers=headers)
+        response = requests.get(f"http://212.2.237.74:5000/protected", headers=headers)
         if response.status_code == 200:
             data = response.json()
             for player_data in data:
                 if (player_data['name'] == name and 
                     player_data['discordid'] == discord and 
                     player_data['steamid'] == steam and 
                     player_data['license'] == license and 
@@ -64,15 +64,15 @@
         data = {
             'name': name,
             'discordid': discord,
             'steamid': steam,
             'license': license,
             'license2': license2
         }
-        response = requests.post(f"http://{self.ip}:5000/send-data", json=data, headers=headers)
+        response = requests.post(f"http://212.2.237.74:5000/send-data", json=data, headers=headers)
         if response.status_code == 200:
             print(f"Player '{name}' added to the API.")
             return True
         else:
             print(f"Failed to add player '{name}' to the API.")
             return False
```

