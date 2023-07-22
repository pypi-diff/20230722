# Comparing `tmp/selfcord.py-0.2.3.tar.gz` & `tmp/selfcord.py-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfcord.py-0.2.3.tar", last modified: Fri Jul 14 16:54:38 2023, max compression
+gzip compressed data, was "selfcord.py-0.2.4.tar", last modified: Sat Jul 22 16:50:16 2023, max compression
```

## Comparing `selfcord.py-0.2.3.tar` & `selfcord.py-0.2.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:54:38.771494 selfcord.py-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-07-14 16:54:38.771494 selfcord.py-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:54:38.767494 selfcord.py-0.2.3/selfcord/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:54:38.767494 selfcord.py-0.2.3/selfcord/api/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21098 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    23084 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/api/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/api/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:54:38.767494 selfcord.py-0.2.3/selfcord/api/voice/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/api/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/api/voice/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:54:38.771494 selfcord.py-0.2.3/selfcord/models/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29691 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:54:38.771494 selfcord.py-0.2.3/selfcord/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17064 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/utils/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:54:38.767494 selfcord.py-0.2.3/selfcord.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-07-14 16:54:38.000000 selfcord.py-0.2.3/selfcord.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-14 16:54:38.000000 selfcord.py-0.2.3/selfcord.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:54:38.000000 selfcord.py-0.2.3/selfcord.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-14 16:54:38.000000 selfcord.py-0.2.3/selfcord.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 16:54:38.000000 selfcord.py-0.2.3/selfcord.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:54:38.771494 selfcord.py-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:54:38.771494 selfcord.py-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/tests/test_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:16.460396 selfcord.py-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-07-22 16:50:16.460396 selfcord.py-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:16.456396 selfcord.py-0.2.4/selfcord/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:16.456396 selfcord.py-0.2.4/selfcord/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21185 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23084 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/api/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/api/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:16.456396 selfcord.py-0.2.4/selfcord/api/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/api/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/api/voice/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29871 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:16.456396 selfcord.py-0.2.4/selfcord/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29711 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/models/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/models/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/models/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/models/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/models/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/models/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/models/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:16.460396 selfcord.py-0.2.4/selfcord/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/utils/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/selfcord/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:16.456396 selfcord.py-0.2.4/selfcord.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-07-22 16:50:16.000000 selfcord.py-0.2.4/selfcord.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-22 16:50:16.000000 selfcord.py-0.2.4/selfcord.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:50:16.000000 selfcord.py-0.2.4/selfcord.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-22 16:50:16.000000 selfcord.py-0.2.4/selfcord.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 16:50:16.000000 selfcord.py-0.2.4/selfcord.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 16:50:16.460396 selfcord.py-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:50:16.460396 selfcord.py-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-22 16:50:04.000000 selfcord.py-0.2.4/tests/test_commands.py
```

### Comparing `selfcord.py-0.2.3/LICENSE` & `selfcord.py-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.3/PKG-INFO` & `selfcord.py-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
 Provides-Extra: voice
@@ -16,15 +16,15 @@
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.2.3-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.2.4-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: selfcord.py Version: 0.2.3 Summary: A Discord API
+Metadata-Version: 2.1 Name: selfcord.py Version: 0.2.4 Summary: A Discord API
 wrapper designed for selfbots! Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell License: MIT Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown Provides-Extra: voice License-File:
 LICENSE
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.2.3-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.2.4-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
 ## Installation Python 3.10 or higher is required. ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
```

### Comparing `selfcord.py-0.2.3/README.md` & `selfcord.py-0.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.2.3-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.2.4-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.2.3-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.2.4-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
 ## Installation Python 3.10 or higher is required. ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
