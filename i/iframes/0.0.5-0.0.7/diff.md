# Comparing `tmp/iframes-0.0.5.tar.gz` & `tmp/iframes-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iframes-0.0.5.tar", last modified: Sat Sep 17 02:58:52 2022, max compression
+gzip compressed data, was "iframes-0.0.7.tar", last modified: Sat Jul 22 09:27:54 2023, max compression
```

## Comparing `iframes-0.0.5.tar` & `iframes-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2022-09-17 02:58:52.696230 iframes-0.0.5/
--rw-r--r--   0 a         (1000) a         (1000)     1405 2022-09-17 02:58:52.696230 iframes-0.0.5/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      825 2022-09-17 02:55:22.000000 iframes-0.0.5/README.md
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2022-09-17 02:58:52.692230 iframes-0.0.5/bin/
--rw-r--r--   0 a         (1000) a         (1000)       55 2022-08-17 15:34:17.000000 iframes-0.0.5/bin/iframes
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2022-09-17 02:58:52.692230 iframes-0.0.5/iframes.egg-info/
--rw-r--r--   0 a         (1000) a         (1000)     1405 2022-09-17 02:58:52.000000 iframes-0.0.5/iframes.egg-info/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      195 2022-09-17 02:58:52.000000 iframes-0.0.5/iframes.egg-info/SOURCES.txt
--rw-r--r--   0 a         (1000) a         (1000)        1 2022-09-17 02:58:52.000000 iframes-0.0.5/iframes.egg-info/dependency_links.txt
--rw-r--r--   0 a         (1000) a         (1000)       11 2022-09-17 02:58:52.000000 iframes-0.0.5/iframes.egg-info/requires.txt
--rw-r--r--   0 a         (1000) a         (1000)        8 2022-09-17 02:58:52.000000 iframes-0.0.5/iframes.egg-info/top_level.txt
--rw-r--r--   0 a         (1000) a         (1000)     2984 2022-09-17 02:57:59.000000 iframes-0.0.5/iframes.py
--rw-r--r--   0 a         (1000) a         (1000)       38 2022-09-17 02:58:52.696230 iframes-0.0.5/setup.cfg
--rw-r--r--   0 a         (1000) a         (1000)      901 2022-09-17 02:57:59.000000 iframes-0.0.5/setup.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-07-22 09:27:54.217270 iframes-0.0.7/
+-rw-r--r--   0 a         (1000) a         (1000)     1813 2023-07-22 09:27:54.217270 iframes-0.0.7/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)     1252 2023-07-22 09:27:34.000000 iframes-0.0.7/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-07-22 09:27:54.217270 iframes-0.0.7/bin/
+-rw-r--r--   0 a         (1000) a         (1000)       55 2023-07-22 08:32:14.000000 iframes-0.0.7/bin/iframes
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-07-22 09:27:54.217270 iframes-0.0.7/iframes.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)     1813 2023-07-22 09:27:54.000000 iframes-0.0.7/iframes.egg-info/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      195 2023-07-22 09:27:54.000000 iframes-0.0.7/iframes.egg-info/SOURCES.txt
+-rw-r--r--   0 a         (1000) a         (1000)        1 2023-07-22 09:27:54.000000 iframes-0.0.7/iframes.egg-info/dependency_links.txt
+-rw-r--r--   0 a         (1000) a         (1000)       11 2023-07-22 09:27:54.000000 iframes-0.0.7/iframes.egg-info/requires.txt
+-rw-r--r--   0 a         (1000) a         (1000)        8 2023-07-22 09:27:54.000000 iframes-0.0.7/iframes.egg-info/top_level.txt
+-rw-r--r--   0 a         (1000) a         (1000)     3540 2023-07-22 09:27:34.000000 iframes-0.0.7/iframes.py
+-rw-r--r--   0 a         (1000) a         (1000)       38 2023-07-22 09:27:54.217270 iframes-0.0.7/setup.cfg
+-rw-r--r--   0 a         (1000) a         (1000)      901 2023-07-22 08:32:14.000000 iframes-0.0.7/setup.py
```

### Comparing `iframes-0.0.5/PKG-INFO` & `iframes-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: iframes
-Version: 0.0.5
+Version: 0.0.7
 Summary: Fast detection of iframes in mpegts streams
 Home-page: https://github.com/futzu/iframes
 Author: Adrian
 Author-email: spam@iodisco.com
-License: UNKNOWN
 Platform: all
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
@@ -22,23 +21,34 @@
 * pip install iframes
 ```smalltalk
 python3 -mpip install iframes
 ```
 
 ## Run 
 * local file
+```js
+first video.ts
 ```
+
+```js
 iframes video.ts
 ```
 * https
+```rebol
+first https://example.com/video.ts
 ```
+
+```rebol
 iframes https://example.com/video.ts
 ```
 * multicast
+```rebol
+first udp://@227.5.5.5:1234
 ```
+```rebol
 iframes udp://@227.5.5.5:1234
 ```
 ## Output
 * iframe pts
 ```smalltalk
 14648.092267
 14648.342511
@@ -77,9 +87,20 @@
 14656.317144
 14656.433933
 14656.684178
 14656.934433
 14657.184678
 14657.434933
 ```
+### programmatically 
 
+```py3
+from iframes import IFramer
+ifrmr = IFramer()
+first_frame = ifrmr.first('a_video.ts')
+```
 
+```py3
+from iframes import IFramer
+ifrmr = IFramer(shush=True)  # set IFramer.shush=True to suppress printing pts 
+all_iframes = ifrmr.do('https://example.com/coolvideo.ts')
+```
```

### Comparing `iframes-0.0.5/iframes.egg-info/PKG-INFO` & `iframes-0.0.7/iframes.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: iframes
-Version: 0.0.5
+Version: 0.0.7
 Summary: Fast detection of iframes in mpegts streams
 Home-page: https://github.com/futzu/iframes
 Author: Adrian
 Author-email: spam@iodisco.com
-License: UNKNOWN
 Platform: all
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
@@ -22,23 +21,34 @@
 * pip install iframes
 ```smalltalk
 python3 -mpip install iframes
 ```
 
 ## Run 
 * local file
+```js
+first video.ts
 ```
+
+```js
 iframes video.ts
 ```
 * https
+```rebol
+first https://example.com/video.ts
 ```
+
+```rebol
 iframes https://example.com/video.ts
 ```
 * multicast
+```rebol
+first udp://@227.5.5.5:1234
 ```
+```rebol
 iframes udp://@227.5.5.5:1234
 ```
 ## Output
 * iframe pts
 ```smalltalk
 14648.092267
 14648.342511
@@ -77,9 +87,20 @@
 14656.317144
 14656.433933
 14656.684178
 14656.934433
 14657.184678
 14657.434933
 ```
+### programmatically 
 
+```py3
+from iframes import IFramer
+ifrmr = IFramer()
+first_frame = ifrmr.first('a_video.ts')
+```
 
+```py3
+from iframes import IFramer
+ifrmr = IFramer(shush=True)  # set IFramer.shush=True to suppress printing pts 
+all_iframes = ifrmr.do('https://example.com/coolvideo.ts')
+```
```

### Comparing `iframes-0.0.5/setup.py` & `iframes-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/futzu/iframes",
     install_requires=[
         "new_reader",
     ],
     py_modules=["iframes"],
-    scripts=["bin/iframes"],
+    scripts=['bin/iframes'],
     platforms="all",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Programming Language :: Python :: Implementation :: CPython",
```

