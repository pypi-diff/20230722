# Comparing `tmp/airoboros-2.0.3.tar.gz` & `tmp/airoboros-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airoboros-2.0.3.tar", last modified: Sat Jul 22 10:24:55 2023, max compression
+gzip compressed data, was "airoboros-2.0.4.tar", last modified: Sat Jul 22 16:36:49 2023, max compression
```

## Comparing `airoboros-2.0.3.tar` & `airoboros-2.0.4.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:24:55.188892 airoboros-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 10:24:38.000000 airoboros-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-22 10:24:55.188892 airoboros-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-22 10:24:38.000000 airoboros-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:24:55.184892 airoboros-2.0.3/airoboros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:24:55.188892 airoboros-2.0.3/airoboros/instructors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/coding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/cot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/counterfactual_contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/experiences.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/inline_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/orca.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:24:55.188892 airoboros-2.0.3/airoboros/instructors/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/agent.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/coding.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/contextual.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/contextual_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/cot.txt
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/counterfactual_contextual.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/counterfactual_contextual_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/experience.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/general.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/orca.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/plan.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/riddle.txt
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/roleplay.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/trivia.txt
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/wordgame.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/riddles.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/roleplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/simple_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/trivia.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/wordgames.py
--rw-r--r--   0 runner    (1001) docker     (123)    20062 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/self_instruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:24:55.184892 airoboros-2.0.3/airoboros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-22 10:24:55.000000 airoboros-2.0.3/airoboros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-22 10:24:55.000000 airoboros-2.0.3/airoboros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 10:24:55.000000 airoboros-2.0.3/airoboros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-22 10:24:55.000000 airoboros-2.0.3/airoboros.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-22 10:24:55.000000 airoboros-2.0.3/airoboros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-22 10:24:55.000000 airoboros-2.0.3/airoboros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 10:24:55.188892 airoboros-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-22 10:24:38.000000 airoboros-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:36:49.458723 airoboros-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 16:36:35.000000 airoboros-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-22 16:36:49.458723 airoboros-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-22 16:36:35.000000 airoboros-2.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:36:49.450723 airoboros-2.0.4/airoboros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:36:49.454723 airoboros-2.0.4/airoboros/instructors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/coding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/cot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/counterfactual_contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/experiences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/inline_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:36:49.458723 airoboros-2.0.4/airoboros/instructors/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/agent.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/coding.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/contextual.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/contextual_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/cot.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/counterfactual_contextual.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/counterfactual_contextual_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/experience.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/general.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/orca.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/plan.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/riddle.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/roleplay.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/trivia.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/wordgame.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/writing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/writing_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/riddles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/roleplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/simple_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/trivia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/wordgames.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/writing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/self_instruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:36:49.450723 airoboros-2.0.4/airoboros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-22 16:36:49.000000 airoboros-2.0.4/airoboros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-22 16:36:49.000000 airoboros-2.0.4/airoboros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:36:49.000000 airoboros-2.0.4/airoboros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-22 16:36:49.000000 airoboros-2.0.4/airoboros.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-22 16:36:49.000000 airoboros-2.0.4/airoboros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-22 16:36:49.000000 airoboros-2.0.4/airoboros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 16:36:49.458723 airoboros-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-22 16:36:35.000000 airoboros-2.0.4/setup.py
```

### Comparing `airoboros-2.0.3/LICENSE` & `airoboros-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.3/PKG-INFO` & `airoboros-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airoboros
-Version: 2.0.3
+Version: 2.0.4
 Summary: Updated and improved implementation of the self-instruct system.
 Home-page: https://github.com/jondurbin/airoboros
 Author: Jon Durbin
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `airoboros-2.0.3/README.md` & `airoboros-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.3/airoboros/entrypoint.py` & `airoboros-2.0.4/airoboros/entrypoint.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.3/airoboros/instructors/coding.py` & `airoboros-2.0.4/airoboros/instructors/coding.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 
 
 async def generate(instructor):
     """Generator for coding training data."""
     config = instructor.instructors.get("coding")
     if not config:
         return
-    target_count = config.get("count") or instructor.default_count
+    target_count = config.get("count")
+    if target_count is None:
+        target_count = instructor.default_count
+    target_count = int(target_count)
+    if not target_count:
+        return
 
     # Load the prompt template.
     path = config.get("prompt_path", "coding.txt")
     if not os.path.exists(path):
         path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "prompts", path)
     with open(path) as infile:
         template = infile.read()
@@ -24,18 +29,24 @@
     if not coding_languages:
         raise ValueError("At least one coding language must be configured.")
 
     # API params, overriding defaults with this instructor's config.
     api_params = {**instructor.api_params, **config.get("api_params", {})}
 
     # Min similarity score.
-    min_score = config.get("min_docsearch_score") or instructor.min_docsearch_score
+    min_score = instructor.min_docsearch_score
+    if config.get("min_docsearch_score") is not None:
+        min_score = config["min_docsearch_score"]
+    min_score = float(min_score)
 
     # Generate the instruction/response pairs until we reach the target count.
-    batch_size = config.get("batch_size", 10)
+    batch_size = config.get("batch_size")
+    if batch_size is None:
+        batch_size = instructor.default_batch_size
+    batch_size = int(batch_size)
     count = instructor.instructor_counts.get("coding", 0)
     language_index = 0
     language = config.get("language") or instructor.language
     while count < target_count:
         # Inject languages to use for this batch.
         current_languages = []
         for _ in range(batch_size):
```

