# Comparing `tmp/baycomp-1.0.2.tar.gz` & `tmp/baycomp-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/baycomp-1.0.2.tar", last modified: Mon Dec  9 13:05:56 2019, max compression
+gzip compressed data, was "baycomp-1.0.3.tar", last modified: Sat Jul 22 15:51:21 2023, max compression
```

## Comparing `baycomp-1.0.2.tar` & `baycomp-1.0.3.tar`

### file list

```diff
@@ -1,43 +1,24 @@
-drwxr-xr-x   0 janez      (501) staff       (20)        0 2019-12-09 13:05:56.089164 baycomp-1.0.2/
--rw-r--r--   0 janez      (501) staff       (20)    16437 2018-02-08 23:05:18.000000 baycomp-1.0.2/.pylintrc
--rw-r--r--   0 janez      (501) staff       (20)     1090 2018-02-04 13:32:58.000000 baycomp-1.0.2/LICENSE
--rw-r--r--   0 janez      (501) staff       (20)     3926 2019-12-09 13:05:56.088208 baycomp-1.0.2/PKG-INFO
--rw-r--r--   0 janez      (501) staff       (20)     2719 2018-02-04 13:51:10.000000 baycomp-1.0.2/README.md
-drwxr-xr-x   0 janez      (501) staff       (20)        0 2019-12-09 13:05:56.056993 baycomp-1.0.2/baycomp/
--rw-r--r--   0 janez      (501) staff       (20)       81 2018-02-02 20:10:56.000000 baycomp-1.0.2/baycomp/__init__.py
--rw-r--r--   0 janez      (501) staff       (20)     3806 2018-02-02 12:20:25.000000 baycomp-1.0.2/baycomp/hierarchical-t-test.stan
--rw-r--r--   0 janez      (501) staff       (20)    18462 2019-12-09 11:49:25.000000 baycomp-1.0.2/baycomp/multiple.py
--rw-r--r--   0 janez      (501) staff       (20)     8682 2019-12-09 11:49:06.000000 baycomp-1.0.2/baycomp/single.py
--rw-r--r--   0 janez      (501) staff       (20)     2658 2019-12-09 11:48:42.000000 baycomp-1.0.2/baycomp/utils.py
-drwxr-xr-x   0 janez      (501) staff       (20)        0 2019-12-09 13:05:56.059720 baycomp-1.0.2/baycomp.egg-info/
--rw-r--r--   0 janez      (501) staff       (20)     3926 2019-12-09 13:05:56.000000 baycomp-1.0.2/baycomp.egg-info/PKG-INFO
--rw-r--r--   0 janez      (501) staff       (20)      700 2019-12-09 13:05:56.000000 baycomp-1.0.2/baycomp.egg-info/SOURCES.txt
--rw-r--r--   0 janez      (501) staff       (20)        1 2019-12-09 13:05:56.000000 baycomp-1.0.2/baycomp.egg-info/dependency_links.txt
--rw-r--r--   0 janez      (501) staff       (20)       46 2019-12-09 13:05:56.000000 baycomp-1.0.2/baycomp.egg-info/requires.txt
--rw-r--r--   0 janez      (501) staff       (20)       14 2019-12-09 13:05:56.000000 baycomp-1.0.2/baycomp.egg-info/top_level.txt
-drwxr-xr-x   0 janez      (501) staff       (20)        0 2019-12-09 13:05:56.073424 baycomp-1.0.2/docs/
--rw-r--r--   0 janez      (501) staff       (20)      604 2018-02-01 21:01:32.000000 baycomp-1.0.2/docs/Makefile
-drwxr-xr-x   0 janez      (501) staff       (20)        0 2019-12-09 13:05:56.080363 baycomp-1.0.2/docs/_static/
--rw-r--r--   0 janez      (501) staff       (20)    19464 2018-02-03 23:15:32.000000 baycomp-1.0.2/docs/_static/signedrank-histogram.png
--rw-r--r--   0 janez      (501) staff       (20)    62376 2018-02-03 22:09:05.000000 baycomp-1.0.2/docs/_static/signedrank.png
--rw-r--r--   0 janez      (501) staff       (20)    30342 2018-02-03 22:29:34.000000 baycomp-1.0.2/docs/_static/t-norope.svg
--rw-r--r--   0 janez      (501) staff       (20)    30342 2018-02-03 22:29:34.000000 baycomp-1.0.2/docs/_static/t.svg
--rw-r--r--   0 janez      (501) staff       (20)     3861 2018-02-03 23:16:58.000000 baycomp-1.0.2/docs/classes.rst
-drwxr-xr-x   0 janez      (501) staff       (20)        0 2019-12-09 13:05:56.083742 baycomp-1.0.2/docs/code/
--rw-r--r--   0 janez      (501) staff       (20)   198622 2018-01-27 10:03:35.000000 baycomp-1.0.2/docs/code/accuracies.txt
--rw-r--r--   0 janez      (501) staff       (20)     1739 2018-01-30 08:43:24.000000 baycomp-1.0.2/docs/code/data.py
--rw-r--r--   0 janez      (501) staff       (20)      872 2019-12-09 13:05:04.000000 baycomp-1.0.2/docs/code/demo.py
--rw-r--r--   0 janez      (501) staff       (20)     5641 2018-03-07 02:12:20.000000 baycomp-1.0.2/docs/conf.py
--rw-r--r--   0 janez      (501) staff       (20)     3618 2018-02-08 23:25:15.000000 baycomp-1.0.2/docs/functions.rst
--rw-r--r--   0 janez      (501) staff       (20)     2662 2018-02-08 22:28:44.000000 baycomp-1.0.2/docs/index.rst
--rw-r--r--   0 janez      (501) staff       (20)     6169 2019-12-09 10:04:20.000000 baycomp-1.0.2/docs/introduction.rst
--rw-r--r--   0 janez      (501) staff       (20)      811 2018-02-01 21:01:33.000000 baycomp-1.0.2/docs/make.bat
--rw-r--r--   0 janez      (501) staff       (20)     1457 2018-02-03 23:23:00.000000 baycomp-1.0.2/docs/posterior.rst
--rw-r--r--   0 janez      (501) staff       (20)       38 2019-12-09 13:05:56.089346 baycomp-1.0.2/setup.cfg
--rw-r--r--   0 janez      (501) staff       (20)      995 2019-12-09 13:04:48.000000 baycomp-1.0.2/setup.py
-drwxr-xr-x   0 janez      (501) staff       (20)        0 2019-12-09 13:05:56.087003 baycomp-1.0.2/tests/
--rw-r--r--   0 janez      (501) staff       (20)        0 2018-02-03 14:20:51.000000 baycomp-1.0.2/tests/__init__.py
--rw-r--r--   0 janez      (501) staff       (20)     7038 2019-12-09 11:40:35.000000 baycomp-1.0.2/tests/test_multiple.py
--rw-r--r--   0 janez      (501) staff       (20)     5573 2018-02-03 18:25:34.000000 baycomp-1.0.2/tests/test_single.py
--rw-r--r--   0 janez      (501) staff       (20)     1712 2019-12-09 11:43:19.000000 baycomp-1.0.2/tests/test_utils.py
--rw-r--r--   0 janez      (501) staff       (20)     1011 2018-02-03 15:02:47.000000 baycomp-1.0.2/tests/utils.py
+drwxr-xr-x   0 janez      (501) staff       (20)        0 2023-07-22 15:51:21.467083 baycomp-1.0.3/
+-rw-r--r--   0 janez      (501) staff       (20)     1090 2023-07-22 15:43:51.000000 baycomp-1.0.3/LICENSE
+-rw-r--r--   0 janez      (501) staff       (20)     3316 2023-07-22 15:51:21.466895 baycomp-1.0.3/PKG-INFO
+-rw-r--r--   0 janez      (501) staff       (20)     2719 2023-07-22 15:43:51.000000 baycomp-1.0.3/README.md
+drwxr-xr-x   0 janez      (501) staff       (20)        0 2023-07-22 15:51:21.464958 baycomp-1.0.3/baycomp/
+-rw-r--r--   0 janez      (501) staff       (20)       81 2023-07-22 15:43:51.000000 baycomp-1.0.3/baycomp/__init__.py
+-rw-r--r--   0 janez      (501) staff       (20)     3789 2023-07-22 15:43:54.000000 baycomp-1.0.3/baycomp/hierarchical-t-test.stan
+-rw-r--r--   0 janez      (501) staff       (20)    18647 2023-07-22 15:43:54.000000 baycomp-1.0.3/baycomp/multiple.py
+-rw-r--r--   0 janez      (501) staff       (20)     8682 2023-07-22 15:43:51.000000 baycomp-1.0.3/baycomp/single.py
+-rw-r--r--   0 janez      (501) staff       (20)     2658 2023-07-22 15:43:51.000000 baycomp-1.0.3/baycomp/utils.py
+drwxr-xr-x   0 janez      (501) staff       (20)        0 2023-07-22 15:51:21.465851 baycomp-1.0.3/baycomp.egg-info/
+-rw-r--r--   0 janez      (501) staff       (20)     3316 2023-07-22 15:51:21.000000 baycomp-1.0.3/baycomp.egg-info/PKG-INFO
+-rw-r--r--   0 janez      (501) staff       (20)      385 2023-07-22 15:51:21.000000 baycomp-1.0.3/baycomp.egg-info/SOURCES.txt
+-rw-r--r--   0 janez      (501) staff       (20)        1 2023-07-22 15:51:21.000000 baycomp-1.0.3/baycomp.egg-info/dependency_links.txt
+-rw-r--r--   0 janez      (501) staff       (20)       46 2023-07-22 15:51:21.000000 baycomp-1.0.3/baycomp.egg-info/requires.txt
+-rw-r--r--   0 janez      (501) staff       (20)       14 2023-07-22 15:51:21.000000 baycomp-1.0.3/baycomp.egg-info/top_level.txt
+-rw-r--r--   0 janez      (501) staff       (20)       38 2023-07-22 15:51:21.467134 baycomp-1.0.3/setup.cfg
+-rw-r--r--   0 janez      (501) staff       (20)     1049 2023-07-22 15:51:09.000000 baycomp-1.0.3/setup.py
+drwxr-xr-x   0 janez      (501) staff       (20)        0 2023-07-22 15:51:21.466657 baycomp-1.0.3/tests/
+-rw-r--r--   0 janez      (501) staff       (20)        0 2023-07-22 15:43:51.000000 baycomp-1.0.3/tests/__init__.py
+-rw-r--r--   0 janez      (501) staff       (20)     7070 2023-07-22 15:43:54.000000 baycomp-1.0.3/tests/test_multiple.py
+-rw-r--r--   0 janez      (501) staff       (20)     5573 2023-07-22 15:43:51.000000 baycomp-1.0.3/tests/test_single.py
+-rw-r--r--   0 janez      (501) staff       (20)     1712 2023-07-22 15:43:51.000000 baycomp-1.0.3/tests/test_utils.py
+-rw-r--r--   0 janez      (501) staff       (20)     1011 2023-07-22 15:43:51.000000 baycomp-1.0.3/tests/utils.py
```

### Comparing `baycomp-1.0.2/LICENSE` & `baycomp-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `baycomp-1.0.2/PKG-INFO` & `baycomp-1.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,73 @@
-Metadata-Version: 2.1
-Name: baycomp
-Version: 1.0.2
-Summary: Bayesian tests for comparison of classifiers
-Home-page: https://github.com/janezd/baycomp.git
-Author: J. Demsar, A. Benavoli, G. Corani
-Author-email: janez.demsar@fri.uni-lj.si
-License: UNKNOWN
-Description: baycomp
-        =======
-        
-        Baycomp is a library for Bayesian comparison of classifiers.
-        
-        Functions compare two classifiers on one or on multiple data sets. They
-        compute three probabilities: the probability that the first classifier has
-        higher scores than the second, the probability that differences are within
-        the region of practical equivalence (rope), or that the second classifier
-        has higher scores. We will refer to this probabilities as `p_left`, `p_rope`
-        and `p_right`. If the argument `rope` is omitted (or set to zero), functions
-        return only `p_left` and `p_right`.
-        
-        The region of practical equivalence (rope) is specified by the caller and
-        should correspond to what is "equivalent" in practice; for instance,
-        classification accuracies that differ by less than 0.5 may be called
-        equivalent.
-        
-        Similarly, whether higher scores are better or worse depends upon the type
-        of the score.
-        
-        The library can also plot the posterior distributions.
-        
-        The library can be used in three ways.
-        
-        1. Two shortcut functions can be used for comparison on single
-           and on multiple data sets. If `nbc` and `j48` contain a list of average
-           classification accuracies of naive Bayesian classifier and J48 on a
-           collection of data sets, we can call
-        
-                >>> two_on_multiple(nbc, j48, rope=1)
-                (0.23124, 0.00666, 0.7621)
-        
-           (Actual results may differ due to Monte Carlo sampling.)
-        
-           With some additional arguments, the function can also plot the posterior
-           distribution from which these probabilities came.
-        
-        2. Tests are packed into test classes. The above call is equivalent to
-        
-                >>> SignedRankTest.probs(nbc, j48, rope=1)
-                (0.23124, 0.00666, 0.7621)
-        
-           and to get a plot, we call
-        
-                >>> SignedRankTest.plot(nbc, j48, rope=1, names=("nbc", "j48"))
-        
-           To switch to another test, use another class::
-        
-                >>> SignTest.probs(nbc, j48, rope=1)
-                (0.26508, 0.13274, 0.60218)
-        
-        3. Finally, we can construct and query sampled posterior distributions.
-        
-                >>> posterior = SignedRankTest(nbc, j48, rope=0.5)
-                >>> posterior.probs()
-                (0.23124, 0.00666, 0.7621)
-                >>> posterior.plot(names=("nbc", "j48"))
-        
-        Installation
-        ------------
-        
-        Install from [PyPI](https://pypi.python.org/pypi/baycomp):
-        
-            pip install baycomp
-        
-        Documentation
-        -------------
-        
-        User documentation is available on [https://baycomp.readthedocs.io/](https://baycomp.readthedocs.io/).
-        
-        
-        A detailed description of the implemented methods is available in [Time for a Change: a Tutorial for Comparing Multiple Classifiers Through Bayesian Analysis](http://jmlr.org/papers/volume18/16-305/16-305.pdf), Alessio Benavoli, Giorgio Corani, Janez Demšar, Marco Zaffalon. Journal of Machine Learning Research, 18 (2017) 1-36.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3
-Description-Content-Type: text/markdown
+baycomp
+=======
+
+Baycomp is a library for Bayesian comparison of classifiers.
+
+Functions compare two classifiers on one or on multiple data sets. They
+compute three probabilities: the probability that the first classifier has
+higher scores than the second, the probability that differences are within
+the region of practical equivalence (rope), or that the second classifier
+has higher scores. We will refer to this probabilities as `p_left`, `p_rope`
+and `p_right`. If the argument `rope` is omitted (or set to zero), functions
+return only `p_left` and `p_right`.
+
+The region of practical equivalence (rope) is specified by the caller and
+should correspond to what is "equivalent" in practice; for instance,
+classification accuracies that differ by less than 0.5 may be called
+equivalent.
+
+Similarly, whether higher scores are better or worse depends upon the type
+of the score.
+
+The library can also plot the posterior distributions.
+
+The library can be used in three ways.
+
+1. Two shortcut functions can be used for comparison on single
+   and on multiple data sets. If `nbc` and `j48` contain a list of average
+   classification accuracies of naive Bayesian classifier and J48 on a
+   collection of data sets, we can call
+
+        >>> two_on_multiple(nbc, j48, rope=1)
+        (0.23124, 0.00666, 0.7621)
+
+   (Actual results may differ due to Monte Carlo sampling.)
+
+   With some additional arguments, the function can also plot the posterior
+   distribution from which these probabilities came.
+
+2. Tests are packed into test classes. The above call is equivalent to
+
+        >>> SignedRankTest.probs(nbc, j48, rope=1)
+        (0.23124, 0.00666, 0.7621)
+
+   and to get a plot, we call
+
+        >>> SignedRankTest.plot(nbc, j48, rope=1, names=("nbc", "j48"))
+
+   To switch to another test, use another class::
+
+        >>> SignTest.probs(nbc, j48, rope=1)
+        (0.26508, 0.13274, 0.60218)
+
+3. Finally, we can construct and query sampled posterior distributions.
+
+        >>> posterior = SignedRankTest(nbc, j48, rope=0.5)
+        >>> posterior.probs()
+        (0.23124, 0.00666, 0.7621)
+        >>> posterior.plot(names=("nbc", "j48"))
+
+Installation
+------------
+
+Install from [PyPI](https://pypi.python.org/pypi/baycomp):
+
+    pip install baycomp
+
+Documentation
+-------------
+
+User documentation is available on [https://baycomp.readthedocs.io/](https://baycomp.readthedocs.io/).
+
+
+A detailed description of the implemented methods is available in [Time for a Change: a Tutorial for Comparing Multiple Classifiers Through Bayesian Analysis](http://jmlr.org/papers/volume18/16-305/16-305.pdf), Alessio Benavoli, Giorgio Corani, Janez Demšar, Marco Zaffalon. Journal of Machine Learning Research, 18 (2017) 1-36.
```

