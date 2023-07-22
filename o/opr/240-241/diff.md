# Comparing `tmp/opr-240.tar.gz` & `tmp/opr-241.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opr-240.tar", last modified: Mon Jul 17 05:58:43 2023, max compression
+gzip compressed data, was "opr-241.tar", last modified: Sat Jul 22 13:22:38 2023, max compression
```

## Comparing `opr-240.tar` & `opr-241.tar`

### file list

```diff
@@ -1,55 +1,44 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-17 05:58:43.156785 opr-240/
--rw-r--r--   0 bart      (1000) bart      (1000)     2593 2023-07-17 05:58:43.156785 opr-240/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     2029 2023-07-15 21:11:27.000000 opr-240/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-17 05:58:43.152785 opr-240/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1000)     1990 2023-07-17 04:56:56.000000 opr-240/bin/opr
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-17 05:58:43.152785 opr-240/opr/
--rw-r--r--   0 bart      (1000) bart      (1000)     1725 2023-07-17 04:55:54.000000 opr-240/opr/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1021 2023-07-17 04:55:54.000000 opr-240/opr/brokers.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1952 2023-07-17 04:55:54.000000 opr-240/opr/command.py
--rw-r--r--   0 bart      (1000) bart      (1000)      284 2023-07-17 04:55:54.000000 opr-240/opr/configs.py
--rw-r--r--   0 bart      (1000) bart      (1000)      938 2023-07-17 04:55:54.000000 opr-240/opr/decoder.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1558 2023-07-17 04:55:54.000000 opr-240/opr/encoder.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1248 2023-07-17 04:55:54.000000 opr-240/opr/errored.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1158 2023-07-17 04:55:54.000000 opr-240/opr/evented.py
--rw-r--r--   0 bart      (1000) bart      (1000)      353 2023-07-17 04:55:54.000000 opr-240/opr/locking.py
--rw-r--r--   0 bart      (1000) bart      (1000)      802 2023-07-17 04:55:54.000000 opr-240/opr/loggers.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-17 05:58:43.156785 opr-240/opr/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      380 2023-07-17 04:56:00.000000 opr-240/opr/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3528 2023-07-17 04:56:00.000000 opr-240/opr/modules/bsc.py
--rw-r--r--   0 bart      (1000) bart      (1000)    19192 2023-07-17 04:56:00.000000 opr-240/opr/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      829 2023-07-17 04:56:00.000000 opr-240/opr/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4057 2023-07-17 04:56:00.000000 opr-240/opr/modules/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17641 2023-07-17 04:56:00.000000 opr-240/opr/modules/mdl.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2401 2023-07-17 04:56:00.000000 opr-240/opr/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)     7441 2023-07-17 04:56:00.000000 opr-240/opr/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1036 2023-07-17 04:56:00.000000 opr-240/opr/modules/shp.py
--rw-r--r--   0 bart      (1000) bart      (1000)      998 2023-07-17 04:56:00.000000 opr-240/opr/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2664 2023-07-17 04:56:00.000000 opr-240/opr/modules/udp.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5754 2023-07-17 04:56:00.000000 opr-240/opr/modules/wsd.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1009 2023-07-17 04:56:00.000000 opr-240/opr/modules/wsh.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5069 2023-07-17 04:55:54.000000 opr-240/opr/objects.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1297 2023-07-17 04:55:54.000000 opr-240/opr/parsers.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4332 2023-07-17 04:55:54.000000 opr-240/opr/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2174 2023-07-17 04:55:54.000000 opr-240/opr/reactor.py
--rw-r--r--   0 bart      (1000) bart      (1000)      928 2023-07-17 04:55:54.000000 opr-240/opr/recurse.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1246 2023-07-17 04:55:54.000000 opr-240/opr/repeats.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1873 2023-07-17 04:55:54.000000 opr-240/opr/threads.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2153 2023-07-17 04:55:54.000000 opr-240/opr/utility.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-17 05:58:43.156785 opr-240/opr.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     2593 2023-07-17 05:58:43.000000 opr-240/opr.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      848 2023-07-17 05:58:43.000000 opr-240/opr.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-07-17 05:58:43.000000 opr-240/opr.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        7 2023-07-17 05:58:43.000000 opr-240/opr.egg-info/requires.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        4 2023-07-17 05:58:43.000000 opr-240/opr.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)     1131 2023-07-15 21:11:01.000000 opr-240/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-07-17 05:58:43.156785 opr-240/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      206 2023-07-15 21:11:56.000000 opr-240/setup.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-17 05:58:43.156785 opr-240/test/
--rw-r--r--   0 bart      (1000) bart      (1000)      748 2023-07-15 21:13:01.000000 opr-240/test/test_composite.py
--rw-r--r--   0 bart      (1000) bart      (1000)      504 2023-07-15 21:13:12.000000 opr-240/test/test_decoder.py
--rw-r--r--   0 bart      (1000) bart      (1000)      463 2023-07-15 21:13:25.000000 opr-240/test/test_encoder.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1009 2023-07-15 21:13:43.000000 opr-240/test/test_inherit.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4414 2023-07-15 21:14:03.000000 opr-240/test/test_objects.py
--rw-r--r--   0 bart      (1000) bart      (1000)      427 2023-07-15 21:14:15.000000 opr-240/test/test_parse.py
--rw-r--r--   0 bart      (1000) bart      (1000)      670 2023-07-15 21:14:39.000000 opr-240/test/test_recursive.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-22 13:22:38.746986 opr-241/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2896 2023-07-22 13:22:38.746986 opr-241/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     2332 2023-07-20 05:20:09.000000 opr-241/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-22 13:22:38.742986 opr-241/opr/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1697 2023-07-21 16:25:39.000000 opr-241/opr/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2470 2023-07-21 16:29:53.000000 opr-241/opr/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      963 2023-07-21 16:17:50.000000 opr-241/opr/brokers.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1969 2023-07-21 16:17:59.000000 opr-241/opr/command.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      226 2023-07-21 16:18:06.000000 opr-241/opr/configs.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      899 2023-07-21 16:18:14.000000 opr-241/opr/decoder.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1577 2023-07-21 16:18:22.000000 opr-241/opr/encoder.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1190 2023-07-21 16:18:31.000000 opr-241/opr/errored.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1099 2023-07-21 16:18:39.000000 opr-241/opr/evented.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      295 2023-07-21 16:18:47.000000 opr-241/opr/locking.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      461 2023-07-21 16:18:56.000000 opr-241/opr/loggers.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-22 13:22:38.746986 opr-241/opr/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      373 2023-07-21 16:39:23.000000 opr-241/opr/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3531 2023-07-21 16:19:16.000000 opr-241/opr/modules/bsc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    19208 2023-07-21 16:19:31.000000 opr-241/opr/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      771 2023-07-21 16:19:40.000000 opr-241/opr/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5170 2023-07-21 16:19:49.000000 opr-241/opr/modules/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     7408 2023-07-21 16:20:15.000000 opr-241/opr/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      951 2023-07-21 16:20:23.000000 opr-241/opr/modules/shp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      940 2023-07-21 16:20:31.000000 opr-241/opr/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2933 2023-07-21 16:20:39.000000 opr-241/opr/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      951 2023-07-21 16:20:59.000000 opr-241/opr/modules/wsh.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5060 2023-07-21 16:21:20.000000 opr-241/opr/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1277 2023-07-21 16:21:29.000000 opr-241/opr/parsers.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3849 2023-07-21 16:21:38.000000 opr-241/opr/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2158 2023-07-21 16:21:46.000000 opr-241/opr/reactor.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      869 2023-07-21 16:21:55.000000 opr-241/opr/recurse.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1260 2023-07-21 16:22:06.000000 opr-241/opr/repeats.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1815 2023-07-21 16:22:17.000000 opr-241/opr/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2501 2023-07-21 16:22:30.000000 opr-241/opr/utility.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-07-22 13:22:38.742986 opr-241/opr.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2896 2023-07-22 13:22:38.000000 opr-241/opr.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      680 2023-07-22 13:22:38.000000 opr-241/opr.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-07-22 13:22:38.000000 opr-241/opr.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       45 2023-07-22 13:22:38.000000 opr-241/opr.egg-info/entry_points.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        7 2023-07-22 13:22:38.000000 opr-241/opr.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        4 2023-07-22 13:22:38.000000 opr-241/opr.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)     1054 2023-07-22 07:36:16.000000 opr-241/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-07-22 13:22:38.746986 opr-241/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      101 2023-07-17 16:14:42.000000 opr-241/setup.py
```

### Comparing `opr-240/PKG-INFO` & `opr-241/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 Metadata-Version: 2.1
 Name: opr
