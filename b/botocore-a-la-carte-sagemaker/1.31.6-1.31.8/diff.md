# Comparing `tmp/botocore-a-la-carte-sagemaker-1.31.6.tar.gz` & `tmp/botocore-a-la-carte-sagemaker-1.31.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-sagemaker-1.31.6.tar", last modified: Thu Jul 20 01:20:44 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-sagemaker-1.31.8.tar", last modified: Fri Jul 21 01:21:54 2023, max compression
```

## Comparing `botocore-a-la-carte-sagemaker-1.31.6.tar` & `botocore-a-la-carte-sagemaker-1.31.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:44.110907 botocore-a-la-carte-sagemaker-1.31.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-20 01:20:43.000000 botocore-a-la-carte-sagemaker-1.31.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-20 01:20:44.110907 botocore-a-la-carte-sagemaker-1.31.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:44.110907 botocore-a-la-carte-sagemaker-1.31.6/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:44.110907 botocore-a-la-carte-sagemaker-1.31.6/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:44.110907 botocore-a-la-carte-sagemaker-1.31.6/botocore/data/sagemaker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:44.110907 botocore-a-la-carte-sagemaker-1.31.6/botocore/data/sagemaker/2017-07-24/
--rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-07-20 01:19:55.000000 botocore-a-la-carte-sagemaker-1.31.6/botocore/data/sagemaker/2017-07-24/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 01:19:55.000000 botocore-a-la-carte-sagemaker-1.31.6/botocore/data/sagemaker/2017-07-24/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-07-20 01:19:55.000000 botocore-a-la-carte-sagemaker-1.31.6/botocore/data/sagemaker/2017-07-24/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)  1668206 2023-07-20 01:19:55.000000 botocore-a-la-carte-sagemaker-1.31.6/botocore/data/sagemaker/2017-07-24/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-07-20 01:19:55.000000 botocore-a-la-carte-sagemaker-1.31.6/botocore/data/sagemaker/2017-07-24/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:44.110907 botocore-a-la-carte-sagemaker-1.31.6/botocore_a_la_carte_sagemaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-20 01:20:44.000000 botocore-a-la-carte-sagemaker-1.31.6/botocore_a_la_carte_sagemaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-20 01:20:44.000000 botocore-a-la-carte-sagemaker-1.31.6/botocore_a_la_carte_sagemaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 01:20:44.000000 botocore-a-la-carte-sagemaker-1.31.6/botocore_a_la_carte_sagemaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 01:20:44.000000 botocore-a-la-carte-sagemaker-1.31.6/botocore_a_la_carte_sagemaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 01:20:44.110907 botocore-a-la-carte-sagemaker-1.31.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-20 01:20:43.000000 botocore-a-la-carte-sagemaker-1.31.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:54.299531 botocore-a-la-carte-sagemaker-1.31.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:54.000000 botocore-a-la-carte-sagemaker-1.31.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-21 01:21:54.299531 botocore-a-la-carte-sagemaker-1.31.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:54.295531 botocore-a-la-carte-sagemaker-1.31.8/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:54.295531 botocore-a-la-carte-sagemaker-1.31.8/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:54.295531 botocore-a-la-carte-sagemaker-1.31.8/botocore/data/sagemaker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:54.295531 botocore-a-la-carte-sagemaker-1.31.8/botocore/data/sagemaker/2017-07-24/
+-rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-07-21 01:21:06.000000 botocore-a-la-carte-sagemaker-1.31.8/botocore/data/sagemaker/2017-07-24/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 01:21:06.000000 botocore-a-la-carte-sagemaker-1.31.8/botocore/data/sagemaker/2017-07-24/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-07-21 01:21:06.000000 botocore-a-la-carte-sagemaker-1.31.8/botocore/data/sagemaker/2017-07-24/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1674704 2023-07-21 01:21:06.000000 botocore-a-la-carte-sagemaker-1.31.8/botocore/data/sagemaker/2017-07-24/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-07-21 01:21:06.000000 botocore-a-la-carte-sagemaker-1.31.8/botocore/data/sagemaker/2017-07-24/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:54.299531 botocore-a-la-carte-sagemaker-1.31.8/botocore_a_la_carte_sagemaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-21 01:21:54.000000 botocore-a-la-carte-sagemaker-1.31.8/botocore_a_la_carte_sagemaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-21 01:21:54.000000 botocore-a-la-carte-sagemaker-1.31.8/botocore_a_la_carte_sagemaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:54.000000 botocore-a-la-carte-sagemaker-1.31.8/botocore_a_la_carte_sagemaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:54.000000 botocore-a-la-carte-sagemaker-1.31.8/botocore_a_la_carte_sagemaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:54.299531 botocore-a-la-carte-sagemaker-1.31.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-21 01:21:54.000000 botocore-a-la-carte-sagemaker-1.31.8/setup.py
```

### Comparing `botocore-a-la-carte-sagemaker-1.31.6/LICENSE.txt` & `botocore-a-la-carte-sagemaker-1.31.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sagemaker-1.31.6/PKG-INFO` & `botocore-a-la-carte-sagemaker-1.31.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-sagemaker
-Version: 1.31.6
+Version: 1.31.8
 Summary: sagemaker data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-sagemaker-1.31.6/botocore/data/sagemaker/2017-07-24/endpoint-rule-set-1.json` & `botocore-a-la-carte-sagemaker-1.31.8/botocore/data/sagemaker/2017-07-24/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sagemaker-1.31.6/botocore/data/sagemaker/2017-07-24/paginators-1.json` & `botocore-a-la-carte-sagemaker-1.31.8/botocore/data/sagemaker/2017-07-24/paginators-1.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9927536231884058%*

 * *Differences: {"'pagination'": "{'ListResourceCatalogs': OrderedDict([('input_token', 'NextToken'), "*

 * *                 "('output_token', 'NextToken'), ('limit_key', 'MaxResults'), ('result_key', "*

 * *                 "'ResourceCatalogs')])}"}*

