# Comparing `tmp/interpres-0.3.3b4.tar.gz` & `tmp/interpres-0.3.3b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interpres-0.3.3b4.tar", last modified: Sat Jul 22 14:22:06 2023, max compression
+gzip compressed data, was "interpres-0.3.3b5.tar", last modified: Sat Jul 22 14:25:56 2023, max compression
```

## Comparing `interpres-0.3.3b4.tar` & `interpres-0.3.3b5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 14:22:06.537615 interpres-0.3.3b4/
--rw-r--r--   0 waser     (1000) waser     (1000)    16725 2023-03-02 14:55:14.000000 interpres-0.3.3b4/LICENSE
--rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 14:22:06.537615 interpres-0.3.3b4/PKG-INFO
--rw-r--r--   0 waser     (1000) waser     (1000)     8589 2023-03-14 11:37:33.000000 interpres-0.3.3b4/README.md
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 14:22:06.537615 interpres-0.3.3b4/interpres.egg-info/
--rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 14:22:06.000000 interpres-0.3.3b4/interpres.egg-info/PKG-INFO
--rw-r--r--   0 waser     (1000) waser     (1000)      373 2023-07-22 14:22:06.000000 interpres-0.3.3b4/interpres.egg-info/SOURCES.txt
--rw-r--r--   0 waser     (1000) waser     (1000)        1 2023-07-22 14:22:06.000000 interpres-0.3.3b4/interpres.egg-info/dependency_links.txt
--rw-r--r--   0 waser     (1000) waser     (1000)       51 2023-07-22 14:22:06.000000 interpres-0.3.3b4/interpres.egg-info/entry_points.txt
--rw-r--r--   0 waser     (1000) waser     (1000)      136 2023-07-22 14:22:06.000000 interpres-0.3.3b4/interpres.egg-info/requires.txt
--rw-r--r--   0 waser     (1000) waser     (1000)       11 2023-07-22 14:22:06.000000 interpres-0.3.3b4/interpres.egg-info/top_level.txt
--rw-r--r--   0 waser     (1000) waser     (1000)      731 2023-03-13 21:07:52.000000 interpres-0.3.3b4/pyproject.toml
--rw-r--r--   0 waser     (1000) waser     (1000)       38 2023-07-22 14:22:06.537615 interpres-0.3.3b4/setup.cfg
--rw-r--r--   0 waser     (1000) waser     (1000)     4037 2023-07-22 00:45:47.000000 interpres-0.3.3b4/setup.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 14:22:06.537615 interpres-0.3.3b4/translator/
--rw-r--r--   0 waser     (1000) waser     (1000)      140 2023-07-22 14:20:46.000000 interpres-0.3.3b4/translator/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      165 2023-03-02 14:55:14.000000 interpres-0.3.3b4/translator/__main__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     3038 2023-03-11 23:51:51.000000 interpres-0.3.3b4/translator/language.py
--rw-r--r--   0 waser     (1000) waser     (1000)    29259 2023-07-22 12:50:01.000000 interpres-0.3.3b4/translator/main.py
--rw-r--r--   0 waser     (1000) waser     (1000)     1950 2023-07-22 14:20:36.000000 interpres-0.3.3b4/translator/translate.py
--rw-r--r--   0 waser     (1000) waser     (1000)      714 2023-03-04 01:47:57.000000 interpres-0.3.3b4/translator/utils.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 14:25:56.533558 interpres-0.3.3b5/
+-rw-r--r--   0 waser     (1000) waser     (1000)    16725 2023-03-02 14:55:14.000000 interpres-0.3.3b5/LICENSE
+-rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 14:25:56.533558 interpres-0.3.3b5/PKG-INFO
+-rw-r--r--   0 waser     (1000) waser     (1000)     8589 2023-03-14 11:37:33.000000 interpres-0.3.3b5/README.md
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 14:25:56.533558 interpres-0.3.3b5/interpres.egg-info/
+-rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 14:25:56.000000 interpres-0.3.3b5/interpres.egg-info/PKG-INFO
+-rw-r--r--   0 waser     (1000) waser     (1000)      373 2023-07-22 14:25:56.000000 interpres-0.3.3b5/interpres.egg-info/SOURCES.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)        1 2023-07-22 14:25:56.000000 interpres-0.3.3b5/interpres.egg-info/dependency_links.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)       51 2023-07-22 14:25:56.000000 interpres-0.3.3b5/interpres.egg-info/entry_points.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)      136 2023-07-22 14:25:56.000000 interpres-0.3.3b5/interpres.egg-info/requires.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)       11 2023-07-22 14:25:56.000000 interpres-0.3.3b5/interpres.egg-info/top_level.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)      731 2023-03-13 21:07:52.000000 interpres-0.3.3b5/pyproject.toml
+-rw-r--r--   0 waser     (1000) waser     (1000)       38 2023-07-22 14:25:56.533558 interpres-0.3.3b5/setup.cfg
+-rw-r--r--   0 waser     (1000) waser     (1000)     4037 2023-07-22 00:45:47.000000 interpres-0.3.3b5/setup.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 14:25:56.533558 interpres-0.3.3b5/translator/
+-rw-r--r--   0 waser     (1000) waser     (1000)      140 2023-07-22 14:24:41.000000 interpres-0.3.3b5/translator/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      165 2023-03-02 14:55:14.000000 interpres-0.3.3b5/translator/__main__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     3038 2023-03-11 23:51:51.000000 interpres-0.3.3b5/translator/language.py
+-rw-r--r--   0 waser     (1000) waser     (1000)    29259 2023-07-22 12:50:01.000000 interpres-0.3.3b5/translator/main.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     1953 2023-07-22 14:24:28.000000 interpres-0.3.3b5/translator/translate.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      714 2023-03-04 01:47:57.000000 interpres-0.3.3b5/translator/utils.py
```

### Comparing `interpres-0.3.3b4/LICENSE` & `interpres-0.3.3b5/LICENSE`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b4/PKG-INFO` & `interpres-0.3.3b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpres
-Version: 0.3.3b4
+Version: 0.3.3b5
 Summary: Translate from one language to another.
 Home-page: https://github.com/wasertech/Translator
 Author: Danny Waser
 License: LICENSE
 Project-URL: Documentation, https://github.com/wasertech/Translator/blob/main/README.md
 Project-URL: Code, https://github.com/wasertech/Translator
 Project-URL: Issue tracker, https://github.com/wasertech/Translator/issues
```