-Version: 240
+Version: 241
 Summary: Object Programming Runtime
 Author-email: Bart Thate <programmingobject@gmail.com>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/opr
 Project-URL: bugs, https://github.com/bthate/opr/issues
 Project-URL: source, https://github.com/bthate/opr
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Topic :: Utilities
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 
-# This file is placed in the Public Domain.
-#
-# __author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 NAME
 
 ::
 
    OPR - Object Programming Runtime
 
 
@@ -62,47 +57,47 @@
 USAGE
 
 
 ::
 
     list of commands
 
-    $ opr cmd
-    cmd,err,flt,sts,thr,upt
+        $ opr cmd
+        cmd,err,flt,sts,thr,upt
 
     start a console
 
-    $ opr -c
-    >
+        $ opr -c
+        >
 
     start additional modules
 
-    $ opr mod=<mod1,mod2> -c
-    >
+        $ opr mod=<mod1,mod2> -c
+        >
 
     list of modules
 
-    $ opr mod
-    cmd,err,flt,fnd,irc,log,mdl,mod,
-    req, rss,slg,sts,tdo,thr,upt,ver
+        $ opr mod
+        cmd,err,flt,fnd,irc,log,mdl,mod,
+        req, rss,slg,sts,tdo,thr,upt,ver
 
     to start irc, add mod=irc when
     starting
 
-    $ opr mod=irc -c
+        $ opr mod=irc -c
 
     to start rss, also add mod=rss
     when starting
 
-    $ opr mod=irc,rss -c
+        $ opr mod=irc,rss -c
 
     start as daemon
 
-    $ opr  mod=irc,rss -d
-    $ 
+        $ opr  mod=irc,rss -d
+        $ 
 
 
 CONFIGURATION
 
 
 ::
 
@@ -144,14 +139,37 @@
     pwd - sasl nickserv name/pass
     rem - removes a rss feed
     rss - add a feed
     slg - slogan
     thr - show the running threads
 
 
+SYSTEMD
+
+::
+
+ [Unit]
+ Description=Object Programming Runtime
+ Requires=network.target
+ After=network.target
+
+ [Service]
+ DynamicUser=True
+ Type=fork
+ User=bart
+ Group=bart
+ PIDFile=opr.pid
+ WorkingDirectory=/home/bart/.opr
+ ExecStart=/home/bart/.local/pipx/venvs/opr/bin/opr mod=irc,rss,mdl -d
+ RemainAfterExit=yes
+
+ [Install]
+ WantedBy=multi-user.target
+
+
 FILES
 
 ::
 
     ~/.local/bin/opr
     ~/.local/pipx/venvs/opr/
```

### Comparing `opr-240/README.rst` & `opr-241/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-# This file is placed in the Public Domain.
-#
-# __author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 NAME
 
 ::
 
    OPR - Object Programming Runtime
 
 
@@ -45,47 +40,47 @@
 USAGE
 
 
 ::
 
     list of commands
 
-    $ opr cmd
-    cmd,err,flt,sts,thr,upt
+        $ opr cmd
+        cmd,err,flt,sts,thr,upt
 
     start a console
 
-    $ opr -c
-    >
+        $ opr -c
+        >
 
     start additional modules
 
-    $ opr mod=<mod1,mod2> -c
-    >
+        $ opr mod=<mod1,mod2> -c
+        >
 
     list of modules
 
-    $ opr mod
-    cmd,err,flt,fnd,irc,log,mdl,mod,
-    req, rss,slg,sts,tdo,thr,upt,ver
+        $ opr mod
+        cmd,err,flt,fnd,irc,log,mdl,mod,
+        req, rss,slg,sts,tdo,thr,upt,ver
 
     to start irc, add mod=irc when
     starting
 
-    $ opr mod=irc -c
+        $ opr mod=irc -c
 
     to start rss, also add mod=rss
     when starting
 
-    $ opr mod=irc,rss -c
+        $ opr mod=irc,rss -c
 
     start as daemon
 
-    $ opr  mod=irc,rss -d
-    $ 
+        $ opr  mod=irc,rss -d
+        $ 
 
 
 CONFIGURATION
 
 
 ::
 
