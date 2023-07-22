# Comparing `tmp/sklearn_mlmlm-0.0.8.tar.gz` & `tmp/sklearn_mlmlm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_mlmlm-0.0.8.tar", last modified: Fri Jul 21 22:36:56 2023, max compression
+gzip compressed data, was "sklearn_mlmlm-0.0.9.tar", max compression
```

## Comparing `sklearn_mlmlm-0.0.8.tar` & `sklearn_mlmlm-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,7 @@
-drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 22:36:56.725717 sklearn_mlmlm-0.0.8/
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     1556 2023-07-04 20:07:57.000000 sklearn_mlmlm-0.0.8/LICENSE
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)       67 2023-07-21 22:23:16.000000 sklearn_mlmlm-0.0.8/MANIFEST.in
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)     1685 2023-07-21 22:36:56.725717 sklearn_mlmlm-0.0.8/PKG-INFO
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      650 2023-07-04 21:07:46.000000 sklearn_mlmlm-0.0.8/README.rst
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)      850 2023-07-21 22:35:46.000000 sklearn_mlmlm-0.0.8/pyproject.toml
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)       83 2023-07-21 21:12:25.000000 sklearn_mlmlm-0.0.8/requirements.txt
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      148 2023-07-21 22:36:56.725717 sklearn_mlmlm-0.0.8/setup.cfg
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     1863 2023-07-21 22:36:48.000000 sklearn_mlmlm-0.0.8/setup.py
-drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 22:36:56.725717 sklearn_mlmlm-0.0.8/sklearn_mlmlm.egg-info/
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)     1685 2023-07-21 22:36:56.000000 sklearn_mlmlm-0.0.8/sklearn_mlmlm.egg-info/PKG-INFO
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)      366 2023-07-21 22:36:56.000000 sklearn_mlmlm-0.0.8/sklearn_mlmlm.egg-info/SOURCES.txt
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        1 2023-07-21 22:36:56.000000 sklearn_mlmlm-0.0.8/sklearn_mlmlm.egg-info/dependency_links.txt
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        1 2023-07-21 22:24:14.000000 sklearn_mlmlm-0.0.8/sklearn_mlmlm.egg-info/not-zip-safe
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)      119 2023-07-21 22:36:56.000000 sklearn_mlmlm-0.0.8/sklearn_mlmlm.egg-info/requires.txt
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        1 2023-07-21 22:36:56.000000 sklearn_mlmlm-0.0.8/sklearn_mlmlm.egg-info/top_level.txt
-drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 22:36:56.715717 sklearn_mlmlm-0.0.8/src/
-drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 22:36:56.725717 sklearn_mlmlm-0.0.8/src/sklearn_mlmlm/
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 22:33:13.000000 sklearn_mlmlm-0.0.8/src/sklearn_mlmlm/__init__.py
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     7858 2023-07-21 21:14:25.000000 sklearn_mlmlm-0.0.8/src/sklearn_mlmlm/sklearn_mlmlm.py
+-rwxr-xr-x   0        0        0     1556 2023-07-04 20:07:57.577077 sklearn_mlmlm-0.0.9/LICENSE
+-rwxr-xr-x   0        0        0      650 2023-07-04 21:07:46.633291 sklearn_mlmlm-0.0.9/README.rst
+-rw-r--r--   0        0        0     1006 2023-07-22 14:07:48.775033 sklearn_mlmlm-0.0.9/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-07-21 22:33:13.402509 sklearn_mlmlm-0.0.9/src/sklearn_mlmlm/__init__.py
+-rwxr-xr-x   0        0        0     7858 2023-07-21 21:14:25.759073 sklearn_mlmlm-0.0.9/src/sklearn_mlmlm/sklearn_mlmlm.py
+-rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 sklearn_mlmlm-0.0.9/setup.py
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 sklearn_mlmlm-0.0.9/PKG-INFO
```

### Comparing `sklearn_mlmlm-0.0.8/LICENSE` & `sklearn_mlmlm-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_mlmlm-0.0.8/README.rst` & `sklearn_mlmlm-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `sklearn_mlmlm-0.0.8/pyproject.toml` & `sklearn_mlmlm-0.0.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 [project]
+
+[tool.poetry]
 name = "sklearn_mlmlm"
-version = "0.0.8"
-authors = [
-  { name="Daniel E Fredriksen", email="dfredriksen@quantyra.org" },
-]
+version = "0.0.9"
+authors = ["Daniel E Fredriksen <dfredriksen@quantyra.org>"]
 description = "A python and sklearn compatible implementation of ML-MLM."
 readme = "README.rst"
-requires-python = ">=3.10"
 classifiers = [
     'Intended Audience :: Science/Research',
     'Programming Language :: Python',
     'Topic :: Software Development',
     'Topic :: Scientific/Engineering',
     'Operating System :: Microsoft :: Windows',
     'Operating System :: POSIX',
     'Operating System :: Unix',
     'Operating System :: MacOS',
     'Programming Language :: Python :: 3.10'
 ]
+packages = [{ include = "sklearn_mlmlm", from = "src" }]
+
+[tool.poetry.dependencies]
+python=">=3.10,<3.13"
+joblib = "^1.3.1"
+numpy = "^1.25.1"
+scikit-learn = "^1.3.0"
+scipy = "^1.11.1"
 
 [project.urls]
 "Homepage" = 'https://github.com/quantyra/scikit-mlmlm'
 "Bug Tracker" = 'https://github.com/quantyra/scikit-mlmlm/issues'
 
 [build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `sklearn_mlmlm-0.0.8/src/sklearn_mlmlm/sklearn_mlmlm.py` & `sklearn_mlmlm-0.0.9/src/sklearn_mlmlm/sklearn_mlmlm.py`

 * *Files identical despite different names*

