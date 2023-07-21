# Comparing `tmp/application_properties-0.8.0.tar.gz` & `tmp/application_properties-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "application_properties-0.8.0.tar", last modified: Sun Jul 16 21:53:09 2023, max compression
+gzip compressed data, was "application_properties-0.8.1.tar", last modified: Fri Jul 21 23:09:55 2023, max compression
```

## Comparing `application_properties-0.8.0.tar` & `application_properties-0.8.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 21:53:09.716650 application_properties-0.8.0/
--rw-rw-rw-   0        0        0     1066 2023-05-14 22:38:18.000000 application_properties-0.8.0/LICENSE.txt
--rw-rw-rw-   0        0        0      125 2023-07-16 16:33:32.000000 application_properties-0.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5862 2023-07-16 21:53:09.716650 application_properties-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     8311 2023-07-15 23:41:15.000000 application_properties-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 21:53:09.698560 application_properties-0.8.0/application_properties/
--rw-rw-rw-   0        0        0       13 2023-05-14 22:38:18.000000 application_properties-0.8.0/application_properties/.external-package
--rw-rw-rw-   0        0        0     1339 2023-07-16 21:17:57.000000 application_properties-0.8.0/application_properties/__init__.py
--rw-rw-rw-   0        0        0    17605 2023-07-16 03:47:33.000000 application_properties-0.8.0/application_properties/application_properties.py
--rw-rw-rw-   0        0        0     8126 2023-04-28 01:01:24.000000 application_properties-0.8.0/application_properties/application_properties_config_loader.py
--rw-rw-rw-   0        0        0     4911 2022-08-24 23:33:16.000000 application_properties-0.8.0/application_properties/application_properties_facade.py
--rw-rw-rw-   0        0        0     3048 2023-04-23 03:27:58.000000 application_properties-0.8.0/application_properties/application_properties_json_loader.py
--rw-rw-rw-   0        0        0      955 2023-04-23 03:26:29.000000 application_properties-0.8.0/application_properties/application_properties_loader_helper.py
--rw-rw-rw-   0        0        0     3566 2023-04-23 03:27:58.000000 application_properties-0.8.0/application_properties/application_properties_toml_loader.py
--rw-rw-rw-   0        0        0     4117 2023-07-16 21:41:04.000000 application_properties-0.8.0/application_properties/application_properties_utilities.py
--rw-rw-rw-   0        0        0     4555 2023-07-16 04:02:08.000000 application_properties-0.8.0/application_properties/application_properties_yaml_loader.py
--rw-rw-rw-   0        0        0       13 2023-05-14 22:38:18.000000 application_properties-0.8.0/application_properties/py.typed
--rw-rw-rw-   0        0        0      212 2023-07-16 21:40:50.000000 application_properties-0.8.0/application_properties/version.py
-drwxrwxrwx   0        0        0        0 2023-07-16 21:53:09.703559 application_properties-0.8.0/application_properties.egg-info/
--rw-rw-rw-   0        0        0     5862 2023-07-16 21:53:09.000000 application_properties-0.8.0/application_properties.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1368 2023-07-16 21:53:09.000000 application_properties-0.8.0/application_properties.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 21:53:09.000000 application_properties-0.8.0/application_properties.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-16 21:53:09.000000 application_properties-0.8.0/application_properties.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-16 21:53:09.000000 application_properties-0.8.0/application_properties.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       40 2023-07-15 15:07:10.000000 application_properties-0.8.0/install-requirements.txt
--rw-rw-rw-   0        0        0      798 2023-07-16 21:53:09.717650 application_properties-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     3084 2023-07-16 17:47:15.000000 application_properties-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 21:53:09.715774 application_properties-0.8.0/test/
--rw-rw-rw-   0        0        0    14171 2023-07-16 21:41:52.000000 application_properties-0.8.0/test/test_application_properties.py
--rw-rw-rw-   0        0        0    23586 2023-06-25 21:12:27.000000 application_properties-0.8.0/test/test_application_properties_config_loader.py
--rw-rw-rw-   0        0        0     8820 2023-06-25 20:38:43.000000 application_properties-0.8.0/test/test_application_properties_facade.py
--rw-rw-rw-   0        0        0    14361 2023-07-16 03:30:16.000000 application_properties-0.8.0/test/test_application_properties_json_loader.py
--rw-rw-rw-   0        0        0    23303 2023-06-25 21:14:32.000000 application_properties-0.8.0/test/test_application_properties_toml_loader.py
--rw-rw-rw-   0        0        0    20569 2023-07-15 19:12:59.000000 application_properties-0.8.0/test/test_application_properties_utilities.py
--rw-rw-rw-   0        0        0    24775 2023-07-16 03:36:04.000000 application_properties-0.8.0/test/test_application_properties_yaml_loader.py
--rw-rw-rw-   0        0        0     3917 2023-06-25 20:34:07.000000 application_properties-0.8.0/test/test_get_boolean.py
--rw-rw-rw-   0        0        0     3885 2023-06-25 20:34:32.000000 application_properties-0.8.0/test/test_get_integer.py
--rw-rw-rw-   0        0        0     6299 2023-06-25 20:58:42.000000 application_properties-0.8.0/test/test_get_string.py
--rw-rw-rw-   0        0        0    24741 2023-07-16 03:26:31.000000 application_properties-0.8.0/test/test_set_manual_property.py
--rw-rw-rw-   0        0        0      518 2023-06-25 19:04:56.000000 application_properties-0.8.0/test/test_version.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:09:55.659921 application_properties-0.8.1/
+-rw-rw-rw-   0        0        0     1066 2023-07-16 21:57:21.000000 application_properties-0.8.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      125 2023-07-16 23:43:00.000000 application_properties-0.8.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5862 2023-07-21 23:09:55.659921 application_properties-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8311 2023-07-17 02:49:10.000000 application_properties-0.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 23:09:55.633922 application_properties-0.8.1/application_properties/
+-rw-rw-rw-   0        0        0       13 2023-07-16 21:57:21.000000 application_properties-0.8.1/application_properties/.external-package
+-rw-rw-rw-   0        0        0     1339 2023-07-16 21:59:26.000000 application_properties-0.8.1/application_properties/__init__.py
+-rw-rw-rw-   0        0        0    17605 2023-07-16 21:59:26.000000 application_properties-0.8.1/application_properties/application_properties.py
+-rw-rw-rw-   0        0        0     8126 2023-07-16 21:57:21.000000 application_properties-0.8.1/application_properties/application_properties_config_loader.py
+-rw-rw-rw-   0        0        0     4911 2023-07-16 21:57:21.000000 application_properties-0.8.1/application_properties/application_properties_facade.py
+-rw-rw-rw-   0        0        0     3048 2023-07-16 21:57:21.000000 application_properties-0.8.1/application_properties/application_properties_json_loader.py
+-rw-rw-rw-   0        0        0      955 2023-07-16 21:57:21.000000 application_properties-0.8.1/application_properties/application_properties_loader_helper.py
+-rw-rw-rw-   0        0        0     3566 2023-07-16 21:57:21.000000 application_properties-0.8.1/application_properties/application_properties_toml_loader.py
+-rw-rw-rw-   0        0        0     4117 2023-07-16 21:59:26.000000 application_properties-0.8.1/application_properties/application_properties_utilities.py
+-rw-rw-rw-   0        0        0     4555 2023-07-16 21:59:26.000000 application_properties-0.8.1/application_properties/application_properties_yaml_loader.py
+-rw-rw-rw-   0        0        0       13 2023-07-16 21:57:21.000000 application_properties-0.8.1/application_properties/py.typed
+-rw-rw-rw-   0        0        0      212 2023-07-21 03:57:16.000000 application_properties-0.8.1/application_properties/version.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:09:55.641921 application_properties-0.8.1/application_properties.egg-info/
+-rw-rw-rw-   0        0        0     5862 2023-07-21 23:09:55.000000 application_properties-0.8.1/application_properties.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1368 2023-07-21 23:09:55.000000 application_properties-0.8.1/application_properties.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 23:09:55.000000 application_properties-0.8.1/application_properties.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-21 23:09:55.000000 application_properties-0.8.1/application_properties.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-21 23:09:55.000000 application_properties-0.8.1/application_properties.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       53 2023-07-21 04:24:35.000000 application_properties-0.8.1/install-requirements.txt
+-rw-rw-rw-   0        0        0      798 2023-07-21 23:09:55.660920 application_properties-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     3084 2023-07-17 02:48:25.000000 application_properties-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 23:09:55.658921 application_properties-0.8.1/test/
+-rw-rw-rw-   0        0        0    14171 2023-07-16 21:59:26.000000 application_properties-0.8.1/test/test_application_properties.py
+-rw-rw-rw-   0        0        0    23586 2023-07-16 21:57:21.000000 application_properties-0.8.1/test/test_application_properties_config_loader.py
+-rw-rw-rw-   0        0        0     8820 2023-07-16 21:57:21.000000 application_properties-0.8.1/test/test_application_properties_facade.py
+-rw-rw-rw-   0        0        0    14361 2023-07-16 21:59:26.000000 application_properties-0.8.1/test/test_application_properties_json_loader.py
+-rw-rw-rw-   0        0        0    23303 2023-07-16 21:57:21.000000 application_properties-0.8.1/test/test_application_properties_toml_loader.py
+-rw-rw-rw-   0        0        0    20569 2023-07-16 21:57:21.000000 application_properties-0.8.1/test/test_application_properties_utilities.py
+-rw-rw-rw-   0        0        0    24775 2023-07-16 21:59:26.000000 application_properties-0.8.1/test/test_application_properties_yaml_loader.py
+-rw-rw-rw-   0        0        0     3917 2023-07-16 21:57:21.000000 application_properties-0.8.1/test/test_get_boolean.py
+-rw-rw-rw-   0        0        0     3885 2023-07-16 21:57:21.000000 application_properties-0.8.1/test/test_get_integer.py
+-rw-rw-rw-   0        0        0     6299 2023-07-16 21:57:21.000000 application_properties-0.8.1/test/test_get_string.py
+-rw-rw-rw-   0        0        0    24741 2023-07-16 21:59:26.000000 application_properties-0.8.1/test/test_set_manual_property.py
+-rw-rw-rw-   0        0        0      518 2023-07-16 21:57:21.000000 application_properties-0.8.1/test/test_version.py
```

### Comparing `application_properties-0.8.0/LICENSE.txt` & `application_properties-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/PKG-INFO` & `application_properties-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: application_properties
-Version: 0.8.0
+Version: 0.8.1
 Summary: A simple, easy to use, unified manner of accessing program properties.
 Home-page: https://github.com/jackdewinter/application_properties
 Author: Jack De Winter
 Author-email: jack.de.winter@outlook.com
 Maintainer: Jack De Winter
 Maintainer-email: jack.de.winter@outlook.com
 Project-URL: Change Log, https://github.com/jackdewinter/application_properties/blob/main/changelog.md
