# Comparing `tmp/rfswarm-reporter-1.1.3.tar.gz` & `tmp/rfswarm-reporter-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfswarm-reporter-1.1.3.tar", last modified: Sun Jun  4 05:25:59 2023, max compression
+gzip compressed data, was "rfswarm-reporter-1.1.4.tar", last modified: Sat Jul 22 13:01:08 2023, max compression
```

## Comparing `rfswarm-reporter-1.1.3.tar` & `rfswarm-reporter-1.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-04 05:25:59.893687 rfswarm-reporter-1.1.3/
--rw-r--r--   0 dave      (1000) dave      (1000)    35149 2023-02-10 08:46:44.000000 rfswarm-reporter-1.1.3/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)     3158 2023-06-04 05:25:59.893687 rfswarm-reporter-1.1.3/PKG-INFO
--rw-r--r--   0 dave      (1000) dave      (1000)     5809 2023-06-04 04:58:34.000000 rfswarm-reporter-1.1.3/README.md
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-04 05:25:59.893687 rfswarm-reporter-1.1.3/rfswarm_reporter/
--rw-r--r--   0 dave      (1000) dave      (1000)       53 2023-06-04 05:25:57.000000 rfswarm-reporter-1.1.3/rfswarm_reporter/__init__.py
--rw-r--r--   0 dave      (1000) dave      (1000)   312855 2023-06-04 05:25:57.000000 rfswarm-reporter-1.1.3/rfswarm_reporter/rfswarm_reporter.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-04 05:25:59.893687 rfswarm-reporter-1.1.3/rfswarm_reporter.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     3158 2023-06-04 05:25:59.000000 rfswarm-reporter-1.1.3/rfswarm_reporter.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      343 2023-06-04 05:25:59.000000 rfswarm-reporter-1.1.3/rfswarm_reporter.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-04 05:25:59.000000 rfswarm-reporter-1.1.3/rfswarm_reporter.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       80 2023-06-04 05:25:59.000000 rfswarm-reporter-1.1.3/rfswarm_reporter.egg-info/entry_points.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       85 2023-06-04 05:25:59.000000 rfswarm-reporter-1.1.3/rfswarm_reporter.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-06-04 05:25:59.000000 rfswarm-reporter-1.1.3/rfswarm_reporter.egg-info/top_level.txt
--rw-r--r--   0 dave      (1000) dave      (1000)     1504 2023-06-04 05:25:57.000000 rfswarm-reporter-1.1.3/setup-reporter.py
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-06-04 05:25:59.897687 rfswarm-reporter-1.1.3/setup.cfg
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-22 13:01:08.018849 rfswarm-reporter-1.1.4/
+-rw-r--r--   0 dave      (1000) dave      (1000)    35149 2023-02-10 08:46:44.000000 rfswarm-reporter-1.1.4/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3158 2023-07-22 13:01:08.018849 rfswarm-reporter-1.1.4/PKG-INFO
+-rw-r--r--   0 dave      (1000) dave      (1000)     6597 2023-07-22 12:53:23.000000 rfswarm-reporter-1.1.4/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-22 13:01:08.018849 rfswarm-reporter-1.1.4/rfswarm_reporter/
+-rw-r--r--   0 dave      (1000) dave      (1000)       53 2023-07-22 13:01:06.000000 rfswarm-reporter-1.1.4/rfswarm_reporter/__init__.py
+-rw-r--r--   0 dave      (1000) dave      (1000)   314079 2023-07-22 13:01:06.000000 rfswarm-reporter-1.1.4/rfswarm_reporter/rfswarm_reporter.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-22 13:01:08.018849 rfswarm-reporter-1.1.4/rfswarm_reporter.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3158 2023-07-22 13:01:07.000000 rfswarm-reporter-1.1.4/rfswarm_reporter.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      343 2023-07-22 13:01:07.000000 rfswarm-reporter-1.1.4/rfswarm_reporter.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-22 13:01:07.000000 rfswarm-reporter-1.1.4/rfswarm_reporter.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       80 2023-07-22 13:01:07.000000 rfswarm-reporter-1.1.4/rfswarm_reporter.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       85 2023-07-22 13:01:07.000000 rfswarm-reporter-1.1.4/rfswarm_reporter.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-07-22 13:01:07.000000 rfswarm-reporter-1.1.4/rfswarm_reporter.egg-info/top_level.txt
+-rw-r--r--   0 dave      (1000) dave      (1000)     1504 2023-07-22 13:01:06.000000 rfswarm-reporter-1.1.4/setup-reporter.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-07-22 13:01:08.018849 rfswarm-reporter-1.1.4/setup.cfg
```

### Comparing `rfswarm-reporter-1.1.3/LICENSE` & `rfswarm-reporter-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rfswarm-reporter-1.1.3/PKG-INFO` & `rfswarm-reporter-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfswarm-reporter
-Version: 1.1.3
+Version: 1.1.4
 Summary: rfswarm reporter
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
 License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
