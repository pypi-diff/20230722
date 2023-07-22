# Comparing `tmp/yandil-0.3.3.tar.gz` & `tmp/yandil-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yandil-0.3.3.tar", max compression
+gzip compressed data, was "yandil-0.4.0.tar", max compression
```

## Comparing `yandil-0.3.3.tar` & `yandil-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1498 2023-07-06 15:41:06.050516 yandil-0.3.3/LICENSE
--rw-r--r--   0        0        0    11594 2023-07-06 15:41:06.050516 yandil-0.3.3/README.md
--rw-r--r--   0        0        0      988 2023-07-06 15:42:15.159197 yandil-0.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/__init__.py
--rw-r--r--   0        0        0      148 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/argument.py
--rw-r--r--   0        0        0        0 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/configuration/__init__.py
--rw-r--r--   0        0        0      800 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/configuration/configuration_container.py
--rw-r--r--   0        0        0      507 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/configuration/environment.py
--rw-r--r--   0        0        0    11387 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/container.py
--rw-r--r--   0        0        0        0 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/declarative/__init__.py
--rw-r--r--   0        0        0      516 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/declarative/decorators.py
--rw-r--r--   0        0        0      799 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/dependency.py
--rw-r--r--   0        0        0     1505 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/dependency_filler.py
--rw-r--r--   0        0        0        0 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/discovery/__init__.py
--rw-r--r--   0        0        0     3653 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/discovery/class_discovery.py
--rw-r--r--   0        0        0      883 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/discovery/module_discovery.py
--rw-r--r--   0        0        0        0 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/errors/__init__.py
--rw-r--r--   0        0        0      246 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/errors/abstract_class_not_allowed_error.py
--rw-r--r--   0        0        0      467 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/errors/configuration_value_type_mismatch_error.py
--rw-r--r--   0        0        0      239 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/errors/dependency_not_found_error.py
--rw-r--r--   0        0        0      279 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/errors/instance_and_class_does_not_match_error.py
--rw-r--r--   0        0        0      257 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/errors/missing_configuration_value_error.py
--rw-r--r--   0        0        0      127 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/errors/missing_type_hint_item_type_error.py
--rw-r--r--   0        0        0      301 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/errors/primary_dependency_already_defined_error.py
--rw-r--r--   0        0        0      243 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/errors/primary_dependency_not_found_error.py
--rw-r--r--   0        0        0        0 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/loaders/__init__.py
--rw-r--r--   0        0        0     1188 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/loaders/declarative_dependency_loader.py
--rw-r--r--   0        0        0     4954 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/loaders/self_discover_dependency_loader.py
--rw-r--r--   0        0        0     1238 2023-07-06 15:41:06.054517 yandil-0.3.3/src/yandil/typing_tools.py
--rw-r--r--   0        0        0    12144 1970-01-01 00:00:00.000000 yandil-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1498 2023-07-22 16:17:01.368250 yandil-0.4.0/LICENSE
+-rw-r--r--   0        0        0    11720 2023-07-22 16:17:01.368250 yandil-0.4.0/README.md
+-rw-r--r--   0        0        0      988 2023-07-22 16:18:09.555567 yandil-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/__init__.py
+-rw-r--r--   0        0        0      148 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/argument.py
+-rw-r--r--   0        0        0        0 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/configuration/__init__.py
+-rw-r--r--   0        0        0      800 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/configuration/configuration_container.py
+-rw-r--r--   0        0        0      507 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/configuration/environment.py
+-rw-r--r--   0        0        0    11387 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/container.py
+-rw-r--r--   0        0        0        0 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/declarative/__init__.py
+-rw-r--r--   0        0        0      516 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/declarative/decorators.py
+-rw-r--r--   0        0        0      799 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/dependency.py
+-rw-r--r--   0        0        0     1505 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/dependency_filler.py
+-rw-r--r--   0        0        0        0 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/discovery/__init__.py
+-rw-r--r--   0        0        0     3653 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/discovery/class_discovery.py
+-rw-r--r--   0        0        0      386 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/discovery/class_feature_checks.py
+-rw-r--r--   0        0        0      883 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/discovery/module_discovery.py
+-rw-r--r--   0        0        0        0 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/errors/__init__.py
+-rw-r--r--   0        0        0      246 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/errors/abstract_class_not_allowed_error.py
+-rw-r--r--   0        0        0      467 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/errors/configuration_value_type_mismatch_error.py
+-rw-r--r--   0        0        0      239 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/errors/dependency_not_found_error.py
+-rw-r--r--   0        0        0      279 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/errors/instance_and_class_does_not_match_error.py
+-rw-r--r--   0        0        0      257 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/errors/missing_configuration_value_error.py
+-rw-r--r--   0        0        0      127 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/errors/missing_type_hint_item_type_error.py
+-rw-r--r--   0        0        0      301 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/errors/primary_dependency_already_defined_error.py
+-rw-r--r--   0        0        0      243 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/errors/primary_dependency_not_found_error.py
+-rw-r--r--   0        0        0        0 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/loaders/__init__.py
+-rw-r--r--   0        0        0     1188 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/loaders/declarative_dependency_loader.py
+-rw-r--r--   0        0        0     5342 2023-07-22 16:17:01.368250 yandil-0.4.0/src/yandil/loaders/self_discover_dependency_loader.py
+-rw-r--r--   0        0        0     1238 2023-07-22 16:17:01.372250 yandil-0.4.0/src/yandil/typing_tools.py
+-rw-r--r--   0        0        0    12270 1970-01-01 00:00:00.000000 yandil-0.4.0/PKG-INFO
```

### Comparing `yandil-0.3.3/LICENSE` & `yandil-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yandil-0.3.3/README.md` & `yandil-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 ```
 
 In order to tune the dependency injection discovery process the loader has the following options:
 - **excluded_modules**: Set of module or package names to be excluded from the dependency injection discovery process. For example for excluding the folder which contains the models in a web application.
 - **should_exclude_classes_without_public_methods**: If set to True, classes which not define any public method will be excluded from the dependency injection discovery process. For example for excluding DTO classes.
 - **should_exclude_dataclasses**: If set to True, dataclasses will be excluded from the dependency injection discovery process.
 - **mandatory_modules**: Set of module paths which classes contained should be loaded as dependencies without checking if they meet any condition.
+- **should_exclude_exceptions**: If set to True, exceptions will be excluded from the dependency injection discovery process.
 
 ### Declarative way
 In this way you will need to decorate the classes which you want to be loaded as dependencies.
 
 Giving the following python project structure:
 ```
 ├── app
