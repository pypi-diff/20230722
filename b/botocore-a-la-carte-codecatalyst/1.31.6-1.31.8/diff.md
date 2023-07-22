# Comparing `tmp/botocore-a-la-carte-codecatalyst-1.31.6.tar.gz` & `tmp/botocore-a-la-carte-codecatalyst-1.31.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-codecatalyst-1.31.6.tar", last modified: Thu Jul 20 01:20:06 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-codecatalyst-1.31.8.tar", last modified: Fri Jul 21 01:21:14 2023, max compression
```

## Comparing `botocore-a-la-carte-codecatalyst-1.31.6.tar` & `botocore-a-la-carte-codecatalyst-1.31.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:06.146567 botocore-a-la-carte-codecatalyst-1.31.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-20 01:20:05.000000 botocore-a-la-carte-codecatalyst-1.31.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-20 01:20:06.146567 botocore-a-la-carte-codecatalyst-1.31.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:06.142567 botocore-a-la-carte-codecatalyst-1.31.6/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:06.142567 botocore-a-la-carte-codecatalyst-1.31.6/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:06.146567 botocore-a-la-carte-codecatalyst-1.31.6/botocore/data/codecatalyst/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:06.146567 botocore-a-la-carte-codecatalyst-1.31.6/botocore/data/codecatalyst/2022-09-28/
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-20 01:19:55.000000 botocore-a-la-carte-codecatalyst-1.31.6/botocore/data/codecatalyst/2022-09-28/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-20 01:19:55.000000 botocore-a-la-carte-codecatalyst-1.31.6/botocore/data/codecatalyst/2022-09-28/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   100921 2023-07-20 01:19:55.000000 botocore-a-la-carte-codecatalyst-1.31.6/botocore/data/codecatalyst/2022-09-28/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 01:19:55.000000 botocore-a-la-carte-codecatalyst-1.31.6/botocore/data/codecatalyst/2022-09-28/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:20:06.146567 botocore-a-la-carte-codecatalyst-1.31.6/botocore_a_la_carte_codecatalyst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-20 01:20:06.000000 botocore-a-la-carte-codecatalyst-1.31.6/botocore_a_la_carte_codecatalyst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-20 01:20:06.000000 botocore-a-la-carte-codecatalyst-1.31.6/botocore_a_la_carte_codecatalyst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 01:20:06.000000 botocore-a-la-carte-codecatalyst-1.31.6/botocore_a_la_carte_codecatalyst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 01:20:06.000000 botocore-a-la-carte-codecatalyst-1.31.6/botocore_a_la_carte_codecatalyst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 01:20:06.146567 botocore-a-la-carte-codecatalyst-1.31.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-20 01:20:05.000000 botocore-a-la-carte-codecatalyst-1.31.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:14.594800 botocore-a-la-carte-codecatalyst-1.31.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:14.000000 botocore-a-la-carte-codecatalyst-1.31.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-21 01:21:14.594800 botocore-a-la-carte-codecatalyst-1.31.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:14.594800 botocore-a-la-carte-codecatalyst-1.31.8/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:14.594800 botocore-a-la-carte-codecatalyst-1.31.8/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:14.594800 botocore-a-la-carte-codecatalyst-1.31.8/botocore/data/codecatalyst/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:14.594800 botocore-a-la-carte-codecatalyst-1.31.8/botocore/data/codecatalyst/2022-09-28/
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-21 01:21:06.000000 botocore-a-la-carte-codecatalyst-1.31.8/botocore/data/codecatalyst/2022-09-28/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-21 01:21:06.000000 botocore-a-la-carte-codecatalyst-1.31.8/botocore/data/codecatalyst/2022-09-28/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   116958 2023-07-21 01:21:06.000000 botocore-a-la-carte-codecatalyst-1.31.8/botocore/data/codecatalyst/2022-09-28/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-21 01:21:06.000000 botocore-a-la-carte-codecatalyst-1.31.8/botocore/data/codecatalyst/2022-09-28/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:14.594800 botocore-a-la-carte-codecatalyst-1.31.8/botocore_a_la_carte_codecatalyst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-21 01:21:14.000000 botocore-a-la-carte-codecatalyst-1.31.8/botocore_a_la_carte_codecatalyst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-21 01:21:14.000000 botocore-a-la-carte-codecatalyst-1.31.8/botocore_a_la_carte_codecatalyst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:14.000000 botocore-a-la-carte-codecatalyst-1.31.8/botocore_a_la_carte_codecatalyst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:14.000000 botocore-a-la-carte-codecatalyst-1.31.8/botocore_a_la_carte_codecatalyst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:14.594800 botocore-a-la-carte-codecatalyst-1.31.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-21 01:21:14.000000 botocore-a-la-carte-codecatalyst-1.31.8/setup.py
```

### Comparing `botocore-a-la-carte-codecatalyst-1.31.6/LICENSE.txt` & `botocore-a-la-carte-codecatalyst-1.31.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codecatalyst-1.31.6/PKG-INFO` & `botocore-a-la-carte-codecatalyst-1.31.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-codecatalyst
-Version: 1.31.6
+Version: 1.31.8
 Summary: codecatalyst data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-codecatalyst-1.31.6/botocore/data/codecatalyst/2022-09-28/endpoint-rule-set-1.json` & `botocore-a-la-carte-codecatalyst-1.31.8/botocore/data/codecatalyst/2022-09-28/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codecatalyst-1.31.6/botocore/data/codecatalyst/2022-09-28/paginators-1.json` & `botocore-a-la-carte-codecatalyst-1.31.8/botocore/data/codecatalyst/2022-09-28/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codecatalyst-1.31.6/botocore/data/codecatalyst/2022-09-28/service-2.json` & `botocore-a-la-carte-codecatalyst-1.31.8/botocore/data/codecatalyst/2022-09-28/service-2.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.87022165831492%*

 * *Differences: {"'documentation'": "'<p>Welcome to the Amazon CodeCatalyst API reference. This reference provides "*

 * *                    'descriptions of operations and data types for Amazon CodeCatalyst. You can '*

 * *                    'use the Amazon CodeCatalyst API to work with the following objects. </p> '*

 * *                    '<p>Spaces, by calling the following:</p> <ul> <li> <p> <a>DeleteSpace</a>, '*

 * *                    'which deletes a space.</p> </li> <li> <p> <a>GetSpace</a>, which returns '*

 * *                    'in […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "documentation": "<p>Welcome to the Amazon CodeCatalyst API reference. This reference provides descriptions of operations and data types for Amazon CodeCatalyst. You can use the Amazon CodeCatalyst API to work with the following objects. </p> <p>Dev Environments and the Amazon Web Services Toolkits, by calling the following:</p> <ul> <li> <p> <a>CreateAccessToken</a>, which creates a personal access token (PAT) for the current user.</p> </li> <li> <p> <a>CreateDevEnvironment</a>, which creates a Dev Environment, where you can quickly work on the code stored in the source repositories of your project.</p> </li> <li> <p> <a>CreateProject</a> which creates a project in a specified space.</p> </li> <li> <p> <a>CreateSourceRepositoryBranch</a>, which creates a branch in a specified repository where you can work on code.</p> </li> <li> <p> <a>DeleteDevEnvironment</a>, which deletes a Dev Environment.</p> </li> <li> <p> <a>GetDevEnvironment</a>, which returns information about a Dev Environment.</p> </li> <li> <p> <a>GetProject</a>, which returns information about a project.</p> </li> <li> <p> <a>GetSourceRepositoryCloneUrls</a>, which returns information about the URLs that can be used with a Git client to clone a source repository.</p> </li> <li> <p> <a>GetSpace</a>, which returns information about a space.</p> </li> <li> <p> <a>GetSubscription</a>, which returns information about the Amazon Web Services account used for billing purposes and the billing plan for the space.</p> </li> <li> <p> <a>GetUserDetails</a>, which returns information about a user in Amazon CodeCatalyst.</p> </li> <li> <p> <a>ListDevEnvironments</a>, which retrieves a list of Dev Environments in a project.</p> </li> <li> <p> <a>ListDevEnvironmentSessions</a>, which retrieves a list of active Dev Environment sessions in a project.</p> </li> <li> <p> <a>ListProjects</a>, which retrieves a list of projects in a space.</p> </li> <li> <p> <a>ListSourceRepositories</a>, which retrieves a list of source repositories in a project.</p> </li> <li> <p> <a>ListSourceRepositoryBranches</a>, which retrieves a list of branches in a source repository.</p> </li> <li> <p> <a>ListSpaces</a>, which retrieves a list of spaces.</p> </li> <li> <p> <a>StartDevEnvironment</a>, which starts a specified Dev Environment and puts it into an active state.</p> </li> <li> <p> <a>StartDevEnvironmentSession</a>, which starts a session to a specified Dev Environment.</p> </li> <li> <p> <a>StopDevEnvironment</a>, which stops a specified Dev Environment and puts it into an stopped state.</p> </li> <li> <p> <a>StopDevEnvironmentSession</a>, which stops a session for a specified Dev Environment.</p> </li> <li> <p> <a>UpdateDevEnvironment</a>, which changes one or more values for a Dev Environment.</p> </li> <li> <p> <a>VerifySession</a>, which verifies whether the calling user has a valid Amazon CodeCatalyst login and session.</p> </li> </ul> <p>Security, activity, and resource management in Amazon CodeCatalyst, by calling the following:</p> <ul> <li> <p> <a>DeleteAccessToken</a>, which deletes a specified personal access token (PAT).</p> </li> <li> <p> <a>ListAccessTokens</a>, which lists all personal access tokens (PATs) associated with a user.</p> </li> <li> <p> <a>ListEventLogs</a>, which retrieves a list of events that occurred during a specified time period in a space.</p> </li> </ul> <note> <p>If you are using the Amazon CodeCatalyst APIs with an SDK or the CLI, you must configure your computer to work with Amazon CodeCatalyst and single sign-on (SSO). For more information, see <a href=\"https://docs.aws.amazon.com/codecatalyst/latest/userguide/set-up-cli.html\">Setting up to use the CLI with Amazon CodeCatalyst</a> and the SSO documentation for your SDK.</p> </note>",
+    "documentation": "<p>Welcome to the Amazon CodeCatalyst API reference. This reference provides descriptions of operations and data types for Amazon CodeCatalyst. You can use the Amazon CodeCatalyst API to work with the following objects. </p> <p>Spaces, by calling the following:</p> <ul> <li> <p> <a>DeleteSpace</a>, which deletes a space.</p> </li> <li> <p> <a>GetSpace</a>, which returns information about a space.</p> </li> <li> <p> <a>GetSubscription</a>, which returns information about the Amazon Web Services account used for billing purposes and the billing plan for the space.</p> </li> <li> <p> <a>ListSpaces</a>, which retrieves a list of spaces.</p> </li> <li> <p> <a>UpdateSpace</a>, which hanges one or more values for a space.</p> </li> </ul> <p>Projects, by calling the following:</p> <ul> <li> <p> <a>CreateProject</a> which creates a project in a specified space.</p> </li> <li> <p> <a>GetProject</a>, which returns information about a project.</p> </li> <li> <p> <a>ListProjects</a>, which retrieves a list of projects in a space.</p> </li> </ul> <p>Users, by calling the following:</p> <ul> <li> <p> <a>GetUserDetails</a>, which returns information about a user in Amazon CodeCatalyst.</p> </li> </ul> <p>Source repositories, by calling the following:</p> <ul> <li> <p> <a>CreateSourceRepository</a>, which creates an empty Git-based source repository in a specified project.</p> </li> <li> <p> <a>CreateSourceRepositoryBranch</a>, which creates a branch in a specified repository where you can work on code.</p> </li> <li> <p> <a>DeleteSourceRepository</a>, which deletes a source repository.</p> </li> <li> <p> <a>GetSourceRepository</a>, which returns information about a source repository.</p> </li> <li> <p> <a>GetSourceRepositoryCloneUrls</a>, which returns information about the URLs that can be used with a Git client to clone a source repository.</p> </li> <li> <p> <a>ListSourceRepositories</a>, which retrieves a list of source repositories in a project.</p> </li> <li> <p> <a>ListSourceRepositoryBranches</a>, which retrieves a list of branches in a source repository.</p> </li> </ul> <p>Dev Environments and the Amazon Web Services Toolkits, by calling the following:</p> <ul> <li> <p> <a>CreateDevEnvironment</a>, which creates a Dev Environment, where you can quickly work on the code stored in the source repositories of your project.</p> </li> <li> <p> <a>DeleteDevEnvironment</a>, which deletes a Dev Environment.</p> </li> <li> <p> <a>GetDevEnvironment</a>, which returns information about a Dev Environment.</p> </li> <li> <p> <a>ListDevEnvironments</a>, which retrieves a list of Dev Environments in a project.</p> </li> <li> <p> <a>ListDevEnvironmentSessions</a>, which retrieves a list of active Dev Environment sessions in a project.</p> </li> <li> <p> <a>StartDevEnvironment</a>, which starts a specified Dev Environment and puts it into an active state.</p> </li> <li> <p> <a>StartDevEnvironmentSession</a>, which starts a session to a specified Dev Environment.</p> </li> <li> <p> <a>StopDevEnvironment</a>, which stops a specified Dev Environment and puts it into an stopped state.</p> </li> <li> <p> <a>StopDevEnvironmentSession</a>, which stops a session for a specified Dev Environment.</p> </li> <li> <p> <a>UpdateDevEnvironment</a>, which changes one or more values for a Dev Environment.</p> </li> </ul> <p>Security, activity, and resource management in Amazon CodeCatalyst, by calling the following:</p> <ul> <li> <p> <a>CreateAccessToken</a>, which creates a personal access token (PAT) for the current user.</p> </li> <li> <p> <a>DeleteAccessToken</a>, which deletes a specified personal access token (PAT).</p> </li> <li> <p> <a>ListAccessTokens</a>, which lists all personal access tokens (PATs) associated with a user.</p> </li> <li> <p> <a>ListEventLogs</a>, which retrieves a list of events that occurred during a specified time period in a space.</p> </li> <li> <p> <a>VerifySession</a>, which verifies whether the calling user has a valid Amazon CodeCatalyst login and session.</p> </li> </ul> <note> <p>If you are using the Amazon CodeCatalyst APIs with an SDK or the CLI, you must configure your computer to work with Amazon CodeCatalyst and single sign-on (SSO). For more information, see <a href=\"https://docs.aws.amazon.com/codecatalyst/latest/userguide/set-up-cli.html\">Setting up to use the CLI with Amazon CodeCatalyst</a> and the SSO documentation for your SDK.</p> </note>",
     "metadata": {
         "apiVersion": "2022-09-28",
         "endpointPrefix": "codecatalyst",
         "jsonVersion": "1.1",
         "protocol": "rest-json",
         "serviceFullName": "Amazon CodeCatalyst",
         "serviceId": "CodeCatalyst",
@@ -115,14 +115,50 @@
                 "shape": "CreateProjectRequest"
             },
             "name": "CreateProject",
             "output": {
                 "shape": "CreateProjectResponse"
             }
         },
