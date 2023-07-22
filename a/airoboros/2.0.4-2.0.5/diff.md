# Comparing `tmp/airoboros-2.0.4.tar.gz` & `tmp/airoboros-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airoboros-2.0.4.tar", last modified: Sat Jul 22 16:36:49 2023, max compression
+gzip compressed data, was "airoboros-2.0.5.tar", last modified: Sat Jul 22 17:05:55 2023, max compression
```

## Comparing `airoboros-2.0.4.tar` & `airoboros-2.0.5.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:36:49.458723 airoboros-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 16:36:35.000000 airoboros-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-22 16:36:49.458723 airoboros-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-22 16:36:35.000000 airoboros-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:36:49.450723 airoboros-2.0.4/airoboros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:36:49.454723 airoboros-2.0.4/airoboros/instructors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/coding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/cot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/counterfactual_contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/experiences.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/inline_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/orca.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:36:49.458723 airoboros-2.0.4/airoboros/instructors/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/agent.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/coding.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/contextual.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/contextual_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/cot.txt
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/counterfactual_contextual.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/counterfactual_contextual_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/experience.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/general.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/orca.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/plan.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/riddle.txt
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/roleplay.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/trivia.txt
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/wordgame.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/writing.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/prompts/writing_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/riddles.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/roleplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/simple_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/trivia.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/wordgames.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/instructors/writing.py
--rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-07-22 16:36:35.000000 airoboros-2.0.4/airoboros/self_instruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:36:49.450723 airoboros-2.0.4/airoboros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-22 16:36:49.000000 airoboros-2.0.4/airoboros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-22 16:36:49.000000 airoboros-2.0.4/airoboros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:36:49.000000 airoboros-2.0.4/airoboros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-22 16:36:49.000000 airoboros-2.0.4/airoboros.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-22 16:36:49.000000 airoboros-2.0.4/airoboros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-22 16:36:49.000000 airoboros-2.0.4/airoboros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 16:36:49.458723 airoboros-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-22 16:36:35.000000 airoboros-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:05:55.951523 airoboros-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 17:05:44.000000 airoboros-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-22 17:05:55.951523 airoboros-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-22 17:05:44.000000 airoboros-2.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:05:55.947523 airoboros-2.0.5/airoboros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:05:55.951523 airoboros-2.0.5/airoboros/instructors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/coding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/cot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/counterfactual_contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/experience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/inline_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:05:55.951523 airoboros-2.0.5/airoboros/instructors/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/agent.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/card.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/coding.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/contextual.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/contextual_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/cot.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/counterfactual_contextual.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/counterfactual_contextual_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/experience.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/general.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/orca.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/plan.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/riddle.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/roleplay.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/trivia.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/wordgame.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/writing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/writing_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/riddle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/roleplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/simple_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/trivia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/wordgame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/writing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/self_instruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:05:55.947523 airoboros-2.0.5/airoboros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-22 17:05:55.000000 airoboros-2.0.5/airoboros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-22 17:05:55.000000 airoboros-2.0.5/airoboros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 17:05:55.000000 airoboros-2.0.5/airoboros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-22 17:05:55.000000 airoboros-2.0.5/airoboros.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-22 17:05:55.000000 airoboros-2.0.5/airoboros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-22 17:05:55.000000 airoboros-2.0.5/airoboros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 17:05:55.951523 airoboros-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-22 17:05:44.000000 airoboros-2.0.5/setup.py
```

### Comparing `airoboros-2.0.4/LICENSE` & `airoboros-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/PKG-INFO` & `airoboros-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airoboros
-Version: 2.0.4
+Version: 2.0.5
 Summary: Updated and improved implementation of the self-instruct system.
 Home-page: https://github.com/jondurbin/airoboros
 Author: Jon Durbin
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `airoboros-2.0.4/README.md` & `airoboros-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/entrypoint.py` & `airoboros-2.0.5/airoboros/entrypoint.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/coding.py` & `airoboros-2.0.5/airoboros/instructors/coding.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/contextual.py` & `airoboros-2.0.5/airoboros/instructors/contextual.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/counterfactual_contextual.py` & `airoboros-2.0.5/airoboros/instructors/counterfactual_contextual.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/experiences.py` & `airoboros-2.0.5/airoboros/instructors/experience.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         return
     target_count = config.get("count")
     if target_count is None:
         target_count = instructor.default_count
     target_count = int(target_count)
 
     # Load the prompt template.
-    path = config.get("prompt_path", "experiences.txt")
+    path = config.get("prompt_path", "experience.txt")
     if not os.path.exists(path):
         path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "prompts", path)
     with open(path) as infile:
         prompt = infile.read()
 
     # API params, overriding defaults with this instructor's config.
     api_params = {**instructor.api_params, **config.get("api_params", {})}
@@ -26,15 +26,15 @@
     # Min similarity score.
     min_score = config.get("min_docsearch_score")
     if min_score is None:
         min_score = instructor.min_docsearch_score
     min_score = float(min_score)
 
     # Generate the instruction/response pairs until we reach the target count.
-    count = instructor.instructor_counts.get("experiences", 0)
+    count = instructor.instructor_counts.get("experience", 0)
     language = config.get("language") or instructor.language
     batch_size = config.get("batch_size")
     if batch_size is None:
         batch_size = instructor.default_batch_size
     batch_size = int(batch_size)
     futures = []
     while count < target_count:
@@ -61,13 +61,13 @@
                 or not response
                 or await instructor.is_too_similar(instruction, min_score=min_score)
             ):
                 continue
             yield {
                 "instruction": instruction,
                 "response": response,
-                "category": "experiences",
+                "category": "experience",
             }
             count += 1
             if count >= target_count:
                 break
         futures = []
```

