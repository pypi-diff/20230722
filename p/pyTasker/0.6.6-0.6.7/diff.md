# Comparing `tmp/pyTasker-0.6.6.tar.gz` & `tmp/pyTasker-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTasker-0.6.6.tar", last modified: Sun Jul  9 13:15:14 2023, max compression
+gzip compressed data, was "pyTasker-0.6.7.tar", last modified: Sat Jul 22 12:48:44 2023, max compression
```

## Comparing `pyTasker-0.6.6.tar` & `pyTasker-0.6.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 13:15:14.739399 pyTasker-0.6.6/
--rw-rw-rw-   0        0        0      305 2023-07-08 17:38:54.000000 pyTasker-0.6.6/.gitignore
--rw-rw-rw-   0        0        0     1115 2022-03-07 21:04:39.000000 pyTasker-0.6.6/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      733 2022-03-07 21:04:39.000000 pyTasker-0.6.6/CHANGELOG.md
--rw-rw-rw-   0        0        0    35746 2022-02-03 21:25:58.000000 pyTasker-0.6.6/LICENSE
--rw-rw-rw-   0        0        0     7532 2023-07-09 13:15:14.739399 pyTasker-0.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     6460 2023-07-08 17:38:54.000000 pyTasker-0.6.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 13:15:14.712398 pyTasker-0.6.6/Tasker/
--rw-rw-rw-   0        0        0      569 2023-07-08 17:38:54.000000 pyTasker-0.6.6/Tasker/__init__.py
--rw-rw-rw-   0        0        0     3109 2023-07-08 17:38:54.000000 pyTasker-0.6.6/Tasker/__main__.py
--rw-rw-rw-   0        0        0       23 2023-07-09 13:14:09.000000 pyTasker-0.6.6/Tasker/__version__.py
--rw-rw-rw-   0        0        0     3554 2023-07-08 17:38:54.000000 pyTasker-0.6.6/Tasker/cli.py
--rw-rw-rw-   0        0        0     2712 2023-07-08 17:38:54.000000 pyTasker-0.6.6/Tasker/common.py
--rw-rw-rw-   0        0        0     2578 2022-03-07 21:04:39.000000 pyTasker-0.6.6/Tasker/inspector.py
--rw-rw-rw-   0        0        0    15270 2023-07-08 17:38:54.000000 pyTasker-0.6.6/Tasker/operations.py
--rw-rw-rw-   0        0        0    27340 2023-07-09 13:13:58.000000 pyTasker-0.6.6/Tasker/parser.py
--rw-rw-rw-   0        0        0     1315 2022-03-07 21:04:39.000000 pyTasker-0.6.6/Tasker/parser_test.py
--rw-rw-rw-   0        0        0    17710 2023-07-08 17:38:54.000000 pyTasker-0.6.6/Tasker/templater.py
--rw-rw-rw-   0        0        0     6988 2023-07-09 13:08:50.000000 pyTasker-0.6.6/Tasker/types.py
-drwxrwxrwx   0        0        0        0 2023-07-09 13:15:14.735399 pyTasker-0.6.6/pyTasker.egg-info/
--rw-rw-rw-   0        0        0     7532 2023-07-09 13:15:14.000000 pyTasker-0.6.6/pyTasker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      568 2023-07-09 13:15:14.000000 pyTasker-0.6.6/pyTasker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 13:15:14.000000 pyTasker-0.6.6/pyTasker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-09 13:15:14.000000 pyTasker-0.6.6/pyTasker.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       58 2023-07-09 13:15:14.000000 pyTasker-0.6.6/pyTasker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-09 13:15:14.000000 pyTasker-0.6.6/pyTasker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      268 2022-03-07 21:04:39.000000 pyTasker-0.6.6/pyproject.toml
--rw-rw-rw-   0        0        0      113 2023-07-08 17:38:54.000000 pyTasker-0.6.6/requirements.txt
--rw-rw-rw-   0        0        0      191 2023-07-09 13:15:14.741398 pyTasker-0.6.6/setup.cfg
--rw-rw-rw-   0        0        0     1787 2023-07-09 13:14:07.000000 pyTasker-0.6.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 13:15:14.738398 pyTasker-0.6.6/static/
--rw-rw-rw-   0        0        0   424108 2022-02-03 21:25:58.000000 pyTasker-0.6.6/static/Copy PDFs then zip.png
--rw-rw-rw-   0        0        0   136520 2022-02-03 21:25:58.000000 pyTasker-0.6.6/static/Copy PDFs.png
+drwxrwxrwx   0        0        0        0 2023-07-22 12:48:44.285249 pyTasker-0.6.7/
+-rw-rw-rw-   0        0        0      327 2023-07-22 12:20:52.000000 pyTasker-0.6.7/.gitignore
+-rw-rw-rw-   0        0        0     1115 2022-03-07 21:04:39.000000 pyTasker-0.6.7/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0      733 2022-03-07 21:04:39.000000 pyTasker-0.6.7/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35746 2022-02-03 21:25:58.000000 pyTasker-0.6.7/LICENSE
+-rw-rw-rw-   0        0        0     7532 2023-07-22 12:48:44.285249 pyTasker-0.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6460 2023-07-08 17:38:54.000000 pyTasker-0.6.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 12:48:44.251248 pyTasker-0.6.7/Tasker/
+-rw-rw-rw-   0        0        0      569 2023-07-08 17:38:54.000000 pyTasker-0.6.7/Tasker/__init__.py
+-rw-rw-rw-   0        0        0     3109 2023-07-08 17:38:54.000000 pyTasker-0.6.7/Tasker/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-07-22 12:20:17.000000 pyTasker-0.6.7/Tasker/__version__.py
+-rw-rw-rw-   0        0        0     3554 2023-07-08 17:38:54.000000 pyTasker-0.6.7/Tasker/cli.py
+-rw-rw-rw-   0        0        0     2712 2023-07-08 17:38:54.000000 pyTasker-0.6.7/Tasker/common.py
+-rw-rw-rw-   0        0        0     2578 2022-03-07 21:04:39.000000 pyTasker-0.6.7/Tasker/inspector.py
+-rw-rw-rw-   0        0        0    15270 2023-07-08 17:38:54.000000 pyTasker-0.6.7/Tasker/operations.py
+-rw-rw-rw-   0        0        0    28361 2023-07-22 12:47:51.000000 pyTasker-0.6.7/Tasker/parser.py
+-rw-rw-rw-   0        0        0     1315 2022-03-07 21:04:39.000000 pyTasker-0.6.7/Tasker/parser_test.py
+-rw-rw-rw-   0        0        0    17710 2023-07-08 17:38:54.000000 pyTasker-0.6.7/Tasker/templater.py
+-rw-rw-rw-   0        0        0     7246 2023-07-22 12:34:52.000000 pyTasker-0.6.7/Tasker/types.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:48:44.278248 pyTasker-0.6.7/pyTasker.egg-info/
+-rw-rw-rw-   0        0        0     7532 2023-07-22 12:48:43.000000 pyTasker-0.6.7/pyTasker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      568 2023-07-22 12:48:44.000000 pyTasker-0.6.7/pyTasker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 12:48:43.000000 pyTasker-0.6.7/pyTasker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-22 12:48:43.000000 pyTasker-0.6.7/pyTasker.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       58 2023-07-22 12:48:43.000000 pyTasker-0.6.7/pyTasker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-22 12:48:43.000000 pyTasker-0.6.7/pyTasker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      268 2022-03-07 21:04:39.000000 pyTasker-0.6.7/pyproject.toml
+-rw-rw-rw-   0        0        0      100 2023-07-22 12:47:49.000000 pyTasker-0.6.7/requirements.txt
+-rw-rw-rw-   0        0        0      191 2023-07-22 12:48:44.290247 pyTasker-0.6.7/setup.cfg
+-rw-rw-rw-   0        0        0     1787 2023-07-22 12:20:17.000000 pyTasker-0.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 12:48:44.283249 pyTasker-0.6.7/static/
+-rw-rw-rw-   0        0        0   424108 2022-02-03 21:25:58.000000 pyTasker-0.6.7/static/Copy PDFs then zip.png
+-rw-rw-rw-   0        0        0   136520 2022-02-03 21:25:58.000000 pyTasker-0.6.7/static/Copy PDFs.png
```

### Comparing `pyTasker-0.6.6/.pre-commit-config.yaml` & `pyTasker-0.6.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.6/CHANGELOG.md` & `pyTasker-0.6.7/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.6/LICENSE` & `pyTasker-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.6/PKG-INFO` & `pyTasker-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTasker
-Version: 0.6.6
+Version: 0.6.7
 Summary: Run pipelines on your own computer for better automation
 Home-page: https://github.com/carlossilva2/pyTasker
 Author: Carlos Silva
 Author-email: carlos.miguel.silva@protonmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/carlossilva2/pyTasker
 Project-URL: Documentation, https://cmsilva.gitbook.io/pytasker/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyTasker Version: 0.6.6 Summary: Run pipelines on
