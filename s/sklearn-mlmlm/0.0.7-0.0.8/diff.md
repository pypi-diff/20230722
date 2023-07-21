# Comparing `tmp/sklearn_mlmlm-0.0.7.tar.gz` & `tmp/sklearn_mlmlm-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_mlmlm-0.0.7.tar", last modified: Fri Jul 21 22:25:46 2023, max compression
+gzip compressed data, was "sklearn_mlmlm-0.0.8.tar", last modified: Fri Jul 21 22:36:56 2023, max compression
```

## Comparing `sklearn_mlmlm-0.0.7.tar` & `sklearn_mlmlm-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 22:25:46.356104 sklearn_mlmlm-0.0.7/
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     1556 2023-07-04 20:07:57.000000 sklearn_mlmlm-0.0.7/LICENSE
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)       67 2023-07-21 22:23:16.000000 sklearn_mlmlm-0.0.7/MANIFEST.in
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)     1475 2023-07-21 22:25:46.356104 sklearn_mlmlm-0.0.7/PKG-INFO
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      650 2023-07-04 21:07:46.000000 sklearn_mlmlm-0.0.7/README.rst
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)       83 2023-07-21 21:12:25.000000 sklearn_mlmlm-0.0.7/requirements.txt
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      148 2023-07-21 22:25:46.356104 sklearn_mlmlm-0.0.7/setup.cfg
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     2016 2023-07-21 22:19:18.000000 sklearn_mlmlm-0.0.7/setup.py
-drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 22:25:46.356104 sklearn_mlmlm-0.0.7/sklearn_mlmlm.egg-info/
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)     1475 2023-07-21 22:25:46.000000 sklearn_mlmlm-0.0.7/sklearn_mlmlm.egg-info/PKG-INFO
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)      381 2023-07-21 22:25:46.000000 sklearn_mlmlm-0.0.7/sklearn_mlmlm.egg-info/SOURCES.txt
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        1 2023-07-21 22:25:46.000000 sklearn_mlmlm-0.0.7/sklearn_mlmlm.egg-info/dependency_links.txt
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        1 2023-07-21 22:24:14.000000 sklearn_mlmlm-0.0.7/sklearn_mlmlm.egg-info/not-zip-safe
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)      119 2023-07-21 22:25:46.000000 sklearn_mlmlm-0.0.7/sklearn_mlmlm.egg-info/requires.txt
--rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        1 2023-07-21 22:25:46.000000 sklearn_mlmlm-0.0.7/sklearn_mlmlm.egg-info/top_level.txt
-drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 22:25:46.346104 sklearn_mlmlm-0.0.7/src/
-drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 22:25:46.356104 sklearn_mlmlm-0.0.7/src/sklearn_mlmlm/
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      137 2023-07-04 20:12:01.000000 sklearn_mlmlm-0.0.7/src/sklearn_mlmlm/__init__.py
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)       21 2023-07-21 22:24:05.000000 sklearn_mlmlm-0.0.7/src/sklearn_mlmlm/_version.py
--rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     7858 2023-07-21 21:14:25.000000 sklearn_mlmlm-0.0.7/src/sklearn_mlmlm/sklearn_mlmlm.py
+drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 22:36:56.725717 sklearn_mlmlm-0.0.8/
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     1556 2023-07-04 20:07:57.000000 sklearn_mlmlm-0.0.8/LICENSE
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)       67 2023-07-21 22:23:16.000000 sklearn_mlmlm-0.0.8/MANIFEST.in
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)     1685 2023-07-21 22:36:56.725717 sklearn_mlmlm-0.0.8/PKG-INFO
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      650 2023-07-04 21:07:46.000000 sklearn_mlmlm-0.0.8/README.rst
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)      850 2023-07-21 22:35:46.000000 sklearn_mlmlm-0.0.8/pyproject.toml
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)       83 2023-07-21 21:12:25.000000 sklearn_mlmlm-0.0.8/requirements.txt
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)      148 2023-07-21 22:36:56.725717 sklearn_mlmlm-0.0.8/setup.cfg
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     1863 2023-07-21 22:36:48.000000 sklearn_mlmlm-0.0.8/setup.py
+drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 22:36:56.725717 sklearn_mlmlm-0.0.8/sklearn_mlmlm.egg-info/
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)     1685 2023-07-21 22:36:56.000000 sklearn_mlmlm-0.0.8/sklearn_mlmlm.egg-info/PKG-INFO
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)      366 2023-07-21 22:36:56.000000 sklearn_mlmlm-0.0.8/sklearn_mlmlm.egg-info/SOURCES.txt
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        1 2023-07-21 22:36:56.000000 sklearn_mlmlm-0.0.8/sklearn_mlmlm.egg-info/dependency_links.txt
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        1 2023-07-21 22:24:14.000000 sklearn_mlmlm-0.0.8/sklearn_mlmlm.egg-info/not-zip-safe
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)      119 2023-07-21 22:36:56.000000 sklearn_mlmlm-0.0.8/sklearn_mlmlm.egg-info/requires.txt
+-rw-r--r--   0 dfredriksen  (1000) dfredriksen  (1000)        1 2023-07-21 22:36:56.000000 sklearn_mlmlm-0.0.8/sklearn_mlmlm.egg-info/top_level.txt
+drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 22:36:56.715717 sklearn_mlmlm-0.0.8/src/
+drwxr-xr-x   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 22:36:56.725717 sklearn_mlmlm-0.0.8/src/sklearn_mlmlm/
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)        0 2023-07-21 22:33:13.000000 sklearn_mlmlm-0.0.8/src/sklearn_mlmlm/__init__.py
+-rwxrwxrwx   0 dfredriksen  (1000) dfredriksen  (1000)     7858 2023-07-21 21:14:25.000000 sklearn_mlmlm-0.0.8/src/sklearn_mlmlm/sklearn_mlmlm.py
```

### Comparing `sklearn_mlmlm-0.0.7/LICENSE` & `sklearn_mlmlm-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_mlmlm-0.0.7/PKG-INFO` & `sklearn_mlmlm-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: sklearn_mlmlm
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python and sklearn compatible implementation of ML-MLM.
 Home-page: https://github.com/quantyra/scikit-mlmlm
 Download-URL: https://github.com/quantyra/scikit-mlmlm
