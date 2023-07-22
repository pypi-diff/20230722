# Comparing `tmp/fugue-0.8.6.dev1.tar.gz` & `tmp/fugue-0.8.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fugue-0.8.6.dev1.tar", last modified: Thu Jul 13 06:02:02 2023, max compression
+gzip compressed data, was "fugue-0.8.6.dev2.tar", last modified: Sat Jul 22 18:36:12 2023, max compression
```

## Comparing `fugue-0.8.6.dev1.tar` & `fugue-0.8.6.dev2.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.021720 fugue-0.8.6.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-13 06:02:02.021720 fugue-0.8.6.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:01.997720 fugue-0.8.6.dev1/fugue/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.001720 fugue-0.8.6.dev1/fugue/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/_utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/_utils/interfaceless.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/_utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.001720 fugue-0.8.6.dev1/fugue/bag/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/bag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/bag/array_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/bag/bag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.005720 fugue-0.8.6.dev1/fugue/collections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17248 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/collections/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/collections/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/collections/yielded.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.005720 fugue-0.8.6.dev1/fugue/column/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/column/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/column/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/column/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.009720 fugue-0.8.6.dev1/fugue/dataframe/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/array_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/arrow_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    17247 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/dataframe_iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/dataframes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/pandas_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataframe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.009720 fugue-0.8.6.dev1/fugue/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataset/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.009720 fugue-0.8.6.dev1/fugue/execution/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39818 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/execution/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/execution/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/execution/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13293 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/execution/native_execution_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.009720 fugue-0.8.6.dev1/fugue/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue/extensions/_builtins/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/_builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/_builtins/creators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/_builtins/outputters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/_builtins/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue/extensions/creator/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/creator/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/creator/creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue/extensions/outputter/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/outputter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/outputter/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/outputter/outputter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue/extensions/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/processor/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/processor/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue/extensions/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/transformer/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    23380 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/transformer/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/extensions/transformer/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/rpc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/rpc/flask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/sql/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    33844 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/sql/_visitors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/sql/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/sql/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/workflow/_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/workflow/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/workflow/_workflow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/workflow/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/workflow/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/workflow/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    88219 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.001720 fugue-0.8.6.dev1/fugue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-13 06:02:01.000000 fugue-0.8.6.dev1/fugue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-13 06:02:01.000000 fugue-0.8.6.dev1/fugue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 06:02:01.000000 fugue-0.8.6.dev1/fugue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-13 06:02:01.000000 fugue-0.8.6.dev1/fugue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-13 06:02:01.000000 fugue-0.8.6.dev1/fugue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-13 06:02:01.000000 fugue-0.8.6.dev1/fugue.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue_contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_contrib/contrib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue_contrib/seaborn/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_contrib/seaborn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.013720 fugue-0.8.6.dev1/fugue_contrib/viz/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_contrib/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_contrib/viz/_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_dask/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_dask/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_dask/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_dask/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_dask/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_dask/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_dask/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_dask/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_duckdb/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_duckdb/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_duckdb/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_duckdb/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_duckdb/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_duckdb/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_duckdb/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_ibis/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ibis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ibis/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ibis/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ibis/dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_ibis/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ibis/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ibis/execution/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ibis/execution/pandas_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ibis/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ibis/extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_notebook/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_notebook/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_notebook/nbextension/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_notebook/nbextension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_notebook/nbextension/description.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_notebook/nbextension/main.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_polars/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_polars/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_polars/polars_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_polars/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_ray/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ray/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_ray/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ray/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ray/_utils/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ray/_utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ray/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10577 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ray/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ray/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_ray/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.017720 fugue-0.8.6.dev1/fugue_spark/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.021720 fugue-0.8.6.dev1/fugue_spark/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/_utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/_utils/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    32029 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_spark/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.021720 fugue-0.8.6.dev1/fugue_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_sql/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.021720 fugue-0.8.6.dev1/fugue_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_test/bag_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    76338 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_test/builtin_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    19082 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_test/dataframe_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    50948 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_test/execution_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_test/ibis_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:02:02.021720 fugue-0.8.6.dev1/fugue_version/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/fugue_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-13 06:02:02.021720 fugue-0.8.6.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-13 05:59:41.000000 fugue-0.8.6.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.849341 fugue-0.8.6.dev2/fugue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.853341 fugue-0.8.6.dev2/fugue/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/_utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/_utils/interfaceless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/_utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.853341 fugue-0.8.6.dev2/fugue/bag/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/bag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/bag/array_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/bag/bag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.853341 fugue-0.8.6.dev2/fugue/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17248 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/collections/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/collections/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/collections/yielded.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.853341 fugue-0.8.6.dev2/fugue/column/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/column/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/column/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/column/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/column/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.853341 fugue-0.8.6.dev2/fugue/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/array_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/arrow_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/dataframe_iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/pandas_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataframe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.853341 fugue-0.8.6.dev2/fugue/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataset/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39818 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/execution/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/execution/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/execution/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13293 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/execution/native_execution_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/extensions/_builtins/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/_builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/_builtins/creators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/_builtins/outputters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/_builtins/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/extensions/creator/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/creator/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/creator/creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/extensions/outputter/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/outputter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/outputter/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/outputter/outputter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/extensions/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/processor/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/processor/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/extensions/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/transformer/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23380 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/transformer/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/extensions/transformer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/rpc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/rpc/flask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/sql/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33844 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/sql/_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/sql/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/sql/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.857341 fugue-0.8.6.dev2/fugue/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/workflow/_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/workflow/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/workflow/_workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/workflow/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/workflow/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/workflow/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88219 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.849341 fugue-0.8.6.dev2/fugue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-22 18:36:12.000000 fugue-0.8.6.dev2/fugue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-22 18:36:12.000000 fugue-0.8.6.dev2/fugue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 18:36:12.000000 fugue-0.8.6.dev2/fugue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-22 18:36:12.000000 fugue-0.8.6.dev2/fugue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-22 18:36:12.000000 fugue-0.8.6.dev2/fugue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-22 18:36:12.000000 fugue-0.8.6.dev2/fugue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.861341 fugue-0.8.6.dev2/fugue_contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_contrib/contrib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.861341 fugue-0.8.6.dev2/fugue_contrib/seaborn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_contrib/seaborn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.861341 fugue-0.8.6.dev2/fugue_contrib/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_contrib/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_contrib/viz/_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.861341 fugue-0.8.6.dev2/fugue_dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_dask/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_dask/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_dask/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_dask/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_dask/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_dask/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_dask/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.861341 fugue-0.8.6.dev2/fugue_duckdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_duckdb/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_duckdb/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_duckdb/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_duckdb/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_duckdb/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_duckdb/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_duckdb/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.861341 fugue-0.8.6.dev2/fugue_ibis/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ibis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ibis/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ibis/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ibis/dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.861341 fugue-0.8.6.dev2/fugue_ibis/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ibis/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ibis/execution/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ibis/execution/pandas_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ibis/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ibis/extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.861341 fugue-0.8.6.dev2/fugue_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_notebook/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.861341 fugue-0.8.6.dev2/fugue_notebook/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_notebook/nbextension/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_notebook/nbextension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_notebook/nbextension/description.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_notebook/nbextension/main.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/fugue_polars/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_polars/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_polars/polars_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_polars/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/fugue_ray/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ray/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/fugue_ray/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ray/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ray/_utils/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ray/_utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ray/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10577 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ray/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ray/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_ray/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/fugue_spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/fugue_spark/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/_utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/_utils/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32440 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_spark/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/fugue_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_sql/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/fugue_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_test/bag_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78396 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_test/builtin_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19082 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_test/dataframe_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50948 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_test/execution_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_test/ibis_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 18:36:12.865341 fugue-0.8.6.dev2/fugue_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/fugue_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-22 18:36:12.869341 fugue-0.8.6.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-22 18:33:33.000000 fugue-0.8.6.dev2/setup.py
```

### Comparing `fugue-0.8.6.dev1/LICENSE` & `fugue-0.8.6.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/PKG-INFO` & `fugue-0.8.6.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue
-Version: 0.8.6.dev1
+Version: 0.8.6.dev2
 Summary: An abstraction layer for distributed computation
 Home-page: http://github.com/fugue-project/fugue
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue
```

### Comparing `fugue-0.8.6.dev1/README.md` & `fugue-0.8.6.dev2/README.md`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/__init__.py` & `fugue-0.8.6.dev2/fugue/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/_utils/display.py` & `fugue-0.8.6.dev2/fugue/_utils/display.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/_utils/exception.py` & `fugue-0.8.6.dev2/fugue/_utils/exception.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/_utils/interfaceless.py` & `fugue-0.8.6.dev2/fugue/_utils/interfaceless.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/_utils/io.py` & `fugue-0.8.6.dev2/fugue/_utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/_utils/misc.py` & `fugue-0.8.6.dev2/fugue/_utils/misc.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/api.py` & `fugue-0.8.6.dev2/fugue/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/bag/array_bag.py` & `fugue-0.8.6.dev2/fugue/bag/array_bag.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/bag/bag.py` & `fugue-0.8.6.dev2/fugue/bag/bag.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/collections/partition.py` & `fugue-0.8.6.dev2/fugue/collections/partition.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/collections/sql.py` & `fugue-0.8.6.dev2/fugue/collections/sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/collections/yielded.py` & `fugue-0.8.6.dev2/fugue/collections/yielded.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/column/expressions.py` & `fugue-0.8.6.dev2/fugue/column/expressions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/column/functions.py` & `fugue-0.8.6.dev2/fugue/column/functions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/column/sql.py` & `fugue-0.8.6.dev2/fugue/column/sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/constants.py` & `fugue-0.8.6.dev2/fugue/constants.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/dataframe/__init__.py` & `fugue-0.8.6.dev2/fugue/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/dataframe/api.py` & `fugue-0.8.6.dev2/fugue/dataframe/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/dataframe/array_dataframe.py` & `fugue-0.8.6.dev2/fugue/dataframe/array_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/dataframe/arrow_dataframe.py` & `fugue-0.8.6.dev2/fugue/dataframe/arrow_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/dataframe/dataframe.py` & `fugue-0.8.6.dev2/fugue/dataframe/dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,21 @@
         """
         arr = self.peek_array()
         return {self.columns[i]: arr[i] for i in range(len(self.columns))}
 
     def as_pandas(self) -> pd.DataFrame:
         """Convert to pandas DataFrame"""
         pdf = pd.DataFrame(self.as_array(), columns=self.columns)
+        if len(pdf) == 0:  # TODO: move to triad
+            return pd.DataFrame(
+                {
+                    k: pd.Series(dtype=v.type.to_pandas_dtype())
+                    for k, v in self.schema.items()
+                }
+            )
         return PD_UTILS.enforce_type(pdf, self.schema.pa_schema, null_safe=True)
 
     def as_arrow(self, type_safe: bool = False) -> pa.Table:
         """Convert to pyArrow DataFrame"""
         return pa.Table.from_pandas(
             self.as_pandas().reset_index(drop=True),
             preserve_index=False,
```

