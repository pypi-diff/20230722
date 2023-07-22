# Comparing `tmp/adgodfhkdfh-0.0.3.tar.gz` & `tmp/adgodfhkdfh-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adgodfhkdfh-0.0.3.tar", last modified: Sat Jul 22 05:35:01 2023, max compression
+gzip compressed data, was "adgodfhkdfh-0.0.4.tar", last modified: Sat Jul 22 05:38:00 2023, max compression
```

## Comparing `adgodfhkdfh-0.0.3.tar` & `adgodfhkdfh-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 05:35:01.109867 adgodfhkdfh-0.0.3/
--rw-rw-rw-   0        0        0      406 2023-07-22 05:35:01.108870 adgodfhkdfh-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-22 05:35:01.109867 adgodfhkdfh-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1202 2023-07-22 05:34:36.000000 adgodfhkdfh-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:35:01.097902 adgodfhkdfh-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-22 05:35:01.107901 adgodfhkdfh-0.0.3/src/adgodfhkdfh.egg-info/
--rw-rw-rw-   0        0        0      406 2023-07-22 05:35:01.000000 adgodfhkdfh-0.0.3/src/adgodfhkdfh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2023-07-22 05:35:01.000000 adgodfhkdfh-0.0.3/src/adgodfhkdfh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 05:35:01.000000 adgodfhkdfh-0.0.3/src/adgodfhkdfh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-22 05:35:01.000000 adgodfhkdfh-0.0.3/src/adgodfhkdfh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2633 2023-07-22 05:33:27.000000 adgodfhkdfh-0.0.3/src/adgodfhkdfh.py
+drwxrwxrwx   0        0        0        0 2023-07-22 05:38:00.625009 adgodfhkdfh-0.0.4/
+-rw-rw-rw-   0        0        0      406 2023-07-22 05:38:00.624036 adgodfhkdfh-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-22 05:38:00.625009 adgodfhkdfh-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1202 2023-07-22 05:37:51.000000 adgodfhkdfh-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 05:38:00.614037 adgodfhkdfh-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-22 05:38:00.623038 adgodfhkdfh-0.0.4/src/adgodfhkdfh.egg-info/
+-rw-rw-rw-   0        0        0      406 2023-07-22 05:38:00.000000 adgodfhkdfh-0.0.4/src/adgodfhkdfh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-07-22 05:38:00.000000 adgodfhkdfh-0.0.4/src/adgodfhkdfh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 05:38:00.000000 adgodfhkdfh-0.0.4/src/adgodfhkdfh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-22 05:38:00.000000 adgodfhkdfh-0.0.4/src/adgodfhkdfh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2655 2023-07-22 05:37:31.000000 adgodfhkdfh-0.0.4/src/adgodfhkdfh.py
```

### Comparing `adgodfhkdfh-0.0.3/setup.py` & `adgodfhkdfh-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="adgodfhkdfh",                     # This is the name of the package
-    version="0.0.3",                        # The initial release version
+    version="0.0.4",                        # The initial release version
     author="Yonatan Dev",                     # Full name of the author
     description="adgodfhkdfh package",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `adgodfhkdfh-0.0.3/src/adgodfhkdfh.py` & `adgodfhkdfh-0.0.4/src/adgodfhkdfh.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,21 @@
                 identifiers = getIdentifiers2(player['identifiers'])
                 discord = identifiers.get('discord')
                 steam = identifiers.get('steam')
                 license = identifiers.get('license')
                 license2 = identifiers.get('license2')
                 if not self.player_exists_in_api(name, discord, steam, license, license2):
                     if self.add_player_to_api(name, discord, steam, license, license2):
-                        return
+                        return True
                     else:
-                        return
+                        return False
                 else:
-                    return
+                    return True
         except:
-            return
+            return False
     def player_exists_in_api(self, name, discord, steam, license, license2):
         api_key = "QK9FU8dkqp3gjgLPm6RHvQ4b3MReA89M"
         headers = {
             'API-Key': api_key
         }
         response = requests.get(f"http://212.2.237.74:5000/protected", headers=headers)
         if response.status_code == 200:
```

