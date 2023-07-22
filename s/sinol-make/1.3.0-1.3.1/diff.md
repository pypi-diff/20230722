# Comparing `tmp/sinol-make-1.3.0.tar.gz` & `tmp/sinol-make-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinol-make-1.3.0.tar", last modified: Thu Jul  6 15:36:21 2023, max compression
+gzip compressed data, was "sinol-make-1.3.1.tar", last modified: Sat Jul 22 14:36:50 2023, max compression
```

## Comparing `sinol-make-1.3.0.tar` & `sinol-make-1.3.1.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:36:21.083261 sinol-make-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-06 15:36:10.000000 sinol-make-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-06 15:36:21.083261 sinol-make-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-06 15:36:10.000000 sinol-make-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-06 15:36:10.000000 sinol-make-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 15:36:21.083261 sinol-make-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:36:21.079261 sinol-make-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:36:21.083261 sinol-make-1.3.0/src/sinol_make/
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-06 15:36:10.000000 sinol-make-1.3.0/src/sinol_make/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:36:21.079261 sinol-make-1.3.0/src/sinol_make/commands/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:36:21.083261 sinol-make-1.3.0/src/sinol_make/commands/inwer/
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-06 15:36:10.000000 sinol-make-1.3.0/src/sinol_make/commands/inwer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-06 15:36:10.000000 sinol-make-1.3.0/src/sinol_make/commands/inwer/inwer_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-06 15:36:10.000000 sinol-make-1.3.0/src/sinol_make/commands/inwer/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:36:21.083261 sinol-make-1.3.0/src/sinol_make/commands/run/
--rw-r--r--   0 runner    (1001) docker     (123)    45204 2023-07-06 15:36:10.000000 sinol-make-1.3.0/src/sinol_make/commands/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-06 15:36:10.000000 sinol-make-1.3.0/src/sinol_make/commands/run/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:36:21.083261 sinol-make-1.3.0/src/sinol_make/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:36:10.000000 sinol-make-1.3.0/src/sinol_make/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-06 15:36:10.000000 sinol-make-1.3.0/src/sinol_make/helpers/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-06 15:36:10.000000 sinol-make-1.3.0/src/sinol_make/helpers/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-06 15:36:10.000000 sinol-make-1.3.0/src/sinol_make/helpers/package_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-06 15:36:10.000000 sinol-make-1.3.0/src/sinol_make/helpers/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:36:21.083261 sinol-make-1.3.0/src/sinol_make/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-06 15:36:10.000000 sinol-make-1.3.0/src/sinol_make/interfaces/BaseCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-06 15:36:10.000000 sinol-make-1.3.0/src/sinol_make/interfaces/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 15:36:10.000000 sinol-make-1.3.0/src/sinol_make/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:36:21.083261 sinol-make-1.3.0/src/sinol_make/structs/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-06 15:36:10.000000 sinol-make-1.3.0/src/sinol_make/structs/compiler_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-07-06 15:36:10.000000 sinol-make-1.3.0/src/sinol_make/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:36:21.083261 sinol-make-1.3.0/src/sinol_make.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-06 15:36:21.000000 sinol-make-1.3.0/src/sinol_make.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-06 15:36:21.000000 sinol-make-1.3.0/src/sinol_make.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 15:36:21.000000 sinol-make-1.3.0/src/sinol_make.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-06 15:36:21.000000 sinol-make-1.3.0/src/sinol_make.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-06 15:36:21.000000 sinol-make-1.3.0/src/sinol_make.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 15:36:21.000000 sinol-make-1.3.0/src/sinol_make.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 15:36:21.083261 sinol-make-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-06 15:36:10.000000 sinol-make-1.3.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.028787 sinol-make-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-22 14:36:38.000000 sinol-make-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-22 14:36:50.028787 sinol-make-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-22 14:36:38.000000 sinol-make-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-22 14:36:38.000000 sinol-make-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 14:36:50.028787 sinol-make-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.024787 sinol-make-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.024787 sinol-make-1.3.1/src/sinol_make/
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.024787 sinol-make-1.3.1/src/sinol_make/commands/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.028787 sinol-make-1.3.1/src/sinol_make/commands/inwer/
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/commands/inwer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/commands/inwer/inwer_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/commands/inwer/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.028787 sinol-make-1.3.1/src/sinol_make/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (123)    46165 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/commands/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/commands/run/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.028787 sinol-make-1.3.1/src/sinol_make/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/helpers/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/helpers/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/helpers/package_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/helpers/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/helpers/printer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.028787 sinol-make-1.3.1/src/sinol_make/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/interfaces/BaseCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/interfaces/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.028787 sinol-make-1.3.1/src/sinol_make/structs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/structs/compiler_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-22 14:36:38.000000 sinol-make-1.3.1/src/sinol_make/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.024787 sinol-make-1.3.1/src/sinol_make.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-22 14:36:50.000000 sinol-make-1.3.1/src/sinol_make.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-22 14:36:50.000000 sinol-make-1.3.1/src/sinol_make.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 14:36:50.000000 sinol-make-1.3.1/src/sinol_make.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-22 14:36:50.000000 sinol-make-1.3.1/src/sinol_make.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-22 14:36:50.000000 sinol-make-1.3.1/src/sinol_make.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-22 14:36:50.000000 sinol-make-1.3.1/src/sinol_make.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:36:50.028787 sinol-make-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-22 14:36:38.000000 sinol-make-1.3.1/tests/test_util.py
```

### Comparing `sinol-make-1.3.0/LICENSE` & `sinol-make-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sinol-make-1.3.0/PKG-INFO` & `sinol-make-1.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinol-make
-Version: 1.3.0
+Version: 1.3.1
 Summary: CLI tool for creating sio2 task packages
 Author-email: Mateusz Masiarz <m.masiarz@fri.edu.pl>
 Maintainer-email: Tomasz Nowak <tomasz.nowak@tonowak.com>
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -55,17 +55,26 @@
 ```
 
 As `oiejq` works only on Linux-based operating systems,
 *we do not recommend* using operating systems such as Windows or macOS.
 Nevertheless `sinol-make` supports those operating systems,
 though there are additional installation steps required to use
 other tools for measuring time (which are non-deterministic and produce reports different from sio2):
-- Windows (WSL): `apt install time timeout`
+- Windows (WSL): `apt install time`
 - macOS: `brew install gnu-time coreutils`
 
+### Autocompletion (optional)
+
+If you would like to have autocompletion for `sinol-make` commands,
+run the following command and refresh the shell (e.g. by opening a new terminal):
+
+```shell
+activate-global-python-argcomplete
+```
+
 ### Usage
 
 The availabe commands (see `sinol-make --help`) are:
 
 - `sinol-make run` -- Runs selected solutions (by default all solutions) on selected tests (by default all tests) with a given number
 of CPUs. Measures the solutions' time with oiejq, unless specified otherwise. After running the solutions, it
 compares the solutions' scores with the ones saved in config.yml.
```