### Comparing `airoboros-2.0.4/airoboros/instructors/general.py` & `airoboros-2.0.5/airoboros/instructors/general.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/inline_qa.py` & `airoboros-2.0.5/airoboros/instructors/inline_qa.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,19 +37,20 @@
     if batch_size is None:
         batch_size = instructor.default_batch_size
     batch_size = int(batch_size)
     count = instructor.instructor_counts.get(category, 0)
     language = config.get("language") or instructor.language
     while count < target_count:
         # Get a batch of instructions.
-        prompt = (
-            template.format(batch_size=batch_size, language=language)
-            if "{batch_size}" in template
-            else template.format(language=language)
-        )
+        prompt_args = {"language": language}
+        if "{batch_size}" in template:
+            prompt_args["batch_size"] = batch_size
+        if "{topic_avoidance}" in template:
+            prompt_args["topic_avoidance"] = instructor.topic_avoidance
+        prompt = template.format(**prompt_args)
         response = await instructor.generate_response(
             prompt, filter_response=filter_response, **api_params
         )
         if not response:
             continue
 
         # Parse instructions and generate responses.
```

### Comparing `airoboros-2.0.4/airoboros/instructors/prompts/agent.txt` & `airoboros-2.0.5/airoboros/instructors/prompts/agent.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/prompts/coding.txt` & `airoboros-2.0.5/airoboros/instructors/prompts/coding.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/prompts/contextual.txt` & `airoboros-2.0.5/airoboros/instructors/prompts/contextual.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/prompts/contextual_response.txt` & `airoboros-2.0.5/airoboros/instructors/prompts/contextual_response.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/prompts/cot.txt` & `airoboros-2.0.5/airoboros/instructors/prompts/cot.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/prompts/counterfactual_contextual.txt` & `airoboros-2.0.5/airoboros/instructors/prompts/counterfactual_contextual.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/prompts/counterfactual_contextual_response.txt` & `airoboros-2.0.5/airoboros/instructors/prompts/counterfactual_contextual_response.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/prompts/experience.txt` & `airoboros-2.0.5/airoboros/instructors/prompts/experience.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/prompts/general.txt` & `airoboros-2.0.5/airoboros/instructors/prompts/general.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/prompts/orca.txt` & `airoboros-2.0.5/airoboros/instructors/prompts/orca.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/prompts/plan.txt` & `airoboros-2.0.5/airoboros/instructors/prompts/plan.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/prompts/riddle.txt` & `airoboros-2.0.5/airoboros/instructors/prompts/riddle.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/prompts/roleplay.txt` & `airoboros-2.0.5/airoboros/instructors/prompts/roleplay.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/prompts/trivia.txt` & `airoboros-2.0.5/airoboros/instructors/prompts/trivia.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/prompts/wordgame.txt` & `airoboros-2.0.5/airoboros/instructors/prompts/wordgame.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/prompts/writing.txt` & `airoboros-2.0.5/airoboros/instructors/prompts/writing.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/prompts/writing_response.txt` & `airoboros-2.0.5/airoboros/instructors/prompts/writing_response.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/simple_task.py` & `airoboros-2.0.5/airoboros/instructors/simple_task.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/instructors/trivia.py` & `airoboros-2.0.5/airoboros/instructors/trivia.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.4/airoboros/self_instruct.py` & `airoboros-2.0.5/airoboros/self_instruct.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,37 +426,41 @@
         async for item in method_map[category](self):
             self.persist(item)
             running_total += 1
             logger.success(
                 f"Generated unique instruction [{category}, total={running_total}]: {item['instruction'][:100]}"
             )
         delta = (datetime.datetime.now() - started_at).total_seconds()
