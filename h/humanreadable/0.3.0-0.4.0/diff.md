# Comparing `tmp/humanreadable-0.3.0.tar.gz` & `tmp/humanreadable-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humanreadable-0.3.0.tar", last modified: Sat Apr 22 17:38:07 2023, max compression
+gzip compressed data, was "humanreadable-0.4.0.tar", last modified: Sat Jul 22 15:34:12 2023, max compression
```

## Comparing `humanreadable-0.3.0.tar` & `humanreadable-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-04-22 17:38:07.723380 humanreadable-0.3.0/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2023-04-22 17:37:50.000000 humanreadable-0.3.0/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      179 2023-04-22 17:37:50.000000 humanreadable-0.3.0/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     7460 2023-04-22 17:38:07.723380 humanreadable-0.3.0/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     5940 2023-04-22 17:37:50.000000 humanreadable-0.3.0/README.rst
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-04-22 17:38:07.723380 humanreadable-0.3.0/humanreadable/
--rw-r--r--   0 toor      (1000) toor      (1000)      430 2023-04-22 17:37:50.000000 humanreadable-0.3.0/humanreadable/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-04-22 17:37:50.000000 humanreadable-0.3.0/humanreadable/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3952 2023-04-22 17:37:50.000000 humanreadable-0.3.0/humanreadable/_base.py
--rw-r--r--   0 toor      (1000) toor      (1000)     8273 2023-04-22 17:37:50.000000 humanreadable-0.3.0/humanreadable/_persec.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9298 2023-04-22 17:37:50.000000 humanreadable-0.3.0/humanreadable/_time.py
--rw-r--r--   0 toor      (1000) toor      (1000)   109604 2023-04-22 17:37:50.000000 humanreadable-0.3.0/humanreadable/_typing.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1416 2023-04-22 17:37:50.000000 humanreadable-0.3.0/humanreadable/error.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-04-22 17:37:50.000000 humanreadable-0.3.0/humanreadable/py.typed
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-04-22 17:38:07.723380 humanreadable-0.3.0/humanreadable.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     7460 2023-04-22 17:38:07.000000 humanreadable-0.3.0/humanreadable.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      546 2023-04-22 17:38:07.000000 humanreadable-0.3.0/humanreadable.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-04-22 17:38:07.000000 humanreadable-0.3.0/humanreadable.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       54 2023-04-22 17:38:07.000000 humanreadable-0.3.0/humanreadable.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       14 2023-04-22 17:38:07.000000 humanreadable-0.3.0/humanreadable.egg-info/top_level.txt
--rw-r--r--   0 toor      (1000) toor      (1000)     1230 2023-04-22 17:37:50.000000 humanreadable-0.3.0/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-04-22 17:38:07.723380 humanreadable-0.3.0/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       17 2023-04-22 17:37:50.000000 humanreadable-0.3.0/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       29 2023-04-22 17:37:50.000000 humanreadable-0.3.0/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-04-22 17:38:07.723380 humanreadable-0.3.0/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2730 2023-04-22 17:37:50.000000 humanreadable-0.3.0/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-04-22 17:38:07.723380 humanreadable-0.3.0/test/
--rw-r--r--   0 toor      (1000) toor      (1000)     9861 2023-04-22 17:37:50.000000 humanreadable-0.3.0/test/test_persec.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6658 2023-04-22 17:37:50.000000 humanreadable-0.3.0/test/test_time.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1055 2023-04-22 17:37:50.000000 humanreadable-0.3.0/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-22 15:34:12.040839 humanreadable-0.4.0/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1074 2023-07-22 15:33:43.000000 humanreadable-0.4.0/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      161 2023-07-22 15:33:43.000000 humanreadable-0.4.0/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     8106 2023-07-22 15:34:12.040839 humanreadable-0.4.0/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     6636 2023-07-22 15:33:43.000000 humanreadable-0.4.0/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-22 15:34:12.040839 humanreadable-0.4.0/humanreadable/
+-rw-r--r--   0 toor      (1000) toor      (1000)      424 2023-07-22 15:33:43.000000 humanreadable-0.4.0/humanreadable/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-07-22 15:33:43.000000 humanreadable-0.4.0/humanreadable/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3727 2023-07-22 15:33:43.000000 humanreadable-0.4.0/humanreadable/_base.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      272 2023-07-22 15:33:43.000000 humanreadable-0.4.0/humanreadable/_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      228 2023-07-22 15:33:43.000000 humanreadable-0.4.0/humanreadable/_const.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9419 2023-07-22 15:33:43.000000 humanreadable-0.4.0/humanreadable/_persec.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9246 2023-07-22 15:33:43.000000 humanreadable-0.4.0/humanreadable/_time.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      557 2023-07-22 15:33:43.000000 humanreadable-0.4.0/humanreadable/_types.py
+-rw-r--r--   0 toor      (1000) toor      (1000)   109604 2023-07-22 15:33:43.000000 humanreadable-0.4.0/humanreadable/_typing.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1416 2023-07-22 15:33:43.000000 humanreadable-0.4.0/humanreadable/error.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-07-22 15:33:43.000000 humanreadable-0.4.0/humanreadable/py.typed
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-22 15:34:12.040839 humanreadable-0.4.0/humanreadable.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     8106 2023-07-22 15:34:12.000000 humanreadable-0.4.0/humanreadable.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      619 2023-07-22 15:34:12.000000 humanreadable-0.4.0/humanreadable.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-07-22 15:34:12.000000 humanreadable-0.4.0/humanreadable.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       54 2023-07-22 15:34:12.000000 humanreadable-0.4.0/humanreadable.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       14 2023-07-22 15:34:12.000000 humanreadable-0.4.0/humanreadable.egg-info/top_level.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)     1343 2023-07-22 15:33:43.000000 humanreadable-0.4.0/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-22 15:34:12.040839 humanreadable-0.4.0/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       17 2023-07-22 15:33:43.000000 humanreadable-0.4.0/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       29 2023-07-22 15:33:43.000000 humanreadable-0.4.0/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-07-22 15:34:12.040839 humanreadable-0.4.0/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2681 2023-07-22 15:33:43.000000 humanreadable-0.4.0/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-07-22 15:34:12.040839 humanreadable-0.4.0/test/
+-rw-r--r--   0 toor      (1000) toor      (1000)    10460 2023-07-22 15:33:43.000000 humanreadable-0.4.0/test/test_persec.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6726 2023-07-22 15:33:43.000000 humanreadable-0.4.0/test/test_time.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      992 2023-07-22 15:33:43.000000 humanreadable-0.4.0/tox.ini
```

### Comparing `humanreadable-0.3.0/LICENSE` & `humanreadable-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `humanreadable-0.3.0/PKG-INFO` & `humanreadable-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: humanreadable
-Version: 0.3.0
+Version: 0.4.0
 Summary: humanreadable is a Python library to convert human-readable values to other units.
 Home-page: https://github.com/thombashi/humanreadable
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/humanreadable
 Project-URL: Tracker, https://github.com/thombashi/humanreadable/issues
 Keywords: human-readable,converter
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 .. contents:: **humanreadable**
    :backlinks: top
    :depth: 2
@@ -45,16 +44,16 @@
     :target: https://badge.fury.io/py/humanreadable
     :alt: PyPI package version
 
 .. image:: https://img.shields.io/pypi/pyversions/humanreadable.svg
    :target: https://pypi.org/project/humanreadable
     :alt: Supported Python versions
 
-.. image:: https://img.shields.io/pypi/implementation/pathvalidate.svg
-    :target: https://pypi.org/project/pathvalidate
+.. image:: https://img.shields.io/pypi/implementation/humanreadable.svg
+    :target: https://pypi.org/project/humanreadable
     :alt: Supported Python implementations
 
 .. image:: https://github.com/thombashi/humanreadable/actions/workflows/lint_and_test.yml/badge.svg
     :target: https://github.com/thombashi/humanreadable/actions/workflows/lint_and_test.yml
     :alt: CI status of Linux/macOS/Windows
 
 .. image:: https://coveralls.io/repos/github/thombashi/humanreadable/badge.svg?branch=master
@@ -76,25 +75,25 @@
 :Sample Code:
     .. code-block:: python
 
         import humanreadable as hr
 
         print("\n[Examples: humanreadable.Time]")
         value = "120 sec"
-        print("'{}' to msecs -> {}".format(value, hr.Time(value).milliseconds))
-        print("'{}' to minutes -> {}".format(value, hr.Time(value).minutes))
+        print(f"'{value}' to msecs -> {hr.Time(value).milliseconds}")
+        print(f"'{value}' to minutes -> {hr.Time(value).minutes}")
 
         value = "12 min 40 sec"
-        print("'{}' to seconds -> {}".format(value, hr.Time(value).seconds))
+        print(f"'{value}' to seconds -> {hr.Time(value).seconds}")
 
         print("\n[Examples: humanreadable.BitsPerSecond]")
         value = "1 Gbps"
-        print("'{}' to Mbps -> {}".format(value, hr.BitsPerSecond(value).mega_bps))
-        print("'{}' to Kbps -> {}".format(value, hr.BitsPerSecond(value).kilo_bps))
-        print("'{}' to Kibps -> {}".format(value, hr.BitsPerSecond(value).kibi_bps))
+        print(f"'{value}' to Mbps -> {hr.BitsPerSecond(value).mega_bps}")
+        print(f"'{value}' to Kbps -> {hr.BitsPerSecond(value).kilo_bps}")
+        print(f"'{value}' to Kibps -> {hr.BitsPerSecond(value).kibi_bps}")
 
 :Output:
     .. code-block::
 
         [Examples: humanreadable.Time]
         '120 sec' to msecs -> 120000.0
         '120 sec' to minutes -> 2.0
@@ -109,20 +108,23 @@
 Convert a value to a human readable string
 ----------------------------------------------
 :Sample Code:
     .. code-block:: python
 
         import humanreadable as hr
 
-        hr.Time("400", default_unit=hr.Time.Unit.SECOND).to_humanreadable()
+        t = hr.Time("400", default_unit=hr.Time.Unit.SECOND)
+        print(t.to_humanreadable())
+        print(t.to_humanreadable(style="short"))
 
 :Output:
     .. code-block::
 
         6 minutes 40 seconds
+        6m 40s
 
 Set default unit
 -------------------------------------------
 Unit for an instance is determined by input value.
 If a valid unit is not found, ``default_unit`` will be used for the instance (defaults to ``None``).
 
 :Sample Code:
@@ -138,53 +140,53 @@
         1.0 seconds
 
 
 Units
 -------------------------------------------
 .. table:: Available units for ``humanreadable.Time``
 
-    +------------+----------------------------------------------------------+
-    |    Unit    |                Available specifiers (str)                |
-    +============+==========================================================+
-    |days        |``d``/``day``/``days``                                    |
-    +------------+----------------------------------------------------------+
-    |hours       |``h``/``hour``/``hours``                                  |
-    +------------+----------------------------------------------------------+
-    |minutes     |``m``/``min``/``mins``/``minute``/``minutes``             |
-    +------------+----------------------------------------------------------+
-    |seconds     |``s``/``sec``/``secs``/``second``/``seconds``             |
-    +------------+----------------------------------------------------------+
-    |milliseconds|``ms``/``msec``/``msecs``/``millisecond``/``milliseconds``|
-    +------------+----------------------------------------------------------+
-    |microseconds|``us``/``usec``/``usecs``/``microsecond``/``microseconds``|
-    +------------+----------------------------------------------------------+
+    +--------------+------------------------------------------------------------+
+    |     Unit     |              Available unit specifiers (str)               |
+    +==============+============================================================+
+    | days         | ``d``/``day``/``days``                                     |
+    +--------------+------------------------------------------------------------+
+    | hours        | ``h``/``hour``/``hours``                                   |
+    +--------------+------------------------------------------------------------+
+    | minutes      | ``m``/``min``/``mins``/``minute``/``minutes``              |
+    +--------------+------------------------------------------------------------+
+    | seconds      | ``s``/``sec``/``secs``/``second``/``seconds``              |
+    +--------------+------------------------------------------------------------+
+    | milliseconds | ``ms``/``msec``/``msecs``/``millisecond``/``milliseconds`` |
+    +--------------+------------------------------------------------------------+
+    | microseconds | ``us``/``usec``/``usecs``/``microsecond``/``microseconds`` |
+    +--------------+------------------------------------------------------------+
 
 .. table:: Available units for ``humanreadable.BitsPerSecond``
 
-    +-----+-----------------------------+
-    |Unit |Available specifiers (str)   |
-    +=====+=============================+
-    |bps  |``bps``/``bits?/s``          |
-    +-----+-----------------------------+
-    |Kbps |``[kK]bps``/``[kK]bits?/s``  |
-    +-----+-----------------------------+
-    |Kibps|``[kK]ibps``/``[kK]ibits?/s``|
-    +-----+-----------------------------+
-    |Mbps |``[mM]bps``/``[mM]bits?/s``  |
-    +-----+-----------------------------+
-    |Mibps|``[mM]ibps``/``[mM]ibits?/s``|
-    +-----+-----------------------------+
-    |Gbps |``[gG]bps``/``[gG]bits?/s``  |
-    +-----+-----------------------------+
-    |Gibps|``[gG]ibps``/``[gG]ibits?/s``|
-    +-----+-----------------------------+
-    |Tbps |``[tT]bps``/``[tT]bits?/s``  |
-    +-----+-----------------------------+
-    |Tibps|``[tT]ibps``/``[tT]ibits?/s``|
-    +-----+-----------------------------+
+    +-------+--------------------------------------------------------+
+    | Unit  |            Available unit specifiers (str)             |
+    +=======+========================================================+
+    | Kbps  | ``[kK]bps``/``[kK]bits?(/|\s?per\s?)(s|sec|second)``   |
+    +-------+--------------------------------------------------------+
+    | Kibps | ``[kK]ibps``/``[kK]ibits?(/|\s?per\s?)(s|sec|second)`` |
+    +-------+--------------------------------------------------------+
+    | Mbps  | ``[mM]bps``/``[mM]bits?(/|\s?per\s?)(s|sec|second)``   |
+    +-------+--------------------------------------------------------+
+    | Mibps | ``[mM]ibps``/``[mM]ibits?(/|\s?per\s?)(s|sec|second)`` |
+    +-------+--------------------------------------------------------+
+    | Gbps  | ``[gG]bps``/``[gG]bits?(/|\s?per\s?)(s|sec|second)``   |
+    +-------+--------------------------------------------------------+
+    | Gibps | ``[gG]ibps``/``[gG]ibits?(/|\s?per\s?)(s|sec|second)`` |
+    +-------+--------------------------------------------------------+
+    | Tbps  | ``[tT]bps``/``[tT]bits?(/|\s?per\s?)(s|sec|second)``   |
+    +-------+--------------------------------------------------------+
+    | Tibps | ``[tT]ibps``/``[tT]ibits?(/|\s?per\s?)(s|sec|second)`` |
+    +-------+--------------------------------------------------------+
+    | bps   | ``bps``/``bits?(/|\s?per\s?)(s|sec|second)``           |
+    +-------+--------------------------------------------------------+
 
 
 Installation
 ============================================
 Installation: pip
 ------------------------------
 ::
@@ -198,9 +200,9 @@
     sudo add-apt-repository ppa:thombashi/ppa
     sudo apt update
     sudo apt install python3-humanreadable
 
 
 Dependencies
 ============================================
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/humanreadable/network/dependencies>`__
```

### Comparing `humanreadable-0.3.0/README.rst` & `humanreadable-0.4.0/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     :target: https://badge.fury.io/py/humanreadable
     :alt: PyPI package version
 
 .. image:: https://img.shields.io/pypi/pyversions/humanreadable.svg
    :target: https://pypi.org/project/humanreadable
     :alt: Supported Python versions
 
