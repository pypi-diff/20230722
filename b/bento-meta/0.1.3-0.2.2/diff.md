# Comparing `tmp/bento_meta-0.1.3.tar.gz` & `tmp/bento_meta-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bento_meta-0.1.3.tar", max compression
+gzip compressed data, was "bento_meta-0.2.2.tar", max compression
```

## Comparing `bento_meta-0.1.3.tar` & `bento_meta-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0    11446 2020-10-16 17:49:04.916483 bento_meta-0.1.3/LICENSE
--rw-r--r--   0        0        0      157 2020-10-16 17:49:04.917102 bento_meta-0.1.3/README.md
--rw-r--r--   0        0        0     2197 2023-05-23 18:53:13.654125 bento_meta-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       70 2023-02-08 23:10:38.928433 bento_meta-0.1.3/src/bento_meta/__init__.py
--rw-r--r--   0        0        0    22569 2023-02-12 23:42:52.167649 bento_meta-0.1.3/src/bento_meta/entity.py
--rw-r--r--   0        0        0      502 2023-02-12 23:42:52.168386 bento_meta-0.1.3/src/bento_meta/logs/log.ini
--rw-r--r--   0        0        0      388 2023-02-08 23:10:38.930201 bento_meta-0.1.3/src/bento_meta/mdb/__init__.py
--rw-r--r--   0        0        0     8997 2023-05-23 18:53:13.655094 bento_meta-0.1.3/src/bento_meta/mdb/loaders.py
--rw-r--r--   0        0        0    13412 2023-02-08 23:10:38.931335 bento_meta-0.1.3/src/bento_meta/mdb/mdb.py
--rw-r--r--   0        0        0       89 2023-02-08 23:10:38.932332 bento_meta-0.1.3/src/bento_meta/mdb/mdb_tools/__init__.py
--rw-r--r--   0        0        0    28784 2023-02-08 23:10:38.933304 bento_meta-0.1.3/src/bento_meta/mdb/mdb_tools/mdb_tools.py
--rw-r--r--   0        0        0     3616 2023-02-08 23:10:38.933480 bento_meta-0.1.3/src/bento_meta/mdb/searchable.py
--rw-r--r--   0        0        0     2426 2023-02-08 23:10:38.934620 bento_meta-0.1.3/src/bento_meta/mdb/writeable.py
--rw-r--r--   0        0        0    19629 2023-05-23 18:53:13.656567 bento_meta-0.1.3/src/bento_meta/model.py
--rw-r--r--   0        0        0    25896 2023-02-08 23:10:38.936099 bento_meta-0.1.3/src/bento_meta/object_map.py
--rw-r--r--   0        0        0    10465 2023-02-12 23:30:19.090576 bento_meta-0.1.3/src/bento_meta/objects.py
--rw-r--r--   0        0        0      196 2023-02-08 23:10:38.940527 bento_meta-0.1.3/src/bento_meta/util/__init__.py
--rw-r--r--   0        0        0    15507 2023-02-08 23:10:38.941405 bento_meta-0.1.3/src/bento_meta/util/_engine.py
--rw-r--r--   0        0        0       87 2023-02-08 23:10:38.942242 bento_meta-0.1.3/src/bento_meta/util/cypher/__init__.py
--rw-r--r--   0        0        0     7427 2023-02-08 23:10:38.943782 bento_meta-0.1.3/src/bento_meta/util/cypher/clauses.py
--rw-r--r--   0        0        0    19302 2023-02-08 23:10:38.944679 bento_meta-0.1.3/src/bento_meta/util/cypher/entities.py
--rw-r--r--   0        0        0     2067 2023-02-08 23:10:38.945608 bento_meta-0.1.3/src/bento_meta/util/cypher/functions.py
--rw-r--r--   0        0        0    24424 2022-02-25 15:35:38.969950 bento_meta-0.1.3/src/bento_meta/util/cypher.py.old
--rw-r--r--   0        0        0     2532 2023-02-08 23:10:38.946393 bento_meta-0.1.3/src/bento_meta/util/makeq.py
--rw-r--r--   0        0        0     4910 2022-01-28 18:56:52.458052 bento_meta-0.1.3/src/bento_meta/util/query_paths.yml
--rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 bento_meta-0.1.3/setup.py
--rw-r--r--   0        0        0     1231 1970-01-01 00:00:00.000000 bento_meta-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11446 2023-07-21 22:20:26.966968 bento_meta-0.2.2/LICENSE
+-rw-r--r--   0        0        0      157 2023-07-21 22:20:26.966968 bento_meta-0.2.2/README.md
+-rw-r--r--   0        0        0     2772 2023-07-21 22:20:26.970968 bento_meta-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    10416 2023-07-21 22:20:26.970968 bento_meta-0.2.2/scripts/compare_models.py
+-rw-r--r--   0        0        0     5809 2023-07-21 22:20:26.970968 bento_meta-0.2.2/scripts/compare_val_set_terms.py
+-rw-r--r--   0        0        0    15577 2023-07-21 22:20:26.970968 bento_meta-0.2.2/scripts/make_diff_changelog.py
+-rw-r--r--   0        0        0    10021 2023-07-21 22:20:26.970968 bento_meta-0.2.2/scripts/make_mapping_changelog.py
+-rw-r--r--   0        0        0    11554 2023-07-21 22:20:26.970968 bento_meta-0.2.2/scripts/make_model_changelog.py
+-rw-r--r--   0        0        0       70 2023-07-21 22:20:26.970968 bento_meta-0.2.2/src/bento_meta/__init__.py
+-rw-r--r--   0        0        0    23264 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/entity.py
+-rw-r--r--   0        0        0      502 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/logs/log.ini
+-rw-r--r--   0        0        0      388 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/mdb/__init__.py
+-rw-r--r--   0        0        0     8997 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/mdb/loaders.py
+-rw-r--r--   0        0        0    13439 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/mdb/mdb.py
+-rw-r--r--   0        0        0       89 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/mdb/mdb_tools/__init__.py
+-rw-r--r--   0        0        0    31805 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/mdb/mdb_tools/mdb_tools.py
+-rw-r--r--   0        0        0     3606 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/mdb/searchable.py
+-rw-r--r--   0        0        0     2426 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/mdb/writeable.py
+-rw-r--r--   0        0        0    19629 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/model.py
+-rw-r--r--   0        0        0    26098 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/object_map.py
+-rw-r--r--   0        0        0    11048 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/objects.py
+-rw-r--r--   0        0        0      196 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/util/__init__.py
+-rw-r--r--   0        0        0    15507 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/util/_engine.py
+-rw-r--r--   0        0        0       87 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/util/cypher/__init__.py
+-rw-r--r--   0        0        0     9414 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/util/cypher/clauses.py
+-rw-r--r--   0        0        0    19302 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/util/cypher/entities.py
+-rw-r--r--   0        0        0     2067 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/util/cypher/functions.py
+-rw-r--r--   0        0        0     2532 2023-07-21 22:20:26.974968 bento_meta-0.2.2/src/bento_meta/util/makeq.py
+-rw-r--r--   0        0        0     1341 1970-01-01 00:00:00.000000 bento_meta-0.2.2/PKG-INFO
```

### Comparing `bento_meta-0.1.3/LICENSE` & `bento_meta-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bento_meta-0.1.3/pyproject.toml` & `bento_meta-0.2.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bento-meta"
-version = "0.1.3"
+version = "0.2.2"
 description = "Python drivers for Bento Metamodel Database"
 authors = [
   { name="Mark A. Jensen", email = "mark.jensen@nih.gov"},
   { name="Mark Benson", email = "mark.benson@nih.gov"},
   { name="Nelson Moore", email = "nelson.moore@essential-soft.com"}
 ]
 requires-python = ">=3.8"
@@ -16,53 +16,63 @@
 
 [project.urls]
 "Homepage" = "https://cbiit.github.io/bento-meta/"
 "Bug Tracker" = "https://github.com/CBIIT/bento-meta/issues"
 
 [tool.poetry]
 name = "bento-meta"
