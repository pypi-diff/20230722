# Comparing `tmp/lsstream-0.0.1.tar.gz` & `tmp/lsstream-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsstream-0.0.1.tar", last modified: Sat Jul 22 14:43:07 2023, max compression
+gzip compressed data, was "lsstream-0.0.7.tar", last modified: Sat Jul 22 16:41:06 2023, max compression
```

## Comparing `lsstream-0.0.1.tar` & `lsstream-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 14:43:07.692665 lsstream-0.0.1/
--rw-rw-rw-   0        0        0     1082 2023-07-22 14:12:28.000000 lsstream-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      698 2023-07-22 14:43:07.691090 lsstream-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      110 2023-07-22 14:12:28.000000 lsstream-0.0.1/README.md
--rw-rw-rw-   0        0        0      721 2023-07-22 14:42:41.000000 lsstream-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-22 14:43:07.693666 lsstream-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-22 14:43:07.622643 lsstream-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-22 14:43:07.657858 lsstream-0.0.1/src/lsstream/
--rw-rw-rw-   0        0        0        0 2023-07-22 14:17:59.000000 lsstream-0.0.1/src/lsstream/__init__.py
--rw-rw-rw-   0        0        0     1118 2023-07-22 13:03:23.000000 lsstream-0.0.1/src/lsstream/file_generation.py
--rw-rw-rw-   0        0        0     2303 2023-07-22 14:24:45.000000 lsstream-0.0.1/src/lsstream/main.py
--rw-rw-rw-   0        0        0      834 2023-07-22 13:01:34.000000 lsstream-0.0.1/src/lsstream/prompts.py
--rw-rw-rw-   0        0        0      215 2023-07-22 12:58:49.000000 lsstream-0.0.1/src/lsstream/style.py
--rw-rw-rw-   0        0        0      164 2023-07-22 13:02:15.000000 lsstream-0.0.1/src/lsstream/template.py
--rw-rw-rw-   0        0        0      278 2023-07-22 13:02:29.000000 lsstream-0.0.1/src/lsstream/test.py
-drwxrwxrwx   0        0        0        0 2023-07-22 14:43:07.688123 lsstream-0.0.1/src/lsstream.egg-info/
--rw-rw-rw-   0        0        0      698 2023-07-22 14:43:07.000000 lsstream-0.0.1/src/lsstream.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-07-22 14:43:07.000000 lsstream-0.0.1/src/lsstream.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 14:43:07.000000 lsstream-0.0.1/src/lsstream.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-22 14:43:07.000000 lsstream-0.0.1/src/lsstream.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-22 14:43:07.000000 lsstream-0.0.1/src/lsstream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:41:06.578504 lsstream-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-22 16:40:55.000000 lsstream-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-22 16:41:06.578504 lsstream-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-22 16:40:55.000000 lsstream-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-22 16:40:55.000000 lsstream-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 16:41:06.578504 lsstream-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:41:06.574504 lsstream-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:41:06.578504 lsstream-0.0.7/src/lsstream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:40:55.000000 lsstream-0.0.7/src/lsstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-22 16:40:55.000000 lsstream-0.0.7/src/lsstream/file_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-22 16:40:55.000000 lsstream-0.0.7/src/lsstream/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-22 16:40:55.000000 lsstream-0.0.7/src/lsstream/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-22 16:40:55.000000 lsstream-0.0.7/src/lsstream/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-22 16:40:55.000000 lsstream-0.0.7/src/lsstream/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-22 16:40:55.000000 lsstream-0.0.7/src/lsstream/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:41:06.578504 lsstream-0.0.7/src/lsstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-22 16:41:06.000000 lsstream-0.0.7/src/lsstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-22 16:41:06.000000 lsstream-0.0.7/src/lsstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:41:06.000000 lsstream-0.0.7/src/lsstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-22 16:41:06.000000 lsstream-0.0.7/src/lsstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 16:41:06.000000 lsstream-0.0.7/src/lsstream.egg-info/top_level.txt
```

### Comparing `lsstream-0.0.1/PKG-INFO` & `lsstream-0.0.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
-Name: lsstream
-Version: 0.0.1
-Summary: To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
-Author-email: Wermutton <redacted@redacted.redacted>
-Project-URL: Homepage, https://github.com/Wermutton/lsstream
-Project-URL: Bug Tracker, https://github.com/Wermutton/lsstream/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# lsstream
-To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests :sleeping: :desktop: 
+Metadata-Version: 2.1
+Name: lsstream
+Version: 0.0.7
+Summary: To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
+Author-email: Wermutton <redacted@redacted.redacted>
+Project-URL: Homepage, https://github.com/Wermutton/lsstream
+Project-URL: Bug Tracker, https://github.com/Wermutton/lsstream/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# lsstream
+To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
```

### Comparing `lsstream-0.0.1/pyproject.toml` & `lsstream-0.0.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "lsstream"
-version = "0.0.1"
-authors = [
-  { name="Wermutton", email="redacted@redacted.redacted" },
-]
-description = "To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️"
-readme = "README.md"
-requires-python = ">=3.7"
-dependencies = [
-  "pyfiglet",
-  "termcolor"
-]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/Wermutton/lsstream"
-"Bug Tracker" = "https://github.com/Wermutton/lsstream/issues"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "lsstream"
+version = "0.0.7"
+authors = [
+  { name="Wermutton", email="redacted@redacted.redacted" },
+]
+description = "To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️"
+readme = "README.md"
+requires-python = ">=3.7"
+dependencies = [
+  "pyfiglet",
+  "termcolor"
+]
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/Wermutton/lsstream"
+"Bug Tracker" = "https://github.com/Wermutton/lsstream/issues"
```

### Comparing `lsstream-0.0.1/src/lsstream/file_generation.py` & `lsstream-0.0.7/src/lsstream/file_generation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import os
-from template import TEMPLATE_1     # choose the template you want
-from style import color
-from prompts import prompt_directory, prompt_details
-
-# Creates the files and returns its contents
-def create_file(movie_title, media_link, output_directory):
-    output_file_path = os.path.join(output_directory, f'{movie_title}.txt')
-    file_content = TEMPLATE_1.format(LINK=media_link, TITLE=movie_title)
-
-    with open(output_file_path, 'w') as f:
-        f.write(file_content)
-    
-    return output_file_path, file_content 
-
-# Loop for file and content generation
-def create_content():
-    new_contents = []
-    new_files = []
-
-    output_directory = prompt_directory()
-
-    while True:
-        movie_title, media_link = prompt_details()
-        new_file, new_content = create_file(movie_title, media_link, output_directory)  
-
-        new_files.append(new_file)
-        new_contents.append(new_content)  
-
-        continue_prompt = input(color('\nContinue? (Y/N): ', 'white'))
-        if continue_prompt.lower() != 'y':
-            break
-    
+import os
+from .template import TEMPLATE_1     # choose the template you want
+from .style import color
+from .prompts import prompt_directory, prompt_details
+
+# Creates the files and returns its contents
+def create_file(movie_title, media_link, output_directory):
+    output_file_path = os.path.join(output_directory, f'{movie_title}.txt')
+    file_content = TEMPLATE_1.format(LINK=media_link, TITLE=movie_title)
+
+    with open(output_file_path, 'w') as f:
+        f.write(file_content)
+    
+    return output_file_path, file_content 
+
+# Loop for file and content generation
+def create_content():
+    new_contents = []
+    new_files = []
+
+    output_directory = prompt_directory()
+
+    while True:
+        movie_title, media_link = prompt_details()
+        new_file, new_content = create_file(movie_title, media_link, output_directory)  
+
+        new_files.append(new_file)
+        new_contents.append(new_content)  
+
+        continue_prompt = input(color('\nContinue? (Y/N): ', 'white'))
+        if continue_prompt.lower() != 'y':
+            break
+    
     return new_files, new_contents
