# Comparing `tmp/readtime-2.0.0.tar.gz` & `tmp/readtime-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readtime-2.0.0.tar", last modified: Fri May 20 04:46:29 2022, max compression
+gzip compressed data, was "readtime-3.0.0.tar", last modified: Sat Jul 22 06:50:22 2023, max compression
```

## Comparing `readtime-2.0.0.tar` & `readtime-3.0.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2022-05-20 04:46:29.295578 readtime-2.0.0/
--rw-r--r--   0 user       (501) staff       (20)      253 2022-05-20 04:43:33.000000 readtime-2.0.0/AUTHORS
--rw-r--r--   0 user       (501) staff       (20)     1055 2022-05-20 04:26:27.000000 readtime-2.0.0/HISTORY.rst
--rw-r--r--   0 user       (501) staff       (20)     1343 2019-04-03 07:31:08.000000 readtime-2.0.0/LICENSE
--rw-r--r--   0 user       (501) staff       (20)       88 2016-08-23 19:08:46.000000 readtime-2.0.0/MANIFEST.in
--rw-r--r--   0 user       (501) staff       (20)     3451 2022-05-20 04:46:29.295739 readtime-2.0.0/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     2442 2022-05-20 04:38:12.000000 readtime-2.0.0/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2022-05-20 04:46:29.273296 readtime-2.0.0/readtime/
--rw-r--r--   0 user       (501) staff       (20)      433 2022-05-20 04:46:10.000000 readtime-2.0.0/readtime/__about__.py
--rw-r--r--   0 user       (501) staff       (20)      281 2016-08-23 21:31:29.000000 readtime-2.0.0/readtime/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1064 2017-03-25 23:32:32.000000 readtime-2.0.0/readtime/_compat.py
--rw-r--r--   0 user       (501) staff       (20)      764 2019-02-13 05:50:22.000000 readtime-2.0.0/readtime/api.py
--rw-r--r--   0 user       (501) staff       (20)     2155 2019-02-13 05:58:14.000000 readtime-2.0.0/readtime/result.py
--rw-r--r--   0 user       (501) staff       (20)     2868 2019-02-13 06:07:19.000000 readtime-2.0.0/readtime/utils.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2022-05-20 04:46:29.295299 readtime-2.0.0/readtime.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     3451 2022-05-20 04:46:28.000000 readtime-2.0.0/readtime.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      391 2022-05-20 04:46:29.000000 readtime-2.0.0/readtime.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2022-05-20 04:46:28.000000 readtime-2.0.0/readtime.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2016-08-23 23:48:05.000000 readtime-2.0.0/readtime.egg-info/not-zip-safe
--rw-r--r--   0 user       (501) staff       (20)       52 2022-05-20 04:46:29.000000 readtime-2.0.0/readtime.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        9 2022-05-20 04:46:29.000000 readtime-2.0.0/readtime.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)       52 2022-05-20 04:14:56.000000 readtime-2.0.0/requirements.txt
--rw-r--r--   0 user       (501) staff       (20)      135 2022-05-20 04:46:29.296320 readtime-2.0.0/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)     1404 2022-05-20 04:24:19.000000 readtime-2.0.0/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-22 06:50:22.018106 readtime-3.0.0/
+-rw-r--r--   0 user       (501) staff       (20)      253 2022-05-20 04:43:33.000000 readtime-3.0.0/AUTHORS
+-rw-r--r--   0 user       (501) staff       (20)     1205 2023-07-22 06:49:24.000000 readtime-3.0.0/CHANGES.md
+-rw-r--r--   0 user       (501) staff       (20)     1343 2019-04-03 07:31:08.000000 readtime-3.0.0/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)       87 2023-07-22 06:45:36.000000 readtime-3.0.0/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     3421 2023-07-22 06:50:22.018243 readtime-3.0.0/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     2461 2023-07-22 06:39:23.000000 readtime-3.0.0/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-22 06:50:22.015647 readtime-3.0.0/readtime/
+-rw-r--r--   0 user       (501) staff       (20)      433 2023-07-22 06:49:51.000000 readtime-3.0.0/readtime/__about__.py
+-rw-r--r--   0 user       (501) staff       (20)      257 2023-07-22 06:39:23.000000 readtime-3.0.0/readtime/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      740 2023-07-22 06:39:23.000000 readtime-3.0.0/readtime/api.py
+-rw-r--r--   0 user       (501) staff       (20)     1638 2023-07-22 06:39:23.000000 readtime-3.0.0/readtime/result.py
+-rw-r--r--   0 user       (501) staff       (20)     2771 2023-07-22 06:39:23.000000 readtime-3.0.0/readtime/utils.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-22 06:50:22.017848 readtime-3.0.0/readtime.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3421 2023-07-22 06:50:21.000000 readtime-3.0.0/readtime.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      370 2023-07-22 06:50:21.000000 readtime-3.0.0/readtime.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-07-22 06:50:21.000000 readtime-3.0.0/readtime.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2016-08-23 23:48:05.000000 readtime-3.0.0/readtime.egg-info/not-zip-safe
+-rw-r--r--   0 user       (501) staff       (20)       52 2023-07-22 06:50:21.000000 readtime-3.0.0/readtime.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        9 2023-07-22 06:50:21.000000 readtime-3.0.0/readtime.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)       52 2022-05-20 04:14:56.000000 readtime-3.0.0/requirements.txt
+-rw-r--r--   0 user       (501) staff       (20)      135 2023-07-22 06:50:22.018735 readtime-3.0.0/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)     1356 2023-07-22 06:32:42.000000 readtime-3.0.0/setup.py
```

### Comparing `readtime-2.0.0/LICENSE` & `readtime-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `readtime-2.0.0/PKG-INFO` & `readtime-3.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: readtime
-Version: 2.0.0
+Version: 3.0.0
 Summary: Calculates the time some text takes the average human to read, based on Medium's read time forumula
 Home-page: https://github.com/alanhamlett/readtime
 Author: Alan Hamlett
 Author-email: alan.hamlett@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 # readtime
 
-[![Tests](https://img.shields.io/github/workflow/status/alanhamlett/readtime/Tests/master)](https://github.com/alanhamlett/readtime/actions/workflows/tests.yml)
+[![Tests](https://img.shields.io/github/actions/workflow/status/alanhamlett/readtime/tests.yml?branch=master)](https://github.com/alanhamlett/readtime/actions/workflows/tests.yml)
 [![Coverage](https://codecov.io/gh/alanhamlett/readtime/branch/master/graph/badge.svg?token=EbUnuwbra3)](https://codecov.io/gh/alanhamlett/readtime)
 
 Calculates the time some text takes the average human to read, based on Medium's [read time forumula](https://help.medium.com/hc/en-us/articles/214991667-Read-time).
 
 
 ### Algorithm
```

