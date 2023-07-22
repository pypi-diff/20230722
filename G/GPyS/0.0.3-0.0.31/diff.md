# Comparing `tmp/GPyS-0.0.3.tar.gz` & `tmp/GPyS-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPyS-0.0.3.tar", last modified: Mon Jul 17 18:50:18 2023, max compression
+gzip compressed data, was "GPyS-0.0.31.tar", last modified: Sat Jul 22 19:12:19 2023, max compression
```

## Comparing `GPyS-0.0.3.tar` & `GPyS-0.0.31.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 18:50:18.671534 GPyS-0.0.3/
--rw-rw-rw-   0        0        0    34727 2023-07-17 03:05:27.000000 GPyS-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1782 2023-07-17 18:50:18.670534 GPyS-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1352 2023-07-17 17:17:44.000000 GPyS-0.0.3/README.md
--rw-rw-rw-   0        0        0      588 2023-07-17 18:49:58.000000 GPyS-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-17 18:50:18.671534 GPyS-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-17 18:50:18.655534 GPyS-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 18:50:18.660534 GPyS-0.0.3/src/GPyS.egg-info/
--rw-rw-rw-   0        0        0     1782 2023-07-17 18:50:18.000000 GPyS-0.0.3/src/GPyS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-07-17 18:50:18.000000 GPyS-0.0.3/src/GPyS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 18:50:18.000000 GPyS-0.0.3/src/GPyS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-07-17 18:50:18.000000 GPyS-0.0.3/src/GPyS.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-17 18:50:18.663534 GPyS-0.0.3/src/GPyS_LOOCV_error/
--rw-rw-rw-   0        0        0     9311 2023-07-17 17:57:19.000000 GPyS-0.0.3/src/GPyS_LOOCV_error/GPyS_LOOCV_error.py
--rw-rw-rw-   0        0        0       35 2023-07-17 17:39:29.000000 GPyS-0.0.3/src/GPyS_LOOCV_error/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 18:50:18.666534 GPyS-0.0.3/src/GPyS_prediction/
--rw-rw-rw-   0        0        0    16517 2023-07-17 17:57:59.000000 GPyS-0.0.3/src/GPyS_prediction/GPyS_prediction.py
--rw-rw-rw-   0        0        0       41 2023-07-17 03:05:27.000000 GPyS-0.0.3/src/GPyS_prediction/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 18:50:18.668534 GPyS-0.0.3/src/GPyS_preprocessor/
--rw-rw-rw-   0        0        0     2084 2023-07-17 03:05:27.000000 GPyS-0.0.3/src/GPyS_preprocessor/GPyS_preprocessor.py
--rw-rw-rw-   0        0        0       45 2023-07-17 03:05:27.000000 GPyS-0.0.3/src/GPyS_preprocessor/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-17 03:05:27.000000 GPyS-0.0.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 19:12:19.232463 GPyS-0.0.31/
+-rw-rw-rw-   0        0        0    34727 2023-07-20 16:07:58.000000 GPyS-0.0.31/LICENSE
+-rw-rw-rw-   0        0        0     1891 2023-07-22 19:12:19.230409 GPyS-0.0.31/PKG-INFO
+-rw-rw-rw-   0        0        0     1369 2023-07-20 16:07:58.000000 GPyS-0.0.31/README.md
+-rw-rw-rw-   0        0        0      659 2023-07-22 19:11:59.000000 GPyS-0.0.31/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-22 19:12:19.233445 GPyS-0.0.31/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-22 19:12:19.169981 GPyS-0.0.31/src/
+drwxrwxrwx   0        0        0        0 2023-07-22 19:12:19.190403 GPyS-0.0.31/src/GPyS.egg-info/
+-rw-rw-rw-   0        0        0     1891 2023-07-22 19:12:19.000000 GPyS-0.0.31/src/GPyS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-07-22 19:12:19.000000 GPyS-0.0.31/src/GPyS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 19:12:19.000000 GPyS-0.0.31/src/GPyS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-07-22 19:12:19.000000 GPyS-0.0.31/src/GPyS.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 19:12:19.200454 GPyS-0.0.31/src/GPyS_LOOCV_error/
+-rw-rw-rw-   0        0        0     9401 2023-07-22 18:45:07.000000 GPyS-0.0.31/src/GPyS_LOOCV_error/GPyS_LOOCV_error.py
+-rw-rw-rw-   0        0        0       35 2023-07-20 16:07:58.000000 GPyS-0.0.31/src/GPyS_LOOCV_error/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 19:12:19.212442 GPyS-0.0.31/src/GPyS_prediction/
+-rw-rw-rw-   0        0        0    20191 2023-07-22 00:10:49.000000 GPyS-0.0.31/src/GPyS_prediction/GPyS_prediction.py
+-rw-rw-rw-   0        0        0       41 2023-07-20 16:07:58.000000 GPyS-0.0.31/src/GPyS_prediction/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 19:12:19.223455 GPyS-0.0.31/src/GPyS_preprocessor/
+-rw-rw-rw-   0        0        0     2918 2023-07-22 15:57:37.000000 GPyS-0.0.31/src/GPyS_preprocessor/GPyS_preprocessor.py
+-rw-rw-rw-   0        0        0       45 2023-07-20 16:07:58.000000 GPyS-0.0.31/src/GPyS_preprocessor/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-20 16:07:58.000000 GPyS-0.0.31/src/__init__.py
```

### Comparing `GPyS-0.0.3/LICENSE` & `GPyS-0.0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `GPyS-0.0.3/PKG-INFO` & `GPyS-0.0.31/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: GPyS
-Version: 0.0.3
+Version: 0.0.31
 Summary: Gaussian Process Subspace Prediction
-Author-email: Taiwo Adebiyi <taadebi2@cougarnet.uh.edu>
+Author-email: "ZHANG, Ruda" <rudaz@Central.UH.EDU>, Taiwo Adebiyi <taadebi2@cougarnet.uh.edu>
+Project-URL: Homepage, https://github.com/UQUH/GPyS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -26,18 +27,18 @@
 ## Example Use 
 
 After installing the package you can load it via: 
 
 #### For GPS Preprocessor: 
   - from GPyS_preprocessor import Preprocessor
   - Note that only Preprocessor.setup(X) takes in argument X and this must be called first before any other functions
-  - The remaining functions merely returns preprocessing quantities of interests
+  - The remaining functions merely return preprocessing quantities of interests
 
 #### For GPS Hyperparameter training:
 - from GPyS_LOOCV_error import LOOCV
 - Utilize hSSDist(length) method for the objective function computation at a given (default) length scale
-- Refer to the working script to see an example computation of optimal lengthscale for GPS. 
+- Please take a look at the LOOCV_script.py to see an example computation of optimal lengthscale for GPS. 
 
 #### For GPS Prediction: 
   - from GPyS_prediction import Prediction
   - All the functions can be independently called here. 
-  - Also, user can directly call Prediction.GPS_Prediction() to immediately obtain prediction results
+  - Also, the user can directly call Prediction.GPS_Prediction() to immediately obtain prediction results
```

