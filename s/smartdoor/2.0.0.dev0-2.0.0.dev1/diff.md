# Comparing `tmp/smartdoor-2.0.0.dev0.tar.gz` & `tmp/smartdoor-2.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartdoor-2.0.0.dev0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "smartdoor-2.0.0.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `smartdoor-2.0.0.dev0.tar` & `smartdoor-2.0.0.dev1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1839 2023-05-19 06:36:25.675356 smartdoor-2.0.0.dev0/.gitignore
--rw-r--r--   0        0        0     1136 2023-05-18 06:25:36.917565 smartdoor-2.0.0.dev0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1512 2023-05-17 14:36:57.361107 smartdoor-2.0.0.dev0/LICENSE.md
--rw-r--r--   0        0        0      723 2023-05-19 06:47:07.059427 smartdoor-2.0.0.dev0/README.md
--rw-r--r--   0        0        0     1786 2023-05-19 03:24:13.739873 smartdoor-2.0.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     3632 2023-05-19 06:36:04.938451 smartdoor-2.0.0.dev0/smartdoor/__init__.py
--rw-r--r--   0        0        0      180 2023-05-17 14:44:02.403787 smartdoor-2.0.0.dev0/smartdoor/core/__init__.py
--rw-r--r--   0        0        0     3208 2023-05-19 04:53:42.692678 smartdoor-2.0.0.dev0/smartdoor/core/authenticate.py
--rw-r--r--   0        0        0     4932 2023-05-19 04:53:42.672677 smartdoor-2.0.0.dev0/smartdoor/core/smartlock.py
--rw-r--r--   0        0        0     2081 2023-05-17 12:16:39.347238 smartdoor-2.0.0.dev0/smartdoor/default_config.toml
--rw-r--r--   0        0        0      794 2023-05-19 06:31:54.619552 smartdoor-2.0.0.dev0/smartdoor/logging.conf
--rw-r--r--   0        0        0     8740 2023-05-19 04:58:29.569525 smartdoor-2.0.0.dev0/smartdoor/smartdoor.py
--rw-r--r--   0        0        0     1941 1970-01-01 00:00:00.000000 smartdoor-2.0.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1839 2023-05-19 06:36:25.675356 smartdoor-2.0.0.dev1/.gitignore
+-rw-r--r--   0        0        0     1136 2023-05-18 06:25:36.917565 smartdoor-2.0.0.dev1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1512 2023-05-17 14:36:57.361107 smartdoor-2.0.0.dev1/LICENSE.md
+-rw-r--r--   0        0        0     2025 2023-07-22 10:51:48.525680 smartdoor-2.0.0.dev1/README.md
+-rw-r--r--   0        0        0     1861 2023-07-22 10:50:43.482784 smartdoor-2.0.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     6155 2023-07-22 10:50:18.729682 smartdoor-2.0.0.dev1/smartdoor/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-17 14:44:02.403787 smartdoor-2.0.0.dev1/smartdoor/core/__init__.py
+-rw-r--r--   0        0        0     3244 2023-05-20 08:34:52.724385 smartdoor-2.0.0.dev1/smartdoor/core/authenticate.py
+-rw-r--r--   0        0        0     4968 2023-05-20 08:34:48.408198 smartdoor-2.0.0.dev1/smartdoor/core/smartlock.py
+-rw-r--r--   0        0        0     2065 2023-07-22 10:47:46.218895 smartdoor-2.0.0.dev1/smartdoor/default_config.toml
+-rw-r--r--   0        0        0      794 2023-05-19 06:31:54.619552 smartdoor-2.0.0.dev1/smartdoor/logging.conf
+-rw-r--r--   0        0        0     8775 2023-07-22 08:42:24.603572 smartdoor-2.0.0.dev1/smartdoor/smartdoor.py
+-rw-r--r--   0        0        0      222 2023-07-21 04:14:11.966183 smartdoor-2.0.0.dev1/smartdoor/smartdoor.service
+-rw-r--r--   0        0        0     3346 1970-01-01 00:00:00.000000 smartdoor-2.0.0.dev1/PKG-INFO
```

### Comparing `smartdoor-2.0.0.dev0/.gitignore` & `smartdoor-2.0.0.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev0/.pre-commit-config.yaml` & `smartdoor-2.0.0.dev1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev0/LICENSE.md` & `smartdoor-2.0.0.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev0/pyproject.toml` & `smartdoor-2.0.0.dev1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Operating System :: POSIX :: Linux",
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Home Automation",
     "Topic :: Security",
 ]
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 dependencies = [
     "rich-click",
     "requests",
     "nfcpy",
     "gpiozero",
     'tomli; python_version < "3.11"',
 ]
@@ -42,15 +44,15 @@
 [project.urls]
 Home = "https://github.com/munechika-koyo/smartdoor"
 
 [project.scripts]
 smartdoor = "smartdoor:cli"
 
 [tool.flit.sdist]
