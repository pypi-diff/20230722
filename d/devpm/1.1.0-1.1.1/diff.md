# Comparing `tmp/devpm-1.1.0.tar.gz` & `tmp/devpm-1.1.1.tar.gz`

## Comparing `devpm-1.1.0.tar` & `devpm-1.1.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     9103 2020-02-02 00:00:00.000000 devpm-1.1.0/devpackage.schema.json
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/__main__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/__init__.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/cli/base_command.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/cli/main.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/__init__.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/base_run.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/cr.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/install.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/lint.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/pr.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/restart.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/run.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/start.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/stop.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/test.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/commands/version.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/utils/bash.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/utils/bin.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/utils/code.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/utils/context.py
--rw-r--r--   0        0        0    10298 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/utils/git.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/utils/log.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 devpm-1.1.0/devpm/_internal/utils/pip.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 devpm-1.1.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 devpm-1.1.0/LICENSE
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 devpm-1.1.0/README.md
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 devpm-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 devpm-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     9260 2020-02-02 00:00:00.000000 devpm-1.1.1/devpackage.schema.json
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/__main__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/__init__.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/cli/base_command.py
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/cli/main.py
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/commands/base_run.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/commands/cr.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/commands/githook.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/commands/install.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/commands/lint.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/commands/pr.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/commands/restart.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/commands/run.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/commands/start.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/commands/stop.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/commands/test.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/commands/version.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/utils/bash.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/utils/bin.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/utils/code.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/utils/context.py
+-rw-r--r--   0        0        0     9179 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/utils/git.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/utils/log.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 devpm-1.1.1/devpm/_internal/utils/pip.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 devpm-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 devpm-1.1.1/LICENSE
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 devpm-1.1.1/README.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 devpm-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 devpm-1.1.1/PKG-INFO
```

### Comparing `devpm-1.1.0/devpackage.schema.json` & `devpm-1.1.1/devpackage.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999962903608737%*

 * *Differences: {"'definitions'": "{'gitHook': {'properties': {'commit-msg': {'properties': {'pattern': "*

 * *                  "{'description': 'The pattern(s) to match the commit-msg', 'oneOf': "*

 * *                  "[OrderedDict([('type', 'string'), ('format', 'regex')]), OrderedDict([('type', "*

 * *                  "'array'), ('items', OrderedDict([('type', 'string'), ('format', 'regex')]))])], "*

 * *                  "delete: ['type']}}}}}}"}*

```diff
@@ -4,16 +4,28 @@
         "gitHook": {
             "description": "Write to git hooks for root project and it's git submodules. Support commit-msg, pre-commit",
             "properties": {
                 "commit-msg": {
                     "description": "The commit-msg git hook.",
                     "properties": {
                         "pattern": {
-                            "description": "The pattern for type regexp",
-                            "type": "string"
+                            "description": "The pattern(s) to match the commit-msg",
+                            "oneOf": [
+                                {
+                                    "format": "regex",
+                                    "type": "string"
+                                },
+                                {
+                                    "items": {
+                                        "format": "regex",
+                                        "type": "string"
+                                    },
+                                    "type": "array"
+                                }
+                            ]
                         },
                         "tips": {
                             "description": "The tips to show when the commit-msg test failed, used array to show multi-line.",
                             "items": {
                                 "type": "string"
                             },
                             "type": "array"
```

### Comparing `devpm-1.1.0/devpm/__main__.py` & `devpm-1.1.1/devpm/__main__.py`

 * *Files identical despite different names*

### Comparing `devpm-1.1.0/devpm/_internal/cli/base_command.py` & `devpm-1.1.1/devpm/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `devpm-1.1.0/devpm/_internal/cli/main.py` & `devpm-1.1.1/devpm/_internal/cli/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     parser = ArgumentParser(add_help=False)
     parser.usage = "devpm <commands> [options]"
     parser.description = "Development package manager."
     parser.epilog = "See <http://github.com/wequick/devpm> for the full manual."
 
     parser.add_argument('-h', '--help', action="help")
     parser.add_argument('-v', '--version', dest='version', action="store_true", default=False)
