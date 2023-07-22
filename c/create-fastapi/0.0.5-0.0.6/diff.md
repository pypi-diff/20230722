# Comparing `tmp/create-fastapi-0.0.5.tar.gz` & `tmp/create-fastapi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create-fastapi-0.0.5.tar", last modified: Sat Jul 22 08:58:33 2023, max compression
+gzip compressed data, was "create-fastapi-0.0.6.tar", last modified: Sat Jul 22 09:05:54 2023, max compression
```

## Comparing `create-fastapi-0.0.5.tar` & `create-fastapi-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 08:58:33.267278 create-fastapi-0.0.5/
--rw-rw-rw-   0        0        0    11558 2023-07-21 09:43:38.000000 create-fastapi-0.0.5/LICENSE
--rw-rw-rw-   0        0        0    14130 2023-07-22 08:58:33.266711 create-fastapi-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       20 2023-07-21 09:43:38.000000 create-fastapi-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 08:58:33.263945 create-fastapi-0.0.5/create_fastapi.egg-info/
--rw-rw-rw-   0        0        0    14130 2023-07-22 08:58:33.000000 create-fastapi-0.0.5/create_fastapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-07-22 08:58:33.000000 create-fastapi-0.0.5/create_fastapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 08:58:33.000000 create-fastapi-0.0.5/create_fastapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-22 08:58:33.000000 create-fastapi-0.0.5/create_fastapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-07-22 08:58:33.000000 create-fastapi-0.0.5/create_fastapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 08:58:33.000000 create-fastapi-0.0.5/create_fastapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1197 2023-07-22 08:58:09.000000 create-fastapi-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-22 08:58:33.267278 create-fastapi-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-22 09:05:54.267906 create-fastapi-0.0.6/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 09:43:38.000000 create-fastapi-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0    14130 2023-07-22 09:05:54.267906 create-fastapi-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2023-07-21 09:43:38.000000 create-fastapi-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 09:05:54.235738 create-fastapi-0.0.6/cfa/
+-rw-rw-rw-   0        0        0        0 2023-07-21 13:10:51.000000 create-fastapi-0.0.6/cfa/__init__.py
+-rw-rw-rw-   0        0        0      401 2023-07-21 16:06:12.000000 create-fastapi-0.0.6/cfa/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:05:54.235738 create-fastapi-0.0.6/cfa/commands/
+-rw-rw-rw-   0        0        0       93 2023-07-21 09:53:03.000000 create-fastapi-0.0.6/cfa/commands/ICommand.py
+-rw-rw-rw-   0        0        0        0 2023-07-21 09:43:42.000000 create-fastapi-0.0.6/cfa/commands/__init__.py
+-rw-rw-rw-   0        0        0      873 2023-07-21 12:21:25.000000 create-fastapi-0.0.6/cfa/commands/command_builder.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:05:54.251839 create-fastapi-0.0.6/cfa/commands/impl/
+-rw-rw-rw-   0        0        0        0 2023-07-21 11:40:39.000000 create-fastapi-0.0.6/cfa/commands/impl/__init__.py
+-rw-rw-rw-   0        0        0      548 2023-07-21 12:24:21.000000 create-fastapi-0.0.6/cfa/commands/impl/clone_git.py
+-rw-rw-rw-   0        0        0     1067 2023-07-21 12:55:39.000000 create-fastapi-0.0.6/cfa/commands/impl/dependency_installer.py
+-rw-rw-rw-   0        0        0      314 2023-07-21 11:42:31.000000 create-fastapi-0.0.6/cfa/commands/impl/dir_creator.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:05:54.251839 create-fastapi-0.0.6/cfa/config/
+-rw-rw-rw-   0        0        0      341 2023-07-21 13:01:48.000000 create-fastapi-0.0.6/cfa/config/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:05:54.251839 create-fastapi-0.0.6/cfa/helpers/
+-rw-rw-rw-   0        0        0        0 2023-07-21 11:36:51.000000 create-fastapi-0.0.6/cfa/helpers/__init__.py
+-rw-rw-rw-   0        0        0      279 2023-07-21 11:38:30.000000 create-fastapi-0.0.6/cfa/helpers/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:05:54.235738 create-fastapi-0.0.6/cfa/venv/
+drwxrwxrwx   0        0        0        0 2023-07-22 09:05:54.267906 create-fastapi-0.0.6/cfa/venv/Scripts/
+-rw-rw-rw-   0        0        0     1169 2023-07-21 09:44:48.000000 create-fastapi-0.0.6/cfa/venv/Scripts/activate_this.py
+-rw-rw-rw-   0        0        0      696 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2html.py
+-rw-rw-rw-   0        0        0      818 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2html4.py
+-rw-rw-rw-   0        0        0     1153 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2html5.py
+-rw-rw-rw-   0        0        0      895 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2latex.py
+-rw-rw-rw-   0        0        0      718 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2man.py
+-rw-rw-rw-   0        0        0      884 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2odt.py
+-rw-rw-rw-   0        0        0      690 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2odt_prepstyles.py
+-rw-rw-rw-   0        0        0      703 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2pseudoxml.py
+-rw-rw-rw-   0        0        0      739 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2s5.py
+-rw-rw-rw-   0        0        0      975 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2xetex.py
+-rw-rw-rw-   0        0        0      704 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2xml.py
+-rw-rw-rw-   0        0        0      772 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rstpep2html.py
+drwxrwxrwx   0        0        0        0 2023-07-22 09:05:54.267906 create-fastapi-0.0.6/create_fastapi.egg-info/
+-rw-rw-rw-   0        0        0    14130 2023-07-22 09:05:54.000000 create-fastapi-0.0.6/create_fastapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      975 2023-07-22 09:05:54.000000 create-fastapi-0.0.6/create_fastapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 09:05:54.000000 create-fastapi-0.0.6/create_fastapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-22 09:05:54.000000 create-fastapi-0.0.6/create_fastapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-07-22 09:05:54.000000 create-fastapi-0.0.6/create_fastapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-22 09:05:54.000000 create-fastapi-0.0.6/create_fastapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1201 2023-07-22 09:05:37.000000 create-fastapi-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-22 09:05:54.267906 create-fastapi-0.0.6/setup.cfg
```

### Comparing `create-fastapi-0.0.5/LICENSE` & `create-fastapi-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `create-fastapi-0.0.5/PKG-INFO` & `create-fastapi-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: create-fastapi
-Version: 0.0.5
+Version: 0.0.6
 Summary: create-fastapi-app
 Author-email: Shahar Luftig <shaharluftig@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `create-fastapi-0.0.5/create_fastapi.egg-info/PKG-INFO` & `create-fastapi-0.0.6/create_fastapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: create-fastapi
-Version: 0.0.5
+Version: 0.0.6
 Summary: create-fastapi-app
 Author-email: Shahar Luftig <shaharluftig@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `create-fastapi-0.0.5/pyproject.toml` & `create-fastapi-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "create-fastapi"
 description = "create-fastapi-app"
 readme = "README.md"
-version = "0.0.5"
+version = "0.0.6"
 
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
-create-fastapi-app = "cli:main_cli"
+create-fastapi-app = "cfa.cli:main_cli"
```

