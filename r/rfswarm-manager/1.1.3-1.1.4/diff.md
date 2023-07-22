# Comparing `tmp/rfswarm-manager-1.1.3.tar.gz` & `tmp/rfswarm-manager-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfswarm-manager-1.1.3.tar", last modified: Sun Jun  4 05:25:58 2023, max compression
+gzip compressed data, was "rfswarm-manager-1.1.4.tar", last modified: Sat Jul 22 13:01:07 2023, max compression
```

## Comparing `rfswarm-manager-1.1.3.tar` & `rfswarm-manager-1.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-04 05:25:58.609713 rfswarm-manager-1.1.3/
--rw-r--r--   0 dave      (1000) dave      (1000)    35149 2023-02-10 08:46:44.000000 rfswarm-manager-1.1.3/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)     3156 2023-06-04 05:25:58.609713 rfswarm-manager-1.1.3/PKG-INFO
--rw-r--r--   0 dave      (1000) dave      (1000)     5809 2023-06-04 04:58:34.000000 rfswarm-manager-1.1.3/README.md
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-04 05:25:58.605713 rfswarm-manager-1.1.3/rfswarm_manager/
--rw-r--r--   0 dave      (1000) dave      (1000)       53 2023-06-04 05:25:57.000000 rfswarm-manager-1.1.3/rfswarm_manager/__init__.py
--rw-r--r--   0 dave      (1000) dave      (1000)   314437 2023-06-04 05:25:57.000000 rfswarm-manager-1.1.3/rfswarm_manager/rfswarm.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-04 05:25:58.609713 rfswarm-manager-1.1.3/rfswarm_manager.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     3156 2023-06-04 05:25:58.000000 rfswarm-manager-1.1.3/rfswarm_manager.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      325 2023-06-04 05:25:58.000000 rfswarm-manager-1.1.3/rfswarm_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-04 05:25:58.000000 rfswarm-manager-1.1.3/rfswarm_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      111 2023-06-04 05:25:58.000000 rfswarm-manager-1.1.3/rfswarm_manager.egg-info/entry_points.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       78 2023-06-04 05:25:58.000000 rfswarm-manager-1.1.3/rfswarm_manager.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       16 2023-06-04 05:25:58.000000 rfswarm-manager-1.1.3/rfswarm_manager.egg-info/top_level.txt
--rw-r--r--   0 dave      (1000) dave      (1000)     1419 2023-06-04 05:25:57.000000 rfswarm-manager-1.1.3/setup-manager.py
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-06-04 05:25:58.609713 rfswarm-manager-1.1.3/setup.cfg
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-22 13:01:07.218849 rfswarm-manager-1.1.4/
+-rw-r--r--   0 dave      (1000) dave      (1000)    35149 2023-02-10 08:46:44.000000 rfswarm-manager-1.1.4/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3156 2023-07-22 13:01:07.218849 rfswarm-manager-1.1.4/PKG-INFO
+-rw-r--r--   0 dave      (1000) dave      (1000)     6597 2023-07-22 12:53:23.000000 rfswarm-manager-1.1.4/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-22 13:01:07.214849 rfswarm-manager-1.1.4/rfswarm_manager/
+-rw-r--r--   0 dave      (1000) dave      (1000)       53 2023-07-22 13:01:06.000000 rfswarm-manager-1.1.4/rfswarm_manager/__init__.py
+-rw-r--r--   0 dave      (1000) dave      (1000)   315294 2023-07-22 13:01:06.000000 rfswarm-manager-1.1.4/rfswarm_manager/rfswarm.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-22 13:01:07.218849 rfswarm-manager-1.1.4/rfswarm_manager.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3156 2023-07-22 13:01:07.000000 rfswarm-manager-1.1.4/rfswarm_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      325 2023-07-22 13:01:07.000000 rfswarm-manager-1.1.4/rfswarm_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-22 13:01:07.000000 rfswarm-manager-1.1.4/rfswarm_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      111 2023-07-22 13:01:07.000000 rfswarm-manager-1.1.4/rfswarm_manager.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       78 2023-07-22 13:01:07.000000 rfswarm-manager-1.1.4/rfswarm_manager.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       16 2023-07-22 13:01:07.000000 rfswarm-manager-1.1.4/rfswarm_manager.egg-info/top_level.txt
+-rw-r--r--   0 dave      (1000) dave      (1000)     1419 2023-07-22 13:01:06.000000 rfswarm-manager-1.1.4/setup-manager.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-07-22 13:01:07.218849 rfswarm-manager-1.1.4/setup.cfg
```

### Comparing `rfswarm-manager-1.1.3/LICENSE` & `rfswarm-manager-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rfswarm-manager-1.1.3/PKG-INFO` & `rfswarm-manager-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfswarm-manager
-Version: 1.1.3
+Version: 1.1.4
 Summary: rfswarm manager
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
 License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
