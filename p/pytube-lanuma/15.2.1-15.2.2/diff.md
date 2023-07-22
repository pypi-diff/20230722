# Comparing `tmp/pytube-lanuma-15.2.1.tar.gz` & `tmp/pytube-lanuma-15.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytube-lanuma-15.2.1.tar", last modified: Thu Jul 20 19:01:34 2023, max compression
+gzip compressed data, was "pytube-lanuma-15.2.2.tar", last modified: Sat Jul 22 17:13:26 2023, max compression
```

## Comparing `pytube-lanuma-15.2.1.tar` & `pytube-lanuma-15.2.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 lanuma     (502) staff       (20)        0 2023-07-20 19:01:34.986892 pytube-lanuma-15.2.1/
--rw-r--r--   0 lanuma     (502) staff       (20)     1211 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/LICENSE
--rw-r--r--   0 lanuma     (502) staff       (20)       55 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/MANIFEST.in
--rw-r--r--   0 lanuma     (502) staff       (20)     5315 2023-07-20 19:01:34.986688 pytube-lanuma-15.2.1/PKG-INFO
--rw-r--r--   0 lanuma     (502) staff       (20)     4057 2023-06-26 09:01:35.000000 pytube-lanuma-15.2.1/README.md
-drwxr-xr-x   0 lanuma     (502) staff       (20)        0 2023-07-20 19:01:34.979262 pytube-lanuma-15.2.1/pytube/
--rw-r--r--   0 lanuma     (502) staff       (20)      592 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/pytube/__init__.py
--rw-r--r--   0 lanuma     (502) staff       (20)    15423 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/pytube/__main__.py
--rw-r--r--   0 lanuma     (502) staff       (20)     5648 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/pytube/captions.py
--rw-r--r--   0 lanuma     (502) staff       (20)    21912 2023-07-20 18:52:33.000000 pytube-lanuma-15.2.1/pytube/cipher.py
--rwxr-xr-x   0 lanuma     (502) staff       (20)    16641 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/pytube/cli.py
-drwxr-xr-x   0 lanuma     (502) staff       (20)        0 2023-07-20 19:01:34.980072 pytube-lanuma-15.2.1/pytube/contrib/
--rw-r--r--   0 lanuma     (502) staff       (20)        0 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/pytube/contrib/__init__.py
--rw-r--r--   0 lanuma     (502) staff       (20)     6576 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/pytube/contrib/channel.py
--rw-r--r--   0 lanuma     (502) staff       (20)    14204 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/pytube/contrib/playlist.py
--rw-r--r--   0 lanuma     (502) staff       (20)     8898 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/pytube/contrib/search.py
--rw-r--r--   0 lanuma     (502) staff       (20)     3907 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/pytube/exceptions.py
--rw-r--r--   0 lanuma     (502) staff       (20)    17798 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/pytube/extract.py
--rw-r--r--   0 lanuma     (502) staff       (20)     9794 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/pytube/helpers.py
--rw-r--r--   0 lanuma     (502) staff       (20)    15775 2023-06-26 09:53:58.000000 pytube-lanuma-15.2.1/pytube/innertube.py
--rw-r--r--   0 lanuma     (502) staff       (20)     4311 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/pytube/itags.py
--rw-r--r--   0 lanuma     (502) staff       (20)     1482 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/pytube/metadata.py
--rw-r--r--   0 lanuma     (502) staff       (20)      451 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/pytube/monostate.py
--rw-r--r--   0 lanuma     (502) staff       (20)     5931 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/pytube/parser.py
--rw-r--r--   0 lanuma     (502) staff       (20)    12844 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/pytube/query.py
--rw-r--r--   0 lanuma     (502) staff       (20)     8662 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/pytube/request.py
--rw-r--r--   0 lanuma     (502) staff       (20)    15288 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/pytube/streams.py
--rw-r--r--   0 lanuma     (502) staff       (20)       74 2023-07-20 19:01:27.000000 pytube-lanuma-15.2.1/pytube/version.py
-drwxr-xr-x   0 lanuma     (502) staff       (20)        0 2023-07-20 19:01:34.981543 pytube-lanuma-15.2.1/pytube_lanuma.egg-info/
--rw-r--r--   0 lanuma     (502) staff       (20)     5315 2023-07-20 19:01:34.000000 pytube-lanuma-15.2.1/pytube_lanuma.egg-info/PKG-INFO
--rw-r--r--   0 lanuma     (502) staff       (20)     1045 2023-07-20 19:01:34.000000 pytube-lanuma-15.2.1/pytube_lanuma.egg-info/SOURCES.txt
--rw-r--r--   0 lanuma     (502) staff       (20)        1 2023-07-20 19:01:34.000000 pytube-lanuma-15.2.1/pytube_lanuma.egg-info/dependency_links.txt
--rw-r--r--   0 lanuma     (502) staff       (20)       50 2023-07-20 19:01:34.000000 pytube-lanuma-15.2.1/pytube_lanuma.egg-info/entry_points.txt
--rw-r--r--   0 lanuma     (502) staff       (20)        7 2023-07-20 19:01:34.000000 pytube-lanuma-15.2.1/pytube_lanuma.egg-info/top_level.txt
--rw-r--r--   0 lanuma     (502) staff       (20)        1 2023-07-20 19:01:34.000000 pytube-lanuma-15.2.1/pytube_lanuma.egg-info/zip-safe
--rw-r--r--   0 lanuma     (502) staff       (20)       38 2023-07-20 19:01:34.986944 pytube-lanuma-15.2.1/setup.cfg
--rwxr-xr-x   0 lanuma     (502) staff       (20)     2000 2023-06-26 10:45:25.000000 pytube-lanuma-15.2.1/setup.py
-drwxr-xr-x   0 lanuma     (502) staff       (20)        0 2023-07-20 19:01:34.985602 pytube-lanuma-15.2.1/tests/
--rw-r--r--   0 lanuma     (502) staff       (20)       57 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/tests/__init__.py
--rw-r--r--   0 lanuma     (502) staff       (20)     4921 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/tests/conftest.py
-drwxr-xr-x   0 lanuma     (502) staff       (20)        0 2023-07-20 19:01:34.986328 pytube-lanuma-15.2.1/tests/contrib/
--rw-r--r--   0 lanuma     (502) staff       (20)     3122 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/tests/contrib/test_channel.py
--rw-r--r--   0 lanuma     (502) staff       (20)    11623 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/tests/contrib/test_playlist.py
--rw-r--r--   0 lanuma     (502) staff       (20)     5759 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/tests/test_captions.py
--rw-r--r--   0 lanuma     (502) staff       (20)     2736 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/tests/test_cipher.py
--rw-r--r--   0 lanuma     (502) staff       (20)    17295 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/tests/test_cli.py
--rw-r--r--   0 lanuma     (502) staff       (20)     3452 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/tests/test_exceptions.py
--rw-r--r--   0 lanuma     (502) staff       (20)     2957 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/tests/test_extract.py
--rw-r--r--   0 lanuma     (502) staff       (20)     5024 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/tests/test_helpers.py
--rw-r--r--   0 lanuma     (502) staff       (20)      276 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/tests/test_itags.py
--rw-r--r--   0 lanuma     (502) staff       (20)     1915 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/tests/test_main.py
--rw-r--r--   0 lanuma     (502) staff       (20)      498 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/tests/test_metadata.py
--rw-r--r--   0 lanuma     (502) staff       (20)     1406 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/tests/test_parser.py
--rw-r--r--   0 lanuma     (502) staff       (20)     6148 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/tests/test_query.py
--rw-r--r--   0 lanuma     (502) staff       (20)     1820 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/tests/test_request.py
--rw-r--r--   0 lanuma     (502) staff       (20)    13696 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.1/tests/test_streams.py
+drwxr-xr-x   0 lanuma     (502) staff       (20)        0 2023-07-22 17:13:26.289379 pytube-lanuma-15.2.2/
+-rw-r--r--   0 lanuma     (502) staff       (20)     1211 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/LICENSE
+-rw-r--r--   0 lanuma     (502) staff       (20)       55 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/MANIFEST.in
+-rw-r--r--   0 lanuma     (502) staff       (20)     5315 2023-07-22 17:13:26.289252 pytube-lanuma-15.2.2/PKG-INFO
+-rw-r--r--   0 lanuma     (502) staff       (20)     4057 2023-07-22 17:13:11.000000 pytube-lanuma-15.2.2/README.md
+drwxr-xr-x   0 lanuma     (502) staff       (20)        0 2023-07-22 17:13:26.285072 pytube-lanuma-15.2.2/pytube/
+-rw-r--r--   0 lanuma     (502) staff       (20)      592 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/pytube/__init__.py
+-rw-r--r--   0 lanuma     (502) staff       (20)    15423 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/pytube/__main__.py
+-rw-r--r--   0 lanuma     (502) staff       (20)     5648 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/pytube/captions.py
+-rw-r--r--   0 lanuma     (502) staff       (20)    21972 2023-07-22 17:13:11.000000 pytube-lanuma-15.2.2/pytube/cipher.py
+-rwxr-xr-x   0 lanuma     (502) staff       (20)    16641 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/pytube/cli.py
+drwxr-xr-x   0 lanuma     (502) staff       (20)        0 2023-07-22 17:13:26.285542 pytube-lanuma-15.2.2/pytube/contrib/
+-rw-r--r--   0 lanuma     (502) staff       (20)        0 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/pytube/contrib/__init__.py
+-rw-r--r--   0 lanuma     (502) staff       (20)     6576 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/pytube/contrib/channel.py
+-rw-r--r--   0 lanuma     (502) staff       (20)    14204 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/pytube/contrib/playlist.py
+-rw-r--r--   0 lanuma     (502) staff       (20)     8898 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/pytube/contrib/search.py
+-rw-r--r--   0 lanuma     (502) staff       (20)     3907 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/pytube/exceptions.py
+-rw-r--r--   0 lanuma     (502) staff       (20)    17798 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/pytube/extract.py
+-rw-r--r--   0 lanuma     (502) staff       (20)     9794 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/pytube/helpers.py
+-rw-r--r--   0 lanuma     (502) staff       (20)    15775 2023-07-22 17:13:11.000000 pytube-lanuma-15.2.2/pytube/innertube.py
+-rw-r--r--   0 lanuma     (502) staff       (20)     4311 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/pytube/itags.py
+-rw-r--r--   0 lanuma     (502) staff       (20)     1482 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/pytube/metadata.py
+-rw-r--r--   0 lanuma     (502) staff       (20)      451 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/pytube/monostate.py
+-rw-r--r--   0 lanuma     (502) staff       (20)     5931 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/pytube/parser.py
+-rw-r--r--   0 lanuma     (502) staff       (20)    12844 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/pytube/query.py
+-rw-r--r--   0 lanuma     (502) staff       (20)     8662 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/pytube/request.py
+-rw-r--r--   0 lanuma     (502) staff       (20)    15288 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/pytube/streams.py
+-rw-r--r--   0 lanuma     (502) staff       (20)       74 2023-07-22 17:13:19.000000 pytube-lanuma-15.2.2/pytube/version.py
+drwxr-xr-x   0 lanuma     (502) staff       (20)        0 2023-07-22 17:13:26.286295 pytube-lanuma-15.2.2/pytube_lanuma.egg-info/
+-rw-r--r--   0 lanuma     (502) staff       (20)     5315 2023-07-22 17:13:26.000000 pytube-lanuma-15.2.2/pytube_lanuma.egg-info/PKG-INFO
+-rw-r--r--   0 lanuma     (502) staff       (20)     1045 2023-07-22 17:13:26.000000 pytube-lanuma-15.2.2/pytube_lanuma.egg-info/SOURCES.txt
+-rw-r--r--   0 lanuma     (502) staff       (20)        1 2023-07-22 17:13:26.000000 pytube-lanuma-15.2.2/pytube_lanuma.egg-info/dependency_links.txt
+-rw-r--r--   0 lanuma     (502) staff       (20)       50 2023-07-22 17:13:26.000000 pytube-lanuma-15.2.2/pytube_lanuma.egg-info/entry_points.txt
+-rw-r--r--   0 lanuma     (502) staff       (20)        7 2023-07-22 17:13:26.000000 pytube-lanuma-15.2.2/pytube_lanuma.egg-info/top_level.txt
+-rw-r--r--   0 lanuma     (502) staff       (20)        1 2023-07-22 17:13:26.000000 pytube-lanuma-15.2.2/pytube_lanuma.egg-info/zip-safe
+-rw-r--r--   0 lanuma     (502) staff       (20)       38 2023-07-22 17:13:26.289414 pytube-lanuma-15.2.2/setup.cfg
+-rwxr-xr-x   0 lanuma     (502) staff       (20)     2000 2023-07-22 17:13:11.000000 pytube-lanuma-15.2.2/setup.py
+drwxr-xr-x   0 lanuma     (502) staff       (20)        0 2023-07-22 17:13:26.288808 pytube-lanuma-15.2.2/tests/
+-rw-r--r--   0 lanuma     (502) staff       (20)       57 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/tests/__init__.py
+-rw-r--r--   0 lanuma     (502) staff       (20)     4921 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/tests/conftest.py
+drwxr-xr-x   0 lanuma     (502) staff       (20)        0 2023-07-22 17:13:26.289065 pytube-lanuma-15.2.2/tests/contrib/
+-rw-r--r--   0 lanuma     (502) staff       (20)     3122 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/tests/contrib/test_channel.py
+-rw-r--r--   0 lanuma     (502) staff       (20)    11623 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/tests/contrib/test_playlist.py
+-rw-r--r--   0 lanuma     (502) staff       (20)     5759 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/tests/test_captions.py
+-rw-r--r--   0 lanuma     (502) staff       (20)     2736 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/tests/test_cipher.py
+-rw-r--r--   0 lanuma     (502) staff       (20)    17295 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/tests/test_cli.py
+-rw-r--r--   0 lanuma     (502) staff       (20)     3452 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/tests/test_exceptions.py
+-rw-r--r--   0 lanuma     (502) staff       (20)     2957 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/tests/test_extract.py
+-rw-r--r--   0 lanuma     (502) staff       (20)     5024 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/tests/test_helpers.py
+-rw-r--r--   0 lanuma     (502) staff       (20)      276 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/tests/test_itags.py
+-rw-r--r--   0 lanuma     (502) staff       (20)     1915 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/tests/test_main.py
+-rw-r--r--   0 lanuma     (502) staff       (20)      498 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/tests/test_metadata.py
+-rw-r--r--   0 lanuma     (502) staff       (20)     1406 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/tests/test_parser.py
+-rw-r--r--   0 lanuma     (502) staff       (20)     6148 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/tests/test_query.py
+-rw-r--r--   0 lanuma     (502) staff       (20)     1820 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/tests/test_request.py
+-rw-r--r--   0 lanuma     (502) staff       (20)    13696 2023-06-26 08:39:01.000000 pytube-lanuma-15.2.2/tests/test_streams.py
```

### Comparing `pytube-lanuma-15.2.1/LICENSE` & `pytube-lanuma-15.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/PKG-INFO` & `pytube-lanuma-15.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytube-lanuma
-Version: 15.2.1
+Version: 15.2.2
 Summary: Python 3 library for downloading YouTube Videos.
 Home-page: https://github.com/lanuma/pytube-lanuma
 Author: Angga Lanuma
 Author-email: lanuma.angga@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/lanuma/pytube-lanuma/issues
 Project-URL: Read the Docs, https://pytube.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytube-lanuma Version: 15.2.1 Summary: Python 3
