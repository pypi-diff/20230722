# Comparing `tmp/one-api-tool-0.4.8.tar.gz` & `tmp/one-api-tool-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.4.8.tar", last modified: Fri Jul 21 08:12:24 2023, max compression
+gzip compressed data, was "one-api-tool-0.4.9.tar", last modified: Fri Jul 21 10:18:02 2023, max compression
```

## Comparing `one-api-tool-0.4.8.tar` & `one-api-tool-0.4.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 08:12:24.634886 one-api-tool-0.4.8/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.4.8/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     7677 2023-07-21 08:12:24.634702 one-api-tool-0.4.8/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     7121 2023-07-21 08:10:20.000000 one-api-tool-0.4.8/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 08:12:24.632772 one-api-tool-0.4.8/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     7677 2023-07-21 08:12:24.000000 one-api-tool-0.4.8/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      359 2023-07-21 08:12:24.000000 one-api-tool-0.4.8/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-21 08:12:24.000000 one-api-tool-0.4.8/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-21 08:12:24.000000 one-api-tool-0.4.8/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       86 2023-07-21 08:12:24.000000 one-api-tool-0.4.8/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-21 08:12:24.000000 one-api-tool-0.4.8/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 08:12:24.633736 one-api-tool-0.4.8/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 04:37:23.000000 one-api-tool-0.4.8/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 08:12:24.634274 one-api-tool-0.4.8/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.4.8/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-06-26 09:39:20.000000 one-api-tool-0.4.8/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    21439 2023-07-21 08:10:55.000000 one-api-tool-0.4.8/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3598 2023-07-04 12:02:12.000000 one-api-tool-0.4.8/oneapi/utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-21 08:12:24.634941 one-api-tool-0.4.8/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1078 2023-07-21 08:11:12.000000 one-api-tool-0.4.8/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 10:18:02.522126 one-api-tool-0.4.9/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.4.9/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7677 2023-07-21 10:18:02.521964 one-api-tool-0.4.9/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7121 2023-07-21 08:10:20.000000 one-api-tool-0.4.9/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 10:18:02.519221 one-api-tool-0.4.9/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7677 2023-07-21 10:18:02.000000 one-api-tool-0.4.9/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      382 2023-07-21 10:18:02.000000 one-api-tool-0.4.9/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-21 10:18:02.000000 one-api-tool-0.4.9/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-21 10:18:02.000000 one-api-tool-0.4.9/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       86 2023-07-21 10:18:02.000000 one-api-tool-0.4.9/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-21 10:18:02.000000 one-api-tool-0.4.9/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 10:18:02.520678 one-api-tool-0.4.9/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-04 04:37:23.000000 one-api-tool-0.4.9/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 10:18:02.521400 one-api-tool-0.4.9/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.4.9/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-06-26 09:39:20.000000 one-api-tool-0.4.9/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    21837 2023-07-21 10:15:35.000000 one-api-tool-0.4.9/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)      907 2023-07-21 10:14:04.000000 one-api-tool-0.4.9/oneapi/one_api_test.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3598 2023-07-04 12:02:12.000000 one-api-tool-0.4.9/oneapi/utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-21 10:18:02.522174 one-api-tool-0.4.9/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1078 2023-07-21 10:16:41.000000 one-api-tool-0.4.9/setup.py
```

### Comparing `one-api-tool-0.4.8/LICENSE` & `one-api-tool-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.8/PKG-INFO` & `one-api-tool-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.4.8
+Version: 0.4.9
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.4.8/README.md` & `one-api-tool-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.8/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.4.9/one_api_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.4.8
+Version: 0.4.9
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.4.8/oneapi/commands/one_api_requst.py` & `one-api-tool-0.4.9/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.8/oneapi/one_api.py` & `one-api-tool-0.4.9/oneapi/one_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,23 +22,25 @@
 )
 CLAUDE_TEMPLATE = "\n\nHuman: {prompt}\n\nAssistant:"
     
 class AbstrctMethod(BaseModel):
     api_key: str
     api_base: str
     api_type: str
+    api_version: str
     method_list_models :str 
     method_model_info :str
     method_chat :str
     method_commpletions :str
 
 class ClaudeMethod(AbstrctMethod):
     api_key: str
     api_base: str = "https://api.anthropic.com",
     api_type: str = "claude"
+    api_version: str = None
     method_list_models = ""
     method_model_info = ""
     method_chat = "/v1/complete"
     method_commpletions = ""
 
 class AzureMethod(AbstrctMethod):
     api_key: str
