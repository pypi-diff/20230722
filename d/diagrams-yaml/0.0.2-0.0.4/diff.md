# Comparing `tmp/diagrams-yaml-0.0.2.tar.gz` & `tmp/diagrams-yaml-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diagrams-yaml-0.0.2.tar", last modified: Fri Jul 21 15:12:25 2023, max compression
+gzip compressed data, was "diagrams-yaml-0.0.4.tar", last modified: Sat Jul 22 08:42:18 2023, max compression
```

## Comparing `diagrams-yaml-0.0.2.tar` & `diagrams-yaml-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-21 15:12:25.653851 diagrams-yaml-0.0.2/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        6 2023-07-21 10:51:47.000000 diagrams-yaml-0.0.2/.project-version
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1075 2023-07-21 10:32:46.000000 diagrams-yaml-0.0.2/LICENSE
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       87 2023-07-21 10:33:03.000000 diagrams-yaml-0.0.2/MANIFEST.in
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     4054 2023-07-21 15:12:25.653898 diagrams-yaml-0.0.2/PKG-INFO
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     3237 2023-07-21 15:11:10.000000 diagrams-yaml-0.0.2/README.md
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-21 15:12:25.653027 diagrams-yaml-0.0.2/diagrams_yaml/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-21 08:47:14.000000 diagrams-yaml-0.0.2/diagrams_yaml/__init__.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     4528 2023-07-21 14:22:19.000000 diagrams-yaml-0.0.2/diagrams_yaml/entrypoint.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      206 2023-07-21 14:10:41.000000 diagrams-yaml-0.0.2/diagrams_yaml/enums.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      781 2023-07-21 10:18:15.000000 diagrams-yaml-0.0.2/diagrams_yaml/resources.py
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      842 2023-07-21 10:15:30.000000 diagrams-yaml-0.0.2/diagrams_yaml/schema.py
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-21 15:12:25.653661 diagrams-yaml-0.0.2/diagrams_yaml.egg-info/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     4054 2023-07-21 15:12:25.000000 diagrams-yaml-0.0.2/diagrams_yaml.egg-info/PKG-INFO
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      457 2023-07-21 15:12:25.000000 diagrams-yaml-0.0.2/diagrams_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)        1 2023-07-21 15:12:25.000000 diagrams-yaml-0.0.2/diagrams_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       71 2023-07-21 15:12:25.000000 diagrams-yaml-0.0.2/diagrams_yaml.egg-info/entry_points.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       47 2023-07-21 15:12:25.000000 diagrams-yaml-0.0.2/diagrams_yaml.egg-info/requires.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       14 2023-07-21 15:12:25.000000 diagrams-yaml-0.0.2/diagrams_yaml.egg-info/top_level.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      374 2023-07-21 10:31:27.000000 diagrams-yaml-0.0.2/pyproject.toml
-drwxr-xr-x   0 dmytrostriletskyi   (501) staff       (20)        0 2023-07-21 15:12:25.653762 diagrams-yaml-0.0.2/requirements/
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)       47 2023-07-21 10:35:05.000000 diagrams-yaml-0.0.2/requirements/project.txt
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)      195 2023-07-21 15:12:25.654069 diagrams-yaml-0.0.2/setup.cfg
--rw-r--r--   0 dmytrostriletskyi   (501) staff       (20)     1483 2023-07-21 15:06:40.000000 diagrams-yaml-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:42:18.328854 diagrams-yaml-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/.project-version
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-07-22 08:42:18.328854 diagrams-yaml-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:42:18.328854 diagrams-yaml-0.0.4/diagrams_yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/diagrams_yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/diagrams_yaml/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/diagrams_yaml/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/diagrams_yaml/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/diagrams_yaml/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:42:18.328854 diagrams-yaml-0.0.4/diagrams_yaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-07-22 08:42:18.000000 diagrams-yaml-0.0.4/diagrams_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-22 08:42:18.000000 diagrams-yaml-0.0.4/diagrams_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 08:42:18.000000 diagrams-yaml-0.0.4/diagrams_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-22 08:42:18.000000 diagrams-yaml-0.0.4/diagrams_yaml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-22 08:42:18.000000 diagrams-yaml-0.0.4/diagrams_yaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-22 08:42:18.000000 diagrams-yaml-0.0.4/diagrams_yaml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:42:18.328854 diagrams-yaml-0.0.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/requirements/project.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-22 08:42:18.328854 diagrams-yaml-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/setup.py
```

### Comparing `diagrams-yaml-0.0.2/LICENSE` & `diagrams-yaml-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `diagrams-yaml-0.0.2/PKG-INFO` & `diagrams-yaml-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diagrams-yaml
-Version: 0.0.2
+Version: 0.0.4
 Summary: Diagram as Code in a declarative way using YAML for drawing cloud system architectures.
 Home-page: https://github.com/dmytrostriletskyi/diagrams-yaml
 Author: Dmytro Striletskyi
 Author-email: dmytro.striletskyi@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/dmytrostriletskyi/diagrams-yaml/issues
 Project-URL: Source Code, https://github.com/dmytrostriletskyi/diagrams-yaml
@@ -90,19 +90,19 @@
 
 ## Usage
 
 To draw an architecture, call `diagrams-yaml` command line interface, providing a path to a `YAML` file with 
 configurations:
 
 ```bash
