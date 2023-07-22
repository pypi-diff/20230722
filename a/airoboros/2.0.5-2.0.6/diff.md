# Comparing `tmp/airoboros-2.0.5.tar.gz` & `tmp/airoboros-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airoboros-2.0.5.tar", last modified: Sat Jul 22 17:05:55 2023, max compression
+gzip compressed data, was "airoboros-2.0.6.tar", last modified: Sat Jul 22 17:27:44 2023, max compression
```

## Comparing `airoboros-2.0.5.tar` & `airoboros-2.0.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:05:55.951523 airoboros-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 17:05:44.000000 airoboros-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-22 17:05:55.951523 airoboros-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-22 17:05:44.000000 airoboros-2.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:05:55.947523 airoboros-2.0.5/airoboros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:05:55.951523 airoboros-2.0.5/airoboros/instructors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/coding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/cot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/counterfactual_contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/experience.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/inline_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/orca.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:05:55.951523 airoboros-2.0.5/airoboros/instructors/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/agent.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/card.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/coding.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/contextual.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/contextual_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/cot.txt
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/counterfactual_contextual.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/counterfactual_contextual_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/experience.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/general.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/orca.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/plan.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/riddle.txt
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/roleplay.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/trivia.txt
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/wordgame.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/writing.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/prompts/writing_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/riddle.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/roleplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/simple_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/trivia.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/wordgame.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/instructors/writing.py
--rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-07-22 17:05:44.000000 airoboros-2.0.5/airoboros/self_instruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:05:55.947523 airoboros-2.0.5/airoboros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-22 17:05:55.000000 airoboros-2.0.5/airoboros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-22 17:05:55.000000 airoboros-2.0.5/airoboros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 17:05:55.000000 airoboros-2.0.5/airoboros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-22 17:05:55.000000 airoboros-2.0.5/airoboros.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-22 17:05:55.000000 airoboros-2.0.5/airoboros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-22 17:05:55.000000 airoboros-2.0.5/airoboros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 17:05:55.951523 airoboros-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-22 17:05:44.000000 airoboros-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:27:44.462581 airoboros-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 17:27:30.000000 airoboros-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-22 17:27:44.462581 airoboros-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-22 17:27:30.000000 airoboros-2.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:27:44.450581 airoboros-2.0.6/airoboros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:27:44.454581 airoboros-2.0.6/airoboros/instructors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/coding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/cot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/counterfactual_contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/experience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/inline_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:27:44.458581 airoboros-2.0.6/airoboros/instructors/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/prompts/agent.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/prompts/card.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/prompts/coding.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/prompts/contextual.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/prompts/contextual_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/prompts/cot.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/prompts/counterfactual_contextual.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/prompts/counterfactual_contextual_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/prompts/experience.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/prompts/general.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/prompts/orca.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/prompts/plan.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/prompts/riddle.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/prompts/roleplay.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/prompts/trivia.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/prompts/wordgame.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/prompts/writing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/prompts/writing_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/riddle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/roleplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/simple_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/trivia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/wordgame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/instructors/writing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-07-22 17:27:30.000000 airoboros-2.0.6/airoboros/self_instruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 17:27:44.450581 airoboros-2.0.6/airoboros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-22 17:27:44.000000 airoboros-2.0.6/airoboros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-22 17:27:44.000000 airoboros-2.0.6/airoboros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 17:27:44.000000 airoboros-2.0.6/airoboros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-22 17:27:44.000000 airoboros-2.0.6/airoboros.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-22 17:27:44.000000 airoboros-2.0.6/airoboros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-22 17:27:44.000000 airoboros-2.0.6/airoboros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 17:27:44.462581 airoboros-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-22 17:27:30.000000 airoboros-2.0.6/setup.py
```

### Comparing `airoboros-2.0.5/LICENSE` & `airoboros-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/PKG-INFO` & `airoboros-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airoboros
-Version: 2.0.5
+Version: 2.0.6
 Summary: Updated and improved implementation of the self-instruct system.
 Home-page: https://github.com/jondurbin/airoboros
 Author: Jon Durbin
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `airoboros-2.0.5/README.md` & `airoboros-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/entrypoint.py` & `airoboros-2.0.6/airoboros/entrypoint.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/coding.py` & `airoboros-2.0.6/airoboros/instructors/coding.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/contextual.py` & `airoboros-2.0.6/airoboros/instructors/contextual.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/counterfactual_contextual.py` & `airoboros-2.0.6/airoboros/instructors/counterfactual_contextual.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/experience.py` & `airoboros-2.0.6/airoboros/instructors/experience.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/general.py` & `airoboros-2.0.6/airoboros/instructors/general.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/inline_qa.py` & `airoboros-2.0.6/airoboros/instructors/inline_qa.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/prompts/agent.txt` & `airoboros-2.0.6/airoboros/instructors/prompts/agent.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/prompts/card.txt` & `airoboros-2.0.6/airoboros/instructors/prompts/card.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/prompts/coding.txt` & `airoboros-2.0.6/airoboros/instructors/prompts/coding.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/prompts/contextual.txt` & `airoboros-2.0.6/airoboros/instructors/prompts/contextual.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/prompts/contextual_response.txt` & `airoboros-2.0.6/airoboros/instructors/prompts/contextual_response.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/prompts/cot.txt` & `airoboros-2.0.6/airoboros/instructors/prompts/cot.txt`

 * *Files 10% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 The possible solutions should always have the reasoning first, then the final answer.  Don't ever put the final answer first, then reasoning.
 
 Be sure the new questions contain instructions to use chain-of-thought reasoning, as the examples do.
 
 Provide a set of {batch_size} new, complex, unique, diverse tasks.
 