```

### Comparing `rfswarm-manager-1.1.3/README.md` & `rfswarm-manager-1.1.4/README.md`

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

### Comparing `rfswarm-manager-1.1.3/rfswarm_manager/rfswarm.py` & `rfswarm-manager-1.1.4/rfswarm_manager/rfswarm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 #
 # 	Robot Framework Swarm
 # 		Manager
-#    Version 1.1.3
+#    Version 1.1.4
 #
 
 # 	Helpful links
 #
 #
 
 import argparse
@@ -443,15 +443,15 @@
 	# 	log_request is here to stop BaseHTTPRequestHandler logging to the console
 	# 		https://stackoverflow.com/questions/10651052/how-to-quiet-simplehttpserver/10651257#10651257
 	def log_request(self, code='-', size='-'):
 		pass
 
 
 class RFSwarmBase:
-	version = "1.1.3"
+	version = "1.1.4"
 	debuglvl = 0
 
 	config = None
 	manager_ini = None
 
 	save_ini = True
 
@@ -1252,67 +1252,95 @@
 			base.debugmsg(8, "pathout:", pathout)
 
 		# ${EXECDIR}
 		# not sure how to handle this for now
 
 		# ${/}
 		if pathout.find("${/}") > -1:
+			base.debugmsg(8, "Found ${/} in", pathout)
 			if pathout.find("${/}") == 0:
-				pathlst = "${rfpv}" + pathout.split("${/}")
-				pathjoin = os.path.join(*pathlst)
+				pathlst = ["${rfpv}"] + pathout.split("${/}")
 				base.debugmsg(8, "pathlst:", pathlst)
+				pathjoin = os.path.join(*pathlst)
 				base.debugmsg(8, "pathjoin:", pathjoin)
 				pathjoin = pathjoin.replace("${rfpv}", "")
 				base.debugmsg(8, "pathjoin:", pathjoin)
 			else:
-				pathlst = "${rfpv}" + pathout.split("${/}")
-				pathjoin = os.path.join(*pathlst)
+				pathlst = pathout.split("${/}")
 				base.debugmsg(8, "pathlst:", pathlst)
+				pathjoin = os.path.join(*pathlst)
 				base.debugmsg(8, "pathjoin:", pathjoin)
 
 			if os.path.isfile(pathjoin):
+				base.debugmsg(8, "pathjoin:", pathjoin)
 				pathout = pathjoin
-			else:
 				base.debugmsg(8, "pathout:", pathout)
-				# i guess this could be affected too https://stackoverflow.com/questions/1945920/why-doesnt-os-path-join-work-in-this-case
-				if platform.system() == "Windows":
-					pathout = os.path.abspath(os.path.join(*localdir.split(os.path.sep), *pathjoin.split(os.path.sep)))
-				else:
-					pathout = os.path.abspath(os.path.join(os.path.sep, *localdir.split(os.path.sep), *pathjoin.split(os.path.sep)))
+			else:
+				base.debugmsg(8, "pathjoin:", pathjoin)
+				pathout = self.localrespath(localdir, pathjoin)
 				base.debugmsg(8, "pathout:", pathout)
 
 		# ${:}
 		# ${\n}
 		# not sure whether to handle these for now
