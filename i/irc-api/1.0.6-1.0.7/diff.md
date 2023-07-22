# Comparing `tmp/irc_api-1.0.6.tar.gz` & `tmp/irc_api-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irc_api-1.0.6.tar", last modified: Fri Jul 21 09:23:49 2023, max compression
+gzip compressed data, was "irc_api-1.0.7.tar", last modified: Sat Jul 22 11:43:32 2023, max compression
```

## Comparing `irc_api-1.0.6.tar` & `irc_api-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:23:49.172551 irc_api-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 09:23:36.000000 irc_api-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-21 09:23:49.172551 irc_api-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-21 09:23:36.000000 irc_api-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-21 09:23:36.000000 irc_api-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 09:23:49.172551 irc_api-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-21 09:23:36.000000 irc_api-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:23:49.168551 irc_api-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:23:49.168551 irc_api-1.0.6/src/irc_api/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 09:23:36.000000 irc_api-1.0.6/src/irc_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-07-21 09:23:36.000000 irc_api-1.0.6/src/irc_api/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-21 09:23:36.000000 irc_api-1.0.6/src/irc_api/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-21 09:23:36.000000 irc_api-1.0.6/src/irc_api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-21 09:23:36.000000 irc_api-1.0.6/src/irc_api/irc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-21 09:23:36.000000 irc_api-1.0.6/src/irc_api/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:23:49.172551 irc_api-1.0.6/src/irc_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-21 09:23:49.000000 irc_api-1.0.6/src/irc_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-21 09:23:49.000000 irc_api-1.0.6/src/irc_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:23:49.000000 irc_api-1.0.6/src/irc_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 09:23:49.000000 irc_api-1.0.6/src/irc_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 09:23:49.000000 irc_api-1.0.6/src/irc_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:43:32.117378 irc_api-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-22 11:43:17.000000 irc_api-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-22 11:43:32.117378 irc_api-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-22 11:43:17.000000 irc_api-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-22 11:43:17.000000 irc_api-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 11:43:32.117378 irc_api-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-22 11:43:17.000000 irc_api-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:43:32.113378 irc_api-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:43:32.113378 irc_api-1.0.7/src/irc_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 11:43:17.000000 irc_api-1.0.7/src/irc_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-07-22 11:43:17.000000 irc_api-1.0.7/src/irc_api/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-22 11:43:17.000000 irc_api-1.0.7/src/irc_api/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-22 11:43:17.000000 irc_api-1.0.7/src/irc_api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-22 11:43:17.000000 irc_api-1.0.7/src/irc_api/irc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-22 11:43:17.000000 irc_api-1.0.7/src/irc_api/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:43:32.117378 irc_api-1.0.7/src/irc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-22 11:43:32.000000 irc_api-1.0.7/src/irc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-22 11:43:32.000000 irc_api-1.0.7/src/irc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 11:43:32.000000 irc_api-1.0.7/src/irc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-22 11:43:32.000000 irc_api-1.0.7/src/irc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-22 11:43:32.000000 irc_api-1.0.7/src/irc_api.egg-info/top_level.txt
```

### Comparing `irc_api-1.0.6/LICENSE` & `irc_api-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.6/PKG-INFO` & `irc_api-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irc_api
-Version: 1.0.6
+Version: 1.0.7
 Summary: An API written in Python to make IRC bots.
 Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
 Project-URL: Documentation, https://irc-api.readthedocs.io/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `irc_api-1.0.6/README.md` & `irc_api-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.6/pyproject.toml` & `irc_api-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.6/src/irc_api/bot.py` & `irc_api-1.0.7/src/irc_api/bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,26 +30,33 @@
     commands_help : dict, public
         Same that ``callbacks`` but only with the documented commands. 
     threads : list, public
         A list of threads for the commands with ``@api.every``.
 
     Methods
     -------
-    start : NoneType, public
-        Runs the bot and connects it to IRC server.
-    send : NoneType, public
-        Send a message on the IRC server.
-    add_command : NoneType, public
-        Add a single command to the bot.
-    add_commands : NoneType, public
-        Allow to add a list of command to the bot.
-    add_commands_module : NoneType, public
-        Allow to add a module of command to the bot.
-    remove_command : NoneType, public
-        Remove a command.
+    .. automethod:: __init__
+    .. automethod:: add_command
+    .. automethod:: add_commands
+    .. automethod:: add_commands_module
+    .. automethod:: remove_commands
+    .. automethod:: send
+    .. automethod:: start
+
+    Examples
+    --------
+    Assuming the module was imported as follow: ``from irc_api import api``
+    You can create a bot::
+
+        my_bot = api.Bot(
+                irc_params=(irc.exemple.com, 6697),
+                channels=["#general", "#bot-test"],
+                prefix="!",
+                cmnd_pack1, cmnd_pack2
+            )
     """
     def __init__(
             self,
             irc_params: tuple,
             *commands_modules,
             auth: tuple=(),
             channels: list=["#general"],
@@ -68,26 +75,14 @@
             Contains the names of the channels on which the bot will connect.
         prefix : str
             The bot's prefix for named commands.
         limit : int
             The message history of the bot. By default, the bot will remind 100 messages.
         *commands_module : optionnal
             Modules of commands that you can give to the bot at it's creation.
-
-        Examples
-        --------
-        Assuming the module was imported as follow: ``from irc_api import api``
-        You can create a bot::
-
-            my_bot = api.Bot(
-                    irc_params=(irc.exemple.com, 6697),
-                    channels=["#general", "#bot-test"],
-                    prefix="!",
-                    cmnd_pack1, cmnd_pack2
-                )
         """
         self.prefix = prefix
 
         self.irc = IRC(*irc_params)
         self.history = History(limit)
         self.channels = channels
         self.auth = auth
