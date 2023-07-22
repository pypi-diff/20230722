# Comparing `tmp/interpres-0.3.3b3.tar.gz` & `tmp/interpres-0.3.3b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interpres-0.3.3b3.tar", last modified: Sat Jul 22 00:47:11 2023, max compression
+gzip compressed data, was "interpres-0.3.3b4.tar", last modified: Sat Jul 22 14:22:06 2023, max compression
```

## Comparing `interpres-0.3.3b3.tar` & `interpres-0.3.3b4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 00:47:11.238808 interpres-0.3.3b3/
--rw-r--r--   0 waser     (1000) waser     (1000)    16725 2023-03-02 14:55:14.000000 interpres-0.3.3b3/LICENSE
--rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 00:47:11.238808 interpres-0.3.3b3/PKG-INFO
--rw-r--r--   0 waser     (1000) waser     (1000)     8589 2023-03-14 11:37:33.000000 interpres-0.3.3b3/README.md
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 00:47:11.238808 interpres-0.3.3b3/interpres.egg-info/
--rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 00:47:11.000000 interpres-0.3.3b3/interpres.egg-info/PKG-INFO
--rw-r--r--   0 waser     (1000) waser     (1000)      373 2023-07-22 00:47:11.000000 interpres-0.3.3b3/interpres.egg-info/SOURCES.txt
--rw-r--r--   0 waser     (1000) waser     (1000)        1 2023-07-22 00:47:11.000000 interpres-0.3.3b3/interpres.egg-info/dependency_links.txt
--rw-r--r--   0 waser     (1000) waser     (1000)       51 2023-07-22 00:47:11.000000 interpres-0.3.3b3/interpres.egg-info/entry_points.txt
--rw-r--r--   0 waser     (1000) waser     (1000)      136 2023-07-22 00:47:11.000000 interpres-0.3.3b3/interpres.egg-info/requires.txt
--rw-r--r--   0 waser     (1000) waser     (1000)       11 2023-07-22 00:47:11.000000 interpres-0.3.3b3/interpres.egg-info/top_level.txt
--rw-r--r--   0 waser     (1000) waser     (1000)      731 2023-03-13 21:07:52.000000 interpres-0.3.3b3/pyproject.toml
--rw-r--r--   0 waser     (1000) waser     (1000)       38 2023-07-22 00:47:11.238808 interpres-0.3.3b3/setup.cfg
--rw-r--r--   0 waser     (1000) waser     (1000)     4037 2023-07-22 00:45:47.000000 interpres-0.3.3b3/setup.py
-drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 00:47:11.238808 interpres-0.3.3b3/translator/
--rw-r--r--   0 waser     (1000) waser     (1000)      140 2023-07-22 00:45:52.000000 interpres-0.3.3b3/translator/__init__.py
--rw-r--r--   0 waser     (1000) waser     (1000)      165 2023-03-02 14:55:14.000000 interpres-0.3.3b3/translator/__main__.py
--rw-r--r--   0 waser     (1000) waser     (1000)     3038 2023-03-11 23:51:51.000000 interpres-0.3.3b3/translator/language.py
--rw-r--r--   0 waser     (1000) waser     (1000)    29033 2023-03-14 11:40:43.000000 interpres-0.3.3b3/translator/main.py
--rw-r--r--   0 waser     (1000) waser     (1000)     1950 2023-03-13 15:42:00.000000 interpres-0.3.3b3/translator/translate.py
--rw-r--r--   0 waser     (1000) waser     (1000)      714 2023-03-04 01:47:57.000000 interpres-0.3.3b3/translator/utils.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 14:22:06.537615 interpres-0.3.3b4/
+-rw-r--r--   0 waser     (1000) waser     (1000)    16725 2023-03-02 14:55:14.000000 interpres-0.3.3b4/LICENSE
+-rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 14:22:06.537615 interpres-0.3.3b4/PKG-INFO
+-rw-r--r--   0 waser     (1000) waser     (1000)     8589 2023-03-14 11:37:33.000000 interpres-0.3.3b4/README.md
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 14:22:06.537615 interpres-0.3.3b4/interpres.egg-info/
+-rw-r--r--   0 waser     (1000) waser     (1000)    11977 2023-07-22 14:22:06.000000 interpres-0.3.3b4/interpres.egg-info/PKG-INFO
+-rw-r--r--   0 waser     (1000) waser     (1000)      373 2023-07-22 14:22:06.000000 interpres-0.3.3b4/interpres.egg-info/SOURCES.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)        1 2023-07-22 14:22:06.000000 interpres-0.3.3b4/interpres.egg-info/dependency_links.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)       51 2023-07-22 14:22:06.000000 interpres-0.3.3b4/interpres.egg-info/entry_points.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)      136 2023-07-22 14:22:06.000000 interpres-0.3.3b4/interpres.egg-info/requires.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)       11 2023-07-22 14:22:06.000000 interpres-0.3.3b4/interpres.egg-info/top_level.txt
+-rw-r--r--   0 waser     (1000) waser     (1000)      731 2023-03-13 21:07:52.000000 interpres-0.3.3b4/pyproject.toml
+-rw-r--r--   0 waser     (1000) waser     (1000)       38 2023-07-22 14:22:06.537615 interpres-0.3.3b4/setup.cfg
+-rw-r--r--   0 waser     (1000) waser     (1000)     4037 2023-07-22 00:45:47.000000 interpres-0.3.3b4/setup.py
+drwxr-xr-x   0 waser     (1000) waser     (1000)        0 2023-07-22 14:22:06.537615 interpres-0.3.3b4/translator/
+-rw-r--r--   0 waser     (1000) waser     (1000)      140 2023-07-22 14:20:46.000000 interpres-0.3.3b4/translator/__init__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      165 2023-03-02 14:55:14.000000 interpres-0.3.3b4/translator/__main__.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     3038 2023-03-11 23:51:51.000000 interpres-0.3.3b4/translator/language.py
+-rw-r--r--   0 waser     (1000) waser     (1000)    29259 2023-07-22 12:50:01.000000 interpres-0.3.3b4/translator/main.py
+-rw-r--r--   0 waser     (1000) waser     (1000)     1950 2023-07-22 14:20:36.000000 interpres-0.3.3b4/translator/translate.py
+-rw-r--r--   0 waser     (1000) waser     (1000)      714 2023-03-04 01:47:57.000000 interpres-0.3.3b4/translator/utils.py
```

### Comparing `interpres-0.3.3b3/LICENSE` & `interpres-0.3.3b4/LICENSE`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b3/PKG-INFO` & `interpres-0.3.3b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpres
-Version: 0.3.3b3
+Version: 0.3.3b4
 Summary: Translate from one language to another.
 Home-page: https://github.com/wasertech/Translator
 Author: Danny Waser
 License: LICENSE
 Project-URL: Documentation, https://github.com/wasertech/Translator/blob/main/README.md
 Project-URL: Code, https://github.com/wasertech/Translator
 Project-URL: Issue tracker, https://github.com/wasertech/Translator/issues
```

