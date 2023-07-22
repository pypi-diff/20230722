# Comparing `tmp/eztils-0.4.4.tar.gz` & `tmp/eztils-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eztils-0.4.4.tar", max compression
+gzip compressed data, was "eztils-0.4.5.tar", max compression
```

## Comparing `eztils-0.4.4.tar` & `eztils-0.4.5.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1075 2023-07-20 20:08:12.299029 eztils-0.4.4/LICENSE
--rw-r--r--   0        0        0    12741 2023-07-20 20:08:12.299029 eztils-0.4.4/README.md
--rw-r--r--   0        0        0      542 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/__init__.py
--rw-r--r--   0        0        0     2359 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/default/__init__.py
--rw-r--r--   0        0        0     3689 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/default/dict_operations.py
--rw-r--r--   0        0        0     2246 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/default/itertools.py
--rw-r--r--   0        0        0     2458 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/default/logging.py
--rw-r--r--   0        0        0     1412 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/default/math.py
--rw-r--r--   0        0        0     1091 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/default/structures.py
--rw-r--r--   0        0        0     1992 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/default/typing_validator.py
--rw-r--r--   0        0        0     2346 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/git/__init__.py
--rw-r--r--   0        0        0     1551 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/torch/__init__.py
--rw-r--r--   0        0        0    15657 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/torch/distributions.py
--rw-r--r--   0        0        0      155 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/torch/lightning.py
--rw-r--r--   0        0        0      173 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/torch/math.py
--rw-r--r--   0        0        0     2550 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/torch/modules.py
--rw-r--r--   0        0        0     1420 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/torch/parameters.py
--rw-r--r--   0        0        0     1668 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/torch/tensor_creators.py
--rw-r--r--   0        0        0     2858 2023-07-20 20:08:12.299029 eztils-0.4.4/eztils/torch/to.py
--rw-r--r--   0        0        0     3624 2023-07-20 20:08:12.299029 eztils-0.4.4/pyproject.toml
--rw-r--r--   0        0        0    13903 1970-01-01 00:00:00.000000 eztils-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-22 01:06:32.317262 eztils-0.4.5/LICENSE
+-rw-r--r--   0        0        0    12741 2023-07-22 01:06:32.317262 eztils-0.4.5/README.md
+-rw-r--r--   0        0        0      542 2023-07-22 01:06:32.317262 eztils-0.4.5/eztils/__init__.py
+-rw-r--r--   0        0        0     2465 2023-07-22 01:06:32.317262 eztils-0.4.5/eztils/default/__init__.py
+-rw-r--r--   0        0        0     3689 2023-07-22 01:06:32.317262 eztils-0.4.5/eztils/default/dict_operations.py
+-rw-r--r--   0        0        0     2246 2023-07-22 01:06:32.321262 eztils-0.4.5/eztils/default/itertools.py
+-rw-r--r--   0        0        0     2458 2023-07-22 01:06:32.321262 eztils-0.4.5/eztils/default/logging.py
+-rw-r--r--   0        0        0     1412 2023-07-22 01:06:32.321262 eztils-0.4.5/eztils/default/math.py
+-rw-r--r--   0        0        0     1091 2023-07-22 01:06:32.321262 eztils-0.4.5/eztils/default/structures.py
+-rw-r--r--   0        0        0     2346 2023-07-22 01:06:32.321262 eztils-0.4.5/eztils/git/__init__.py
+-rw-r--r--   0        0        0     1607 2023-07-22 01:06:32.321262 eztils-0.4.5/eztils/torch/__init__.py
+-rw-r--r--   0        0        0    15657 2023-07-22 01:06:32.321262 eztils-0.4.5/eztils/torch/distributions.py
+-rw-r--r--   0        0        0      155 2023-07-22 01:06:32.321262 eztils-0.4.5/eztils/torch/lightning.py
+-rw-r--r--   0        0        0      173 2023-07-22 01:06:32.321262 eztils-0.4.5/eztils/torch/math.py
+-rw-r--r--   0        0        0     2550 2023-07-22 01:06:32.321262 eztils-0.4.5/eztils/torch/modules.py
+-rw-r--r--   0        0        0     1420 2023-07-22 01:06:32.321262 eztils-0.4.5/eztils/torch/parameters.py
+-rw-r--r--   0        0        0     1668 2023-07-22 01:06:32.321262 eztils-0.4.5/eztils/torch/tensor_creators.py
+-rw-r--r--   0        0        0     2858 2023-07-22 01:06:32.321262 eztils-0.4.5/eztils/torch/to.py
+-rw-r--r--   0        0        0     3624 2023-07-22 01:06:32.321262 eztils-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0    13903 1970-01-01 00:00:00.000000 eztils-0.4.5/PKG-INFO
```

### Comparing `eztils-0.4.4/LICENSE` & `eztils-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eztils-0.4.4/README.md` & `eztils-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `eztils-0.4.4/eztils/__init__.py` & `eztils-0.4.5/eztils/__init__.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.4/eztils/default/__init__.py` & `eztils-0.4.5/eztils/default/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import inspect as inspect_
 import os
 import sys
+from dataclasses import dataclass
 from inspect import getsourcefile, isfunction
 
 """
 miscellaneous functions that are often used
 """
 
 
@@ -68,13 +69,16 @@
 """
 # beartype
 from beartype import beartype
 from beartype.door import die_if_unbearable  # <-- like "assert isinstance(...)"
 from beartype.door import is_bearable  # <-------- like "isinstance(...)"
 from beartype.vale import Is
 
+enforced_dataclass = beartype(dataclass)
+frozen_enforced_dataclass = beartype(dataclass(frozen=True))
+
+
 from .dict_operations import *
 from .itertools import *
 from .logging import *
 from .math import *
 from .structures import *
-from .typing_validator import *
```