### Comparing `airoboros-2.0.3/airoboros/instructors/contextual.py` & `airoboros-2.0.4/airoboros/instructors/contextual.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,15 +139,20 @@
 
 
 async def generate(instructor):
     """Generator for contextual training data."""
     config = instructor.instructors.get("contextual")
     if not config:
         return
-    target_count = config.get("count") or instructor.default_count
+    target_count = config.get("count")
+    if target_count is None:
+        target_count = instructor.default_count
+    target_count = int(target_count)
+    if not target_count:
+        return
 
     # Load the prompt template.
     path = config.get("prompt_path", "contextual.txt")
     if not os.path.exists(path):
         path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "prompts", path)
     with open(path) as infile:
         template = infile.read()
@@ -165,19 +170,25 @@
         "index": 0,
     }
 
     # API params, overriding defaults with this instructor's config.
     api_params = {**instructor.api_params, **config.get("api_params", {})}
 
     # Min similarity score.
-    min_score = config.get("min_docsearch_score") or instructor.min_docsearch_score
+    min_score = config.get("min_docsearch_score")
+    if min_score is None:
+        min_score = instructor.min_docsearch_score
+    min_score = float(min_score)
 
     # Generate the instruction/response pairs until we reach the target count.
     count = instructor.instructor_counts.get("contextual", 0)
-    batch_size = config.get("batch_size") or instructor.default_batch_size
+    batch_size = config.get("batch_size")
+    if batch_size is None:
+        batch_size = instructor.default_batch_size
+    batch_size = int(batch_size)
     futures = []
     while count < target_count:
         prompt = generate_prompt(instructor, config, template, topic_iter)
         futures.append(instructor.generate_response(prompt, **api_params))
         if len(futures) < batch_size:
             continue
         instructions = []
```

### Comparing `airoboros-2.0.3/airoboros/instructors/counterfactual_contextual.py` & `airoboros-2.0.4/airoboros/instructors/counterfactual_contextual.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,20 @@
 
 
 async def generate(instructor):
     """Generator for contextual training data."""
     config = instructor.instructors.get("counterfactual_contextual")
     if not config:
         return
-    target_count = config.get("count") or instructor.default_count
+    target_count = config.get("count")
+    if target_count is None:
+        target_count = instructor.default_count
+    target_count = int(target_count)
+    if not target_count:
+        return
 
     # Load the prompt template.
     path = config.get("prompt_path", "counterfactual_contextual.txt")
     if not os.path.exists(path):
         path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "prompts", path)
     with open(path) as infile:
         template = infile.read()
@@ -40,19 +45,25 @@
     with open(path) as infile:
         response_template = infile.read()
 
     # API params, overriding defaults with this instructor's config.
     api_params = {**instructor.api_params, **config.get("api_params", {})}
 
     # Min similarity score.
-    min_score = config.get("min_docsearch_score") or instructor.min_docsearch_score
+    min_score = config.get("min_docsearch_score")
+    if min_score is None:
+        min_score = instructor.min_docsearch_score
+    min_score = float(min_score)
 
     # Generate the instruction/response pairs until we reach the target count.
     count = instructor.instructor_counts.get("counterfactual_contextual", 0)
