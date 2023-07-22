# Comparing `tmp/hytato-0.2.tar.gz` & `tmp/hytato-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hytato-0.2.tar", last modified: Fri Jul 21 10:38:14 2023, max compression
+gzip compressed data, was "hytato-0.3.tar", last modified: Sat Jul 22 15:27:37 2023, max compression
```

## Comparing `hytato-0.2.tar` & `hytato-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:14.496197 hytato-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-21 10:38:02.000000 hytato-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-21 10:38:14.496197 hytato-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-21 10:38:02.000000 hytato-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:14.492197 hytato-0.2/hytato/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-21 10:38:02.000000 hytato-0.2/hytato/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-07-21 10:38:02.000000 hytato-0.2/hytato/hytato.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:38:14.496197 hytato-0.2/hytato.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-21 10:38:14.000000 hytato-0.2/hytato.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-21 10:38:14.000000 hytato-0.2/hytato.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:38:14.000000 hytato-0.2/hytato.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 10:38:14.000000 hytato-0.2/hytato.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 10:38:14.496197 hytato-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-21 10:38:02.000000 hytato-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:27:37.978606 hytato-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-22 15:27:19.000000 hytato-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-22 15:27:37.978606 hytato-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-22 15:27:19.000000 hytato-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:27:37.974606 hytato-0.3/hytato/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-22 15:27:19.000000 hytato-0.3/hytato/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-07-22 15:27:19.000000 hytato-0.3/hytato/hytato.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:27:37.974606 hytato-0.3/hytato.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-22 15:27:37.000000 hytato-0.3/hytato.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-22 15:27:37.000000 hytato-0.3/hytato.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 15:27:37.000000 hytato-0.3/hytato.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-22 15:27:37.000000 hytato-0.3/hytato.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 15:27:37.978606 hytato-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-22 15:27:19.000000 hytato-0.3/setup.py
```

### Comparing `hytato-0.2/LICENSE` & `hytato-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hytato-0.2/README.md` & `hytato-0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 # hytato
- Module for storing python dictionaries in a different format.
-
-Supported down to python 3.2.
+Module for storing python dictionaries in a different format.
+Supported down to python 3.3.
 
 ### why?
 cause why not?
 
-Needed a way to store data in a way that fit *my* needs, and so decided to create potato(lib) 
-
+Needed a way to store data in a way that fit *my* needs, and so decided to create potato(lib).
 Potato works with dictionaries. You could use json for that but as I said, needed something for *my* needs.
 
 ### Potato types
 There are two different kinds of potato files: HTATO and STATO.
 
 HTATO or hard potato have a fixed number of keys.
 STATO or soft potato don't have a fixed number of keys.
 
-There are a number of other differences which will be made clear later
-
+There are a number of other differences which will be made clearer in the future.
 One difference being that STATO files are inherently different. The HTATO files are really just `.txt`, whereas STATO are zip files.
 This means you can store a "tree" of data, and also version history
 
 ### Usage
 HTATO example:
-```py
-from potato import POTATO
+
+```
+from hytato import POTATO
 
 #Add the path of the potato file in HTATO class, which will have either the .htato or .stato file extension.
 config_potato = POTATO.HTATO('.\\config.htato')
 
 #if it doesn't exist yet, create the potato file
 #add the list of keys you want
 config_potato.PLANT(['token', 'passcode', 'fatherless'])
```

### Comparing `hytato-0.2/hytato/hytato.py` & `hytato-0.3/hytato/hytato.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,58 @@
-import ast; import os; import sys; from zipfile import ZipFile, ZipInfo
-
+import ast; import os; import sys; from zipfile import ZipFile, ZipInfo; import warnings; import inspect; import platform; import multiprocessing; import time
 '''
+Hyphens Potato is a module allowing you (more me) to store dictionaries in a way that I (yes I) would like.
+I needed a middle ground between a database and json, in addition to it being light, powerful, and just simple
+to interact with (for me). Main thing is probably to not lose your data while using files as a near db
+
+Because of that last one, this is mainly for windows, but supports linux
+OS is only important if you use HTATO though. Since file locking was difficult for zip archives, which is what
+STATO files actually are. STATO uses a flag file inside to indicate some other process is inside. There is a 
+timeout on the file though. If a process wait for more than 5 seconds (too much time in computer terms) then it
+ignores it carries on. This only affects inject operations btw. Any read operations in stato do not give regard 
+to the flag.
+I would very much prefer STATO also use msvcrt & fcntl filelocks. The issue I faced was with file descriptors.
+If someone has a suggestion on getting file descriptors from zip files hmu pls!
+
 HTATO stands for HARD POTATO. These files must be created by the HTATO class, and has fixed keys.
 Meaning you can not easily add a new key to it. This makes it more suitable for files storing the 
 permanent data like status or settings.
 
 STATO stands for SOFT POTATO. These can have a variable number of keys. Making it more suitable
 for files that might be used to store temporary data.
 
 Apart from the number of keys, HTATO and STATO have other characteristics that make it suitable for their use
 
 .potato files are for use by potato lib only (!)
 '''
 
