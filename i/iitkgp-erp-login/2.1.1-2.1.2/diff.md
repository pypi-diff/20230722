# Comparing `tmp/iitkgp_erp_login-2.1.1.tar.gz` & `tmp/iitkgp_erp_login-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iitkgp_erp_login-2.1.1.tar", last modified: Sat Jul 22 18:06:57 2023, max compression
+gzip compressed data, was "iitkgp_erp_login-2.1.2.tar", last modified: Sat Jul 22 20:44:13 2023, max compression
```

## Comparing `iitkgp_erp_login-2.1.1.tar` & `iitkgp_erp_login-2.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:06:57.991418 iitkgp_erp_login-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-22 18:06:15.000000 iitkgp_erp_login-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-07-22 18:06:57.991418 iitkgp_erp_login-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16160 2023-07-22 18:06:15.000000 iitkgp_erp_login-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-22 18:06:40.000000 iitkgp_erp_login-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 18:06:57.991418 iitkgp_erp_login-2.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:06:57.987418 iitkgp_erp_login-2.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:06:57.991418 iitkgp_erp_login-2.1.1/src/iitkgp_erp_login/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 18:06:15.000000 iitkgp_erp_login-2.1.1/src/iitkgp_erp_login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-22 18:06:15.000000 iitkgp_erp_login-2.1.1/src/iitkgp_erp_login/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-22 18:06:15.000000 iitkgp_erp_login-2.1.1/src/iitkgp_erp_login/erp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-22 18:06:15.000000 iitkgp_erp_login-2.1.1/src/iitkgp_erp_login/read_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-22 18:06:15.000000 iitkgp_erp_login-2.1.1/src/iitkgp_erp_login/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:06:57.991418 iitkgp_erp_login-2.1.1/src/iitkgp_erp_login.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-07-22 18:06:57.000000 iitkgp_erp_login-2.1.1/src/iitkgp_erp_login.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-22 18:06:57.000000 iitkgp_erp_login-2.1.1/src/iitkgp_erp_login.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 18:06:57.000000 iitkgp_erp_login-2.1.1/src/iitkgp_erp_login.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-22 18:06:57.000000 iitkgp_erp_login-2.1.1/src/iitkgp_erp_login.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-22 18:06:57.000000 iitkgp_erp_login-2.1.1/src/iitkgp_erp_login.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:44:13.388147 iitkgp_erp_login-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-22 20:43:34.000000 iitkgp_erp_login-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-07-22 20:44:13.388147 iitkgp_erp_login-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16160 2023-07-22 20:43:34.000000 iitkgp_erp_login-2.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-22 20:43:57.000000 iitkgp_erp_login-2.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 20:44:13.388147 iitkgp_erp_login-2.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:44:13.388147 iitkgp_erp_login-2.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:44:13.388147 iitkgp_erp_login-2.1.2/src/iitkgp_erp_login/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 20:43:34.000000 iitkgp_erp_login-2.1.2/src/iitkgp_erp_login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-22 20:43:34.000000 iitkgp_erp_login-2.1.2/src/iitkgp_erp_login/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-22 20:43:34.000000 iitkgp_erp_login-2.1.2/src/iitkgp_erp_login/erp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-22 20:43:34.000000 iitkgp_erp_login-2.1.2/src/iitkgp_erp_login/read_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-22 20:43:34.000000 iitkgp_erp_login-2.1.2/src/iitkgp_erp_login/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:44:13.388147 iitkgp_erp_login-2.1.2/src/iitkgp_erp_login.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-07-22 20:44:13.000000 iitkgp_erp_login-2.1.2/src/iitkgp_erp_login.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-22 20:44:13.000000 iitkgp_erp_login-2.1.2/src/iitkgp_erp_login.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 20:44:13.000000 iitkgp_erp_login-2.1.2/src/iitkgp_erp_login.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-22 20:44:13.000000 iitkgp_erp_login-2.1.2/src/iitkgp_erp_login.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-22 20:44:13.000000 iitkgp_erp_login-2.1.2/src/iitkgp_erp_login.egg-info/top_level.txt
```

### Comparing `iitkgp_erp_login-2.1.1/LICENSE` & `iitkgp_erp_login-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iitkgp_erp_login-2.1.1/PKG-INFO` & `iitkgp_erp_login-2.1.2/src/iitkgp_erp_login.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: iitkgp_erp_login
-Version: 2.1.1
+Name: iitkgp-erp-login
+Version: 2.1.2
 Summary: A package to automate login process in ERP for IIT-KGP
 Author-email: Arpit Bhardwaj <proffapt@pm.me>
 Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iitkgp_erp_login Version: 2.1.1 Summary: A package
