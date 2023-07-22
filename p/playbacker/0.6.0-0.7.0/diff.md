# Comparing `tmp/playbacker-0.6.0.tar.gz` & `tmp/playbacker-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playbacker-0.6.0.tar", max compression
+gzip compressed data, was "playbacker-0.7.0.tar", max compression
```

## Comparing `playbacker-0.6.0.tar` & `playbacker-0.7.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1254 2023-06-04 10:56:30.501816 playbacker-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-04 10:55:57.257497 playbacker-0.6.0/src/playbacker/__init__.py
--rw-r--r--   0        0        0     5020 2023-06-04 10:55:57.257497 playbacker-0.6.0/src/playbacker/app.py
--rw-r--r--   0        0        0      527 2023-06-04 10:55:57.257497 playbacker-0.6.0/src/playbacker/config.py
--rw-r--r--   0        0        0        0 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/__init__.py
--rw-r--r--   0        0        0      850 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/audiofile.py
--rw-r--r--   0        0        0     1292 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/clock.py
--rw-r--r--   0        0        0     3423 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/playback.py
--rw-r--r--   0        0        0     1444 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/player.py
--rw-r--r--   0        0        0      974 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/setlist.py
--rw-r--r--   0        0        0     3408 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/settings.py
--rw-r--r--   0        0        0      892 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/song.py
--rw-r--r--   0        0        0     3137 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/stream.py
--rw-r--r--   0        0        0      757 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/tempo.py
--rw-r--r--   0        0        0     2607 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/track.py
--rw-r--r--   0        0        0        0 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/tracks/__init__.py
--rw-r--r--   0        0        0     1812 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/tracks/countdown.py
--rw-r--r--   0        0        0     2064 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/tracks/metronome.py
--rw-r--r--   0        0        0     1122 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/validate.py
--rw-r--r--   0        0        0    21934 2023-06-04 10:56:29.545807 playbacker-0.6.0/src/playbacker/dist/assets/index-04f532a9.js
--rw-r--r--   0        0        0     8295 2023-06-04 10:56:29.545807 playbacker-0.6.0/src/playbacker/dist/assets/index-c1f1d727.css
--rw-r--r--   0        0        0      388 2023-06-04 10:56:29.545807 playbacker-0.6.0/src/playbacker/dist/index.html
--rw-r--r--   0        0        0     2807 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/main.py
--rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 playbacker-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1254 2023-07-22 06:54:02.513766 playbacker-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-22 06:53:31.345172 playbacker-0.7.0/src/playbacker/__init__.py
+-rw-r--r--   0        0        0     5020 2023-07-22 06:53:31.345172 playbacker-0.7.0/src/playbacker/app.py
+-rw-r--r--   0        0        0      527 2023-07-22 06:53:31.345172 playbacker-0.7.0/src/playbacker/config.py
+-rw-r--r--   0        0        0        0 2023-07-22 06:53:31.345172 playbacker-0.7.0/src/playbacker/core/__init__.py
+-rw-r--r--   0        0        0      850 2023-07-22 06:53:31.345172 playbacker-0.7.0/src/playbacker/core/audiofile.py
+-rw-r--r--   0        0        0     1292 2023-07-22 06:53:31.345172 playbacker-0.7.0/src/playbacker/core/clock.py
+-rw-r--r--   0        0        0     3423 2023-07-22 06:53:31.345172 playbacker-0.7.0/src/playbacker/core/playback.py
+-rw-r--r--   0        0        0     1444 2023-07-22 06:53:31.345172 playbacker-0.7.0/src/playbacker/core/player.py
+-rw-r--r--   0        0        0      974 2023-07-22 06:53:31.345172 playbacker-0.7.0/src/playbacker/core/setlist.py
+-rw-r--r--   0        0        0     3497 2023-07-22 06:53:31.345172 playbacker-0.7.0/src/playbacker/core/settings.py
+-rw-r--r--   0        0        0      892 2023-07-22 06:53:31.345172 playbacker-0.7.0/src/playbacker/core/song.py
+-rw-r--r--   0        0        0     3137 2023-07-22 06:53:31.345172 playbacker-0.7.0/src/playbacker/core/stream.py
+-rw-r--r--   0        0        0      765 2023-07-22 06:53:31.345172 playbacker-0.7.0/src/playbacker/core/tempo.py
+-rw-r--r--   0        0        0     2607 2023-07-22 06:53:31.345172 playbacker-0.7.0/src/playbacker/core/track.py
+-rw-r--r--   0        0        0        0 2023-07-22 06:53:31.345172 playbacker-0.7.0/src/playbacker/core/tracks/__init__.py
+-rw-r--r--   0        0        0     2066 2023-07-22 06:53:31.345172 playbacker-0.7.0/src/playbacker/core/tracks/countdown.py
+-rw-r--r--   0        0        0     2611 2023-07-22 06:53:31.345172 playbacker-0.7.0/src/playbacker/core/tracks/metronome.py
+-rw-r--r--   0        0        0     1122 2023-07-22 06:53:31.345172 playbacker-0.7.0/src/playbacker/core/validate.py
+-rw-r--r--   0        0        0    21934 2023-07-22 06:54:01.937755 playbacker-0.7.0/src/playbacker/dist/assets/index-04f532a9.js
+-rw-r--r--   0        0        0     8295 2023-07-22 06:54:01.937755 playbacker-0.7.0/src/playbacker/dist/assets/index-c1f1d727.css
+-rw-r--r--   0        0        0      388 2023-07-22 06:54:01.937755 playbacker-0.7.0/src/playbacker/dist/index.html
+-rw-r--r--   0        0        0     2807 2023-07-22 06:53:31.345172 playbacker-0.7.0/src/playbacker/main.py
+-rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 playbacker-0.7.0/PKG-INFO
```

### Comparing `playbacker-0.6.0/pyproject.toml` & `playbacker-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "playbacker"
-version = "v0.6.0"
+version = "v0.7.0"
 description = "Live music performance playback"
 authors = ["Lev Vereshchagin <mail@vrslev.com>"]
 license = "MIT"
 # TODO: readme
 # readme = "../README.md"
 include = ["src/playbacker/dist/**/*"]
