# Comparing `tmp/dj_beatcloud-2.6.0b7.tar.gz` & `tmp/dj_beatcloud-2.6.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_beatcloud-2.6.0b7.tar", last modified: Wed Jul 19 23:06:50 2023, max compression
+gzip compressed data, was "dj_beatcloud-2.6.0b8.tar", last modified: Fri Jul 21 23:14:05 2023, max compression
```

## Comparing `dj_beatcloud-2.6.0b7.tar` & `dj_beatcloud-2.6.0b8.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 23:06:50.063555 dj_beatcloud-2.6.0b7/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.6.0b7/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 dj_beatcloud-2.6.0b7/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)     2556 2023-07-19 23:06:50.063744 dj_beatcloud-2.6.0b7/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-26 21:16:19.000000 dj_beatcloud-2.6.0b7/README.md
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 23:06:50.033940 dj_beatcloud-2.6.0b7/dj_beatcloud.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)     2556 2023-07-19 23:06:50.000000 dj_beatcloud-2.6.0b7/dj_beatcloud.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1239 2023-07-19 23:06:50.000000 dj_beatcloud-2.6.0b7/dj_beatcloud.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-07-19 23:06:50.000000 dj_beatcloud-2.6.0b7/dj_beatcloud.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-07-19 23:06:50.000000 dj_beatcloud-2.6.0b7/dj_beatcloud.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-07-19 23:06:50.000000 dj_beatcloud-2.6.0b7/dj_beatcloud.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-07-19 23:06:50.000000 dj_beatcloud-2.6.0b7/dj_beatcloud.egg-info/top_level.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 23:06:50.036630 dj_beatcloud-2.6.0b7/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)     2541 2023-07-19 21:40:19.000000 dj_beatcloud-2.6.0b7/djtools/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1774 2023-07-19 21:40:04.000000 dj_beatcloud-2.6.0b7/djtools/__main__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 23:06:50.045032 dj_beatcloud-2.6.0b7/djtools/collection/
--rw-r--r--   0 alrichards   (502) staff       (20)     1428 2023-07-19 21:39:04.000000 dj_beatcloud-2.6.0b7/djtools/collection/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)    12876 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/djtools/collection/collections.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2807 2023-07-19 21:39:18.000000 dj_beatcloud-2.6.0b7/djtools/collection/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2514 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/djtools/collection/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    27145 2023-07-19 21:38:35.000000 dj_beatcloud-2.6.0b7/djtools/collection/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7582 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/djtools/collection/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)    15832 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/djtools/collection/playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2404 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/djtools/collection/shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    13902 2023-07-19 22:57:46.000000 dj_beatcloud-2.6.0b7/djtools/collection/tracks.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 23:06:50.049444 dj_beatcloud-2.6.0b7/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b7/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1179 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/djtools/configs/collection_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     1765 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1300 2023-07-19 23:06:36.000000 dj_beatcloud-2.6.0b7/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    17102 2023-07-19 22:26:44.000000 dj_beatcloud-2.6.0b7/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b7/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b7/djtools/configs/spotify_playlists.yaml
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 23:06:50.049847 dj_beatcloud-2.6.0b7/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b7/djtools/logs/empty.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 23:06:50.052302 dj_beatcloud-2.6.0b7/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      735 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3258 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    16599 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6053 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/djtools/spotify/playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 23:06:50.054759 dj_beatcloud-2.6.0b7/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      825 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3532 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7682 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5170 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/djtools/sync/sync_operations.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 23:06:50.062160 dj_beatcloud-2.6.0b7/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1409 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    10160 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b7/djtools/utils/url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-07-19 23:05:37.000000 dj_beatcloud-2.6.0b7/djtools/version.py
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.6.0b7/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)       99 2023-07-19 23:06:50.064454 dj_beatcloud-2.6.0b7/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2345 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b7/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-21 23:14:05.585915 dj_beatcloud-2.6.0b8/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.6.0b8/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 dj_beatcloud-2.6.0b8/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)     2556 2023-07-21 23:14:05.586014 dj_beatcloud-2.6.0b8/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-26 21:16:19.000000 dj_beatcloud-2.6.0b8/README.md
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-21 23:14:05.554611 dj_beatcloud-2.6.0b8/dj_beatcloud.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2556 2023-07-21 23:14:05.000000 dj_beatcloud-2.6.0b8/dj_beatcloud.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1239 2023-07-21 23:14:05.000000 dj_beatcloud-2.6.0b8/dj_beatcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-07-21 23:14:05.000000 dj_beatcloud-2.6.0b8/dj_beatcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-07-21 23:14:05.000000 dj_beatcloud-2.6.0b8/dj_beatcloud.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-07-21 23:14:05.000000 dj_beatcloud-2.6.0b8/dj_beatcloud.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-07-21 23:14:05.000000 dj_beatcloud-2.6.0b8/dj_beatcloud.egg-info/top_level.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-21 23:14:05.556320 dj_beatcloud-2.6.0b8/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2541 2023-07-19 21:40:19.000000 dj_beatcloud-2.6.0b8/djtools/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1885 2023-07-21 23:07:04.000000 dj_beatcloud-2.6.0b8/djtools/__main__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-21 23:14:05.567594 dj_beatcloud-2.6.0b8/djtools/collection/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1428 2023-07-19 21:39:04.000000 dj_beatcloud-2.6.0b8/djtools/collection/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    12876 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/collection/collections.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2807 2023-07-19 21:39:18.000000 dj_beatcloud-2.6.0b8/djtools/collection/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3001 2023-07-21 22:36:23.000000 dj_beatcloud-2.6.0b8/djtools/collection/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    27170 2023-07-21 21:03:04.000000 dj_beatcloud-2.6.0b8/djtools/collection/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7582 2023-07-21 21:03:31.000000 dj_beatcloud-2.6.0b8/djtools/collection/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    15832 2023-07-21 21:47:34.000000 dj_beatcloud-2.6.0b8/djtools/collection/playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2404 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/collection/shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    13902 2023-07-19 22:57:46.000000 dj_beatcloud-2.6.0b8/djtools/collection/tracks.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-21 23:14:05.573143 dj_beatcloud-2.6.0b8/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b8/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1179 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/configs/collection_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     1765 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1300 2023-07-21 20:46:32.000000 dj_beatcloud-2.6.0b8/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    20888 2023-07-21 21:08:32.000000 dj_beatcloud-2.6.0b8/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b8/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b8/djtools/configs/spotify_playlists.yaml
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-21 23:14:05.573771 dj_beatcloud-2.6.0b8/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b8/djtools/logs/empty.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-21 23:14:05.577145 dj_beatcloud-2.6.0b8/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      735 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3258 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    16599 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6053 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/spotify/playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-21 23:14:05.580460 dj_beatcloud-2.6.0b8/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      874 2023-07-21 22:58:50.000000 dj_beatcloud-2.6.0b8/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3693 2023-07-21 20:46:29.000000 dj_beatcloud-2.6.0b8/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7682 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5349 2023-07-21 23:04:47.000000 dj_beatcloud-2.6.0b8/djtools/sync/sync_operations.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-21 23:14:05.585499 dj_beatcloud-2.6.0b8/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1409 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    10160 2023-07-19 18:51:19.000000 dj_beatcloud-2.6.0b8/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b8/djtools/utils/url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-07-21 23:08:54.000000 dj_beatcloud-2.6.0b8/djtools/version.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.6.0b8/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)       99 2023-07-21 23:14:05.586498 dj_beatcloud-2.6.0b8/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2345 2023-07-21 21:08:42.000000 dj_beatcloud-2.6.0b8/setup.py
```

### Comparing `dj_beatcloud-2.6.0b7/LICENSE` & `dj_beatcloud-2.6.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/PKG-INFO` & `dj_beatcloud-2.6.0b8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_beatcloud
-Version: 2.6.0b7
+Version: 2.6.0b8
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
-Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.6.0b7 Summary: DJ Tools is
+Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.6.0b8 Summary: DJ Tools is
 a library for managing a collection of music. Home-page: https://github.com/a-
 rich/DJ-tools Author: Alex Richards Author-email: alex.richards006@gmail.com
 Keywords: DJ Rekordbox spotify reddit aws s3 Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: End Users/Desktop Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Operating System :: MacOS