### Comparing `GPyS-0.0.3/README.md` & `GPyS-0.0.31/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 ## Example Use 
 
 After installing the package you can load it via: 
 
 #### For GPS Preprocessor: 
   - from GPyS_preprocessor import Preprocessor
   - Note that only Preprocessor.setup(X) takes in argument X and this must be called first before any other functions
-  - The remaining functions merely returns preprocessing quantities of interests
+  - The remaining functions merely return preprocessing quantities of interests
 
 #### For GPS Hyperparameter training:
 - from GPyS_LOOCV_error import LOOCV
 - Utilize hSSDist(length) method for the objective function computation at a given (default) length scale
-- Refer to the working script to see an example computation of optimal lengthscale for GPS. 
+- Please take a look at the LOOCV_script.py to see an example computation of optimal lengthscale for GPS. 
 
 #### For GPS Prediction: 
   - from GPyS_prediction import Prediction
   - All the functions can be independently called here. 
-  - Also, user can directly call Prediction.GPS_Prediction() to immediately obtain prediction results
+  - Also, the user can directly call Prediction.GPS_Prediction() to immediately obtain prediction results
```

### Comparing `GPyS-0.0.3/src/GPyS.egg-info/PKG-INFO` & `GPyS-0.0.31/src/GPyS.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: GPyS
-Version: 0.0.3
+Version: 0.0.31
 Summary: Gaussian Process Subspace Prediction
