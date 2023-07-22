# Comparing `tmp/playcode-0.0.2.tar.gz` & `tmp/playcode-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playcode-0.0.2.tar", last modified: Sat Jan 21 12:13:15 2023, max compression
+gzip compressed data, was "playcode-0.0.4.tar", last modified: Sat Jul 22 02:36:44 2023, max compression
```

## Comparing `playcode-0.0.2.tar` & `playcode-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-01-21 12:13:15.608686 playcode-0.0.2/
--rw-rw-rw-   0        0        0      410 2023-01-21 12:13:15.607679 playcode-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-01-21 11:52:00.000000 playcode-0.0.2/README
-drwxrwxrwx   0        0        0        0 2023-01-21 12:13:15.581928 playcode-0.0.2/playcode/
--rw-rw-rw-   0        0        0        0 2023-01-21 10:55:46.000000 playcode-0.0.2/playcode/__init__.py
--rw-rw-rw-   0        0        0      404 2023-01-21 12:10:02.000000 playcode-0.0.2/playcode/password_make.py
--rw-rw-rw-   0        0        0       85 2023-01-21 12:07:02.000000 playcode-0.0.2/playcode/test.py
-drwxrwxrwx   0        0        0        0 2023-01-21 12:13:15.603905 playcode-0.0.2/playcode.egg-info/
--rw-rw-rw-   0        0        0      410 2023-01-21 12:13:14.000000 playcode-0.0.2/playcode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-01-21 12:13:15.000000 playcode-0.0.2/playcode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-21 12:13:14.000000 playcode-0.0.2/playcode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-01-21 12:13:14.000000 playcode-0.0.2/playcode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-21 12:13:15.609684 playcode-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      677 2023-01-21 12:10:02.000000 playcode-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 02:36:44.816451 playcode-0.0.4/
+-rw-rw-rw-   0        0        0      410 2023-07-22 02:36:44.815517 playcode-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-01-21 11:52:00.000000 playcode-0.0.4/README
+drwxrwxrwx   0        0        0        0 2023-07-22 02:36:44.800577 playcode-0.0.4/playcode/
+-rw-rw-rw-   0        0        0        0 2023-01-21 10:55:46.000000 playcode-0.0.4/playcode/__init__.py
+-rw-rw-rw-   0        0        0       85 2023-01-21 12:07:02.000000 playcode-0.0.4/playcode/test.py
+drwxrwxrwx   0        0        0        0 2023-07-22 02:36:44.812614 playcode-0.0.4/playcode.egg-info/
+-rw-rw-rw-   0        0        0      410 2023-07-22 02:36:44.000000 playcode-0.0.4/playcode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2023-07-22 02:36:44.000000 playcode-0.0.4/playcode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 02:36:44.000000 playcode-0.0.4/playcode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-22 02:36:44.000000 playcode-0.0.4/playcode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-22 02:36:44.816451 playcode-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      677 2023-07-22 02:27:44.000000 playcode-0.0.4/setup.py
```

### Comparing `playcode-0.0.2/setup.py` & `playcode-0.0.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="playcode", # Replace with your own PyPI username(id)
-    version="0.0.2",
+    version="0.0.4",
     author="Seungjun Min",
     author_email="sjmin213@gmail.com",
     description="Creating password",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sjmin/",
     packages=setuptools.find_packages(),
```

