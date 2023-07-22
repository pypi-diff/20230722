# Comparing `tmp/airoboros-2.0.2.tar.gz` & `tmp/airoboros-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airoboros-2.0.2.tar", last modified: Tue Jul 18 18:40:34 2023, max compression
+gzip compressed data, was "airoboros-2.0.3.tar", last modified: Sat Jul 22 10:24:55 2023, max compression
```

## Comparing `airoboros-2.0.2.tar` & `airoboros-2.0.3.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:40:34.688363 airoboros-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 18:40:23.000000 airoboros-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-18 18:40:34.688363 airoboros-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-18 18:40:23.000000 airoboros-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:40:34.684363 airoboros-2.0.2/airoboros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:40:34.688363 airoboros-2.0.2/airoboros/instructors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/coding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/cot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/counterfactual_contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/experiences.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/inline_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/orca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:40:34.688363 airoboros-2.0.2/airoboros/instructors/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/prompts/agent.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/prompts/coding.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/prompts/contextual.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/prompts/contextual_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/prompts/cot.txt
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/prompts/counterfactual_contextual.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/prompts/counterfactual_contextual_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/prompts/experience.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/prompts/general.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/prompts/orca.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/prompts/riddle.txt
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/prompts/roleplay.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/prompts/trivia.txt
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/prompts/wordgame.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/riddles.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/roleplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/simple_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/trivia.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/instructors/wordgames.py
--rw-r--r--   0 runner    (1001) docker     (123)    19952 2023-07-18 18:40:23.000000 airoboros-2.0.2/airoboros/self_instruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:40:34.684363 airoboros-2.0.2/airoboros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-18 18:40:34.000000 airoboros-2.0.2/airoboros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-18 18:40:34.000000 airoboros-2.0.2/airoboros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:40:34.000000 airoboros-2.0.2/airoboros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-18 18:40:34.000000 airoboros-2.0.2/airoboros.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-18 18:40:34.000000 airoboros-2.0.2/airoboros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 18:40:34.000000 airoboros-2.0.2/airoboros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:40:34.688363 airoboros-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-18 18:40:23.000000 airoboros-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:24:55.188892 airoboros-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 10:24:38.000000 airoboros-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-22 10:24:55.188892 airoboros-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-22 10:24:38.000000 airoboros-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:24:55.184892 airoboros-2.0.3/airoboros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:24:55.188892 airoboros-2.0.3/airoboros/instructors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/coding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/cot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/counterfactual_contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/experiences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/inline_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:24:55.188892 airoboros-2.0.3/airoboros/instructors/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/agent.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/coding.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/contextual.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/contextual_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/cot.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/counterfactual_contextual.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/counterfactual_contextual_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/experience.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/general.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/orca.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/plan.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/riddle.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/roleplay.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/trivia.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/prompts/wordgame.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/riddles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/roleplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/simple_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/trivia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/instructors/wordgames.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20062 2023-07-22 10:24:38.000000 airoboros-2.0.3/airoboros/self_instruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 10:24:55.184892 airoboros-2.0.3/airoboros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-22 10:24:55.000000 airoboros-2.0.3/airoboros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-22 10:24:55.000000 airoboros-2.0.3/airoboros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 10:24:55.000000 airoboros-2.0.3/airoboros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-22 10:24:55.000000 airoboros-2.0.3/airoboros.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-22 10:24:55.000000 airoboros-2.0.3/airoboros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-22 10:24:55.000000 airoboros-2.0.3/airoboros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 10:24:55.188892 airoboros-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-22 10:24:38.000000 airoboros-2.0.3/setup.py
```

### Comparing `airoboros-2.0.2/LICENSE` & `airoboros-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/PKG-INFO` & `airoboros-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airoboros
-Version: 2.0.2
+Version: 2.0.3
 Summary: Updated and improved implementation of the self-instruct system.
 Home-page: https://github.com/jondurbin/airoboros
 Author: Jon Durbin
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `airoboros-2.0.2/README.md` & `airoboros-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/entrypoint.py` & `airoboros-2.0.3/airoboros/entrypoint.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/coding.py` & `airoboros-2.0.3/airoboros/instructors/coding.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/contextual.py` & `airoboros-2.0.3/airoboros/instructors/contextual.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/counterfactual_contextual.py` & `airoboros-2.0.3/airoboros/instructors/counterfactual_contextual.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/experiences.py` & `airoboros-2.0.3/airoboros/instructors/experiences.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/general.py` & `airoboros-2.0.3/airoboros/instructors/general.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/inline_qa.py` & `airoboros-2.0.3/airoboros/instructors/inline_qa.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,19 @@
 
     # Generate the instruction/response pairs until we reach the target count.
     batch_size = config.get("batch_size", 10)
     count = instructor.instructor_counts.get(category, 0)
     language = config.get("language") or instructor.language
     while count < target_count:
         # Get a batch of instructions.
-        prompt = template.format(batch_size=batch_size, language=language)
+        prompt = (
+            template.format(batch_size=batch_size, language=language)
+            if "{batch_size}" in template
+            else template.format(language=language)
+        )
         response = await instructor.generate_response(prompt, **api_params)
         if not response:
             continue
 
         # Parse instructions and generate responses.
         for instruction, response in re.findall(
             f"{start_key}:(.*?){end_key}:(.*?)(?={start_key}|$)", response, re.DOTALL
```

