# Comparing `tmp/sqlpiece-0.1.0.tar.gz` & `tmp/sqlpiece-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlpiece-0.1.0.tar", last modified: Thu Jul 20 09:51:10 2023, max compression
+gzip compressed data, was "sqlpiece-0.1.1.tar", last modified: Sat Jul 22 10:47:07 2023, max compression
```

## Comparing `sqlpiece-0.1.0.tar` & `sqlpiece-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-07-20 09:51:10.932291 sqlpiece-0.1.0/
--rw-rw-r--   0 haris     (1000) haris     (1000)      883 2023-07-20 09:51:10.932291 sqlpiece-0.1.0/PKG-INFO
--rw-rw-r--   0 haris     (1000) haris     (1000)       48 2023-07-14 12:59:28.000000 sqlpiece-0.1.0/README.md
--rw-rw-r--   0 haris     (1000) haris     (1000)       38 2023-07-20 09:51:10.932291 sqlpiece-0.1.0/setup.cfg
--rw-rw-r--   0 haris     (1000) haris     (1000)     1309 2023-07-20 09:47:56.000000 sqlpiece-0.1.0/setup.py
-drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-07-20 09:51:10.916290 sqlpiece-0.1.0/src/
-drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-07-20 09:51:10.916290 sqlpiece-0.1.0/src/sqlpiece/
-drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-07-20 09:51:10.916290 sqlpiece-0.1.0/src/sqlpiece/SQLPieceBPE/
--rw-rw-r--   0 haris     (1000) haris     (1000)       35 2023-07-14 13:05:31.000000 sqlpiece-0.1.0/src/sqlpiece/SQLPieceBPE/__init__.py
--rw-rw-r--   0 haris     (1000) haris     (1000)     6210 2023-07-20 07:40:39.000000 sqlpiece-0.1.0/src/sqlpiece/SQLPieceBPE/tokenizer.py
-drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-07-20 09:51:10.920291 sqlpiece-0.1.0/src/sqlpiece/SQLPieceBPE/vocab/
--rw-rw-r--   0 haris     (1000) haris     (1000)  1042827 2023-07-20 07:28:11.000000 sqlpiece-0.1.0/src/sqlpiece/SQLPieceBPE/vocab/bpe_sql_vocab.json
--rw-rw-r--   0 haris     (1000) haris     (1000)   456318 2023-07-14 12:59:28.000000 sqlpiece-0.1.0/src/sqlpiece/SQLPieceBPE/vocab/gpt2_merges.txt
--rw-rw-r--   0 haris     (1000) haris     (1000)   798156 2023-07-14 12:59:28.000000 sqlpiece-0.1.0/src/sqlpiece/SQLPieceBPE/vocab/gpt2_vocab.json
--rw-rw-r--   0 haris     (1000) haris     (1000)      408 2023-07-14 12:59:28.000000 sqlpiece-0.1.0/src/sqlpiece/SQLPieceBPE/vocab/sql_vocab.pkl
-drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-07-20 09:51:10.932291 sqlpiece-0.1.0/src/sqlpiece/SQLPieceWPE/
--rw-rw-r--   0 haris     (1000) haris     (1000)       35 2023-07-14 13:05:59.000000 sqlpiece-0.1.0/src/sqlpiece/SQLPieceWPE/__init__.py
--rw-rw-r--   0 haris     (1000) haris     (1000) 14083579 2023-07-14 13:06:59.000000 sqlpiece-0.1.0/src/sqlpiece/SQLPieceWPE/lookup_dict.pkl
--rw-rw-r--   0 haris     (1000) haris     (1000)    63879 2023-07-14 13:06:53.000000 sqlpiece-0.1.0/src/sqlpiece/SQLPieceWPE/no_morph_vocab.txt
--rw-rw-r--   0 haris     (1000) haris     (1000)     4776 2023-07-15 03:40:24.000000 sqlpiece-0.1.0/src/sqlpiece/SQLPieceWPE/tokenizer.py
--rw-rw-r--   0 haris     (1000) haris     (1000)   190673 2023-07-14 13:06:53.000000 sqlpiece-0.1.0/src/sqlpiece/SQLPieceWPE/with_morph_vocab.txt
--rw-rw-r--   0 haris     (1000) haris     (1000)       76 2023-07-20 09:47:21.000000 sqlpiece-0.1.0/src/sqlpiece/__init__.py
-drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-07-20 09:51:10.916290 sqlpiece-0.1.0/src/sqlpiece.egg-info/
--rw-rw-r--   0 haris     (1000) haris     (1000)      883 2023-07-20 09:51:10.000000 sqlpiece-0.1.0/src/sqlpiece.egg-info/PKG-INFO
--rw-rw-r--   0 haris     (1000) haris     (1000)      718 2023-07-20 09:51:10.000000 sqlpiece-0.1.0/src/sqlpiece.egg-info/SOURCES.txt
--rw-rw-r--   0 haris     (1000) haris     (1000)        1 2023-07-20 09:51:10.000000 sqlpiece-0.1.0/src/sqlpiece.egg-info/dependency_links.txt
--rw-rw-r--   0 haris     (1000) haris     (1000)       26 2023-07-20 09:51:10.000000 sqlpiece-0.1.0/src/sqlpiece.egg-info/requires.txt
--rw-rw-r--   0 haris     (1000) haris     (1000)        9 2023-07-20 09:51:10.000000 sqlpiece-0.1.0/src/sqlpiece.egg-info/top_level.txt
-drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-07-20 09:51:10.932291 sqlpiece-0.1.0/tests/
--rw-rw-r--   0 haris     (1000) haris     (1000)      163 2023-07-18 15:34:29.000000 sqlpiece-0.1.0/tests/test_sqlpiecebpe.py
+drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-07-22 10:47:07.507140 sqlpiece-0.1.1/
+-rw-rw-r--   0 haris     (1000) haris     (1000)      883 2023-07-22 10:47:07.507140 sqlpiece-0.1.1/PKG-INFO
+-rw-rw-r--   0 haris     (1000) haris     (1000)       48 2023-07-14 12:59:28.000000 sqlpiece-0.1.1/README.md
+-rw-rw-r--   0 haris     (1000) haris     (1000)       38 2023-07-22 10:47:07.507140 sqlpiece-0.1.1/setup.cfg
+-rw-rw-r--   0 haris     (1000) haris     (1000)     1309 2023-07-22 10:41:07.000000 sqlpiece-0.1.1/setup.py
+drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-07-22 10:47:07.491140 sqlpiece-0.1.1/src/
+drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-07-22 10:47:07.491140 sqlpiece-0.1.1/src/sqlpiece/
+drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-07-22 10:47:07.491140 sqlpiece-0.1.1/src/sqlpiece/SQLPieceBPE/
+-rw-rw-r--   0 haris     (1000) haris     (1000)       35 2023-07-14 13:05:31.000000 sqlpiece-0.1.1/src/sqlpiece/SQLPieceBPE/__init__.py
+-rw-rw-r--   0 haris     (1000) haris     (1000)     6677 2023-07-21 12:27:00.000000 sqlpiece-0.1.1/src/sqlpiece/SQLPieceBPE/tokenizer.py
+drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-07-22 10:47:07.491140 sqlpiece-0.1.1/src/sqlpiece/SQLPieceBPE/vocab/
+-rw-rw-r--   0 haris     (1000) haris     (1000)   456318 2023-07-20 17:57:36.000000 sqlpiece-0.1.1/src/sqlpiece/SQLPieceBPE/vocab/merges.txt
+-rw-rw-r--   0 haris     (1000) haris     (1000)      408 2023-07-14 12:59:28.000000 sqlpiece-0.1.1/src/sqlpiece/SQLPieceBPE/vocab/sql_vocab.pkl
+-rw-rw-r--   0 haris     (1000) haris     (1000)  1042940 2023-07-20 18:09:30.000000 sqlpiece-0.1.1/src/sqlpiece/SQLPieceBPE/vocab/vocab.json
+drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-07-22 10:47:07.507140 sqlpiece-0.1.1/src/sqlpiece/SQLPieceWPE/
+-rw-rw-r--   0 haris     (1000) haris     (1000)       35 2023-07-14 13:05:59.000000 sqlpiece-0.1.1/src/sqlpiece/SQLPieceWPE/__init__.py
+-rw-rw-r--   0 haris     (1000) haris     (1000) 14083579 2023-07-14 13:06:59.000000 sqlpiece-0.1.1/src/sqlpiece/SQLPieceWPE/lookup_dict.pkl
+-rw-rw-r--   0 haris     (1000) haris     (1000)    63879 2023-07-14 13:06:53.000000 sqlpiece-0.1.1/src/sqlpiece/SQLPieceWPE/no_morph_vocab.txt
+-rw-rw-r--   0 haris     (1000) haris     (1000)     4776 2023-07-15 03:40:24.000000 sqlpiece-0.1.1/src/sqlpiece/SQLPieceWPE/tokenizer.py
+-rw-rw-r--   0 haris     (1000) haris     (1000)   190673 2023-07-14 13:06:53.000000 sqlpiece-0.1.1/src/sqlpiece/SQLPieceWPE/with_morph_vocab.txt
+-rw-rw-r--   0 haris     (1000) haris     (1000)       76 2023-07-20 09:47:21.000000 sqlpiece-0.1.1/src/sqlpiece/__init__.py
+drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-07-22 10:47:07.491140 sqlpiece-0.1.1/src/sqlpiece.egg-info/
+-rw-rw-r--   0 haris     (1000) haris     (1000)      883 2023-07-22 10:47:07.000000 sqlpiece-0.1.1/src/sqlpiece.egg-info/PKG-INFO
+-rw-rw-r--   0 haris     (1000) haris     (1000)      658 2023-07-22 10:47:07.000000 sqlpiece-0.1.1/src/sqlpiece.egg-info/SOURCES.txt
+-rw-rw-r--   0 haris     (1000) haris     (1000)        1 2023-07-22 10:47:07.000000 sqlpiece-0.1.1/src/sqlpiece.egg-info/dependency_links.txt
+-rw-rw-r--   0 haris     (1000) haris     (1000)       26 2023-07-22 10:47:07.000000 sqlpiece-0.1.1/src/sqlpiece.egg-info/requires.txt
+-rw-rw-r--   0 haris     (1000) haris     (1000)        9 2023-07-22 10:47:07.000000 sqlpiece-0.1.1/src/sqlpiece.egg-info/top_level.txt
+drwxrwxr-x   0 haris     (1000) haris     (1000)        0 2023-07-22 10:47:07.507140 sqlpiece-0.1.1/tests/
+-rw-rw-r--   0 haris     (1000) haris     (1000)      163 2023-07-18 15:34:29.000000 sqlpiece-0.1.1/tests/test_sqlpiecebpe.py
```

### Comparing `sqlpiece-0.1.0/PKG-INFO` & `sqlpiece-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlpiece
-Version: 0.1.0
+Version: 0.1.1
 Summary: An SQL tokenization package for use with HuggingFace
 Home-page: https://github.com/MaveriQ/SQLPiece
 Author: Haris Jabbar
 Author-email: harisjabbar@gmail.com
 License: Apache-2.0 license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sqlpiece-0.1.0/setup.py` & `sqlpiece-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='sqlpiece',
