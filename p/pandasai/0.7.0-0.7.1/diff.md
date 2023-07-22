# Comparing `tmp/pandasai-0.7.0.tar.gz` & `tmp/pandasai-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.7.0.tar", max compression
+gzip compressed data, was "pandasai-0.7.1.tar", max compression
```

## Comparing `pandasai-0.7.0.tar` & `pandasai-0.7.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1055 2023-07-20 13:09:33.567383 pandasai-0.7.0/LICENSE
--rw-r--r--   0        0        0     7705 2023-07-20 13:09:33.567383 pandasai-0.7.0/README.md
--rw-r--r--   0        0        0    26182 2023-07-20 13:09:33.571383 pandasai-0.7.0/pandasai/__init__.py
--rw-r--r--   0        0        0      522 2023-07-20 13:09:33.571383 pandasai-0.7.0/pandasai/callbacks/base.py
--rw-r--r--   0        0        0     1438 2023-07-20 13:09:33.571383 pandasai-0.7.0/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-07-20 13:09:33.571383 pandasai-0.7.0/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-20 13:09:33.571383 pandasai-0.7.0/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3814 2023-07-20 13:09:33.571383 pandasai-0.7.0/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     6404 2023-07-20 13:09:33.571383 pandasai-0.7.0/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1742 2023-07-20 13:09:33.571383 pandasai-0.7.0/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-07-20 13:09:33.571383 pandasai-0.7.0/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1493 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3070 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/helpers/openai_info.py
--rw-r--r--   0        0        0     3507 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     9911 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0        0 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4289 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    12056 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1213 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     4440 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      585 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     3130 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      948 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      653 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      647 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1686 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1261 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1513 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1342 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1900 2023-07-20 13:09:33.575383 pandasai-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     8919 1970-01-01 00:00:00.000000 pandasai-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-07-22 21:11:48.623788 pandasai-0.7.1/LICENSE
+-rw-r--r--   0        0        0     7705 2023-07-22 21:11:48.623788 pandasai-0.7.1/README.md
+-rw-r--r--   0        0        0    26182 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/__init__.py
+-rw-r--r--   0        0        0      522 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/callbacks/base.py
+-rw-r--r--   0        0        0     1438 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3814 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     6404 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1742 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1493 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3070 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/helpers/openai_info.py
+-rw-r--r--   0        0        0     3507 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     9911 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0        0 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4289 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    12126 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     4440 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      585 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     3130 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      948 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      653 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      647 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1578 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1261 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1380 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1256 2023-07-22 21:11:48.631788 pandasai-0.7.1/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1900 2023-07-22 21:11:48.635788 pandasai-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     8919 1970-01-01 00:00:00.000000 pandasai-0.7.1/PKG-INFO
```

### Comparing `pandasai-0.7.0/LICENSE` & `pandasai-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/README.md` & `pandasai-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/__init__.py` & `pandasai-0.7.1/pandasai/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/callbacks/base.py` & `pandasai-0.7.1/pandasai/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/constants.py` & `pandasai-0.7.1/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/exceptions.py` & `pandasai-0.7.1/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/helpers/_optional.py` & `pandasai-0.7.1/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/helpers/anonymizer.py` & `pandasai-0.7.1/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/helpers/cache.py` & `pandasai-0.7.1/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/helpers/from_excel.py` & `pandasai-0.7.1/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/helpers/notebook.py` & `pandasai-0.7.1/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/helpers/openai_info.py` & `pandasai-0.7.1/pandasai/helpers/openai_info.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/helpers/save_chart.py` & `pandasai-0.7.1/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/helpers/shortcuts.py` & `pandasai-0.7.1/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/llm/azure_openai.py` & `pandasai-0.7.1/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/llm/base.py` & `pandasai-0.7.1/pandasai/llm/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,17 @@
             NoCodeFoundError: No code found in the response
 
         Returns:
             str: Extracted code from the response
         """
         code = response
         match = re.search(
-            rf"{START_CODE_TAG}(.*)({END_CODE_TAG}|{END_CODE_TAG.replace('<', '</')})",
+            rf"{START_CODE_TAG}(.*)({END_CODE_TAG}"
+            rf"|{END_CODE_TAG.replace('<', '</')}"
+            rf"|{START_CODE_TAG.replace('<', '</')})",
             code,
             re.DOTALL,
         )
         if match:
             code = match.group(1).strip()
         if len(code.split(separator)) > 1:
             code = code.split(separator)[1]
```

### Comparing `pandasai-0.7.0/pandasai/llm/fake.py` & `pandasai-0.7.1/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/llm/falcon.py` & `pandasai-0.7.1/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/llm/google_palm.py` & `pandasai-0.7.1/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/llm/langchain.py` & `pandasai-0.7.1/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/llm/openai.py` & `pandasai-0.7.1/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/llm/starcoder.py` & `pandasai-0.7.1/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/middlewares/base.py` & `pandasai-0.7.1/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/middlewares/charts.py` & `pandasai-0.7.1/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/middlewares/streamlit.py` & `pandasai-0.7.1/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/prompts/base.py` & `pandasai-0.7.1/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.7.1/pandasai/prompts/correct_error_prompt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ Prompt to correct Python Code on Error
 ```
-Today is {today_date}.
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
 This is the metadata of the dataframe:
 {df_head}.
 
 The user asked the following question:
 {question}
 
@@ -15,25 +14,23 @@
 {error_returned}
 
 Correct the python code and return a new python code (do not import anything) that fixes the above
 mentioned error. Do not generate the same code again. Make sure to prefix the requested python
 code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly.
 ```
 """  # noqa: E501
