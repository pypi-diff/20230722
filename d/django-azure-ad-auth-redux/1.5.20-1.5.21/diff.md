# Comparing `tmp/django_azure_ad_auth_redux-1.5.20.tar.gz` & `tmp/django_azure_ad_auth_redux-1.5.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_azure_ad_auth_redux-1.5.20.tar", max compression
+gzip compressed data, was "django_azure_ad_auth_redux-1.5.21.tar", max compression
```

## Comparing `django_azure_ad_auth_redux-1.5.20.tar` & `django_azure_ad_auth_redux-1.5.21.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1588 2023-07-21 18:20:38.857349 django_azure_ad_auth_redux-1.5.20/LICENSE
--rw-r--r--   0        0        0     1610 2023-07-21 17:45:48.627893 django_azure_ad_auth_redux-1.5.20/README.md
--rw-r--r--   0        0        0      623 2023-07-22 14:59:26.692077 django_azure_ad_auth_redux-1.5.20/azure_ad_auth/__init__.py
--rw-r--r--   0        0        0     3736 2023-07-21 18:57:34.242612 django_azure_ad_auth_redux-1.5.20/azure_ad_auth/backends.py
--rw-r--r--   0        0        0      186 2023-07-21 18:29:17.765056 django_azure_ad_auth_redux-1.5.20/azure_ad_auth/urls.py
--rw-r--r--   0        0        0     3778 2023-07-21 18:52:14.696198 django_azure_ad_auth_redux-1.5.20/azure_ad_auth/utils.py
--rw-r--r--   0        0        0     1744 2023-07-21 18:53:49.464263 django_azure_ad_auth_redux-1.5.20/azure_ad_auth/views.py
--rw-r--r--   0        0        0     5536 2023-07-22 15:05:30.495331 django_azure_ad_auth_redux-1.5.20/pyproject.toml
--rw-r--r--   0        0        0     2951 1970-01-01 00:00:00.000000 django_azure_ad_auth_redux-1.5.20/PKG-INFO
+-rw-r--r--   0        0        0     1588 2023-07-21 18:20:38.857349 django_azure_ad_auth_redux-1.5.21/LICENSE
+-rw-r--r--   0        0        0     1610 2023-07-21 17:45:48.627893 django_azure_ad_auth_redux-1.5.21/README.md
+-rw-r--r--   0        0        0      632 2023-07-22 21:05:27.012443 django_azure_ad_auth_redux-1.5.21/azure_ad_auth/__init__.py
+-rw-r--r--   0        0        0     3736 2023-07-21 18:57:34.242612 django_azure_ad_auth_redux-1.5.21/azure_ad_auth/backends.py
+-rw-r--r--   0        0        0      186 2023-07-21 18:29:17.765056 django_azure_ad_auth_redux-1.5.21/azure_ad_auth/urls.py
+-rw-r--r--   0        0        0     3861 2023-07-22 21:07:58.186030 django_azure_ad_auth_redux-1.5.21/azure_ad_auth/utils.py
+-rw-r--r--   0        0        0     1744 2023-07-21 18:53:49.464263 django_azure_ad_auth_redux-1.5.21/azure_ad_auth/views.py
+-rw-r--r--   0        0        0     5536 2023-07-22 21:08:29.405302 django_azure_ad_auth_redux-1.5.21/pyproject.toml
+-rw-r--r--   0        0        0     2951 1970-01-01 00:00:00.000000 django_azure_ad_auth_redux-1.5.21/PKG-INFO
```

### Comparing `django_azure_ad_auth_redux-1.5.20/LICENSE` & `django_azure_ad_auth_redux-1.5.21/LICENSE`

 * *Files identical despite different names*

### Comparing `django_azure_ad_auth_redux-1.5.20/README.md` & `django_azure_ad_auth_redux-1.5.21/README.md`

 * *Files identical despite different names*

### Comparing `django_azure_ad_auth_redux-1.5.20/azure_ad_auth/backends.py` & `django_azure_ad_auth_redux-1.5.21/azure_ad_auth/backends.py`

 * *Files identical despite different names*

### Comparing `django_azure_ad_auth_redux-1.5.20/azure_ad_auth/utils.py` & `django_azure_ad_auth_redux-1.5.21/azure_ad_auth/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,21 +89,23 @@
         ]
     except Exception:  # TODO - which ones exactly?
         keys = []
     return keys
 
 
 def get_token_payload(token=None, audience=CLIENT_ID, nonce=None):
+    headers = jwt.get_unverified_header(token)
+    algorithm = header.get("alg", "RS256"]
     for key in get_public_keys():
         try:
             payload = jwt.decode(
                 token,
                 key=key,
                 audience=audience,
-                algorithms=["HS256", "RS256"],
+                algorithms=[algorithm],
             )
 
             if payload["nonce"] != nonce:
                 continue
 
             return payload
         except (jwt.InvalidTokenError, IndexError) as e:
```

### Comparing `django_azure_ad_auth_redux-1.5.20/azure_ad_auth/views.py` & `django_azure_ad_auth_redux-1.5.21/azure_ad_auth/views.py`

 * *Files identical despite different names*

### Comparing `django_azure_ad_auth_redux-1.5.20/pyproject.toml` & `django_azure_ad_auth_redux-1.5.21/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-azure-ad-auth-redux"
-version = "1.5.20"
+version = "1.5.21"
 description="Authenticate users using Azure Active Directory."
 authors = ["Scott Sharkey <scott.sharkey@rsginc.com>"]
 license = "MIT"
 packages = [{include = "azure_ad_auth"}]
 readme = "README.md"
 repository = "https://github.com/lanshark/django-azure-ad-auth-redux"
 homepage = "https://github.com/lanshark/django-azure-ad-auth-redux"
```

### Comparing `django_azure_ad_auth_redux-1.5.20/PKG-INFO` & `django_azure_ad_auth_redux-1.5.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-azure-ad-auth-redux
-Version: 1.5.20
+Version: 1.5.21
 Summary: Authenticate users using Azure Active Directory.
 Home-page: https://github.com/lanshark/django-azure-ad-auth-redux
 License: MIT
 Keywords: Python, Active Directory, Django
 Author: Scott Sharkey
 Author-email: scott.sharkey@rsginc.com
 Requires-Python: >=3.10,<3.12
```

