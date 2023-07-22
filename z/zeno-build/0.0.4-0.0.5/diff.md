# Comparing `tmp/zeno_build-0.0.4.tar.gz` & `tmp/zeno_build-0.0.5.tar.gz`

## Comparing `zeno_build-0.0.4.tar` & `zeno_build-0.0.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/__init__.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/cache_utils.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/version.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/__init__.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/audio_metrics/__init__.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/audio_metrics/error.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/code_metrics/__init__.py
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/code_metrics/execution_accuracy.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/code_metrics/execution_accuracy_utils.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_features/__init__.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_features/capitalization.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_features/clustering.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_features/exact_match.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_features/frequency.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_features/length.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_features/numbers.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_metrics/__init__.py
--rw-r--r--   0        0        0    16437 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_metrics/critique.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_tokenizers/__init__.py
--rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/evaluation/text_tokenizers/unicode.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/experiments/__init__.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/experiments/experiment_run.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/experiments/search_space.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/__init__.py
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/chat_generate.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/dataset_config.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/global_models.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/lm_config.py
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/text_generate.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/providers/__init__.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/providers/cohere_utils.py
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/providers/huggingface_utils.py
--rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/providers/openai_utils.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/models/providers/vllm_utils.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/optimizers/__init__.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/optimizers/base.py
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/optimizers/exhaustive.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/optimizers/random.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/optimizers/standard.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/optimizers/vizier.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/prompts/__init__.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/prompts/chat_prompt.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/prompts/prompt_utils.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/reporting/__init__.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/reporting/aggregate_results.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/reporting/reporting_utils.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 zeno_build-0.0.4/zeno_build/reporting/visualize.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 zeno_build-0.0.4/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zeno_build-0.0.4/LICENSE
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 zeno_build-0.0.4/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zeno_build-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 zeno_build-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/__init__.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/cache_utils.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/version.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/evaluation/__init__.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/evaluation/audio_metrics/__init__.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/evaluation/audio_metrics/error.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/evaluation/code_metrics/__init__.py
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/evaluation/code_metrics/execution_accuracy.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/evaluation/code_metrics/execution_accuracy_utils.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/evaluation/text_features/__init__.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/evaluation/text_features/capitalization.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/evaluation/text_features/clustering.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/evaluation/text_features/exact_match.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/evaluation/text_features/frequency.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/evaluation/text_features/length.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/evaluation/text_features/numbers.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/evaluation/text_metrics/__init__.py
+-rw-r--r--   0        0        0    16437 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/evaluation/text_metrics/critique.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/evaluation/text_tokenizers/__init__.py
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/evaluation/text_tokenizers/unicode.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/experiments/__init__.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/experiments/experiment_run.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/experiments/search_space.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/models/__init__.py
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/models/chat_generate.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/models/dataset_config.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/models/global_models.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/models/lm_config.py
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/models/text_generate.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/models/providers/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/models/providers/cohere_utils.py
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/models/providers/huggingface_utils.py
+-rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/models/providers/openai_utils.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/models/providers/vllm_utils.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/optimizers/__init__.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/optimizers/base.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/optimizers/exhaustive.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/optimizers/random.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/optimizers/standard.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/optimizers/vizier.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/prompts/__init__.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/prompts/chat_prompt.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/prompts/prompt_utils.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/reporting/__init__.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/reporting/aggregate_results.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/reporting/reporting_utils.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 zeno_build-0.0.5/zeno_build/reporting/visualize.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 zeno_build-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zeno_build-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 zeno_build-0.0.5/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zeno_build-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 zeno_build-0.0.5/PKG-INFO
```

### Comparing `zeno_build-0.0.4/zeno_build/cache_utils.py` & `zeno_build-0.0.5/zeno_build/cache_utils.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/evaluation/audio_metrics/error.py` & `zeno_build-0.0.5/zeno_build/evaluation/audio_metrics/error.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/evaluation/code_metrics/execution_accuracy.py` & `zeno_build-0.0.5/zeno_build/evaluation/code_metrics/execution_accuracy.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/evaluation/code_metrics/execution_accuracy_utils.py` & `zeno_build-0.0.5/zeno_build/evaluation/code_metrics/execution_accuracy_utils.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/evaluation/text_features/capitalization.py` & `zeno_build-0.0.5/zeno_build/evaluation/text_features/capitalization.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/evaluation/text_features/clustering.py` & `zeno_build-0.0.5/zeno_build/evaluation/text_features/clustering.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/evaluation/text_features/exact_match.py` & `zeno_build-0.0.5/zeno_build/evaluation/text_features/exact_match.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/evaluation/text_features/frequency.py` & `zeno_build-0.0.5/zeno_build/evaluation/text_features/frequency.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/evaluation/text_features/length.py` & `zeno_build-0.0.5/zeno_build/evaluation/text_features/length.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/evaluation/text_features/numbers.py` & `zeno_build-0.0.5/zeno_build/evaluation/text_features/numbers.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/evaluation/text_metrics/critique.py` & `zeno_build-0.0.5/zeno_build/evaluation/text_metrics/critique.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/evaluation/text_tokenizers/unicode.py` & `zeno_build-0.0.5/zeno_build/evaluation/text_tokenizers/unicode.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/experiments/search_space.py` & `zeno_build-0.0.5/zeno_build/experiments/search_space.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/models/chat_generate.py` & `zeno_build-0.0.5/zeno_build/models/chat_generate.py`

 * *Files 11% similar despite different names*

```diff
@@ -53,34 +53,38 @@
         The generated text.
     """
     print(
         f"Generating with {prompt_template=}, {model_config.model=}, "
         f"{temperature=}, {max_tokens=}, {top_p=}, {context_length=}..."
     )
     if model_config.provider == "openai":
+        response_per_api_call = 1
         return asyncio.run(
             generate_from_openai_completion(
                 _contexts_to_prompts(
                     full_contexts, prompt_template, model_config, context_length
                 ),
                 model_config,
                 temperature,
                 max_tokens,
+                response_per_api_call,
                 top_p,
                 requests_per_minute,
             )
         )
     elif model_config.provider == "openai_chat":
+        response_per_api_call = 1
         return asyncio.run(
             generate_from_openai_chat_completion(
                 full_contexts,
                 prompt_template,
                 model_config,
                 temperature,
                 max_tokens,
+                response_per_api_call,
                 top_p,
                 context_length,
                 requests_per_minute,
             )
         )
     elif model_config.provider == "cohere":
         return asyncio.run(
```

### Comparing `zeno_build-0.0.4/zeno_build/models/dataset_config.py` & `zeno_build-0.0.5/zeno_build/models/dataset_config.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/models/lm_config.py` & `zeno_build-0.0.5/zeno_build/models/lm_config.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/models/text_generate.py` & `zeno_build-0.0.5/zeno_build/models/text_generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,21 +47,23 @@
             prompts,
             model_config,
             temperature,
             max_tokens,
             top_p,
         )
     elif model_config.provider == "openai":
+        response_per_api_call = 1
         prompts = [replace_variables(prompt_template, vars) for vars in variables]
         return asyncio.run(
             generate_from_openai_completion(
                 prompts,
                 model_config,
                 temperature,
                 max_tokens,
+                response_per_api_call,
                 top_p,
                 requests_per_minute,
             )
         )
     elif model_config.provider == "openai_chat":
         full_contexts = [
             ChatMessages(
@@ -78,14 +80,15 @@
             generate_from_openai_chat_completion(
                 full_contexts=full_contexts,
                 prompt_template=ChatMessages([]),
                 model_config=model_config,
                 temperature=temperature,
                 max_tokens=max_tokens,
                 top_p=top_p,
+                n=1,
                 context_length=1,
                 requests_per_minute=requests_per_minute,
             )
         )
     elif model_config.provider == "cohere":
         import cohere
```

### Comparing `zeno_build-0.0.4/zeno_build/models/providers/cohere_utils.py` & `zeno_build-0.0.5/zeno_build/models/providers/cohere_utils.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/models/providers/huggingface_utils.py` & `zeno_build-0.0.5/zeno_build/models/providers/huggingface_utils.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/models/providers/openai_utils.py` & `zeno_build-0.0.5/zeno_build/models/providers/openai_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,87 +3,88 @@
 import asyncio
 import logging
 import os
 from typing import Any
 
 import aiolimiter
 import openai
-import openai.error
 from aiohttp import ClientSession
+from openai import error
 from tqdm.asyncio import tqdm_asyncio
 
 from zeno_build.models import lm_config
 from zeno_build.prompts import chat_prompt
 
+ERROR_ERRORS_TO_MESSAGES = {
+    error.InvalidRequestError: "OpenAI API Invalid Request: Prompt was filtered",
+    error.RateLimitError: "OpenAI API rate limit exceeded. Sleeping for 10 seconds.",
+    error.APIConnectionError: "OpenAI API Connection Error: Error Communicating with OpenAI",  # noqa E501
+    error.Timeout: "OpenAI APITimeout Error: OpenAI Timeout",
+    error.ServiceUnavailableError: "OpenAI service unavailable error: {e}",
+    error.APIError: "OpenAI API error: {e}",
+}
+
 
 async def _throttled_openai_completion_acreate(
     engine: str,
     prompt: str,
     temperature: float,
     max_tokens: int,
+    n: int,
     top_p: float,
     limiter: aiolimiter.AsyncLimiter,
 ) -> dict[str, Any]:
     async with limiter:
         for _ in range(3):
             try:
                 return await openai.Completion.acreate(
                     engine=engine,
                     prompt=prompt,
                     temperature=temperature,
                     max_tokens=max_tokens,
+                    n=n,
                     top_p=top_p,
                 )
-            except openai.error.RateLimitError:
-                logging.warning(
-                    "OpenAI API rate limit exceeded. Sleeping for 10 seconds."
-                )
-                await asyncio.sleep(10)
-            except asyncio.exceptions.TimeoutError:
-                logging.warning("OpenAI API timeout. Sleeping for 10 seconds.")
-                await asyncio.sleep(10)
-            except openai.error.InvalidRequestError:
-                logging.warning("OpenAI API Invalid Request: Prompt was filtered")
-                return {
-                    "choices": [
-                        {"message": {"content": "Invalid Request: Prompt was filtered"}}
-                    ]
-                }
-            except openai.error.APIConnectionError:
-                logging.warning(
-                    "OpenAI API Connection Error: Error Communicating with OpenAI"
-                )
-                await asyncio.sleep(10)
-            except openai.error.Timeout:
-                logging.warning("OpenAI APITimeout Error: OpenAI Timeout")
-                await asyncio.sleep(10)
-            except openai.error.ServiceUnavailableError as e:
-                logging.warning(f"OpenAI service unavailable error: {e}")
-                await asyncio.sleep(10)
-            except openai.error.APIError as e:
-                logging.warning(f"OpenAI API error: {e}")
+            except tuple(ERROR_ERRORS_TO_MESSAGES.keys()) as e:
+                if isinstance(e, (error.ServiceUnavailableError, error.APIError)):
+                    logging.warning(ERROR_ERRORS_TO_MESSAGES[type(e)].format(e=e))
+                elif isinstance(e, error.InvalidRequestError):
+                    logging.warning(ERROR_ERRORS_TO_MESSAGES[type(e)])
+                    return {
+                        "choices": [
+                            {
+                                "message": {
+                                    "content": "Invalid Request: Prompt was filtered"
+                                }
+                            }
+                        ]
+                    }
+                else:
+                    logging.warning(ERROR_ERRORS_TO_MESSAGES[type(e)])
                 await asyncio.sleep(10)
         return {"choices": [{"message": {"content": ""}}]}
 
 
 async def generate_from_openai_completion(
     prompts: list[str],
     model_config: lm_config.LMConfig,
     temperature: float,
     max_tokens: int,
+    n: int,
     top_p: float,
     requests_per_minute: int = 150,
 ) -> list[str]:
     """Generate from OpenAI Completion API.
 
     Args:
         prompts: List of prompts to generate from.
         model_config: Model configuration.
         temperature: Temperature to use.
         max_tokens: Maximum number of tokens to generate.
