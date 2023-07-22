# Comparing `tmp/allocine-seances-0.0.5.tar.gz` & `tmp/allocine-seances-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allocine-seances-0.0.5.tar", last modified: Wed Apr 19 17:52:44 2023, max compression
+gzip compressed data, was "allocine-seances-0.0.6.tar", last modified: Sat Jul 22 12:55:18 2023, max compression
```

## Comparing `allocine-seances-0.0.5.tar` & `allocine-seances-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 17:52:44.250181 allocine-seances-0.0.5/
--rw-rw-rw-   0        0        0     1088 2023-04-15 16:16:47.000000 allocine-seances-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     4607 2023-04-19 17:52:44.250181 allocine-seances-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2779 2023-04-15 18:32:35.000000 allocine-seances-0.0.5/README.md
--rw-rw-rw-   0        0        0      721 2023-04-19 17:52:30.000000 allocine-seances-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 17:52:44.250181 allocine-seances-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-19 17:52:44.220332 allocine-seances-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 17:52:44.230599 allocine-seances-0.0.5/src/allocineAPI/
--rw-rw-rw-   0        0        0        0 2023-04-15 16:02:27.000000 allocine-seances-0.0.5/src/allocineAPI/__init__.py
--rw-rw-rw-   0        0        0     6515 2023-04-19 17:48:48.000000 allocine-seances-0.0.5/src/allocineAPI/allocineAPI.py
-drwxrwxrwx   0        0        0        0 2023-04-19 17:52:44.250181 allocine-seances-0.0.5/src/allocine_seances.egg-info/
--rw-rw-rw-   0        0        0     4607 2023-04-19 17:52:44.000000 allocine-seances-0.0.5/src/allocine_seances.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-04-19 17:52:44.000000 allocine-seances-0.0.5/src/allocine_seances.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 17:52:44.000000 allocine-seances-0.0.5/src/allocine_seances.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-19 17:52:44.000000 allocine-seances-0.0.5/src/allocine_seances.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-19 17:52:44.000000 allocine-seances-0.0.5/src/allocine_seances.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 12:55:18.817734 allocine-seances-0.0.6/
+-rw-rw-rw-   0        0        0     1088 2023-04-15 16:16:47.000000 allocine-seances-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     4607 2023-07-22 12:55:18.815214 allocine-seances-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2779 2023-04-15 18:32:35.000000 allocine-seances-0.0.6/README.md
+-rw-rw-rw-   0        0        0      721 2023-07-22 12:55:01.000000 allocine-seances-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-22 12:55:18.818737 allocine-seances-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-22 12:55:18.783983 allocine-seances-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-22 12:55:18.790511 allocine-seances-0.0.6/src/allocineAPI/
+-rw-rw-rw-   0        0        0        0 2023-04-15 16:02:27.000000 allocine-seances-0.0.6/src/allocineAPI/__init__.py
+-rw-rw-rw-   0        0        0     9755 2023-07-22 12:52:52.000000 allocine-seances-0.0.6/src/allocineAPI/allocineAPI.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:55:18.813210 allocine-seances-0.0.6/src/allocine_seances.egg-info/
+-rw-rw-rw-   0        0        0     4607 2023-07-22 12:55:18.000000 allocine-seances-0.0.6/src/allocine_seances.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-07-22 12:55:18.000000 allocine-seances-0.0.6/src/allocine_seances.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 12:55:18.000000 allocine-seances-0.0.6/src/allocine_seances.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-22 12:55:18.000000 allocine-seances-0.0.6/src/allocine_seances.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-22 12:55:18.000000 allocine-seances-0.0.6/src/allocine_seances.egg-info/top_level.txt
```

### Comparing `allocine-seances-0.0.5/LICENSE` & `allocine-seances-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `allocine-seances-0.0.5/PKG-INFO` & `allocine-seances-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allocine-seances
-Version: 0.0.5
+Version: 0.0.6
 Summary: Récupération des scéances de cinémas sur allociné
 Author-email: lefevre-dev <louislefevre.dev@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `allocine-seances-0.0.5/README.md` & `allocine-seances-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `allocine-seances-0.0.5/pyproject.toml` & `allocine-seances-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "allocine-seances"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="lefevre-dev", email="louislefevre.dev@gmail.com" },
 ]
 description = "Récupération des scéances de cinémas sur allociné"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
```

### Comparing `allocine-seances-0.0.5/src/allocine_seances.egg-info/PKG-INFO` & `allocine-seances-0.0.6/src/allocine_seances.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allocine-seances
-Version: 0.0.5
+Version: 0.0.6
 Summary: Récupération des scéances de cinémas sur allociné
 Author-email: lefevre-dev <louislefevre.dev@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

