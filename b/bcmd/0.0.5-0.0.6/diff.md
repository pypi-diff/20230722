# Comparing `tmp/bcmd-0.0.5.tar.gz` & `tmp/bcmd-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcmd-0.0.5.tar", last modified: Sat Jul 22 02:11:42 2023, max compression
+gzip compressed data, was "bcmd-0.0.6.tar", last modified: Sat Jul 22 06:58:07 2023, max compression
```

## Comparing `bcmd-0.0.5.tar` & `bcmd-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 02:11:42.547428 bcmd-0.0.5/
--rw-rw-rw-   0        0        0      239 2023-07-22 02:11:42.546427 bcmd-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-22 02:11:42.536390 bcmd-0.0.5/bcmd/
--rw-rw-rw-   0        0        0        0 2023-07-21 02:19:54.000000 bcmd-0.0.5/bcmd/__init__.py
--rw-rw-rw-   0        0        0      430 2023-07-20 07:37:53.000000 bcmd-0.0.5/bcmd/dev.py
--rw-rw-rw-   0        0        0      259 2023-07-22 02:11:10.000000 bcmd-0.0.5/bcmd/main.py
-drwxrwxrwx   0        0        0        0 2023-07-22 02:11:42.545428 bcmd-0.0.5/bcmd/tasks/
--rw-rw-rw-   0        0        0        0 2023-07-20 07:37:38.000000 bcmd-0.0.5/bcmd/tasks/__init__.py
--rw-rw-rw-   0        0        0     2488 2023-07-21 02:02:14.000000 bcmd-0.0.5/bcmd/tasks/time.py
-drwxrwxrwx   0        0        0        0 2023-07-22 02:11:42.544426 bcmd-0.0.5/bcmd.egg-info/
--rw-rw-rw-   0        0        0      239 2023-07-22 02:11:42.000000 bcmd-0.0.5/bcmd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-07-22 02:11:42.000000 bcmd-0.0.5/bcmd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 02:11:42.000000 bcmd-0.0.5/bcmd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-22 02:11:42.000000 bcmd-0.0.5/bcmd.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      149 2023-07-22 02:11:42.000000 bcmd-0.0.5/bcmd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-22 02:11:42.000000 bcmd-0.0.5/bcmd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      622 2023-07-22 02:11:26.000000 bcmd-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-22 02:11:42.547428 bcmd-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-22 06:58:07.526740 bcmd-0.0.6/
+-rw-rw-rw-   0        0        0      239 2023-07-22 06:58:07.525740 bcmd-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-22 06:58:07.517739 bcmd-0.0.6/bcmd/
+-rw-rw-rw-   0        0        0        0 2023-07-21 02:19:54.000000 bcmd-0.0.6/bcmd/__init__.py
+-rw-rw-rw-   0        0        0      473 2023-07-22 06:56:21.000000 bcmd-0.0.6/bcmd/dev.py
+-rw-rw-rw-   0        0        0      259 2023-07-22 02:11:10.000000 bcmd-0.0.6/bcmd/main.py
+drwxrwxrwx   0        0        0        0 2023-07-22 06:58:07.524740 bcmd-0.0.6/bcmd/tasks/
+-rw-rw-rw-   0        0        0        0 2023-07-20 07:37:38.000000 bcmd-0.0.6/bcmd/tasks/__init__.py
+-rw-rw-rw-   0        0        0     2476 2023-07-22 06:27:05.000000 bcmd-0.0.6/bcmd/tasks/time.py
+drwxrwxrwx   0        0        0        0 2023-07-22 06:58:07.522740 bcmd-0.0.6/bcmd.egg-info/
+-rw-rw-rw-   0        0        0      239 2023-07-22 06:58:07.000000 bcmd-0.0.6/bcmd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-07-22 06:58:07.000000 bcmd-0.0.6/bcmd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 06:58:07.000000 bcmd-0.0.6/bcmd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-22 06:58:07.000000 bcmd-0.0.6/bcmd.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      149 2023-07-22 06:58:07.000000 bcmd-0.0.6/bcmd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-22 06:58:07.000000 bcmd-0.0.6/bcmd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      622 2023-07-22 06:56:33.000000 bcmd-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-22 06:58:07.526740 bcmd-0.0.6/setup.cfg
```

### Comparing `bcmd-0.0.5/bcmd/tasks/time.py` & `bcmd-0.0.6/bcmd/tasks/time.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,8 +67,7 @@
     for tzname in tzname_list:
         datetime_tz = datetime_utc.astimezone(ZoneInfo(tzname))
         dstStr = ''
         dst = datetime_tz.dst()
         if dst:
             dstStr = f'(DST+{dst})'
         print(f'{datetime_tz} {tzname} {dstStr}')
-    print()
```

### Comparing `bcmd-0.0.5/pyproject.toml` & `bcmd-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # https://peps.python.org/pep-0621/#example
 
 [project]
 name = "bcmd"
-version = "0.0.5"
+version = "0.0.6"
 description = "Utils commands for Beni"
 requires-python = ">=3.10"
 keywords = ["benimang", "beni", "bcmd"]
 authors = [
   {email = "benimang@126.com"},
   {name = "Beni Mang"}
 ]
@@ -15,15 +15,15 @@
 ]
 
 dependencies = [
   'aioconsole',
   'aiofiles',
   'aiohttp',
   'autopep8',
-  'benimang==0.4.2',
+  'benimang==0.4.4',
   'build',
   'colorama',
   'nest-asyncio',
   'orjson',
   'portalocker',
   'pretty_errors',
   'pyperclip',
```

