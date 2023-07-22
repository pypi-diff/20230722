# Comparing `tmp/rfswarm-agent-1.1.3.tar.gz` & `tmp/rfswarm-agent-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfswarm-agent-1.1.3.tar", last modified: Sun Jun  4 05:25:59 2023, max compression
+gzip compressed data, was "rfswarm-agent-1.1.4.tar", last modified: Sat Jul 22 13:01:07 2023, max compression
```

## Comparing `rfswarm-agent-1.1.3.tar` & `rfswarm-agent-1.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-04 05:25:59.301699 rfswarm-agent-1.1.3/
--rw-r--r--   0 dave      (1000) dave      (1000)    35149 2023-02-10 08:46:44.000000 rfswarm-agent-1.1.3/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)     3152 2023-06-04 05:25:59.301699 rfswarm-agent-1.1.3/PKG-INFO
--rw-r--r--   0 dave      (1000) dave      (1000)     5809 2023-06-04 04:58:34.000000 rfswarm-agent-1.1.3/README.md
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-04 05:25:59.301699 rfswarm-agent-1.1.3/rfswarm_agent/
--rw-r--r--   0 dave      (1000) dave      (1000)       53 2023-06-04 05:25:57.000000 rfswarm-agent-1.1.3/rfswarm_agent/__init__.py
--rw-r--r--   0 dave      (1000) dave      (1000)    49769 2023-06-04 05:25:57.000000 rfswarm-agent-1.1.3/rfswarm_agent/rfswarm_agent.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-04 05:25:59.301699 rfswarm-agent-1.1.3/rfswarm_agent.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     3152 2023-06-04 05:25:59.000000 rfswarm-agent-1.1.3/rfswarm_agent.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      313 2023-06-04 05:25:59.000000 rfswarm-agent-1.1.3/rfswarm_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-04 05:25:59.000000 rfswarm-agent-1.1.3/rfswarm_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       71 2023-06-04 05:25:59.000000 rfswarm-agent-1.1.3/rfswarm_agent.egg-info/entry_points.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       44 2023-06-04 05:25:59.000000 rfswarm-agent-1.1.3/rfswarm_agent.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       14 2023-06-04 05:25:59.000000 rfswarm-agent-1.1.3/rfswarm_agent.egg-info/top_level.txt
--rw-r--r--   0 dave      (1000) dave      (1000)     1138 2023-06-04 05:25:57.000000 rfswarm-agent-1.1.3/setup-agent.py
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-06-04 05:25:59.301699 rfswarm-agent-1.1.3/setup.cfg
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-22 13:01:07.650849 rfswarm-agent-1.1.4/
+-rw-r--r--   0 dave      (1000) dave      (1000)    35149 2023-02-10 08:46:44.000000 rfswarm-agent-1.1.4/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3152 2023-07-22 13:01:07.650849 rfswarm-agent-1.1.4/PKG-INFO
+-rw-r--r--   0 dave      (1000) dave      (1000)     6597 2023-07-22 12:53:23.000000 rfswarm-agent-1.1.4/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-22 13:01:07.646849 rfswarm-agent-1.1.4/rfswarm_agent/
+-rw-r--r--   0 dave      (1000) dave      (1000)       53 2023-07-22 13:01:06.000000 rfswarm-agent-1.1.4/rfswarm_agent/__init__.py
+-rw-r--r--   0 dave      (1000) dave      (1000)    49964 2023-07-22 13:01:06.000000 rfswarm-agent-1.1.4/rfswarm_agent/rfswarm_agent.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-22 13:01:07.650849 rfswarm-agent-1.1.4/rfswarm_agent.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3152 2023-07-22 13:01:07.000000 rfswarm-agent-1.1.4/rfswarm_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      313 2023-07-22 13:01:07.000000 rfswarm-agent-1.1.4/rfswarm_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-22 13:01:07.000000 rfswarm-agent-1.1.4/rfswarm_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       71 2023-07-22 13:01:07.000000 rfswarm-agent-1.1.4/rfswarm_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       44 2023-07-22 13:01:07.000000 rfswarm-agent-1.1.4/rfswarm_agent.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       14 2023-07-22 13:01:07.000000 rfswarm-agent-1.1.4/rfswarm_agent.egg-info/top_level.txt
+-rw-r--r--   0 dave      (1000) dave      (1000)     1138 2023-07-22 13:01:06.000000 rfswarm-agent-1.1.4/setup-agent.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-07-22 13:01:07.650849 rfswarm-agent-1.1.4/setup.cfg
```

### Comparing `rfswarm-agent-1.1.3/LICENSE` & `rfswarm-agent-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rfswarm-agent-1.1.3/PKG-INFO` & `rfswarm-agent-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfswarm-agent
-Version: 1.1.3
+Version: 1.1.4
 Summary: rfswarm Agent
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
 License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
