# Comparing `tmp/cloud_data_connector-1.0.1.tar.gz` & `tmp/cloud_data_connector-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_data_connector-1.0.1.tar", last modified: Fri Jun 30 19:47:14 2023, max compression
+gzip compressed data, was "cloud_data_connector-1.0.2.tar", last modified: Fri Jul 21 20:53:13 2023, max compression
```

## Comparing `cloud_data_connector-1.0.1.tar` & `cloud_data_connector-1.0.2.tar`

### file list

```diff
@@ -1,42 +1,39 @@
-drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-06-30 19:47:14.594604 cloud_data_connector-1.0.1/
--rw-r--r--   0 mapineda (12146662) ansible   (1005)    11357 2023-06-30 19:44:30.000000 cloud_data_connector-1.0.1/LICENSE
--rw-r--r--   0 mapineda (12146662) ansible   (1005)    31670 2023-06-30 19:47:14.594604 cloud_data_connector-1.0.1/PKG-INFO
--rw-r--r--   0 mapineda (12146662) ansible   (1005)    18199 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/README.md
-drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-06-30 19:47:14.590604 cloud_data_connector-1.0.1/cloud_data_connector.egg-info/
--rw-r--r--   0 mapineda (12146662) ansible   (1005)    31670 2023-06-30 19:47:13.000000 cloud_data_connector-1.0.1/cloud_data_connector.egg-info/PKG-INFO
--rw-r--r--   0 mapineda (12146662) ansible   (1005)     1044 2023-06-30 19:47:14.000000 cloud_data_connector-1.0.1/cloud_data_connector.egg-info/SOURCES.txt
--rw-r--r--   0 mapineda (12146662) ansible   (1005)        1 2023-06-30 19:47:13.000000 cloud_data_connector-1.0.1/cloud_data_connector.egg-info/dependency_links.txt
--rw-r--r--   0 mapineda (12146662) ansible   (1005)      304 2023-06-30 19:47:13.000000 cloud_data_connector-1.0.1/cloud_data_connector.egg-info/requires.txt
--rw-r--r--   0 mapineda (12146662) ansible   (1005)       15 2023-06-30 19:47:13.000000 cloud_data_connector-1.0.1/cloud_data_connector.egg-info/top_level.txt
-drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-06-30 19:47:14.590604 cloud_data_connector-1.0.1/data_connector/
--rw-r--r--   0 mapineda (12146662) ansible   (1005)        0 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/__init__.py
-drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-06-30 19:47:14.590604 cloud_data_connector-1.0.1/data_connector/aws/
--rw-r--r--   0 mapineda (12146662) ansible   (1005)     6181 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/aws/README.md
--rw-r--r--   0 mapineda (12146662) ansible   (1005)      777 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/aws/__init__.py
--rw-r--r--   0 mapineda (12146662) ansible   (1005)     1604 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/aws/connector.py
--rw-r--r--   0 mapineda (12146662) ansible   (1005)     2966 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/aws/downloader.py
--rw-r--r--   0 mapineda (12146662) ansible   (1005)     2196 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/aws/uploader.py
-drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-06-30 19:47:14.594604 cloud_data_connector-1.0.1/data_connector/azure/
--rw-r--r--   0 mapineda (12146662) ansible   (1005)      670 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/azure/AzureML.md
--rw-r--r--   0 mapineda (12146662) ansible   (1005)     2483 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/azure/README.md
--rw-r--r--   0 mapineda (12146662) ansible   (1005)      942 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/azure/__init__.py
--rw-r--r--   0 mapineda (12146662) ansible   (1005)     3640 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/azure/connector.py
--rw-r--r--   0 mapineda (12146662) ansible   (1005)     1756 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/azure/connector_object.py
--rw-r--r--   0 mapineda (12146662) ansible   (1005)     3326 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/azure/downloader.py
--rw-r--r--   0 mapineda (12146662) ansible   (1005)     2173 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/azure/ml_uploader.py
--rw-r--r--   0 mapineda (12146662) ansible   (1005)     4520 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/azure/uploader.py
-drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-06-30 19:47:14.594604 cloud_data_connector-1.0.1/data_connector/gcp/
--rw-r--r--   0 mapineda (12146662) ansible   (1005)    10397 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/gcp/README.md
--rw-r--r--   0 mapineda (12146662) ansible   (1005)      813 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/gcp/__init__.py
--rw-r--r--   0 mapineda (12146662) ansible   (1005)     7435 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/gcp/connector.py
--rw-r--r--   0 mapineda (12146662) ansible   (1005)     2921 2023-06-30 19:43:49.000000 cloud_data_connector-1.0.1/data_connector/gcp/downloader.py
--rw-r--r--   0 mapineda (12146662) ansible   (1005)     7468 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/gcp/query.py
--rw-r--r--   0 mapineda (12146662) ansible   (1005)     1736 2023-06-30 19:43:49.000000 cloud_data_connector-1.0.1/data_connector/gcp/uploader.py
-drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-06-30 19:47:14.594604 cloud_data_connector-1.0.1/data_connector/int/
--rw-r--r--   0 mapineda (12146662) ansible   (1005)        0 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/int/__init__.py
--rw-r--r--   0 mapineda (12146662) ansible   (1005)      971 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/int/int_connector.py
--rw-r--r--   0 mapineda (12146662) ansible   (1005)      912 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/int/int_downloader.py
--rw-r--r--   0 mapineda (12146662) ansible   (1005)      990 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/int/int_uploader.py
--rw-r--r--   0 mapineda (12146662) ansible   (1005)     1223 2023-06-30 19:44:50.000000 cloud_data_connector-1.0.1/pyproject.toml
--rw-r--r--   0 mapineda (12146662) ansible   (1005)      405 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/security.md
--rw-r--r--   0 mapineda (12146662) ansible   (1005)       38 2023-06-30 19:47:14.594604 cloud_data_connector-1.0.1/setup.cfg
+drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-07-21 20:53:13.002604 cloud_data_connector-1.0.2/
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)    11348 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/LICENSE
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)    32047 2023-07-21 20:53:13.002604 cloud_data_connector-1.0.2/PKG-INFO
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)    18577 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/README.md
+drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-07-21 20:53:12.998603 cloud_data_connector-1.0.2/cloud_data_connector/
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)        0 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/__init__.py
+drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-07-21 20:53:12.998603 cloud_data_connector-1.0.2/cloud_data_connector/aws/
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     6259 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/aws/README.md
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)      777 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/aws/__init__.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     1610 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/aws/connector.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     2972 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/aws/downloader.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     2202 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/aws/uploader.py
+drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-07-21 20:53:13.002604 cloud_data_connector-1.0.2/cloud_data_connector/azure/
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)       38 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/azure/.gitattributes
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)      670 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/azure/AzureML.md
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     2507 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/azure/README.md
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)      942 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/azure/__init__.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     3646 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/azure/connector.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     1756 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/azure/connector_object.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     3332 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/azure/downloader.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     2173 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/azure/ml_uploader.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     4526 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/azure/uploader.py
+drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-07-21 20:53:13.002604 cloud_data_connector-1.0.2/cloud_data_connector/gcp/
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)    10701 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/gcp/README.md
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)      813 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/gcp/__init__.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     7441 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/gcp/connector.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     2927 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/gcp/downloader.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     7468 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/gcp/query.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     1736 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/gcp/uploader.py
+drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-07-21 20:53:13.002604 cloud_data_connector-1.0.2/cloud_data_connector/int/
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)        0 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/int/__init__.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)      971 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/int/int_connector.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)      912 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/int/int_downloader.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)      990 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/cloud_data_connector/int/int_uploader.py
+drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-07-21 20:53:13.002604 cloud_data_connector-1.0.2/cloud_data_connector.egg-info/
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     1011 2023-07-21 20:53:12.000000 cloud_data_connector-1.0.2/cloud_data_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     1235 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/pyproject.toml
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)      405 2023-07-21 18:54:35.000000 cloud_data_connector-1.0.2/security.md
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)       38 2023-07-21 20:53:13.002604 cloud_data_connector-1.0.2/setup.cfg
```

### Comparing `cloud_data_connector-1.0.1/LICENSE` & `cloud_data_connector-1.0.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -183,20 +183,20 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2023 Intel Corporation
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

### Comparing `cloud_data_connector-1.0.1/PKG-INFO` & `cloud_data_connector-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud_data_connector
-Version: 1.0.1
+Version: 1.0.2
 Summary: Intel's cloud data connector
 Author-email: IntelAI <IntelAI@intel.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -188,100 +188,101 @@
               replaced with your own identifying information. (Don't include
               the brackets!)  The text should be enclosed in the appropriate
               comment syntax for the file format. We also recommend that a
               file or class name and description of purpose be included on the
               same "printed page" as the copyright notice for easier
               identification within third-party archives.
         