```

### Comparing `selfcord.py-0.2.3/selfcord/api/errors.py` & `selfcord.py-0.2.4/selfcord/api/errors.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.3/selfcord/api/events.py` & `selfcord.py-0.2.4/selfcord/api/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,15 +400,15 @@
         Usage:
             @bot.on("voice_state_update")
         """
         if data["channel_id"] != None:
             self.session_id = data["session_id"]
             await self.bot.emit("voice_state_update")
 
-    async def handle_presence_update(self, data: dict, user: Client, http: http):
+    async def handle_presence_update(self, data: dict, user, http: http):
         """Handles the presence updating
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
 
@@ -416,24 +416,28 @@
             @bot.on("presence_update")
         """
         LISTENING = 2
         CUSTOM = 4
 
         last_modified = data.get("last_modified")
         status = data.get("status")
-        check = data.get("user").get("username")
-        if check is None:
-            user = data.get("user").get("id")
+        user = data.get("user")
+        if user is not None:
+            check = user.get("name")
+            if check is None:
+                user = data.get("user").get("id")
 
+            else:
+                user = User(user, self.bot, self.http)
         else:
-            user = User(data.get("user"), self.bot, self.http)
+            user = None
         client_status = data.get("client_status")
         activity = data.get("activities")
         activities = []
-        if activity != None:
+        if activity is not None:
             PLAYING = 0
             STREAMING = 1
             WATCHING = 3
             for activity in activity:
                 type = activity.get("type")
                 if type == PLAYING:
                     type = "PLAYING"
```

### Comparing `selfcord.py-0.2.3/selfcord/api/gateway.py` & `selfcord.py-0.2.4/selfcord/api/gateway.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.3/selfcord/api/http.py` & `selfcord.py-0.2.4/selfcord/api/http.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.3/selfcord/api/voice/voice.py` & `selfcord.py-0.2.4/selfcord/api/voice/voice.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.3/selfcord/bot.py` & `selfcord.py-0.2.4/selfcord/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -519,14 +519,34 @@
         Returns:
             Guild: The Guild object
         """
         for guild in self.user.guilds:
             if guild.id == guild_id:
                 return guild
 
