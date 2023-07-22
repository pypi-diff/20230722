# Comparing `tmp/degiro-cli-0.1.0.tar.gz` & `tmp/degiro-cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degiro-cli-0.1.0.tar", last modified: Sat Jul 22 11:54:48 2023, max compression
+gzip compressed data, was "degiro-cli-0.1.1.tar", last modified: Sat Jul 22 11:59:57 2023, max compression
```

## Comparing `degiro-cli-0.1.0.tar` & `degiro-cli-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 11:54:48.916509 degiro-cli-0.1.0/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1075 2023-07-22 11:48:36.000000 degiro-cli-0.1.0/LICENSE
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     7463 2023-07-22 11:54:48.912509 degiro-cli-0.1.0/PKG-INFO
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     6816 2023-07-22 11:39:55.000000 degiro-cli-0.1.0/README.md
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 11:54:48.912509 degiro-cli-0.1.0/bin/
--rwxrw-r--   0 laumas    (1000) laumas    (1000)      152 2023-07-22 09:17:36.000000 degiro-cli-0.1.0/bin/degiro-history
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      148 2023-07-22 09:17:43.000000 degiro-cli-0.1.0/bin/degiro-login
--rw-rw-r--   0 laumas    (1000) laumas    (1000)        0 2023-07-07 09:16:27.000000 degiro-cli-0.1.0/bin/degiro-logout
--rw-rw-r--   0 laumas    (1000) laumas    (1000)        0 2023-07-07 09:16:32.000000 degiro-cli-0.1.0/bin/degiro-portfolio
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      150 2023-07-22 09:17:55.000000 degiro-cli-0.1.0/bin/degiro-search
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 11:54:48.912509 degiro-cli-0.1.0/degiro_cli.egg-info/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     7463 2023-07-22 11:54:48.000000 degiro-cli-0.1.0/degiro_cli.egg-info/PKG-INFO
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      303 2023-07-22 11:54:48.000000 degiro-cli-0.1.0/degiro_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)        1 2023-07-22 11:54:48.000000 degiro-cli-0.1.0/degiro_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)       94 2023-07-22 11:54:48.000000 degiro-cli-0.1.0/degiro_cli.egg-info/requires.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)        1 2023-07-22 11:54:48.000000 degiro-cli-0.1.0/degiro_cli.egg-info/top_level.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      108 2023-07-22 11:52:04.000000 degiro-cli-0.1.0/pyproject.toml
--rw-rw-r--   0 laumas    (1000) laumas    (1000)       38 2023-07-22 11:54:48.916509 degiro-cli-0.1.0/setup.cfg
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     2108 2023-07-22 11:46:27.000000 degiro-cli-0.1.0/setup.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 11:59:57.559414 degiro-cli-0.1.1/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1075 2023-07-22 11:48:36.000000 degiro-cli-0.1.1/LICENSE
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     7485 2023-07-22 11:59:57.559414 degiro-cli-0.1.1/PKG-INFO
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     6827 2023-07-22 11:58:06.000000 degiro-cli-0.1.1/README.md
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 11:59:57.559414 degiro-cli-0.1.1/bin/
+-rwxrw-r--   0 laumas    (1000) laumas    (1000)      152 2023-07-22 09:17:36.000000 degiro-cli-0.1.1/bin/degiro-history
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      148 2023-07-22 09:17:43.000000 degiro-cli-0.1.1/bin/degiro-login
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)        0 2023-07-07 09:16:27.000000 degiro-cli-0.1.1/bin/degiro-logout
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)        0 2023-07-07 09:16:32.000000 degiro-cli-0.1.1/bin/degiro-portfolio
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      150 2023-07-22 09:17:55.000000 degiro-cli-0.1.1/bin/degiro-search
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-22 11:59:57.559414 degiro-cli-0.1.1/degiro_cli.egg-info/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     7485 2023-07-22 11:59:57.000000 degiro-cli-0.1.1/degiro_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      303 2023-07-22 11:59:57.000000 degiro-cli-0.1.1/degiro_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)        1 2023-07-22 11:59:57.000000 degiro-cli-0.1.1/degiro_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)       94 2023-07-22 11:59:57.000000 degiro-cli-0.1.1/degiro_cli.egg-info/requires.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)        1 2023-07-22 11:59:57.000000 degiro-cli-0.1.1/degiro_cli.egg-info/top_level.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      108 2023-07-22 11:52:04.000000 degiro-cli-0.1.1/pyproject.toml
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)       38 2023-07-22 11:59:57.559414 degiro-cli-0.1.1/setup.cfg
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     2119 2023-07-22 11:58:29.000000 degiro-cli-0.1.1/setup.py
```

### Comparing `degiro-cli-0.1.0/LICENSE` & `degiro-cli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `degiro-cli-0.1.0/PKG-INFO` & `degiro-cli-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: degiro-cli
-Version: 0.1.0
-Summary: Command line tools for Degiro
+Version: 0.1.1
+Summary: Unofficial command line tools for Degiro
 Home-page: https://github.com/OhMajesticLama/degiro-cli
 Author-email: ohmajesticlama@gmail.com
 Project-URL: Documentation, https://ohmajesticlama.github.io/degiro-cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -26,15 +26,15 @@
 
 At this stage, it does not allow to monitor portfolio, access, place or cancel
 orders.
 
 ## Installation
 
 ``` sh