-    version='0.1.0',    
+    version='0.1.1',    
     description='An SQL tokenization package for use with HuggingFace',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/MaveriQ/SQLPiece',
     author='Haris Jabbar',
     author_email='harisjabbar@gmail.com',
     license='Apache-2.0 license',
```

### Comparing `sqlpiece-0.1.0/src/sqlpiece/SQLPieceBPE/tokenizer.py` & `sqlpiece-0.1.1/src/sqlpiece/SQLPieceBPE/tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,27 +50,27 @@
     def __init__(
         self,
         vocab_file=None,
         merges_file=None,
         sql_vocab_file=None,
         ver=1.0,
         errors="replace",
-        unk_token="<|endoftext|>",
-        bos_token="<|endoftext|>",
-        eos_token="<|endoftext|>",
-        pad_token=None,
+        unk_token="<UNK>",
+        bos_token="<BOS>",
+        eos_token="<EOS>",
+        pad_token="<PAD>",
         add_prefix_space=False,
         add_bos_token=False,
         **kwargs
     ):
         if sql_vocab_file is None:
             if ver==1.0:
                 sql_vocab_file = path/'vocab/sql_vocab.pkl'
-                vocab_file = path/'vocab/bpe_sql_vocab.json'
-                merges_file = path/'vocab/gpt2_merges.txt'
+                vocab_file = path/'vocab/vocab.json'
+                merges_file = path/'vocab/merges.txt'
         super().__init__(
         vocab_file,
         merges_file,
         errors,
         unk_token,
         bos_token,
         eos_token,
@@ -79,15 +79,27 @@
         add_bos_token,
         **kwargs
         )
         
         self.sql_vocab = pickle.load(open(sql_vocab_file,'rb'))
         self.counter_sql = dict.fromkeys(self.sql_vocab,0)   
         self.counter_bpe = dict()   
