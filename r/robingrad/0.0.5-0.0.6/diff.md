# Comparing `tmp/robingrad-0.0.5.tar.gz` & `tmp/robingrad-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robingrad-0.0.5.tar", last modified: Thu Jul 20 13:31:42 2023, max compression
+gzip compressed data, was "robingrad-0.0.6.tar", last modified: Sat Jul 22 12:47:57 2023, max compression
```

## Comparing `robingrad-0.0.5.tar` & `robingrad-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 13:31:42.201097 robingrad-0.0.5/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-07-11 17:52:34.000000 robingrad-0.0.5/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2950 2023-07-20 13:31:42.200420 robingrad-0.0.5/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1289 2023-07-20 13:31:13.000000 robingrad-0.0.5/README.md
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      694 2023-07-20 13:30:46.000000 robingrad-0.0.5/pyproject.toml
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 13:31:42.194384 robingrad-0.0.5/robingrad/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       78 2023-07-20 13:30:55.000000 robingrad-0.0.5/robingrad/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-07-12 20:52:44.000000 robingrad-0.0.5/robingrad/graph.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2267 2023-07-13 14:47:01.000000 robingrad-0.0.5/robingrad/lab.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 13:31:42.197286 robingrad-0.0.5/robingrad/nn/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      423 2023-07-13 16:36:34.000000 robingrad-0.0.5/robingrad/nn/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1564 2023-07-20 13:31:06.000000 robingrad-0.0.5/robingrad/optim.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1384 2023-07-15 12:31:49.000000 robingrad-0.0.5/robingrad/state.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10337 2023-07-17 14:12:32.000000 robingrad-0.0.5/robingrad/tensor.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 13:31:42.196792 robingrad-0.0.5/robingrad.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2950 2023-07-20 13:31:42.000000 robingrad-0.0.5/robingrad.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      358 2023-07-20 13:31:42.000000 robingrad-0.0.5/robingrad.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-07-20 13:31:42.000000 robingrad-0.0.5/robingrad.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       15 2023-07-20 13:31:42.000000 robingrad-0.0.5/robingrad.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       10 2023-07-20 13:31:42.000000 robingrad-0.0.5/robingrad.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-07-20 13:31:42.201269 robingrad-0.0.5/setup.cfg
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-20 13:31:42.198469 robingrad-0.0.5/tests/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4840 2023-07-13 15:05:49.000000 robingrad-0.0.5/tests/test_tensor.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-22 12:47:57.817217 robingrad-0.0.6/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-07-11 17:52:34.000000 robingrad-0.0.6/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2950 2023-07-22 12:47:57.816946 robingrad-0.0.6/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1289 2023-07-22 12:47:33.000000 robingrad-0.0.6/README.md
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      694 2023-07-22 12:47:24.000000 robingrad-0.0.6/pyproject.toml
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-22 12:47:57.814193 robingrad-0.0.6/robingrad/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       78 2023-07-22 12:47:28.000000 robingrad-0.0.6/robingrad/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-07-12 20:52:44.000000 robingrad-0.0.6/robingrad/graph.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3030 2023-07-22 10:30:14.000000 robingrad-0.0.6/robingrad/lab.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-22 12:47:57.816241 robingrad-0.0.6/robingrad/nn/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      423 2023-07-13 16:36:34.000000 robingrad-0.0.6/robingrad/nn/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1564 2023-07-20 13:31:06.000000 robingrad-0.0.6/robingrad/optim.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1384 2023-07-15 12:31:49.000000 robingrad-0.0.6/robingrad/state.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11131 2023-07-22 10:23:56.000000 robingrad-0.0.6/robingrad/tensor.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-22 12:47:57.815930 robingrad-0.0.6/robingrad.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2950 2023-07-22 12:47:57.000000 robingrad-0.0.6/robingrad.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      358 2023-07-22 12:47:57.000000 robingrad-0.0.6/robingrad.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-07-22 12:47:57.000000 robingrad-0.0.6/robingrad.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       15 2023-07-22 12:47:57.000000 robingrad-0.0.6/robingrad.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       10 2023-07-22 12:47:57.000000 robingrad-0.0.6/robingrad.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-07-22 12:47:57.817295 robingrad-0.0.6/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-22 12:47:57.816537 robingrad-0.0.6/tests/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     6291 2023-07-22 10:35:08.000000 robingrad-0.0.6/tests/test_tensor.py
```

### Comparing `robingrad-0.0.5/LICENSE` & `robingrad-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.5/PKG-INFO` & `robingrad-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robingrad
-Version: 0.0.5
+Version: 0.0.6
 Summary: Something between Tinygrad and Micrograd
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2023 Marco Salvalaggio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -32,15 +32,15 @@
 
 
 ## Installation
 
 To install the current release,
 
 ```console
-pip install robingrad==0.0.5
+pip install robingrad==0.0.6
 ```
 
 From source
 
 ```console
 git clone https://github.com/marcosalvalaggio/robingrad.git
 cd robingrad
```

