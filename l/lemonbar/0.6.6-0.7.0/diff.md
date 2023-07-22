# Comparing `tmp/lemonbar-0.6.6.tar.gz` & `tmp/lemonbar-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemonbar-0.6.6.tar", last modified: Sat Jul 22 14:53:54 2023, max compression
+gzip compressed data, was "lemonbar-0.7.0.tar", last modified: Sat Jul 22 16:01:05 2023, max compression
```

## Comparing `lemonbar-0.6.6.tar` & `lemonbar-0.7.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:53:54.584266 lemonbar-0.6.6/
--rw-r--r--   0 ori       (1000) ori       (1000)     1066 2023-07-22 12:38:48.000000 lemonbar-0.6.6/LICENSE
--rw-r--r--   0 ori       (1000) ori       (1000)     5641 2023-07-22 14:53:54.585266 lemonbar-0.6.6/PKG-INFO
--rw-r--r--   0 ori       (1000) ori       (1000)     4834 2023-07-22 13:48:25.000000 lemonbar-0.6.6/README.md
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:53:54.583266 lemonbar-0.6.6/lemonbar/
--rw-r--r--   0 ori       (1000) ori       (1000)      129 2023-07-22 13:46:23.000000 lemonbar-0.6.6/lemonbar/__init__.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1166 2023-07-22 12:58:07.000000 lemonbar-0.6.6/lemonbar/async_utils.py
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:53:54.584266 lemonbar-0.6.6/lemonbar/formatters/
--rw-r--r--   0 ori       (1000) ori       (1000)      110 2023-07-22 13:48:25.000000 lemonbar-0.6.6/lemonbar/formatters/__init__.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1078 2023-07-21 19:14:24.000000 lemonbar-0.6.6/lemonbar/formatters/_formatter.py
--rw-r--r--   0 ori       (1000) ori       (1000)      521 2023-07-22 13:36:40.000000 lemonbar-0.6.6/lemonbar/formatters/attributes.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1047 2023-07-22 13:36:40.000000 lemonbar-0.6.6/lemonbar/formatters/basic_formatters.py
--rw-r--r--   0 ori       (1000) ori       (1000)      369 2023-07-22 13:36:40.000000 lemonbar-0.6.6/lemonbar/formatters/button.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1324 2023-07-22 13:36:40.000000 lemonbar-0.6.6/lemonbar/formatters/change_monitor.py
--rw-r--r--   0 ori       (1000) ori       (1000)     6187 2023-07-22 13:46:54.000000 lemonbar-0.6.6/lemonbar/lemonbar.py
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:53:54.584266 lemonbar-0.6.6/lemonbar/models/
--rw-r--r--   0 ori       (1000) ori       (1000)      109 2023-07-22 13:38:31.000000 lemonbar-0.6.6/lemonbar/models/__init__.py
--rw-r--r--   0 ori       (1000) ori       (1000)      985 2023-07-22 13:48:25.000000 lemonbar-0.6.6/lemonbar/models/bar_geometry.py
--rw-r--r--   0 ori       (1000) ori       (1000)       99 2023-07-21 17:39:08.000000 lemonbar-0.6.6/lemonbar/models/bar_placement.py
--rw-r--r--   0 ori       (1000) ori       (1000)     3282 2023-07-22 13:39:01.000000 lemonbar-0.6.6/lemonbar/models/lemonbar_arguments.py
--rw-r--r--   0 ori       (1000) ori       (1000)      839 2023-07-22 14:53:04.000000 lemonbar-0.6.6/lemonbar/models/monitor.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1934 2023-07-22 13:25:07.000000 lemonbar-0.6.6/lemonbar/module.py
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:53:54.584266 lemonbar-0.6.6/lemonbar/modules/
--rw-r--r--   0 ori       (1000) ori       (1000)        0 2023-07-21 21:42:55.000000 lemonbar-0.6.6/lemonbar/modules/__init__.py
--rw-r--r--   0 ori       (1000) ori       (1000)     1692 2023-07-22 13:45:37.000000 lemonbar-0.6.6/lemonbar/modules/clock.py
-drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 14:53:54.583266 lemonbar-0.6.6/lemonbar.egg-info/
--rw-r--r--   0 ori       (1000) ori       (1000)     5641 2023-07-22 14:53:54.000000 lemonbar-0.6.6/lemonbar.egg-info/PKG-INFO
--rw-r--r--   0 ori       (1000) ori       (1000)      701 2023-07-22 14:53:54.000000 lemonbar-0.6.6/lemonbar.egg-info/SOURCES.txt
--rw-r--r--   0 ori       (1000) ori       (1000)        1 2023-07-22 14:53:54.000000 lemonbar-0.6.6/lemonbar.egg-info/dependency_links.txt
--rw-r--r--   0 ori       (1000) ori       (1000)       41 2023-07-22 14:53:54.000000 lemonbar-0.6.6/lemonbar.egg-info/requires.txt
--rw-r--r--   0 ori       (1000) ori       (1000)        9 2023-07-22 14:53:54.000000 lemonbar-0.6.6/lemonbar.egg-info/top_level.txt
--rw-r--r--   0 ori       (1000) ori       (1000)       79 2023-07-22 14:53:54.585266 lemonbar-0.6.6/setup.cfg
--rw-r--r--   0 ori       (1000) ori       (1000)     1079 2023-07-22 14:53:04.000000 lemonbar-0.6.6/setup.py
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 16:01:05.304823 lemonbar-0.7.0/
+-rw-r--r--   0 ori       (1000) ori       (1000)     1066 2023-07-22 12:38:48.000000 lemonbar-0.7.0/LICENSE
+-rw-r--r--   0 ori       (1000) ori       (1000)     5641 2023-07-22 16:01:05.304823 lemonbar-0.7.0/PKG-INFO
+-rw-r--r--   0 ori       (1000) ori       (1000)     4834 2023-07-22 13:48:25.000000 lemonbar-0.7.0/README.md
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 16:01:05.303822 lemonbar-0.7.0/lemonbar/
+-rw-r--r--   0 ori       (1000) ori       (1000)      187 2023-07-22 15:50:45.000000 lemonbar-0.7.0/lemonbar/__init__.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1166 2023-07-22 12:58:07.000000 lemonbar-0.7.0/lemonbar/async_utils.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1474 2023-07-22 15:56:32.000000 lemonbar-0.7.0/lemonbar/command_handler.py
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 16:01:05.303822 lemonbar-0.7.0/lemonbar/formatters/
+-rw-r--r--   0 ori       (1000) ori       (1000)      110 2023-07-22 13:48:25.000000 lemonbar-0.7.0/lemonbar/formatters/__init__.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1078 2023-07-21 19:14:24.000000 lemonbar-0.7.0/lemonbar/formatters/_formatter.py
+-rw-r--r--   0 ori       (1000) ori       (1000)      521 2023-07-22 13:36:40.000000 lemonbar-0.7.0/lemonbar/formatters/attributes.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1047 2023-07-22 13:36:40.000000 lemonbar-0.7.0/lemonbar/formatters/basic_formatters.py
+-rw-r--r--   0 ori       (1000) ori       (1000)      369 2023-07-22 13:36:40.000000 lemonbar-0.7.0/lemonbar/formatters/button.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1324 2023-07-22 13:36:40.000000 lemonbar-0.7.0/lemonbar/formatters/change_monitor.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     6237 2023-07-22 15:26:02.000000 lemonbar-0.7.0/lemonbar/lemonbar.py
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 16:01:05.304823 lemonbar-0.7.0/lemonbar/models/
+-rw-r--r--   0 ori       (1000) ori       (1000)      109 2023-07-22 13:38:31.000000 lemonbar-0.7.0/lemonbar/models/__init__.py
+-rw-r--r--   0 ori       (1000) ori       (1000)      985 2023-07-22 13:48:25.000000 lemonbar-0.7.0/lemonbar/models/bar_geometry.py
+-rw-r--r--   0 ori       (1000) ori       (1000)       99 2023-07-21 17:39:08.000000 lemonbar-0.7.0/lemonbar/models/bar_placement.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     3282 2023-07-22 13:39:01.000000 lemonbar-0.7.0/lemonbar/models/lemonbar_arguments.py
+-rw-r--r--   0 ori       (1000) ori       (1000)      839 2023-07-22 14:53:04.000000 lemonbar-0.7.0/lemonbar/models/monitor.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1964 2023-07-22 15:16:48.000000 lemonbar-0.7.0/lemonbar/module.py
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 16:01:05.304823 lemonbar-0.7.0/lemonbar/modules/
+-rw-r--r--   0 ori       (1000) ori       (1000)        0 2023-07-21 21:42:55.000000 lemonbar-0.7.0/lemonbar/modules/__init__.py
+-rw-r--r--   0 ori       (1000) ori       (1000)     1626 2023-07-22 15:56:32.000000 lemonbar-0.7.0/lemonbar/modules/clock.py
+drwxr-xr-x   0 ori       (1000) ori       (1000)        0 2023-07-22 16:01:05.303822 lemonbar-0.7.0/lemonbar.egg-info/
+-rw-r--r--   0 ori       (1000) ori       (1000)     5641 2023-07-22 16:01:05.000000 lemonbar-0.7.0/lemonbar.egg-info/PKG-INFO
+-rw-r--r--   0 ori       (1000) ori       (1000)      729 2023-07-22 16:01:05.000000 lemonbar-0.7.0/lemonbar.egg-info/SOURCES.txt
+-rw-r--r--   0 ori       (1000) ori       (1000)        1 2023-07-22 16:01:05.000000 lemonbar-0.7.0/lemonbar.egg-info/dependency_links.txt
+-rw-r--r--   0 ori       (1000) ori       (1000)       41 2023-07-22 16:01:05.000000 lemonbar-0.7.0/lemonbar.egg-info/requires.txt
+-rw-r--r--   0 ori       (1000) ori       (1000)        9 2023-07-22 16:01:05.000000 lemonbar-0.7.0/lemonbar.egg-info/top_level.txt
+-rw-r--r--   0 ori       (1000) ori       (1000)       79 2023-07-22 16:01:05.304823 lemonbar-0.7.0/setup.cfg
+-rw-r--r--   0 ori       (1000) ori       (1000)     1079 2023-07-22 15:59:40.000000 lemonbar-0.7.0/setup.py
```

### Comparing `lemonbar-0.6.6/LICENSE` & `lemonbar-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.6/PKG-INFO` & `lemonbar-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lemonbar
-Version: 0.6.6
+Version: 0.7.0
 Summary: A Python API for interacting with Lemonbar
 Home-page: https://github.com/Heknon/lemonbar-api
