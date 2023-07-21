# Comparing `tmp/bs_python_utils-0.2.tar.gz` & `tmp/bs_python_utils-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_python_utils-0.2.tar", max compression
+gzip compressed data, was "bs_python_utils-0.3.tar", max compression
```

## Comparing `bs_python_utils-0.2.tar` & `bs_python_utils-0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1073 2023-04-21 14:06:07.000000 bs_python_utils-0.2/LICENSE
--rw-r--r--   0        0        0     1564 2023-07-17 22:10:49.909803 bs_python_utils-0.2/README.md
--rw-r--r--   0        0        0     1799 2023-04-24 19:42:58.000000 bs_python_utils-0.2/bs_python_utils/Timer.py
--rw-r--r--   0        0        0        0 2023-04-24 19:42:58.000000 bs_python_utils-0.2/bs_python_utils/__init__.py
--rw-r--r--   0        0        0    28473 2023-04-24 22:57:44.000000 bs_python_utils-0.2/bs_python_utils/bs_altair.py
--rw-r--r--   0        0        0     2976 2023-04-24 20:25:24.000000 bs_python_utils-0.2/bs_python_utils/bs_logging.py
--rw-r--r--   0        0        0     3577 2023-04-24 19:42:58.000000 bs_python_utils-0.2/bs_python_utils/bs_mathstr.py
--rw-r--r--   0        0        0     4338 2023-04-24 21:45:53.000000 bs_python_utils-0.2/bs_python_utils/bs_mem.py
--rw-r--r--   0        0        0    13890 2023-07-17 22:06:48.747455 bs_python_utils-0.2/bs_python_utils/bs_opt.py
--rw-r--r--   0        0        0       36 2023-04-24 19:42:58.000000 bs_python_utils-0.2/bs_python_utils/bs_plots.py
--rw-r--r--   0        0        0     4507 2023-04-24 20:32:13.000000 bs_python_utils-0.2/bs_python_utils/bs_seaborn.py
--rw-r--r--   0        0        0     1391 2023-04-24 22:48:26.000000 bs_python_utils-0.2/bs_python_utils/bs_sparse_gaussian.py
--rw-r--r--   0        0        0      905 2023-04-24 19:42:58.000000 bs_python_utils-0.2/bs_python_utils/bsmplutils.py
--rw-r--r--   0        0        0    32084 2023-06-20 20:51:26.000000 bs_python_utils-0.2/bs_python_utils/bsnputils.py
--rw-r--r--   0        0        0     2132 2023-04-24 20:25:24.000000 bs_python_utils-0.2/bs_python_utils/bssputils.py
--rw-r--r--   0        0        0    15489 2023-04-24 20:25:24.000000 bs_python_utils-0.2/bs_python_utils/bsstats.py
--rw-r--r--   0        0        0     9471 2023-05-08 18:43:13.000000 bs_python_utils-0.2/bs_python_utils/bsutils.py
--rw-r--r--   0        0        0    14016 2023-06-20 20:58:35.000000 bs_python_utils-0.2/bs_python_utils/chebyshev.py
--rw-r--r--   0        0        0     7801 2023-04-24 21:45:53.000000 bs_python_utils-0.2/bs_python_utils/distance_covariances.py
--rw-r--r--   0        0        0     1350 2023-04-24 22:36:28.000000 bs_python_utils-0.2/bs_python_utils/example_opt.py
--rw-r--r--   0        0        0     3833 2023-04-24 22:48:26.000000 bs_python_utils-0.2/bs_python_utils/examples_altair.py
--rw-r--r--   0        0        0     1013 2023-04-24 22:36:28.000000 bs_python_utils-0.2/bs_python_utils/examples_distance_covariances.py
--rw-r--r--   0        0        0      552 2023-04-24 22:36:28.000000 bs_python_utils-0.2/bs_python_utils/examples_mem.py
--rw-r--r--   0        0        0      771 2023-04-24 21:45:53.000000 bs_python_utils-0.2/bs_python_utils/examples_seaborn.py
--rw-r--r--   0        0        0      786 2023-04-24 22:36:28.000000 bs_python_utils-0.2/bs_python_utils/examples_sklearn.py
--rw-r--r--   0        0        0     7426 2023-04-24 20:25:24.000000 bs_python_utils-0.2/bs_python_utils/pandas_utils.py
--rw-r--r--   0        0        0     1872 2023-04-24 21:46:50.000000 bs_python_utils-0.2/bs_python_utils/sklearn_utils.py
--rw-r--r--   0        0        0     1868 2023-07-17 22:09:47.445621 bs_python_utils-0.2/pyproject.toml
--rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 bs_python_utils-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-21 14:06:07.415664 bs_python_utils-0.3/LICENSE
+-rw-r--r--   0        0        0     1701 2023-07-21 22:13:37.495534 bs_python_utils-0.3/README.md
+-rw-r--r--   0        0        0     1799 2023-07-21 20:34:46.059698 bs_python_utils-0.3/bs_python_utils/Timer.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:42:58.429294 bs_python_utils-0.3/bs_python_utils/__init__.py
+-rw-r--r--   0        0        0    28473 2023-04-24 22:57:44.859499 bs_python_utils-0.3/bs_python_utils/bs_altair.py
+-rw-r--r--   0        0        0     2976 2023-04-24 20:25:24.489951 bs_python_utils-0.3/bs_python_utils/bs_logging.py
+-rw-r--r--   0        0        0     3577 2023-04-24 19:42:58.433666 bs_python_utils-0.3/bs_python_utils/bs_mathstr.py
+-rw-r--r--   0        0        0     4338 2023-04-24 21:45:53.142922 bs_python_utils-0.3/bs_python_utils/bs_mem.py
+-rw-r--r--   0        0        0    15009 2023-07-21 21:46:32.207754 bs_python_utils-0.3/bs_python_utils/bs_opt.py
+-rw-r--r--   0        0        0       36 2023-04-24 19:42:58.438686 bs_python_utils-0.3/bs_python_utils/bs_plots.py
+-rw-r--r--   0        0        0     4507 2023-04-24 20:32:13.556809 bs_python_utils-0.3/bs_python_utils/bs_seaborn.py
+-rw-r--r--   0        0        0     1391 2023-04-24 22:48:26.302214 bs_python_utils-0.3/bs_python_utils/bs_sparse_gaussian.py
+-rw-r--r--   0        0        0      905 2023-04-24 19:42:58.441367 bs_python_utils-0.3/bs_python_utils/bsmplutils.py
+-rw-r--r--   0        0        0    33601 2023-07-21 21:46:32.440282 bs_python_utils-0.3/bs_python_utils/bsnputils.py
+-rw-r--r--   0        0        0     2132 2023-04-24 20:25:24.253141 bs_python_utils-0.3/bs_python_utils/bssputils.py
+-rw-r--r--   0        0        0    15438 2023-07-21 21:58:00.037774 bs_python_utils-0.3/bs_python_utils/bsstats.py
+-rw-r--r--   0        0        0     9471 2023-05-08 18:43:13.753098 bs_python_utils-0.3/bs_python_utils/bsutils.py
+-rw-r--r--   0        0        0    14016 2023-06-20 20:58:35.000000 bs_python_utils-0.3/bs_python_utils/chebyshev.py
+-rw-r--r--   0        0        0     7801 2023-04-24 21:45:53.165270 bs_python_utils-0.3/bs_python_utils/distance_covariances.py
+-rw-r--r--   0        0        0     1350 2023-04-24 22:36:28.733299 bs_python_utils-0.3/bs_python_utils/example_opt.py
+-rw-r--r--   0        0        0     3833 2023-04-24 22:48:26.344134 bs_python_utils-0.3/bs_python_utils/examples_altair.py
+-rw-r--r--   0        0        0     1013 2023-04-24 22:36:28.733372 bs_python_utils-0.3/bs_python_utils/examples_distance_covariances.py
+-rw-r--r--   0        0        0      552 2023-04-24 22:36:28.733335 bs_python_utils-0.3/bs_python_utils/examples_mem.py
+-rw-r--r--   0        0        0      771 2023-04-24 21:45:53.146924 bs_python_utils-0.3/bs_python_utils/examples_seaborn.py
+-rw-r--r--   0        0        0      786 2023-04-24 22:36:28.733292 bs_python_utils-0.3/bs_python_utils/examples_sklearn.py
+-rw-r--r--   0        0        0     7426 2023-04-24 20:25:24.576148 bs_python_utils-0.3/bs_python_utils/pandas_utils.py
+-rw-r--r--   0        0        0     1872 2023-04-24 21:46:50.361114 bs_python_utils-0.3/bs_python_utils/sklearn_utils.py
+-rw-r--r--   0        0        0     1868 2023-07-21 22:13:53.203848 bs_python_utils-0.3/pyproject.toml
+-rw-r--r--   0        0        0     2670 1970-01-01 00:00:00.000000 bs_python_utils-0.3/PKG-INFO
```

### Comparing `bs_python_utils-0.2/LICENSE` & `bs_python_utils-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/README.md` & `bs_python_utils-0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 My Python utilities.
 
 -   **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
 -   **Documentation** <https://bsalanie.github.io/bs-python-utils/>
 
 ### Release notes
 