+        "CreateSourceRepository": {
+            "documentation": "<p>Creates an empty Git-based source repository in a specified project. The repository is created with an initial empty commit with a default branch named <code>main</code>.</p>",
+            "errors": [
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                }
+            ],
+            "http": {
+                "method": "PUT",
+                "requestUri": "/v1/spaces/{spaceName}/projects/{projectName}/sourceRepositories/{name}",
+                "responseCode": 201
+            },
+            "idempotent": true,
+            "input": {
+                "shape": "CreateSourceRepositoryRequest"
+            },
+            "name": "CreateSourceRepository",
+            "output": {
+                "shape": "CreateSourceRepositoryResponse"
+            }
+        },
         "CreateSourceRepositoryBranch": {
             "documentation": "<p>Creates a branch in a specified source repository in Amazon CodeCatalyst. </p> <note> <p>This API only creates a branch in a source repository hosted in Amazon CodeCatalyst. You cannot use this API to create a branch in a linked repository.</p> </note>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
@@ -223,14 +259,122 @@
                 "shape": "DeleteDevEnvironmentRequest"
             },
             "name": "DeleteDevEnvironment",
             "output": {
                 "shape": "DeleteDevEnvironmentResponse"
             }
         },
+        "DeleteProject": {
+            "documentation": "<p>Deletes a project in a space.</p>",
+            "errors": [
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                }
+            ],
+            "http": {
+                "method": "DELETE",
+                "requestUri": "/v1/spaces/{spaceName}/projects/{name}",
+                "responseCode": 200
+            },
+            "idempotent": true,
+            "input": {
+                "shape": "DeleteProjectRequest"
+            },
+            "name": "DeleteProject",
+            "output": {
+                "shape": "DeleteProjectResponse"
+            }
+        },
+        "DeleteSourceRepository": {
+            "documentation": "<p>Deletes a source repository in Amazon CodeCatalyst. You cannot use this API to delete a linked repository. It can only be used to delete a Amazon CodeCatalyst source repository.</p>",
+            "errors": [
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                }
+            ],
+            "http": {
+                "method": "DELETE",
+                "requestUri": "/v1/spaces/{spaceName}/projects/{projectName}/sourceRepositories/{name}",
+                "responseCode": 200
+            },
+            "idempotent": true,
+            "input": {
+                "shape": "DeleteSourceRepositoryRequest"
+            },
+            "name": "DeleteSourceRepository",
+            "output": {
+                "shape": "DeleteSourceRepositoryResponse"
+            }
+        },
+        "DeleteSpace": {
+            "documentation": "<p>Deletes a space.</p> <important> <p>Deleting a space cannot be undone. Additionally, since space names must be unique across Amazon CodeCatalyst, you cannot reuse names of deleted spaces.</p> </important>",
+            "errors": [
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                }
+            ],
+            "http": {
+                "method": "DELETE",
+                "requestUri": "/v1/spaces/{name}",
+                "responseCode": 200
+            },
+            "idempotent": true,
+            "input": {
+                "shape": "DeleteSpaceRequest"
+            },
+            "name": "DeleteSpace",
+            "output": {
+                "shape": "DeleteSpaceResponse"
+            }
+        },
         "GetDevEnvironment": {
             "documentation": "<p>Returns information about a Dev Environment for a source repository in a project. Dev Environments are specific to the user who creates them.</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
@@ -293,14 +437,49 @@
                 "shape": "GetProjectRequest"
             },
             "name": "GetProject",
             "output": {
                 "shape": "GetProjectResponse"
             }
         },