+Metadata-Version: 2.1 Name: pyTasker Version: 0.6.7 Summary: Run pipelines on
 your own computer for better automation Home-page: https://github.com/
 carlossilva2/pyTasker Author: Carlos Silva Author-email:
 carlos.miguel.silva@protonmail.com License: GPLv3 Project-URL: Source, https://
 github.com/carlossilva2/pyTasker Project-URL: Documentation, https://
 cmsilva.gitbook.io/pytasker/ Platform: UNKNOWN Classifier: Development Status
 :: 4 - Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: GNU General Public License v3
```

### Comparing `pyTasker-0.6.6/README.md` & `pyTasker-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.6/Tasker/__init__.py` & `pyTasker-0.6.7/Tasker/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.6/Tasker/__main__.py` & `pyTasker-0.6.7/Tasker/__main__.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.6/Tasker/cli.py` & `pyTasker-0.6.7/Tasker/cli.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.6/Tasker/common.py` & `pyTasker-0.6.7/Tasker/common.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.6/Tasker/inspector.py` & `pyTasker-0.6.7/Tasker/inspector.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.6/Tasker/operations.py` & `pyTasker-0.6.7/Tasker/operations.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.6/Tasker/parser.py` & `pyTasker-0.6.7/Tasker/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 import os.path as Path
 import platform
 import sys
 from hashlib import md5
 from importlib.machinery import SourceFileLoader as importer
 from logging import WARNING, Logger, getLogger
 from time import time
