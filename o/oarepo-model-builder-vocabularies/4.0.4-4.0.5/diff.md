# Comparing `tmp/oarepo-model-builder-vocabularies-4.0.4.tar.gz` & `tmp/oarepo-model-builder-vocabularies-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-vocabularies-4.0.4.tar", last modified: Fri Jul 14 10:29:54 2023, max compression
+gzip compressed data, was "oarepo-model-builder-vocabularies-4.0.5.tar", last modified: Sat Jul 22 20:49:57 2023, max compression
```

## Comparing `oarepo-model-builder-vocabularies-4.0.4.tar` & `oarepo-model-builder-vocabularies-4.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:54.901685 oarepo-model-builder-vocabularies-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-14 10:29:54.901685 oarepo-model-builder-vocabularies-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:54.901685 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:54.901685 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/builders/setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:54.901685 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/models/vocabulary.json
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/models/vocabulary.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:54.901685 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-14 10:29:54.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-14 10:29:54.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:29:54.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-14 10:29:54.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:26:58.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-14 10:29:54.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 10:29:54.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-14 10:29:54.905685 oarepo-model-builder-vocabularies-4.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:49:57.115395 oarepo-model-builder-vocabularies-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-22 20:46:41.000000 oarepo-model-builder-vocabularies-4.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-22 20:49:57.115395 oarepo-model-builder-vocabularies-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-22 20:46:41.000000 oarepo-model-builder-vocabularies-4.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:49:57.115395 oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 20:46:41.000000 oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:49:57.115395 oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 20:46:41.000000 oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-22 20:46:41.000000 oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies/builders/setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-22 20:46:41.000000 oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-22 20:46:41.000000 oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:49:57.115395 oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 20:46:41.000000 oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-22 20:46:41.000000 oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies/models/vocabulary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-22 20:46:41.000000 oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies/models/vocabulary.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:49:57.115395 oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-22 20:49:57.000000 oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-22 20:49:57.000000 oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 20:49:57.000000 oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-22 20:49:57.000000 oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 20:47:40.000000 oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-22 20:49:57.000000 oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-22 20:49:57.000000 oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-22 20:46:41.000000 oarepo-model-builder-vocabularies-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-22 20:49:57.119395 oarepo-model-builder-vocabularies-4.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-22 20:46:41.000000 oarepo-model-builder-vocabularies-4.0.5/setup.py
```

### Comparing `oarepo-model-builder-vocabularies-4.0.4/PKG-INFO` & `oarepo-model-builder-vocabularies-4.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-vocabularies
-Version: 4.0.4
+Version: 4.0.5
 Summary: "A model builder plugin to reference vocabularies"
 Home-page: https://github.com/oarepo/oarepo-model-builder-vocabularies
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio vocabulary model builder
 Platform: any
```

### Comparing `oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/components.py` & `oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,9 @@
         self,
         datatype,
         facet_definition: FacetDefinition,
     ):
         # do not build facet definition for children of this component
         return []
 
-COMPONENTS = [VocabularyDataTypeComponent]
+
+COMPONENTS = [VocabularyDataTypeComponent]
```

### Comparing `oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/datatypes.py` & `oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies/datatypes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import marshmallow as ma
 from marshmallow import fields
+from oarepo_model_builder.datatypes.components.model.utils import array_contains_value
 from oarepo_model_builder.datatypes.datatypes import DataType
 from oarepo_model_builder.validation import InvalidModelException
 from oarepo_model_builder_relations.datatypes import RelationDataType
