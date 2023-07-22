# Comparing `tmp/hoom-0.1.3.tar.gz` & `tmp/hoom-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoom-0.1.3.tar", max compression
+gzip compressed data, was "hoom-0.1.4.tar", max compression
```

## Comparing `hoom-0.1.3.tar` & `hoom-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    35149 2023-07-22 17:56:51.705601 hoom-0.1.3/LICENSE
--rw-r--r--   0        0        0     1453 2023-07-22 17:56:51.705601 hoom-0.1.3/README.md
--rw-r--r--   0        0        0       21 2023-07-22 17:56:51.705601 hoom-0.1.3/hoom/__init__.py
--rw-r--r--   0        0        0      737 2023-07-22 17:56:51.705601 hoom-0.1.3/hoom/accessory_types/Lightbulb.py
--rw-r--r--   0        0        0      785 2023-07-22 17:56:51.705601 hoom-0.1.3/hoom/accessory_types/TemperatureSensor.py
--rw-r--r--   0        0        0       57 2023-07-22 17:56:51.705601 hoom-0.1.3/hoom/accessory_types/__init__.py
--rw-r--r--   0        0        0     1880 2023-07-22 17:56:51.705601 hoom-0.1.3/hoom/bridge.py
--rw-r--r--   0        0        0   232868 2023-07-22 17:56:51.709601 hoom-0.1.3/hoom/pages/assets/bootstrap/css/bootstrap.min.css
--rw-r--r--   0        0        0    80373 2023-07-22 17:56:51.709601 hoom-0.1.3/hoom/pages/assets/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0      314 2023-07-22 17:56:51.709601 hoom-0.1.3/hoom/pages/assets/img/error.png
--rw-r--r--   0        0        0    89501 2023-07-22 17:56:51.709601 hoom-0.1.3/hoom/pages/assets/js/jquery.min.js
--rw-r--r--   0        0        0    19927 2023-07-22 17:56:51.709601 hoom-0.1.3/hoom/pages/assets/js/qrcode.min.js
--rw-r--r--   0        0        0     7653 2023-07-22 17:56:51.709601 hoom-0.1.3/hoom/pages/connect.html
--rw-r--r--   0        0        0      938 2023-07-22 17:56:51.709601 hoom-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2660 1970-01-01 00:00:00.000000 hoom-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-22 21:53:10.649759 hoom-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1555 2023-07-22 21:53:10.649759 hoom-0.1.4/README.md
+-rw-r--r--   0        0        0       21 2023-07-22 21:53:10.649759 hoom-0.1.4/hoom/__init__.py
+-rw-r--r--   0        0        0      737 2023-07-22 21:53:10.649759 hoom-0.1.4/hoom/accessory_types/Lightbulb.py
+-rw-r--r--   0        0        0      785 2023-07-22 21:53:10.649759 hoom-0.1.4/hoom/accessory_types/TemperatureSensor.py
+-rw-r--r--   0        0        0       57 2023-07-22 21:53:10.649759 hoom-0.1.4/hoom/accessory_types/__init__.py
+-rw-r--r--   0        0        0     5600 2023-07-22 21:53:10.649759 hoom-0.1.4/hoom/bridge.py
+-rw-r--r--   0        0        0   232868 2023-07-22 21:53:10.649759 hoom-0.1.4/hoom/pages/assets/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0        0        0    80373 2023-07-22 21:53:10.649759 hoom-0.1.4/hoom/pages/assets/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0      314 2023-07-22 21:53:10.649759 hoom-0.1.4/hoom/pages/assets/img/error.png
+-rw-r--r--   0        0        0    89501 2023-07-22 21:53:10.649759 hoom-0.1.4/hoom/pages/assets/js/jquery.min.js
+-rw-r--r--   0        0        0    19927 2023-07-22 21:53:10.649759 hoom-0.1.4/hoom/pages/assets/js/qrcode.min.js
+-rw-r--r--   0        0        0     4412 2023-07-22 21:53:10.649759 hoom-0.1.4/hoom/pages/connect.html
+-rw-r--r--   0        0        0      938 2023-07-22 21:53:10.649759 hoom-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 hoom-0.1.4/PKG-INFO
```

### Comparing `hoom-0.1.3/LICENSE` & `hoom-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hoom-0.1.3/README.md` & `hoom-0.1.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,14 @@
-<h1 align="center">🏡 Hoom</h1>
-<p align="center">Build your own HomeKit Bridge & Accessories with Hoom</p>
+<img src="https://bcdn.berrysauce.me/shared/hoom-banner-modified.png">
+<img src="https://bcdn.berrysauce.me/shared/hoom-ad-modified.png">
+
+<br>
+
+# 🏡 Hoom
+Build your own HomeKit Bridge & Accessories with Hoom
 
 ### ✨ Features
 - [x] HomeKit Bridge
 - [x] Minimalist Web UI
 - [x] Create custom HomeKit Accessories with function decorators
 - [x] Customizable
 - [x] Easy to use
