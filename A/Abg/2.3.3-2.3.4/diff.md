# Comparing `tmp/Abg-2.3.3.tar.gz` & `tmp/Abg-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Abg-2.3.3.tar", last modified: Sun Jul 16 14:45:33 2023, max compression
+gzip compressed data, was "Abg-2.3.4.tar", last modified: Sat Jul 22 08:39:36 2023, max compression
```

## Comparing `Abg-2.3.3.tar` & `Abg-2.3.4.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.437919 Abg-2.3.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.429920 Abg-2.3.3/Abg/
--rw-r--r--   0 root         (0) root         (0)      325 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.433920 Abg-2.3.3/Abg/helpers/
--rw-r--r--   0 root         (0) root         (0)      855 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3710 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/get_user.py
--rw-r--r--   0 root         (0) root         (0)     3184 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/http_helper.py
--rw-r--r--   0 root         (0) root         (0)     2589 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/human_read.py
--rw-r--r--   0 root         (0) root         (0)     7351 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/msg_types.py
--rw-r--r--   0 root         (0) root         (0)     1279 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/parser.py
--rw-r--r--   0 root         (0) root         (0)     2533 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/pyro_progress.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/ratelimit.py
--rw-r--r--   0 root         (0) root         (0)     5335 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/helpers/string.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.433920 Abg-2.3.3/Abg/inline/
--rw-r--r--   0 root         (0) root         (0)      274 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/inline/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6105 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/inline/inline_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     4267 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/inline/inline_pagination_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/inline/reply_keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.433920 Abg-2.3.3/Abg/patch/
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.433920 Abg-2.3.3/Abg/patch/bound/
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/bound/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11979 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/bound/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.437919 Abg-2.3.3/Abg/patch/decorators/
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13387 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/decorators/adminsOnly.py
--rw-r--r--   0 root         (0) root         (0)     3723 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/decorators/on_cb.py
--rw-r--r--   0 root         (0) root         (0)     5333 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/decorators/on_cmd.py
--rw-r--r--   0 root         (0) root         (0)     2048 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/decorators/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.437919 Abg-2.3.3/Abg/patch/listen/
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/listen/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12016 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/listen/listen.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/listen/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.437919 Abg-2.3.3/Abg/patch/methods/
--rw-r--r--   0 root         (0) root         (0)      127 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/methods/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2172 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/methods/edit_message_text.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/methods/send_as_file.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-07-16 14:45:05.000000 Abg-2.3.3/Abg/patch/methods/send_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 14:45:33.429920 Abg-2.3.3/Abg.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4402 2023-07-16 14:45:33.000000 Abg-2.3.3/Abg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      967 2023-07-16 14:45:33.000000 Abg-2.3.3/Abg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-16 14:45:33.000000 Abg-2.3.3/Abg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-16 14:45:33.000000 Abg-2.3.3/Abg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4402 2023-07-16 14:45:33.437919 Abg-2.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2657 2023-07-16 14:45:05.000000 Abg-2.3.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-16 14:45:33.437919 Abg-2.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3006 2023-07-16 14:45:05.000000 Abg-2.3.3/setup.py
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.591057 Abg-2.3.4/
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.587057 Abg-2.3.4/Abg/
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      322 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/__init__.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      415 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/config.py
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.587057 Abg-2.3.4/Abg/helpers/
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      855 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/__init__.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     3710 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/get_user.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     3184 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/helpers.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     1596 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/http_helper.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     2589 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/human_read.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     7351 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/msg_types.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     1279 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/parser.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     2533 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/pyro_progress.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     2834 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/ratelimit.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     5335 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/helpers/string.py
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.587057 Abg-2.3.4/Abg/inline/
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      274 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/inline/__init__.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     6105 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/inline/inline_keyboard.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     4267 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/inline/inline_pagination_keyboard.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     1487 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/inline/reply_keyboard.py
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.587057 Abg-2.3.4/Abg/patch/
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      105 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/__init__.py
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.587057 Abg-2.3.4/Abg/patch/bound/
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)       29 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/bound/__init__.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)    12057 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/bound/message.py
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.587057 Abg-2.3.4/Abg/patch/decorators/
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      140 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/decorators/__init__.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)    13150 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/decorators/adminsOnly.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     4398 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/decorators/on_cb.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     5327 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/decorators/on_cmd.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     3675 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/decorators/utils.py
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.587057 Abg-2.3.4/Abg/patch/listen/
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)       55 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/listen/__init__.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)    12016 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/listen/listen.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      776 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/listen/utils.py
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.591057 Abg-2.3.4/Abg/patch/methods/
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)      127 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/methods/__init__.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     2172 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/methods/edit_message_text.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     1713 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/methods/send_as_file.py
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     2933 2023-07-22 08:39:01.000000 Abg-2.3.4/Abg/patch/methods/send_message.py
+drwxrwxr-x   0 Guri8837  (1000) Guri8837  (1000)        0 2023-07-22 08:39:36.587057 Abg-2.3.4/Abg.egg-info/
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     5745 2023-07-22 08:39:36.000000 Abg-2.3.4/Abg.egg-info/PKG-INFO
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     1007 2023-07-22 08:39:36.000000 Abg-2.3.4/Abg.egg-info/SOURCES.txt
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)        1 2023-07-22 08:39:36.000000 Abg-2.3.4/Abg.egg-info/dependency_links.txt
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)        1 2023-07-22 08:39:36.000000 Abg-2.3.4/Abg.egg-info/not-zip-safe
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)        4 2023-07-22 08:39:36.000000 Abg-2.3.4/Abg.egg-info/top_level.txt
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     5745 2023-07-22 08:39:36.591057 Abg-2.3.4/PKG-INFO
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     3088 2023-07-22 08:39:01.000000 Abg-2.3.4/README.md
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)       38 2023-07-22 08:39:36.591057 Abg-2.3.4/setup.cfg
+-rw-rw-r--   0 Guri8837  (1000) Guri8837  (1000)     3045 2023-07-22 08:39:01.000000 Abg-2.3.4/setup.py
```

### Comparing `Abg-2.3.3/Abg/helpers/__init__.py` & `Abg-2.3.4/Abg/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.3/Abg/helpers/get_user.py` & `Abg-2.3.4/Abg/helpers/get_user.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.3/Abg/helpers/helpers.py` & `Abg-2.3.4/Abg/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.3/Abg/helpers/http_helper.py` & `Abg-2.3.4/Abg/helpers/http_helper.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.3/Abg/helpers/human_read.py` & `Abg-2.3.4/Abg/helpers/human_read.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.3/Abg/helpers/msg_types.py` & `Abg-2.3.4/Abg/helpers/msg_types.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.3/Abg/helpers/parser.py` & `Abg-2.3.4/Abg/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.3/Abg/helpers/pyro_progress.py` & `Abg-2.3.4/Abg/helpers/pyro_progress.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.3/Abg/helpers/ratelimit.py` & `Abg-2.3.4/Abg/helpers/ratelimit.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.3/Abg/helpers/string.py` & `Abg-2.3.4/Abg/helpers/string.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.3/Abg/inline/inline_keyboard.py` & `Abg-2.3.4/Abg/inline/inline_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.3/Abg/inline/inline_pagination_keyboard.py` & `Abg-2.3.4/Abg/inline/inline_pagination_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.3/Abg/inline/reply_keyboard.py` & `Abg-2.3.4/Abg/inline/reply_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.3/Abg/patch/bound/message.py` & `Abg-2.3.4/Abg/patch/bound/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import html
 import io
 from asyncio import get_event_loop
 from asyncio import sleep as asleep
 from logging import getLogger
 from typing import Union
 
