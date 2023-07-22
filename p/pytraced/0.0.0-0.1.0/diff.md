# Comparing `tmp/pytraced-0.0.0.tar.gz` & `tmp/pytraced-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytraced-0.0.0.tar", last modified: Mon Jun 19 08:01:43 2023, max compression
+gzip compressed data, was "pytraced-0.1.0.tar", last modified: Sat Jul 22 08:31:32 2023, max compression
```

## Comparing `pytraced-0.0.0.tar` & `pytraced-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 08:01:43.186538 pytraced-0.0.0/
--rw-rw-rw-   0        0        0    32746 2023-05-31 05:09:04.000000 pytraced-0.0.0/LICENSE.md
--rw-rw-rw-   0        0        0    39130 2023-06-19 08:01:43.186538 pytraced-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      634 2023-06-19 07:26:12.000000 pytraced-0.0.0/README.md
--rw-rw-rw-   0        0        0      103 2023-06-19 05:55:31.000000 pytraced-0.0.0/dev_requirements.txt
--rw-rw-rw-   0        0        0     1271 2023-06-19 08:00:36.000000 pytraced-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0        0 2023-06-19 06:34:49.000000 pytraced-0.0.0/requirements.txt
--rw-rw-rw-   0        0        0     1122 2023-06-19 08:01:43.190537 pytraced-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0       73 2023-05-31 04:06:47.000000 pytraced-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:01:43.142537 pytraced-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 08:01:43.170538 pytraced-0.0.0/src/pytraced/
--rw-rw-rw-   0        0        0       48 2023-06-19 06:44:45.000000 pytraced-0.0.0/src/pytraced/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-19 06:02:35.000000 pytraced-0.0.0/src/pytraced/py.typed
-drwxrwxrwx   0        0        0        0 2023-06-19 08:01:43.182539 pytraced-0.0.0/src/pytraced.egg-info/
--rw-rw-rw-   0        0        0    39130 2023-06-19 08:01:43.000000 pytraced-0.0.0/src/pytraced.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-06-19 08:01:43.000000 pytraced-0.0.0/src/pytraced.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 08:01:43.000000 pytraced-0.0.0/src/pytraced.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2023-06-19 08:01:43.000000 pytraced-0.0.0/src/pytraced.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-19 08:01:43.000000 pytraced-0.0.0/src/pytraced.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 08:01:43.183535 pytraced-0.0.0/tests/
--rw-rw-rw-   0        0        0      142 2023-06-19 05:58:28.000000 pytraced-0.0.0/tests/test_metadata.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:31:32.201329 pytraced-0.1.0/
+-rw-rw-rw-   0        0        0    32746 2023-06-19 08:13:23.000000 pytraced-0.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0    45373 2023-07-22 08:31:32.201329 pytraced-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6886 2023-07-22 08:21:49.000000 pytraced-0.1.0/README.md
+-rw-rw-rw-   0        0        0      146 2023-06-29 07:47:42.000000 pytraced-0.1.0/dev_requirements.txt
+-rw-rw-rw-   0        0        0     1328 2023-07-11 21:03:09.000000 pytraced-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       15 2023-07-11 21:01:30.000000 pytraced-0.1.0/requirements.txt
+-rw-rw-rw-   0        0        0     1120 2023-07-22 08:31:32.206328 pytraced-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       89 2023-07-05 23:12:07.000000 pytraced-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:31:32.054327 pytraced-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-22 08:31:32.128327 pytraced-0.1.0/src/pytraced/
+-rw-rw-rw-   0        0        0     2866 2023-07-13 08:36:55.000000 pytraced-0.1.0/src/pytraced/__init__.py
+-rw-rw-rw-   0        0        0     9289 2023-07-22 07:44:34.000000 pytraced-0.1.0/src/pytraced/_config.py
+-rw-rw-rw-   0        0        0     6055 2023-07-22 06:28:10.000000 pytraced-0.1.0/src/pytraced/_formatter.py
+-rw-rw-rw-   0        0        0     2415 2023-07-22 06:27:27.000000 pytraced-0.1.0/src/pytraced/_levels.py
+-rw-rw-rw-   0        0        0    22708 2023-07-22 07:44:34.000000 pytraced-0.1.0/src/pytraced/_logger.py
+-rw-rw-rw-   0        0        0     1610 2023-07-22 06:24:47.000000 pytraced-0.1.0/src/pytraced/_record.py
+-rw-rw-rw-   0        0        0     3462 2023-07-22 06:24:42.000000 pytraced-0.1.0/src/pytraced/_sink.py
+-rw-rw-rw-   0        0        0     1820 2023-07-22 06:24:27.000000 pytraced-0.1.0/src/pytraced/_traceback.py
+drwxrwxrwx   0        0        0        0 2023-07-22 08:31:32.150326 pytraced-0.1.0/src/pytraced/colours/
+-rw-rw-rw-   0        0        0     1033 2023-07-22 07:44:34.000000 pytraced-0.1.0/src/pytraced/colours/__init__.py
+-rw-rw-rw-   0        0        0     3658 2023-07-22 07:44:34.000000 pytraced-0.1.0/src/pytraced/colours/_colouriser.py
+-rw-rw-rw-   0        0        0     2377 2023-07-22 06:29:11.000000 pytraced-0.1.0/src/pytraced/colours/_colours.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 08:13:23.000000 pytraced-0.1.0/src/pytraced/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-22 08:31:32.142327 pytraced-0.1.0/src/pytraced.egg-info/
+-rw-rw-rw-   0        0        0    45373 2023-07-22 08:31:32.000000 pytraced-0.1.0/src/pytraced.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      838 2023-07-22 08:31:32.000000 pytraced-0.1.0/src/pytraced.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 08:31:32.000000 pytraced-0.1.0/src/pytraced.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      146 2023-07-22 08:31:32.000000 pytraced-0.1.0/src/pytraced.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-22 08:31:32.000000 pytraced-0.1.0/src/pytraced.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-22 08:31:32.197327 pytraced-0.1.0/tests/
+-rw-rw-rw-   0        0        0     1284 2023-07-22 07:44:34.000000 pytraced-0.1.0/tests/test_colouriser.py
+-rw-rw-rw-   0        0        0      713 2023-07-14 21:54:52.000000 pytraced-0.1.0/tests/test_colours.py
+-rw-rw-rw-   0        0        0     3046 2023-07-22 07:44:34.000000 pytraced-0.1.0/tests/test_config.py
+-rw-rw-rw-   0        0        0     6747 2023-07-22 06:28:40.000000 pytraced-0.1.0/tests/test_formatter.py
+-rw-rw-rw-   0        0        0      609 2023-07-18 02:56:35.000000 pytraced-0.1.0/tests/test_level.py
+-rw-rw-rw-   0        0        0    10555 2023-07-22 07:44:48.000000 pytraced-0.1.0/tests/test_logger.py
+-rw-rw-rw-   0        0        0      567 2023-07-14 21:26:53.000000 pytraced-0.1.0/tests/test_metadata.py
+-rw-rw-rw-   0        0        0      506 2023-07-18 20:28:35.000000 pytraced-0.1.0/tests/test_performance.py
+-rw-rw-rw-   0        0        0     1265 2023-07-18 23:04:02.000000 pytraced-0.1.0/tests/test_record.py
+-rw-rw-rw-   0        0        0     2155 2023-07-18 02:56:58.000000 pytraced-0.1.0/tests/test_sink.py
+-rw-rw-rw-   0        0        0      798 2023-07-19 08:51:38.000000 pytraced-0.1.0/tests/test_traceback.py
```

### Comparing `pytraced-0.0.0/LICENSE.md` & `pytraced-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pytraced-0.0.0/PKG-INFO` & `pytraced-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pytraced
-Version: 0.0.0
+Version: 0.1.0
 Summary: A simple, lightweight, & extensible logging library for python
