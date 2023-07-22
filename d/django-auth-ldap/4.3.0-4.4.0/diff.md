# Comparing `tmp/django-auth-ldap-4.3.0.tar.gz` & `tmp/django-auth-ldap-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-auth-ldap-4.3.0.tar", last modified: Wed Apr 26 19:45:49 2023, max compression
+gzip compressed data, was "django-auth-ldap-4.4.0.tar", last modified: Sat Jul 22 19:16:36 2023, max compression
```

## Comparing `django-auth-ldap-4.3.0.tar` & `django-auth-ldap-4.4.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 19:45:49.770546 django-auth-ldap-4.3.0/
--rw-------   0 freitafr  (1000) freitafr  (1000)     1297 2020-12-14 12:14:26.000000 django-auth-ldap-4.3.0/LICENSE
--rw-------   0 freitafr  (1000) freitafr  (1000)       64 2023-03-28 09:44:55.000000 django-auth-ldap-4.3.0/MANIFEST.in
--rw-------   0 freitafr  (1000) freitafr  (1000)     7121 2023-04-26 19:45:49.770546 django-auth-ldap-4.3.0/PKG-INFO
--rw-------   0 freitafr  (1000) freitafr  (1000)     5484 2022-08-16 11:46:04.000000 django-auth-ldap-4.3.0/README.rst
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 19:45:49.767212 django-auth-ldap-4.3.0/django_auth_ldap/
--rw-------   0 freitafr  (1000) freitafr  (1000)      113 2021-05-05 13:49:26.000000 django-auth-ldap-4.3.0/django_auth_ldap/__init__.py
--rw-------   0 freitafr  (1000) freitafr  (1000)    32422 2022-06-13 12:14:29.000000 django-auth-ldap-4.3.0/django_auth_ldap/backend.py
--rw-------   0 freitafr  (1000) freitafr  (1000)    24980 2022-06-13 12:14:29.000000 django-auth-ldap-4.3.0/django_auth_ldap/config.py
--rw-------   0 freitafr  (1000) freitafr  (1000)      160 2023-04-26 19:45:49.000000 django-auth-ldap-4.3.0/django_auth_ldap/version.py
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 19:45:49.767212 django-auth-ldap-4.3.0/django_auth_ldap.egg-info/
--rw-------   0 freitafr  (1000) freitafr  (1000)     7121 2023-04-26 19:45:49.000000 django-auth-ldap-4.3.0/django_auth_ldap.egg-info/PKG-INFO
--rw-------   0 freitafr  (1000) freitafr  (1000)      793 2023-04-26 19:45:49.000000 django-auth-ldap-4.3.0/django_auth_ldap.egg-info/SOURCES.txt
--rw-------   0 freitafr  (1000) freitafr  (1000)        1 2023-04-26 19:45:49.000000 django-auth-ldap-4.3.0/django_auth_ldap.egg-info/dependency_links.txt
--rw-------   0 freitafr  (1000) freitafr  (1000)       29 2023-04-26 19:45:49.000000 django-auth-ldap-4.3.0/django_auth_ldap.egg-info/requires.txt
--rw-------   0 freitafr  (1000) freitafr  (1000)       17 2023-04-26 19:45:49.000000 django-auth-ldap-4.3.0/django_auth_ldap.egg-info/top_level.txt
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 19:45:49.770546 django-auth-ldap-4.3.0/docs/
--rw-------   0 freitafr  (1000) freitafr  (1000)      620 2020-12-14 12:14:26.000000 django-auth-ldap-4.3.0/docs/Makefile
--rw-------   0 freitafr  (1000) freitafr  (1000)     7313 2021-05-05 13:49:22.000000 django-auth-ldap-4.3.0/docs/authentication.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)     8558 2022-01-12 14:50:13.000000 django-auth-ldap-4.3.0/docs/changes.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)     5920 2022-06-13 12:14:29.000000 django-auth-ldap-4.3.0/docs/conf.py
--rw-------   0 freitafr  (1000) freitafr  (1000)      969 2023-03-28 09:38:27.000000 django-auth-ldap-4.3.0/docs/contributing.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)     5051 2021-02-15 09:20:44.000000 django-auth-ldap-4.3.0/docs/custombehavior.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)     2462 2021-02-15 09:20:44.000000 django-auth-ldap-4.3.0/docs/example.rst
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 19:45:49.770546 django-auth-ldap-4.3.0/docs/ext/
--rw-------   0 freitafr  (1000) freitafr  (1000)      196 2020-12-14 12:14:26.000000 django-auth-ldap-4.3.0/docs/ext/daldocs.py
--rw-------   0 freitafr  (1000) freitafr  (1000)     4248 2021-02-15 09:20:44.000000 django-auth-ldap-4.3.0/docs/groups.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)      966 2022-06-13 12:14:29.000000 django-auth-ldap-4.3.0/docs/index.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)     1591 2021-10-20 09:01:15.000000 django-auth-ldap-4.3.0/docs/install.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)      639 2021-02-15 09:20:44.000000 django-auth-ldap-4.3.0/docs/logging.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)     1748 2021-02-15 09:20:44.000000 django-auth-ldap-4.3.0/docs/multiconfig.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)     1687 2020-12-14 12:14:26.000000 django-auth-ldap-4.3.0/docs/performance.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)     3940 2020-12-14 12:14:26.000000 django-auth-ldap-4.3.0/docs/permissions.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)    20968 2021-09-16 14:26:42.000000 django-auth-ldap-4.3.0/docs/reference.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)       15 2021-05-05 13:49:26.000000 django-auth-ldap-4.3.0/docs/requirements.txt
--rw-------   0 freitafr  (1000) freitafr  (1000)     6560 2021-02-15 09:20:44.000000 django-auth-ldap-4.3.0/docs/users.rst
--rw-------   0 freitafr  (1000) freitafr  (1000)      189 2023-03-28 09:38:27.000000 django-auth-ldap-4.3.0/pyproject.toml
--rw-------   0 freitafr  (1000) freitafr  (1000)     1587 2023-04-26 19:45:49.770546 django-auth-ldap-4.3.0/setup.cfg
-drwx------   0 freitafr  (1000) freitafr  (1000)        0 2023-04-26 19:45:49.770546 django-auth-ldap-4.3.0/tests/
--rw-------   0 freitafr  (1000) freitafr  (1000)        0 2020-12-14 12:14:26.000000 django-auth-ldap-4.3.0/tests/__init__.py
--rw-------   0 freitafr  (1000) freitafr  (1000)      581 2021-02-15 09:20:44.000000 django-auth-ldap-4.3.0/tests/models.py
--rw-------   0 freitafr  (1000) freitafr  (1000)      322 2021-05-05 13:49:26.000000 django-auth-ldap-4.3.0/tests/settings.py
--rw-------   0 freitafr  (1000) freitafr  (1000)     4037 2020-12-14 12:14:26.000000 django-auth-ldap-4.3.0/tests/tests.ldif
--rw-------   0 freitafr  (1000) freitafr  (1000)    61622 2022-08-16 10:13:05.000000 django-auth-ldap-4.3.0/tests/tests.py
--rw-------   0 freitafr  (1000) freitafr  (1000)      920 2023-04-26 19:31:31.000000 django-auth-ldap-4.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:16:36.808713 django-auth-ldap-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-07-22 19:16:36.808713 django-auth-ldap-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:16:36.800712 django-auth-ldap-4.4.0/django_auth_ldap/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/django_auth_ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32422 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/django_auth_ldap/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24980 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/django_auth_ldap/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-22 19:16:36.000000 django-auth-ldap-4.4.0/django_auth_ldap/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:16:36.804712 django-auth-ldap-4.4.0/django_auth_ldap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-07-22 19:16:36.000000 django-auth-ldap-4.4.0/django_auth_ldap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-22 19:16:36.000000 django-auth-ldap-4.4.0/django_auth_ldap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 19:16:36.000000 django-auth-ldap-4.4.0/django_auth_ldap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-22 19:16:36.000000 django-auth-ldap-4.4.0/django_auth_ldap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-22 19:16:36.000000 django-auth-ldap-4.4.0/django_auth_ldap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:16:36.808713 django-auth-ldap-4.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/docs/authentication.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/docs/custombehavior.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/docs/example.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:16:36.808713 django-auth-ldap-4.4.0/docs/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/docs/ext/daldocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/docs/groups.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/docs/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/docs/multiconfig.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/docs/performance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/docs/permissions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20968 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/docs/users.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-22 19:16:36.808713 django-auth-ldap-4.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:16:36.808713 django-auth-ldap-4.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/tests/tests.ldif
+-rw-r--r--   0 runner    (1001) docker     (123)    61622 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-22 19:16:20.000000 django-auth-ldap-4.4.0/tox.ini
```

### Comparing `django-auth-ldap-4.3.0/LICENSE` & `django-auth-ldap-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/PKG-INFO` & `django-auth-ldap-4.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: django-auth-ldap
-Version: 4.3.0
-Summary: Django LDAP authentication backend.
-Home-page: https://github.com/django-auth-ldap/django-auth-ldap
-Author: Peter Sagerson
-Author-email: psagers@ignorare.net
+Version: 4.4.0
+Summary: Django LDAP authentication backend
+Author-email: Peter Sagerson <psagers@ignorare.net>
+Maintainer-email: François Freitag <mail@franek.fr>
 License: BSD
