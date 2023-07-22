# Comparing `tmp/flufl_lock-8.0.1.tar.gz` & `tmp/flufl_lock-8.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flufl_lock-8.0.1.tar", last modified: Thu Jun 22 17:28:37 2023, max compression
+gzip compressed data, was "flufl_lock-8.0.2.tar", last modified: Sat Jul 22 19:14:48 2023, max compression
```

## Comparing `flufl_lock-8.0.1.tar` & `flufl_lock-8.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      558 2023-06-22 17:28:10.404516 flufl_lock-8.0.1/LICENSE
--rw-r--r--   0        0        0     2131 2023-06-22 17:28:10.405433 flufl_lock-8.0.1/README.rst
--rw-r--r--   0        0        0     2961 2023-06-22 17:28:10.405433 flufl_lock-8.0.1/conftest.py
--rw-r--r--   0        0        0     7513 2023-06-22 17:28:10.405433 flufl_lock-8.0.1/docs/NEWS.rst
--rw-r--r--   0        0        0        0 2023-06-22 17:28:10.426516 flufl_lock-8.0.1/docs/__init__.py
--rw-r--r--   0        0        0      273 2023-06-22 17:28:10.405433 flufl_lock-8.0.1/docs/_static/lock-dark.svg
--rw-r--r--   0        0        0      337 2023-06-22 17:28:10.405433 flufl_lock-8.0.1/docs/_static/lock-light.svg
--rw-r--r--   0        0        0     1634 2023-06-22 17:28:10.405433 flufl_lock-8.0.1/docs/_static/logo-dark.png
--rw-r--r--   0        0        0     1273 2023-06-22 17:28:10.405433 flufl_lock-8.0.1/docs/_static/logo-dark.svg
--rw-r--r--   0        0        0     1302 2023-06-22 17:28:10.405433 flufl_lock-8.0.1/docs/_static/logo-light.png
--rw-r--r--   0        0        0     1308 2023-06-22 17:28:10.405433 flufl_lock-8.0.1/docs/_static/logo-light.svg
--rw-r--r--   0        0        0      405 2023-06-22 17:28:10.405433 flufl_lock-8.0.1/docs/apiref.rst
--rw-r--r--   0        0        0     6814 2023-06-22 17:28:10.405433 flufl_lock-8.0.1/docs/conf.py
--rw-r--r--   0        0        0     1834 2023-06-22 17:28:10.405433 flufl_lock-8.0.1/docs/index.rst
--rw-r--r--   0        0        0     9350 2023-06-22 17:28:10.405433 flufl_lock-8.0.1/docs/theory.rst
--rw-r--r--   0        0        0     9430 2023-06-22 17:28:10.405433 flufl_lock-8.0.1/docs/using.rst
--rw-r--r--   0        0        0     3187 2023-06-22 17:28:37.739036 flufl_lock-8.0.1/pyproject.toml
--rw-r--r--   0        0        0      453 2023-06-22 17:28:10.406349 flufl_lock-8.0.1/src/flufl/lock/__init__.py
--rw-r--r--   0        0        0    25626 2023-06-22 17:28:10.406349 flufl_lock-8.0.1/src/flufl/lock/_lockfile.py
--rw-r--r--   0        0        0        0 2023-06-22 17:28:10.426516 flufl_lock-8.0.1/src/flufl/lock/py.typed
--rw-r--r--   0        0        0        0 2023-06-22 17:28:10.426516 flufl_lock-8.0.1/test/__init__.py
--rw-r--r--   0        0        0      296 2023-06-22 17:28:10.406349 flufl_lock-8.0.1/test/test_api.py
--rw-r--r--   0        0        0    19924 2023-06-22 17:28:10.406349 flufl_lock-8.0.1/test/test_lock.py
--rw-r--r--   0        0        0      772 2023-06-22 17:28:10.407266 flufl_lock-8.0.1/tox.ini
--rw-r--r--   0        0        0     3276 1970-01-01 00:00:00.000000 flufl_lock-8.0.1/PKG-INFO
+-rw-r--r--   0        0        0      558 2023-07-22 19:14:22.287609 flufl_lock-8.0.2/LICENSE
+-rw-r--r--   0        0        0     2131 2023-07-22 19:14:22.287609 flufl_lock-8.0.2/README.rst
+-rw-r--r--   0        0        0     2961 2023-07-22 19:14:22.287609 flufl_lock-8.0.2/conftest.py
+-rw-r--r--   0        0        0     7616 2023-07-22 19:14:22.287609 flufl_lock-8.0.2/docs/NEWS.rst
+-rw-r--r--   0        0        0        0 2023-07-22 19:14:22.311610 flufl_lock-8.0.2/docs/__init__.py
+-rw-r--r--   0        0        0      273 2023-07-22 19:14:22.287609 flufl_lock-8.0.2/docs/_static/lock-dark.svg
+-rw-r--r--   0        0        0      337 2023-07-22 19:14:22.287609 flufl_lock-8.0.2/docs/_static/lock-light.svg
+-rw-r--r--   0        0        0     1634 2023-07-22 19:14:22.287609 flufl_lock-8.0.2/docs/_static/logo-dark.png
+-rw-r--r--   0        0        0     1273 2023-07-22 19:14:22.288609 flufl_lock-8.0.2/docs/_static/logo-dark.svg
+-rw-r--r--   0        0        0     1302 2023-07-22 19:14:22.288609 flufl_lock-8.0.2/docs/_static/logo-light.png
+-rw-r--r--   0        0        0     1308 2023-07-22 19:14:22.288609 flufl_lock-8.0.2/docs/_static/logo-light.svg
+-rw-r--r--   0        0        0      405 2023-07-22 19:14:22.288609 flufl_lock-8.0.2/docs/apiref.rst
+-rw-r--r--   0        0        0     6816 2023-07-22 19:14:22.288609 flufl_lock-8.0.2/docs/conf.py
+-rw-r--r--   0        0        0     1834 2023-07-22 19:14:22.288609 flufl_lock-8.0.2/docs/index.rst
+-rw-r--r--   0        0        0     9350 2023-07-22 19:14:22.288609 flufl_lock-8.0.2/docs/theory.rst
+-rw-r--r--   0        0        0     9430 2023-07-22 19:14:22.288609 flufl_lock-8.0.2/docs/using.rst
+-rw-r--r--   0        0        0     3187 2023-07-22 19:14:48.540609 flufl_lock-8.0.2/pyproject.toml
+-rw-r--r--   0        0        0      453 2023-07-22 19:14:22.289609 flufl_lock-8.0.2/src/flufl/lock/__init__.py
+-rw-r--r--   0        0        0    25580 2023-07-22 19:14:22.289609 flufl_lock-8.0.2/src/flufl/lock/_lockfile.py
+-rw-r--r--   0        0        0        0 2023-07-22 19:14:22.312610 flufl_lock-8.0.2/src/flufl/lock/py.typed
+-rw-r--r--   0        0        0        0 2023-07-22 19:14:22.312610 flufl_lock-8.0.2/test/__init__.py
+-rw-r--r--   0        0        0      296 2023-07-22 19:14:22.289609 flufl_lock-8.0.2/test/test_api.py
+-rw-r--r--   0        0        0    19924 2023-07-22 19:14:22.289609 flufl_lock-8.0.2/test/test_lock.py
+-rw-r--r--   0        0        0      772 2023-07-22 19:14:22.289609 flufl_lock-8.0.2/tox.ini
+-rw-r--r--   0        0        0     3276 1970-01-01 00:00:00.000000 flufl_lock-8.0.2/PKG-INFO
```

### Comparing `flufl_lock-8.0.1/LICENSE` & `flufl_lock-8.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flufl_lock-8.0.1/README.rst` & `flufl_lock-8.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `flufl_lock-8.0.1/conftest.py` & `flufl_lock-8.0.2/conftest.py`

 * *Files identical despite different names*