-Download-URL: https://github.com/Heknon/lemonbar-api/archive/refs/tags/v0.6.6.tar.gz
+Download-URL: https://github.com/Heknon/lemonbar-api/archive/refs/tags/v0.7.0.tar.gz
 Author: Ori Harel
 Author-email: oeharel@gmail.com
 License: MIT
 Keywords: lemonbar,api,lemonbar-api,arch,linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `lemonbar-0.6.6/README.md` & `lemonbar-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.6/lemonbar/async_utils.py` & `lemonbar-0.7.0/lemonbar/async_utils.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.6/lemonbar/formatters/_formatter.py` & `lemonbar-0.7.0/lemonbar/formatters/_formatter.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.6/lemonbar/formatters/attributes.py` & `lemonbar-0.7.0/lemonbar/formatters/attributes.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.6/lemonbar/formatters/basic_formatters.py` & `lemonbar-0.7.0/lemonbar/formatters/basic_formatters.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.6/lemonbar/formatters/change_monitor.py` & `lemonbar-0.7.0/lemonbar/formatters/change_monitor.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.6/lemonbar/lemonbar.py` & `lemonbar-0.7.0/lemonbar/lemonbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import List, Optional, Dict
 
 from .async_utils import state_kept_await
 from .models.bar_geometry import BarGeometry
 from .models.bar_placement import BarPlacement
 from .models.lemonbar_arguments import LemonbarArguments
 from .models.monitor import MonitorId
-from .module import Module
+from .module import Module, EventHandler
 
 _DEFAULT_LOGGER = logging.getLogger("lemonbar")
 
 
 class Lemonbar:
     def __init__(
             self,
@@ -80,15 +80,15 @@
             [event_pipe], [], [event_pipe],
             self.minimum_wait_time.total_seconds()
         )
 
         if event_pipe in exceptions:
             raise RuntimeError("An error occurred waiting for Lemonbar to write!")
 
-        event = event_pipe.readline().rstrip() if event_pipe in readables else None
+        event = event_pipe.readline().strip() if event_pipe in readables else None
 
         render_cycles = [state_kept_await(module, self._handle_module_cycle(module, event)) for module in self._modules]
         for cycle_data in asyncio.as_completed(render_cycles):
             module, render_value = await cycle_data
             had_exception = isinstance(render_value, Exception)
             try:
                 if had_exception:
@@ -111,15 +111,15 @@
                     self._module_last_render[module] = datetime.datetime.now()
 
         self._lemonbar_process.stdin.write('\n')
         self._lemonbar_process.stdin.flush()
 
     async def _handle_module_cycle(self, module: Module, event: Optional[str]) -> str:
         should_handle_event = False
-        if event and await module.should_handle_event(event):
+        if event and isinstance(module, EventHandler) and await module.should_handle_event(event):
             await module.handle_event(event)
             should_handle_event = True
 
         current_time = datetime.datetime.now()
         module_config = module.config
 
         last_render_time = self._module_last_render.get(module)
```

