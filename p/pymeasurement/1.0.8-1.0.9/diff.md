# Comparing `tmp/pymeasurement-1.0.8.tar.gz` & `tmp/pymeasurement-1.0.9.tar.gz`

## Comparing `pymeasurement-1.0.8.tar` & `pymeasurement-1.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/Makefile
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/aggregate_operations.rst
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/basics.rst
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/chemistry_example.rst
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/conf.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/get_started.rst
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/index.rst
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/initialize.rst
--rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/lab_example.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/make.bat
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/operations.rst
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/physics_example.rst
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/requirements.txt
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/table_operations.rst
--rw-r--r--   0        0        0    62858 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/test.ipynb
--rw-r--r--   0        0        0    32256 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/_static/Combustion_Lab_1920_Student_Data.xls
--rw-r--r--   0        0        0    11723 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/_static/Combustion_Lab_1920_Student_Data.xlsx
--rw-r--r--   0        0        0    36352 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/_static/example.xls
--rw-r--r--   0        0        0    10729 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/_static/example.xlsx
--rw-r--r--   0        0        0    44032 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/_static/output.xls
--rw-r--r--   0        0        0    13465 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/_static/output.xlsx
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/documentation/index.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/documentation/measurement.rst
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/documentation/sigfig.rst
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/documentation/util/index.rst
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/documentation/util/parser.rst
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/documentation/util/typecheck.rst
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/documentation/util/chem/compound.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/documentation/util/chem/element.rst
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/documentation/util/includes/measurement.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/docs/documentation/util/includes/sigfig.rst
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/src/pymeasurement/__init__.py
--rw-r--r--   0        0        0    23936 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/src/pymeasurement/measurement.py
--rw-r--r--   0        0        0    10526 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/src/pymeasurement/sigfig.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/src/pymeasurement/util/parser.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/src/pymeasurement/util/typecheck.py
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/src/pymeasurement/util/chem/compound.py
--rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/src/pymeasurement/util/chem/element.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/tests/__init__.py
--rw-r--r--   0        0        0     6990 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/tests/test_pymeasurement.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/LICENSE
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/README.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pymeasurement-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    32256 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/Combustion_Lab_1920_Student_Data.xls
+-rw-r--r--   0        0        0    11723 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/Combustion_Lab_1920_Student_Data.xlsx
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/Makefile
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/aggregate_operations.rst
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/basics.rst
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/chemistry_example.rst
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/conf.py
+-rw-r--r--   0        0        0    36352 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/example.xls
+-rw-r--r--   0        0        0    10729 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/example.xlsx
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/get_started.rst
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/index.rst
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/initialize.rst
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/lab_example.rst
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/make.bat
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/operations.rst
+-rw-r--r--   0        0        0    44032 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/output.xls
+-rw-r--r--   0        0        0    13465 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/output.xlsx
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/physics_example.rst
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/requirements.txt
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/table_operations.rst
+-rw-r--r--   0        0        0    64392 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/test.ipynb
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/documentation/index.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/documentation/measurement.rst
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/documentation/sigfig.rst
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/documentation/util/index.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/documentation/util/parser.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/documentation/util/typecheck.rst
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/documentation/util/chem/compound.rst
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/documentation/util/chem/element.rst
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/documentation/util/includes/measurement.rst
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/docs/documentation/util/includes/sigfig.rst
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/src/pymeasurement/__init__.py
+-rw-r--r--   0        0        0    24573 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/src/pymeasurement/measurement.py
+-rw-r--r--   0        0        0    10793 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/src/pymeasurement/sigfig.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/src/pymeasurement/util/parser.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/src/pymeasurement/util/typecheck.py
+-rw-r--r--   0        0        0     6316 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/src/pymeasurement/util/chem/compound.py
+-rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/src/pymeasurement/util/chem/element.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/tests/test_pymeasurement.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/LICENSE
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/README.md
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pymeasurement-1.0.9/PKG-INFO
```

### Comparing `pymeasurement-1.0.8/docs/Makefile` & `pymeasurement-1.0.9/docs/Makefile`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Minimal makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line, and also
-# from the environment for the first two.
-SPHINXOPTS    ?=
-SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = .
-BUILDDIR      = _build
-
-# Put it first so that "make" without argument is like "make help".
-help:
-	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
-
-.PHONY: help Makefile
-
-# Catch-all target: route all unknown targets to Sphinx using the new
-# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+# Minimal makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line, and also
+# from the environment for the first two.
+SPHINXOPTS    ?=
+SPHINXBUILD   ?= sphinx-build
+SOURCEDIR     = .
+BUILDDIR      = _build
+
+# Put it first so that "make" without argument is like "make help".
+help:
+	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+.PHONY: help Makefile
+
+# Catch-all target: route all unknown targets to Sphinx using the new
+# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
+%: Makefile
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `pymeasurement-1.0.8/docs/basics.rst` & `pymeasurement-1.0.9/docs/basics.rst`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-Measurement Basics
-==================
-
-Every measurement has a sample, uncertainty, and units.
-
-The uncertainty can be expressed as an absolute value or as a relative percentage.
-
-
-**In-Place Mutation**
-
-The below method mutates the measurement uncertainty style in-place.
-
-.. testsetup:: *
-
-    from pymeasurement import Measurement
-
-.. doctest:: python
-
-        >>> m = Measurement.fromStr("2.00 +/- 0.03 m")
-
-        >>> m.toAbsolute()
-        2.00 +/- 0.03 m
-
-        >>> m
-        2.00 +/- 0.03 m
-
-.. doctest:: python
-
-        >>> m.toPercent()
-        2.00 +/- 1.5% m
-
-        >>> m
-        2.00 +/- 1.5% m
-
-**Immutable**
-
-The below method creates a new measurement object with the given uncertainty style.
-
-.. doctest:: python
-
-        >>> m.absolute()
-        2.00 +/- 0.03 m
-
-.. doctest:: python
-
-        >>> m.percent()
+Measurement Basics
+==================
+
+Every measurement has a sample, uncertainty, and units.
+
+The uncertainty can be expressed as an absolute value or as a relative percentage.
+
+
+**In-Place Mutation**
+
+The below method mutates the measurement uncertainty style in-place.
+
+.. testsetup:: *
+
+    from pymeasurement import Measurement
+
+.. doctest:: python
+
+        >>> m = Measurement.fromStr("2.00 +/- 0.03 m")
+
+        >>> m.toAbsolute()
+        2.00 +/- 0.03 m
+
+        >>> m
+        2.00 +/- 0.03 m
+
+.. doctest:: python
+
+        >>> m.toPercent()
+        2.00 +/- 1.5% m
+
+        >>> m
+        2.00 +/- 1.5% m
+
+**Immutable**
+
+The below method creates a new measurement object with the given uncertainty style.
+
+.. doctest:: python
+
+        >>> m.absolute()
+        2.00 +/- 0.03 m
+
+.. doctest:: python
+
+        >>> m.percent()
         2.00 +/- 1.5% m
```

### Comparing `pymeasurement-1.0.8/docs/conf.py` & `pymeasurement-1.0.9/docs/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,38 @@
-# Configuration file for the Sphinx documentation builder.
-#
-# For the full list of built-in configuration values, see the documentation:
-# https://www.sphinx-doc.org/en/master/usage/configuration.html
-
-import os
-import sys
-sys.path.insert(0, os.path.abspath('../src/'))
-
-# -- Project information -----------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
-
-project = 'pymeasurement'
-copyright = '2023, Saptak Das'
-author = 'Saptak Das'
-release = '1.0.8'
-
-# -- General configuration ---------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
-
-extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.viewcode',
-    'sphinx.ext.githubpages',
-    'sphinx.ext.doctest',
-    'sphinx.ext.mathjax',
-    'sphinx_copybutton',
-    'sphinxcontrib.exceltable'
-]
-
-templates_path = ['_templates']
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
-
-
-
-# -- Options for HTML output -------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
-
-html_theme = 'furo'
-html_static_path = ['_static']
-
-# html_sidebars = {
-#     "**": [
-#         "about.html",
-#         "navigation.html",
-#         "relations.html",
-#         "searchbox.html",
-#         "donate.html",
-#     ]
-# }
-# html_sidebars = {
-#     "index": ["localtoc.html", "search.html"],
-#     "**": ["localtoc.html", "search.html"],
-# }
-# singlehtml_sidebars = {"index": ["localtoc.html", "search.html"]}
+# Configuration file for the Sphinx documentation builder.
+#
+# For the full list of built-in configuration values, see the documentation:
+# https://www.sphinx-doc.org/en/master/usage/configuration.html
+
+# -- Project information -----------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
+
+project = 'pymeasurement'
+copyright = '2023, Saptak Das'
+author = 'Saptak Das'
+release = '1.0.9'
+
+# -- General configuration ---------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
+
+import os
+import sys
+
+sys.path.append(os.path.abspath("./sphinxcontrib"))
+
+extensions = [
+    'sphinx.ext.autodoc',
+    'sphinx.ext.viewcode',
+    'sphinx.ext.githubpages',
+    'sphinx.ext.doctest',
+    'sphinx.ext.mathjax',
+    'sphinx_copybutton',
+    'sphinxcontrib.exceltable'
+]
+
+sys.path.insert(0, os.path.abspath('../../src/'))
+
+templates_path = ['_templates']
+exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+
+html_theme = 'furo'
+html_static_path = ['_static']
```

### Comparing `pymeasurement-1.0.8/docs/index.rst` & `pymeasurement-1.0.9/docs/index.rst`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-.. pymeasurement documentation master file, created by
-   sphinx-quickstart on Tue Feb  7 02:24:49 2023.
-   You can adapt this file completely to your liking, but it should at least
-   contain the root `toctree` directive.
-
-Welcome to pymeasurement's documentation!
-=========================================
-A Measurement Calculator with Fixed Point Precision, Uncertainties, and Units.
-
-Get started with pymeasurement by reading the :doc:`get_started` section.
-
-Read the :doc:`documentation/index` section for detailed information on the package.
-
-View on `PyPi <https://pypi.org/project/pymeasurement/>`_ and on `Github <https://github.com/Saptak625/pymeasurement>`_.
-
-.. toctree::
-   :maxdepth: 2
-   :caption: Contents:
-   
-   get_started
-   basics
-   initialize
-   operations
-   aggregate_operations
-   table_operations
-   physics_example
-   chemistry_example
-   lab_example
-   documentation/index
-   genindex
-
+.. pymeasurement documentation master file, created by
+   sphinx-quickstart on Tue Feb  7 02:24:49 2023.
+   You can adapt this file completely to your liking, but it should at least
+   contain the root `toctree` directive.
+
+Welcome to pymeasurement's documentation!
+=========================================
+A Measurement Calculator with Fixed Point Precision, Uncertainties, and Units.
+
+Get started with pymeasurement by reading the :doc:`get_started` section.
+
+Read the :doc:`documentation/index` section for detailed information on the package.
+
+View on `PyPi <https://pypi.org/project/pymeasurement/>`_ and on `Github <https://github.com/Saptak625/pymeasurement>`_.
+
+.. toctree::
+   :maxdepth: 2
+   :caption: Contents:
+   
+   get_started
+   basics
+   initialize
+   operations
+   aggregate_operations
+   table_operations
+   physics_example
+   chemistry_example
+   lab_example
+   documentation/index
+   genindex
+
```

### Comparing `pymeasurement-1.0.8/docs/lab_example.rst` & `pymeasurement-1.0.9/docs/lab_example.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-Lab Example
-=================
-
-Pymeasurement's Measurement type can be used to perform precision-based calculations with uncertainty propagation in standard Python data structures such as Pandas DataFrames. This example shows how to use the Measurement type to evaluate the data from a calorimetry experiment.
-
-Problem
---------
-
-Calculate the relationship between the molar enthalpy of combustion and the carbon chain length of primary alcohol fuels.
-
-
-**Data Table throughout Calorimetry Lab**
-
-.. exceltable:: 
-    :file: _static\Combustion_Lab_1920_Student_Data.xls
-    :header: 1
-    :selection: A1:F24
-
-Solution
---------
-
-The data from the lab is imported into a Pandas DataFrame.
-
-.. doctest:: python
-
-    >>> import pandas as pd
-    >>> df = pd.read_excel('_static\Combustion_Lab_1920_Student_Data.xlsx')
-
-The DataFrame columns are converted into pymeasurement Measurements.
-
-.. doctest:: python
-
-    >>> from pymeasurement import Measurement as M
-    >>> decimals = [3, 3, 3, 1, 1]
-    >>> units = ['g', 'g', 'g', 'ºC', 'ºC']
-    >>> for i in range(5):
-    ...     df.iloc[:, i + 3] = M.importColumn(df.iloc[:, i + 3], d=True, un=units[i], decimals=decimals[i])
-
-Now using the below formulas, the enthalpy of combustion can be calculated for each trial.
-
-.. math::
-
-    Q = m c \Delta T = m c (T_f - T_i)
-
-.. math::
-
-    n = m / M
-
-.. math::
-
-    \Delta H = -\frac{Q}{n}
-
-.. doctest:: python
-    
-    >>> heat_capacity = M.fromStr('4.18c J/g*ºC')
-    >>> j_to_kj = M.fromStr('0.001c kJ/J')
-    >>> results_df_1 = df.iloc[:, 0:3]
-    >>> results_df_1['Q of H2O (kJ)'] = df['Mass of water (+/- 0.001 g)'] * heat_capacity * (df['Final temperature (+/- 0.1 ºC)'] - df['Initial temperature (+/- 0.1 ºC)']) * j_to_kj
-    >>> results_df_1['Mass of Alcohol (g)'] = df['Initial mass of spirit burner (+/- 0.001 g)'] - df['Final mass of spirit burner (+/- 0.001 g)']
-    >>> molar_masses = {'Ethanol': M.fromStr('46.08c g/mol'), 'Propan-1-ol': M.fromStr('60.11c g/mol'), 'Butan-1-ol': M.fromStr('74.14c g/mol'), 'Pentan-1-ol': M.fromStr('88.17c g/mol')}
-    >>> results_df_1['Molar Mass of Alcohol (g/mol)'] = results_df_1.apply(lambda x: x['Mass of Alcohol (g)'] / molar_masses[x['Alcohol tested']], axis=1)
-    >>> results_df_1['Molar Enthalpy of Combustion (kJ/mol)'] = - results_df_1['Q of H2O (kJ)'] / results_df_1['Molar Mass of Alcohol (g/mol)']
-
-**Results Table 1: Individual Molar Enthalpy of Combustion**
-
-.. exceltable:: 
-    :file: _static\output.xls
-    :header: 1
-    :selection: A1:G24
-
-Now, to calculate the average molar enthalpy of combustion for each of the alcohols, the data is grouped by alcohol type and the average is taken.
-
-.. doctest:: python
-
-    >>> results_df_2 = pd.DataFrame()
-    >>> results_df_2['Alcohol'] = results_df_1['Alcohol tested'].unique()
-    >>> grouped_data = list(results_df_1.groupby('Alcohol tested')['Molar Enthalpy of Combustion (kJ/mol)'])
-    >>> grouped_data_dict = {i[0]: i[1] for i in grouped_data}
-    >>> results_df_2['Average Molar Enthalpy of Combustion (kJ/mol)'] = [M.average(list(grouped_data_dict[i])).percent() for i in results_df_2['Alcohol']]
-    >>> results_df_2['Accepted Molar Enthalpy of Combustion (kJ/mol)'] = [M.fromStr('-1367c kJ/mol'), M.fromStr('-2021c kJ/mol'), M.fromStr('-2676c kJ/mol'), M.fromStr('-3329c kJ/mol')]
-    >>> results_df_2['Percent Error (%)'] = results_df_2.apply(lambda x: ((x['Accepted Molar Enthalpy of Combustion (kJ/mol)'] - x['Average Molar Enthalpy of Combustion (kJ/mol)']) * 100 / x['Accepted Molar Enthalpy of Combustion (kJ/mol)']), axis=1)
-
-**Results Table 2: Average Molar Enthalpy of Combustion**
-
-.. exceltable:: 
-    :file: _static\output.xls
-    :header: 1
-    :selection: J1:M5
-
-
-Finally, we can convert the Measurement columns back into standard numeric columns.
-
-.. doctest:: python
-
-    >>> final_results_df_1 = results_df_1.copy()
-    >>> for i in range(4):
-    ...     M.exportColumn(final_results_df_1, results_df_1.iloc[:, i + 3])
-    >>> final_results_df_2 = results_df_2.copy()
-    >>> final_results_df_2 = results_df_2.copy()
-    >>> for i in range(3):
-    ...     M.exportColumn(final_results_df_2, results_df_2.iloc[:, i + 1], addUncertainty=i==0)
-
-**Final Results Table 1: Individual Molar Enthalpy of Combustion**
-
-.. exceltable:: 
-    :file: _static\output.xls
-    :header: 1
-    :selection: A31:K54
-
-**Final Results Table 2: Average Molar Enthalpy of Combustion**
-
-.. exceltable:: 
-    :file: _static\output.xls
-    :header: 1
-    :selection: P31:T35
+Lab Example
+=================
+
+Pymeasurement's Measurement type can be used to perform precision-based calculations with uncertainty propagation in standard Python data structures such as Pandas DataFrames. This example shows how to use the Measurement type to evaluate the data from a calorimetry experiment.
+
+Problem
+--------
+
+Calculate the relationship between the molar enthalpy of combustion and the carbon chain length of primary alcohol fuels.
+
+
+**Data Table throughout Calorimetry Lab**
+
+.. exceltable:: 
+    :file: Combustion_Lab_1920_Student_Data.xls
+    :selection: A1:F24
+    :header: 1
+
+Solution
+--------
+
+The data from the lab is imported into a Pandas DataFrame.
+
+.. doctest:: python
+
+    >>> import pandas as pd
+    >>> df = pd.read_excel('Combustion_Lab_1920_Student_Data.xlsx')
+
+The DataFrame columns are converted into pymeasurement Measurements.
+
+.. doctest:: python
+
+    >>> from pymeasurement import Measurement as M
+    >>> decimals = [3, 3, 3, 1, 1]
+    >>> units = ['g', 'g', 'g', 'ºC', 'ºC']
+    >>> for i in range(5):
+    ...     df.iloc[:, i + 3] = M.importColumn(df.iloc[:, i + 3], d=True, un=units[i], decimals=decimals[i])
+
+Now using the below formulas, the enthalpy of combustion can be calculated for each trial.
+
+.. math::
+
+    Q = m c \Delta T = m c (T_f - T_i)
+
+.. math::
+
+    n = m / M
+
+.. math::
+
+    \Delta H = -\frac{Q}{n}
+
+.. doctest:: python
+    
+    >>> heat_capacity = M.fromStr('4.18c J/g*ºC')
+    >>> j_to_kj = M.fromStr('0.001c kJ/J')
+    >>> results_df_1 = df.iloc[:, 0:3]
+    >>> results_df_1['Q of H2O (kJ)'] = df['Mass of water (+/- 0.001 g)'] * heat_capacity * (df['Final temperature (+/- 0.1 ºC)'] - df['Initial temperature (+/- 0.1 ºC)']) * j_to_kj
+    >>> results_df_1['Mass of Alcohol (g)'] = df['Initial mass of spirit burner (+/- 0.001 g)'] - df['Final mass of spirit burner (+/- 0.001 g)']
+    >>> molar_masses = {'Ethanol': M.fromStr('46.08c g/mol'), 'Propan-1-ol': M.fromStr('60.11c g/mol'), 'Butan-1-ol': M.fromStr('74.14c g/mol'), 'Pentan-1-ol': M.fromStr('88.17c g/mol')}
+    >>> results_df_1['Molar Mass of Alcohol (g/mol)'] = results_df_1.apply(lambda x: x['Mass of Alcohol (g)'] / molar_masses[x['Alcohol tested']], axis=1)
+    >>> results_df_1['Molar Enthalpy of Combustion (kJ/mol)'] = - results_df_1['Q of H2O (kJ)'] / results_df_1['Molar Mass of Alcohol (g/mol)']
+
+**Results Table 1: Individual Molar Enthalpy of Combustion**
+
+.. exceltable:: 
+    :file: output.xls
+    :selection: A1:G24
+    :header: 1
+
+Now, to calculate the average molar enthalpy of combustion for each of the alcohols, the data is grouped by alcohol type and the average is taken.
+
+.. doctest:: python
+
+    >>> results_df_2 = pd.DataFrame()
+    >>> results_df_2['Alcohol'] = results_df_1['Alcohol tested'].unique()
+    >>> grouped_data = list(results_df_1.groupby('Alcohol tested')['Molar Enthalpy of Combustion (kJ/mol)'])
+    >>> grouped_data_dict = {i[0]: i[1] for i in grouped_data}
+    >>> results_df_2['Average Molar Enthalpy of Combustion (kJ/mol)'] = [M.average(list(grouped_data_dict[i])).percent() for i in results_df_2['Alcohol']]
+    >>> results_df_2['Accepted Molar Enthalpy of Combustion (kJ/mol)'] = [M.fromStr('-1367c kJ/mol'), M.fromStr('-2021c kJ/mol'), M.fromStr('-2676c kJ/mol'), M.fromStr('-3329c kJ/mol')]
+    >>> results_df_2['Percent Error (%)'] = results_df_2.apply(lambda x: ((x['Accepted Molar Enthalpy of Combustion (kJ/mol)'] - x['Average Molar Enthalpy of Combustion (kJ/mol)']) * 100 / x['Accepted Molar Enthalpy of Combustion (kJ/mol)']), axis=1)
+
+**Results Table 2: Average Molar Enthalpy of Combustion**
+
+.. exceltable:: 
+    :file: output.xls
+    :selection: J1:M5
+    :header: 1
+
+
+Finally, we can convert the Measurement columns back into standard numeric columns.
+
+.. doctest:: python
+
+    >>> final_results_df_1 = results_df_1.copy()
+    >>> for i in range(4):
+    ...     M.exportColumn(final_results_df_1, results_df_1.iloc[:, i + 3])
+    >>> final_results_df_2 = results_df_2.copy()
+    >>> final_results_df_2 = results_df_2.copy()
+    >>> for i in range(3):
+    ...     M.exportColumn(final_results_df_2, results_df_2.iloc[:, i + 1], addUncertainty=i==0)
+
+**Final Results Table 1: Individual Molar Enthalpy of Combustion**
+
+.. exceltable:: 
+    :file: output.xls
+    :selection: A31:K54
+    :header: 1
+
+**Final Results Table 2: Average Molar Enthalpy of Combustion**
+
+.. exceltable:: 
+    :file: output.xls
+    :selection: P31:T35
+    :header: 1
```

### Comparing `pymeasurement-1.0.8/docs/make.bat` & `pymeasurement-1.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymeasurement-1.0.8/docs/operations.rst` & `pymeasurement-1.0.9/docs/operations.rst`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-Measurement Operations
-=======================
-
-The following operations are available for measurements:
-
-* ``+``: Add two measurements together.
-* ``-``: Subtract two measurements.
-* ``*``: Multiply two measurements or a measurement and a float together.
-* ``/``: Divide two measurements or a measurement and a float.
-* ``-``: Negate a measurement.
-* ``**``: Raise a measurement to an integer power.
-
-
-All of these operations return a new measurement object.
-
-.. testsetup:: *
-
-    from pymeasurement import Measurement as M
-
-.. doctest:: python
-
-        >>> a = M.fromStr('3.14d m/s')
-
-        >>> b = M.fromStr('2.71d m/s')
-
-        >>> a + b
-        5.85 +/- 0.02 m/s
-
-        >>> a - b
-        0.43 +/- 0.02 m/s
-
-        >>> a * b
-        8.51 +/- 0.69% m^2/s^2
-
-        >>> a / b
-        1.16 +/- 0.69%
-        
-        >>> a * 2
-        6.28 +/- 0.32% m/s
-        
-        >>> a / 2
-        1.57 +/- 0.32% m/s
-        
-        >>> -a
-        -3.14 +/- 0.01 m/s
-        
-        >>> a ** 2
-        9.86 +/- 0.64% m^2/s^2
-        
-
+Measurement Operations
+=======================
+
+The following operations are available for measurements:
+
+* ``+``: Add two measurements together.
+* ``-``: Subtract two measurements.
+* ``*``: Multiply two measurements or a measurement and a float together.
+* ``/``: Divide two measurements or a measurement and a float.
+* ``-``: Negate a measurement.
+* ``**``: Raise a measurement to an integer power.
+
+
+All of these operations return a new measurement object.
+
+.. testsetup:: *
+
+    from pymeasurement import Measurement as M
+
+.. doctest:: python
+
+        >>> a = M.fromStr('3.14d m/s')
+
+        >>> b = M.fromStr('2.71d m/s')
+
+        >>> a + b
+        5.85 +/- 0.02 m/s
+
+        >>> a - b
+        0.43 +/- 0.02 m/s
+
+        >>> a * b
+        8.51 +/- 0.69% m^2/s^2
+
+        >>> a / b
+        1.16 +/- 0.69%
+        
+        >>> a * 2
+        6.28 +/- 0.32% m/s
+        
+        >>> a / 2
+        1.57 +/- 0.32% m/s
+        
+        >>> -a
+        -3.14 +/- 0.01 m/s
+        
+        >>> a ** 2
+        9.86 +/- 0.64% m^2/s^2
+        
+
```

