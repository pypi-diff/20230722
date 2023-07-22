# Comparing `tmp/mine-4.0a3.tar.gz` & `tmp/mine-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mine-4.0a3.tar", max compression
+gzip compressed data, was "mine-4.1.tar", max compression
```

## Comparing `mine-4.0a3.tar` & `mine-4.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1088 2019-05-21 02:49:19.000000 mine-4.0a3/LICENSE.md
--rw-r--r--   0        0        0     2841 2023-07-19 21:05:32.369830 mine-4.0a3/README.md
--rw-r--r--   0        0        0      340 2023-04-16 19:25:03.010573 mine-4.0a3/mine/__init__.py
--rw-r--r--   0        0        0     6866 2023-07-19 22:27:02.284270 mine-4.0a3/mine/cli.py
--rw-r--r--   0        0        0     2889 2023-07-19 02:12:18.943946 mine-4.0a3/mine/common.py
--rw-r--r--   0        0        0     6665 2023-07-19 22:45:25.548783 mine-4.0a3/mine/manager.py
--rw-r--r--   0        0        0      217 2023-07-19 02:12:18.944037 mine-4.0a3/mine/models/__init__.py
--rw-r--r--   0        0        0     1095 2023-07-19 03:18:20.515733 mine-4.0a3/mine/models/application.py
--rw-r--r--   0        0        0     2121 2023-07-19 02:18:02.802475 mine-4.0a3/mine/models/computer.py
--rw-r--r--   0        0        0     3772 2023-07-19 22:18:01.818807 mine-4.0a3/mine/models/config.py
--rw-r--r--   0        0        0     5413 2023-07-19 02:28:30.879778 mine-4.0a3/mine/models/data.py
--rw-r--r--   0        0        0     5878 2023-07-19 22:22:09.135433 mine-4.0a3/mine/models/status.py
--rw-r--r--   0        0        0      882 2023-07-19 02:12:18.944631 mine-4.0a3/mine/models/timestamp.py
--rwxr-xr-x   0        0        0     2720 2023-07-19 02:46:39.336705 mine-4.0a3/mine/services.py
--rw-r--r--   0        0        0      578 2023-07-19 02:12:18.944827 mine-4.0a3/mine/settings.py
--rw-r--r--   0        0        0       34 2016-09-23 05:48:42.000000 mine-4.0a3/mine/tests/__init__.py
--rw-r--r--   0        0        0     1044 2023-07-19 22:32:22.022967 mine-4.0a3/mine/tests/conftest.py
--rw-r--r--   0        0        0        9 2016-09-23 02:41:14.000000 mine-4.0a3/mine/tests/files/.gitignore
--rw-r--r--   0        0        0      513 2016-09-23 02:41:14.000000 mine-4.0a3/mine/tests/files/mine-in.yml
--rw-r--r--   0        0        0      587 2016-09-23 02:41:14.000000 mine-4.0a3/mine/tests/files/mine-out.yml
--rw-r--r--   0        0        0     3995 2023-07-19 22:16:31.053982 mine-4.0a3/mine/tests/test_cli.py
--rw-r--r--   0        0        0     3493 2023-07-19 22:51:10.384382 mine-4.0a3/mine/tests/test_manager.py
--rw-r--r--   0        0        0     1002 2023-07-19 01:11:50.938610 mine-4.0a3/mine/tests/test_models_application.py
--rw-r--r--   0        0        0     2193 2023-07-19 01:11:50.938810 mine-4.0a3/mine/tests/test_models_computer.py
--rw-r--r--   0        0        0     3086 2023-07-19 02:12:18.936287 mine-4.0a3/mine/tests/test_models_config.py
--rw-r--r--   0        0        0      782 2023-07-19 21:55:07.916719 mine-4.0a3/mine/tests/test_models_data.py
--rw-r--r--   0        0        0     4961 2023-04-16 19:11:58.200402 mine-4.0a3/mine/tests/test_models_status.py
--rw-r--r--   0        0        0     1750 2023-04-16 19:11:58.200536 mine-4.0a3/mine/tests/test_models_timestamp.py
--rw-r--r--   0        0        0     3226 2023-07-19 02:41:25.796394 mine-4.0a3/mine/tests/test_services.py
--rw-r--r--   0        0        0     2240 2023-07-19 22:42:55.992809 mine-4.0a3/pyproject.toml
--rw-r--r--   0        0        0     4173 1970-01-01 00:00:00.000000 mine-4.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1088 2019-05-21 02:49:19.000000 mine-4.1/LICENSE.md
+-rw-r--r--   0        0        0     2841 2023-07-20 03:59:49.514562 mine-4.1/README.md
+-rw-r--r--   0        0        0      340 2023-07-20 16:16:17.756329 mine-4.1/mine/__init__.py
+-rw-r--r--   0        0        0     6947 2023-07-22 17:36:25.564173 mine-4.1/mine/cli.py
+-rw-r--r--   0        0        0     2889 2023-07-20 03:59:49.515236 mine-4.1/mine/common.py
+-rw-r--r--   0        0        0      738 2023-07-22 17:00:58.306091 mine-4.1/mine/daemon.py
+-rw-r--r--   0        0        0     6572 2023-07-21 15:47:11.834590 mine-4.1/mine/manager.py
+-rw-r--r--   0        0        0      217 2023-07-20 03:59:49.515737 mine-4.1/mine/models/__init__.py
+-rw-r--r--   0        0        0     1095 2023-07-20 03:59:49.516054 mine-4.1/mine/models/application.py
+-rw-r--r--   0        0        0     2256 2023-07-20 17:01:39.723214 mine-4.1/mine/models/computer.py
+-rw-r--r--   0        0        0     3849 2023-07-20 16:44:45.581239 mine-4.1/mine/models/config.py
+-rw-r--r--   0        0        0     5504 2023-07-22 17:26:46.814498 mine-4.1/mine/models/data.py
+-rw-r--r--   0        0        0     5851 2023-07-22 17:26:02.306292 mine-4.1/mine/models/status.py
+-rw-r--r--   0        0        0      882 2023-07-20 03:59:49.517420 mine-4.1/mine/models/timestamp.py
+-rwxr-xr-x   0        0        0     2633 2023-07-21 15:47:11.835482 mine-4.1/mine/services.py
+-rw-r--r--   0        0        0      578 2023-07-20 03:59:49.517606 mine-4.1/mine/settings.py
+-rw-r--r--   0        0        0       34 2016-09-23 05:48:42.000000 mine-4.1/mine/tests/__init__.py
+-rw-r--r--   0        0        0     1044 2023-07-22 16:40:54.685419 mine-4.1/mine/tests/conftest.py
+-rw-r--r--   0        0        0        9 2016-09-23 02:41:14.000000 mine-4.1/mine/tests/files/.gitignore
+-rw-r--r--   0        0        0      513 2016-09-23 02:41:14.000000 mine-4.1/mine/tests/files/mine-in.yml
+-rw-r--r--   0        0        0      587 2016-09-23 02:41:14.000000 mine-4.1/mine/tests/files/mine-out.yml
+-rw-r--r--   0        0        0     4331 2023-07-22 17:37:18.341856 mine-4.1/mine/tests/test_cli.py
+-rw-r--r--   0        0        0     3493 2023-07-20 03:59:49.518427 mine-4.1/mine/tests/test_manager.py
+-rw-r--r--   0        0        0     1002 2023-07-19 01:11:50.938610 mine-4.1/mine/tests/test_models_application.py
+-rw-r--r--   0        0        0     2259 2023-07-20 17:04:31.061085 mine-4.1/mine/tests/test_models_computer.py
+-rw-r--r--   0        0        0     3129 2023-07-20 17:03:59.687664 mine-4.1/mine/tests/test_models_config.py
+-rw-r--r--   0        0        0     1317 2023-07-22 17:32:29.302799 mine-4.1/mine/tests/test_models_data.py
+-rw-r--r--   0        0        0     4953 2023-07-21 16:23:58.330586 mine-4.1/mine/tests/test_models_status.py
+-rw-r--r--   0        0        0     1750 2023-04-16 19:11:58.200536 mine-4.1/mine/tests/test_models_timestamp.py
+-rw-r--r--   0        0        0     3283 2023-07-21 15:47:11.836361 mine-4.1/mine/tests/test_services.py
+-rw-r--r--   0        0        0     2238 2023-07-22 17:06:03.413807 mine-4.1/pyproject.toml
+-rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 mine-4.1/PKG-INFO
```

### Comparing `mine-4.0a3/LICENSE.md` & `mine-4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mine-4.0a3/README.md` & `mine-4.1/README.md`

 * *Files identical despite different names*

### Comparing `mine-4.0a3/mine/cli.py` & `mine-4.1/mine/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 #!/usr/bin/env python
 
 """Command-line interface."""
 
 import argparse
