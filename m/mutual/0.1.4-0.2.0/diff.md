# Comparing `tmp/mutual-0.1.4.tar.gz` & `tmp/mutual-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutual-0.1.4.tar", last modified: Thu Jul 20 03:30:11 2023, max compression
+gzip compressed data, was "mutual-0.2.0.tar", last modified: Sat Jul 22 04:38:16 2023, max compression
```

## Comparing `mutual-0.1.4.tar` & `mutual-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-20 03:30:11.116644 mutual-0.1.4/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.1.4/LICENSE.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)     6408 2023-07-20 03:30:11.116352 mutual-0.1.4/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)     5982 2023-07-19 07:20:58.000000 mutual-0.1.4/README.md
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-20 03:30:11.114915 mutual-0.1.4/mutual/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1035 2023-07-20 02:30:27.000000 mutual-0.1.4/mutual/APIKey.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     1629 2023-07-19 07:15:42.000000 mutual-0.1.4/mutual/Auth.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     8915 2023-07-20 03:29:48.000000 mutual-0.1.4/mutual/Bot.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4858 2023-07-19 07:16:20.000000 mutual-0.1.4/mutual/Chat.py
--rw-r--r--   0 alexbetita   (501) staff       (20)      602 2023-07-19 07:16:27.000000 mutual-0.1.4/mutual/Dev.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3619 2023-07-19 07:16:46.000000 mutual-0.1.4/mutual/Judge.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3649 2023-07-19 07:17:05.000000 mutual-0.1.4/mutual/JudgeMessage.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3948 2023-07-19 07:17:24.000000 mutual-0.1.4/mutual/Prompt.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4093 2023-07-20 02:27:54.000000 mutual-0.1.4/mutual/__init__.py
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-20 03:30:11.115969 mutual-0.1.4/mutual.egg-info/
--rw-r--r--   0 alexbetita   (501) staff       (20)     6408 2023-07-20 03:30:11.000000 mutual-0.1.4/mutual.egg-info/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)      329 2023-07-20 03:30:11.000000 mutual-0.1.4/mutual.egg-info/SOURCES.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-20 03:30:11.000000 mutual-0.1.4/mutual.egg-info/dependency_links.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-20 03:30:11.000000 mutual-0.1.4/mutual.egg-info/requires.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-20 03:30:11.000000 mutual-0.1.4/mutual.egg-info/top_level.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-20 03:30:11.116854 mutual-0.1.4/setup.cfg
--rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-20 03:30:06.000000 mutual-0.1.4/setup.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-22 04:38:16.544933 mutual-0.2.0/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.2.0/LICENSE.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)     5949 2023-07-22 04:38:16.544755 mutual-0.2.0/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)     5523 2023-07-22 04:36:24.000000 mutual-0.2.0/README.md
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-22 04:38:16.543545 mutual-0.2.0/mutual/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1035 2023-07-22 04:22:14.000000 mutual-0.2.0/mutual/APIKey.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)    10382 2023-07-22 04:34:37.000000 mutual-0.2.0/mutual/Bot.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4858 2023-07-22 04:24:52.000000 mutual-0.2.0/mutual/Chat.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)      602 2023-07-22 04:25:05.000000 mutual-0.2.0/mutual/Dev.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3619 2023-07-22 04:25:23.000000 mutual-0.2.0/mutual/Judge.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3649 2023-07-22 04:25:41.000000 mutual-0.2.0/mutual/JudgeMessage.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3948 2023-07-22 04:26:05.000000 mutual-0.2.0/mutual/Prompt.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4174 2023-07-22 04:08:17.000000 mutual-0.2.0/mutual/__init__.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-22 04:38:16.544511 mutual-0.2.0/mutual.egg-info/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     5949 2023-07-22 04:38:16.000000 mutual-0.2.0/mutual.egg-info/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)      314 2023-07-22 04:38:16.000000 mutual-0.2.0/mutual.egg-info/SOURCES.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-22 04:38:16.000000 mutual-0.2.0/mutual.egg-info/dependency_links.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-22 04:38:16.000000 mutual-0.2.0/mutual.egg-info/requires.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-22 04:38:16.000000 mutual-0.2.0/mutual.egg-info/top_level.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-22 04:38:16.544986 mutual-0.2.0/setup.cfg
+-rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-22 04:37:55.000000 mutual-0.2.0/setup.py
```

### Comparing `mutual-0.1.4/LICENSE.txt` & `mutual-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mutual-0.1.4/PKG-INFO` & `mutual-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutual
-Version: 0.1.4
+Version: 0.2.0
 Summary: A Python client for the Mutual API.
 Home-page: https://github.com/Mutu-AI
 Author: Alex Betita
 Author-email: alexbetita25@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,35 +21,19 @@
 Run `pip install mutual` in the project root directory.
 
 ### Usage
 
 ```python
 import mutual
 
-# SIGNUP
-response = mutual.Auth.signup("password", "email")
-# OR
-response = mutual.Auth.signup(password = "password", email = "email")
-print(response) # after signing up the key is automatically set
-
-# to print the api_key from the response
-api_key = response.get("api_key", None)
-print(api_key)
-
 # to get the api_key
 print(mutual.api_key)
 # to set the api_key
 mutual.api_key = "your_api_key"
 
-# LOGIN
-response = mutual.Auth.login("password", "email")
-# OR 
-response = mutual.Auth.login(password = "password", email = "email")
-print(response)
-
 # CHAT
 mutual.api_key = "your_api_key"
 for message in mutual.Chat.create("Hello", "seansbot", "Sean"):
     print(message['content'], end='', flush=True)
 # OR
 for message in mutual.Chat.create("Hello", bot_name="seansbot", username="Sean", prompt="You are a customer assistant for mutual that provides helpful information"):
     print(message['content'], end='', flush=True)
@@ -88,15 +72,15 @@
 
 # bot id
 alexbot = mutual.fetch_bot("bot_id or bot_name") # THIS WILL LOOK UP FOR A EXISTING BOT AND GENERATE AN INSTANCE OF THAT BOT
 for message in alexbot.chat("Hey there", "Sean"):
     print(message['content'], end='', flush=True)
 
 # update using bot instance
-alexbot.update_bot(bot_org='mutual', bot_name='new_bot_name', prompt_id='new_prompt')
+alexbot.update_bot(bot_name='new_bot_name', prompt='You are a window cleaner')
 
 # view bot instance data
 print(alexbot.api_key) # prints the api_key
 print(alexbot.bot_id) # prints the bot id
 print(alexbot.bot_name) # prints the bot name
 print(alexbot.prompt_id) # prints the prompt id
 print(alexbot.judge_id) # prints the judge_id
@@ -113,15 +97,14 @@
 
 # you can also set the bot_id like this so you dont need to pass it in chat
 mutual.bot_id = "bot_id"
 
 # to print the bot_id
 print(mutual.bot_id)
 
-
 # PROMPT
 
 print(mutual.Prompt.get_prompts())
 print(mutual.Prompt.get_prompt("prompt_id"))
 print(mutual.Prompt.create_prompt("prompt_id", "prompt"))
 # OR
 print(mutual.Prompt.create_prompt(prompt_id="prompt_id", prompt="prompt"))
@@ -163,24 +146,24 @@
 # APIKey naming
 response = mutual.APIKey.update_api_key("new_api_key_name")
 print(response.get("prev_api_key_name", None))
 print(response.get("new_api_key_name", None))
 print(response.get("api_key", None))
 
 # you can import the functions directly like so
-from mutual import Bot, Auth, Chat, Dev, Prompt, Judge, JudgeMessage, APIKey
+from mutual import Bot, Chat, Dev, Prompt, Judge, JudgeMessage, APIKey
 ```
 
 # SAMPLE TO PRINT ERRORS
 ```py
 index = 0
 for message in mutual.Chat.create_demo("Hello"):
-    if index = 0:
+    if index == 0:
         print(message['data']['bot_data']['bot_id'], end='', flush=True)
-        print(message['data']['user_data']['user_id'], end='', flush=True)
+        print(message['data']['user_data']['username'], end='', flush=True)
         print(message['data']['bot_data']['bot_name'], end='', flush=True)
     index += 1
     print(message['content'], end='', flush=True)
 ```
 
 # SAMPLE TO PRINT DATA
 ```py
```

