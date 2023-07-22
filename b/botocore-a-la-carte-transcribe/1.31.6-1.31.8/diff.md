# Comparing `tmp/botocore-a-la-carte-transcribe-1.31.6.tar.gz` & `tmp/botocore-a-la-carte-transcribe-1.31.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-transcribe-1.31.6.tar", last modified: Thu Jul 20 01:20:45 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-transcribe-1.31.8.tar", last modified: Fri Jul 21 01:21:55 2023, max compression
```

## Comparing `botocore-a-la-carte-transcribe-1.31.6.tar` & `botocore-a-la-carte-transcribe-1.31.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:45.142916 botocore-a-la-carte-transcribe-1.31.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-20 01:20:44.000000 botocore-a-la-carte-transcribe-1.31.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-20 01:20:45.142916 botocore-a-la-carte-transcribe-1.31.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:45.142916 botocore-a-la-carte-transcribe-1.31.6/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:45.142916 botocore-a-la-carte-transcribe-1.31.6/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:45.142916 botocore-a-la-carte-transcribe-1.31.6/botocore/data/transcribe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:45.142916 botocore-a-la-carte-transcribe-1.31.6/botocore/data/transcribe/2017-10-26/
--rw-r--r--   0 runner    (1001) docker     (123)    23887 2023-07-20 01:19:55.000000 botocore-a-la-carte-transcribe-1.31.6/botocore/data/transcribe/2017-10-26/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 01:19:55.000000 botocore-a-la-carte-transcribe-1.31.6/botocore/data/transcribe/2017-10-26/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 01:19:55.000000 botocore-a-la-carte-transcribe-1.31.6/botocore/data/transcribe/2017-10-26/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   239580 2023-07-20 01:19:55.000000 botocore-a-la-carte-transcribe-1.31.6/botocore/data/transcribe/2017-10-26/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:45.142916 botocore-a-la-carte-transcribe-1.31.6/botocore_a_la_carte_transcribe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-20 01:20:45.000000 botocore-a-la-carte-transcribe-1.31.6/botocore_a_la_carte_transcribe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-20 01:20:45.000000 botocore-a-la-carte-transcribe-1.31.6/botocore_a_la_carte_transcribe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 01:20:45.000000 botocore-a-la-carte-transcribe-1.31.6/botocore_a_la_carte_transcribe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 01:20:45.000000 botocore-a-la-carte-transcribe-1.31.6/botocore_a_la_carte_transcribe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 01:20:45.142916 botocore-a-la-carte-transcribe-1.31.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-20 01:20:44.000000 botocore-a-la-carte-transcribe-1.31.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:55.751556 botocore-a-la-carte-transcribe-1.31.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:55.000000 botocore-a-la-carte-transcribe-1.31.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-21 01:21:55.751556 botocore-a-la-carte-transcribe-1.31.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:55.747555 botocore-a-la-carte-transcribe-1.31.8/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:55.747555 botocore-a-la-carte-transcribe-1.31.8/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:55.747555 botocore-a-la-carte-transcribe-1.31.8/botocore/data/transcribe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:55.747555 botocore-a-la-carte-transcribe-1.31.8/botocore/data/transcribe/2017-10-26/
+-rw-r--r--   0 runner    (1001) docker     (123)    23887 2023-07-21 01:21:06.000000 botocore-a-la-carte-transcribe-1.31.8/botocore/data/transcribe/2017-10-26/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 01:21:06.000000 botocore-a-la-carte-transcribe-1.31.8/botocore/data/transcribe/2017-10-26/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 01:21:06.000000 botocore-a-la-carte-transcribe-1.31.8/botocore/data/transcribe/2017-10-26/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   241463 2023-07-21 01:21:06.000000 botocore-a-la-carte-transcribe-1.31.8/botocore/data/transcribe/2017-10-26/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:55.751556 botocore-a-la-carte-transcribe-1.31.8/botocore_a_la_carte_transcribe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-21 01:21:55.000000 botocore-a-la-carte-transcribe-1.31.8/botocore_a_la_carte_transcribe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-21 01:21:55.000000 botocore-a-la-carte-transcribe-1.31.8/botocore_a_la_carte_transcribe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:55.000000 botocore-a-la-carte-transcribe-1.31.8/botocore_a_la_carte_transcribe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:55.000000 botocore-a-la-carte-transcribe-1.31.8/botocore_a_la_carte_transcribe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:55.751556 botocore-a-la-carte-transcribe-1.31.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-21 01:21:55.000000 botocore-a-la-carte-transcribe-1.31.8/setup.py
```

### Comparing `botocore-a-la-carte-transcribe-1.31.6/LICENSE.txt` & `botocore-a-la-carte-transcribe-1.31.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-transcribe-1.31.6/PKG-INFO` & `botocore-a-la-carte-transcribe-1.31.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-transcribe
-Version: 1.31.6
+Version: 1.31.8
 Summary: transcribe data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-transcribe-1.31.6/botocore/data/transcribe/2017-10-26/endpoint-rule-set-1.json` & `botocore-a-la-carte-transcribe-1.31.8/botocore/data/transcribe/2017-10-26/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-transcribe-1.31.6/botocore/data/transcribe/2017-10-26/service-2.json` & `botocore-a-la-carte-transcribe-1.31.8/botocore/data/transcribe/2017-10-26/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978877923976608%*

 * *Differences: {"'shapes'": "{'StartTranscriptionJobRequest': {'members': {'ToxicityDetection': "*

 * *             "OrderedDict([('shape', 'ToxicityDetection'), ('documentation', '<p>Enables toxic "*

 * *             'speech detection in your transcript. If you include <code>ToxicityDetection</code> '*

 * *             'in your request, you must also include <code>ToxicityCategories</code>.</p> <p>For '*

 * *             'information on the types of toxic speech Amazon Transcribe can detect, see <a '*

 * *             'href="https://docs.aws.ama […]*

```diff
@@ -3224,14 +3224,18 @@
                     "documentation": "<p>Produces subtitle files for your input media. You can specify WebVTT (*.vtt) and SubRip (*.srt) formats.</p>",
                     "shape": "Subtitles"
                 },
                 "Tags": {
                     "documentation": "<p>Adds one or more custom tags, each in the form of a key:value pair, to a new transcription job at the time you start this new job.</p> <p>To learn more about using tags with Amazon Transcribe, refer to <a href=\"https://docs.aws.amazon.com/transcribe/latest/dg/tagging.html\">Tagging resources</a>.</p>",
                     "shape": "TagList"
                 },
+                "ToxicityDetection": {
+                    "documentation": "<p>Enables toxic speech detection in your transcript. If you include <code>ToxicityDetection</code> in your request, you must also include <code>ToxicityCategories</code>.</p> <p>For information on the types of toxic speech Amazon Transcribe can detect, see <a href=\"https://docs.aws.amazon.com/transcribe/latest/dg/toxic-language.html\">Detecting toxic speech</a>.</p>",
+                    "shape": "ToxicityDetection"
+                },
                 "TranscriptionJobName": {
                     "documentation": "<p>A unique name, chosen by you, for your transcription job. The name that you specify is also used as the default name of your transcription output file. If you want to specify a different name for your transcription output, use the <code>OutputKey</code> parameter.</p> <p>This name is case sensitive, cannot contain spaces, and must be unique within an Amazon Web Services account. If you try to create a new job with the same name as an existing job, you get a <code>ConflictException</code> error.</p>",
                     "shape": "TranscriptionJobName"
                 }
             },
             "required": [
                 "TranscriptionJobName",
@@ -3380,14 +3384,49 @@
             "type": "string"
         },
         "TimestampMilliseconds": {
             "max": 14400000,
             "min": 0,
             "type": "long"
         },
+        "ToxicityCategories": {
+            "max": 1,
+            "member": {
+                "shape": "ToxicityCategory"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "ToxicityCategory": {
+            "enum": [
+                "ALL"
+            ],
+            "type": "string"
+        },
+        "ToxicityDetection": {
+            "max": 1,
+            "member": {
+                "shape": "ToxicityDetectionSettings"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "ToxicityDetectionSettings": {
+            "documentation": "<p>Contains <code>ToxicityCategories</code>, which is a required parameter if you want to enable toxicity detection (<code>ToxicityDetection</code>) in your transcription request.</p>",
+            "members": {
+                "ToxicityCategories": {
+                    "documentation": "<p> If you include <code>ToxicityDetection</code> in your transcription request, you must also include <code>ToxicityCategories</code>. The only accepted value for this parameter is <code>ALL</code>.</p>",
+                    "shape": "ToxicityCategories"
+                }
+            },
+            "required": [
+                "ToxicityCategories"
+            ],
+            "type": "structure"
+        },
         "TranscribeArn": {
             "max": 1011,
             "min": 1,
             "pattern": "arn:aws(-[^:]+)?:transcribe:[a-zA-Z0-9-]*:[0-9]{12}:[a-zA-Z-]*/[0-9a-zA-Z._-]+",
             "type": "string"
         },
         "Transcript": {
@@ -3523,14 +3562,18 @@
                     "documentation": "<p>Indicates whether subtitles were generated with your transcription.</p>",
                     "shape": "SubtitlesOutput"
                 },
                 "Tags": {
                     "documentation": "<p>The tags, each in the form of a key:value pair, assigned to the specified transcription job.</p>",
                     "shape": "TagList"
                 },
+                "ToxicityDetection": {
+                    "documentation": "<p>Provides information about the toxicity detection settings applied to your transcription.</p>",
+                    "shape": "ToxicityDetection"
+                },
                 "Transcript": {
                     "documentation": "<p>Provides you with the Amazon S3 URI you can use to access your transcript.</p>",
                     "shape": "Transcript"
                 },
                 "TranscriptionJobName": {
                     "documentation": "<p>The name of the transcription job. Job names are case sensitive and must be unique within an Amazon Web Services account.</p>",
                     "shape": "TranscriptionJobName"
@@ -3609,14 +3652,18 @@
                     "documentation": "<p>Indicates where the specified transcription output is stored.</p> <p>If the value is <code>CUSTOMER_BUCKET</code>, the location is the Amazon S3 bucket you specified using the <code>OutputBucketName</code> parameter in your request. If you also included <code>OutputKey</code> in your request, your output is located in the path you specified in your request.</p> <p>If the value is <code>SERVICE_BUCKET</code>, the location is a service-managed Amazon S3 bucket. To access a transcript stored in a service-managed bucket, use the URI shown in the <code>TranscriptFileUri</code> or <code>RedactedTranscriptFileUri</code> field.</p>",
                     "shape": "OutputLocationType"
                 },
                 "StartTime": {
                     "documentation": "<p>The date and time your transcription job began processing.</p> <p>Timestamps are in the format <code>YYYY-MM-DD'T'HH:MM:SS.SSSSSS-UTC</code>. For example, <code>2022-05-04T12:32:58.789000-07:00</code> represents a transcription job that started processing at 12:32 PM UTC-7 on May 4, 2022.</p>",
                     "shape": "DateTime"
                 },
+                "ToxicityDetection": {
+                    "documentation": "<p>Indicates whether toxicity detection was enabled for the specified transcription job.</p>",
+                    "shape": "ToxicityDetection"
+                },
                 "TranscriptionJobName": {
                     "documentation": "<p>The name of the transcription job. Job names are case sensitive and must be unique within an Amazon Web Services account.</p>",
                     "shape": "TranscriptionJobName"
                 },
                 "TranscriptionJobStatus": {
                     "documentation": "<p>Provides the status of your transcription job.</p> <p>If the status is <code>COMPLETED</code>, the job is finished and you can find the results at the location specified in <code>TranscriptFileUri</code> (or <code>RedactedTranscriptFileUri</code>, if you requested transcript redaction). If the status is <code>FAILED</code>, <code>FailureReason</code> provides details on why your transcription job failed.</p>",
                     "shape": "TranscriptionJobStatus"
```

### Comparing `botocore-a-la-carte-transcribe-1.31.6/botocore_a_la_carte_transcribe.egg-info/PKG-INFO` & `botocore-a-la-carte-transcribe-1.31.8/botocore_a_la_carte_transcribe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-transcribe
-Version: 1.31.6
+Version: 1.31.8
 Summary: transcribe data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-transcribe-1.31.6/setup.py` & `botocore-a-la-carte-transcribe-1.31.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-transcribe',
-    version="1.31.6",
+    version="1.31.8",
     description='transcribe data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/transcribe/*/*.json'],
```