-exclude = ["doc/", "serviceConfig/"]
+exclude = ["doc/"]
 
 [tool.black]
 line-length = 100
 
 [tool.ruff]
 line-length = 100
```

### Comparing `smartdoor-2.0.0.dev0/smartdoor/__init__.py` & `smartdoor-2.0.0.dev1/smartdoor/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Smartdoor system including NFC card detecting, key locking/unlocking, turning LED on/off, etc.
 
 This system is designed to be used with Raspberry Pi.
 
 Some CLIs including main sequence is implemented here.
 """
+from __future__ import annotations
+
+import subprocess
 from logging import config as log_config
 from logging import getLogger
 from pathlib import Path
 from pprint import pformat
 
 import rich_click as click
 
@@ -18,15 +21,15 @@
 try:
     import tomllib
 except ImportError:
     import tomli as tomllib
 
 from .smartdoor import SmartDoor
 
-__version__ = "2.0.0.dev0"
+__version__ = "2.0.0.dev1"
 __all__ = ["SmartDoor"]
 
 
 @click.group(context_settings=dict(help_option_names=["-h", "--help"]))
 @click.version_option(__version__, "-V", "--version")
 def cli():
     """Smartdoor system CLI."""
@@ -36,15 +39,16 @@
 @cli.command()
 @click.option(
     "--locked/--unlocked", default=True, show_default=True, help="Set initial key status."
 )
 def start(locked: bool):
     """Start SmartDoor system.
 
-    The initial key status can be set by `--locked` or `--unlocked` option, by default `--locked`.
+    The infinite loop workflow is executed at foreground. The initial key status can be set by
+    `--locked` or `--unlocked` option, by default `--locked`.
 
     If you want to stop this system, press Ctrl+C.
     """
     # Instantiate SmartDoor
     logger.info("start smartdoor system")
     door = SmartDoor()
 
@@ -102,28 +106,81 @@
     if log.exists():
         click.echo(log.read_text())
     else:
         click.echo("log file not found.")
 
 
 @cli.command()
-def show_config():
-    """Show configuation in key-value format.
+@click.option("--show", is_flag=True, help="show current configuration parameters")
+@click.option(
+    "--generate", is_flag=True, help="generate default config file as ~/.config/smartdoor.toml"
+)
+def config(show: bool, generate: bool):
+    """Configuration tool for SmartDoor system.
 
-    If user-specific config exists at `~/.config/smartdoor.toml`, overrided one is shown.
+    If you want to configure smartdoor system, edit `~/.config/smartdoor.toml` directly, after
+    generating default config file by `--generate` option.
     """
     # Load default configuration file
-    with open(Path(__file__).parent / "default_config.toml", "rb") as file:
+    default_config_path = Path(__file__).parent / "default_config.toml"
+    with default_config_path.open("rb") as file:
         config = tomllib.load(file)
 
     # Load user-specific configuration file if exists
     config_path = Path.home() / ".config" / "smartdoor.toml"
     if config_path.exists():
-        with open(config_path, "rb") as file:
+        with config_path.open("rb") as file:
             config.update(tomllib.load(file))
 
+    # If config file not found and `--generate` option is specified, generate default config file
+    if generate and not config_path.exists():
+        config_path.parent.mkdir(parents=True, exist_ok=True)
+        with config_path.open("w") as file:
+            file.write(default_config_path.read_text())
+        click.echo(f"generated default config file as {config_path}")
+
     # Show configuation
-    click.echo(pformat(config))
+    elif show:
+        click.echo(pformat(config))
+    else:
+        click.echo("please specify `--show` or `--generate` option")
+
+
+@cli.command()
+@click.option("--register", is_flag=True, help="register service to systemd and start it")
+@click.option("--unregister", is_flag=True, help="unregister service from systemd")
+@click.option("--start", is_flag=True, help="start service")
+@click.option("--stop", is_flag=True, help="stop service")
+def service(register: bool, unregister: bool, start: bool, stop: bool):
+    """Systemd Service tool for SmartDoor system.
+
+    If you want to register/unregister smartdoor system to/from systemd, use `--register` or
+    `--unregister` option. If choose `--register` option, smartdoor system will be started.
+    """
+    if register:
+        service_file = Path(__file__).parent / "smartdoor.service"
+        subprocess.run(
+            ["sudo", "ln", "-s", str(service_file), "/etc/systemd/system/smartdoor.service"]
+        )
+        subprocess.run(["sudo", "systemctl", "daemon-reload"])
+        subprocess.run(["sudo", "systemctl", "enable", "smartdoor.service"])
+        click.echo("registered service to systemd")
+
+    elif unregister:
+        subprocess.run(["sudo", "systemctl", "stop", "smartdoor.service"])
+        subprocess.run(["sudo", "systemctl", "disable", "smartdoor.service"])
+        click.echo("unregistered service from systemd")
+
+    elif start:
+        subprocess.run(["sudo", "systemctl", "start", "smartdoor.service"])
+        click.echo("started service")
+
+    elif stop:
+        subprocess.run(["sudo", "systemctl", "stop", "smartdoor.service"])
+        click.echo("stopped service")
+
+    else:
+        click.echo("please specify `--register` or `--unregister` option")
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `smartdoor-2.0.0.dev0/smartdoor/core/authenticate.py` & `smartdoor-2.0.0.dev1/smartdoor/core/authenticate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """This module provides IDm authentication functions communicating with database through web api."""
+from __future__ import annotations
+
 import sys
 from logging import getLogger
 
 from requests import Request, Session
 
 module_logger = getLogger(__name__)
```

