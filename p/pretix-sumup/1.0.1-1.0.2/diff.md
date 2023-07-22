# Comparing `tmp/pretix-sumup-1.0.1.tar.gz` & `tmp/pretix-sumup-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-sumup-1.0.1.tar", last modified: Fri Jul 21 08:40:05 2023, max compression
+gzip compressed data, was "pretix-sumup-1.0.2.tar", last modified: Sat Jul 22 09:41:41 2023, max compression
```

## Comparing `pretix-sumup-1.0.1.tar` & `pretix-sumup-1.0.2.tar`

### file list

```diff
@@ -1,47 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.080200 pretix-sumup-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    33886 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-07-21 08:40:05.080200 pretix-sumup-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.076200 pretix-sumup-1.0.1/pretix_sumup/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.072200 pretix-sumup-1.0.1/pretix_sumup/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.072200 pretix-sumup-1.0.1/pretix_sumup/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.076200 pretix-sumup-1.0.1/pretix_sumup/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.076200 pretix-sumup-1.0.1/pretix_sumup/locale/de_Informal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.076200 pretix-sumup-1.0.1/pretix_sumup/locale/de_Informal/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.072200 pretix-sumup-1.0.1/pretix_sumup/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.076200 pretix-sumup-1.0.1/pretix_sumup/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.072200 pretix-sumup-1.0.1/pretix_sumup/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.076200 pretix-sumup-1.0.1/pretix_sumup/static/pretix_sumup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/static/pretix_sumup/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.072200 pretix-sumup-1.0.1/pretix_sumup/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.076200 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/checkout_confirm_render.html
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/control.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.080200 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/email/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/email/order_pending.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/not_available.html
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/pending.html
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/prepare.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.076200 pretix-sumup-1.0.1/pretix_sumup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-07-21 08:40:05.000000 pretix-sumup-1.0.1/pretix_sumup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-21 08:40:05.000000 pretix-sumup-1.0.1/pretix_sumup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:40:05.000000 pretix-sumup-1.0.1/pretix_sumup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-21 08:40:05.000000 pretix-sumup-1.0.1/pretix_sumup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 08:40:05.000000 pretix-sumup-1.0.1/pretix_sumup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-21 08:40:05.080200 pretix-sumup-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:40:05.080200 pretix-sumup-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-21 08:38:34.000000 pretix-sumup-1.0.1/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    33886 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-07-22 09:41:41.385984 pretix-sumup-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.377984 pretix-sumup-1.0.2/pretix_sumup/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.373984 pretix-sumup-1.0.2/pretix_sumup/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/locale/de_Informal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/locale/de_Informal/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/locale/django.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.373984 pretix-sumup-1.0.2/pretix_sumup/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.373984 pretix-sumup-1.0.2/pretix_sumup/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.373984 pretix-sumup-1.0.2/pretix_sumup/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.373984 pretix-sumup-1.0.2/pretix_sumup/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/static/pretix_sumup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/static/pretix_sumup/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.377984 pretix-sumup-1.0.2/pretix_sumup/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/checkout_confirm_render.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/control.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/email/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/email/order_pending.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/not_available.html
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/pending.html
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/prepare.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/pretix_sumup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-07-22 09:41:41.000000 pretix-sumup-1.0.2/pretix_sumup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-22 09:41:41.000000 pretix-sumup-1.0.2/pretix_sumup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 09:41:41.000000 pretix-sumup-1.0.2/pretix_sumup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-22 09:41:41.000000 pretix-sumup-1.0.2/pretix_sumup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-22 09:41:41.000000 pretix-sumup-1.0.2/pretix_sumup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-22 09:41:41.385984 pretix-sumup-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 09:41:41.381984 pretix-sumup-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-22 09:39:53.000000 pretix-sumup-1.0.2/tests/test_main.py
```

### Comparing `pretix-sumup-1.0.1/LICENSE` & `pretix-sumup-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.1/PKG-INFO` & `pretix-sumup-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-sumup
-Version: 1.0.1
+Version: 1.0.2
 Summary: Sumup plugin
 Author-email: Ronan Le Meillat <ronan@highcanfly.club>
 Maintainer-email: Ronan Le Meillat <ronan@highcanfly.club>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
         Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `pretix-sumup-1.0.1/README.md` & `pretix-sumup-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.1/pretix_sumup/apps.py` & `pretix-sumup-1.0.2/pretix_sumup/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.1/pretix_sumup/locale/fr/LC_MESSAGES/django.po` & `pretix-sumup-1.0.2/pretix_sumup/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.1/pretix_sumup/payment.py` & `pretix-sumup-1.0.2/pretix_sumup/payment.py`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.1/pretix_sumup/signals.py` & `pretix-sumup-1.0.2/pretix_sumup/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.1/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg` & `pretix-sumup-1.0.2/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html` & `pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.1/pretix_sumup/templates/pretix_sumup/control.html` & `pretix-sumup-1.0.2/pretix_sumup/templates/pretix_sumup/control.html`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.1/pretix_sumup.egg-info/PKG-INFO` & `pretix-sumup-1.0.2/pretix_sumup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-sumup
-Version: 1.0.1
+Version: 1.0.2
 Summary: Sumup plugin
 Author-email: Ronan Le Meillat <ronan@highcanfly.club>
 Maintainer-email: Ronan Le Meillat <ronan@highcanfly.club>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
         Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `pretix-sumup-1.0.1/pretix_sumup.egg-info/SOURCES.txt` & `pretix-sumup-1.0.2/pretix_sumup.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,18 +9,21 @@
 pretix_sumup/payment.py
 pretix_sumup/signals.py
 pretix_sumup.egg-info/PKG-INFO
 pretix_sumup.egg-info/SOURCES.txt
 pretix_sumup.egg-info/dependency_links.txt
 pretix_sumup.egg-info/entry_points.txt
 pretix_sumup.egg-info/top_level.txt
+pretix_sumup/locale/django.pot
 pretix_sumup/locale/de/LC_MESSAGES/django.po
 pretix_sumup/locale/de_Informal/.gitkeep
 pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po
+pretix_sumup/locale/es/LC_MESSAGES/django.po
 pretix_sumup/locale/fr/LC_MESSAGES/django.po
+pretix_sumup/locale/it/LC_MESSAGES/django.po
 pretix_sumup/static/pretix_sumup/.gitkeep
 pretix_sumup/static/pretix_sumup/sumup-logo-black.svg
 pretix_sumup/templates/pretix_sumup/.gitkeep
 pretix_sumup/templates/pretix_sumup/checkout_confirm_render.html
 pretix_sumup/templates/pretix_sumup/checkout_payment_form.html
 pretix_sumup/templates/pretix_sumup/control.html
 pretix_sumup/templates/pretix_sumup/not_available.html
```

### Comparing `pretix-sumup-1.0.1/pyproject.toml` & `pretix-sumup-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.1/setup.cfg` & `pretix-sumup-1.0.2/setup.cfg`

 * *Files identical despite different names*