-version = "0.1.3"
+version = "0.2.2"
 description = "Python drivers for Bento Metamodel Database"
 authors = [
     "Mark A. Jensen <mark.jensen@nih.gov>",
     "Mark Benson <mark.benson@nih.gov>",
     "Nelson Moore <nelson.moore@essential-soft.com>"
 ]
 license = "Apache 2.0"
 readme = "README.md"
 include = ["logs/log.ini"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-PyYAML = ">=6"
+PyYAML = ">=6.0.1"
 delfick-project = "^0.7.9"
 neo4j = ">=4.0"
 nanoid = "^2.0.0"
 requests = "^2.28.1"
 tqdm = "^4.64.1"
 setuptools = "^65.4.1"
 numpy = {version = "^1.23.5", optional = true}
 pandas = {version = "^1.5.2", optional = true}
 spacy = {version = "^3.4.3", optional = true}
 click = {version = "^8.1.3", optional = true}
-#scispacy = {version = "^0.5.1", optional = true}
+liquichange = "^0.2.1"
+bento-mdf = "^0.9.1"
 
 [tool.poetry.extras]
-Tools = ["click", "numpy", "pandas", "spacy"] #"scispacy",
+Tools = ["click", "numpy", "pandas", "spacy", "liquichange"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
-# docker-compose = {version = "^1.29.2", optional = true}
 pytest-docker = "^1.0.1"
 requests = "^2.28.1"
 myst-nb = {version = "^0.17.1", python = "^3.8"}
 sphinx-autoapi = "^2.0.1"
 sphinx-rtd-theme = "^1.1.1"
 python-semantic-release = "^7.33.0"
 pytest-cov = "^4.0.0"
+liquichange = "^0.2.1"
+sphinx = "5.3.0"
+bento-mdf = "^0.9.1"
+
+[tool.poetry.scripts]
+"compare_models" = { reference = "scripts/compare_models.py", type = "file", extras = ["click", "spacy", "pandas"]}
+"compare_val_set_terms" = { reference = "scripts/compare_val_set_terms.py", type = "file", extras = ["click", "pandas"] }
+"make_model_changelog" = {reference = "scripts/make_model_changelog.py", type = "file", extras = ["click", "liquichange"]}
+"make_diff_changelog" = {reference = "scripts/make_diff_changelog.py", type = "file", extras = ["click", "liquichange"]}
+"make_mapping_changelog" = {reference = "scripts/make_mapping_changelog.py", type = "file", extras = ["click", "liquichange"]}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = "pyproject.toml:version"
@@ -70,9 +80,9 @@
 changelog_file = "CHANGELOG.md"
 build_command = "poetry build"
 dist_path = "dist/"
 upload_to_release = true
 upload_to_pypi = false
 remove_dist = false
 patch_without_tag = true
-major_on_zero = false # while major version on 0.y.z, won't bump to 1.0.0
-version_source = "tag" # temp?
+major_on_zero = false
+version_source = "tag"
```

### Comparing `bento_meta-0.1.3/src/bento_meta/entity.py` & `bento_meta-0.2.2/src/bento_meta/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 =================
 
 This module contains 
 * `Entity`, the base class for metamodel objects, 
 * the `CollValue` class to manage collection-valued attributes, and 
 * the `ArgError` exception.
 """
+from collections import UserDict
+
 # from pdb import set_trace
 from warnings import warn
-from collections import UserDict
 
 
 class ArgError(Exception):
     """Exception for method argument errors"""
+
     pass
 
 
 class Entity(object):
     """Base class for all metamodel objects.
 
     Entity contains all the magic for metamodel objects such as
@@ -28,24 +30,25 @@
 
     The Entity class also defines private and declared attributes that are
     common to all metamodel objects. It provides the machinery to manage
     private attributes separately from declared attributes, and to raise
     exceptions when attempts are made to access attributes that are not
     declared.
     """
+
     pvt_attr = [
         "pvt",
         "neoid",
         "dirty",
         "removed_entities",
         "attspec",
         "mapspec",
         "belongs",
     ]
-    defaults = {},
+    defaults = ({},)
     attspec_ = {
         "_id": "simple",
         "nanoid": "simple",
         "desc": "simple",
         "_next": "object",
         "_prev": "object",
         "_from": "simple",
@@ -53,17 +56,22 @@
         "_commit": "simple",
         "tags": "collection",
     }
     attspec = attspec_
     mapspec_ = {
         "label": None,
         "key": "_id",
-        "property": {"_id": "id", "desc": "desc",
-                     "_from": "_from", "_to": "_to",
-                     "_commit": "_commit", "nanoid": "nanoid"},
+        "property": {
+            "_id": "id",
+            "desc": "desc",
+            "_from": "_from",
+            "_to": "_to",
+            "_commit": "_commit",
+            "nanoid": "nanoid",
+        },
         "relationship": {
             "_next": {"rel": ":_next>", "end_cls": set()},
             "_prev": {"rel": ":_prev>", "end_cls": set()},
             "tags": {"rel": ":has_tag", "end_cls": {"Tag"}},
         },
     }
     object_map = None
@@ -139,27 +147,26 @@
     @classmethod
     def default(cls, propname):
         """Returns a default value for the property named, or None if no default defined."""
         if cls.defaults.get(propname):
             return cls.defaults[propname]
         else:
             return None
-        
 
     # @classmethod
     def get_by_id(self, id):
         """Get an object from the db with the id attribute (not the Neo4j id). Returns a new object.
         :param string id: value of id for desired object
         """
         if self.object_map:
-            print('  > now in entity.get_by_id where self is {}'.format(self))
-            print('  > and class is {}'.format(self.__class__))
+            print("  > now in entity.get_by_id where self is {}".format(self))
+            print("  > and class is {}".format(self.__class__))
             return self.object_map.get_by_id(self, id)
         else:
-            print('    _NO_ cls.object_map detected')
+            print("    _NO_ cls.object_map detected")
             pass
 
     @property
     def dirty(self):
         """Flag whether this instance has been changed since retrieval from
         the database
         Set to -1, ensure that the next time an attribute is accessed, the instance
@@ -429,16 +436,16 @@
                     del getattr(owner, att[0])[att[1]]
                 else:
                     setattr(owner, att[0], None)
 
     def dget(self, refresh=False):
         """Update self from the database
         :param boolean refresh: if True, force a retrieval from db;
-            if False, retrieve from cache;
-            don't disrupt changes already made
+        if False, retrieve from cache;
+        don't disrupt changes already made
         """
         if type(self).object_map:
             return type(self).object_map.get(self, refresh)
         else:
             pass
 
     def dput(self):
@@ -502,27 +509,50 @@
 """.format(
                 att=cls.__name__.lower() + "." + att,
                 obj=str_for_obj(cls.mapspec_["relationship"][att]["end_cls"]),
             )
         doc += "\n"
         return doc
 
+    def get_label(self) -> str:
+        """returns type of entity as label"""
+        return self.mapspec_["label"]
+
+    def get_attr_dict(self):
+        """
+        Returns given entity's set attributes as a dictionary.
+
+        Dictionary of attributes used as the parameters
+        of methods with the write_txn decorator.
+        """
+        attr_dict = {}
+        for key, val in vars(self).items():
+            if (
+                val
+                and val is not None
+                and key != "pvt"
+                and isinstance(val, (str, int, float, complex, bool))
+            ):
+                attr_dict[key] = str(val)
+        return attr_dict
+
 
 class CollValue(UserDict):
     """A UserDict for housing Entity collection attributes.
     This class contains a hook for recording the Entity that
     owns the value that is being set. The value is marked as belonging
     to the *containing object*, not this collection object.
     It also protects against adding arbitrarily typed elements to the
     collection; it throws unless a value to set is an `Entity`. `__setitem__`
     is instrumented for managing versioning.
 
     :param owner: `Entity` object of which this collection is an attribute
     :param owner_key: the attribute name of this collection on the owner
     """
+
     def __init__(self, init=None, *, owner, owner_key):
         self.__dict__["__owner"] = owner
         self.__dict__["__owner_key"] = owner_key
         super().__init__(init)
 
     @property
     def owner(self):
```

### Comparing `bento_meta-0.1.3/src/bento_meta/mdb/loaders.py` & `bento_meta-0.2.2/src/bento_meta/mdb/loaders.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.1.3/src/bento_meta/mdb/mdb.py` & `bento_meta-0.2.2/src/bento_meta/mdb/mdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 class MDB:
     def __init__(self, uri=os.environ.get("NEO4J_MDB_URI"),
                  user=os.environ.get("NEO4J_MDB_USER"),
                  password=os.environ.get("NEO4J_MDB_PASS")):
         self.uri = uri
         self.user = user
         self.password = password
+        self.driver = None
         try:
             self.driver = GraphDatabase.driver(self.uri,
                                                auth=(self.user, self.password))
         except Exception as e:
             warn("MDB not connected: {}".format(e))
         self._txfns = {}
         """ Create an :class:`MDB` object, with a connection to a Neo4j instance of a metamodel database.
```

### Comparing `bento_meta-0.1.3/src/bento_meta/mdb/mdb_tools/mdb_tools.py` & `bento_meta-0.2.2/src/bento_meta/mdb/mdb_tools/mdb_tools.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,637 +1,662 @@
 """
 ToolsMDB: subclass of 'WriteableMDB' to support interactions with the MDB.
-"""
 
-from pathlib import Path
+EntityValidator: validates that entities have required attributes.
+"""
 import csv
-from typing import List
 import logging
+from importlib.util import find_spec
 from logging.config import fileConfig
+from pathlib import Path
+from subprocess import check_call
+from sys import executable
+from typing import Dict, Iterable, List, Optional, Set, Tuple, Type, Union
 
-import spacy
-from nanoid import generate
 from bento_meta.entity import Entity
-from bento_meta.mdb import read_txn, read_txn_data, read_txn_value
+from bento_meta.mdb import make_nanoid, read_txn_data, read_txn_value
 from bento_meta.mdb.writeable import WriteableMDB, write_txn
-from bento_meta.objects import Concept, Predicate, Property, Term
-from bento_meta.util.cypher.clauses import Match, Return, Statement
-from bento_meta.util.cypher.entities import N, VarLenR, NoDirT
+from bento_meta.objects import (
+    Concept,
+    Edge,
+    Node,
+    Predicate,
+    Property,
+    Tag,
+    Term,
+    ValueSet,
+)
+from bento_meta.util.cypher.clauses import (
+    As,
+    Collect,
+    DetachDelete,
+    Match,
+    Merge,
+    OptionalMatch,
+    Return,
+    Statement,
+    With,
+)
+from bento_meta.util.cypher.entities import N0, R0, G, N, P, R, T, _plain_var
+from bento_meta.util.cypher.functions import count
 
 # logging stuff
 log_ini_path = Path(__file__).parents[2].joinpath("logs/log.ini")
 log_file_path = Path(__file__).parents[2].joinpath(f"logs/{__name__}.log")
-fileConfig(log_ini_path, defaults={'logfilename': log_file_path.as_posix()})
+fileConfig(log_ini_path, defaults={"logfilename": log_file_path.as_posix()})
 logger = logging.getLogger(__name__)
 
 
-class EntNotFoundError(Exception):
-    """Raised when an entity is not found and shouldn't be created"""
-
-
-def get_entity_type(entity: Entity):
-    """returns type of entity"""
-    if entity.__class__.__name__.lower() == "edge":
-        return "relationship"
-    return entity.__class__.__name__.lower()
-
-
 class ToolsMDB(WriteableMDB):
     """Adds mdb-tools to WriteableMDB"""
 
     def __init__(self, uri, user, password):
         WriteableMDB.__init__(self, uri, user, password)
 
-    # FIXME: this should interpolate cypher $parameters, not the actual
-    # values
-    # (use utils.cypher...)
-    def get_entity_attrs(self, entity: Entity, output_str: bool = True):
-        """
-        Returns attributes as str or dict for given entity.
-
-        Param output_as_str parm defaults to True and returns a string
-        that is usable in Cypher query as node properties.
-
-        If output_as_str = False, return dict of attributes instead,
-        which is used as params of function with write_txn decorator.
-        """
-        attr_dict = {}
-        for key, val in vars(entity).items():
-            if val and val is not None and key != "pvt":
-                attr_dict[key] = val
-
-        attr_str = "{"
-        for key, val in attr_dict.items():
-            attr_str += f"{key}: '{val}', "
-        attr_str = attr_str[:-2]
-        attr_str += "}"
-
-        if not output_str:
-            return attr_dict
-        return attr_str
+    class EntityNotUniqueError(Exception):
+        """Raised when an entity's attributes identify more than 1 property graph node in an MDB"""
 
-    @write_txn
-    def detach_delete_entity(self, entity: Entity) -> tuple:
-        """
-        Remove given Entity node from the database.
+    class EntityNotFoundError(Exception):
+        """Raised when an entity's attributes fail to identify a property graph node in an MDB"""
 
-        Accepts the following bento-meta Entities:
-            Concept, Node, Predicate, Property, Edge, Term
+    class PatternNotUniqueError(Exception):
+        """
+        Raised when a match pattern's attributes identify more than 1
+        property graph triple or set of overlapping triples in an MDB
         """
-        entity_type = get_entity_type(entity)
-        entity_attr_str = self.get_entity_attrs(entity)
-        entity_attr_dict = self.get_entity_attrs(entity, output_str=False)
-
-        qry = f"MATCH (e:{entity_type} " f"{entity_attr_str}) DETACH DELETE e"
 
-        logging.info(f"Removing {entity_type} node with with properties: {entity_attr_str}")
-        return (qry, entity_attr_dict)
+    class PatternNotFoundError(Exception):
+        """
+        Raised when a match pattern's attributes fail to identify
+        a property graph triple or set of overlapping triples in an MDB
+        """
 
     @read_txn_value
-    def get_entity_count(self, entity: Entity) -> tuple:
+    def _get_entity_count(self, entity: Entity):
         """
-        Returns count of given entity (w/ its properties) found in MDB.
+        Returns count of given entity found in an MDB.
 
-        If count = 0, entity with given properties not found in MDB.
-        If count = 1, entity with given properties is unique in MDB
-        If count > 1, more properties needed to uniquely id entity in MDB.
-        """
-        # if not (term.origin_name and term.value):
-        #     raise RuntimeError("arg 'term' must have both origin_name and value")
-        entity_type = get_entity_type(entity)
-        if entity.nanoid:
-            entity_attr_str = "{nanoid:$nanoid}"
-            entity_attr_dict = {"nanoid": entity.nanoid}
-        else:
-            entity_attr_str = self.get_entity_attrs(entity)
-            entity_attr_dict = self.get_entity_attrs(entity, output_str=False)
+        If count = 0, entity with given attributes not found in MDB.
+        If count = 1, entity with given attributes is unique in MDB
+        If count > 1, more attributes needed to uniquely id entity in MDB.
+        """
+        ent = N(label=entity.get_label(), props=entity.get_attr_dict())
 
-        qry = (
-            f"MATCH (e:{entity_type} {entity_attr_str}) "
-            "RETURN COUNT(e) as entity_count"
+        stmt = Statement(
+            Match(ent),
+            Return(count(ent.var)),
+            As("entity_count"),
+            use_params=True,
         )
 
-        return (qry, entity_attr_dict, "entity_count")
+        qry = str(stmt)
+        parms = stmt.params
+
+        return (qry, parms, "entity_count")
 
     @read_txn_value
-    def get_triple_count(
-        self,
-        src_entity: Entity,
-        dst_entity: Entity,
-        relationship: str,
-    ) -> tuple:
+    def _get_pattern_count(self, pattern: Union[T, G]):
+        """
+        Returns count of given match pattern, which could be a triple like:
+        (n)-[r]->(m), or a set of overlapping triples (Path) found in MDB.
+
+        If count = 0, pattern with given attributes not found in MDB.
+        If count = 1, pattern with given attributes is unique in MDB
+        If count > 1, more attributes needed to uniquely id pattern in MDB.
+        """
+        stmt = Statement(
+            Match(pattern), Return(count("*")), As("pattern_count"), use_params=True
+        )
+
+        qry = str(stmt)
+        parms = stmt.params
+
+        return (qry, parms, "pattern_count")
+
+    def validate_entity_unique(self, entity: Entity) -> None:
         """
-        Returns count of given triple, (src)-[rel]->(dst), found in MDB.
+        Validates that the given entity occurs once (& only once) in an MDB
+
+        Raises EntityNotUniqueError if entity attributes match multiple property
+            graph nodes in the MDB.
+
+        Raises EntityNotFoundError if entity attributes don't match any in the MDB.
 
-        If count = 0, triple with given properties not found in MDB.
-        If count = 1, triple with given properties is unique in MDB
-        If count > 1, more properties needed to uniquely id triple in MDB.
+        Note: doesn't validate the entity itself because not all entity attibutes
+            necessarily required to locate an entity in the MDB.
+            (e.g. handle and model OR nanoid alone can identify a node)
         """
-        src_entity_type = get_entity_type(src_entity)
-        dst_entity_type = get_entity_type(dst_entity)
 
-        qry = (
-            "MATCH (s:{src_type} {{nanoid:$src_nano}}) "
-            "-[:{relationship}]->"
-            "(d:{dst_type} {{nanoid: $dst_nano}}) "
-            "RETURN COUNT(*) as triple_count".format(
-                src_type=src_entity_type,
-                dst_type=dst_entity_type,
-                relationship=relationship,
+        ent_count = int(self._get_entity_count(entity)[0])
+        if ent_count > 1:
+            logger.error(str(self.EntityNotUniqueError))
+            raise self.EntityNotUniqueError
+        if ent_count < 1:
+            logger.error(str(self.EntityNotFoundError))
+            raise self.EntityNotFoundError
+
+    def validate_entities_unique(self, entities: Iterable[Entity]) -> None:
+        """Runs self.validate_entity_unique() over multiple entities"""
+        for entity in entities:
+            self.validate_entity_unique(entity)
+
+    def validate_pattern_unique(self, pattern: Union[T, G]) -> None:
+        """
+        Validates that the given match pattern occurs once (& only once) in an MDB
+
+        Raises PatternNotUniqueError if entity attributes match multiple property
+        graph nodes in the MDB.
+
+        Raises PatternNotFoundError if entity attributes don't match any in the MDB.
+        """
+        pattern_count = int(self._get_pattern_count(pattern)[0])
+        if pattern_count > 1:
+            logger.error(
+                str(
+                    self.PatternNotUniqueError(
+                        f"Pattern: {pattern.pattern()} not unique."
+                    )
+                )
             )
-        )
+            raise self.PatternNotUniqueError(
+                f"Pattern: {pattern.pattern()} not unique."
+            )
+        if pattern_count < 1:
+            logger.error(
+                str(
+                    self.PatternNotFoundError(
+                        f"Pattern: {pattern.pattern()} not found."
+                    )
+                )
+            )
+            raise self.PatternNotFoundError(f"Pattern: {pattern.pattern()} not found.")
 
-        parms = {
-            "src_nano": src_entity.nanoid,
-            "dst_nano": dst_entity.nanoid,
-        }
+    @write_txn
+    def remove_entity_from_mdb(self, entity: Entity):
+        """
+        Remove given Entity node from the database.
+
+        Accepts the following bento-meta Entities:
+            Concept, Node, Predicate, Property, Edge, Term
+        """
+        self.validate_entity_unique(entity)
+
+        ent_label = entity.get_label()
+        ent_attrs = entity.get_attr_dict()
 
-        return (qry, parms, "triple_count")
+        ent = N(label=ent_label, props=ent_attrs)
+
+        stmt = Statement(Match(ent), DetachDelete(ent.var), use_params=True)
+
+        qry = str(stmt)
+        parms = stmt.params
+
+        logging.info(f"Removing {ent_label} entity with with properties: {ent_attrs}")
+        return (qry, parms)
 
     @write_txn
-    def create_entity(
+    def add_entity_to_mdb(
         self,
         entity: Entity,
         _commit=None,
-    ) -> tuple:
-        """Adds given Entity node to database"""
-        if not entity.nanoid:
-            logging.error("entity has no nanoid")
-            raise RuntimeError(
-                "Entity needs a nanoid before creating - please set valid entity nanoid. "
-                "entity_name.nanoid = mdb_name.get_or_make_nano(entity_name) AFTER "
-                "declaring some other entity properties is a good way to do this."
-            )
+    ):
+        """Adds given Entity node to MDB instance"""
+        EntityValidator.validate_entity(entity)
+        EntityValidator.validate_entity_has_attribute(entity, "nanoid")
+
         if _commit:
             entity._commit = _commit
-        entity_type = get_entity_type(entity)
-        entity_attr_str = self.get_entity_attrs(entity)
-        entity_attr_dict = self.get_entity_attrs(entity, output_str=False)
 
-        qry = f"MERGE (e:{entity_type} {entity_attr_str})"
+        ent_label = entity.get_label()
+        ent_attrs = entity.get_attr_dict()
+
+        ent = N(label=ent_label, props=ent_attrs)
+
+        if isinstance(entity, Edge):
+            src = N(label="node", props=entity.src.get_attr_dict())
+            dst = N(label="node", props=entity.dst.get_attr_dict())
+            src_rel = R(Type="has_src")
+            dst_rel = R(Type="has_dst")
+            src_trip = src_rel.relate(_plain_var(ent), _plain_var(src))
+            dst_trip = dst_rel.relate(_plain_var(ent), _plain_var(dst))
+            stmt = Statement(
+                Merge(ent),
+                Merge(src),
+                Merge(dst),
+                Merge(src_trip),
+                Merge(dst_trip),
+                use_params=True,
+            )
+        else:
+            stmt = Statement(Merge(ent), use_params=True)
 
-        logging.info(f"Creating new {entity_type} node with properties: {entity_attr_str}")
-        return (qry, entity_attr_dict)
+        qry = str(stmt)
+        parms = stmt.params
+
+        logging.info(
+            f"Merging new {ent_label} node with properties: {ent_attrs} into the MDB"
+        )
+
+        return (qry, parms)
 
     @read_txn_value
-    def get_concepts(self, entity: Entity):
-        """Returns list of concepts represented by given entity"""
-        # if not (term.origin_name and term.value):
-        #     raise RuntimeError("arg 'term' must have both origin_name and value")
-        entity_type = get_entity_type(entity)
-
-        if entity.nanoid:
-            entity_attr_str = "{nanoid:$nanoid}"
-            entity_attr_dict = {"nanoid": entity.nanoid}
+    def get_concept_nanoids_linked_to_entity(
+        self, entity: Entity, mapping_source: Optional[str] = None
+    ):
+        """
+        Returns list of concept nanoids linked to given entity by
+        "represents" or "has_concept" relationships tagged with
+        the given mapping source.
+        """
+        self.validate_entity_unique(entity)
+
+        ent = N(label=entity.get_label(), props=entity.get_attr_dict())
+        concept = N(label="concept")
+        if isinstance(entity, Term):
+            rel = R(Type="represents")
         else:
-            entity_attr_str = self.get_entity_attrs(entity)
-            entity_attr_dict = self.get_entity_attrs(entity, output_str=False)
+            rel = R(Type="has_concept")
+        ent_trip = rel.relate(ent, concept)
 
-        if entity_type == "term":
-            qry = (
-                f"MATCH (e:{entity_type} {entity_attr_str}) "
-                "-[:represents]->(c:concept) RETURN c.nanoid AS concept"
+        if mapping_source is not None:
+            tag = N(
+                label="tag",
+                props={"key": "mapping_source", "value": mapping_source},
             )
+            tag_trip = T(concept, R(Type="has_tag"), tag)
+            path = G(ent_trip, tag_trip)
         else:
-            qry = (
-                f"MATCH (e:{entity_type} {entity_attr_str}) "
-                "-[:has_concept]->(c:concept) RETURN c.nanoid AS concept"
-            )
-        return (qry, entity_attr_dict, "concept")
+            path = ent_trip
+
+        stmt = Statement(
+            Match(path),
+            Return(f"{concept.var}.nanoid"),
+            As("concept_nanoids"),
+            use_params=True,
+        )
+
+        qry = str(stmt)
+        parms = stmt.params
+        logging.debug(f"{qry=}; {parms=}")
+
+        return (qry, parms, "concept_nanoids")
 
     @write_txn
-    def create_relationship(
+    def add_relationship_to_mdb(
         self,
+        relationship_type: str,
         src_entity: Entity,
         dst_entity: Entity,
-        relationship: str,
-        _commit=None,
+        _commit: str = "",
     ):
-        """Adds relationship between given entities in MDB"""
-        # gets number of entities in MDB matching given entity (w/ given properties)
-        ent_1_count = self.get_entity_count(src_entity)[0]
-        ent_2_count = self.get_entity_count(dst_entity)[0]
-        # at least one of the given entities doesn't uniquely id a node in the MDB.
-        if ent_1_count > 1 or ent_2_count > 1:
-            logging.error("Given attributes don't uniquely identify MDB entities.")
-            raise RuntimeError(
-                "Given entities must uniquely identify nodes in the MDB. Please add "
-                "necessary properties to the entity so that it can be uniquely identified."
-            )
-        # at least one of given entities not found and shouldn't be added
-        if ent_1_count < 1 or ent_2_count < 1:
-            logging.error("One or more of the given entities aren't in the MDB.")
-            raise RuntimeError("One or more of the given entities aren't in the MDB.")
-        src_entity_type = get_entity_type(src_entity)
-        dst_entity_type = get_entity_type(dst_entity)
-
-        src_attr_str = self.get_entity_attrs(src_entity)
-        dst_attr_str = self.get_entity_attrs(dst_entity)
-        _commit_str = ""
-        if _commit:
-            _commit_str = f"{{_commit:'{_commit}'}}"
+        """
+        Adds relationship between given entities in MDB.
+        """
+        self.validate_entities_unique([src_entity, dst_entity])
 
-        # check if triple (ent1)-[relationship]-(ent2) already exists
-        trip_count = self.get_triple_count(
-            src_entity=src_entity,
-            dst_entity=dst_entity,
-            relationship=relationship,
-        )[0]
-
-        if trip_count > 1:
-            logging.error("Relationship exists more than once")
-            raise RuntimeError(
-                "This relationship exists more than once, check the MDB "
-                "instance as this shouldn't be the case."
-            )
-        elif trip_count == 1:
-            logging.warning(
-                f"{relationship} relationship already exists between src {src_entity_type} with "
-                f"properties: {src_attr_str} to dst {dst_entity_type} with properties: {dst_attr_str}"
-            )
-            # way to exit out of decorator? maybe can fix w/ upcoming cypher.utils integration
-            # for now removing commit str before merging (which won't create an extra relationship)
-            qry = (
-                "MATCH (s:{src_type} {{nanoid:$src_nano}}), "
-                "(d:{dst_type} {{nanoid: $dst_nano}}) "
-                "MERGE (s)-[:{relationship}]->(d)".format(
-                    src_type=src_entity_type,
-                    dst_type=dst_entity_type,
-                    relationship=relationship,
-                )
-            )
-            parms = {
-                "src_nano": src_entity.nanoid,
-                "dst_nano": dst_entity.nanoid,
-            }
-            return (qry, parms)
-
-        qry = (
-            "MATCH (s:{src_type} {{nanoid:$src_nano}}), "
-            "(d:{dst_type} {{nanoid: $dst_nano}}) "
-            "MERGE (s)-[:{relationship} {commit}]->(d)".format(
-                src_type=src_entity_type,
-                dst_type=dst_entity_type,
-                relationship=relationship,
-                commit=_commit_str,
-            )
-        )
+        rel = R(Type=relationship_type)
+
+        src = N(label=src_entity.get_label(), props=src_entity.get_attr_dict())
+        dst = N(label=dst_entity.get_label(), props=dst_entity.get_attr_dict())
+        trip = rel.relate(src, dst)
+        plain_trip = rel.relate(_plain_var(src), _plain_var(dst))
+
+        try:
+            # check for existance shouldn't include _commit?
+            self.validate_pattern_unique(trip)
+        except self.PatternNotFoundError:
+            # if triple doesn't already exist, add _commit? this means that
+            # if triple exists w/ different _commit, merge shouldn't add anything?
+            rel.props["_commit"] = P(handle="_commit", value=_commit)
+
+        stmt = Statement(Match(src, dst), Merge(plain_trip), use_params=True)
+
+        qry = str(stmt)
+        parms = stmt.params
+
+        print(stmt)
 
-        parms = {
-            "src_nano": src_entity.nanoid,
-            "dst_nano": dst_entity.nanoid,
-        }
         logging.info(
-            f"Adding {relationship} relationship between src {src_entity_type} with "
-            f"properties: {src_attr_str} to dst {dst_entity_type} with properties: {dst_attr_str}"
+            f"Adding {relationship_type} relationship between src {src.label} with "
+            f"properties: {src_entity.get_attr_dict()} to dst {dst.label} "
+            f"with properties: {dst_entity.get_attr_dict()}"
         )
         return (qry, parms)
 
     def link_synonyms(
         self,
         entity_1: Entity,
         entity_2: Entity,
-        add_missing_ent_1: bool = False,
-        add_missing_ent_2: bool = False,
-        _commit=None,
-    ):
+        mapping_source: str,
+        _commit: str = "",
+    ) -> None:
         """
         Link two synonymous entities in the MDB via a Concept node.
 
         This function takes two synonymous Entities (as determined by user/SME) as
         bento-meta objects connects them to a Concept node via a 'represents' relationship.
 
-        If one or both doesn't exist in the MDB and add_missing_ent is True they will be added.
-
-        If one or both doesn't uniquely identify a node in the MDB will give error.
+        Entities must both exist in the MDB instance and given entity attributes must
+        uniquely identify property graph nodes in the MDB.
 
         If _commit is set (to a string), the _commit property of any node created is set to
         this value.
         """
-        # gets number of entities in MDB matching given entity (w/ given properties)
-        ent_1_count = self.get_entity_count(entity_1)[0]
-        ent_2_count = self.get_entity_count(entity_2)[0]
-        # at least one of the given entities doesn't uniquely id a node in the MDB.
-        if ent_1_count > 1 or ent_2_count > 1:
-            logging.error("Given entities don't uniquely identify MDB entities")
-            raise RuntimeError(
-                "Given entities must uniquely identify nodes in the MDB. Please add "
-                "necessary properties to the entity so that it can be uniquely identified."
-            )
-        # entity 1 not found and shouldn't be added
-        if ent_1_count < 1 and not add_missing_ent_1:
-            logging.error("Entity 1 isn't in the MDB and add_missing_ent_1 is False.")
-            raise EntNotFoundError(
-                "Entity 1 isn't in the MDB and add_missing_ent_1 is False."
-                "Please add the missing entity to the MDB or set add_missing_ent_1 to True."
-            )
-        # entity 2 not found and shouldn't be added
-        if ent_2_count < 1 and not add_missing_ent_2:
-            logging.error("Entity 2 isn't in the MDB and add_missing_ent_2 is False.")
-            raise EntNotFoundError(
-                "Entity 2 isn't in the MDB and add_missing_ent_2 is False."
-                "Please add the missing entity to the MDB or set add_missing_ent_2 to True."
-            )
-        # entity 1 not found and should be added
-        if not ent_1_count and add_missing_ent_1:
-            self.create_entity(entity_1, _commit=_commit)
-        # entity 2 not found and should be added
-        if not ent_2_count and add_missing_ent_2:
-            self.create_entity(entity_2, _commit=_commit)
-        # get any existing concepts and create new concept if none found
-        ent_1_concepts = self.get_concepts(entity_1)
-        ent_2_concepts = self.get_concepts(entity_2)
+        self.validate_entities_unique([entity_1, entity_2])
+
+        ent_1_concepts = self.get_concept_nanoids_linked_to_entity(
+            entity=entity_1, mapping_source=mapping_source
+        )
+        ent_2_concepts = self.get_concept_nanoids_linked_to_entity(
+            entity=entity_2, mapping_source=mapping_source
+        )
+        shared_concepts = list(set(ent_1_concepts).intersection(ent_2_concepts))
+
+        # has concept been tagged by this mapping src before
+        if shared_concepts:
+            logging.warning(
+                f"This mapping has already been added by this source via "
+                f"Concept with nanoid: {shared_concepts[0]}"
+            )
+            return
+
+        # one of the entities has a concept created by the given mapping source
         if ent_1_concepts:
+            logging.info(f"Using existing concept with nanoid {ent_1_concepts[0]}")
             concept = Concept({"nanoid": ent_1_concepts[0]})
         elif ent_2_concepts:
+            logging.info(f"Using existing concept with nanoid {ent_2_concepts[0]}")
             concept = Concept({"nanoid": ent_2_concepts[0]})
         else:
-            concept = Concept({"nanoid": self.make_nano()})
-            self.create_entity(concept, _commit=_commit)
-        # entities are already connected by a concept
-        if not set(ent_1_concepts).isdisjoint(set(ent_2_concepts)):
-            concept = set(ent_1_concepts).intersection(set(ent_2_concepts))
-            logging.warning(f"Both entities are already connected via Concept {list(concept)[0]}")
-            return
-        # create specified relationship between each entity and a concept
-        if get_entity_type(entity_1) == "term":
-            self.create_relationship(entity_1, concept, "represents", _commit=_commit)
-            self.create_relationship(entity_2, concept, "represents", _commit=_commit)
-        else:
-            self.create_relationship(entity_1, concept, "has_concept", _commit=_commit)
-            self.create_relationship(entity_2, concept, "has_concept", _commit=_commit)
-
-    def make_nano(self):
-        """Generates valid nanoid"""
-        return generate(
-            size=6,
-            alphabet="abcdefghijkmnopqrstuvwxyzABCDEFGHJKMNPQRSTUVWXYZ0123456789",
-        )
+            concept = Concept({"nanoid": make_nanoid()})
+            self.add_entity_to_mdb(concept, _commit=_commit)
+            self.add_tag_to_mdb_entity(
+                tag=Tag(
+                    {
+                        "key": "mapping_source",
+                        "value": mapping_source,
+                        "nanoid": make_nanoid(),
+                    }
+                ),
+                entity=concept,
+            )
 
-    def _get_prop_nano(self, prop: Entity, node_handle: str):
-        """
-        Takes Property and Node entities and returns Property nanoid.
+        # create specified relationship between each entity and a concept
+        rel_type_1 = "represents" if isinstance(entity_1, Term) else "has_concept"
+        rel_type_2 = "represents" if isinstance(entity_2, Term) else "has_concept"
 
-        This is used to help uniquely identify a property node in the MDB,
-        which requires a node connected via the has_property relationship.
-        """
-        qry = (
-            "MATCH (p:property {handle:$prop_handle, model: $prop_model})"
-            "<-[:has_property]-(n:node {handle: $node_handle}) "
-            "RETURN p.nanoid as prop_nano"
+        self.add_relationship_to_mdb(
+            relationship_type=rel_type_1,
+            src_entity=entity_1,
+            dst_entity=concept,
+            _commit=_commit,
+        )
+        self.add_relationship_to_mdb(
+            relationship_type=rel_type_2,
+            src_entity=entity_2,
+            dst_entity=concept,
+            _commit=_commit,
         )
-        parms = {
-            "prop_handle": prop.handle,
-            "prop_model": prop.model,
-            "node_handle": node_handle,
-        }
-        return (qry, parms, "prop_nano")
 
-    def _get_edge_nano(self, edge: Entity, src_handle: str, dst_handle: str):
+    @read_txn_value
+    def get_entity_nanoid(self, entity: Entity):
         """
-        Takes Edge, src node handle, and dst Node handle and returns Edge nanoid.
-
-        This is used to help uniquely identify an edge node in the MDB,
-        which requires nodes connected via the has_src and has_dst relationships.
+        Takes a unique entity in the MDB and returns its nanoid.
         """
-        qry = (
-            "MATCH (s:node {handle: $src_handle})<-[:has_src]-"
-            "(r:relationship {handle: $edge_handle, model: $edge_model})-"
-            "[:has_dst]->(d:node {handle: $dst_handle}) "
-            "RETURN r.nanoid as edge_nano"
-        )
-        parms = {
-            "edge_handle": edge.handle,
-            "edge_model": edge.model,
-            "src_handle": src_handle,
-            "dst_handle": dst_handle,
-        }
-        return (qry, parms, "edge_nano")
+        self.validate_entity_unique(entity)
 
-    @read_txn_value
-    def get_entity_nano(
-        self, entity: Entity, extra_handle_1: str = "", extra_handle_2: str = ""
-    ) -> tuple:
-        """
-        Takes an entity and returns its nanoid. If entity requires handles of connected nodes
-        for unique identification (Property or Edge), extra_handle_1 and _2 hold these as str.
-
-        Note: If an entity exists in the MDB with the given properties, but doesn't have an
-        assigned nanoid for some reason, returns [None] instead of [].
-        """
-        ent_type = get_entity_type(entity)
-        if ent_type == "property":
-            if not extra_handle_1:
-                logging.error("Property entity doesn't have connected node handle")
-                raise RuntimeError(
-                    "Property entities require the handle of a node connected via 'has_property' "
-                    "for unique identification. Set 'extra_handle_1' to that node handle str."
-                )
-            return self._get_prop_nano(prop=entity, node_handle=extra_handle_1)
-        if ent_type == "relationship":
-            if not extra_handle_1 or not extra_handle_2:
-                logging.error("Edge entity doesn't have src or dst node handle")
-                raise RuntimeError(
-                    "Edge entities require the handles of a node connected via "
-                    "'has_src' relationship and of a node connected via 'has_dst' "
-                    "relationship for unique identification. Set 'extra_handle_1' to "
-                    "the src handle and 'extra_handle_2' to the dst handle"
-                )
-            return self._get_edge_nano(
-                edge=entity, src_handle=extra_handle_1, dst_handle=extra_handle_2
-            )
+        ent = N(label=entity.get_label(), props=entity.get_attr_dict())
 
-        ent_count = self.get_entity_count(entity)[0]
-        if ent_count > 1:
-            logging.error("Given entities don't uniquely identify MDB entities")
-            raise RuntimeError(
-                "Given entities must uniquely identify nodes in the MDB. Please add "
-                "necesary properties to the entity so that it can be uniquely identified."
-            )
-        # if ent_count < 1:
-        #     raise RuntimeError("Given entity wasn't found in the MDB")
+        if isinstance(entity, Edge):
+            src = N(label="node", props=entity.src.get_attr_dict())
+            dst = N(label="node", props=entity.dst.get_attr_dict())
+            src_rel = R(Type="has_src")
+            dst_rel = R(Type="has_dst")
+            src_trip = src_rel.relate(ent, src)
+            dst_trip = dst_rel.relate(ent, dst)
+            path = G(src_trip, dst_trip)
+            match_clause = Match(path)
+        else:
+            match_clause = Match(ent)
 
-        ent_attr_str = self.get_entity_attrs(entity)
-        ent_attr_dict = self.get_entity_attrs(entity, output_str=False)
+        stmt = Statement(
+            match_clause,
+            Return(f"{ent.var}.nanoid"),
+            As("entity_nanoid"),
+            use_params=True,
+        )
 
-        qry = f"MATCH (e:{ent_type} {ent_attr_str}) RETURN e.nanoid as ent_nano"
+        qry = str(stmt)
+        parms = stmt.params
 
-        return (qry, ent_attr_dict, "ent_nano")
+        return (qry, parms, "entity_nanoid")
 
-    def get_or_make_nano(
-        self, entity: Entity, extra_handle_1: str = "", extra_handle_2: str = ""
-    ) -> str:
+    def get_or_make_entity_nanoid(self, entity: Entity) -> str:
         """Obtains existing entity's nanoid or creates one for new entity."""
-        nano_list = self.get_entity_nano(entity, extra_handle_1, extra_handle_2)
-        if len(nano_list) > 1:
-            logging.error("Given entity doesn't uniquely identify MDB entities")
-            raise RuntimeError(
-                "More than one entity exists with these properties. Please "
-                "add more properties of the desired entity to uniquely ID."
-            )
-        elif nano_list and not nano_list[0]:
-            logging.error("Entity exists but doesn't have nanoid")
-            raise RuntimeError(
-                "An entity with these properties exists in the MDB but doesn't "
-                "have an assigned nanoid for some reason."
-            )
-        elif nano_list:
-            nano = nano_list[0]
-            return nano
-        nano = self.make_nano()
-        return nano
+        try:
+            return self.get_entity_nanoid(entity)[0]
+        except self.EntityNotFoundError:
+            nanoid = make_nanoid()
+            return nanoid
 
     @read_txn_value
-    def get_term_nanos(self, concept: Concept):
+    def get_term_nanoids(self, concept: Concept, mapping_source: str = ""):
         """Returns list of term nanoids representing given concept"""
-        if not concept.nanoid:
-            logging.error("Concept doesn't have a nanoid")
-            raise RuntimeError("arg 'concept' must have nanoid")
-        entity_attr_str = self.get_entity_attrs(concept)
-        entity_attr_dict = self.get_entity_attrs(concept, output_str=False)
-        qry = (
-            f"MATCH (t:term)-[:represents]->(c:concept {entity_attr_str}) "
-            "RETURN t.nanoid AS term_nano"
+        self.validate_entity_unique(concept)
+
+        ent = N(label="concept", props=concept.get_attr_dict())
+        term = N(label="term")
+        ent_trip = T(term, R(Type="represents"), ent)
+
+        if mapping_source:
+            tag_trip = T(
+                concept,
+                R(Type="has_tag"),
+                N(
+                    label="tag",
+                    props={"key": "mapping_source", "value": mapping_source},
+                ),
+            )
+            path = G(ent_trip, tag_trip)
+        else:
+            path = ent_trip
+
+        stmt = Statement(
+            Match(path),
+            Return(f"{term.var}.nanoid"),
+            As("term_nanoids"),
+            use_params=True,
         )
-        return (qry, entity_attr_dict, "term_nano")
+
+        qry = str(stmt)
+        parms = stmt.params
+
+        return (qry, parms, "term_nanoids")
 
     @read_txn_value
-    def get_predicate_nanos(self, concept: Concept):
+    def get_predicate_nanoids(self, concept: Concept, mapping_source: str = ""):
         """Returns list of predicate nanoids with relationship to given concept"""
-        if not concept.nanoid:
-            logging.error("Concept doesn't have a nanoid")
-            raise RuntimeError("arg 'concept' must have nanoid")
-        entity_attr_str = self.get_entity_attrs(concept)
-        entity_attr_dict = self.get_entity_attrs(concept, output_str=False)
-        qry = (
-            f"MATCH (p:predicate)-[r]->(c:concept {entity_attr_str}) "
-            "RETURN p.nanoid AS pred_nano"
+        self.validate_entity_unique(concept)
+
+        ent = N(label="concept", props=concept.get_attr_dict())
+        predicate = N(label="predicate")
+        ent_trip = T(predicate, R0(), ent)
+
+        if mapping_source:
+            tag = N(
+                label="tag",
+                props={"key": "mapping_source", "value": mapping_source},
+            )
+            tag_trip = T(ent, R(Type="has_tag"), tag)
+            path = G(ent_trip, tag_trip)
+        else:
+            path = ent_trip
+
+        stmt = Statement(
+            Match(path),
+            Return(f"{predicate.var}.nanoid"),
+            As("predicate_nanoids"),
+            use_params=True,
         )
-        return (qry, entity_attr_dict, "pred_nano")
+
+        qry = str(stmt)
+        parms = stmt.params
+
+        return (qry, parms, "predicate_nanoids")
 
     @read_txn_value
-    def get_predicate_relationship(self, concept: Concept, predicate: Predicate):
-        """Returns relationship type between given concept and predicate"""
-        if not concept.nanoid or not predicate.nanoid:
-            logging.error("Concept or Predicate don't have a nanoid")
-            raise RuntimeError("args 'concept' and 'predicate' must have nanoid")
-        qry = (
-            "MATCH (p:predicate {nanoid: $pred_nano})-[r]->(c:concept {nanoid: $con_nano}) "
-            "RETURN TYPE(r) as rel_type"
+    def get_relationship_between_entities(self, src_entity: Entity, dst_entity: Entity):
+        """Returns relationship type between given entities with (src)-[:rel_type]->(dst)"""
+        self.validate_entities_unique([src_entity, dst_entity])
+
+        trip = T(
+            N(label=src_entity.get_label(), props=src_entity.get_attr_dict()),
+            R(),
+            N(label=dst_entity.get_label(), props=dst_entity.get_attr_dict()),
         )
-        parms = {"pred_nano": predicate.nanoid, "con_nano": concept.nanoid}
-        return (qry, parms, "rel_type")
 
-    def link_concepts_to_predicate(
+        stmt = Statement(
+            Match(trip),
+            Return(f"TYPE({trip._edge.var})"),
+            As("relationship_type"),
+            use_params=True,
+        )
+
+        qry = str(stmt)
+        parms = stmt.params
+
+        return (qry, parms, "relationship_type")
+
+    def link_concepts_via_predicate(
         self,
-        concept_1: Concept,
-        concept_2: Concept,
-        predicate_handle: str = "exactMatch",
-        _commit=None,
+        subject_concept: Concept,
+        object_concept: Concept,
+        predicate: Predicate,
+        _commit="",
     ) -> None:
         """
         Links two synonymous Concepts via a Predicate
 
         This function takes two synonymous Concepts as objects and links
         them via a Predicate node and has_subject and has_object relationships.
         """
-        if not (concept_1.nanoid and concept_2.nanoid):
-            logging.error("Concepts don't have a nanoid")
-            raise RuntimeError("args 'concept_1' and 'concept_2' must have nanoid")
-        valid_predicate_handles = [
-            "exactMatch",
-            "closeMatch",
-            "broader",
-            "narrower",
-            "related",
-        ]
-        if predicate_handle not in valid_predicate_handles:
-            logging.error(f"Predicate handle: {predicate_handle} not a valid predicate handle")
-            raise RuntimeError(
-                f"'handle' key must be one the following: {valid_predicate_handles}"
-            )
-        # create predicate
-        new_predicate = Predicate(
-            {"handle": predicate_handle, "nanoid": self.make_nano()}
-        )
-        self.create_entity(new_predicate, _commit=_commit)
-        # link concepts to predicate via subject & object relationships
-        self.create_relationship(
-            new_predicate, concept_1, "has_subject", _commit=_commit
-        )
-        self.create_relationship(
-            new_predicate, concept_2, "has_object", _commit=_commit
+        self.validate_entities_unique([subject_concept, object_concept])
+
+        predicate.subject = subject_concept
+        predicate.object = object_concept
+
+        predicate.nanoid = self.get_or_make_entity_nanoid(predicate)
+        self.add_entity_to_mdb(predicate, _commit=_commit)
+
+        self.add_relationship_to_mdb(
+            relationship_type="has_subject",
+            src_entity=predicate,
+            dst_entity=predicate.subject,
+            _commit=_commit,
+        )
+        self.add_relationship_to_mdb(
+            relationship_type="has_object",
+            src_entity=predicate,
+            dst_entity=predicate.object,
+            _commit=_commit,
         )
 
     def merge_two_concepts(
-        self, concept_1: Concept, concept_2: Concept, _commit=None
+        self,
+        concept_1: Concept,
+        concept_2: Concept,
+        mapping_source: str = "",
+        _commit="",
     ) -> None:
         """
         Combine two synonymous Concepts into a single Concept.
 
         This function takes two synonymous Concept as bento-meta objects and
         merges them into a single Concept along with any connected Terms and Predicates.
         """
-        if not (concept_1.nanoid and concept_2.nanoid):
-            logging.error("Concept doesn't have a nanoid")
-            raise RuntimeError("args 'concept_1' and 'concept_2' must have nanoid")
+        self.validate_entities_unique([concept_1, concept_2])
+
         # get list of terms connected to concept 2
-        c2_term_nanos = self.get_term_nanos(concept_2)
-        c2_terms = []
-        for nano in c2_term_nanos:
-            c2_terms.append(Term({"nanoid": nano}))
-        # get list of predicates w/ relationship type connected to concept 2
-        c2_pred_nanos = self.get_predicate_nanos(concept_2)
-        c2_pred_rels = []
-        for nano in c2_pred_nanos:
-            pred = Predicate({"nanoid": nano})
-            rel = self.get_predicate_relationship(concept_2, pred)[0]
-            c2_pred_rels.append([pred, rel])
+        c2_term_nanoids = self.get_term_nanoids(concept_2, mapping_source)
+        c2_terms: List[Term] = []
+        for nanoid in c2_term_nanoids:
+            c2_terms.append(Term({"nanoid": nanoid}))
+
+        # get list of predicates connected to concept 2
+        c2_predicate_nanoids = self.get_predicate_nanoids(concept_2, mapping_source)
+        c2_predicates_with_rel = []
+        for nanoid in c2_predicate_nanoids:
+            predicate = Predicate({"nanoid": nanoid})
+            predicate_rel = self.get_relationship_between_entities(
+                src_entity=predicate, dst_entity=concept_2
+            )[0]
+            c2_predicates_with_rel.append((predicate, predicate_rel))
+
         # delete concept 2
-        self.detach_delete_entity(concept_2)
+        self.remove_entity_from_mdb(concept_2)
+
         # connect terms from deleted (c2) to remaining concept (c1)
         for term in c2_terms:
-            self.create_relationship(term, concept_1, "represents", _commit=_commit)
+            self.add_relationship_to_mdb(
+                relationship_type="represents",
+                src_entity=term,
+                dst_entity=concept_1,
+                _commit=_commit,
+            )
+
         # connect predicates from deleted (c2) to remaining concept (c1)
-        for pred_rel in c2_pred_rels:
-            c2_pred = pred_rel[0]
-            c2_rel = pred_rel[1]
-            self.create_relationship(c2_pred, concept_1, c2_rel, _commit=_commit)
+        for predicate, rel in c2_predicates_with_rel:
+            self.add_relationship_to_mdb(
+                relationship_type=rel,
+                src_entity=predicate,
+                dst_entity=concept_1,
+                _commit=_commit,
+            )
 
-    @read_txn
+    @read_txn_data
     def _get_all_terms(self):
-        """Gets value, origin_name, and nanoid for all terms in database."""
-        qry = (
-            "MATCH (t:term) "
-            "RETURN t.value AS term_val, t.origin_name AS term_origin, t.nanoid as term_nano"
-        )
-        return (qry, {})
-
-    def get_term_synonyms(self, term: Term, threshhold: float = 0.8) -> List[dict]:
-        """Returns list of dicts representing Term nodes synonymous to given Term"""
-        if not (term.origin_name and term.value):
-            logging.error("Term doesn't have origin_name and value")
-            raise RuntimeError("arg 'term' must have both origin_name and value")
-        # load spaCy NER model
-        nlp = spacy.load("en_ner_bionlp13cg_md")
-        # get result with all term values, origin_names, and nanoids in the database
+        """Returns list of all terms in an MDB."""
+        term = N(label="term")
+
+        stmt = Statement(Match(term), Return(term.var))
+
+        qry = str(stmt)
+        parms = {}
+
+        print(qry)
+
+        return (qry, parms)
+
+    def get_potential_term_synonyms(
+        self, term: Term, threshhold: float = 0.8
+    ) -> List[dict]:
+        """
+        Returns list of dicts representing potential Term nodes synonymous to given Term
+        in an MDB
+        """
+        self.validate_entity_unique(term)
+
+        nlp = _get_nlp_model()
+
         all_terms_result = self._get_all_terms()
+        all_terms = [list(item.values())[0] for item in all_terms_result]
+
         # get likely synonyms
         synonyms = []
-        for record in all_terms_result:
+        for term_attr_dict in all_terms:
             # calculate similarity between each Term and input Term
             term_1 = nlp(term.value)
-            term_2 = nlp(str(record["term_val"]))  # type: ignore
+            term_2 = nlp(term_attr_dict["value"])
             similarity_score = term_1.similarity(term_2)
             # if similarity threshold met, add to list of potential synonyms
             if similarity_score >= threshhold:
                 synonym = {
-                    "value": record["term_val"],  # type: ignore
-                    "origin_name": record["term_origin"],  # type: ignore
-                    "nanoid": record["term_nano"],  # type: ignore
+                    "value": term_attr_dict["value"],
+                    "origin_name": term_attr_dict["origin_name"],
+                    "nanoid": term_attr_dict["nanoid"],
                     "similarity": similarity_score,
                     "valid_synonym": 0,  # mark 1 if synonym when uploading later
                 }
                 synonyms.append(synonym)
         synonyms_sorted = sorted(synonyms, key=lambda d: d["similarity"], reverse=True)
         return synonyms_sorted
 
@@ -640,43 +665,245 @@
     ) -> None:
         """Given a list of synonymous Terms as dicts, outputs to CSV file at given output path"""
         with open(output_path, "w", encoding="utf8", newline="") as output_file:
             dict_writer = csv.DictWriter(output_file, fieldnames=input_data[0].keys())
             dict_writer.writeheader()
             dict_writer.writerows(input_data)
 
-    def link_term_synonyms_csv(self, term: Term, csv_path: str, _commit=None) -> None:
+    def link_term_synonyms_csv(
+        self, term: Term, csv_path: str, mapping_source: str, _commit: str = ""
+    ) -> None:
         """Given a CSV of syonymous Terms, links each via a Concept node to given Term"""
         with open(csv_path, encoding="UTF-8") as csvfile:
             synonym_reader = csv.reader(csvfile)
             for line in synonym_reader:
                 if line[3] == "1":
                     synonym = Term()
                     synonym.value = line[0]
                     synonym.origin_name = line[1]
-                    self.link_synonyms(term, synonym, _commit=_commit)
+                    self.link_synonyms(
+                        entity_1=term,
+                        entity_2=synonym,
+                        mapping_source=mapping_source,
+                        _commit=_commit,
+                    )
 
     @read_txn_data
-    def get_property_synonyms(self, prop: Property):
+    def get_property_synonyms_direct(self, entity: Property, mapping_source: str = ""):
         """
         Returns list of properties linked by concept to given property
-        or to synonym of given property
         """
-        if not prop.nanoid:
-            logging.error("Property doesn't have a nanoid")
-            raise RuntimeError("property entity needs a nanoid")
-        p_attrs = self.get_entity_attrs(prop, output_str=False)
-        prop_1 = N(label="property", props=p_attrs)
-        prop_2 = N(label="property")
-        vl_rel = VarLenR(Type="has_concept")
-        trip = NoDirT(prop_1, vl_rel, prop_2)
+        self.validate_entity_unique(entity)
+
+        ent = N(label="property", props=entity.get_attr_dict())
+        prop = N(label="property")
+        concept = N(label="concept")
+        ent_trip_1 = T(ent, R(Type="has_concept"), concept)
+        ent_trip_2 = T(prop, R(Type="has_concept"), concept)
+
+        if mapping_source:
+            tag = N(
+                label="tag",
+                props={"key": "mapping_source", "value": mapping_source},
+            )
+            tag_trip = T(concept, R(Type="has_tag"), tag)
+            path = G(ent_trip_1, ent_trip_2, tag_trip)
+        else:
+            path = G(ent_trip_1, ent_trip_2)
 
         stmt = Statement(
-            Match(trip),
-            Return(f"distinct({prop_2.Return()})"),
-            use_params=True
+            Match(path),
+            With(f"{Collect(_plain_var(prop).pattern())}"),
+            As("synonyms"),
+            Return("synonyms"),
+            use_params=True,
         )
 
         qry = str(stmt)
         parms = stmt.params
 
         return (qry, parms)
+
+    def _get_property_synonyms_direct_as_list(self, entity: Property) -> List[Property]:
+        """
+        converts results of read_txn_data-wrapped function
+        with one item to a simple list of bento_meta.objects.Property entities
+        """
+        data = self.get_property_synonyms_direct(entity)
+        return [Property(s) for s in data[0]["synonyms"]]
+
+    def get_property_synonyms_all(self, entity: Property) -> List[Property]:
+        """
+        Returns list of properties linked by concept to given property
+        or to synonym of given property (and so on)
+        """
+        self.validate_entity_unique(entity)
+        all_synonyms = []
+        queue = [entity]
+        visited = {entity.nanoid}
+
+        while queue:
+            current = queue.pop(0)
+            direct_synonyms = self._get_property_synonyms_direct_as_list(current)
+            for synonym in direct_synonyms:
+                if synonym.nanoid not in visited:
+                    visited.add(synonym.nanoid)
+                    queue.append(synonym)
+                    all_synonyms.append(synonym)
+
+        return all_synonyms
+
+    @read_txn_data
+    def _get_property_parents_data(self, entity: Property):
+        """get list of nodes/edges connected to given property
+        via the "has_property" relationship"""
+        self.validate_entity_unique(entity)
+        p_attrs = entity.get_attr_dict()
+        child_prop = N(label="property", props=p_attrs)
+        parent_node = N(label="node")
+        parent_edge = N(label="relationship")
+        rel = R(Type="has_property", _dir="_left")
+        trip1 = rel.relate(child_prop, N0())
+        trip2 = rel.relate(_plain_var(child_prop), parent_node)
+        trip3 = rel.relate(_plain_var(child_prop), parent_edge)
+
+        stmt = Statement(
+            Match(trip1),
+            OptionalMatch(trip2),
+            OptionalMatch(trip3),
+            With(),
+            Collect(_plain_var(parent_node).pattern()),
+            As("nodes,"),
+            Collect(_plain_var(parent_edge).pattern()),
+            As("edges"),
+            Return("nodes, edges"),
+            use_params=True,
+        )
+
+        qry = str(stmt)
+        parms = stmt.params
+
+        return (qry, parms)
+
+    def get_property_parents(self, entity: Property) -> List[Union[Node, Edge]]:
+        """
+        returns results of _get_property_parents_data as a list of
+        bento_meta Nodes or Edges
+        """
+        self.validate_entity_unique(entity)
+
+        data = self._get_property_parents_data(entity)
+        node_parents = [Node(p) for p in data[0]["nodes"]]
+        edge_parents = [Edge(p) for p in data[0]["edges"]]
+        return node_parents + edge_parents
+
+    def add_tag_to_mdb_entity(self, tag: Tag, entity: Entity) -> None:
+        """Adds a tag to an existing entity in an MDB."""
+        self.validate_entity_unique(entity)
+        self.add_entity_to_mdb(tag)
+        self.add_relationship_to_mdb(
+            relationship_type="has_tag", src_entity=entity, dst_entity=tag
+        )
+
+
+class EntityValidator:
+    """Entity validator that validate entities have all required attributes"""
+
+    required_attrs_by_entity_type: Dict[Type[Entity], List[str]] = {
+        Node: ["handle", "model"],
+        Edge: ["handle", "model", "src", "dst"],
+        Property: ["handle", "model"],
+        Term: ["origin_name", "value"],  # add? "origin_id", "origin_version"
+        Concept: ["nanoid"],
+        Predicate: ["handle", "subject", "object"],
+        Tag: ["key", "value"],
+        ValueSet: ["handle"],
+    }
+
+    valid_attrs: Dict[Tuple[Type[Entity], str], Set[str]] = {
+        (Predicate, "handle"): {
+            "exactMatch",
+            "closeMatch",
+            "broader",
+            "narrower",
+            "related",
+        }
+    }
+
+    class MissingAttributeError(Exception):
+        """Raised when an entity doesn't have the attributes required for unique identification"""
+
+    class InvalidAttributeError(Exception):
+        """Raised when an entity attribute is invalid"""
+
+    @staticmethod
+    def validate_entity_has_attribute(entity: Entity, attr_name: str) -> None:
+        """Validates the presence of an entity's attribute"""
+        if not getattr(entity, attr_name):
+            raise EntityValidator.MissingAttributeError(
+                f"{entity.__class__.__name__} needs a {attr_name} attribute"
+            )
+
+    @staticmethod
+    def _validate_entity_attribute(entity_type: Type[Entity], attr_name: str) -> None:
+        """Checks that an entity attribute is in a set of valid attributes"""
+        valid_attrs = EntityValidator.valid_attrs.get((entity_type, attr_name))
+
+        if valid_attrs and getattr(entity_type, attr_name) not in valid_attrs:
+            raise EntityValidator.InvalidAttributeError(
+                f"{entity_type.__name__} {attr_name} must be one of: "
+                f"{', '.join(list(valid_attrs))}"
+            )
+
+    @staticmethod
+    def validate_entity(entity: Entity) -> None:
+        """
+        Checks if entity has all attributes required by MDB for its type, and
+        that all of those attributes are valid themselves if they are entities or
+        if they have a fixed set of possible values.
+
+        Verifies that bento-meta entity has all necesssary attributes before
+        it is added to an MDB instance.
+
+        If looking for a unique identifier for the entity (i.e. nanoid), ensures
+        entity has all the required attributes for unique identification.
+        """
+        entity_type = type(entity)
+        required_attrs = EntityValidator.required_attrs_by_entity_type.get(entity_type)
+
+        if not required_attrs:
+            raise ValueError(f"Entity type {entity_type.__name__} not supported")
+
+        for attr_name in required_attrs:
+            try:
+                # validate attr that is an entity (e.g. Edge.src)
+                if isinstance(getattr(entity, attr_name), Entity):
+                    EntityValidator.validate_entity(getattr(entity, attr_name))
+                # check entity has attr if required
+                EntityValidator.validate_entity_has_attribute(entity, attr_name)
+                # check attr with fixed set of possible values is valid
+                EntityValidator._validate_entity_attribute(entity_type, attr_name)
+            except (
+                EntityValidator.MissingAttributeError,
+                EntityValidator.InvalidAttributeError,
+            ) as error:
+                logger.error(str(error))
+                raise
+
+
+def _get_nlp_model():
+    """Installs and imports spacy & scispacy nlp model if any not already installed"""
+    model_name = "en_ner_bionlp13cg_md"
+    model_url = "https://s3-us-west-2.amazonaws.com/ai2-s2-scispacy/releases/v0.5.1/en_ner_bionlp13cg_md-0.5.1.tar.gz"
+
+    try:
+        if not find_spec("spacy"):  # ensure spacy is installed
+            check_call([executable, "-m", "pip", "install", "spacy"])
+        import spacy
+
+        if not find_spec(model_name):  # ensure model is installed
+            check_call([executable, "-m", "pip", "install", model_url])
+        nlp = spacy.load(model_url)
+        return nlp
+    except Exception as error:
+        logger.error(str(error))
+        raise
```

### Comparing `bento_meta-0.1.3/src/bento_meta/mdb/searchable.py` & `bento_meta-0.2.2/src/bento_meta/mdb/searchable.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         if limit:
             parms['limit'] = limit
         return (qry, parms)
 
     def search_entity_handles(self, qstring):
         """Fulltext search of qstring over node, relationship, and property handles.
         Returns { node:[ {ent:<entity dict>,score:<lucene score>},... ],
-                  relationship:[ <...> ], property:[ <...> ] }"""
+        relationship:[ <...> ], property:[ <...> ] }"""
 
         result = self.query_index('entityHandle', qstring)
         if not result:
             return None
         plural = {"node":"nodes", "relationship":"relationships",
                   "property":"properties"}
         ret = {"nodes": [], "relationships": [], "properties": []}
```

### Comparing `bento_meta-0.1.3/src/bento_meta/mdb/writeable.py` & `bento_meta-0.2.2/src/bento_meta/mdb/writeable.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.1.3/src/bento_meta/model.py` & `bento_meta-0.2.2/src/bento_meta/model.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.1.3/src/bento_meta/object_map.py` & `bento_meta-0.2.2/src/bento_meta/object_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 from neo4j import BoltDriver, Neo4jDriver
 from bento_meta.entity import *
 from bento_meta.objects import *
 # from pdb import set_trace
 
 
 class ObjectMap(object):
+    """This module contains :class:`ObjectMap`, a class which provides the 
+    machinery for mapping bento_meta objects to a Bento Metamodel Database
+    in Neo4j. Mostly not for human consumption."""
     cache = {}
 
     def __init__(self, *, cls=None, drv=None):
         if not cls:
             raise ArgError("arg cls= is required")
         self.cls = cls
         if drv:
```

### Comparing `bento_meta-0.1.3/src/bento_meta/objects.py` & `bento_meta-0.2.2/src/bento_meta/objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 ==================
 
 This module contains the subclasses of :class:`Entity` which are used 
 in representing the models contained in the `MDB <https://github.com/CBIIT/bento-mdf>`_.
 
 """
 import sys
+
 sys.path.append("..")
 from copy import deepcopy
+
 from bento_meta.entity import Entity
+
 # from pdb import set_trace
 
 
 def mergespec(clsname, attspec, mapspec):
     """Merge subclass attribute and mapping specification dicts with the
     base class's. Not for human consumption.
     """
@@ -46,25 +49,26 @@
     mapspec_ = {
         "label": "node",
         "key": "handle",
         "property": {"handle": "handle", "model": "model", "nanoid": "nanoid"},
         "relationship": {
             "concept": {"rel": ":has_concept>", "end_cls": "Concept"},
             "props": {"rel": ":has_property>", "end_cls": "Property"},
-            "tags": {"rel": ":has_tag>", "end_cls":"Tag"}
+            "tags": {"rel": ":has_tag>", "end_cls": "Tag"},
         },
     }
     (attspec, _mapspec) = mergespec("Node", attspec_, mapspec_)
 
     def __init__(self, init=None):
         super().__init__(init=init)
 
 
 class Property(Entity):
     """Subclass that models a property of a node or relationship (edge)."""
+
     pvt_attr = Entity.pvt_attr + ["value_types"]
     attspec_ = {
         "handle": "simple",
         "model": "simple",
         "nanoid": "simple",
         "value_domain": "simple",
         "units": "simple",
@@ -86,20 +90,20 @@
             "units": "units",
             "item_domain": "item_domain",
             "is_required": "is_required",
         },
         "relationship": {
             "concept": {"rel": ":has_concept>", "end_cls": "Concept"},
             "value_set": {"rel": ":has_value_set>", "end_cls": "ValueSet"},
-            "tags": {"rel": ":has_tag>", "end_cls":"Tag"}
+            "tags": {"rel": ":has_tag>", "end_cls": "Tag"},
         },
     }
     (attspec, _mapspec) = mergespec("Property", attspec_, mapspec_)
-    defaults = { "value_domain":"TBD" }
-    
+    defaults = {"value_domain": "TBD"}
+
     def __init__(self, init=None):
         super().__init__(init=init)
         self.value_types = []
 
     @property
     def terms(self):
         """If the `Property` has a ``value_set`` domain, return the `Term` objects
@@ -117,14 +121,15 @@
         """
         if self.value_set:
             return [self.terms[x].value for x in self.terms]
 
 
 class Edge(Entity):
     """Subclass that models a relationship between model nodes."""
+
     defaults = {
         "multiplicity": "many_to_many",
     }
     attspec_ = {
         "handle": "simple",
         "model": "simple",
         "nanoid": "simple",
@@ -146,19 +151,19 @@
             "is_required": "is_required",
         },
         "relationship": {
             "src": {"rel": ":has_src>", "end_cls": "Node"},
             "dst": {"rel": ":has_dst>", "end_cls": "Node"},
             "concept": {"rel": ":has_concept>", "end_cls": "Concept"},
             "props": {"rel": ":has_property>", "end_cls": "Property"},
-            "tags": {"rel": ":has_tag>", "end_cls":"Tag"}
+            "tags": {"rel": ":has_tag>", "end_cls": "Tag"},
         },
     }
     (attspec, _mapspec) = mergespec("Edge", attspec_, mapspec_)
-     
+
     def __init__(self, init=None):
         super().__init__(init=init)
 
     @property
     def triplet(self):
         """A 3-tuple that fully qualifies the edge: ``(edge.handle, src.handle, dst.handle)``
         ``src`` and ``dst`` attributes must be set.
@@ -196,15 +201,15 @@
             "origin_version": "origin_version",
             "origin_definition": "origin_definition",
             "origin_name": "origin_name",
         },
         "relationship": {
             "concept": {"rel": ":represents>", "end_cls": "Concept"},
             "origin": {"rel": ":has_origin>", "end_cls": "Origin"},
-            "tags": {"rel": ":has_tag>", "end_cls":"Tag"}
+            "tags": {"rel": ":has_tag>", "end_cls": "Tag"},
         },
     }
     (attspec, _mapspec) = mergespec("Term", attspec_, mapspec_)
 
     def __init__(self, init=None):
         super().__init__(init=init)
 
@@ -212,30 +217,35 @@
 # for ValueSet - updating terms prop should dirty the connected Property
 # (from Bento::Meta), signal need to refresh. Engineer so this happens
 # here (__setattr__ override), not in Entity
 class ValueSet(Entity):
     """Subclass that models an enumerated set of :class:`Property` values.
     Essentially a container for :class:`Term` instances.
     """
+
     attspec_ = {
         "handle": "simple",
         "nanoid": "simple",
         "url": "simple",
         "prop": "object",
         "origin": "object",
         "terms": "collection",
     }
     mapspec_ = {
         "label": "value_set",
-        "property": {"handle": "handle", "url": "url", "nanoid": "nanoid",},
+        "property": {
+            "handle": "handle",
+            "url": "url",
+            "nanoid": "nanoid",
+        },
         "relationship": {
             "prop": {"rel": "<:has_value_set", "end_cls": "Property"},
             "terms": {"rel": ":has_term>", "end_cls": "Term"},
             "origin": {"rel": ":has_origin>", "end_cls": "Origin"},
-            "tags": {"rel": ":has_tag>", "end_cls":"Tag"}
+            "tags": {"rel": ":has_tag>", "end_cls": "Tag"},
         },
     }
     (attspec, _mapspec) = mergespec("ValueSet", attspec_, mapspec_)
 
     def __init__(self, init=None):
         super().__init__(init=init)
 
@@ -259,75 +269,101 @@
     """Subclass that models a semantic concept."""
 
     attspec_ = {"terms": "collection"}
     mapspec_ = {
         "label": "concept",
         "relationship": {
             "terms": {"rel": "<:represents", "end_cls": "Term"},
-            "tags": {"rel": ":has_tag>", "end_cls":"Tag"}            
+            "tags": {"rel": ":has_tag>", "end_cls": "Tag"},
         },
     }
     (attspec, _mapspec) = mergespec("Concept", attspec_, mapspec_)
 
     def __init__(self, init=None):
         super().__init__(init=init)
 
+
 class Predicate(Entity):
     """Subclass that models a semantic link between concepts."""
-    attspec_ = {
-        "handle": "simple",
-        "subject": "object",
-        "object": "object"}
+
+    attspec_ = {"handle": "simple", "subject": "object", "object": "object"}
     mapspec_ = {
         "label": "predicate",
         "key": "handle",
         "property": {
             "handle": "handle",
         },
         "relationship": {
             "subject": {"rel": ":has_subject>", "end_cls": "Concept"},
             "object": {"rel": ":has_object>", "end_cls": "Concept"},
-            "tags": {"rel": ":has_tag>", "end_cls":"Tag"}            
+            "tags": {"rel": ":has_tag>", "end_cls": "Tag"},
         },
     }
     (attspec, _mapspec) = mergespec("Predicate", attspec_, mapspec_)
 
     def __init__(self, init=None):
         super().__init__(init=init)
-        
+
 
 class Origin(Entity):
     """Subclass that models a :class:`Term` 's authoritative source."""
 
-    attspec_ = {"url": "simple", "is_external": "simple", "name": "simple", "nanoid": "simple",}
+    attspec_ = {
+        "url": "simple",
+        "is_external": "simple",
+        "name": "simple",
+        "nanoid": "simple",
+    }
     mapspec_ = {
         "label": "origin",
         "key": "name",
         "property": {
             "name": "name",
             "url": "url",
             "is_external": "is_external",
             "nanoid": "nanoid",
         },
-        "relationship": {
-            "tags": {"rel": ":has_tag>", "end_cls":"Tag"}
-        }
+        "relationship": {"tags": {"rel": ":has_tag>", "end_cls": "Tag"}},
     }
     (attspec, _mapspec) = mergespec("Origin", attspec_, mapspec_)
 
     def __init__(self, init=None):
         super().__init__(init=init)
 
 
 class Tag(Entity):
     """Subclass that allows simple key-value tagging of a model at arbitrary points."""
 
-    attspec_ = {"key":"simple", "value": "simple"}
+    attspec_ = {"key": "simple", "value": "simple"}
     mapspec_ = {
         "label": "tag",
         "key": "key",
         "property": {"key": "key", "value": "value"},
     }
     (attspec, _mapspec) = mergespec("Tag", attspec_, mapspec_)
 
     def __init__(self, init=None):
         super().__init__(init=init)
+
+
+class Model(Entity):
+    """Subclass with information regarding data model."""
+
+    attspec_ = {
+        "handle": "simple",
+        "name": "simple",
+        "repository": "simple",
+        "nanoid": "simple",
+    }
+    mapspec_ = {
+        "label": "model",
+        "key": "handle",
+        "property": {
+            "handle": "handle",
+            "name": "name",
+            "repository": "repository",
+        },
+    }
+    (attspec, _mapspec) = mergespec("Model", attspec_, mapspec_)
+
+    def __init__(self, init=None):
+        super().__init__(init=init)
```

### Comparing `bento_meta-0.1.3/src/bento_meta/util/_engine.py` & `bento_meta-0.2.2/src/bento_meta/util/_engine.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.1.3/src/bento_meta/util/cypher/clauses.py` & `bento_meta-0.2.2/src/bento_meta/util/cypher/clauses.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 bento_meta.util.cypher.clauses
 
 Representations of Cypher statement clauses, statements,
 and statement parameters.
 """
+from pdb import set_trace
 from string import Template
-from bento_meta.util.cypher.entities import (
-    N, R, P, _return, _condition, _pattern
-    )
+
+from bento_meta.util.cypher.entities import N, P, R, _condition, _pattern, _return
 from bento_meta.util.cypher.functions import Func
-from pdb import set_trace
+
 
 class Clause(object):
     """Represents a generic Cypher clause."""
+
     template = Template("$slot1")
     joiner = ", "
 
     @staticmethod
     def context(arg):
         return _return(arg)
 
@@ -31,92 +32,97 @@
                 values.append(c)
             elif isinstance(c, Func):
                 values.append(str(c))
             elif isinstance(c, list):
                 values.extend([str(x) for x in c])
             else:
                 values.append(str(c))
-        return self.template.substitute(
-            slot1=self.joiner.join(values)
-            )
+        return self.template.substitute(slot1=self.joiner.join(values))
 
 
 class Match(Clause):
     """Create a MATCH clause with the arguments."""
+
     template = Template("MATCH $slot1")
 
     @staticmethod
     def context(arg):
         return _pattern(arg)
 
     def __init__(self, *args):
         super().__init__(*args)
 
 
 class Where(Clause):
     """Create a WHERE clause with the arguments
     (joining conditions with 'op')."""
+
     template = Template("WHERE $slot1")
     joiner = " {} "
 
     @staticmethod
     def context(arg):
         return _condition(arg)
 
-    def __init__(self, *args, op='AND'):
+    def __init__(self, *args, op="AND"):
         super().__init__(*args, op=op)
         self.op = op
 
     def __str__(self):
         values = []
         for c in [self.context(x) for x in self.args]:
             if isinstance(c, str):
                 values.append(c)
             elif isinstance(c, Func):
                 values.append(str(c))
             elif isinstance(c, list):
                 values.extend([str(x) for x in c])
             else:
                 values.append(str(c))
-        return self.template.substitute(
-            slot1=self.joiner.format(self.op).join(values)
-            )
+        return self.template.substitute(slot1=self.joiner.format(self.op).join(values))
 
 
 class With(Clause):
     """Create a WITH clause with the arguments."""
+
     template = Template("WITH $slot1")
 
     def __init__(self, *args):
         super().__init__(*args)
 
 
 class Create(Clause):
     """Create a CREATE clause with the arguments."""
+
     template = Template("CREATE $slot1")
+
     @staticmethod
     def context(arg):
         return _pattern(arg)
 
     def __init__(self, *args):
         super().__init__(*args)
 
 
 class Merge(Clause):
     """Create a MERGE clause with the arguments."""
+
     template = Template("MERGE $slot1")
+
     @staticmethod
     def context(arg):
         return _pattern(arg)
 
     def __init__(self, *args):
         super().__init__(*args)
 
+
 class Remove(Clause):
     """Create a REMOVE clause with the arguments."""
+
     template = Template("REMOVE $slot1")
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def __str__(self):
         ent = self.args[0]
@@ -125,22 +131,23 @@
         if "prop" in self.kwargs:
             item = self.kwargs["prop"]
             sep = "."
         elif "label" in self.kwargs:
             item = self.kwargs["label"]
             sep = ":"
         return self.template.substitute(
-            slot1="{}{}{}".format(self.context(ent),sep,item)
-            )
-        
+            slot1="{}{}{}".format(self.context(ent), sep, item)
+        )
+
 
 class Set(Clause):
     """
     Create a SET clause with the arguments. (Only property arguments matter.)
     """
+
     template = Template("SET $slot1")
 
     @staticmethod
     def context(arg):
         return _condition(arg)
 
     def __init__(self, *args, **kwargs):
@@ -153,98 +160,195 @@
                 values.append(c)
             elif isinstance(c, Func):
                 values.append(str(c))
             elif isinstance(c, list):
                 values.extend([str(x) for x in c])
             else:
                 values.append(str(c))
-        if 'update' in self.kwargs:
-            values = [x.replace("=","+=") for x in values]
-        return self.template.substitute(
-            slot1=self.joiner.join(values)
-            )
+        if "update" in self.kwargs:
+            values = [x.replace("=", "+=") for x in values]
+        return self.template.substitute(slot1=self.joiner.join(values))
 
 
 class OnCreateSet(Set):
     """Create an ON CREATE SET clause for a MERGE with the arguments."""
+
     template = Template("ON CREATE SET $slot1")
 
     def __init__(self, *args):
         super().__init__(*args)
 
 
 class OnMatchSet(Set):
     """Create an ON CREATE SET clause for a MERGE with the arguments."""
+
     template = Template("ON MATCH SET $slot1")
 
     def __init__(self, *args):
         super().__init__(*args)
 
 
 class Return(Clause):
     """Create a RETURN clause with the arguments."""
+
     template = Template("RETURN $slot1")
 
     def __init__(self, *args):
         super().__init__(*args)
 
 
 class OptionalMatch(Clause):
     """Create an OPTIONAL MATCH clause with the arguments."""
+
     template = Template("OPTIONAL MATCH $slot1")
 
     @staticmethod
     def context(arg):
         return _pattern(arg)
 
     def __init__(self, *args):
         super().__init__(*args)
 
 
 class Collect(Clause):
     """Create a COLLECT clause with the arguments."""
+
     template = Template("COLLECT $slot1")
 
     def __init__(self, *args):
         super().__init__(*args)
 
 
 class Unwind(Clause):
     """Create an UNWIND clause with the arguments."""
+
     template = Template("UNWIND $slot1")
 
     def __init__(self, *args):
         super().__init__(*args)
 
 
 class As(Clause):
     """Create an AS clause with the arguments."""
+
     template = Template("AS $slot1")
 
     def __init__(self, *args):
         super().__init__(*args)
 
 
+class Delete(Clause):
+    """Create a DELETE clause with the arguments."""
+
+    template = Template("DELETE $slot1")
+
+    def __init__(self, *args):
+        super().__init__(*args)
+
+
+class DetachDelete(Clause):
+    """Create a DETACH DELETE clause with the arguments."""
+
+    template = Template("DETACH DELETE $slot1")
+
+    def __init__(self, *args):
+        super().__init__(*args)
+
+
+class Case(Clause):
+    """Create a CASE clause with the arguments."""
+
+    template = Template("CASE $slot1")
+
+    def __init__(self, *args):
+        super().__init__(*args)
+
+
+class When(Clause):
+    """Create a WHEN clause with the arguments."""
+
+    template = Template("WHEN $slot1")
+    joiner = " {} "
+
+    @staticmethod
+    def context(arg):
+        return _condition(arg)
+
+    def __init__(self, *args, op="AND"):
+        super().__init__(*args, op=op)
+        self.op = op
+
+    def __str__(self):
+        values = []
+        for c in [self.context(x) for x in self.args]:
+            if isinstance(c, str):
+                values.append(c)
+            elif isinstance(c, Func):
+                values.append(str(c))
+            elif isinstance(c, list):
+                values.extend([str(x) for x in c])
+            else:
+                values.append(str(c))
+        return self.template.substitute(slot1=self.joiner.format(self.op).join(values))
+
+
+class Then(Clause):
+    """Create a THEN clause with the arguments."""
+
+    template = Template("THEN $slot1")
+
+    def __init__(self, *args):
+        super().__init__(*args)
+
+
+class Else(Clause):
+    """Create an ELSE clause with the arguments."""
+
+    template = Template("ELSE $slot1")
+
+    def __init__(self, *args):
+        super().__init__(*args)
+
+
+class End(Clause):
+    """Create an END clause with the arguments."""
+
+    template = Template("END $slot1")
+
+    def __init__(self, *args):
+        super().__init__(*args)
+
+
+class ForEach(Clause):
+    """Create an FOREACH clause with the arguments."""
+
+    template = Template("FOREACH $slot1")
+
+    def __init__(self, *args):
+        super().__init__(*args)
+
+
 class Statement(object):
     """Create a Neo4j statement comprised of clauses (and strings) in order."""
+
     def __init__(self, *args, terminate=False, use_params=False):
         self.clauses = args
         self.terminate = terminate
         self.use_params = use_params
         self._params = None
 
     def __str__(self):
         stash = P.parameterize
         if self.use_params:
             P.parameterize = True
         else:
             P.parameterize = False
         ret = " ".join([str(x) for x in self.clauses])
         if self.terminate:
-            ret = ret+";"
+            ret = ret + ";"
         P.parameterize = stash
         return ret
 
     # def params(self):
     #     if not self._params:
     #         self._params = re.findall("\\$[a-zA-A0-9_]+", str(self))
     #     return self._params
@@ -254,16 +358,16 @@
             self._params = {}
             for c in self.clauses:
                 for ent in c.args:
                     if isinstance(ent, (N, R)):
                         for p in ent.props.values():
                             self._params[p.var] = p.value
                     else:
-                        if 'nodes' in vars(type(ent)):
+                        if "nodes" in vars(type(ent)):
                             for n in ent.nodes():
                                 for p in n.props.values():
                                     self._params[p.var] = p.value
-                        if 'edges' in vars(type(ent)):
+                        if "edges" in vars(type(ent)):
                             for e in ent.edges():
                                 for p in e.props.values():
                                     self._params[p.var] = p.value
         return self._params
```

### Comparing `bento_meta-0.1.3/src/bento_meta/util/cypher/entities.py` & `bento_meta-0.2.2/src/bento_meta/util/cypher/entities.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.1.3/src/bento_meta/util/cypher/functions.py` & `bento_meta-0.2.2/src/bento_meta/util/cypher/functions.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.1.3/src/bento_meta/util/makeq.py` & `bento_meta-0.2.2/src/bento_meta/util/makeq.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.1.3/PKG-INFO` & `bento_meta-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: bento-meta
-Version: 0.1.3
+Version: 0.2.2
 Summary: Python drivers for Bento Metamodel Database
 License: Apache 2.0
 Author: Mark A. Jensen
 Author-email: mark.jensen@nih.gov
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: tools
-Requires-Dist: PyYAML (>=6)
+Requires-Dist: PyYAML (>=6.0.1)
+Requires-Dist: bento-mdf (>=0.9.1,<0.10.0)
 Requires-Dist: click (>=8.1.3,<9.0.0) ; extra == "tools"
 Requires-Dist: delfick-project (>=0.7.9,<0.8.0)
+Requires-Dist: liquichange (>=0.2.1,<0.3.0) ; extra == "tools"
 Requires-Dist: nanoid (>=2.0.0,<3.0.0)
 Requires-Dist: neo4j (>=4.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0) ; extra == "tools"
 Requires-Dist: pandas (>=1.5.2,<2.0.0) ; extra == "tools"
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: setuptools (>=65.4.1,<66.0.0)
 Requires-Dist: spacy (>=3.4.3,<4.0.0) ; extra == "tools"
```

