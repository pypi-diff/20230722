# Comparing `tmp/nova-playlist-0.3.0.tar.gz` & `tmp/nova_playlist-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nova-playlist-0.3.0.tar", last modified: Thu Feb 11 02:40:56 2021, max compression
+gzip compressed data, was "nova_playlist-0.4.0.tar", max compression
```

## Comparing `nova-playlist-0.3.0.tar` & `nova_playlist-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1069 2020-04-04 03:58:49.260476 nova-playlist-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     2187 2021-02-11 02:35:09.454821 nova-playlist-0.3.0/README.md
--rw-r--r--   0        0        0     2535 2021-02-11 02:37:58.504007 nova-playlist-0.3.0/nova_playlist.py
--rw-r--r--   0        0        0      483 2021-02-11 02:37:58.504007 nova-playlist-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2996 2021-02-11 02:40:56.473800 nova-playlist-0.3.0/setup.py
--rw-r--r--   0        0        0     2775 2021-02-11 02:40:56.474833 nova-playlist-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2020-04-04 03:58:49.260476 nova_playlist-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     2395 2023-07-22 17:26:02.132299 nova_playlist-0.4.0/README.md
+-rw-r--r--   0        0        0      544 2023-07-22 17:26:02.132299 nova_playlist-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-22 17:26:02.132299 nova_playlist-0.4.0/src/nova_playlist/__init__.py
+-rw-r--r--   0        0        0     1429 2023-07-22 17:26:02.135632 nova_playlist-0.4.0/src/nova_playlist/cli.py
+-rw-r--r--   0        0        0     1546 2023-07-22 17:26:02.135632 nova_playlist-0.4.0/src/nova_playlist/nova.py
+-rw-r--r--   0        0        0     3759 2023-07-22 17:26:02.135632 nova_playlist-0.4.0/src/nova_playlist/parser.py
+-rw-r--r--   0        0        0     3042 1970-01-01 00:00:00.000000 nova_playlist-0.4.0/PKG-INFO
```

### Comparing `nova-playlist-0.3.0/LICENSE.txt` & `nova_playlist-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nova-playlist-0.3.0/README.md` & `nova_playlist-0.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,53 @@
 # nova-playlist
 
-[Radio Nova][0] plays amazing music at night.
+[Radio Nova][] plays amazing music at night.
 
-There could be Fela Kuti, then hip-hop from the 1990s, then Motown, then Tuareg
-music, then some minimal electro, then Hungarian folk songs, then David Bowie,
-then Amazonian cumbia, then a French song that was released last month, then
-Sufi devotional music from Punjab, then Nina Simone, then a tune from the
-north-east of Brazil. It's wild.
-
-And if you, like me, live a few time zones west of Paris, you get to
-conveniently enjoy it all in the evening instead of having to be up in the
-middle of the night!
-
-Often, I want to know which song is currently playing, so that I can find out
-more about it and the artist. There is a [page][1] where one can find what
-music has aired on the Radio in the past, but it's buggy and a bit annoying to
-use. And even if the page was great to use, it wouldn't be as great as using
-the command line for it! _Ergo_ this little script.
+There could be Fela Kuti, then hip-hop from the 1990s, then Motown, then Tuareg music, then some minimal electro, then Hungarian folk songs, then David Bowie, then Amazonian cumbia, then a French song that was released last month, then Sufi devotional music from Punjab, then Nina Simone, then a tune from the north-east of Brazil.
+It's wild.
 
+And if you, like me, live a few time zones west of Paris, you get to conveniently enjoy it all in the evening instead of having to be up in the middle of the night!
 
-## Installation
-
-    pipx install nova-playlist
+Often, I want to know which song is currently playing, so that I can find out more about it and the artist.
+There is a [page][song-history] where one can find what music has aired on the Radio in the past, but it's buggy and a bit annoying to use.
+And even if the page was great to use, it wouldn't be as great as using the command line for it!
+_Ergo_ this little program.
 
-Or use `pip`.
+## Installation
 