-.. image:: https://img.shields.io/pypi/implementation/pathvalidate.svg
-    :target: https://pypi.org/project/pathvalidate
+.. image:: https://img.shields.io/pypi/implementation/humanreadable.svg
+    :target: https://pypi.org/project/humanreadable
     :alt: Supported Python implementations
 
 .. image:: https://github.com/thombashi/humanreadable/actions/workflows/lint_and_test.yml/badge.svg
     :target: https://github.com/thombashi/humanreadable/actions/workflows/lint_and_test.yml
     :alt: CI status of Linux/macOS/Windows
 
 .. image:: https://coveralls.io/repos/github/thombashi/humanreadable/badge.svg?branch=master
@@ -42,25 +42,25 @@
 :Sample Code:
     .. code-block:: python
 
         import humanreadable as hr
 
         print("\n[Examples: humanreadable.Time]")
         value = "120 sec"
-        print("'{}' to msecs -> {}".format(value, hr.Time(value).milliseconds))
-        print("'{}' to minutes -> {}".format(value, hr.Time(value).minutes))
+        print(f"'{value}' to msecs -> {hr.Time(value).milliseconds}")
+        print(f"'{value}' to minutes -> {hr.Time(value).minutes}")
 
         value = "12 min 40 sec"
-        print("'{}' to seconds -> {}".format(value, hr.Time(value).seconds))
+        print(f"'{value}' to seconds -> {hr.Time(value).seconds}")
 
         print("\n[Examples: humanreadable.BitsPerSecond]")
         value = "1 Gbps"
-        print("'{}' to Mbps -> {}".format(value, hr.BitsPerSecond(value).mega_bps))
-        print("'{}' to Kbps -> {}".format(value, hr.BitsPerSecond(value).kilo_bps))
-        print("'{}' to Kibps -> {}".format(value, hr.BitsPerSecond(value).kibi_bps))
+        print(f"'{value}' to Mbps -> {hr.BitsPerSecond(value).mega_bps}")
+        print(f"'{value}' to Kbps -> {hr.BitsPerSecond(value).kilo_bps}")
+        print(f"'{value}' to Kibps -> {hr.BitsPerSecond(value).kibi_bps}")
 
 :Output:
     .. code-block::
 
         [Examples: humanreadable.Time]
         '120 sec' to msecs -> 120000.0
         '120 sec' to minutes -> 2.0