+
+#### 0.3 (July 21, 2023)
+Added in Numpy utils a function to set upper and lower triangle to a scalar;
+and `minimize_free` in `bs_opt`.
+
 #### 0.2 (July 17, 2023)
 Fixed printing in accelerated gradient descent.
 
 #### 0.1 (June 20, 2023)
 Added `grid_function` and the `chebyshev` module. 
 
 #### 0.0.6 (May 9, 2023)
```

### Comparing `bs_python_utils-0.2/bs_python_utils/Timer.py` & `bs_python_utils-0.3/bs_python_utils/Timer.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     """
 
     @wraps(func)
     def wrapper(*args: Iterable, **kwargs: dict) -> Any:
         start = time.perf_counter()
         result = func(*args, **kwargs)
         end = time.perf_counter()
-        print(f"{func.__name__} executed in {end - start:.6f} seconds")
+        print(f"{func.__name__} executed in {end - start:.3f} seconds")
         return result
 
     return wrapper
 
 
 class Timer:
     """
```

### Comparing `bs_python_utils-0.2/bs_python_utils/bs_altair.py` & `bs_python_utils-0.3/bs_python_utils/bs_altair.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/bs_python_utils/bs_logging.py` & `bs_python_utils-0.3/bs_python_utils/bs_logging.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/bs_python_utils/bs_mathstr.py` & `bs_python_utils-0.3/bs_python_utils/bs_mathstr.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/bs_python_utils/bs_mem.py` & `bs_python_utils-0.3/bs_python_utils/bs_mem.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/bs_python_utils/bs_opt.py` & `bs_python_utils-0.3/bs_python_utils/bs_opt.py`

 * *Files 12% similar despite different names*

```diff
@@ -335,14 +335,15 @@
         arr_full = np.array(t_full)
         grad_full = grad_obj(arr_full, other_args)
         return np.delete(grad_full, fixed_vars)
 
     return fixed_obj, fixed_grad_obj
 
 