+        "GetSourceRepository": {
+            "documentation": "<p>Returns information about a source repository.</p>",
+            "errors": [
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                }
+            ],
+            "http": {
+                "method": "GET",
+                "requestUri": "/v1/spaces/{spaceName}/projects/{projectName}/sourceRepositories/{name}",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "GetSourceRepositoryRequest"
+            },
+            "name": "GetSourceRepository",
+            "output": {
+                "shape": "GetSourceRepositoryResponse"
+            }
+        },
         "GetSourceRepositoryCloneUrls": {
             "documentation": "<p>Returns information about the URLs that can be used with a Git client to clone a source repository.</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
@@ -892,14 +1071,86 @@
                 "shape": "UpdateDevEnvironmentRequest"
             },
             "name": "UpdateDevEnvironment",
             "output": {
                 "shape": "UpdateDevEnvironmentResponse"
             }
         },
+        "UpdateProject": {
+            "documentation": "<p>Changes one or more values for a project.</p>",
+            "errors": [
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                }
+            ],
+            "http": {
+                "method": "PATCH",
+                "requestUri": "/v1/spaces/{spaceName}/projects/{name}",
+                "responseCode": 200
+            },
+            "idempotent": true,
+            "input": {
+                "shape": "UpdateProjectRequest"
+            },
+            "name": "UpdateProject",
+            "output": {
+                "shape": "UpdateProjectResponse"
+            }
+        },
+        "UpdateSpace": {
+            "documentation": "<p>Changes one or more values for a space.</p>",
+            "errors": [
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ConflictException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                }
+            ],
+            "http": {
+                "method": "PATCH",
+                "requestUri": "/v1/spaces/{name}",
+                "responseCode": 200
+            },
+            "idempotent": true,
+            "input": {
+                "shape": "UpdateSpaceRequest"
+            },
+            "name": "UpdateSpace",
+            "output": {
+                "shape": "UpdateSpaceResponse"
+            }
+        },
         "VerifySession": {
             "documentation": "<p>Verifies whether the calling user has a valid Amazon CodeCatalyst login and session. If successful, this returns the ID of the user in Amazon CodeCatalyst.</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
@@ -1077,15 +1328,15 @@
                     "shape": "CreateDevEnvironmentRequestAliasString"
                 },
                 "clientToken": {
                     "documentation": "<p>A user-specified idempotency token. Idempotency ensures that an API request completes only once. With an idempotent request, if the original request completes successfully, the subsequent retries return the result from the original successful request and have no additional effect.</p>",
                     "shape": "ClientToken"
                 },
                 "ides": {
-                    "documentation": "<p>Information about the integrated development environment (IDE) configured for a Dev Environment.</p> <note> <p>An IDE is required to create a Dev Environment. For Dev Environment creation, this field contains configuration information and must be provided.</p> </note>",
+                    "documentation": "<p>Information about the integrated development environment (IDE) configured for a Dev Environment.</p> <note> <p>An IDE is required to create a Dev Environment. For Dev Environment creation, this field contains configuration information and must be provided. </p> </note>",
                     "shape": "IdeConfigurationList"
                 },
                 "inactivityTimeoutMinutes": {
                     "documentation": "<p>The amount of time the Dev Environment will run without any activity detected before stopping, in minutes. Only whole integers are allowed. Dev Environments consume compute minutes when running.</p>",
                     "shape": "InactivityTimeoutMinutes"
                 },
                 "instanceType": {
@@ -1252,14 +1503,72 @@
                 "ref": {
                     "documentation": "<p>The Git reference name of the branch.</p>",
                     "shape": "SourceRepositoryBranchRefString"
                 }
             },
             "type": "structure"
         },
