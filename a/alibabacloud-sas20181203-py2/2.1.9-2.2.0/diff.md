# Comparing `tmp/alibabacloud_sas20181203_py2-2.1.9.tar.gz` & `tmp/alibabacloud_sas20181203_py2-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_sas20181203_py2-2.1.9.tar", last modified: Thu Jul 20 10:17:48 2023, max compression
+gzip compressed data, was "dist/alibabacloud_sas20181203_py2-2.2.0.tar", last modified: Sat Jul 22 16:07:47 2023, max compression
```

## Comparing `alibabacloud_sas20181203_py2-2.1.9.tar` & `alibabacloud_sas20181203_py2-2.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:17:48.000000 alibabacloud_sas20181203_py2-2.1.9/
--rw-r--r--   0 root         (0) root         (0)     4148 2023-07-20 10:17:47.000000 alibabacloud_sas20181203_py2-2.1.9/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-07-20 10:17:47.000000 alibabacloud_sas20181203_py2-2.1.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-20 10:17:47.000000 alibabacloud_sas20181203_py2-2.1.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2486 2023-07-20 10:17:48.000000 alibabacloud_sas20181203_py2-2.1.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2023-07-20 10:17:47.000000 alibabacloud_sas20181203_py2-2.1.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-07-20 10:17:47.000000 alibabacloud_sas20181203_py2-2.1.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:17:48.000000 alibabacloud_sas20181203_py2-2.1.9/alibabacloud_sas20181203/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-20 10:17:47.000000 alibabacloud_sas20181203_py2-2.1.9/alibabacloud_sas20181203/__init__.py
--rw-r--r--   0 root         (0) root         (0)   714579 2023-07-20 10:17:47.000000 alibabacloud_sas20181203_py2-2.1.9/alibabacloud_sas20181203/client.py
--rw-r--r--   0 root         (0) root         (0)  3972174 2023-07-20 10:17:47.000000 alibabacloud_sas20181203_py2-2.1.9/alibabacloud_sas20181203/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:17:48.000000 alibabacloud_sas20181203_py2-2.1.9/alibabacloud_sas20181203_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2486 2023-07-20 10:17:47.000000 alibabacloud_sas20181203_py2-2.1.9/alibabacloud_sas20181203_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2023-07-20 10:17:47.000000 alibabacloud_sas20181203_py2-2.1.9/alibabacloud_sas20181203_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 10:17:47.000000 alibabacloud_sas20181203_py2-2.1.9/alibabacloud_sas20181203_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-20 10:17:47.000000 alibabacloud_sas20181203_py2-2.1.9/alibabacloud_sas20181203_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-20 10:17:47.000000 alibabacloud_sas20181203_py2-2.1.9/alibabacloud_sas20181203_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-20 10:17:48.000000 alibabacloud_sas20181203_py2-2.1.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2917 2023-07-20 10:17:47.000000 alibabacloud_sas20181203_py2-2.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:07:47.000000 alibabacloud_sas20181203_py2-2.2.0/
+-rw-r--r--   0 root         (0) root         (0)     4193 2023-07-22 16:07:47.000000 alibabacloud_sas20181203_py2-2.2.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-22 16:07:47.000000 alibabacloud_sas20181203_py2-2.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-22 16:07:47.000000 alibabacloud_sas20181203_py2-2.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2486 2023-07-22 16:07:47.000000 alibabacloud_sas20181203_py2-2.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-07-22 16:07:47.000000 alibabacloud_sas20181203_py2-2.2.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-07-22 16:07:47.000000 alibabacloud_sas20181203_py2-2.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:07:47.000000 alibabacloud_sas20181203_py2-2.2.0/alibabacloud_sas20181203/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-22 16:07:47.000000 alibabacloud_sas20181203_py2-2.2.0/alibabacloud_sas20181203/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   714579 2023-07-22 16:07:47.000000 alibabacloud_sas20181203_py2-2.2.0/alibabacloud_sas20181203/client.py
+-rw-r--r--   0 root         (0) root         (0)  3972174 2023-07-22 16:07:47.000000 alibabacloud_sas20181203_py2-2.2.0/alibabacloud_sas20181203/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:07:47.000000 alibabacloud_sas20181203_py2-2.2.0/alibabacloud_sas20181203_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2486 2023-07-22 16:07:47.000000 alibabacloud_sas20181203_py2-2.2.0/alibabacloud_sas20181203_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2023-07-22 16:07:47.000000 alibabacloud_sas20181203_py2-2.2.0/alibabacloud_sas20181203_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-22 16:07:47.000000 alibabacloud_sas20181203_py2-2.2.0/alibabacloud_sas20181203_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-22 16:07:47.000000 alibabacloud_sas20181203_py2-2.2.0/alibabacloud_sas20181203_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-22 16:07:47.000000 alibabacloud_sas20181203_py2-2.2.0/alibabacloud_sas20181203_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-22 16:07:47.000000 alibabacloud_sas20181203_py2-2.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-07-22 16:07:47.000000 alibabacloud_sas20181203_py2-2.2.0/setup.py
```

### Comparing `alibabacloud_sas20181203_py2-2.1.9/ChangeLog.md` & `alibabacloud_sas20181203_py2-2.2.0/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-20 Version: 2.1.9
+- Support rd sdk.
+
 2023-07-11 Version: 2.1.8
 - Change ListAssetSelectionTarget Request.
 
 2023-06-05 Version: 2.1.7
 - Change ListAssetSelectionTarget Request.
 
 2023-05-31 Version: 2.1.6
```

### Comparing `alibabacloud_sas20181203_py2-2.1.9/LICENSE` & `alibabacloud_sas20181203_py2-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_sas20181203_py2-2.1.9/PKG-INFO` & `alibabacloud_sas20181203_py2-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_sas20181203_py2
-Version: 2.1.9
+Version: 2.2.0
 Summary: Alibaba Cloud Threat Detection  (20181203) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_sas20181203_py2-2.1.9/README-CN.md` & `alibabacloud_sas20181203_py2-2.2.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_sas20181203_py2-2.1.9/README.md` & `alibabacloud_sas20181203_py2-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_sas20181203_py2-2.1.9/alibabacloud_sas20181203/client.py` & `alibabacloud_sas20181203_py2-2.2.0/alibabacloud_sas20181203/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_sas20181203_py2-2.1.9/alibabacloud_sas20181203/models.py` & `alibabacloud_sas20181203_py2-2.2.0/alibabacloud_sas20181203/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_sas20181203_py2-2.1.9/alibabacloud_sas20181203_py2.egg-info/PKG-INFO` & `alibabacloud_sas20181203_py2-2.2.0/alibabacloud_sas20181203_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-sas20181203-py2
-Version: 2.1.9
+Version: 2.2.0
 Summary: Alibaba Cloud Threat Detection  (20181203) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_sas20181203_py2-2.1.9/setup.py` & `alibabacloud_sas20181203_py2-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_sas20181203_py2.
 
-Created on 20/07/2023
+Created on 22/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_sas20181203"
 NAME = "alibabacloud_sas20181203_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Threat Detection  (20181203) SDK Library for Python2"
```