```

### Comparing `dj_beatcloud-2.6.0b7/README.md` & `dj_beatcloud-2.6.0b8/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/dj_beatcloud.egg-info/PKG-INFO` & `dj_beatcloud-2.6.0b8/dj_beatcloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-beatcloud
-Version: 2.6.0b7
+Version: 2.6.0b8
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
-Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.6.0b7 Summary: DJ Tools is
+Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.6.0b8 Summary: DJ Tools is
 a library for managing a collection of music. Home-page: https://github.com/a-
 rich/DJ-tools Author: Alex Richards Author-email: alex.richards006@gmail.com
 Keywords: DJ Rekordbox spotify reddit aws s3 Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: End Users/Desktop Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Operating System :: MacOS
```

### Comparing `dj_beatcloud-2.6.0b7/dj_beatcloud.egg-info/SOURCES.txt` & `dj_beatcloud-2.6.0b8/dj_beatcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/__init__.py` & `dj_beatcloud-2.6.0b8/djtools/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/__main__.py` & `dj_beatcloud-2.6.0b8/djtools/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,29 +8,31 @@
         locations.
     * SHUFFLE_PLAYLISTS (shuffle_playlists.py): Set ID3 tags of tracks in
         playlists sequentially (after shuffling) to randomize.
 
 Spotify operations:
     * SPOTIFY_PLAYLISTS (spotify.playlist_builder.py): Creating and updating
         Spotify playlists using subreddit top posts.