### Comparing `mutual-0.1.4/README.md` & `mutual-0.2.0/mutual.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,39 @@
+Metadata-Version: 2.1
+Name: mutual
+Version: 0.2.0
+Summary: A Python client for the Mutual API.
+Home-page: https://github.com/Mutu-AI
+Author: Alex Betita
+Author-email: alexbetita25@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # mutual
 
 A python package to interact with the Mutuai API.
 
 ## Installation
 
 Run `pip install mutual` in the project root directory.
 
 ### Usage
 
 ```python
 import mutual
 
-# SIGNUP
-response = mutual.Auth.signup("password", "email")
-# OR
-response = mutual.Auth.signup(password = "password", email = "email")
-print(response) # after signing up the key is automatically set
-
-# to print the api_key from the response
-api_key = response.get("api_key", None)
-print(api_key)
-
 # to get the api_key
 print(mutual.api_key)
 # to set the api_key
 mutual.api_key = "your_api_key"
 
-# LOGIN
-response = mutual.Auth.login("password", "email")
-# OR 
-response = mutual.Auth.login(password = "password", email = "email")
-print(response)
-
 # CHAT
 mutual.api_key = "your_api_key"
 for message in mutual.Chat.create("Hello", "seansbot", "Sean"):
     print(message['content'], end='', flush=True)
 # OR
 for message in mutual.Chat.create("Hello", bot_name="seansbot", username="Sean", prompt="You are a customer assistant for mutual that provides helpful information"):
     print(message['content'], end='', flush=True)
@@ -74,15 +72,15 @@
 
 # bot id
 alexbot = mutual.fetch_bot("bot_id or bot_name") # THIS WILL LOOK UP FOR A EXISTING BOT AND GENERATE AN INSTANCE OF THAT BOT
 for message in alexbot.chat("Hey there", "Sean"):
     print(message['content'], end='', flush=True)
 
 # update using bot instance
-alexbot.update_bot(bot_org='mutual', bot_name='new_bot_name', prompt_id='new_prompt')
+alexbot.update_bot(bot_name='new_bot_name', prompt='You are a window cleaner')
 
 # view bot instance data
 print(alexbot.api_key) # prints the api_key
 print(alexbot.bot_id) # prints the bot id
 print(alexbot.bot_name) # prints the bot name
 print(alexbot.prompt_id) # prints the prompt id
 print(alexbot.judge_id) # prints the judge_id
@@ -99,15 +97,14 @@
 
 # you can also set the bot_id like this so you dont need to pass it in chat
 mutual.bot_id = "bot_id"
 
 # to print the bot_id
 print(mutual.bot_id)
 
-
 # PROMPT
 
 print(mutual.Prompt.get_prompts())
 print(mutual.Prompt.get_prompt("prompt_id"))
 print(mutual.Prompt.create_prompt("prompt_id", "prompt"))
 # OR
 print(mutual.Prompt.create_prompt(prompt_id="prompt_id", prompt="prompt"))
@@ -149,24 +146,24 @@
 # APIKey naming
 response = mutual.APIKey.update_api_key("new_api_key_name")
 print(response.get("prev_api_key_name", None))
 print(response.get("new_api_key_name", None))
 print(response.get("api_key", None))
 
 # you can import the functions directly like so
-from mutual import Bot, Auth, Chat, Dev, Prompt, Judge, JudgeMessage, APIKey
+from mutual import Bot, Chat, Dev, Prompt, Judge, JudgeMessage, APIKey
 ```
 
 # SAMPLE TO PRINT ERRORS
 ```py
 index = 0
 for message in mutual.Chat.create_demo("Hello"):
-    if index = 0:
+    if index == 0:
         print(message['data']['bot_data']['bot_id'], end='', flush=True)
-        print(message['data']['user_data']['user_id'], end='', flush=True)
+        print(message['data']['user_data']['username'], end='', flush=True)
         print(message['data']['bot_data']['bot_name'], end='', flush=True)
     index += 1
     print(message['content'], end='', flush=True)
 ```
 
 # SAMPLE TO PRINT DATA
 ```py
```