+Project-URL: Homepage, https://github.com/django-auth-ldap/django-auth-ldap
 Project-URL: Documentation, https://django-auth-ldap.readthedocs.io/
 Project-URL: Source, https://github.com/django-auth-ldap/django-auth-ldap
 Project-URL: Tracker, https://github.com/django-auth-ldap/django-auth-ldap/issues
 Project-URL: Changelog, https://github.com/django-auth-ldap/django-auth-ldap/releases/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -18,23 +18,22 @@
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory :: LDAP
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ================================
 Django Authentication Using LDAP
 ================================
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-auth-ldap-4.3.0/README.rst` & `django-auth-ldap-4.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/django_auth_ldap/backend.py` & `django-auth-ldap-4.4.0/django_auth_ldap/backend.py`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/django_auth_ldap/config.py` & `django-auth-ldap-4.4.0/django_auth_ldap/config.py`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/django_auth_ldap.egg-info/PKG-INFO` & `django-auth-ldap-4.4.0/django_auth_ldap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: django-auth-ldap
-Version: 4.3.0
-Summary: Django LDAP authentication backend.
-Home-page: https://github.com/django-auth-ldap/django-auth-ldap
-Author: Peter Sagerson
-Author-email: psagers@ignorare.net
+Version: 4.4.0
+Summary: Django LDAP authentication backend
+Author-email: Peter Sagerson <psagers@ignorare.net>
+Maintainer-email: François Freitag <mail@franek.fr>
 License: BSD
