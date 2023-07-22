# Comparing `tmp/gspot_django_auth-0.1.4.tar.gz` & `tmp/gspot_django_auth-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspot_django_auth-0.1.4.tar", last modified: Thu Jul 20 19:31:27 2023, max compression
+gzip compressed data, was "gspot_django_auth-0.1.5.tar", last modified: Sat Jul 22 12:47:04 2023, max compression
```

## Comparing `gspot_django_auth-0.1.4.tar` & `gspot_django_auth-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-20 19:31:27.714051 gspot_django_auth-0.1.4/
--rw-r--r--   0 vitya      (501) staff       (20)     1063 2023-06-20 19:08:32.000000 gspot_django_auth-0.1.4/LICENSE
--rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 gspot_django_auth-0.1.4/MANIFEST.in
--rw-r--r--   0 vitya      (501) staff       (20)     5063 2023-07-20 19:31:27.714212 gspot_django_auth-0.1.4/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)     4467 2023-07-20 19:26:21.000000 gspot_django_auth-0.1.4/README.md
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-20 19:31:27.709564 gspot_django_auth-0.1.4/gspot_django_auth/
--rw-r--r--   0 vitya      (501) staff       (20)        0 2023-06-27 13:10:00.000000 gspot_django_auth-0.1.4/gspot_django_auth/__init__.py
--rw-r--r--   0 vitya      (501) staff       (20)     1221 2023-07-08 19:28:37.000000 gspot_django_auth-0.1.4/gspot_django_auth/authentication.py
--rw-r--r--   0 vitya      (501) staff       (20)      176 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.4/gspot_django_auth/exceptions.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-20 19:31:27.711855 gspot_django_auth-0.1.4/gspot_django_auth/management/
--rw-r--r--   0 vitya      (501) staff       (20)        0 2023-07-18 13:34:18.000000 gspot_django_auth-0.1.4/gspot_django_auth/management/__init__.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-20 19:31:27.712194 gspot_django_auth-0.1.4/gspot_django_auth/management/commands/
--rw-r--r--   0 vitya      (501) staff       (20)        0 2023-07-18 13:45:15.000000 gspot_django_auth-0.1.4/gspot_django_auth/management/commands/__init__.py
--rw-r--r--   0 vitya      (501) staff       (20)     5152 2023-07-20 19:22:22.000000 gspot_django_auth-0.1.4/gspot_django_auth/management/commands/load_test_tokens.py
--rw-r--r--   0 vitya      (501) staff       (20)     1381 2023-07-20 17:42:19.000000 gspot_django_auth-0.1.4/gspot_django_auth/models.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-20 19:31:27.713714 gspot_django_auth-0.1.4/gspot_django_auth/permissions/
--rw-r--r--   0 vitya      (501) staff       (20)      189 2023-07-08 19:43:37.000000 gspot_django_auth-0.1.4/gspot_django_auth/permissions/__init__.py
--rw-r--r--   0 vitya      (501) staff       (20)     1070 2023-07-08 19:08:49.000000 gspot_django_auth-0.1.4/gspot_django_auth/permissions/permissons.py
--rw-r--r--   0 vitya      (501) staff       (20)     1119 2023-07-03 13:21:53.000000 gspot_django_auth-0.1.4/gspot_django_auth/permissions/validators.py
--rw-r--r--   0 vitya      (501) staff       (20)     1683 2023-07-07 20:05:39.000000 gspot_django_auth-0.1.4/gspot_django_auth/permissions/verifiers.py
--rw-r--r--   0 vitya      (501) staff       (20)      781 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.4/gspot_django_auth/redis_client.py
--rw-r--r--   0 vitya      (501) staff       (20)      243 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.4/gspot_django_auth/token.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-20 19:31:27.711642 gspot_django_auth-0.1.4/gspot_django_auth.egg-info/
--rw-r--r--   0 vitya      (501) staff       (20)     5063 2023-07-20 19:31:27.000000 gspot_django_auth-0.1.4/gspot_django_auth.egg-info/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      776 2023-07-20 19:31:27.000000 gspot_django_auth-0.1.4/gspot_django_auth.egg-info/SOURCES.txt
--rw-r--r--   0 vitya      (501) staff       (20)        1 2023-07-20 19:31:27.000000 gspot_django_auth-0.1.4/gspot_django_auth.egg-info/dependency_links.txt
--rw-r--r--   0 vitya      (501) staff       (20)      158 2023-07-20 19:31:27.000000 gspot_django_auth-0.1.4/gspot_django_auth.egg-info/requires.txt
--rw-r--r--   0 vitya      (501) staff       (20)       18 2023-07-20 19:31:27.000000 gspot_django_auth-0.1.4/gspot_django_auth.egg-info/top_level.txt
--rw-r--r--   0 vitya      (501) staff       (20)      989 2023-07-20 19:31:22.000000 gspot_django_auth-0.1.4/pyproject.toml
--rw-r--r--   0 vitya      (501) staff       (20)      702 2023-07-20 19:31:27.714651 gspot_django_auth-0.1.4/setup.cfg
--rw-r--r--   0 vitya      (501) staff       (20)      168 2023-07-08 19:52:39.000000 gspot_django_auth-0.1.4/setup.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-22 12:47:04.848108 gspot_django_auth-0.1.5/
+-rw-r--r--   0 vitya      (501) staff       (20)     1063 2023-06-20 19:08:32.000000 gspot_django_auth-0.1.5/LICENSE
+-rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 gspot_django_auth-0.1.5/MANIFEST.in
+-rw-r--r--   0 vitya      (501) staff       (20)     5918 2023-07-22 12:47:04.848200 gspot_django_auth-0.1.5/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)     5322 2023-07-22 12:46:37.000000 gspot_django_auth-0.1.5/README.md
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-22 12:47:04.844774 gspot_django_auth-0.1.5/gspot_django_auth/
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2023-06-27 13:10:00.000000 gspot_django_auth-0.1.5/gspot_django_auth/__init__.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1221 2023-07-08 19:28:37.000000 gspot_django_auth-0.1.5/gspot_django_auth/authentication.py
+-rw-r--r--   0 vitya      (501) staff       (20)      176 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.5/gspot_django_auth/exceptions.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-22 12:47:04.846251 gspot_django_auth-0.1.5/gspot_django_auth/management/
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2023-07-18 13:34:18.000000 gspot_django_auth-0.1.5/gspot_django_auth/management/__init__.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-22 12:47:04.846551 gspot_django_auth-0.1.5/gspot_django_auth/management/commands/
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2023-07-18 13:45:15.000000 gspot_django_auth-0.1.5/gspot_django_auth/management/commands/__init__.py
+-rw-r--r--   0 vitya      (501) staff       (20)     6301 2023-07-22 12:46:37.000000 gspot_django_auth-0.1.5/gspot_django_auth/management/commands/load_test_tokens.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1394 2023-07-22 12:41:26.000000 gspot_django_auth-0.1.5/gspot_django_auth/models.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-22 12:47:04.847839 gspot_django_auth-0.1.5/gspot_django_auth/permissions/
+-rw-r--r--   0 vitya      (501) staff       (20)      189 2023-07-08 19:43:37.000000 gspot_django_auth-0.1.5/gspot_django_auth/permissions/__init__.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1070 2023-07-08 19:08:49.000000 gspot_django_auth-0.1.5/gspot_django_auth/permissions/permissons.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1119 2023-07-03 13:21:53.000000 gspot_django_auth-0.1.5/gspot_django_auth/permissions/validators.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1683 2023-07-07 20:05:39.000000 gspot_django_auth-0.1.5/gspot_django_auth/permissions/verifiers.py
+-rw-r--r--   0 vitya      (501) staff       (20)      781 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.5/gspot_django_auth/redis_client.py
+-rw-r--r--   0 vitya      (501) staff       (20)      243 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.5/gspot_django_auth/token.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-22 12:47:04.846067 gspot_django_auth-0.1.5/gspot_django_auth.egg-info/
+-rw-r--r--   0 vitya      (501) staff       (20)     5918 2023-07-22 12:47:04.000000 gspot_django_auth-0.1.5/gspot_django_auth.egg-info/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      776 2023-07-22 12:47:04.000000 gspot_django_auth-0.1.5/gspot_django_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 vitya      (501) staff       (20)        1 2023-07-22 12:47:04.000000 gspot_django_auth-0.1.5/gspot_django_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 vitya      (501) staff       (20)      158 2023-07-22 12:47:04.000000 gspot_django_auth-0.1.5/gspot_django_auth.egg-info/requires.txt
+-rw-r--r--   0 vitya      (501) staff       (20)       18 2023-07-22 12:47:04.000000 gspot_django_auth-0.1.5/gspot_django_auth.egg-info/top_level.txt
+-rw-r--r--   0 vitya      (501) staff       (20)      989 2023-07-22 12:46:45.000000 gspot_django_auth-0.1.5/pyproject.toml
+-rw-r--r--   0 vitya      (501) staff       (20)      702 2023-07-22 12:47:04.848546 gspot_django_auth-0.1.5/setup.cfg
+-rw-r--r--   0 vitya      (501) staff       (20)      168 2023-07-08 19:52:39.000000 gspot_django_auth-0.1.5/setup.py
```

### Comparing `gspot_django_auth-0.1.4/LICENSE` & `gspot_django_auth-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.4/PKG-INFO` & `gspot_django_auth-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: gspot_django_auth
-Version: 0.1.4
-Summary: A Django app for auth.
-Home-page: https://github.com/DJWOMS/GSpot
-Author: Kosenko Viktor
-Author-email: oxpaoff <kosenkoviktor11@gmail.com>
-License: MIT License
-Project-URL: Homepage, https://github.com/oxpaoff/gspot_auth
-Project-URL: Bug Tracker, https://github.com/oxpaoff/gspot_auth/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Overview
 
 GSpot Auth is a Django app for GSpot project https://github.com/DJWOMS/GSpot
 
 Installation
 -----------
 ``$ pip install gspot-django-auth``