-    batch_size = config.get("batch_size") or instructor.default_batch_size
+    batch_size = config.get("batch_size")
+    if batch_size is None:
+        batch_size = instructor.default_batch_size
+    batch_size = int(batch_size)
     language = config.get("language") or instructor.language
     while count < target_count:
         response = await instructor.generate_response(
             template.format(batch_size=batch_size, language=language), **api_params
         )
         if not response or not response.strip():
             continue
```

### Comparing `airoboros-2.0.3/airoboros/instructors/experiences.py` & `airoboros-2.0.4/airoboros/instructors/experiences.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 import asyncio
 import os
 import re
 
 
 async def generate(instructor):
     """Generator for experiences."""
-    config = instructor.instructors.get("experiences")
+    config = instructor.instructors.get("experience")
     if not config:
         return
-    target_count = config.get("count") or instructor.default_count
+    target_count = config.get("count")
+    if target_count is None:
+        target_count = instructor.default_count
+    target_count = int(target_count)
 
     # Load the prompt template.
     path = config.get("prompt_path", "experiences.txt")
     if not os.path.exists(path):
         path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "prompts", path)
     with open(path) as infile:
         prompt = infile.read()
 
     # API params, overriding defaults with this instructor's config.
     api_params = {**instructor.api_params, **config.get("api_params", {})}
 
     # Min similarity score.
-    min_score = config.get("min_docsearch_score") or instructor.min_docsearch_score
+    min_score = config.get("min_docsearch_score")
+    if min_score is None:
+        min_score = instructor.min_docsearch_score
+    min_score = float(min_score)
 
     # Generate the instruction/response pairs until we reach the target count.
     count = instructor.instructor_counts.get("experiences", 0)
     language = config.get("language") or instructor.language
-    batch_size = config.get("batch_size") or instructor.default_batch_size
+    batch_size = config.get("batch_size")
+    if batch_size is None:
+        batch_size = instructor.default_batch_size
+    batch_size = int(batch_size)
     futures = []
     while count < target_count:
         futures.append(
             instructor.generate_response(prompt.format(language=language), **api_params)
         )
         if len(futures) < batch_size:
             continue
```

### Comparing `airoboros-2.0.3/airoboros/instructors/general.py` & `airoboros-2.0.4/airoboros/instructors/inline_qa.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,70 @@
-import asyncio
-import json
 import os
 import re
 
 
-async def generate(instructor):
-    """Generator for generic/general training data."""
-    config = instructor.instructors.get("general")
+async def generate(
+    instructor, category, start_key="QUESTION", end_key="ANSWER", filter_response=True
+):
+    """Generator for generic inline question answer pair training data."""
+    config = instructor.instructors.get(category)
     if not config:
         return
-    target_count = config.get("count") or instructor.default_count
+    target_count = config.get("count")
+    if target_count is None:
+        target_count = instructor.default_count
+    target_count = int(target_count)
+    if not target_count:
+        return
 
     # Load the prompt template.
-    path = config.get("prompt_path", "general.txt")
+    path = config.get("prompt_path", f"{category}.txt")
     if not os.path.exists(path):
         path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "prompts", path)
     with open(path) as infile:
         template = infile.read()
 
-    # Load the topics.
-    topics = instructor.get_instructor_topics(config)
-    topic_index = 0
-
     # API params, overriding defaults with this instructor's config.
     api_params = {**instructor.api_params, **config.get("api_params", {})}
 
     # Min similarity score.
-    min_score = config.get("min_docsearch_score") or instructor.min_docsearch_score
+    min_score = config.get("min_docsearch_score")
+    if min_score is None:
+        min_score = instructor.min_docsearch_score
+    min_score = float(min_score)
 
     # Generate the instruction/response pairs until we reach the target count.
-    batch_size = config.get("batch_size") or config.default_batch_size
-    count = instructor.instructor_counts.get("general", 0)
+    batch_size = config.get("batch_size")
+    if batch_size is None:
+        batch_size = instructor.default_batch_size
+    batch_size = int(batch_size)
+    count = instructor.instructor_counts.get(category, 0)
     language = config.get("language") or instructor.language
     while count < target_count:
-        # Inject the topics to use for this batch.
-        current_topics = []
-        for _ in range(batch_size):
-            current_topics.append(topics[topic_index])
-            topic_index += 1
-            if topic_index >= len(topics):
-                topic_index = 0
-        topics_str = "\n".join(
-            [
-                f" * instruction {idx + 1} must be related to topic: {json.dumps(topic)}"
-                for idx, topic in enumerate(current_topics)
-            ]
-        )
-
         # Get a batch of instructions.