-import subprocess
 import sys
 import time
 
+import datafiles
 import log
-from datafiles import frozen
-from datafiles.model import create_model
 from startfile import startfile
 
-from . import CLI, DESCRIPTION, VERSION, common, services
-from .manager import BaseManager, get_manager
-from .models import Application, Data, Versions
-
-daemon = Application(CLI, versions=Versions(mac="mine", windows="mine", linux="mine"))
+from . import CLI, DESCRIPTION, VERSION, common, daemon, services
+from .manager import get_manager
+from .models import Data
 
 
 def main(args=None):
     """Process command-line arguments and run the program."""
 
     # Shared options
     debug = argparse.ArgumentParser(add_help=False)
@@ -50,28 +46,34 @@
         "--daemon",
         metavar="DELAY",
         nargs="?",
         const=300,
         type=int,
         help="run continuously with delay [seconds]",
     )
-    parser.add_argument("-f", "--file", help="custom settings file path")
+    parser.add_argument(
+        "-f",
+        "--file",
+        help="custom settings file path",
+    )
     subs = parser.add_subparsers(help="", dest="command", metavar="<command>")
 
     # Build switch parser
     info = "start applications on another computer"
     sub = subs.add_parser(
         "switch",
         description=info.capitalize() + ".",
         help=info,
         formatter_class=common.HelpFormatter,
         parents=[debug],
     )
     sub.add_argument(
-        "name", nargs="?", help="computer to queue for launch (default: current)"
+        "name",
+        nargs="?",
+        help="computer to queue for launch (default: current)",
     )
 
     # Build close parser
     info = "close applications on this computer"
     sub = subs.add_parser(
         "close",
         description=info.capitalize() + ".",
@@ -101,27 +103,41 @@
     )
     sub.add_argument(
         "-f",
         "--force",
         action="store_true",
         help="actually delete the conflicted files",
     )
+    sub.add_argument(
+        "-r",
+        "--reset",
+        action="store_true",
+        help="reset the internal status counter",
+    )
+    sub.add_argument(
+        "-s",
+        "--stop",
+        action="store_true",
+        help="stop the background daemon process",
+    )
 
     # Parse arguments
     args = parser.parse_args(args=args)
     kwargs = {"delay": args.daemon}
     if args.command == "switch":
         kwargs["switch"] = args.name if args.name else True
     elif args.command == "close":
         kwargs["switch"] = False
     elif args.command == "edit":
         kwargs["edit"] = True
     elif args.command == "clean":
         kwargs["delete"] = True
         kwargs["force"] = args.force
+        kwargs["reset"] = args.reset
+        kwargs["stop"] = args.stop
 
     # Configure logging
     common.configure_logging(args.verbose)
 
     # Run the program
     try:
         log.debug("Running main command...")