-        self.counter_token = dict()   
+        self.counter_token = dict()
+
+        special_tokens_dict = {
+                               "cls_token": "<CLS>",
+                               "sep_token": "<SEP>",
+                               "mask_token": "<MASK>",
+                            #    "pad_token": "<PAD>",
+                            #    "unk_token": "<UNK>",
+                            #    "bos_token": "<BOS>",
+                            #    "eos_token": "<EOS>",
+                               }
+
+        self.add_special_tokens(special_tokens_dict)   
 
     def get_byte_encoding(self,token):
         return "".join(
             self.byte_encoder[b] for b in token.encode("utf-8")
         )  # Maps all our bytes to unicode strings, avoiding control tokens of the BPE (spaces in our case)
         
     def _get_bpe(self,token):
```

### Comparing `sqlpiece-0.1.0/src/sqlpiece/SQLPieceBPE/vocab/bpe_sql_vocab.json` & `sqlpiece-0.1.1/src/sqlpiece/SQLPieceBPE/vocab/vocab.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998608211551844%*

 * *Differences: {"'<BOS>'": '50293',*

 * * "'<CLS>'": '50288',*

 * * "'<EOS>'": '50294',*

 * * "'<MASK>'": '50292',*

 * * "'<PAD>'": '50290',*

 * * "'<SEP>'": '50289',*

 * * "'<UNK>'": '50291'}*