@@ -127,14 +122,37 @@
     pwd - sasl nickserv name/pass
     rem - removes a rss feed
     rss - add a feed
     slg - slogan
     thr - show the running threads
 
 
+SYSTEMD
+
+::
+
+ [Unit]
+ Description=Object Programming Runtime
+ Requires=network.target
+ After=network.target
+
+ [Service]
+ DynamicUser=True
+ Type=fork
+ User=bart
+ Group=bart
+ PIDFile=opr.pid
+ WorkingDirectory=/home/bart/.opr
+ ExecStart=/home/bart/.local/pipx/venvs/opr/bin/opr mod=irc,rss,mdl -d
+ RemainAfterExit=yes
+
+ [Install]
+ WantedBy=multi-user.target
+
+
 FILES
 
 ::
 
     ~/.local/bin/opr
     ~/.local/pipx/venvs/opr/
```

### Comparing `opr-240/bin/opr` & `opr-241/opr/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-#!/usr/bin/env python3
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C,I,R
+# flake8: noqa=E402
 
 
-"object programming runtime"
-
-
-__author__ = "Bart Thate <programmingobject@gmail.com>"
+"runtime"
 
 
 import os
 import readline
 import sys
 import termios
 import _thread
 
 
 sys.path.insert(0, os.getcwd())
 
 
-from opr import Broker, Cfg, Command, Event, Logging, Persist, Reactor
-from opr import banner, parse, scan, waiter
-from opr import modules
+from . import Cfg
 
 
 Cfg.mod = "bsc"
-Cfg.name = "opr"
+Cfg.name = __file__.split(os.sep)[-2]
 Cfg.verbose = False
-Cfg.version = 20
+Cfg.version = 241
+
 
+from . import Broker, Command, Event, Logging, Persist, Reactor
+from . import banner, parse, scan, wait, waiter
+from . import modules
 
-Persist.workdir = os.path.expanduser("~/.{Cfg.name}")
+
+Persist.workdir = os.path.expanduser(f"~/.{Cfg.name}")
 
 
 readline.redisplay()
 
 
 class CLI(Reactor):
 
     def __init__(self):
         Reactor.__init__(self)
         Broker.add(self)
         self.register("event", Command.handle)
 
     def announce(self, txt):
-        self.raw(txt)
+        pass
 
     def raw(self, txt):
         print(txt)
 
 
 class Console(CLI):
 
@@ -67,14 +67,28 @@
             _thread.interrupt_main()
 
 def cprint(txt):
     print(txt)
     sys.stdout.flush()
 
 
+def daemon():
+    pid = os.fork()
+    if pid != 0:
+        os._exit(0)
+    os.setsid()
+    os.umask(0)
+    sis = open('/dev/null', 'r', encoding="utf-8")
+    os.dup2(sis.fileno(), sys.stdin.fileno())
+    sos = open('/dev/null', 'a+', encoding="utf-8")
+    ses = open('/dev/null', 'a+', encoding="utf-8")
+    os.dup2(sos.fileno(), sys.stdout.fileno())
+    os.dup2(ses.fileno(), sys.stderr.fileno())
+
+
 def wrap(func) -> None:
     old = termios.tcgetattr(sys.stdin.fileno())
     try:
         func()
     except (EOFError, KeyboardInterrupt):
         print("")
         sys.stdout.flush()
@@ -84,24 +98,32 @@
 
 
 def main():
     parse(Cfg, " ".join(sys.argv[1:]))
     if "v" in Cfg.opts:
         Logging.raw = print
         Logging.verbose = True
-    if "c" in Cfg.opts:
+    if "d" in Cfg.opts:
+        daemon()
+        scan(modules, Cfg.mod, True, "a" in Cfg.opts)
+        wait()
+    elif "c" in Cfg.opts:
         print(banner(Cfg.name, Cfg.version))
         csl = Console()
         scan(modules, Cfg.mod, True, "a" in Cfg.opts)
         csl.loop()
     else:
         cli = CLI()
-        scan(modules, Cfg.mod, False, True)
+        scan(modules, Cfg.mod)
         evt = Event()
         evt.orig = repr(cli)
-        evt.txt = Cfg.txt
+        evt.txt = Cfg.otxt
         Command.handle(evt)
 
 
-if __name__ == "__main__":
+def wrapped():
     wrap(main)
     waiter()
+
+
+if __name__ == "__main__":
+    wrapped()
```

### Comparing `opr-240/opr/__init__.py` & `opr-241/opr/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C,I,R,W0401,W0614
+# flake8: noqa=F401
 
 
-"object programming runtime"
-
-
-__author__ = "Bart Thate <programmingobject@gmail.com>"
+"main package"
 
 
 from .command import Command, scan
 from .configs import Cfg
 from .decoder import load, loads
 from .encoder import dump, dumps
 from .errored import Error, Errors, waiter
@@ -18,22 +16,20 @@
 from .loggers import Logging
 from .objects import *
 from .parsers import parse
 from .persist import Persist, find, fntime, last, read, write
 from .reactor import Reactor
 from .repeats import Repeater
 from .threads import launch
-from .utility import banner, laps, spl
+from .utility import banner, laps, spl, wait
 
 
 from .brokers import Broker
 
-
-from . import modules
-
+from . import configs
 
 def __dir__():
     return (
             "Broker",
             "Cfg",
             'Command',
             "Error",
@@ -54,14 +50,15 @@
             'load',
             'loads',
             'modules',
             "parse",
             "read",
             "scan",
             "spl",
+            "wait",
             "waiter",
             "write"
            )
 
 
 def __dir2__():
     return (
```

### Comparing `opr-240/opr/brokers.py` & `opr-241/opr/brokers.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 #
 # pylint: disable=C,I,R
 
 
 "object brokers"
 
 
-__author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 from .objects import Object
 
 
 def __dir__():
     return (
             "Broker",
            )
```

### Comparing `opr-240/opr/command.py` & `opr-241/opr/command.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 #
 # pylint: disable=C,I,R,W0718,E0402
 
 
 "commands"
 
 
-__author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 import inspect
 import os
 
 
 from .errored import Errors
 from .objects import Object, get
 from .parsers import parse
@@ -30,15 +27,14 @@
 __all__ = __dir__()
 
 
 class Command(Object):
 
     cmds = Object()
 
-
     @staticmethod
     def add(func):
         Command.cmds[func.__name__] = func
 
     @staticmethod
     def handle(evt):
         if "txt" in evt:
@@ -68,15 +64,19 @@
             if 'event' in cmd.__code__.co_varnames:
                 Command.add(cmd)
 
 
 def scan(pkg, mods, init=None, doall=False, wait=False) -> None:
     path = pkg.__path__[0]
     if doall:
-        modlist = [x[:-3] for x in os.listdir(path) if x.endswith(".py") and x not in [ "__init__.py", "__main__.py"]]
+        modlist = [
+                   x[:-3] for x in os.listdir(path)
+                   if x.endswith(".py")
+                   and x not in ["__init__.py", "__main__.py"]
+                  ]
         mods = ",".join(sorted(modlist))
     threads = []
     for modname in spl(mods):
         module = getattr(pkg, modname, None)
         if module:
             Command.scan(module)
         if init and "start" in dir(module):
```

### Comparing `opr-240/opr/decoder.py` & `opr-241/opr/decoder.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C,I,R,E0402
+# flake8: noqa=C901
 
 
 "deconding objects"
 
 
-__author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 import json
 
 
 from .objects import Object
 
 
 def __dir__():
@@ -22,15 +20,14 @@
             'loads',
            )
 
 
 __all__ = __dir__()
 
 
