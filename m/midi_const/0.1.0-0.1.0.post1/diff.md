# Comparing `tmp/midi_const-0.1.0.tar.gz` & `tmp/midi_const-0.1.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midi_const-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "midi_const-0.1.0.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `midi_const-0.1.0.tar` & `midi_const-0.1.0.post1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      165 2023-07-22 18:03:50.913912 midi_const-0.1.0/.gitignore
--rw-r--r--   0        0        0      313 2023-07-22 17:08:37.427638 midi_const-0.1.0/.reuse/dep5
--rw-r--r--   0        0        0      169 2023-07-22 20:04:52.965669 midi_const-0.1.0/LICENSE
--rw-r--r--   0        0        0     7048 2023-07-22 16:42:23.687188 midi_const-0.1.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0     1078 2023-07-22 17:06:46.493218 midi_const-0.1.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0     1211 2023-07-22 17:06:51.338162 midi_const-0.1.0/LICENSES/Unlicense.txt
--rw-r--r--   0        0        0     1371 2023-07-22 20:45:38.928667 midi_const-0.1.0/README.md
--rw-r--r--   0        0        0      966 2023-07-22 19:58:58.258349 midi_const-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    51566 2023-07-22 20:56:33.042519 midi_const-0.1.0/src/midi_const/__init__.py
--rw-r--r--   0        0        0      971 2023-07-22 19:34:13.701144 midi_const-0.1.0/src/midi_const/_utils.py
--rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 midi_const-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      165 2023-07-22 18:03:50.913912 midi_const-0.1.0.post1/.gitignore
+-rw-r--r--   0        0        0      313 2023-07-22 17:08:37.427638 midi_const-0.1.0.post1/.reuse/dep5
+-rw-r--r--   0        0        0      169 2023-07-22 20:04:52.965669 midi_const-0.1.0.post1/LICENSE
+-rw-r--r--   0        0        0     7048 2023-07-22 16:42:23.687188 midi_const-0.1.0.post1/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0     1078 2023-07-22 17:06:46.493218 midi_const-0.1.0.post1/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     1211 2023-07-22 17:06:51.338162 midi_const-0.1.0.post1/LICENSES/Unlicense.txt
+-rw-r--r--   0        0        0     1371 2023-07-22 20:45:38.928667 midi_const-0.1.0.post1/README.md
+-rw-r--r--   0        0        0     1017 2023-07-22 21:01:20.722699 midi_const-0.1.0.post1/pyproject.toml
+-rw-r--r--   0        0        0    51571 2023-07-22 21:12:15.241297 midi_const-0.1.0.post1/src/midi_const/__init__.py
+-rw-r--r--   0        0        0      971 2023-07-22 19:34:13.701144 midi_const-0.1.0.post1/src/midi_const/_utils.py
+-rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 midi_const-0.1.0.post1/PKG-INFO
```

### Comparing `midi_const-0.1.0/LICENSES/CC0-1.0.txt` & `midi_const-0.1.0.post1/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `midi_const-0.1.0/LICENSES/MIT.txt` & `midi_const-0.1.0.post1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `midi_const-0.1.0/LICENSES/Unlicense.txt` & `midi_const-0.1.0.post1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `midi_const-0.1.0/README.md` & `midi_const-0.1.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `midi_const-0.1.0/pyproject.toml` & `midi_const-0.1.0.post1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# SPDX-FileCopyrightText: 2023 Raphaël Doursenaud <rdoursenaud@gmail.com>
-#
-# SPDX-License-Identifier: CC0-1.0 OR MIT OR Unlicense
-
-[build-system]
-requires = ["flit_core ~=3.2"]
-build-backend = "flit_core.buildapi"
-
-[project]
-name = "midi_const"
-authors = [{name = "Raphaël Doursenaud", email = "rdoursenaud@gmail.com"}]
-license = {file = "LICENSE"}
-classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Intended Audience :: Developers",
-    "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
-    "License :: OSI Approved :: MIT License",
-    "License :: OSI Approved :: The Unlicense (Unlicense)",
-    "Natural Language :: English",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Topic :: Multimedia :: Sound/Audio :: MIDI",
-    "Topic :: Scientific/Engineering",
-    "Topic :: Software Development",
-]
-dynamic = ["version", "description"]
-
-[project.urls]
-Home = "https://github.com/ematech/midi_const"
+# SPDX-FileCopyrightText: 2023 Raphaël Doursenaud <rdoursenaud@gmail.com>
+#
+# SPDX-License-Identifier: CC0-1.0 OR MIT OR Unlicense
+
+[build-system]
+requires = ["flit_core ~=3.2"]
+build-backend = "flit_core.buildapi"
+
+[project]
+name = "midi_const"
+authors = [{name = "Raphaël Doursenaud", email = "rdoursenaud@gmail.com"}]
+readme = "README.md"
+license = {file = "LICENSE"}
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
+    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: The Unlicense (Unlicense)",
+    "Natural Language :: English",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Topic :: Multimedia :: Sound/Audio :: MIDI",
+    "Topic :: Scientific/Engineering",
+    "Topic :: Software Development",
+]
+dynamic = ["version", "description"]
+
+[project.urls]
+Home = "https://github.com/ematech/midi_const"
```

### Comparing `midi_const-0.1.0/src/midi_const/__init__.py` & `midi_const-0.1.0.post1/src/midi_const/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # This Python file uses the following encoding: utf-8
 #
 # SPDX-FileCopyrightText: 2021 Raphaël Doursenaud <rdoursenaud@gmail.com>
 #
 # SPDX-License-Identifier: CC0-1.0 OR MIT OR Unlicense
-
 """
 Python MIDI constants.
 
 Derived from official MIDI specifications available at:
 - MIDI Association, ex MIDI Manufacturers Association (MMA) [US]:
   https://midi.org
 - Association of Musical Electronics Industry (AMEI) [JP]:
   (https://www.amei.or.jp/)
 - MIDI Standard Committee (MSC) [JP]:
   http://amei.or.jp/midistandardcommittee
 """
 
-__version__ = "0.1.0"
+__version__ = "0.1.0.post1"
 
 VERSION = {
     1: "1.0",
     2: "2.0"  # TODO
 }
 
 ###
```

### Comparing `midi_const-0.1.0/src/midi_const/_utils.py` & `midi_const-0.1.0.post1/src/midi_const/_utils.py`

 * *Files identical despite different names*

