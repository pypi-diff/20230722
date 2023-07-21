# Comparing `tmp/pdf_reports-0.3.4.tar.gz` & `tmp/pdf_reports-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_reports-0.3.4.tar", last modified: Thu May  5 12:58:46 2022, max compression
+gzip compressed data, was "pdf_reports-0.3.5.tar", last modified: Fri Jul 21 22:25:37 2023, max compression
```

## Comparing `pdf_reports-0.3.4.tar` & `pdf_reports-0.3.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 12:58:46.227334 pdf_reports-0.3.4/
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1081 2022-05-05 10:51:32.000000 pdf_reports-0.3.4/LICENCE.txt
--rwxrwxr-x   0 peter     (1000) peter     (1000)       84 2022-05-05 10:51:32.000000 pdf_reports-0.3.4/MANIFEST.in
--rw-rw-r--   0 peter     (1000) peter     (1000)     2279 2022-05-05 12:58:46.227334 pdf_reports-0.3.4/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     7053 2022-05-05 12:58:35.000000 pdf_reports-0.3.4/README.rst
--rwxrwxr-x   0 peter     (1000) peter     (1000)     8512 2022-05-05 10:51:32.000000 pdf_reports-0.3.4/ez_setup.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 12:58:46.223334 pdf_reports-0.3.4/pdf_reports/
--rw-rw-r--   0 peter     (1000) peter     (1000)      239 2022-05-05 10:51:32.000000 pdf_reports-0.3.4/pdf_reports/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 12:58:46.227334 pdf_reports-0.3.4/pdf_reports/css/
--rwxrwxr-x   0 peter     (1000) peter     (1000)    19352 2022-05-05 10:51:32.000000 pdf_reports-0.3.4/pdf_reports/css/egf-logo.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)   618735 2022-05-05 10:51:32.000000 pdf_reports-0.3.4/pdf_reports/css/semantic.min.css
--rw-rw-r--   0 peter     (1000) peter     (1000)     1502 2022-05-05 10:51:32.000000 pdf_reports-0.3.4/pdf_reports/css/style.css
--rw-rw-r--   0 peter     (1000) peter     (1000)     6822 2022-05-05 10:51:32.000000 pdf_reports-0.3.4/pdf_reports/pdf_reports.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5695 2022-05-05 12:58:35.000000 pdf_reports-0.3.4/pdf_reports/tools.py
--rw-rw-r--   0 peter     (1000) peter     (1000)       22 2022-05-05 12:58:35.000000 pdf_reports-0.3.4/pdf_reports/version.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-05-05 12:58:46.223334 pdf_reports-0.3.4/pdf_reports.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)     2279 2022-05-05 12:58:45.000000 pdf_reports-0.3.4/pdf_reports.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      428 2022-05-05 12:58:46.000000 pdf_reports-0.3.4/pdf_reports.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2022-05-05 12:58:45.000000 pdf_reports-0.3.4/pdf_reports.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       91 2022-05-05 12:58:46.000000 pdf_reports-0.3.4/pdf_reports.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       12 2022-05-05 12:58:46.000000 pdf_reports-0.3.4/pdf_reports.egg-info/top_level.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)     1981 2022-05-05 10:51:32.000000 pdf_reports-0.3.4/pypi-readme.rst
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2022-05-05 12:58:46.227334 pdf_reports-0.3.4/setup.cfg
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1299 2022-05-05 10:51:32.000000 pdf_reports-0.3.4/setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-21 22:25:37.636816 pdf_reports-0.3.5/
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1081 2022-05-05 10:51:32.000000 pdf_reports-0.3.5/LICENCE.txt
+-rwxrwxr-x   0 peter     (1000) peter     (1000)       84 2022-05-05 10:51:32.000000 pdf_reports-0.3.5/MANIFEST.in
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1888 2023-07-21 22:25:37.636816 pdf_reports-0.3.5/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7102 2023-07-21 22:25:15.000000 pdf_reports-0.3.5/README.rst
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     8512 2022-05-05 10:51:32.000000 pdf_reports-0.3.5/ez_setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-21 22:25:37.632816 pdf_reports-0.3.5/pdf_reports/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      239 2022-05-05 10:51:32.000000 pdf_reports-0.3.5/pdf_reports/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-21 22:25:37.636816 pdf_reports-0.3.5/pdf_reports/css/
+-rwxrwxr-x   0 peter     (1000) peter     (1000)    19352 2022-05-05 10:51:32.000000 pdf_reports-0.3.5/pdf_reports/css/egf-logo.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)   618735 2022-05-05 10:51:32.000000 pdf_reports-0.3.5/pdf_reports/css/semantic.min.css
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1502 2022-05-05 10:51:32.000000 pdf_reports-0.3.5/pdf_reports/css/style.css
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6822 2022-05-05 10:51:32.000000 pdf_reports-0.3.5/pdf_reports/pdf_reports.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5645 2023-07-21 22:25:15.000000 pdf_reports-0.3.5/pdf_reports/tools.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)       22 2023-07-21 22:25:15.000000 pdf_reports-0.3.5/pdf_reports/version.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-21 22:25:37.632816 pdf_reports-0.3.5/pdf_reports.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1888 2023-07-21 22:25:36.000000 pdf_reports-0.3.5/pdf_reports.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      428 2023-07-21 22:25:37.000000 pdf_reports-0.3.5/pdf_reports.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-07-21 22:25:37.000000 pdf_reports-0.3.5/pdf_reports.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       87 2023-07-21 22:25:37.000000 pdf_reports-0.3.5/pdf_reports.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       12 2023-07-21 22:25:37.000000 pdf_reports-0.3.5/pdf_reports.egg-info/top_level.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1590 2023-07-21 22:25:15.000000 pdf_reports-0.3.5/pypi-readme.rst
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-07-21 22:25:37.636816 pdf_reports-0.3.5/setup.cfg
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1295 2023-07-21 22:25:15.000000 pdf_reports-0.3.5/setup.py
```

### Comparing `pdf_reports-0.3.4/LICENCE.txt` & `pdf_reports-0.3.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.4/PKG-INFO` & `pdf_reports-0.3.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 Metadata-Version: 2.1
 Name: pdf_reports
