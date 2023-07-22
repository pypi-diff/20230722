# Comparing `tmp/FJUtils-0.0.5.tar.gz` & `tmp/FJUtils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FJUtils-0.0.5.tar", last modified: Sat Jun 17 08:26:47 2023, max compression
+gzip compressed data, was "FJUtils-0.0.6.tar", last modified: Sat Jul 22 12:21:41 2023, max compression
```

## Comparing `FJUtils-0.0.5.tar` & `FJUtils-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-17 08:26:47.152570 FJUtils-0.0.5/
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-17 08:26:47.152570 FJUtils-0.0.5/FJUtils.egg-info/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-06-17 08:26:47.000000 FJUtils-0.0.5/FJUtils.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      313 2023-06-17 08:26:47.000000 FJUtils-0.0.5/FJUtils.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-06-17 08:26:47.000000 FJUtils-0.0.5/FJUtils.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      123 2023-06-17 08:26:47.000000 FJUtils-0.0.5/FJUtils.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-06-17 08:26:47.000000 FJUtils-0.0.5/FJUtils.egg-info/top_level.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-06-06 11:02:09.000000 FJUtils-0.0.5/LICENSE
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-06-17 08:26:47.152570 FJUtils-0.0.5/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2911 2023-06-06 11:02:09.000000 FJUtils-0.0.5/README.md
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-17 08:26:47.152570 FJUtils-0.0.5/fjutils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      708 2023-06-06 11:02:09.000000 FJUtils-0.0.5/fjutils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     8332 2023-06-17 08:26:17.000000 FJUtils-0.0.5/fjutils/checkpointing.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9932 2023-06-17 07:11:27.000000 FJUtils-0.0.5/fjutils/easylm.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1800 2023-06-06 11:02:09.000000 FJUtils-0.0.5/fjutils/load.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9494 2023-06-17 07:36:45.000000 FJUtils-0.0.5/fjutils/optimizers.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     7287 2023-06-17 07:27:33.000000 FJUtils-0.0.5/fjutils/utils.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      533 2023-06-06 11:02:09.000000 FJUtils-0.0.5/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-06-17 08:26:47.152570 FJUtils-0.0.5/setup.cfg
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1216 2023-06-17 08:26:40.000000 FJUtils-0.0.5/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-22 12:21:41.812266 FJUtils-0.0.6/
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-22 12:21:41.812266 FJUtils-0.0.6/FJUtils.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-07-22 12:21:41.000000 FJUtils-0.0.6/FJUtils.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      313 2023-07-22 12:21:41.000000 FJUtils-0.0.6/FJUtils.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-07-22 12:21:41.000000 FJUtils-0.0.6/FJUtils.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      123 2023-07-22 12:21:41.000000 FJUtils-0.0.6/FJUtils.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-07-22 12:21:41.000000 FJUtils-0.0.6/FJUtils.egg-info/top_level.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-06-06 11:02:09.000000 FJUtils-0.0.6/LICENSE
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-07-22 12:21:41.812266 FJUtils-0.0.6/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2911 2023-06-06 11:02:09.000000 FJUtils-0.0.6/README.md
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-22 12:21:41.812266 FJUtils-0.0.6/fjutils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      708 2023-06-06 11:02:09.000000 FJUtils-0.0.6/fjutils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8332 2023-06-17 08:26:17.000000 FJUtils-0.0.6/fjutils/checkpointing.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9956 2023-07-22 12:20:22.000000 FJUtils-0.0.6/fjutils/easylm.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1800 2023-06-06 11:02:09.000000 FJUtils-0.0.6/fjutils/load.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9724 2023-06-24 10:11:24.000000 FJUtils-0.0.6/fjutils/optimizers.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     7278 2023-07-22 12:19:47.000000 FJUtils-0.0.6/fjutils/utils.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      533 2023-06-06 11:02:09.000000 FJUtils-0.0.6/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-07-22 12:21:41.812266 FJUtils-0.0.6/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1216 2023-07-22 12:21:00.000000 FJUtils-0.0.6/setup.py
```

### Comparing `FJUtils-0.0.5/FJUtils.egg-info/PKG-INFO` & `FJUtils-0.0.6/FJUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FJUtils
-Version: 0.0.5
+Version: 0.0.6
 Summary: UNKNOWN
 Home-page: https://github.com/erfanzar/
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@yahoo.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FJUtils-0.0.5/LICENSE` & `FJUtils-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.5/PKG-INFO` & `FJUtils-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FJUtils
-Version: 0.0.5
+Version: 0.0.6
 Summary: UNKNOWN
 Home-page: https://github.com/erfanzar/
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@yahoo.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FJUtils-0.0.5/README.md` & `FJUtils-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.5/fjutils/__init__.py` & `FJUtils-0.0.6/fjutils/__init__.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.5/fjutils/checkpointing.py` & `FJUtils-0.0.6/fjutils/checkpointing.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.5/fjutils/easylm.py` & `FJUtils-0.0.6/fjutils/easylm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import jax
 import jax.numpy as jnp
 import re
