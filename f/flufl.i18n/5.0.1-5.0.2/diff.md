# Comparing `tmp/flufl_i18n-5.0.1.tar.gz` & `tmp/flufl_i18n-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flufl_i18n-5.0.1.tar", last modified: Tue Jun 13 20:27:55 2023, max compression
+gzip compressed data, was "flufl_i18n-5.0.2.tar", last modified: Sat Jul 22 01:02:43 2023, max compression
```

## Comparing `flufl_i18n-5.0.1.tar` & `flufl_i18n-5.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      558 2023-06-13 20:27:30.440667 flufl_i18n-5.0.1/LICENSE
--rw-r--r--   0        0        0      909 2023-06-13 20:27:30.440667 flufl_i18n-5.0.1/README.rst
--rw-r--r--   0        0        0     1214 2023-06-13 20:27:30.440667 flufl_i18n-5.0.1/conftest.py
--rw-r--r--   0        0        0     5407 2023-06-13 20:27:30.440667 flufl_i18n-5.0.1/docs/NEWS.rst
--rw-r--r--   0        0        0        0 2023-06-13 20:27:30.463667 flufl_i18n-5.0.1/docs/__init__.py
--rw-r--r--   0        0        0      701 2023-06-13 20:27:30.440667 flufl_i18n-5.0.1/docs/apiref.rst
--rw-r--r--   0        0        0     6680 2023-06-13 20:27:30.440667 flufl_i18n-5.0.1/docs/conf.py
--rw-r--r--   0        0        0     1113 2023-06-13 20:27:30.440667 flufl_i18n-5.0.1/docs/expand.rst
--rw-r--r--   0        0        0     2301 2023-06-13 20:27:30.440667 flufl_i18n-5.0.1/docs/index.rst
--rw-r--r--   0        0        0     3290 2023-06-13 20:27:30.440667 flufl_i18n-5.0.1/docs/strategies.rst
--rw-r--r--   0        0        0    10901 2023-06-13 20:27:30.441666 flufl_i18n-5.0.1/docs/using.rst
--rw-r--r--   0        0        0     3455 2023-06-13 20:27:55.987905 flufl_i18n-5.0.1/pyproject.toml
--rw-r--r--   0        0        0     1005 2023-06-13 20:27:30.441666 flufl_i18n-5.0.1/src/flufl/i18n/__init__.py
--rw-r--r--   0        0        0    10234 2023-06-13 20:27:30.441666 flufl_i18n-5.0.1/src/flufl/i18n/_application.py
--rw-r--r--   0        0        0      806 2023-06-13 20:27:30.441666 flufl_i18n-5.0.1/src/flufl/i18n/_expand.py
--rw-r--r--   0        0        0     1053 2023-06-13 20:27:30.441666 flufl_i18n-5.0.1/src/flufl/i18n/_registry.py
--rw-r--r--   0        0        0     2371 2023-06-13 20:27:30.441666 flufl_i18n-5.0.1/src/flufl/i18n/_strategy.py
--rw-r--r--   0        0        0      770 2023-06-13 20:27:30.441666 flufl_i18n-5.0.1/src/flufl/i18n/_substitute.py
--rw-r--r--   0        0        0     2975 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/src/flufl/i18n/_translator.py
--rw-r--r--   0        0        0        0 2023-06-13 20:27:30.466667 flufl_i18n-5.0.1/src/flufl/i18n/py.typed
--rw-r--r--   0        0        0     4442 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/src/flufl/i18n/types.py
--rw-r--r--   0        0        0        0 2023-06-13 20:27:30.466667 flufl_i18n-5.0.1/test/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 20:27:30.466667 flufl_i18n-5.0.1/test/data/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 20:27:30.466667 flufl_i18n-5.0.1/test/data/messages/__init__.py
--rw-r--r--   0        0        0      506 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/test/data/messages/xx/LC_MESSAGES/flufl.mo
--rw-r--r--   0        0        0      673 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/test/data/messages/xx/LC_MESSAGES/flufl.po
--rw-r--r--   0        0        0      505 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/test/data/messages/yy/LC_MESSAGES/flufl.mo
--rw-r--r--   0        0        0      672 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/test/data/messages/yy/LC_MESSAGES/flufl.po
--rw-r--r--   0        0        0      370 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/test/test_application.py
--rw-r--r--   0        0        0      845 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/test/test_expand.py
--rw-r--r--   0        0        0      520 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/test/test_substitute.py
--rw-r--r--   0        0        0     3617 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/test/test_translator.py
--rw-r--r--   0        0        0      772 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/tox.ini
--rw-r--r--   0        0        0     2179 1970-01-01 00:00:00.000000 flufl_i18n-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0      558 2023-07-22 01:02:18.658783 flufl_i18n-5.0.2/LICENSE
+-rw-r--r--   0        0        0      909 2023-07-22 01:02:18.658783 flufl_i18n-5.0.2/README.rst
+-rw-r--r--   0        0        0     1214 2023-07-22 01:02:18.658783 flufl_i18n-5.0.2/conftest.py
+-rw-r--r--   0        0        0     5510 2023-07-22 01:02:18.658783 flufl_i18n-5.0.2/docs/NEWS.rst
+-rw-r--r--   0        0        0        0 2023-07-22 01:02:18.681783 flufl_i18n-5.0.2/docs/__init__.py
+-rw-r--r--   0        0        0      701 2023-07-22 01:02:18.658783 flufl_i18n-5.0.2/docs/apiref.rst
+-rw-r--r--   0        0        0     6682 2023-07-22 01:02:18.658783 flufl_i18n-5.0.2/docs/conf.py
+-rw-r--r--   0        0        0     1113 2023-07-22 01:02:18.658783 flufl_i18n-5.0.2/docs/expand.rst
+-rw-r--r--   0        0        0     2303 2023-07-22 01:02:18.658783 flufl_i18n-5.0.2/docs/index.rst
+-rw-r--r--   0        0        0     3443 2023-07-22 01:02:18.658783 flufl_i18n-5.0.2/docs/strategies.rst
+-rw-r--r--   0        0        0    10901 2023-07-22 01:02:18.659783 flufl_i18n-5.0.2/docs/using.rst
+-rw-r--r--   0        0        0     3455 2023-07-22 01:02:43.322473 flufl_i18n-5.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1005 2023-07-22 01:02:18.659783 flufl_i18n-5.0.2/src/flufl/i18n/__init__.py
+-rw-r--r--   0        0        0    10234 2023-07-22 01:02:18.659783 flufl_i18n-5.0.2/src/flufl/i18n/_application.py
+-rw-r--r--   0        0        0      806 2023-07-22 01:02:18.659783 flufl_i18n-5.0.2/src/flufl/i18n/_expand.py
+-rw-r--r--   0        0        0     1053 2023-07-22 01:02:18.659783 flufl_i18n-5.0.2/src/flufl/i18n/_registry.py
+-rw-r--r--   0        0        0     2371 2023-07-22 01:02:18.659783 flufl_i18n-5.0.2/src/flufl/i18n/_strategy.py
+-rw-r--r--   0        0        0      770 2023-07-22 01:02:18.659783 flufl_i18n-5.0.2/src/flufl/i18n/_substitute.py
+-rw-r--r--   0        0        0     2975 2023-07-22 01:02:18.659783 flufl_i18n-5.0.2/src/flufl/i18n/_translator.py
+-rw-r--r--   0        0        0        0 2023-07-22 01:02:18.682783 flufl_i18n-5.0.2/src/flufl/i18n/py.typed
+-rw-r--r--   0        0        0     4442 2023-07-22 01:02:18.659783 flufl_i18n-5.0.2/src/flufl/i18n/types.py
+-rw-r--r--   0        0        0        0 2023-07-22 01:02:18.682783 flufl_i18n-5.0.2/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-22 01:02:18.682783 flufl_i18n-5.0.2/test/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-22 01:02:18.682783 flufl_i18n-5.0.2/test/data/messages/__init__.py
+-rw-r--r--   0        0        0      506 2023-07-22 01:02:18.660783 flufl_i18n-5.0.2/test/data/messages/xx/LC_MESSAGES/flufl.mo
+-rw-r--r--   0        0        0      673 2023-07-22 01:02:18.660783 flufl_i18n-5.0.2/test/data/messages/xx/LC_MESSAGES/flufl.po
+-rw-r--r--   0        0        0      505 2023-07-22 01:02:18.660783 flufl_i18n-5.0.2/test/data/messages/yy/LC_MESSAGES/flufl.mo
+-rw-r--r--   0        0        0      672 2023-07-22 01:02:18.660783 flufl_i18n-5.0.2/test/data/messages/yy/LC_MESSAGES/flufl.po
+-rw-r--r--   0        0        0      370 2023-07-22 01:02:18.660783 flufl_i18n-5.0.2/test/test_application.py
+-rw-r--r--   0        0        0      845 2023-07-22 01:02:18.660783 flufl_i18n-5.0.2/test/test_expand.py
+-rw-r--r--   0        0        0      520 2023-07-22 01:02:18.660783 flufl_i18n-5.0.2/test/test_substitute.py
+-rw-r--r--   0        0        0     3617 2023-07-22 01:02:18.660783 flufl_i18n-5.0.2/test/test_translator.py
+-rw-r--r--   0        0        0      772 2023-07-22 01:02:18.660783 flufl_i18n-5.0.2/tox.ini
+-rw-r--r--   0        0        0     2179 1970-01-01 00:00:00.000000 flufl_i18n-5.0.2/PKG-INFO
```

### Comparing `flufl_i18n-5.0.1/LICENSE` & `flufl_i18n-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flufl_i18n-5.0.1/README.rst` & `flufl_i18n-5.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `flufl_i18n-5.0.1/conftest.py` & `flufl_i18n-5.0.2/conftest.py`

 * *Files identical despite different names*