@@ -144,106 +160,101 @@
     path=None,
     cleanup=True,
     delay=None,
     switch=None,
     edit=False,
     delete=False,
     force=False,
+    reset=False,
+    stop=False,
 ):
     """Run the program.
 
     :param path: custom settings file path
     :param cleanup: remove unused items from the config
     :param delay: number of seconds to delay before repeating
 
     :param switch: computer name to queue for launch
 
     :param edit: launch the configuration file for editing
 
     :param delete: attempt to delete conflicted files
     :param force: actually delete conflicted files
+    :param reset: reset the internal status counter
+    :param stop: stop the background daemon process
 
-    """  # pylint: disable=too-many-arguments,too-many-branches
+    """
     manager = get_manager()
     if not manager.is_running(services.APPLICATION):
         manager.start(services.APPLICATION)
 
     root = services.find_root()
     path = path or services.find_config_path(root=root)
-
-    data: Data = create_model(Data, pattern=path, defaults=True)()
-
-    config = data.config
-    status = data.status
+    data = Data(path)
 
     log.info("Identifying current computer...")
-    computer = config.get_current_computer()
+    with datafiles.frozen(data):
+        computer = data.config.get_current_computer()
     log.info("Current computer: %s", computer)
 
+    if stop:
+        daemon.stop(manager)
+    if reset:
+        with datafiles.frozen(data):
+            data.prune_status(reset_counter=True)
     if edit:
         return startfile(path)
     if delete:
         return services.delete_conflicts(root, force=force)
 
     if switch is True:
         switch = computer
     elif switch is False:
-        data.close_all_applications(config, manager)
+        data.close_all_applications(manager)
     elif switch:
-        switch = config.match_computer(switch)
+        switch = data.config.match_computer(switch)
 
     if switch:
         if switch != computer:
-            data.close_all_applications(config, manager)
-        data.queue_all_applications(config, status, switch)
+            data.close_all_applications(manager)
+        data.queue_all_applications(switch)
 
     while True:
-        services.delete_conflicts(root, config_only=True, force=True)
-        with frozen(data):
-            data.launch_queued_applications(config, status, computer, manager)
-            data.update_status(config, status, computer, manager)
+        if services.delete_conflicts(root, config_only=True, force=True):
+            log.info("Delaying 10 seconds for changes to delete...")
+            time.sleep(10)
+        with datafiles.frozen(data):
+            data.launch_queued_applications(computer, manager)
+            data.update_status(computer, manager)
 
         if delay is None or delay <= 0:
             break
 
-        log.info("Delaying %s seconds for files to sync...", delay)
-        time.sleep(delay)
+        if data.modified:
+            log.info("Delaying 10 seconds for changes to upload...")
+            time.sleep(10)
 
-        step = 5
         elapsed = 0
-        log.info("Waiting %s seconds for status changes...", delay)
-        while elapsed < delay and not data.modified:
-            time.sleep(step)
-            elapsed += step
-
-        short_delay = 30
-        log.info("Delaying %s seconds for files to sync...", short_delay)
-        time.sleep(short_delay)
+        log.info(f"Waiting up to {delay} seconds for changes...")
+        while elapsed < delay:
+            time.sleep(5)
+            elapsed += 5
+            if data.modified:
+                log.info(f"Status changed after {elapsed} seconds")
+                log.info("Delaying 10 seconds for changes to download...")
+                time.sleep(10)
+                break
+        else:
+            log.info(f"No status change after {elapsed} seconds")
 
     if cleanup:
-        with frozen(data):
-            data.prune_status(config, status)
+        with datafiles.frozen(data):
+            data.prune_status()
 
     if delay is None:
-        return _restart_daemon(manager)
-
-    return True
-
-
-def _restart_daemon(manager: BaseManager):
-    cmd = "nohup {} --daemon --verbose >> /tmp/mine.log 2>&1 &".format(CLI)
-    if daemon and not manager.is_running(daemon):
-        log.warning("Daemon is not running, attempting to restart...")
-
-        log.info("$ %s", cmd)
-        subprocess.call(cmd, shell=True)
-        if manager.is_running(daemon):
-            return True
-
-        log.error("Manually start daemon: %s", cmd)
-        return False
+        return daemon.restart(manager)
 
     return True
 
 
-if __name__ == "__main__":  # pragma: no cover (manual test)
+if __name__ == "__main__":
     main()
```

### Comparing `mine-4.0a3/mine/common.py` & `mine-4.1/mine/common.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a3/mine/manager.py` & `mine-4.1/mine/manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,62 +6,55 @@
 import os
 import platform
 import time
 
 import log
 import psutil
 
-# TODO: delete this after implementing `BaseManager`
-# https://github.com/jacebrowning/mine/issues/8
-# https://github.com/jacebrowning/mine/issues/9
 
-
-# TODO: enable coverage when a Linux test is implemented
-def log_running(func):  # pragma: no cover (manual)
+def log_running(func):
     @functools.wraps(func)
     def wrapped(self, application):
-        log.debug("Determining if %s is running...", application)
+        log.debug(f"Determining if {application} is running...")
         running = func(self, application)
         if running is None:
-            status = "Application untracked"
+            status = "Application is untracked"
         elif running:
-            status = "Application running on current machine"
+            status = "Application running on this computer"
         else:
-            status = "Application not running on current machine"
-        log.info("%s: %s", status, application)
+            status = "Application not running on this computer"
+        log.info(f"{status}: {application}")
         return running
 
     return wrapped
 
 
-# TODO: enable coverage when a Linux test is implemented
-def log_starting(func):  # pragma: no cover (manual)
+def log_starting(func):
     @functools.wraps(func)
     def wrapped(self, application):
         log.info("Starting %s...", application)
         result = func(self, application)
         log.info("Running: %s", application)
         return result
 
     return wrapped
 
 
-# TODO: enable coverage when a Linux test is implemented
-def log_stopping(func):  # pragma: no cover (manual)
+def log_stopping(func):
     @functools.wraps(func)
     def wrapped(self, application):
         log.info("Stopping %s...", application)
         result = func(self, application)
         log.info("Not running: %s", application)
         return result
 
     return wrapped
 
 
-class BaseManager(metaclass=abc.ABCMeta):  # pragma: no cover (abstract)
+class Manager(metaclass=abc.ABCMeta):  # pragma: no cover (abstract)
     """Base application manager."""
 
     NAME = FRIENDLY = ""
 
     IGNORED_APPLICATION_NAMES: list[str] = []
 
     def __str__(self):
@@ -114,15 +107,15 @@
                     break
             else:
                 return process
 
         return None
 
 
-class LinuxManager(BaseManager):  # pragma: no cover (manual)
+class LinuxManager(Manager):  # pragma: no cover (manual)
     """Application manager for Linux."""
 
     NAME = "Linux"
     FRIENDLY = NAME
 
     def is_running(self, application):
         name = application.versions.linux
@@ -132,34 +125,40 @@
         return process is not None
 
     def start(self, application):
         pass
 
     def stop(self, application):
         name = application.versions.linux
-        process = self._get_process(name)
-        if process.is_running():
-            process.terminate()
+        while True:
+            process = self._get_process(name)
+            if process and process.is_running():
+                process.terminate()
+                process.wait()
+            else:
+                break
 
 
-class MacManager(BaseManager):  # pragma: no cover (manual)
+class MacManager(Manager):  # pragma: no cover (manual)
     """Application manager for macOS."""
 
     NAME = "Darwin"
-    FRIENDLY = "Mac"
+    FRIENDLY = "macOS"
 
     IGNORED_APPLICATION_NAMES = [
-        "iTunesHelper.app",
-        "slack helper.app",
+        "com.apple.mail.spotlightindexextension",
+        "com.apple.notes.spotlightindexextension",
+        "com.apple.podcasts.spotlightindexextension",
         "garcon.appex",
-        "musiccacheextension",
-        "podcastswidget",
+        "iTunesHelper.app",
         "mailcachedelete",
-        "com.apple.mail.spotlightindexextension",
         "mailshortcutsextension",
+        "musiccacheextension",
+        "podcastswidget",
+        "slack helper.app",
     ]
 
     @log_running
     def is_running(self, application):
         name = application.versions.mac
         if not name:
             return None
@@ -187,28 +186,32 @@
         else:
             assert path, "Not found: {}".format(application)
         return self._start_app(path)
 
     @log_stopping
     def stop(self, application):
         name = application.versions.mac
-        process = self._get_process(name)
-        if process and process.is_running():
-            process.terminate()
+        while True:
+            process = self._get_process(name)
+            if process and process.is_running():
+                process.terminate()
+                process.wait()
+            else:
+                break
 
     @staticmethod
     def _start_app(path):
         """Start an application from it's .app directory."""
         assert os.path.exists(path), path
         process = psutil.Popen(["open", path])
         time.sleep(1)
         return process
 
 