### Comparing `smartdoor-2.0.0.dev0/smartdoor/core/smartlock.py` & `smartdoor-2.0.0.dev1/smartdoor/core/smartlock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Module for SmartLock class."""
+from __future__ import annotations
+
 from logging import getLogger
 from time import sleep
 
 from gpiozero import LED, Button, Buzzer, Device, Servo
 
 module_logger = getLogger(__name__)
```

### Comparing `smartdoor-2.0.0.dev0/smartdoor/default_config.toml` & `smartdoor-2.0.0.dev1/smartdoor/default_config.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# Smartdoor Default Configuration File
-# ======================================
+# Smartdoor Configuration File
+# ============================
 # This file is used to set default configuration of smartdoor system.
-# The user-specific configuration should be written in ~/.config/smartdoor.toml file which is
-# automatically loaded after this file and overrides the default configuration.
+# You can change the configuration by editing this file.
 #
 # -------------------------------------------------------------------
 # Smartdoor host authentication URL.
 # - Note:
 #   Smartdoor host deploys website where NFC keys can be registered,
 #   manages stored keys data, and provides authentication API.
 #   (see https://github.com/munechika-koyo/smartdoor_host)
@@ -20,29 +19,31 @@
 #   smartdoor host must have the Allow_"room" attribute (e.g. Allow_N2_423)
 # -------------------------------------------------------------------
 room = "423"
 
 # -------------------------------------------------------------------
 # Pin Assignment
 # - Note:
-#   Rasberry-pi's GPIO pin must be the number of PIN, not GPIO number.
+#   smartdoor uses Broadcom (BCM) pin numbering for the GPIO pins.
+#   For example, if you use a "GPIO2" as an button input pin,
+#   you should set "button = 2" in the [pins] section.
 # -------------------------------------------------------------------
 [pins]
-button = 10  # input from push button
-LED_red = 5   # output to red LED
-LED_green = 7  # output to green LED
-LED_button = 13  # output to push button LED
-buzzer = 11  # output to buzzer
-servo = 3  # output to servomotor
+button = 25  # input from push button
+LED_red = 17   # output to red LED
+LED_green = 27  # output to green LED
+LED_button = 24  # output to push button LED
+buzzer = 5  # output to buzzer
+servo = 12  # output to servomotor
 
 
 # -------------------------------------------------------------------
 # IFTTT POST URLs
 # - Note:
 #   Post values to IFTTT Webhooks to trigger events are
 #   "value1": "date"  # (e.g. "2021/06/21 12:00:00")
 #   "value2": "username"  # (e.g. "unknown")
 #   "value3": "action"  # (e.g. "LOCK")
 # -------------------------------------------------------------------
 [IFTTT_URLs]
-url1 = "https://maker.ifttt.com/trigger/{event1}/with/key/{your_key}"
-url2 = "https://maker.ifttt.com/trigger/{event2}/with/key/{your_key}"
+# url1 = "https://maker.ifttt.com/trigger/{event1}/with/key/{your_key}"
+# url2 = "https://maker.ifttt.com/trigger/{event2}/with/key/{your_key}"
```

### Comparing `smartdoor-2.0.0.dev0/smartdoor/logging.conf` & `smartdoor-2.0.0.dev1/smartdoor/logging.conf`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev0/smartdoor/smartdoor.py` & `smartdoor-2.0.0.dev1/smartdoor/smartdoor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """This module provides a main class of SmartDoor system."""
+from __future__ import annotations
+
 from binascii import hexlify
 from collections import deque
 from datetime import datetime
 from logging import getLogger
 from pathlib import Path
 from time import sleep
 
@@ -41,15 +43,15 @@
         # Load default configuration file
         with open(Path(__file__).parent / "default_config.toml", "rb") as file:
             config = tomllib.load(file)
 
         # Load user-specific configuration file if exists
         config_path = Path.home() / ".config" / "smartdoor.toml"
         if config_path.exists():
-            with open(config_path, "rb") as file:
+            with config_path.open("rb") as file:
                 config.update(tomllib.load(file))
                 self.logger.debug(f"Loaded user-specific configuration file: {config_path}")
 
         # === Initialization ==================================================
         # IFTTT
         self._urls: dict[str, str] = {}
         self.urls = config["IFTTT_URLs"]
```

