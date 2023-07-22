# Comparing `tmp/babymaycry-0.0.3.tar.gz` & `tmp/babymaycry-0.0.4.tar.gz`

## Comparing `babymaycry-0.0.3.tar` & `babymaycry-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 babymaycry-0.0.3/src/babymaycry/__init__.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 babymaycry-0.0.3/src/babymaycry/api.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 babymaycry-0.0.3/.gitignore
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 babymaycry-0.0.3/README.md
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 babymaycry-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 babymaycry-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 babymaycry-0.0.4/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 babymaycry-0.0.4/src/babymaycry/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 babymaycry-0.0.4/src/babymaycry/api.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 babymaycry-0.0.4/.gitignore
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 babymaycry-0.0.4/README.md
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 babymaycry-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 babymaycry-0.0.4/PKG-INFO
```

### Comparing `babymaycry-0.0.3/src/babymaycry/api.py` & `babymaycry-0.0.4/src/babymaycry/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pyaudio
 import telegram
+import asyncio
 
 
 class BabyMayCry:
     def __init__(self, bot_token, chat_id):
         self.bot_token = bot_token
         self.chat_id = chat_id
         self.threshold = 1000
@@ -28,9 +29,9 @@
 
         stream.stop_stream()
         stream.close()
         audio.terminate()
     
     def send_message(self, text):
         bot = telegram.Bot(token=self.bot_token)
-        bot.sendMessage(chat_id=self.chat_id, text=text)
+        asyncio.run(bot.sendMessage(chat_id=self.chat_id, text=text))
```

### Comparing `babymaycry-0.0.3/.gitignore` & `babymaycry-0.0.4/.gitignore`

 * *Files identical despite different names*