+Project-URL: Homepage, https://github.com/django-auth-ldap/django-auth-ldap
 Project-URL: Documentation, https://django-auth-ldap.readthedocs.io/
 Project-URL: Source, https://github.com/django-auth-ldap/django-auth-ldap
 Project-URL: Tracker, https://github.com/django-auth-ldap/django-auth-ldap/issues
 Project-URL: Changelog, https://github.com/django-auth-ldap/django-auth-ldap/releases/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -18,23 +18,22 @@
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory :: LDAP
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ================================
 Django Authentication Using LDAP
 ================================
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-auth-ldap-4.3.0/django_auth_ldap.egg-info/SOURCES.txt` & `django-auth-ldap-4.4.0/django_auth_ldap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/docs/Makefile` & `django-auth-ldap-4.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/docs/authentication.rst` & `django-auth-ldap-4.4.0/docs/authentication.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/docs/changes.rst` & `django-auth-ldap-4.4.0/docs/changes.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/docs/conf.py` & `django-auth-ldap-4.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/docs/contributing.rst` & `django-auth-ldap-4.4.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/docs/custombehavior.rst` & `django-auth-ldap-4.4.0/docs/custombehavior.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/docs/example.rst` & `django-auth-ldap-4.4.0/docs/example.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/docs/groups.rst` & `django-auth-ldap-4.4.0/docs/groups.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/docs/index.rst` & `django-auth-ldap-4.4.0/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 groups, and permissions.
 
 * Documentation: https://django-auth-ldap.readthedocs.io/
 * PyPI: https://pypi.org/project/django-auth-ldap/
 * Repository: https://github.com/django-auth-ldap/django-auth-ldap
 * License: BSD 2-Clause
 
-This version is supported on Python 3.7+; and Django 2.2+. It requires
+This version is supported on Python 3.8+; and Django 2.2+. It requires
 `python-ldap`_ >= 3.1.
 
 .. toctree::
     :maxdepth: 2
 
     install
     authentication