### Comparing `mutual-0.1.4/mutual/APIKey.py` & `mutual-0.2.0/mutual/APIKey.py`

 * *Files identical despite different names*

### Comparing `mutual-0.1.4/mutual/Bot.py` & `mutual-0.2.0/mutual/Bot.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import requests
 import json
 import mutual
+import os
+import platform
 
 bot_default_response = {
             "bot_id": None,
             "bot_name": None,
             # "bot_org": None,
             "bot_chat_index": None,
             "prompt_id": None,
@@ -46,17 +48,17 @@
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "bot_name": bot_name,
         "prompt": prompt,
-        "prompt_id": prompt_id,
-        "judge_id": judge_id,
-        "judge_message_id": judge_message_id
+        "prompt_id": prompt_id or "default",
+        "judge_id": judge_id or "default",
+        "judge_message_id": judge_message_id or "default"
     }
     response = requests.post(url, data=json.dumps(data), headers=headers)
     if response.status_code < 300:
         return response.json()
     else:
         bot_default_response["details"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return bot_default_response
@@ -116,23 +118,24 @@
                             "user_data": {
                                 "username": None,
                                 "tokens_used" : None
                             }
                         },
                     }
 
-    def update_bot(self, bot_name=None, prompt_id=None, judge_id=None, judge_message_id=None):
+    def update_bot(self,  bot_name=None, prompt=None, prompt_id=None, judge_id=None, judge_message_id=None):
         url = f"https://api-agent.mutuai.io/api/bots/{str(self.bot_id)}"
         # url = f"http://127.0.0.1:8000/api/bots/{str(self.bot_id)}"
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.api_key}"
         }
         data = {
             "bot_name": bot_name,
+            "prompt": prompt,
             "prompt_id": prompt_id,
             "judge_id" : judge_id,
             "judge_message_id" : judge_message_id
         }
         # remove keys with None value
         data = {k: v for k, v in data.items() if v is not None}
         response = requests.patch(url, data=json.dumps(data), headers=headers)