```

### Comparing `playbacker-0.6.0/src/playbacker/app.py` & `playbacker-0.7.0/src/playbacker/app.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.6.0/src/playbacker/config.py` & `playbacker-0.7.0/src/playbacker/config.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.6.0/src/playbacker/core/audiofile.py` & `playbacker-0.7.0/src/playbacker/core/audiofile.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.6.0/src/playbacker/core/clock.py` & `playbacker-0.7.0/src/playbacker/core/clock.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.6.0/src/playbacker/core/playback.py` & `playbacker-0.7.0/src/playbacker/core/playback.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.6.0/src/playbacker/core/player.py` & `playbacker-0.7.0/src/playbacker/core/player.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.6.0/src/playbacker/core/setlist.py` & `playbacker-0.7.0/src/playbacker/core/setlist.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.6.0/src/playbacker/core/settings.py` & `playbacker-0.7.0/src/playbacker/core/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     name: str | None
     pretty_name: str
     sample_rate: int
     channel_map: _ChannelMap
 
 
 class _MetronomePaths(BaseModel):
+    accent: Path
     tick_1_4: Path = Field(alias="1/4")
     tick_1_8: Path = Field(alias="1/8")
     tick_1_16: Path = Field(alias="1/16")
 
 
 class _CountdownPaths(BaseModel):
     count_1: Path
