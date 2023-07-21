# Comparing `tmp/resoto-plugin-aws-3.6.1.tar.gz` & `tmp/resoto-plugin-aws-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-aws-3.6.1.tar", last modified: Fri Jul 14 17:00:21 2023, max compression
+gzip compressed data, was "resoto-plugin-aws-3.6.2.tar", last modified: Fri Jul 21 22:11:50 2023, max compression
```

## Comparing `resoto-plugin-aws-3.6.1.tar` & `resoto-plugin-aws-3.6.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:21.454192 resoto-plugin-aws-3.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-14 17:00:21.454192 resoto-plugin-aws-3.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:21.434192 resoto-plugin-aws-3.6.1/resoto_plugin_aws/
--rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/aws_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:21.438192 resoto-plugin-aws-3.6.1/resoto_plugin_aws/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11963 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:21.446192 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27876 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/athena.py
--rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/autoscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    25341 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    53735 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cloudfront.py
--rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cloudtrail.py
--rw-r--r--   0 runner    (1001) docker     (123)    18938 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cognito.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)   117358 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)    78300 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/efs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/eks.py
--rw-r--r--   0 runner    (1001) docker     (123)    26210 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/elasticache.py
--rw-r--r--   0 runner    (1001) docker     (123)    16406 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/elasticbeanstalk.py
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/elb.py
--rw-r--r--   0 runner    (1001) docker     (123)    22914 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/elbv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/glacier.py
--rw-r--r--   0 runner    (1001) docker     (123)    31557 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/kms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16952 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/lambda_.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/pricing.py
--rw-r--r--   0 runner    (1001) docker     (123)    39859 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/rds.py
--rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/route53.py
--rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)   234332 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/service_quotas.py
--rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:21.438192 resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-14 17:00:21.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-14 17:00:21.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:00:21.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 17:00:21.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:54:15.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 17:00:21.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 17:00:21.000000 resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-14 17:00:21.454192 resoto-plugin-aws-3.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:21.446192 resoto-plugin-aws-3.6.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/aws_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/collector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/configuration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/graphbuilder_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:21.454192 resoto-plugin-aws-3.6.1/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/apigateway_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/athena_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/autoscaling_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/cloudformation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/cloudfront_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/cloudtrail_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/cloudwatch_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/cognito_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/dynamodb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/ec2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/ecs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/efs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/eks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/elasticache_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/elasticbeanstalk_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/elb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/elbv2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/glacier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/iam_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/kinesis_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/kms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/lambda_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/pricing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/rds_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/redshift_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/route53_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/s3_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/sagemaker_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/service_quotas_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/sns_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/resources/sqs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-14 16:53:15.000000 resoto-plugin-aws-3.6.1/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:11:50.420334 resoto-plugin-aws-3.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-21 22:11:50.420334 resoto-plugin-aws-3.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:11:50.408333 resoto-plugin-aws-3.6.2/resoto_plugin_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16289 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/aws_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:11:50.408333 resoto-plugin-aws-3.6.2/resoto_plugin_aws/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:11:50.412334 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27876 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/autoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20641 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53735 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/cloudfront.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/cloudtrail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19802 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/cognito.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122318 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78300 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/efs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/eks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26210 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/elasticache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16406 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/elasticbeanstalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/elb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22914 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/elbv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/glacier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31557 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/kms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17029 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/lambda_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/pricing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39859 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/rds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/route53.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)   234332 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/service_quotas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:11:50.408333 resoto-plugin-aws-3.6.2/resoto_plugin_aws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-21 22:11:50.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-21 22:11:50.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:11:50.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 22:11:50.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:06:45.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-21 22:11:50.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 22:11:50.000000 resoto-plugin-aws-3.6.2/resoto_plugin_aws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-21 22:11:50.420334 resoto-plugin-aws-3.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:11:50.412334 resoto-plugin-aws-3.6.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/aws_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/collector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/configuration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/graphbuilder_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:11:50.420334 resoto-plugin-aws-3.6.2/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/apigateway_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/athena_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/autoscaling_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/cloudformation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/cloudfront_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/cloudtrail_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/cloudwatch_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/cognito_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/dynamodb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/ec2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/ecs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/efs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/eks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/elasticache_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/elasticbeanstalk_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/elb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/elbv2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/glacier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/iam_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/kinesis_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/kms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/lambda_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/pricing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/rds_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/redshift_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/route53_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/s3_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/sagemaker_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/service_quotas_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/sns_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/resources/sqs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-21 22:06:11.000000 resoto-plugin-aws-3.6.2/test/test_utils.py
```

### Comparing `resoto-plugin-aws-3.6.1/PKG-INFO` & `resoto-plugin-aws-3.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws
-Version: 3.6.1
+Version: 3.6.2
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-aws-3.6.1/README.md` & `resoto-plugin-aws-3.6.2/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/pyproject.toml` & `resoto-plugin-aws-3.6.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resoto-plugin-aws"
-version = "3.6.1"
+version = "3.6.2"
 authors = [{name="Some Engineering Inc."}]
 description = "Runs collector plugins and sends the result to resotocore."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -23,15 +23,16 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.6.1",
+    "resotolib==3.6.2",
+    "resotodata",
     "retrying",
     "boto3",
     "botocore",
 ]
 
 [project.entry-points."resoto.plugins"]
 aws = "resoto_plugin_aws:AWSCollectorPlugin"
@@ -39,9 +40,7 @@
 [project.urls]
 Documentation = "https://resoto.com"
 Source = "https://github.com/someengineering/resoto/tree/main/plugins/aws"
 
 [build-system]
 requires = ["setuptools>=67.8.0", "wheel>=0.40.0", "build>=0.10.0"]
 build-backend = "setuptools.build_meta"
