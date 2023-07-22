# Comparing `tmp/pymemuc-0.4.2.tar.gz` & `tmp/pymemuc-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemuc-0.4.2.tar", max compression
+gzip compressed data, was "pymemuc-0.4.3.tar", max compression
```

## Comparing `pymemuc-0.4.2.tar` & `pymemuc-0.4.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1057 2023-06-15 00:06:44.775289 pymemuc-0.4.2/LICENSE
--rw-r--r--   0        0        0     1586 2023-06-15 00:06:44.775289 pymemuc-0.4.2/README.md
--rw-r--r--   0        0        0      386 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/__init__.py
--rw-r--r--   0        0        0    23371 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/_command.py
--rw-r--r--   0        0        0      465 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/_constants.py
--rw-r--r--   0        0        0     5146 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/_control.py
--rw-r--r--   0        0        0     1214 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/_decorators.py
--rw-r--r--   0        0        0    15149 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/_manage.py
--rw-r--r--   0        0        0     4624 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/_memuc.py
--rw-r--r--   0        0        0      891 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/exceptions.py
--rw-r--r--   0        0        0     3014 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/pymemuc.py
--rw-r--r--   0        0        0      379 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/vminfo.py
--rw-r--r--   0        0        0     1665 2023-06-15 00:07:06.403401 pymemuc-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pymemuc-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-07-22 18:56:11.965993 pymemuc-0.4.3/LICENSE
+-rw-r--r--   0        0        0     1586 2023-07-22 18:56:11.965993 pymemuc-0.4.3/README.md
+-rw-r--r--   0        0        0      386 2023-07-22 18:56:11.969993 pymemuc-0.4.3/pymemuc/__init__.py
+-rw-r--r--   0        0        0    24771 2023-07-22 18:56:11.969993 pymemuc-0.4.3/pymemuc/_command.py
+-rw-r--r--   0        0        0      465 2023-07-22 18:56:11.969993 pymemuc-0.4.3/pymemuc/_constants.py
+-rw-r--r--   0        0        0     5146 2023-07-22 18:56:11.969993 pymemuc-0.4.3/pymemuc/_control.py
+-rw-r--r--   0        0        0     1214 2023-07-22 18:56:11.969993 pymemuc-0.4.3/pymemuc/_decorators.py
+-rw-r--r--   0        0        0    15149 2023-07-22 18:56:11.969993 pymemuc-0.4.3/pymemuc/_manage.py
+-rw-r--r--   0        0        0     4624 2023-07-22 18:56:11.969993 pymemuc-0.4.3/pymemuc/_memuc.py
+-rw-r--r--   0        0        0      891 2023-07-22 18:56:11.969993 pymemuc-0.4.3/pymemuc/exceptions.py
+-rw-r--r--   0        0        0     3042 2023-07-22 18:56:11.969993 pymemuc-0.4.3/pymemuc/pymemuc.py
+-rw-r--r--   0        0        0      379 2023-07-22 18:56:11.969993 pymemuc-0.4.3/pymemuc/vminfo.py
+-rw-r--r--   0        0        0     1665 2023-07-22 18:56:32.786285 pymemuc-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pymemuc-0.4.3/PKG-INFO
```

### Comparing `pymemuc-0.4.2/LICENSE` & `pymemuc-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.2/README.md` & `pymemuc-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.2/pymemuc/_command.py` & `pymemuc-0.4.3/pymemuc/_command.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module contains functions for commanding running virtual machines with memuc.exe.
 Functions for interacting with running VMs are defined here."""
 from typing import TYPE_CHECKING, Literal, Tuple, Union
+from urllib.parse import urlparse
 
 from ._decorators import _retryable
 from .exceptions import PyMemucError, PyMemucIndexError, PyMemucTimeoutExpired
 
 if TYPE_CHECKING:
     from pymemuc import PyMemuc
 
@@ -624,7 +625,42 @@
         )
         return output
     if vm_name is not None:
         _, output = self.memuc_run(["-n", vm_name, "adb"] + command, timeout=timeout)
         return output
 
     raise PyMemucIndexError("Please specify either a vm index or a vm name")
+
+
+def get_adb_connection(
+    self: "PyMemuc",
+    vm_index: Union[int, None] = None,
+    vm_name: Union[str, None] = None,
+    timeout: Union[int, None] = None,
+) -> Tuple[Union[str, None], Union[int, None]]:
+    """Get the adb connection information for a VM
+
+    :param vm_index: VM index. Defaults to None.
+    :type vm_index: int, optional
+    :param vm_name: VM name. Defaults to None.
+    :type vm_name: str, optional
+    :param timeout: Timeout for the command. Defaults to None.
+    :type timeout: int, optional
+    :raises PyMemucIndexError: an error if neither a vm index or a vm name is specified
+    :raises PyMemucTimeoutExpired: an error if the command times out
+    :raises PyMemucError: an error if the command fails
+    :return: the ip and port of the adb connection as a tuple
+    :rtype: tuple[str | None, int | None]
+    """
+    adb_output = self.send_adb_command_vm(
+        ["shell", "ifconfig"],
+        vm_index=vm_index,
+        vm_name=vm_name,
+        timeout=timeout,
+    )
+    try:
+        adb_output = adb_output.split("\n")[0]
+        _, connection_string = adb_output.split("connected to ")
+        connection_string = urlparse(f"//{connection_string}")
+        return connection_string.hostname, connection_string.port
+    except ValueError as err:
+        raise PyMemucError(f"Failed to get adb connection: {adb_output}") from err
```

### Comparing `pymemuc-0.4.2/pymemuc/_control.py` & `pymemuc-0.4.3/pymemuc/_control.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.2/pymemuc/_decorators.py` & `pymemuc-0.4.3/pymemuc/_decorators.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.2/pymemuc/_manage.py` & `pymemuc-0.4.3/pymemuc/_manage.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.2/pymemuc/_memuc.py` & `pymemuc-0.4.3/pymemuc/_memuc.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.2/pymemuc/exceptions.py` & `pymemuc-0.4.3/pymemuc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.2/pymemuc/pymemuc.py` & `pymemuc-0.4.3/pymemuc/pymemuc.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
     from ._command import (
         change_gps_vm,
         connect_internet_vm,
         create_app_shortcut_vm,
         disconnect_internet_vm,
         execute_command_vm,
+        get_adb_connection,
         get_app_info_list_vm,
         get_public_ip_vm,
         input_text_vm,
         install_apk_vm,
         rotate_window_vm,
         send_adb_command_vm,
         set_accelerometer_vm,
```

### Comparing `pymemuc-0.4.2/pyproject.toml` & `pymemuc-0.4.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pymemuc"
-version = "v0.4.2"
+version = "v0.4.3"
 description = "A Memuc.exe wrapper for Python"
 readme = "README.md"
 authors = ["Martin Miglio <code@martinmiglio.dev>"]
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pymemuc-0.4.2/PKG-INFO` & `pymemuc-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymemuc
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Memuc.exe wrapper for Python
 Home-page: https://github.com/martinmiglio/pymemuc
 License: MIT
 Keywords: memu,memuc,wrapper,api
 Author: Martin Miglio
 Author-email: code@martinmiglio.dev
 Requires-Python: >=3.9,<4.0
```