```diff
@@ -1360,14 +1360,21 @@
     ";;;;;;;;": 25887,
     ";;;;;;;;;;;;": 46939,
     ";}": 46956,
     "<": 27,
     "</": 3556,
     "<<": 16791,
     "<?": 47934,
+    "<BOS>": 50293,
+    "<CLS>": 50288,
+    "<EOS>": 50294,
+    "<MASK>": 50292,
+    "<PAD>": 50290,
+    "<SEP>": 50289,
+    "<UNK>": 50291,
     "<|endoftext|>": 50256,
     "=": 28,
     "=\"": 2625,
     "=\"\"": 33151,
     "=\"#": 25698,
     "=\"/": 35922,
     "=#": 46249,
```

### Comparing `sqlpiece-0.1.0/src/sqlpiece/SQLPieceBPE/vocab/gpt2_merges.txt` & `sqlpiece-0.1.1/src/sqlpiece/SQLPieceBPE/vocab/merges.txt`

 * *Files identical despite different names*

### Comparing `sqlpiece-0.1.0/src/sqlpiece/SQLPieceWPE/lookup_dict.pkl` & `sqlpiece-0.1.1/src/sqlpiece/SQLPieceWPE/lookup_dict.pkl`

 * *Files identical despite different names*

### Comparing `sqlpiece-0.1.0/src/sqlpiece/SQLPieceWPE/no_morph_vocab.txt` & `sqlpiece-0.1.1/src/sqlpiece/SQLPieceWPE/no_morph_vocab.txt`

 * *Files identical despite different names*

### Comparing `sqlpiece-0.1.0/src/sqlpiece/SQLPieceWPE/tokenizer.py` & `sqlpiece-0.1.1/src/sqlpiece/SQLPieceWPE/tokenizer.py`

 * *Files identical despite different names*

### Comparing `sqlpiece-0.1.0/src/sqlpiece/SQLPieceWPE/with_morph_vocab.txt` & `sqlpiece-0.1.1/src/sqlpiece/SQLPieceWPE/with_morph_vocab.txt`

 * *Files identical despite different names*

### Comparing `sqlpiece-0.1.0/src/sqlpiece.egg-info/PKG-INFO` & `sqlpiece-0.1.1/src/sqlpiece.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlpiece
-Version: 0.1.0
+Version: 0.1.1
 Summary: An SQL tokenization package for use with HuggingFace
 Home-page: https://github.com/MaveriQ/SQLPiece
 Author: Haris Jabbar
 Author-email: harisjabbar@gmail.com
 License: Apache-2.0 license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sqlpiece-0.1.0/src/sqlpiece.egg-info/SOURCES.txt` & `sqlpiece-0.1.1/src/sqlpiece.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 src/sqlpiece.egg-info/PKG-INFO
 src/sqlpiece.egg-info/SOURCES.txt
 src/sqlpiece.egg-info/dependency_links.txt
 src/sqlpiece.egg-info/requires.txt
 src/sqlpiece.egg-info/top_level.txt
 src/sqlpiece/SQLPieceBPE/__init__.py
 src/sqlpiece/SQLPieceBPE/tokenizer.py
-src/sqlpiece/SQLPieceBPE/vocab/bpe_sql_vocab.json
-src/sqlpiece/SQLPieceBPE/vocab/gpt2_merges.txt
-src/sqlpiece/SQLPieceBPE/vocab/gpt2_vocab.json
+src/sqlpiece/SQLPieceBPE/vocab/merges.txt
 src/sqlpiece/SQLPieceBPE/vocab/sql_vocab.pkl
+src/sqlpiece/SQLPieceBPE/vocab/vocab.json
 src/sqlpiece/SQLPieceWPE/__init__.py
 src/sqlpiece/SQLPieceWPE/lookup_dict.pkl
 src/sqlpiece/SQLPieceWPE/no_morph_vocab.txt
 src/sqlpiece/SQLPieceWPE/tokenizer.py
 src/sqlpiece/SQLPieceWPE/with_morph_vocab.txt
 tests/test_sqlpiecebpe.py
```