-    * PLAYLISTS_FROM_UPLOAD (spotify.playlist_builder.py): Creating and
+    * SPOTIFY_PLAYLISTS_FROM_UPLOAD (spotify.playlist_builder.py): Creating and
         updating Spotify playlists using the Discord webhook output from users
         uploading music.
 
 Utils operations:
     * CHECK_TRACKS (check_tracks.py): Identify overlap between Spotify 
         playlists and / or local directories and and the Beatcloud.
     * URL_DOWNLOAD (url_download.py): Download tracks from a URL (e.g.
         Soundcloud playlist).
 
 Sync operations:
-    * DOWNLOAD_MUSIC: Sync tracks from beatcloud to USB_PATH.
+    * DOWNLOAD_MUSIC: Sync tracks from Beatcloud to USB_PATH.
     * DOWNLOAD_COLLECTION: Sync IMPORT_USER's collection to COLLECTION_PATH's
         parent folder.
-    * UPLOAD_MUSIC: Sync tracks from USB_PATH to beatcloud.
+    * DOWNLOAD_SPOTIFY_PLAYLIST: Sync tracks in a Spotify playlist from
+        Beatcloud to USB_PATH.
+    * UPLOAD_MUSIC: Sync tracks from USB_PATH to Beatcloud.
     * UPLOAD_COLLECTION: Sync COLLECTION_PATH to USER's collection folder.
 """
 
 import logging
 
 from djtools import main
```

### Comparing `dj_beatcloud-2.6.0b7/djtools/collection/__init__.py` & `dj_beatcloud-2.6.0b8/djtools/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/collection/collections.py` & `dj_beatcloud-2.6.0b8/djtools/collection/collections.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/collection/config.py` & `dj_beatcloud-2.6.0b8/djtools/collection/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/collection/copy_playlists.py` & `dj_beatcloud-2.6.0b8/djtools/collection/copy_playlists.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 new locations.
 
 The purpose of this utility is to:
 
 * backup subsets of your library
 * ensure you have easy access to a preparation independent of the setup
 """
+from collections import defaultdict
 from concurrent.futures import ThreadPoolExecutor
 import os
 
 from tqdm import tqdm
 
 from djtools.collection.helpers import copy_file, PLATFORM_REGISTRY
 from djtools.configs.config import BaseConfig
@@ -32,38 +33,50 @@
     collection = PLATFORM_REGISTRY[config.PLATFORM]["collection"](
         path=config.COLLECTION_PATH
     )
 
     # Create destination directory.
     config.COPY_PLAYLISTS_DESTINATION.mkdir(parents=True, exist_ok=True)
 
-    # Get the set of track IDs across the provided playlists.
-    # Get the parents of playlists so they aren't removed from the output
-    # playlists.
     playlist_tracks = {}
+    lineage = defaultdict(set)
+    playlists = []
+
+    # Get the playlists from the collection.
     for playlist_name in config.COPY_PLAYLISTS:
-        playlists = collection.get_playlists(playlist_name)
-        if not playlists:
+        found_playlists = collection.get_playlists(playlist_name)
+        if not found_playlists:
             raise LookupError(f"{playlist_name} not found")
-
-        for playlist in playlists:
-            if playlist.is_folder():
-                continue
-
-            parent = playlist.get_parent()
-            while parent:
-                for child in list(parent):
-                    if child is playlist:
-                        continue
-                    parent.remove_playlist(child)
-                parent = parent.get_parent()
-
-            playlist_tracks.update(playlist.get_tracks())
+        playlists.extend(
+            [
+                playlist for playlist in found_playlists
+                if not playlist.is_folder()
+            ]
+        )
+    
+    # Traverse the playlist to get tracks for the desired playlists and mark
+    # the rest for removal.
+    for playlist in playlists:
+        playlist_tracks.update(playlist.get_tracks())
+        parent = playlist.get_parent()
+        while parent:
+            for child in list(parent):
+                if child is not playlist and child not in lineage:
+                    lineage[parent].add(child)
+                    continue
+                elif any([child in children for children in lineage.values()]):
+                    lineage[parent].discard(child)
+            parent = parent.get_parent()
     collection.set_tracks(playlist_tracks)
