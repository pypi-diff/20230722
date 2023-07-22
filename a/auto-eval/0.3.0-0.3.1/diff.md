# Comparing `tmp/auto-eval-0.3.0.tar.gz` & `tmp/auto-eval-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-eval-0.3.0.tar", last modified: Fri Jul 21 10:57:34 2023, max compression
+gzip compressed data, was "auto-eval-0.3.1.tar", last modified: Sat Jul 22 04:48:09 2023, max compression
```

## Comparing `auto-eval-0.3.0.tar` & `auto-eval-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 10:57:34.295325 auto-eval-0.3.0/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.3.0/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-07-21 10:57:34.295078 auto-eval-0.3.0/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)    16083 2023-06-07 06:25:31.000000 auto-eval-0.3.0/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 10:57:34.291531 auto-eval-0.3.0/auto_eval.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-07-21 10:57:34.000000 auto-eval-0.3.0/auto_eval.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-07-21 10:57:34.000000 auto-eval-0.3.0/auto_eval.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-21 10:57:34.000000 auto-eval-0.3.0/auto_eval.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-07-21 10:57:34.000000 auto-eval-0.3.0/auto_eval.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-07-21 10:57:34.000000 auto-eval-0.3.0/auto_eval.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-07-21 10:57:34.000000 auto-eval-0.3.0/auto_eval.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 10:57:34.291978 auto-eval-0.3.0/eval/
--rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.3.0/eval/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    14793 2023-07-21 10:50:50.000000 auto-eval-0.3.0/eval/auto_llms_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 10:57:34.292532 auto-eval-0.3.0/eval/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.3.0/eval/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     6144 2023-07-21 06:55:27.000000 auto-eval-0.3.0/eval/commands/auto_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 10:57:34.293941 auto-eval-0.3.0/eval/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.3.0/eval/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3094 2023-06-27 06:27:16.000000 auto-eval-0.3.0/eval/prompt_template/prompter.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2646 2023-06-28 02:43:09.000000 auto-eval-0.3.0/eval/prompt_template/prompts.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 10:57:34.294697 auto-eval-0.3.0/eval/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.3.0/eval/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     4197 2023-06-29 07:42:59.000000 auto-eval-0.3.0/eval/utils/data_utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-21 10:57:34.295400 auto-eval-0.3.0/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-07-21 10:51:03.000000 auto-eval-0.3.0/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 04:48:09.893572 auto-eval-0.3.1/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.3.1/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-07-22 04:48:09.893414 auto-eval-0.3.1/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16083 2023-06-07 06:25:31.000000 auto-eval-0.3.1/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 04:48:09.890006 auto-eval-0.3.1/auto_eval.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-07-22 04:48:09.000000 auto-eval-0.3.1/auto_eval.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-07-22 04:48:09.000000 auto-eval-0.3.1/auto_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-22 04:48:09.000000 auto-eval-0.3.1/auto_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-07-22 04:48:09.000000 auto-eval-0.3.1/auto_eval.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-07-22 04:48:09.000000 auto-eval-0.3.1/auto_eval.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-07-22 04:48:09.000000 auto-eval-0.3.1/auto_eval.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 04:48:09.890608 auto-eval-0.3.1/eval/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.3.1/eval/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    14809 2023-07-22 02:38:37.000000 auto-eval-0.3.1/eval/auto_llms_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 04:48:09.891065 auto-eval-0.3.1/eval/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.3.1/eval/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     6144 2023-07-21 06:55:27.000000 auto-eval-0.3.1/eval/commands/auto_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 04:48:09.892336 auto-eval-0.3.1/eval/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.3.1/eval/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3094 2023-06-27 06:27:16.000000 auto-eval-0.3.1/eval/prompt_template/prompter.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2646 2023-06-28 02:43:09.000000 auto-eval-0.3.1/eval/prompt_template/prompts.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 04:48:09.893048 auto-eval-0.3.1/eval/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.3.1/eval/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4197 2023-06-29 07:42:59.000000 auto-eval-0.3.1/eval/utils/data_utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-22 04:48:09.893612 auto-eval-0.3.1/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-07-22 02:45:15.000000 auto-eval-0.3.1/setup.py
```

### Comparing `auto-eval-0.3.0/LICENSE` & `auto-eval-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.0/PKG-INFO` & `auto-eval-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.3.0
+Version: 0.3.1
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `auto-eval-0.3.0/README.md` & `auto-eval-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.0/auto_eval.egg-info/PKG-INFO` & `auto-eval-0.3.1/auto_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.3.0
+Version: 0.3.1
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `auto-eval-0.3.0/eval/auto_llms_eval.py` & `auto-eval-0.3.1/eval/auto_llms_eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,17 +98,17 @@
                       engine=engine,
                       temperature=temperature,
                       max_new_tokens=max_new_tokens)
     if scores is not None and len(scores) == len(candidate_answers):
         group.at[0, 'raw_response'] = raw_response
         for i in range(len(scores)):
             group.at[i, 'score'] = scores[i]
