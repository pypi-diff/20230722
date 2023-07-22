# Comparing `tmp/paper-qa-3.3.3.tar.gz` & `tmp/paper-qa-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-3.3.3.tar", last modified: Tue Jul 18 21:01:33 2023, max compression
+gzip compressed data, was "paper-qa-3.4.0.tar", last modified: Sat Jul 22 16:10:24 2023, max compression
```

## Comparing `paper-qa-3.3.3.tar` & `paper-qa-3.4.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:01:33.657306 paper-qa-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 21:00:55.000000 paper-qa-3.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-18 21:01:33.653306 paper-qa-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-07-18 21:00:55.000000 paper-qa-3.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:01:33.649306 paper-qa-3.3.3/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-18 21:01:33.000000 paper-qa-3.3.3/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-18 21:01:33.000000 paper-qa-3.3.3/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 21:01:33.000000 paper-qa-3.3.3/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-18 21:01:33.000000 paper-qa-3.3.3/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 21:01:33.000000 paper-qa-3.3.3/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:01:33.653306 paper-qa-3.3.3/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/chains.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:01:33.653306 paper-qa-3.3.3/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    23494 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 21:01:33.657306 paper-qa-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-18 21:00:55.000000 paper-qa-3.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:01:33.653306 paper-qa-3.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    27622 2023-07-18 21:00:55.000000 paper-qa-3.3.3/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:10:24.078141 paper-qa-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 16:09:47.000000 paper-qa-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-22 16:10:24.078141 paper-qa-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-07-22 16:09:47.000000 paper-qa-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:10:24.070141 paper-qa-3.4.0/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-22 16:10:24.000000 paper-qa-3.4.0/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-22 16:10:24.000000 paper-qa-3.4.0/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:10:24.000000 paper-qa-3.4.0/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-22 16:10:24.000000 paper-qa-3.4.0/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-22 16:10:24.000000 paper-qa-3.4.0/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:10:24.074141 paper-qa-3.4.0/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/chains.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:10:24.074141 paper-qa-3.4.0/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23951 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 16:09:47.000000 paper-qa-3.4.0/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 16:10:24.078141 paper-qa-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-22 16:09:47.000000 paper-qa-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:10:24.078141 paper-qa-3.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    27845 2023-07-22 16:09:47.000000 paper-qa-3.4.0/tests/test_paperqa.py
```

### Comparing `paper-qa-3.3.3/LICENSE` & `paper-qa-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.3/PKG-INFO` & `paper-qa-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.3.3
+Version: 3.4.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.3.3/README.md` & `paper-qa-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.3/paper_qa.egg-info/PKG-INFO` & `paper-qa-3.4.0/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.3.3
+Version: 3.4.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.3.3/paperqa/chains.py` & `paper-qa-3.4.0/paperqa/chains.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.3/paperqa/contrib/zotero.py` & `paper-qa-3.4.0/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.3/paperqa/docs.py` & `paper-qa-3.4.0/paperqa/docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,14 +363,15 @@
     def get_evidence(
         self,
         answer: Answer,
         k: int = 3,
         max_sources: int = 5,
         marginal_relevance: bool = True,
         get_callbacks: CallbackFactory = lambda x: None,
+        detailed_citations: bool = False,
     ) -> Answer:
         # special case for jupyter notebooks
         if "get_ipython" in globals() or "google.colab" in sys.modules:
             import nest_asyncio
 
             nest_asyncio.apply()
         try:
@@ -381,24 +382,26 @@
         return loop.run_until_complete(
             self.aget_evidence(
                 answer,
                 k=k,
                 max_sources=max_sources,
                 marginal_relevance=marginal_relevance,
                 get_callbacks=get_callbacks,
+                detailed_citations=detailed_citations,
             )
         )
 
     async def aget_evidence(
         self,
         answer: Answer,
         k: int = 3,
         max_sources: int = 5,
         marginal_relevance: bool = True,
         get_callbacks: CallbackFactory = lambda x: None,
+        detailed_citations: bool = False,
     ) -> Answer:
         if len(self.docs) == 0 and self.doc_index is None:
             return answer
         self._build_texts_index(keys=answer.dockey_filter)
         if self.texts_index is None:
             return answer
         self.texts_index = cast(VectorStore, self.texts_index)
@@ -444,17 +447,21 @@
             # This is dangerous because it
             # could mask errors that are important- like auth errors
             # I also cannot know what the exception
             # type is because any model could be used
             # my best idea is see if there is a 4XX
             # http code in the exception
             try:
+                citation = match.metadata["doc"]["citation"]
+                if detailed_citations:
+                    match.metadata["name"] + ": " + citation
                 context = await summary_chain.arun(
                     question=answer.question,
-                    citation=match.metadata["doc"]["citation"],
+                    # Add name so chunk is stated
+                    citation=citation,
                     summary_length=answer.summary_length,
                     text=match.page_content,
                     callbacks=callbacks,
                 )
             except Exception as e:
                 if guess_is_4xx(str(e)):
                     return None
@@ -480,15 +487,19 @@
         if len(contexts) == 0:
             return answer
         contexts = sorted(contexts, key=lambda x: x.score, reverse=True)
         contexts = contexts[:max_sources]
         # add to answer contexts
         answer.contexts += contexts
         context_str = "\n\n".join(
-            [f"{c.text.name}: {c.context}" for c in answer.contexts]
+            [
+                f"{c.text.name}: {c.context}"
+                + (f". Based on {c.text.doc.citation}" if detailed_citations else "")
+                for c in answer.contexts
+            ]
         )
         valid_names = [c.text.name for c in answer.contexts]
         context_str += "\n\nValid keys: " + ", ".join(valid_names)
         answer.context = context_str
         return answer
 
     def query(
```

### Comparing `paper-qa-3.3.3/paperqa/prompts.py` & `paper-qa-3.4.0/paperqa/prompts.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.3/paperqa/readers.py` & `paper-qa-3.4.0/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.3/paperqa/types.py` & `paper-qa-3.4.0/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.3/paperqa/utils.py` & `paper-qa-3.4.0/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.3/setup.py` & `paper-qa-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.3/tests/test_paperqa.py` & `paper-qa-3.4.0/tests/test_paperqa.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,20 @@
     docs = Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     evidence = docs.get_evidence(
         Answer(question="For which state was Bates a governor?"), k=1, max_sources=1
     )
     print(evidence.context)
     assert "Missouri" in evidence.context
+
+    evidence = docs.get_evidence(
+        Answer(question="For which state was Bates a governor?"),
+        detailed_citations=True,
+    )
+    assert "Based on WikiMedia Foundation, 2023, Accessed now" in evidence.context
     os.remove(doc_path)
 
 
 def test_query():
     docs = Docs()
     docs.add_url(
         "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
```