-        prompt = template.format(
-            batch_size=batch_size,
-            topics=topics_str,
-            topic_avoidance=instructor.topic_avoidance,
-            language=language,
+        prompt = (
+            template.format(batch_size=batch_size, language=language)
+            if "{batch_size}" in template
+            else template.format(language=language)
+        )
+        response = await instructor.generate_response(
+            prompt, filter_response=filter_response, **api_params
         )
-        response = await instructor.generate_response(prompt, **api_params)
         if not response:
             continue
 
         # Parse instructions and generate responses.
-        futures = []
-        instructions = []
-        for instruction in re.findall(
-            r"(?:^|\n)TSK \d+\. (.*?)(?:$|(?=\nTSK \d+\. ))", response, re.DOTALL
+        for instruction, response in re.findall(
+            f"{start_key}:(.*?){end_key}:(.*?)(?={start_key}|$)", response, re.DOTALL
         ):
             if not instruction.strip() or await instructor.is_too_similar(
                 instruction, min_score=min_score
             ):
                 continue
-            instructions.append(instruction)
-            futures.append(instructor.generate_response(instruction, **api_params))
-        if not futures:
-            continue
-        responses = await asyncio.gather(*futures)
-        for idx in range(len(futures)):
-            response = responses[idx]
-            if not response or not response.strip():
-                continue
             yield {
-                "instruction": instructions[idx].strip(),
+                "instruction": instruction.strip(),
                 "response": response.strip(),
-                "category": "general",
+                "category": category,
             }
             count += 1
             if count >= target_count:
                 break
```

### Comparing `airoboros-2.0.3/airoboros/instructors/inline_qa.py` & `airoboros-2.0.4/airoboros/instructors/general.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,98 @@
+import asyncio
+import json
 import os
 import re
 
 
-async def generate(instructor, category, start_key="QUESTION", end_key="ANSWER"):
-    """Generator for generic inline question answer pair training data."""
-    config = instructor.instructors.get(category)
+async def generate(instructor):
+    """Generator for generic/general training data."""
+    config = instructor.instructors.get("general")
     if not config:
         return
-    target_count = config.get("count") or instructor.default_count
+    target_count = config.get("count")
+    if target_count is None:
+        target_count = instructor.default_count
+    target_count = int(target_count)
+    if not target_count:
+        return
 
     # Load the prompt template.
-    path = config.get("prompt_path", f"{category}.txt")
+    path = config.get("prompt_path", "general.txt")
     if not os.path.exists(path):
         path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "prompts", path)
     with open(path) as infile:
         template = infile.read()
 
+    # Load the topics.
+    topics = instructor.get_instructor_topics(config)
+    topic_index = 0
+
     # API params, overriding defaults with this instructor's config.
     api_params = {**instructor.api_params, **config.get("api_params", {})}
 
     # Min similarity score.
-    min_score = config.get("min_docsearch_score") or instructor.min_docsearch_score
+    min_score = config.get("min_docsearch_score")
+    if min_score is None:
+        min_score = instructor.min_docsearch_score
+    min_score = float(min_score)
 
     # Generate the instruction/response pairs until we reach the target count.
-    batch_size = config.get("batch_size", 10)
-    count = instructor.instructor_counts.get(category, 0)
+    batch_size = config.get("batch_size")
+    if batch_size is None:
+        batch_size = config.default_batch_size
+    batch_size = int(batch_size)
+    count = instructor.instructor_counts.get("general", 0)
     language = config.get("language") or instructor.language
     while count < target_count:
+        # Inject the topics to use for this batch.
+        current_topics = []
+        for _ in range(batch_size):
+            current_topics.append(topics[topic_index])
+            topic_index += 1
+            if topic_index >= len(topics):
+                topic_index = 0
+        topics_str = "\n".join(
+            [
+                f" * instruction {idx + 1} must be related to topic: {json.dumps(topic)}"
+                for idx, topic in enumerate(current_topics)
+            ]
+        )
+
         # Get a batch of instructions.
-        prompt = (
-            template.format(batch_size=batch_size, language=language)
-            if "{batch_size}" in template
-            else template.format(language=language)
+        prompt = template.format(
+            batch_size=batch_size,
+            topics=topics_str,
+            topic_avoidance=instructor.topic_avoidance,
+            language=language,
         )
         response = await instructor.generate_response(prompt, **api_params)
         if not response:
             continue
 
         # Parse instructions and generate responses.
-        for instruction, response in re.findall(
-            f"{start_key}:(.*?){end_key}:(.*?)(?={start_key}|$)", response, re.DOTALL
+        futures = []
+        instructions = []
+        for instruction in re.findall(
+            r"(?:^|\n)TSK \d+\. (.*?)(?:$|(?=\nTSK \d+\. ))", response, re.DOTALL
         ):
             if not instruction.strip() or await instructor.is_too_similar(
                 instruction, min_score=min_score
             ):
                 continue
+            instructions.append(instruction)
+            futures.append(instructor.generate_response(instruction, **api_params))
+        if not futures:
+            continue
+        responses = await asyncio.gather(*futures)
+        for idx in range(len(futures)):
+            response = responses[idx]
+            if not response or not response.strip():
+                continue
             yield {
-                "instruction": instruction.strip(),
+                "instruction": instructions[idx].strip(),
                 "response": response.strip(),
-                "category": category,
+                "category": "general",
             }
             count += 1
             if count >= target_count:
                 break
```

### Comparing `airoboros-2.0.3/airoboros/instructors/prompts/agent.txt` & `airoboros-2.0.4/airoboros/instructors/prompts/agent.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.3/airoboros/instructors/prompts/coding.txt` & `airoboros-2.0.4/airoboros/instructors/prompts/coding.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.3/airoboros/instructors/prompts/contextual.txt` & `airoboros-2.0.4/airoboros/instructors/prompts/contextual.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.3/airoboros/instructors/prompts/contextual_response.txt` & `airoboros-2.0.4/airoboros/instructors/prompts/contextual_response.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.3/airoboros/instructors/prompts/cot.txt` & `airoboros-2.0.4/airoboros/instructors/prompts/cot.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.3/airoboros/instructors/prompts/counterfactual_contextual.txt` & `airoboros-2.0.4/airoboros/instructors/prompts/counterfactual_contextual.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.3/airoboros/instructors/prompts/counterfactual_contextual_response.txt` & `airoboros-2.0.4/airoboros/instructors/prompts/counterfactual_contextual_response.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.3/airoboros/instructors/prompts/experience.txt` & `airoboros-2.0.4/airoboros/instructors/prompts/experience.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.3/airoboros/instructors/prompts/general.txt` & `airoboros-2.0.4/airoboros/instructors/prompts/general.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.3/airoboros/instructors/prompts/orca.txt` & `airoboros-2.0.4/airoboros/instructors/prompts/orca.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.3/airoboros/instructors/prompts/plan.txt` & `airoboros-2.0.4/airoboros/instructors/prompts/plan.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.3/airoboros/instructors/prompts/riddle.txt` & `airoboros-2.0.4/airoboros/instructors/prompts/riddle.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.3/airoboros/instructors/prompts/roleplay.txt` & `airoboros-2.0.4/airoboros/instructors/prompts/roleplay.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.3/airoboros/instructors/prompts/trivia.txt` & `airoboros-2.0.4/airoboros/instructors/prompts/trivia.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.3/airoboros/instructors/prompts/wordgame.txt` & `airoboros-2.0.4/airoboros/instructors/prompts/wordgame.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.3/airoboros/instructors/simple_task.py` & `airoboros-2.0.4/airoboros/instructors/simple_task.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,31 +4,51 @@
 
 
 async def generate(instructor, category):
     """Generator for simple instruction response tasks (e.g. roleplay, wordgames)."""
     config = instructor.instructors.get(category)
     if not config:
         return
-    target_count = config.get("count") or instructor.default_count
+    target_count = config.get("count")
+    if target_count is None:
+        target_count = instructor.default_count
+    target_count = int(target_count)
+    if not target_count:
+        return
 
     # Load the prompt template.
     path = config.get("prompt_path", f"{category}.txt")
     if not os.path.exists(path):
         path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "prompts", path)
     with open(path) as infile:
         template = infile.read()
 
+    # Response prompt template (optional).
+    response_prompt = None
+    path = config.get("response_prompt_path", f"{category}_response.txt")
+    if not os.path.exists(path):
+        path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "prompts", path)
+        if os.path.exists(path):
+            with open(path) as infile:
+                response_prompt = infile.read()
+
     # API params, overriding defaults with this instructor's config.
     api_params = {**instructor.api_params, **config.get("api_params", {})}
 
     # Min similarity score.
-    min_score = config.get("min_docsearch_score") or instructor.min_docsearch_score
+    min_score = config.get("min_docsearch_score")
+    if min_score is None:
+        min_score = instructor.min_docsearch_score
+    min_score = float(min_score)
 
     # Generate the instruction/response pairs until we reach the target count.
-    batch_size = config.get("batch_size") or instructor.default_batch_size
+    batch_size = config.get("batch_size")
+    if batch_size is None:
+        batch_size = instructor.default_batch_size
+    batch_size = int(batch_size)
     count = instructor.instructor_counts.get(category, 0)
     language = config.get("language") or instructor.language
     while count < target_count:
         # Get a batch of instructions.
         prompt = (
             template.format(batch_size=batch_size, language=language)
             if "{topic_avoidance}" not in template
@@ -49,15 +69,18 @@
             r"(?:^|\n)TSK \d+\. (.*?)(?:$|(?=\nTSK \d+\. ))", response, re.DOTALL
         ):
             if not instruction.strip() or await instructor.is_too_similar(
                 instruction, min_score=min_score
             ):
                 continue
             instructions.append(instruction)
-            futures.append(instructor.generate_response(instruction, **api_params))
+            full_prompt = instruction
+            if response_prompt:
+                full_prompt = response_prompt.format(instruction=instruction)
+            futures.append(instructor.generate_response(full_prompt, **api_params))
         if not futures:
             continue
         responses = await asyncio.gather(*futures)
         for idx in range(len(responses)):
             response = responses[idx]
             if not response or not response.strip():
                 continue
```

### Comparing `airoboros-2.0.3/airoboros/instructors/trivia.py` & `airoboros-2.0.4/airoboros/instructors/trivia.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.3/airoboros/self_instruct.py` & `airoboros-2.0.4/airoboros/self_instruct.py`

 * *Files 9% similar despite different names*

```diff
@@ -106,16 +106,20 @@
             "frequency_penalty": float(api_params.get("frequency_penalty") or 0.0),
             "presence_penalty": float(api_params.get("presence_penalty") or 2.0),
         }
         self.topic_prompt = raw_config["topic_prompt"].format(
             topic_avoidance=self.topic_avoidance
         )
         self.topic_request_count = int(raw_config.get("topic_request_count") or 20)