+Author-email: Daniel E Fredriksen <dfredriksen@quantyra.org>
 Maintainer: Daniel E Fredriksen
 Maintainer-email: dfredriksen@quantyra.org
 License: new BSD
+Project-URL: Homepage, https://github.com/quantyra/scikit-mlmlm
+Project-URL: Bug Tracker, https://github.com/quantyra/scikit-mlmlm/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
+Requires-Python: >=3.10
+Description-Content-Type: text/x-rst
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
-.. -*- mode: rst -*-
-
-.. |ReadTheDocs| image:: https://readthedocs.org/projects/scikit-mlmlm/badge/?version=latest
-.. _ReadTheDocs: https://scikit-mlmlm.readthedocs.io/en/latest/?badge=latest
-
-scikit-mlmlm - A python and sklearn compatible implementation of ML-MLM.
-========================================================================
-
-`scikit-mlmlm` is a Python and scikit-learn compatible implementation of Minimal Learning Machine - Multi Label Classifier, based on the Arxiv paper `Minimal Learning Machine for Multi-Label Learning <https://arxiv.org/abs/2305.05518>`_ and the GitHub repository https://github.com/jookriha/ml-mlm.
-
+.. -*- mode: rst -*-
+
+.. |ReadTheDocs| image:: https://readthedocs.org/projects/scikit-mlmlm/badge/?version=latest
+.. _ReadTheDocs: https://scikit-mlmlm.readthedocs.io/en/latest/?badge=latest
+
+scikit-mlmlm - A python and sklearn compatible implementation of ML-MLM.
+========================================================================
+
+`scikit-mlmlm` is a Python and scikit-learn compatible implementation of Minimal Learning Machine - Multi Label Classifier, based on the Arxiv paper `Minimal Learning Machine for Multi-Label Learning <https://arxiv.org/abs/2305.05518>`_ and the GitHub repository https://github.com/jookriha/ml-mlm.
+
```

### Comparing `sklearn_mlmlm-0.0.7/README.rst` & `sklearn_mlmlm-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `sklearn_mlmlm-0.0.7/setup.py` & `sklearn_mlmlm-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,29 +2,24 @@
 """A python and sklearn compatible implementation of ML-MLM."""
 
 import codecs
 import os
 
 from setuptools import find_packages, setup
 
-# get __version__ from _version.py
-ver_file = os.path.join('src', 'sklearn_mlmlm', '_version.py')
-with open(ver_file) as f:
-    exec(f.read())
-
 DISTNAME = 'sklearn_mlmlm'
 DESCRIPTION = 'A python and sklearn compatible implementation of ML-MLM.'
 with codecs.open('README.rst', encoding='utf-8-sig') as f:
     LONG_DESCRIPTION = f.read()
 MAINTAINER = 'Daniel E Fredriksen'
 MAINTAINER_EMAIL = 'dfredriksen@quantyra.org'
 URL = 'https://github.com/quantyra/scikit-mlmlm'
 LICENSE = 'new BSD'
 DOWNLOAD_URL = 'https://github.com/quantyra/scikit-mlmlm'
-VERSION = __version__
+VERSION = "0.0.8"
 INSTALL_REQUIRES = ['numpy', 'scipy', 'scikit-learn']
 CLASSIFIERS = ['Intended Audience :: Science/Research',
                'Programming Language :: Python',
                'Topic :: Software Development',
                'Topic :: Scientific/Engineering',
                'Operating System :: Microsoft :: Windows',
                'Operating System :: POSIX',
```