```

### Comparing `yandil-0.3.3/pyproject.toml` & `yandil-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yandil"
-version = "0.3.3"
+version = "0.4.0"
 description = "Yet ANother Dependency Injection Library"
 readme = "README.md"
 authors = ["DeejayRevok <seryi_one@hotmail.com>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/DeejayRevok/yandil"
 homepage = "https://github.com/DeejayRevok/yandil"
 keywords = ["dependency injection", "di"]
@@ -34,15 +34,15 @@
 [tool.isort]
 profile = "black"
 py_version=310
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.3.3"
+version = "0.4.0"
 tag_format = "$version"
 version_files = [
   "pyproject.toml:version"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `yandil-0.3.3/src/yandil/configuration/configuration_container.py` & `yandil-0.4.0/src/yandil/configuration/configuration_container.py`

 * *Files identical despite different names*

### Comparing `yandil-0.3.3/src/yandil/container.py` & `yandil-0.4.0/src/yandil/container.py`

 * *Files identical despite different names*

### Comparing `yandil-0.3.3/src/yandil/declarative/decorators.py` & `yandil-0.4.0/src/yandil/declarative/decorators.py`

 * *Files identical despite different names*

### Comparing `yandil-0.3.3/src/yandil/dependency.py` & `yandil-0.4.0/src/yandil/dependency.py`

 * *Files identical despite different names*

### Comparing `yandil-0.3.3/src/yandil/dependency_filler.py` & `yandil-0.4.0/src/yandil/dependency_filler.py`

 * *Files identical despite different names*

### Comparing `yandil-0.3.3/src/yandil/discovery/class_discovery.py` & `yandil-0.4.0/src/yandil/discovery/class_discovery.py`

 * *Files identical despite different names*

### Comparing `yandil-0.3.3/src/yandil/discovery/module_discovery.py` & `yandil-0.4.0/src/yandil/discovery/module_discovery.py`

 * *Files identical despite different names*

### Comparing `yandil-0.3.3/src/yandil/loaders/declarative_dependency_loader.py` & `yandil-0.4.0/src/yandil/loaders/declarative_dependency_loader.py`

 * *Files identical despite different names*

### Comparing `yandil-0.3.3/src/yandil/loaders/self_discover_dependency_loader.py` & `yandil-0.4.0/src/yandil/loaders/self_discover_dependency_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 from ast import ClassDef
-from inspect import getmembers, isfunction
 from pathlib import Path
 from typing import Iterable, Optional, Set, Type
 
 from yandil.container import Container, default_container
 from yandil.discovery.class_discovery import (
     ClassData,
     discover_classes_from_module,
     exclude_abstract_classes,
     exclude_classes_without_public_methods,
     exclude_dataclasses,
     transform_class_nodes_to_class_data,
 )
+from yandil.discovery.class_feature_checks import has_public_methods, is_enum, is_exception
 from yandil.discovery.module_discovery import discover_modules
 
 
 class SelfDiscoverDependencyLoader:
     def __init__(
         self,
         discovery_base_path: str,
         sources_root_path: str,
         container: Optional[Container] = None,
         excluded_modules: Optional[Set[str]] = None,
         should_exclude_classes_without_public_methods: bool = True,
         should_exclude_dataclasses: bool = True,
         mandatory_modules: Optional[Set[Path]] = None,
+        should_exclude_exceptions: bool = True,
     ):
         if container is None:
             container = default_container
         self.__container = container
         self.__excluded_modules = excluded_modules
         self.__should_exclude_classes_without_public_methods = should_exclude_classes_without_public_methods
         self.__should_exclude_dataclasses = should_exclude_dataclasses
         self.__sources_root_path = sources_root_path
         self.__discovery_base_path = discovery_base_path
         if mandatory_modules is None:
             mandatory_modules = set()
         self.__mandatory_modules = mandatory_modules
+        self.__should_exclude_exceptions = should_exclude_exceptions
 
     def load(self) -> None:
         for module_data in discover_modules(self.__discovery_base_path, self.__excluded_modules):
             module_file_path = module_data.module_path + ".py"
 
             classes_without_defined_public_methods: Set[ClassDef] = set()
             if self.__is_module_mandatory(module_data.module_path):
@@ -51,14 +53,16 @@
                     self.__should_exclude_classes_without_public_methods,
                     self.__should_exclude_dataclasses,
                     classes_without_defined_public_methods=classes_without_defined_public_methods,
                 )
 
             for class_data in module_classes:
                 cls = class_data.to_class(self.__sources_root_path)
+                if not self.__class_should_be_added(cls):
+                    continue
                 self.__container.add(cls)
 
             self.__add_classes_without_defined_public_methods_with_public_methods(
                 classes_without_defined_public_methods,
                 module_file_path,
             )
 
@@ -99,12 +103,18 @@
         for class_without_defined_public_methods in transform_class_nodes_to_class_data(
             classes_without_defined_public_methods,
             module_file_path,
         ):
             class_without_defined_public_methods = class_without_defined_public_methods.to_class(
                 self.__sources_root_path
             )
-            if self.__class_has_public_methods(class_without_defined_public_methods):
+            if has_public_methods(class_without_defined_public_methods) and self.__class_should_be_added(
+                class_without_defined_public_methods
+            ):
                 self.__container.add(class_without_defined_public_methods)
 
-    def __class_has_public_methods(self, cls: Type) -> bool:
-        return any(name for name, member in getmembers(cls) if isfunction(member) and not name.startswith("_"))
+    def __class_should_be_added(self, cls: Type) -> bool:
+        if is_enum(cls):
+            return False
+        if self.__should_exclude_exceptions and is_exception(cls):
+            return False
+        return True
```

### Comparing `yandil-0.3.3/src/yandil/typing_tools.py` & `yandil-0.4.0/src/yandil/typing_tools.py`

 * *Files identical despite different names*

### Comparing `yandil-0.3.3/PKG-INFO` & `yandil-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandil
-Version: 0.3.3
+Version: 0.4.0
 Summary: Yet ANother Dependency Injection Library
 Home-page: https://github.com/DeejayRevok/yandil
 License: BSD-3-Clause
 Keywords: dependency injection,di
 Author: DeejayRevok
 Author-email: seryi_one@hotmail.com
 Requires-Python: >=3.10.0,<3.11.0
@@ -89,14 +89,15 @@
 ```
 
 In order to tune the dependency injection discovery process the loader has the following options:
 - **excluded_modules**: Set of module or package names to be excluded from the dependency injection discovery process. For example for excluding the folder which contains the models in a web application.
 - **should_exclude_classes_without_public_methods**: If set to True, classes which not define any public method will be excluded from the dependency injection discovery process. For example for excluding DTO classes.
 - **should_exclude_dataclasses**: If set to True, dataclasses will be excluded from the dependency injection discovery process.
 - **mandatory_modules**: Set of module paths which classes contained should be loaded as dependencies without checking if they meet any condition.
+- **should_exclude_exceptions**: If set to True, exceptions will be excluded from the dependency injection discovery process.
 
 ### Declarative way
 In this way you will need to decorate the classes which you want to be loaded as dependencies.
 
 Giving the following python project structure:
 ```
 ├── app
```