+    parser.add_argument('-r', '--root', dest='root', help='The dirname for devpackage.json')
 
     commands = {}
     subparsers = parser.add_subparsers(dest='command', help='commands')
     for k in commands_dict:
         command = create_command(context, k)
         command.create_parser(subparsers)
         commands[k] = command
@@ -49,14 +50,16 @@
     if options.version:
         sys.stdout.write(parser.version)
         sys.stdout.write(os.linesep)
         sys.exit()
     if not options.command:
         parser.print_help()
         sys.exit(1)
+    if options.root:
+        context.cwd = options.root
     command = commands[options.command]
     command.options = options
     command_args = sys.argv[1:]
     command.parse_args(command_args)
     commands[options.command].main(command_args)
```

### Comparing `devpm-1.1.0/devpm/_internal/commands/__init__.py` & `devpm-1.1.1/devpm/_internal/commands/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     "run": CommandInfo("Run [NAME] script in devpackage.json."),
     "lint": CommandInfo("Run lint script in devpackage.json."),
     "test": CommandInfo("Run test script in devpackage.json."),
     "start": CommandInfo("Run start script in devpackage.json."),
     "stop": CommandInfo("Run stop script in devpackage.json."),
     "restart": CommandInfo("Run restart script in devpackage.json."),
     "version": CommandInfo("Bump a package version and auto-gen CHANGELOG."),
+    "githook": CommandInfo("Run git hook."),
 }
 
 
 def create_command(context: Context, name: str, **kwargs: Any) -> Command:
     """
     Create an instance of the Command class with the given name.
     """
```

### Comparing `devpm-1.1.0/devpm/_internal/commands/base_run.py` & `devpm-1.1.1/devpm/_internal/commands/base_run.py`

 * *Files identical despite different names*

### Comparing `devpm-1.1.0/devpm/_internal/commands/install.py` & `devpm-1.1.1/devpm/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `devpm-1.1.0/devpm/_internal/commands/run.py` & `devpm-1.1.1/devpm/_internal/commands/run.py`

 * *Files identical despite different names*

### Comparing `devpm-1.1.0/devpm/_internal/commands/version.py` & `devpm-1.1.1/devpm/_internal/commands/version.py`

 * *Files identical despite different names*

### Comparing `devpm-1.1.0/devpm/_internal/utils/bash.py` & `devpm-1.1.1/devpm/_internal/utils/bash.py`

 * *Files identical despite different names*

### Comparing `devpm-1.1.0/devpm/_internal/utils/bin.py` & `devpm-1.1.1/devpm/_internal/utils/bin.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,29 +40,29 @@
         if not self.name:
             self.abort()
         if self.err:
             self.abort()
         args = self.version_args
         args.insert(0, self.name)
         try:
-            self.version = subprocess.check_output(args).decode('utf-8')
+            self.version = subprocess.check_output(args, shell=self.shell).decode('utf-8')
             self.err = self.verify_version(self.version)
             if self.err:
                 self.abort()
             self.bin = self.name
         except:
             for path in self.search_paths:
                 if os.path.exists(path):
                     self.bin = path
             if not self.bin:
                 self.err = 'command not found'
             else:
                 args = self.version_args
                 args.insert(0, self.bin)
-                self.version = subprocess.check_output(args).decode('utf-8')
+                self.version = subprocess.check_output(args, shell=self.shell).decode('utf-8')
             self.abort()
 
     def run(self, args, cwd=None, echo_only=False) -> str | None:
         self.check_bin()
         args.insert(0, self.bin)
         try:
             if echo_only:
```

### Comparing `devpm-1.1.0/devpm/_internal/utils/code.py` & `devpm-1.1.1/devpm/_internal/utils/code.py`

 * *Files identical despite different names*

### Comparing `devpm-1.1.0/devpm/_internal/utils/context.py` & `devpm-1.1.1/devpm/_internal/utils/context.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # This software is distributed under the MIT license.
 
 # System context manager
 
 import json
 import os
 import subprocess
+import sys
 from devpm._internal.utils.git import Git
 from devpm._internal.utils.bash import Bash
 from devpm._internal.utils.log import Log
 from devpm._internal.utils.code import Code
 from devpm._internal.utils.pip import Pip
 
 
@@ -23,21 +24,31 @@
         self.log = Log()
         self.code = Code()
         self.pip = Pip()
         self.bash = Bash()
         self.git = Git()
 
     def load_config(self) -> dict:
-        config_file = os.path.join(self.cwd, 'devpackage.json')
-        if not os.path.exists(config_file):
-            print('devpackage.json no found.')
-            exit(1)
         config = {}
-        with open(config_file, 'r', encoding='utf-8') as file:
-            config = json.load(file)
+        if not sys.stdin.isatty():
+            # Read from stdin
+            s = ''
+            for line in sys.stdin:
+                s += line.strip()
+            try:
+                config = json.loads(s)
+            except:
+                self.log.abort('Invalid config data')
+        else:
+            # Read from file
+            config_file = os.path.join(self.cwd, 'devpackage.json')
+            if not os.path.exists(config_file):
+                self.log.abort('devpackage.json no found.')
+            with open(config_file, 'r', encoding='utf-8') as file:
+                config = json.load(file)
         return config
 
     def check_install_exe(self, exe, url):
         installed_ver = None
         args = [exe, '-h']
         try:
             p = subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
```

### Comparing `devpm-1.1.0/devpm/_internal/utils/git.py` & `devpm-1.1.1/devpm/_internal/utils/git.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,28 +58,21 @@
         self.make_exec(script_file)
         return 'dev_modules/git-hooks/%s' % name
     
     def append_hook(self, root_path, git_path, name, hook, apply_submodules):
         t = hook['type'] if 'type' in hook else None
         if not t:
             return
-        available_types = ['exec', 'regexp', 'pre-commit']
+        available_types = ['regexp', 'pre-commit']
         if not t in available_types:
             return
-        
+
         modules = self.get_modules(root_path)
-        if t == 'exec':
-            self.append_hook_script(modules, name, hook['bin'])
-        elif t == 'regexp':
-            # write git-hook file
-            if not 'pattern' in hook or not 'tips' in hook:
-                print('    pattern, tips required for regexp mode.')
-                return
-            script_bin = self.create_regexp_hook_script(root_path, name, hook['pattern'], hook['tips'])
-            return self.append_hook_script(modules, name, script_bin)
+        if t == 'regexp':
+            self.append_hook_script(modules, name)
         elif t == 'pre-commit':
             self.install_pre_commit(modules, hook['repos'], root_path)
 
     def make_exec(self, file):
         st = os.stat(file)
         mode = st.st_mode & stat.S_IEXEC
         if mode == 0:
@@ -101,58 +94,44 @@
                         host,
                         os.path.join(host, sub),
                         os.path.join(git_path, 'modules', sub),
                         os.path.relpath('.', sub).replace('\\', '/'),
                         True))
         return modules
 
-    def append_hook_script(self, modules, name, script_file):
-        hook_enabled = len(script_file) > 0
-        if hook_enabled:
-            if not os.path.exists(script_file):
-                print('script file not exists: %s' % script_file)
-                return
-        self.make_exec(script_file)
+    def append_hook_script(self, modules, name):
         for module in modules:
             hook_path = os.path.join(module.git_path, 'hooks')
-            self.append_hook_script_sub(hook_enabled, module.host_root_path, hook_path, name, module.rel_path + '/' + script_file)
+            self.append_hook_script_sub(module.host_root_path, hook_path, name, module.rel_path)
 
