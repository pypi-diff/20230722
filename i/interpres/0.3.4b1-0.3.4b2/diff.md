# Comparing `tmp/interpres-0.3.4b1.tar.gz` & `tmp/interpres-0.3.4b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interpres-0.3.4b1.tar", last modified: Sat Jul 22 14:57:22 2023, max compression
+gzip compressed data, was "interpres-0.3.4b2.tar", last modified: Sat Jul 22 15:02:33 2023, max compression
```

## Comparing `interpres-0.3.4b1.tar` & `interpres-0.3.4b2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 14:57:22.818940 interpres-0.3.4b1/
--rw-r--r--   0 waser     (1000) waser     (1000)    16725 2023-03-02 14:55:14.000000 interpres-0.3.4b1/LICENSE
--rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 14:57:22.818940 interpres-0.3.4b1/PKG-INFO
--rw-r--r--   0 waser     (1000) waser     (1000)     8589 2023-03-14 11:37:33.000000 interpres-0.3.4b1/README.md
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 14:57:22.818940 interpres-0.3.4b1/interpres.egg-info/
--rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 14:57:22.000000 interpres-0.3.4b1/interpres.egg-info/PKG-INFO
--rw-r--r--   0 waser     (1000) waser     (1000)      373 2023-07-22 14:57:22.000000 interpres-0.3.4b1/interpres.egg-info/SOURCES.txt
--rw-r--r--   0 waser     (1000) waser     (1000)        1 2023-07-22 14:57:22.000000 interpres-0.3.4b1/interpres.egg-info/dependency_links.txt
--rw-r--r--   0 waser     (1000) waser     (1000)       51 2023-07-22 14:57:22.000000 interpres-0.3.4b1/interpres.egg-info/entry_points.txt
--rw-r--r--   0 waser     (1000) waser     (1000)      136 2023-07-22 14:57:22.000000 interpres-0.3.4b1/interpres.egg-info/requires.txt
--rw-r--r--   0 waser     (1000) waser     (1000)       11 2023-07-22 14:57:22.000000 interpres-0.3.4b1/interpres.egg-info/top_level.txt
--rw-r--r--   0 waser     (1000) waser     (1000)      731 2023-03-13 21:07:52.000000 interpres-0.3.4b1/pyproject.toml
--rw-r--r--   0 waser     (1000) waser     (1000)       38 2023-07-22 14:57:22.818940 interpres-0.3.4b1/setup.cfg
--rw-r--r--   0 waser     (1000) waser     (1000)     4037 2023-07-22 00:45:47.000000 interpres-0.3.4b1/setup.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 14:57:22.818940 interpres-0.3.4b1/translator/
--rw-r--r--   0 waser     (1000) waser     (1000)      140 2023-07-22 14:55:43.000000 interpres-0.3.4b1/translator/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      165 2023-03-02 14:55:14.000000 interpres-0.3.4b1/translator/__main__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     3038 2023-03-11 23:51:51.000000 interpres-0.3.4b1/translator/language.py
--rw-r--r--   0 waser     (1000) waser     (1000)    29259 2023-07-22 12:50:01.000000 interpres-0.3.4b1/translator/main.py
--rw-r--r--   0 waser     (1000) waser     (1000)     2124 2023-07-22 14:56:05.000000 interpres-0.3.4b1/translator/translate.py
--rw-r--r--   0 waser     (1000) waser     (1000)      714 2023-03-04 01:47:57.000000 interpres-0.3.4b1/translator/utils.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 15:02:33.943042 interpres-0.3.4b2/
+-rw-r--r--   0 waser     (1000) waser     (1000)    16725 2023-03-02 14:55:14.000000 interpres-0.3.4b2/LICENSE
+-rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 15:02:33.943042 interpres-0.3.4b2/PKG-INFO
+-rw-r--r--   0 waser     (1000) waser     (1000)     8589 2023-03-14 11:37:33.000000 interpres-0.3.4b2/README.md
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 15:02:33.943042 interpres-0.3.4b2/interpres.egg-info/
+-rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 15:02:33.000000 interpres-0.3.4b2/interpres.egg-info/PKG-INFO
+-rw-r--r--   0 waser     (1000) waser     (1000)      373 2023-07-22 15:02:33.000000 interpres-0.3.4b2/interpres.egg-info/SOURCES.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)        1 2023-07-22 15:02:33.000000 interpres-0.3.4b2/interpres.egg-info/dependency_links.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)       51 2023-07-22 15:02:33.000000 interpres-0.3.4b2/interpres.egg-info/entry_points.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)      136 2023-07-22 15:02:33.000000 interpres-0.3.4b2/interpres.egg-info/requires.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)       11 2023-07-22 15:02:33.000000 interpres-0.3.4b2/interpres.egg-info/top_level.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)      731 2023-03-13 21:07:52.000000 interpres-0.3.4b2/pyproject.toml
+-rw-r--r--   0 waser     (1000) waser     (1000)       38 2023-07-22 15:02:33.943042 interpres-0.3.4b2/setup.cfg
+-rw-r--r--   0 waser     (1000) waser     (1000)     4037 2023-07-22 00:45:47.000000 interpres-0.3.4b2/setup.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 15:02:33.943042 interpres-0.3.4b2/translator/
+-rw-r--r--   0 waser     (1000) waser     (1000)      140 2023-07-22 15:01:21.000000 interpres-0.3.4b2/translator/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      165 2023-03-02 14:55:14.000000 interpres-0.3.4b2/translator/__main__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     3038 2023-03-11 23:51:51.000000 interpres-0.3.4b2/translator/language.py
+-rw-r--r--   0 waser     (1000) waser     (1000)    29259 2023-07-22 12:50:01.000000 interpres-0.3.4b2/translator/main.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     2104 2023-07-22 15:00:39.000000 interpres-0.3.4b2/translator/translate.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      714 2023-03-04 01:47:57.000000 interpres-0.3.4b2/translator/utils.py
```

### Comparing `interpres-0.3.4b1/LICENSE` & `interpres-0.3.4b2/LICENSE`

 * *Files identical despite different names*

### Comparing `interpres-0.3.4b1/PKG-INFO` & `interpres-0.3.4b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpres
-Version: 0.3.4b1
+Version: 0.3.4b2
 Summary: Translate from one language to another.
 Home-page: https://github.com/wasertech/Translator
 Author: Danny Waser
 License: LICENSE
 Project-URL: Documentation, https://github.com/wasertech/Translator/blob/main/README.md
 Project-URL: Code, https://github.com/wasertech/Translator
 Project-URL: Issue tracker, https://github.com/wasertech/Translator/issues
