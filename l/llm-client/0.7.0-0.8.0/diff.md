# Comparing `tmp/llm_client-0.7.0.tar.gz` & `tmp/llm_client-0.8.0.tar.gz`

## Comparing `llm_client-0.7.0.tar` & `llm_client-0.8.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 llm_client-0.7.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 llm_client-0.7.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/base_llm_client.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/consts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_api_client/__init__.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_api_client/ai21_client.py
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_api_client/aleph_alpha_client.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_api_client/anthropic_client.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_api_client/base_llm_api_client.py
--rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_api_client/google_client.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_api_client/huggingface_client.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_api_client/llm_api_client_factory.py
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_api_client/openai_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_client/__init__.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_client/local_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/sync/__init__.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/sync/sync_llm_api_client_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/__init__.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/conftest.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/test_llm_api_client_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/ai21_client/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/ai21_client/conftest.py
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/ai21_client/test_ai21.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/anthropic_client/__init__.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/anthropic_client/conftest.py
--rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/anthropic_client/test_anthropic_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/google_client/__init__.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/google_client/conftest.py
--rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/google_client/test_google_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/huggingface_client/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/huggingface_client/conftest.py
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/huggingface_client/test_huggingface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/openai_client/__init__.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/openai_client/conftest.py
--rw-r--r--   0        0        0     9036 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/openai_client/test_openai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_client/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_client/local_client/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_client/local_client/conftest.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_client/local_client/test_local_client.py
--rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/resources/ai21/text_completion.json
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/resources/ai21/tokenize.json
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/resources/google/chat_completion.json
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/resources/google/embedding.json
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/resources/google/text_completion.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/resources/google/tokens_count.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/resources/huggingface/text_completion.json
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/resources/openai/chat_completion.json
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/resources/openai/text_completion.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/test_utils/__init__.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/test_utils/load_json_resource.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 llm_client-0.7.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 llm_client-0.7.0/LICENSE
--rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 llm_client-0.7.0/README.md
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 llm_client-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 llm_client-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 llm_client-0.8.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 llm_client-0.8.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 llm_client-0.8.0/llm_client/__init__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 llm_client-0.8.0/llm_client/base_llm_client.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 llm_client-0.8.0/llm_client/consts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.8.0/llm_client/llm_api_client/__init__.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 llm_client-0.8.0/llm_client/llm_api_client/ai21_client.py
+-rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 llm_client-0.8.0/llm_client/llm_api_client/aleph_alpha_client.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 llm_client-0.8.0/llm_client/llm_api_client/anthropic_client.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 llm_client-0.8.0/llm_client/llm_api_client/base_llm_api_client.py
+-rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 llm_client-0.8.0/llm_client/llm_api_client/google_client.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 llm_client-0.8.0/llm_client/llm_api_client/huggingface_client.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 llm_client-0.8.0/llm_client/llm_api_client/llm_api_client_factory.py
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 llm_client-0.8.0/llm_client/llm_api_client/openai_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.8.0/llm_client/llm_client/__init__.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 llm_client-0.8.0/llm_client/llm_client/local_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.8.0/llm_client/sync/__init__.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 llm_client-0.8.0/llm_client/sync/sync_llm_api_client_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_api_client/__init__.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_api_client/conftest.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_api_client/test_llm_api_client_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_api_client/ai21_client/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_api_client/ai21_client/conftest.py
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_api_client/ai21_client/test_ai21.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_api_client/anthropic_client/__init__.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_api_client/anthropic_client/conftest.py
+-rw-r--r--   0        0        0     8122 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_api_client/anthropic_client/test_anthropic_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_api_client/google_client/__init__.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_api_client/google_client/conftest.py
+-rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_api_client/google_client/test_google_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_api_client/huggingface_client/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_api_client/huggingface_client/conftest.py
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_api_client/huggingface_client/test_huggingface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_api_client/openai_client/__init__.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_api_client/openai_client/conftest.py
+-rw-r--r--   0        0        0    10569 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_api_client/openai_client/test_openai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_client/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_client/local_client/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_client/local_client/conftest.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/llm_client/local_client/test_local_client.py
+-rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/resources/ai21/text_completion.json
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/resources/ai21/tokenize.json
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/resources/google/chat_completion.json
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/resources/google/embedding.json
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/resources/google/text_completion.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/resources/google/tokens_count.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/resources/huggingface/text_completion.json
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/resources/openai/chat_completion.json
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/resources/openai/text_completion.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.8.0/tests/test_utils/load_json_resource.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 llm_client-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 llm_client-0.8.0/LICENSE
+-rw-r--r--   0        0        0     8921 2020-02-02 00:00:00.000000 llm_client-0.8.0/README.md
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 llm_client-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    10593 2020-02-02 00:00:00.000000 llm_client-0.8.0/PKG-INFO
```

### Comparing `llm_client-0.7.0/.github/workflows/python-publish.yml` & `llm_client-0.8.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/.github/workflows/test.yml` & `llm_client-0.8.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/llm_client/__init__.py` & `llm_client-0.8.0/llm_client/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 
 from llm_client.base_llm_client import BaseLLMClient
 
 # load api clients
 try:
