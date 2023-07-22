# Comparing `tmp/pymino-1.2.3.8.tar.gz` & `tmp/pymino-1.2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymino-1.2.3.8.tar", last modified: Thu Jul 20 02:36:44 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\sss\pymino-1.2.3.8\dist\.tmp-c7bzuq5d\pymino-1.2.3.9.tar", last modified: Sat Jul 22 04:10:38 2023, max compression
```

## Comparing `pymino-1.2.3.8.tar` & `pymino-1.2.3.9.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 02:36:44.840171 pymino-1.2.3.8/
--rw-rw-rw-   0        0        0     1085 2023-07-14 23:58:40.000000 pymino-1.2.3.8/LICENSE
--rw-rw-rw-   0        0        0     7424 2023-07-20 02:36:44.840171 pymino-1.2.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     6706 2023-07-20 02:36:23.000000 pymino-1.2.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 02:36:44.701586 pymino-1.2.3.8/pymino/
--rw-rw-rw-   0        0        0      775 2023-07-20 02:33:23.000000 pymino-1.2.3.8/pymino/__init__.py
--rw-rw-rw-   0        0        0    11744 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/async_bot.py
--rw-rw-rw-   0        0        0    37317 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/async_client.py
--rw-rw-rw-   0        0        0    31005 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/bot.py
--rw-rw-rw-   0        0        0    36840 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-07-20 02:36:44.780748 pymino-1.2.3.8/pymino/ext/
--rw-rw-rw-   0        0        0      651 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0      192 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/_global.py
--rw-rw-rw-   0        0        0    11196 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/account.py
--rw-rw-rw-   0        0        0    11496 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/async_account.py
--rw-rw-rw-   0        0        0   345197 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    21402 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    25878 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0    72111 2023-07-20 02:29:35.000000 pymino-1.2.3.8/pymino/ext/async_global_client.py
--rw-rw-rw-   0        0        0     7233 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   344129 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/console.py
--rw-rw-rw-   0        0        0    45520 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1856 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-07-20 02:36:44.817489 pymino-1.2.3.8/pymino/ext/entities/
--rw-rw-rw-   0        0        0      428 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/entities/acm.py
--rw-rw-rw-   0        0        0     9014 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/entities/admin_log.py
--rw-rw-rw-   0        0        0     1670 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    17769 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/entities/bubble.py
--rw-rw-rw-   0        0        0    20322 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    16021 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43827 2023-07-20 01:14:10.000000 pymino-1.2.3.8/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4802 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0     3831 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/entities/member.py
--rw-rw-rw-   0        0        0    42520 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1839 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31711 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/entities/sticker.py
--rw-rw-rw-   0        0        0     6185 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    32554 2023-07-20 02:18:21.000000 pymino-1.2.3.8/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0    74405 2023-07-20 01:25:38.000000 pymino-1.2.3.8/pymino/ext/global_client.py
--rw-rw-rw-   0        0        0      543 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6657 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-07-20 02:36:44.838172 pymino-1.2.3.8/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11544 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6280 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1110 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10404 2023-07-14 23:58:40.000000 pymino-1.2.3.8/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-20 02:36:44.716544 pymino-1.2.3.8/pymino.egg-info/
--rw-rw-rw-   0        0        0     7424 2023-07-20 02:36:44.000000 pymino-1.2.3.8/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1640 2023-07-20 02:36:44.000000 pymino-1.2.3.8/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 02:36:44.000000 pymino-1.2.3.8/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2023-07-20 02:36:44.000000 pymino-1.2.3.8/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-20 02:36:44.000000 pymino-1.2.3.8/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-07-20 02:36:44.851141 pymino-1.2.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1394 2023-07-14 23:58:40.000000 pymino-1.2.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 04:10:38.225197 pymino-1.2.3.9/
+-rw-rw-rw-   0        0        0     1085 2023-07-14 23:58:40.000000 pymino-1.2.3.9/LICENSE
+-rw-rw-rw-   0        0        0     7373 2023-07-22 04:10:38.225197 pymino-1.2.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6706 2023-07-20 02:36:23.000000 pymino-1.2.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 04:10:38.109628 pymino-1.2.3.9/pymino/
+-rw-rw-rw-   0        0        0      952 2023-07-22 04:00:11.000000 pymino-1.2.3.9/pymino/__init__.py
+-rw-rw-rw-   0        0        0    12297 2023-07-22 04:05:59.000000 pymino-1.2.3.9/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    38219 2023-07-22 04:02:40.000000 pymino-1.2.3.9/pymino/async_client.py
+-rw-rw-rw-   0        0        0    32248 2023-07-22 03:46:10.000000 pymino-1.2.3.9/pymino/bot.py
+-rw-rw-rw-   0        0        0    37736 2023-07-22 04:05:43.000000 pymino-1.2.3.9/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-07-22 04:10:38.164684 pymino-1.2.3.9/pymino/ext/
+-rw-rw-rw-   0        0        0      638 2023-07-22 03:26:20.000000 pymino-1.2.3.9/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    11300 2023-07-22 04:04:33.000000 pymino-1.2.3.9/pymino/ext/account.py
+-rw-rw-rw-   0        0        0    11529 2023-07-22 04:02:21.000000 pymino-1.2.3.9/pymino/ext/async_account.py
+-rw-rw-rw-   0        0        0   345197 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    21402 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    25878 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0    72111 2023-07-20 02:29:35.000000 pymino-1.2.3.9/pymino/ext/async_global_client.py
+-rw-rw-rw-   0        0        0     7203 2023-07-22 02:16:09.000000 pymino-1.2.3.9/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   344131 2023-07-22 03:45:27.000000 pymino-1.2.3.9/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    45520 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     2052 2023-07-21 19:38:46.000000 pymino-1.2.3.9/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-07-22 04:10:38.204365 pymino-1.2.3.9/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      428 2023-07-22 03:26:32.000000 pymino-1.2.3.9/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/entities/acm.py
+-rw-rw-rw-   0        0        0     9014 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/entities/admin_log.py
+-rw-rw-rw-   0        0        0     1670 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    17769 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/entities/bubble.py
+-rw-rw-rw-   0        0        0    20322 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    16021 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43827 2023-07-20 01:14:10.000000 pymino-1.2.3.9/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     5516 2023-07-21 20:49:34.000000 pymino-1.2.3.9/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0     3831 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/entities/member.py
+-rw-rw-rw-   0        0        0    42520 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1839 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31711 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/entities/sticker.py
+-rw-rw-rw-   0        0        0     6185 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    32554 2023-07-22 03:19:41.000000 pymino-1.2.3.9/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0    74405 2023-07-20 01:25:38.000000 pymino-1.2.3.9/pymino/ext/global_client.py
+-rw-rw-rw-   0        0        0      543 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6609 2023-07-21 21:24:55.000000 pymino-1.2.3.9/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-07-22 04:10:38.223708 pymino-1.2.3.9/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11719 2023-07-22 02:49:03.000000 pymino-1.2.3.9/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6280 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1514 2023-07-22 04:06:11.000000 pymino-1.2.3.9/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-07-14 23:58:40.000000 pymino-1.2.3.9/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10853 2023-07-22 03:21:49.000000 pymino-1.2.3.9/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-22 04:10:38.123516 pymino-1.2.3.9/pymino.egg-info/
+-rw-rw-rw-   0        0        0     7373 2023-07-22 04:10:38.000000 pymino-1.2.3.9/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1618 2023-07-22 04:10:38.000000 pymino-1.2.3.9/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 04:10:38.000000 pymino-1.2.3.9/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-07-22 04:10:38.000000 pymino-1.2.3.9/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-22 04:10:38.000000 pymino-1.2.3.9/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      833 2023-07-22 04:10:38.227180 pymino-1.2.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-07-22 02:34:26.000000 pymino-1.2.3.9/setup.py
```

### Comparing `pymino-1.2.3.8/LICENSE` & `pymino-1.2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/PKG-INFO` & `pymino-1.2.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.3.8
+Version: 1.2.3.9
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <h1 style="color: #0d47a1; font-size: 3em;">pymino</h1>
   
   <p>
```

#### html2text {}

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.3.8 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.3.9 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE
+:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Requires-Python: >=3.8 Description-Content-Type:
+text/markdown License-File: LICENSE
                              ****** pymino ******
 [Discord] [Libraries.io_dependency_status_for_GitHub_repo] [GitHub_last_commit]
                               [PyPI_-_Downloads]
            A Python wrapper to communicate with the Amino Apps API.
     Easily create a bot for Amino Apps using a modern, easy-to-use library.
                                **** WARNING ****
  Pymino is a fully reverse-engineered client. By using this client, you may be
```

### Comparing `pymino-1.2.3.8/README.md` & `pymino-1.2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/__init__.py` & `pymino-1.2.3.9/pymino/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,32 @@
+from typing import List
+from requests import get
+from colorama import Fore, Style
+
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.2.3.8'
+__version__ = '1.2.3.9'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
-from .bot import Bot as Bot
-from .async_bot import AsyncBot as AsyncBot
-from .client import Client as Client
-from .async_client import AsyncClient as AsyncClient
+from .bot import Bot
+from .async_bot import AsyncBot
+from .client import Client
+from .async_client import AsyncClient
 
-from requests import get
-from colorama import Fore, Style
+__all__: List[str] = [
+    'Bot',
+    'AsyncBot',
+    'Client',
+    'AsyncClient',
+]
 
 print("Join the pymino discord server: https://discord.gg/RuRzyya55Z")
 
