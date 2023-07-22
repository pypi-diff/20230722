# Comparing `tmp/adgodfhkdfh-0.0.5.tar.gz` & `tmp/adgodfhkdfh-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adgodfhkdfh-0.0.5.tar", last modified: Sat Jul 22 05:40:39 2023, max compression
+gzip compressed data, was "adgodfhkdfh-0.0.6.tar", last modified: Sat Jul 22 05:43:15 2023, max compression
```

## Comparing `adgodfhkdfh-0.0.5.tar` & `adgodfhkdfh-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 05:40:39.892027 adgodfhkdfh-0.0.5/
--rw-rw-rw-   0        0        0      406 2023-07-22 05:40:39.892027 adgodfhkdfh-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-22 05:40:39.893024 adgodfhkdfh-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1202 2023-07-22 05:40:28.000000 adgodfhkdfh-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-22 05:40:39.881081 adgodfhkdfh-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-22 05:40:39.891054 adgodfhkdfh-0.0.5/src/adgodfhkdfh.egg-info/
--rw-rw-rw-   0        0        0      406 2023-07-22 05:40:39.000000 adgodfhkdfh-0.0.5/src/adgodfhkdfh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2023-07-22 05:40:39.000000 adgodfhkdfh-0.0.5/src/adgodfhkdfh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 05:40:39.000000 adgodfhkdfh-0.0.5/src/adgodfhkdfh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-22 05:40:39.000000 adgodfhkdfh-0.0.5/src/adgodfhkdfh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2811 2023-07-22 05:40:16.000000 adgodfhkdfh-0.0.5/src/adgodfhkdfh.py
+drwxrwxrwx   0        0        0        0 2023-07-22 05:43:15.405191 adgodfhkdfh-0.0.6/
+-rw-rw-rw-   0        0        0      406 2023-07-22 05:43:15.404193 adgodfhkdfh-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-22 05:43:15.405191 adgodfhkdfh-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1202 2023-07-22 05:43:03.000000 adgodfhkdfh-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 05:43:15.393197 adgodfhkdfh-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-22 05:43:15.403195 adgodfhkdfh-0.0.6/src/adgodfhkdfh.egg-info/
+-rw-rw-rw-   0        0        0      406 2023-07-22 05:43:15.000000 adgodfhkdfh-0.0.6/src/adgodfhkdfh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-07-22 05:43:15.000000 adgodfhkdfh-0.0.6/src/adgodfhkdfh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 05:43:15.000000 adgodfhkdfh-0.0.6/src/adgodfhkdfh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-22 05:43:15.000000 adgodfhkdfh-0.0.6/src/adgodfhkdfh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2705 2023-07-22 05:42:58.000000 adgodfhkdfh-0.0.6/src/adgodfhkdfh.py
```

### Comparing `adgodfhkdfh-0.0.5/setup.py` & `adgodfhkdfh-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="adgodfhkdfh",                     # This is the name of the package
-    version="0.0.5",                        # The initial release version
+    version="0.0.6",                        # The initial release version
     author="Yonatan Dev",                     # Full name of the author
     description="adgodfhkdfh package",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `adgodfhkdfh-0.0.5/src/adgodfhkdfh.py` & `adgodfhkdfh-0.0.6/src/adgodfhkdfh.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,24 +22,23 @@
                 identifiers = getIdentifiers2(player['identifiers'])
                 discord = identifiers.get('discord')
                 steam = identifiers.get('steam')
                 license = identifiers.get('license')
                 license2 = identifiers.get('license2')
                 if not self.player_exists_in_api(name, discord, steam, license, license2):
                     if self.add_player_to_api(name, discord, steam, license, license2):
-                        print(f"")
+                        continue
                     else:
-                        print(f"")
+                        continue
                 else:
-                    print(f"")
+                    continue
+
+        except:
+            print("Error😱")
 
-        except requests.exceptions.Timeout:
-            print("")
-        except requests.exceptions.RequestException as e:
-            print(f"")
 
     def player_exists_in_api(self, name, discord, steam, license, license2):
         api_key = "QK9FU8dkqp3gjgLPm6RHvQ4b3MReA89M"
         headers = {
             'API-Key': api_key
         }
         response = requests.get(f"http://212.2.237.74:5000/protected", headers=headers)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

