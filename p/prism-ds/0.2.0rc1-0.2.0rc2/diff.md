# Comparing `tmp/prism-ds-0.2.0rc1.tar.gz` & `tmp/prism-ds-0.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prism-ds-0.2.0rc1.tar", last modified: Wed Jun 28 01:56:10 2023, max compression
+gzip compressed data, was "prism-ds-0.2.0rc2.tar", last modified: Thu Jul 20 02:38:10 2023, max compression
```

## Comparing `prism-ds-0.2.0rc1.tar` & `prism-ds-0.2.0rc2.tar`

### file list

```diff
@@ -1,450 +1,473 @@
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.661272 prism-ds-0.2.0rc1/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11312 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc1/LICENSE
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      219 2023-05-16 12:01:01.000000 prism-ds-0.2.0rc1/MANIFEST.in
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5536 2023-06-28 01:56:10.661401 prism-ds-0.2.0rc1/PKG-INFO
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4572 2023-05-16 12:50:41.000000 prism-ds-0.2.0rc1/README.md
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.560805 prism-ds-0.2.0rc1/prism/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:34:22.000000 prism-ds-0.2.0rc1/prism/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/admin.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.562640 prism-ds-0.2.0rc1/prism/agents/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/agents/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7797 2023-06-28 00:35:11.000000 prism-ds-0.2.0rc1/prism/agents/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    18553 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/agents/docker_agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    37258 2023-06-28 00:56:35.000000 prism-ds-0.2.0rc1/prism/agents/ec2.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      533 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/agents/meta.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.563271 prism-ds-0.2.0rc1/prism/agents/scripts/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-16 12:00:13.000000 prism-ds-0.2.0rc1/prism/agents/scripts/__init__.py
--rwxr-xr-x   0 mihirtrivedi   (501) staff       (20)     3307 2023-06-28 01:07:53.000000 prism-ds-0.2.0rc1/prism/agents/scripts/apply.sh
--rwxr-xr-x   0 mihirtrivedi   (501) staff       (20)      710 2023-06-28 01:05:16.000000 prism-ds-0.2.0rc1/prism/agents/scripts/run.sh
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.565817 prism-ds-0.2.0rc1/prism/cli/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc1/prism/cli/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9934 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/cli/agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7058 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/cli/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8047 2023-06-28 01:31:58.000000 prism-ds-0.2.0rc1/prism/cli/compile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4457 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/cli/connect.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4222 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/cli/create_agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4835 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/cli/create_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4444 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/cli/create_trigger.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5445 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/cli/graph.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5506 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/cli/init.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9408 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/cli/run.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      724 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/cli/spark_submit.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.566092 prism-ds-0.2.0rc1/prism/client/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    12170 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/client/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4973 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/constants.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.567065 prism-ds-0.2.0rc1/prism/decorators/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/decorators/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7124 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/decorators/target.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3116 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/decorators/task.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.567249 prism-ds-0.2.0rc1/prism/docs/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       79 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/docs/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.570425 prism-ds-0.2.0rc1/prism/docs/build/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    50665 2023-03-25 19:27:00.000000 prism-ds-0.2.0rc1/prism/docs/build/311ea03002abadcdcaba.png
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6035 2023-03-25 19:27:00.000000 prism-ds-0.2.0rc1/prism/docs/build/54968a39190c43d592b9.svg
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15406 2023-03-25 19:27:00.000000 prism-ds-0.2.0rc1/prism/docs/build/737ad70b3f2d3a9b5f6e.ico
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       86 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/docs/build/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4653 2023-03-25 19:27:00.000000 prism-ds-0.2.0rc1/prism/docs/build/ce188596011a8fa32931.png
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)   560665 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/docs/build/index.html
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      961 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/docs/build/main.js.LICENSE.txt
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.570776 prism-ds-0.2.0rc1/prism/event_managers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc1/prism/event_managers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6081 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/event_managers/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7589 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/exceptions.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.572631 prism-ds-0.2.0rc1/prism/infra/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc1/prism/infra/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13457 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/infra/compiler.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13019 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/infra/executor.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2401 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/infra/hooks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2811 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/infra/manifest.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7801 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/infra/module.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3635 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/infra/pipeline.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    17171 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/infra/project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1673 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/infra/sys_path.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      816 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/infra/task_manager.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    25019 2023-06-28 01:11:01.000000 prism-ds-0.2.0rc1/prism/main.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.578188 prism-ds-0.2.0rc1/prism/mixins/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.2.0rc1/prism/mixins/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2405 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/mixins/agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2823 2023-06-08 13:53:30.000000 prism-ds-0.2.0rc1/prism/mixins/aws.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1124 2023-04-02 17:52:18.000000 prism-ds-0.2.0rc1/prism/mixins/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8194 2023-06-28 01:33:28.000000 prism-ds-0.2.0rc1/prism/mixins/compile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7301 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/mixins/connect.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2312 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/mixins/create_agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5716 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/mixins/create_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5428 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/mixins/create_trigger.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2438 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/mixins/graph.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1107 2023-04-02 17:52:18.000000 prism-ds-0.2.0rc1/prism/mixins/run.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4244 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/mixins/sys_handler.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.578896 prism-ds-0.2.0rc1/prism/parsers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc1/prism/parsers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    24860 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/parsers/ast_parser.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2206 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/parsers/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3049 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/parsers/yml_parser.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    21581 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/prism_logging.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.581855 prism-ds-0.2.0rc1/prism/profiles/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc1/prism/profiles/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2745 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/profiles/adapter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3611 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/profiles/bigquery.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15601 2023-05-15 03:40:20.000000 prism-ds-0.2.0rc1/prism/profiles/dbt.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      539 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/profiles/meta.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4501 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/profiles/postgres.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9117 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/profiles/profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4089 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/profiles/pyspark.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4491 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/profiles/redshift.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4077 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/profiles/snowflake.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6292 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/profiles/trino.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.582390 prism-ds-0.2.0rc1/prism/spark/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc1/prism/spark/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      439 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/spark/script.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2889 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/spark/wrapper.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1582 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/target.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5171 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/task.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.582559 prism-ds-0.2.0rc1/prism/templates/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:55:51.000000 prism-ds-0.2.0rc1/prism/templates/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.582987 prism-ds-0.2.0rc1/prism/templates/agents/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       59 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/templates/agents/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      233 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/templates/agents/docker.yml
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      191 2023-05-20 15:36:38.000000 prism-ds-0.2.0rc1/prism/templates/agents/ec2.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.583740 prism-ds-0.2.0rc1/prism/templates/minimal_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-16 12:31:03.000000 prism-ds-0.2.0rc1/prism/templates/minimal_project/.gitignore
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/templates/minimal_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.584348 prism-ds-0.2.0rc1/prism/templates/minimal_project/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-05-30 01:38:51.000000 prism-ds-0.2.0rc1/prism/templates/minimal_project/modules/class_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      938 2023-05-30 01:39:48.000000 prism-ds-0.2.0rc1/prism/templates/minimal_project/modules/decorated_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1328 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/templates/minimal_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.584681 prism-ds-0.2.0rc1/prism/templates/profile/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/templates/profile/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.584863 prism-ds-0.2.0rc1/prism/templates/profile/bigquery/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      148 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/templates/profile/bigquery/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.585106 prism-ds-0.2.0rc1/prism/templates/profile/dbt/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      141 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/templates/profile/dbt/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.585368 prism-ds-0.2.0rc1/prism/templates/profile/postgres/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/templates/profile/postgres/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.585557 prism-ds-0.2.0rc1/prism/templates/profile/pyspark/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      478 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/templates/profile/pyspark/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.585707 prism-ds-0.2.0rc1/prism/templates/profile/redshift/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/templates/profile/redshift/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.585867 prism-ds-0.2.0rc1/prism/templates/profile/snowflake/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      193 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/templates/profile/snowflake/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.586027 prism-ds-0.2.0rc1/prism/templates/profile/trino/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      189 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/templates/profile/trino/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.586786 prism-ds-0.2.0rc1/prism/templates/starter_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc1/prism/templates/starter_project/.gitignore
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/templates/starter_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.587056 prism-ds-0.2.0rc1/prism/templates/starter_project/data/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.2.0rc1/prism/templates/starter_project/data/.exists
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.587149 prism-ds-0.2.0rc1/prism/templates/starter_project/dev/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      788 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc1/prism/templates/starter_project/dev/dev.ipynb
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.587687 prism-ds-0.2.0rc1/prism/templates/starter_project/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-05-30 01:39:55.000000 prism-ds-0.2.0rc1/prism/templates/starter_project/modules/class_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      938 2023-05-30 01:39:55.000000 prism-ds-0.2.0rc1/prism/templates/starter_project/modules/decorated_task.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.587940 prism-ds-0.2.0rc1/prism/templates/starter_project/output/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.2.0rc1/prism/templates/starter_project/output/.exists
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1114 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/templates/starter_project/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/templates/starter_project/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.589246 prism-ds-0.2.0rc1/prism/templates/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      426 2023-05-27 16:07:03.000000 prism-ds-0.2.0rc1/prism/templates/tasks/pyspark_cls.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      427 2023-05-27 16:07:03.000000 prism-ds-0.2.0rc1/prism/templates/tasks/pyspark_dec.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      426 2023-05-27 16:07:03.000000 prism-ds-0.2.0rc1/prism/templates/tasks/python_cls.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      427 2023-05-27 16:07:03.000000 prism-ds-0.2.0rc1/prism/templates/tasks/python_dec.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      155 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/templates/tasks/sql.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.590032 prism-ds-0.2.0rc1/prism/templates/triggers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/templates/triggers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      267 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/templates/triggers/function.yml
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      208 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/templates/triggers/prism_project.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.590323 prism-ds-0.2.0rc1/prism/tests/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc1/prism/tests/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.592997 prism-ds-0.2.0rc1/prism/tests/integration/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc1/prism/tests/integration/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7872 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/tests/integration/integration_test_class.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    14197 2023-05-15 03:40:20.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_client.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7755 2023-06-26 11:22:36.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_compile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10444 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_connect.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6520 2023-05-27 16:07:03.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_create.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4020 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_dbt.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5738 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_hooks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4539 2023-05-30 01:42:39.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_init.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.550429 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.593696 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/001_init/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/001_init/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.594251 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/001_init/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-05-30 01:39:55.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/001_init/modules/class_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      938 2023-05-30 01:39:55.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/001_init/modules/decorated_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1122 2023-06-28 01:34:52.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/001_init/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/001_init/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.594601 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/001a_init_minimal/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/001a_init_minimal/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.595088 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/001a_init_minimal/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-05-30 01:38:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/001a_init_minimal/modules/class_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      938 2023-05-30 01:39:48.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/001a_init_minimal/modules/decorated_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1345 2023-06-28 01:34:52.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.595406 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/002_no_project_py/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/002_no_project_py/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/002_no_project_py/functions.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.596267 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/002_no_project_py/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      835 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      867 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      867 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.596604 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/003_project_with_cycle/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/003_project_with_cycle/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.597253 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/003_project_with_cycle/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      888 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      921 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.597647 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/004_simple_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/004_simple_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.598370 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/004_simple_project/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/004_simple_project/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/004_simple_project/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      917 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/004_simple_project/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1035 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/004_simple_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.599085 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/005_simple_project_no_null/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/005_simple_project_no_null/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/005_simple_project_no_null/functions.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.599866 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1031 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1152 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      986 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/005_simple_project_no_null/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.600212 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/006_simple_project_with_profile/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/006_simple_project_with_profile/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.601536 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1104 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      986 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1259 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.601932 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/007_spark_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/007_spark_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.602655 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/007_spark_project/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1790 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/007_spark_project/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1176 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/007_spark_project/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1051 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/007_spark_project/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      622 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/007_spark_project/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/007_spark_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.603004 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/008_targets/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/008_targets/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.605481 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/008_targets/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      973 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/008_targets/modules/csv.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1535 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/008_targets/modules/csv_iter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1589 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/008_targets/modules/csv_mult.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1796 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/008_targets/modules/parquet.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      494 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/008_targets/modules/txt.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/008_targets/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.605642 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/009_simple_dbt_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/009_simple_dbt_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.605752 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.606100 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      576 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/bad_adapter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      583 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/filter_customers.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.606402 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/010_project_nested_module_dirs/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/010_project_nested_module_dirs/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.606672 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.607028 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1112 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.607210 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      994 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.607474 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/011_bad_task_ref/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/011_bad_task_ref/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.607630 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/011_bad_task_ref/modules/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.607999 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1120 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.608160 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      994 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.608442 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/012_concurrency/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/012_concurrency/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.609127 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/012_concurrency/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1242 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/012_concurrency/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1245 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/012_concurrency/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1188 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/012_concurrency/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/012_concurrency/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/012_concurrency/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.609411 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/013_hooks_sql_spark/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/013_hooks_sql_spark/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.610125 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1359 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1090 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1838 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2154 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.610415 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/014_test_triggers_normal/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/014_test_triggers_normal/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.610924 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/014_test_triggers_normal/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      362 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/014_test_triggers_normal/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      347 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/014_test_triggers_normal/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.611287 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/015_test_triggers_no_dir/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/015_test_triggers_no_dir/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.611562 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/015_test_triggers_no_dir/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      362 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/015_test_triggers_no_dir/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1153 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.612141 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/016_test_triggers_error/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/016_test_triggers_error/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.612312 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/016_test_triggers_error/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/016_test_triggers_error/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/016_test_triggers_error/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.613314 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/017_test_triggers_extra_key/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/017_test_triggers_extra_key/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.613531 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/017_test_triggers_extra_key/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.614278 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/018_test_triggers_no_include/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/018_test_triggers_no_include/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.614555 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/018_test_triggers_no_include/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.614949 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/019_dec_targets/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/019_dec_targets/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.615499 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/019_dec_targets/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      578 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/019_dec_targets/modules/extract.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      620 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/019_dec_targets/modules/load.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/019_dec_targets/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.616204 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/020_dec_retries/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/020_dec_retries/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.616648 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/020_dec_retries/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      399 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/020_dec_retries/modules/extract.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      703 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/020_dec_retries/modules/load.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/020_dec_retries/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/020_dec_retries/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.616962 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/021_no_py_in_ref/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/021_no_py_in_ref/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.617924 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/021_no_py_in_ref/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1031 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/021_no_py_in_ref/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1149 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/021_no_py_in_ref/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/021_no_py_in_ref/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      919 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/021_no_py_in_ref/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/021_no_py_in_ref/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.618224 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/common/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/common/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      376 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_projects/common/functions.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    38789 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_run.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11839 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_spark_submit.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5323 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/tests/integration/test_targets.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.620653 prism-ds-0.2.0rc1/prism/tests/unit/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc1/prism/tests/unit/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.620902 prism-ds-0.2.0rc1/prism/tests/unit/dummy_modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/unit/dummy_modules/dummy_module1.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13721 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_adapter_profile.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.621004 prism-ds-0.2.0rc1/prism/tests/unit/test_agent/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1232 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_agent/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10137 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_agents.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    26210 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_dag_fns.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.621162 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       77 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.622470 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/dag_cycle/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      173 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/dag_cycle/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      224 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleE.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.625531 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      436 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      211 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module05.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module06.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module07.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module08.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module09.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module10.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module11.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module12.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module13.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module14.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module15.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.626475 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      134 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      183 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      211 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      210 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module03.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.627738 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      179 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleE.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.630959 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_norefs/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      179 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_norefs/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleE.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.634081 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_selfref/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_selfref/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      175 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleE.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      405 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_import.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4992 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_jinja.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10289 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_module_parser_cls.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9472 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_module_parser_dec.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.654382 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      143 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/bad_run_extra_arg.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      127 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/bad_run_missing_arg.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      135 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/bad_run_no_tasks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       92 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/dec_bad_dec_no_parentheses.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      105 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/dec_bad_run_extra_arg.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       87 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/dec_bad_run_missing_arg.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      124 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/dec_diff_decorator_structure.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      156 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/dec_multiple_prism_tasks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       49 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/dec_no_prism_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       93 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/dec_one_prism_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/dec_other_functions.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      301 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/dec_task_with_target.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      451 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/dec_tasks_refs.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      133 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/diff_import_structure.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      173 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/if_name_main.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      226 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/multiple_prism_tasks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      120 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/no_prism_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      121 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/no_run_func.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      133 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/one_prism_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      199 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/other_classes.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      332 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/task_with_target.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      345 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_modules/tasks_refs.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.658006 prism-ds-0.2.0rc1/prism/tests/unit/test_prism_project_py/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_prism_project_py/bad_trigger_key.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      915 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_prism_project_py/multiple_profiles.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      879 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_prism_project_py/no_profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      909 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_prism_project_py/non_null_profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      894 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_prism_project_py/null_profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1002 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1002 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      998 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_prism_project_py/triggers_normal.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7556 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8920 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_trigger.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.659062 prism-ds-0.2.0rc1/prism/tests/unit/test_trigger_yml/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_trigger_yml/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      111 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc1/prism/tests/unit/test_trigger_yml/test_fn.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.659333 prism-ds-0.2.0rc1/prism/triggers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19500 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc1/prism/triggers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      810 2023-05-04 14:39:42.000000 prism-ds-0.2.0rc1/prism/ui.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-06-28 01:56:10.661149 prism-ds-0.2.0rc1/prism_ds.egg-info/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5536 2023-06-28 01:56:10.000000 prism-ds-0.2.0rc1/prism_ds.egg-info/PKG-INFO
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    18049 2023-06-28 01:56:10.000000 prism-ds-0.2.0rc1/prism_ds.egg-info/SOURCES.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-06-28 01:56:10.000000 prism-ds-0.2.0rc1/prism_ds.egg-info/dependency_links.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       44 2023-06-28 01:56:10.000000 prism-ds-0.2.0rc1/prism_ds.egg-info/entry_points.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-06-26 13:49:56.000000 prism-ds-0.2.0rc1/prism_ds.egg-info/not-zip-safe
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      550 2023-06-28 01:56:10.000000 prism-ds-0.2.0rc1/prism_ds.egg-info/requires.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       11 2023-06-28 01:56:10.000000 prism-ds-0.2.0rc1/prism_ds.egg-info/top_level.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      743 2022-11-12 14:33:04.000000 prism-ds-0.2.0rc1/pyproject.toml
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1754 2023-06-28 01:56:10.661819 prism-ds-0.2.0rc1/setup.cfg
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       70 2023-05-04 13:05:27.000000 prism-ds-0.2.0rc1/setup.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.452599 prism-ds-0.2.0rc2/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11312 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/LICENSE
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      219 2023-05-16 12:01:01.000000 prism-ds-0.2.0rc2/MANIFEST.in
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5536 2023-07-20 02:38:10.452732 prism-ds-0.2.0rc2/PKG-INFO
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4572 2023-05-16 12:50:41.000000 prism-ds-0.2.0rc2/README.md
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.364681 prism-ds-0.2.0rc2/prism/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:34:22.000000 prism-ds-0.2.0rc2/prism/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/admin.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.365970 prism-ds-0.2.0rc2/prism/agents/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/agents/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7762 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/agents/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    18549 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/agents/docker_agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    37974 2023-07-20 02:37:50.000000 prism-ds-0.2.0rc2/prism/agents/ec2.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      533 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/agents/meta.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.366576 prism-ds-0.2.0rc2/prism/agents/scripts/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-16 12:00:13.000000 prism-ds-0.2.0rc2/prism/agents/scripts/__init__.py
+-rwxr-xr-x   0 mihirtrivedi   (501) staff       (20)     3447 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/agents/scripts/apply.sh
+-rwxr-xr-x   0 mihirtrivedi   (501) staff       (20)      710 2023-06-28 01:05:16.000000 prism-ds-0.2.0rc2/prism/agents/scripts/run.sh
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.369826 prism-ds-0.2.0rc2/prism/cli/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/cli/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10729 2023-07-20 02:05:38.000000 prism-ds-0.2.0rc2/prism/cli/agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7470 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/cli/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10421 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/cli/compile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4457 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/cli/connect.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4222 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/cli/create_agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4817 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/cli/create_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4444 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/cli/create_trigger.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5443 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/cli/graph.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5506 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/cli/init.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9402 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/cli/run.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      724 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/cli/spark_submit.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.370198 prism-ds-0.2.0rc2/prism/client/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    16701 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/client/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4973 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/constants.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.371033 prism-ds-0.2.0rc2/prism/decorators/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/decorators/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7124 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/decorators/target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3116 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/decorators/task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.371213 prism-ds-0.2.0rc2/prism/docs/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       79 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/docs/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.374847 prism-ds-0.2.0rc2/prism/docs/build/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    50665 2023-07-18 21:18:50.000000 prism-ds-0.2.0rc2/prism/docs/build/311ea03002abadcdcaba.png
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6035 2023-07-18 21:18:50.000000 prism-ds-0.2.0rc2/prism/docs/build/54968a39190c43d592b9.svg
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15406 2023-07-18 21:18:50.000000 prism-ds-0.2.0rc2/prism/docs/build/737ad70b3f2d3a9b5f6e.ico
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       79 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/docs/build/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4653 2023-07-18 21:18:50.000000 prism-ds-0.2.0rc2/prism/docs/build/ce188596011a8fa32931.png
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)   560712 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/docs/build/index.html
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      961 2023-07-18 21:18:50.000000 prism-ds-0.2.0rc2/prism/docs/build/main.js.LICENSE.txt
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.375179 prism-ds-0.2.0rc2/prism/event_managers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/event_managers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6081 2023-07-13 03:54:01.000000 prism-ds-0.2.0rc2/prism/event_managers/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7852 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/exceptions.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.379950 prism-ds-0.2.0rc2/prism/infra/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/infra/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6833 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/infra/compiled_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    14303 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/infra/compiler.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13388 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/infra/executor.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3900 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/infra/hooks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2704 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/infra/manifest.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3716 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/infra/pipeline.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    17198 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/infra/project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1421 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/infra/sys_path.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2628 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/infra/task_manager.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    24529 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/main.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.382216 prism-ds-0.2.0rc2/prism/mixins/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.2.0rc2/prism/mixins/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2405 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/mixins/agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2823 2023-06-08 13:53:30.000000 prism-ds-0.2.0rc2/prism/mixins/aws.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1288 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/mixins/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11668 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/mixins/compile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7301 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/mixins/connect.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2312 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/mixins/create_agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5706 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/mixins/create_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5428 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/mixins/create_trigger.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2438 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/mixins/graph.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1107 2023-04-02 17:52:18.000000 prism-ds-0.2.0rc2/prism/mixins/run.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4232 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/mixins/sys_handler.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.383179 prism-ds-0.2.0rc2/prism/parsers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/parsers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    31631 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/parsers/ast_parser.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2206 2023-07-15 21:15:27.000000 prism-ds-0.2.0rc2/prism/parsers/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3049 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/parsers/yml_parser.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    22013 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/prism_logging.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.385817 prism-ds-0.2.0rc2/prism/profiles/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/profiles/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2745 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/profiles/adapter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3733 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/profiles/bigquery.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15570 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/profiles/dbt.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      539 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/profiles/meta.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4567 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/profiles/postgres.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9117 2023-07-05 11:15:15.000000 prism-ds-0.2.0rc2/prism/profiles/profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4089 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/profiles/pyspark.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4557 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/profiles/redshift.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4176 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/profiles/snowflake.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6358 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/profiles/trino.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.386484 prism-ds-0.2.0rc2/prism/spark/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/spark/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      439 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/spark/script.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2889 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/spark/wrapper.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1448 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5171 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.386666 prism-ds-0.2.0rc2/prism/templates/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:55:51.000000 prism-ds-0.2.0rc2/prism/templates/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.387448 prism-ds-0.2.0rc2/prism/templates/agents/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       59 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/templates/agents/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      233 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/templates/agents/docker.yml
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      191 2023-05-20 15:36:38.000000 prism-ds-0.2.0rc2/prism/templates/agents/ec2.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.388294 prism-ds-0.2.0rc2/prism/templates/minimal_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-16 12:31:03.000000 prism-ds-0.2.0rc2/prism/templates/minimal_project/.gitignore
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/templates/minimal_project/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1326 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/templates/minimal_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.388859 prism-ds-0.2.0rc2/prism/templates/minimal_project/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/templates/minimal_project/tasks/class_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      937 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/templates/minimal_project/tasks/decorated_task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.389124 prism-ds-0.2.0rc2/prism/templates/profile/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/templates/profile/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.389292 prism-ds-0.2.0rc2/prism/templates/profile/bigquery/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      148 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/templates/profile/bigquery/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.389627 prism-ds-0.2.0rc2/prism/templates/profile/dbt/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      141 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/templates/profile/dbt/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.389904 prism-ds-0.2.0rc2/prism/templates/profile/postgres/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/templates/profile/postgres/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.390078 prism-ds-0.2.0rc2/prism/templates/profile/pyspark/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      478 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/templates/profile/pyspark/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.390241 prism-ds-0.2.0rc2/prism/templates/profile/redshift/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/templates/profile/redshift/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.390481 prism-ds-0.2.0rc2/prism/templates/profile/snowflake/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      193 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/templates/profile/snowflake/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.390701 prism-ds-0.2.0rc2/prism/templates/profile/trino/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      189 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/templates/profile/trino/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.391420 prism-ds-0.2.0rc2/prism/templates/starter_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/templates/starter_project/.gitignore
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/templates/starter_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.391680 prism-ds-0.2.0rc2/prism/templates/starter_project/data/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.2.0rc2/prism/templates/starter_project/data/.exists
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.391779 prism-ds-0.2.0rc2/prism/templates/starter_project/dev/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      786 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/templates/starter_project/dev/dev.ipynb
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.391981 prism-ds-0.2.0rc2/prism/templates/starter_project/output/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.2.0rc2/prism/templates/starter_project/output/.exists
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1112 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/templates/starter_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.392308 prism-ds-0.2.0rc2/prism/templates/starter_project/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/templates/starter_project/tasks/class_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      938 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/templates/starter_project/tasks/decorated_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/templates/starter_project/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.394798 prism-ds-0.2.0rc2/prism/templates/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      426 2023-05-27 16:07:03.000000 prism-ds-0.2.0rc2/prism/templates/tasks/pyspark_cls.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      427 2023-05-27 16:07:03.000000 prism-ds-0.2.0rc2/prism/templates/tasks/pyspark_dec.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      426 2023-05-27 16:07:03.000000 prism-ds-0.2.0rc2/prism/templates/tasks/python_cls.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      427 2023-05-27 16:07:03.000000 prism-ds-0.2.0rc2/prism/templates/tasks/python_dec.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      155 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/templates/tasks/sql.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.395416 prism-ds-0.2.0rc2/prism/templates/triggers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/templates/triggers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      267 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/templates/triggers/function.yml
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      208 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/templates/triggers/prism_project.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.395859 prism-ds-0.2.0rc2/prism/tests/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/tests/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.399003 prism-ds-0.2.0rc2/prism/tests/integration/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/tests/integration/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7886 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/integration_test_class.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15381 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_client.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10484 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_compile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10444 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_connect.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6512 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_create.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4012 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_dbt.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5728 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_hooks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4539 2023-05-30 01:42:39.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_init.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.359850 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.399672 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1120 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.400135 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/tasks/class_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      938 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/tasks/decorated_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.400469 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001a_init_minimal/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001a_init_minimal/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1343 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.400824 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001a_init_minimal/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001a_init_minimal/tasks/class_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      937 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001a_init_minimal/tasks/decorated_task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.401105 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/functions.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.401768 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      825 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      857 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      857 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.402036 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.403634 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      806 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      807 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.404089 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.405454 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      935 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1027 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      801 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1033 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.406175 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/functions.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.407129 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1100 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      868 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      808 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.407657 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/functions.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.408381 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1127 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      923 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      913 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module04.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.408741 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.409715 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      969 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1090 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      974 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      910 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1257 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.410064 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.411306 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1751 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/tasks/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1139 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/tasks/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      940 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/tasks/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      636 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/tasks/module04.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.411666 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.413291 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      982 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/csv.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1548 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/csv_iter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1632 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/csv_mult.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1765 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/parquet.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      498 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/txt.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.413546 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/009_simple_dbt_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/009_simple_dbt_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.413709 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.414212 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      569 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/bad_adapter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      576 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/filter_customers.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.414611 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.414853 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.415269 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      934 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1059 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.415513 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      875 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      812 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.415903 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-09 15:09:25.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.416129 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.416718 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      934 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1067 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.416940 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      875 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      812 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.417233 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.418169 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1196 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1195 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1045 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      808 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.418521 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency_local/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency_local/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency_local/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.418952 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency_local/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1239 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency_local/tasks/local_tasks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      597 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency_local/tasks/non_local_task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.419285 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.420350 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1287 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1133 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1871 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2147 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.420822 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/014_test_triggers_normal/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/014_test_triggers_normal/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.421381 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/014_test_triggers_normal/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      358 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/014_test_triggers_normal/tasks/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      345 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/014_test_triggers_normal/tasks/module02.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.421798 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/015_test_triggers_no_dir/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/015_test_triggers_no_dir/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1151 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.422011 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/015_test_triggers_no_dir/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      358 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/015_test_triggers_no_dir/tasks/module01.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.422549 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/016_test_triggers_error/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/016_test_triggers_error/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.422812 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/016_test_triggers_error/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/016_test_triggers_error/tasks/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/016_test_triggers_error/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.423363 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.423677 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/tasks/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.424203 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.424514 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/tasks/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.424792 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/019_dec_targets/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/019_dec_targets/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/019_dec_targets/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.425111 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/019_dec_targets/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      578 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/019_dec_targets/tasks/extract.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      620 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/019_dec_targets/tasks/load.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.425531 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/020_dec_retries/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/020_dec_retries/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/020_dec_retries/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.425933 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/020_dec_retries/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      399 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/020_dec_retries/tasks/extract.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      703 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/020_dec_retries/tasks/load.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/020_dec_retries/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.426219 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/021_project_with_local_tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/021_project_with_local_tasks/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/021_project_with_local_tasks/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.426564 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      628 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/extract.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      952 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/transform_load.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.426833 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.427342 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      388 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/tasks/extract.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      785 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/tasks/transform_load.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.428013 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/common/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/common/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      376 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_projects/common/functions.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    54103 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_run.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    14051 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_spark_submit.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5594 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/integration/test_targets.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.431035 prism-ds-0.2.0rc2/prism/tests/unit/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/tests/unit/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.431328 prism-ds-0.2.0rc2/prism/tests/unit/dummy_modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/tests/unit/dummy_modules/dummy_module1.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13721 2023-06-28 00:14:15.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_adapter_profile.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.431498 prism-ds-0.2.0rc2/prism/tests/unit/test_agent/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1230 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_agent/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10244 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_agents.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    28403 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_dag_fns.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.431701 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       65 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.432778 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/dag_cycle/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/dag_cycle/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      173 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      150 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      204 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      204 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleE.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.436005 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      467 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      125 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      146 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      172 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task05.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task06.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      365 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task07.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task08.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      169 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task09.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task10.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      179 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task11.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task12.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task13.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      150 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task14.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      150 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task15.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.436777 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      123 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/task01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      146 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/task02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      145 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/task03.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.440008 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      247 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      148 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      148 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskE.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.440985 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      251 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleE.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.441872 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      253 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleE.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    25008 2023-07-20 00:59:23.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_ast_parser.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      405 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_import.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4992 2023-05-26 22:30:47.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_jinja.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.443367 prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/bad_trigger_key.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      915 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/multiple_profiles.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      879 2022-08-08 04:50:27.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/no_profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      909 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/non_null_profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      894 2023-03-01 23:08:44.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/null_profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1000 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1000 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      996 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/triggers_normal.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7948 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.448652 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      133 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_bad_run_extra_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      117 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_bad_run_missing_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      125 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_bad_run_no_tasks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      123 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_diff_import_structure.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      163 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_if_name_main.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_multiple_prism_tasks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      118 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_no_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      111 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_no_run_func.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      123 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_one_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_other_classes.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      346 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_task_with_target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      329 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/cls_tasks_refs.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       92 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_bad_dec_no_parentheses.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      105 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_bad_run_extra_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       87 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_bad_run_missing_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      124 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_diff_decorator_structure.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      156 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_multiple_prism_tasks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       49 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_no_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       93 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_one_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_other_functions.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      301 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_task_with_target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      361 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/dec_tasks_refs.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.449669 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/refd_tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/refd_tasks/func_0.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/refd_tasks/func_1.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/refd_tasks/hello.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_tasks/refd_tasks/world.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8773 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_trigger.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.450142 prism-ds-0.2.0rc2/prism/tests/unit/test_trigger_yml/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      936 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_trigger_yml/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      111 2023-04-04 01:59:51.000000 prism-ds-0.2.0rc2/prism/tests/unit/test_trigger_yml/test_fn.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.450433 prism-ds-0.2.0rc2/prism/triggers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19492 2023-07-20 00:59:24.000000 prism-ds-0.2.0rc2/prism/triggers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      810 2023-05-04 14:39:42.000000 prism-ds-0.2.0rc2/prism/ui.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 02:38:10.452396 prism-ds-0.2.0rc2/prism_ds.egg-info/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5536 2023-07-20 02:38:10.000000 prism-ds-0.2.0rc2/prism_ds.egg-info/PKG-INFO
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19334 2023-07-20 02:38:10.000000 prism-ds-0.2.0rc2/prism_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-07-20 02:38:10.000000 prism-ds-0.2.0rc2/prism_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       44 2023-07-20 02:38:10.000000 prism-ds-0.2.0rc2/prism_ds.egg-info/entry_points.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-06-26 13:49:56.000000 prism-ds-0.2.0rc2/prism_ds.egg-info/not-zip-safe
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      550 2023-07-20 02:38:10.000000 prism-ds-0.2.0rc2/prism_ds.egg-info/requires.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       11 2023-07-20 02:38:10.000000 prism-ds-0.2.0rc2/prism_ds.egg-info/top_level.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      743 2022-11-12 14:33:04.000000 prism-ds-0.2.0rc2/pyproject.toml
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1754 2023-07-20 02:38:10.453360 prism-ds-0.2.0rc2/setup.cfg
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       70 2023-05-04 13:05:27.000000 prism-ds-0.2.0rc2/setup.py
```

### Comparing `prism-ds-0.2.0rc1/LICENSE` & `prism-ds-0.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/PKG-INFO` & `prism-ds-0.2.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prism-ds
-Version: 0.2.0rc1
+Version: 0.2.0rc2
 Summary: The easiest way to create data pipelines in Python.
 Author: prism founders
 Author-email: hello@runprism.com
 License: Apache-2.0
 Project-URL: homepage, https://www.runprism.com
 Project-URL: documentation, https://docs.runprism.com
 Project-URL: repository, https://github.com/runprism/prism
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prism-ds Version: 0.2.0rc1 Summary: The easiest way
+Metadata-Version: 2.1 Name: prism-ds Version: 0.2.0rc2 Summary: The easiest way
 to create data pipelines in Python. Author: prism founders Author-email:
 hello@runprism.com License: Apache-2.0 Project-URL: homepage, https://
 www.runprism.com Project-URL: documentation, https://docs.runprism.com Project-
 URL: repository, https://github.com/runprism/prism Platform: unix Platform:
 linux Platform: osx Platform: win32 Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `prism-ds-0.2.0rc1/README.md` & `prism-ds-0.2.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/admin.py` & `prism-ds-0.2.0rc2/prism/admin.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/agents/base.py` & `prism-ds-0.2.0rc2/prism/agents/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 
         # If no exception has been raised, return True
         return True
 
     def prepare_paths_for_copy(self, project: PrismProject, tmpdir: str):
         """
         Prism projects often rely on more than just their own directory. They can import
-        functions / modules or reference configuration files from other directories. We
+        functions / tasks or reference configuration files from other directories. We
         need to copy all relevant directories into our agent, and we need to ensure that
         these paths have the same relative location to the project directory.
 
         args:
             project: Prism project
         returns:
             commands to copy directories into agent's computing environment
@@ -170,33 +170,33 @@
         """
 
         # Construct command
         full_tb = self.args.full_tb
         log_level = self.args.log_level
         vars = self.args.vars
         context = self.args.context
-        modules = self.args.modules
+        tasks = self.args.tasks
         all_upstream = self.args.all_upstream
         all_downstream = self.args.all_downstream
 
         # Namespace to string conversion
         full_tb_cmd = "" if not full_tb else "--full-tb"
         log_level_cmd = "" if log_level == "info" else f"--log-level {log_level}"
         vars_cmd = "" if vars is None else " ".join([
             f"{k}={v}" for k, v in vars.items()
         ])
         context_cmd = "" if context == '{}' else f"--context '{context}'"
-        modules_cmd = "" if modules is None else " " .join([
-            f"--module {m.replace('.py', '')}" for m in modules
+        tasks_cmd = "" if tasks is None else " " .join([
+            f"--task {m}" for m in tasks
         ])
         all_upstream_cmd = "" if not all_upstream else "--all-upstream"
         all_downstream_cmd = "" if not all_downstream else "--all-downstream"
 
         # Full command
-        full_cmd = f"prism run {full_tb_cmd} {log_level_cmd} {vars_cmd} {context_cmd} {modules_cmd} {all_upstream_cmd} {all_downstream_cmd}"  # noqa: E501
+        full_cmd = f"prism run {full_tb_cmd} {log_level_cmd} {vars_cmd} {context_cmd} {tasks_cmd} {all_upstream_cmd} {all_downstream_cmd}"  # noqa: E501
         return full_cmd
 
     def parse_environment_variables(self, agent_conf: Dict[str, Any]) -> Dict[str, str]:
         raise prism.exceptions.NotImplementedException(
             message=f"`parse_environment_variables` not implemented for agent {self.__class__.__name__}"  # noqa: E501
         )
```

### Comparing `prism-ds-0.2.0rc1/prism/agents/docker_agent.py` & `prism-ds-0.2.0rc2/prism/agents/docker_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,15 +280,15 @@
 
     def prepare_paths_for_copy(self,
         project: PrismProject,
         tmpdir: str,
     ):
         """
         Prism projects often rely on more than just their own directory. They can import
-        functions / modules or reference configuration files from other directories. We
+        functions / tasks or reference configuration files from other directories. We
         need to copy all relevant directories into our agent, and we need to ensure that
         these paths have the same relative location to the project directory.
 
         args:
             project: Prism project
             tmpdir: temporary directory in which to copy directories
 
@@ -362,15 +362,15 @@
             if not isinstance(agent_conf["image"], str):
                 raise prism.exceptions.InvalidAgentsConfException(
                     "`image` is not correctly specified... should be a string"
                 )
             return agent_conf["image"]
 
         # If the user doesn't specify a base image, then use the default image specified
-        # in the Prism constants module.
+        # in the Prism constants task.
         else:
             return prism.constants.DEFAULT_DOCKER_IMAGE
 
     def parse_environment_variables(self,
         agent_conf: Dict[str, Any]
     ) -> Dict[str, str]:
         """
```

### Comparing `prism-ds-0.2.0rc1/prism/agents/ec2.py` & `prism-ds-0.2.0rc2/prism/agents/ec2.py`

 * *Files 2% similar despite different names*

```diff
@@ -376,15 +376,15 @@
             ]
         else:
             ip_permissions = [
                 {
                     'IpProtocol': 'tcp',
                     'FromPort': 22,
                     'ToPort': 22,
-                    'Ipv6Ranges': [{'CidrIpv6': f'{external_ip}'}]
+                    'Ipv6Ranges': [{'CidrIpv6': f'{external_ip}/128'}]
                 },
             ]
 
         _ = ec2_client.authorize_security_group_ingress(
             GroupId=security_group_id,
             IpPermissions=ip_permissions
         )
@@ -738,15 +738,15 @@
             return []
 
     def get_all_project_paths(self,
         project: PrismProject,
     ):
         """
         Prism projects often rely on more than just their own directory. They can import
-        functions / modules or reference configuration files from other directories. We
+        functions / tasks or reference configuration files from other directories. We
         need to copy all relevant directories into our agent, and we need to ensure that
         these paths have the same relative location to the project directory.
 
         args:
             project: Prism project
         returns:
             list of project paths
@@ -862,15 +862,15 @@
                 output = process.stderr.readline()  # type: ignore
 
             # Stream the logs
             if process.poll() is not None:
                 break
             self._log_output(color, which, output)
 
-        return process.stdout, process.stderr
+        return process.stdout, process.stderr, process.returncode
 
     def apply(self):
         """
         Create the EC2 instance image
         """
         # Fire an empty line -- it just looks a little nicer
         prism.prism_logging.fire_console_event(prism.prism_logging.EmptyLineEvent())
@@ -913,16 +913,25 @@
             '-n', public_dns_name,
             '-d', str(self.project.project_dir),
             '-c', project_paths_cli,
             '-e', env_cli,
         ]
 
         # Open a subprocess and stream the logs
-        return_code = self.stream_logs(cmd, prism.ui.AGENT_WHICH_BUILD, "build")
-        return return_code
+        _, err, returncode = self.stream_logs(cmd, prism.ui.AGENT_WHICH_BUILD, "build")
+
+        # Log anything from stderr that was printed in the project
+        for line in err.readlines():
+            prism.prism_logging.DEFAULT_LOGGER.agent(  # type: ignore
+                f"{prism.ui.AGENT_EVENT}{self.instance_name}{prism.ui.AGENT_WHICH_BUILD}[build]{prism.ui.RESET} | {line.rstrip()}"  # noqa: E501
+            )
+
+        # Return the returncode. Return a dictionary in order to avoid confusing this
+        # output with the output of an event manager.
+        return {"return_code": returncode}
 
     def run(self):
         """
         Run the project using the EC2 agent
         """
         # Full command
         full_cmd = self.construct_command()
@@ -943,22 +952,26 @@
             '/bin/sh', self.AGENT_RUN_SCRIPT,
             '-p', str(self.pem_key_path),
             '-u', 'ec2-user',
             '-n', self.public_dns_name,
             '-d', str(self.project.project_dir),
             '-c', full_cmd,
         ]
-        out, _ = self.stream_logs(cmd, prism.ui.AGENT_WHICH_RUN, "run")
+        out, _, returncode = self.stream_logs(cmd, prism.ui.AGENT_WHICH_RUN, "run")
 
         # Log anything from stdout that was printed in the project
         for line in out.readlines():
             prism.prism_logging.DEFAULT_LOGGER.agent(  # type: ignore
                 f"{prism.ui.AGENT_EVENT}{self.instance_name}{prism.ui.AGENT_WHICH_RUN}[run]{prism.ui.RESET} | {line.rstrip()}"  # noqa: E501
             )
 
+        # Return the returncode. Return a dictionary in order to avoid confusing this
+        # output with the output of an event manager.
+        return {"return_code": returncode}
+
     def delete(self):
         """
         Delete all resources associated with agent. This includes:
             - Key pair
             - Security group
             - Instance
```

### Comparing `prism-ds-0.2.0rc1/prism/agents/meta.py` & `prism-ds-0.2.0rc2/prism/agents/meta.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/agents/scripts/apply.sh` & `prism-ds-0.2.0rc2/prism/agents/scripts/apply.sh`

 * *Files 12% similar despite different names*

```diff
@@ -56,22 +56,24 @@
 
 # Log
 echo "Updating remote project and file paths"
 
 # Copy project directory and other copy paths into the EC2 instance
 ssh -i ${pem_path} ${user}@${public_dns_name} "sudo mkdir -p .${project_dir}; sudo chmod 777 -R .${project_dir}"
 scp -r -i ${pem_path} ${project_dir} ${user}@${public_dns_name}:.${project_dir}
+echo "Copied project directory into instance"
 
 IFS=',' read -ra array <<< "${copy_paths}"
 for path in "${array[@]}"; do
 	# Make a directory and change the permissions
 	ssh -i ${pem_path} ${user}@${public_dns_name} "sudo mkdir -p .${path%/*}; sudo chmod 777 -R .${path%/*}"
 
 	# Copy
 	scp -r -i ${pem_path} ${path} ${user}@${public_dns_name}:.${path%/*} 2> scp.log
+	echo "Copied path ${path} into instance"
 done
 
 # Environment variables. Environment variable are passed a comma-separated list of
 # key-value pairs, i.e. ENV1=value1,ENV2=value2,...
 IFS=',' read -ra env_array <<< "${env}"; unset IFS;
 SED_COMMAND=""
 for keyvalue in "${env_array[@]}"; do
@@ -81,16 +83,16 @@
     if ssh -i ${pem_path} ${user}@${public_dns_name} "grep -q '^export ${key}=' ~/.bashrc"; then
         ssh -i ${pem_path} ${user}@${public_dns_name} "sed -i 's/^export ${key}=.*$/export ${key}=${value}/' ~/.bashrc"
 
     # Add the new key-value pair to the end of .bashrc if it doesn't exist
     else
         ssh -i ${pem_path} ${user}@${public_dns_name} "echo 'export ${key}=${value}' >> ~/.bashrc"
     fi
+	echo "Updated environment variable ${key}=${value}"
 done
 
 # Reload .bashrc to update environment variables
 ssh -i ${pem_path} ${user}@${public_dns_name} "source ~/.bashrc"
 
 # Move all folders into the root folder
 ssh -i ${pem_path} ${user}@${public_dns_name} 'cd ~ && for dir in */; do sudo mv $dir ../../$dir ; done'
-
 echo "Done updating remote project and file paths"
```

### Comparing `prism-ds-0.2.0rc1/prism/agents/scripts/run.sh` & `prism-ds-0.2.0rc2/prism/agents/scripts/run.sh`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/cli/agent.py` & `prism-ds-0.2.0rc2/prism/cli/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,28 +106,28 @@
 
         # If we just want to run the agent, we do that in a separate function call.
         if args.which == "agent-run":
             return agent
 
         elif args.which == "agent-delete":
             agent.delete()
+            return agent
 
         # Otherwise, we either want to build the agent (`prism agent apply`) or build &
         # run the agent (`prism agent build`). We run the agent in a separate function,
         # so focus on just building it for now.
         else:
             agent.apply()
             return agent
 
     def run_agent(self, agent: Agent):
         """
         Thin wrapper around the agent `run` function.
         """
-        agent.run()
-        return
+        return agent.run()
 
     def run(self) -> prism.cli.base.TaskRunReturnResult:
         """
         Create and/or run the project on an agent.
         """
         # Event list
         event_list: List[Event] = []
@@ -227,24 +227,32 @@
             prism_project=self.prism_project,
         )
 
         agent = build_manager_output.outputs
         build_event_to_fire = build_manager_output.event_to_fire
         event_list = build_manager_output.event_list
 
-        # Log an error if one occurs
+        # Log any Python error that we encounter
         if agent == 0:
             event_list = fire_console_event(
                 build_event_to_fire,
                 event_list,
                 log_level='error'
             )
             event_list = self.fire_tail_event(event_list)
             return prism.cli.base.TaskRunReturnResult(event_list, True)
 
+        # If the `apply` script exits with a non-zero return code, then exit
+        if isinstance(agent, dict) and agent["return_code"] != 0:
+            event_list = fire_console_event(
+                prism.prism_logging.SeparatorEvent(),
+                event_list
+            )
+            return prism.cli.base.TaskRunReturnResult(event_list, True)
+
         # ------------------------------------------------------------------------------
         # Execute the agent
 
         if self.args.which in ["agent-apply", "agent-build"]:
             event_list = fire_empty_line_event(event_list)
 
         # Only execute the agent with `agent-run` or `agent-build`
@@ -267,24 +275,32 @@
                 event_list=event_list,
                 agent=agent
             )
             agent_output = agent_event_manager_output.outputs
             agent_event_to_fire = agent_event_manager_output.event_to_fire
             event_list = agent_event_manager_output.event_list
 
-            # Log an error if one occurs
+            # Log any Python error that we encounter
             if agent_output == 0:
                 event_list = fire_console_event(
                     agent_event_to_fire,
                     event_list,
                     log_level='error'
                 )
                 event_list = self.fire_tail_event(event_list)
                 return prism.cli.base.TaskRunReturnResult(event_list, True)
 
+            # If the `run` script exits with a non-zero return code, then return
+            if isinstance(agent_output, dict) and agent_output["return_code"] != 0:
+                event_list = fire_console_event(
+                    prism.prism_logging.SeparatorEvent(),
+                    event_list
+                )
+                return prism.cli.base.TaskRunReturnResult(event_list, True)
+
             # Now, we're done streaming logs
             event_list = fire_empty_line_event()
             event_list = fire_console_event(
                 prism.prism_logging.StreamingLogsEndEvent(),
                 event_list
             )
```

### Comparing `prism-ds-0.2.0rc1/prism/cli/base.py` & `prism-ds-0.2.0rc2/prism/cli/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,22 +47,34 @@
     # Otherwise, check parent directories for prism_project.py file
     root_path = Path(os.sep).resolve()
     cwd = Path.cwd()
 
     while cwd != root_path:
         project_file = cwd / 'prism_project.py'
         if project_file.is_file():
-            if not Path(cwd / 'modules').is_dir():
-                modules_dir_not_found_msg = ' '.join([
-                    'modules directory not found in project directory or any',
-                    'of its parents',
-                ])
-                raise prism.exceptions.ModulesDirNotFoundException(
-                    modules_dir_not_found_msg
-                )
+
+            # Check if `tasks` and/or `modules` directory exist
+            tasks_dir = Path(cwd) / 'tasks'
+            modules_dir = Path(cwd) / 'modules'
+            if not tasks_dir.is_dir():
+
+                # If the `modules`` directory exists, then skip... we'll throw a warning
+                # later
+                if modules_dir.is_dir():
+                    pass
+
+                # Otherwise, throw an error
+                else:
+                    tasks_dir_not_found_msg = ' '.join([
+                        'tasks directory not found in project directory or any',
+                        'of its parents',
+                    ])
+                    raise prism.exceptions.TasksDirNotFoundException(
+                        tasks_dir_not_found_msg
+                    )
             return cwd
         else:
             cwd = cwd.parent
 
     project_py_no_found_msg = ' '.join([
         'prism_project.py file not found in current directory or any',
         'of its parents',
```

### Comparing `prism-ds-0.2.0rc1/prism/cli/compile.py` & `prism-ds-0.2.0rc2/prism/cli/graph.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,231 +1,167 @@
 """
-Compile task class definition, called via `prism compile`
+GenerateDocs class definition, called via `prism gen-docs`
 
 Table of Contents
 - Imports
 - Class definition
 """
 
 
 ###########
 # Imports #
 ###########
 
 # Standard library imports
 import os
-import argparse
-from pathlib import Path
-from typing import List, Optional, Union
+import webbrowser
+from typing import List
+import signal
+from http.server import SimpleHTTPRequestHandler
+from socketserver import TCPServer
+import sys
 
 # Prism-specific imports
 import prism.cli.base
-import prism.mixins.compile
-import prism.exceptions
-import prism.constants
+import prism.cli.compile
 import prism.prism_logging
-from prism.prism_logging import fire_console_event, fire_empty_line_event
-from prism.event_managers.base import BaseEventManager, EventManagerOutput
-from prism.infra.project import PrismProject
+from prism.prism_logging import Event, fire_empty_line_event, fire_console_event
+import prism.mixins.graph
+import prism.event_managers.base as base_event_manager
 
 
-####################
-# Class definition #
-####################
-
-class CompileTask(prism.cli.base.BaseTask, prism.mixins.compile.CompileMixin):
+class GraphTask(prism.cli.compile.CompileTask, prism.mixins.graph.GraphMixin):
     """
-    Class for compiling a prism project and computing the DAG
+    Class for generating Prism documentation
     """
 
-    def run(self) -> prism.cli.base.TaskRunReturnResult:
-        """
-        Run the compile task. This task is executed when the user runs the compile task
-        from the CLI.
-        """
+    def run(self):
 
         # ------------------------------------------------------------------------------
         # Fire header events
 
-        event_list, project_dir = self.fire_header_events()
+        event_list: List[Event] = []
+        event_list, project_dir = self.fire_header_events(event_list)
         if project_dir is None:
             return prism.cli.base.TaskRunReturnResult(event_list)
+        event_list = fire_empty_line_event(event_list)
         os.chdir(project_dir)
 
-        # ------------------------------------------------------------------------------
-        # Define directories and get modules to compile
-
+        # Compiled dir
         compiled_dir = self.create_compiled_dir(project_dir)
 
-        # Modules directory
-        try:
-            modules_dir = self.get_modules_dir(project_dir)
-        except prism.exceptions.CompileException as err:
-            e = prism.prism_logging.PrismExceptionErrorEvent(
-                err,
-                'accessing modules directory'
-            )
-            event_list = fire_console_event(e, event_list, 0, 'error')
-            event_list = self.fire_tail_event(event_list)
-            return prism.cli.base.TaskRunReturnResult(event_list, True)
+        # ------------------------------------------------------------------------------
+        # Create compiled DAG
 
-        # Get modules to compile
-        user_arg_module_em = BaseEventManager(
-            idx=None,
-            total=None,
-            name='grabbing user-specified modules',
-            full_tb=self.args.full_tb,
-            func=self.user_arg_modules
-        )
-        user_arg_module_em_output = user_arg_module_em.manage_events_during_run(
-            fire_exec_events=False,
-            event_list=event_list,
+        result = super().run_for_subclass(
             args=self.args,
-            modules_dir=modules_dir
+            project_dir=project_dir,
+            event_list=event_list,
+            project=None,
+            fire_exec_events=True
         )
-        user_arg_modules = user_arg_module_em_output.outputs
-        event_to_fire = user_arg_module_em_output.event_to_fire
-        event_list = user_arg_module_em_output.event_list
-        if user_arg_modules == 0:
+        if isinstance(result, prism.cli.base.TaskRunReturnResult):
+            return result
+
+        compiled_dag = result.outputs
+        compiled_dag_error_event = result.event_to_fire
+        event_list = result.event_list
+
+        # If no tasks in DAG, return
+        if compiled_dag == 0 and compiled_dag_error_event is not None:
+            event_list = fire_empty_line_event(event_list)
             event_list = fire_console_event(
-                event_to_fire,
+                compiled_dag_error_event,
                 event_list,
                 log_level='error'
             )
             event_list = self.fire_tail_event(event_list)
-            return prism.cli.base.TaskRunReturnResult(event_list, True)
-
-        all_modules = self.get_modules(modules_dir)
-        event_list = fire_empty_line_event(event_list)
+            return prism.cli.base.TaskRunReturnResult(event_list)
 
         # ------------------------------------------------------------------------------
-        # Parse module references
+        # Create / populate the docs folder
 
-        compiler_manager = BaseEventManager(
+        docs_build_manager = base_event_manager.BaseEventManager(
             idx=None,
             total=None,
-            name='module DAG',
+            name='populate docs build',
             full_tb=self.args.full_tb,
-            func=self.compile_dag
+            func=self.populate_docs_build
         )
-        compiled_event_manager_output = compiler_manager.manage_events_during_run(
+        compiled_event_manager_output = docs_build_manager.manage_events_during_run(
             event_list=event_list,
             project_dir=project_dir,
-            compiled_dir=compiled_dir,
-            all_modules=all_modules,
-            user_arg_modules=user_arg_modules
+            compiled_dir=compiled_dir
         )
-        compiled_dag = compiled_event_manager_output.outputs
+        build_path = compiled_event_manager_output.outputs
         event_to_fire = compiled_event_manager_output.event_to_fire
         event_list = compiled_event_manager_output.event_list
-        if compiled_dag == 0:
+
+        # If an error occurred, raise
+        if build_path == 0:
+            event_list = fire_empty_line_event(event_list)
             event_list = fire_console_event(
                 event_to_fire,
                 event_list,
                 log_level='error'
             )
             event_list = self.fire_tail_event(event_list)
-            return prism.cli.base.TaskRunReturnResult(event_list, True)
+            return prism.cli.base.TaskRunReturnResult(event_list)
+
+        # ------------------------------------------------------------------------------
+        # Serve docs
+
+        # Send clean messages when Ctrl+C is pressed
+        def handler(signum, frame):
+            nonlocal event_list
+            event_list = fire_empty_line_event(event_list)
+            res = input('Shutdown the Prism docs server (y/n)? ')
+            if res == "y":
+                event_list = fire_empty_line_event(event_list)
+                event_list = fire_console_event(
+                    prism.prism_logging.TaskSuccessfulEndEvent(),
+                    event_list,
+                    0,
+                    log_level='info'
+                )
+                event_list = self.fire_tail_event(event_list)
+                sys.exit(0)
+            else:
+                # do nothing
+                pass
+
+        signal.signal(signal.SIGINT, handler)
+
+        # Serve the docs
+        os.chdir(build_path)
+        port = self.args.port
+        address = "0.0.0.0"
 
-        # Print output message if successfully executed
         event_list = fire_empty_line_event(event_list)
         event_list = fire_console_event(
-            prism.prism_logging.TaskSuccessfulEndEvent(),
-            event_list,
-            0,
+            prism.prism_logging.ServingDocsEvent(address=address, port=port),
             log_level='info'
         )
-        event_list = self.fire_tail_event(event_list)
-
-        # Return
-        return prism.cli.base.TaskRunReturnResult(event_list)
-
-    def run_for_subclass(self,
-        args: argparse.Namespace,
-        project_dir: Path,
-        event_list: List[prism.prism_logging.Event],
-        project: Optional[PrismProject] = None,
-        fire_exec_events: bool = True
-    ) -> Union[prism.cli.base.TaskRunReturnResult, EventManagerOutput]:
-        """
-        Run the compile task. This task is executed when the user runs a subclass of the
-        CompileTask (e.g., the RunTask)
-
-        args:
-            args: user arguments
-            project_dir: project directory
-            compiled_dir: directory to store manifest.json
-            event_list: list of events
-            fire_exec_events: bool controlling whether to fire logging events
-        returns:
-            dag: list of modules to run in sorted order
-        """
-
-        # Modules directory
-        try:
-            modules_dir = self.get_modules_dir(project_dir)
-        except prism.exceptions.CompileException as err:
-            e = prism.prism_logging.PrismExceptionErrorEvent(
-                err,
-                'accessing modules directory'
-            )
-            event_list = fire_console_event(e, event_list, 0, log_level='error')
-            event_list = self.fire_tail_event(event_list)
-            return prism.cli.base.TaskRunReturnResult(event_list)
-
-        # Get modules to compile
-        user_arg_module_em = BaseEventManager(
-            idx=None,
-            total=None,
-            name='grabbing user-specified modules',
-            full_tb=self.args.full_tb,
-            func=self.user_arg_modules
-        )
-        user_arg_module_em_output = user_arg_module_em.manage_events_during_run(
-            fire_exec_events=False,
-            event_list=event_list,
-            args=self.args,
-            modules_dir=modules_dir
+        event_list = fire_console_event(
+            prism.prism_logging.ServingDocsExitInfo(),
+            log_level='info'
         )
-        user_arg_modules = user_arg_module_em_output.outputs
-        event_to_fire = user_arg_module_em_output.event_to_fire
-        event_list = user_arg_module_em_output.event_list
-        if user_arg_modules == 0:
-            event_list = fire_console_event(
-                event_to_fire,
-                event_list,
-                log_level='error'
-            )
-            event_list = self.fire_tail_event(event_list)
-            return prism.cli.base.TaskRunReturnResult(event_list, True)
-
-        all_modules = self.get_modules(modules_dir)
-
-        # All downstream
-        all_downstream = args.all_downstream
+        event_list = fire_empty_line_event(event_list)
 
-        # Create compiled directory
-        compiled_dir = self.create_compiled_dir(project_dir)
+        # mypy doesn't think SimpleHTTPRequestHandler is ok here, but it is
+        httpd = TCPServer(  # type: ignore
+            (address, port), SimpleHTTPRequestHandler  # type: ignore
+        )  # type: ignore
+
+        if not self.args.no_browser:
+            try:
+                webbrowser.open_new_tab(f"http://127.0.0.1:{port}")
+            except webbrowser.Error:
+                pass
 
-        # Parse module references
-        compiler_manager = BaseEventManager(
-            idx=None,
-            total=None,
-            name='module DAG',
-            full_tb=args.full_tb,
-            func=self.compile_dag
-        )
-        compiled_event_manager_output = compiler_manager.manage_events_during_run(
-            event_list=event_list,
-            fire_exec_events=fire_exec_events,
-            project_dir=project_dir,
-            compiled_dir=compiled_dir,
-            all_modules=all_modules,
-            user_arg_modules=user_arg_modules,
-            user_arg_all_downstream=all_downstream,
-            project=project
-        )
-        compiled_dag = compiled_event_manager_output.outputs
-        if compiled_dag == 0:
-            return compiled_event_manager_output
+        try:
+            httpd.serve_forever()  # blocks
+        finally:
+            httpd.shutdown()
+            httpd.server_close()
 
-        return compiled_event_manager_output
+        return prism.cli.base.TaskRunReturnResult(event_list)
```

### Comparing `prism-ds-0.2.0rc1/prism/cli/connect.py` & `prism-ds-0.2.0rc2/prism/cli/connect.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/cli/create_agent.py` & `prism-ds-0.2.0rc2/prism/cli/create_agent.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/cli/create_task.py` & `prism-ds-0.2.0rc2/prism/cli/create_task.py`

 * *Files 15% similar despite different names*

```diff
@@ -67,36 +67,36 @@
             )
             event_list = fire_console_event(e, event_list, 0, log_level='error')
             event_list = self.fire_tail_event(event_list)
             return prism.cli.base.TaskRunReturnResult(event_list)
 
         # Grab the template
         if decorated:
-            template_module = importlib.import_module(
+            template_task = importlib.import_module(
                 name=f"prism.templates.tasks.{task_type}_dec"
             )
         else:
-            template_module = importlib.import_module(
+            template_task = importlib.import_module(
                 name=f"prism.templates.tasks.{task_type}_cls"
             )
-        template = template_module.TEMPLATE
+        template = template_task.TEMPLATE
         task_template = Environment(loader=BaseLoader).from_string(template)  # type: ignore # noqa: E501
 
         # Get the number of tasks to create and the task name
         task_number = self.args.number
         user_task_name = self.args.name
 
         # Get directory. If it's blank, then new tasks should be dumped into the
-        # `modules/` directory. Otherwise, add the inputted directory to the modules
+        # `tasks/` directory. Otherwise, add the inputted directory to the tasks
         # directory.
-        modules_dir = self.get_modules_dir(self.prism_project.project_dir)
+        tasks_dir = self.get_tasks_dir(self.prism_project.project_dir)
         if self.args.dir == "":
-            task_dir = modules_dir
+            task_dir = tasks_dir
         else:
-            task_dir = modules_dir / self.args.dir
+            task_dir = tasks_dir / self.args.dir
 
         # Fire events
         event_list = fire_console_event(
             prism.prism_logging.CreatingTasksEvent(),
             event_list,
             log_level='info'
         )
```

### Comparing `prism-ds-0.2.0rc1/prism/cli/create_trigger.py` & `prism-ds-0.2.0rc2/prism/cli/create_trigger.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/cli/init.py` & `prism-ds-0.2.0rc2/prism/cli/init.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/cli/run.py` & `prism-ds-0.2.0rc2/prism/cli/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         if isinstance(result, prism.cli.base.TaskRunReturnResult):
             return result
 
         compiled_dag = result.outputs
         compiled_dag_error_event = result.event_to_fire
         event_list = result.event_list
 
-        # If no modules in DAG, return
+        # If no tasks in DAG, return
         if compiled_dag == 0 and compiled_dag_error_event is not None:
             event_list = self.fire_error_events(
                 event_list,
                 compiled_dag_error_event,
                 trigger_manager
             )
             self.run_context = self.prism_project.cleanup(self.run_context)
@@ -190,16 +190,16 @@
             total=None,
             name='executing pipeline',
             full_tb=self.args.full_tb,
             func=pipeline.exec
         )
 
         # We don't fire the actual exec events for this manager, since executor class
-        # fired individual exec events for each module. This manager is simply for
-        # capturing any non-module related errors in the logger.
+        # fired individual exec events for each task. This manager is simply for
+        # capturing any non-task related errors in the logger.
         exec_event_manager_output = pipeline_exec_manager.manage_events_during_run(
             fire_exec_events=False,
             fire_empty_line_events=False,
             event_list=event_list,
             full_tb=self.args.full_tb
         )
         executor_output = exec_event_manager_output.outputs
```

### Comparing `prism-ds-0.2.0rc1/prism/cli/spark_submit.py` & `prism-ds-0.2.0rc2/prism/cli/spark_submit.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/client/__init__.py` & `prism-ds-0.2.0rc2/prism/client/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,30 +13,34 @@
 # Imports #
 ###########
 
 # Standard library imports
 import argparse
 import os
 from pathlib import Path
+import re
 from typing import Any, Dict, List, Optional
 
 # Prism-specific imports
 import prism.constants
 import prism.cli.base
 import prism.exceptions
+from prism.task import PrismTask
 from prism.infra import executor as prism_executor
-from prism.infra import module as prism_module
 from prism.infra import compiler as prism_compiler
+from prism.infra.compiler import CompiledDag
+from prism.infra.compiled_task import CompiledTask
 import prism.mixins.base
 import prism.mixins.compile
 import prism.mixins.connect
 import prism.mixins.run
 import prism.mixins.sys_handler
-from prism.parsers import ast_parser
 import prism.prism_logging
+import prism.cli.run
+from prism.triggers import TriggerManager
 
 
 ####################
 # Class definition #
 ####################
 
 class PrismDAG(
@@ -53,56 +57,71 @@
     def __init__(self,
         project_dir: Path,
         log_level: str = 'warn'
     ):
         self.project_dir = project_dir
         self.log_level = log_level
 
-        # Set the project to None.
+        # Set up default logger
+        self.args = argparse.Namespace()
+        self.args.log_level = self.log_level
+        prism.prism_logging.set_up_logger(self.args)
 
         # Check if project is valid
         self._is_valid_project(self.project_dir)
 
-        # Modules directory
-        self.modules_dir = self.get_modules_dir(self.project_dir)
+        # Tasks directory
+        self.tasks_dir = self.get_tasks_dir(self.project_dir)
 
-        # All modules in project
-        self.all_modules = self.get_modules(self.modules_dir)
+        # All tasks in project
+        self.all_modules = self.get_modules(self.tasks_dir)
+        self.all_tasks = self.parse_all_tasks(
+            all_modules=self.all_modules,
+            tasks_dir=self.tasks_dir
+        )
 
         # Define run context
         self.run_context = prism.constants.CONTEXT.copy()
 
-        # Set up default logger
-        args = argparse.Namespace()
-        args.log_level = self.log_level
-        prism.prism_logging.set_up_logger(args)
+        # Store outputs of tasks
+        self.task_outputs: Dict[str, Any] = {}
 
     def _is_valid_project(self, user_project_dir: Path) -> bool:
         """
         Determine if `user_project_dir` is a valid project (i.e., that is has a
-        `prism_project.py` file and a `modules` folder)
+        `prism_project.py` file and a `tasks` folder)
 
         args:
             user_project_dir: project path
         raises:
             exception if Prism project is not valid
         """
         os.chdir(user_project_dir)
         temp_project_dir = prism.cli.base.get_project_dir()
 
         # Inputted project directory is not the same as the computed project directory
         if temp_project_dir != user_project_dir:
             msg = f'no project at `{str(user_project_dir)}, closest project found at `{str(temp_project_dir)}`'   # noqa: E501
             raise prism.exceptions.InvalidProjectException(message=msg)
 
-        # Modules folder is not found
-        if not Path(user_project_dir / 'modules').is_dir():
-            raise prism.exceptions.InvalidProjectException(
-                message=f'`modules` directory not found in `{str(user_project_dir)}`'
-            )
+        # Tasks folder is not found
+        if not Path(user_project_dir / 'tasks').is_dir():
+
+            # If the `modules` directory is found, then raise a warning
+            if Path(user_project_dir / 'modules').is_dir():
+                prism.prism_logging.fire_console_event(
+                    prism.prism_logging.ModulesFolderDeprecated(),
+                    log_level='warn'
+                )
+
+            # Otherwise, raise an error
+            else:
+                raise prism.exceptions.InvalidProjectException(
+                    message=f'`tasks` directory not found in `{str(user_project_dir)}`'
+                )
 
         return True
 
     def connect(self,
         connection_type: str,
         user_context: Optional[Dict[str, Any]] = None
     ):
@@ -141,163 +160,258 @@
             self.create_connection(connection_type, profile_yml_path)  # type: ignore
         except Exception as e:
             raise e
         finally:
             self.run_context = prism_project.cleanup(self.run_context)
 
     def compile(self,
-        modules: Optional[List[str]] = None,
+        tasks: Optional[List[str]] = None,
         all_downstream: bool = True
     ) -> prism_compiler.CompiledDag:
         """
         Compile the Prism project
         """
-        if modules is None:
-            module_paths = self.all_modules
-        else:
-            module_paths = [Path(p) for p in modules]
-        self.user_arg_modules_list = module_paths
+        # Prism project
+        prism_project = self.create_project(
+            project_dir=self.project_dir,
+            user_context={},
+            which="compile",
+            filename="prism_project.py"
+        )
+        self.run_context = prism_project.run_context
+
+        # Construct list of all tasks
+        self.args.tasks = tasks
+        user_arg_tasks = self.user_arg_tasks(self.args, self.tasks_dir, self.all_tasks)
 
-        # Create compiled directory and compile the DAG
+        # Create compiled directory
         compiled_dir = self.create_compiled_dir(self.project_dir)
         self.compiled_dir = compiled_dir
-        return self.compile_dag(
-            self.project_dir,
-            self.compiled_dir,
-            self.all_modules,
-            self.user_arg_modules_list,
-            all_downstream
-        )
+
+        # Try to compile the DAG. If we encounter an error, then cleanup first and then
+        # raise the exception.
+        try:
+            compiled_dag = self.compile_dag(
+                project_dir=self.project_dir,
+                tasks_dir=self.tasks_dir,
+                compiled_dir=compiled_dir,
+                all_parsed_tasks=self.all_tasks,
+                user_arg_tasks=user_arg_tasks,
+                user_arg_all_downstream=all_downstream,
+                project=prism_project
+            )
+        except Exception as e:
+            raise e
+        finally:
+            self.run_context = prism_project.cleanup(self.run_context)
+
+        # Return
+        self.compiled_dag = compiled_dag
+        return compiled_dag
 
     def run(self,
-        modules: Optional[List[str]] = None,
+        tasks: Optional[List[str]] = None,
         all_upstream: bool = True,
         all_downstream: bool = False,
         full_tb: bool = True,
         user_context: Optional[Dict[str, Any]] = None
     ):
         """
         Run the Prism project
         """
-        # Create PrismProject
+        # Create Prism project
         if user_context is None:
             user_context = {}
         prism_project = self.create_project(
             project_dir=self.project_dir,
             user_context=user_context,
             which="run",
             filename="prism_project.py",
         )
+        self.run_context = prism_project.run_context
 
-        # Run sys.path engine
-        sys_path_engine = prism_project.sys_path_engine
-        self.run_context = sys_path_engine.modify_sys_path(
-            prism_project.sys_path_config
-        )
+        # Wrap everything in a try-except block. If any error occurs, cleanup the Prism
+        # project before re-running anything
+        try:
+            # Run sys.path engine
+            sys_path_engine = prism_project.sys_path_engine
+            self.run_context = sys_path_engine.modify_sys_path(
+                prism_project.sys_path_config
+            )
 
-        # Compile the DAG
-        compiled_dag = self.compile(modules, all_downstream)
+            # Prepare triggers
+            triggers_yml_path = prism_project.triggers_yml_path
+            trigger_manager = TriggerManager(
+                triggers_yml_path,
+                prism_project,
+            )
 
-        # Create DAG executor and Pipeline objects
-        threads = prism_project.thread_count
-        dag_executor = prism_executor.DagExecutor(
-            self.project_dir,
-            compiled_dag,
-            all_upstream,
-            all_downstream,
-            threads,
-            user_context
-        )
-        pipeline = self.create_pipeline(
-            prism_project, dag_executor, self.run_context
-        )
+            # Construct list of all tasks
+            self.args.tasks = tasks
+            user_arg_tasks = self.user_arg_tasks(
+                self.args,
+                self.tasks_dir,
+                self.all_tasks
+            )
 
-        # Create args and exec
-        output = pipeline.exec(full_tb)
+            # Create compiled directory
+            self.compiled_dir = self.create_compiled_dir(self.project_dir)
 
-        # Cleanup
-        self.run_context = prism_project.cleanup(
-            self.run_context
-        )
+            # Compile the DAG
+            self.compiled_dag = self.compile_dag(
+                project_dir=self.project_dir,
+                tasks_dir=self.tasks_dir,
+                compiled_dir=self.compiled_dir,
+                all_parsed_tasks=self.all_tasks,
+                user_arg_tasks=user_arg_tasks,
+                user_arg_all_downstream=all_downstream,
+                project=prism_project
+            )
 
-        # Write error
-        if output.error_event is not None:
-            event = output.error_event
-            try:
-                # Exception is a PrismException
-                exception = event.err
-            except AttributeError:
-                # All other exceptions
-                exception = event.value
-            raise exception
+            # Create DAG executor and Pipeline objects
+            threads = prism_project.thread_count
+            dag_executor = prism_executor.DagExecutor(
+                self.project_dir,
+                self.compiled_dag,
+                all_upstream,
+                all_downstream,
+                threads,
+                user_context
+            )
+            pipeline = self.create_pipeline(
+                prism_project, dag_executor, self.run_context
+            )
 
-    def _get_task_cls_from_namespace(self, module_path: Path):
-        """
-        Get PrismTask associated with `module_path` from Prism namespace
+            # Create args and exec
+            output = pipeline.exec(full_tb)
 
-        args:
-            module_path: path to module (relative to `modules/` folder)
-        returns:
-            task class
-        """
+            # Write error
+            if output.error_event is not None:
+                event = output.error_event
+                try:
+                    # Exception is a PrismException
+                    exception = event.err
+                except AttributeError:
+                    # All other exceptions
+                    exception = event.value
+
+                # Fire the `on_failure` events
+                trigger_manager.exec(
+                    'on_failure',
+                    full_tb,
+                    [],
+                    self.run_context,
+                )
+                raise exception
+
+            # Otherwise, fire the `on_success` events
+            trigger_manager.exec(
+                'on_success',
+                full_tb,
+                [],
+                self.run_context,
+            )
+
+            # Store the outputs of the various tasks
+            for task in user_arg_tasks:
+                task_instance = self.run_context[task]
+                if not isinstance(task_instance, PrismTask):
+                    raise prism.exceptions.RuntimeException(
+                        "task is not an instance of the `PrismTask` class"
+                    )
+                self.task_outputs[task] = task_instance.get_output()
 
-        # Name of variable containing the PrismTask for `module_path`
-        task_var_name = prism_module.get_task_var_name(module_path)
-        task_cls = self.run_context.get(task_var_name)
-
-        # If class is None, then raise an error. Otherwise, return the class
-        if task_cls is None:
-            msg_list = [
-                f'no output found for `{str(module_path)}` in the PrismProject namespace',                     # noqa: E501
-                f'check that `{str(module_path)}` has a PrismTask and that `{str(module_path)}` has been run'  # noqa: E501
-            ]
-            raise prism.exceptions.RuntimeException(message='\n'.join(msg_list))
-        return task_cls
+            # Cleanup
+            self.run_context = prism_project.cleanup(
+                self.run_context
+            )
+
+        # If we encounter any exception, then cleanup first and then raise
+        except Exception:
+            self.run_context = prism_project.cleanup(
+                self.run_context
+            )
+            raise
+
+    def clear_task_output(self):
+        self.task_outputs = {}
 
     def get_task_output(self,
-        module_path: Path,
+        task_name: str,
         bool_run: bool = False,
         **kwargs
     ) -> Any:
         """
-        Get output of the task in `module`. If bool_run==True, then run the project
+        Get output of the task in `task`. If bool_run==True, then run the project
         first. Note that if bool_run==False, then only tasks with a target can be
         parsed.
 
         args:
-            module: path to module (relative to `modules/` folder)
+            task_name: either `<module_name>` or `<module_name>.<task_name>`. Note that
+                if the user inputs the former, then the module should only have one
+                task.
             bool_run: boolean indicating whether to run pipeline first; default is False
             **kwargs: keyword arguments for running
         returns:
             task output
         """
-        # The user may have run the project in their script. Try retrieving the output
+        # Remove the `.py` from the ending of the task name, if it exists
+        task_name = re.sub(r'\.py$', '', task_name)
+
+        # Process the task name
+        tmp_module_name = task_name.split(".")[0]
+        tmp_task_name = None
         try:
-            task_cls = self._get_task_cls_from_namespace(module_path)
-            return task_cls.get_output()
+            tmp_task_name = task_name.split(".")[1]
+        except IndexError:
+            for _p in self.all_tasks:
+                if Path(f"{tmp_module_name}.py") == _p.task_relative_path:
+                    if len(_p.prism_task_names) == 0:
+                        raise prism.exceptions.ParserException(
+                            message=f"no PrismTask in `{str(_p.task_relative_path)}`"
+                        )
+                    if len(_p.prism_task_names) > 1:
+                        raise prism.exceptions.RuntimeException(
+                            message=f"module `{tmp_module_name}` has multiple tasks...specify the task name and try again"  # noqa: E501
+                        )
+                    tmp_task_name = _p.prism_task_names[0]
+
+        # If task name is still null, then something when wrong
+        if tmp_task_name is None:
+            raise prism.exceptions.RuntimeException(
+                message=f"could not find any task with module `{tmp_module_name}`"
+            )
+        processed_task_name = f"{tmp_module_name}.{tmp_task_name}"
 
-        except prism.exceptions.RuntimeException:
+        # The user may have run the project in their script. In that case, the PrismDAG
+        # instance will have a `compiled_dag` attribute that stores an instance of the
+        # `CompiledDag` class.
+        try:
+            return self.task_outputs[processed_task_name]
+
+        except KeyError:
             # If project is run, then any output can be retrieved from any task
             if bool_run:
                 self.run(**kwargs)
-                task_cls = self._get_task_cls_from_namespace(module_path)
-                return task_cls.get_output()
+                return self.task_outputs[processed_task_name]
 
             # If project is not run, then only targets can be retrieved
             else:
-                parsed_ast_module = ast_parser.AstParser(module_path, self.modules_dir)
-                prism_task_cls = parsed_ast_module.get_prism_task_node(
-                    parsed_ast_module.classes, parsed_ast_module.bases
-                )
-                if prism_task_cls is None:
-                    return None
-                prism_task_cls_name = prism_task_cls.name
+
+                # We need to compile the project
+                compiled_dag: CompiledDag = self.compile()
+
+                # Get the task associated with `processed_task_name`
+                compiled_task: CompiledTask
+                for _t in compiled_dag.compiled_tasks:
+                    if _t.task_var_name == processed_task_name:
+                        compiled_task = _t
 
                 # We need to update sys.path to include all paths in SYS_PATH_CONF,
-                # since some target locations may depend on vars stored in modules
+                # since some target locations may depend on vars stored in tasks
                 # imported from directories contained therein.
                 user_context = kwargs.get("user_context", {})
                 prism_project = self.create_project(
                     project_dir=self.project_dir,
                     user_context=user_context,
                     which="run",
                     filename="prism_project.py"
@@ -306,24 +420,28 @@
                 # Run sys.path engine
                 sys_path_engine = prism_project.sys_path_engine
                 self.run_context = sys_path_engine.modify_sys_path(
                     prism_project.sys_path_config
                 )
 
                 # Execute the class definition code
-                exec(parsed_ast_module.module_str, self.run_context)
-                task = self.run_context[prism_task_cls_name](False)  # type: ignore # noqa: E501
-
-                # No need for an actual task_manager/hooks, since we're only accessing
-                # the target
                 try:
-                    task.set_hooks(None)
-                    task.set_task_manager(None)
-                    task.exec()
-                    output = task.get_output()
+                    task_var_name = compiled_task.instantiate_task_class(
+                        run_context=self.run_context,
+                        task_manager=None,  # type: ignore
+                        hooks=None,  # type: ignore
+                        explicit_run=False
+                    )
+                    task_cls = self.run_context[task_var_name]
+                    if not isinstance(task_cls, PrismTask):
+                        raise prism.exceptions.RuntimeException(
+                            "task is not an instance of the `PrismTask` class"
+                        )
+                    task_cls.exec()
+                    output = task_cls.get_output()
 
                     # Cleanup
                     self.run_context = prism_project.cleanup(
                         self.run_context
                     )
                     return output
```

### Comparing `prism-ds-0.2.0rc1/prism/constants.py` & `prism-ds-0.2.0rc2/prism/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 #############
 # Constants #
 #############
 
 # Version number
-VERSION = '0.2.0rc1'
+VERSION = '0.2.0rc2'
 
 # Root directory of project
 ROOT_DIR = str(Path(os.path.dirname(__file__)).parent)
 
 # Files to ignore when instantiating Prism project
 IGNORE_FILES = ["__pycache__", '*checkpoint.ipynb', '.ipynb_checkpoints']
```

### Comparing `prism-ds-0.2.0rc1/prism/decorators/target.py` & `prism-ds-0.2.0rc2/prism/decorators/target.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/decorators/task.py` & `prism-ds-0.2.0rc2/prism/decorators/task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/docs/build/311ea03002abadcdcaba.png` & `prism-ds-0.2.0rc2/prism/docs/build/311ea03002abadcdcaba.png`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/docs/build/54968a39190c43d592b9.svg` & `prism-ds-0.2.0rc2/prism/docs/build/54968a39190c43d592b9.svg`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/docs/build/737ad70b3f2d3a9b5f6e.ico` & `prism-ds-0.2.0rc2/prism/docs/build/737ad70b3f2d3a9b5f6e.ico`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/docs/build/ce188596011a8fa32931.png` & `prism-ds-0.2.0rc2/prism/docs/build/ce188596011a8fa32931.png`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/docs/build/index.html` & `prism-ds-0.2.0rc2/prism/docs/build/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -34768,275 +34768,278 @@
 00087cf0: 3829 2c74 3d6e 2839 3134 3229 3b65 2e75  8),t=n(9142);e.u
 00087d00: 7365 2874 293b 636c 6173 7320 727b 636f  se(t);class r{co
 00087d10: 6e73 7472 7563 746f 7228 6529 7b74 6869  nstructor(e){thi
 00087d20: 732e 6461 7461 3d65 2c74 6869 732e 6b65  s.data=e,this.ke
 00087d30: 7973 3d4f 626a 6563 742e 6b65 7973 2865  ys=Object.keys(e
 00087d40: 293b 636f 6e73 7420 743d 5b22 7461 7267  );const t=["targ
 00087d50: 6574 7322 2c22 7072 6973 6d5f 7072 6f6a  ets","prism_proj
-00087d60: 6563 7422 2c22 6d6f 6475 6c65 7322 2c22  ect","modules","
-00087d70: 7265 6673 225d 3b63 6f6e 736f 6c65 2e61  refs"];console.a
-00087d80: 7373 6572 7428 4172 7261 792e 6973 4172  ssert(Array.isAr
-00087d90: 7261 7928 7468 6973 2e6b 6579 7329 2626  ray(this.keys)&&
-00087da0: 4172 7261 792e 6973 4172 7261 7928 7429  Array.isArray(t)
-00087db0: 2626 7468 6973 2e6b 6579 732e 6c65 6e67  &&this.keys.leng
-00087dc0: 7468 3d3d 3d74 2e6c 656e 6774 6826 2674  th===t.length&&t
-00087dd0: 6869 732e 6b65 7973 2e65 7665 7279 2828  his.keys.every((
-00087de0: 2865 2c6e 293d 3e65 3d3d 3d74 5b6e 5d29  (e,n)=>e===t[n])
-00087df0: 292c 224a 534f 4e20 646f 6573 206e 6f74  ),"JSON does not
-00087e00: 2061 6468 6572 6520 746f 2065 7870 6563   adhere to expec
-00087e10: 7465 6420 7374 7275 6374 7572 6522 292c  ted structure"),
-00087e20: 7468 6973 2e6d 6f64 756c 6573 3d74 6869  this.modules=thi
-00087e30: 732e 6461 7461 2e6d 6f64 756c 6573 2c74  s.data.modules,t
-00087e40: 6869 732e 7461 7267 6574 733d 7468 6973  his.targets=this
-00087e50: 2e64 6174 612e 7461 7267 6574 732c 7468  .data.targets,th
-00087e60: 6973 2e72 6566 733d 7468 6973 2e64 6174  is.refs=this.dat
-00087e70: 612e 7265 6673 7d70 6172 7365 4e6f 6465  a.refs}parseNode
-00087e80: 4461 7461 2829 7b76 6172 2065 3d6e 6577  Data(){var e=new
-00087e90: 204d 6170 2c74 3d6e 6577 204d 6170 3b66   Map,t=new Map;f
-00087ea0: 6f72 286c 6574 206e 3d30 3b6e 3c74 6869  or(let n=0;n<thi
-00087eb0: 732e 6d6f 6475 6c65 732e 6c65 6e67 7468  s.modules.length
-00087ec0: 3b6e 2b2b 2965 2e73 6574 2874 6869 732e  ;n++)e.set(this.
-00087ed0: 6d6f 6475 6c65 735b 6e5d 2c6e 2b31 292c  modules[n],n+1),
-00087ee0: 742e 7365 7428 6e2b 312c 7468 6973 2e6d  t.set(n+1,this.m
-00087ef0: 6f64 756c 6573 5b6e 5d29 3b72 6574 7572  odules[n]);retur
-00087f00: 6e7b 6e6f 6465 4944 733a 652c 6e6f 6465  n{nodeIDs:e,node
-00087f10: 4e61 6d65 733a 747d 7d67 6574 5f6e 6f64  Names:t}}get_nod
-00087f20: 6573 2865 297b 7661 7220 743d 5b5d 3b66  es(e){var t=[];f
-00087f30: 6f72 286c 6574 2072 3d30 3b72 3c74 6869  or(let r=0;r<thi
-00087f40: 732e 6d6f 6475 6c65 732e 6c65 6e67 7468  s.modules.length
-00087f50: 3b72 2b2b 297b 7661 7220 6e3d 7b64 6174  ;r++){var n={dat
-00087f60: 613a 7b69 643a 652e 6765 7428 7468 6973  a:{id:e.get(this
-00087f70: 2e6d 6f64 756c 6573 5b72 5d29 2c6c 6162  .modules[r]),lab
-00087f80: 656c 3a74 6869 732e 6d6f 6475 6c65 735b  el:this.modules[
-00087f90: 725d 2e72 6570 6c61 6365 2822 5f22 2c22  r].replace("_","
-00087fa0: 5fe2 808b 2229 2e72 6570 6c61 6365 2822  _...").replace("
-00087fb0: 2f22 2c22 e280 8b2f e280 8b22 297d 7d3b  /",".../...")}};
-00087fc0: 742e 7075 7368 286e 297d 7265 7475 726e  t.push(n)}return
-00087fd0: 2074 7d67 6574 5f65 6467 6573 2865 297b   t}get_edges(e){
-00087fe0: 7661 7220 743d 5b5d 3b66 6f72 286c 6574  var t=[];for(let
-00087ff0: 2061 3d30 3b61 3c74 6869 732e 7265 6673   a=0;a<this.refs
-00088000: 2e6c 656e 6774 683b 612b 2b29 7b76 6172  .length;a++){var
-00088010: 206e 3d74 6869 732e 7265 6673 5b61 5d2c   n=this.refs[a],
-00088020: 723d 652e 6765 7428 6e2e 736f 7572 6365  r=e.get(n.source
-00088030: 292c 693d 652e 6765 7428 6e2e 7461 7267  ),i=e.get(n.targ
-00088040: 6574 292c 6f3d 7b64 6174 613a 7b69 643a  et),o={data:{id:
-00088050: 7061 7273 6549 6e74 2860 247b 727d 247b  parseInt(`${r}${
-00088060: 697d 6029 2c73 6f75 7263 653a 722c 7461  i}`),source:r,ta
-00088070: 7267 6574 3a69 2c6d 696e 4c65 6e3a 312c  rget:i,minLen:1,
-00088080: 636f 6e74 726f 6c50 6f69 6e74 4469 7374  controlPointDist
-00088090: 616e 6365 733a 2230 2030 227d 7d3b 742e  ances:"0 0"}};t.
-000880a0: 7075 7368 286f 297d 7265 7475 726e 2074  push(o)}return t
-000880b0: 7d63 7265 6174 655f 6379 746f 7363 6170  }create_cytoscap
-000880c0: 655f 6772 6170 6828 297b 7661 7220 743d  e_graph(){var t=
-000880d0: 7468 6973 2e70 6172 7365 4e6f 6465 4461  this.parseNodeDa
-000880e0: 7461 2829 2e6e 6f64 6549 4473 2c6e 3d74  ta().nodeIDs,n=t
-000880f0: 6869 732e 6765 745f 6e6f 6465 7328 7429  his.get_nodes(t)
-00088100: 2c72 3d74 6869 732e 6765 745f 6564 6765  ,r=this.get_edge
-00088110: 7328 7429 2c69 3d65 287b 636f 6e74 6169  s(t),i=e({contai
-00088120: 6e65 723a 646f 6375 6d65 6e74 2e67 6574  ner:document.get
-00088130: 456c 656d 656e 7442 7949 6428 2263 7922  ElementById("cy"
-00088140: 292c 656c 656d 656e 7473 3a7b 6e6f 6465  ),elements:{node
-00088150: 733a 6e2c 6564 6765 733a 727d 2c6c 6179  s:n,edges:r},lay
-00088160: 6f75 743a 7b6e 616d 653a 2264 6167 7265  out:{name:"dagre
-00088170: 222c 7261 6e6b 5365 703a 3130 302c 6564  ",rankSep:100,ed
-00088180: 6765 5365 703a 3530 2c6e 6f64 6553 6570  geSep:50,nodeSep
-00088190: 3a33 302c 7261 6e6b 4469 723a 224c 5222  :30,rankDir:"LR"
-000881a0: 7d2c 7374 796c 653a 5b7b 7365 6c65 6374  },style:[{select
-000881b0: 6f72 3a22 6e6f 6465 222c 6373 733a 7b6c  or:"node",css:{l
-000881c0: 6162 656c 3a22 6461 7461 286c 6162 656c  abel:"data(label
-000881d0: 2922 2c77 6964 7468 3a31 3030 2c22 7465  )",width:100,"te
-000881e0: 7874 2d76 616c 6967 6e22 3a22 6365 6e74  xt-valign":"cent
-000881f0: 6572 222c 2274 6578 742d 6d61 782d 7769  er","text-max-wi
-00088200: 6474 6822 3a31 3030 2c22 7465 7874 2d77  dth":100,"text-w
-00088210: 7261 7022 3a22 656c 6c69 7073 6973 222c  rap":"ellipsis",
-00088220: 2262 6163 6b67 726f 756e 642d 6669 7422  "background-fit"
-00088230: 3a22 636f 6e74 6169 6e22 2c73 6861 7065  :"contain",shape
-00088240: 3a22 726f 756e 6472 6563 7461 6e67 6c65  :"roundrectangle
-00088250: 222c 2262 6163 6b67 726f 756e 642d 636f  ","background-co
-00088260: 6c6f 7222 3a22 2334 3738 4642 3622 2c6f  lor":"#478FB6",o
-00088270: 7061 6369 7479 3a22 3122 2c68 6569 6768  pacity:"1",heigh
-00088280: 743a 3235 2c22 626f 7264 6572 2d77 6964  t:25,"border-wid
-00088290: 7468 223a 2e37 352c 2270 6164 6469 6e67  th":.75,"padding
-000882a0: 2d72 6967 6874 223a 322c 2270 6164 6469  -right":2,"paddi
-000882b0: 6e67 2d6c 6566 7422 3a32 2c22 7061 6464  ng-left":2,"padd
-000882c0: 696e 672d 746f 7022 3a32 2c22 7061 6464  ing-top":2,"padd
-000882d0: 696e 672d 626f 7474 6f6d 223a 322c 2274  ing-bottom":2,"t
-000882e0: 6578 742d 6576 656e 7473 223a 2279 6573  ext-events":"yes
-000882f0: 222c 2266 6f6e 742d 7369 7a65 223a 2230  ","font-size":"0
-00088300: 2e35 3565 6d22 2c63 6f6c 6f72 3a22 7768  .55em",color:"wh
-00088310: 6974 6522 2c22 666f 6e74 2d66 616d 696c  ite","font-famil
-00088320: 7922 3a27 2246 6972 6120 5361 6e73 222c  y":'"Fira Sans",
-00088330: 2022 4865 6c76 6574 6963 6120 4e65 7565   "Helvetica Neue
-00088340: 222c 2048 656c 7665 7469 6361 4e65 7565  ", HelveticaNeue
-00088350: 2d4c 6967 6874 2c20 2250 726f 7869 6d61  -Light, "Proxima
-00088360: 204e 6f76 6122 2c20 2248 656c 7665 7469   Nova", "Helveti
-00088370: 6361 204e 6575 6522 2c20 4865 6c76 6574  ca Neue", Helvet
-00088380: 6963 612c 2041 7269 616c 2c20 224c 7563  ica, Arial, "Luc
-00088390: 6964 6120 4772 616e 6465 222c 2073 616e  ida Grande", san
-000883a0: 732d 7365 7269 6627 2c22 666f 6e74 2d77  s-serif',"font-w
-000883b0: 6569 6768 7422 3a22 3430 3022 7d7d 2c7b  eight":"400"}},{
-000883c0: 7365 6c65 6374 6f72 3a22 6564 6765 222c  selector:"edge",
-000883d0: 7374 796c 653a 7b77 6964 7468 3a31 2c22  style:{width:1,"
-000883e0: 6375 7276 652d 7374 796c 6522 3a22 756e  curve-style":"un
-000883f0: 6275 6e64 6c65 642d 6265 7a69 6572 222c  bundled-bezier",
-00088400: 2263 6f6e 7472 6f6c 2d70 6f69 6e74 2d77  "control-point-w
-00088410: 6569 6768 7473 223a 2230 2e33 2030 2e37  eights":"0.3 0.7
-00088420: 222c 2263 6f6e 7472 6f6c 2d70 6f69 6e74  ","control-point
-00088430: 2d64 6973 7461 6e63 6573 223a 2264 6174  -distances":"dat
-00088440: 6128 636f 6e74 726f 6c50 6f69 6e74 4469  a(controlPointDi
-00088450: 7374 616e 6365 7329 222c 226c 696e 652d  stances)","line-
-00088460: 636f 6c6f 7222 3a22 6772 6179 222c 226c  color":"gray","l
-00088470: 696e 652d 7374 796c 6522 3a22 736f 6c69  ine-style":"soli
-00088480: 6422 2c22 7461 7267 6574 2d61 7272 6f77  d","target-arrow
-00088490: 2d73 6861 7065 223a 2274 7269 616e 676c  -shape":"triangl
-000884a0: 6522 2c22 7461 7267 6574 2d61 7272 6f77  e","target-arrow
-000884b0: 2d63 6f6c 6f72 223a 2267 7261 7922 2c22  -color":"gray","
-000884c0: 6172 726f 772d 7363 616c 6522 3a22 302e  arrow-scale":"0.
-000884d0: 3735 222c 2274 6578 742d 726f 7461 7469  75","text-rotati
-000884e0: 6f6e 223a 2261 7574 6f72 6f74 6174 6522  on":"autorotate"
-000884f0: 2c6c 6162 656c 3a22 6461 7461 286c 6162  ,label:"data(lab
-00088500: 656c 2922 2c22 736f 7572 6365 2d65 6e64  el)","source-end
-00088510: 706f 696e 7422 3a22 3530 2520 3025 222c  point":"50% 0%",
-00088520: 2274 6172 6765 742d 656e 6470 6f69 6e74  "target-endpoint
-00088530: 223a 2232 3730 6465 6722 2c22 6564 6765  ":"270deg","edge
-00088540: 2d64 6973 7461 6e63 6573 223a 226e 6f64  -distances":"nod
-00088550: 652d 706f 7369 7469 6f6e 227d 7d2c 7b73  e-position"}},{s
-00088560: 656c 6563 746f 723a 222e 4261 6467 6522  elector:".Badge"
-00088570: 2c73 7479 6c65 3a7b 2262 6f72 6465 722d  ,style:{"border-
-00088580: 7769 6474 6822 3a31 7d7d 5d2c 6d69 6e5a  width":1}}],minZ
-00088590: 6f6f 6d3a 2e31 2c6d 6178 5a6f 6f6d 3a32  oom:.1,maxZoom:2
-000885a0: 2c7a 6f6f 6d69 6e67 456e 6162 6c65 643a  ,zoomingEnabled:
-000885b0: 2130 2c75 7365 725a 6f6f 6d69 6e67 456e  !0,userZoomingEn
-000885c0: 6162 6c65 643a 2130 2c61 7574 6f75 6e67  abled:!0,autoung
-000885d0: 7261 6269 6679 3a21 312c 6175 746f 756e  rabify:!1,autoun
-000885e0: 7365 6c65 6374 6966 793a 2130 7d29 3b72  selectify:!0});r
-000885f0: 6574 7572 6e20 692e 6564 6765 7328 292e  eturn i.edges().
-00088600: 666f 7245 6163 6828 2865 3d3e 6675 6e63  forEach((e=>func
-00088610: 7469 6f6e 2865 297b 636f 6e73 7420 743d  tion(e){const t=
-00088620: 2d2e 322a 2865 2e73 6f75 7263 6528 292e  -.2*(e.source().
-00088630: 7265 6e64 6572 6564 506f 7369 7469 6f6e  renderedPosition
-00088640: 2822 7922 292d 652e 7461 7267 6574 2829  ("y")-e.target()
-00088650: 2e72 656e 6465 7265 6450 6f73 6974 696f  .renderedPositio
-00088660: 6e28 2279 2229 292c 6e3d 5b2d 312a 742c  n("y")),n=[-1*t,
-00088670: 745d 3b65 2e64 6174 6128 2263 6f6e 7472  t];e.data("contr
-00088680: 6f6c 506f 696e 7444 6973 7461 6e63 6573  olPointDistances
-00088690: 222c 6e2e 6a6f 696e 2822 2022 2929 7d28  ",n.join(" "))}(
-000886a0: 6529 2929 2c69 7d7d 7661 7220 693d 6e28  e))),i}}var i=n(
-000886b0: 3333 3739 292c 6f3d 6e2e 6e28 6929 2c61  3379),o=n.n(i),a
-000886c0: 3d6e 2837 3739 3529 2c73 3d6e 2e6e 2861  =n(7795),s=n.n(a
-000886d0: 292c 753d 6e28 3536 3929 2c6c 3d6e 2e6e  ),u=n(569),l=n.n
-000886e0: 2875 292c 633d 6e28 3335 3635 292c 643d  (u),c=n(3565),d=
-000886f0: 6e2e 6e28 6329 2c68 3d6e 2839 3231 3629  n.n(c),h=n(9216)
-00088700: 2c66 3d6e 2e6e 2868 292c 703d 6e28 3435  ,f=n.n(h),p=n(45
-00088710: 3839 292c 763d 6e2e 6e28 7029 2c67 3d6e  89),v=n.n(p),g=n
-00088720: 2837 3231 292c 793d 7b7d 3b79 2e73 7479  (721),y={};y.sty
-00088730: 6c65 5461 6754 7261 6e73 666f 726d 3d76  leTagTransform=v
-00088740: 2829 2c79 2e73 6574 4174 7472 6962 7574  (),y.setAttribut
-00088750: 6573 3d64 2829 2c79 2e69 6e73 6572 743d  es=d(),y.insert=
-00088760: 6c28 292e 6269 6e64 286e 756c 6c2c 2268  l().bind(null,"h
-00088770: 6561 6422 292c 792e 646f 6d41 5049 3d73  ead"),y.domAPI=s
-00088780: 2829 2c79 2e69 6e73 6572 7453 7479 6c65  (),y.insertStyle
-00088790: 456c 656d 656e 743d 6628 292c 6f28 2928  Element=f(),o()(
-000887a0: 672e 5a2c 7929 2c67 2e5a 2626 672e 5a2e  g.Z,y),g.Z&&g.Z.
-000887b0: 6c6f 6361 6c73 2626 672e 5a2e 6c6f 6361  locals&&g.Z.loca
-000887c0: 6c73 2c6e 2839 3735 3529 3b6c 6574 206d  ls,n(9755);let m
-000887d0: 3d6e 2839 3035 3829 2c62 3d6e 2834 3734  =n(9058),b=n(474
-000887e0: 293b 7661 7220 783d 6e65 7720 4172 7261  );var x=new Arra
-000887f0: 793b 6675 6e63 7469 6f6e 2077 2865 297b  y;function w(e){
-00088800: 666f 7228 636f 6e73 745b 742c 6e5d 6f66  for(const[t,n]of
-00088810: 2065 2e6e 6f64 6573 2829 2e65 6e74 7269   e.nodes().entri
-00088820: 6573 2829 2978 2e70 7573 6828 6e2e 6964  es())x.push(n.id
-00088830: 2829 293b 652e 6e6f 6465 7328 292e 7374  ());e.nodes().st
-00088840: 796c 6528 7b22 6261 636b 6772 6f75 6e64  yle({"background
-00088850: 2d63 6f6c 6f72 223a 2270 7572 706c 6522  -color":"purple"
-00088860: 7d29 2c65 2e65 6467 6573 2829 2e73 7479  }),e.edges().sty
-00088870: 6c65 287b 226c 696e 652d 636f 6c6f 7222  le({"line-color"
-00088880: 3a22 7075 7270 6c65 227d 292c 652e 6564  :"purple"}),e.ed
-00088890: 6765 7328 292e 7374 796c 6528 7b22 7461  ges().style({"ta
-000888a0: 7267 6574 2d61 7272 6f77 2d63 6f6c 6f72  rget-arrow-color
-000888b0: 223a 2270 7572 706c 6522 7d29 7d66 756e  ":"purple"})}fun
-000888c0: 6374 696f 6e20 4528 6529 7b66 6f72 2863  ction E(e){for(c
-000888d0: 6f6e 7374 5b74 2c6e 5d6f 6620 652e 6e6f  onst[t,n]of e.no
-000888e0: 6465 7328 292e 656e 7472 6965 7328 2929  des().entries())
-000888f0: 7b63 6f6e 7374 2065 3d78 2e69 6e64 6578  {const e=x.index
-00088900: 4f66 286e 2e69 6428 2929 3b78 2e73 706c  Of(n.id());x.spl
-00088910: 6963 6528 652c 3129 7d65 2e6e 6f64 6573  ice(e,1)}e.nodes
-00088920: 2829 2e73 7479 6c65 287b 2262 6163 6b67  ().style({"backg
-00088930: 726f 756e 642d 636f 6c6f 7222 3a22 2334  round-color":"#4
-00088940: 3738 4642 3622 7d29 2c65 2e65 6467 6573  78FB6"}),e.edges
-00088950: 2829 2e73 7479 6c65 287b 226c 696e 652d  ().style({"line-
-00088960: 636f 6c6f 7222 3a22 6772 6179 227d 292c  color":"gray"}),
-00088970: 652e 6564 6765 7328 292e 7374 796c 6528  e.edges().style(
-00088980: 7b22 7461 7267 6574 2d61 7272 6f77 2d63  {"target-arrow-c
-00088990: 6f6c 6f72 223a 2267 7261 7922 7d29 7d62  olor":"gray"})}b
-000889a0: 286d 293b 7661 7220 6b2c 433d 6e28 3931  (m);var k,C=n(91
-000889b0: 3338 292c 533d 7b7d 3b53 2e73 7479 6c65  38),S={};S.style
-000889c0: 5461 6754 7261 6e73 666f 726d 3d76 2829  TagTransform=v()
-000889d0: 2c53 2e73 6574 4174 7472 6962 7574 6573  ,S.setAttributes
-000889e0: 3d64 2829 2c53 2e69 6e73 6572 743d 6c28  =d(),S.insert=l(
-000889f0: 292e 6269 6e64 286e 756c 6c2c 2268 6561  ).bind(null,"hea
-00088a00: 6422 292c 532e 646f 6d41 5049 3d73 2829  d"),S.domAPI=s()
-00088a10: 2c53 2e69 6e73 6572 7453 7479 6c65 456c  ,S.insertStyleEl
-00088a20: 656d 656e 743d 6628 292c 6f28 2928 432e  ement=f(),o()(C.
-00088a30: 5a2c 5329 2c43 2e5a 2626 432e 5a2e 6c6f  Z,S),C.Z&&C.Z.lo
-00088a40: 6361 6c73 2626 432e 5a2e 6c6f 6361 6c73  cals&&C.Z.locals
-00088a50: 2c66 6574 6368 2822 6d61 6e69 6665 7374  ,fetch("manifest
-00088a60: 2e6a 736f 6e22 292e 7468 656e 2828 653d  .json").then((e=
-00088a70: 3e65 2e6a 736f 6e28 2929 292e 7468 656e  >e.json())).then
-00088a80: 2828 653d 3e6b 3d65 2929 2e74 6865 6e28  ((e=>k=e)).then(
-00088a90: 2828 293d 3e66 756e 6374 696f 6e28 6529  (()=>function(e)
-00088aa0: 7b76 6172 2074 3d6e 6577 2072 2865 292e  {var t=new r(e).
-00088ab0: 6372 6561 7465 5f63 7974 6f73 6361 7065  create_cytoscape
-00088ac0: 5f67 7261 7068 2829 2c6e 3d7b 6576 7454  _graph(),n={evtT
-00088ad0: 7970 653a 2263 7874 7461 7022 2c6d 656e  ype:"cxttap",men
-00088ae0: 7549 7465 6d73 3a5b 7b69 643a 2265 7870  uItems:[{id:"exp
-00088af0: 6f72 7450 4e47 222c 636f 6e74 656e 743a  ortPNG",content:
-00088b00: 2245 7870 6f72 7420 504e 4722 2c74 6f6f  "Export PNG",too
-00088b10: 6c74 6970 5465 7874 3a22 4578 706f 7274  ltipText:"Export
-00088b20: 2074 6865 2044 4147 2061 7320 6120 504e   the DAG as a PN
-00088b30: 4722 2c73 656c 6563 746f 723a 226e 6f64  G",selector:"nod
-00088b40: 6522 2c63 6f72 6541 7357 656c 6c3a 2130  e",coreAsWell:!0
-00088b50: 2c6f 6e43 6c69 636b 4675 6e63 7469 6f6e  ,onClickFunction
-00088b60: 3a66 756e 6374 696f 6e28 6529 7b76 6172  :function(e){var
-00088b70: 206e 3d74 2e70 6e67 287b 6267 3a22 7267   n=t.png({bg:"rg
-00088b80: 6228 3233 352c 3233 352c 3233 3529 227d  b(235,235,235)"}
-00088b90: 292c 723d 646f 6375 6d65 6e74 2e63 7265  ),r=document.cre
-00088ba0: 6174 6545 6c65 6d65 6e74 2822 6122 293b  ateElement("a");
-00088bb0: 722e 646f 776e 6c6f 6164 3d22 7072 6973  r.download="pris
-00088bc0: 6d2d 6461 672e 706e 6722 2c72 2e68 7265  m-dag.png",r.hre
-00088bd0: 663d 6e2c 722e 636c 6963 6b28 297d 7d5d  f=n,r.click()}}]
-00088be0: 2c6d 656e 7549 7465 6d43 6c61 7373 6573  ,menuItemClasses
-00088bf0: 3a5b 2263 792d 636f 6e74 6578 742d 6d65  :["cy-context-me
-00088c00: 6e75 732d 6378 742d 6d65 6e75 6974 656d  nus-cxt-menuitem
-00088c10: 222c 2263 792d 636f 6e74 6578 742d 6d65  ","cy-context-me
-00088c20: 6e75 732d 6469 7669 6465 7222 5d2c 636f  nus-divider"],co
-00088c30: 6e74 6578 744d 656e 7543 6c61 7373 6573  ntextMenuClasses
-00088c40: 3a5b 2263 792d 636f 6e74 6578 742d 6d65  :["cy-context-me
-00088c50: 6e75 732d 6378 742d 6d65 6e75 225d 7d3b  nus-cxt-menu"]};
-00088c60: 742e 636f 6e74 6578 744d 656e 7573 286e  t.contextMenus(n
-00088c70: 293b 7661 7220 693d 2d31 3b74 2e6f 6e28  );var i=-1;t.on(
-00088c80: 2263 6c69 636b 222c 226e 6f64 6522 2c28  "click","node",(
-00088c90: 6675 6e63 7469 6f6e 2865 297b 6c65 7420  function(e){let 
-00088ca0: 6e3d 652e 7461 7267 6574 2e69 6428 293b  n=e.target.id();
-00088cb0: 7661 7220 723d 742e 2428 2223 222b 6e29  var r=t.$("#"+n)
-00088cc0: 2c6f 3d72 2e70 7265 6465 6365 7373 6f72  ,o=r.predecessor
-00088cd0: 7328 292c 613d 722e 7375 6363 6573 736f  s(),a=r.successo
-00088ce0: 7273 2829 3b69 6628 693d 3d6e 2945 2872  rs();if(i==n)E(r
-00088cf0: 292c 4528 6f29 2c45 2861 292c 693d 2d31  ),E(o),E(a),i=-1
-00088d00: 3b65 6c73 657b 6966 282d 3121 3d69 297b  ;else{if(-1!=i){
-00088d10: 7661 7220 733d 742e 2428 2223 222b 6929  var s=t.$("#"+i)
-00088d20: 2c75 3d73 2e70 7265 6465 6365 7373 6f72  ,u=s.predecessor
-00088d30: 7328 292c 6c3d 732e 7375 6363 6573 736f  s(),l=s.successo
-00088d40: 7273 2829 3b45 2873 292c 4528 7529 2c45  rs();E(s),E(u),E
-00088d50: 286c 297d 7728 7229 2c77 286f 292c 7728  (l)}w(r),w(o),w(
-00088d60: 6129 2c69 3d6e 7d7d 2929 7d28 6b29 2929  a),i=n}}))}(k)))
-00088d70: 2e63 6174 6368 2828 6675 6e63 7469 6f6e  .catch((function
-00088d80: 2865 297b 636f 6e73 6f6c 652e 6c6f 6728  (e){console.log(
-00088d90: 6529 2c77 696e 646f 772e 616c 6572 7428  e),window.alert(
-00088da0: 226d 616e 6966 6573 742e 6a73 6f6e 206e  "manifest.json n
-00088db0: 6f74 2066 6f75 6e64 2069 6e20 636f 6d70  ot found in comp
-00088dc0: 696c 6564 2064 6972 6563 746f 7279 5c6e  iled directory\n
-00088dd0: 7265 2d63 6f6d 7069 6c65 2074 6865 2070  re-compile the p
-00088de0: 726f 6a65 6374 2061 6e64 2074 7279 2061  roject and try a
-00088df0: 6761 696e 2229 7d29 297d 2928 297d 2928  gain")}))})()})(
-00088e00: 293b 3c2f 7363 7269 7074 3e3c 2f62 6f64  );</script></bod
-00088e10: 793e 3c2f 6874 6d6c 3e                   y></html>
+00087d60: 6563 7422 2c22 7461 736b 7322 2c22 7265  ect","tasks","re
+00087d70: 6673 225d 3b63 6f6e 736f 6c65 2e61 7373  fs"];console.ass
+00087d80: 6572 7428 4172 7261 792e 6973 4172 7261  ert(Array.isArra
+00087d90: 7928 7468 6973 2e6b 6579 7329 2626 4172  y(this.keys)&&Ar
+00087da0: 7261 792e 6973 4172 7261 7928 7429 2626  ray.isArray(t)&&
+00087db0: 7468 6973 2e6b 6579 732e 6c65 6e67 7468  this.keys.length
+00087dc0: 3d3d 3d74 2e6c 656e 6774 6826 2674 6869  ===t.length&&thi
+00087dd0: 732e 6b65 7973 2e65 7665 7279 2828 2865  s.keys.every(((e
+00087de0: 2c6e 293d 3e65 3d3d 3d74 5b6e 5d29 292c  ,n)=>e===t[n])),
+00087df0: 224a 534f 4e20 646f 6573 206e 6f74 2061  "JSON does not a
+00087e00: 6468 6572 6520 746f 2065 7870 6563 7465  dhere to expecte
+00087e10: 6420 7374 7275 6374 7572 6522 292c 7468  d structure"),th
+00087e20: 6973 2e74 6173 6b73 3d74 6869 732e 6461  is.tasks=this.da
+00087e30: 7461 2e74 6173 6b73 2c74 6869 732e 7461  ta.tasks,this.ta
+00087e40: 7267 6574 733d 7468 6973 2e64 6174 612e  rgets=this.data.
+00087e50: 7461 7267 6574 732c 7468 6973 2e72 6566  targets,this.ref
+00087e60: 733d 7468 6973 2e64 6174 612e 7265 6673  s=this.data.refs
+00087e70: 7d70 6172 7365 4e6f 6465 4461 7461 2829  }parseNodeData()
+00087e80: 7b76 6172 2065 3d6e 6577 204d 6170 2c74  {var e=new Map,t
+00087e90: 3d6e 6577 204d 6170 3b66 6f72 286c 6574  =new Map;for(let
+00087ea0: 206e 3d30 3b6e 3c74 6869 732e 7461 736b   n=0;n<this.task
+00087eb0: 732e 6c65 6e67 7468 3b6e 2b2b 2965 2e73  s.length;n++)e.s
+00087ec0: 6574 2874 6869 732e 7461 736b 735b 6e5d  et(this.tasks[n]
+00087ed0: 2c6e 2b31 292c 742e 7365 7428 6e2b 312c  ,n+1),t.set(n+1,
+00087ee0: 7468 6973 2e74 6173 6b73 5b6e 5d29 3b72  this.tasks[n]);r
+00087ef0: 6574 7572 6e7b 6e6f 6465 4944 733a 652c  eturn{nodeIDs:e,
+00087f00: 6e6f 6465 4e61 6d65 733a 747d 7d67 6574  nodeNames:t}}get
+00087f10: 5f6e 6f64 6573 2865 297b 7661 7220 743d  _nodes(e){var t=
+00087f20: 5b5d 3b66 6f72 286c 6574 2072 3d30 3b72  [];for(let r=0;r
+00087f30: 3c74 6869 732e 7461 736b 732e 6c65 6e67  <this.tasks.leng
+00087f40: 7468 3b72 2b2b 297b 7661 7220 6e3d 7b64  th;r++){var n={d
+00087f50: 6174 613a 7b69 643a 652e 6765 7428 7468  ata:{id:e.get(th
+00087f60: 6973 2e74 6173 6b73 5b72 5d29 2c6c 6162  is.tasks[r]),lab
+00087f70: 656c 3a74 6869 732e 7461 736b 735b 725d  el:this.tasks[r]
+00087f80: 2e72 6570 6c61 6365 2822 5f22 2c22 5fe2  .replace("_","_.
+00087f90: 808b 2229 2e72 6570 6c61 6365 2822 2f22  ..").replace("/"
+00087fa0: 2c22 e280 8b2f e280 8b22 297d 7d3b 742e  ,".../...")}};t.
+00087fb0: 7075 7368 286e 297d 7265 7475 726e 2074  push(n)}return t
+00087fc0: 7d67 6574 5f65 6467 6573 2865 297b 7661  }get_edges(e){va
+00087fd0: 7220 743d 5b5d 3b66 6f72 2876 6172 206e  r t=[];for(var n
+00087fe0: 206f 6620 4f62 6a65 6374 2e6b 6579 7328   of Object.keys(
+00087ff0: 7468 6973 2e72 6566 7329 297b 7661 7220  this.refs)){var 
+00088000: 723d 7468 6973 2e72 6566 735b 6e5d 3b66  r=this.refs[n];f
+00088010: 6f72 2876 6172 2069 206f 6620 4f62 6a65  or(var i of Obje
+00088020: 6374 2e6b 6579 7328 7229 297b 7661 7220  ct.keys(r)){var 
+00088030: 6f3d 6024 7b6e 7d2e 247b 697d 602c 613d  o=`${n}.${i}`,a=
+00088040: 652e 6765 7428 6f29 3b66 6f72 286c 6574  e.get(o);for(let
+00088050: 206e 3d30 3b6e 3c72 5b69 5d2e 6c65 6e67   n=0;n<r[i].leng
+00088060: 7468 3b6e 2b2b 297b 7661 7220 733d 725b  th;n++){var s=r[
+00088070: 695d 5b6e 5d2c 753d 652e 6765 7428 7329  i][n],u=e.get(s)
+00088080: 2c6c 3d7b 6461 7461 3a7b 6964 3a70 6172  ,l={data:{id:par
+00088090: 7365 496e 7428 6024 7b75 7d24 7b61 7d60  seInt(`${u}${a}`
+000880a0: 292c 736f 7572 6365 3a75 2c74 6172 6765  ),source:u,targe
+000880b0: 743a 612c 6d69 6e4c 656e 3a31 2c63 6f6e  t:a,minLen:1,con
+000880c0: 7472 6f6c 506f 696e 7444 6973 7461 6e63  trolPointDistanc
+000880d0: 6573 3a22 3020 3022 7d7d 3b74 2e70 7573  es:"0 0"}};t.pus
+000880e0: 6828 6c29 7d7d 7d72 6574 7572 6e20 747d  h(l)}}}return t}
+000880f0: 6372 6561 7465 5f63 7974 6f73 6361 7065  create_cytoscape
+00088100: 5f67 7261 7068 2829 7b76 6172 2074 3d74  _graph(){var t=t
+00088110: 6869 732e 7061 7273 654e 6f64 6544 6174  his.parseNodeDat
+00088120: 6128 292e 6e6f 6465 4944 732c 6e3d 7468  a().nodeIDs,n=th
+00088130: 6973 2e67 6574 5f6e 6f64 6573 2874 292c  is.get_nodes(t),
+00088140: 723d 7468 6973 2e67 6574 5f65 6467 6573  r=this.get_edges
+00088150: 2874 292c 693d 6528 7b63 6f6e 7461 696e  (t),i=e({contain
+00088160: 6572 3a64 6f63 756d 656e 742e 6765 7445  er:document.getE
+00088170: 6c65 6d65 6e74 4279 4964 2822 6379 2229  lementById("cy")
+00088180: 2c65 6c65 6d65 6e74 733a 7b6e 6f64 6573  ,elements:{nodes
+00088190: 3a6e 2c65 6467 6573 3a72 7d2c 6c61 796f  :n,edges:r},layo
+000881a0: 7574 3a7b 6e61 6d65 3a22 6461 6772 6522  ut:{name:"dagre"
+000881b0: 2c72 616e 6b53 6570 3a31 3030 2c65 6467  ,rankSep:100,edg
+000881c0: 6553 6570 3a35 302c 6e6f 6465 5365 703a  eSep:50,nodeSep:
+000881d0: 3330 2c72 616e 6b44 6972 3a22 4c52 227d  30,rankDir:"LR"}
+000881e0: 2c73 7479 6c65 3a5b 7b73 656c 6563 746f  ,style:[{selecto
+000881f0: 723a 226e 6f64 6522 2c63 7373 3a7b 6c61  r:"node",css:{la
+00088200: 6265 6c3a 2264 6174 6128 6c61 6265 6c29  bel:"data(label)
+00088210: 222c 7769 6474 683a 3130 302c 2274 6578  ",width:100,"tex
+00088220: 742d 7661 6c69 676e 223a 2263 656e 7465  t-valign":"cente
+00088230: 7222 2c22 7465 7874 2d6d 6178 2d77 6964  r","text-max-wid
+00088240: 7468 223a 3130 302c 2274 6578 742d 7772  th":100,"text-wr
+00088250: 6170 223a 2265 6c6c 6970 7369 7322 2c22  ap":"ellipsis","
+00088260: 6261 636b 6772 6f75 6e64 2d66 6974 223a  background-fit":
+00088270: 2263 6f6e 7461 696e 222c 7368 6170 653a  "contain",shape:
+00088280: 2272 6f75 6e64 7265 6374 616e 676c 6522  "roundrectangle"
+00088290: 2c22 6261 636b 6772 6f75 6e64 2d63 6f6c  ,"background-col
+000882a0: 6f72 223a 2223 4345 4344 4636 222c 6f70  or":"#CECDF6",op
+000882b0: 6163 6974 793a 2231 222c 6865 6967 6874  acity:"1",height
+000882c0: 3a32 352c 2262 6f72 6465 722d 7769 6474  :25,"border-widt
+000882d0: 6822 3a2e 352c 2270 6164 6469 6e67 2d72  h":.5,"padding-r
+000882e0: 6967 6874 223a 322c 2270 6164 6469 6e67  ight":2,"padding
+000882f0: 2d6c 6566 7422 3a32 2c22 7061 6464 696e  -left":2,"paddin
+00088300: 672d 746f 7022 3a32 2c22 7061 6464 696e  g-top":2,"paddin
+00088310: 672d 626f 7474 6f6d 223a 322c 2274 6578  g-bottom":2,"tex
+00088320: 742d 6576 656e 7473 223a 2279 6573 222c  t-events":"yes",
+00088330: 2266 6f6e 742d 7369 7a65 223a 2230 2e35  "font-size":"0.5
+00088340: 656d 222c 636f 6c6f 723a 2262 6c61 636b  em",color:"black
+00088350: 222c 2266 6f6e 742d 6661 6d69 6c79 223a  ","font-family":
+00088360: 2722 4865 6c76 6574 6963 6120 4e65 7565  '"Helvetica Neue
+00088370: 222c 2048 656c 7665 7469 6361 4e65 7565  ", HelveticaNeue
+00088380: 2d4c 6967 6874 2c20 2250 726f 7869 6d61  -Light, "Proxima
+00088390: 204e 6f76 6122 2c20 2248 656c 7665 7469   Nova", "Helveti
+000883a0: 6361 204e 6575 6522 2c20 4865 6c76 6574  ca Neue", Helvet
+000883b0: 6963 612c 2041 7269 616c 2c20 224c 7563  ica, Arial, "Luc
+000883c0: 6964 6120 4772 616e 6465 222c 2073 616e  ida Grande", san
+000883d0: 732d 7365 7269 6627 2c22 666f 6e74 2d77  s-serif',"font-w
+000883e0: 6569 6768 7422 3a22 3430 3022 7d7d 2c7b  eight":"400"}},{
+000883f0: 7365 6c65 6374 6f72 3a22 6564 6765 222c  selector:"edge",
+00088400: 7374 796c 653a 7b77 6964 7468 3a31 2c22  style:{width:1,"
+00088410: 6375 7276 652d 7374 796c 6522 3a22 756e  curve-style":"un
+00088420: 6275 6e64 6c65 642d 6265 7a69 6572 222c  bundled-bezier",
+00088430: 2263 6f6e 7472 6f6c 2d70 6f69 6e74 2d77  "control-point-w
+00088440: 6569 6768 7473 223a 2230 2e33 2030 2e37  eights":"0.3 0.7
+00088450: 222c 2263 6f6e 7472 6f6c 2d70 6f69 6e74  ","control-point
+00088460: 2d64 6973 7461 6e63 6573 223a 2264 6174  -distances":"dat
+00088470: 6128 636f 6e74 726f 6c50 6f69 6e74 4469  a(controlPointDi
+00088480: 7374 616e 6365 7329 222c 226c 696e 652d  stances)","line-
+00088490: 636f 6c6f 7222 3a22 6772 6179 222c 226c  color":"gray","l
+000884a0: 696e 652d 7374 796c 6522 3a22 736f 6c69  ine-style":"soli
+000884b0: 6422 2c22 7461 7267 6574 2d61 7272 6f77  d","target-arrow
+000884c0: 2d73 6861 7065 223a 2274 7269 616e 676c  -shape":"triangl
+000884d0: 6522 2c22 7461 7267 6574 2d61 7272 6f77  e","target-arrow
+000884e0: 2d63 6f6c 6f72 223a 2267 7261 7922 2c22  -color":"gray","
+000884f0: 6172 726f 772d 7363 616c 6522 3a22 302e  arrow-scale":"0.
+00088500: 3735 222c 2274 6578 742d 726f 7461 7469  75","text-rotati
+00088510: 6f6e 223a 2261 7574 6f72 6f74 6174 6522  on":"autorotate"
+00088520: 2c6c 6162 656c 3a22 6461 7461 286c 6162  ,label:"data(lab
+00088530: 656c 2922 2c22 736f 7572 6365 2d65 6e64  el)","source-end
+00088540: 706f 696e 7422 3a22 3530 2520 3025 222c  point":"50% 0%",
+00088550: 2274 6172 6765 742d 656e 6470 6f69 6e74  "target-endpoint
+00088560: 223a 2232 3730 6465 6722 2c22 6564 6765  ":"270deg","edge
+00088570: 2d64 6973 7461 6e63 6573 223a 226e 6f64  -distances":"nod
+00088580: 652d 706f 7369 7469 6f6e 227d 7d2c 7b73  e-position"}},{s
+00088590: 656c 6563 746f 723a 222e 4261 6467 6522  elector:".Badge"
+000885a0: 2c73 7479 6c65 3a7b 2262 6f72 6465 722d  ,style:{"border-
+000885b0: 7769 6474 6822 3a31 7d7d 5d2c 6d69 6e5a  width":1}}],minZ
+000885c0: 6f6f 6d3a 2e31 2c6d 6178 5a6f 6f6d 3a32  oom:.1,maxZoom:2
+000885d0: 2c7a 6f6f 6d69 6e67 456e 6162 6c65 643a  ,zoomingEnabled:
+000885e0: 2130 2c75 7365 725a 6f6f 6d69 6e67 456e  !0,userZoomingEn
+000885f0: 6162 6c65 643a 2130 2c61 7574 6f75 6e67  abled:!0,autoung
+00088600: 7261 6269 6679 3a21 312c 6175 746f 756e  rabify:!1,autoun
+00088610: 7365 6c65 6374 6966 793a 2130 7d29 3b72  selectify:!0});r
+00088620: 6574 7572 6e20 692e 6564 6765 7328 292e  eturn i.edges().
+00088630: 666f 7245 6163 6828 2865 3d3e 6675 6e63  forEach((e=>func
+00088640: 7469 6f6e 2865 297b 636f 6e73 7420 743d  tion(e){const t=
+00088650: 2d2e 322a 2865 2e73 6f75 7263 6528 292e  -.2*(e.source().
+00088660: 7265 6e64 6572 6564 506f 7369 7469 6f6e  renderedPosition
+00088670: 2822 7922 292d 652e 7461 7267 6574 2829  ("y")-e.target()
+00088680: 2e72 656e 6465 7265 6450 6f73 6974 696f  .renderedPositio
+00088690: 6e28 2279 2229 292c 6e3d 5b2d 312a 742c  n("y")),n=[-1*t,
+000886a0: 745d 3b65 2e64 6174 6128 2263 6f6e 7472  t];e.data("contr
+000886b0: 6f6c 506f 696e 7444 6973 7461 6e63 6573  olPointDistances
+000886c0: 222c 6e2e 6a6f 696e 2822 2022 2929 7d28  ",n.join(" "))}(
+000886d0: 6529 2929 2c69 7d7d 7661 7220 693d 6e28  e))),i}}var i=n(
+000886e0: 3333 3739 292c 6f3d 6e2e 6e28 6929 2c61  3379),o=n.n(i),a
+000886f0: 3d6e 2837 3739 3529 2c73 3d6e 2e6e 2861  =n(7795),s=n.n(a
+00088700: 292c 753d 6e28 3536 3929 2c6c 3d6e 2e6e  ),u=n(569),l=n.n
+00088710: 2875 292c 633d 6e28 3335 3635 292c 643d  (u),c=n(3565),d=
+00088720: 6e2e 6e28 6329 2c68 3d6e 2839 3231 3629  n.n(c),h=n(9216)
+00088730: 2c66 3d6e 2e6e 2868 292c 703d 6e28 3435  ,f=n.n(h),p=n(45
+00088740: 3839 292c 763d 6e2e 6e28 7029 2c67 3d6e  89),v=n.n(p),g=n
+00088750: 2837 3231 292c 793d 7b7d 3b79 2e73 7479  (721),y={};y.sty
+00088760: 6c65 5461 6754 7261 6e73 666f 726d 3d76  leTagTransform=v
+00088770: 2829 2c79 2e73 6574 4174 7472 6962 7574  (),y.setAttribut
+00088780: 6573 3d64 2829 2c79 2e69 6e73 6572 743d  es=d(),y.insert=
+00088790: 6c28 292e 6269 6e64 286e 756c 6c2c 2268  l().bind(null,"h
+000887a0: 6561 6422 292c 792e 646f 6d41 5049 3d73  ead"),y.domAPI=s
+000887b0: 2829 2c79 2e69 6e73 6572 7453 7479 6c65  (),y.insertStyle
+000887c0: 456c 656d 656e 743d 6628 292c 6f28 2928  Element=f(),o()(
+000887d0: 672e 5a2c 7929 2c67 2e5a 2626 672e 5a2e  g.Z,y),g.Z&&g.Z.
+000887e0: 6c6f 6361 6c73 2626 672e 5a2e 6c6f 6361  locals&&g.Z.loca
+000887f0: 6c73 2c6e 2839 3735 3529 3b6c 6574 206d  ls,n(9755);let m
+00088800: 3d6e 2839 3035 3829 2c62 3d6e 2834 3734  =n(9058),b=n(474
+00088810: 293b 7661 7220 783d 6e65 7720 4172 7261  );var x=new Arra
+00088820: 793b 6675 6e63 7469 6f6e 2077 2865 297b  y;function w(e){
+00088830: 666f 7228 636f 6e73 745b 742c 6e5d 6f66  for(const[t,n]of
+00088840: 2065 2e6e 6f64 6573 2829 2e65 6e74 7269   e.nodes().entri
+00088850: 6573 2829 2978 2e70 7573 6828 6e2e 6964  es())x.push(n.id
+00088860: 2829 293b 652e 6e6f 6465 7328 292e 7374  ());e.nodes().st
+00088870: 796c 6528 7b22 6261 636b 6772 6f75 6e64  yle({"background
+00088880: 2d63 6f6c 6f72 223a 2223 4235 4432 4442  -color":"#B5D2DB
+00088890: 227d 292c 652e 6564 6765 7328 292e 7374  "}),e.edges().st
+000888a0: 796c 6528 7b22 6c69 6e65 2d63 6f6c 6f72  yle({"line-color
+000888b0: 223a 2267 7265 656e 227d 292c 652e 6564  ":"green"}),e.ed
+000888c0: 6765 7328 292e 7374 796c 6528 7b22 7461  ges().style({"ta
+000888d0: 7267 6574 2d61 7272 6f77 2d63 6f6c 6f72  rget-arrow-color
+000888e0: 223a 2267 7265 656e 227d 297d 6675 6e63  ":"green"})}func
+000888f0: 7469 6f6e 2045 2865 297b 666f 7228 636f  tion E(e){for(co
+00088900: 6e73 745b 742c 6e5d 6f66 2065 2e6e 6f64  nst[t,n]of e.nod
+00088910: 6573 2829 2e65 6e74 7269 6573 2829 297b  es().entries()){
+00088920: 636f 6e73 7420 653d 782e 696e 6465 784f  const e=x.indexO
+00088930: 6628 6e2e 6964 2829 293b 782e 7370 6c69  f(n.id());x.spli
+00088940: 6365 2865 2c31 297d 652e 6e6f 6465 7328  ce(e,1)}e.nodes(
+00088950: 292e 7374 796c 6528 7b22 6261 636b 6772  ).style({"backgr
+00088960: 6f75 6e64 2d63 6f6c 6f72 223a 2223 4345  ound-color":"#CE
+00088970: 4344 4636 227d 292c 652e 6564 6765 7328  CDF6"}),e.edges(
+00088980: 292e 7374 796c 6528 7b22 6c69 6e65 2d63  ).style({"line-c
+00088990: 6f6c 6f72 223a 2267 7261 7922 7d29 2c65  olor":"gray"}),e
+000889a0: 2e65 6467 6573 2829 2e73 7479 6c65 287b  .edges().style({
+000889b0: 2274 6172 6765 742d 6172 726f 772d 636f  "target-arrow-co
+000889c0: 6c6f 7222 3a22 6772 6179 227d 297d 6228  lor":"gray"})}b(
+000889d0: 6d29 3b76 6172 206b 2c43 3d6e 2839 3133  m);var k,C=n(913
+000889e0: 3829 2c53 3d7b 7d3b 532e 7374 796c 6554  8),S={};S.styleT
+000889f0: 6167 5472 616e 7366 6f72 6d3d 7628 292c  agTransform=v(),
+00088a00: 532e 7365 7441 7474 7269 6275 7465 733d  S.setAttributes=
+00088a10: 6428 292c 532e 696e 7365 7274 3d6c 2829  d(),S.insert=l()
+00088a20: 2e62 696e 6428 6e75 6c6c 2c22 6865 6164  .bind(null,"head
+00088a30: 2229 2c53 2e64 6f6d 4150 493d 7328 292c  "),S.domAPI=s(),
+00088a40: 532e 696e 7365 7274 5374 796c 6545 6c65  S.insertStyleEle
+00088a50: 6d65 6e74 3d66 2829 2c6f 2829 2843 2e5a  ment=f(),o()(C.Z
+00088a60: 2c53 292c 432e 5a26 2643 2e5a 2e6c 6f63  ,S),C.Z&&C.Z.loc
+00088a70: 616c 7326 2643 2e5a 2e6c 6f63 616c 732c  als&&C.Z.locals,
+00088a80: 6665 7463 6828 226d 616e 6966 6573 742e  fetch("manifest.
+00088a90: 6a73 6f6e 2229 2e74 6865 6e28 2865 3d3e  json").then((e=>
+00088aa0: 652e 6a73 6f6e 2829 2929 2e74 6865 6e28  e.json())).then(
+00088ab0: 2865 3d3e 6b3d 6529 292e 7468 656e 2828  (e=>k=e)).then((
+00088ac0: 2829 3d3e 6675 6e63 7469 6f6e 2865 297b  ()=>function(e){
+00088ad0: 7661 7220 743d 6e65 7720 7228 6529 2e63  var t=new r(e).c
+00088ae0: 7265 6174 655f 6379 746f 7363 6170 655f  reate_cytoscape_
+00088af0: 6772 6170 6828 292c 6e3d 7b65 7674 5479  graph(),n={evtTy
+00088b00: 7065 3a22 6378 7474 6170 222c 6d65 6e75  pe:"cxttap",menu
+00088b10: 4974 656d 733a 5b7b 6964 3a22 6578 706f  Items:[{id:"expo
+00088b20: 7274 504e 4722 2c63 6f6e 7465 6e74 3a22  rtPNG",content:"
+00088b30: 4578 706f 7274 2050 4e47 222c 746f 6f6c  Export PNG",tool
+00088b40: 7469 7054 6578 743a 2245 7870 6f72 7420  tipText:"Export 
+00088b50: 7468 6520 4441 4720 6173 2061 2050 4e47  the DAG as a PNG
+00088b60: 222c 7365 6c65 6374 6f72 3a22 6e6f 6465  ",selector:"node
+00088b70: 222c 636f 7265 4173 5765 6c6c 3a21 302c  ",coreAsWell:!0,
+00088b80: 6f6e 436c 6963 6b46 756e 6374 696f 6e3a  onClickFunction:
+00088b90: 6675 6e63 7469 6f6e 2865 297b 7661 7220  function(e){var 
+00088ba0: 6e3d 742e 706e 6728 7b62 673a 2272 6762  n=t.png({bg:"rgb
+00088bb0: 2832 3335 2c32 3335 2c32 3335 2922 7d29  (235,235,235)"})
+00088bc0: 2c72 3d64 6f63 756d 656e 742e 6372 6561  ,r=document.crea
+00088bd0: 7465 456c 656d 656e 7428 2261 2229 3b72  teElement("a");r
+00088be0: 2e64 6f77 6e6c 6f61 643d 2270 7269 736d  .download="prism
+00088bf0: 2d64 6167 2e70 6e67 222c 722e 6872 6566  -dag.png",r.href
+00088c00: 3d6e 2c72 2e63 6c69 636b 2829 7d7d 5d2c  =n,r.click()}}],
+00088c10: 6d65 6e75 4974 656d 436c 6173 7365 733a  menuItemClasses:
+00088c20: 5b22 6379 2d63 6f6e 7465 7874 2d6d 656e  ["cy-context-men
+00088c30: 7573 2d63 7874 2d6d 656e 7569 7465 6d22  us-cxt-menuitem"
+00088c40: 2c22 6379 2d63 6f6e 7465 7874 2d6d 656e  ,"cy-context-men
+00088c50: 7573 2d64 6976 6964 6572 225d 2c63 6f6e  us-divider"],con
+00088c60: 7465 7874 4d65 6e75 436c 6173 7365 733a  textMenuClasses:
+00088c70: 5b22 6379 2d63 6f6e 7465 7874 2d6d 656e  ["cy-context-men
+00088c80: 7573 2d63 7874 2d6d 656e 7522 5d7d 3b74  us-cxt-menu"]};t
+00088c90: 2e63 6f6e 7465 7874 4d65 6e75 7328 6e29  .contextMenus(n)
+00088ca0: 3b76 6172 2069 3d2d 313b 742e 6f6e 2822  ;var i=-1;t.on("
+00088cb0: 636c 6963 6b22 2c22 6e6f 6465 222c 2866  click","node",(f
+00088cc0: 756e 6374 696f 6e28 6529 7b6c 6574 206e  unction(e){let n
+00088cd0: 3d65 2e74 6172 6765 742e 6964 2829 3b76  =e.target.id();v
+00088ce0: 6172 2072 3d74 2e24 2822 2322 2b6e 292c  ar r=t.$("#"+n),
+00088cf0: 6f3d 722e 7072 6564 6563 6573 736f 7273  o=r.predecessors
+00088d00: 2829 2c61 3d72 2e73 7563 6365 7373 6f72  (),a=r.successor
+00088d10: 7328 293b 6966 2869 3d3d 6e29 4528 7229  s();if(i==n)E(r)
+00088d20: 2c45 286f 292c 4528 6129 2c69 3d2d 313b  ,E(o),E(a),i=-1;
+00088d30: 656c 7365 7b69 6628 2d31 213d 6929 7b76  else{if(-1!=i){v
+00088d40: 6172 2073 3d74 2e24 2822 2322 2b69 292c  ar s=t.$("#"+i),
+00088d50: 753d 732e 7072 6564 6563 6573 736f 7273  u=s.predecessors
+00088d60: 2829 2c6c 3d73 2e73 7563 6365 7373 6f72  (),l=s.successor
+00088d70: 7328 293b 4528 7329 2c45 2875 292c 4528  s();E(s),E(u),E(
+00088d80: 6c29 7d77 2872 292c 7728 6f29 2c77 2861  l)}w(r),w(o),w(a
+00088d90: 292c 693d 6e7d 7d29 297d 286b 2929 292e  ),i=n}}))}(k))).
+00088da0: 6361 7463 6828 2866 756e 6374 696f 6e28  catch((function(
+00088db0: 6529 7b63 6f6e 736f 6c65 2e6c 6f67 2865  e){console.log(e
+00088dc0: 292c 7769 6e64 6f77 2e61 6c65 7274 2822  ),window.alert("
+00088dd0: 6d61 6e69 6665 7374 2e6a 736f 6e20 6e6f  manifest.json no
+00088de0: 7420 666f 756e 6420 696e 2063 6f6d 7069  t found in compi
+00088df0: 6c65 6420 6469 7265 6374 6f72 795c 6e72  led directory\nr
+00088e00: 652d 636f 6d70 696c 6520 7468 6520 7072  e-compile the pr
+00088e10: 6f6a 6563 7420 616e 6420 7472 7920 6167  oject and try ag
+00088e20: 6169 6e22 297d 2929 7d29 2829 7d29 2829  ain")}))})()})()
+00088e30: 3b3c 2f73 6372 6970 743e 3c2f 626f 6479  ;</script></body
+00088e40: 3e3c 2f68 746d 6c3e                      ></html>
```

### Comparing `prism-ds-0.2.0rc1/prism/docs/build/main.js.LICENSE.txt` & `prism-ds-0.2.0rc2/prism/docs/build/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/event_managers/base.py` & `prism-ds-0.2.0rc2/prism/event_managers/base.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/exceptions.py` & `prism-ds-0.2.0rc2/prism/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,17 +71,17 @@
         self.message = message
         super().__init__(self.message)
 
     def __str__(self):
         return self.message
 
 
-class ModulesDirNotFoundException(PrismException):
+class TasksDirNotFoundException(PrismException):
     """
-    Exception raised if modules dir isn't not found
+    Exception raised if tasks dir isn't not found
     """
 
     def __init__(self, message):
         self.message = message
         super().__init__(self.message)
 
     def __str__(self):
@@ -340,7 +340,20 @@
 
     def __init__(self, task_name):
         self.message = f"invalid task name `{task_name}`...task names should only have lowercase letters and underscores"  # noqa: E501
         super().__init__(self.message)
 
     def __str__(self):
         return self.message
+
+
+class ReferenceException(PrismException):
+    """
+    Exception raised with a bad `tasks.ref()` call
+    """
+
+    def __init__(self, message):
+        self.message = message
+        super().__init__(self.message)
+
+    def __str__(self):
+        return self.message
```

### Comparing `prism-ds-0.2.0rc1/prism/infra/compiler.py` & `prism-ds-0.2.0rc2/prism/infra/compiler.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,122 +17,160 @@
 from typing import Any, Dict, List, Optional, Tuple
 
 # Prism-specific imports
 import prism.constants
 import prism.exceptions
 import prism.prism_logging
 import prism.parsers.ast_parser as ast_parser
-import prism.infra.module
-from prism.infra.manifest import Manifest, ModuleManifest
+import prism.infra.compiled_task
+from prism.infra.manifest import Manifest, TaskManifest
 from prism.infra.project import PrismProject
 
 
 ####################
 # Class definition #
 ####################
 
 class CompiledDag:
     """
     Compiled DAG
     """
     def __init__(self,
-        modules_dir: Path,
+        tasks_dir: Path,
         nxdag: nx.DiGraph,
-        topological_sort: List[Path],
-        user_arg_modules: List[Path],
-        module_manifests: Dict[Path, ModuleManifest]
+        topological_sort: List[str],
+        user_arg_tasks: List[str],
+        task_manifests: Dict[str, TaskManifest],
+        parsed_tasks: List[ast_parser.AstParser],
     ):
-        self.modules_dir = modules_dir
+        self.tasks_dir = tasks_dir
         self.nxdag = nxdag
         self.topological_sort = topological_sort
-        self.user_arg_modules = user_arg_modules
-        self.module_manifests = module_manifests
+        self.user_arg_tasks = user_arg_tasks
+        self.task_manifests = task_manifests
+        self.parsed_tasks = parsed_tasks
 
         # Store full paths in attribute
-        self.topological_sort_full_path = [
-            self.modules_dir / module for module in self.topological_sort
-        ]
-
-        # Create module objects
-        self.compiled_modules = []
-        for relative, full in zip(self.topological_sort, self.topological_sort_full_path):  # noqa: E501
-            self.compiled_modules.append(
-                prism.infra.module.CompiledModule(
-                    relative, full, self.module_manifests[relative]
+        self.topological_sort_full_path = []
+
+        # Create task objects
+        self.compiled_tasks = []
+        for _task in self.topological_sort:
+            # Task name
+            task_name = _task.split('.')[1]
+
+            # Relative path and full path
+            relative_path = Path(f'{_task.split(".")[0]}.py')
+            full_path = tasks_dir / relative_path
+
+            # Current parser
+            task_ast_parser = [
+                _p for _p in self.parsed_tasks if _p.task_relative_path == relative_path  # noqa: E501
+            ][0]
+
+            # Update attribute
+            self.topological_sort_full_path.append(full_path)
+
+            # Compiled task
+            self.compiled_tasks.append(
+                prism.infra.compiled_task.CompiledTask(
+                    task_name,
+                    relative_path,
+                    full_path,
+                    self.task_manifests[_task],
+                    task_ast_parser,
                 )
             )
 
 
 class DagCompiler:
     """
     Class for parsing mod refs, building DAG
     """
 
     def __init__(self,
         project_dir: Path,
+        tasks_dir: Path,
         compiled_dir: Path,
-        all_modules: List[Path],
-        user_arg_modules: List[Path],
+        all_tasks: List[str],
+        parsed_tasks: List[ast_parser.AstParser],
+        user_arg_tasks: List[str],
         user_arg_all_downstream: bool,
         project: Optional[PrismProject] = None
     ):
         self.project_dir = project_dir
         self.compiled_dir = compiled_dir
-        self.all_modules = all_modules
-        self.user_arg_modules = user_arg_modules
+        self.all_tasks = all_tasks
+        self.user_arg_tasks = user_arg_tasks
         self.project = project
         os.chdir(project_dir)
 
-        # Modules can only be executed if their predecessors are explicitly run or have
+        # Parsed tasks
+        self.parsed_tasks = parsed_tasks
+
+        # Tasks can only be executed if their predecessors are explicitly run or have
         # targets. For example, if our DAG is A --> B --> C and we call `prism run
-        # --module C`, then Prism will parse the execution order, instantiate but NOT
+        # --task C`, then Prism will parse the execution order, instantiate but NOT
         # execute tasks A and B, and then run task C. In other words, A and B will
         # always be instantiated; the --all-upstream argument controls whether A and B
         # are executed.
 
         # This is why we don't need to keep track of the --all-upstream argument; it
         # doesn't affect what our topological sort looks like. However, the
         # --all-downstream argument does, since successors do not need to be
         # instantiated at all.
         self.user_arg_all_downstream = user_arg_all_downstream
 
-        # Path of modules
-        self.modules_dir = self.project_dir / 'modules'
+        # Path of tasks
+        self.tasks_dir = tasks_dir
 
-        # Module manifests
-        self.module_manifests: Dict[Path, ModuleManifest] = {}
+        # Task manifests
+        self.task_manifests: Dict[str, TaskManifest] = {}
 
     def parse_task_refs(self,
-        modules: List[Path],
-        parent_path: Path
-    ) -> Dict[Path, Any]:
+        tasks: List[str],
+        parsed_tasks: List[ast_parser.AstParser],
+    ) -> Dict[str, List[str]]:
         """
         Parse node dictionary listed at the beginning of each python script. If
         node_dict does not exist in any script, throw an error.
 
         args:
-            modules: modules to compile
-            parent_path: parent path of modules
+            tasks: tasks to compile
+            parent_path: parent path of tasks
         returns:
-            module references as a dictionary
+            task references as a dictionary
         """
 
-        # This is only ever called on the output of `get_all_modules`, which sorts the
-        # modules alphabetically. Therefore, all mod refs will be sorted.
-        task_refs_dict: Dict[Path, Any] = {}
-        for m in modules:
-            parser = ast_parser.AstParser(m, parent_path)
-            task_refs = parser.parse()
-            if task_refs is None or task_refs == '' or task_refs == []:
-                task_refs_dict[m] = None
-            else:
-                task_refs_dict[m] = task_refs
+        # This is only ever called on the output of `get_all_tasks`, which sorts the
+        # tasks alphabetically. Therefore, all mod refs will be sorted.
+        task_refs_dict: Dict[str, List[str]] = {}
+
+        # Iterate through all of the tasks
+        for _mod in tasks:
+            # Current module / task
+            current_module = Path(f"{_mod.split('.')[0]}.py")
+            curr_task = _mod.split('.')[1]
+
+            # Current parser
+            curr_parser = [
+                _p for _p in parsed_tasks if _p.task_relative_path == current_module
+            ][0]
+
+            # Other parsers
+            other_parsers = [
+                _p for _p in parsed_tasks if _p.task_relative_path != current_module
+            ]
+
+            # Get task refs
+            task_refs = curr_parser.parse(curr_task, other_parsers)
+            task_refs_dict[_mod] = task_refs
 
-            # Keep track of module manifest
-            self.module_manifests[m] = parser.module_manifest
+            # Keep track of task manifest
+            self.task_manifests[_mod] = curr_parser.task_manifest
 
         return task_refs_dict
 
     def add_graph_elem(self,
         elem: Any,
         master: List[Any]
     ) -> List[Any]:
@@ -148,74 +186,70 @@
         if elem not in master:
             master += [elem]  # type: ignore
         else:
             return master
         return master
 
     def add_graph_node(self,
-        elem: Path,
-        master: List[Path]
-    ) -> List[Path]:
+        elem: str,
+        master: List[str]
+    ) -> List[str]:
         """
         To resolve mypy errors...
         """
         return self.add_graph_elem(elem, master)
 
     def add_graph_edge(self,
-        elem: Tuple[Path, Path],
-        master: List[Tuple[Path, Path]]
-    ) -> List[Tuple[Path, Path]]:
+        elem: Tuple[str, str],
+        master: List[Tuple[str, str]]
+    ) -> List[Tuple[str, str]]:
         """
         To resolve mypy errors...
         """
         return self.add_graph_elem(elem, master)
 
     def create_nodes_edges(self,
-        module_references: Dict[Path, Any]
-    ) -> Tuple[List[Path], List[Tuple[Path, Path]]]:
+        task_references: Dict[str, Any]
+    ) -> Tuple[List[str], List[Tuple[str, str]]]:
         """
-        Create nodes / edges from module connections
+        Create nodes / edges from task connections
 
         args:
-            module_references: connections defined via {{ mod(...) }} in modules
+            task_references: connections defined via {{ mod(...) }} in tasks
         outputs:
-            nodes: list of nodes (modules)
-            edges: list of edges (tuple of nodes, i.e. modules)
+            nodes: list of nodes (tasks)
+            edges: list of edges (tuple of nodes, i.e. tasks)
         """
-
         # Create edges and nodes
-        edges: List[Tuple[Path, Path]] = []
-        nodes: List[Path] = []
+        edges: List[Tuple[str, str]] = []
+        nodes: List[str] = []
 
-        # Iterate through module references. Keys represent distinct modules in the DAG,
-        # and values represent the modules that feed into the key.
-        for mod, ref in module_references.items():
+        # Iterate through task references. Keys represent distinct tasks in the DAG,
+        # and values represent the tasks that feed into the key.
+        for mod, refs in task_references.items():
             nodes = self.add_graph_node(mod, nodes)
-            if ref is None:
-                pass
-            elif isinstance(ref, Path):
-                nodes = self.add_graph_node(ref, nodes)
-                edges = self.add_graph_edge((ref, mod), edges)
+            if refs is None:
+                continue
             else:
-                for v in ref:
+                for v in refs:
                     nodes = self.add_graph_node(v, nodes)
                     edges = self.add_graph_edge((v, mod), edges)
         return nodes, edges
 
     def create_dag(self,
-        nodes: List[Path],
-        edges: List[Tuple[Path, Path]]
+        nodes: List[str],
+        edges: List[Tuple[str, str]]
     ) -> nx.DiGraph:
         """
         Create DAG from edges
 
         args:
-            user_arg_modules: modules passed in user arguments
-            nodes: list of nodes (modules)
-            edges: list of edges (tuple of nodes, i.e. modules)
+            user_arg_tasks: tasks passed in user arguments
+            nodes: list of nodes (tasks)
+            edges: list of edges (tuple of nodes, i.e. tasks)
         outputs:
             topological sort of edges
         """
         # Instantiate graph
         graph = nx.DiGraph()
 
         # If there are no nodes in the DAG, then throw an error. This should never
@@ -234,21 +268,20 @@
             for component in all_scc:
                 component = set([str(elem) for elem in list(component)])
                 if len(component) > 1:
                     cycles.append(component)
             raise prism.exceptions.DAGException(
                 message=f"invalid DAG, cycle found in {str(cycles)}"
             )
-
         return graph
 
     def get_node_dependencies(self,
         graph: nx.DiGraph,
-        start_nodes: List[Path]
-    ) -> List[Path]:
+        start_nodes: List[str]
+    ) -> List[str]:
         """
         Parse the DiGraph and get all nodes upstream of the `start_nodes`
 
         args:
             graph: DAG
             start_nodes: list of nodes for which to retrieve upstream dependencies
         returns:
@@ -264,16 +297,16 @@
 
         # Get unique dependencies
         unique_deps = list(set(deps))
         return unique_deps
 
     def get_node_successors(self,
         graph: nx.DiGraph,
-        start_nodes: List[Path]
-    ) -> List[Path]:
+        start_nodes: List[str]
+    ) -> List[str]:
         """
         Parse the DiGraph and get all nodes downstream of the `start_nodes`
 
         args:
             graph: DAG
             start_nodes: list of nodes for which to retrieve upstream dependencies
         returns:
@@ -288,87 +321,89 @@
                 successors.append(postnode)
 
         # Get unique dependencies
         unique_successors = list(set(successors))
         return unique_successors
 
     def create_topsort(self,
-        all_modules: List[Path],
-        user_arg_modules: List[Path],
-        parent_path: Path
+        all_tasks: List[str],
+        user_arg_tasks: List[str],
+        parsed_tasks: List[ast_parser.AstParser],
     ) -> Any:
         """
         Parse mod refs, create the DAG, and create a topological sort of the DAG
 
         args:
-            all_modules: list of all modules
-            user_arg_modules: modules passed in user arguments
-            parent_path: path containing the modules
-            compiler_dict: globals dictionary for compiler
+            all_tasks: list of all tasks
+            user_arg_tasks: tasks passed in user arguments
+            parsed_tasks: list of AstParsers associated with each task module
         returns:
             topological sorted DAG as a list
         """
 
-        # Create a DAG using all the modules. We use `all_modules` instead of
-        # `user_arg_modules`, because using `user_arg_modules` will only compile/run the
-        # modules referenced in the modules themselves. For example, if we have a dag A
+        # Create a DAG using all the tasks. We use `all_tasks` instead of
+        # `user_arg_tasks`, because using `user_arg_tasks` will only compile/run the
+        # tasks referenced in the tasks themselves. For example, if we have a dag A
         # --> B --> C and wish to to only compile/run script C, then our code will only
         # run script B. This will throw an error, because script B relies on script A,
         # and we will need to instantiate the script A task for the script B task to
         # execute fully.
-        task_refs = self.parse_task_refs(all_modules, parent_path)
+        task_refs = self.parse_task_refs(
+            all_tasks,
+            parsed_tasks,
+        )
         nodes, edges = self.create_nodes_edges(task_refs)
         dag = self.create_dag(nodes, edges)
 
-        # If `user_arg_modules` is equivalent to `all_modules`, then create a
+        # If `user_arg_tasks` is equivalent to `all_tasks`, then create a
         # topological sorting of the full DAG. From the NetworkX documentation: A
         # topological sort is a nonunique permutation of the nodes of a directed graph
         # such that an edge from u to v implies that u appears before v in the
         # topological sort order. This ordering is valid only if the graph has no
         # directed cycles.
-        if len(user_arg_modules) == len(all_modules):
+        if len(user_arg_tasks) == len(all_tasks):
             all_topological_sorts = nx.algorithms.dag.all_topological_sorts(dag)
             all_topological_sorts_list = next(all_topological_sorts)
 
-        # Otherwise, the user has selected to run a subset of the modules. Identify all
-        # modules upstream (and potentially downstream) of `user_arg_modules`.
+        # Otherwise, the user has selected to run a subset of the tasks. Identify all
+        # tasks upstream (and potentially downstream) of `user_arg_tasks`.
         else:
 
             # Keep only the dependencies, and create a topological sort.
-            all_nodes = self.get_node_dependencies(dag, user_arg_modules)
+            all_nodes = self.get_node_dependencies(dag, user_arg_tasks)
 
             # Add successors if the user wants them
             if self.user_arg_all_downstream:
-                all_nodes.extend(self.get_node_successors(dag, user_arg_modules))
+                all_nodes.extend(self.get_node_successors(dag, user_arg_tasks))
 
             subgraph = dag.subgraph(list(set(all_nodes)))
             all_topological_sorts = nx.algorithms.dag.all_topological_sorts(subgraph)  # noqa: E501
             all_topological_sorts_list = next(all_topological_sorts)
 
-        # Add each module to manifest
+        # Add each task to manifest
         for elem in all_topological_sorts_list:
 
             # Raise error if node not in project
-            if elem not in all_modules:
+            if elem not in all_tasks:
                 raise prism.exceptions.CompileException(
-                    message=f'module `{str(elem)}` not found in project'
+                    message=f'task `{str(elem)}` not found in project'
                 )
 
         return dag, all_topological_sorts_list
 
     def compile(self) -> CompiledDag:
         """
         Compile the DAG
         """
         nxdag, all_topological_sorts_list = self.create_topsort(
-            self.all_modules, self.user_arg_modules, self.modules_dir
+            self.all_tasks, self.user_arg_tasks, self.parsed_tasks
         )
 
         # Dump manifest
-        manifest = Manifest(list(self.module_manifests.values()))
+        manifest = Manifest(list(self.task_manifests.values()))
 
         # Add the prism project to the Manifest
         if self.project is not None:
             prism_project_py_str = self.project.prism_project_py_str
         else:
             prism_project = PrismProject(
                 project_dir=self.project_dir,
@@ -378,14 +413,15 @@
             )
             prism_project_py_str = prism_project.prism_project_py_str
         manifest.add_prism_project(prism_project_py_str)
         manifest.json_dump(self.compiled_dir)
 
         # Return dag
         dag = CompiledDag(
-            self.modules_dir,
+            self.tasks_dir,
             nxdag,
             all_topological_sorts_list,
-            self.user_arg_modules,
-            self.module_manifests
+            self.user_arg_tasks,
+            self.task_manifests,
+            self.parsed_tasks,
         )
         return dag
```

### Comparing `prism-ds-0.2.0rc1/prism/infra/executor.py` & `prism-ds-0.2.0rc2/prism/infra/executor.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 
 # Standard library imports
 from dataclasses import dataclass
 from multiprocessing.dummy import Pool
 from pathlib import Path
 import time
 from typing import Any, Dict, List, Optional, Union
+import re
 
 # Prism-specific imports
 import prism.exceptions
-from prism.infra import module as prism_module
+from prism.infra import compiled_task
 from prism.infra import compiler as prism_compiler
 from prism.infra.task_manager import PrismTaskManager
 from prism.infra.hooks import PrismHooks
 import prism.prism_logging
 from prism.prism_logging import Event, fire_console_event
 from prism.event_managers import base as base_event_manager
 from prism.constants import INTERNAL_TASK_MANAGER_VARNAME, INTERNAL_HOOKS_VARNAME
@@ -58,27 +59,27 @@
         threads: int,
         user_context: Dict[Any, Any] = {}
     ):
         self.project_dir = project_dir
         self.compiled_dag = compiled_dag
 
         # Extract attributes from compiled_dag instance
-        self.compiled_modules = self.compiled_dag.compiled_modules
+        self.compiled_tasks = self.compiled_dag.compiled_tasks
         self.nxdag = self.compiled_dag.nxdag
-        self.topological_sort_relative_path = self.compiled_dag.topological_sort
+        self.topological_sort_task_names = self.compiled_dag.topological_sort
         self.topological_sort_full_path = self.compiled_dag.topological_sort_full_path
-        self.user_arg_modules = self.compiled_dag.user_arg_modules
+        self.user_arg_tasks = self.compiled_dag.user_arg_tasks
         self.user_arg_all_upstream = user_arg_all_upstream
         self.user_arg_all_downstream = user_arg_all_downstream
         self.user_context = user_context
 
         # Identify nodes not explicitly run and update (only if --all-upstream is False)
         if not self.user_arg_all_upstream and not self.user_arg_all_downstream:
             self.nodes_not_explicitly_run = list(
-                set(self.topological_sort_relative_path) - set(self.user_arg_modules)
+                set(self.topological_sort_task_names) - set(self.user_arg_tasks)
             )
         else:
             self.nodes_not_explicitly_run = []
 
         # Number of processes used to run concurrent tasks
         self.threads = threads
 
@@ -87,122 +88,134 @@
         Set executor globals; needs to be called before `exec`
 
         args:
             run_context: globals for DAG execution
         """
         self.run_context = run_context
 
-    def check_task_refs(self, module: prism_module.CompiledModule) -> List[str]:
+    def check_task_refs(self, task: compiled_task.CompiledTask) -> List[str]:
         """
         Get task refs
 
         args:
-            module: CompiledModule object
+            task: CompiledTask object
         returns:
             refs as a list of strings
         """
-        if isinstance(module.refs, str):
-            return [module.refs]
+        if isinstance(task.refs, str):
+            return [task.refs]
         else:
-            if not isinstance(module.refs, list):
+            if not isinstance(task.refs, list):
                 raise prism.exceptions.CompileException(
-                    message=f'invalid type `{type(module.refs)}`, must be list'
+                    message=f'invalid type `{type(task.refs)}`, must be list'
                 )
-            return module.refs
+            return task.refs
 
     def exec_single(self,
         full_tb: bool,
-        module: prism_module.CompiledModule,
+        task: compiled_task.CompiledTask,
         task_manager: Union[int, PrismTaskManager],
         hooks: PrismHooks,
         user_context: Dict[Any, Any] = {}
     ) -> base_event_manager.EventManagerOutput:
         """
-        Callback used to get results of module execution in Pool
+        Callback used to get results of task execution in Pool
         """
+        # Keep track of current module in tasks manager
+        if isinstance(task_manager, PrismTaskManager):
+            task_manager.curr_module = re.sub(
+                r'\.py$', '', task.task_relative_path.name
+            )
+
         # Keep track of events
         event_list: List[Event] = []
         if task_manager == 0:
-            base_event_manager.EventManagerOutput(0, None, event_list)
-        relative_path = module.module_relative_path
-        full_path = module.module_full_path
+            return base_event_manager.EventManagerOutput(0, None, event_list)
+        task_name = task.task_var_name
+        relative_path = task.task_relative_path
 
         # Boolean for whether to fire exec event for current script. We do not want to
         # fire the exec events if the user did not explicitly include the script in
         # their arguments
-        fire_exec_events = relative_path in self.user_arg_modules \
+        fire_exec_events = task_name in self.user_arg_tasks \
             or self.user_arg_all_upstream \
             or self.user_arg_all_downstream
 
-        # If all upstream modules are to be run, the compute the idx and total using the
+        # If all upstream tasks are to be run, the compute the idx and total using the
         # `dag`` list. Otherwise, if the script is explicitly included in the user's run
-        # command then compute the idx and total using the `modules` list. Otherwise,
+        # command then compute the idx and total using the `tasks` list. Otherwise,
         # set both to None.
 
-        # First, sort the user arg modules in the order in which they appear in the DAG
-        modules_idx = [
-            self.topological_sort_relative_path.index(m) for m in self.user_arg_modules
+        # First, sort the user arg tasks in the order in which they appear in the DAG
+        tasks_idx = [
+            self.topological_sort_task_names.index(m) for m in self.user_arg_tasks
         ]
-        modules_sorted = [x for _, x in sorted(zip(modules_idx, self.user_arg_modules))]
+        tasks_sorted = [x for _, x in sorted(zip(tasks_idx, self.user_arg_tasks))]
 
         # Define the idx and total
         if self.user_arg_all_upstream or self.user_arg_all_downstream:
-            idx = self.topological_sort_full_path.index(full_path) + 1
-            total = len(self.topological_sort_full_path)
-        elif relative_path in self.user_arg_modules:
-            idx = modules_sorted.index(relative_path) + 1
-            total = len(modules_sorted)
+            idx = self.topological_sort_task_names.index(task_name) + 1
+            total = len(self.topological_sort_task_names)
+        elif task_name in self.user_arg_tasks:
+            idx = tasks_sorted.index(task_name) + 1
+            total = len(tasks_sorted)
         else:
             idx = None
             total = None
 
-        # Event manager. We want '__file__' to be the path to the un-compiled module.
+        # Event manager. We want '__file__' to be the path to the un-compiled task.
         # Instances of DagExecutor will only be called within the project directory.
-        # Therefore, __files__ should be modules/{name of script}
+        # Therefore, __files__ should be tasks/{name of script}
         self.run_context['__file__'] = str(
-            self.project_dir / f'modules/{str(relative_path)}'
+            Path(self.compiled_dag.tasks_dir) / str(relative_path)
         )
 
-        # Execute the module with appropriate number of retries
-        retries, retry_delay_seconds = module.grab_retries_metadata()
+        # Execute the task with appropriate number of retries
+        retries, retry_delay_seconds = task.grab_retries_metadata()
         num_runs = 0
         num_expected_runs = retries + 1
         outputs = 0
-        name = module.name
+        name = task.task_var_name
 
         # For testing, keep track of all events
         all_events = []
 
         while num_runs != num_expected_runs and outputs == 0:
+            # Keep track of script events
+            script_event_list: List[Event] = []
+
             num_runs += 1
             if num_runs > 1:
-                event_list = fire_console_event(
-                    prism.prism_logging.DelayEvent(name, retry_delay_seconds),
+                script_event_list = fire_console_event(
+                    prism.prism_logging.DelayEvent(
+                        name, retry_delay_seconds
+                    ),
+                    script_event_list,
                     log_level='warn'
                 )
                 time.sleep(retry_delay_seconds)
-                name = module.name + f' (RETRY {num_runs - 1})'
+                name = name + f' (RETRY {num_runs - 1})'
 
             # Only fire empty line if last retry has been executed
             fire_empty_line_events = num_runs == num_expected_runs
             script_manager = base_event_manager.BaseEventManager(
                 idx=idx,
                 total=total,
                 name=name,
                 full_tb=full_tb,
-                func=module.exec
+                func=task.exec
             )
             script_event_manager_result: base_event_manager.EventManagerOutput = script_manager.manage_events_during_run(  # noqa: E501
-                event_list,
+                script_event_list,
                 fire_exec_events,
                 fire_empty_line_events,
                 run_context=self.run_context,
                 task_manager=task_manager,
                 hooks=hooks,
-                explicit_run=relative_path not in self.nodes_not_explicitly_run,
+                explicit_run=task.task_var_name not in self.nodes_not_explicitly_run,
                 user_context=user_context
             )
 
             # All events
             all_events += script_event_manager_result.event_list
 
             # Set output
@@ -220,15 +233,15 @@
         pool.close()
         pool.terminate()
         pool.join()
 
     def exec(self, full_tb: bool):
         """
         Execute DAG. Our general approach is as follows:
-            1. Create a queue of the tasks (i.e., the modules) that need to be executed.
+            1. Create a queue of the tasks (i.e., the tasks) that need to be executed.
             2. Create a pool with `n` processes
             3. While queue is not empty
                 - Get task from the top of the queue
                 - If task doesn't have any refs, add it to the pool
                 - If task does have refs, then wait for those refs to finish before
                   adding it to pool
                 - Once task has been added to queue, remove it from queue
@@ -253,18 +266,18 @@
 
         # Execute all statements, stopping at first error
         self.task_manager = self.run_context[INTERNAL_TASK_MANAGER_VARNAME]
         self.hooks = self.run_context[INTERNAL_HOOKS_VARNAME]
         self._wait_and_return = False
         self.error_event = None
 
-        # If single-threaded, just run the modules in order
+        # If single-threaded, just run the tasks in order
         if self.threads == 1:
-            while self.compiled_modules != []:
-                curr = self.compiled_modules.pop(0)
+            while self.compiled_tasks != []:
+                curr: compiled_task.CompiledTask = self.compiled_tasks.pop(0)
                 result = self.exec_single(
                     full_tb,
                     curr,
                     self.task_manager,
                     self.hooks,
                     self.user_context
                 )
@@ -272,40 +285,40 @@
                 if self.task_manager == 0:
                     return ExecutorOutput(0, self.error_event, self.event_list)
 
             # We need the error event and event list to cascade up to the PrismPipeline
             # class.
             return ExecutorOutput(1, self.error_event, self.event_list)
 
-        # If the pool has multiple threads, then iterate through modules and add them to
+        # If the pool has multiple threads, then iterate through tasks and add them to
         # the Pool
         else:
             async_results = {}
             with Pool(processes=self.threads) as pool:
-                while self.compiled_modules != []:
+                while self.compiled_tasks != []:
 
-                    # Get first module to execute
-                    curr = self.compiled_modules[0]
+                    # Get first task to execute
+                    curr = self.compiled_tasks[0]
                     refs = self.check_task_refs(curr)
 
                     # If an error occurred, skip all remaining tasks
                     if self._wait_and_return:
                         break  # type: ignore
 
                     else:
 
-                        # If no refs, then add module to pool
+                        # If no refs, then add task to pool
                         if len(refs) == 0:
                             res = pool.apply_async(
                                 self.exec_single,
                                 args=(full_tb, curr, self.task_manager, self.hooks, self.user_context),  # noqa: E501
                                 callback=callback
                             )
-                            async_results[curr.name] = res
-                            self.compiled_modules.pop(0)
+                            async_results[curr.task_var_name] = res
+                            self.compiled_tasks.pop(0)
 
                         # Since DAG is run in order, refs should have been added to pool
                         # before current task. Wait for upstream tasks
                         else:
                             for ref in refs:
                                 async_results[ref].wait()
 
@@ -314,16 +327,16 @@
                                 break  # type: ignore
                             else:
                                 res = pool.apply_async(
                                     self.exec_single,
                                     args=(full_tb, curr, self.task_manager, self.hooks, self.user_context),  # noqa: E501
                                     callback=callback
                                 )
-                                async_results[curr.name] = res
-                                self.compiled_modules.pop(0)
+                                async_results[curr.task_var_name] = res
+                                self.compiled_tasks.pop(0)
                 pool.close()
                 pool.join()
 
             # If error was found, then terminate pool
             if self._wait_and_return:
                 self._cancel_connections(pool)
                 # We need the error event and event list to cascade up to the
```

### Comparing `prism-ds-0.2.0rc1/prism/infra/manifest.py` & `prism-ds-0.2.0rc2/prism/infra/manifest.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,88 +9,79 @@
 ###########
 # Imports #
 ###########
 
 # Standard library imports
 import json
 from pathlib import Path
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List
+import re
 
 
 ####################
 # Class definition #
 ####################
 
-class ModuleManifest:
+class TaskManifest:
     """
-    Class used to store metadata on a parsed module
+    Class used to store metadata on a parsed task
     """
 
     def __init__(self):
-        self.manifest_dict: Dict[str, Any] = {"targets": [], "modules": [], "refs": []}
+        self.manifest_dict: Dict[str, Any] = {"targets": {}, "tasks": [], "refs": {}}
 
-    def add_module(self, module_name: Path):
-        self.manifest_dict["modules"].append(str(module_name))
-
-    def add_ref(self, target: Path, source: Path):
-        obj = {
-            "target": str(target),
-            "source": str(source)
-        }
-        self.manifest_dict["refs"].append(obj)
-
-    def add_target(self, module_name: Path, loc: Union[str, List[str]]):
-        obj = {
-            "module_name": str(module_name),
-            "target_locs": loc
-        }
-        self.manifest_dict["targets"].append(obj)
+    def add_task(self,
+        task_module: Path,
+        task_name: str
+    ):
+        task_module_no_py = re.sub(r'\.py$', '', str(task_module))
+        processed_task_name = f"{task_module_no_py}.{task_name}"
+        self.manifest_dict["tasks"].append(processed_task_name)
+
+    def add_refs(self,
+        target_module: Path,
+        target_task: str,
+        sources: List[str]
+    ):
+        target_module_no_py = re.sub(r'\.py$', '', str(target_module))
+        if target_module_no_py not in self.manifest_dict["refs"].keys():
+            self.manifest_dict["refs"][target_module_no_py] = {}
+        self.manifest_dict["refs"][target_module_no_py][target_task] = sources
+
+    def add_targets(self,
+        module_relative_path: Path,
+        task_name: str,
+        locs: List[str]
+    ):
+        module_name_no_py = re.sub(r'\.py$', '', str(module_relative_path))
+        if module_name_no_py not in self.manifest_dict["targets"].keys():
+            self.manifest_dict["targets"][module_name_no_py] = {}
+        self.manifest_dict["targets"][module_name_no_py][task_name] = locs
 
 
 class Manifest:
     """
     Class used to store metadata on compiled prism project
     """
 
-    def __init__(self, module_manifests: List[ModuleManifest] = []):
+    def __init__(self, task_manifests: List[TaskManifest] = []):
         self.manifest_dict: Dict[str, Any] = {
-            "targets": [], "prism_project": "", "modules": [], "refs": []
+            "targets": {}, "prism_project": "", "tasks": [], "refs": {}
         }
-        self.module_manifests = module_manifests
+        self.task_manifests = task_manifests
 
-        # Iterate through module manifests and add to manifest
-        for mm in self.module_manifests:
-            self.manifest_dict["targets"].extend(mm.manifest_dict["targets"])
-            self.manifest_dict["modules"].extend(mm.manifest_dict["modules"])
-            self.manifest_dict["refs"].extend(mm.manifest_dict["refs"])
+        # Iterate through task manifests and add to manifest
+        for mm in self.task_manifests:
+            self.manifest_dict["targets"].update(mm.manifest_dict["targets"])
+            self.manifest_dict["tasks"].extend(mm.manifest_dict["tasks"])
+            self.manifest_dict["refs"].update(mm.manifest_dict["refs"])
 
     def add_prism_project(self, prism_project_data: str):
         self.manifest_dict["prism_project"] = prism_project_data
 
-    def add_module(self, module_name: Path, module_data: str):
-        obj = {
-            "module_name": str(module_name),
-            "module_data": module_data
-        }
-        self.manifest_dict["modules"].append(obj)
-
-    def add_ref(self, target: Path, source: Path):
-        obj = {
-            "target": str(target),
-            "source": str(source)
-        }
-        self.manifest_dict["refs"].append(obj)
-
-    def add_target(self, module_name: Path, loc: Union[str, List[str]]):
-        obj = {
-            "module_name": str(module_name),
-            "target_locs": loc
-        }
-        self.manifest_dict["targets"].append(obj)
-
     def json_dump(self, path: Path):
         with open(path / 'manifest.json', 'w') as f:
             json.dump(self.manifest_dict, f, sort_keys=False)
         f.close()
 
     def json_load(self, path: Path):
         with open(path / 'manifest.json', 'r') as f:
```

### Comparing `prism-ds-0.2.0rc1/prism/infra/pipeline.py` & `prism-ds-0.2.0rc2/prism/infra/pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Prism Module class
+Prism Task class
 
 Table of Contents
 - Imports
 - Class definition
 """
 
 ###########
@@ -63,15 +63,18 @@
         if 'pyspark' in adapter_types:
             if self.project.which == 'run':
                 raise prism.exceptions.RuntimeException(
                     message='`pyspark` adapter found in profile YML, use `spark-submit` command'  # noqa; E501
                 )
 
         # Create task_manager and hooks objects
-        task_manager_obj = task_manager.PrismTaskManager(upstream={})
+        task_manager_obj = task_manager.PrismTaskManager(
+            upstream={},
+            parsed_tasks=executor.compiled_dag.parsed_tasks
+        )
         hooks_obj = hooks.PrismHooks(self.project)
 
         # If PySpark adapter is specified in the profile, then explicitly add
         # SparkSession to hooks
         if 'pyspark' in adapter_types:
             for atype, aobj in zip(adapter_types, adapter_objs):
                 if atype == "pyspark":
```

### Comparing `prism-ds-0.2.0rc1/prism/infra/project.py` & `prism-ds-0.2.0rc2/prism/infra/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     ):
         """
         Execute project
         """
         os.chdir(self.project_dir)
 
         # By importing the prism_project, we take advantage of Python's import
-        # caching. That is, if we execute a module that imports prism_project,
+        # caching. That is, if we execute a task that imports prism_project,
         # Python will see that prism_project has already been imported and will not
         # re-import it and overwrite the user context.
         run_context = sys_path_engine.add_sys_path(self.project_dir, run_context)
         exec(f"import {self.filename.replace('.py', '')}", run_context)
 
         # Update internal vars
         for user_k, user_v in self.user_context.items():
@@ -101,15 +101,16 @@
         Set up prism project. This should always be directly after object instantiation
         (except for in testing).
         """
         self.run_context = prism.constants.CONTEXT.copy()
 
         # Create sys.path engine
         self.sys_path_engine = SysPathEngine(
-            self.run_context
+            self.run_context,
+            self.project_dir,
         )
 
         # Execute
         self.exec(self.run_context, self.sys_path_engine)
 
         # ------------------------------------------------------------------------------
         # Admin
@@ -484,13 +485,13 @@
             "on_success": success_triggers,
             "on_failure": failure_triggers,
         }
 
     def cleanup(self, run_context: Dict[Any, Any]):
         """
         Thin wrapper around SysPathEngine's `revert_to_base_sys_path` function. This
-        removes all project modules from sys.path
+        removes all project tasks from sys.path
         """
         return self.sys_path_engine.revert_to_base_sys_path(
             self.sys_path_config,
             run_context
         )
```

### Comparing `prism-ds-0.2.0rc1/prism/infra/sys_path.py` & `prism-ds-0.2.0rc2/prism/infra/sys_path.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,25 +24,19 @@
 
 class SysPathEngine(SysHandlerMixin):
     """
     Class for modifying the project's sys.path
     """
 
     def __init__(self,
-        run_context: Dict[Any, Any]
+        run_context: Dict[Any, Any],
+        project_dir: Path,
     ):
-        self.run_context = run_context
-
-        # Define base sys path and base sys modules
-        temp_context: Dict[Any, Any] = {}
-        exec('import sys', temp_context)
-        self.base_sys_path = [p for p in temp_context['sys'].path]
-        self.base_sys_modules = {
-            k: v for k, v in temp_context['sys'].modules.items()
-        }
+        self.run_context = self.import_sys(run_context)
+        self.project_dir = project_dir
 
     def modify_sys_path(self, sys_path_config):
         """
         Modify the sys.path values for this project
         """
         # Configure sys.path
         self.add_paths_to_sys_path(
@@ -51,18 +45,18 @@
         )
 
         # Return run context
         return self.run_context
 
     def revert_to_base_sys_path(self, sys_path_config, run_context: Dict[Any, Any]):
         """
-        Remove project dir and all associated modules from sys path
+        Remove project dir and all associated tasks from sys path
         """
-        run_context = self.remove_project_modules(
+        run_context = self.remove_project_tasks(
             sys_path_config, run_context
         )
         self.run_context = self.remove_paths_from_sys_path(
-            self.base_sys_path, sys_path_config, run_context
+            sys_path_config, run_context
         )
 
         # Return run context
         return self.run_context
```

### Comparing `prism-ds-0.2.0rc1/prism/infra/task_manager.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,33 @@
-"""
-PrismTaskManager class
-
-Table of Contents
-- Imports
-- Class definition
-"""
-
 ###########
 # Imports #
 ###########
 
-# Standard library imports
-import re
-from typing import Any, Dict
+# Prism infrastructure imports
+import prism.task
+import prism.target
+import prism.decorators
 
 
 ####################
 # Class definition #
 ####################
 
-class PrismTaskManager:
-    """
-    PrismTaskManager class. This class manages all tasks in the DAG (and their
-    associated outputs). An instance of the task manager is passed to all `run`
-    functions (via the kw `tasks`), and users can reference the output of other tasks
-    via `tasks.ref('...')`.
-    """
-
-    def __init__(self, upstream: Dict[str, Any]):
-        self.upstream = upstream
-
-    def ref(self, module: str):
-        if len(re.findall(r'\.py$', module)) == 0:
-            module = f'{module}.py'
-        return self.upstream[module].get_output()
+class Task03(prism.task.PrismTask):
+
+    # Run
+    def run(self, tasks, hooks):
+        """
+        Execute task.
+
+        args:
+            tasks: used to reference output of other tasks --> tasks.ref('...')
+            hooks: built-in Prism hooks. These include:
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
+        returns:
+            task output
+        """
+        with open(tasks.ref('extract/module02.py')) as f:
+            lines = f.read()
+        return lines + '\n' + 'Hello from task 3!'
```

### Comparing `prism-ds-0.2.0rc1/prism/main.py` & `prism-ds-0.2.0rc2/prism/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -59,45 +59,37 @@
     _ = json.loads(inputted_context)
     if len(inputted_vars) > 0 and inputted_context != '{}':
         raise prism.exceptions.ArgumentException(
             message="`vars` and `context` are mutually exclusive arguments"
         )
 
 
-def _process_modules(inputted_modules) -> Optional[List[Any]]:
-    processed_modules = []
-    for m in list(inputted_modules):
+def _process_tasks(inputted_tasks) -> Optional[List[Any]]:
+    processed_tasks = []
+    for m in list(inputted_tasks):
         processed = m
 
-        # If the user adds modules/ at the beginning of their modules (for auto-fill
+        # If the user adds tasks/ at the beginning of their tasks (for auto-fill
         # purposes), then just remove that prefix.
-        if len(re.findall(r'^modules\/', processed)) > 0:
+        if len(re.findall(r'^tasks\/', processed)) > 0:
             click.echo(
-                f"{RED}ArgumentError: remove `modules/` from your --module argument `{m}`{RESET}"  # noqa: E501
+                f"{RED}ArgumentError: remove `tasks/` from your --task argument `{m}`{RESET}"  # noqa: E501
             )
             sys.exit(1)
 
-        # If the user wants to run a specific module and puts .py at the end, fire a
+        # If the user wants to run a specific task and puts .py at the end, fire a
         # warning.
         if len(re.findall(r'\.py$', processed)) > 0:
             click.echo(
-                f'{YELLOW}ArgumentWarning: `.py` in --module arguments will be an error in a future version of Prism.{RESET}'  # noqa: E501
+                f'{YELLOW}ArgumentWarning: `.py` in --task arguments will be an error in a future version of Prism.{RESET}'  # noqa: E501
             )
+        processed_tasks.append(processed)
 
-        # If the user wants to run a specific module but doesn't put .py at the end,
-        # then add it in.
-        if (
-            len(re.findall(r'\.py$', processed)) == 0
-            and len(re.findall(r'\/\*$', processed)) == 0  # noqa: W503
-        ):
-            processed = f'{processed}.py'
-        processed_modules.append(processed)
-
-    if len(processed_modules) > 0:
-        return processed_modules
+    if len(processed_tasks) > 0:
+        return processed_tasks
     return None
 
 
 ##############
 # Arg parser #
 ##############
 
@@ -137,15 +129,15 @@
     type=str,
     help="""Project name""",
     required=False
 )
 @click.option(
     "--minimal",
     is_flag=True,
-    help="""Create minimal project (just `prism_project.py` and `modules`)""",
+    help="""Create minimal project (just `prism_project.py` and `tasks`)""",
     default=False,
     required=False
 )
 @click.option(
     '--log-level', '-l',
     type=click.Choice(['info', 'warn', 'error', 'debug']),
     default="info",
@@ -266,30 +258,30 @@
     task = prism.cli.connect.ConnectTask(ns)
     result = task.run()
     return result
 
 
 @cli.command()
 @click.option(
-    '--module', '-m',
+    '--task', '-t',
     type=str,
-    help="Modules to execute. You can specify multiple modules with as follows: `-m <your_first_module> -m <your_second_module>`.",  # noqa: E501
+    help="Tasks to execute. You can specify multiple tasks with as follows: `-t <your_first_task> -t <your_second_task>`.",  # noqa: E501
     multiple=True,
     default=[]
 )
 @click.option(
     '--all-downstream',
     is_flag=True,
-    help="Execute all tasks downstream of modules specified with `--module`"
+    help="Execute all tasks downstream of tasks specified with `--task`"
 )
 @click.option(
     '--all-upstream',
     is_flag=True,
     type=bool,
-    help="Execute all tasks upstream of modules specified with `--module`"
+    help="Execute all tasks upstream of tasks specified with `--task`"
 )
 @click.option(
     '--log-level', '-l',
     type=click.Choice(['info', 'warn', 'error', 'debug']),
     default="info",
     help="""Set the log level""",
     required=False
@@ -308,41 +300,41 @@
 @click.option(
     '--context',
     type=str,
     help="Context as a dictionary. Must be a valid JSON. These overwrite variables in prism_project.py",  # noqa: E501
     default='{}'
 )
 def run(
-    module,
+    task,
     all_downstream,
     all_upstream,
     log_level,
     full_tb,
     vars,
     context
 ):
     """Execute your Prism project.
 
     <br>Examples:
     - prism run
-    - prism run -m module01.py -m module02.py
-    - prism run -m module01 --all-downstream
+    - prism run -t task01.py -t task02.py
+    - prism run -t task01 --all-downstream
     - prism run -v VAR1=VALUE1 -v VAR2=VALUE2
     - prism run --context '{"hi": 1}'
     """
-    # Convert tuple of modules to list
-    modules_list: Optional[List[Any]] = _process_modules(module)
+    # Convert tuple of tasks to list
+    tasks_list: Optional[List[Any]] = _process_tasks(task)
 
     # Check `vars` and `context`
     vars_dict = _check_vars_format(vars)
     _check_context(vars, context)
 
     # Namespace
     ns = argparse.Namespace()
-    ns.modules = modules_list
+    ns.tasks = tasks_list
     ns.all_upstream = all_upstream
     ns.all_downstream = all_downstream
     ns.full_tb = full_tb
     ns.log_level = log_level
     ns.vars = vars_dict
     ns.context = context
     ns.which = 'run'
@@ -445,25 +437,25 @@
     type=str,
     required=False,
     default="new_task",
     help="""
     Task name. If only a single task is requested, then the task will be named
     `<task_name>.py`. If multiple tasks are requested, then the tasks will be named
     `<task_name>_<number>.py`. Tasks should have short, all-lowercase names. Underscores
-    can be used in the module name if it improves readability.
+    can be used in the task name if it improves readability.
     """
 )
 @click.option(
     '--dir',
     type=str,
     required=False,
     default="",
     help="""
-    Folder within the `modules` directory in which the new tasks should live. If not
-        specified, then new tasks will be dumpted into `modules/`
+    Folder within the `tasks` directory in which the new tasks should live. If not
+        specified, then new tasks will be dumpted into `tasks/`
     """
 )
 @click.option(
     '--log-level', '-l',
     type=click.Choice(['info', 'warn', 'error', 'debug']),
     default="info",
     help="""Set the log level""",
@@ -707,30 +699,30 @@
 @click.option(
     "--file", "-f",
     required=True,
     type=str,
     help="Path to agent configuration YML"
 )
 @click.option(
-    '--module', '-m',
+    '--task', '-t',
     type=str,
-    help="Modules to execute. You can specify multiple modules with as follows: `-m <your_first_module> -m <your_second_module>`.",  # noqa: E501
+    help="Tasks to execute. You can specify multiple tasks with as follows: `-t <your_first_task> -t <your_second_task>`.",  # noqa: E501
     multiple=True,
     default=[]
 )
 @click.option(
     '--all-downstream',
     is_flag=True,
-    help="Execute all tasks downstream of modules specified with `--module`"
+    help="Execute all tasks downstream of tasks specified with `--task`"
 )
 @click.option(
     '--all-upstream',
     is_flag=True,
     type=bool,
-    help="Execute all tasks upstream of modules specified with `--module`"
+    help="Execute all tasks upstream of tasks specified with `--task`"
 )
 @click.option(
     '--log-level', '-l',
     type=click.Choice(['info', 'warn', 'error', 'debug']),
     default="info",
     help="""Set the log level""",
     required=False
@@ -750,43 +742,43 @@
     '--context',
     type=str,
     help="Context as a dictionary. Must be a valid JSON. These overwrite variables in prism_project.py",  # noqa: E501
     default='{}'
 )
 def agent_run(
     file,
-    module,
+    task,
     all_downstream,
     all_upstream,
     log_level,
     full_tb,
     vars,
     context
 ):
     """Run your project using an agent.
 
     <br>Examples:
-    - prism agent run -f ./ec2.yml --module module01.py --module module02.py
-    - prism agent run -f ./docker.yml --m module01
+    - prism agent run -f ./ec2.yml --task task01.py --task task02.py
+    - prism agent run -f ./docker.yml --t task01
     - prism agent run -f /Users/docker.yml --vars VAR1=VALUE1
     """
     # Namespace
     ns = argparse.Namespace()
 
-    # Convert tuple of modules to list
-    modules_list: Optional[List[Any]] = _process_modules(module)
+    # Convert tuple of tasks to list
+    tasks_list: Optional[List[Any]] = _process_tasks(task)
 
     # Check `vars` and `context`
     vars_dict = _check_vars_format(vars)
     _check_context(vars, context)
 
     # Namespace
     ns = argparse.Namespace()
     ns.file = file
-    ns.modules = modules_list
+    ns.tasks = tasks_list
     ns.all_upstream = all_upstream
     ns.all_downstream = all_downstream
     ns.full_tb = full_tb
     ns.log_level = log_level
     ns.vars = vars_dict
     ns.context = context
     ns.which = 'agent-run'
@@ -801,30 +793,30 @@
 @click.option(
     "--file", "-f",
     required=True,
     type=str,
     help="Path to agent configuration YML"
 )
 @click.option(
-    '--module', '-m',
+    '--task', '-t',
     type=str,
-    help="Modules to execute. You can specify multiple modules with as follows: `-m <your_first_module> -m <your_second_module>`.",  # noqa: E501
+    help="Tasks to execute. You can specify multiple tasks with as follows: `-t <your_first_task> -t <your_second_task>`.",  # noqa: E501
     multiple=True,
     default=[]
 )
 @click.option(
     '--all-downstream',
     is_flag=True,
-    help="Execute all tasks downstream of modules specified with `--module`"
+    help="Execute all tasks downstream of tasks specified with `--task`"
 )
 @click.option(
     '--all-upstream',
     is_flag=True,
     type=bool,
-    help="Execute all tasks upstream of modules specified with `--module`"
+    help="Execute all tasks upstream of tasks specified with `--task`"
 )
 @click.option(
     '--log-level', '-l',
     type=click.Choice(['info', 'warn', 'error', 'debug']),
     default="info",
     help="""Set the log level""",
     required=False
@@ -844,15 +836,15 @@
     '--context',
     type=str,
     help="Context as a dictionary. Must be a valid JSON. These overwrite variables in prism_project.py",  # noqa: E501
     default='{}'
 )
 def agent_build(
     file,
-    module,
+    task,
     all_downstream,
     all_upstream,
     log_level,
     full_tb,
     vars,
     context
 ):
@@ -862,25 +854,25 @@
     <br>Examples:
     - prism agent build -f ./ec2.yml
     - prism agent build -f /Users/docker.yml --context '{"HI": 1}'
     """
     # Namespace
     ns = argparse.Namespace()
 
-    # Convert tuple of modules to list
-    modules_list: Optional[List[Any]] = _process_modules(module)
+    # Convert tuple of tasks to list
+    tasks_list: Optional[List[Any]] = _process_tasks(task)
 
     # Check `vars` and `context`
     vars_dict = _check_vars_format(vars)
     _check_context(vars, context)
 
     # Namespace
     ns = argparse.Namespace()
     ns.file = file
-    ns.modules = modules_list
+    ns.tasks = tasks_list
     ns.all_upstream = all_upstream
     ns.all_downstream = all_downstream
     ns.full_tb = full_tb
     ns.log_level = log_level
     ns.vars = vars_dict
     ns.context = context
     ns.which = 'agent-build'
@@ -937,30 +929,30 @@
     task = prism.cli.agent.AgentTask(ns)
     result = task.run()
     return result
 
 
 @cli.command('spark-submit')
 @click.option(
-    '--module', '-m',
+    '--task', '-t',
     type=str,
-    help="Modules to execute. You can specify multiple modules with as follows: `-m <your_first_module> -m <your_second_module>`.",  # noqa: E501
+    help="Tasks to execute. You can specify multiple tasks with as follows: `-t <your_first_task> -t <your_second_task>`.",  # noqa: E501
     multiple=True,
     default=[]
 )
 @click.option(
     '--all-downstream',
     is_flag=True,
-    help="Execute all tasks downstream of modules specified with `--module`."
+    help="Execute all tasks downstream of tasks specified with `--task`."
 )
 @click.option(
     '--all-upstream',
     is_flag=True,
     type=bool,
-    help="Execute all tasks upstream of modules specified with `--module`."
+    help="Execute all tasks upstream of tasks specified with `--task`."
 )
 @click.option(
     '--log-level', '-l',
     type=click.Choice(['info', 'warn', 'error', 'debug']),
     default="info",
     help="""Set the log level.""",
     required=False
@@ -979,41 +971,41 @@
 @click.option(
     '--context',
     type=str,
     help="Context as a dictionary. Must be a valid JSON. These overwrite variables in prism_project.py.",  # noqa: E501
     default='{}'
 )
 def spark_submit(
-    module,
+    task,
     all_downstream,
     all_upstream,
     log_level,
     full_tb,
     vars,
     context
 ):
     """Execute your Prism project as a PySpark job.
 
     <br>Examples:
     - prism spark-submit
-    - prism spark-submit -m module01.py -m module02.py
-    - prism spark-submit -m module01 --all-downstream
+    - prism spark-submit -t task01.py -t task02.py
+    - prism spark-submit -t task01 --all-downstream
     - prism spark-submit -v VAR1=VALUE1 -v VAR2=VALUE2
     - prism spark-submit --context '{"hi": 1}'
     """
-    # Convert tuple of modules to list
-    modules_list: Optional[List[Any]] = _process_modules(module)
+    # Convert tuple of tasks to list
+    tasks_list: Optional[List[Any]] = _process_tasks(task)
 
     # Check `vars` and `context`
     vars_dict = _check_vars_format(vars)
     _check_context(vars, context)
 
     # Namespace
     ns = argparse.Namespace()
-    ns.modules = modules_list
+    ns.tasks = tasks_list
     ns.all_upstream = all_upstream
     ns.all_downstream = all_downstream
     ns.full_tb = full_tb
     ns.log_level = log_level
     ns.vars = vars_dict
     ns.context = context
     ns.which = 'spark-submit'
```

### Comparing `prism-ds-0.2.0rc1/prism/mixins/agent.py` & `prism-ds-0.2.0rc2/prism/mixins/agent.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/mixins/aws.py` & `prism-ds-0.2.0rc2/prism/mixins/aws.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/mixins/base.py` & `prism-ds-0.2.0rc2/prism/mixins/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,18 +35,20 @@
         filename: str = 'prism_project.py'
     ) -> prism_project.PrismProject:
         """
         Wrapper for creation of PrismPipeline object. Needed in order to be compatible
         with event manager.
 
         args:
-            code: str or code object to run
-            globals_dict: globals dictionary
+            project_dir: project directory
+            user_context: user-defined context to override prism_project.py
+            which: task that requires Prism project
+            filename: filename of prism_project.py. Default is `prism_project.py`.
         returns:
-            PrismPipeline object
+            PrismProject object
         """
         project = prism_project.PrismProject(
             project_dir=project_dir,
             user_context=user_context,
             which=which,
             filename=filename
         )
```

### Comparing `prism-ds-0.2.0rc1/prism/mixins/connect.py` & `prism-ds-0.2.0rc2/prism/mixins/connect.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/mixins/create_agent.py` & `prism-ds-0.2.0rc2/prism/mixins/create_agent.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/mixins/create_task.py` & `prism-ds-0.2.0rc2/prism/mixins/create_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,23 +80,23 @@
 
                 # Remove "_"
                 class_name = name_proper_case.replace("_", "")
                 return class_name
             else:
                 return user_task_name
 
-    def create_task_module(self,
+    def create_task_task(self,
         task_type: str,
         task_template: Template,
         args: Dict[str, str],
         user_task_name: str,
         task_dir: Path,
     ) -> Path:
         f"""
-        Create the standalone module associated with the new task
+        Create the standalone task associated with the new task
 
         args:
             task_type: one of {','.join(prism.constants.VALID_TASK_TYPES)}
             task_template: task Jinja2 template
             args: arguments to populate template
             user_task_name: user-inputted task name argument. This will be the task's
                             filename
@@ -153,15 +153,15 @@
         # Only one task is requested
         if task_number == 1:
             template_args = {
                 "task_name": self.process_user_task_name(
                     task_type, user_task_name, decorated
                 )
             }
-            self.create_task_module(
+            self.create_task_task(
                 task_type,
                 task_template,
                 template_args,
                 user_task_name,
                 task_dir
             )
 
@@ -175,15 +175,15 @@
                 )
                 cls_name += str(i)
                 template_args = {
                     "task_name": cls_name
                 }
                 new_user_task_name = user_task_name + f"_{i}"
 
-                # Create task modules
-                self.create_task_module(
+                # Create task tasks
+                self.create_task_task(
                     task_type,
                     task_template,
                     template_args,
                     new_user_task_name,
                     task_dir
                 )
```

### Comparing `prism-ds-0.2.0rc1/prism/mixins/create_trigger.py` & `prism-ds-0.2.0rc2/prism/mixins/create_trigger.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/mixins/graph.py` & `prism-ds-0.2.0rc2/prism/mixins/graph.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/mixins/run.py` & `prism-ds-0.2.0rc2/prism/mixins/run.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/parsers/base.py` & `prism-ds-0.2.0rc2/prism/parsers/base.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/parsers/yml_parser.py` & `prism-ds-0.2.0rc2/prism/parsers/yml_parser.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/prism_logging.py` & `prism-ds-0.2.0rc2/prism/prism_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 
 ###########
 # Imports #
 ###########
 
 # General package imports
+from io import StringIO
 import argparse
 import re
 import os
 import copy
 import math
 import logging
 import time
@@ -126,34 +127,34 @@
 # Agent level num
 AGENT_LEVEL = logging.INFO + 5
 
 
 # Add logging level
 def add_logging_level(level_name, level_num, method_name=None):
     """
-    Comprehensively adds a new logging level to the `logging` module and the
+    Comprehensively adds a new logging level to the `logging` task and the
     currently configured logging class. Inspired heavily by the answer here:
     https://stackoverflow.com/a/35804945/1691778
 
     args:
         level_name: desired level name
         level_num: number associated with level
         method_name: method name used to invoke log level. If not specified,
                      `level_name.lower()` is used.
     return:
-        `level_name` becomes an attribute of the `logging` module with the value
+        `level_name` becomes an attribute of the `logging` task with the value
         `level_num`
     """
     if not method_name:
         method_name = level_name.lower()
 
     if hasattr(logging, level_name):
-        raise AttributeError('{} already defined in logging module'.format(level_name))
+        raise AttributeError('{} already defined in logging task'.format(level_name))
     if hasattr(logging, method_name):
-        raise AttributeError('{} already defined in logging module'.format(method_name))
+        raise AttributeError('{} already defined in logging task'.format(method_name))
     if hasattr(logging.getLoggerClass(), method_name):
         raise AttributeError('{} already defined in logger class'.format(method_name))
 
     # This method was inspired by the answers to Stack Overflow post
     # http://stackoverflow.com/q/2183233/2988730, especially
     # http://stackoverflow.com/a/13638084/2988730
     def logForLevel(self, message, *args, **kwargs):
@@ -197,16 +198,26 @@
         # Otherwise, adjust the formatting based on the level
         else:
             log_fmt = self.FORMATS.get(record.levelno)
             formatter = logging.Formatter(log_fmt, "%H:%M:%S")
             return formatter.format(record)
 
 
+class FileHandlerFormatter(FormatterWithAnsi):
+    def format(self, record):
+        return escape_ansi(super().format(record))
+
+
 DEFAULT_LOGGER: logging.Logger
 
+# String handler
+string_streamer = StringIO()
+string_stream_handler = logging.StreamHandler(stream=string_streamer)
+string_stream_handler.setFormatter(FileHandlerFormatter())
+
 
 def set_up_logger(args: argparse.Namespace):
     if globals().get('DEFAULT_LOGGER', None) is None:
         global DEFAULT_LOGGER
 
         DEFAULT_LOGGER = logging.getLogger('PRISM_LOGGER')
 
@@ -228,26 +239,23 @@
 
         # Stream handler
         handler = logging.StreamHandler()
         handler = _set_level(handler, args.log_level)
         handler.setFormatter(FormatterWithAnsi())
 
         # File handler -- remove ANSI codes
-        class FileHandlerFormatter(FormatterWithAnsi):
-            def format(self, record):
-                return escape_ansi(super().format(record))
-
         file_handler = logging.FileHandler('logs.log')
         file_handler = _set_level(file_handler, args.log_level)
         file_handler.setLevel(logging.INFO)
         file_handler.setFormatter(FileHandlerFormatter())
 
         # Add handlers
         DEFAULT_LOGGER.addHandler(file_handler)
         DEFAULT_LOGGER.addHandler(handler)
+        DEFAULT_LOGGER.addHandler(string_stream_handler)
 
 
 #################
 # Event classes #
 #################
 
 class Event:
@@ -393,19 +401,26 @@
 class EmptyLineEvent(Event):
 
     def message(self):
         return ' '
 
 
 @dataclass
-class ModulesFolderNotFoundEvent(Event):
+class TasksFolderNotFoundEvent(Event):
     path: str
 
     def message(self):
-        return f'{RED}`modules` subfolder not found in {self.path}{RESET}'
+        return f'{RED}`tasks` subfolder not found in {self.path}{RESET}'
+
+
+@dataclass
+class ModulesFolderDeprecated(Event):
+
+    def message(self):
+        return f'{YELLOW}`modules` should be renamed to `tasks`...this will be an error in a future version of Prism{RESET}'  # noqa: E501
 
 
 @dataclass
 class SeparatorEvent(Event):
 
     def message(self):
         try:
@@ -575,18 +590,18 @@
 
     def message(self):
         return f'{YELLOW}`THREADS` not found in prism_project.py; defaulting to 1{RESET}'  # noqa: E501
 
 
 @dataclass
 class PyWarningEvent(Event):
-    module_name: str
+    task_name: str
 
     def message(self):
-        return f'{YELLOW}Found `.py` in a tasks.ref(...) argument in `{self.module_name}`...This will be an error in a future version of Prism.{RESET}'  # noqa: E501
+        return f'{YELLOW}Found `.py` in a tasks.ref(...) argument in `{self.task_name}`...This will be an error in a future version of Prism.{RESET}'  # noqa: E501
 
 
 @dataclass
 class DelayEvent(Event):
     name: str
     delay_seconds: int
```

### Comparing `prism-ds-0.2.0rc1/prism/profiles/adapter.py` & `prism-ds-0.2.0rc2/prism/profiles/adapter.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/profiles/bigquery.py` & `prism-ds-0.2.0rc2/prism/profiles/bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,10 +105,15 @@
         ctx = bigquery.Client(credentials=credentials)
         return ctx
 
     def execute_sql(self, query: str, return_type: str) -> pd.DataFrame:
         """
         Execute the SQL query
         """
-        df = self.engine.query(query).to_dataframe()
+        data = self.engine.query(query)
         if return_type == "pandas":
+            df = data.to_dataframe()
             return df
+        res = []
+        for row in data.result():
+            res.append(row)
+        return res
```

### Comparing `prism-ds-0.2.0rc1/prism/profiles/dbt.py` & `prism-ds-0.2.0rc2/prism/profiles/dbt.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     use_colors: Optional[bool]
 
 
 @dataclass
 class InitializeDbtCompileTaskArgs:
     selector_name: Optional[str]
     select: List[str]
-    models: List[str]
+    tasks: List[str]
     exclude: Tuple[str, str]
     state: Optional[Path]
     single_threaded: Optional[bool]
 
 
 ####################
 # Class definition #
@@ -203,15 +203,15 @@
         )
         return RuntimeConfig.from_args(args)
 
     def initialize_dbt_flags(self,
         profiles_dir: str
     ):
         """
-        Initializes the flags module from dbt. This module ensures that the dbt compile
+        Initializes the flags task from dbt. This task ensures that the dbt compile
         task does not throw an error.
 
         args:
             profiles_dir: dbt profiles directory
         """
         args = InitializeFlagsArgs(profiles_dir, None)
         user_config = read_user_config(profiles_dir)
@@ -226,15 +226,15 @@
     def initialize_compile_task(self,
         profiles_dir: str,
         dbt_config: RuntimeConfig,
         manifest,
     ):
         """
         Initialize the compile task and call _runtime_initialize(). This must be done
-        after the flags module has been initialized.
+        after the flags task has been initialized.
 
         args:
             profiles_dir: directory of dbt profiles
         """
         # Initialize tracking
         dbt.tracking.initialize_from_flags(True, profiles_dir)
 
@@ -275,77 +275,77 @@
             dbt SQLAdapter
         """
         dbt.adapters.factory.reset_adapters()
         dbt.adapters.factory.register_adapter(dbt_config)
         adapter: SQLAdapter = adapters_factory.get_adapter(dbt_config)
         return adapter
 
-    def get_parsed_model_node(self,
+    def get_parsed_task_node(self,
         target_model_name: str,
         target_model_package: Optional[str],
         target_model_version: Optional[str],
         project_dir: str,
         manifest: Manifest
     ) -> ResultNode:
         """
-        Get the node associated with the inputted target model
+        Get the node associated with the inputted target task
 
         args:
-            target_model_name: name of model to retrieve from manifest
-            target_package_name: package containing model
+            target_model_name: name of task to retrieve from manifest
+            target_package_name: package containing task
             project_dir: project directory
             manifest: dbt Manifest
         returns:
-            node associated with inputted target model
+            node associated with inputted target task
         """
         # Use `resolve_ref` method from manifest class. For simple projects, it should
         # be the case that `node_package` is identical to `project_directory`. There may
         # be more complex projects where this is not the case. We implement the simple
         # version for now.
 
-        # TODO: test target model creation where node_package != project_dir
+        # TODO: test target task creation where node_package != project_dir
         target_model: MaybeNonSource = manifest.resolve_ref(
             target_model_name=target_model_name,
             target_model_package=target_model_package,
             target_model_version=target_model_version,
             current_project=project_dir,
             node_package=project_dir
         )
 
-        # If model isn't found, then throw an error.
+        # If task isn't found, then throw an error.
         package_str = f"'{target_model_package}'." if target_model_package is not None else ""  # noqa: E501
-        model_str = f"{package_str}'{target_model_name}'"
+        task_str = f"{package_str}'{target_model_name}'"
         if target_model is None:
             raise prism.exceptions.RuntimeException(
-                message=f'could not find model dbt model `{model_str}`'
+                message=f'could not find task dbt task `{task_str}`'
             )
 
-        # The model could be disabled
+        # The task could be disabled
         if isinstance(target_model, Disabled):
             raise prism.exceptions.RuntimeException(
-                message=f'dbt model `{model_str}` is disabled'
+                message=f'dbt task `{task_str}` is disabled'
             )
 
         return target_model
 
     def get_target_model_relation(self,
         target: ResultNode,
         adapter: SQLAdapter,
         manifest: Manifest
     ):
         """
-        Get target model relation (i.e., the location of target model in syntax of
+        Get target task relation (i.e., the location of target task in syntax of
         project's SQL engine)
 
         args:
-            target: target model node
+            target: target task node
             adapter: dbt adapter
             manifest: dbt Manifest
         returns:
-            target model relation
+            target task relation
         """
 
         # Create a unique adapter connection and avoid clashes
         name = "relation:" + str(hash(str(target))) + ":" + str(uuid4())
         relation = None
         with adapter.connection_named(name):
             adapter.set_relations_cache(manifest, True)
@@ -413,45 +413,45 @@
 
     def handle_ref(self,
         target_1: str,
         target_2: Optional[str] = None,
         target_version: Optional[str] = None,
     ) -> pd.DataFrame:
         """
-        Download a dbt model into a Pandas DataFrame:
+        Download a dbt task into a Pandas DataFrame:
 
         args:
-            target_1, target_2: dbt model
+            target_1, target_2: dbt task
         returns:
             pandas DataFrame
         """
-        # Convert inputs into package and model name
+        # Convert inputs into package and task name
         target_model_name = target_1
         target_package_name = None
         if target_2 is not None:
             target_package_name = target_1
             target_model_name = target_2
 
-        # Get target model
-        target_model = self.get_parsed_model_node(
+        # Get target task
+        target_model = self.get_parsed_task_node(
             target_model_name,
             target_package_name,
             target_version,
             self.dbt_project_dir,
             self.manifest
         )
 
         # Get relation
         target_model_relation = self.get_target_model_relation(
             target_model,
             self.adapter,
             self.manifest
         )
 
-        # Download model
+        # Download task
         query = f"SELECT * FROM {target_model_relation}"
         response, result = self.execute_sql(self.adapter, query)
         df = self.remote_result_to_pd(result)
         return df
 
     def execute(self, return_type: str = "list"):
         """
```

### Comparing `prism-ds-0.2.0rc1/prism/profiles/meta.py` & `prism-ds-0.2.0rc2/prism/profiles/meta.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/profiles/postgres.py` & `prism-ds-0.2.0rc2/prism/profiles/redshift.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """
-Postgres adapter class definition
+Redshift adapter class definition
 
 Table of Contents
 - Imports
 - Class definition
 """
 
 ###########
 # Imports #
 ###########
 
 # Standard library imports
 import pandas as pd
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 import psycopg2
 
 # Prism-specific imports
 from .adapter import Adapter
 import prism.exceptions
 
 
 ####################
 # Class definition #
 ####################
 
-class Postgres(Adapter):
+class Redshift(Adapter):
 
     def is_valid_config(self,
         config_dict: Dict[str, str],
         adapter_name: str,
         profile_name: str,
     ) -> bool:
         """
         Check that config dictionary is profile YML is valid
 
         args:
-            config_dict: config dictionary under PostgresQL adapter in profile YML
+            config_dict: config dictionary under Redshift adapter in profile YML
             adapter_name: name assigned to adapter
             profile_name: profile name containing adapter
         returns:
             boolean indicating whether config dictionary in profile YML is valid
         """
 
         # Required config vars
@@ -85,23 +85,23 @@
 
     def create_engine(self,
         adapter_dict: Dict[str, Any],
         adapter_name: str,
         profile_name: str
     ):
         """
-        Parse PostgresQL adapter, represented as a dict and return the PostgresQL
-        connector object
+        Parse Redshift adapter, represented as a dict and return the Redshift connector
+        object
 
         args:
-            adapter_dict: PostgresQL adapter represented as a dictionary
+            adapter_dict: Redshift adapter represented as a dictionary
             adapter_name: name assigned to adapter
             profile_name: profile name containing adapter
         returns:
-            PostgresQL connector object
+            Redshift connector object
         """
 
         # Get configuration and check if config is valid
         self.is_valid_config(adapter_dict, adapter_name, profile_name)
 
         # Create psycopg2 connection
         conn = psycopg2.connect(
@@ -116,26 +116,29 @@
         try:
             autocommit_config = bool(adapter_dict['autocommit'])
             conn.set_session(autocommit=autocommit_config)
         except KeyError:
             conn.set_session(autocommit=True)
         return conn
 
-    def execute_sql(self, query: str, return_type: str) -> pd.DataFrame:
+    def execute_sql(self, query: str, return_type: Optional[str]) -> pd.DataFrame:
         """
         Execute the SQL query
         """
         # Create cursor for every SQL query -- this ensures thread safety
         cursor = self.engine.cursor()
         cursor.execute(query)
+        data = cursor.fetchall()
+
+        # If the return type is `pandas`, then return a DataFrame
         if return_type == "pandas":
-            data = cursor.fetchall()
             cols = []
             for elts in cursor.description:
                 cols.append(elts[0])
             df: pd.DataFrame = pd.DataFrame(data=data, columns=cols)
             cursor.close()
             return df
+
+        # Otherwise, return the data as it exists
         else:
-            # Fetch one to ensure that the query was executed
-            cursor.fetchone()
             cursor.close()
+            return data
```

### Comparing `prism-ds-0.2.0rc1/prism/profiles/profile.py` & `prism-ds-0.2.0rc2/prism/profiles/profile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/profiles/pyspark.py` & `prism-ds-0.2.0rc2/prism/profiles/pyspark.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/profiles/redshift.py` & `prism-ds-0.2.0rc2/prism/profiles/snowflake.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,141 +1,133 @@
 """
-Redshift adapter class definition
+Snowflake adapter class definition
 
 Table of Contents
 - Imports
 - Class definition
 """
 
 ###########
 # Imports #
 ###########
 
 # Standard library imports
 import pandas as pd
-from typing import Any, Dict
-import psycopg2
+from typing import Any, Dict, Optional
 
 # Prism-specific imports
 from .adapter import Adapter
 import prism.exceptions
 
 
 ####################
 # Class definition #
 ####################
 
-class Redshift(Adapter):
+class Snowflake(Adapter):
 
     def is_valid_config(self,
         config_dict: Dict[str, str],
         adapter_name: str,
-        profile_name: str,
+        profile_name: str
     ) -> bool:
         """
         Check that config dictionary is profile YML is valid
 
         args:
-            config_dict: config dictionary under Redshift adapter in profile YML
+            config_dict: config dictionary under snowflake adapter in profile YML
             adapter_name: name assigned to adapter
             profile_name: profile name containing adapter
         returns:
             boolean indicating whether config dictionary in profile YML is valid
         """
 
         # Required config vars
         required_config_vars = [
             'type',
             'user',
             'password',
-            'port',
-            'host',
-            'database'
-        ]
-
-        # Optional config vars
-        optional_config_vars = [
-            'autocommit'
+            'account',
+            'role',
+            'warehouse',
+            'database',
+            'schema'
         ]
 
         # Raise an error if:
         #   1. Config doesn't contain any of the required vars or contains additional
         #      config vars
         #   2. Any of the config values are None
         actual_config_vars = []
         for k, v in config_dict.items():
-            if k not in required_config_vars and k not in optional_config_vars:
+            if k not in required_config_vars:
                 raise prism.exceptions.InvalidProfileException(
                     message=f'invalid var `{k}` - see `{adapter_name}` adapter in `{profile_name}` profile in profile YML'  # noqa: E501
                 )
-            if k in required_config_vars:
-                actual_config_vars.append(k)
+            actual_config_vars.append(k)
             if v is None:
                 raise prism.exceptions.InvalidProfileException(
-                    message=f'var `{k}` cannot be None - see `{adapter_name}` adapter in `{profile_name}` profile in profile YML'  # noqa: E501
+                    message=f'`{k}` cannot be None - see `{adapter_name}` adapter in `{profile_name}` profile in profile YML'  # noqa: E501
                 )
         vars_not_defined = list(set(required_config_vars) - set(actual_config_vars))
         if len(vars_not_defined) > 0:
             v = vars_not_defined.pop()
             raise prism.exceptions.InvalidProfileException(
-                message=f'var `{v}` must be defined - see `{adapter_name}` adapter in `{profile_name}` profile in profile YML'  # noqa: E501
+                message=f'`{v}` must be defined - see `{adapter_name}` adapter in `{profile_name}` profile in profile YML'  # noqa: E501
             )
 
         # If no exception has been raised, return True
         return True
 
     def create_engine(self,
         adapter_dict: Dict[str, Any],
         adapter_name: str,
         profile_name: str
     ):
         """
-        Parse Redshift adapter, represented as a dict and return the Redshift connector
-        object
+        Parse Snowflake adapter, represented as a dict and return the Snowflake
+        connector object
 
         args:
-            adapter_dict: Redshift adapter represented as a dictionary
+            adapter_dict: Snowflake adapter represented as a dictionary
             adapter_name: name assigned to adapter
             profile_name: profile name containing adapter
         returns:
-            Redshift connector object
+            Snowflake connector object
         """
+        # Import snowflake connector
+        import snowflake.connector
 
         # Get configuration and check if config is valid
         self.is_valid_config(adapter_dict, adapter_name, profile_name)
 
-        # Create psycopg2 connection
-        conn = psycopg2.connect(
-            dbname=adapter_dict['database'],
-            host=adapter_dict['host'],
-            port=adapter_dict['port'],
+        # Connection
+        ctx = snowflake.connector.connect(
+            account=adapter_dict['account'],
             user=adapter_dict['user'],
-            password=adapter_dict['password']
+            password=adapter_dict['password'],
+            database=adapter_dict['database'],
+            schema=adapter_dict['schema'],
+            warehouse=adapter_dict['warehouse'],
+            role=adapter_dict['role']
         )
+        return ctx
 
-        # Autocommit. If no autocommit is specified, then set to True
-        try:
-            autocommit_config = bool(adapter_dict['autocommit'])
-            conn.set_session(autocommit=autocommit_config)
-        except KeyError:
-            conn.set_session(autocommit=True)
-        return conn
-
-    def execute_sql(self, query: str, return_type: str) -> pd.DataFrame:
+    def execute_sql(self, query: str, return_type: Optional[str]) -> pd.DataFrame:
         """
         Execute the SQL query
         """
         # Create cursor for every SQL query -- this ensures thread safety
         cursor = self.engine.cursor()
         cursor.execute(query)
+
+        # If the return type is `pandas`, then return a DataFrame
         if return_type == "pandas":
-            data = cursor.fetchall()
-            cols = []
-            for elts in cursor.description:
-                cols.append(elts[0])
-            df: pd.DataFrame = pd.DataFrame(data=data, columns=cols)
+            df: pd.DataFrame = cursor.fetch_pandas_all()
             cursor.close()
             return df
+
+        # Otherwise, just return the data
         else:
-            # Fetch one to ensure that the query was executed
-            cursor.fetchone()
+            data = cursor.fetchall()
             cursor.close()
+            return data
```

### Comparing `prism-ds-0.2.0rc1/prism/profiles/snowflake.py` & `prism-ds-0.2.0rc2/prism/profiles/postgres.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,129 +1,144 @@
 """
-Snowflake adapter class definition
+Postgres adapter class definition
 
 Table of Contents
 - Imports
 - Class definition
 """
 
 ###########
 # Imports #
 ###########
 
 # Standard library imports
 import pandas as pd
-from typing import Any, Dict
+from typing import Any, Dict, Optional
+import psycopg2
 
 # Prism-specific imports
 from .adapter import Adapter
 import prism.exceptions
 
 
 ####################
 # Class definition #
 ####################
 
-class Snowflake(Adapter):
+class Postgres(Adapter):
 
     def is_valid_config(self,
         config_dict: Dict[str, str],
         adapter_name: str,
-        profile_name: str
+        profile_name: str,
     ) -> bool:
         """
         Check that config dictionary is profile YML is valid
 
         args:
-            config_dict: config dictionary under snowflake adapter in profile YML
+            config_dict: config dictionary under PostgresQL adapter in profile YML
             adapter_name: name assigned to adapter
             profile_name: profile name containing adapter
         returns:
             boolean indicating whether config dictionary in profile YML is valid
         """
 
         # Required config vars
         required_config_vars = [
             'type',
             'user',
             'password',
-            'account',
-            'role',
-            'warehouse',
-            'database',
-            'schema'
+            'port',
+            'host',
+            'database'
+        ]
+
+        # Optional config vars
+        optional_config_vars = [
+            'autocommit'
         ]
 
         # Raise an error if:
         #   1. Config doesn't contain any of the required vars or contains additional
         #      config vars
         #   2. Any of the config values are None
         actual_config_vars = []
         for k, v in config_dict.items():
-            if k not in required_config_vars:
+            if k not in required_config_vars and k not in optional_config_vars:
                 raise prism.exceptions.InvalidProfileException(
                     message=f'invalid var `{k}` - see `{adapter_name}` adapter in `{profile_name}` profile in profile YML'  # noqa: E501
                 )
-            actual_config_vars.append(k)
+            if k in required_config_vars:
+                actual_config_vars.append(k)
             if v is None:
                 raise prism.exceptions.InvalidProfileException(
-                    message=f'`{k}` cannot be None - see `{adapter_name}` adapter in `{profile_name}` profile in profile YML'  # noqa: E501
+                    message=f'var `{k}` cannot be None - see `{adapter_name}` adapter in `{profile_name}` profile in profile YML'  # noqa: E501
                 )
         vars_not_defined = list(set(required_config_vars) - set(actual_config_vars))
         if len(vars_not_defined) > 0:
             v = vars_not_defined.pop()
             raise prism.exceptions.InvalidProfileException(
-                message=f'`{v}` must be defined - see `{adapter_name}` adapter in `{profile_name}` profile in profile YML'  # noqa: E501
+                message=f'var `{v}` must be defined - see `{adapter_name}` adapter in `{profile_name}` profile in profile YML'  # noqa: E501
             )
 
         # If no exception has been raised, return True
         return True
 
     def create_engine(self,
         adapter_dict: Dict[str, Any],
         adapter_name: str,
         profile_name: str
     ):
         """
-        Parse Snowflake adapter, represented as a dict and return the Snowflake
+        Parse PostgresQL adapter, represented as a dict and return the PostgresQL
         connector object
 
         args:
-            adapter_dict: Snowflake adapter represented as a dictionary
+            adapter_dict: PostgresQL adapter represented as a dictionary
             adapter_name: name assigned to adapter
             profile_name: profile name containing adapter
         returns:
-            Snowflake connector object
+            PostgresQL connector object
         """
-        # Import snowflake connector
-        import snowflake.connector
 
         # Get configuration and check if config is valid
         self.is_valid_config(adapter_dict, adapter_name, profile_name)
 
-        # Connection
-        ctx = snowflake.connector.connect(
-            account=adapter_dict['account'],
+        # Create psycopg2 connection
+        conn = psycopg2.connect(
+            dbname=adapter_dict['database'],
+            host=adapter_dict['host'],
+            port=adapter_dict['port'],
             user=adapter_dict['user'],
-            password=adapter_dict['password'],
-            database=adapter_dict['database'],
-            schema=adapter_dict['schema'],
-            warehouse=adapter_dict['warehouse'],
-            role=adapter_dict['role']
+            password=adapter_dict['password']
         )
-        return ctx
 
-    def execute_sql(self, query: str, return_type: str) -> pd.DataFrame:
+        # Autocommit. If no autocommit is specified, then set to True
+        try:
+            autocommit_config = bool(adapter_dict['autocommit'])
+            conn.set_session(autocommit=autocommit_config)
+        except KeyError:
+            conn.set_session(autocommit=True)
+        return conn
+
+    def execute_sql(self, query: str, return_type: Optional[str]) -> pd.DataFrame:
         """
         Execute the SQL query
         """
         # Create cursor for every SQL query -- this ensures thread safety
         cursor = self.engine.cursor()
         cursor.execute(query)
+        data = cursor.fetchall()
+
+        # If the return type is `pandas`, then return a DataFrame
         if return_type == "pandas":
-            df: pd.DataFrame = cursor.fetch_pandas_all()
+            cols = []
+            for elts in cursor.description:
+                cols.append(elts[0])
+            df: pd.DataFrame = pd.DataFrame(data=data, columns=cols)
             cursor.close()
             return df
+
+        # Otherwise, return the data as it exists
         else:
-            # Fetch one to ensure that the query was executed
-            cursor.fetchone()
             cursor.close()
+            return data
```

### Comparing `prism-ds-0.2.0rc1/prism/profiles/trino.py` & `prism-ds-0.2.0rc2/prism/profiles/trino.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ###########
 # Imports #
 ###########
 
 # Standard library imports
 import pandas as pd
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 import trino
 
 # Prism-specific imports
 from .adapter import Adapter
 import prism.exceptions
 
 
@@ -158,26 +158,29 @@
                     adapter_dict['user'],
                     adapter_dict['password']
                 )
             )
 
         return conn
 
-    def execute_sql(self, query: str, return_type: str) -> pd.DataFrame:
+    def execute_sql(self, query: str, return_type: Optional[str]) -> pd.DataFrame:
         """
         Execute the SQL query
         """
         # Create cursor for every SQL query -- this ensures thread safety
         cursor = self.engine.cursor()
         cursor.execute(query)
+        data = cursor.fetchall()
+
+        # If the return type is `pandas`, then return a DataFrame
         if return_type == "pandas":
-            data = cursor.fetchall()
             cols = []
             for elts in cursor.description:
                 cols.append(elts[0])
             df: pd.DataFrame = pd.DataFrame(data=data, columns=cols)
             cursor.close()
             return df
+
+        # Otherwise, return the data as it exists
         else:
-            # Fetch one to ensure that the query was executed
-            cursor.fetchone()
             cursor.close()
+            return data
```

### Comparing `prism-ds-0.2.0rc1/prism/spark/wrapper.py` & `prism-ds-0.2.0rc2/prism/spark/wrapper.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/target.py` & `prism-ds-0.2.0rc2/prism/target.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,16 +69,12 @@
 
     def save(self, **kwargs):
 
         # Imports
         import json
 
         # Check object type
-        if not isinstance(self.obj, dict):
-            raise ValueError(
-                "object must be a dictionary!"
-            )
         json_object = json.dumps(self.obj, **kwargs)
 
         # Write
         with open(self.loc, "w") as f:
             f.write(json_object)
```

### Comparing `prism-ds-0.2.0rc1/prism/task.py` & `prism-ds-0.2.0rc2/prism/task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/templates/minimal_project/modules/class_task.py` & `prism-ds-0.2.0rc2/prism/templates/minimal_project/tasks/class_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/templates/minimal_project/modules/decorated_task.py` & `prism-ds-0.2.0rc2/prism/templates/starter_project/tasks/decorated_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/templates/minimal_project/prism_project.py` & `prism-ds-0.2.0rc2/prism/templates/minimal_project/prism_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
     # Add more paths here!
 ]
```

### Comparing `prism-ds-0.2.0rc1/prism/templates/starter_project/dev/dev.ipynb` & `prism-ds-0.2.0rc2/prism/templates/starter_project/dev/dev.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921875%*

 * *Differences: {"'cells'": "{0: {'source': ['**Use this notebook for developing code before productionizing it "*

 * *            "within tasks**']}}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "7eafd19a",
             "metadata": {},
             "source": [
-                "**Use this notebook for developing code before productionizing it within modules**"
+                "**Use this notebook for developing code before productionizing it within tasks**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "b771bf53",
             "metadata": {},
```

### Comparing `prism-ds-0.2.0rc1/prism/templates/starter_project/modules/class_task.py` & `prism-ds-0.2.0rc2/prism/templates/starter_project/tasks/class_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/templates/starter_project/modules/decorated_task.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/tasks/decorated_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/templates/starter_project/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/unit/test_agent/prism_project.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,51 +5,51 @@
 # Imports
 from prism.admin import generate_run_id, generate_run_slug
 import logging
 from pathlib import Path
 
 
 # Project metadata
-NAME = ""
+NAME = "Docker agent test"
 AUTHOR = ""
 VERSION = ""
 DESCRIPTION = """
 """
 
 # Admin
 RUN_ID = generate_run_id()
 SLUG = generate_run_slug()
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
-    # Add more paths here!
+    Path(__file__).parent.parent / 'test_trigger_yml'
 ]
 
 
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
 # then 1 task is run at a time.
 THREADS = 1
 
 
 # Profile directory and name
-PROFILE_YML_PATH = Path(__file__).parent / 'profile.yml'
-PROFILE = "default"
+PROFILE_YML_PATH = Path(__file__).parent / 'paths_test' / 'profile.yml'
+PROFILE = "profile_agent_test"
 
 
 # Logger
 PRISM_LOGGER = logging.getLogger("PRISM_LOGGER")
 
 
 # Triggers
-TRIGGERS_YML_PATH = Path(__file__).parent / 'triggers.yml'
+TRIGGERS_YML_PATH = Path(__file__).parent.parent / 'test_trigger_yml' / 'triggers.yml'
 TRIGGERS = {
-    'on_success': [],
+    'on_success': ["test_agent_trigger"],
     'on_failure': [],
 }
 
 
 # Other variables / parameters. Make sure to capitalize all of these!
 VAR_1 = {'a': 'b'}
 VAR_2 = 200
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/integration_test_class.py` & `prism-ds-0.2.0rc2/prism/tests/integration/integration_test_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 import yaml
 import pandas as pd
 import json
 from typing import Any, Dict, List
 
 # Prism imports
 import prism.cli.base
-# from prism.main import main
 import prism.prism_logging
 
 # Ignore ResourceWarnings introduced by boto3
 import warnings
 
 #################################
 # Test case directory and paths #
@@ -56,52 +55,55 @@
             os.unlink(Path.cwd() / 'logs.log')
 
         os.chdir(TEST_PROJECTS)
 
     def _is_valid_project(self, path):
         """
         Determine if `path` is a valid project (i.e., that is has a `prism_project.py`
-        file and a `modules` folder)
+        file and a `tasks` folder)
 
         args:
             path: project path
         returns:
             boolean indicating whether `path` is a valid project
         """
         os.chdir(path)
         project_dir = prism.cli.base.get_project_dir()
         self.assertTrue(project_dir == path)
-        self.assertTrue(Path(project_dir / 'modules').is_dir())
+        self.assertTrue(Path(project_dir / 'tasks').is_dir())
 
     def _load_manifest(self, path: Path) -> dict:
         """
         Load manifest
         """
         with open(path, 'r') as f:
             manifest = json.load(f)
         f.close()
         return manifest
 
-    def _load_module_refs(
+    def _load_task_refs(
         self,
         module_name: str,
+        task_name: str,
         manifest: Dict[str, Any]
     ) -> List[str]:
         """
-        Load refs associated with module
+        Load refs associated with task
         """
-        module_refs = []
+        task_refs = []
         all_refs = manifest["refs"]
-        for ref_obj in all_refs:
-            if ref_obj["target"] == module_name:
-                module_refs.append(ref_obj["source"])
-        if len(module_refs) == 1:
-            return module_refs[0]
+        if module_name in all_refs.keys():
+            module_refs = all_refs[module_name]
+            if task_name in module_refs.keys():
+                task_refs = module_refs[task_name]
+                return task_refs
+            else:
+                return []
         else:
-            return module_refs
+            return []
 
     def _run_prism(self, args: list):
         """
         Run prism using `args`
         """
         return invoke(args, bool_return=True)
 
@@ -211,38 +213,38 @@
                 os.unlink(filename)
 
     def _file_as_str(self, path):
         """
         Open file as string
         """
         with open(path, 'r') as f:
-            compiled_module_str = f.read()
+            compiled_task_str = f.read()
         f.close()
-        return compiled_module_str
+        return compiled_task_str
 
-    def _compiled_module_if_name_main(self, path):
+    def _compiled_task_if_name_main(self, path):
         """
         Get `if __name__ == "__main__"` body from `path
         """
-        compiled_module_str = self._file_as_str(path)
-        if_name_main_body = self._get_if_name_main_body(compiled_module_str)
+        compiled_task_str = self._file_as_str(path)
+        if_name_main_body = self._get_if_name_main_body(compiled_task_str)
         return if_name_main_body
 
-    def _get_if_name_main_body(self, module_str: str) -> str:
+    def _get_if_name_main_body(self, task_str: str) -> str:
         """
         Get the body of `if __name__ == "__main__"` and return it as a string
 
         args:
-            module_str: module with `if __name__ == "__main__"` as a string
+            task_str: task with `if __name__ == "__main__"` as a string
         returns:
             the body of `if __name__ == "__main__"`
         """
-        module_ast_tree = ast.parse(module_str)
-        self.assertTrue(isinstance(module_ast_tree, ast.Module))
-        if_name_main_block = module_ast_tree.body[-1]
+        task_ast_tree = ast.parse(task_str)
+        self.assertTrue(isinstance(task_ast_tree, ast.Module))
+        if_name_main_block = task_ast_tree.body[-1]
         self.assertTrue(isinstance(if_name_main_block, ast.If))
         return astor.to_source(if_name_main_block)
 
     def _remove_profile_yml(self, wkdir):
         """
         Remove the profile YML file, if it exists
         """
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_client.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,18 +32,19 @@
 TEST_CASE_WKDIR = os.path.dirname(__file__)
 TEST_PROJECTS = Path(TEST_CASE_WKDIR) / 'test_projects'
 
 # Project directories
 P002_NO_PROJECT_PY = Path(TEST_PROJECTS / '002_no_project_py')
 P003_PROJECT_WITH_CYCLE = Path(TEST_PROJECTS / '003_project_with_cycle')
 P004_SIMPLE_PROJECT = Path(TEST_PROJECTS / '004_simple_project')
-P005_SIMPLE_PROJECT_NO_NULL = Path(TEST_PROJECTS / '005_simple_project_no_null')
+P005_SIMPLE_PROJECT_NO_NULL = Path(TEST_PROJECTS / '005_simple_project_no_null_tasks')
 P006_SIMPLE_PROJECT_WITH_PROFILE = Path(TEST_PROJECTS / '006_simple_project_with_profile')  # noqa: E501
 P007_SPARK_PROJECT = Path(TEST_PROJECTS / '007_spark_project')
 P009_SIMPLE_DBT_PROJECT = Path(TEST_PROJECTS / '009_simple_dbt_project' / 'prism')
+P014_TEST_TRIGGERS_NORMAL = Path(TEST_PROJECTS / '014_test_triggers_normal')
 
 
 #############
 # Constants #
 #############
 
 expected_snowflake_dict = test_connect.expected_snowflake_dict
@@ -88,16 +89,16 @@
             shutil.rmtree(Path(P003_PROJECT_WITH_CYCLE / '.compiled'))
 
         # Compile
         with self.assertRaises(prism.exceptions.DAGException) as cm:
             dag.compile()
         expected_msg = "invalid DAG, cycle found in"
         self.assertTrue(expected_msg in str(cm.exception))
-        self.assertTrue('module02.py' in str(cm.exception))
-        self.assertTrue('module03.py' in str(cm.exception))
+        self.assertTrue('module02.Task02' in str(cm.exception))
+        self.assertTrue('module03.Task03' in str(cm.exception))
 
         # Check that manifest is not formed
         self.assertFalse(
             Path(P003_PROJECT_WITH_CYCLE / '.compiled' / 'manifest.json').is_file()
         )
 
         # Set up directory for next test
@@ -122,25 +123,28 @@
             Path(P004_SIMPLE_PROJECT / '.compiled' / 'manifest.json').is_file()
         )
 
         # Check manifest
         manifest = self._load_manifest(
             Path(P004_SIMPLE_PROJECT / '.compiled' / 'manifest.json')
         )
-        module01_refs = self._load_module_refs("module01.py", manifest)
-        module02_refs = self._load_module_refs("module02.py", manifest)
-        module03_refs = self._load_module_refs("module03.py", manifest)
-        self.assertEqual([], module01_refs)
-        self.assertEqual('module01.py', module02_refs)
-        self.assertEqual([], module03_refs)
+        task01_refs = self._load_task_refs("module01", "Task01", manifest)
+        task02_refs = self._load_task_refs("module02", "Task02", manifest)
+        task03_refs = self._load_task_refs("module03", "Task03", manifest)
+        self.assertEqual([], task01_refs)
+        self.assertEqual(['module01.Task01'], task02_refs)
+        self.assertEqual([], task03_refs)
 
         # Check topological sort
         topsort = compiled_dag.topological_sort
         topsort_str = [str(t) for t in topsort]
-        self.assertEqual(['module03.py', 'module01.py', 'module02.py'], topsort_str)
+        self.assertEqual(
+            ['module03.Task03', 'module01.Task01', 'module02.Task02'],
+            topsort_str
+        )
 
         # Remove the .compiled directory, if it exists
         self._remove_compiled_dir(P004_SIMPLE_PROJECT)
 
         # Set up directory for next test
         self._set_up_wkdir()
 
@@ -200,87 +204,87 @@
             Path(P004_SIMPLE_PROJECT / '.compiled' / 'manifest.json').is_file()
         )
 
         # Check manifest.json
         manifest = self._load_manifest(
             Path(P004_SIMPLE_PROJECT / '.compiled' / 'manifest.json')
         )
-        module01_refs = self._load_module_refs("module01.py", manifest)
-        module02_refs = self._load_module_refs("module02.py", manifest)
-        module03_refs = self._load_module_refs("module03.py", manifest)
-        self.assertEqual([], module01_refs)
-        self.assertEqual('module01.py', module02_refs)
-        self.assertEqual([], module03_refs)
+        task01_refs = self._load_task_refs("module01", "Task01", manifest)
+        task02_refs = self._load_task_refs("module02", "Task02", manifest)
+        task03_refs = self._load_task_refs("module03", "Task03", manifest)
+        self.assertEqual([], task01_refs)
+        self.assertEqual(['module01.Task01'], task02_refs)
+        self.assertEqual([], task03_refs)
 
         # Cleanup
         self._remove_compiled_dir(P004_SIMPLE_PROJECT)
 
         # ------------------------------------------------------------------------------
-        # Run P005_SIMPLE_PROJECT_NO_NULL (with and without the `modules` param defined)
+        # Run P005_SIMPLE_PROJECT_NO_NULL (with and without the `tasks` param defined)
 
         # Remove compiled directory and outputs, if they exist
         self._remove_compiled_dir(P005_SIMPLE_PROJECT_NO_NULL)
         self._remove_files_in_output(P005_SIMPLE_PROJECT_NO_NULL)
 
         # -------------------------------------------------------
-        # With `module` param
-        dag5.run(modules=['module01.py'])
+        # With `task` param
+        dag5.run(tasks=['module01'])
 
         # Confirm creation of manifest
         self.assertTrue(Path(P005_SIMPLE_PROJECT_NO_NULL / '.compiled').is_dir())
         self.assertTrue(
             Path(P005_SIMPLE_PROJECT_NO_NULL / '.compiled' / 'manifest.json').is_file()
         )
 
         # Confirm creation of outputs
         self.assertTrue(
-            Path(P005_SIMPLE_PROJECT_NO_NULL / 'output' / 'module01.txt').is_file()
+            Path(P005_SIMPLE_PROJECT_NO_NULL / 'output' / 'task01.txt').is_file()
         )
         self.assertFalse(
-            Path(P005_SIMPLE_PROJECT_NO_NULL / 'output' / 'module02.txt').is_file()
+            Path(P005_SIMPLE_PROJECT_NO_NULL / 'output' / 'task02.txt').is_file()
         )
 
         # Confirm contents of outputs
-        module01_txt = self._file_as_str(
-            Path(P005_SIMPLE_PROJECT_NO_NULL / 'output' / 'module01.txt')
+        task01_txt = self._file_as_str(
+            Path(P005_SIMPLE_PROJECT_NO_NULL / 'output' / 'task01.txt')
         )
-        expected_output = 'Hello from module 1!'
-        self.assertEqual(expected_output, module01_txt)
+        expected_output = 'Hello from task 1!'
+        self.assertEqual(expected_output, task01_txt)
 
         # -------------------------------------------------------
-        # Without `module` param
+        # Without `task` param
         dag5.run()
 
         # Confirm creation of outputs
         self.assertTrue(
-            Path(P005_SIMPLE_PROJECT_NO_NULL / 'output' / 'module01.txt').is_file()
+            Path(P005_SIMPLE_PROJECT_NO_NULL / 'output' / 'task01.txt').is_file()
         )
         self.assertTrue(
-            Path(P005_SIMPLE_PROJECT_NO_NULL / 'output' / 'module02.txt').is_file()
+            Path(P005_SIMPLE_PROJECT_NO_NULL / 'output' / 'task02.txt').is_file()
         )
 
         # Confirm contents of outputs
-        module02_txt = self._file_as_str(
-            Path(P005_SIMPLE_PROJECT_NO_NULL / 'output' / 'module02.txt')
+        task02_txt = self._file_as_str(
+            Path(P005_SIMPLE_PROJECT_NO_NULL / 'output' / 'task02.txt')
         )
-        expected_output = 'Hello from module 1!\nHello from module 2!'
-        self.assertEqual(expected_output, module02_txt)
+        expected_output = 'Hello from task 1!\nHello from task 2!'
+        self.assertEqual(expected_output, task02_txt)
 
         # Remove compiled directory and outputs, if they exist
         self._remove_compiled_dir(P005_SIMPLE_PROJECT_NO_NULL)
 
         # ------------------------------------------------------------------------------
         # Run P009_SIMPLE_DBT_PROJECT to confirm that projects with profiles run as
         # expected
 
         # Remove compiled directory and outputs, if they exist
         self._remove_compiled_dir(P009_SIMPLE_DBT_PROJECT)
         self._remove_files_in_output(P009_SIMPLE_DBT_PROJECT)
 
-        dag9.run(modules=['filter_customers.py'])
+        dag9.run(tasks=['filter_customers.py'])
 
         self.assertTrue(Path(P009_SIMPLE_DBT_PROJECT / '.compiled').is_dir())
         self.assertTrue(
             Path(P009_SIMPLE_DBT_PROJECT / '.compiled' / 'manifest.json').is_file()
         )
 
         # Check contents of output
@@ -306,40 +310,72 @@
 
         # Remove compiled folder
         self._remove_compiled_dir(P009_SIMPLE_DBT_PROJECT)
 
         # Set up directory for next test
         self._set_up_wkdir()
 
+    def test_run_with_triggers(self):
+        """
+        Test run with some triggers
+        """
+        dag = prism.client.PrismDAG(P014_TEST_TRIGGERS_NORMAL)
+
+        # Confirm expected output doesn't exist
+        trigger_output = Path(P014_TEST_TRIGGERS_NORMAL / 'output' / 'trigger.txt')
+        if trigger_output.is_file():
+            os.unlink(trigger_output)
+        self.assertFalse(trigger_output.is_file())
+
+        # Run. This will produce an error, but we want to see if our trigger output was
+        # created
+        try:
+            dag.run()
+        except Exception:
+            pass
+
+        # We expect the trigger to produce an output
+        self.assertTrue(trigger_output.is_file())
+        with open(trigger_output, 'r') as f:
+            trigger_output_str = f.read()
+        expected_str = 'This is outputted from the trigger function!'
+        self.assertTrue(expected_str, trigger_output_str)
+
+        # Remove compiled folder
+        self._remove_compiled_dir(P014_TEST_TRIGGERS_NORMAL)
+
+        # Set up directory for next test
+        self._set_up_wkdir()
+
     def test_get_task_output(self):
         """
         Test task output retrieval
         """
         # Use P005_SIMPLE_PROJECT_NO_NULL for testing
         dag5 = prism.client.PrismDAG(P005_SIMPLE_PROJECT_NO_NULL)
 
         # Get output of a task without a target (without running pipeline). This should
         # result in an error.
         with self.assertRaises(prism.exceptions.RuntimeException) as cm:
-            dag5.get_task_output('module03.py')
+            dag5.get_task_output('module03')
         expected_msg_components = ['cannot access the output of', 'either explicitly running task or setting a target']  # noqa: E501
         for comp in expected_msg_components:
             self.assertTrue(comp in str(cm.exception))
 
         # Get output of a task with a target (without running pipeline)
-        module01_output = dag5.get_task_output('module01.py')
+        task01_output = dag5.get_task_output('module01.py')
         expected_output = str(
-            Path(P005_SIMPLE_PROJECT_NO_NULL / 'output' / 'module01.txt')
+            Path(P005_SIMPLE_PROJECT_NO_NULL / 'output' / 'task01.txt')
         )
-        self.assertEqual(str(module01_output), expected_output)
+        self.assertEqual(str(task01_output), expected_output)
 
         # Get output of a task without a target (after running pipeline)
         dag5.run()
         output = dag5.get_task_output('module03.py')
-        expected_output = 'Hello from module 1!\nHello from module 2!\nHello from module 3!'  # noqa: E501
+        expected_output = 'Hello from task 1!\nHello from task 2!\nHello from task 3!'  # noqa: E501
         self.assertEqual(expected_output, output)
 
         # Remove compiled directory and outputs, if they exist
         self._remove_compiled_dir(P005_SIMPLE_PROJECT_NO_NULL)
 
         # Set up directory for next test
         self._set_up_wkdir()
@@ -358,15 +394,15 @@
         expected_msg_components = ['cannot access the output of', 'either explicitly running task or setting a target']  # noqa: E501
         for comp in expected_msg_components:
             self.assertTrue(comp in str(cm.exception))
 
         # Get output of a task with a target (without running pipeline)
         dag5.run()
         output = dag5.get_pipeline_output()
-        expected_output = 'Hello from module 1!\nHello from module 2!\nHello from module 3!\nHello from module 4!'  # noqa: E501
+        expected_output = 'Hello from task 1!\nHello from task 2!\nHello from task 3!\nHello from task 4!'  # noqa: E501
         self.assertEqual(expected_output, output)
 
         # Remove compiled directory and outputs, if they exist
         self._remove_compiled_dir(P005_SIMPLE_PROJECT_NO_NULL)
 
         # Set up directory for next test
         self._set_up_wkdir()
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_compile.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_compile.py`

 * *Files 20% similar despite different names*

```diff
@@ -45,31 +45,31 @@
 
 # Expected events for `compile` task when called on project with cycle
 project_with_error_expected_events = [
     'SeparatorEvent',
     'TaskRunEvent',
     'CurrentProjectDirEvent',
     'EmptyLineEvent',
-    'ExecutionEvent - module DAG - RUN',
-    'ExecutionEvent - module DAG - ERROR',
+    'ExecutionEvent - task DAG - RUN',
+    'ExecutionEvent - task DAG - ERROR',
     'EmptyLineEvent',
     'PrismExceptionErrorEvent',
     'SeparatorEvent'
 ]
 
 # Expected events for `compile` task when called on a simple project. Not that the
-# `compile` task does not fire events for each module that is compiled, so the different
+# `compile` task does not fire events for each task that is compiled, so the different
 # compile  CLI arguments below should produce the same events.
 simple_project_expected_events = [
     'SeparatorEvent',
     'TaskRunEvent',
     'CurrentProjectDirEvent',
     'EmptyLineEvent',
-    'ExecutionEvent - module DAG - RUN',
-    'ExecutionEvent - module DAG - DONE',
+    'ExecutionEvent - task DAG - RUN',
+    'ExecutionEvent - task DAG - DONE',
     'EmptyLineEvent',
     'TaskSuccessfulEndEvent',
     'SeparatorEvent'
 ]
 
 
 ##############################
@@ -89,15 +89,15 @@
 
         # Execute command
         args = ['compile']
         compile_run = self._run_prism(args)
         compile_run_results = compile_run.get_results()
         self.assertEqual(' | '.join(no_project_py_expected_events), compile_run_results)
 
-        # Check that none of the modules are compiled
+        # Check that none of the tasks are compiled
         self.assertFalse(Path(wkdir / '.compiled').is_dir())
         self.assertFalse(Path(wkdir / '.compiled' / 'manifest.json').is_file())
 
         # Set up wkdir for the next test case
         self._set_up_wkdir()
 
     def test_project_with_cycle(self):
@@ -117,25 +117,25 @@
         compile_run = self._run_prism(args)
         compile_run_results = compile_run.get_results()
         self.assertEqual(
             ' | '.join(project_with_error_expected_events),
             compile_run_results
         )
 
-        # Check that none of the modules are compiled
+        # Check that none of the tasks are compiled
         self.assertTrue(Path(wkdir / '.compiled').is_dir())
         self.assertFalse(Path(wkdir / '.compiled' / 'manifest.json').is_file())
 
         # Set up wkdir for the next test case
         shutil.rmtree(Path(wkdir / '.compiled'))
         self._set_up_wkdir()
 
-    def test_simple_project_all_modules(self):
+    def test_simple_project_all_tasks(self):
         """
-        `prism compile` using all modules
+        `prism compile` using all tasks
         """
 
         # Set working directory
         wkdir = Path(TEST_PROJECTS) / '004_simple_project'
         os.chdir(wkdir)
 
         # Remove the .compiled directory, if it exists
@@ -152,28 +152,28 @@
 
         # Check that .compiled directory is formed
         self.assertTrue(Path(wkdir / '.compiled').is_dir())
         self.assertTrue(Path(wkdir / '.compiled' / 'manifest.json').is_file())
 
         # Check elements of manifest
         manifest = self._load_manifest(Path(wkdir / '.compiled' / 'manifest.json'))
-        module01_refs = self._load_module_refs("module01.py", manifest)
-        module02_refs = self._load_module_refs("module02.py", manifest)
-        module03_refs = self._load_module_refs("module03.py", manifest)
-        self.assertEqual([], module01_refs)
-        self.assertEqual('module01.py', module02_refs)
-        self.assertEqual([], module03_refs)
+        task01_refs = self._load_task_refs("module01", "Task01", manifest)
+        task02_refs = self._load_task_refs("module02", "Task02", manifest)
+        task03_refs = self._load_task_refs("module03", "Task03", manifest)
+        self.assertEqual([], task01_refs)
+        self.assertEqual(['module01.Task01'], task02_refs)
+        self.assertEqual([], task03_refs)
 
         # Set up wkdir for the next test case
         shutil.rmtree(Path(wkdir / '.compiled'))
         self._set_up_wkdir()
 
-    def test_project_nested_module_dirs(self):
+    def test_project_nested_task_dirs(self):
         """
-        `prism compile` in a project with directories in the modules folder
+        `prism compile` in a project with directories in the tasks folder
         """
 
         # Set working directory
         wkdir = Path(TEST_PROJECTS) / '010_project_nested_module_dirs'
         os.chdir(wkdir)
 
         # Remove the .compiled directory, if it exists
@@ -190,22 +190,38 @@
 
         # Check that .compiled directory is formed
         self.assertTrue(Path(wkdir / '.compiled').is_dir())
         self.assertTrue(Path(wkdir / '.compiled' / 'manifest.json').is_file())
 
         # Check elements of manifest
         manifest = self._load_manifest(Path(wkdir / '.compiled' / 'manifest.json'))
-        extract_module01_refs = self._load_module_refs("extract/module01.py", manifest)
-        extract_module02_refs = self._load_module_refs("extract/module02.py", manifest)
-        load_module03_refs = self._load_module_refs("load/module03.py", manifest)
-        module04_refs = self._load_module_refs("module04.py", manifest)
-        self.assertEqual([], extract_module01_refs)
-        self.assertEqual("extract/module01.py", extract_module02_refs)
-        self.assertEqual("extract/module02.py", load_module03_refs)
-        self.assertEqual("load/module03.py", module04_refs)
+        extract_task01_refs = self._load_task_refs(
+            "extract/module01",
+            'Task01',
+            manifest
+        )
+        extract_task02_refs = self._load_task_refs(
+            "extract/module02",
+            'Task02',
+            manifest
+        )
+        load_task03_refs = self._load_task_refs(
+            "load/module03",
+            'Task03',
+            manifest
+        )
+        task04_refs = self._load_task_refs(
+            "module04",
+            "Task04",
+            manifest
+        )
+        self.assertEqual([], extract_task01_refs)
+        self.assertEqual(["extract/module01.Task01"], extract_task02_refs)
+        self.assertEqual(["extract/module02.Task02"], load_task03_refs)
+        self.assertEqual(["load/module03.Task03"], task04_refs)
 
         # Set up wkdir for the next test case
         shutil.rmtree(Path(wkdir / '.compiled'))
         self._set_up_wkdir()
 
     def test_bad_task_ref(self):
         """
@@ -223,14 +239,89 @@
         args = ['compile']
         compile_run = self._run_prism(args)
         compile_run_results = compile_run.get_results()
         self.assertEqual(
             ' | '.join(project_with_error_expected_events),
             compile_run_results
         )
+
+        # Check that .compiled directory is not created
+        self.assertTrue(Path(wkdir / '.compiled').is_dir())
+        self.assertFalse(Path(wkdir / '.compiled' / 'manifest.json').is_file())
+
+        # Set up wkdir for the next test case
+        shutil.rmtree(Path(wkdir / '.compiled'))
+        self._set_up_wkdir()
+
+    def test_project_with_local_tasks(self):
+        """
+        `prism compile` works as expected with multiple tasks are defined in a single
+        file and `local` is correctly specified
+        """
+        # Set working directory
+        wkdir = Path(TEST_PROJECTS) / '021_project_with_local_tasks'
+        os.chdir(wkdir)
+
+        # Remove compiled directory, if it exists
+        self._remove_compiled_dir(wkdir)
+
+        # Compile the project
+        args = ['compile']
+        compile_run = self._run_prism(args)
+        compile_run_results = compile_run.get_results()
+        self.assertEqual(
+            ' | '.join(simple_project_expected_events),
+            compile_run_results
+        )
+
+        # Check elements of manifest
+        manifest = self._load_manifest(Path(wkdir / '.compiled' / 'manifest.json'))
+        extract_refs = self._load_task_refs(
+            "extract",
+            'extract',
+            manifest
+        )
+        transform_refs = self._load_task_refs(
+            "transform_load",
+            'transform',
+            manifest
+        )
+        load_refs = self._load_task_refs(
+            "transform_load",
+            'load',
+            manifest
+        )
+        self.assertEqual([], extract_refs)
+        self.assertEqual(["extract.extract"], transform_refs)
+        self.assertEqual(["transform_load.transform"], load_refs)
+
+        # Set up wkdir for the next test case
+        shutil.rmtree(Path(wkdir / '.compiled'))
+        self._set_up_wkdir()
+
+    def test_project_with_bad_local_tasks(self):
+        """
+        `prism compile` works as expected with multiple tasks are defined in a single
+        file and `local` is correctly specified
+        """
+        # Set working directory
+        wkdir = Path(TEST_PROJECTS) / '022_project_with_bad_local_tasks'
+        os.chdir(wkdir)
+
+        # Remove compiled directory, if it exists
+        self._remove_compiled_dir(wkdir)
+
+        # Compile the project
+        args = ['compile']
+        compile_run = self._run_prism(args)
+        compile_run_results = compile_run.get_results()
+        self.assertEqual(
+            ' | '.join(project_with_error_expected_events),
+            compile_run_results
+        )
 
         # Check that .compiled directory is not created
         self.assertTrue(Path(wkdir / '.compiled').is_dir())
         self.assertFalse(Path(wkdir / '.compiled' / 'manifest.json').is_file())
 
         # Set up wkdir for the next test case
         shutil.rmtree(Path(wkdir / '.compiled'))
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_connect.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_connect.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_create.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #################################
 
 # Directory containing all prism_project.py test cases
 TEST_CASE_WKDIR = os.path.dirname(__file__)
 TEST_PROJECTS = Path(TEST_CASE_WKDIR) / 'test_projects'
 
 # Project directories
-P005_SIMPLE_PROJECT_NO_NULL = Path(TEST_PROJECTS / '005_simple_project_no_null')
+P005_SIMPLE_PROJECT_NO_NULL = Path(TEST_PROJECTS / '021_project_with_local_tasks')
 
 
 ###################
 # Expected events #
 ###################
 
 SUCCESS_EXPECTED_CREATE_START_EVENTS = [
@@ -76,15 +76,15 @@
         """
         Create `triggers.yml` file
         """
         # Change directory to 005_simple_project_with_profile
         self.maxDiff = None
 
         # Set working directory
-        wkdir = Path(TEST_PROJECTS) / '005_simple_project_no_null'
+        wkdir = Path(TEST_PROJECTS) / '021_project_with_local_tasks'
         os.chdir(wkdir)
 
         # First, check that `triggers.yml` does not exist in the project
         self.assertFalse(Path(wkdir / 'triggers.yml').is_file())
 
         # Run
         args = ['create', 'trigger', '--type', 'function']
@@ -107,86 +107,86 @@
         """
         Create new tasks
         """
         # Change directory to 005_simple_project_with_profile
         self.maxDiff = None
 
         # Set working directory
-        wkdir = Path(TEST_PROJECTS) / '005_simple_project_no_null'
+        wkdir = Path(TEST_PROJECTS) / '021_project_with_local_tasks'
         os.chdir(wkdir)
 
         # First, check that `dummy_task.py` does not exist in the project
-        self.assertFalse(Path(wkdir / 'modules' / 'dummy_task.py').is_file())
+        self.assertFalse(Path(wkdir / 'tasks' / 'dummy_task.py').is_file())
 
         # ------------------------------------------------------------------------------
         # Run
         args = ['create', 'task', '--type', 'python', '--name', 'dummy_task']
         create_task_run = self._run_prism(args)
 
         # `triggers.yml` file was found
-        self.assertTrue(Path(wkdir / 'modules' / 'dummy_task.py').is_file())
+        self.assertTrue(Path(wkdir / 'tasks' / 'dummy_task.py').is_file())
 
         # Expected events
         expected_events = SUCCESS_EXPECTED_CREATE_START_EVENTS \
             + SUCCESS_EXPECTED_CREATE_TASK_EVENTS \
             + SUCCESS_EXPECTED_CREATE_END_EVENTS
         self.assertEqual(' | '.join(expected_events), create_task_run.get_results())
 
         # Get the class name
-        with open(Path(wkdir / 'modules' / 'dummy_task.py'), 'r') as f:
+        with open(Path(wkdir / 'tasks' / 'dummy_task.py'), 'r') as f:
             dummy_task_py = f.read()
         self.assertTrue("class DummyTask(prism.task.PrismTask):" in dummy_task_py)
 
         # ------------------------------------------------------------------------------
         # Try creating `dummy_task.py` again. It should raise an error
         run_twice = self._run_prism(args)
         expected_events = SUCCESS_EXPECTED_CREATE_START_EVENTS \
             + SUCCESS_EXPECTED_CREATE_TASK_EVENTS \
             + TASK_ALREADY_EXISTS_END_EVENTS
         self.assertEqual(' | '.join(expected_events), run_twice.get_results())
 
         # Remove task
-        os.unlink(Path(wkdir / 'modules' / 'dummy_task.py'))
+        os.unlink(Path(wkdir / 'tasks' / 'dummy_task.py'))
 
         # Set up wkdir for the next test case
         self._set_up_wkdir()
 
     def test_create_decorated_task(self):
         """
         Created a task using the --decorated flag. This will create a class that has
         a decorated function rather than a class.
         """
         # Change directory to 005_simple_project_with_profile
         self.maxDiff = None
 
         # Set working directory
-        wkdir = Path(TEST_PROJECTS) / '005_simple_project_no_null'
+        wkdir = Path(TEST_PROJECTS) / '021_project_with_local_tasks'
         os.chdir(wkdir)
 
         # First, check that `dummy_task.py` does not exist in the project
-        self.assertFalse(Path(wkdir / 'modules' / 'dummy_task.py').is_file())
+        self.assertFalse(Path(wkdir / 'tasks' / 'dummy_task.py').is_file())
 
         # ------------------------------------------------------------------------------
         # Run
         args = [
             'create', 'task', '--type', 'python', '--name', 'dummy_task', '--decorated'
         ]
         create_task_run = self._run_prism(args)
 
         # `triggers.yml` file was found
-        self.assertTrue(Path(wkdir / 'modules' / 'dummy_task.py').is_file())
+        self.assertTrue(Path(wkdir / 'tasks' / 'dummy_task.py').is_file())
 
         # Expected events
         expected_events = SUCCESS_EXPECTED_CREATE_START_EVENTS \
             + SUCCESS_EXPECTED_CREATE_TASK_EVENTS \
             + SUCCESS_EXPECTED_CREATE_END_EVENTS
         self.assertEqual(' | '.join(expected_events), create_task_run.get_results())
 
         # Get the class name
-        with open(Path(wkdir / 'modules' / 'dummy_task.py'), 'r') as f:
+        with open(Path(wkdir / 'tasks' / 'dummy_task.py'), 'r') as f:
             dummy_task_py = f.read()
         self.assertTrue("class DummyTask(prism.task.PrismTask):" not in dummy_task_py)
         decorated_string = "\n".join([
             "@task(",
             "    retries=0,",
             "    retry_delay_seconds=0,",
             "    targets=[",
@@ -194,11 +194,11 @@
             "    ]",
             ")"
         ])
         self.assertTrue(decorated_string in dummy_task_py)
         self.assertTrue("def dummy_task(tasks, hooks):" in dummy_task_py)
 
         # Remove task
-        os.unlink(Path(wkdir / 'modules' / 'dummy_task.py'))
+        os.unlink(Path(wkdir / 'tasks' / 'dummy_task.py'))
 
         # Set up wkdir for the next test case
         self._set_up_wkdir()
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_dbt.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_dbt.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,23 +48,23 @@
         """
         self.maxDiff = None
 
         # Set working directory
         wkdir = Path(TEST_PROJECTS) / '009_simple_dbt_project' / 'prism'
         os.chdir(wkdir)
 
-        # Remove all compiled modules
+        # Remove all compiled tasks
         self._remove_compiled_dir(wkdir)
 
         # Remove all folders / files in the output directory
         self._remove_dirs_in_output(wkdir)
         self._remove_files_in_output(wkdir)
 
         # Execute command.
-        args = ['run', '--module', 'filter_customers.py']
+        args = ['run', '--task', 'filter_customers.py']
         run_results = self._run_prism(args)
         self.assertTrue(Path(wkdir / '.compiled').is_dir())
         self.assertTrue(Path(wkdir / '.compiled' / 'manifest.json').is_file())
         
         # Check contents of output
         df = pd.read_csv(wkdir / 'output' / 'jaffle_shop_customers.csv')
         expected_columns = [
@@ -97,24 +97,24 @@
         """
         self.maxDiff = None
 
         # Set working directory
         wkdir = Path(TEST_PROJECTS) / '009_simple_dbt_project' / 'prism'
         os.chdir(wkdir)
 
-        # Remove all compiled modules
+        # Remove all compiled tasks
         self._remove_compiled_dir(wkdir)
 
         # Remove all folders / files in the output directory
         self._remove_dirs_in_output(wkdir)
         self._remove_files_in_output(wkdir)
         self.assertFalse(Path(wkdir / 'output' / 'bad_adapter.csv').is_file())
 
         # Execute command.
-        args = ['run', '--module', 'bad_adapter.py']
+        args = ['run', '--task', 'bad_adapter.py']
         run_results = self._run_prism(args)
 
         # Nothing should be produced
         self.assertFalse(Path(wkdir / 'output' / 'bad_adapter.csv').is_file())
 
         # Last event in run_results (before separator event) should be an error event
         error_event = run_results.event_list[-2]
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_hooks.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_hooks.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,18 +49,18 @@
         if Path(wkdir / '.compiled').is_dir():
             shutil.rmtree(Path(wkdir / '.compiled'))
         self.maxDiff = None
 
         # ------------------------------------------------------------------------------
         # Run snowflake.py and spark.py
 
-        args = ['spark-submit', '--module', 'snowflake.py', '--module', 'spark.py']
+        args = ['spark-submit', '--task', 'snowflake.py', '--task', 'spark.py']
         self._run_prism(args)
 
-        # Get module 1 and 2 outputs
+        # Get task 1 and 2 outputs
         machinery_sample = pd.read_csv(wkdir / 'output' / 'machinery_sample.csv')
         household_sample = pd.read_csv(wkdir / 'output' / 'household_sample.csv')
         machinery_sample_filtered = pd.read_csv(
             wkdir / 'output' / 'machinery_sample_filtered.csv'
         )
         household_sample_filtered = pd.read_csv(
             wkdir / 'output' / 'household_sample_filtered.csv'
@@ -112,15 +112,15 @@
         if Path(wkdir / '.compiled').is_dir():
             shutil.rmtree(Path(wkdir / '.compiled'))
         self.maxDiff = None
 
         # ------------------------------------------------------------------------------
         # Run bad_adapter.py
 
-        args = ['spark-submit', '--module', 'bad_adapter.py']
+        args = ['spark-submit', '--task', 'bad_adapter.py']
         _ = self._run_prism(args)
 
         # We can't check the error events directly; for now, let's just check that the
         # output wasn't created.
         self.assertFalse(Path(wkdir / 'output' / 'bad_adapter.csv').is_file())
 
         # Remove the .compiled directory, if it exists
@@ -147,15 +147,15 @@
         self.maxDiff = None
 
         # Check that expected output doesn't already exist
         expected_output = Path(wkdir) / 'output' / 'sample_postgres_data.csv'
         self.assertFalse(expected_output.is_file())
 
         # Run project
-        args = ['spark-submit', '--module', 'postgres.py']
+        args = ['spark-submit', '--task', 'postgres.py']
         self._run_prism(args)
 
         # Check output
         self.assertTrue(expected_output.is_file())
         df = pd.read_csv(expected_output)
         self.assertEqual(df.shape[0], 1)
         self.assertEqual(df.test_col[0], 1)
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_init.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/001_init/modules/class_task.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/tasks/class_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/001_init/modules/decorated_task.py` & `prism-ds-0.2.0rc2/prism/templates/minimal_project/tasks/decorated_task.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,12 +31,12 @@
     Execute task.
 
     args:
         tasks: used to reference output of other tasks --> tasks.ref('...')
         hooks: hooks used to augment Prism functionality. These include:
             hooks.sql     --> for executing sql query using an adapter in profile YML
             hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
-            hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
+            hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
     returns:
         task output
     """
     return "Hello, world!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/001_init/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001_init/prism_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()
 SLUG = generate_run_slug()
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
     # Add more paths here!
 ]
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/001a_init_minimal/modules/class_task.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001a_init_minimal/tasks/class_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/001a_init_minimal/modules/decorated_task.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001a_init_minimal/tasks/decorated_task.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,12 +31,12 @@
     Execute task.
 
     args:
         tasks: used to reference output of other tasks --> tasks.ref('...')
         hooks: hooks used to augment Prism functionality. These include:
             hooks.sql     --> for executing sql query using an adapter in profile YML
             hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
-            hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
+            hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
     returns:
         task output
     """
     return "Hello, world!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
     # Add more paths here!
 ]
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/002_no_project_py/functions.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/functions.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,32 +3,39 @@
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
+# Prism project imports
+import prism_project
 
-######################
-## Class definition ##
-######################
 
-class Module01(prism.task.PrismTask):
-
-    ## Run
+####################
+# Class definition #
+####################
+
+class Task02(prism.task.PrismTask):
+    
+    # Run
+    @prism.decorators.target(type=prism.target.Txt, loc=prism_project.OUTPUT / 'task02.txt')
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
+                - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
                 - hooks.sql     --> for executing sql query using an adapter in profile YML
                 - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
         returns:
             task output
         """
-        return "Hello, world!"
+        with open(tasks.ref('module01.py'), 'r') as f:
+            lines = f.read()
+        f.close()
+        return lines + "\n" + "Hello from task 2!"
 
 
 # EOF
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,33 +3,39 @@
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
+# Prism project imports
+import prism_project
 
-######################
-## Class definition ##
-######################
 
-class Module02(prism.task.PrismTask):
+####################
+# Class definition #
+####################
 
-    ## Run
+class Task02(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.Txt,
+        loc=prism_project.OUTPUT / 'task02.txt'
+    )
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        # TODO: Implement the `run` method
-        return None
-
-
-# EOF
+        with open(tasks.ref('extract/module01.py'), 'r') as f:
+            lines = f.read()
+        f.close()
+        return lines + "\n" + "Hello from task 2!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,33 +3,39 @@
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
+# Prism project imports
+import prism_project
 
-######################
-## Class definition ##
-######################
 
-class Module03(prism.task.PrismTask):
+####################
+# Class definition #
+####################
 
-    ## Run
+class Task02(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.Txt,
+        loc=prism_project.OUTPUT / 'task02.txt'
+    )
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        # TODO: Implement the `run` method
-        return None
-
-
-# EOF
+        with open(tasks.ref('extract/this_is_an_error.py'), 'r') as f:
+            lines = f.read()
+        f.close()
+        return lines + "\n" + "Hello from task 2!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 import prism.target
 import prism.decorators
 
 # Prism project imports
 import prism_project
 
 
-######################
-## Class definition ##
-######################
+####################
+# Class definition #
+####################
 
-class Module01(prism.task.PrismTask):
+class Task04(prism.task.PrismTask):
 
-    ## Run
+    # Run
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
+                - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
                 - hooks.sql     --> for executing sql query using an adapter in profile YML
                 - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
         returns:
             task output
         """
-        return "Hello from module 1!"
+        return tasks.ref('module03.py') + "\n" + "Hello from task 4!"
 
 
 # EOF
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,31 +7,32 @@
 import prism.target
 import prism.decorators
 
 # Prism project imports
 import prism_project
 
 
-######################
-## Class definition ##
-######################
+####################
+# Class definition #
+####################
 
-class Module02(prism.task.PrismTask):
+class Task01(prism.task.PrismTask):
 
-    ## Run
+    # Run
+    @prism.decorators.target(type=prism.target.Txt, loc=prism_project.OUTPUT / 'task01.txt')
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
+                - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
                 - hooks.sql     --> for executing sql query using an adapter in profile YML
                 - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
         returns:
             task output
         """
-        return tasks.ref('module03.py') + '\n' + 'Hello fro module 3!'
+        return "Hello from task 1!"
 
 
 # EOF
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,31 +7,33 @@
 import prism.target
 import prism.decorators
 
 # Prism project imports
 import prism_project
 
 
-######################
-## Class definition ##
-######################
-
-class Module03(prism.task.PrismTask):
-
-    ## Run
+####################
+# Class definition #
+####################
+
+class Task03(prism.task.PrismTask):
+    
+    # Run
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
+                - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
                 - hooks.sql     --> for executing sql query using an adapter in profile YML
                 - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
         returns:
             task output
         """
-        return tasks.ref('module02.py') + '\n' + 'Hello from module 3!'
+        with open(tasks.ref('module02.py')) as f:
+            lines = f.read()
+        return lines + '\n' + 'Hello from task 3!'
 
 
 # EOF
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/021_project_with_local_tasks/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/004_simple_project/modules/module01.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,32 +7,47 @@
 import prism.target
 import prism.decorators
 
 # Prism project imports
 import prism_project
 
 
-######################
-## Class definition ##
-######################
-
-class Module01(prism.task.PrismTask):
-
-    ## Run
-    @prism.decorators.target(type=prism.target.Txt, loc=prism_project.OUTPUT / 'module01.txt')
+####################
+# Class definition #
+####################
+
+class BadAdapterTask(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.PandasCsv,
+        loc=prism_project.OUTPUT / 'bad_adapter.csv',
+        index=False
+    )
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        return "Hello from module 1!"
 
-
-# EOF
+        sql = """
+        SELECT
+            *
+        FROM "SNOWFLAKE_SAMPLE_DATA"."TPCH_SF1"."CUSTOMER"
+        WHERE
+            C_MKTSEGMENT = 'MACHINERY'
+        LIMIT 50
+        """
+        df = hooks.sql(
+            adapter_name="snowflake_profile_abcde",
+            query=sql,
+            return_type="pandas"
+        )
+        return df
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/004_simple_project/modules/module02.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,39 +3,31 @@
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
-# Prism project imports
-import prism_project
 
+####################
+# Class definition #
+####################
 
-######################
-## Class definition ##
-######################
+class Task03(prism.task.PrismTask):
 
-class Module02(prism.task.PrismTask):
-
-    ## Run
-    @prism.decorators.target(type=prism.target.Txt, loc=prism_project.OUTPUT / 'module02.txt')
+    # Run
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        with open(tasks.ref('module01.py'), 'r') as f:
+        with open(tasks.ref('extract/module02.py')) as f:
             lines = f.read()
-        f.close()
-        return lines[-5:]
-
-
-# EOF
+        return lines + '\n' + 'Hello from task 3!'
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/004_simple_project/modules/module03.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/modules/module02.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,42 @@
+
 ###########
 # Imports #
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
 # Prism project imports
 import prism_project
 
 
-######################
-## Class definition ##
-######################
-
-class Module03(prism.task.PrismTask):
-    
-    ## Run
+####################
+# Class definition #
+####################
+
+class Task02(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.Txt,
+        loc=prism_project.OUTPUT / 'task01.txt'
+    )
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        # TODO: Implement the `run` method
-        return None
-
-
-# EOF
+        with open(tasks.ref('module01.py'), 'r') as f:
+            lines = f.read()
+        f.close()
+        return lines[-5:]
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/004_simple_project/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/prism_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
 # sys.path config. This gives your tasks access to local modules / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
-    Path(__file__).parent
+    Path(__file__).parent,
+    Path(__file__).parent.parent,
 ]
 
 
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
 # then 1 task is run at a time.
 THREADS = 1
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/005_simple_project_no_null/functions.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/functions.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module01.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module02.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 ###########
 # Imports #
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
@@ -10,32 +11,35 @@
 # Prism project imports
 import prism_project
 
 # Other imports
 from pathlib import Path
 
 
-######################
-## Class definition ##
-######################
-
-class Module01(prism.task.PrismTask):
-
-    ## Run
-    @prism.decorators.target(type=prism.target.Txt, loc=Path(prism_project.OUTPUT) / 'module01.txt')
+####################
+# Class definition #
+####################
+
+class Task02(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.Txt,
+        loc=Path(prism_project.OUTPUT) / 'task02.txt'
+    )
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        return "Hello from module 1!"
-
-
-# EOF
+        with open(tasks.ref('module01.py'), 'r') as f:
+            lines = f.read()
+        f.close()
+        return lines + "\n" + "Hello from task 2!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module02.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/modules/module03.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,42 +3,40 @@
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
-# Prism project imports
-import prism_project
-
 # Other imports
-from pathlib import Path
+import pandas as pd
+
+
+####################
+# Class definition #
+####################
 
+class Task03(prism.task.PrismTask):
 
-######################
-## Class definition ##
-######################
+    def get_txt_output(self, path):
+        with open(path) as f:
+            lines = f.read()
+        f.close()
+        return lines
 
-class Module02(prism.task.PrismTask):
-    
-    ## Run
-    @prism.decorators.target(type=prism.target.Txt, loc=Path(prism_project.OUTPUT) / 'module02.txt')
+    # Run
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        with open(tasks.ref('module01.py'), 'r') as f:
-            lines = f.read()
-        f.close()
-        return lines + "\n" + "Hello from module 2!"
-
-
-# EOF
+        _ = pd.read_csv(tasks.ref('module01.py'))
+        _ = pd.read_csv(tasks.ref('module02.py'))
+        return 'Hello from task 3!'
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module03.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/tasks/module02.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,34 +6,39 @@
 import prism.task
 import prism.target
 import prism.decorators
 
 # Prism project imports
 import prism_project
 
+# Other imports
+import pyspark.sql.functions as F
 
-######################
-## Class definition ##
-######################
-
-class Module03(prism.task.PrismTask):
-    
-    ## Run
+
+####################
+# Class definition #
+####################
+
+class Task02(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.PySparkParquet,
+        loc=str(prism_project.OUTPUT / 'task02'),
+        mode='overwrite'
+    )
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        with open(tasks.ref('module02.py')) as f:
-            lines = f.read()
-        return lines + '\n' + 'Hello from module 3!'
-
-
-# EOF
+        df = hooks.spark.read.parquet(tasks.ref('module01.py'))
+        df_new = df.filter(F.col('col1') >= F.lit('col1_value2'))
+        return df_new
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module04.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,46 @@
+
 ###########
 # Imports #
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
 # Prism project imports
 import prism_project
 
 
-######################
-## Class definition ##
-######################
-
-class Module04(prism.task.PrismTask):
-
-    ## Run
+####################
+# Class definition #
+####################
+
+class PostgresTask(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.PandasCsv,
+        loc=prism_project.OUTPUT / 'sample_postgres_data.csv',
+        index=False
+    )
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        return tasks.ref('module03.py') + "\n" + "Hello from module 4!"
-
-
-# EOF
+        sql = "SELECT 1 AS test_col"
+        df = hooks.sql(
+            adapter_name="postgres_base",
+            query=sql,
+            return_type="pandas"
+        )
+        return df
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/005_simple_project_no_null/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
     Path(__file__).parent.parent,
 ]
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/modules/module01.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,39 @@
+
 ###########
 # Imports #
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
 # Prism project imports
 import prism_project
 
 
-######################
-## Class definition ##
-######################
-
-class Module01(prism.task.PrismTask):
-
-    ## Run
-    @prism.decorators.target(type=prism.target.Txt, loc=prism_project.OUTPUT / 'module01.txt')
+####################
+# Class definition #
+####################
+
+class Task01(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.Txt,
+        loc=prism_project.OUTPUT / 'task01.txt'
+    )
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        return "Hello from module 1!"
-
-
-# EOF
+        return "Hello from task 1!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/modules/module01.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,50 @@
+
 ###########
 # Imports #
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
 # Prism project imports
 import prism_project
 
-
-######################
-## Class definition ##
-######################
-
-class Module02(prism.task.PrismTask):
-    
-    ## Run
-    @prism.decorators.target(type=prism.target.Txt, loc=prism_project.OUTPUT / 'module02.txt')
+# Other imports
+import time
+import pandas as pd
+
+
+####################
+# Class definition #
+####################
+
+class Task01(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.PandasCsv,
+        loc=prism_project.OUTPUT / 'task01.csv', index=False
+    )
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        with open(tasks.ref('module01.py'), 'r') as f:
-            lines = f.read()
-        f.close()
-        return lines + "\n" + "Hello from module 2!"
-
-
-# EOF
+        start_time = time.time()
+        time.sleep(15)
+        end_time = time.time()
+        time_df = pd.DataFrame({
+            'start_time': [start_time],
+            'end_time': [end_time]
+        })
+        return time_df
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/004_simple_project/modules/module03.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,33 @@
+
 ###########
 # Imports #
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
-# Prism project imports
-import prism_project
 
+####################
+# Class definition #
+####################
 
-######################
-## Class definition ##
-######################
+class Task03(prism.task.PrismTask):
 
-class Module03(prism.task.PrismTask):
-    
-    ## Run
+    # Run
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        with open(tasks.ref('module02.py')) as f:
-            lines = f.read()
-        return lines + '\n' + 'Hello from module 3!'
-
-
-# EOF
+        # TODO: Implement the `run` method
+        return None
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module04.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,32 @@
+
 ###########
 # Imports #
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
-# Prism project imports
-import prism_project
-
 
-######################
-## Class definition ##
-######################
+####################
+# Class definition #
+####################
 
-class Module04(prism.task.PrismTask):
+class Task04(prism.task.PrismTask):
 
-    ## Run
+    # Run
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        return tasks.ref('module03.py') + "\n" + "Hello from module 4!"
-
-
-# EOF
+        return tasks.ref('module03.py') + "\n" + "Hello from task 4!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
     Path(__file__).parent.parent,
 ]
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/007_spark_project/modules/module01.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/tasks/module01.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,32 +10,36 @@
 # Prism project imports
 import prism_project
 
 # Other imports
 from pyspark.sql.types import StructType, StructField, StringType
 
 
-######################
-## Class definition ##
-######################
-
-class Module01(prism.task.PrismTask):
-
-    ## Run
-    @prism.decorators.target(type=prism.target.PySparkParquet, loc=str(prism_project.OUTPUT / 'module01'), mode='overwrite')
+####################
+# Class definition #
+####################
+
+class Task01(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.PySparkParquet,
+        loc=str(prism_project.OUTPUT / 'task01'),
+        mode='overwrite'
+    )
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
         # Define schema
         schema = StructType([
             StructField('col1', StringType(), True),
             StructField('col2', StringType(), True),
@@ -51,10 +55,7 @@
             ('col1_value5', 'col2_value5', 'col3_value5'),
             ('col1_value6', 'col2_value6', 'col3_value6')
         ]
 
         # Load data into schema
         df = hooks.spark.createDataFrame(data, schema)
         return df
-
-
-# EOF
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/007_spark_project/modules/module02.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/modules/module04.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,32 @@
+
 ###########
 # Imports #
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
-# Prism project imports
-import prism_project
-
-# Other imports
-import pyspark.sql.functions as F
-
 
-######################
-## Class definition ##
-######################
+####################
+# Class definition #
+####################
 
-class Module02(prism.task.PrismTask):
+class Task04(prism.task.PrismTask):
 
-    ## Run
-    @prism.decorators.target(type=prism.target.PySparkParquet, loc=str(prism_project.OUTPUT / 'module02'), mode='overwrite')
+    # Run
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        df = hooks.spark.read.parquet(tasks.ref('module01.py'))
-        df_new = df.filter(F.col('col1')>=F.lit('col1_value2'))
-        return df_new
-
-
-# EOF
+        return tasks.ref('module03.py') + "\n" + "Hello from task 4!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/007_spark_project/modules/module03.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,37 +6,33 @@
 import prism.task
 import prism.target
 import prism.decorators
 
 # Prism project imports
 import prism_project
 
-# Other imports
-import pyspark.sql.functions as F
 
-
-######################
-## Class definition ##
-######################
-
-class Module03(prism.task.PrismTask):
-
-    ## Run
+####################
+# Class definition #
+####################
+
+class Task01(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.Txt,
+        loc=prism_project.OUTPUT / 'task01.txt'
+    )
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        df = hooks.spark.read.parquet(tasks.ref('module02.py'))
-        df_new = df.filter(F.col('col1')>=F.lit('col1_value3'))
-        return df_new
-
-
-# EOF
+        return "Hello from task 1!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/007_spark_project/modules/module04.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/filter_customers.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,25 +6,23 @@
 import prism.task
 import prism.target
 import prism.decorators
 
 # Prism project imports
 import prism_project
 
-# Other imports
-import pyspark.sql.functions as F
 
+####################
+# Class definition #
+####################
 
-######################
-## Class definition ##
-######################
+class FilterCustomers(prism.task.PrismTask):
 
-class Module04(prism.task.PrismTask):
-
-    ## Run
-    @prism.decorators.target(type=prism.target.PySparkParquet, loc=str(prism_project.OUTPUT / 'module04'), mode='overwrite')
+    # Run    
+    @prism.decorators.target(type=prism.target.PandasCsv, loc=prism_project.OUTPUT / 'jaffle_shop_customers.csv', index=False)
     def run(self, tasks, hooks):
-        df_new = tasks.ref('module03.py').filter(F.col('col1')>=F.lit('col1_value4'))
+        df = hooks.dbt_ref('dbt_profile', 'customers')
+        df_new = df.iloc[:10]
         return df_new
 
 
 # EOF
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/007_spark_project/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
     Path(__file__).parent.parent,
 ]
 
 
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
 # then 1 task is run at a time.
-THREADS = 1
+THREADS = 2
 
 
 # Profile directory and name
 PROFILE_YML_PATH = Path(__file__).parent / 'profile.yml'
 PROFILE = 'default'  # name of profile within `profiles.yml`
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/008_targets/modules/csv.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/csv.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 ###########
 # Imports #
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
@@ -10,29 +11,29 @@
 # Prism project imports
 import prism_project
 
 # Other imports
 import pandas as pd
 
 
-######################
-## Class definition ##
-######################
-
-class Module03(prism.task.PrismTask):
-
-    ## Run    
-    @prism.decorators.target(type=prism.target.PandasCsv, loc=prism_project.OUTPUT / 'target_csv.csv', index=False)
+####################
+# Class definition #
+####################
+
+class BasicCsvTask(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.PandasCsv,
+        loc=prism_project.OUTPUT / 'target_csv.csv', index=False
+    )
     def run(self, tasks, hooks):
         data = {
             'col1': ['col1_value1', 'col1_value2', 'col1_value3'],
             'col2': ['col2_value1', 'col2_value2', 'col2_value3'],
             'col3': ['col3_value1', 'col3_value2', 'col3_value3'],
             'col4': ['col4_value1', 'col4_value2', 'col4_value3'],
             'col5': ['col5_value1', 'col5_value2', 'col5_value3'],
             'col6': ['col6_value1', 'col6_value2', 'col6_value3']
         }
         df = pd.DataFrame(data)
         return df
-
-
-# EOF
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/008_targets/modules/csv_iter.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/csv_mult.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 ###########
 # Imports #
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
@@ -10,22 +11,31 @@
 # Prism project imports
 import prism_project
 
 # Other imports
 import pandas as pd
 
 
-######################
-## Class definition ##
-######################
-
-class CsvIteratorTask(prism.task.PrismTask):
-
-    ## Run    
-    @prism.decorators.target_iterator(type=prism.target.PandasCsv, loc=prism_project.OUTPUT, index=False)
+####################
+# Class definition #
+####################
+
+class MultipleCsvsTask(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.PandasCsv,
+        loc=prism_project.OUTPUT / 'target_csv_mult_df1.csv',
+        index=False
+    )
+    @prism.decorators.target(
+        type=prism.target.PandasCsv,
+        loc=prism_project.OUTPUT / 'target_csv_mult_df2.csv',
+        index=False
+    )
     def run(self, tasks, hooks):
         data1 = {
             'col1': ['col1_value1', 'col1_value2', 'col1_value3'],
             'col2': ['col2_value1', 'col2_value2', 'col2_value3'],
             'col3': ['col3_value1', 'col3_value2', 'col3_value3'],
             'col4': ['col4_value1', 'col4_value2', 'col4_value3'],
             'col5': ['col5_value1', 'col5_value2', 'col5_value3'],
@@ -39,14 +49,8 @@
             'colD': ['colD_value1', 'colD_value2', 'colD_value3'],
             'colE': ['colE_value1', 'colE_value2', 'colE_value3'],
             'colF': ['colF_value1', 'colF_value2', 'colF_value3']
         }
         df1 = pd.DataFrame(data1)
         df2 = pd.DataFrame(data2)
 
-        return {
-            'target_csv_iter_df1.csv': df1,
-            'target_csv_iter_df2.csv': df2,
-        }
-
-
-# EOF
+        return df1, df2
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/008_targets/modules/csv_mult.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/csv_iter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 ###########
 # Imports #
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
@@ -10,23 +11,26 @@
 # Prism project imports
 import prism_project
 
 # Other imports
 import pandas as pd
 
 
-######################
-## Class definition ##
-######################
-
-class Module03(prism.task.PrismTask):
-
-    ## Run    
-    @prism.decorators.target(type=prism.target.PandasCsv, loc=prism_project.OUTPUT / 'target_csv_mult_df1.csv', index=False)
-    @prism.decorators.target(type=prism.target.PandasCsv, loc=prism_project.OUTPUT / 'target_csv_mult_df2.csv', index=False)
+####################
+# Class definition #
+####################
+
+class CsvIteratorTask(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target_iterator(
+        type=prism.target.PandasCsv,
+        loc=prism_project.OUTPUT,
+        index=False
+    )
     def run(self, tasks, hooks):
         data1 = {
             'col1': ['col1_value1', 'col1_value2', 'col1_value3'],
             'col2': ['col2_value1', 'col2_value2', 'col2_value3'],
             'col3': ['col3_value1', 'col3_value2', 'col3_value3'],
             'col4': ['col4_value1', 'col4_value2', 'col4_value3'],
             'col5': ['col5_value1', 'col5_value2', 'col5_value3'],
@@ -39,12 +43,12 @@
             'colC': ['colC_value1', 'colC_value2', 'colC_value3'],
             'colD': ['colD_value1', 'colD_value2', 'colD_value3'],
             'colE': ['colE_value1', 'colE_value2', 'colE_value3'],
             'colF': ['colF_value1', 'colF_value2', 'colF_value3']
         }
         df1 = pd.DataFrame(data1)
         df2 = pd.DataFrame(data2)
-        
-        return df1, df2
-
 
-# EOF
+        return {
+            'target_csv_iter_df1.csv': df1,
+            'target_csv_iter_df2.csv': df2,
+        }
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/008_targets/modules/parquet.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/tasks/parquet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 ###########
 # Imports #
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
@@ -10,32 +11,36 @@
 # Prism project imports
 import prism_project
 
 # Other imports
 from pyspark.sql.types import StructType, StructField, StringType
 
 
-######################
-## Class definition ##
-######################
-
-class Module01(prism.task.PrismTask):
-
-    ## Run
-    @prism.decorators.target(type=prism.target.PySparkParquet, loc=str(prism_project.OUTPUT / 'target_parquet'), mode='overwrite')
+####################
+# Class definition #
+####################
+
+class ParquetTask(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.PySparkParquet,
+        loc=str(prism_project.OUTPUT / 'target_parquet'),
+        mode='overwrite'
+    )
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
         # Define schema
         schema = StructType([
             StructField('col1', StringType(), True),
             StructField('col2', StringType(), True),
@@ -51,10 +56,7 @@
             ('col1_value5', 'col2_value5', 'col3_value5'),
             ('col1_value6', 'col2_value6', 'col3_value6')
         ]
 
         # Load data into schema
         df = hooks.spark.createDataFrame(data, schema)
         return df
-
-
-# EOF
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/008_targets/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/prism_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,30 +16,30 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
     Path(__file__).parent.parent,
 ]
 
 
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
 # then 1 task is run at a time.
 THREADS = 1
 
 
 # Profile directory and name
 PROFILE_YML_PATH = Path(__file__).parent / 'profile.yml'
-PROFILE = 'default'  # name of profile within `profiles.yml`
+PROFILE = None  # name of profile within `profiles.yml`
 
 
 # Logger
 PRISM_LOGGER = logging.getLogger("PRISM_LOGGER")
 
 
 # Other variables / parameters. Make sure to capitalize all of these!
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/bad_adapter.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/bad_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 import prism.target
 import prism.decorators
 
 # Prism project imports
 import prism_project
 
 
-######################
-## Class definition ##
-######################
+####################
+# Class definition #
+####################
 
 class FilterCustomers(prism.task.PrismTask):
 
-    ## Run    
+    # Run    
     @prism.decorators.target(type=prism.target.PandasCsv, loc=prism_project.OUTPUT / 'bad_adapter.csv', index=False)
     def run(self, tasks, hooks):
         df = hooks.dbt_ref('dbt_prsdfofile', 'customers')
         df_new = df.iloc[:10]
         return df_new
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/filter_customers.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/tasks/module04.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,23 +6,26 @@
 import prism.task
 import prism.target
 import prism.decorators
 
 # Prism project imports
 import prism_project
 
+# Other imports
+import pyspark.sql.functions as F
 
-######################
-## Class definition ##
-######################
 
-class FilterCustomers(prism.task.PrismTask):
-
-    ## Run    
-    @prism.decorators.target(type=prism.target.PandasCsv, loc=prism_project.OUTPUT / 'jaffle_shop_customers.csv', index=False)
+####################
+# Class definition #
+####################
+
+class Task04(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.PySparkParquet,
+        loc=str(prism_project.OUTPUT / 'task04'),
+        mode='overwrite'
+    )
     def run(self, tasks, hooks):
-        df = hooks.dbt_ref('dbt_profile', 'customers')
-        df_new = df.iloc[:10]
+        df_new = tasks.ref('module03.py').filter(F.col('col1') >= F.lit('col1_value4'))
         return df_new
-
-
-# EOF
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/prism_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,30 +16,30 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
     Path(__file__).parent.parent,
 ]
 
 
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
 # then 1 task is run at a time.
 THREADS = 1
 
 
 # Profile directory and name
 PROFILE_YML_PATH = Path(__file__).parent / 'profile.yml'
-PROFILE = 'default'  # name of profile within `profiles.yml`
+PROFILE = None  # name of profile within `profiles.yml`
 
 
 # Logger
 PRISM_LOGGER = logging.getLogger("PRISM_LOGGER")
 
 
 # Other variables / parameters. Make sure to capitalize all of these!
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 import prism.target
 import prism.decorators
 
 # Prism project imports
 import prism_project
 
 
-######################
-## Class definition ##
-######################
-
-class Module01(prism.task.PrismTask):
-
-    ## Run
-    @prism.decorators.target(type=prism.target.Txt, loc=prism_project.OUTPUT / 'module01.txt')
+####################
+# Class definition #
+####################
+
+class Task01(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.Txt,
+        loc=prism_project.OUTPUT / 'task01.txt'
+    )
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        return "Hello from module 1!"
-
-
-# EOF
+        return "Hello from task 1!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/modules/module02.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,50 @@
+
 ###########
 # Imports #
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
 # Prism project imports
 import prism_project
 
-
-######################
-## Class definition ##
-######################
-
-class Module02(prism.task.PrismTask):
-    
-    ## Run
-    @prism.decorators.target(type=prism.target.Txt, loc=prism_project.OUTPUT / 'module02.txt')
+# Other imports
+import time
+import pandas as pd
+
+
+####################
+# Class definition #
+####################
+
+class Task02(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.PandasCsv,
+        loc=prism_project.OUTPUT / 'task02.csv', index=False
+    )
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        with open(tasks.ref('extract/module01.py'), 'r') as f:
-            lines = f.read()
-        f.close()
-        return lines + "\n" + "Hello from module 2!"
-
-
-# EOF
+        start_time = time.time()
+        time.sleep(5)
+        end_time = time.time()
+        time_df = pd.DataFrame({
+            'start_time': [start_time],
+            'end_time': [end_time]
+        })
+        return time_df
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module03.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,35 @@
+
 ###########
 # Imports #
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
-# Prism project imports
-import prism_project
 
+####################
+# Class definition #
+####################
 
-######################
-## Class definition ##
-######################
+class Task03(prism.task.PrismTask):
 
-class Module03(prism.task.PrismTask):
-    
-    ## Run
+    # Run
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        with open(tasks.ref('extract/module02.py')) as f:
+        # Use just the module name to get the task output
+        with open(tasks.ref('module02')) as f:
             lines = f.read()
-        return lines + '\n' + 'Hello from module 3!'
-
-
-# EOF
+        return lines + '\n' + 'Hello from task 3!'
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,35 +3,29 @@
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
-# Prism project imports
-import prism_project
 
+####################
+# Class definition #
+####################
 
-######################
-## Class definition ##
-######################
+class Task01(prism.task.PrismTask):
 
-class Module04(prism.task.PrismTask):
-    
-    ## Run
+    # Run
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        return tasks.ref('load/module03.py') + '\n' + "Hello from module 4!"
-
-
-# EOF
+        return "Hello from task 1!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
     Path(__file__).parent.parent,
 ]
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/016_test_triggers_error/tasks/module01.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,36 +3,29 @@
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
-# Prism project imports
-import prism_project
 
+####################
+# Class definition #
+####################
 
-######################
-## Class definition ##
-######################
+class Task01(prism.task.PrismTask):
 
-class Module01(prism.task.PrismTask):
-
-    ## Run
-    @prism.decorators.target(type=prism.target.Txt, loc=prism_project.OUTPUT / 'module01.txt')
+    # Run
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        return "Hello from module 1!"
-
-
-# EOF
+        return "Hello from task 1!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module02.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,43 @@
+
 ###########
 # Imports #
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
 # Prism project imports
 import prism_project
 
 
-######################
-## Class definition ##
-######################
-
-class Module02(prism.task.PrismTask):
-    
-    ## Run
-    @prism.decorators.target(type=prism.target.Txt, loc=prism_project.OUTPUT / 'module02.txt')
+####################
+# Class definition #
+####################
+
+class Task02(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.Txt,
+        loc=prism_project.OUTPUT / 'task02.txt'
+    )
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        with open(tasks.ref('extract/this_is_an_error.py'), 'r') as f:
+        # Use the module name and the task name to get the task output
+        with open(tasks.ref('module01.Task01'), 'r') as f:
             lines = f.read()
         f.close()
-        return lines + "\n" + "Hello from module 2!"
-
-
-# EOF
+        return lines + "\n" + "Hello from task 2!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/tasks/module01.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,37 +3,29 @@
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
-# Prism project imports
-import prism_project
 
+####################
+# Class definition #
+####################
 
-######################
-## Class definition ##
-######################
+class Task01(prism.task.PrismTask):
 
-class Module03(prism.task.PrismTask):
-    
-    ## Run
+    # Run
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        with open(tasks.ref('extract/module02.py')) as f:
-            lines = f.read()
-        return lines + '\n' + 'Hello from module 3!'
-
-
-# EOF
+        return "Hello from task 1!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/tasks/module01.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,35 +3,29 @@
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
-# Prism project imports
-import prism_project
 
+####################
+# Class definition #
+####################
 
-######################
-## Class definition ##
-######################
+class Task01(prism.task.PrismTask):
 
-class Module04(prism.task.PrismTask):
-    
-    ## Run
+    # Run
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        return tasks.ref('load/module03.py') + '\n' + "Hello from module 4!"
-
-
-# EOF
+        return "Hello from task 1!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
     Path(__file__).parent.parent,
 ]
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/012_concurrency/modules/module03.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module04.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,34 @@
+
 ###########
 # Imports #
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
-# Prism project imports
-import prism_project
 
-# Other imports
-import pandas as pd
+####################
+# Class definition #
+####################
 
+class Task04(prism.task.PrismTask):
 
-######################
-## Class definition ##
-######################
-
-class Module03(prism.task.PrismTask):
-
-    def get_txt_output(self, path):
-        with open(path) as f:
-            lines = f.read()
-        f.close()
-        return lines
-    
-    ## Run
+    # Run
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        module1_times = pd.read_csv(tasks.ref('module01.py'))
-        module2_times = pd.read_csv(tasks.ref('module02.py'))
-        return 'Hello from module 3!'
-
-
-# EOF
+        # Use the module name + `.py` suffix to get the task output. This should throw
+        # a warning.
+        return tasks.ref('module03') + "\n" + "Hello from task 4!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/012_concurrency/modules/module04.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,35 +3,29 @@
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
-# Prism project imports
-import prism_project
 
+####################
+# Class definition #
+####################
 
-######################
-## Class definition ##
-######################
+class Task04(prism.task.PrismTask):
 
-class Module04(prism.task.PrismTask):
-
-    ## Run
+    # Run
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        return tasks.ref('module03.py') + "\n" + "Hello from module 4!"
-
-
-# EOF
+        return tasks.ref('load/module03.py') + '\n' + "Hello from task 4!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/012_concurrency/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency/prism_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
     Path(__file__).parent.parent,
 ]
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,35 +3,29 @@
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
-# Prism project imports
-import prism_project
-
 
 ####################
 # Class definition #
 ####################
 
-class PostgresTask(prism.task.PrismTask):
-    
-    ## Run
-    @prism.decorators.target(type=prism.target.PandasCsv, loc=prism_project.OUTPUT / 'sample_postgres_data.csv', index=False)
+class Task04(prism.task.PrismTask):
+
+    # Run
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        sql = "SELECT 1 AS test_col"
-        df = hooks.sql(adapter_name="postgres_base", query=sql)
-        return df
+        return tasks.ref('load/module03.py') + '\n' + "Hello from task 4!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,73 @@
+
 ###########
 # Imports #
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
 # Prism project imports
 import prism_project
 
-# Other imports
-import time
-import pandas as pd
-
 
-######################
-## Class definition ##
-######################
+####################
+# Class definition #
+####################
 
 class SnowflakeTask(prism.task.PrismTask):
 
-    ## Run
-    @prism.decorators.target(type=prism.target.PandasCsv, loc=prism_project.OUTPUT / 'machinery_sample.csv', index=False)
-    @prism.decorators.target(type=prism.target.PandasCsv, loc=prism_project.OUTPUT / 'household_sample.csv', index=False)
+    # Run
+    @prism.decorators.target(
+        type=prism.target.PandasCsv,
+        loc=prism_project.OUTPUT / 'machinery_sample.csv',
+        index=False
+    )
+    @prism.decorators.target(
+        type=prism.target.PandasCsv,
+        loc=prism_project.OUTPUT / 'household_sample.csv',
+        index=False
+    )
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        machinery_sql = f"""
+        machinery_sql = """
         SELECT
             *
         FROM "SNOWFLAKE_SAMPLE_DATA"."TPCH_SF1"."CUSTOMER"
         WHERE
             c_mktsegment = 'MACHINERY'
         ORDER BY
             c_custkey
         LIMIT 50
         """
-        machinery_df = hooks.sql(adapter_name="snowflake_base", query=machinery_sql)
+        machinery_df = hooks.sql(
+            adapter_name="snowflake_base", query=machinery_sql, return_type="pandas"
+        )
 
-        household_sql = f"""
+        household_sql = """
         SELECT
             *
         FROM "SNOWFLAKE_SAMPLE_DATA"."TPCH_SF1"."CUSTOMER"
         WHERE
             c_mktsegment = 'HOUSEHOLD'
         ORDER BY
             c_custkey
         LIMIT 50
         """
-        household_df = hooks.sql(adapter_name="snowflake_base", query=household_sql)
+        household_df = hooks.sql(
+            adapter_name="snowflake_base", query=household_sql, return_type="pandas"
+        )
 
         return machinery_df, household_df
-
-
-# EOF
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,31 +12,31 @@
 
 # Other imports
 import time
 import pandas as pd
 import pyspark.sql.functions as F
 
 
-######################
-## Class definition ##
-######################
+####################
+# Class definition #
+####################
 
 class PysparkTask(prism.task.PrismTask):
     
     # Run
     @prism.decorators.target(type=prism.target.PandasCsv, loc=prism_project.OUTPUT / 'machinery_sample_filtered.csv', index=False)
     @prism.decorators.target(type=prism.target.PandasCsv, loc=prism_project.OUTPUT / 'household_sample_filtered.csv', index=False)
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
+                - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
                 - hooks.sql     --> for executing sql query using an adapter in profile YML
                 - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
         returns:
             task output
         """
         dfs = tasks.ref('snowflake.py')
         machinery_df_path = str(dfs[0])
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/012_concurrency_local/prism_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,30 +16,30 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
     Path(__file__).parent.parent,
 ]
 
 
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
 # then 1 task is run at a time.
 THREADS = 2
 
 
 # Profile directory and name
 PROFILE_YML_PATH = Path(__file__).parent / 'profile.yml'
-PROFILE = 'default'  # name of profile within `profiles.yml`
+PROFILE = None  # name of profile within `profiles.yml`
 
 
 # Logger
 PRISM_LOGGER = logging.getLogger("PRISM_LOGGER")
 
 
 # Other variables / parameters. Make sure to capitalize all of these!
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
 ]
 
 
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
-    Path(__file__).parent
+    Path(__file__).parent,
 ]
 
 
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
 # then 1 task is run at a time.
 THREADS = 1
 
@@ -49,11 +49,12 @@
 # Paths
 WKDIR = Path(__file__).parent
 DATA = WKDIR / 'data'
 OUTPUT = WKDIR / 'output'
 
 
 # Triggers
+TRIGGERS_YML_PATH = Path(__file__).parent / 'triggers.yml'
 TRIGGERS = {
     'on_success': ['test_trigger_function'],
     'on_failure': ['test_trigger_function'],
 }
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/016_test_triggers_error/modules/module01.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,38 +3,33 @@
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
-# Prism project imports
-import prism_project
 
-# Other imports
-from pathlib import Path
+####################
+# Class definition #
+####################
 
+class Task02(prism.task.PrismTask):
 
-######################
-## Class definition ##
-######################
-
-class Module01(prism.task.PrismTask):
-
-    ## Run
+    # Run
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
+                - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
                 - hooks.sql     --> for executing sql query using an adapter in profile YML
                 - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
         returns:
             task output
         """
-        return "Hello from module 1!"
+        # TODO: Implement the `run` method
+        return None
 
 
 # EOF
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
 ]
 
 
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/module01.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,38 +3,33 @@
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
-# Prism project imports
-import prism_project
 
-# Other imports
-from pathlib import Path
+####################
+# Class definition #
+####################
 
+class Task03(prism.task.PrismTask):
 
-######################
-## Class definition ##
-######################
-
-class Module01(prism.task.PrismTask):
-
-    ## Run
+    # Run
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
+                - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
                 - hooks.sql     --> for executing sql query using an adapter in profile YML
                 - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
         returns:
             task output
         """
-        return "Hello from module 1!"
+        # TODO: Implement the `run` method
+        return None
 
 
 # EOF
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
 ]
 
 
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/module01.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module01.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 ###########
 # Imports #
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
@@ -10,31 +11,32 @@
 # Prism project imports
 import prism_project
 
 # Other imports
 from pathlib import Path
 
 
-######################
-## Class definition ##
-######################
-
-class Module01(prism.task.PrismTask):
-
-    ## Run
+####################
+# Class definition #
+####################
+
+class Task01(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.Txt,
+        loc=Path(prism_project.OUTPUT) / 'task01.txt'
+    )
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        return "Hello from module 1!"
-
-
-# EOF
+        return "Hello from task 1!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/019_dec_targets/prism_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
 ]
 
 
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/019_dec_targets/modules/extract.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/019_dec_targets/tasks/extract.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/019_dec_targets/modules/load.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/019_dec_targets/tasks/load.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/019_dec_targets/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/020_dec_retries/prism_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
 ]
 
 
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/020_dec_retries/modules/load.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/020_dec_retries/tasks/load.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/020_dec_retries/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/prism_project.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,29 +16,30 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
+    Path(__file__).parent.parent,
 ]
 
 
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
 # then 1 task is run at a time.
 THREADS = 1
 
 
 # Profile directory and name
 PROFILE_YML_PATH = Path(__file__).parent / 'profile.yml'
-PROFILE = None  # name of profile within `profiles.yml`
+PROFILE = 'default'  # name of profile within `profiles.yml`
 
 
 # Logger
 PRISM_LOGGER = logging.getLogger("PRISM_LOGGER")
 
 
 # Other variables / parameters. Make sure to capitalize all of these!
@@ -46,15 +47,7 @@
 VAR_2 = 200
 VAR_3 = '2015-01-01'
 
 # Paths
 WKDIR = Path(__file__).parent
 DATA = WKDIR / 'data'
 OUTPUT = WKDIR / 'output'
-
-
-# Triggers
-TRIGGERS_YML_PATH = Path(__file__).parent / 'triggers.yml'
-TRIGGERS = {
-    'on_success': ['test_trigger_function'],
-    'on_failure': ['test_trigger_function'],
-}
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/021_no_py_in_ref/modules/module01.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module01.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 ###########
 # Imports #
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
@@ -10,32 +11,32 @@
 # Prism project imports
 import prism_project
 
 # Other imports
 from pathlib import Path
 
 
-######################
-## Class definition ##
-######################
-
-class Module01(prism.task.PrismTask):
-
-    ## Run
-    @prism.decorators.target(type=prism.target.Txt, loc=Path(prism_project.OUTPUT) / 'module01.txt')
+####################
+# Class definition #
+####################
+
+class Task01(prism.task.PrismTask):
+
+    # Run
+    @prism.decorators.target(
+        type=prism.target.Txt,
+        loc=Path(prism_project.OUTPUT) / 'task01.txt'
+    )
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        return "Hello from module 1!"
-
-
-# EOF
+        return "Hello from task 1!"
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/021_no_py_in_ref/modules/module03.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,37 +3,29 @@
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
-# Prism project imports
-import prism_project
 
+####################
+# Class definition #
+####################
 
-######################
-## Class definition ##
-######################
+class Task03(prism.task.PrismTask):
 
-class Module03(prism.task.PrismTask):
-    
-    ## Run
+    # Run
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        with open(tasks.ref('module02')) as f:
-            lines = f.read()
-        return lines + '\n' + 'Hello from module 3!'
-
-
-# EOF
+        return tasks.ref('module02.py') + '\n' + 'Hello from task 3!'
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/021_no_py_in_ref/modules/module04.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/007_spark_project/tasks/module03.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,35 +3,34 @@
 ###########
 
 # Prism infrastructure imports
 import prism.task
 import prism.target
 import prism.decorators
 
-# Prism project imports
-import prism_project
+# Other imports
+import pyspark.sql.functions as F
 
 
-######################
-## Class definition ##
-######################
+####################
+# Class definition #
+####################
 
-class Module04(prism.task.PrismTask):
+class Task03(prism.task.PrismTask):
 
-    ## Run
+    # Run
     def run(self, tasks, hooks):
         """
         Execute task.
 
         args:
             tasks: used to reference output of other tasks --> tasks.ref('...')
             hooks: built-in Prism hooks. These include:
-                - hooks.dbt_ref --> for getting dbt models as a pandas DataFrame
-                - hooks.sql     --> for executing sql query using an adapter in profile YML
-                - hooks.spark   --> for accessing SparkSession (if pyspark specified in profile YML)
+            - hooks.dbt_ref --> for getting dbt tasks as a pandas DataFrame
+            - hooks.sql     --> for executing sql query using an adapter in profile YML
+            - hooks.spark   --> for accessing SparkSession
         returns:
             task output
         """
-        return tasks.ref('module03') + "\n" + "Hello from module 4!"
-
-
-# EOF
+        df = hooks.spark.read.parquet(tasks.ref('module02.py'))
+        df_new = df.filter(F.col('col1') >= F.lit('col1_value3'))
+        return df_new
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_projects/021_no_py_in_ref/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_projects/008_targets/prism_project.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,30 +16,30 @@
 """
 
 # Admin
 RUN_ID = generate_run_id()  # don't delete this!
 SLUG = generate_run_slug()  # don't delete this!
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
     Path(__file__).parent.parent,
 ]
 
 
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
 # then 1 task is run at a time.
 THREADS = 1
 
 
 # Profile directory and name
 PROFILE_YML_PATH = Path(__file__).parent / 'profile.yml'
-PROFILE = None  # name of profile within `profiles.yml`
+PROFILE = 'default'  # name of profile within `profiles.yml`
 
 
 # Logger
 PRISM_LOGGER = logging.getLogger("PRISM_LOGGER")
 
 
 # Other variables / parameters. Make sure to capitalize all of these!
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_spark_submit.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_spark_submit.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,19 +8,23 @@
 """
 
 ###########
 # Imports #
 ###########
 
 # Standard library imports
+from io import StringIO
 import os
 from pathlib import Path
 import pandas as pd
 
 # Prism imports
+from click.testing import CliRunner
+from prism.main import cli
+from prism.prism_logging import string_stream_handler
 import prism.tests.integration.integration_test_class as integration_test_class
 
 
 #################################
 # Test case directory and paths #
 #################################
 
@@ -38,180 +42,197 @@
     def test_project_no_profile(self):
         """
         `prism spark-submit` on a project without a valid profile throws an error
         """
         self.maxDiff = None
 
         # Set working directory
-        wkdir = Path(TEST_PROJECTS) / '005_simple_project_no_null'
+        wkdir = Path(TEST_PROJECTS) / '005_simple_project_no_null_tasks'
         os.chdir(wkdir)
 
+        # Update logger streamer
+        new_streamer = StringIO()
+        string_stream_handler.setStream(new_streamer)
+
         # Remove the .compiled directory, if it exists
         self._remove_compiled_dir(wkdir)
 
         # # Remove all files in the output directory
         self._remove_files_in_output(wkdir)
 
         # Execute command.
         args = ['spark-submit']
         self._run_prism(args)
-        self.assertFalse(Path(wkdir / 'output' / 'module01.txt').is_file())
-        self.assertFalse(Path(wkdir / 'output' / 'module02.txt').is_file())
+        self.assertFalse(Path(wkdir / 'output' / 'task01.txt').is_file())
+        self.assertFalse(Path(wkdir / 'output' / 'task02.txt').is_file())
 
-        # Execute run command to re-create module outputs
+        # Execute run command to re-create task outputs
         args = ['run']
         self._run_prism(args)
         self._remove_compiled_dir(wkdir)
 
         # Set up wkdir for the next test case
         self._set_up_wkdir()
 
-    def test_spark_project_all_modules(self):
+    def test_spark_project_all_tasks(self):
         """
-        `prism spark-submit` with all modules
+        `prism spark-submit` with all tasks
         """
         self.maxDiff = None
 
         # Set working directory
         wkdir = Path(TEST_PROJECTS) / '007_spark_project'
         os.chdir(wkdir)
 
+        # Update logger streamer
+        new_streamer = StringIO()
+        string_stream_handler.setStream(new_streamer)
+
         # Remove the .compiled directory, if it exists
         self._remove_compiled_dir(wkdir)
 
         # Remove all files in the output directory
         self._remove_dirs_in_output(wkdir)
 
         # Execute spark-submit command
         args = ['spark-submit']
         self._run_prism(args)
 
         # Check manifest
         self.assertTrue(Path(wkdir / '.compiled').is_dir())
         self.assertTrue(Path(wkdir / '.compiled' / 'manifest.json').is_file())
         manifest = self._load_manifest(Path(wkdir / '.compiled' / 'manifest.json'))
-        module01_refs = self._load_module_refs("module01.py", manifest)
-        module02_refs = self._load_module_refs("module02.py", manifest)
-        module03_refs = self._load_module_refs("module03.py", manifest)
-        module04_refs = self._load_module_refs("module04.py", manifest)
-
-        self.assertEqual([], module01_refs)
-        self.assertEqual('module01.py', module02_refs)
-        self.assertEqual('module02.py', module03_refs)
-        self.assertEqual('module03.py', module04_refs)
+        task01_refs = self._load_task_refs("module01", "Task01", manifest)
+        task02_refs = self._load_task_refs("module02", "Task02", manifest)
+        task03_refs = self._load_task_refs("module03", "Task03", manifest)
+        task04_refs = self._load_task_refs("module04", "Task04", manifest)
+
+        self.assertEqual([], task01_refs)
+        self.assertEqual(['module01.Task01'], task02_refs)
+        self.assertEqual(['module02.Task02'], task03_refs)
+        self.assertEqual(['module03.Task03'], task04_refs)
+
+        # Check output
+        self.assertTrue(Path(wkdir / 'output' / 'task01').is_dir())
+        self.assertTrue(Path(wkdir / 'output' / 'task02').is_dir())
+        self.assertTrue(Path(wkdir / 'output' / 'task04').is_dir())
 
         # Set up wkdir for the next test case
         self._set_up_wkdir()
 
         # Remove the .compiled directory, if it exists
         self._remove_compiled_dir(wkdir)
 
         # Remove all files in the output directory (to avoid having to commit and
         # re-commit to Github)
         self._remove_dirs_in_output(wkdir)
 
     def test_spark_project_subset(self):
         """
-        `prism spark-submit` on a subset of modules at a time
+        `prism spark-submit` on a subset of tasks at a time
         """
         self.maxDiff = None
 
         # Set working directory
         wkdir = Path(TEST_PROJECTS) / '007_spark_project'
         os.chdir(wkdir)
 
+        # Update logger streamer
+        new_streamer = StringIO()
+        string_stream_handler.setStream(new_streamer)
+
         # Remove the .compiled directory, if it exists
         self._remove_compiled_dir(wkdir)
 
         # Remove all files in the output directory
         self._remove_dirs_in_output(wkdir)
 
         # ***************** #
-        # Run only module 1 #
+        # Run only task 1 #
         # ***************** #
 
-        # Expecatation: module 1 is the first module in the DAG. Therefore, we should
+        # Expecatation: task 1 is the first task in the DAG. Therefore, we should
         # not encounter any errors with this command.
-        args = ['spark-submit', '--module', 'module01.py']
+        args = ['spark-submit', '--task', 'module01']
         self._run_prism(args)
 
         # Check manifest
         self.assertTrue(Path(wkdir / '.compiled').is_dir())
         self.assertTrue(Path(wkdir / '.compiled' / 'manifest.json').is_file())
         manifest = self._load_manifest(Path(wkdir / '.compiled' / 'manifest.json'))
-        module01_refs = self._load_module_refs("module01.py", manifest)
-        module02_refs = self._load_module_refs("module02.py", manifest)
-        module03_refs = self._load_module_refs("module03.py", manifest)
-        module04_refs = self._load_module_refs("module04.py", manifest)
-
-        self.assertEqual([], module01_refs)
-        self.assertEqual('module01.py', module02_refs)
-        self.assertEqual('module02.py', module03_refs)
-        self.assertEqual('module03.py', module04_refs)
+        task01_refs = self._load_task_refs("module01", "Task01", manifest)
+        task02_refs = self._load_task_refs("module02", "Task02", manifest)
+        task03_refs = self._load_task_refs("module03", "Task03", manifest)
+        task04_refs = self._load_task_refs("module04", "Task04", manifest)
+
+        self.assertEqual([], task01_refs)
+        self.assertEqual(['module01.Task01'], task02_refs)
+        self.assertEqual(['module02.Task02'], task03_refs)
+        self.assertEqual(['module03.Task03'], task04_refs)
 
         # Check the results of the output directory
-        self.assertTrue(Path(wkdir / 'output' / 'module01').is_dir())
-        self.assertFalse(Path(wkdir / 'output' / 'module02').is_dir())
-        module01_df = pd.read_parquet(Path(wkdir / 'output' / 'module01'))
-        self.assertEqual(['col1', 'col2', 'col3'], list(module01_df.columns))
-        self.assertEqual('col1_value1', module01_df['col1'][0])
+        self.assertTrue(Path(wkdir / 'output' / 'task01').is_dir())
+        self.assertFalse(Path(wkdir / 'output' / 'task02').is_dir())
+        task01_df = pd.read_parquet(Path(wkdir / 'output' / 'task01'))
+        self.assertEqual(['col1', 'col2', 'col3'], list(task01_df.columns))
+        self.assertEqual('col1_value1', task01_df['col1'][0])
 
         # **************** #
-        # Execute module 2 #
+        # Execute task 2 #
         # **************** #
 
-        # Expecatation: module 2 depends on module 1. However, since we just ran module
-        # 1, and the output of module 1 is stored in a target, we do not need to re-run
-        # module 1 in order to run module 2. Therefore, we should not encounter any
+        # Expecatation: task 2 depends on task 1. However, since we just ran task
+        # 1, and the output of task 1 is stored in a target, we do not need to re-run
+        # task 1 in order to run task 2. Therefore, we should not encounter any
         # errors with this command.
-        args = ['spark-submit', '--module', 'module02.py']
+        args = ['spark-submit', '--task', 'module02']
         self._run_prism(args)
 
         # Check the results of the output directory
-        self.assertTrue(Path(wkdir / 'output' / 'module01').is_dir())
-        self.assertTrue(Path(wkdir / 'output' / 'module02').is_dir())
-        module02_df = pd.read_parquet(Path(wkdir / 'output' / 'module02'))
-        self.assertEqual(['col1', 'col2', 'col3'], list(module02_df.columns))
-        self.assertEqual(5, module02_df.shape[0])
-        module02_df.sort_values(by='col1', inplace=True)
-        module02_df.reset_index(inplace=True)
-        module02_df.drop(columns=['index'], inplace=True)
-        self.assertEqual('col1_value2', module02_df['col1'][0])
+        self.assertTrue(Path(wkdir / 'output' / 'task01').is_dir())
+        self.assertTrue(Path(wkdir / 'output' / 'task02').is_dir())
+        task02_df = pd.read_parquet(Path(wkdir / 'output' / 'task02'))
+        self.assertEqual(['col1', 'col2', 'col3'], list(task02_df.columns))
+        self.assertEqual(5, task02_df.shape[0])
+        task02_df.sort_values(by='col1', inplace=True)
+        task02_df.reset_index(inplace=True)
+        task02_df.drop(columns=['index'], inplace=True)
+        self.assertEqual('col1_value2', task02_df['col1'][0])
 
         # ************************************************* #
-        # Execute module 4 (with and without `all-upstream` #
+        # Execute task 4 (with and without `all-upstream` #
         # ************************************************* #
 
-        # Expectation: module 4 depends on module 3. However, the output of module 3 is
-        # not stored in a target. Therefore, running module 4 without including
+        # Expectation: task 4 depends on task 3. However, the output of task 3 is
+        # not stored in a target. Therefore, running task 4 without including
         # 'all-upstream' should cause an error.
 
         # -------------------------------------
         # Execute command without `all-upstream`
-        args = ['spark-submit', '--module', 'module04.py']
+        args = ['spark-submit', '--task', 'module04']
         self._run_prism(args)
-        self.assertFalse(Path(wkdir / 'output' / 'module04').is_dir())
+        self.assertFalse(Path(wkdir / 'output' / 'task04').is_dir())
 
         # -----------------------------------
         # Execute command with `all-upstream`
-        args = ['spark-submit', '--module', 'module04.py', '--all-upstream']
+        args = ['spark-submit', '--task', 'module04', '--all-upstream']
         self._run_prism(args)
-        self.assertTrue(Path(wkdir / 'output' / 'module04').is_dir())
-        module04_df = pd.read_parquet(Path(wkdir / 'output' / 'module04'))
-        self.assertEqual(['col1', 'col2', 'col3'], list(module04_df.columns))
-        self.assertEqual(3, module04_df.shape[0])
-        module04_df.sort_values(by='col1', inplace=True)
-        module04_df.reset_index(inplace=True)
-        module04_df.drop(columns=['index'], inplace=True)
-        self.assertEqual('col1_value4', module04_df['col1'][0])
+        self.assertTrue(Path(wkdir / 'output' / 'task04').is_dir())
+        task04_df = pd.read_parquet(Path(wkdir / 'output' / 'task04'))
+        self.assertEqual(['col1', 'col2', 'col3'], list(task04_df.columns))
+        self.assertEqual(3, task04_df.shape[0])
+        task04_df.sort_values(by='col1', inplace=True)
+        task04_df.reset_index(inplace=True)
+        task04_df.drop(columns=['index'], inplace=True)
+        self.assertEqual('col1_value4', task04_df['col1'][0])
 
         # Remove parquet files from outputs (to avoid re-comitting to Github)
-        self._remove_parquet_files_in_dir(Path(wkdir / 'output' / 'module01'))
-        self._remove_parquet_files_in_dir(Path(wkdir / 'output' / 'module02'))
-        self._remove_parquet_files_in_dir(Path(wkdir / 'output' / 'module04'))
+        self._remove_parquet_files_in_dir(Path(wkdir / 'output' / 'task01'))
+        self._remove_parquet_files_in_dir(Path(wkdir / 'output' / 'task02'))
+        self._remove_parquet_files_in_dir(Path(wkdir / 'output' / 'task04'))
 
         # Remove the .compiled directory, if it exists
         self._remove_compiled_dir(wkdir)
 
         # Set up wkdir for next tst
         self._set_up_wkdir()
 
@@ -221,81 +242,124 @@
         """
         self.maxDiff = None
 
         # Set working directory
         wkdir = Path(TEST_PROJECTS) / '007_spark_project'
         os.chdir(wkdir)
 
+        # Update logger streamer
+        new_streamer = StringIO()
+        string_stream_handler.setStream(new_streamer)
+
         # Remove the .compiled directory, if it exists
         self._remove_compiled_dir(wkdir)
 
         # Remove all files in the output directory
         self._remove_dirs_in_output(wkdir)
 
-        # Run all modules downstream of module01.py
-        args = ['spark-submit', '--module', 'module01.py', '--all-downstream']
+        # Run all tasks downstream of module01.py
+        args = ['spark-submit', '--task', 'module01', '--all-downstream']
         self._run_prism(args)
 
         # Check manifest
         self.assertTrue(Path(wkdir / '.compiled').is_dir())
         self.assertTrue(Path(wkdir / '.compiled' / 'manifest.json').is_file())
         manifest = self._load_manifest(Path(wkdir / '.compiled' / 'manifest.json'))
-        module01_refs = self._load_module_refs("module01.py", manifest)
-        module02_refs = self._load_module_refs("module02.py", manifest)
-        module03_refs = self._load_module_refs("module03.py", manifest)
-        module04_refs = self._load_module_refs("module04.py", manifest)
-
-        self.assertEqual([], module01_refs)
-        self.assertEqual('module01.py', module02_refs)
-        self.assertEqual('module02.py', module03_refs)
-        self.assertEqual('module03.py', module04_refs)
+        task01_refs = self._load_task_refs("module01", "Task01", manifest)
+        task02_refs = self._load_task_refs("module02", "Task02", manifest)
+        task03_refs = self._load_task_refs("module03", "Task03", manifest)
+        task04_refs = self._load_task_refs("module04", "Task04", manifest)
+
+        self.assertEqual([], task01_refs)
+        self.assertEqual(['module01.Task01'], task02_refs)
+        self.assertEqual(['module02.Task02'], task03_refs)
+        self.assertEqual(['module03.Task03'], task04_refs)
 
         # ------------------------------------------------------------------------------
         # Check the results of the output directory
 
         # ------------------
         # Output files exist
-        self.assertTrue(Path(wkdir / 'output' / 'module01').is_dir())
-        self.assertTrue(Path(wkdir / 'output' / 'module02').is_dir())
-        self.assertTrue(Path(wkdir / 'output' / 'module04').is_dir())
+        self.assertTrue(Path(wkdir / 'output' / 'task01').is_dir())
+        self.assertTrue(Path(wkdir / 'output' / 'task02').is_dir())
+        self.assertTrue(Path(wkdir / 'output' / 'task04').is_dir())
 
         # Output structure are what we expect
-        module01_df = pd.read_parquet(Path(wkdir / 'output' / 'module01'))
-        module02_df = pd.read_parquet(Path(wkdir / 'output' / 'module02'))
-        module04_df = pd.read_parquet(Path(wkdir / 'output' / 'module04'))
-        self.assertEqual(['col1', 'col2', 'col3'], list(module01_df.columns))
-        self.assertEqual(['col1', 'col2', 'col3'], list(module02_df.columns))
-        self.assertEqual(['col1', 'col2', 'col3'], list(module04_df.columns))
+        task01_df = pd.read_parquet(Path(wkdir / 'output' / 'task01'))
+        task02_df = pd.read_parquet(Path(wkdir / 'output' / 'task02'))
+        task04_df = pd.read_parquet(Path(wkdir / 'output' / 'task04'))
+        self.assertEqual(['col1', 'col2', 'col3'], list(task01_df.columns))
+        self.assertEqual(['col1', 'col2', 'col3'], list(task02_df.columns))
+        self.assertEqual(['col1', 'col2', 'col3'], list(task04_df.columns))
 
         # ----------------------------------
         # Output contents are what we expect
 
-        # Module 1
-        self.assertEqual('col1_value1', module01_df['col1'][0])
-        self.assertEqual(5, module02_df.shape[0])
-
-        # Module 2
-        module02_df.sort_values(by='col1', inplace=True)
-        module02_df.reset_index(inplace=True)
-        module02_df.drop(columns=['index'], inplace=True)
-        self.assertEqual('col1_value2', module02_df['col1'][0])
-
-        # Module 4
-        self.assertEqual(3, module04_df.shape[0])
-        module04_df.sort_values(by='col1', inplace=True)
-        module04_df.reset_index(inplace=True)
-        module04_df.drop(columns=['index'], inplace=True)
-        self.assertEqual('col1_value4', module04_df['col1'][0])
+        # Task 1
+        self.assertEqual('col1_value1', task01_df['col1'][0])
+        self.assertEqual(5, task02_df.shape[0])
+
+        # Task 2
+        task02_df.sort_values(by='col1', inplace=True)
+        task02_df.reset_index(inplace=True)
+        task02_df.drop(columns=['index'], inplace=True)
+        self.assertEqual('col1_value2', task02_df['col1'][0])
+
+        # Task 4
+        self.assertEqual(3, task04_df.shape[0])
+        task04_df.sort_values(by='col1', inplace=True)
+        task04_df.reset_index(inplace=True)
+        task04_df.drop(columns=['index'], inplace=True)
+        self.assertEqual('col1_value4', task04_df['col1'][0])
+
+        # ----------------------------------
+        # Cleanup
+
+        # Remove parquet files from outputs (to avoid re-comitting to Github)
+        self._remove_parquet_files_in_dir(Path(wkdir / 'output' / 'task01'))
+        self._remove_parquet_files_in_dir(Path(wkdir / 'output' / 'task02'))
+        self._remove_parquet_files_in_dir(Path(wkdir / 'output' / 'task04'))
+
+        # Remove the .compiled directory, if it exists
+        self._remove_compiled_dir(wkdir)
+
+        # Set up wkdir for next test
+        self._set_up_wkdir()
+
+    def test_py_in_task_arg(self):
+        """
+        If `.py` is included in a `--task` arg with `prism spark-submit`, Prism throws
+        a warning
+        """
+        self.maxDiff = None
+
+        # Set working directory
+        wkdir = Path(TEST_PROJECTS) / '007_spark_project'
+        os.chdir(wkdir)
+
+        # Remove the .compiled directory, if it exists
+        self._remove_compiled_dir(wkdir)
+
+        # Remove all files in the output directory
+        self._remove_dirs_in_output(wkdir)
+
+        # Run all tasks downstream of module01.py
+        args = ['spark-submit', '--task', 'module01.py', '--all-downstream']
+        runner = CliRunner()
+        result = runner.invoke(cli, args)
+        expected_msg = "ArgumentWarning: `.py` in --task arguments will be an error in a future version of Prism.\n"  # noqa: E501
+        self.assertEqual(expected_msg, result.output)
+        self.assertEqual(0, result.exit_code)
 
         # ----------------------------------
         # Cleanup
 
         # Remove parquet files from outputs (to avoid re-comitting to Github)
-        self._remove_parquet_files_in_dir(Path(wkdir / 'output' / 'module01'))
-        self._remove_parquet_files_in_dir(Path(wkdir / 'output' / 'module02'))
-        self._remove_parquet_files_in_dir(Path(wkdir / 'output' / 'module04'))
+        self._remove_parquet_files_in_dir(Path(wkdir / 'output' / 'task01'))
+        self._remove_parquet_files_in_dir(Path(wkdir / 'output' / 'task02'))
+        self._remove_parquet_files_in_dir(Path(wkdir / 'output' / 'task04'))
 
         # Remove the .compiled directory, if it exists
         self._remove_compiled_dir(wkdir)
 
         # Set up wkdir for next test
         self._set_up_wkdir()
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/integration/test_targets.py` & `prism-ds-0.2.0rc2/prism/tests/integration/test_targets.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,29 +41,36 @@
         """
         self.maxDiff = None
 
         # Set working directory
         wkdir = Path(TEST_PROJECTS) / '008_targets'
         os.chdir(wkdir)
 
-        # Remove all compiled modules
+        # Remove all compiled tasks
         self._remove_compiled_dir(wkdir)
 
         # Remove all folders / files in the output directory
         self._remove_dirs_in_output(wkdir)
         self._remove_files_in_output(wkdir)
 
         # Execute command.
         args = ['spark-submit']
         _ = self._run_prism(args)
         self.assertTrue(Path(wkdir / '.compiled').is_dir())
         self.assertTrue(Path(wkdir / '.compiled' / 'manifest.json').is_file())
         manifest = self._load_manifest(Path(wkdir / '.compiled' / 'manifest.json'))
-        for module in ['parquet.py', 'txt.py', 'csv.py', 'csv_mult.py']:
-            refs = self._load_module_refs(module, manifest)
+        for module_name, task_name in zip(
+            ['parquet.py', 'txt.py', 'csv.py', 'csv_mult.py', 'csv_iter.py'],
+            ["ParquetTask", "TxtTask", "BasicCsvTask", "MultipleCsvsTask", "CsvIteratorTask"]  # noqa: E501
+        ):
+            refs = self._load_task_refs(
+                module_name=module_name,
+                task_name=task_name,
+                manifest=manifest,
+            )
             self.assertEqual([], refs)
 
         # Check contents of output
 
         # Parquet target
         target_parquet_df = pd.read_parquet(Path(wkdir / 'output' / 'target_parquet'))
         expected_df = pd.DataFrame({
@@ -128,12 +135,12 @@
         self.assertTrue(target_csv_iter_df1.equals(expected_df1))
         self.assertTrue(target_csv_iter_df2.equals(expected_df2))
 
         # Remove all files in the output directory (to avoid having to commit and
         # re-commit to Github)
         self._remove_parquet_files_in_dir(Path(wkdir / 'output' / 'target_parquet'))
 
-        # Remove all compiled modules
+        # Remove all compiled tasks
         self._remove_compiled_dir(wkdir)
 
         # Set up wkdir for next test
         self._set_up_wkdir()
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/unit/test_adapter_profile.py` & `prism-ds-0.2.0rc2/prism/tests/unit/test_adapter_profile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/tests/unit/test_agent/prism_project.py` & `prism-ds-0.2.0rc2/prism/templates/starter_project/prism_project.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,51 +5,51 @@
 # Imports
 from prism.admin import generate_run_id, generate_run_slug
 import logging
 from pathlib import Path
 
 
 # Project metadata
-NAME = "Docker agent test"
+NAME = ""
 AUTHOR = ""
 VERSION = ""
 DESCRIPTION = """
 """
 
 # Admin
 RUN_ID = generate_run_id()
 SLUG = generate_run_slug()
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
-    Path(__file__).parent.parent / 'test_trigger_yml'
+    # Add more paths here!
 ]
 
 
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
 # then 1 task is run at a time.
 THREADS = 1
 
 
 # Profile directory and name
-PROFILE_YML_PATH = Path(__file__).parent / 'paths_test' / 'profile.yml'
-PROFILE = "profile_agent_test"
+PROFILE_YML_PATH = Path(__file__).parent / 'profile.yml'
+PROFILE = "default"
 
 
 # Logger
 PRISM_LOGGER = logging.getLogger("PRISM_LOGGER")
 
 
 # Triggers
-TRIGGERS_YML_PATH = Path(__file__).parent.parent / 'test_trigger_yml' / 'triggers.yml'
+TRIGGERS_YML_PATH = Path(__file__).parent / 'triggers.yml'
 TRIGGERS = {
-    'on_success': ["test_agent_trigger"],
+    'on_success': [],
     'on_failure': [],
 }
 
 
 # Other variables / parameters. Make sure to capitalize all of these!
 VAR_1 = {'a': 'b'}
 VAR_2 = 200
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/unit/test_agents.py` & `prism-ds-0.2.0rc2/prism/tests/unit/test_agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from prism.agents.docker_agent import Docker
 import prism.constants
 import prism.exceptions
 
 
 # Skip these tests if we're running in Windows.
 if sys.platform.startswith("win"):
-    pytest.skip("Skipping agent tests on Windows", allow_module_level=True)
+    pytest.skip("Skipping agent tests on Windows", allow_task_level=True)
 
 
 #################################
 # Test case directory and paths #
 #################################
 
 # Directory containing all prism_project.py test cases
@@ -53,15 +53,14 @@
 
 # Prism proejct
 project = PrismProject(
     project_dir=TEST_AGENT,
     user_context={},
     which="agent-run"
 )
-project.setup()
 
 
 ##################
 # Util functions #
 ##################
 
 # Agent objects
@@ -97,14 +96,22 @@
 
 ##############################
 # Test case class definition #
 ##############################
 
 class TestAgent(unittest.TestCase):
 
+    @classmethod
+    def setUpClass(cls) -> None:
+        project.setup()
+
+    @classmethod
+    def tearDownClass(cls) -> None:
+        project.cleanup(project.run_context)
+
     def test_valid_docker_agent_yml_conf(self):
         """
         A valid agent YAML configuration is loaded as expected
         """
         _create_valid_docker_agent()
         _remove_logs()
 
@@ -298,11 +305,7 @@
         agent = _create_valid_docker_agent()
         self.assertEqual(
             {"env_var_1": "value1"},
             agent.parse_environment_variables(agent.agent_conf),
         )
 
         _remove_logs()
-
-
-# Cleanup
-project.cleanup(project.run_context)
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/unit/test_jinja.py` & `prism-ds-0.2.0rc2/prism/tests/unit/test_jinja.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/tests/unit/test_prism_project_py/bad_trigger_key.py` & `prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # Imports
 import os
 import logging
 from pathlib import Path
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
     Path(__file__).parent.parent,
 ]
 
 
@@ -40,11 +40,9 @@
 DATA = WKDIR / 'data'
 OUTPUT = WKDIR / 'output'
 
 
 # Triggers
 TRIGGERS_YML_PATH = Path(__file__).parent / 'triggers.yml'  # location of `triggers.yml` file
 TRIGGERS = {
-    'on_success': ["test_fn"],
     'on_failure': ["test_fn"],
-    'this_key_should_not_exist': [],
 }
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/unit/test_prism_project_py/multiple_profiles.py` & `prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/multiple_profiles.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/tests/unit/test_prism_project_py/no_profile.py` & `prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/no_profile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/tests/unit/test_prism_project_py/non_null_profile.py` & `prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/non_null_profile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/tests/unit/test_prism_project_py/null_profile.py` & `prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/null_profile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py` & `prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/bad_trigger_key.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # Imports
 import os
 import logging
 from pathlib import Path
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
     Path(__file__).parent.parent,
 ]
 
 
@@ -40,9 +40,11 @@
 DATA = WKDIR / 'data'
 OUTPUT = WKDIR / 'output'
 
 
 # Triggers
 TRIGGERS_YML_PATH = Path(__file__).parent / 'triggers.yml'  # location of `triggers.yml` file
 TRIGGERS = {
+    'on_success': ["test_fn"],
     'on_failure': ["test_fn"],
+    'this_key_should_not_exist': [],
 }
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py` & `prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # Imports
 import os
 import logging
 from pathlib import Path
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
     Path(__file__).parent.parent,
 ]
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/unit/test_prism_project_py/triggers_normal.py` & `prism-ds-0.2.0rc2/prism/tests/unit/test_prism_project_py/triggers_normal.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # Imports
 import os
 import logging
 from pathlib import Path
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
     Path(__file__).parent,
     Path(__file__).parent.parent,
 ]
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/unit/test_project.py` & `prism-ds-0.2.0rc2/prism/tests/unit/test_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,16 +67,16 @@
                 user_context={},
                 which="run",
                 filename=filename
             )
 
     def test_non_null_profile(self):
         """
-        The run task uses the AST module to extract the profile variable from the
-        prism_project.py file without executing it. Confirm that this module extracts a
+        The run task uses the AST task to extract the profile variable from the
+        prism_project.py file without executing it. Confirm that this task extracts a
         non-null profile correctly.
         """
         prism_project = project.PrismProject(
             project_dir=PRISM_PROJECT_PY_TEST_CASES,
             user_context={},
             which="run",
             filename=NON_NULL_PROFILE
@@ -150,15 +150,15 @@
         run_context = {}
         prism_project = project.PrismProject(
             project_dir=PRISM_PROJECT_PY_TEST_CASES,
             user_context={},
             which="run",
             filename=TRIGGERS_NORMAL
         )
-        engine = SysPathEngine(run_context)
+        engine = SysPathEngine(run_context, prism_project.project_dir)
         prism_project.exec(run_context, engine)
 
         # Triggers directory
         triggers_yml_path = prism_project.get_triggers_yml_path(run_context)
         self.assertEqual(
             str(triggers_yml_path),
             str(PRISM_PROJECT_PY_TEST_CASES / 'triggers.yml')
@@ -168,70 +168,78 @@
         triggers = prism_project.get_triggers(run_context)
         expected_triggers = {
             "on_success": ['test_fn'],
             "on_failure": ['test_fn'],
         }
         self.assertEqual(triggers, expected_triggers)
 
+        engine.remove_sys_path(prism_project.project_dir, run_context)
+
     def test_on_failure_triggers_only(self):
         """
         on_success triggers is an empty list when not defined
         """
         run_context = {}
         prism_project = project.PrismProject(
             project_dir=PRISM_PROJECT_PY_TEST_CASES,
             user_context={},
             which="run",
             filename=ON_FAILURE_TRIGGERS_ONLY
         )
-        engine = SysPathEngine(run_context)
+        engine = SysPathEngine(run_context, prism_project.project_dir)
         prism_project.exec(run_context, engine)
 
         # Triggers
         triggers = prism_project.get_triggers(run_context)
         expected_triggers = {
             "on_success": [],
             "on_failure": ['test_fn'],
         }
         self.assertEqual(triggers, expected_triggers)
 
+        engine.remove_sys_path(prism_project.project_dir, run_context)
+
     def test_on_success_triggers_only(self):
         """
         on_failure triggers is an empty list when not defined
         """
         run_context = {}
         prism_project = project.PrismProject(
             project_dir=PRISM_PROJECT_PY_TEST_CASES,
             user_context={},
             which="run",
             filename=ON_SUCCESS_TRIGGERS_ONLY
         )
-        engine = SysPathEngine(run_context)
+        engine = SysPathEngine(run_context, prism_project.project_dir)
         prism_project.exec(run_context, engine)
 
         # Triggers
         triggers = prism_project.get_triggers(run_context)
         expected_triggers = {
             "on_success": ['test_fn'],
             "on_failure": [],
         }
         self.assertEqual(triggers, expected_triggers)
 
+        engine.remove_sys_path(prism_project.project_dir, run_context)
+
     def test_bad_trigger_key(self):
         """
         on_failure triggers is an empty list when not defined
         """
         run_context = {}
         prism_project = project.PrismProject(
             project_dir=PRISM_PROJECT_PY_TEST_CASES,
             user_context={},
             which="run",
             filename=BAD_TRIGGER_KEY
         )
-        engine = SysPathEngine(run_context)
+        engine = SysPathEngine(run_context, prism_project.project_dir)
         prism_project.exec(run_context, engine)
 
         # Triggers
         with self.assertRaises(prism.exceptions.InvalidProjectPyException) as cm:
             prism_project.get_triggers(run_context)
         expected_msg = 'invalid key `this_key_should_not_exist` in TRIGGERS dictionary'
         self.assertEqual(str(cm.exception), expected_msg)
+
+        engine.remove_sys_path(prism_project.project_dir, run_context)
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/unit/test_trigger.py` & `prism-ds-0.2.0rc2/prism/tests/unit/test_trigger.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 # Prism project object
 prism_project = PrismProject(
     project_dir=TEST_TRIGGER_YML,
     user_context={},
     which="run",
     filename="prism_project.py"
 )
-prism_project.setup()
 
 
 ###################
 # Helper function #
 ###################
 
 def _load_yml_spec(yml_path: Path, trigger_name: str):
@@ -67,14 +66,22 @@
 
 ##############################
 # Test case class definition #
 ##############################
 
 class TestTrigger(unittest.TestCase):
 
+    @classmethod
+    def setUpClass(cls) -> None:
+        prism_project.setup()
+
+    @classmethod
+    def tearDownClass(cls) -> None:
+        prism_project.cleanup(prism_project.run_context)
+
     def test_triggers(self):
         """
         Normal trigger structure
         """
         # The trigger instantiation should confirm that the trigger is the correct
         # structure.
         trigger_name = "test_trigger_good_structure"
@@ -195,34 +202,32 @@
         ])
         self.assertEqual(expected_message, str(cm.exception))
 
     def test_sys_path(self):
         """
         Paths in `include` are added to the Prism project's sys.path.config
         """
+
         # Path of interest
-        DUMMY_MODULES = Path(TEST_CASE_WKDIR) / 'dummy_modules'
-        print(prism_project.run_context['sys'].path)
+        DUMMY_TASKS = Path(TEST_CASE_WKDIR) / 'dummy_tasks'
 
-        # In `prism_project.py`, we have `Path(__file__).parent` in `SYS_PATH_CONFIG`.
-        # Therefore, `test_trigger_yml` should be in the project's sys.path.
-        self.assertTrue(str(TEST_TRIGGER_YML) in prism_project.run_context['sys'].path)
-        self.assertFalse(str(DUMMY_MODULES) in prism_project.run_context['sys'].path)
+        # Now, it should appear in our project's sys.path
+        self.assertFalse(str(DUMMY_TASKS) in prism_project.run_context['sys'].path)
 
         # Create the TriggerManager
         manager = TriggerManager(
             triggers_yml_path=TRIGGERS_YML_EXTERNAL_INCLUDE,
             prism_project=prism_project
         )
         manager.check_trigger_components(prism_project.run_context)
-        self.assertTrue(str(DUMMY_MODULES) in prism_project.run_context['sys'].path)
+        self.assertTrue(str(DUMMY_TASKS) in prism_project.run_context['sys'].path)
 
         # Cleanup
         prism_project.cleanup(prism_project.run_context)
-        self.assertFalse(str(DUMMY_MODULES) in prism_project.run_context['sys'].path)
+        self.assertFalse(str(DUMMY_TASKS) in prism_project.run_context['sys'].path)
 
         # The original project directory was also removed
         self.assertFalse(str(TEST_TRIGGER_YML) in prism_project.run_context['sys'].path)
 
     def test_trigger_import_statement(self):
         """
         The `import_function` function produces the expected import statement to
@@ -240,11 +245,7 @@
             'test_trigger_good_structure',
             yml,
             {},
             "test"
         )
         expected_import_statement = "import test_fn"
         self.assertEqual(expected_import_statement, actual_import_statement)
-
-
-# Cleanup
-prism_project.cleanup(prism_project.run_context)
```

### Comparing `prism-ds-0.2.0rc1/prism/tests/unit/test_trigger_yml/prism_project.py` & `prism-ds-0.2.0rc2/prism/tests/unit/test_trigger_yml/prism_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 # Imports
 import os
 import logging
 from pathlib import Path
 from prism.admin import generate_run_id, generate_run_slug
 
 
-# sys.path config. This gives your tasks access to local modules / packages that exist
+# sys.path config. This gives your tasks access to local tasks / packages that exist
 # outside of your project structure.
 SYS_PATH_CONF = [
-    Path(__file__).parent,
+    Path(__file__).parent.parent,
 ]
 
 # Run ID and slug
 RUN_ID = generate_run_id()
 SLUG = generate_run_slug()
 
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
```

### Comparing `prism-ds-0.2.0rc1/prism/triggers/__init__.py` & `prism-ds-0.2.0rc2/prism/triggers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,16 +118,16 @@
     def import_function(self,
         trigger_name: str,
         trigger_spec: Dict[Any, Any],
         run_context: Dict[Any, Any],
         mode="prod"
     ) -> Optional[str]:
         """
-        For function triggers, we may need to import the function from a module. Note
-        that the user must ensure that the path to that module is contained in
+        For function triggers, we may need to import the function from a task. Note
+        that the user must ensure that the path to that task is contained in
         SYS_PATH_CONF.
 
         args:
             trigger_name: name of trigger
             trigger_spec: trigger as a dictionary
             run_context: dictionary with run context variables
         returns:
@@ -139,19 +139,19 @@
                 message=f"trigger `{trigger_name}` is not of type `function`"
             )
 
         # Since it's of type function, we know that the spec will have a key `function`
         fn = trigger_spec["function"]
         fn_split = fn.split('.')
 
-        # There must be a parent module specified. If there isn't, then something is
+        # There must be a parent task specified. If there isn't, then something is
         # wrong.
         if len(fn_split) == 1:
             raise prism.exceptions.RuntimeException(
-                message=f"no parent module specified for trigger `{trigger_name}`"
+                message=f"no parent task specified for trigger `{trigger_name}`"
             )
         else:
             if mode == "prod":
                 exec(f"import {'.'.join(fn_split[:-1])}", run_context)
                 return None
             else:
                 return f"import {'.'.join(fn_split[:-1])}"
```

### Comparing `prism-ds-0.2.0rc1/prism/ui.py` & `prism-ds-0.2.0rc2/prism/ui.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/prism_ds.egg-info/PKG-INFO` & `prism-ds-0.2.0rc2/prism_ds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prism-ds
-Version: 0.2.0rc1
+Version: 0.2.0rc2
 Summary: The easiest way to create data pipelines in Python.
 Author: prism founders
 Author-email: hello@runprism.com
 License: Apache-2.0
 Project-URL: homepage, https://www.runprism.com
 Project-URL: documentation, https://docs.runprism.com
 Project-URL: repository, https://github.com/runprism/prism
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prism-ds Version: 0.2.0rc1 Summary: The easiest way
+Metadata-Version: 2.1 Name: prism-ds Version: 0.2.0rc2 Summary: The easiest way
 to create data pipelines in Python. Author: prism founders Author-email:
 hello@runprism.com License: Apache-2.0 Project-URL: homepage, https://
 www.runprism.com Project-URL: documentation, https://docs.runprism.com Project-
 URL: repository, https://github.com/runprism/prism Platform: unix Platform:
 linux Platform: osx Platform: win32 Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `prism-ds-0.2.0rc1/prism_ds.egg-info/requires.txt` & `prism-ds-0.2.0rc2/prism_ds.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/pyproject.toml` & `prism-ds-0.2.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.0rc1/setup.cfg` & `prism-ds-0.2.0rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = prism-ds
 description = The easiest way to create data pipelines in Python.
 long_description_content_type = text/markdown
 long_description = file: README.md
-version = 0.2.0rc1
+version = 0.2.0rc2
 author = prism founders
 author_email = hello@runprism.com
 license = Apache-2.0
 license_file = LICENSE
 platforms = unix, linux, osx, win32
 classifiers = 
 	Programming Language :: Python :: 3
```

