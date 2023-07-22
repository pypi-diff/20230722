# Comparing `tmp/gammarer.aws-ec2-instance-running-scheduler-0.4.5.tar.gz` & `tmp/gammarer.aws-ec2-instance-running-scheduler-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-ec2-instance-running-scheduler-0.4.5.tar", last modified: Fri Jul 21 19:19:42 2023, max compression
+gzip compressed data, was "gammarer.aws-ec2-instance-running-scheduler-0.4.6.tar", last modified: Sat Jul 22 19:19:19 2023, max compression
```

## Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.5.tar` & `gammarer.aws-ec2-instance-running-scheduler-0.4.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:19:42.387485 gammarer.aws-ec2-instance-running-scheduler-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-21 19:19:26.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 19:19:26.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-21 19:19:42.387485 gammarer.aws-ec2-instance-running-scheduler-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-21 19:19:26.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-21 19:19:26.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 19:19:42.387485 gammarer.aws-ec2-instance-running-scheduler-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-21 19:19:26.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:19:42.383485 gammarer.aws-ec2-instance-running-scheduler-0.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:19:42.383485 gammarer.aws-ec2-instance-running-scheduler-0.4.5/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:19:42.383485 gammarer.aws-ec2-instance-running-scheduler-0.4.5/src/gammarer/aws_ec2_instance_running_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)    10824 2023-07-21 19:19:26.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.5/src/gammarer/aws_ec2_instance_running_scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:19:42.387485 gammarer.aws-ec2-instance-running-scheduler-0.4.5/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-21 19:19:26.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.5/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20664 2023-07-21 19:19:26.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.5/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@0.4.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:19:26.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.5/src/gammarer/aws_ec2_instance_running_scheduler/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:19:42.383485 gammarer.aws-ec2-instance-running-scheduler-0.4.5/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-21 19:19:42.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.5/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-21 19:19:42.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.5/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:19:42.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.5/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-21 19:19:42.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.5/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 19:19:42.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.5/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:19:19.440359 gammarer.aws-ec2-instance-running-scheduler-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-22 19:19:06.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-22 19:19:06.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-22 19:19:19.440359 gammarer.aws-ec2-instance-running-scheduler-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-22 19:19:06.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-22 19:19:06.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 19:19:19.440359 gammarer.aws-ec2-instance-running-scheduler-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-22 19:19:06.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:19:19.440359 gammarer.aws-ec2-instance-running-scheduler-0.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:19:19.440359 gammarer.aws-ec2-instance-running-scheduler-0.4.6/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:19:19.440359 gammarer.aws-ec2-instance-running-scheduler-0.4.6/src/gammarer/aws_ec2_instance_running_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)    10824 2023-07-22 19:19:06.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.6/src/gammarer/aws_ec2_instance_running_scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:19:19.440359 gammarer.aws-ec2-instance-running-scheduler-0.4.6/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-22 19:19:06.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.6/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20664 2023-07-22 19:19:06.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.6/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@0.4.6.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 19:19:06.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.6/src/gammarer/aws_ec2_instance_running_scheduler/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:19:19.440359 gammarer.aws-ec2-instance-running-scheduler-0.4.6/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-22 19:19:19.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.6/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-22 19:19:19.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.6/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 19:19:19.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.6/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-22 19:19:19.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.6/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 19:19:19.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.6/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/top_level.txt
```

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.5/LICENSE` & `gammarer.aws-ec2-instance-running-scheduler-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.5/PKG-INFO` & `gammarer.aws-ec2-instance-running-scheduler-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ec2-instance-running-scheduler
-Version: 0.4.5
+Version: 0.4.6
 Summary: AWS EC2 Instance Running Scheduler
 Home-page: https://github.com/yicr/aws-ec2-instance-running-scheduler.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ec2-instance-running-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.5/README.md` & `gammarer.aws-ec2-instance-running-scheduler-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.5/setup.py` & `gammarer.aws-ec2-instance-running-scheduler-0.4.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-ec2-instance-running-scheduler",
-    "version": "0.4.5",
+    "version": "0.4.6",
     "description": "AWS EC2 Instance Running Scheduler",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-ec2-instance-running-scheduler.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_ec2_instance_running_scheduler",
         "gammarer.aws_ec2_instance_running_scheduler._jsii"
     ],
     "package_data": {
         "gammarer.aws_ec2_instance_running_scheduler._jsii": [
-            "aws-ec2-instance-running-scheduler@0.4.5.jsii.tgz"
+            "aws-ec2-instance-running-scheduler@0.4.6.jsii.tgz"
         ],
         "gammarer.aws_ec2_instance_running_scheduler": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.5/src/gammarer/aws_ec2_instance_running_scheduler/__init__.py` & `gammarer.aws-ec2-instance-running-scheduler-0.4.6/src/gammarer/aws_ec2_instance_running_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.5/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/PKG-INFO` & `gammarer.aws-ec2-instance-running-scheduler-0.4.6/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ec2-instance-running-scheduler
-Version: 0.4.5
+Version: 0.4.6
 Summary: AWS EC2 Instance Running Scheduler
 Home-page: https://github.com/yicr/aws-ec2-instance-running-scheduler.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ec2-instance-running-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.5/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt` & `gammarer.aws-ec2-instance-running-scheduler-0.4.6/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt
 src/gammarer.aws_ec2_instance_running_scheduler.egg-info/dependency_links.txt
 src/gammarer.aws_ec2_instance_running_scheduler.egg-info/requires.txt
 src/gammarer.aws_ec2_instance_running_scheduler.egg-info/top_level.txt
 src/gammarer/aws_ec2_instance_running_scheduler/__init__.py
 src/gammarer/aws_ec2_instance_running_scheduler/py.typed
 src/gammarer/aws_ec2_instance_running_scheduler/_jsii/__init__.py
-src/gammarer/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@0.4.5.jsii.tgz
+src/gammarer/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@0.4.6.jsii.tgz
```