-
 class ObjectDecoder(json.JSONDecoder):
 
     def __init__(self, *args, **kwargs):
         ""
         json.JSONDecoder.__init__(self, *args, **kwargs)
 
     def decode(self, s, _w=None):
@@ -41,13 +38,13 @@
         return Object(val)
 
     def raw_decode(self, s, idx=0):
         ""
         return json.JSONDecoder.raw_decode(self, s, idx)
 
 
-def load(fpt, *args, **kw) :
-    return json.load(fpt, *args, cls=ObjectDecoder, **kw)
+def load(fpt, *args, **kw):
+    return json.load(fpt, *args, cls=ObjectDecoder, **kw )
 
 
 def loads(string, *args, **kw):
     return json.loads(string, *args, cls=ObjectDecoder, **kw)
```

### Comparing `opr-240/opr/encoder.py` & `opr-241/opr/encoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 #
 # pylint: disable=C,I,R
 
 
 "encoding objects"
 
 
-__author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 import json
 
 
 from .objects import Object
 
 
 def __dir__():
@@ -56,15 +53,19 @@
         except TypeError:
             return str(o)
 
     def encode(self, o) -> str:
         ""
         return json.JSONEncoder.encode(self, o)
 
-    def iterencode(self, o, _one_shot=False) -> str:
+    def iterencode(
+                   self,
+                   o,
+                   _one_shot=False
+                  ) -> str:
         ""
         return json.JSONEncoder.iterencode(self, o, _one_shot)
 
 
 def dump(*args, **kw) -> None:
     kw["cls"] = ObjectEncoder
     return json.dump(*args, **kw)
```

### Comparing `opr-240/opr/errored.py` & `opr-241/opr/errored.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 #
 # pylint: disable=C,I,R
 
 
 "error handling"
 
 
-__author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 import io
 import traceback
 
 
 from .loggers import Logging
 from .objects import Object
```

### Comparing `opr-240/opr/evented.py` & `opr-241/opr/evented.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 #
 # pylint: disable=C,I,R,E0402
 
 
 "events happen"
 
 
-__author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 import threading
 
 
 from .brokers import Broker
 from .objects import Object
 from .parsers import parse
 
@@ -22,15 +19,14 @@
             "Event",
            )
 
 
 __all__ = __dir__()
 
 
-
 class Event(Object):
 
     __slots__ = ('_ready', '_thr')
 
     def __init__(self, *args, **kwargs):
         Object.__init__(self, *args, **kwargs)
         self._ready = threading.Event()
```

### Comparing `opr-240/opr/modules/bsc.py` & `opr-241/opr/modules/bsc.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 #
 # pylint: disable=C,I,R,W0401
 
 
 "basic commands"
 
 
-__author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 import io
 import os
 import threading
 import time
 import traceback
 
 
@@ -71,15 +68,19 @@
         pass
     event.reply(' | '.join([name(obj) for obj in Broker.objs]))
 
 
 def mod(event):
     from .. import modules
     path = modules.__path__[0]
-    modlist = [x[:-3] for x in os.listdir(path) if x.endswith(".py") and x not in ["__main__.py", "__init__.py"]]
+    modlist = [
+               x[:-3] for x in os.listdir(path)
+               if x.endswith(".py")
+               and x not in ["__main__.py", "__init__.py"]
+              ]
     mods = ",".join(sorted(modlist))
     event.reply(mods)
 
 
 def rld(event):
     if not event.args:
         event.reply("rld <modname>")
```

### Comparing `opr-240/opr/modules/irc.py` & `opr-241/opr/modules/irc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C,I,R,W0401
+# flake8: noqa=C901
 
 
 "internet relay chat"
 
 
-__author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 import base64
 import os
 import queue
 import random
 import socket
 import ssl
 import time
 import textwrap
 import threading
 
 
 from .. import Broker, Cfg, Command, Errors, Event, Logging, Object, Reactor
 from .. import edit, find, fntime, keys, laps, last, prt, write
-from .. import launch, parse, update
+from .. import launch, update
 
 
 from ..locking import saylock
 
 
 def start():
     irc = IRC()
@@ -326,15 +324,14 @@
     def logon(self, server, nck):
         self.events.connected.wait()
         self.events.authed.wait()
         nck = self.cfg.username
         self.command(f'NICK {nck}')
         self.command(f'USER {nck} {server} {server} {nck}')
 
-
     def parsing(self, txt):
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
         rawstr = rawstr.replace('\001', '')
         Logging.debug(txt)
         obj = Event()
         obj.rawstr = rawstr
@@ -380,14 +377,16 @@
         if not obj.txt:
             obj.txt = rawstr.split(':', 2)[-1]
         if not obj.txt and len(arguments) == 1:
             obj.txt = arguments[1]
         spl = obj.txt.split()
         if len(spl) > 1:
             obj.args = spl[1:]
+        if obj.args:
+            obj.rest = " ".join(obj.args)
         obj.orig = repr(self)
         obj.txt = obj.txt.strip()
         obj.type = obj.command
         return obj
 
     def poll(self):
         self.events.connected.wait()
@@ -486,14 +485,80 @@
     def stop(self):
         Broker.remove(self)
         Reactor.stop(self)
         Output.stop(self)
         self.disconnect()
 
 