-
+    
+    # Remove the extra playlists.
+    for parent, children in lineage.items():
+        for child in children:
+            parent.remove_playlist(child)
+    
     # Copy tracks to the destination and update their location.
     payload = [
         playlist_tracks.values(),
         [config.COPY_PLAYLISTS_DESTINATION] * len(playlist_tracks),
     ]
     with ThreadPoolExecutor(max_workers=os.cpu_count() * 4) as executor:
         _ = list(
```

### Comparing `dj_beatcloud-2.6.0b7/djtools/collection/helpers.py` & `dj_beatcloud-2.6.0b8/djtools/collection/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     Raises:
         ValueError: The user's playlist config must not be malformed.
 
     Returns:
         A Playlist or None.
     """
     # Initialize the set of tags in case the caller didn't provide one.
-    tag_set = tag_set or set()
+    tag_set = tag_set if tag_set is not None else set()
 
     # This is not a folder so a playlist with tracks must be created.
     if isinstance(content, str):
         # Apply special logic for creating a "pure" playlist. "Pure" playlists
         # are those that contain tracks with a set of genre tags that all
         # contain the sub-string indicated by the suffix of the playlist name.
         # For example, "Pure Techno" will contain tracks that have genres
```

### Comparing `dj_beatcloud-2.6.0b7/djtools/collection/playlist_builder.py` & `dj_beatcloud-2.6.0b8/djtools/collection/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/collection/playlists.py` & `dj_beatcloud-2.6.0b8/djtools/collection/playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/collection/shuffle_playlists.py` & `dj_beatcloud-2.6.0b8/djtools/collection/shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/collection/tracks.py` & `dj_beatcloud-2.6.0b8/djtools/collection/tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/configs/collection_playlists.yaml` & `dj_beatcloud-2.6.0b8/djtools/configs/collection_playlists.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/configs/config.py` & `dj_beatcloud-2.6.0b8/djtools/configs/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/configs/config.yaml` & `dj_beatcloud-2.6.0b8/djtools/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/configs/helpers.py` & `dj_beatcloud-2.6.0b8/djtools/configs/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """This module is responsible for building this library's configuration objects
 using config.yaml. If command-line arguments are provided, this module
 overrides the corresponding configuration options with these arguments.
 """
-import argparse
-from argparse import ArgumentParser
+from argparse import Action, ArgumentParser, Namespace, RawTextHelpFormatter
 import json
 import logging
 from pathlib import Path
 import sys
 from typing import Any, Dict, List, Union
 
 import yaml
@@ -27,20 +26,20 @@
     "configs": BaseConfig,
     "spotify": SpotifyConfig,
     "sync": SyncConfig,
     "utils": UtilsConfig,
 }
 
 
-class NonEmptyListElementAction(argparse.Action):
+class NonEmptyListElementAction(Action):
     """This Action implementation permits overriding list defaults.
 
     Some configuration options, like UPLOAD_EXCLUDE_DIRS, may be set to some
     sensible default in config.yaml. Because of this users will be unable to
-    run `--upload-music` in conjunction with `--download-include-dirs` without
+    run "--upload-music" in conjunction with "--download-include-dirs" without
     having to first make an edit to their config.yaml (because the
     include/exclude options are mutually exclusive).
     """
     def __call__(self, parser, namespace, values, option_string=None):
         """Filter list-type arguments for empty strings.
 
         Args:
@@ -51,342 +50,426 @@
         """
         values = values or []
         dest = getattr(namespace, self.dest) or []
         dest.extend(filter(None, values))
         setattr(namespace, self.dest, dest)
 
 
-def arg_parse() -> argparse.Namespace:
+def arg_parse() -> Namespace:
     """This function parses command-line arguments.
 
     It also sets the log level and symlinks a user-provided directory to the
     library's configs folder via the --link-configs argument.
 
     Returns:
-        argparse.NameSpace: Command-line arguments.
+        NameSpace with command-line arguments.
     """
     parser = ArgumentParser(
         description=(
             "djtools is a Python library with many features for streamlining "
             "the processes around collecting, curating, and sharing a music "
-            "collection."
+            "collection.\n\nRun djtools with one of the four available "
+            "sub-commands: collection, spotify, sync, utils"
         ),
+        formatter_class=RawTextHelpFormatter,
     )
     parser.add_argument(
         "--link-configs",
         type=convert_to_paths,
-        help="Location to symlink library configuration files to",
+        help=(
+            "The configuration files used by djtools are included at the "
+            "location where this package is installed...\nUse this option to "
+            "symbolically link them to a more accessible location for easier "
+            "editing.\nNote, the directory you're linking to must not already "
+            "exist."
+        ),
     )
     parser.add_argument(
         "--log-level",
         choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"],
-        help="Logger level",
+        help="Logger level.",
     )
     parser.add_argument(
         "--verbosity",
         "-v",
         action="count",
         default=0,
-        help="Logging verbosity",
+        help="Increase the logging verbosity.",
     )
     parser.add_argument(
         "--version",
         action="store_true",
-        help="Display package version",
+        help="Display the version number of the installed djtools.",
     )
-    subparsers = parser.add_subparsers(title="subcommands")
+    subparsers = parser.add_subparsers(title="sub-commands")
 
     ###########################################################################
     # Sub-command for the collection package.
     ###########################################################################
-    collection_parser = subparsers.add_parser("collection")
+    collection_parser = subparsers.add_parser(
+        name="collection",
+        help=(
+            "Perform operations on your DJ collection such as building "
+            "playlists based on your tags, shuffling track numbers, and "
+            "copying playlists to another location." 
+        ),
+        formatter_class=RawTextHelpFormatter,
+    )
     collection_parser.add_argument(
         "--collection-path",
         type=convert_to_paths,
-        help='Path to a collection database',
+        help='Path to a collection database (e.g. "rekordbox.xml").',
     )
     collection_parser.add_argument(
         "--collection-playlists",
         action="store_true",
-        help="Trigger building collection playlists",
+        help="Flag to trigger building collection playlists.",
     )
     collection_parser.add_argument(
         "--collection-playlists-remainder",
         type=str,
         choices=["folder", "playlist"],
         help=(
-            'Place remainder tracks in either an "Other" folder of playlists '
-            'or a single "Other" playlist'
+            "If there are tags not included in your "
+            '"collection_playlists.yaml", the associated tracks are '
+            'automatically pushed into either an "Other" folder of playlists '
+            '(one for each tag) or an "Other" playlist based on this option.'
         ),
     )
     collection_parser.add_argument(
         "--copy-playlists",
         type=str,
         nargs="+",
         action=NonEmptyListElementAction,
-        help="List of playlists to copy audio files from",
+        help=(
+            "By providing a list of playlist names, this option will:\n  - "
+            "copy the audio files in those playlists to "
+            '"--copy-playlists-destination"\n  - create a new collection with '
+            "just those playlists where the tracks contained in them have "
+            "updated locations"
+        ),
     )
     collection_parser.add_argument(
         "--copy-playlists-destination",
         type=convert_to_paths,
-        help="Location to copy playlists' audio files to",
+        help="Location to copy playlists' audio files to.",
     )
     collection_parser.add_argument(
         "--platform",
         type=str,
         choices=["rekordbox"],
-        help="DJ platform to use for the collection package",
+        help='DJ platform used for the collection package (e.g. "rekordbox").',
     )
     collection_parser.add_argument(
         "--shuffle-playlists",
         type=str,
         nargs="+",
         action=NonEmptyListElementAction,
-        help="List of playlist names to randomize tracks in",
+        help=(
+            "By providing a list of playlist names, this option will write to "
+            "the track number attribute to emulate shuffling of the tracks."
+        ),
     )
 
     ###########################################################################
     # Sub-command for the spotify package.
     ###########################################################################
-    spotify_parser = subparsers.add_parser("spotify")
+    spotify_parser = subparsers.add_parser(
+        name="spotify",
+        help=(
+            "Build playlists in Spotify either from:\n  - posts in the "
+            'subreddits configured with "--spotify-playlist-subreddits"\n  - '
+            'the output generated by a user running "--upload-music" with the '
+            '"--discord-url" option configured'
+        ),
+        formatter_class=RawTextHelpFormatter,
+    )
     spotify_parser.add_argument(
         "--reddit-client-id",
         type=str,
-        help="Reddit API client ID",
+        help="Reddit API client ID.",
     )
     spotify_parser.add_argument(
         "--reddit-client-secret",
         type=str,
-        help="Reddit API client secret",
+        help="Reddit API client secret.",
     )
     spotify_parser.add_argument(
         "--reddit-user-agent",
         type=str,
-        help="Reddit API user agent",
+        help="Reddit API user agent.",
     )
     spotify_parser.add_argument(
         "--spotify-client-id",
         type=str,
-        help="Spotify API client ID",
+        help="Spotify API client ID.",
     )
     spotify_parser.add_argument(
         "--spotify-client-secret",
         type=str,
-        help="Spotify API client secret",
+        help="Spotify API client secret.",
     )
     spotify_parser.add_argument(
         "--spotify-playlist-default-limit",
         type=int,
-        help="Default number of tracks for a Spotify playlist",
+        help="Default number of tracks for a Spotify playlist.",
     )
     spotify_parser.add_argument(
         "--spotify-playlist-default-period",
         type=str,
-        help="Default Subreddit time filter for a Spotify playlist",
+        help="Default subreddit time filter for a Spotify playlist.",
     )
     spotify_parser.add_argument(
         "--spotify-playlist-default-type",
         type=str,
-        help="Default Subreddit post filter for a Spotify playlist",
+        help="Default subreddit post filter for a Spotify playlist.",
     )
     spotify_parser.add_argument(
         "--spotify-playlist-from-upload",
         action="store_true",
         help=(
-            "Trigger creating a Spotify playlist using the Discord webhook "
-            "output of a music upload"
+            "Flag to trigger building a Spotify playlist using the copied "
+            "Discord webhook output of a music upload."
         ),
     )
     spotify_parser.add_argument(
         "--spotify-playlist-fuzz-ratio",
         type=int,
-        help="Minimum similarity to add track to a playlist",
+        help="Minimum similarity to add track to a playlist.",
     )
     spotify_parser.add_argument(
         "--spotify-playlist-post-limit",
         type=int,
-        help="Maximum Subreddit posts to query for each playlist",
+        help="Maximum subreddit posts to query for each playlist.",
     )
     spotify_parser.add_argument(
         "--spotify-playlist-subreddits",
         type=parse_json,
         help=(
-            "List of Subreddits configs to generate playlists from; YAML "
-            'strings with "name", "type", "period", and "limit" keys'
+            "List of subreddits configs to build playlists from.\nFormat as "
+            'a JSON string containing a list of dictionaries with "name", '
+            '"type", "period", and "limit" keys.\nNote: "name" is required '
+            "while the other keys are optional.\nExample:\n  "
+            '\'[{"name": "jungle"}, {"name": "techno", "type": "top", '
+            '"period": "week", "limit": 75}]\''
         ),
     )
     spotify_parser.add_argument(
         "--spotify-playlists",
         action="store_true",
-        help="Trigger building Spotify playlists",
+        help="Flag to trigger building Spotify playlists.",
     )
     spotify_parser.add_argument(
         "--spotify-redirect-uri",
         type=str,
-        help="Spotify API redirect URI",
+        help="Spotify API redirect URI.",
     )
     spotify_parser.add_argument(
         "--spotify-username",
         type=str,
-        help="Spotify user to maintain playlists for",
+        help="Spotify user to build playlists for.",
     )
 
     ###########################################################################
     # Sub-command for the sync package.
     ###########################################################################
-    sync_parser = subparsers.add_parser("sync")
+    sync_parser = subparsers.add_parser(
+        name="sync",
+        help=(
+            'Sync audio files and DJ collections between your "--usb-path" '
+            "and the Beatcloud."
+        ),
+        formatter_class=RawTextHelpFormatter,
+    )
     sync_parser.add_argument(
         "--artist-first",
         action="store_true",
         help=(
             "Indicate that Beatcloud tracks are in the format "
-            "`Artist - Track Title` instead of `Track Title - Artist`"
+            '"Artist - Track Title" instead of "Track Title - Artist".\nThe '
+            "ordering is important for any operation that compares your "
+            "tracks' filenames with Spotify tracks or other files...\n"
+            'This includes "--spotify-playlist-from-upload", '
+            '"--download-spotify-playlist", "--spotify-playlists", and '
+            '"--check-tracks".'
         ),
     )
     sync_parser.add_argument(
         "--aws-profile",
         type=str,
-        help="AWS config profile",
+        help="AWS config profile.",
     )
     sync_parser.add_argument(
         "--aws-use-date-modified",
         action="store_true",
         help=(
-            'Drop --size-only flag for "aws s3 sync" command; '
-            '"--aws-use-date-modified" will permit re-downloading/'
-            "re-uploading files if the date modified field changes"
+            'Drop the "--size-only" flag for "aws s3 sync" command; '
+            '"--aws-use-date-modified" will permit re-syncing files if the '
+            "date modified field changes."
         ),
     )
     sync_parser.add_argument(
         "--discord-url",
         type=str,
-        help="Discord webhook URL",
+        help="Discord webhook URL used to post uploaded tracks.",
     )
     sync_parser.add_argument(
         "--download-collection",
         action="store_true",
         help=(
-            "Trigger downloading the collection of IMPORT_USER from the "
-            "Beatcloud"
+            'Flag to trigger downloading the collection of "--import-user" '
+            "from the Beatcloud."
         ),
     )
     sync_parser.add_argument(
         "--download-exclude-dirs",
         type=convert_to_paths,
         nargs="+",
         action=NonEmptyListElementAction,
-        help="Paths to exclude when downloading from the Beatcloud",
+        help=(
+            "List of paths to exclude when downloading tracks from the "
+            "Beatcloud."
+        ),
     )
     sync_parser.add_argument(
         "--download-include-dirs",
         type=convert_to_paths,
         nargs="+",
         action=NonEmptyListElementAction,
-        help="Paths to include when downloading from the Beatcloud",
+        help=(
+            "List of paths to include when downloading tracks from the "
+            "Beatcloud."
+        ),
     )
     sync_parser.add_argument(
         "--download-music",
         action="store_true",
-        help="Trigger downloading new tracks from the Beatcloud",
+        help="Flag to trigger downloading tracks from the Beatcloud.",
     )
     sync_parser.add_argument(
         "--download-spotify-playlist",
         type=str,
-        help="Playlist name containing tracks to download from the Beatcloud",
+        help="Playlist name containing tracks to download from the Beatcloud.",
     )
     sync_parser.add_argument(
         "--dryrun",
         action="store_true",
-        help='Show result of "aws s3 sync" command without running it',
+        help=(
+            'Show result of "--upload-music" or "--download-music" commands '
+            "without actually running them."
+        ),
     )
     sync_parser.add_argument(
         "--import-user",
         type=str,
-        help="USER whose COLLECTION_PATH you're downloading",
+        help='"--user" whose "--collection-path" you\'re downloading.',
     )
     sync_parser.add_argument(
         "--upload-collection",
         action="store_true",
         help=(
-            "Trigger uploading the collection of IMPORT_USER from the "
-            "Beatcloud"
+            'Flag to trigger uploading the collection of "--import_user" from '
+            "the Beatcloud."
         ),
     )
     sync_parser.add_argument(
         "--upload-exclude-dirs",
         type=convert_to_paths,
         nargs="+",
         action=NonEmptyListElementAction,
-        help="List of paths to exclude when uploading to the Beatcloud",
+        help=(
+            "List of paths to exclude when uploading tracks to the Beatcloud."
+        ),
     )
     sync_parser.add_argument(
         "--upload-include-dirs",
         type=convert_to_paths,
         nargs="+",
         action=NonEmptyListElementAction,
-        help="List of paths to include when uploading to the Beatcloud",
+        help=(
+            "List of paths to include when uploading tracks to the Beatcloud."
+        ),
     )
     sync_parser.add_argument(
         "--upload-music",
         action="store_true",
-        help="Trigger uploading new tracks from the Beatcloud",
+        help="Flag to trigger uploading tracks to the Beatcloud.",
     )
     sync_parser.add_argument(
         "--usb-path",
         type=convert_to_paths,
-        help="Path to a drive with audio files",
+        help=(
+            "Path to a drive containing completely and exclusively your set of"
+            " audio files."
+        ),
     )
     sync_parser.add_argument(
         "--user",
         type=str,
-        help="Username of the current user",
+        help=(
+            "Username of the current user.\nIf left empty, your operating "
+            "system username will be used.\nMake sure you set this manually to"
+            " a consistent value so you don't create duplicate track "
+            'collections in the Beatcloud and on your "--usb-path".'
+        ),
     )
 
     ###########################################################################
     # Sub-command for the utils package.
     ###########################################################################
-    utils_parser = subparsers.add_parser("utils")
+    utils_parser = subparsers.add_parser(
+        name="utils",
+        help=(
+            "Utilities that don't fit into any of the other packages.\n  - "
+            "comparing tracks located in a list of Spotify playlists and/or a "
+            "list of local paths to tracks in the Beatcloud to determine if "
+            "you have redundancies\n  - downloading audio files from a URL "
+            "containing embedded audio (e.g. Soundcloud)"
+        ),
+        formatter_class=RawTextHelpFormatter,
+    )
     utils_parser.add_argument(
         "--check-tracks",
         action="store_true",
         help=(
-            "Trigger checking for track overlap between the Beatcloud and"
-            "CHECK_TRACKS_LOCAL_DIRS and / or CHECK_TRACKS_SPOTIFY_PLAYLISTS"
+            "Flag to trigger checking for track overlap between the Beatcloud "
+            'and "--check-tracks-local-dirs" and / or '
+            '"--check-tracks-spotify-playlists".'
         ),
     )
     utils_parser.add_argument(
         "--check-tracks-fuzz-ratio",
         type=int,
         help=(
             "Minimum similarity to indicate overlap between Beatcloud and "
-            "Spotify / local tracks"
+            "Spotify / local tracks."
         ),
     )
     utils_parser.add_argument(
         "--check-tracks-local-dirs",
         type=convert_to_paths,
         nargs="+",
         action=NonEmptyListElementAction,
-        help="List of local directories to check against the Beatcloud",
+        help="List of local directories to check against the Beatcloud.",
     )
     utils_parser.add_argument(
         "--check-tracks-spotify-playlists",
         type=str,
         nargs="+",
-        help="List of Spotify playlist names to check against the Beatcloud",
+        help="List of Spotify playlist names to check against the Beatcloud.",
     )
     utils_parser.add_argument(
         "--url-download",
         type=str,
-        help="URL to download audio file(s) from",
+        help="URL to download audio file(s) from.",
     )
     utils_parser.add_argument(
         "--url-download-destination",
         type=convert_to_paths,
-        help="Location to download audio file(s) to",
+        help="Location to download audio file(s) to.",
     )
 
     ###########################################################################
     ###########################################################################
 
     args = parser.parse_args()
 
@@ -511,15 +594,15 @@
 ) -> Dict[Any, Any]:
     """Filters out the superclass key: value pairs of a subclass.
 
     Args:
         sub_config: Instance of any subclass of BaseConfig.
 
     Returns:
-        Dictionary containing just the keys unique to `sub_config`.
+        Dictionary containing just the keys unique to "sub_config".
     """
     super_keys = set(BaseConfig.__fields__)
     return {
         k: v for k, v in sub_config.dict().items() if k not in super_keys
     }
```

### Comparing `dj_beatcloud-2.6.0b7/djtools/spotify/__init__.py` & `dj_beatcloud-2.6.0b8/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/spotify/config.py` & `dj_beatcloud-2.6.0b8/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/spotify/helpers.py` & `dj_beatcloud-2.6.0b8/djtools/spotify/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/spotify/playlist_builder.py` & `dj_beatcloud-2.6.0b8/djtools/spotify/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/sync/__init__.py` & `dj_beatcloud-2.6.0b8/djtools/sync/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 from djtools.sync.helpers import upload_log
 from djtools.sync.sync_operations import (
     download_collection, download_music, upload_collection, upload_music
 )
 
 
 SYNC_OPERATIONS = {
-    'DOWNLOAD_COLLECTION': download_collection,
-    'DOWNLOAD_MUSIC': download_music,
-    'UPLOAD_COLLECTION': upload_collection,
-    'UPLOAD_MUSIC': upload_music,
+    "DOWNLOAD_COLLECTION": download_collection,
+    "DOWNLOAD_MUSIC": download_music,
+    "DOWNLOAD_SPOTIFY_PLAYLIST": download_music,
+    "UPLOAD_COLLECTION": upload_collection,
+    "UPLOAD_MUSIC": upload_music,
 }
 
 __all__ = (
     "download_collection",
     "download_music",
     "SyncConfig",
     "SYNC_OPERATIONS",
```

### Comparing `dj_beatcloud-2.6.0b7/djtools/sync/config.py` & `dj_beatcloud-2.6.0b8/djtools/sync/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,35 +72,39 @@
             if not self.AWS_PROFILE:
                 msg = "Config must include AWS_PROFILE for sync operations"
                 logger.critical(msg)
                 raise RuntimeError(msg)
 
         os.environ["AWS_PROFILE"] = self.AWS_PROFILE
 
-        if (
-            any([self.DOWNLOAD_MUSIC, self.UPLOAD_MUSIC]) and
-            (not self.USB_PATH or not self.USB_PATH.exists())
-        ):
+        if any([self.DOWNLOAD_MUSIC, self.UPLOAD_MUSIC]) and not self.USB_PATH:
             msg = (
                 "Config must include USB_PATH for both DOWNLOAD_MUSIC and "
                 "UPLOAD_MUSIC sync operations"
             )
             logger.critical(msg)
             raise RuntimeError(msg)
 
+        if (
+            any([self.DOWNLOAD_MUSIC, self.UPLOAD_MUSIC]) and
+            not self.USB_PATH.exists()
+        ):
+            msg = f'Configured USB_PATH "{self.USB_PATH}" was not found!'
+            logger.critical(msg)
+            raise RuntimeError(msg)
+
         if self.UPLOAD_MUSIC and not self.DISCORD_URL:
             logger.warning(
                 'DISCORD_URL is not configured...set this for "New Music" '
                 "discord messages!"
             )
 
         if self.DOWNLOAD_COLLECTION and not self.IMPORT_USER:
             raise RuntimeError(
-                "Unable to import from collection of IMPORT_USER "
-                f'"{self.IMPORT_USER}"'
+                "IMPORT_USER must be set to download a collection"
             )
 
     @validator("USB_PATH")
     @classmethod
     def usb_path_as_pathlib_path(cls, value: str) -> Union[Path, str]:
         """Validator to convert USB_PATH to a pathlib.Path.
```

### Comparing `dj_beatcloud-2.6.0b7/djtools/sync/helpers.py` & `dj_beatcloud-2.6.0b8/djtools/sync/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/sync/sync_operations.py` & `dj_beatcloud-2.6.0b8/djtools/sync/sync_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,16 +34,19 @@
     if config.DOWNLOAD_SPOTIFY_PLAYLIST:
         user = config.DOWNLOAD_SPOTIFY_PLAYLIST.split("Uploads")[0].strip()
         beatcloud_tracks, beatcloud_matches = compare_tracks(
             config,
             beatcloud_tracks=beatcloud_tracks,
             download_spotify_playlist=config.DOWNLOAD_SPOTIFY_PLAYLIST,
         )
+        if not beatcloud_matches:
+            logger.warning("No Beatcloud matches were found! Make sure you've supplied to correct playlist name.")
+            return
         config.DOWNLOAD_INCLUDE_DIRS = [
-            (Path(user) / path.split(f"{Path(user)}/")[-1])
+            (Path(user) / path.as_posix().split(f"{Path(user)}/")[-1])
             for path in beatcloud_matches
         ]
         config.DOWNLOAD_EXCLUDE_DIRS = []
 
     logger.info("Downloading track collection...")
     dest = Path(config.USB_PATH) / "DJ Music"
     glob_path = (Path("**") / "*.*").as_posix()
```

### Comparing `dj_beatcloud-2.6.0b7/djtools/utils/__init__.py` & `dj_beatcloud-2.6.0b8/djtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/utils/check_tracks.py` & `dj_beatcloud-2.6.0b8/djtools/utils/check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/utils/config.py` & `dj_beatcloud-2.6.0b8/djtools/utils/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/utils/helpers.py` & `dj_beatcloud-2.6.0b8/djtools/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/djtools/utils/url_download.py` & `dj_beatcloud-2.6.0b8/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b7/setup.py` & `dj_beatcloud-2.6.0b8/setup.py`

 * *Files identical despite different names*

