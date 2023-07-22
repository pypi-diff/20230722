# Comparing `tmp/clsprop-1.0.0.tar.gz` & `tmp/clsprop-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clsprop-1.0.0.tar", max compression
+gzip compressed data, was "clsprop-1.0.1.tar", max compression
```

## Comparing `clsprop-1.0.0.tar` & `clsprop-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      714 2023-04-11 10:41:34.924530 clsprop-1.0.0/README.md
--rw-r--r--   0        0        0     1108 2023-04-11 10:40:41.632365 clsprop-1.0.0/clsprop.py
--rw-r--r--   0        0        0      391 2023-04-11 10:43:31.343179 clsprop-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 clsprop-1.0.0/setup.py
--rw-r--r--   0        0        0     1305 1970-01-01 00:00:00.000000 clsprop-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      734 2023-04-11 10:52:39.360114 clsprop-1.0.1/README.md
+-rw-r--r--   0        0        0     1128 2023-04-11 10:52:23.550777 clsprop-1.0.1/clsprop.py
+-rw-r--r--   0        0        0      391 2023-04-11 10:55:27.549977 clsprop-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1242 1970-01-01 00:00:00.000000 clsprop-1.0.1/setup.py
+-rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 clsprop-1.0.1/PKG-INFO
```

### Comparing `clsprop-1.0.0/README.md` & `clsprop-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Works just like @property for classes, except deleters don't work (and are
 perhaps impossible).
 
 Inspired by https://stackoverflow.com/a/39542816/43839
 
 ## Example
 
+    import clsprop
+
     class Full:
         _name = 'fool'
 
         @clsprop
         def name(cls):
             return cls._name
```

### Comparing `clsprop-1.0.0/clsprop.py` & `clsprop-1.0.1/clsprop.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 Works just like @property for classes, except deleters don't work (and are
 perhaps impossible).
 
 Inspired by https://stackoverflow.com/a/39542816/43839
 
 ## Example
 
+    import clsprop
+
     class Full:
         _name = 'fool'
 
         @clsprop
         def name(cls):
             return cls._name
```

### Comparing `clsprop-1.0.0/setup.py` & `clsprop-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['clsprop']
 setup_kwargs = {
     'name': 'clsprop',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': '🏫 Just like @property but for classes 🏫',
-    'long_description': "Works just like @property for classes, except deleters don't work (and are\nperhaps impossible).\n\nInspired by https://stackoverflow.com/a/39542816/43839\n\n## Example\n\n    class Full:\n        _name = 'fool'\n\n        @clsprop\n        def name(cls):\n            return cls._name\n\n        @name.setter\n        def name(cls, name):\n            cls._name = name\n\n        # Unfortunately, the deleter never gets called\n        @name.deleter\n        def name(cls, name):\n            raise ValueError('Cannot delete name')\n\n    assert Full.name == 'fool'\n\n    Full.name = 'foll'\n    assert Full.name == 'foll'\n\n    del Full.name  # oh, well\n\n\n### [API Documentation](https://rec.github.io/clsprop#clsprop--api-documentation)\n",
+    'long_description': "Works just like @property for classes, except deleters don't work (and are\nperhaps impossible).\n\nInspired by https://stackoverflow.com/a/39542816/43839\n\n## Example\n\n    import clsprop\n\n    class Full:\n        _name = 'fool'\n\n        @clsprop\n        def name(cls):\n            return cls._name\n\n        @name.setter\n        def name(cls, name):\n            cls._name = name\n\n        # Unfortunately, the deleter never gets called\n        @name.deleter\n        def name(cls, name):\n            raise ValueError('Cannot delete name')\n\n    assert Full.name == 'fool'\n\n    Full.name = 'foll'\n    assert Full.name == 'foll'\n\n    del Full.name  # oh, well\n\n\n### [API Documentation](https://rec.github.io/clsprop#clsprop--api-documentation)\n",
     'author': 'Tom Ritchford',
     'author_email': 'tom@swirly.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'py_modules': modules,
     'python_requires': '>=3.7,<4.0',
```

### Comparing `clsprop-1.0.0/PKG-INFO` & `clsprop-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clsprop
-Version: 1.0.0
+Version: 1.0.1
 Summary: 🏫 Just like @property but for classes 🏫
 License: MIT
 Author: Tom Ritchford
 Author-email: tom@swirly.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,16 @@
 Works just like @property for classes, except deleters don't work (and are
 perhaps impossible).
 
 Inspired by https://stackoverflow.com/a/39542816/43839
 
 ## Example
 
+    import clsprop
+
     class Full:
         _name = 'fool'
 
         @clsprop
         def name(cls):
             return cls._name
```