### Comparing `robingrad-0.0.5/README.md` & `robingrad-0.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 ## Installation
 
 To install the current release,
 
 ```console
-pip install robingrad==0.0.5
+pip install robingrad==0.0.6
 ```
 
 From source
 
 ```console
 git clone https://github.com/marcosalvalaggio/robingrad.git
 cd robingrad
```

### Comparing `robingrad-0.0.5/pyproject.toml` & `robingrad-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "robingrad"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Something between Tinygrad and Micrograd"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `robingrad-0.0.5/robingrad/graph.py` & `robingrad-0.0.6/robingrad/graph.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.5/robingrad/lab.py` & `robingrad-0.0.6/robingrad/lab.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,27 +70,56 @@
 # b = torch.full((3,2), 3., requires_grad=True)
 # c = aa @ b
 # loss = c.sum()
 # loss.backward()
 # print(a.grad)
 # print(b.grad)
 
+# a = Tensor.eye(3, requires_grad=True)
+# b = Tensor.full((3,3), 3., requires_grad=True)
+# c = a @ b
+# d = c.mean(axis=0, keepdim=True)
+# e = Tensor.full((1,3), 4., requires_grad=True)
+# f = d * e
+# loss = f.sum()
+# loss.backward()
+# res_robin_1 = a.grad.tolist()
+# print(res_robin_1)
+# # torch 
+# a = torch.eye(3, requires_grad=True)
+# b = torch.full((3,3), 3., requires_grad=True)
+# c = a @ b
+# d = c.mean(axis=0, keepdim=True)
+# e = torch.full((1,3), 4., requires_grad=True)
+# f = d * e
+# loss = f.sum()
+# loss.backward()
+# res_torch_1 = a.grad.numpy().tolist()
+# print(res_torch_1)
 
-a = Tensor.ones((3,2), requires_grad=True)
-b = a.T
-c = Tensor.full((3,2), 3., requires_grad=True)
-d = b @ c
-loss = d.sum()
-loss.backward()
-draw_dot(loss, filename="img/graph_inspect", inspect=True)
-print(a.grad)
-print(c.grad)
-
-a = torch.ones((3,2), requires_grad=True)
-b = torch.transpose(a,1,0)
-c = torch.full((3,2), 3., requires_grad=True)
-d = b @ c
-loss = d.sum()
-loss.backward()
-print(a.grad)
-print(c.grad)
+a = Tensor.full((5,1), 3., requires_grad=True)
+b = Tensor.full((1,1), 2., requires_grad=True)
+c = a + b
+loss = c.mean()
+try:
+    loss.backward()
+    print(loss.grad)
+    print(c.grad)
+    print(a.grad)
+    print(b.grad)
+    draw_dot(loss, filename="img/graph_inspect", inspect=True)
+except Exception as e:
+    print(e)
 
+print("\n")
+print("- TORCH -")
+a = torch.full((5,1), 3., requires_grad=True)
+b = torch.full((1,1), 2., requires_grad=True)
+c = a + b
+loss = c.mean()
+try:
+    loss.backward()
+    print("torch win")
+    print(a.grad)
+    print(b.grad)
+except Exception as e:
+    print(e)
```

### Comparing `robingrad-0.0.5/robingrad/optim.py` & `robingrad-0.0.6/robingrad/optim.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.5/robingrad/state.py` & `robingrad-0.0.6/robingrad/state.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.5/robingrad/tensor.py` & `robingrad-0.0.6/robingrad/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,31 @@
         
         def _backward():
             self.grad += np.ones_like(self.data) * out.grad
         out._backward = _backward
         
         return out
     