+        "CreateSourceRepositoryRequest": {
+            "members": {
+                "description": {
+                    "documentation": "<p>The description of the source repository.</p>",
+                    "shape": "SourceRepositoryDescriptionString"
+                },
+                "name": {
+                    "documentation": "<p>The name of the source repository. For more information about name requirements, see <a href=\"https://docs.aws.amazon.com/codecatalyst/latest/userguide/source-quotas.html\">Quotas for source repositories</a>.</p>",
+                    "location": "uri",
+                    "locationName": "name",
+                    "shape": "SourceRepositoryNameString"
+                },
+                "projectName": {
+                    "documentation": "<p>The name of the project in the space.</p>",
+                    "location": "uri",
+                    "locationName": "projectName",
+                    "shape": "NameString"
+                },
+                "spaceName": {
+                    "documentation": "<p>The name of the space.</p>",
+                    "location": "uri",
+                    "locationName": "spaceName",
+                    "shape": "NameString"
+                }
+            },
+            "required": [
+                "spaceName",
+                "projectName",
+                "name"
+            ],
+            "type": "structure"
+        },
+        "CreateSourceRepositoryResponse": {
+            "members": {
+                "description": {
+                    "documentation": "<p>The description of the source repository.</p>",
+                    "shape": "SourceRepositoryDescriptionString"
+                },
+                "name": {
+                    "documentation": "<p>The name of the source repository.</p>",
+                    "shape": "SourceRepositoryNameString"
+                },
+                "projectName": {
+                    "documentation": "<p>The name of the project in the space.</p>",
+                    "shape": "NameString"
+                },
+                "spaceName": {
+                    "documentation": "<p>The name of the space.</p>",
+                    "shape": "NameString"
+                }
+            },
+            "required": [
+                "spaceName",
+                "projectName",
+                "name"
+            ],
+            "type": "structure"
+        },
         "DeleteAccessTokenRequest": {
             "members": {
                 "id": {
                     "documentation": "<p>The ID of the personal access token to delete. You can find the IDs of all PATs associated with your Amazon Web Services Builder ID in a space by calling <a>ListAccessTokens</a>.</p>",
                     "location": "uri",
                     "locationName": "id",
                     "shape": "AccessTokenId"
@@ -1320,14 +1629,136 @@
             "required": [
                 "spaceName",
                 "projectName",
                 "id"
             ],
             "type": "structure"
         },
+        "DeleteProjectRequest": {
+            "members": {
+                "name": {
+                    "documentation": "<p>The name of the project in the space. To retrieve a list of project names, use <a>ListProjects</a>.</p>",
+                    "location": "uri",
+                    "locationName": "name",
+                    "shape": "NameString"
+                },
+                "spaceName": {
+                    "documentation": "<p>The name of the space.</p>",
+                    "location": "uri",
+                    "locationName": "spaceName",
+                    "shape": "NameString"
+                }
+            },
+            "required": [
+                "spaceName",
+                "name"
+            ],
+            "type": "structure"
+        },
+        "DeleteProjectResponse": {
+            "members": {
+                "displayName": {
+                    "documentation": "<p>The friendly name displayed to users of the project in Amazon CodeCatalyst.</p>",
+                    "shape": "String"
+                },
+                "name": {
+                    "documentation": "<p>The name of the project in the space.</p>",
+                    "shape": "NameString"
+                },
+                "spaceName": {
+                    "documentation": "<p>The name of the space.</p>",
+                    "shape": "NameString"
+                }
+            },
+            "required": [
+                "spaceName",
+                "name"
+            ],
+            "type": "structure"
+        },
+        "DeleteSourceRepositoryRequest": {
+            "members": {
+                "name": {
+                    "documentation": "<p>The name of the source repository.</p>",
+                    "location": "uri",
+                    "locationName": "name",
+                    "shape": "SourceRepositoryNameString"
+                },
+                "projectName": {
+                    "documentation": "<p>The name of the project in the space.</p>",
+                    "location": "uri",
+                    "locationName": "projectName",
+                    "shape": "NameString"
+                },
+                "spaceName": {
+                    "documentation": "<p>The name of the space.</p>",
+                    "location": "uri",
+                    "locationName": "spaceName",
+                    "shape": "NameString"
+                }
+            },
+            "required": [
+                "spaceName",
+                "projectName",
+                "name"
+            ],
+            "type": "structure"
+        },
+        "DeleteSourceRepositoryResponse": {
+            "members": {
+                "name": {
+                    "documentation": "<p>The name of the repository.</p>",
+                    "shape": "SourceRepositoryNameString"
+                },
+                "projectName": {
+                    "documentation": "<p>The name of the project in the space.</p>",
+                    "shape": "NameString"
+                },
+                "spaceName": {
+                    "documentation": "<p>The name of the space.</p>",
+                    "shape": "NameString"
+                }
+            },
+            "required": [
+                "spaceName",
+                "projectName",
+                "name"
+            ],
+            "type": "structure"
+        },
+        "DeleteSpaceRequest": {
+            "members": {
+                "name": {
+                    "documentation": "<p>The name of the space. To retrieve a list of space names, use <a>ListSpaces</a>.</p>",
+                    "location": "uri",
+                    "locationName": "name",
+                    "shape": "NameString"
+                }
+            },
+            "required": [
+                "name"
+            ],
+            "type": "structure"
+        },
+        "DeleteSpaceResponse": {
+            "members": {
+                "displayName": {
+                    "documentation": "<p>The friendly name of the space displayed to users of the space in Amazon CodeCatalyst.</p>",
+                    "shape": "String"
+                },
+                "name": {
+                    "documentation": "<p>The name of the space.</p>",
+                    "shape": "NameString"
+                }
+            },
+            "required": [
+                "name"
+            ],
+            "type": "structure"
+        },
         "DevEnvironmentAccessDetails": {
             "documentation": "<p>Information about connection details for a Dev Environment.</p>",
             "members": {
                 "streamUrl": {
                     "documentation": "<p>The URL used to send commands to and from the Dev Environment.</p>",
                     "shape": "SensitiveString"
                 },
@@ -1603,15 +2034,15 @@
                     "shape": "EventPayload"
                 },
                 "sourceIpAddress": {
                     "documentation": "<p>The IP address of the user whose actions are recorded in the event.</p>",
                     "shape": "String"
                 },
                 "userAgent": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The user agent whose actions are recorded in the event.</p>",
                     "shape": "String"
                 },
                 "userIdentity": {
                     "documentation": "<p>The system-generated unique ID of the user whose actions are recorded in the event.</p>",
                     "shape": "UserIdentity"
                 }
             },
@@ -1671,26 +2102,26 @@
         },
         "ExecuteCommandSessionConfigurationCommandString": {
             "max": 255,
             "min": 1,
             "type": "string"
         },
         "Filter": {
-            "documentation": "<p/>",
+            "documentation": "<p>Information about a filter used to limit results of a query.</p>",
             "members": {
                 "comparisonOperator": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The operator used to compare the fields.</p>",
                     "shape": "String"
                 },
                 "key": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>A key that can be used to sort results.</p>",
                     "shape": "String"
                 },
                 "values": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The values of the key.</p>",
                     "shape": "StringList"
                 }
             },
             "required": [
                 "key",
                 "values"
             ],