+        n: Number of completions to generate for each API call.
         top_p: Top p to use.
         requests_per_minute: Number of requests per minute to allow.
 
     Returns:
         List of generated responses.
     """
     if "OPENAI_API_KEY" not in os.environ:
@@ -95,14 +96,15 @@
     limiter = aiolimiter.AsyncLimiter(requests_per_minute)
     async_responses = [
         _throttled_openai_completion_acreate(
             engine=model_config.model,
             prompt=prompt,
             temperature=temperature,
             max_tokens=max_tokens,
+            n=n,
             top_p=top_p,
             limiter=limiter,
         )
         for prompt in prompts
     ]
     responses = await tqdm_asyncio.gather(*async_responses)
     # Note: will never be none because it's set, but mypy doesn't know that.
@@ -111,77 +113,69 @@
 
 
 async def _throttled_openai_chat_completion_acreate(
     model: str,
     messages: list[dict[str, str]],
     temperature: float,
     max_tokens: int,
+    n: int,
     top_p: float,
     limiter: aiolimiter.AsyncLimiter,
 ) -> dict[str, Any]:
     async with limiter:
         for _ in range(3):
             try:
                 return await openai.ChatCompletion.acreate(
                     model=model,
                     messages=messages,
                     temperature=temperature,
                     max_tokens=max_tokens,
+                    n=n,
                     top_p=top_p,
                 )
-            except openai.error.RateLimitError:
-                logging.warning(
-                    "OpenAI API rate limit exceeded. Sleeping for 10 seconds."
-                )
-                await asyncio.sleep(10)
-            except asyncio.exceptions.TimeoutError:
-                logging.warning("OpenAI API timeout. Sleeping for 10 seconds.")
-                await asyncio.sleep(10)
-            except openai.error.InvalidRequestError:
-                logging.warning("OpenAI API Invalid Request: Prompt was filtered")
-                return {
-                    "choices": [
-                        {"message": {"content": "Invalid Request: Prompt was filtered"}}
-                    ]
-                }
-            except openai.error.APIConnectionError:
-                logging.warning(
-                    "OpenAI API Connection Error: Error Communicating with OpenAI"
-                )
-                await asyncio.sleep(10)
-            except openai.error.Timeout:
-                logging.warning("OpenAI APITimeout Error: OpenAI Timeout")
-                await asyncio.sleep(10)
-            except openai.error.ServiceUnavailableError as e:
-                logging.warning(f"OpenAI service unavailable error: {e}")
-                await asyncio.sleep(10)
-            except openai.error.APIError as e:
-                logging.warning(f"OpenAI API error: {e}")
+            except tuple(ERROR_ERRORS_TO_MESSAGES.keys()) as e:
+                if isinstance(e, (error.ServiceUnavailableError, error.APIError)):
+                    logging.warning(ERROR_ERRORS_TO_MESSAGES[type(e)].format(e=e))
+                elif isinstance(e, error.InvalidRequestError):
+                    logging.warning(ERROR_ERRORS_TO_MESSAGES[type(e)])
+                    return {
+                        "choices": [
+                            {
+                                "message": {
+                                    "content": "Invalid Request: Prompt was filtered"
+                                }
+                            }
+                        ]
+                    }
+                else:
+                    logging.warning(ERROR_ERRORS_TO_MESSAGES[type(e)])
                 await asyncio.sleep(10)
         return {"choices": [{"message": {"content": ""}}]}
 
 
 async def generate_from_openai_chat_completion(
     full_contexts: list[chat_prompt.ChatMessages],
     prompt_template: chat_prompt.ChatMessages,
     model_config: lm_config.LMConfig,
     temperature: float,
     max_tokens: int,
+    n: int,
     top_p: float,
     context_length: int,
     requests_per_minute: int = 150,
 ) -> list[str]:
     """Generate from OpenAI Chat Completion API.
 
     Args:
         full_contexts: List of full contexts to generate from.
         prompt_template: Prompt template to use.
         model_config: Model configuration.
         temperature: Temperature to use.
         max_tokens: Maximum number of tokens to generate.