### Comparing `lemonbar-0.6.6/lemonbar/models/bar_geometry.py` & `lemonbar-0.7.0/lemonbar/models/bar_geometry.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.6/lemonbar/models/lemonbar_arguments.py` & `lemonbar-0.7.0/lemonbar/models/lemonbar_arguments.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.6/lemonbar/models/monitor.py` & `lemonbar-0.7.0/lemonbar/models/monitor.py`

 * *Files identical despite different names*

### Comparing `lemonbar-0.6.6/lemonbar/module.py` & `lemonbar-0.7.0/lemonbar/module.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,30 +13,14 @@
 
     @abc.abstractmethod
     async def should_render(self) -> bool:
         """
         :return: True if the `render` method should be called next render cycle
         """
 
-    @abc.abstractmethod
-    async def handle_event(self, event: str):
-        """
-        Called when <event> is received through stdout communication with Lemonbar
-        if `should_handle_event` returns True.
-        """
-
-    @abc.abstractmethod
-    async def should_handle_event(self, event: str) -> bool:
-        """
-        Called when <event> is received through stdout communication with Lemonbar
-
-        :param event: The stdout *line* from Lemonbar
-        :return: True if the `handle_event` should be called.
-        """
-
     @property
     def config(self) -> 'Module.Config':
         """
         :return: Module configuration
         """
         return Module.Config()
 