-from jax.experimental.pjit import pjit, PartitionSpec as PS, with_sharding_constraint as _with_sharding_constraint
+from jax.experimental.pjit import pjit, with_sharding_constraint as _with_sharding_constraint
 import numpy as np
+from jax.sharding import PartitionSpec as PS
 from jax.experimental import mesh_utils
 from jax.interpreters import pxla
 import flax
 from functools import partial
 from jax.sharding import Mesh
```

### Comparing `FJUtils-0.0.5/fjutils/load.py` & `FJUtils-0.0.6/fjutils/load.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.5/fjutils/optimizers.py` & `FJUtils-0.0.6/fjutils/optimizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,20 +278,28 @@
         b1: Rate for combining the momentum and the current grad.
         b2: Decay rate for the exponentially weighted average of grads.
         mu_dtype: Optional `dtype` to be used for the momentum; if
           `None` then the `dtype is inferred from `params` and `updates`.
     Return:
         Optimizer , Scheduler
     """
-    scheduler = optax.cosine_decay_schedule(
-        init_value=learning_rate,
-        decay_steps=steps,
-        alpha=alpha,
-        exponent=exponent
-    )
+    try:
+        scheduler = optax.cosine_decay_schedule(
+            init_value=learning_rate,
+            decay_steps=steps,
+            alpha=alpha,
+            exponent=exponent
+        )
+    except:
+        scheduler = optax.cosine_decay_schedule(
+            init_value=learning_rate,
+            decay_steps=steps,
+            alpha=alpha,
+            # exponent=exponent
+        )
     tx = optax.chain(
         optax.scale_by_lion(
             b1=b1,
             b2=b2,
             mu_dtype=mu_dtype
         ),
         optax.scale_by_schedule(scheduler),
```

### Comparing `FJUtils-0.0.5/fjutils/utils.py` & `FJUtils-0.0.6/fjutils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import List, Optional, Callable, Any
 
 from fjutils.checkpointing import StreamingCheckpointer
 from jax import numpy as jnp
 import numpy as np
 import json
 import re
-from jax.experimental.pjit import PartitionSpec as PS
+from jax.sharding import PartitionSpec as PS
 import flax
 from jax.interpreters import pxla
 from fjutils.easylm import with_sharding_constraint
 from flax.serialization import from_bytes, to_bytes, to_state_dict
 from flax.traverse_util import flatten_dict
 from fjutils.easylm import float_tensor_to_dtype
```

### Comparing `FJUtils-0.0.5/pyproject.toml` & `FJUtils-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.5/setup.py` & `FJUtils-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="FJUtils",
-    version='0.0.5',
+    version='0.0.6',
     author="Erfan Zare Chavoshi",
     author_email="erfanzare82@yahoo.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/erfanzar/",
     packages=setuptools.find_packages(),
     install_requires=[
```

