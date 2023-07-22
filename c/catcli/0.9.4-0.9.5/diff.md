# Comparing `tmp/catcli-0.9.4.tar.gz` & `tmp/catcli-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catcli-0.9.4.tar", last modified: Sun May 21 19:02:16 2023, max compression
+gzip compressed data, was "catcli-0.9.5.tar", last modified: Mon Jul 10 09:17:58 2023, max compression
```

## Comparing `catcli-0.9.4.tar` & `catcli-0.9.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:02:16.424508 catcli-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-21 19:01:54.000000 catcli-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-21 19:01:54.000000 catcli-0.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17670 2023-05-21 19:02:16.424508 catcli-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-05-21 19:01:54.000000 catcli-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:02:16.424508 catcli-0.9.4/catcli/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/catalog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12386 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/catcli.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/decomp.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/fuser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/nodeprinter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29990 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/noder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:02:16.424508 catcli-0.9.4/catcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17670 2023-05-21 19:02:16.000000 catcli-0.9.4/catcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-21 19:02:16.000000 catcli-0.9.4/catcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 19:02:16.000000 catcli-0.9.4/catcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-21 19:02:16.000000 catcli-0.9.4/catcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-21 19:02:16.000000 catcli-0.9.4/catcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 19:02:16.000000 catcli-0.9.4/catcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-21 19:01:54.000000 catcli-0.9.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 19:02:16.424508 catcli-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-21 19:01:54.000000 catcli-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:17:58.412301 catcli-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-10 09:17:29.000000 catcli-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 09:17:29.000000 catcli-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17670 2023-07-10 09:17:58.412301 catcli-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-07-10 09:17:29.000000 catcli-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:17:58.412301 catcli-0.9.5/catcli/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-10 09:17:29.000000 catcli-0.9.5/catcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-07-10 09:17:29.000000 catcli-0.9.5/catcli/catalog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12386 2023-07-10 09:17:29.000000 catcli-0.9.5/catcli/catcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-10 09:17:29.000000 catcli-0.9.5/catcli/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-10 09:17:29.000000 catcli-0.9.5/catcli/decomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-10 09:17:29.000000 catcli-0.9.5/catcli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-07-10 09:17:29.000000 catcli-0.9.5/catcli/fuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-10 09:17:29.000000 catcli-0.9.5/catcli/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-10 09:17:29.000000 catcli-0.9.5/catcli/nodeprinter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30317 2023-07-10 09:17:29.000000 catcli-0.9.5/catcli/noder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-07-10 09:17:29.000000 catcli-0.9.5/catcli/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-10 09:17:29.000000 catcli-0.9.5/catcli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-10 09:17:29.000000 catcli-0.9.5/catcli/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-07-10 09:17:29.000000 catcli-0.9.5/catcli/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:17:58.412301 catcli-0.9.5/catcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17670 2023-07-10 09:17:58.000000 catcli-0.9.5/catcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-10 09:17:58.000000 catcli-0.9.5/catcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:17:58.000000 catcli-0.9.5/catcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 09:17:58.000000 catcli-0.9.5/catcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-10 09:17:58.000000 catcli-0.9.5/catcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 09:17:58.000000 catcli-0.9.5/catcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-10 09:17:29.000000 catcli-0.9.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 09:17:58.412301 catcli-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-10 09:17:29.000000 catcli-0.9.5/setup.py
```

### Comparing `catcli-0.9.4/LICENSE` & `catcli-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `catcli-0.9.4/PKG-INFO` & `catcli-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: catcli
-Version: 0.9.4
+Version: 0.9.5
 Summary: The command line catalog tool for your offline data
 Home-page: https://github.com/deadc0de6/catcli
 Author: deadc0de6
 Author-email: deadc0de6@foo.bar
 License: GPLv3
-Download-URL: https://github.com/deadc0de6/catcli/archive/v0.9.4.tar.gz
+Download-URL: https://github.com/deadc0de6/catcli/archive/v0.9.5.tar.gz
 Description: # CATCLI
         
         [![Tests Status](https://github.com/deadc0de6/catcli/workflows/tests/badge.svg?branch=master)](https://github.com/deadc0de6/catcli/actions)
         [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0)
         [![Coveralls](https://img.shields.io/coveralls/github/deadc0de6/catcli)](https://coveralls.io/github/deadc0de6/catcli?branch=master)
         
         [![PyPI version](https://badge.fury.io/py/catcli.svg)](https://badge.fury.io/py/catcli)
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: catcli Version: 0.9.4 Summary: The command line
+Metadata-Version: 2.1 Name: catcli Version: 0.9.5 Summary: The command line
 catalog tool for your offline data Home-page: https://github.com/deadc0de6/
 catcli Author: deadc0de6 Author-email: deadc0de6@foo.bar License: GPLv3
-Download-URL: https://github.com/deadc0de6/catcli/archive/v0.9.4.tar.gz
+Download-URL: https://github.com/deadc0de6/catcli/archive/v0.9.5.tar.gz
 Description: # CATCLI [![Tests Status](https://github.com/deadc0de6/catcli/
 workflows/tests/badge.svg?branch=master)](https://github.com/deadc0de6/catcli/
 actions) [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-
 blue.svg)](http://www.gnu.org/licenses/gpl-3.0) [![Coveralls](https://
 img.shields.io/coveralls/github/deadc0de6/catcli)](https://coveralls.io/github/
 deadc0de6/catcli?branch=master) [![PyPI version](https://badge.fury.io/py/
 catcli.svg)](https://badge.fury.io/py/catcli) [![AUR](https://img.shields.io/
```

