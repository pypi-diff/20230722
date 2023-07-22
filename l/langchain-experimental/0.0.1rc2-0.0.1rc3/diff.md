# Comparing `tmp/langchain_experimental-0.0.1rc2.tar.gz` & `tmp/langchain_experimental-0.0.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_experimental-0.0.1rc2.tar", max compression
+gzip compressed data, was "langchain_experimental-0.0.1rc3.tar", max compression
```

## Comparing `langchain_experimental-0.0.1rc2.tar` & `langchain_experimental-0.0.1rc3.tar`

### file list

```diff
@@ -1,52 +1,51 @@
--rw-r--r--   0        0        0       93 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/README.md
--rw-r--r--   0        0        0        1 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/__init__.py
--rw-r--r--   0        0        0      617 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/__init__.py
--rw-r--r--   0        0        0      188 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/__init__.py
--rw-r--r--   0        0        0     5244 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/agent.py
--rw-r--r--   0        0        0     1073 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/memory.py
--rw-r--r--   0        0        0     1750 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/output_parser.py
--rw-r--r--   0        0        0     3274 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/prompt.py
--rw-r--r--   0        0        0     6587 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/prompt_generator.py
--rw-r--r--   0        0        0      514 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/__init__.py
--rw-r--r--   0        0        0     7469 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/baby_agi.py
--rw-r--r--   0        0        0     1284 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/task_creation.py
--rw-r--r--   0        0        0      835 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/task_execution.py
--rw-r--r--   0        0        0     1076 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/task_prioritization.py
--rw-r--r--   0        0        0      100 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/README.md
--rw-r--r--   0        0        0        0 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/__init__.py
--rw-r--r--   0        0        0     9041 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/base.py
--rw-r--r--   0        0        0      198 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/constants.py
--rw-r--r--   0        0        0     8322 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/models.py
--rw-r--r--   0        0        0        0 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/univariate/__init__.py
--rw-r--r--   0        0        0     2175 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/univariate/causal.py
--rw-r--r--   0        0        0      706 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/univariate/intervention.py
--rw-r--r--   0        0        0     1750 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/univariate/narrative.py
--rw-r--r--   0        0        0     4503 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/univariate/query.py
--rw-r--r--   0        0        0      260 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/generative_agents/__init__.py
--rw-r--r--   0        0        0    10150 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/generative_agents/generative_agent.py
--rw-r--r--   0        0        0    12461 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/generative_agents/memory.py
--rw-r--r--   0        0        0      199 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/llms/__init__.py
--rw-r--r--   0        0        0     1839 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/llms/jsonformer_decoder.py
--rw-r--r--   0        0        0     2028 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/llms/rellm_decoder.py
--rw-r--r--   0        0        0      277 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/pal_chain/__init__.py
--rw-r--r--   0        0        0    12458 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/pal_chain/base.py
--rw-r--r--   0        0        0     2645 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/pal_chain/colored_object_prompt.py
--rw-r--r--   0        0        0     4301 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/pal_chain/math_prompt.py
--rw-r--r--   0        0        0      363 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/__init__.py
--rw-r--r--   0        0        0     2078 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/agent_executor.py
--rw-r--r--   0        0        0        0 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/executors/__init__.py
--rw-r--r--   0        0        0     1463 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/executors/agent_executor.py
--rw-r--r--   0        0        0     1156 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/executors/base.py
--rw-r--r--   0        0        0        0 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/planners/__init__.py
--rw-r--r--   0        0        0     1362 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/planners/base.py
--rw-r--r--   0        0        0     1799 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/planners/chat_planner.py
--rw-r--r--   0        0        0     1150 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/schema.py
--rw-r--r--   0        0        0       87 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/prompts/__init__.py
--rw-r--r--   0        0        0     1874 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/prompts/load.py
--rw-r--r--   0        0        0      140 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/sql/__init__.py
--rw-r--r--   0        0        0    11414 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/sql/base.py
--rw-r--r--   0        0        0    14202 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/sql/prompt.py
--rw-r--r--   0        0        0     1950 2023-07-21 21:52:48.327310 langchain_experimental-0.0.1rc2/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 langchain_experimental-0.0.1rc2/PKG-INFO
+-rw-r--r--   0        0        0       93 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/README.md
+-rw-r--r--   0        0        0      617 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/__init__.py
+-rw-r--r--   0        0        0      188 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/autogpt/__init__.py
+-rw-r--r--   0        0        0     5244 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/autogpt/agent.py
+-rw-r--r--   0        0        0     1072 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/autogpt/memory.py
+-rw-r--r--   0        0        0     1750 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/autogpt/output_parser.py
+-rw-r--r--   0        0        0     3274 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/autogpt/prompt.py
+-rw-r--r--   0        0        0     6587 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py
+-rw-r--r--   0        0        0      514 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/baby_agi/__init__.py
+-rw-r--r--   0        0        0     7469 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py
+-rw-r--r--   0        0        0     1284 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/baby_agi/task_creation.py
+-rw-r--r--   0        0        0      835 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/baby_agi/task_execution.py
+-rw-r--r--   0        0        0     1076 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py
+-rw-r--r--   0        0        0      100 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/cpal/README.md
+-rw-r--r--   0        0        0        0 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/cpal/__init__.py
+-rw-r--r--   0        0        0     9041 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/cpal/base.py
+-rw-r--r--   0        0        0      198 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/cpal/constants.py
+-rw-r--r--   0        0        0     8322 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/cpal/models.py
+-rw-r--r--   0        0        0        0 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/cpal/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/cpal/templates/univariate/__init__.py
+-rw-r--r--   0        0        0     2175 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/cpal/templates/univariate/causal.py
+-rw-r--r--   0        0        0      706 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/cpal/templates/univariate/intervention.py
+-rw-r--r--   0        0        0     1750 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/cpal/templates/univariate/narrative.py
+-rw-r--r--   0        0        0     4503 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/cpal/templates/univariate/query.py
+-rw-r--r--   0        0        0      260 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/generative_agents/__init__.py
+-rw-r--r--   0        0        0    10150 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/generative_agents/generative_agent.py
+-rw-r--r--   0        0        0    12461 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/generative_agents/memory.py
+-rw-r--r--   0        0        0      199 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/llms/__init__.py
+-rw-r--r--   0        0        0     1838 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/llms/jsonformer_decoder.py
+-rw-r--r--   0        0        0     2027 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/llms/rellm_decoder.py
+-rw-r--r--   0        0        0      277 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/pal_chain/__init__.py
+-rw-r--r--   0        0        0    12482 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/pal_chain/base.py
+-rw-r--r--   0        0        0     2645 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/pal_chain/colored_object_prompt.py
+-rw-r--r--   0        0        0     4301 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/pal_chain/math_prompt.py
+-rw-r--r--   0        0        0      363 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/plan_and_execute/__init__.py
+-rw-r--r--   0        0        0     2078 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/plan_and_execute/agent_executor.py
+-rw-r--r--   0        0        0        0 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/plan_and_execute/executors/__init__.py
+-rw-r--r--   0        0        0     1464 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/plan_and_execute/executors/agent_executor.py
+-rw-r--r--   0        0        0     1156 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/plan_and_execute/executors/base.py
+-rw-r--r--   0        0        0        0 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/plan_and_execute/planners/__init__.py
+-rw-r--r--   0        0        0     1362 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/plan_and_execute/planners/base.py
+-rw-r--r--   0        0        0     1800 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/plan_and_execute/planners/chat_planner.py
+-rw-r--r--   0        0        0     1149 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/plan_and_execute/schema.py
+-rw-r--r--   0        0        0       87 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/prompts/__init__.py
+-rw-r--r--   0        0        0     1873 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/prompts/load.py
+-rw-r--r--   0        0        0      140 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/sql/__init__.py
+-rw-r--r--   0        0        0    11411 2023-07-22 01:33:52.773154 langchain_experimental-0.0.1rc3/langchain_experimental/sql/base.py
+-rw-r--r--   0        0        0    14202 2023-07-22 01:33:52.777154 langchain_experimental-0.0.1rc3/langchain_experimental/sql/prompt.py
+-rw-r--r--   0        0        0     1907 2023-07-22 01:33:52.781154 langchain_experimental-0.0.1rc3/pyproject.toml
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 langchain_experimental-0.0.1rc3/PKG-INFO
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/__init__.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from langchain.experimental.autonomous_agents.autogpt.agent import AutoGPT
-from langchain.experimental.autonomous_agents.baby_agi.baby_agi import BabyAGI
-from langchain.experimental.generative_agents.generative_agent import GenerativeAgent
-from langchain.experimental.generative_agents.memory import GenerativeAgentMemory
-from langchain.experimental.plan_and_execute import (
+from langchain_experimental.autonomous_agents.autogpt.agent import AutoGPT
+from langchain_experimental.autonomous_agents.baby_agi.baby_agi import BabyAGI
+from langchain_experimental.generative_agents.generative_agent import GenerativeAgent
+from langchain_experimental.generative_agents.memory import GenerativeAgentMemory
+from langchain_experimental.plan_and_execute import (
     PlanAndExecute,
     load_agent_executor,
     load_chat_planner,
 )
 
 __all__ = [
     "BabyAGI",
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/agent.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/autogpt/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
-from pydantic import ValidationError
-
 from langchain.chains.llm import LLMChain
 from langchain.chat_models.base import BaseChatModel
-from langchain.experimental.autonomous_agents.autogpt.output_parser import (
-    AutoGPTOutputParser,
-    BaseAutoGPTOutputParser,
-)
-from langchain.experimental.autonomous_agents.autogpt.prompt import AutoGPTPrompt
-from langchain.experimental.autonomous_agents.autogpt.prompt_generator import (
-    FINISH_NAME,
-)
 from langchain.memory import ChatMessageHistory
 from langchain.schema import (
     BaseChatMessageHistory,
     Document,
 )
 from langchain.schema.messages import AIMessage, HumanMessage, SystemMessage
 from langchain.tools.base import BaseTool
 from langchain.tools.human.tool import HumanInputRun
 from langchain.vectorstores.base import VectorStoreRetriever
+from pydantic import ValidationError
+
+from langchain_experimental.autonomous_agents.autogpt.output_parser import (
+    AutoGPTOutputParser,
+    BaseAutoGPTOutputParser,
+)
+from langchain_experimental.autonomous_agents.autogpt.prompt import AutoGPTPrompt
+from langchain_experimental.autonomous_agents.autogpt.prompt_generator import (
+    FINISH_NAME,
+)
 
 
 class AutoGPT:
     """Agent class for interacting with Auto-GPT."""
 
     def __init__(
         self,
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/memory.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/autogpt/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Any, Dict, List
 
-from pydantic import Field
-
 from langchain.memory.chat_memory import BaseChatMemory, get_prompt_input_key
 from langchain.vectorstores.base import VectorStoreRetriever
+from pydantic import Field
 
 
 class AutoGPTMemory(BaseChatMemory):
     retriever: VectorStoreRetriever = Field(exclude=True)
     """VectorStoreRetriever object to connect to."""
 
     @property
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/output_parser.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/autogpt/output_parser.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/prompt.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/autogpt/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import time
 from typing import Any, Callable, List
 
-from pydantic import BaseModel
-
-from langchain.experimental.autonomous_agents.autogpt.prompt_generator import get_prompt
 from langchain.prompts.chat import (
     BaseChatPromptTemplate,
 )
 from langchain.schema.messages import BaseMessage, HumanMessage, SystemMessage
 from langchain.tools.base import BaseTool
 from langchain.vectorstores.base import VectorStoreRetriever
+from pydantic import BaseModel
+
+from langchain_experimental.autonomous_agents.autogpt.prompt_generator import get_prompt
 
 
 class AutoGPTPrompt(BaseChatPromptTemplate, BaseModel):
     ai_name: str
     ai_role: str
     tools: List[BaseTool]
     token_counter: Callable[[str], int]
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/prompt_generator.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/__init__.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/baby_agi/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from langchain.experimental.autonomous_agents.baby_agi.baby_agi import BabyAGI
-from langchain.experimental.autonomous_agents.baby_agi.task_creation import (
+from langchain_experimental.autonomous_agents.baby_agi.baby_agi import BabyAGI
+from langchain_experimental.autonomous_agents.baby_agi.task_creation import (
     TaskCreationChain,
 )
-from langchain.experimental.autonomous_agents.baby_agi.task_execution import (
+from langchain_experimental.autonomous_agents.baby_agi.task_execution import (
     TaskExecutionChain,
 )
-from langchain.experimental.autonomous_agents.baby_agi.task_prioritization import (
+from langchain_experimental.autonomous_agents.baby_agi.task_prioritization import (
     TaskPrioritizationChain,
 )
 
 __all__ = [
     "BabyAGI",
     "TaskPrioritizationChain",
     "TaskExecutionChain",
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/baby_agi.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """BabyAGI agent."""
 from collections import deque
 from typing import Any, Dict, List, Optional
 
-from pydantic import BaseModel, Field
-
 from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.chains.base import Chain
-from langchain.experimental.autonomous_agents.baby_agi.task_creation import (
+from langchain.schema.language_model import BaseLanguageModel
+from langchain.vectorstores.base import VectorStore
+from pydantic import BaseModel, Field
+
+from langchain_experimental.autonomous_agents.baby_agi.task_creation import (
     TaskCreationChain,
 )
-from langchain.experimental.autonomous_agents.baby_agi.task_execution import (
+from langchain_experimental.autonomous_agents.baby_agi.task_execution import (
     TaskExecutionChain,
 )
-from langchain.experimental.autonomous_agents.baby_agi.task_prioritization import (
+from langchain_experimental.autonomous_agents.baby_agi.task_prioritization import (
     TaskPrioritizationChain,
 )
-from langchain.schema.language_model import BaseLanguageModel
-from langchain.vectorstores.base import VectorStore
 
 
 class BabyAGI(Chain, BaseModel):
     """Controller model for the BabyAGI agent."""
 
     task_list: deque = Field(default_factory=deque)
     task_creation_chain: Chain = Field(...)
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/task_creation.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/baby_agi/task_creation.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/task_execution.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/baby_agi/task_execution.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/task_prioritization.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/cpal/base.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/cpal/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,41 +3,41 @@
 """
 from __future__ import annotations
 
 import json
 from typing import Any, ClassVar, Dict, List, Optional, Type
 
 import pydantic
-
 from langchain.base_language import BaseLanguageModel
 from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.chains.base import Chain
 from langchain.chains.llm import LLMChain
-from langchain.experimental.cpal.constants import Constant
-from langchain.experimental.cpal.models import (
+from langchain.output_parsers import PydanticOutputParser
+from langchain.prompts.prompt import PromptTemplate
+
+from langchain_experimental.cpal.constants import Constant
+from langchain_experimental.cpal.models import (
     CausalModel,
     InterventionModel,
     NarrativeModel,
     QueryModel,
     StoryModel,
 )
-from langchain.experimental.cpal.templates.univariate.causal import (
+from langchain_experimental.cpal.templates.univariate.causal import (
     template as causal_template,
 )
-from langchain.experimental.cpal.templates.univariate.intervention import (
+from langchain_experimental.cpal.templates.univariate.intervention import (
     template as intervention_template,
 )
-from langchain.experimental.cpal.templates.univariate.narrative import (
+from langchain_experimental.cpal.templates.univariate.narrative import (
     template as narrative_template,
 )
-from langchain.experimental.cpal.templates.univariate.query import (
+from langchain_experimental.cpal.templates.univariate.query import (
     template as query_template,
 )
-from langchain.output_parsers import PydanticOutputParser
-from langchain.prompts.prompt import PromptTemplate
 
 
 class _BaseStoryElementChain(Chain):
     chain: LLMChain
     input_key: str = Constant.narrative_input.value  #: :meta private:
     output_key: str = Constant.chain_answer.value  #: :meta private:
     pydantic_model: ClassVar[
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/cpal/models.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/cpal/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations  # allows pydantic model to reference itself
 
 import re
 from typing import Any, Optional, Union
 
 import duckdb
 import pandas as pd
+from langchain.graphs.networkx_graph import NetworkxEntityGraph
 from pydantic import BaseModel, Field, PrivateAttr, root_validator, validator
 
-from langchain.experimental.cpal.constants import Constant
-from langchain.graphs.networkx_graph import NetworkxEntityGraph
+from langchain_experimental.cpal.constants import Constant
 
 
 class NarrativeModel(BaseModel):
     """
     Represent the narrative input as three story elements.
     """
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/univariate/causal.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/cpal/templates/univariate/causal.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/univariate/intervention.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/cpal/templates/univariate/intervention.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/univariate/narrative.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/cpal/templates/univariate/narrative.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/univariate/query.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/cpal/templates/univariate/query.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/generative_agents/generative_agent.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/generative_agents/generative_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import re
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Tuple
 
-from pydantic import BaseModel, Field
-
 from langchain.chains import LLMChain
-from langchain.experimental.generative_agents.memory import GenerativeAgentMemory
 from langchain.prompts import PromptTemplate
 from langchain.schema.language_model import BaseLanguageModel
+from pydantic import BaseModel, Field
+
+from langchain_experimental.generative_agents.memory import GenerativeAgentMemory
 
 
 class GenerativeAgent(BaseModel):
     """A character with memory and innate characteristics."""
 
     name: str
     """The character's name."""
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/generative_agents/memory.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/generative_agents/memory.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/llms/jsonformer_decoder.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/llms/jsonformer_decoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Experimental implementation of jsonformer wrapped LLM."""
 from __future__ import annotations
 
 import json
 from typing import TYPE_CHECKING, Any, List, Optional, cast
 
-from pydantic import Field, root_validator
-
 from langchain.callbacks.manager import CallbackManagerForLLMRun
 from langchain.llms.huggingface_pipeline import HuggingFacePipeline
+from pydantic import Field, root_validator
 
 if TYPE_CHECKING:
     import jsonformer
 
 
 def import_jsonformer() -> jsonformer:
     """Lazily import jsonformer."""
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/llms/rellm_decoder.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/llms/rellm_decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Experimental implementation of RELLM wrapped LLM."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, List, Optional, cast
 
-from pydantic import Field, root_validator
-
 from langchain.callbacks.manager import CallbackManagerForLLMRun
 from langchain.llms.huggingface_pipeline import HuggingFacePipeline
 from langchain.llms.utils import enforce_stop_tokens
+from pydantic import Field, root_validator
 
 if TYPE_CHECKING:
     import rellm
     from regex import Pattern as RegexPattern
 else:
     try:
         from regex import Pattern as RegexPattern
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/pal_chain/base.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/pal_chain/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 
 from __future__ import annotations
 
 import ast
 import warnings
 from typing import Any, Dict, List, Optional
 
-from pydantic import Extra, Field, root_validator
-
 from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.chains.base import Chain
 from langchain.chains.llm import LLMChain
-from langchain.chains.pal.colored_object_prompt import COLORED_OBJECT_PROMPT
-from langchain.chains.pal.math_prompt import MATH_PROMPT
 from langchain.schema import BasePromptTemplate
 from langchain.schema.language_model import BaseLanguageModel
 from langchain.utilities import PythonREPL
+from pydantic import Extra, Field, root_validator
+
+from langchain_experimental.pal_chain.colored_object_prompt import COLORED_OBJECT_PROMPT
+from langchain_experimental.pal_chain.math_prompt import MATH_PROMPT
 
 COMMAND_EXECUTION_FUNCTIONS = ["system", "exec", "execfile", "eval"]
 
 
 class PALValidation:
     SOLUTION_EXPRESSION_TYPE_FUNCTION = ast.FunctionDef
     SOLUTION_EXPRESSION_TYPE_VARIABLE = ast.Name
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/pal_chain/colored_object_prompt.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/pal_chain/colored_object_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/pal_chain/math_prompt.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/pal_chain/math_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/agent_executor.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/plan_and_execute/agent_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Optional
 
-from pydantic import Field
-
 from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.chains.base import Chain
-from langchain.experimental.plan_and_execute.executors.base import BaseExecutor
-from langchain.experimental.plan_and_execute.planners.base import BasePlanner
-from langchain.experimental.plan_and_execute.schema import (
+from pydantic import Field
+
+from langchain_experimental.plan_and_execute.executors.base import BaseExecutor
+from langchain_experimental.plan_and_execute.planners.base import BasePlanner
+from langchain_experimental.plan_and_execute.schema import (
     BaseStepContainer,
     ListStepContainer,
 )
 
 
 class PlanAndExecute(Chain):
     planner: BasePlanner
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/executors/agent_executor.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/plan_and_execute/executors/agent_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import List
 
 from langchain.agents.agent import AgentExecutor
 from langchain.agents.structured_chat.base import StructuredChatAgent
-from langchain.experimental.plan_and_execute.executors.base import ChainExecutor
 from langchain.schema.language_model import BaseLanguageModel
 from langchain.tools import BaseTool
 
+from langchain_experimental.plan_and_execute.executors.base import ChainExecutor
+
 HUMAN_MESSAGE_TEMPLATE = """Previous steps: {previous_steps}
 
 Current objective: {current_step}
 
 {agent_scratchpad}"""
 
 TASK_PREFIX = """{objective}
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/executors/base.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/plan_and_execute/executors/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import abstractmethod
 from typing import Any
 
-from pydantic import BaseModel
-
 from langchain.callbacks.manager import Callbacks
 from langchain.chains.base import Chain
-from langchain.experimental.plan_and_execute.schema import StepResponse
+from pydantic import BaseModel
+
+from langchain_experimental.plan_and_execute.schema import StepResponse
 
 
 class BaseExecutor(BaseModel):
     @abstractmethod
     def step(
         self, inputs: dict, callbacks: Callbacks = None, **kwargs: Any
     ) -> StepResponse:
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/planners/base.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/plan_and_execute/planners/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import abstractmethod
 from typing import Any, List, Optional
 
-from pydantic import BaseModel
-
 from langchain.callbacks.manager import Callbacks
 from langchain.chains.llm import LLMChain
-from langchain.experimental.plan_and_execute.schema import Plan, PlanOutputParser
+from pydantic import BaseModel
+
+from langchain_experimental.plan_and_execute.schema import Plan, PlanOutputParser
 
 
 class BasePlanner(BaseModel):
     @abstractmethod
     def plan(self, inputs: dict, callbacks: Callbacks = None, **kwargs: Any) -> Plan:
         """Given input, decide what to do."""
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/planners/chat_planner.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/plan_and_execute/planners/chat_planner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import re
 
 from langchain.chains import LLMChain
-from langchain.experimental.plan_and_execute.planners.base import LLMPlanner
-from langchain.experimental.plan_and_execute.schema import (
+from langchain.prompts import ChatPromptTemplate, HumanMessagePromptTemplate
+from langchain.schema.language_model import BaseLanguageModel
+from langchain.schema.messages import SystemMessage
+
+from langchain_experimental.plan_and_execute.planners.base import LLMPlanner
+from langchain_experimental.plan_and_execute.schema import (
     Plan,
     PlanOutputParser,
     Step,
 )
-from langchain.prompts import ChatPromptTemplate, HumanMessagePromptTemplate
-from langchain.schema.language_model import BaseLanguageModel
-from langchain.schema.messages import SystemMessage
 
 SYSTEM_PROMPT = (
     "Let's first understand the problem and devise a plan to solve the problem."
     " Please output the plan starting with the header 'Plan:' "
     "and then followed by a numbered list of steps. "
     "Please make the plan the minimum number of steps required "
     "to accurately complete the task. If the task is a question, "
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/schema.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/plan_and_execute/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from abc import abstractmethod
 from typing import List, Tuple
 
-from pydantic import BaseModel, Field
-
 from langchain.schema import BaseOutputParser
+from pydantic import BaseModel, Field
 
 
 class Step(BaseModel):
     value: str
 
 
 class Plan(BaseModel):
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/prompts/load.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/prompts/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Susceptible to arbitrary code execution: https://github.com/hwchase17/langchain/issues/4849
 import importlib
 import json
 from pathlib import Path
 from typing import Union
 
 import yaml
-
 from langchain.prompts.loading import load_prompt_from_config, try_load_from_hub
 from langchain.schema.prompts import BasePromptTemplate
 
 
 def load_prompt(path: Union[str, Path]) -> BasePromptTemplate:
     """Unified method for loading a prompt from LangChainHub or local fs."""
     if hub_result := try_load_from_hub(
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/sql/base.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/sql/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """Chain for interacting with SQL Database."""
 from __future__ import annotations
 
 import warnings
 from typing import Any, Dict, List, Optional
 
-from pydantic import Extra, Field, root_validator
-
 from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.chains.base import Chain
 from langchain.chains.llm import LLMChain
-from langchain.chains.sql_database.prompt import DECIDER_PROMPT, PROMPT, SQL_PROMPTS
 from langchain.prompts.prompt import PromptTemplate
 from langchain.schema import BasePromptTemplate
 from langchain.schema.language_model import BaseLanguageModel
 from langchain.tools.sql_database.prompt import QUERY_CHECKER
 from langchain.utilities.sql_database import SQLDatabase
+from pydantic import Extra, Field, root_validator
+
+from langchain_experimental.sql.prompt import DECIDER_PROMPT, PROMPT, SQL_PROMPTS
 
 INTERMEDIATE_STEPS_KEY = "intermediate_steps"
 
 
 class SQLDatabaseChain(Chain):
     """Chain for interacting with SQL Database.
 
     Example:
         .. code-block:: python
 
-            from langchain.experimental.sql import SQLDatabaseChain
+            from langchain_experimental.sql import SQLDatabaseChain
             from langchain import OpenAI, SQLDatabase
             db = SQLDatabase(...)
             db_chain = SQLDatabaseChain.from_llm(OpenAI(), db)
     """
 
     llm_chain: LLMChain
     llm: Optional[BaseLanguageModel] = None
```

### Comparing `langchain_experimental-0.0.1rc2/langchain/experimental/sql/prompt.py` & `langchain_experimental-0.0.1rc3/langchain_experimental/sql/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc2/pyproject.toml` & `langchain_experimental-0.0.1rc3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 [tool.poetry]
 name = "langchain-experimental"
-version = "0.0.1rc2"
+version = "0.0.1rc3"
 description = "Building applications with LLMs through composability"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://www.github.com/hwchase17/langchain"
-packages = [
-    {include = "langchain"}
-]
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 langchain = ">=0.0.239"
```

### Comparing `langchain_experimental-0.0.1rc2/PKG-INFO` & `langchain_experimental-0.0.1rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-experimental
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: Building applications with LLMs through composability
 Home-page: https://www.github.com/hwchase17/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

