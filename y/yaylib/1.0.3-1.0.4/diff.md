# Comparing `tmp/yaylib-1.0.3.tar.gz` & `tmp/yaylib-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaylib-1.0.3.tar", last modified: Tue Jul 18 10:33:39 2023, max compression
+gzip compressed data, was "yaylib-1.0.4.tar", last modified: Sat Jul 22 09:15:23 2023, max compression
```

## Comparing `yaylib-1.0.3.tar` & `yaylib-1.0.4.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 10:33:39.051243 yaylib-1.0.3/
--rw-rw-rw-   0        0        0     1096 2023-07-09 07:25:01.000000 yaylib-1.0.3/LICENSE
--rw-rw-rw-   0        0        0    10828 2023-07-18 10:33:39.050242 yaylib-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     9964 2023-07-18 08:52:45.000000 yaylib-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-18 10:33:39.051243 yaylib-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1552 2023-07-16 09:10:03.000000 yaylib-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 10:33:38.998476 yaylib-1.0.3/tests/
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.3/tests/test_call.py
--rw-rw-rw-   0        0        0     1935 2023-07-09 07:25:01.000000 yaylib-1.0.3/tests/test_cassandra.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.3/tests/test_chat.py
--rw-rw-rw-   0        0        0     1337 2023-07-09 07:25:01.000000 yaylib-1.0.3/tests/test_group.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.3/tests/test_misc.py
--rw-rw-rw-   0        0        0     3723 2023-07-09 07:25:01.000000 yaylib-1.0.3/tests/test_post.py
--rw-rw-rw-   0        0        0     2028 2023-07-09 07:25:01.000000 yaylib-1.0.3/tests/test_review.py
--rw-rw-rw-   0        0        0     1339 2023-07-09 07:25:01.000000 yaylib-1.0.3/tests/test_thread.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.3/tests/test_user.py
-drwxrwxrwx   0        0        0        0 2023-07-18 10:33:39.011415 yaylib-1.0.3/yaylib/
--rw-rw-rw-   0        0        0      519 2023-07-09 07:25:01.000000 yaylib-1.0.3/yaylib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 10:33:39.048943 yaylib-1.0.3/yaylib/api/
--rw-rw-rw-   0        0        0      697 2023-07-09 07:25:01.000000 yaylib-1.0.3/yaylib/api/__init__.py
--rw-rw-rw-   0        0        0    10255 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/api.py
--rw-rw-rw-   0        0        0     9431 2023-07-18 10:27:35.000000 yaylib-1.0.3/yaylib/api/call.py
--rw-rw-rw-   0        0        0     2699 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/cassandra.py
--rw-rw-rw-   0        0        0    14881 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/chat.py
--rw-rw-rw-   0        0        0    23695 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/group.py
--rw-rw-rw-   0        0        0     8205 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/login.py
--rw-rw-rw-   0        0        0     7417 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/misc.py
--rw-rw-rw-   0        0        0    33692 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/post.py
--rw-rw-rw-   0        0        0     4488 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/review.py
--rw-rw-rw-   0        0        0     5945 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/thread.py
--rw-rw-rw-   0        0        0    24492 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/api/user.py
--rw-rw-rw-   0        0        0    86745 2023-07-18 10:29:00.000000 yaylib-1.0.3/yaylib/client.py
--rw-rw-rw-   0        0        0    19269 2023-07-18 10:33:32.000000 yaylib-1.0.3/yaylib/config.py
--rw-rw-rw-   0        0        0     2131 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/errors.py
--rw-rw-rw-   0        0        0    53336 2023-07-09 07:25:01.000000 yaylib-1.0.3/yaylib/models.py
--rw-rw-rw-   0        0        0    33426 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/responses.py
--rw-rw-rw-   0        0        0     4472 2023-07-18 08:52:45.000000 yaylib-1.0.3/yaylib/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-18 10:33:39.032985 yaylib-1.0.3/yaylib.egg-info/
--rw-rw-rw-   0        0        0    10828 2023-07-18 10:33:38.000000 yaylib-1.0.3/yaylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      721 2023-07-18 10:33:38.000000 yaylib-1.0.3/yaylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 10:33:38.000000 yaylib-1.0.3/yaylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-18 10:33:38.000000 yaylib-1.0.3/yaylib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-18 10:33:38.000000 yaylib-1.0.3/yaylib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 09:15:23.303621 yaylib-1.0.4/
+-rw-rw-rw-   0        0        0     1096 2023-07-09 07:25:01.000000 yaylib-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0    10828 2023-07-22 09:15:23.302615 yaylib-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9964 2023-07-18 08:52:45.000000 yaylib-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-22 09:15:23.303621 yaylib-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1584 2023-07-21 11:06:20.000000 yaylib-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:15:23.254603 yaylib-1.0.4/tests/
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.4/tests/test_call.py
+-rw-rw-rw-   0        0        0     1935 2023-07-09 07:25:01.000000 yaylib-1.0.4/tests/test_cassandra.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.4/tests/test_chat.py
+-rw-rw-rw-   0        0        0     1337 2023-07-09 07:25:01.000000 yaylib-1.0.4/tests/test_group.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.4/tests/test_misc.py
+-rw-rw-rw-   0        0        0     3723 2023-07-09 07:25:01.000000 yaylib-1.0.4/tests/test_post.py
+-rw-rw-rw-   0        0        0     2028 2023-07-09 07:25:01.000000 yaylib-1.0.4/tests/test_review.py
+-rw-rw-rw-   0        0        0     1339 2023-07-09 07:25:01.000000 yaylib-1.0.4/tests/test_thread.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.4/tests/test_user.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:15:23.265092 yaylib-1.0.4/yaylib/
+-rw-rw-rw-   0        0        0      664 2023-07-21 11:06:20.000000 yaylib-1.0.4/yaylib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:15:23.301608 yaylib-1.0.4/yaylib/api/
+-rw-rw-rw-   0        0        0      697 2023-07-09 07:25:01.000000 yaylib-1.0.4/yaylib/api/__init__.py
+-rw-rw-rw-   0        0        0    10255 2023-07-19 13:28:39.000000 yaylib-1.0.4/yaylib/api/api.py
+-rw-rw-rw-   0        0        0     9431 2023-07-18 11:05:38.000000 yaylib-1.0.4/yaylib/api/call.py
+-rw-rw-rw-   0        0        0     2699 2023-07-18 08:52:45.000000 yaylib-1.0.4/yaylib/api/cassandra.py
+-rw-rw-rw-   0        0        0    15017 2023-07-21 11:06:20.000000 yaylib-1.0.4/yaylib/api/chat.py
+-rw-rw-rw-   0        0        0    23695 2023-07-18 08:52:45.000000 yaylib-1.0.4/yaylib/api/group.py
+-rw-rw-rw-   0        0        0     8224 2023-07-20 07:15:23.000000 yaylib-1.0.4/yaylib/api/login.py
+-rw-rw-rw-   0        0        0     7417 2023-07-18 08:52:45.000000 yaylib-1.0.4/yaylib/api/misc.py
+-rw-rw-rw-   0        0        0    33686 2023-07-22 09:13:37.000000 yaylib-1.0.4/yaylib/api/post.py
+-rw-rw-rw-   0        0        0     4488 2023-07-18 08:52:45.000000 yaylib-1.0.4/yaylib/api/review.py
+-rw-rw-rw-   0        0        0     5945 2023-07-18 08:52:45.000000 yaylib-1.0.4/yaylib/api/thread.py
+-rw-rw-rw-   0        0        0    23744 2023-07-19 12:23:37.000000 yaylib-1.0.4/yaylib/api/user.py
+-rw-rw-rw-   0        0        0    86548 2023-07-21 11:06:20.000000 yaylib-1.0.4/yaylib/client.py
+-rw-rw-rw-   0        0        0    19309 2023-07-22 09:15:14.000000 yaylib-1.0.4/yaylib/config.py
+-rw-rw-rw-   0        0        0     2131 2023-07-18 08:52:45.000000 yaylib-1.0.4/yaylib/errors.py
+-rw-rw-rw-   0        0        0    56113 2023-07-21 11:49:21.000000 yaylib-1.0.4/yaylib/models.py
+-rw-rw-rw-   0        0        0    34292 2023-07-21 11:34:08.000000 yaylib-1.0.4/yaylib/responses.py
+-rw-rw-rw-   0        0        0     4473 2023-07-20 07:15:24.000000 yaylib-1.0.4/yaylib/utils.py
+-rw-rw-rw-   0        0        0     9374 2023-07-21 12:27:01.000000 yaylib-1.0.4/yaylib/websocket.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:15:23.283775 yaylib-1.0.4/yaylib.egg-info/
+-rw-rw-rw-   0        0        0    10828 2023-07-22 09:15:23.000000 yaylib-1.0.4/yaylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      741 2023-07-22 09:15:23.000000 yaylib-1.0.4/yaylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 09:15:23.000000 yaylib-1.0.4/yaylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-07-22 09:15:23.000000 yaylib-1.0.4/yaylib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-22 09:15:23.000000 yaylib-1.0.4/yaylib.egg-info/top_level.txt
```

### Comparing `yaylib-1.0.3/LICENSE` & `yaylib-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/PKG-INFO` & `yaylib-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 1.0.3
+Version: 1.0.4
 Summary: This Python package provides an easy-to-use interface for accessing data from Yay! (https://yay.space/). With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts.
 Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib
 Author: Qvco, Konn
 Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn
 Maintainer-email: nikola.desuga@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yaylib Version: 1.0.3 Summary: This Python package
+Metadata-Version: 2.1 Name: yaylib Version: 1.0.4 Summary: This Python package
 provides an easy-to-use interface for accessing data from Yay! (https://
 yay.space/). With this API Client, you can retrieve user profiles, posts,
 comments, and other content from Yay!, as well as perform common tasks like
 liking and commenting on posts. Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib Author: Qvco, Konn Author-email:
 nikola.desuga@gmail.com Maintainer: Qvco, Konn Maintainer-email:
 nikola.desuga@gmail.com License: MIT Keywords:
```

### Comparing `yaylib-1.0.3/README.md` & `yaylib-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/setup.py` & `yaylib-1.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     "ライブラリ",
 ]
 
 install_requires = [
     "httpx>=0.17.1",
     "Pillow>=9.3.0",
     "cryptography>=41.0.1",
+    "websocket-client>=1.6.0",
 ]
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
 ]