@@ -236,17 +231,17 @@
         The function to execute when the BotCommand is called.
     events : list, public
         The list of the conditions on which the BotCommand will be called.
     desc : str, public
         The description of the BotCommand. By default, the function's docstring is used.
     cmnd_type : int, public
         The type of the command.
-        - if ``cmnd_type = 0``, the command is triggered on an event.
-        - if ``cmnd_type = 1``, the command is a named command.
-        - if ``cmnd_type = 2``, the command is a routine automatically triggered.
+        * if ``cmnd_type = 0``, the command is triggered on an event.
+        * if ``cmnd_type = 1``, the command is a named command.
+        * if ``cmnd_type = 2``, the command is a routine automatically triggered.
     bot : irc_api.bot.Bot, public
         The bot the command belongs to.
     """
     def __init__(self, name: str, func, events: list, desc: str, cmnd_type: int):
         """Constructor method.
 
         Parameters
@@ -257,17 +252,17 @@
             The function to execute when the BotCommand is called.
         events : list
             The list of the conditions on which the BotCommand will be called.
         desc : str
             The description of the BotCommand. By default, the function's docstring is used.
         cmnd_type : int
             The type of the command.
-            - if ``cmnd_type = 0``, the command is triggered on an event.
-            - if ``cmnd_type = 1``, the command is a named command.
-            - if ``cmnd_type = 2``, the command is a routine automatically triggered.
+            * if ``cmnd_type = 0``, the command is triggered on an event.
+            * if ``cmnd_type = 1``, the command is a named command.
+            * if ``cmnd_type = 2``, the command is a routine automatically triggered.
         """
         self.name = name
         self.func = func
         self.events = events
         self.cmnd_type = cmnd_type
 
         if desc:
```

### Comparing `irc_api-1.0.6/src/irc_api/commands.py` & `irc_api-1.0.7/src/irc_api/commands.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.6/src/irc_api/history.py` & `irc_api-1.0.7/src/irc_api/history.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,35 +8,27 @@
     content : list, private
         The content of the History.
     limit : int, private
         The maximum number of messages that the History stored.
 
     Methods
     -------
-    add : NoneType, public
-        Add an element to the History. If the History is full, the oldest message is deleted.
-    get : list, public
-        Returns the content of the History.
+    .. automethod:: add
+    .. automethod:: get
     """
     def __init__(self, limit: int):
-        """Initialize the History.
-        
-        Parameters
-        ----------
-        limit : int
-            The maximum number of messages the History's instance can handle.
-        """
+        """Constructor method."""
         self.__content = []
         if limit:
             self.__limit = limit
         else:
             self.__limit = 100
 
     def __len__(self):
-        """Returns the lenght of the History's instance."""
+        """Returns the length of the History's instance."""
         return len(self.__content)
 
     def add(self, elmnt):
         """Add a new element to the History's instance. If the History is full, the oldest message
         is deleted.
 
         Parameters
```

### Comparing `irc_api-1.0.6/src/irc_api/irc.py` & `irc_api-1.0.7/src/irc_api/irc.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,28 +21,21 @@
         The IRC's socket.
     inbox : Queue, private
         Queue of the incomming messages.
     handler : Thread, private
 
     Methods
     -------
-    connection : NoneType, public
-        Starts the IRC layer and manage authentication.
-    send : NoneType, public
-        Sends a message to a given channel.
-    receive : Message, public
-        Receive a new raw message and return the processed message. 
-    join : NoneType, public
-        Allows to join a given channel.
-    waitfor : str, public
-        Wait for a raw message that matches the given condition.
+    .. automethod:: __init__
+    .. automethod:: connection
+    .. automethod:: join
+    .. automethod:: receive
+    .. automethod:: send
+    .. automethod:: waitfor
 
-    handle : NoneType, private
-        Handles the ping and store incoming messages into the inbox attribute.
-    
     """
     def __init__(self, host: str, port: int):
         """Initialize an IRC wrapper.
 
         Parameters
         ----------
         host : str
```

### Comparing `irc_api-1.0.6/src/irc_api/message.py` & `irc_api-1.0.7/src/irc_api/message.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.6/src/irc_api.egg-info/PKG-INFO` & `irc_api-1.0.7/src/irc_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irc-api
-Version: 1.0.6
+Version: 1.0.7
 Summary: An API written in Python to make IRC bots.
 Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
 Project-URL: Documentation, https://irc-api.readthedocs.io/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
```