-$ diagrams-yaml examples/web-services-aws-architecture.yaml
+$ diagrams-yaml examples/web-services-aws.yaml
 ```
 
 The drawing will be saved in the folder the command line interface was executed from:
 
 ```bash
 $ ls
 ├── ...
-└── web_services_aws_architecture.png
+└── web_services_aws.png
 ```
```

### Comparing `diagrams-yaml-0.0.2/README.md` & `diagrams-yaml-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -71,17 +71,17 @@
 
 ## Usage
 
 To draw an architecture, call `diagrams-yaml` command line interface, providing a path to a `YAML` file with 
 configurations:
 
 ```bash
-$ diagrams-yaml examples/web-services-aws-architecture.yaml
+$ diagrams-yaml examples/web-services-aws.yaml
 ```
 
 The drawing will be saved in the folder the command line interface was executed from:
 
 ```bash
 $ ls
 ├── ...
-└── web_services_aws_architecture.png
+└── web_services_aws.png
 ```
```

### Comparing `diagrams-yaml-0.0.2/diagrams_yaml/schema.py` & `diagrams-yaml-0.0.4/diagrams_yaml/schema.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 """
 Provide implementation of schemas.
 """
+from __future__ import annotations
+
 from pydantic import BaseModel
 
+from diagrams_yaml.enums import RelationType
+
 
 class YamlDiagram(BaseModel):
     """
     YAML diagram schema implementation.
     """
 
     name: str
     show: bool
-    resources: list['YamlDiagramResource']
+    resources: list[YamlDiagramResource]
 
 
 class YamlDiagramResource(BaseModel):
     """
     YAML diagram resource schema implementation.
     """
 
     id: str | int
     name: str
     type: str
-    of: list['YamlDiagramResource'] | None = []
-    relates: list['YamlDiagramResourceRelationship'] | None = []
+    of: list[YamlDiagramResource] | None = []
+    relates: list[YamlDiagramResourceRelationship] | None = []
 
 
 class YamlDiagramResourceRelationship(BaseModel):
     """
     Yaml diagram resource relationship schema implementation.
     """
 
     to: str
-    type: str
+    type: RelationType
 
 
 class Relationship(BaseModel):
     """
     Relationship schema implementation.
 
     Is used internally between layers and functions.
```

### Comparing `diagrams-yaml-0.0.2/diagrams_yaml.egg-info/PKG-INFO` & `diagrams-yaml-0.0.4/diagrams_yaml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diagrams-yaml
-Version: 0.0.2
+Version: 0.0.4
 Summary: Diagram as Code in a declarative way using YAML for drawing cloud system architectures.
 Home-page: https://github.com/dmytrostriletskyi/diagrams-yaml
 Author: Dmytro Striletskyi
 Author-email: dmytro.striletskyi@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/dmytrostriletskyi/diagrams-yaml/issues
 Project-URL: Source Code, https://github.com/dmytrostriletskyi/diagrams-yaml
@@ -90,19 +90,19 @@
 
 ## Usage
 
 To draw an architecture, call `diagrams-yaml` command line interface, providing a path to a `YAML` file with 
 configurations:
 
 ```bash
-$ diagrams-yaml examples/web-services-aws-architecture.yaml
+$ diagrams-yaml examples/web-services-aws.yaml
 ```
 
 The drawing will be saved in the folder the command line interface was executed from:
 
 ```bash
 $ ls
 ├── ...
-└── web_services_aws_architecture.png
+└── web_services_aws.png
 ```
```

### Comparing `diagrams-yaml-0.0.2/setup.py` & `diagrams-yaml-0.0.4/setup.py`

 * *Files identical despite different names*