-Author-email: Taiwo Adebiyi <taadebi2@cougarnet.uh.edu>
+Author-email: "ZHANG, Ruda" <rudaz@Central.UH.EDU>, Taiwo Adebiyi <taadebi2@cougarnet.uh.edu>
+Project-URL: Homepage, https://github.com/UQUH/GPyS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -26,18 +27,18 @@
 ## Example Use 
 
 After installing the package you can load it via: 
 
 #### For GPS Preprocessor: 
   - from GPyS_preprocessor import Preprocessor
   - Note that only Preprocessor.setup(X) takes in argument X and this must be called first before any other functions
-  - The remaining functions merely returns preprocessing quantities of interests
+  - The remaining functions merely return preprocessing quantities of interests
 
 #### For GPS Hyperparameter training:
 - from GPyS_LOOCV_error import LOOCV
 - Utilize hSSDist(length) method for the objective function computation at a given (default) length scale
-- Refer to the working script to see an example computation of optimal lengthscale for GPS. 
+- Please take a look at the LOOCV_script.py to see an example computation of optimal lengthscale for GPS. 
 
 #### For GPS Prediction: 
   - from GPyS_prediction import Prediction
   - All the functions can be independently called here. 
-  - Also, user can directly call Prediction.GPS_Prediction() to immediately obtain prediction results
+  - Also, the user can directly call Prediction.GPS_Prediction() to immediately obtain prediction results
```

### Comparing `GPyS-0.0.3/src/GPyS_LOOCV_error/GPyS_LOOCV_error.py` & `GPyS-0.0.31/src/GPyS_LOOCV_error/GPyS_LOOCV_error.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,122 +3,115 @@
 from GPyS_preprocessor import Preprocessor
 from GPyS_prediction import Prediction as Pred
 
 
 import numpy as np
 import scipy
 import scipy.linalg as la
+from typing import TypeAlias, Union, Optional
 
 
+vector: TypeAlias = list[float]
+matrix: TypeAlias = list[vector]
+
 class LOOCV():
+    """
+    =============================================================
+    leave-one-out cross validation (LOOCV)
+    =============================================================
+
+    Setting the hyperparameters by minimizing the LOOCV predictive error (sum of squared errors)
+    as a means to optimize a certain criterion.
+
+    For GPS, the LOOCV error are measured in Riemannian distances.
+
+    The hSSDist() is the core function in the LOOCV package for criterion optimization.
+
+    Other important functions includes:
+    --> PrAngles() for computing the principal angles between two subspaces
+    --> RiemannianDist() for computing the Riemannian distance between two subspaces: 2-norm of principal angles
+    --> LOOPredEvd() for computing the LOO prediction: EVD version
+    --> LOODistEVD() for computing the LOO Riemannian distances: EVD version
+    --> default_length() for computing the rule of thumb length scale
+
+
+    """
 
-    def __init__(self, X, sample, beta):
+    def __init__(self, X: matrix, sample: matrix, beta: Union[int, float]) -> None:
         """
-        :param X ([[float]]): Concatenated orthonormal bases
-        :param sample ([[float]]): vector of scalar parameters, or matrix of vector parameters
-        :param length_scale ([float]): length-scale of correlation, isotropic (scaler)
+        :param X: Concatenated orthonormal bases (matrix of size n by kl)*
+        :param sample : vector of scalar parameters, or matrix of vector parameters
+        :param beta: length-scale of correlation, isotropic (scaler)
                                         or separable (vector)
+
+        * n: ambient dimension of the Euclidean space; k: subspace dimension; l: sample size
         """
         self.sample = np.array(sample)
         self.beta = beta
         self.X = X
         self.get_Preprocessor()
         self.get_dimensions()
         self.get_ones()
         self.get_K_and_K_inv()
 