```

### Comparing `rfswarm-agent-1.1.3/README.md` & `rfswarm-agent-1.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 
 |Version|Manager|Agent|Reporter|
 |---|---|---|---|
 |[![Latest PyPI version](https://img.shields.io/pypi/v/rfswarm-manager.svg)](https://pypi.python.org/pypi/rfswarm-manager/) | [![Number of Manager PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-manager.svg)](https://pypi.python.org/pypi/rfswarm-manager/) | [![Number of Agent PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-agent.svg)](https://pypi.python.org/pypi/rfswarm-agent/) | [![Number of Reporter PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-reporter.svg)](https://pypi.python.org/pypi/rfswarm-reporter/) |
 
 | Master | Branch |
 | -- | -- |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=v1.1.3&label=Linter) |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=v1.1.3&label=Regression%20Tests) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=v1.1.4&label=Linter) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=v1.1.4&label=Regression%20Tests) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=v1.1.4&label=Linter) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=v1.1.4&label=Regression%20Tests) |
 
 <img align="right" src="Doc/Images/Icon_Information.png">
 
 ## About
 rfswarm is a testing tool that allows you use [Robot Framework](https://robotframework.org/) test cases for performance or load testing.
 
 > _Swarm being the collective noun for Robots, just as Flock is for Birds and Herd for Sheep, so it made sense to use swarm for a performance testing tool using Robot Framework, hence rfswarm_
@@ -65,8 +67,8 @@
 
 ## Donations
 
 If you would like to thank me for this project please consider using one of the sponsorship methods:
 - [GitHub](https://github.com/sponsors/damies13?frequency=one-time&sponsor=damies13)
 - [PayPal.me](https://paypal.me/damies13/5) (the $5 is a suggestion, feel free to change to any amount you would like)
 
-[See our sponsors](Doc/Sponsors.md)
+[See our sponsors](Doc/Sponsors.md)
```

### Comparing `rfswarm-agent-1.1.3/rfswarm_agent/rfswarm_agent.py` & `rfswarm-agent-1.1.4/rfswarm_agent/rfswarm_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 #
 # 	Robot Framework Swarm
 #
-#    Version 1.1.3
+#    Version 1.1.4
 #
 
 
 # https://stackoverflow.com/questions/48090535/csv-file-reading-and-find-the-value-from-nth-column-using-robot-framework
 
 import argparse
 import base64
@@ -31,15 +31,15 @@
 import pkg_resources
 import psutil
 import requests
 
 
 class RFSwarmAgent():
 
-	version = "1.1.3"
+	version = "1.1.4"
 	config = None
 	isconnected = False
 	isrunning = False
 	isstopping = False
 	runagent = True
 	run_name = None
 	swarmmanager = None
@@ -163,15 +163,15 @@
 		t = threading.Thread(target=self.tick_counter)
 		t.start()
 
 		t = threading.Thread(target=self.findlibraries)
 		t.start()
 
 		self.agentproperties["OS: Platform"] = platform.platform()  # 'Linux-3.3.0-8.fc16.x86_64-x86_64-with-fedora-16-Verne'
-		self.agentproperties["OS: System"] = platform.system()  # 'Windows'
+		self.agentproperties["OS: System"] = platform.system()  # 'Windows'		Returns the system/OS name, such as 'Linux', 'Darwin', 'Java', 'Windows'
 		self.agentproperties["OS: Release"] = platform.release()  # 'XP'
 		self.agentproperties["OS: Version"] = platform.version()  # '5.1.2600'
 
 		if platform.system() == 'Windows':
 			vararr = platform.version().split(".")
 		else:
 			vararr = platform.release().split(".")
@@ -777,14 +777,17 @@
 
 		self.jobs[jobid]["Iteration"] += 1
 
 		hash = self.jobs[jobid]['ScriptHash']
 		self.debugmsg(6, "runthread: hash:", hash)
 		test = self.jobs[jobid]['Test']
 		self.debugmsg(6, "runthread: test:", test)
+		if platform.system() != 'Windows':
+			test = test.replace(r'${', r'\${')
+			self.debugmsg(6, "runthread: test:", test)
 
 		if 'localfile' not in self.scriptlist[hash]:
 			if self.corethreads["getscripts"].is_alive():
 				self.corethreads["getscripts"].join()
 			else:
 				self.corethreads["getscripts"] = threading.Thread(target=self.getscripts)
 				self.corethreads["getscripts"].start()
```

### Comparing `rfswarm-agent-1.1.3/rfswarm_agent.egg-info/PKG-INFO` & `rfswarm-agent-1.1.4/rfswarm_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfswarm-agent
-Version: 1.1.3
+Version: 1.1.4
 Summary: rfswarm Agent
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
 License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
```

### Comparing `rfswarm-agent-1.1.3/setup-agent.py` & `rfswarm-agent-1.1.4/setup-agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README_PyPi.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="rfswarm-agent",
-	version="1.1.3",
+	version="1.1.4",
 	author="damies13",
 	author_email="damies13+rfswarm@gmail.com",
 	description="rfswarm Agent",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/damies13/rfswarm",
 	packages=setuptools.find_packages(exclude=["*fswarm_report*", "*rfswarm_manager*", "build/*"]),
```

