# Comparing `tmp/pyroostermoney-0.2.2.tar.gz` & `tmp/pyroostermoney-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroostermoney-0.2.2.tar", last modified: Thu Jul 20 13:16:51 2023, max compression
+gzip compressed data, was "pyroostermoney-0.2.3.tar", last modified: Sat Jul 22 13:03:52 2023, max compression
```

## Comparing `pyroostermoney-0.2.2.tar` & `pyroostermoney-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:16:51.398360 pyroostermoney-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:16:51.394360 pyroostermoney-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:16:51.394360 pyroostermoney-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 13:16:51.398360 pyroostermoney-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:16:51.394360 pyroostermoney-0.2.2/pyroostermoney/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:16:51.398360 pyroostermoney-0.2.2/pyroostermoney/child/
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/child/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/child/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/child/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/child/money_pot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/child/standing_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/child/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/family_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/roostermoney.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:16:51.398360 pyroostermoney-0.2.2/pyroostermoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 13:16:51.000000 pyroostermoney-0.2.2/pyroostermoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-20 13:16:51.000000 pyroostermoney-0.2.2/pyroostermoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:16:51.000000 pyroostermoney-0.2.2/pyroostermoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 13:16:51.000000 pyroostermoney-0.2.2/pyroostermoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 13:16:51.000000 pyroostermoney-0.2.2/pyroostermoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-20 13:16:51.398360 pyroostermoney-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:03:52.368996 pyroostermoney-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:03:52.364996 pyroostermoney-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:03:52.368996 pyroostermoney-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-22 13:03:52.368996 pyroostermoney-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:03:52.368996 pyroostermoney-0.2.3/pyroostermoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/pyroostermoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/pyroostermoney/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:03:52.368996 pyroostermoney-0.2.3/pyroostermoney/child/
+-rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/pyroostermoney/child/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/pyroostermoney/child/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/pyroostermoney/child/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/pyroostermoney/child/money_pot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/pyroostermoney/child/standing_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/pyroostermoney/child/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/pyroostermoney/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/pyroostermoney/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/pyroostermoney/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/pyroostermoney/family_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/pyroostermoney/roostermoney.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:03:52.368996 pyroostermoney-0.2.3/pyroostermoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-22 13:03:52.000000 pyroostermoney-0.2.3/pyroostermoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-22 13:03:52.000000 pyroostermoney-0.2.3/pyroostermoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 13:03:52.000000 pyroostermoney-0.2.3/pyroostermoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-22 13:03:52.000000 pyroostermoney-0.2.3/pyroostermoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-22 13:03:52.000000 pyroostermoney-0.2.3/pyroostermoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-22 13:03:52.368996 pyroostermoney-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-22 13:03:39.000000 pyroostermoney-0.2.3/setup.py
```

### Comparing `pyroostermoney-0.2.2/.github/workflows/build.yml` & `pyroostermoney-0.2.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.2/.gitignore` & `pyroostermoney-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.2/LICENSE` & `pyroostermoney-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.2/PKG-INFO` & `pyroostermoney-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.2.2
+Version: 0.2.3
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.2.2/pyroostermoney/api.py` & `pyroostermoney-0.2.3/pyroostermoney/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,76 @@
 """Rooster Money requests and session handler."""
 # pylint: disable=too-many-arguments
 # pylint: disable=too-many-branches
 # pylint: disable=too-many-arguments
 # pylint: disable=too-many-instance-attributes
-import json
 import logging
 import base64
 import asyncio
 from datetime import datetime, timedelta
 
 import aiohttp
 
-from .const import HEADERS, BASE_URL, LOGIN_BODY, URLS
+from .const import HEADERS, BASE_URL, LOGIN_BODY, URLS, OAUTH_TOKEN_URL
 from .exceptions import InvalidAuthError, NotLoggedIn, AuthenticationExpired
 from .events import Events
 
 _LOGGER = logging.getLogger(__name__)
 
 async def _fetch_request(url, headers=None):
     if headers is None:
         headers=HEADERS
     async with aiohttp.ClientSession() as session:
         async with session.get(f"{BASE_URL}/{url}", headers=headers) as response:
-            text = await response.text()
+            data = await response.json()
             return {
                 "status": response.status,
-                "response": json.loads(text)
+                "response": data
             }
 
 async def _post_request(url, body: dict, auth=None, headers=None):
     if headers is None:
         headers=HEADERS
     async with aiohttp.ClientSession() as session:
         async with session.post(f"{BASE_URL}/{url}",
                                 json=body,
                                 headers=headers,
                                 auth=auth) as response:
-            text = await response.text()
+            data = await response.json()
             return {
                 "status": response.status,
-                "response": json.loads(text)
+                "response": data
+            }
+
+async def _put_request(url, body: dict, auth=None, headers=None):
+    if headers is None:
+        headers=HEADERS
+    async with aiohttp.ClientSession() as session:
+        async with session.put(f"{BASE_URL}/{url}",
+                                json=body,
+                                headers=headers,
+                                auth=auth) as response:
+            data = await response.json()
+            return {
+                "status": response.status,
+                "response": data
             }
 
 async def _delete_request(url, body: dict, auth=None, headers=None):
     if headers is None:
         headers=HEADERS
     async with aiohttp.ClientSession() as session:
         async with session.delete(f"{BASE_URL}/{url}",
                                 json=body,
                                 headers=headers,
                                 auth=auth) as response:
