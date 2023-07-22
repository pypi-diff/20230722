# Comparing `tmp/babymaycry-0.0.2.tar.gz` & `tmp/babymaycry-0.0.3.tar.gz`

## Comparing `babymaycry-0.0.2.tar` & `babymaycry-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 babymaycry-0.0.2/src/babymaycry/__init__.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 babymaycry-0.0.2/src/babymaycry/api.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 babymaycry-0.0.2/.gitignore
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 babymaycry-0.0.2/README.md
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 babymaycry-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 babymaycry-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 babymaycry-0.0.3/src/babymaycry/__init__.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 babymaycry-0.0.3/src/babymaycry/api.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 babymaycry-0.0.3/.gitignore
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 babymaycry-0.0.3/README.md
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 babymaycry-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 babymaycry-0.0.3/PKG-INFO
```

### Comparing `babymaycry-0.0.2/src/babymaycry/api.py` & `babymaycry-0.0.3/src/babymaycry/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pyaudio
 import telegram
 
 
-class BabyMaCry:
+class BabyMayCry:
     def __init__(self, bot_token, chat_id):
         self.bot_token = bot_token
         self.chat_id = chat_id
         self.threshold = 1000
         
     def run(self):
         audio = pyaudio.PyAudio()
```

### Comparing `babymaycry-0.0.2/.gitignore` & `babymaycry-0.0.3/.gitignore`

 * *Files identical despite different names*

