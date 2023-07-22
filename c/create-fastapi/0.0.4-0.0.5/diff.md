# Comparing `tmp/create-fastapi-0.0.4.tar.gz` & `tmp/create-fastapi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create-fastapi-0.0.4.tar", last modified: Fri Jul 21 16:06:50 2023, max compression
+gzip compressed data, was "create-fastapi-0.0.5.tar", last modified: Sat Jul 22 08:58:33 2023, max compression
```

## Comparing `create-fastapi-0.0.4.tar` & `create-fastapi-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 16:06:50.081465 create-fastapi-0.0.4/
--rw-rw-rw-   0        0        0    11558 2023-07-21 09:43:38.000000 create-fastapi-0.0.4/LICENSE
--rw-rw-rw-   0        0        0    14130 2023-07-21 16:06:50.073634 create-fastapi-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       20 2023-07-21 09:43:38.000000 create-fastapi-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 16:06:50.073634 create-fastapi-0.0.4/create_fastapi.egg-info/
--rw-rw-rw-   0        0        0    14130 2023-07-21 16:06:50.000000 create-fastapi-0.0.4/create_fastapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-07-21 16:06:50.000000 create-fastapi-0.0.4/create_fastapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 16:06:50.000000 create-fastapi-0.0.4/create_fastapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-21 16:06:50.000000 create-fastapi-0.0.4/create_fastapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-07-21 16:06:50.000000 create-fastapi-0.0.4/create_fastapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 16:06:50.000000 create-fastapi-0.0.4/create_fastapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1184 2023-07-21 16:06:35.000000 create-fastapi-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-21 16:06:50.081465 create-fastapi-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-22 08:58:33.267278 create-fastapi-0.0.5/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 09:43:38.000000 create-fastapi-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0    14130 2023-07-22 08:58:33.266711 create-fastapi-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2023-07-21 09:43:38.000000 create-fastapi-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 08:58:33.263945 create-fastapi-0.0.5/create_fastapi.egg-info/
+-rw-rw-rw-   0        0        0    14130 2023-07-22 08:58:33.000000 create-fastapi-0.0.5/create_fastapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-07-22 08:58:33.000000 create-fastapi-0.0.5/create_fastapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 08:58:33.000000 create-fastapi-0.0.5/create_fastapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-22 08:58:33.000000 create-fastapi-0.0.5/create_fastapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-07-22 08:58:33.000000 create-fastapi-0.0.5/create_fastapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 08:58:33.000000 create-fastapi-0.0.5/create_fastapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1197 2023-07-22 08:58:09.000000 create-fastapi-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-22 08:58:33.267278 create-fastapi-0.0.5/setup.cfg
```

### Comparing `create-fastapi-0.0.4/LICENSE` & `create-fastapi-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `create-fastapi-0.0.4/PKG-INFO` & `create-fastapi-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: create-fastapi
-Version: 0.0.4
+Version: 0.0.5
 Summary: create-fastapi-app
 Author-email: Shahar Luftig <shaharluftig@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `create-fastapi-0.0.4/create_fastapi.egg-info/PKG-INFO` & `create-fastapi-0.0.5/create_fastapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: create-fastapi
-Version: 0.0.4
+Version: 0.0.5
 Summary: create-fastapi-app
 Author-email: Shahar Luftig <shaharluftig@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `create-fastapi-0.0.4/pyproject.toml` & `create-fastapi-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "create-fastapi"
 description = "create-fastapi-app"
 readme = "README.md"
-version = "0.0.4"
+version = "0.0.5"
 
 authors = [{ name = "Shahar Luftig", email = "shaharluftig@gmail.com" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 
 keywords = [
     "backend",
@@ -36,8 +36,8 @@
 
 dependencies = ["typer~=0.9.0", "virtualenv~=20.24.1", "GitPython~=3.1.32"]
 
 [project.urls]
 "Homepage" = "https://github.com/shaharluftig/create-fastapi-app"
 
 [project.scripts]
-app = "cli:main_cli"
+create-fastapi-app = "cli:main_cli"
```