-    def get_K_and_K_inv(self, sample=None, length_scale=None):
+    def get_K_and_K_inv(self, sample: Optional[matrix] = None,
+                        length_scale: Optional[Union[int, float]] = None) -> tuple[np.ndarray, np.ndarray]:
         """
-        Computes squared-exponential correlation matrix
-        :param sample ([[float]]): vector of scalar parameters, or matrix of vector parameters
-        :param length_scale ([float]): length-scale of correlation, isotropic (scaler)
+        Computes squared-exponential correlation matrix and its corresponding inverse
+        :param sample : vector of scalar parameters, or matrix of vector parameters
+        :param length_scale: length-scale of correlation, isotropic (scaler)
                                         or separable (vector)
         :returns: a correlation matrix K
         """
         if sample is None:
             sample = self.sample
         if length_scale is None:
             length_scale = self.beta
         self.K = Pred.construct_corr_matrix0(sample, length_scale)
         self.K_inv = la.solve(self.K, np.identity(self.K.shape[0]))
         return (self.K, self.K_inv)
 
     @staticmethod
-    def default_length(d, l):
+    def default_length(d: int, l: int) -> float:
         """
         Rule-of-thumb lengthscale of the SE kernel for GPS
         :param d: parameter dimension
         :param l: sample size
         returns: isotropic lengthscale for the unit box [0, 1]^d.
         """
-        return 8/3 * np.sqrt(d) * d/l
+        return (3 * d**(3/2)) / l
 
-    def get_Preprocessor(self):
+    def get_Preprocessor(self) -> np.ndarray:
         """
         :returns: preprocessing quantities of interest
         """
         Preprocessor.setup(self.X)
         self.XtX = Preprocessor.get_XX_cross_product()
         self.VtX = Preprocessor.get_Vt_X()
         return self.XtX, self.VtX
 
-    def get_dimensions(self):
+    def get_dimensions(self) -> int:
         """
         :returns: subspace dimension
         """
         _, K_inv = self.get_K_and_K_inv()
         self.k = self.XtX.shape[-1] // K_inv.shape[-1]
         return self.k
 
-    def get_ones(self):
+    def get_ones(self) -> np.ndarray:
         """
         :returns: matrix of ones (k * k)
         """
         self.Jk = np.ones((self.k, self.k))
         return self.Jk
 
-
-    def LOODistSvd(self, i, K_inv = None, VtX = None):
-        """
-         Compute LOO Riemannian distances: SVD version
-        :param i (int): LOO index
-        :param K_inv: inverse of correlation of matrix
-        :returns: Riemannian distances (normed angle)
-        """
-        if K_inv is None:
-            _, K_inv = self.get_K_and_K_inv()
-        if VtX is None:
-            VtX = self.VtX
-        ## Construct \Pi_{-1}
-        kbii = K_inv[i, i]
-        kbio = np.delete(K_inv[i], [i])
-        kbi = np.delete(np.delete(K_inv, i, 0), i, 1)
-        Dkbioi = np.diag(1 / kbio)
-        Deltai = Dkbioi @ kbi @ Dkbioi * kbii - 1
-        Deltai = np.tril(Deltai) + np.triu(Deltai.T, 1)  # force symmetry of Deltai
-        # row / column indices of the i-th training point
-        idxi = (i-1) * self.k + np.arange(1, self.k+1) + (self.k-1)
-        deltaBoxi = (np.delete(np.delete(self.XtX, idxi, 0), idxi, 1)) * np.kron(Deltai, self.Jk)
-        # compute cholesky
-        U = la.cholesky(deltaBoxi)
-        # triangular inverse
-        U_inv = la.solve(U, np.identity(U.shape[0]))
-        VXiUinv = np.delete(VtX, idxi, 1) @ U_inv
-        Vcheck = scipy.sparse.linalg.svds(VXiUinv, self.k)
-        sigma0 = (VtX[:, idxi]).T @ Vcheck[0]
-        # compute sigma singular values
-        sigma1 = la.svd(sigma0)[1]
-        sigma1[sigma1 > 1] = 1
-        angle = np.arccos(sigma1)
-        normed_angle = la.norm(angle)
-        return normed_angle
-
     # compute Riemannian distance
-    def PrAngles(self, X, Y):
+    def PrAngles(self, X: np.ndarray, Y: np.ndarray) -> np.ndarray:
         """
+         Principal angles between two subspaces
         :param X: subspace representation
         :param Y: subspace representation
         returns: a vector of principal angles in increasing order, [0, pi/2]
         """
         XtY = X.T @ Y
         svdXtY = la.svd(XtY)
         sigma = svdXtY[1]