### Comparing `fugue-0.8.6.dev1/fugue/dataframe/dataframe_iterable_dataframe.py` & `fugue-0.8.6.dev2/fugue/dataframe/dataframe_iterable_dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         self, columns: Optional[List[str]] = None, type_safe: bool = False
     ) -> Iterable[Any]:
         for df in self.native:
             yield from df.as_array_iterable(columns=columns, type_safe=type_safe)
 
     def as_pandas(self) -> pd.DataFrame:
         if self.empty:
-            return ArrayDataFrame([], self.schema).as_pandas()
+            return PandasDataFrame(schema=self.schema).as_pandas()
 
         return pd.concat(df.as_pandas() for df in self.native)
 
     def as_arrow(self, type_safe: bool = False) -> pa.Table:
         if self.empty:
             return ArrayDataFrame([], self.schema).as_arrow()
```

### Comparing `fugue-0.8.6.dev1/fugue/dataframe/dataframes.py` & `fugue-0.8.6.dev2/fugue/dataframe/dataframes.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/dataframe/function_wrapper.py` & `fugue-0.8.6.dev2/fugue/dataframe/function_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,17 +19,18 @@
     KeywordParam,
     PositionalParam,
     function_wrapper,
 )
 from triad.utils.iter import EmptyAwareIterable, make_empty_aware
 
 from ..constants import FUGUE_ENTRYPOINT