+    def mean(self, axis=None, keepdim: bool = False) -> "Tensor":
+        if axis is None:
+            data = self.data.mean()
+        else:
+            data = self.data.mean(axis=axis, keepdims=keepdim)
+        out = Tensor(data, dtype=self.data.dtype, _children=(self,), _op="μ", _origin="mean", requires_grad=self.requires_grad)
+    
+        def _backward():
+            if axis is None:
+                self.grad += np.ones_like(self.data) * out.grad / self.data.size
+            else:
+                axis_sum_size = self.data.shape[axis] if keepdim else 1
+                self.grad += np.ones_like(self.data) * out.grad / axis_sum_size
+        out._backward = _backward
+
+        return out
+
     def relu(self) -> "Tensor":
         out = Tensor(np.maximum(0, self.data), dtype=self.data.dtype, _children=(self,), _op="relu()", _origin="ReLU", requires_grad=self.requires_grad)
 
         def _backward():
             self.grad += (out.data > 0) * out.grad
         out._backward = _backward
 
@@ -115,15 +132,16 @@
     
     def __add__(self, other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor":
         other = other if isinstance(other, Tensor) else Tensor.broadcast(self, other, dtype=self.data.dtype, requires_grad=self.requires_grad)
         out = Tensor(self.data + other.data, dtype=self.data.dtype, _children=(self, other), _op='+', _origin="__add__", requires_grad=self.requires_grad)
         
         def _backward():
             self.grad += out.grad
-            other.grad += out.grad
+            # other.grad += out.grad
+            other.grad += np.sum(out.grad, axis=0) if len(other.data.shape) > 1 else out.grad
         out._backward = _backward
 
         return out
     
     def __mul__(self, other: Union["Tensor", np.ndarray, List, int, float]) -> "Tensor":
         other = other if isinstance(other, Tensor) else Tensor.broadcast(self, other, dtype=self.data.dtype, requires_grad=self.requires_grad)
         out = Tensor(self.data * other.data, dtype=self.data.dtype, _children=(self, other), _op='*', _origin="__mul__", requires_grad=self.requires_grad)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `robingrad-0.0.5/robingrad.egg-info/PKG-INFO` & `robingrad-0.0.6/robingrad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robingrad
-Version: 0.0.5
+Version: 0.0.6
 Summary: Something between Tinygrad and Micrograd
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2023 Marco Salvalaggio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -32,15 +32,15 @@
 
 
 ## Installation
 
 To install the current release,
 
 ```console
-pip install robingrad==0.0.5
+pip install robingrad==0.0.6
 ```
 
 From source
 
 ```console
 git clone https://github.com/marcosalvalaggio/robingrad.git
 cd robingrad
```

### Comparing `robingrad-0.0.5/tests/test_tensor.py` & `robingrad-0.0.6/tests/test_tensor.py`

 * *Files 11% similar despite different names*

```diff
@@ -147,11 +147,55 @@
         loss.backward()
         res_torch_1 = a.grad.numpy().tolist()
         res_torch_2 = c.grad.numpy().tolist()
         #test
         self.assertEqual(res_robin_1, res_torch_1)
         self.assertEqual(res_robin_2, res_torch_2)
 
+    def test_mean(self):
+        # robin
+        a = Tensor.eye(3, requires_grad=True)
+        b = Tensor.full((3,3), 3., requires_grad=True)
+        c = a @ b
+        d = c.mean(axis=0, keepdim=True)
+        e = Tensor.full((1,3), 4., requires_grad=True)
+        f = d * e
+        loss = f.sum()
+        loss.backward()
+        res_robin_1 = a.grad.tolist()
+        # torch 
+        a = torch.eye(3, requires_grad=True)
+        b = torch.full((3,3), 3., requires_grad=True)
+        c = a @ b
+        d = c.mean(axis=0, keepdim=True)
+        e = torch.full((1,3), 4., requires_grad=True)
+        f = d * e
+        loss = f.sum()
+        loss.backward()
+        res_torch_1 = a.grad.numpy().tolist()
+        # test 
+        self.assertAlmostEqual(res_robin_1, res_torch_1)
+
+    def test_new_add(self):
+        # robin
+        a = Tensor.full((5,1), 3., requires_grad=True)
+        b = Tensor.full((1,1), 2., requires_grad=True)
+        c = a + b
+        loss = c.mean()
+        loss.backward()
+        res_robin_1 = a.grad.tolist()
+        res_robin_2 = b.grad.tolist()
+        # torch
+        a = torch.full((5,1), 3., requires_grad=True)
+        b = torch.full((1,1), 2., requires_grad=True)
+        c = a + b
+        loss = c.mean()
+        loss.backward()
+        res_torch_1 = a.grad.tolist()
+        res_torch_2 = b.grad.tolist()
+        #test
+        self.assertEqual(res_robin_1, res_torch_1)
+        self.assertEqual(res_robin_2, res_torch_2)
```