-    from llm_client.llm_api_client.base_llm_api_client import BaseLLMAPIClient, LLMAPIClientConfig
+    from llm_client.llm_api_client.base_llm_api_client import BaseLLMAPIClient, LLMAPIClientConfig, ChatMessage, Role
     from llm_client.llm_api_client.llm_api_client_factory import LLMAPIClientFactory, LLMAPIClientType
     # load base-api clients
     try:
         from llm_client.llm_api_client.ai21_client import AI21Client
         from llm_client.llm_api_client.aleph_alpha_client import AlephAlphaClient
         from llm_client.llm_api_client.google_client import GoogleClient, MessagePrompt
     except ImportError:
         pass
     # load apis with different dependencies
     try:
-        from llm_client.llm_api_client.openai_client import OpenAIClient, ChatMessage, Role
+        from llm_client.llm_api_client.openai_client import OpenAIClient
     except ImportError:
         pass
     try:
         from llm_client.llm_api_client.huggingface_client import HuggingFaceClient
     except ImportError:
         pass
     try:
```

### Comparing `llm_client-0.7.0/llm_client/llm_api_client/ai21_client.py` & `llm_client-0.8.0/llm_client/llm_api_client/ai21_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/llm_client/llm_api_client/aleph_alpha_client.py` & `llm_client-0.8.0/llm_client/llm_api_client/aleph_alpha_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/llm_client/llm_api_client/anthropic_client.py` & `llm_client-0.8.0/llm_client/llm_api_client/huggingface_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 from typing import Optional
 
-from anthropic import AsyncAnthropic
+from transformers import AutoTokenizer
 
 from llm_client.llm_api_client.base_llm_api_client import BaseLLMAPIClient, LLMAPIClientConfig
-from llm_client.consts import PROMPT_KEY
 
-COMPLETE_PATH = "complete"
-BASE_URL = "https://api.anthropic.com/v1/"
-COMPLETIONS_KEY = "completion"
-AUTH_HEADER = "x-api-key"
-ACCEPT_HEADER = "Accept"
-VERSION_HEADER = "anthropic-version"
-ACCEPT_VALUE = "application/json"
-MAX_TOKENS_KEY = "max_tokens_to_sample"
+DEFAULT_DIR = "OpenAssistant"
+BASE_URL = f"https://api-inference.huggingface.co/models/{DEFAULT_DIR}/"
+COMPLETIONS_KEY = 0
+INPUT_KEY = "inputs"
+TEXT_KEY = "generated_text"
+AUTH_HEADER = "Authorization"
+BEARER_TOKEN = "Bearer "
+DEFAULT_MODEL = "oasst-sft-4-pythia-12b-epoch-3.5"
+CONST_SLASH = '/'
+EMPTY_STR = ''
+NEWLINE = '\n'
+TEMPERATURE_KEY = "temperature"
+TOKENS_KEY = "max_length"
 
 
-class AnthropicClient(BaseLLMAPIClient):
+class HuggingFaceClient(BaseLLMAPIClient):
     def __init__(self, config: LLMAPIClientConfig):
         super().__init__(config)
         if self._base_url is None:
             self._base_url = BASE_URL