+from ..dataset.api import count as df_count
 from .array_dataframe import ArrayDataFrame
 from .arrow_dataframe import ArrowDataFrame
-from .dataframe import DataFrame, LocalDataFrame
+from .dataframe import AnyDataFrame, DataFrame, LocalDataFrame, as_fugue_df
 from .dataframe_iterable_dataframe import (
     IterableArrowDataFrame,
     IterablePandasDataFrame,
     LocalDataFrameIterableDataFrame,
 )
 from .dataframes import DataFrames
 from .iterable_dataframe import IterableDataFrame
@@ -168,14 +169,27 @@
     def count(self, df: Any) -> int:
         if df.is_bounded:
             return df.count()
         else:
             return sum(1 for _ in df.as_array_iterable())
 
 
+@fugue_annotated_param(AnyDataFrame)
+class _AnyDataFrameParam(DataFrameParam):
+    def to_output_df(self, output: AnyDataFrame, schema: Any, ctx: Any) -> DataFrame:
+        return (
+            as_fugue_df(output)
+            if schema is None
+            else as_fugue_df(output, schema=schema)
+        )
+
+    def count(self, df: Any) -> int:
+        return df_count(df)
+
+
 @fugue_annotated_param(LocalDataFrame, "l", child_can_reuse_code=True)
 class LocalDataFrameParam(DataFrameParam):
     def to_input_data(self, df: DataFrame, ctx: Any) -> LocalDataFrame:
         return df.as_local()
 
     def to_output_df(self, output: LocalDataFrame, schema: Any, ctx: Any) -> DataFrame:
         assert_or_throw(
@@ -329,14 +343,17 @@
 class _PandasParam(LocalDataFrameParam):
     @no_type_check
     def to_input_data(self, df: DataFrame, ctx: Any) -> pd.DataFrame:
         return df.as_pandas()
 
     @no_type_check
     def to_output_df(self, output: pd.DataFrame, schema: Any, ctx: Any) -> DataFrame:
+        _schema: Optional[Schema] = None if schema is None else Schema(schema)
+        if _schema is not None and _schema.names != list(output.columns):
+            output = output[_schema.names]
         return PandasDataFrame(output, schema)
 
     @no_type_check
     def count(self, df: pd.DataFrame) -> int:
         return df.shape[0]
 
     def format_hint(self) -> Optional[str]:
@@ -357,16 +374,23 @@
                 yield sub.as_pandas()
 
     @no_type_check
     def to_output_df(
         self, output: Iterable[pd.DataFrame], schema: Any, ctx: Any
     ) -> DataFrame:
         def dfs():
+            _schema: Optional[Schema] = None if schema is None else Schema(schema)
+            has_return = False
             for df in output:
-                yield PandasDataFrame(df, schema)
+                if _schema is not None and _schema.names != list(df.columns):
+                    df = df[_schema.names]
+                yield PandasDataFrame(df, _schema)
+                has_return = True
+            if not has_return and _schema is not None:
+                yield PandasDataFrame(schema=_schema)
 
         return IterablePandasDataFrame(dfs())
 
     @no_type_check
     def count(self, df: Iterable[pd.DataFrame]) -> int:
         return sum(_.shape[0] for _ in df)
 
@@ -377,15 +401,20 @@
 @fugue_annotated_param(pa.Table)
 class _PyArrowTableParam(LocalDataFrameParam):
     def to_input_data(self, df: DataFrame, ctx: Any) -> Any:
         return df.as_arrow()
 
     def to_output_df(self, output: Any, schema: Any, ctx: Any) -> DataFrame:
         assert isinstance(output, pa.Table)
-        return ArrowDataFrame(output, schema=schema)
+        adf: DataFrame = ArrowDataFrame(output)
+        if schema is not None:
+            _schema = Schema(schema)
+            if adf.schema != _schema:
+                adf = adf[_schema.names].alter_columns(_schema)
+        return adf
 
     def count(self, df: Any) -> int:  # pragma: no cover
         return df.count()
 
     def format_hint(self) -> Optional[str]:
         return "pyarrow"
 
@@ -405,21 +434,23 @@
 
     @no_type_check
     def to_output_df(
         self, output: Iterable[pa.Table], schema: Any, ctx: Any
     ) -> DataFrame:
         def dfs():
             _schema: Optional[Schema] = None if schema is None else Schema(schema)
+            has_return = False
             for df in output:
-                adf = ArrowDataFrame(df)
-                if _schema is not None and not (  # pylint: disable-all
-                    adf.schema == schema
-                ):
+                adf: DataFrame = ArrowDataFrame(df)
+                if _schema is not None and adf.schema != _schema:
                     adf = adf[_schema.names].alter_columns(_schema)
                 yield adf
+                has_return = True
+            if not has_return and _schema is not None:
+                yield ArrowDataFrame(schema=_schema)
 
         return IterableArrowDataFrame(dfs())
 
     @no_type_check
     def count(self, df: Iterable[pa.Table]) -> int:
         return sum(_.shape[0] for _ in df)
```

### Comparing `fugue-0.8.6.dev1/fugue/dataframe/iterable_dataframe.py` & `fugue-0.8.6.dev2/fugue/dataframe/iterable_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/dataframe/pandas_dataframe.py` & `fugue-0.8.6.dev2/fugue/dataframe/pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/dataframe/utils.py` & `fugue-0.8.6.dev2/fugue/dataframe/utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/dataset/api.py` & `fugue-0.8.6.dev2/fugue/dataset/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/dataset/dataset.py` & `fugue-0.8.6.dev2/fugue/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/dev.py` & `fugue-0.8.6.dev2/fugue/dev.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/exceptions.py` & `fugue-0.8.6.dev2/fugue/exceptions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/execution/api.py` & `fugue-0.8.6.dev2/fugue/execution/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/execution/execution_engine.py` & `fugue-0.8.6.dev2/fugue/execution/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/execution/factory.py` & `fugue-0.8.6.dev2/fugue/execution/factory.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/execution/native_execution_engine.py` & `fugue-0.8.6.dev2/fugue/execution/native_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/extensions/__init__.py` & `fugue-0.8.6.dev2/fugue/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/extensions/_builtins/__init__.py` & `fugue-0.8.6.dev2/fugue/extensions/_builtins/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/extensions/_builtins/creators.py` & `fugue-0.8.6.dev2/fugue/extensions/_builtins/creators.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/extensions/_builtins/outputters.py` & `fugue-0.8.6.dev2/fugue/extensions/_builtins/outputters.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/extensions/_builtins/processors.py` & `fugue-0.8.6.dev2/fugue/extensions/_builtins/processors.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/extensions/_utils.py` & `fugue-0.8.6.dev2/fugue/extensions/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/extensions/context.py` & `fugue-0.8.6.dev2/fugue/extensions/context.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/extensions/creator/convert.py` & `fugue-0.8.6.dev2/fugue/extensions/creator/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/extensions/creator/creator.py` & `fugue-0.8.6.dev2/fugue/extensions/creator/creator.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/extensions/outputter/convert.py` & `fugue-0.8.6.dev2/fugue/extensions/outputter/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/extensions/outputter/outputter.py` & `fugue-0.8.6.dev2/fugue/extensions/outputter/outputter.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/extensions/processor/convert.py` & `fugue-0.8.6.dev2/fugue/extensions/processor/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/extensions/processor/processor.py` & `fugue-0.8.6.dev2/fugue/extensions/processor/processor.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/extensions/transformer/convert.py` & `fugue-0.8.6.dev2/fugue/extensions/transformer/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/extensions/transformer/transformer.py` & `fugue-0.8.6.dev2/fugue/extensions/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/plugins.py` & `fugue-0.8.6.dev2/fugue/plugins.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/registry.py` & `fugue-0.8.6.dev2/fugue/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/rpc/base.py` & `fugue-0.8.6.dev2/fugue/rpc/base.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/rpc/flask.py` & `fugue-0.8.6.dev2/fugue/rpc/flask.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/sql/_utils.py` & `fugue-0.8.6.dev2/fugue/sql/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/sql/_visitors.py` & `fugue-0.8.6.dev2/fugue/sql/_visitors.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/sql/api.py` & `fugue-0.8.6.dev2/fugue/sql/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/sql/workflow.py` & `fugue-0.8.6.dev2/fugue/sql/workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/workflow/_checkpoint.py` & `fugue-0.8.6.dev2/fugue/workflow/_checkpoint.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/workflow/_tasks.py` & `fugue-0.8.6.dev2/fugue/workflow/_tasks.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/workflow/_workflow_context.py` & `fugue-0.8.6.dev2/fugue/workflow/_workflow_context.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/workflow/api.py` & `fugue-0.8.6.dev2/fugue/workflow/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/workflow/module.py` & `fugue-0.8.6.dev2/fugue/workflow/module.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue/workflow/workflow.py` & `fugue-0.8.6.dev2/fugue/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue.egg-info/PKG-INFO` & `fugue-0.8.6.dev2/fugue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue
-Version: 0.8.6.dev1
+Version: 0.8.6.dev2
 Summary: An abstraction layer for distributed computation
 Home-page: http://github.com/fugue-project/fugue
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue
```

### Comparing `fugue-0.8.6.dev1/fugue.egg-info/SOURCES.txt` & `fugue-0.8.6.dev2/fugue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue.egg-info/requires.txt` & `fugue-0.8.6.dev2/fugue.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -22,28 +22,28 @@
 polars
 
 [all:python_version < "3.8"]
 dask[dataframe,distributed]
 ibis-framework>=2.1.1
 
 [all:python_version >= "3.8"]
-dask[dataframe,distributed]>=2022.9.0
+dask[dataframe,distributed]<2023.7.1,>=2022.9.0
 ibis-framework<6,>=3.2.0
 
 [cpp_sql_parser]
 fugue-sql-antlr[cpp]>=0.1.6
 
 [dask]
 qpd[dask]>=0.4.4
 
 [dask:python_version < "3.8"]
 dask[dataframe,distributed]
 
 [dask:python_version >= "3.8"]
-dask[dataframe,distributed]>=2022.9.0
+dask[dataframe,distributed]<2023.7.1,>=2022.9.0
 
 [duckdb]
 duckdb>=0.5.0
 pyarrow>=6.0.1
 numpy
 
 [ibis]
```

### Comparing `fugue-0.8.6.dev1/fugue_contrib/seaborn/__init__.py` & `fugue-0.8.6.dev2/fugue_contrib/seaborn/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_contrib/viz/__init__.py` & `fugue-0.8.6.dev2/fugue_contrib/viz/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_contrib/viz/_ext.py` & `fugue-0.8.6.dev2/fugue_contrib/viz/_ext.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_dask/_io.py` & `fugue-0.8.6.dev2/fugue_dask/_io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_dask/_utils.py` & `fugue-0.8.6.dev2/fugue_dask/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_dask/dataframe.py` & `fugue-0.8.6.dev2/fugue_dask/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_dask/execution_engine.py` & `fugue-0.8.6.dev2/fugue_dask/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_dask/ibis_engine.py` & `fugue-0.8.6.dev2/fugue_dask/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_dask/registry.py` & `fugue-0.8.6.dev2/fugue_dask/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_duckdb/_io.py` & `fugue-0.8.6.dev2/fugue_duckdb/_io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_duckdb/_utils.py` & `fugue-0.8.6.dev2/fugue_duckdb/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_duckdb/dask.py` & `fugue-0.8.6.dev2/fugue_duckdb/dask.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_duckdb/dataframe.py` & `fugue-0.8.6.dev2/fugue_duckdb/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_duckdb/execution_engine.py` & `fugue-0.8.6.dev2/fugue_duckdb/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_duckdb/ibis_engine.py` & `fugue-0.8.6.dev2/fugue_duckdb/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_duckdb/registry.py` & `fugue-0.8.6.dev2/fugue_duckdb/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_ibis/_utils.py` & `fugue-0.8.6.dev2/fugue_ibis/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_ibis/dataframe.py` & `fugue-0.8.6.dev2/fugue_ibis/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_ibis/execution/ibis_engine.py` & `fugue-0.8.6.dev2/fugue_ibis/execution/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_ibis/execution/pandas_backend.py` & `fugue-0.8.6.dev2/fugue_ibis/execution/pandas_backend.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_ibis/execution_engine.py` & `fugue-0.8.6.dev2/fugue_ibis/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_ibis/extensions.py` & `fugue-0.8.6.dev2/fugue_ibis/extensions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_notebook/__init__.py` & `fugue-0.8.6.dev2/fugue_notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_notebook/env.py` & `fugue-0.8.6.dev2/fugue_notebook/env.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_notebook/nbextension/main.js` & `fugue-0.8.6.dev2/fugue_notebook/nbextension/main.js`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_polars/polars_dataframe.py` & `fugue-0.8.6.dev2/fugue_polars/polars_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_polars/registry.py` & `fugue-0.8.6.dev2/fugue_polars/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_ray/_constants.py` & `fugue-0.8.6.dev2/fugue_ray/_constants.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_ray/_utils/cluster.py` & `fugue-0.8.6.dev2/fugue_ray/_utils/cluster.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_ray/_utils/dataframe.py` & `fugue-0.8.6.dev2/fugue_ray/_utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_ray/_utils/io.py` & `fugue-0.8.6.dev2/fugue_ray/_utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_ray/dataframe.py` & `fugue-0.8.6.dev2/fugue_ray/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_ray/execution_engine.py` & `fugue-0.8.6.dev2/fugue_ray/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_ray/registry.py` & `fugue-0.8.6.dev2/fugue_ray/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_spark/_utils/convert.py` & `fugue-0.8.6.dev2/fugue_spark/_utils/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_spark/_utils/io.py` & `fugue-0.8.6.dev2/fugue_spark/_utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_spark/_utils/misc.py` & `fugue-0.8.6.dev2/fugue_spark/_utils/misc.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_spark/_utils/partition.py` & `fugue-0.8.6.dev2/fugue_spark/_utils/partition.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_spark/dataframe.py` & `fugue-0.8.6.dev2/fugue_spark/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_spark/execution_engine.py` & `fugue-0.8.6.dev2/fugue_spark/execution_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,35 +130,45 @@
         output_schema: Any,
         partition_spec: PartitionSpec,
         on_init: Optional[Callable[[int, DataFrame], Any]] = None,
         map_func_format_hint: Optional[str] = None,
     ) -> DataFrame:
         output_schema = Schema(output_schema)
         if self._should_use_pandas_udf(output_schema):
-            # pandas udf can only be used for pyspark > 3
             if len(partition_spec.partition_by) > 0:
-                if partition_spec.algo == "coarse":
+                if partition_spec.algo in ["coarse", "even"]:
                     return self._map_by_pandas_udf(
                         df,
                         map_func=map_func,
                         output_schema=output_schema,
                         partition_spec=partition_spec,
                         on_init=on_init,
                         map_func_format_hint=map_func_format_hint,
                     )
-                elif partition_spec.algo != "even" or self.is_spark_connect:
+                else:
+                    if (  # not simple partitioning
+                        partition_spec.algo != "hash"
+                        or partition_spec.num_partitions != "0"
+                    ):
+                        # TODO: not sure if presort should be done
+                        # on physical partition level
+                        df = self.to_df(
+                            self.execution_engine.repartition(
+                                df, PartitionSpec(partition_spec, presort=[])
+                            )
+                        )
                     return self._group_map_by_pandas_udf(
                         df,
                         map_func=map_func,
                         output_schema=output_schema,
                         partition_spec=partition_spec,
                         on_init=on_init,
                         map_func_format_hint=map_func_format_hint,
                     )
-            elif len(partition_spec.partition_by) == 0:
+            else:
                 return self._map_by_pandas_udf(
                     df,
                     map_func=map_func,
                     output_schema=output_schema,
                     partition_spec=partition_spec,
                     on_init=on_init,
                     map_func_format_hint=map_func_format_hint,
```

### Comparing `fugue-0.8.6.dev1/fugue_spark/ibis_engine.py` & `fugue-0.8.6.dev2/fugue_spark/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_spark/registry.py` & `fugue-0.8.6.dev2/fugue_spark/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_test/bag_suite.py` & `fugue-0.8.6.dev2/fugue_test/bag_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_test/builtin_suite.py` & `fugue-0.8.6.dev2/fugue_test/builtin_suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import pyarrow as pa
 import pytest
 from pytest import raises
 from triad import SerializableRLock
 
 import fugue.api as fa
 from fugue import (
+    AnyDataFrame,
     ArrayDataFrame,
     CoTransformer,
     DataFrame,
     DataFrames,
     ExecutionEngine,
     FileSystem,
     FugueWorkflow,
@@ -361,14 +362,20 @@
                 b2 = dag.process(a, a, a, using=MockProcessor3)
                 b2.assert_eq(ArrayDataFrame([[3]], "a:int"))
                 a.process(mock_processor2).assert_eq(ArrayDataFrame([[1]], "a:int"))
                 a.output(mock_outputter2)
                 dag.output(dict(df=a), using=mock_outputter2)
                 a.partition(num=3).output(MockOutputter3)
                 dag.output(dict(aa=a, bb=b), using=MockOutputter4)
+
+                a = dag.create(mock_creator2, params=dict(p=2))
+                b = dag.create(mock_creator2, params=dict(p=2))
+                c = dag.process(a, b, using=mock_processor4)
+                c.assert_eq(ArrayDataFrame([[2]], "a:int"))
+                dag.output(a, b, using=mock_outputter4)
             dag.run(self.engine)
 
         def test_zip(self):
             with FugueWorkflow() as dag:
                 a = dag.df([[1, 2], [2, 3], [2, 5]], "a:int,b:int")
                 b = dag.df([[1, 3]], "a:int,c:int")
                 c1 = a.zip(b)
@@ -431,42 +438,73 @@
                 b.assert_eq(a)
             dag.run(self.engine)
 
         def test_transform_iterable_dfs(self):
             # this test is important for using mapInPandas in spark
 
             # schema: *,c:int
-            def mt_pandas(dfs: Iterable[pd.DataFrame]) -> Iterator[pd.DataFrame]:
+            def mt_pandas(
+                dfs: Iterable[pd.DataFrame], empty: bool = False
+            ) -> Iterator[pd.DataFrame]:
                 for df in dfs:
-                    yield df.assign(c=2)
+                    if not empty:
+                        df = df.assign(c=2)
+                        df = df[reversed(list(df.columns))]
+                        yield df
 
             with FugueWorkflow() as dag:
                 a = dag.df([[1, 2], [3, 4]], "a:int,b:int")
                 b = a.transform(mt_pandas)
                 dag.df([[1, 2, 2], [3, 4, 2]], "a:int,b:int,c:int").assert_eq(b)
             dag.run(self.engine)
 
+            # when iterable returns nothing
+            with FugueWorkflow() as dag:
+                a = dag.df([[1, 2], [3, 4]], "a:int,b:int")
+                # without partitioning
+                b = a.transform(mt_pandas, params=dict(empty=True))
+                dag.df([], "a:int,b:int,c:int").assert_eq(b)
+                # with partitioning
+                b = a.partition_by("a").transform(mt_pandas, params=dict(empty=True))
+                dag.df([], "a:int,b:int,c:int").assert_eq(b)
+            dag.run(self.engine)
+
             # schema: *
-            def mt_arrow(dfs: Iterable[pa.Table]) -> Iterator[pa.Table]:
+            def mt_arrow(
+                dfs: Iterable[pa.Table], empty: bool = False
+            ) -> Iterator[pa.Table]:
                 for df in dfs:
-                    yield df
+                    if not empty:
+                        df = df.select(reversed(df.schema.names))
+                        yield df
 
             # schema: a:long
             def mt_arrow_2(dfs: Iterable[pa.Table]) -> Iterator[pa.Table]:
                 for df in dfs:
                     yield df.drop(["b"])
 
             with FugueWorkflow() as dag:
                 a = dag.df([[1, 2], [3, 4]], "a:int,b:int")
                 b = a.transform(mt_arrow)
                 dag.df([[1, 2], [3, 4]], "a:int,b:int").assert_eq(b)
                 b = a.transform(mt_arrow_2)
                 dag.df([[1], [3]], "a:long").assert_eq(b)
             dag.run(self.engine)
 
+            # when iterable returns nothing
+            with FugueWorkflow() as dag:
+                a = dag.df([[1, 2], [3, 4]], "a:int,b:int")
+                # without partitioning
+                b = a.transform(mt_arrow, params=dict(empty=True))
+                dag.df([], "a:int,b:int").assert_eq(b)
+                # with partitioning
+                b = a.partition_by("a").transform(mt_arrow, params=dict(empty=True))
+                dag.df([], "a:int,b:int").assert_eq(b)
+            dag.run(self.engine)
+
         def test_transform_binary(self):
             with FugueWorkflow() as dag:
                 a = dag.df([[1, pickle.dumps([0, "a"])]], "a:int,b:bytes")
                 c = a.transform(mock_tf3).persist()
                 b = dag.df([[1, pickle.dumps([1, "ax"])]], "a:int,b:bytes")
                 b.assert_eq(c, check_order=True)
             dag.run(self.engine)
@@ -1825,14 +1863,18 @@
                 )
 
 
 def mock_creator(p: int) -> DataFrame:
     return ArrayDataFrame([[p]], "a:int")
 
 
+def mock_creator2(p: int) -> AnyDataFrame:
+    return fa.as_fugue_df([[p]], schema="a:int")
+
+
 def mock_processor(df1: List[List[Any]], df2: List[List[Any]]) -> DataFrame:
     return ArrayDataFrame([[len(df1) + len(df2)]], "a:int")
 
 
 def mock_processor2(e: ExecutionEngine, dfs: DataFrames) -> DataFrame:
     assert "test" in e.conf
     return ArrayDataFrame([[sum(s.count() for s in dfs.values())]], "a:int")
@@ -1840,27 +1882,35 @@
 
 class MockProcessor3(Processor):
     def process(self, dfs):
         assert "test" in self.workflow_conf
         return ArrayDataFrame([[sum(s.count() for s in dfs.values())]], "a:int")
 
 
+def mock_processor4(df1: AnyDataFrame, df2: AnyDataFrame) -> AnyDataFrame:
+    return ArrayDataFrame([[fa.count(df1) + fa.count(df2)]], "a:int")
+
+
 def mock_outputter(df1: List[List[Any]], df2: List[List[Any]]) -> None:
     assert len(df1) == len(df2)
 
 
 def mock_outputter2(df: List[List[Any]]) -> None:
     print(df)
 
 
 class MockOutputter3(Outputter):
     def process(self, dfs):
         assert "3" == self.partition_spec.num_partitions
 
 
+def mock_outputter4(df1: AnyDataFrame, df2: AnyDataFrame) -> None:
+    assert fa.count(df1) == fa.count(df2)
+
+
 class MockOutputter4(Outputter):
     def process(self, dfs):
         for k, v in dfs.items():
             print(k)
             v.show()
 
 
@@ -1891,16 +1941,16 @@
 def mock_tf0(df: pd.DataFrame, p=1, col="p") -> pd.DataFrame:
     df[col] = p
     return df
 
 
 # schema: *,ct:int,p:int
 def mock_tf1(df: pd.DataFrame, p=1) -> pd.DataFrame:
-    df["ct"] = df.shape[0]
     df["p"] = p
+    df["ct"] = df.shape[0]
     return df
 
 
 def mock_tf2_except(df: Iterable[Dict[str, Any]], p=1) -> Iterable[Dict[str, Any]]:
     n = 0
     for row in df:
         yield row
```

### Comparing `fugue-0.8.6.dev1/fugue_test/dataframe_suite.py` & `fugue-0.8.6.dev2/fugue_test/dataframe_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_test/execution_suite.py` & `fugue-0.8.6.dev2/fugue_test/execution_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/fugue_test/ibis_suite.py` & `fugue-0.8.6.dev2/fugue_test/ibis_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/setup.cfg` & `fugue-0.8.6.dev2/setup.cfg`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev1/setup.py` & `fugue-0.8.6.dev2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             "sqlglot",
             "jinja2",
         ],
         "cpp_sql_parser": ["fugue-sql-antlr[cpp]>=0.1.6"],
         "spark": ["pyspark>=3.1.1"],
         "dask": [
             "dask[distributed,dataframe]; python_version < '3.8'",
-            "dask[distributed,dataframe]>=2022.9.0; python_version >= '3.8'",
+            "dask[distributed,dataframe]>=2022.9.0,<2023.7.1; python_version >= '3.8'",
             "qpd[dask]>=0.4.4",
         ],
         "ray": ["ray[data]>=2.1.0", "duckdb>=0.5.0", "pyarrow>=6.0.1"],
         "duckdb": [
             "duckdb>=0.5.0",
             "pyarrow>=6.0.1",
             "numpy",
@@ -69,15 +69,15 @@
         "notebook": ["notebook", "jupyterlab", "ipython>=7.10.0"],
         "all": [
             "sqlglot",
             "jinja2",
             "fugue-sql-antlr[cpp]>=0.1.6",
             "pyspark>=3.1.1",
             "dask[distributed,dataframe]; python_version < '3.8'",
-            "dask[distributed,dataframe]>=2022.9.0; python_version >= '3.8'",
+            "dask[distributed,dataframe]>=2022.9.0,<2023.7.1; python_version >= '3.8'",
             "ray[data]>=2.1.0",
             "qpd[dask]>=0.4.4",
             "notebook",
             "jupyterlab",
             "ipython>=7.10.0",
             "duckdb>=0.5.0",
             "pyarrow>=6.0.1",
```