+@timeit
 def minimize_some_fixed(
     obj: Callable,
     grad_obj: Callable,
     x_init: np.ndarray,
     args: Iterable,
     fixed_vars: list[int] | None,
     fixed_vals: np.ndarray | None,
@@ -355,15 +356,15 @@
     Args:
         obj: the original function
         grad_obj: its gradient function
         fixed_vars: a list if the indices of variables whose values are fixed
         fixed_vals: their fixed values
         x_init: the initial values of all variables (those on fixed variables are not used)
         args: other parameters
-        options: any options passed on to scipy.optimize.minimize
+        options: any options passed on to `scipy.optimize.minimize`
         bounds: the bounds on all variables (those on fixed variables are not used)
 
     Returns:
         the result of optimization, on all variables
     """
     if fixed_vars is None:
         resopt = spopt.minimize(
@@ -415,14 +416,60 @@
         # and re-fill the values of the gradients
         g = grad_obj(np.array(t_full), args)
         resopt.jac = g
 
     return resopt
 
 
+@timeit
+def minimize_free(
+    obj: Callable,
+    grad_obj: Callable,
+    x_init: np.ndarray,
+    args: Iterable,
+    options: dict | None = None,
+    bounds: list[tuple[float, float]] | None = None,
+) -> Any:
+    """
+    minimize a function on all of its variables, using BFGS or L-BFGS-B
+
+    Args:
+        obj: the original function
+        grad_obj: its gradient function
+        x_init: the initial values of all variables
+        args: other parameters
+        options: any options passed on to `scipy.optimize.minimize`
+        bounds: the bounds on all variables, if any
+
+    Returns:
+        the result of optimization, on all variables
+    """
+    if bounds is None:
+        resopt = spopt.minimize(
+            obj,
+            x_init,
+            method="BFGS",
+            args=args,
+            options=options,
+            jac=grad_obj,
+        )
+    else:
+        resopt = spopt.minimize(
+            obj,
+            x_init,
+            method="L-BFGS-B",
+            args=args,
+            options=options,
+            jac=grad_obj,
+            bounds=bounds,
+        )
+
+    return resopt
+
+
 def dfp_update(
     hess_inv: np.ndarray, gradient_diff: np.ndarray, x_diff: np.ndarray
 ) -> np.ndarray:
     """runs a DFP update for the inverse Hessian
 
     Args:
         hess_inv: the current inverse Hessian
```

### Comparing `bs_python_utils-0.2/bs_python_utils/bs_seaborn.py` & `bs_python_utils-0.3/bs_python_utils/bs_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/bs_python_utils/bs_sparse_gaussian.py` & `bs_python_utils-0.3/bs_python_utils/bs_sparse_gaussian.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/bs_python_utils/bsmplutils.py` & `bs_python_utils-0.3/bs_python_utils/bsmplutils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/bs_python_utils/bsnputils.py` & `bs_python_utils-0.3/bs_python_utils/bsnputils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1054,7 +1054,50 @@
             for i in range(nv):
                 s += f"  {qv[i]: >10.3f}"
             print(f"{s}")
     else:
         bs_error_abort("v must be  a vector or a list of vectors")
 
     return cast(np.ndarray, qvals)
+
+
+def set_elements_abovebelow_diagonal(
+    matrix: np.ndarray, scalar: int | float, location: str
+) -> np.ndarray:
+    """
+    Sets all elements of the given matrix above or below the diagonal
+    to the specified scalar value.
+
+    Args:
+        matrix: the input matrix; it must be square
+        scalar: The scalar value to set the elements above or below the diagonal.
+        location: 'above', 'below', 'on_above', 'on_below'.
+
+    Returns:
+        The updated matrix with elements above or below the diagonal set to the scalar value,
+        including the diagonal for the `on_` options.
+    """
+    _ = check_square(matrix, "set_elements_abovebelow_diagonal")
+    # copy the matrix
+    new_matrix = matrix.copy()
+
+    # Get the indices of elements above or below the diagonal
+    if location == "above":
+        row_indices, col_indices = np.triu_indices_from(new_matrix, k=1)
+    elif location == "below":
+        row_indices, col_indices = np.tril_indices_from(new_matrix, k=-1)
+    elif location == "on_above":
+        row_indices, col_indices = np.triu_indices_from(new_matrix, k=0)
+    elif location == "on_below":
+        row_indices, col_indices = np.tril_indices_from(new_matrix, k=0)
+    else:
+        bs_error_abort(
+            f"""
+        location can only be 'above', 'below', 
+        'on_above' or 'on_below', not {location}
+        """
+        )
+
+    # Set the elements above or below the diagonal to the scalar value
+    new_matrix[row_indices, col_indices] = scalar
+
+    return new_matrix
```

### Comparing `bs_python_utils-0.2/bs_python_utils/bssputils.py` & `bs_python_utils-0.3/bs_python_utils/bssputils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/bs_python_utils/bsstats.py` & `bs_python_utils-0.3/bs_python_utils/bsstats.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,31 +20,28 @@
 )
 from bs_python_utils.bssputils import spline_reg
 from bs_python_utils.bsutils import bs_error_abort
 
 
 @dataclass
 class TslsResults:
-    """
-    contains full results of a TSLS regression
-    """
+    """contains the full results of a TSLS regression"""
 
     iv_estimates: float | np.ndarray | None
     r2_first_iv: float | np.ndarray | None
     r2_y: float | None
     r2_second: float | np.ndarray | None
     y_proj: float | np.ndarray | None
     y_coeffs: float | np.ndarray | None
     X_IV_proj: float | np.ndarray | None
     b_proj_IV: float | np.ndarray | None
 
 
 def _powers_Z(Z: np.ndarray, degrees: np.ndarray) -> np.ndarray:
-    """
-    used internally by `proj_Z`; returns `\\prod_{k=1}^m  Z_{\\cdot k}^{l_k}`
+    """used internally by `proj_Z`; returns `\\prod_{k=1}^m  Z_{\\cdot k}^{l_k}`
 
     Args:
         Z: a matrix `(n, m)`
         list_ints: a list of integers
 
     Returns:
         the product of the powers of `Z`
@@ -101,16 +98,15 @@
     Zp = Zp[:, :k]
     return Zp, k
 
 
 def proj_Z(
     W: np.ndarray, Z: np.ndarray, p: int = 1, verbose: bool = False
 ) -> tuple[np.ndarray, np.ndarray, float]:
-    """
-    project `W` on `Z` up to degree `p` interactions
+    """project `W` on `Z` up to degree `p` interactions
 
     Args:
         W: variable(s) `(nobs)` or `(nobs, nw)`
         Z: instruments `(nobs) or `(nobs, nz)`;
             they should **not** include a constant term
         p: maximum total degree for interactions of the columns of `Z`
         verbose: prints stuff if True
@@ -136,16 +132,15 @@
         if verbose:
             print(f"_proj_Z with degree {p}, using {k} regressors")
 
     return _final_proj(Zp, W)
 
 
 def tsls(y: np.ndarray, X: np.ndarray, Z: np.ndarray) -> TslsResults:
-    """
-    TSLS of `y` on `X` with instruments `Z`
+    """TSLS of `y` on `X` with instruments `Z`
 
     Args:
         y: independent variable `(nobs)`
         X: covariates `(nobs, nx)`
         Z: instruments `(nobs, nz)`
 
     Returns:
@@ -171,16 +166,15 @@
 def reg_nonpar(
     y: np.ndarray,
     X: np.ndarray,
     var_types: str | None = None,
     n_sub: int | None = None,
     n_res: int | None = 1,
 ) -> tuple[KernelReg, np.ndarray]:
-    """
-    nonparametric regression of y on the columns of X;
+    """nonparametric regression of y on the columns of X;
     bandwidth chosen on a subsample of size nsub if nsub < nobs, and rescaled
 
     Args:
         y: a vector of size nobs
         X: a (nobs) vector or a matrix of shape (nobs, m)
         var_types: specify types of all `X` variables if not all of them are continuous;
             one character per variable
@@ -224,16 +218,15 @@
     y: np.ndarray,
     X: np.ndarray,
     var_types: str | None = None,
     n_sub: int | None = None,
     n_res: int = 1,
     verbose: bool = False,
 ) -> np.ndarray:
-    """
-    nonparametric regression of y on the columns of X; bandwidth chosen on a subsample of size nsub if nsub < nobs, and rescaled
+    """nonparametric regression of y on the columns of X; bandwidth chosen on a subsample of size nsub if nsub < nobs, and rescaled
 
     Args:
         y: a vector of size nobs
         X: a (nobs) vector or a matrix of shape (nobs, m)
         var_types: specify types of all `X` variables if not all of them are continuous;
             one character per variable
             * 'c' for continuous
@@ -256,16 +249,15 @@
     X: np.ndarray,
     mode: str = "NP",
     var_types: str | None = None,
     n_sub: int | None = None,
     n_res: int = 1,
     verbose: bool = False,
 ) -> np.ndarray:
-    """
-    flexible regression  of `Y` on `X`
+    """flexible regression  of `Y` on `X`
 
     Args:
         Y: independent variable `(nobs)` or `(nobs, ny)`
         X: covariates `(nobs)` or `(nobs, nx)`; should **not** include a constant term
         mode: what flexible means
             * 'NP': non parametric
             * 'SPL': spline regression, only on one covariate
@@ -314,16 +306,15 @@
         preg, _, _ = proj_Z(Y, X, p=imode, verbose=verbose)
         return preg
 
 
 def bs_multivariate_normal_pdf(
     values_x: np.ndarray, means_x: float | np.ndarray, cov_mat: float | np.ndarray
 ) -> np.ndarray:
-    """
-    Multivariate (or univariate) normal probability density function at values_x
+    """Multivariate (or univariate) normal probability density function at values_x
 
     Args:
         values_x: values at which to evaluate the pdf, an `n`-vector or an `(n, nvars)` matrix
         means_x: means of the multivariate normal, a float or an `(nvars)` vector
         cov_mat: covariance matrix of the multivariate normal, a float or an `(nvars, nvars)` matrix
 
     Returns:
@@ -362,16 +353,15 @@
 
 def estimate_pdf(
     x_obs: np.ndarray,
     x_points: np.ndarray,
     MIN_SIZE_NONPAR: int = 200,
     weights: np.ndarray | None = None,
 ) -> np.ndarray:
-    """
-    return an estimate of the conditional densities of `x` at points `values_x` (Silverman rule)
+    """return an estimate of the conditional densities of `x` at points `values_x` (Silverman rule)
 
     Args:
         x_obs: an `n`-vector or an `(n, nvars)` matrix of the observed values of `x`
         x_points: an `m`-vector or an `(m, nvars)` matrix of x values
         MIN_SIZE_NONPAR: minimum size above which we use kernel density estimators
         weights: an `n`-vector of weights for the observations, if present
 
@@ -427,16 +417,15 @@
             f_x *= weights / np.mean(weights)
     return cast(np.ndarray, f_x)
 
 
 def estimate_densities_at_quantiles(
     X: np.ndarray, qtiles: np.ndarray
 ) -> tuple[np.ndarray, np.ndarray] | tuple[np.ndarray, np.ndarray, np.ndarray]:
-    """
-    estimate densities of margins at prespecified quantiles (Silverman rule)
+    """estimate densities of margins at prespecified quantiles (Silverman rule)
     and the joint density at each vector of these quantiles
 
     Args:
         X: `n`-vector or `(n, nx)`-matrix
         qtiles: vector of `nq` numbers between 0 and 1
 
     Returns:
```