### Comparing `flufl_i18n-5.0.1/docs/NEWS.rst` & `flufl_i18n-5.0.2/docs/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =====================
 flufl.i18n change log
 =====================
 
+5.0.2 (2023-07-21)
+==================
+* Update dependencies.
+* Other minor improvements and cleanups.
+
 5.0.1 (2023-06-13)
 ==================
 * Fix the build backend.
 
 5.0 (unreleased)
 ================
 * Drop Python 3.7 support. (GL#15)
```

### Comparing `flufl_i18n-5.0.1/docs/apiref.rst` & `flufl_i18n-5.0.2/docs/apiref.rst`

 * *Files identical despite different names*

### Comparing `flufl_i18n-5.0.1/docs/conf.py` & `flufl_i18n-5.0.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.intersphinx',
     ]
 
 intersphinx_mapping = {
-    'python': ('https://docs.python.org/', None),
+    'python': ('https://docs.python.org/3/', None),
     }
 
 autodoc_typehints = 'both'
 autoclass_content = 'both'
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['../../_templates']
```

### Comparing `flufl_i18n-5.0.1/docs/expand.rst` & `flufl_i18n-5.0.2/docs/expand.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 .. currentmodule:: flufl.i18n
 
 The Python standard library defines :class:`string.Template` strings, which
 are the implementation of `PEP 292`_ simple string templates.  Substitution
 placeholders are identified by a leading ``$``-sign [#]_.  A substitution
 dictionary names the keys and values that should be substituted into the
-template, replacing the placeholders.  This module defines the :meth:`expand()`
-function which takes the translated string and a substitution dictionary, and
-returns the resulting string.
+template, replacing the placeholders.  This module defines the
+:meth:`expand()` function which takes the translated string and a substitution
+dictionary, and returns the resulting string.
 
 Normally though, you shouldn't have to call this function yourself.
 ::
 
     >>> key_1 = 'key_1'
     >>> key_2 = 'key_2'
```

### Comparing `flufl_i18n-5.0.1/docs/index.rst` & `flufl_i18n-5.0.2/docs/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ===============
 
  * Project home: https://gitlab.com/warsaw/flufl.i18n
  * Report bugs at: https://gitlab.com/warsaw/flufl.i18n/issues
  * Code hosting: https://gitlab.com/warsaw/flufl.i18n.git
  * Documentation: https://flufli18n.readthedocs.io/
 
-You can install it with `pip`::
+You can install it with ``pip``::
 
     % pip install flufl.i18n
 
 You can grab the latest development copy of the code using git.  The master
 repository is hosted on GitLab.  If you have git installed, you can grab
 your own branch of the code like this::
```

### Comparing `flufl_i18n-5.0.1/docs/strategies.rst` & `flufl_i18n-5.0.2/docs/strategies.rst`

 * *Files 10% similar despite different names*

```diff
@@ -20,27 +20,28 @@
 ``<code>/LC_MESSAGES/<application>.mo``.
 
 .. note::
     :doc:`As before <using>` these examples will use the faux ``xx`` language,
     and the faux ``messages`` module referred to in these examples contains the
     language code directories.
 
-First import the Python package containing the message catalogs.
+First import the Python package containing the message catalogs for these
+examples [#]_.
 
     >>> import messages
 
 By setting the ``$LANG`` environment variable, we can specify that the
 application translates into that language automatically.
 
     >>> import os
     >>> os.environ['LANG'] = 'xx'
 
-Now we can instantiate a package strategy which finds its catalogs in the
-``messages`` Python package.  The first argument is the application name,
-which must be unique among all registered strategies.
+Now we can instantiate a package strategy which finds its catalogs in this
+example's ``messages`` Python package.  The first argument is the application
+name, which must be unique among all registered strategies.
 
     >>> from flufl.i18n import PackageStrategy
     >>> strategy = PackageStrategy('flufl', messages)
 
 Once you have the strategy you need, register it with the global registry.
 The registration process returns an application object which can be used to
 look up language codes.
@@ -100,7 +101,10 @@
 
     >>> print(get_gettext(
     ...     PackageStrategy('example', messages))('A test message'))
     A test message
 
 
 .. _gettext: https://www.gnu.org/software/gettext/manual/gettext.html
+
+.. [#] ``messages`` is not a standard Python package.  It exists only for
+       the examples in this documentation.
```

### Comparing `flufl_i18n-5.0.1/docs/using.rst` & `flufl_i18n-5.0.2/docs/using.rst`

 * *Files identical despite different names*

### Comparing `flufl_i18n-5.0.1/pyproject.toml` & `flufl_i18n-5.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Localization",
 ]
 dependencies = [
     "atpublic",
 ]
 dynamic = []
-version = "5.0.1"
+version = "5.0.2"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 "Home Page" = "https://flufli18n.readthedocs.io"
 Documentation = "https://flufli18n.readthedocs.io"
@@ -63,17 +63,17 @@
     "coverage[toml]",
     "diff-cover",
     "pytest",
     "pytest-cov",
     "sybil",
 ]
 qa = [
-    "ruff",
     "blue",
     "mypy",
+    "ruff",
 ]
 docs = [
     "sphinx",
     "furo",
 ]
 
 [tool.pytest.ini_options]
```

### Comparing `flufl_i18n-5.0.1/src/flufl/i18n/__init__.py` & `flufl_i18n-5.0.2/src/flufl/i18n/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from flufl.i18n.types import (
     RuntimeTranslator,
     TranslationContextManager,
     TranslationStrategy,
 )
 
 
-__version__ = '5.0.1'
+__version__ = '5.0.2'
 
 
 _public(
     Application=Application,
     PackageStrategy=PackageStrategy,
     RuntimeTranslator=RuntimeTranslator,
     SimpleStrategy=SimpleStrategy,
```

### Comparing `flufl_i18n-5.0.1/src/flufl/i18n/_application.py` & `flufl_i18n-5.0.2/src/flufl/i18n/_application.py`

 * *Files identical despite different names*

### Comparing `flufl_i18n-5.0.1/src/flufl/i18n/_expand.py` & `flufl_i18n-5.0.2/src/flufl/i18n/_expand.py`

 * *Files identical despite different names*

### Comparing `flufl_i18n-5.0.1/src/flufl/i18n/_registry.py` & `flufl_i18n-5.0.2/src/flufl/i18n/_registry.py`

 * *Files identical despite different names*

### Comparing `flufl_i18n-5.0.1/src/flufl/i18n/_strategy.py` & `flufl_i18n-5.0.2/src/flufl/i18n/_strategy.py`

 * *Files identical despite different names*

### Comparing `flufl_i18n-5.0.1/src/flufl/i18n/_substitute.py` & `flufl_i18n-5.0.2/src/flufl/i18n/_substitute.py`

 * *Files identical despite different names*

### Comparing `flufl_i18n-5.0.1/src/flufl/i18n/_translator.py` & `flufl_i18n-5.0.2/src/flufl/i18n/_translator.py`

 * *Files identical despite different names*

### Comparing `flufl_i18n-5.0.1/src/flufl/i18n/types.py` & `flufl_i18n-5.0.2/src/flufl/i18n/types.py`

 * *Files identical despite different names*

### Comparing `flufl_i18n-5.0.1/test/data/messages/xx/LC_MESSAGES/flufl.po` & `flufl_i18n-5.0.2/test/data/messages/xx/LC_MESSAGES/flufl.po`

 * *Files identical despite different names*

### Comparing `flufl_i18n-5.0.1/test/data/messages/yy/LC_MESSAGES/flufl.po` & `flufl_i18n-5.0.2/test/data/messages/yy/LC_MESSAGES/flufl.po`

 * *Files identical despite different names*

### Comparing `flufl_i18n-5.0.1/test/test_expand.py` & `flufl_i18n-5.0.2/test/test_expand.py`

 * *Files identical despite different names*

### Comparing `flufl_i18n-5.0.1/test/test_substitute.py` & `flufl_i18n-5.0.2/test/test_substitute.py`

 * *Files identical despite different names*

### Comparing `flufl_i18n-5.0.1/test/test_translator.py` & `flufl_i18n-5.0.2/test/test_translator.py`

 * *Files identical despite different names*

### Comparing `flufl_i18n-5.0.1/tox.ini` & `flufl_i18n-5.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `flufl_i18n-5.0.1/PKG-INFO` & `flufl_i18n-5.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flufl-i18n
-Version: 5.0.1
+Name: flufl.i18n
+Version: 5.0.2
 Summary: A high level API for internationalizing Python libraries and applications
 Keywords: i18n internationalization
 Author-Email: Barry Warsaw <barry@python.org>
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
```