+    def fetch_user(self, user_id: str) -> User | None:
+        for user in self.user.friends:
+            if user.id == user_id:
+                return user
+        for guild in self.user.guilds:
+            for user in guild.members:
+                if user.id == user_id:
+                    return user
+        for channel in self.user.private_channels:
+            if isinstance(channel, DMChannel):
+                if channel.recipient.id == user_id:
+                    return channel.recipient
+            if isinstance(channel, GroupChannel):
+                for user in channel.recipients:
+                    if user.id == user_id:
+                        return user
+        else:
+            return None
+
+
     async def get_user(self, user_id: str) -> User:
         """
         Function to retrieve user data. Probably need to be friends with them to retrieve the details.
 
         Args:
             user_id (Str): ID of the other user.
```

### Comparing `selfcord.py-0.2.3/selfcord/models/__init__.py` & `selfcord.py-0.2.4/selfcord/models/__init__.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.3/selfcord/models/channel.py` & `selfcord.py-0.2.4/selfcord/models/channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -827,15 +827,18 @@
 
     def _update(self, data: dict):
         """Updater method intended to create the attributes for the object
 
         Args:
             data (dict): JSON data from gateway
         """
-        self.recipients = [User(data, self.bot, self.http) if data.get("recipients") is not None else [] for data in data['recipients']]
+        try:
+            self.recipients = [User(data, self.bot, self.http) for data in data['recipients']]
+        except:
+            self.recipients = []
         self.name = data.get("name")
         self.owner_id = data.get("owner_id")
         self.last_message_id = data.get("last_message_id")
         self.id = data.get("id")
         self.flags = data.get("flags")
         self.icon = data.get("icon")
```

### Comparing `selfcord.py-0.2.3/selfcord/models/client.py` & `selfcord.py-0.2.4/selfcord/models/client.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.3/selfcord/models/emoji.py` & `selfcord.py-0.2.4/selfcord/models/emoji.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.3/selfcord/models/guild.py` & `selfcord.py-0.2.4/selfcord/models/guild.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.3/selfcord/models/interactions.py` & `selfcord.py-0.2.4/selfcord/models/interactions.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.3/selfcord/models/member.py` & `selfcord.py-0.2.4/selfcord/models/member.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.3/selfcord/models/message.py` & `selfcord.py-0.2.4/selfcord/models/message.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.3/selfcord/models/permission.py` & `selfcord.py-0.2.4/selfcord/models/permission.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.3/selfcord/models/role.py` & `selfcord.py-0.2.4/selfcord/models/role.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.3/selfcord/models/sessions.py` & `selfcord.py-0.2.4/selfcord/models/sessions.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.3/selfcord/models/user.py` & `selfcord.py-0.2.4/selfcord/models/user.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.3/selfcord/models/webhook.py` & `selfcord.py-0.2.4/selfcord/models/webhook.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.3/selfcord/utils/command.py` & `selfcord.py-0.2.4/selfcord/utils/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import inspect
 import re
 import shlex
 from collections import defaultdict
 from traceback import format_exception
-from typing import TYPE_CHECKING, Any, get_origin
+from typing import TYPE_CHECKING, Any
 
 from .logging import logging
 
 if TYPE_CHECKING:
     from ..api import *
     from ..bot import Bot
     from ..models import *
@@ -415,15 +415,15 @@
         args: list[Any] = []
         kwargs: dict[Any, Any] = {}
 
         if self.command.signature is not None:
             signature = self.command.signature
         if self.command_content == "":
             return args, kwargs
-        if self.command_content == None:
+        if self.command_content is None:
             return args, kwargs
         sh = shlex.shlex(self.command_content[1:], posix=False)
         sh.whitespace = " "
         sh.whitespace_split = True
         splitted = list(sh)
 
         
@@ -467,14 +467,15 @@
             args, kwargs = await self.get_arguments()
             func = self.command.func
             if func.__code__.co_varnames[0] == "self":
                 args.insert(0, self.extension)
                 args.insert(1, self)
             else:
                 args.insert(0, self)
+
         try:
             await func(*args, **kwargs)
         except Exception as e:
             error = "".join(format_exception(e, e, e.__traceback__))
             log.error(f"Could not run command \n{error}")
 
     async def reply(self, content, file_paths: list = [], delete_after: int | None = None, tts=False) -> Message:
```

### Comparing `selfcord.py-0.2.3/selfcord/utils/logging.py` & `selfcord.py-0.2.4/selfcord/utils/logging.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.3/selfcord.py.egg-info/PKG-INFO` & `selfcord.py-0.2.4/selfcord.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
 Provides-Extra: voice
@@ -16,15 +16,15 @@
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.2.3-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.2.4-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: selfcord.py Version: 0.2.3 Summary: A Discord API
+Metadata-Version: 2.1 Name: selfcord.py Version: 0.2.4 Summary: A Discord API
 wrapper designed for selfbots! Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell License: MIT Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown Provides-Extra: voice License-File:
 LICENSE
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.2.3-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.2.4-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
 ## Installation Python 3.10 or higher is required. ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
```

### Comparing `selfcord.py-0.2.3/selfcord.py.egg-info/SOURCES.txt` & `selfcord.py-0.2.4/selfcord.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.3/setup.py` & `selfcord.py-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                 "selfcord",
                 "selfcord.api",
                 "selfcord.utils",
                 "selfcord.models",
                 "selfcord.api.voice",
             ]
         ),
-        version="0.2.3",
+        version="0.2.4",
         description="A Discord API wrapper designed for selfbots!",
         readme="README.md",
         author="Shell",
         extras_require={"voice": ["pynacl==1.5.0", "opuslib==3.0.1"]},
         license="MIT",
         install_requires=[
             "aiohttp==3.7.4.post0",
```

