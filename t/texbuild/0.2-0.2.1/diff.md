# Comparing `tmp/texbuild-0.2.tar.gz` & `tmp/texbuild-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texbuild-0.2.tar", last modified: Sat Jul 22 04:56:39 2023, max compression
+gzip compressed data, was "texbuild-0.2.1.tar", last modified: Sat Jul 22 05:00:16 2023, max compression
```

## Comparing `texbuild-0.2.tar` & `texbuild-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 danielsank (268076) primarygroup (89939)        0 2023-07-22 04:56:39.513709 texbuild-0.2/
--rw-r--r--   0 danielsank (268076) primarygroup (89939)     1075 2022-07-29 23:37:42.000000 texbuild-0.2/LICENSE
--rw-r--r--   0 danielsank (268076) primarygroup (89939)     3242 2023-07-22 04:56:39.513709 texbuild-0.2/PKG-INFO
--rw-r--r--   0 danielsank (268076) primarygroup (89939)     1464 2022-07-29 23:50:12.000000 texbuild-0.2/README.md
--rw-r--r--   0 danielsank (268076) primarygroup (89939)      730 2023-07-22 04:55:43.000000 texbuild-0.2/pyproject.toml
--rw-r--r--   0 danielsank (268076) primarygroup (89939)       38 2023-07-22 04:56:39.513709 texbuild-0.2/setup.cfg
-drwxr-xr-x   0 danielsank (268076) primarygroup (89939)        0 2023-07-22 04:56:39.509709 texbuild-0.2/src/
-drwxr-xr-x   0 danielsank (268076) primarygroup (89939)        0 2023-07-22 04:56:39.513709 texbuild-0.2/src/texbuild/
--rw-r--r--   0 danielsank (268076) primarygroup (89939)        0 2022-07-29 23:37:42.000000 texbuild-0.2/src/texbuild/__init__.py
--rwxr-xr-x   0 danielsank (268076) primarygroup (89939)     9106 2023-07-22 04:44:52.000000 texbuild-0.2/src/texbuild/build.py
-drwxr-xr-x   0 danielsank (268076) primarygroup (89939)        0 2023-07-22 04:56:39.513709 texbuild-0.2/src/texbuild.egg-info/
--rw-r--r--   0 danielsank (268076) primarygroup (89939)     3242 2023-07-22 04:56:39.000000 texbuild-0.2/src/texbuild.egg-info/PKG-INFO
--rw-r--r--   0 danielsank (268076) primarygroup (89939)      307 2023-07-22 04:56:39.000000 texbuild-0.2/src/texbuild.egg-info/SOURCES.txt
--rw-r--r--   0 danielsank (268076) primarygroup (89939)        1 2023-07-22 04:56:39.000000 texbuild-0.2/src/texbuild.egg-info/dependency_links.txt
--rw-r--r--   0 danielsank (268076) primarygroup (89939)       49 2023-07-22 04:56:39.000000 texbuild-0.2/src/texbuild.egg-info/entry_points.txt
--rw-r--r--   0 danielsank (268076) primarygroup (89939)       12 2023-07-22 04:56:39.000000 texbuild-0.2/src/texbuild.egg-info/requires.txt
--rw-r--r--   0 danielsank (268076) primarygroup (89939)        9 2023-07-22 04:56:39.000000 texbuild-0.2/src/texbuild.egg-info/top_level.txt
+drwxr-xr-x   0 danielsank (268076) primarygroup (89939)        0 2023-07-22 05:00:16.783143 texbuild-0.2.1/
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)     1075 2022-07-29 23:37:42.000000 texbuild-0.2.1/LICENSE
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)     3251 2023-07-22 05:00:16.783143 texbuild-0.2.1/PKG-INFO
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)     1471 2023-07-22 04:59:29.000000 texbuild-0.2.1/README.md
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)      732 2023-07-22 04:59:43.000000 texbuild-0.2.1/pyproject.toml
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)       38 2023-07-22 05:00:16.783143 texbuild-0.2.1/setup.cfg
+drwxr-xr-x   0 danielsank (268076) primarygroup (89939)        0 2023-07-22 05:00:16.779143 texbuild-0.2.1/src/
+drwxr-xr-x   0 danielsank (268076) primarygroup (89939)        0 2023-07-22 05:00:16.779143 texbuild-0.2.1/src/texbuild/
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)        0 2022-07-29 23:37:42.000000 texbuild-0.2.1/src/texbuild/__init__.py
+-rwxr-xr-x   0 danielsank (268076) primarygroup (89939)     9106 2023-07-22 04:44:52.000000 texbuild-0.2.1/src/texbuild/build.py
+drwxr-xr-x   0 danielsank (268076) primarygroup (89939)        0 2023-07-22 05:00:16.783143 texbuild-0.2.1/src/texbuild.egg-info/
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)     3251 2023-07-22 05:00:16.000000 texbuild-0.2.1/src/texbuild.egg-info/PKG-INFO
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)      307 2023-07-22 05:00:16.000000 texbuild-0.2.1/src/texbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)        1 2023-07-22 05:00:16.000000 texbuild-0.2.1/src/texbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)       49 2023-07-22 05:00:16.000000 texbuild-0.2.1/src/texbuild.egg-info/entry_points.txt
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)       12 2023-07-22 05:00:16.000000 texbuild-0.2.1/src/texbuild.egg-info/requires.txt
+-rw-r--r--   0 danielsank (268076) primarygroup (89939)        9 2023-07-22 05:00:16.000000 texbuild-0.2.1/src/texbuild.egg-info/top_level.txt
```

### Comparing `texbuild-0.2/LICENSE` & `texbuild-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `texbuild-0.2/PKG-INFO` & `texbuild-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texbuild
-Version: 0.2
+Version: 0.2.1
 Summary: Build system for LaTeX documents.
 Author-email: Daniel Sank <sank.daniel@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Daniel Thomas Sank
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -94,8 +94,8 @@
 To see `texbuild` in action, install it and use it to build the example LaTeX documemt provided in this repo, by following these steps:
 ```
 $ pip install texbuild
 $ git clone https://github.com/DanielSank/texbuild
 $ cd texbuild/example
 $ texbuild
 