-Author: Eris Fletcher
-Author-email: Eris Fletcher <fletcher.eris@gmail.com>
+Author: Eris
+Author-email: Eris <theferretdetective@gmail.com>
 License: # GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
         <https://fsf.org/>
         
@@ -620,26 +620,182 @@
         reviewing courts shall apply local law that most closely approximates
         an absolute waiver of all civil liability in connection with the
         Program, unless a warranty or assumption of liability accompanies a
         copy of the Program in return for a fee.
         
         END OF TERMS AND CONDITIONS
         
-Project-URL: Homepage, https://github.com/ErisFletcher/py_tracer
-Project-URL: IssueTracker, https://github.com/ErisFletcher/py_tracer/issues
+Project-URL: Homepage, https://github.com/FerretDetective/pytraced
+Project-URL: IssueTracker, https://github.com/FerretDetective/pytraced/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
-# PyTracer
+# pytraced
 
 ---
 **A simple, lightweight, & extensible logging library for python.**
 
-![Tests](https://github.com/ErisFletcher/py_tracer/actions/workflows/tests.yml/badge.svg) ![mypy: passing](https://img.shields.io/static/v1?label=mypy&message=passing&color=green) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![PyPi](https://img.shields.io/pypi/v/pytraced)](https://pypi.org/project/pytraced/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![Tests](https://github.com/FerretDetective/pytraced/actions/workflows/tests.yml/badge.svg)](https://github.com/FerretDetective/pytraced/actions/workflows/tests.yml) [![TypeChecking](https://github.com/FerretDetective/pytraced/actions/workflows/types.yml/badge.svg)](https://github.com/FerretDetective/pytraced/actions/workflows/types.yml) [![Linting](https://github.com/FerretDetective/pytraced/actions/workflows/lint.yml/badge.svg)](https://github.com/FerretDetective/pytraced/actions/workflows/lint.yml) [![mypy: checked](https://img.shields.io/static/v1?label=mypy&message=checked&color=green)](https://github.com/python/mypy) [![linting](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+
+## Table of Contents
+
+- [Overview](#overview)
+- [Installation](#installation)
+- [Basic Usage](#basic-usage)
+- [Links](#links)
+- [License](#license)
+
+## Overview
+
+Pytraced is a simple, lightweight, & extensible logging library for python. Its aim is to provide flexible logging while maintaining the ease of use of something like using `print()`. It accomplishes this by adding numerous useful features used to configure and produce informative logs.
+
+This library is architected around the idea of having a single logger object which all logs pass through. This is done using the top level `logger` object. Despite that, pytraced also provides the `Logger` class which can be used to further distribute and/or configure logging with more control.
+
+## Installation
+
+The following are instructions on the most common way and easiest ways to download & install this library.
+
+### Installing from PyPi
+
+To install the latest version of `pytraced` from PyPi simply pip install it using the following command.
+
+```sh
+pip install pytraced
+```
+
+### Installing from Github using Git
+
+To install the most up-to-date version of `pytraced` from Github using Git simply run the following command.
+
+```sh
+pip install git+https://github.com/FerretDetective/pytraced
+```
+
+### Installing from Github without Git
+
+If Git is unavailable to you, use the following instructions to download and install it from Github.
+
+1. Navigate to [home page](https://github.com/FerretDetective/pytraced).
+2. Click the green "Code" button.
+3. With that menu open, click on the button labelled "Download Zip".
+4. Find the downloaded zip.
+5. Extract the zipped files.
+6. Move the extracted folder to the desired install location.
+7. Open your terminal in the location of the extracted folder.
+8. Run the following command.
+
+```sh
+pip install .
+```
+
+## Basic Usage
+
+The following are basic examples of how to the use the logger. For more information view the docstring of any functions, class, or module.
+
+### Basic Logging
+
+For convenience the `logger` object is configured to log to stderr by default; however this is completely configurable. The `logger` object also comes with a accompanying method for all of the built in logging levels.
+
+```python
+from pytraced import logger
+
+# default level methods
+logger.info("info")
+logger.debug("debug")
+logger.trace("trace")
+logger.success("success")
+logger.warning("warning")
+logger.error("error")
+logger.critical("critical")
+
+# for logging with custom and/or dynamic levels, the `log()` method should be used
+logger.log("LOG", "log")
+```
+
+### Adding New Outputs
+
+To add new outputs to the logger the `add()` method is used. This method can be used to add callables, TextIo objects, file paths, or anything that implements `SupportsWrite[str]`. The `on_close` parameter is used to register a callback for either when the output is removed or when the interpreter exits.
+
+```python
+from pytraced import logger
+
+OUTPUT = open("info.log", "a", encoding="utf-8")
+logger.add(OUTPUT, on_remove=OUTPUT.close)  # call `close()` when this output is removed or on interpreter exit
+
+# create the file (if necessary), and open it with the specified mode and encoding.
+logger.add("logging.log", open_mode="a", encoding="utf-8")  # maintains a handle to the file during logging
+
+# function which will be called with the formatted logging message
+def log_message(message: str) -> None:
+    ...
+
+logger.add(log_message)
+```
+
+### Removing Existing Outputs
+
+To remove an existing output from the logger the `remove()` method is used. This method takes in the id of the existing output and removes it calling the `on_remove()` callback if one was provided.
+
+```python
+from sys import stderr
+
+from pytraced import logger
+
+# default output is always 0
+logger.remove(0)
+
+# the id of the output is given when it is added
+ID = logger.add(stderr)
+logger.remove(ID)
+```
+
+### Customising the Format of Logs
+
+To customise the format, the `add()` method is again used. This method accepts formats with the `log_format` parameter, filters using the `log_filter` parameter, a customisable minimum logging level with `min_level`, and finally the `colourise` parameter to toggle whether colours should be added to logs.
+
+```python
+from pytraced import logger, Record
+
+# remove the default stderr output
+logger.remove(0)
+
+# disable the colouring if logs
+logger.add("log.log", colourise=False)
+
+# anything with a severity less than `ERROR` will not be logged
+logger.add("log0.log", min_level="ERROR")
+
+# customisable date-time formats, trace styles & more
+logger.add("log1.log", log_format="%{time:dd/mm/yyyy, HH:MM:SS}% | %{lvl}% | %{trace:simple}% - %{msg}%")
+
+# make your own custom formatter
+def custom_formatter(record: Record) -> str:
+    return f"[{record.level.name}] - {record.message}"
+
+logger.add("log2.log", log_format=custom_formatter)
+
+# filter your logs with a callback
+SHOULD_LOG: bool = ...
+
+def should_log(record: Record) -> bool:
+    return SHOULD_LOG
+
+logger.add("log3.log", log_filter=should_log)
+```
+
+## Links
+
+- [Home Page](https://github.com/FerretDetective/pytraced)
+- [Issue Tracker](https://github.com/FerretDetective/pytraced/issues)
+- [License](https://github.com/FerretDetective/pytraced/blob/main/LICENSE.md)
+
+## License
+
+This project is licensed with the GNU General Public License V3, for more information view the license file which can be accessed on github located [here](https://github.com/FerretDetective/pytraced/blob/main/LICENSE.md).
```

### Comparing `pytraced-0.0.0/setup.cfg` & `pytraced-0.1.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,70 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7974 7261 6365 640d 0a76 6572   = pytraced..ver
 00000020: 7369 6f6e 203d 2061 7474 723a 2070 7974  sion = attr: pyt
 00000030: 7261 6365 642e 5f5f 7665 7273 696f 6e5f  raced.__version_
 00000040: 5f0d 0a64 6573 6372 6970 7469 6f6e 203d  _..description =
-00000050: 2041 2041 2073 696d 706c 652c 206c 6967   A A simple, lig
-00000060: 6874 7765 6967 6874 2c20 2620 6578 7465  htweight, & exte
-00000070: 6e73 6962 6c65 206c 6f67 6769 6e67 206c  nsible logging l
-00000080: 6962 7261 7279 2066 6f72 2070 7974 686f  ibrary for pytho
-00000090: 6e0d 0a6c 6f6e 675f 6465 7363 7269 7074  n..long_descript
-000000a0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
-000000b0: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
-000000c0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
-000000d0: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
-000000e0: 646f 776e 0d0a 6c69 6365 6e73 6520 3d20  down..license = 
-000000f0: 474e 5520 4765 6e65 7261 6c20 5075 626c  GNU General Publ
-00000100: 6963 204c 6963 656e 7365 2076 3320 2847  ic License v3 (G
-00000110: 504c 7633 290d 0a61 7574 686f 7220 3d20  PLv3)..author = 
-00000120: 4572 6973 2046 6c65 7463 6865 720d 0a61  Eris Fletcher..a
-00000130: 7574 686f 725f 656d 6169 6c20 3d20 666c  uthor_email = fl
-00000140: 6574 6368 6572 2e65 7269 7340 676d 6169  etcher.eris@gmai
-00000150: 6c2e 636f 6d0d 0a63 6c61 7373 6966 6965  l.com..classifie
-00000160: 7273 203d 200d 0a09 4465 7665 6c6f 706d  rs = ...Developm
-00000170: 656e 7420 5374 6174 7573 203a 3a20 3320  ent Status :: 3 
-00000180: 2d20 416c 7068 610d 0a09 496e 7465 6e64  - Alpha...Intend
-00000190: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
-000001a0: 6576 656c 6f70 6572 730d 0a09 4c69 6365  evelopers...Lice
-000001b0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-000001c0: 7665 6420 3a3a 2047 4e55 2047 656e 6572  ved :: GNU Gener
-000001d0: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
-000001e0: 6520 7633 2028 4750 4c76 3329 0d0a 094f  e v3 (GPLv3)...O
-000001f0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000200: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-00000210: 740d 0a09 5072 6f67 7261 6d6d 696e 6720  t...Programming 
-00000220: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000230: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
-00000240: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000250: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000260: 2e31 310d 0a70 7974 686f 6e5f 7265 7175  .11..python_requ
-00000270: 6972 6573 203d 203e 3d33 2e31 302c 203c  ires = >=3.10, <
-00000280: 340d 0a70 726f 6a65 6374 5f75 726c 7320  4..project_urls 
-00000290: 3d20 0d0a 0948 6f6d 6570 6167 6520 3d20  = ...Homepage = 
-000002a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000002b0: 6f6d 2f45 7269 7346 6c65 7463 6865 722f  om/ErisFletcher/
-000002c0: 7079 5f74 7261 6365 720d 0a09 4973 7375  py_tracer...Issu
-000002d0: 6554 7261 636b 6572 203d 2068 7474 7073  eTracker = https
-000002e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4572  ://github.com/Er
-000002f0: 6973 466c 6574 6368 6572 2f70 795f 7472  isFletcher/py_tr
-00000300: 6163 6572 2f69 7373 7565 730d 0a0d 0a5b  acer/issues....[
-00000310: 6f70 7469 6f6e 735d 0d0a 696e 7374 616c  options]..instal
-00000320: 6c5f 7265 7175 6972 6573 203d 2066 696c  l_requires = fil
-00000330: 653a 2072 6571 7569 7265 6d65 6e74 732e  e: requirements.
-00000340: 7478 740d 0a70 6163 6b61 6765 5f64 6972  txt..package_dir
-00000350: 203d 200d 0a09 3d20 7372 630d 0a70 6163   = ...= src..pac
-00000360: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a0d  kages = find:...
-00000370: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-00000380: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-00000390: 3d20 7372 630d 0a65 7863 6c75 6465 203d  = src..exclude =
-000003a0: 200d 0a09 6578 616d 706c 6573 2a0d 0a09   ...examples*...
-000003b0: 746f 6f6c 732a 0d0a 0964 6f63 732a 0d0a  tools*...docs*..
-000003c0: 0974 6573 7473 2a0d 0a0d 0a5b 6f70 7469  .tests*....[opti
-000003d0: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
-000003e0: 5d0d 0a6d 7970 6b67 203d 200d 0a09 7079  ]..mypkg = ...py
-000003f0: 2e74 7970 6564 0d0a 0d0a 5b6f 7074 696f  .typed....[optio
-00000400: 6e73 2e65 7874 7261 735f 7265 7175 6972  ns.extras_requir
-00000410: 655d 0d0a 6465 7620 3d20 6669 6c65 3a20  e]..dev = file: 
-00000420: 6465 765f 7265 7175 6972 656d 656e 7473  dev_requirements
-00000430: 2e74 7874 0d0a 0d0a 5b65 6767 5f69 6e66  .txt....[egg_inf
-00000440: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000450: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-00000460: 0d0a                                     ..
+00000050: 2041 2073 696d 706c 652c 206c 6967 6874   A simple, light
+00000060: 7765 6967 6874 2c20 2620 6578 7465 6e73  weight, & extens
+00000070: 6962 6c65 206c 6f67 6769 6e67 206c 6962  ible logging lib
+00000080: 7261 7279 2066 6f72 2070 7974 686f 6e0d  rary for python.
+00000090: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+000000a0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
+000000b0: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
+000000c0: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
+000000d0: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
+000000e0: 776e 0d0a 6c69 6365 6e73 6520 3d20 474e  wn..license = GN
+000000f0: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
+00000100: 204c 6963 656e 7365 2076 3320 2847 504c   License v3 (GPL
+00000110: 7633 290d 0a61 7574 686f 7220 3d20 4572  v3)..author = Er
+00000120: 6973 0d0a 6175 7468 6f72 5f65 6d61 696c  is..author_email
+00000130: 203d 2074 6865 6665 7272 6574 6465 7465   = theferretdete
+00000140: 6374 6976 6540 676d 6169 6c2e 636f 6d0d  ctive@gmail.com.
+00000150: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
+00000160: 0a09 4465 7665 6c6f 706d 656e 7420 5374  ..Development St
+00000170: 6174 7573 203a 3a20 3320 2d20 416c 7068  atus :: 3 - Alph
+00000180: 610d 0a09 496e 7465 6e64 6564 2041 7564  a...Intended Aud
+00000190: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
+000001a0: 6572 730d 0a09 4c69 6365 6e73 6520 3a3a  ers...License ::
+000001b0: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+000001c0: 2047 4e55 2047 656e 6572 616c 2050 7562   GNU General Pub
+000001d0: 6c69 6320 4c69 6365 6e73 6520 7633 2028  lic License v3 (
+000001e0: 4750 4c76 3329 0d0a 094f 7065 7261 7469  GPLv3)...Operati
+000001f0: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
+00000200: 496e 6465 7065 6e64 656e 740d 0a09 5072  Independent...Pr
+00000210: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000220: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000230: 332e 3130 0d0a 0950 726f 6772 616d 6d69  3.10...Programmi
+00000240: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000250: 7974 686f 6e20 3a3a 2033 2e31 310d 0a70  ython :: 3.11..p
+00000260: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+00000270: 203e 3d33 2e31 302c 203c 340d 0a70 726f   >=3.10, <4..pro
+00000280: 6a65 6374 5f75 726c 7320 3d20 0d0a 0948  ject_urls = ...H
+00000290: 6f6d 6570 6167 6520 3d20 6874 7470 733a  omepage = https:
+000002a0: 2f2f 6769 7468 7562 2e63 6f6d 2f46 6572  //github.com/Fer
+000002b0: 7265 7444 6574 6563 7469 7665 2f70 7974  retDetective/pyt
+000002c0: 7261 6365 640d 0a09 4973 7375 6554 7261  raced...IssueTra
+000002d0: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
+000002e0: 6974 6875 622e 636f 6d2f 4665 7272 6574  ithub.com/Ferret
+000002f0: 4465 7465 6374 6976 652f 7079 7472 6163  Detective/pytrac
+00000300: 6564 2f69 7373 7565 730d 0a0d 0a5b 6f70  ed/issues....[op
+00000310: 7469 6f6e 735d 0d0a 696e 7374 616c 6c5f  tions]..install_
+00000320: 7265 7175 6972 6573 203d 2066 696c 653a  requires = file:
+00000330: 2072 6571 7569 7265 6d65 6e74 732e 7478   requirements.tx
+00000340: 740d 0a70 6163 6b61 6765 5f64 6972 203d  t..package_dir =
+00000350: 200d 0a09 3d20 7372 630d 0a70 6163 6b61   ...= src..packa
+00000360: 6765 7320 3d20 6669 6e64 3a0d 0a0d 0a5b  ges = find:....[
+00000370: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
+00000380: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
+00000390: 7372 630d 0a65 7863 6c75 6465 203d 200d  src..exclude = .
+000003a0: 0a09 6578 616d 706c 6573 2a0d 0a09 746f  ..examples*...to
+000003b0: 6f6c 732a 0d0a 0964 6f63 732a 0d0a 0974  ols*...docs*...t
+000003c0: 6573 7473 2a0d 0a0d 0a5b 6f70 7469 6f6e  ests*....[option
+000003d0: 732e 7061 636b 6167 655f 6461 7461 5d0d  s.package_data].
+000003e0: 0a6d 7970 6b67 203d 200d 0a09 7079 2e74  .mypkg = ...py.t
+000003f0: 7970 6564 0d0a 0d0a 5b6f 7074 696f 6e73  yped....[options
+00000400: 2e65 7874 7261 735f 7265 7175 6972 655d  .extras_require]
+00000410: 0d0a 6465 7620 3d20 6669 6c65 3a20 6465  ..dev = file: de
+00000420: 765f 7265 7175 6972 656d 656e 7473 2e74  v_requirements.t
+00000430: 7874 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  xt....[egg_info]
+00000440: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+00000450: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `pytraced-0.0.0/src/pytraced.egg-info/PKG-INFO` & `pytraced-0.1.0/src/pytraced.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pytraced
-Version: 0.0.0
+Version: 0.1.0
 Summary: A simple, lightweight, & extensible logging library for python
-Author: Eris Fletcher
-Author-email: Eris Fletcher <fletcher.eris@gmail.com>
+Author: Eris
+Author-email: Eris <theferretdetective@gmail.com>
 License: # GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
         <https://fsf.org/>
         
@@ -620,26 +620,182 @@
         reviewing courts shall apply local law that most closely approximates
         an absolute waiver of all civil liability in connection with the
         Program, unless a warranty or assumption of liability accompanies a
         copy of the Program in return for a fee.
         
         END OF TERMS AND CONDITIONS
         
-Project-URL: Homepage, https://github.com/ErisFletcher/py_tracer
-Project-URL: IssueTracker, https://github.com/ErisFletcher/py_tracer/issues
+Project-URL: Homepage, https://github.com/FerretDetective/pytraced
+Project-URL: IssueTracker, https://github.com/FerretDetective/pytraced/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
-# PyTracer
+# pytraced
 
 ---
 **A simple, lightweight, & extensible logging library for python.**
 
-![Tests](https://github.com/ErisFletcher/py_tracer/actions/workflows/tests.yml/badge.svg) ![mypy: passing](https://img.shields.io/static/v1?label=mypy&message=passing&color=green) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![PyPi](https://img.shields.io/pypi/v/pytraced)](https://pypi.org/project/pytraced/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![Tests](https://github.com/FerretDetective/pytraced/actions/workflows/tests.yml/badge.svg)](https://github.com/FerretDetective/pytraced/actions/workflows/tests.yml) [![TypeChecking](https://github.com/FerretDetective/pytraced/actions/workflows/types.yml/badge.svg)](https://github.com/FerretDetective/pytraced/actions/workflows/types.yml) [![Linting](https://github.com/FerretDetective/pytraced/actions/workflows/lint.yml/badge.svg)](https://github.com/FerretDetective/pytraced/actions/workflows/lint.yml) [![mypy: checked](https://img.shields.io/static/v1?label=mypy&message=checked&color=green)](https://github.com/python/mypy) [![linting](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+
+## Table of Contents
+
+- [Overview](#overview)
+- [Installation](#installation)
+- [Basic Usage](#basic-usage)
+- [Links](#links)
+- [License](#license)
+
+## Overview
+
+Pytraced is a simple, lightweight, & extensible logging library for python. Its aim is to provide flexible logging while maintaining the ease of use of something like using `print()`. It accomplishes this by adding numerous useful features used to configure and produce informative logs.
+
+This library is architected around the idea of having a single logger object which all logs pass through. This is done using the top level `logger` object. Despite that, pytraced also provides the `Logger` class which can be used to further distribute and/or configure logging with more control.
+
+## Installation
+
+The following are instructions on the most common way and easiest ways to download & install this library.
+
+### Installing from PyPi
+
+To install the latest version of `pytraced` from PyPi simply pip install it using the following command.
+
+```sh
+pip install pytraced
+```
+
+### Installing from Github using Git
+
+To install the most up-to-date version of `pytraced` from Github using Git simply run the following command.
+
+```sh
+pip install git+https://github.com/FerretDetective/pytraced
+```
+
+### Installing from Github without Git
+
+If Git is unavailable to you, use the following instructions to download and install it from Github.
+
+1. Navigate to [home page](https://github.com/FerretDetective/pytraced).
+2. Click the green "Code" button.
+3. With that menu open, click on the button labelled "Download Zip".
+4. Find the downloaded zip.
+5. Extract the zipped files.
+6. Move the extracted folder to the desired install location.
+7. Open your terminal in the location of the extracted folder.
+8. Run the following command.
+
+```sh
+pip install .
+```
+
+## Basic Usage
+
+The following are basic examples of how to the use the logger. For more information view the docstring of any functions, class, or module.
+
+### Basic Logging
+
+For convenience the `logger` object is configured to log to stderr by default; however this is completely configurable. The `logger` object also comes with a accompanying method for all of the built in logging levels.
+
+```python
+from pytraced import logger
+
+# default level methods
+logger.info("info")
+logger.debug("debug")
+logger.trace("trace")
+logger.success("success")
+logger.warning("warning")
+logger.error("error")
+logger.critical("critical")
+
+# for logging with custom and/or dynamic levels, the `log()` method should be used
+logger.log("LOG", "log")
+```
+
+### Adding New Outputs
+
+To add new outputs to the logger the `add()` method is used. This method can be used to add callables, TextIo objects, file paths, or anything that implements `SupportsWrite[str]`. The `on_close` parameter is used to register a callback for either when the output is removed or when the interpreter exits.
+
+```python
+from pytraced import logger
+
+OUTPUT = open("info.log", "a", encoding="utf-8")
+logger.add(OUTPUT, on_remove=OUTPUT.close)  # call `close()` when this output is removed or on interpreter exit
+
+# create the file (if necessary), and open it with the specified mode and encoding.
+logger.add("logging.log", open_mode="a", encoding="utf-8")  # maintains a handle to the file during logging
+
+# function which will be called with the formatted logging message
+def log_message(message: str) -> None:
+    ...
+
+logger.add(log_message)
+```
+
+### Removing Existing Outputs
+
+To remove an existing output from the logger the `remove()` method is used. This method takes in the id of the existing output and removes it calling the `on_remove()` callback if one was provided.
+
+```python
+from sys import stderr
+
+from pytraced import logger
+
+# default output is always 0
+logger.remove(0)
+
+# the id of the output is given when it is added
+ID = logger.add(stderr)
+logger.remove(ID)
+```
+
+### Customising the Format of Logs
+
+To customise the format, the `add()` method is again used. This method accepts formats with the `log_format` parameter, filters using the `log_filter` parameter, a customisable minimum logging level with `min_level`, and finally the `colourise` parameter to toggle whether colours should be added to logs.
+
+```python
+from pytraced import logger, Record
+
+# remove the default stderr output
+logger.remove(0)
+
+# disable the colouring if logs
+logger.add("log.log", colourise=False)
+
+# anything with a severity less than `ERROR` will not be logged
+logger.add("log0.log", min_level="ERROR")
+
+# customisable date-time formats, trace styles & more
+logger.add("log1.log", log_format="%{time:dd/mm/yyyy, HH:MM:SS}% | %{lvl}% | %{trace:simple}% - %{msg}%")
+
+# make your own custom formatter
+def custom_formatter(record: Record) -> str:
+    return f"[{record.level.name}] - {record.message}"
+
+logger.add("log2.log", log_format=custom_formatter)
+
+# filter your logs with a callback
+SHOULD_LOG: bool = ...
+
+def should_log(record: Record) -> bool:
+    return SHOULD_LOG
+
+logger.add("log3.log", log_filter=should_log)
+```
+
+## Links
+
+- [Home Page](https://github.com/FerretDetective/pytraced)
+- [Issue Tracker](https://github.com/FerretDetective/pytraced/issues)
+- [License](https://github.com/FerretDetective/pytraced/blob/main/LICENSE.md)
+
+## License
+
+This project is licensed with the GNU General Public License V3, for more information view the license file which can be accessed on github located [here](https://github.com/FerretDetective/pytraced/blob/main/LICENSE.md).
```

