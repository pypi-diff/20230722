# Comparing `tmp/botocore-a-la-carte-route53resolver-1.31.6.tar.gz` & `tmp/botocore-a-la-carte-route53resolver-1.31.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-route53resolver-1.31.6.tar", last modified: Thu Jul 20 01:20:42 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-route53resolver-1.31.8.tar", last modified: Fri Jul 21 01:21:52 2023, max compression
```

## Comparing `botocore-a-la-carte-route53resolver-1.31.6.tar` & `botocore-a-la-carte-route53resolver-1.31.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:42.586895 botocore-a-la-carte-route53resolver-1.31.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-20 01:20:42.000000 botocore-a-la-carte-route53resolver-1.31.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-20 01:20:42.586895 botocore-a-la-carte-route53resolver-1.31.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:42.586895 botocore-a-la-carte-route53resolver-1.31.6/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:42.586895 botocore-a-la-carte-route53resolver-1.31.6/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:42.586895 botocore-a-la-carte-route53resolver-1.31.6/botocore/data/route53resolver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:42.586895 botocore-a-la-carte-route53resolver-1.31.6/botocore/data/route53resolver/2018-04-01/
--rw-r--r--   0 runner    (1001) docker     (123)    20574 2023-07-20 01:19:55.000000 botocore-a-la-carte-route53resolver-1.31.6/botocore/data/route53resolver/2018-04-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 01:19:55.000000 botocore-a-la-carte-route53resolver-1.31.6/botocore/data/route53resolver/2018-04-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-20 01:19:55.000000 botocore-a-la-carte-route53resolver-1.31.6/botocore/data/route53resolver/2018-04-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-20 01:19:55.000000 botocore-a-la-carte-route53resolver-1.31.6/botocore/data/route53resolver/2018-04-01/paginators-1.sdk-extras.json
--rw-r--r--   0 runner    (1001) docker     (123)   226948 2023-07-20 01:19:55.000000 botocore-a-la-carte-route53resolver-1.31.6/botocore/data/route53resolver/2018-04-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:42.586895 botocore-a-la-carte-route53resolver-1.31.6/botocore_a_la_carte_route53resolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-20 01:20:42.000000 botocore-a-la-carte-route53resolver-1.31.6/botocore_a_la_carte_route53resolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-20 01:20:42.000000 botocore-a-la-carte-route53resolver-1.31.6/botocore_a_la_carte_route53resolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 01:20:42.000000 botocore-a-la-carte-route53resolver-1.31.6/botocore_a_la_carte_route53resolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 01:20:42.000000 botocore-a-la-carte-route53resolver-1.31.6/botocore_a_la_carte_route53resolver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 01:20:42.590895 botocore-a-la-carte-route53resolver-1.31.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-20 01:20:42.000000 botocore-a-la-carte-route53resolver-1.31.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:52.751505 botocore-a-la-carte-route53resolver-1.31.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:52.000000 botocore-a-la-carte-route53resolver-1.31.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-21 01:21:52.751505 botocore-a-la-carte-route53resolver-1.31.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:52.747505 botocore-a-la-carte-route53resolver-1.31.8/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:52.747505 botocore-a-la-carte-route53resolver-1.31.8/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:52.747505 botocore-a-la-carte-route53resolver-1.31.8/botocore/data/route53resolver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:52.747505 botocore-a-la-carte-route53resolver-1.31.8/botocore/data/route53resolver/2018-04-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    17660 2023-07-21 01:21:06.000000 botocore-a-la-carte-route53resolver-1.31.8/botocore/data/route53resolver/2018-04-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 01:21:06.000000 botocore-a-la-carte-route53resolver-1.31.8/botocore/data/route53resolver/2018-04-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-21 01:21:06.000000 botocore-a-la-carte-route53resolver-1.31.8/botocore/data/route53resolver/2018-04-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-21 01:21:06.000000 botocore-a-la-carte-route53resolver-1.31.8/botocore/data/route53resolver/2018-04-01/paginators-1.sdk-extras.json
+-rw-r--r--   0 runner    (1001) docker     (123)   240123 2023-07-21 01:21:06.000000 botocore-a-la-carte-route53resolver-1.31.8/botocore/data/route53resolver/2018-04-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:52.751505 botocore-a-la-carte-route53resolver-1.31.8/botocore_a_la_carte_route53resolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-21 01:21:52.000000 botocore-a-la-carte-route53resolver-1.31.8/botocore_a_la_carte_route53resolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-21 01:21:52.000000 botocore-a-la-carte-route53resolver-1.31.8/botocore_a_la_carte_route53resolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:52.000000 botocore-a-la-carte-route53resolver-1.31.8/botocore_a_la_carte_route53resolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:52.000000 botocore-a-la-carte-route53resolver-1.31.8/botocore_a_la_carte_route53resolver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:52.751505 botocore-a-la-carte-route53resolver-1.31.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-21 01:21:52.000000 botocore-a-la-carte-route53resolver-1.31.8/setup.py
```

### Comparing `botocore-a-la-carte-route53resolver-1.31.6/LICENSE.txt` & `botocore-a-la-carte-route53resolver-1.31.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53resolver-1.31.6/PKG-INFO` & `botocore-a-la-carte-route53resolver-1.31.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-route53resolver
-Version: 1.31.6
+Version: 1.31.8
 Summary: route53resolver data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-route53resolver-1.31.6/botocore/data/route53resolver/2018-04-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-route53resolver-1.31.8/botocore/data/route53resolver/2018-04-01/endpoint-rule-set-1.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999255782274%*

 * *Differences: {"'rules'": "{1: {'rules': {0: {'rules': {0: {'rules': {1: {'rules': {0: {'rules': {0: {'rules': "*

 * *            '{delete: [1, 0]}}}}}}}}}}}}}'}*