-Version: 0.3.4
+Version: 0.3.5
 Summary: Create nice-looking PDF reports from HTML content.
 Home-page: https://github.com/Edinburgh-Genome-Foundry/pdf_reports
 Author: Zulko
 License: MIT
 Keywords: PDF report web jinja weasyprint
 Platform: UNKNOWN
 License-File: LICENCE.txt
 
 PDF Reports
 ===========
 
-.. image:: https://travis-ci.org/Edinburgh-Genome-Foundry/pdf_reports.svg?branch=master
-   :target: https://travis-ci.org/Edinburgh-Genome-Foundry/pdf_reports
-   :alt: Travis CI build status
-
-.. image:: https://coveralls.io/repos/github/Edinburgh-Genome-Foundry/pdf_reports/badge.svg?branch=master
-   :target: https://coveralls.io/github/Edinburgh-Genome-Foundry/pdf_reports?branch=master
-
-
 *PDF Reports* (complete documentation `here <https://edinburgh-genome-foundry.github.io/pdf_reports/>`_) is a Python library to create nice-looking PDF reports from HTML or `Pug <https://pugjs.org>`_ templates. It features modern-looking components (via the `Semantic UI <https://semantic-ui.com/>`_ framework) and provides routines to embed tables or plots in the documents.
 
 
 Example of use
 --------------
 
 Your Pug template file ``template.pug`` may look like this (see a `full example <https://github.com/Edinburgh-Genome-Foundry/pdf_reports/blob/master/examples/example_template.pug>`_):
```

### Comparing `pdf_reports-0.3.4/README.rst` & `pdf_reports-0.3.5/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
     <br /><br />
     </p>
 
 
 PDF_Reports
 ===========
 