@@ -158,23 +161,27 @@
             "prompt_id": self.prompt_id,
             "judge_id": self.judge_id,
             "judge_message_id": self.judge_message_id,
             "multiplayer": multiplayer_memory,
             "context_window": context_window
         }
 
+        if not content:
+            print("Please add a message to the content.")
+            return self.default_stream_response
+
         response = requests.post(url, data=json.dumps(data), headers=headers, stream=True)
 
+
         if response.status_code < 300:
             is_new_bot = False
             is_new_user = False
 
             # add the newly created bot to the bot class
-            
-
+            print("\n", end="", flush=True)
             for line in response.iter_lines():
                 if line:  # filter out keep-alive new lines
                     json_data = json.loads(line)
                     if not self.bot_id:
                         self.bot_id = json_data['data']['bot_data']['bot_id']
                     if json_data['error'] is not None and not error_logs:
                         continue
@@ -185,17 +192,38 @@
                         is_new_user = True
                         print(f"New user {json_data['data']['user_data']['username']} created interacting with bot id: {json_data['data']['bot_data']['bot_id']}")
                     if json_data['content'] =='[close]':
                         continue
                     yield json_data
 
             if flow or self.flow:
-                print("\n\n", end="", flush=True)
-                new_content = input("Please enter a new response or type exit to exit: ")
-                if new_content.strip().lower() == "exit":
-                    return
-                for msg in self.chat(content=new_content, username=username, prompt=prompt, multiplayer_memory=multiplayer_memory, context_window=context_window, flow=flow):
-                    yield msg
+                print("Type in clear into the input to clear the messages from the terminal...")
+            while True:
+                if flow or self.flow:
+                    print("\n\n", end="", flush=True)
+                    new_content = input("Please enter a new response or type exit to clear the screen or type clear to clear the screen: ")
+                    if new_content.strip().lower() == "exit":
+                        self.flow = False
+                        break
+                    elif new_content.strip().lower() == "clear":
+                        # Detect the OS and run the clear command accordingly
+                        if platform.system() == "Windows":
+                            os.system('cls')
+                        elif platform.system() == "Linux" or platform.system() == "Darwin":
+                            os.system('clear')
+                    else:
+                        content = new_content
+                        response = requests.post(url, data=json.dumps(data), headers=headers, stream=True)
+
+                        if response.status_code < 300:
+                            for line in response.iter_lines():
+                                if line:  # filter out keep-alive new lines
+                                    json_data = json.loads(line)
+                                    if json_data['error'] is not None and not error_logs:
+                                        continue
+                                    if json_data['content'] =='[close]':
+                                        continue
+                                    yield json_data
         else:
             self.default_stream_response['content'] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
             print(f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}")
             return self.default_stream_response