-class WindowsManager(BaseManager):  # pragma: no cover (manual)
+class WindowsManager(Manager):  # pragma: no cover (manual)
     """Application manager for Windows."""
 
     NAME = "Windows"
     FRIENDLY = NAME
 
     def is_running(self, application):
         pass
@@ -216,18 +219,18 @@
     def start(self, application):
         pass
 
     def stop(self, application):
         pass
 
 
-def get_manager(name=None) -> BaseManager:
+def get_manager(name=None) -> Manager:
     """Return an application manager for the current operating system."""
-    log.info("Detecting the current system...")
+    log.info("Detecting the operating system...")
     name = name or platform.system()
     manager = {  # type: ignore
         WindowsManager.NAME: WindowsManager,
         MacManager.NAME: MacManager,
         LinuxManager.NAME: LinuxManager,
     }[name]()
-    log.info("Current system: %s", manager)
+    log.info("Identified operating system: %s", manager)
     return manager
```

### Comparing `mine-4.0a3/mine/models/application.py` & `mine-4.1/mine/models/application.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a3/mine/models/computer.py` & `mine-4.1/mine/models/computer.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,28 +4,32 @@
 import platform
 import re
 import socket
 import subprocess
 import uuid
 from dataclasses import dataclass
 
+from .. import __version__
+
 
 @dataclass
 class Computer:
     """A dictionary of identifying computer information."""
 
     name: str
-    hostname: str = ""
-    address: str = ""
     serial: str = ""
+    address: str = ""
+    hostname: str = ""
+    mine: str = "v" + __version__
 
     def __post_init__(self):
         self.address = self.address or self.get_address()
         self.hostname = self.hostname or self.get_hostname()
         self.serial = self.serial or self.get_serial()
+        assert ":" in self.address, f"Invalid address: {self.address!r}"
 
     def __str__(self):
         return self.name
 
     def __eq__(self, other):
         return str(self).lower() == str(other).lower()
```

### Comparing `mine-4.0a3/mine/models/config.py` & `mine-4.1/mine/models/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,37 +46,38 @@
         return None
 
     def get_current_computer(self, default_name: str = ""):
         """Get the current computer's information."""
         this = Computer("?")
         log.debug(f"Comparing information with {this!r}...")
 
-        # Search for a matching hostname
-        for other in self.computers:
-            if this.hostname == other.hostname:
-                log.debug(f"Matched via hostname: {other!r}")
-                other.address = this.address
-                if this.serial:
-                    other.serial = this.serial
-                return other
-
-        # Else, search for a matching serial
+        # Search for a matching serial
         for other in self.computers:
             if this.serial and this.serial == other.serial:
                 log.debug(f"Matched via serial: {other!r}")
                 other.hostname = this.hostname