-latestVersion = get("https://pypi.org/pypi/pymino/json").json()["info"]["version"]
-
-if __version__ != latestVersion:
-    print(f"{Fore.RED}WARNING:{Style.RESET_ALL} You are using an outdated version of pymino ({__version__}). The latest version is {latestVersion}.")
+try:
+    latest_version = get("https://pypi.org/pypi/pymino/json").json()["info"]["version"]
+except Exception as e:
+    print(f"Failed to check the latest version: {e}")
+else:
+    if __version__ != latest_version:
+        print(f"{Fore.RED}WARNING:{Style.RESET_ALL} You are using an outdated version of pymino ({__version__}). The latest version is {latest_version}.")
```

### Comparing `pymino-1.2.3.8/pymino/async_bot.py` & `pymino-1.2.3.9/pymino/async_bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import asyncio
 from typing import Optional, Union
 from time import time, perf_counter
 
 from .ext.entities import *
 from .ext.async_socket import AsyncWSClient
+from .ext.utilities.generate import Generator
 from .ext.async_community import AsyncCommunity
-from .ext.utilities.generate import device_id as generate_device_id
+from .ext.async_global_client import AsyncGlobal
 from .ext.utilities.async_request_handler import AsyncRequestHandler
 
 
-class AsyncBot(AsyncWSClient):
+class AsyncBot(AsyncWSClient, AsyncGlobal):
     def __init__(
         self,
         command_prefix: Optional[str] = "!",
         community_id: Union[str, int] = None,
         device_id: Optional[str] = None,
         intents: bool = False,
         online_status: bool = False,
-        proxy: Optional[str] = None
-        ):
+        proxy: Optional[str] = None,
+        hash_prefix: Union[str, int] = 19,
+        device_key: str = "E7309ECC0953C6FA60005B2765F99DBBC965C8E9",
+        signature_key: str  = "DFA5ED192DDA6E88A12FE12130DC6206B1251E44"
+        ) -> None:
         self.loop:              asyncio.AbstractEventLoop = asyncio.get_event_loop()
         self._cooldown_message  = None
         self._debug:            bool = check_debugger()
         self._intents:          bool = intents
         self._is_ready:         bool = False
         self._userId:           str = None
         self._sid:              str = None
@@ -30,29 +34,35 @@
         self.cache:             Cache = Cache("cache")
 
         self.command_prefix:    Optional[str] = command_prefix
         if self.command_prefix == "":
             raise InvalidCommandPrefix()
 
         self.community_id:      Union[str, int] = community_id
+        self.generate:          Generator = Generator(
+                                prefix=hash_prefix,
+                                device_key=device_key,
+                                signature_key=signature_key
+                                )
         self.online_status:     bool = online_status
-        self.device_id:         Optional[str] = device_id or generate_device_id()
+        self.device_id:         Optional[str] = device_id or self.generate.device_id()
         self.request:           AsyncRequestHandler = AsyncRequestHandler(
                                 bot = self,
                                 loop = self.loop,
-                                proxy=proxy
+                                proxy=proxy,
+                                generator=self.generate
                                 )
         self.community:         AsyncCommunity = AsyncCommunity(
                                 bot = self,
                                 session=self.request,
                                 community_id=self.community_id
                                 )
         if self.community_id:   self.set_community_id(community_id)
 
-        AsyncWSClient.__init__(self)
+        super().__init__()
 
     @property
     def debug(self) -> bool:
         return self._debug
 
     @debug.setter
     def debug(self, value: bool) -> None:
```

### Comparing `pymino-1.2.3.8/pymino/async_client.py` & `pymino-1.2.3.9/pymino/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import asyncio
 from time import time
 from typing import Any, Callable, Optional, TypeVar, Union
 
 from .ext.entities import *
 from .ext.async_global_client import AsyncGlobal
+from .ext.utilities.generate import Generator
 from .ext import AsyncRequestHandler, AsyncAccount, AsyncCommunity
-from .ext.utilities.generate import device_id as generate_device_id
 
 
 F = TypeVar("F", bound=Callable[..., Any])
 
 class AsyncClient(AsyncGlobal):
     """
     `Client` - This is the main client.
 
     `**Parameters**``
     - `**kwargs` - any other parameters to use for the client.
-
     - `device_id` - device id to use for the client.
-
     - `proxy` - proxy string to use for the client.
+    - `hash_prefix` - The hash prefix to use for the bot. `Defaults` to `19`.
+    - `device_key` - The device key to use for the bot. `Defaults` to `E7309ECC0953C6FA60005B2765F99DBBC965C8E9`.
+    - `signature_key` - The signature key to use for the bot. `Defaults` to `DFA5ED192DDA6E88A12FE12130DC6206B1251E44`.
+    
     
     ----------------------------
     Why use `Client` over `Bot`?
 
     - Used for scripts rather than bots.
     - Lightweight, does not utilize websocket.
 
@@ -109,28 +111,41 @@
         chatId = "000000-0000-0000-0000-000000",
         content = "Hello, world!",
         comId = comId
     )
     ```
 
     """
-    def __init__(self, **kwargs):
+    def __init__(
+        self,
+        community_id: Optional[Union[str, int]] = None,
+        hash_prefix: Union[str, int] = 19,
+        device_key: str = "E7309ECC0953C6FA60005B2765F99DBBC965C8E9",
+        signature_key: str  = "DFA5ED192DDA6E88A12FE12130DC6206B1251E44",
+        **kwargs
+        ) -> None:
         self._debug:            bool = check_debugger()
         self.loop:              asyncio.AbstractEventLoop = asyncio.get_event_loop()
         self._is_authenticated: bool = False
         self._userId:           str = None
         self._sid:              str = None
         self._cached:           bool = False
         self.cache:             Cache = Cache("cache")
