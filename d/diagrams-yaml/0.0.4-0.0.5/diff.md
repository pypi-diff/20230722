# Comparing `tmp/diagrams-yaml-0.0.4.tar.gz` & `tmp/diagrams-yaml-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diagrams-yaml-0.0.4.tar", last modified: Sat Jul 22 08:42:18 2023, max compression
+gzip compressed data, was "diagrams-yaml-0.0.5.tar", last modified: Sat Jul 22 12:55:08 2023, max compression
```

## Comparing `diagrams-yaml-0.0.4.tar` & `diagrams-yaml-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:42:18.328854 diagrams-yaml-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/.project-version
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-07-22 08:42:18.328854 diagrams-yaml-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:42:18.328854 diagrams-yaml-0.0.4/diagrams_yaml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/diagrams_yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/diagrams_yaml/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/diagrams_yaml/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/diagrams_yaml/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/diagrams_yaml/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:42:18.328854 diagrams-yaml-0.0.4/diagrams_yaml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-07-22 08:42:18.000000 diagrams-yaml-0.0.4/diagrams_yaml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-22 08:42:18.000000 diagrams-yaml-0.0.4/diagrams_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 08:42:18.000000 diagrams-yaml-0.0.4/diagrams_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-22 08:42:18.000000 diagrams-yaml-0.0.4/diagrams_yaml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-22 08:42:18.000000 diagrams-yaml-0.0.4/diagrams_yaml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-22 08:42:18.000000 diagrams-yaml-0.0.4/diagrams_yaml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:42:18.328854 diagrams-yaml-0.0.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/requirements/project.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-22 08:42:18.328854 diagrams-yaml-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-22 08:41:58.000000 diagrams-yaml-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:55:08.857562 diagrams-yaml-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 12:54:48.000000 diagrams-yaml-0.0.5/.project-version
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-22 12:54:48.000000 diagrams-yaml-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-22 12:54:48.000000 diagrams-yaml-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-07-22 12:55:08.857562 diagrams-yaml-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-07-22 12:54:48.000000 diagrams-yaml-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:55:08.857562 diagrams-yaml-0.0.5/diagrams_yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 12:54:48.000000 diagrams-yaml-0.0.5/diagrams_yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-07-22 12:54:48.000000 diagrams-yaml-0.0.5/diagrams_yaml/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-22 12:54:48.000000 diagrams-yaml-0.0.5/diagrams_yaml/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-22 12:54:48.000000 diagrams-yaml-0.0.5/diagrams_yaml/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-22 12:54:48.000000 diagrams-yaml-0.0.5/diagrams_yaml/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:55:08.857562 diagrams-yaml-0.0.5/diagrams_yaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-07-22 12:55:08.000000 diagrams-yaml-0.0.5/diagrams_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-22 12:55:08.000000 diagrams-yaml-0.0.5/diagrams_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 12:55:08.000000 diagrams-yaml-0.0.5/diagrams_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-22 12:55:08.000000 diagrams-yaml-0.0.5/diagrams_yaml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-22 12:55:08.000000 diagrams-yaml-0.0.5/diagrams_yaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-22 12:55:08.000000 diagrams-yaml-0.0.5/diagrams_yaml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-22 12:54:48.000000 diagrams-yaml-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:55:08.857562 diagrams-yaml-0.0.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-22 12:54:48.000000 diagrams-yaml-0.0.5/requirements/project.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-22 12:55:08.861563 diagrams-yaml-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-22 12:54:48.000000 diagrams-yaml-0.0.5/setup.py
```

### Comparing `diagrams-yaml-0.0.4/LICENSE` & `diagrams-yaml-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `diagrams-yaml-0.0.4/diagrams_yaml/entrypoint.py` & `diagrams-yaml-0.0.5/diagrams_yaml/entrypoint.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import sys
 
 import yaml
 from diagrams import (
     Cluster,
     Diagram,
+    Edge,
     Node,
 )
 
 from diagrams_yaml.enums import (
     ServiceResourceType,
     RelationType,
 )
@@ -89,14 +90,17 @@
         })
 
         for relation in resource.relates:
             relationship = Relationship(
                 from_=f'{parent_id}.{resource.id}',
                 to=f'diagram.{relation.to}',
                 type=relation.type,
+                label=relation.label,
+                color=relation.color,
+                style=relation.style,
             )
 
             relationships.append(relationship)
 
         for resource_of in resource.of:
             process_resource(resource=resource_of, parent_id=f'{parent_id}.{resource.id}', group=diagram_group)
 
@@ -111,14 +115,17 @@
         })
 
         for relation in resource.relates:
             relationship = Relationship(
                 from_=f'{parent_id}.{resource.id}',
                 to=f'diagram.{relation.to}',
                 type=relation.type,
+                label=relation.label,
+                color=relation.color,
+                style=relation.style,
             )
 
             relationships.append(relationship)
 
         if group is not None:
             group.add_node(node=resource_instance)
 
@@ -137,53 +144,76 @@
     diagram = YamlDiagram(**diagram_as_dict)
 
     with Diagram(diagram.name, show=diagram.show):
         for resource in diagram.resources:
             process_resource(resource, 'diagram')
 
         for relationship in relationships:
+            edge = Edge(label=relationship.label, color=relationship.color, style=relationship.style)
+
             resource_from_instance = resources.get(relationship.from_)
             resource_to_instance = resources.get(relationship.to)
 
             is_resource_from_node = not isinstance(resource_from_instance, DiagramGroup)
             is_resource_from_group = isinstance(resource_from_instance, DiagramGroup)
 
             is_resource_to_node = not isinstance(resource_to_instance, DiagramGroup)
             is_resource_to_group = isinstance(resource_to_instance, DiagramGroup)
 
             if is_resource_from_node and is_resource_to_node:
                 if relationship.type == RelationType.LEFT:
-                    resource_from_instance.__lshift__(other=resource_to_instance)
+                    resource_from_instance.__lshift__(other=edge)
+                    edge.__lshift__(other=resource_to_instance)
 
                 if relationship.type == RelationType.RIGHT:
-                    resource_from_instance.__rshift__(other=resource_to_instance)
+                    resource_from_instance.__rshift__(other=edge)
+                    edge.__rshift__(other=resource_to_instance)
 
                 if relationship.type == RelationType.UNIDIRECTIONAL:
-                    resource_from_instance.__sub__(other=resource_to_instance)
+                    resource_from_instance.__sub__(other=edge)
+                    edge.__sub__(other=resource_to_instance)
+
+                if relationship.type == RelationType.BOTH:
+                    resource_from_instance.__rshift__(other=edge)
+                    edge.__lshift__(other=resource_to_instance)
 
             if is_resource_from_group and is_resource_to_node:
                 group_nodes = resource_from_instance.get_nodes()
 
                 if relationship.type == RelationType.LEFT:
-                    resource_to_instance.__rlshift__(other=group_nodes)
+                    group_nodes_edges = edge.__rlshift__(other=group_nodes)
+                    resource_to_instance.__rlshift__(other=group_nodes_edges)
 
                 if relationship.type == RelationType.RIGHT:
-                    resource_to_instance.__rrshift__(other=group_nodes)
+                    group_nodes_edges = edge.__rrshift__(other=group_nodes)
+                    resource_to_instance.__rrshift__(other=group_nodes_edges)
 
                 if relationship.type == RelationType.UNIDIRECTIONAL:
-                    resource_to_instance.__sub__(other=group_nodes)
+                    group_nodes_edges = edge.__rsub__(other=group_nodes)
+                    resource_to_instance.__rsub__(other=group_nodes_edges)
+
+                if relationship.type == RelationType.BOTH:
+                    group_nodes_edges = edge.__rrshift__(other=group_nodes)
+                    resource_to_instance.__rlshift__(other=group_nodes_edges)
 
             if is_resource_from_node and is_resource_to_group:
                 group_nodes = resource_to_instance.get_nodes()
 
                 if relationship.type == RelationType.LEFT:
-                    resource_from_instance.__lshift__(other=group_nodes)
+                    resource_from_instance.__lshift__(other=edge)
+                    edge.__lshift__(other=group_nodes)
 
                 if relationship.type == RelationType.RIGHT:
-                    resource_from_instance.__rshift__(other=group_nodes)
+                    resource_from_instance.__rshift__(other=edge)
+                    edge.__rshift__(other=group_nodes)
 
                 if relationship.type == RelationType.UNIDIRECTIONAL:
-                    resource_from_instance.__sub__(other=group_nodes)
+                    resource_from_instance.__sub__(other=edge)
+                    edge.__sub__(other=group_nodes)
+
+                if relationship.type == RelationType.BOTH:
+                    resource_from_instance.__rshift__(other=edge)
+                    edge.__lshift__(other=group_nodes)
 
 
 if __name__ == '__main__':
     entrypoint()
```

### Comparing `diagrams-yaml-0.0.4/diagrams_yaml/resources.py` & `diagrams-yaml-0.0.5/diagrams_yaml/resources.py`

 * *Files identical despite different names*

### Comparing `diagrams-yaml-0.0.4/setup.py` & `diagrams-yaml-0.0.5/setup.py`

 * *Files identical despite different names*