### Comparing `catcli-0.9.4/README.md` & `catcli-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `catcli-0.9.4/catcli/catalog.py` & `catcli-0.9.5/catcli/catalog.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 author: deadc0de6 (https://github.com/deadc0de6)
 Copyright (c) 2017, deadc0de6
 
 Class that represents the catcli catalog
 """
 
 import os
-from typing import Optional
-from anytree.exporter import JsonExporter  # type: ignore
+from typing import Optional, List, Dict, Tuple, Union, Any
+from anytree.exporter import JsonExporter, DictExporter  # type: ignore
 from anytree.importer import JsonImporter  # type: ignore
+from anytree import AnyNode  # type: ignore
 
 # local imports
 from catcli import nodes
 from catcli.nodes import NodeMeta, NodeTop
 from catcli.utils import ask
 from catcli.logger import Logger
 
@@ -25,15 +26,15 @@
                  force: bool = False) -> None:
         """
         @path: catalog path
         @usepickle: use pickle
         @debug: debug mode
         @force: force overwrite if exists
         """
-        self.path = path
+        self.path = os.path.expanduser(path)
         self.debug = debug
         self.force = force
         self.metanode: Optional[NodeMeta] = None
 
     def set_metanode(self, metanode: NodeMeta) -> None:
         """remove the metanode until tree is re-written"""
         self.metanode = metanode
@@ -81,25 +82,77 @@
         if not self.debug:
             return
         Logger.debug(text)
 
     def _save_json(self, top: NodeTop) -> bool:
         """export the catalog in json"""
         self._debug(f'saving {top} to json...')
-        exp = JsonExporter(indent=2, sort_keys=True)
+        dexporter = DictExporter(attriter=attriter)
+        exp = JsonExporter(dictexporter=dexporter, indent=2, sort_keys=True)
         with open(self.path, 'w', encoding='UTF-8') as file:
             exp.write(top, file)
         self._debug(f'Catalog saved to json \"{self.path}\"')
         return True
 
     def _restore_json(self, string: str) -> Optional[NodeTop]:
         """restore the tree from json"""
-        imp = JsonImporter()
+        imp = JsonImporter(dictimporter=_DictImporter(debug=self.debug))
         self._debug('import from string...')
         root = imp.import_(string)
         self._debug(f'Catalog imported from json \"{self.path}\"')
         self._debug(f'root imported: {root}')
         if root.type != nodes.TYPE_TOP:
             return None
         top = NodeTop(root.name, children=root.children)
         self._debug(f'top imported: {top}')
         return top
+
+
+class _DictImporter():
+
+    def __init__(self,
+                 nodecls: AnyNode = AnyNode,
+                 debug: bool = False):
+        self.nodecls = nodecls
+        self.debug = debug
+
+    def import_(self, data: Dict[str, str]) -> AnyNode:
+        """Import tree from `data`."""
+        return self.__import(data)
+
+    def __import(self, data: Union[str, Any],
+                 parent: AnyNode = None) -> AnyNode:
+        """overwrite parent imoprt"""
+        assert isinstance(data, dict)
+        assert "parent" not in data
+        attrs = dict(data)
+        # replace attr
+        attrs = back_attriter(attrs, debug=self.debug)
+        children: Union[str, Any] = attrs.pop("children", [])
+        node = self.nodecls(parent=parent, **attrs)
+        for child in children:
+            self.__import(child, parent=node)
+        return node
+
+
+def back_attriter(adict: Dict[str, str],
+                  debug: bool = False) -> Dict[str, str]:
+    """replace attribute on json restore"""
+    attrs = {}
+    for k, val in adict.items():
+        if k == 'size':
+            if debug:
+                Logger.debug(f'changing {k}={val}')
+            k = 'nodesize'
+        attrs[k] = val
+    return attrs
+
+
+def attriter(attrs: List[Tuple[str, Any]]) -> List[Tuple[str, Any]]:
+    """replace attribute on json save"""
+    newattr = []
+    for attr in attrs:
+        k, val = attr
+        if k == 'nodesize':
+            k = 'size'
+        newattr.append((k, val))
+    return newattr
```

### Comparing `catcli-0.9.4/catcli/catcli.py` & `catcli-0.9.5/catcli/catcli.py`

 * *Files identical despite different names*

### Comparing `catcli-0.9.4/catcli/colors.py` & `catcli-0.9.5/catcli/colors.py`

 * *Files identical despite different names*

### Comparing `catcli-0.9.4/catcli/decomp.py` & `catcli-0.9.5/catcli/decomp.py`

 * *Files identical despite different names*

### Comparing `catcli-0.9.4/catcli/fuser.py` & `catcli-0.9.5/catcli/fuser.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,39 +70,39 @@
     def _getattr(self, path: str) -> Dict[str, Any]:
         entry = self._get_entry(path)
         if not entry:
             return {}
 
         maccess = time()
         mode: Any = S_IFREG
-        size: int = 0
+        nodesize: int = 0
         if entry.type == nodes.TYPE_ARCHIVED:
             mode = S_IFREG
-            size = entry.size
+            nodesize = entry.nodesize
         elif entry.type == nodes.TYPE_DIR:
             mode = S_IFDIR
-            size = entry.size
+            nodesize = entry.nodesize
             maccess = entry.maccess
         elif entry.type == nodes.TYPE_FILE:
             mode = S_IFREG
-            size = entry.size
+            nodesize = entry.nodesize
             maccess = entry.maccess
         elif entry.type == nodes.TYPE_STORAGE:
             mode = S_IFDIR
-            size = entry.size
+            nodesize = entry.nodesize
             maccess = entry.ts
         elif entry.type == nodes.TYPE_META:
             mode = S_IFREG
         elif entry.type == nodes.TYPE_TOP:
             mode = S_IFREG
         mode = mode | 0o777
         return {
             'st_mode': (mode),  # file type
             'st_nlink': 1,  # count hard link
-            'st_size': size,
+            'st_size': nodesize,
             'st_ctime': maccess,  # attr last modified
             'st_mtime': maccess,  # content last modified
             'st_atime': maccess,  # access time
             'st_uid': os.getuid(),
             'st_gid': os.getgid(),
         }
```

### Comparing `catcli-0.9.4/catcli/logger.py` & `catcli-0.9.5/catcli/logger.py`

 * *Files identical despite different names*

### Comparing `catcli-0.9.4/catcli/nodeprinter.py` & `catcli-0.9.5/catcli/nodeprinter.py`

 * *Files identical despite different names*

### Comparing `catcli-0.9.4/catcli/noder.py` & `catcli-0.9.5/catcli/noder.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,37 +134,39 @@
     def rec_size(self, node: Union[NodeDir, NodeStorage],
                  store: bool = True) -> int:
         """
         recursively traverse tree and return size
         @store: store the size in the node
         """
         if node.type == nodes.TYPE_FILE:
-            self._debug(f'size of {node.type} \"{node.name}\": {node.size}')
-            return node.size
+            node.__class__ = NodeFile
+            msg = f'size of {node.type} \"{node.name}\": {node.nodesize}'
+            self._debug(msg)
+            return node.nodesize
         msg = f'getting node size recursively for \"{node.name}\"'
         self._debug(msg)
-        size: int = 0
+        fullsize: int = 0
         for i in node.children:
             if node.type == nodes.TYPE_DIR:
                 sub_size = self.rec_size(i, store=store)
                 if store:
-                    i.size = sub_size
-                size += sub_size
+                    i.nodesize = sub_size
+                fullsize += sub_size
                 continue
             if node.type == nodes.TYPE_STORAGE:
                 sub_size = self.rec_size(i, store=store)
                 if store:
-                    i.size = sub_size
-                size += sub_size
+                    i.nodesize = sub_size
+                fullsize += sub_size
                 continue
             self._debug(f'skipping {node.name}')
         if store:
-            node.size = size
-        self._debug(f'size of {node.type} \"{node.name}\": {size}')
-        return size
+            node.nodesize = fullsize
+        self._debug(f'size of {node.type} \"{node.name}\": {fullsize}')
+        return fullsize
 
     ###############################################################
     # public helpers
     ###############################################################
     @staticmethod
     def attrs_to_string(attr: Union[List[str], Dict[str, str], str]) -> str:
         """format the storage attr for saving"""
@@ -257,15 +259,15 @@
                            self.attrs_to_string(attrs),
                            parent=parent)
 
     def new_archive_node(self, name: str, path: str,
                          parent: str, archive: str) -> NodeArchived:
         """create a new node for archive data"""
         return NodeArchived(name=name, relpath=path,
-                            parent=parent, size=0, md5='',
+                            parent=parent, nodesize=0, md5='',
                             archive=archive)
 
     ###############################################################
     # node management
     ###############################################################
     def update_metanode(self, top: NodeTop) -> NodeMeta:
         """create or update meta node information"""
@@ -347,15 +349,15 @@
             out.append(node.name.replace('"', '""'))  # name
             out.append(node.type)  # type
             parents = self._get_parents(node)
             storage = self._get_storage(node)
             fullpath = os.path.join(storage.name, parents)
             out.append(fullpath.replace('"', '""'))  # full path
 
-            out.append(size_to_str(node.size, raw=raw))  # size
+            out.append(size_to_str(node.nodesize, raw=raw))  # size
             out.append(epoch_to_str(storage.ts))  # indexed_at
             if self._has_attr(node, 'maccess'):
                 out.append(epoch_to_str(node.maccess))  # maccess
             else:
                 out.append('')  # fake maccess
             if self._has_attr(node, 'md5'):
                 out.append(node.md5)  # md5
@@ -388,57 +390,61 @@
         @withdepth: print the node depth info
         @withstorage: print the node storage it belongs to
         @recalcparent: get relpath from tree instead of relpath field
         @raw: print raw size rather than human readable
         """
         if node.type == nodes.TYPE_TOP:
             # top node