### Comparing `baycomp-1.0.2/README.md` & `baycomp-1.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: baycomp
+Version: 1.0.3
+Summary: Bayesian tests for comparison of classifiers
+Home-page: https://github.com/janezd/baycomp.git
+Author: J. Demsar, A. Benavoli, G. Corani
+Author-email: janez.demsar@fri.uni-lj.si
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 baycomp
 =======
 
 Baycomp is a library for Bayesian comparison of classifiers.
 
 Functions compare two classifiers on one or on multiple data sets. They
 compute three probabilities: the probability that the first classifier has
```

### Comparing `baycomp-1.0.2/baycomp/hierarchical-t-test.stan` & `baycomp-1.0.3/baycomp/hierarchical-t-test.stan`

 * *Files 5% similar despite different names*

```diff
@@ -45,30 +45,30 @@
 
     /* M is the correlation matrix of the mvn noise.
     invM is its inverse, detM its determinant */
     matrix[Nsamples,Nsamples] invM;
     real detM;
 
     //The determinant of M is analytically known
-    detM <- (1+(Nsamples-1)*rho)*(1-rho)^(Nsamples-1);
+    detM = (1+(Nsamples-1)*rho)*(1-rho)^(Nsamples-1);
 
     //build H and invM. They do not depend on the data.
     for (j in 1:Nsamples){
-      zeroMeanVec[j]<-0;
-      H[j]<-1;
+      zeroMeanVec[j] = 0;
+      H[j] = 1;
       for (i in 1:Nsamples){
         if (j==i)
-          invM[j,i]<- (1 + (Nsamples-2)*rho)*pow((1-rho),Nsamples-2);
+          invM[j,i] = (1 + (Nsamples-2)*rho)*pow((1-rho),Nsamples-2);
         else
-          invM[j,i]<- -rho * pow((1-rho),Nsamples-2);
+          invM[j,i] = -rho * pow((1-rho),Nsamples-2);
         }
     }
     /*at this point invM contains the adjugate of M.
     we  divide it by det(M) to obtain the inverse of M.*/