@@ -75,20 +75,23 @@
 Convert a value to a human readable string
 ----------------------------------------------
 :Sample Code:
     .. code-block:: python
 
         import humanreadable as hr
 
-        hr.Time("400", default_unit=hr.Time.Unit.SECOND).to_humanreadable()
+        t = hr.Time("400", default_unit=hr.Time.Unit.SECOND)
+        print(t.to_humanreadable())
+        print(t.to_humanreadable(style="short"))
 
 :Output:
     .. code-block::
 
         6 minutes 40 seconds
+        6m 40s
 
 Set default unit
 -------------------------------------------
 Unit for an instance is determined by input value.
 If a valid unit is not found, ``default_unit`` will be used for the instance (defaults to ``None``).
 
 :Sample Code:
@@ -104,53 +107,53 @@
         1.0 seconds
 
 
 Units
 -------------------------------------------
 .. table:: Available units for ``humanreadable.Time``
 
-    +------------+----------------------------------------------------------+
-    |    Unit    |                Available specifiers (str)                |
-    +============+==========================================================+
-    |days        |``d``/``day``/``days``                                    |
-    +------------+----------------------------------------------------------+
-    |hours       |``h``/``hour``/``hours``                                  |
-    +------------+----------------------------------------------------------+
-    |minutes     |``m``/``min``/``mins``/``minute``/``minutes``             |
-    +------------+----------------------------------------------------------+
-    |seconds     |``s``/``sec``/``secs``/``second``/``seconds``             |
-    +------------+----------------------------------------------------------+
-    |milliseconds|``ms``/``msec``/``msecs``/``millisecond``/``milliseconds``|
-    +------------+----------------------------------------------------------+
-    |microseconds|``us``/``usec``/``usecs``/``microsecond``/``microseconds``|
-    +------------+----------------------------------------------------------+
+    +--------------+------------------------------------------------------------+
+    |     Unit     |              Available unit specifiers (str)               |
+    +==============+============================================================+
+    | days         | ``d``/``day``/``days``                                     |
+    +--------------+------------------------------------------------------------+
+    | hours        | ``h``/``hour``/``hours``                                   |
+    +--------------+------------------------------------------------------------+
+    | minutes      | ``m``/``min``/``mins``/``minute``/``minutes``              |
+    +--------------+------------------------------------------------------------+
+    | seconds      | ``s``/``sec``/``secs``/``second``/``seconds``              |
+    +--------------+------------------------------------------------------------+
+    | milliseconds | ``ms``/``msec``/``msecs``/``millisecond``/``milliseconds`` |
+    +--------------+------------------------------------------------------------+
+    | microseconds | ``us``/``usec``/``usecs``/``microsecond``/``microseconds`` |
+    +--------------+------------------------------------------------------------+
 
 .. table:: Available units for ``humanreadable.BitsPerSecond``
 
-    +-----+-----------------------------+
-    |Unit |Available specifiers (str)   |
-    +=====+=============================+
-    |bps  |``bps``/``bits?/s``          |
-    +-----+-----------------------------+
-    |Kbps |``[kK]bps``/``[kK]bits?/s``  |
-    +-----+-----------------------------+
-    |Kibps|``[kK]ibps``/``[kK]ibits?/s``|
-    +-----+-----------------------------+
-    |Mbps |``[mM]bps``/``[mM]bits?/s``  |
-    +-----+-----------------------------+
-    |Mibps|``[mM]ibps``/``[mM]ibits?/s``|
-    +-----+-----------------------------+
-    |Gbps |``[gG]bps``/``[gG]bits?/s``  |
-    +-----+-----------------------------+
-    |Gibps|``[gG]ibps``/``[gG]ibits?/s``|
-    +-----+-----------------------------+
-    |Tbps |``[tT]bps``/``[tT]bits?/s``  |
-    +-----+-----------------------------+
-    |Tibps|``[tT]ibps``/``[tT]ibits?/s``|
-    +-----+-----------------------------+
+    +-------+--------------------------------------------------------+
+    | Unit  |            Available unit specifiers (str)             |
+    +=======+========================================================+
+    | Kbps  | ``[kK]bps``/``[kK]bits?(/|\s?per\s?)(s|sec|second)``   |
+    +-------+--------------------------------------------------------+
+    | Kibps | ``[kK]ibps``/``[kK]ibits?(/|\s?per\s?)(s|sec|second)`` |
+    +-------+--------------------------------------------------------+
+    | Mbps  | ``[mM]bps``/``[mM]bits?(/|\s?per\s?)(s|sec|second)``   |
+    +-------+--------------------------------------------------------+
+    | Mibps | ``[mM]ibps``/``[mM]ibits?(/|\s?per\s?)(s|sec|second)`` |
+    +-------+--------------------------------------------------------+
+    | Gbps  | ``[gG]bps``/``[gG]bits?(/|\s?per\s?)(s|sec|second)``   |
+    +-------+--------------------------------------------------------+
+    | Gibps | ``[gG]ibps``/``[gG]ibits?(/|\s?per\s?)(s|sec|second)`` |
+    +-------+--------------------------------------------------------+
+    | Tbps  | ``[tT]bps``/``[tT]bits?(/|\s?per\s?)(s|sec|second)``   |
+    +-------+--------------------------------------------------------+
+    | Tibps | ``[tT]ibps``/``[tT]ibits?(/|\s?per\s?)(s|sec|second)`` |
+    +-------+--------------------------------------------------------+
+    | bps   | ``bps``/``bits?(/|\s?per\s?)(s|sec|second)``           |
+    +-------+--------------------------------------------------------+
 
 
 Installation
 ============================================
 Installation: pip
 ------------------------------
 ::
@@ -164,9 +167,9 @@
     sudo add-apt-repository ppa:thombashi/ppa
     sudo apt update
     sudo apt install python3-humanreadable
 
 
 Dependencies
 ============================================
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/humanreadable/network/dependencies>`__
```

### Comparing `humanreadable-0.3.0/humanreadable/_base.py` & `humanreadable-0.4.0/humanreadable/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,27 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 import abc
 import re
 from decimal import Decimal
-from typing import Dict, List, Optional, Pattern, Tuple, Union, cast
+from typing import List, Optional, Pattern, Tuple, Union, cast
 
 from typepy import RealNumber, String
 
+from ._types import SupportsUnit, TextUnitsMap
 from .error import ParameterError, UnitNotFoundError
 
 
 try:
-    from typing import Final, Protocol
+    from typing import Final
 except ImportError:
     # typing.Final and typing.Protocol are only available starting from Python 3.8.
-    from ._typing import Final, Protocol  # type: ignore
-
-
-class SupportsUnit(Protocol):
-    @property
-    def name(self) -> str:  # pragma: no cover
-        ...
-
-    @property
-    def regexp(self) -> Pattern:  # pragma: no cover
-        ...
-
-
-Units = List[str]
-TextUnitsMap = Dict[SupportsUnit, Units]
+    from ._typing import Final  # type: ignore
 
 
 _RE_NUMBER: Final[Pattern] = re.compile(r"^[-\+]?[0-9\.]+$")
 
 
 def _get_unit_msg(text_units: TextUnitsMap) -> str:
     return ", ".join([", ".join(values) for values in text_units.values()])
```

### Comparing `humanreadable-0.3.0/humanreadable/_persec.py` & `humanreadable-0.4.0/humanreadable/_persec.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,124 +1,125 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-import re
 from collections import OrderedDict
+from dataclasses import dataclass
 from decimal import Decimal
 from typing import Dict, List, NamedTuple, Optional, Pattern, Union, cast
 