```

### Comparing `yaylib-1.0.3/tests/test_call.py` & `yaylib-1.0.4/tests/test_call.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/tests/test_cassandra.py` & `yaylib-1.0.4/tests/test_cassandra.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/tests/test_chat.py` & `yaylib-1.0.4/tests/test_chat.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/tests/test_group.py` & `yaylib-1.0.4/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/tests/test_misc.py` & `yaylib-1.0.4/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/tests/test_post.py` & `yaylib-1.0.4/tests/test_post.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/tests/test_review.py` & `yaylib-1.0.4/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/tests/test_thread.py` & `yaylib-1.0.4/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/tests/test_user.py` & `yaylib-1.0.4/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/yaylib/api/__init__.py` & `yaylib-1.0.4/yaylib/api/__init__.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/yaylib/api/api.py` & `yaylib-1.0.4/yaylib/api/api.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/yaylib/api/call.py` & `yaylib-1.0.4/yaylib/api/call.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/yaylib/api/cassandra.py` & `yaylib-1.0.4/yaylib/api/cassandra.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/yaylib/api/chat.py` & `yaylib-1.0.4/yaylib/api/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,18 +38,21 @@
     StickerPacksResponse,
     UnreadStatusResponse,
 )
 
 
 def accept_chat_request(self, chat_room_ids: List[int], access_token: str = None):
     self._check_authorization(access_token)