@@ -1896,14 +2327,78 @@
                 }
             },
             "required": [
                 "https"
             ],
             "type": "structure"
         },
+        "GetSourceRepositoryRequest": {
+            "members": {
+                "name": {
+                    "documentation": "<p>The name of the source repository.</p>",
+                    "location": "uri",
+                    "locationName": "name",
+                    "shape": "SourceRepositoryNameString"
+                },
+                "projectName": {
+                    "documentation": "<p>The name of the project in the space.</p>",
+                    "location": "uri",
+                    "locationName": "projectName",
+                    "shape": "NameString"
+                },
+                "spaceName": {
+                    "documentation": "<p>The name of the space.</p>",
+                    "location": "uri",
+                    "locationName": "spaceName",
+                    "shape": "NameString"
+                }
+            },
+            "required": [
+                "spaceName",
+                "projectName",
+                "name"
+            ],
+            "type": "structure"
+        },
+        "GetSourceRepositoryResponse": {
+            "members": {
+                "createdTime": {
+                    "documentation": "<p>The time the source repository was created, in coordinated universal time (UTC) timestamp format as specified in <a href=\"https://www.rfc-editor.org/rfc/rfc3339#section-5.6\">RFC 3339</a>.</p>",
+                    "shape": "Timestamp"
+                },
+                "description": {
+                    "documentation": "<p>The description of the source repository.</p>",
+                    "shape": "SourceRepositoryDescriptionString"
+                },
+                "lastUpdatedTime": {
+                    "documentation": "<p>The time the source repository was last updated, in coordinated universal time (UTC) timestamp format as specified in <a href=\"https://www.rfc-editor.org/rfc/rfc3339#section-5.6\">RFC 3339</a>.</p>",
+                    "shape": "Timestamp"
+                },
+                "name": {
+                    "documentation": "<p>The name of the source repository.</p>",
+                    "shape": "SourceRepositoryNameString"
+                },
+                "projectName": {
+                    "documentation": "<p>The name of the project in the space.</p>",
+                    "shape": "NameString"
+                },
+                "spaceName": {
+                    "documentation": "<p>The name of the space.</p>",
+                    "shape": "NameString"
+                }
+            },
+            "required": [
+                "spaceName",
+                "projectName",
+                "name",
+                "lastUpdatedTime",
+                "createdTime"
+            ],
+            "type": "structure"
+        },
         "GetSpaceRequest": {
             "members": {
                 "name": {
                     "documentation": "<p>The name of the space.</p>",
                     "location": "uri",
                     "locationName": "name",
                     "shape": "NameString"
@@ -2666,15 +3161,15 @@
                     "shape": "ComparisonOperator"
                 },
                 "key": {
                     "documentation": "<p>A key that can be used to sort results.</p>",
                     "shape": "FilterKey"
                 },
                 "values": {
-                    "documentation": "<p>The value of the key.</p>",
+                    "documentation": "<p>The values of the key.</p>",
                     "shape": "StringList"
                 }
             },
             "required": [
                 "key",
                 "values"
             ],
@@ -2801,14 +3296,20 @@
         },
         "SourceRepositoryNameString": {
             "max": 100,
             "min": 1,
             "pattern": "(?!.*[.]git$)[\\w\\-.]*",
             "type": "string"
         },