### Comparing `flufl_lock-8.0.1/docs/NEWS.rst` & `flufl_lock-8.0.2/docs/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =====================
 flufl.lock change log
 =====================
 
+8.0.2 (2023-07-21)
+==================
+* Update dependencies.
+* Other minor improvements and cleanups.
+
 8.0.1 (2023-06-22)
 ==================
 * Minor documentation fix.
 
 8.0 (2023-06-21)
 ================
 * Drop Python 3.7 support (GL#34)
```

### Comparing `flufl_lock-8.0.1/docs/_static/logo-dark.png` & `flufl_lock-8.0.2/docs/_static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `flufl_lock-8.0.1/docs/_static/logo-dark.svg` & `flufl_lock-8.0.2/docs/_static/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `flufl_lock-8.0.1/docs/_static/logo-light.png` & `flufl_lock-8.0.2/docs/_static/logo-light.png`

 * *Files identical despite different names*

### Comparing `flufl_lock-8.0.1/docs/_static/logo-light.svg` & `flufl_lock-8.0.2/docs/_static/logo-light.svg`

 * *Files identical despite different names*

### Comparing `flufl_lock-8.0.1/docs/conf.py` & `flufl_lock-8.0.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
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

### Comparing `flufl_lock-8.0.1/docs/index.rst` & `flufl_lock-8.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `flufl_lock-8.0.1/docs/theory.rst` & `flufl_lock-8.0.2/docs/theory.rst`

 * *Files identical despite different names*

### Comparing `flufl_lock-8.0.1/docs/using.rst` & `flufl_lock-8.0.2/docs/using.rst`

 * *Files identical despite different names*

### Comparing `flufl_lock-8.0.1/pyproject.toml` & `flufl_lock-8.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "atpublic",
     "psutil",
 ]
 dynamic = []
-version = "8.0.1"
+version = "8.0.2"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 "Home Page" = "https://flufllock.readthedocs.io"
 Documentation = "https://flufllock.readthedocs.io"
```

### Comparing `flufl_lock-8.0.1/src/flufl/lock/_lockfile.py` & `flufl_lock-8.0.2/src/flufl/lock/_lockfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -588,17 +588,15 @@
         # that lock.  All we really need to do is to log and return.  If a
         # timeout was given, eventually the .lock() call will timeout.
         # However if no timeout was given, the .lock() will block forever.
         try:
             self.details                            # noqa: B018
         except NotLockedError:
             log.error(
-                "lockfile exists but isn't safe to break: {}".format(
-                    self._lockfile
-                )
+                f"lockfile exists but isn't safe to break: {self._lockfile}"
             )
             return
         # Touch the lock file.  This reduces but does not eliminate the
         # chance for a race condition during breaking.  Two processes could
         # both pass the test for lock expiry in lock() before one of them gets
         # to touch the lock file.  This shouldn't be too bad because all
         # they'll do in that function is delete the lock files, not claim the
```

### Comparing `flufl_lock-8.0.1/test/test_lock.py` & `flufl_lock-8.0.2/test/test_lock.py`

 * *Files identical despite different names*

### Comparing `flufl_lock-8.0.1/tox.ini` & `flufl_lock-8.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `flufl_lock-8.0.1/PKG-INFO` & `flufl_lock-8.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flufl-lock
-Version: 8.0.1
+Name: flufl.lock
+Version: 8.0.2
 Summary: NFS-safe file locking with timeouts for POSIX and Windows
 Keywords: locking locks lock
 Author-Email: Barry Warsaw <barry@python.org>
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
```