-            text = await response.text()
+            data = await response.json()
             return {
                 "status": response.status,
-                "response": json.loads(text)
+                "response": data
             }
 
 class RoosterSession:
     """The main Rooster Session."""
 
     def __init__(self,
                  username: str,
@@ -70,14 +83,27 @@
         self._headers = HEADERS
         self._logged_in = False
         self._logging_in = asyncio.Lock()
         self.events = Events()
         self.update_interval = update_interval
         self.use_updater = use_updater
 
+    def _parse_login(self, login_response, token):
+        """Parses a login response"""
+        if "tokens" in login_response:
+            login_response=login_response.get("tokens")
+        return {
+                "access_token": login_response.get("access_token"),
+                "refresh_token": login_response.get("refresh_token"),
+                "token_type": login_response.get("token_type"),
+                "expiry_time": datetime.now() + timedelta(0,
+                                                          login_response.get("expires_in")),
+                "security_code": token
+            }
+
     async def async_login(self):
         """Logs into RoosterMoney and starts a new active session."""
         if self._logging_in.locked():
             _LOGGER.warning("Login already attempting. Only one execution allowed.")
             while self._logging_in.locked():
                 await asyncio.sleep(1)
             return True
@@ -103,32 +129,37 @@
 
             if login_response["status"] == 401:
                 raise InvalidAuthError(self._username, login_response["status"])
 
             login_response = login_response["response"]
             token = base64.b64encode(str(self._password[::-1]).encode('utf-8')).decode('utf-8')
 
-            self._session = {
-                "access_token": login_response["tokens"]["access_token"],
-                "refresh_token": login_response["tokens"]["refresh_token"],
-                "token_type": login_response["tokens"]["token_type"],
-                "expiry_time": datetime.now() + timedelta(0,
-                                                          login_response["tokens"]["expires_in"]),
-                "security_code": token
-            }
+            self._session = self._parse_login(login_response, token)
 
             token_type = login_response["tokens"]["token_type"]
             access_token = login_response["tokens"]["access_token"]
 
             self._headers["Authorization"] = f"{token_type} {access_token}"
 
             self._logged_in = True
 
         return True
 
+    async def refresh_token(self):
+        """Refresh the current access token when the session expires."""
+        async with aiohttp.ClientSession() as session:
+            form = aiohttp.FormData()
+            form.add_field("audience", "rooster-app")
+            form.add_field("grant_type", "refresh_token")
+            form.add_field("client_id", "rooster-app")
+            form.add_field("refresh_token", self._session.get("refresh_token"))
+            async with session.post(OAUTH_TOKEN_URL, data=form) as request:
+                data = await request.json()
+                self._session = self._parse_login(data, self._session.get("security_code"))
+
     async def _internal_request_handler(self,
                                         url,
                                         body=None,
                                         headers=None,
                                         auth=None,
                                         method="GET",
                                         login_request=False,
@@ -162,14 +193,16 @@
         if add_security_token:
             headers["securitytoken"] = self._session["security_code"]
 
         if method == "GET":
             return await _fetch_request(url, headers=headers)
         if method == "POST":
             return await _post_request(url, body=body, headers=headers)
+        if method == "PUT":
+            return await _put_request(url, body=body, headers=headers)
         if method == "DELETE":
             return await _delete_request(url, body=body, headers=headers)
         else:
             raise ValueError("Invalid type argument.")
 
     async def request_handler(self,
                                         url,
@@ -188,15 +221,15 @@
                 headers=headers,
                 auth=auth,
                 method=method,
                 login_request=login_request,
                 add_security_token=add_security_token
             )
         except AuthenticationExpired:
-            await self.async_login()
+            await self.refresh_token()
             return await self._internal_request_handler(
                 url=url,
                 body=body,
                 headers=headers,
                 auth=auth,
                 method=method,
                 login_request=login_request
```

### Comparing `pyroostermoney-0.2.2/pyroostermoney/child/__init__.py` & `pyroostermoney-0.2.3/pyroostermoney/child/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,7 +228,20 @@
                 user_id=self.user_id,
                 standing_order_id=standing_order.regular_id
             ),
             method="DELETE"
         )
 
         return bool(output.get("status") == 200)
+
+    async def update_allowance(self, paused: bool = False, amount: float = 0.0):
+        """Updates the allowance for the child."""
+        data = {
+            "locked": paused,
+            "pocketMoneyAmount": amount,
+            "stripData": True,
+            "userId": self.user_id
+        }
+
+        await self._session.request_handler(URLS.get("get_child").format(user_id=self.user_id),
+                                            body=data,
+                                            method="PUT")
```

### Comparing `pyroostermoney-0.2.2/pyroostermoney/child/card.py` & `pyroostermoney-0.2.3/pyroostermoney/child/card.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.2/pyroostermoney/child/money_pot.py` & `pyroostermoney-0.2.3/pyroostermoney/child/money_pot.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.2/pyroostermoney/child/standing_order.py` & `pyroostermoney-0.2.3/pyroostermoney/child/standing_order.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.2/pyroostermoney/child/transaction.py` & `pyroostermoney-0.2.3/pyroostermoney/child/transaction.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.2/pyroostermoney/const.py` & `pyroostermoney-0.2.3/pyroostermoney/const.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # pylint: disable=line-too-long
 """Static Rooster Money variables"""
 
-VERSION="0.2.2"
+VERSION="0.2.3"
 BASE_URL="https://api.rooster.money"
+OAUTH_TOKEN_URL="https://auth.rooster.money/oidc/token"
 LANGUAGE="en-GB"
 COUNTRY="gb"
 CURRENCY="GBP"
 TIMEZONE_ID=60
 TIMEZONE="GMT+01:00"
 DEFAULT_PRECISION=2
 DEFAULT_BANK_NAME="Rooster Money"
 DEFAULT_BANK_TYPE="Business"
 MOBILE_APP_VERSION="10.3.1"
 
-SAVINGS_POT_ID="savings"
-SPEND_POT_ID="spend"
-GIVE_POT_ID="give"
-GOAL_POT_ID="goal"
+SAVINGS_POT_ID="SAVE_POT"
+SPEND_POT_ID="SPEND_POT"
+GIVE_POT_ID="GIVE_POT"
+GOAL_POT_ID="GOAL_POT"
 
 URLS = {
     "login": "api/v1/parent",
     "get_account_info": "api/parent",
     "get_child": "api/parent/child/{user_id}",
     "get_child_allowance_periods": "api/parent/child/{user_id}/allowance-periods",
     "get_top_up_methods": "api/parent/acquirer/topup/methods?currency={currency}",
@@ -33,15 +34,17 @@
     "create_payment": "api/parent/acquirer/create-payment",
     "get_child_card_details": "api/parent/child/{user_id}/card/details",
     "get_child_card_pin": "api/parent/child/{user_id}/cards/{card_id}/pin",
     "get_family_account_cards": "api/parent/family/cards",
     "get_child_standing_orders": "api/parent/child/{user_id}/standingorder",
     "create_child_standing_order": "api/parent/child/{user_id}/standingorder/",
     "delete_child_standing_order": "api/parent/child/{user_id}/standingorder/{delete_child_standing_order}",
-    "get_master_job_list": "api/parent/master-jobs"
+    "get_master_job_list": "api/parent/master-jobs",
+    "boost_pot": "api/v1/families/{family_id}/children/{user_id}/pots/{pot_id}/boost",
+    "scheduled_job_action": "/api/parent/scheduled-jobs/{schedule_id}/{action}"
 }
 
 HEADERS = {
     "content-type": "application/json",
     "accept": "application/json",
     "user-agent": f"Mozilla/5.0 Rooster Money {MOBILE_APP_VERSION}"
 }
@@ -81,7 +84,19 @@
         "encryptedSecurityCode": "",
         "holderName": "",
         "type": "scheme"
     },
     "returnUrl": "roostermoneyapp://",
     "shopperEmail": ""
 }
