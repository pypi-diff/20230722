# Comparing `tmp/bayesianbandits-0.4.4.tar.gz` & `tmp/bayesianbandits-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesianbandits-0.4.4.tar", max compression
+gzip compressed data, was "bayesianbandits-0.4.5.tar", max compression
```

## Comparing `bayesianbandits-0.4.4.tar` & `bayesianbandits-0.4.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-07-06 00:14:50.505508 bayesianbandits-0.4.4/LICENSE
--rw-r--r--   0        0        0     1093 2023-07-06 00:14:50.505508 bayesianbandits-0.4.4/README.md
--rw-r--r--   0        0        0     2991 2023-07-06 00:14:50.505508 bayesianbandits-0.4.4/bayesianbandits/__init__.py
--rw-r--r--   0        0        0     3774 2023-07-06 00:14:50.505508 bayesianbandits-0.4.4/bayesianbandits/_arm.py
--rw-r--r--   0        0        0    23085 2023-07-06 00:14:50.505508 bayesianbandits-0.4.4/bayesianbandits/_basebandit.py
--rw-r--r--   0        0        0    29847 2023-07-06 00:14:50.505508 bayesianbandits-0.4.4/bayesianbandits/_estimators.py
--rw-r--r--   0        0        0     1304 2023-07-06 00:14:50.505508 bayesianbandits-0.4.4/bayesianbandits/_np_utils.py
--rw-r--r--   0        0        0     5036 2023-07-06 00:14:50.505508 bayesianbandits-0.4.4/bayesianbandits/_policy_decorators.py
--rw-r--r--   0        0        0     2634 2023-07-06 00:14:50.505508 bayesianbandits-0.4.4/bayesianbandits/_typing.py
--rw-r--r--   0        0        0      765 2023-07-06 00:14:50.509508 bayesianbandits-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 bayesianbandits-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-22 01:21:51.309334 bayesianbandits-0.4.5/LICENSE
+-rw-r--r--   0        0        0     1093 2023-07-22 01:21:51.309334 bayesianbandits-0.4.5/README.md
+-rw-r--r--   0        0        0     2991 2023-07-22 01:21:51.309334 bayesianbandits-0.4.5/bayesianbandits/__init__.py
+-rw-r--r--   0        0        0     4046 2023-07-22 01:21:51.309334 bayesianbandits-0.4.5/bayesianbandits/_arm.py
+-rw-r--r--   0        0        0    23085 2023-07-22 01:21:51.309334 bayesianbandits-0.4.5/bayesianbandits/_basebandit.py
+-rw-r--r--   0        0        0    29847 2023-07-22 01:21:51.309334 bayesianbandits-0.4.5/bayesianbandits/_estimators.py
+-rw-r--r--   0        0        0     1304 2023-07-22 01:21:51.309334 bayesianbandits-0.4.5/bayesianbandits/_np_utils.py
+-rw-r--r--   0        0        0     5036 2023-07-22 01:21:51.309334 bayesianbandits-0.4.5/bayesianbandits/_policy_decorators.py
+-rw-r--r--   0        0        0     2634 2023-07-22 01:21:51.309334 bayesianbandits-0.4.5/bayesianbandits/_typing.py
+-rw-r--r--   0        0        0      765 2023-07-22 01:21:51.313335 bayesianbandits-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 bayesianbandits-0.4.5/PKG-INFO
```

### Comparing `bayesianbandits-0.4.4/LICENSE` & `bayesianbandits-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.4/README.md` & `bayesianbandits-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.4/bayesianbandits/__init__.py` & `bayesianbandits-0.4.5/bayesianbandits/__init__.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.4/bayesianbandits/_arm.py` & `bayesianbandits-0.4.5/bayesianbandits/_arm.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,27 +26,33 @@
         if self.learner is None:
             raise ValueError("Learner is not set.")
         return func(self, *args, **kwargs)
 
     return wrapper
 
 
+def identity(
+    x: Union[np.float_, NDArray[np.float_]]
+) -> Union[np.float_, NDArray[np.float_]]:
+    return x
+
+
 class Arm:
     """Arm of a bandit.
 
     Parameters
     ----------
     action_token : Any
         Token to return when the arm is pulled. This should be something processed
         by the user's code to execute the action associated with the arm.
-    reward_function : RewardFunction
+    reward_function : Optional[RewardFunction], default=None
         Function to call to compute the reward. Takes the output of the learner's
         `sample` function as input and should return a scalar reward. Should take
         a single scalar or array-like argument and return a scalar or
-        1D array.
+        1D array. If None, the identity function is used.
     learner : Optional[Learner], default=None
         Learner to use for the arm. If None, the arm cannot be used.
 
     Examples
     --------
     >>> from bayesianbandits import Arm
     >>> import numpy as np
@@ -65,18 +71,20 @@
     >>> arm.update(np.array([[1]]), np.array([1]))
 
     """
 
     def __init__(
         self,
         action_token: Any,
-        reward_function: RewardFunction,
+        reward_function: Optional[RewardFunction] = None,
         learner: Optional[Learner] = None,
     ) -> None:
         self.action_token = ActionToken(action_token)
+        if reward_function is None:
+            reward_function = identity
         self.reward_function = reward_function
         self.learner = learner
 
     @requires_learner
     def pull(self) -> ActionToken:
         """Pull the arm."""
         return self.action_token
```

### Comparing `bayesianbandits-0.4.4/bayesianbandits/_basebandit.py` & `bayesianbandits-0.4.5/bayesianbandits/_basebandit.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.4/bayesianbandits/_estimators.py` & `bayesianbandits-0.4.5/bayesianbandits/_estimators.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.4/bayesianbandits/_np_utils.py` & `bayesianbandits-0.4.5/bayesianbandits/_np_utils.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.4/bayesianbandits/_policy_decorators.py` & `bayesianbandits-0.4.5/bayesianbandits/_policy_decorators.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.4/bayesianbandits/_typing.py` & `bayesianbandits-0.4.5/bayesianbandits/_typing.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.4/pyproject.toml` & `bayesianbandits-0.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bayesianbandits"
-version = "0.4.4"
+version = "0.4.5"
 description = "A Pythonic microframework for Multi-Armed Bandit algorithms."
 authors = ["Rishi Kulkarni <rishi@kulkarni.science>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9, <3.12"
 scipy = "^1.10.0"
```

### Comparing `bayesianbandits-0.4.4/PKG-INFO` & `bayesianbandits-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayesianbandits
-Version: 0.4.4
+Version: 0.4.5
 Summary: A Pythonic microframework for Multi-Armed Bandit algorithms.
 Author: Rishi Kulkarni
 Author-email: rishi@kulkarni.science
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