-        return group
+        return group, True
     else:
-        return None
+        return data_group, False
 
         
 async def aeval_one_group(
     api_tool: OneAPITool,
     eval_prompter: Prompter,
     data_group: pd.DataFrame,
     engine: str,
@@ -130,17 +130,17 @@
                       engine=engine,
                       temperature=temperature,
                       max_new_tokens=max_new_tokens)
     if scores is not None and len(scores) == len(candidate_answers):
         group.at[0, 'raw_response'] = raw_response
         for i in range(len(scores)):
             group.at[i, 'score'] = scores[i]
-        return group
+        return group, True
     else:
-        return None
+        return data_group, False
 
 
 
 def prepare_eval_data(
     eval_data_path: List[str],
     eval_categories: Optional[List[str]] = None, 
     question_column_names: Optional[List[str]] = None,
@@ -272,42 +272,42 @@
 
     process_num = len(eval_config.api_config_files)
     # Init api tool and prompter
     if process_num == 1:
         failed_groups = []
         tool = OneAPITool.from_config_file(eval_config.api_config_files[0])
         for group in tqdm(unscored_groups):
-            result = eval_one_group(tool, eval_config.eval_prompter,  group,  eval_config.engine, eval_config.temperature, eval_config.max_new_tokens)
-            if result is not None:
+            result, status = eval_one_group(tool, eval_config.eval_prompter,  group,  eval_config.engine, eval_config.temperature, eval_config.max_new_tokens)
+            if status:
                 scored_groups.append(result)
             else:
                 failed_groups.append(group)
             time.sleep(eval_config.request_interval)
 
         # Retry failed requests
         if len(failed_groups) > 0 and eval_config.retry:
             for group in tqdm(failed_groups.copy(), desc='RETRY'):
-                result = eval_one_group(tool, eval_config.eval_prompter,  group,  eval_config.engine, eval_config.temperature, eval_config.max_new_tokens)
-                if result is not None:
+                result, status = eval_one_group(tool, eval_config.eval_prompter,  group,  eval_config.engine, eval_config.temperature, eval_config.max_new_tokens)
+                if status:
                     scored_groups.append(result)
                     failed_groups = [df for df in failed_groups if not df.equals(group)]
                 time.sleep(eval_config.request_interval)
     else:
         score_results = asyncio.run(aeval_groups(eval_config, unscored_groups))
         failed_groups = []
-        for result in score_results:
-            if result is not None:
+        for (result, status) in score_results:
+            if status:
                 scored_groups.append(result)
             else:
                 failed_groups.append(result)
         # Retry failed requests
         if len(failed_groups) > 0 and eval_config.retry:
             score_results = asyncio.run(aeval_groups(eval_config, failed_groups))
             for result in score_results:
-                if result is not None:
+                if status:
                     scored_groups.append(result)
                     failed_groups = [df for df in failed_groups if not df.equals(result)]
 
     scored_results_df = pd.concat(scored_groups)
     log_score_results(eval_results_df=scored_results_df, score_by=eval_config.score_by)
     log_eval_prompt_scores_loss(eval_results_df=scored_results_df)
     # Log score results
```

### Comparing `auto-eval-0.3.0/eval/commands/auto_eval.py` & `auto-eval-0.3.1/eval/commands/auto_eval.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.0/eval/prompt_template/prompter.py` & `auto-eval-0.3.1/eval/prompt_template/prompter.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.0/eval/prompt_template/prompts.py` & `auto-eval-0.3.1/eval/prompt_template/prompts.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.0/eval/utils/data_utils.py` & `auto-eval-0.3.1/eval/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.0/setup.py` & `auto-eval-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-eval",
-    version="0.3.0",
+    version="0.3.1",
     packages=find_packages(),
     # package_data={
     #   "eval":["prompt_template/eval_prompt_template.json"]  
     # },
     install_requires=[
         # Add your library's dependencies here
         "one-api-tool",
```