+    chat_room_ids = (
+        [chat_room_ids] if not isinstance(chat_room_ids, list) else chat_room_ids
+    )
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.CHAT_ROOMS_V1}/accept_chat_request",
-        payload={"chat_room_ids[]": chat_room_ids},
+        payload={"chat_room_ids": chat_room_ids},
         access_token=access_token,
     )
     self.logger.info("Accepted chat requests")
     return response
 
 
 def check_unread_status(
@@ -423,30 +426,31 @@
     message_type: str,
     call_type: str = None,
     text: str = None,
     font_size: int = None,
     gif_image_id: int = None,
     attachment_file_name: str = None,
     sticker_pack_id: int = None,
+    sticker_id: int = None,
     video_file_name: str = None,
     access_token: str = None,
 ) -> MessageResponse:
     self._check_authorization(access_token)
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.CHAT_ROOMS_V3}/{chat_room_id}/messages/new",
         payload={
-            "chat_room_id": chat_room_id,
             "message_type": message_type,
             "call_type": call_type,
             "text": text,
             "font_size": font_size,
             "gif_image_id": gif_image_id,
             "attachment_file_name": attachment_file_name,
             "sticker_pack_id": sticker_pack_id,
+            "sticker_id": sticker_id,
             "video_file_name": video_file_name,
         },
         data_type=MessageResponse,
         access_token=access_token,
     )
     self.logger.info("Your message has been sent.")
     return response