+class User(Object):
+
+    def __init__(self, val=None):
+        Object.__init__(self)
+        self.user = ''
+        self.perms = []
+        if val:
+            update(self, val)
+
+    def isok(self):
+        return True
+
+    def isthere(self):
+        return True
+
+
+class Users(Object):
+
+    @staticmethod
+    def allowed(origin, perm):
+        perm = perm.upper()
+        user = Users.get_user(origin)
+        val = False
+        if user and perm in user.perms:
+            val = True
+        return val
+
+    @staticmethod
+    def delete(origin, perm):
+        res = False
+        for user in Users.get_users(origin):
+            try:
+                user.perms.remove(perm)
+                write(user)
+                res = True
+            except ValueError:
+                pass
+        return res
+
+    @staticmethod
+    def get_users(origin=''):
+        selector = {'user': origin}
+        return find('user', selector)
+
+    @staticmethod
+    def get_user(origin):
+        users = list(Users.get_users(origin))
+        res = None
+        if len(users) > 0:
+            res = users[-1]
+        return res
+
+    @staticmethod
+    def perm(origin, permission):
+        user = Users.get_user(origin)
+        if not user:
+            raise NoUser(origin)
+        if permission.upper() not in user.perms:
+            user.perms.append(permission.upper())
+            write(user)
+        return user
+
+
+# CALLBACKS
+
+
 def cb_auth(evt):
     bot = evt.bot()
     assert evt
     assert bot.cfg.password
     bot.direct(f'AUTHENTICATE {bot.cfg.password}')
 
 
@@ -555,86 +620,25 @@
         elif evt.txt.startswith(f'{bot.cfg.nick}:'):
             evt.txt = evt.txt[len(bot.cfg.nick)+1:]
         else:
             return
         if bot.cfg.users and not Users.allowed(evt.origin, 'USER'):
             return
         Logging.debug(f"command from {evt.origin}: {evt.txt}")
-        parse(evt, evt.txt)
         Command.handle(evt)
 
 
 def cb_quit(evt):
     bot = evt.bot()
     Logging.debug(f"quit from {bot.cfg.server}")
     if evt.orig and evt.orig in bot.zelf:
         bot.stop()
 
 
