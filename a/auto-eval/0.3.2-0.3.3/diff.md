# Comparing `tmp/auto-eval-0.3.2.tar.gz` & `tmp/auto-eval-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-eval-0.3.2.tar", last modified: Sat Jul 22 06:12:35 2023, max compression
+gzip compressed data, was "auto-eval-0.3.3.tar", last modified: Sat Jul 22 06:59:42 2023, max compression
```

## Comparing `auto-eval-0.3.2.tar` & `auto-eval-0.3.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 06:12:35.187170 auto-eval-0.3.2/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.3.2/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-07-22 06:12:35.186406 auto-eval-0.3.2/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)    16083 2023-06-07 06:25:31.000000 auto-eval-0.3.2/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 06:12:35.183364 auto-eval-0.3.2/auto_eval.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-07-22 06:12:35.000000 auto-eval-0.3.2/auto_eval.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-07-22 06:12:35.000000 auto-eval-0.3.2/auto_eval.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-22 06:12:35.000000 auto-eval-0.3.2/auto_eval.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-07-22 06:12:35.000000 auto-eval-0.3.2/auto_eval.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-07-22 06:12:35.000000 auto-eval-0.3.2/auto_eval.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-07-22 06:12:35.000000 auto-eval-0.3.2/auto_eval.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 06:12:35.183788 auto-eval-0.3.2/eval/
--rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.3.2/eval/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    14819 2023-07-22 06:10:27.000000 auto-eval-0.3.2/eval/auto_llms_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 06:12:35.184050 auto-eval-0.3.2/eval/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.3.2/eval/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     6144 2023-07-21 06:55:27.000000 auto-eval-0.3.2/eval/commands/auto_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 06:12:35.185221 auto-eval-0.3.2/eval/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.3.2/eval/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3094 2023-06-27 06:27:16.000000 auto-eval-0.3.2/eval/prompt_template/prompter.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2646 2023-06-28 02:43:09.000000 auto-eval-0.3.2/eval/prompt_template/prompts.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 06:12:35.186035 auto-eval-0.3.2/eval/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.3.2/eval/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     4197 2023-06-29 07:42:59.000000 auto-eval-0.3.2/eval/utils/data_utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-22 06:12:35.187218 auto-eval-0.3.2/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-07-22 06:12:04.000000 auto-eval-0.3.2/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 06:59:42.219111 auto-eval-0.3.3/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.3.3/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-07-22 06:59:42.218814 auto-eval-0.3.3/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16083 2023-06-07 06:25:31.000000 auto-eval-0.3.3/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 06:59:42.215883 auto-eval-0.3.3/auto_eval.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-07-22 06:59:42.000000 auto-eval-0.3.3/auto_eval.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-07-22 06:59:42.000000 auto-eval-0.3.3/auto_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-22 06:59:42.000000 auto-eval-0.3.3/auto_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-07-22 06:59:42.000000 auto-eval-0.3.3/auto_eval.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-07-22 06:59:42.000000 auto-eval-0.3.3/auto_eval.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-07-22 06:59:42.000000 auto-eval-0.3.3/auto_eval.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 06:59:42.216313 auto-eval-0.3.3/eval/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.3.3/eval/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    14997 2023-07-22 06:59:31.000000 auto-eval-0.3.3/eval/auto_llms_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 06:59:42.216573 auto-eval-0.3.3/eval/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.3.3/eval/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     6145 2023-07-22 06:52:22.000000 auto-eval-0.3.3/eval/commands/auto_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 06:59:42.217760 auto-eval-0.3.3/eval/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.3.3/eval/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3094 2023-06-27 06:27:16.000000 auto-eval-0.3.3/eval/prompt_template/prompter.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2646 2023-06-28 02:43:09.000000 auto-eval-0.3.3/eval/prompt_template/prompts.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-22 06:59:42.218428 auto-eval-0.3.3/eval/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.3.3/eval/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4197 2023-06-29 07:42:59.000000 auto-eval-0.3.3/eval/utils/data_utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-22 06:59:42.219213 auto-eval-0.3.3/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-07-22 06:52:53.000000 auto-eval-0.3.3/setup.py
```

### Comparing `auto-eval-0.3.2/LICENSE` & `auto-eval-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.2/PKG-INFO` & `auto-eval-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.3.2
+Version: 0.3.3
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `auto-eval-0.3.2/README.md` & `auto-eval-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.2/auto_eval.egg-info/PKG-INFO` & `auto-eval-0.3.3/auto_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.3.2
+Version: 0.3.3
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `auto-eval-0.3.2/eval/auto_llms_eval.py` & `auto-eval-0.3.3/eval/auto_llms_eval.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,19 @@
 from typing import Optional, Tuple
 import numpy as np
 import time
 import sys
 from dataclasses import dataclass
 import aiohttp
 import asyncio