-from typing import List, Literal, Union
+from typing import Dict, List, Literal, Union
 from webbrowser import open as FileOpener
 
 import chalk
 from requests import get
 
+from .cli import get_logger
 from .common import Timer, pip, pip_freeze
 from .inspector import implements
 from .operations import *
 from .types import (
     DESTINATION_CHECK_MAP,
     OP_COMMAND,
     OP_COPY,
@@ -28,31 +29,39 @@
     OP_MOVE,
     OP_REQUEST,
     OP_TASK,
     OP_ZIP,
     OPERATIONS,
     Alias,
     CustomOperation,
+    Extension,
     InstructionSet,
     OperationType,
     ParserType,
     Settings,
     Task,
 )
 
 
 @implements(ParserType)
 class Parser(ParserType):
-    def __init__(self, task: str, logger: Logger, abort_exit: bool = False) -> None:
+    def __init__(
+        self,
+        task: str,
+        logger: Logger = None,
+        abort_exit: bool = False,
+        from_ui: bool = False,
+    ) -> None:
         self.abort_exit = abort_exit
+        self.__from_ui = from_ui
         self.execution = {}
         t = Timer()
         t.start()
-        self.supported_os = ["Windows"]  # List of Tasker supported OSes
-        self.logger = logger
+        self.supported_os = ["Windows", "Linux"]  # List of Tasker supported OSes
+        self.logger = logger if logger is not None else get_logger()
         if task not in self.list_all_tasks():
             self.abort(f"'{task}' InstructionSet was not found")
         self.warn_user()
         self.__first_execution_routine()
         self.task: InstructionSet = json.load(
             open(f"{self.default_location}/{task}.tasker.json", "r")
         )
@@ -65,37 +74,39 @@
         self.extensions: List[CustomOperation] = self.__load_extensions()
         self.__change_relative_locations(self.settings["current_location"])
         self.__executed_tasks: List[Task] = []
         self.__operation_stack: List[OperationType] = []
         t.stop()
         self.execution["initialization"] = t.ellapsed_time
 
-    def execute(self) -> None:
+    def execute(self) -> Dict[str, Dict[str, bool | str]]:
         t = Timer()
         t.start()
         self.task["tasks"] = sorted(self.task["tasks"], key=lambda d: d["step"])
+        task_report = {}
         for task in self.task["tasks"]:
-            if self.__execute(task):
-                self.logger.debug(f"Task \"{task['name']}\" - {chalk.green('OK')}")
+            status = self.__execute(task)
+            message = f"Task \"{task['name']}\" - {chalk.green('OK') if status else chalk.red('ERROR')}"
+            if self.__from_ui:
+                task_report[task["name"]] = {"result": status, "message": message}
             else:
-                self.logger.error(f"Task \"{task['name']}\" - {chalk.red('ERROR')}")
+                self.logger.debug(message)
         # Reverse Operation Stack
         # Do this to use rollback feature on a reverse order
         self.__operation_stack.reverse()
         tick = True
         for operation in self.__operation_stack:
             if not operation.get_state() and "-No-Rollback" not in os.environ:
                 if tick:
-                    print()
-                    print("--------------  Rollbacks  --------------")
-                    print()
+                    print("\n--------------  Rollbacks  --------------\n")
                     tick = False
                 operation.rollback()
         t.stop()
         self.execution["execution"] = t.ellapsed_time
+        return task_report
 
     def warn_user(self) -> None:
         "Verifies if current OS is one of the allowed ones"
         self.system = platform.system()
         if (self.system not in self.supported_os) and ("-No-Warning" not in os.environ):
             ans = input(
                 f"'{self.system}' is not part of the current supported OS list.\nAre you sure you want to continue? Y/n\n"
@@ -109,15 +120,18 @@
                 sys.exit(1)
 
     def abort(self, reason: str) -> None:
         self.logger.error(reason)
         if self.abort_exit:
             sys.exit(1)
         else:
-            raise Exception("Aborting due to error")
+            raise Exception(reason)
+
+    def get_execution_time(self) -> str:
+        return self.execution["execution"]
 
     def __execute(self, task: Task) -> bool:
         try:
             self.__check_destination_path(task, DESTINATION_CHECK_MAP[task["operation"]])
             if task["operation"] == "copy":
                 c = Copy(self, task, self.logger)
                 self.__operation_stack.append(c)
@@ -303,15 +317,17 @@
         j: Settings = json.load(open(f"{Path.expanduser('~')}/.tasker/config.json"))
         return j
 
     def __load_extensions(self) -> List[CustomOperation]:
         modules: List[CustomOperation] = []
         for extension in self.settings["extensions"]:
             try:
-                spec: OperationType = importer(f"{extension['file'].replace('.py', '')}", extension["path"]).load_module()  # type: ignore
+                spec: OperationType = importer(
+                    f"{extension['file'].replace('.py', '')}", extension["path"]
+                ).load_module()  # type: ignore
                 modules.append(CustomOperation(executable=spec, summon=extension["name"]))
             except Exception:
                 self.abort(
                     f"There was a problem importing {chalk.yellow(extension['name'])} Custom Extension. Please revise code implementation",
                 )
         return modules
 
@@ -437,15 +453,15 @@
 
     @staticmethod
     def open_file_for_edit(file: str) -> None:
         Parser.do_config()
         FileOpener(f"{Path.expanduser('~')}/.tasker/Tasks/{file}.tasker.json")
 
     @staticmethod
-    def create_extension(name: str) -> None:
+    def create_extension(name: str) -> str:
         Parser.do_config()
         root = Path.expanduser("~")
         with open(f"{root}/.tasker/template.txt", "r") as template:
             t = template.read()
             t = t.replace("<name>", name)
             _n = md5(f"{time()}_{name}".encode("UTF-8")).hexdigest()[:10]
             f_name = f"extension_{_n}.py"
@@ -459,28 +475,42 @@
                     "file": f_name,
                     "path": f"{root}/.tasker/Templates/{f_name}",
                     "version": 0,
                 }
             )
             json.dump(j, open(f"{root}/.tasker/config.json", "w"), indent=4)
             template.close()
+            return f"{root}/.tasker/Templates/{f_name}"
 
     @staticmethod
     def add_alias(alias: Alias, logger: Logger) -> None:
         root = Path.expanduser("~")
         settings: Settings = json.load(open(f"{root}/.tasker/config.json"))
         # check if alias is already present
         for _alias in settings["alias"]:
             if alias["name"] == _alias["name"]:
                 logger.error("An Alias with that name already exists")
                 sys.exit(1)
         settings["alias"].append(alias)
         json.dump(settings, open(f"{root}/.tasker/config.json", "w"), indent=4)
 
     @staticmethod