+                other.mine = this.mine
+                return other
+
+        # Else, search for a matching hostname
+        for other in self.computers:
+            if this.hostname == other.hostname:
+                log.debug(f"Matched via hostname: {other!r}")
+                other.address = this.address
+                other.serial = other.serial or this.serial
+                other.mine = this.mine
                 return other
 
         # Else, search for a matching address
         for other in self.computers:
             if this.address == other.address:
                 log.debug(f"Matched via address: {other!r}")
                 other.hostname = this.hostname
-                if this.serial:
-                    other.serial = this.serial
+                other.serial = other.serial or this.serial
+                other.mine = this.mine
                 return other
 
         # Else, this is a new computer
         this.name = default_name or self.generate_computer_name(this)
         assert this.name != "localhost"
         log.debug(f"Detected new computer: {this!r}")
         self.computers.append(this)
```

### Comparing `mine-4.0a3/mine/models/data.py` & `mine-4.1/mine/models/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Data structures that combine all program data."""
 
-from dataclasses import dataclass, field
 
 import crayons
 import log
+from datafiles import datafile, field
 
-from ..manager import BaseManager
+from ..manager import Manager
+from .computer import Computer
 from .config import ProgramConfig
 from .status import ProgramStatus
 
 
-@dataclass
+@datafile("{self.path}", defaults=True)
 class Data:
     """Primary wrapper for all settings."""
 
+    path: str
     config: ProgramConfig = field(default_factory=ProgramConfig)
     status: ProgramStatus = field(default_factory=ProgramStatus)
 
     def __post_init__(self):
         self._last_counter = self.status.counter
 
     def __repr__(self):
@@ -25,102 +27,99 @@
 
     @property
     def modified(self):
         changed = self.status.counter != self._last_counter
         self._last_counter = self.status.counter
         return changed
 
-    @staticmethod
-    def prune_status(config: ProgramConfig, status: ProgramStatus):
+    def prune_status(self, *, reset_counter=False):
         """Remove undefined applications and computers."""
         log.info("Cleaning up applications and computers...")
-        for appstatus in status.applications.copy():
-            if not config.find_application(appstatus.application):
-                status.applications.remove(appstatus)
-                log.info("Removed application: %s", appstatus)
+        for status in self.status.applications.copy():
+            if not self.config.find_application(status.application):
+                self.status.applications.remove(status)
+                log.info("Removed application: %s", status)
             else:
-                for computerstate in appstatus.computers.copy():
-                    if not config.find_computer(computerstate.computer):
-                        appstatus.computers.remove(computerstate)
-                        log.info("Removed computer: %s", computerstate)
+                for state in status.computers.copy():
+                    if not self.config.find_computer(state.computer):
+                        status.computers.remove(state)
+                        log.info("Removed computer: %s", state)
+        if reset_counter:
+            self.status.counter = 0
+            for status in self.status.applications:
+                for computer in status.computers:
+                    computer.timestamp.started = 0
+                    computer.timestamp.stopped = 0
 
-    @staticmethod
-    def queue_all_applications(config: ProgramConfig, status: ProgramStatus, computer):
+    def queue_all_applications(self, computer: Computer):
         """Queue applications for launch."""
         log.info("Queuing applications for launch...")
-        for application in config.applications:
+        for application in self.config.applications:
             if application.auto_queue:
                 log.debug("Queuing %s on %s...", application, computer)
-                status.queue(application, computer)
+                self.status.queue(application, computer)
 
-    @staticmethod
-    def launch_queued_applications(
-        config: ProgramConfig, status: ProgramStatus, computer, manager: BaseManager
-    ):
+    def launch_queued_applications(self, computer: Computer, manager: Manager):
         """Launch applications that have been queued."""
         log.info("Launching queued applications...")
-        for app_status in status.applications:
-            if app_status.next:
-                application = config.get_application(app_status.application)
-                print(crayons.yellow(f"{application} is queued for {app_status.next}"))
-                if app_status.next == computer:
-                    latest = status.get_latest(application)
+        for status in self.status.applications:
+            if status.next:
+                application = self.config.get_application(status.application)
+                print(crayons.yellow(f"{application} is queued for {status.next}"))
+                if status.next == computer:
+                    latest = self.status.get_latest(application)
                     if latest in (computer, None) or application.no_wait:
                         if not manager.is_running(application):
                             manager.start(application)
-                        app_status.next = None
+                        status.next = None
                     else:
                         print(
                             crayons.yellow(
                                 f"{application} is still running on {latest}"
                             )
                         )
                 elif manager.is_running(application):
                     manager.stop(application)
 
-    @staticmethod
-    def close_all_applications(config: ProgramConfig, manager: BaseManager):
+    def close_all_applications(self, manager: Manager):
         """Close all applications running on this computer."""
         log.info("Closing all applications on this computer...")
-        for application in config.applications:
+        for application in self.config.applications:
             manager.stop(application)
 
-    @staticmethod
-    def update_status(
-        config: ProgramConfig, status: ProgramStatus, computer, manager: BaseManager
-    ):
+    def update_status(self, computer: Computer, manager: Manager):
         """Update each application's status."""
         log.info("Recording application status...")
-        for application in config.applications:
-            latest = status.get_latest(application)
+        for application in self.config.applications:
+            latest = self.status.get_latest(application)
             if manager.is_running(application):
                 if computer != latest:
-                    if status.is_running(application, computer):
+                    if self.status.is_running(application, computer):
                         # case 1: application just launched remotely
                         manager.stop(application)