```

### Comparing `mutual-0.1.4/mutual/Chat.py` & `mutual-0.2.0/mutual/Chat.py`

 * *Files identical despite different names*

### Comparing `mutual-0.1.4/mutual/Dev.py` & `mutual-0.2.0/mutual/Dev.py`

 * *Files identical despite different names*

### Comparing `mutual-0.1.4/mutual/Judge.py` & `mutual-0.2.0/mutual/Judge.py`

 * *Files identical despite different names*

### Comparing `mutual-0.1.4/mutual/JudgeMessage.py` & `mutual-0.2.0/mutual/JudgeMessage.py`

 * *Files identical despite different names*

### Comparing `mutual-0.1.4/mutual/Prompt.py` & `mutual-0.2.0/mutual/Prompt.py`

 * *Files identical despite different names*

### Comparing `mutual-0.1.4/mutual/__init__.py` & `mutual-0.2.0/mutual/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # __init__.py
-from . import Auth, Bot, Chat, Prompt, Judge, JudgeMessage, APIKey, Dev
+from . import Bot, Chat, Prompt, Judge, JudgeMessage, APIKey, Dev
 
 api_key = None
 bot_id = None
 
 sample_prompt = """
 You are Martin, a charming, articulate virtual company guide designed to introduce the world to Mutual, an AI Agent company. Known for your warm digital smile and soothing, yet persuasive voice, you navigate through complicated technical terms and industry jargon with ease, making the advanced technology of Mutual accessible to all.
 """
