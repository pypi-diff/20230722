# Comparing `tmp/dsversioner-0.9.4.tar.gz` & `tmp/dsversioner-0.9.5.tar.gz`

## Comparing `dsversioner-0.9.4.tar` & `dsversioner-0.9.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dsversioner-0.9.4/CONTRIBUTING.md
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 dsversioner-0.9.4/SECURITY.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 dsversioner-0.9.4/docs/developer.md
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dsversioner-0.9.4/docs/index.md
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 dsversioner-0.9.4/dsversioner/Dataset.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 dsversioner-0.9.4/dsversioner/DatasetMetadata.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 dsversioner-0.9.4/dsversioner/DatasetRecordData.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 dsversioner-0.9.4/dsversioner/DatasetVersion.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 dsversioner-0.9.4/dsversioner/Exceptions.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dsversioner-0.9.4/dsversioner/FileSystemStorage.py
--rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 dsversioner-0.9.4/dsversioner/ObjectDataset.py
--rw-r--r--   0        0        0    20123 2020-02-02 00:00:00.000000 dsversioner-0.9.4/dsversioner/ObjectDatasetFileSystemStorage.py
--rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 dsversioner-0.9.4/dsversioner/ObjectDatasetMetadata.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 dsversioner-0.9.4/dsversioner/ObjectDatasetRecordData.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 dsversioner-0.9.4/dsversioner/ObjectDatasetStorage.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 dsversioner-0.9.4/dsversioner/ObjectDatasetVersion.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 dsversioner-0.9.4/dsversioner/Serializable.py
--rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 dsversioner-0.9.4/dsversioner/Storage.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 dsversioner-0.9.4/dsversioner/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 dsversioner-0.9.4/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dsversioner-0.9.4/LICENSE
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 dsversioner-0.9.4/README.md
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 dsversioner-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 dsversioner-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dsversioner-0.9.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 dsversioner-0.9.5/SECURITY.md
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 dsversioner-0.9.5/docs/developer.md
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dsversioner-0.9.5/docs/index.md
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 dsversioner-0.9.5/dsversioner/Dataset.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 dsversioner-0.9.5/dsversioner/DatasetMetadata.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 dsversioner-0.9.5/dsversioner/DatasetRecordData.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 dsversioner-0.9.5/dsversioner/DatasetVersion.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 dsversioner-0.9.5/dsversioner/Exceptions.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dsversioner-0.9.5/dsversioner/FileSystemStorage.py
+-rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 dsversioner-0.9.5/dsversioner/ObjectDataset.py
+-rw-r--r--   0        0        0    20213 2020-02-02 00:00:00.000000 dsversioner-0.9.5/dsversioner/ObjectDatasetFileSystemStorage.py
+-rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 dsversioner-0.9.5/dsversioner/ObjectDatasetMetadata.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 dsversioner-0.9.5/dsversioner/ObjectDatasetRecordData.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 dsversioner-0.9.5/dsversioner/ObjectDatasetStorage.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 dsversioner-0.9.5/dsversioner/ObjectDatasetVersion.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 dsversioner-0.9.5/dsversioner/Serializable.py
+-rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 dsversioner-0.9.5/dsversioner/Storage.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 dsversioner-0.9.5/dsversioner/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 dsversioner-0.9.5/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dsversioner-0.9.5/LICENSE
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 dsversioner-0.9.5/README.md
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 dsversioner-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 dsversioner-0.9.5/PKG-INFO
```

### Comparing `dsversioner-0.9.4/SECURITY.md` & `dsversioner-0.9.5/SECURITY.md`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.4/docs/developer.md` & `dsversioner-0.9.5/docs/developer.md`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.4/dsversioner/Dataset.py` & `dsversioner-0.9.5/dsversioner/Dataset.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.4/dsversioner/DatasetMetadata.py` & `dsversioner-0.9.5/dsversioner/DatasetMetadata.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.4/dsversioner/DatasetVersion.py` & `dsversioner-0.9.5/dsversioner/DatasetVersion.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.4/dsversioner/Exceptions.py` & `dsversioner-0.9.5/dsversioner/Exceptions.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.4/dsversioner/ObjectDataset.py` & `dsversioner-0.9.5/dsversioner/ObjectDataset.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.4/dsversioner/ObjectDatasetFileSystemStorage.py` & `dsversioner-0.9.5/dsversioner/ObjectDatasetFileSystemStorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 This module
 """
 
 import json
 import os
 import shutil
 from pathlib import Path
-from typing import Type
 
 from .Storage import RecordStorageFormats
 from .Exceptions import DatasetExistsException, InvalidRecordStorageFormatException, \
     DatasetVersionDoesNotExistException
 from .FileSystemStorage import FileSystemStorage
 from .ObjectDatasetMetadata import ObjectDatasetMetadata
 from .ObjectDatasetStorage import ObjectDatasetVersionStorage, ObjectDatasetMetadataStorage, \
@@ -21,19 +20,20 @@
 
 class FileSystemObjectDatasetVersionStorageSchema(JsonSerializable):
     """
     This class
     """
 
     def __init__(self,
-                 versions: list[ObjectDatasetVersion] = None):
+                 #versions: list[ObjectDatasetVersion] = None):
+                 versions: list = None):
         self._versions = versions
 
     @property
-    def versions(self) -> list[ObjectDatasetVersion]:
+    def versions(self) -> list: #list[ObjectDatasetVersion]:
         """
 
         :return:
         """
         return self._versions
 
     def to_json(self) -> dict:
@@ -262,19 +262,21 @@
 
 
 class FileSystemObjectDatasetMetadataStorageSchema(JsonSerializable):
     """
     This class...
     """
 
-    def __init__(self, metadata: list[FileSystemObjectDatasetMetadataStorageContainerSchema] = None):
+    def __init__(self,
+                 #metadata: list[FileSystemObjectDatasetMetadataStorageContainerSchema] = None):
+                 metadata: list= None):
         self._metadata = metadata
 
     @property
-    def metadata(self) -> list[FileSystemObjectDatasetMetadataStorageContainerSchema]:
+    def metadata(self) -> list: #list[FileSystemObjectDatasetMetadataStorageContainerSchema]:
         """
 
         :return:
         """
         return self._metadata
 
     def to_json(self) -> dict:
```

### Comparing `dsversioner-0.9.4/dsversioner/ObjectDatasetMetadata.py` & `dsversioner-0.9.5/dsversioner/ObjectDatasetMetadata.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.4/dsversioner/ObjectDatasetRecordData.py` & `dsversioner-0.9.5/dsversioner/ObjectDatasetRecordData.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.4/dsversioner/ObjectDatasetStorage.py` & `dsversioner-0.9.5/dsversioner/ObjectDatasetStorage.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.4/dsversioner/ObjectDatasetVersion.py` & `dsversioner-0.9.5/dsversioner/ObjectDatasetVersion.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.4/dsversioner/Serializable.py` & `dsversioner-0.9.5/dsversioner/Serializable.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.4/dsversioner/Storage.py` & `dsversioner-0.9.5/dsversioner/Storage.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.4/dsversioner/__init__.py` & `dsversioner-0.9.5/dsversioner/__init__.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.4/LICENSE` & `dsversioner-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.4/pyproject.toml` & `dsversioner-0.9.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "dsversioner"
-version = "0.9.4"
+version = "0.9.5"
 authors = [
   { name="Maxim Dernovoi", email="author@example.com" },
 ]
 description = "Flexible and extensible dataset versioning."
 readme = "README.md"
 license = {file = "LICENSE"}
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 # in synch with requirements.txt
 dependencies = [
```

### Comparing `dsversioner-0.9.4/PKG-INFO` & `dsversioner-0.9.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsversioner
-Version: 0.9.4
+Version: 0.9.5
 Summary: Flexible and extensible dataset versioning.
 Author-email: Maxim Dernovoi <author@example.com>
 License: MIT License
         
         Copyright (c) 2023 Maxim Dernovoi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,15 +24,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: pandas==2.0.1
 Requires-Dist: pyarrow==12.0.0
 Description-Content-Type: text/markdown
 
 # dsversioner
 
 :construction: **Currently under construction** :construction:
```