-                        status.stop(application, computer)
+                        self.status.stop(application, computer)
                         print(
                             crayons.green(f"{application} is now running on {latest}")
                         )
                         print(
                             crayons.red(f"{application} is now stopped on {computer}")
                         )
                     else:
                         # case 2: application just launched locally
-                        status.start(application, computer)
+                        self.status.start(application, computer)
                         print(
                             crayons.green(f"{application} is now running on {computer}")
                         )
                 else:
                     # case 3: application already running locally
                     print(crayons.cyan(f"{application} is running on {computer}"))
             else:
-                if status.is_running(application, computer):
+                if self.status.is_running(application, computer):
                     # case 4: application just closed locally
-                    status.stop(application, computer)
+                    self.status.stop(application, computer)
                     print(crayons.red(f"{application} is now stopped on {computer}"))
                 elif latest:
                     # case 5: application already closed locally
                     print(crayons.magenta(f"{application} is running on {latest}"))
                 else:
                     # case 6: application is not running
                     print(crayons.white(f"{application} is not running"))
```

### Comparing `mine-4.0a3/mine/models/status.py` & `mine-4.1/mine/models/status.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,47 +76,46 @@
         return str(self.application).lower() < str(other.application).lower()
 
 
 @dataclass
 class ProgramStatus:
     """Dictionary of current program status."""
 
-    applications: list[Status] = field(default_factory=list)
     counter: int = 0
+    applications: list[Status] = field(default_factory=list)
 
-    def find(self, application):
+    def find(self, application: Application):
         """Return the application status for an application."""
-        for app_status in self.applications:
-            if app_status.application == application.name:
+        for status in self.applications:
+            if status.application == application.name:
                 break
         else:
-            app_status = Status(application.name)
-            self.applications.append(app_status)
-        return app_status
+            status = Status(application.name)
+            self.applications.append(status)
+        return status
 
-    def get_latest(self, application):
+    def get_latest(self, application: Application) -> str | None:
         """Get the last computer's name logged as running an application."""
         for status in self.applications:
             if status.application == application.name:
                 states = [s for s in status.computers if s.timestamp.active]
                 if states:
                     states.sort(key=lambda s: s.timestamp, reverse=True)
                     log.debug(
                         "%s marked as started on: %s",
                         application,
                         ", ".join(str(s) for s in states),
                     )
-                    # TODO: consider returning the computer instance?
                     return states[0].computer
 
         log.debug(f"{application} marked as started on: nothing")
         return None
 
     @log_running
-    def is_running(self, application, computer):
+    def is_running(self, application: Application, computer: Computer):
         """Determine if an application is logged as running on a computer."""
         for status in self.applications:
             if status.application == application.name:
                 for state in status.computers:
                     if state.computer == computer.name:
                         return state.timestamp.active
```

### Comparing `mine-4.0a3/mine/models/timestamp.py` & `mine-4.1/mine/models/timestamp.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a3/mine/services.py` & `mine-4.1/mine/services.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import log
 
 from .models.application import Application, Versions
 
 ROOTS = (r"C:\Users", r"/Users", r"/home")
 SERVICES = ("Dropbox", "Dropbox (Personal)")