-        self.community_id:      Optional[str] = kwargs.get("comId", kwargs.get("community_id"))
-        self.device_id:         Optional[str] = kwargs.get("device_id") or generate_device_id()
+        self.community_id:      Optional[str] = community_id or kwargs.get("comId")
+        self.generate:          Generator = Generator(
+                                prefix=hash_prefix,
+                                device_key=device_key,
+                                signature_key=signature_key
+                                )
+        self.device_id:         Optional[str] = kwargs.get("device_id") or self.generate.device_id()
         self.request:           AsyncRequestHandler = AsyncRequestHandler(
                                 bot=self,
                                 loop = self.loop,
-                                proxy = kwargs.get("proxy")
+                                proxy = kwargs.get("proxy"),
+                                generator=self.generate
                                 )
         self.account:           AsyncAccount = AsyncAccount(
                                 session=self.request
                                 )
         self.community:         AsyncCommunity = AsyncCommunity(
                                 bot=self,
                                 session=self.request,
@@ -802,15 +817,15 @@
 
         This method fetches the user profile of the authenticated user. The method calls the `fetch_profile` method of the
         `account` object to get the profile information. The result is a `UserProfile` object that contains the user's profile
         information.
 
         The method returns the `UserProfile` object.
         """
-        return await self.account.fetch_profile()
+        return await self.account.fetch_profile(self.userId)
 
 
     @authenticated
     async def set_amino_id(self, aminoId: str) -> ApiResponse:
         """
         Sets the Amino ID of the authenticated user.
```

### Comparing `pymino-1.2.3.8/pymino/bot.py` & `pymino-1.2.3.9/pymino/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,225 +4,231 @@
 
 from .ext.console import *
 from .ext.entities import *
 from .ext.socket import WSClient
 from .ext.global_client import Global
 from .ext.account import Account
 from .ext.community import Community
+from .ext.utilities.generate import Generator
 from .ext.utilities.request_handler import RequestHandler
-from .ext.utilities.generate import device_id as generate_device_id
 
-class Bot(WSClient, Global):
-    """
-    `Bot` - This is the main client.
 
-    `**Parameters**``
-    - `command_prefix` - The prefix to use for commands. `Defaults` to `!`.
-    - `community_id` - The community id to use for the bot. `Defaults` to `None`.
-    - `console_enabled` - Whether to enable the console. `Defaults` to `True`.
-    - `device_id` - The device id to use for the bot. `Defaults` to `None`.
-    - `intents` - Avoids receiving events that you do not need. `Defaults` to `False`.
-    - `online_status` - Whether to set the bot's online status to `online`. `Defaults` to `True`.
-    - `proxy` - The proxy to use for the bot. `Defaults` to `None`.
-
-    ----------------------------
-    When should I use `Bot` instead of `Client`?
-
-    - If you want to create a bot that responds to commands or events.
-    - `Client` does not respond to commands or events.
-
-    ----------------------------
-
-    How do I login to my bot account?
-
-    - You can login to your bot account by using the `run` method.
-
-    ----------------------------
-
-    How do I use the `run` method?
-    
-    - It's simple! Just use the `run` method like this:
-
-        ```py
-        bot = Bot()
-        #NOTE: Keep in mind bot.run() should be the last line of your code.
-        bot.run(email="email", password="password")
-        ```
-
-    ----------------------------
-    How do I login to my bot account with a proxy?
-
-    - It's as easy as adding a `proxy` parameter to the `bot` class.
-
-        ```py
-        bot = Bot(proxy="http://username:password@ip:port")
-
-        bot.run(email="email", password="password")
-        ```
-    ----------------------------
-    How do I know if my bot is ready?
-
-    - You can check if your bot is ready by using the `is_ready` attribute.
-    - `is_ready` is a `bool` that is `True` if the bot is ready and `False` if the bot is not ready.
-    - Alternatively, you can use the `on_ready` event.
-    - `on_ready` is an event that is called when the bot is ready.
-
-    ----------------------------
-    How do I use the `on_ready` event?
-
-    - You can use the `ready` event like this:
-
-        ```py
-        bot = Bot()
-
-        @bot.on("on_ready")
-        def on_ready():
-            print(f"Logged in as {bot.profile.username}(bot.profile.userId)")
-
-        bot.run(email="email", password="password")
-        ```
-    ----------------------------
-    How do I use the is_ready attribute?
-
-    - You can use the `is_ready` attribute like this:
-
-        ```py
-        bot = Bot()
-
-        bot.run(email="email", password="password")
-
-        if bot.is_ready:
-            print(f"Logged in as {bot.profile.username}(bot.profile.userId)")
-
-        ```
-    ----------------------------
-    How do I set the community id for my bot?
-
-    - If you know the community id, you can use the `set_community_id` method to set the community id for your bot.
-    - Alternatively, if you do not know the community id, you can use the `fetch_community_id` method to get the community id from the community's link.
-
-    ----------------------------
-    How do I use the `set_community_id` method?
-
-    - You can use the `set_community_id` method like this:
-
-        ```py
-        bot = Bot()
-
-        bot.run(email="email", password="password")
-        bot.set_community_id(community_id=123456789)
-        ```
-    ----------------------------
-    How do I use the `fetch_community_id` method?
-
-    - You can use the `fetch_community_id` method like this:
-
-        ```py
-        bot = Bot()
-
-        bot.run(email="email", password="password")
-        bot.fetch_community_id(community_link="https://aminoapps.com/c/OnePiece")
-        ```
-    ----------------------------
-    Ok, I'm ready to make my first bot! What do I do now?
-    - You can start by making a `command`.
-    - They are functions that are called when a user sends a message that starts with the `command_prefix`.
-    - You can make a command like this:
-
-        ```py
-        from pymino import Bot
-        from pymino.ext import *
-
-        bot = Bot()
-
-        @bot.command(command_name="ping")
-        def ping_command(ctx: Context):
-            ctx.send("Pong!")
-
-        bot.run(email="email", password="password")
-        ```
-    ----------------------------
-    What is my command prefix?
-    - Your command prefix by default is `!`.
-    - You can change your command prefix by using the `command_prefix` parameter in the `Bot` class.
-    - You can change your command prefix like this:
-
-        ```py
-        bot = Bot(command_prefix=".")
-        # Now your command prefix is "." instead of "!".
-        ```
-    ----------------------------
-    Can I use multiple names for my command?
-    - Yes! You can use multiple names for your command by using the `aliases` parameter in the `command` decorator.
-    - You can use multiple names for your command like this:
-
-        ```py
-        from pymino import Bot
-        from pymino.ext import *
-
-        bot = Bot()
-        #NOTE: This will register the command as "ping", "p", and "pong".
-        # Meaning the command will be called if the message starts with "!ping", "!p", or "!pong".
-        @bot.command(command_name="ping", aliases=["p", "pong"])
-        def ping_command(ctx: Context):
-            ctx.send("Pong!")
-
-        bot.run(email="email", password="password")
-        ```
-    ----------------------------
-    How about cooldowns? Can I use them?
-    - Yes! You can use cooldowns for your commands by using the `cooldown` parameter in the `command` decorator.
-    - You can use cooldowns like this:
-
-        ```py
-        from pymino import Bot
-        from pymino.ext import *
-
-        bot = Bot()
-        #NOTE: This will set the cooldown for the command to 5 seconds.
-        # The cooldown is user based, meaning that each user will have their own cooldown.
-        @bot.command(command_name="ping", cooldown=5)
-        def ping_command(ctx: Context):
-            ctx.send("Pong!")
-
-        bot.run(email="email", password="password")
-        ```
-    ----------------------------
-    Is there a help command built in?
-    - Yes! There is a built in help command that you can use.
-    - It will return a list of all the commands that the bot has and their descriptions.
-    
-    How do I set the description for my command?
-    - You can set the description for your command by using the `command_description` parameter in the `command` decorator.
-    - You can set the description for your command like this:
-
-        ```py
-        from pymino import Bot
-        from pymino.ext import *
-
-        bot = Bot()
-        # This way when the user uses the help command, it will return the description for the command.
-        @bot.command(command_name="ping", command_description="This command will return pong.")
-        def ping_command(ctx: Context):
-            ctx.send("Pong!")
-
-        bot.run(email="email", password="password")
-        ```
-    """
+class Bot(WSClient, Global):
     def __init__(
         self,
         command_prefix: Optional[str] = "!",
         community_id: Union[str, int] = None,
         console_enabled: bool = False,
         device_id: str = None,
         intents: bool = False,
         online_status: bool = False,
-        proxy: str = None
-        ):
+        proxy: str = None,
+        hash_prefix: Union[str, int] = 19,
+        device_key: str = "E7309ECC0953C6FA60005B2765F99DBBC965C8E9",
+        signature_key: str  = "DFA5ED192DDA6E88A12FE12130DC6206B1251E44"
+        ) -> None:
+        """
+        `Bot` - This is the main client.
+
+        `**Parameters**``
+        - `command_prefix` - The prefix to use for commands. `Defaults` to `!`.
+        - `community_id` - The community id to use for the bot. `Defaults` to `None`.
+        - `console_enabled` - Whether to enable the console. `Defaults` to `True`.
+        - `device_id` - The device id to use for the bot. `Defaults` to `None`.
+        - `intents` - Avoids receiving events that you do not need. `Defaults` to `False`.
+        - `online_status` - Whether to set the bot's online status to `online`. `Defaults` to `True`.
+        - `proxy` - The proxy to use for the bot. `Defaults` to `None`.
+        - `hash_prefix` - The hash prefix to use for the bot. `Defaults` to `19`.
+        - `device_key` - The device key to use for the bot. `Defaults` to `E7309ECC0953C6FA60005B2765F99DBBC965C8E9`.
+        - `signature_key` - The signature key to use for the bot. `Defaults` to `DFA5ED192DDA6E88A12FE12130DC6206B1251E44`.
+
+        ----------------------------
+        When should I use `Bot` instead of `Client`?
+
+        - If you want to create a bot that responds to commands or events.
+        - `Client` does not respond to commands or events.
+
+        ----------------------------
+
+        How do I login to my bot account?
+
+        - You can login to your bot account by using the `run` method.
+
+        ----------------------------
+
+        How do I use the `run` method?
+        
+        - It's simple! Just use the `run` method like this:
+
+            ```py
+            bot = Bot()
+            #NOTE: Keep in mind bot.run() should be the last line of your code.
+            bot.run(email="email", password="password")
+            ```
+
+        ----------------------------
+        How do I login to my bot account with a proxy?
+
+        - It's as easy as adding a `proxy` parameter to the `bot` class.
+
+            ```py
+            bot = Bot(proxy="http://username:password@ip:port")
+
+            bot.run(email="email", password="password")
+            ```
+        ----------------------------
+        How do I know if my bot is ready?
+
+        - You can check if your bot is ready by using the `is_ready` attribute.
+        - `is_ready` is a `bool` that is `True` if the bot is ready and `False` if the bot is not ready.
+        - Alternatively, you can use the `on_ready` event.
+        - `on_ready` is an event that is called when the bot is ready.
+
+        ----------------------------
+        How do I use the `on_ready` event?
+
+        - You can use the `ready` event like this:
+
+            ```py
+            bot = Bot()
+
+            @bot.on("on_ready")
+            def on_ready():
+                print(f"Logged in as {bot.profile.username}(bot.profile.userId)")
+
+            bot.run(email="email", password="password")
+            ```
+        ----------------------------
+        How do I use the is_ready attribute?
+
+        - You can use the `is_ready` attribute like this:
+
+            ```py
+            bot = Bot()
+
+            bot.run(email="email", password="password")
+
+            if bot.is_ready:
+                print(f"Logged in as {bot.profile.username}(bot.profile.userId)")
+
+            ```
+        ----------------------------
+        How do I set the community id for my bot?
+
+        - If you know the community id, you can use the `set_community_id` method to set the community id for your bot.
+        - Alternatively, if you do not know the community id, you can use the `fetch_community_id` method to get the community id from the community's link.
+
+        ----------------------------
+        How do I use the `set_community_id` method?
+
+        - You can use the `set_community_id` method like this:
+
+            ```py
+            bot = Bot()
+
+            bot.run(email="email", password="password")
+            bot.set_community_id(community_id=123456789)
+            ```
+        ----------------------------
+        How do I use the `fetch_community_id` method?
+
+        - You can use the `fetch_community_id` method like this:
+
+            ```py
+            bot = Bot()
+
+            bot.run(email="email", password="password")
+            bot.fetch_community_id(community_link="https://aminoapps.com/c/OnePiece")
+            ```
+        ----------------------------
+        Ok, I'm ready to make my first bot! What do I do now?
+        - You can start by making a `command`.
+        - They are functions that are called when a user sends a message that starts with the `command_prefix`.
+        - You can make a command like this:
+
+            ```py
+            from pymino import Bot
+            from pymino.ext import *
+
+            bot = Bot()
+
+            @bot.command(command_name="ping")
+            def ping_command(ctx: Context):
+                ctx.send("Pong!")
+
+            bot.run(email="email", password="password")
+            ```
+        ----------------------------
+        What is my command prefix?
+        - Your command prefix by default is `!`.
+        - You can change your command prefix by using the `command_prefix` parameter in the `Bot` class.
+        - You can change your command prefix like this:
+
+            ```py
+            bot = Bot(command_prefix=".")
+            # Now your command prefix is "." instead of "!".
+            ```
+        ----------------------------
+        Can I use multiple names for my command?
+        - Yes! You can use multiple names for your command by using the `aliases` parameter in the `command` decorator.
+        - You can use multiple names for your command like this:
+
+            ```py
+            from pymino import Bot
+            from pymino.ext import *
+
+            bot = Bot()
+            #NOTE: This will register the command as "ping", "p", and "pong".
+            # Meaning the command will be called if the message starts with "!ping", "!p", or "!pong".
+            @bot.command(command_name="ping", aliases=["p", "pong"])
+            def ping_command(ctx: Context):
+                ctx.send("Pong!")
+
+            bot.run(email="email", password="password")
+            ```
+        ----------------------------
+        How about cooldowns? Can I use them?
+        - Yes! You can use cooldowns for your commands by using the `cooldown` parameter in the `command` decorator.
+        - You can use cooldowns like this:
+
+            ```py
+            from pymino import Bot
+            from pymino.ext import *
+
+            bot = Bot()
+            #NOTE: This will set the cooldown for the command to 5 seconds.
+            # The cooldown is user based, meaning that each user will have their own cooldown.
+            @bot.command(command_name="ping", cooldown=5)
+            def ping_command(ctx: Context):
+                ctx.send("Pong!")
+
+            bot.run(email="email", password="password")
+            ```
+        ----------------------------
+        Is there a help command built in?
+        - Yes! There is a built in help command that you can use.
+        - It will return a list of all the commands that the bot has and their descriptions.
         
+        How do I set the description for my command?
+        - You can set the description for your command by using the `command_description` parameter in the `command` decorator.
+        - You can set the description for your command like this:
+
+            ```py
+            from pymino import Bot
+            from pymino.ext import *
+
+            bot = Bot()
+            # This way when the user uses the help command, it will return the description for the command.
+            @bot.command(command_name="ping", command_description="This command will return pong.")
+            def ping_command(ctx: Context):
+                ctx.send("Pong!")
+
+            bot.run(email="email", password="password")
+            ```
+        """
         self._debug:            bool = check_debugger()
         self._console_enabled:  bool = console_enabled
         self._cooldown_message  = None
         self._intents:          bool = intents
         self._is_ready:         bool = False
         self._userId:           str = None
         self._sid:              str = None