-.. image:: https://travis-ci.com/Edinburgh-Genome-Foundry/pdf_reports.svg?branch=master
-   :target: https://travis-ci.com/Edinburgh-Genome-Foundry/pdf_reports
-   :alt: Travis CI build status
+.. image:: https://github.com/Edinburgh-Genome-Foundry/pdf_reports/actions/workflows/build.yml/badge.svg
+   :target: https://github.com/Edinburgh-Genome-Foundry/pdf_reports/actions/workflows/build.yml
+   :alt: GitHub CI build status
 
 .. image:: https://coveralls.io/repos/github/Edinburgh-Genome-Foundry/pdf_reports/badge.svg?branch=master
    :target: https://coveralls.io/github/Edinburgh-Genome-Foundry/pdf_reports?branch=master
 
 
 
 *PDF Reports* (complete documentation `here <https://edinburgh-genome-foundry.github.io/pdf_reports/>`_) is a Python library to create nice-looking PDF reports from HTML or `Pug <https://pugjs.org>`_ templates. It features modern-looking components (via the `Semantic UI <https://semantic-ui.com/>`_ framework) and provides routines to embed tables or plots in the documents.
@@ -170,18 +170,20 @@
 
 Alternatively, you can unzip the sources in a folder and type:
 
 .. code::
 
     python setup.py install
 
-**Note:** the package depends on the WeasyPrint Python package. If there are any issues, see installation instructions
-in the `WeasyPrint documentation <https://doc.courtbouillon.org/weasyprint/stable/first_steps.html>`_.
-The version is `fixed to <=52 <https://github.com/Edinburgh-Genome-Foundry/pdf_reports/blob/master/setup.py>`_
-as not all GNU/Linux distributions have the latest Pango that is required by the latest WeasyPrint.
+**Note:** the package depends on the WeasyPrint Python package. If there are any issues,
+see installation instructions in the `WeasyPrint documentation <https://doc.courtbouillon.org/weasyprint/stable/first_steps.html>`_.
+
+If you have an older GNU/Linux distribution (e.g. Ubuntu 18.04), then install an older WeasyPrint (<=52),
+as they don't have the latest Pango that is required by the latest WeasyPrint: ``pip install weasyprint==52``
+
 
 **Note: on some Debian systems** you may need to first install ``libffi-dev`` (``apt install libffi-dev``). The package name may be ``libffi-devel`` on some systems.
 
 **Note: on macOS,** you may need to first install pango with: ``brew install pango``
 
 
 License = MIT
```

### Comparing `pdf_reports-0.3.4/ez_setup.py` & `pdf_reports-0.3.5/ez_setup.py`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.4/pdf_reports/css/egf-logo.svg` & `pdf_reports-0.3.5/pdf_reports/css/egf-logo.svg`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.4/pdf_reports/css/semantic.min.css` & `pdf_reports-0.3.5/pdf_reports/css/semantic.min.css`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.4/pdf_reports/css/style.css` & `pdf_reports-0.3.5/pdf_reports/css/style.css`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.4/pdf_reports/pdf_reports.py` & `pdf_reports-0.3.5/pdf_reports/pdf_reports.py`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.4/pdf_reports/tools.py` & `pdf_reports-0.3.5/pdf_reports/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from bs4 import BeautifulSoup
 import base64
 import pandas
 from io import BytesIO
 import datetime
 import textwrap
 
+from matplotlib.axes import Axes
+
 
 def dataframe_to_html(
     dataframe,
     extra_classes=(),
     index=False,
     header=True,
     use_default_classes=True,
@@ -153,16 +155,15 @@
     bbox_inches
       Keeping this option to "tight" will ensure that your plot's delimitation
       is optimal.
 
     **kwargs
       Any other option of Matplotlib's figure.savefig() method.
     """
-    if "AxesSubplot" in str(fig.__class__):
-        # A matplotlib axis was provided: take its containing figure.
+    if isinstance(fig, Axes):
         fig = fig.figure
     output = BytesIO()
     original_size = fig.get_size_inches()
     if size is not None:
         fig.set_size_inches((int(size[0]), int(size[1])))
     fig.savefig(output, format=fmt, bbox_inches=bbox_inches, **kwargs)
     fig.set_size_inches(original_size)
```

