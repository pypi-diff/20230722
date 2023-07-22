# Comparing `tmp/xlogit-0.2.5.tar.gz` & `tmp/xlogit-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlogit-0.2.5.tar", last modified: Fri Jun 16 08:15:00 2023, max compression
+gzip compressed data, was "xlogit-0.2.6.tar", last modified: Sat Jul 22 13:21:46 2023, max compression
```

## Comparing `xlogit-0.2.5.tar` & `xlogit-0.2.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 das       (1000) das       (1000)        0 2023-06-16 08:15:00.841240 xlogit-0.2.5/
--rw-rw-r--   0 das       (1000) das       (1000)    35149 2022-03-23 01:15:13.000000 xlogit-0.2.5/LICENSE
--rw-r--r--   0 das       (1000) das       (1000)    10383 2023-06-16 08:15:00.841240 xlogit-0.2.5/PKG-INFO
--rw-r--r--   0 das       (1000) das       (1000)    10041 2023-06-16 08:10:09.000000 xlogit-0.2.5/README.rst
--rw-r--r--   0 das       (1000) das       (1000)       38 2023-06-16 08:15:00.841240 xlogit-0.2.5/setup.cfg
--rw-r--r--   0 das       (1000) das       (1000)      872 2023-06-16 08:10:30.000000 xlogit-0.2.5/setup.py
-drwxr-xr-x   0 das       (1000) das       (1000)        0 2023-06-16 08:15:00.841240 xlogit-0.2.5/tests/
--rwxr-xr-x   0 das       (1000) das       (1000)     3091 2022-06-11 06:21:48.000000 xlogit-0.2.5/tests/test__choice_model.py
--rwxrwxr-x   0 das       (1000) das       (1000)     1761 2022-06-01 07:42:17.000000 xlogit-0.2.5/tests/test__device.py
--rw-rw-r--   0 das       (1000) das       (1000)     5214 2023-06-16 03:10:49.000000 xlogit-0.2.5/tests/test_mixed_logit.py
--rwxrwxr-x   0 das       (1000) das       (1000)     3518 2023-06-16 03:10:49.000000 xlogit-0.2.5/tests/test_multinomial_logit.py
--rwxrwxr-x   0 das       (1000) das       (1000)     1940 2022-06-25 05:26:01.000000 xlogit-0.2.5/tests/test_utils.py
-drwxr-xr-x   0 das       (1000) das       (1000)        0 2023-06-16 08:15:00.841240 xlogit-0.2.5/xlogit/
--rw-rw-r--   0 das       (1000) das       (1000)      112 2022-03-23 01:15:13.000000 xlogit-0.2.5/xlogit/__init__.py
--rwxrwxr-x   0 das       (1000) das       (1000)    11115 2023-06-16 03:10:49.000000 xlogit-0.2.5/xlogit/_choice_model.py
--rwxrwxr-x   0 das       (1000) das       (1000)     1983 2022-06-01 05:55:09.000000 xlogit-0.2.5/xlogit/_device.py
--rw-r--r--   0 das       (1000) das       (1000)     3098 2022-06-25 05:00:58.000000 xlogit-0.2.5/xlogit/_optimize.py
--rw-rw-r--   0 das       (1000) das       (1000)    31981 2023-06-16 03:12:49.000000 xlogit-0.2.5/xlogit/mixed_logit.py
--rw-rw-r--   0 das       (1000) das       (1000)    13869 2023-06-16 03:13:14.000000 xlogit-0.2.5/xlogit/multinomial_logit.py
--rwxrwxr-x   0 das       (1000) das       (1000)     3851 2022-06-25 05:23:47.000000 xlogit-0.2.5/xlogit/utils.py
-drwxr-xr-x   0 das       (1000) das       (1000)        0 2023-06-16 08:15:00.841240 xlogit-0.2.5/xlogit.egg-info/
--rw-r--r--   0 das       (1000) das       (1000)    10383 2023-06-16 08:15:00.000000 xlogit-0.2.5/xlogit.egg-info/PKG-INFO
--rw-r--r--   0 das       (1000) das       (1000)      480 2023-06-16 08:15:00.000000 xlogit-0.2.5/xlogit.egg-info/SOURCES.txt
--rw-r--r--   0 das       (1000) das       (1000)        1 2023-06-16 08:15:00.000000 xlogit-0.2.5/xlogit.egg-info/dependency_links.txt
--rw-r--r--   0 das       (1000) das       (1000)        1 2022-06-25 05:41:05.000000 xlogit-0.2.5/xlogit.egg-info/not-zip-safe
--rw-r--r--   0 das       (1000) das       (1000)       27 2023-06-16 08:15:00.000000 xlogit-0.2.5/xlogit.egg-info/requires.txt
--rw-r--r--   0 das       (1000) das       (1000)        7 2023-06-16 08:15:00.000000 xlogit-0.2.5/xlogit.egg-info/top_level.txt
+drwxrwxr-x   0 das       (1000) das       (1000)        0 2023-07-22 13:21:46.608198 xlogit-0.2.6/
+-rw-rw-r--   0 das       (1000) das       (1000)    35149 2022-03-23 01:15:13.000000 xlogit-0.2.6/LICENSE
+-rw-rw-r--   0 das       (1000) das       (1000)    10383 2023-07-22 13:21:46.608198 xlogit-0.2.6/PKG-INFO
+-rw-r--r--   0 das       (1000) das       (1000)    10041 2023-06-16 08:10:09.000000 xlogit-0.2.6/README.rst
+-rw-rw-r--   0 das       (1000) das       (1000)       38 2023-07-22 13:21:46.608198 xlogit-0.2.6/setup.cfg
+-rw-r--r--   0 das       (1000) das       (1000)      872 2023-07-22 13:17:34.000000 xlogit-0.2.6/setup.py
+drwxrwxr-x   0 das       (1000) das       (1000)        0 2023-07-22 13:21:46.608198 xlogit-0.2.6/tests/
+-rwxr-xr-x   0 das       (1000) das       (1000)     3091 2022-06-11 06:21:48.000000 xlogit-0.2.6/tests/test__choice_model.py
+-rwxrwxr-x   0 das       (1000) das       (1000)     1761 2022-06-01 07:42:17.000000 xlogit-0.2.6/tests/test__device.py
+-rw-rw-r--   0 das       (1000) das       (1000)     5214 2023-06-16 03:10:49.000000 xlogit-0.2.6/tests/test_mixed_logit.py
+-rwxrwxr-x   0 das       (1000) das       (1000)     3518 2023-06-16 03:10:49.000000 xlogit-0.2.6/tests/test_multinomial_logit.py
+-rwxrwxr-x   0 das       (1000) das       (1000)     1940 2022-06-25 05:26:01.000000 xlogit-0.2.6/tests/test_utils.py
+drwxrwxr-x   0 das       (1000) das       (1000)        0 2023-07-22 13:21:46.608198 xlogit-0.2.6/xlogit/
+-rw-rw-r--   0 das       (1000) das       (1000)      112 2022-03-23 01:15:13.000000 xlogit-0.2.6/xlogit/__init__.py
+-rwxrwxr-x   0 das       (1000) das       (1000)    11115 2023-06-16 03:10:49.000000 xlogit-0.2.6/xlogit/_choice_model.py
+-rwxrwxr-x   0 das       (1000) das       (1000)     1983 2022-06-01 05:55:09.000000 xlogit-0.2.6/xlogit/_device.py
+-rw-r--r--   0 das       (1000) das       (1000)     3098 2022-06-25 05:00:58.000000 xlogit-0.2.6/xlogit/_optimize.py
+-rw-rw-r--   0 das       (1000) das       (1000)    32208 2023-07-22 13:16:15.000000 xlogit-0.2.6/xlogit/mixed_logit.py
+-rw-rw-r--   0 das       (1000) das       (1000)    14106 2023-07-22 13:16:15.000000 xlogit-0.2.6/xlogit/multinomial_logit.py
+-rwxrwxr-x   0 das       (1000) das       (1000)     3851 2022-06-25 05:23:47.000000 xlogit-0.2.6/xlogit/utils.py
+drwxrwxr-x   0 das       (1000) das       (1000)        0 2023-07-22 13:21:46.608198 xlogit-0.2.6/xlogit.egg-info/
+-rw-r--r--   0 das       (1000) das       (1000)    10383 2023-07-22 13:21:46.000000 xlogit-0.2.6/xlogit.egg-info/PKG-INFO
+-rw-r--r--   0 das       (1000) das       (1000)      480 2023-07-22 13:21:46.000000 xlogit-0.2.6/xlogit.egg-info/SOURCES.txt
+-rw-r--r--   0 das       (1000) das       (1000)        1 2023-07-22 13:21:46.000000 xlogit-0.2.6/xlogit.egg-info/dependency_links.txt
+-rw-r--r--   0 das       (1000) das       (1000)        1 2022-06-25 05:41:05.000000 xlogit-0.2.6/xlogit.egg-info/not-zip-safe
+-rw-r--r--   0 das       (1000) das       (1000)       27 2023-07-22 13:21:46.000000 xlogit-0.2.6/xlogit.egg-info/requires.txt
+-rw-r--r--   0 das       (1000) das       (1000)        7 2023-07-22 13:21:46.000000 xlogit-0.2.6/xlogit.egg-info/top_level.txt
```

### Comparing `xlogit-0.2.5/LICENSE` & `xlogit-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.5/PKG-INFO` & `xlogit-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlogit
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python package for GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/arteagac/xlogit
 Author: Cristian Arteaga
 Author-email: cristiandavidarteaga@gmail.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