### Comparing `interpres-0.3.3b4/README.md` & `interpres-0.3.3b5/README.md`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b4/interpres.egg-info/PKG-INFO` & `interpres-0.3.3b5/interpres.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpres
-Version: 0.3.3b4
+Version: 0.3.3b5
 Summary: Translate from one language to another.
 Home-page: https://github.com/wasertech/Translator
 Author: Danny Waser
 License: LICENSE
 Project-URL: Documentation, https://github.com/wasertech/Translator/blob/main/README.md
 Project-URL: Code, https://github.com/wasertech/Translator
 Project-URL: Issue tracker, https://github.com/wasertech/Translator/issues
```

### Comparing `interpres-0.3.3b4/pyproject.toml` & `interpres-0.3.3b5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b4/setup.py` & `interpres-0.3.3b5/setup.py`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b4/translator/language.py` & `interpres-0.3.3b5/translator/language.py`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b4/translator/main.py` & `interpres-0.3.3b5/translator/main.py`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b4/translator/translate.py` & `interpres-0.3.3b5/translator/translate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from transformers import AutoTokenizer, AutoModelForSeq2SeqLM, pipeline
 import torch
 import logging
 
-logger = logging.Logger(__name__)
+logger = logging.getLogger(__name__)
 
 class Translator:
     
     def __init__(self, source_language, target_language, max_length=500, model_id="facebook/nllb-200-distilled-600M", pipe_line="translation", batch_size=128, n_proc=4) -> None:
         logger.debug("Initializing Translator...")
         self.source = source_language
         logger.debug(f"{self.source}")
```

### Comparing `interpres-0.3.3b4/translator/utils.py` & `interpres-0.3.3b5/translator/utils.py`

 * *Files identical despite different names*