-from oarepo_model_builder.datatypes.components.model.utils import array_contains_value
 
 
 class VocabularyDataType(RelationDataType):
     model_type = "vocabulary"
     facets = {
-        'facet-class': "VocabularyFacet",
-        'imports': [
-            {"import": "oarepo_vocabularies.services.facets.VocabularyFacet"}
-        ],
+        "facet-class": "VocabularyFacet",
+        "imports": [{"import": "oarepo_vocabularies.services.facets.VocabularyFacet"}],
     }
 
     class ModelSchema(RelationDataType.ModelSchema):
         vocabulary_type = ma.fields.String(
             attribute="vocabulary-type", data_key="vocabulary-type"
         )
 
     def prepare(self, context):
         vocabulary_type = self.definition.get("vocabulary-type", None)
         vocabulary_class = self.definition.pop("class", None)
 
         vocabulary_imports = self.definition.setdefault("imports", [])
         self.definition.setdefault("model", "vocabularies")
-        self.definition.setdefault("keys", ["id", "title"])
+        keys = list(self.definition.setdefault("keys", ["id", "title"]))
         self.definition.setdefault("marshmallow", {})
         self.definition.setdefault("ui", {}).setdefault("marshmallow", {})
         self.definition["ui"].setdefault("detail", "vocabulary_item")
         self.definition["ui"].setdefault("edit", "vocabulary_item")
         pid_field = self.definition.get("pid-field", None)
 
         if not pid_field:
@@ -50,20 +48,29 @@
                     )
                 pid_field = f"{vocabulary_class}.pid"
 
         # self.definition["type"] = "relation"
         self.definition["pid-field"] = pid_field
 
         # set up vocabulary argument to facets
-        facets = self.definition.setdefault('facets', {})
-        facets_args = facets.setdefault('args', [])
-        vocabulary_attr = f'vocabulary={repr(vocabulary_type)}'
+        facets = self.definition.setdefault("facets", {})
+        facets_args = facets.setdefault("args", [])
+        vocabulary_attr = f"vocabulary={repr(vocabulary_type)}"
         if not array_contains_value(facets_args, vocabulary_attr):
             facets_args.append(vocabulary_attr)
 
+        transformed_keys = []
+        for key in keys:
+            if isinstance(key, str) and key.startswith("props."):
+                transformed_keys.append(
+                    {"key": key, "model": {"type": "keyword"}, "target": key[6:]}
+                )
+            else:
+                transformed_keys.append(key)
+        self.definition["keys"] = transformed_keys
         super().prepare(context)
 
     def get_facet(self, stack, parent_path):
         if not stack:
             # we are the facet, unlike normal container, for which a facet is not generated,
             # we need to generate it -> calling direct data type
             return DataType.get_facet(self, stack, parent_path)
@@ -97,16 +104,16 @@
         )
         model = fields.String(required=False)
 
 
 class TaxonomyDataType(VocabularyDataType):
     model_type = "taxonomy"
     facets = {
-        'facet-class': "HierarchyVocabularyFacet",
-        'imports': [
+        "facet-class": "HierarchyVocabularyFacet",
+        "imports": [
             {"import": "oarepo_vocabularies.services.facets.HierarchyVocabularyFacet"}
         ],
     }
 
     def prepare(self, context):
         keys = list(self.definition.get("keys", []))
         self.definition.setdefault("ui", {}).setdefault("detail", "taxonomy_item")
```

### Comparing `oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/models/vocabulary.json` & `oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies/models/vocabulary.json`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/models/vocabulary.yaml` & `oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies/models/vocabulary.yaml`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/PKG-INFO` & `oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-vocabularies
-Version: 4.0.4
+Version: 4.0.5
 Summary: "A model builder plugin to reference vocabularies"
 Home-page: https://github.com/oarepo/oarepo-model-builder-vocabularies
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio vocabulary model builder
 Platform: any
```

### Comparing `oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt` & `oarepo-model-builder-vocabularies-4.0.5/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-vocabularies-4.0.4/setup.cfg` & `oarepo-model-builder-vocabularies-4.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-vocabularies
-version = 4.0.4
+version = 4.0.5
 description = "A model builder plugin to reference vocabularies"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = invenio vocabulary model builder
 license = MIT
 author = Miroslav Simek
 author_email = simek.miroslav@techlib.cz
```

