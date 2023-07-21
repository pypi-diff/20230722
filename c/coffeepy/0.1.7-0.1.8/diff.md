# Comparing `tmp/coffeepy-0.1.7.tar.gz` & `tmp/coffeepy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coffeepy-0.1.7.tar", last modified: Sun Jul 16 11:17:43 2023, max compression
+gzip compressed data, was "coffeepy-0.1.8.tar", last modified: Fri Jul 21 22:52:00 2023, max compression
```

## Comparing `coffeepy-0.1.7.tar` & `coffeepy-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:17:43.625823 coffeepy-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-16 11:17:32.000000 coffeepy-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-16 11:17:43.625823 coffeepy-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-16 11:17:32.000000 coffeepy-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-16 11:17:32.000000 coffeepy-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:17:43.625823 coffeepy-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:17:43.625823 coffeepy-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:17:43.625823 coffeepy-0.1.7/src/coffeepy/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 11:17:32.000000 coffeepy-0.1.7/src/coffeepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-16 11:17:32.000000 coffeepy-0.1.7/src/coffeepy/coffeepy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:17:43.625823 coffeepy-0.1.7/src/coffeepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-16 11:17:43.000000 coffeepy-0.1.7/src/coffeepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-16 11:17:43.000000 coffeepy-0.1.7/src/coffeepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:17:43.000000 coffeepy-0.1.7/src/coffeepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-16 11:17:43.000000 coffeepy-0.1.7/src/coffeepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-16 11:17:43.000000 coffeepy-0.1.7/src/coffeepy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:17:43.625823 coffeepy-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-16 11:17:32.000000 coffeepy-0.1.7/tests/test_coffeepy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:52:00.437009 coffeepy-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-21 22:51:50.000000 coffeepy-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-21 22:52:00.437009 coffeepy-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-21 22:51:50.000000 coffeepy-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-21 22:51:50.000000 coffeepy-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 22:52:00.437009 coffeepy-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:52:00.433009 coffeepy-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:52:00.437009 coffeepy-0.1.8/src/coffeepy/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 22:51:50.000000 coffeepy-0.1.8/src/coffeepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-21 22:51:50.000000 coffeepy-0.1.8/src/coffeepy/coffeepy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:52:00.437009 coffeepy-0.1.8/src/coffeepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-21 22:52:00.000000 coffeepy-0.1.8/src/coffeepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-21 22:52:00.000000 coffeepy-0.1.8/src/coffeepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:52:00.000000 coffeepy-0.1.8/src/coffeepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-21 22:52:00.000000 coffeepy-0.1.8/src/coffeepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 22:52:00.000000 coffeepy-0.1.8/src/coffeepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:52:00.437009 coffeepy-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-07-21 22:51:50.000000 coffeepy-0.1.8/tests/test_coffeepy.py
```

### Comparing `coffeepy-0.1.7/LICENSE` & `coffeepy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `coffeepy-0.1.7/PKG-INFO` & `coffeepy-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: coffeepy
-Version: 0.1.7
+Version: 0.1.8
 Summary: Coffeepy prevents the system from sleeping
 Author-email: kuvaus <coffeepy@kuvaus.org>
 Project-URL: Homepage, https://github.com/kuvaus/coffeepy
 Project-URL: Bug Tracker, https://github.com/kuvaus/coffeepy/issues
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/coffeepy.svg?style=flat)](https://pypi.python.org/pypi/coffeepy/) [![PyPI Version](https://img.shields.io/pypi/v/coffeepy.svg)](https://pypi.python.org/pypi/coffeepy)
 # Coffeepy
 
 Coffeepy ☕️ is a small program that prevents the system from sleeping.
```

