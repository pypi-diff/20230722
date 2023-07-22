# Comparing `tmp/common_utils_pkg-0.1.4.tar.gz` & `tmp/common_utils_pkg-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common_utils_pkg-0.1.4.tar", last modified: Sun Jun 25 20:04:22 2023, max compression
+gzip compressed data, was "common_utils_pkg-0.1.5.tar", last modified: Sat Jul 22 21:07:45 2023, max compression
```

## Comparing `common_utils_pkg-0.1.4.tar` & `common_utils_pkg-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-06-25 20:04:22.444092 common_utils_pkg-0.1.4/
--rw-r--r--   0 nikitagetman   (501) staff       (20)      520 2023-06-25 20:04:22.443792 common_utils_pkg-0.1.4/PKG-INFO
-drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-06-25 20:04:22.440642 common_utils_pkg-0.1.4/common_utils_pkg/
--rw-r--r--   0 nikitagetman   (501) staff       (20)      162 2023-06-25 20:03:41.000000 common_utils_pkg-0.1.4/common_utils_pkg/__init__.py
--rw-r--r--   0 nikitagetman   (501) staff       (20)     1634 2023-06-25 20:03:50.000000 common_utils_pkg-0.1.4/common_utils_pkg/aws_adapter.py
--rw-r--r--   0 nikitagetman   (501) staff       (20)     3344 2023-06-14 15:33:57.000000 common_utils_pkg-0.1.4/common_utils_pkg/logger.py
--rw-r--r--   0 nikitagetman   (501) staff       (20)     1026 2023-05-28 07:07:47.000000 common_utils_pkg-0.1.4/common_utils_pkg/notifications.py
--rw-r--r--   0 nikitagetman   (501) staff       (20)     1021 2023-05-28 07:55:01.000000 common_utils_pkg-0.1.4/common_utils_pkg/scheduler.py
-drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-06-25 20:04:22.443241 common_utils_pkg-0.1.4/common_utils_pkg.egg-info/
--rw-r--r--   0 nikitagetman   (501) staff       (20)      520 2023-06-25 20:04:22.000000 common_utils_pkg-0.1.4/common_utils_pkg.egg-info/PKG-INFO
--rw-r--r--   0 nikitagetman   (501) staff       (20)      359 2023-06-25 20:04:22.000000 common_utils_pkg-0.1.4/common_utils_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 nikitagetman   (501) staff       (20)        1 2023-06-25 20:04:22.000000 common_utils_pkg-0.1.4/common_utils_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 nikitagetman   (501) staff       (20)       23 2023-06-25 20:04:22.000000 common_utils_pkg-0.1.4/common_utils_pkg.egg-info/requires.txt
--rw-r--r--   0 nikitagetman   (501) staff       (20)       17 2023-06-25 20:04:22.000000 common_utils_pkg-0.1.4/common_utils_pkg.egg-info/top_level.txt
--rw-r--r--   0 nikitagetman   (501) staff       (20)       38 2023-06-25 20:04:22.444222 common_utils_pkg-0.1.4/setup.cfg
--rw-r--r--   0 nikitagetman   (501) staff       (20)      802 2023-06-25 20:03:30.000000 common_utils_pkg-0.1.4/setup.py
+drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-07-22 21:07:45.260871 common_utils_pkg-0.1.5/
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      520 2023-07-22 21:07:45.260427 common_utils_pkg-0.1.5/PKG-INFO
+drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-07-22 21:07:45.256958 common_utils_pkg-0.1.5/common_utils_pkg/
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      162 2023-06-25 20:03:41.000000 common_utils_pkg-0.1.5/common_utils_pkg/__init__.py
+-rw-r--r--   0 nikitagetman   (501) staff       (20)     1860 2023-07-22 21:07:02.000000 common_utils_pkg-0.1.5/common_utils_pkg/aws_adapter.py
+-rw-r--r--   0 nikitagetman   (501) staff       (20)     3344 2023-06-14 15:33:57.000000 common_utils_pkg-0.1.5/common_utils_pkg/logger.py
+-rw-r--r--   0 nikitagetman   (501) staff       (20)     1026 2023-05-28 07:07:47.000000 common_utils_pkg-0.1.5/common_utils_pkg/notifications.py
+-rw-r--r--   0 nikitagetman   (501) staff       (20)     1021 2023-07-01 11:35:11.000000 common_utils_pkg-0.1.5/common_utils_pkg/scheduler.py
+drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-07-22 21:07:45.259939 common_utils_pkg-0.1.5/common_utils_pkg.egg-info/
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      520 2023-07-22 21:07:45.000000 common_utils_pkg-0.1.5/common_utils_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      359 2023-07-22 21:07:45.000000 common_utils_pkg-0.1.5/common_utils_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 nikitagetman   (501) staff       (20)        1 2023-07-22 21:07:45.000000 common_utils_pkg-0.1.5/common_utils_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 nikitagetman   (501) staff       (20)       23 2023-07-22 21:07:45.000000 common_utils_pkg-0.1.5/common_utils_pkg.egg-info/requires.txt
+-rw-r--r--   0 nikitagetman   (501) staff       (20)       17 2023-07-22 21:07:45.000000 common_utils_pkg-0.1.5/common_utils_pkg.egg-info/top_level.txt
+-rw-r--r--   0 nikitagetman   (501) staff       (20)       38 2023-07-22 21:07:45.261073 common_utils_pkg-0.1.5/setup.cfg
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      802 2023-07-22 21:07:39.000000 common_utils_pkg-0.1.5/setup.py
```

### Comparing `common_utils_pkg-0.1.4/PKG-INFO` & `common_utils_pkg-0.1.5/common_utils_pkg.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: common_utils_pkg
-Version: 0.1.4
+Name: common-utils-pkg
+Version: 0.1.5
 Summary: Common utils package. With some basic classes.
 Author: John Johny
 Author-email: love.dev.2020@email.com
 Keywords: python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `common_utils_pkg-0.1.4/common_utils_pkg/aws_adapter.py` & `common_utils_pkg-0.1.5/common_utils_pkg/aws_adapter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from .logger import Logger
 
 import boto3
+from boto3.s3.transfer import TransferConfig
 from botocore.exceptions import ClientError
 
 
 class AWSAdapter:
     def __init__(self, logger: Logger, region):
         self.logger = logger.create_prefix("AWSAdapter")
         self.region = region
 
     def upload_file_to_s3(self, bucket_name, file_path, file_key):
         try:
             self.logger.info(
                 f"Uploading file {file_path} to Bucket (region: {self.region}): {bucket_name} -> {file_key}"
             )
             s3_resource = boto3.resource("s3", region_name=self.region)
-            s3_resource.Bucket(bucket_name).upload_file(file_path, file_key)
+            config = TransferConfig(
+                multipart_threshold=1024 * 25, max_concurrency=10, multipart_chunksize=1024 * 25, use_threads=True
+            )
+            s3_resource.Bucket(bucket_name).upload_file(file_path, file_key, Config=config)
             self.logger.info(f"File {file_path} uploaded")
         except ClientError as e:
             self.logger.error(
                 f"Error uploading file {file_path} to Bucket: {bucket_name} -> {file_key}: {e.response['Error']['Message']}",
                 notify=True,
             )
```