```

### Comparing `application_properties-0.8.0/README.md` & `application_properties-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/application_properties/__init__.py` & `application_properties-0.8.1/application_properties/__init__.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/application_properties/application_properties.py` & `application_properties-0.8.1/application_properties/application_properties.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/application_properties/application_properties_config_loader.py` & `application_properties-0.8.1/application_properties/application_properties_config_loader.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/application_properties/application_properties_facade.py` & `application_properties-0.8.1/application_properties/application_properties_facade.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/application_properties/application_properties_json_loader.py` & `application_properties-0.8.1/application_properties/application_properties_json_loader.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/application_properties/application_properties_loader_helper.py` & `application_properties-0.8.1/application_properties/application_properties_loader_helper.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/application_properties/application_properties_toml_loader.py` & `application_properties-0.8.1/application_properties/application_properties_toml_loader.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/application_properties/application_properties_utilities.py` & `application_properties-0.8.1/application_properties/application_properties_utilities.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/application_properties/application_properties_yaml_loader.py` & `application_properties-0.8.1/application_properties/application_properties_yaml_loader.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/application_properties.egg-info/PKG-INFO` & `application_properties-0.8.1/application_properties.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: application-properties
-Version: 0.8.0
+Version: 0.8.1
 Summary: A simple, easy to use, unified manner of accessing program properties.
 Home-page: https://github.com/jackdewinter/application_properties
 Author: Jack De Winter
 Author-email: jack.de.winter@outlook.com
 Maintainer: Jack De Winter
 Maintainer-email: jack.de.winter@outlook.com
 Project-URL: Change Log, https://github.com/jackdewinter/application_properties/blob/main/changelog.md