### Comparing `pymeasurement-1.0.8/docs/table_operations.rst` & `pymeasurement-1.0.9/docs/table_operations.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-Table Operations
-================
-
-pymeasurement can be used with Pandas DataFrames to perform precision-based uncertainty calculations on tables of data.
-
-**Original Data Table**
-
-.. exceltable:: 
-    :file: _static\example.xls
-    :header: 1
-    :selection: A1:C7
-
-In order to acheive this, the DataFrame is converted into Measurement objects for calculations using the below. 
-
-All data can be normalized in this step as well.
-
-.. doctest:: python
-
-    >>> import pandas as pd
-    >>> df = pd.read_excel('_static\example.xlsx')
-    >>> from pymeasurement import Measurement as M
-    >>> converted = pd.DataFrame()
-    >>> converted['Mass (± 0.001 kg)'] = M.importColumn(df['Mass (± 0.001 kg)'], d=True, un='kg', decimals=3)
-    >>> converted['Average Acceleration (m/s^2)'] = M.importColumn(df['Average Acceleration (m/s^2)'], uncertaintyColumn=df['Average Acceleration Percent Uncertainty (%)'], df=df, up=True, un='m/s^2', decimals=2)
-
-**Converted Data Table**
-
-.. exceltable:: 
-    :file: _static\example.xls
-    :header: 1
-    :selection: F1:G7
-
-Now calculations can easily be performed on the DataFrame using the Measurement objects.
-
-.. doctest:: python
-
-    >>> converted['Force (N)'] = converted['Mass (± 0.001 kg)'] * converted['Average Acceleration (m/s^2)']
-
-**Calculated Data Table**
-
-.. exceltable:: 
-    :file: _static\example.xls
-    :header: 1
-    :selection: J1:L7
-
-Once the calculations are complete, the DataFrame can be converted back into a numeric types using the below.
-
-.. doctest:: python
-
-    >>> final_table = converted.copy()
-    >>> M.exportColumn(final_table, converted['Mass (± 0.001 kg)'], addUncertainty=False)
-    >>> M.exportColumn(final_table, converted['Average Acceleration (m/s^2)'])
-    >>> M.exportColumn(final_table, converted['Force (N)'], asPercent=False)
-
-.. exceltable:: 
-    :file: _static\example.xls
-    :header: 1
-    :selection: O1:S7
+Table Operations
+================
+
+pymeasurement can be used with Pandas DataFrames to perform precision-based uncertainty calculations on tables of data.
+
+**Original Data Table**
+
+.. exceltable:: 
+    :file: example.xls
+    :selection: A1:C7
+    :header: 1
+
+In order to acheive this, the DataFrame is converted into Measurement objects for calculations using the below. 
+
+All data can be normalized in this step as well.
+
+.. doctest:: python
+
+    >>> import pandas as pd
+    >>> df = pd.read_excel('example.xlsx')
+    >>> from pymeasurement import Measurement as M
+    >>> converted = pd.DataFrame()
+    >>> converted['Mass (± 0.001 kg)'] = M.importColumn(df['Mass (± 0.001 kg)'], d=True, un='kg', decimals=3)
+    >>> converted['Average Acceleration (m/s^2)'] = M.importColumn(df['Average Acceleration (m/s^2)'], uncertaintyColumn=df['Average Acceleration Percent Uncertainty (%)'], df=df, up=True, un='m/s^2', decimals=2)
+
+**Converted Data Table**
+
+.. exceltable:: 
+    :file: example.xls
+    :selection: F1:G7
+    :header: 1
+
+Now calculations can easily be performed on the DataFrame using the Measurement objects.
+
+.. doctest:: python
+
+    >>> converted['Force (N)'] = converted['Mass (± 0.001 kg)'] * converted['Average Acceleration (m/s^2)']
+
+**Calculated Data Table**
+
+.. exceltable:: 
+    :file: example.xls
+    :selection: J1:L7
+    :header: 1
+
+Once the calculations are complete, the DataFrame can be converted back into a numeric types using the below.
+
+.. doctest:: python
+
+    >>> final_table = converted.copy()
+    >>> M.exportColumn(final_table, converted['Mass (± 0.001 kg)'], addUncertainty=False)
+    >>> M.exportColumn(final_table, converted['Average Acceleration (m/s^2)'])
+    >>> M.exportColumn(final_table, converted['Force (N)'], asPercent=False)
+
+.. exceltable:: 
+    :file: example.xls
+    :selection: O1:S7
+    :header: 1
```

### Comparing `pymeasurement-1.0.8/docs/test.ipynb` & `pymeasurement-1.0.9/docs/test.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9860763888888888%*

 * *Differences: {"'cells'": '{0: {\'execution_count\': 10, \'source\': {insert: [(3, "df = '*

 * *            'pd.read_excel(\'Combustion_Lab_1920_Student_Data.xlsx\')")], delete: [3]}}, 1: '*

 * *            "{'execution_count': 11, 'outputs': {0: {'execution_count': 11}}}, 2: "*

 * *            "{'execution_count': 12}, 3: {'execution_count': 13}, 4: {'execution_count': 14}, 5: "*

 * *            "{'execution_count': 15, 'outputs': {0: {'execution_count': 15}}}, 6: "*

 * *            "{'execution_count': 16, 'outputs': {0: {'execution_count': 16 […]*

```diff
@@ -1,24 +1,24 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 41,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import pandas as pd\n",
                 "from pymeasurement import Measurement as M, SigFig\n",
                 "\n",
-                "df = pd.read_excel('_static\\Combustion_Lab_1920_Student_Data.xlsx')"
+                "df = pd.read_excel('Combustion_Lab_1920_Student_Data.xlsx')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 42,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -404,15 +404,15 @@
                             "18                69.6 +/- 0.1 \u00baC  \n",
                             "19                76.7 +/- 0.1 \u00baC  \n",
                             "20                71.8 +/- 0.1 \u00baC  \n",
                             "21                71.6 +/- 0.1 \u00baC  \n",
                             "22                60.6 +/- 0.1 \u00baC  "
                         ]
                     },
-                    "execution_count": 42,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "decimals = [3, 3, 3, 1, 1]\n",
                 "units = ['g', 'g', 'g', '\u00baC', '\u00baC']\n",
@@ -421,46 +421,46 @@
                 "\n",
                 "\n",
                 "df"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 43,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [],
             "source": [
                 "heat_capacity = M.fromStr('4.18c J/g*\u00baC')\n",
                 "j_to_kj = M.fromStr('0.001c kJ/J')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 44,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [],
             "source": [
                 "results_df_1 = df.iloc[:, 0:3]\n",
                 "results_df_1['Q of H2O (kJ)'] = df['Mass of water (+/- 0.001 g)'] * heat_capacity * (df['Final temperature (+/- 0.1 \u00baC)'] - df['Initial temperature (+/- 0.1 \u00baC)']) * j_to_kj"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 45,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [],
             "source": [
                 "results_df_1['Mass of Alcohol (g)'] = df['Initial mass of spirit burner (+/- 0.001 g)'] - df['Final mass of spirit burner (+/- 0.001 g)']\n",
                 "molar_masses = {'Ethanol': M.fromStr('46.08c g/mol'), 'Propan-1-ol': M.fromStr('60.11c g/mol'), 'Butan-1-ol': M.fromStr('74.14c g/mol'), 'Pentan-1-ol': M.fromStr('88.17c g/mol')}\n",
                 "results_df_1['Molar Mass of Alcohol (g/mol)'] = results_df_1.apply(lambda x: x['Mass of Alcohol (g)'] / molar_masses[x['Alcohol tested']], axis=1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 46,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -772,28 +772,28 @@
                             "18         0.01885 +/- 0.12% mol             -1.51E+3 +/- 0.54% kJ/mol  \n",
                             "19          0.0103 +/- 0.22% mol             -1.42E+3 +/- 0.59% kJ/mol  \n",
                             "20         0.01330 +/- 0.17% mol             -1.01E+3 +/- 0.56% kJ/mol  \n",
                             "21         0.01587 +/- 0.14% mol                 -958 +/- 0.53% kJ/mol  \n",
                             "22         0.01341 +/- 0.17% mol                 -882 +/- 0.67% kJ/mol  "
                         ]
                     },
-                    "execution_count": 46,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "results_df_1['Molar Enthalpy of Combustion (kJ/mol)'] = - results_df_1['Q of H2O (kJ)'] / results_df_1['Molar Mass of Alcohol (g/mol)']\n",
                 "\n",
                 "results_df_1"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 47,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -862,15 +862,15 @@
                             "  Accepted Molar Enthalpy of Combustion (kJ/mol) Percent Error (%)  \n",
                             "0                                   -1367 kJ/mol      63.57 +/- 9%  \n",
                             "1                                   -2021 kJ/mol     74.869 +/- 7%  \n",
                             "2                                   -2676 kJ/mol   71.543 +/- 1.6%  \n",
                             "3                                   -3329 kJ/mol      63.30 +/- 6%  "
                         ]
                     },
-                    "execution_count": 47,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "results_df_2 = pd.DataFrame()\n",
                 "results_df_2['Alcohol'] = results_df_1['Alcohol tested'].unique()\n",
@@ -881,15 +881,15 @@
                 "results_df_2['Percent Error (%)'] = results_df_2.apply(lambda x: ((x['Accepted Molar Enthalpy of Combustion (kJ/mol)'] - x['Average Molar Enthalpy of Combustion (kJ/mol)']) * 100 / x['Accepted Molar Enthalpy of Combustion (kJ/mol)']), axis=1)\n",
                 "\n",
                 "results_df_2"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 48,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -1397,30 +1397,30 @@
                             "18                                               0.54    \n",
                             "19                                               0.59    \n",
                             "20                                               0.56    \n",
                             "21                                               0.53    \n",
                             "22                                               0.67    "
                         ]
                     },
-                    "execution_count": 48,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "final_results_df_1 = results_df_1.copy()\n",
                 "for i in range(4):\n",
                 "  M.exportColumn(final_results_df_1, results_df_1.iloc[:, i + 3])\n",
                 "\n",
                 "final_results_df_1"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 49,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -1500,15 +1500,15 @@
                             "  Accepted Molar Enthalpy of Combustion (kJ/mol) Percent Error (%)  \n",
                             "0                                          -1367             63.57  \n",
                             "1                                          -2021            74.869  \n",
                             "2                                          -2676            71.543  \n",
                             "3                                          -3329             63.30  "
                         ]
                     },
-                    "execution_count": 49,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "final_results_df_2 = results_df_2.copy()\n",
                 "for i in range(3):\n",
```

### Comparing `pymeasurement-1.0.8/docs/_static/Combustion_Lab_1920_Student_Data.xls` & `pymeasurement-1.0.9/docs/Combustion_Lab_1920_Student_Data.xls`

 * *Files identical despite different names*

### Comparing `pymeasurement-1.0.8/docs/_static/Combustion_Lab_1920_Student_Data.xlsx` & `pymeasurement-1.0.9/docs/Combustion_Lab_1920_Student_Data.xlsx`

 * *Files identical despite different names*

### Comparing `pymeasurement-1.0.8/docs/_static/example.xls` & `pymeasurement-1.0.9/docs/example.xls`

 * *Files identical despite different names*

### Comparing `pymeasurement-1.0.8/docs/_static/example.xlsx` & `pymeasurement-1.0.9/docs/example.xlsx`

 * *Files identical despite different names*

### Comparing `pymeasurement-1.0.8/docs/_static/output.xls` & `pymeasurement-1.0.9/docs/output.xls`

 * *Files identical despite different names*

### Comparing `pymeasurement-1.0.8/docs/_static/output.xlsx` & `pymeasurement-1.0.9/docs/output.xlsx`

 * *Files identical despite different names*

### Comparing `pymeasurement-1.0.8/src/pymeasurement/measurement.py` & `pymeasurement-1.0.9/src/pymeasurement/measurement.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,637 +1,637 @@
-from pymeasurement.sigfig import SigFig
-import math
-
-class Measurement:
-  """
-  Measurement
-  A class to represent a SigFig sample with a SigFig uncertainty and corresponding units.
-  This class can be used to perform calculations with uncertainty propagation.
-  Units are also automatically derived through operations with other measurements.
-
-  :param sample: The sample value as a SigFig object or a string.
-  :type sample: SigFig or str
-  :param precision: The number of significant figures to use when printing the number. If None, the number of significant figures will be automatically determined.
-  :type precision: int
-  :param uncertainty: The uncertainty of the sample as a SigFig object or a string.
-  :type uncertainty: SigFig or str
-  :param uncertaintyPercent: If True, the uncertainty will be interpreted as a percentage of the sample value.
-  :type uncertaintyPercent: bool
-  :param digital: If True, the uncertainty will be automatically determined based on the precision of the device.
-  :type digital: bool
-  :param analog: If True, the uncertainty will be automatically determined based on the precision of the device.
-  :type analog: bool
-  :param units: The units of the measurement as a string.
-  :type units: str
-  :param P: The number of significant figures to use when printing the number. If None, the number of significant figures will be automatically determined.
-  :type P: int
-  :param U: The uncertainty of the sample as a SigFig object or a string.
-  :type U: SigFig or str
-  :param UP: If True, the uncertainty will be interpreted as a percentage of the sample value.
-  :type UP: bool
-  :param D: If True, the uncertainty will be automatically determined based on the precision of the device.
-  :type D: bool
-  :param A: If True, the uncertainty will be automatically determined based on the precision of the device.
-  :type A: bool
-  :param UN: The units of the measurement as a string.
-  :type UN: str
-  """
-  def __init__(self, sample, precision=None, uncertainty=None, uncertaintyPercent=False, digital=False, analog=False, units=None, P=None, U=None, UP=False, D=False, A=False, UN=None):
-    """
-    Measurement Constructor
-    """
-    if P is not None:
-      precision = P
-    if U is not None:
-      uncertainty = U
-    if UP:
-      uncertaintyPercent = UP
-    if D:
-      digital = D
-    if A:
-      analog = A
-    if UN is not None:
-      units = UN
-    
-    if not isinstance(sample, SigFig):
-      if '(' in sample or '[' in sample:
-        sample, precision = sample.split()
-        try:
-          precision = int(precision[1:-1]) #Precision in Sig Figs
-        except ValueError:
-          raise Exception('Measurement Error: Invalid Literal for Sig Fig Precision.')
-    if not isinstance(sample, SigFig):
-      if precision == float('inf'):
-        self.sample = SigFig(sample, constant=True)
-      else:
-        self.sample = SigFig(sample, sigfigs=precision) 
-    else:
-      self.sample = sample
-
-    #Automatic Determination of Uncertainty based on Device
-    self.uncertainty = None
-    if analog:
-      self.uncertainty = SigFig(f"5e{self.sample.decimals}", decimals=self.sample.decimals)
-    elif digital:
-      self.uncertainty = SigFig(f"1e{self.sample.decimals}", decimals=self.sample.decimals)
-    
-    #Main Override
-    if uncertainty is not None:
-      if not isinstance(uncertainty, SigFig):
-        if '%' in uncertainty:
-          uncertaintyPercent = True
-          uncertainty = uncertainty.replace('%', '')
-      self.uncertainty = SigFig(uncertainty, decimals=self.sample.decimals) if not isinstance(uncertainty, SigFig) else uncertainty
-    self.uncertaintyPercent = uncertaintyPercent
-
-    #Chemistry Percent Rules(if <2%, 2 sig figs. Else 1 sig fig)
-    if self.uncertainty is not None and self.uncertaintyPercent:
-      self.uncertainty = SigFig(str(self.uncertainty.decimalValue), sigfigs=(2 if self.uncertainty < SigFig('2', constant=True) else 1))
-
-    #Determine Units
-    #Will use units class to allow for conversions later.
-    self.units = units
-    self.nUnits = [i.strip('() ') for i in self.units.split('*')] if self.units is not None else []
-    self.dUnits = []
-    if self.units is not None:
-      if '/' in units:
-        nUnitsStr, dUnitsStr = self.units.split('/')
-        nUnitsStr = nUnitsStr.strip('() ')
-        dUnitsStr = dUnitsStr.strip('() ')
-        self.nUnits = [i.strip('() ') for i in nUnitsStr.split('*')]
-        self.dUnits = [i.strip('() ') for i in dUnitsStr.split('*')]
-        if '^' in nUnitsStr:
-          newNUnits = []
-          for i in self.nUnits:
-            if '^' in i:
-              i, repeat = i.split('^')
-              for n in range(int(repeat)-1):
-                newNUnits.append(i)
-            newNUnits.append(i)
-          self.nUnits = newNUnits
-        if '^' in dUnitsStr:
-          newDUnits = []
-          for i in self.dUnits:
-            if '^' in i:
-              i, repeat = i.split('^')
-              for n in range(int(repeat)-1):
-                newDUnits.append(i)
-            newDUnits.append(i)
-          self.dUnits = newDUnits
-    newNUnits = self.nUnits
-    newDUnits = self.dUnits
-    for i in self.nUnits:
-      if i in newDUnits:
-        newNUnits.remove(i)
-        newDUnits.remove(i)
-    #Sort units alphabetically
-    self.nUnits=sorted(newNUnits)
-    self.dUnits=sorted(newDUnits)
-    #Reformat units string
-    self.units = Measurement.formatUnits(self.nUnits, self.dUnits)
-
-  def fromStr(string):
-    """Creates a Measurement object from a string.
-    The string must be in the form of a number, uncertainty, and units.
-    The uncertainty can be in the form of a percentage or a number.
-    A 'a' or 'd' can be used to indicate an analog or digital device for automatic uncertainty determination.
-
-    :param string: The string to create the Measurement object from.
-    :type string: str
-    :return: The Measurement object created from the string.
-    :rtype: Measurement
-    """
-    sample = string.strip()
-    uncertainty = None
-    units = None
-    values = sample.split()
-    if '+/-' in sample or '+-' in sample:
-      if len(values) == 3:
-        if '+/-' in sample:
-          sample, uncertainty = string.split('+/-')
-        elif '+-' in sample:
-          sample, uncertainty = string.split('+-')
-      elif len(values) >= 4:
-        sample, _, uncertainty, *units = values
-        if len(units) == 2: # Assuming form will mol H2O
-          if '_' not in units[1]:
-            from pymeasurement.util.chem.compound import Compound
-            units[1] = str(Compound(units[1])) # Format Compound String
-        units = ' '.join(units)
-    else:
-      if len(values) >= 2:
-        sample, *units = values
-        if len(units) == 2: # Assuming form will mol H2O
-          if '_' not in units[1]:
-            from pymeasurement.util.chem.compound import Compound
-            units[1] = str(Compound(units[1])) # Format Compound String
-        units = ' '.join(units)
-    precision = None
-    digital = False
-    analog = False
-    if uncertainty is None:
-      if 'c' in sample:
-        precision = float('inf')
-        sample = sample.replace('c', '')
-      elif 'd' in sample:
-        digital = True
-        sample = sample.replace('d', '')
-      elif 'a' in sample:
-        analog = True
-        sample = sample.replace('a', '')
-    return Measurement(sample.strip(), precision=precision, uncertainty=(uncertainty.strip() if isinstance(uncertainty, str) else uncertainty), digital=digital, analog=analog, units=units)
-
-  def fromFloat(f, units=''): #Assume float is a constant with infinite precision and no uncertainty.
-    """
-    Creates a Measurement constant from a float.
-
-    :param f: The float to create the Measurement constant from.
-    :type f: float
-    :param units: The units of the Measurement constant.
-    :type units: str
-    :return: The Measurement constant created from the float.
-    :rtype: Measurement
-    """
-    return Measurement.fromStr(f'{f}c {units}')
-  
-  def toAbsolute(self):
-    """
-    Converts the uncertainty to an absolute value. Note that this mutates the object.
-
-    :return: The Measurement object with the uncertainty converted to an absolute value.
-    :rtype: Measurement
-    """
-    if self.uncertaintyPercent and isinstance(self.uncertainty, SigFig):
-      self.uncertaintyPercent = False
-      self.uncertainty *= (self.sample / SigFig('100', constant=True)).abs()
-      self.uncertainty = SigFig(str(self.uncertainty.decimalValue), decimals=self.sample.decimals)
-    return self
-
-  def toPercent(self):
-    """
-    Converts the uncertainty to a percentage. Note that this mutates the object.
-
-    :return: The Measurement object with the uncertainty converted to a percentage.
-    :rtype: Measurement
-    """
-    if not self.uncertaintyPercent and isinstance(self.uncertainty, SigFig):
-      self.uncertaintyPercent = True
-      self.uncertainty = SigFig(self.uncertainty.value, constant=True) * SigFig((SigFig('100', constant=True) / self.sample).abs().value, constant=True)
-      self.uncertainty = SigFig(str(self.uncertainty.decimalValue), sigfigs=(2 if self.uncertainty < SigFig('2', constant=True) else 1))
-    return self
-
-  def absolute(m):
-    """
-    Returns a copy of the Measurement with the uncertainty converted to an absolute value.
-
-    :return: A copy of the Measurement with the uncertainty converted to an absolute value.
-    :rtype: Measurement
-    """
-    return m.deepCopy().toAbsolute()
-
-  def percent(m):
-    """
-    Returns a copy of the Measurement with the uncertainty converted to a percentage.
-
-    :return: A copy of the Measurement with the uncertainty converted to a percentage.
-    :rtype: Measurement
-    """
-    return m.deepCopy().toPercent()
-  
-  def deepCopy(self):
-    """
-    Returns a deep copy of the Measurement object.
-
-    :return: A deep copy of the Measurement object.
-    :rtype: Measurement
-    """
-    return Measurement(self.sample.deepCopy(), uncertainty = self.uncertainty.deepCopy() if self.uncertainty is not None else None, uncertaintyPercent = self.uncertaintyPercent, units=self.units)
-  
-  def __str__(self):
-    """
-    Returns a string representation of the Measurement object.
-
-    :return: A string representation of the Measurement object.
-    :rtype: str
-    """
-    return str(self.sample) + (f' +/- {self.uncertainty}' + ('%' if self.uncertaintyPercent else '') if isinstance(self.uncertainty, SigFig) else '') + (f' {Measurement.formatUnits(self.nUnits, self.dUnits)}' if self.units is not None else '')
-
-  def __repr__(self):
-    """
-    Returns a string representation of the Measurement object.
-
-    :return: A string representation of the Measurement object.
-    :rtype: str
-    """
-    return str(self)
-
-  def multUnits(nUnits1, dUnits1, nUnits2, dUnits2):
-    """
-    Multiplies two sets of units.
-
-    :param nUnits1: The numerator units of the first set.
-    :type nUnits1: list
-    :param dUnits1: The denominator units of the first set.
-    :type dUnits1: list
-    :param nUnits2: The numerator units of the second set.
-    :type nUnits2: list
-    :param dUnits2: The denominator units of the second set.
-    :type dUnits2: list
-    :return: The multiplied units.
-    :rtype: tuple
-    """
-    nUnits = nUnits1 + nUnits2
-    dUnits = dUnits1 + dUnits2
-    newNUnits = nUnits
-    newDUnits = dUnits
-    for i in nUnits:
-      if i in newDUnits:
-        newNUnits.remove(i)
-        newDUnits.remove(i)
-    return (sorted(newNUnits), sorted(newDUnits))
-
-  def formatUnits(nUnits, dUnits):
-    """
-    Formats a set of units into a string.
-
-    :param nUnits: The numerator units.
-    :type nUnits: list
-    :param dUnits: The denominator units.
-    :type dUnits: list
-    :return: The formatted units.
-    :rtype: str
-    """
-    combinedNUnits = sorted([i if nUnits.count(i) == 1 else f'{i}^{nUnits.count(i)}' for i in set(nUnits)])
-    combinedDUnits = sorted([i if dUnits.count(i) == 1 else f'{i}^{dUnits.count(i)}' for i in set(dUnits)])
-    nUnitsStr = '1' if not nUnits else '*'.join(combinedNUnits)
-    dUnitsStr = '' if not dUnits else '*'.join(combinedDUnits)
-    if len(combinedNUnits) > 1:
-      nUnitsStr = '(' + nUnitsStr + ')'
-    if len(combinedDUnits) > 1:
-      dUnitsStr = '(' + dUnitsStr + ')'
-    return None if nUnitsStr == '1' and dUnitsStr == '' else nUnitsStr + (f'/{dUnitsStr}' if dUnitsStr else '')
-
-  def __eq__(self, other):
-    """
-    Returns True if the two Measurement objects are equal.
-
-    :param other: The Measurement object to compare.
-    :type other: Measurement
-    :returns: True if the two Measurement objects are equal.
-    :rtype: bool
-    """
-    return self.sample == other.sample
-
-  def __lt__(self, other):
-    """
-    Returns True if the first Measurement object is less than the second.
-
-    :param other: The Measurement object to compare.
-    :type other: Measurement
-    :returns: True if the first Measurement object is less than the second.
-    :rtype: bool
-    """
-    return self.sample < other.sample
-
-  def __gt__(self, other):
-    """
-    Returns True if the first Measurement object is greater than the second.
-
-    :param other: The Measurement object to compare.
-    :type other: Measurement
-    :returns: True if the first Measurement object is greater than the second.
-    :rtype: bool
-    """
-    return self.sample > other.sample
-
-  def __le__(self, other):
-    """
-    Returns True if the first Measurement object is less than or equal to the second.
-
-    :param other: The Measurement object to compare.
-    :type other: Measurement
-    :returns: True if the first Measurement object is less than or equal to the second.
-    :rtype: bool
-    """
-    return self < other or self == other
-
-  def __ge__(self, other):
-    """
-    Returns True if the first Measurement object is greater than or equal to the second.
-
-    :param other: The Measurement object to compare.
-    :type other: Measurement
-    :returns: True if the first Measurement object is greater than or equal to the second.
-    :rtype: bool
-    """
-    return self > other or self == other
-  
-  def __neg__(self):
-    """
-    Returns the negation of the Measurement object.
-
-    :returns: The negation of the Measurement object.
-    :rtype: Measurement
-    """
-    neg = self.deepCopy()
-    neg.sample = -self.sample
-    return neg
-
-  def __add__(self, other):
-    """
-    Returns the sum of the two Measurement objects.
-
-    :param other: The Measurement object to add.
-    :type other: Measurement
-    :returns: The sum of the two Measurement objects.
-    :rtype: Measurement
-    """
-    if self.nUnits != other.nUnits or self.dUnits != other.dUnits:
-      raise Exception(f'Measurement Error: Cannot add {self} and {other} with different units.')
-    uSum = SigFig('0', constant=True)
-    uncertainties = [Measurement.absolute(i).uncertainty for i in [self, other] if i.uncertainty is not None]
-    for u in uncertainties:
-      uSum += u
-    return Measurement(self.sample + other.sample, uncertainty=uSum if uncertainties else None, units=self.units)
-  
-  def __radd__(self, other):
-    """
-    Returns the sum of the two Measurement objects.
-
-    :param other: The Measurement object to add to.
-    :type other: Measurement
-    :returns: The sum of the two Measurement objects.
-    :rtype: Measurement
-    """
-    return self + other
-  
-  def __sub__(self, other):
-    """
-    Returns the difference of the two Measurement objects.
-
-    :param other: The Measurement object to subtract.
-    :type other: Measurement
-    :returns: The difference of the two Measurement objects.
-    :rtype: Measurement
-    """
-    return -other + self
-
-  def __rsub__(self, other):
-    """
-    Returns the difference of the two Measurement objects.
-
-    :param other: The Measurement object to subtract from.
-    :type other: Measurement
-    :returns: The difference of the two Measurement objects.
-    :rtype: Measurement
-    """
-    return -self + other
-
-  def __mul__(self, other):
-    """
-    Returns the product of the two Measurement objects.
-
-    :param other: The Measurement object to multiply by.
-    :type other: Measurement
-    :returns: The product of the two Measurement objects.
-    :rtype: Measurement
-    """
-    if isinstance(other, float) or isinstance(other, int):
-      other = Measurement.fromFloat(other)
-    uSum = SigFig('0', constant=True)
-    uncertainties = [Measurement.percent(i).uncertainty for i in [self, other] if i.uncertainty is not None]
-    for u in uncertainties:
-      uSum += u
-    nUnits, dUnits = Measurement.multUnits(self.nUnits, self.dUnits, other.nUnits, other.dUnits)
-    return Measurement(self.sample * other.sample, uncertainty=uSum if uncertainties else None, uncertaintyPercent=True, units=Measurement.formatUnits(nUnits, dUnits))
-  
-  def __rmul__(self, other):
-    """
-    Returns the product of the two Measurement objects.
-
-    :param other: The Measurement object to multiply by.
-    :type other: Measurement
-    :returns: The product of the two Measurement objects.
-    :rtype: Measurement
-    """
-    return self * other
-
-  def __truediv__(self, other):
-    """
-    Returns the quotient of the two Measurement objects.
-
-    :param other: The Measurement object to divide by.
-    :type other: Measurement
-    :returns: The quotient of the two Measurement objects.
-    :rtype: Measurement
-    """
-    if isinstance(other, float) or isinstance(other, int):
-      other = Measurement.fromFloat(other)
-    uSum = SigFig('0', constant=True)
-    uncertainties = [Measurement.percent(i).uncertainty for i in [self, other] if i.uncertainty is not None]
-    for u in uncertainties:
-      uSum += u
-    nUnits, dUnits = Measurement.multUnits(self.nUnits, self.dUnits, other.dUnits, other.nUnits)
-    return Measurement(self.sample / other.sample, uncertainty=uSum if uncertainties else None, uncertaintyPercent=True, units=Measurement.formatUnits(nUnits, dUnits))
-    
-  def __rtruediv__(self, other):
-    """
-    Returns the quotient of the two Measurement objects.
-
-    :param other: The Measurement object to divide by.
-    :type other: Measurement
-    :returns: The quotient of the two Measurement objects.
-    :rtype: Measurement
-    """
-    return other / self
-
-  def __pow__(self, integer):
-    """
-    Returns the Measurement object raised to the given integer power.
-
-    :param integer: The integer power to raise the Measurement object to.
-    :type integer: int
-    :returns: The Measurement object raised to the given integer power.
-    :rtype: Measurement
-    """
-    product = Measurement('1', precision=float('inf'))
-    for i in range(integer):
-      product *= self
-    return product
-
-  def sum(measurements):
-    """
-    Returns the sum of the given list of Measurement objects.
-
-    :param measurements: The list of Measurement objects.
-    :type measurements: list
-    :returns: The sum of the given list of Measurement objects.
-    :rtype: Measurement
-    """
-    if not measurements:
-      return Measurement.fromStr('0c')
-    s = measurements[0]
-    for i in measurements[1:]:
-      s += i
-    return s
-
-  def max(measurements):
-    """
-    Returns the maximum of the given list of Measurement objects.
-
-    :param measurements: The list of Measurement objects.
-    :type measurements: list
-    :returns: The maximum of the given list of Measurement objects.
-    :rtype: Measurement
-    """
-    m = measurements[0]
-    for i in measurements[1:]:
-      if m < i:
-        m = i
-    return m
-
-  def min(measurements):
-    """
-    Returns the minimum of the given list of Measurement objects.
-
-    :param measurements: The list of Measurement objects.
-    :type measurements: list
-    :returns: The minimum of the given list of Measurement objects.
-    :rtype: Measurement
-    """
-    m = measurements[0]
-    for i in measurements[1:]:
-      if m > i:
-        m = i
-    return m
-
-  def average(measurements):
-    """
-    Returns the average of the given list of Measurement objects. Uses (max - min) / (2 * sqrt(n)) as the uncertainty.
-
-    :param measurements: The list of Measurement objects.
-    :type measurements: list
-    :returns: The average of the given list of Measurement objects.
-    :rtype: Measurement
-    """
-    avg_sample = Measurement.sum(measurements) / len(measurements)
-    avg_uncertainty = (Measurement.max(measurements) - Measurement.min(measurements)).sample / (2 * math.sqrt(len(measurements)))
-    return Measurement(avg_sample.sample, uncertainty=avg_uncertainty.value, units=avg_sample.units)
-
-  def convert(sample, uncertainty=None, uncertaintyPercent=False, units='', analog=False, digital=False, constant=False, u=None, up=False, a=False, d=False, un='', decimals=None):
-    """
-    Returns a Measurement object with the given sample, uncertainty, and units.
-    
-    :param sample: The sample of the Measurement object.
-    :type sample: float or str
-    :param uncertainty: The uncertainty of the Measurement object.
-    :type uncertainty: float or str
-    :param uncertaintyPercent: Whether the uncertainty is a percent.
-    :type uncertaintyPercent: bool
-    :param units: The units of the Measurement object.
-    :type units: str
-    :param analog: Whether the Measurement object is analog.
-    :type analog: bool
-    :param digital: Whether the Measurement object is digital.
-    :type digital: bool
-    :param constant: Whether the Measurement object is constant.
-    :type constant: bool
-    :param u: The uncertainty of the Measurement object.
-    :type u: float or str
-    :param up: Whether the uncertainty is a percent.
-    :type up: bool
-    :param a: Whether the Measurement object is analog.
-    :type a: bool
-    :param d: Whether the Measurement object is digital.
-    :type d: bool
-    :param un: The units of the Measurement object.
-    :type un: str
-    :param decimals: The number of decimals to round to.
-    :type decimals: int
-    """
-    if u is not None:
-      uncertainty = u
-    if up:
-      uncertaintyPercent = up
-    if a:
-      analog = a
-    if d:
-      digital = d
-    if un:
-      units = un
-
-    return Measurement(SigFig(str(sample), decimals=-decimals if decimals is not None else None), uncertaintyPercent=uncertaintyPercent, uncertainty=str(uncertainty) if uncertainty is not None else None, precision=float('inf') if constant else None, units=units, analog=analog, digital=digital)
-  
-  def importColumn(column, uncertaintyColumn=None, df=None, **kwargs):
-    """
-    Convert a numeric Pandas DataFrame column to Measurement objects.
-    
-    :param column: The numeric Pandas DataFrame column.
-    :type column: pandas.core.series.Series
-    :param kwargs: Keyword arguments to pass to Measurement.convert.
-    :type kwargs: dict
-    """
-    if uncertaintyColumn is None:
-      return column.apply(Measurement.convert, **kwargs)
-    else:
-      return df.apply(lambda x: Measurement.convert(x[column.name], u=x[uncertaintyColumn.name], **kwargs), axis=1)
-
-  def exportColumn(savedf, column, addUncertainty=True, asPercent=True):
-    """
-    Convert a Measurement Pandas DataFrame column to numeric values.
-
-    :param savedf: The Pandas DataFrame to save to.
-    :type savedf: pandas.core.frame.DataFrame
-    :param column: The Measurement Pandas DataFrame column.
-    :type column: pandas.core.series.Series
-    :param addUncertainty: Whether to add the uncertainty to the DataFrame.
-    :type addUncertainty: bool
-    :param asPercent: Whether to add the uncertainty as a percent.
-    :type asPercent: bool
-    """
-    savedf[column.name] = column.apply(lambda x: x.sample)
-    if addUncertainty:
-      label, units = (' ('.join(column.name.split(' (')[:-1]), ' (' + column.name.split(' (')[-1]) if ' (' in column.name else (column.name, '')
-      if asPercent:
-        savedf.insert(savedf.columns.get_loc(column.name) + 1, f'{label} Percent Uncertainty (%)', column.apply(lambda x: x.percent().uncertainty))
-      else:
-        savedf.insert(savedf.columns.get_loc(column.name) + 1, f'{label} Absolute Uncertainty{units}', column.apply(lambda x: x.absolute().uncertainty))
+from pymeasurement.sigfig import SigFig
+import math
+
+class Measurement:
+  """
+  Measurement
+  A class to represent a SigFig sample with a SigFig uncertainty and corresponding units.
+  This class can be used to perform calculations with uncertainty propagation.
+  Units are also automatically derived through operations with other measurements.
+
+  :param sample: The sample value as a SigFig object or a string.
+  :type sample: SigFig or str
+  :param precision: The number of significant figures to use when printing the number. If None, the number of significant figures will be automatically determined.
+  :type precision: int
+  :param uncertainty: The uncertainty of the sample as a SigFig object or a string.
+  :type uncertainty: SigFig or str
+  :param uncertaintyPercent: If True, the uncertainty will be interpreted as a percentage of the sample value.
+  :type uncertaintyPercent: bool
+  :param digital: If True, the uncertainty will be automatically determined based on the precision of the device.
+  :type digital: bool
+  :param analog: If True, the uncertainty will be automatically determined based on the precision of the device.
+  :type analog: bool
+  :param units: The units of the measurement as a string.
+  :type units: str
+  :param P: The number of significant figures to use when printing the number. If None, the number of significant figures will be automatically determined.
+  :type P: int
+  :param U: The uncertainty of the sample as a SigFig object or a string.
+  :type U: SigFig or str
+  :param UP: If True, the uncertainty will be interpreted as a percentage of the sample value.
+  :type UP: bool
+  :param D: If True, the uncertainty will be automatically determined based on the precision of the device.
+  :type D: bool
+  :param A: If True, the uncertainty will be automatically determined based on the precision of the device.
+  :type A: bool
+  :param UN: The units of the measurement as a string.
+  :type UN: str
+  """
+  def __init__(self, sample, precision=None, uncertainty=None, uncertaintyPercent=False, digital=False, analog=False, units=None, P=None, U=None, UP=False, D=False, A=False, UN=None):
+    """
+    Measurement Constructor
+    """
+    if P is not None:
+      precision = P
+    if U is not None:
+      uncertainty = U
+    if UP:
+      uncertaintyPercent = UP
+    if D:
+      digital = D
+    if A:
+      analog = A
+    if UN is not None:
+      units = UN
+    
+    if not isinstance(sample, SigFig):
+      if '(' in sample or '[' in sample:
+        sample, precision = sample.split()
+        try:
+          precision = int(precision[1:-1]) #Precision in Sig Figs
+        except ValueError:
+          raise Exception('Measurement Error: Invalid Literal for Sig Fig Precision.')
+    if not isinstance(sample, SigFig):
+      if precision == float('inf'):
+        self.sample = SigFig(sample, constant=True)
+      else:
+        self.sample = SigFig(sample, sigfigs=precision) 
+    else:
+      self.sample = sample
+
+    #Automatic Determination of Uncertainty based on Device
+    self.uncertainty = None
+    if analog:
+      self.uncertainty = SigFig(f"5e{self.sample.decimals}", decimals=self.sample.decimals)
+    elif digital:
+      self.uncertainty = SigFig(f"1e{self.sample.decimals}", decimals=self.sample.decimals)
+    
+    #Main Override
+    if uncertainty is not None:
+      if not isinstance(uncertainty, SigFig):
+        if '%' in uncertainty:
+          uncertaintyPercent = True
+          uncertainty = uncertainty.replace('%', '')
+      self.uncertainty = SigFig(uncertainty, decimals=self.sample.decimals) if not isinstance(uncertainty, SigFig) else uncertainty
+    self.uncertaintyPercent = uncertaintyPercent
+
+    #Chemistry Percent Rules(if <2%, 2 sig figs. Else 1 sig fig)
+    if self.uncertainty is not None and self.uncertaintyPercent:
+      self.uncertainty = SigFig(str(self.uncertainty.decimalValue), sigfigs=(2 if self.uncertainty < SigFig('2', constant=True) else 1))
+
+    #Determine Units
+    #Will use units class to allow for conversions later.
+    self.units = units
+    self.nUnits = [i.strip('() ') for i in self.units.split('*')] if self.units is not None else []
+    self.dUnits = []
+    if self.units is not None:
+      if '/' in units:
+        nUnitsStr, dUnitsStr = self.units.split('/')
+        nUnitsStr = nUnitsStr.strip('() ')
+        dUnitsStr = dUnitsStr.strip('() ')
+        self.nUnits = [i.strip('() ') for i in nUnitsStr.split('*')]
+        self.dUnits = [i.strip('() ') for i in dUnitsStr.split('*')]
+        if '^' in nUnitsStr:
+          newNUnits = []
+          for i in self.nUnits:
+            if '^' in i:
+              i, repeat = i.split('^')
+              for n in range(int(repeat)-1):
+                newNUnits.append(i)
+            newNUnits.append(i)
+          self.nUnits = newNUnits
+        if '^' in dUnitsStr:
+          newDUnits = []
+          for i in self.dUnits:
+            if '^' in i:
+              i, repeat = i.split('^')
+              for n in range(int(repeat)-1):
+                newDUnits.append(i)
+            newDUnits.append(i)
+          self.dUnits = newDUnits
+    newNUnits = self.nUnits
+    newDUnits = self.dUnits
+    for i in self.nUnits:
+      if i in newDUnits:
+        newNUnits.remove(i)
+        newDUnits.remove(i)
+    #Sort units alphabetically
+    self.nUnits=sorted(newNUnits)
+    self.dUnits=sorted(newDUnits)
+    #Reformat units string
+    self.units = Measurement.formatUnits(self.nUnits, self.dUnits)
+
+  def fromStr(string):
+    """Creates a Measurement object from a string.
+    The string must be in the form of a number, uncertainty, and units.
+    The uncertainty can be in the form of a percentage or a number.
+    A 'a' or 'd' can be used to indicate an analog or digital device for automatic uncertainty determination.
+
+    :param string: The string to create the Measurement object from.
+    :type string: str
+    :return: The Measurement object created from the string.
+    :rtype: Measurement
+    """
+    sample = string.strip()
+    uncertainty = None
+    units = None
+    values = sample.split()
+    if '+/-' in sample or '+-' in sample:
+      if len(values) == 3:
+        if '+/-' in sample:
+          sample, uncertainty = string.split('+/-')
+        elif '+-' in sample:
+          sample, uncertainty = string.split('+-')
+      elif len(values) >= 4:
+        sample, _, uncertainty, *units = values
+        if len(units) == 2: # Assuming form will mol H2O
+          if '_' not in units[1]:
+            from pymeasurement.util.chem.compound import Compound
+            units[1] = str(Compound(units[1])) # Format Compound String
+        units = ' '.join(units)
+    else:
+      if len(values) >= 2:
+        sample, *units = values
+        if len(units) == 2: # Assuming form will mol H2O
+          if '_' not in units[1]:
+            from pymeasurement.util.chem.compound import Compound
+            units[1] = str(Compound(units[1])) # Format Compound String
+        units = ' '.join(units)
+    precision = None
+    digital = False
+    analog = False
+    if uncertainty is None:
+      if 'c' in sample:
+        precision = float('inf')
+        sample = sample.replace('c', '')
+      elif 'd' in sample:
+        digital = True
+        sample = sample.replace('d', '')
+      elif 'a' in sample:
+        analog = True
+        sample = sample.replace('a', '')
+    return Measurement(sample.strip(), precision=precision, uncertainty=(uncertainty.strip() if isinstance(uncertainty, str) else uncertainty), digital=digital, analog=analog, units=units)
+
+  def fromFloat(f, units=''): #Assume float is a constant with infinite precision and no uncertainty.
+    """
+    Creates a Measurement constant from a float.
+
+    :param f: The float to create the Measurement constant from.
+    :type f: float
+    :param units: The units of the Measurement constant.
+    :type units: str
+    :return: The Measurement constant created from the float.
+    :rtype: Measurement
+    """
+    return Measurement.fromStr(f'{f}c {units}')
+  
+  def toAbsolute(self):
+    """
+    Converts the uncertainty to an absolute value. Note that this mutates the object.
+
+    :return: The Measurement object with the uncertainty converted to an absolute value.
+    :rtype: Measurement
+    """
+    if self.uncertaintyPercent and isinstance(self.uncertainty, SigFig):
+      self.uncertaintyPercent = False
+      self.uncertainty *= (self.sample / SigFig('100', constant=True)).abs()
+      self.uncertainty = SigFig(str(self.uncertainty.decimalValue), decimals=self.sample.decimals)
+    return self
+
+  def toPercent(self):
+    """
+    Converts the uncertainty to a percentage. Note that this mutates the object.
+
+    :return: The Measurement object with the uncertainty converted to a percentage.
+    :rtype: Measurement
+    """
+    if not self.uncertaintyPercent and isinstance(self.uncertainty, SigFig):
+      self.uncertaintyPercent = True
+      self.uncertainty = SigFig(self.uncertainty.value, constant=True) * SigFig((SigFig('100', constant=True) / self.sample).abs().value, constant=True)
+      self.uncertainty = SigFig(str(self.uncertainty.decimalValue), sigfigs=(2 if self.uncertainty < SigFig('2', constant=True) else 1))
+    return self
+
+  def absolute(m):
+    """
+    Returns a copy of the Measurement with the uncertainty converted to an absolute value.
+
+    :return: A copy of the Measurement with the uncertainty converted to an absolute value.
+    :rtype: Measurement
+    """
+    return m.deepCopy().toAbsolute()
+
+  def percent(m):
+    """
+    Returns a copy of the Measurement with the uncertainty converted to a percentage.
+
+    :return: A copy of the Measurement with the uncertainty converted to a percentage.
+    :rtype: Measurement
+    """
+    return m.deepCopy().toPercent()
+  
+  def deepCopy(self):
+    """
+    Returns a deep copy of the Measurement object.
+
+    :return: A deep copy of the Measurement object.
+    :rtype: Measurement
+    """
+    return Measurement(self.sample.deepCopy(), uncertainty = self.uncertainty.deepCopy() if self.uncertainty is not None else None, uncertaintyPercent = self.uncertaintyPercent, units=self.units)
+  
+  def __str__(self):
+    """
+    Returns a string representation of the Measurement object.
+
+    :return: A string representation of the Measurement object.
+    :rtype: str
+    """
+    return str(self.sample) + (f' +/- {self.uncertainty}' + ('%' if self.uncertaintyPercent else '') if isinstance(self.uncertainty, SigFig) else '') + (f' {Measurement.formatUnits(self.nUnits, self.dUnits)}' if self.units is not None else '')
+
+  def __repr__(self):
+    """
+    Returns a string representation of the Measurement object.
+
+    :return: A string representation of the Measurement object.
+    :rtype: str
+    """
+    return str(self)
+
+  def multUnits(nUnits1, dUnits1, nUnits2, dUnits2):
+    """
+    Multiplies two sets of units.
+
+    :param nUnits1: The numerator units of the first set.
+    :type nUnits1: list
+    :param dUnits1: The denominator units of the first set.
+    :type dUnits1: list
+    :param nUnits2: The numerator units of the second set.
+    :type nUnits2: list
+    :param dUnits2: The denominator units of the second set.
+    :type dUnits2: list
+    :return: The multiplied units.
+    :rtype: tuple
+    """
+    nUnits = nUnits1 + nUnits2
+    dUnits = dUnits1 + dUnits2
+    newNUnits = nUnits
+    newDUnits = dUnits
+    for i in nUnits:
+      if i in newDUnits:
+        newNUnits.remove(i)
+        newDUnits.remove(i)
+    return (sorted(newNUnits), sorted(newDUnits))
+
+  def formatUnits(nUnits, dUnits):
+    """
+    Formats a set of units into a string.
+
+    :param nUnits: The numerator units.
+    :type nUnits: list
+    :param dUnits: The denominator units.
+    :type dUnits: list
+    :return: The formatted units.
+    :rtype: str
+    """
+    combinedNUnits = sorted([i if nUnits.count(i) == 1 else f'{i}^{nUnits.count(i)}' for i in set(nUnits)])
+    combinedDUnits = sorted([i if dUnits.count(i) == 1 else f'{i}^{dUnits.count(i)}' for i in set(dUnits)])
+    nUnitsStr = '1' if not nUnits else '*'.join(combinedNUnits)
+    dUnitsStr = '' if not dUnits else '*'.join(combinedDUnits)
+    if len(combinedNUnits) > 1:
+      nUnitsStr = '(' + nUnitsStr + ')'
+    if len(combinedDUnits) > 1:
+      dUnitsStr = '(' + dUnitsStr + ')'
+    return None if nUnitsStr == '1' and dUnitsStr == '' else nUnitsStr + (f'/{dUnitsStr}' if dUnitsStr else '')
+
+  def __eq__(self, other):
+    """
+    Returns True if the two Measurement objects are equal.
+
+    :param other: The Measurement object to compare.
+    :type other: Measurement
+    :returns: True if the two Measurement objects are equal.
+    :rtype: bool
+    """
+    return self.sample == other.sample
+
+  def __lt__(self, other):
+    """
+    Returns True if the first Measurement object is less than the second.
+
+    :param other: The Measurement object to compare.
+    :type other: Measurement
+    :returns: True if the first Measurement object is less than the second.
+    :rtype: bool
+    """
+    return self.sample < other.sample
+
+  def __gt__(self, other):
+    """
+    Returns True if the first Measurement object is greater than the second.
+
+    :param other: The Measurement object to compare.
+    :type other: Measurement
+    :returns: True if the first Measurement object is greater than the second.
+    :rtype: bool
+    """
+    return self.sample > other.sample
+
+  def __le__(self, other):
+    """
+    Returns True if the first Measurement object is less than or equal to the second.
+
+    :param other: The Measurement object to compare.
+    :type other: Measurement
+    :returns: True if the first Measurement object is less than or equal to the second.
+    :rtype: bool
+    """
+    return self < other or self == other
+
+  def __ge__(self, other):
+    """
+    Returns True if the first Measurement object is greater than or equal to the second.
+
+    :param other: The Measurement object to compare.
+    :type other: Measurement
+    :returns: True if the first Measurement object is greater than or equal to the second.
+    :rtype: bool
+    """
+    return self > other or self == other
+  
+  def __neg__(self):
+    """
+    Returns the negation of the Measurement object.
+
+    :returns: The negation of the Measurement object.
+    :rtype: Measurement
+    """
+    neg = self.deepCopy()
+    neg.sample = -self.sample
+    return neg
+
+  def __add__(self, other):
+    """
+    Returns the sum of the two Measurement objects.
+
+    :param other: The Measurement object to add.
+    :type other: Measurement
+    :returns: The sum of the two Measurement objects.
+    :rtype: Measurement
+    """
+    if self.nUnits != other.nUnits or self.dUnits != other.dUnits:
+      raise Exception(f'Measurement Error: Cannot add {self} and {other} with different units.')
+    uSum = SigFig('0', constant=True)
+    uncertainties = [Measurement.absolute(i).uncertainty for i in [self, other] if i.uncertainty is not None]
+    for u in uncertainties:
+      uSum += u
+    return Measurement(self.sample + other.sample, uncertainty=uSum if uncertainties else None, units=self.units)
+  
+  def __radd__(self, other):
+    """
+    Returns the sum of the two Measurement objects.
+
+    :param other: The Measurement object to add to.
+    :type other: Measurement
+    :returns: The sum of the two Measurement objects.
+    :rtype: Measurement
+    """
+    return self + other
+  
+  def __sub__(self, other):
+    """
+    Returns the difference of the two Measurement objects.
+
+    :param other: The Measurement object to subtract.
+    :type other: Measurement
+    :returns: The difference of the two Measurement objects.
+    :rtype: Measurement
+    """
+    return -other + self
+
+  def __rsub__(self, other):
+    """
+    Returns the difference of the two Measurement objects.
+
+    :param other: The Measurement object to subtract from.
+    :type other: Measurement
+    :returns: The difference of the two Measurement objects.
+    :rtype: Measurement
+    """
+    return -self + other
+
+  def __mul__(self, other):
+    """
+    Returns the product of the two Measurement objects.
+
+    :param other: The Measurement object to multiply by.
+    :type other: Measurement
+    :returns: The product of the two Measurement objects.
+    :rtype: Measurement
+    """
+    if isinstance(other, float) or isinstance(other, int):
+      other = Measurement.fromFloat(other)
+    uSum = SigFig('0', constant=True)
+    uncertainties = [Measurement.percent(i).uncertainty for i in [self, other] if i.uncertainty is not None]
+    for u in uncertainties:
+      uSum += u
+    nUnits, dUnits = Measurement.multUnits(self.nUnits, self.dUnits, other.nUnits, other.dUnits)
+    return Measurement(self.sample * other.sample, uncertainty=uSum if uncertainties else None, uncertaintyPercent=True, units=Measurement.formatUnits(nUnits, dUnits))
+  
+  def __rmul__(self, other):
+    """
+    Returns the product of the two Measurement objects.
+
+    :param other: The Measurement object to multiply by.
+    :type other: Measurement
+    :returns: The product of the two Measurement objects.
+    :rtype: Measurement
+    """
+    return self * other
+
+  def __truediv__(self, other):
+    """
+    Returns the quotient of the two Measurement objects.
+
+    :param other: The Measurement object to divide by.
+    :type other: Measurement
+    :returns: The quotient of the two Measurement objects.
+    :rtype: Measurement
+    """
+    if isinstance(other, float) or isinstance(other, int):
+      other = Measurement.fromFloat(other)
+    uSum = SigFig('0', constant=True)
+    uncertainties = [Measurement.percent(i).uncertainty for i in [self, other] if i.uncertainty is not None]
+    for u in uncertainties:
+      uSum += u
+    nUnits, dUnits = Measurement.multUnits(self.nUnits, self.dUnits, other.dUnits, other.nUnits)
+    return Measurement(self.sample / other.sample, uncertainty=uSum if uncertainties else None, uncertaintyPercent=True, units=Measurement.formatUnits(nUnits, dUnits))
+    
+  def __rtruediv__(self, other):
+    """
+    Returns the quotient of the two Measurement objects.
+
+    :param other: The Measurement object to divide by.
+    :type other: Measurement
+    :returns: The quotient of the two Measurement objects.
+    :rtype: Measurement
+    """
+    return other / self
+
+  def __pow__(self, integer):
+    """
+    Returns the Measurement object raised to the given integer power.
+
+    :param integer: The integer power to raise the Measurement object to.
+    :type integer: int
+    :returns: The Measurement object raised to the given integer power.
+    :rtype: Measurement
+    """
+    product = Measurement('1', precision=float('inf'))
+    for i in range(integer):
+      product *= self
+    return product
+
+  def sum(measurements):
+    """
+    Returns the sum of the given list of Measurement objects.
+
+    :param measurements: The list of Measurement objects.
+    :type measurements: list
+    :returns: The sum of the given list of Measurement objects.
+    :rtype: Measurement
+    """
+    if not measurements:
+      return Measurement.fromStr('0c')
+    s = measurements[0]
+    for i in measurements[1:]:
+      s += i
+    return s
+
+  def max(measurements):
+    """
+    Returns the maximum of the given list of Measurement objects.
+
+    :param measurements: The list of Measurement objects.
+    :type measurements: list
+    :returns: The maximum of the given list of Measurement objects.
+    :rtype: Measurement
+    """
+    m = measurements[0]
+    for i in measurements[1:]:
+      if m < i:
+        m = i
+    return m
+
+  def min(measurements):
+    """
+    Returns the minimum of the given list of Measurement objects.
+
+    :param measurements: The list of Measurement objects.
+    :type measurements: list
+    :returns: The minimum of the given list of Measurement objects.
+    :rtype: Measurement
+    """
+    m = measurements[0]
+    for i in measurements[1:]:
+      if m > i:
+        m = i
+    return m
+
+  def average(measurements):
+    """
+    Returns the average of the given list of Measurement objects. Uses (max - min) / (2 * sqrt(n)) as the uncertainty.
+
+    :param measurements: The list of Measurement objects.
+    :type measurements: list
+    :returns: The average of the given list of Measurement objects.
+    :rtype: Measurement
+    """
+    avg_sample = Measurement.sum(measurements) / len(measurements)
+    avg_uncertainty = (Measurement.max(measurements) - Measurement.min(measurements)).sample / (2 * math.sqrt(len(measurements)))
+    return Measurement(avg_sample.sample, uncertainty=avg_uncertainty.value, units=avg_sample.units)
+
+  def convert(sample, uncertainty=None, uncertaintyPercent=False, units='', analog=False, digital=False, constant=False, u=None, up=False, a=False, d=False, un='', decimals=None):
+    """
+    Returns a Measurement object with the given sample, uncertainty, and units.
+    
+    :param sample: The sample of the Measurement object.
+    :type sample: float or str
+    :param uncertainty: The uncertainty of the Measurement object.
+    :type uncertainty: float or str
+    :param uncertaintyPercent: Whether the uncertainty is a percent.
+    :type uncertaintyPercent: bool
+    :param units: The units of the Measurement object.
+    :type units: str
+    :param analog: Whether the Measurement object is analog.
+    :type analog: bool
+    :param digital: Whether the Measurement object is digital.
+    :type digital: bool
+    :param constant: Whether the Measurement object is constant.
+    :type constant: bool
+    :param u: The uncertainty of the Measurement object.
+    :type u: float or str
+    :param up: Whether the uncertainty is a percent.
+    :type up: bool
+    :param a: Whether the Measurement object is analog.
+    :type a: bool
+    :param d: Whether the Measurement object is digital.
+    :type d: bool
+    :param un: The units of the Measurement object.
+    :type un: str
+    :param decimals: The number of decimals to round to.
+    :type decimals: int
+    """
+    if u is not None:
+      uncertainty = u
+    if up:
+      uncertaintyPercent = up
+    if a:
+      analog = a
+    if d:
+      digital = d
+    if un:
+      units = un
+
+    return Measurement(SigFig(str(sample), decimals=-decimals if decimals is not None else None), uncertaintyPercent=uncertaintyPercent, uncertainty=str(uncertainty) if uncertainty is not None else None, precision=float('inf') if constant else None, units=units, analog=analog, digital=digital)
+  
+  def importColumn(column, uncertaintyColumn=None, df=None, **kwargs):
+    """
+    Convert a numeric Pandas DataFrame column to Measurement objects.
+    
+    :param column: The numeric Pandas DataFrame column.
+    :type column: pandas.core.series.Series
+    :param kwargs: Keyword arguments to pass to Measurement.convert.
+    :type kwargs: dict
+    """
+    if uncertaintyColumn is None:
+      return column.apply(Measurement.convert, **kwargs)
+    else:
+      return df.apply(lambda x: Measurement.convert(x[column.name], u=x[uncertaintyColumn.name], **kwargs), axis=1)
+
+  def exportColumn(savedf, column, addUncertainty=True, asPercent=True):
+    """
+    Convert a Measurement Pandas DataFrame column to numeric values.
+
+    :param savedf: The Pandas DataFrame to save to.
+    :type savedf: pandas.core.frame.DataFrame
+    :param column: The Measurement Pandas DataFrame column.
+    :type column: pandas.core.series.Series
+    :param addUncertainty: Whether to add the uncertainty to the DataFrame.
+    :type addUncertainty: bool
+    :param asPercent: Whether to add the uncertainty as a percent.
+    :type asPercent: bool
+    """
+    savedf[column.name] = column.apply(lambda x: x.sample)
+    if addUncertainty:
+      label, units = (' ('.join(column.name.split(' (')[:-1]), ' (' + column.name.split(' (')[-1]) if ' (' in column.name else (column.name, '')
+      if asPercent:
+        savedf.insert(savedf.columns.get_loc(column.name) + 1, f'{label} Percent Uncertainty (%)', column.apply(lambda x: x.percent().uncertainty))
+      else:
+        savedf.insert(savedf.columns.get_loc(column.name) + 1, f'{label} Absolute Uncertainty{units}', column.apply(lambda x: x.absolute().uncertainty))
```

### Comparing `pymeasurement-1.0.8/src/pymeasurement/sigfig.py` & `pymeasurement-1.0.9/src/pymeasurement/sigfig.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,268 +1,268 @@
-from decimal import Decimal, Context
-
-class SigFig:
-  """A class for representing numbers with significant figures. SigFig objects are immutable. Internally, all numbers are stored as Decimal objects (fixed point numbers) for extra accuracy and precision. The central paradigm of this class is that the decimal value is the true value of the number, and the sigfigs and decimals are the precision of the number. The sigfigs and decimals are used to determine the precision of the number when it is printed.
-
-  :param value: The value of the number as a string.
-  :type value: str
-  :param sigfigs: The number of significant figures to use when printing the number. If None, the number of significant figures will be automatically determined.
-  :type sigfigs: int or None
-  :param decimals: The number of decimal places to use when printing the number. If None, the number of decimal places will be automatically determined.
-  :type decimals: int or None
-  :param constant: If True, the number will be assumed to be perfectly accurate for all calculations. If False, the number will be assumed to have some precision that must be followed.
-  :type constant: bool
-  """
-  def __init__(self, value, sigfigs=None, decimals=None, constant=False):
-    """SigFig Constructor
-    """
-    self.value = value
-    try:
-      self.decimalValue = Decimal(value) #True Value of Decimal including extra calculation precision.
-    except:
-      raise Exception(f'Sig Fig Error: Could not convert "{self.value}" into sig fig.')
-    sign, digits, exponent = self.decimalValue.as_tuple()
-    self.sigfigs = len(digits)
-    self.decimal = Decimal((sign, digits, exponent)) #Sig Fig Decimal Representation
-    if constant:
-      #Constants are assumed to be perfectly accurate for all calculations.
-      self.sigfigs = float('inf')
-      self.decimals = float('-inf')
-    else:
-      #Value has some precision that must be followed.
-      #Automatic Override
-      if '.' in self.value: #Decimal Value
-        #Force override to maintain sig fig precision
-        self.decimal = SigFig.changeSigFigs(value, self.sigfigs)
-        self.decimals = exponent
-      else:
-        newSigfigs = len([int(i) for i in ''.join([str(i) for i in digits]).rstrip('0')])
-        if newSigfigs != self.sigfigs and newSigfigs > 0:
-          self.decimal = SigFig.changeSigFigs(value, newSigfigs)
-          self.sigfigs = newSigfigs
-        self.decimals = len(digits) - self.sigfigs
-  
-      #Manual override for sigfig or decimal precision.
-      if sigfigs != None and sigfigs != float("inf"):
-        self.sigfigs = sigfigs
-        self.decimal = SigFig.changeSigFigs(value, sigfigs)
-        sign, digits, exponent = self.decimal.as_tuple()
-        if exponent < 0: #Decimal Value
-          self.decimals = exponent
-        else:
-          self.decimals = len(digits) - self.sigfigs
-      elif decimals != None:
-        self.decimals = decimals
-        self.decimal = self.decimal.quantize(Decimal(f"1E{self.decimals}"))
-        sign, digits, exponent = self.decimal.as_tuple()
-        self.sigfigs = len(digits) - self.decimals + exponent
-
-  def changeSigFigs(value, sigfigs):
-    """Changes the number of significant figures of a number.
-
-    :param value: The value of the number as a string.
-    :type value: str
-    :param sigfigs: The number of significant figures to use.
-    :type sigfigs: int
-    :return: The number with the new number of significant figures.
-    :rtype: Decimal
-    """
-    sign, digits, exponent = Context(prec=sigfigs).create_decimal(value).as_tuple()
-    if len(digits) < sigfigs:
-      missing = sigfigs - len(digits)
-      digits = digits + (0,) * missing
-      exponent -= missing
-    return Decimal((sign, digits, exponent))
-
-  def deepCopy(self):
-    """Returns a deep copy of the SigFig object.
-    
-    :return: A deep copy of the SigFig object.
-    :rtype: SigFig
-    """
-    new = SigFig('0')
-    new.value = self.value
-    new.decimalValue = self.decimalValue
-    new.decimal = self.decimal
-    new.sigfigs = self.sigfigs
-    new.decimals = self.decimals
-    return new
-  
-  def __str__(self):
-    """Returns the string representation of the SigFig object.
-
-    :return: The string representation of the SigFig object.
-    :rtype: str
-    """
-    return str(self.decimal)
-
-  def __repr__(self):
-    """Returns the string representation of the SigFig object.
-
-    :return: The string representation of the SigFig object.
-    :rtype: str
-    """
-    return str(self)
-
-  def __eq__(self, other):
-    """Checks if the two SigFig objects are equal.
-
-    :param other: The other SigFig object to compare to this one.
-    :type other: SigFig
-    :return: True if the two SigFig objects are equal.
-    :rtype: bool
-    """
-    return self.decimal == other.decimal
-
-  def __lt__(self, other):
-    """Checks if the SigFig object is less than the other SigFig object.
-
-    :param other: The other SigFig object to compare to this one.
-    :type other: SigFig
-    :return: True if the SigFig object is less than the other SigFig object.
-    :rtype: bool
-    """
-    return self.decimal < other.decimal
-
-  def __gt__(self, other):
-    """Checks if the SigFig object is greater than the other SigFig object.
-
-    :param other: The other SigFig object to compare to this one.
-    :type other: SigFig
-    :return: True if the SigFig object is greater than the other SigFig object.
-    :rtype: bool
-    """
-    return self.decimal > other.decimal
-
-  def __le__(self, other):
-    """Checks if the SigFig object is less than or equal to the other SigFig object.
-
-    :param other: The other SigFig object to compare to this one.
-    :type other: SigFig
-    :return: True if the SigFig object is less than or equal to the other SigFig object.
-    :rtype: bool
-    """
-    return self < other or self == other
-
-  def __ge__(self, other):
-    """Checks if the SigFig object is greater than or equal to the other SigFig object.
-
-    :param other: The other SigFig object to compare to this one.
-    :type other: SigFig
-    :return: True if the SigFig object is greater than or equal to the other SigFig object.
-    :rtype: bool
-    """
-    return self > other or self == other
-  
-  def __neg__(self):
-    """Returns the negative of the SigFig object.
-
-    :return: The negative of the SigFig object.
-    :rtype: SigFig
-    """
-    neg = self.deepCopy()
-    neg.value = self.value.replace('-', '') if '-' in self.value else f'-{self.value}'
-    neg.decimal = -self.decimal
-    neg.decimalValue = -self.decimalValue
-    return neg
-
-  def __add__(self, other):
-    """Returns the sum of the two SigFig objects as a new SigFig object, following the rules of significant figures.
-
-    :param other: The other SigFig object to add to this one.
-    :type other: SigFig
-    :return: The sum of the two SigFig objects as a new SigFig object.
-    :rtype: SigFig
-    """
-    if isinstance(other, float) or isinstance(other, int):
-      other = SigFig(str(other), constant=True)
-    decimals = max(self.decimals, other.decimals)
-    return SigFig(str(self.decimalValue + other.decimalValue), decimals=decimals, constant=decimals == float('-inf'))
-  
-  def __radd__(self, other):
-    """Returns the sum of the two SigFig objects as a new SigFig object, following the rules of significant figures.
-
-    :param other: The other SigFig object to add to this one.
-    :type other: SigFig
-    :return: The sum of the two SigFig objects as a new SigFig object.
-    :rtype: SigFig
-    """
-    return self + other
-  
-  def __sub__(self, other):
-    """Returns the difference of the two SigFig objects as a new SigFig object, following the rules of significant figures.
-
-    :param other: The other SigFig object to subtract from this one.
-    :type other: SigFig
-    :return: The difference of the two SigFig objects as a new SigFig object.
-    :rtype: SigFig
-    """
-    if isinstance(other, float) or isinstance(other, int):
-      other = SigFig(str(other), constant=True)
-    return -other + self
-
-  def __rsub__(self, other):
-    """Returns the difference of the two SigFig objects as a new SigFig object, following the rules of significant figures.
-
-    :param other: The other SigFig object to subtract from this one.
-    :type other: SigFig
-    :return: The difference of the two SigFig objects as a new SigFig object.
-    :rtype: SigFig
-    """
-    return -self + other
-
-  def __mul__(self, other):
-    """Returns the product of the two SigFig objects as a new SigFig object, following the rules of significant figures.
-
-    :param other: The other SigFig object to multiply by this one.
-    :type other: SigFig
-    :return: The product of the two SigFig objects as a new SigFig object.
-    :rtype: SigFig
-    """
-    if isinstance(other, float) or isinstance(other, int):
-      other = SigFig(str(other), constant=True)
-    sigfigs = min(self.sigfigs, other.sigfigs)
-    return SigFig(str(self.decimalValue * other.decimalValue), sigfigs=sigfigs, constant=sigfigs == float('inf'))
-
-  def __rmul__(self, other):
-    """Returns the product of the two SigFig objects as a new SigFig object, following the rules of significant figures.
-
-    :param other: The other SigFig object to multiply by this one.
-    :type other: SigFig
-    :return: The product of the two SigFig objects as a new SigFig object.
-    :rtype: SigFig
-    """
-    return self * other
-
-  def __truediv__(self, other):
-    """Returns the quotient of the two SigFig objects as a new SigFig object, following the rules of significant figures.
-
-    :param other: The other SigFig object to divide by this one.
-    :type other: SigFig
-    :return: This SigFig object divided by the other SigFig object.
-    :rtype: SigFig
-    """
-    if isinstance(other, float) or isinstance(other, int):
-      other = SigFig(str(other), constant=True)
-    sigfigs = min(self.sigfigs, other.sigfigs)
-    return SigFig(str(self.decimalValue / other.decimalValue), sigfigs=sigfigs, constant=sigfigs == float('inf'))
-
-  def __rtruediv__(self, other):
-    """Returns the quotient of the two SigFig objects as a new SigFig object, following the rules of significant figures.
-
-    :param other: The other SigFig object to divide by this one.
-    :type other: SigFig
-    :return: Other SigFig object divided by this one.
-    :rtype: SigFig
-    """
-    return other / self
-
-  def abs(self):
-    """Returns the absolute value of the SigFig object.
-
-    :return: The absolute value of the SigFig object.
-    :rtype: SigFig
-    """
-    if self >= SigFig('0', constant=True):
-      return self
-    else:
+from decimal import Decimal, Context
+
+class SigFig:
+  """A class for representing numbers with significant figures. SigFig objects are immutable. Internally, all numbers are stored as Decimal objects (fixed point numbers) for extra accuracy and precision. The central paradigm of this class is that the decimal value is the true value of the number, and the sigfigs and decimals are the precision of the number. The sigfigs and decimals are used to determine the precision of the number when it is printed.
+
+  :param value: The value of the number as a string.
+  :type value: str
+  :param sigfigs: The number of significant figures to use when printing the number. If None, the number of significant figures will be automatically determined.
+  :type sigfigs: int or None
+  :param decimals: The number of decimal places to use when printing the number. If None, the number of decimal places will be automatically determined.
+  :type decimals: int or None
+  :param constant: If True, the number will be assumed to be perfectly accurate for all calculations. If False, the number will be assumed to have some precision that must be followed.
+  :type constant: bool
+  """
+  def __init__(self, value, sigfigs=None, decimals=None, constant=False):
+    """SigFig Constructor
+    """
+    self.value = value
+    try:
+      self.decimalValue = Decimal(value) #True Value of Decimal including extra calculation precision.
+    except:
+      raise Exception(f'Sig Fig Error: Could not convert "{self.value}" into sig fig.')
+    sign, digits, exponent = self.decimalValue.as_tuple()
+    self.sigfigs = len(digits)
+    self.decimal = Decimal((sign, digits, exponent)) #Sig Fig Decimal Representation
+    if constant:
+      #Constants are assumed to be perfectly accurate for all calculations.
+      self.sigfigs = float('inf')
+      self.decimals = float('-inf')
+    else:
+      #Value has some precision that must be followed.
+      #Automatic Override
+      if '.' in self.value: #Decimal Value
+        #Force override to maintain sig fig precision
+        self.decimal = SigFig.changeSigFigs(value, self.sigfigs)
+        self.decimals = exponent
+      else:
+        newSigfigs = len([int(i) for i in ''.join([str(i) for i in digits]).rstrip('0')])
+        if newSigfigs != self.sigfigs and newSigfigs > 0:
+          self.decimal = SigFig.changeSigFigs(value, newSigfigs)
+          self.sigfigs = newSigfigs
+        self.decimals = len(digits) - self.sigfigs
+  
+      #Manual override for sigfig or decimal precision.
+      if sigfigs != None and sigfigs != float("inf"):
+        self.sigfigs = sigfigs
+        self.decimal = SigFig.changeSigFigs(value, sigfigs)
+        sign, digits, exponent = self.decimal.as_tuple()
+        if exponent < 0: #Decimal Value
+          self.decimals = exponent
+        else:
+          self.decimals = len(digits) - self.sigfigs
+      elif decimals != None:
+        self.decimals = decimals
+        self.decimal = self.decimal.quantize(Decimal(f"1E{self.decimals}"))
+        sign, digits, exponent = self.decimal.as_tuple()
+        self.sigfigs = len(digits) - self.decimals + exponent
+
+  def changeSigFigs(value, sigfigs):
+    """Changes the number of significant figures of a number.
+
+    :param value: The value of the number as a string.
+    :type value: str
+    :param sigfigs: The number of significant figures to use.
+    :type sigfigs: int
+    :return: The number with the new number of significant figures.
+    :rtype: Decimal
+    """
+    sign, digits, exponent = Context(prec=sigfigs).create_decimal(value).as_tuple()
+    if len(digits) < sigfigs:
+      missing = sigfigs - len(digits)
+      digits = digits + (0,) * missing
+      exponent -= missing
+    return Decimal((sign, digits, exponent))
+
+  def deepCopy(self):
+    """Returns a deep copy of the SigFig object.
+    
+    :return: A deep copy of the SigFig object.
+    :rtype: SigFig
+    """
+    new = SigFig('0')
+    new.value = self.value
+    new.decimalValue = self.decimalValue
+    new.decimal = self.decimal
+    new.sigfigs = self.sigfigs
+    new.decimals = self.decimals
+    return new
+  
+  def __str__(self):
+    """Returns the string representation of the SigFig object.
+
+    :return: The string representation of the SigFig object.
+    :rtype: str
+    """
+    return str(self.decimal)
+
+  def __repr__(self):
+    """Returns the string representation of the SigFig object.
+
+    :return: The string representation of the SigFig object.
+    :rtype: str
+    """
+    return str(self)
+
+  def __eq__(self, other):
+    """Checks if the two SigFig objects are equal.
+
+    :param other: The other SigFig object to compare to this one.
+    :type other: SigFig
+    :return: True if the two SigFig objects are equal.
+    :rtype: bool
+    """
+    return self.decimal == other.decimal
+
+  def __lt__(self, other):
+    """Checks if the SigFig object is less than the other SigFig object.
+
+    :param other: The other SigFig object to compare to this one.
+    :type other: SigFig
+    :return: True if the SigFig object is less than the other SigFig object.
+    :rtype: bool
+    """
+    return self.decimal < other.decimal
+
+  def __gt__(self, other):
+    """Checks if the SigFig object is greater than the other SigFig object.
+
+    :param other: The other SigFig object to compare to this one.
+    :type other: SigFig
+    :return: True if the SigFig object is greater than the other SigFig object.
+    :rtype: bool
+    """
+    return self.decimal > other.decimal
+
+  def __le__(self, other):
+    """Checks if the SigFig object is less than or equal to the other SigFig object.
+
+    :param other: The other SigFig object to compare to this one.
+    :type other: SigFig
+    :return: True if the SigFig object is less than or equal to the other SigFig object.
+    :rtype: bool
+    """
+    return self < other or self == other
+
+  def __ge__(self, other):
+    """Checks if the SigFig object is greater than or equal to the other SigFig object.
+
+    :param other: The other SigFig object to compare to this one.
+    :type other: SigFig
+    :return: True if the SigFig object is greater than or equal to the other SigFig object.
+    :rtype: bool
+    """
+    return self > other or self == other
+  
+  def __neg__(self):
+    """Returns the negative of the SigFig object.
+
+    :return: The negative of the SigFig object.
+    :rtype: SigFig
+    """
+    neg = self.deepCopy()
+    neg.value = self.value.replace('-', '') if '-' in self.value else f'-{self.value}'
+    neg.decimal = -self.decimal
+    neg.decimalValue = -self.decimalValue
+    return neg
+
+  def __add__(self, other):
+    """Returns the sum of the two SigFig objects as a new SigFig object, following the rules of significant figures.
+
+    :param other: The other SigFig object to add to this one.
+    :type other: SigFig
+    :return: The sum of the two SigFig objects as a new SigFig object.
+    :rtype: SigFig
+    """
+    if isinstance(other, float) or isinstance(other, int):
+      other = SigFig(str(other), constant=True)
+    decimals = max(self.decimals, other.decimals)
+    return SigFig(str(self.decimalValue + other.decimalValue), decimals=decimals, constant=decimals == float('-inf'))
+  
+  def __radd__(self, other):
+    """Returns the sum of the two SigFig objects as a new SigFig object, following the rules of significant figures.
+
+    :param other: The other SigFig object to add to this one.
+    :type other: SigFig
+    :return: The sum of the two SigFig objects as a new SigFig object.
+    :rtype: SigFig
+    """
+    return self + other
+  
+  def __sub__(self, other):
+    """Returns the difference of the two SigFig objects as a new SigFig object, following the rules of significant figures.
+
+    :param other: The other SigFig object to subtract from this one.
+    :type other: SigFig
+    :return: The difference of the two SigFig objects as a new SigFig object.
+    :rtype: SigFig
+    """
+    if isinstance(other, float) or isinstance(other, int):
+      other = SigFig(str(other), constant=True)
+    return -other + self
+
+  def __rsub__(self, other):
+    """Returns the difference of the two SigFig objects as a new SigFig object, following the rules of significant figures.
+
+    :param other: The other SigFig object to subtract from this one.
+    :type other: SigFig
+    :return: The difference of the two SigFig objects as a new SigFig object.
+    :rtype: SigFig
+    """
+    return -self + other
+
+  def __mul__(self, other):
+    """Returns the product of the two SigFig objects as a new SigFig object, following the rules of significant figures.
+
+    :param other: The other SigFig object to multiply by this one.
+    :type other: SigFig
+    :return: The product of the two SigFig objects as a new SigFig object.
+    :rtype: SigFig
+    """
+    if isinstance(other, float) or isinstance(other, int):
+      other = SigFig(str(other), constant=True)
+    sigfigs = min(self.sigfigs, other.sigfigs)
+    return SigFig(str(self.decimalValue * other.decimalValue), sigfigs=sigfigs, constant=sigfigs == float('inf'))
+
+  def __rmul__(self, other):
+    """Returns the product of the two SigFig objects as a new SigFig object, following the rules of significant figures.
+
+    :param other: The other SigFig object to multiply by this one.
+    :type other: SigFig
+    :return: The product of the two SigFig objects as a new SigFig object.
+    :rtype: SigFig
+    """
+    return self * other
+
+  def __truediv__(self, other):
+    """Returns the quotient of the two SigFig objects as a new SigFig object, following the rules of significant figures.
+
+    :param other: The other SigFig object to divide by this one.
+    :type other: SigFig
+    :return: This SigFig object divided by the other SigFig object.
+    :rtype: SigFig
+    """
+    if isinstance(other, float) or isinstance(other, int):
+      other = SigFig(str(other), constant=True)
+    sigfigs = min(self.sigfigs, other.sigfigs)
+    return SigFig(str(self.decimalValue / other.decimalValue), sigfigs=sigfigs, constant=sigfigs == float('inf'))
+
+  def __rtruediv__(self, other):
+    """Returns the quotient of the two SigFig objects as a new SigFig object, following the rules of significant figures.
+
+    :param other: The other SigFig object to divide by this one.
+    :type other: SigFig
+    :return: Other SigFig object divided by this one.
+    :rtype: SigFig
+    """
+    return other / self
+
+  def abs(self):
+    """Returns the absolute value of the SigFig object.
+
+    :return: The absolute value of the SigFig object.
+    :rtype: SigFig
+    """
+    if self >= SigFig('0', constant=True):
+      return self
+    else:
       return -self
```

### Comparing `pymeasurement-1.0.8/src/pymeasurement/util/chem/compound.py` & `pymeasurement-1.0.9/src/pymeasurement/util/chem/compound.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,188 +1,188 @@
-from pymeasurement.util.parser import Parser
-from pymeasurement.util.chem.element import Element
-from pymeasurement.measurement import Measurement
-import re
-
-class Compound(Parser):
-  """A class to represent a chemical compound.
-
-  :param string: The string to parse.
-  :type string: str
-  """
-
-  latexPrint = False # Whether to print the compound in latex format.
-
-  def setLatexPrint(value):
-    """Set whether to print the compound in latex format.
-
-    :param value: Whether to print the compound in latex format.
-    :type value: bool
-    """
-    Element.setLatexPrint(value)
-    Compound.latexPrint = value
-  
-  def __init__(self, string):
-    """Compound Constructor
-    """
-    super().__init__(string)
-    self.composition = {}
-    self.element = ""
-    self.number = ""
-    self.parenthesesOn = False
-    self.parentheses = ')'
-    self.subString = ""
-    self.compoundString = self.string
-    self.stateString = ""
-    self.splitString(self.string, checks = self.split)
-    for i in range(len(self.compoundString)):
-      if not self.compoundString[i].isdigit():
-        self.compoundString = self.compoundString[i:].strip()
-        break
-    self.readByCharacter(self.compoundString, checks = self.checks, endSetup = self.save)
-    self.mass = Measurement.sum([e.mass * Measurement.fromFloat(self.composition[e]) for e in self.composition])
-
-  def split(self, string):
-    """Split the string into a compound string and a state string.
-
-    :param string: The string to split.
-    :type string: str
-    """
-    if '(s)' in string or '(l)' in string or '(g)' in string or '(aq)' in string:
-      if '(s)' in string:
-        self.stateString = '(s)'
-      elif '(l)' in string:
-        self.stateString = '(l)'
-      elif '(g)' in string:
-        self.stateString = '(g)'
-      else:
-        self.stateString = '(aq)'
-      self.compoundString = self.string.replace(self.stateString, '').strip()
-  
-  def checks(self, i, char):
-    """Check the character.
-
-    :param i: The index of the character.
-    :type i: int
-    :param char: The character to check.
-    :type char: str
-    """
-    if char.isalpha():
-      if self.parenthesesOn:
-          self.subString += char
-      else:
-        if char.isupper():
-          self.save()
-          self.element += char
-        else:
-          self.element += char
-    elif char.isdigit():
-      if self.parenthesesOn:
-        self.subString += char
-      else:
-        self.number += char
-    else:
-      if char == '(' or char == '[':
-        if not self.parenthesesOn:
-          self.save()
-          self.parenthesesOn = True
-          self.parentheses = ')' if char == '(' else ']'
-        else:
-          self.subString += char
-      elif char == ')' or char == ']':
-        if char == self.parentheses:
-          self.parenthesesOn = False
-        else:
-          self.subString += char
-      else:
-        raise Exception(f"Compound Parser Exception: Unknown character '{char}'")
-
-  def saveElement(self, element, number, multiple = 1):
-    """Save the element to the composition.
-
-    :param element: The element to save.
-    :type element: str
-    :param number: The number of the element.
-    :type number: str
-    :param multiple: The multiple of the element.
-    :type multiple: int
-    """
-    if Element(element) not in self.composition:
-      self.composition[Element(element)] = (int(number) if number else 1) * multiple
-    else:
-      self.composition[Element(element)] += (int(number) if number else 1) * multiple
-
-  def saveSubcompound(self):
-    """Save subcompound to the composition.
-    """
-    subCompound = Compound(self.subString)
-    for element in subCompound.composition:
-      self.saveElement(element.string, self.number, multiple = subCompound.composition[element])
-
-  def save(self):
-    """Save the element or subcompound to the composition.
-    """
-    if self.element or self.subString:
-      if self.element:
-        self.saveElement(self.element, self.number)
-      if self.subString:
-        self.saveSubcompound()
-    self.element = ""
-    self.number = ""
-    self.subString = ""
-
-  def __str__(self, textOverride = False):
-    """Get the string representation of the compound.
-
-    :param textOverride: Whether to override the latex print setting.
-    :type textOverride: bool
-    :return: The string representation of the compound.
-    :rtype: str
-    """
-    if Compound.latexPrint and not textOverride:
-      allCoefficients = re.findall("\d+", self.compoundString)
-      finalString = ''
-      currentIndex = 0
-      for i in allCoefficients:
-        ind = self.compoundString[currentIndex:].index(i)
-        finalString += self.compoundString[currentIndex:currentIndex + ind]+f'_{{{i}}}'
-        currentIndex = currentIndex + ind + len(i)
-      if currentIndex < len(self.compoundString):
-        finalString += self.compoundString[currentIndex:]
-      return finalString + (self.stateString if self.stateString else '')
-    return self.compoundString + (self.stateString if self.stateString else '')
-
-  def __eq__(self, other):
-    """Check if the compound is equal to another compound.
-    
-    :param other: The other compound to check.
-    :type other: Compound
-    :return: Whether the compounds are equal.
-    :rtype: bool
-    """
-    return self.composition == other.composition
-
-  def __ne__(self, other):
-    """Check if the compound is not equal to another compound.
-    
-    :param other: The other compound to check.
-    :type other: Compound
-    :return: Whether the compounds are not equal.
-    :rtype: bool
-    """
-    return self.composition != other.composition
-  
-  def massPercentComposition(self):
-    """Get the mass percent composition of the compound.
-
-    :return: The mass percent composition of the compound.
-    :rtype: list
-    """
-    return [['Element', 'Mass']]+[[str(i), self.composition[i]*i.mass] for i in self.composition]
-
-  def molePercentComposition(self):
-    """Get the mole percent composition of the compound.
-
-    :return: The mole percent composition of the compound.
-    :rtype: list
-    """
+from pymeasurement.util.parser import Parser
+from pymeasurement.util.chem.element import Element
+from pymeasurement.measurement import Measurement
+import re
+
+class Compound(Parser):
+  """A class to represent a chemical compound.
+
+  :param string: The string to parse.
+  :type string: str
+  """
+
+  latexPrint = False # Whether to print the compound in latex format.
+
+  def setLatexPrint(value):
+    """Set whether to print the compound in latex format.
+
+    :param value: Whether to print the compound in latex format.
+    :type value: bool
+    """
+    Element.setLatexPrint(value)
+    Compound.latexPrint = value
+  
+  def __init__(self, string):
+    """Compound Constructor
+    """
+    super().__init__(string)
+    self.composition = {}
+    self.element = ""
+    self.number = ""
+    self.parenthesesOn = False
+    self.parentheses = ')'
+    self.subString = ""
+    self.compoundString = self.string
+    self.stateString = ""
+    self.splitString(self.string, checks = self.split)
+    for i in range(len(self.compoundString)):
+      if not self.compoundString[i].isdigit():
+        self.compoundString = self.compoundString[i:].strip()
+        break
+    self.readByCharacter(self.compoundString, checks = self.checks, endSetup = self.save)
+    self.mass = Measurement.sum([e.mass * Measurement.fromFloat(self.composition[e]) for e in self.composition])
+
+  def split(self, string):
+    """Split the string into a compound string and a state string.
+
+    :param string: The string to split.
+    :type string: str
+    """
+    if '(s)' in string or '(l)' in string or '(g)' in string or '(aq)' in string:
+      if '(s)' in string:
+        self.stateString = '(s)'
+      elif '(l)' in string:
+        self.stateString = '(l)'
+      elif '(g)' in string:
+        self.stateString = '(g)'
+      else:
+        self.stateString = '(aq)'
+      self.compoundString = self.string.replace(self.stateString, '').strip()
+  
+  def checks(self, i, char):
+    """Check the character.
+
+    :param i: The index of the character.
+    :type i: int
+    :param char: The character to check.
+    :type char: str
+    """
+    if char.isalpha():
+      if self.parenthesesOn:
+          self.subString += char
+      else:
+        if char.isupper():
+          self.save()
+          self.element += char
+        else:
+          self.element += char
+    elif char.isdigit():
+      if self.parenthesesOn:
+        self.subString += char
+      else:
+        self.number += char
+    else:
+      if char == '(' or char == '[':
+        if not self.parenthesesOn:
+          self.save()
+          self.parenthesesOn = True
+          self.parentheses = ')' if char == '(' else ']'
+        else:
+          self.subString += char
+      elif char == ')' or char == ']':
+        if char == self.parentheses:
+          self.parenthesesOn = False
+        else:
+          self.subString += char
+      else:
+        raise Exception(f"Compound Parser Exception: Unknown character '{char}'")
+
+  def saveElement(self, element, number, multiple = 1):
+    """Save the element to the composition.
+
+    :param element: The element to save.
+    :type element: str
+    :param number: The number of the element.
+    :type number: str
+    :param multiple: The multiple of the element.
+    :type multiple: int
+    """
+    if Element(element) not in self.composition:
+      self.composition[Element(element)] = (int(number) if number else 1) * multiple
+    else:
+      self.composition[Element(element)] += (int(number) if number else 1) * multiple
+
+  def saveSubcompound(self):
+    """Save subcompound to the composition.
+    """
+    subCompound = Compound(self.subString)
+    for element in subCompound.composition:
+      self.saveElement(element.string, self.number, multiple = subCompound.composition[element])
+
+  def save(self):
+    """Save the element or subcompound to the composition.
+    """
+    if self.element or self.subString:
+      if self.element:
+        self.saveElement(self.element, self.number)
+      if self.subString:
+        self.saveSubcompound()
+    self.element = ""
+    self.number = ""
+    self.subString = ""
+
+  def __str__(self, textOverride = False):
+    """Get the string representation of the compound.
+
+    :param textOverride: Whether to override the latex print setting.
+    :type textOverride: bool
+    :return: The string representation of the compound.
+    :rtype: str
+    """
+    if Compound.latexPrint and not textOverride:
+      allCoefficients = re.findall("\d+", self.compoundString)
+      finalString = ''
+      currentIndex = 0
+      for i in allCoefficients:
+        ind = self.compoundString[currentIndex:].index(i)
+        finalString += self.compoundString[currentIndex:currentIndex + ind]+f'_{{{i}}}'
+        currentIndex = currentIndex + ind + len(i)
+      if currentIndex < len(self.compoundString):
+        finalString += self.compoundString[currentIndex:]
+      return finalString + (self.stateString if self.stateString else '')
+    return self.compoundString + (self.stateString if self.stateString else '')
+
+  def __eq__(self, other):
+    """Check if the compound is equal to another compound.
+    
+    :param other: The other compound to check.
+    :type other: Compound
+    :return: Whether the compounds are equal.
+    :rtype: bool
+    """
+    return self.composition == other.composition
+
+  def __ne__(self, other):
+    """Check if the compound is not equal to another compound.
+    
+    :param other: The other compound to check.
+    :type other: Compound
+    :return: Whether the compounds are not equal.
+    :rtype: bool
+    """
+    return self.composition != other.composition
+  
+  def massPercentComposition(self):
+    """Get the mass percent composition of the compound.
+
+    :return: The mass percent composition of the compound.
+    :rtype: list
+    """
+    return [['Element', 'Mass']]+[[str(i), self.composition[i]*i.mass] for i in self.composition]
+
+  def molePercentComposition(self):
+    """Get the mole percent composition of the compound.
+
+    :return: The mole percent composition of the compound.
+    :rtype: list
+    """
     return [['Element', 'Moles']]+[[str(i), self.composition[i]] for i in self.composition]
```

### Comparing `pymeasurement-1.0.8/src/pymeasurement/util/chem/element.py` & `pymeasurement-1.0.9/src/pymeasurement/util/chem/element.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-from pymeasurement.util.typecheck import typecheck
-from pymeasurement.measurement import Measurement
-
-class Element:
-  """A class to represent an chemical element.
-
-  :param string: The name of the element.
-    :type string: str
-    :param protons: The number of protons in the element.
-    :type protons: int or None
-    :param neutrons: The number of neutrons in the element.
-    :type neutrons: int or None
-    :param mass: The mass of the element.
-    :type mass: int or None
-  """
-  latexPrint = False # Whether to print the element in latex format.
-
-  def setLatexPrint(value):
-    """Set whether to print the element in latex format.
-
-    :param value: Whether to print the element in latex format.
-    :type value: bool
-    """
-    Element.latexPrint = value
-  
-  def __init__(self, string, protons = None, neutrons = None, mass = None):
-    """Element Constructor
-    """
-    typecheck(string, str)
-    typecheck(protons, int, None)
-    typecheck(neutrons, int, None)
-    typecheck(mass, int, None)
-    if not (len(string) > 0 and len(string) <= 2 and string.isalpha()):
-      raise Exception("Element Exception: Element Name must be 1 or 2 letters long.")
-    self.string = string
-    #Protons will only override if element does not exist.
-    self.protons = Element.elements().index(self.string) + 1 if self.string in Element.elements() else None
-    if self.protons == None:
-      self.protons = protons
-    self.neutrons = neutrons
-    self.mass = mass
-    total = (1 if self.protons != None else 0) + (1 if self.neutrons != None else 0) + (1 if self.mass != None else 0)
-    if total == 2:
-      if self.protons == None:
-        self.protons = self.mass - self.neutrons
-      elif self.neutrons == None:
-        self.neutrons = self.mass - self.protons
-      else:
-        self.mass = self.protons + self.neutrons
-
-    if self.mass == None:
-      self.mass = Measurement.fromStr(f'{Element.atomicWeights()[self.protons]}c') if self.protons in Element.atomicWeights() else None
-
-  def fromAtomicNumber(num):
-    """Create an element from an atomic number.
-
-    :param num: The atomic number of the element.
-    :type num: int
-    :returns: The element with the given atomic number.
-    """
-    if num < 1 or num > 118:
-      raise Exception("Element Exception: Atomic Number must be from 1-118.")
-    return Element(Element.elements[num-1])
-
-  def elements():
-    """Get a list of all elements.
-
-    :returns: A list of all elements.
-    :rtype: list
-    """
-    return ['H', 'He', 'Li', 'Be', 'B', 'C', 'N', 'O', 'F', 'Ne', 'Na', 'Mg', 'Al', 'Si', 'P', 'S', 'Cl', 'Ar', 'K', 'Ca', 'Sc', 'Ti', 'V', 'Cr', 'Mn', 'Fe', 'Co', 'Ni', 'Cu', 'Zn', 'Ga', 'Ge', 'As', 'Se', 'Br', 'Kr', 'Rb', 'Sr', 'Y', 'Zr', 'Nb', 'Mo', 'Tc', 'Ru', 'Rh', 'Pd', 'Ag', 'Cd', 'In', 'Sn', 'Sb', 'Te', 'I', 'Xe', 'Cs', 'Ba', 'La', 'Ce', 'Pr', 'Nd', 'Pm', 'Sm', 'Eu', 'Gd', 'Tb', 'Dy', 'Ho', 'Er', 'Tm', 'Yb', 'Lu', 'Hf', 'Ta', 'W', 'Re', 'Os', 'Ir', 'Pt', 'Au', 'Hg', 'Tl', 'Pb', 'Bi', 'Po', 'At', 'Rn', 'Fr', 'Ra', 'Ac', 'Th', 'Pa', 'U', 'Np', 'Pu', 'Am', 'Cm', 'Bk', 'Cf', 'Es', 'Fm', 'Md', 'No', 'Lr', 'Rf', 'Db', 'Sg', 'Bh', 'Hs', 'Mt', 'Ds', 'Rg', 'Cn', 'Nh', 'Fl', 'Mc', 'Lv', 'Ts', 'Og']
-
-  def atomicWeights():
-    """Get a dictionary of all atomic weights.
-
-    :returns: A dictionary of all atomic weights.
-    :rtype: dict
-    """
-    return {1: '1.01', 2: '4.00', 3: '6.94', 4: '9.01', 5: '10.81', 6: '12.01', 7: '14.01', 8: '16.00', 9: '19.00', 10: '20.18', 11: '22.99', 12: '24.31', 13: '26.98', 14: '28.09', 15: '30.97', 16: '32.07', 17: '35.45', 18: '39.95', 19: '39.1', 20: '40.08', 21: '44.96', 22: '47.87', 23: '50.94', 24: '52.00', 25: '54.94', 26: '55.85', 27: '58.93', 28: '58.69', 29: '63.55', 30: '65.41', 31: '69.72', 32: '72.64', 33: '74.92', 34: '78.96', 35: '79.90', 36: '83.80', 37: '85.47', 38: '87.62', 39: '88.91', 40: '91.22', 41: '92.91', 42: '95.94', 43: '98.00', 44: '101.07', 45: '102.91', 46: '106.42', 47: '107.87', 48: '112.41', 49: '114.82', 50: '118.71', 51: '121.76', 52: '127.6', 53: '126.9', 54: '131.29', 55: '132.91', 56: '137.33', 57: '138.91', 58: '140.12', 59: '140.91', 60: '144.24', 61: '145.0', 62: '150.36', 63: '151.97', 64: '157.25', 65: '158.93', 66: '162.5', 67: '164.93', 68: '167.26', 69: '168.93', 70: '173.04', 71: '174.97', 72: '178.49', 73: '180.95', 74: '183.84', 75: '186.21', 76: '190.23', 77: '192.22', 78: '195.08', 79: '196.97', 80: '200.59', 81: '204.38', 82: '207.2', 83: '208.98', 84: '209.0', 85: '210.00', 86: '222.0', 87: '223.0', 88: '226.0', 89: '227.0', 90: '232.04', 91: '231.04', 92: '238.03', 93: '237.0', 94: '244.0', 95: '243.0', 96: '247.0', 97: '247.0', 98: '251.0', 99: '252.0', 100: '257.0', 101: '258.0', 102: '259.0', 103: '262.0', 104: '261.0', 105: '262.0', 106: '266.00', 107: '264.00', 108: '277.00', 109: '268.0', 110: '269.0', 111: '272.0', 112: '285.00', 113: '286.00', 114: '289.00', 115: '289.00', 116: '293.00', 117: '293.00', 118: '294.00'}
-    
-  def __str__(self): #Add Latex String for Elements
-    """Get the string representation of the element.
-
-    :returns: The string representation of the element.
-    :rtype: str"""
-    return self.string
-
-  def __repr__(self):
-    """Get the string representation of the element.
-
-    :returns: The string representation of the element.
-    :rtype: str
-    """
-    return str(self)
-
-  def __eq__(self, other):
-    """Check if two elements are equal.
-
-    :param other: The other element to compare to.
-    :type other: Element
-    :returns: True if the elements are equal, False otherwise.
-    :rtype: bool
-    """
-    return self.string == other.string
-
-  def __hash__(self):
-    """Get the hash of the element.
-    
-    :returns: The hash of the element.
-    :rtype: int
-    """
+from pymeasurement.util.typecheck import typecheck
+from pymeasurement.measurement import Measurement
+
+class Element:
+  """A class to represent an chemical element.
+
+  :param string: The name of the element.
+    :type string: str
+    :param protons: The number of protons in the element.
+    :type protons: int or None
+    :param neutrons: The number of neutrons in the element.
+    :type neutrons: int or None
+    :param mass: The mass of the element.
+    :type mass: int or None
+  """
+  latexPrint = False # Whether to print the element in latex format.
+
+  def setLatexPrint(value):
+    """Set whether to print the element in latex format.
+
+    :param value: Whether to print the element in latex format.
+    :type value: bool
+    """
+    Element.latexPrint = value
+  
+  def __init__(self, string, protons = None, neutrons = None, mass = None):
+    """Element Constructor
+    """
+    typecheck(string, str)
+    typecheck(protons, int, None)
+    typecheck(neutrons, int, None)
+    typecheck(mass, int, None)
+    if not (len(string) > 0 and len(string) <= 2 and string.isalpha()):
+      raise Exception("Element Exception: Element Name must be 1 or 2 letters long.")
+    self.string = string
+    #Protons will only override if element does not exist.
+    self.protons = Element.elements().index(self.string) + 1 if self.string in Element.elements() else None
+    if self.protons == None:
+      self.protons = protons
+    self.neutrons = neutrons
+    self.mass = mass
+    total = (1 if self.protons != None else 0) + (1 if self.neutrons != None else 0) + (1 if self.mass != None else 0)
+    if total == 2:
+      if self.protons == None:
+        self.protons = self.mass - self.neutrons
+      elif self.neutrons == None:
+        self.neutrons = self.mass - self.protons
+      else:
+        self.mass = self.protons + self.neutrons
+
+    if self.mass == None:
+      self.mass = Measurement.fromStr(f'{Element.atomicWeights()[self.protons]}c') if self.protons in Element.atomicWeights() else None
+
+  def fromAtomicNumber(num):
+    """Create an element from an atomic number.
+
+    :param num: The atomic number of the element.
+    :type num: int
+    :returns: The element with the given atomic number.
+    """
+    if num < 1 or num > 118:
+      raise Exception("Element Exception: Atomic Number must be from 1-118.")
+    return Element(Element.elements[num-1])
+
+  def elements():
+    """Get a list of all elements.
+
+    :returns: A list of all elements.
+    :rtype: list
+    """
+    return ['H', 'He', 'Li', 'Be', 'B', 'C', 'N', 'O', 'F', 'Ne', 'Na', 'Mg', 'Al', 'Si', 'P', 'S', 'Cl', 'Ar', 'K', 'Ca', 'Sc', 'Ti', 'V', 'Cr', 'Mn', 'Fe', 'Co', 'Ni', 'Cu', 'Zn', 'Ga', 'Ge', 'As', 'Se', 'Br', 'Kr', 'Rb', 'Sr', 'Y', 'Zr', 'Nb', 'Mo', 'Tc', 'Ru', 'Rh', 'Pd', 'Ag', 'Cd', 'In', 'Sn', 'Sb', 'Te', 'I', 'Xe', 'Cs', 'Ba', 'La', 'Ce', 'Pr', 'Nd', 'Pm', 'Sm', 'Eu', 'Gd', 'Tb', 'Dy', 'Ho', 'Er', 'Tm', 'Yb', 'Lu', 'Hf', 'Ta', 'W', 'Re', 'Os', 'Ir', 'Pt', 'Au', 'Hg', 'Tl', 'Pb', 'Bi', 'Po', 'At', 'Rn', 'Fr', 'Ra', 'Ac', 'Th', 'Pa', 'U', 'Np', 'Pu', 'Am', 'Cm', 'Bk', 'Cf', 'Es', 'Fm', 'Md', 'No', 'Lr', 'Rf', 'Db', 'Sg', 'Bh', 'Hs', 'Mt', 'Ds', 'Rg', 'Cn', 'Nh', 'Fl', 'Mc', 'Lv', 'Ts', 'Og']
+
+  def atomicWeights():
+    """Get a dictionary of all atomic weights.
+
+    :returns: A dictionary of all atomic weights.
+    :rtype: dict
+    """
+    return {1: '1.01', 2: '4.00', 3: '6.94', 4: '9.01', 5: '10.81', 6: '12.01', 7: '14.01', 8: '16.00', 9: '19.00', 10: '20.18', 11: '22.99', 12: '24.31', 13: '26.98', 14: '28.09', 15: '30.97', 16: '32.07', 17: '35.45', 18: '39.95', 19: '39.1', 20: '40.08', 21: '44.96', 22: '47.87', 23: '50.94', 24: '52.00', 25: '54.94', 26: '55.85', 27: '58.93', 28: '58.69', 29: '63.55', 30: '65.41', 31: '69.72', 32: '72.64', 33: '74.92', 34: '78.96', 35: '79.90', 36: '83.80', 37: '85.47', 38: '87.62', 39: '88.91', 40: '91.22', 41: '92.91', 42: '95.94', 43: '98.00', 44: '101.07', 45: '102.91', 46: '106.42', 47: '107.87', 48: '112.41', 49: '114.82', 50: '118.71', 51: '121.76', 52: '127.6', 53: '126.9', 54: '131.29', 55: '132.91', 56: '137.33', 57: '138.91', 58: '140.12', 59: '140.91', 60: '144.24', 61: '145.0', 62: '150.36', 63: '151.97', 64: '157.25', 65: '158.93', 66: '162.5', 67: '164.93', 68: '167.26', 69: '168.93', 70: '173.04', 71: '174.97', 72: '178.49', 73: '180.95', 74: '183.84', 75: '186.21', 76: '190.23', 77: '192.22', 78: '195.08', 79: '196.97', 80: '200.59', 81: '204.38', 82: '207.2', 83: '208.98', 84: '209.0', 85: '210.00', 86: '222.0', 87: '223.0', 88: '226.0', 89: '227.0', 90: '232.04', 91: '231.04', 92: '238.03', 93: '237.0', 94: '244.0', 95: '243.0', 96: '247.0', 97: '247.0', 98: '251.0', 99: '252.0', 100: '257.0', 101: '258.0', 102: '259.0', 103: '262.0', 104: '261.0', 105: '262.0', 106: '266.00', 107: '264.00', 108: '277.00', 109: '268.0', 110: '269.0', 111: '272.0', 112: '285.00', 113: '286.00', 114: '289.00', 115: '289.00', 116: '293.00', 117: '293.00', 118: '294.00'}
+    
+  def __str__(self): #Add Latex String for Elements
+    """Get the string representation of the element.
+
+    :returns: The string representation of the element.
+    :rtype: str"""
+    return self.string
+
+  def __repr__(self):
+    """Get the string representation of the element.
+
+    :returns: The string representation of the element.
+    :rtype: str
+    """
+    return str(self)
+
+  def __eq__(self, other):
+    """Check if two elements are equal.
+
+    :param other: The other element to compare to.
+    :type other: Element
+    :returns: True if the elements are equal, False otherwise.
+    :rtype: bool
+    """
+    return self.string == other.string
+
+  def __hash__(self):
+    """Get the hash of the element.
+    
+    :returns: The hash of the element.
+    :rtype: int
+    """
     return hash(self.string)
```

### Comparing `pymeasurement-1.0.8/tests/test_pymeasurement.py` & `pymeasurement-1.0.9/tests/test_pymeasurement.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-import unittest
-import sys
-import os
-sys.path.insert(0, os.path.join(os.path.dirname(__file__), '..', 'src'))
-from pymeasurement import Measurement
-from pymeasurement.sigfig import SigFig
-
-class TestMeasurement(unittest.TestCase):
-    def test_create_measurement(self):
-        m = Measurement("2.0", uncertainty="0.13", units="m")
-        self.assertEqual(m.sample, SigFig("2.0"))
-        self.assertEqual(m.uncertainty, SigFig("0.1"))
-        self.assertEqual(m.units, "m")
-        self.assertEqual(str(m), "2.0 +/- 0.1 m")
-
-    def test_create_measurement_with_sigfigs(self):
-        m = Measurement("2.0", uncertainty="0.13", units="m", precision=3)
-        self.assertEqual(m.sample, SigFig("2.00"))
-        self.assertEqual(m.uncertainty, SigFig("0.13"))
-        self.assertEqual(m.units, "m")
-        self.assertEqual(str(m), "2.00 +/- 0.13 m")
-
-    def test_create_measurement_from_str(self):
-        m = Measurement.fromStr("2.0 +/- 0.13 m")
-        self.assertEqual(m.sample, SigFig("2.0"))
-        self.assertEqual(m.uncertainty, SigFig("0.1"))
-        self.assertEqual(m.units, "m")
-        self.assertEqual(str(m), "2.0 +/- 0.1 m")
-
-    def test_create_measurement_from_float(self):
-        m = Measurement.fromFloat(3.14)
-        self.assertEqual(m.sample, SigFig("3.14", constant=True))
-        self.assertEqual(m.uncertainty, None)
-        self.assertEqual(m.sample.sigfigs, float("inf"))
-        self.assertEqual(str(m), "3.14")
-
-    def test_add_measurements(self):
-        m1 = Measurement("2.0", uncertainty="0.13", units="m")
-        m2 = Measurement("3.0", uncertainty="0.1", units="m")
-        m3 = m1 + m2
-        self.assertEqual(m3.sample, SigFig("5.0"))
-        self.assertEqual(m3.uncertainty, SigFig("0.2"))
-        self.assertEqual(m3.units, "m")
-        self.assertEqual(str(m3), "5.0 +/- 0.2 m")
-    
-    def test_subtract_measurments(self):
-        m1 = Measurement("2.0", uncertainty="0.13", units="m")
-        m2 = Measurement("3.0", uncertainty="0.1", units="m")
-        m3 = m1 - m2
-        self.assertEqual(m3.sample, SigFig("-1.0"))
-        self.assertEqual(m3.uncertainty, SigFig("0.2"))
-        self.assertEqual(m3.units, "m")
-        self.assertEqual(str(m3), "-1.0 +/- 0.2 m")
-
-    def test_multiply_measurements(self):
-        m1 = Measurement("2.0", uncertainty="0.13", units="m")
-        m2 = Measurement("3.0", uncertainty="0.1", units="m")
-        m3 = m1 * m2
-        self.assertEqual(m3.sample, SigFig("6.0"))
-        self.assertEqual(m3.absolute().uncertainty, SigFig("0.6"))
-        self.assertEqual(m3.units, "m^2")
-        self.assertEqual(str(m3), "6.0 +/- 1E+1% m^2")
-
-    def test_divide_measurements(self):
-        m1 = Measurement("2.0", uncertainty="0.13", units="m")
-        m2 = Measurement("3.0", uncertainty="0.1", units="m")
-        m3 = m1 / m2
-        self.assertEqual(m3.sample, SigFig("0.67"))
-        self.assertEqual(m3.uncertainty, SigFig("10", sigfigs=1))
-        self.assertEqual(m3.units, None)
-        self.assertEqual(str(m3), "0.67 +/- 1E+1%")
-
-    def test_add_measurement_to_scalar(self):
-        m1 = Measurement("2.0", uncertainty="0.13", units="m")
-        m2 = m1 + Measurement.fromFloat(2, units="m")
-        self.assertEqual(m2.sample, SigFig("4.0"))
-        self.assertEqual(m2.uncertainty, SigFig("0.1"))
-        self.assertEqual(m2.units, "m")
-        self.assertEqual(str(m2), "4.0 +/- 0.1 m")
-
-    def test_subtract_scalar_from_measurement(self):
-        m1 = Measurement("2.0", uncertainty="0.13", units="m")
-        m2 = m1 - Measurement.fromFloat(2, units="m")
-        self.assertEqual(m2.sample, SigFig("0.0"))
-        self.assertEqual(m2.uncertainty, SigFig("0.1"))
-        self.assertEqual(m2.units, "m")
-        self.assertEqual(str(m2), "0.0 +/- 0.1 m")
-
-    def test_divide_measurement_by_scalar(self):
-        m1 = Measurement("2.0", uncertainty="0.13", units="m")
-        m2 = m1 / 2
-        self.assertEqual(m2.sample, SigFig("1.0"))
-        self.assertEqual(m2.uncertainty, SigFig("6"))
-        self.assertEqual(m2.units, "m")
-        self.assertEqual(str(m2), "1.0 +/- 6% m")
-
-    def test_multiply_measurement_by_scalar(self):
-        m1 = Measurement("2.0", uncertainty="0.13", units="m")
-        m2 = m1 * 2
-        self.assertEqual(m2.sample, SigFig("4.0"))
-        self.assertEqual(m2.uncertainty, SigFig("6"))
-        self.assertEqual(m2.units, "m")
-        self.assertEqual(str(m2), "4.0 +/- 6% m")
-
-    def test_square_measurement(self):
-        m1 = Measurement("2.0", uncertainty="0.13", units="m")
-        m2 = m1 ** 2
-        self.assertEqual(m2.sample, SigFig("4.0"))
-        self.assertEqual(m2.uncertainty, SigFig("1E+1"))
-        self.assertEqual(m2.units, "m^2")
-        self.assertEqual(str(m2), "4.0 +/- 1E+1% m^2")
-
-    def test_absolute_uncertainty(self):
-        m = Measurement.fromStr("2.0 +/- 0.13 m")
-        self.assertEqual(m.absolute().uncertainty, SigFig("0.1"))
-        self.assertEqual(m.absolute().units, "m")
-        self.assertEqual(str(m.absolute()), "2.0 +/- 0.1 m")
-
-    def test_percent_uncertainty(self):
-        m = Measurement.fromStr("2.0 +/- 0.13 m")
-        self.assertEqual(m.percent().uncertainty, SigFig("6", sigfigs=1))
-        self.assertEqual(m.percent().units, "m")
-        self.assertEqual(str(m.percent()), "2.0 +/- 6% m")
-
-    def test_sum_measurements(self):
-        m1 = Measurement.fromStr("2.0 +/- 0.13 m")
-        m2 = Measurement.fromStr("3.0 +/- 0.1 m")
-        m3 = Measurement.fromStr("4.0 +/- 0.1 m")
-        m4 = Measurement.sum([m1, m2, m3])
-        self.assertEqual(m4.sample, SigFig("9.0"))
-        self.assertEqual(m4.uncertainty, SigFig("0.3"))
-        self.assertEqual(m4.units, "m")
-        self.assertEqual(str(m4), "9.0 +/- 0.3 m")
-
-    def test_max_measurements(self):
-        m1 = Measurement.fromStr("2.0 +/- 0.13 m")
-        m2 = Measurement.fromStr("3.0 +/- 0.1 m")
-        m3 = Measurement.fromStr("4.0 +/- 0.1 m")
-        m4 = max([m1, m2, m3])
-        self.assertEqual(m4.sample, SigFig("4.0"))
-        self.assertEqual(m4.uncertainty, SigFig("0.1"))
-        self.assertEqual(m4.units, "m")
-        self.assertEqual(str(m4), "4.0 +/- 0.1 m")
-
-    def test_min_measurements(self):
-        m1 = Measurement.fromStr("2.0 +/- 0.13 m")
-        m2 = Measurement.fromStr("3.0 +/- 0.1 m")
-        m3 = Measurement.fromStr("4.0 +/- 0.1 m")
-        m4 = min([m1, m2, m3])
-        self.assertEqual(m4.sample, SigFig("2.0"))
-        self.assertEqual(m4.uncertainty, SigFig("0.1"))
-        self.assertEqual(m4.units, "m")
-        self.assertEqual(str(m4), "2.0 +/- 0.1 m")    
-
-    def test_average_measurements(self):
-        m1 = Measurement.fromStr("2.0 +/- 0.13 m")
-        m2 = Measurement.fromStr("3.0 +/- 0.1 m")
-        m3 = Measurement.fromStr("4.0 +/- 0.1 m")
-        m4 = Measurement.average([m1, m2, m3])
-        self.assertEqual(m4.sample, SigFig("3.0"))
-        self.assertEqual(m4.uncertainty, SigFig("0.58"))
-        self.assertEqual(m4.units, "m")
+import unittest
+import sys
+import os
+sys.path.insert(0, os.path.join(os.path.dirname(__file__), '..', 'src'))
+from pymeasurement import Measurement
+from pymeasurement.sigfig import SigFig
+
+class TestMeasurement(unittest.TestCase):
+    def test_create_measurement(self):
+        m = Measurement("2.0", uncertainty="0.13", units="m")
+        self.assertEqual(m.sample, SigFig("2.0"))
+        self.assertEqual(m.uncertainty, SigFig("0.1"))
+        self.assertEqual(m.units, "m")
+        self.assertEqual(str(m), "2.0 +/- 0.1 m")
+
+    def test_create_measurement_with_sigfigs(self):
+        m = Measurement("2.0", uncertainty="0.13", units="m", precision=3)
+        self.assertEqual(m.sample, SigFig("2.00"))
+        self.assertEqual(m.uncertainty, SigFig("0.13"))
+        self.assertEqual(m.units, "m")
+        self.assertEqual(str(m), "2.00 +/- 0.13 m")
+
+    def test_create_measurement_from_str(self):
+        m = Measurement.fromStr("2.0 +/- 0.13 m")
+        self.assertEqual(m.sample, SigFig("2.0"))
+        self.assertEqual(m.uncertainty, SigFig("0.1"))
+        self.assertEqual(m.units, "m")
+        self.assertEqual(str(m), "2.0 +/- 0.1 m")
+
+    def test_create_measurement_from_float(self):
+        m = Measurement.fromFloat(3.14)
+        self.assertEqual(m.sample, SigFig("3.14", constant=True))
+        self.assertEqual(m.uncertainty, None)
+        self.assertEqual(m.sample.sigfigs, float("inf"))
+        self.assertEqual(str(m), "3.14")
+
+    def test_add_measurements(self):
+        m1 = Measurement("2.0", uncertainty="0.13", units="m")
+        m2 = Measurement("3.0", uncertainty="0.1", units="m")
+        m3 = m1 + m2
+        self.assertEqual(m3.sample, SigFig("5.0"))
+        self.assertEqual(m3.uncertainty, SigFig("0.2"))
+        self.assertEqual(m3.units, "m")
+        self.assertEqual(str(m3), "5.0 +/- 0.2 m")
+    
+    def test_subtract_measurments(self):
+        m1 = Measurement("2.0", uncertainty="0.13", units="m")
+        m2 = Measurement("3.0", uncertainty="0.1", units="m")
+        m3 = m1 - m2
+        self.assertEqual(m3.sample, SigFig("-1.0"))
+        self.assertEqual(m3.uncertainty, SigFig("0.2"))
+        self.assertEqual(m3.units, "m")
+        self.assertEqual(str(m3), "-1.0 +/- 0.2 m")
+
+    def test_multiply_measurements(self):
+        m1 = Measurement("2.0", uncertainty="0.13", units="m")
+        m2 = Measurement("3.0", uncertainty="0.1", units="m")
+        m3 = m1 * m2
+        self.assertEqual(m3.sample, SigFig("6.0"))
+        self.assertEqual(m3.absolute().uncertainty, SigFig("0.6"))
+        self.assertEqual(m3.units, "m^2")
+        self.assertEqual(str(m3), "6.0 +/- 1E+1% m^2")
+
+    def test_divide_measurements(self):
+        m1 = Measurement("2.0", uncertainty="0.13", units="m")
+        m2 = Measurement("3.0", uncertainty="0.1", units="m")
+        m3 = m1 / m2
+        self.assertEqual(m3.sample, SigFig("0.67"))
+        self.assertEqual(m3.uncertainty, SigFig("10", sigfigs=1))
+        self.assertEqual(m3.units, None)
+        self.assertEqual(str(m3), "0.67 +/- 1E+1%")
+
+    def test_add_measurement_to_scalar(self):
+        m1 = Measurement("2.0", uncertainty="0.13", units="m")
+        m2 = m1 + Measurement.fromFloat(2, units="m")
+        self.assertEqual(m2.sample, SigFig("4.0"))
+        self.assertEqual(m2.uncertainty, SigFig("0.1"))
+        self.assertEqual(m2.units, "m")
+        self.assertEqual(str(m2), "4.0 +/- 0.1 m")
+
+    def test_subtract_scalar_from_measurement(self):
+        m1 = Measurement("2.0", uncertainty="0.13", units="m")
+        m2 = m1 - Measurement.fromFloat(2, units="m")
+        self.assertEqual(m2.sample, SigFig("0.0"))
+        self.assertEqual(m2.uncertainty, SigFig("0.1"))
+        self.assertEqual(m2.units, "m")
+        self.assertEqual(str(m2), "0.0 +/- 0.1 m")
+
+    def test_divide_measurement_by_scalar(self):
+        m1 = Measurement("2.0", uncertainty="0.13", units="m")
+        m2 = m1 / 2
+        self.assertEqual(m2.sample, SigFig("1.0"))
+        self.assertEqual(m2.uncertainty, SigFig("6"))
+        self.assertEqual(m2.units, "m")
+        self.assertEqual(str(m2), "1.0 +/- 6% m")
+
+    def test_multiply_measurement_by_scalar(self):
+        m1 = Measurement("2.0", uncertainty="0.13", units="m")
+        m2 = m1 * 2
+        self.assertEqual(m2.sample, SigFig("4.0"))
+        self.assertEqual(m2.uncertainty, SigFig("6"))
+        self.assertEqual(m2.units, "m")
+        self.assertEqual(str(m2), "4.0 +/- 6% m")
+
+    def test_square_measurement(self):
+        m1 = Measurement("2.0", uncertainty="0.13", units="m")
+        m2 = m1 ** 2
+        self.assertEqual(m2.sample, SigFig("4.0"))
+        self.assertEqual(m2.uncertainty, SigFig("1E+1"))
+        self.assertEqual(m2.units, "m^2")
+        self.assertEqual(str(m2), "4.0 +/- 1E+1% m^2")
+
+    def test_absolute_uncertainty(self):
+        m = Measurement.fromStr("2.0 +/- 0.13 m")
+        self.assertEqual(m.absolute().uncertainty, SigFig("0.1"))
+        self.assertEqual(m.absolute().units, "m")
+        self.assertEqual(str(m.absolute()), "2.0 +/- 0.1 m")
+
+    def test_percent_uncertainty(self):
+        m = Measurement.fromStr("2.0 +/- 0.13 m")
+        self.assertEqual(m.percent().uncertainty, SigFig("6", sigfigs=1))
+        self.assertEqual(m.percent().units, "m")
+        self.assertEqual(str(m.percent()), "2.0 +/- 6% m")
+
+    def test_sum_measurements(self):
+        m1 = Measurement.fromStr("2.0 +/- 0.13 m")
+        m2 = Measurement.fromStr("3.0 +/- 0.1 m")
+        m3 = Measurement.fromStr("4.0 +/- 0.1 m")
+        m4 = Measurement.sum([m1, m2, m3])
+        self.assertEqual(m4.sample, SigFig("9.0"))
+        self.assertEqual(m4.uncertainty, SigFig("0.3"))
+        self.assertEqual(m4.units, "m")
+        self.assertEqual(str(m4), "9.0 +/- 0.3 m")
+
+    def test_max_measurements(self):
+        m1 = Measurement.fromStr("2.0 +/- 0.13 m")
+        m2 = Measurement.fromStr("3.0 +/- 0.1 m")
+        m3 = Measurement.fromStr("4.0 +/- 0.1 m")
+        m4 = max([m1, m2, m3])
+        self.assertEqual(m4.sample, SigFig("4.0"))
+        self.assertEqual(m4.uncertainty, SigFig("0.1"))
+        self.assertEqual(m4.units, "m")
+        self.assertEqual(str(m4), "4.0 +/- 0.1 m")
+
+    def test_min_measurements(self):
+        m1 = Measurement.fromStr("2.0 +/- 0.13 m")
+        m2 = Measurement.fromStr("3.0 +/- 0.1 m")
+        m3 = Measurement.fromStr("4.0 +/- 0.1 m")
+        m4 = min([m1, m2, m3])
+        self.assertEqual(m4.sample, SigFig("2.0"))
+        self.assertEqual(m4.uncertainty, SigFig("0.1"))
+        self.assertEqual(m4.units, "m")
+        self.assertEqual(str(m4), "2.0 +/- 0.1 m")    
+
+    def test_average_measurements(self):
+        m1 = Measurement.fromStr("2.0 +/- 0.13 m")
+        m2 = Measurement.fromStr("3.0 +/- 0.1 m")
+        m3 = Measurement.fromStr("4.0 +/- 0.1 m")
+        m4 = Measurement.average([m1, m2, m3])
+        self.assertEqual(m4.sample, SigFig("3.0"))
+        self.assertEqual(m4.uncertainty, SigFig("0.6"))
+        self.assertEqual(m4.units, "m")
         self.assertEqual(str(m4), "3.0 +/- 0.6 m")
```

### Comparing `pymeasurement-1.0.8/LICENSE` & `pymeasurement-1.0.9/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 SaptakD625
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 SaptakD625
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pymeasurement-1.0.8/README.md` & `pymeasurement-1.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: pymeasurement
+Version: 1.0.9
+Summary: A Measurement Calculator with Fixed Point Precision, Uncertainties, and Units
+Project-URL: Homepage, https://github.com/Saptak625/pymeasurement
+Project-URL: Bug Tracker, https://github.com/Saptak625/pymeasurement/issues
+Author-email: Saptak Das <saptak.das625@gmail.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # pymeasurement
 A Measurement Calculator with Fixed Point Precision, Uncertainties, and Units.
 
 View at [PyPi], [Github], and [Read the Docs].
 
 ## Installation
 pymeasurement is distributed on [PyPI].
```