### Comparing `readtime-2.0.0/README.md` & `readtime-3.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # readtime
 
-[![Tests](https://img.shields.io/github/workflow/status/alanhamlett/readtime/Tests/master)](https://github.com/alanhamlett/readtime/actions/workflows/tests.yml)
+[![Tests](https://img.shields.io/github/actions/workflow/status/alanhamlett/readtime/tests.yml?branch=master)](https://github.com/alanhamlett/readtime/actions/workflows/tests.yml)
 [![Coverage](https://codecov.io/gh/alanhamlett/readtime/branch/master/graph/badge.svg?token=EbUnuwbra3)](https://codecov.io/gh/alanhamlett/readtime)
 
 Calculates the time some text takes the average human to read, based on Medium's [read time forumula](https://help.medium.com/hc/en-us/articles/214991667-Read-time).
 
 
 ### Algorithm
```

### Comparing `readtime-2.0.0/readtime/api.py` & `readtime-3.0.0/readtime/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
     readtime.api
     ~~~~~~~~~~~~
 
     Contains public methods.
 
     :copyright: (c) 2016 Alan Hamlett.
```

### Comparing `readtime-2.0.0/readtime/result.py` & `readtime-3.0.0/readtime/result.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,50 @@
-# -*- coding: utf-8 -*-
 """
     readtime.result
     ~~~~~~~~~~~~~~~
 
     For returning read time results.
 
     :copyright: (c) 2016 Alan Hamlett.
     :license: BSD, see LICENSE for more details.
 """
 
 
-from __future__ import division
-
 import math
 import operator
 from datetime import timedelta
 
-from ._compat import u, IS_PY2
-
 
-class Result(object):
+class Result:
     delta = None
 
     def __init__(self, seconds=None, wpm=None):
         self.wpm = wpm
         self.delta = timedelta(seconds=seconds)
         self._add_operator_methods()
 
     def __repr__(self):
-        return u(self.text + ' read')
-
-    def __unicode__(self):
-        return self.__repr__()  # pragma: nocover
+        return self.text + ' read'
 
     def __str__(self):
-        if IS_PY2:
-            return self.__repr__().encode('utf-8')
-        else:
-            return self.__repr__()
+        return self.__repr__()
 
     @property
     def seconds(self):
-        return int(self.total_seconds(self.delta))
+        return int(self.delta.total_seconds())
 
     @property
     def minutes(self):
-        minutes = int(math.ceil(self.seconds / 60))
-        if minutes < 1:  # Medium's formula has a minimum of 1 min read time
-            minutes = 1
+        minutes = math.ceil(self.seconds / 60)
+        minutes = max(1, minutes)  # Medium's formula has a minimum of 1 min read time
         return minutes
 
     @property
     def text(self):
-        return u('{minutes} min').format(minutes=self.minutes)
-
-    def total_seconds(self, delta):
-        """timedelta.total_seconds for Python2.6 compatibility."""
-
-        return ((delta.microseconds + (delta.seconds + delta.days * 24 * 3600) * 1e6) / 1e6)
+        return f'{self.minutes} min'
 
     def _add_operator_methods(self):
         for op in dir(operator):
             can_set = (getattr(self.__class__, op, None) is None and
                        getattr(self.delta, op, None) is not None and
                        op.startswith('__') and
                        op.endswith('__'))
@@ -72,10 +55,10 @@
                     pass
 
     def _create_method(self, op):
         fn = getattr(self.delta, op)
 
         def method(cls, other, *args, **kwargs):
             delta = fn(other.delta)
-            return Result(seconds=self.total_seconds(delta), wpm=self.wpm)
+            return Result(seconds=delta.total_seconds(), wpm=self.wpm)
 
         return method
```

### Comparing `readtime-2.0.0/readtime/utils.py` & `readtime-3.0.0/readtime/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-# -*- coding: utf-8 -*-
 """
     readtime.utils
     ~~~~~~~~~~~~~~
 
     Utility and non-public methods.
 
     :copyright: (c) 2016 Alan Hamlett.
     :license: BSD, see LICENSE for more details.
 """
 
 
-from __future__ import division
 
-import lxml
 import math
-import markdown2
 import re
+
+import lxml
+import markdown2
 from pyquery import PyQuery as pq
 
 from .result import Result
-from ._compat import u
 
 DEFAULT_WPM = 265  # Medium says they use 275 WPM but they actually use 265
 WORD_DELIMITER = re.compile(r'\W+')
 
 
 def read_time(content, format=None, wpm=None):
     """Returns the read time of some content.
@@ -51,15 +49,15 @@
 
     elif format == 'html':
         el = pq(content)
         text, images = parse_html(el)
         seconds = read_time_as_seconds(text, images=images, wpm=wpm)
 
     else:
-        raise Exception(u('Unsupported format: {0}').format(format))
+        raise Exception(f'Unsupported format: {format}')
 
     return Result(seconds=seconds, wpm=wpm)
 
 
 def read_time_as_seconds(text, images=0, wpm=None):
     """Returns the read time as seconds of some plain text.
 
@@ -71,19 +69,19 @@
         wpm = DEFAULT_WPM
 
     try:
         num_words = len(re.split(WORD_DELIMITER, text.strip()))
     except (AttributeError, TypeError):
         num_words = 0
 
-    seconds = int(math.ceil(num_words / wpm * 60))
+    seconds = math.ceil(num_words / wpm * 60)
 
     # add extra seconds for inline images
     delta = 12
-    for img in range(images):
+    for _ in range(images):
         seconds += delta
         if delta > 3:
             delta -= 1
 
     return seconds
```

### Comparing `readtime-2.0.0/readtime.egg-info/PKG-INFO` & `readtime-3.0.0/readtime.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: readtime
-Version: 2.0.0
+Version: 3.0.0
 Summary: Calculates the time some text takes the average human to read, based on Medium's read time forumula
 Home-page: https://github.com/alanhamlett/readtime
 Author: Alan Hamlett
 Author-email: alan.hamlett@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 # readtime
 
-[![Tests](https://img.shields.io/github/workflow/status/alanhamlett/readtime/Tests/master)](https://github.com/alanhamlett/readtime/actions/workflows/tests.yml)
+[![Tests](https://img.shields.io/github/actions/workflow/status/alanhamlett/readtime/tests.yml?branch=master)](https://github.com/alanhamlett/readtime/actions/workflows/tests.yml)
 [![Coverage](https://codecov.io/gh/alanhamlett/readtime/branch/master/graph/badge.svg?token=EbUnuwbra3)](https://codecov.io/gh/alanhamlett/readtime)
 
 Calculates the time some text takes the average human to read, based on Medium's [read time forumula](https://help.medium.com/hc/en-us/articles/214991667-Read-time).
 
 
 ### Algorithm
```

### Comparing `readtime-2.0.0/setup.py` & `readtime-3.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,13 @@
         'Environment :: Console',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Natural Language :: English',
         'Topic :: Software Development :: Build Tools',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