-class User(Object):
-
-    def __init__(self, val=None):
-        Object.__init__(self)
-        self.user = ''
-        self.perms = []
-        if val:
-            update(self, val)
-
-    def isok(self):
-        return True
-
-    def isthere(self):
-        return True
-
-
-class Users(Object):
-
-    @staticmethod
-    def allowed(origin, perm):
-        perm = perm.upper()
-        user = Users.get_user(origin)
-        val = False
-        if user and perm in user.perms:
-            val = True
-        return val
-
-    @staticmethod
-    def delete(origin, perm):
-        res = False
-        for user in Users.get_users(origin):
-            try:
-                user.perms.remove(perm)
-                write(user)
-                res = True
-            except ValueError:
-                pass
-        return res
-
-    @staticmethod
-    def get_users(origin=''):
-        selector = {'user': origin}
-        return find('user', selector)
-
-    @staticmethod
-    def get_user(origin):
-        users = list(Users.get_users(origin))
-        res = None
-        if len(users) > 0:
-            res = users[-1]
-        return res
-
-    @staticmethod
-    def perm(origin, permission):
-        user = Users.get_user(origin)
-        if not user:
-            raise NoUser(origin)
-        if permission.upper() not in user.perms:
-            user.perms.append(permission.upper())
-            write(user)
-        return user
+# COMMANDS
 
 
 def cfg(event):
     config = Config()
     last(config)
     if not event.sets:
         event.reply(
```

### Comparing `opr-240/opr/modules/log.py` & `opr-241/opr/modules/log.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 #
 # pylint: disable=C,I,R
 
 
 "log text"
 
 
-__author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 import time
 
 
 from .. import Object
 from .. import find, fntime, laps, write
```

### Comparing `opr-240/opr/modules/rss.py` & `opr-241/opr/modules/rss.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 #
 # pylint: disable=C,I,R,W0401
 
 
 "rich site syndicte"
 
 
-__author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 import html.parser
 import re
 import threading
 import time
 import urllib
 import _thread
 
@@ -24,15 +21,15 @@
 
 from .. import Broker, Cfg, Object, Repeater
 from .. import find, fntime, laps, prt, update, write
 from .. import launch, last, spl
 
 
 def start():
-    time.sleep(15.0)
+    time.sleep(30.0)
     fetcher = Fetcher()
     fetcher.start()
     return fetcher
 
 
 fetchlock = _thread.allocate_lock()
 
@@ -174,14 +171,17 @@
             obj = Object()
             for itm in spl(item):
                 setattr(obj, itm, Parser.getitem(line, itm))
             res.append(obj)
         return res
 
 
+# UTILITY
+
+
 def getfeed(url, item):
     if Cfg.debug:
         return [Object(), Object()]
     try:
         result = geturl(url)
     except (ValueError, HTTPError, URLError):
         return [Object(), Object()]
@@ -227,14 +227,17 @@
     return html.unescape(txt)
 
 
 def useragent(txt):
     return 'Mozilla/5.0 (X11; Linux x86_64) ' + txt
 
 
+# COMMANDS
+
+
 def dpl(event):
     if len(event.args) < 2:
         event.reply('dpl <stringinurl> <item1,item2>')
         return
     setter = {'display_list': event.args[1]}
     for feed in find('rss', {'rss': event.args[0]}):
         if feed:
```

### Comparing `opr-240/opr/modules/shp.py` & `opr-241/opr/modules/tdo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,53 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C,I,R
 
 
-"shopping list"
-
-
-__author__ = "Bart Thate <programmingobject@gmail.com>"
+"todo list"
 
 
 import time
 
 
-from .. import Cfg, Object 
-from .. import find, fntime, laps, write
+from .. import Object
+from .. import laps, find, fntime, write
 
 
-class Shop(Object):
+class Todo(Object):
 
     def __init__(self):
         super().__init__()
         self.txt = ''
 
-    def size(self):
-        return len(self.__dict__)
+    def len(self):
+        return 0
 
-    def length(self):
+    def size(self):
         return len(self.__dict__)
 
 
-def got(event):
+def dne(event):
     if not event.args:
         return
     selector = {'txt': event.args[0]}
-    for obj in find('shop', selector):
+    for obj in find('todo', selector):
         obj.__deleted__ = True
         write(obj)
-        event.reply('ok') # okdan
+        event.reply('ok')
+        break
 
 
-def shp(event):
+def tdo(event):
     if not event.rest:
         nmr = 0
-        for obj in find(Cfg.workdir, 'shop'):
+        for obj in find('todo'):
             lap = laps(time.time()-fntime(obj.__oid__))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
-            event.reply("no shops")
+            event.reply("no todo")
         return
-    obj = Shop()
+    obj = Todo()
     obj.txt = event.rest
     write(obj)
     event.reply('ok')
```

### Comparing `opr-240/opr/modules/tdo.py` & `opr-241/opr/modules/wsh.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,52 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,I,R
+# pylint: disable=C,I,R,W0401,W0614
 
 
-"todo list"
-
-
-__author__ = "Bart Thate <programmingobject@gmail.com>"
+"wish list"
 
 
 import time
 
 
 from .. import Object
-from .. import laps, find, fntime, write
+from .. import find, fntime, laps, write
 
 
-class Todo(Object):
+class Wish(Object):
 
     def __init__(self):
-        super().__init__()
+        Object.__init__(self)
         self.txt = ''
 
-    def len(self):
-        return 0
+    def gettxt(self):
+        return self.txt
 
-    def size(self):
-        return len(self.__dict__)
+    def settxt(self, txt):
+        self.txt = txt
 
 
-def dne(event):
+def ful(event):
     if not event.args:
         return
     selector = {'txt': event.args[0]}
-    for obj in find('todo', selector):
+    for obj in find('wish', selector):
         obj.__deleted__ = True
         write(obj)
-        event.reply('ok')
-        break
+        event.reply('done')
 
 
-def tdo(event):
+def wsh(event):
     if not event.rest:
         nmr = 0
-        for obj in find('todo'):
+        for obj in find('wish'):
             lap = laps(time.time()-fntime(obj.__oid__))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
-            event.reply("no todo")
+            event.reply("no wishes")
         return
-    obj = Todo()
+    obj = Wish()
     obj.txt = event.rest
     write(obj)
     event.reply('ok')
```

### Comparing `opr-240/opr/modules/udp.py` & `opr-241/opr/modules/udp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C,I,R
+# flake8: noqa=E501
 
 
 "udp to irc relay"
 
 
-__author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 import select
 import socket
 import sys
 import time
 
 
 from .. import Broker, Object
@@ -89,20 +87,29 @@
 def udp(event):
     cfg = Cfg()
     last(cfg)
     if len(sys.argv) > 2:
         txt = " ".join(sys.argv[2:])
         toudp(cfg.host, cfg.port, txt)
         return
-    if not select.select([sys.stdin, ], [], [], 0.0)[0]:
+    if not select.select(
+                         [sys.stdin, ],
+                         [],
+                         [],
+                         0.0
+                        )[0]:
         return
     size = 0
     while 1:
         try:
-            (inp, _out, err) = select.select([sys.stdin,], [], [sys.stderr,])
+            (inp, _out, err) = select.select(
+                                             [sys.stdin,],
+                                             [],
+                                             [sys.stderr,]
+                                            )
         except KeyboardInterrupt:
             return
         if err:
             break
         stop = False
         for sock in inp:
             txt = sock.readline()
```

### Comparing `opr-240/opr/modules/wsh.py` & `opr-241/opr/modules/shp.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,I,R,W0401,W0614
+# pylint: disable=C,I,R
 
 
-"wish list"
-
-
-__author__ = "Bart Thate <programmingobject@gmail.com>"
+"shopping list"
 
 
 import time
 
 
 from .. import Object
 from .. import find, fntime, laps, write
 
 
-class Wish(Object):
+class Shop(Object):
 
     def __init__(self):
-        Object.__init__(self)
+        super().__init__()
         self.txt = ''
 
-    def gettxt(self):
-        return self.txt
+    def size(self):
+        return len(self.__dict__)
 
-    def settxt(self, txt):
-        self.txt = txt
+    def length(self):
+        return len(self.__dict__)
 
 
-def ful(event):
+def got(event):
     if not event.args:
         return
     selector = {'txt': event.args[0]}
-    for obj in find('wish', selector):
+    for obj in find('shop', selector):
         obj.__deleted__ = True
         write(obj)
-        event.reply('done')
+        event.reply('ok')
 
 
-def wsh(event):
+def shp(event):
     if not event.rest:
         nmr = 0
-        for obj in find('wish'):
+        for obj in find('shop'):
             lap = laps(time.time()-fntime(obj.__oid__))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
-            event.reply("no wishes")
+            event.reply("no shops")
         return
-    obj = Wish()
+    obj = Shop()
     obj.txt = event.rest
     write(obj)
     event.reply('ok')
```

### Comparing `opr-240/opr/objects.py` & `opr-241/opr/objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C,I,R
+# flake8: noqa=C901
 
 
 "clean namespace"
 
 
-__author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 import datetime
 import os
 import uuid
 
 
 def __dir__():
     return (
@@ -36,19 +34,18 @@
 
 
 __all__ = __dir__()
 
 
 class Object:
 
-    __slots__ = ("__dict__", "__oid__")
-
-    default = ""
+    __slots__ = ("__dict__", "__default__", "__oid__")
 
     def __init__(self, *args, **kwargs):
+        self.__default__ = ""
         self.__oid__ = ident(self)
         if args:
             val = args[0]
             if isinstance(val, list):
                 update(self, dict(val))
             elif isinstance(val, zip):
                 update(self, dict(val))
@@ -62,15 +59,15 @@
     def __contains__(self, key):
         return key in self.__dict__
 
     def __delitem__(self, key):
         return self.__dict__.__delitem__(key)
 
     def __getattr__(self, key):
-        return self.__dict__.get(key, Object.default)
+        return self.__dict__.get(key, self.__default__)
 
     def __getitem__(self, key):
         return self.__dict__.__getitem__(key)
 
     def __iter__(self):
         return iter(self.__dict__)
```

### Comparing `opr-240/opr/parsers.py` & `opr-241/opr/parsers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C,I,R
+# flake8: noqa=C901
 
 
 "parse events"
 
 
-__author__ = "Bart Thate <programmingobject@gmail.com>"
+from .objects import Object
 
 
 def __dir__():
     return (
             "parse",
            )
 
 
 __all__ = __dir__()
 
 
 def parse(obj, txt):
     obj.cmd = obj.cmd or ""
-    obj.args = obj.args or []
-    obj.gets = obj.gets or {}
+    obj.args = []
+    obj.gets = obj.gets or Object()
     obj.mod = obj.mod or ""
     obj.opts = obj.opts or ""
     obj.otxt = txt or ""
-    obj.rest = obj.rest or ""
-    obj.sets = obj.sets or {}
+    obj.rest = ""
+    obj.sets = obj.sets or Object()
     for spli in txt.split():
         if spli.startswith("-"):
             try:
                 obj.index = int(spli[1:])
             except ValueError:
                 obj.opts += spli[1:]
             continue
```

### Comparing `opr-240/opr/persist.py` & `opr-241/opr/persist.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 #
 # pylint: disable=C,I,R
 
 
 "persistence"
 
 
-__author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 import os
 import sys
 import time
 
+
 from .objects import kind
 from .decoder import load
 from .encoder import dump
 from .locking import disklock
 from .objects import Object, ident, items, update
 from .utility import cdir, strip
 
@@ -31,67 +29,58 @@
             'write'
            )
 
 
 __all__ = __dir__()
 
 
-
 class Persist:
 
-    """directory to persist to"""
-
     workdir = ""
 
     @staticmethod
     def path(pth) -> str:
-        """return store path"""
         return os.path.join(Persist.workdir, 'store', pth)
 
     @staticmethod
     def storedir() -> str:
-        """return storage directory"""
         return os.path.join(Persist.workdir, "store", "")
 
 
 def files() -> []:
-    """show all files in store"""
     res = []
     path = Persist.storedir()
     if os.path.exists(path):
         res = os.listdir(path)
     return res
 
 
 def find(mtc, selector=None) -> []:
-    """locate specific objects"""
     if selector is None:
         selector = {}
     for fnm in fns(mtc):
         obj = hook(fnm)
         if '__deleted__' in obj:
             continue
         if selector and not search(obj, selector):
             continue
         yield obj
 
 
 def fnclass(pth) -> str:
-    """return class from filename"""
     try:
         *_rest, mpth = pth.split("store")
         splitted = mpth.split(os.sep)
         return splitted[0]
     except ValueError:
         pass
     return None
 
 
 def fns(mtc) -> []:
-    """return matching filenames"""
     dname = ''
     lst = mtc.lower().split(".")[-1]
     for rootdir, dirs, _files in os.walk(Persist.storedir(), topdown=False):
         if dirs:
             dname = sorted(dirs)[-1]
             if dname.count('-') == 2:
                 ddd = os.path.join(rootdir, dname)
@@ -100,15 +89,14 @@
                     path2 = os.path.join(ddd, fls[-1])
                     splitted = strip(path2).split(os.sep, maxsplit=1)[0]
                     if lst in splitted.lower().split(".")[-1]:
                         yield strip(path2)
 
 
 def fntime(daystr) -> float:
-    """return time from filename"""
     daystr = daystr.replace('_', ':')
     datestr = ' '.join(daystr.split(os.sep)[-2:])
     if '.' in datestr:
         datestr, rest = datestr.rsplit('.', 1)
     else:
         rest = ''
     tme = time.mktime(time.strptime(datestr, '%Y-%m-%d %H:%M:%S'))
@@ -116,15 +104,14 @@
         tme += float('.' + rest)
     else:
         tme = 0
     return tme
 
 
 def hook(otp) -> type:
-    """return object from filename"""
     clz = fnclass(otp)
     splitted = clz.split(".")
     modname = ".".join(splitted[:1])
     clz = splitted[-1]
     mod = sys.modules.get(modname, None)
     if mod:
         cls = getattr(mod, clz, None)
@@ -137,30 +124,28 @@
     return obj
 
 
 # METHODS
 
 
 def last(obj, selector=None) -> None:
-    """update with last saved version"""
     if selector is None:
         selector = {}
     result = sorted(
                     find(kind(obj), selector),
                     key=lambda x: fntime(x.__oid__)
                    )
     if result:
         inp = result[-1]
         update(obj, inp)
         obj.__oid__ = inp.__oid__
     return obj.__oid__
 
 
 def read(obj, pth) -> str:
-    """read object from path"""
     pth = Persist.path(pth)
     with disklock:
         with open(pth, 'r', encoding='utf-8') as ofile:
             data = load(ofile)
             update(obj, data)
     obj.__oid__ = strip(pth)
     return obj.__oid__
@@ -176,15 +161,14 @@
                 break
         except KeyError:
             continue
     return res
 
 
 def write(obj) -> str:
-    """write object to disk"""
     try:
         pth = obj.__oid__
     except TypeError:
         pth = ident(obj)
     pth = Persist.path(pth)
     cdir(pth)
     with disklock:
```

### Comparing `opr-240/opr/reactor.py` & `opr-241/opr/reactor.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,32 +2,28 @@
 #
 # pylint: disable=C,I,R,W0212,W0718
 
 
 "reacting"
 
 
-__author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 import queue
 import ssl
 import threading
 
 
 from .errored import Errors
 from .evented import Event
 from .objects import Object
 from .threads import launch
 
 
 def __dir__():
     return (
             'Reactor',
-            "dispatch"
            )
 
 
 __all__ = __dir__()
 
 
 class Reactor(Object):
@@ -37,25 +33,37 @@
         self.cbs = Object()
         self.queue = queue.Queue()
         self.stopped = threading.Event()
 
     def announce(self, txt) -> None:
         self.raw(txt)
 
+    @staticmethod
+    def dispatch(func, evt) -> None:
+        try:
+            func(evt)
+        except Exception as ex:
+            exc = ex.with_traceback(ex.__traceback__)
+            Errors.errors.append(exc)
+            try:
+                evt.ready()
+            except AttributeError:
+                pass
+
     def event(self, txt) -> Event:
         msg = Event()
         msg.type = 'event'
         msg.orig = repr(self)
         msg.txt = txt
         return msg
 
     def handle(self, evt) -> Event:
         func = getattr(self.cbs, evt.type, None)
         if func:
-            evt._thr = launch(dispatch, func, evt, name=evt.cmd)
+            evt._thr = launch(Reactor.dispatch, func, evt, name=evt.cmd)
             evt._thr.join()
         return evt
 
     def loop(self) -> None:
         while not self.stopped.is_set():
             try:
                 self.handle(self.poll())
@@ -88,19 +96,7 @@
 
     def start(self) -> None:
         launch(self.loop)
 
     def stop(self) -> None:
         self.stopped.set()
         self.queue.put_nowait(None)
-
-
-def dispatch(func, evt) -> None:
-    try:
-        func(evt)
-    except Exception as ex:
-        exc = ex.with_traceback(ex.__traceback__)
-        Errors.errors.append(exc)
-        try:
-            evt.ready()
-        except AttributeError:
-            pass
```

### Comparing `opr-240/opr/recurse.py` & `opr-241/opr/recurse.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 #
 # pylint: disable=C,I,R,E0402
 
 
 "recursive functions"
 
 
-__author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
-from .objects  import Object, items, update
+from .objects import Object, items, update
 from .persist import read, write
 
 
 def __dir__():
     return (
             'readrec',
             'writerec'
```

### Comparing `opr-240/opr/repeats.py` & `opr-241/opr/repeats.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C,I,R,E0402
 
 
+"repeaters"
+
+
 import threading
 import time
 
 
 from .objects import Object
 from .threads import launch
```

### Comparing `opr-240/opr/threads.py` & `opr-241/opr/threads.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 #
 # pylint: disable=C,I,R,W0718
 
 
 "running threads"
 
 
-__author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 import functools
 import queue
 import threading
 import time
 
 
 from .errored import Errors
```

### Comparing `opr-240/opr/utility.py` & `opr-241/opr/utility.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,36 @@
 #
 # pylint: disable=C,I,R
 
 
 "utilities"
 
 
-__author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 import os
 import pathlib
 import time
 import types
 
 
+def __dir__():
+    return (
+            "banner",
+            "cdir",
+            "laps",
+            "name",
+            "skip",
+            "spl",
+            "strip",
+            "wait"
+           )
+
+
+__all__ = __dir__()
+
+
 def banner(names, version):
     times = time.ctime(time.time())
     return f"{names.upper()} {version} {times}"
 
 
 def cdir(pth) -> None:
     if not pth.endswith(os.sep):
@@ -83,17 +96,29 @@
     if '__name__' in dir(obj):
         clz = obj.__class__.__name__
         nme = obj.__name__
         return f'{clz}.{nme}'
     return None
 
 
+def skip(txt, skipping) -> bool:
+    for skp in spl(skipping):
+        if skp in txt:
+            return True
+    return False
+
+
 def spl(txt) -> []:
     try:
         res = txt.split(',')
     except (TypeError, ValueError):
         res = txt
     return [x for x in res if x]
 
 
 def strip(path) -> str:
     return os.sep.join(path.split(os.sep)[-4:])
+
+
+def wait():
+    while 1:
+        time.sleep(1.0)
```

### Comparing `opr-240/opr.egg-info/PKG-INFO` & `opr-241/opr.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 Metadata-Version: 2.1
 Name: opr
-Version: 240
+Version: 241
 Summary: Object Programming Runtime
 Author-email: Bart Thate <programmingobject@gmail.com>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/opr
 Project-URL: bugs, https://github.com/bthate/opr/issues
 Project-URL: source, https://github.com/bthate/opr
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Topic :: Utilities
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 
-# This file is placed in the Public Domain.
-#
-# __author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 NAME
 
 ::
 
    OPR - Object Programming Runtime
 
 
@@ -62,47 +57,47 @@
 USAGE
 
 
 ::
 
     list of commands
 
-    $ opr cmd
-    cmd,err,flt,sts,thr,upt
+        $ opr cmd
+        cmd,err,flt,sts,thr,upt
 
     start a console
 
-    $ opr -c
-    >
+        $ opr -c
+        >
 
     start additional modules
 
-    $ opr mod=<mod1,mod2> -c
-    >
+        $ opr mod=<mod1,mod2> -c
+        >
 
     list of modules
 
-    $ opr mod
-    cmd,err,flt,fnd,irc,log,mdl,mod,
-    req, rss,slg,sts,tdo,thr,upt,ver
+        $ opr mod
+        cmd,err,flt,fnd,irc,log,mdl,mod,
+        req, rss,slg,sts,tdo,thr,upt,ver
 
     to start irc, add mod=irc when
     starting
 
-    $ opr mod=irc -c
+        $ opr mod=irc -c
 
     to start rss, also add mod=rss
     when starting
 
-    $ opr mod=irc,rss -c
+        $ opr mod=irc,rss -c
 
     start as daemon
 
-    $ opr  mod=irc,rss -d
-    $ 
+        $ opr  mod=irc,rss -d
+        $ 
 
 
 CONFIGURATION
 
 
 ::
 
@@ -144,14 +139,37 @@
     pwd - sasl nickserv name/pass
     rem - removes a rss feed
     rss - add a feed
     slg - slogan
     thr - show the running threads
 
 
+SYSTEMD
+
+::
+
+ [Unit]
+ Description=Object Programming Runtime
+ Requires=network.target
+ After=network.target
+
+ [Service]
+ DynamicUser=True
+ Type=fork
+ User=bart
+ Group=bart
+ PIDFile=opr.pid
+ WorkingDirectory=/home/bart/.opr
+ ExecStart=/home/bart/.local/pipx/venvs/opr/bin/opr mod=irc,rss,mdl -d
+ RemainAfterExit=yes
+
+ [Install]
+ WantedBy=multi-user.target
+
+
 FILES
 
 ::
 
     ~/.local/bin/opr
     ~/.local/pipx/venvs/opr/
```

### Comparing `opr-240/pyproject.toml` & `opr-241/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,21 @@
-# This file is placed in the Public Domain.
-#
-# __author__ = "Bart Thate <programmingobject@gmail.com>"
-
-
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [options]
 zip_safe = true
 include_package_data = true
 
 
 [project]
 name = "opr"
 description = "Object Programming Runtime"
-version = "240"
+version = "241"
 authors = [
     {name = "Bart Thate", email = "programmingobject@gmail.com" },
 ]
 readme = "README.rst"
 license = { text="Public Domain"}
 classifiers = [ 
                'Development Status :: 3 - Alpha',
@@ -32,23 +27,25 @@
 
 
 [project.urls]
 "home" = "https://pypi.org/project/opr"
 "bugs" = "https://github.com/bthate/opr/issues"
 "source" = "https://github.com/bthate/opr"
 
+[project.scripts]
+opr = "opr.__main__:wrapped"
+
 
 [project.optional-dependencies]
 dev = []
 
-[tool.setuptools]
-script-files = ["bin/opr"]
-
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["opr*"]
-exclude = ["tests*",]
+exclude = ["test*",]
 namespaces = false
 
 
-[tool.setuptools.package-data]
-"*" = ["bin/opr*"]
+[tool.pytest.ini_options]
+minversion = "6.0"
+addopts = ""
+testpaths = ["bin"]
```

