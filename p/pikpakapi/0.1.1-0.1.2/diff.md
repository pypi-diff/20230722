# Comparing `tmp/pikpakapi-0.1.1.tar.gz` & `tmp/pikpakapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikpakapi-0.1.1.tar", max compression
+gzip compressed data, was "pikpakapi-0.1.2.tar", max compression
```

## Comparing `pikpakapi-0.1.1.tar` & `pikpakapi-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0       72 2022-11-06 14:25:05.626706 pikpakapi-0.1.1/README.md
--rw-r--r--   0        0        0      307 2022-11-06 14:25:05.626706 pikpakapi-0.1.1/pikpakapi/PikpakException.py
--rw-r--r--   0        0        0    17231 2022-11-06 14:25:05.626706 pikpakapi-0.1.1/pikpakapi/__init__.py
--rw-r--r--   0        0        0      190 2022-11-06 14:25:05.626706 pikpakapi-0.1.1/pikpakapi/enums.py
--rw-r--r--   0        0        0      446 2022-11-06 14:25:05.626706 pikpakapi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 pikpakapi-0.1.1/setup.py
--rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 pikpakapi-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-07-22 17:30:22.790715 pikpakapi-0.1.2/README.md
+-rw-r--r--   0        0        0      307 2023-07-22 17:30:22.790715 pikpakapi-0.1.2/pikpakapi/PikpakException.py
+-rw-r--r--   0        0        0    17231 2023-07-22 17:30:22.790715 pikpakapi-0.1.2/pikpakapi/__init__.py
+-rw-r--r--   0        0        0      190 2023-07-22 17:30:22.790715 pikpakapi-0.1.2/pikpakapi/enums.py
+-rw-r--r--   0        0        0      448 2023-07-22 17:30:22.790715 pikpakapi-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 pikpakapi-0.1.2/PKG-INFO
```

### Comparing `pikpakapi-0.1.1/pikpakapi/__init__.py` & `pikpakapi-0.1.2/pikpakapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pikpakapi-0.1.1/PKG-INFO` & `pikpakapi-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pikpakapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: PikPakAPI
 Home-page: https://github.com/Quan666/PikPakAPI
 License: GPL-3.0-only
 Keywords: pikpak,api
 Author: Quan666
 Author-email: i@Rori.eMail
 Requires-Python: >=3.8.3,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: httpx (>=0.22.0,<0.23.0)
+Requires-Dist: httpx (>=0.24.1)
 Project-URL: Repository, https://github.com/Quan666/PikPakAPI
 Description-Content-Type: text/markdown
 
 # PikPakApi
 
 PikPak API Python 实现
```