+
+BOOST_BODY = {
+    "amount": {
+        "amount": 0.0,
+        "currency": CURRENCY,
+        "precision": DEFAULT_PRECISION
+    },
+    "metaData": {
+        "flowSource": "spend pot"
+    },
+    "reason": ""
+}
```

### Comparing `pyroostermoney-0.2.2/pyroostermoney/events.py` & `pyroostermoney-0.2.3/pyroostermoney/events.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.2/pyroostermoney/exceptions.py` & `pyroostermoney-0.2.3/pyroostermoney/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.2/pyroostermoney/family_account.py` & `pyroostermoney-0.2.3/pyroostermoney/family_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         self.account_number = raw_response["accountNumber"]
         self.sort_code = raw_response["sortCode"]
         self._precision = raw_response["suggestedMonthlyTransfer"]["precision"]
         amount = raw_response["suggestedMonthlyTransfer"]["amount"]
         self.suggested_monthly_transfer = amount / (1 * 10**self._precision)
         self.currency = raw_response["suggestedMonthlyTransfer"]["currency"]
         self.balance = account_info.get("familyLedgerBalance", None)
+        self.family_id = account_info.get("familyId")
         if self.balance is not None:
             self.balance = float(self.balance)
 
     async def update(self):
         """Updates the FamilyAccount object data."""
         if self._update_lock.locked():
             return True
```

### Comparing `pyroostermoney-0.2.2/pyroostermoney/roostermoney.py` & `pyroostermoney-0.2.3/pyroostermoney/roostermoney.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.2/pyroostermoney.egg-info/PKG-INFO` & `pyroostermoney-0.2.3/pyroostermoney.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.2.2
+Version: 0.2.3
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.2.2/pyroostermoney.egg-info/SOURCES.txt` & `pyroostermoney-0.2.3/pyroostermoney.egg-info/SOURCES.txt`

 * *Files identical despite different names*