+        "SpaceDescription": {
+            "max": 200,
+            "min": 0,
+            "pattern": "[a-zA-Z0-9]+(?:[-_a-zA-Z0-9.,;:/\\+=?&$%    ])*",
+            "type": "string"
+        },
         "SpaceSummaries": {
             "member": {
                 "shape": "SpaceSummary"
             },
             "type": "list"
         },
         "SpaceSummary": {
@@ -3238,23 +3739,104 @@
         },
         "UpdateDevEnvironmentResponseAliasString": {
             "max": 128,
             "min": 1,
             "pattern": "[a-zA-Z0-9]+(?:[-_\\.][a-zA-Z0-9]+)*",
             "type": "string"
         },
+        "UpdateProjectRequest": {
+            "members": {
+                "description": {
+                    "documentation": "<p>The description of the project.</p>",
+                    "shape": "ProjectDescription"
+                },
+                "name": {
+                    "documentation": "<p>The name of the project.</p>",
+                    "location": "uri",
+                    "locationName": "name",
+                    "shape": "NameString"
+                },
+                "spaceName": {
+                    "documentation": "<p>The name of the space.</p>",
+                    "location": "uri",
+                    "locationName": "spaceName",
+                    "shape": "NameString"
+                }
+            },
+            "required": [
+                "spaceName",
+                "name"
+            ],
+            "type": "structure"
+        },
+        "UpdateProjectResponse": {
+            "members": {
+                "description": {
+                    "documentation": "<p>The description of the project.</p>",
+                    "shape": "String"
+                },
+                "displayName": {
+                    "documentation": "<p>The friendly name of the project displayed to users in Amazon CodeCatalyst.</p>",
+                    "shape": "String"
+                },
+                "name": {
+                    "documentation": "<p>The name of the project.</p>",
+                    "shape": "NameString"
+                },
+                "spaceName": {
+                    "documentation": "<p>The name of the space.</p>",
+                    "shape": "NameString"
+                }
+            },
+            "type": "structure"
+        },
+        "UpdateSpaceRequest": {
+            "members": {
+                "description": {
+                    "documentation": "<p>The description of the space.</p>",
+                    "shape": "SpaceDescription"
+                },
+                "name": {
+                    "documentation": "<p>The name of the space.</p>",
+                    "location": "uri",
+                    "locationName": "name",
+                    "shape": "NameString"
+                }
+            },
+            "required": [
+                "name"
+            ],
+            "type": "structure"
+        },
+        "UpdateSpaceResponse": {
+            "members": {
+                "description": {
+                    "documentation": "<p>The description of the space.</p>",
+                    "shape": "String"
+                },
+                "displayName": {
+                    "documentation": "<p>The friendly name of the space displayed to users in Amazon CodeCatalyst.</p>",
+                    "shape": "String"
+                },
+                "name": {
+                    "documentation": "<p>The name of the space.</p>",
+                    "shape": "NameString"
+                }
+            },
+            "type": "structure"
+        },
         "UserIdentity": {
             "documentation": "<p>Information about a user whose activity is recorded in an event for a space.</p>",
             "members": {
                 "awsAccountId": {
                     "documentation": "<p>The Amazon Web Services account number of the user in Amazon Web Services, if any.</p>",
                     "shape": "String"
                 },
                 "principalId": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>The ID of the Amazon CodeCatalyst service principal.</p>",
                     "shape": "String"
                 },
                 "userName": {
                     "documentation": "<p>The display name of the user in Amazon CodeCatalyst.</p>",
                     "shape": "String"
                 },
                 "userType": {
```

### Comparing `botocore-a-la-carte-codecatalyst-1.31.6/botocore_a_la_carte_codecatalyst.egg-info/PKG-INFO` & `botocore-a-la-carte-codecatalyst-1.31.8/botocore_a_la_carte_codecatalyst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-codecatalyst
-Version: 1.31.6
+Version: 1.31.8
 Summary: codecatalyst data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-codecatalyst-1.31.6/setup.py` & `botocore-a-la-carte-codecatalyst-1.31.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-codecatalyst',
-    version="1.31.6",
+    version="1.31.8",
     description='codecatalyst data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/codecatalyst/*/*.json'],
```

