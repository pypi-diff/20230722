# Comparing `tmp/klaviyo-for-django-0.0.3.tar.gz` & `tmp/klaviyo-for-django-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klaviyo-for-django-0.0.3.tar", last modified: Thu Jul 20 18:32:29 2023, max compression
+gzip compressed data, was "klaviyo-for-django-0.0.4.tar", last modified: Fri Jul 21 22:25:09 2023, max compression
```

## Comparing `klaviyo-for-django-0.0.3.tar` & `klaviyo-for-django-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:32:29.571361 klaviyo-for-django-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-20 18:32:17.000000 klaviyo-for-django-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-20 18:32:29.571361 klaviyo-for-django-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-20 18:32:17.000000 klaviyo-for-django-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:32:29.571361 klaviyo-for-django-0.0.3/klaviyo_for_django/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-20 18:32:17.000000 klaviyo-for-django-0.0.3/klaviyo_for_django/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:32:29.571361 klaviyo-for-django-0.0.3/klaviyo_for_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-20 18:32:29.000000 klaviyo-for-django-0.0.3/klaviyo_for_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-20 18:32:29.000000 klaviyo-for-django-0.0.3/klaviyo_for_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:32:29.000000 klaviyo-for-django-0.0.3/klaviyo_for_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 18:32:29.000000 klaviyo-for-django-0.0.3/klaviyo_for_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-20 18:32:29.000000 klaviyo-for-django-0.0.3/klaviyo_for_django.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:32:29.571361 klaviyo-for-django-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-20 18:32:17.000000 klaviyo-for-django-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:25:09.396158 klaviyo-for-django-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-21 22:24:59.000000 klaviyo-for-django-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-21 22:25:09.396158 klaviyo-for-django-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-21 22:24:59.000000 klaviyo-for-django-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:25:09.392158 klaviyo-for-django-0.0.4/klaviyo_for_django/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-21 22:24:59.000000 klaviyo-for-django-0.0.4/klaviyo_for_django/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:25:09.392158 klaviyo-for-django-0.0.4/klaviyo_for_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-21 22:25:09.000000 klaviyo-for-django-0.0.4/klaviyo_for_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-21 22:25:09.000000 klaviyo-for-django-0.0.4/klaviyo_for_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:25:09.000000 klaviyo-for-django-0.0.4/klaviyo_for_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-21 22:25:09.000000 klaviyo-for-django-0.0.4/klaviyo_for_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 22:25:09.000000 klaviyo-for-django-0.0.4/klaviyo_for_django.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 22:25:09.396158 klaviyo-for-django-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-21 22:24:59.000000 klaviyo-for-django-0.0.4/setup.py
```

### Comparing `klaviyo-for-django-0.0.3/LICENSE` & `klaviyo-for-django-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `klaviyo-for-django-0.0.3/PKG-INFO` & `klaviyo-for-django-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klaviyo-for-django
-Version: 0.0.3
+Version: 0.0.4
 Home-page: http://pypi.python.org/pypi/klaviyo-for-django/
 Author: Santiago Fernandez
 Author-email: 
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -20,13 +20,13 @@
 
 ## Usage
 
 ```python
 from klaviyo_for_django import send_event
 
 send_event(
-    'profile_email@email.com',
     'event_name',
+    profile_find={'email':'profile_email@email.com'},
     event_properties={'property_name': 'property_value'},
     profile_properties={'other_property_name': 'other_property_value'}
 )
 ```
```

### Comparing `klaviyo-for-django-0.0.3/klaviyo_for_django.egg-info/PKG-INFO` & `klaviyo-for-django-0.0.4/klaviyo_for_django.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klaviyo-for-django
-Version: 0.0.3
+Version: 0.0.4
 Home-page: http://pypi.python.org/pypi/klaviyo-for-django/
 Author: Santiago Fernandez
 Author-email: 
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -20,13 +20,13 @@
 
 ## Usage
 
 ```python
 from klaviyo_for_django import send_event
 
 send_event(
-    'profile_email@email.com',
     'event_name',
+    profile_find={'email':'profile_email@email.com'},
     event_properties={'property_name': 'property_value'},
     profile_properties={'other_property_name': 'other_property_value'}
 )
 ```
```

### Comparing `klaviyo-for-django-0.0.3/setup.py` & `klaviyo-for-django-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="klaviyo-for-django",
-    version="0.0.3",
+    version="0.0.4",
     author="Santiago Fernandez",
     author_email="",
     packages=find_packages(),
     scripts=[],
     url="http://pypi.python.org/pypi/klaviyo-for-django/",
     license="MIT",
     description="",
```