-Be sure to randomize the ordering of the optimal solution within the list of possible solutions, i.e., the best solution should sometimes be solution 1, sometimes solution 2, and sometimes solution 3+.
+Rotate the order if the optimal solution in each ANSWER segment, i.e. if the first ANSWER segment has the optimal solution as "Solution 1", the second ANSWER should have the optimal solution as "Solution 2", and so on, so the optimal solution for each ANSWER block is in a different position, starting over at 1 if we exceed the number of possible solutions.  You must provide an even distribution of optimal solution positions across all ANSWER segments.
 
 Be sure to include at least 2, preferably 3 possible solutions for each question.
 
 All output text should be in {language}, but the exact terms "QUESTION" and "ANSWER" are special tokens that must not be translated.
 
 The output format should be:
 QUESTION: [question 1]
```

### Comparing `airoboros-2.0.5/airoboros/instructors/prompts/counterfactual_contextual.txt` & `airoboros-2.0.6/airoboros/instructors/prompts/counterfactual_contextual.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/prompts/counterfactual_contextual_response.txt` & `airoboros-2.0.6/airoboros/instructors/prompts/counterfactual_contextual_response.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/prompts/experience.txt` & `airoboros-2.0.6/airoboros/instructors/prompts/experience.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/prompts/general.txt` & `airoboros-2.0.6/airoboros/instructors/prompts/general.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/prompts/orca.txt` & `airoboros-2.0.6/airoboros/instructors/prompts/orca.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/prompts/plan.txt` & `airoboros-2.0.6/airoboros/instructors/prompts/plan.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/prompts/riddle.txt` & `airoboros-2.0.6/airoboros/instructors/prompts/riddle.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/prompts/roleplay.txt` & `airoboros-2.0.6/airoboros/instructors/prompts/roleplay.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/prompts/trivia.txt` & `airoboros-2.0.6/airoboros/instructors/prompts/trivia.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/prompts/wordgame.txt` & `airoboros-2.0.6/airoboros/instructors/prompts/wordgame.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/prompts/writing.txt` & `airoboros-2.0.6/airoboros/instructors/prompts/writing.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/prompts/writing_response.txt` & `airoboros-2.0.6/airoboros/instructors/prompts/writing_response.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/simple_task.py` & `airoboros-2.0.6/airoboros/instructors/simple_task.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/instructors/trivia.py` & `airoboros-2.0.6/airoboros/instructors/trivia.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros/self_instruct.py` & `airoboros-2.0.6/airoboros/self_instruct.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/airoboros.egg-info/PKG-INFO` & `airoboros-2.0.6/airoboros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airoboros
-Version: 2.0.5
+Version: 2.0.6
 Summary: Updated and improved implementation of the self-instruct system.
 Home-page: https://github.com/jondurbin/airoboros
 Author: Jon Durbin
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `airoboros-2.0.5/airoboros.egg-info/SOURCES.txt` & `airoboros-2.0.6/airoboros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.5/setup.py` & `airoboros-2.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md")) as infile:
     long_description = infile.read()
 
 setup(
     name="airoboros",
-    version="2.0.5",
+    version="2.0.6",
     description="Updated and improved implementation of the self-instruct system.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jondurbin/airoboros",
     author="Jon Durbin",
     license="Apache 2.0",
     packages=["airoboros", "airoboros.instructors", "airoboros.instructors.prompts"],
```

