# Comparing `tmp/babymaycry-0.0.5.tar.gz` & `tmp/babymaycry-0.0.6.tar.gz`

## Comparing `babymaycry-0.0.5.tar` & `babymaycry-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 babymaycry-0.0.5/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 babymaycry-0.0.5/src/babymaycry/__init__.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 babymaycry-0.0.5/src/babymaycry/api.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 babymaycry-0.0.5/.gitignore
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 babymaycry-0.0.5/README.md
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 babymaycry-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 babymaycry-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 babymaycry-0.0.6/main.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 babymaycry-0.0.6/src/babymaycry/__init__.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 babymaycry-0.0.6/src/babymaycry/api.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 babymaycry-0.0.6/.gitignore
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 babymaycry-0.0.6/README.md
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 babymaycry-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 babymaycry-0.0.6/PKG-INFO
```

### Comparing `babymaycry-0.0.5/src/babymaycry/api.py` & `babymaycry-0.0.6/src/babymaycry/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,20 @@
         self.bot_token = bot_token
         self.chat_id = chat_id
         self.threshold = threadhold
         self.verbose = verbose
         
     def run(self):
         audio = pyaudio.PyAudio()
-        stream = p.open(format=pyaudio.paInt16,
-                channels=1,
-                rate=44100,
-                input=True,
-                frames_per_buffer=1024)
+        stream = audio.open(
+            format=pyaudio.paInt16,
+            channels=1,
+            rate=44100,
+            input=True,
+            frames_per_buffer=1024)
 
         print("Listening for baby cry...")
 
         while True:
             try:
                 data = stream.read(1024)
                 rms = audioop.rms(data, 2)
```

### Comparing `babymaycry-0.0.5/.gitignore` & `babymaycry-0.0.6/.gitignore`

 * *Files identical despite different names*