### Comparing `coffeepy-0.1.7/README.md` & `coffeepy-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `coffeepy-0.1.7/pyproject.toml` & `coffeepy-0.1.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coffeepy"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="kuvaus", email="coffeepy@kuvaus.org" },
 ]
 description = "Coffeepy prevents the system from sleeping"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `coffeepy-0.1.7/src/coffeepy/coffeepy.py` & `coffeepy-0.1.8/src/coffeepy/coffeepy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-
-from importlib.metadata import version
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 
 import ctypes
 import sys
 import subprocess
 import time
 import argparse
 import os
+import warnings
 
 animation = [
     "  ☕️   ",
     " ☁️☕️   ",
     "  ☕️   ",
     "  ☕️☁️  ",
     " ☁️☕️   ",
@@ -25,36 +26,57 @@
 ]
 
 def display_animation(animation=animation):
     for frame in animation:
         print('\r' + frame, end='')
         time.sleep(0.5)  # Adjust the delay time as desired
 
+def get_version(package):
+    if sys.version_info >= (3, 8):
+        from importlib.metadata import version
+        return version(package)
+    else:
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=DeprecationWarning)
+            import pkg_resources
+            return pkg_resources.get_distribution(package).version
 
 def check_caffeinate():
     try:
         subprocess.check_output(['which', 'caffeinate'])
         return True
     except subprocess.CalledProcessError:
         return False
 
+def check_x11():
+    try:
+        subprocess.check_output(['which', 'xset'])
+        return True
+    except subprocess.CalledProcessError:
+        print("You need to install either \'caffeinate\' or \'x11-xserver-utils\' package for this program to run")
+        return False
+
+
 def check_windows_terminal():
-    if 'win32' in sys.platform:
-        if os.environ.get("WT_SESSION") is not None:
-            return True
-        else:
-            return False
+    if ('win32' in sys.platform) and (os.environ.get("WT_SESSION") is not None):
+        return True
     else:
         return False
 
 def parse_args(args=None):
-    parser = argparse.ArgumentParser(description='Coffeepy (v'+version('coffeepy')+') ☕️ prevents the system from sleeping.\n'
-                                                 'You can set the time with -t flag\n'
-                                                 'Made by kuvaus',
-                                                 formatter_class=argparse.RawTextHelpFormatter)
+
+    coffee_emoji = "☕️"
+    if 'win32' in sys.platform and not check_windows_terminal():
+        coffee_emoji = ""
+
+    description = 'Coffeepy (v'+get_version('coffeepy')+') '+coffee_emoji+""" prevents the system from sleeping.
+You can set the time with -t flag
+Made by kuvaus"""
+
+    parser = argparse.ArgumentParser(description=description, formatter_class=argparse.RawTextHelpFormatter)
 
     parser.add_argument('-t', '--time', type=float, default=0, help='Optional: Duration of animation in minutes. Use 0 for indefinite duration')
     parser.add_argument('-a', '--no-animation', action='store_true', help='Optional: Disable animation')
 
     return parser.parse_args(args)
     
 def run(runtime=0, no_animation=False):
@@ -78,33 +100,32 @@
         print('Running \'coffeepy\' on MacOS to prevent the system from sleeping')
         proc = subprocess.Popen(['caffeinate', '-dims'])
 
     elif 'linux' in sys.platform:
         print('Running \'coffeepy\' on Linux to prevent the system from sleeping')
         if check_caffeinate():
             proc = subprocess.Popen(['caffeinate', '-dims'])
-        else:
+        elif check_x11():
             subprocess.Popen(['xset', 's', 'off'])
             subprocess.Popen(['xset', '-dpms'])
+        else:
+            sys.exit(0)
 
     elif 'win32' in sys.platform:
         print('Running \'coffeepy\' on Windows to prevent the system from sleeping')
         ctypes.windll.kernel32.SetThreadExecutionState(0x80000002)
 
     print('Press Ctrl-C to quit')
     
     try:
         start_time = time.time()
         while time.time() - start_time < duration or duration == float('inf'):
             if not args.no_animation:
-                if 'win32' in sys.platform:
-                    if check_windows_terminal() == True:
-                        display_animation()
-                    else:
-                        display_animation(ascii_animation)
+                if 'win32' in sys.platform and not check_windows_terminal():
+                    display_animation(ascii_animation)
                 else:
                     display_animation()
             else:
                 time.sleep(1)
 
     except KeyboardInterrupt:
         print('\nExiting')
@@ -114,12 +135,11 @@
             proc.terminate()
         if 'linux' in sys.platform and not check_caffeinate():
             # Reset xset settings
             subprocess.Popen(['xset', 's', 'on'])
             subprocess.Popen(['xset', '+dpms'])
         if 'win32' in sys.platform:
             ctypes.windll.kernel32.SetThreadExecutionState(0x80000000)
-        #sys.exit(0)
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `coffeepy-0.1.7/src/coffeepy.egg-info/PKG-INFO` & `coffeepy-0.1.8/src/coffeepy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: coffeepy
-Version: 0.1.7
+Version: 0.1.8
 Summary: Coffeepy prevents the system from sleeping
 Author-email: kuvaus <coffeepy@kuvaus.org>
 Project-URL: Homepage, https://github.com/kuvaus/coffeepy
 Project-URL: Bug Tracker, https://github.com/kuvaus/coffeepy/issues
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/coffeepy.svg?style=flat)](https://pypi.python.org/pypi/coffeepy/) [![PyPI Version](https://img.shields.io/pypi/v/coffeepy.svg)](https://pypi.python.org/pypi/coffeepy)
 # Coffeepy
 
 Coffeepy ☕️ is a small program that prevents the system from sleeping.
```

### Comparing `coffeepy-0.1.7/tests/test_coffeepy.py` & `coffeepy-0.1.8/tests/test_coffeepy.py`

 * *Files 5% similar despite different names*

```diff
@@ -158,28 +158,55 @@
     mock_popen.return_value.returncode = 0
     runtime = 0.01
     run(runtime)
     mock_popen.assert_called_once_with(['caffeinate', '-dims'])
 
 #
 # Linux
-# Use mock to simulate 'subprocess.Popen'
+# Use mock to simulate 'check_x11'
 #
+
+#need to return error on caffeinate but success on xset
+def side_effect(arg):
+    if arg == ['which', 'caffeinate']:
+        raise subprocess.CalledProcessError(1, 'which')
+    elif arg == ['which', 'xset']:
+        return '/opt/X11/bin/xset'.encode()  # check_output returns bytes in Python 3
+    else:
+        return None  # default return value
+
 @patch('sys.platform', new='linux')
 @patch('subprocess.Popen')
-@patch('subprocess.check_output')
+@patch('subprocess.check_output', side_effect=side_effect)
 def test_plaform_linux_without_caffeinate(mock_subproc, mock_popen):
-    mock_subproc.side_effect = subprocess.CalledProcessError(1, 'which')
     mock_popen.return_value.returncode = 0
     runtime = 0.01
     run(runtime)
     calls = [call(['xset', 's', 'off']), call(['xset', '-dpms'])]
     mock_popen.assert_has_calls(calls, any_order=True)
 
 #
+# Linux
+# 
+#
+@patch('sys.platform', new='linux')
+@patch('subprocess.Popen')
+@patch('subprocess.check_output')
+def test_plaform_linux_without_caffeinate_or_x11(mock_subproc, mock_popen, capsys):
+    with pytest.raises(SystemExit) as excinfo:
+        mock_subproc.side_effect = subprocess.CalledProcessError(1, 'which')
+        mock_popen.return_value.returncode = 0
+        runtime = 0.01
+        run(runtime)
+
+    out, err = capsys.readouterr()
+    assert "You need to install either 'caffeinate' or 'x11-xserver-utils' package for this program to run" in out
+    assert excinfo.value.code == 0
+
+#
 # Windows
 # Use mock to simulate 'ctypes.windll.kernel32.SetThreadExecutionState'
 #
 @patch('sys.platform', new='win32')
 @patch('ctypes.windll', create=True)
 def test_platform_windows(self):
     runtime = 0.01
```