-from datetime import date
 
 from pandasai.constants import END_CODE_TAG, START_CODE_TAG
 from .base import Prompt
 
 
 class CorrectErrorPrompt(Prompt):
     """Prompt to Correct Python code on Error"""
 
     text: str = """
-Today is {today_date}.
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
 This is the metadata of the dataframe:
 {df_head}.
 
 The user asked the following question:
 {question}
 
@@ -48,9 +45,8 @@
 """  # noqa: E501
 
     def __init__(self, **kwargs):
         super().__init__(
             **kwargs,
             START_CODE_TAG=START_CODE_TAG,
             END_CODE_TAG=END_CODE_TAG,
-            today_date=date.today()
         )
```

### Comparing `pandasai-0.7.0/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.7.1/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.0/pandasai/prompts/generate_python_code.py` & `pandasai-0.7.1/pandasai/prompts/generate_python_code.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 """ Prompt to generate Python code
 ```
-Today is {today_date}.
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
 This is the metadata of the dataframe:
 {df_head}.
 
 When asked about the data, your response should include a python code that describes the
 dataframe `df`. Using the provided dataframe, df, return the python code and make sure to prefix
 the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG}
 exactly to get the answer to the following question:
 ```
 """  # noqa: E501
 
-from datetime import date
 
 from pandasai.constants import END_CODE_TAG, START_CODE_TAG
 from .base import Prompt
 
 
 class GeneratePythonCodePrompt(Prompt):
     """Prompt to generate Python code"""
 
     text: str = """
-Today is {today_date}.
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
 This is the metadata of the dataframe:
 {df_head}.
 
 When asked about the data, your response should include a python code that describes the dataframe `df`.
 Using the provided dataframe, df, return the python code and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
 """  # noqa: E501
 
     def __init__(self, **kwargs):
         super().__init__(
-            **kwargs,
-            START_CODE_TAG=START_CODE_TAG,
-            END_CODE_TAG=END_CODE_TAG,
-            today_date=date.today()
+            **kwargs, START_CODE_TAG=START_CODE_TAG, END_CODE_TAG=END_CODE_TAG
         )
```

### Comparing `pandasai-0.7.0/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.7.1/pandasai/prompts/multiple_dataframes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """ Prompt to generate Python code for multiple dataframes """
 
-from datetime import date
 
 import pandas as pd
 
 from pandasai.constants import END_CODE_TAG, START_CODE_TAG
 from .base import Prompt
 
 
 class MultipleDataframesPrompt(Prompt):
     """Prompt to generate Python code"""
 
     text: str = """
-Today is {today_date}.
 You are provided with the following pandas dataframes:"""
     instruction: str = """
 When asked about the data, your response should include a python code that describes the dataframes provided.
 Using the provided dataframes and no other dataframes, return the python code and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
 """  # noqa: E501
 
     def __init__(self, dataframes: list[pd.DataFrame]):
@@ -26,14 +24,13 @@
             self.text += f"""
 Dataframe df{i}, with {row} rows and {col} columns.
 This is the metadata of the dataframe df{i}:
 {dataframe}"""
 
         self.text += self.instruction
         self.text = self.text.format(
-            today_date=date.today(),
             START_CODE_TAG=START_CODE_TAG,
             END_CODE_TAG=END_CODE_TAG,
         )
 
     def __str__(self):
         return self.text
```

### Comparing `pandasai-0.7.0/pyproject.toml` & `pandasai-0.7.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.7.0"
+version = "0.7.1"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pandasai-0.7.0/PKG-INFO` & `pandasai-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.7.0
+Version: 0.7.1
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