+            node.__class__ = NodeTop
             Logger.stdout_nocolor(f'{pre}{node.name}')
         elif node.type == nodes.TYPE_FILE:
             # node of type file
+            node.__class__ = NodeFile
             name = node.name
             if withpath:
                 if recalcparent:
                     name = os.sep.join([self._get_parents(node.parent), name])
                 else:
                     name = node.relpath
             name = name.lstrip(os.sep)
             if withstorage:
                 storage = self._get_storage(node)
             attr_str = ''
             if node.md5:
                 attr_str = f', md5:{node.md5}'
-            size = size_to_str(node.size, raw=raw)
+            size = size_to_str(node.nodesize, raw=raw)
             compl = f'size:{size}{attr_str}'
             if withstorage:
                 content = Logger.get_bold_text(storage.name)
                 compl += f', storage:{content}'
             NodePrinter.print_file_native(pre, name, compl)
         elif node.type == nodes.TYPE_DIR:
             # node of type directory
+            node.__class__ = NodeDir
             name = node.name
             if withpath:
                 if recalcparent:
                     name = os.sep.join([self._get_parents(node.parent), name])
                 else:
                     name = node.relpath
             name = name.lstrip(os.sep)
             depth = 0
             if withdepth:
                 depth = len(node.children)
             if withstorage:
                 storage = self._get_storage(node)
             attr: List[Tuple[str, str]] = []