@@ -82,14 +65,39 @@
     "is_active": True,
     "groups": [],
     "user_permissions": [],
     "developer_groups": [],
     "developer_permissions": []
 }
 ```
+Token and data for SuperUser Admin
+```
+admin_superuser_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgyNzcwLCJleHAiOjE2ODk2ODMwODB9.47CONTJjEqoL6JMjyERM5WJYYA5jna55w6CXaoW55PI"
+admin_superuser_token = {
+    "username": "admin_username",
+    "first_name": "admin_first_name",
+    "last_name": "admin_last_name",
+    "user_id": "7fff5488-a091-44a1-9a4e-cb9f535a7f34",
+    "role": "administrator",
+    "avatar": "",
+    "permissions": [],
+    "email": "admin@gmail.com",
+    "phone": "88005553535",
+    "country": None,
+    "created_at": "2023-07-08 21:04:32.226941+00:00",
+    "update_at": "2023-07-08 21:04:32.226953+00:00",
+    "is_superuser": True,
+    "is_banned": False,
+    "is_active": True,
+    "groups": [],
+    "user_permissions": [],
+    "developer_groups": [],
+    "developer_permissions": []
+}
+```
 Token and data for Developer
 ```
 dev_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgzMTI3LCJleHAiOjE2ODk2ODM0Mjd9.h-pqm9eDO9yOs2FrHIW0nPTwT45kT9rHvieYfvJoUXc"
 dev_data = {
     "username": "dev_username",
     "first_name": "dev_first_name",
     "last_name": "dev_last_name",
@@ -171,8 +179,8 @@
     "is_banned": False,
     "is_active": True,
     "country": {
         "id": 1,
         "name": "Russia"
     }
 }