-
-
```

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/__init__.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/aws_client.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/aws_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,15 +348,15 @@
         elif code in RetryableErrors:
             log.warning(f"Call to {aws_service} action {action} failed and will be retried eventually. Error: {e}")
             accumulate("FailedAndRetried", f"Retryable call has failed: {code}.")
             raise e  # already have been retried, give up here
         else:
             log.error(
                 f"An AWS API error {code} occurred during resource collection of {aws_service} action {action} in "  # noqa: E501
-                f"account {self.account_id} region {self.region} - skipping resources: {e}"
+                f"account {self.account_id} region {self.region} - skipping single resource: {e}"
             )
             accumulate(code, f"An AWS API error occurred during resource collection: {code}. Skipping resources.")
 
     def retry_for(self, aws_service: str, code: str) -> bool:
         """
         This method is called for retryable errors to determine whether we should retry the call or not, based on
         the partition, region, account and service name.
```

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/collector.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,29 +34,22 @@
     route53,
     s3,
     sagemaker,
     service_quotas,
     sns,
     sqs,
 )
-from resoto_plugin_aws.resource.base import (
-    AwsAccount,
-    AwsApiSpec,
-    AwsRegion,
-    AwsResource,
-    ExecutorQueue,
-    GatherFutures,
-    GraphBuilder,
-)
+from resoto_plugin_aws.resource.base import AwsAccount, AwsApiSpec, AwsRegion, AwsResource, GraphBuilder
 
 from resotolib.baseresources import Cloud, EdgeType
 from resotolib.core.actions import CoreFeedback
 from resotolib.core.progress import ProgressDone, ProgressTree
 from resotolib.graph import Graph
 from resotolib.proc import set_thread_name
+from resotolib.threading import ExecutorQueue, GatherFutures
 from resotolib.types import Json
 from resotolib.json import value_in_path
 
 from .utils import global_region_by_partition
 
 log = logging.getLogger("resoto.plugins.aws")
 
@@ -162,38 +155,37 @@
     def collect(self) -> None:
         with ThreadPoolExecutor(
             thread_name_prefix=f"aws_{self.account.id}", max_workers=self.config.resource_pool_size
         ) as executor:
             # The shared executor is used to spread work for the whole account.
             # Note: only tasks_per_key threads are running max for each region.
             tpk = self.config.shared_tasks_per_key([r.id for r in self.regions])
-            shared_queue = ExecutorQueue(executor, tasks_per_key=tpk, name=self.account.safe_name)
+            shared_queue = ExecutorQueue(executor, name=self.account.safe_name, tasks_per_key=tpk)
 
             def get_last_run() -> Optional[datetime]:
                 td = self.task_data
                 if not td:
                     return None
                 timestamp = value_in_path(td, ["timing", td.get("step", ""), "started_at"])
 
                 if timestamp is None:
                     return None
 
                 return datetime.fromtimestamp(timestamp, timezone.utc)
 
             last_run = get_last_run()
-
             global_builder = GraphBuilder(
                 self.graph,
                 self.cloud,
                 self.account,
                 self.global_region,
                 self.client,
                 shared_queue,
                 self.core_feedback,
-                last_run=last_run,
+                last_run_started_at=last_run,
             )
             global_builder.submit_work("iam", self.update_account)
 
             # mark open progress for all regions
             progress = ProgressTree(self.account.dname, path=[self.cloud.id])
             progress.add_progress(ProgressDone(self.global_region.safe_name, 0, 1))
             for region in self.regions:
```

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/configuration.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/configuration.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/apigateway.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/apigateway.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/athena.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/athena.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/autoscaling.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/autoscaling.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/base.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 from __future__ import annotations
 
-import concurrent
 import logging
 from abc import ABC
-from collections import defaultdict, deque
-from concurrent.futures import Executor, Future
+from concurrent.futures import Future
 from datetime import datetime, timezone, timedelta
-from functools import lru_cache, reduce
-from threading import Event, Lock
-from typing import Any, Callable, ClassVar, Deque, Dict, Iterator, List, Optional, Tuple, Type, TypeVar
+from functools import lru_cache
+from typing import Any, Callable, ClassVar, Dict, Iterator, List, Optional, Type, TypeVar
 from math import ceil
 
-from attr import evolve, field
+from attr import evolve
 from attrs import define
 from boto3.exceptions import Boto3Error
-from resotolib.utils import utc
 
 from resoto_plugin_aws.aws_client import AwsClient
 from resoto_plugin_aws.configuration import AwsConfig
 from resoto_plugin_aws.resource.pricing import AwsPricingPrice
 from resoto_plugin_aws.utils import arn_partition
+from resotolib.utils import utc
 from resotolib.baseresources import (
     BaseAccount,
     BaseRegion,
     BaseResource,
     BaseVolumeType,
     Cloud,
     EdgeType,
     ModelReference,
 )
 from resotolib.config import Config, current_config
 from resotolib.core.actions import CoreFeedback
 from resotolib.graph import ByNodeId, BySearchCriteria, EdgeKey, Graph, NodeSelector
-from resotolib.json import from_json
+from resotolib.json import from_json, value_in_path
 from resotolib.json_bender import Bender, bend
 from resotolib.lock import RWLock
 from resotolib.proc import set_thread_name
+from resotolib.threading import ExecutorQueue
 from resotolib.types import Json
+from resotodata.cloud import instances as cloud_instance_data
 
 log = logging.getLogger("resoto.plugins.aws")
 
 
 def get_client(config: Config, resource: BaseResource) -> AwsClient:
     account = resource.account()
     assert isinstance(account, AwsAccount)
@@ -316,195 +315,46 @@
 
 
 @define(eq=False, slots=False)
 class AwsEc2VolumeType(AwsResource, BaseVolumeType):
     kind: ClassVar[str] = "aws_ec2_volume_type"
 
 
-class CancelOnFirstError(Exception):
-    pass
-
-
-class GatherFutures:
-    def __init__(self, futures: List[Future[Any]]) -> None:
-        self._futures = futures
-        self._lock = Lock()
-        self._to_wait = len(futures)
-        self._when_done: Future[None] = Future()
-        for future in futures:
-            future.add_done_callback(self._on_future_done)
-
-    def _on_future_done(self, _: Future[Any]) -> None:
-        with self._lock:
-            self._to_wait -= 1
-            if self._to_wait == 0:
-                self._when_done.set_result(None)
-
-    @staticmethod
-    def all(futures: List[Future[Any]]) -> Future[None]:
-        return GatherFutures(futures)._when_done
-
-
-@define
-class ExecutorQueueTask:
-    key: Any
-    fn: Callable[..., T]
-    args: Tuple[Any, ...]
-    kwargs: Dict[str, Any]
-    future: Future[Any]
-
-    def __call__(self) -> T:  # type: ignore
-        try:
-            result: T = self.fn(*self.args, **self.kwargs)
-            self.future.set_result(result)
-            return result
-        except Exception as e:
-            self.future.set_exception(e)
-            raise
-
-
-@define
-class ExecutorQueue:
-    """
-    Use an underlying executor to perform work in parallel, but limit the number of tasks per key.
-    If fail_on_first_exception_in_group is True, then the first exception in a group
-    will not execute any more tasks in the same group.
-    """
-
-    executor: Executor
-    tasks_per_key: Callable[[str], int]
-    name: str
-    fail_on_first_exception_in_group: bool = False
-    _tasks_lock: Lock = Lock()
-    _tasks: Dict[str, Deque[ExecutorQueueTask]] = field(factory=lambda: defaultdict(deque))
-    _in_progress: Dict[str, int] = field(factory=lambda: defaultdict(int))
-    _futures: List[Future[Any]] = field(factory=list)
-    _exceptions: Dict[Any, Exception] = field(factory=dict)
-    _task_finished: Event = Event()
-
-    def submit_work(self, key: Any, fn: Callable[..., T], *args: Any, **kwargs: Any) -> Future[T]:
-        future = Future[T]()
-        task = ExecutorQueueTask(key=key, fn=fn, args=args, kwargs=kwargs, future=future)
-        self.__append_work(task)
-        return future
-
-    def __append_work(self, task: ExecutorQueueTask) -> None:
-        with self._tasks_lock:
-            self._tasks[task.key].appendleft(task)
-            self.__check_queue(task.key)
-
-    def __check_queue(self, key: Any) -> None:
-        # note: this method is not thread safe, it should only be called from within a lock
-        in_progress = self._in_progress[key]
-        tasks = self._tasks[key]
-
-        if self.fail_on_first_exception_in_group and self._exceptions.get(key) is not None:
-            # Fail all tasks in this group
-            ex = CancelOnFirstError("Exception happened in another thread. Do not start work.")
-            for task in tasks:
-                task.future.set_exception(ex)
-            # Clear the queue, so we don't execute them
-            # Clear the queue, so we don't execute them
-            tasks.clear()
-
-        if in_progress < self.tasks_per_key(key) and tasks:
-            task = tasks.pop()
-            self._in_progress[key] += 1
-            self.__perform_task(task)
-
-    def __perform_task(self, task: ExecutorQueueTask) -> Future[T]:
-        def only_start_when_no_error() -> T:
-            # in case of exception let's fail fast and do not execute the function
-            if self._exceptions.get(task.key) is None:
-                try:
-                    return task()
-                except Exception as e:
-                    # only store the first exception if we should fail on first future
-                    if self._exceptions.get(task.key) is None:
-                        self._exceptions[task.key] = e
-                    raise e
-            else:
-                raise CancelOnFirstError(
-                    "Exception happened in another thread. Do not start work."
-                ) from self._exceptions[task.key]
-
-        def execute() -> T:
-            try:
-                return only_start_when_no_error() if self.fail_on_first_exception_in_group else task()
-            finally:
-                with self._tasks_lock:
-                    self._in_progress[task.key] -= 1
-                    self._task_finished.set()
-                    self.__check_queue(task.key)
-
-        future = self.executor.submit(execute)
-
-        self._futures.append(future)
-        return future
-
-    def wait_for_submitted_work(self) -> None:
-        # wait until all futures are complete
-        to_wait = []
-
-        # step 1: wait until all tasks are committed to the executor
-        while True:
-            with self._tasks_lock:
-                ip = reduce(lambda x, y: x + y, self._in_progress.values(), 0)
-                if ip == 0:
-                    to_wait = self._futures
-                    self._futures = []
-                    break
-                else:
-                    # safe inside the lock. clear this event and check when next task is done
-                    self._task_finished.clear()
-            self._task_finished.wait()
-
-        # step 2: wait for all tasks to complete
-        for future in concurrent.futures.as_completed(to_wait):
-            try:
-                future.result()
-            except CancelOnFirstError:
-                pass
-            except Exception as ex:
-                log.exception(f"Unhandled exception in {self.name}: {ex}")
-                raise
-
-
 class GraphBuilder:
     def __init__(
         self,
         graph: Graph,
         cloud: Cloud,
         account: AwsAccount,
         region: AwsRegion,
         client: AwsClient,
         executor: ExecutorQueue,
         core_feedback: CoreFeedback,
         global_instance_types: Optional[Dict[str, Any]] = None,
         graph_nodes_access: Optional[RWLock] = None,
         graph_edges_access: Optional[RWLock] = None,
-        last_run: Optional[datetime] = None,
+        last_run_started_at: Optional[datetime] = None,
     ) -> None:
         self.graph = graph
         self.cloud = cloud
         self.account = account
         self.region = region
         self.client = client
         self.executor = executor
         self.name = f"AWS:{account.name}:{region.name}"
         self.global_instance_types: Dict[str, Any] = global_instance_types if global_instance_types is not None else {}
         self.core_feedback = core_feedback
         self.graph_nodes_access = graph_nodes_access or RWLock()
         self.graph_edges_access = graph_edges_access or RWLock()
-        self.last_run_started_at = last_run
+        self.last_run_started_at = last_run_started_at
         self.created_at = utc()
 
-        if self.last_run_started_at:
+        if last_run_started_at:
             now = utc()
-            start = self.last_run_started_at
+            start = last_run_started_at
             delta = now - start
             # AWS requires period to be a muliple of 60, ceil because we want to overlap when in doubt
             delta = timedelta(seconds=ceil(delta.seconds / 60) * 60)
             min_delta = max(delta, timedelta(seconds=600))
             # in case the last collection happened too quickly, raise the metrics timedelta to 600s,
             # otherwise we get no results from AWS
             if min_delta != delta:
@@ -616,29 +466,38 @@
             ]
 
     @lru_cache(maxsize=None)
     def instance_type(self, region: AwsRegion, instance_type: str) -> Optional[Any]:
         if (it := self.global_instance_types.get(instance_type)) is None:
             return None  # instance type not found
 
-        price = AwsPricingPrice.instance_type_price(self.client.for_region(region.id), instance_type, region.safe_name)
-        result = evolve(it, region=region, ondemand_cost=price.on_demand_price_usd if price else None)
+        price = value_in_path(cloud_instance_data, ["aws", instance_type, "pricing", region.id, "linux", "ondemand"])
+        physical_processor = value_in_path(cloud_instance_data, ["aws", instance_type, "physical_processor"])
+        gpu_model = value_in_path(cloud_instance_data, ["aws", instance_type, "GPU_model"])
+        pretty_name = value_in_path(cloud_instance_data, ["aws", instance_type, "pretty_name"])
+        ecu = value_in_path(cloud_instance_data, ["aws", instance_type, "ECU"])
+        ecu = float(ecu) if isinstance(ecu, (int, float)) else None
+        result = evolve(it, region=region, ondemand_cost=price, pretty_name=pretty_name, ecu=ecu)
+        if getattr(result, "instance_type_processor_info", None):
+            result.instance_type_processor_info.physical_processor = physical_processor
+        if getattr(result, "instance_type_gpu_info", None):
+            result.instance_type_gpu_info.gpu_model = gpu_model
         # add this instance type to the graph
         self.add_node(result, region=region)
         self.add_edge(region, node=result)
         return result
 
     @lru_cache(maxsize=None)
     def volume_type(self, volume_type: str) -> Optional[Any]:
         price = AwsPricingPrice.volume_type_price(self.client, volume_type, self.region.safe_name)
         vt = AwsEc2VolumeType(
             id=volume_type,
             name=volume_type,
             volume_type=volume_type,
-            ondemand_cost=price.on_demand_price_usd if price else 0,
+            ondemand_cost=price.on_demand_price_usd if price else None,
             region=self.region,
         )
         self.add_node(vt, {})
         return vt
 
     def for_region(self, region: AwsRegion) -> GraphBuilder:
         return GraphBuilder(
```

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cloudformation.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/cloudformation.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cloudfront.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/cloudfront.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cloudtrail.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/cloudtrail.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cloudwatch.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/cloudwatch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import re
 from datetime import datetime, timedelta
