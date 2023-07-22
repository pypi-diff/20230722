# Comparing `tmp/error-alerts-5.8.tar.gz` & `tmp/error-alerts-5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-alerts-5.8.tar", last modified: Thu Jul  6 16:06:07 2023, max compression
+gzip compressed data, was "error-alerts-5.9.tar", last modified: Sat Jul 22 10:27:24 2023, max compression
```

## Comparing `error-alerts-5.8.tar` & `error-alerts-5.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 16:06:07.352740 error-alerts-5.8/
--rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-5.8/.gitignore
--rw-rw-rw-   0        0        0     1301 2023-07-06 16:06:07.352740 error-alerts-5.8/PKG-INFO
--rw-rw-rw-   0        0        0      994 2023-06-27 12:00:22.000000 error-alerts-5.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 16:06:07.346743 error-alerts-5.8/error_alerts/
--rw-rw-rw-   0        0        0     4305 2023-07-06 16:06:02.000000 error-alerts-5.8/error_alerts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 16:06:07.351740 error-alerts-5.8/error_alerts.egg-info/
--rw-rw-rw-   0        0        0     1301 2023-07-06 16:06:06.000000 error-alerts-5.8/error_alerts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-06 16:06:07.000000 error-alerts-5.8/error_alerts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 16:06:06.000000 error-alerts-5.8/error_alerts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-06 16:06:06.000000 error-alerts-5.8/error_alerts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-06 16:06:06.000000 error-alerts-5.8/error_alerts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-06 16:06:07.353738 error-alerts-5.8/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-06 16:06:04.000000 error-alerts-5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 10:27:24.350672 error-alerts-5.9/
+-rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-5.9/.gitignore
+-rw-rw-rw-   0        0        0     1301 2023-07-22 10:27:24.350672 error-alerts-5.9/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2023-06-27 12:00:22.000000 error-alerts-5.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 10:27:24.345676 error-alerts-5.9/error_alerts/
+-rw-rw-rw-   0        0        0     4322 2023-07-22 10:27:19.000000 error-alerts-5.9/error_alerts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 10:27:24.349673 error-alerts-5.9/error_alerts.egg-info/
+-rw-rw-rw-   0        0        0     1301 2023-07-22 10:27:23.000000 error-alerts-5.9/error_alerts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-22 10:27:24.000000 error-alerts-5.9/error_alerts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 10:27:23.000000 error-alerts-5.9/error_alerts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-22 10:27:23.000000 error-alerts-5.9/error_alerts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-22 10:27:23.000000 error-alerts-5.9/error_alerts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-22 10:27:24.351672 error-alerts-5.9/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-22 10:27:20.000000 error-alerts-5.9/setup.py
```

### Comparing `error-alerts-5.8/PKG-INFO` & `error-alerts-5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 5.8
+Version: 5.9
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

### Comparing `error-alerts-5.8/README.md` & `error-alerts-5.9/README.md`

 * *Files identical despite different names*

### Comparing `error-alerts-5.8/error_alerts/__init__.py` & `error-alerts-5.9/error_alerts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 DEFAULT_IGNORED_ERRORS = [
     'The service is currently unavailable', # Google sheets API down
     'Could not authenticate you', # Twitter app suspended
     ]
 
 class alerts(Bot):
-    def __init__(self, token=None, channel=None, logger=None, raise_error=False, resend_repeat_errors=False):
+    def __init__(self, token=None, channel=None, logger=None, raise_error=False, resend_repeat_errors=False, full_error=None):
         if token and channel:
             bot = super()
             bot.__init__(token=token)
             self.telegram_bot = bot
 
             chat = self.get_chat(channel)
             # print(chat.title)
```

### Comparing `error-alerts-5.8/error_alerts.egg-info/PKG-INFO` & `error-alerts-5.9/error_alerts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 5.8
+Version: 5.9
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

