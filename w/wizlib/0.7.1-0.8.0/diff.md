# Comparing `tmp/wizlib-0.7.1.tar.gz` & `tmp/wizlib-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizlib-0.7.1.tar", last modified: Fri Jul 21 04:48:40 2023, max compression
+gzip compressed data, was "wizlib-0.8.0.tar", last modified: Sat Jul 22 20:27:24 2023, max compression
```

## Comparing `wizlib-0.7.1.tar` & `wizlib-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:48:40.650342 wizlib-0.7.1/
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-21 04:47:50.000000 wizlib-0.7.1/.version
--rw-r--r--   0 root         (0) root         (0)     5115 2023-07-21 04:48:40.650342 wizlib-0.7.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4850 2023-07-21 04:48:32.000000 wizlib-0.7.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-07-21 04:48:32.000000 wizlib-0.7.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 04:48:40.651342 wizlib-0.7.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:48:40.648342 wizlib-0.7.1/test/
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-21 04:48:32.000000 wizlib-0.7.1/test/test_class_family.py
--rw-rw-rw-   0 root         (0) root         (0)     2366 2023-07-21 04:48:32.000000 wizlib-0.7.1/test/test_config_machine.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-07-21 04:48:32.000000 wizlib-0.7.1/test/test_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2023-07-21 04:48:32.000000 wizlib-0.7.1/test/test_super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:48:40.649342 wizlib-0.7.1/wizlib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-21 04:48:32.000000 wizlib-0.7.1/wizlib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4413 2023-07-21 04:48:32.000000 wizlib-0.7.1/wizlib/class_family.py
--rw-rw-rw-   0 root         (0) root         (0)     2168 2023-07-21 04:48:32.000000 wizlib-0.7.1/wizlib/command_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1601 2023-07-21 04:48:32.000000 wizlib-0.7.1/wizlib/config_machine.py
--rw-rw-rw-   0 root         (0) root         (0)     1754 2023-07-21 04:48:32.000000 wizlib-0.7.1/wizlib/rlinput.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-07-21 04:48:32.000000 wizlib-0.7.1/wizlib/super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 04:48:40.650342 wizlib-0.7.1/wizlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5115 2023-07-21 04:48:40.000000 wizlib-0.7.1/wizlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2023-07-21 04:48:40.000000 wizlib-0.7.1/wizlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 04:48:40.000000 wizlib-0.7.1/wizlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-21 04:48:40.000000 wizlib-0.7.1/wizlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-21 04:48:40.000000 wizlib-0.7.1/wizlib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:27:24.346964 wizlib-0.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-22 20:26:33.000000 wizlib-0.8.0/.version
+-rw-r--r--   0 root         (0) root         (0)     5384 2023-07-22 20:27:24.346964 wizlib-0.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5119 2023-07-22 20:27:15.000000 wizlib-0.8.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-07-22 20:27:15.000000 wizlib-0.8.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-22 20:27:24.346964 wizlib-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:27:24.345964 wizlib-0.8.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-22 20:27:15.000000 wizlib-0.8.0/test/test_class_family.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-22 20:27:15.000000 wizlib-0.8.0/test/test_command_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     3010 2023-07-22 20:27:15.000000 wizlib-0.8.0/test/test_config_machine.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-07-22 20:27:15.000000 wizlib-0.8.0/test/test_super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:27:24.345964 wizlib-0.8.0/wizlib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-22 20:27:15.000000 wizlib-0.8.0/wizlib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4413 2023-07-22 20:27:15.000000 wizlib-0.8.0/wizlib/class_family.py
+-rw-rw-rw-   0 root         (0) root         (0)     2764 2023-07-22 20:27:15.000000 wizlib-0.8.0/wizlib/command_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2023-07-22 20:27:15.000000 wizlib-0.8.0/wizlib/config_machine.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2023-07-22 20:27:15.000000 wizlib-0.8.0/wizlib/rlinput.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-07-22 20:27:15.000000 wizlib-0.8.0/wizlib/super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:27:24.346964 wizlib-0.8.0/wizlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5384 2023-07-22 20:27:24.000000 wizlib-0.8.0/wizlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      427 2023-07-22 20:27:24.000000 wizlib-0.8.0/wizlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-22 20:27:24.000000 wizlib-0.8.0/wizlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-22 20:27:24.000000 wizlib-0.8.0/wizlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-22 20:27:24.000000 wizlib-0.8.0/wizlib.egg-info/top_level.txt
```

### Comparing `wizlib-0.7.1/PKG-INFO` & `wizlib-0.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: wizlib
-Version: 0.7.1
-Summary: A collection of Python modules that are useful across multiple projects
-Author-email: Francis Potter <wizlib@steampunkwizard.ca>
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # WizLib
 
 A collection of Python modules that might be useful across multiple projects
 
 ## ClassFamily
 
 A class family is a set of class definitions that use single inheritance
@@ -67,14 +58,17 @@
     def execute(self, name):
         print(f"Hello {name}")
 
 c = NewChild()
 c.execute("Jane")
 ```
 
+Note that for a method to be "wrappable" it must take the form shown above, and explicitly call the method that's handed into it. So strictly, this is different from regular inheritance, where the parent class method has the same signature as the child class method.
+
+
 ## CommandHandler
 
 ## ConfigMachine
 
 Enables easy configuration across multiple levels. Tries each of the following approaches in order until one finds the required config option
 
 - First look for specific options (ie. `--gitlab-host`) on the command line, typically hyphenated
```

