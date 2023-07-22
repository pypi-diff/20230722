# Comparing `tmp/irisml-tasks-azure-computervision-0.0.6.tar.gz` & `tmp/irisml-tasks-azure-computervision-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml-tasks-azure-computervision-0.0.6.tar", last modified: Fri Jul 21 00:57:49 2023, max compression
+gzip compressed data, was "irisml-tasks-azure-computervision-0.0.7.tar", last modified: Sat Jul 22 05:32:57 2023, max compression
```

## Comparing `irisml-tasks-azure-computervision-0.0.6.tar` & `irisml-tasks-azure-computervision-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:57:49.539739 irisml-tasks-azure-computervision-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-21 00:57:49.539739 irisml-tasks-azure-computervision-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:57:49.535739 irisml-tasks-azure-computervision-0.0.6/irisml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:57:49.535739 irisml-tasks-azure-computervision-0.0.6/irisml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/irisml/tasks/create_azure_computervision_caption_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/irisml/tasks/create_azure_computervision_classification_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/irisml/tasks/create_azure_computervision_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/irisml/tasks/create_azure_computervision_ocr_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/irisml/tasks/delete_azure_computervision_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11782 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/irisml/tasks/train_azure_computervision_custom_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:57:49.535739 irisml-tasks-azure-computervision-0.0.6/irisml_tasks_azure_computervision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-21 00:57:49.000000 irisml-tasks-azure-computervision-0.0.6/irisml_tasks_azure_computervision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-21 00:57:49.000000 irisml-tasks-azure-computervision-0.0.6/irisml_tasks_azure_computervision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 00:57:49.000000 irisml-tasks-azure-computervision-0.0.6/irisml_tasks_azure_computervision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 00:57:49.000000 irisml-tasks-azure-computervision-0.0.6/irisml_tasks_azure_computervision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 00:57:49.000000 irisml-tasks-azure-computervision-0.0.6/irisml_tasks_azure_computervision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-21 00:57:49.539739 irisml-tasks-azure-computervision-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:57:49.539739 irisml-tasks-azure-computervision-0.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/test/test_create_azure_computervision_caption_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/test/test_create_azure_computervision_classification_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/test/test_create_azure_computervision_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/test/test_create_azure_computervision_ocr_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/test/test_delete_azure_computervision_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-21 00:55:21.000000 irisml-tasks-azure-computervision-0.0.6/test/test_train_azure_computervision_custom_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:32:57.049574 irisml-tasks-azure-computervision-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-22 05:30:43.000000 irisml-tasks-azure-computervision-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-22 05:32:57.049574 irisml-tasks-azure-computervision-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-22 05:30:43.000000 irisml-tasks-azure-computervision-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:32:57.045574 irisml-tasks-azure-computervision-0.0.7/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:32:57.045574 irisml-tasks-azure-computervision-0.0.7/irisml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-22 05:30:43.000000 irisml-tasks-azure-computervision-0.0.7/irisml/tasks/create_azure_computervision_caption_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-22 05:30:43.000000 irisml-tasks-azure-computervision-0.0.7/irisml/tasks/create_azure_computervision_classification_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-22 05:30:43.000000 irisml-tasks-azure-computervision-0.0.7/irisml/tasks/create_azure_computervision_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-22 05:30:43.000000 irisml-tasks-azure-computervision-0.0.7/irisml/tasks/create_azure_computervision_ocr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-22 05:30:43.000000 irisml-tasks-azure-computervision-0.0.7/irisml/tasks/create_azure_computervision_product_recognizer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-22 05:30:43.000000 irisml-tasks-azure-computervision-0.0.7/irisml/tasks/delete_azure_computervision_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11782 2023-07-22 05:30:43.000000 irisml-tasks-azure-computervision-0.0.7/irisml/tasks/train_azure_computervision_custom_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:32:57.045574 irisml-tasks-azure-computervision-0.0.7/irisml_tasks_azure_computervision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-22 05:32:57.000000 irisml-tasks-azure-computervision-0.0.7/irisml_tasks_azure_computervision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-22 05:32:57.000000 irisml-tasks-azure-computervision-0.0.7/irisml_tasks_azure_computervision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 05:32:57.000000 irisml-tasks-azure-computervision-0.0.7/irisml_tasks_azure_computervision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-22 05:32:57.000000 irisml-tasks-azure-computervision-0.0.7/irisml_tasks_azure_computervision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-22 05:32:57.000000 irisml-tasks-azure-computervision-0.0.7/irisml_tasks_azure_computervision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-22 05:30:43.000000 irisml-tasks-azure-computervision-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-22 05:32:57.049574 irisml-tasks-azure-computervision-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:32:57.049574 irisml-tasks-azure-computervision-0.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-22 05:30:43.000000 irisml-tasks-azure-computervision-0.0.7/test/test_create_azure_computervision_caption_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-22 05:30:43.000000 irisml-tasks-azure-computervision-0.0.7/test/test_create_azure_computervision_classification_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-22 05:30:43.000000 irisml-tasks-azure-computervision-0.0.7/test/test_create_azure_computervision_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-22 05:30:43.000000 irisml-tasks-azure-computervision-0.0.7/test/test_create_azure_computervision_ocr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-22 05:30:43.000000 irisml-tasks-azure-computervision-0.0.7/test/test_create_azure_computervision_product_recognizer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-22 05:30:43.000000 irisml-tasks-azure-computervision-0.0.7/test/test_delete_azure_computervision_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-22 05:30:43.000000 irisml-tasks-azure-computervision-0.0.7/test/test_train_azure_computervision_custom_model.py
```

### Comparing `irisml-tasks-azure-computervision-0.0.6/LICENSE` & `irisml-tasks-azure-computervision-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.6/PKG-INFO` & `irisml-tasks-azure-computervision-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-azure-computervision
-Version: 0.0.6
+Version: 0.0.7
 Summary: Azure Computer Vision API tasks for IrisML
 Home-page: https://github.com/microsoft/irisml-tasks-azure-computervision
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-azure-computervision-0.0.6/README.md` & `irisml-tasks-azure-computervision-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.6/irisml/tasks/create_azure_computervision_caption_model.py` & `irisml-tasks-azure-computervision-0.0.7/irisml/tasks/create_azure_computervision_caption_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.6/irisml/tasks/create_azure_computervision_classification_model.py` & `irisml-tasks-azure-computervision-0.0.7/irisml/tasks/create_azure_computervision_classification_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.6/irisml/tasks/create_azure_computervision_custom_model.py` & `irisml-tasks-azure-computervision-0.0.7/irisml/tasks/create_azure_computervision_custom_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.6/irisml/tasks/create_azure_computervision_ocr_model.py` & `irisml-tasks-azure-computervision-0.0.7/irisml/tasks/create_azure_computervision_ocr_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.6/irisml/tasks/delete_azure_computervision_custom_model.py` & `irisml-tasks-azure-computervision-0.0.7/irisml/tasks/delete_azure_computervision_custom_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.6/irisml/tasks/train_azure_computervision_custom_model.py` & `irisml-tasks-azure-computervision-0.0.7/irisml/tasks/train_azure_computervision_custom_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.6/irisml_tasks_azure_computervision.egg-info/PKG-INFO` & `irisml-tasks-azure-computervision-0.0.7/irisml_tasks_azure_computervision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-azure-computervision
-Version: 0.0.6
+Version: 0.0.7
 Summary: Azure Computer Vision API tasks for IrisML
 Home-page: https://github.com/microsoft/irisml-tasks-azure-computervision
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-azure-computervision-0.0.6/irisml_tasks_azure_computervision.egg-info/SOURCES.txt` & `irisml-tasks-azure-computervision-0.0.7/irisml_tasks_azure_computervision.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 README.md
 pyproject.toml
 setup.cfg
 irisml/tasks/create_azure_computervision_caption_model.py
 irisml/tasks/create_azure_computervision_classification_model.py
 irisml/tasks/create_azure_computervision_custom_model.py
 irisml/tasks/create_azure_computervision_ocr_model.py