+from pyrogram.errors import ChatAdminRequired  # TopicClosed,
 from pyrogram.errors import (
-    ChatAdminRequired,
     ChatWriteForbidden,
     FloodWait,
     MessageAuthorRequired,
     MessageDeleteForbidden,
     MessageIdInvalid,
     MessageNotModified,
     MessageTooLong,
@@ -84,14 +84,16 @@
         if del_in == 0:
             return msg
         await asleep(del_in)
         return bool(await msg.delete_msg())
     except FloodWait as e:
         await asleep(e.value)
         return await reply_text(self, text, *args, **kwargs)
+    # except TopicClosed:
+    # return
     except (ChatWriteForbidden, ChatAdminRequired):
         LOGGER.info(
             f"Leaving from {self.chat.title} [{self.chat.id}] because doesn't have admin permission."
         )
         return await self.chat.leave()
```

### Comparing `Abg-2.3.3/Abg/patch/decorators/adminsOnly.py` & `Abg-2.3.4/Abg/patch/decorators/adminsOnly.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,29 @@
-import os
-import typing
-from functools import wraps
+from functools import partial, wraps
 from logging import getLogger
 from typing import Union
 
 import pyrogram
 from cachetools import TTLCache
 from pyrogram import Client
 from pyrogram.enums import ChatMemberStatus, ChatType
+from pyrogram.errors import UserNotParticipant
 from pyrogram.methods import Decorators
-from pyrogram.types import CallbackQuery, ChatPrivileges, Message
+from pyrogram.types import CallbackQuery, Message
+
+from Abg.config import Config
+
+from .utils import handle_error
 
 LOGGER = getLogger(__name__)
 
 ANON = TTLCache(maxsize=250, ttl=30)
 
-# ENV
-try:
-    OWNER_ID = int(os.environ.get("OWNER_ID"))
-except ValueError:
-    raise Exception("Your OWNER_ID env variable is not a valid integer.")
-
-try:
-    DEV_USERS = {int(x) for x in os.environ.get("DEV_USER", "").split()}
-except ValueError:
-    raise Exception("Your DEV_USER list does not contain valid integers.")
-
-DEV_USER = list(DEV_USERS)
-DEVS = list(set([int(OWNER_ID)] + DEV_USER))
+DEV_USER = list(Config.DEV_USERS)
+DEVS = list(set([int(Config.OWNER_ID)] + DEV_USER))
 
 
 async def anonymous_admin_verification(
     self, CallbackQuery: pyrogram.types.CallbackQuery
 ):
     if int(
         f"{CallbackQuery.message.chat.id}{CallbackQuery.data.split('.')[1]}"
@@ -75,221 +67,213 @@
     self,
     permissions: Union[list, str] = None,
     is_bot: bool = False,
     is_user: bool = False,
     is_both: bool = False,
     only_owner: bool = False,
     only_dev: bool = False,
-    no_reply: object = False,
-    pass_anon: typing.Union[bool, bool] = False,
+    allow_pm: bool = True,
+    allow_channel: bool = True,
 ):
     """Check for permission level to perform some operations
 
     Args:
         permissions (str, optional): permission type to check. Defaults to None.
         is_bot (bool, optional): If bot can perform the action. Defaults to False.
         is_user (bool, optional): If user can perform the action. Defaults to False.
         is_both (bool, optional): If both user and bot can perform the action. Defaults to False.
         only_owner (bool, optional): If only owner can perform the action. Defaults to False. (It's Chat Owner)
         only_dev (bool, optional): if only dev users can perform the operation. Defaults to False.
-        no_reply (boot, optional): If should not reply. Defaults to False. (when isinstance is `callback` it's give alert and if isinstance is `command` it's give reply)
-        pass_anon (boot, optional): If the user is an Anonymous Admin, then it bypasses his right check.
     """
 
     def decorator(func):
         @wraps(func)
         async def wrapper(
             abg: Client, message: Union[CallbackQuery, Message], *args, **kwargs
         ):
             if isinstance(message, CallbackQuery):
+                sender = partial(message.answer, show_alert=True)
                 msg = message.message
-            elif isinstance(message, Message):
-                msg = message
+                chat = message.message.chat
+                user = message.message.from_user
             else:
-                raise NotImplementedError(
-                    f"require_admin can't process updates with the type '{message.__name__}' yet."
-                )
-            chat = msg.chat
-            user = msg.from_user
+                sender = message.reply_text
+                msg = message
+                chat = message.chat
+                user = message.from_user
 
             if msg.chat.type == ChatType.PRIVATE and not (only_dev or only_owner):
-                return await func(abg, message, *args, *kwargs)
-
-            if msg.chat.type == ChatType.CHANNEL:
-                return await func(abg, message, *args, *kwargs)
+                if allow_pm:
+                    return await func(abg, message, *args, *kwargs)
+                return await sender("ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ ᴄᴀɴ'ᴛ ʙᴇ ᴜsᴇᴅ ɪɴ ᴀ ᴘʀɪᴠᴀᴛᴇ ᴄʜᴀᴛ.")
+
+            if msg.chat.type == ChatType.CHANNEL and not (only_dev or only_owner):
+                if allow_channel:
+                    return await func(abg, message, *args, *kwargs)
+                return await sender("ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ ᴄᴀɴ'ᴛ ʙᴇ ᴜsᴇᴅ ɪɴ ᴀ ᴄʜᴀɴɴᴇʟ.")
 
-            if not message.from_user and not pass_anon:
-                ANON[int(f"{msg.chat.id}{msg.id}")] = (
-                    message,
-                    func,
-                    permissions,
-                )
+            if not msg.from_user:
+                ANON[int(f"{msg.chat.id}{msg.id}")] = (msg, func, permissions)
                 keyboard = pyrogram.types.InlineKeyboardMarkup(
                     [
                         [
                             pyrogram.types.InlineKeyboardButton(
-                                text="ᴘʀᴏᴠᴇ ɪᴅᴇɴᴛɪᴛʏ ",
+                                text="✅ ᴘʀᴏᴠᴇ ɪᴅᴇɴᴛɪᴛʏ",
                                 callback_data=f"anon.{msg.id}",
                             ),
                         ]
                     ]
                 )
                 return await msg.reply_text(
                     "ʏᴏᴜ'ʀᴇ ᴀɴ ᴀɴᴏɴʏᴍᴏᴜs ᴀᴅᴍɪɴ, ᴄʟɪᴄᴋ ᴏɴ ᴛʜᴇ ʙᴜᴛᴛᴏɴ ʙᴇʟᴏᴡ ᴛᴏ ᴘʀᴏᴠᴇ ʏᴏᴜʀ ɪᴅᴇɴᴛɪᴛʏ",
                     reply_markup=keyboard,
                 )
 
-            bot = (
-                await abg.get_chat_member(chat.id, abg.me.id)
-                if is_bot or is_both
-                else None
-            )
-            user = (
-                await abg.get_chat_member(chat.id, user.id)
-                if is_user or is_both
-                else None
-            )
+            try:
+                bot = await chat.get_member(abg.me.id)
+                user = await chat.get_member(message.from_user.id)
+            except UserNotParticipant:
+                return await sender(
+                    f"ᴜsᴇʀ: {message.from_user.id} ɴᴏᴛ ᴍᴀᴍʙᴇʀ ᴏғ ᴛʜɪs ᴄʜᴀᴛ."
+                )
+            except BaseException as e:
+                return await handle_error(e, msg)
+
             if only_owner:
-                user_ = await msg.chat.get_member(msg.from_user.id)
-                if user_.status == ChatMemberStatus.OWNER:
+                if user.status == ChatMemberStatus.OWNER:
                     return await func(abg, message, *args, **kwargs)
-                elif no_reply:
-                    return await msg.answer(
-                        "ᴏɴʟʏ ᴄʜᴀᴛ ᴏᴡɴᴇʀ ᴄᴀɴ ᴘᴇʀғᴏʀᴍ ᴛʜɪs ᴀᴄᴛɪᴏɴ.", show_alert=True
-                    )
                 else:
-                    return await message.reply_text(
-                        "ᴏɴʟʏ ᴄʜᴀᴛ ᴏᴡɴᴇʀ ᴄᴀɴ ᴘᴇʀғᴏʀᴍ ᴛʜɪs ᴀᴄᴛɪᴏɴ."
-                    )
+                    return await sender("ᴏɴʟʏ ᴄʜᴀᴛ ᴏᴡɴᴇʀ ᴄᴀɴ ᴘᴇʀғᴏʀᴍ ᴛʜɪs ᴀᴄᴛɪᴏɴ.")
 
             if only_dev:
                 if msg.from_user.id in DEVS:
                     return await func(abg, message, *args, **kwargs)
-                elif no_reply:
-                    return await msg.answer(
-                        "ᴏɴʟʏ ᴏɴʟʏ ʙᴏᴛ ᴅᴇᴠ ᴄᴀɴ ᴘᴇʀғᴏʀᴍ ᴛʜɪs ᴀᴄᴛɪᴏɴ.", show_alert=True
-                    )
                 else:
-                    return await message.reply_text(
+                    return await sender(
                         "ᴏɴʟʏ ʙᴏᴛ ᴅᴇᴠ ᴄᴀɴ ᴘᴇʀғᴏʀᴍ ᴛʜɪs ᴀᴄᴛɪᴏɴ.",
                     )
 
+            if msg.from_user.id in DEVS:
+                return await func(abg, message, *args, **kwargs)
+
             if permissions:
                 if permissions == "can_promote_members":
                     no_permission = "ᴀᴅᴅ ɴᴇᴡ ᴀᴅᴍɪɴs"
                 elif permissions == "can_change_info":
                     no_permission = "ᴄʜᴀɴɢᴇ ɢʀᴏᴜᴘ ɪɴғᴏ"
                 elif permissions == "can_pin_messages":
                     no_permission = "ᴘɪɴ/ᴜɴᴘɪɴ ᴍᴇssᴀɢᴇs"
                 elif permissions == "can_invite_users":
                     no_permission = "ɪɴᴠɪᴛᴇ ᴜsᴇʀs ᴠɪᴀ ʟɪɴᴋ"
                 elif permissions == "can_restrict_members":
                     no_permission = "ʙᴀɴ/ᴜɴʙᴀɴ ᴜsᴇʀs"
                 elif permissions == "can_delete_messages":
                     no_permission = "ᴅᴇʟᴇᴛᴇ ᴍᴇssᴀɢᴇs"
+                elif permissions == "can_manage_chat":
+                    no_permission = "ᴍᴀɴᴀɢᴇ ᴄʜᴀᴛ"
+                elif permissions == "can_manage_video_chats":
+                    no_permission = "ᴍᴀɴᴀɢᴇ ᴠɪᴅᴇᴏ ᴄʜᴀᴛ"
+                elif permissions == "can_post_messages":
+                    no_permission = "ᴘᴏsᴛ ᴍᴇssᴀɢᴇ"
+                elif permissions == "can_edit_messages":
+                    no_permission = "ᴇᴅɪᴛ ᴍᴇssᴀɢᴇ"
                 elif permissions == "can_manage_topics":
                     no_permission = "ᴍᴀɴᴀɢᴇ ᴛᴏᴘɪᴄs"
                 elif permissions == "is_anonymous":
                     no_permission = "ʀᴇᴍᴀɪɴ ᴀɴᴏɴʏᴍᴏᴜs"
                 if is_bot:
-                    if (
-                        getattr(bot.privileges, permissions)
-                        if isinstance(bot.privileges, ChatPrivileges)
-                        else False
-                    ):
+                    if bot.status != ChatMemberStatus.ADMINISTRATOR:
+                        return await sender("ɪ ᴍᴜsᴛ ʙᴇ ᴀᴅᴍɪɴ ᴛᴏ ᴇxᴇᴄᴜᴛᴇ ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ.")
+
+                    if getattr(bot.privileges, permissions) is True:
                         return await func(abg, message, *args, **kwargs)
-                    elif no_reply:
-                        return await msg.answer(
-                            f"ɪ ᴅᴏɴ'ᴛ ʜᴀᴠᴇ ᴘᴇʀᴍɪssɪᴏɴ ᴛᴏ {no_permission}",
-                            show_alert=True,
-                        )
                     else:
-                        return await message.reply_text(
+                        return await sender(
                             f"ɪ ᴅᴏɴ'ᴛ ʜᴀᴠᴇ ᴘᴇʀᴍɪssɪᴏɴ ᴛᴏ {no_permission}."
                         )
                 if is_user:
-                    if (
-                        getattr(user.privileges, permissions)
-                        if isinstance(user.privileges, ChatPrivileges)
-                        else False or user.id in DEVS
-                    ):
-                        return await func(abg, message, *args, **kwargs)
-                    elif no_reply:
-                        return await msg.answer(
-                            f"ʏᴏᴜ ᴅᴏɴ'ᴛ ʜᴀᴠᴇ ᴘᴇʀᴍɪssɪᴏɴ ᴛᴏ {no_permission}",
-                            show_alert=True,
+                    if user.status not in [
+                        ChatMemberStatus.ADMINISTRATOR,
+                        ChatMemberStatus.OWNER,
+                    ]:
+                        return await sender(
+                            "ʏᴏᴜ ᴍᴜsᴛ ʙᴇ ᴀɴ ᴀᴅᴍɪɴɪsᴛʀᴀᴛᴏʀ ᴛᴏ ᴜsᴇ ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ."
                         )
+
+                    if getattr(user.privileges, permissions) is True:
+                        return await func(abg, message, *args, **kwargs)
                     else:
-                        return await message.reply_text(
+                        return await sender(
                             f"ʏᴏᴜ ᴅᴏɴ'ᴛ ʜᴀᴠᴇ ᴘᴇʀᴍɪssɪᴏɴ ᴛᴏ {no_permission}."
                         )
                 if is_both:
-                    if (
-                        getattr(bot.privileges, permissions)
-                        if isinstance(bot.privileges, ChatPrivileges)
-                        else False
-                    ):
+                    if bot.status != ChatMemberStatus.ADMINISTRATOR:
+                        return await sender("ɪ ᴍᴜsᴛ ʙᴇ ᴀᴅᴍɪɴ ᴛᴏ ᴇxᴇᴄᴜᴛᴇ ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ.")
+
+                    if getattr(bot.privileges, permissions) is True:
                         pass
-                    elif no_reply:
-                        return await msg.answer(
-                            f"ɪ ᴅᴏɴ'ᴛ ʜᴀᴠᴇ ᴘᴇʀᴍɪssɪᴏɴ ᴛᴏ {no_permission}",
-                            show_alert=True,
-                        )
                     else:
-                        return await message.reply_text(
+                        return await sender(
                             f"ɪ ᴅᴏɴ'ᴛ ʜᴀᴠᴇ ᴘᴇʀᴍɪssɪᴏɴ ᴛᴏ {no_permission}."
                         )
 
-                    if (
-                        getattr(user.privileges, permissions)
-                        if isinstance(user.privileges, ChatPrivileges)
-                        else False or user.id in DEVS
-                    ):
-                        pass
-                    elif no_reply:
-                        return await msg.answer(
-                            f"ʏᴏᴜ ᴅᴏɴ'ᴛ ʜᴀᴠᴇ ᴘᴇʀᴍɪssɪᴏɴ ᴛᴏ {no_permission}",
-                            show_alert=True,
+                    if user.status not in [
+                        ChatMemberStatus.ADMINISTRATOR,
+                        ChatMemberStatus.OWNER,
+                    ]:
+                        return await sender(
+                            "ʏᴏᴜ ᴍᴜsᴛ ʙᴇ ᴀɴ ᴀᴅᴍɪɴɪsᴛʀᴀᴛᴏʀ ᴛᴏ ᴜsᴇ ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ."
                         )
+
+                    if getattr(user.privileges, permissions) is True:
+                        pass
                     else:
-                        return await message.reply_text(
+                        return await sender(
                             f"ʏᴏᴜ ᴅᴏɴ'ᴛ ʜᴀᴠᴇ ᴘᴇʀᴍɪssɪᴏɴ ᴛᴏ {no_permission}."
                         )
                     return await func(abg, message, *args, **kwargs)
                 else:
                     if is_bot:
                         if bot.status == ChatMemberStatus.ADMINISTRATOR:
                             return await func(abg, message, *args, **kwargs)
                         else:
-                            return await message.reply_text("ɪ'ᴍ ɴᴏᴛ ᴀᴅᴍɪɴ ʜᴇʀᴇ.")
+                            return await sender(
+                                "ɪ ᴍᴜsᴛ ʙᴇ ᴀᴅᴍɪɴ ᴛᴏ ᴇxᴇᴄᴜᴛᴇ ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ."
+                            )
                     elif is_user:
                         if user.status in [
                             ChatMemberStatus.ADMINISTRATOR,
                             ChatMemberStatus.OWNER,
                         ]:
                             return await func(abg, message, *args, **kwargs)
-                        elif user.id in DEVS:
+                        elif msg.from_user.id in DEVS:
                             return await func(abg, message, *args, **kwargs)
                         else:
-                            return await message.reply_text("ʏᴏᴜ ᴀʀᴇ ɴᴏᴛ ᴀᴅᴍɪɴ ʜᴇʀᴇ.")
+                            return await sender(
+                                "ɪ ᴍᴜsᴛ ʙᴇ ᴀᴅᴍɪɴ ᴛᴏ ᴇxᴇᴄᴜᴛᴇ ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ."
+                            )
                     elif is_both:
                         if user.status == ChatMemberStatus.ADMINISTRATOR:
                             pass
                         else:
-                            return await message.reply_text("ɪ'ᴍ ɴᴏᴛ ᴀᴅᴍɪɴ ʜᴇʀᴇ.")
+                            return await sender(
+                                "ɪ ᴍᴜsᴛ ʙᴇ ᴀᴅᴍɪɴ ᴛᴏ ᴇxᴇᴄᴜᴛᴇ ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ."
+                            )
 
                         if user.status in [
                             ChatMemberStatus.ADMINISTRATOR,
                             ChatMemberStatus.OWNER,
                         ]:
                             pass
-                        elif user.id in DEVS:
+                        elif msg.from_user.id in DEVS:
                             pass
                         else:
-                            return await message.reply_text("ʏᴏᴜ ᴀʀᴇ ɴᴏᴛ ᴀᴅᴍɪɴ ʜᴇʀᴇ.")
+                            return await sender(
+                                "ʏᴏᴜ ᴍᴜsᴛ ʙᴇ ᴀɴ ᴀᴅᴍɪɴɪsᴛʀᴀᴛᴏʀ ᴛᴏ ᴜsᴇ ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ."
+                            )
                         return await func(abg, message, *args, **kwargs)
 
         self.add_handler(
             pyrogram.handlers.CallbackQueryHandler(
                 anonymous_admin_verification,
                 pyrogram.filters.regex("^anon."),
             ),
```

### Comparing `Abg-2.3.3/Abg/patch/decorators/on_cmd.py` & `Abg-2.3.4/Abg/patch/decorators/on_cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import asyncio
 import typing
 from logging import getLogger
 
 import pyrogram
+from pyrogram import Client
 from pyrogram.errors import FloodWait, Forbidden, SlowmodeWait
 from pyrogram.methods import Decorators
 
 from .utils import handle_error
 
-HANDLER = ["/", "!", "~", ".", "+", "*", "$"]
+HANDLER = ["/", "!", "~", ".", "+", "*", "$", " @"]
 
 LOGGER = getLogger(__name__)
 
 
 def command(
     self,
     command: typing.Union[str, list],
@@ -54,15 +55,15 @@
     #### Example
     .. code-block:: python
         import pyrogram
 
         app = pyrogram.Client()
 
         @app.on_cmd("start", is_disabled=False, group_only=False, pm_only=False, self_admin=False, self_only=False, pyrogram.filters.chat("777000") and pyrogram.filters.text)
-        async def start(client, message):
+        async def start(abg: Client, message):
             await message.reply_text(f"Hello {message.from_user.mention}")
     """
     if handler is None:
         handler = HANDLER
     if filter:
         if self_only:
             filter = (
@@ -82,50 +83,48 @@
                 pyrogram.filters.command(command, prefixes=handler)
                 & pyrogram.filters.me
             )
         else:
             filter = pyrogram.filters.command(command, prefixes=handler)
 
     def wrapper(func):
-        async def decorator(client, message: pyrogram.types.Message):
+        async def decorator(abg: Client, message: pyrogram.types.Message):
             if is_disabled:
                 return await message.reply_text(
                     "sᴏʀʀʏ, ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ ʜᴀs ʙᴇᴇɴ ᴅɪsᴀʙʟᴇᴅ ʙʏ ᴏᴡɴᴇʀ."
                 )
             if self_admin and message.chat.type != pyrogram.enums.ChatType.SUPERGROUP:
                 return await message.reply_text(
                     "ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ ᴄᴀɴ ʙᴇ ᴜsᴇᴅ ɪɴ sᴜᴘᴇʀɢʀᴏᴜᴘs ᴏɴʟʏ."
                 )
             if self_admin:
-                me = await client.get_chat_member(
-                    message.chat.id, (await client.get_me()).id
-                )
+                me = await abg.get_chat_member(message.chat.id, (await abg.get_me()).id)
                 if me.status not in (
                     pyrogram.enums.ChatMemberStatus.OWNER,
                     pyrogram.enums.ChatMemberStatus.ADMINISTRATOR,
                 ):
                     return await message.reply_text(
                         "ɪ ᴍᴜsᴛ ʙᴇ ᴀᴅᴍɪɴ ᴛᴏ ᴇxᴇᴄᴜᴛᴇ ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ"
                     )
             if group_only and message.chat.type != pyrogram.enums.ChatType.SUPERGROUP:
                 return await message.reply_text(
                     "ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ ᴄᴀɴ ʙᴇ ᴜsᴇᴅ ɪɴ sᴜᴘᴇʀɢʀᴏᴜᴘs ᴏɴʟʏ."
                 )
             if pm_only and message.chat.type != pyrogram.enums.ChatType.PRIVATE:
                 return await message.reply_text("ᴛʜɪs ᴄᴏᴍᴍᴀɴᴅ ᴄᴀɴ ʙᴇ ᴜsᴇᴅ ɪɴ ᴘᴍs ᴏɴʟʏ.")
             try:
-                await func(client, message)
+                await func(abg, message)
             except FloodWait as fw:
                 LOGGER.warning(str(fw))
                 await asyncio.sleep(fw.value)
             except (Forbidden, SlowmodeWait):
                 LOGGER.info(
-                    f"Leaving chat : {message.chat.title} [{message.chat.id}], because doesn't have admin permission."
+                    f"Leaving chat : {message.chat.title} [{message.chat.id}], because doesn't have write permission."
                 )
-                return await client.leave_chat(message.chat.id)
+                return await abg.leave_chat(message.chat.id)
             except BaseException as e:
                 return await handle_error(e, message)
 
         self.add_handler(
             pyrogram.handlers.MessageHandler(callback=decorator, filters=filter)
         )
         return decorator
```

### Comparing `Abg-2.3.3/Abg/patch/listen/listen.py` & `Abg-2.3.4/Abg/patch/listen/listen.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.3/Abg/patch/listen/utils.py` & `Abg-2.3.4/Abg/patch/listen/utils.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.3/Abg/patch/methods/edit_message_text.py` & `Abg-2.3.4/Abg/patch/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.3/Abg/patch/methods/send_as_file.py` & `Abg-2.3.4/Abg/patch/methods/send_as_file.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.3/Abg/patch/methods/send_message.py` & `Abg-2.3.4/Abg/patch/methods/send_message.py`

 * *Files identical despite different names*

### Comparing `Abg-2.3.3/Abg.egg-info/PKG-INFO` & `Abg-2.3.4/Abg.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,276 +1,360 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 4162 670a  : 2.1.Name: Abg.
-00000020: 5665 7273 696f 6e3a 2032 2e33 2e33 0a53  Version: 2.3.3.S
-00000030: 756d 6d61 7279 3a20 5465 6c65 6772 616d  ummary: Telegram
-00000040: 2062 6f74 2068 656c 7065 7273 0a48 6f6d   bot helpers.Hom
-00000050: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
-00000060: 6769 7468 7562 2e63 6f6d 2f41 6269 7368  github.com/Abish
-00000070: 6e6f 6936 392f 4162 670a 4175 7468 6f72  noi69/Abg.Author
-00000080: 3a20 4162 6973 686e 6f69 0a41 7574 686f  : Abishnoi.Autho
-00000090: 722d 656d 6169 6c3a 2041 6269 7368 6e6f  r-email: Abishno
-000000a0: 6936 3940 4162 672e 6f72 670a 4c69 6365  i69@Abg.org.Lice
-000000b0: 6e73 653a 204d 4954 0a44 6f77 6e6c 6f61  nse: MIT.Downloa
-000000c0: 642d 5552 4c3a 2068 7474 7073 3a2f 2f67  d-URL: https://g
-000000d0: 6974 6875 622e 636f 6d2f 4162 6973 686e  ithub.com/Abishn
-000000e0: 6f69 3639 2f41 6267 2f72 656c 6561 7365  oi69/Abg/release
-000000f0: 732f 6c61 7465 7374 0a50 726f 6a65 6374  s/latest.Project
-00000100: 2d55 524c 3a20 5472 6163 6b65 722c 2068  -URL: Tracker, h
-00000110: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000120: 6d2f 4162 6973 686e 6f69 3639 2f41 6267  m/Abishnoi69/Abg
-00000130: 2f69 7373 7565 730a 5072 6f6a 6563 742d  /issues.Project-
-00000140: 5552 4c3a 2043 6f6d 6d75 6e69 7479 2c20  URL: Community, 
-00000150: 6874 7470 733a 2f2f 742e 6d65 2f41 6267  https://t.me/Abg
-00000160: 7079 0a50 726f 6a65 6374 2d55 524c 3a20  py.Project-URL: 
-00000170: 536f 7572 6365 2c20 6874 7470 733a 2f2f  Source, https://
-00000180: 6769 7468 7562 2e63 6f6d 2f41 6269 7368  github.com/Abish
-00000190: 6e6f 6936 392f 4162 670a 5072 6f6a 6563  noi69/Abg.Projec
-000001a0: 742d 5552 4c3a 2044 6f63 756d 656e 7461  t-URL: Documenta
-000001b0: 7469 6f6e 2c20 6874 7470 733a 2f2f 6769  tion, https://gi
-000001c0: 7468 7562 2e63 6f6d 2f41 6269 7368 6e6f  thub.com/Abishno
-000001d0: 6936 392f 4162 672f 7472 6565 2f6d 6173  i69/Abg/tree/mas
-000001e0: 7465 722f 646f 6365 0a4b 6579 776f 7264  ter/doce.Keyword
-000001f0: 733a 2074 656c 6567 7261 6d20 626f 7420  s: telegram bot 
-00000200: 6368 6174 206d 6573 7365 6e67 6572 206d  chat messenger m
-00000210: 7470 726f 746f 2061 7069 2063 6c69 656e  tproto api clien
-00000220: 7420 6c69 6272 6172 7920 7079 7468 6f6e  t library python
-00000230: 2063 6f6e 7665 7273 6174 696f 6e20 6b65   conversation ke
-00000240: 7962 6f61 7264 2075 7365 7262 6f74 2070  yboard userbot p
-00000250: 6174 6368 2062 6f74 6170 6920 6874 7470  atch botapi http
-00000260: 730a 506c 6174 666f 726d 3a20 554e 4b4e  s.Platform: UNKN
-00000270: 4f57 4e0a 436c 6173 7369 6669 6572 3a20  OWN.Classifier: 
-00000280: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
-00000290: 7573 203a 3a20 3520 2d20 5072 6f64 7563  us :: 5 - Produc
-000002a0: 7469 6f6e 2f53 7461 626c 650a 436c 6173  tion/Stable.Clas
-000002b0: 7369 6669 6572 3a20 496e 7465 6e64 6564  sifier: Intended
-000002c0: 2041 7564 6965 6e63 6520 3a3a 2044 6576   Audience :: Dev
-000002d0: 656c 6f70 6572 730a 436c 6173 7369 6669  elopers.Classifi
-000002e0: 6572 3a20 4e61 7475 7261 6c20 4c61 6e67  er: Natural Lang
-000002f0: 7561 6765 203a 3a20 456e 676c 6973 680a  uage :: English.
-00000300: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
-00000310: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000320: 4f53 2049 6e64 6570 656e 6465 6e74 0a43  OS Independent.C
-00000330: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000340: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000350: 3a3a 2050 7974 686f 6e0a 436c 6173 7369  :: Python.Classi
-00000360: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000370: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000380: 7468 6f6e 203a 3a20 330a 436c 6173 7369  thon :: 3.Classi
-00000390: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000003a0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000003b0: 7468 6f6e 203a 3a20 332e 370a 436c 6173  thon :: 3.7.Clas
-000003c0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-000003d0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000003e0: 5079 7468 6f6e 203a 3a20 332e 380a 436c  Python :: 3.8.Cl
-000003f0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000400: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000410: 3a20 5079 7468 6f6e 203a 3a20 332e 390a  : Python :: 3.9.
-00000420: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000430: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000440: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000450: 3130 0a43 6c61 7373 6966 6965 723a 2050  10.Classifier: P
-00000460: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000470: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000480: 2033 2e31 310a 436c 6173 7369 6669 6572   3.11.Classifier
-00000490: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-000004a0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000004b0: 203a 3a20 496d 706c 656d 656e 7461 7469   :: Implementati
-000004c0: 6f6e 0a43 6c61 7373 6966 6965 723a 2050  on.Classifier: P
-000004d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000004e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000004f0: 2049 6d70 6c65 6d65 6e74 6174 696f 6e20   Implementation 
-00000500: 3a3a 2043 5079 7468 6f6e 0a43 6c61 7373  :: CPython.Class
-00000510: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000520: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000530: 7974 686f 6e20 3a3a 2049 6d70 6c65 6d65  ython :: Impleme
-00000540: 6e74 6174 696f 6e20 3a3a 2050 7950 790a  ntation :: PyPy.
-00000550: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
-00000560: 6320 3a3a 2049 6e74 6572 6e65 740a 436c  c :: Internet.Cl
-00000570: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-00000580: 3a3a 2043 6f6d 6d75 6e69 6361 7469 6f6e  :: Communication
-00000590: 730a 436c 6173 7369 6669 6572 3a20 546f  s.Classifier: To
-000005a0: 7069 6320 3a3a 2043 6f6d 6d75 6e69 6361  pic :: Communica
-000005b0: 7469 6f6e 7320 3a3a 2043 6861 740a 436c  tions :: Chat.Cl
-000005c0: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-000005d0: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
-000005e0: 6c6f 706d 656e 7420 3a3a 204c 6962 7261  lopment :: Libra
-000005f0: 7269 6573 0a43 6c61 7373 6966 6965 723a  ries.Classifier:
-00000600: 2054 6f70 6963 203a 3a20 536f 6674 7761   Topic :: Softwa
-00000610: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
-00000620: 3a20 4c69 6272 6172 6965 7320 3a3a 2050  : Libraries :: P
-00000630: 7974 686f 6e20 4d6f 6475 6c65 730a 436c  ython Modules.Cl
-00000640: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-00000650: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
-00000660: 6c6f 706d 656e 7420 3a3a 204c 6962 7261  lopment :: Libra
-00000670: 7269 6573 203a 3a20 4170 706c 6963 6174  ries :: Applicat
-00000680: 696f 6e20 4672 616d 6577 6f72 6b73 0a52  ion Frameworks.R
-00000690: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
-000006a0: 7e3d 332e 370a 4465 7363 7269 7074 696f  ~=3.7.Descriptio
-000006b0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-000006c0: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a23  text/markdown..#
-000006d0: 20e1 b480 ca99 c9a2 203a 2d3e 205b 215b   ....... :-> [![
-000006e0: 446f 776e 6c6f 6164 735d 2868 7474 7073  Downloads](https
-000006f0: 3a2f 2f73 7461 7469 632e 7065 7079 2e74  ://static.pepy.t
-00000700: 6563 682f 7065 7273 6f6e 616c 697a 6564  ech/personalized
-00000710: 2d62 6164 6765 2f61 6267 3f70 6572 696f  -badge/abg?perio
-00000720: 643d 746f 7461 6c26 756e 6974 733d 6162  d=total&units=ab
-00000730: 6272 6576 6961 7469 6f6e 266c 6566 745f  breviation&left_
-00000740: 636f 6c6f 723d 626c 6163 6b26 7269 6768  color=black&righ
-00000750: 745f 636f 6c6f 723d 626c 6163 6b26 6c65  t_color=black&le
-00000760: 6674 5f74 6578 743d 446f 776e 6c6f 6164  ft_text=Download
-00000770: 733a 295d 2868 7474 7073 3a2f 2f70 6570  s:)](https://pep
-00000780: 792e 7465 6368 2f70 726f 6a65 6374 2f61  y.tech/project/a
-00000790: 6267 290a 0a3e 200a 2323 2320 e280 a220  bg)..> .### ... 
-000007a0: 4162 670a 0a60 6060 7079 7468 6f6e 0a66  Abg..```python.f
-000007b0: 726f 6d20 7079 726f 6772 616d 2069 6d70  rom pyrogram imp
-000007c0: 6f72 7420 6669 6c74 6572 732c 2043 6c69  ort filters, Cli
-000007d0: 656e 740a 6672 6f6d 2070 7972 6f67 7261  ent.from pyrogra
-000007e0: 6d2e 7479 7065 7320 696d 706f 7274 2043  m.types import C
-000007f0: 616c 6c62 6163 6b51 7565 7279 2c20 4d65  allbackQuery, Me
-00000800: 7373 6167 650a 6672 6f6d 2041 6267 2069  ssage.from Abg i
-00000810: 6d70 6f72 7420 7061 7463 6820 2023 2074  mport patch  # t
-00000820: 7970 6520 3a20 6967 6e6f 7265 0a66 726f  ype : ignore.fro
-00000830: 6d20 4162 672e 6865 6c70 6572 7320 696d  m Abg.helpers im
-00000840: 706f 7274 2069 6b62 0a0a 6170 7020 3d20  port ikb..app = 
-00000850: 436c 6965 6e74 2822 6d79 5f61 6363 6f75  Client("my_accou
-00000860: 6e74 2229 0a0a 4061 7070 2e6f 6e5f 636d  nt")..@app.on_cm
-00000870: 6428 226d 7969 6e66 6f22 290a 6173 796e  d("myinfo").asyn
-00000880: 6320 6465 6620 6d79 5f69 6e66 6f28 7365  c def my_info(se
-00000890: 6c66 3a20 436c 6965 6e74 2c20 6374 783a  lf: Client, ctx:
-000008a0: 204d 6573 7361 6765 293a 0a20 2020 2069   Message):.    i
-000008b0: 6620 6e6f 7420 6374 782e 6672 6f6d 5f75  f not ctx.from_u
-000008c0: 7365 723a 0a20 2020 2020 2020 2072 6574  ser:.        ret
-000008d0: 7572 6e0a 2020 2020 6e61 6d65 203d 2061  urn.    name = a
-000008e0: 7761 6974 2063 7478 2e63 6861 742e 6173  wait ctx.chat.as
-000008f0: 6b28 2254 7970 6520 596f 7572 204e 616d  k("Type Your Nam
-00000900: 6522 290a 2020 2020 6167 6520 3d20 6177  e").    age = aw
-00000910: 6169 7420 6374 782e 6368 6174 2e61 736b  ait ctx.chat.ask
-00000920: 2822 5479 7065 2079 6f75 7220 6167 6522  ("Type your age"
-00000930: 290a 2020 2020 6164 6420 3d20 6177 6169  ).    add = awai
-00000940: 7420 6374 782e 6368 6174 2e61 736b 2822  t ctx.chat.ask("
-00000950: 5479 7065 2079 6f75 7220 6164 6472 6573  Type your addres
-00000960: 7322 290a 2020 2020 2320 796f 7520 6361  s").    # you ca
-00000970: 6e20 616c 736f 2075 7365 203a 2063 7478  n also use : ctx
-00000980: 2e72 6570 6c79 5f74 6578 7428 2e2e 2e29  .reply_text(...)
-00000990: 0a20 2020 2061 7761 6974 2073 656c 662e  .    await self.
-000009a0: 7365 6e64 5f6d 7367 280a 2020 2020 2020  send_msg(.      
-000009b0: 2020 6368 6174 5f69 643d 6374 782e 6368    chat_id=ctx.ch
-000009c0: 6174 2e69 642c 0a20 2020 2020 2020 2074  at.id,.        t
-000009d0: 6578 743d 6622 596f 7572 206e 616d 6520  ext=f"Your name 
-000009e0: 6973 3a20 7b6e 616d 652e 7465 7874 7d5c  is: {name.text}\
-000009f0: 6e59 6f75 7220 6167 6520 6973 3a20 7b61  nYour age is: {a
-00000a00: 6765 2e74 6578 747d 5c6e 796f 7572 2061  ge.text}\nyour a
-00000a10: 6464 7265 7373 2069 733a 207b 6164 642e  ddress is: {add.
-00000a20: 7465 7874 7d22 2c0a 2020 2020 2020 2020  text}",.        
-00000a30: 7265 706c 795f 6d61 726b 7570 3d69 6b62  reply_markup=ikb
-00000a40: 285b 5b28 22ca 99e1 b49c e1b4 9be1 b49b  ([[("...........
-00000a50: e1b4 8fc9 b422 2c20 2268 656c 6c6f 2229  .....", "hello")
-00000a60: 5d5d 292c 0a20 2020 2029 0a0a 2320 6361  ]]),.    )..# ca
-00000a70: 6c6c 6261 636b 200a 4061 7070 2e6f 6e5f  llback .@app.on_
-00000a80: 6362 2822 6865 6c6c 6f22 290a 6173 796e  cb("hello").asyn
-00000a90: 6320 6465 6620 6865 6c6c 6f28 633a 2043  c def hello(c: C
-00000aa0: 6c69 656e 742c 2071 3a20 4361 6c6c 6261  lient, q: Callba
-00000ab0: 636b 5175 6572 7929 3a0a 2020 2020 6177  ckQuery):.    aw
-00000ac0: 6169 7420 712e 616e 7377 6572 2822 4865  ait q.answer("He
-00000ad0: 6c6c 6f20 4672 6f6d 2041 6267 222c 2073  llo From Abg", s
-00000ae0: 686f 775f 616c 6572 743d 5472 7565 290a  how_alert=True).
-00000af0: 0a20 2061 7070 2e72 756e 2829 0a60 6060  .  app.run().```
-00000b00: 0a3e 0a23 2323 20e2 80a2 2055 7365 7220  .>.### ... User 
-00000b10: 5269 6768 7473 200a 0a60 6060 7079 7468  Rights ..```pyth
-00000b20: 6f6e 0a66 726f 6d20 4162 6720 696d 706f  on.from Abg impo
-00000b30: 7274 2070 6174 6368 2020 2320 616c 6c20  rt patch  # all 
-00000b40: 7061 7463 680a 6672 6f6d 2070 7972 6f67  patch.from pyrog
-00000b50: 7261 6d2e 7479 7065 7320 696d 706f 7274  ram.types import
-00000b60: 204d 6573 7361 6765 0a66 726f 6d20 7079   Message.from py
-00000b70: 726f 6772 616d 2069 6d70 6f72 7420 436c  rogram import Cl
-00000b80: 6965 6e74 0a0a 6170 7020 3d20 436c 6965  ient..app = Clie
-00000b90: 6e74 2822 6d79 5f61 6363 6f75 6e74 2229  nt("my_account")
-00000ba0: 0a0a 4061 7070 2e6f 6e5f 636d 6428 2264  ..@app.on_cmd("d
-00000bb0: 656c 222c 2067 726f 7570 5f6f 6e6c 793d  el", group_only=
-00000bc0: 5472 7565 290a 4061 7070 2e61 646d 696e  True).@app.admin
-00000bd0: 734f 6e6c 7928 7065 726d 6973 7369 6f6e  sOnly(permission
-00000be0: 733d 2263 616e 5f64 656c 6574 655f 6d65  s="can_delete_me
-00000bf0: 7373 6167 6573 222c 2069 735f 626f 7468  ssages", is_both
-00000c00: 3d54 7275 6529 0a61 7379 6e63 2064 6566  =True).async def
-00000c10: 2064 656c 5f6d 7367 2863 3a20 436c 6965   del_msg(c: Clie
-00000c20: 6e74 2c20 6d3a 204d 6573 7361 6765 293a  nt, m: Message):
-00000c30: 0a20 2020 2069 6620 6d2e 7265 706c 795f  .    if m.reply_
-00000c40: 746f 5f6d 6573 7361 6765 3a0a 2020 2020  to_message:.    
-00000c50: 2020 2020 6177 6169 7420 6d2e 6465 6c65      await m.dele
-00000c60: 7465 2829 0a20 2020 2020 2020 2061 7761  te().        awa
-00000c70: 6974 2063 2e64 656c 6574 655f 6d65 7373  it c.delete_mess
-00000c80: 6167 6573 280a 2020 2020 2020 2020 2020  ages(.          
-00000c90: 2020 6368 6174 5f69 643d 6d2e 6368 6174    chat_id=m.chat
-00000ca0: 2e69 642c 0a20 2020 2020 2020 2020 2020  .id,.           
-00000cb0: 206d 6573 7361 6765 5f69 6473 3d6d 2e72   message_ids=m.r
-00000cc0: 6570 6c79 5f74 6f5f 6d65 7373 6167 652e  eply_to_message.
-00000cd0: 6964 2c0a 2020 2020 2020 2020 290a 2020  id,.        ).  
-00000ce0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00000cf0: 6177 6169 7420 6d2e 7265 706c 795f 7465  await m.reply_te
-00000d00: 7874 2874 6578 743d 22e1 b4a1 ca9c e1b4  xt(text=".......
-00000d10: 80e1 b49b 20e1 b485 e1b4 8f20 ca8f e1b4  .... ...... ....
-00000d20: 8fe1 b49c 20e1 b4a1 e1b4 80c9 b4c9 b4e1  .... ...........
-00000d30: b480 20e1 b485 e1b4 87ca 9fe1 b487 e1b4  .. .............
-00000d40: 9be1 b487 3f22 290a 2020 2020 7265 7475  ....?").    retu
-00000d50: 726e 0a20 200a 2020 6170 702e 7275 6e28  rn.  .  app.run(
-00000d60: 290a 6060 600a 0a0a 3e0a 2323 2320 e280  ).```...>.### ..
-00000d70: a220 4b65 7962 6f61 7264 730a 0a60 6060  . Keyboards..```
-00000d80: 7079 7468 6f6e 0a66 726f 6d20 4162 672e  python.from Abg.
-00000d90: 696e 6c69 6e65 2069 6d70 6f72 7420 496e  inline import In
-00000da0: 6c69 6e65 4b65 7962 6f61 7264 2c20 496e  lineKeyboard, In
-00000db0: 6c69 6e65 4275 7474 6f6e 0a0a 0a6b 6579  lineButton...key
-00000dc0: 626f 6172 6420 3d20 496e 6c69 6e65 4b65  board = InlineKe
-00000dd0: 7962 6f61 7264 2872 6f77 5f77 6964 7468  yboard(row_width
-00000de0: 3d33 290a 6b65 7962 6f61 7264 2e61 6464  =3).keyboard.add
-00000df0: 280a 2020 2020 496e 6c69 6e65 4275 7474  (.    InlineButt
-00000e00: 6f6e 2827 3127 2c20 2769 6e6c 696e 655f  on('1', 'inline_
-00000e10: 6b65 7962 6f61 7264 3a31 2729 2c0a 2020  keyboard:1'),.  
-00000e20: 2020 496e 6c69 6e65 4275 7474 6f6e 2827    InlineButton('
-00000e30: 3227 2c20 2769 6e6c 696e 655f 6b65 7962  2', 'inline_keyb
-00000e40: 6f61 7264 3a32 2729 2c0a 2020 2020 496e  oard:2'),.    In
-00000e50: 6c69 6e65 4275 7474 6f6e 2827 3327 2c20  lineButton('3', 
-00000e60: 2769 6e6c 696e 655f 6b65 7962 6f61 7264  'inline_keyboard
-00000e70: 3a33 2729 2c0a 2020 2020 496e 6c69 6e65  :3'),.    Inline
-00000e80: 4275 7474 6f6e 2827 3427 2c20 2769 6e6c  Button('4', 'inl
-00000e90: 696e 655f 6b65 7962 6f61 7264 3a34 2729  ine_keyboard:4')
-00000ea0: 2c0a 2020 2020 496e 6c69 6e65 4275 7474  ,.    InlineButt
-00000eb0: 6f6e 2827 3527 2c20 2769 6e6c 696e 655f  on('5', 'inline_
-00000ec0: 6b65 7962 6f61 7264 3a35 2729 2c0a 2020  keyboard:5'),.  
-00000ed0: 2020 496e 6c69 6e65 4275 7474 6f6e 2827    InlineButton('
-00000ee0: 3627 2c20 2769 6e6c 696e 655f 6b65 7962  6', 'inline_keyb
-00000ef0: 6f61 7264 3a36 2729 2c0a 2020 2020 496e  oard:6'),.    In
-00000f00: 6c69 6e65 4275 7474 6f6e 2827 3727 2c20  lineButton('7', 
-00000f10: 2769 6e6c 696e 655f 6b65 7962 6f61 7264  'inline_keyboard
-00000f20: 3a37 2729 0a29 0a60 6060 0a0a 2323 2323  :7').).```..####
-00000f30: 2052 6573 756c 740a 0a3c 703e 3c69 6d67   Result..<p><img
-00000f40: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00000f50: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00000f60: 656e 742e 636f 6d2f 4162 6973 686e 6f69  ent.com/Abishnoi
-00000f70: 3639 2f41 6267 2f6d 6173 7465 722f 646f  69/Abg/master/do
-00000f80: 6365 2f69 6d61 6765 732f 6164 645f 696e  ce/images/add_in
-00000f90: 6c69 6e65 5f62 7574 746f 6e2e 706e 6722  line_button.png"
-00000fa0: 2061 6c74 3d22 6164 645f 696e 6c69 6e65   alt="add_inline
-00000fb0: 5f62 7574 746f 6e22 3e3c 2f70 3e0a 0a0a  _button"></p>...
-00000fc0: 2323 2320 c9aa c9b4 73e1 b49b e1b4 80ca  ### ....s.......
-00000fd0: 9fca 9fc9 aac9 b4c9 a220 3a2d 3e0a 0a60  ......... :->..`
-00000fe0: 6060 6261 7368 0a70 6970 2069 6e73 7461  ``bash.pip insta
-00000ff0: 6c6c 202d 5520 4162 670a 6060 600a 0ae2  ll -U Abg.```...
-00001000: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00001010: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00001020: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00001030: 9481 e294 81e2 9481 e294 810a 2323 20c9  ............## .
-00001040: b4e1 b48f e1b4 9be1 b487 203a 2d3e 0a0a  .......... :->..
-00001050: 2d20 5468 6973 206c 6962 7261 7279 2069  - This library i
-00001060: 7320 6d61 6465 2066 6f72 206d 7920 7065  s made for my pe
-00001070: 7273 6f6e 616c 2050 726f 6a65 6374 2073  rsonal Project s
-00001080: 6f20 646f 6e27 7420 7461 6b65 2069 7420  o don't take it 
-00001090: 6465 6570 6c79 202e 0a2d 204d 7920 5072  deeply ..- My Pr
-000010a0: 6f6a 6563 7420 5b40 4775 6172 6478 526f  oject [@GuardxRo
-000010b0: 626f 745d 2868 7474 7073 3a2f 2f74 2e6d  bot](https://t.m
-000010c0: 652f 4775 6172 6478 526f 626f 7429 200a  e/GuardxRobot) .
-000010d0: 0a2d 20e1 b487 c9b4 e1b4 8ae1 b48f ca8f  .- .............
-000010e0: 20ca 99e1 b480 ca99 ca8f 20e2 99a1 200a   ......... ... .
-000010f0: 0ae2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00001100: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00001110: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00001120: 81e2 9481 e294 81e2 9481 e294 8120 0a0a  ............. ..
-00001130: 0a0a                                     ..
+00000020: 5665 7273 696f 6e3a 2032 2e33 2e34 0a53  Version: 2.3.4.S
+00000030: 756d 6d61 7279 3a20 6164 642d 6f6e 2066  ummary: add-on f
+00000040: 6f72 2050 7972 6f67 7261 6d20 7c7c 2054  or Pyrogram || T
+00000050: 656c 6567 7261 6d20 626f 7420 6865 6c70  elegram bot help
+00000060: 6572 7320 7c7c 2045 6173 7920 626f 7474  ers || Easy bott
+00000070: 696e 670a 486f 6d65 2d70 6167 653a 2068  ing.Home-page: h
+00000080: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000090: 6d2f 4162 6973 686e 6f69 3639 2f41 6267  m/Abishnoi69/Abg
+000000a0: 0a41 7574 686f 723a 2041 6269 7368 6e6f  .Author: Abishno
+000000b0: 690a 4175 7468 6f72 2d65 6d61 696c 3a20  i.Author-email: 
+000000c0: 4162 6973 686e 6f69 3639 4041 6267 2e6f  Abishnoi69@Abg.o
+000000d0: 7267 0a4c 6963 656e 7365 3a20 4d49 540a  rg.License: MIT.
+000000e0: 446f 776e 6c6f 6164 2d55 524c 3a20 6874  Download-URL: ht
+000000f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000100: 2f41 6269 7368 6e6f 6936 392f 4162 672f  /Abishnoi69/Abg/
+00000110: 7265 6c65 6173 6573 2f6c 6174 6573 740a  releases/latest.
+00000120: 5072 6f6a 6563 742d 5552 4c3a 2054 7261  Project-URL: Tra
+00000130: 636b 6572 2c20 6874 7470 733a 2f2f 6769  cker, https://gi
+00000140: 7468 7562 2e63 6f6d 2f41 6269 7368 6e6f  thub.com/Abishno
+00000150: 6936 392f 4162 672f 6973 7375 6573 0a50  i69/Abg/issues.P
+00000160: 726f 6a65 6374 2d55 524c 3a20 436f 6d6d  roject-URL: Comm
+00000170: 756e 6974 792c 2068 7474 7073 3a2f 2f74  unity, https://t
+00000180: 2e6d 652f 4162 6770 790a 5072 6f6a 6563  .me/Abgpy.Projec
+00000190: 742d 5552 4c3a 2053 6f75 7263 652c 2068  t-URL: Source, h
+000001a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000001b0: 6d2f 4162 6973 686e 6f69 3639 2f41 6267  m/Abishnoi69/Abg
+000001c0: 0a50 726f 6a65 6374 2d55 524c 3a20 446f  .Project-URL: Do
+000001d0: 6375 6d65 6e74 6174 696f 6e2c 2068 7474  cumentation, htt
+000001e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000001f0: 4162 6973 686e 6f69 3639 2f41 6267 2f74  Abishnoi69/Abg/t
+00000200: 7265 652f 6d61 7374 6572 2f64 6f63 650a  ree/master/doce.
+00000210: 4465 7363 7269 7074 696f 6e3a 203c 7020  Description: <p 
+00000220: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+00000230: 2020 2020 2020 2020 3c62 3e20 4142 4720          <b> ABG 
+00000240: 3c2f 623e 0a20 2020 2020 2020 203c 2f70  </b>.        </p
+00000250: 3e0a 2020 2020 2020 2020 0a20 2020 2020  >.        .     
+00000260: 2020 203c 7020 616c 6967 6e3d 2263 656e     <p align="cen
+00000270: 7465 7222 3e3c 6120 6872 6566 3d22 6874  ter"><a href="ht
+00000280: 7470 733a 2f2f 7065 7079 2e74 6563 682f  tps://pepy.tech/
+00000290: 7072 6f6a 6563 742f 6162 6722 3e20 3c69  project/abg"> <i
+000002a0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000002b0: 7374 6174 6963 2e70 6570 792e 7465 6368  static.pepy.tech
+000002c0: 2f70 6572 736f 6e61 6c69 7a65 642d 6261  /personalized-ba
+000002d0: 6467 652f 6162 673f 7065 7269 6f64 3d74  dge/abg?period=t
+000002e0: 6f74 616c 2675 6e69 7473 3d69 6e74 6572  otal&units=inter
+000002f0: 6e61 7469 6f6e 616c 5f73 7973 7465 6d26  national_system&
+00000300: 6c65 6674 5f63 6f6c 6f72 3d62 6c61 636b  left_color=black
+00000310: 2672 6967 6874 5f63 6f6c 6f72 3d62 6c61  &right_color=bla
+00000320: 636b 266c 6566 745f 7465 7874 3d44 6f77  ck&left_text=Dow
+00000330: 6e6c 6f61 6473 2220 7769 6474 683d 2231  nloads" width="1
+00000340: 3639 2220 6865 6967 6874 3d22 3239 2e36  69" height="29.6
+00000350: 3922 2f3e 3c2f 613e 3c2f 703e 0a20 2020  9"/></a></p>.   
+00000360: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
+00000370: 2320 5265 7175 6972 656d 656e 7473 200a  # Requirements .
+00000380: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000390: 202d 2050 7974 686f 6e20 332e 3720 e1b4   - Python 3.7 ..
+000003a0: 8fca 8020 6869 6768 6572 2e0a 2020 2020  ... higher..    
+000003b0: 2020 2020 2d20 4120 5be1 b49b e1b4 87ca      - A [.......
+000003c0: 9fe1 b487 c9a2 ca80 e1b4 80e1 b48d 20e1  .............. .
+000003d0: b480 e1b4 98c9 aa20 e1b4 8be1 b487 ca8f  ....... ........
+000003e0: 5d28 6874 7470 733a 2f2f 646f 6373 2e70  ](https://docs.p
+000003f0: 7972 6f67 7261 6d2e 6f72 672f 696e 7472  yrogram.org/intr
+00000400: 6f2f 7365 7475 7023 6170 692d 6b65 7973  o/setup#api-keys
+00000410: 292e 0a20 2020 2020 2020 202d 20e1 b480  )..        - ...
+00000420: ca99 c9a2 205b e1b4 84e1 b48f c9b4 d293  .... [..........
+00000430: c9aa c9a2 5d28 6874 7470 733a 2f2f 6769  ....](https://gi
+00000440: 7468 7562 2e63 6f6d 2f41 6269 7368 6e6f  thub.com/Abishno
+00000450: 6936 392f 4162 6723 636f 6e66 6967 7572  i69/Abg#configur
+00000460: 6174 6f69 6e73 292e 0a20 2020 2020 2020  atoins)..       
+00000470: 200a 2020 2020 2020 2020 2323 2320 496e   .        ### In
+00000480: 7374 616c 6c69 6e67 203a 0a20 2020 2020  stalling :.     
+00000490: 2020 200a 2020 2020 2020 2020 6060 6062     .        ```b
+000004a0: 6173 680a 2020 2020 2020 2020 7069 7020  ash.        pip 
+000004b0: 696e 7374 616c 6c20 2d55 2041 6267 0a20  install -U Abg. 
+000004c0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+000004d0: 2020 2023 2323 2320 73e1 b487 e1b4 9be1     #### s.......
+000004e0: b49c e1b4 980a 2020 2020 2020 2020 6060  ......        ``
+000004f0: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
+00000500: 6672 6f6d 2070 7972 6f67 7261 6d20 696d  from pyrogram im
+00000510: 706f 7274 2066 696c 7465 7273 2c20 436c  port filters, Cl
+00000520: 6965 6e74 0a20 2020 2020 2020 2066 726f  ient.        fro
+00000530: 6d20 7079 726f 6772 616d 2e74 7970 6573  m pyrogram.types
+00000540: 2069 6d70 6f72 7420 4361 6c6c 6261 636b   import Callback
+00000550: 5175 6572 792c 204d 6573 7361 6765 0a20  Query, Message. 
+00000560: 2020 2020 2020 2066 726f 6d20 4162 6720         from Abg 
+00000570: 696d 706f 7274 2070 6174 6368 2020 2320  import patch  # 
+00000580: 7479 7065 203a 2069 676e 6f72 650a 2020  type : ignore.  
+00000590: 2020 2020 2020 6672 6f6d 2041 6267 2e68        from Abg.h
+000005a0: 656c 7065 7273 2069 6d70 6f72 7420 696b  elpers import ik
+000005b0: 620a 2020 2020 2020 2020 0a20 2020 2020  b.        .     
+000005c0: 2020 2061 7070 203d 2043 6c69 656e 7428     app = Client(
+000005d0: 226d 795f 6163 636f 756e 7422 290a 2020  "my_account").  
+000005e0: 2020 2020 2020 0a20 2020 2020 2020 2040        .        @
+000005f0: 6170 702e 6f6e 5f63 6d64 2822 6d79 696e  app.on_cmd("myin
+00000600: 666f 2229 0a20 2020 2020 2020 2052 6573  fo").        Res
+00000610: 756c 7464 6566 206d 795f 696e 666f 2873  ultdef my_info(s
+00000620: 656c 663a 2043 6c69 656e 742c 2063 7478  elf: Client, ctx
+00000630: 3a20 4d65 7373 6167 6529 3a0a 2020 2020  : Message):.    
+00000640: 2020 2020 2020 2020 6966 206e 6f74 2063          if not c
+00000650: 7478 2e66 726f 6d5f 7573 6572 3a0a 2020  tx.from_user:.  
+00000660: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00000670: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
+00000680: 206e 616d 6520 3d20 6177 6169 7420 6374   name = await ct
+00000690: 782e 6368 6174 2e61 736b 2822 5479 7065  x.chat.ask("Type
+000006a0: 2059 6f75 7220 4e61 6d65 2229 0a20 2020   Your Name").   
+000006b0: 2020 2020 2020 2020 2061 6765 203d 2061           age = a
+000006c0: 7761 6974 2063 7478 2e63 6861 742e 6173  wait ctx.chat.as
+000006d0: 6b28 2254 7970 6520 796f 7572 2061 6765  k("Type your age
+000006e0: 2229 0a20 2020 2020 2020 2020 2020 2061  ").            a
+000006f0: 6464 203d 2061 7761 6974 2063 7478 2e63  dd = await ctx.c
+00000700: 6861 742e 6173 6b28 2254 7970 6520 796f  hat.ask("Type yo
+00000710: 7572 2061 6464 7265 7373 2229 0a20 2020  ur address").   
+00000720: 2020 2020 2020 2020 2023 2079 6f75 2063           # you c
+00000730: 616e 2061 6c73 6f20 7573 6520 3a20 6374  an also use : ct
+00000740: 782e 7265 706c 795f 7465 7874 282e 2e2e  x.reply_text(...
+00000750: 290a 2020 2020 2020 2020 2020 2020 6177  ).            aw
+00000760: 6169 7420 7365 6c66 2e73 656e 645f 6d73  ait self.send_ms
+00000770: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
+00000780: 2020 2063 6861 745f 6964 3d63 7478 2e63     chat_id=ctx.c
+00000790: 6861 742e 6964 2c0a 2020 2020 2020 2020  hat.id,.        
+000007a0: 2020 2020 2020 2020 7465 7874 3d66 2259          text=f"Y
+000007b0: 6f75 7220 6e61 6d65 2069 733a 207b 6e61  our name is: {na
+000007c0: 6d65 2e74 6578 747d 5c6e 596f 7572 2061  me.text}\nYour a
+000007d0: 6765 2069 733a 207b 6167 652e 7465 7874  ge is: {age.text
+000007e0: 7d5c 6e79 6f75 7220 6164 6472 6573 7320  }\nyour address 
+000007f0: 6973 3a20 7b61 6464 2e74 6578 747d 222c  is: {add.text}",
+00000800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000810: 2072 6570 6c79 5f6d 6172 6b75 703d 696b   reply_markup=ik
+00000820: 6228 5b5b 2822 ca99 e1b4 9ce1 b49b e1b4  b([[("..........
+00000830: 9be1 b48f c9b4 222c 2022 6865 6c6c 6f22  ......", "hello"
+00000840: 295d 5d29 2c0a 2020 2020 2020 2020 2020  )]]),.          
+00000850: 2020 290a 2020 2020 2020 2020 0a20 2020    ).        .   
+00000860: 2020 2020 2023 2063 616c 6c62 6163 6b20       # callback 
+00000870: 0a20 2020 2020 2020 2040 6170 702e 6f6e  .        @app.on
+00000880: 5f63 6228 2268 656c 6c6f 2229 0a20 2020  _cb("hello").   
+00000890: 2020 2020 2061 7379 6e63 2064 6566 2068       async def h
+000008a0: 656c 6c6f 2863 3a20 436c 6965 6e74 2c20  ello(c: Client, 
+000008b0: 713a 2043 616c 6c62 6163 6b51 7565 7279  q: CallbackQuery
+000008c0: 293a 0a20 2020 2020 2020 2020 2020 2061  ):.            a
+000008d0: 7761 6974 2071 2e61 6e73 7765 7228 2248  wait q.answer("H
+000008e0: 656c 6c6f 2046 726f 6d20 4162 6722 2c20  ello From Abg", 
+000008f0: 7368 6f77 5f61 6c65 7274 3d54 7275 6529  show_alert=True)
+00000900: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000910: 2020 2020 6170 702e 7275 6e28 290a 2020      app.run().  
+00000920: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+00000930: 2020 3e0a 2020 2020 2020 2020 2323 2323    >.        ####
+00000940: 20e1 b49c 73e1 b487 ca80 2fca 99e1 b48f   ...s...../.....
+00000950: e1b4 9b20 ca80 c9aa c9a2 ca9c e1b4 9b73  ... ...........s
+00000960: 200a 2020 2020 2020 2020 0a20 2020 2020   .        .     
+00000970: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
+00000980: 2020 2020 2066 726f 6d20 4162 6720 696d       from Abg im
+00000990: 706f 7274 2070 6174 6368 2020 2320 616c  port patch  # al
+000009a0: 6c20 7061 7463 680a 2020 2020 2020 2020  l patch.        
+000009b0: 6672 6f6d 2070 7972 6f67 7261 6d2e 7479  from pyrogram.ty
+000009c0: 7065 7320 696d 706f 7274 204d 6573 7361  pes import Messa
+000009d0: 6765 0a20 2020 2020 2020 2066 726f 6d20  ge.        from 
+000009e0: 7079 726f 6772 616d 2069 6d70 6f72 7420  pyrogram import 
+000009f0: 436c 6965 6e74 0a20 2020 2020 2020 200a  Client.        .
+00000a00: 2020 2020 2020 2020 6170 7020 3d20 436c          app = Cl
+00000a10: 6965 6e74 2822 6d79 5f61 6363 6f75 6e74  ient("my_account
+00000a20: 2229 0a20 2020 2020 2020 200a 2020 2020  ").        .    
+00000a30: 2020 2020 4061 7070 2e6f 6e5f 636d 6428      @app.on_cmd(
+00000a40: 2264 656c 222c 2067 726f 7570 5f6f 6e6c  "del", group_onl
+00000a50: 793d 5472 7565 290a 2020 2020 2020 2020  y=True).        
+00000a60: 4061 7070 2e61 646d 696e 734f 6e6c 7928  @app.adminsOnly(
+00000a70: 7065 726d 6973 7369 6f6e 733d 2263 616e  permissions="can
+00000a80: 5f64 656c 6574 655f 6d65 7373 6167 6573  _delete_messages
+00000a90: 222c 2069 735f 626f 7468 3d54 7275 6529  ", is_both=True)
+00000aa0: 0a20 2020 2020 2020 2061 7379 6e63 2064  .        async d
+00000ab0: 6566 2064 656c 5f6d 7367 2863 3a20 436c  ef del_msg(c: Cl
+00000ac0: 6965 6e74 2c20 6d3a 204d 6573 7361 6765  ient, m: Message
+00000ad0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+00000ae0: 6620 6d2e 7265 706c 795f 746f 5f6d 6573  f m.reply_to_mes
+00000af0: 7361 6765 3a0a 2020 2020 2020 2020 2020  sage:.          
+00000b00: 2020 2020 2020 6177 6169 7420 6d2e 6465        await m.de
+00000b10: 6c65 7465 2829 0a20 2020 2020 2020 2020  lete().         
+00000b20: 2020 2020 2020 2061 7761 6974 2063 2e64         await c.d
+00000b30: 656c 6574 655f 6d65 7373 6167 6573 280a  elete_messages(.
+00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b50: 2020 2020 6368 6174 5f69 643d 6d2e 6368      chat_id=m.ch
+00000b60: 6174 2e69 642c 0a20 2020 2020 2020 2020  at.id,.         
+00000b70: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00000b80: 6765 5f69 6473 3d6d 2e72 6570 6c79 5f74  ge_ids=m.reply_t
+00000b90: 6f5f 6d65 7373 6167 652e 6964 2c0a 2020  o_message.id,.  
+00000ba0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00000bb0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00000bc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000bd0: 2020 6177 6169 7420 6d2e 7265 706c 795f    await m.reply_
+00000be0: 7465 7874 2874 6578 743d 22e1 b4a1 ca9c  text(text=".....
+00000bf0: e1b4 80e1 b49b 20e1 b485 e1b4 8f20 ca8f  ...... ...... ..
+00000c00: e1b4 8fe1 b49c 20e1 b4a1 e1b4 80c9 b4c9  ...... .........
+00000c10: b4e1 b480 20e1 b485 e1b4 87ca 9fe1 b487  .... ...........
+00000c20: e1b4 9be1 b487 3f22 290a 2020 2020 2020  ......?").      
+00000c30: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+00000c40: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000c50: 2020 6170 702e 7275 6e28 290a 2020 2020    app.run().    
+00000c60: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
+00000c70: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000c80: 2020 3e0a 2020 2020 2020 2020 2323 2320    >.        ### 
+00000c90: 6b65 7962 6f61 7264 2773 0a20 2020 2020  keyboard's.     
+00000ca0: 2020 200a 2020 2020 2020 2020 6060 6070     .        ```p
+00000cb0: 7974 686f 6e0a 2020 2020 2020 2020 6672  ython.        fr
+00000cc0: 6f6d 2041 6267 2e69 6e6c 696e 6520 696d  om Abg.inline im
+00000cd0: 706f 7274 2049 6e6c 696e 654b 6579 626f  port InlineKeybo
+00000ce0: 6172 642c 2049 6e6c 696e 6542 7574 746f  ard, InlineButto
+00000cf0: 6e0a 2020 2020 2020 2020 0a20 2020 2020  n.        .     
+00000d00: 2020 200a 2020 2020 2020 2020 6b65 7962     .        keyb
+00000d10: 6f61 7264 203d 2049 6e6c 696e 654b 6579  oard = InlineKey
+00000d20: 626f 6172 6428 726f 775f 7769 6474 683d  board(row_width=
+00000d30: 3329 0a20 2020 2020 2020 206b 6579 626f  3).        keybo
+00000d40: 6172 642e 6164 6428 0a20 2020 2020 2020  ard.add(.       
+00000d50: 2020 2020 2049 6e6c 696e 6542 7574 746f       InlineButto
+00000d60: 6e28 2731 272c 2027 696e 6c69 6e65 5f6b  n('1', 'inline_k
+00000d70: 6579 626f 6172 643a 3127 292c 0a20 2020  eyboard:1'),.   
+00000d80: 2020 2020 2020 2020 2049 6e6c 696e 6542           InlineB
+00000d90: 7574 746f 6e28 2732 272c 2027 696e 6c69  utton('2', 'inli
+00000da0: 6e65 5f6b 6579 626f 6172 643a 3227 292c  ne_keyboard:2'),
+00000db0: 0a20 2020 2020 2020 2020 2020 2049 6e6c  .            Inl
+00000dc0: 696e 6542 7574 746f 6e28 2733 272c 2027  ineButton('3', '
+00000dd0: 696e 6c69 6e65 5f6b 6579 626f 6172 643a  inline_keyboard:
+00000de0: 3327 292c 0a20 2020 2020 2020 2020 2020  3'),.           
+00000df0: 2049 6e6c 696e 6542 7574 746f 6e28 2734   InlineButton('4
+00000e00: 272c 2027 696e 6c69 6e65 5f6b 6579 626f  ', 'inline_keybo
+00000e10: 6172 643a 3427 292c 0a20 2020 2020 2020  ard:4'),.       
+00000e20: 2020 2020 2049 6e6c 696e 6542 7574 746f       InlineButto
+00000e30: 6e28 2735 272c 2027 696e 6c69 6e65 5f6b  n('5', 'inline_k
+00000e40: 6579 626f 6172 643a 3527 292c 0a20 2020  eyboard:5'),.   
+00000e50: 2020 2020 2020 2020 2049 6e6c 696e 6542           InlineB
+00000e60: 7574 746f 6e28 2736 272c 2027 696e 6c69  utton('6', 'inli
+00000e70: 6e65 5f6b 6579 626f 6172 643a 3627 292c  ne_keyboard:6'),
+00000e80: 0a20 2020 2020 2020 2020 2020 2049 6e6c  .            Inl
+00000e90: 696e 6542 7574 746f 6e28 2737 272c 2027  ineButton('7', '
+00000ea0: 696e 6c69 6e65 5f6b 6579 626f 6172 643a  inline_keyboard:
+00000eb0: 3727 290a 2020 2020 2020 2020 290a 2020  7').        ).  
+00000ec0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+00000ed0: 2020 0a20 2020 2020 2020 2023 2323 2320    .        #### 
+00000ee0: ca80 e1b4 8773 e1b4 9cca 9fe1 b49b 0a20  .....s......... 
+00000ef0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000f00: 3c70 3e3c 696d 6720 7372 633d 2268 7474  <p><img src="htt
+00000f10: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00000f20: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f41  sercontent.com/A
+00000f30: 6269 7368 6e6f 6936 392f 4162 672f 6d61  bishnoi69/Abg/ma
+00000f40: 7374 6572 2f64 6f63 652f 696d 6167 6573  ster/doce/images
+00000f50: 2f61 6464 5f69 6e6c 696e 655f 6275 7474  /add_inline_butt
+00000f60: 6f6e 2e70 6e67 2220 616c 743d 2261 6464  on.png" alt="add
+00000f70: 5f69 6e6c 696e 655f 6275 7474 6f6e 223e  _inline_button">
+00000f80: 3c2f 703e 0a20 2020 2020 2020 200a 2020  </p>.        .  
+00000f90: 2020 2020 2020 e294 81e2 9481 e294 81e2        ..........
+00000fa0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00000fb0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00000fc0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00000fd0: 9481 0a20 2020 2020 2020 2023 2323 2043  ...        ### C
+00000fe0: 6f6e 6669 6775 7261 746f 696e 730a 2020  onfiguratoins.  
+00000ff0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+00001000: 2020 4f57 4e45 525f 4944 203d 20ca 8fe1    OWNER_ID = ...
+00001010: b48f e1b4 9cca 8020 e1b4 9be1 b487 ca9f  ....... ........
+00001020: e1b4 87c9 a2ca 80e1 b480 e1b4 8d20 c9aa  ............. ..
+00001030: e1b4 852e 0a20 2020 2020 2020 2044 4556  .....        DEV
+00001040: 5f55 5345 5253 203d 20ca 99e1 b48f e1b4  _USERS = .......
+00001050: 9b20 e1b4 85e1 b487 e1b4 a073 20c9 aae1  . .........s ...
+00001060: b485 2e20 28ca 8fe1 b48f e1b4 9c20 e1b4  ... (........ ..
+00001070: 84e1 b480 c9b4 20e1 b480 e1b4 85e1 b485  ...... .........
+00001080: 20e1 b480 20ca 9fc9 aa73 e1b4 9b20 3a20   ... ....s... : 
+00001090: 3120 3220 3329 0a20 2020 2020 2020 204c  1 2 3).        L
+000010a0: 4f47 4745 525f 4944 203d 20ca 8fe1 b48f  OGGER_ID = .....
+000010b0: e1b4 9cca 8020 e1b4 98ca 80c9 aae1 b4a0  ..... ..........
+000010c0: e1b4 80e1 b49b e1b4 8720 c9a2 ca80 e1b4  ......... ......
+000010d0: 8fe1 b49c e1b4 982f e1b4 84ca 9ce1 b480  ......./........
+000010e0: c9b4 c9b4 e1b4 87ca 9f20 c9aa e1b4 852e  ......... ......
+000010f0: 2028 ca9c e1b4 87ca 80e1 b487 20ca 99e1   (.......... ...
+00001100: b48f e1b4 9b20 73e1 b487 c9b4 e1b4 8520  ..... s........ 
+00001110: ca9f e1b4 8fc9 a273 290a 2020 2020 2020  .......s).      
+00001120: 2020 6060 600a 2020 2020 2020 2020 e294    ```.        ..
+00001130: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00001140: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00001150: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00001160: 81e2 9481 e294 81e2 9481 200a 2020 2020  .......... .    
+00001170: 2020 2020 0a20 2020 2020 2020 200a 4b65      .        .Ke
+00001180: 7977 6f72 6473 3a20 6164 642d 6f6e 2070  ywords: add-on p
+00001190: 7972 6f67 7261 6d20 626f 7473 2074 656c  yrogram bots tel
+000011a0: 6567 7261 6d20 626f 7420 6368 6174 206d  egram bot chat m
+000011b0: 6573 7365 6e67 6572 206d 7470 726f 746f  essenger mtproto
+000011c0: 2061 7069 2063 6c69 656e 7420 6c69 6272   api client libr
+000011d0: 6172 7920 7079 7468 6f6e 2063 6f6e 7665  ary python conve
+000011e0: 7273 6174 696f 6e20 6b65 7962 6f61 7264  rsation keyboard
+000011f0: 2075 7365 7262 6f74 2070 6174 6368 2068   userbot patch h
+00001200: 7474 7073 0a50 6c61 7466 6f72 6d3a 2055  ttps.Platform: U
+00001210: 4e4b 4e4f 574e 0a43 6c61 7373 6966 6965  NKNOWN.Classifie
+00001220: 723a 2044 6576 656c 6f70 6d65 6e74 2053  r: Development S
+00001230: 7461 7475 7320 3a3a 2035 202d 2050 726f  tatus :: 5 - Pro
+00001240: 6475 6374 696f 6e2f 5374 6162 6c65 0a43  duction/Stable.C
+00001250: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
+00001260: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+00001270: 4465 7665 6c6f 7065 7273 0a43 6c61 7373  Developers.Class
+00001280: 6966 6965 723a 204e 6174 7572 616c 204c  ifier: Natural L
+00001290: 616e 6775 6167 6520 3a3a 2045 6e67 6c69  anguage :: Engli
+000012a0: 7368 0a43 6c61 7373 6966 6965 723a 204f  sh.Classifier: O
+000012b0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+000012c0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+000012d0: 740a 436c 6173 7369 6669 6572 3a20 5072  t.Classifier: Pr
+000012e0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000012f0: 6765 203a 3a20 5079 7468 6f6e 0a43 6c61  ge :: Python.Cla
+00001300: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00001310: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00001320: 2050 7974 686f 6e20 3a3a 2033 0a43 6c61   Python :: 3.Cla
+00001330: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00001340: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00001350: 2050 7974 686f 6e20 3a3a 2033 2e37 0a43   Python :: 3.7.C
+00001360: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00001370: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00001380: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
+00001390: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000013a0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000013b0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000013c0: 2e39 0a43 6c61 7373 6966 6965 723a 2050  .9.Classifier: P
+000013d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000013e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000013f0: 2033 2e31 300a 436c 6173 7369 6669 6572   3.10.Classifier
+00001400: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00001410: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00001420: 203a 3a20 332e 3131 0a43 6c61 7373 6966   :: 3.11.Classif
+00001430: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00001440: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00001450: 686f 6e20 3a3a 2049 6d70 6c65 6d65 6e74  hon :: Implement
+00001460: 6174 696f 6e0a 436c 6173 7369 6669 6572  ation.Classifier
+00001470: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00001480: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00001490: 203a 3a20 496d 706c 656d 656e 7461 7469   :: Implementati
+000014a0: 6f6e 203a 3a20 4350 7974 686f 6e0a 436c  on :: CPython.Cl
+000014b0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000014c0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000014d0: 3a20 5079 7468 6f6e 203a 3a20 496d 706c  : Python :: Impl
+000014e0: 656d 656e 7461 7469 6f6e 203a 3a20 5079  ementation :: Py
+000014f0: 5079 0a43 6c61 7373 6966 6965 723a 2054  Py.Classifier: T
+00001500: 6f70 6963 203a 3a20 496e 7465 726e 6574  opic :: Internet
+00001510: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+00001520: 6963 203a 3a20 436f 6d6d 756e 6963 6174  ic :: Communicat
+00001530: 696f 6e73 0a43 6c61 7373 6966 6965 723a  ions.Classifier:
+00001540: 2054 6f70 6963 203a 3a20 436f 6d6d 756e   Topic :: Commun
+00001550: 6963 6174 696f 6e73 203a 3a20 4368 6174  ications :: Chat
+00001560: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+00001570: 6963 203a 3a20 536f 6674 7761 7265 2044  ic :: Software D
+00001580: 6576 656c 6f70 6d65 6e74 203a 3a20 4c69  evelopment :: Li
+00001590: 6272 6172 6965 730a 436c 6173 7369 6669  braries.Classifi
+000015a0: 6572 3a20 546f 7069 6320 3a3a 2053 6f66  er: Topic :: Sof
+000015b0: 7477 6172 6520 4465 7665 6c6f 706d 656e  tware Developmen
+000015c0: 7420 3a3a 204c 6962 7261 7269 6573 203a  t :: Libraries :
+000015d0: 3a20 5079 7468 6f6e 204d 6f64 756c 6573  : Python Modules
+000015e0: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+000015f0: 6963 203a 3a20 536f 6674 7761 7265 2044  ic :: Software D
+00001600: 6576 656c 6f70 6d65 6e74 203a 3a20 4c69  evelopment :: Li
+00001610: 6272 6172 6965 7320 3a3a 2041 7070 6c69  braries :: Appli
+00001620: 6361 7469 6f6e 2046 7261 6d65 776f 726b  cation Framework
+00001630: 730a 5265 7175 6972 6573 2d50 7974 686f  s.Requires-Pytho
+00001640: 6e3a 207e 3d33 2e37 0a44 6573 6372 6970  n: ~=3.7.Descrip
+00001650: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
+00001660: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
+00001670: 0a                                       .
```

### Comparing `Abg-2.3.3/Abg.egg-info/SOURCES.txt` & `Abg-2.3.4/Abg.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 README.md
 setup.py
 Abg/__init__.py
+Abg/config.py
 Abg.egg-info/PKG-INFO
 Abg.egg-info/SOURCES.txt
 Abg.egg-info/dependency_links.txt
+Abg.egg-info/not-zip-safe
 Abg.egg-info/top_level.txt
 Abg/helpers/__init__.py
 Abg/helpers/get_user.py
 Abg/helpers/helpers.py
 Abg/helpers/http_helper.py
 Abg/helpers/human_read.py
 Abg/helpers/msg_types.py
```

### Comparing `Abg-2.3.3/PKG-INFO` & `Abg-2.3.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,276 +1,360 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 4162 670a  : 2.1.Name: Abg.
-00000020: 5665 7273 696f 6e3a 2032 2e33 2e33 0a53  Version: 2.3.3.S
-00000030: 756d 6d61 7279 3a20 5465 6c65 6772 616d  ummary: Telegram
-00000040: 2062 6f74 2068 656c 7065 7273 0a48 6f6d   bot helpers.Hom
-00000050: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
-00000060: 6769 7468 7562 2e63 6f6d 2f41 6269 7368  github.com/Abish
-00000070: 6e6f 6936 392f 4162 670a 4175 7468 6f72  noi69/Abg.Author
-00000080: 3a20 4162 6973 686e 6f69 0a41 7574 686f  : Abishnoi.Autho
-00000090: 722d 656d 6169 6c3a 2041 6269 7368 6e6f  r-email: Abishno
-000000a0: 6936 3940 4162 672e 6f72 670a 4c69 6365  i69@Abg.org.Lice
-000000b0: 6e73 653a 204d 4954 0a44 6f77 6e6c 6f61  nse: MIT.Downloa
-000000c0: 642d 5552 4c3a 2068 7474 7073 3a2f 2f67  d-URL: https://g
-000000d0: 6974 6875 622e 636f 6d2f 4162 6973 686e  ithub.com/Abishn
-000000e0: 6f69 3639 2f41 6267 2f72 656c 6561 7365  oi69/Abg/release
-000000f0: 732f 6c61 7465 7374 0a50 726f 6a65 6374  s/latest.Project
-00000100: 2d55 524c 3a20 5472 6163 6b65 722c 2068  -URL: Tracker, h
-00000110: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000120: 6d2f 4162 6973 686e 6f69 3639 2f41 6267  m/Abishnoi69/Abg
-00000130: 2f69 7373 7565 730a 5072 6f6a 6563 742d  /issues.Project-
-00000140: 5552 4c3a 2043 6f6d 6d75 6e69 7479 2c20  URL: Community, 
-00000150: 6874 7470 733a 2f2f 742e 6d65 2f41 6267  https://t.me/Abg
-00000160: 7079 0a50 726f 6a65 6374 2d55 524c 3a20  py.Project-URL: 
-00000170: 536f 7572 6365 2c20 6874 7470 733a 2f2f  Source, https://
-00000180: 6769 7468 7562 2e63 6f6d 2f41 6269 7368  github.com/Abish
-00000190: 6e6f 6936 392f 4162 670a 5072 6f6a 6563  noi69/Abg.Projec
-000001a0: 742d 5552 4c3a 2044 6f63 756d 656e 7461  t-URL: Documenta
-000001b0: 7469 6f6e 2c20 6874 7470 733a 2f2f 6769  tion, https://gi
-000001c0: 7468 7562 2e63 6f6d 2f41 6269 7368 6e6f  thub.com/Abishno
-000001d0: 6936 392f 4162 672f 7472 6565 2f6d 6173  i69/Abg/tree/mas
-000001e0: 7465 722f 646f 6365 0a4b 6579 776f 7264  ter/doce.Keyword
-000001f0: 733a 2074 656c 6567 7261 6d20 626f 7420  s: telegram bot 
-00000200: 6368 6174 206d 6573 7365 6e67 6572 206d  chat messenger m
-00000210: 7470 726f 746f 2061 7069 2063 6c69 656e  tproto api clien
-00000220: 7420 6c69 6272 6172 7920 7079 7468 6f6e  t library python
-00000230: 2063 6f6e 7665 7273 6174 696f 6e20 6b65   conversation ke
-00000240: 7962 6f61 7264 2075 7365 7262 6f74 2070  yboard userbot p
-00000250: 6174 6368 2062 6f74 6170 6920 6874 7470  atch botapi http
-00000260: 730a 506c 6174 666f 726d 3a20 554e 4b4e  s.Platform: UNKN
-00000270: 4f57 4e0a 436c 6173 7369 6669 6572 3a20  OWN.Classifier: 
-00000280: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
-00000290: 7573 203a 3a20 3520 2d20 5072 6f64 7563  us :: 5 - Produc
-000002a0: 7469 6f6e 2f53 7461 626c 650a 436c 6173  tion/Stable.Clas
-000002b0: 7369 6669 6572 3a20 496e 7465 6e64 6564  sifier: Intended
-000002c0: 2041 7564 6965 6e63 6520 3a3a 2044 6576   Audience :: Dev
-000002d0: 656c 6f70 6572 730a 436c 6173 7369 6669  elopers.Classifi
-000002e0: 6572 3a20 4e61 7475 7261 6c20 4c61 6e67  er: Natural Lang
-000002f0: 7561 6765 203a 3a20 456e 676c 6973 680a  uage :: English.
-00000300: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
-00000310: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000320: 4f53 2049 6e64 6570 656e 6465 6e74 0a43  OS Independent.C
-00000330: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000340: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000350: 3a3a 2050 7974 686f 6e0a 436c 6173 7369  :: Python.Classi
-00000360: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000370: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000380: 7468 6f6e 203a 3a20 330a 436c 6173 7369  thon :: 3.Classi
-00000390: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000003a0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000003b0: 7468 6f6e 203a 3a20 332e 370a 436c 6173  thon :: 3.7.Clas
-000003c0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-000003d0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000003e0: 5079 7468 6f6e 203a 3a20 332e 380a 436c  Python :: 3.8.Cl
-000003f0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000400: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000410: 3a20 5079 7468 6f6e 203a 3a20 332e 390a  : Python :: 3.9.
-00000420: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000430: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000440: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000450: 3130 0a43 6c61 7373 6966 6965 723a 2050  10.Classifier: P
-00000460: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000470: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000480: 2033 2e31 310a 436c 6173 7369 6669 6572   3.11.Classifier
-00000490: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-000004a0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000004b0: 203a 3a20 496d 706c 656d 656e 7461 7469   :: Implementati
-000004c0: 6f6e 0a43 6c61 7373 6966 6965 723a 2050  on.Classifier: P
-000004d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000004e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000004f0: 2049 6d70 6c65 6d65 6e74 6174 696f 6e20   Implementation 
-00000500: 3a3a 2043 5079 7468 6f6e 0a43 6c61 7373  :: CPython.Class
-00000510: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000520: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000530: 7974 686f 6e20 3a3a 2049 6d70 6c65 6d65  ython :: Impleme
-00000540: 6e74 6174 696f 6e20 3a3a 2050 7950 790a  ntation :: PyPy.
-00000550: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
-00000560: 6320 3a3a 2049 6e74 6572 6e65 740a 436c  c :: Internet.Cl
-00000570: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-00000580: 3a3a 2043 6f6d 6d75 6e69 6361 7469 6f6e  :: Communication
-00000590: 730a 436c 6173 7369 6669 6572 3a20 546f  s.Classifier: To
-000005a0: 7069 6320 3a3a 2043 6f6d 6d75 6e69 6361  pic :: Communica
-000005b0: 7469 6f6e 7320 3a3a 2043 6861 740a 436c  tions :: Chat.Cl
-000005c0: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-000005d0: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
-000005e0: 6c6f 706d 656e 7420 3a3a 204c 6962 7261  lopment :: Libra
-000005f0: 7269 6573 0a43 6c61 7373 6966 6965 723a  ries.Classifier:
-00000600: 2054 6f70 6963 203a 3a20 536f 6674 7761   Topic :: Softwa
-00000610: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
-00000620: 3a20 4c69 6272 6172 6965 7320 3a3a 2050  : Libraries :: P
-00000630: 7974 686f 6e20 4d6f 6475 6c65 730a 436c  ython Modules.Cl
-00000640: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-00000650: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
-00000660: 6c6f 706d 656e 7420 3a3a 204c 6962 7261  lopment :: Libra
-00000670: 7269 6573 203a 3a20 4170 706c 6963 6174  ries :: Applicat
-00000680: 696f 6e20 4672 616d 6577 6f72 6b73 0a52  ion Frameworks.R
-00000690: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
-000006a0: 7e3d 332e 370a 4465 7363 7269 7074 696f  ~=3.7.Descriptio
-000006b0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-000006c0: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a23  text/markdown..#
-000006d0: 20e1 b480 ca99 c9a2 203a 2d3e 205b 215b   ....... :-> [![
-000006e0: 446f 776e 6c6f 6164 735d 2868 7474 7073  Downloads](https
-000006f0: 3a2f 2f73 7461 7469 632e 7065 7079 2e74  ://static.pepy.t
-00000700: 6563 682f 7065 7273 6f6e 616c 697a 6564  ech/personalized
-00000710: 2d62 6164 6765 2f61 6267 3f70 6572 696f  -badge/abg?perio
-00000720: 643d 746f 7461 6c26 756e 6974 733d 6162  d=total&units=ab
-00000730: 6272 6576 6961 7469 6f6e 266c 6566 745f  breviation&left_
-00000740: 636f 6c6f 723d 626c 6163 6b26 7269 6768  color=black&righ
-00000750: 745f 636f 6c6f 723d 626c 6163 6b26 6c65  t_color=black&le
-00000760: 6674 5f74 6578 743d 446f 776e 6c6f 6164  ft_text=Download
-00000770: 733a 295d 2868 7474 7073 3a2f 2f70 6570  s:)](https://pep
-00000780: 792e 7465 6368 2f70 726f 6a65 6374 2f61  y.tech/project/a
-00000790: 6267 290a 0a3e 200a 2323 2320 e280 a220  bg)..> .### ... 
-000007a0: 4162 670a 0a60 6060 7079 7468 6f6e 0a66  Abg..```python.f
-000007b0: 726f 6d20 7079 726f 6772 616d 2069 6d70  rom pyrogram imp
-000007c0: 6f72 7420 6669 6c74 6572 732c 2043 6c69  ort filters, Cli
-000007d0: 656e 740a 6672 6f6d 2070 7972 6f67 7261  ent.from pyrogra
-000007e0: 6d2e 7479 7065 7320 696d 706f 7274 2043  m.types import C
-000007f0: 616c 6c62 6163 6b51 7565 7279 2c20 4d65  allbackQuery, Me
-00000800: 7373 6167 650a 6672 6f6d 2041 6267 2069  ssage.from Abg i
-00000810: 6d70 6f72 7420 7061 7463 6820 2023 2074  mport patch  # t
-00000820: 7970 6520 3a20 6967 6e6f 7265 0a66 726f  ype : ignore.fro
-00000830: 6d20 4162 672e 6865 6c70 6572 7320 696d  m Abg.helpers im
-00000840: 706f 7274 2069 6b62 0a0a 6170 7020 3d20  port ikb..app = 
-00000850: 436c 6965 6e74 2822 6d79 5f61 6363 6f75  Client("my_accou
-00000860: 6e74 2229 0a0a 4061 7070 2e6f 6e5f 636d  nt")..@app.on_cm
-00000870: 6428 226d 7969 6e66 6f22 290a 6173 796e  d("myinfo").asyn
-00000880: 6320 6465 6620 6d79 5f69 6e66 6f28 7365  c def my_info(se
-00000890: 6c66 3a20 436c 6965 6e74 2c20 6374 783a  lf: Client, ctx:
-000008a0: 204d 6573 7361 6765 293a 0a20 2020 2069   Message):.    i
-000008b0: 6620 6e6f 7420 6374 782e 6672 6f6d 5f75  f not ctx.from_u
-000008c0: 7365 723a 0a20 2020 2020 2020 2072 6574  ser:.        ret
-000008d0: 7572 6e0a 2020 2020 6e61 6d65 203d 2061  urn.    name = a
-000008e0: 7761 6974 2063 7478 2e63 6861 742e 6173  wait ctx.chat.as
-000008f0: 6b28 2254 7970 6520 596f 7572 204e 616d  k("Type Your Nam
-00000900: 6522 290a 2020 2020 6167 6520 3d20 6177  e").    age = aw
-00000910: 6169 7420 6374 782e 6368 6174 2e61 736b  ait ctx.chat.ask
-00000920: 2822 5479 7065 2079 6f75 7220 6167 6522  ("Type your age"
-00000930: 290a 2020 2020 6164 6420 3d20 6177 6169  ).    add = awai
-00000940: 7420 6374 782e 6368 6174 2e61 736b 2822  t ctx.chat.ask("
-00000950: 5479 7065 2079 6f75 7220 6164 6472 6573  Type your addres
-00000960: 7322 290a 2020 2020 2320 796f 7520 6361  s").    # you ca
-00000970: 6e20 616c 736f 2075 7365 203a 2063 7478  n also use : ctx
-00000980: 2e72 6570 6c79 5f74 6578 7428 2e2e 2e29  .reply_text(...)
-00000990: 0a20 2020 2061 7761 6974 2073 656c 662e  .    await self.
-000009a0: 7365 6e64 5f6d 7367 280a 2020 2020 2020  send_msg(.      
-000009b0: 2020 6368 6174 5f69 643d 6374 782e 6368    chat_id=ctx.ch
-000009c0: 6174 2e69 642c 0a20 2020 2020 2020 2074  at.id,.        t
-000009d0: 6578 743d 6622 596f 7572 206e 616d 6520  ext=f"Your name 
-000009e0: 6973 3a20 7b6e 616d 652e 7465 7874 7d5c  is: {name.text}\
-000009f0: 6e59 6f75 7220 6167 6520 6973 3a20 7b61  nYour age is: {a
-00000a00: 6765 2e74 6578 747d 5c6e 796f 7572 2061  ge.text}\nyour a
-00000a10: 6464 7265 7373 2069 733a 207b 6164 642e  ddress is: {add.
-00000a20: 7465 7874 7d22 2c0a 2020 2020 2020 2020  text}",.        
-00000a30: 7265 706c 795f 6d61 726b 7570 3d69 6b62  reply_markup=ikb
-00000a40: 285b 5b28 22ca 99e1 b49c e1b4 9be1 b49b  ([[("...........
-00000a50: e1b4 8fc9 b422 2c20 2268 656c 6c6f 2229  .....", "hello")
-00000a60: 5d5d 292c 0a20 2020 2029 0a0a 2320 6361  ]]),.    )..# ca
-00000a70: 6c6c 6261 636b 200a 4061 7070 2e6f 6e5f  llback .@app.on_
-00000a80: 6362 2822 6865 6c6c 6f22 290a 6173 796e  cb("hello").asyn
-00000a90: 6320 6465 6620 6865 6c6c 6f28 633a 2043  c def hello(c: C
-00000aa0: 6c69 656e 742c 2071 3a20 4361 6c6c 6261  lient, q: Callba
-00000ab0: 636b 5175 6572 7929 3a0a 2020 2020 6177  ckQuery):.    aw
-00000ac0: 6169 7420 712e 616e 7377 6572 2822 4865  ait q.answer("He
-00000ad0: 6c6c 6f20 4672 6f6d 2041 6267 222c 2073  llo From Abg", s
-00000ae0: 686f 775f 616c 6572 743d 5472 7565 290a  how_alert=True).
-00000af0: 0a20 2061 7070 2e72 756e 2829 0a60 6060  .  app.run().```
-00000b00: 0a3e 0a23 2323 20e2 80a2 2055 7365 7220  .>.### ... User 
-00000b10: 5269 6768 7473 200a 0a60 6060 7079 7468  Rights ..```pyth
-00000b20: 6f6e 0a66 726f 6d20 4162 6720 696d 706f  on.from Abg impo
-00000b30: 7274 2070 6174 6368 2020 2320 616c 6c20  rt patch  # all 
-00000b40: 7061 7463 680a 6672 6f6d 2070 7972 6f67  patch.from pyrog
-00000b50: 7261 6d2e 7479 7065 7320 696d 706f 7274  ram.types import
-00000b60: 204d 6573 7361 6765 0a66 726f 6d20 7079   Message.from py
-00000b70: 726f 6772 616d 2069 6d70 6f72 7420 436c  rogram import Cl
-00000b80: 6965 6e74 0a0a 6170 7020 3d20 436c 6965  ient..app = Clie
-00000b90: 6e74 2822 6d79 5f61 6363 6f75 6e74 2229  nt("my_account")
-00000ba0: 0a0a 4061 7070 2e6f 6e5f 636d 6428 2264  ..@app.on_cmd("d
-00000bb0: 656c 222c 2067 726f 7570 5f6f 6e6c 793d  el", group_only=
-00000bc0: 5472 7565 290a 4061 7070 2e61 646d 696e  True).@app.admin
-00000bd0: 734f 6e6c 7928 7065 726d 6973 7369 6f6e  sOnly(permission
-00000be0: 733d 2263 616e 5f64 656c 6574 655f 6d65  s="can_delete_me
-00000bf0: 7373 6167 6573 222c 2069 735f 626f 7468  ssages", is_both
-00000c00: 3d54 7275 6529 0a61 7379 6e63 2064 6566  =True).async def
-00000c10: 2064 656c 5f6d 7367 2863 3a20 436c 6965   del_msg(c: Clie
-00000c20: 6e74 2c20 6d3a 204d 6573 7361 6765 293a  nt, m: Message):
-00000c30: 0a20 2020 2069 6620 6d2e 7265 706c 795f  .    if m.reply_
-00000c40: 746f 5f6d 6573 7361 6765 3a0a 2020 2020  to_message:.    
-00000c50: 2020 2020 6177 6169 7420 6d2e 6465 6c65      await m.dele
-00000c60: 7465 2829 0a20 2020 2020 2020 2061 7761  te().        awa
-00000c70: 6974 2063 2e64 656c 6574 655f 6d65 7373  it c.delete_mess
-00000c80: 6167 6573 280a 2020 2020 2020 2020 2020  ages(.          
-00000c90: 2020 6368 6174 5f69 643d 6d2e 6368 6174    chat_id=m.chat
-00000ca0: 2e69 642c 0a20 2020 2020 2020 2020 2020  .id,.           
-00000cb0: 206d 6573 7361 6765 5f69 6473 3d6d 2e72   message_ids=m.r
-00000cc0: 6570 6c79 5f74 6f5f 6d65 7373 6167 652e  eply_to_message.
-00000cd0: 6964 2c0a 2020 2020 2020 2020 290a 2020  id,.        ).  
-00000ce0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00000cf0: 6177 6169 7420 6d2e 7265 706c 795f 7465  await m.reply_te
-00000d00: 7874 2874 6578 743d 22e1 b4a1 ca9c e1b4  xt(text=".......
-00000d10: 80e1 b49b 20e1 b485 e1b4 8f20 ca8f e1b4  .... ...... ....
-00000d20: 8fe1 b49c 20e1 b4a1 e1b4 80c9 b4c9 b4e1  .... ...........
-00000d30: b480 20e1 b485 e1b4 87ca 9fe1 b487 e1b4  .. .............
-00000d40: 9be1 b487 3f22 290a 2020 2020 7265 7475  ....?").    retu
-00000d50: 726e 0a20 200a 2020 6170 702e 7275 6e28  rn.  .  app.run(
-00000d60: 290a 6060 600a 0a0a 3e0a 2323 2320 e280  ).```...>.### ..
-00000d70: a220 4b65 7962 6f61 7264 730a 0a60 6060  . Keyboards..```
-00000d80: 7079 7468 6f6e 0a66 726f 6d20 4162 672e  python.from Abg.
-00000d90: 696e 6c69 6e65 2069 6d70 6f72 7420 496e  inline import In
-00000da0: 6c69 6e65 4b65 7962 6f61 7264 2c20 496e  lineKeyboard, In
-00000db0: 6c69 6e65 4275 7474 6f6e 0a0a 0a6b 6579  lineButton...key
-00000dc0: 626f 6172 6420 3d20 496e 6c69 6e65 4b65  board = InlineKe
-00000dd0: 7962 6f61 7264 2872 6f77 5f77 6964 7468  yboard(row_width
-00000de0: 3d33 290a 6b65 7962 6f61 7264 2e61 6464  =3).keyboard.add
-00000df0: 280a 2020 2020 496e 6c69 6e65 4275 7474  (.    InlineButt
-00000e00: 6f6e 2827 3127 2c20 2769 6e6c 696e 655f  on('1', 'inline_
-00000e10: 6b65 7962 6f61 7264 3a31 2729 2c0a 2020  keyboard:1'),.  
-00000e20: 2020 496e 6c69 6e65 4275 7474 6f6e 2827    InlineButton('
-00000e30: 3227 2c20 2769 6e6c 696e 655f 6b65 7962  2', 'inline_keyb
-00000e40: 6f61 7264 3a32 2729 2c0a 2020 2020 496e  oard:2'),.    In
-00000e50: 6c69 6e65 4275 7474 6f6e 2827 3327 2c20  lineButton('3', 
-00000e60: 2769 6e6c 696e 655f 6b65 7962 6f61 7264  'inline_keyboard
-00000e70: 3a33 2729 2c0a 2020 2020 496e 6c69 6e65  :3'),.    Inline
-00000e80: 4275 7474 6f6e 2827 3427 2c20 2769 6e6c  Button('4', 'inl
-00000e90: 696e 655f 6b65 7962 6f61 7264 3a34 2729  ine_keyboard:4')
-00000ea0: 2c0a 2020 2020 496e 6c69 6e65 4275 7474  ,.    InlineButt
-00000eb0: 6f6e 2827 3527 2c20 2769 6e6c 696e 655f  on('5', 'inline_
-00000ec0: 6b65 7962 6f61 7264 3a35 2729 2c0a 2020  keyboard:5'),.  
-00000ed0: 2020 496e 6c69 6e65 4275 7474 6f6e 2827    InlineButton('
-00000ee0: 3627 2c20 2769 6e6c 696e 655f 6b65 7962  6', 'inline_keyb
-00000ef0: 6f61 7264 3a36 2729 2c0a 2020 2020 496e  oard:6'),.    In
-00000f00: 6c69 6e65 4275 7474 6f6e 2827 3727 2c20  lineButton('7', 
-00000f10: 2769 6e6c 696e 655f 6b65 7962 6f61 7264  'inline_keyboard
-00000f20: 3a37 2729 0a29 0a60 6060 0a0a 2323 2323  :7').).```..####
-00000f30: 2052 6573 756c 740a 0a3c 703e 3c69 6d67   Result..<p><img
-00000f40: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00000f50: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00000f60: 656e 742e 636f 6d2f 4162 6973 686e 6f69  ent.com/Abishnoi
-00000f70: 3639 2f41 6267 2f6d 6173 7465 722f 646f  69/Abg/master/do
-00000f80: 6365 2f69 6d61 6765 732f 6164 645f 696e  ce/images/add_in
-00000f90: 6c69 6e65 5f62 7574 746f 6e2e 706e 6722  line_button.png"
-00000fa0: 2061 6c74 3d22 6164 645f 696e 6c69 6e65   alt="add_inline
-00000fb0: 5f62 7574 746f 6e22 3e3c 2f70 3e0a 0a0a  _button"></p>...
-00000fc0: 2323 2320 c9aa c9b4 73e1 b49b e1b4 80ca  ### ....s.......
-00000fd0: 9fca 9fc9 aac9 b4c9 a220 3a2d 3e0a 0a60  ......... :->..`
-00000fe0: 6060 6261 7368 0a70 6970 2069 6e73 7461  ``bash.pip insta
-00000ff0: 6c6c 202d 5520 4162 670a 6060 600a 0ae2  ll -U Abg.```...
-00001000: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00001010: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00001020: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00001030: 9481 e294 81e2 9481 e294 810a 2323 20c9  ............## .
-00001040: b4e1 b48f e1b4 9be1 b487 203a 2d3e 0a0a  .......... :->..
-00001050: 2d20 5468 6973 206c 6962 7261 7279 2069  - This library i
-00001060: 7320 6d61 6465 2066 6f72 206d 7920 7065  s made for my pe
-00001070: 7273 6f6e 616c 2050 726f 6a65 6374 2073  rsonal Project s
-00001080: 6f20 646f 6e27 7420 7461 6b65 2069 7420  o don't take it 
-00001090: 6465 6570 6c79 202e 0a2d 204d 7920 5072  deeply ..- My Pr
-000010a0: 6f6a 6563 7420 5b40 4775 6172 6478 526f  oject [@GuardxRo
-000010b0: 626f 745d 2868 7474 7073 3a2f 2f74 2e6d  bot](https://t.m
-000010c0: 652f 4775 6172 6478 526f 626f 7429 200a  e/GuardxRobot) .
-000010d0: 0a2d 20e1 b487 c9b4 e1b4 8ae1 b48f ca8f  .- .............
-000010e0: 20ca 99e1 b480 ca99 ca8f 20e2 99a1 200a   ......... ... .
-000010f0: 0ae2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00001100: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00001110: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00001120: 81e2 9481 e294 81e2 9481 e294 8120 0a0a  ............. ..
-00001130: 0a0a                                     ..
+00000020: 5665 7273 696f 6e3a 2032 2e33 2e34 0a53  Version: 2.3.4.S
+00000030: 756d 6d61 7279 3a20 6164 642d 6f6e 2066  ummary: add-on f
+00000040: 6f72 2050 7972 6f67 7261 6d20 7c7c 2054  or Pyrogram || T
+00000050: 656c 6567 7261 6d20 626f 7420 6865 6c70  elegram bot help
+00000060: 6572 7320 7c7c 2045 6173 7920 626f 7474  ers || Easy bott
+00000070: 696e 670a 486f 6d65 2d70 6167 653a 2068  ing.Home-page: h
+00000080: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000090: 6d2f 4162 6973 686e 6f69 3639 2f41 6267  m/Abishnoi69/Abg
+000000a0: 0a41 7574 686f 723a 2041 6269 7368 6e6f  .Author: Abishno
+000000b0: 690a 4175 7468 6f72 2d65 6d61 696c 3a20  i.Author-email: 
+000000c0: 4162 6973 686e 6f69 3639 4041 6267 2e6f  Abishnoi69@Abg.o
+000000d0: 7267 0a4c 6963 656e 7365 3a20 4d49 540a  rg.License: MIT.
+000000e0: 446f 776e 6c6f 6164 2d55 524c 3a20 6874  Download-URL: ht
+000000f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000100: 2f41 6269 7368 6e6f 6936 392f 4162 672f  /Abishnoi69/Abg/
+00000110: 7265 6c65 6173 6573 2f6c 6174 6573 740a  releases/latest.
+00000120: 5072 6f6a 6563 742d 5552 4c3a 2054 7261  Project-URL: Tra
+00000130: 636b 6572 2c20 6874 7470 733a 2f2f 6769  cker, https://gi
+00000140: 7468 7562 2e63 6f6d 2f41 6269 7368 6e6f  thub.com/Abishno
+00000150: 6936 392f 4162 672f 6973 7375 6573 0a50  i69/Abg/issues.P
+00000160: 726f 6a65 6374 2d55 524c 3a20 436f 6d6d  roject-URL: Comm
+00000170: 756e 6974 792c 2068 7474 7073 3a2f 2f74  unity, https://t
+00000180: 2e6d 652f 4162 6770 790a 5072 6f6a 6563  .me/Abgpy.Projec
+00000190: 742d 5552 4c3a 2053 6f75 7263 652c 2068  t-URL: Source, h
+000001a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000001b0: 6d2f 4162 6973 686e 6f69 3639 2f41 6267  m/Abishnoi69/Abg
+000001c0: 0a50 726f 6a65 6374 2d55 524c 3a20 446f  .Project-URL: Do
+000001d0: 6375 6d65 6e74 6174 696f 6e2c 2068 7474  cumentation, htt
+000001e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000001f0: 4162 6973 686e 6f69 3639 2f41 6267 2f74  Abishnoi69/Abg/t
+00000200: 7265 652f 6d61 7374 6572 2f64 6f63 650a  ree/master/doce.
+00000210: 4465 7363 7269 7074 696f 6e3a 203c 7020  Description: <p 
+00000220: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+00000230: 2020 2020 2020 2020 3c62 3e20 4142 4720          <b> ABG 
+00000240: 3c2f 623e 0a20 2020 2020 2020 203c 2f70  </b>.        </p
+00000250: 3e0a 2020 2020 2020 2020 0a20 2020 2020  >.        .     
+00000260: 2020 203c 7020 616c 6967 6e3d 2263 656e     <p align="cen
+00000270: 7465 7222 3e3c 6120 6872 6566 3d22 6874  ter"><a href="ht
+00000280: 7470 733a 2f2f 7065 7079 2e74 6563 682f  tps://pepy.tech/
+00000290: 7072 6f6a 6563 742f 6162 6722 3e20 3c69  project/abg"> <i
+000002a0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000002b0: 7374 6174 6963 2e70 6570 792e 7465 6368  static.pepy.tech
+000002c0: 2f70 6572 736f 6e61 6c69 7a65 642d 6261  /personalized-ba
+000002d0: 6467 652f 6162 673f 7065 7269 6f64 3d74  dge/abg?period=t
+000002e0: 6f74 616c 2675 6e69 7473 3d69 6e74 6572  otal&units=inter
+000002f0: 6e61 7469 6f6e 616c 5f73 7973 7465 6d26  national_system&
+00000300: 6c65 6674 5f63 6f6c 6f72 3d62 6c61 636b  left_color=black
+00000310: 2672 6967 6874 5f63 6f6c 6f72 3d62 6c61  &right_color=bla
+00000320: 636b 266c 6566 745f 7465 7874 3d44 6f77  ck&left_text=Dow
+00000330: 6e6c 6f61 6473 2220 7769 6474 683d 2231  nloads" width="1
+00000340: 3639 2220 6865 6967 6874 3d22 3239 2e36  69" height="29.6
+00000350: 3922 2f3e 3c2f 613e 3c2f 703e 0a20 2020  9"/></a></p>.   
+00000360: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
+00000370: 2320 5265 7175 6972 656d 656e 7473 200a  # Requirements .
+00000380: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000390: 202d 2050 7974 686f 6e20 332e 3720 e1b4   - Python 3.7 ..
+000003a0: 8fca 8020 6869 6768 6572 2e0a 2020 2020  ... higher..    
+000003b0: 2020 2020 2d20 4120 5be1 b49b e1b4 87ca      - A [.......
+000003c0: 9fe1 b487 c9a2 ca80 e1b4 80e1 b48d 20e1  .............. .
+000003d0: b480 e1b4 98c9 aa20 e1b4 8be1 b487 ca8f  ....... ........
+000003e0: 5d28 6874 7470 733a 2f2f 646f 6373 2e70  ](https://docs.p
+000003f0: 7972 6f67 7261 6d2e 6f72 672f 696e 7472  yrogram.org/intr
+00000400: 6f2f 7365 7475 7023 6170 692d 6b65 7973  o/setup#api-keys
+00000410: 292e 0a20 2020 2020 2020 202d 20e1 b480  )..        - ...
+00000420: ca99 c9a2 205b e1b4 84e1 b48f c9b4 d293  .... [..........
+00000430: c9aa c9a2 5d28 6874 7470 733a 2f2f 6769  ....](https://gi
+00000440: 7468 7562 2e63 6f6d 2f41 6269 7368 6e6f  thub.com/Abishno
+00000450: 6936 392f 4162 6723 636f 6e66 6967 7572  i69/Abg#configur
+00000460: 6174 6f69 6e73 292e 0a20 2020 2020 2020  atoins)..       
+00000470: 200a 2020 2020 2020 2020 2323 2320 496e   .        ### In
+00000480: 7374 616c 6c69 6e67 203a 0a20 2020 2020  stalling :.     
+00000490: 2020 200a 2020 2020 2020 2020 6060 6062     .        ```b
+000004a0: 6173 680a 2020 2020 2020 2020 7069 7020  ash.        pip 
+000004b0: 696e 7374 616c 6c20 2d55 2041 6267 0a20  install -U Abg. 
+000004c0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+000004d0: 2020 2023 2323 2320 73e1 b487 e1b4 9be1     #### s.......
+000004e0: b49c e1b4 980a 2020 2020 2020 2020 6060  ......        ``
+000004f0: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
+00000500: 6672 6f6d 2070 7972 6f67 7261 6d20 696d  from pyrogram im
+00000510: 706f 7274 2066 696c 7465 7273 2c20 436c  port filters, Cl
+00000520: 6965 6e74 0a20 2020 2020 2020 2066 726f  ient.        fro
+00000530: 6d20 7079 726f 6772 616d 2e74 7970 6573  m pyrogram.types
+00000540: 2069 6d70 6f72 7420 4361 6c6c 6261 636b   import Callback
+00000550: 5175 6572 792c 204d 6573 7361 6765 0a20  Query, Message. 
+00000560: 2020 2020 2020 2066 726f 6d20 4162 6720         from Abg 
+00000570: 696d 706f 7274 2070 6174 6368 2020 2320  import patch  # 
+00000580: 7479 7065 203a 2069 676e 6f72 650a 2020  type : ignore.  
+00000590: 2020 2020 2020 6672 6f6d 2041 6267 2e68        from Abg.h
+000005a0: 656c 7065 7273 2069 6d70 6f72 7420 696b  elpers import ik
+000005b0: 620a 2020 2020 2020 2020 0a20 2020 2020  b.        .     
+000005c0: 2020 2061 7070 203d 2043 6c69 656e 7428     app = Client(
+000005d0: 226d 795f 6163 636f 756e 7422 290a 2020  "my_account").  
+000005e0: 2020 2020 2020 0a20 2020 2020 2020 2040        .        @
+000005f0: 6170 702e 6f6e 5f63 6d64 2822 6d79 696e  app.on_cmd("myin
+00000600: 666f 2229 0a20 2020 2020 2020 2052 6573  fo").        Res
+00000610: 756c 7464 6566 206d 795f 696e 666f 2873  ultdef my_info(s
+00000620: 656c 663a 2043 6c69 656e 742c 2063 7478  elf: Client, ctx
+00000630: 3a20 4d65 7373 6167 6529 3a0a 2020 2020  : Message):.    
+00000640: 2020 2020 2020 2020 6966 206e 6f74 2063          if not c
+00000650: 7478 2e66 726f 6d5f 7573 6572 3a0a 2020  tx.from_user:.  
+00000660: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00000670: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
+00000680: 206e 616d 6520 3d20 6177 6169 7420 6374   name = await ct
+00000690: 782e 6368 6174 2e61 736b 2822 5479 7065  x.chat.ask("Type
+000006a0: 2059 6f75 7220 4e61 6d65 2229 0a20 2020   Your Name").   
+000006b0: 2020 2020 2020 2020 2061 6765 203d 2061           age = a
+000006c0: 7761 6974 2063 7478 2e63 6861 742e 6173  wait ctx.chat.as
+000006d0: 6b28 2254 7970 6520 796f 7572 2061 6765  k("Type your age
+000006e0: 2229 0a20 2020 2020 2020 2020 2020 2061  ").            a
+000006f0: 6464 203d 2061 7761 6974 2063 7478 2e63  dd = await ctx.c
+00000700: 6861 742e 6173 6b28 2254 7970 6520 796f  hat.ask("Type yo
+00000710: 7572 2061 6464 7265 7373 2229 0a20 2020  ur address").   
+00000720: 2020 2020 2020 2020 2023 2079 6f75 2063           # you c
+00000730: 616e 2061 6c73 6f20 7573 6520 3a20 6374  an also use : ct
+00000740: 782e 7265 706c 795f 7465 7874 282e 2e2e  x.reply_text(...
+00000750: 290a 2020 2020 2020 2020 2020 2020 6177  ).            aw
+00000760: 6169 7420 7365 6c66 2e73 656e 645f 6d73  ait self.send_ms
+00000770: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
+00000780: 2020 2063 6861 745f 6964 3d63 7478 2e63     chat_id=ctx.c
+00000790: 6861 742e 6964 2c0a 2020 2020 2020 2020  hat.id,.        
+000007a0: 2020 2020 2020 2020 7465 7874 3d66 2259          text=f"Y
+000007b0: 6f75 7220 6e61 6d65 2069 733a 207b 6e61  our name is: {na
+000007c0: 6d65 2e74 6578 747d 5c6e 596f 7572 2061  me.text}\nYour a
+000007d0: 6765 2069 733a 207b 6167 652e 7465 7874  ge is: {age.text
+000007e0: 7d5c 6e79 6f75 7220 6164 6472 6573 7320  }\nyour address 
+000007f0: 6973 3a20 7b61 6464 2e74 6578 747d 222c  is: {add.text}",
+00000800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000810: 2072 6570 6c79 5f6d 6172 6b75 703d 696b   reply_markup=ik
+00000820: 6228 5b5b 2822 ca99 e1b4 9ce1 b49b e1b4  b([[("..........
+00000830: 9be1 b48f c9b4 222c 2022 6865 6c6c 6f22  ......", "hello"
+00000840: 295d 5d29 2c0a 2020 2020 2020 2020 2020  )]]),.          
+00000850: 2020 290a 2020 2020 2020 2020 0a20 2020    ).        .   
+00000860: 2020 2020 2023 2063 616c 6c62 6163 6b20       # callback 
+00000870: 0a20 2020 2020 2020 2040 6170 702e 6f6e  .        @app.on
+00000880: 5f63 6228 2268 656c 6c6f 2229 0a20 2020  _cb("hello").   
+00000890: 2020 2020 2061 7379 6e63 2064 6566 2068       async def h
+000008a0: 656c 6c6f 2863 3a20 436c 6965 6e74 2c20  ello(c: Client, 
+000008b0: 713a 2043 616c 6c62 6163 6b51 7565 7279  q: CallbackQuery
+000008c0: 293a 0a20 2020 2020 2020 2020 2020 2061  ):.            a
+000008d0: 7761 6974 2071 2e61 6e73 7765 7228 2248  wait q.answer("H
+000008e0: 656c 6c6f 2046 726f 6d20 4162 6722 2c20  ello From Abg", 
+000008f0: 7368 6f77 5f61 6c65 7274 3d54 7275 6529  show_alert=True)
+00000900: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000910: 2020 2020 6170 702e 7275 6e28 290a 2020      app.run().  
+00000920: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+00000930: 2020 3e0a 2020 2020 2020 2020 2323 2323    >.        ####
+00000940: 20e1 b49c 73e1 b487 ca80 2fca 99e1 b48f   ...s...../.....
+00000950: e1b4 9b20 ca80 c9aa c9a2 ca9c e1b4 9b73  ... ...........s
+00000960: 200a 2020 2020 2020 2020 0a20 2020 2020   .        .     
+00000970: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
+00000980: 2020 2020 2066 726f 6d20 4162 6720 696d       from Abg im
+00000990: 706f 7274 2070 6174 6368 2020 2320 616c  port patch  # al
+000009a0: 6c20 7061 7463 680a 2020 2020 2020 2020  l patch.        
+000009b0: 6672 6f6d 2070 7972 6f67 7261 6d2e 7479  from pyrogram.ty
+000009c0: 7065 7320 696d 706f 7274 204d 6573 7361  pes import Messa
+000009d0: 6765 0a20 2020 2020 2020 2066 726f 6d20  ge.        from 
+000009e0: 7079 726f 6772 616d 2069 6d70 6f72 7420  pyrogram import 
+000009f0: 436c 6965 6e74 0a20 2020 2020 2020 200a  Client.        .
+00000a00: 2020 2020 2020 2020 6170 7020 3d20 436c          app = Cl
+00000a10: 6965 6e74 2822 6d79 5f61 6363 6f75 6e74  ient("my_account
+00000a20: 2229 0a20 2020 2020 2020 200a 2020 2020  ").        .    
+00000a30: 2020 2020 4061 7070 2e6f 6e5f 636d 6428      @app.on_cmd(
+00000a40: 2264 656c 222c 2067 726f 7570 5f6f 6e6c  "del", group_onl
+00000a50: 793d 5472 7565 290a 2020 2020 2020 2020  y=True).        
+00000a60: 4061 7070 2e61 646d 696e 734f 6e6c 7928  @app.adminsOnly(
+00000a70: 7065 726d 6973 7369 6f6e 733d 2263 616e  permissions="can
+00000a80: 5f64 656c 6574 655f 6d65 7373 6167 6573  _delete_messages
+00000a90: 222c 2069 735f 626f 7468 3d54 7275 6529  ", is_both=True)
+00000aa0: 0a20 2020 2020 2020 2061 7379 6e63 2064  .        async d
+00000ab0: 6566 2064 656c 5f6d 7367 2863 3a20 436c  ef del_msg(c: Cl
+00000ac0: 6965 6e74 2c20 6d3a 204d 6573 7361 6765  ient, m: Message
+00000ad0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+00000ae0: 6620 6d2e 7265 706c 795f 746f 5f6d 6573  f m.reply_to_mes
+00000af0: 7361 6765 3a0a 2020 2020 2020 2020 2020  sage:.          
+00000b00: 2020 2020 2020 6177 6169 7420 6d2e 6465        await m.de
+00000b10: 6c65 7465 2829 0a20 2020 2020 2020 2020  lete().         
+00000b20: 2020 2020 2020 2061 7761 6974 2063 2e64         await c.d
+00000b30: 656c 6574 655f 6d65 7373 6167 6573 280a  elete_messages(.
+00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b50: 2020 2020 6368 6174 5f69 643d 6d2e 6368      chat_id=m.ch
+00000b60: 6174 2e69 642c 0a20 2020 2020 2020 2020  at.id,.         
+00000b70: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00000b80: 6765 5f69 6473 3d6d 2e72 6570 6c79 5f74  ge_ids=m.reply_t
+00000b90: 6f5f 6d65 7373 6167 652e 6964 2c0a 2020  o_message.id,.  
+00000ba0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00000bb0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00000bc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000bd0: 2020 6177 6169 7420 6d2e 7265 706c 795f    await m.reply_
+00000be0: 7465 7874 2874 6578 743d 22e1 b4a1 ca9c  text(text=".....
+00000bf0: e1b4 80e1 b49b 20e1 b485 e1b4 8f20 ca8f  ...... ...... ..
+00000c00: e1b4 8fe1 b49c 20e1 b4a1 e1b4 80c9 b4c9  ...... .........
+00000c10: b4e1 b480 20e1 b485 e1b4 87ca 9fe1 b487  .... ...........
+00000c20: e1b4 9be1 b487 3f22 290a 2020 2020 2020  ......?").      
+00000c30: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+00000c40: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000c50: 2020 6170 702e 7275 6e28 290a 2020 2020    app.run().    
+00000c60: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
+00000c70: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000c80: 2020 3e0a 2020 2020 2020 2020 2323 2320    >.        ### 
+00000c90: 6b65 7962 6f61 7264 2773 0a20 2020 2020  keyboard's.     
+00000ca0: 2020 200a 2020 2020 2020 2020 6060 6070     .        ```p
+00000cb0: 7974 686f 6e0a 2020 2020 2020 2020 6672  ython.        fr
+00000cc0: 6f6d 2041 6267 2e69 6e6c 696e 6520 696d  om Abg.inline im
+00000cd0: 706f 7274 2049 6e6c 696e 654b 6579 626f  port InlineKeybo
+00000ce0: 6172 642c 2049 6e6c 696e 6542 7574 746f  ard, InlineButto
+00000cf0: 6e0a 2020 2020 2020 2020 0a20 2020 2020  n.        .     
+00000d00: 2020 200a 2020 2020 2020 2020 6b65 7962     .        keyb
+00000d10: 6f61 7264 203d 2049 6e6c 696e 654b 6579  oard = InlineKey
+00000d20: 626f 6172 6428 726f 775f 7769 6474 683d  board(row_width=
+00000d30: 3329 0a20 2020 2020 2020 206b 6579 626f  3).        keybo
+00000d40: 6172 642e 6164 6428 0a20 2020 2020 2020  ard.add(.       
+00000d50: 2020 2020 2049 6e6c 696e 6542 7574 746f       InlineButto
+00000d60: 6e28 2731 272c 2027 696e 6c69 6e65 5f6b  n('1', 'inline_k
+00000d70: 6579 626f 6172 643a 3127 292c 0a20 2020  eyboard:1'),.   
+00000d80: 2020 2020 2020 2020 2049 6e6c 696e 6542           InlineB
+00000d90: 7574 746f 6e28 2732 272c 2027 696e 6c69  utton('2', 'inli
+00000da0: 6e65 5f6b 6579 626f 6172 643a 3227 292c  ne_keyboard:2'),
+00000db0: 0a20 2020 2020 2020 2020 2020 2049 6e6c  .            Inl
+00000dc0: 696e 6542 7574 746f 6e28 2733 272c 2027  ineButton('3', '
+00000dd0: 696e 6c69 6e65 5f6b 6579 626f 6172 643a  inline_keyboard:
+00000de0: 3327 292c 0a20 2020 2020 2020 2020 2020  3'),.           
+00000df0: 2049 6e6c 696e 6542 7574 746f 6e28 2734   InlineButton('4
+00000e00: 272c 2027 696e 6c69 6e65 5f6b 6579 626f  ', 'inline_keybo
+00000e10: 6172 643a 3427 292c 0a20 2020 2020 2020  ard:4'),.       
+00000e20: 2020 2020 2049 6e6c 696e 6542 7574 746f       InlineButto
+00000e30: 6e28 2735 272c 2027 696e 6c69 6e65 5f6b  n('5', 'inline_k
+00000e40: 6579 626f 6172 643a 3527 292c 0a20 2020  eyboard:5'),.   
+00000e50: 2020 2020 2020 2020 2049 6e6c 696e 6542           InlineB
+00000e60: 7574 746f 6e28 2736 272c 2027 696e 6c69  utton('6', 'inli
+00000e70: 6e65 5f6b 6579 626f 6172 643a 3627 292c  ne_keyboard:6'),
+00000e80: 0a20 2020 2020 2020 2020 2020 2049 6e6c  .            Inl
+00000e90: 696e 6542 7574 746f 6e28 2737 272c 2027  ineButton('7', '
+00000ea0: 696e 6c69 6e65 5f6b 6579 626f 6172 643a  inline_keyboard:
+00000eb0: 3727 290a 2020 2020 2020 2020 290a 2020  7').        ).  
+00000ec0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+00000ed0: 2020 0a20 2020 2020 2020 2023 2323 2320    .        #### 
+00000ee0: ca80 e1b4 8773 e1b4 9cca 9fe1 b49b 0a20  .....s......... 
+00000ef0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000f00: 3c70 3e3c 696d 6720 7372 633d 2268 7474  <p><img src="htt
+00000f10: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00000f20: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f41  sercontent.com/A
+00000f30: 6269 7368 6e6f 6936 392f 4162 672f 6d61  bishnoi69/Abg/ma
+00000f40: 7374 6572 2f64 6f63 652f 696d 6167 6573  ster/doce/images
+00000f50: 2f61 6464 5f69 6e6c 696e 655f 6275 7474  /add_inline_butt
+00000f60: 6f6e 2e70 6e67 2220 616c 743d 2261 6464  on.png" alt="add
+00000f70: 5f69 6e6c 696e 655f 6275 7474 6f6e 223e  _inline_button">
+00000f80: 3c2f 703e 0a20 2020 2020 2020 200a 2020  </p>.        .  
+00000f90: 2020 2020 2020 e294 81e2 9481 e294 81e2        ..........
+00000fa0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00000fb0: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00000fc0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00000fd0: 9481 0a20 2020 2020 2020 2023 2323 2043  ...        ### C
+00000fe0: 6f6e 6669 6775 7261 746f 696e 730a 2020  onfiguratoins.  
+00000ff0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+00001000: 2020 4f57 4e45 525f 4944 203d 20ca 8fe1    OWNER_ID = ...
+00001010: b48f e1b4 9cca 8020 e1b4 9be1 b487 ca9f  ....... ........
+00001020: e1b4 87c9 a2ca 80e1 b480 e1b4 8d20 c9aa  ............. ..
+00001030: e1b4 852e 0a20 2020 2020 2020 2044 4556  .....        DEV
+00001040: 5f55 5345 5253 203d 20ca 99e1 b48f e1b4  _USERS = .......
+00001050: 9b20 e1b4 85e1 b487 e1b4 a073 20c9 aae1  . .........s ...
+00001060: b485 2e20 28ca 8fe1 b48f e1b4 9c20 e1b4  ... (........ ..
+00001070: 84e1 b480 c9b4 20e1 b480 e1b4 85e1 b485  ...... .........
+00001080: 20e1 b480 20ca 9fc9 aa73 e1b4 9b20 3a20   ... ....s... : 
+00001090: 3120 3220 3329 0a20 2020 2020 2020 204c  1 2 3).        L
+000010a0: 4f47 4745 525f 4944 203d 20ca 8fe1 b48f  OGGER_ID = .....
+000010b0: e1b4 9cca 8020 e1b4 98ca 80c9 aae1 b4a0  ..... ..........
+000010c0: e1b4 80e1 b49b e1b4 8720 c9a2 ca80 e1b4  ......... ......
+000010d0: 8fe1 b49c e1b4 982f e1b4 84ca 9ce1 b480  ......./........
+000010e0: c9b4 c9b4 e1b4 87ca 9f20 c9aa e1b4 852e  ......... ......
+000010f0: 2028 ca9c e1b4 87ca 80e1 b487 20ca 99e1   (.......... ...
+00001100: b48f e1b4 9b20 73e1 b487 c9b4 e1b4 8520  ..... s........ 
+00001110: ca9f e1b4 8fc9 a273 290a 2020 2020 2020  .......s).      
+00001120: 2020 6060 600a 2020 2020 2020 2020 e294    ```.        ..
+00001130: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00001140: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00001150: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00001160: 81e2 9481 e294 81e2 9481 200a 2020 2020  .......... .    
+00001170: 2020 2020 0a20 2020 2020 2020 200a 4b65      .        .Ke
+00001180: 7977 6f72 6473 3a20 6164 642d 6f6e 2070  ywords: add-on p
+00001190: 7972 6f67 7261 6d20 626f 7473 2074 656c  yrogram bots tel
+000011a0: 6567 7261 6d20 626f 7420 6368 6174 206d  egram bot chat m
+000011b0: 6573 7365 6e67 6572 206d 7470 726f 746f  essenger mtproto
+000011c0: 2061 7069 2063 6c69 656e 7420 6c69 6272   api client libr
+000011d0: 6172 7920 7079 7468 6f6e 2063 6f6e 7665  ary python conve
+000011e0: 7273 6174 696f 6e20 6b65 7962 6f61 7264  rsation keyboard
+000011f0: 2075 7365 7262 6f74 2070 6174 6368 2068   userbot patch h
+00001200: 7474 7073 0a50 6c61 7466 6f72 6d3a 2055  ttps.Platform: U
+00001210: 4e4b 4e4f 574e 0a43 6c61 7373 6966 6965  NKNOWN.Classifie
+00001220: 723a 2044 6576 656c 6f70 6d65 6e74 2053  r: Development S
+00001230: 7461 7475 7320 3a3a 2035 202d 2050 726f  tatus :: 5 - Pro
+00001240: 6475 6374 696f 6e2f 5374 6162 6c65 0a43  duction/Stable.C
+00001250: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
+00001260: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+00001270: 4465 7665 6c6f 7065 7273 0a43 6c61 7373  Developers.Class
+00001280: 6966 6965 723a 204e 6174 7572 616c 204c  ifier: Natural L
+00001290: 616e 6775 6167 6520 3a3a 2045 6e67 6c69  anguage :: Engli
+000012a0: 7368 0a43 6c61 7373 6966 6965 723a 204f  sh.Classifier: O
+000012b0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+000012c0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+000012d0: 740a 436c 6173 7369 6669 6572 3a20 5072  t.Classifier: Pr
+000012e0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000012f0: 6765 203a 3a20 5079 7468 6f6e 0a43 6c61  ge :: Python.Cla
+00001300: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00001310: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00001320: 2050 7974 686f 6e20 3a3a 2033 0a43 6c61   Python :: 3.Cla
+00001330: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00001340: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00001350: 2050 7974 686f 6e20 3a3a 2033 2e37 0a43   Python :: 3.7.C
+00001360: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00001370: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00001380: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
+00001390: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000013a0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000013b0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000013c0: 2e39 0a43 6c61 7373 6966 6965 723a 2050  .9.Classifier: P
+000013d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000013e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000013f0: 2033 2e31 300a 436c 6173 7369 6669 6572   3.10.Classifier
+00001400: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00001410: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00001420: 203a 3a20 332e 3131 0a43 6c61 7373 6966   :: 3.11.Classif
+00001430: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00001440: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00001450: 686f 6e20 3a3a 2049 6d70 6c65 6d65 6e74  hon :: Implement
+00001460: 6174 696f 6e0a 436c 6173 7369 6669 6572  ation.Classifier
+00001470: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00001480: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00001490: 203a 3a20 496d 706c 656d 656e 7461 7469   :: Implementati
+000014a0: 6f6e 203a 3a20 4350 7974 686f 6e0a 436c  on :: CPython.Cl
+000014b0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000014c0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000014d0: 3a20 5079 7468 6f6e 203a 3a20 496d 706c  : Python :: Impl
+000014e0: 656d 656e 7461 7469 6f6e 203a 3a20 5079  ementation :: Py
+000014f0: 5079 0a43 6c61 7373 6966 6965 723a 2054  Py.Classifier: T
+00001500: 6f70 6963 203a 3a20 496e 7465 726e 6574  opic :: Internet
+00001510: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+00001520: 6963 203a 3a20 436f 6d6d 756e 6963 6174  ic :: Communicat
+00001530: 696f 6e73 0a43 6c61 7373 6966 6965 723a  ions.Classifier:
+00001540: 2054 6f70 6963 203a 3a20 436f 6d6d 756e   Topic :: Commun
+00001550: 6963 6174 696f 6e73 203a 3a20 4368 6174  ications :: Chat
+00001560: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+00001570: 6963 203a 3a20 536f 6674 7761 7265 2044  ic :: Software D
+00001580: 6576 656c 6f70 6d65 6e74 203a 3a20 4c69  evelopment :: Li
+00001590: 6272 6172 6965 730a 436c 6173 7369 6669  braries.Classifi
+000015a0: 6572 3a20 546f 7069 6320 3a3a 2053 6f66  er: Topic :: Sof
+000015b0: 7477 6172 6520 4465 7665 6c6f 706d 656e  tware Developmen
+000015c0: 7420 3a3a 204c 6962 7261 7269 6573 203a  t :: Libraries :
+000015d0: 3a20 5079 7468 6f6e 204d 6f64 756c 6573  : Python Modules
+000015e0: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+000015f0: 6963 203a 3a20 536f 6674 7761 7265 2044  ic :: Software D
+00001600: 6576 656c 6f70 6d65 6e74 203a 3a20 4c69  evelopment :: Li
+00001610: 6272 6172 6965 7320 3a3a 2041 7070 6c69  braries :: Appli
+00001620: 6361 7469 6f6e 2046 7261 6d65 776f 726b  cation Framework
+00001630: 730a 5265 7175 6972 6573 2d50 7974 686f  s.Requires-Pytho
+00001640: 6e3a 207e 3d33 2e37 0a44 6573 6372 6970  n: ~=3.7.Descrip
+00001650: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
+00001660: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
+00001670: 0a                                       .
```

### Comparing `Abg-2.3.3/README.md` & `Abg-2.3.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,167 +1,193 @@
-00000000: 2320 e1b4 80ca 99c9 a220 3a2d 3e20 5b21  # ....... :-> [!
-00000010: 5b44 6f77 6e6c 6f61 6473 5d28 6874 7470  [Downloads](http
-00000020: 733a 2f2f 7374 6174 6963 2e70 6570 792e  s://static.pepy.
-00000030: 7465 6368 2f70 6572 736f 6e61 6c69 7a65  tech/personalize
-00000040: 642d 6261 6467 652f 6162 673f 7065 7269  d-badge/abg?peri
-00000050: 6f64 3d74 6f74 616c 2675 6e69 7473 3d61  od=total&units=a
-00000060: 6262 7265 7669 6174 696f 6e26 6c65 6674  bbreviation&left
-00000070: 5f63 6f6c 6f72 3d62 6c61 636b 2672 6967  _color=black&rig
-00000080: 6874 5f63 6f6c 6f72 3d62 6c61 636b 266c  ht_color=black&l
-00000090: 6566 745f 7465 7874 3d44 6f77 6e6c 6f61  eft_text=Downloa
-000000a0: 6473 3a29 5d28 6874 7470 733a 2f2f 7065  ds:)](https://pe
-000000b0: 7079 2e74 6563 682f 7072 6f6a 6563 742f  py.tech/project/
-000000c0: 6162 6729 0a0a 3e20 0a23 2323 20e2 80a2  abg)..> .### ...
-000000d0: 2041 6267 0a0a 6060 6070 7974 686f 6e0a   Abg..```python.
-000000e0: 6672 6f6d 2070 7972 6f67 7261 6d20 696d  from pyrogram im
-000000f0: 706f 7274 2066 696c 7465 7273 2c20 436c  port filters, Cl
-00000100: 6965 6e74 0a66 726f 6d20 7079 726f 6772  ient.from pyrogr
-00000110: 616d 2e74 7970 6573 2069 6d70 6f72 7420  am.types import 
-00000120: 4361 6c6c 6261 636b 5175 6572 792c 204d  CallbackQuery, M
-00000130: 6573 7361 6765 0a66 726f 6d20 4162 6720  essage.from Abg 
-00000140: 696d 706f 7274 2070 6174 6368 2020 2320  import patch  # 
-00000150: 7479 7065 203a 2069 676e 6f72 650a 6672  type : ignore.fr
-00000160: 6f6d 2041 6267 2e68 656c 7065 7273 2069  om Abg.helpers i
-00000170: 6d70 6f72 7420 696b 620a 0a61 7070 203d  mport ikb..app =
-00000180: 2043 6c69 656e 7428 226d 795f 6163 636f   Client("my_acco
-00000190: 756e 7422 290a 0a40 6170 702e 6f6e 5f63  unt")..@app.on_c
-000001a0: 6d64 2822 6d79 696e 666f 2229 0a61 7379  md("myinfo").asy
-000001b0: 6e63 2064 6566 206d 795f 696e 666f 2873  nc def my_info(s
-000001c0: 656c 663a 2043 6c69 656e 742c 2063 7478  elf: Client, ctx
-000001d0: 3a20 4d65 7373 6167 6529 3a0a 2020 2020  : Message):.    
-000001e0: 6966 206e 6f74 2063 7478 2e66 726f 6d5f  if not ctx.from_
-000001f0: 7573 6572 3a0a 2020 2020 2020 2020 7265  user:.        re
-00000200: 7475 726e 0a20 2020 206e 616d 6520 3d20  turn.    name = 
-00000210: 6177 6169 7420 6374 782e 6368 6174 2e61  await ctx.chat.a
-00000220: 736b 2822 5479 7065 2059 6f75 7220 4e61  sk("Type Your Na
-00000230: 6d65 2229 0a20 2020 2061 6765 203d 2061  me").    age = a
-00000240: 7761 6974 2063 7478 2e63 6861 742e 6173  wait ctx.chat.as
-00000250: 6b28 2254 7970 6520 796f 7572 2061 6765  k("Type your age
-00000260: 2229 0a20 2020 2061 6464 203d 2061 7761  ").    add = awa
-00000270: 6974 2063 7478 2e63 6861 742e 6173 6b28  it ctx.chat.ask(
-00000280: 2254 7970 6520 796f 7572 2061 6464 7265  "Type your addre
-00000290: 7373 2229 0a20 2020 2023 2079 6f75 2063  ss").    # you c
-000002a0: 616e 2061 6c73 6f20 7573 6520 3a20 6374  an also use : ct
-000002b0: 782e 7265 706c 795f 7465 7874 282e 2e2e  x.reply_text(...
-000002c0: 290a 2020 2020 6177 6169 7420 7365 6c66  ).    await self
-000002d0: 2e73 656e 645f 6d73 6728 0a20 2020 2020  .send_msg(.     
-000002e0: 2020 2063 6861 745f 6964 3d63 7478 2e63     chat_id=ctx.c
-000002f0: 6861 742e 6964 2c0a 2020 2020 2020 2020  hat.id,.        
-00000300: 7465 7874 3d66 2259 6f75 7220 6e61 6d65  text=f"Your name
-00000310: 2069 733a 207b 6e61 6d65 2e74 6578 747d   is: {name.text}
-00000320: 5c6e 596f 7572 2061 6765 2069 733a 207b  \nYour age is: {
-00000330: 6167 652e 7465 7874 7d5c 6e79 6f75 7220  age.text}\nyour 
-00000340: 6164 6472 6573 7320 6973 3a20 7b61 6464  address is: {add
-00000350: 2e74 6578 747d 222c 0a20 2020 2020 2020  .text}",.       
-00000360: 2072 6570 6c79 5f6d 6172 6b75 703d 696b   reply_markup=ik
-00000370: 6228 5b5b 2822 ca99 e1b4 9ce1 b49b e1b4  b([[("..........
-00000380: 9be1 b48f c9b4 222c 2022 6865 6c6c 6f22  ......", "hello"
-00000390: 295d 5d29 2c0a 2020 2020 290a 0a23 2063  )]]),.    )..# c
-000003a0: 616c 6c62 6163 6b20 0a40 6170 702e 6f6e  allback .@app.on
-000003b0: 5f63 6228 2268 656c 6c6f 2229 0a61 7379  _cb("hello").asy
-000003c0: 6e63 2064 6566 2068 656c 6c6f 2863 3a20  nc def hello(c: 
-000003d0: 436c 6965 6e74 2c20 713a 2043 616c 6c62  Client, q: Callb
-000003e0: 6163 6b51 7565 7279 293a 0a20 2020 2061  ackQuery):.    a
-000003f0: 7761 6974 2071 2e61 6e73 7765 7228 2248  wait q.answer("H
-00000400: 656c 6c6f 2046 726f 6d20 4162 6722 2c20  ello From Abg", 
-00000410: 7368 6f77 5f61 6c65 7274 3d54 7275 6529  show_alert=True)
-00000420: 0a0a 2020 6170 702e 7275 6e28 290a 6060  ..  app.run().``
-00000430: 600a 3e0a 2323 2320 e280 a220 5573 6572  `.>.### ... User
-00000440: 2052 6967 6874 7320 0a0a 6060 6070 7974   Rights ..```pyt
-00000450: 686f 6e0a 6672 6f6d 2041 6267 2069 6d70  hon.from Abg imp
-00000460: 6f72 7420 7061 7463 6820 2023 2061 6c6c  ort patch  # all
-00000470: 2070 6174 6368 0a66 726f 6d20 7079 726f   patch.from pyro
-00000480: 6772 616d 2e74 7970 6573 2069 6d70 6f72  gram.types impor
-00000490: 7420 4d65 7373 6167 650a 6672 6f6d 2070  t Message.from p
-000004a0: 7972 6f67 7261 6d20 696d 706f 7274 2043  yrogram import C
-000004b0: 6c69 656e 740a 0a61 7070 203d 2043 6c69  lient..app = Cli
-000004c0: 656e 7428 226d 795f 6163 636f 756e 7422  ent("my_account"
-000004d0: 290a 0a40 6170 702e 6f6e 5f63 6d64 2822  )..@app.on_cmd("
-000004e0: 6465 6c22 2c20 6772 6f75 705f 6f6e 6c79  del", group_only
-000004f0: 3d54 7275 6529 0a40 6170 702e 6164 6d69  =True).@app.admi
-00000500: 6e73 4f6e 6c79 2870 6572 6d69 7373 696f  nsOnly(permissio
-00000510: 6e73 3d22 6361 6e5f 6465 6c65 7465 5f6d  ns="can_delete_m
-00000520: 6573 7361 6765 7322 2c20 6973 5f62 6f74  essages", is_bot
-00000530: 683d 5472 7565 290a 6173 796e 6320 6465  h=True).async de
-00000540: 6620 6465 6c5f 6d73 6728 633a 2043 6c69  f del_msg(c: Cli
-00000550: 656e 742c 206d 3a20 4d65 7373 6167 6529  ent, m: Message)
-00000560: 3a0a 2020 2020 6966 206d 2e72 6570 6c79  :.    if m.reply
-00000570: 5f74 6f5f 6d65 7373 6167 653a 0a20 2020  _to_message:.   
-00000580: 2020 2020 2061 7761 6974 206d 2e64 656c       await m.del
-00000590: 6574 6528 290a 2020 2020 2020 2020 6177  ete().        aw
-000005a0: 6169 7420 632e 6465 6c65 7465 5f6d 6573  ait c.delete_mes
-000005b0: 7361 6765 7328 0a20 2020 2020 2020 2020  sages(.         
-000005c0: 2020 2063 6861 745f 6964 3d6d 2e63 6861     chat_id=m.cha
-000005d0: 742e 6964 2c0a 2020 2020 2020 2020 2020  t.id,.          
-000005e0: 2020 6d65 7373 6167 655f 6964 733d 6d2e    message_ids=m.
-000005f0: 7265 706c 795f 746f 5f6d 6573 7361 6765  reply_to_message
-00000600: 2e69 642c 0a20 2020 2020 2020 2029 0a20  .id,.        ). 
-00000610: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00000620: 2061 7761 6974 206d 2e72 6570 6c79 5f74   await m.reply_t
-00000630: 6578 7428 7465 7874 3d22 e1b4 a1ca 9ce1  ext(text="......
-00000640: b480 e1b4 9b20 e1b4 85e1 b48f 20ca 8fe1  ..... ...... ...
-00000650: b48f e1b4 9c20 e1b4 a1e1 b480 c9b4 c9b4  ..... ..........
-00000660: e1b4 8020 e1b4 85e1 b487 ca9f e1b4 87e1  ... ............
-00000670: b49b e1b4 873f 2229 0a20 2020 2072 6574  .....?").    ret
-00000680: 7572 6e0a 2020 0a20 2061 7070 2e72 756e  urn.  .  app.run
-00000690: 2829 0a60 6060 0a0a 0a3e 0a23 2323 20e2  ().```...>.### .
-000006a0: 80a2 204b 6579 626f 6172 6473 0a0a 6060  .. Keyboards..``
-000006b0: 6070 7974 686f 6e0a 6672 6f6d 2041 6267  `python.from Abg
-000006c0: 2e69 6e6c 696e 6520 696d 706f 7274 2049  .inline import I
-000006d0: 6e6c 696e 654b 6579 626f 6172 642c 2049  nlineKeyboard, I
-000006e0: 6e6c 696e 6542 7574 746f 6e0a 0a0a 6b65  nlineButton...ke
-000006f0: 7962 6f61 7264 203d 2049 6e6c 696e 654b  yboard = InlineK
-00000700: 6579 626f 6172 6428 726f 775f 7769 6474  eyboard(row_widt
-00000710: 683d 3329 0a6b 6579 626f 6172 642e 6164  h=3).keyboard.ad
-00000720: 6428 0a20 2020 2049 6e6c 696e 6542 7574  d(.    InlineBut
-00000730: 746f 6e28 2731 272c 2027 696e 6c69 6e65  ton('1', 'inline
-00000740: 5f6b 6579 626f 6172 643a 3127 292c 0a20  _keyboard:1'),. 
-00000750: 2020 2049 6e6c 696e 6542 7574 746f 6e28     InlineButton(
-00000760: 2732 272c 2027 696e 6c69 6e65 5f6b 6579  '2', 'inline_key
-00000770: 626f 6172 643a 3227 292c 0a20 2020 2049  board:2'),.    I
-00000780: 6e6c 696e 6542 7574 746f 6e28 2733 272c  nlineButton('3',
-00000790: 2027 696e 6c69 6e65 5f6b 6579 626f 6172   'inline_keyboar
-000007a0: 643a 3327 292c 0a20 2020 2049 6e6c 696e  d:3'),.    Inlin
-000007b0: 6542 7574 746f 6e28 2734 272c 2027 696e  eButton('4', 'in
-000007c0: 6c69 6e65 5f6b 6579 626f 6172 643a 3427  line_keyboard:4'
-000007d0: 292c 0a20 2020 2049 6e6c 696e 6542 7574  ),.    InlineBut
-000007e0: 746f 6e28 2735 272c 2027 696e 6c69 6e65  ton('5', 'inline
-000007f0: 5f6b 6579 626f 6172 643a 3527 292c 0a20  _keyboard:5'),. 
-00000800: 2020 2049 6e6c 696e 6542 7574 746f 6e28     InlineButton(
-00000810: 2736 272c 2027 696e 6c69 6e65 5f6b 6579  '6', 'inline_key
-00000820: 626f 6172 643a 3627 292c 0a20 2020 2049  board:6'),.    I
-00000830: 6e6c 696e 6542 7574 746f 6e28 2737 272c  nlineButton('7',
-00000840: 2027 696e 6c69 6e65 5f6b 6579 626f 6172   'inline_keyboar
-00000850: 643a 3727 290a 290a 6060 600a 0a23 2323  d:7').).```..###
-00000860: 2320 5265 7375 6c74 0a0a 3c70 3e3c 696d  # Result..<p><im
-00000870: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00000880: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00000890: 7465 6e74 2e63 6f6d 2f41 6269 7368 6e6f  tent.com/Abishno
-000008a0: 6936 392f 4162 672f 6d61 7374 6572 2f64  i69/Abg/master/d
-000008b0: 6f63 652f 696d 6167 6573 2f61 6464 5f69  oce/images/add_i
-000008c0: 6e6c 696e 655f 6275 7474 6f6e 2e70 6e67  nline_button.png
-000008d0: 2220 616c 743d 2261 6464 5f69 6e6c 696e  " alt="add_inlin
-000008e0: 655f 6275 7474 6f6e 223e 3c2f 703e 0a0a  e_button"></p>..
-000008f0: 0a23 2323 20c9 aac9 b473 e1b4 9be1 b480  .### ....s......
-00000900: ca9f ca9f c9aa c9b4 c9a2 203a 2d3e 0a0a  .......... :->..
-00000910: 6060 6062 6173 680a 7069 7020 696e 7374  ```bash.pip inst
-00000920: 616c 6c20 2d55 2041 6267 0a60 6060 0a0a  all -U Abg.```..
-00000930: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00000940: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
-00000950: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00000960: e294 81e2 9481 e294 81e2 9481 0a23 2320  .............## 
-00000970: c9b4 e1b4 8fe1 b49b e1b4 8720 3a2d 3e0a  ........... :->.
-00000980: 0a2d 2054 6869 7320 6c69 6272 6172 7920  .- This library 
-00000990: 6973 206d 6164 6520 666f 7220 6d79 2070  is made for my p
-000009a0: 6572 736f 6e61 6c20 5072 6f6a 6563 7420  ersonal Project 
-000009b0: 736f 2064 6f6e 2774 2074 616b 6520 6974  so don't take it
-000009c0: 2064 6565 706c 7920 2e0a 2d20 4d79 2050   deeply ..- My P
-000009d0: 726f 6a65 6374 205b 4047 7561 7264 7852  roject [@GuardxR
-000009e0: 6f62 6f74 5d28 6874 7470 733a 2f2f 742e  obot](https://t.
-000009f0: 6d65 2f47 7561 7264 7852 6f62 6f74 2920  me/GuardxRobot) 
-00000a00: 0a0a 2d20 e1b4 87c9 b4e1 b48a e1b4 8fca  ..- ............
-00000a10: 8f20 ca99 e1b4 80ca 99ca 8f20 e299 a120  . ......... ... 
-00000a20: 0a0a e294 81e2 9481 e294 81e2 9481 e294  ................
-00000a30: 81e2 9481 e294 81e2 9481 e294 81e2 9481  ................
-00000a40: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
-00000a50: 9481 e294 81e2 9481 e294 81e2 9481 200a  .............. .
-00000a60: 0a                                       .
+00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000010: 223e 0a3c 623e 2041 4247 203c 2f62 3e0a  ">.<b> ABG </b>.
+00000020: 3c2f 703e 0a0a 3c70 2061 6c69 676e 3d22  </p>..<p align="
+00000030: 6365 6e74 6572 223e 3c61 2068 7265 663d  center"><a href=
+00000040: 2268 7474 7073 3a2f 2f70 6570 792e 7465  "https://pepy.te
+00000050: 6368 2f70 726f 6a65 6374 2f61 6267 223e  ch/project/abg">
+00000060: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00000070: 3a2f 2f73 7461 7469 632e 7065 7079 2e74  ://static.pepy.t
+00000080: 6563 682f 7065 7273 6f6e 616c 697a 6564  ech/personalized
+00000090: 2d62 6164 6765 2f61 6267 3f70 6572 696f  -badge/abg?perio
+000000a0: 643d 746f 7461 6c26 756e 6974 733d 696e  d=total&units=in
+000000b0: 7465 726e 6174 696f 6e61 6c5f 7379 7374  ternational_syst
+000000c0: 656d 266c 6566 745f 636f 6c6f 723d 626c  em&left_color=bl
+000000d0: 6163 6b26 7269 6768 745f 636f 6c6f 723d  ack&right_color=
+000000e0: 626c 6163 6b26 6c65 6674 5f74 6578 743d  black&left_text=
+000000f0: 446f 776e 6c6f 6164 7322 2077 6964 7468  Downloads" width
+00000100: 3d22 3136 3922 2068 6569 6768 743d 2232  ="169" height="2
+00000110: 392e 3639 222f 3e3c 2f61 3e3c 2f70 3e0a  9.69"/></a></p>.
+00000120: 0a23 2323 2052 6571 7569 7265 6d65 6e74  .### Requirement
+00000130: 7320 0a0a 2d20 5079 7468 6f6e 2033 2e37  s ..- Python 3.7
+00000140: 20e1 b48f ca80 2068 6967 6865 722e 0a2d   ..... higher..-
+00000150: 2041 205b e1b4 9be1 b487 ca9f e1b4 87c9   A [............
+00000160: a2ca 80e1 b480 e1b4 8d20 e1b4 80e1 b498  ......... ......
+00000170: c9aa 20e1 b48b e1b4 87ca 8f5d 2868 7474  .. ........](htt
+00000180: 7073 3a2f 2f64 6f63 732e 7079 726f 6772  ps://docs.pyrogr
+00000190: 616d 2e6f 7267 2f69 6e74 726f 2f73 6574  am.org/intro/set
+000001a0: 7570 2361 7069 2d6b 6579 7329 2e0a 2d20  up#api-keys)..- 
+000001b0: e1b4 80ca 99c9 a220 5be1 b484 e1b4 8fc9  ....... [.......
+000001c0: b4d2 93c9 aac9 a25d 2868 7474 7073 3a2f  .......](https:/
+000001d0: 2f67 6974 6875 622e 636f 6d2f 4162 6973  /github.com/Abis
+000001e0: 686e 6f69 3639 2f41 6267 2363 6f6e 6669  hnoi69/Abg#confi
+000001f0: 6775 7261 746f 696e 7329 2e0a 0a23 2323  guratoins)...###
+00000200: 2049 6e73 7461 6c6c 696e 6720 3a0a 0a60   Installing :..`
+00000210: 6060 6261 7368 0a70 6970 2069 6e73 7461  ``bash.pip insta
+00000220: 6c6c 202d 5520 4162 670a 6060 600a 2323  ll -U Abg.```.##
+00000230: 2323 2073 e1b4 87e1 b49b e1b4 9ce1 b498  ## s............
+00000240: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00000250: 7079 726f 6772 616d 2069 6d70 6f72 7420  pyrogram import 
+00000260: 6669 6c74 6572 732c 2043 6c69 656e 740a  filters, Client.
+00000270: 6672 6f6d 2070 7972 6f67 7261 6d2e 7479  from pyrogram.ty
+00000280: 7065 7320 696d 706f 7274 2043 616c 6c62  pes import Callb
+00000290: 6163 6b51 7565 7279 2c20 4d65 7373 6167  ackQuery, Messag
+000002a0: 650a 6672 6f6d 2041 6267 2069 6d70 6f72  e.from Abg impor
+000002b0: 7420 7061 7463 6820 2023 2074 7970 6520  t patch  # type 
+000002c0: 3a20 6967 6e6f 7265 0a66 726f 6d20 4162  : ignore.from Ab
+000002d0: 672e 6865 6c70 6572 7320 696d 706f 7274  g.helpers import
+000002e0: 2069 6b62 0a0a 6170 7020 3d20 436c 6965   ikb..app = Clie
+000002f0: 6e74 2822 6d79 5f61 6363 6f75 6e74 2229  nt("my_account")
+00000300: 0a0a 4061 7070 2e6f 6e5f 636d 6428 226d  ..@app.on_cmd("m
+00000310: 7969 6e66 6f22 290a 5265 7375 6c74 6465  yinfo").Resultde
+00000320: 6620 6d79 5f69 6e66 6f28 7365 6c66 3a20  f my_info(self: 
+00000330: 436c 6965 6e74 2c20 6374 783a 204d 6573  Client, ctx: Mes
+00000340: 7361 6765 293a 0a20 2020 2069 6620 6e6f  sage):.    if no
+00000350: 7420 6374 782e 6672 6f6d 5f75 7365 723a  t ctx.from_user:
+00000360: 0a20 2020 2020 2020 2072 6574 7572 6e0a  .        return.
+00000370: 2020 2020 6e61 6d65 203d 2061 7761 6974      name = await
+00000380: 2063 7478 2e63 6861 742e 6173 6b28 2254   ctx.chat.ask("T
+00000390: 7970 6520 596f 7572 204e 616d 6522 290a  ype Your Name").
+000003a0: 2020 2020 6167 6520 3d20 6177 6169 7420      age = await 
+000003b0: 6374 782e 6368 6174 2e61 736b 2822 5479  ctx.chat.ask("Ty
+000003c0: 7065 2079 6f75 7220 6167 6522 290a 2020  pe your age").  
+000003d0: 2020 6164 6420 3d20 6177 6169 7420 6374    add = await ct
+000003e0: 782e 6368 6174 2e61 736b 2822 5479 7065  x.chat.ask("Type
+000003f0: 2079 6f75 7220 6164 6472 6573 7322 290a   your address").
+00000400: 2020 2020 2320 796f 7520 6361 6e20 616c      # you can al
+00000410: 736f 2075 7365 203a 2063 7478 2e72 6570  so use : ctx.rep
+00000420: 6c79 5f74 6578 7428 2e2e 2e29 0a20 2020  ly_text(...).   
+00000430: 2061 7761 6974 2073 656c 662e 7365 6e64   await self.send
+00000440: 5f6d 7367 280a 2020 2020 2020 2020 6368  _msg(.        ch
+00000450: 6174 5f69 643d 6374 782e 6368 6174 2e69  at_id=ctx.chat.i
+00000460: 642c 0a20 2020 2020 2020 2074 6578 743d  d,.        text=
+00000470: 6622 596f 7572 206e 616d 6520 6973 3a20  f"Your name is: 
+00000480: 7b6e 616d 652e 7465 7874 7d5c 6e59 6f75  {name.text}\nYou
+00000490: 7220 6167 6520 6973 3a20 7b61 6765 2e74  r age is: {age.t
+000004a0: 6578 747d 5c6e 796f 7572 2061 6464 7265  ext}\nyour addre
+000004b0: 7373 2069 733a 207b 6164 642e 7465 7874  ss is: {add.text
+000004c0: 7d22 2c0a 2020 2020 2020 2020 7265 706c  }",.        repl
+000004d0: 795f 6d61 726b 7570 3d69 6b62 285b 5b28  y_markup=ikb([[(
+000004e0: 22ca 99e1 b49c e1b4 9be1 b49b e1b4 8fc9  "...............
+000004f0: b422 2c20 2268 656c 6c6f 2229 5d5d 292c  .", "hello")]]),
+00000500: 0a20 2020 2029 0a0a 2320 6361 6c6c 6261  .    )..# callba
+00000510: 636b 200a 4061 7070 2e6f 6e5f 6362 2822  ck .@app.on_cb("
+00000520: 6865 6c6c 6f22 290a 6173 796e 6320 6465  hello").async de
+00000530: 6620 6865 6c6c 6f28 633a 2043 6c69 656e  f hello(c: Clien
+00000540: 742c 2071 3a20 4361 6c6c 6261 636b 5175  t, q: CallbackQu
+00000550: 6572 7929 3a0a 2020 2020 6177 6169 7420  ery):.    await 
+00000560: 712e 616e 7377 6572 2822 4865 6c6c 6f20  q.answer("Hello 
+00000570: 4672 6f6d 2041 6267 222c 2073 686f 775f  From Abg", show_
+00000580: 616c 6572 743d 5472 7565 290a 0a20 2061  alert=True)..  a
+00000590: 7070 2e72 756e 2829 0a60 6060 0a3e 0a23  pp.run().```.>.#
+000005a0: 2323 2320 e1b4 9c73 e1b4 87ca 802f ca99  ### ...s...../..
+000005b0: e1b4 8fe1 b49b 20ca 80c9 aac9 a2ca 9ce1  ...... .........
+000005c0: b49b 7320 0a0a 6060 6070 7974 686f 6e0a  ..s ..```python.
+000005d0: 6672 6f6d 2041 6267 2069 6d70 6f72 7420  from Abg import 
+000005e0: 7061 7463 6820 2023 2061 6c6c 2070 6174  patch  # all pat
+000005f0: 6368 0a66 726f 6d20 7079 726f 6772 616d  ch.from pyrogram
+00000600: 2e74 7970 6573 2069 6d70 6f72 7420 4d65  .types import Me
+00000610: 7373 6167 650a 6672 6f6d 2070 7972 6f67  ssage.from pyrog
+00000620: 7261 6d20 696d 706f 7274 2043 6c69 656e  ram import Clien
+00000630: 740a 0a61 7070 203d 2043 6c69 656e 7428  t..app = Client(
+00000640: 226d 795f 6163 636f 756e 7422 290a 0a40  "my_account")..@
+00000650: 6170 702e 6f6e 5f63 6d64 2822 6465 6c22  app.on_cmd("del"
+00000660: 2c20 6772 6f75 705f 6f6e 6c79 3d54 7275  , group_only=Tru
+00000670: 6529 0a40 6170 702e 6164 6d69 6e73 4f6e  e).@app.adminsOn
+00000680: 6c79 2870 6572 6d69 7373 696f 6e73 3d22  ly(permissions="
+00000690: 6361 6e5f 6465 6c65 7465 5f6d 6573 7361  can_delete_messa
+000006a0: 6765 7322 2c20 6973 5f62 6f74 683d 5472  ges", is_both=Tr
+000006b0: 7565 290a 6173 796e 6320 6465 6620 6465  ue).async def de
+000006c0: 6c5f 6d73 6728 633a 2043 6c69 656e 742c  l_msg(c: Client,
+000006d0: 206d 3a20 4d65 7373 6167 6529 3a0a 2020   m: Message):.  
+000006e0: 2020 6966 206d 2e72 6570 6c79 5f74 6f5f    if m.reply_to_
+000006f0: 6d65 7373 6167 653a 0a20 2020 2020 2020  message:.       
+00000700: 2061 7761 6974 206d 2e64 656c 6574 6528   await m.delete(
+00000710: 290a 2020 2020 2020 2020 6177 6169 7420  ).        await 
+00000720: 632e 6465 6c65 7465 5f6d 6573 7361 6765  c.delete_message
+00000730: 7328 0a20 2020 2020 2020 2020 2020 2063  s(.            c
+00000740: 6861 745f 6964 3d6d 2e63 6861 742e 6964  hat_id=m.chat.id
+00000750: 2c0a 2020 2020 2020 2020 2020 2020 6d65  ,.            me
+00000760: 7373 6167 655f 6964 733d 6d2e 7265 706c  ssage_ids=m.repl
+00000770: 795f 746f 5f6d 6573 7361 6765 2e69 642c  y_to_message.id,
+00000780: 0a20 2020 2020 2020 2029 0a20 2020 2065  .        ).    e
+00000790: 6c73 653a 0a20 2020 2020 2020 2061 7761  lse:.        awa
+000007a0: 6974 206d 2e72 6570 6c79 5f74 6578 7428  it m.reply_text(
+000007b0: 7465 7874 3d22 e1b4 a1ca 9ce1 b480 e1b4  text="..........
+000007c0: 9b20 e1b4 85e1 b48f 20ca 8fe1 b48f e1b4  . ...... .......
+000007d0: 9c20 e1b4 a1e1 b480 c9b4 c9b4 e1b4 8020  . ............. 
+000007e0: e1b4 85e1 b487 ca9f e1b4 87e1 b49b e1b4  ................
+000007f0: 873f 2229 0a20 2020 2072 6574 7572 6e0a  .?").    return.
+00000800: 2020 0a20 2061 7070 2e72 756e 2829 0a60    .  app.run().`
+00000810: 6060 0a0a 0a3e 0a23 2323 206b 6579 626f  ``...>.### keybo
+00000820: 6172 6427 730a 0a60 6060 7079 7468 6f6e  ard's..```python
+00000830: 0a66 726f 6d20 4162 672e 696e 6c69 6e65  .from Abg.inline
+00000840: 2069 6d70 6f72 7420 496e 6c69 6e65 4b65   import InlineKe
+00000850: 7962 6f61 7264 2c20 496e 6c69 6e65 4275  yboard, InlineBu
+00000860: 7474 6f6e 0a0a 0a6b 6579 626f 6172 6420  tton...keyboard 
+00000870: 3d20 496e 6c69 6e65 4b65 7962 6f61 7264  = InlineKeyboard
+00000880: 2872 6f77 5f77 6964 7468 3d33 290a 6b65  (row_width=3).ke
+00000890: 7962 6f61 7264 2e61 6464 280a 2020 2020  yboard.add(.    
+000008a0: 496e 6c69 6e65 4275 7474 6f6e 2827 3127  InlineButton('1'
+000008b0: 2c20 2769 6e6c 696e 655f 6b65 7962 6f61  , 'inline_keyboa
+000008c0: 7264 3a31 2729 2c0a 2020 2020 496e 6c69  rd:1'),.    Inli
+000008d0: 6e65 4275 7474 6f6e 2827 3227 2c20 2769  neButton('2', 'i
+000008e0: 6e6c 696e 655f 6b65 7962 6f61 7264 3a32  nline_keyboard:2
+000008f0: 2729 2c0a 2020 2020 496e 6c69 6e65 4275  '),.    InlineBu
+00000900: 7474 6f6e 2827 3327 2c20 2769 6e6c 696e  tton('3', 'inlin
+00000910: 655f 6b65 7962 6f61 7264 3a33 2729 2c0a  e_keyboard:3'),.
+00000920: 2020 2020 496e 6c69 6e65 4275 7474 6f6e      InlineButton
+00000930: 2827 3427 2c20 2769 6e6c 696e 655f 6b65  ('4', 'inline_ke
+00000940: 7962 6f61 7264 3a34 2729 2c0a 2020 2020  yboard:4'),.    
+00000950: 496e 6c69 6e65 4275 7474 6f6e 2827 3527  InlineButton('5'
+00000960: 2c20 2769 6e6c 696e 655f 6b65 7962 6f61  , 'inline_keyboa
+00000970: 7264 3a35 2729 2c0a 2020 2020 496e 6c69  rd:5'),.    Inli
+00000980: 6e65 4275 7474 6f6e 2827 3627 2c20 2769  neButton('6', 'i
+00000990: 6e6c 696e 655f 6b65 7962 6f61 7264 3a36  nline_keyboard:6
+000009a0: 2729 2c0a 2020 2020 496e 6c69 6e65 4275  '),.    InlineBu
+000009b0: 7474 6f6e 2827 3727 2c20 2769 6e6c 696e  tton('7', 'inlin
+000009c0: 655f 6b65 7962 6f61 7264 3a37 2729 0a29  e_keyboard:7').)
+000009d0: 0a60 6060 0a0a 2323 2323 20ca 80e1 b487  .```..#### .....
+000009e0: 73e1 b49c ca9f e1b4 9b0a 0a3c 703e 3c69  s..........<p><i
+000009f0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000a00: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+00000a10: 6e74 656e 742e 636f 6d2f 4162 6973 686e  ntent.com/Abishn
+00000a20: 6f69 3639 2f41 6267 2f6d 6173 7465 722f  oi69/Abg/master/
+00000a30: 646f 6365 2f69 6d61 6765 732f 6164 645f  doce/images/add_
+00000a40: 696e 6c69 6e65 5f62 7574 746f 6e2e 706e  inline_button.pn
+00000a50: 6722 2061 6c74 3d22 6164 645f 696e 6c69  g" alt="add_inli
+00000a60: 6e65 5f62 7574 746f 6e22 3e3c 2f70 3e0a  ne_button"></p>.
+00000a70: 0ae2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00000a80: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00000a90: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00000aa0: 81e2 9481 e294 81e2 9481 e294 810a 2323  ..............##
+00000ab0: 2320 436f 6e66 6967 7572 6174 6f69 6e73  # Configuratoins
+00000ac0: 0a60 6060 0a4f 574e 4552 5f49 4420 3d20  .```.OWNER_ID = 
+00000ad0: ca8f e1b4 8fe1 b49c ca80 20e1 b49b e1b4  .......... .....
+00000ae0: 87ca 9fe1 b487 c9a2 ca80 e1b4 80e1 b48d  ................
+00000af0: 20c9 aae1 b485 2e0a 4445 565f 5553 4552   .......DEV_USER
+00000b00: 5320 3d20 ca99 e1b4 8fe1 b49b 20e1 b485  S = ........ ...
+00000b10: e1b4 87e1 b4a0 7320 c9aa e1b4 852e 2028  ......s ...... (
+00000b20: ca8f e1b4 8fe1 b49c 20e1 b484 e1b4 80c9  ........ .......
+00000b30: b420 e1b4 80e1 b485 e1b4 8520 e1b4 8020  . ......... ... 
+00000b40: ca9f c9aa 73e1 b49b 203a 2031 2032 2033  ....s... : 1 2 3
+00000b50: 290a 4c4f 4747 4552 5f49 4420 3d20 ca8f  ).LOGGER_ID = ..
+00000b60: e1b4 8fe1 b49c ca80 20e1 b498 ca80 c9aa  ........ .......
+00000b70: e1b4 a0e1 b480 e1b4 9be1 b487 20c9 a2ca  ............ ...
+00000b80: 80e1 b48f e1b4 9ce1 b498 2fe1 b484 ca9c  ........../.....
+00000b90: e1b4 80c9 b4c9 b4e1 b487 ca9f 20c9 aae1  ............ ...
+00000ba0: b485 2e20 28ca 9ce1 b487 ca80 e1b4 8720  ... (.......... 
+00000bb0: ca99 e1b4 8fe1 b49b 2073 e1b4 87c9 b4e1  ........ s......
+00000bc0: b485 20ca 9fe1 b48f c9a2 7329 0a60 6060  .. .......s).```
+00000bd0: 0ae2 9481 e294 81e2 9481 e294 81e2 9481  ................
+00000be0: e294 81e2 9481 e294 81e2 9481 e294 81e2  ................
+00000bf0: 9481 e294 81e2 9481 e294 81e2 9481 e294  ................
+00000c00: 81e2 9481 e294 81e2 9481 e294 8120 0a0a  ............. ..
```

### Comparing `Abg-2.3.3/setup.py` & `Abg-2.3.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 
 import setuptools
 
 with open("README.md", encoding="utf8") as readme:
     long_description = readme.read()
 
 """    
-def read(file: str) -> list:
-    with open(file, encoding="utf-8") as r:
-        return [i.strip() for i in r]
+with open("requirements.txt", encoding="utf-8") as f:
+    requires = f.read().splitlines()
 """
 
+
 setuptools.setup(
     name="Abg",
     packages=setuptools.find_packages(),
-    version="2.3.3",
-    description="Telegram bot helpers",
+    version="2.3.4",
+    description="add-on for Pyrogram || Telegram bot helpers || Easy botting",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Abishnoi69/Abg",
     download_url="https://github.com/Abishnoi69/Abg/releases/latest",
     author="Abishnoi",
     author_email="Abishnoi69@Abg.org",
     license="MIT",
@@ -59,17 +59,18 @@
         "Topic :: Internet",
         "Topic :: Communications",
         "Topic :: Communications :: Chat",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
     ],
-    keywords="telegram bot chat messenger mtproto api client library python conversation keyboard userbot patch botapi https",
+    keywords="add-on pyrogram bots telegram bot chat messenger mtproto api client library python conversation keyboard userbot patch https",
     project_urls={
         "Tracker": "https://github.com/Abishnoi69/Abg/issues",
         "Community": "https://t.me/Abgpy",
         "Source": "https://github.com/Abishnoi69/Abg",
         "Documentation": "https://github.com/Abishnoi69/Abg/tree/master/doce",
     },
     python_requires="~=3.7",
-    # install_requires=read("requirements.txt")
+    zip_safe=False,
+    # install_requires=requires,
 )
```