-This produces `texbuild/example/build/main.pdf`, which illustrates the use of `texbuild`.
+This produces `texbuild/example/texbuild-out/main.pdf`, which illustrates the use of `texbuild`.
```

### Comparing `texbuild-0.2/README.md` & `texbuild-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,8 +57,8 @@
 To see `texbuild` in action, install it and use it to build the example LaTeX documemt provided in this repo, by following these steps:
 ```
 $ pip install texbuild
 $ git clone https://github.com/DanielSank/texbuild
 $ cd texbuild/example
 $ texbuild
 
-This produces `texbuild/example/build/main.pdf`, which illustrates the use of `texbuild`.
+This produces `texbuild/example/texbuild-out/main.pdf`, which illustrates the use of `texbuild`.
```

### Comparing `texbuild-0.2/pyproject.toml` & `texbuild-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "texbuild"
-version = "0.2"
+version = "0.2.1"
 authors = [
   { name="Daniel Sank", email="sank.daniel@gmail.com" },
 ]
 description = "Build system for LaTeX documents."
 keywords = ["latex"]
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `texbuild-0.2/src/texbuild/build.py` & `texbuild-0.2.1/src/texbuild/build.py`

 * *Files identical despite different names*

### Comparing `texbuild-0.2/src/texbuild.egg-info/PKG-INFO` & `texbuild-0.2.1/src/texbuild.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texbuild
-Version: 0.2
+Version: 0.2.1
 Summary: Build system for LaTeX documents.
 Author-email: Daniel Sank <sank.daniel@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Daniel Thomas Sank
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -94,8 +94,8 @@
 To see `texbuild` in action, install it and use it to build the example LaTeX documemt provided in this repo, by following these steps:
 ```
 $ pip install texbuild
 $ git clone https://github.com/DanielSank/texbuild
 $ cd texbuild/example
 $ texbuild
 
-This produces `texbuild/example/build/main.pdf`, which illustrates the use of `texbuild`.
+This produces `texbuild/example/texbuild-out/main.pdf`, which illustrates the use of `texbuild`.
```

