# Comparing `tmp/zshgpt-0.1.2.tar.gz` & `tmp/zshgpt-0.2.0.tar.gz`

## Comparing `zshgpt-0.1.2.tar` & `zshgpt-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0    81149 2020-02-02 00:00:00.000000 zshgpt-0.1.2/Peek 2023-07-17 17-27.gif
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 zshgpt-0.1.2/src/zshgpt/__about__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.1.2/src/zshgpt/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 zshgpt-0.1.2/src/zshgpt/__main__.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 zshgpt-0.1.2/src/zshgpt/cli/__init__.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 zshgpt-0.1.2/src/zshgpt/cli/messages.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 zshgpt-0.1.2/zsh_plugin/zsh_plugin.zsh
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 zshgpt-0.1.2/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zshgpt-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 zshgpt-0.1.2/README.md
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 zshgpt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 zshgpt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    81149 2020-02-02 00:00:00.000000 zshgpt-0.2.0/Peek 2023-07-17 17-27.gif
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 zshgpt-0.2.0/cicd_plan.md
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 zshgpt-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 zshgpt-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 zshgpt-0.2.0/src/zshgpt/__about__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.2.0/src/zshgpt/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 zshgpt-0.2.0/src/zshgpt/__main__.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 zshgpt-0.2.0/src/zshgpt/cli/__init__.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 zshgpt-0.2.0/src/zshgpt/cli/messages.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 zshgpt-0.2.0/tests/test_main.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 zshgpt-0.2.0/zsh_plugin/zsh_plugin.zsh
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 zshgpt-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zshgpt-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 zshgpt-0.2.0/README.md
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 zshgpt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 zshgpt-0.2.0/PKG-INFO
```

### Comparing `zshgpt-0.1.2/Peek 2023-07-17 17-27.gif` & `zshgpt-0.2.0/Peek 2023-07-17 17-27.gif`

 * *Files identical despite different names*

### Comparing `zshgpt-0.1.2/src/zshgpt/cli/__init__.py` & `zshgpt-0.2.0/src/zshgpt/cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 # SPDX-FileCopyrightText: 2023-present Anders Steen <asteennilsen@gmail.com
 #
 # SPDX-License-Identifier: MIT
-import os
-import shutil
-
 import click
 import openai
 
 from zshgpt.__about__ import __version__
 from zshgpt.cli.messages import messages
```

### Comparing `zshgpt-0.1.2/src/zshgpt/cli/messages.py` & `zshgpt-0.2.0/src/zshgpt/cli/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,22 +17,25 @@
     {
         'role': 'assistant',
         'content': "echo '<html><body><h1>Hello World!</h1></body></html>' > web-app/index.html",
     },
     {'role': 'user', 'content': '# open it with vi'},
     {'role': 'assistant', 'content': 'vi web-app/index.html'},
     {'role': 'user', 'content': '# How do I make a greek salad explained in 4 lines or less'},
-    {'role': 'assistant', 'content': """# To make a Greek salad, you will need:
+    {
+        'role': 'assistant',
+        'content': """# To make a Greek salad, you will need:
 # 1. Chop tomatoes, cucumbers, and red onions.
 # 2. Add feta cheese, Kalamata olives, and fresh herbs like oregano.
 # 3. Drizzle olive oil and lemon juice as dressing.
 # 4. Toss everything together and serve.
 
 # Enjoy your Greek salad!
-"""},
+""",
+    },
     {'role': 'user', 'content': "# what's running on port 1018?"},
     {'role': 'assistant', 'content': 'lsof -i :1018'},
     {'role': 'user', 'content': '# kill process 1584'},
     {'role': 'assistant', 'content': 'kill -9 1584'},
     {'role': 'user', 'content': '# what other devices are on my network?'},
     {'role': 'assistant', 'content': 'arp -a'},
     {'role': 'user', 'content': '# how much storage is left?'},
```

#### html2text {}

```diff
@@ -9,19 +9,19 @@
 processes are hogging the most cpu?'}, {'role': 'assistant', 'content': 'ps aux
 | sort -nrk 3,3 | head -n 10.'}, {'role': 'user', 'content': '# add a hello
 world website to the index'}, { 'role': 'assistant', 'content': "echo '
 ****** Hello World! ******
 ' > web-app/index.html", }, {'role': 'user', 'content': '# open it with vi'},
 {'role': 'assistant', 'content': 'vi web-app/index.html'}, {'role': 'user',
 'content': '# How do I make a greek salad explained in 4 lines or less'},
-{'role': 'assistant', 'content': """# To make a Greek salad, you will need: #
+{ 'role': 'assistant', 'content': """# To make a Greek salad, you will need: #
 1. Chop tomatoes, cucumbers, and red onions. # 2. Add feta cheese, Kalamata
 olives, and fresh herbs like oregano. # 3. Drizzle olive oil and lemon juice as
 dressing. # 4. Toss everything together and serve. # Enjoy your Greek salad!
-"""}, {'role': 'user', 'content': "# what's running on port 1018?"}, {'role':
+""", }, {'role': 'user', 'content': "# what's running on port 1018?"}, {'role':
 'assistant', 'content': 'lsof -i :1018'}, {'role': 'user', 'content': '# kill
 process 1584'}, {'role': 'assistant', 'content': 'kill -9 1584'}, {'role':
 'user', 'content': '# what other devices are on my network?'}, {'role':
 'assistant', 'content': 'arp -a'}, {'role': 'user', 'content': '# how much
 storage is left?'}, {'role': 'assistant', 'content': 'df -h'}, {'role': 'user',
 'content': '# Tell me a joke'}, { 'role': 'assistant', 'content': """# Sure,
 here's a joke for you: Why did the tomato turn red? # Because it saw the salad
```

### Comparing `zshgpt-0.1.2/zsh_plugin/zsh_plugin.zsh` & `zshgpt-0.2.0/zsh_plugin/zsh_plugin.zsh`

 * *Files identical despite different names*

### Comparing `zshgpt-0.1.2/.gitignore` & `zshgpt-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `zshgpt-0.1.2/LICENSE.txt` & `zshgpt-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zshgpt-0.1.2/README.md` & `zshgpt-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `zshgpt-0.1.2/pyproject.toml` & `zshgpt-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,14 @@
 Documentation = "https://github.com/unknown/zshgpt#readme"
 Issues = "https://github.com/unknown/zshgpt/issues"
 Source = "https://github.com/unknown/zshgpt"
 
 [project.scripts]
 zshgpt = "zshgpt.cli:zshgpt"
 
-[tool.hatch.version]
-path = "src/zshgpt/__about__.py"
-
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
@@ -62,14 +59,21 @@
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
 ]
+
+[tool.hatch.version]
+path = "src/zshgpt/__about__.py"
+
+[tool.hatch.build.targets.app]
+
+
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:src/zshgpt tests}"
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
 ]
 fmt = [
```

### Comparing `zshgpt-0.1.2/PKG-INFO` & `zshgpt-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zshgpt
-Version: 0.1.2
+Version: 0.2.0
 Summary: Level up z shell with GPT
 Project-URL: Documentation, https://github.com/unknown/zshgpt#readme
 Project-URL: Issues, https://github.com/unknown/zshgpt/issues
 Project-URL: Source, https://github.com/unknown/zshgpt
 Author-email: Anders Steen <anders.steen@knowit.no>
 License-Expression: MIT
 License-File: LICENSE.txt
```