@@ -230,19 +236,21 @@
         self.cache:             Cache = Cache("cache")
 
         self.command_prefix:    Optional[str] = command_prefix
         if self.command_prefix == "":
             raise InvalidCommandPrefix()
         
         self.community_id:      Union[str, int] = community_id
+        self.generate           = Generator(hash_prefix, device_key, signature_key)
         self.online_status:     bool = online_status
-        self.device_id:         Optional[str] = device_id or generate_device_id()
+        self.device_id:         Optional[str] = device_id or self.generate.device_id()
         self.request:           RequestHandler = RequestHandler(
                                 bot = self,
-                                proxy=proxy
+                                proxy=proxy,
+                                generator=self.generate
                                 )
         self.community:         Community = Community(
                                 bot = self,
                                 session=self.request,
                                 community_id=self.community_id
                                 )
         self.account:           Account = Account(
```

### Comparing `pymino-1.2.3.8/pymino/client.py` & `pymino-1.2.3.9/pymino/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from time import time
 from typing import Any, Callable, Optional, TypeVar, Union
 
 from .ext.entities import *
 from .ext.global_client import Global
+from .ext.utilities.generate import Generator
 from .ext import RequestHandler, Account, Community
-from .ext.utilities.generate import device_id as generate_device_id
 
 
 F = TypeVar("F", bound=Callable[..., Any])
 
 class Client(Global):
     """
     `Client` - This is the main client.
 
     `**Parameters**``
     - `**kwargs` - any other parameters to use for the client.
-
     - `device_id` - device id to use for the client.
-
     - `proxy` - proxy string to use for the client.
+    - `hash_prefix` - The hash prefix to use for the bot. `Defaults` to `19`.
+    - `device_key` - The device key to use for the bot. `Defaults` to `E7309ECC0953C6FA60005B2765F99DBBC965C8E9`.
+    - `signature_key` - The signature key to use for the bot. `Defaults` to `DFA5ED192DDA6E88A12FE12130DC6206B1251E44`.
     
     ----------------------------
     Why use `Client` over `Bot`?
 
     - Used for scripts rather than bots.
     - Lightweight, does not utilize websocket.
 
@@ -108,26 +109,39 @@
         chatId = "000000-0000-0000-0000-000000",
         content = "Hello, world!",
         comId = comId
     )
     ```
 
     """
-    def __init__(self, **kwargs):
+    def __init__(
+        self,
+        community_id: Optional[Union[str, int]] = None,
+        hash_prefix: Union[str, int] = 19,
+        device_key: str = "E7309ECC0953C6FA60005B2765F99DBBC965C8E9",
+        signature_key: str  = "DFA5ED192DDA6E88A12FE12130DC6206B1251E44",
+        **kwargs
+        ) -> None:
         self._debug:            bool = check_debugger()
         self._is_authenticated: bool = False
         self._userId:           str = None
         self._sid:              str = None
         self._cached:           bool = False
         self.cache:             Cache = Cache("cache")
-        self.community_id:      Optional[str] = kwargs.get("comId", kwargs.get("community_id"))
-        self.device_id:         Optional[str] = kwargs.get("device_id") or generate_device_id()
+        self.community_id:      Optional[str] = community_id or kwargs.get("comId")
+        self.generate:          Generator = Generator(
+                                prefix=hash_prefix,
+                                device_key=device_key,
+                                signature_key=signature_key
+                                )
+        self.device_id:         Optional[str] = kwargs.get("device_id") or self.generate.device_id()
         self.request:           RequestHandler = RequestHandler(
                                 self,
-                                proxy=kwargs.get("proxy")
+                                proxy=kwargs.get("proxy"),
+                                generator=self.generate
                                 )
         self.account:           Account = Account(
                                 session=self.request
                                 )
         self.community:         Community = Community(
                                 bot=self,
                                 session=self.request,
@@ -799,15 +813,15 @@
 
         This method fetches the user profile of the authenticated user. The method calls the `fetch_profile` method of the
         `account` object to get the profile information. The result is a `UserProfile` object that contains the user's profile
         information.
 
         The method returns the `UserProfile` object.
         """
-        return self.account.fetch_profile()
+        return self.account.fetch_profile(self.userId)
 
 
     @authenticated
     def set_amino_id(self, aminoId: str) -> ApiResponse:
         """
         Sets the Amino ID of the authenticated user.
```

### Comparing `pymino-1.2.3.8/pymino/ext/__init__.py` & `pymino-1.2.3.9/pymino/ext/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 from .global_client import *
 from .community import *
 from .async_community import *
 from .dispatcher import *
 from .handle_queue import *
 from .async_account import *
 from .async_event_handler import *
-from .async_community import AsyncCommunity
+from .async_community import *
 from .utilities.request_handler import *
 from .utilities.async_request_handler import *
```

### Comparing `pymino-1.2.3.8/pymino/ext/account.py` & `pymino-1.2.3.9/pymino/ext/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from time import time
 
-from .utilities.generate import device_id
+from .utilities.generate import Generator
 from .entities.userprofile import UserProfile
 from .entities.general import (
     ApiResponse, Authenticate, ResetPassword, Wallet
     )
 
 class Account:
     """
@@ -40,15 +40,15 @@
         ```
         """
         return Authenticate(self.session.handler(
             method = "POST",
             url="/g/s/auth/register",
             data={
                 "secret": f"0 {password}",
-                "deviceID": device_id(),
+                "deviceID": self.session.generate.device_id(),
                 "email": email,
                 "clientType": 100,
                 "nickname": username,
                 "validationContext": {
                     "data": {"code": verificationCode}, "type": 1, "identity": email},
                 "type": 1,
                 "identity": email,
@@ -76,15 +76,15 @@
         print(response)
         ```"""
         return ApiResponse(self.session.handler(
             method = "POST",
             url="/g/s/account/delete-request",
             data={
                 "secret": f"0 {password}",
-                "deviceID": device_id(),
+                "deviceID": self.session.generate.device_id(),
                 "email": email,
                 "timestamp": int(time() * 1000)
             }))
 
     def delete_request_cancel(self, email: str, password: str) -> ApiResponse:
         """
         `**delete_request_cancel**` - Cancels the delete request.
@@ -107,15 +107,15 @@
         ```
         """
         return ApiResponse(self.session.handler(
             method = "POST",
             url="/g/s/account/delete-request/cancel",
             data={
                 "secret": f"0 {password}",
-                "deviceID": device_id(),
+                "deviceID": self.session.generate.device_id(),
                 "email": email,
                 "timestamp": int(time() * 1000)
             }))
 
     def check_device(self, deviceId: str) -> ApiResponse:
         """
         `**check_device**` - Checks if the device is valid.
@@ -180,15 +180,15 @@
         response = bot.upload_image(image="image.jpg")
         print(response)
         ```
         """
         return ApiResponse(self.session.handler(method="POST", url="/g/s/media/upload",
             data=open(image, "rb").read(), content_type="image/jpg")).mediaValue
 
-    def fetch_profile(self) -> UserProfile:
+    def fetch_profile(self, userId: str) -> UserProfile:
         """
         `**fetch_profile**` - Fetches the profile information.
         
         `**Example**`
         
         ```py
         from pymino import *
@@ -196,15 +196,15 @@
         bot = Bot()
         bot.run(email=email, password=password)
         response = bot.fetch_profile()
         print(response)
         ```
         """
         return UserProfile(self.session.handler(
-            method = "GET", url = f"/g/s/user-profile/{self.userId}"))
+            method = "GET", url = f"/g/s/user-profile/{userId}"))
 
     def set_amino_id(self, aminoId: str) -> ApiResponse:
         """
         `**set_amino_id**` - Sets the amino id.
 
         `**Parameters**`
 
@@ -263,15 +263,15 @@
         ```
         """
         return ApiResponse(self.session.handler(
             method = "POST", url="/g/s/auth/request-security-validation",
             data={
                 "identity": email,
                 "type": 1,
-                "deviceID": device_id(),
+                "deviceID": self.session.generate.device_id(),
                 "level": 2 if resetPassword else None,
                 "purpose": "reset-password" if resetPassword else None,
                 "timestamp": int(time() * 1000)
             }))
 
     def activate_email(self, email: str, code: str) -> ApiResponse:
         """
@@ -296,15 +296,15 @@
         return ApiResponse(self.session.handler(
             method = "POST",
             url="/g/s/auth/activate-email",
             data={
                 "type": 1,
                 "identity": email,
                 "data": {"code":code},
-                "deviceID": device_id(),
+                "deviceID": self.session.generate.device_id(),
                 "timestamp": int(time() * 1000)
             }))
     
     
     def verify(self, email: str, code: str, deviceId: str) -> ApiResponse:
         """
         `**verify**` - Verifies the code sent to the email.
@@ -334,15 +334,15 @@
                 "type": 1,
                 "identity": email,
                 "data": {"code":code},
                 "deviceID": deviceId,
                 "timestamp": int(time() * 1000)
             }))
 
-    def reset_password(self, email: str, newPassword: str, code: str, deviceId: str = device_id()) -> ResetPassword:
+    def reset_password(self, email: str, newPassword: str, code: str, deviceId: str) -> ResetPassword:
         """
         `**reset_password**` - Resets the password.
 
         `**Parameters**`
 
         - `email` - The email of the account.
```

### Comparing `pymino-1.2.3.8/pymino/ext/async_account.py` & `pymino-1.2.3.9/pymino/ext/async_account.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from time import time
 
-from .utilities.generate import device_id
 from .entities.userprofile import UserProfile
 from .entities.general import (
     ApiResponse, Authenticate, ResetPassword, Wallet
     )
 
+
 class AsyncAccount:
     """
     Account class for handling account related requests.
     """
     def __init__(self, session):
         self.session = session
 
-
     async def register(self, email: str, password: str, username: str, verificationCode: str) -> Authenticate:
         """
         `**register**` - Registers a new account.
 
         `**Parameters**`
 
         - `email` - The email of the account.
@@ -41,26 +40,25 @@
         ```
         """
         return Authenticate(await self.session.handler(
             method = "POST",
             url="/g/s/auth/register",
             data={
                 "secret": f"0 {password}",
-                "deviceID": device_id(),
+                "deviceID": self.session.generate.device_id(),
                 "email": email,
                 "clientType": 100,
                 "nickname": username,
                 "validationContext": {
                     "data": {"code": verificationCode}, "type": 1, "identity": email},
                 "type": 1,
                 "identity": email,
                 "timestamp": int(time() * 1000)
                 }))
 
-
     async def delete_request(self, email: str, password: str) -> ApiResponse:
         """
         `**delete_request**` - Sends a delete request to the account.
 
         `**Parameters**`
 
         - `email` - The email of the account.
@@ -78,20 +76,19 @@
         print(response)
         ```"""
         return ApiResponse(await self.session.handler(
             method = "POST",
             url="/g/s/account/delete-request",
             data={
                 "secret": f"0 {password}",
-                "deviceID": device_id(),
+                "deviceID": self.session.generate.device_id(),
                 "email": email,
                 "timestamp": int(time() * 1000)
             }))
 
-
     async def delete_request_cancel(self, email: str, password: str) -> ApiResponse:
         """
         `**delete_request_cancel**` - Cancels the delete request.
 
         `**Parameters**`
 
         - `email` - The email of the account.
@@ -110,20 +107,19 @@
         ```
         """
         return ApiResponse(await self.session.handler(
             method = "POST",
             url="/g/s/account/delete-request/cancel",
             data={
                 "secret": f"0 {password}",
-                "deviceID": device_id(),
+                "deviceID": self.session.generate.device_id(),
                 "email": email,
                 "timestamp": int(time() * 1000)
             }))
 
-
     async def check_device(self, deviceId: str) -> ApiResponse:
         """
         `**check_device**` - Checks if the device is valid.
 
         `**Parameters**`
 
         - `deviceId` - The device id of the account.
@@ -145,15 +141,14 @@
                 "deviceID": deviceId,
                 "clientType": 100,
                 "timezone": -310,
                 "systemPushEnabled": True,
                 "timestamp": int(time() * 1000)
                 }))
 
-
     async def fetch_account(self) -> ApiResponse:
         """
         `**fetch_account**` - Fetches the account information.
         
         `**Example**`
         
         ```py
@@ -163,15 +158,14 @@
         bot.run(email=email, password=password)
         response = bot.fetch_account()
         print(response)
         ```
         """
         return ApiResponse(await self.session.handler(method = "GET", url="/g/s/account"))
 
-
     async def upload_image(self, image: str) -> str:
         """
         `**upload_image**` - Uploads an image to the server.
 
         `**Parameters**`
 
         - `image` - The image to upload.
@@ -190,16 +184,15 @@
         return ApiResponse(await self.session.handler(
             method="POST",
             url="/g/s/media/upload",
             data=open(image, "rb").read(),
             content_type="image/jpg"
             )).mediaValue
 
-
-    async def fetch_profile(self) -> UserProfile:
+    async def fetch_profile(self, userId: str) -> UserProfile:
         """
         `**fetch_profile**` - Fetches the profile information.
         
         `**Example**`
         
         ```py
         from pymino import *
@@ -208,18 +201,17 @@
         bot.run(email=email, password=password)
         response = bot.fetch_profile()
         print(response)
         ```
         """
         return UserProfile(await self.session.handler(
             method = "GET",
-            url = f"/g/s/user-profile/{self.userId}"
+            url = f"/g/s/user-profile/{userId}"
             ))
 
-
     async def set_amino_id(self, aminoId: str) -> ApiResponse:
         """
         `**set_amino_id**` - Sets the amino id.
 
         `**Parameters**`
 
         - `aminoId` - The amino id to set.
@@ -237,15 +229,14 @@
         """
         return ApiResponse(await self.session.handler(
             method="POST",
             url="/g/s/account/change-amino-id",
             data={"aminoId": aminoId, "timestamp": int(time() * 1000)}
             ))
 
-
     async def fetch_wallet(self) -> Wallet:
         """
         `**fetch_wallet**` - Fetches the wallet information.
         
         `**Example**`
         
         ```py
@@ -254,15 +245,14 @@
         bot = Bot()
         bot.run(email=email, password=password)
         response = bot.fetch_wallet()
         print(response)
         """
         return Wallet(await self.session.handler(method="GET", url="/g/s/wallet"))
 
-
     async def request_security_validation(self, email: str, resetPassword: bool = False) -> ApiResponse:
         """
         `**request_security_validation**` - Requests a security validation.
 
         `**Parameters**`
 
         - `email` - The email of the account.
@@ -281,21 +271,20 @@
         """
         return ApiResponse(await self.session.handler(
             method = "POST",
             url="/g/s/auth/request-security-validation",
             data={
                 "identity": email,
                 "type": 1,
-                "deviceID": device_id(),
+                "deviceID": self.session.generate.device_id(),
                 "level": 2 if resetPassword else None,
                 "purpose": "reset-password" if resetPassword else None,
                 "timestamp": int(time() * 1000)
             }))
 
-
     async def activate_email(self, email: str, code: str) -> ApiResponse:
         """
         `**activate_email**` - Activates an email.
 
         `**Parameters**`
 
         - `email` - The email of the account.
@@ -315,19 +304,18 @@
         return ApiResponse(await self.session.handler(
             method = "POST",
             url="/g/s/auth/activate-email",
             data={
                 "type": 1,
                 "identity": email,
                 "data": {"code":code},
-                "deviceID": device_id(),
+                "deviceID": self.session.generate.device_id(),
                 "timestamp": int(time() * 1000)
             }))
 
-    
     async def verify(self, email: str, code: str, deviceId: str) -> ApiResponse:
         """
         `**verify**` - Verifies the code sent to the email.
 
         `**Parameters**`
         
         - `email` - The email of the account.
@@ -353,16 +341,15 @@
                 "type": 1,
                 "identity": email,
                 "data": {"code":code},
                 "deviceID": deviceId,
                 "timestamp": int(time() * 1000)
             }))
 
-
-    async def reset_password(self, email: str, newPassword: str, code: str, deviceId: str = device_id()) -> ResetPassword:
+    async def reset_password(self, email: str, newPassword: str, code: str, deviceId: str) -> ResetPassword:
         """
         `**reset_password**` - Resets the password.
 
         `**Parameters**`
 
         - `email` - The email of the account.
```

### Comparing `pymino-1.2.3.8/pymino/ext/async_community.py` & `pymino-1.2.3.9/pymino/ext/async_community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/async_context.py` & `pymino-1.2.3.9/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/async_event_handler.py` & `pymino-1.2.3.9/pymino/ext/async_event_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/async_global_client.py` & `pymino-1.2.3.9/pymino/ext/async_global_client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/async_socket.py` & `pymino-1.2.3.9/pymino/ext/async_socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from ujson import loads, JSONDecodeError
 from contextlib import asynccontextmanager
 
 from .entities import *
 from .handle_queue import QueueHandler
 from .async_event_handler import AsyncEventHandler
 from .dispatcher import AsyncMessageDispatcher
-from .utilities.generate import device_id, generate_signature
 
 if orjson_exists():
     from orjson import loads as orjson_loads
 
 
 @asynccontextmanager
 async def create_client_session():
@@ -112,21 +111,21 @@
         if self.session:
             await self.session.close()
             del self.session
 
         try:
             async with create_client_session() as session:
                 self.session = session
-                ws_data = f"{device_id()}|{int(time() * 1000)}"
+                ws_data = f"{self.generate.device_id()}|{int(time() * 1000)}"
                 self.ws = await session.ws_connect(
                     url=f"{await self.fetch_ws_url()}/?{urlencode({'signbody': ws_data})}",
                     headers={
-                        "NDCDEVICEID": device_id(),
+                        "NDCDEVICEID": self.generate.device_id(),
                         "NDCAUTH": f"sid={self.sid}",
-                        "NDC-MSG-SIG": generate_signature(ws_data)
+                        "NDC-MSG-SIG": self.generate.signature(ws_data)
                     }
                 )
 
                 if not self.tasks:
                     await asyncio.gather(
                         self._ready(),
                         self.start_worker_pool(),
```

### Comparing `pymino-1.2.3.8/pymino/ext/community.py` & `pymino-1.2.3.9/pymino/ext/community.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,20 +499,20 @@
 
         **Example usage:**
 
         >>> invitation_id = client.fetch_invitationId(invite_code="ABCD1234")
         >>> print(invitation_id)
         """
         if "inviteCode" in kwargs: #TODO: Remove this in the near future.
-            inviteCode = kwargs["inviteCode"]
+            invite_code = kwargs["inviteCode"]
             print("The 'inviteCode' parameter has been deprecated. Please use 'invite_code' instead.")
 
         return InvitationId(self.session.handler(
             method = "GET",
-            url = f"/g/s/community/link-identify?q={inviteCode}"
+            url = f"/g/s/community/link-identify?q={invite_code}"
             )).invitationId
 
 
     @community
     def join_community_by_code(self, invite_code: str, comId: Union[str, int] = None, **kwargs) -> ApiResponse:
         """
         Joins a community using the invite code.
```

### Comparing `pymino-1.2.3.8/pymino/ext/console.py` & `pymino-1.2.3.9/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/context.py` & `pymino-1.2.3.9/pymino/ext/context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/dispatcher.py` & `pymino-1.2.3.9/pymino/ext/dispatcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 from typing import Callable
 from threading import Thread
+from contextlib import contextmanager
+
+
+@contextmanager
+def thread_executor(handler: Callable, message: dict):
+    thread = Thread(target=handler, args=(message,))
+    thread.start()
+    yield
+    thread.join()
 
 class MessageDispatcher:
     """
     `MessageDispatcher` - Simple message dispatcher that allows you to register handlers for specific message types.
  
     `**Example**`
 
@@ -26,17 +35,16 @@
     def register(self, message_type: int, handler: Callable):
         self.dispatch_table[message_type] = handler
 
     def handle(self, message: dict):
         message_type = message.get("t")
         if message_type not in self.dispatch_table:
             return None
-        return Thread(
-            target=self.dispatch_table[message_type],args=(message,)
-            ).start()
+        with thread_executor(self.dispatch_table[message_type], message):
+            pass
 
 
 class AsyncMessageDispatcher:
     """
     `AsyncMessageDispatcher` - Simple async message dispatcher that allows you to register handlers for specific message types.
  
     `**Example**`
```

### Comparing `pymino-1.2.3.8/pymino/ext/entities/acm.py` & `pymino-1.2.3.9/pymino/ext/entities/acm.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/entities/admin_log.py` & `pymino-1.2.3.9/pymino/ext/entities/admin_log.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/entities/api_response.py` & `pymino-1.2.3.9/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/entities/bubble.py` & `pymino-1.2.3.9/pymino/ext/entities/bubble.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/entities/chat_threads.py` & `pymino-1.2.3.9/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/entities/comments.py` & `pymino-1.2.3.9/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/entities/enums.py` & `pymino-1.2.3.9/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/entities/exceptions.py` & `pymino-1.2.3.9/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/entities/general.py` & `pymino-1.2.3.9/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/entities/handlers.py` & `pymino-1.2.3.9/pymino/ext/entities/handlers.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,29 +18,54 @@
     """
     with suppress(Exception):
         return any([
             search("vscode", environ.get("TERM_PROGRAM")),
             search("pycharm", environ.get("TERM_PROGRAM")),
             is_repl(), is_android()
             ])
-    
+
+def install_wsaccel() -> None:
+    """
+    Try to install wsaccel if it isn't installed.
+    """
+    with Cache("cache") as cache:
+        if cache.get("wsaccel"):
+            return None
+
+        try:
+            from wsaccel import __version__
+            cache.set("wsaccel", True)
+            return True
+        except ImportError:
+            pipmain(["install", "wsaccel"])
+            cache.set("wsaccel", True)
+            system("cls || clear")
+            return None
+
 def orjson_exists() -> bool:
     """
     Checks if orjson is installed. If it isn't, it will install it.
     """
     if is_android(): return False
 
-    try:
-        from orjson import dumps as dumps
-        return True
-    except ImportError:
-        pipmain(["install", "orjson"])
-        system("cls || clear")
-        return True
-    
+    install_wsaccel()
+    with Cache("cache") as cache:
+        if cache.get("orjson"):
+            return True
+
+        try:
+            from orjson import dumps as dumps
+            cache.set("orjson", True)
+            return True
+        except ImportError:
+            pipmain(["install", "orjson"])
+            cache.set("orjson", True)
+            system("cls || clear")
+            return True
+
 def is_android() -> bool:
     """
     Checks if the program is running on an Android device.
     """
     return any(key in environ for key in ("ANDROID_ROOT", "ANDROID_DATA"))
 
 def is_repl() -> bool:
```

### Comparing `pymino-1.2.3.8/pymino/ext/entities/link_info.py` & `pymino-1.2.3.9/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/entities/member.py` & `pymino-1.2.3.9/pymino/ext/entities/member.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/entities/messages.py` & `pymino-1.2.3.9/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/entities/notification.py` & `pymino-1.2.3.9/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/entities/sticker.py` & `pymino-1.2.3.9/pymino/ext/entities/sticker.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/entities/threads.py` & `pymino-1.2.3.9/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/entities/userprofile.py` & `pymino-1.2.3.9/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/entities/wsevents.py` & `pymino-1.2.3.9/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/global_client.py` & `pymino-1.2.3.9/pymino/ext/global_client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/handle_queue.py` & `pymino-1.2.3.9/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/socket.py` & `pymino-1.2.3.9/pymino/ext/socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-from os import system
 from random import randint
 from typing import Optional
 from threading import Thread
 from contextlib import suppress
 from urllib.parse import urlencode
 from time import sleep as delay, time
 from ujson import loads, dumps, JSONDecodeError
 
 from .entities import *
 from .context import EventHandler
 from .dispatcher import MessageDispatcher
-from .utilities.generate import device_id, generate_signature
 
 if orjson_exists():
     from orjson import (
         loads as orjson_loads, dumps as orjson_dumps
         )
 
-
 try:
     from websocket import WebSocket, WebSocketApp
 except ImportError as e:
-    system("pip uninstall websocket -y")
-    system("pip install websocket-client==1.6.1")
+    pipmain(["uninstall", "websocket", "-y"])
+    pipmain(["install", "websocket-client==1.6.1"])
     raise WrongWebSocketPackage from e
 
 
 class WSClient(EventHandler):
     """
     `WSClient` is a class that handles the websocket.
     """
@@ -55,25 +52,25 @@
         """Connects to the websocket."""
         self.run_forever()
         return self.emit("ready")
 
 
     def run_forever(self) -> None:
         """Runs the websocket forever."""
-        ws_data = f"{device_id()}|{int(time() * 1000)}"
+        ws_data = f"{self.generate.device_id()}|{int(time() * 1000)}"
         self.ws = WebSocketApp(
             url = f"{self.fetch_ws_url()}/?{urlencode({'signbody': ws_data})}",
             on_open=self.on_websocket_open,
             on_message=self.on_websocket_message,
             on_error=self.on_websocket_error,
             on_close=self.on_websocket_close,
             header={
-            "NDCDEVICEID": device_id(),
+            "NDCDEVICEID": self.generate.device_id(),
             "NDCAUTH": f"sid={self.sid}",
-            "NDC-MSG-SIG": generate_signature(ws_data)
+            "NDC-MSG-SIG": self.generate.signature(ws_data)
             })
         return self.start_processes()
 
 
     def start_processes(self) -> None:
         """Starts the websocket processes."""
         websocket_thread = Thread(target=self.ws.run_forever)
```

### Comparing `pymino-1.2.3.8/pymino/ext/utilities/async_request_handler.py` & `pymino-1.2.3.9/pymino/ext/utilities/async_request_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from colorama import Fore, Style
 from aiohttp import ClientSession
 from asyncio import AbstractEventLoop
 
 from aiohttp.client_exceptions import *
 from typing import Optional, Union, Tuple, Callable
 
+from .generate import Generator
 from ..entities.handlers import orjson_exists
-from .generate import device_id, generate_signature
 
 from ..entities import (
     Forbidden,
     BadGateway,
     NullResponse,
     APIException,
     ServiceUnavailable
@@ -28,44 +28,49 @@
 
 class AsyncRequestHandler:
     """
     `AsyncRequestHandler` - A class that handles all requests asynchronously
 
     `**Parameters**``
     - `bot` - The main bot class.
+    - `generator` - The generator class.
+    - `loop` - The event loop to use.
     - `proxy` - The proxy to use for requests.
 
     """
-
-    def __init__(self, bot, loop: AbstractEventLoop, proxy: Optional[str] = None):
+    def __init__(
+        self,
+        bot,
+        generator: Generator,
+        loop: AbstractEventLoop,
+        proxy: Optional[str] = None
+        ) -> None:
         self.bot        = bot
+        self.generate   = generator
         self.loop:      AbstractEventLoop = loop
         self.session:   Optional[ClientSession] = None
         self.sid:       Optional[str] = None
         self.userId:    Optional[str] = None
         self.orjson:    bool = False
 
         self.proxy = proxy if proxy is not None else None
 
         self.response_map = {
             403: Forbidden,
             502: BadGateway,
             503: ServiceUnavailable
         }
 
-
     async def initialize_session(self):
         self.session = ClientSession()
 
-
     async def close_session(self):
         if self.session is not None:
             await self.session.close()
 
-
     def service_url(self, url: str) -> str:
         """
         `service_url` - Appends the endpoint to the service url
 
         `**Parameters**``
         - `url` - The endpoint to append to the service url.
 
@@ -84,15 +89,14 @@
             "HOST": "service.aminoapps.com",
             "CONNECTION": "Keep-Alive",
             "ACCEPT-ENCODING": "gzip, deflate, br",
             "NDCAUTH": f"sid={self.sid}",
             "AUID": self.userId or str(uuid4())
         }
 
-
     async def fetch_request(self, method: str) -> Callable:
         """
         `fetch_request` - Returns the request method
 
         `**Parameters**``
         - `method` - The request method to return.
 
@@ -103,15 +107,14 @@
         request_methods = {
             "GET": self.session.get,
             "POST": self.session.post,
             "DELETE": self.session.delete,
         }
         return request_methods[method]
 
-
     async def send_request(
             self,
             method: str,
             url: str,
             data: Union[dict, bytes, None],
             headers: dict,
             content_type: Optional[str]
@@ -159,15 +162,14 @@
             WSServerHandshakeError,
         ):
             return await self.handler(method, url, data, content_type)
         
         finally:
             await self.close_session()
 
-
     async def handler(
             self,
             method: str,
             url: str,
             data: Union[dict, bytes, None] = None,
             content_type: Optional[str] = None
     ) -> dict:
@@ -198,15 +200,14 @@
         except Exception as e:
             print(e)
 
         self.print_response(method=method, url=url, status_code=status_code)
 
         return await self.handle_response(status_code=status_code, response=content)
 
-
     async def service_handler(
             self,
             url: str,
             data: Union[dict, bytes, None] = None,
             content_type: Optional[str] = None
     ) -> Tuple[str, dict, Union[dict, bytes, None]]:
         """
@@ -218,22 +219,21 @@
         - `content_type` - The content type of the data.
 
         `**Returns**``
         - `Tuple[str, dict, Union[dict, bytes, None]]` - The service url, headers and data.
 
         """
 
-        headers = {"NDCDEVICEID": device_id(), **await self.service_headers()}
+        headers = {"NDCDEVICEID": self.generate.device_id(), **await self.service_headers()}
 
         if data or content_type:
             headers, data = await self.fetch_signature(data, headers, content_type)
 
         return url, headers, self.ensure_utf8(data)
 
-
     def ensure_utf8(self, data: Union[dict, bytes, None]) -> Union[dict, bytes, None]:
         """
         `ensure_utf8` - Ensures the data is utf-8 encoded
 
         `**Parameters**``
         - `data` - The data to encode.
 
@@ -254,15 +254,14 @@
         handlers = {
             dict: handle_dict,
             str: handle_str
         }
 
         return handlers.get(type(data), lambda x: x)(data)
 
-
     async def fetch_signature(
             self,
             data: Union[dict, bytes, None],
             headers: dict,
             content_type: str = None
     ) -> Tuple[dict, Union[dict, bytes, None]]:
         """
@@ -285,20 +284,19 @@
                 else dumps(data)
             )
 
         headers.update(
             {
                 "CONTENT-LENGTH": f"{len(data)}",
                 "CONTENT-TYPE": content_type or "application/json; charset=utf-8",
-                "NDC-MSG-SIG": generate_signature(data),
+                "NDC-MSG-SIG": self.generate.signature(data),
             }
         )
         return headers, data
 
-
     async def raise_error(self, response: dict) -> None:
         """
         `raise_error` - Raises an error if an error is in the response
 
         `**Parameters**``
         - `response` - The response from the request.
 
@@ -314,15 +312,14 @@
                 ]
         ):
             return await self.bot.run(self.email, self.password, use_cache=False)
 
         else:
             raise APIException(response)
 
-
     async def handle_response(self, status_code: int, response: str) -> dict:
         """
         `handle_response` - Handles the response and returns the response as a dict
 
         `**Parameters**``
         - `status_code` - The status code of the response.
         - `response` - The response to handle.
@@ -349,15 +346,14 @@
                 response = loads(response)
 
             if status_code != 200:
                 await self.raise_error(response)
 
             return response
 
-
     def print_response(self, method: str, url: str, status_code: int):
         """
         `print_response` - Prints the response if debug is enabled
 
         `**Parameters**``
         - `method` - The request method used.
         - `url` - The url the request was sent to.
@@ -374,12 +370,11 @@
                     "POST": Fore.GREEN,
                     "DELETE": Fore.MAGENTA,
                     "LITE": Fore.YELLOW,
                 }.get(method, Fore.RED)
             )
             print(f"{color}{Style.BRIGHT}{method}{Style.RESET_ALL} - {url}")
 
-
     async def close_session(self):
         if self.session is not None:
             await self.session.close()
             self.session = None
```

### Comparing `pymino-1.2.3.8/pymino/ext/utilities/chat_console.py` & `pymino-1.2.3.9/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/utilities/commands.py` & `pymino-1.2.3.9/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/utilities/community_console.py` & `pymino-1.2.3.9/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/utilities/menu.py` & `pymino-1.2.3.9/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/utilities/profile_console.py` & `pymino-1.2.3.9/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.3.8/pymino/ext/utilities/request_handler.py` & `pymino-1.2.3.9/pymino/ext/utilities/request_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from time import sleep
 from uuid import uuid4
 from ujson import loads, dumps
 from colorama import Fore, Style
 from typing import Optional, Union, Tuple, Callable
 
+from .generate import Generator
 from ..entities.handlers import orjson_exists
-from .generate import device_id, generate_signature
 from requests import Session as Http, Response as HttpResponse
 
 from ..entities import (
     Forbidden,
     BadGateway,
-    NullResponse,
     APIException,
     ServiceUnavailable
     )
+
 from requests.exceptions import (
     ConnectionError,
     ReadTimeout,
     SSLError,
     ProxyError,
     ConnectTimeout
     )
@@ -31,29 +31,36 @@
 
 class RequestHandler:
     """
     `RequestHandler` - A class that handles all requests
 
     `**Parameters**``
     - `bot` - The main bot class.
+    - `generator` - The generator class.    
     - `proxy` - The proxy to use for requests.
 
     """
-    def __init__(self, bot, proxy: Optional[str] = None):
+    def __init__(
+        self,
+        bot,
+        generator: Generator,
+        proxy: Optional[str] = None
+        ) -> None:
         self.bot             = bot
+        self.generate        = generator
         self.http_handler:   Http = Http()
         self.sid:            Optional[str] = None
         self.userId:         Optional[str] = None
         self.orjson:         bool = orjson_exists()
 
         self.proxy = {
             "http": proxy,
             "https": proxy
             } if proxy is not None else None
-        
+
         self.response_map = {
             403: Forbidden,
             502: BadGateway,
             503: ServiceUnavailable
             }
 
     def service_url(self, url: str) -> str:
@@ -103,27 +110,27 @@
     def send_request(
             self,
             method: str,
             url: str,
             data: Union[dict, bytes, None],
             headers: dict,
             content_type: Optional[str]
-        ) -> Union[int, str]:
+        ) -> Tuple[int, str]:
         """
         `send_request` - Sends a request
         
         `**Parameters**``
         - `method` - The request method to use.
         - `url` - The url to send the request to.
         - `data` - The data to send with the request.
         - `headers` - The headers to send with the request.
         - `content_type` - The content type of the data.
         
         `**Returns**``
-        - `Union[int, str]` - The status code and response from the request.
+        - `Tuple[int, str]` - The status code and response from the request.
         
         """
         try:
             response: HttpResponse = self.fetch_request(method)(
                 url, data=data, headers=headers, proxies=self.proxy
             )
             return response.status_code, response.text
