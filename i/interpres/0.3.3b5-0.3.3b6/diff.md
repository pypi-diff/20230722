# Comparing `tmp/interpres-0.3.3b5.tar.gz` & `tmp/interpres-0.3.3b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interpres-0.3.3b5.tar", last modified: Sat Jul 22 14:25:56 2023, max compression
+gzip compressed data, was "interpres-0.3.3b6.tar", last modified: Sat Jul 22 14:30:38 2023, max compression
```

## Comparing `interpres-0.3.3b5.tar` & `interpres-0.3.3b6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 14:25:56.533558 interpres-0.3.3b5/
--rw-r--r--   0 waser     (1000) waser     (1000)    16725 2023-03-02 14:55:14.000000 interpres-0.3.3b5/LICENSE
--rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 14:25:56.533558 interpres-0.3.3b5/PKG-INFO
--rw-r--r--   0 waser     (1000) waser     (1000)     8589 2023-03-14 11:37:33.000000 interpres-0.3.3b5/README.md
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 14:25:56.533558 interpres-0.3.3b5/interpres.egg-info/
--rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 14:25:56.000000 interpres-0.3.3b5/interpres.egg-info/PKG-INFO
--rw-r--r--   0 waser     (1000) waser     (1000)      373 2023-07-22 14:25:56.000000 interpres-0.3.3b5/interpres.egg-info/SOURCES.txt
--rw-r--r--   0 waser     (1000) waser     (1000)        1 2023-07-22 14:25:56.000000 interpres-0.3.3b5/interpres.egg-info/dependency_links.txt
--rw-r--r--   0 waser     (1000) waser     (1000)       51 2023-07-22 14:25:56.000000 interpres-0.3.3b5/interpres.egg-info/entry_points.txt
--rw-r--r--   0 waser     (1000) waser     (1000)      136 2023-07-22 14:25:56.000000 interpres-0.3.3b5/interpres.egg-info/requires.txt
--rw-r--r--   0 waser     (1000) waser     (1000)       11 2023-07-22 14:25:56.000000 interpres-0.3.3b5/interpres.egg-info/top_level.txt
--rw-r--r--   0 waser     (1000) waser     (1000)      731 2023-03-13 21:07:52.000000 interpres-0.3.3b5/pyproject.toml
--rw-r--r--   0 waser     (1000) waser     (1000)       38 2023-07-22 14:25:56.533558 interpres-0.3.3b5/setup.cfg
--rw-r--r--   0 waser     (1000) waser     (1000)     4037 2023-07-22 00:45:47.000000 interpres-0.3.3b5/setup.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 14:25:56.533558 interpres-0.3.3b5/translator/
--rw-r--r--   0 waser     (1000) waser     (1000)      140 2023-07-22 14:24:41.000000 interpres-0.3.3b5/translator/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      165 2023-03-02 14:55:14.000000 interpres-0.3.3b5/translator/__main__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     3038 2023-03-11 23:51:51.000000 interpres-0.3.3b5/translator/language.py
--rw-r--r--   0 waser     (1000) waser     (1000)    29259 2023-07-22 12:50:01.000000 interpres-0.3.3b5/translator/main.py
--rw-r--r--   0 waser     (1000) waser     (1000)     1953 2023-07-22 14:24:28.000000 interpres-0.3.3b5/translator/translate.py
--rw-r--r--   0 waser     (1000) waser     (1000)      714 2023-03-04 01:47:57.000000 interpres-0.3.3b5/translator/utils.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 14:30:38.917518 interpres-0.3.3b6/
+-rw-r--r--   0 waser     (1000) waser     (1000)    16725 2023-03-02 14:55:14.000000 interpres-0.3.3b6/LICENSE
+-rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 14:30:38.917518 interpres-0.3.3b6/PKG-INFO
+-rw-r--r--   0 waser     (1000) waser     (1000)     8589 2023-03-14 11:37:33.000000 interpres-0.3.3b6/README.md
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 14:30:38.917518 interpres-0.3.3b6/interpres.egg-info/
+-rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 14:30:38.000000 interpres-0.3.3b6/interpres.egg-info/PKG-INFO
+-rw-r--r--   0 waser     (1000) waser     (1000)      373 2023-07-22 14:30:38.000000 interpres-0.3.3b6/interpres.egg-info/SOURCES.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)        1 2023-07-22 14:30:38.000000 interpres-0.3.3b6/interpres.egg-info/dependency_links.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)       51 2023-07-22 14:30:38.000000 interpres-0.3.3b6/interpres.egg-info/entry_points.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)      136 2023-07-22 14:30:38.000000 interpres-0.3.3b6/interpres.egg-info/requires.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)       11 2023-07-22 14:30:38.000000 interpres-0.3.3b6/interpres.egg-info/top_level.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)      731 2023-03-13 21:07:52.000000 interpres-0.3.3b6/pyproject.toml
+-rw-r--r--   0 waser     (1000) waser     (1000)       38 2023-07-22 14:30:38.917518 interpres-0.3.3b6/setup.cfg
+-rw-r--r--   0 waser     (1000) waser     (1000)     4037 2023-07-22 00:45:47.000000 interpres-0.3.3b6/setup.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 14:30:38.917518 interpres-0.3.3b6/translator/
+-rw-r--r--   0 waser     (1000) waser     (1000)      140 2023-07-22 14:29:23.000000 interpres-0.3.3b6/translator/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      165 2023-03-02 14:55:14.000000 interpres-0.3.3b6/translator/__main__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     3038 2023-03-11 23:51:51.000000 interpres-0.3.3b6/translator/language.py
+-rw-r--r--   0 waser     (1000) waser     (1000)    29259 2023-07-22 12:50:01.000000 interpres-0.3.3b6/translator/main.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2058 2023-07-22 14:29:16.000000 interpres-0.3.3b6/translator/translate.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      714 2023-03-04 01:47:57.000000 interpres-0.3.3b6/translator/utils.py
```

### Comparing `interpres-0.3.3b5/LICENSE` & `interpres-0.3.3b6/LICENSE`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b5/PKG-INFO` & `interpres-0.3.3b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpres
-Version: 0.3.3b5
+Version: 0.3.3b6
 Summary: Translate from one language to another.
 Home-page: https://github.com/wasertech/Translator
 Author: Danny Waser
 License: LICENSE
 Project-URL: Documentation, https://github.com/wasertech/Translator/blob/main/README.md
 Project-URL: Code, https://github.com/wasertech/Translator
 Project-URL: Issue tracker, https://github.com/wasertech/Translator/issues
```