```

### Comparing `application_properties-0.8.0/application_properties.egg-info/SOURCES.txt` & `application_properties-0.8.1/application_properties.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/setup.cfg` & `application_properties-0.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/setup.py` & `application_properties-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/test/test_application_properties.py` & `application_properties-0.8.1/test/test_application_properties.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/test/test_application_properties_config_loader.py` & `application_properties-0.8.1/test/test_application_properties_config_loader.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/test/test_application_properties_facade.py` & `application_properties-0.8.1/test/test_application_properties_facade.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/test/test_application_properties_json_loader.py` & `application_properties-0.8.1/test/test_application_properties_json_loader.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/test/test_application_properties_toml_loader.py` & `application_properties-0.8.1/test/test_application_properties_toml_loader.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/test/test_application_properties_utilities.py` & `application_properties-0.8.1/test/test_application_properties_utilities.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/test/test_application_properties_yaml_loader.py` & `application_properties-0.8.1/test/test_application_properties_yaml_loader.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/test/test_get_boolean.py` & `application_properties-0.8.1/test/test_get_boolean.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/test/test_get_integer.py` & `application_properties-0.8.1/test/test_get_integer.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/test/test_get_string.py` & `application_properties-0.8.1/test/test_get_string.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/test/test_set_manual_property.py` & `application_properties-0.8.1/test/test_set_manual_property.py`

 * *Files identical despite different names*

### Comparing `application_properties-0.8.0/test/test_version.py` & `application_properties-0.8.1/test/test_version.py`

 * *Files identical despite different names*