+Metadata-Version: 2.1 Name: iitkgp-erp-login Version: 2.1.2 Summary: A package
 to automate login process in ERP for IIT-KGP Author-email: Arpit Bhardwaj
 pm.me> Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # ERP Login Module Tired of the tedious ERP login process? Wanted to
```

### Comparing `iitkgp_erp_login-2.1.1/README.md` & `iitkgp_erp_login-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `iitkgp_erp_login-2.1.1/pyproject.toml` & `iitkgp_erp_login-2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "iitkgp_erp_login"
-version = "2.1.1"
+version = "2.1.2"
 authors = [
   { name="Arpit Bhardwaj", email="proffapt@pm.me" },
 ]
 description = "A package to automate login process in ERP for IIT-KGP"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `iitkgp_erp_login-2.1.1/src/iitkgp_erp_login/erp.py` & `iitkgp_erp_login-2.1.2/src/iitkgp_erp_login/erp.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 class ErpLoginError(Exception):
     pass
 
 
 def login(headers, session, ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False, SESSION_STORAGE_FILE=None):
     global sessionToken
     ssoToken = None
-	if len(sys.argv) == 1 and sys.argv[0] == '-c':
-		caller_file = None
-	else:
+    if len(sys.argv) == 1 and sys.argv[0] == '-c':
+        caller_file = None
+    else:
         caller_file = inspect.getframeinfo(inspect.currentframe().f_back).filename
-    token_file = f"{get_import_location(caller_file)}/{SESSION_STORAGE_FILE}" if SESSION_STORAGE_FILE else None
+    token_file = f"{get_import_location(caller_file)}/{SESSION_STORAGE_FILE}" if SESSION_STORAGE_FILE else ""
     if SESSION_STORAGE_FILE:
         try:
             with open(token_file, "r") as file:
                 lines = file.readlines()
                 sessionToken = lines[0].strip() if len(lines) > 0 else None
                 ssoToken = lines[1].strip() if len(lines) > 1 else None
             logging.info(" Retrieved tokens from the file") if LOGGING else None
```

### Comparing `iitkgp_erp_login-2.1.1/src/iitkgp_erp_login/read_mail.py` & `iitkgp_erp_login-2.1.2/src/iitkgp_erp_login/read_mail.py`

 * *Files identical despite different names*

### Comparing `iitkgp_erp_login-2.1.1/src/iitkgp_erp_login/utils.py` & `iitkgp_erp_login-2.1.2/src/iitkgp_erp_login/utils.py`

 * *Files identical despite different names*

### Comparing `iitkgp_erp_login-2.1.1/src/iitkgp_erp_login.egg-info/PKG-INFO` & `iitkgp_erp_login-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: iitkgp-erp-login
-Version: 2.1.1
+Name: iitkgp_erp_login
+Version: 2.1.2
 Summary: A package to automate login process in ERP for IIT-KGP
 Author-email: Arpit Bhardwaj <proffapt@pm.me>
 Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iitkgp-erp-login Version: 2.1.1 Summary: A package
+Metadata-Version: 2.1 Name: iitkgp_erp_login Version: 2.1.2 Summary: A package
 to automate login process in ERP for IIT-KGP Author-email: Arpit Bhardwaj
 pm.me> Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # ERP Login Module Tired of the tedious ERP login process? Wanted to
```