### Comparing `sinol-make-1.3.0/README.md` & `sinol-make-1.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -39,17 +39,26 @@
 ```
 
 As `oiejq` works only on Linux-based operating systems,
 *we do not recommend* using operating systems such as Windows or macOS.
 Nevertheless `sinol-make` supports those operating systems,
 though there are additional installation steps required to use
 other tools for measuring time (which are non-deterministic and produce reports different from sio2):
-- Windows (WSL): `apt install time timeout`
+- Windows (WSL): `apt install time`
 - macOS: `brew install gnu-time coreutils`
 
+### Autocompletion (optional)
+
+If you would like to have autocompletion for `sinol-make` commands,
+run the following command and refresh the shell (e.g. by opening a new terminal):
+
+```shell
+activate-global-python-argcomplete
+```
+
 ### Usage
 
 The availabe commands (see `sinol-make --help`) are:
 
 - `sinol-make run` -- Runs selected solutions (by default all solutions) on selected tests (by default all tests) with a given number
 of CPUs. Measures the solutions' time with oiejq, unless specified otherwise. After running the solutions, it
 compares the solutions' scores with the ones saved in config.yml.
```

### Comparing `sinol-make-1.3.0/pyproject.toml` & `sinol-make-1.3.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -2,39 +2,40 @@
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sinol-make"
 dynamic = ["version"]
 authors = [
-  { name="Mateusz Masiarz", email="m.masiarz@fri.edu.pl" }
+    { name="Mateusz Masiarz", email="m.masiarz@fri.edu.pl" }
 ]
 maintainers = [
-  { name="Tomasz Nowak", email="tomasz.nowak@tonowak.com" }
+    { name="Tomasz Nowak", email="tomasz.nowak@tonowak.com" }
 ]
 description = "CLI tool for creating sio2 task packages"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-	"argparse",
-	"requests",
-	"PyYAML",
-	"dictdiffer"
+    "argparse",
+    "argcomplete",
+    "requests",
+    "PyYAML",
+    "dictdiffer"
 ]
 
 [project.optional-dependencies]
 tests = [
-  "pytest",
-  "pytest-cov",
-  "requests-mock",
+    "pytest",
+    "pytest-cov",
+    "requests-mock",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/sio2project/sinol-make"
 "Bug Tracker" = "https://github.com/sio2project/sinol-make/issues"
 
 [project.scripts]
```

### Comparing `sinol-make-1.3.0/src/sinol_make/__init__.py` & `sinol-make-1.3.1/src/sinol_make/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+# PYTHON_ARCOMPLETE_OK
+
+import argcomplete
 import argparse
 import sys
 
 from sinol_make import util
 
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 def configure_parsers():
     parser = argparse.ArgumentParser(
         prog='sinol-make',
         description='Tool for creating and testing sio2 tasks',
     )
     parser.add_argument("-v", "--version", action="version", version="%(prog)s " + __version__)
@@ -18,21 +21,23 @@
     )
     subparsers.required = False
 
     commands = util.get_commands()
 
     for command in commands:
         command.configure_subparser(subparsers)
+
+    argcomplete.autocomplete(parser)
     return parser
 
 
 def main():
     parser = configure_parsers()
-    commands = util.get_commands()
     args = parser.parse_args()
+    commands = util.get_commands()
 
     for command in commands:
         if command.get_name() == args.command:
             new_version = util.check_for_updates(__version__)
             if new_version is not None:
                 print(util.warning(f'New version of sinol-make is available (your version: {__version__}, available version: {new_version}).\n'
                                    f' You can update it by running `pip3 install sinol-make --upgrade`.'))
@@ -43,15 +48,15 @@
                 try:
                     if util.install_oiejq():
                         print(util.info('`oiejq` was successfully installed.'))
                     else:
                         util.exit_with_error('`oiejq` could not be installed.\n'
                                              'You can download it from https://oij.edu.pl/zawodnik/srodowisko/oiejq.tar.gz'
                                              ', unpack it to `~/.local/bin/` and rename oiejq.sh to oiejq.\n'
-                                             'You can also use --oiejq_path to specify path to your oiejq.')
+                                             'You can also use --oiejq-path to specify path to your oiejq.')
                 except Exception as err:
                     util.exit_with_error('`oiejq` could not be installed.\n' + err)
 
             command.run(args)
             exit(0)
 
     parser.print_help()
```

### Comparing `sinol-make-1.3.0/src/sinol_make/commands/inwer/__init__.py` & `sinol-make-1.3.1/src/sinol_make/commands/inwer/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import subprocess
+import sys
+import signal
+import threading
 import argparse
 import os
 import multiprocessing as mp
 
 from sinol_make import util
 from sinol_make.commands.inwer.structs import TestResult, InwerExecution, VerificationResult, TableData
-from sinol_make.helpers import package_util, compile
+from sinol_make.helpers import package_util, compile, printer
 from sinol_make.helpers.parsers import add_compilation_arguments
 from sinol_make.interfaces.BaseCommand import BaseCommand
 from sinol_make.commands.inwer import inwer_util
 
 
 class Command(BaseCommand):
     """
@@ -26,22 +29,22 @@
             description='Verify if input files are correct using inwer program '
                         '(for example prog/abcinwer.cpp for abc task). You can also '
                         'specify your inwer source file which will be used.'
         )
 
         parser.add_argument('inwer_path', type=str, nargs='?',
                             help='path to inwer source file, for example prog/abcinwer.cpp')
-        parser.add_argument('--tests', type=str, nargs='+',
+        parser.add_argument('-t', '--tests', type=str, nargs='+',
                             help='test to verify, for example in/abc{0,1}*')
-        parser.add_argument('--cpus', type=int,
+        parser.add_argument('-c', '--cpus', type=int,
                             help=f'number of cpus to use, by default {mp.cpu_count()} (all available)')
         add_compilation_arguments(parser)
 
     def compile_inwer(self, args: argparse.Namespace):
-        self.inwer_executable, compile_log_path = inwer_util.compile_inwer(self.inwer, args)
+        self.inwer_executable, compile_log_path = inwer_util.compile_inwer(self.inwer, args, args.weak_compilation_flags)
         if self.inwer_executable is None:
             print(util.error('Compilation failed.'))
             compile.print_compile_log(compile_log_path)
             exit(1)
         else:
             print(util.info('Compilation successful.'))
 
@@ -51,15 +54,25 @@
         Verifies a test and returns the result of inwer on this test.
         """
         output_dir = os.path.join(os.getcwd(), 'cache', 'executions', execution.test_name)
         os.makedirs(output_dir, exist_ok=True)
 
         command = [execution.inwer_exe_path]
         with open(execution.test_path, 'r') as test:
-            process = subprocess.Popen(command, stdin=test, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+            process = subprocess.Popen(command, stdin=test, stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
+                                       preexec_fn=os.setsid)
+
+            def sigint_handler(signum, frame):
+                try:
+                    os.killpg(os.getpgid(process.pid), signal.SIGTERM)
+                except ProcessLookupError:
+                    pass
+                sys.exit(1)
+            signal.signal(signal.SIGINT, sigint_handler)
+
             process.wait()
         exit_code = process.returncode
         out, _ = process.communicate()
 
         return VerificationResult(
             execution.test_path,
             exit_code == 0,
@@ -70,20 +83,40 @@
         results = {}
         sorted_tests = sorted(self.tests, key=lambda x: x[0])
         executions: list[InwerExecution] = []
         for test in sorted_tests:
             results[test] = TestResult(test)
             executions.append(InwerExecution(test, results[test].test_name, self.inwer_executable))
 
+        has_terminal, terminal_width, terminal_height = util.get_terminal_size()
+
         table_data = TableData(results, 0)
-        print('Verifying tests...\n\n')
-        with mp.Pool(self.cpus) as pool:
-            for i, result in enumerate(pool.imap(self.verify_test, executions)):
-                table_data.results[result.test_path].set_results(result.valid, result.output)
-                inwer_util.print_view(table_data)
+        if has_terminal:
+            run_event = threading.Event()
+            run_event.set()
+            thr = threading.Thread(target=printer.printer_thread, args=(run_event, inwer_util.print_view, table_data))
+            thr.start()
+
+        keyboard_interrupt = False
+        try:
+            with mp.Pool(self.cpus) as pool:
+                for i, result in enumerate(pool.imap(self.verify_test, executions)):
+                    table_data.results[result.test_path].set_results(result.valid, result.output)
+                    table_data.i = i
+        except KeyboardInterrupt:
+            keyboard_interrupt = True
+
+        if has_terminal:
+            run_event.clear()
+            thr.join()
+
+        print("\n".join(inwer_util.print_view(terminal_width, terminal_height, table_data)[0]))
+
+        if keyboard_interrupt:
+            util.exit_with_error('Keyboard interrupt.')
 
         return results
 
     def run(self, args: argparse.Namespace):
         if not util.check_if_project():
             util.exit_with_error('You are not in a project directory (couldn\'t find config.yml in current directory).')
```

### Comparing `sinol-make-1.3.0/src/sinol_make/commands/inwer/structs.py` & `sinol-make-1.3.1/src/sinol_make/commands/inwer/structs.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     """
     Data used for printing table with verification results.
     """
 
     # Dictionary with test path as key and verification result as value.
     results: dict[str, TestResult]
 
-    # Previous vertical height of table, used for moving cursor up.
-    previous_vertical_height: int
+    # Number of executions finished
+    i: int
 
 @dataclass
 class InwerExecution:
     test_path: str
     test_name: str
     inwer_exe_path: str
```

### Comparing `sinol-make-1.3.0/src/sinol_make/commands/run/__init__.py` & `sinol-make-1.3.1/src/sinol_make/commands/run/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,202 @@
 # Modified version of https://sinol3.dasie.mimuw.edu.pl/oij/jury/package/-/blob/master/runner.py
 # Author of the original code: Bartosz Kostka <kostka@oij.edu.pl>
 # Version 0.6 (2021-08-29)
 import subprocess
+import signal
+import threading
+from io import StringIO
 import glob
 
-from sinol_make.commands.run.structs import ExecutionResult, ResultChange, ValidationResult, ExecutionData, PointsChange
+from sinol_make.commands.run.structs import ExecutionResult, ResultChange, ValidationResult, ExecutionData, \
+    PointsChange, PrintData
 from sinol_make.helpers.parsers import add_compilation_arguments
 from sinol_make.interfaces.BaseCommand import BaseCommand
 from sinol_make.interfaces.Errors import CompilationError, CheckerOutputException
-from sinol_make.helpers import compile, compiler, package_util
+from sinol_make.helpers import compile, compiler, package_util, printer
 import sinol_make.util as util
-import yaml, os, collections, sys, re, math, dictdiffer, glob
+import yaml, os, collections, sys, re, math, dictdiffer
 import multiprocessing as mp
 
+
+def color_memory(memory, limit):
+    if memory == -1: return util.color_yellow("")
+    memory_str = "%.1fMB" % (memory / 1024.0)
+    if memory > limit:
+        return util.color_red(memory_str)
+    elif memory > limit / 2.0:
+        return util.color_yellow(memory_str)
+    else:
+        return util.color_green(memory_str)
+
+
+def color_time(time, limit):
+    if time == -1: return util.color_yellow("")
+    time_str = "%.2fs" % (time / 1000.0)
+    if time > limit:
+        return util.color_red(time_str)
+    elif time > limit / 2.0:
+        return util.color_yellow(time_str)
+    else:
+        return util.color_green(time_str)
+
+
+def colorize_status(status):
+    if status == "OK": return util.bold(util.color_green(status))
+    if status == "  " or status == "??": return util.warning(status)
+    return util.error(status)
+
+
+def update_group_status(group_status, new_status):
+    order = ["CE", "TL", "ML", "RE", "WA", "OK"]
+    if order.index(new_status) < order.index(group_status):
+        return new_status
+    return group_status
+
+
+def print_view(term_width, term_height, program_groups_scores, all_results, print_data: PrintData, names, executions,
+               groups, scores, tests, possible_score, time_limit, memory_limit, cpus, hide_memory):
+    width = term_width - 13  # First column has 6 characters, the " | " separator has 3 characters and 4 for margin
+    programs_in_row = width // 13  # Each program has 10 characters and the " | " separator has 3 characters
+
+    previous_stdout = sys.stdout
+    output = StringIO()
+    sys.stdout = output
+
+    program_scores = collections.defaultdict(int)
+    program_times = collections.defaultdict(lambda: -1)
+    program_memory = collections.defaultdict(lambda: -1)
+    time_remaining = (len(executions) - print_data.i - 1) * 2 * time_limit / cpus / 1000.0
+    title = 'Done %4d/%4d. Time remaining (in the worst case): %5d seconds.' \
+            % (print_data.i + 1, len(executions), time_remaining)
+    title = title.center(term_width)
+    margin = "  "
+    for program_ix in range(0, len(names), programs_in_row):
+        program_group = names[program_ix:program_ix + programs_in_row]
+
+        def print_table_end():
+            print("-" * 8, end="-+-")
+            for i in range(len(program_group)):
+                if i != len(program_group) - 1:
+                    print("-" * 10, end="-+-")
+                else:
+                    print("-" * 10, end="-+")
+            print()
+
+        print_table_end()
+
+        print(margin + "groups", end=" | ")
+        for program in program_group:
+            print("%10s" % program, end=" | ")
+        print()
+        print(8 * "-", end=" | ")
+        for program in program_group:
+            print(10 * "-", end=" | ")
+        print()
+        for group in groups:
+            print(margin + "%6s" % group, end=" | ")
+            for program in program_group:
+                results = all_results[program][group]
+                group_status = "OK"
+                min_points = 100
+
+                for test in results:
+                    min_points = min(min_points, results[test].Points)
+                    status = results[test].Status
+                    if getattr(results[test], "Time") is not None:
+                        program_times[program] = max(
+                            program_times[program], results[test].Time)
+                    elif status == "TL":
+                        program_times[program] = 2 * time_limit
+                    if getattr(results[test], "Memory") is not None:
+                        program_memory[program] = max(
+                            program_memory[program], results[test].Memory)
+                    elif status == "ML":
+                        program_memory[program] = 2 * memory_limit
+                    if status == "  ":
+                        group_status = "  "
+                        min_points = 0
+                    else:
+                        group_status = update_group_status(group_status, status)
+
+                points = math.floor(min_points / 100 * scores[group])
+                print("%3s" % util.bold(util.color_green(group_status)) if group_status == "OK" else util.bold(
+                    util.color_red(group_status)),
+                      "%3s/%3s" % (points, scores[group]),
+                      end=" | ")
+                program_scores[program] += scores[group] if group_status == "OK" else 0
+                program_groups_scores[program][group] = {"status": group_status, "points": points}
+            print()
+        print(8 * " ", end=" | ")
+        for program in program_group:
+            print(10 * " ", end=" | ")
+        print()
+        print(margin + "points", end=" | ")
+        for program in program_group:
+            print(util.bold("   %3s/%3s" % (program_scores[program], possible_score)), end=" | ")
+        print()
+        print(margin + "  time", end=" | ")
+        for program in program_group:
+            program_time = program_times[program]
+            print(util.bold(("%20s" % color_time(program_time, time_limit))
+                            if program_time < 2 * time_limit and program_time >= 0
+                            else "   " + 7 * '-'), end=" | ")
+        print()
+        print(margin + "memory", end=" | ")
+        for program in program_group:
+            program_mem = program_memory[program]
+            print(util.bold(("%20s" % color_memory(program_mem, memory_limit))
+                            if program_mem < 2 * memory_limit and program_mem >= 0
+                            else "   " + 7 * '-'), end=" | ")
+        print()
+        print(8*" ", end=" | ")
+        for program in program_group:
+            print(10*" ", end=" | ")
+        print()
+
+        def print_group_seperator():
+            print(8 * "-", end=" | ")
+            for program in program_group:
+                print(10 * "-", end=" | ")
+            print()
+
+        print_group_seperator()
+
+        last_group = None
+        for test in tests:
+            group = package_util.get_group(test)
+            if last_group != group:
+                if last_group is not None:
+                    print_group_seperator()
+                last_group = group
+
+            print(margin + "%6s" % package_util.extract_test_id(test), end=" | ")
+            for program in program_group:
+                result = all_results[program][package_util.get_group(test)][test]
+                status = result.Status
+                if status == "  ": print(10*' ', end=" | ")
+                else:
+                    print("%3s" % colorize_status(status),
+                         ("%17s" % color_time(result.Time, time_limit)) if getattr(result, "Time") is not None else 7*" ", end=" | ")
+            print()
+            if not hide_memory:
+                print(8*" ", end=" | ")
+                for program in program_group:
+                    result = all_results[program][package_util.get_group(test)][test]
+                    print(("%20s" % color_memory(result.Memory, memory_limit)) if getattr(result, "Memory") is not None else 10*" ", end=" | ")
+                print()
+
+        print_table_end()
+        print()
+
+
+    sys.stdout = previous_stdout
+    return output.getvalue().splitlines(), title, "Use arrows to move."
+
+
 class Command(BaseCommand):
     """
     Class for running current task
     """
 
 
     def get_name(self):
@@ -32,79 +212,50 @@
                 with a given number of cpus. \
                 Measures the solutions\' time with oiejq, unless specified otherwise. \
                 After running the solutions, it compares the solutions\' scores with the ones saved in config.yml.'
         )
 
         default_timetool = 'oiejq' if sys.platform == 'linux' else 'time'
 
-        parser.add_argument('--solutions', type=str, nargs='+',
+        parser.add_argument('-s', '--solutions', type=str, nargs='+',
                             help='solutions to be run, for example prog/abc{b,s}*.{cpp,py}')
-        parser.add_argument('--tests', type=str, nargs='+',
+        parser.add_argument('-t', '--tests', type=str, nargs='+',
                             help='tests to be run, for example in/abc{0,1}*')
-        parser.add_argument('--cpus', type=int,
+        parser.add_argument('-c', '--cpus', type=int,
                             help='number of cpus to use, you have %d avaliable' % mp.cpu_count())
         parser.add_argument('--tl', type=float, help='time limit (in s)')
         parser.add_argument('--ml', type=float, help='memory limit (in MB)')
-        parser.add_argument('--hide_memory', dest='hide_memory', action='store_true',
+        parser.add_argument('--hide-memory', dest='hide_memory', action='store_true',
                             help='hide memory usage in report')
-        parser.add_argument('--solutions_report', type=str,
+        parser.add_argument('--solutions-report', dest='solutions_report', type=str,
                             help='file to store report from solution executions (in markdown)')
-        parser.add_argument('--time_tool', choices=['oiejq', 'time'], default=default_timetool,
+        parser.add_argument('-T', '--time-tool', dest='time_tool', choices=['oiejq', 'time'], default=default_timetool,
                             help='tool to measure time and memory usage (default when possible: oiejq)')
-        parser.add_argument('--oiejq_path', type=str,
+        parser.add_argument('--oiejq-path', dest='oiejq_path', type=str,
                             help='path to oiejq executable (default: `~/.local/bin/oiejq`)')
         add_compilation_arguments(parser)
-        parser.add_argument('--weak_compilation_flags', dest='weak_compilation_flags', action='store_true',
-                            help='use weaker compilation flags')
-        parser.add_argument('--apply_suggestions', dest='apply_suggestions', action='store_true',
+        parser.add_argument('-a', '--apply-suggestions', dest='apply_suggestions', action='store_true',
                             help='apply suggestions from expected scores report')
 
-
-    def color_memory(self, memory, limit):
-        if memory == -1: return util.color_yellow("")
-        memory_str = "%.1fMB" % (memory / 1024.0)
-        if memory > limit: return util.color_red(memory_str)
-        elif memory > limit / 2.0: return util.color_yellow(memory_str)
-        else: return util.color_green(memory_str)
-
-
-    def color_time(self, time, limit):
-        if time == -1: return util.color_yellow("")
-        time_str = "%.2fs" % (time / 1000.0)
-        if time > limit: return util.color_red(time_str)
-        elif time > limit / 2.0: return util.color_yellow(time_str)
-        else: return util.color_green(time_str)
-
-
-    def colorize_status(self, status):
-        if status == "OK": return util.bold(util.color_green(status))
-        if status == "  " or status == "??": return util.warning(status)
-        return util.error(status)
-
-
     def parse_time(self, time_str):
         if len(time_str) < 3: return -1
         return int(time_str[:-2])
 
 
     def parse_memory(self, memory_str):
         if len(memory_str) < 3: return -1
         return int(memory_str[:-2])
 
 
-    def extract_test_id(self, test_path):
-        return os.path.split(os.path.splitext(test_path)[0])[1][len(self.ID):]
-
-
     def extract_file_name(self, file_path):
         return os.path.split(file_path)[1]
 
 
     def get_group(self, test_path):
-        return int("".join(filter(str.isdigit, self.extract_test_id(test_path))))
+        return int("".join(filter(str.isdigit, package_util.extract_test_id(test_path))))
 
 
     def get_executable_key(self, executable):
         name = package_util.get_file_name(executable)
         value = [0, 0]
         if name[3] == 's':
             value[0] = 1
@@ -231,41 +382,57 @@
             return correct, 100 if correct else 0
         else:
             open(output_file_path, "w").write("\n".join(output))
             return self.check_output_checker(name, input_file, output_file_path, answer_file_path)
 
 
     def execute_oiejq(self, command, name, result_file_path, input_file_path, output_file_path, answer_file_path,
-                      time_limit, memory_limit):
+                      time_limit, memory_limit, hard_time_limit):
         env = os.environ.copy()
         env["MEM_LIMIT"] = f'{memory_limit}K'
         env["MEASURE_MEM"] = "1"
+
+        timeout = False
         with open(input_file_path, "r") as input_file:
-            process = subprocess.Popen(command, shell=True, stdin=input_file, stdout=subprocess.PIPE, stderr=subprocess.PIPE, env=env)
-            process.wait()
-        timeout_exit_code = process.returncode
-        lines = process.stderr.read().decode("utf-8").splitlines()
-        output = process.stdout.read().decode("utf-8").splitlines()
+            process = subprocess.Popen(command, shell=True, stdin=input_file, stdout=subprocess.PIPE,
+                                       stderr=subprocess.PIPE, env=env, preexec_fn=os.setsid)
+
+            def sigint_handler(signum, frame):
+                try:
+                    os.killpg(os.getpgid(process.pid), signal.SIGTERM)
+                except ProcessLookupError:
+                    pass
+                sys.exit(1)
+            signal.signal(signal.SIGINT, sigint_handler)
+
+            try:
+                output, lines = process.communicate(timeout=hard_time_limit)
+            except subprocess.TimeoutExpired:
+                timeout = True
+                os.killpg(os.getpgid(process.pid), signal.SIGTERM)
+                process.communicate()
 
         result = ExecutionResult()
 
-        for line in lines:
-            line = line.strip()
-            if ": " in line:
-                (key, value) = line.split(": ")[:2]
-                if key == "Time":
-                    result.Time = self.parse_time(value)
-                elif key == "Memory":
-                    result.Memory = self.parse_memory(value)
-                else:
-                    setattr(result, key, value)
+        if not timeout:
+            lines = lines.decode('utf-8').splitlines()
+            output = output.decode('utf-8').splitlines()
+
+            for line in lines:
+                line = line.strip()
+                if ": " in line:
+                    (key, value) = line.split(": ")[:2]
+                    if key == "Time":
+                        result.Time = self.parse_time(value)
+                    elif key == "Memory":
+                        result.Memory = self.parse_memory(value)
+                    else:
+                        setattr(result, key, value)
 
-        # If timeout kills the process, the exit code should be 137.
-        # But on Arch Linux it returns the negative value of the signal that killed the process.
-        if timeout_exit_code == 137 or timeout_exit_code == -9:
+        if timeout:
             result.Status = "TL"
         elif getattr(result, "Time") is not None and result.Time > time_limit:
             result.Status = "TL"
         elif getattr(result, "Memory") is not None and result.Memory > memory_limit:
             result.Status = "ML"
         elif getattr(result, "Status") is None:
             result.Status = "RE"
@@ -285,46 +452,62 @@
         else:
             result.Status = result.Status[:2]
 
         return result
 
 
     def execute_time(self, command, name, result_file_path, input_file_path, output_file_path, answer_file_path,
-                      time_limit, memory_limit):
+                      time_limit, memory_limit, hard_time_limit):
+
+        timeout = False
         with open(input_file_path, "r") as input_file:
-            process = subprocess.Popen(command, stdin=input_file, stdout=subprocess.PIPE, stderr=subprocess.DEVNULL)
-            process.wait()
-        timeout_exit_code = process.returncode
-        output = process.stdout.read().decode("utf-8").splitlines()
+            process = subprocess.Popen(command, stdin=input_file, stdout=subprocess.PIPE, stderr=subprocess.DEVNULL,
+                                       preexec_fn=os.setsid)
+
+            def sigint_handler(signum, frame):
+                try:
+                    os.killpg(os.getpgid(process.pid), signal.SIGTERM)
+                except ProcessLookupError:
+                    pass
+                sys.exit(1)
+            signal.signal(signal.SIGINT, sigint_handler)
+
+            try:
+                output, _ = process.communicate(timeout=hard_time_limit)
+            except subprocess.TimeoutExpired:
+                timeout = True
+                os.killpg(os.getpgid(process.pid), signal.SIGTERM)
 
         result = ExecutionResult()
-        lines = open(result_file_path).readlines()
         program_exit_code = None
-        if len(lines) == 3:
-            """
-            If programs runs successfully, the output looks like this:
-             - first line is CPU time in seconds
-             - second line is memory in KB
-             - third line is exit code
-            This format is defined by -f flag in time command.
-            """
-            result.Time = round(float(lines[0].strip()) * 1000)
-            result.Memory = int(lines[1].strip())
-            program_exit_code = int(lines[2].strip())
-        if len(lines) > 0 and "Command terminated by signal " in lines[0]:
-            """
-            If there was a runtime error, the first line is the error message with signal number.
-            For example:
-                Command terminated by signal 11
-            """
-            program_exit_code = int(lines[0].strip().split(" ")[-1])
+        if not timeout:
+            output = output.decode("utf-8").splitlines()
+            lines = open(result_file_path).readlines()
+            if len(lines) == 3:
+                """
+                If programs runs successfully, the output looks like this:
+                 - first line is CPU time in seconds
+                 - second line is memory in KB
+                 - third line is exit code
+                This format is defined by -f flag in time command.
+                """
+                result.Time = round(float(lines[0].strip()) * 1000)
+                result.Memory = int(lines[1].strip())
+                program_exit_code = int(lines[2].strip())
+            if len(lines) > 0 and "Command terminated by signal " in lines[0]:
+                """
+                If there was a runtime error, the first line is the error message with signal number.
+                For example:
+                    Command terminated by signal 11
+                """
+                program_exit_code = int(lines[0].strip().split(" ")[-1])
 
-        if program_exit_code != None and program_exit_code != 0:
+        if program_exit_code is not None and program_exit_code != 0:
             result.Status = "RE"
-        elif timeout_exit_code != 0:
+        elif timeout:
             result.Status = "TL"
         elif result.Time > time_limit:
             result.Status = "TL"
         elif result.Memory > memory_limit:
             result.Status = "ML"
         else:
             try:
@@ -343,45 +526,39 @@
 
     def run_solution(self, data_for_execution: ExecutionData):
         """
         Run an execution and return the result as ExecutionResult object.
         """
 
         (name, executable, test, time_limit, memory_limit, timetool_path) = data_for_execution
-        file_no_ext = os.path.join(self.EXECUTIONS_DIR, name, self.extract_test_id(test))
+        file_no_ext = os.path.join(self.EXECUTIONS_DIR, name, package_util.extract_test_id(test))
         output_file = file_no_ext + ".out"
         result_file = file_no_ext + ".res"
         hard_time_limit_in_s = math.ceil(2 * time_limit / 1000.0)
 
         if self.args.time_tool == 'oiejq':
-            command = f'timeout -k {hard_time_limit_in_s}s -s SIGKILL {hard_time_limit_in_s}s "{timetool_path}" "{executable}"'
+            command = f'"{timetool_path}" "{executable}"'
 
-            return self.execute_oiejq(command,  name, result_file, test, output_file, self.get_output_file(test), time_limit, memory_limit)
+            return self.execute_oiejq(command, name, result_file, test, output_file, self.get_output_file(test),
+                                      time_limit, memory_limit, hard_time_limit_in_s)
         elif self.args.time_tool == 'time':
             if sys.platform == 'darwin':
                 timeout_name = 'gtimeout'
                 time_name = 'gtime'
             elif sys.platform == 'linux':
                 timeout_name = 'timeout'
                 time_name = 'time'
             elif sys.platform == 'win32' or sys.platform == 'cygwin':
                 raise Exception("Measuring time with GNU time on Windows is not supported.")
 
-            command = [f'{timeout_name}', '-k', f'{hard_time_limit_in_s}s', f'{hard_time_limit_in_s}s',
-                       f'{time_name}', '-f', '%U\\n%M\\n%x', '-o', result_file, executable]
-            return self.execute_time(command,  name, result_file, test, output_file, self.get_output_file(test), time_limit, memory_limit)
+            command = [f'{time_name}', '-f', '%U\\n%M\\n%x', '-o', result_file, executable]
+            return self.execute_time(command, name, result_file, test, output_file, self.get_output_file(test),
+                                     time_limit, memory_limit, hard_time_limit_in_s)
 
-
-    def update_group_status(self, group_status, new_status):
-        order = ["CE", "TL", "ML", "RE", "WA", "OK"]
-        if order.index(new_status) < order.index(group_status):
-            return new_status
-        return group_status
-
-    def run_solutions(self, compiled_commands, names, solutions, report_file):
+    def run_solutions(self, compiled_commands, names, solutions):
         """
         Run solutions on tests and print the results as a table to stdout.
         """
 
         executions = []
         all_results = collections.defaultdict(
             lambda: collections.defaultdict(lambda: collections.defaultdict(map)))
@@ -393,143 +570,50 @@
                 os.makedirs(os.path.join(self.EXECUTIONS_DIR, name), exist_ok=True)
             else:
                 for test in self.tests:
                     all_results[name][self.get_group(test)][test] = ExecutionResult("CE")
         print()
         executions.sort(key = lambda x: (self.get_executable_key(x[1]), x[2]))
         program_groups_scores = collections.defaultdict(dict)
+        print_data = PrintData(0)
 
-        def print_view(output_file=None):
-            def print_stream(*values, end='\n'):
-                if output_file is not None:
-                    print(*values, end=end, file=output_file)
-                else:
-                    print(*values, end=end)
+        has_terminal, terminal_width, terminal_height = util.get_terminal_size()
 
-            if i != 0 and output_file is None:
-                # TODO: always display both tables
-                # if self.args.verbose:
-                #   cursor_delta = len(self.tests) + len(self.groups)+ 9
-                #   if not self.args.hide_memory:
-                #       cursor_delta += len(self.tests)
-                # else:
-                cursor_delta = len(self.groups) + 7
-                number_of_rows = (len(solutions) + self.PROGRAMS_IN_ROW - 1) // self.PROGRAMS_IN_ROW
-                sys.stdout.write('\033[%dA' % (cursor_delta * number_of_rows + 1))
-            program_scores = collections.defaultdict(int)
-            program_times = collections.defaultdict(lambda: -1)
-            program_memory = collections.defaultdict(lambda: -1)
-            if output_file is None:
-                time_remaining = (len(executions) - i - 1) * 2 * self.time_limit / self.cpus / 1000.0
-                print_stream('Done %4d/%4d. Time remaining (in the worst case): %5d seconds.'
-                             % (i+1, len(executions), time_remaining))
-            for program_ix in range(0, len(names), self.PROGRAMS_IN_ROW):
-                # how to jump one line up
-                program_group = names[program_ix:program_ix + self.PROGRAMS_IN_ROW]
-                print_stream("groups", end=" | ")
-                for program in program_group:
-                    print_stream("%10s" % program, end=" | ")
-                print_stream()
-                print_stream(6*"-", end=" | ")
-                for program in program_group:
-                    print_stream(10*"-", end=" | ")
-                print_stream()
-                for group in self.groups:
-                    print_stream("%6s" % group, end=" | ")
-                    for program in program_group:
-                        results = all_results[program][group]
-                        group_status = "OK"
-                        min_points = 100
-
-                        for test in results:
-                            min_points = min(min_points, results[test].Points)
-                            status = results[test].Status
-                            if getattr(results[test], "Time") is not None:
-                                program_times[program] = max(
-                                    program_times[program], results[test].Time)
-                            elif status == "TL":
-                                program_times[program] = 2 * self.time_limit
-                            if getattr(results[test], "Memory") is not None:
-                                program_memory[program] = max(
-                                    program_memory[program], results[test].Memory)
-                            elif status == "ML":
-                                program_memory[program] = 2 * self.memory_limit
-                            if status == "  ":
-                                group_status = "  "
-                                min_points = 0
-                            else:
-                                group_status = self.update_group_status(group_status, status)
-
-                        points = math.floor(min_points / 100 * self.scores[group])
-                        print_stream("%3s" % util.bold(util.color_green(group_status)) if group_status == "OK" else util.bold(util.color_red(group_status)),
-                                     "%3s/%3s" % (points, self.scores[group]),
-                                     end=" | ")
-                        program_scores[program] += self.scores[group] if group_status == "OK" else 0
-                        program_groups_scores[program][group] = {"status": group_status, "points": points}
-                    print_stream()
-                print_stream(6*" ", end=" | ")
-                for program in program_group:
-                    print_stream(10*" ", end=" | ")
-                print_stream()
-                print_stream("points", end=" | ")
-                for program in program_group:
-                    print_stream(util.bold("   %3s/%3s" % (program_scores[program], self.possible_score)), end=" | ")
-                print_stream()
-                print_stream("  time", end=" | ")
-                for program in program_group:
-                    program_time = program_times[program]
-                    print_stream(util.bold(("%20s" % self.color_time(program_time, self.time_limit))
-                                           if program_time < 2 * self.time_limit and program_time >= 0
-                                           else "   "+7*'-'), end=" | ")
-                print_stream()
-                print_stream("memory", end=" | ")
-                for program in program_group:
-                    program_mem = program_memory[program]
-                    print_stream(util.bold(("%20s" % self.color_memory(program_mem, self.memory_limit))
-                                           if program_mem < 2 * self.memory_limit and program_mem >= 0
-                                           else "   "+7*'-'), end=" | ")
-                print_stream()
-                # TODO: always display both tables
-                # if self.args.verbose:
-                #   print_stream(6*" ", end=" | ")
-                #   for program in program_group:
-                #       print_stream(10*" ", end=" | ")
-                #   print_stream()
-                #   for test in self.tests:
-                #       print_stream("%6s" % self.extract_test_id(test), end=" | ")
-                #       for program in program_group:
-                #           result = all_results[program][self.get_group(test)][test]
-                #           status = result.Status
-                #           if status == "  ": print_stream(10*' ', end=" | ")
-                #           else:
-                #               print_stream("%3s" % self.colorize_status(status),
-                #                   ("%17s" % self.color_time(result.Time, self.time_limit)) if getattr(result, "Time") is not None else 7*" ", end=" | ")
-                #       print_stream()
-                #       if not self.args.hide_memory:
-                #           print_stream(6*" ", end=" | ")
-                #           for program in program_group:
-                #               result = all_results[program][self.get_group(test)][test]
-                #               print_stream(("%20s" % self.color_memory(result.Memory, self.memory_limit))  if getattr(result, "Memory") is not None else 10*" ", end=" | ")
-                #           print_stream()
-                #   print_stream()
-                print_stream(10*len(program_group)*' ')
-
-            if output_file is not None:
-                os.system('sed -i -r "s/\x1B\[([0-9]{1,3}(;[0-9]{1,2})?)?[mGK]//g" %s' % output_file) # TODO: make this work on Windows
-                print("Report has been saved to", util.bold(output_file))
-                print()
+        if has_terminal:
+            run_event = threading.Event()
+            run_event.set()
+            thr = threading.Thread(target=printer.printer_thread,
+                                   args=(run_event, print_view, program_groups_scores, all_results, print_data, names,
+                                         executions, self.groups, self.scores, self.tests, self.possible_score,
+                                         self.time_limit, self.memory_limit, self.cpus, self.args.hide_memory))
+            thr.start()
 
-        print("Performing %d executions..." % len(executions))
-        with mp.Pool(self.cpus) as pool:
+        pool = mp.Pool(self.cpus)
+        keyboard_interrupt = False
+        try:
             for i, result in enumerate(pool.imap(self.run_solution, executions)):
                 (name, executable, test) = executions[i][:3]
                 all_results[name][self.get_group(test)][test] = result
-                print_view()
-        if report_file:
-            print_view(report_file)
+                print_data.i = i
+            pool.terminate()
+        except KeyboardInterrupt:
+            keyboard_interrupt = True
+            pool.terminate()
+        finally:
+            if has_terminal:
+                run_event.clear()
+                thr.join()
+
+        print("\n".join(print_view(terminal_width, terminal_height, program_groups_scores, all_results, print_data,
+                                   names, executions, self.groups, self.scores, self.tests, self.possible_score,
+                                   self.time_limit, self.memory_limit, self.cpus, self.args.hide_memory)[0]))
+
+        if keyboard_interrupt:
+            util.exit_with_error("Stopped due to keyboard interrupt.")
+
         return program_groups_scores, all_results
 
 
     def calculate_points(self, results):
         points = 0
         for group, result in results.items():
             if group != 0 and group not in self.scores:
@@ -539,28 +623,23 @@
                     points += self.scores[group]
             elif isinstance(result, dict):
                 points += result["points"]
         return points
 
     def compile_and_run(self, solutions):
         compilation_results = self.compile_solutions(solutions)
-        compiled_solutions = []
         for i in range(len(solutions)):
-            if compilation_results[i]:
-                compiled_solutions.append(solutions[i])
-            else:
+            if not compilation_results[i]:
                 self.failed_compilations.append(solutions[i])
-        compilation_results = [result for result in compilation_results if result]
-
         os.makedirs(self.EXECUTIONS_DIR, exist_ok=True)
         executables = [os.path.join(self.EXECUTABLES_DIR, package_util.get_executable(solution))
-                       for solution in compiled_solutions]
-        compiled_commands = zip(compiled_solutions, executables, compilation_results)
-        names = compiled_solutions
-        return self.run_solutions(compiled_commands, names, compiled_solutions, self.args.solutions_report)
+                       for solution in solutions]
+        compiled_commands = zip(solutions, executables, compilation_results)
+        names = solutions
+        return self.run_solutions(compiled_commands, names, solutions)
 
 
     def print_expected_scores(self, expected_scores):
         yaml_dict = { "sinol_expected_scores": expected_scores }
         print(yaml.dump(yaml_dict, default_flow_style=None))
 
 
@@ -766,15 +845,15 @@
                         config_expected_scores[solution] = diff.new_expected_scores[solution]
 
 
                 self.config["sinol_expected_scores"] = config_expected_scores
                 util.save_config(self.config)
                 print(util.info("Saved suggested expected scores description."))
             else:
-                util.exit_with_error("Use flag --apply_suggestions to apply suggestions.")
+                util.exit_with_error("Use flag --apply-suggestions to apply suggestions.")
 
 
     def set_constants(self):
         self.ID = package_util.get_task_id()
         self.TMP_DIR = os.path.join(os.getcwd(), "cache")
         self.COMPILATION_DIR = os.path.join(self.TMP_DIR, "compilation")
         self.EXECUTIONS_DIR = os.path.join(self.TMP_DIR, "executions")
@@ -852,18 +931,18 @@
         self.possible_score = self.get_possible_score(self.groups)
 
     def get_valid_input_files(self):
         """
         Returns list of input files that have corresponding output file.
         """
         output_tests = glob.glob(os.path.join(os.getcwd(), "out", "*.out"))
-        output_tests_ids = [self.extract_test_id(test) for test in output_tests]
+        output_tests_ids = [package_util.extract_test_id(test) for test in output_tests]
         valid_input_files = []
         for test in self.tests:
-            if self.extract_test_id(test) in output_tests_ids:
+            if package_util.extract_test_id(test) in output_tests_ids:
                 valid_input_files.append(test)
         return valid_input_files
 
     def validate_existence_of_outputs(self):
         """
         Checks if all input files have corresponding output files.
         """
@@ -895,15 +974,15 @@
             print(util.warning('There are no tests to run.'))
 
     def check_errors(self, results: dict[str, dict[str, dict[str, ExecutionResult]]]):
         error_msg = ""
         for solution in results:
             for group in results[solution]:
                 for test in results[solution][group]:
-                    if results[solution][group][test].Status == "CE":
+                    if results[solution][group][test].Status == "CE" and results[solution][group][test].Error is not None:
                         error_msg += f'Solution {solution} had an error on test {test}: {results[solution][group][test].Error}\n'
         if error_msg != "":
             util.exit_with_error(error_msg)
 
     def run(self, args):
         if not util.check_if_project():
             print(util.warning('You are not in a project directory (couldn\'t find config.yml in current directory).'))
```

### Comparing `sinol-make-1.3.0/src/sinol_make/commands/run/structs.py` & `sinol-make-1.3.1/src/sinol_make/commands/run/structs.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,7 +59,18 @@
     test: str
     # Time limit for this test in milliseconds
     time_limit: int
     # Memory limit in KB
     memory_limit: int
     # Path to the timetool executable
     timetool_path: str
+    # Dictionary of pids for each execution
+    execution_pids: dict[dict[str, int]]
+
+
+@dataclass
+class PrintData:
+    """
+    Represents data for printing results of execution.
+    """
+
+    i: int
```

### Comparing `sinol-make-1.3.0/src/sinol_make/helpers/compile.py` & `sinol-make-1.3.1/src/sinol_make/helpers/compile.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,34 +50,35 @@
 
     if process.returncode != 0:
         raise CompilationError('Compilation failed')
     else:
         return True
 
 
-def compile_file(file_path: str, name: str, compilers: Compilers) -> Tuple[str or None, str]:
+def compile_file(file_path: str, name: str, compilers: Compilers, weak_compilation_flags = False) -> Tuple[str or None, str]:
     """
     Compile a file
     :param file_path: Path to the file to compile
     :param name: Name of the executable
     :param compilers: Compilers object
+    :param weak_compilation_flags: Use weaker compilation flags
     :return: Tuple of (executable path or None if compilation failed, log path)
     """
 
     executable_dir = os.path.join(os.getcwd(), 'cache', 'executables')
     compile_log_dir = os.path.join(os.getcwd(), 'cache', 'compilation')
     os.makedirs(executable_dir, exist_ok=True)
     os.makedirs(compile_log_dir, exist_ok=True)
 
     output = os.path.join(executable_dir, name)
     compile_log_path = os.path.join(compile_log_dir, os.path.splitext(name)[0] + '.compile_log')
     compile_log = open(compile_log_path, 'w')
 
     try:
-        if compile(file_path, output, compilers, compile_log):
+        if compile(file_path, output, compilers, compile_log, weak_compilation_flags):
             return output, compile_log_path
         else:
             return None, compile_log_path
     except CompilationError:
         return None, compile_log_path
```

### Comparing `sinol-make-1.3.0/src/sinol_make/helpers/compiler.py` & `sinol-make-1.3.1/src/sinol_make/helpers/compiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,33 +84,33 @@
     for solution in solutions:
         ext = os.path.splitext(solution)[1]
         compiler = ""
         tried = ""
         flag = ""
         if ext == '.c' and args.c_compiler_path is None:
             compiler = 'C compiler'
-            flag = '--c_compiler_path'
+            flag = '--c-compiler-path'
             if sys.platform == 'darwin':
                 tried = 'gcc-{9,10}'
             else:
                 tried = 'gcc'
         elif ext == '.cpp' and args.cpp_compiler_path is None:
             compiler = 'C++ compiler'
-            flag = '--cpp_compiler_path'
+            flag = '--cpp-compiler-path'
             if sys.platform == 'darwin':
                 tried = 'g++-{9,10}'
             else:
                 tried = 'g++'
         elif ext == '.py' and args.python_interpreter_path is None:
             compiler = 'Python interpreter'
-            flag = '--python_interpreter_path'
+            flag = '--python-interpreter-path'
             tried = 'python3'
         elif ext == '.java' and args.java_compiler_path is None:
             compiler = 'Java compiler'
-            flag = '--java_compiler_path'
+            flag = '--java-compiler-path'
             tried = 'javac'
 
         if compiler != "":
             util.exit_with_error(
                 'Couldn\'t find a %s. Tried %s. Try specifying a compiler with %s.' % (compiler, tried, flag))
 
     return Compilers(
```

### Comparing `sinol-make-1.3.0/src/sinol_make/helpers/package_util.py` & `sinol-make-1.3.1/src/sinol_make/helpers/package_util.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.3.0/src/sinol_make/helpers/parsers.py` & `sinol-make-1.3.1/src/sinol_make/helpers/parsers.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,17 @@
     if sys.platform == 'darwin':
         gcc_versions = 'gcc-9, gcc-10, gcc-11'
         gpp_versions = 'g++-9, g++-10, g++-11'
     else:
         gcc_versions = 'gcc'
         gpp_versions = 'g++'
 
-    parser.add_argument('--c_compiler_path', type=str, default=compiler.get_c_compiler_path(),
+    parser.add_argument('--c-compiler-path', dest='c_compiler_path', type=str, default=compiler.get_c_compiler_path(),
                         help=f'C compiler to use (default {gcc_versions})')
-    parser.add_argument('--cpp_compiler_path', type=str, default=compiler.get_cpp_compiler_path(),
+    parser.add_argument('--cpp-compiler-path', dest='cpp_compiler_path', type=str, default=compiler.get_cpp_compiler_path(),
                         help=f'C++ compiler to use (default {gpp_versions})')
-    parser.add_argument('--python_interpreter_path', type=str, default=compiler.get_python_interpreter_path(),
+    parser.add_argument('--python-interpreter-path', dest='python_interpreter_path', type=str, default=compiler.get_python_interpreter_path(),
                         help='Python interpreter to use (default: python3)')
-    parser.add_argument('--java_compiler_path', type=str, default=compiler.get_java_compiler_path(),
+    parser.add_argument('--java-compiler-path', dest='java_compiler_path', type=str, default=compiler.get_java_compiler_path(),
                         help='Java compiler to use (default: javac)')
+    parser.add_argument('--weak-compilation-flags', dest='weak_compilation_flags', action='store_true',
+                        help='use weaker compilation flags')
```

### Comparing `sinol-make-1.3.0/src/sinol_make/structs/compiler_structs.py` & `sinol-make-1.3.1/src/sinol_make/structs/compiler_structs.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.3.0/src/sinol_make/util.py` & `sinol-make-1.3.1/src/sinol_make/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -244,14 +244,29 @@
     """
     Function to compare two files.
     Returns True if they are the same, False otherwise.
     """
     return lines_diff(open(file1).readlines(), open(file2).readlines())
 
 
+def get_terminal_size():
+    """
+    Function to get the size of the terminal.
+    :return: triple (has_terminal, width, height)
+    """
+    has_terminal = True
+    try:
+        terminal_width = os.get_terminal_size().columns
+        terminal_height = os.get_terminal_size().lines
+    except OSError:
+        has_terminal = False
+        terminal_width = 80
+        terminal_height = 30
+    return has_terminal, terminal_width, terminal_height
+
 def color_red(text): return "\033[91m{}\033[00m".format(text)
 def color_green(text): return "\033[92m{}\033[00m".format(text)
 def color_yellow(text): return "\033[93m{}\033[00m".format(text)
 def bold(text): return "\033[01m{}\033[00m".format(text)
 
 def info(text):
     return bold(color_green(text))
```

### Comparing `sinol-make-1.3.0/src/sinol_make.egg-info/PKG-INFO` & `sinol-make-1.3.1/src/sinol_make.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinol-make
-Version: 1.3.0
+Version: 1.3.1
 Summary: CLI tool for creating sio2 task packages
 Author-email: Mateusz Masiarz <m.masiarz@fri.edu.pl>
 Maintainer-email: Tomasz Nowak <tomasz.nowak@tonowak.com>
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -55,17 +55,26 @@
 ```
 
 As `oiejq` works only on Linux-based operating systems,
 *we do not recommend* using operating systems such as Windows or macOS.
 Nevertheless `sinol-make` supports those operating systems,
 though there are additional installation steps required to use
 other tools for measuring time (which are non-deterministic and produce reports different from sio2):
-- Windows (WSL): `apt install time timeout`
+- Windows (WSL): `apt install time`
 - macOS: `brew install gnu-time coreutils`
 
+### Autocompletion (optional)
+
+If you would like to have autocompletion for `sinol-make` commands,
+run the following command and refresh the shell (e.g. by opening a new terminal):
+
+```shell
+activate-global-python-argcomplete
+```
+
 ### Usage
 
 The availabe commands (see `sinol-make --help`) are:
 
 - `sinol-make run` -- Runs selected solutions (by default all solutions) on selected tests (by default all tests) with a given number
 of CPUs. Measures the solutions' time with oiejq, unless specified otherwise. After running the solutions, it
 compares the solutions' scores with the ones saved in config.yml.
```

### Comparing `sinol-make-1.3.0/src/sinol_make.egg-info/SOURCES.txt` & `sinol-make-1.3.1/src/sinol_make.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,12 +15,14 @@
 src/sinol_make/commands/run/__init__.py
 src/sinol_make/commands/run/structs.py
 src/sinol_make/helpers/__init__.py
 src/sinol_make/helpers/compile.py
 src/sinol_make/helpers/compiler.py
 src/sinol_make/helpers/package_util.py
 src/sinol_make/helpers/parsers.py
+src/sinol_make/helpers/printer.py
 src/sinol_make/interfaces/BaseCommand.py
 src/sinol_make/interfaces/Errors.py
 src/sinol_make/interfaces/__init__.py
+src/sinol_make/structs/__init__.py
 src/sinol_make/structs/compiler_structs.py
 tests/test_util.py
```

### Comparing `sinol-make-1.3.0/tests/test_util.py` & `sinol-make-1.3.1/tests/test_util.py`

 * *Files identical despite different names*