-           Copyright [yyyy] [name of copyright owner]
+           Copyright 2023 Intel Corporation
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
+        
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Cloud Data Connector
 
 [![Intel: AI](https://img.shields.io/badge/intel-AI-0071C5)](https://www.intel.com/content/www/us/en/developer/topic-technology/artificial-intelligence/overview.html)
-[![Python](https://img.shields.io/badge/Python-3.8/3.9/3.10-green)](https://www.intel.com/content/www/us/en/developer/topic-technology/artificial-intelligence/overview.html)
+[![Python](https://img.shields.io/badge/Python-3.9/3.10-green)](https://www.intel.com/content/www/us/en/developer/topic-technology/artificial-intelligence/overview.html)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 [![security: SNYK](https://img.shields.io/badge/Security-SNYK-yellow)](https://github.com/PyCQA/bandit)
 [![security: BDBA](https://img.shields.io/badge/Security-BDBA-yellow)](https://github.com/PyCQA/bandit)
 [![security: Checkmarks](https://img.shields.io/badge/Security-Checkmarks-yellow)](https://github.com/PyCQA/bandit)
 
 
 _____
 ## Overview
 ---
-data_connector is a tool to connect to AzureML, Azure blob, GCP storage, GCP Big Query  and AWS storage S3. 
+**Cloud data connector** is a tool to connect to AzureML, Azure blob, GCP storage, GCP Big Query  and AWS storage S3. 
 The goal is provide all cloud managers in one place and provide documentation for an easy integration.
 
-For more details, visit the [Data Connector](https://github.com/IntelAI/models/tree/master/datasets/data_connector) GitHub repository.
+For more details, visit the [Cloud Data Connector](https://github.com/IntelAI/models/tree/master/datasets/cloud_data_connector) GitHub repository.
 <br/><br/>
 
 ## Hardware Requirements
 ---
 The hardware should comply with the same requirements that the cloud service.
 <br/><br/>
 
 ## How it Works
 ---
 The package contains the following modules:
 
 | Package Components   |
 | -------------------- |
-| data_connector.aws   |
-| data_connector.gcp   |
-| data_connector.azure |
+| cloud_data_connector.aws   |
+| cloud_data_connector.gcp   |
+| cloud_data_connector.azure |
 
 Each module is capable of connect, download and upload operation to it-s corresponding cloud service.
 <br/><br/>
 
-## Getting Started with data_connector
+## Getting Started with **Cloud Data Connector**
 ---
 
 It is strongly recommended to use a virtual environment to ensure proper operation, example:
 ```bash
 conda create -n venv python=3.10 -c conda-forge
 conda activate venv
 ```
 
 You can install the package with:
 ```bash
 python -m pip install cloud-data-connector
 ```
 
 Please follow module specific documentation for use case, hands-examples.
-1. data_connector/azure/README.md
-2. data_connector/azure/AzureML.md
-3. data_connector/aws/README.md
-4. data_connector/gcp/README.md
+1. cloud_data_connector/azure/README.md
+2. cloud_data_connector/azure/AzureML.md
+3. cloud_data_connector/aws/README.md
+4. cloud_data_connector/gcp/README.md
 <br/><br/>
 
-## Getting Started with data_connector.azure
+## Getting Started with **Cloud Data Connector Azure**
 ---
 
 ### Abstract
-Intel's [Data Connector](../../README.md) AzureML tool allows users follow a simple flow to work locally on model training and upload jobs to AzureML configuring a job, workflow, upload models or training scripts.
+Intel's [Cloud Data Connector](https://github.com/IntelAI/models/tree/master/datasets/cloud_data_connector/README.md) AzureML tool allows users follow a simple flow to work locally on model training and upload jobs to AzureML configuring a job, workflow, upload models or training scripts.
 Data connector for Azure is a tool to connect to Azure Blob and Azure Machine Learning tools.
 
 ### Requirements
 This tool requires an account on Azure Cloud and an Azure ML worskspace active.
 * Azure Account 
 * Access to AzureML
 * [Create a workspace of Azure ML](https://learn.microsoft.com/en-us/azure/machine-learning/quickstart-create-resources#create-the-workspace)
@@ -303,15 +304,15 @@
 Azure ML is a service to train models connecting data sources and deploy it in production using Azure infrastructure.
 
 Data connector provides a tool to connect to Azure ML workspaces and upload configurations for this proposes.
 
 ### Sample
 **Blob Connector**
 ```python
-    from data_connector.azure import connect
+    from cloud_data_connector.azure import connect
     connection_string_sample = """
         DefaultEndpointsProtocol=http;
         AccountName=<YOUR_ACCOUNT_NAME>;
         AccountKey=<YOUR_ACCOUNT_KEY>;
         BlobEndpoint=http://127.0.0.1:10000/
         devstoreaccount1;
         QueueEndpoint=http://127.0.0.1:10001/
@@ -335,39 +336,39 @@
 >az storage account show-connection-string --name <storageAccount> 
 ```
 * This process not works for WSL 
 
 
 **Blob upload**
 ```python
-    from data_connector.azure import Uploader
+    from cloud_data_connector.azure import Uploader
 
     uploader = Uploader(connector= connector)
     uploader.upload(
         'sample.txt',
         blob_container_name='sample_container'
     )
 ```
 
 **Blob downloader**
 ```python
-    from data_connector.azure import Downloader
+    from cloud_data_connector.azure import Downloader
 
     downloader = Downloader(connector=connector)
     downloader.download()
 ```
-[See sample Here](https://github.com/IntelAI/models/blob/master/datasets/data_connector/samples/azure/blob_sample.py)
+[See sample Here](https://github.com/IntelAI/models/blob/master/datasets/cloud_data_connector/samples/azure/blob_sample.py)
 <br/><br/>
 
 
-## Getting Started with data_connector.aws
+## Getting Started with **Cloud Data Connector AWS**
 ---
-### Data Connector AWS S3 
+### Cloud Data Connector AWS S3 
 
-Data Connector for AWS S3 allows you to connect to S3 buckets and list contents, download and upload files.
+Cloud Data Connector for AWS S3 allows you to connect to S3 buckets and list contents, download and upload files.
 
 ### Access S3 buckets
 
 To access S3 buckets, you will need to sign up for an AWS account and create access keys. 
 
 Access keys consist of an access key ID and secret access key, which are used to sign programmatic requests that you make to AWS.
 
@@ -393,15 +394,15 @@
 You can add more configuration settings listed [here](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html#using-environment-variables). For example, you can set the `AWS_SESSION_TOKEN`, it is only needed when you are using temporary credentials.
 
 ### Usage
 
 You need to import the DataConnector class.
 
 ```python
-from data_connector.aws.connector import Connector
+from cloud_data_connector.aws.connector import Connector
 ```
 
 Connector class has the method connect(), it creates an AWS S3 object, by default the function will create a S3 connector using the credentials saved in your environment variables.
 
 ```python
 connector = Connector()
 ```
@@ -411,81 +412,81 @@
 ```python
 conection_object = connector.connect()
 ```
 
 Import the Downloader class and use the connection object returned by connect() function.
 
 ```python
-from data_connector.aws.downloader import Downloader
+from cloud_data_connector.aws.downloader import Downloader
 
 downloader = Downloader(conection_object)
 ```
 
 The Downloader class has two methods:
 
 - list_blobs(container_obj): The function to get a list of the objects in a bucket.
 - download(container_obj, data_file, destiny): The function to download a file from a S3 bucket.
 
 A first step with buckets is to list their content using the `list_blobs(container_obj)` method. Specify the next parameter.
 
 - container_obj: The bucket name to list.
 
 ```python
-from data_connector.aws.downloader import Downloader
+from cloud_data_connector.aws.downloader import Downloader
 
 downloader = Downloader(conection_object)
 
 list_blobs = downloader.list_blobs('MY_BUCKET_NAME')
 print(list_blobs)
 ```
 
 To download a file use the `download(container_obj, data_file, destiny)` method and specify the next parameters.
 
 - container_obj: The name of the bucket to download from.
 - data_file: The name of the file to download from.
 - destiny: The path to the file to download to.
 
 ```python
-from data_connector.aws.downloader import Downloader
+from cloud_data_connector.aws.downloader import Downloader
 
 downloader = Downloader(conection_object)
 file_name = "path/to_file.csv"
 downloader.download(bucket_name, file_name, 'path/to_destiny.csv')
 ```
 
 You can import an Uploader class and use the upload method to send a file from you local machine to a bucket. You need to add the connector object to Uploader constructor.
 
 ```python
-from data_connector.aws.uploader import Uploader
-from data_connector.aws.connector import Connector
+from cloud_data_connector.aws.uploader import Uploader
+from cloud_data_connector.aws.connector import Connector
 
 connector = Connector()
 conection_object = connector.connect()
 uploader = Uploader(conection_object)
 
 ```
 Specify the next parameters in upload function.
 
 - container_obj: The name of the bucket to upload to.
 - data_file: The path to the file to upload.
 - object_name: The name of the file to upload to.
 
 ```python
-from data_connector.aws.uploader import Uploader
+from cloud_data_connector.aws.uploader import Uploader
 
 uploader = Uploader(conection_object)
 uploader.upload(bucket_name, 'path/to_local_file.csv', 'path/to_object_name.csv')
 ```
 
 ### List objects in a bucket
 
 ```python
 # import the dataconnector package
-from data_connector.aws.connector import Connector
-from data_connector.aws.downloader import Downloader
+from cloud_data_connector.aws.connector import Connector
+from cloud_data_connector.aws.downloader import Downloader
 
 # specify a S3 bucket name
 bucket_name = 'MY_BUCKET_NAME'
 # create a connector
 connector = Connector()
 # connect to aws using default AWS access keys
 # connect() method uses the configurations settings for AWS account
@@ -500,16 +501,16 @@
 
 ```
 
 ### Download a file
 
 ```python
 # import the dataconnector package
-from data_connector.aws.connector import Connector
-from data_connector.aws.downloader import Downloader
+from cloud_data_connector.aws.connector import Connector
+from cloud_data_connector.aws.downloader import Downloader
 
 # specify a S3 bucket name
 bucket_name = 'MY_BUCKET_NAME'
 # create a connector
 connector = Connector()
 # connect to aws using default aws access keys
 conection_object = connector.connect()
@@ -522,16 +523,16 @@
 downloader.download(bucket_name, file_name, 'path/to_destiny.csv')
 ```
 
 ### Upload a file
 
 ```python
 # import dataconnector package
-from data_connector.aws.connector import Connector
-from data_connector.aws.uploader import Uploader
+from cloud_data_connector.aws.connector import Connector
+from cloud_data_connector.aws.uploader import Uploader
 
 # specify a S3 bucket name
 bucket_name = 'MY_BUCKET_NAME'
 # create a connector
 connector = Connector()
 # connect to aws using default aws access keys
 conection_object = connector.connect()
@@ -539,42 +540,42 @@
 # create a uploader object using a connection object
 uploader = Uploader(conection_object)
 # upload a file
 uploader.upload(bucket_name, 'path/to_local_file.csv', 'path/to_object_name.csv')
 ```
 <br/><br/>
 
-## Getting Started with data_connector.gcp
+## Getting Started with **Cloud Data Connector GCP**
 ---
 ### GCP Permissions
 To enable permissions in GCP to use Storage and BigQuery, from the the left side navigation menu, inside Google Cloud, go to "APIs & Services > Library" and search and enable:
 - Cloud Storage
 - Google Cloud Storage JSON API
 - BigQuery API
 
 You need one of two authentication tools: Oauth or Service Account
 ### Oauth
 To enable oauth2, from the the left side navigation menu go to "APIs & Services > Credentials" and select "+ CREATE CREDENTIALS". From the three available options select "OAuth client ID". When creating an ID it is necessary to provide an "Application type" and a Name, which for this case select "Desktop app" for  "Application type" and type a name of your preference. Once the ID has been created a window will pop with the Client ID and Secret; select "DOWNLOAD JSON" and store the JSON file in a secure place.
 ### Service Account
-To enable a service account, from the left side navigation menu go to "APIs & Services > Credentials" and select "+ CREATE CREDENTIALS". From the three available options select "Service account". In "Service account details" provide a service account name and ID and select "CREATE AND CONTINUE". In "Grant this service account access to project" select roles: "Cloud Storage -> Storage Admin" and "BigQuery -> BigQuery Admin". After defining roles press "Done". Go to the created service account by selecting the service e-mail in "Service Accounts" and go to "KEYS", from there you can create a new key for the account(it will provide a JSON file).
+To enable a service account, from the left side navigation menu go to "APIs & Services > Credentials" and select "+ CREATE CREDENTIALS". From the three available options select "Service account". In "Service account details" provide a service account name and ID and select "CREATE AND CONTINUE". In "Grant this service account access to project" select roles: "Cloud Storage > Storage Admin" and "BigQuery > BigQuery Admin". After defining roles press "Done". Go to the created service account by selecting the service e-mail in "Service Accounts" and go to "KEYS", from there you can create a new key for the account(it will provide a JSON file).
 
 ### Installing Into Docker Container
 To be able to run data connector inside a Docker container execute the following command changing options as needed:
 ```bash
 docker run  -it  --name <container_name> --net=host -v <path to frameworks.ai.models.intel-mode.data-connector>:/workspace/model-zoo --env HTTPS_PROXY=$HTTPS_PROXY --env no_proxy=$no_proxy --env HTTP_PROXY=$HTTP_PROXY --env http_proxy=$http_proxy  --entrypoint bash conda/miniconda3:latest
 ```
 
 Inside the docker container set source to activate conda:
 ```bash
 source /usr/local/bin/activate
 ```
 To install requirements.txt file, first a conda environment must be created:
 ```bash
-conda create -n data_connector python=3.9 -y && \
-conda activate data_connector
+conda create -n cloud_data_connector python=3.9 -y && \
+conda activate cloud_data_connector
 ```
 To be able to run the GCP part of the connector, GCP CLI must be [installed](https://cloud.google.com/sdk/docs/install). The easy way to install the CLI repository is by running the following commands inside the container:
 ```bash
 apt-get update && \
 apt-get install apt-transport-https ca-certificates gnupg curl gpg -y && \
 echo "deb [signed-by=/usr/share/keyrings/cloud.google.gpg] http://packages.cloud.google.com/apt cloud-sdk main" | tee -a /etc/apt/sources.list.d/google-cloud-sdk.list && curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | apt-key --keyring /usr/share/keyrings/cloud.google.gpg  add - && apt-get update -y && apt-get install google-cloud-cli -y
 ```
@@ -592,53 +593,53 @@
 
 To provide access for the libraries to oauth run:
 ```bash
 gcloud auth application-default login
 ```
 Open the provided link in a web browser. GCP will ask for permissions to access the account; allow the permissions and copy the provided verification code in gcloud CLI.
 
-Go to data_connector directory, upgrade pip packages and install requirements.txt:
+Go to cloud_data_connector directory, upgrade pip packages and install requirements.txt:
 ```bash
-cd /workspace/model-zoo/data_connector
+cd /workspace/model-zoo/cloud_data_connector
 pip install --upgrade pip wheel setuptools
-pip install -r data_connector/gcp/requirements.txt 
+pip install -r cloud_data_connector/gcp/requirements.txt 
 ```
 
 ### Running Code Samples
 To run code portions inside a container and VS code the port to be used by OAuth must be added to the list of forwarded ports. Open OUTPUT terminal (Ctrl + Shift + U), go to PORTS and select "Add Port".
 
-To provide the JSON key obtained for OAuth in Google Cloud, the file content must be assigned to the 'CLIENT_SECRETS' environment variable. Also it can be obtained from a ".env" file that contains the variable. To use it from a ".env" file "python-dotenv" must be installed and the file must be in a location were "load_dotenv()" can find it. dotenv can find ".env" file inside the directory where a script is being executed, e.g. for the samples provided below you can add ".env" file into <base_path_to_model_zoo>/data_connector/data_connector/samples/gcp/ directory.
+To provide the JSON key obtained for OAuth in Google Cloud, the file content must be assigned to the 'CLIENT_SECRETS' environment variable. Also it can be obtained from a ".env" file that contains the variable. To use it from a ".env" file "python-dotenv" must be installed and the file must be in a location were "load_dotenv()" can find it. dotenv can find ".env" file inside the directory where a script is being executed, e.g. for the samples provided below you can add ".env" file into ```<base_path_to_model_zoo>/cloud_data_connector/cloud_data_connector/samples/gcp/``` directory.
 
 ```bash
 pip install python-dotenv
 ```
 To provide the JSON key obtained for the service account, the file path must be provided to the sample scripts if access to Storage or BigCloud is going to be made through service account.
 
 To test GCP Storage a bucket must be created. Go to "Cloud Storage > Buckets" and select "Create". There you need to provide several  options to create a bucket (for the example the name of the bucket will be "dataconnector_data_bucket"), for the following example the default values can be used.
 
-To test GCP Storage there is a script located in <base_path_to_model_zoo>/data_connector/data_connector/samples/gcp/storage.py. To run it execute from the base path of data connector for OAuth:
+To test GCP Storage there is a script located in ```<base_path_to_model_zoo>/cloud_data_connector/cloud_data_connector/samples/gcp/storage.py```. To run it execute from the base path of data connector for OAuth:
 ```bash
 python -m samples.gcp.storage -o
 ```
 For service account:
 ```bash
 python -m samples.gcp.storage -p <project_name> -c <credentials_path>
 ```
 User must provide the project name using flag (-p) and the local path to the JSON file with the credentials (-c).
 
-To test GCP BigQuery there is a script located in <base_path_to_model_zoo>/data_connector/data_connector/samples/gcp/bigquery.py. To run it execute from the base path of data connector for OAuth:
+To test GCP BigQuery there is a script located in ```<base_path_to_model_zoo>/cloud_data_connector/cloud_data_connector/samples/gcp/bigquery.py```. To run it execute from the base path of data connector for OAuth:
 ```bash
 python -m samples.gcp.bigquery -o
 ```
 For service account:
 ```bash
 python -m samples.gcp.bigquery -p <project_name> -c <credentials_path>
 ```
 User must provide the project name using flag (-p) and the local path to the JSON file with the credentials (-c).
 <br/><br/>
 
 
 ## Support
 ---
 If you have questions or issues about this package, contact the [Support Team](mailto:IntelAI@intel.com).
-data_connector has an Apache license, as found in the [LICENSE](https://www.apache.org/licenses/LICENSE-2.0) file.
+Cloud Data Connector has an Apache license, as found in the [LICENSE](https://www.apache.org/licenses/LICENSE-2.0) file.
 Dependencies versions higher than currently implemented ones are in beta and should be used with caution.
```

### Comparing `cloud_data_connector-1.0.1/README.md` & `cloud_data_connector-1.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 # Cloud Data Connector
 
 [![Intel: AI](https://img.shields.io/badge/intel-AI-0071C5)](https://www.intel.com/content/www/us/en/developer/topic-technology/artificial-intelligence/overview.html)
-[![Python](https://img.shields.io/badge/Python-3.8/3.9/3.10-green)](https://www.intel.com/content/www/us/en/developer/topic-technology/artificial-intelligence/overview.html)
+[![Python](https://img.shields.io/badge/Python-3.9/3.10-green)](https://www.intel.com/content/www/us/en/developer/topic-technology/artificial-intelligence/overview.html)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 [![security: SNYK](https://img.shields.io/badge/Security-SNYK-yellow)](https://github.com/PyCQA/bandit)
 [![security: BDBA](https://img.shields.io/badge/Security-BDBA-yellow)](https://github.com/PyCQA/bandit)
 [![security: Checkmarks](https://img.shields.io/badge/Security-Checkmarks-yellow)](https://github.com/PyCQA/bandit)
 
 
 _____
 ## Overview
 ---
-data_connector is a tool to connect to AzureML, Azure blob, GCP storage, GCP Big Query  and AWS storage S3. 
+**Cloud data connector** is a tool to connect to AzureML, Azure blob, GCP storage, GCP Big Query  and AWS storage S3. 
 The goal is provide all cloud managers in one place and provide documentation for an easy integration.
 
-For more details, visit the [Data Connector](https://github.com/IntelAI/models/tree/master/datasets/data_connector) GitHub repository.
+For more details, visit the [Cloud Data Connector](https://github.com/IntelAI/models/tree/master/datasets/cloud_data_connector) GitHub repository.
 <br/><br/>
 
 ## Hardware Requirements
 ---
 The hardware should comply with the same requirements that the cloud service.
 <br/><br/>
 
 ## How it Works
 ---
 The package contains the following modules:
 
 | Package Components   |
 | -------------------- |
-| data_connector.aws   |
-| data_connector.gcp   |
-| data_connector.azure |
+| cloud_data_connector.aws   |
+| cloud_data_connector.gcp   |
+| cloud_data_connector.azure |
 
 Each module is capable of connect, download and upload operation to it-s corresponding cloud service.
 <br/><br/>
 
-## Getting Started with data_connector
+## Getting Started with **Cloud Data Connector**
 ---
 
 It is strongly recommended to use a virtual environment to ensure proper operation, example:
 ```bash
 conda create -n venv python=3.10 -c conda-forge
 conda activate venv
 ```
 
 You can install the package with:
 ```bash
 python -m pip install cloud-data-connector
 ```
 
 Please follow module specific documentation for use case, hands-examples.
-1. data_connector/azure/README.md
-2. data_connector/azure/AzureML.md
-3. data_connector/aws/README.md
-4. data_connector/gcp/README.md
+1. cloud_data_connector/azure/README.md
+2. cloud_data_connector/azure/AzureML.md
+3. cloud_data_connector/aws/README.md
+4. cloud_data_connector/gcp/README.md
 <br/><br/>
 
-## Getting Started with data_connector.azure
+## Getting Started with **Cloud Data Connector Azure**
 ---
 
 ### Abstract
-Intel's [Data Connector](../../README.md) AzureML tool allows users follow a simple flow to work locally on model training and upload jobs to AzureML configuring a job, workflow, upload models or training scripts.
+Intel's [Cloud Data Connector](https://github.com/IntelAI/models/tree/master/datasets/cloud_data_connector/README.md) AzureML tool allows users follow a simple flow to work locally on model training and upload jobs to AzureML configuring a job, workflow, upload models or training scripts.
 Data connector for Azure is a tool to connect to Azure Blob and Azure Machine Learning tools.
 
 ### Requirements
 This tool requires an account on Azure Cloud and an Azure ML worskspace active.
 * Azure Account 
 * Access to AzureML
 * [Create a workspace of Azure ML](https://learn.microsoft.com/en-us/azure/machine-learning/quickstart-create-resources#create-the-workspace)
@@ -87,15 +87,15 @@
 Azure ML is a service to train models connecting data sources and deploy it in production using Azure infrastructure.
 
 Data connector provides a tool to connect to Azure ML workspaces and upload configurations for this proposes.
 
 ### Sample
 **Blob Connector**
 ```python
-    from data_connector.azure import connect
+    from cloud_data_connector.azure import connect
     connection_string_sample = """
         DefaultEndpointsProtocol=http;
         AccountName=<YOUR_ACCOUNT_NAME>;
         AccountKey=<YOUR_ACCOUNT_KEY>;
         BlobEndpoint=http://127.0.0.1:10000/
         devstoreaccount1;
         QueueEndpoint=http://127.0.0.1:10001/
@@ -119,39 +119,39 @@
 >az storage account show-connection-string --name <storageAccount> 
 ```
 * This process not works for WSL 
 
 
 **Blob upload**
 ```python
-    from data_connector.azure import Uploader
+    from cloud_data_connector.azure import Uploader
 
     uploader = Uploader(connector= connector)
     uploader.upload(
         'sample.txt',
         blob_container_name='sample_container'
     )
 ```
 
 **Blob downloader**
 ```python
-    from data_connector.azure import Downloader
+    from cloud_data_connector.azure import Downloader
 
     downloader = Downloader(connector=connector)
     downloader.download()
 ```
-[See sample Here](https://github.com/IntelAI/models/blob/master/datasets/data_connector/samples/azure/blob_sample.py)
+[See sample Here](https://github.com/IntelAI/models/blob/master/datasets/cloud_data_connector/samples/azure/blob_sample.py)
 <br/><br/>
 
 
-## Getting Started with data_connector.aws
+## Getting Started with **Cloud Data Connector AWS**
 ---
-### Data Connector AWS S3 
+### Cloud Data Connector AWS S3 
 
-Data Connector for AWS S3 allows you to connect to S3 buckets and list contents, download and upload files.
+Cloud Data Connector for AWS S3 allows you to connect to S3 buckets and list contents, download and upload files.
 
 ### Access S3 buckets
 
 To access S3 buckets, you will need to sign up for an AWS account and create access keys. 
 
 Access keys consist of an access key ID and secret access key, which are used to sign programmatic requests that you make to AWS.
 
@@ -177,15 +177,15 @@
 You can add more configuration settings listed [here](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html#using-environment-variables). For example, you can set the `AWS_SESSION_TOKEN`, it is only needed when you are using temporary credentials.
 
 ### Usage
 
 You need to import the DataConnector class.
 
 ```python
-from data_connector.aws.connector import Connector
+from cloud_data_connector.aws.connector import Connector
 ```
 
 Connector class has the method connect(), it creates an AWS S3 object, by default the function will create a S3 connector using the credentials saved in your environment variables.
 
 ```python
 connector = Connector()
 ```
@@ -195,81 +195,81 @@
 ```python
 conection_object = connector.connect()
 ```
 
 Import the Downloader class and use the connection object returned by connect() function.
 
 ```python
-from data_connector.aws.downloader import Downloader
+from cloud_data_connector.aws.downloader import Downloader
 
 downloader = Downloader(conection_object)
 ```
 
 The Downloader class has two methods:
 
 - list_blobs(container_obj): The function to get a list of the objects in a bucket.
 - download(container_obj, data_file, destiny): The function to download a file from a S3 bucket.
 
 A first step with buckets is to list their content using the `list_blobs(container_obj)` method. Specify the next parameter.
 
 - container_obj: The bucket name to list.
 
 ```python
-from data_connector.aws.downloader import Downloader
+from cloud_data_connector.aws.downloader import Downloader
 
 downloader = Downloader(conection_object)
 
 list_blobs = downloader.list_blobs('MY_BUCKET_NAME')
 print(list_blobs)
 ```
 
 To download a file use the `download(container_obj, data_file, destiny)` method and specify the next parameters.
 
 - container_obj: The name of the bucket to download from.
 - data_file: The name of the file to download from.
 - destiny: The path to the file to download to.
 
 ```python
-from data_connector.aws.downloader import Downloader
+from cloud_data_connector.aws.downloader import Downloader
 
 downloader = Downloader(conection_object)
 file_name = "path/to_file.csv"
 downloader.download(bucket_name, file_name, 'path/to_destiny.csv')
 ```
 
 You can import an Uploader class and use the upload method to send a file from you local machine to a bucket. You need to add the connector object to Uploader constructor.
 
 ```python
-from data_connector.aws.uploader import Uploader
-from data_connector.aws.connector import Connector
+from cloud_data_connector.aws.uploader import Uploader
+from cloud_data_connector.aws.connector import Connector
 
 connector = Connector()
 conection_object = connector.connect()
 uploader = Uploader(conection_object)
 
 ```
 Specify the next parameters in upload function.
 
 - container_obj: The name of the bucket to upload to.
 - data_file: The path to the file to upload.
 - object_name: The name of the file to upload to.
 
 ```python
-from data_connector.aws.uploader import Uploader
+from cloud_data_connector.aws.uploader import Uploader
 
 uploader = Uploader(conection_object)
 uploader.upload(bucket_name, 'path/to_local_file.csv', 'path/to_object_name.csv')
 ```
 
 ### List objects in a bucket
 
 ```python
 # import the dataconnector package
-from data_connector.aws.connector import Connector
-from data_connector.aws.downloader import Downloader
+from cloud_data_connector.aws.connector import Connector
+from cloud_data_connector.aws.downloader import Downloader
 
 # specify a S3 bucket name
 bucket_name = 'MY_BUCKET_NAME'
 # create a connector
 connector = Connector()
 # connect to aws using default AWS access keys
 # connect() method uses the configurations settings for AWS account
@@ -284,16 +284,16 @@
 
 ```
 
 ### Download a file
 
 ```python
 # import the dataconnector package
-from data_connector.aws.connector import Connector
-from data_connector.aws.downloader import Downloader
+from cloud_data_connector.aws.connector import Connector
+from cloud_data_connector.aws.downloader import Downloader
 
 # specify a S3 bucket name
 bucket_name = 'MY_BUCKET_NAME'
 # create a connector
 connector = Connector()
 # connect to aws using default aws access keys
 conection_object = connector.connect()
@@ -306,16 +306,16 @@
 downloader.download(bucket_name, file_name, 'path/to_destiny.csv')
 ```
 
 ### Upload a file
 
 ```python
 # import dataconnector package
-from data_connector.aws.connector import Connector
-from data_connector.aws.uploader import Uploader
+from cloud_data_connector.aws.connector import Connector
+from cloud_data_connector.aws.uploader import Uploader
 
 # specify a S3 bucket name
 bucket_name = 'MY_BUCKET_NAME'
 # create a connector
 connector = Connector()
 # connect to aws using default aws access keys
 conection_object = connector.connect()
@@ -323,42 +323,42 @@
 # create a uploader object using a connection object
 uploader = Uploader(conection_object)
 # upload a file
 uploader.upload(bucket_name, 'path/to_local_file.csv', 'path/to_object_name.csv')
 ```
 <br/><br/>
 
-## Getting Started with data_connector.gcp
+## Getting Started with **Cloud Data Connector GCP**
 ---
 ### GCP Permissions
 To enable permissions in GCP to use Storage and BigQuery, from the the left side navigation menu, inside Google Cloud, go to "APIs & Services > Library" and search and enable:
 - Cloud Storage
 - Google Cloud Storage JSON API
 - BigQuery API
 
 You need one of two authentication tools: Oauth or Service Account
 ### Oauth
 To enable oauth2, from the the left side navigation menu go to "APIs & Services > Credentials" and select "+ CREATE CREDENTIALS". From the three available options select "OAuth client ID". When creating an ID it is necessary to provide an "Application type" and a Name, which for this case select "Desktop app" for  "Application type" and type a name of your preference. Once the ID has been created a window will pop with the Client ID and Secret; select "DOWNLOAD JSON" and store the JSON file in a secure place.
 ### Service Account
-To enable a service account, from the left side navigation menu go to "APIs & Services > Credentials" and select "+ CREATE CREDENTIALS". From the three available options select "Service account". In "Service account details" provide a service account name and ID and select "CREATE AND CONTINUE". In "Grant this service account access to project" select roles: "Cloud Storage -> Storage Admin" and "BigQuery -> BigQuery Admin". After defining roles press "Done". Go to the created service account by selecting the service e-mail in "Service Accounts" and go to "KEYS", from there you can create a new key for the account(it will provide a JSON file).
+To enable a service account, from the left side navigation menu go to "APIs & Services > Credentials" and select "+ CREATE CREDENTIALS". From the three available options select "Service account". In "Service account details" provide a service account name and ID and select "CREATE AND CONTINUE". In "Grant this service account access to project" select roles: "Cloud Storage > Storage Admin" and "BigQuery > BigQuery Admin". After defining roles press "Done". Go to the created service account by selecting the service e-mail in "Service Accounts" and go to "KEYS", from there you can create a new key for the account(it will provide a JSON file).
 
 ### Installing Into Docker Container
 To be able to run data connector inside a Docker container execute the following command changing options as needed:
 ```bash
 docker run  -it  --name <container_name> --net=host -v <path to frameworks.ai.models.intel-mode.data-connector>:/workspace/model-zoo --env HTTPS_PROXY=$HTTPS_PROXY --env no_proxy=$no_proxy --env HTTP_PROXY=$HTTP_PROXY --env http_proxy=$http_proxy  --entrypoint bash conda/miniconda3:latest
 ```
 
 Inside the docker container set source to activate conda:
 ```bash
 source /usr/local/bin/activate
 ```
 To install requirements.txt file, first a conda environment must be created:
 ```bash
-conda create -n data_connector python=3.9 -y && \
-conda activate data_connector
+conda create -n cloud_data_connector python=3.9 -y && \
+conda activate cloud_data_connector
 ```
 To be able to run the GCP part of the connector, GCP CLI must be [installed](https://cloud.google.com/sdk/docs/install). The easy way to install the CLI repository is by running the following commands inside the container:
 ```bash
 apt-get update && \
 apt-get install apt-transport-https ca-certificates gnupg curl gpg -y && \
 echo "deb [signed-by=/usr/share/keyrings/cloud.google.gpg] http://packages.cloud.google.com/apt cloud-sdk main" | tee -a /etc/apt/sources.list.d/google-cloud-sdk.list && curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | apt-key --keyring /usr/share/keyrings/cloud.google.gpg  add - && apt-get update -y && apt-get install google-cloud-cli -y
 ```
@@ -376,53 +376,53 @@
 
 To provide access for the libraries to oauth run:
 ```bash
 gcloud auth application-default login
 ```
 Open the provided link in a web browser. GCP will ask for permissions to access the account; allow the permissions and copy the provided verification code in gcloud CLI.
 
-Go to data_connector directory, upgrade pip packages and install requirements.txt:
+Go to cloud_data_connector directory, upgrade pip packages and install requirements.txt:
 ```bash
-cd /workspace/model-zoo/data_connector
+cd /workspace/model-zoo/cloud_data_connector
 pip install --upgrade pip wheel setuptools
-pip install -r data_connector/gcp/requirements.txt 
+pip install -r cloud_data_connector/gcp/requirements.txt 
 ```
 
 ### Running Code Samples
 To run code portions inside a container and VS code the port to be used by OAuth must be added to the list of forwarded ports. Open OUTPUT terminal (Ctrl + Shift + U), go to PORTS and select "Add Port".
 
-To provide the JSON key obtained for OAuth in Google Cloud, the file content must be assigned to the 'CLIENT_SECRETS' environment variable. Also it can be obtained from a ".env" file that contains the variable. To use it from a ".env" file "python-dotenv" must be installed and the file must be in a location were "load_dotenv()" can find it. dotenv can find ".env" file inside the directory where a script is being executed, e.g. for the samples provided below you can add ".env" file into <base_path_to_model_zoo>/data_connector/data_connector/samples/gcp/ directory.
+To provide the JSON key obtained for OAuth in Google Cloud, the file content must be assigned to the 'CLIENT_SECRETS' environment variable. Also it can be obtained from a ".env" file that contains the variable. To use it from a ".env" file "python-dotenv" must be installed and the file must be in a location were "load_dotenv()" can find it. dotenv can find ".env" file inside the directory where a script is being executed, e.g. for the samples provided below you can add ".env" file into ```<base_path_to_model_zoo>/cloud_data_connector/cloud_data_connector/samples/gcp/``` directory.
 
 ```bash
 pip install python-dotenv
 ```
 To provide the JSON key obtained for the service account, the file path must be provided to the sample scripts if access to Storage or BigCloud is going to be made through service account.
 
 To test GCP Storage a bucket must be created. Go to "Cloud Storage > Buckets" and select "Create". There you need to provide several  options to create a bucket (for the example the name of the bucket will be "dataconnector_data_bucket"), for the following example the default values can be used.
 
-To test GCP Storage there is a script located in <base_path_to_model_zoo>/data_connector/data_connector/samples/gcp/storage.py. To run it execute from the base path of data connector for OAuth:
+To test GCP Storage there is a script located in ```<base_path_to_model_zoo>/cloud_data_connector/cloud_data_connector/samples/gcp/storage.py```. To run it execute from the base path of data connector for OAuth:
 ```bash
 python -m samples.gcp.storage -o
 ```
 For service account:
 ```bash
 python -m samples.gcp.storage -p <project_name> -c <credentials_path>
 ```
 User must provide the project name using flag (-p) and the local path to the JSON file with the credentials (-c).
 
-To test GCP BigQuery there is a script located in <base_path_to_model_zoo>/data_connector/data_connector/samples/gcp/bigquery.py. To run it execute from the base path of data connector for OAuth:
+To test GCP BigQuery there is a script located in ```<base_path_to_model_zoo>/cloud_data_connector/cloud_data_connector/samples/gcp/bigquery.py```. To run it execute from the base path of data connector for OAuth:
 ```bash
 python -m samples.gcp.bigquery -o
 ```
 For service account:
 ```bash
 python -m samples.gcp.bigquery -p <project_name> -c <credentials_path>
 ```
 User must provide the project name using flag (-p) and the local path to the JSON file with the credentials (-c).
 <br/><br/>
 
 
 ## Support
 ---
 If you have questions or issues about this package, contact the [Support Team](mailto:IntelAI@intel.com).
-data_connector has an Apache license, as found in the [LICENSE](https://www.apache.org/licenses/LICENSE-2.0) file.
+Cloud Data Connector has an Apache license, as found in the [LICENSE](https://www.apache.org/licenses/LICENSE-2.0) file.
 Dependencies versions higher than currently implemented ones are in beta and should be used with caution.
```

### Comparing `cloud_data_connector-1.0.1/data_connector/aws/README.md` & `cloud_data_connector-1.0.2/cloud_data_connector/aws/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Cloud Data Connector: AWS S3 
 
-Data Connector for AWS S3 allows you to connect to S3 buckets and list contents, download and upload files.
+Cloud Data Connector for AWS S3 allows you to connect to S3 buckets and list contents, download and upload files.
 
 ## Access S3 buckets
 
 To access S3 buckets, you will need to sign up for an AWS account and create access keys. 
 
 Access keys consist of an access key ID and secret access key, which are used to sign programmatic requests that you make to AWS.
 
@@ -31,15 +31,15 @@
 You can add more configuration settings listed [here](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html#using-environment-variables). For example, you can set the `AWS_SESSION_TOKEN`, it is only needed when you are using temporary credentials.
 
 ## Usage
 
 You need to import the DataConnector class.
 
 ```python
-from data_connector.aws import Connector as aws_connector
+from cloud_data_connector.aws import Connector as aws_connector
 ```
 
 Connector class has the method connect(), it creates an AWS S3 object, by default the function will create a S3 connector using the credentials saved in your environment variables.
 
 ```python
 aws_bucket_connector = aws_connector()
 ```
@@ -52,29 +52,29 @@
 
 Downloader
 ---
 Import the Downloader class and use the connection object returned by connect() function.
 
 
 ```python
-from data_connector.aws import Downloader as aws_downloader
+from cloud_data_connector.aws import Downloader as aws_downloader
 
 aws_file_downloader = aws_downloader(aws_conection_object)
 ```
 
 
 
 To download a file use the `download(container_obj, data_file, destiny)` method and specify the next parameters.
 
 - container_obj: The name of the bucket to download from.
 - data_file: The name of the file to download from.
 - destiny: The path to the file to download to.
 
 ```python
-from data_connector.aws import Downloader as aws_downloader
+from cloud_data_connector.aws import Downloader as aws_downloader
 
 downloader = aws_downloader(aws_conection_object)
 file_name = "path/to_file.csv"
 downloader.download(bucket_name, file_name, 'path/to_destiny.csv')
 ```
 List Blobs
 ---
@@ -83,15 +83,15 @@
 - download(container_obj, data_file, destiny): The function to download a file from a S3 bucket.
 
 A first step with buckets is to list their content using the `list_blobs(container_obj)` method. Specify the next parameter.
 
 - container_obj: The bucket name to list.
 
 ```python
-from data_connector.aws import Downloader as aws_downloader
+from cloud_data_connector.aws import Downloader as aws_downloader
 
 aws_bucket_downloader = aws_downloader(aws_conection_object)
 
 list_blobs = aws_bucket_downloader.list_blob(
     'MY_BUCKET_NAME'
 )
 print(list_blobs)
@@ -99,16 +99,16 @@
 
 Upload
 ---
 
 You can import an Uploader class and use the upload method to send a file from you local machine to a bucket. You need to add the connector object to Uploader constructor.
 
 ```python
-from data_connector.aws import Uploader as aws_uploader
-from data_connector.aws  import Connector as aws_connector
+from cloud_data_connector.aws import Uploader as aws_uploader
+from cloud_data_connector.aws  import Connector as aws_connector
 
 aws_bucket_connector = aws_connector()
 aws_conection_object = aws_bucket_connector.connect()
 aws_bucker_uploader = aws_uploader(aws_conection_object)
 
 ```
 Specify the next parameters in upload function.
@@ -124,16 +124,16 @@
 
 Samples
 ---
 ### List objects in a bucket
 
 ```python
 # import the dataconnector package
-from data_connector.aws import Connector as aws_connector
-from data_connector.aws import Downloader as aws_downloader
+from cloud_data_connector.aws import Connector as aws_connector
+from cloud_data_connector.aws import Downloader as aws_downloader
 
 # specify a S3 bucket name
 bucket_name = 'MY_BUCKET_NAME'
 # create a connector
 aws_bucket_connector = aws_connector()
 # connect to aws using default AWS access keys
 # connect() method uses the configurations settings for AWS account
@@ -148,16 +148,16 @@
 
 ```
 
 ### Download a file
 
 ```python
 # import the dataconnector package
-from data_connector.aws import Connector as aws_connector
-from data_connector.aws import Downloader as aws_connector
+from cloud_data_connector.aws import Connector as aws_connector
+from cloud_data_connector.aws import Downloader as aws_connector
 
 # specify a S3 bucket name
 bucket_name = 'MY_BUCKET_NAME'
 # create a connector
 aws_bucket_connector = aws_connector()
 # connect to aws using default aws access keys
 aws_conection_object = aws_bucket_connector.connect()
@@ -170,16 +170,16 @@
 aws_downloader.download(bucket_name, file_name, 'path/to_destiny.csv')
 ```
 
 ### Upload a file
 
 ```python
 # import dataconnector package
-from data_connector.aws import Connector as aws_connector
-from data_connector.aws import Uploader as aws_uploader
+from cloud_data_connector.aws import Connector as aws_connector
+from cloud_data_connector.aws import Uploader as aws_uploader
 
 # specify a S3 bucket name
 bucket_name = 'MY_BUCKET_NAME'
 # create a connector
 aws_bucket_connector = aws_connector()
 # connect to aws using default aws access keys
 aws_conection_object = aws_bucket_connector.connect()
```

### Comparing `cloud_data_connector-1.0.1/data_connector/aws/__init__.py` & `cloud_data_connector-1.0.2/cloud_data_connector/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.1/data_connector/aws/connector.py` & `cloud_data_connector-1.0.2/cloud_data_connector/aws/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import boto3
 import botocore
-from data_connector.int.int_connector import IntConnector
+from cloud_data_connector.int.int_connector import IntConnector
 
 class Connector(IntConnector):
     """
     This is a class for create a connection to AWS S3 buckets.
 
     """
     def __init__(self):
```

### Comparing `cloud_data_connector-1.0.1/data_connector/aws/downloader.py` & `cloud_data_connector-1.0.2/cloud_data_connector/aws/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from data_connector.int.int_downloader import IntDownloader
+from cloud_data_connector.int.int_downloader import IntDownloader
 import botocore.exceptions
 import botocore.client
 import logging
 
 # Set up our logger
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
```

### Comparing `cloud_data_connector-1.0.1/data_connector/aws/uploader.py` & `cloud_data_connector-1.0.2/cloud_data_connector/aws/uploader.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import os
-from data_connector.int.int_uploader import IntUploader
+from cloud_data_connector.int.int_uploader import IntUploader
 from botocore.exceptions import ClientError
 import logging
 import botocore
 
 class Uploader(IntUploader):
     """
     This is a class for upload operations for AWS S3 buckets.
```

### Comparing `cloud_data_connector-1.0.1/data_connector/azure/AzureML.md` & `cloud_data_connector-1.0.2/cloud_data_connector/azure/AzureML.md`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.1/data_connector/azure/README.md` & `cloud_data_connector-1.0.2/cloud_data_connector/azure/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 Data connector provides a tool to connect to Azure ML workspaces and upload configurations for this proposes.
 
 Sample
 
 Blob Connector
 ---
 ```python
-    from data_connector.azure import connect as connect_az
+    from cloud_data_connector.azure import connect as connect_az
 
     connection_string_sample = """
         DefaultEndpointsProtocol=http;
         AccountName=<YOUR_ACCOUNT_NAME>;
         AccountKey=<YOUR_ACCOUNT_KEY>
         BlobEndpoint=http://127.0.0.1:10000/
         devstoreaccount1;
@@ -48,15 +48,15 @@
     az_connector = connect_az(
         connection_string=connection_string_sample
     )
 
 ```
 How to get a [Connection String](https://learn.microsoft.com/en-us/answers/questions/1071173/where-can-i-find-storage-account-connection-string)? 
 
-![Azure Connection String Sample](data_connector/../../../docs/img/connection_string.png)
+![Azure Connection String Sample](cloud_data_connector/../../../docs/img/connection_string.png)
 
 Also you can get connection strings using Azure CLI
 ```bash
 >az storage account show-connection-string --name <storageAccount> --resource-group <resourceGroup> --subscription <subscription>
 ```
 Or just 
 ```bash
@@ -64,27 +64,27 @@
 ```
 * This process not works for WSL 
 
 
 Uploader
 ---------
 ```python
-    from data_connector.azure import Uploader as az_uploader
+    from cloud_data_connector.azure import Uploader as az_uploader
 
     uploader = az_uploader(connector= az_connector)
     az_uploader.upload(
         '<file path>',
         blob_container_name='<countainer name>'
     )
 ```
 
 Downloader
 -----
 ```python
-    from data_connector.azure import Downloader
+    from cloud_data_connector.azure import Downloader
 
     downloader = Downloader(connector=connector)
     downloader.download()
 ```
 
 [See sample](../../samples/azure/blob_sample.py)
 -----
```

### Comparing `cloud_data_connector-1.0.1/data_connector/azure/__init__.py` & `cloud_data_connector-1.0.2/cloud_data_connector/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.1/data_connector/azure/connector.py` & `cloud_data_connector-1.0.2/cloud_data_connector/azure/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from data_connector.int.int_connector import IntConnector
+from cloud_data_connector.int.int_connector import IntConnector
 
 # Python
 from os.path import exists
 
 # Azure Blob
 from azure.storage.blob import BlobServiceClient
```

### Comparing `cloud_data_connector-1.0.1/data_connector/azure/connector_object.py` & `cloud_data_connector-1.0.2/cloud_data_connector/azure/connector_object.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.1/data_connector/azure/downloader.py` & `cloud_data_connector-1.0.2/cloud_data_connector/azure/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from data_connector.int.int_downloader import IntDownloader
+from cloud_data_connector.int.int_downloader import IntDownloader
 # Azure
 from azure.storage.blob import BlobServiceClient, ContainerClient
 from azureml.core.model import Model
 from azureml.core.dataset import Dataset
 from azure.ai.ml import MLClient
 from azure.storage.blob import BlobClient, ContainerClient
 CONNECTOR_TYPE_ERROR = "Connector for blobs should be a BlobServiceClient"
```

### Comparing `cloud_data_connector-1.0.1/data_connector/azure/ml_uploader.py` & `cloud_data_connector-1.0.2/cloud_data_connector/azure/ml_uploader.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.1/data_connector/azure/uploader.py` & `cloud_data_connector-1.0.2/cloud_data_connector/azure/uploader.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from azure.storage.blob import BlobServiceClient, ContainerClient
 from azureml.core.environment import DockerBuildContext, Environment
 from azureml.core.workspace import Workspace
 from azure.ai.ml import MLClient
 # Exceptions
 from azure.core.exceptions import ResourceExistsError
 # Interface
-from data_connector.int.int_uploader import IntUploader
+from cloud_data_connector.int.int_uploader import IntUploader
 
 
 DOCKER_FILE_NOT_EXISTS = "Docker file not exists "
 FILE_SOURCE_NOT_FOUND = "Source file not found "
 BAD_CONNECTOR_INSTANCE = "Connector instance is not correct "
 BLOB_ALREADY_EXISTS = "Blob file already exist with this name"
```

### Comparing `cloud_data_connector-1.0.1/data_connector/gcp/README.md` & `cloud_data_connector-1.0.2/cloud_data_connector/gcp/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,58 @@
-# Cloud Data Connector: Google Cloud Platform (GCP) 
+# Cloud Data Connector: Google Cloud Platform (GCP)
 
-* [Permissions](#permissions)
+* [Authorization](#authorization)
+* [Authentication](#authentication)
+* [Installing Into Docker Container](#installing-into-docker-container)
 * [Connect](#connect)
 * [Uploader](#uploader)
-* [List Blobs](#list-blobs)
 * [Downloader](#downloader)
+* [List Blobs](#list-blobs)
+* [Big Query](#big-query)
 * [Sample](#sample)
-___
-Authorization
----
-To enable permissions in GCP= to use Storage and BigQuery, from the the left side navigation menu, inside Google Cloud, go to "APIs & Services > Library" and search and enable:
+
+
+# Authorization
+
+To enable permissions in GCP to use Storage and BigQuery, from the the left side navigation menu, inside Google Cloud, go to "APIs & Services > Library" and search and enable:
 - Cloud Storage
 - Google Cloud Storage JSON API
 - BigQuery API
 
-You need one of two authentication tools: Oauth or Service Account
+You need one of two authentication tools: OAuth or Service Account
 
-___
-## Authentication
----
 
-Oauth
----
-To enable oauth2, from the the left side navigation menu go to 
+# Authentication
 
-"APIs & Services > Credentials" 
+## Oauth
 
-and select
+To enable OAuth, from the the left side navigation menu go to  "APIs & Services > Credentials" and select "+ CREATE CREDENTIALS".
+From the three available options select "OAuth client ID".
 
-"+ CREATE CREDENTIALS"
+ When creating an ID it is necessary to provide an "Application type" and a name, which for this case select "Desktop app" for  "Application type" and type a name of your preference. Once the ID has been created a window will pop with the Client ID and Secret; select "DOWNLOAD JSON" and store the JSON file in a secure place.
 
-From the three available options select 
+## Service Account
 
-"OAuth client ID"
+To enable a service account, from the left side navigation menu go to "APIs & Services > Credentials" and select "+ CREATE CREDENTIALS". From the three available options select "Service account". In "Service account details" provide a service account name and ID and select "CREATE AND CONTINUE". In "Grant this service account access to project" select roles: "Cloud Storage > Storage Admin" and "BigQuery > BigQuery Admin". After defining roles press "Done". Go to the created service account by selecting the service e-mail in "Service Accounts" and go to "KEYS", from there you can create a new key for the account (it will provide a JSON file).
 
- When creating an ID it is necessary to provide an "Application type" and a Name, which for this case select "Desktop app" for  "Application type" and type a name of your preference. Once the ID has been created a window will pop with the Client ID and Secret; select 
- 
- "DOWNLOAD JSON" and store the JSON file in a secure place.
+# Installing Into Docker Container
 
-Service Account
----
-To enable a service account, from the left side navigation menu go to "APIs & Services > Credentials" and select "+ CREATE CREDENTIALS". From the three available options select "Service account". In "Service account details" provide a service account name and ID and select "CREATE AND CONTINUE". In "Grant this service account access to project" select roles: "Cloud Storage -> Storage Admin" and "BigQuery -> BigQuery Admin". After defining roles press "Done". Go to the created service account by selecting the service e-mail in "Service Accounts" and go to "KEYS", from there you can create a new key for the account(it will provide a JSON file).
-___
-Installing Into Docker Container
----
-To be able to run data connector inside a Docker container execute the following command changing options as needed:
+To be able to run cloud data connector inside a Docker container execute the following command changing options as needed:
 ```bash
 docker run  -it  --name <container_name> --net=host -v <path to IntelAI/models>:/workspace/model-zoo --entrypoint bash conda/miniconda3:latest
 ```
 
 Inside the docker container set source to activate conda:
 ```bash
 source /usr/local/bin/activate
 ```
 To install requirements.txt file, first a conda environment must be created:
 ```bash
-conda create -n data_connector python=3.9 -y && \
-conda activate data_connector
+conda create -n cloud_data_connector python=3.9 -y && \
+conda activate cloud_data_connector
 ```
 To be able to run the GCP part of the connector, GCP CLI must be [installed](https://cloud.google.com/sdk/docs/install). The easy way to install the CLI repository is by running the following commands inside the container:
 ```bash
 apt-get update && \
 apt-get install apt-transport-https ca-certificates gnupg curl gpg -y && \
 echo "deb [signed-by=/usr/share/keyrings/cloud.google.gpg] http://packages.cloud.google.com/apt cloud-sdk main" | tee -a /etc/apt/sources.list.d/google-cloud-sdk.list && curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | apt-key --keyring /usr/share/keyrings/cloud.google.gpg  add - && apt-get update -y && apt-get install google-cloud-cli -y
 ```
@@ -72,168 +64,165 @@
 ```
 To initialize the CLI you must have a GCP account. Run the following command, accept the login request, open the provided link in a web browser:
 ```bash
 gcloud init
 ```
 Once in the browser GCP will ask for permissions to access the account; allow the permissions and copy the provided verification code in gcloud CLI. When providing the verification code select the desired cloud project. 
 
-To provide access for the libraries to oauth run:
+To provide access for the libraries to OAuth run:
 ```bash
 gcloud auth application-default login
 ```
 Open the provided link in a web browser. GCP will ask for permissions to access the account; allow the permissions and copy the provided verification code in gcloud CLI.
 
-Go to data_connector directory, upgrade pip packages and install requirements.txt:
+Go to cloud_data_connector directory, upgrade pip packages and install requirements.txt:
 ```bash
-cd /workspace/model-zoo/data_connector
+cd /workspace/model-zoo/cloud_data_connector
 pip install --upgrade pip wheel setuptools
-pip install -r data_connector/gcp/requirements.txt 
+pip install -r cloud_data_connector/gcp/requirements.txt 
 ```
-___
-Connect
----
-### Oauth Connection
-Oauth authentication is a way to authenticate users and delegate functions related with authorizations.
 
-To connect using Oauth you need go to your gcp console and follow instructions to get your [client secret json file](#oauth), in [sample](../../samples/gcp/storage.py) you can see that this file location is handled as environment varialbe called CLIENT_SECRETS. 
+# Connect
+
+## OAuth Connection
+OAuth authentication is a way to authenticate users and delegate functions related with authorizations.
+
+To connect using OAuth you need go to your gcp console and follow instructions to get your [client secret json file](#oauth), in [sample](../../samples/gcp/storage.py) you can see that this file location is handled as environment varialbe called CLIENT_SECRETS. 
 ```python
-from data_connector.gcp import Connector as gcp_connector
-# Get location of oauth client secrets file from 
+from cloud_data_connector.gcp import Connector as gcp_connector
+# Get location of OAuth client secrets file from 
 # environment variables.
 CLIENT_SECRETS_LOCATION = os.getenv('CLIENT_SECRETS')
 # Creates a GCP connector for storage functionality
 gcp_storage_connector = gcp_connector("storage")
-# Here is where oauth process start, you will see a 
+# Here is where OAuth process start, you will see a 
 # navigator open in GCP asking for access to this resource
 gcp_oauth_credentials = gcp_connector.get_credentials_from_config(
     CLIENT_SECRETS_LOCATION,
-    # You can choose any other free port to open oauth 
+    # You can choose any other free port to open OAuth 
     # local sever
     port=8080 
 )
 gcp_storage_client = gcp_connect(
     connector_object=gcp_credentials
 )
 ```
-### Service Account Connectio
+## Service Account Connection
 
-Service account is a server to server authentication tecnique. 
-GCP povides service account connection where is necesary specify the 
-services you want to give access.
-In this sample a json file related with service account is associated with an environment varialbe called GOOGLE_APPLICATION_CREDENTIALS
+Service account is a server to server authentication technique. 
+GCP provides service account connection where is necessary specify the services you want to give access.
+In this sample a json file related with service account is associated with an environment variable called GOOGLE_APPLICATION_CREDENTIALS
 
 ```python
-from data_connector.gcp import Connector as gcp_connector
+from cloud_data_connector.gcp import Connector as gcp_connector
 gcp_storage_connector = gcp_connector.connect("Storage")
 gcp_storage_client = gcp_storage_connector.connect(connection_string='<YOUR_PROJECT_NAME>')
 ```
 
-### Service Account Connection
-Uploader
----
+# Uploader
+Sample code of how to upload blobs:
 ```python
-from data_connector.gcp  import Uploader as gcp_uploader
+from cloud_data_connector.gcp  import Uploader as gcp_uploader
 
 file_path = '<File path to upload>'
 bucket_name = '<Your bucket name>'
 storage_blob_name = '<your storage blob name>'
 # Creating a connector gcp
 gcp_blob_uploader = gcp_uploader(gcp_storage_client)
 # Upload file
 gcp_blob_uploader.upload_to_bucket(
     bucket_name,
     file_path,
     storage_blob_name
 )
 ```
 
-Downloader
----
+# Downloader
+Sample code of how to download blobs:
 ```python
-from data_connector.gcp import Downloader as gcp_downloader
+from cloud_data_connector.gcp import Downloader as gcp_downloader
 
 gcp_blob_downloader = gcp_blob_downloader(gcp_storage_client)
 
 gcp_blob_downloader.download(
     bucket_name,
     storage_blob_name,
     '<Destiny path with file name>'
 )
 ```
 
 
-List blobs
----
+# List Blobs
+Sample code of how to list blobs:
 ```python
-from data_connector.gcp import Downloader as gcp_downloader
+from cloud_data_connector.gcp import Downloader as gcp_downloader
 
 gcp_blob_downloader = gcp_blob_downloader(gcp_storage_client)
 gcp_blob_downloader.list_blobs(
     bucket_name
 )
 ```
 
 
-Big Query
----
-    You need an authentication object created for this. 
+# Big Query
+
+You need an authentication object created for this. 
 Big query is a tool to store a huge database in cloud. If you are familiar with big query you only need three concept names from your big query project.
-    * Dataset name
-    * Table name
-    * Project name
+* Dataset name
+* Table name
+* Project name
 
-### Oauth Connection
+## OAuth Connection
 
-__This sample has a json file from [gcp oauth](#oauth) and environment variable called CLIENT_SECRETS with this file path associated__ 
+This sample has a json file from [gcp oauth](#oauth) and environment variable called CLIENT_SECRETS with this file path associated
 ```python
-from data_connector.gcp import Connector as gcp_connector
+from cloud_data_connector.gcp import Connector as gcp_connector
 
 client_secrets_json_path = os.getenv("CLIENT_SECRETS")
 gcp_bq_connector = gcp_connector.get_credentials_from_config(client_secrets_json_path)
 big_query_client = gcp_bq_connector.connect(connector_object=gcp_bq_connector)
 
 ```
 
-### Service Account Connection
-__ This sample has  a json file from [gcp service account](#service-account) and enviroment variable called GOOGLE_APPLICATION_CREDENTIALS with this file path associatied, 
-also you requires a project name to connect to datasets__
+## Service Account Connection
+This sample has  a json file from [gcp service account](#service-account) and enviroment variable called GOOGLE_APPLICATION_CREDENTIALS with this file path associatied, 
+also you requires a project name to connect to datasets
 
 ```python
-from data_connector.gcp import Connector as gcp_connector
+from cloud_data_connector.gcp import Connector as gcp_connector
 
 gcp_bq_connector = gcp_connector("bigquery") 
 gcp_bq_client = gcp_bq_connector.connect(connection_string='<Your Project Name>')
 
 ```
 
+# Sample
 
-Sample
----
-To run code portions inside a container and VS code the port to be used by OAuth must be added to the list of forwarded ports. Open OUTPUT terminal (Ctrl + Shift + U), go to PORTS and select "Add Port".
+To run code portions inside a container using Visual Studio Code the port to be used by OAuth must be added to the list of forwarded ports. Open OUTPUT terminal (Ctrl + Shift + U), go to PORTS and select "Add Port".
 
-To provide the JSON key obtained for OAuth in Google Cloud, the file content must be assigned to the 'CLIENT_SECRETS' environment variable. Also it can be obtained from a ".env" file that contains the variable. To use it from a ".env" file "python-dotenv" must be installed and the file must be in a location were "load_dotenv()" can find it. dotenv can find ".env" file inside the directory where a script is being executed, e.g. for the samples provided below you can add ".env" file into <base_path_to_model_zoo>/data_connector/data_connector/samples/gcp/ directory.
+To provide the JSON key obtained for OAuth in Google Cloud, the file content must be assigned to the 'CLIENT_SECRETS' environment variable. Also it can be obtained from a ".env" file that contains the variable. To use it from a ".env" file "python-dotenv" must be installed and the file must be in a location were "load_dotenv()" can find it. dotenv can find ".env" file inside the directory where a script is being executed, e.g. for the samples provided below you can add ".env" file into ```<base_path_to_model_zoo>/cloud_data_connector/cloud_data_connector/samples/gcp/``` directory.
 
 ```bash
 pip install python-dotenv
 ```
 To provide the JSON key obtained for the service account, the file path must be provided to the sample scripts if access to Storage or BigCloud is going to be made through service account.
 
 To test GCP Storage a bucket must be created. Go to "Cloud Storage > Buckets" and select "Create". There you need to provide several  options to create a bucket (for the example the name of the bucket will be "dataconnector_data_bucket"), for the following example the default values can be used.
 
-To test GCP Storage there is a script located in <base_path_to_model_zoo>/data_connector/data_connector/samples/gcp/storage.py. To run it execute from the base path of data connector for OAuth:
+To test GCP Storage there is a script located in ```<base_path_to_model_zoo>/cloud_data_connector/cloud_data_connector/samples/gcp/storage.py```. To run it execute from the base path of cloud data connector for OAuth:
 ```bash
 python -m samples.gcp.storage -o
 ```
 For service account:
 ```bash
 python -m samples.gcp.storage -p <project_name> -c <credentials_path>
 ```
 User must provide the project name using flag (-p) and the local path to the JSON file with the credentials (-c).
 
-To test GCP BigQuery there is a script located in <base_path_to_model_zoo>/data_connector/data_connector/samples/gcp/bigquery.py. To run it execute from the base path of data connector for OAuth:
+To test GCP BigQuery there is a script located in ```<base_path_to_model_zoo>/cloud_data_connector/cloud_data_connector/samples/gcp/bigquery.py```. To run it execute from the base path of cloud data connector for OAuth:
 ```bash
 python -m samples.gcp.bigquery -o
 ```
 For service account:
 ```bash
 python -m samples.gcp.bigquery -p <project_name> -c <credentials_path>
 ```
```

### Comparing `cloud_data_connector-1.0.1/data_connector/gcp/__init__.py` & `cloud_data_connector-1.0.2/cloud_data_connector/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.1/data_connector/gcp/connector.py` & `cloud_data_connector-1.0.2/cloud_data_connector/gcp/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from data_connector.int.int_connector import IntConnector
+from cloud_data_connector.int.int_connector import IntConnector
 from google.oauth2.credentials import Credentials
 from google.cloud.client import Client
 from google_auth_oauthlib import flow
 from google.cloud import bigquery
 from google.cloud import storage
 from abc import ABCMeta
 import json
```

### Comparing `cloud_data_connector-1.0.1/data_connector/gcp/downloader.py` & `cloud_data_connector-1.0.2/cloud_data_connector/gcp/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from data_connector.int.int_downloader import IntDownloader
+from cloud_data_connector.int.int_downloader import IntDownloader
 from google.api_core.exceptions import NotFound
 from google.cloud.storage.client import Client
 from abc import ABCMeta
 
 class Downloader(IntDownloader, metaclass=ABCMeta):
     
     def __init__(self, connector: object):
```

### Comparing `cloud_data_connector-1.0.1/data_connector/gcp/query.py` & `cloud_data_connector-1.0.2/cloud_data_connector/gcp/query.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.1/data_connector/gcp/uploader.py` & `cloud_data_connector-1.0.2/cloud_data_connector/gcp/uploader.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.1/data_connector/int/int_connector.py` & `cloud_data_connector-1.0.2/cloud_data_connector/int/int_connector.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.1/data_connector/int/int_downloader.py` & `cloud_data_connector-1.0.2/cloud_data_connector/int/int_downloader.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.1/data_connector/int/int_uploader.py` & `cloud_data_connector-1.0.2/cloud_data_connector/int/int_uploader.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.1/pyproject.toml` & `cloud_data_connector-1.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cloud_data_connector"
-version = "1.0.1"
+version = "1.0.2"
 requires-python = ">=3.9,<3.11"
 authors = [
     { name="IntelAI", email="IntelAI@intel.com"}
 ]
 description = "Intel's cloud data connector"
 readme = "README.md"
 license = {file = "LICENSE"}
@@ -34,10 +34,10 @@
     "google-cloud-storage>=2.1.0",
     "packaging>=21.3",
     "python-dotenv>=1.0.0"
 ]
 
 [tool.setuptools.packages.find]
 where = ["."]  # list of folders that contain the packages (["."] by default)
-include = ["data_connector*"]
-exclude = ["data_connector.egg-info"]
+include = ["cloud_data_connector*"]
+exclude = ["cloud_data_connector.egg-info"]
 namespaces = false
```