-CONFIG = "mine4.yml"  # TODO: Change back to "mine.yml" with 4.x release
+CONFIG = "mine.yml"
 CONFLICT_BASE = r"{} \(.+'s conflicted copy \d+-\d+-\d+.*\).*"
 CONFLICT_ANY = CONFLICT_BASE.format(".+")
 CONFLICT_CONFIG = CONFLICT_BASE.format("mine")
 DEPTH = 3  # number of levels to search for the settings file
 APPLICATION = Application(
     "Dropbox",
     versions=Versions(mac="Dropbox.app", windows="Dropbox.exe", linux="dropbox"),
@@ -27,15 +27,15 @@
     log.debug("Looking for sharing service in '%s'...", top)
     for directory in os.listdir(top):
         if directory in SERVICES:
             path = os.path.join(top, directory)
             log.debug("Found sharing service: %s", path)
             return path
 
-    msg = "no sharing service found"
+    msg = "No sharing service found"
     if os.getenv("CI"):
         log.warning(msg)
         return top
 
     raise EnvironmentError(msg)
 
 
@@ -55,30 +55,29 @@
         if os.path.isfile(path) and not os.path.isfile(os.path.join(path, "setup.py")):
             log.info("Found settings file: %s", path)
             return path
 
     raise EnvironmentError("No '{}' file found".format(CONFIG))
 
 
-def delete_conflicts(root=None, config_only=False, force=False):
+def delete_conflicts(root=None, config_only=False, force=False) -> int:
     """Delete all files with conflicted filenames."""
     root = root or find_root()
 
     log.info("%s conflicted files...", "Deleting" if force else "Displaying")
     pattern = CONFLICT_CONFIG if config_only else CONFLICT_ANY
-    log.debug("Pattern: %r", pattern)
     regex = re.compile(pattern)
     count = 0
     for dirname, _, filenames in os.walk(root):
         for filename in filenames:
             if regex.match(filename):
                 count += 1
                 path = os.path.join(dirname, filename)
                 if force:
                     os.remove(path)
                 print(path)
 
     if count and not force:
         print(f"\nRun again with '--force' to delete these {count} conflict(s)")
-        return False
+        return 0
 
-    return True
+    return count
```

### Comparing `mine-4.0a3/mine/settings.py` & `mine-4.1/mine/settings.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a3/mine/tests/conftest.py` & `mine-4.1/mine/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a3/mine/tests/files/mine-in.yml` & `mine-4.1/mine/tests/files/mine-in.yml`

 * *Files identical despite different names*

### Comparing `mine-4.0a3/mine/tests/files/mine-out.yml` & `mine-4.1/mine/tests/files/mine-out.yml`

 * *Files identical despite different names*

### Comparing `mine-4.0a3/mine/tests/test_cli.py` & `mine-4.1/mine/tests/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     @patch("mine.cli.run", Mock(side_effect=KeyboardInterrupt))
     def test_interrupt_verbose(self, mock_log):
         """Verify the CLI can be interrupted (verbose output)."""
         with pytest.raises(SystemExit):
             cli.main(["-vvvv"])
         assert mock_log.exception.call_count == 1
 
-    @patch("mine.cli.daemon", None)
+    @patch("mine.daemon.application", None)
     def test_path(self, tmp_path):
         """Verify a custom setting file path can be used."""
         cli.main(["--file", tmp_path])
 
         assert os.path.isfile(tmp_path)
 
     @patch("mine.cli.run")
@@ -61,15 +61,15 @@
         mock_run.assert_called_once_with(path=None, delay=300)
 
     @patch("mine.cli.run")
     def test_daemon_with_specific_delay(self, mock_run):
         cli.main(["--daemon", "42"])
         mock_run.assert_called_once_with(path=None, delay=42)
 
-    @patch("mine.cli.daemon", Application("?"))
+    @patch("mine.daemon.application", Application("?"))
     def test_warning_when_daemon_is_not_running(self, tmp_path):
         with pytest.raises(SystemExit):
             cli.main(["--file", tmp_path])
 
 
 class TestSwitch:
     """Unit tests for the `switch` function."""
@@ -88,21 +88,30 @@
 
 
 class TestClean:
     @patch("mine.cli.run")
     def test_clean(self, mock_run):
         cli.main(["clean"])
         mock_run.assert_called_once_with(
-            path=None, delay=None, delete=True, force=False
+            path=None, delay=None, delete=True, force=False, reset=False, stop=False
         )
 
     @patch("mine.cli.run")
     def test_clean_with_force(self, mock_run):
         cli.main(["clean", "--force"])
-        mock_run.assert_called_once_with(path=None, delay=None, delete=True, force=True)
+        mock_run.assert_called_once_with(
+            path=None, delay=None, delete=True, force=True, reset=False, stop=False
+        )
+
+    @patch("mine.cli.run")
+    def test_clean_with_stop(self, mock_run):
+        cli.main(["clean", "--stop"])
+        mock_run.assert_called_once_with(
+            path=None, delay=None, delete=True, force=False, reset=False, stop=True
+        )
 
 
 class TestEdit:
     @patch("mine.cli.run")
     def test_edit(self, mock_run):
         cli.main(["edit"])
         mock_run.assert_called_once_with(path=None, delay=None, edit=True)
```

### Comparing `mine-4.0a3/mine/tests/test_manager.py` & `mine-4.1/mine/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a3/mine/tests/test_models_application.py` & `mine-4.1/mine/tests/test_models_application.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a3/mine/tests/test_models_computer.py` & `mine-4.1/mine/tests/test_models_computer.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,18 +13,19 @@
         computer = Computer("my-sample")
         assert "my-sample" == computer.name
         assert "00:00:00:00:00:00" == computer.address
         assert "Sample.local" == computer.hostname
 
     def test_init_defaults(self):
         """Verify the correct computer information can be overridden."""
-        computer = Computer("name", "hostname", "address")
+        computer = Computer("name", "serial", "address:", "hostname")
         assert "name" == computer.name
-        assert "address" == computer.address
+        assert "address:" == computer.address
         assert "hostname" == computer.hostname
+        assert "serial" == computer.serial
 
     def test_eq(self):
         """Verify computers and strings can be equated."""
         assert Computer("mac1") == Computer("mac1")
         assert Computer("mac1") != Computer("mac2")
         assert Computer("mac1") == "mac1"
         assert "mac1" != Computer("mac2")
@@ -34,24 +35,24 @@
         assert Computer("mac1") < Computer("mac2")
         assert Computer("def") > Computer("ABC")
 
     # TODO: move these to test_models_config.py
 
     def test_get_match_none(self):
         """Verify a computer is added when missing."""
-        other = Computer("name", "hostname", "address", "serial")
+        other = Computer("name", "serial", "address:", "hostname")
         config = ProgramConfig(computers=[other])
         this = config.get_current_computer()
         assert "sample" == this.name
         assert "00:00:00:00:00:00" == this.address
         assert "Sample.local" == this.hostname
         assert 2 == len(config.computers)
 
     def test_get_match_all(self):
         """Verify a computer can be matched exactly."""
-        other = Computer("all", "Sample.local", "00:00:00:00:00:00")
+        other = Computer("all", "serial", "00:00:00:00:00:00", "Sample.local")
         config = ProgramConfig(computers=[other])
         this = config.get_current_computer()
         assert "all" == this.name
         assert "00:00:00:00:00:00" == this.address
         assert "Sample.local" == this.hostname
         assert 1 == len(config.computers)
```

### Comparing `mine-4.0a3/mine/tests/test_models_config.py` & `mine-4.1/mine/tests/test_models_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 @patch("socket.gethostname", Mock(return_value="Sample.local"))
 class TestProgramConfig:
     """Unit tests for the program configuration class."""
 
     config = ProgramConfig(
         applications=[Application("iTunes"), Application("HipChat")],
         computers=[
-            Computer("abc", "abc.local", "1"),
-            Computer("def", "def.local", "2"),
-            Computer("My iMac", "imac.local", "3"),
-            Computer("My Mac", "mac.local", "4"),
+            Computer("abc", "s1", "1:1", "abc.local"),
+            Computer("def", "s2", "2:2", "def.local"),
+            Computer("My iMac", "s3", "3:3", "imac.local"),
+            Computer("My Mac", "s4", "4:4", "mac.local"),
         ],
     )
 
     def test_init(self):
         """Verify a new program configuration is blank."""
         config = ProgramConfig()
         assert not config.applications
@@ -62,22 +62,22 @@
         computer = Computer("", hostname="Jaces-iMac.local")
         name = config.generate_computer_name(computer)
         assert "jaces-imac" == name
 
     def test_generate_name_duplicates(self):
         """Verify a computer name is generated correctly with duplicates."""
         config = ProgramConfig(computers=[Computer("jaces-imac")])
-        computer = Computer("", hostname="Jaces-iMac.local")
+        computer = Computer("", "s", hostname="Jaces-iMac.local")
         name = config.generate_computer_name(computer)
         assert "jaces-imac-2" == name
 
     def test_get_current_computer_by_matching_address(self):
         config = ProgramConfig(
-            computers=[Computer("abc", "foobar", "00:00:00:00:00:00")]
+            computers=[Computer("abc", "s", "00:00:00:00:00:00", "foobar")]
         )
         computer = config.get_current_computer()
         assert "abc" == computer.name
 
     def test_get_current_computer_by_matching_hostname(self):
-        config = ProgramConfig(computers=[Computer("abc", "Sample.local", "foobar")])
+        config = ProgramConfig(computers=[Computer("abc", "s", "a:", "Sample.local")])
         computer = config.get_current_computer()
         assert "abc" == computer.name
```

### Comparing `mine-4.0a3/mine/tests/test_models_data.py` & `mine-4.1/mine/tests/test_models_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,28 +6,41 @@
 from mine.models import Data
 
 
 def describe_data():
     @pytest.fixture
     def data(monkeypatch):
         monkeypatch.setattr(datafiles.settings, "HOOKS_ENABLED", False)
-        return Data()
+        return Data("../../tests/files/mine.yml")
 
     def describe_repr():
-        def it_should_always_be_a_simple_name(data):
+        def it_should_always_be_a_simple_name(data: Data):
             assert "settings" == repr(data)
 
     def describe_modified():
-        def is_false_initially(data):
+        def is_false_initially(data: Data):
             assert False is data.modified
 
-        def is_true_when_the_counter_changes(data):
+        def is_true_when_the_counter_changes(data: Data):
             data.status.counter += 1
 
             assert True is data.modified
 
-        def is_false_after_reading(data):
+        def is_false_after_reading(data: Data):
             data.status.counter += 1
 
             print(data.modified)
 
             assert False is data.modified
+
+    def describe_prune_status():
+        def it_can_preserve_counter(data: Data):
+            data.datafile.load()  # type: ignore
+            assert data.status.counter > 0
+            data.prune_status()
+            assert data.status.counter > 0
+
+        def it_can_reset_counter(data: Data):
+            data.datafile.load()  # type: ignore
+            assert data.status.counter > 0
+            data.prune_status(reset_counter=True)
+            assert data.status.counter == 0
```

### Comparing `mine-4.0a3/mine/tests/test_models_status.py` & `mine-4.1/mine/tests/test_models_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,16 +93,16 @@
         """Verify no app is running when the list is empty."""
         assert False is self.status.is_running(self.application, self.computer)
         assert 0 == self.status.counter
 
     def test_queue(self):
         """Verify queuing an application sets the next computer."""
         self.status.queue(self.application, self.computer)
-        app_status = self.status.find(self.application)
-        assert self.computer.name == app_status.next
+        status = self.status.find(self.application)
+        assert self.computer.name == status.next
 
     def test_start(self):
         """Verify starting an application adds it to the list."""
         self.status.start(self.application, self.computer)
         names = [status.application for status in self.status.applications]
         assert self.application.name in names
         assert 1 == self.status.counter
```

### Comparing `mine-4.0a3/mine/tests/test_models_timestamp.py` & `mine-4.1/mine/tests/test_models_timestamp.py`

 * *Files identical despite different names*

### Comparing `mine-4.0a3/mine/tests/test_services.py` & `mine-4.1/mine/tests/test_services.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,31 +82,33 @@
             touch(tmp_dir, filename)
 
         return tmp_dir
 
     def test_fail_when_leftover_conflicts(self, _, tmpdir):
         root = self._create_conflicts(tmpdir)
 
-        result = services.delete_conflicts(root)
+        count = services.delete_conflicts(root)
 
-        assert False is result
+        assert count == 0
 
     def test_pass_when_no_conflicts(self, _, tmpdir):
         root = self._create_conflicts(tmpdir, count=0)
 
-        result = services.delete_conflicts(root)
+        count = services.delete_conflicts(root)
 
-        assert True is result
+        assert count == 0
 
     def test_no_deletion_without_force(self, mock_remove, tmpdir):
         root = self._create_conflicts(tmpdir)
 
-        services.delete_conflicts(root, force=False)
+        count = services.delete_conflicts(root, force=False)
 
+        assert count == 0
         assert 0 == mock_remove.call_count
 
     def test_deletion_count_is_correct(self, mock_remove, tmpdir):
         root = self._create_conflicts(tmpdir, count=2)
 
-        services.delete_conflicts(root, force=True)
+        count = services.delete_conflicts(root, force=True)
 
+        assert count == 2
         assert 2 == mock_remove.call_count
```

### Comparing `mine-4.0a3/pyproject.toml` & `mine-4.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "mine"
-version = "4.0a3"
+version = "4.1"
 description = "Share application state across computers using Dropbox."
 
 license = "MIT"
 
 authors = ["Jace Browning <jacebrowning@gmail.com>"]
 
 readme = "README.md"
```

### Comparing `mine-4.0a3/PKG-INFO` & `mine-4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mine
-Version: 4.0a3
+Version: 4.1
 Summary: Share application state across computers using Dropbox.
 Home-page: https://pypi.org/project/mine
 License: MIT
 Author: Jace Browning
 Author-email: jacebrowning@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