-        self._anthropic = AsyncAnthropic()
-        if self._headers.get(VERSION_HEADER) is None:
-            self._headers[VERSION_HEADER] = self._anthropic.default_headers[VERSION_HEADER]
-        self._headers[ACCEPT_HEADER] = ACCEPT_VALUE
-        self._headers[AUTH_HEADER] = self._api_key
-
-    async def text_completion(self, prompt: str, model: Optional[str] = None, max_tokens: Optional[int] = None,
-                              temperature: float = 1, top_p: Optional[float] = None,
-                              **kwargs) -> \
-            list[str]:
-        if max_tokens is None and kwargs.get(MAX_TOKENS_KEY) is None:
-            raise ValueError(f"max_tokens or {MAX_TOKENS_KEY} must be specified")
-        if top_p:
-            kwargs["top_p"] = top_p
-        self._set_model_in_kwargs(kwargs, model)
-        kwargs[PROMPT_KEY] = prompt
-        kwargs[MAX_TOKENS_KEY] = kwargs.pop(MAX_TOKENS_KEY, max_tokens)
-        kwargs["temperature"] = temperature
-        response = await self._session.post(self._base_url + COMPLETE_PATH,
+        if self._default_model is None:
+            self._default_model = DEFAULT_MODEL
+        self._headers[AUTH_HEADER] = BEARER_TOKEN + self._api_key
+
+    async def text_completion(self, prompt: str, max_tokens: Optional[int] = None, temperature: float = 1.0,
+                              model: Optional[str] = None, top_p: Optional[float] = None, **kwargs) -> list[str]:
+        model = model or self._default_model
+        kwargs["top_p"] = top_p
+        kwargs[INPUT_KEY] = prompt
+        kwargs[TEMPERATURE_KEY] = temperature
+        kwargs[TOKENS_KEY] = kwargs.pop(TOKENS_KEY, max_tokens)
+        response = await self._session.post(self._base_url + model + CONST_SLASH,
                                             json=kwargs,
                                             headers=self._headers,
                                             raise_for_status=True)
         response_json = await response.json()
-        return [response_json[COMPLETIONS_KEY]]
-
-    async def get_tokens_count(self, text: str, **kwargs) -> int:
-        return await self._anthropic.count_tokens(text)
+        if isinstance(response_json, list):
+            completions = response_json[COMPLETIONS_KEY][TEXT_KEY]
+        else:
+            completions = response_json[TEXT_KEY]
+        return [completion for completion in completions.split(NEWLINE) if completion != EMPTY_STR][1:]
+
+    def get_tokens_count(self, text: str, **kwargs) -> int:
+        tokenizer = AutoTokenizer.from_pretrained(DEFAULT_DIR + CONST_SLASH + self._default_model)
+        return len(tokenizer.encode(text))
```

### Comparing `llm_client-0.7.0/llm_client/llm_api_client/google_client.py` & `llm_client-0.8.0/llm_client/llm_api_client/google_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/llm_client/llm_api_client/llm_api_client_factory.py` & `llm_client-0.8.0/llm_client/llm_api_client/llm_api_client_factory.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/llm_client/llm_client/local_client.py` & `llm_client-0.8.0/llm_client/llm_client/local_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/llm_client/sync/sync_llm_api_client_factory.py` & `llm_client-0.8.0/llm_client/sync/sync_llm_api_client_factory.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/tests/llm_api_client/test_llm_api_client_factory.py` & `llm_client-0.8.0/tests/llm_api_client/test_llm_api_client_factory.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/tests/llm_api_client/ai21_client/conftest.py` & `llm_client-0.8.0/tests/llm_api_client/ai21_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/tests/llm_api_client/ai21_client/test_ai21.py` & `llm_client-0.8.0/tests/llm_api_client/ai21_client/test_ai21.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/tests/llm_api_client/anthropic_client/conftest.py` & `llm_client-0.8.0/tests/llm_api_client/anthropic_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/tests/llm_api_client/anthropic_client/test_anthropic_client.py` & `llm_client-0.8.0/tests/llm_api_client/anthropic_client/test_anthropic_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,70 @@
+from unittest.mock import AsyncMock
+
 import pytest
 
-from llm_client import LLMAPIClientFactory, LLMAPIClientType
+from llm_client import LLMAPIClientFactory, LLMAPIClientType, ChatMessage
 from llm_client.consts import PROMPT_KEY, MODEL_KEY
 from llm_client.llm_api_client.anthropic_client import AUTH_HEADER, COMPLETIONS_KEY, MAX_TOKENS_KEY, ACCEPT_HEADER, \
-    ACCEPT_VALUE, VERSION_HEADER, AnthropicClient
+    ACCEPT_VALUE, VERSION_HEADER, AnthropicClient, USER_PREFIX, ASSISTANT_PREFIX, START_PREFIX, SYSTEM_START_PREFIX, \
+    SYSTEM_END_PREFIX
+from llm_client.llm_api_client.base_llm_api_client import Role
 
 
 @pytest.mark.asyncio
 async def test_get_llm_api_client__with_anthropic(config):
     del config.session
     async with LLMAPIClientFactory() as llm_api_client_factory:
         actual = llm_api_client_factory.get_llm_api_client(LLMAPIClientType.ANTHROPIC, **config.__dict__)
 
     assert isinstance(actual, AnthropicClient)
 
 @pytest.mark.asyncio
+async def test_chat_completion_sanity(llm_client):
+    text_completion_mock = AsyncMock(return_value=["completion text"])
+    llm_client.text_completion = text_completion_mock
+
+    actual = await llm_client.chat_completion(messages=[ChatMessage(Role.USER, "Why is the sky blue?")], max_tokens=10)
+
+    assert actual == ["completion text"]
+    text_completion_mock.assert_awaited_once_with(f"{START_PREFIX}{USER_PREFIX} Why is the sky blue?"
+                                                  f"{START_PREFIX}{ASSISTANT_PREFIX}", None, 10, 1)
+
+
+@pytest.mark.asyncio
+async def test_chat_completion_with_assistant_in_the_end(llm_client):
+    text_completion_mock = AsyncMock(return_value=["completion text"])
+    llm_client.text_completion = text_completion_mock
+
+    actual = await llm_client.chat_completion(messages=[ChatMessage(Role.USER, "Why is the sky blue?"),
+                                                        ChatMessage(Role.ASSISTANT, "Answer - ")], temperature=10)
+
+    assert actual == ["completion text"]
+    text_completion_mock.assert_awaited_once_with(f"{START_PREFIX}{USER_PREFIX} Why is the sky blue?"
+                                                  f"{START_PREFIX}{ASSISTANT_PREFIX} Answer -", None, None,
+                                                  10)
+
+
+@pytest.mark.asyncio
+async def test_chat_completion_with_system(llm_client):
+    text_completion_mock = AsyncMock(return_value=["completion text"])
+    llm_client.text_completion = text_completion_mock
+
+    actual = await llm_client.chat_completion(messages=[ChatMessage(Role.SYSTEM, "Be nice!"),
+                                                        ChatMessage(Role.USER, "Why is the sky blue?")], max_tokens=10,
+                                              temperature=2)
+
+    assert actual == ["completion text"]
+    text_completion_mock.assert_awaited_once_with(f"{START_PREFIX}{USER_PREFIX} "
+                                                  f"{SYSTEM_START_PREFIX}Be nice!{SYSTEM_END_PREFIX}{START_PREFIX}"
+                                                  f"{USER_PREFIX} Why is the sky blue?"
+                                                  f"{START_PREFIX}{ASSISTANT_PREFIX}", None, 10, 2)
+
+
+@pytest.mark.asyncio
 async def test_text_completion__sanity(mock_aioresponse, llm_client, complete_url, anthropic_version):
     mock_aioresponse.post(
         complete_url,
         payload={COMPLETIONS_KEY: "completion text"}
     )
 
     actual = await llm_client.text_completion(prompt="These are a few of my favorite", max_tokens=10,)
```

### Comparing `llm_client-0.7.0/tests/llm_api_client/google_client/conftest.py` & `llm_client-0.8.0/tests/llm_api_client/google_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/tests/llm_api_client/google_client/test_google_client.py` & `llm_client-0.8.0/tests/llm_api_client/google_client/test_google_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/tests/llm_api_client/huggingface_client/conftest.py` & `llm_client-0.8.0/tests/llm_api_client/huggingface_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/tests/llm_api_client/huggingface_client/test_huggingface.py` & `llm_client-0.8.0/tests/llm_api_client/huggingface_client/test_huggingface.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/tests/llm_api_client/openai_client/conftest.py` & `llm_client-0.8.0/tests/llm_api_client/openai_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/tests/llm_api_client/openai_client/test_openai.py` & `llm_client-0.8.0/tests/llm_api_client/openai_client/test_openai.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from unittest.mock import AsyncMock, MagicMock
 
 import pytest
 from aiohttp import ClientSession
 from openai.openai_object import OpenAIObject
 
 from llm_client import OpenAIClient, LLMAPIClientType, LLMAPIClientFactory
-from llm_client.llm_api_client.base_llm_api_client import LLMAPIClientConfig
-from llm_client.llm_api_client.openai_client import ChatMessage, Role
+from llm_client.llm_api_client.base_llm_api_client import LLMAPIClientConfig, Role
+from llm_client.llm_api_client.openai_client import ChatMessage
 from tests.test_utils.load_json_resource import load_json_resource
 
 
 @pytest.mark.asyncio
 async def test_get_llm_api_client__with_open_ai(config):
     del config.session
     async with LLMAPIClientFactory() as llm_api_client_factory:
-
         actual = llm_api_client_factory.get_llm_api_client(LLMAPIClientType.OPEN_AI, **config.__dict__)
 
     assert isinstance(actual, OpenAIClient)
 
 
 def test_init__sanity(openai_mock, client_session):
     OpenAIClient(LLMAPIClientConfig("fake_api_key", client_session))
@@ -33,151 +32,176 @@
         return_value=OpenAIObject.construct_from(load_json_resource("openai/text_completion.json")))
     actual = await open_ai_client.text_completion(prompt="These are a few of my favorite")
 
     assert actual == ["\n\nThis is indeed a test"]
     openai_mock.Completion.acreate.assert_awaited_once_with(
         model=model_name,
         prompt="These are a few of my favorite",
-        headers={},temperature=0,max_tokens=16,top_p=1)
+        headers={}, temperature=0, max_tokens=16, top_p=1)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__return_multiple_completions(openai_mock, open_ai_client, model_name):
     open_ai_object = OpenAIObject.construct_from(load_json_resource("openai/text_completion.json"))
     open_ai_object.choices.append(OpenAIObject.construct_from({"text": "second completion"}))
     openai_mock.Completion.acreate = AsyncMock(return_value=open_ai_object)
 
     actual = await open_ai_client.text_completion(prompt="These are a few of my favorite")
 
     assert actual == ["\n\nThis is indeed a test", "second completion"]
     openai_mock.Completion.acreate.assert_awaited_once_with(
         model=model_name,
         prompt="These are a few of my favorite",
-        headers={},temperature=0,max_tokens=16,top_p=1)
+        headers={}, temperature=0, max_tokens=16, top_p=1)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__override_model(openai_mock, open_ai_client, model_name):
     new_model_name = "gpt3"
     openai_mock.Completion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/text_completion.json")))
 
     actual = await open_ai_client.text_completion(prompt="These are a few of my favorite", model=new_model_name)
 
     assert actual == ["\n\nThis is indeed a test"]
     openai_mock.Completion.acreate.assert_awaited_once_with(
         model=new_model_name,
         prompt="These are a few of my favorite",
-        headers={},temperature=0,max_tokens=16,top_p=1)
+        headers={}, temperature=0, max_tokens=16, top_p=1)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__with_kwargs(openai_mock, open_ai_client, model_name):
     openai_mock.Completion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/text_completion.json")))
 
     actual = await open_ai_client.text_completion(prompt="These are a few of my favorite", max_tokens=10)
 
     assert actual == ["\n\nThis is indeed a test"]
     openai_mock.Completion.acreate.assert_awaited_once_with(
         model=model_name,
         prompt="These are a few of my favorite",
-        temperature=0,max_tokens=10,top_p=1,
+        temperature=0, max_tokens=10, top_p=1,
         headers={})
 
 
 @pytest.mark.asyncio
 async def test_text_completion__with_headers(openai_mock, model_name):
     openai_mock.Completion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/text_completion.json")))
     open_ai_client = OpenAIClient(LLMAPIClientConfig("fake_api_key", MagicMock(ClientSession), default_model=model_name,
-                                  headers={"header_name": "header_value"}))
+                                                     headers={"header_name": "header_value"}))
 
     actual = await open_ai_client.text_completion(prompt="These are a few of my favorite")
 
     assert actual == ["\n\nThis is indeed a test"]
     openai_mock.Completion.acreate.assert_awaited_once_with(
         model=model_name,
         prompt="These are a few of my favorite",
-        headers={"header_name": "header_value"},temperature=0,max_tokens=16,top_p=1)
+        headers={"header_name": "header_value"}, temperature=0, max_tokens=16, top_p=1)
 
 
 @pytest.mark.asyncio
 async def test_chat_completion__sanity(openai_mock, open_ai_client, model_name):
     openai_mock.ChatCompletion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/chat_completion.json")))
 
     actual = await open_ai_client.chat_completion([ChatMessage(Role.USER, "Hello!")])
 
     assert actual == ["\n\nHello there, how may I assist you today?"]
     openai_mock.ChatCompletion.acreate.assert_awaited_once_with(
         model=model_name,
         messages=[{'content': 'Hello!', 'role': 'user'}],
-        headers={},temperature=0,max_tokens=16,top_p=1)
+        headers={}, temperature=0, max_tokens=16, top_p=1)
 
 
 @pytest.mark.asyncio
 async def test_chat_completion__return_multiple_completions(openai_mock, open_ai_client, model_name):
     open_ai_object = OpenAIObject.construct_from(load_json_resource("openai/chat_completion.json"))
     open_ai_object.choices.append(OpenAIObject.construct_from({"message": {"content": "second completion"}}))
     openai_mock.ChatCompletion.acreate = AsyncMock(return_value=open_ai_object)
 
     actual = await open_ai_client.chat_completion([ChatMessage(Role.USER, "Hello!")])
 
     assert actual == ["\n\nHello there, how may I assist you today?", "second completion"]
     openai_mock.ChatCompletion.acreate.assert_awaited_once_with(
         model=model_name,
         messages=[{'content': 'Hello!', 'role': 'user'}],
-        headers={},temperature=0,max_tokens=16,top_p=1)
+        headers={}, temperature=0, max_tokens=16, top_p=1)
 
 
 @pytest.mark.asyncio
 async def test_chat_completion__override_model(openai_mock, open_ai_client, model_name):
     new_model_name = "gpt3"
     openai_mock.ChatCompletion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/chat_completion.json")))
 
     actual = await open_ai_client.chat_completion([ChatMessage(Role.USER, "Hello!")], model=new_model_name)
 
     assert actual == ["\n\nHello there, how may I assist you today?"]
     openai_mock.ChatCompletion.acreate.assert_awaited_once_with(
         model=new_model_name,
         messages=[{'content': 'Hello!', 'role': 'user'}],
-        headers={},temperature=0,max_tokens=16,top_p=1)
+        headers={}, temperature=0, max_tokens=16, top_p=1)
 
 
 @pytest.mark.asyncio
 async def test_chat_completion__with_kwargs(openai_mock, open_ai_client, model_name):
     openai_mock.ChatCompletion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/chat_completion.json")))
 
