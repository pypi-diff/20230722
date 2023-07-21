# Comparing `tmp/ginormal-0.0.4.tar.gz` & `tmp/ginormal-0.0.5.tar.gz`

## Comparing `ginormal-0.0.4.tar` & `ginormal-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 ginormal-0.0.4/src/ginormal/__init__.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 ginormal-0.0.4/src/ginormal/example.py
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 ginormal-0.0.4/src/ginormal/main.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 ginormal-0.0.4/src/intermediate/_F0g.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ginormal-0.0.4/src/intermediate/__init__.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 ginormal-0.0.4/src/intermediate/_dg1.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ginormal-0.0.4/src/intermediate/_msh.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 ginormal-0.0.4/src/intermediate/_pbd.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 ginormal-0.0.4/src/intermediate/_rtg1.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ginormal-0.0.4/.gitignore
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ginormal-0.0.4/LICENSE.md
--rw-r--r--   0        0        0     8646 2020-02-02 00:00:00.000000 ginormal-0.0.4/README.md
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 ginormal-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     9503 2020-02-02 00:00:00.000000 ginormal-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 ginormal-0.0.5/src/ginormal/__init__.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 ginormal-0.0.5/src/ginormal/example.py
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 ginormal-0.0.5/src/ginormal/main.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 ginormal-0.0.5/src/intermediate/_F0g.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ginormal-0.0.5/src/intermediate/__init__.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 ginormal-0.0.5/src/intermediate/_dg1.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ginormal-0.0.5/src/intermediate/_msh.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 ginormal-0.0.5/src/intermediate/_pbd.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 ginormal-0.0.5/src/intermediate/_rtg1.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ginormal-0.0.5/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ginormal-0.0.5/LICENSE.md
+-rw-r--r--   0        0        0     8518 2020-02-02 00:00:00.000000 ginormal-0.0.5/README.md
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 ginormal-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     9377 2020-02-02 00:00:00.000000 ginormal-0.0.5/PKG-INFO
```

### Comparing `ginormal-0.0.4/src/ginormal/__init__.py` & `ginormal-0.0.5/src/ginormal/__init__.py`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.4/src/ginormal/example.py` & `ginormal-0.0.5/src/ginormal/example.py`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.4/src/ginormal/main.py` & `ginormal-0.0.5/src/ginormal/main.py`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.4/src/intermediate/_F0g.py` & `ginormal-0.0.5/src/intermediate/_F0g.py`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.4/src/intermediate/_dg1.py` & `ginormal-0.0.5/src/intermediate/_dg1.py`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.4/src/intermediate/_rtg1.py` & `ginormal-0.0.5/src/intermediate/_rtg1.py`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.4/README.md` & `ginormal-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-![Density and draws from GIN(5,0,1) distribution](/static/GIN.png?raw=true "Density and draws from GIN(5,0,1) distribution")
-
 # Generalized Inverse Normal distribution
 The `ginormal` package provides the density function and random variable generation from the generalized inverse normal (GIN) distribution introduced by [Robert (1991)](#2). The GIN distribution is a way to generalize the distribution of the reciprocal of a normal random variable. That is, the distribution generalizes the distribution of the random variable $Z = 1/X$ where $X \sim \text{Normal}(\mu, \sigma^2)$. This distribution is *different* from the generalized inverse Gaussian (GIG) distribution [(Jørgensen, 2012)](#3) despite the similarities in naming (see [below](#digression)).
 
 The GIN distribution is supported on the entire real line $z \in (-\infty, \infty)$ and takes three parameters:
 - $\alpha > 1$, a degrees-of-freedom parameter,
 - $\mu \in (-\infty, \infty)$, similar to a location parameter, it shifts the density of the distribution left and right,
 - $\tau > 0$, similar to a scale parameter, it spreads the density of the distribution.
```

### Comparing `ginormal-0.0.4/pyproject.toml` & `ginormal-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 # Package metadata
 [project]
 name = "ginormal"
-version = "0.0.4"
+version = "0.0.5"
 requires-python = ">=3.8"
 description = "Generalized Inverse Normal distribution density and generation"
 readme = "README.md"
 authors = [
   { name = "Santiago Montoya-Blandón", email = "Santiago.Montoya-Blandon@glasgow.ac.uk" },
   { name = "Cheng Ding", email = "cheng.ding.emory@gmail.com"},
   { name = "Juan Estrada", email = "jjestra@emory.edu"},
```

### Comparing `ginormal-0.0.4/PKG-INFO` & `ginormal-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ginormal
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generalized Inverse Normal distribution density and generation
 Project-URL: Homepage, https://github.com/smonto2/GIN
 Project-URL: Bug tracking, https://github.com/smonto2/GIN/issues
 Author-email: Santiago Montoya-Blandón <Santiago.Montoya-Blandon@glasgow.ac.uk>, Cheng Ding <cheng.ding.emory@gmail.com>, Juan Estrada <jjestra@emory.edu>, Zhilang Xia <zhilang.xia@glasgow.ac.uk>
 Maintainer-email: Santiago Montoya-Blandón <Santiago.Montoya-Blandon@glasgow.ac.uk>
 License-File: LICENSE.md
 Keywords: distribution,generalized inverse normal,random variable generation,statistics
@@ -13,16 +13,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Requires-Dist: cardano-method
 Requires-Dist: numpy
 Requires-Dist: scipy
 Description-Content-Type: text/markdown
 
-![Density and draws from GIN(5,0,1) distribution](/static/GIN.png?raw=true "Density and draws from GIN(5,0,1) distribution")
-
 # Generalized Inverse Normal distribution
 The `ginormal` package provides the density function and random variable generation from the generalized inverse normal (GIN) distribution introduced by [Robert (1991)](#2). The GIN distribution is a way to generalize the distribution of the reciprocal of a normal random variable. That is, the distribution generalizes the distribution of the random variable $Z = 1/X$ where $X \sim \text{Normal}(\mu, \sigma^2)$. This distribution is *different* from the generalized inverse Gaussian (GIG) distribution [(Jørgensen, 2012)](#3) despite the similarities in naming (see [below](#digression)).
 
 The GIN distribution is supported on the entire real line $z \in (-\infty, \infty)$ and takes three parameters:
 - $\alpha > 1$, a degrees-of-freedom parameter,
 - $\mu \in (-\infty, \infty)$, similar to a location parameter, it shifts the density of the distribution left and right,
 - $\tau > 0$, similar to a scale parameter, it spreads the density of the distribution.
```