```diff
@@ -232,52 +232,14 @@
                                                 }
                                             ],
                                             "rules": [
                                                 {
                                                     "conditions": [],
                                                     "rules": [
                                                         {
-                                                            "conditions": [
-                                                                {
-                                                                    "argv": [
-                                                                        {
-                                                                            "ref": "Region"
-                                                                        },
-                                                                        "us-gov-east-1"
-                                                                    ],
-                                                                    "fn": "stringEquals"
-                                                                }
-                                                            ],
-                                                            "endpoint": {
-                                                                "headers": {},
-                                                                "properties": {},
-                                                                "url": "https://route53resolver.us-gov-east-1.amazonaws.com"
-                                                            },
-                                                            "type": "endpoint"
-                                                        },
-                                                        {
-                                                            "conditions": [
-                                                                {
-                                                                    "argv": [
-                                                                        {
-                                                                            "ref": "Region"
-                                                                        },
-                                                                        "us-gov-west-1"
-                                                                    ],
-                                                                    "fn": "stringEquals"
-                                                                }
-                                                            ],
-                                                            "endpoint": {
-                                                                "headers": {},
-                                                                "properties": {},
-                                                                "url": "https://route53resolver.us-gov-west-1.amazonaws.com"
-                                                            },
-                                                            "type": "endpoint"
-                                                        },
-                                                        {
                                                             "conditions": [],
                                                             "endpoint": {
                                                                 "headers": {},
                                                                 "properties": {},
                                                                 "url": "https://route53resolver-fips.{Region}.{PartitionResult#dnsSuffix}"
                                                             },
                                                             "type": "endpoint"
```

### Comparing `botocore-a-la-carte-route53resolver-1.31.6/botocore/data/route53resolver/2018-04-01/paginators-1.json` & `botocore-a-la-carte-route53resolver-1.31.8/botocore/data/route53resolver/2018-04-01/paginators-1.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'pagination'": "{'ListOutpostResolvers': OrderedDict([('input_token', 'NextToken'), "*

 * *                 "('output_token', 'NextToken'), ('limit_key', 'MaxResults'), ('result_key', "*

 * *                 "'OutpostResolvers')])}"}*

```diff
@@ -32,14 +32,20 @@
         },
         "ListFirewallRules": {
             "input_token": "NextToken",
             "limit_key": "MaxResults",
             "output_token": "NextToken",
             "result_key": "FirewallRules"
         },
+        "ListOutpostResolvers": {
+            "input_token": "NextToken",
+            "limit_key": "MaxResults",
+            "output_token": "NextToken",
+            "result_key": "OutpostResolvers"
+        },
         "ListResolverConfigs": {
             "input_token": "NextToken",
             "limit_key": "MaxResults",
             "output_token": "NextToken",
             "result_key": "ResolverConfigs"
         },
         "ListResolverDnssecConfigs": {
```

