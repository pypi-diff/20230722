# Comparing `tmp/botocore-a-la-carte-securitylake-1.31.6.tar.gz` & `tmp/botocore-a-la-carte-securitylake-1.31.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-securitylake-1.31.6.tar", last modified: Thu Jul 20 01:20:47 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-securitylake-1.31.8.tar", last modified: Fri Jul 21 01:21:58 2023, max compression
```

## Comparing `botocore-a-la-carte-securitylake-1.31.6.tar` & `botocore-a-la-carte-securitylake-1.31.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:47.702936 botocore-a-la-carte-securitylake-1.31.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-20 01:20:47.000000 botocore-a-la-carte-securitylake-1.31.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-20 01:20:47.702936 botocore-a-la-carte-securitylake-1.31.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:47.702936 botocore-a-la-carte-securitylake-1.31.6/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:47.702936 botocore-a-la-carte-securitylake-1.31.6/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:47.702936 botocore-a-la-carte-securitylake-1.31.6/botocore/data/securitylake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:47.702936 botocore-a-la-carte-securitylake-1.31.6/botocore/data/securitylake/2018-05-10/
--rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-07-20 01:19:55.000000 botocore-a-la-carte-securitylake-1.31.6/botocore/data/securitylake/2018-05-10/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-20 01:19:55.000000 botocore-a-la-carte-securitylake-1.31.6/botocore/data/securitylake/2018-05-10/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-20 01:19:55.000000 botocore-a-la-carte-securitylake-1.31.6/botocore/data/securitylake/2018-05-10/paginators-1.sdk-extras.json
--rw-r--r--   0 runner    (1001) docker     (123)    90044 2023-07-20 01:19:55.000000 botocore-a-la-carte-securitylake-1.31.6/botocore/data/securitylake/2018-05-10/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:47.702936 botocore-a-la-carte-securitylake-1.31.6/botocore_a_la_carte_securitylake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-20 01:20:47.000000 botocore-a-la-carte-securitylake-1.31.6/botocore_a_la_carte_securitylake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-20 01:20:47.000000 botocore-a-la-carte-securitylake-1.31.6/botocore_a_la_carte_securitylake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 01:20:47.000000 botocore-a-la-carte-securitylake-1.31.6/botocore_a_la_carte_securitylake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 01:20:47.000000 botocore-a-la-carte-securitylake-1.31.6/botocore_a_la_carte_securitylake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 01:20:47.702936 botocore-a-la-carte-securitylake-1.31.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-20 01:20:47.000000 botocore-a-la-carte-securitylake-1.31.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:58.047594 botocore-a-la-carte-securitylake-1.31.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:57.000000 botocore-a-la-carte-securitylake-1.31.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-21 01:21:58.047594 botocore-a-la-carte-securitylake-1.31.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:58.043594 botocore-a-la-carte-securitylake-1.31.8/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:58.043594 botocore-a-la-carte-securitylake-1.31.8/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:58.043594 botocore-a-la-carte-securitylake-1.31.8/botocore/data/securitylake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:58.043594 botocore-a-la-carte-securitylake-1.31.8/botocore/data/securitylake/2018-05-10/
+-rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-07-21 01:21:06.000000 botocore-a-la-carte-securitylake-1.31.8/botocore/data/securitylake/2018-05-10/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-21 01:21:06.000000 botocore-a-la-carte-securitylake-1.31.8/botocore/data/securitylake/2018-05-10/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-21 01:21:06.000000 botocore-a-la-carte-securitylake-1.31.8/botocore/data/securitylake/2018-05-10/paginators-1.sdk-extras.json
+-rw-r--r--   0 runner    (1001) docker     (123)    98594 2023-07-21 01:21:06.000000 botocore-a-la-carte-securitylake-1.31.8/botocore/data/securitylake/2018-05-10/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:58.047594 botocore-a-la-carte-securitylake-1.31.8/botocore_a_la_carte_securitylake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-21 01:21:58.000000 botocore-a-la-carte-securitylake-1.31.8/botocore_a_la_carte_securitylake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-21 01:21:58.000000 botocore-a-la-carte-securitylake-1.31.8/botocore_a_la_carte_securitylake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:58.000000 botocore-a-la-carte-securitylake-1.31.8/botocore_a_la_carte_securitylake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:58.000000 botocore-a-la-carte-securitylake-1.31.8/botocore_a_la_carte_securitylake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:58.047594 botocore-a-la-carte-securitylake-1.31.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-21 01:21:57.000000 botocore-a-la-carte-securitylake-1.31.8/setup.py
```

### Comparing `botocore-a-la-carte-securitylake-1.31.6/LICENSE.txt` & `botocore-a-la-carte-securitylake-1.31.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-securitylake-1.31.6/PKG-INFO` & `botocore-a-la-carte-securitylake-1.31.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-securitylake
-Version: 1.31.6
+Version: 1.31.8
 Summary: securitylake data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-securitylake-1.31.6/botocore/data/securitylake/2018-05-10/endpoint-rule-set-1.json` & `botocore-a-la-carte-securitylake-1.31.8/botocore/data/securitylake/2018-05-10/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-securitylake-1.31.6/botocore/data/securitylake/2018-05-10/paginators-1.json` & `botocore-a-la-carte-securitylake-1.31.8/botocore/data/securitylake/2018-05-10/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-securitylake-1.31.6/botocore/data/securitylake/2018-05-10/service-2.json` & `botocore-a-la-carte-securitylake-1.31.8/botocore/data/securitylake/2018-05-10/service-2.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9825071459118838%*

 * *Differences: {"'operations'": "{'CreateAwsLogSource': {'documentation': '<p>Adds a natively supported Amazon "*

 * *                 'Web Service as an Amazon Security Lake source. Enables source types for member '*

 * *                 'accounts in required Amazon Web Services Regions, based on the parameters you '*

 * *                 'specify. You can choose any source type in any Region for either accounts that '*

 * *                 'are part of a trusted organization or standalone accounts. Once you add an '*

 * *                 'Amazo […]*

```diff
@@ -9,15 +9,15 @@
         "serviceId": "SecurityLake",
         "signatureVersion": "v4",
         "signingName": "securitylake",
         "uid": "securitylake-2018-05-10"
     },
     "operations": {
         "CreateAwsLogSource": {
-            "documentation": "<p>Adds a natively supported Amazon Web Service as an Amazon Security Lake source. Enables source types for member accounts in required Amazon Web Services Regions, based on the parameters you specify. You can choose any source type in any Region for either accounts that are part of a trusted organization or standalone accounts. Once you add an Amazon Web Service as a source, Security Lake starts collecting logs and events from it, </p> <p>You can use this API only to enable natively supported Amazon Web Services as a source. Use <code>CreateCustomLogSource</code> to enable data collection from a custom source.</p>",
+            "documentation": "<p>Adds a natively supported Amazon Web Service as an Amazon Security Lake source. Enables source types for member accounts in required Amazon Web Services Regions, based on the parameters you specify. You can choose any source type in any Region for either accounts that are part of a trusted organization or standalone accounts. Once you add an Amazon Web Service as a source, Security Lake starts collecting logs and events from it.</p> <p>You can use this API only to enable natively supported Amazon Web Services as a source. Use <code>CreateCustomLogSource</code> to enable data collection from a custom source.</p>",
             "errors": [
                 {
                     "shape": "BadRequestException"
                 },
                 {
                     "shape": "ResourceNotFoundException"
                 },
@@ -80,15 +80,15 @@
             },
             "name": "CreateCustomLogSource",
             "output": {
                 "shape": "CreateCustomLogSourceResponse"
             }
         },
         "CreateDataLake": {
-            "documentation": "<p>Initializes an Amazon Security Lake instance with the provided (or default) configuration. You can enable Security Lake in Amazon Web Services Regions with customized settings before enabling log collection in Regions. By default, the <code>CreateDataLake</code> Security Lake in all Regions. To specify particular Regions, configure these Regions using the <code>configurations</code> parameter. If you have already enabled Security Lake in a Region when you call this command, the command will update the Region if you provide new configuration parameters. If you have not already enabled Security Lake in the Region when you call this API, it will set up the data lake in the Region with the specified configurations.</p> <p>When you enable Security Lake, it starts ingesting security data after the <code>CreateAwsLogSource</code> call. This includes ingesting security data from sources, storing data, and making data accessible to subscribers. Security Lake also enables all the existing settings and resources that it stores or maintains for your Amazon Web Services account in the current Region, including security log and event data. For more information, see the <a href=\"https://docs.aws.amazon.com/security-lake/latest/userguide/what-is-security-lake.html\">Amazon Security Lake User Guide</a>.</p>",
+            "documentation": "<p>Initializes an Amazon Security Lake instance with the provided (or default) configuration. You can enable Security Lake in Amazon Web Services Regions with customized settings before enabling log collection in Regions. To specify particular Regions, configure these Regions using the <code>configurations</code> parameter. If you have already enabled Security Lake in a Region when you call this command, the command will update the Region if you provide new configuration parameters. If you have not already enabled Security Lake in the Region when you call this API, it will set up the data lake in the Region with the specified configurations.</p> <p>When you enable Security Lake, it starts ingesting security data after the <code>CreateAwsLogSource</code> call. This includes ingesting security data from sources, storing data, and making data accessible to subscribers. Security Lake also enables all the existing settings and resources that it stores or maintains for your Amazon Web Services account in the current Region, including security log and event data. For more information, see the <a href=\"https://docs.aws.amazon.com/security-lake/latest/userguide/what-is-security-lake.html\">Amazon Security Lake User Guide</a>.</p>",
             "errors": [
                 {
                     "shape": "BadRequestException"
                 },
                 {
                     "shape": "ResourceNotFoundException"
                 },
@@ -398,15 +398,15 @@
             },
             "name": "DeleteDataLakeExceptionSubscription",
             "output": {
                 "shape": "DeleteDataLakeExceptionSubscriptionResponse"
             }
         },
         "DeleteDataLakeOrganizationConfiguration": {
-            "documentation": "<p>Removes automatic the enablement of configuration settings for new member accounts (but retains the settings for the delegated administrator) from Amazon Security Lake. You must run this API using the credentials of the delegated administrator. When you run this API, new member accounts that are added after the organization enables Security Lake won't contribute to the data lake.</p>",
+            "documentation": "<p>Turns off automatic enablement of Amazon Security Lake for member accounts that are added to an organization in Organizations. Only the delegated Security Lake administrator for an organization can perform this operation. If the delegated Security Lake administrator performs this operation, new member accounts won't automatically contribute data to the data lake.</p>",
             "errors": [
                 {
                     "shape": "BadRequestException"
                 },
                 {
                     "shape": "ResourceNotFoundException"
                 },
@@ -716,15 +716,15 @@
             },
             "name": "ListDataLakeExceptions",
             "output": {
                 "shape": "ListDataLakeExceptionsResponse"
             }
         },
         "ListDataLakes": {
-            "documentation": "<p>Retrieves the Amazon Security Lake configuration object for the specified Amazon Web Services account ID. You can use the <code>ListDataLakes</code> API to know whether Security Lake is enabled for any region.</p>",
+            "documentation": "<p>Retrieves the Amazon Security Lake configuration object for the specified Amazon Web Services Regions. You can use this operation to determine whether Security Lake is enabled for a Region.</p>",
             "errors": [
                 {
                     "shape": "BadRequestException"
                 },
                 {
                     "shape": "ResourceNotFoundException"
                 },
@@ -820,14 +820,49 @@
                 "shape": "ListSubscribersRequest"
             },
             "name": "ListSubscribers",
             "output": {
                 "shape": "ListSubscribersResponse"
             }
         },
+        "ListTagsForResource": {
+            "documentation": "<p>Retrieves the tags (keys and values) that are associated with an Amazon Security Lake resource: a subscriber, or the data lake configuration for your Amazon Web Services account in a particular Amazon Web Services Region.</p>",
+            "errors": [
+                {
+                    "shape": "BadRequestException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "InternalServerException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/v1/tags/{resourceArn}",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "ListTagsForResourceRequest"
+            },
+            "name": "ListTagsForResource",
+            "output": {
+                "shape": "ListTagsForResourceResponse"
+            }
+        },
         "RegisterDataLakeDelegatedAdministrator": {
             "documentation": "<p>Designates the Amazon Security Lake delegated administrator account for the organization. This API can only be called by the organization management account. The organization management account cannot be the delegated administrator account.</p>",
             "errors": [
                 {
                     "shape": "BadRequestException"
                 },
                 {
@@ -855,14 +890,86 @@
                 "shape": "RegisterDataLakeDelegatedAdministratorRequest"
             },
             "name": "RegisterDataLakeDelegatedAdministrator",
             "output": {
                 "shape": "RegisterDataLakeDelegatedAdministratorResponse"
             }
         },
+        "TagResource": {
+            "documentation": "<p>Adds or updates one or more tags that are associated with an Amazon Security Lake resource: a subscriber, or the data lake configuration for your Amazon Web Services account in a particular Amazon Web Services Region. A <i>tag</i> is a label that you can define and associate with Amazon Web Services resources. Each tag consists of a required <i>tag key</i> and an associated <i>tag value</i>. A <i>tag key</i> is a general label that acts as a category for a more specific tag value. A <i>tag value</i> acts as a descriptor for a tag key. Tags can help you identify, categorize, and manage resources in different ways, such as by owner, environment, or other criteria. For more information, see <a href=\"https://docs.aws.amazon.com/security-lake/latest/userguide/tagging-resources.html\">Tagging Amazon Security Lake resources</a> in the <i>Amazon Security Lake User Guide</i>.</p>",
+            "errors": [
+                {
+                    "shape": "BadRequestException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "InternalServerException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/v1/tags/{resourceArn}",
+                "responseCode": 200
+            },
+            "idempotent": true,
+            "input": {
+                "shape": "TagResourceRequest"
+            },
+            "name": "TagResource",
+            "output": {
+                "shape": "TagResourceResponse"
+            }
+        },
+        "UntagResource": {
+            "documentation": "<p>Removes one or more tags (keys and values) from an Amazon Security Lake resource: a subscriber, or the data lake configuration for your Amazon Web Services account in a particular Amazon Web Services Region.</p>",
+            "errors": [
+                {
+                    "shape": "BadRequestException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "InternalServerException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                }
+            ],
+            "http": {
+                "method": "DELETE",
+                "requestUri": "/v1/tags/{resourceArn}",
+                "responseCode": 200
+            },
+            "idempotent": true,
+            "input": {
+                "shape": "UntagResourceRequest"
+            },
+            "name": "UntagResource",
+            "output": {
+                "shape": "UntagResourceResponse"
+            }
+        },
         "UpdateDataLake": {
             "documentation": "<p>Specifies where to store your security data and for how long. You can add a rollup Region to consolidate data from multiple Amazon Web Services Regions.</p>",
             "errors": [
                 {
                     "shape": "BadRequestException"
                 },
                 {
@@ -1286,14 +1393,18 @@
                 "configurations": {
                     "documentation": "<p>Specify the Region or Regions that will contribute data to the rollup region.</p>",
                     "shape": "DataLakeConfigurationList"
                 },
                 "metaStoreManagerRoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) used to create and update the Glue table. This table contains partitions generated by the ingestion and normalization of Amazon Web Services log sources and custom sources.</p>",
                     "shape": "RoleArn"
+                },
+                "tags": {
+                    "documentation": "<p>An array of objects, one for each tag to associate with the data lake configuration. For each tag, you must specify both a tag key and a tag value. A tag value cannot be null, but it can be an empty string.</p>",
+                    "shape": "TagList"
                 }
             },
             "required": [
                 "configurations",
                 "metaStoreManagerRoleArn"
             ],
             "type": "structure"
@@ -1352,14 +1463,18 @@
                 "subscriberIdentity": {
                     "documentation": "<p>The AWS identity used to access your data.</p>",
                     "shape": "AwsIdentity"
                 },
                 "subscriberName": {
                     "documentation": "<p>The name of your Security Lake subscriber account.</p>",
                     "shape": "CreateSubscriberRequestSubscriberNameString"
+                },
+                "tags": {
+                    "documentation": "<p>An array of objects, one for each tag to associate with the subscriber. For each tag, you must specify both a tag key and a tag value. A tag value cannot be null, but it can be an empty string.</p>",
+                    "shape": "TagList"
                 }
             },
             "required": [
                 "sources",
                 "subscriberIdentity",
                 "subscriberName"
             ],
@@ -1538,15 +1653,15 @@
                     "documentation": "<p>The id of KMS encryption key used by Amazon Security Lake to encrypt the Security Lake object.</p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
         "DataLakeException": {
-            "documentation": "<p>The details for a Security Lake exception</p>",
+            "documentation": "<p>The details for an Amazon Security Lake exception.</p>",
             "members": {
                 "exception": {
                     "documentation": "<p>The underlying exception of a Security Lake exception.</p>",
                     "shape": "SafeString"
                 },
                 "region": {
                     "documentation": "<p>The Amazon Web Services Regions where the exception occurred.</p>",
@@ -1829,15 +1944,15 @@
         "DeleteDataLakeExceptionSubscriptionResponse": {
             "members": {},
             "type": "structure"
         },
         "DeleteDataLakeOrganizationConfigurationRequest": {
             "members": {
                 "autoEnableNewAccount": {
-                    "documentation": "<p>Removes the automatic enablement of configuration settings for new member accounts in Security Lake.</p>",
+                    "documentation": "<p>Turns off automatic enablement of Security Lake for member accounts that are added to an organization.</p>",
                     "shape": "DataLakeAutoEnableNewAccountConfigurationList"
                 }
             },
             "required": [
                 "autoEnableNewAccount"
             ],
             "type": "structure"
@@ -2030,15 +2145,15 @@
                     "shape": "HttpsNotificationConfigurationEndpointString"
                 },
                 "httpMethod": {
                     "documentation": "<p>The HTTPS method used for the notification subscription.</p>",
                     "shape": "HttpMethod"
                 },
                 "targetRoleArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the EventBridge API destinations IAM role that you created. For more information about ARNs and how to use them in policies, see <a href=\"https://docs.aws.amazon.com//security-lake/latest/userguide/subscriber-data-access.html\">Managing data access</a> and <a href=\"https://docs.aws.amazon.com/security-lake/latest/userguide/security-iam-awsmanpol.html\">Amazon Web Services Managed Policies</a> in the Amazon Security Lake User Guide.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the EventBridge API destinations IAM role that you created. For more information about ARNs and how to use them in policies, see <a href=\"https://docs.aws.amazon.com//security-lake/latest/userguide/subscriber-data-access.html\">Managing data access</a> and <a href=\"https://docs.aws.amazon.com/security-lake/latest/userguide/security-iam-awsmanpol.html\">Amazon Web Services Managed Policies</a> in the <i>Amazon Security Lake User Guide</i>.</p>",
                     "shape": "RoleArn"
                 }
             },
             "required": [
                 "endpoint",
                 "targetRoleArn"
             ],
@@ -2183,14 +2298,37 @@
                 "subscribers": {
                     "documentation": "<p>The subscribers available for the specified Security Lake account ID.</p>",
                     "shape": "SubscriberResourceList"
                 }
             },
             "type": "structure"
         },
+        "ListTagsForResourceRequest": {
+            "members": {
+                "resourceArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the Amazon Security Lake resource to retrieve the tags for.</p>",
+                    "location": "uri",
+                    "locationName": "resourceArn",
+                    "shape": "AmazonResourceName"
+                }
+            },
+            "required": [
+                "resourceArn"
+            ],
+            "type": "structure"
+        },
+        "ListTagsForResourceResponse": {
+            "members": {
+                "tags": {
+                    "documentation": "<p>An array of objects, one for each tag (key and value) that\u2019s associated with the Amazon Security Lake resource.</p>",
+                    "shape": "TagList"
+                }
+            },
+            "type": "structure"
+        },
         "LogSource": {
             "documentation": "<p>Amazon Security Lake can collect logs and events from natively-supported Amazon Web Services services and custom sources. </p>",
             "members": {
                 "account": {
                     "documentation": "<p>Specify the account from which you want to collect logs.</p>",
                     "shape": "AwsAccountId"
                 },
@@ -2208,22 +2346,22 @@
         "LogSourceList": {
             "member": {
                 "shape": "LogSource"
             },
             "type": "list"
         },
         "LogSourceResource": {
-            "documentation": "<p>The supported source types from which logs and events are collected in Amazon Security Lake. For the list of supported Amazon Web Services, see the <a href=\"https://docs.aws.amazon.com/security-lake/latest/userguide/internal-sources.html\">Amazon Security Lake User Guide</a>.</p>",
+            "documentation": "<p>The supported source types from which logs and events are collected in Amazon Security Lake. For a list of supported Amazon Web Services, see the <a href=\"https://docs.aws.amazon.com/security-lake/latest/userguide/internal-sources.html\">Amazon Security Lake User Guide</a>.</p>",
             "members": {
                 "awsLogSource": {
-                    "documentation": "<p>Amazon Security Lake supports log and event collection for natively supported Amazon Web Services.</p>",
+                    "documentation": "<p>Amazon Security Lake supports log and event collection for natively supported Amazon Web Services. For more information, see the <a href=\"https://docs.aws.amazon.com/security-lake/latest/userguide/internal-sources.html\">Amazon Security Lake User Guide</a>.</p>",
                     "shape": "AwsLogSourceResource"
                 },
                 "customLogSource": {
-                    "documentation": "<p>Amazon Security Lake supports custom source types. For a detailed list, see the Amazon Security Lake User Guide.</p>",
+                    "documentation": "<p>Amazon Security Lake supports custom source types. For more information, see the <a href=\"https://docs.aws.amazon.com/security-lake/latest/userguide/custom-sources.html\">Amazon Security Lake User Guide</a>.</p>",
                     "shape": "CustomLogSourceResource"
                 }
             },
             "type": "structure",
             "union": true
         },
         "LogSourceResourceList": {
@@ -2384,15 +2522,15 @@
                     "shape": "RoleArn"
                 },
                 "s3BucketArn": {
                     "documentation": "<p>The ARN for the Amazon S3 bucket.</p>",
                     "shape": "S3BucketArn"
                 },
                 "sources": {
-                    "documentation": "<p>Amazon Security Lake supports log and event collection for natively supported Amazon Web Services. For more information, see the Amazon Security Lake User Guide.</p>",
+                    "documentation": "<p>Amazon Security Lake supports log and event collection for natively supported Amazon Web Services. For more information, see the <a href=\"https://docs.aws.amazon.com/security-lake/latest/userguide/source-management.html\">Amazon Security Lake User Guide</a>.</p>",
                     "shape": "LogSourceResourceList"
                 },
                 "subscriberArn": {
                     "documentation": "<p>The subscriber ARN of the Amazon Security Lake subscriber account.</p>",
                     "shape": "AmazonResourceName"
                 },
                 "subscriberDescription": {
@@ -2452,14 +2590,81 @@
             "pattern": "^[a-z\\-]*$",
             "type": "string"
         },
         "SyntheticTimestamp_date_time": {
             "timestampFormat": "iso8601",
             "type": "timestamp"
         },
+        "Tag": {
+            "documentation": "<p>A <i>tag</i> is a label that you can define and associate with Amazon Web Services resources, including certain types of Amazon Security Lake resources. Tags can help you identify, categorize, and manage resources in different ways, such as by owner, environment, or other criteria. You can associate tags with the following types of Security Lake resources: subscribers, and the data lake configuration for your Amazon Web Services account in individual Amazon Web Services Regions.</p> <p>A resource can have up to 50 tags. Each tag consists of a required <i>tag key</i> and an associated <i>tag value</i>. A <i>tag key</i> is a general label that acts as a category for a more specific tag value. Each tag key must be unique and it can have only one tag value. A <i>tag value</i> acts as a descriptor for a tag key. Tag keys and values are case sensitive. They can contain letters, numbers, spaces, or the following symbols: _ . : / = + @ -</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/security-lake/latest/userguide/tagging-resources.html\">Tagging Amazon Security Lake resources</a> in the <i>Amazon Security Lake User Guide</i>.</p>",
+            "members": {
+                "key": {
+                    "documentation": "<p>The name of the tag. This is a general label that acts as a category for a more specific tag value (<code>value</code>).</p>",
+                    "shape": "TagKey"
+                },
+                "value": {
+                    "documentation": "<p>The value that\u2019s associated with the specified tag key (<code>key</code>). This value acts as a descriptor for the tag key. A tag value cannot be null, but it can be an empty string.</p>",
+                    "shape": "TagValue"
+                }
+            },
+            "required": [
+                "key",
+                "value"
+            ],
+            "type": "structure"
+        },
+        "TagKey": {
+            "max": 128,
+            "min": 1,
+            "type": "string"
+        },
+        "TagKeyList": {
+            "max": 50,
+            "member": {
+                "shape": "TagKey"
+            },
+            "min": 0,
+            "type": "list"
+        },
+        "TagList": {
+            "max": 50,
+            "member": {
+                "shape": "Tag"
+            },
+            "min": 0,
+            "type": "list"
+        },
+        "TagResourceRequest": {
+            "members": {
+                "resourceArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the Amazon Security Lake resource to add or update the tags for.</p>",
+                    "location": "uri",
+                    "locationName": "resourceArn",
+                    "shape": "AmazonResourceName"
+                },
+                "tags": {
+                    "documentation": "<p>An array of objects, one for each tag (key and value) to associate with the Amazon Security Lake resource. For each tag, you must specify both a tag key and a tag value. A tag value cannot be null, but it can be an empty string.</p>",
+                    "shape": "TagList"
+                }
+            },
+            "required": [
+                "resourceArn",
+                "tags"
+            ],
+            "type": "structure"
+        },
+        "TagResourceResponse": {
+            "members": {},
+            "type": "structure"
+        },
+        "TagValue": {
+            "max": 256,
+            "min": 0,
+            "type": "string"
+        },
         "ThrottlingException": {
             "documentation": "<p>The limit on the number of requests per second was exceeded.</p>",
             "error": {
                 "httpStatusCode": 429,
                 "senderFault": true
             },
             "exception": true,
@@ -2487,14 +2692,39 @@
             },
             "type": "structure"
         },
         "UUID": {
             "pattern": "^[a-f0-9]{8}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{12}$",
             "type": "string"
         },
+        "UntagResourceRequest": {
+            "members": {
+                "resourceArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the Amazon Security Lake resource to remove one or more tags from.</p>",
+                    "location": "uri",
+                    "locationName": "resourceArn",
+                    "shape": "AmazonResourceName"
+                },
+                "tagKeys": {
+                    "documentation": "<p>A list of one or more tag keys. For each value in the list, specify the tag key for a tag to remove from the Amazon Security Lake resource.</p>",
+                    "location": "querystring",
+                    "locationName": "tagKeys",
+                    "shape": "TagKeyList"
+                }
+            },
+            "required": [
+                "resourceArn",
+                "tagKeys"
+            ],
+            "type": "structure"
+        },
+        "UntagResourceResponse": {
+            "members": {},
+            "type": "structure"
+        },
         "UpdateDataLakeExceptionSubscriptionRequest": {
             "members": {
                 "exceptionTimeToLive": {
                     "documentation": "<p>The time-to-live (TTL) for the exception message to remain.</p>",
                     "shape": "UpdateDataLakeExceptionSubscriptionRequestExceptionTimeToLiveLong"
                 },
                 "notificationEndpoint": {
```

### Comparing `botocore-a-la-carte-securitylake-1.31.6/botocore_a_la_carte_securitylake.egg-info/PKG-INFO` & `botocore-a-la-carte-securitylake-1.31.8/botocore_a_la_carte_securitylake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-securitylake
-Version: 1.31.6
+Version: 1.31.8
 Summary: securitylake data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-securitylake-1.31.6/setup.py` & `botocore-a-la-carte-securitylake-1.31.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-securitylake',
-    version="1.31.6",
+    version="1.31.8",
     description='securitylake data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/securitylake/*/*.json'],
```

