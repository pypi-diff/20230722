# Comparing `tmp/equiformer-pytorch-0.3.1.tar.gz` & `tmp/equiformer-pytorch-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equiformer-pytorch-0.3.1.tar", last modified: Wed Jul 12 18:17:21 2023, max compression
+gzip compressed data, was "equiformer-pytorch-0.3.2.tar", last modified: Sat Jul 22 00:15:42 2023, max compression
```

## Comparing `equiformer-pytorch-0.3.1.tar` & `equiformer-pytorch-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:17:21.590266 equiformer-pytorch-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-12 18:17:21.590266 equiformer-pytorch-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:17:21.518267 equiformer-pytorch-0.3.1/equiformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/equiformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/equiformer_pytorch/basis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:17:21.518267 equiformer-pytorch-0.3.1/equiformer_pytorch/data/
--rw-r--r--   0 runner    (1001) docker     (123) 36766718 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/equiformer_pytorch/data/J_dense.pt
--rw-r--r--   0 runner    (1001) docker     (123)    35782 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/equiformer_pytorch/equiformer_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/equiformer_pytorch/irr_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/equiformer_pytorch/reversible.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/equiformer_pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/equiformer_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:17:21.518267 equiformer-pytorch-0.3.1/equiformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-12 18:17:21.000000 equiformer-pytorch-0.3.1/equiformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-12 18:17:21.000000 equiformer-pytorch-0.3.1/equiformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:17:21.000000 equiformer-pytorch-0.3.1/equiformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 18:17:21.000000 equiformer-pytorch-0.3.1/equiformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 18:17:21.000000 equiformer-pytorch-0.3.1/equiformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 18:17:21.590266 equiformer-pytorch-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-12 18:15:33.000000 equiformer-pytorch-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:15:42.654640 equiformer-pytorch-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-22 00:13:39.000000 equiformer-pytorch-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-22 00:13:39.000000 equiformer-pytorch-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-22 00:15:42.654640 equiformer-pytorch-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-07-22 00:13:39.000000 equiformer-pytorch-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:15:42.530631 equiformer-pytorch-0.3.2/equiformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-22 00:13:39.000000 equiformer-pytorch-0.3.2/equiformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-07-22 00:13:39.000000 equiformer-pytorch-0.3.2/equiformer_pytorch/basis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:15:42.530631 equiformer-pytorch-0.3.2/equiformer_pytorch/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 36766718 2023-07-22 00:13:39.000000 equiformer-pytorch-0.3.2/equiformer_pytorch/data/J_dense.pt
+-rw-r--r--   0 runner    (1001) docker     (123)    35782 2023-07-22 00:13:39.000000 equiformer-pytorch-0.3.2/equiformer_pytorch/equiformer_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-22 00:13:39.000000 equiformer-pytorch-0.3.2/equiformer_pytorch/irr_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-07-22 00:13:39.000000 equiformer-pytorch-0.3.2/equiformer_pytorch/reversible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-22 00:13:39.000000 equiformer-pytorch-0.3.2/equiformer_pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 00:13:39.000000 equiformer-pytorch-0.3.2/equiformer_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 00:15:42.530631 equiformer-pytorch-0.3.2/equiformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-22 00:15:42.000000 equiformer-pytorch-0.3.2/equiformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-22 00:15:42.000000 equiformer-pytorch-0.3.2/equiformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 00:15:42.000000 equiformer-pytorch-0.3.2/equiformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-22 00:15:42.000000 equiformer-pytorch-0.3.2/equiformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-22 00:15:42.000000 equiformer-pytorch-0.3.2/equiformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-22 00:15:42.658640 equiformer-pytorch-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-22 00:13:39.000000 equiformer-pytorch-0.3.2/setup.py
```

### Comparing `equiformer-pytorch-0.3.1/LICENSE` & `equiformer-pytorch-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `equiformer-pytorch-0.3.1/PKG-INFO` & `equiformer-pytorch-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equiformer-pytorch
-Version: 0.3.1
+Version: 0.3.2
 Summary: Equiformer - SE3/E3 Graph Attention Transformer for Molecules and Proteins
 Home-page: https://github.com/lucidrains/equiformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,equivariance,molecules,proteins
 Classifier: Development Status :: 4 - Beta
```

### Comparing `equiformer-pytorch-0.3.1/README.md` & `equiformer-pytorch-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `equiformer-pytorch-0.3.1/equiformer_pytorch/basis.py` & `equiformer-pytorch-0.3.2/equiformer_pytorch/basis.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
         basis[f'({d_in},{d_out})'] = K_Js # (mi, mf)
 
     return basis
 
 # functions for rotating r_ij to z-axis
 
-def rot_x_to_y_direction(x, y):
+def rot_x_to_y_direction(x, y, eps = 1e-6):
     '''
     Rotates a vector x to the same direction as vector y
     Taken from https://math.stackexchange.com/a/2672702
     This formulation, although not the shortest path, has the benefit of rotation matrix being symmetric; rotating back to x upon two rotations
     '''
     n, dtype, device = x.shape[-1], x.dtype, x.device
 
@@ -173,15 +173,15 @@
     x, y = x.double(), y.double()
 
     x, y = map(l2norm, (x, y))
 
     xy = rearrange(x + y, '... n -> ... n 1')
     xy_t = rearrange(xy, '... n 1 -> ... 1 n')
 
-    R = 2 * (xy @ xy_t) / (xy_t @ xy) - I
+    R = 2 * (xy @ xy_t) / (xy_t @ xy).clamp(min = eps) - I
     return R.type(dtype)
 
 @torch.no_grad()
 def get_D_to_from_z_axis(r_ij, max_degree):
     device, dtype = r_ij.device, r_ij.dtype
 
     D = dict()
```

### Comparing `equiformer-pytorch-0.3.1/equiformer_pytorch/data/J_dense.pt` & `equiformer-pytorch-0.3.2/equiformer_pytorch/data/J_dense.pt`

 * *Files identical despite different names*

### Comparing `equiformer-pytorch-0.3.1/equiformer_pytorch/equiformer_pytorch.py` & `equiformer-pytorch-0.3.2/equiformer_pytorch/equiformer_pytorch.py`

 * *Files identical despite different names*

### Comparing `equiformer-pytorch-0.3.1/equiformer_pytorch/irr_repr.py` & `equiformer-pytorch-0.3.2/equiformer_pytorch/irr_repr.py`

 * *Files identical despite different names*

### Comparing `equiformer-pytorch-0.3.1/equiformer_pytorch/reversible.py` & `equiformer-pytorch-0.3.2/equiformer_pytorch/reversible.py`

 * *Files identical despite different names*

### Comparing `equiformer-pytorch-0.3.1/equiformer_pytorch/utils.py` & `equiformer-pytorch-0.3.2/equiformer_pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `equiformer-pytorch-0.3.1/equiformer_pytorch.egg-info/PKG-INFO` & `equiformer-pytorch-0.3.2/equiformer_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equiformer-pytorch
-Version: 0.3.1
+Version: 0.3.2
 Summary: Equiformer - SE3/E3 Graph Attention Transformer for Molecules and Proteins
 Home-page: https://github.com/lucidrains/equiformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,equivariance,molecules,proteins
 Classifier: Development Status :: 4 - Beta
```

### Comparing `equiformer-pytorch-0.3.1/equiformer_pytorch.egg-info/SOURCES.txt` & `equiformer-pytorch-0.3.2/equiformer_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `equiformer-pytorch-0.3.1/setup.py` & `equiformer-pytorch-0.3.2/setup.py`

 * *Files identical despite different names*