-    def append_hook_script_sub(self, hook_enabled, host, hook_path, name, bin):
-        exec = 'DEVPME=exec;$DEVPME'
-        script = '%s %s $1' % (exec, bin)
+    def append_hook_script_sub(self, host, hook_path, name, root):
+        devpm = 'exec devpm'
+        script = f'cat {root}/devpackage.json | {devpm} githook {name} "$@"'
         if os.path.exists(hook_path):
             hook_file = os.path.join(hook_path, name)
             new_file_content = None
             if not os.path.exists(hook_file):
-                if hook_enabled:
-                    new_file_content = '#!/bin/bash\n\n# Auto-generated by devpm.\n' + script + '\n'
+                new_file_content = '#!/bin/bash\n\n# Auto-generated by devpm.\n' + script + '\n'
             else:
                 with open(hook_file, 'r', encoding='utf-8') as f:
                     needs_update = False
                     file_content = ''
-                    found = False
+                    added = False
                     for line in f.readlines():
-                        index = line.find(exec)
+                        index = line.find(devpm)
                         if index < 0:
                             file_content += line
                         else:
-                            found = True
-                            hook_added = not '#' in line[:index]
-                            if hook_added == hook_enabled:
-                                if not hook_enabled or script == line.strip():
-                                    break
-                                needs_update = True
+                            if not added:
+                                added = True
+                                needs_update = line.strip() != script
                                 file_content += script + '\n'
                             else:
-                                needs_update = True
-                                if hook_enabled:
-                                    file_content += script + '\n'
-                                else:
-                                    file_content += '# ' + line
-                    if not found and hook_enabled:
+                                needs_update = True  # Remove old scripts
+                    if not added:
                         needs_update = True
                         file_content += script + '\n'
                     if needs_update:
                         new_file_content = file_content
             result = '%s installed at %s' % (name, os.path.relpath(hook_file, host))
             if new_file_content:
                 with open(hook_file, 'w', encoding='utf-8') as f:
```

### Comparing `devpm-1.1.0/devpm/_internal/utils/log.py` & `devpm-1.1.1/devpm/_internal/utils/log.py`

 * *Files identical despite different names*

### Comparing `devpm-1.1.0/devpm/_internal/utils/pip.py` & `devpm-1.1.1/devpm/_internal/utils/pip.py`

 * *Files identical despite different names*

### Comparing `devpm-1.1.0/.gitignore` & `devpm-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `devpm-1.1.0/LICENSE` & `devpm-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `devpm-1.1.0/README.md` & `devpm-1.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -61,17 +61,18 @@
 ### Example
 
 ```json
 {
   "$schema": "https://raw.githubusercontent.com/wequick/devpm/main/devpackage.schema.json",
   "vscodeDependencies": {
     "ms-vscode.cpptools-extension-pack": "",
-    "wequick.cpp-creator": "",
+    "wequick.filegen": "",
     "wequick.coverage-gutters": "",
-    "mine.cpplint": ""
+    "mine.cpplint": "",
+    "ms-python.pylint": ""
   },
   "vscodeUserSettings": {
     "cpplint.cpplintPath": "$pip.which:cpplint",
     "cmake.cmakePath": "$bash.which:cmake"
   },
   "pythonDependencies": {
     "gcovr": "4.2",
@@ -87,15 +88,18 @@
       "linux": "apt-get install cppcheck",
       "darwin": "brew install cppcheck"
     }
   },
   "gitHooks": {
     "commit-msg": {
       "type": "regexp",
-      "pattern": "^[feat|fix|refactor|chore|test|style|docs]",
+      "pattern": [
+        "^(feat|fix|refactor|chore|test|style|docs)",
+        "^(Merge)"
+      ],
       "tips": [
         "Invalid commit message style, please format as following:",
         "  fix: some msg",
         "  ^^^^              Type: feat|fix|refactor|chore|test|style|docs",
         "       ^^^^^^^^     Summary in present tense",
         "Type:",
         "  feat     : new feature for the user, not a new feature for build script",
@@ -114,19 +118,33 @@
       "type": "pre-commit",
       "repos": [
         {
           "repo": "https://github.com/pocc/pre-commit-hooks",
           "rev": "v1.3.5",
           "hooks": [
             { "id": "cpplint" },
-            { "id": "cppcheck" }
+            {
+              "id": "cppcheck",
+              "args": [
+                "--suppress=missingInclude",
+                "--suppress=missingIncludeSystem",
+                "--std=c++14",
+                "--force"
+              ]
+            }
           ]
         }
       ]
     }
+  },
+  "scripts": {
+    "prestart": "echo prestart",
+    "start": "echo prestart",
+    "poststart": "echo poststart",
+    "version": "devpm --version"
   }
 }
 ```
 
 ## Develop
 
 ```bash
```