-    actual = await open_ai_client.chat_completion([ChatMessage(Role.USER, "Hello!")], max_tokens=10,top_p=1)
+    actual = await open_ai_client.chat_completion([ChatMessage(Role.USER, "Hello!")], max_tokens=10, top_p=1)
 
     assert actual == ["\n\nHello there, how may I assist you today?"]
     openai_mock.ChatCompletion.acreate.assert_awaited_once_with(
         model=model_name,
         messages=[{'content': 'Hello!', 'role': 'user'}],
         max_tokens=10,
-        headers={},temperature=0,top_p=1)
+        headers={}, temperature=0, top_p=1)
 
 
 @pytest.mark.asyncio
 async def test_chat_completion__with_headers(openai_mock, model_name):
     openai_mock.ChatCompletion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/chat_completion.json")))
     open_ai_client = OpenAIClient(LLMAPIClientConfig("fake_api_key", MagicMock(ClientSession), default_model=model_name,
-                                  headers={"header_name": "header_value"}))
+                                                     headers={"header_name": "header_value"}))
 
     actual = await open_ai_client.chat_completion([ChatMessage(Role.USER, "Hello!")])
 
     assert actual == ["\n\nHello there, how may I assist you today?"]
     openai_mock.ChatCompletion.acreate.assert_awaited_once_with(
         model=model_name,
         messages=[{'content': 'Hello!', 'role': 'user'}],
-        headers={"header_name": "header_value"},temperature=0,max_tokens=16,top_p=1)
+        headers={"header_name": "header_value"}, temperature=0, max_tokens=16, top_p=1)
+
+
+@pytest.mark.asyncio
+@pytest.mark.parametrize("model_name,expected", [("gpt-3.5-turbo-0301", 127), ("gpt-3.5-turbo-0613", 129),
+                                                 ("gpt-3.5-turbo", 129), ("gpt-4-0314", 129), ("gpt-4-0613", 129),
+                                                 ("gpt-4", 129)])
+async def test_get_chat_tokens_count__with_examples_from_openai_cookbook(model_name, expected, open_ai_client):
+    example_messages = [
+        ChatMessage(Role.SYSTEM,
+                    "You are a helpful, pattern-following assistant that translates corporate jargon "
+                    "into plain English."),
+        ChatMessage(Role.SYSTEM, "New synergies will help drive top-line growth.", name="example_user"),
+        ChatMessage(Role.SYSTEM, "Things working well together will increase revenue.", name="example_assistant"),
+        ChatMessage(Role.SYSTEM,
+                    "Let's circle back when we have more bandwidth to touch base on opportunities "
+                    "for increased leverage.", name="example_user"),
+        ChatMessage(Role.SYSTEM, "Let's talk later when we're less busy about how to do better.",
+                    name="example_assistant"),
+        ChatMessage(Role.USER,
+                    "This late pivot means we don't have time to boil the ocean for the client deliverable."),
+    ]
+
+    actual = await open_ai_client.get_chat_tokens_count(example_messages, model=model_name)
+
+    assert actual == expected
 
 
 @pytest.mark.asyncio
 async def test_get_tokens_count__sanity(model_name, open_ai_client, tiktoken_mock):
     tokeniser_mock = tiktoken_mock.encoding_for_model.return_value
     tokeniser_mock.encode.return_value = [123, 456]
     text = "This is a test"