@@ -50,7 +34,25 @@
             and `should_render`, ignore the `minimum_render_time` and call `render`.
         :param cache_exceptions: If true, if an exception is thrown during render
             it is cached and render is only called again if <minimum_render_interval> has passed
         """
         minimum_render_interval: datetime.timedelta = datetime.timedelta(seconds=1)
         force_render_on_event: bool = True
         cache_exceptions: bool = True
+
+
+class EventHandler(abc.ABC):
+    @abc.abstractmethod
+    async def handle_event(self, event: str):
+        """
+        Called when <event> is received through stdout communication with Lemonbar
+        if `should_handle_event` returns True.
+        """
+
+    @abc.abstractmethod
+    async def should_handle_event(self, event: str) -> bool:
+        """
+        Called when <event> is received through stdout communication with Lemonbar
+
+        :param event: The stdout *line* from Lemonbar
+        :return: True if the `handle_event` should be called.
+        """
```

### Comparing `lemonbar-0.6.6/lemonbar/modules/clock.py` & `lemonbar-0.7.0/lemonbar/modules/clock.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,55 @@
 import datetime
 from time import strftime
 from typing import Optional
 
-from lemonbar import formatters
+from lemonbar import CommandHandler, Button
 from lemonbar.module import Module
 
 _EVENT_NAME = "toggle_clock"
 
 
-class Clock(Module):
+class Clock(Module, CommandHandler):
     _CONFIG = Module.Config(
         minimum_render_interval=datetime.timedelta(milliseconds=700),
         force_render_on_event=True,
         cache_exceptions=True
     )
 
     def __init__(self):
         """A simple clock.
 
         The clock can be clicked and will switch to the date for a period of
         time.
         """
         super().__init__()
         self._toggled_at: Optional[datetime.datetime] = None
+        self.register_command(_EVENT_NAME, Button.LEFT, lambda button: Clock.toggle(self, button))
 
     async def render(self):
         # If the clock has been toggled for more than a certain period of time
         if self._toggled_at and datetime.datetime.now() > self._toggled_at + datetime.timedelta(seconds=5):
             self._toggled_at = None  # Automatically toggle back to the clock
 
         if self._toggled_at:
-            return formatters.button(
-                formatters.Button.LEFT,
+            return self.as_command(
                 _EVENT_NAME,
                 strftime('%d/%m/%Y')
             )
         else:
-            return formatters.button(
-                formatters.Button.LEFT,
+            return self.as_command(
                 _EVENT_NAME,
                 strftime('%H:%M:%S')
             )
 
     async def should_render(self) -> bool:
         return True
 
-    async def handle_event(self, event):
+    def toggle(self, button: Button):
         if not self._toggled_at:
             self._toggled_at = datetime.datetime.now()
         else:
             self._toggled_at = None
 
-    async def should_handle_event(self, event: str) -> bool:
-        return event.strip() == _EVENT_NAME
-
     @property
     def config(self) -> Module.Config:
         return self._CONFIG
```

### Comparing `lemonbar-0.6.6/lemonbar.egg-info/PKG-INFO` & `lemonbar-0.7.0/lemonbar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lemonbar
-Version: 0.6.6
+Version: 0.7.0
 Summary: A Python API for interacting with Lemonbar
 Home-page: https://github.com/Heknon/lemonbar-api
-Download-URL: https://github.com/Heknon/lemonbar-api/archive/refs/tags/v0.6.6.tar.gz
+Download-URL: https://github.com/Heknon/lemonbar-api/archive/refs/tags/v0.7.0.tar.gz
 Author: Ori Harel
 Author-email: oeharel@gmail.com
 License: MIT
 Keywords: lemonbar,api,lemonbar-api,arch,linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `lemonbar-0.6.6/lemonbar.egg-info/SOURCES.txt` & `lemonbar-0.7.0/lemonbar.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 lemonbar/__init__.py
 lemonbar/async_utils.py
+lemonbar/command_handler.py
 lemonbar/lemonbar.py
 lemonbar/module.py
 lemonbar.egg-info/PKG-INFO
 lemonbar.egg-info/SOURCES.txt
 lemonbar.egg-info/dependency_links.txt
 lemonbar.egg-info/requires.txt
 lemonbar.egg-info/top_level.txt
```

### Comparing `lemonbar-0.6.6/setup.py` & `lemonbar-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from distutils.core import setup
 from pathlib import Path
 
 setup(
     name='lemonbar',
-    version='0.6.6',
+    version='0.7.0',
     license='MIT',
     description='A Python API for interacting with Lemonbar',
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     author='Ori Harel',
     author_email='oeharel@gmail.com',
     url='https://github.com/Heknon/lemonbar-api',
-    download_url='https://github.com/Heknon/lemonbar-api/archive/refs/tags/v0.6.6.tar.gz',
+    download_url='https://github.com/Heknon/lemonbar-api/archive/refs/tags/v0.7.0.tar.gz',
     keywords=['lemonbar', 'api', 'lemonbar-api', "arch", "linux"],
     install_requires=[
         'pydantic',
         'screeninfo',
         'pydantic_extra_types',
     ],
     classifiers=[
```