```

### Comparing `xlogit-0.2.5/README.rst` & `xlogit-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.5/setup.py` & `xlogit-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import codecs
 
 with codecs.open('README.rst', encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(name='xlogit',
-                 version='0.2.5',
+                 version='0.2.6',
                  description='A Python package for GPU-accelerated ' +
                  'estimation of mixed logit models.',
                  long_description=long_description,
                  long_description_content_type="text/x-rst",
                  url='https://github.com/arteagac/xlogit',
                  author='Cristian Arteaga',
                  author_email='cristiandavidarteaga@gmail.com',
```

### Comparing `xlogit-0.2.5/tests/test__choice_model.py` & `xlogit-0.2.6/tests/test__choice_model.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.5/tests/test__device.py` & `xlogit-0.2.6/tests/test__device.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.5/tests/test_mixed_logit.py` & `xlogit-0.2.6/tests/test_mixed_logit.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.5/tests/test_multinomial_logit.py` & `xlogit-0.2.6/tests/test_multinomial_logit.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.5/tests/test_utils.py` & `xlogit-0.2.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.5/xlogit/_choice_model.py` & `xlogit-0.2.6/xlogit/_choice_model.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.5/xlogit/_device.py` & `xlogit-0.2.6/xlogit/_device.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.5/xlogit/_optimize.py` & `xlogit-0.2.6/xlogit/_optimize.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.5/xlogit/mixed_logit.py` & `xlogit-0.2.6/xlogit/mixed_logit.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         super(MixedLogit, self).__init__()
         self._rvidx = None  # Index of random variables (True when random var)
         self._rvdist = None  # List of mixing distributions of rand vars
 
     def fit(self, X, y, varnames, alts, ids, randvars, isvars=None, weights=None, avail=None,  panels=None,
             base_alt=None, fit_intercept=False, init_coeff=None, maxiter=2000, random_state=None, n_draws=1000,
             halton=True, verbose=1, batch_size=None, halton_opts=None, tol_opts=None, robust=False, num_hess=False,
-            scale_factor=None, optim_method="BFGS", mnl_init=True, addit=None):
+            scale_factor=None, optim_method="BFGS", mnl_init=True, addit=None, skip_std_errs=False):
         """Fit Mixed Logit models.
 
         Parameters
         ----------
         X : array-like, shape (n_samples*n_alts, n_variables)
             Input data for explanatory variables in long format
 
@@ -167,14 +167,17 @@
 
         robust: bool, default=False
             Whether robust standard errors should be computed
 
         num_hess: bool, default=False
             Whether numerical hessian should be used for estimation of standard errors
 
+        skip_std_errs: bool, default=False
+            Whether estimation of standard errors should be skipped
+
         mnl_init: bool, default=True
             Whether to initialize coefficients using estimates from a multinomial logit
         Returns
         -------
         None.
         """
         # Handle array-like inputs by converting everything to numpy arrays
@@ -215,17 +218,19 @@
         if scale_factor is not None:
             coef_names = np.append(coef_names, "_scale_factor")
 
         num_hess = num_hess if scale_factor is None else True
         if optim_method == "L-BFGS-B":
             optim_res['grad_n'] = self._loglik_gradient(optim_res['x'], *fargs, return_gradient=True)[2]
 
-        if num_hess or optim_method == "L-BFGS-B":
+        if (num_hess or optim_method == "L-BFGS-B") and not skip_std_errs:
             optim_res['hess_inv'] = _numerical_hessian(optim_res['x'], self._loglik_gradient, args=fargs)
-        
+        else:
+            optim_res['hess_inv'] = np.eye(len(optim_res['x']))
+
         self._post_fit(optim_res, coef_names, X.shape[0], verbose, robust)
 
 
 
     def predict(self, X, varnames, alts, ids, isvars=None, weights=None, avail=None,  panels=None, random_state=None,
                 n_draws=1000, halton=True, verbose=1, batch_size=None, return_proba=False, return_freq=False,
                 halton_opts=None, scale_factor=None, addit=None):
```

### Comparing `xlogit-0.2.5/xlogit/multinomial_logit.py` & `xlogit-0.2.6/xlogit/multinomial_logit.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,17 @@
 
         bic : float
             Bayesian information criteria of the estimated model
     """
 
     def fit(self, X, y, varnames, alts, ids, isvars=None,
             weights=None, avail=None, base_alt=None, fit_intercept=False,
-            init_coeff=None, maxiter=2000, random_state=None, tol_opts=None, verbose=1,
-            robust=False, num_hess=False, scale_factor=None, addit=None):
+            init_coeff=None, maxiter=2000, random_state=None, tol_opts=None,
+            verbose=1, robust=False, num_hess=False, scale_factor=None,
+            addit=None, skip_std_errs=False):
         """Fit multinomial and/or conditional logit models.
 
         Parameters
         ----------
         X : array-like, shape (n_samples*n_alts, n_variables)
             Input data for explanatory variables in long format
 
@@ -109,14 +110,17 @@
 
         robust: bool, default=False
             Whether robust standard errors should be computed
 
         num_hess: bool, default=False
             Whether numerical hessian should be used for estimation of standard errors
 
+        skip_std_errs: bool, default=False
+            Whether estimation of standard errors should be skipped
+
         random_state : int, default=None
             Random seed for numpy random generator
 
         tol_opts : dict, default=None
             Options for tolerance of optimization routine. The dictionary accepts the following options (keys):
 
                 ftol : float, default=1e-10
@@ -153,16 +157,18 @@
         fargs = (Xd, scale_d, addit_d, weights, avail)
         optim_res = _minimize(self._loglik_gradient, betas, args=fargs, method="BFGS", tol=tol['ftol'],
                               options={'maxiter': maxiter, 'disp': verbose > 1})
         coef_names = Xnames
         if scale_factor is not None:
             coef_names = np.append(coef_names, "_scale_factor")
 
-        if num_hess or True:
+        if num_hess and not skip_std_errs:
             optim_res['hess_inv'] = _numerical_hessian(optim_res['x'], self._loglik_gradient, args=fargs)
+        else:
+            optim_res['hess_inv'] = np.eye(len(optim_res['x']))
         self._post_fit(optim_res, coef_names, X.shape[0], verbose, robust)
 
 
     def predict(self, X, varnames, alts, ids, isvars=None, weights=None,
                 avail=None, random_state=None, verbose=1,
                 return_proba=False, return_freq=False, scale_factor=None, addit=None):
         """Predict chosen alternatives.
```

### Comparing `xlogit-0.2.5/xlogit/utils.py` & `xlogit-0.2.6/xlogit/utils.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.5/xlogit.egg-info/PKG-INFO` & `xlogit-0.2.6/xlogit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlogit
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python package for GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/arteagac/xlogit
 Author: Cristian Arteaga
 Author-email: cristiandavidarteaga@gmail.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
```