```

### Comparing `llm_client-0.7.0/tests/llm_client/local_client/conftest.py` & `llm_client-0.8.0/tests/llm_client/local_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/tests/llm_client/local_client/test_local_client.py` & `llm_client-0.8.0/tests/llm_client/local_client/test_local_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/tests/resources/ai21/text_completion.json` & `llm_client-0.8.0/tests/resources/ai21/text_completion.json`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/.gitignore` & `llm_client-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/LICENSE` & `llm_client-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_client-0.7.0/README.md` & `llm_client-0.8.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,32 +8,48 @@
 
 Our vision is to provide async native and production ready SDK while creating 
 a powerful and fast integration with different LLM without letting the user lose 
 any flexibility (API params, endpoints etc.). *We also provide sync version, see
 more details below in Usage section.
 
 ## Base Interface
-The package exposes two simple interfaces for communicating with LLMs (In the future, we 
+The package exposes two simple interfaces for seamless integration with LLMs (In the future, we 
 will expand the interface to support more tasks like list models, edits, etc.):
 ```python
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from typing import Any, Optional
+from enum import Enum
+from dataclasses_json import dataclass_json, config
 from aiohttp import ClientSession
 
 
 class BaseLLMClient(ABC):
     @abstractmethod
     async def text_completion(self, prompt: str, **kwargs) -> list[str]:
         raise NotImplementedError()
 
     async def get_tokens_count(self, text: str, **kwargs) -> int:
         raise NotImplementedError()
 
 