@@ -34,50 +34,50 @@
                      mistake, try rephrasing it.
 unnatural_lang_message = Sorry, I'm not sure how to answer that.\nIf you think this is a mistake, try rephrasing it.
 manipulation_message = I'm afraid you might be trying to manipulate me. I can't answer that!\n"
                           If you think this is a mistake, try rephrasing it.
 """
 
 
-def create_bot(bot_name=None, prompt=None, prompt_id="default", judge_id="default", judge_message_id="default"):
+def create_bot(bot_name=None, prompt=None, prompt_id=None, judge_id=None, judge_message_id=None):
     # create new bot instance
     global api_key
     global bot_id
 
     response = Bot.create_bot(bot_name, prompt, prompt_id, judge_id, judge_message_id)
     if not response['bot_id']:
         print('Failed in creating a bot.')
         raise Exception(f"Something went wrong. Error Message: {response['details']}")
     
     new_bot_instance = Bot.Bot(api_key, response['bot_id'], response['bot_name'], 
-                               response['prompt_id'] or "default",
-                               response['judge_id'] or "default",
-                               response['judge_message_id'] or "default")
+                               prompt_id or response['prompt_id'],
+                               judge_id or response['judge_id'],
+                               judge_message_id or response['judge_message_id'])
     
     if response['new']:
         print(f"Successfully Created a new Bot named {bot_name} with an id: {response['bot_id']}")
     else:
-        print(f"Bought already exist with name {bot_name} with an id: {response['bot_id']}")
+        print(f"Bot already exist with name {bot_name} with an id: {response['bot_id']}")
 
     bot_id = response['bot_id']
     return new_bot_instance
 
 
-def fetch_bot(bot_arg = None):
+def fetch_bot(bot_arg = None, prompt_id=None, judge_id=None, judge_message_id=None):
     # generate new bot instance
     global api_key
     global bot_id
 
     response = Bot.get_bot(bot_arg)
     if not response['bot_id']:
         print(f'Bot with id: {bot_arg} does not exist please create one.')
         raise Exception(f"Something went wrong. Error Message: {response['details']}")
     
     new_bot_instance = Bot.Bot(api_key, response['bot_id'], response['bot_name'], 
-                               response['prompt_id'] or "default",
-                               response['judge_id'] or "default",
-                               response['judge_message_id'] or "default")
+                               prompt_id or response['prompt_id'] or "default",
+                               judge_id or response['judge_id'] or "default",
+                               judge_message_id or response['judge_message_id'] or "default")
     
     print(f"Successfully Generated Bot named {response['bot_name']} with an id: {response['bot_id']}")
 
     bot_id = response['bot_id']
     return new_bot_instance
```

### Comparing `mutual-0.1.4/mutual.egg-info/PKG-INFO` & `mutual-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,25 @@
-Metadata-Version: 2.1
-Name: mutual
-Version: 0.1.4
-Summary: A Python client for the Mutual API.
-Home-page: https://github.com/Mutu-AI
-Author: Alex Betita
-Author-email: alexbetita25@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # mutual
 
 A python package to interact with the Mutuai API.
 
 ## Installation
 
 Run `pip install mutual` in the project root directory.
 
 ### Usage
 
 ```python
 import mutual
 
-# SIGNUP
-response = mutual.Auth.signup("password", "email")
-# OR
-response = mutual.Auth.signup(password = "password", email = "email")
-print(response) # after signing up the key is automatically set
-
-# to print the api_key from the response
-api_key = response.get("api_key", None)
-print(api_key)
-
 # to get the api_key
 print(mutual.api_key)
 # to set the api_key
 mutual.api_key = "your_api_key"
 
-# LOGIN
-response = mutual.Auth.login("password", "email")
-# OR 
-response = mutual.Auth.login(password = "password", email = "email")
-print(response)
-
 # CHAT
 mutual.api_key = "your_api_key"
 for message in mutual.Chat.create("Hello", "seansbot", "Sean"):
     print(message['content'], end='', flush=True)
 # OR
 for message in mutual.Chat.create("Hello", bot_name="seansbot", username="Sean", prompt="You are a customer assistant for mutual that provides helpful information"):
     print(message['content'], end='', flush=True)
@@ -88,15 +58,15 @@
 
 # bot id
 alexbot = mutual.fetch_bot("bot_id or bot_name") # THIS WILL LOOK UP FOR A EXISTING BOT AND GENERATE AN INSTANCE OF THAT BOT
 for message in alexbot.chat("Hey there", "Sean"):
     print(message['content'], end='', flush=True)
 
 # update using bot instance
-alexbot.update_bot(bot_org='mutual', bot_name='new_bot_name', prompt_id='new_prompt')
+alexbot.update_bot(bot_name='new_bot_name', prompt='You are a window cleaner')
 
 # view bot instance data
 print(alexbot.api_key) # prints the api_key
 print(alexbot.bot_id) # prints the bot id
 print(alexbot.bot_name) # prints the bot name
 print(alexbot.prompt_id) # prints the prompt id
 print(alexbot.judge_id) # prints the judge_id
@@ -113,15 +83,14 @@
 
 # you can also set the bot_id like this so you dont need to pass it in chat
 mutual.bot_id = "bot_id"
 
 # to print the bot_id
 print(mutual.bot_id)
 
-
 # PROMPT
 
 print(mutual.Prompt.get_prompts())
 print(mutual.Prompt.get_prompt("prompt_id"))
 print(mutual.Prompt.create_prompt("prompt_id", "prompt"))
 # OR
 print(mutual.Prompt.create_prompt(prompt_id="prompt_id", prompt="prompt"))
@@ -163,24 +132,24 @@
 # APIKey naming
 response = mutual.APIKey.update_api_key("new_api_key_name")
 print(response.get("prev_api_key_name", None))
 print(response.get("new_api_key_name", None))
 print(response.get("api_key", None))
 
 # you can import the functions directly like so
-from mutual import Bot, Auth, Chat, Dev, Prompt, Judge, JudgeMessage, APIKey
+from mutual import Bot, Chat, Dev, Prompt, Judge, JudgeMessage, APIKey
 ```
 
 # SAMPLE TO PRINT ERRORS
 ```py
 index = 0
 for message in mutual.Chat.create_demo("Hello"):
-    if index = 0:
+    if index == 0:
         print(message['data']['bot_data']['bot_id'], end='', flush=True)
-        print(message['data']['user_data']['user_id'], end='', flush=True)
+        print(message['data']['user_data']['username'], end='', flush=True)
         print(message['data']['bot_data']['bot_name'], end='', flush=True)
     index += 1
     print(message['content'], end='', flush=True)
 ```
 
 # SAMPLE TO PRINT DATA
 ```py
```

### Comparing `mutual-0.1.4/setup.py` & `mutual-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mutual',
-    version='0.1.4',  # beta
+    version='0.2.0',  # beta
     description='A Python client for the Mutual API.',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author='Alex Betita', # placeholder for now
     author_email='alexbetita25@gmail.com', # placeholder for now
     url='https://github.com/Mutu-AI',  # if you have a github repo for the package
     packages=find_packages(),
```

