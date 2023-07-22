# Comparing `tmp/bentoctl-0.3.4.tar.gz` & `tmp/bentoctl-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bentoctl-0.3.4.tar", max compression
+gzip compressed data, was "bentoctl-0.4.0.tar", last modified: Sat Jul 22 05:48:57 2023, max compression
```

## Comparing `bentoctl-0.3.4.tar` & `bentoctl-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,48 @@
--rw-r--r--   0        0        0     3875 2022-04-07 10:56:34.418942 bentoctl-0.3.4/LICENSE.md
--rw-r--r--   0        0        0     4326 2022-08-09 01:57:00.642991 bentoctl-0.3.4/README.md
--rw-r--r--   0        0        0      224 2022-04-05 13:47:13.698433 bentoctl-0.3.4/bentoctl/__init__.py
--rw-r--r--   0        0        0     6605 2022-09-20 11:18:12.631250 bentoctl-0.3.4/bentoctl/cli/__init__.py
--rw-r--r--   0        0        0     9349 2022-07-15 08:03:28.816598 bentoctl-0.3.4/bentoctl/cli/interactive.py
--rw-r--r--   0        0        0     7132 2022-07-25 10:24:03.603680 bentoctl-0.3.4/bentoctl/cli/operator_management.py
--rw-r--r--   0        0        0     3866 2022-09-20 11:18:12.631250 bentoctl-0.3.4/bentoctl/cli/utils.py
--rw-r--r--   0        0        0     1696 2022-07-18 06:28:00.662787 bentoctl-0.3.4/bentoctl/console.py
--rw-r--r--   0        0        0     8435 2022-09-06 17:38:23.033218 bentoctl-0.3.4/bentoctl/deployment_config.py
--rw-r--r--   0        0        0     5118 2022-09-20 11:18:12.631250 bentoctl-0.3.4/bentoctl/docker_utils.py
--rw-r--r--   0        0        0     5122 2022-07-15 08:03:28.816598 bentoctl-0.3.4/bentoctl/exceptions.py
--rw-r--r--   0        0        0     1104 2022-07-15 08:03:28.816598 bentoctl-0.3.4/bentoctl/operator/README.md
--rw-r--r--   0        0        0      212 2022-03-27 13:44:20.829949 bentoctl-0.3.4/bentoctl/operator/__init__.py
--rw-r--r--   0        0        0      481 2022-07-18 06:28:00.662787 bentoctl-0.3.4/bentoctl/operator/constants.py
--rw-r--r--   0        0        0     6246 2022-07-15 08:03:28.816598 bentoctl-0.3.4/bentoctl/operator/operator.py
--rw-r--r--   0        0        0     8596 2022-07-18 06:28:00.666787 bentoctl-0.3.4/bentoctl/operator/registry.py
--rw-r--r--   0        0        0     1423 2022-07-21 06:50:49.564216 bentoctl-0.3.4/bentoctl/operator/utils/__init__.py
--rw-r--r--   0        0        0     3635 2022-07-15 08:03:28.816598 bentoctl-0.3.4/bentoctl/operator/utils/github.py
--rw-r--r--   0        0        0      572 2022-07-25 10:24:03.603680 bentoctl-0.3.4/bentoctl/utils/__init__.py
--rw-r--r--   0        0        0      329 2022-07-15 08:03:28.816598 bentoctl-0.3.4/bentoctl/utils/operator_helpers/__init__.py
--rw-r--r--   0        0        0     1225 2022-07-18 06:28:00.666787 bentoctl-0.3.4/bentoctl/utils/operator_helpers/create_deployable.py
--rw-r--r--   0        0        0     2859 2022-07-15 08:03:28.816598 bentoctl-0.3.4/bentoctl/utils/operator_helpers/generate.py
--rw-r--r--   0        0        0      669 2022-07-15 08:03:28.820598 bentoctl-0.3.4/bentoctl/utils/operator_helpers/utils.py
--rw-r--r--   0        0        0     1476 2022-07-15 08:03:28.820598 bentoctl-0.3.4/bentoctl/utils/operator_helpers/values.py
--rw-r--r--   0        0        0     1257 2022-07-19 10:59:52.480768 bentoctl-0.3.4/bentoctl/utils/temp_dir.py
--rw-r--r--   0        0        0     1996 2022-08-25 20:05:25.136570 bentoctl-0.3.4/bentoctl/utils/terraform.py
--rw-r--r--   0        0        0     1438 2022-07-25 10:23:59.117941 bentoctl-0.3.4/bentoctl/utils/usage_stats.py
--rw-r--r--   0        0        0     1766 2022-09-20 12:12:17.391758 bentoctl-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     5571 2022-09-20 12:12:36.952538 bentoctl-0.3.4/setup.py
--rw-r--r--   0        0        0     5559 2022-09-20 12:12:36.952828 bentoctl-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     3875 2023-07-22 05:48:48.064868 bentoctl-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     4840 2023-07-22 05:48:48.064868 bentoctl-0.4.0/README.md
+-rw-r--r--   0        0        0      224 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/__init__.py
+-rw-r--r--   0        0        0    11719 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/cli/__init__.py
+-rw-r--r--   0        0        0    10560 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/cli/interactive.py
+-rw-r--r--   0        0        0     7132 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/cli/operator_management.py
+-rw-r--r--   0        0        0     3902 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/cli/utils.py
+-rw-r--r--   0        0        0     1696 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/console.py
+-rw-r--r--   0        0        0    10920 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/deployment_config.py
+-rw-r--r--   0        0        0     5624 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/docker_utils.py
+-rw-r--r--   0        0        0     5122 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/exceptions.py
+-rw-r--r--   0        0        0     1104 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/operator/README.md
+-rw-r--r--   0        0        0      212 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/operator/__init__.py
+-rw-r--r--   0        0        0      481 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/operator/constants.py
+-rw-r--r--   0        0        0     6246 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/operator/operator.py
+-rw-r--r--   0        0        0     8596 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/operator/registry.py
+-rw-r--r--   0        0        0     1423 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/operator/utils/__init__.py
+-rw-r--r--   0        0        0     3635 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/operator/utils/github.py
+-rw-r--r--   0        0        0      572 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/utils/__init__.py
+-rw-r--r--   0        0        0      329 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/utils/operator_helpers/__init__.py
+-rw-r--r--   0        0        0     1225 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/utils/operator_helpers/create_deployable.py
+-rw-r--r--   0        0        0     2858 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/utils/operator_helpers/generate.py
+-rw-r--r--   0        0        0      833 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/utils/operator_helpers/utils.py
+-rw-r--r--   0        0        0     1764 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/utils/operator_helpers/values.py
+-rw-r--r--   0        0        0     1256 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/utils/temp_dir.py
+-rw-r--r--   0        0        0     2245 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/utils/terraform.py
+-rw-r--r--   0        0        0     1766 2023-07-22 05:48:48.064868 bentoctl-0.4.0/bentoctl/utils/usage_stats.py
+-rw-r--r--   0        0        0     1954 2023-07-22 05:48:57.569513 bentoctl-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      766 2023-07-22 05:48:48.096871 bentoctl-0.4.0/tests/README.md
+-rw-r--r--   0        0        0        0 2023-07-22 05:48:48.096871 bentoctl-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     1849 2023-07-22 05:48:48.096871 bentoctl-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0      597 2023-07-22 05:48:48.096871 bentoctl-0.4.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     1121 2023-07-22 05:48:48.096871 bentoctl-0.4.0/tests/integration/test_service.py
+-rw-r--r--   0        0        0       85 2023-07-22 05:48:48.096871 bentoctl-0.4.0/tests/test-operator/README.md
+-rw-r--r--   0        0        0     2559 2023-07-22 05:48:48.096871 bentoctl-0.4.0/tests/test-operator/operator_config.py
+-rw-r--r--   0        0        0      164 2023-07-22 05:48:48.096871 bentoctl-0.4.0/tests/test-operator/testop/__init__.py
+-rw-r--r--   0        0        0      167 2023-07-22 05:48:48.096871 bentoctl-0.4.0/tests/testbento/bentofile.yaml
+-rw-r--r--   0        0        0      730 2023-07-22 05:48:48.096871 bentoctl-0.4.0/tests/testbento/service.py
+-rw-r--r--   0        0        0      435 2023-07-22 05:48:48.096871 bentoctl-0.4.0/tests/testbento/train.py
+-rw-r--r--   0        0        0        0 2023-07-22 05:48:48.096871 bentoctl-0.4.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     6198 2023-07-22 05:48:48.096871 bentoctl-0.4.0/tests/unit/cli/test_cli_basic.py
+-rw-r--r--   0        0        0     4069 2023-07-22 05:48:48.096871 bentoctl-0.4.0/tests/unit/cli/test_interactive.py
+-rw-r--r--   0        0        0     1210 2023-07-22 05:48:48.096871 bentoctl-0.4.0/tests/unit/operator/test_operator.py
+-rw-r--r--   0        0        0     2490 2023-07-22 05:48:48.096871 bentoctl-0.4.0/tests/unit/operator/test_operator_registry.py
+-rw-r--r--   0        0        0     1256 2023-07-22 05:48:48.096871 bentoctl-0.4.0/tests/unit/operator/test_operator_utils.py
+-rw-r--r--   0        0        0     4928 2023-07-22 05:48:48.096871 bentoctl-0.4.0/tests/unit/test_deployment_config.py
+-rw-r--r--   0        0        0      210 2023-07-22 05:48:48.096871 bentoctl-0.4.0/tests/unit/test_deployment_config.yaml
+-rw-r--r--   0        0        0     5946 1970-01-01 00:00:00.000000 bentoctl-0.4.0/PKG-INFO
```

### Comparing `bentoctl-0.3.4/LICENSE.md` & `bentoctl-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bentoctl-0.3.4/README.md` & `bentoctl-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,67 @@
-<div align="center">
-  <h1>bentoctl</h1>
-  <i>Fast model deployment with BentoML on cloud platforms</i>
-  <p>
-    <img alt="PyPI" src="https://img.shields.io/pypi/v/bentoctl?style=flat-square">
-    <img alt="GitHub branch checks state" src="https://img.shields.io/github/checks-status/bentoml/bentoctl/main?style=flat-square">
-    <img alt="Codecov" src="https://img.shields.io/codecov/c/github/bentoml/bentoctl?style=flat-square">
-</p>
-</div>
-
-<br>
-
-`bentoctl` is a CLI tool for deploying your machine-learning models to any cloud platforms. It built on top of [BentoML: the unified model serving framework](https://github.com/bentoml/BentoML), and makes it easy to bring any BentoML packaged model to production.
-
-👉 [Pop into our Slack community!](https://l.linklyhq.com/l/ktPp) We're happy to help with any issue you face or even just to meet you and hear what you're working on :)
-
-## Features:
-
-* Supports major cloud providers: AWS, Azure, Google Cloud, and more.
-* Easy to deploy, update and reproduce model deployments.
-* First class integration with Terraform.
-* Optimized for CI/CD workflow.
-* Extensible with custom operators.
-* High performance serving powered by [BentoML](https://github.com/bentoml/BentoML)
+# 🚀 Fast model deployment on any cloud
+
+[![actions_status](https://github.com/bentoml/bentoctl/workflows/Bentoctl-CI/badge.svg)](https://github.com/bentoml/yatai/actions)
+[![docs](https://badgen.net/badge/%F0%9F%93%96/Documentation/blue)](https://github.com/bentoml/bentoctl/tree/main/docs)
+[![join_slack](https://badgen.net/badge/Join/Community%20Slack/cyan?icon=slack&style=flat-square)](https://join.slack.bentoml.org)
+
+bentoctl helps deploy any machine learning models as production-ready API endpoints on the cloud, supporting AWS SageMaker, AWS Lambda, EC2, Google Compute Engine, Azure, Heroku and more.
+
+👉 [Join our Slack community today!](https://l.bentoml.com/join-slack)
+
+✨ Looking deploy your ML service quickly? You can checkout [BentoML Cloud](https://www.bentoml.com/bentoml-cloud/)
+for the easiest and fastest way to deploy your bento. It's a full featured, serverless environment with a model repository and built in monitoring and logging.
+
+
+## Highlights
+
+* Framework-agnostic model deployment for Tensorflow, PyTorch, XGBoost, Scikit-Learn, ONNX, and many more via
+ [BentoML: the unified model serving framework](https://github.com/bentoml/bentoml).
+* Simplify the deployment lifecycle of deploy, update, delete, and rollback.
+* Take full advantage of BentoML's performance optimizations and cloud platform features out-of-the-box.
+* Tailor bentoctl to your DevOps needs by customizing deployment operator and Terraform templates.
+
+
+## Getting Started
+
+- [💻 Quickstart Guide](./docs/quickstart.md) - Deploy your first model to AWS Lambda as a serverless API endpoint.
+- [📖 Core Concepts](./docs/core-concepts.md) - Learn the core concepts in bentoctl.
+- [🕹️ Operators List](./docs/operator-list.md) - List of official operators and advanced configuration options.
+- [💬 Join Community Slack](https://l.linklyhq.com/l/ktPp) - Get help from our community and maintainers.
+
 
 ## Supported Platforms:
 
 * [AWS Lambda](https://github.com/bentoml/aws-lambda-deploy)
 * [AWS SageMaker](https://github.com/bentoml/aws-sagemaker-deploy)
 * [AWS EC2](https://github.com/bentoml/aws-ec2-deploy)
 * [Google Cloud Run](https://github.com/bentoml/google-cloud-run-deploy)
 * [Google Compute Engine](https://github.com/bentoml/google-compute-engine-deploy)
 * [Azure Container Instances](https://github.com/bentoml/azure-container-instances-deploy)
 * [Heroku](https://github.com/bentoml/heroku-deploy)
-* Looking for **Kubernetes**? Try out [Yatai: Model deployment at scale on Kubernetes](https://github.com/bentoml/Yatai).
-* **Customize deploy target** by creating bentoctl plugin from the [deployment operator template](https://github.com/bentoml/bentoctl-operator-template).
 
-**Upcoming:**
+### Upcoming
 * [Azure Functions](https://github.com/bentoml/azure-functions-deploy)
-* [Knative](https://github.com/bentoml/bentoctl/issues/79)
 
+### Custom Operator
 
-## Install bentoctl
-```bash
-pip install bentoctl
-```
+Users can built custom bentoctl plugin from the [deployment operator template](https://github.com/bentoml/bentoctl-operator-template)
+to deploy to cloud platforms not yet supported or to internal infrastructure.
 
-| 💡 bentoctl designed to work with BentoML version 1.0.0 and above. For BentoML 0.13 or below, you can use the `pre-v1.0` branch in the operator repositories and follow the instruction in the README. You can also check out the quickstart guide for 0.13 [here](./docs/013-deployment.md).
+If you are looking for deploying with **Kubernetes**, check out [Yatai: Model deployment at scale on Kubernetes](https://github.com/bentoml/Yatai).
 
 
+## Installation
 
+```bash
+pip install bentoctl
+```
 
-## Next steps
+| 💡 bentoctl designed to work with BentoML version 1.0.0 and above. For BentoML 0.13 or below, you can use the `pre-v1.0` branch in the operator repositories and follow the instruction in the README. You can also check out the quickstart guide for 0.13 [here](./docs/013-deployment.md).
 
-- [Quickstart Guide](./docs/quickstart.md) walks through a series of steps to deploy a bento to AWS Lambda as API server.
-- [Core Concepts](./docs/core-concepts.md) explains the core concepts in bentoctl.
-- [Operator List](./docs/operator-list.md) lists official operators and their current status.
 
 ## Community
 
 - To report a bug or suggest a feature request, use [GitHub Issues](https://github.com/bentoml/bentoctl/issues/new/choose).
 - For other discussions, use [Github Discussions](https://github.com/bentoml/BentoML/discussions) under the [BentoML repo](https://github.com/bentoml/BentoML/)
 - To receive release announcements and get support, join us on [Slack](http://join.slack.bentoml.org).
 
@@ -80,7 +83,11 @@
 never collect user code, model data, model names, or stack traces. Here's the
 [code](./bentoctl/utils/usage_stats.py) for usage tracking. You can opt-out of
 usage tracking by setting environment variable `BENTOML_DO_NOT_TRACK=True`:
 
 ```bash
 export BENTOML_DO_NOT_TRACK=True
 ```
+
+## Licence
+
+[Elastic License 2.0 (ELv2)](https://github.com/bentoml/bentoctl/blob/main/LICENSE.md)
```

### Comparing `bentoctl-0.3.4/bentoctl/cli/interactive.py` & `bentoctl-0.4.0/bentoctl/cli/interactive.py`

 * *Files 6% similar despite different names*

```diff
@@ -164,23 +164,42 @@
             )
         if not input_value:
             input_value = None
     elif rule.get("type") == "dict":
         input_value = {}
         if not belongs_to_list:
             indented_print(f"{field_name}:", indent_level)
-            for key in rule.get("schema").keys():
-                input_value[key] = prompt_input(
-                    key, rule.get("schema").get(key), indent_level + 1
-                )
+            if "schema" in rule:
+                for key in rule["schema"].keys():
+                    input_value[key] = prompt_input(
+                        key, rule["schema"].get(key, {}), indent_level + 1
+                    )
+            else:
+                # We don't have a schema so this is a dict with arbitrary keys.
+                help_message = rule.get("help_message")
+                with display_console_message(PromptMsg(help_message, None)):
+                    should_add_item_to_dict = prompt_confirmation(
+                        f"Do you want to add item to {field_name}"
+                    )
+                while should_add_item_to_dict:
+                    key = prompt_input_value("key", rule.get("keysrules", {}))
+                    value = prompt_input_value("value", rule.get("valuesrules", {}))
+                    display_input_result = f"{key}: {value}"
+                    indented_print(display_input_result, indent_level=indent_level + 1)
+                    input_value[key] = value
+
+                    with display_console_message(PromptMsg(help_message, None)):
+                        should_add_item_to_dict = prompt_confirmation(
+                            f"Do you want to add item to {field_name}"
+                        )
         else:
-            for i, key in enumerate(rule.get("schema").keys()):
+            for i, key in enumerate(rule["schema"].keys()):
                 input_value[key] = prompt_input(
                     key,
-                    rule.get("schema").get(key),
+                    rule["schema"].get(key, {}),
                     indent_level,
                     belongs_to_list,
                     i == 0,  # require display '-' for first item of a dict
                 )
         input_value = dict((k, v) for k, v in input_value.items() if v is not None)
     else:
         input_value = prompt_input_value(field_name, rule)
@@ -272,8 +291,11 @@
     deployment_config["template"] = template_name
     console.print(f"[b]template:[/] {template_name}")
 
     console.print("[bold]spec: [/]")
     spec = generate_spec(operator.schema)
     deployment_config["spec"] = dict(spec)
 
+    env = prompt_input("[b]env", deployment_config_schema.get("env"), indent_level=0)
+    deployment_config["env"] = dict(env)
+
     return DeploymentConfig(deployment_config)
```

### Comparing `bentoctl-0.3.4/bentoctl/cli/operator_management.py` & `bentoctl-0.4.0/bentoctl/cli/operator_management.py`

 * *Files identical despite different names*

### Comparing `bentoctl-0.3.4/bentoctl/cli/utils.py` & `bentoctl-0.4.0/bentoctl/cli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import functools
 import os
 import sys
 import time
 
 import click
```

### Comparing `bentoctl-0.3.4/bentoctl/console.py` & `bentoctl-0.4.0/bentoctl/console.py`

 * *Files identical despite different names*

### Comparing `bentoctl-0.3.4/bentoctl/deployment_config.py` & `bentoctl-0.4.0/bentoctl/deployment_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import copy
 import logging
 import os
 import typing as t
+from contextlib import contextmanager
 from pathlib import Path
 
 import bentoml
 import cerberus
 import fs
+import fs.mirror
 import yaml
-from bentoml._internal.bento import Bento
+from bentoml import Bento
 from bentoml.exceptions import NotFound
+from bentoml.models import get as get_model
 
 from bentoctl.exceptions import (
     BentoNotFound,
     DeploymentConfigNotFound,
     InvalidDeploymentConfig,
     OperatorNotFound,
 )
@@ -50,30 +53,52 @@
         "required": True,
         "default": "terraform",
         "help_message": "The template type for generated deployment",
     },
     "spec": {
         "required": True,
     },
+    "env": {
+        "required": False,
+        "nullable": True,
+        "type": "dict",
+        "keysrules": {
+            "type": "string",
+            "regex": "[a-zA-Z_]{1,}[a-zA-Z0-9_]{0,}",
+            "help_message": "An environment variable name to set for deployment",
+        },
+        "valuesrules": {
+            "type": "string",
+            "help_message": "An environment variable value to set for deployment",
+        },
+        "help_message": "Used to set runtime environment variables for deployment",
+    },
 }
 
 
 def remove_help_message(schema):
     """
-    Remove the help_messages in the validation dict.
+    Recursively remove the help_messages from the cerberus schema
     """
     for field, rules in schema.items():
+        if not isinstance(rules, dict):
+            continue
+
         if "help_message" in rules:
             del rules["help_message"]
         if rules.get("type") == "dict":
-            rules["schema"] = remove_help_message(rules.get("schema"))
+            if "schema" in rules:
+                rules["schema"] = remove_help_message(rules.get("schema"))
+            for key in ("keysrules", "valuesrules"):
+                if key in rules:
+                    rules[key] = remove_help_message({key: rules[key]})[key]
         elif rules.get("type") == "list":
-            rules["schema"] = remove_help_message({"list_item": rules.get("schema")})[
-                "list_item"
-            ]
+            rules["schema"] = remove_help_message(
+                {"list_item": rules.get("schema", {})}
+            )["list_item"]
         schema[field] = rules
     return schema
 
 
 def get_bento_metadata(bento_path: str) -> dict:
     metadata = {}
 
@@ -99,14 +124,15 @@
         if not deployment_config.get("api_version") == "v1":
             raise InvalidDeploymentConfig("api_version should be 'v1'.")
 
         self.deployment_config = deployment_config
         self._set_name()
         self._set_operator()
         self._set_template_type()
+        self._set_env()
         self._set_operator_spec()
 
     def _set_name(self):
         self.deployment_name = self.deployment_config.get("name")
         self.repository_name = self.deployment_name
         if self.deployment_name is None:
             raise InvalidDeploymentConfig("name not found")
@@ -139,22 +165,42 @@
                 (
                     f"template '{self.template_type}' not supported by operator "
                     f"{self.operator_name}. Available template types are "
                     f"{self.operator.available_templates}."
                 )
             )
 
+    def _set_env(self):
+        copied_env = copy.deepcopy(self.deployment_config.get("env"))
+        validated_env = None
+        if copied_env is not None:
+            v = cerberus.Validator()
+            env_schema = remove_help_message(
+                {"env": copy.deepcopy(deployment_config_schema["env"])}
+            )
+            validated_env = v.validated({"env": copied_env}, env_schema)["env"]
+            if validated_env is None:
+                raise InvalidDeploymentConfig(config_errors=v.errors)
+        self.env = validated_env
+
     def _set_operator_spec(self):
         # cleanup operator_schema by removing 'help_message' field
         operator_schema = remove_help_message(schema=self.operator.schema)
         copied_operator_spec = copy.deepcopy(self.deployment_config["spec"])
         v = cerberus.Validator()
         validated_spec = v.validated(copied_operator_spec, schema=operator_schema)
         if validated_spec is None:
             raise InvalidDeploymentConfig(config_errors=v.errors)
+
+        # We add `env` through the operator spec to avoid introducing an
+        # additional argument to every operator which would be a breaking change.
+        # TODO: introduce the breaking change to clean up the interface.
+        if self.env is not None:
+            validated_spec["env"] = self.env
+
         self.operator_spec = validated_spec
 
     def set_bento(self, bento_tag: str):
         try:
             self.bento = bentoml.get(bento_tag)
         except NotFound as e:
             raise BentoNotFound(bento_tag) from e
@@ -194,31 +240,48 @@
             template_type=self.template_type,
             destination_dir=destination_dir,
             values_only=values_only,
         )
 
         return generated_files
 
+    @contextmanager
+    def _prepare_bento_dir(self) -> t.Generator[str, None, None]:
+        assert self.bento is not None
+        with fs.open_fs("temp://") as temp_fs, fs.open_fs(self.bento.path) as bento_fs:
+            fs.mirror.mirror(bento_fs, temp_fs)
+            models_fs = temp_fs.makedirs("models", recreate=True)
+            for model_info in self.bento.info.models:
+                model = get_model(model_info.tag)
+                model_fs = models_fs.makedirs(model_info.tag.path())
+                fs.mirror.mirror(model.path, model_fs)
+            yield temp_fs.getsyspath("/")
+
     def create_deployable(self, destination_dir=os.curdir) -> str:
         """
         Creates the deployable in the destination_dir and returns
         the docker args for building
         """
         # NOTE: In the case of debug mode, we want to keep the deployable
         # for debugging purpose. So by setting overwrite_deployable to false,
         # we don't delete the deployable after the build.
-        return self.operator.create_deployable(
-            bento_path=self.bento.path,
-            destination_dir=destination_dir,
-            bento_metadata=get_bento_metadata(self.bento.path),
-            overwrite_deployable=not is_debug_mode(),
-        )
+        with self._prepare_bento_dir() as bento_path:
+            return self.operator.create_deployable(
+                bento_path=bento_path,
+                destination_dir=destination_dir,
+                bento_metadata=get_bento_metadata(bento_path),
+                overwrite_deployable=not is_debug_mode(),
+            )
 
     def create_repository(self):
-        (repository_url, username, password,) = self.operator.create_repository(
+        (
+            repository_url,
+            username,
+            password,
+        ) = self.operator.create_repository(
             repository_name=self.repository_name,
             operator_spec=self.operator_spec,
         )
         return repository_url, username, password
 
     def delete_repository(self):
         return self.operator.delete_repository(self.repository_name, self.operator_spec)
```

### Comparing `bentoctl-0.3.4/bentoctl/docker_utils.py` & `bentoctl-0.4.0/bentoctl/docker_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from __future__ import annotations
+
+import typing as t
 from collections import OrderedDict
 
 import docker
-from bentoml._internal.utils import buildx
+from bentoml import container
 from rich.live import Live
 
 from bentoctl.console import console
 from bentoctl.deployment_config import DeploymentConfig
 from bentoctl.exceptions import BentoctlDockerException
 from bentoctl.utils.temp_dir import TempDirectory
 
@@ -47,60 +50,78 @@
                 f"{layer_id}: {line.get('status')} {line.get('progress_str')}"
             )
 
         yield "\n".join(progress_table)
 
 
 def generate_deployable_container(
-    tag: str, deployment_config: DeploymentConfig, cleanup: bool
+    tags: list[str],
+    deployment_config: DeploymentConfig,
+    cleanup: bool,
+    allow: list[str],
+    build_args: dict[str, str],
+    build_context: dict[str, str],
+    builder: str,
+    cache_from: list[str],
+    cache_to: list[str],
+    load: bool,
+    no_cache: bool,
+    output: dict[str, str] | None,
+    platform: list[str],
+    progress: t.Literal["auto", "tty", "plain"],
+    pull: bool,
+    push: bool,
+    target: str,
 ):
     with TempDirectory(cleanup=cleanup) as dist_dir:
         if cleanup is False:
             # --debug flag is passed. show the path for the saved deployable
             console.print(
                 f"In debug mode. Intermediate bento saved to [b]{dist_dir}[/b]"
             )
-        env = {"DOCKER_BUILDKIT": "1", "DOCKER_SCAN_SUGGEST": "false"}
         buildx_args = {
-            "subprocess_env": env,
-            "cwd": deployment_config.create_deployable(destination_dir=str(dist_dir)),
+            "context_path": deployment_config.create_deployable(
+                destination_dir=str(dist_dir)
+            ),
             "file": DOCKERFILE_PATH,
-            "tags": tag,
+            "tag": tags,
             "add_host": None,
-            "allow": None,
-            "build_args": None,
-            "build_context": None,
-            "builder": None,
-            "cache_from": None,
-            "cache_to": None,
+            "allow": allow,
+            "build_args": build_args,
+            "build_context": build_context,
+            "builder": builder,
+            "cache_from": cache_from,
+            "cache_to": cache_to,
             "cgroup_parent": None,
             "iidfile": None,
             "labels": None,
-            "load": True,  # loading built container to local registry.
+            "load": load,  # loading built container to local registry.
             "metadata_file": None,
             "network": None,
-            "no_cache": False,
+            "no_cache": no_cache,
             "no_cache_filter": None,
-            "output": None,
-            "platform": "linux/amd64",
-            "progress": "auto",
-            "pull": False,
-            "push": False,
+            "output": output,
+            "platform": platform,
+            "progress": progress,
+            "pull": pull,
+            "push": push,
             "quiet": False,
             "secrets": None,
             "shm_size": None,
             "rm": False,
             "ssh": None,
-            "target": None,
+            "target": target,
             "ulimit": None,
         }
+        buildx_args = {k: v or None for k, v in buildx_args.items()}
 
         # run health check whether buildx is install locally
-        buildx.health()
-        buildx.build(**buildx_args)
+        container.health("buildx")
+        backend = container.get_backend("buildx")
+        backend.build(**buildx_args)
 
 
 def tag_docker_image(image_name, image_tag):
     docker_client = docker.from_env()
     try:
         img = docker_client.images.get(image_name)
         was_tagged = img.tag(image_tag)
```

### Comparing `bentoctl-0.3.4/bentoctl/exceptions.py` & `bentoctl-0.4.0/bentoctl/exceptions.py`

 * *Files identical despite different names*

### Comparing `bentoctl-0.3.4/bentoctl/operator/README.md` & `bentoctl-0.4.0/bentoctl/operator/README.md`

 * *Files identical despite different names*

### Comparing `bentoctl-0.3.4/bentoctl/operator/operator.py` & `bentoctl-0.4.0/bentoctl/operator/operator.py`

 * *Files identical despite different names*

### Comparing `bentoctl-0.3.4/bentoctl/operator/registry.py` & `bentoctl-0.4.0/bentoctl/operator/registry.py`

 * *Files identical despite different names*

### Comparing `bentoctl-0.3.4/bentoctl/operator/utils/__init__.py` & `bentoctl-0.4.0/bentoctl/operator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bentoctl-0.3.4/bentoctl/operator/utils/github.py` & `bentoctl-0.4.0/bentoctl/operator/utils/github.py`

 * *Files identical despite different names*

### Comparing `bentoctl-0.3.4/bentoctl/utils/__init__.py` & `bentoctl-0.4.0/bentoctl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bentoctl-0.3.4/bentoctl/utils/operator_helpers/create_deployable.py` & `bentoctl-0.4.0/bentoctl/utils/operator_helpers/create_deployable.py`

 * *Files identical despite different names*

### Comparing `bentoctl-0.3.4/bentoctl/utils/operator_helpers/generate.py` & `bentoctl-0.4.0/bentoctl/utils/operator_helpers/generate.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         return template_file
 
     def generate_terraform_template(self, _, destination_dir: str):
         return self.copy_template("terraform_default", destination_dir)
 
     @staticmethod
     def generate_terraform_values(name: str, spec: dict, destination_dir: str):
-
         params = DeploymentValues(name, spec, "terraform")
         values_file = os.path.join(destination_dir, TERRAFORM_VALUES_FILE_NAME)
         params.to_params_file(values_file)
 
         return values_file
 
     def __call__(
```

### Comparing `bentoctl-0.3.4/bentoctl/utils/operator_helpers/values.py` & `bentoctl-0.4.0/bentoctl/utils/operator_helpers/values.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from collections import UserDict
 
 DEPLOYMENT_PARAMS_WARNING = """# This file is maintained automatically by
 # "bentoctl generate" and "bentoctl build" commands.
 # Manual edits may be lost the next time these commands are run.
 
 """
@@ -31,13 +32,19 @@
     @classmethod
     def from_params_file(cls, file_path):
         pass
 
     def generate_terraform_tfvars_file(self, file_path):
         params = []
         for param_name, param_value in self.items():
-            params.append(f'{param_name} = "{param_value}"')
+            if isinstance(param_value, (dict, list)):
+                write_value = json.dumps(param_value)
+            elif isinstance(param_value, bool):
+                write_value = str(param_value).lower()
+            else:
+                write_value = f'"{param_value}"'
+            params.append(f"{param_name} = {write_value}")
 
         with open(file_path, "w", encoding="utf-8") as params_file:
             params_file.write(DEPLOYMENT_PARAMS_WARNING)
             params_file.write("\n".join(params))
             params_file.write("\n")
```

### Comparing `bentoctl-0.3.4/bentoctl/utils/temp_dir.py` & `bentoctl-0.4.0/bentoctl/utils/temp_dir.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     """
 
     def __init__(
         self,
         cleanup=True,
         prefix="temp",
     ):
-
         self._cleanup = cleanup
         self._prefix = prefix
         self.path = None
 
     def __repr__(self):
         return "<{} {!r}>".format(self.__class__.__name__, self.path)
```

### Comparing `bentoctl-0.3.4/bentoctl/utils/terraform.py` & `bentoctl-0.4.0/bentoctl/utils/terraform.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,35 +23,49 @@
     except FileNotFoundError:
         raise BentoctlException(
             "terraform not available. Please make "
             "sure terraform is installed and available your path."
         )
 
 
-def terraform_destroy():
+def terraform_destroy(auto_approve):
     if not is_terraform_initialised():
         raise BentoctlException("terraform is not initialised")
     if not os.path.exists(os.path.join(os.curdir, TERRAFORM_VALUES_FILE)):
         raise BentoctlException(
             f"{TERRAFORM_VALUES_FILE} not found in current directory."
         )
-    terraform_run(
-        ["apply", "-destroy", "-var-file", TERRAFORM_VALUES_FILE, "-auto-approve"]
-    )
+
+    terraform_cmd = [
+        "apply",
+        "-destroy",
+        "-var-file",
+        TERRAFORM_VALUES_FILE,
+    ]
+    if auto_approve:
+        terraform_cmd.append("-auto-approve")
+    terraform_run(terraform_cmd)
 
 
 def is_terraform_initialised():
     return os.path.exists(os.path.join(os.curdir, TERRAFORM_INIT_FOLDER))
 
 
-def terraform_apply():
+def terraform_apply(auto_approve):
     if not is_terraform_initialised():
         terraform_run(["init"])
 
-    terraform_run(["apply", "-var-file", TERRAFORM_VALUES_FILE, "-auto-approve"])
+    terraform_cmd = [
+        "apply",
+        "-var-file",
+        TERRAFORM_VALUES_FILE,
+    ]
+    if auto_approve:
+        terraform_cmd.append("-auto-approve")
+    terraform_run(terraform_cmd)
 
 
 def terraform_output():
     return_code, result, error = terraform_run(["output", "-json"], return_output=True)
     if return_code != 0:
         raise BentoctlException(error)
     return json.loads(result)
```

### Comparing `bentoctl-0.3.4/bentoctl/utils/usage_stats.py` & `bentoctl-0.4.0/bentoctl/utils/usage_stats.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,33 @@
+import os
 import typing as t
+from functools import lru_cache
 
 import attr
 
-# These are internal apis. We will need to make sure update these when BentoML changes.
+# These are internal apis. We will need to make sure update these when BentoML changes
 from bentoml._internal.utils.analytics.schemas import EventMeta
 from bentoml._internal.utils.analytics.usage_stats import (  # noqa pylint: disable=unused-import
     BENTOML_DO_NOT_TRACK,
-    do_not_track,
     track,
 )
 
 from bentoctl import __version__
 from bentoctl.deployment_config import DeploymentConfig
 
 
+@lru_cache(maxsize=1)
+def do_not_track() -> bool:  # pragma: no cover
+    """
+    Returns True if and only if the environment variable is defined and has value True.
+    The function is cached for better performance.
+    """
+    return os.environ.get(BENTOML_DO_NOT_TRACK, str(False)).lower() == "true"
+
+
 @attr.define
 class BentoctlCliEvent(EventMeta):
     cmd_group: str
     cmd_name: str
     duration_in_ms: t.Optional[t.Any] = attr.field(default=None)
     error_type: t.Optional[str] = attr.field(default=None)
     return_code: t.Optional[int] = attr.field(default=None)
```

### Comparing `bentoctl-0.3.4/pyproject.toml` & `bentoctl-0.4.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,73 +1,88 @@
-[tool.poetry]
+[build-system]
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
+
+[project]
 name = "bentoctl"
-version = "0.3.4"
 description = "Fast model deployment with BentoML on cloud platforms."
-authors = ["bentoml.org <contact@bentoml.com>"]
-homepage = "https://github.com/bentoml/bentoctl"
-readme = "./README.md"
-license = "Apache-2.0"
+authors = [
+    { name = "bentoml.org", email = "contact@bentoml.com" },
+]
+requires-python = ">=3.8,<4.0"
+dependencies = [
+    "bentoml>=1.0.24,<2",
+    "click>=8",
+    "cerberus<2,>=1",
+    "rich==12.*",
+    "PYYAML>=6",
+    "simple-term-menu==0.4.4",
+    "docker>=5",
+    "semantic-version<3.0.0,>=2.9.0",
+]
+readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development",
 ]
+dynamic = []
+version = "0.4.0"
 
-[tool.poetry.scripts]
-bentoctl = "bentoctl.cli:bentoctl"
+[project.license]
+text = "Apache-2.0"
 
-[tool.poetry.urls]
-"Source" =  "https://github.com/bentoml/bentoctl"
+[project.urls]
+Source = "https://github.com/bentoml/bentoctl"
 "User Slack community" = "http://join.slack.bentoml.org"
 "Bug Reports" = "https://github.com/bentoml/bentoctl/issues"
+Homepage = "https://github.com/bentoml/bentoctl"
 
-[tool.poetry.dependencies]
-python = "^3.7"
-bentoml = "1.*"
-click = "^8"
-cerberus = "^1"
-rich = ""
-PyYaml = "^6"
-simple-term-menu = "0.4.4"
-importlib-metadata = { version = "", python = "<3.8" }
-docker = "^5"
-semantic_version = "^2.9.0"
-
-[tool.poetry.dev-dependencies]
-flake8 = "^3.8.2"
-pylint = "^2.6.2"
-black = "*"
-isort = "^5"
-pytest = "^6"
-pytest-cov = "^3"
+[project.scripts]
+bentoctl = "bentoctl.cli:bentoctl"
 
 [tool.isort]
 profile = "black"
 
 [tool.black]
 line-length = 88
-target-version = ["py37", "py38", "py39", "py310"]
-include = '\.pyi?$'
-exclude = '''
-/(
-    \.git
-  | \.hg
-  | \.mypy_cache
-  | \.tox
-  | \.venv
-  | _build
-  | buck-out
-  | build
-  | dist
-)/
-'''
+target-version = [
+    "py38",
+    "py39",
+    "py310",
+    "py311",
+]
+include = "\\.pyi?$"
+exclude = "/(\n    \\.git\n  | \\.hg\n  | \\.mypy_cache\n  | \\.tox\n  | \\.venv\n  | _build\n  | buck-out\n  | build\n  | dist\n)/\n"
 
-[tool.pytest.ini_options]
-asyncio_mode="strict"
+[tool.pdm.dev-dependencies]
+dev = [
+    "flake8>=3.8.2",
+    "black",
+    "isort>=5",
+    "pytest>=7",
+    "pytest-cov>=3",
+]
 
-[build-system]
-# Use the latest poetry build system to enable the use of `pip install -e`. After this change is released, we can switch back to "poetry_core>=1.0.0"
-requires = ["poetry-core @ git+https://github.com/python-poetry/poetry-core.git@master"]
-build-backend = "poetry.core.masonry.api"
+[tool.pdm.build]
+includes = [
+    "bentoctl",
+]
+
+[tool.pdm.version]
+source = "scm"
+
+[tool.pdm.scripts]
+format = "black -S ."
+test = "pytest tests/unit --cov=bentoctl --cov-config=.coveragerc --cov-report=xml:unit.xml"
+
+[tool.pdm.scripts.lint]
+shell = "black -S --check . && flake8 ."
+
+[tool.pytest.ini_options]
+asyncio_mode = "strict"
```

### Comparing `bentoctl-0.3.4/setup.py` & `bentoctl-0.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,121 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: bentoctl
+Version: 0.4.0
+Summary: Fast model deployment with BentoML on cloud platforms.
+Author-Email: bentoml.org <contact@bentoml.com>
+License: Apache-2.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Project-URL: Source, https://github.com/bentoml/bentoctl
+Project-URL: User slack community, http://join.slack.bentoml.org
+Project-URL: Bug reports, https://github.com/bentoml/bentoctl/issues
+Project-URL: Homepage, https://github.com/bentoml/bentoctl
+Requires-Python: <4.0,>=3.8
+Requires-Dist: bentoml<2,>=1.0.24
+Requires-Dist: click>=8
+Requires-Dist: cerberus<2,>=1
+Requires-Dist: rich==12.*
+Requires-Dist: PYYAML>=6
+Requires-Dist: simple-term-menu==0.4.4
+Requires-Dist: docker>=5
+Requires-Dist: semantic-version<3.0.0,>=2.9.0
+Description-Content-Type: text/markdown
 
-packages = \
-['bentoctl',
- 'bentoctl.cli',
- 'bentoctl.operator',
- 'bentoctl.operator.utils',
- 'bentoctl.utils',
- 'bentoctl.utils.operator_helpers']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyYaml>=6,<7',
- 'bentoml>=1.0.0,<2.0.0',
- 'cerberus>=1,<2',
- 'click>=8,<9',
- 'docker>=5,<6',
- 'rich',
- 'semantic_version>=2.9.0,<3.0.0',
- 'simple-term-menu==0.4.4']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib-metadata']}
-
-entry_points = \
-{'console_scripts': ['bentoctl = bentoctl.cli:bentoctl']}
-
-setup_kwargs = {
-    'name': 'bentoctl',
-    'version': '0.3.4',
-    'description': 'Fast model deployment with BentoML on cloud platforms.',
-    'long_description': '<div align="center">\n  <h1>bentoctl</h1>\n  <i>Fast model deployment with BentoML on cloud platforms</i>\n  <p>\n    <img alt="PyPI" src="https://img.shields.io/pypi/v/bentoctl?style=flat-square">\n    <img alt="GitHub branch checks state" src="https://img.shields.io/github/checks-status/bentoml/bentoctl/main?style=flat-square">\n    <img alt="Codecov" src="https://img.shields.io/codecov/c/github/bentoml/bentoctl?style=flat-square">\n</p>\n</div>\n\n<br>\n\n`bentoctl` is a CLI tool for deploying your machine-learning models to any cloud platforms. It built on top of [BentoML: the unified model serving framework](https://github.com/bentoml/BentoML), and makes it easy to bring any BentoML packaged model to production.\n\n👉 [Pop into our Slack community!](https://l.linklyhq.com/l/ktPp) We\'re happy to help with any issue you face or even just to meet you and hear what you\'re working on :)\n\n## Features:\n\n* Supports major cloud providers: AWS, Azure, Google Cloud, and more.\n* Easy to deploy, update and reproduce model deployments.\n* First class integration with Terraform.\n* Optimized for CI/CD workflow.\n* Extensible with custom operators.\n* High performance serving powered by [BentoML](https://github.com/bentoml/BentoML)\n\n## Supported Platforms:\n\n* [AWS Lambda](https://github.com/bentoml/aws-lambda-deploy)\n* [AWS SageMaker](https://github.com/bentoml/aws-sagemaker-deploy)\n* [AWS EC2](https://github.com/bentoml/aws-ec2-deploy)\n* [Google Cloud Run](https://github.com/bentoml/google-cloud-run-deploy)\n* [Google Compute Engine](https://github.com/bentoml/google-compute-engine-deploy)\n* [Azure Container Instances](https://github.com/bentoml/azure-container-instances-deploy)\n* [Heroku](https://github.com/bentoml/heroku-deploy)\n* Looking for **Kubernetes**? Try out [Yatai: Model deployment at scale on Kubernetes](https://github.com/bentoml/Yatai).\n* **Customize deploy target** by creating bentoctl plugin from the [deployment operator template](https://github.com/bentoml/bentoctl-operator-template).\n\n**Upcoming:**\n* [Azure Functions](https://github.com/bentoml/azure-functions-deploy)\n* [Knative](https://github.com/bentoml/bentoctl/issues/79)\n\n\n## Install bentoctl\n```bash\npip install bentoctl\n```\n\n| 💡 bentoctl designed to work with BentoML version 1.0.0 and above. For BentoML 0.13 or below, you can use the `pre-v1.0` branch in the operator repositories and follow the instruction in the README. You can also check out the quickstart guide for 0.13 [here](./docs/013-deployment.md).\n\n\n\n\n## Next steps\n\n- [Quickstart Guide](./docs/quickstart.md) walks through a series of steps to deploy a bento to AWS Lambda as API server.\n- [Core Concepts](./docs/core-concepts.md) explains the core concepts in bentoctl.\n- [Operator List](./docs/operator-list.md) lists official operators and their current status.\n\n## Community\n\n- To report a bug or suggest a feature request, use [GitHub Issues](https://github.com/bentoml/bentoctl/issues/new/choose).\n- For other discussions, use [Github Discussions](https://github.com/bentoml/BentoML/discussions) under the [BentoML repo](https://github.com/bentoml/BentoML/)\n- To receive release announcements and get support, join us on [Slack](http://join.slack.bentoml.org).\n\n\n## Contributing\n\nThere are many ways to contribute to the project:\n\n- Create and share new operators. Use [deployment operator template](https://github.com/bentoml/bentoctl-operator-template) to get started.\n- If you have any feedback on the project, share it with the community in [Github Discussions](https://github.com/bentoml/BentoML/discussions) under the [BentoML repo](https://github.com/bentoml/BentoML/).\n- Report issues you\'re facing and "Thumbs up" on issues and feature requests that are relevant to you.\n- Investigate bugs and reviewing other developer\'s pull requests.\n\n## Usage Reporting\n\nBentoML and bentoctl collects usage data that helps our team to\nimprove the product. Only bentoctl\'s CLI commands calls are being reported. We\nstrip out as much potentially sensitive information as possible, and we will\nnever collect user code, model data, model names, or stack traces. Here\'s the\n[code](./bentoctl/utils/usage_stats.py) for usage tracking. You can opt-out of\nusage tracking by setting environment variable `BENTOML_DO_NOT_TRACK=True`:\n\n```bash\nexport BENTOML_DO_NOT_TRACK=True\n```\n',
-    'author': 'bentoml.org',
-    'author_email': 'contact@bentoml.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/bentoml/bentoctl',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+# 🚀 Fast model deployment on any cloud
 
+[![actions_status](https://github.com/bentoml/bentoctl/workflows/Bentoctl-CI/badge.svg)](https://github.com/bentoml/yatai/actions)
+[![docs](https://badgen.net/badge/%F0%9F%93%96/Documentation/blue)](https://github.com/bentoml/bentoctl/tree/main/docs)
+[![join_slack](https://badgen.net/badge/Join/Community%20Slack/cyan?icon=slack&style=flat-square)](https://join.slack.bentoml.org)
 
-setup(**setup_kwargs)
+bentoctl helps deploy any machine learning models as production-ready API endpoints on the cloud, supporting AWS SageMaker, AWS Lambda, EC2, Google Compute Engine, Azure, Heroku and more.
+
+👉 [Join our Slack community today!](https://l.bentoml.com/join-slack)
+
+✨ Looking deploy your ML service quickly? You can checkout [BentoML Cloud](https://www.bentoml.com/bentoml-cloud/)
+for the easiest and fastest way to deploy your bento. It's a full featured, serverless environment with a model repository and built in monitoring and logging.
+
+
+## Highlights
+
+* Framework-agnostic model deployment for Tensorflow, PyTorch, XGBoost, Scikit-Learn, ONNX, and many more via
+ [BentoML: the unified model serving framework](https://github.com/bentoml/bentoml).
+* Simplify the deployment lifecycle of deploy, update, delete, and rollback.
+* Take full advantage of BentoML's performance optimizations and cloud platform features out-of-the-box.
+* Tailor bentoctl to your DevOps needs by customizing deployment operator and Terraform templates.
+
+
+## Getting Started
+
+- [💻 Quickstart Guide](./docs/quickstart.md) - Deploy your first model to AWS Lambda as a serverless API endpoint.
+- [📖 Core Concepts](./docs/core-concepts.md) - Learn the core concepts in bentoctl.
+- [🕹️ Operators List](./docs/operator-list.md) - List of official operators and advanced configuration options.
+- [💬 Join Community Slack](https://l.linklyhq.com/l/ktPp) - Get help from our community and maintainers.
+
+
+## Supported Platforms:
+
+* [AWS Lambda](https://github.com/bentoml/aws-lambda-deploy)
+* [AWS SageMaker](https://github.com/bentoml/aws-sagemaker-deploy)
+* [AWS EC2](https://github.com/bentoml/aws-ec2-deploy)
+* [Google Cloud Run](https://github.com/bentoml/google-cloud-run-deploy)
+* [Google Compute Engine](https://github.com/bentoml/google-compute-engine-deploy)
+* [Azure Container Instances](https://github.com/bentoml/azure-container-instances-deploy)
+* [Heroku](https://github.com/bentoml/heroku-deploy)
+
+### Upcoming
+* [Azure Functions](https://github.com/bentoml/azure-functions-deploy)
+
+### Custom Operator
+
+Users can built custom bentoctl plugin from the [deployment operator template](https://github.com/bentoml/bentoctl-operator-template)
+to deploy to cloud platforms not yet supported or to internal infrastructure.
+
+If you are looking for deploying with **Kubernetes**, check out [Yatai: Model deployment at scale on Kubernetes](https://github.com/bentoml/Yatai).
+
+
+## Installation
+
+```bash
+pip install bentoctl
+```
+
+| 💡 bentoctl designed to work with BentoML version 1.0.0 and above. For BentoML 0.13 or below, you can use the `pre-v1.0` branch in the operator repositories and follow the instruction in the README. You can also check out the quickstart guide for 0.13 [here](./docs/013-deployment.md).
+
+
+## Community
+
+- To report a bug or suggest a feature request, use [GitHub Issues](https://github.com/bentoml/bentoctl/issues/new/choose).
+- For other discussions, use [Github Discussions](https://github.com/bentoml/BentoML/discussions) under the [BentoML repo](https://github.com/bentoml/BentoML/)
+- To receive release announcements and get support, join us on [Slack](http://join.slack.bentoml.org).
+
+
+## Contributing
+
+There are many ways to contribute to the project:
+
+- Create and share new operators. Use [deployment operator template](https://github.com/bentoml/bentoctl-operator-template) to get started.
+- If you have any feedback on the project, share it with the community in [Github Discussions](https://github.com/bentoml/BentoML/discussions) under the [BentoML repo](https://github.com/bentoml/BentoML/).
+- Report issues you're facing and "Thumbs up" on issues and feature requests that are relevant to you.
+- Investigate bugs and reviewing other developer's pull requests.
+
+## Usage Reporting
+
+BentoML and bentoctl collects usage data that helps our team to
+improve the product. Only bentoctl's CLI commands calls are being reported. We
+strip out as much potentially sensitive information as possible, and we will
+never collect user code, model data, model names, or stack traces. Here's the
+[code](./bentoctl/utils/usage_stats.py) for usage tracking. You can opt-out of
+usage tracking by setting environment variable `BENTOML_DO_NOT_TRACK=True`:
+
+```bash
+export BENTOML_DO_NOT_TRACK=True
+```
+
+## Licence
+
+[Elastic License 2.0 (ELv2)](https://github.com/bentoml/bentoctl/blob/main/LICENSE.md)
```