+    def get_alias() -> List[Alias]:
+        "Return all available aliases"
+        root = Path.expanduser("~")
+        settings: Settings = json.load(open(f"{root}/.tasker/config.json"))
+        return settings["alias"]
+
+    @staticmethod
+    def list_extensions() -> List[Extension]:
+        root = Path.expanduser("~")
+        settings: Settings = json.load(open(f"{root}/.tasker/config.json"))
+        return settings["extensions"]
+
+    @staticmethod
     def install_remote_extension(
         extension: str, logger: Logger, upgrade: bool = False
     ) -> bool:
         def install(context: dict, extension: str, logger: Logger) -> bool:
             # Check if extension is allowed on Current OS
             os = platform.system()
             if (
@@ -659,19 +689,20 @@
         # Check if extension exists on remote
         if extension not in context.keys():
             logger.error("Extension does not exist. Check spelling")
             sys.exit(1)
         logger.debug(f"{extension}=={context[extension]['version']}")
 
     @staticmethod
-    def list_remote(logger: Logger) -> None:
+    def list_remote(logger: Logger | None = None) -> None:
         Parser.do_config()
         # Remove DEBUG WARNINGS
         getLogger("requests").setLevel(WARNING)
         getLogger("urllib3").setLevel(WARNING)
         # Get Context file
         context = get(
             "https://raw.githubusercontent.com/carlossilva2/pyTasker-actions/main/context.json"
         ).json()
-        for extension in context.keys():
-            logger.debug(f"{extension}=={context[extension]['version']}")
+        if logger:
+            for extension in context.keys():
+                logger.debug(f"{extension}=={context[extension]['version']}")
         return context
```

### Comparing `pyTasker-0.6.6/Tasker/parser_test.py` & `pyTasker-0.6.7/Tasker/parser_test.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.6/Tasker/templater.py` & `pyTasker-0.6.7/Tasker/templater.py`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.6/Tasker/types.py` & `pyTasker-0.6.7/Tasker/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,33 +193,37 @@
     alias: List[Alias]
 
 
 class ParserType:
 
     system: str
     abort_exit: bool
+    from_ui: bool
     task: InstructionSet
     logger: Logger
     settings: Settings
     execution: Dict[str, Union[float, str]]
     supported_os: List[str]
     extensions: list
     default_location: str
     __executed_tasks: List[Task]
     __operation_stack: list
 
-    def execute(self) -> None:
+    def execute(self) -> Dict[str, Dict[str, bool | str]]:
         pass
 
     def warn_user(self) -> None:
         pass
 
     def abort(self, reason: str) -> None:
         pass
 
+    def get_execution_time(self) -> str:
+        pass
+
     def __execute(self, task: Task) -> bool:
         return True
 
     def __check_destination_path(self, task: Task) -> None:
         pass
 
     def __analyse_keys(self) -> Tuple[bool, str, str, str]:
@@ -262,21 +266,29 @@
         return InstructionSet()
 
     @staticmethod
     def open_file_for_edit(file: str) -> None:
         pass
 
     @staticmethod
-    def create_extension(name: str) -> None:
+    def create_extension(name: str) -> str:
         pass
 
     @staticmethod
     def add_alias(alias: Alias, logger: Logger) -> None:
         pass
 
+    @staticmethod
+    def get_alias() -> List[Alias]:
+        pass
+
+    @staticmethod
+    def list_extensions() -> List[Extension]:
+        pass
+
 
 class OperationType:
     "Skeleton class for creating other, more complex Operations"
 
     task: Task
     context: ParserType
     logger: Logger
```

### Comparing `pyTasker-0.6.6/pyTasker.egg-info/PKG-INFO` & `pyTasker-0.6.7/pyTasker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTasker
-Version: 0.6.6
+Version: 0.6.7
 Summary: Run pipelines on your own computer for better automation
 Home-page: https://github.com/carlossilva2/pyTasker
 Author: Carlos Silva
 Author-email: carlos.miguel.silva@protonmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/carlossilva2/pyTasker
 Project-URL: Documentation, https://cmsilva.gitbook.io/pytasker/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyTasker Version: 0.6.6 Summary: Run pipelines on
+Metadata-Version: 2.1 Name: pyTasker Version: 0.6.7 Summary: Run pipelines on
 your own computer for better automation Home-page: https://github.com/
 carlossilva2/pyTasker Author: Carlos Silva Author-email:
 carlos.miguel.silva@protonmail.com License: GPLv3 Project-URL: Source, https://
 github.com/carlossilva2/pyTasker Project-URL: Documentation, https://
 cmsilva.gitbook.io/pytasker/ Platform: UNKNOWN Classifier: Development Status
 :: 4 - Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: GNU General Public License v3
```

### Comparing `pyTasker-0.6.6/pyTasker.egg-info/SOURCES.txt` & `pyTasker-0.6.7/pyTasker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.6/setup.py` & `pyTasker-0.6.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 setup(
     author="Carlos Silva",
     author_email="carlos.miguel.silva@protonmail.com",
     name="pyTasker",
     description="Run pipelines on your own computer for better automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.6.6",
+    version="0.6.7",
     url="https://github.com/carlossilva2/pyTasker",
     packages=find_packages(),
     license="GPLv3",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
```

### Comparing `pyTasker-0.6.6/static/Copy PDFs then zip.png` & `pyTasker-0.6.7/static/Copy PDFs then zip.png`

 * *Files identical despite different names*

### Comparing `pyTasker-0.6.6/static/Copy PDFs.png` & `pyTasker-0.6.7/static/Copy PDFs.png`

 * *Files identical despite different names*

