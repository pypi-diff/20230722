# Comparing `tmp/estyp-0.2.4.tar.gz` & `tmp/estyp-0.2.5.tar.gz`

## Comparing `estyp-0.2.4.tar` & `estyp-0.2.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 estyp-0.2.4/estyp/linear_model/__init__.py
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 estyp-0.2.4/estyp/linear_model/stepwise.py
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 estyp-0.2.4/estyp/testing/__init__.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 estyp-0.2.4/estyp/testing/__base/__init__.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 estyp-0.2.4/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 estyp-0.2.4/LICENSE
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 estyp-0.2.4/README.md
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 estyp-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 estyp-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 estyp-0.2.5/estyp/linear_model/__init__.py
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 estyp-0.2.5/estyp/linear_model/stepwise.py
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 estyp-0.2.5/estyp/testing/__init__.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 estyp-0.2.5/estyp/testing/__base/__init__.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 estyp-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 estyp-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 estyp-0.2.5/README.md
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 estyp-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 estyp-0.2.5/PKG-INFO
```

### Comparing `estyp-0.2.4/estyp/linear_model/__init__.py` & `estyp-0.2.5/estyp/linear_model/__init__.py`

 * *Files identical despite different names*

### Comparing `estyp-0.2.4/estyp/linear_model/stepwise.py` & `estyp-0.2.5/estyp/linear_model/stepwise.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     "y": [1, 2, 3, 4, 5],
     "x1": [1, 2, 3, 4, 5],
     "x2": [6, 7, 8, 9, 10],
 })
 
 formula = "y ~ x1 + x2"
 
-model = sm.GLM(data=data, formula=formula, family=sm.families.Gaussian())
+model = sm.GLM
 
-final_formula = both_selection(formula=formula, data=data, model=model, max_iter=10000)
+final_formula = both_selection(formula=formula, data=data, model=model)
 
 print(final_formula)
     """
     print("Este proceso tarda un buen tiempo ¡Paciencia! Momento de cuestionarte si eres feliz.")
     # Preparación
     fi = formula
     e = model.from_formula(fi, data)
```

### Comparing `estyp-0.2.4/.gitignore` & `estyp-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `estyp-0.2.4/LICENSE` & `estyp-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `estyp-0.2.4/README.md` & `estyp-0.2.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,29 @@
 
 ## Description
 
 This library is a collection of statistical functions for Python. It includes a function for performing stepwise with AIC criterion and a function for the F-ratio test.
 
 Actually, the name comes from the way my friends call me (esty), plus the "p" which is the initial of `python`.
 
+## Changelog 
+
+### V0.2.5
+
+* Added `scipy>=1.11.1` as a depedency of the library.
+* New modularization of the functions in the `testing` module.
+* R like documentation in the `testing.var_test()` function.
+* Added `testing.t_test()` function to perform t-test like in software R.
+
 ## Functions
 
 * `linear_model.LogisticRegression()`: This class implements a logistic regression model. It inherits from the `sklearn.linear_model.LogisticRegression()` class, but adds additional methods for calculating confidence intervals, p-values, and model summaries.
 * `linear_model.stepwise.both_selection()`: This function performs both forward and backward variable selection using the Akaike Information Criterion (AIC). 
-* `testing.var_test()`: Performs an F-ratio test to compare the variances of two samples. The output was inspired by the `var_test()` function in `R`.
+* `testing.var_test()`: Performs an F test to compare the variances of two samples from normal populations. This function is inspired by the `var.test()` function of the software R.
+* `testing.t_test()`: Performs one and two sample t-tests on groups of data. This function is inspired by the `t.test()` function of the software R.
 
 # Installation
 
 To install this library, you can use pip:
 
 ```bash
 pip install estyp
```

### Comparing `estyp-0.2.4/pyproject.toml` & `estyp-0.2.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "estyp"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
     { name="estebanrucan", email="errucan@gmail.com" },
 ]
 description = "Extended Statistical Toolkit Yet Practical"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9.12"
@@ -19,13 +19,13 @@
     "Development Status :: 1 - Planning"
 ]
 dependencies = [
     "numpy >= 1.22.3",
     "scikit-learn >= 1.2.1",
     "patsy >= 0.5.3",
     "statsmodels >= 0.13.5",
-    "scipy >= 1.8.1"
+    "scipy >= 1.11.1"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/estebanrucan/estyp"
 "Bug Tracker" = "https://github.com/estebanrucan/estyp/issues"
```

### Comparing `estyp-0.2.4/PKG-INFO` & `estyp-0.2.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estyp
-Version: 0.2.4
+Version: 0.2.5
 Summary: Extended Statistical Toolkit Yet Practical
 Project-URL: Homepage, https://github.com/estebanrucan/estyp
 Project-URL: Bug Tracker, https://github.com/estebanrucan/estyp/issues
 Author-email: estebanrucan <errucan@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Esteban Rucán Carrasco
@@ -31,31 +31,41 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9.12
 Requires-Dist: numpy>=1.22.3
 Requires-Dist: patsy>=0.5.3
 Requires-Dist: scikit-learn>=1.2.1
-Requires-Dist: scipy>=1.8.1
+Requires-Dist: scipy>=1.11.1
 Requires-Dist: statsmodels>=0.13.5
 Description-Content-Type: text/markdown
 
 # ESTYP: Extended Statistical Toolkit Yet Practical
 
 ## Description
 
 This library is a collection of statistical functions for Python. It includes a function for performing stepwise with AIC criterion and a function for the F-ratio test.
 
 Actually, the name comes from the way my friends call me (esty), plus the "p" which is the initial of `python`.
 
+## Changelog 
+
+### V0.2.5
+
+* Added `scipy>=1.11.1` as a depedency of the library.
+* New modularization of the functions in the `testing` module.
+* R like documentation in the `testing.var_test()` function.
+* Added `testing.t_test()` function to perform t-test like in software R.
+
 ## Functions
 
 * `linear_model.LogisticRegression()`: This class implements a logistic regression model. It inherits from the `sklearn.linear_model.LogisticRegression()` class, but adds additional methods for calculating confidence intervals, p-values, and model summaries.
 * `linear_model.stepwise.both_selection()`: This function performs both forward and backward variable selection using the Akaike Information Criterion (AIC). 
-* `testing.var_test()`: Performs an F-ratio test to compare the variances of two samples. The output was inspired by the `var_test()` function in `R`.
+* `testing.var_test()`: Performs an F test to compare the variances of two samples from normal populations. This function is inspired by the `var.test()` function of the software R.
+* `testing.t_test()`: Performs one and two sample t-tests on groups of data. This function is inspired by the `t.test()` function of the software R.
 
 # Installation
 
 To install this library, you can use pip:
 
 ```bash
 pip install estyp
```

