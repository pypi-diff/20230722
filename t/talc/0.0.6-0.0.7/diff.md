# Comparing `tmp/talc-0.0.6.tar.gz` & `tmp/talc-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talc-0.0.6.tar", last modified: Fri Jul 21 19:39:24 2023, max compression
+gzip compressed data, was "talc-0.0.7.tar", last modified: Fri Jul 21 22:22:06 2023, max compression
```

## Comparing `talc-0.0.6.tar` & `talc-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-21 19:39:24.433575 talc-0.0.6/
--rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:11:13.000000 talc-0.0.6/LICENSE
--rw-r--r--   0 mkerr      (501) staff       (20)     2065 2023-07-21 19:39:24.433450 talc-0.0.6/PKG-INFO
--rw-r--r--   0 mkerr      (501) staff       (20)     1642 2023-07-20 23:07:33.000000 talc-0.0.6/README.md
--rw-r--r--   0 mkerr      (501) staff       (20)      585 2023-07-21 19:37:59.000000 talc-0.0.6/pyproject.toml
--rw-r--r--   0 mkerr      (501) staff       (20)       38 2023-07-21 19:39:24.433606 talc-0.0.6/setup.cfg
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-21 19:39:24.431987 talc-0.0.6/src/
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-21 19:39:24.432485 talc-0.0.6/src/talc/
--rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:12:06.000000 talc-0.0.6/src/talc/__init__.py
--rw-r--r--   0 mkerr      (501) staff       (20)    10553 2023-07-21 19:27:01.000000 talc-0.0.6/src/talc/talc.py
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-21 19:39:24.433309 talc-0.0.6/src/talc.egg-info/
--rw-r--r--   0 mkerr      (501) staff       (20)     2065 2023-07-21 19:39:24.000000 talc-0.0.6/src/talc.egg-info/PKG-INFO
--rw-r--r--   0 mkerr      (501) staff       (20)      229 2023-07-21 19:39:24.000000 talc-0.0.6/src/talc.egg-info/SOURCES.txt
--rw-r--r--   0 mkerr      (501) staff       (20)        1 2023-07-21 19:39:24.000000 talc-0.0.6/src/talc.egg-info/dependency_links.txt
--rw-r--r--   0 mkerr      (501) staff       (20)       31 2023-07-21 19:39:24.000000 talc-0.0.6/src/talc.egg-info/requires.txt
--rw-r--r--   0 mkerr      (501) staff       (20)        5 2023-07-21 19:39:24.000000 talc-0.0.6/src/talc.egg-info/top_level.txt
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-21 22:22:06.810775 talc-0.0.7/
+-rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:11:13.000000 talc-0.0.7/LICENSE
+-rw-r--r--   0 mkerr      (501) staff       (20)     2065 2023-07-21 22:22:06.810666 talc-0.0.7/PKG-INFO
+-rw-r--r--   0 mkerr      (501) staff       (20)     1642 2023-07-20 23:07:33.000000 talc-0.0.7/README.md
+-rw-r--r--   0 mkerr      (501) staff       (20)      585 2023-07-21 22:21:50.000000 talc-0.0.7/pyproject.toml
+-rw-r--r--   0 mkerr      (501) staff       (20)       38 2023-07-21 22:22:06.810805 talc-0.0.7/setup.cfg
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-21 22:22:06.809343 talc-0.0.7/src/
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-21 22:22:06.809848 talc-0.0.7/src/talc/
+-rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:12:06.000000 talc-0.0.7/src/talc/__init__.py
+-rw-r--r--   0 mkerr      (501) staff       (20)    10653 2023-07-21 22:20:08.000000 talc-0.0.7/src/talc/talc.py
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2023-07-21 22:22:06.810529 talc-0.0.7/src/talc.egg-info/
+-rw-r--r--   0 mkerr      (501) staff       (20)     2065 2023-07-21 22:22:06.000000 talc-0.0.7/src/talc.egg-info/PKG-INFO
+-rw-r--r--   0 mkerr      (501) staff       (20)      229 2023-07-21 22:22:06.000000 talc-0.0.7/src/talc.egg-info/SOURCES.txt
+-rw-r--r--   0 mkerr      (501) staff       (20)        1 2023-07-21 22:22:06.000000 talc-0.0.7/src/talc.egg-info/dependency_links.txt
+-rw-r--r--   0 mkerr      (501) staff       (20)       31 2023-07-21 22:22:06.000000 talc-0.0.7/src/talc.egg-info/requires.txt
+-rw-r--r--   0 mkerr      (501) staff       (20)        5 2023-07-21 22:22:06.000000 talc-0.0.7/src/talc.egg-info/top_level.txt
```

### Comparing `talc-0.0.6/PKG-INFO` & `talc-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talc
-Version: 0.0.6
+Version: 0.0.7
 Summary: Logging client for Talc Debugger.
 Author-email: Max Kerr <max@talc.ai>, Matt Lee <matt@talc.ai>
 Project-URL: homepage, https://talc.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `talc-0.0.6/README.md` & `talc-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `talc-0.0.6/pyproject.toml` & `talc-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "talc"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Max Kerr", email="max@talc.ai" },
   { name="Matt Lee", email="matt@talc.ai" },
 ]
 description = "Logging client for Talc Debugger."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `talc-0.0.6/src/talc/talc.py` & `talc-0.0.7/src/talc/talc.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,24 +45,25 @@
                     "organization": self.__organization,
                 }
             )
             .execute()
         )
         return response.data[0]["id"]
 
-    def __createInput(self, sessionId, generationId, role, content, index):
+    def __createInput(self, sessionId, generationId, role, content, name, index):
         response = (
             self.supabase.table("inputs")
             .insert(
                 {
                     "session": sessionId,
                     "generation": generationId,
                     "role": role,
                     "content": content,
                     "index": index,
+                    "name": name,
                 }
             )
             .execute()
         )
         return response.data[0]["id"]
 
     def __createGeneration(
@@ -95,14 +96,15 @@
     def __historyArrayToInputs(self, history, generationId, sessionId):
         for index, chat in enumerate(history):
             self.__createInput(
                 sessionId,
                 generationId,
                 chat["role"],
                 chat["content"],
+                chat.get("name", None),  # Name is optional
                 # Index is reversed because we want the most recent message to have the lowest index
                 len(history) - index,
             )
 
     def log(
         self,
         sessionId,
```

### Comparing `talc-0.0.6/src/talc.egg-info/PKG-INFO` & `talc-0.0.7/src/talc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talc
-Version: 0.0.6
+Version: 0.0.7
 Summary: Logging client for Talc Debugger.
 Author-email: Max Kerr <max@talc.ai>, Matt Lee <matt@talc.ai>
 Project-URL: homepage, https://talc.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