-```
+```
```

### Comparing `gspot_django_auth-0.1.4/README.md` & `gspot_django_auth-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: gspot_django_auth
+Version: 0.1.5
+Summary: A Django app for auth.
+Home-page: https://github.com/DJWOMS/GSpot
+Author: Kosenko Viktor
+Author-email: oxpaoff <kosenkoviktor11@gmail.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/oxpaoff/gspot_auth
+Project-URL: Bug Tracker, https://github.com/oxpaoff/gspot_auth/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Overview
 
 GSpot Auth is a Django app for GSpot project https://github.com/DJWOMS/GSpot
 
 Installation
 -----------
 ``$ pip install gspot-django-auth``
@@ -65,14 +82,39 @@
     "is_active": True,
     "groups": [],
     "user_permissions": [],
     "developer_groups": [],
     "developer_permissions": []
 }
 ```
+Token and data for SuperUser Admin
+```
+admin_superuser_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgyNzcwLCJleHAiOjE2ODk2ODMwODB9.47CONTJjEqoL6JMjyERM5WJYYA5jna55w6CXaoW55PI"
+admin_superuser_token = {
+    "username": "admin_username",
+    "first_name": "admin_first_name",
+    "last_name": "admin_last_name",
+    "user_id": "7fff5488-a091-44a1-9a4e-cb9f535a7f34",
+    "role": "administrator",
+    "avatar": "",
+    "permissions": [],
+    "email": "admin@gmail.com",
+    "phone": "88005553535",
+    "country": None,
+    "created_at": "2023-07-08 21:04:32.226941+00:00",
+    "update_at": "2023-07-08 21:04:32.226953+00:00",
+    "is_superuser": True,
+    "is_banned": False,
+    "is_active": True,
+    "groups": [],
+    "user_permissions": [],
+    "developer_groups": [],
+    "developer_permissions": []
+}
+```
 Token and data for Developer
 ```
 dev_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgzMTI3LCJleHAiOjE2ODk2ODM0Mjd9.h-pqm9eDO9yOs2FrHIW0nPTwT45kT9rHvieYfvJoUXc"
 dev_data = {
     "username": "dev_username",
     "first_name": "dev_first_name",
     "last_name": "dev_last_name",
@@ -154,8 +196,8 @@
     "is_banned": False,
     "is_active": True,
     "country": {
         "id": 1,
         "name": "Russia"
     }
 }