+        n: Number of responses to generate for each API call.
         top_p: Top p to use.
         context_length: Length of context to use.
         requests_per_minute: Number of requests per minute to allow.
 
     Returns:
         List of generated responses.
     """
@@ -196,14 +190,15 @@
         _throttled_openai_chat_completion_acreate(
             model=model_config.model,
             messages=prompt_template.to_openai_chat_completion_messages(
                 full_context=full_context.limit_length(context_length),
             ),
             temperature=temperature,
             max_tokens=max_tokens,
+            n=n,
             top_p=top_p,
             limiter=limiter,
         )
         for full_context in full_contexts
     ]
     responses = await tqdm_asyncio.gather(*async_responses)
     # Note: will never be none because it's set, but mypy doesn't know that.
```

### Comparing `zeno_build-0.0.4/zeno_build/models/providers/vllm_utils.py` & `zeno_build-0.0.5/zeno_build/models/providers/vllm_utils.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/optimizers/base.py` & `zeno_build-0.0.5/zeno_build/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/optimizers/exhaustive.py` & `zeno_build-0.0.5/zeno_build/optimizers/exhaustive.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/optimizers/random.py` & `zeno_build-0.0.5/zeno_build/optimizers/random.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/optimizers/vizier.py` & `zeno_build-0.0.5/zeno_build/optimizers/vizier.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/prompts/chat_prompt.py` & `zeno_build-0.0.5/zeno_build/prompts/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/reporting/aggregate_results.py` & `zeno_build-0.0.5/zeno_build/reporting/aggregate_results.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/reporting/reporting_utils.py` & `zeno_build-0.0.5/zeno_build/reporting/reporting_utils.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/zeno_build/reporting/visualize.py` & `zeno_build-0.0.5/zeno_build/reporting/visualize.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/.gitignore` & `zeno_build-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/LICENSE` & `zeno_build-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/README.md` & `zeno_build-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/pyproject.toml` & `zeno_build-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.4/PKG-INFO` & `zeno_build-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeno_build
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library for comparing multiple llm-based systems.
 Author-email: Ángel Alexander Cabrera <alex.cabrera@gmail.com>, Graham Neubig <neubig@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Zeno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