```

### Comparing `lsstream-0.0.1/src/lsstream/main.py` & `lsstream-0.0.7/src/lsstream/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-import os
-import webbrowser
-from style import intro, color
-from file_generation import create_content
-from prompts import prompt_test_html
-from test import test_html
-
-# Delete current batch of html files
-def end_session(new_files, new_contents):
-    end_prompt = input(color('\nAre you done with this session? (Y/N): ', 'white'))
-    if end_prompt.lower() == 'y':
-        if os.path.exists('temp.html'):
-            os.remove('temp.html')
-
-        print(color(f'\n✔ Done!', 'green'))
-
-    else:
-        while True:
-            print(color('\nA: Start a new batch?', 'yellow'))
-            print(color('B: Test the media(s)?', 'cyan'))
-            print(color('C: Remove the newly created files and restart?', 'red'))
-            print(color('D: End session?', 'green'))
-            continue_prompt = input(color('What would you like to do? (', 'white') + color('A', 'yellow') + color('/', 'white') + color('B', 'cyan') + color('/', 'white') + color('C', 'red') + color('/', 'white') + color('D', 'green') + color('): ', 'white'))
-            
-            if continue_prompt.lower() == 'a':
-                lsstream()
-                break
-            elif continue_prompt.lower() == 'b':
-                webbrowser.open('file://' + os.path.realpath('temp.html'))
-                end_session(new_files, new_contents)
-                break
-            elif continue_prompt.lower() == 'c':
-                for file in new_files:
-                    os.remove(file)
-                if os.path.exists('temp.html'):
-                    os.remove('temp.html')
-                lsstream()
-                break
-            elif continue_prompt.lower() == 'd':
-                if os.path.exists('temp.html'):
-                    os.remove('temp.html')
-                    
-                print(color(f'\n✔ Done!', 'green'))
-                break
-            else:
-                print(color('\nInvalid option, please choose A, B, or C.', 'red'))
-
-def lsstream():    
-    new_files, new_contents = create_content()
-
-    if prompt_test_html(new_contents): test_html(new_contents)
-
-    end_session(new_files, new_contents) 
-
-
-def main():
-    print(color(intro.renderText('LSSTREAM'), 'green'))
-    lsstream() 
-
-if __name__ == "__main__":
-    main()
+import os
+import webbrowser
+from .style import intro, color
+from .file_generation import create_content
+from .prompts import prompt_test_html
+from .test import test_html
+
+# Delete current batch of html files
+def end_session(new_files, new_contents):
+    end_prompt = input(color('\nAre you done with this session? (Y/N): ', 'white'))
+    if end_prompt.lower() == 'y':
+        if os.path.exists('temp.html'):
+            os.remove('temp.html')
+
+        print(color(f'\n✔ Done!', 'green'))
+
+    else:
+        while True:
+            print(color('\nA: Start a new batch?', 'yellow'))
+            print(color('B: Test the media(s)?', 'cyan'))
+            print(color('C: Remove the newly created files and restart?', 'red'))
+            print(color('D: End session?', 'green'))
+            continue_prompt = input(color('What would you like to do? (', 'white') + color('A', 'yellow') + color('/', 'white') + color('B', 'cyan') + color('/', 'white') + color('C', 'red') + color('/', 'white') + color('D', 'green') + color('): ', 'white'))
+            
+            if continue_prompt.lower() == 'a':
+                lsstream()
+                break
+            elif continue_prompt.lower() == 'b':
+                webbrowser.open('file://' + os.path.realpath('temp.html'))
+                end_session(new_files, new_contents)
+                break
+            elif continue_prompt.lower() == 'c':
+                for file in new_files:
+                    os.remove(file)
+                if os.path.exists('temp.html'):
+                    os.remove('temp.html')
+                lsstream()
+                break
+            elif continue_prompt.lower() == 'd':
+                if os.path.exists('temp.html'):
+                    os.remove('temp.html')
+                    
+                print(color(f'\n✔ Done!', 'green'))
+                break
+            else:
+                print(color('\nInvalid option, please choose A, B, or C.', 'red'))
+
+def lsstream():    
+    new_files, new_contents = create_content()
+
+    if prompt_test_html(new_contents): test_html(new_contents)
+
+    end_session(new_files, new_contents) 
+
+
+def main():
+    print(color(intro.renderText('LSSTREAM'), 'green'))
+    lsstream() 
+
+if __name__ == "__main__":
+    main()
```

### Comparing `lsstream-0.0.1/src/lsstream.egg-info/PKG-INFO` & `lsstream-0.0.7/src/lsstream.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
-Name: lsstream
-Version: 0.0.1
-Summary: To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
-Author-email: Wermutton <redacted@redacted.redacted>
-Project-URL: Homepage, https://github.com/Wermutton/lsstream
-Project-URL: Bug Tracker, https://github.com/Wermutton/lsstream/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# lsstream
-To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests :sleeping: :desktop: 
+Metadata-Version: 2.1
+Name: lsstream
+Version: 0.0.7
+Summary: To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
+Author-email: Wermutton <redacted@redacted.redacted>
+Project-URL: Homepage, https://github.com/Wermutton/lsstream
+Project-URL: Bug Tracker, https://github.com/Wermutton/lsstream/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# lsstream
+To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
```

