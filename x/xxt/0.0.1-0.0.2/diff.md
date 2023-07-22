# Comparing `tmp/xxt-0.0.1.tar.gz` & `tmp/xxt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xxt-0.0.1.tar", last modified: Mon Jul 17 09:54:32 2023, max compression
+gzip compressed data, was "xxt-0.0.2.tar", last modified: Sat Jul 22 08:27:30 2023, max compression
```

## Comparing `xxt-0.0.1.tar` & `xxt-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 09:54:32.401342 xxt-0.0.1/
--rw-rw-rw-   0        0        0     1122 2023-07-17 09:54:32.401342 xxt-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-07-17 09:54:17.000000 xxt-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 09:54:32.401342 xxt-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1040 2023-07-17 09:53:24.000000 xxt-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:54:32.370093 xxt-0.0.1/xxt/
--rw-rw-rw-   0        0        0       23 2023-07-17 09:53:32.000000 xxt-0.0.1/xxt/__init__.py
--rw-rw-rw-   0        0        0     5133 2023-07-17 09:13:59.000000 xxt-0.0.1/xxt/funcs.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:54:32.385718 xxt-0.0.1/xxt.egg-info/
--rw-rw-rw-   0        0        0     1122 2023-07-17 09:54:32.000000 xxt-0.0.1/xxt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      181 2023-07-17 09:54:32.000000 xxt-0.0.1/xxt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 09:54:32.000000 xxt-0.0.1/xxt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 09:54:32.000000 xxt-0.0.1/xxt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-17 09:54:32.000000 xxt-0.0.1/xxt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 08:27:30.301180 xxt-0.0.2/
+-rw-rw-rw-   0        0        0     2092 2023-07-22 08:27:30.301180 xxt-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1568 2023-07-17 13:09:27.000000 xxt-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-22 08:27:30.301180 xxt-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1040 2023-07-17 12:01:43.000000 xxt-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:27:30.254301 xxt-0.0.2/xxt/
+-rw-rw-rw-   0        0        0       23 2023-07-17 09:53:32.000000 xxt-0.0.2/xxt/__init__.py
+-rw-rw-rw-   0        0        0     5133 2023-07-17 09:13:59.000000 xxt-0.0.2/xxt/funcs.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:27:30.301180 xxt-0.0.2/xxt.egg-info/
+-rw-rw-rw-   0        0        0     2092 2023-07-22 08:27:30.000000 xxt-0.0.2/xxt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2023-07-22 08:27:30.000000 xxt-0.0.2/xxt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 08:27:30.000000 xxt-0.0.2/xxt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-22 08:27:30.000000 xxt-0.0.2/xxt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-22 08:27:30.000000 xxt-0.0.2/xxt.egg-info/top_level.txt
```

### Comparing `xxt-0.0.1/setup.py` & `xxt-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="xxt",
-    version="0.0.1",
+    version="0.0.2",
     description="Library with many uses",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Xi Teo",
     author_email="diamondraft1575@gmail.com",
     license="MIT",
```

### Comparing `xxt-0.0.1/xxt/funcs.py` & `xxt-0.0.2/xxt/funcs.py`

 * *Files identical despite different names*

