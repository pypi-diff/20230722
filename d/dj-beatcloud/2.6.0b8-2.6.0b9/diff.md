# Comparing `tmp/dj_beatcloud-2.6.0b8.tar.gz` & `tmp/dj_beatcloud-2.6.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_beatcloud-2.6.0b8.tar", last modified: Fri Jul 21 23:14:05 2023, max compression
+gzip compressed data, was "dj_beatcloud-2.6.0b9.tar", last modified: Sat Jul 22 18:30:41 2023, max compression
```

## Comparing `dj_beatcloud-2.6.0b8.tar` & `dj_beatcloud-2.6.0b9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-21 23:14:05.585915 dj_beatcloud-2.6.0b8/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.6.0b8/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 dj_beatcloud-2.6.0b8/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)     2556 2023-07-21 23:14:05.586014 dj_beatcloud-2.6.0b8/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-26 21:16:19.000000 dj_beatcloud-2.6.0b8/README.md
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-21 23:14:05.554611 dj_beatcloud-2.6.0b8/dj_beatcloud.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)     2556 2023-07-21 23:14:05.000000 dj_beatcloud-2.6.0b8/dj_beatcloud.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1239 2023-07-21 23:14:05.000000 dj_beatcloud-2.6.0b8/dj_beatcloud.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-07-21 23:14:05.000000 dj_beatcloud-2.6.0b8/dj_beatcloud.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-07-21 23:14:05.000000 dj_beatcloud-2.6.0b8/dj_beatcloud.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-07-21 23:14:05.000000 dj_beatcloud-2.6.0b8/dj_beatcloud.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-07-21 23:14:05.000000 dj_beatcloud-2.6.0b8/dj_beatcloud.egg-info/top_level.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-21 23:14:05.556320 dj_beatcloud-2.6.0b8/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)     2541 2023-07-19 21:40:19.000000 dj_beatcloud-2.6.0b8/djtools/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1885 2023-07-21 23:07:04.000000 dj_beatcloud-2.6.0b8/djtools/__main__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-21 23:14:05.567594 dj_beatcloud-2.6.0b8/djtools/collection/
--rw-r--r--   0 alrichards   (502) staff       (20)     1428 2023-07-19 21:39:04.000000 dj_beatcloud-2.6.0b8/djtools/collection/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)    12876 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/collection/collections.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2807 2023-07-19 21:39:18.000000 dj_beatcloud-2.6.0b8/djtools/collection/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3001 2023-07-21 22:36:23.000000 dj_beatcloud-2.6.0b8/djtools/collection/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    27170 2023-07-21 21:03:04.000000 dj_beatcloud-2.6.0b8/djtools/collection/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7582 2023-07-21 21:03:31.000000 dj_beatcloud-2.6.0b8/djtools/collection/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)    15832 2023-07-21 21:47:34.000000 dj_beatcloud-2.6.0b8/djtools/collection/playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2404 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/collection/shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    13902 2023-07-19 22:57:46.000000 dj_beatcloud-2.6.0b8/djtools/collection/tracks.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-21 23:14:05.573143 dj_beatcloud-2.6.0b8/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b8/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1179 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/configs/collection_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     1765 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1300 2023-07-21 20:46:32.000000 dj_beatcloud-2.6.0b8/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    20888 2023-07-21 21:08:32.000000 dj_beatcloud-2.6.0b8/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b8/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b8/djtools/configs/spotify_playlists.yaml
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-21 23:14:05.573771 dj_beatcloud-2.6.0b8/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b8/djtools/logs/empty.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-21 23:14:05.577145 dj_beatcloud-2.6.0b8/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      735 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3258 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    16599 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6053 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/spotify/playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-21 23:14:05.580460 dj_beatcloud-2.6.0b8/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      874 2023-07-21 22:58:50.000000 dj_beatcloud-2.6.0b8/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3693 2023-07-21 20:46:29.000000 dj_beatcloud-2.6.0b8/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7682 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5349 2023-07-21 23:04:47.000000 dj_beatcloud-2.6.0b8/djtools/sync/sync_operations.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-21 23:14:05.585499 dj_beatcloud-2.6.0b8/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1409 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    10160 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b8/djtools/utils/url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-07-21 23:08:54.000000 dj_beatcloud-2.6.0b8/djtools/version.py
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.6.0b8/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)       99 2023-07-21 23:14:05.586498 dj_beatcloud-2.6.0b8/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2345 2023-07-21 21:08:42.000000 dj_beatcloud-2.6.0b8/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-22 18:30:41.059523 dj_beatcloud-2.6.0b9/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.6.0b9/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 dj_beatcloud-2.6.0b9/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)     2556 2023-07-22 18:30:41.059615 dj_beatcloud-2.6.0b9/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-26 21:16:19.000000 dj_beatcloud-2.6.0b9/README.md
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-22 18:30:41.024445 dj_beatcloud-2.6.0b9/dj_beatcloud.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2556 2023-07-22 18:30:40.000000 dj_beatcloud-2.6.0b9/dj_beatcloud.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1239 2023-07-22 18:30:41.000000 dj_beatcloud-2.6.0b9/dj_beatcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-07-22 18:30:40.000000 dj_beatcloud-2.6.0b9/dj_beatcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-07-22 18:30:40.000000 dj_beatcloud-2.6.0b9/dj_beatcloud.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-07-22 18:30:40.000000 dj_beatcloud-2.6.0b9/dj_beatcloud.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-07-22 18:30:40.000000 dj_beatcloud-2.6.0b9/dj_beatcloud.egg-info/top_level.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-22 18:30:41.027233 dj_beatcloud-2.6.0b9/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2541 2023-07-19 21:40:19.000000 dj_beatcloud-2.6.0b9/djtools/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1885 2023-07-21 23:07:04.000000 dj_beatcloud-2.6.0b9/djtools/__main__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-22 18:30:41.036704 dj_beatcloud-2.6.0b9/djtools/collection/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1428 2023-07-19 21:39:04.000000 dj_beatcloud-2.6.0b9/djtools/collection/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    12876 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b9/djtools/collection/collections.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2807 2023-07-19 21:39:18.000000 dj_beatcloud-2.6.0b9/djtools/collection/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2985 2023-07-22 18:21:41.000000 dj_beatcloud-2.6.0b9/djtools/collection/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    27170 2023-07-21 21:03:04.000000 dj_beatcloud-2.6.0b9/djtools/collection/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7582 2023-07-21 21:03:31.000000 dj_beatcloud-2.6.0b9/djtools/collection/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    15832 2023-07-21 21:47:34.000000 dj_beatcloud-2.6.0b9/djtools/collection/playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2404 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b9/djtools/collection/shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    13902 2023-07-19 22:57:46.000000 dj_beatcloud-2.6.0b9/djtools/collection/tracks.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-22 18:30:41.043982 dj_beatcloud-2.6.0b9/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b9/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1179 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b9/djtools/configs/collection_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     1765 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b9/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1300 2023-07-22 18:28:08.000000 dj_beatcloud-2.6.0b9/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    20888 2023-07-21 21:08:32.000000 dj_beatcloud-2.6.0b9/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b9/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b9/djtools/configs/spotify_playlists.yaml
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-22 18:30:41.044444 dj_beatcloud-2.6.0b9/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b9/djtools/logs/empty.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-22 18:30:41.047214 dj_beatcloud-2.6.0b9/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      735 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b9/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3258 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b9/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    16599 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b9/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6053 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b9/djtools/spotify/playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-22 18:30:41.052873 dj_beatcloud-2.6.0b9/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      874 2023-07-21 22:58:50.000000 dj_beatcloud-2.6.0b9/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3693 2023-07-21 20:46:29.000000 dj_beatcloud-2.6.0b9/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7682 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b9/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5415 2023-07-21 23:22:44.000000 dj_beatcloud-2.6.0b9/djtools/sync/sync_operations.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-22 18:30:41.058973 dj_beatcloud-2.6.0b9/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b9/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b9/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1409 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b9/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    10160 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b9/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b9/djtools/utils/url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-07-22 18:29:16.000000 dj_beatcloud-2.6.0b9/djtools/version.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.6.0b9/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)       99 2023-07-22 18:30:41.060838 dj_beatcloud-2.6.0b9/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2345 2023-07-21 21:08:42.000000 dj_beatcloud-2.6.0b9/setup.py
```

### Comparing `dj_beatcloud-2.6.0b8/LICENSE` & `dj_beatcloud-2.6.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/PKG-INFO` & `dj_beatcloud-2.6.0b9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_beatcloud
-Version: 2.6.0b8
+Version: 2.6.0b9
 Summary: DJ Tools is a library for managing a collection of music.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 Keywords: DJ Rekordbox spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.6.0b8 Summary: DJ Tools is
+Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.6.0b9 Summary: DJ Tools is
 a library for managing a collection of music. Home-page: https://github.com/a-
 rich/DJ-tools Author: Alex Richards Author-email: alex.richards006@gmail.com
 Keywords: DJ Rekordbox spotify reddit aws s3 Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: End Users/Desktop Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Operating System :: MacOS
```

### Comparing `dj_beatcloud-2.6.0b8/README.md` & `dj_beatcloud-2.6.0b9/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/dj_beatcloud.egg-info/PKG-INFO` & `dj_beatcloud-2.6.0b9/dj_beatcloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-beatcloud
-Version: 2.6.0b8
+Version: 2.6.0b9
 Summary: DJ Tools is a library for managing a collection of music.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 Keywords: DJ Rekordbox spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.6.0b8 Summary: DJ Tools is
+Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.6.0b9 Summary: DJ Tools is
 a library for managing a collection of music. Home-page: https://github.com/a-
 rich/DJ-tools Author: Alex Richards Author-email: alex.richards006@gmail.com
 Keywords: DJ Rekordbox spotify reddit aws s3 Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: End Users/Desktop Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Operating System :: MacOS
```

### Comparing `dj_beatcloud-2.6.0b8/dj_beatcloud.egg-info/SOURCES.txt` & `dj_beatcloud-2.6.0b9/dj_beatcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/__init__.py` & `dj_beatcloud-2.6.0b9/djtools/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/__main__.py` & `dj_beatcloud-2.6.0b9/djtools/__main__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/collection/__init__.py` & `dj_beatcloud-2.6.0b9/djtools/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/collection/collections.py` & `dj_beatcloud-2.6.0b9/djtools/collection/collections.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/collection/config.py` & `dj_beatcloud-2.6.0b9/djtools/collection/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/collection/copy_playlists.py` & `dj_beatcloud-2.6.0b9/djtools/collection/copy_playlists.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,35 +48,35 @@
             raise LookupError(f"{playlist_name} not found")
         playlists.extend(
             [
                 playlist for playlist in found_playlists
                 if not playlist.is_folder()
             ]
         )