### Comparing `wizlib-0.7.1/README.md` & `wizlib-0.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: wizlib
+Version: 0.8.0
+Summary: A collection of Python modules that are useful across multiple projects
+Author-email: Francis Potter <wizlib@steampunkwizard.ca>
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 # WizLib
 
 A collection of Python modules that might be useful across multiple projects
 
 ## ClassFamily
 
 A class family is a set of class definitions that use single inheritance
@@ -58,14 +67,17 @@
     def execute(self, name):
         print(f"Hello {name}")
 
 c = NewChild()
 c.execute("Jane")
 ```
 
+Note that for a method to be "wrappable" it must take the form shown above, and explicitly call the method that's handed into it. So strictly, this is different from regular inheritance, where the parent class method has the same signature as the child class method.
+
+
 ## CommandHandler
 
 ## ConfigMachine
 
 Enables easy configuration across multiple levels. Tries each of the following approaches in order until one finds the required config option
 
 - First look for specific options (ie. `--gitlab-host`) on the command line, typically hyphenated
```

### Comparing `wizlib-0.7.1/pyproject.toml` & `wizlib-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wizlib-0.7.1/test/test_super_wrapper.py` & `wizlib-0.8.0/test/test_super_wrapper.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.7.1/wizlib/class_family.py` & `wizlib-0.8.0/wizlib/class_family.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.7.1/wizlib/command_handler.py` & `wizlib-0.8.0/wizlib/command_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,78 @@
-from argparse import ArgumentParser
 import sys
+from argparse import ArgumentError, ArgumentParser
 from dataclasses import dataclass
 
 from wizlib.class_family import ClassFamily
 from wizlib.super_wrapper import SuperWrapper
 
 
 class CommandHandler:
     """Handle commands from a ClassFamily"""
 
     def __init__(self, atriarch):
         """Pass in the command base class, the atriarch of a
         classfamily that meeting the CommandHandler spec"""
-        self.parser = ArgumentParser(prog=atriarch.app_name)
+        self.parser = ArgumentParser(prog=atriarch.app_name,
+                                     exit_on_error=False)
+        atriarch.add_app_args(self.parser)
         subparsers = self.parser.add_subparsers(dest='command')
         for command in atriarch.family_members('name'):
             key = command.get_member_attr('key')
             aliases = [key] if key else []
             subparser = subparsers.add_parser(command.name, aliases=aliases)
-            command.add_arg_spec(subparser)
+            command.add_args(subparser)
         self.atriarch = atriarch
 
-    def handle(self, args=None):
+    def get_command(self, args=None):
         args = args if args else [self.atriarch.default]
-        values = vars(self.parser.parse_args(args))
+        try:
+            values = vars(self.parser.parse_args(args))
+        except ArgumentError as error:
+            print(error.message)
+            return
+        except SystemExit:
+            return
         command = values.pop('command')
         command_class = self.atriarch.family_member('name', command)
         if not command_class:
             raise Exception(f"Unknown command {command}")
-        command = command_class(**values)
-        result = command.execute()
-        return result, command.status
+        return command_class(**values)
+
+    def handle(self, args=None):
+        command = self.get_command(args)
+        if command:
+            result = command.execute()
+            return result, command.status
+        else:
+            return None, None
 
     @classmethod
     def shell(cls, atriarch):
         """Call this from a shell/main entrypoint"""
         result, status = cls(atriarch).handle(sys.argv[1:])
         if result:
             print(result)
         if status:
             print(status)
 
 
 @dataclass
-class Atriarch(ClassFamily, SuperWrapper):
+class Command(ClassFamily, SuperWrapper):
 
     status = ''
 
     @classmethod
-    def add_arg_spec(self, parser):
+    def add_app_args(self, parser):
+        """Add pre-subcommand arguments via argparse by optionally overriding -
+        only works in the atricarch"""
+        pass
+
+    @classmethod
+    def add_args(self, parser):
         """Add arguments to the command's parser - override this.
         Add global arguments in the base class. Not wrapped."""
         pass
 
     def handle_args(self):
         """Clean up args, calculate any, ask through UI, etc. - override
         this"""
```

### Comparing `wizlib-0.7.1/wizlib/rlinput.py` & `wizlib-0.8.0/wizlib/rlinput.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.7.1/wizlib.egg-info/PKG-INFO` & `wizlib-0.8.0/wizlib.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 0.7.1
+Version: 0.8.0
 Summary: A collection of Python modules that are useful across multiple projects
 Author-email: Francis Potter <wizlib@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WizLib
@@ -67,14 +67,17 @@
     def execute(self, name):
         print(f"Hello {name}")
 
 c = NewChild()
 c.execute("Jane")
 ```
 
+Note that for a method to be "wrappable" it must take the form shown above, and explicitly call the method that's handed into it. So strictly, this is different from regular inheritance, where the parent class method has the same signature as the child class method.
+
+
 ## CommandHandler
 
 ## ConfigMachine
 
 Enables easy configuration across multiple levels. Tries each of the following approaches in order until one finds the required config option
 
 - First look for specific options (ie. `--gitlab-host`) on the command line, typically hyphenated
```