-Python 3.9 is required, along with a IANA timezone database on your system
-(Unix-y systems should have that already, otherwise you can try installing
-`tzdata` from PyPI.)
+The package is available on the Python Package Index (PyPI) as [nova-playlist][].
+The recommended way of installing it is with [pipx][].
 
+Python 3.9 or above is required, along with a IANA timezone database on your system.
+Unix-y systems should alreay have it, otherwise you can try installing `tzdata` from PyPI.
 
 ## Usage
 
     $ nova
     20:36  Orchestra Baobab - Liiti Liiti
     20:30  Chico Buarque - Construção
     20:27  Abner Jay - My Middle Name Is The Blues
     20:23  Brigitte Fontaine - Le Goudron
     ...
 
-By default, the times are in the "Canada/Atlantic" time zone. If you want them
-in another time zone, you can pass the `-t`/`--timezone` argument:
+By default, the times are in the "Canada/Atlantic" time zone.
+If you want them in another time zone, you can pass the `-t`/`--timezone` argument:
 
     $ nova -t Europe/Berlin
     03:12  Los Camperos De Valles - El Gallo
     03:09  Karen Dalton - Something On Your Mind
     03:04  Têtes Raides & Yann Tiersen - Ginette
     02:59  The Toraia Orchestra Of Algiers - Nar Houbi Techaal
     ...
 
-
 ## Caveat
 
-This can be somewhat brittle. Sometimes, the data stops being updated on the
-site. Or the data gets updated, but the timestamps are 11 minutes off from
-what's playing in the stream. And of course, if they ever change their HTML
-structure in any way, this could also start failing miserably. But so far, so
-good!
-
-
-[0]: https://www.nova.fr/radios/nova-la-nuit/
-[1]: https://www.nova.fr/radios/radio-nova/
+This can be somewhat brittle.
+Sometimes, the data stops being updated on the site.
+Or the data gets updated, but the timestamps are 11 minutes off from what's playing in the stream.
+Finally, if Radio Nova changes their HTML structure in any way, this could start failing miserably.
+But so far, so good!
+
+[Radio Nova]: https://www.nova.fr/radios/nova-la-nuit/
+[nova-playlist]: https://pypi.org/project/nova-playlist/
+[pipx]: https://pypa.github.io/pipx/
+[song-history]: https://www.nova.fr/radios/radio-nova/
```

### Comparing `nova-playlist-0.3.0/setup.py` & `nova_playlist-0.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,71 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nova-playlist
+Version: 0.4.0
+Summary: Display information about the songs that recently played on Radio Nova
+Home-page: https://github.com/rafikdraoui/nova-playlist
+License: MIT
+Author: Rafik Draoui
+Author-email: rafik@rafik.ca
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/rafikdraoui/nova-playlist
+Description-Content-Type: text/markdown
 