@@ -40,8 +45,8 @@
 
 As you can see, Hoom is very similar to frameworks like FastAPI. No need for complicated classes with lots of methods. Just use the `@hoom.accessory` decorator and you're good to go.
 
 ### 📣 Credits
 A special thanks goes out to these Python packages/frameworks and their authors:
 
 - [HAP-python](https://github.com/ikalchev/HAP-python) - Hoom wouldn't be possible without this HomeKit Accessory Protocol implementation by [Ivan Kalchev](https://github.com/ikalchev)
-- [FastAPI](https://github.com/tiangolo/fastapi) - Hoom uses FastAPI by [Sebastián Ramírez](https://github.com/tiangolo) for its web server & UI and is heavily inspired by it
+- [FastAPI](https://github.com/tiangolo/fastapi) - Hoom uses FastAPI by [Sebastián Ramírez](https://github.com/tiangolo) for its web server & UI and is heavily inspired by it
```

### Comparing `hoom-0.1.3/hoom/accessory_types/Lightbulb.py` & `hoom-0.1.4/hoom/accessory_types/Lightbulb.py`

 * *Files identical despite different names*

### Comparing `hoom-0.1.3/hoom/accessory_types/TemperatureSensor.py` & `hoom-0.1.4/hoom/accessory_types/TemperatureSensor.py`

 * *Files identical despite different names*

### Comparing `hoom-0.1.3/hoom/pages/assets/bootstrap/css/bootstrap.min.css` & `hoom-0.1.4/hoom/pages/assets/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hoom-0.1.3/hoom/pages/assets/bootstrap/js/bootstrap.min.js` & `hoom-0.1.4/hoom/pages/assets/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hoom-0.1.3/hoom/pages/assets/js/jquery.min.js` & `hoom-0.1.4/hoom/pages/assets/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `hoom-0.1.3/hoom/pages/assets/js/qrcode.min.js` & `hoom-0.1.4/hoom/pages/assets/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `hoom-0.1.3/pyproject.toml` & `hoom-0.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoom"
-version = "0.1.3"
+version = "0.1.4"
 description = "Build your own HomeKit Bridge & Accessories with Hoom"
 authors = ["Paul Haedrich <hey@foerstal.com>"]
 readme = "README.md"
 license = "GPL-3.0-only"
 homepage = "https://github.com/berrysauce/hoom"
 repository = "https://github.com/berrysauce/hoom"
 documentation = "https://github.com/berrysauce/hoom"
```

### Comparing `hoom-0.1.3/PKG-INFO` & `hoom-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoom
-Version: 0.1.3
+Version: 0.1.4
 Summary: Build your own HomeKit Bridge & Accessories with Hoom
 Home-page: https://github.com/berrysauce/hoom
 License: GPL-3.0-only
 Author: Paul Haedrich
 Author-email: hey@foerstal.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -24,16 +24,21 @@
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pyqrcode (>=1.2.1,<2.0.0)
 Requires-Dist: uvicorn (>=0.23.1,<0.24.0)
 Project-URL: Documentation, https://github.com/berrysauce/hoom
 Project-URL: Repository, https://github.com/berrysauce/hoom
 Description-Content-Type: text/markdown
 
-<h1 align="center">🏡 Hoom</h1>
-<p align="center">Build your own HomeKit Bridge & Accessories with Hoom</p>
+<img src="https://bcdn.berrysauce.me/shared/hoom-banner-modified.png">
+<img src="https://bcdn.berrysauce.me/shared/hoom-ad-modified.png">
+
+<br>
+
+# 🏡 Hoom
+Build your own HomeKit Bridge & Accessories with Hoom
 
 ### ✨ Features
 - [x] HomeKit Bridge
 - [x] Minimalist Web UI
 - [x] Create custom HomeKit Accessories with function decorators
 - [x] Customizable
 - [x] Easy to use
@@ -71,7 +76,8 @@
 As you can see, Hoom is very similar to frameworks like FastAPI. No need for complicated classes with lots of methods. Just use the `@hoom.accessory` decorator and you're good to go.
 
 ### 📣 Credits
 A special thanks goes out to these Python packages/frameworks and their authors:
 
 - [HAP-python](https://github.com/ikalchev/HAP-python) - Hoom wouldn't be possible without this HomeKit Accessory Protocol implementation by [Ivan Kalchev](https://github.com/ikalchev)
 - [FastAPI](https://github.com/tiangolo/fastapi) - Hoom uses FastAPI by [Sebastián Ramírez](https://github.com/tiangolo) for its web server & UI and is heavily inspired by it
+
```