-        self.default_count = int(raw_config.get("default_count") or 100)
-        self.default_batch_size = int(raw_config.get("default_batch_size") or 5)
+        self.default_count = 100
+        if raw_config.get("default_count") is not None:
+            self.default_count = int(raw_config["default_count"])
+        self.default_batch_size = 5
+        if raw_config.get("default_batch_size") is not None:
+            self.default_batch_size = raw_config["default_batch_size"]
         self.language = raw_config.get("language") or "English"
 
         # Validate the model for each generator.
         self.instructors = raw_config.get("instructors")
         self.validate_model(self.model)
         valid_models = {self.model: True}
         for key, config in self.instructors.items():
@@ -139,15 +143,15 @@
                         task = json.loads(line)
                         self.instructor_counts[task.get("category", "general")] += 1
                         docs.append(task["instruction"])
                 logger.info(
                     f"Found {len(docs)} existing machine-generated instruction(s)."
                 )
                 for category, count in self.instructor_counts.items():
-                    logger.info(f"  - category {category}: {count}")
+                    logger.info(f" * category {category}: {count}")
             else:
                 raise RuntimeError(
                     f"{self.output_path} already exists, but overwrite and append are false!"
                 )
         logger.info(
             "Initializing in-memory document store for similarity comparison..."
         )