+		base.debugmsg(8, "pathout:", pathout)
+
+		return pathout
+
+	def localrespath(self, localdir, resfile):
+		base.debugmsg(5, "localdir:", localdir)
+		base.debugmsg(5, "resfile:", resfile)
+		llocaldir = re.findall(r"[^\/\\]+", localdir)
+		lresfile = re.findall(r"[^\/\\]+", resfile)
+
+		base.debugmsg(5, "llocaldir:", llocaldir)
+		base.debugmsg(5, "lresfile:", lresfile)
+
+		# i guess this could be affected too https://stackoverflow.com/questions/1945920/why-doesnt-os-path-join-work-in-this-case
+		if platform.system() == "Windows":
+			joindpath = os.path.join(*llocaldir, *lresfile)
+		else:
+			joindpath = os.path.join(os.path.sep, *llocaldir, *lresfile)
+		base.debugmsg(5, "joindpath:", joindpath)
+
+		pathout = os.path.abspath(joindpath)
+		base.debugmsg(5, "pathout:", pathout)
 
 		return pathout
 
 	def find_dependancies(self, hash):
 		keep_going = True
 		checking = False
 
 		# determine if is a robot file
 		base.debugmsg(8, "scriptfiles[", hash, "]", self.scriptfiles[hash])
 		localpath = self.scriptfiles[hash]['localpath']
 		localdir = os.path.dirname(localpath)
+
+		if 'basedir' in self.scriptfiles[hash]:
+			basedir = self.scriptfiles[hash]['basedir']
+		else:
+			basedir = localdir
+
 		# look for __init__. files - Issue #90
 		initfiles = os.path.abspath(os.path.join(localdir, "__init__.*"))
 		base.debugmsg(7, "initfiles", initfiles)
 		filelst = glob.glob(initfiles)
 		for file in filelst:
 			base.debugmsg(7, "file:", file)
-			relpath = file.replace(localdir, "")[1:]
-			base.debugmsg(7, "relpath:", relpath)
-			newhash = self.hash_file(file, relpath)
+			relfile = os.path.relpath(file, start=basedir)
+			base.debugmsg(7, "relfile:", relfile)
+			newhash = self.hash_file(file, relfile)
 			base.debugmsg(7, "newhash:", newhash)
 			if newhash not in self.scriptfiles:
 				self.scriptfiles[newhash] = {
 					'id': newhash,
+					'basedir': basedir,
 					'localpath': file,
-					'relpath': relpath,
+					'relpath': relfile,
 					'type': "Initialization"
 				}
 				filename, fileext = os.path.splitext(file)
 				# splitext leaves the . on the extention, the list below needs to have the extentions
 				# starting with a . - Issue #94
 				if fileext.lower() in ['.robot', '.resource']:
 					t = threading.Thread(target=base.find_dependancies, args=(newhash, ))
@@ -1350,27 +1378,25 @@
 								if resfile:
 									base.debugmsg(7, "resfile", resfile)
 									# here we are assuming the resfile is a relative path! should we also consider files with full local paths?
 									# Issue #129 Handle ``${CURDIR}/``
 									if resfile.find("${") > -1:
 										localrespath = base.replace_rf_path_variables(resfile, localdir)
 									else:
-										# i guess this could be affected too https://stackoverflow.com/questions/1945920/why-doesnt-os-path-join-work-in-this-case
-										if platform.system() == "Windows":
-											localrespath = os.path.abspath(os.path.join(*localdir.split(os.path.sep), *resfile.split(os.path.sep)))
-										else:
-											localrespath = os.path.abspath(os.path.join(os.path.sep, *localdir.split(os.path.sep), *resfile.split(os.path.sep)))
+										localrespath = self.localrespath(localdir, resfile)
+
 									base.debugmsg(7, "localrespath", localrespath)
 									if os.path.isfile(localrespath):
-										relfile = os.path.relpath(localrespath, start=localdir)
+										relfile = os.path.relpath(localrespath, start=basedir)
 										base.debugmsg(7, "relfile", relfile)
 										newhash = self.hash_file(localrespath, relfile)
 										base.debugmsg(7, "newhash", newhash)
 										self.scriptfiles[newhash] = {
 											'id': newhash,
+											'basedir': basedir,
 											'localpath': localrespath,
 											'relpath': relfile,
 											'type': linearr[0]
 										}
 
 										t = threading.Thread(target=base.find_dependancies, args=(newhash, ))
 										t.start()