### Comparing `airoboros-2.0.2/airoboros/instructors/prompts/agent.txt` & `airoboros-2.0.3/airoboros/instructors/prompts/agent.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Below are example prompt/response pairs that showing examples of an "agent"/"router" prompt for an artificial intelligence assistant.
+Below is an example prompt/response pair that showing examples of an "agent"/"router" prompt for an artificial intelligence assistant.
 
 PROMPT:
-Please select an appropriate function and parameters to use from the list of available functions below, based on the provided user input.
+Please select an appropriate function and parameters to use from the list of available functions below, based on the provided user input.  Provide your response in YAML format.
 
 Input: From the provided CSV, generate an aggregate table containing a count per email address.
 
 Available functions:
 search:
   description: Help the user find information by converting the input query into a series of search terms and filters that may help pinpoint the location of the information.
   parameters:
@@ -34,15 +34,15 @@
 
 Be sure the prompt includes the description that it's supposed to be an agent with direction to select the best function.
 
 Be sure to include an input that could make use of one of the functions.
 
 Be sure to format the list of available functions as proper YAML, with appropriate spacing for nested objects.
 
-Be sure to format the answers as proper YAML, with appropriate spacing for nested objects.
+The new prompts should ask for output to be in either YAML or JSON format; be sure to format each answer according to the format requested by it's corresponding prompt.
 
 Be sure to randomize the ordering of the available functions so the selected function is not always the first function.  The selected function should sometimes be the first function, other times be the second function, and so on for all N in number of functions.
 
 All output text should be in {language}, but the exact terms "PROMPT" and "ANSWER" are special tokens that must not be translated.
 
 Response format:
 PROMPT: [question 1]
```

### Comparing `airoboros-2.0.2/airoboros/instructors/prompts/coding.txt` & `airoboros-2.0.3/airoboros/instructors/prompts/coding.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/prompts/contextual.txt` & `airoboros-2.0.3/airoboros/instructors/prompts/contextual.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/prompts/contextual_response.txt` & `airoboros-2.0.3/airoboros/instructors/prompts/contextual_response.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/prompts/cot.txt` & `airoboros-2.0.3/airoboros/instructors/prompts/cot.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/prompts/counterfactual_contextual.txt` & `airoboros-2.0.3/airoboros/instructors/prompts/counterfactual_contextual.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/prompts/counterfactual_contextual_response.txt` & `airoboros-2.0.3/airoboros/instructors/prompts/counterfactual_contextual_response.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/prompts/experience.txt` & `airoboros-2.0.3/airoboros/instructors/prompts/experience.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/prompts/general.txt` & `airoboros-2.0.3/airoboros/instructors/prompts/general.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/prompts/orca.txt` & `airoboros-2.0.3/airoboros/instructors/prompts/orca.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/prompts/riddle.txt` & `airoboros-2.0.3/airoboros/instructors/prompts/riddle.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/prompts/roleplay.txt` & `airoboros-2.0.3/airoboros/instructors/prompts/roleplay.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/prompts/trivia.txt` & `airoboros-2.0.3/airoboros/instructors/prompts/trivia.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/prompts/wordgame.txt` & `airoboros-2.0.3/airoboros/instructors/prompts/wordgame.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/simple_task.py` & `airoboros-2.0.3/airoboros/instructors/simple_task.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/instructors/trivia.py` & `airoboros-2.0.3/airoboros/instructors/trivia.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.2/airoboros/self_instruct.py` & `airoboros-2.0.3/airoboros/self_instruct.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,27 +405,29 @@
         from airoboros.instructors.cot import generate as cot_generator
         from airoboros.instructors.counterfactual_contextual import (
             generate as counterfactual_contextual_generator,
         )
         from airoboros.instructors.experiences import generate as experience_generator
         from airoboros.instructors.general import generate as general_generator
         from airoboros.instructors.orca import generate as orca_generator