-    invM <-invM/detM;
+    invM = invM/detM;
   }
 
   parameters {
     //mean of the  hyperprior from which we sample the delta_i
     real<lower=deltaLow,upper=deltaHi> delta0;
 
     //std of the hyperprior from which we sample the delta_i
@@ -105,29 +105,29 @@
     vector[q] oneOverSigma2;
 
     vector[q] logDetSigma;
 
     vector[q] logLik;
 
     //degrees of freedom
-    nu <- nuMinusOne + 1 ;
+    nu = nuMinusOne + 1 ;
 
     //1 over the variance of each data set
-    oneOverSigma2 <- rep_vector(1, q) ./ sigma;
-    oneOverSigma2 <- oneOverSigma2 ./ sigma;
+    oneOverSigma2 = rep_vector(1, q) ./ sigma;
+    oneOverSigma2 = oneOverSigma2 ./ sigma;
 
     /*the data (x) minus a matrix done as follows:
     the delta vector (of lenght q) pasted side by side Nsamples times*/
-    diff <- x - rep_matrix(delta,Nsamples);
+    diff = x - rep_matrix(delta,Nsamples);
 
     //efficient matrix computation of the likelihood.
-    diagQuad <- diagonal (quad_form (invM,diff'));
-    logDetSigma <- 2*Nsamples*log(sigma) + log(detM) ;
-    logLik <- -0.5 * logDetSigma - 0.5*Nsamples*log(6.283);
-    logLik <- logLik - 0.5 * oneOverSigma2 .* diagQuad;
+    diagQuad = diagonal (quad_form (invM,diff'));
+    logDetSigma = 2*Nsamples*log(sigma) + log(detM) ;
+    logLik = -0.5 * logDetSigma - 0.5*Nsamples*log(6.283);
+    logLik = logLik - 0.5 * oneOverSigma2 .* diagQuad;
 
   }
 
   model {
     /*mu0 and std0 are not explicitly sampled here.
     Stan automatically samples them: mu0 as uniform and std0 as
     uniform over its domain (std0Low,std0Hi).*/
@@ -135,9 +135,9 @@
     //sampling the degrees of freedom
     nuMinusOne ~ gamma ( gammaAlpha, gammaBeta);
 
     //vectorial sampling of the delta_i of each data set
     delta ~ student_t(nu, delta0, std0);
 
     //logLik is computed in the previous block
-    increment_log_prob(sum(logLik));
+    target += sum(logLik);
   }
```

### Comparing `baycomp-1.0.2/baycomp/multiple.py` & `baycomp-1.0.3/baycomp/multiple.py`

 * *Files 9% similar despite different names*

```diff
@@ -145,16 +145,16 @@
             ax.axvline(x=0.5, color="#ffad2f", linewidth=2)
             return fig
 
 
 class Test:
     LEFT, ROPE, RIGHT = range(3)
 
-    def __new__(cls, x, y, rope=0, *, nsamples=50000, **kwargs):
-        return Posterior(cls.sample(x, y, rope, nsamples=nsamples, **kwargs))
+    def __new__(cls, x, y, rope=0, *, nsamples=50000, random_state=None, **kwargs):
+        return Posterior(cls.sample(x, y, rope, nsamples=nsamples, random_state=random_state, **kwargs))
 
     @classmethod
     def sample(cls, x, y, rope=0, nsamples=50000, **kwargs):
         """
         Compute a sample of posterior distribution.
 
         Derived classes override this method to implement specific
@@ -264,29 +264,31 @@
     rope region, or a tuple with prior's position and strength, for instance
     `(SignTest.LEFT, 1.0)`. Position can be `SignTest.LEFT`, `SignTest.ROPE`
     or `SignTest.RIGHT`.
     """
 
     @classmethod
     # pylint: disable=arguments-differ
-    def sample(cls, x, y, rope=0, *, prior=1, nsamples=50000):
+    def sample(cls, x, y, rope=0, *, prior=1, nsamples=50000, random_state=None):
         if isinstance(prior, tuple):
             prior, prior_place = prior
         else:
             prior_place = cls.ROPE
         check_args(x, y, rope, prior, nsamples)
 
+        _random_state = np.random.RandomState(random_state)
+
         diff = y - x
         nleft = sum(diff < -rope)
         nright = sum(diff > rope)
         nrope = len(diff) - nleft - nright
         alpha = np.array([nleft, nrope, nright], dtype=float)
         alpha += 0.0001  # for numerical stability
         alpha[prior_place] += prior
-        return np.random.dirichlet(alpha, nsamples)
+        return _random_state.dirichlet(alpha, nsamples)
 
 
 class SignedRankTest(Test):
     """
     Compute a Bayesian signed-rank test
     (`A Bayesian Wilcoxon signed-rank test based on the Dirichlet process
     <http://proceedings.mlr.press/v32/benavoli14.pdf>`_,
@@ -295,15 +297,15 @@
     Arguments `x` and `y` should be one-dimensional arrays with average
     performances across data sets. These can be obtained using any sampling
     method, not necessarily cross validation.
     """
 
     @classmethod
     # pylint: disable=arguments-differ
-    def sample(cls, x, y, rope=0, *, prior=0.5, nsamples=50000):
+    def sample(cls, x, y, rope=0, *, prior=0.5, nsamples=50000, random_state=None):
         def heaviside(a, thresh):
             return (a > thresh).astype(float) + 0.5 * (a == thresh).astype(float)
 
         def diff_sums(x, y):
             diff = np.hstack(([0], y - x))
             diff_m = np.lib.stride_tricks.as_strided(
                 diff, strides=diff.strides + (0,), shape=diff.shape * 2)
@@ -312,26 +314,28 @@
             return diff_m + diff_m.T, weights
 
         def with_rope():
             sums, weights = diff_sums(x, y)
             above_rope = heaviside(sums, 2 * rope)
             below_rope = heaviside(-sums, 2 * rope)
             samples = np.zeros((nsamples, 3))
-            for i, samp_weights in enumerate(np.random.dirichlet(weights, nsamples)):
+            _random_state = np.random.RandomState(random_state)
+            for i, samp_weights in enumerate(_random_state.dirichlet(weights, nsamples)):
                 prod_weights = np.outer(samp_weights, samp_weights)
                 samples[i, 0] = np.sum(prod_weights * below_rope)
                 samples[i, 2] = np.sum(prod_weights * above_rope)
             samples[:, 1] = -samples[:, 0] - samples[:, 2] + 1
             return samples
 
         def without_rope():
             sums, weights = diff_sums(x, y)
             above_0 = heaviside(sums, 0)
             samples = np.zeros((nsamples, 3))
-            for i, samp_weights in enumerate(np.random.dirichlet(weights, nsamples)):
+            _random_state = np.random.RandomState(random_state)
+            for i, samp_weights in enumerate(_random_state.dirichlet(weights, nsamples)):
                 prod_weights = np.outer(samp_weights, samp_weights)
                 samples[i, 2] = np.sum(prod_weights * above_0)
             samples[:, 0] = -samples[:, 2] + 1
             return samples
 
         check_args(x, y, rope, nsamples)
         return with_rope() if rope > 0 else without_rope()
@@ -351,23 +355,25 @@
 
     @classmethod
     # pylint: disable=arguments-differ
     # pylint: disable=unused-argument
     def sample(cls, x, y, rope, *, runs=1,
                lower_alpha=1, upper_alpha=2,
                lower_beta=0.01, upper_beta=0.1,
-               upper_sigma=1000, chains=4, nsamples=None):
+               upper_sigma=1000, chains=4, nsamples=10000,
+               random_state=None):
         try:
-            import pystan
+            import stan
         except ImportError:
-            raise ImportError("Hierarchical model requires 'pystan'; "
-                              "install it by 'pip install pystan'")
+            raise ImportError("Hierarchical model requires 'pystan >= 3.4.0'; "
+                              "install it e.g. by 'pip install pystan==3.4.0'")
+
+        _random_state = np.random.RandomState(random_state)
 
         LAST_SAMPLE_PICKLE = "last-sample.pickle"
-        STAN_MODEL_PICKLE = "stored-stan-model.pickle"
         stan_file = os.path.join(os.path.split(__file__)[0], "hierarchical-t-test.stan")
 
         args_signature = (
             hash(tuple(tuple(e for e in row) for row in y - x)),
             runs, lower_alpha, upper_alpha, lower_beta, upper_beta, upper_sigma)
 
         def try_unpickle(fname):
@@ -395,15 +401,15 @@
             ndatasets, nscores = diff.shape
             nfolds = nscores / runs
 
             # avoid numerical problems with zero variance
             nscores_2 = nscores // 2
             for sample in diff:
                 if np.var(sample) == 0:
-                    sample[:nscores_2] = np.random.uniform(-rope, rope, nscores_2)
+                    sample[:nscores_2] = _random_state.uniform(-rope, rope, nscores_2)
                     sample[nscores_2:] = -sample[:nscores_2]
 
             std_within = np.mean(np.std(diff, axis=1))  # may be different from std_diff!
             std_among = np.std(np.mean(diff, axis=1)) if ndatasets > 1 else std_within
             maxdiff = np.max(np.abs(diff))
 
             return dict(
@@ -412,41 +418,34 @@
                 deltaLow=-maxdiff, deltaHi=maxdiff,
                 lowerAlpha=lower_alpha, upperAlpha=upper_alpha,
                 lowerBeta=lower_beta, upperBeta=upper_beta,
                 stdLow=0, stdHi=std_within * upper_sigma,
                 std0Low=0, std0Hi=std_among * upper_sigma
             )
 
-        def get_stan_model(model_file):
-            stan_model = try_unpickle(STAN_MODEL_PICKLE)
-            if stan_model is None:
-                model_code = open(model_file).read()
-                stan_model = pystan.StanModel(model_code=model_code)
-                try_pickle(stan_model, STAN_MODEL_PICKLE)
-            return stan_model
-
-        def run_stan(diff):
+        def run_stan(diff, **kwargs):
             stan_data = prepare_stan_data(diff)
 
             # check if the last pickled result can be reused
             cached = try_unpickle(LAST_SAMPLE_PICKLE)
             if cached is not None and cached[0] == args_signature:
                 return cached[1]
 
-            model = get_stan_model(stan_file)
-            fit = model.sampling(data=stan_data, chains=chains)
-            results = fit.extract(permuted=True)
-            mu = results["delta0"]
-            stdh = results["std0"]
-            nu = results["nu"]
+            program_code = open(stan_file).read()
+            model: stan.model.Model = stan.build(program_code, data=stan_data)
+            fit: stan.fit.Fit = model.sample(**kwargs)
+
+            mu = fit["delta0"][0]
+            stdh = fit["std0"][0]
+            nu = fit["nu"][0]
             try_pickle((args_signature, (mu, stdh, nu)), LAST_SAMPLE_PICKLE)
             return mu, stdh, nu
 
         rope, diff = scaled_data(x, y, rope)
-        mu, stdh, nu = run_stan(diff)
+        mu, stdh, nu = run_stan(diff, num_samples=nsamples, num_chains=chains)
         samples = np.empty((len(nu), 3))
         for mui, std, df, sample_row in zip(mu, stdh, nu, samples):
             sample_row[2] = 1 - stats.t.cdf(rope, df, mui, std)
             sample_row[0] = stats.t.cdf(-rope, df, mui, std)
             sample_row[1] = 1 - sample_row[0] - sample_row[2]
         return samples
 
@@ -468,14 +467,15 @@
         y (np.array): a vector of scores for the second model
         rope (float): the width of the region of practical equivalence (default: 0)
         runs (int): the number of repetitions of cross validation
             (for hierarhical model) (default: 1)
         nsamples (int): the number of samples (default: 50000)
         plot (bool): if `True`, the function also return a histogram (default: False)
         names (tuple of str): names of classifiers (ignored if `plot` is `False`)
+        random_state (int or None): random seed for drawing the samples, if None a random seed is picked
 
     Returns:
         `(p_left, p_rope, p_right)` if `rope > 0`; otherwise `(p_left, p_right)`.
 
         If `plot=True`, the function also returns a matplotlib figure,
         that is, `((p_left, p_rope, p_right), fig)`
         """
```

### Comparing `baycomp-1.0.2/baycomp/single.py` & `baycomp-1.0.3/baycomp/single.py`

 * *Files identical despite different names*

### Comparing `baycomp-1.0.2/baycomp/utils.py` & `baycomp-1.0.3/baycomp/utils.py`

 * *Files identical despite different names*

### Comparing `baycomp-1.0.2/baycomp.egg-info/PKG-INFO` & `baycomp-1.0.3/baycomp.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,90 +1,89 @@
 Metadata-Version: 2.1
 Name: baycomp
-Version: 1.0.2
+Version: 1.0.3
 Summary: Bayesian tests for comparison of classifiers
 Home-page: https://github.com/janezd/baycomp.git
 Author: J. Demsar, A. Benavoli, G. Corani
 Author-email: janez.demsar@fri.uni-lj.si
-License: UNKNOWN
-Description: baycomp
-        =======
-        
-        Baycomp is a library for Bayesian comparison of classifiers.
-        
-        Functions compare two classifiers on one or on multiple data sets. They
-        compute three probabilities: the probability that the first classifier has
-        higher scores than the second, the probability that differences are within
-        the region of practical equivalence (rope), or that the second classifier
-        has higher scores. We will refer to this probabilities as `p_left`, `p_rope`
-        and `p_right`. If the argument `rope` is omitted (or set to zero), functions
-        return only `p_left` and `p_right`.
-        
-        The region of practical equivalence (rope) is specified by the caller and
-        should correspond to what is "equivalent" in practice; for instance,
-        classification accuracies that differ by less than 0.5 may be called
-        equivalent.
-        
-        Similarly, whether higher scores are better or worse depends upon the type
-        of the score.
-        
-        The library can also plot the posterior distributions.
-        
-        The library can be used in three ways.
-        
-        1. Two shortcut functions can be used for comparison on single
-           and on multiple data sets. If `nbc` and `j48` contain a list of average
-           classification accuracies of naive Bayesian classifier and J48 on a
-           collection of data sets, we can call
-        
-                >>> two_on_multiple(nbc, j48, rope=1)
-                (0.23124, 0.00666, 0.7621)
-        
-           (Actual results may differ due to Monte Carlo sampling.)
-        
-           With some additional arguments, the function can also plot the posterior
-           distribution from which these probabilities came.
-        
-        2. Tests are packed into test classes. The above call is equivalent to
-        
-                >>> SignedRankTest.probs(nbc, j48, rope=1)
-                (0.23124, 0.00666, 0.7621)
-        
-           and to get a plot, we call
-        
-                >>> SignedRankTest.plot(nbc, j48, rope=1, names=("nbc", "j48"))
-        
-           To switch to another test, use another class::
-        
-                >>> SignTest.probs(nbc, j48, rope=1)
-                (0.26508, 0.13274, 0.60218)
-        
-        3. Finally, we can construct and query sampled posterior distributions.
-        
-                >>> posterior = SignedRankTest(nbc, j48, rope=0.5)
-                >>> posterior.probs()
-                (0.23124, 0.00666, 0.7621)
-                >>> posterior.plot(names=("nbc", "j48"))
-        
-        Installation
-        ------------
-        
-        Install from [PyPI](https://pypi.python.org/pypi/baycomp):
-        
-            pip install baycomp
-        
-        Documentation
-        -------------
-        
-        User documentation is available on [https://baycomp.readthedocs.io/](https://baycomp.readthedocs.io/).
-        
-        
-        A detailed description of the implemented methods is available in [Time for a Change: a Tutorial for Comparing Multiple Classifiers Through Bayesian Analysis](http://jmlr.org/papers/volume18/16-305/16-305.pdf), Alessio Benavoli, Giorgio Corani, Janez Demšar, Marco Zaffalon. Journal of Machine Learning Research, 18 (2017) 1-36.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+baycomp
+=======
+
+Baycomp is a library for Bayesian comparison of classifiers.
+
+Functions compare two classifiers on one or on multiple data sets. They
+compute three probabilities: the probability that the first classifier has
+higher scores than the second, the probability that differences are within
+the region of practical equivalence (rope), or that the second classifier
+has higher scores. We will refer to this probabilities as `p_left`, `p_rope`
+and `p_right`. If the argument `rope` is omitted (or set to zero), functions
+return only `p_left` and `p_right`.
+
+The region of practical equivalence (rope) is specified by the caller and
+should correspond to what is "equivalent" in practice; for instance,
+classification accuracies that differ by less than 0.5 may be called
+equivalent.
+
+Similarly, whether higher scores are better or worse depends upon the type
+of the score.
+
+The library can also plot the posterior distributions.
+
+The library can be used in three ways.
+
+1. Two shortcut functions can be used for comparison on single
+   and on multiple data sets. If `nbc` and `j48` contain a list of average
+   classification accuracies of naive Bayesian classifier and J48 on a
+   collection of data sets, we can call
+
+        >>> two_on_multiple(nbc, j48, rope=1)
+        (0.23124, 0.00666, 0.7621)
+
+   (Actual results may differ due to Monte Carlo sampling.)
+
+   With some additional arguments, the function can also plot the posterior
+   distribution from which these probabilities came.
+
+2. Tests are packed into test classes. The above call is equivalent to
+
+        >>> SignedRankTest.probs(nbc, j48, rope=1)
+        (0.23124, 0.00666, 0.7621)
+
+   and to get a plot, we call
+
+        >>> SignedRankTest.plot(nbc, j48, rope=1, names=("nbc", "j48"))
+
+   To switch to another test, use another class::
+
+        >>> SignTest.probs(nbc, j48, rope=1)
+        (0.26508, 0.13274, 0.60218)
+
+3. Finally, we can construct and query sampled posterior distributions.
+
+        >>> posterior = SignedRankTest(nbc, j48, rope=0.5)
+        >>> posterior.probs()
+        (0.23124, 0.00666, 0.7621)
+        >>> posterior.plot(names=("nbc", "j48"))
+
+Installation
+------------
+
+Install from [PyPI](https://pypi.python.org/pypi/baycomp):
+
+    pip install baycomp
+
+Documentation
+-------------
+
+User documentation is available on [https://baycomp.readthedocs.io/](https://baycomp.readthedocs.io/).
+
+
+A detailed description of the implemented methods is available in [Time for a Change: a Tutorial for Comparing Multiple Classifiers Through Bayesian Analysis](http://jmlr.org/papers/volume18/16-305/16-305.pdf), Alessio Benavoli, Giorgio Corani, Janez Demšar, Marco Zaffalon. Journal of Machine Learning Research, 18 (2017) 1-36.
```

### Comparing `baycomp-1.0.2/setup.py` & `baycomp-1.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setup(
     name='baycomp',
-    version='1.0.2',
+    version='1.0.3',
     url='https://github.com/janezd/baycomp.git',
     author='J. Demsar, A. Benavoli, G. Corani',
     author_email='janez.demsar@fri.uni-lj.si',
     description='Bayesian tests for comparison of classifiers',
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
@@ -20,11 +20,14 @@
         'Programming Language :: Python :: 3'
     ],
     packages=find_packages(),
     install_requires=[
         'matplotlib >= 2.1.2',
         'numpy >= 1.13.1',
         'scipy >= 0.19.1'],
+    extra_requires=[
+        'pystan >= 3.4.0'
+    ],
     python_requires='>=3',
     package_data={
         'baycomp': ['hierarchical-t-test.stan']}
 )
```

### Comparing `baycomp-1.0.2/tests/test_multiple.py` & `baycomp-1.0.3/tests/test_multiple.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 class TestTest(TestTestBase):
     @patch.object(Test, "sample", return_value=Mock())
     @patch("baycomp.multiple.Posterior")
     def test_new(self, mockposterior, mocksample):
         x = np.array([4, 2, 6])
         y = np.array([5, 7, 3])
         Test(x, y, 1, nsamples=3, foo=42)
-        mocksample.assert_called_with(x, y, 1, nsamples=3, foo=42)
+        mocksample.assert_called_with(x, y, 1, nsamples=3, foo=42, random_state=None)
         mockposterior.assert_called_with(mocksample.return_value)
 
     def test_probs(self):
         x = np.array([4, 2, 6])
         y = np.array([5, 7, 3])
 
         self.assert_forwards(
@@ -104,22 +104,22 @@
             Test, "plot_histogram", x, y, nsamples=42, names=names,
             new_args=(x, y), new_kwargs=dict(nsamples=42, rope=0),
             meth_args=(names, )
         )
 
 
 class SignTestTest(unittest.TestCase):
-    @patch("numpy.random.dirichlet")
-    def test_sample(self, mockdirichlet):
+    @patch("numpy.random.RandomState")
+    def test_sample(self, mockrandomstate):
         x = np.array([15, 16, 17, 24, 11, 12, 13, 14])
         y = np.array([10, 13, 15, 24, 15, 82, 83, 84])
         # diff =      -5  -3  -2   0  4   70  70  70
 
         def assert_dirichlet(s, nsamples=50000):
-            alpha, ns = mockdirichlet.call_args[0]
+            alpha, ns = mockrandomstate.mock_calls[-1].args
             np.testing.assert_almost_equal(alpha, np.array(s) + 0.0001)
             self.assertEqual(ns, nsamples)
 
         SignTest.sample(x, y, prior=0)
         assert_dirichlet([3, 1, 4])
         SignTest.sample(x, y, prior=0, rope=1)
         assert_dirichlet([3, 1, 4])
```

### Comparing `baycomp-1.0.2/tests/test_single.py` & `baycomp-1.0.3/tests/test_single.py`

 * *Files identical despite different names*

### Comparing `baycomp-1.0.2/tests/test_utils.py` & `baycomp-1.0.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `baycomp-1.0.2/tests/utils.py` & `baycomp-1.0.3/tests/utils.py`

 * *Files identical despite different names*