+system_os = platform.uname().system
+if system_os == 'Windows':
+    import msvcrt
+    def lock_file(file_descriptor: int, file_path: str):
+        msvcrt.locking(file_descriptor, msvcrt.LK_LOCK, os.path.getsize(file_path))
+
+    def unlock_file(file_descriptor: int, file_path: str):
+        msvcrt.locking(file_descriptor, msvcrt.LK_UNLCK, os.path.getsize(file_path))
+
+elif system_os == 'Linux':
+    import fcntl
+    def lock_file(file_descriptor: int, file_path: str):
+        fcntl.flock(file_descriptor, fcntl.LOCK_EX | fcntl.LOCK_NB)
+
+    def unlock_file(file_descriptor: int, file_path: str):
+        fcntl.flock(file_descriptor, fcntl.LOCK_UN)
+
+elif bool(system_os) == False:
+    warnings.warn('Platform module could not get system os. Hytato will not load')
+    sys.exit()
+else:
+    warnings.warn('Platform module reported an unsupported os. Hytato will not load')
+    sys.exit()
+
 version_major = int(sys.version_info.major)
 version_minor = int(sys.version_info.minor)
 
 # Exceptions:
 
 class POTATOExists(Exception):
     """Exception for when the specified potato file (whether hard or soft) already exists in the directory"""
@@ -39,17 +75,22 @@
         if os.path.exists(args[0].potato) == True:
             raise POTATOExists('Found existing potato file at path')
         return fn(*args, **kwargs)
     return func
 
 def CheckPotatoNonExistant(fn):
     """must have self parameter and the potato path inside self parameter: self.potato"""
+    signature = inspect.signature(fn)
     def func(*args, **kwargs):
         if os.path.exists(args[0].potato) == False:
-            raise POTATONonExists('Did not find existing potato file at path')
+            if signature.parameters.get('plant_if_non_existant'):
+                args[0].PLANT(KEYS=list(kwargs['data'].keys()))
+                warnings.warn('Did not find existing potato file at path. Created one for you')
+            else:
+                raise POTATONonExists('Did not find existing potato file at path')
         return fn(*args, **kwargs)
     return func
 
 # Return classes:
 
 class potato_returns():
     class stato():
@@ -135,17 +176,19 @@
             parsed = dict()
             for x in read:
                 if bool(x): #since its not .readlines() we need to make sure the string actually has something
                     x = x.replace("\n", "").split(':')  # unlikely to have "\n" in the string now but eh
                     key = x[0].strip()
                     value = ast.literal_eval(x[1].strip())
                     parsed[key] = value
+
             return parsed
 
-        def INJECT(self, data: dict, starch: str = 'data') -> potato_returns.stato.StatoInjectReturn:
+        @CheckPotatoNonExistant
+        def INJECT(self, *, data: dict, starch: str = 'data', plant_if_non_existant: bool = True) -> potato_returns.stato.StatoInjectReturn:
             """Update the data in the potato file at the path. Starch specifies the part you want to edit.\n
             Type 'data' (default) for the simple dictionary stored inside, or 'config' for the preferences set during planting. 'history' is not yet supported
             returns a StatoInjectReturn class with parameters: complete, update, all"""
 
             if starch == 'data':
                 starch = 'data.potato'
             if starch == 'config':
@@ -208,20 +251,38 @@
                         if type(value) == str:
                             value = '"{}"'.format(value)
                         oldpotatofile_string += '{}: {}'.format(key, value) + '\n'
                     history['version_history/{}.txt'.format(index)] = oldpotatofile_string
 
                 zipfile.close()
 
-            #after this, the old potato is cleared...
+
+            flag_file_path = os.path.dirname(self.potato) + '\\' + (os.path.basename(self.potato).split('.')[0] + '.flag')
+            green_light = False
+            start = time.perf_counter()
+            #about 6 - 8 seconds
+            for x in range(70000000):
+                if os.path.exists(flag_file_path):
+                    pass
+                else:
+                    green_light = True
+                    break
+            stop = time.perf_counter()
+            if green_light == False:
+                warnings.warn('The inject method waited {} fractional seconds before ignoring the flag.'.format(stop-start))
+
             with ZipFile(self.potato, 'w') as zipfile:
+                with open(flag_file_path, 'w') as flag_file:
+                    flag_file.write(str([multiprocessing.process.current_process(), platform.python_build(), platform.uname()]))
+                    flag_file.close()
                 zipfile.writestr(data=potatofile_string, zinfo_or_arcname='data.potato')
                 zipfile.writestr(data=configfile_string, zinfo_or_arcname='config.potato')
                 for x in history.keys():
                     zipfile.writestr(data=history[x], zinfo_or_arcname=x)
+                os.remove(flag_file_path)
                 zipfile.close()
 
             return potato_returns.stato.StatoInjectReturn(complete=True, update=data, all=data_stained) #all needs to be edited to account for the starch
 
     class HTATO():
         def __init__(self, potato: str) -> None:
             """HTATO stands for HARD POTATO. These files must be created by the HTATO class, and has fixed keys. Meaning you can not easily add a new key to it. This makes it more suitable for files storing the permanent data like status or settings."""
@@ -254,14 +315,15 @@
             parsed = dict()
             for x in read:
                 # python still sometimes read the \n ending.
                 x = x.replace("\n", "").split(':')
                 key = x[0].strip()
                 value = ast.literal_eval(x[1].strip())
                 parsed[key] = value
+
             return parsed
 
         @CheckPotatoNonExistant
         def INJECT(self, data: dict) -> potato_returns.htato.HtatoInjectReturn:
             """Update the data in the potato file at the path.\n
             returns a HtatoInjectReturn class with parameters: complete, update, all"""
 
@@ -273,12 +335,15 @@
             potatofile_string = str()
             for x in stained.keys():
                 key = x
                 value = stained[key]
                 if type(value) == str:
                     value = '"{}"'.format(value)
                 potatofile_string += '{}: {}'.format(key, value) + '\n'
+
             potatofile = open(self.potato, 'w')
+            lock_file(potatofile.fileno(), self.potato)
             potatofile.write(potatofile_string)
+            unlock_file(potatofile.fileno(), self.potato)
             potatofile.close()
 
             return potato_returns().htato().HtatoInjectReturn(complete=True, update=data, all=stained)
```