+Metadata-Version: 2.1 Name: pytube-lanuma Version: 15.2.2 Summary: Python 3
 library for downloading YouTube Videos. Home-page: https://github.com/lanuma/
 pytube-lanuma Author: Angga Lanuma Author-email: lanuma.angga@gmail.com
 License: MIT Project-URL: Bug Reports, https://github.com/lanuma/pytube-lanuma/
 issues Project-URL: Read the Docs, https://pytube.io Keywords:
 youtube,download,video,stream Classifier: Development Status :: 5 - Production/
 Stable Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
```

### Comparing `pytube-lanuma-15.2.1/README.md` & `pytube-lanuma-15.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/pytube/__init__.py` & `pytube-lanuma-15.2.2/pytube/__init__.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/pytube/__main__.py` & `pytube-lanuma-15.2.2/pytube/__main__.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/pytube/captions.py` & `pytube-lanuma-15.2.2/pytube/captions.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/pytube/cipher.py` & `pytube-lanuma-15.2.2/pytube/cipher.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,23 +194,24 @@
     name = re.escape(get_initial_function_name(js))
     pattern = r"%s=function\(\w\){[a-z=\.\(\"\)]*;(.*);(?:.+)}" % name
     logger.debug("getting transform plan")
     return regex_search(pattern, js, group=1).split(";")
 
 
 def get_transform_object(js: str, var: str) -> List[str]:
+    """Extract the "transform object"""
     pattern = r"var %s={(.*?)};" % re.escape(var)
     logger.debug("getting transform object")
     regex = re.compile(pattern, flags=re.DOTALL)
     transform_match = regex.search(js)
-
     if not transform_match:
-        # i commented out the line raising the error
-        # raise RegexMatchError(caller="get_transform_object", pattern=pattern)
-        return []  # Return an empty list if no match is found
+        # This line raises the RegexMatchError exception
+        #raise RegexMatchError(caller="get_transform_object", pattern=pattern)
+        logger.error(f"No match found for pattern: {pattern}")
+        return []
 
     return transform_match.group(1).replace("\n", " ").split(", ")
 
 
 def get_transform_map(js: str, var: str) -> Dict:
     """Build a transform function lookup.
```

### Comparing `pytube-lanuma-15.2.1/pytube/cli.py` & `pytube-lanuma-15.2.2/pytube/cli.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/pytube/contrib/channel.py` & `pytube-lanuma-15.2.2/pytube/contrib/channel.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/pytube/contrib/playlist.py` & `pytube-lanuma-15.2.2/pytube/contrib/playlist.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/pytube/contrib/search.py` & `pytube-lanuma-15.2.2/pytube/contrib/search.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/pytube/exceptions.py` & `pytube-lanuma-15.2.2/pytube/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/pytube/extract.py` & `pytube-lanuma-15.2.2/pytube/extract.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/pytube/helpers.py` & `pytube-lanuma-15.2.2/pytube/helpers.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/pytube/innertube.py` & `pytube-lanuma-15.2.2/pytube/innertube.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/pytube/itags.py` & `pytube-lanuma-15.2.2/pytube/itags.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/pytube/metadata.py` & `pytube-lanuma-15.2.2/pytube/metadata.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/pytube/parser.py` & `pytube-lanuma-15.2.2/pytube/parser.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/pytube/query.py` & `pytube-lanuma-15.2.2/pytube/query.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/pytube/request.py` & `pytube-lanuma-15.2.2/pytube/request.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/pytube/streams.py` & `pytube-lanuma-15.2.2/pytube/streams.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/pytube_lanuma.egg-info/PKG-INFO` & `pytube-lanuma-15.2.2/pytube_lanuma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytube-lanuma
-Version: 15.2.1
+Version: 15.2.2
 Summary: Python 3 library for downloading YouTube Videos.
 Home-page: https://github.com/lanuma/pytube-lanuma
 Author: Angga Lanuma
 Author-email: lanuma.angga@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/lanuma/pytube-lanuma/issues
 Project-URL: Read the Docs, https://pytube.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytube-lanuma Version: 15.2.1 Summary: Python 3
+Metadata-Version: 2.1 Name: pytube-lanuma Version: 15.2.2 Summary: Python 3
 library for downloading YouTube Videos. Home-page: https://github.com/lanuma/
 pytube-lanuma Author: Angga Lanuma Author-email: lanuma.angga@gmail.com
 License: MIT Project-URL: Bug Reports, https://github.com/lanuma/pytube-lanuma/
 issues Project-URL: Read the Docs, https://pytube.io Keywords:
 youtube,download,video,stream Classifier: Development Status :: 5 - Production/
 Stable Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
```

### Comparing `pytube-lanuma-15.2.1/pytube_lanuma.egg-info/SOURCES.txt` & `pytube-lanuma-15.2.2/pytube_lanuma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/setup.py` & `pytube-lanuma-15.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/tests/conftest.py` & `pytube-lanuma-15.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/tests/contrib/test_channel.py` & `pytube-lanuma-15.2.2/tests/contrib/test_channel.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/tests/contrib/test_playlist.py` & `pytube-lanuma-15.2.2/tests/contrib/test_playlist.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/tests/test_captions.py` & `pytube-lanuma-15.2.2/tests/test_captions.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/tests/test_cipher.py` & `pytube-lanuma-15.2.2/tests/test_cipher.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/tests/test_cli.py` & `pytube-lanuma-15.2.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/tests/test_exceptions.py` & `pytube-lanuma-15.2.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/tests/test_extract.py` & `pytube-lanuma-15.2.2/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/tests/test_helpers.py` & `pytube-lanuma-15.2.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/tests/test_main.py` & `pytube-lanuma-15.2.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/tests/test_parser.py` & `pytube-lanuma-15.2.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/tests/test_query.py` & `pytube-lanuma-15.2.2/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/tests/test_request.py` & `pytube-lanuma-15.2.2/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `pytube-lanuma-15.2.1/tests/test_streams.py` & `pytube-lanuma-15.2.2/tests/test_streams.py`

 * *Files identical despite different names*