-import openai
 from oneapi import OneAPITool
 sys.path.append(os.path.normpath(f'{os.path.dirname(os.path.abspath(__file__))}/..'))
 from eval.utils import df_saver, df_reader, binary_cross_entropy
 from eval.prompt_template import Prompter
 
-
 def eval_one_qa(
              api_tool: OneAPITool,
              eval_prompter: Prompter,
              question: str,
              candidate_answers: List[str],
              target: Union[str, None]='',
              engine: str='',
@@ -297,15 +295,15 @@
         for (result, status) in score_results:
             if status:
                 scored_groups.append(result)
             else:
                 failed_groups.append(result)
         # Retry failed requests
         if len(failed_groups) > 0 and eval_config.retry:
-            score_results = asyncio.run(aeval_groups(eval_config, failed_groups))
+            score_results = asyncio.run(aeval_groups(eval_config, failed_groups, desc='RETRY'))
             for (result, status) in score_results:
                 if status:
                     scored_groups.append(result)
                     failed_groups = [df for df in failed_groups if not df.equals(result)]
 
     scored_results_df = pd.concat(scored_groups)
     log_score_results(eval_results_df=scored_results_df, score_by=eval_config.score_by)
@@ -317,27 +315,30 @@
     results_df = pd.concat([scored_results_df, pd.concat(failed_groups)]) if len(failed_groups) > 0 else scored_results_df
     # Save results
     if eval_config.output_path:
         save_results(results_df=results_df, output_path=eval_config.output_path)
 
 
 
-async def bound_fetch(sem, pbar,*params, **kwargs):
+async def bound_fetch(sem, *params, **kwargs):
     async with sem:
         result = await aeval_one_group(*params, **kwargs)
-        pbar.update(1)
         return result
 
-async def aeval_groups(eval_config: EvalConfig, unscored_groups: List[pd.DataFrame]):
+async def aeval_groups(eval_config: EvalConfig, unscored_groups: List[pd.DataFrame], desc: str='EVAL'):
     # Preparing data
     process_num = len(eval_config.api_config_files)
-    pbar = tqdm(total=len(unscored_groups))
+    pbar = tqdm(total=len(unscored_groups), desc=desc)
     sem = asyncio.Semaphore(process_num)
-    async with aiohttp.ClientSession() as session:
-        openai.aiosession.set(session)
-        tools = [OneAPITool.from_config_file(config_file) for config_file in eval_config.api_config_files]
-        tasks = [asyncio.ensure_future(bound_fetch(sem, pbar, tools[i%process_num], eval_config.eval_prompter,  group,  eval_config.engine, eval_config.temperature, eval_config.max_new_tokens)) for i, group in enumerate(unscored_groups)]
-        results = await asyncio.gather(*tasks)
+    tools = [OneAPITool.from_config_file(config_file) for config_file in eval_config.api_config_files]
+    tasks = [asyncio.ensure_future(bound_fetch(sem, tools[i%process_num], eval_config.eval_prompter,  group,  eval_config.engine, eval_config.temperature, eval_config.max_new_tokens)) for i, group in enumerate(unscored_groups)]
+    task_batches = [tasks[i:i + process_num] for i in range(0, len(tasks), process_num)]
+    results = []
+    for task_batch in task_batches:
+        batch_results = await asyncio.gather(*task_batch)
+        results.extend(batch_results)
+        pbar.update(process_num)
+        await asyncio.sleep(eval_config.request_interval)
     return results
```

### Comparing `auto-eval-0.3.2/eval/commands/auto_eval.py` & `auto-eval-0.3.3/eval/commands/auto_eval.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         required=False,
     )
 
     parser.add_argument(
         "-v",
         "--verbose",
         type=bool,
-        default=True,
+        default=False,
         help="print every prompt and response detail",
         required=False,
     )
     parser.add_argument(
         "-m",
         "--model",
         default='',
```

### Comparing `auto-eval-0.3.2/eval/prompt_template/prompter.py` & `auto-eval-0.3.3/eval/prompt_template/prompter.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.2/eval/prompt_template/prompts.py` & `auto-eval-0.3.3/eval/prompt_template/prompts.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.2/eval/utils/data_utils.py` & `auto-eval-0.3.3/eval/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.3.2/setup.py` & `auto-eval-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-eval",
-    version="0.3.2",
+    version="0.3.3",
     packages=find_packages(),
     # package_data={
     #   "eval":["prompt_template/eval_prompt_template.json"]  
     # },
     install_requires=[
         # Add your library's dependencies here
         "one-api-tool",
```

