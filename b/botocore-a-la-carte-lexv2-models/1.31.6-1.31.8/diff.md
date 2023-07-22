# Comparing `tmp/botocore-a-la-carte-lexv2-models-1.31.6.tar.gz` & `tmp/botocore-a-la-carte-lexv2-models-1.31.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-lexv2-models-1.31.6.tar", last modified: Thu Jul 20 01:20:29 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-lexv2-models-1.31.8.tar", last modified: Fri Jul 21 01:21:39 2023, max compression
```

## Comparing `botocore-a-la-carte-lexv2-models-1.31.6.tar` & `botocore-a-la-carte-lexv2-models-1.31.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:29.554762 botocore-a-la-carte-lexv2-models-1.31.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-20 01:20:29.000000 botocore-a-la-carte-lexv2-models-1.31.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-20 01:20:29.554762 botocore-a-la-carte-lexv2-models-1.31.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:29.554762 botocore-a-la-carte-lexv2-models-1.31.6/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:29.554762 botocore-a-la-carte-lexv2-models-1.31.6/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:29.554762 botocore-a-la-carte-lexv2-models-1.31.6/botocore/data/lexv2-models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:29.554762 botocore-a-la-carte-lexv2-models-1.31.6/botocore/data/lexv2-models/2020-08-07/
--rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-07-20 01:19:55.000000 botocore-a-la-carte-lexv2-models-1.31.6/botocore/data/lexv2-models/2020-08-07/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 01:19:55.000000 botocore-a-la-carte-lexv2-models-1.31.6/botocore/data/lexv2-models/2020-08-07/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 01:19:55.000000 botocore-a-la-carte-lexv2-models-1.31.6/botocore/data/lexv2-models/2020-08-07/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   594234 2023-07-20 01:19:55.000000 botocore-a-la-carte-lexv2-models-1.31.6/botocore/data/lexv2-models/2020-08-07/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-07-20 01:19:55.000000 botocore-a-la-carte-lexv2-models-1.31.6/botocore/data/lexv2-models/2020-08-07/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:29.554762 botocore-a-la-carte-lexv2-models-1.31.6/botocore_a_la_carte_lexv2_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-20 01:20:29.000000 botocore-a-la-carte-lexv2-models-1.31.6/botocore_a_la_carte_lexv2_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-20 01:20:29.000000 botocore-a-la-carte-lexv2-models-1.31.6/botocore_a_la_carte_lexv2_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 01:20:29.000000 botocore-a-la-carte-lexv2-models-1.31.6/botocore_a_la_carte_lexv2_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 01:20:29.000000 botocore-a-la-carte-lexv2-models-1.31.6/botocore_a_la_carte_lexv2_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 01:20:29.554762 botocore-a-la-carte-lexv2-models-1.31.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-20 01:20:29.000000 botocore-a-la-carte-lexv2-models-1.31.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:39.059247 botocore-a-la-carte-lexv2-models-1.31.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:38.000000 botocore-a-la-carte-lexv2-models-1.31.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-21 01:21:39.059247 botocore-a-la-carte-lexv2-models-1.31.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:39.059247 botocore-a-la-carte-lexv2-models-1.31.8/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:39.059247 botocore-a-la-carte-lexv2-models-1.31.8/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:39.059247 botocore-a-la-carte-lexv2-models-1.31.8/botocore/data/lexv2-models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:39.059247 botocore-a-la-carte-lexv2-models-1.31.8/botocore/data/lexv2-models/2020-08-07/
+-rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-07-21 01:21:06.000000 botocore-a-la-carte-lexv2-models-1.31.8/botocore/data/lexv2-models/2020-08-07/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 01:21:06.000000 botocore-a-la-carte-lexv2-models-1.31.8/botocore/data/lexv2-models/2020-08-07/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 01:21:06.000000 botocore-a-la-carte-lexv2-models-1.31.8/botocore/data/lexv2-models/2020-08-07/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   595154 2023-07-21 01:21:06.000000 botocore-a-la-carte-lexv2-models-1.31.8/botocore/data/lexv2-models/2020-08-07/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-07-21 01:21:06.000000 botocore-a-la-carte-lexv2-models-1.31.8/botocore/data/lexv2-models/2020-08-07/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:39.059247 botocore-a-la-carte-lexv2-models-1.31.8/botocore_a_la_carte_lexv2_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-21 01:21:39.000000 botocore-a-la-carte-lexv2-models-1.31.8/botocore_a_la_carte_lexv2_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-21 01:21:39.000000 botocore-a-la-carte-lexv2-models-1.31.8/botocore_a_la_carte_lexv2_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:39.000000 botocore-a-la-carte-lexv2-models-1.31.8/botocore_a_la_carte_lexv2_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:39.000000 botocore-a-la-carte-lexv2-models-1.31.8/botocore_a_la_carte_lexv2_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:39.059247 botocore-a-la-carte-lexv2-models-1.31.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-21 01:21:38.000000 botocore-a-la-carte-lexv2-models-1.31.8/setup.py
```

### Comparing `botocore-a-la-carte-lexv2-models-1.31.6/LICENSE.txt` & `botocore-a-la-carte-lexv2-models-1.31.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lexv2-models-1.31.6/PKG-INFO` & `botocore-a-la-carte-lexv2-models-1.31.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-lexv2-models
-Version: 1.31.6
+Version: 1.31.8
 Summary: lexv2-models data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-lexv2-models-1.31.6/botocore/data/lexv2-models/2020-08-07/endpoint-rule-set-1.json` & `botocore-a-la-carte-lexv2-models-1.31.8/botocore/data/lexv2-models/2020-08-07/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lexv2-models-1.31.6/botocore/data/lexv2-models/2020-08-07/service-2.json` & `botocore-a-la-carte-lexv2-models-1.31.8/botocore/data/lexv2-models/2020-08-07/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995966666213176%*

 * *Differences: {"'operations'": "{'ListIntentStageMetrics': {'documentation': '<p>Retrieves summary metrics for "*

 * *                 'the stages within intents in your bot. The following fields are required:</p> '*

 * *                 '<ul> <li> <p> <code>metrics</code> – A list of <a '*

 * *                 'href="https://docs.aws.amazon.com/lexv2/latest/APIReference/API_AnalyticsIntentStageMetric.html">AnalyticsIntentStageMetric</a> '*

 * *                 'objects. In each object, use the <code>name</code> field to specify the metric  […]*

```diff
@@ -1922,15 +1922,15 @@
             },
             "name": "ListIntentPaths",
             "output": {
                 "shape": "ListIntentPathsResponse"
             }
         },
         "ListIntentStageMetrics": {
-            "documentation": "<p>Retrieves summary metrics for the intent stages in your bot. The following fields are required:</p> <ul> <li> <p> <code>metrics</code> \u2013 A list of <a href=\"https://docs.aws.amazon.com/lexv2/latest/APIReference/API_AnalyticsIntentStageMetric.html\">AnalyticsIntentStageMetric</a> objects. In each object, use the <code>name</code> field to specify the metric to calculate, the <code>statistic</code> field to specify whether to calculate the <code>Sum</code>, <code>Average</code>, or <code>Max</code> number, and the <code>order</code> field to specify whether to sort the results in <code>Ascending</code> or <code>Descending</code> order.</p> </li> <li> <p> <code>startDateTime</code> and <code>endDateTime</code> \u2013 Define a time range for which you want to retrieve results.</p> </li> </ul> <p>Of the optional fields, you can organize the results in the following ways:</p> <ul> <li> <p>Use the <code>filters</code> field to filter the results, the <code>groupBy</code> field to specify categories by which to group the results, and the <code>binBy</code> field to specify time intervals by which to group the results.</p> </li> <li> <p>Use the <code>maxResults</code> field to limit the number of results to return in a single response and the <code>nextToken</code> field to return the next batch of results if the response does not return the full set of results.</p> </li> </ul> <p>Note that an <code>order</code> field exists in both <code>binBy</code> and <code>metrics</code>. You can only specify one <code>order</code> in a given request.</p>",
+            "documentation": "<p>Retrieves summary metrics for the stages within intents in your bot. The following fields are required:</p> <ul> <li> <p> <code>metrics</code> \u2013 A list of <a href=\"https://docs.aws.amazon.com/lexv2/latest/APIReference/API_AnalyticsIntentStageMetric.html\">AnalyticsIntentStageMetric</a> objects. In each object, use the <code>name</code> field to specify the metric to calculate, the <code>statistic</code> field to specify whether to calculate the <code>Sum</code>, <code>Average</code>, or <code>Max</code> number, and the <code>order</code> field to specify whether to sort the results in <code>Ascending</code> or <code>Descending</code> order.</p> </li> <li> <p> <code>startDateTime</code> and <code>endDateTime</code> \u2013 Define a time range for which you want to retrieve results.</p> </li> </ul> <p>Of the optional fields, you can organize the results in the following ways:</p> <ul> <li> <p>Use the <code>filters</code> field to filter the results, the <code>groupBy</code> field to specify categories by which to group the results, and the <code>binBy</code> field to specify time intervals by which to group the results.</p> </li> <li> <p>Use the <code>maxResults</code> field to limit the number of results to return in a single response and the <code>nextToken</code> field to return the next batch of results if the response does not return the full set of results.</p> </li> </ul> <p>Note that an <code>order</code> field exists in both <code>binBy</code> and <code>metrics</code>. You can only specify one <code>order</code> in a given request.</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -2288,15 +2288,15 @@
             },
             "name": "ListTestSets",
             "output": {
                 "shape": "ListTestSetsResponse"
             }
         },
         "ListUtteranceAnalyticsData": {
-            "documentation": "<p>Retrieves a list of metadata for individual user utterances to your bot. The <code>startDateTime</code> and <code>endDateTime</code> fields are required. These fields define a time range for which you want to retrieve results. Of the optional fields, you can organize the results in the following ways:</p> <ul> <li> <p>Use the <code>filters</code> field to filter the results and the <code>sortBy</code> field to specify the values by which to sort the results.</p> </li> <li> <p>Use the <code>maxResults</code> field to limit the number of results to return in a single response and the <code>nextToken</code> field to return the next batch of results if the response does not return the full set of results.</p> </li> </ul>",
+            "documentation": "<note> <p>To use this API operation, your IAM role must have permissions to perform the <a href=\"https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListAggregatedUtterances.html\">ListAggregatedUtterances</a> operation, which provides access to utterance-related analytics. See <a href=\"https://docs.aws.amazon.com/lexv2/latest/dg/monitoring-utterances.html\">Viewing utterance statistics</a> for the IAM policy to apply to the IAM role.</p> </note> <p>Retrieves a list of metadata for individual user utterances to your bot. The following fields are required:</p> <ul> <li> <p> <code>startDateTime</code> and <code>endDateTime</code> \u2013 Define a time range for which you want to retrieve results.</p> </li> </ul> <p>Of the optional fields, you can organize the results in the following ways:</p> <ul> <li> <p>Use the <code>filters</code> field to filter the results and the <code>sortBy</code> field to specify the values by which to sort the results.</p> </li> <li> <p>Use the <code>maxResults</code> field to limit the number of results to return in a single response and the <code>nextToken</code> field to return the next batch of results if the response does not return the full set of results.</p> </li> </ul>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -2320,15 +2320,15 @@
             },
             "name": "ListUtteranceAnalyticsData",
             "output": {
                 "shape": "ListUtteranceAnalyticsDataResponse"
             }
         },
         "ListUtteranceMetrics": {
-            "documentation": "<p>Retrieves summary metrics for the utterances in your bot. The following fields are required:</p> <ul> <li> <p> <code>metrics</code> \u2013 A list of <a href=\"https://docs.aws.amazon.com/lexv2/latest/APIReference/API_AnalyticsUtteranceMetric.html\">AnalyticsUtteranceMetric</a> objects. In each object, use the <code>name</code> field to specify the metric to calculate, the <code>statistic</code> field to specify whether to calculate the <code>Sum</code>, <code>Average</code>, or <code>Max</code> number, and the <code>order</code> field to specify whether to sort the results in <code>Ascending</code> or <code>Descending</code> order.</p> </li> <li> <p> <code>startDateTime</code> and <code>endDateTime</code> \u2013 Define a time range for which you want to retrieve results.</p> </li> </ul> <p>Of the optional fields, you can organize the results in the following ways:</p> <ul> <li> <p>Use the <code>filters</code> field to filter the results, the <code>groupBy</code> field to specify categories by which to group the results, and the <code>binBy</code> field to specify time intervals by which to group the results.</p> </li> <li> <p>Use the <code>maxResults</code> field to limit the number of results to return in a single response and the <code>nextToken</code> field to return the next batch of results if the response does not return the full set of results.</p> </li> </ul> <p>Note that an <code>order</code> field exists in both <code>binBy</code> and <code>metrics</code>. Currently, you can specify it in either field, but not in both.</p>",
+            "documentation": "<note> <p>To use this API operation, your IAM role must have permissions to perform the <a href=\"https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListAggregatedUtterances.html\">ListAggregatedUtterances</a> operation, which provides access to utterance-related analytics. See <a href=\"https://docs.aws.amazon.com/lexv2/latest/dg/monitoring-utterances.html\">Viewing utterance statistics</a> for the IAM policy to apply to the IAM role.</p> </note> <p>Retrieves summary metrics for the utterances in your bot. The following fields are required:</p> <ul> <li> <p> <code>metrics</code> \u2013 A list of <a href=\"https://docs.aws.amazon.com/lexv2/latest/APIReference/API_AnalyticsUtteranceMetric.html\">AnalyticsUtteranceMetric</a> objects. In each object, use the <code>name</code> field to specify the metric to calculate, the <code>statistic</code> field to specify whether to calculate the <code>Sum</code>, <code>Average</code>, or <code>Max</code> number, and the <code>order</code> field to specify whether to sort the results in <code>Ascending</code> or <code>Descending</code> order.</p> </li> <li> <p> <code>startDateTime</code> and <code>endDateTime</code> \u2013 Define a time range for which you want to retrieve results.</p> </li> </ul> <p>Of the optional fields, you can organize the results in the following ways:</p> <ul> <li> <p>Use the <code>filters</code> field to filter the results, the <code>groupBy</code> field to specify categories by which to group the results, and the <code>binBy</code> field to specify time intervals by which to group the results.</p> </li> <li> <p>Use the <code>maxResults</code> field to limit the number of results to return in a single response and the <code>nextToken</code> field to return the next batch of results if the response does not return the full set of results.</p> </li> </ul> <p>Note that an <code>order</code> field exists in both <code>binBy</code> and <code>metrics</code>. Currently, you can specify it in either field, but not in both.</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -3256,14 +3256,19 @@
             },
             "min": 1,
             "type": "list"
         },
         "AnalyticsBinValue": {
             "type": "long"
         },
+        "AnalyticsChannel": {
+            "max": 50,
+            "min": 1,
+            "type": "string"
+        },
         "AnalyticsCommonFilterName": {
             "enum": [
                 "BotAliasId",
                 "BotVersion",
                 "LocaleId",
                 "Modality",
                 "Channel"
@@ -4143,15 +4148,15 @@
             ],
             "type": "string"
         },
         "AnalyticsUtteranceMetricResult": {
             "documentation": "<p>An object containing the results for the utterance metric you requested.</p>",
             "members": {
                 "name": {
-                    "documentation": "<p>The metric that you requested.</p> <ul> <li> <p> <code>Count</code> \u2013 The number of utterances.</p> </li> <li> <p> <code>Missed</code> \u2013 The number of utterances that Amazon Lex failed to recognize.</p> </li> <li> <p> <code>Detected</code> \u2013 The number of utterances that Amazon Lex managed to detect.</p> </li> <li> <p> <code>UtteranceTimeStamp</code> \u2013 The date and time of the utterance.</p> </li> </ul>",
+                    "documentation": "<p>The metric that you requested.</p> <ul> <li> <p> <code>Count</code> \u2013 The number of utterances.</p> </li> <li> <p> <code>Missed</code> \u2013 The number of utterances that Amazon Lex failed to recognize.</p> </li> <li> <p> <code>Detected</code> \u2013 The number of utterances that Amazon Lex managed to detect.</p> </li> <li> <p> <code>UtteranceTimestamp</code> \u2013 The date and time of the utterance.</p> </li> </ul>",
                     "shape": "AnalyticsUtteranceMetricName"
                 },
                 "statistic": {
                     "documentation": "<p>The summary statistic that you requested to calculate.</p> <ul> <li> <p> <code>Sum</code> \u2013 The total count for the category you provide in <code>name</code>.</p> </li> <li> <p> <code>Average</code> \u2013 The total count divided by the number of utterances in the category you provide in <code>name</code>.</p> </li> <li> <p> <code>Max</code> \u2013 The highest count in the category you provide in <code>name</code>.</p> </li> </ul>",
                     "shape": "AnalyticsMetricStatistic"
                 },
                 "value": {
@@ -4665,22 +4670,14 @@
             "required": [
                 "botId",
                 "botAliasId",
                 "localeId"
             ],
             "type": "structure"
         },
-        "BotChannelType": {
-            "enum": [
-                "Facebook",
-                "Slack",
-                "TwilioSms"
-            ],
-            "type": "string"
-        },
         "BotExportSpecification": {
             "documentation": "<p>Provides the identity of a the bot that was exported.</p>",
             "members": {
                 "botId": {
                     "documentation": "<p>The identifier of the bot assigned by Amazon Lex.</p>",
                     "shape": "Id"
                 },
@@ -12310,15 +12307,15 @@
                 },
                 "botVersion": {
                     "documentation": "<p>The version of the bot that the session was held with.</p>",
                     "shape": "NumericalBotVersion"
                 },
                 "channel": {
                     "documentation": "<p>The channel that is integrated with the bot that the session was held with.</p>",
-                    "shape": "BotChannelType"
+                    "shape": "AnalyticsChannel"
                 },
                 "conversationDurationSeconds": {
                     "documentation": "<p>The duration of the conversation in seconds. A conversation is defined as a unique combination of a <code>sessionId</code> and an <code>originatingRequestId</code>.</p>",
                     "shape": "AnalyticsLongValue"
                 },
                 "conversationEndState": {
                     "documentation": "<p>The final state of the conversation. A conversation is defined as a unique combination of a <code>sessionId</code> and an <code>originatingRequestId</code>.</p>",
@@ -15350,15 +15347,15 @@
             ],
             "type": "string"
         },
         "UtteranceDataSortBy": {
             "documentation": "<p>An object specifying the measure and method by which to sort the utterance data.</p>",
             "members": {
                 "name": {
-                    "documentation": "<p>The measure by which to sort the utterance analytics data.</p> <ul> <li> <p> <code>Count</code> \u2013 The number of utterances.</p> </li> <li> <p> <code>UtteranceTimeStamp</code> \u2013 The date and time of the utterance.</p> </li> </ul>",
+                    "documentation": "<p>The measure by which to sort the utterance analytics data.</p> <ul> <li> <p> <code>Count</code> \u2013 The number of utterances.</p> </li> <li> <p> <code>UtteranceTimestamp</code> \u2013 The date and time of the utterance.</p> </li> </ul>",
                     "shape": "AnalyticsUtteranceSortByName"
                 },
                 "order": {
                     "documentation": "<p>Specifies whether to sort the results in ascending or descending order.</p>",
                     "shape": "AnalyticsSortOrder"
                 }
             },
@@ -15452,15 +15449,15 @@
                 },
                 "botVersion": {
                     "documentation": "<p>The version of the bot that the utterance was made to.</p>",
                     "shape": "NumericalBotVersion"
                 },
                 "channel": {
                     "documentation": "<p>The channel that is integrated with the bot that the utterance was made to.</p>",
-                    "shape": "BotChannelType"
+                    "shape": "AnalyticsChannel"
                 },
                 "conversationEndTime": {
                     "documentation": "<p>The date and time when the conversation in which the utterance took place ended. A conversation is defined as a unique combination of a <code>sessionId</code> and an <code>originatingRequestId</code>.</p>",
                     "shape": "Timestamp"
                 },
                 "conversationStartTime": {
                     "documentation": "<p>The date and time when the conversation in which the utterance took place began. A conversation is defined as a unique combination of a <code>sessionId</code> and an <code>originatingRequestId</code>.</p>",
```

### Comparing `botocore-a-la-carte-lexv2-models-1.31.6/botocore/data/lexv2-models/2020-08-07/waiters-2.json` & `botocore-a-la-carte-lexv2-models-1.31.8/botocore/data/lexv2-models/2020-08-07/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lexv2-models-1.31.6/botocore_a_la_carte_lexv2_models.egg-info/PKG-INFO` & `botocore-a-la-carte-lexv2-models-1.31.8/botocore_a_la_carte_lexv2_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-lexv2-models
-Version: 1.31.6
+Version: 1.31.8
 Summary: lexv2-models data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-lexv2-models-1.31.6/botocore_a_la_carte_lexv2_models.egg-info/SOURCES.txt` & `botocore-a-la-carte-lexv2-models-1.31.8/botocore_a_la_carte_lexv2_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lexv2-models-1.31.6/setup.py` & `botocore-a-la-carte-lexv2-models-1.31.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-lexv2-models',
-    version="1.31.6",
+    version="1.31.8",
     description='lexv2-models data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/lexv2-models/*/*.json'],
```