@@ -131,16 +138,16 @@
             ConnectionError,
             ReadTimeout,
             SSLError,
             ProxyError,
             ConnectTimeout,
         ):
             sleep(1.5)
-            self.handler(method, url, data, content_type)
-    
+            return self.handler(method, url, data, content_type)
+
     def handler(
         self,
         method: str,
         url: str,
         data: Union[dict, bytes, None] = None,
         content_type: Optional[str] = None
     ) -> dict:
@@ -160,21 +167,29 @@
         url = self.service_url(url)
 
         url, headers, binary_data = self.service_handler(url, data, content_type)
 
         if all([method=="POST", data is None]):
             headers["CONTENT-TYPE"] = "application/octet-stream"
 
-        status_code, content = self.send_request(
-            method, url, binary_data, headers, content_type
-        )
+        try:
+            status_code, content = self.send_request(
+                method, url, binary_data, headers, content_type
+            )
+        except TypeError: # NOTE: Not sure if this is even needed.
+            return self.handler(method, url, data, content_type)
 
         self.print_response(method=method, url=url, status_code=status_code)
 
-        return self.handle_response(status_code=status_code, response=content)
+        response = self.handle_response(status_code=status_code, response=content)
+
+        if response is None:
+            return self.handler(method, url, data, content_type)
+        
+        return response
 
     def service_handler(
         self,
         url: str,
         data: Union[dict, bytes, None] = None,
         content_type: Optional[str] = None
     ) -> Tuple[str, dict, Union[dict, bytes, None]]:
@@ -187,15 +202,15 @@
         - `content_type` - The content type of the data.
         
         `**Returns**``
         - `Tuple[str, dict, Union[dict, bytes, None]]` - The service url, headers and data.
 
         """
         
-        headers = {"NDCDEVICEID": device_id(), **self.service_headers()}
+        headers = {"NDCDEVICEID": self.generate.device_id(), **self.service_headers()}
 
         if data or content_type:
             headers, data = self.fetch_signature(data, headers, content_type)
 
         return url, headers, self.ensure_utf8(data)
 
     def ensure_utf8(self, data: Union[dict, bytes, None]) -> Union[dict, bytes, None]:
@@ -247,39 +262,42 @@
         if not isinstance(data, bytes):
             data = orjson_dumps(data).decode("utf-8") if self.orjson else dumps(data)
 
         headers.update({
             "CONTENT-LENGTH": f"{len(data)}",
             "CONTENT-TYPE": content_type or "application/json; charset=utf-8",
             "NDC-MSG-SIG": (
-                generate_signature(data)
+                self.generate.signature(data)
             )
         })
         return headers, data
 
     def raise_error(self, response: dict) -> None:
         """
         `raise_error` - Raises an error if an error is in the response
         
         `**Parameters**``
         - `response` - The response from the request.
         
         `**Returns**``
         - `None` - Raises an error if the status code is in the response map.
+        - `404` - Returns 404 if the status code is 105 and the email and password is set.
         
         """
-        if all([
-            response.get("api:statuscode", 200) == 105,
-            hasattr(self, "email"),
-            hasattr(self, "password")
-            ]):
-            # NOTE: Login expired will have to run request manually
-            return self.bot.run(self.email, self.password, use_cache=False)
-        
-        else: raise APIException(response)
+        if all(
+            [
+                response.get("api:statuscode", 200) == 105,
+                hasattr(self, "email"),
+                hasattr(self, "password"),
+            ]
+        ):
+            self.bot.run(self.email, self.password, use_cache=False)
+            return 404      
+      
+        raise APIException(response)
         
     def handle_response(self, status_code: int, response: str) -> dict:
         """
         `handle_response` - Handles the response and returns the response as a dict
         
         `**Parameters**``
         - `status_code` - The status code of the response.