```

### Comparing `rfswarm-reporter-1.1.3/README.md` & `rfswarm-reporter-1.1.4/README.md`

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

### Comparing `rfswarm-reporter-1.1.3/rfswarm_reporter/rfswarm_reporter.py` & `rfswarm-reporter-1.1.4/rfswarm_reporter/rfswarm_reporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 #
 # 	Robot Framework Swarm
 # 		Reporter
-#    Version 1.1.3
+#    Version 1.1.4
 #
 
 import argparse
 import base64  # used for embedding images  # used for xhtml export
 import configparser
 import inspect
 import math
@@ -114,15 +114,15 @@
 			base.debugmsg(8, "res:", res)
 			return res
 		except Exception as e:
 			base.debugmsg(5, "Exception:", e)
 
 
 class ReporterBase():
-	version = "1.1.3"
+	version = "1.1.4"
 	debuglvl = 0
 
 	save_ini = True
 	running = True
 	displaygui = True
 	gui = None
 	darkmode = False
@@ -319,20 +319,22 @@
 	#
 	# Report Functions
 	#
 
 	def report_save(self):
 		saved = False
 		if 'Reporter' in base.config:
-			if 'Report' in base.config['Reporter']:
+			if 'Report' in base.config['Reporter'] and len(base.config['Reporter']['Report']) > 0:
 				filename = base.config['Reporter']['Report']
-				with open(filename, 'w', encoding="utf8") as reportfile:    # save
-					base.report.write(reportfile)
-					self.debugmsg(6, "Report Saved:", filename)
-					saved = True
+				filedir = os.path.dirname(filename)
+				if os.path.isdir(filedir):
+					with open(filename, 'w', encoding="utf8") as reportfile:    # save
+						base.report.write(reportfile)
+						self.debugmsg(6, "Report Saved:", filename)
+						saved = True
 		return saved
 
 	def report_open(self):
 		filename = base.config['Reporter']['Report']
 		base.debugmsg(7, "filename: ", filename)
 		base.reportdata = {}
 		base.report = None
@@ -973,25 +975,25 @@
 				# sql += 		"count(ro.result) as _other "
 				# sql += "FROM Results as r "
 				# sql += 		"LEFT JOIN Results as rp ON r.rowid == rp.rowid AND rp.result == 'PASS' "
 				# sql += 		"LEFT JOIN Results as rf ON r.rowid == rf.rowid AND rf.result == 'FAIL' "
 				# sql += 		"LEFT JOIN Results as ro ON r.rowid == ro.rowid AND ro.result <> 'PASS' AND ro.result <> 'FAIL' "
 
 			if RType == "TPS":
-				sql += "end_time as 'Time' "
+				sql += "floor(end_time) as 'Time' "
 				sql += ", count(result) as 'Value' "
 				# sql += ", result_name as 'Name' "
 				sql += ", result_name"
 				if EnFR and FRType in [None, "", "None"]:
 					sql += " || ' - ' || result"
 				if EnFA and FAType in [None, "", "None"]:
 					sql += " || ' - ' || agent"
 				sql += " as [" + colname + "] "
 			if RType == "Total TPS":
-				sql += "end_time as 'Time'"
+				sql += "floor(end_time) as 'Time'"
 				sql += ", count(result) as 'Value' "
 				# sql += ", result as 'Name' "
 				sql += ", result"
 				if EnFR and FRType in [None, "", "None"]:
 					sql += " || ' - ' || result"
 				if EnFA and FAType in [None, "", "None"]:
 					sql += " || ' - ' || agent"
@@ -1064,22 +1066,28 @@
 				pass
 			if RType == "Response Time":
 				# sql += 		"result_name "
 				pass
 
 			if RType == "TPS":
 				sql += "GROUP by "
-				sql += "end_time "
+				sql += "floor(end_time) "
 				sql += ", result_name "
 				sql += ", result "
-				sql += "ORDER by end_time, result DESC, count(result) DESC "
+				sql += "ORDER by "
+				sql += "floor(end_time)"
+				sql += ", result DESC"
+				sql += ", count(result) DESC "
 			if RType == "Total TPS":
-				sql += "end_time "
+				sql += "GROUP by "
+				sql += "floor(end_time) "
 				sql += ", result "
-				sql += "ORDER by end_time, count(result) DESC "
+				sql += "ORDER by "
+				sql += "floor(end_time)"
+				sql += ", count(result) DESC "
 
 		if DataType == "Metric":
 			MType = self.rt_table_get_mt(id)
 			PM = self.rt_table_get_pm(id)
 			SM = self.rt_table_get_sm(id)
 			# isnum = self.rt_table_get_isnumeric(id)
 			# sc = self.rt_table_get_showcount(id)
@@ -1369,18 +1377,21 @@
 				sql += "GROUP by "
 
 			if RType == "Response Time":
 				sql += "[" + colname + "] "
 			if RType == "TPS":
 				sql += "[" + colname + "] "
 				sql += ", result "