@@ -51,14 +53,15 @@
     method_model_info :str = ""
     method_commpletions :str = ""
 
 class OpenAIMethod(AbstrctMethod):
     api_key: str
     api_base: str = "https://api.openai.com/v1"
     api_type: str = "open_ai"
+    api_version: str = None
     method_list_models = "models"
     method_model_info = "models"
     method_chat = "/chat/completions"
     method_commpletions = "completions"
 
 class OpenAIDecodingArguments(BaseModel):
     messages: List[dict] 
@@ -112,28 +115,30 @@
         
 
 class OpenAITool(AbstractAPITool):
 
     def __init__(self,method : AbstrctMethod) -> None:
         self.method = method
         self.encoder = None
-        if isinstance(self.method, AzureMethod):
-            openai.api_key = self.method.api_key
-            openai.api_base = self.method.api_base
-            openai.api_type = self.method.api_type
-            openai.api_version = self.method.api_version
-        else:
-            openai.api_key = self.method.api_key
-            openai.api_base = self.method.api_base
+
+
+    def reset_environment(self):
+        """Reset the environment variables to the default values. When using asyncio to all multiple apis, this function should be called before each api call.
+        """
+        openai.api_key = self.method.api_key
+        openai.api_base = self.method.api_base
+        openai.api_type = self.method.api_type
+        openai.api_version = self.method.api_version
 
     def simple_chat(self, args: OpenAIDecodingArguments):
         """
         https://learn.microsoft.com/en-us/azure/cognitive-services/openai/how-to/chatgpt?pivots=programming-language-chat-completions
         https://platform.openai.com/docs/api-reference/chat
         """
+        self.reset_environment()
         data = args.dict()
         is_function_call = data.get("functions", None) is not None
         if is_function_call:
             data["stream"] = False  
         else:
             if isinstance(args, OpenAIDecodingArguments):
                 data.pop("functions")
@@ -156,23 +161,24 @@
             response_message = completion.choices[0].message
             if is_function_call:
                 if response_message.get("function_call") is not None:
                     return response_message
             return response_message.get("content", "")
 
     async def asimple_chat(self, args: OpenAIDecodingArguments):
+        self.reset_environment()
         data = args.dict()
         is_function_call = data.get("functions", None) is not None
         if is_function_call:
             data["stream"] = False  
         else:
             if isinstance(args, OpenAIDecodingArguments):
                 data.pop("functions")
                 data.pop("function_call")
-        completion = await openai.ChatCompletion.acreate(**data)
+        completion = await openai.ChatCompletion.acreate(**data, api_key=self.method.api_key, api_base=self.method.api_base, api_type=self.method.api_type, api_version=self.method.api_version)
         if data.get("stream", False):
             # create variables to collect the stream of chunks
             collected_chunks = []
             collected_messages = []
             # iterate through the stream of events
             async for chunk in completion:
                 collected_chunks.append(chunk)  # save the event response
@@ -188,29 +194,32 @@
                 if response_message.get("function_call") is not None:
                     return response_message
             return response_message.get("content", "")
          
 
 
     def get_embeddings(self, texts: List[str], engine="text-embedding-ada-002") -> List[List[float]]:
+        self.reset_environment()
         assert len(texts) <= 2048, "The batch size should not be larger than 2048."
         # replace newlines, which can negatively affect performance.
         texts = [text.replace("\n", " ") for text in texts]
 
         data = openai.Embedding.create(input=texts, engine=engine).data
         data = sorted(data, key=lambda x: x["index"])  # maintain the same order as input.
         return [d["embedding"] for d in data]
 
 
     def get_embedding(self, text: str, engine="text-embedding-ada-002") -> List[float]:
+        self.reset_environment()
         # replace newlines, which can negatively affect performance.
         text = text.replace("\n", " ")
         return openai.Embedding.create(input=[text], engine=engine)["data"][0]["embedding"]
 
     def count_tokens(self, texts: List[str], encoding_name: str = 'cl100k_base') -> int:
+        self.reset_environment()
         """
         Encoding name	OpenAI models
         cl100k_base	    gpt-4, gpt-3.5-turbo, text-embedding-ada-002
         p50k_base	    Codex models, text-davinci-002, text-davinci-003
         r50k_base (or gpt2)	GPT-3 models like davinci
         Args:
             texts (List[str]): [description]
```

### Comparing `one-api-tool-0.4.8/oneapi/utils.py` & `one-api-tool-0.4.9/oneapi/utils.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.8/setup.py` & `one-api-tool-0.4.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.4.8",
+    version="0.4.9",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