-from ._base import HumanReadableValue, SupportsUnit, TextUnitsMap
-
-
-_PATTERN_TEMPLETE = r"\s?{}$"
-_BPS_PATTERN = r"bits?(/|\s?per\s?)(s|sec|second)"
-
-_BPS_STR_UNITS = ["bps", _BPS_PATTERN]
-_KBPS_STR_UNITS = ["[kK]bps", "[kK]" + _BPS_PATTERN]
-_KIBPS_STR_UNITS = ["[kK]ibps", "[kK]i" + _BPS_PATTERN]
-_MBPS_STR_UNITS = ["[mM]bps", "[mM]" + _BPS_PATTERN]
-_MIBPS_STR_UNITS = ["[mM]ibps", "[mM]i" + _BPS_PATTERN]
-_GBPS_STR_UNITS = ["[gG]bps", "[gG]" + _BPS_PATTERN]
-_GIBPS_STR_UNITS = ["[gG]ibps", "[gG]i" + _BPS_PATTERN]
-_TBPS_STR_UNITS = ["[tT]bps", "[tT]" + _BPS_PATTERN]
-_TIBPS_STR_UNITS = ["[tT]ibps", "[tT]i" + _BPS_PATTERN]
+from ._base import HumanReadableValue
+from ._common import compile_units_regex_pattern
+from ._types import HumanReadableStyle, SupportsUnit, TextUnitsMap, Units
+
+
+try:
+    from typing import Final
+except ImportError:
+    # typing.Final and typing.Protocol are only available starting from Python 3.8.
+    from ._typing import Final  # type: ignore
+
+
+_BPS_PATTERN: Final[str] = r"bits?(/|\s?per\s?)(s|sec|second)"
+
+_BPS_STR_UNITS: Final[Units] = ("bps", _BPS_PATTERN)
+_KBPS_STR_UNITS: Final[Units] = ("[kK]bps", "[kK]" + _BPS_PATTERN)
+_KIBPS_STR_UNITS: Final[Units] = ("[kK]ibps", "[kK]i" + _BPS_PATTERN)
+_MBPS_STR_UNITS: Final[Units] = ("[mM]bps", "[mM]" + _BPS_PATTERN)
+_MIBPS_STR_UNITS: Final[Units] = ("[mM]ibps", "[mM]i" + _BPS_PATTERN)
+_GBPS_STR_UNITS: Final[Units] = ("[gG]bps", "[gG]" + _BPS_PATTERN)
+_GIBPS_STR_UNITS: Final[Units] = ("[gG]ibps", "[gG]i" + _BPS_PATTERN)
+_TBPS_STR_UNITS: Final[Units] = ("[tT]bps", "[tT]" + _BPS_PATTERN)
+_TIBPS_STR_UNITS: Final[Units] = ("[tT]ibps", "[tT]i" + _BPS_PATTERN)
 
 
 class ByteUnit(NamedTuple):
     name: str
-    regexp: Pattern
-    kilo_size: int
+    regexp: Pattern[str]
+    k_size: int
     factor: int
+    full_unit_expr: str
 
 
-class BitPerSecond(HumanReadableValue):
+class BitsPerSecond(HumanReadableValue):
     """
     String converter that human-readable byte size to a number.
 
     Args:
         readable_value (str):
             Human readable size (bit per second). e.g. 256 Mbps
     """
 
+    @dataclass(frozen=True)
     class Unit:
         BPS = ByteUnit(
             name="bps",
-            regexp=re.compile(
-                "|".join([_PATTERN_TEMPLETE.format(unit) for unit in _BPS_STR_UNITS])
-            ),
-            kilo_size=1000,
+            regexp=compile_units_regex_pattern(_BPS_STR_UNITS),
+            k_size=1000,
             factor=0,
+            full_unit_expr="bits per second",
         )
         KBPS = ByteUnit(
             name="Kbps",
-            regexp=re.compile(
-                "|".join([_PATTERN_TEMPLETE.format(unit) for unit in _KBPS_STR_UNITS])
-            ),
-            kilo_size=1000,
+            regexp=compile_units_regex_pattern(_KBPS_STR_UNITS),
+            k_size=1000,
             factor=1,
+            full_unit_expr="kilobits per second",
         )
         KIBPS = ByteUnit(
             name="Kibps",
-            regexp=re.compile(
-                "|".join([_PATTERN_TEMPLETE.format(unit) for unit in _KIBPS_STR_UNITS])
-            ),
-            kilo_size=1024,
+            regexp=compile_units_regex_pattern(_KIBPS_STR_UNITS),
+            k_size=1024,
             factor=1,
+            full_unit_expr="kibibits per second",
         )
         MBPS = ByteUnit(
             name="Mbps",
-            regexp=re.compile(
-                "|".join([_PATTERN_TEMPLETE.format(unit) for unit in _MBPS_STR_UNITS])
-            ),
-            kilo_size=1000,
+            regexp=compile_units_regex_pattern(_MBPS_STR_UNITS),
+            k_size=1000,
             factor=2,
+            full_unit_expr="megabits per second",
         )
         MIBPS = ByteUnit(
             name="Mibps",
-            regexp=re.compile(
-                "|".join([_PATTERN_TEMPLETE.format(unit) for unit in _MIBPS_STR_UNITS])
-            ),
-            kilo_size=1024,
+            regexp=compile_units_regex_pattern(_MIBPS_STR_UNITS),
+            k_size=1024,
             factor=2,
+            full_unit_expr="mebibits per second",
         )
         GBPS = ByteUnit(
             name="Gbps",
-            regexp=re.compile(
-                "|".join([_PATTERN_TEMPLETE.format(unit) for unit in _GBPS_STR_UNITS])
-            ),
-            kilo_size=1000,
+            regexp=compile_units_regex_pattern(_GBPS_STR_UNITS),
+            k_size=1000,
             factor=3,
+            full_unit_expr="gigabits per second",
         )
         GIBPS = ByteUnit(
             name="Gibps",
-            regexp=re.compile(
-                "|".join([_PATTERN_TEMPLETE.format(unit) for unit in _GIBPS_STR_UNITS])
-            ),
-            kilo_size=1024,
+            regexp=compile_units_regex_pattern(_GIBPS_STR_UNITS),
+            k_size=1024,
             factor=3,
+            full_unit_expr="gibibits per second",
         )
         TBPS = ByteUnit(
             name="Tbps",
-            regexp=re.compile(
-                "|".join([_PATTERN_TEMPLETE.format(unit) for unit in _TBPS_STR_UNITS])
-            ),
-            kilo_size=1000,
+            regexp=compile_units_regex_pattern(_TBPS_STR_UNITS),
+            k_size=1000,
             factor=4,
+            full_unit_expr="terabits per second",
         )
         TIBPS = ByteUnit(
             name="Tibps",
-            regexp=re.compile(
-                "|".join([_PATTERN_TEMPLETE.format(unit) for unit in _TIBPS_STR_UNITS])
-            ),
-            kilo_size=1024,
+            regexp=compile_units_regex_pattern(_TIBPS_STR_UNITS),
+            k_size=1024,
             factor=4,
+            full_unit_expr="tebibits per second",
         )
 