```

### Comparing `interpres-0.3.4b1/README.md` & `interpres-0.3.4b2/README.md`

 * *Files identical despite different names*

### Comparing `interpres-0.3.4b1/interpres.egg-info/PKG-INFO` & `interpres-0.3.4b2/interpres.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpres
-Version: 0.3.4b1
+Version: 0.3.4b2
 Summary: Translate from one language to another.
 Home-page: https://github.com/wasertech/Translator
 Author: Danny Waser
 License: LICENSE
 Project-URL: Documentation, https://github.com/wasertech/Translator/blob/main/README.md
 Project-URL: Code, https://github.com/wasertech/Translator
 Project-URL: Issue tracker, https://github.com/wasertech/Translator/issues
```

### Comparing `interpres-0.3.4b1/pyproject.toml` & `interpres-0.3.4b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `interpres-0.3.4b1/setup.py` & `interpres-0.3.4b2/setup.py`

 * *Files identical despite different names*

### Comparing `interpres-0.3.4b1/translator/language.py` & `interpres-0.3.4b2/translator/language.py`

 * *Files identical despite different names*

### Comparing `interpres-0.3.4b1/translator/main.py` & `interpres-0.3.4b2/translator/main.py`

 * *Files identical despite different names*

### Comparing `interpres-0.3.4b1/translator/translate.py` & `interpres-0.3.4b2/translator/translate.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         self.model_id = model_id
         self.logger.debug(f"{self.model_id}")
         self.n_proc = n_proc
         self.batch_size = batch_size
         self.device = "cuda:0" if torch.cuda.is_available() else "cpu"
         self.logger.debug(f"{self.device}")
         self.logger.debug("Loading model...")
-        self.model = AutoModelForSeq2SeqLM.from_pretrained(model_id, max_length=max_length, device=self.device)
+        self.model = AutoModelForSeq2SeqLM.from_pretrained(model_id, max_length=max_length)
         self.logger.debug("Loading tokenizer...")
         self.tokenizer = AutoTokenizer.from_pretrained(model_id, max_length=max_length)
         self.logger.debug("Setting up translation pipeline...")
         self.translator = pipeline(
             "translation",
             model=self.model,
             tokenizer=self.tokenizer,
```

### Comparing `interpres-0.3.4b1/translator/utils.py` & `interpres-0.3.4b2/translator/utils.py`

 * *Files identical despite different names*