@@ -2147,18 +2173,26 @@
 		if 'Plan' not in base.config:
 			base.config['Plan'] = {}
 			base.saveini()
 
 		if 'ScriptDir' not in base.config['Plan']:
 			base.config['Plan']['ScriptDir'] = base.inisafevalue(base.dir_path)
 			base.saveini()
+		else:
+			if not os.path.isdir(base.config['Plan']['ScriptDir']):
+				base.config['Plan']['ScriptDir'] = base.inisafevalue(base.dir_path)
+				base.saveini()
 
 		if 'ScenarioDir' not in base.config['Plan']:
 			base.config['Plan']['ScenarioDir'] = base.inisafevalue(base.dir_path)
 			base.saveini()
+		else:
+			if not os.path.isdir(base.config['Plan']['ScenarioDir']):
+				base.config['Plan']['ScenarioDir'] = base.inisafevalue(base.dir_path)
+				base.saveini()
 
 		if 'ScenarioFile' not in base.config['Plan']:
 			base.config['Plan']['ScenarioFile'] = ""
 			base.saveini()
 		else:
 			# check file exists - it may have been deleted since rfswarm last ran with this ini file
 			if not os.path.exists(base.config['Plan']['ScenarioFile']):
@@ -2174,14 +2208,18 @@
 		if 'Run' not in base.config:
 			base.config['Run'] = {}
 			base.saveini()
 
 		if 'ResultsDir' not in base.config['Run']:
 			base.config['Run']['ResultsDir'] = base.inisafevalue(os.path.join(base.dir_path, "results"))
 			base.saveini()
+		else:
+			if not os.path.isdir(base.config['Run']['ResultsDir']):
+				base.config['Run']['ResultsDir'] = base.inisafevalue(base.dir_path)
+				base.saveini()
 
 		if 'display_index' not in base.config['Run']:
 			base.config['Run']['display_index'] = str(False)
 			base.saveini()
 
 		if 'display_iteration' not in base.config['Run']:
 			base.config['Run']['display_iteration'] = str(False)
@@ -4341,15 +4379,15 @@
 				FNType = grphWindow.settings["FNType"].get()
 				base.debugmsg(7, "FNType:", FNType)
 
 				inpFP = grphWindow.settings["FPattern"].get()
 				base.debugmsg(7, "inpFP:", inpFP)
 
 				sql = "SELECT "
-				sql += "  CAST(end_time as INTEGER) as 'endtime' "
+				sql += "  floor(end_time) as 'endtime' "
 				if RType == "Response Time":
 					sql += ", result_name "
 					sql += ", elapsed_time "
 				if RType == "TPS":
 					sql += ", count(result)  as 'count' "
 					sql += ", result_name "
 					sql += ", result "
@@ -4388,15 +4426,15 @@
 				for iwhere in lwhere:
 					if i == 0:
 						sql += "WHERE {} ".format(iwhere)
 					else:
 						sql += "AND {} ".format(iwhere)
 					i += 1
 
-				sql += "GROUP by CAST(end_time as INTEGER) "
+				sql += "GROUP by floor(end_time) "
 				if RType == "Response Time":
 					sql += ", result_name "
 					sql += ", elapsed_time "
 				if RType == "TPS":
 					sql += ", result_name "
 					sql += ", result "
 				if RType == "Total TPS":
```

### Comparing `rfswarm-manager-1.1.3/rfswarm_manager.egg-info/PKG-INFO` & `rfswarm-manager-1.1.4/rfswarm_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfswarm-manager
-Version: 1.1.3
+Version: 1.1.4
 Summary: rfswarm manager
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
 License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
```

### Comparing `rfswarm-manager-1.1.3/setup-manager.py` & `rfswarm-manager-1.1.4/setup-manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README_PyPi.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="rfswarm-manager",
-	version="1.1.3",
+	version="1.1.4",
 	author="damies13",
 	author_email="damies13+rfswarm@gmail.com",
 	description="rfswarm manager",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/damies13/rfswarm",
 	packages=setuptools.find_packages(exclude=["*fswarm_report*", "*fswarm_agen*", "build/*"]),
```