-    _TEXT_UNITS: TextUnitsMap = OrderedDict(
+    _TEXT_UNITS: Final[TextUnitsMap] = OrderedDict(
         {
             Unit.KBPS: _KBPS_STR_UNITS,
             Unit.KIBPS: _KIBPS_STR_UNITS,
             Unit.MBPS: _MBPS_STR_UNITS,
             Unit.MIBPS: _MIBPS_STR_UNITS,
             Unit.GBPS: _GBPS_STR_UNITS,
             Unit.GIBPS: _GIBPS_STR_UNITS,
@@ -236,17 +237,17 @@
 
     def __gt__(self, other) -> bool:
         return self.bps > other.bps
 
     def __ge__(self, other) -> bool:
         return self.bps >= other.bps
 
-    def __add__(self, other: "BitPerSecond") -> "BitPerSecond":
+    def __add__(self, other: "BitsPerSecond") -> "BitsPerSecond":
         number = self._number + Decimal(other.get_as(self._from_unit))
-        return BitPerSecond(str(number), default_unit=self._from_unit)
+        return BitsPerSecond(str(number), default_unit=self._from_unit)
 
     def get_as(self, unit: Union[str, SupportsUnit]) -> float:
         unit_maps: Dict[SupportsUnit, str] = {
             self.Unit.BPS: "bps",
             self.Unit.KBPS: "kilo_bps",
             self.Unit.KIBPS: "kibi_bps",
             self.Unit.MBPS: "mega_bps",
@@ -265,16 +266,39 @@
         if isinstance(unit, ByteUnit):
             return unit
 
         return super()._normalize_unit(unit)
 
     def __calc_coef(self, from_unit: SupportsUnit, to_unit: ByteUnit) -> Decimal:
         from_unit_bu = cast(ByteUnit, from_unit)
-        if from_unit_bu.kilo_size == to_unit.kilo_size:
-            return Decimal(from_unit_bu.kilo_size ** (from_unit_bu.factor - to_unit.factor))
+        if from_unit_bu.k_size == to_unit.k_size:
+            return Decimal(from_unit_bu.k_size ** (from_unit_bu.factor - to_unit.factor))
 
-        return Decimal(from_unit_bu.kilo_size**from_unit_bu.factor) / Decimal(
-            to_unit.kilo_size**to_unit.factor
+        return Decimal(from_unit_bu.k_size**from_unit_bu.factor) / Decimal(
+            to_unit.k_size**to_unit.factor
         )
 
+    def __filter_units_by_k(
+        self, units: List[SupportsUnit], from_unit: SupportsUnit
+    ) -> List[SupportsUnit]:
+        from_unit_bu = cast(ByteUnit, from_unit)
+        return [u for u in units if cast(ByteUnit, u).k_size == from_unit_bu.k_size]
+
+    def to_humanreadable(self, style: HumanReadableStyle = "full") -> str:
+        def _to_unit_str(unit, style: str) -> str:
+            if style == "full":
+                return f" {unit.full_unit_expr}"
+
+            return f" {unit.name}"
+
+        filtered_units = self.__filter_units_by_k(self._units, self._from_unit)
+        for unit in reversed(sorted(filtered_units, key=lambda u: cast(ByteUnit, u).factor)):
+            number = self.get_as(unit)
+            if number < 1:
+                continue
+
+            return f"{number:.1f}{_to_unit_str(unit, style)}"
+
+        raise ValueError("unit not found")
+
 
-BitsPerSecond = BitPerSecond
+BitPerSecond = BitsPerSecond
```

### Comparing `humanreadable-0.3.0/humanreadable/_time.py` & `humanreadable-0.4.0/humanreadable/_time.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,100 +1,93 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 import re
 from collections import OrderedDict
+from dataclasses import dataclass
 from decimal import Decimal
 from typing import Dict, List, NamedTuple, Optional, Pattern, Union, cast
 
-from ._base import HumanReadableValue, SupportsUnit, TextUnitsMap
+from ._base import HumanReadableValue
+from ._common import compile_units_regex_pattern
+from ._types import HumanReadableStyle, SupportsUnit, TextUnitsMap, Units
 from .error import ParameterError
 
 
-_PATTERN_TEMPLETE = r"\s?{}$"
+try:
+    from typing import Final
+except ImportError:
+    # typing.Final and typing.Protocol are only available starting from Python 3.8.
+    from ._typing import Final  # type: ignore
 
-_DAY_STR_UNITS = ["d", "day", "days"]
-_HOUR_STR_UNITS = ["h", "hour", "hours"]
-_MINUTE_STR_UNITS = ["m", "min", "mins", "minute", "minutes"]
-_SEC_STR_UNITS = ["s", "sec", "secs", "second", "seconds"]
-_MSEC_STR_UNITS = ["ms", "msec", "msecs", "millisecond", "milliseconds"]
-_USEC_STR_UNITS = ["us", "usec", "usecs", "microsecond", "microseconds"]
+
+_DAY_STR_UNITS: Final[Units] = ("d", "day", "days")
+_HOUR_STR_UNITS: Final[Units] = ("h", "hour", "hours")
+_MINUTE_STR_UNITS: Final[Units] = ("m", "min", "mins", "minute", "minutes")
+_SEC_STR_UNITS: Final[Units] = ("s", "sec", "secs", "second", "seconds")
+_MSEC_STR_UNITS: Final[Units] = ("ms", "msec", "msecs", "millisecond", "milliseconds")
+_USEC_STR_UNITS: Final[Units] = ("us", "usec", "usecs", "microsecond", "microseconds")
 
 
 class TimeUnit(NamedTuple):
     name: str
-    regexp: Pattern
+    regexp: Pattern[str]
     thousand_factor: int
     sixty_factor: int
     day_factor: int
 
 
 class Time(HumanReadableValue):
+    @dataclass(frozen=True)
     class Unit:
         DAY = TimeUnit(
             name="days",
-            regexp=re.compile(
-                "|".join([_PATTERN_TEMPLETE.format(unit) for unit in _DAY_STR_UNITS]), re.IGNORECASE
-            ),
+            regexp=compile_units_regex_pattern(_DAY_STR_UNITS, re.IGNORECASE),
             thousand_factor=0,
             sixty_factor=0,
             day_factor=0,
         )
         HOUR = TimeUnit(
             name="hours",
-            regexp=re.compile(
-                "|".join([_PATTERN_TEMPLETE.format(unit) for unit in _HOUR_STR_UNITS]),
-                re.IGNORECASE,
-            ),
+            regexp=compile_units_regex_pattern(_HOUR_STR_UNITS, re.IGNORECASE),
             thousand_factor=0,
             sixty_factor=0,
             day_factor=1,
         )
         MINUTE = TimeUnit(
             name="minutes",
-            regexp=re.compile(
-                "|".join([_PATTERN_TEMPLETE.format(unit) for unit in _MINUTE_STR_UNITS]),
-                re.IGNORECASE,
-            ),
+            regexp=compile_units_regex_pattern(_MINUTE_STR_UNITS, re.IGNORECASE),
             thousand_factor=0,
             sixty_factor=1,
             day_factor=1,
         )
         SECOND = TimeUnit(
             name="seconds",
-            regexp=re.compile(
-                "|".join([_PATTERN_TEMPLETE.format(unit) for unit in _SEC_STR_UNITS]), re.IGNORECASE
-            ),
+            regexp=compile_units_regex_pattern(_SEC_STR_UNITS, re.IGNORECASE),
             thousand_factor=0,
             sixty_factor=2,
             day_factor=1,
         )
         MILLISECOND = TimeUnit(
             name="milliseconds",
-            regexp=re.compile(
-                "|".join([_PATTERN_TEMPLETE.format(unit) for unit in _MSEC_STR_UNITS]),
-                re.IGNORECASE,
-            ),
+            regexp=compile_units_regex_pattern(_MSEC_STR_UNITS, re.IGNORECASE),
             thousand_factor=1,
             sixty_factor=2,
             day_factor=1,
         )
         MICROSECOND = TimeUnit(
             name="microseconds",
-            regexp=re.compile(
-                "|".join([_PATTERN_TEMPLETE.format(unit) for unit in _USEC_STR_UNITS]),
-                re.IGNORECASE,
-            ),
+            regexp=compile_units_regex_pattern(_USEC_STR_UNITS, re.IGNORECASE),
             thousand_factor=2,
             sixty_factor=2,
             day_factor=1,
         )
 
-    _TEXT_UNITS: TextUnitsMap = OrderedDict(
+    _TEXT_UNITS: Final[TextUnitsMap] = OrderedDict(
         {
             Unit.DAY: _DAY_STR_UNITS,
             Unit.HOUR: _HOUR_STR_UNITS,
             Unit.MINUTE: _MINUTE_STR_UNITS,
             Unit.SECOND: _SEC_STR_UNITS,
             Unit.MILLISECOND: _MSEC_STR_UNITS,
             Unit.MICROSECOND: _USEC_STR_UNITS,
@@ -177,15 +170,15 @@
     def __ge__(self, other) -> bool:
         return self.microseconds >= other.microseconds
 
     def __add__(self, other: "Time") -> "Time":
         number = self._number + Decimal(other.get_as(self._from_unit))
         return Time(str(number), default_unit=self._from_unit)
 
-    def validate(self, min_value=None, max_value=None):
+    def validate(self, min_value=None, max_value=None) -> None:
         if min_value is not None:
             if not isinstance(min_value, Time):
                 min_value = Time(min_value)
 
             if self < min_value:
                 raise ParameterError(
                     "time value is too low",
@@ -214,29 +207,28 @@
             self.Unit.MICROSECOND: "microseconds",
         }
         norm_unit = self._normalize_unit(unit)
         assert norm_unit
 
         return getattr(self, unit_maps[norm_unit])
 
-    def to_humanreadable(self, style: str = "full") -> str:
-        def _to_unit_str(unit, style: str) -> str:
+    def to_humanreadable(self, style: HumanReadableStyle = "full") -> str:
+        def _to_unit_str(unit: SupportsUnit, style: str) -> str:
             if style in ("short", "abbr"):
                 return unit.name[0]
 
             if style == "full":
                 return f" {unit.name}"
 
             return unit.name
 
-        style = style.strip().lower()
-        items = []
+        items: List[str] = []
 
         if self.days >= 1:
-            items.append(f"{self.days:d}{_to_unit_str(self.Unit.DAY, style)}")
+            items.append(f"{int(self.days):d}{_to_unit_str(self.Unit.DAY, style)}")
         if self.hours % 24 >= 1:
             items.append(f"{int(self.hours) % 24:d}{_to_unit_str(self.Unit.HOUR, style)}")
         if self.minutes % 60 >= 1:
             items.append(f"{int(self.minutes) % 60:d}{_to_unit_str(self.Unit.MINUTE, style)}")
         if self.seconds % 60 >= 1:
             items.append(f"{int(self.seconds) % 60:d}{_to_unit_str(self.Unit.SECOND, style)}")
         if self.milliseconds % 1000 >= 1:
```

### Comparing `humanreadable-0.3.0/humanreadable/_typing.py` & `humanreadable-0.4.0/humanreadable/_typing.py`

 * *Files identical despite different names*

### Comparing `humanreadable-0.3.0/humanreadable/error.py` & `humanreadable-0.4.0/humanreadable/error.py`

 * *Files identical despite different names*

### Comparing `humanreadable-0.3.0/humanreadable.egg-info/PKG-INFO` & `humanreadable-0.4.0/humanreadable.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: humanreadable
-Version: 0.3.0
+Version: 0.4.0
 Summary: humanreadable is a Python library to convert human-readable values to other units.
 Home-page: https://github.com/thombashi/humanreadable
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/humanreadable
 Project-URL: Tracker, https://github.com/thombashi/humanreadable/issues
 Keywords: human-readable,converter
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 .. contents:: **humanreadable**
    :backlinks: top
    :depth: 2
@@ -45,16 +44,16 @@
     :target: https://badge.fury.io/py/humanreadable
     :alt: PyPI package version
 
 .. image:: https://img.shields.io/pypi/pyversions/humanreadable.svg
    :target: https://pypi.org/project/humanreadable
     :alt: Supported Python versions
 
-.. image:: https://img.shields.io/pypi/implementation/pathvalidate.svg
-    :target: https://pypi.org/project/pathvalidate
+.. image:: https://img.shields.io/pypi/implementation/humanreadable.svg
+    :target: https://pypi.org/project/humanreadable
     :alt: Supported Python implementations
 
 .. image:: https://github.com/thombashi/humanreadable/actions/workflows/lint_and_test.yml/badge.svg
     :target: https://github.com/thombashi/humanreadable/actions/workflows/lint_and_test.yml
     :alt: CI status of Linux/macOS/Windows
 
 .. image:: https://coveralls.io/repos/github/thombashi/humanreadable/badge.svg?branch=master
@@ -76,25 +75,25 @@
 :Sample Code:
     .. code-block:: python
 
         import humanreadable as hr
 
         print("\n[Examples: humanreadable.Time]")
         value = "120 sec"
-        print("'{}' to msecs -> {}".format(value, hr.Time(value).milliseconds))
-        print("'{}' to minutes -> {}".format(value, hr.Time(value).minutes))
+        print(f"'{value}' to msecs -> {hr.Time(value).milliseconds}")
+        print(f"'{value}' to minutes -> {hr.Time(value).minutes}")
 
         value = "12 min 40 sec"
-        print("'{}' to seconds -> {}".format(value, hr.Time(value).seconds))
+        print(f"'{value}' to seconds -> {hr.Time(value).seconds}")
 
         print("\n[Examples: humanreadable.BitsPerSecond]")
         value = "1 Gbps"
-        print("'{}' to Mbps -> {}".format(value, hr.BitsPerSecond(value).mega_bps))
-        print("'{}' to Kbps -> {}".format(value, hr.BitsPerSecond(value).kilo_bps))
-        print("'{}' to Kibps -> {}".format(value, hr.BitsPerSecond(value).kibi_bps))
+        print(f"'{value}' to Mbps -> {hr.BitsPerSecond(value).mega_bps}")
+        print(f"'{value}' to Kbps -> {hr.BitsPerSecond(value).kilo_bps}")
+        print(f"'{value}' to Kibps -> {hr.BitsPerSecond(value).kibi_bps}")
 
 :Output:
     .. code-block::
 
         [Examples: humanreadable.Time]
         '120 sec' to msecs -> 120000.0
         '120 sec' to minutes -> 2.0
@@ -109,20 +108,23 @@
 Convert a value to a human readable string
 ----------------------------------------------
 :Sample Code:
     .. code-block:: python
 
         import humanreadable as hr
 
-        hr.Time("400", default_unit=hr.Time.Unit.SECOND).to_humanreadable()
+        t = hr.Time("400", default_unit=hr.Time.Unit.SECOND)
+        print(t.to_humanreadable())
+        print(t.to_humanreadable(style="short"))
 
 :Output:
     .. code-block::
 
         6 minutes 40 seconds
+        6m 40s
 
 Set default unit
 -------------------------------------------
 Unit for an instance is determined by input value.
 If a valid unit is not found, ``default_unit`` will be used for the instance (defaults to ``None``).
 
 :Sample Code:
@@ -138,53 +140,53 @@
         1.0 seconds
 
 
 Units
 -------------------------------------------
 .. table:: Available units for ``humanreadable.Time``
 
-    +------------+----------------------------------------------------------+
-    |    Unit    |                Available specifiers (str)                |
-    +============+==========================================================+
-    |days        |``d``/``day``/``days``                                    |
-    +------------+----------------------------------------------------------+
-    |hours       |``h``/``hour``/``hours``                                  |
-    +------------+----------------------------------------------------------+
-    |minutes     |``m``/``min``/``mins``/``minute``/``minutes``             |
-    +------------+----------------------------------------------------------+
-    |seconds     |``s``/``sec``/``secs``/``second``/``seconds``             |
-    +------------+----------------------------------------------------------+
-    |milliseconds|``ms``/``msec``/``msecs``/``millisecond``/``milliseconds``|
-    +------------+----------------------------------------------------------+
-    |microseconds|``us``/``usec``/``usecs``/``microsecond``/``microseconds``|
-    +------------+----------------------------------------------------------+
+    +--------------+------------------------------------------------------------+
+    |     Unit     |              Available unit specifiers (str)               |
+    +==============+============================================================+
+    | days         | ``d``/``day``/``days``                                     |
+    +--------------+------------------------------------------------------------+
+    | hours        | ``h``/``hour``/``hours``                                   |
+    +--------------+------------------------------------------------------------+
+    | minutes      | ``m``/``min``/``mins``/``minute``/``minutes``              |
+    +--------------+------------------------------------------------------------+
+    | seconds      | ``s``/``sec``/``secs``/``second``/``seconds``              |
+    +--------------+------------------------------------------------------------+
+    | milliseconds | ``ms``/``msec``/``msecs``/``millisecond``/``milliseconds`` |
+    +--------------+------------------------------------------------------------+
+    | microseconds | ``us``/``usec``/``usecs``/``microsecond``/``microseconds`` |
+    +--------------+------------------------------------------------------------+
 
 .. table:: Available units for ``humanreadable.BitsPerSecond``
 
-    +-----+-----------------------------+
-    |Unit |Available specifiers (str)   |
-    +=====+=============================+
-    |bps  |``bps``/``bits?/s``          |
-    +-----+-----------------------------+
-    |Kbps |``[kK]bps``/``[kK]bits?/s``  |
-    +-----+-----------------------------+
-    |Kibps|``[kK]ibps``/``[kK]ibits?/s``|
-    +-----+-----------------------------+
-    |Mbps |``[mM]bps``/``[mM]bits?/s``  |
-    +-----+-----------------------------+
-    |Mibps|``[mM]ibps``/``[mM]ibits?/s``|
-    +-----+-----------------------------+
-    |Gbps |``[gG]bps``/``[gG]bits?/s``  |
-    +-----+-----------------------------+
-    |Gibps|``[gG]ibps``/``[gG]ibits?/s``|
-    +-----+-----------------------------+
-    |Tbps |``[tT]bps``/``[tT]bits?/s``  |
-    +-----+-----------------------------+
-    |Tibps|``[tT]ibps``/``[tT]ibits?/s``|
-    +-----+-----------------------------+
+    +-------+--------------------------------------------------------+
+    | Unit  |            Available unit specifiers (str)             |
+    +=======+========================================================+
+    | Kbps  | ``[kK]bps``/``[kK]bits?(/|\s?per\s?)(s|sec|second)``   |
+    +-------+--------------------------------------------------------+
+    | Kibps | ``[kK]ibps``/``[kK]ibits?(/|\s?per\s?)(s|sec|second)`` |
+    +-------+--------------------------------------------------------+
+    | Mbps  | ``[mM]bps``/``[mM]bits?(/|\s?per\s?)(s|sec|second)``   |
+    +-------+--------------------------------------------------------+
+    | Mibps | ``[mM]ibps``/``[mM]ibits?(/|\s?per\s?)(s|sec|second)`` |
+    +-------+--------------------------------------------------------+
+    | Gbps  | ``[gG]bps``/``[gG]bits?(/|\s?per\s?)(s|sec|second)``   |
+    +-------+--------------------------------------------------------+
+    | Gibps | ``[gG]ibps``/``[gG]ibits?(/|\s?per\s?)(s|sec|second)`` |
+    +-------+--------------------------------------------------------+
+    | Tbps  | ``[tT]bps``/``[tT]bits?(/|\s?per\s?)(s|sec|second)``   |
+    +-------+--------------------------------------------------------+
+    | Tibps | ``[tT]ibps``/``[tT]ibits?(/|\s?per\s?)(s|sec|second)`` |
+    +-------+--------------------------------------------------------+
+    | bps   | ``bps``/``bits?(/|\s?per\s?)(s|sec|second)``           |
+    +-------+--------------------------------------------------------+
 
 
 Installation
 ============================================
 Installation: pip
 ------------------------------
 ::
@@ -198,9 +200,9 @@
     sudo add-apt-repository ppa:thombashi/ppa
     sudo apt update
     sudo apt install python3-humanreadable
 
 
 Dependencies
 ============================================
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/humanreadable/network/dependencies>`__
```

### Comparing `humanreadable-0.3.0/humanreadable.egg-info/SOURCES.txt` & `humanreadable-0.4.0/humanreadable.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 README.rst
 pyproject.toml
 setup.py
 tox.ini
 humanreadable/__init__.py
 humanreadable/__version__.py
 humanreadable/_base.py
+humanreadable/_common.py
+humanreadable/_const.py
 humanreadable/_persec.py
 humanreadable/_time.py
+humanreadable/_types.py
 humanreadable/_typing.py
 humanreadable/error.py
 humanreadable/py.typed
 humanreadable.egg-info/PKG-INFO
 humanreadable.egg-info/SOURCES.txt
 humanreadable.egg-info/dependency_links.txt
 humanreadable.egg-info/requires.txt
```

### Comparing `humanreadable-0.3.0/pyproject.toml` & `humanreadable-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 100
 exclude = '''
 /(
       \.eggs
     | \.git
@@ -15,15 +16,15 @@
     | buck-out
     | build
     | dist
 )/
 | docs/conf.py
 | humanreadable/_typing.py
 '''
-target-version = ['py36', 'py37', 'py38', 'py39', 'py310', 'py311']
+target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 
 [tool.coverage.run]
 source = ['humanreadable']
 branch = true
 
 [tool.coverage.report]
 show_missing = true
@@ -58,16 +59,20 @@
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
 python_version = 3.8
 
 pretty = true
+
+no_implicit_optional = true
 show_error_codes = true
 show_error_context = true
+warn_redundant_casts = true
 warn_unreachable = true
 warn_unused_configs = true
+warn_unused_ignores = true
 
 [tool.pytest.ini_options]
 md_report = true
 md_report_verbose = 0
 md_report_color = "auto"
```

### Comparing `humanreadable-0.3.0/setup.py` & `humanreadable-0.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,25 +50,24 @@
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(exclude=["test*"]),
     package_data={MODULE_NAME: ["py.typed"]},
     project_urls={
         "Source": REPOSITORY_URL,
         "Tracker": f"{REPOSITORY_URL:s}/issues",
     },
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=INSTALL_REQUIRES,
     extras_require={"test": TESTS_REQUIRES},
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `humanreadable-0.3.0/test/test_persec.py` & `humanreadable-0.4.0/test/test_persec.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 """
 
 import sys
 from decimal import Decimal
 
 import pytest
 
-from humanreadable import BitPerSecond, BitsPerSecond, ParameterError, UnitNotFoundError
+from humanreadable import BitsPerSecond, ParameterError, UnitNotFoundError
 
 
 KILO = Decimal(1000**1)
 MEGA = Decimal(1000**2)
 GIGA = Decimal(1000**3)
 TERA = Decimal(1000**4)
 KIBI = Decimal(1024**1)
 MEBI = Decimal(1024**2)
 GIBI = Decimal(1024**3)
 TEBI = Decimal(1024**4)
 
 
-class Test_BitPerSecond_constructor:
+class Test_BitsPerSecond_constructor:
     @pytest.mark.parametrize(
         ["value", "exception"],
         [
             ["10", UnitNotFoundError],
             [None, TypeError],
             [True, TypeError],
             [float("nan"), TypeError],
@@ -36,74 +36,74 @@
             ["2m", ParameterError],
             ["2ms", ParameterError],
             ["two Gbps", ParameterError],
         ],
     )
     def test_exception(self, value, exception):
         with pytest.raises(exception):
-            BitPerSecond(value).bps
+            BitsPerSecond(value).bps
 
 
-class Test_BitPerSecond_repr:
+class Test_BitsPerSecond_repr:
     @pytest.mark.parametrize(
         ["value", "expected"],
         [
             ["2 Kbps", "2 Kbps"],
         ],
     )
     def test_exception(self, value, expected):
-        assert str(BitPerSecond(value)) == expected
+        assert str(BitsPerSecond(value)) == expected
 
 
-class Test_BitPerSecond_eq:
+class Test_BitsPerSecond_eq:
     @pytest.mark.parametrize(
         ["lhs", "rhs", "expected"],
         [
             ["5 bps", "5.0 bit/s", True],
             ["5.0 bit/s", "5 bits/sec", True],
             ["60000bps", "60 Kbps", True],
             ["1 bps", "2 bps", False],
         ],
     )
     def test_exception(self, lhs, rhs, expected):
-        assert (BitPerSecond(lhs) == BitPerSecond(rhs)) is expected
-        assert (BitPerSecond(lhs) == BitsPerSecond(rhs)) is expected
+        assert (BitsPerSecond(lhs) == BitsPerSecond(rhs)) is expected
+        assert (BitsPerSecond(lhs) == BitsPerSecond(rhs)) is expected
 
 
-class Test_BitPerSecond_add:
+class Test_BitsPerSecond_add:
     @pytest.mark.parametrize(
         ["lhs", "rhs", "expected"],
         [
             ["1Kbps", "1 Kbits/sec", "2 Kbps"],
         ],
     )
     def test_exception(self, lhs, rhs, expected):
-        assert (BitPerSecond(lhs) + BitPerSecond(rhs)) == BitPerSecond(expected)
+        assert (BitsPerSecond(lhs) + BitsPerSecond(rhs)) == BitsPerSecond(expected)
 
 
-class Test_BitPerSecond_less_than:
+class Test_BitsPerSecond_less_than:
     @pytest.mark.parametrize(
         ["lhs", "rhs", "expected"],
         [
             ["20 Gbps", "32Gbps", True],
             ["20 Gibps", "32Gbps", True],
             ["40 Gibps", "32Gbps", False],
         ],
     )
     def test_exception(self, lhs, rhs, expected):
-        lhs = BitPerSecond(lhs)
-        rhs = BitPerSecond(rhs)
+        lhs = BitsPerSecond(lhs)
+        rhs = BitsPerSecond(rhs)
 
         print(f"lhs={lhs.mega_bps}Mbps, rhs={rhs.mega_bps}Mbps", file=sys.stderr)
 
         assert (lhs < rhs) is expected
         assert (lhs <= rhs) is expected
 
 
-class Test_BitPerSecond_bps:
+class Test_BitsPerSecond_bps:
     @pytest.mark.parametrize(
         ["value", "expected"],
         [
             ["2bps", 2],
             ["2 bps", 2],
             ["2kbps", 2 * 1000**1],
             ["2 Kbps", 2 * 1000**1],
@@ -117,20 +117,20 @@
             ["2.5 Gibit/s", 2.5 * 1024**3],
             ["2Tbps", 2 * 1000**4],
             ["2 Tbps", 2 * 1000**4],
             ["2.5 Tibit/s", 2.5 * 1024**4],
         ],
     )
     def test_normal(self, value, expected):
-        value = BitPerSecond(value)
+        value = BitsPerSecond(value)
         assert value.bps == expected
         assert value.byte_per_sec == value.bps / 8
 
 
-class Test_BitPerSecond_kbps:
+class Test_BitsPerSecond_kbps:
     @pytest.mark.parametrize(
         ["value", "expected"],
         [
             ["2bps", 2 * 1000**-1],
             ["2Kbps", 2 * 1000**0],
             ["2Mbps", 2 * 1000**1],
             ["2Gbps", 2 * 1000**2],
@@ -138,15 +138,15 @@
             ["2Kibps", 2 * KIBI / KILO],
             ["2Mibps", 2 * MEBI / KILO],
             ["2Gibps", 2 * GIBI / KILO],
             ["2Tibps", 2 * TEBI / KILO],
         ],
     )
     def test_normal_kilo(self, value, expected):
-        value = BitPerSecond(value)
+        value = BitsPerSecond(value)
         assert value.kilo_bps == float(expected)
         assert value.kilo_byte_per_sec == value.kilo_bps / 8
 
     @pytest.mark.parametrize(
         ["value", "expected"],
         [
             ["2Kbps", 2 * KILO / KIBI],
@@ -156,35 +156,35 @@
             ["2Kibps", 2 * 1024**0],
             ["2Mibps", 2 * 1024**1],
             ["2Gibps", 2 * 1024**2],
             ["2Tibps", 2 * 1024**3],
         ],
     )
     def test_normal_kibi(self, value, expected):
-        value = BitPerSecond(value)
+        value = BitsPerSecond(value)
         assert value.kibi_bps == expected
         assert value.kibi_byte_per_sec == value.kibi_bps / 8
 
     @pytest.mark.parametrize(
         ["value", "default_unit", "expected"],
         [
-            ["2", BitPerSecond.Unit.KBPS, 2],
+            ["2", BitsPerSecond.Unit.KBPS, 2],
             ["2", "kbps", 2],
-            ["2", BitPerSecond.Unit.MBPS, 2000],
+            ["2", BitsPerSecond.Unit.MBPS, 2000],
             ["2", "mbps", 2000],
         ],
     )
     def test_normal_default_unit(self, value, default_unit, expected):
-        bps = BitPerSecond(value, default_unit=default_unit)
+        bps = BitsPerSecond(value, default_unit=default_unit)
         print(bps, file=sys.stderr)
 
         assert bps.kilo_bps == expected
 
 
-class Test_BitPerSecond_mbps:
+class Test_BitsPerSecond_mbps:
     @pytest.mark.parametrize(
         ["value", "expected"],
         [
             ["2bps", 2 * 1000**-2],
             ["2Kbps", 2 * 1000**-1],
             ["2Mbps", 2 * 1000**0],
             ["2Gbps", 2 * 1000**1],
@@ -192,15 +192,15 @@
             ["2Kibps", 2 * KIBI / MEGA],
             ["2Mibps", 2 * MEBI / MEGA],
             ["2Gibps", 2 * GIBI / MEGA],
             ["2Tibps", 2 * TEBI / MEGA],
         ],
     )
     def test_normal_mega(self, value, expected):
-        value = BitPerSecond(value)
+        value = BitsPerSecond(value)
         assert value.mega_bps == float(expected)
         assert value.mega_byte_per_sec == value.mega_bps / 8
 
     @pytest.mark.parametrize(
         ["value", "expected"],
         [
             ["2Kbps", 2 * KILO / MEBI],
@@ -210,20 +210,20 @@
             ["2Kibps", 2 * 1024**-1],
             ["2Mibps", 2 * 1024**0],
             ["2Gibps", 2 * 1024**1],
             ["2Tibps", 2 * 1024**2],
         ],
     )
     def test_normal_mebi(self, value, expected):
-        value = BitPerSecond(value)
+        value = BitsPerSecond(value)
         assert value.mebi_bps == expected
         assert value.mebi_byte_per_sec == value.mebi_bps / 8
 
 
-class Test_BitPerSecond_gbps:
+class Test_BitsPerSecond_gbps:
     @pytest.mark.parametrize(
         ["value", "expected"],
         [
             ["2bps", 2 * 1000**-3],
             ["2Kbps", 2 * 1000**-2],
             ["2Mbps", 2 * 1000**-1],
             ["2Gbps", 2 * 1000**0],
@@ -231,15 +231,15 @@
             ["2Kibps", 2 * KIBI / GIGA],
             ["2Mibps", 2 * MEBI / GIGA],
             ["2Gibps", 2 * GIBI / GIGA],
             ["2Tibps", 2 * TEBI / GIGA],
         ],
     )
     def test_normal_giga(self, value, expected):
-        value = BitPerSecond(value)
+        value = BitsPerSecond(value)
         assert value.giga_bps == float(expected)
         assert value.giga_byte_per_sec == value.giga_bps / 8
 
     @pytest.mark.parametrize(
         ["value", "expected"],
         [
             ["2Kbps", 2 * KILO / GIBI],
@@ -249,20 +249,20 @@
             ["2Kibps", 2 * 1024**-2],
             ["2Mibps", 2 * 1024**-1],
             ["2Gibps", 2 * 1024**0],
             ["2Tibps", 2 * 1024**1],
         ],
     )
     def test_normal_gibi(self, value, expected):
-        value = BitPerSecond(value)
+        value = BitsPerSecond(value)
         assert value.gibi_bps == expected
         assert value.gibi_byte_per_sec == value.gibi_bps / 8
 
 
-class Test_BitPerSecond_tbps:
+class Test_BitsPerSecond_tbps:
     @pytest.mark.parametrize(
         ["value", "expected"],
         [
             ["2bps", 2 * 1000**-4],
             ["2Kbps", 2 * 1000**-3],
             ["2Mbps", 2 * 1000**-2],
             ["2Gbps", 2 * 1000**-1],
@@ -270,15 +270,15 @@
             ["2Kibps", 2 * KIBI / TERA],
             ["2Mibps", 2 * MEBI / TERA],
             ["2Gibps", 2 * GIBI / TERA],
             ["2Tibps", 2 * TEBI / TERA],
         ],
     )
     def test_normal_tera(self, value, expected):
-        value = BitPerSecond(value)
+        value = BitsPerSecond(value)
         assert value.tera_bps == float(expected)
         assert value.tera_byte_per_sec == value.tera_bps / 8
 
     @pytest.mark.parametrize(
         ["value", "expected"],
         [
             ["2Kbps", 2 * KILO / TEBI],
@@ -288,34 +288,49 @@
             ["2Kibps", 2 * 1024**-3],
             ["2Mibps", 2 * 1024**-2],
             ["2Gibps", 2 * 1024**-1],
             ["2Tibps", 2 * 1024**0],
         ],
     )
     def test_normal_gibi(self, value, expected):
-        value = BitPerSecond(value)
+        value = BitsPerSecond(value)
         assert value.tebi_bps == expected
         assert value.tebi_byte_per_sec == value.tebi_bps / 8
 
 
-class Test_BitPerSecond_get_as:
+class Test_BitsPerSecond_get_as:
     @pytest.mark.parametrize(
         ["value", "default_unit", "expected"],
         [
-            ["2bps", BitPerSecond.Unit.BPS, 2],
-            ["2Kbps", BitPerSecond.Unit.KBPS, 2],
-            ["2Kibps", BitPerSecond.Unit.KIBPS, 2],
-            ["2Mbps", BitPerSecond.Unit.MBPS, 2],
-            ["2Mibps", BitPerSecond.Unit.MIBPS, 2],
-            ["2Gbps", BitPerSecond.Unit.GBPS, 2],
+            ["2bps", BitsPerSecond.Unit.BPS, 2],
+            ["2Kbps", BitsPerSecond.Unit.KBPS, 2],
+            ["2Kibps", BitsPerSecond.Unit.KIBPS, 2],
+            ["2Mbps", BitsPerSecond.Unit.MBPS, 2],
+            ["2Mibps", BitsPerSecond.Unit.MIBPS, 2],
+            ["2Gbps", BitsPerSecond.Unit.GBPS, 2],
             ["2Gbps", "gbps", 2],
-            ["2Gibps", BitPerSecond.Unit.GIBPS, 2],
-            ["2Tbps", BitPerSecond.Unit.TBPS, 2],
+            ["2Gibps", BitsPerSecond.Unit.GIBPS, 2],
+            ["2Tbps", BitsPerSecond.Unit.TBPS, 2],
             ["2Tbps", "tbps", 2],
-            ["2Tibps", BitPerSecond.Unit.TIBPS, 2],
+            ["2Tibps", BitsPerSecond.Unit.TIBPS, 2],
         ],
     )
     def test_normal_default_unit(self, value, default_unit, expected):
-        bps = BitPerSecond(value, default_unit=default_unit)
+        bps = BitsPerSecond(value, default_unit=default_unit)
         print(bps, file=sys.stderr)
 
         assert bps.get_as(default_unit) == expected
+
+
+class Test_BitsPerSecond_to_humanreadable:
+    @pytest.mark.parametrize(
+        ["value", "style", "expected"],
+        [
+            ["1bps", "full", "1.0 bits per second"],
+            ["100Mbps", "full", "100.0 megabits per second"],
+            ["123456 Mbps", "full", "123.5 gigabits per second"],
+            ["1Gibps", "full", "1.0 gibibits per second"],
+            ["1Gibps", "short", "1.0 Gibps"],
+        ],
+    )
+    def test_normal_default_unit(self, value, style, expected):
+        assert BitsPerSecond(value).to_humanreadable(style=style) == expected
```

### Comparing `humanreadable-0.3.0/test/test_time.py` & `humanreadable-0.4.0/test/test_time.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,11 +227,12 @@
 class Test_Time_to_humanreadable:
     @pytest.mark.parametrize(
         ["value", "default_unit", "style", "expected"],
         [
             ["0", Time.Unit.SECOND, "full", "0 seconds"],
             ["4000", Time.Unit.SECOND, "full", "1 hours 6 minutes 40 seconds"],
             ["4000", Time.Unit.SECOND, "short", "1h 6m 40s"],
+            ["400000", Time.Unit.SECOND, "short", "4d 15h 6m 40s"],
         ],
     )
     def test_normal_default_unit(self, value, default_unit, style, expected):
         assert Time(value, default_unit=default_unit).to_humanreadable(style=style) == expected
```

### Comparing `humanreadable-0.3.0/tox.ini` & `humanreadable-0.4.0/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tox]
 envlist =
-    py{36,37,38,39,310,311}
+    py{37,38,39,310,311}
     pypy3
     build
     cov
     fmt
     lint
 
 [testenv]
 extras =
     test
 commands =
     pytest {posargs}
 
 [testenv:build]
 deps =
+    build>=0.10
     twine
     wheel
 commands =
-    python setup.py sdist bdist_wheel
+    python -m build
     twine check dist/*.whl dist/*.tar.gz
-    python setup.py clean --all
 
 [testenv:clean]
 skip_install = true
 deps =
     cleanpy>=0.4
 commands =
     cleanpy --all --exclude-envs .
@@ -52,11 +52,10 @@
 [testenv:lint]
 skip_install = true
 deps =
     codespell
     mypy>=1
     pylama>=8.4.1
 commands =
-    python setup.py check
     mypy humanreadable/ setup.py
     codespell humanreadable examples test -q2 --check-filenames
     pylama
```