### Comparing `common_utils_pkg-0.1.4/common_utils_pkg/logger.py` & `common_utils_pkg-0.1.5/common_utils_pkg/logger.py`

 * *Files identical despite different names*

### Comparing `common_utils_pkg-0.1.4/common_utils_pkg/notifications.py` & `common_utils_pkg-0.1.5/common_utils_pkg/notifications.py`

 * *Files identical despite different names*

### Comparing `common_utils_pkg-0.1.4/common_utils_pkg/scheduler.py` & `common_utils_pkg-0.1.5/common_utils_pkg/scheduler.py`

 * *Files identical despite different names*

### Comparing `common_utils_pkg-0.1.4/common_utils_pkg.egg-info/PKG-INFO` & `common_utils_pkg-0.1.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: common-utils-pkg
-Version: 0.1.4
+Name: common_utils_pkg
+Version: 0.1.5
 Summary: Common utils package. With some basic classes.
 Author: John Johny
 Author-email: love.dev.2020@email.com
 Keywords: python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `common_utils_pkg-0.1.4/setup.py` & `common_utils_pkg-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.1.4"
+VERSION = "0.1.5"
 DESCRIPTION = "Common utils package. With some basic classes."
 LONG_DESCRIPTION = "Package with common utils for new projects."
 
 setup(
     name="common_utils_pkg",
     version=VERSION,
     author="John Johny",
```