-from typing import ClassVar, Dict, List, Optional, Type, Tuple
+from typing import ClassVar, Dict, List, Optional, Type, Tuple, TypeVar
 
 from attr import define, field
 
 from resoto_plugin_aws.aws_client import AwsClient
 from resoto_plugin_aws.resource.base import AwsApiSpec, AwsResource, GraphBuilder
 from resoto_plugin_aws.resource.kms import AwsKmsKey
-from resoto_plugin_aws.utils import ToDict
-from resotolib.baseresources import ModelReference
+from resoto_plugin_aws.utils import ToDict, MetricNormalization
+from resotolib.baseresources import ModelReference, BaseResource
 from resotolib.graph import Graph
 from resotolib.json import from_json
 from resotolib.json_bender import S, Bend, Bender, ForallBend, bend, F, SecondsFromEpochToDatetime
 from resotolib.types import Json
 from resotolib.utils import chunks
 
 service_name = "cloudwatch"
@@ -446,7 +446,31 @@
                 if metric.id:
                     result[lookup[metric.id]] = metric
 
         return result
 
 
 resources: List[Type[AwsResource]] = [AwsCloudwatchAlarm, AwsCloudwatchLogGroup, AwsCloudwatchMetricFilter]
+
+V = TypeVar("V", bound=BaseResource)
+
+
+def update_resource_metrics(
+    resources_map: Dict[str, V],
+    cloudwatch_result: Dict[AwsCloudwatchQuery, AwsCloudwatchMetricData],
+    metric_normalizers: Dict[str, MetricNormalization],
+) -> None:
+    for query, metric in cloudwatch_result.items():
+        resource = resources_map.get(query.ref_id)
+        if resource is None:
+            continue
+        metric_value = next(iter(metric.metric_values), None)
+        if metric_value is None:
+            continue
+        normalizer = metric_normalizers.get(query.metric_name)
+        if not normalizer:
+            continue
+
+        name = normalizer.name
+        value = metric_normalizers[query.metric_name].normalize_value(metric_value)
+
+        resource._resource_usage[name][normalizer.stat_map[query.stat]] = value
```

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/cognito.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/cognito.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/config.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/dynamodb.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/dynamodb.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/ec2.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/ec2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 from datetime import datetime
-from typing import ClassVar, Dict, Optional, List, Type, Any, Callable, NamedTuple
+from typing import ClassVar, Dict, Optional, List, Type, Any
 import copy
 
 from attrs import define, field
 from resoto_plugin_aws.aws_client import AwsClient
 
 from resoto_plugin_aws.resource.base import AwsResource, GraphBuilder, AwsApiSpec, get_client
-from resoto_plugin_aws.resource.cloudwatch import AwsCloudwatchQuery, AwsCloudwatchMetricData
+from resoto_plugin_aws.resource.cloudwatch import AwsCloudwatchQuery, AwsCloudwatchMetricData, update_resource_metrics
 from resoto_plugin_aws.resource.kms import AwsKmsKey
 from resoto_plugin_aws.resource.s3 import AwsS3Bucket
-from resoto_plugin_aws.utils import ToDict, TagsValue, identity
+from resoto_plugin_aws.utils import ToDict, TagsValue, MetricNormalization
 from resotolib.baseresources import (
     BaseInstance,
     EdgeType,
     BaseVolume,
     BaseInstanceType,
     VolumeStatus,
     InstanceStatus,
@@ -83,14 +83,15 @@
     kind: ClassVar[str] = "aws_ec2_processor_info"
     mapping: ClassVar[Dict[str, Bender]] = {
         "supported_architectures": S("SupportedArchitectures", default=[]),
         "sustained_clock_speed_in_ghz": S("SustainedClockSpeedInGhz"),
     }
     supported_architectures: List[str] = field(factory=list)
     sustained_clock_speed_in_ghz: Optional[float] = field(default=None)
+    physical_processor: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class AwsEc2VCpuInfo:
     kind: ClassVar[str] = "aws_ec2_v_cpu_info"
     mapping: ClassVar[Dict[str, Bender]] = {
         "default_v_cpus": S("DefaultVCpus"),
@@ -228,14 +229,15 @@
     kind: ClassVar[str] = "aws_ec2_gpu_info"
     mapping: ClassVar[Dict[str, Bender]] = {
         "gpus": S("Gpus", default=[]) >> ForallBend(AwsEc2GpuDeviceInfo.mapping),
         "total_gpu_memory_in_mi_b": S("TotalGpuMemoryInMiB"),
     }
     gpus: List[AwsEc2GpuDeviceInfo] = field(factory=list)
     total_gpu_memory_in_mi_b: Optional[int] = field(default=None)
+    gpu_model: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class AwsEc2FpgaDeviceInfo:
     kind: ClassVar[str] = "aws_ec2_fpga_device_info"
     mapping: ClassVar[Dict[str, Bender]] = {
         "name": S("Name"),
@@ -323,14 +325,16 @@
         >> Bend(AwsEc2InferenceAcceleratorInfo.mapping),
         "hibernation_supported": S("HibernationSupported"),
         "burstable_performance_supported": S("BurstablePerformanceSupported"),
         "dedicated_hosts_supported": S("DedicatedHostsSupported"),
         "auto_recovery_supported": S("AutoRecoverySupported"),
         "supported_boot_modes": S("SupportedBootModes", default=[]),
     }
+    pretty_name: Optional[str] = field(default=None)
+    ecu: Optional[float] = field(default=None)
     current_generation: Optional[bool] = field(default=None)
     free_tier_eligible: Optional[bool] = field(default=None)
     supported_usage_classes: List[str] = field(factory=list)
     supported_root_device_types: List[str] = field(factory=list)
     supported_virtualization_types: List[str] = field(factory=list)
     bare_metal: Optional[bool] = field(default=None)
     hypervisor: Optional[str] = field(default=None)
@@ -476,14 +480,99 @@
             if volume := AwsEc2Volume.from_api(js, builder):
                 instance = builder.add_node(volume, js)
                 volumes.append(instance)
                 if vt := builder.volume_type(instance.volume_type):
                     builder.add_edge(vt, EdgeType.default, node=instance)
         update_atime_mtime()
 
+    @classmethod
+    def collect_usage_metrics(cls: Type[AwsResource], builder: GraphBuilder) -> None:
+        volumes = {
+            volume.id: volume
+            for volume in builder.nodes(clazz=AwsEc2Volume)
+            if volume.region().id == builder.region.id and volume
+        }
+        queries = []
+        delta = builder.metrics_delta
+        start = builder.metrics_start
+        now = builder.created_at
+        for volume_id in volumes:
+            queries.extend(
+                [
+                    AwsCloudwatchQuery.create(
+                        metric_name=metric_name,
+                        namespace="AWS/EBS",
+                        period=delta,
+                        ref_id=volume_id,
+                        stat="Sum",
+                        unit="Bytes",
+                        VolumeId=volume_id,
+                    )
+                    for metric_name in ["VolumeWriteBytes", "VolumeReadBytes"]
+                ]
+            )
+            queries.extend(
+                [
+                    AwsCloudwatchQuery.create(
+                        metric_name=metric_name,
+                        namespace="AWS/EBS",
+                        period=delta,
+                        ref_id=volume_id,
+                        stat="Sum",
+                        unit="Count",
+                        VolumeId=volume_id,
+                    )
+                    for metric_name in ["VolumeWriteOps", "VolumeReadOps"]
+                ]
+            )
+            queries.extend(
+                [
+                    AwsCloudwatchQuery.create(
+                        metric_name=metric_name,
+                        namespace="AWS/EBS",
+                        period=delta,
+                        ref_id=volume_id,
+                        stat="Sum",
+                        unit="Seconds",
+                        VolumeId=volume_id,
+                    )
+                    for metric_name in ["VolumeTotalWriteTime", "VolumeIdleTime"]
+                ]
+            )
+            queries.extend(
+                [
+                    AwsCloudwatchQuery.create(
+                        metric_name="VolumeQueueLength",
+                        namespace="AWS/EBS",
+                        period=delta,
+                        ref_id=volume_id,
+                        stat=stat,
+                        unit="Count",
+                        VolumeId=volume_id,
+                    )
+                    for stat in ["Minimum", "Average", "Maximum"]
+                ]
+            )
+
+        metric_normalizers = {
+            "VolumeWriteBytes": MetricNormalization(name="volume_write_bytes"),
+            "VolumeReadBytes": MetricNormalization(name="volume_read_bytes"),
+            "VolumeWriteOps": MetricNormalization(name="volume_write_ops"),
+            "VolumeReadOps": MetricNormalization(name="volume_read_ops"),
+            "VolumeTotalWriteTime": MetricNormalization(name="volume_total_write_time"),
+            "VolumeIdleTime": MetricNormalization(name="volume_idle_time"),
+            "VolumeQueueLength": MetricNormalization(
+                name="volume_queue_length", normalize_value=lambda x: round(x, ndigits=3)
+            ),
+        }
+
+        cloudwatch_result = AwsCloudwatchMetricData.query_for(builder.client, queries, start, now)
+
+        update_resource_metrics(volumes, cloudwatch_result, metric_normalizers)
+
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         super().connect_in_graph(builder, source)
         for attachment in self.volume_attachments:
             builder.dependant_node(self, reverse=True, clazz=AwsEc2Instance, id=attachment.instance_id)
         if self.volume_kms_key_id:
             builder.dependant_node(
                 self,
@@ -898,19 +987,14 @@
     "shutting-down": InstanceStatus.STOPPED,
     "terminated": InstanceStatus.TERMINATED,
     "stopping": InstanceStatus.STOPPED,
     "stopped": InstanceStatus.STOPPED,
 }
 
 
-class MetricNormalization(NamedTuple):
-    name: str
-    normalize_value: Callable[[float], float] = identity
-
-
 @define(eq=False, slots=False)
 class AwsEc2Instance(EC2Taggable, AwsResource, BaseInstance):
     kind: ClassVar[str] = "aws_ec2_instance"
     api_spec: ClassVar[AwsApiSpec] = AwsApiSpec(service_name, "describe-instances", "Reservations")
     reference_kinds: ClassVar[ModelReference] = {
         "predecessors": {"default": ["aws_vpc"], "delete": ["aws_ec2_keypair", "aws_vpc"]},
         "successors": {"default": ["aws_ec2_keypair"]},
@@ -1052,19 +1136,17 @@
     def collect_usage_metrics(cls: Type[AwsResource], builder: GraphBuilder) -> None:
         instances = {
             instance.id: instance
             for instance in builder.nodes(clazz=AwsEc2Instance)
             if instance.region().id == builder.region.id and instance.instance_status == InstanceStatus.RUNNING
         }
         queries = []
-
         delta = builder.metrics_delta
         start = builder.metrics_start
         now = builder.created_at
-
         for instance_id in instances:
             queries.extend(
                 [
                     AwsCloudwatchQuery.create(
                         metric_name="CPUUtilization",
                         namespace="AWS/EC2",
                         period=delta,
@@ -1072,37 +1154,73 @@
                         stat=stat,
                         unit="Percent",
                         InstanceId=instance_id,
                     )
                     for stat in ["Minimum", "Average", "Maximum"]
                 ]
             )
+            queries.extend(
+                [
+                    AwsCloudwatchQuery.create(
+                        metric_name=name,
+                        namespace="AWS/EC2",
+                        period=delta,
+                        ref_id=instance_id,
+                        stat="Sum",
+                        unit="Bytes",
+                        InstanceId=instance_id,
+                    )
+                    for name in ["NetworkIn", "NetworkOut"]
+                ]
+            )
+            queries.extend(
+                [
+                    AwsCloudwatchQuery.create(
+                        metric_name=name,
+                        namespace="AWS/EC2",
+                        period=delta,
+                        ref_id=instance_id,
+                        stat="Sum",
+                        unit="Count",
+                        InstanceId=instance_id,
+                    )
+                    for name in ["DiskReadOps", "DiskWriteOps"]
+                ]
+            )
+            queries.extend(
+                [
+                    AwsCloudwatchQuery.create(
+                        metric_name=name,
+                        namespace="AWS/EC2",
+                        period=delta,
+                        ref_id=instance_id,
+                        stat="Sum",
+                        unit="Bytes",
+                        InstanceId=instance_id,
+                    )
+                    for name in ["DiskReadBytes", "DiskWriteBytes"]
+                ]
+            )
 
-        metric_normalizers = {"CPUUtilization": MetricNormalization("cpu", lambda x: round(x, ndigits=3))}
-
-        stat_name = {
-            "Minimum": "min",
-            "Average": "avg",
-            "Maximum": "max",
+        metric_normalizers = {
+            "CPUUtilization": MetricNormalization(
+                name="cpu_utilization",
+                normalize_value=lambda x: round(x, ndigits=3),
+            ),
+            "NetworkIn": MetricNormalization(name="network_in"),
+            "NetworkOut": MetricNormalization(name="network_out"),
+            "DiskReadOps": MetricNormalization(name="disk_read_ops"),
+            "DiskWriteOps": MetricNormalization(name="disk_write_ops"),
+            "DiskReadBytes": MetricNormalization(name="disk_read_bytes"),
+            "DiskWriteBytes": MetricNormalization(name="disk_write_bytes"),
         }
 
         cloudwatch_result = AwsCloudwatchMetricData.query_for(builder.client, queries, start, now)
 
-        for query, metric in cloudwatch_result.items():
-            instance = instances.get(query.ref_id)
-            if instance is None:
-                continue
-            metric_value = next(iter(metric.metric_values), None)
-            if metric_value is None:
-                continue
-
-            name = metric_normalizers[query.metric_name].name
-            value = metric_normalizers[query.metric_name].normalize_value(metric_value)
-
-            instance._resource_usage[name][stat_name[query.stat]] = value
+        update_resource_metrics(instances, cloudwatch_result, metric_normalizers)
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         super().connect_in_graph(builder, source)
         # connect instance type and copy values
         # noinspection PyTypeChecker
         if instance_type := builder.instance_type(self.region(), self.instance_type):
             self.instance_cores = instance_type.instance_cores
```

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/ecs.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/ecs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/efs.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/efs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/eks.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/eks.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/elasticache.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/elasticache.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/elasticbeanstalk.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/elasticbeanstalk.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/elb.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/elb.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/elbv2.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/elbv2.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/glacier.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/glacier.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/iam.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/iam.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/kinesis.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/kinesis.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/kms.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/kms.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/lambda_.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/lambda_.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,17 @@
             AwsApiSpec(service_name, "get-policy"),
             AwsApiSpec(service_name, "list-tags"),
         ]
 
     @classmethod
     def collect(cls: Type[AwsResource], json: List[Json], builder: GraphBuilder) -> None:
         def add_tags(function: AwsLambdaFunction) -> None:
-            tags = builder.client.get(service_name, "list-tags", "Tags", Resource=function.arn)
+            tags = builder.client.get(
+                service_name, "list-tags", "Tags", Resource=function.arn, expected_errors=["ResourceNotFoundException"]
+            )
             if tags:
                 function.tags = tags
 
         def get_policy(function: AwsLambdaFunction) -> None:
             if policy := builder.client.get(
                 service_name,
                 "get-policy",
```

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/pricing.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/pricing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/rds.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/rds.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/redshift.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/redshift.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/route53.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/route53.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/s3.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/s3.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/sagemaker.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/sagemaker.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/service_quotas.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/service_quotas.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/sns.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/sns.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
     def collect(cls: Type[AwsResource], json: List[Json], builder: GraphBuilder) -> None:
         for entry in json:
             subscription = builder.client.get(
                 service_name,
                 "get-subscription-attributes",
                 SubscriptionArn=entry["SubscriptionArn"],
                 result_name="Attributes",
-                expected_errors=["InvalidParameter"],
+                expected_errors=["InvalidParameter", "NotFound"],
             )
             if subscription:
                 if subscription_instance := cls.from_api(subscription, builder):
                     builder.add_node(subscription_instance, subscription)
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         if self.subscription_topic_arn:
```

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/resource/sqs.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/resource/sqs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws/utils.py` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import uuid
 from configparser import ConfigParser
 from pathlib import Path
 from typing import Any, Callable, Dict, Iterable, List, Optional, TypeVar
+from attrs import frozen
 
 from boto3.session import Session as BotoSession
 from botocore.exceptions import ConnectionClosedError, CredentialRetrievalError
 from prometheus_client import Counter
 from retrying import retry
 
 from resotolib.baseresources import BaseRegion, BaseResource
@@ -187,7 +188,19 @@
 
 
 T = TypeVar("T")
 
 
 def identity(x: T) -> T:
     return x
+
+
+@frozen(kw_only=True)
+class MetricNormalization:
+    name: str
+    stat_map: Dict[str, str] = {
+        "Minimum": "min",
+        "Average": "avg",
+        "Maximum": "max",
+        "Sum": "sum",
+    }
+    normalize_value: Callable[[float], float] = identity
```

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/PKG-INFO` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws
-Version: 3.6.1
+Version: 3.6.2
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-aws-3.6.1/resoto_plugin_aws.egg-info/SOURCES.txt` & `resoto-plugin-aws-3.6.2/resoto_plugin_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/__init__.py` & `resoto-plugin-aws-3.6.2/test/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 from typing import Iterator
 
 from pytest import fixture
 
 from resoto_plugin_aws.collector import AwsAccountCollector
 from resoto_plugin_aws.configuration import AwsConfig
 from resoto_plugin_aws.aws_client import AwsClient
-from resoto_plugin_aws.resource.base import AwsAccount, AwsRegion, GraphBuilder, ExecutorQueue
+from resoto_plugin_aws.resource.base import AwsAccount, AwsRegion, GraphBuilder
 from resotolib.baseresources import Cloud
 from resotolib.core.actions import CoreFeedback
 from resotolib.graph import Graph
+from resotolib.threading import ExecutorQueue
 from test.resources import BotoFileBasedSession
 
 
 @fixture
 def aws_config() -> AwsConfig:
     config = AwsConfig(discard_account_on_resource_error=True)
     config.sessions().session_class_factory = BotoFileBasedSession
@@ -25,15 +26,15 @@
 def aws_client(aws_config: AwsConfig) -> AwsClient:
     return AwsClient(aws_config, "test", region="us-east-1")
 
 
 @fixture
 def builder(aws_client: AwsClient, no_feedback: CoreFeedback) -> Iterator[GraphBuilder]:
     with ThreadPoolExecutor(1) as executor:
-        queue = ExecutorQueue(executor, lambda _: 1, "dummy")
+        queue = ExecutorQueue(executor, "dummy", lambda _: 1)
         yield GraphBuilder(
             Graph(), Cloud(id="aws"), AwsAccount(id="test"), AwsRegion(id="us-east-1"), aws_client, queue, no_feedback
         )
 
 
 @fixture
 def no_feedback() -> CoreFeedback:
```

### Comparing `resoto-plugin-aws-3.6.1/test/aws_client_test.py` & `resoto-plugin-aws-3.6.2/test/aws_client_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/collector_test.py` & `resoto-plugin-aws-3.6.2/test/collector_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/configuration_test.py` & `resoto-plugin-aws-3.6.2/test/configuration_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/graphbuilder_test.py` & `resoto-plugin-aws-3.6.2/test/graphbuilder_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 from typing import List
 
+from resotolib.json import value_in_path
 from resoto_plugin_aws.resource.base import GraphBuilder, AwsRegion
 from resoto_plugin_aws.resource.ec2 import AwsEc2InstanceType
+from resotodata.cloud import instances as cloud_instance_data
 
 from test import builder, aws_client, aws_config, no_feedback  # noqa: F401
 
 
 def test_instance_type(builder: GraphBuilder) -> None:
-    builder.global_instance_types["m4.large"] = AwsEc2InstanceType(id="m4.large")
-    m4l: AwsEc2InstanceType = builder.instance_type(builder.region, "m4.large")  # type: ignore
-    assert m4l == builder.instance_type(builder.region, "m4.large")
-    assert m4l.ondemand_cost == 0.051
+    instance_type = "m4.large"
+    builder.global_instance_types[instance_type] = AwsEc2InstanceType(id=instance_type)
+    m4l: AwsEc2InstanceType = builder.instance_type(builder.region, instance_type)  # type: ignore
+    assert m4l == builder.instance_type(builder.region, instance_type)
+    assert m4l.ondemand_cost == value_in_path(
+        cloud_instance_data, ["aws", instance_type, "pricing", builder.region.id, "linux", "ondemand"]
+    )
     eu_builder = builder.for_region(AwsRegion(id="eu-central-1"))
-    m4l_eu: AwsEc2InstanceType = eu_builder.instance_type(eu_builder.region, "m4.large")  # type: ignore
+    m4l_eu: AwsEc2InstanceType = eu_builder.instance_type(eu_builder.region, instance_type)  # type: ignore
     assert m4l != m4l_eu
-    assert m4l_eu == eu_builder.instance_type(eu_builder.region, "m4.large")
-    assert m4l_eu.ondemand_cost == 0.12
+    assert m4l_eu == eu_builder.instance_type(eu_builder.region, instance_type)
+    assert m4l_eu.ondemand_cost == value_in_path(
+        cloud_instance_data, ["aws", instance_type, "pricing", eu_builder.region.id, "linux", "ondemand"]
+    )
 
 
 def test_executor(builder: GraphBuilder) -> None:
     result: List[int] = []
 
     def do_something(key: int) -> None:
         result.append(key)
```

### Comparing `resoto-plugin-aws-3.6.1/test/resources/__init__.py` & `resoto-plugin-aws-3.6.2/test/resources/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from resoto_plugin_aws.resource.base import (
     GraphBuilder,
     AwsResourceType,
     AwsAccount,
     AwsRegion,
     AwsResource,
     AwsApiSpec,
-    ExecutorQueue,
 )
 from resotolib.baseresources import Cloud
 from resotolib.core.actions import CoreFeedback
 from resotolib.graph import Graph
+from resotolib.threading import ExecutorQueue
 
 
 class BotoDummyStsClient:
     def __getattr__(self, action_name: str) -> Callable[[], Any]:
         def call(*args: Any, **kwargs: Any) -> Any:
             return {"Credentials": {"AccessKeyId": "xxx", "SecretAccessKey": "xxx", "SessionToken": "xxx"}}
```

### Comparing `resoto-plugin-aws-3.6.1/test/resources/apigateway_test.py` & `resoto-plugin-aws-3.6.2/test/resources/apigateway_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/athena_test.py` & `resoto-plugin-aws-3.6.2/test/resources/athena_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/autoscaling_test.py` & `resoto-plugin-aws-3.6.2/test/resources/autoscaling_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/base_test.py` & `resoto-plugin-aws-3.6.2/test/resources/base_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from collections import defaultdict
 from concurrent.futures import ThreadPoolExecutor, Future
 from typing import Sequence, Tuple, List, Optional, Callable, Any
 
 from more_itertools import flatten
 
-from resoto_plugin_aws.resource.base import ExecutorQueue, AwsRegion, GraphBuilder, GatherFutures
+from resoto_plugin_aws.resource.base import AwsRegion, GraphBuilder
 from resoto_plugin_aws.resource.ec2 import AwsEc2InstanceType
+from resotolib.threading import ExecutorQueue, GatherFutures
 from test import account_collector, builder, aws_client, aws_config, no_feedback  # noqa: F401
 
 
 def check_executor_work(
     work: List[Tuple[str, int]],
     workers: int,
     tasks_per_key: int,
@@ -26,15 +27,15 @@
         in_progress.remove(num)
         if num % 100 == 5:
             raise Exception(f"Abort {num}")
         work_done.append(num)
 
     with ThreadPoolExecutor(max_workers=workers) as executor:
         queue = ExecutorQueue(
-            executor, lambda _: tasks_per_key, "test", fail_on_first_exception_in_group=fail_on_first_exception
+            executor, "test", lambda _: tasks_per_key, fail_on_first_exception_in_group=fail_on_first_exception
         )
         for key, idx in work:
             queue.submit_work(key, do_work, idx)
 
         try:
             queue.wait_for_submitted_work()
             return work_done, None
```

### Comparing `resoto-plugin-aws-3.6.1/test/resources/cloudformation_test.py` & `resoto-plugin-aws-3.6.2/test/resources/cloudformation_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/cloudfront_test.py` & `resoto-plugin-aws-3.6.2/test/resources/cloudfront_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/cloudtrail_test.py` & `resoto-plugin-aws-3.6.2/test/resources/cloudtrail_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from concurrent.futures import ThreadPoolExecutor
 
-from resoto_plugin_aws.resource.base import ExecutorQueue
 from resoto_plugin_aws.resource.cloudtrail import AwsCloudTrail
 from resoto_plugin_aws.resource.kms import AwsKmsKey
 from resoto_plugin_aws.resource.s3 import AwsS3Bucket
 from resoto_plugin_aws.resource.sns import AwsSnsTopic
+from resotolib.threading import ExecutorQueue
 from test.resources import round_trip_for
 
 
 def test_trails() -> None:
     first, builder = round_trip_for(AwsCloudTrail, region_name="us-east-1")
     with ThreadPoolExecutor(1) as executor:
-        builder.executor = ExecutorQueue(executor, lambda _: 1, "dummy")
+        builder.executor = ExecutorQueue(executor, "dummy")
         AwsS3Bucket.collect_resources(builder)
         AwsKmsKey.collect_resources(builder)
         AwsSnsTopic.collect_resources(builder)
         data = builder.graph.nodes(data=True)[first]
         first.connect_in_graph(builder, data["source"])
         assert len(builder.edges_of(AwsCloudTrail, AwsS3Bucket)) == 1
         assert len(builder.edges_of(AwsCloudTrail, AwsKmsKey)) == 1
```

### Comparing `resoto-plugin-aws-3.6.1/test/resources/cloudwatch_test.py` & `resoto-plugin-aws-3.6.2/test/resources/cloudwatch_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/cognito_test.py` & `resoto-plugin-aws-3.6.2/test/resources/cognito_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/dynamodb_test.py` & `resoto-plugin-aws-3.6.2/test/resources/dynamodb_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/ec2_test.py` & `resoto-plugin-aws-3.6.2/test/resources/ec2_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/ecs_test.py` & `resoto-plugin-aws-3.6.2/test/resources/ecs_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/eks_test.py` & `resoto-plugin-aws-3.6.2/test/resources/eks_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/elasticache_test.py` & `resoto-plugin-aws-3.6.2/test/resources/elasticache_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/elasticbeanstalk_test.py` & `resoto-plugin-aws-3.6.2/test/resources/elasticbeanstalk_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/elb_test.py` & `resoto-plugin-aws-3.6.2/test/resources/elb_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/elbv2_test.py` & `resoto-plugin-aws-3.6.2/test/resources/elbv2_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/glacier_test.py` & `resoto-plugin-aws-3.6.2/test/resources/glacier_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/iam_test.py` & `resoto-plugin-aws-3.6.2/test/resources/iam_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/kinesis_test.py` & `resoto-plugin-aws-3.6.2/test/resources/kinesis_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/kms_test.py` & `resoto-plugin-aws-3.6.2/test/resources/kms_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/lambda_test.py` & `resoto-plugin-aws-3.6.2/test/resources/lambda_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/pricing_test.py` & `resoto-plugin-aws-3.6.2/test/resources/pricing_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/rds_test.py` & `resoto-plugin-aws-3.6.2/test/resources/rds_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/redshift_test.py` & `resoto-plugin-aws-3.6.2/test/resources/redshift_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/route53_test.py` & `resoto-plugin-aws-3.6.2/test/resources/route53_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/s3_test.py` & `resoto-plugin-aws-3.6.2/test/resources/s3_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/sagemaker_test.py` & `resoto-plugin-aws-3.6.2/test/resources/sagemaker_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/service_quotas_test.py` & `resoto-plugin-aws-3.6.2/test/resources/service_quotas_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/sns_test.py` & `resoto-plugin-aws-3.6.2/test/resources/sns_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/resources/sqs_test.py` & `resoto-plugin-aws-3.6.2/test/resources/sqs_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.1/test/test_utils.py` & `resoto-plugin-aws-3.6.2/test/test_utils.py`

 * *Files identical despite different names*