### Comparing `interpres-0.3.3b5/README.md` & `interpres-0.3.3b6/README.md`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b5/interpres.egg-info/PKG-INFO` & `interpres-0.3.3b6/interpres.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpres
-Version: 0.3.3b5
+Version: 0.3.3b6
 Summary: Translate from one language to another.
 Home-page: https://github.com/wasertech/Translator
 Author: Danny Waser
 License: LICENSE
 Project-URL: Documentation, https://github.com/wasertech/Translator/blob/main/README.md
 Project-URL: Code, https://github.com/wasertech/Translator
 Project-URL: Issue tracker, https://github.com/wasertech/Translator/issues
```

### Comparing `interpres-0.3.3b5/pyproject.toml` & `interpres-0.3.3b6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b5/setup.py` & `interpres-0.3.3b6/setup.py`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b5/translator/language.py` & `interpres-0.3.3b6/translator/language.py`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b5/translator/main.py` & `interpres-0.3.3b6/translator/main.py`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b5/translator/translate.py` & `interpres-0.3.3b6/translator/translate.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,41 +3,42 @@
 import logging
 
 logger = logging.getLogger(__name__)
 
 class Translator:
     
     def __init__(self, source_language, target_language, max_length=500, model_id="facebook/nllb-200-distilled-600M", pipe_line="translation", batch_size=128, n_proc=4) -> None:
-        logger.debug("Initializing Translator...")
+        self.logger = logger or logging.getLogger(__name__)
+        self.logger.debug("Initializing Translator...")
         self.source = source_language
-        logger.debug(f"{self.source}")
+        self.logger.debug(f"{self.source}")
         self.target = target_language
-        logger.debug(f"{self.target}")
+        self.logger.debug(f"{self.target}")
         self.model_id = model_id
-        logger.debug(f"{self.model_id}")
+        self.logger.debug(f"{self.model_id}")
         self.n_proc = n_proc
         self.batch_size = batch_size
         self.device = "cuda:0" if torch.cuda.is_available() else "cpu"
-        logger.debug(f"{self.device}")
-        logger.debug("Loading model...")
+        self.logger.debug(f"{self.device}")
+        self.logger.debug("Loading model...")
         self.model = AutoModelForSeq2SeqLM.from_pretrained(model_id)
-        logger.debug("Loading tokenizer...")
+        self.logger.debug("Loading tokenizer...")
         self.tokenizer = AutoTokenizer.from_pretrained(model_id)
-        logger.debug("Setting up translation pipeline...")
+        self.logger.debug("Setting up translation pipeline...")
         self.translator = pipeline(
             "translation",
             model=self.model,
             tokenizer=self.tokenizer,
             src_lang=source_language,
             tgt_lang=target_language,
             max_length=max_length,
             device=self.device,
             #device_map="auto",
         )
-        logger.debug("Translator has been successfully loaded.")
+        self.logger.debug("Translator has been successfully loaded.")
 
     def translate(self, to_translate, num_workers=None, batch_size=None):
         
         if not num_workers: num_workers=self.n_proc
         if not batch_size: batch_size=self.batch_size
 
         try:
```

### Comparing `interpres-0.3.3b5/translator/utils.py` & `interpres-0.3.3b6/translator/utils.py`

 * *Files identical despite different names*