### Comparing `bs_python_utils-0.2/bs_python_utils/bsutils.py` & `bs_python_utils-0.3/bs_python_utils/bsutils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/bs_python_utils/chebyshev.py` & `bs_python_utils-0.3/bs_python_utils/chebyshev.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/bs_python_utils/distance_covariances.py` & `bs_python_utils-0.3/bs_python_utils/distance_covariances.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/bs_python_utils/example_opt.py` & `bs_python_utils-0.3/bs_python_utils/example_opt.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/bs_python_utils/examples_altair.py` & `bs_python_utils-0.3/bs_python_utils/examples_altair.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/bs_python_utils/examples_distance_covariances.py` & `bs_python_utils-0.3/bs_python_utils/examples_distance_covariances.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/bs_python_utils/examples_mem.py` & `bs_python_utils-0.3/bs_python_utils/examples_mem.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/bs_python_utils/examples_seaborn.py` & `bs_python_utils-0.3/bs_python_utils/examples_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/bs_python_utils/examples_sklearn.py` & `bs_python_utils-0.3/bs_python_utils/examples_sklearn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/bs_python_utils/pandas_utils.py` & `bs_python_utils-0.3/bs_python_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/bs_python_utils/sklearn_utils.py` & `bs_python_utils-0.3/bs_python_utils/sklearn_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.2/pyproject.toml` & `bs_python_utils-0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bs_python_utils"
-version = "0.2"
+version = "0.3"
 description = "my Python utilities"
 authors = ["Bernard Salanie <bsalanie@columbia.edu>"]
 repository = "https://github.com/bsalanie/bs-python-utils"
 documentation = "https://bsalanie.github.io/bs-python-utils/"
 readme = "README.md"
 packages = [
   {include = "bs_python_utils"}
@@ -24,15 +24,15 @@
 pytest = "^7.2.0"
 mypy = "^0.981"
 pre-commit = "^2.20.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocs-material = "^8.5.10"
-mkdocstrings = {extras = ["python"], version = "^0.19.0"}
+mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
```

### Comparing `bs_python_utils-0.2/PKG-INFO` & `bs_python_utils-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bs-python-utils
-Version: 0.2
+Version: 0.3
 Summary: my Python utilities
 Home-page: https://github.com/bsalanie/bs-python-utils
 Author: Bernard Salanie
 Author-email: bsalanie@columbia.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -33,14 +33,19 @@
 My Python utilities.
 
 -   **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
 -   **Documentation** <https://bsalanie.github.io/bs-python-utils/>
 
 ### Release notes
 
+
+#### 0.3 (July 21, 2023)
+Added in Numpy utils a function to set upper and lower triangle to a scalar;
+and `minimize_free` in `bs_opt`.
+
 #### 0.2 (July 17, 2023)
 Fixed printing in accelerated gradient descent.
 
 #### 0.1 (June 20, 2023)
 Added `grid_function` and the `chebyshev` module. 
 
 #### 0.0.6 (May 9, 2023)
```