+class Role(Enum):
+    SYSTEM = "system"
+    USER = "user"
+    ASSISTANT = "assistant"
+
+
+@dataclass_json
+@dataclass
+class ChatMessage:
+    role: Role = field(metadata=config(encoder=lambda role: role.value, decoder=Role))
+    content: str
+    name: Optional[str] = field(default=None, metadata=config(exclude=lambda name: name is None))
+    example: bool = field(default=False, metadata=config(exclude=lambda _: True))
+    
 
 @dataclass
 class LLMAPIClientConfig:
     api_key: str
     session: ClientSession
     base_url: Optional[str] = None
     default_model: Optional[str] = None
@@ -45,16 +61,23 @@
         ...
 
     @abstractmethod
     async def text_completion(self, prompt: str, model: Optional[str] = None, max_tokens: int | None = None,
                               temperature: Optional[float] = None, top_p: Optional[float] = None, **kwargs) -> list[str]:
         raise NotImplementedError()
 
+    async def chat_completion(self, messages: list[ChatMessage], temperature: float = 0,
+                              max_tokens: int = 16, model: Optional[str] = None, **kwargs) -> list[str]:
+        raise NotImplementedError()
+
     async def embedding(self, text: str, model: Optional[str] = None, **kwargs) -> list[float]:
         raise NotImplementedError()