```

### Comparing `yaylib-1.0.3/yaylib/api/group.py` & `yaylib-1.0.4/yaylib/api/group.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/yaylib/api/login.py` & `yaylib-1.0.4/yaylib/api/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
             self.secret_key = secret_key
             self.fernet = Fernet(secret_key)
             session = decrypt(fernet=self.fernet, session=session)
             self.session.headers.setdefault(
                 "Authorization", f"Bearer {session['access_token']}"
             )
             self.logger.info(f"Successfully logged in as '{session['user_id']}'")
-            return session
+            return LoginUserResponse(session)
         elif session is not None:
             message = f"{Colors.WARNING}Session file found. The 'secret_key' must be provided to decrypt the credentials.{Colors.RESET}"
             console_print(message)
 
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V3}/login_with_email",
```

### Comparing `yaylib-1.0.3/yaylib/api/misc.py` & `yaylib-1.0.4/yaylib/api/misc.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/yaylib/api/post.py` & `yaylib-1.0.4/yaylib/api/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,15 +275,15 @@
         payload={
             "text": text,
             "font_size": font_size,
             "color": color,
             "in_reply_to": in_reply_to,
             "group_id": group_id,
             "post_type": post_type,
-            "mention_ids[]": mention_ids,
+            "mention_ids": mention_ids,
             "choices": choices,
             "shared_url": shared_url,
             "message_tags": message_tags,
             "attachment_filename": attachment_filename,
             "attachment_2_filename": attachment_2_filename,
             "attachment_3_filename": attachment_3_filename,
             "attachment_4_filename": attachment_4_filename,
@@ -362,15 +362,15 @@
             "post_id": post_id,
             "text": text,
             "font_size": font_size,
             "color": color,
             "in_reply_to": in_reply_to,
             "group_id": group_id,
             "post_type": post_type,
-            "mention_ids[]": mention_ids,
+            "mention_ids": mention_ids,
             "choices": choices,
             "shared_url": shared_url,
             "message_tags": message_tags,
             "attachment_filename": attachment_filename,
             "attachment_2_filename": attachment_2_filename,
             "attachment_3_filename": attachment_3_filename,
             "attachment_4_filename": attachment_4_filename,
@@ -483,15 +483,15 @@
             "id": post_id,
             "text": text,
             "font_size": font_size,
             "color": color,
             "in_reply_to": in_reply_to,
             "group_id": group_id,
             "post_type": post_type,
-            "mention_ids[]": mention_ids,
+            "mention_ids": mention_ids,
             "choices": choices,
             "shared_url": shared_url,
             "message_tags": message_tags,
             "attachment_filename": attachment_filename,
             "attachment_2_filename": attachment_2_filename,
             "attachment_3_filename": attachment_3_filename,
             "attachment_4_filename": attachment_4_filename,
```

### Comparing `yaylib-1.0.3/yaylib/api/review.py` & `yaylib-1.0.4/yaylib/api/review.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/yaylib/api/thread.py` & `yaylib-1.0.4/yaylib/api/thread.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/yaylib/api/user.py` & `yaylib-1.0.4/yaylib/api/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,34 +418,14 @@
         params={"user_ids[]": user_ids},
         data_type=UsersResponse,
         headers=headers,
         access_token=access_token,
     )
 
 
