# Comparing `tmp/ramanspy-0.1.0.tar.gz` & `tmp/ramanspy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramanspy-0.1.0.tar", last modified: Wed Jul  5 18:49:54 2023, max compression
+gzip compressed data, was "ramanspy-0.1.1.tar", last modified: Sat Jul 22 09:17:07 2023, max compression
```

## Comparing `ramanspy-0.1.0.tar` & `ramanspy-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-05 18:49:54.806256 ramanspy-0.1.0/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1503 2023-06-26 11:18:57.000000 ramanspy-0.1.0/LICENSE
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       73 2023-06-30 18:02:25.000000 ramanspy-0.1.0/MANIFEST.in
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4783 2023-07-05 18:49:54.806150 ramanspy-0.1.0/PKG-INFO
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2335 2023-07-05 18:43:55.000000 ramanspy-0.1.0/README.md
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1118 2023-07-05 18:46:47.000000 ramanspy-0.1.0/pyproject.toml
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       38 2023-07-05 18:49:54.806301 ramanspy-0.1.0/setup.cfg
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-05 18:49:54.800274 ramanspy-0.1.0/src/
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-05 18:49:54.802301 ramanspy-0.1.0/src/ramanspy/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      471 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/__init__.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-05 18:49:54.803967 ramanspy-0.1.0/src/ramanspy/analysis/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3187 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/analysis/Step.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       85 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/analysis/__init__.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1035 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/analysis/cluster.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2284 2023-07-04 16:22:48.000000 ramanspy-0.1.0/src/ramanspy/analysis/decompose.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     7553 2023-07-04 18:23:45.000000 ramanspy-0.1.0/src/ramanspy/analysis/unmix.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    11990 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/core.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    18768 2023-06-30 17:54:47.000000 ramanspy-0.1.0/src/ramanspy/datasets.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    10385 2023-06-26 22:05:02.000000 ramanspy-0.1.0/src/ramanspy/load.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4974 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/metrics.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-05 18:49:54.804587 ramanspy-0.1.0/src/ramanspy/plot/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      196 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/plot/__init__.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     7777 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/plot/_core.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    25767 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/plot/plot.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-05 18:49:54.805953 ramanspy-0.1.0/src/ramanspy/preprocessing/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     5493 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/preprocessing/Pipeline.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4862 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/preprocessing/Step.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      262 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/preprocessing/__init__.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    16856 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/preprocessing/baseline.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4168 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/preprocessing/denoise.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2370 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/preprocessing/despike.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2138 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/preprocessing/misc.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3573 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/preprocessing/normalise.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3143 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/preprocessing/protocols.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      465 2023-06-26 22:05:02.000000 ramanspy-0.1.0/src/ramanspy/utils.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-05 18:49:54.803006 ramanspy-0.1.0/src/ramanspy.egg-info/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4783 2023-07-05 18:49:54.000000 ramanspy-0.1.0/src/ramanspy.egg-info/PKG-INFO
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      950 2023-07-05 18:49:54.000000 ramanspy-0.1.0/src/ramanspy.egg-info/SOURCES.txt
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        1 2023-07-05 18:49:54.000000 ramanspy-0.1.0/src/ramanspy.egg-info/dependency_links.txt
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       90 2023-07-05 18:49:54.000000 ramanspy-0.1.0/src/ramanspy.egg-info/requires.txt
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        9 2023-07-05 18:49:54.000000 ramanspy-0.1.0/src/ramanspy.egg-info/top_level.txt
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-22 09:17:07.041569 ramanspy-0.1.1/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1503 2023-06-26 11:18:57.000000 ramanspy-0.1.1/LICENSE
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       73 2023-06-30 18:02:25.000000 ramanspy-0.1.1/MANIFEST.in
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     5185 2023-07-22 09:17:07.041443 ramanspy-0.1.1/PKG-INFO
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2636 2023-07-22 09:14:26.000000 ramanspy-0.1.1/README.md
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1209 2023-07-22 09:15:54.000000 ramanspy-0.1.1/pyproject.toml
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       38 2023-07-22 09:17:07.041628 ramanspy-0.1.1/setup.cfg
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-22 09:17:07.035327 ramanspy-0.1.1/src/
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-22 09:17:07.037340 ramanspy-0.1.1/src/ramanspy/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      471 2023-06-26 11:18:57.000000 ramanspy-0.1.1/src/ramanspy/__init__.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-22 09:17:07.038790 ramanspy-0.1.1/src/ramanspy/analysis/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3187 2023-06-26 11:18:57.000000 ramanspy-0.1.1/src/ramanspy/analysis/Step.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       85 2023-06-26 11:18:57.000000 ramanspy-0.1.1/src/ramanspy/analysis/__init__.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1035 2023-06-26 11:18:57.000000 ramanspy-0.1.1/src/ramanspy/analysis/cluster.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2284 2023-07-04 16:22:48.000000 ramanspy-0.1.1/src/ramanspy/analysis/decompose.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     7553 2023-07-04 18:23:45.000000 ramanspy-0.1.1/src/ramanspy/analysis/unmix.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    11990 2023-06-26 11:18:57.000000 ramanspy-0.1.1/src/ramanspy/core.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    18768 2023-06-30 17:54:47.000000 ramanspy-0.1.1/src/ramanspy/datasets.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    10385 2023-06-26 22:05:02.000000 ramanspy-0.1.1/src/ramanspy/load.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4974 2023-06-26 11:18:57.000000 ramanspy-0.1.1/src/ramanspy/metrics.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-22 09:17:07.039414 ramanspy-0.1.1/src/ramanspy/plot/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      196 2023-06-26 11:18:57.000000 ramanspy-0.1.1/src/ramanspy/plot/__init__.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     7777 2023-06-26 11:18:57.000000 ramanspy-0.1.1/src/ramanspy/plot/_core.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    25767 2023-06-26 11:18:57.000000 ramanspy-0.1.1/src/ramanspy/plot/plot.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-22 09:17:07.041213 ramanspy-0.1.1/src/ramanspy/preprocessing/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     5493 2023-06-26 11:18:57.000000 ramanspy-0.1.1/src/ramanspy/preprocessing/Pipeline.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4862 2023-06-26 11:18:57.000000 ramanspy-0.1.1/src/ramanspy/preprocessing/Step.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      262 2023-06-26 11:18:57.000000 ramanspy-0.1.1/src/ramanspy/preprocessing/__init__.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    16856 2023-06-26 11:18:57.000000 ramanspy-0.1.1/src/ramanspy/preprocessing/baseline.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4168 2023-06-26 11:18:57.000000 ramanspy-0.1.1/src/ramanspy/preprocessing/denoise.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2370 2023-06-26 11:18:57.000000 ramanspy-0.1.1/src/ramanspy/preprocessing/despike.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2138 2023-06-26 11:18:57.000000 ramanspy-0.1.1/src/ramanspy/preprocessing/misc.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3573 2023-06-26 11:18:57.000000 ramanspy-0.1.1/src/ramanspy/preprocessing/normalise.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3143 2023-06-26 11:18:57.000000 ramanspy-0.1.1/src/ramanspy/preprocessing/protocols.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      465 2023-06-26 22:05:02.000000 ramanspy-0.1.1/src/ramanspy/utils.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-22 09:17:07.038018 ramanspy-0.1.1/src/ramanspy.egg-info/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     5185 2023-07-22 09:17:07.000000 ramanspy-0.1.1/src/ramanspy.egg-info/PKG-INFO
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      950 2023-07-22 09:17:07.000000 ramanspy-0.1.1/src/ramanspy.egg-info/SOURCES.txt
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        1 2023-07-22 09:17:07.000000 ramanspy-0.1.1/src/ramanspy.egg-info/dependency_links.txt
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       90 2023-07-22 09:17:07.000000 ramanspy-0.1.1/src/ramanspy.egg-info/requires.txt
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        9 2023-07-22 09:17:07.000000 ramanspy-0.1.1/src/ramanspy.egg-info/top_level.txt
```

### Comparing `ramanspy-0.1.0/LICENSE` & `ramanspy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ramanspy-0.1.0/PKG-INFO` & `ramanspy-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramanspy
-Version: 0.1.0
+Version: 0.1.1
 Summary: RamanSPy: An open-source Python package for integrative Raman spectroscopy data analysis
 Author-email: Dimitar Georgiev <d.georgiev21@imperial.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Dimitar Georgiev
         
         Redistribution and use in source and binary forms, with or without