-modules = \
-['nova_playlist']
-install_requires = \
-['beautifulsoup4>=4.8,<5.0']
-
-entry_points = \
-{'console_scripts': ['nova = nova_playlist:main']}
-
-setup_kwargs = {
-    'name': 'nova-playlist',
-    'version': '0.3.0',
-    'description': 'Display information about the songs that recently played on Radio Nova',
-    'long_description': '# nova-playlist\n\n[Radio Nova][0] plays amazing music at night.\n\nThere could be Fela Kuti, then hip-hop from the 1990s, then Motown, then Tuareg\nmusic, then some minimal electro, then Hungarian folk songs, then David Bowie,\nthen Amazonian cumbia, then a French song that was released last month, then\nSufi devotional music from Punjab, then Nina Simone, then a tune from the\nnorth-east of Brazil. It\'s wild.\n\nAnd if you, like me, live a few time zones west of Paris, you get to\nconveniently enjoy it all in the evening instead of having to be up in the\nmiddle of the night!\n\nOften, I want to know which song is currently playing, so that I can find out\nmore about it and the artist. There is a [page][1] where one can find what\nmusic has aired on the Radio in the past, but it\'s buggy and a bit annoying to\nuse. And even if the page was great to use, it wouldn\'t be as great as using\nthe command line for it! _Ergo_ this little script.\n\n\n## Installation\n\n    pipx install nova-playlist\n\nOr use `pip`.\n\nPython 3.9 is required, along with a IANA timezone database on your system\n(Unix-y systems should have that already, otherwise you can try installing\n`tzdata` from PyPI.)\n\n\n## Usage\n\n    $ nova\n    20:36  Orchestra Baobab - Liiti Liiti\n    20:30  Chico Buarque - Construção\n    20:27  Abner Jay - My Middle Name Is The Blues\n    20:23  Brigitte Fontaine - Le Goudron\n    ...\n\nBy default, the times are in the "Canada/Atlantic" time zone. If you want them\nin another time zone, you can pass the `-t`/`--timezone` argument:\n\n    $ nova -t Europe/Berlin\n    03:12  Los Camperos De Valles - El Gallo\n    03:09  Karen Dalton - Something On Your Mind\n    03:04  Têtes Raides & Yann Tiersen - Ginette\n    02:59  The Toraia Orchestra Of Algiers - Nar Houbi Techaal\n    ...\n\n\n## Caveat\n\nThis can be somewhat brittle. Sometimes, the data stops being updated on the\nsite. Or the data gets updated, but the timestamps are 11 minutes off from\nwhat\'s playing in the stream. And of course, if they ever change their HTML\nstructure in any way, this could also start failing miserably. But so far, so\ngood!\n\n\n[0]: https://www.nova.fr/radios/nova-la-nuit/\n[1]: https://www.nova.fr/radios/radio-nova/\n',
-    'author': 'Rafik Draoui',
-    'author_email': 'rafik@rafik.ca',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/rafikdraoui/nova-playlist',
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+# nova-playlist
 
+[Radio Nova][] plays amazing music at night.
+
+There could be Fela Kuti, then hip-hop from the 1990s, then Motown, then Tuareg music, then some minimal electro, then Hungarian folk songs, then David Bowie, then Amazonian cumbia, then a French song that was released last month, then Sufi devotional music from Punjab, then Nina Simone, then a tune from the north-east of Brazil.
+It's wild.
+
+And if you, like me, live a few time zones west of Paris, you get to conveniently enjoy it all in the evening instead of having to be up in the middle of the night!
+
+Often, I want to know which song is currently playing, so that I can find out more about it and the artist.
+There is a [page][song-history] where one can find what music has aired on the Radio in the past, but it's buggy and a bit annoying to use.
+And even if the page was great to use, it wouldn't be as great as using the command line for it!
+_Ergo_ this little program.
+
+## Installation
+
+The package is available on the Python Package Index (PyPI) as [nova-playlist][].
+The recommended way of installing it is with [pipx][].
+
+Python 3.9 or above is required, along with a IANA timezone database on your system.
+Unix-y systems should alreay have it, otherwise you can try installing `tzdata` from PyPI.
+
+## Usage
+
+    $ nova
+    20:36  Orchestra Baobab - Liiti Liiti
+    20:30  Chico Buarque - Construção
+    20:27  Abner Jay - My Middle Name Is The Blues
+    20:23  Brigitte Fontaine - Le Goudron
+    ...
+
+By default, the times are in the "Canada/Atlantic" time zone.
+If you want them in another time zone, you can pass the `-t`/`--timezone` argument:
+
+    $ nova -t Europe/Berlin
+    03:12  Los Camperos De Valles - El Gallo
+    03:09  Karen Dalton - Something On Your Mind
+    03:04  Têtes Raides & Yann Tiersen - Ginette
+    02:59  The Toraia Orchestra Of Algiers - Nar Houbi Techaal
+    ...
+
+## Caveat
+
+This can be somewhat brittle.
+Sometimes, the data stops being updated on the site.
+Or the data gets updated, but the timestamps are 11 minutes off from what's playing in the stream.
+Finally, if Radio Nova changes their HTML structure in any way, this could start failing miserably.
+But so far, so good!
+
+[Radio Nova]: https://www.nova.fr/radios/nova-la-nuit/
+[nova-playlist]: https://pypi.org/project/nova-playlist/
+[pipx]: https://pypa.github.io/pipx/
+[song-history]: https://www.nova.fr/radios/radio-nova/
 
-setup(**setup_kwargs)
```