+
+    async def get_chat_tokens_count(self, messages: list[ChatMessage], **kwargs) -> int:
+        raise NotImplementedError()
 ```
 
 ## Requirements
 
 Python 3.9+
 
 ## Installation
@@ -105,18 +128,20 @@
 
 
 async def main():
     async with ClientSession() as session:
         llm_client = OpenAIClient(LLMAPIClientConfig(OPENAI_API_KEY, session, default_model="text-davinci-003",
                                                      headers={"OpenAI-Organization": OPENAI_ORG_ID}))  # The headers are optional
         text = "This is indeed a test"
+        messages = [ChatMessage(role=Role.USER, content="Hello!"),
+                    ChatMessage(role=Role.SYSTEM, content="Hi there! How can I assist you today?")]
 
         print("number of tokens:", await llm_client.get_tokens_count(text))  # 5
-        print("generated chat:", await llm_client.chat_completion(  
-            messages=[ChatMessage(role=Role.USER, content="Hello!")], model="gpt-3.5-turbo"))  # ['Hi there! How can I assist you today?']
+        print("number of tokens for chat completion:", await llm_client.get_chat_tokens_count(messages, model="gpt-3.5-turbo"))  # 23
+        print("generated chat:", await llm_client.chat_completion(messages, model="gpt-3.5-turbo"))  # ['Hi there! How can I assist you today?']
         print("generated text:", await llm_client.text_completion(text))  # [' string\n\nYes, this is a test string. Test strings are used to']
         print("generated embedding:", await llm_client.embedding(text))  # [0.0023064255, -0.009327292, ...]
 ```
 Using LLMAPIClientFactory - Perfect if you want to move fast and to not handle the client session yourself
 ```python
 import os
 from llm_client import LLMAPIClientFactory, LLMAPIClientType
@@ -186,15 +211,15 @@
 
 - [x] Add support for more LLMs
   - [x] Anthropic
   - [x] Google
   - [ ] Cohere
 - [x] Add support for more functions via LLMs 
   - [x] embeddings
-  - [ ] chat
+  - [x] chat
   - [ ] list models
   - [ ] edits
   - [ ] more
 - [ ] Add contributing guidelines and linter
 - [ ] Create an easy way to run multiple LLMs in parallel with the same prompts
 - [x] Convert common models parameter
   - [x] temperature
```

### Comparing `llm_client-0.7.0/pyproject.toml` & `llm_client-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,18 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-dependencies = ["aiohttp >=3.0.0,<4.0.0"]
+dependencies = [
+    "aiohttp >=3.0.0,<4.0.0",
+    "dataclasses_json >= 0.5.0"
+]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/uripeled2/llm-client-sdk"
 
 [project.optional-dependencies]
 test = [
@@ -33,15 +36,14 @@
     "pytest-asyncio",
     "pytest-mock",
     "aioresponses"
 ]
 openai = [
     "openai >=0.27.4",
     "tiktoken >=0.3.3",
-    "dataclasses_json >= 0.5.0"
 ]
 huggingface = [
     "transformers >= 4.0.0"
 ]
 anthropic = [
     "anthropic >= 0.3.2"
 ]
```

### Comparing `llm_client-0.7.0/PKG-INFO` & `llm_client-0.8.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: llm-client
-Version: 0.7.0
+Version: 0.8.0
 Summary: SDK for using LLM
 Project-URL: Homepage, https://github.com/uripeled2/llm-client-sdk
 Author-email: Uri Peled <uripeled2@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Requires-Dist: aiohttp<4.0.0,>=3.0.0
+Requires-Dist: dataclasses-json>=0.5.0
 Provides-Extra: all
 Requires-Dist: llm-client[api,local,sync]; extra == 'all'
 Provides-Extra: anthropic
 Requires-Dist: anthropic>=0.3.2; extra == 'anthropic'
 Provides-Extra: api
 Requires-Dist: llm-client[anthropic,google,huggingface,openai]; extra == 'api'
 Provides-Extra: google
 Requires-Dist: google-generativeai>=0.1.0; extra == 'google'
 Provides-Extra: huggingface
 Requires-Dist: transformers>=4.0.0; extra == 'huggingface'
 Provides-Extra: local
 Requires-Dist: transformers>=4.0.0; extra == 'local'
 Provides-Extra: openai