### Comparing `sklearn_mlmlm-0.0.7/sklearn_mlmlm.egg-info/PKG-INFO` & `sklearn_mlmlm-0.0.8/sklearn_mlmlm.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: sklearn-mlmlm
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python and sklearn compatible implementation of ML-MLM.
 Home-page: https://github.com/quantyra/scikit-mlmlm
 Download-URL: https://github.com/quantyra/scikit-mlmlm
+Author-email: Daniel E Fredriksen <dfredriksen@quantyra.org>
 Maintainer: Daniel E Fredriksen
 Maintainer-email: dfredriksen@quantyra.org
 License: new BSD
+Project-URL: Homepage, https://github.com/quantyra/scikit-mlmlm
+Project-URL: Bug Tracker, https://github.com/quantyra/scikit-mlmlm/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
+Requires-Python: >=3.10
+Description-Content-Type: text/x-rst
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
-.. -*- mode: rst -*-
-
-.. |ReadTheDocs| image:: https://readthedocs.org/projects/scikit-mlmlm/badge/?version=latest
-.. _ReadTheDocs: https://scikit-mlmlm.readthedocs.io/en/latest/?badge=latest
-
-scikit-mlmlm - A python and sklearn compatible implementation of ML-MLM.
-========================================================================
-
-`scikit-mlmlm` is a Python and scikit-learn compatible implementation of Minimal Learning Machine - Multi Label Classifier, based on the Arxiv paper `Minimal Learning Machine for Multi-Label Learning <https://arxiv.org/abs/2305.05518>`_ and the GitHub repository https://github.com/jookriha/ml-mlm.
-
+.. -*- mode: rst -*-
+
+.. |ReadTheDocs| image:: https://readthedocs.org/projects/scikit-mlmlm/badge/?version=latest
+.. _ReadTheDocs: https://scikit-mlmlm.readthedocs.io/en/latest/?badge=latest
+
+scikit-mlmlm - A python and sklearn compatible implementation of ML-MLM.
+========================================================================
+
+`scikit-mlmlm` is a Python and scikit-learn compatible implementation of Minimal Learning Machine - Multi Label Classifier, based on the Arxiv paper `Minimal Learning Machine for Multi-Label Learning <https://arxiv.org/abs/2305.05518>`_ and the GitHub repository https://github.com/jookriha/ml-mlm.
+
```

### Comparing `sklearn_mlmlm-0.0.7/src/sklearn_mlmlm/sklearn_mlmlm.py` & `sklearn_mlmlm-0.0.8/src/sklearn_mlmlm/sklearn_mlmlm.py`

 * *Files identical despite different names*