-pip3 install degirocli
+pip3 install degiro-cli
 ```
 
 ## Use
 All outputs are in CSV format. If needed, take a look at command line CSV
 manipulation tools such as [CSV Kit](https://csvkit.rtfd.org/). Especially
 the `csvlook` command if you intend to just visualize outputes from command
 line.
@@ -146,15 +146,15 @@
 # EPA,SAF,Safran,EUR,FR0000073272
 # EPA,EL,Essilor,EUR,FR0000121667
 # IRL,CRG,CRH PLC,EUR,IE0001827041
 # EPA,VIV,Vivendi,EUR,FR0000127771
 
 ```
 
-## By Index
+## Get symbol history
 ``` sh
 degiro-history --period 1m EPA.SAF
 # exchange,symbol,date,currency,open,high,low,close
 # EPA,SAF,2023-06-22T00:00:00,EUR,141.2,141.2,138.84,140.06
 # EPA,SAF,2023-06-23T00:00:00,EUR,139.12,140.24,138.02,139.48
 # EPA,SAF,2023-06-26T00:00:00,EUR,139.98,140.26,137.18,139.16
 # EPA,SAF,2023-06-27T00:00:00,EUR,139.3,140.0,138.38,139.62
```

### Comparing `degiro-cli-0.1.0/README.md` & `degiro-cli-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 At this stage, it does not allow to monitor portfolio, access, place or cancel
 orders.
 
 ## Installation
 
 ``` sh
-pip3 install degirocli
+pip3 install degiro-cli
 ```
 
 ## Use
 All outputs are in CSV format. If needed, take a look at command line CSV
 manipulation tools such as [CSV Kit](https://csvkit.rtfd.org/). Especially
 the `csvlook` command if you intend to just visualize outputes from command
 line.
@@ -129,15 +129,15 @@
 # EPA,SAF,Safran,EUR,FR0000073272
 # EPA,EL,Essilor,EUR,FR0000121667
 # IRL,CRG,CRH PLC,EUR,IE0001827041
 # EPA,VIV,Vivendi,EUR,FR0000127771
 
 ```
 
-## By Index
+## Get symbol history
 ``` sh
 degiro-history --period 1m EPA.SAF
 # exchange,symbol,date,currency,open,high,low,close
 # EPA,SAF,2023-06-22T00:00:00,EUR,141.2,141.2,138.84,140.06
 # EPA,SAF,2023-06-23T00:00:00,EUR,139.12,140.24,138.02,139.48
 # EPA,SAF,2023-06-26T00:00:00,EUR,139.98,140.26,137.18,139.16
 # EPA,SAF,2023-06-27T00:00:00,EUR,139.3,140.0,138.38,139.62
```

### Comparing `degiro-cli-0.1.0/degiro_cli.egg-info/PKG-INFO` & `degiro-cli-0.1.1/degiro_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: degiro-cli
-Version: 0.1.0
-Summary: Command line tools for Degiro
+Version: 0.1.1
+Summary: Unofficial command line tools for Degiro
 Home-page: https://github.com/OhMajesticLama/degiro-cli
 Author-email: ohmajesticlama@gmail.com
 Project-URL: Documentation, https://ohmajesticlama.github.io/degiro-cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -26,15 +26,15 @@
 
 At this stage, it does not allow to monitor portfolio, access, place or cancel
 orders.
 
 ## Installation
 
 ``` sh
-pip3 install degirocli
+pip3 install degiro-cli
 ```
 
 ## Use
 All outputs are in CSV format. If needed, take a look at command line CSV
 manipulation tools such as [CSV Kit](https://csvkit.rtfd.org/). Especially
 the `csvlook` command if you intend to just visualize outputes from command
 line.
@@ -146,15 +146,15 @@
 # EPA,SAF,Safran,EUR,FR0000073272
 # EPA,EL,Essilor,EUR,FR0000121667
 # IRL,CRG,CRH PLC,EUR,IE0001827041
 # EPA,VIV,Vivendi,EUR,FR0000127771
 
 ```
 
-## By Index
+## Get symbol history
 ``` sh
 degiro-history --period 1m EPA.SAF
 # exchange,symbol,date,currency,open,high,low,close
 # EPA,SAF,2023-06-22T00:00:00,EUR,141.2,141.2,138.84,140.06
 # EPA,SAF,2023-06-23T00:00:00,EUR,139.12,140.24,138.02,139.48
 # EPA,SAF,2023-06-26T00:00:00,EUR,139.98,140.26,137.18,139.16
 # EPA,SAF,2023-06-27T00:00:00,EUR,139.3,140.0,138.38,139.62
```

### Comparing `degiro-cli-0.1.0/setup.py` & `degiro-cli-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 import sys
 import os
 
 import setuptools
 
 
 if __name__ == '__main__':
-    description = "Command line tools for Degiro"
+    description = "Unofficial command line tools for Degiro"
     readme_path = os.path.join(os.path.dirname(__file__), 'README.md')
     with open(readme_path, "r") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name="degiro-cli",
-        version="0.1.0",
+        version="0.1.1",
         author_email="ohmajesticlama@gmail.com",
         description=description,
         long_description=long_description,
         long_description_content_type='text/markdown',
         url="https://github.com/OhMajesticLama/degiro-cli",
         project_urls={
             'Documentation':
```