-				sql += "ORDER by result DESC, count(result) DESC "
+				sql += "ORDER BY "
+				sql += "result DESC"
+				sql += ", count(result) DESC "
 			if RType == "Total TPS":
 				sql += " [" + colname + "] "
-				sql += "ORDER by count([" + colname + "]) DESC "
+				sql += "ORDER BY "
+				sql += "count([" + colname + "]) DESC "
 
 		if DataType == "Metric":
 			MType = self.rt_table_get_mt(id)
 			PM = self.rt_table_get_pm(id)
 			SM = self.rt_table_get_sm(id)
 			isnum = self.rt_table_get_isnumeric(id)
 			sc = self.rt_table_get_showcount(id)
@@ -1419,15 +1430,14 @@
 			if SM not in [None, "", "None"] and len(SM) > 0:
 				if "SecondaryMetric" in mcolumns:
 					mcolumns.remove("SecondaryMetric")
 				wherelst.append("SecondaryMetric == '{}'".format(SM))
 				if "SecondaryMetric" in grouplst:
 					grouplst.remove("SecondaryMetric")
 
-
 			if len(mcolumns) < 1:
 				# mcolumns.append("'" + SM + "'")
 				mcolumns.append("SecondaryMetric")
 				grouplst.append("SecondaryMetric")
 
 			if colours:
 				colourcolumn = " || ' - ' || ".join(grouplst)
@@ -2389,26 +2399,50 @@
 		if 'Reporter' not in base.config:
 			base.config['Reporter'] = {}
 			base.saveini()
 
 		if 'ResultDir' not in base.config['Reporter']:
 			base.config['Reporter']['ResultDir'] = base.dir_path
 			base.saveini()
+		else:
+			if not os.path.isdir(base.config['Reporter']['ResultDir']):
+				base.config['Reporter']['ResultDir'] = base.dir_path
+				base.saveini()
 
 		if 'Results' not in base.config['Reporter']:
 			base.config['Reporter']['Results'] = ""
 			base.saveini()
+		else:
+			if not os.path.isfile(base.config['Reporter']['Results']):
+				base.config['Reporter']['Results'] = ""
+				base.saveini()
+
+		if 'Report' not in base.config['Reporter']:
+			base.config['Reporter']['Report'] = ""
+			base.saveini()
+		else:
+			if not os.path.isfile(base.config['Reporter']['Report']):
+				base.config['Reporter']['Report'] = ""
+				base.saveini()
 
 		if 'Template' not in base.config['Reporter']:
 			base.config['Reporter']['Template'] = ""
 			base.saveini()
+		else:
+			if not os.path.isfile(base.config['Reporter']['Template']):
+				base.config['Reporter']['Template'] = ""
+				base.saveini()
 
 		if 'TemplateDir' not in base.config['Reporter']:
 			base.config['Reporter']['TemplateDir'] = ""
 			base.saveini()
+		else:
+			if not os.path.isdir(base.config['Reporter']['TemplateDir']):
+				base.config['Reporter']['TemplateDir'] = ""
+				base.saveini()
 
 		usetemplate = False
 		if base.args.template:
 			usetemplate = True
 			base.config['Reporter']['Template'] = base.whitespace_set_ini_value(base.args.template)
 
 		if base.args.dir:
@@ -6902,15 +6936,21 @@
 
 	#
 	# Preview
 	#
 
 	def content_preview(self, id):
 		base.debugmsg(9, "id:", id)
-		self.updateStatus("Preview Loading.....")
+
+		if base.config['Reporter']['Results']:
+			self.updateStatus("Preview Loading.....")
+		else:
+			sres = "Please select a result file"
+			self.updateStatus(sres)
+			return None
 		try:
 			self.cp_generate_preview(id)
 		except Exception as e:
 			base.debugmsg(5, "e:", e)
 
 		# self.t_preview[id] = threading.Thread(target=lambda: self.cp_generate_preview(id))
 		# self.t_preview[id].start()
```

### Comparing `rfswarm-reporter-1.1.3/rfswarm_reporter.egg-info/PKG-INFO` & `rfswarm-reporter-1.1.4/rfswarm_reporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfswarm-reporter
-Version: 1.1.3
+Version: 1.1.4
 Summary: rfswarm reporter
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
 License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
```

### Comparing `rfswarm-reporter-1.1.3/setup-reporter.py` & `rfswarm-reporter-1.1.4/setup-reporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README_PyPi.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="rfswarm-reporter",
-	version="1.1.3",
+	version="1.1.4",
 	author="damies13",
 	author_email="damies13+rfswarm@gmail.com",
 	description="rfswarm reporter",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/damies13/rfswarm",
 	packages=setuptools.find_packages(exclude=["*fswarm_manag*", "*fswarm_agen*", "build/*"]),
```