-        logger.success(f"Finished generating {running_total} instructions [{category}] in {delta} seconds.")
+        logger.success(
+            f"Finished generating {running_total} instructions [{category}] in {delta} seconds."
+        )
 
     async def run(self):
         """Run prompt generation and answer to completion."""
         from airoboros.instructors.agent import generate as agent_generator
+        from airoboros.instructors.card import generate as card_generator
         from airoboros.instructors.coding import generate as coding_generator
         from airoboros.instructors.contextual import generate as contextual_generator
         from airoboros.instructors.cot import generate as cot_generator
         from airoboros.instructors.counterfactual_contextual import (
             generate as counterfactual_contextual_generator,
         )
-        from airoboros.instructors.experiences import generate as experience_generator
+        from airoboros.instructors.experience import generate as experience_generator
         from airoboros.instructors.general import generate as general_generator
         from airoboros.instructors.orca import generate as orca_generator
         from airoboros.instructors.plan import generate as plan_generator
-        from airoboros.instructors.riddles import generate as riddle_generator
+        from airoboros.instructors.riddle import generate as riddle_generator
         from airoboros.instructors.roleplay import generate as roleplay_generator
         from airoboros.instructors.trivia import generate as trivia_generator
-        from airoboros.instructors.wordgames import generate as wordgame_generator
+        from airoboros.instructors.wordgame import generate as wordgame_generator
         from airoboros.instructors.writing import generate as writing_generator
 
         method_map = {
             "agent": agent_generator,
+            "card": card_generator,
             "coding": coding_generator,
             "contextual": contextual_generator,
             "cot": cot_generator,
             "counterfactual_contextual": counterfactual_contextual_generator,
             "experience": experience_generator,
             "general": general_generator,
             "plan": plan_generator,
```

### Comparing `airoboros-2.0.4/airoboros.egg-info/PKG-INFO` & `airoboros-2.0.5/airoboros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airoboros
-Version: 2.0.4
+Version: 2.0.5
 Summary: Updated and improved implementation of the self-instruct system.
 Home-page: https://github.com/jondurbin/airoboros
 Author: Jon Durbin
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `airoboros-2.0.4/airoboros.egg-info/SOURCES.txt` & `airoboros-2.0.5/airoboros.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,30 +9,32 @@
 airoboros.egg-info/SOURCES.txt
 airoboros.egg-info/dependency_links.txt
 airoboros.egg-info/entry_points.txt
 airoboros.egg-info/requires.txt
 airoboros.egg-info/top_level.txt
 airoboros/instructors/__init__.py
 airoboros/instructors/agent.py
+airoboros/instructors/card.py
 airoboros/instructors/coding.py
 airoboros/instructors/contextual.py
 airoboros/instructors/cot.py
 airoboros/instructors/counterfactual_contextual.py
-airoboros/instructors/experiences.py
+airoboros/instructors/experience.py
 airoboros/instructors/general.py
 airoboros/instructors/inline_qa.py
 airoboros/instructors/orca.py
 airoboros/instructors/plan.py
-airoboros/instructors/riddles.py
+airoboros/instructors/riddle.py
 airoboros/instructors/roleplay.py
 airoboros/instructors/simple_task.py
 airoboros/instructors/trivia.py
-airoboros/instructors/wordgames.py
+airoboros/instructors/wordgame.py
 airoboros/instructors/writing.py
 airoboros/instructors/prompts/agent.txt
+airoboros/instructors/prompts/card.txt
 airoboros/instructors/prompts/coding.txt
 airoboros/instructors/prompts/contextual.txt
 airoboros/instructors/prompts/contextual_response.txt
 airoboros/instructors/prompts/cot.txt
 airoboros/instructors/prompts/counterfactual_contextual.txt
 airoboros/instructors/prompts/counterfactual_contextual_response.txt
 airoboros/instructors/prompts/experience.txt
```

### Comparing `airoboros-2.0.4/setup.py` & `airoboros-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md")) as infile:
     long_description = infile.read()
 
 setup(
     name="airoboros",
-    version="2.0.4",
+    version="2.0.5",
     description="Updated and improved implementation of the self-instruct system.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jondurbin/airoboros",
     author="Jon Durbin",
     license="Apache 2.0",
     packages=["airoboros", "airoboros.instructors", "airoboros.instructors.prompts"],
```