-    
+
     # Traverse the playlist to get tracks for the desired playlists and mark
     # the rest for removal.
     for playlist in playlists:
         playlist_tracks.update(playlist.get_tracks())
         parent = playlist.get_parent()
         while parent:
             for child in list(parent):
                 if child is not playlist and child not in lineage:
                     lineage[parent].add(child)
                     continue
-                elif any([child in children for children in lineage.values()]):
+                if any(child in children for children in lineage.values()):
                     lineage[parent].discard(child)
             parent = parent.get_parent()
     collection.set_tracks(playlist_tracks)
-    
+
     # Remove the extra playlists.
     for parent, children in lineage.items():
         for child in children:
             parent.remove_playlist(child)
-    
+
     # Copy tracks to the destination and update their location.
     payload = [
         playlist_tracks.values(),
         [config.COPY_PLAYLISTS_DESTINATION] * len(playlist_tracks),
     ]
     with ThreadPoolExecutor(max_workers=os.cpu_count() * 4) as executor:
         _ = list(
```

### Comparing `dj_beatcloud-2.6.0b8/djtools/collection/helpers.py` & `dj_beatcloud-2.6.0b9/djtools/collection/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/collection/playlist_builder.py` & `dj_beatcloud-2.6.0b9/djtools/collection/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/collection/playlists.py` & `dj_beatcloud-2.6.0b9/djtools/collection/playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/collection/shuffle_playlists.py` & `dj_beatcloud-2.6.0b9/djtools/collection/shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/collection/tracks.py` & `dj_beatcloud-2.6.0b9/djtools/collection/tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/configs/collection_playlists.yaml` & `dj_beatcloud-2.6.0b9/djtools/configs/collection_playlists.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/configs/config.py` & `dj_beatcloud-2.6.0b9/djtools/configs/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/configs/config.yaml` & `dj_beatcloud-2.6.0b9/djtools/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/configs/helpers.py` & `dj_beatcloud-2.6.0b9/djtools/configs/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/spotify/__init__.py` & `dj_beatcloud-2.6.0b9/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/spotify/config.py` & `dj_beatcloud-2.6.0b9/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/spotify/helpers.py` & `dj_beatcloud-2.6.0b9/djtools/spotify/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/spotify/playlist_builder.py` & `dj_beatcloud-2.6.0b9/djtools/spotify/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/sync/__init__.py` & `dj_beatcloud-2.6.0b9/djtools/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/sync/config.py` & `dj_beatcloud-2.6.0b9/djtools/sync/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/sync/helpers.py` & `dj_beatcloud-2.6.0b9/djtools/sync/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/sync/sync_operations.py` & `dj_beatcloud-2.6.0b9/djtools/sync/sync_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,19 @@
         user = config.DOWNLOAD_SPOTIFY_PLAYLIST.split("Uploads")[0].strip()
         beatcloud_tracks, beatcloud_matches = compare_tracks(
             config,
             beatcloud_tracks=beatcloud_tracks,
             download_spotify_playlist=config.DOWNLOAD_SPOTIFY_PLAYLIST,
         )
         if not beatcloud_matches:
-            logger.warning("No Beatcloud matches were found! Make sure you've supplied to correct playlist name.")
-            return
+            logger.warning(
+                "No Beatcloud matches were found! Make sure you've supplied "
+                "to correct playlist name."
+            )
+            return beatcloud_tracks
         config.DOWNLOAD_INCLUDE_DIRS = [
             (Path(user) / path.as_posix().split(f"{Path(user)}/")[-1])
             for path in beatcloud_matches
         ]
         config.DOWNLOAD_EXCLUDE_DIRS = []
 
     logger.info("Downloading track collection...")
```

### Comparing `dj_beatcloud-2.6.0b8/djtools/utils/__init__.py` & `dj_beatcloud-2.6.0b9/djtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/utils/check_tracks.py` & `dj_beatcloud-2.6.0b9/djtools/utils/check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/utils/config.py` & `dj_beatcloud-2.6.0b9/djtools/utils/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/utils/helpers.py` & `dj_beatcloud-2.6.0b9/djtools/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/djtools/utils/url_download.py` & `dj_beatcloud-2.6.0b9/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b8/setup.py` & `dj_beatcloud-2.6.0b9/setup.py`

 * *Files identical despite different names*