-def reduce_kenta_penalty(self, user_id: int, access_token: str = None):
-    self._check_authorization(access_token)
-    timestamp = int(datetime.now().timestamp())
-    response = self._make_request(
-        "POST",
-        endpoint=f"{Configs.YAY_API_URL}/api/v3/users/{user_id}/reduce_penalty",
-        payload={
-            "app_version": self.api_version,
-            "timestamp": timestamp,
-            "api_key": self.api_key,
-            "signed_info": signed_info_calculating(self.device_uuid, timestamp),
-            "signed_version": signed_version_calculating(),
-            "uuid": self.uuid,
-        },
-        access_token=access_token,
-    )
-    self.logger.info("Penalty has been reduced.")
-    return response
-
-
 def refresh_counter(self, counter: str, access_token: str = None):
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V1}/reset_counters",
         payload={"counter": counter},
         access_token=access_token,
     )
```

### Comparing `yaylib-1.0.3/yaylib/client.py` & `yaylib-1.0.4/yaylib/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     invite_users_to_chat_call,
     kick_and_ban_from_call,
     set_call,
     set_user_role,
     start_call,
     start_anonymous_call,
     stop_call,
-    stop__anonymous_call
+    stop__anonymous_call,
 )
 from .api.cassandra import (
     get_user_activities,
     get_user_merged_activities,
     received_notification,
 )
 from .api.chat import (
@@ -235,15 +235,14 @@
     get_user,
     get_user_email,
     get_user_followers,
     get_user_followings,
     get_user_from_qr,
     get_user_without_leaving_footprint,
     get_users,
-    reduce_kenta_penalty,
     refresh_counter,
     register_user,
     remove_user_avatar,
     remove_user_cover,
     report_user,
     reset_password,
     search_lobi_users,
@@ -932,14 +931,15 @@
         message_type: str,
         call_type: str = None,
         text: str = None,
         font_size: int = None,
         gif_image_id: int = None,
         attachment_file_name: str = None,
         sticker_pack_id: int = None,
+        sticker_id: int = None,
         video_file_name: str = None,
         access_token: str = None,
     ) -> MessageResponse:
         """
 
         チャットルームにメッセージを送信します
 
@@ -950,14 +950,15 @@
             message_type,
             call_type,
             text,
             font_size,
             gif_image_id,
             attachment_file_name,
             sticker_pack_id,
+            sticker_id,
             video_file_name,
             access_token,
         )
 
     def unhide_chat(self, chat_room_ids: int, access_token: str = None) -> dict:
         """
 
@@ -2931,22 +2932,14 @@
         """
 
         複数のユーザーの情報を取得します
 
         """
         return get_users(self, user_ids, access_token)
 