@@ -253,23 +257,24 @@
             if not topics:
                 raise ValueError(
                     f"Found empty topics file: {instructor_config['topics_path']}"
                 )
         return topics
 
     @backoff.on_exception(
-        backoff.expo,
+        backoff.fibo,
         (
             requests.exceptions.ConnectionError,
             requests.exceptions.Timeout,
             ServerError,
             RateLimitError,
             TooManyRequestsError,
             ServerOverloadedError,
         ),
+        max_value=19,
     )
     async def _post(self, path: str, payload: Dict[str, Any]) -> Dict[str, Any]:
         """Perform a post request to OpenAI API.
 
         :param path: URL path to send request to.
         :type path: str
 
@@ -329,20 +334,18 @@
 
     async def generate_response(self, instruction: str, **kwargs) -> str:
         """Call OpenAI with the specified instruction and return the text response.
 
         :param instruction: The instruction to respond to.
         :type instruction: str
 
-        :param recurse: Allow recursive calls, e.g. to rephrase to remove AI refs.
-        :type recurse: bool
-
         :return: Response text.
         :rtype: str
         """
+        filter_response = kwargs.pop("filter_response", True)
         model = kwargs.get("model", self.model)
         completions = True if model in MODEL_ENDPOINTS["completions"] else False
         path = "/v1/completions" if completions else "/v1/chat/completions"
         payload = {**kwargs}
         if "model" not in payload:
             payload["model"] = model
         if completions:
@@ -359,20 +362,22 @@
             return None
         text = None
         if self._completions:
             text = response["choices"][0]["text"]
         else:
             text = response["choices"][0]["message"]["content"]
 
-        if any([banned.search(text, re.I) for banned in self.response_filters]):
-            logger.warning(f"Banned response: {text}")
-            return None
-        if text.startswith(("I'm sorry,", "Apologies,", "I can't", "I won't")):
-            logger.warning(f"Banned response: {text}")
-            return None
+        if filter_response:
+            for banned in self.response_filters:
+                if banned.search(text, re.I):
+                    logger.warning(f"Banned response [{banned}]: {text}")
+                    return None
+            if text.startswith(("I'm sorry,", "Apologies,", "I can't", "I won't")):
+                logger.warning(f"Banned response [apology]: {text}")
+                return None
         return text
 
     async def is_too_similar(self, instruction: str, min_score: float = None):
         """Check the similarity of a new instruction to the existing set.
 
         :param instruction: The instruction string to compare.
         :type instruction: str