@@ -100,14 +101,15 @@
 
     return Settings(
         device=device.name,
         sample_rate=device.sample_rate,
         channel_map=device.channel_map,
         sounds=_Sounds(
             metronome=MetronomeSounds(
+                accent=AudioFile(metronome.accent, device.sample_rate),
                 tick_1_4=AudioFile(metronome.tick_1_4, device.sample_rate),
                 tick_1_8=AudioFile(metronome.tick_1_8, device.sample_rate),
                 tick_1_16=AudioFile(metronome.tick_1_16, device.sample_rate),
             ),
             countdown=CountdownSounds(
                 count_1=AudioFile(countdown.count_1, device.sample_rate),
                 count_2=AudioFile(countdown.count_2, device.sample_rate),
```

### Comparing `playbacker-0.6.0/src/playbacker/core/song.py` & `playbacker-0.7.0/src/playbacker/core/song.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.6.0/src/playbacker/core/stream.py` & `playbacker-0.7.0/src/playbacker/core/stream.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.6.0/src/playbacker/core/tempo.py` & `playbacker-0.7.0/src/playbacker/core/tempo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Literal
 
 from pydantic import BaseModel
 
-TimeSignature = Literal["4/4", "6/8"]
+TimeSignature = Literal["4/4", "6/8", "12/4"]
 Duration = Literal["1/4", "1/8", "1/16"]
 
 
 class Tempo(BaseModel, frozen=True):
     bpm: float
     time_signature: TimeSignature
     duration: Duration
```

### Comparing `playbacker-0.6.0/src/playbacker/core/track.py` & `playbacker-0.7.0/src/playbacker/core/track.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.6.0/src/playbacker/core/tracks/countdown.py` & `playbacker-0.7.0/src/playbacker/core/tracks/countdown.py`

 * *Files 22% similar despite different names*

```diff
@@ -57,8 +57,16 @@
         _Entry(end=5, instruction=1),
         _Entry(end=11, instruction=2),
         _Entry(end=14, instruction=1),
         _Entry(end=17, instruction=2),
         _Entry(end=20, instruction=3),
         _Entry(end=23, instruction=4),
     ],
+    "12/4": [
+        _Entry(end=5, instruction=1),
+        _Entry(end=11, instruction=2),
+        _Entry(end=14, instruction=1),
+        _Entry(end=17, instruction=2),
+        _Entry(end=20, instruction=3),
+        _Entry(end=23, instruction=4),
+    ],
 }
```

### Comparing `playbacker-0.6.0/src/playbacker/core/tracks/metronome.py` & `playbacker-0.7.0/src/playbacker/core/tracks/metronome.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 
 from playbacker.core.audiofile import AudioArray, AudioFile
 from playbacker.core.tempo import Duration, Tempo, TimeSignature
 from playbacker.core.track import SoundTrack
 
 
 class MetronomeSounds(NamedTuple):
+    accent: AudioFile
     tick_1_4: AudioFile
     tick_1_8: AudioFile
     tick_1_16: AudioFile
 
 
-_Instruction = Literal[4, 8, 16]
+_Instruction = Literal["accent", 4, 8, 16]
 
 
 @dataclass
 class MetronomeTrack(SoundTrack[MetronomeSounds]):
     instruction_to_sound: dict[_Instruction, AudioFile] = field(init=False, repr=False)
 
     def __post_init__(self) -> None:
         super().__post_init__()
         self.instruction_to_sound = {
+            "accent": self.sounds.accent,
             4: self.sounds.tick_1_4,
             8: self.sounds.tick_1_8,
             16: self.sounds.tick_1_16,
         }
 
     def get_sound(self) -> AudioArray | None:
         if instruction := get_instruction(self.shared.tempo, self.shared.position):
@@ -39,15 +41,19 @@
     divider: int
     instruction: _Instruction
 
 
 metronome_schemes: dict[TimeSignature, dict[Duration, list[_Entry]]] = {
     "4/4": {
         "1/4": [_Entry(divider=4, instruction=4)],
-        "1/8": [_Entry(divider=4, instruction=4), _Entry(divider=2, instruction=8)],
+        "1/8": [
+            _Entry(divider=16, instruction="accent"),
+            _Entry(divider=4, instruction=4),
+            _Entry(divider=2, instruction=8),
+        ],
         "1/16": [
             _Entry(divider=4, instruction=4),
             _Entry(divider=2, instruction=8),
             _Entry(divider=1, instruction=16),
         ],
     },
     "6/8": {
@@ -55,14 +61,26 @@
         "1/8": [_Entry(divider=6, instruction=4), _Entry(divider=2, instruction=8)],
         "1/16": [
             _Entry(divider=6, instruction=4),
             _Entry(divider=2, instruction=8),
             _Entry(divider=1, instruction=16),
         ],
     },
+    "12/4": {
+        "1/4": [_Entry(divider=12, instruction="accent")],
+        "1/8": [
+            _Entry(divider=12, instruction="accent"),
+            _Entry(divider=2, instruction=8),
+        ],
+        "1/16": [
+            _Entry(divider=12, instruction="accent"),
+            _Entry(divider=2, instruction=8),
+            _Entry(divider=1, instruction=16),
+        ],
+    },
 }
 
 
 def get_instruction(tempo: Tempo, position: int) -> _Instruction | None:
     for divider, instruction in metronome_schemes[tempo.time_signature][tempo.duration]:
         if position % divider == 0:
             return instruction
```

### Comparing `playbacker-0.6.0/src/playbacker/core/validate.py` & `playbacker-0.7.0/src/playbacker/core/validate.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.6.0/src/playbacker/dist/assets/index-04f532a9.js` & `playbacker-0.7.0/src/playbacker/dist/assets/index-04f532a9.js`

 * *Files identical despite different names*

### Comparing `playbacker-0.6.0/src/playbacker/dist/assets/index-c1f1d727.css` & `playbacker-0.7.0/src/playbacker/dist/assets/index-c1f1d727.css`

 * *Files identical despite different names*

### Comparing `playbacker-0.6.0/src/playbacker/main.py` & `playbacker-0.7.0/src/playbacker/main.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.6.0/PKG-INFO` & `playbacker-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playbacker
-Version: 0.6.0
+Version: 0.7.0
 Summary: Live music performance playback
 License: MIT
 Author: Lev Vereshchagin
 Author-email: mail@vrslev.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