### Comparing `pdf_reports-0.3.4/pdf_reports.egg-info/PKG-INFO` & `pdf_reports-0.3.5/pdf_reports.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 Metadata-Version: 2.1
 Name: pdf-reports
-Version: 0.3.4
+Version: 0.3.5
 Summary: Create nice-looking PDF reports from HTML content.
 Home-page: https://github.com/Edinburgh-Genome-Foundry/pdf_reports
 Author: Zulko
 License: MIT
 Keywords: PDF report web jinja weasyprint
 Platform: UNKNOWN
 License-File: LICENCE.txt
 
 PDF Reports
 ===========
 
-.. image:: https://travis-ci.org/Edinburgh-Genome-Foundry/pdf_reports.svg?branch=master
-   :target: https://travis-ci.org/Edinburgh-Genome-Foundry/pdf_reports
-   :alt: Travis CI build status
-
-.. image:: https://coveralls.io/repos/github/Edinburgh-Genome-Foundry/pdf_reports/badge.svg?branch=master
-   :target: https://coveralls.io/github/Edinburgh-Genome-Foundry/pdf_reports?branch=master
-
-
 *PDF Reports* (complete documentation `here <https://edinburgh-genome-foundry.github.io/pdf_reports/>`_) is a Python library to create nice-looking PDF reports from HTML or `Pug <https://pugjs.org>`_ templates. It features modern-looking components (via the `Semantic UI <https://semantic-ui.com/>`_ framework) and provides routines to embed tables or plots in the documents.
 
 
 Example of use
 --------------
 
 Your Pug template file ``template.pug`` may look like this (see a `full example <https://github.com/Edinburgh-Genome-Foundry/pdf_reports/blob/master/examples/example_template.pug>`_):
```

### Comparing `pdf_reports-0.3.4/pypi-readme.rst` & `pdf_reports-0.3.5/pypi-readme.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,10 @@
 PDF Reports
 ===========
 
-.. image:: https://travis-ci.org/Edinburgh-Genome-Foundry/pdf_reports.svg?branch=master
-   :target: https://travis-ci.org/Edinburgh-Genome-Foundry/pdf_reports
-   :alt: Travis CI build status
-
-.. image:: https://coveralls.io/repos/github/Edinburgh-Genome-Foundry/pdf_reports/badge.svg?branch=master
-   :target: https://coveralls.io/github/Edinburgh-Genome-Foundry/pdf_reports?branch=master
-
-
 *PDF Reports* (complete documentation `here <https://edinburgh-genome-foundry.github.io/pdf_reports/>`_) is a Python library to create nice-looking PDF reports from HTML or `Pug <https://pugjs.org>`_ templates. It features modern-looking components (via the `Semantic UI <https://semantic-ui.com/>`_ framework) and provides routines to embed tables or plots in the documents.
 
 
 Example of use
 --------------
 
 Your Pug template file ``template.pug`` may look like this (see a `full example <https://github.com/Edinburgh-Genome-Foundry/pdf_reports/blob/master/examples/example_template.pug>`_):
```

### Comparing `pdf_reports-0.3.4/setup.py` & `pdf_reports-0.3.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     license="MIT",
     keywords="PDF report web jinja weasyprint",
     packages=find_packages(exclude="docs"),
     include_package_data=True,
     install_requires=[
         "pypugjs",
         "jinja2",
-        "weasyprint<=52",
+        "weasyprint",
         "beautifulsoup4",
         "pandas",
         "Markdown",
         "backports.functools-lru-cache",
     ],
 )
```