### Comparing `eztils-0.4.4/eztils/default/dict_operations.py` & `eztils-0.4.5/eztils/default/dict_operations.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.4/eztils/default/itertools.py` & `eztils-0.4.5/eztils/default/itertools.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.4/eztils/default/logging.py` & `eztils-0.4.5/eztils/default/logging.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.4/eztils/default/math.py` & `eztils-0.4.5/eztils/default/math.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.4/eztils/default/structures.py` & `eztils-0.4.5/eztils/default/structures.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.4/eztils/git/__init__.py` & `eztils-0.4.5/eztils/git/__init__.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.4/eztils/torch/__init__.py` & `eztils-0.4.5/eztils/torch/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 import random
 from pathlib import Path
 
 import numpy as np
 import torch
 from einops import rearrange as rea
 from einops import reduce
-from jaxtyping import Bool, Float, Float16, Float32, Int
+
+try:
+    from jaxtyping import Bool, Float, Float16, Float32, Int
+except RuntimeError:  # python < 3.9
+    pass
 from torch import einsum, nn, tensor
 from torch.nn import functional as F
 from torchvision.utils import save_image
 
 """
 globals
 """
```

### Comparing `eztils-0.4.4/eztils/torch/distributions.py` & `eztils-0.4.5/eztils/torch/distributions.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.4/eztils/torch/modules.py` & `eztils-0.4.5/eztils/torch/modules.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.4/eztils/torch/parameters.py` & `eztils-0.4.5/eztils/torch/parameters.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.4/eztils/torch/tensor_creators.py` & `eztils-0.4.5/eztils/torch/tensor_creators.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.4/eztils/torch/to.py` & `eztils-0.4.5/eztils/torch/to.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.4/pyproject.toml` & `eztils-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = ["ezhang7423 <ezhang7423@student.palomar.edu>"]
 description = "eds utilities"
 homepage = "https://github.com/ezhang7423/eztils"
 license = "MIT"
 name = "eztils"
 readme = "README.md"
 repository = "https://github.com/ezhang7423/eztils"
-version = "0.4.4"
+version = "0.4.5"
 
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
 keywords = [] #! Update me
 
 # Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [
   #! Update me
```

### Comparing `eztils-0.4.4/PKG-INFO` & `eztils-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eztils
-Version: 0.4.4
+Version: 0.4.5
 Summary: eds utilities
 Home-page: https://github.com/ezhang7423/eztils
 License: MIT
 Author: ezhang7423
 Author-email: ezhang7423@student.palomar.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

