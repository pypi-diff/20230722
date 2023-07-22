# Comparing `tmp/kontolibs-5.9.1.tar.gz` & `tmp/kontolibs-9.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kontolibs-5.9.1.tar", last modified: Sat Jul 22 15:05:41 2023, max compression
+gzip compressed data, was "kontolibs-9.9.1.tar", last modified: Tue Jul 11 03:34:19 2023, max compression
```

## Comparing `kontolibs-5.9.1.tar` & `kontolibs-9.9.1.tar`

### file list

```diff
@@ -1,42 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:05:41.490117 kontolibs-5.9.1/
--rw-r--r--   0 root         (0) root         (0)     2536 2023-07-22 15:05:41.490117 kontolibs-5.9.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1584 2023-07-22 13:02:42.000000 kontolibs-5.9.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:05:41.140117 kontolibs-5.9.1/kontolibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2536 2023-07-22 15:05:40.000000 kontolibs-5.9.1/kontolibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      995 2023-07-22 15:05:40.000000 kontolibs-5.9.1/kontolibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-22 15:05:40.000000 kontolibs-5.9.1/kontolibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-22 15:05:40.000000 kontolibs-5.9.1/kontolibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-22 15:05:40.000000 kontolibs-5.9.1/kontolibs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:05:41.160117 kontolibs-5.9.1/kynaylibs/
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-22 15:01:39.000000 kontolibs-5.9.1/kynaylibs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:05:41.200117 kontolibs-5.9.1/kynaylibs/nan/
--rw-r--r--   0 root         (0) root         (0)     1737 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/load.py
--rw-r--r--   0 root         (0) root         (0)      890 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:05:41.430117 kontolibs-5.9.1/kynaylibs/nan/utils/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/PyroHelpers.py
--rw-r--r--   0 root         (0) root         (0)      371 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/adminHelpers.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/ai.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/aiohttp_helper.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/basic.py
--rw-r--r--   0 root         (0) root         (0)    15599 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:05:41.470117 kontolibs-5.9.1/kynaylibs/nan/utils/db/
--rw-r--r--   0 root         (0) root         (0)     2502 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/db/_BaseClient.py
--rw-r--r--   0 root         (0) root         (0)    14229 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1578 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/db/dbExpired.py
--rw-r--r--   0 root         (0) root         (0)     1190 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/db/permit.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/function.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/get_id.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/http.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/inline.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/interval.py
--rw-r--r--   0 root         (0) root         (0)     6722 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/parser.py
--rw-r--r--   0 root         (0) root         (0)     1844 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/pilter.py
--rw-r--r--   0 root         (0) root         (0)    17772 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/tools.py
--rw-r--r--   0 root         (0) root         (0)      567 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/unpack.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-07-22 13:02:42.000000 kontolibs-5.9.1/kynaylibs/nan/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)       46 2023-07-22 15:05:28.000000 kontolibs-5.9.1/kynaylibs/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-22 15:05:41.490117 kontolibs-5.9.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1561 2023-07-22 15:02:29.000000 kontolibs-5.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:34:19.923748 kontolibs-9.9.1/
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-07-11 03:34:19.923748 kontolibs-9.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1584 2023-07-11 00:03:12.000000 kontolibs-9.9.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:34:19.593748 kontolibs-9.9.1/kontolibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-07-11 03:34:18.000000 kontolibs-9.9.1/kontolibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      921 2023-07-11 03:34:18.000000 kontolibs-9.9.1/kontolibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 03:34:18.000000 kontolibs-9.9.1/kontolibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-11 03:34:18.000000 kontolibs-9.9.1/kontolibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-11 03:34:18.000000 kontolibs-9.9.1/kontolibs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:34:19.623748 kontolibs-9.9.1/kynaylibs/
+-rw-r--r--   0 root         (0) root         (0)       33 2023-07-11 03:33:12.000000 kontolibs-9.9.1/kynaylibs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:34:19.653748 kontolibs-9.9.1/kynaylibs/nan/
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/load.py
+-rw-r--r--   0 root         (0) root         (0)      890 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:34:19.873748 kontolibs-9.9.1/kynaylibs/nan/utils/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/PyroHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      371 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/adminHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/ai.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/aiohttp_helper.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/basic.py
+-rw-r--r--   0 root         (0) root         (0)    15599 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:34:19.913748 kontolibs-9.9.1/kynaylibs/nan/utils/db/
+-rw-r--r--   0 root         (0) root         (0)    14229 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/db/permit.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/function.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/get_id.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/http.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/inline.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/interval.py
+-rw-r--r--   0 root         (0) root         (0)     6722 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/pilter.py
+-rw-r--r--   0 root         (0) root         (0)    17772 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/tools.py
+-rw-r--r--   0 root         (0) root         (0)      567 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/unpack.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-07-11 00:03:12.000000 kontolibs-9.9.1/kynaylibs/nan/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-11 02:51:11.000000 kontolibs-9.9.1/kynaylibs/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 03:34:19.933748 kontolibs-9.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1561 2023-07-11 03:34:12.000000 kontolibs-9.9.1/setup.py
```

### Comparing `kontolibs-5.9.1/PKG-INFO` & `kontolibs-9.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kontolibs
-Version: 5.9.1
+Version: 9.9.1
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: bisghav
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kontolibs-5.9.1/README.md` & `kontolibs-9.9.1/README.md`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kontolibs.egg-info/PKG-INFO` & `kontolibs-9.9.1/kontolibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kontolibs
-Version: 5.9.1
+Version: 9.9.1
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: bisghav
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kontolibs-5.9.1/kontolibs.egg-info/SOURCES.txt` & `kontolibs-9.9.1/kontolibs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,11 +24,9 @@
 kynaylibs/nan/utils/interval.py
 kynaylibs/nan/utils/misc.py
 kynaylibs/nan/utils/parser.py
 kynaylibs/nan/utils/pilter.py
 kynaylibs/nan/utils/tools.py
 kynaylibs/nan/utils/unpack.py
 kynaylibs/nan/utils/utility.py
-kynaylibs/nan/utils/db/_BaseClient.py
 kynaylibs/nan/utils/db/__init__.py
-kynaylibs/nan/utils/db/dbExpired.py
 kynaylibs/nan/utils/db/permit.py
```

