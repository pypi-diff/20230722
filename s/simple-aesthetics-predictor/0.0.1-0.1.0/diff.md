# Comparing `tmp/simple_aesthetics_predictor-0.0.1.tar.gz` & `tmp/simple_aesthetics_predictor-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_aesthetics_predictor-0.0.1.tar", max compression
+gzip compressed data, was "simple_aesthetics_predictor-0.1.0.tar", max compression
```

## Comparing `simple_aesthetics_predictor-0.0.1.tar` & `simple_aesthetics_predictor-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2023-07-22 07:14:59.901885 simple_aesthetics_predictor-0.0.1/LICENSE
--rw-r--r--   0        0        0     2019 2023-07-22 07:14:59.901885 simple_aesthetics_predictor-0.0.1/README.md
--rw-r--r--   0        0        0      178 2023-07-22 07:14:59.901885 simple_aesthetics_predictor-0.0.1/aesthetics_predictor/__init__.py
--rw-r--r--   0        0        0      461 2023-07-22 07:14:59.901885 simple_aesthetics_predictor-0.0.1/aesthetics_predictor/utils.py
--rw-r--r--   0        0        0     2338 2023-07-22 07:14:59.901885 simple_aesthetics_predictor-0.0.1/aesthetics_predictor/v1.py
--rw-r--r--   0        0        0     4467 2023-07-22 07:14:59.901885 simple_aesthetics_predictor-0.0.1/aesthetics_predictor/v2.py
--rw-r--r--   0        0        0      685 2023-07-22 07:15:14.838268 simple_aesthetics_predictor-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 simple_aesthetics_predictor-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-22 07:27:34.538768 simple_aesthetics_predictor-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2428 2023-07-22 07:27:34.538768 simple_aesthetics_predictor-0.1.0/README.md
+-rw-r--r--   0        0        0      178 2023-07-22 07:27:34.538768 simple_aesthetics_predictor-0.1.0/aesthetics_predictor/__init__.py
+-rw-r--r--   0        0        0      525 2023-07-22 07:27:34.538768 simple_aesthetics_predictor-0.1.0/aesthetics_predictor/utils.py
+-rw-r--r--   0        0        0     2338 2023-07-22 07:27:34.542768 simple_aesthetics_predictor-0.1.0/aesthetics_predictor/v1.py
+-rw-r--r--   0        0        0     4467 2023-07-22 07:27:34.542768 simple_aesthetics_predictor-0.1.0/aesthetics_predictor/v2.py
+-rw-r--r--   0        0        0      685 2023-07-22 07:27:47.678723 simple_aesthetics_predictor-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3010 1970-01-01 00:00:00.000000 simple_aesthetics_predictor-0.1.0/PKG-INFO
```

### Comparing `simple_aesthetics_predictor-0.0.1/LICENSE` & `simple_aesthetics_predictor-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_aesthetics_predictor-0.0.1/README.md` & `simple_aesthetics_predictor-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # 🤗 Simple Aesthetics Predictor
 
 [![CI](https://github.com/shunk031/simple-aesthetics-predictor/actions/workflows/ci.yaml/badge.svg)](https://github.com/shunk031/simple-aesthetics-predictor/actions/workflows/ci.yaml)
+[![Release](https://github.com/shunk031/simple-aesthetics-predictor/actions/workflows/deploy_and_release.yaml/badge.svg)](https://github.com/shunk031/simple-aesthetics-predictor/actions/workflows/deploy_and_release.yaml)
+![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue?logo=python)
+[![PyPI](https://img.shields.io/pypi/v/simple-aesthetics-predictor.svg)](https://pypi.python.org/pypi/simple-aesthetics-predictor)
 
 [CLIP](https://arxiv.org/abs/2103.00020)-based aesthetics predictor inspired by the interface of [🤗 huggingface transformers](https://huggingface.co/docs/transformers/index). This library provides a simple wrapper that can load the predictor using the `from_pretrained` method.
 
 ## Install
 
 ```shell
-pip install git+https://github.com/shunk031/simple-aesthetics-predictor.git
+pip install simple-aesthetics-predictor
 ```
 
 ## How to Use
 
 ```python
 import requests
 import torch
@@ -47,14 +50,14 @@
 prediction = outputs.logits
 
 print(f"Aesthetics score: {prediction}")
 ```
 
 ## The Predictors found in 🤗 Huggingface Hub
 
-- [🤗 aesthetics-predictor-v1](https://huggingface.co/models?search=aesthetics-predictor-v1)
-- [🤗 aesthetics-predictor-v2](https://huggingface.co/models?search=aesthetics-predictor-v2)
+- 🤗 [aesthetics-predictor-v1](https://huggingface.co/models?search=aesthetics-predictor-v1)
+- 🤗 [aesthetics-predictor-v2](https://huggingface.co/models?search=aesthetics-predictor-v2)
 
 ## Acknowledgements
 
 - LAION-AI/aesthetic-predictor: A linear estimator on top of clip to predict the aesthetic quality of pictures https://github.com/LAION-AI/aesthetic-predictor 
 - christophschuhmann/improved-aesthetic-predictor: CLIP+MLP Aesthetic Score Predictor https://github.com/christophschuhmann/improved-aesthetic-predictor
```

### Comparing `simple_aesthetics_predictor-0.0.1/aesthetics_predictor/v1.py` & `simple_aesthetics_predictor-0.1.0/aesthetics_predictor/v1.py`

 * *Files identical despite different names*

### Comparing `simple_aesthetics_predictor-0.0.1/aesthetics_predictor/v2.py` & `simple_aesthetics_predictor-0.1.0/aesthetics_predictor/v2.py`

 * *Files identical despite different names*

### Comparing `simple_aesthetics_predictor-0.0.1/pyproject.toml` & `simple_aesthetics_predictor-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simple-aesthetics-predictor"
-version = "0.0.1" # specified by poetry-dynamic-versioning
+version = "0.1.0" # specified by poetry-dynamic-versioning
 description = ""
 authors = ["Shunsuke KITADA <shunsuke.kitada.0831@gmail.com>"]
 readme = "README.md"
 packages = [{include = "aesthetics_predictor"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `simple_aesthetics_predictor-0.0.1/PKG-INFO` & `simple_aesthetics_predictor-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-aesthetics-predictor
-Version: 0.0.1
+Version: 0.1.0
 Summary: 
 Author: Shunsuke KITADA
 Author-email: shunsuke.kitada.0831@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -14,21 +14,24 @@
 Requires-Dist: torchvision (>=0.2.1)
 Requires-Dist: transformers (>=4.30.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # 🤗 Simple Aesthetics Predictor
 
 [![CI](https://github.com/shunk031/simple-aesthetics-predictor/actions/workflows/ci.yaml/badge.svg)](https://github.com/shunk031/simple-aesthetics-predictor/actions/workflows/ci.yaml)
+[![Release](https://github.com/shunk031/simple-aesthetics-predictor/actions/workflows/deploy_and_release.yaml/badge.svg)](https://github.com/shunk031/simple-aesthetics-predictor/actions/workflows/deploy_and_release.yaml)
+![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue?logo=python)
+[![PyPI](https://img.shields.io/pypi/v/simple-aesthetics-predictor.svg)](https://pypi.python.org/pypi/simple-aesthetics-predictor)
 
 [CLIP](https://arxiv.org/abs/2103.00020)-based aesthetics predictor inspired by the interface of [🤗 huggingface transformers](https://huggingface.co/docs/transformers/index). This library provides a simple wrapper that can load the predictor using the `from_pretrained` method.
 
 ## Install
 
 ```shell
-pip install git+https://github.com/shunk031/simple-aesthetics-predictor.git
+pip install simple-aesthetics-predictor
 ```
 
 ## How to Use
 
 ```python
 import requests
 import torch
@@ -64,15 +67,15 @@
 prediction = outputs.logits
 
 print(f"Aesthetics score: {prediction}")
 ```
 
 ## The Predictors found in 🤗 Huggingface Hub
 
-- [🤗 aesthetics-predictor-v1](https://huggingface.co/models?search=aesthetics-predictor-v1)
-- [🤗 aesthetics-predictor-v2](https://huggingface.co/models?search=aesthetics-predictor-v2)
+- 🤗 [aesthetics-predictor-v1](https://huggingface.co/models?search=aesthetics-predictor-v1)
+- 🤗 [aesthetics-predictor-v2](https://huggingface.co/models?search=aesthetics-predictor-v2)
 
 ## Acknowledgements
 
 - LAION-AI/aesthetic-predictor: A linear estimator on top of clip to predict the aesthetic quality of pictures https://github.com/LAION-AI/aesthetic-predictor 
 - christophschuhmann/improved-aesthetic-predictor: CLIP+MLP Aesthetic Score Predictor https://github.com/christophschuhmann/improved-aesthetic-predictor
```

