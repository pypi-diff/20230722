# Comparing `tmp/balcony-0.1.8.tar.gz` & `tmp/balcony-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balcony-0.1.8.tar", max compression
+gzip compressed data, was "balcony-0.1.9.tar", max compression
```

## Comparing `balcony-0.1.8.tar` & `balcony-0.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.1.8/LICENSE
--rw-r--r--   0        0        0     3851 2023-07-17 18:52:57.338228 balcony-0.1.8/README.md
--rw-r--r--   0        0        0      933 2023-04-29 21:23:00.565222 balcony-0.1.8/balcony/__init__.py
--rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.1.8/balcony/__main__.py
--rw-r--r--   0        0        0     5622 2023-04-21 19:12:44.411429 balcony-0.1.8/balcony/aws.py
--rw-r--r--   0        0        0    15169 2023-06-27 10:41:54.525900 balcony-0.1.8/balcony/botocore_utils.py
--rw-r--r--   0        0        0    22612 2023-07-17 18:22:23.044112 balcony-0.1.8/balcony/cli.py
--rw-r--r--   0        0        0     3723 2023-06-27 12:34:24.543878 balcony-0.1.8/balcony/config.py
--rw-r--r--   0        0        0      488 2023-04-29 22:03:44.770391 balcony-0.1.8/balcony/custom_nodes/__init__.py
--rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.1.8/balcony/custom_nodes/codebuild.py
--rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.1.8/balcony/custom_nodes/ecs.py
--rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.1.8/balcony/custom_nodes/iam.py
--rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.1.8/balcony/custom_nodes/lambda_functions.py
--rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.1.8/balcony/custom_nodes/s3.py
--rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.1.8/balcony/custom_nodes/ses.py
--rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.1.8/balcony/custom_nodes/ssm.py
--rw-r--r--   0        0        0        0 2023-06-18 18:05:04.079497 balcony-0.1.8/balcony/custom_tf_import_configs/_example_import_conf.yaml
--rw-r--r--   0        0        0     2306 2023-07-16 15:42:11.020304 balcony-0.1.8/balcony/custom_tf_import_configs/ec2.yaml
--rw-r--r--   0        0        0      935 2023-07-18 19:25:23.582721 balcony-0.1.8/balcony/custom_tf_import_configs/ecs.yaml
--rw-r--r--   0        0        0     1610 2023-07-17 18:20:28.021261 balcony-0.1.8/balcony/custom_tf_import_configs/iam.yaml
--rw-r--r--   0        0        0     1845 2023-06-27 20:18:18.446771 balcony-0.1.8/balcony/custom_tf_import_configs/rds.yaml
--rw-r--r--   0        0        0      336 2023-06-22 11:23:28.065064 balcony-0.1.8/balcony/custom_tf_import_configs/s3.yaml
--rw-r--r--   0        0        0     4257 2023-07-17 18:18:53.104515 balcony-0.1.8/balcony/custom_tf_import_configs/vpc.yaml
--rw-r--r--   0        0        0     3271 2023-07-18 18:28:06.436858 balcony-0.1.8/balcony/custom_yamls/_example_service.yaml
--rw-r--r--   0        0        0      842 2023-07-16 11:53:29.831094 balcony-0.1.8/balcony/custom_yamls/ec2.yaml
--rw-r--r--   0        0        0     2704 2023-07-18 19:10:24.404655 balcony-0.1.8/balcony/custom_yamls/ecs.yaml
--rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.1.8/balcony/custom_yamls/iam.yaml
--rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.1.8/balcony/custom_yamls/s3.yaml
--rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.1.8/balcony/errors.py
--rw-r--r--   0        0        0    49370 2023-07-18 18:50:11.229744 balcony-0.1.8/balcony/nodes.py
--rw-r--r--   0        0        0    17448 2023-06-27 11:52:38.036399 balcony-0.1.8/balcony/reader.py
--rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.1.8/balcony/registries.py
--rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.1.8/balcony/relations.py
--rw-r--r--   0        0        0        0 2023-06-18 17:41:34.879852 balcony-0.1.8/balcony/terraform_import/__init__.py
--rw-r--r--   0        0        0    10693 2023-07-17 17:11:29.424367 balcony-0.1.8/balcony/terraform_import/importer.py
--rw-r--r--   0        0        0     1320 2023-07-17 16:45:25.594486 balcony-0.1.8/balcony/terraform_import/models.py
--rw-r--r--   0        0        0     3877 2023-07-17 16:46:47.909479 balcony-0.1.8/balcony/terraform_import/parsers.py
--rw-r--r--   0        0        0    16069 2023-06-27 13:47:03.229109 balcony-0.1.8/balcony/terraform_import/wizard.py
--rw-r--r--   0        0        0     2980 2023-06-19 18:24:25.368221 balcony-0.1.8/balcony/test.py
--rw-r--r--   0        0        0     6553 2023-07-07 16:07:51.678302 balcony-0.1.8/balcony/utils.py
--rw-r--r--   0        0        0     2344 2023-07-18 18:43:44.785613 balcony-0.1.8/balcony/yaml_config.py
--rw-r--r--   0        0        0     2124 2023-07-18 18:27:00.154209 balcony-0.1.8/balcony/yaml_validators.py
--rw-r--r--   0        0        0      748 2023-07-18 19:26:08.878958 balcony-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5147 1970-01-01 00:00:00.000000 balcony-0.1.8/setup.py
--rw-r--r--   0        0        0     4957 1970-01-01 00:00:00.000000 balcony-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3965 2023-07-22 10:16:18.349371 balcony-0.1.9/README.md
+-rw-r--r--   0        0        0      933 2023-04-29 21:23:00.565222 balcony-0.1.9/balcony/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.1.9/balcony/__main__.py
+-rw-r--r--   0        0        0     5622 2023-04-21 19:12:44.411429 balcony-0.1.9/balcony/aws.py
+-rw-r--r--   0        0        0    15169 2023-06-27 10:41:54.525900 balcony-0.1.9/balcony/botocore_utils.py
+-rw-r--r--   0        0        0    22612 2023-07-17 18:22:23.044112 balcony-0.1.9/balcony/cli.py
+-rw-r--r--   0        0        0     3723 2023-06-27 12:34:24.543878 balcony-0.1.9/balcony/config.py
+-rw-r--r--   0        0        0      488 2023-04-29 22:03:44.770391 balcony-0.1.9/balcony/custom_nodes/__init__.py
+-rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.1.9/balcony/custom_nodes/codebuild.py
+-rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.1.9/balcony/custom_nodes/ecs.py
+-rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.1.9/balcony/custom_nodes/iam.py
+-rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.1.9/balcony/custom_nodes/lambda_functions.py
+-rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.1.9/balcony/custom_nodes/s3.py
+-rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.1.9/balcony/custom_nodes/ses.py
+-rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.1.9/balcony/custom_nodes/ssm.py
+-rw-r--r--   0        0        0     2306 2023-07-16 15:42:11.020304 balcony-0.1.9/balcony/custom_tf_import_configs/ec2.yaml
+-rw-r--r--   0        0        0      935 2023-07-18 19:25:23.582721 balcony-0.1.9/balcony/custom_tf_import_configs/ecs.yaml
+-rw-r--r--   0        0        0     4728 2023-07-22 11:34:28.352856 balcony-0.1.9/balcony/custom_tf_import_configs/iam.yaml
+-rw-r--r--   0        0        0     2015 2023-07-22 14:31:51.087927 balcony-0.1.9/balcony/custom_tf_import_configs/lambda.yaml
+-rw-r--r--   0        0        0     1845 2023-06-27 20:18:18.446771 balcony-0.1.9/balcony/custom_tf_import_configs/rds.yaml
+-rw-r--r--   0        0        0     6175 2023-07-22 15:35:18.928011 balcony-0.1.9/balcony/custom_tf_import_configs/s3.yaml
+-rw-r--r--   0        0        0     4257 2023-07-17 18:18:53.104515 balcony-0.1.9/balcony/custom_tf_import_configs/vpc.yaml
+-rw-r--r--   0        0        0     3271 2023-07-18 18:28:06.436858 balcony-0.1.9/balcony/custom_yamls/_example_service.yaml
+-rw-r--r--   0        0        0      842 2023-07-16 11:53:29.831094 balcony-0.1.9/balcony/custom_yamls/ec2.yaml
+-rw-r--r--   0        0        0     2704 2023-07-18 19:10:24.404655 balcony-0.1.9/balcony/custom_yamls/ecs.yaml
+-rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.1.9/balcony/custom_yamls/iam.yaml
+-rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.1.9/balcony/custom_yamls/s3.yaml
+-rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.1.9/balcony/errors.py
+-rw-r--r--   0        0        0    49314 2023-07-22 10:13:58.426856 balcony-0.1.9/balcony/nodes.py
+-rw-r--r--   0        0        0    17434 2023-07-22 10:14:21.080169 balcony-0.1.9/balcony/reader.py
+-rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.1.9/balcony/registries.py
+-rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.1.9/balcony/relations.py
+-rw-r--r--   0        0        0        0 2023-06-18 17:41:34.879852 balcony-0.1.9/balcony/terraform_import/__init__.py
+-rw-r--r--   0        0        0    10761 2023-07-22 10:49:58.891484 balcony-0.1.9/balcony/terraform_import/importer.py
+-rw-r--r--   0        0        0     1320 2023-07-17 16:45:25.594486 balcony-0.1.9/balcony/terraform_import/models.py
+-rw-r--r--   0        0        0     3877 2023-07-17 16:46:47.909479 balcony-0.1.9/balcony/terraform_import/parsers.py
+-rw-r--r--   0        0        0    16069 2023-06-27 13:47:03.229109 balcony-0.1.9/balcony/terraform_import/wizard.py
+-rw-r--r--   0        0        0     2980 2023-06-19 18:24:25.368221 balcony-0.1.9/balcony/test.py
+-rw-r--r--   0        0        0     6553 2023-07-07 16:07:51.678302 balcony-0.1.9/balcony/utils.py
+-rw-r--r--   0        0        0     2344 2023-07-18 18:43:44.785613 balcony-0.1.9/balcony/yaml_config.py
+-rw-r--r--   0        0        0     2124 2023-07-18 18:27:00.154209 balcony-0.1.9/balcony/yaml_validators.py
+-rw-r--r--   0        0        0      748 2023-07-22 16:31:26.037712 balcony-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5263 1970-01-01 00:00:00.000000 balcony-0.1.9/setup.py
+-rw-r--r--   0        0        0     5071 1970-01-01 00:00:00.000000 balcony-0.1.9/PKG-INFO
```

### Comparing `balcony-0.1.8/LICENSE` & `balcony-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/README.md` & `balcony-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -74,22 +74,24 @@
 ![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-import-blocks-example.gif)
 
 
 ---
 
 ### Generate actual Terraform Resource Code 
 