-```
+```
```

### Comparing `gspot_django_auth-0.1.4/gspot_django_auth/authentication.py` & `gspot_django_auth-0.1.5/gspot_django_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.4/gspot_django_auth/management/commands/load_test_tokens.py` & `gspot_django_auth-0.1.5/gspot_django_auth/management/commands/load_test_tokens.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,36 @@
             "update_at": "2023-07-08 21:04:32.226953+00:00",
             "is_superuser": False,
             "groups": [],
             "user_permissions": [],
             "developer_groups": [],
             "developer_permissions": []
         }
+        admin_superuser_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgyNzcwLCJleHAiOjE2ODk2ODMwODB9.47CONTJjEqoL6JMjyERM5WJYYA5jna55w6CXaoW55PI"
+        admin_superuser_data = {
+            "username": "admin_username",
+            "first_name": "admin_first_name",
+            "last_name": "admin_last_name",
+            "is_banned": False,
+            "is_active": True,
+            "user_id": "7fff5488-a091-44a1-9a4e-cb9f535a7f34",
+            "role": "administrator",
+            "avatar": "",
+            "permissions": [],
+            "email": "admin@gmail.com",
+            "phone": "88005553535",
+            "country": None,
+            "created_at": "2023-07-08 21:04:32.226941+00:00",
+            "update_at": "2023-07-08 21:04:32.226953+00:00",
+            "is_superuser": True,
+            "groups": [],
+            "user_permissions": [],
+            "developer_groups": [],
+            "developer_permissions": []
+        }
 
         dev_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgzMTI3LCJleHAiOjE2ODk2ODM0Mjd9.h-pqm9eDO9yOs2FrHIW0nPTwT45kT9rHvieYfvJoUXc"
         dev_data = {
             "username": "dev_username",
             "first_name": "dev_first_name",
             "last_name": "dev_last_name",
             "is_banned": False,
@@ -114,20 +136,25 @@
             "country": {
                 "id": 1,
                 "name": "Russia"
             }
         }
         tokens = {
             admin_token: admin_data,
+            admin_superuser_token: admin_superuser_data,
             dev_token: dev_data,
             owner_token: owner_data,
             customer_token: customer_data
         }
         return tokens
 
     @staticmethod
     def add_to_redis(tokens: dict):
         redis_client = RedisAccessClient()
         for token, value in tokens.items():