@@ -30,24 +30,28 @@
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Documentation, https://ramanspy.readthedocs.io
 Project-URL: Source, https://github.com/barahona-research-group/RamanSPy
+Project-URL: Preprint, https://chemrxiv.org/engage/chemrxiv/article-details/64a53861ba3e99daef8c9c51
 Keywords: Raman spectroscopy,spectral analysis,chemometrics,preprocessing pipeline,artificial intelligence,machine learning,Python package
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RamanSPy
 
+[![Downloads](https://static.pepy.tech/badge/ramanspy)](https://pepy.tech/project/ramanspy)   [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)]([https://github.com/dwyl/esta/issues](https://github.com/barahona-research-group/RamanSPy/issues))
+
+
 *RamanSPy* is an open-source Python package for integrative
 Raman spectroscopy data analysis.
 
 ## Installation
 
 *RamanSPy* has been published on PyPI and can be installed
 via pip:
```

### Comparing `ramanspy-0.1.0/README.md` & `ramanspy-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # RamanSPy
 
+[![Downloads](https://static.pepy.tech/badge/ramanspy)](https://pepy.tech/project/ramanspy)   [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)]([https://github.com/dwyl/esta/issues](https://github.com/barahona-research-group/RamanSPy/issues))
+
+
 *RamanSPy* is an open-source Python package for integrative
 Raman spectroscopy data analysis.
 
 ## Installation
 
 *RamanSPy* has been published on PyPI and can be installed
 via pip:
```

### Comparing `ramanspy-0.1.0/pyproject.toml` & `ramanspy-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ramanspy"
-version = "0.1.0"
+version = "0.1.1"
 description = "RamanSPy: An open-source Python package for integrative Raman spectroscopy data analysis"
 readme = "README.md"
 authors = [{ name = "Dimitar Georgiev", email = "d.georgiev21@imperial.ac.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
@@ -33,16 +33,17 @@
     "pybaselines",
     "pysptools",
     "cvxopt",
     "renishawWiRE",
     "pandas",
     "wget",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 
 
 [project.urls]
 Documentation = "https://ramanspy.readthedocs.io"
 Source = "https://github.com/barahona-research-group/RamanSPy"
+Preprint = "https://chemrxiv.org/engage/chemrxiv/article-details/64a53861ba3e99daef8c9c51"
 
 [options.packages.find]
 where = "src"
```

### Comparing `ramanspy-0.1.0/src/ramanspy/analysis/Step.py` & `ramanspy-0.1.1/src/ramanspy/analysis/Step.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.1.0/src/ramanspy/analysis/cluster.py` & `ramanspy-0.1.1/src/ramanspy/analysis/cluster.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.1.0/src/ramanspy/analysis/decompose.py` & `ramanspy-0.1.1/src/ramanspy/analysis/decompose.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.1.0/src/ramanspy/analysis/unmix.py` & `ramanspy-0.1.1/src/ramanspy/analysis/unmix.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.1.0/src/ramanspy/core.py` & `ramanspy-0.1.1/src/ramanspy/core.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.1.0/src/ramanspy/datasets.py` & `ramanspy-0.1.1/src/ramanspy/datasets.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.1.0/src/ramanspy/load.py` & `ramanspy-0.1.1/src/ramanspy/load.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.1.0/src/ramanspy/metrics.py` & `ramanspy-0.1.1/src/ramanspy/metrics.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.1.0/src/ramanspy/plot/_core.py` & `ramanspy-0.1.1/src/ramanspy/plot/_core.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.1.0/src/ramanspy/plot/plot.py` & `ramanspy-0.1.1/src/ramanspy/plot/plot.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.1.0/src/ramanspy/preprocessing/Pipeline.py` & `ramanspy-0.1.1/src/ramanspy/preprocessing/Pipeline.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.1.0/src/ramanspy/preprocessing/Step.py` & `ramanspy-0.1.1/src/ramanspy/preprocessing/Step.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.1.0/src/ramanspy/preprocessing/baseline.py` & `ramanspy-0.1.1/src/ramanspy/preprocessing/baseline.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.1.0/src/ramanspy/preprocessing/denoise.py` & `ramanspy-0.1.1/src/ramanspy/preprocessing/denoise.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.1.0/src/ramanspy/preprocessing/despike.py` & `ramanspy-0.1.1/src/ramanspy/preprocessing/despike.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.1.0/src/ramanspy/preprocessing/misc.py` & `ramanspy-0.1.1/src/ramanspy/preprocessing/misc.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.1.0/src/ramanspy/preprocessing/normalise.py` & `ramanspy-0.1.1/src/ramanspy/preprocessing/normalise.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.1.0/src/ramanspy/preprocessing/protocols.py` & `ramanspy-0.1.1/src/ramanspy/preprocessing/protocols.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.1.0/src/ramanspy.egg-info/PKG-INFO` & `ramanspy-0.1.1/src/ramanspy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramanspy
-Version: 0.1.0
+Version: 0.1.1
 Summary: RamanSPy: An open-source Python package for integrative Raman spectroscopy data analysis
 Author-email: Dimitar Georgiev <d.georgiev21@imperial.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Dimitar Georgiev
         
         Redistribution and use in source and binary forms, with or without
@@ -30,24 +30,28 @@
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Documentation, https://ramanspy.readthedocs.io
 Project-URL: Source, https://github.com/barahona-research-group/RamanSPy
+Project-URL: Preprint, https://chemrxiv.org/engage/chemrxiv/article-details/64a53861ba3e99daef8c9c51
 Keywords: Raman spectroscopy,spectral analysis,chemometrics,preprocessing pipeline,artificial intelligence,machine learning,Python package
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RamanSPy
 
+[![Downloads](https://static.pepy.tech/badge/ramanspy)](https://pepy.tech/project/ramanspy)   [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)]([https://github.com/dwyl/esta/issues](https://github.com/barahona-research-group/RamanSPy/issues))
+
+
 *RamanSPy* is an open-source Python package for integrative
 Raman spectroscopy data analysis.
 
 ## Installation
 
 *RamanSPy* has been published on PyPI and can be installed
 via pip:
```

### Comparing `ramanspy-0.1.0/src/ramanspy.egg-info/SOURCES.txt` & `ramanspy-0.1.1/src/ramanspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