@@ -393,14 +398,44 @@
             if min_ <= min_score:
                 logger.warning(
                     f"Skipping instruction, too similar [{min_}]: {instruction}"
                 )
                 return True
             return False
 
+    def persist(self, item):
+        """Persist a single item to the output file and docstore."""
+        self.outfile.write(json.dumps(item) + "\n")
+        self.outfile.flush()
+        self.docstores[-1].add_texts([item["instruction"]])
+        self.docstore_size += 1
+        if self.docstore_size >= MAX_DOCSTORE_SIZE:
+            logger.info("Initializing new docstore...")
+            self.docstores.append(
+                Chroma.from_texts(["__initialize__"], self.embeddings)
+            )
+            self.docstore_size = 0
+
+    async def run_instructor(self, category, method_map):
+        """Run a single instructor, as an async task."""
+        if category not in method_map:
+            logger.warning(f"Unknown category: {category}, skipping...")
+            return
+        logger.info(f"Generating instructions for {category}...")
+        started_at = datetime.datetime.now()
+        running_total = self.instructor_counts.get(category, 0)
+        async for item in method_map[category](self):
+            self.persist(item)
+            running_total += 1
+            logger.success(
+                f"Generated unique instruction [{category}, total={running_total}]: {item['instruction'][:100]}"
+            )
+        delta = (datetime.datetime.now() - started_at).total_seconds()
+        logger.success(f"Finished generating {running_total} instructions [{category}] in {delta} seconds.")
+
     async def run(self):
         """Run prompt generation and answer to completion."""
         from airoboros.instructors.agent import generate as agent_generator
         from airoboros.instructors.coding import generate as coding_generator
         from airoboros.instructors.contextual import generate as contextual_generator
         from airoboros.instructors.cot import generate as cot_generator
         from airoboros.instructors.counterfactual_contextual import (
@@ -410,14 +445,15 @@
         from airoboros.instructors.general import generate as general_generator
         from airoboros.instructors.orca import generate as orca_generator
         from airoboros.instructors.plan import generate as plan_generator
         from airoboros.instructors.riddles import generate as riddle_generator
         from airoboros.instructors.roleplay import generate as roleplay_generator
         from airoboros.instructors.trivia import generate as trivia_generator
         from airoboros.instructors.wordgames import generate as wordgame_generator
+        from airoboros.instructors.writing import generate as writing_generator
 
         method_map = {
             "agent": agent_generator,
             "coding": coding_generator,
             "contextual": contextual_generator,
             "cot": cot_generator,
             "counterfactual_contextual": counterfactual_contextual_generator,
@@ -425,48 +461,36 @@
             "general": general_generator,
             "plan": plan_generator,
             "orca": orca_generator,
             "riddle": riddle_generator,
             "roleplay": roleplay_generator,
             "trivia": trivia_generator,
             "wordgame": wordgame_generator,
+            "writing": writing_generator,
         }
 
         await self.initialize_topics()
         self.initialize_docstores()
 
         # Generate instructions for each category.
-        total = sum(self.instructor_counts.values())
-        with open(self.output_path, "a+") as outfile:
-            for category in self.instructors:
-                if category not in method_map:
-                    logger.warning(f"Unknown category: {category}, skipping...")
-                    continue
-                count = self.instructors[category].get("count") or self.default_count
-                logger.info(f"Generating {count} instructions for {category}...")
-                started_at = datetime.datetime.now()
-                async for item in method_map[category](self):
-                    delta = round(
-                        (datetime.datetime.now() - started_at).total_seconds(), 3
-                    )
-                    outfile.write(json.dumps(item) + "\n")
-                    outfile.flush()
-                    self.docstores[-1].add_texts([item["instruction"]])
-                    self.docstore_size += 1
-                    if self.docstore_size >= MAX_DOCSTORE_SIZE:
-                        logger.info("Initializing new docstore...")
-                        self.docstores.append(
-                            Chroma.from_texts(["__initialize__"], self.embeddings)
-                        )
-                        self.docstore_size = 0
-                    total += 1
-                    logger.success(
-                        f"Generated unique instruction in {delta}s [total={total}]: {item['instruction'][:100]}"
-                    )
-                    started_at = datetime.datetime.now()
+        self.outfile = open(self.output_path, "a+")
+        started_at = datetime.datetime.now()
+        try:
+            tasks = [
+                asyncio.create_task(self.run_instructor(category, method_map))
+                for category in self.instructors
+            ]
+            for task in tasks:
+                await task
+        finally:
+            self.outfile.close()
+        delta = (datetime.datetime.now() - started_at).total_seconds()
+        logger.success(
+            f"Finished generating all instructions in {delta} seconds, enjoy!"
+        )
 
 
 def generate_instructions(args):
     random.seed(secrets.randbelow(1000000000))
     parser = argparse.ArgumentParser()
     for arg, kwargs in SelfInstructor.CLI_ARGS.items():
         parser.add_argument(arg, **kwargs)
```

### Comparing `airoboros-2.0.3/airoboros.egg-info/PKG-INFO` & `airoboros-2.0.4/airoboros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airoboros
-Version: 2.0.3
+Version: 2.0.4
 Summary: Updated and improved implementation of the self-instruct system.
 Home-page: https://github.com/jondurbin/airoboros
 Author: Jon Durbin
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `airoboros-2.0.3/airoboros.egg-info/SOURCES.txt` & `airoboros-2.0.4/airoboros.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -23,22 +23,25 @@
 airoboros/instructors/orca.py
 airoboros/instructors/plan.py
 airoboros/instructors/riddles.py
 airoboros/instructors/roleplay.py
 airoboros/instructors/simple_task.py
 airoboros/instructors/trivia.py
 airoboros/instructors/wordgames.py
+airoboros/instructors/writing.py
 airoboros/instructors/prompts/agent.txt
 airoboros/instructors/prompts/coding.txt
 airoboros/instructors/prompts/contextual.txt
 airoboros/instructors/prompts/contextual_response.txt
 airoboros/instructors/prompts/cot.txt
 airoboros/instructors/prompts/counterfactual_contextual.txt
 airoboros/instructors/prompts/counterfactual_contextual_response.txt
 airoboros/instructors/prompts/experience.txt
 airoboros/instructors/prompts/general.txt
 airoboros/instructors/prompts/orca.txt
 airoboros/instructors/prompts/plan.txt
 airoboros/instructors/prompts/riddle.txt
 airoboros/instructors/prompts/roleplay.txt
 airoboros/instructors/prompts/trivia.txt
-airoboros/instructors/prompts/wordgame.txt
+airoboros/instructors/prompts/wordgame.txt
+airoboros/instructors/prompts/writing.txt
+airoboros/instructors/prompts/writing_response.txt
```

### Comparing `airoboros-2.0.3/setup.py` & `airoboros-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md")) as infile:
     long_description = infile.read()
 
 setup(
     name="airoboros",
-    version="2.0.3",
+    version="2.0.4",
     description="Updated and improved implementation of the self-instruct system.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jondurbin/airoboros",
     author="Jon Durbin",
     license="Apache 2.0",
     packages=["airoboros", "airoboros.instructors", "airoboros.instructors.prompts"],
```