-            value_data = json.dumps(value)
             name = f'{redis_client._prefix}:{token}'
+            try:
+                redis_client.conn.delete(name)
+            except:
+                pass
+            value_data = json.dumps(value)
             redis_client.conn.set(name=name, value=value_data)
```

### Comparing `gspot_django_auth-0.1.4/gspot_django_auth/models.py` & `gspot_django_auth-0.1.5/gspot_django_auth/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     company: dict
     groups: List[str] = field(default_factory=list)
     user_permissions: List[str] = field(default_factory=list)
 
 
 @dataclass(frozen=True)
 class CustomerUser(BaseUser):
+    age: int
     birthday: datetime
     friends: List[str] = field(default_factory=list)
 
 
 class UserFactory:
     users = {'administrator': AdminUser, 'developer': DeveloperUser, 'customer': CustomerUser}
```

### Comparing `gspot_django_auth-0.1.4/gspot_django_auth/permissions/permissons.py` & `gspot_django_auth-0.1.5/gspot_django_auth/permissions/permissons.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.4/gspot_django_auth/permissions/validators.py` & `gspot_django_auth-0.1.5/gspot_django_auth/permissions/validators.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.4/gspot_django_auth/permissions/verifiers.py` & `gspot_django_auth-0.1.5/gspot_django_auth/permissions/verifiers.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.4/gspot_django_auth/redis_client.py` & `gspot_django_auth-0.1.5/gspot_django_auth/redis_client.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.4/gspot_django_auth.egg-info/PKG-INFO` & `gspot_django_auth-0.1.5/gspot_django_auth.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspot-django-auth
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Django app for auth.
 Home-page: https://github.com/DJWOMS/GSpot
 Author: Kosenko Viktor
 Author-email: oxpaoff <kosenkoviktor11@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/oxpaoff/gspot_auth
 Project-URL: Bug Tracker, https://github.com/oxpaoff/gspot_auth/issues
@@ -81,14 +81,39 @@
     "is_banned": False,
     "is_active": True,
     "groups": [],
     "user_permissions": [],
     "developer_groups": [],
     "developer_permissions": []
 }
+```
+Token and data for SuperUser Admin
+```
+admin_superuser_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgyNzcwLCJleHAiOjE2ODk2ODMwODB9.47CONTJjEqoL6JMjyERM5WJYYA5jna55w6CXaoW55PI"
+admin_superuser_token = {
+    "username": "admin_username",
+    "first_name": "admin_first_name",
+    "last_name": "admin_last_name",
+    "user_id": "7fff5488-a091-44a1-9a4e-cb9f535a7f34",
+    "role": "administrator",
+    "avatar": "",
+    "permissions": [],
+    "email": "admin@gmail.com",
+    "phone": "88005553535",
+    "country": None,
+    "created_at": "2023-07-08 21:04:32.226941+00:00",
+    "update_at": "2023-07-08 21:04:32.226953+00:00",
+    "is_superuser": True,
+    "is_banned": False,
+    "is_active": True,
+    "groups": [],
+    "user_permissions": [],
+    "developer_groups": [],
+    "developer_permissions": []
+}
 ```
 Token and data for Developer
 ```
 dev_token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiaWF0IjoxNjg5NjgzMTI3LCJleHAiOjE2ODk2ODM0Mjd9.h-pqm9eDO9yOs2FrHIW0nPTwT45kT9rHvieYfvJoUXc"
 dev_data = {
     "username": "dev_username",
     "first_name": "dev_first_name",
```

### Comparing `gspot_django_auth-0.1.4/gspot_django_auth.egg-info/SOURCES.txt` & `gspot_django_auth-0.1.5/gspot_django_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.4/pyproject.toml` & `gspot_django_auth-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gspot_django_auth"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
     { name = "oxpaoff", email = "kosenkoviktor11@gmail.com" },
 ]
 description = "A Django app for auth."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gspot_django_auth-0.1.4/setup.cfg` & `gspot_django_auth-0.1.5/setup.cfg`

 * *Files identical despite different names*