@@ -287,29 +305,26 @@
         
         `**Returns**``
         - `dict` - The response as a dict.
         
         """
         if status_code in self.response_map:
             raise self.response_map[status_code]
-        
-        elif response.startswith("null"):
-            raise NullResponse
-        
-        else:
-            
-            try:
-                response = orjson_loads(response) if self.orjson else loads(response)
-            except Exception:
-                response = loads(response)
 
-            if status_code != 200:
-                self.raise_error(response)
+        try:
+            response = orjson_loads(response) if self.orjson else loads(response)
+        except Exception:
+            response = loads(response)
+
+        if status_code != 200:
+            check_response = self.raise_error(response)
+            if check_response == 404:
+                return None
 
-            return response
+        return response
 
     def print_response(self, method: str, url: str, status_code: int):
         """
         `print_response` - Prints the response if debug is enabled
 
         `**Parameters**``
         - `method` - The request method used.
```

### Comparing `pymino-1.2.3.8/pymino.egg-info/PKG-INFO` & `pymino-1.2.3.9/pymino.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.3.8
+Version: 1.2.3.9
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <h1 style="color: #0d47a1; font-size: 3em;">pymino</h1>
   
   <p>
```

#### html2text {}

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.3.8 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.3.9 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE
+:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Requires-Python: >=3.8 Description-Content-Type:
+text/markdown License-File: LICENSE
                              ****** pymino ******
 [Discord] [Libraries.io_dependency_status_for_GitHub_repo] [GitHub_last_commit]
                               [PyPI_-_Downloads]
            A Python wrapper to communicate with the Amino Apps API.
     Easily create a bot for Amino Apps using a modern, easy-to-use library.
                                **** WARNING ****
  Pymino is a fully reverse-engineered client. By using this client, you may be
```