```diff
@@ -320,14 +320,20 @@
         },
         "ListProcessingJobs": {
             "input_token": "NextToken",
             "limit_key": "MaxResults",
             "output_token": "NextToken",
             "result_key": "ProcessingJobSummaries"
         },
+        "ListResourceCatalogs": {
+            "input_token": "NextToken",
+            "limit_key": "MaxResults",
+            "output_token": "NextToken",
+            "result_key": "ResourceCatalogs"
+        },
         "ListSpaces": {
             "input_token": "NextToken",
             "limit_key": "MaxResults",
             "output_token": "NextToken",
             "result_key": "Spaces"
         },
         "ListStageDevices": {
```

### Comparing `botocore-a-la-carte-sagemaker-1.31.6/botocore/data/sagemaker/2017-07-24/service-2.json` & `botocore-a-la-carte-sagemaker-1.31.8/botocore/data/sagemaker/2017-07-24/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991154975491986%*

 * *Differences: {"'operations'": "{'UpdateFeatureGroup': {'documentation': '<p>Updates the feature group by either "*

 * *                 'adding features or updating the online store configuration. Use one of the '*

 * *                 'following request parameters at a time while using the '*

 * *                 '<code>UpdateFeatureGroup</code> API.</p> <p>You can add features for your '*

 * *                 'feature group using the <code>FeatureAdditions</code> request parameter. '*

 * *                 'Features cannot be removed from a fe […]*

```diff
@@ -4036,14 +4036,28 @@
                 "shape": "ListProjectsInput"
             },
             "name": "ListProjects",
             "output": {
                 "shape": "ListProjectsOutput"
             }
         },
+        "ListResourceCatalogs": {
+            "documentation": "<p> Lists Amazon SageMaker Catalogs based on given filters and orders. The maximum number of <code>ResourceCatalog</code>s viewable is 1000. </p>",
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "ListResourceCatalogsRequest"
+            },
+            "name": "ListResourceCatalogs",
+            "output": {
+                "shape": "ListResourceCatalogsResponse"
+            }
+        },
         "ListSpaces": {
             "documentation": "<p>Lists spaces.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -4906,15 +4920,15 @@
             },
             "name": "UpdateExperiment",
             "output": {
                 "shape": "UpdateExperimentResponse"
             }
         },
         "UpdateFeatureGroup": {
-            "documentation": "<p>Updates the feature group.</p>",
+            "documentation": "<p>Updates the feature group by either adding features or updating the online store configuration. Use one of the following request parameters at a time while using the <code>UpdateFeatureGroup</code> API.</p> <p>You can add features for your feature group using the <code>FeatureAdditions</code> request parameter. Features cannot be removed from a feature group.</p> <p>You can update the online store configuration by using the <code>OnlineStoreConfig</code> request parameter. If a <code>TtlDuration</code> is specified, the default <code>TtlDuration</code> applies for all records added to the feature group <i>after the feature group is updated</i>. If a record level <code>TtlDuration</code> exists from using the <code>PutRecord</code> API, the record level <code>TtlDuration</code> applies to that record instead of the default <code>TtlDuration</code>.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -11560,14 +11574,21 @@
                 }
             },
             "type": "structure"
         },
         "CreationTime": {
             "type": "timestamp"
         },
+        "CrossAccountFilterOption": {
+            "enum": [
+                "SameAccount",
+                "CrossAccount"
+            ],
+            "type": "string"
+        },
         "CsvContentType": {
             "max": 256,
             "min": 1,
             "pattern": "^[a-zA-Z0-9](-*[a-zA-Z0-9])*\\/[a-zA-Z0-9](-*[a-zA-Z0-9.])*",
             "type": "string"
         },
         "CsvContentTypes": {
@@ -14287,16 +14308,16 @@
                 }
             },
             "type": "structure"
         },
         "DescribeFeatureGroupRequest": {
             "members": {
                 "FeatureGroupName": {
-                    "documentation": "<p>The name of the <code>FeatureGroup</code> you want described. </p>",
-                    "shape": "FeatureGroupName"
+                    "documentation": "<p>The name or Amazon Resource Name (ARN) of the <code>FeatureGroup</code> you want described. </p>",
+                    "shape": "FeatureGroupNameOrArn"
                 },
                 "NextToken": {
                     "documentation": "<p>A token to resume pagination of the list of <code>Features</code> (<code>FeatureDefinitions</code>). 2,500 <code>Features</code> are returned by default.</p>",
                     "shape": "NextToken"
                 }
             },
             "required": [
@@ -14385,16 +14406,16 @@
                 "NextToken"
             ],
             "type": "structure"
         },
         "DescribeFeatureMetadataRequest": {
             "members": {
                 "FeatureGroupName": {
-                    "documentation": "<p>The name of the feature group containing the feature.</p>",
-                    "shape": "FeatureGroupName"
+                    "documentation": "<p>The name or Amazon Resource Name (ARN) of the feature group containing the feature.</p>",
+                    "shape": "FeatureGroupNameOrArn"
                 },
                 "FeatureName": {
                     "documentation": "<p>The name of the feature.</p>",
                     "shape": "FeatureName"
                 }
             },
             "required": [
@@ -18903,14 +18924,20 @@
             "type": "string"
         },
         "FeatureGroupNameContains": {
             "max": 64,
             "min": 1,
             "type": "string"
         },
+        "FeatureGroupNameOrArn": {
+            "max": 256,
+            "min": 1,
+            "pattern": "(arn:aws[a-z\\-]*:sagemaker:[a-z0-9\\-]*:[0-9]{12}:feature-group\\/)?([a-zA-Z0-9]([_-]*[a-zA-Z0-9]){0,63})",
+            "type": "string"
+        },
         "FeatureGroupSortBy": {
             "enum": [
                 "Name",
                 "FeatureGroupStatus",
                 "OfflineStoreStatus",
                 "CreationTime"
             ],
@@ -18936,15 +18963,15 @@
         "FeatureGroupSummaries": {
             "member": {
                 "shape": "FeatureGroupSummary"
             },
             "type": "list"
         },
         "FeatureGroupSummary": {
-            "documentation": "<p>The name, Arn, <code>CreationTime</code>, <code>FeatureGroup</code> values, <code>LastUpdatedTime</code> and <code>EnableOnlineStorage</code> status of a <code>FeatureGroup</code>.</p>",
+            "documentation": "<p>The name, ARN, <code>CreationTime</code>, <code>FeatureGroup</code> values, <code>LastUpdatedTime</code> and <code>EnableOnlineStorage</code> status of a <code>FeatureGroup</code>.</p>",
             "members": {
                 "CreationTime": {
                     "documentation": "<p>A timestamp indicating the time of creation time of the <code>FeatureGroup</code>.</p>",
                     "shape": "Timestamp"
                 },
                 "FeatureGroupArn": {
                     "documentation": "<p>Unique identifier for the <code>FeatureGroup</code>.</p>",
@@ -25578,14 +25605,60 @@
                 }
             },
             "required": [
                 "ProjectSummaryList"
             ],
             "type": "structure"
         },
+        "ListResourceCatalogsRequest": {
+            "members": {
+                "CreationTimeAfter": {
+                    "documentation": "<p> Use this parameter to search for <code>ResourceCatalog</code>s created after a specific date and time. </p>",
+                    "shape": "Timestamp"
+                },
+                "CreationTimeBefore": {
+                    "documentation": "<p> Use this parameter to search for <code>ResourceCatalog</code>s created before a specific date and time. </p>",
+                    "shape": "Timestamp"
+                },
+                "MaxResults": {
+                    "documentation": "<p> The maximum number of results returned by <code>ListResourceCatalogs</code>. </p>",
+                    "shape": "MaxResults"
+                },
+                "NameContains": {
+                    "documentation": "<p> A string that partially matches one or more <code>ResourceCatalog</code>s names. Filters <code>ResourceCatalog</code> by name. </p>",
+                    "shape": "ResourceCatalogName"
+                },
+                "NextToken": {
+                    "documentation": "<p> A token to resume pagination of <code>ListResourceCatalogs</code> results. </p>",
+                    "shape": "NextToken"
+                },
+                "SortBy": {
+                    "documentation": "<p> The value on which the resource catalog list is sorted. </p>",
+                    "shape": "ResourceCatalogSortBy"
+                },
+                "SortOrder": {
+                    "documentation": "<p> The order in which the resource catalogs are listed. </p>",
+                    "shape": "ResourceCatalogSortOrder"
+                }
+            },
+            "type": "structure"
+        },
+        "ListResourceCatalogsResponse": {
+            "members": {
+                "NextToken": {
+                    "documentation": "<p> A token to resume pagination of <code>ListResourceCatalogs</code> results. </p>",
+                    "shape": "NextToken"
+                },
+                "ResourceCatalogs": {
+                    "documentation": "<p> A list of the requested <code>ResourceCatalog</code>s. </p>",
+                    "shape": "ResourceCatalogList"
+                }
+            },
+            "type": "structure"
+        },
         "ListSpacesRequest": {
             "members": {
                 "DomainIdEquals": {
                     "documentation": "<p>A parameter to search for the Domain ID.</p>",
                     "shape": "DomainId"
                 },
                 "MaxResults": {
@@ -32553,14 +32626,75 @@
             "type": "structure"
         },
         "ResourceArn": {
             "max": 256,
             "pattern": "arn:aws[a-z-]*:sagemaker:[a-z0-9-]*:[0-9]{12}:.+",
             "type": "string"
         },
+        "ResourceCatalog": {
+            "documentation": "<p> A resource catalog containing all of the resources of a specific resource type within a resource owner account. For an example on sharing the Amazon SageMaker Feature Store <code>DefaultFeatureGroupCatalog</code>, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/feature-store-cross-account-discoverability-share-sagemaker-catalog.html\">Share Amazon SageMaker Catalog resource type</a> in the Amazon SageMaker Developer Guide. </p>",
+            "members": {
+                "CreationTime": {
+                    "documentation": "<p> The time the <code>ResourceCatalog</code> was created. </p>",
+                    "shape": "Timestamp"
+                },
+                "Description": {
+                    "documentation": "<p> A free form description of the <code>ResourceCatalog</code>. </p>",
+                    "shape": "ResourceCatalogDescription"
+                },
+                "ResourceCatalogArn": {
+                    "documentation": "<p> The Amazon Resource Name (ARN) of the <code>ResourceCatalog</code>. </p>",
+                    "shape": "ResourceCatalogArn"
+                },
+                "ResourceCatalogName": {
+                    "documentation": "<p> The name of the <code>ResourceCatalog</code>. </p>",
+                    "shape": "ResourceCatalogName"
+                }
+            },
+            "required": [
+                "ResourceCatalogArn",
+                "ResourceCatalogName",
+                "Description",
+                "CreationTime"
+            ],
+            "type": "structure"
+        },
+        "ResourceCatalogArn": {
+            "max": 256,
+            "pattern": "arn:aws[a-z\\-]*:sagemaker:[a-z0-9\\-]*:[0-9]{12}:sagemaker-catalog/.*",
+            "type": "string"
+        },
+        "ResourceCatalogDescription": {
+            "max": 256,
+            "type": "string"
+        },
+        "ResourceCatalogList": {
+            "member": {
+                "shape": "ResourceCatalog"
+            },
+            "type": "list"
+        },
+        "ResourceCatalogName": {
+            "max": 64,
+            "min": 1,
+            "type": "string"
+        },
+        "ResourceCatalogSortBy": {
+            "enum": [
+                "CreationTime"
+            ],
+            "type": "string"
+        },
+        "ResourceCatalogSortOrder": {
+            "enum": [
+                "Ascending",
+                "Descending"
+            ],
+            "type": "string"
+        },
         "ResourceConfig": {
             "documentation": "<p>Describes the resources, including machine learning (ML) compute instances and ML storage volumes, to use for model training. </p>",
             "members": {
                 "InstanceCount": {
                     "documentation": "<p>The number of ML compute instances to use. For distributed training, provide a value greater than 1. </p>",
                     "shape": "TrainingInstanceCount"
                 },
@@ -33109,14 +33243,18 @@
                     "shape": "TrialComponent"
                 }
             },
             "type": "structure"
         },
         "SearchRequest": {
             "members": {
+                "CrossAccountFilterOption": {
+                    "documentation": "<p> A cross account filter option. When the value is <code>\"CrossAccount\"</code> the search results will only include resources made discoverable to you from other accounts. When the value is <code>\"SameAccount\"</code> or <code>null</code> the search results will only include resources from your account. Default is <code>null</code>. For more information on searching for resources made discoverable to your account, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/feature-store-cross-account-discoverability-use.html\"> Search discoverable resources</a> in the SageMaker Developer Guide. The maximum number of <code>ResourceCatalog</code>s viewable is 1000. </p>",
+                    "shape": "CrossAccountFilterOption"
+                },
                 "MaxResults": {
                     "box": true,
                     "documentation": "<p>The maximum number of results to return.</p>",
                     "shape": "MaxResults"
                 },
                 "NextToken": {
                     "documentation": "<p>If more than <code>MaxResults</code> resources match the specified <code>SearchExpression</code>, the response includes a <code>NextToken</code>. The <code>NextToken</code> can be passed to the next <code>SearchRequest</code> to continue retrieving results.</p>",
@@ -36644,16 +36782,16 @@
         "UpdateFeatureGroupRequest": {
             "members": {
                 "FeatureAdditions": {
                     "documentation": "<p>Updates the feature group. Updating a feature group is an asynchronous operation. When you get an HTTP 200 response, you've made a valid request. It takes some time after you've made a valid request for Feature Store to update the feature group.</p>",
                     "shape": "FeatureAdditions"
                 },
                 "FeatureGroupName": {
-                    "documentation": "<p>The name of the feature group that you're updating.</p>",
-                    "shape": "FeatureGroupName"
+                    "documentation": "<p>The name or Amazon Resource Name (ARN) of the feature group that you're updating.</p>",
+                    "shape": "FeatureGroupNameOrArn"
                 },
                 "OnlineStoreConfig": {
                     "documentation": "<p>Updates the feature group online store configuration.</p>",
                     "shape": "OnlineStoreConfigUpdate"
                 }
             },
             "required": [
@@ -36676,16 +36814,16 @@
         "UpdateFeatureMetadataRequest": {
             "members": {
                 "Description": {
                     "documentation": "<p>A description that you can write to better describe the feature.</p>",
                     "shape": "FeatureDescription"
                 },
                 "FeatureGroupName": {
-                    "documentation": "<p>The name of the feature group containing the feature that you're updating.</p>",
-                    "shape": "FeatureGroupName"
+                    "documentation": "<p>The name or Amazon Resource Name (ARN) of the feature group containing the feature that you're updating.</p>",
+                    "shape": "FeatureGroupNameOrArn"
                 },
                 "FeatureName": {
                     "documentation": "<p>The name of the feature that you're updating.</p>",
                     "shape": "FeatureName"
                 },
                 "ParameterAdditions": {
                     "documentation": "<p>A list of key-value pairs that you can add to better describe the feature.</p>",
```

### Comparing `botocore-a-la-carte-sagemaker-1.31.6/botocore/data/sagemaker/2017-07-24/waiters-2.json` & `botocore-a-la-carte-sagemaker-1.31.8/botocore/data/sagemaker/2017-07-24/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sagemaker-1.31.6/botocore_a_la_carte_sagemaker.egg-info/PKG-INFO` & `botocore-a-la-carte-sagemaker-1.31.8/botocore_a_la_carte_sagemaker.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-sagemaker
-Version: 1.31.6
+Version: 1.31.8
 Summary: sagemaker data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-sagemaker-1.31.6/setup.py` & `botocore-a-la-carte-sagemaker-1.31.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-sagemaker',
-    version="1.31.6",
+    version="1.31.8",
     description='sagemaker data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/sagemaker/*/*.json'],
```