@@ -129,25 +122,25 @@
         M = (X @ svdXtY[0] - (Y @ (svdXtY[2].T @ np.diag(svdXtY[1])))) @ (svdXtY[2])
         svdM = la.svd(M)
         thetaGL19 = np.flip(np.arcsin(svdM[1]))
         isSmall = theta < (0.1 * np.pi / 2)
         theta[isSmall] = thetaGL19[isSmall]
         return theta
 
-    def RiemannianDist(self, X, Y, normalize=True):
+    def RiemannianDist(self, X: np.ndarray, Y: np.ndarray, normalize: bool =True) -> float:
         angles = self.PrAngles(X, Y)
         if normalize:
             angles = angles / (np.pi / 2)
         return np.sqrt(np.sum(angles ** 2))
 
-    def LOOPredEvd(self, i, K_inv=None, VtX=None):
+    def LOOPredEvd(self, i, K_inv: Optional[np.ndarray] = None, VtX: Optional[np.ndarray] = None) -> np.ndarray:
         """
         Compute LOO prediction: EVD version
         :param i (int): LOO index
-        :param K_inv (([[float]]): inverse of correlation of matrix
+        :param K_inv (: inverse of correlation of matrix
         :returns:LOO prediction in the global basis, \equation{\circ{V}_{-i}}.
         """
         if K_inv is None:
             K, K_inv = self.get_K_and_K_inv()
         if VtX is None:
             VtX = self.VtX
         # Row / column indices of the i-th training point
@@ -173,35 +166,35 @@
             values, vectors = la.eigh(Pi)
             return vectors[:, np.arange(0, self.k)]
         else:
             values, vectors = scipy.sparse.linalg.eigsh(Pi, self.k, maxiter=10000, tol=1e-16)
             return vectors
 
 
-    def LOODistEVD(self, i, K_inv=None, VtX=None):
+    def LOODistEVD(self, i,  K_inv: Optional[np.ndarray] = None, VtX: Optional[np.ndarray] = None) -> float:
         """
          Compute LOO Riemannian distances: EVD version
         :param i (int): LOO index
-        :param K_inv ([[float]]): inverse of correlation of matrix
-        :param VtX ([[float]]): preprocessing quantity of interest
+        :param K_inv : inverse of correlation of matrix
+        :param VtX : preprocessing quantity of interest
         :returns: Riemannian distances (normed angle)
         """
         if K_inv is None:
             _, K_inv = self.get_K_and_K_inv()
         if VtX is None:
             VtX = self.VtX
         Vcirc = self.LOOPredEvd(i, K_inv, VtX)
         # Row/colum indices of the i-th training point
         idxi = (i-1) * self.k + np.arange(1, self.k+1) + (self.k - 1)
         return self.RiemannianDist(self.VtX[:, idxi], Vcirc)
 
     # Criterion to minimize, the LOOCV prediction error: sum of squared Riemannian distances.
     # @note require (thetaTrain, XtX, VbtX; getKinv)
 
-    def hSSDist(self, length):
+    def hSSDist(self, length: Union[int, float]) -> float:
         """
         Criterion to minimize, the LOOCV prediction error
         :param length: default lengthscale
         :returns: sum of squared Riemannian distances.
         """
         _, K_inv = self.get_K_and_K_inv(length_scale=[length])
         if len(self.sample.shape) > 1:
@@ -225,36 +218,33 @@
 
     LOO = LOOCV(X, sample=sample, beta=beta)
 
     #Test get_K_and_K_inv()
     K, K_inv = LOO.get_K_and_K_inv()
 
     #Test default_length ()
-    LOO.default_length(1, len(sample))
+    print(LOO.default_length(1, len(sample)))
 
     # Test get_Preprocessor()
     LOO.get_Preprocessor()
 
     # Test get_dimensions()
     LOO.get_dimensions()
 
     # Test get_ones()
     LOO.get_ones()
 
-    # Test LOODistSvd()
-    LOO.LOODistSvd(0)
-
     #Test LOOPredEvd
     LOO.LOOPredEvd(0)
 
     #Test LOODistEVD()
     LOO.LOODistEVD(0)
 
     # Test hSSDist()
-    print("hSSDist", LOO.hSSDist(3))
+    print("hSSDist", LOO.hSSDist(1.44213061))
```