### Comparing `kontolibs-5.9.1/kynaylibs/nan/__init__.py` & `kontolibs-9.9.1/kynaylibs/nan/__init__.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/load.py` & `kontolibs-9.9.1/kynaylibs/nan/load.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/log.py` & `kontolibs-9.9.1/kynaylibs/nan/log.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/utils/PyroHelpers.py` & `kontolibs-9.9.1/kynaylibs/nan/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/utils/adminHelpers.py` & `kontolibs-9.9.1/kynaylibs/nan/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/utils/ai.py` & `kontolibs-9.9.1/kynaylibs/nan/utils/ai.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/utils/aiohttp_helper.py` & `kontolibs-9.9.1/kynaylibs/nan/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/utils/basic.py` & `kontolibs-9.9.1/kynaylibs/nan/utils/basic.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/utils/constants.py` & `kontolibs-9.9.1/kynaylibs/nan/utils/constants.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/utils/db/__init__.py` & `kontolibs-9.9.1/kynaylibs/nan/utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/utils/db/permit.py` & `kontolibs-9.9.1/kynaylibs/nan/utils/db/permit.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/utils/function.py` & `kontolibs-9.9.1/kynaylibs/nan/utils/function.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/utils/get_id.py` & `kontolibs-9.9.1/kynaylibs/nan/utils/get_id.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/utils/http.py` & `kontolibs-9.9.1/kynaylibs/nan/utils/http.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/utils/inline.py` & `kontolibs-9.9.1/kynaylibs/nan/utils/inline.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                     callback_data="{}_module({},{})".format(
                         prefix, chat, x.__MODULE__.replace(" ", "_").lower()
                     ),
                 )
                 for x in module_dict.values()
             ]
         )
-    line = 3
+    line = 4
     pairs = list(zip(modules[::2], modules[1::2]))
     i = 0
     for m in pairs:
         for _ in m:
             i += 1
     if len(modules) - i == 1:
         pairs.append((modules[-1],))
@@ -58,18 +58,18 @@
     max_num_pages = ceil(len(pairs) / line)
     modulo_page = page_n % max_num_pages
 
     if len(pairs) > line:
         pairs = pairs[modulo_page * line : line * (modulo_page + 1)] + [
             (
                 EqInlineKeyboardButton(
-                    "◄",
+                    "❮❮",
                     callback_data="{}_prev({})".format(prefix, modulo_page),
                 ),
                 EqInlineKeyboardButton(
-                    "►",
+                    "❯❯",
                     callback_data="{}_next({})".format(prefix, modulo_page),
                 ),
             )
         ]
 
     return pairs
```

### Comparing `kontolibs-5.9.1/kynaylibs/nan/utils/interval.py` & `kontolibs-9.9.1/kynaylibs/nan/utils/interval.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/utils/misc.py` & `kontolibs-9.9.1/kynaylibs/nan/utils/misc.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/utils/parser.py` & `kontolibs-9.9.1/kynaylibs/nan/utils/parser.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/utils/pilter.py` & `kontolibs-9.9.1/kynaylibs/nan/utils/pilter.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/utils/tools.py` & `kontolibs-9.9.1/kynaylibs/nan/utils/tools.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/utils/unpack.py` & `kontolibs-9.9.1/kynaylibs/nan/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/kynaylibs/nan/utils/utility.py` & `kontolibs-9.9.1/kynaylibs/nan/utils/utility.py`

 * *Files identical despite different names*

### Comparing `kontolibs-5.9.1/setup.py` & `kontolibs-9.9.1/setup.py`

 * *Files identical despite different names*