+irisml/tasks/create_azure_computervision_product_recognizer_model.py
 irisml/tasks/delete_azure_computervision_custom_model.py
 irisml/tasks/train_azure_computervision_custom_model.py
 irisml_tasks_azure_computervision.egg-info/PKG-INFO
 irisml_tasks_azure_computervision.egg-info/SOURCES.txt
 irisml_tasks_azure_computervision.egg-info/dependency_links.txt
 irisml_tasks_azure_computervision.egg-info/requires.txt
 irisml_tasks_azure_computervision.egg-info/top_level.txt
 test/test_create_azure_computervision_caption_model.py
 test/test_create_azure_computervision_classification_model.py
 test/test_create_azure_computervision_custom_model.py
 test/test_create_azure_computervision_ocr_model.py
+test/test_create_azure_computervision_product_recognizer_model.py
 test/test_delete_azure_computervision_custom_model.py
 test/test_train_azure_computervision_custom_model.py
```

### Comparing `irisml-tasks-azure-computervision-0.0.6/setup.cfg` & `irisml-tasks-azure-computervision-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = irisml-tasks-azure-computervision
-version = 0.0.6
+version = 0.0.7
 url = https://github.com/microsoft/irisml-tasks-azure-computervision
 description = Azure Computer Vision API tasks for IrisML
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = irisdev
 license = MIT
```

### Comparing `irisml-tasks-azure-computervision-0.0.6/test/test_create_azure_computervision_caption_model.py` & `irisml-tasks-azure-computervision-0.0.7/test/test_create_azure_computervision_caption_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.6/test/test_create_azure_computervision_classification_model.py` & `irisml-tasks-azure-computervision-0.0.7/test/test_create_azure_computervision_classification_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.6/test/test_create_azure_computervision_custom_model.py` & `irisml-tasks-azure-computervision-0.0.7/test/test_create_azure_computervision_custom_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.6/test/test_create_azure_computervision_ocr_model.py` & `irisml-tasks-azure-computervision-0.0.7/test/test_create_azure_computervision_ocr_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.6/test/test_delete_azure_computervision_custom_model.py` & `irisml-tasks-azure-computervision-0.0.7/test/test_delete_azure_computervision_custom_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.6/test/test_train_azure_computervision_custom_model.py` & `irisml-tasks-azure-computervision-0.0.7/test/test_train_azure_computervision_custom_model.py`

 * *Files identical despite different names*