+        from airoboros.instructors.plan import generate as plan_generator
         from airoboros.instructors.riddles import generate as riddle_generator
         from airoboros.instructors.roleplay import generate as roleplay_generator
         from airoboros.instructors.trivia import generate as trivia_generator
         from airoboros.instructors.wordgames import generate as wordgame_generator
 
         method_map = {
             "agent": agent_generator,
             "coding": coding_generator,
             "contextual": contextual_generator,
             "cot": cot_generator,
             "counterfactual_contextual": counterfactual_contextual_generator,
             "experience": experience_generator,
             "general": general_generator,
+            "plan": plan_generator,
             "orca": orca_generator,
             "riddle": riddle_generator,
             "roleplay": roleplay_generator,
             "trivia": trivia_generator,
             "wordgame": wordgame_generator,
         }
```

### Comparing `airoboros-2.0.2/airoboros.egg-info/PKG-INFO` & `airoboros-2.0.3/airoboros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airoboros
-Version: 2.0.2
+Version: 2.0.3
 Summary: Updated and improved implementation of the self-instruct system.
 Home-page: https://github.com/jondurbin/airoboros
 Author: Jon Durbin
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `airoboros-2.0.2/airoboros.egg-info/SOURCES.txt` & `airoboros-2.0.3/airoboros.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 airoboros/instructors/contextual.py
 airoboros/instructors/cot.py
 airoboros/instructors/counterfactual_contextual.py
 airoboros/instructors/experiences.py
 airoboros/instructors/general.py
 airoboros/instructors/inline_qa.py
 airoboros/instructors/orca.py
+airoboros/instructors/plan.py
 airoboros/instructors/riddles.py
 airoboros/instructors/roleplay.py
 airoboros/instructors/simple_task.py
 airoboros/instructors/trivia.py
 airoboros/instructors/wordgames.py
 airoboros/instructors/prompts/agent.txt
 airoboros/instructors/prompts/coding.txt
@@ -32,11 +33,12 @@
 airoboros/instructors/prompts/contextual_response.txt
 airoboros/instructors/prompts/cot.txt
 airoboros/instructors/prompts/counterfactual_contextual.txt
 airoboros/instructors/prompts/counterfactual_contextual_response.txt
 airoboros/instructors/prompts/experience.txt
 airoboros/instructors/prompts/general.txt
 airoboros/instructors/prompts/orca.txt
+airoboros/instructors/prompts/plan.txt
 airoboros/instructors/prompts/riddle.txt
 airoboros/instructors/prompts/roleplay.txt
 airoboros/instructors/prompts/trivia.txt
 airoboros/instructors/prompts/wordgame.txt
```

### Comparing `airoboros-2.0.2/setup.py` & `airoboros-2.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md")) as infile:
     long_description = infile.read()
 
 setup(
     name="airoboros",
-    version="2.0.2",
+    version="2.0.3",
     description="Updated and improved implementation of the self-instruct system.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jondurbin/airoboros",
     author="Jon Durbin",
     license="Apache 2.0",
     packages=["airoboros", "airoboros.instructors", "airoboros.instructors.prompts"],
```