### Comparing `devpm-1.1.0/pyproject.toml` & `devpm-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.hatch.build]
 sources = ["src"]
 directory = "devpm"
 include = ["**/*.py", "devpackage.schema.json"]
 
 [project]
 name = "devpm"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Galen Lin", email="oolgloo.2012@gmail.com" },
 ]
 description = "Development package manager"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `devpm-1.1.0/PKG-INFO` & `devpm-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpm
-Version: 1.1.0
+Version: 1.1.1
 Summary: Development package manager
 Project-URL: Homepage, https://github.com/wequick/devpm
 Project-URL: Bug Tracker, https://github.com/wequick/devpm/issues
 Author-email: Galen Lin <oolgloo.2012@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -75,17 +75,18 @@
 ### Example
 
 ```json
 {
   "$schema": "https://raw.githubusercontent.com/wequick/devpm/main/devpackage.schema.json",
   "vscodeDependencies": {
     "ms-vscode.cpptools-extension-pack": "",
-    "wequick.cpp-creator": "",
+    "wequick.filegen": "",
     "wequick.coverage-gutters": "",
-    "mine.cpplint": ""
+    "mine.cpplint": "",
+    "ms-python.pylint": ""
   },
   "vscodeUserSettings": {
     "cpplint.cpplintPath": "$pip.which:cpplint",
     "cmake.cmakePath": "$bash.which:cmake"
   },
   "pythonDependencies": {
     "gcovr": "4.2",
@@ -101,15 +102,18 @@
       "linux": "apt-get install cppcheck",
       "darwin": "brew install cppcheck"
     }
   },
   "gitHooks": {
     "commit-msg": {
       "type": "regexp",
-      "pattern": "^[feat|fix|refactor|chore|test|style|docs]",
+      "pattern": [
+        "^(feat|fix|refactor|chore|test|style|docs)",
+        "^(Merge)"
+      ],
       "tips": [
         "Invalid commit message style, please format as following:",
         "  fix: some msg",
         "  ^^^^              Type: feat|fix|refactor|chore|test|style|docs",
         "       ^^^^^^^^     Summary in present tense",
         "Type:",
         "  feat     : new feature for the user, not a new feature for build script",
@@ -128,19 +132,33 @@
       "type": "pre-commit",
       "repos": [
         {
           "repo": "https://github.com/pocc/pre-commit-hooks",
           "rev": "v1.3.5",
           "hooks": [
             { "id": "cpplint" },
-            { "id": "cppcheck" }
+            {
+              "id": "cppcheck",
+              "args": [
+                "--suppress=missingInclude",
+                "--suppress=missingIncludeSystem",
+                "--std=c++14",
+                "--force"
+              ]
+            }
           ]
         }
       ]
     }
+  },
+  "scripts": {
+    "prestart": "echo prestart",
+    "start": "echo prestart",
+    "poststart": "echo poststart",
+    "version": "devpm --version"
   }
 }
 ```
 
 ## Develop
 
 ```bash
```