-    def reduce_kenta_penalty(self, user_id: int, access_token: str = None) -> dict:
-        """
-
-        ペナルティーを緩和します
-
-        """
-        return reduce_kenta_penalty(self, user_id, access_token)
-
     def refresh_counter(self, counter: str, access_token: str = None) -> dict:
         """
 
         カウンターを更新します
 
         """
         return refresh_counter(self, counter, access_token)
```

### Comparing `yaylib-1.0.3/yaylib/config.py` & `yaylib-1.0.4/yaylib/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,27 +22,28 @@
 SOFTWARE.
 """
 
 from enum import Enum
 
 
 class Configs:
-    YAYLIB_VERSION = "1.0.3"
+    YAYLIB_VERSION = "1.0.4"
     YAY_API_VERSION = "3.20"
     YAY_VERSION_NAME = "3.20.1"
     YAY_API_VERSION_KEY = "d4420f4943bebe2831c20b2b4cb4a8c1"
     YAY_API_KEY = "ccd59ee269c01511ba763467045c115779fcae3050238a252f1bd1a4b65cfec6"
     YAY_SHARED_KEY = "yayZ1"
     YAY_STORE_KEY = "yayZ1payment"
     AGORA_APP_ID = "79046b8c9be54945b7f10a4d128d5395"
     ID_CARD_CHECK_SECRET_KEY = "4aa6d1c301a97154bc1098c2"
     YAY_REVIEW_HOST_1 = "review.yay.space"
     YAY_REVIEW_HOST_2 = "cas-stg.yay.space"
     YAY_STAGING_HOST_1 = "stg.yay.space"
     YAY_STAGING_HOST_2 = "cas.yay.space"
+    YAY_CABLE_HOST = "cable.yay.space"
     YAY_PRODUCTION_HOST = "api.yay.space"
     YAY_API_URL = "https://" + YAY_PRODUCTION_HOST
     ID_CARD_CHECK_HOST_PRODUCTION = "idcardcheck.com"
     ID_CARD_CHECK_HOST_STAGING = "stg.idcardcheck.com"
     USER_AGENT = "android 11 (3.5x 1440x2960 Galaxy S9)"
     REQUEST_HEADERS = {
         "Host": YAY_PRODUCTION_HOST,
```

### Comparing `yaylib-1.0.3/yaylib/errors.py` & `yaylib-1.0.4/yaylib/errors.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.3/yaylib/models.py` & `yaylib-1.0.4/yaylib/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
         self.background = data.get("background")
 
         self.last_message = data.get("last_message")
         if self.last_message is not None:
             self.last_message = Message(self.last_message)
 
-        self.name = data.get("updated_at")
+        self.name = data.get("name")
         self.is_group = data.get("is_group")
 
         self.owner = data.get("owner")
         if self.owner is not None:
             self.owner = User(self.owner)
 
         self.is_request = data.get("is_request")
@@ -186,14 +186,76 @@
         self.id = data.get("id")
         self.text = data.get("text")
 
     def __repr__(self):
         return f"ChatRoomDraft(data={self.data})"
 
 
+class MessageEvent:
+    __slots__ = (
+        "data",
+        "message",
+        "event",
+    )
+
+    def __init__(self, data):
+        self.data = data
+
+        self.message = data.get("data")
+        if self.message is not None:
+            self.message = Message(self.message)
+
+        self.event = data.get("event")
+
+    def __repr__(self):
+        return f"MessageEvent(data={self.data})"
+
+
+class ChatRoomEvent:
+    __slots__ = (
+        "data",
+        "icon_thumbnail",
+        "id",
+        "last_message",
+        "name",
+        "unread_count",
+    )
+
+    def __init__(self, data):
+        self.data = data
+        self.icon_thumbnail = data.get("icon_thumbnail")
+        self.id = data.get("id")
+
+        self.last_message = data.get("last_message")
+        if self.last_message is not None:
+            self.last_message = Message(self.last_message)
+
+        self.name = data.get("name")
+        self.unread_count = data.get("unread_count")
+
+    def __repr__(self):
+        return f"ChatRoomEvent(data={self.data})"
+
+
+class GroupUpdatesEvent:
+    __slots__ = (
+        "response",
+        "data",
+        "event",
+    )
+
+    def __init__(self, data):
+        self.response = data
+        self.data = data.get("data")
+        self.event = data.get("event")
+
+    def __repr__(self):
+        return f"GroupUpdateEvent(data={self.response})"
+
+
 class Choice:
     __slots__ = ("data", "id", "label", "votes_count")
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.label = data.get("label")
@@ -727,27 +789,71 @@
         self.selected = data.get("selected")
 
     def __repr__(self):
         return f"Interest(data={self.data})"
 
 
 class Message:
-    __slots__ = ("data", "id", "user_id", "type", "text", "conference_call")
+    __slots__ = (
+        "data",
+        "attachment",
+        "attachment_android",
+        "attachment_thumbnail",
+        "conference_call",
+        "created_at",
+        "font_size",
+        "gif",
+        "id",
+        "message_type",
+        "reactions_count",
+        "room_id",
+        "sticker",
+        "text",
+        "user",
+        "user_id",
+        "video_processed",
+        "video_thumbnail_big_url",
+        "video_thumbnail_url",
+        "video_url",
+    )
 
     def __init__(self, data):
         self.data = data
-        self.id = data.get("id")
-        self.user_id = data.get("user_id")
-        self.type = data.get("type")
-        self.text = data.get("text")
+        self.attachment = data.get("attachment")
+        self.attachment_android = data.get("attachment_android")
+        self.attachment_thumbnail = data.get("attachment_thumbnail")
 
         self.conference_call = data.get("conference_call")
         if self.conference_call is not None:
             self.conference_call = ConferenceCall(self.conference_call)
 
+        self.created_at = data.get("created_at")
+        self.font_size = data.get("font_size")
+
+        self.gif = data.get("gif")
+        if self.gif is not None:
+            self.gif = GifImage(self.gif)
+
+        self.id = data.get("id")
+        self.message_type = data.get("message_type")
+        self.reactions_count = data.get("reactions_count")
+        self.room_id = data.get("room_id")
+
+        self.sticker = data.get("sticker")
+        if self.sticker is not None:
+            self.sticker = Sticker(self.sticker)
+
+        self.text = data.get("text")
+        self.user = data.get("user")
+        self.user_id = data.get("user_id")
+        self.video_processed = data.get("video_processed")
+        self.video_thumbnail_big_url = data.get("video_thumbnail_big_url")
+        self.video_thumbnail_url = data.get("video_thumbnail_url")
+        self.video_url = data.get("video_url")
+
     def __repr__(self):
         return f"Message(data={self.data})"
 
 
 class MessageTag:
     __slots__ = ("data", "user_id", "offset", "length", "type")
```

### Comparing `yaylib-1.0.3/yaylib/responses.py` & `yaylib-1.0.4/yaylib/responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,15 +250,15 @@
 
 
 class TotalChatRequestResponse:
     __slots__ = ("data", "total")
 
     def __init__(self, data):
         self.data = data
-        self.chat = data.get("total")
+        self.total = data.get("total")
 
     def __repr__(self):
         return f"TotalChatRequestResponse(data={self.data})"
 
 
 class ConferenceCallResponse:
     __slots__ = ("data", "conference_call")
@@ -572,15 +572,15 @@
     __slots__ = ("data", "group")
 
     def __init__(self, data):
         self.data = data
 
         self.group = data.get("group")
         if self.group is not None:
-            self.group = Setting(self.group)
+            self.group = Group(self.group)
 
     def __repr__(self):
         return f"GroupResponse(data={self.data})"
 
 
 class GroupsRelatedResponse:
     __slots__ = ("data", "groups", "next_page_value")
@@ -1186,14 +1186,44 @@
         self.ip_address = data.get("ip_address")
         self.country = data.get("country")
 
     def __repr__(self):
         return f"UserTimestampResponse(data={self.data})"
 
 
+class ChannelResponse:
+    __slots__ = ("data", "identifier", "message", "type", "sid")
+
+    def __init__(self, data):
+        self.data = data
+        self.identifier = data.get("identifier")
+
+        self.message = data.get("message")
+        if self.message is not None and isinstance(self.message, dict):
+            self.message = WebSocketMessageResponse(self.message)
+
+        self.type = data.get("type")
+        self.sid = data.get("sid")
+
+    def __repr__(self):
+        return f"ChannelResponse(data={self.data})"
+
+
+class WebSocketMessageResponse:
+    __slots__ = ("response", "data", "event")
+
+    def __init__(self, data):
+        self.response = data
+        self.data = data.get("data")
+        self.event = data.get("event")
+
+    def __repr__(self):
+        return f"WebSocketMessageResponse(response={self.response})"
+
+
 class WebSocketTokenResponse:
     __slots__ = ("data", "token")
 
     def __init__(self, data):
         self.data = data
         self.token = data.get("token")
```

### Comparing `yaylib-1.0.3/yaylib/utils.py` & `yaylib-1.0.4/yaylib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,27 +105,26 @@
     }
     if email is None:
         updated_session["email"] = session.get("email")
 
     updated_session = encrypt(fernet, updated_session)
 
     with open(base_path + "session.json", "w") as f:
-        json.dump(updated_session, f)
+        json.dump(updated_session, f, indent=4)
 
 
 def load_session(base_path: str, fernet=None, check_email: str = None):
     if not os.path.exists(base_path + "session.json"):
         return None
 
     with open(base_path + "session.json", "r") as f:
         session = json.load(f)
 
     result = all(
-        key in session
-        for key in ("access_token", "refresh_token", "user_id", "email")
+        key in session for key in ("access_token", "refresh_token", "user_id", "email")
     )
     session = None if result is False else session
 
     if check_email is not None and session is not None:
         session = None if check_email != session["email"] else session
 
     if fernet is not None and session is not None:
```

### Comparing `yaylib-1.0.3/yaylib.egg-info/PKG-INFO` & `yaylib-1.0.4/yaylib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 1.0.3
+Version: 1.0.4
 Summary: This Python package provides an easy-to-use interface for accessing data from Yay! (https://yay.space/). With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts.
 Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib
 Author: Qvco, Konn
 Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn
 Maintainer-email: nikola.desuga@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yaylib Version: 1.0.3 Summary: This Python package
+Metadata-Version: 2.1 Name: yaylib Version: 1.0.4 Summary: This Python package
 provides an easy-to-use interface for accessing data from Yay! (https://
 yay.space/). With this API Client, you can retrieve user profiles, posts,
 comments, and other content from Yay!, as well as perform common tasks like
 liking and commenting on posts. Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib Author: Qvco, Konn Author-email:
 nikola.desuga@gmail.com Maintainer: Qvco, Konn Maintainer-email:
 nikola.desuga@gmail.com License: MIT Keywords:
```

### Comparing `yaylib-1.0.3/yaylib.egg-info/SOURCES.txt` & `yaylib-1.0.4/yaylib.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 yaylib/__init__.py
 yaylib/client.py
 yaylib/config.py
 yaylib/errors.py
 yaylib/models.py
 yaylib/responses.py
 yaylib/utils.py
+yaylib/websocket.py
 yaylib.egg-info/PKG-INFO
 yaylib.egg-info/SOURCES.txt
 yaylib.egg-info/dependency_links.txt
 yaylib.egg-info/requires.txt
 yaylib.egg-info/top_level.txt
 yaylib/api/__init__.py
 yaylib/api/api.py
```