### Comparing `botocore-a-la-carte-route53resolver-1.31.6/botocore/data/route53resolver/2018-04-01/paginators-1.sdk-extras.json` & `botocore-a-la-carte-route53resolver-1.31.8/botocore/data/route53resolver/2018-04-01/paginators-1.sdk-extras.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53resolver-1.31.6/botocore/data/route53resolver/2018-04-01/service-2.json` & `botocore-a-la-carte-route53resolver-1.31.8/botocore/data/route53resolver/2018-04-01/service-2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9856170829682153%*

 * *Differences: {"'operations'": "{'CreateOutpostResolver': OrderedDict([('name', 'CreateOutpostResolver'), "*

 * *                 "('http', OrderedDict([('method', 'POST'), ('requestUri', '/')])), ('input', "*

 * *                 "OrderedDict([('shape', 'CreateOutpostResolverRequest')])), ('output', "*

 * *                 "OrderedDict([('shape', 'CreateOutpostResolverResponse')])), ('errors', "*

 * *                 "[OrderedDict([('shape', 'AccessDeniedException')]), OrderedDict([('shape', "*

 * *                 "'InternalServiceErrorExcepti […]*

```diff
@@ -259,14 +259,48 @@
                 "shape": "CreateFirewallRuleGroupRequest"
             },
             "name": "CreateFirewallRuleGroup",
             "output": {
                 "shape": "CreateFirewallRuleGroupResponse"
             }
         },
+        "CreateOutpostResolver": {
+            "documentation": "<p>Creates an Route\u00a053 Resolver on an Outpost.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InternalServiceErrorException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "CreateOutpostResolverRequest"
+            },
+            "name": "CreateOutpostResolver",
+            "output": {
+                "shape": "CreateOutpostResolverResponse"
+            }
+        },
         "CreateResolverEndpoint": {
             "documentation": "<p>Creates a Resolver endpoint. There are two types of Resolver endpoints, inbound and outbound:</p> <ul> <li> <p>An <i>inbound Resolver endpoint</i> forwards DNS queries to the DNS service for a VPC from your network.</p> </li> <li> <p>An <i>outbound Resolver endpoint</i> forwards DNS queries from the DNS service for a VPC to your network.</p> </li> </ul>",
             "errors": [
                 {
                     "shape": "InvalidParameterException"
                 },
                 {
@@ -469,14 +503,48 @@
                 "shape": "DeleteFirewallRuleGroupRequest"
             },
             "name": "DeleteFirewallRuleGroup",
             "output": {
                 "shape": "DeleteFirewallRuleGroupResponse"
             }
         },
+        "DeleteOutpostResolver": {
+            "documentation": "<p>Deletes a Resolver on the Outpost.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "InternalServiceErrorException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "DeleteOutpostResolverRequest"
+            },
+            "name": "DeleteOutpostResolver",
+            "output": {
+                "shape": "DeleteOutpostResolverResponse"
+            }
+        },
         "DeleteResolverEndpoint": {
             "documentation": "<p>Deletes a Resolver endpoint. The effect of deleting a Resolver endpoint depends on whether it's an inbound or an outbound Resolver endpoint:</p> <ul> <li> <p> <b>Inbound</b>: DNS queries from your network are no longer routed to the DNS service for the specified VPC.</p> </li> <li> <p> <b>Outbound</b>: DNS queries from a VPC are no longer routed to your network.</p> </li> </ul>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
@@ -841,14 +909,45 @@
                 "shape": "GetFirewallRuleGroupPolicyRequest"
             },
             "name": "GetFirewallRuleGroupPolicy",
             "output": {
                 "shape": "GetFirewallRuleGroupPolicyResponse"
             }
         },
+        "GetOutpostResolver": {
+            "documentation": "<p>Gets information about a specified Resolver on the Outpost, such as its instance count and type, name, and the current status of the Resolver.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InternalServiceErrorException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "GetOutpostResolverRequest"
+            },
+            "name": "GetOutpostResolver",
+            "output": {
+                "shape": "GetOutpostResolverResponse"
+            }
+        },
         "GetResolverConfig": {
             "documentation": "<p>Retrieves the behavior configuration of Route\u00a053 Resolver behavior for a single VPC from Amazon Virtual Private Cloud.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
@@ -1331,14 +1430,45 @@
                 "shape": "ListFirewallRulesRequest"
             },
             "name": "ListFirewallRules",
             "output": {
                 "shape": "ListFirewallRulesResponse"
             }
         },
+        "ListOutpostResolvers": {
+            "documentation": "<p>Lists all the Resolvers on Outposts that were created using the current Amazon Web Services account.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InternalServiceErrorException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "ListOutpostResolversRequest"
+            },
+            "name": "ListOutpostResolvers",
+            "output": {
+                "shape": "ListOutpostResolversResponse"
+            }
+        },
         "ListResolverConfigs": {
             "documentation": "<p>Retrieves the Resolver configurations that you have defined. Route\u00a053 Resolver uses the configurations to manage DNS resolution behavior for your VPCs.</p>",
             "errors": [
                 {
                     "shape": "InvalidNextTokenException"
                 },
                 {
@@ -1928,14 +2058,51 @@
                 "shape": "UpdateFirewallRuleGroupAssociationRequest"
             },
             "name": "UpdateFirewallRuleGroupAssociation",
             "output": {
                 "shape": "UpdateFirewallRuleGroupAssociationResponse"
             }
         },
+        "UpdateOutpostResolver": {
+            "documentation": "<p>You can use <code>UpdateOutpostResolver</code> to update the instance count, type, or name of a Resolver on an Outpost.</p>",
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "InternalServiceErrorException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "UpdateOutpostResolverRequest"
+            },
+            "name": "UpdateOutpostResolver",
+            "output": {
+                "shape": "UpdateOutpostResolverResponse"
+            }
+        },
         "UpdateResolverConfig": {
             "documentation": "<p>Updates the behavior configuration of Route\u00a053 Resolver behavior for a single VPC from Amazon Virtual Private Cloud.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
@@ -2416,14 +2583,60 @@
                 "FirewallRule": {
                     "documentation": "<p>The firewall rule that you just created. </p>",
                     "shape": "FirewallRule"
                 }
             },
             "type": "structure"
         },
+        "CreateOutpostResolverRequest": {
+            "members": {
+                "CreatorRequestId": {
+                    "documentation": "<p>A unique string that identifies the request and that allows failed requests to be retried without the risk of running the operation twice. </p> <p> <code>CreatorRequestId</code> can be any unique string, for example, a date/time stamp.</p>",
+                    "shape": "CreatorRequestId"
+                },
+                "InstanceCount": {
+                    "box": true,
+                    "documentation": "<p>Number of Amazon EC2 instances for the Resolver on Outpost. The default and minimal value is 4.</p>",
+                    "shape": "InstanceCount"
+                },
+                "Name": {
+                    "documentation": "<p>A friendly name that lets you easily find a configuration in the Resolver dashboard in the Route\u00a053 console.</p>",
+                    "shape": "OutpostResolverName"
+                },
+                "OutpostArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the Outpost. If you specify this, you must also specify a value for the <code>PreferredInstanceType</code>.</p>",
+                    "shape": "OutpostArn"
+                },
+                "PreferredInstanceType": {
+                    "documentation": "<p> The Amazon EC2 instance type. If you specify this, you must also specify a value for the <code>OutpostArn</code>. </p>",
+                    "shape": "OutpostInstanceType"
+                },
+                "Tags": {
+                    "box": true,
+                    "documentation": "<p> A string that helps identify the Route\u00a053 Resolvers on Outpost. </p>",
+                    "shape": "TagList"
+                }
+            },
+            "required": [
+                "CreatorRequestId",
+                "Name",
+                "PreferredInstanceType",
+                "OutpostArn"
+            ],
+            "type": "structure"
+        },
+        "CreateOutpostResolverResponse": {
+            "members": {
+                "OutpostResolver": {
+                    "documentation": "<p>Information about the <code>CreateOutpostResolver</code> request, including the status of the request.</p>",
+                    "shape": "OutpostResolver"
+                }
+            },
+            "type": "structure"
+        },
         "CreateResolverEndpointRequest": {
             "members": {
                 "CreatorRequestId": {
                     "documentation": "<p>A unique string that identifies the request and that allows failed requests to be retried without the risk of running the operation twice. <code>CreatorRequestId</code> can be any unique string, for example, a date/time stamp. </p>",
                     "shape": "CreatorRequestId"
                 },
                 "Direction": {
@@ -2434,17 +2647,27 @@
                     "documentation": "<p>The subnets and IP addresses in your VPC that DNS queries originate from (for outbound endpoints) or that you forward DNS queries to (for inbound endpoints). The subnet ID uniquely identifies a VPC. </p>",
                     "shape": "IpAddressesRequest"
                 },
                 "Name": {
                     "documentation": "<p>A friendly name that lets you easily find a configuration in the Resolver dashboard in the Route 53 console.</p>",
                     "shape": "Name"
                 },
+                "OutpostArn": {
+                    "box": true,
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the Outpost. If you specify this, you must also specify a value for the <code>PreferredInstanceType</code>. </p>",
+                    "shape": "OutpostArn"
+                },
+                "PreferredInstanceType": {
+                    "box": true,
+                    "documentation": "<p>The instance type. If you specify this, you must also specify a value for the <code>OutpostArn</code>.</p>",
+                    "shape": "OutpostInstanceType"
+                },
                 "ResolverEndpointType": {
                     "box": true,
-                    "documentation": "<p> For the endpoint type you can choose either IPv4, IPv6. or dual-stack. A dual-stack endpoint means that it will resolve via both IPv4 and IPv6. This endpoint type is applied to all IP addresses. </p>",
+                    "documentation": "<p> For the endpoint type you can choose either IPv4, IPv6, or dual-stack. A dual-stack endpoint means that it will resolve via both IPv4 and IPv6. This endpoint type is applied to all IP addresses. </p>",
                     "shape": "ResolverEndpointType"
                 },
                 "SecurityGroupIds": {
                     "box": true,
                     "documentation": "<p>The ID of one or more security groups that you want to use to control access to this VPC. The security group that you specify must include one or more inbound rules (for inbound Resolver endpoints) or outbound rules (for outbound Resolver endpoints). Inbound and outbound rules must allow TCP and UDP access. For inbound access, open port 53. For outbound access, open the port that you're using for DNS queries on your network.</p>",
                     "shape": "SecurityGroupIds"
                 },
@@ -2534,15 +2757,15 @@
                 "Tags": {
                     "box": true,
                     "documentation": "<p>A list of the tag keys and values that you want to associate with the endpoint.</p>",
                     "shape": "TagList"
                 },
                 "TargetIps": {
                     "box": true,
-                    "documentation": "<p>The IPs that you want Resolver to forward DNS queries to. You can specify only IPv4 addresses. Separate IP addresses with a space.</p> <p> <code>TargetIps</code> is available only when the value of <code>Rule type</code> is <code>FORWARD</code>.</p>",
+                    "documentation": "<p>The IPs that you want Resolver to forward DNS queries to. You can specify either Ipv4 or Ipv6 addresses but not both in the same rule. Separate IP addresses with a space.</p> <p> <code>TargetIps</code> is available only when the value of <code>Rule type</code> is <code>FORWARD</code>.</p>",
                     "shape": "TargetList"
                 }
             },
             "required": [
                 "CreatorRequestId",
                 "RuleType",
                 "DomainName"
@@ -2627,14 +2850,35 @@
                 "FirewallRule": {
                     "documentation": "<p>The specification for the firewall rule that you just deleted.</p>",
                     "shape": "FirewallRule"
                 }
             },
             "type": "structure"
         },
+        "DeleteOutpostResolverRequest": {
+            "members": {
+                "Id": {
+                    "documentation": "<p>A unique string that identifies the Resolver on the Outpost.</p>",
+                    "shape": "ResourceId"
+                }
+            },
+            "required": [
+                "Id"
+            ],
+            "type": "structure"
+        },
+        "DeleteOutpostResolverResponse": {
+            "members": {
+                "OutpostResolver": {
+                    "documentation": "<p>Information about the <code>DeleteOutpostResolver</code> request, including the status of the request.</p>",
+                    "shape": "OutpostResolver"
+                }
+            },
+            "type": "structure"
+        },
         "DeleteResolverEndpointRequest": {
             "members": {
                 "ResolverEndpointId": {
                     "documentation": "<p>The ID of the Resolver endpoint that you want to delete.</p>",
                     "shape": "ResourceId"
                 }
             },
@@ -3327,14 +3571,35 @@
                 "FirewallRuleGroup": {
                     "documentation": "<p>A collection of rules used to filter DNS network traffic. </p>",
                     "shape": "FirewallRuleGroup"
                 }
             },
             "type": "structure"
         },
+        "GetOutpostResolverRequest": {
+            "members": {
+                "Id": {
+                    "documentation": "<p>The ID of the Resolver on the Outpost.</p>",
+                    "shape": "ResourceId"
+                }
+            },
+            "required": [
+                "Id"
+            ],
+            "type": "structure"
+        },
+        "GetOutpostResolverResponse": {
+            "members": {
+                "OutpostResolver": {
+                    "documentation": "<p>Information about the <code>GetOutpostResolver</code> request, including the status of the request.</p>",
+                    "shape": "OutpostResolver"
+                }
+            },
+            "type": "structure"
+        },
         "GetResolverConfigRequest": {
             "members": {
                 "ResourceId": {
                     "documentation": "<p>Resource ID of the Amazon VPC that you want to get information about.</p>",
                     "shape": "ResourceId"
                 }
             },
@@ -3559,14 +3824,17 @@
                 "StatusMessage": {
                     "documentation": "<p>Additional information about the status of the list, if available.</p>",
                     "shape": "StatusMessage"
                 }
             },
             "type": "structure"
         },
+        "InstanceCount": {
+            "type": "integer"
+        },
         "InternalServiceErrorException": {
             "documentation": "<p>We encountered an unknown error. Try again in a few minutes.</p>",
             "exception": true,
             "members": {
                 "Message": {
                     "shape": "ExceptionMessage"
                 }
@@ -3707,15 +3975,16 @@
                 "ATTACHED",
                 "REMAP_DETACHING",
                 "REMAP_ATTACHING",
                 "DETACHING",
                 "FAILED_RESOURCE_GONE",
                 "DELETING",
                 "DELETE_FAILED_FAS_EXPIRED",
-                "UPDATING"
+                "UPDATING",
+                "UPDATE_FAILED"
             ],
             "type": "string"
         },
         "IpAddressUpdate": {
             "documentation": "<p>In an <a href=\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_UpdateResolverEndpoint.html\">UpdateResolverEndpoint</a> request, information about an IP address to update.</p>",
             "members": {
                 "Ip": {
@@ -3992,14 +4261,47 @@
                 "NextToken": {
                     "documentation": "<p>If objects are still available for retrieval, Resolver returns this token in the response. To retrieve the next batch of objects, provide this token in your next request.</p>",
                     "shape": "NextToken"
                 }
             },
             "type": "structure"
         },
+        "ListOutpostResolversRequest": {
+            "members": {
+                "MaxResults": {
+                    "box": true,
+                    "documentation": "<p>The maximum number of Resolvers on the Outpost that you want to return in the response to a <code>ListOutpostResolver</code> request. If you don't specify a value for <code>MaxResults</code>, the request returns up to 100 Resolvers.</p>",
+                    "shape": "MaxResults"
+                },
+                "NextToken": {
+                    "box": true,
+                    "documentation": "<p>For the first <code>ListOutpostResolver</code> request, omit this value.</p> <p/>",
+                    "shape": "NextToken"
+                },
+                "OutpostArn": {
+                    "box": true,
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the Outpost.</p>",
+                    "shape": "OutpostArn"
+                }
+            },
+            "type": "structure"
+        },
+        "ListOutpostResolversResponse": {
+            "members": {
+                "NextToken": {
+                    "documentation": "<p>If more than <code>MaxResults</code> Resolvers match the specified criteria, you can submit another <code>ListOutpostResolver</code> request to get the next group of results. In the next request, specify the value of <code>NextToken</code> from the previous response.</p>",
+                    "shape": "NextToken"
+                },
+                "OutpostResolvers": {
+                    "documentation": "<p>The Resolvers on Outposts that were created by using the current Amazon Web Services account, and that match the specified filters, if any.</p>",
+                    "shape": "OutpostResolverList"
+                }
+            },
+            "type": "structure"
+        },
         "ListResolverConfigsMaxResult": {
             "max": 100,
             "min": 5,
             "type": "integer"
         },
         "ListResolverConfigsRequest": {
             "members": {
@@ -4358,14 +4660,102 @@
             "max": 64,
             "pattern": "(?!^[0-9]+$)([a-zA-Z0-9\\-_' ']+)",
             "type": "string"
         },
         "NextToken": {
             "type": "string"
         },
+        "OutpostArn": {
+            "max": 255,
+            "min": 1,
+            "pattern": "^arn:aws([a-z-]+)?:outposts:[a-z\\d-]+:\\d{12}:outpost/op-[a-f0-9]{17}$",
+            "type": "string"
+        },
+        "OutpostInstanceType": {
+            "max": 255,
+            "min": 1,
+            "type": "string"
+        },
+        "OutpostResolver": {
+            "documentation": "<p>A complex type that contains settings for an existing Resolver on an Outpost.</p>",
+            "members": {
+                "Arn": {
+                    "documentation": "<p>The ARN (Amazon Resource Name) for the Resolver on an Outpost.</p>",
+                    "shape": "Arn"
+                },
+                "CreationTime": {
+                    "documentation": "<p>The date and time that the Outpost Resolver was created, in Unix time format and Coordinated Universal Time (UTC).</p>",
+                    "shape": "Rfc3339TimeString"
+                },
+                "CreatorRequestId": {
+                    "documentation": "<p>A unique string that identifies the request that created the Resolver endpoint. The <code>CreatorRequestId</code> allows failed requests to be retried without the risk of running the operation twice.</p>",
+                    "shape": "CreatorRequestId"
+                },
+                "Id": {
+                    "documentation": "<p>The ID of the Resolver on Outpost.</p>",
+                    "shape": "ResourceId"
+                },
+                "InstanceCount": {
+                    "documentation": "<p>Amazon EC2 instance count for the Resolver on the Outpost.</p>",
+                    "shape": "InstanceCount"
+                },
+                "ModificationTime": {
+                    "documentation": "<p>The date and time that the Outpost Resolver was modified, in Unix time format and Coordinated Universal Time (UTC).</p>",
+                    "shape": "Rfc3339TimeString"
+                },
+                "Name": {
+                    "documentation": "<p>Name of the Resolver.</p>",
+                    "shape": "OutpostResolverName"
+                },
+                "OutpostArn": {
+                    "documentation": "<p>The ARN (Amazon Resource Name) for the Outpost.</p>",
+                    "shape": "OutpostArn"
+                },
+                "PreferredInstanceType": {
+                    "documentation": "<p> The Amazon EC2 instance type. </p>",
+                    "shape": "OutpostInstanceType"
+                },
+                "Status": {
+                    "documentation": "<p>Status of the Resolver.</p>",
+                    "shape": "OutpostResolverStatus"
+                },
+                "StatusMessage": {
+                    "documentation": "<p>A detailed description of the Resolver.</p>",
+                    "shape": "OutpostResolverStatusMessage"
+                }
+            },
+            "type": "structure"
+        },
+        "OutpostResolverList": {
+            "member": {
+                "shape": "OutpostResolver"
+            },
+            "type": "list"
+        },
+        "OutpostResolverName": {
+            "max": 255,
+            "min": 1,
+            "type": "string"
+        },
+        "OutpostResolverStatus": {
+            "enum": [
+                "CREATING",
+                "OPERATIONAL",
+                "UPDATING",
+                "DELETING",
+                "ACTION_NEEDED",
+                "FAILED_CREATION",
+                "FAILED_DELETION"
+            ],
+            "type": "string"
+        },
+        "OutpostResolverStatusMessage": {
+            "max": 4096,
+            "type": "string"
+        },
         "Port": {
             "max": 65535,
             "min": 0,
             "type": "integer"
         },
         "Priority": {
             "type": "integer"
@@ -4399,15 +4789,15 @@
         "PutResolverQueryLogConfigPolicyRequest": {
             "members": {
                 "Arn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the account that you want to share rules with.</p>",
                     "shape": "Arn"
                 },
                 "ResolverQueryLogConfigPolicy": {
-                    "documentation": "<p>An Identity and Access Management policy statement that lists the query logging configurations that you want to share with another Amazon Web Services account and the operations that you want the account to be able to perform. You can specify the following operations in the <code>Actions</code> section of the statement:</p> <ul> <li> <p> <code>route53resolver:AssociateResolverQueryLogConfig</code> </p> </li> <li> <p> <code>route53resolver:DisassociateResolverQueryLogConfig</code> </p> </li> <li> <p> <code>route53resolver:ListResolverQueryLogConfigAssociations</code> </p> </li> <li> <p> <code>route53resolver:ListResolverQueryLogConfigs</code> </p> </li> </ul> <p>In the <code>Resource</code> section of the statement, you specify the ARNs for the query logging configurations that you want to share with the account that you specified in <code>Arn</code>. </p>",
+                    "documentation": "<p>An Identity and Access Management policy statement that lists the query logging configurations that you want to share with another Amazon Web Services account and the operations that you want the account to be able to perform. You can specify the following operations in the <code>Actions</code> section of the statement:</p> <ul> <li> <p> <code>route53resolver:AssociateResolverQueryLogConfig</code> </p> </li> <li> <p> <code>route53resolver:DisassociateResolverQueryLogConfig</code> </p> </li> <li> <p> <code>route53resolver:ListResolverQueryLogConfigs</code> </p> </li> </ul> <p>In the <code>Resource</code> section of the statement, you specify the ARNs for the query logging configurations that you want to share with the account that you specified in <code>Arn</code>. </p>",
                     "shape": "ResolverQueryLogConfigPolicy"
                 }
             },
             "required": [
                 "Arn",
                 "ResolverQueryLogConfigPolicy"
             ],
@@ -4563,14 +4953,22 @@
                     "documentation": "<p>The date and time that the endpoint was last modified, in Unix time format and Coordinated Universal Time (UTC).</p>",
                     "shape": "Rfc3339TimeString"
                 },
                 "Name": {
                     "documentation": "<p>The name that you assigned to the Resolver endpoint when you submitted a <a href=\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_CreateResolverEndpoint.html\">CreateResolverEndpoint</a> request.</p>",
                     "shape": "Name"
                 },
+                "OutpostArn": {
+                    "documentation": "<p>The ARN (Amazon Resource Name) for the Outpost.</p>",
+                    "shape": "OutpostArn"
+                },
+                "PreferredInstanceType": {
+                    "documentation": "<p> The Amazon EC2 instance type. </p>",
+                    "shape": "OutpostInstanceType"
+                },
                 "ResolverEndpointType": {
                     "documentation": "<p> The Resolver endpoint IP address type. </p>",
                     "shape": "ResolverEndpointType"
                 },
                 "SecurityGroupIds": {
                     "documentation": "<p>The ID of one or more security groups that control access to this VPC. The security group must include one or more inbound rules (for inbound endpoints) or outbound rules (for outbound endpoints). Inbound and outbound rules must allow TCP and UDP access. For inbound access, open port 53. For outbound access, open the port that you're using for DNS queries on your network.</p>",
                     "shape": "SecurityGroupIds"
@@ -4803,15 +5201,15 @@
                     "shape": "ResolverRuleStatus"
                 },
                 "StatusMessage": {
                     "documentation": "<p>A detailed description of the status of a Resolver rule.</p>",
                     "shape": "StatusMessage"
                 },
                 "TargetIps": {
-                    "documentation": "<p>An array that contains the IP addresses and ports that an outbound endpoint forwards DNS queries to. Typically, these are the IP addresses of DNS resolvers on your network. Specify IPv4 addresses. IPv6 is not supported.</p>",
+                    "documentation": "<p>An array that contains the IP addresses and ports that an outbound endpoint forwards DNS queries to. Typically, these are the IP addresses of DNS resolvers on your network. </p>",
                     "shape": "TargetList"
                 }
             },
             "type": "structure"
         },
         "ResolverRuleAssociation": {
             "documentation": "<p>In the response to an <a href=\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_AssociateResolverRule.html\">AssociateResolverRule</a>, <a href=\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_DisassociateResolverRule.html\">DisassociateResolverRule</a>, or <a href=\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_ListResolverRuleAssociations.html\">ListResolverRuleAssociations</a> request, provides information about an association between a Resolver rule and a VPC. The association determines which DNS queries that originate in the VPC are forwarded to your network. </p>",
@@ -4977,14 +5375,24 @@
             "type": "list"
         },
         "ServicePrinciple": {
             "max": 512,
             "min": 1,
             "type": "string"
         },
+        "ServiceQuotaExceededException": {
+            "documentation": "<p>Fulfilling the request would cause one or more quotas to be exceeded.</p>",
+            "exception": true,
+            "members": {
+                "Message": {
+                    "shape": "ExceptionMessage"
+                }
+            },
+            "type": "structure"
+        },
         "ShareStatus": {
             "enum": [
                 "NOT_SHARED",
                 "SHARED_WITH_ME",
                 "SHARED_BY_ME"
             ],
             "type": "string"
@@ -5336,14 +5744,50 @@
             "max": 50,
             "member": {
                 "shape": "UpdateIpAddress"
             },
             "min": 0,
             "type": "list"
         },
+        "UpdateOutpostResolverRequest": {
+            "members": {
+                "Id": {
+                    "documentation": "<p>A unique string that identifies Resolver on an Outpost.</p>",
+                    "shape": "ResourceId"
+                },
+                "InstanceCount": {
+                    "box": true,
+                    "documentation": "<p>The Amazon EC2 instance count for a Resolver on the Outpost.</p>",
+                    "shape": "InstanceCount"
+                },
+                "Name": {
+                    "box": true,
+                    "documentation": "<p>Name of the Resolver on the Outpost.</p>",
+                    "shape": "OutpostResolverName"
+                },
+                "PreferredInstanceType": {
+                    "box": true,
+                    "documentation": "<p> Amazon EC2 instance type. </p>",
+                    "shape": "OutpostInstanceType"
+                }
+            },
+            "required": [
+                "Id"
+            ],
+            "type": "structure"
+        },
+        "UpdateOutpostResolverResponse": {
+            "members": {
+                "OutpostResolver": {
+                    "documentation": "<p>The response to an <code>UpdateOutpostResolver</code> request.</p>",
+                    "shape": "OutpostResolver"
+                }
+            },
+            "type": "structure"
+        },
         "UpdateResolverConfigRequest": {
             "members": {
                 "AutodefinedReverseFlag": {
                     "documentation": "<p>Indicates whether or not the Resolver will create autodefined rules for reverse DNS lookups. This is enabled by default. Disabling this option will also affect EC2-Classic instances using ClassicLink. For more information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/vpc-classiclink.html\">ClassicLink</a> in the <i>Amazon EC2 guide</i>.</p> <important> <p>We are retiring EC2-Classic on August 15, 2022. We recommend that you migrate from EC2-Classic to a VPC. For more information, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/vpc-migrate.html\">Migrate from EC2-Classic to a VPC</a> in the <i>Amazon EC2 guide</i> and the blog <a href=\"http://aws.amazon.com/blogs/aws/ec2-classic-is-retiring-heres-how-to-prepare/\">EC2-Classic Networking is Retiring \u2013 Here\u2019s How to Prepare</a>.</p> </important> <note> <p>It can take some time for the status change to be completed.</p> </note> <p/>",
                     "shape": "AutodefinedReverseFlag"
                 },
                 "ResourceId": {
@@ -5401,20 +5845,20 @@
                 },
                 "ResolverEndpointId": {
                     "documentation": "<p>The ID of the Resolver endpoint that you want to update.</p>",
                     "shape": "ResourceId"
                 },
                 "ResolverEndpointType": {
                     "box": true,
-                    "documentation": "<p> Specifies the endpoint type for what type of IP address the endpoint uses to forward DNS queries. </p>",
+                    "documentation": "<p> Specifies the endpoint type for what type of IP address the endpoint uses to forward DNS queries. </p> <p>Updating to <code>IPV6</code> type isn't currently supported.</p>",
                     "shape": "ResolverEndpointType"
                 },
                 "UpdateIpAddresses": {
                     "box": true,
-                    "documentation": "<p> Updates the Resolver endpoint type to IpV4, Ipv6, or dual-stack. </p>",
+                    "documentation": "<p> Specifies the IPv6 address when you update the Resolver endpoint from IPv4 to dual-stack. If you don't specify an IPv6 address, one will be automatically chosen from your subnet. </p>",
                     "shape": "UpdateIpAddresses"
                 }
             },
             "required": [
                 "ResolverEndpointId"
             ],
             "type": "structure"
```

### Comparing `botocore-a-la-carte-route53resolver-1.31.6/botocore_a_la_carte_route53resolver.egg-info/PKG-INFO` & `botocore-a-la-carte-route53resolver-1.31.8/botocore_a_la_carte_route53resolver.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-route53resolver
-Version: 1.31.6
+Version: 1.31.8
 Summary: route53resolver data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-route53resolver-1.31.6/botocore_a_la_carte_route53resolver.egg-info/SOURCES.txt` & `botocore-a-la-carte-route53resolver-1.31.8/botocore_a_la_carte_route53resolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53resolver-1.31.6/setup.py` & `botocore-a-la-carte-route53resolver-1.31.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-route53resolver',
-    version="1.31.6",
+    version="1.31.8",
     description='route53resolver data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/route53resolver/*/*.json'],
```

