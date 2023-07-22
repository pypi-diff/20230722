# Comparing `tmp/zundamonai-streamer-2.0.1.tar.gz` & `tmp/zundamonai-streamer-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zundamonai-streamer-2.0.1.tar", last modified: Sat Jul  1 21:34:59 2023, max compression
+gzip compressed data, was "zundamonai-streamer-3.0.0.tar", last modified: Sat Jul 22 16:47:43 2023, max compression
```

## Comparing `zundamonai-streamer-2.0.1.tar` & `zundamonai-streamer-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-07-01 21:34:59.415040 zundamonai-streamer-2.0.1/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-06-05 06:55:47.000000 zundamonai-streamer-2.0.1/LICENSE
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     7651 2023-07-01 17:54:59.000000 zundamonai-streamer-2.0.1/LICENSE_ffmpeg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      658 2023-07-01 21:34:59.415040 zundamonai-streamer-2.0.1/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     8475 2023-07-01 17:54:59.000000 zundamonai-streamer-2.0.1/README.md
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-07-01 21:34:59.415040 zundamonai-streamer-2.0.1/setup.cfg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1197 2023-07-01 21:27:02.000000 zundamonai-streamer-2.0.1/setup.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-07-01 21:34:59.415040 zundamonai-streamer-2.0.1/src/
--rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     5946 2023-07-01 17:54:59.000000 zundamonai-streamer-2.0.1/src/ZundamonAIStreamer.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     3966 2023-07-01 17:54:59.000000 zundamonai-streamer-2.0.1/src/ZundamonAIStreamerManager.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)    16934 2023-07-01 17:54:59.000000 zundamonai-streamer-2.0.1/src/ZundamonAIStreamerUI.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      134 2023-07-01 21:27:15.000000 zundamonai-streamer-2.0.1/src/__init__.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-07-01 21:34:59.415040 zundamonai-streamer-2.0.1/src/zundamonai_streamer.egg-info/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      658 2023-07-01 21:34:59.000000 zundamonai-streamer-2.0.1/src/zundamonai_streamer.egg-info/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      424 2023-07-01 21:34:59.000000 zundamonai-streamer-2.0.1/src/zundamonai_streamer.egg-info/SOURCES.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-07-01 21:34:59.000000 zundamonai-streamer-2.0.1/src/zundamonai_streamer.egg-info/dependency_links.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-07-01 17:54:59.000000 zundamonai-streamer-2.0.1/src/zundamonai_streamer.egg-info/not-zip-safe
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       90 2023-07-01 21:34:59.000000 zundamonai-streamer-2.0.1/src/zundamonai_streamer.egg-info/requires.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       75 2023-07-01 21:34:59.000000 zundamonai-streamer-2.0.1/src/zundamonai_streamer.egg-info/top_level.txt
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-07-22 16:47:43.544236 zundamonai-streamer-3.0.0/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-06-05 06:55:47.000000 zundamonai-streamer-3.0.0/LICENSE
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     7651 2023-07-01 17:54:59.000000 zundamonai-streamer-3.0.0/LICENSE_ffmpeg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      630 2023-07-22 16:47:43.544236 zundamonai-streamer-3.0.0/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     9463 2023-07-22 13:52:11.000000 zundamonai-streamer-3.0.0/README.md
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-07-22 16:47:43.544236 zundamonai-streamer-3.0.0/setup.cfg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1197 2023-07-18 14:14:25.000000 zundamonai-streamer-3.0.0/setup.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-07-22 16:47:43.544236 zundamonai-streamer-3.0.0/src/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)    14797 2023-07-22 07:42:33.000000 zundamonai-streamer-3.0.0/src/TransparentViewer.py
+-rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     5946 2023-07-01 17:54:59.000000 zundamonai-streamer-3.0.0/src/ZundamonAIStreamer.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     3966 2023-07-01 17:54:59.000000 zundamonai-streamer-3.0.0/src/ZundamonAIStreamerManager.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)    23967 2023-07-22 07:24:46.000000 zundamonai-streamer-3.0.0/src/ZundamonAIStreamerUI.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      167 2023-07-18 14:13:53.000000 zundamonai-streamer-3.0.0/src/__init__.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-07-22 16:47:43.544236 zundamonai-streamer-3.0.0/src/zundamonai_streamer.egg-info/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      630 2023-07-22 16:47:43.000000 zundamonai-streamer-3.0.0/src/zundamonai_streamer.egg-info/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      449 2023-07-22 16:47:43.000000 zundamonai-streamer-3.0.0/src/zundamonai_streamer.egg-info/SOURCES.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-07-22 16:47:43.000000 zundamonai-streamer-3.0.0/src/zundamonai_streamer.egg-info/dependency_links.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-07-22 13:53:47.000000 zundamonai-streamer-3.0.0/src/zundamonai_streamer.egg-info/not-zip-safe
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       90 2023-07-22 16:47:43.000000 zundamonai-streamer-3.0.0/src/zundamonai_streamer.egg-info/requires.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       93 2023-07-22 16:47:43.000000 zundamonai-streamer-3.0.0/src/zundamonai_streamer.egg-info/top_level.txt
```

### Comparing `zundamonai-streamer-2.0.1/LICENSE` & `zundamonai-streamer-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zundamonai-streamer-2.0.1/LICENSE_ffmpeg` & `zundamonai-streamer-3.0.0/LICENSE_ffmpeg`

 * *Files identical despite different names*

### Comparing `zundamonai-streamer-2.0.1/PKG-INFO` & `zundamonai-streamer-3.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: zundamonai-streamer
-Version: 2.0.1
+Version: 3.0.0
 Summary: Zundamon with ChatGPT brain answers aloud YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStreamer
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 License-File: LICENSE_ffmpeg
-
-UNKNOWN
-
```

### Comparing `zundamonai-streamer-2.0.1/README.md` & `zundamonai-streamer-3.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -7,25 +7,24 @@
 - This Application is Japanese only since it's depend on Japanese voice engine "VOICEVOX", but You can cutomize by modifying MIT liccenced source codes.
 
 ## This application works on
 - Windows OS (tested on Windows 10)
 - .Net Framework v.4 (tested on v4.7.2)
 - the machine on which installed [VOICEVOX](https://voicevox.hiroshiba.jp/) (tested on v.0.14.6)
 
-    Core Module is implemented by Python, so it can adapt to other OS or voice generators.<br>
-    Only avatar image viewer heavily depends on Windows since its codes are written in C#. I have a plan to replace the codes to python in order to be available on other several platforms.
+    Core Module is implemented by Python, so it can adapt to other OS or voice generators.
 <br><br>
 
 ## This application can
 - automatically pick up messages from YouTube chat and make Zundamon speak the GPT answer of those messages out. <br>
 Thogh non Japanese messages are given, Zundamon answers in Japanese.
 - display all comments of YouTube chat, picked up comments, answers of picked up comments.
 - display Zundamon portrait with transparent background.
 - You can use not only Zundamon voice and image but also other ones. <br>
-[![GttsAIStreamer sample](ReadMeParts/zundamon_thumbnail.png)](https://www.youtube.com/embed/7GgssTTo2-c)
+[![ZundamonAIStreamer sample](ReadMeParts/zundamon_thumbnail.png)](https://www.youtube.com/embed/wpTGk_0Yf3M)
 
 ## Usage
 - Install [VOICEVOX](https://voicevox.hiroshiba.jp/)
 - Get OpenAI api-key. Please refer [here(English)](https://www.howtogeek.com/885918/how-to-get-an-openai-api-key/) or [here(Japanese)](https://laboratory.kazuuu.net/how-to-get-an-openai-api-key/)
 - if you want to launch from .exe file.
     - click [here](https://github.com/GeneralYadoc/ZundamonGPTonYouTube/releases) to download newest version.
     - Unzip Downloaded "ZundamonGPTonYouTube.zip" file.
@@ -116,69 +115,110 @@
     It's necessary for generating Zundamon voices, so please don't close the window. (please minimize if you want to hide it.)<br>
     ![](ReadMeParts/voicevox_window.png)<br>
 <br><br>
 
 # Settings
 
 You can customize the application with "setting.yaml" which is exist in the same layer of the application exe file.
+
 ```setting.yaml
 # VoiceVoxの設定
 voicevox_path: ''
 
-# チャット欄ウインドウの設定
-display_user_name_on_chat_window: 'True'
+# チャット欄ウィンドウの設定
+display_user_name_on_chat_window: true
 chat_window_title: 'ちゃっとらん'
-chat_window_size: '350x754'
-chat_window_padx : '9'
-chat_window_pady : '9'
+chat_window_padx : 9
+chat_window_pady : 9
 chat_window_color: '#ffffff'
 chat_font_color: '#000000'
-chat_font_size: '10'
+chat_font_size: 10
 chat_font_type: 'Courier'
 chat_rendering_method: 'normal'
 
-# 質問ウインドウの設定
-display_user_name_on_ask_window: 'False'
+# 質問ウィンドウの設定
+display_user_name_on_ask_window: false
 ask_window_title: 'ぐみんのしつもん'
-ask_window_size: '500x250'
-ask_window_padx : '9'
-ask_window_pady : '9'
+ask_window_padx : 9
+ask_window_pady : 9
 ask_window_color: '#354c87'
 ask_font_color: '#ffe4fb'
-ask_font_size: '12'
+ask_font_size: 12
 ask_font_type: 'Courier'
 ask_rendering_method: 'refresh'
 
-# 回答ウインドウの設定
+# 回答ウィンドウの設定
 answer_window_title: 'てんさいずんだもんのこたえ'
-answer_window_size: '500x450'
-answer_window_padx : '9'
-answer_window_pady : '9'
+answer_window_padx : 9
+answer_window_pady : 9
 answer_window_color: '#ffe4e0'
 answer_font_color: '#004cF7'
-answer_font_size: '13'
+answer_font_size: 13
 answer_font_type: 'Helvetica'
 answer_rendering_method: 'incremental'
 
+# 立ち絵ウインドウの設定
+image_window_title: '立ち絵'
+image_window_refresh_rate: 30
+image_window_transparent_color: '#00ff00'
+image_window_font_color: '#0000ff'
+image_window_font_size: 11
+image_window_font_type: 'Helvetica'
+image_window_label: 'ダブルクリックで\n背景透過/非透過を\n切り替えられます'
+
 # AIの設定
 model: 'gpt-3.5-turbo'
 max_tokens_per_request: 1024
 ask_interval_sec: 20.0
 
 # 回答キャラクターの設定
 speaker_type: 1
 volume: 100
 system_role: 'あなたはユーザーとの会話を楽しく盛り上げるために存在する、日本語話者の愉快なアシスタントです。'
-image_file: zundamon.gif
 ```
 
 - "voicevox_path" can remain blank if VOICEVOX has been installed to default path.
 - You can change AI model by changing "model" value.
 - You can change voice actor by changing "speaker_type" value.
 - You can change Avatar image by changing "image_file" path.
+
+<br>
+Current size and position, frame visibility, bagckground transparency of these windows is memorized and inherited to them in next time of executing.<br>
+They are recorded in "variable_cache.yaml". you can change window size and position also by editing the file when the application is not running.
+
+``` variable_cache.yaml
+answer_frame_visible: false
+answer_window_height: 450
+answer_window_visible: true
+answer_window_width: 500
+answer_window_x: 659
+answer_window_y: 521
+api_key: XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
+ask_frame_visible: false
+ask_window_height: 250
+ask_window_visible: true
+ask_window_width: 500
+ask_window_x: 663
+ask_window_y: 224
+chat_frame_visible: false
+chat_window_height: 754
+chat_window_visible: true
+chat_window_width: 350
+chat_window_x: 246
+chat_window_y: 225
+image_bg_visible: false
+image_window_height: 816
+image_window_visible: true
+image_window_width: 522
+image_window_x: 1234
+image_window_y: 175
+video_id: XXXXXXXXXXX
+```
+
+
 <br><br>
 # Licence
 - The lisence type of this application is MIT, so you can customize freely.
 - the lisence type of ffmeg executable files included in release package is LGPL.
 <br><br>
 # Links
 - [Pixiv page of 坂本アヒル](https://www.pixiv.net/users/12147115) &emsp; I obtained static Zundamon portrait which is the material of the gif animation from here.
```

### Comparing `zundamonai-streamer-2.0.1/setup.py` & `zundamonai-streamer-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
     name="zundamonai-streamer",
-    version="2.0.1",
+    version="3.0.0",
     license="MIT",
     description="Zundamon with ChatGPT brain answers aloud YouTube chat messages.",
     author="General Yadoc",
     author_email="133023047+GeneralYadoc@users.noreply.github.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
```

### Comparing `zundamonai-streamer-2.0.1/src/ZundamonAIStreamer.py` & `zundamonai-streamer-3.0.0/src/ZundamonAIStreamer.py`

 * *Files identical despite different names*

### Comparing `zundamonai-streamer-2.0.1/src/ZundamonAIStreamerManager.py` & `zundamonai-streamer-3.0.0/src/ZundamonAIStreamerManager.py`

 * *Files identical despite different names*

### Comparing `zundamonai-streamer-2.0.1/src/ZundamonAIStreamerUI.py` & `zundamonai-streamer-3.0.0/src/TransparentViewer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,409 +1,367 @@
-from dataclasses import dataclass
-import ZundamonAIStreamerManager as zm
+from importlib.resources import path
+from PIL import Image, ImageTk
 import sys
 import os
-import math
 import time
 import yaml
-import queue
-import subprocess
+import multiprocessing
 import tkinter as tk
 import tkinter.font as font
 
-@dataclass
-class messageSlot():
-  message: str
-  refresh: bool
-
-class ZundamonAIStreamerUI:
-  def __createStartWindow(self):
-    self.__root.geometry('336x120')
-    self.__root.title('なんでもこたえてくれるずんだもん')
-
-    self.__clearStartWindow()
-    self.__widgits_start["video_id_label"] = tk.Label(text='Video ID')
-    self.__widgits_start["video_id_label"].place(x=30, y=15)
-    self.__widgits_start["video_id_entry"] = tk.Entry(width=32)
-    self.__widgits_start["video_id_entry"].place(x=90, y=15)
-
-    self.__widgits_start["api_key_label"] = tk.Label(text='API Key')
-    self.__widgits_start["api_key_label"].place(x=30, y=48)
-    self.__widgits_start["api_key_entry"] = tk.Entry(width=32)
-    self.__widgits_start["api_key_entry"].place(x=90, y=48)
-
-    self.__widgits_start["button"] = tk.Button(self.__root, text="すたーと", command=self.__start)
-    self.__widgits_start["button"].place(x=143, y=80)
-
-  def __clearStartWindow(self):
-    for widgit in self.__widgits_start.values():
-      widgit.destroy()
-    self.__widgits_start.clear()
-
-  def __createMainWindow(self):
-    self.__root.geometry('336x120')
-    self.__root.title('めいんういんどう')
-    self.__root.iconbitmap(default = self.__icon)
+multiprocessing.freeze_support()
+class TransparentViewer(multiprocessing.Process):
+  def __refresh_image(self):
+    self.__img_params["base_image"].seek(self.__img_params["cur_frame_index"])
+    if self.__root.winfo_width() * self.__img_params["base_image"].height / self.__img_params["base_image"].width > self.__root.winfo_height():
+      new_image_width = self.__root.winfo_height() * self.__img_params["base_image"].width / self.__img_params["base_image"].height
+      new_image_height = self.__root.winfo_height()
+    else:
+      new_image_height = self.__root.winfo_width() * self.__img_params["base_image"].height / self.__img_params["base_image"].width
+      new_image_width = self.__root.winfo_width()
 
-    self.__clearMainWindow()
-    self.__widgits_main["buttonChat"] = tk.Button(self.__root, text="ちゃっと", width="6", command=lambda:self.__changeVisible("chat"))
-    self.__widgits_main["buttonChat"].place(x=30, y=20)
-
-    self.__widgits_main["buttonAsk"] = tk.Button(self.__root, text="しつもん", width="6", command=lambda:self.__changeVisible("ask"))
-    self.__widgits_main["buttonAsk"].place(x=104, y=20)
-
-    self.__widgits_main["buttonAnswer"] = tk.Button(self.__root, text="こたえ", width="6", command=lambda:self.__changeVisible("answer"))
-    self.__widgits_main["buttonAnswer"].place(x=178, y=20)
-
-    self.__widgits_main["buttonPortrait"] = tk.Button(self.__root, text="立ち絵", width="6", command=self.__changeVisiblePortrait)
-    self.__widgits_main["buttonPortrait"].place(x=252, y=20)
-
-    self.__widgits_main["volumeLabel"] = tk.Label(text='volume')
-    self.__widgits_main["volumeLabel"].place(x=27, y=70)
-    self.__widgits_main["scaleVolume"] = tk.Scale( self.__root,
-                                                   variable = tk.DoubleVar(),
-                                                   command = self.__changeVolume,
-                                                   orient=tk.HORIZONTAL,
-                                                   sliderlength = 20,
-                                                   length = 200,
-                                                   from_ = 0,
-                                                   to = 500,
-                                                   resolution=5,
-                                                   tickinterval=250 )
-
-    self.__widgits_main["scaleVolume"].set(self.__initial_volume)
-    self.__widgits_main["scaleVolume"].place(x=72, y=50)
-
-    self.__widgits_main["volumeEntry"] = tk.Entry(width=3, justify=tk.RIGHT)
-    self.__widgits_main["volumeEntry"].bind(sequence="<Return>", func=self.__scaleVolume)
-    self.__widgits_main["volumeEntry"].place(x=282, y=70)
-
-    self.__receiveMessage()
-
-  def __clearMainWindow(self):
-    for widgit in self.__widgits_main.values():
-      widgit.destroy()
-    self.__widgits_main.clear()
-
-  def __createMessageWindow(self, key):
-    window = tk.Toplevel()
-    window.title(self.__sub_window_settings[key]["title"])
-    window.geometry(self.__sub_window_settings[key]["window_size"])
-    window.protocol("WM_DELETE_WINDOW", lambda:self.__changeVisible(key))
-    
-    frame = tk.Frame(window)
-    frame.pack(fill = tk.BOTH)
+    self.__canvas.delete("image")
+
+    self.__img_params["resized_image"] = self.__img_params["base_image"].resize([int(new_image_width), int(new_image_height)], Image.Resampling.HAMMING)    
+    self.__img_params["photo_image"] = ImageTk.PhotoImage(self.__img_params["resized_image"])
+    self.__canvas.configure(width=self.__root.winfo_width(), height=self.__root.winfo_height())
+    self.__canvas.create_image( (self.__root.winfo_width() - new_image_width) / 2,
+                                (self.__root.winfo_height() - new_image_height) / 2,
+                                image=self.__img_params["photo_image"], anchor=tk.NW,
+                                tag="image" )
+
+  def __refresh_text(self):
+    self.__canvas.delete("text")
+
+    if (self.__txt_params["visible"]):
+      self.__canvas.create_text( self.__root.winfo_width(),
+                                 self.__root.winfo_height(),
+                                 text=self.__txt_params["text"],
+                                 font=font.Font(size=str(self.__txt_params["font_size"]), family=self.__txt_params["font_type"], weight="bold"),
+                                 anchor=tk.SE, justify=tk.RIGHT,
+                                 fill=self.__txt_params["font_color"],
+                                 tag="text" )
+
+  def __refresh_canvas(self):
+    self.__refresh_image()
+    self.__refresh_text()
+
+  def __show_frames(self):
+    cur_time = time.time()
+    offset_time_ms = int((time.time() - self.__start_time) * 1000)
+    rest_time_ms = offset_time_ms % self.__img_params["total_time_ms"]
+
+    frame_index = i = 0
+    while (rest_time_ms > 0 and i < self.__img_params["base_image"].n_frames - 1):
+      frame_index = i
+      rest_time_ms -= self.__img_params["durations"][frame_index]
+      i += 1
+
+    self.__img_params["cur_frame_index"] = frame_index
+
+    self.__refresh_image()
+    window_duration = int(1000 / self.__win_params["refresh_rate"]) - int((cur_time - self.__prev_time) * 1000)
+    min_win_duration = int(667 / self.__win_params["refresh_rate"])
+    min_win_duration = 1 if min_win_duration <= 0 else min_win_duration
+    if window_duration < min_win_duration:
+      window_duration = min_win_duration
+
+    self.__prev_time = cur_time
+    if not self.__img_params["decimated_animation"]:
+      self.__root.after(window_duration, self.__show_frames)
+    else:
+      self.__img_params["decimated_animation"] = False
+      self.__root.after(int(1000 / self.__win_params["refresh_rate"]), self.__show_frames)
 
-    text = tk.Text( frame,
-                    bg=self.__sub_window_settings[key]["window_color"],
-                    fg=self.__sub_window_settings[key]["font_color"],
-                    selectbackground=self.__sub_window_settings[key]["window_color"],
-                    selectforeground=self.__sub_window_settings[key]["font_color"],
-                    width=800,
-                    height=100,
-                    bd="0",
-                    padx=self.__sub_window_settings[key]["window_padx"],
-                    pady=self.__sub_window_settings[key]["window_pady"],
-                    font=font.Font( size=self.__sub_window_settings[key]["font_size"],
-                                    family=self.__sub_window_settings[key]["font_type"],
-                                    weight="bold" ),
-                    state="disabled" )
-
-
-    self.__sub_windows[key] = {
-      "visible" : False,
-      "body" : window,
-      "text" : text,
-      "mouse_position" : [0, 0],
-      "message_queue" : queue.Queue(1000)
-    }
-    self.__sub_windows[key]["body"].bind(sequence="<Button-1>", func=lambda event:self.__clickWindow(key=key, event=event))
-    self.__sub_windows[key]["body"].bind(sequence="<B1-Motion>", func=lambda event:self.__moveWindow(key=key, event=event))
-    self.__sub_windows[key]["body"].bind(sequence="<Double-Button-1>", func=lambda event:self.__doubleclickWindow(key=key, event=event))
-    self.__sub_windows[key]["text"].pack()
-    self.__sub_windows[key]["body"].withdraw()
-
-  def __interruptibleSleep(self, time_sec):
-    counter = math.floor(time_sec / 0.10)
-    frac = time_sec - (counter * 0.10)
-    for i in range(counter):
-      if not self.__running:
-        break
-      time.sleep(0.10)
-    if not self.__running:
-      return
-    time.sleep(frac)
-
-  def __sendMessageCore(self, key, message, refresh):
-    message_queue = self.__sub_windows[key]["message_queue"]
-    if not message_queue.full():
-      slot = messageSlot(message=message, refresh=refresh)
-      message_queue.put(slot)
-
-  def __sendMessage(self, key, name="", message=""):
-    rendering_method = self.__sub_window_settings[key]["rendering_method"]
-    display_name = self.__sub_window_settings[key]["display_name"]
-
-    if display_name == 'True':
-      message = f"[{name}] {message}"
-
-    if rendering_method == "incremental":
-      for i in range(len(message)):
-        refresh = True if i == 0  else False
-        self.__sendMessageCore(key, message[i : i+1], refresh)
-        self.__interruptibleSleep(0.10)
+  def __initialize_duration_info(self):
+    for i in range(self.__img_params["base_image"].n_frames):
+      self.__img_params["base_image"].seek(i)
+      self.__img_params["durations"].append(self.__img_params["base_image"].info["duration"])
+      self.__img_params["total_time_ms"] += self.__img_params["durations"][i]
+
+  def __play_animation(self):
+    if self.__img_params["base_image"].n_frames > 1:
+      self.__initialize_duration_info()
+      self.__start_time = time.time()
+      self.__show_frames()
     else:
-      refresh = True if rendering_method == "refresh" else False
-      if not refresh:
-        message = f"\n{message}\n"
-      self.__sendMessageCore(key, message, refresh)
+      self.__refresh_image()
 
-  def __showMessage(self, text, message, refresh):
-    text.configure(state="normal")
+  def __save_visibility(self, visible):
+    variable_cache = {}
     try:
-      pos = text.index('end')
+      with open(self.__variable_cache_path, 'r') as file:
+        variable_cache = yaml.safe_load(file)
     except:
-      return
-    
-    if refresh:
-      text.delete('1.0', 'end')
-      pos = text.index('end')
-    
-    text.insert(pos, message)
-    text.see("end")
-    text.configure(state="disabled")
- 
-  def __receiveMessage(self):
-    for key in self.__sub_windows.keys():
-      message_queue = self.__sub_windows[key]["message_queue"]
-      text = self.__sub_windows[key]["text"]
-      while not message_queue.empty():
-        slot = message_queue.get()
-        self.__showMessage(text, slot.message, slot.refresh)
+      pass
 
-    self.__root.after(ms=33, func=self.__receiveMessage)
+    variable_cache["image_window_visible"] = visible
 
-  def __init__(self, workspace="./"):
-    self.__running = False
-    self.__variable_cache_path = os.path.join(workspace, "variable_cache.yaml")
-    self.__setting_path = os.path.join(workspace, "setting.yaml")
+    try:
+      with open(self.__variable_cache_path, 'w', encoding='UTF-8') as file:
+        yaml.safe_dump(variable_cache, file)
+    except:
+      pass
 
+  def __apply_visibility(self):
+    if self.__win_params["visible_mem"]:
+      if self.__win_params["visible_mem"].value:
+        cur_visible = True
+      else:
+        cur_visible = False
+    elif self.__win_params["visible"]:
+        cur_visible = True
+    else:
+        cur_visible = False
+
+    if cur_visible and not self.__win_params["prev_visible"]:
+      self.__root.deiconify()
+      self.__save_visibility(True)
+      self.__win_params["prev_visible"] = True
+    elif not cur_visible and self.__win_params["prev_visible"]:
+      self.__root.withdraw()
+      self.__save_visibility(False)
+      self.__win_params["prev_visible"] = False
+
+    self.__root.after(200, self.__apply_visibility)
+
+  def __image_window_is_cached(self):
     variable_cache = {}
     try:
       with open(self.__variable_cache_path, 'r') as file:
         variable_cache = yaml.safe_load(file)
     except:
-      variable_cache["video_id"] = ""
-      variable_cache["api_key"] = ""
-    
+      pass
+
+    return ("image_window_width" in variable_cache or "image_window_height" in variable_cache or
+            "image_window_x" in variable_cache or "image_window_y" in variable_cache)
+
+  def __createImageWindow(self):
+    self.__img_params["base_image"] = Image.open(self.__img_params["path"])
+
+    self.__root.wm_minsize(width=3, height=3)
+    self.__root.title(self.__title)
+    self.__root.iconbitmap(default = self.__icon)
+    if self.__is_client:
+      self.__root.protocol("WM_DELETE_WINDOW", self.__changeVisible)
+    self.__root.bind(sequence="<Configure>", func=lambda event:self.__configureWindow(event=event))
+
+    frame = tk.Frame(self.__root)
+    frame.pack(fill = tk.BOTH)
+
+    self.__canvas = tk.Canvas(bg=self.__transparent_color)
+    self.__canvas.place(x=-2, y=-2)
+
+    default_width = self.__win_params["default_width"]
+    default_height = self.__win_params["default_height"]
+    default_x = self.__win_params["default_x"]
+    default_y = self.__win_params["default_y"]
+
+    if self.__image_window_is_cached():
+      width = default_width
+      height = default_height
+    elif default_width * self.__img_params["base_image"].height / self.__img_params["base_image"].width > default_height:
+      width = default_height * self.__img_params["base_image"].width / self.__img_params["base_image"].height
+      height = default_height
+    else:
+      height = default_width * self.__img_params["base_image"].height / self.__img_params["base_image"].width
+      width = default_width
+
+    x = default_x
+    y = default_y
+
+    self.__root.geometry(f"{int(width)}x{int(height)}+{x}+{y}")
+    self.__root.update()
+    self.__win_params["prev_width"] = self.__root.winfo_width()
+    self.__win_params["prev_height"] = self.__root.winfo_height()
+
+    if not self.__win_params["default_bg_visible"]:
+      self.__root.wm_overrideredirect(True)
+      self.__root.wm_attributes("-transparentcolor", self.__transparent_color)
+
+    if self.__is_client:
+      self.__apply_visibility()
+    self.__play_animation()
+
+    self.__root.bind(sequence="<Button-1>", func=lambda event:self.__clickWindow(event=event))
+    self.__root.bind(sequence="<B1-Motion>", func=lambda event:self.__moveWindow(event=event))
+    self.__root.bind(sequence="<Double-Button-1>", func=lambda event:self.__doubleclickWindow(event=event))
+
+  def __applySettings(self, workspace):
+    settings = {}
     with open(self.__setting_path, 'r', encoding='shift_jis') as file:
       settings = yaml.safe_load(file)
 
-    self.__voicevox_path = settings['voicevox_path']
-
-    self.__sub_window_settings = {}
-    self.__sub_window_settings["chat"] = {}
-    self.__sub_window_settings["chat"]["display_user_name"] = settings["display_user_name_on_chat_window"]
-    self.__sub_window_settings["chat"]["title"] = settings["chat_window_title"]
-    self.__sub_window_settings["chat"]["window_size"] = settings["chat_window_size"]
-    self.__sub_window_settings["chat"]["window_padx"] = settings["chat_window_padx"]
-    self.__sub_window_settings["chat"]["window_pady"] = settings["chat_window_pady"]
-    self.__sub_window_settings["chat"]["window_color"] = settings["chat_window_color"]
-    self.__sub_window_settings["chat"]["font_color"] = settings["chat_font_color"]
-    self.__sub_window_settings["chat"]["font_size"] = settings["chat_font_size"]
-    self.__sub_window_settings["chat"]["font_type"] = settings["chat_font_type"]
-    self.__sub_window_settings["chat"]["rendering_method"] = settings["chat_rendering_method"]
-    self.__sub_window_settings["chat"]["display_name"] = settings["display_user_name_on_chat_window"]
-
-    self.__sub_window_settings["ask"] = {}
-    self.__sub_window_settings["ask"]["display_user_name"] = settings["display_user_name_on_ask_window"]
-    self.__sub_window_settings["ask"]["title"] = settings["ask_window_title"]
-    self.__sub_window_settings["ask"]["window_size"] = settings["ask_window_size"]
-    self.__sub_window_settings["ask"]["window_padx"] = settings["ask_window_padx"]
-    self.__sub_window_settings["ask"]["window_pady"] = settings["ask_window_pady"]
-    self.__sub_window_settings["ask"]["window_color"] = settings["ask_window_color"]
-    self.__sub_window_settings["ask"]["font_color"] = settings["ask_font_color"]
-    self.__sub_window_settings["ask"]["font_size"] = settings["ask_font_size"]
-    self.__sub_window_settings["ask"]["font_type"] = settings["ask_font_type"]
-    self.__sub_window_settings["ask"]["rendering_method"] = settings["ask_rendering_method"]
-    self.__sub_window_settings["ask"]["display_name"] = settings["display_user_name_on_ask_window"]
-
-    self.__sub_window_settings["answer"] = {}
-    self.__sub_window_settings["answer"]["title"] = settings["answer_window_title"]
-    self.__sub_window_settings["answer"]["window_size"] = settings["answer_window_size"]
-    self.__sub_window_settings["answer"]["window_padx"] = settings["answer_window_padx"]
-    self.__sub_window_settings["answer"]["window_pady"] = settings["answer_window_pady"]
-    self.__sub_window_settings["answer"]["window_color"] = settings["answer_window_color"]
-    self.__sub_window_settings["answer"]["font_color"] = settings["answer_font_color"]
-    self.__sub_window_settings["answer"]["font_size"] = settings["answer_font_size"]
-    self.__sub_window_settings["answer"]["font_type"] = settings["answer_font_type"]
-    self.__sub_window_settings["answer"]["rendering_method"] = settings["answer_rendering_method"]
-    self.__sub_window_settings["answer"]["display_name"] = False
-
-    stream_params = zm.streamParams(
-      video_id = variable_cache["video_id"],
-    )
-
-    ai_params = zm.aiParams(
-      api_key = variable_cache["api_key"],
-      model = settings["model"],
-      system_role = settings["system_role"],
-      max_tokens_per_request = settings["max_tokens_per_request"],
-      interval_sec = settings["ask_interval_sec"]
-    )
-
-    volume = (lambda v: 0 if v < 0 else 500 if v > 500 else v)(settings['volume'])
-
-    self.__zm_streamer_params = zm.params( stream_params=stream_params,
-                                           ai_params=ai_params,
-                                           speaker_type = settings["speaker_type"],
-                                           volume=volume,
-                                           send_message_cb=self.__sendMessage )
+    self.__title = settings["image_window_title"]
+    self.__transparent_color = settings["image_window_transparent_color"]
+    self.__win_params["refresh_rate"] = settings["image_window_refresh_rate"]
+    self.__img_params["path"] = os.path.join(workspace, settings["image_file"])
+    self.__txt_params["font_color"] = settings["image_window_font_color"]
+    self.__txt_params["font_size"] = settings["image_window_font_size"]
+    self.__txt_params["font_type"] = settings["image_window_font_type"]
+    self.__txt_params["text"] = settings["image_window_label"]
 
-    self.__manager = None
-    self.__root = tk.Tk()
-    self.__root.resizable(False, False)
-    self.__root.protocol("WM_DELETE_WINDOW", self.__close)
-    self.__initial_volume = volume
-    self.__icon = os.path.join(workspace, "zundamon_icon1.ico")
-    self.__widgits_start = {}
-    self.__widgits_main = {}
-    self.__sub_windows = {}
-    self.__image_command_path = os.path.join(workspace, "TransparentViewer.exe")
-    self.__image_command_args = "-c"
-    self.__portrait_window_process = None
-    self.__portrait_image_file = settings["image_file"]
-    self.__portrait_visible_file_path = os.path.join(workspace, "viewer_visible.txt")
     try:
-      os.remove(self.__portrait_visible_file_path)
+      with open(self.__variable_cache_path, 'r') as file:
+        variable_cache = yaml.safe_load(file)
     except:
       pass
-    self.__createStartWindow()
 
-  def __start(self):
-    self.__running = True
+    if "image_window_width" in variable_cache:
+      self.__win_params["default_width"] = variable_cache["image_window_width"]
+    if "image_window_height" in variable_cache:
+      self.__win_params["default_height"] = variable_cache["image_window_height"]
+    if "image_window_x" in variable_cache:
+      self.__win_params["default_x"] = variable_cache["image_window_x"]
+    if "image_window_y" in variable_cache:
+      self.__win_params["default_y"] = variable_cache["image_window_y"]
+    if "image_bg_visible" in variable_cache:
+      self.__win_params["default_bg_visible"] = variable_cache["image_bg_visible"]
+
+    self.__txt_params["visible"] = self.__win_params["default_bg_visible"]
+
+  def __init__(self, visible_mem=None, is_client=False, workspace="./"):
+    self.__is_client = is_client
+    self.__title = "立ち絵"
+    self.__icon = os.path.join(workspace, "zundamon_icon1.ico")
+    self.__transparent_color = "#00ff00"
+    self.__mouse_position = [0, 0]
+    self.__canvas = None
+    self.__start_time = 0
+    self.__prev_time = 0
+    self.__win_params = {}
+    self.__win_params["default_width"] = 400
+    self.__win_params["default_height"] = 700
+    self.__win_params["prev_width"] = 0
+    self.__win_params["prev_height"] = 0
+    self.__win_params["default_x"] = 50
+    self.__win_params["default_y"] = 50
+    self.__win_params["visible"] = 1
+    self.__win_params["prev_visible"] = not self.__win_params["visible"]
+    self.__win_params["visible_mem"] = None
+    self.__win_params["default_bg_visible"] = True
+    if visible_mem:
+      self.__win_params["visible_mem"] = visible_mem
+      self.__win_params["prev_visible"] = not visible_mem.value
+    self.__win_params["refresh_rate"] = 30
+    self.__img_params = {}
+    self.__img_params["base_image"] = None
+    self.__img_params["resized_image"] = None
+    self.__img_params["photo_image"] = None
+    self.__img_params["path"] = os.path.join(workspace, "Zundamon.gif")
+    self.__img_params["cur_frame_index"] = 0
+    self.__img_params["durations"] = []
+    self.__img_params["total_time_ms"] = 0
+    self.__img_params["decimated_animation"] = False
+    self.__txt_params = {}
+    self.__txt_params["font_color"] = "#0000ff"
+    self.__txt_params["font_size"] = "11"
+    self.__txt_params["font_type"] = "Helvetica"
+    self.__txt_params["visible"] = "True"
+    self.__txt_params["text"] = "ダブルクリックで\n背景透過/非透過を\n切り替えられます"
+    self.__setting_path = os.path.join(workspace, "setting.yaml")
+    self.__variable_cache_path = os.path.join(workspace, "variable_cache.yaml")
+    self.__applySettings(workspace)
+    super(TransparentViewer, self).__init__(daemon=True)
 
-    variables = {}
-    if self.__widgits_start["video_id_entry"].get() == "":
-      variables["video_id"] = self.__zm_streamer_params.stream_params.video_id
-    else:
-      variables["video_id"] = self.__widgits_start["video_id_entry"].get()
-      self.__zm_streamer_params.stream_params.video_id = variables["video_id"]
-    if self.__widgits_start["api_key_entry"].get() == "":
-      variables["api_key"] = self.__zm_streamer_params.ai_params.api_key
-    else:
-      variables["api_key"] = self.__widgits_start["api_key_entry"].get()
-      self.__zm_streamer_params.ai_params.api_key = variables["api_key"]
+  def run(self):
+    self.__root = tk.Tk()
+    self.__createImageWindow()
+    self.__root.mainloop()
 
-    file = open(self.__variable_cache_path, 'w', encoding='UTF-8')
-    yaml.safe_dump(variables, file)
-    file.close()
-
-    self.__root.title("めいんういんどう")
-    self.__clearStartWindow()
-    self.__createMainWindow()
-    self.__createMessageWindow(key = "chat")
-    self.__createMessageWindow(key = "ask")
-    self.__createMessageWindow(key = "answer")
-
-    visible_file_generated = False
-
-    while (not visible_file_generated):
-      try:
-        file = open(self.__portrait_visible_file_path, mode='w')
-      except:
-        continue
-      file.write("false")
-      file.close()
-      visible_file_generated = True
-
-    self.__portrait_window_process = subprocess.Popen(f"{self.__image_command_path} {self.__image_command_args} {self.__portrait_image_file}")
-
-    self.__manager = zm.ZundamonAIStreamerManager(self.__zm_streamer_params)
-    self.__manager.start()
-
-  def __changeVolume(self, event=None):
-    volume = int(self.__widgits_main["scaleVolume"].get())
-    self.__widgits_main["volumeEntry"].delete(0, tk.END)
-    self.__widgits_main["volumeEntry"].insert(0, str(volume))
-    if self.__manager:
-      self.__manager.volume = volume
+  def __changeVisible(self):
+    if self.__win_params["visible_mem"]:
+      if self.__win_params["visible_mem"].value:
+        self.__win_params["visible_mem"].value = False
+      else:
+        self.__win_params["visible_mem"].value = True
+    elif self.__win_params["visible"]:
+      self.__win_params["visible"] = False
+    else:
+      self.__win_params["visible"] = True
 
-  def __scaleVolume(self, event=None):
-    volume_str = self.__widgits_main["volumeEntry"].get()
+  def __clickWindow(self, event):
+    self.__mouse_position[0] = event.x_root
+    self.__mouse_position[1] = event.y_root
+
+  def __moveWindow(self, event):
+    moved_x = event.x_root - self.__mouse_position[0]
+    moved_y = event.y_root - self.__mouse_position[1]
+    self.__mouse_position[0] = event.x_root
+    self.__mouse_position[1] = event.y_root
+    cur_position_x = self.__root.winfo_x() + moved_x
+    cur_position_y = self.__root.winfo_y() + moved_y
+    self.__root.geometry(f"+{cur_position_x}+{cur_position_y}")
+ 
+  def __doubleclickWindow(self, event=None):
+    variable_cache = {}
     try:
-      volume = int(volume_str)
+      with open(self.__variable_cache_path, 'r') as file:
+        variable_cache = yaml.safe_load(file)
     except:
-      return
-    
-    volume = (lambda v: 0 if v < 0 else 500 if v > 500 else v)(volume)
-    
-    self.__widgits_main["volumeEntry"].delete(0, tk.END)
-    self.__widgits_main["volumeEntry"].insert(0, str(volume))
-
-    self.__widgits_main["scaleVolume"].set(volume)
-
-  def __changeVisible(self, key):
-    if self.__sub_windows[key]["visible"]:
-      self.__sub_windows[key]["visible"] = False
-      self.__sub_windows[key]["body"].withdraw()
+      pass
+
+    if self.__root.wm_overrideredirect():
+      new_bg_visible = True
+      self.__canvas.create_text( self.__root.winfo_width(),
+                                 self.__root.winfo_height(),
+                                 text=self.__txt_params["text"],
+                                 font=font.Font(size=str(self.__txt_params["font_size"]), family=self.__txt_params["font_type"], weight="bold"),
+                                 fill=self.__txt_params["font_color"],
+                                 anchor=tk.SE, justify=tk.RIGHT,
+                                 tag="text" )
+      self.__root.wm_attributes("-transparentcolor", "")
+      self.__root.wm_overrideredirect(False)
     else:
-      self.__sub_windows[key]["visible"] = True
-      self.__sub_windows[key]["body"].deiconify()
+      new_bg_visible = False
+      self.__canvas.delete("text")
+      self.__root.wm_attributes("-transparentcolor", self.__transparent_color)
+      self.__root.wm_overrideredirect(True)
+
+    variable_cache["image_bg_visible"] = new_bg_visible
+    self.__txt_params["visible"] = new_bg_visible
 
-  def __changeVisiblePortrait(self):
     try:
-      file = open(self.__portrait_visible_file_path, mode='r')
+      with open(self.__variable_cache_path, 'w', encoding='UTF-8') as file:
+        yaml.safe_dump(variable_cache, file)
     except:
-      self.__root.after(ms=33, func=self.__changeVisiblePortrait)
-      return
-    
-    visible_str = file.readline().splitlines()[0]
-    visible = True if visible_str == "true" else False
+      pass
+
+  def __configureWindow(self, event=None):
+    if self.__img_params["base_image"].n_frames > 1:
+      self.__img_params["decimated_animation"] = True
+    if self.__win_params["prev_width"] != self.__root.winfo_width() or self.__win_params["prev_height"] != self.__root.winfo_height():
+      self.__refresh_canvas()
+      self.__win_params["prev_width"] = self.__root.winfo_width()
+      self.__win_params["prev_height"] = self.__root.winfo_height()
 
+    variable_cache = {}
     try:
-      file = open(self.__portrait_visible_file_path, mode='w')
+      with open(self.__variable_cache_path, 'r') as file:
+        variable_cache = yaml.safe_load(file)
     except:
-      self.__root.after(ms=33, func=self.__changeVisiblePortrait)
-      return
+      pass
+
+    variable_cache["image_window_width"] = self.__root.winfo_width()
+    variable_cache["image_window_height"] = self.__root.winfo_height()
+    variable_cache["image_window_x"] = self.__root.winfo_x()
+    variable_cache["image_window_y"] = self.__root.winfo_y()
 
-    visible = not visible
-    file.write("true" if visible else "false")
-    file.close()
-  
-  def __clickWindow(self, key, event):
-    self.__sub_windows[key]["mouse_position"][0] = event.x_root
-    self.__sub_windows[key]["mouse_position"][1] = event.y_root
-
-  def __moveWindow(self, key, event):
-    moved_x = event.x_root - self.__sub_windows[key]["mouse_position"][0]
-    moved_y = event.y_root - self.__sub_windows[key]["mouse_position"][1]
-    self.__sub_windows[key]["mouse_position"][0] = event.x_root
-    self.__sub_windows[key]["mouse_position"][1] = event.y_root
-    cur_position_x = self.__sub_windows[key]["body"].winfo_x() + moved_x
-    cur_position_y = self.__sub_windows[key]["body"].winfo_y() + moved_y
-    self.__sub_windows[key]["body"].geometry(f"+{cur_position_x}+{cur_position_y}")
-    pass
-  
-  def __doubleclickWindow(self, key, event=None):
-    self.__sub_windows[key]["body"].wm_overrideredirect(not self.__sub_windows[key]["body"].wm_overrideredirect())
-
-  def __close(self):
-    self.__running = False
-
-    if self.__portrait_window_process:
-      self.__portrait_window_process.kill()
-    if self.__manager:
-      self.__manager.disconnect()
-      self.__manager.join()
-    self.__root.destroy()
     try:
-      os.remove(self.__portrait_visible_file_path)
+      with open(self.__variable_cache_path, 'w', encoding='UTF-8') as file:
+        yaml.safe_dump(variable_cache, file)
     except:
       pass
 
-  def mainloop(self):
-    self.__root.mainloop()
-
 if __name__ == "__main__":
-  ui = ZundamonAIStreamerUI(workspace=os.path.abspath(os.path.dirname(sys.argv[0])))
-  ui.mainloop()
+  is_client = False
+  for arg in sys.argv:
+    if arg == "-c":
+      is_client = True
+      break
+
+  manager = multiprocessing.Manager()
+  visible = manager.Value('b', True)
+
+  ui = TransparentViewer(visible=visible, is_client=is_client)
+  ui.start()
+  ui.join()
```

### Comparing `zundamonai-streamer-2.0.1/src/zundamonai_streamer.egg-info/PKG-INFO` & `zundamonai-streamer-3.0.0/src/zundamonai_streamer.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: zundamonai-streamer
-Version: 2.0.1
+Version: 3.0.0
 Summary: Zundamon with ChatGPT brain answers aloud YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStreamer
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 License-File: LICENSE_ffmpeg
-
-UNKNOWN
-
```