### Comparing `pymino-1.2.3.8/pymino.egg-info/SOURCES.txt` & `pymino-1.2.3.9/pymino.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 pymino/client.py
 pymino.egg-info/PKG-INFO
 pymino.egg-info/SOURCES.txt
 pymino.egg-info/dependency_links.txt
 pymino.egg-info/requires.txt
 pymino.egg-info/top_level.txt
 pymino/ext/__init__.py
-pymino/ext/_global.py
 pymino/ext/account.py
 pymino/ext/async_account.py
 pymino/ext/async_community.py
 pymino/ext/async_context.py
 pymino/ext/async_event_handler.py
 pymino/ext/async_global_client.py
 pymino/ext/async_socket.py
```

### Comparing `pymino-1.2.3.8/setup.cfg` & `pymino-1.2.3.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e32 2e33 2e38 0d0a 6175  on = 1.2.3.8..au
+00000020: 6f6e 203d 2031 2e32 2e33 2e39 0d0a 6175  on = 1.2.3.9..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
@@ -27,29 +27,27 @@
 000001a0: 696e 6f2d 626f 742c 2061 6d69 6e6f 2d62  ino-bot, amino-b
 000001b0: 6f74 730d 0a63 6c61 7373 6966 6965 7273  ots..classifiers
 000001c0: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
 000001d0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
 000001e0: 7468 6f6e 203a 3a20 330d 0a09 5072 6f67  thon :: 3...Prog
 000001f0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
 00000200: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000210: 370d 0a09 5072 6f67 7261 6d6d 696e 6720  7...Programming 
+00000210: 380d 0a09 5072 6f67 7261 6d6d 696e 6720  8...Programming 
 00000220: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000230: 6f6e 203a 3a20 332e 380d 0a09 5072 6f67  on :: 3.8...Prog
-00000240: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000250: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000260: 390d 0a09 546f 7069 6320 3a3a 2053 6f66  9...Topic :: Sof
-00000270: 7477 6172 6520 4465 7665 6c6f 706d 656e  tware Developmen
-00000280: 7420 3a3a 204c 6962 7261 7269 6573 203a  t :: Libraries :
-00000290: 3a20 5079 7468 6f6e 204d 6f64 756c 6573  : Python Modules
-000002a0: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
-000002b0: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-000002c0: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-000002d0: 7320 3d20 0d0a 0972 6571 7565 7374 733d  s = ...requests=
-000002e0: 3d32 2e32 382e 320d 0a09 756a 736f 6e3d  =2.28.2...ujson=
-000002f0: 3d35 2e35 2e30 0d0a 0963 6f6c 6f72 616d  =5.5.0...coloram
-00000300: 613d 3d30 2e34 2e36 0d0a 0977 6562 736f  a==0.4.6...webso
-00000310: 636b 6574 2d63 6c69 656e 743d 3d31 2e34  cket-client==1.4
-00000320: 2e31 0d0a 7079 7468 6f6e 5f72 6571 7569  .1..python_requi
-00000330: 7265 7320 3d20 3e3d 332e 370d 0a0d 0a5b  res = >=3.7....[
-00000340: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-00000350: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-00000360: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000230: 6f6e 203a 3a20 332e 390d 0a09 546f 7069  on :: 3.9...Topi
+00000240: 6320 3a3a 2053 6f66 7477 6172 6520 4465  c :: Software De
+00000250: 7665 6c6f 706d 656e 7420 3a3a 204c 6962  velopment :: Lib
+00000260: 7261 7269 6573 203a 3a20 5079 7468 6f6e  raries :: Python
+00000270: 204d 6f64 756c 6573 0d0a 0d0a 5b6f 7074   Modules....[opt
+00000280: 696f 6e73 5d0d 0a70 6163 6b61 6765 7320  ions]..packages 
+00000290: 3d20 6669 6e64 3a0d 0a69 6e73 7461 6c6c  = find:..install
+000002a0: 5f72 6571 7569 7265 7320 3d20 0d0a 0972  _requires = ...r
+000002b0: 6571 7565 7374 733d 3d32 2e32 382e 320d  equests==2.28.2.
+000002c0: 0a09 756a 736f 6e3d 3d35 2e35 2e30 0d0a  ..ujson==5.5.0..
+000002d0: 0963 6f6c 6f72 616d 613d 3d30 2e34 2e36  .colorama==0.4.6
+000002e0: 0d0a 0977 6562 736f 636b 6574 2d63 6c69  ...websocket-cli
+000002f0: 656e 743d 3d31 2e34 2e31 0d0a 7079 7468  ent==1.4.1..pyth
+00000300: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+00000310: 332e 380d 0a0d 0a5b 6567 675f 696e 666f  3.8....[egg_info
+00000320: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000330: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000340: 0a                                       .
```

### Comparing `pymino-1.2.3.8/setup.py` & `pymino-1.2.3.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,29 +18,27 @@
     packages=find_packages(),
     install_requires=[
         "requests==2.31.0",
         "ujson==5.8.0",
         "colorama==0.4.6",
         "websocket-client==1.6.1",
         "diskcache==5.6.1",
-        "aiohttp==3.8.4",
-        "wsaccel==0.6.4"
+        "aiohttp==3.8.4"
     ],
     keywords=[
         "amino",
         "pymino",
         "narvii",
         "amino-api",
         "narvii-bots",
         "aminoapps",
         "amino-bot",
         "amino-bots"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
-    python_requires=">=3.7"
+    python_requires=">=3.8"
 )
```