### Comparing `interpres-0.3.3b3/README.md` & `interpres-0.3.3b4/README.md`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b3/interpres.egg-info/PKG-INFO` & `interpres-0.3.3b4/interpres.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpres
-Version: 0.3.3b3
+Version: 0.3.3b4
 Summary: Translate from one language to another.
 Home-page: https://github.com/wasertech/Translator
 Author: Danny Waser
 License: LICENSE
 Project-URL: Documentation, https://github.com/wasertech/Translator/blob/main/README.md
 Project-URL: Code, https://github.com/wasertech/Translator
 Project-URL: Issue tracker, https://github.com/wasertech/Translator/issues
```

### Comparing `interpres-0.3.3b3/pyproject.toml` & `interpres-0.3.3b4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b3/setup.py` & `interpres-0.3.3b4/setup.py`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b3/translator/language.py` & `interpres-0.3.3b4/translator/language.py`

 * *Files identical despite different names*

### Comparing `interpres-0.3.3b3/translator/main.py` & `interpres-0.3.3b4/translator/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     ]
 
     if args.language_list or args._from in fetch_languages:
         _log("Language list:", logger, spinner, 'info')
         if args.model_id == "facebook/nllb-200-distilled-600M":
             for l in get_nllb_lang(): print(f"- {l}")
         else:
-            raise NotImplementedError(f"{model_id=} language list not implemented.")
+            raise NotImplementedError(f"{args.model_id=} language list not implemented.")
         print()
         sys.exit(0)
 
     _from, _to, _sentences = "".join(args._from), "".join(args._to), args.sentences
     _directory, _save_path = args.directory, args.save
 
     nepoch, nproc, batch_size = args.nepoch, args.nproc, args.batch_size
@@ -475,41 +475,45 @@
             _log(f"RAM memory used by untranslated dataset: {(mem_after - mem_before):n} MB", logger, spinner, 'debug')
             time_after_2 = time.perf_counter()
             _td_2 = time_after_2 - time_before_2
             untranslated = untranslated_dataset.unique('text')
             _ut_ds = len(untranslated) # _ds - len(_translated)
             _log(f"Took {timedelta(seconds=_td_2)} second(s) to compute {_ut_ds:n} untranslated sentence(s).", logger, spinner, 'debug')
             
+            # Lets be absolutely sure we have the right amount of sentences
             assert _ds - _t_ds == _ut_ds, _log(f"{_ds=} - {_t_ds=} ({_ds - _t_ds}) != {_ut_ds=}", logger, spinner, 'error')
             
             if is_interactive and spinner: spinner.start()
             
             # Translate untranslated data
             time_before_3 = time.perf_counter()
             _log("Translating untranslated sentences...", logger, spinner, 'debug')
-                        
+            
             i, _i, _t = 0, 0, 0
             epoch_split = int(_ut_ds / nepoch)
             _log(f"Epoch size: {epoch_split:n}", logger, spinner, 'info')
 
+            # Lets be absolutely sure epoch_split is not too small or too big
             assert epoch_split > 0, _log(f"Value for {epoch_split=} is too small! Must be greater than 0.", logger, spinner, 'error')
             assert epoch_split < _ut_ds, _log(f"Value for {epoch_split=} is too big! Must be smaller than the amount of sentences to translate ({_ut_ds}).", logger, spinner, 'error')
 
             if is_interactive and spinner:
                 spinner.start()
                 spinner.text = f"Processing first epoch of {epoch_split:n} sentences by batch of {batch_size:n} ({_ut_ds:n} ({nepoch:n} epochs) total)..."
-                        
+            
             for epoch in untranslated_dataset.iter(epoch_split):
                 _t = time.perf_counter()
                 _epoch_text =  epoch['text']
                 _translated += _epoch_text
+                # Here we translate the epoch
                 translations += translate_sentence(_epoch_text, translator)
+                # Then we update statistics
                 time_meanwhile = time.perf_counter()
                 _td = time_meanwhile - _t
-                _td2 = time_meanwhile - time_before_3
+                #_td2 = time_meanwhile - time_before_3
                 i += 1
                 _i += epoch_split
                 _avg1 = epoch_split/_td
                 #_avg2 = _i/_td2
                 #_avg = (_avg1 + _avg2)/2
                 _etr = (_ut_ds - _i) / _avg1
                 update = f"Epoch {i:n}/{nepoch:n} | {_i:n}/{_ut_ds:n} ({_i/_ut_ds:.2%}) | ~{_avg1:.2f} translation(s) / second | ETR: {timedelta(seconds=_etr)} | dT: {timedelta(seconds=_td)}"
```

### Comparing `interpres-0.3.3b3/translator/translate.py` & `interpres-0.3.3b4/translator/translate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from transformers import AutoTokenizer, AutoModelForSeq2SeqLM, pipeline
 import torch
 import logging
 
-logger = logging.Logger(__file__)
+logger = logging.Logger(__name__)
 
 class Translator:
     
     def __init__(self, source_language, target_language, max_length=500, model_id="facebook/nllb-200-distilled-600M", pipe_line="translation", batch_size=128, n_proc=4) -> None:
         logger.debug("Initializing Translator...")
         self.source = source_language
         logger.debug(f"{self.source}")
```

### Comparing `interpres-0.3.3b3/translator/utils.py` & `interpres-0.3.3b4/translator/utils.py`

 * *Files identical despite different names*