-            if node.size:
-                attr.append(('totsize', size_to_str(node.size, raw=raw)))
+            if node.nodesize:
+                attr.append(('totsize', size_to_str(node.nodesize, raw=raw)))
             if withstorage:
                 attr.append(('storage', Logger.get_bold_text(storage.name)))
             NodePrinter.print_dir_native(pre, name, depth=depth, attr=attr)
         elif node.type == nodes.TYPE_STORAGE:
             # node of type storage
+            node.__class__ = NodeStorage
             sztotal = size_to_str(node.total, raw=raw)
             szused = size_to_str(node.total - node.free, raw=raw)
             nbchildren = len(node.children)
             pcent = 0
             if node.total > 0:
                 pcent = node.free * 100 / node.total
             freepercent = f'{pcent:.1f}%'
@@ -463,14 +469,15 @@
             argsstring = ' | '.join(args)
             NodePrinter.print_storage_native(pre,
                                              name,
                                              argsstring,
                                              node.attr)
         elif node.type == nodes.TYPE_ARCHIVED:
             # archive node
+            node.__class__ = NodeArchived
             if self.arc:
                 NodePrinter.print_archive_native(pre, node.name, node.archive)
         else:
             Logger.err(f'bad node encountered: {node}')
 
     def print_tree(self, node: NodeAny,
                    fmt: str = 'native',
@@ -771,17 +778,17 @@
         """sorting nodes dir first and alpha"""
         return (node.type, node.name.lstrip('.').lower())
 
     @staticmethod
     def _sort_size(node: NodeAny) -> float:
         """sorting nodes by size"""
         try:
-            if not node.size:
+            if not node.nodesize:
                 return 0
-            return float(node.size)
+            return float(node.nodesize)
         except AttributeError:
             return 0
 
     def _get_storage(self, node: NodeAny) -> NodeStorage:
         """recursively traverse up to find storage"""
         if node.type == nodes.TYPE_STORAGE:
             return node
```

### Comparing `catcli-0.9.4/catcli/nodes.py` & `catcli-0.9.5/catcli/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,25 +80,25 @@
 
 class NodeFile(NodeAny):
     """a file node"""
 
     def __init__(self,  # type: ignore[no-untyped-def]
                  name: str,
                  relpath: str,
-                 size: int,
+                 nodesize: int,
                  md5: str,
                  maccess: float,
                  parent=None,
                  children=None):
         """build a file node"""
         super().__init__()  # type: ignore[no-untyped-call]
         self.name = name
         self.type = TYPE_FILE
         self.relpath = relpath
-        self.size = size
+        self.nodesize = nodesize
         self.md5 = md5
         self.maccess = maccess
         self.parent = parent
         if children:
             self.children = children
 
     def __str__(self) -> str:
@@ -107,24 +107,24 @@
 
 class NodeDir(NodeAny):
     """a directory node"""
 
     def __init__(self,  # type: ignore[no-untyped-def]
                  name: str,
                  relpath: str,
-                 size: int,
+                 nodesize: int,
                  maccess: float,
                  parent=None,
                  children=None):
         """build a directory node"""
         super().__init__()  # type: ignore[no-untyped-call]
         self.name = name
         self.type = TYPE_DIR
         self.relpath = relpath
-        self.size = size
+        self.nodesize = nodesize
         self.maccess = maccess
         self.parent = parent
         if children:
             self.children = children
 
     def __str__(self) -> str:
         return self._to_str()
@@ -132,25 +132,25 @@
 
 class NodeArchived(NodeAny):
     """an archived node"""
 
     def __init__(self,  # type: ignore[no-untyped-def]
                  name: str,
                  relpath: str,
-                 size: int,
+                 nodesize: int,
                  md5: str,
                  archive: str,
                  parent=None,
                  children=None):
         """build an archived node"""
         super().__init__()  # type: ignore[no-untyped-call]
         self.name = name
         self.type = TYPE_ARCHIVED
         self.relpath = relpath
-        self.size = size
+        self.nodesize = nodesize
         self.md5 = md5
         self.archive = archive
         self.parent = parent
         if children:
             self.children = children
 
     def __str__(self) -> str:
@@ -160,27 +160,27 @@
 class NodeStorage(NodeAny):
     """a storage node"""
 
     def __init__(self,  # type: ignore[no-untyped-def]
                  name: str,
                  free: int,
                  total: int,
-                 size: int,
+                 nodesize: int,
                  ts: float,
                  attr: str,
                  parent=None,
                  children=None):
         """build a storage node"""
         super().__init__()  # type: ignore[no-untyped-call]
         self.name = name
         self.type = TYPE_STORAGE
         self.free = free
         self.total = total
         self.attr = attr
-        self.size = size
+        self.nodesize = nodesize
         self.ts = ts  # pylint: disable=C0103
         self.parent = parent
         if children:
             self.children = children
 
     def __str__(self) -> str:
         return self._to_str()
```

### Comparing `catcli-0.9.4/catcli/utils.py` & `catcli-0.9.5/catcli/utils.py`

 * *Files identical despite different names*

### Comparing `catcli-0.9.4/catcli/walker.py` & `catcli-0.9.5/catcli/walker.py`

 * *Files identical despite different names*

### Comparing `catcli-0.9.4/catcli.egg-info/PKG-INFO` & `catcli-0.9.5/catcli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: catcli
-Version: 0.9.4
+Version: 0.9.5
 Summary: The command line catalog tool for your offline data
 Home-page: https://github.com/deadc0de6/catcli
 Author: deadc0de6
 Author-email: deadc0de6@foo.bar
 License: GPLv3
-Download-URL: https://github.com/deadc0de6/catcli/archive/v0.9.4.tar.gz
+Download-URL: https://github.com/deadc0de6/catcli/archive/v0.9.5.tar.gz
 Description: # CATCLI
         
         [![Tests Status](https://github.com/deadc0de6/catcli/workflows/tests/badge.svg?branch=master)](https://github.com/deadc0de6/catcli/actions)
         [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0)
         [![Coveralls](https://img.shields.io/coveralls/github/deadc0de6/catcli)](https://coveralls.io/github/deadc0de6/catcli?branch=master)
         
         [![PyPI version](https://badge.fury.io/py/catcli.svg)](https://badge.fury.io/py/catcli)
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: catcli Version: 0.9.4 Summary: The command line
+Metadata-Version: 2.1 Name: catcli Version: 0.9.5 Summary: The command line
 catalog tool for your offline data Home-page: https://github.com/deadc0de6/
 catcli Author: deadc0de6 Author-email: deadc0de6@foo.bar License: GPLv3
-Download-URL: https://github.com/deadc0de6/catcli/archive/v0.9.4.tar.gz
+Download-URL: https://github.com/deadc0de6/catcli/archive/v0.9.5.tar.gz
 Description: # CATCLI [![Tests Status](https://github.com/deadc0de6/catcli/
 workflows/tests/badge.svg?branch=master)](https://github.com/deadc0de6/catcli/
 actions) [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-
 blue.svg)](http://www.gnu.org/licenses/gpl-3.0) [![Coveralls](https://
 img.shields.io/coveralls/github/deadc0de6/catcli)](https://coveralls.io/github/
 deadc0de6/catcli?branch=master) [![PyPI version](https://badge.fury.io/py/
 catcli.svg)](https://badge.fury.io/py/catcli) [![AUR](https://img.shields.io/
```

### Comparing `catcli-0.9.4/setup.py` & `catcli-0.9.5/setup.py`

 * *Files identical despite different names*