```

### Comparing `django-auth-ldap-4.3.0/docs/install.rst` & `django-auth-ldap-4.4.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/docs/logging.rst` & `django-auth-ldap-4.4.0/docs/logging.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/docs/multiconfig.rst` & `django-auth-ldap-4.4.0/docs/multiconfig.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/docs/performance.rst` & `django-auth-ldap-4.4.0/docs/performance.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/docs/permissions.rst` & `django-auth-ldap-4.4.0/docs/permissions.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/docs/reference.rst` & `django-auth-ldap-4.4.0/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/docs/users.rst` & `django-auth-ldap-4.4.0/docs/users.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/setup.cfg` & `django-auth-ldap-4.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,59 @@
-[metadata]
-name = django-auth-ldap
-description = Django LDAP authentication backend.
-long_description = file: README.rst
-long_description_content_type = text/x-rst
-author = Peter Sagerson
-author_email = psagers@ignorare.net
-url = https://github.com/django-auth-ldap/django-auth-ldap
-license = BSD
-classifiers = 
-	Development Status :: 5 - Production/Stable
-	Environment :: Web Environment
-	Framework :: Django
-	Framework :: Django :: 3.2
-	Framework :: Django :: 4.1
-	Framework :: Django :: 4.2
-	Intended Audience :: Developers
-	Intended Audience :: System Administrators
-	License :: OSI Approved :: BSD License
-	Programming Language :: Python
-	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
-	Programming Language :: Python :: 3.11
-	Topic :: Internet :: WWW/HTTP
-	Topic :: Software Development :: Libraries :: Python Modules
-	Topic :: System :: Systems Administration :: Authentication/Directory :: LDAP
-project_urls = 
-	Documentation = https://django-auth-ldap.readthedocs.io/
-	Source = https://github.com/django-auth-ldap/django-auth-ldap
-	Tracker = https://github.com/django-auth-ldap/django-auth-ldap/issues
-	Changelog = https://github.com/django-auth-ldap/django-auth-ldap/releases/
+[project]
+name = "django-auth-ldap"
+requires-python = ">=3.8"
+description = "Django LDAP authentication backend"
+readme = "README.rst"
+authors = [
+    { name="Peter Sagerson", email="psagers@ignorare.net"},
+]
+maintainers = [
+    { name="François Freitag", email="mail@franek.fr" },
+]
+license = { text="BSD" }
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Environment :: Web Environment",
+    "Framework :: Django",
+    "Framework :: Django :: 3.2",
+    "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
+    "Intended Audience :: Developers",
+    "Intended Audience :: System Administrators",
+    "License :: OSI Approved :: BSD License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Internet :: WWW/HTTP",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: System :: Systems Administration :: Authentication/Directory :: LDAP",
+]
+dynamic = ["version"]
 
-[options]
-python_requires = >=3.7
-packages = django_auth_ldap
-install_requires = 
-	Django>=3.2
-	python-ldap>=3.1
+dependencies = [
+    "Django>=3.2",
+    "python-ldap>=3.1",
+]
 
-[flake8]
-max-line-length = 88
+[project.urls]
+Homepage = "https://github.com/django-auth-ldap/django-auth-ldap"
+Documentation = "https://django-auth-ldap.readthedocs.io/"
+Source = "https://github.com/django-auth-ldap/django-auth-ldap"
+Tracker = "https://github.com/django-auth-ldap/django-auth-ldap/issues"
+Changelog = "https://github.com/django-auth-ldap/django-auth-ldap/releases/"
 
-[isort]
-profile = black
+[tool.isort]
+profile = "black"
 
-[egg_info]
-tag_build = 
-tag_date = 0
+[build-system]
+requires = [
+    "setuptools>=42",
+    "setuptools_scm[toml]>=3.4",
+]
+build-backend = "setuptools.build_meta"
 
+[tool.setuptools_scm]
+write_to = "django_auth_ldap/version.py"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-auth-ldap-4.3.0/tests/models.py` & `django-auth-ldap-4.4.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/tests/tests.ldif` & `django-auth-ldap-4.4.0/tests/tests.ldif`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/tests/tests.py` & `django-auth-ldap-4.4.0/tests/tests.py`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.3.0/tox.ini` & `django-auth-ldap-4.4.0/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tox]
 envlist =
     black
     flake8
     isort
     docs
     django32
-    django40
     django41
+    django42
     djangomain
 isolated_build = true
 
 [testenv]
 commands = {envpython} -Wa -b -m django test --settings tests.settings
 deps =
     django32: Django>=3.2,<4.0
@@ -37,18 +37,7 @@
 isolated_build = true
 deps =
     readme_renderer
     sphinx
 commands =
     make -C docs html
 allowlist_externals = make
-
-[testenv:packaging]
-deps =
-    build
-    setuptools
-    twine
-    wheel
-skip_install = true
-commands =
-    python -m build
-    twine check --strict dist/*
```