+
 If you have:
 
 - initialized terraform project
 - `import_blocks.tf` file that's generated with `balcony terraform-import` command
 
 you can run `terraform plan -generate-config-out=generated.tf` to generate actual `.tf` resource code.
 
-This feature is achieved with a Docker image.
+This feature is achieved with the [balcony-terraform-import Docker Image](https://github.com/oguzhan-yilmaz/balcony/pkgs/container/balcony-terraform-import).
+
 
 Related Docs: [Generate Terraform Code with Docker Image](https://oguzhan-yilmaz.github.io/balcony/terraform-import-docker/)
 
 ![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/docker-gen-tf-code-ec2-insances-example.gif)
 
 
 ---
```

#### html2text {}

```diff
@@ -25,20 +25,22 @@
 supported resources. Related Docs: [Generate Terraform Import Blocks](https://
 oguzhan-yilmaz.github.io/balcony/terraform-import/) ![](https://
 raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-
 import-blocks-example.gif) --- ### Generate actual Terraform Resource Code If
 you have: - initialized terraform project - `import_blocks.tf` file that's
 generated with `balcony terraform-import` command you can run `terraform plan -
 generate-config-out=generated.tf` to generate actual `.tf` resource code. This
-feature is achieved with a Docker image. Related Docs: [Generate Terraform Code
-with Docker Image](https://oguzhan-yilmaz.github.io/balcony/terraform-import-
-docker/) ![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/
-main/gifs/docker-gen-tf-code-ec2-insances-example.gif) --- ### Interactive
-Wizard to create balcony import configurations Balcony doesn't know how to
-create terraform `import blocks` for all of the AWS resources. It can be taught
-how to do it by creating `import-configurations` yaml files, but it's a manual
-process. This is where the interactive wizard comes in. Interactive Wizards
-asks you required questions to automatically create the `import-configurations`
-yaml files. Related Docs: [Terraform Import Configuration Wizard](https://
-oguzhan-yilmaz.github.io/balcony/terraform-import-wizard/) ![](https://
+feature is achieved with the [balcony-terraform-import Docker Image](https://
+github.com/oguzhan-yilmaz/balcony/pkgs/container/balcony-terraform-import).
+Related Docs: [Generate Terraform Code with Docker Image](https://oguzhan-
+yilmaz.github.io/balcony/terraform-import-docker/) ![](https://
+raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/docker-gen-
+tf-code-ec2-insances-example.gif) --- ### Interactive Wizard to create balcony
+import configurations Balcony doesn't know how to create terraform `import
+blocks` for all of the AWS resources. It can be taught how to do it by creating
+`import-configurations` yaml files, but it's a manual process. This is where
+the interactive wizard comes in. Interactive Wizards asks you required
+questions to automatically create the `import-configurations` yaml files.
+Related Docs: [Terraform Import Configuration Wizard](https://oguzhan-
+yilmaz.github.io/balcony/terraform-import-wizard/) ![](https://
 raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-
 wizard-security-groups-example.gif)
```

### Comparing `balcony-0.1.8/balcony/__init__.py` & `balcony-0.1.9/balcony/__init__.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/aws.py` & `balcony-0.1.9/balcony/aws.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/botocore_utils.py` & `balcony-0.1.9/balcony/botocore_utils.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/cli.py` & `balcony-0.1.9/balcony/cli.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/config.py` & `balcony-0.1.9/balcony/config.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/custom_nodes/codebuild.py` & `balcony-0.1.9/balcony/custom_nodes/codebuild.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/custom_nodes/ecs.py` & `balcony-0.1.9/balcony/custom_nodes/ecs.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/custom_nodes/iam.py` & `balcony-0.1.9/balcony/custom_nodes/iam.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/custom_nodes/lambda_functions.py` & `balcony-0.1.9/balcony/custom_nodes/lambda_functions.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/custom_nodes/s3.py` & `balcony-0.1.9/balcony/custom_nodes/s3.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/custom_nodes/ses.py` & `balcony-0.1.9/balcony/custom_nodes/ses.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/custom_nodes/ssm.py` & `balcony-0.1.9/balcony/custom_nodes/ssm.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/custom_tf_import_configs/ec2.yaml` & `balcony-0.1.9/balcony/custom_tf_import_configs/ec2.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/custom_tf_import_configs/ecs.yaml` & `balcony-0.1.9/balcony/custom_tf_import_configs/ecs.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/custom_tf_import_configs/iam.yaml` & `balcony-0.1.9/balcony/custom_tf_import_configs/rds.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,51 @@
 maintainers:
 - name: Oguzhan Yilmaz
-
 import_configurations:
-- id_generator_jinja2_template: '{{ UserName }}'
-  jmespath_query: '[].Users[]'
-  operation_name: ListUsers
-  resource_node: User
-  service: iam
-  to_resource_name_jinja2_template: '{{ UserName }}'
-  to_resource_type: aws_iam_user
-
-- id_generator_jinja2_template: '{{ item }}'
-  jmespath_query: '[].PolicyNames[]'
-  operation_name: ListRolePolicies
-  resource_node: RolePolicy
-  service: iam
-  to_resource_name_jinja2_template: '{{ item }}'
-  to_resource_type: aws_iam_role_policy
-
-- service: iam
-  resource_node: GroupPolicy
-  operation_name: GetGroupPolicy
-  jmespath_query: '[]'
-  to_resource_type: aws_iam_group_policy
-  to_resource_name_jinja2_template: '{{ GroupName ~ '':'' ~ PolicyName }}'
-  id_generator_jinja2_template: '{{ GroupName ~ '':'' ~ PolicyName }}'
-
-- id_generator_jinja2_template: '{{ Arn }}'
-  jmespath_query: '[].Policies[]'
-  operation_name: ListPolicies
-  resource_node: Policy
-  service: iam
-  to_resource_name_jinja2_template: '{{ PolicyName or PolicyId }}'
-  to_resource_type: aws_iam_policy
-
-- id_generator_jinja2_template: '{{ RoleName }}'
-  jmespath_query: '[].Roles[]'
-  operation_name: ListRoles
-  resource_node: Role
-  service: iam
-  to_resource_name_jinja2_template: '{{ ''role-'' ~ RoleName }}'
-  to_resource_type: aws_iam_role
-
-- id_generator_jinja2_template: '{{ UserName ~ '':''  ~ PolicyName }}'
-  jmespath_query: '[]'
-  operation_name: GetUserPolicy
-  resource_node: UserPolicy
-  service: iam
-  to_resource_name_jinja2_template: '{{ UserName ~ ''-'' ~ PolicyName }}'
-  to_resource_type: aws_iam_user_policy
-
-
+- id_generator_jinja2_template: '{{ DBClusterEndpointIdentifier }}'
+  jmespath_query: '[].DBClusterEndpoints[]'
+  operation_name: DescribeDBClusterEndpoints
+  resource_node: DBClusterEndpoints
+  service: rds
+  to_resource_name_jinja2_template: '{{ DBClusterIdentifier ~ ''-'' ~ Endpoint }}'
+  to_resource_type: aws_rds_cluster_endpoint
+
+- id_generator_jinja2_template: '{{ ParameterName }}'
+  jmespath_query: '[].Parameters[]'
+  operation_name: DescribeDBClusterParameters
+  resource_node: DBClusterParameters
+  service: rds
+  to_resource_name_jinja2_template: '{{ ParameterName }}'
+  to_resource_type: aws_db_parameter_group
+
+- id_generator_jinja2_template: '{{ DBClusterIdentifier }}'
+  jmespath_query: '[].DBClusters[]'
+  operation_name: DescribeDBClusters
+  resource_node: DBClusters
+  service: rds
+  to_resource_name_jinja2_template: '{{ DBClusterIdentifier ~ ''-'' ~ DatabaseName
+    }}'
+  to_resource_type: aws_rds_cluster
+
+- id_generator_jinja2_template: '{{ DBInstanceIdentifier }}'
+  jmespath_query: '[].DBInstances[]'
+  operation_name: DescribeDBInstances
+  resource_node: DBInstances
+  service: rds
+  to_resource_name_jinja2_template: '{{ DBName ~ ''-'' ~ Engine }}'
+  to_resource_type: aws_db_instance
+
+- id_generator_jinja2_template: '{{ DBSubnetGroupName }}'
+  jmespath_query: '[].DBSubnetGroups[]'
+  operation_name: DescribeDBSubnetGroups
+  resource_node: DBSubnetGroups
+  service: rds
+  to_resource_name_jinja2_template: '{{ DBSubnetGroupName }}'
+  to_resource_type: aws_db_subnet_group
+
+- id_generator_jinja2_template: '{{ OptionGroupName }}'
+  jmespath_query: '[].OptionGroupsList[]'
+  operation_name: DescribeOptionGroups
+  resource_node: OptionGroups
+  service: rds
+  to_resource_name_jinja2_template: '{{ OptionGroupName }}'
+  to_resource_type: aws_db_option_group
```

### Comparing `balcony-0.1.8/balcony/custom_tf_import_configs/vpc.yaml` & `balcony-0.1.9/balcony/custom_tf_import_configs/vpc.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/custom_yamls/_example_service.yaml` & `balcony-0.1.9/balcony/custom_yamls/_example_service.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/custom_yamls/ec2.yaml` & `balcony-0.1.9/balcony/custom_yamls/ec2.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/custom_yamls/ecs.yaml` & `balcony-0.1.9/balcony/custom_yamls/ecs.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/custom_yamls/iam.yaml` & `balcony-0.1.9/balcony/custom_yamls/iam.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/nodes.py` & `balcony-0.1.9/balcony/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -619,15 +619,14 @@
 
     def get_pagination_token_output_to_parameter_name_mapping(
         self, operation_name: str
     ) -> Union[Dict[str, str], bool]:
         """Some Operations paginate their output using Pagination Token Parameters defined in `PAGINATION_TOKEN_KEYS`.
 
         Args:
-            resource_node (ResourceNode): _description_
             operation_name (str): Name of the operation in the resource_node.
 
         Returns:
             Union[Dict[str, str], bool]: False or A dictionary with `parameter_name` and `output_key` keys. e.g. `{"parameter_name":"nextToken", "output_key": "NextToken"}`.
         """
         resource_node: ResourceNode = self
```

### Comparing `balcony-0.1.8/balcony/reader.py` & `balcony-0.1.9/balcony/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     def call_operation(
         self, resource_node: "ResourceNode", operation_name: str, api_parameter: Dict, follow_pagination : Optional[bool] = False # noqa  
     ) -> Union[dict, bool]:
         """Calls the given AWS operation with `api_parameter` dict.
         Saves the response data on `self.response_data` and returns it.
 
         Args:
-            resource_node(ResourceNode): Operations Resource Node
+            resource_node: Operations Resource Node
             operation_name (str): Name of the operation
             api_parameter (dict): dictionary to call the operation with
             follow_pagination (Optional[bool]): If the operations output is truncated follow the pagination tokens.
 
         Returns:
             Union[dict, bool]: `False` or response got from AWS API
         """
```

### Comparing `balcony-0.1.8/balcony/registries.py` & `balcony-0.1.9/balcony/registries.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/relations.py` & `balcony-0.1.9/balcony/relations.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/terraform_import/importer.py` & `balcony-0.1.9/balcony/terraform_import/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,11 +280,12 @@
         tf_import_blocks = generate_import_block_from_import_config(
             balcony_client, tf_import_config, follow_pagination
         )
         if not tf_import_blocks:
             logger.debug(
                 f"[red bold]No data found for {tf_import_config.to_resource_type} — {tf_import_config.resource_node}.{tf_import_config.operation_name}."
             )
-        resulting_tf_import_blocks.extend(tf_import_blocks)
-    
+
+        if tf_import_blocks and isinstance(tf_import_blocks, list):
+            resulting_tf_import_blocks.extend(tf_import_blocks)
     logger.debug(f"[underline bold][green]Done Generating[/] Terraform import blocks for[/] {operation_markup}.")
     return resulting_tf_import_blocks
```

### Comparing `balcony-0.1.8/balcony/terraform_import/models.py` & `balcony-0.1.9/balcony/terraform_import/models.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/terraform_import/parsers.py` & `balcony-0.1.9/balcony/terraform_import/parsers.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/terraform_import/wizard.py` & `balcony-0.1.9/balcony/terraform_import/wizard.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/test.py` & `balcony-0.1.9/balcony/test.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/utils.py` & `balcony-0.1.9/balcony/utils.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/yaml_config.py` & `balcony-0.1.9/balcony/yaml_config.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/balcony/yaml_validators.py` & `balcony-0.1.9/balcony/yaml_validators.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.8/pyproject.toml` & `balcony-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "balcony"
-version = "0.1.8"
+version = "0.1.9"
 description = "Read any resource in your AWS Account. You can generate terraform code for them, too."
 authors = ["Oguzhan Yilmaz <oguzhanylmz271@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.scripts]
 balcony = "balcony.cli:run_app"
```

### Comparing `balcony-0.1.8/setup.py` & `balcony-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,17 +21,17 @@
  'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['balcony = balcony.cli:run_app']}
 
 setup_kwargs = {
     'name': 'balcony',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Read any resource in your AWS Account. You can generate terraform code for them, too.',
-    'long_description': '# balcony\n\n\n<div style="display: flex;">\n  <a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml/badge.svg" alt="Build and publish a Docker image to ghcr.io"></a>\n  <span style="width: 5px"></span>\n\n<a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment/badge.svg" alt="Build and Deploy Documentation website"></a>\n</div>\n\n\nbalcony is a modern CLI tool that with some killer features:\n\n- Auto-fill the required parameters for AWS API calls \n- Read the JSON data of any AWS resource in your account\n- Generate [Terraform Import Blocks](https://developer.hashicorp.com/terraform/language/import)\n- Generate actual `.tf` Terraform Resource code\n\nbalcony uses _read-only_ operations, it does not take any action on the used AWS account.\n\n\n### [Visit the Documentation Website](https://oguzhan-yilmaz.github.io/balcony/quickstart/)\n<!-- ### [**Go to QuickStart Page to get started using _balcony_**](quickstart.md) -->\n\n### Installation\n\n```bash\npip3 install balcony\n```\n\nVisit [**Installation & QuickStart Page**](https://oguzhan-yilmaz.github.io/balcony/quickstart/) to get started using _balcony_\n\n```bash  title="Basic usage"\n# see options\nbalcony\n\n# list available resources of ec2\nbalcony aws ec2 \n\n# read a resource\nbalcony aws s3 Buckets\n\n# show documentation\nbalcony aws iam Policy --list\n\n# generate terraform import blocks for a resource\nbalcony terraform-import s3 Buckets\n```\n\n\n## Features\n\n### Read any AWS Resource\n\n`balcony aws <service> <resource-name> --paginate` command reads all resources of a given type in your AWS account.\n\nRelated Docs: [QuickStart](https://oguzhan-yilmaz.github.io/balcony/quickstart/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/aws-read-resource.gif)\n\n\n---\n\n### Generate Terraform Import Blocks\n\nTerraform v1.5 introduced [import blocks](https://developer.hashicorp.com/terraform/language/import) that allows users to define their imports as code.\n\n`balcony terraform-import <service> <resource-name>` command generates these import blocks for you.\n\n`balcony terraform-import --list` to see the list of supported resources.\n\nRelated Docs: [Generate Terraform Import Blocks](https://oguzhan-yilmaz.github.io/balcony/terraform-import/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-import-blocks-example.gif)\n\n\n---\n\n### Generate actual Terraform Resource Code \n\nIf you have:\n\n- initialized terraform project\n- `import_blocks.tf` file that\'s generated with `balcony terraform-import` command\n\nyou can run `terraform plan -generate-config-out=generated.tf` to generate actual `.tf` resource code.\n\nThis feature is achieved with a Docker image.\n\nRelated Docs: [Generate Terraform Code with Docker Image](https://oguzhan-yilmaz.github.io/balcony/terraform-import-docker/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/docker-gen-tf-code-ec2-insances-example.gif)\n\n\n---\n\n### Interactive Wizard to create balcony import configurations \n\nBalcony doesn\'t know how to create terraform `import blocks` for all of the AWS resources.\n\nIt can be taught how to do it by creating `import-configurations` yaml files, but it\'s a manual process. This is where the interactive wizard comes in.\n\nInteractive Wizards asks you required questions to automatically create the `import-configurations` yaml files.\n\nRelated Docs: [Terraform Import Configuration Wizard](https://oguzhan-yilmaz.github.io/balcony/terraform-import-wizard/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-wizard-security-groups-example.gif)\n',
+    'long_description': '# balcony\n\n\n<div style="display: flex;">\n  <a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml/badge.svg" alt="Build and publish a Docker image to ghcr.io"></a>\n  <span style="width: 5px"></span>\n\n<a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment/badge.svg" alt="Build and Deploy Documentation website"></a>\n</div>\n\n\nbalcony is a modern CLI tool that with some killer features:\n\n- Auto-fill the required parameters for AWS API calls \n- Read the JSON data of any AWS resource in your account\n- Generate [Terraform Import Blocks](https://developer.hashicorp.com/terraform/language/import)\n- Generate actual `.tf` Terraform Resource code\n\nbalcony uses _read-only_ operations, it does not take any action on the used AWS account.\n\n\n### [Visit the Documentation Website](https://oguzhan-yilmaz.github.io/balcony/quickstart/)\n<!-- ### [**Go to QuickStart Page to get started using _balcony_**](quickstart.md) -->\n\n### Installation\n\n```bash\npip3 install balcony\n```\n\nVisit [**Installation & QuickStart Page**](https://oguzhan-yilmaz.github.io/balcony/quickstart/) to get started using _balcony_\n\n```bash  title="Basic usage"\n# see options\nbalcony\n\n# list available resources of ec2\nbalcony aws ec2 \n\n# read a resource\nbalcony aws s3 Buckets\n\n# show documentation\nbalcony aws iam Policy --list\n\n# generate terraform import blocks for a resource\nbalcony terraform-import s3 Buckets\n```\n\n\n## Features\n\n### Read any AWS Resource\n\n`balcony aws <service> <resource-name> --paginate` command reads all resources of a given type in your AWS account.\n\nRelated Docs: [QuickStart](https://oguzhan-yilmaz.github.io/balcony/quickstart/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/aws-read-resource.gif)\n\n\n---\n\n### Generate Terraform Import Blocks\n\nTerraform v1.5 introduced [import blocks](https://developer.hashicorp.com/terraform/language/import) that allows users to define their imports as code.\n\n`balcony terraform-import <service> <resource-name>` command generates these import blocks for you.\n\n`balcony terraform-import --list` to see the list of supported resources.\n\nRelated Docs: [Generate Terraform Import Blocks](https://oguzhan-yilmaz.github.io/balcony/terraform-import/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-import-blocks-example.gif)\n\n\n---\n\n### Generate actual Terraform Resource Code \n\n\nIf you have:\n\n- initialized terraform project\n- `import_blocks.tf` file that\'s generated with `balcony terraform-import` command\n\nyou can run `terraform plan -generate-config-out=generated.tf` to generate actual `.tf` resource code.\n\nThis feature is achieved with the [balcony-terraform-import Docker Image](https://github.com/oguzhan-yilmaz/balcony/pkgs/container/balcony-terraform-import).\n\n\nRelated Docs: [Generate Terraform Code with Docker Image](https://oguzhan-yilmaz.github.io/balcony/terraform-import-docker/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/docker-gen-tf-code-ec2-insances-example.gif)\n\n\n---\n\n### Interactive Wizard to create balcony import configurations \n\nBalcony doesn\'t know how to create terraform `import blocks` for all of the AWS resources.\n\nIt can be taught how to do it by creating `import-configurations` yaml files, but it\'s a manual process. This is where the interactive wizard comes in.\n\nInteractive Wizards asks you required questions to automatically create the `import-configurations` yaml files.\n\nRelated Docs: [Terraform Import Configuration Wizard](https://oguzhan-yilmaz.github.io/balcony/terraform-import-wizard/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-wizard-security-groups-example.gif)\n',
     'author': 'Oguzhan Yilmaz',
     'author_email': 'oguzhanylmz271@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 ['*'], 'balcony': ['custom_tf_import_configs/*', 'custom_yamls/*']}
 install_requires = \ ['Jinja2>=3.1.2,<4.0.0', 'PyYAML>=6.0,<7.0',
 'boto3>=1.24.80,<2.0.0', 'inflect>=6.0.0,<7.0.0', 'jmespath>=1.0.1,<2.0.0',
 'mkdocs-autorefs>=0.4.1,<0.5.0', 'mkdocs-material>=8.5.7,<10.0.0',
 'mkdocstrings[python]>=0.21.2,<0.22.0', 'pydantic>=1.10.7,<2.0.0',
 'rich>=13.3.4,<14.0.0', 'typer>=0.7.0,<0.8.0'] entry_points = \
 {'console_scripts': ['balcony = balcony.cli:run_app']} setup_kwargs = { 'name':
-'balcony', 'version': '0.1.8', 'description': 'Read any resource in your AWS
+'balcony', 'version': '0.1.9', 'description': 'Read any resource in your AWS
 Account. You can generate terraform code for them, too.', 'long_description':
 '# balcony\n\n\n
 \n [Build_and_publish_a_Docker_image_to_ghcr.io]\n \n\n[Build_and_Deploy
 Documentation_website]\n
 \n\n\nbalcony is a modern CLI tool that with some killer features:\n\n- Auto-
 fill the required parameters for AWS API calls \n- Read the JSON data of any
 AWS resource in your account\n- Generate [Terraform Import Blocks](https://
@@ -34,26 +34,28 @@
 (https://developer.hashicorp.com/terraform/language/import) that allows users
 to define their imports as code.\n\n`balcony terraform-import  ` command
 generates these import blocks for you.\n\n`balcony terraform-import --list` to
 see the list of supported resources.\n\nRelated Docs: [Generate Terraform
 Import Blocks](https://oguzhan-yilmaz.github.io/balcony/terraform-import/)\n\n!
 [](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/
 terraform-import-blocks-example.gif)\n\n\n---\n\n### Generate actual Terraform
-Resource Code \n\nIf you have:\n\n- initialized terraform project\n-
+Resource Code \n\n\nIf you have:\n\n- initialized terraform project\n-
 `import_blocks.tf` file that\'s generated with `balcony terraform-import`
 command\n\nyou can run `terraform plan -generate-config-out=generated.tf` to
-generate actual `.tf` resource code.\n\nThis feature is achieved with a Docker
-image.\n\nRelated Docs: [Generate Terraform Code with Docker Image](https://
-oguzhan-yilmaz.github.io/balcony/terraform-import-docker/)\n\n![](https://
-raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/docker-gen-
-tf-code-ec2-insances-example.gif)\n\n\n---\n\n### Interactive Wizard to create
-balcony import configurations \n\nBalcony doesn\'t know how to create terraform
-`import blocks` for all of the AWS resources.\n\nIt can be taught how to do it
-by creating `import-configurations` yaml files, but it\'s a manual process.
-This is where the interactive wizard comes in.\n\nInteractive Wizards asks you
+generate actual `.tf` resource code.\n\nThis feature is achieved with the
+[balcony-terraform-import Docker Image](https://github.com/oguzhan-yilmaz/
+balcony/pkgs/container/balcony-terraform-import).\n\n\nRelated Docs: [Generate
+Terraform Code with Docker Image](https://oguzhan-yilmaz.github.io/balcony/
+terraform-import-docker/)\n\n![](https://raw.githubusercontent.com/oguzhan-
+yilmaz/balcony-assets/main/gifs/docker-gen-tf-code-ec2-insances-
+example.gif)\n\n\n---\n\n### Interactive Wizard to create balcony import
+configurations \n\nBalcony doesn\'t know how to create terraform `import
+blocks` for all of the AWS resources.\n\nIt can be taught how to do it by
+creating `import-configurations` yaml files, but it\'s a manual process. This
+is where the interactive wizard comes in.\n\nInteractive Wizards asks you
 required questions to automatically create the `import-configurations` yaml
 files.\n\nRelated Docs: [Terraform Import Configuration Wizard](https://
 oguzhan-yilmaz.github.io/balcony/terraform-import-wizard/)\n\n![](https://
 raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-
 wizard-security-groups-example.gif)\n', 'author': 'Oguzhan Yilmaz',
 'author_email': 'oguzhanylmz271@gmail.com', 'maintainer': 'None',
 'maintainer_email': 'None', 'url': 'None', 'packages': packages,
```

### Comparing `balcony-0.1.8/PKG-INFO` & `balcony-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balcony
-Version: 0.1.8
+Version: 0.1.9
 Summary: Read any resource in your AWS Account. You can generate terraform code for them, too.
 License: GPL-3.0-or-later
 Author: Oguzhan Yilmaz
 Author-email: oguzhanylmz271@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -101,22 +101,24 @@
 ![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-import-blocks-example.gif)
 
 
 ---
 
 ### Generate actual Terraform Resource Code 
 
+
 If you have:
 
 - initialized terraform project
 - `import_blocks.tf` file that's generated with `balcony terraform-import` command
 
 you can run `terraform plan -generate-config-out=generated.tf` to generate actual `.tf` resource code.
 
-This feature is achieved with a Docker image.
+This feature is achieved with the [balcony-terraform-import Docker Image](https://github.com/oguzhan-yilmaz/balcony/pkgs/container/balcony-terraform-import).
+
 
 Related Docs: [Generate Terraform Code with Docker Image](https://oguzhan-yilmaz.github.io/balcony/terraform-import-docker/)
 
 ![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/docker-gen-tf-code-ec2-insances-example.gif)
 
 
 ---
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: balcony Version: 0.1.8 Summary: Read any resource
+Metadata-Version: 2.1 Name: balcony Version: 0.1.9 Summary: Read any resource
 in your AWS Account. You can generate terraform code for them, too. License:
 GPL-3.0-or-later Author: Oguzhan Yilmaz Author-email: oguzhanylmz271@gmail.com
 Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Requires-Dist: Jinja2
@@ -39,20 +39,22 @@
 supported resources. Related Docs: [Generate Terraform Import Blocks](https://
 oguzhan-yilmaz.github.io/balcony/terraform-import/) ![](https://
 raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-
 import-blocks-example.gif) --- ### Generate actual Terraform Resource Code If
 you have: - initialized terraform project - `import_blocks.tf` file that's
 generated with `balcony terraform-import` command you can run `terraform plan -
 generate-config-out=generated.tf` to generate actual `.tf` resource code. This
-feature is achieved with a Docker image. Related Docs: [Generate Terraform Code
-with Docker Image](https://oguzhan-yilmaz.github.io/balcony/terraform-import-
-docker/) ![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/
-main/gifs/docker-gen-tf-code-ec2-insances-example.gif) --- ### Interactive
-Wizard to create balcony import configurations Balcony doesn't know how to
-create terraform `import blocks` for all of the AWS resources. It can be taught
-how to do it by creating `import-configurations` yaml files, but it's a manual
-process. This is where the interactive wizard comes in. Interactive Wizards
-asks you required questions to automatically create the `import-configurations`
-yaml files. Related Docs: [Terraform Import Configuration Wizard](https://
-oguzhan-yilmaz.github.io/balcony/terraform-import-wizard/) ![](https://
+feature is achieved with the [balcony-terraform-import Docker Image](https://
+github.com/oguzhan-yilmaz/balcony/pkgs/container/balcony-terraform-import).
+Related Docs: [Generate Terraform Code with Docker Image](https://oguzhan-
+yilmaz.github.io/balcony/terraform-import-docker/) ![](https://
+raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/docker-gen-
+tf-code-ec2-insances-example.gif) --- ### Interactive Wizard to create balcony
+import configurations Balcony doesn't know how to create terraform `import
+blocks` for all of the AWS resources. It can be taught how to do it by creating
+`import-configurations` yaml files, but it's a manual process. This is where
+the interactive wizard comes in. Interactive Wizards asks you required
+questions to automatically create the `import-configurations` yaml files.
+Related Docs: [Terraform Import Configuration Wizard](https://oguzhan-
+yilmaz.github.io/balcony/terraform-import-wizard/) ![](https://
 raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-
 wizard-security-groups-example.gif)
```