-Requires-Dist: dataclasses-json>=0.5.0; extra == 'openai'
 Requires-Dist: openai>=0.27.4; extra == 'openai'
 Requires-Dist: tiktoken>=0.3.3; extra == 'openai'
 Provides-Extra: sync
 Requires-Dist: async-to-sync>=0.2.0; extra == 'sync'
 Provides-Extra: test
 Requires-Dist: aioresponses; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
@@ -51,32 +51,48 @@
 
 Our vision is to provide async native and production ready SDK while creating 
 a powerful and fast integration with different LLM without letting the user lose 
 any flexibility (API params, endpoints etc.). *We also provide sync version, see
 more details below in Usage section.
 
 ## Base Interface
-The package exposes two simple interfaces for communicating with LLMs (In the future, we 
+The package exposes two simple interfaces for seamless integration with LLMs (In the future, we 
 will expand the interface to support more tasks like list models, edits, etc.):
 ```python
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from typing import Any, Optional
+from enum import Enum
+from dataclasses_json import dataclass_json, config
 from aiohttp import ClientSession
 
 
 class BaseLLMClient(ABC):
     @abstractmethod
     async def text_completion(self, prompt: str, **kwargs) -> list[str]:
         raise NotImplementedError()
 
     async def get_tokens_count(self, text: str, **kwargs) -> int:
         raise NotImplementedError()
 
 
+class Role(Enum):
+    SYSTEM = "system"
+    USER = "user"
+    ASSISTANT = "assistant"
+
+
+@dataclass_json
+@dataclass
+class ChatMessage:
+    role: Role = field(metadata=config(encoder=lambda role: role.value, decoder=Role))
+    content: str
+    name: Optional[str] = field(default=None, metadata=config(exclude=lambda name: name is None))
+    example: bool = field(default=False, metadata=config(exclude=lambda _: True))
+    
 
 @dataclass
 class LLMAPIClientConfig:
     api_key: str
     session: ClientSession
     base_url: Optional[str] = None
     default_model: Optional[str] = None
@@ -88,16 +104,23 @@
         ...
 
     @abstractmethod
     async def text_completion(self, prompt: str, model: Optional[str] = None, max_tokens: int | None = None,
                               temperature: Optional[float] = None, top_p: Optional[float] = None, **kwargs) -> list[str]:
         raise NotImplementedError()
 
+    async def chat_completion(self, messages: list[ChatMessage], temperature: float = 0,
+                              max_tokens: int = 16, model: Optional[str] = None, **kwargs) -> list[str]:
+        raise NotImplementedError()
+
     async def embedding(self, text: str, model: Optional[str] = None, **kwargs) -> list[float]:
         raise NotImplementedError()
+
+    async def get_chat_tokens_count(self, messages: list[ChatMessage], **kwargs) -> int:
+        raise NotImplementedError()
 ```
 
 ## Requirements
 
 Python 3.9+
 
 ## Installation
@@ -148,18 +171,20 @@
 
 
 async def main():
     async with ClientSession() as session:
         llm_client = OpenAIClient(LLMAPIClientConfig(OPENAI_API_KEY, session, default_model="text-davinci-003",
                                                      headers={"OpenAI-Organization": OPENAI_ORG_ID}))  # The headers are optional
         text = "This is indeed a test"
+        messages = [ChatMessage(role=Role.USER, content="Hello!"),
+                    ChatMessage(role=Role.SYSTEM, content="Hi there! How can I assist you today?")]
 
         print("number of tokens:", await llm_client.get_tokens_count(text))  # 5
-        print("generated chat:", await llm_client.chat_completion(  
-            messages=[ChatMessage(role=Role.USER, content="Hello!")], model="gpt-3.5-turbo"))  # ['Hi there! How can I assist you today?']
+        print("number of tokens for chat completion:", await llm_client.get_chat_tokens_count(messages, model="gpt-3.5-turbo"))  # 23
+        print("generated chat:", await llm_client.chat_completion(messages, model="gpt-3.5-turbo"))  # ['Hi there! How can I assist you today?']
         print("generated text:", await llm_client.text_completion(text))  # [' string\n\nYes, this is a test string. Test strings are used to']
         print("generated embedding:", await llm_client.embedding(text))  # [0.0023064255, -0.009327292, ...]
 ```
 Using LLMAPIClientFactory - Perfect if you want to move fast and to not handle the client session yourself
 ```python
 import os
 from llm_client import LLMAPIClientFactory, LLMAPIClientType
@@ -229,15 +254,15 @@
 
 - [x] Add support for more LLMs
   - [x] Anthropic
   - [x] Google
   - [ ] Cohere
 - [x] Add support for more functions via LLMs 
   - [x] embeddings
-  - [ ] chat
+  - [x] chat
   - [ ] list models
   - [ ] edits
   - [ ] more
 - [ ] Add contributing guidelines and linter
 - [ ] Create an easy way to run multiple LLMs in parallel with the same prompts
 - [x] Convert common models parameter
   - [x] temperature
```

