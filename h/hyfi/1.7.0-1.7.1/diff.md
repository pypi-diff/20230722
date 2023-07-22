# Comparing `tmp/hyfi-1.7.0.tar.gz` & `tmp/hyfi-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.7.0.tar", max compression
+gzip compressed data, was "hyfi-1.7.1.tar", max compression
```

## Comparing `hyfi-1.7.0.tar` & `hyfi-1.7.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0     1071 2023-07-22 11:48:50.261604 hyfi-1.7.0/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-22 11:48:50.261604 hyfi-1.7.0/README.md
--rw-r--r--   0        0        0     4853 2023-07-22 11:49:17.081513 hyfi-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     4149 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     3586 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/__click__.py
--rw-r--r--   0        0        0      886 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-22 11:49:17.005514 hyfi-1.7.0/src/hyfi/_version.py
--rw-r--r--   0        0        0     3460 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7292 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    24378 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     7328 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/composer/base.py
--rw-r--r--   0        0        0     1933 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/composer/pydantic.py
--rw-r--r--   0        0        0        0 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      193 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      588 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       44 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       60 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      160 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      209 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      662 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/copier/__init__.yaml
--rw-r--r--   0        0        0      709 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0     1128 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      132 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      955 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       72 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      868 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0       91 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      286 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      424 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      159 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipe/dataset_load_from_disk.yaml
--rw-r--r--   0        0        0      213 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipe/dataset_sample.yaml
--rw-r--r--   0        0        0      113 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipe/dataset_save_to_disk.yaml
--rw-r--r--   0        0        0       69 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      746 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       38 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      142 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      329 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      132 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0     6984 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     1321 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/core/__init__.py
--rw-r--r--   0        0        0    10016 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/core/config.py
--rw-r--r--   0        0        0     5467 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/core/hydra/__init__.py
--rw-r--r--   0        0        0     3266 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/core/hydra/main.py
--rw-r--r--   0        0        0     5695 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/core/hydra/utils.py
--rw-r--r--   0        0        0     5911 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0     3517 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4209 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13823 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    19063 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     4359 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     4092 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/path/base.py
--rw-r--r--   0        0        0      533 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      594 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     1484 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1323 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/pipe/datasets.py
--rw-r--r--   0        0        0     1455 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8129 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     3207 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5854 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/py.typed
--rw-r--r--   0        0        0     3656 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     7131 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0    12742 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/conf.py
--rw-r--r--   0        0        0     1314 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30131 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     9036 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     4930 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    23279 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     7164 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     1116 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-22 13:06:59.311701 hyfi-1.7.1/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-22 13:06:59.311701 hyfi-1.7.1/README.md
+-rw-r--r--   0        0        0     4853 2023-07-22 13:07:25.179579 hyfi-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     4176 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     3586 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      886 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-22 13:07:25.099581 hyfi-1.7.1/src/hyfi/_version.py
+-rw-r--r--   0        0        0     3522 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7292 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    24378 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     7328 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/composer/base.py
+-rw-r--r--   0        0        0     1933 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/composer/pydantic.py
+-rw-r--r--   0        0        0        0 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      588 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       44 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       60 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      160 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      209 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      662 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/copier/__init__.yaml
+-rw-r--r--   0        0        0      709 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0     1128 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      132 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      955 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      876 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      286 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-22 13:06:59.315701 hyfi-1.7.1/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      424 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      159 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/conf/pipe/dataset_load_from_disk.yaml
+-rw-r--r--   0        0        0      213 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/conf/pipe/dataset_sample.yaml
+-rw-r--r--   0        0        0      113 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/conf/pipe/dataset_save_to_disk.yaml
+-rw-r--r--   0        0        0       69 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      738 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       38 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      329 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      132 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0     6984 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     1700 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/core/__init__.py
+-rw-r--r--   0        0        0    10184 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/core/config.py
+-rw-r--r--   0        0        0     5482 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/core/hydra/__init__.py
+-rw-r--r--   0        0        0     3266 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/core/hydra/main.py
+-rw-r--r--   0        0        0     5695 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/core/hydra/utils.py
+-rw-r--r--   0        0        0     5911 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0     3517 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4209 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    19303 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     4359 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     4092 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/path/base.py
+-rw-r--r--   0        0        0      533 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      594 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     1484 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1323 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/pipe/datasets.py
+-rw-r--r--   0        0        0     1455 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8129 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     3207 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5854 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/py.typed
+-rw-r--r--   0        0        0     3656 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     7131 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0    12742 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/utils/conf.py
+-rw-r--r--   0        0        0     1314 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30131 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     9036 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     4930 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    23279 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     7164 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     1116 2023-07-22 13:06:59.319701 hyfi-1.7.1/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.7.1/PKG-INFO
```

### Comparing `hyfi-1.7.0/LICENSE` & `hyfi-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/README.md` & `hyfi-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/pyproject.toml` & `hyfi-1.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.7.0"
+version = "1.7.1"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-1.7.0/src/hyfi/__cli__.py` & `hyfi-1.7.1/src/hyfi/__cli__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import sys
 from typing import List, Optional
 
 import hydra
 from omegaconf import DictConfig
 
-from hyfi.about import __package_name__
+from hyfi.about import __hyfi_package_name__
 from hyfi.core import (
     __about__,
     __config_name__,
     __config_path__,
     __hydra_version_base__,
 )
 from hyfi.core.config import HyfiConfig
@@ -77,21 +77,22 @@
                         If config_path is None no directory is added to the Config search path.
         config_name: The name of the config (usually the file name without the .yaml extension)
     """
     if search_path := __about__.user_config_path:
         sys.argv.append(f"--config-dir={search_path}")
     if config_path is None:
         config_path = __about__.config_path
-    if __about__.__package_name__ != __package_name__:
+    if __about__.__package_name__ != __hyfi_package_name__:
         overrides = overrides or []
         override = f"about={__about__.__package_name__}"
         if override not in overrides:
             overrides.append(override)
             logger.debug(
-                "Overriding `about` config group with `%s`", __about__.__package_name__
+                "Overriding `about` config group with `%s`",
+                __about__.__package_name__,
             )
     hyfi_hydra_main(
         config_path=config_path,
         config_name=config_name,
         version_base=__hydra_version_base__,
         overrides=overrides,
     )(cli_main)()
```

### Comparing `hyfi-1.7.0/src/hyfi/__click__.py` & `hyfi-1.7.1/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/__init__.py` & `hyfi-1.7.1/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/about/__init__.py` & `hyfi-1.7.1/src/hyfi/about/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 
 from pydantic import BaseModel, ConfigDict
 
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
 
-__package_name__: str = "hyfi"
-__package_path__: str = Path(__file__).parent.parent.as_posix()
-__app_name__: str = "HyFI"
-__authors__: str = "Young Joon Lee <entelecheia@hotmail.com>"
-__description__: str = (
+__hyfi_package_name__: str = "hyfi"
+__hyfi_package_path__: str = Path(__file__).parent.parent.as_posix()
+__hyfi_name__: str = "HyFI"
+__hyfi_authors__: str = "Young Joon Lee <entelecheia@hotmail.com>"
+__hyfi_description__: str = (
     "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 )
-__homepage__: str = "https://hyfi.entelecheia.ai"
-__license__: str = "MIT"
+__hyfi_homepage__: str = "https://hyfi.entelecheia.ai"
+__hyfi_license__: str = "MIT"
 
 
 def __hyfi_version__() -> str:
     """
     Returns the version of HyFI.
 
     Returns:
@@ -50,24 +50,24 @@
         license (str): The license under which the package is distributed.
         version (str): The version number of the package.
         model_config (ConfigDict): A ConfigDict that allows extra configuration
             options to be added to the AboutConfig instance.
     """
 
     _config_group_: str = "about"
-    __package_name__: str = __package_name__
-    __package_path__: str = __package_path__
+    __package_name__: str = __hyfi_package_name__
+    __package_path__: str = __hyfi_package_path__
     __user_config_path__: str = "config"
     __version__: str = __hyfi_version__()
 
-    name: str = __app_name__
-    authors: str = __authors__
-    description: str = __description__
-    homepage: str = __homepage__
-    license: str = __license__
+    name: str = __hyfi_name__
+    authors: str = __hyfi_authors__
+    description: str = __hyfi_description__
+    homepage: str = __hyfi_homepage__
+    license: str = __hyfi_license__
     version: str = __hyfi_version__()
 
     model_config = ConfigDict(extra="allow")  # type: ignore
 
     @property
     def config_module(self) -> str:
         """Returns the name of the configuration module."""
```

### Comparing `hyfi-1.7.0/src/hyfi/batch/__init__.py` & `hyfi-1.7.1/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/cached_path/__init__.py` & `hyfi-1.7.1/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.7.1/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/cached_path/cache_file.py` & `hyfi-1.7.1/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/cached_path/common.py` & `hyfi-1.7.1/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/cached_path/file_lock.py` & `hyfi-1.7.1/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/cached_path/meta.py` & `hyfi-1.7.1/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/cached_path/progress.py` & `hyfi-1.7.1/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.7.1/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.7.1/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.7.1/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.7.1/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.7.1/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/cached_path/testing.py` & `hyfi-1.7.1/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/cached_path/util.py` & `hyfi-1.7.1/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/composer/__init__.py` & `hyfi-1.7.1/src/hyfi/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/composer/base.py` & `hyfi-1.7.1/src/hyfi/composer/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/composer/pydantic.py` & `hyfi-1.7.1/src/hyfi/composer/pydantic.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/conf/batch/__init__.yaml` & `hyfi-1.7.1/src/hyfi/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/conf/copier/__init__.yaml` & `hyfi-1.7.1/src/hyfi/conf/copier/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.7.1/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.7.1/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.7.1/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.7.1/src/hyfi/conf/path/__init__.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file defines the path variables used in the project.
 # internal paths for hyfi
 defaults:
   - dirnames: __init__
 
 home: ${__home_path__:}
 hyfi: ${__hyfi_path__:}
-app: ${__app_path__:}
+package: ${__package_path__:}
 resources: ${alt:${oc.env:HYFI_RESOURCE_DIR,null},${.hyfi}/resources}
 runtime: ${get_original_cwd:}
 # global paths
 global_hyfi_root: ${oc.select:..global_hyfi_root,${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}}}
 global_workspace_name: ${oc.select:..global_workspace_name,${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},.hyfi}}
 # project specific paths
 project_name: ${oc.select:..project_name,${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi}}
```

### Comparing `hyfi-1.7.0/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.7.1/src/hyfi/conf/project/__init__.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 defaults:
   - /dotenv: __init__
   - /joblib: __init__
   - /path: __init__
 
 _config_name_: __init__
-project_name: ${alt:${oc.env:HYFI_PROJECT_NAME,null},${oc.select:about.__package_name__,hyfi}}
+project_name: ${alt:${oc.env:HYFI_PROJECT_NAME,null},${alt:${__package_name__:},hyfi}}
 project_description: ${oc.env:HYFI_PROJECT_DESC,""}
 project_root: ${alt:${oc.env:HYFI_PROJECT_ROOT,null},${.global_hyfi_root}/${.global_workspace_name}/projects/${.project_name}}
 project_workspace_name: ${alt:${oc.env:HYFI_PROJECT_WORKSPACE_NAME,null},workspace}
 global_hyfi_root: ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}}
 global_workspace_name: ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},.hyfi}
 num_workers: ${oc.env:HYFI_NUM_WORKERS,1}
 use_huggingface_hub: false
```

### Comparing `hyfi-1.7.0/src/hyfi/copier/__init__.py` & `hyfi-1.7.1/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/core/__init__.py` & `hyfi-1.7.1/src/hyfi/core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,60 @@
 from pathlib import Path
 
 from pydantic import BaseModel
 
-from hyfi.about import AboutConfig, __package_name__
+from hyfi.about import AboutConfig, __hyfi_package_name__
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
 
 __hydra_version_base__ = "1.2"
 __hydra_default_config_group_value__ = "__init__"
 __config_path__ = "conf"
 __config_name__ = "config"
-__config_module_path__ = f"{__package_name__}.{__config_path__}"
+__hyfi_config_module_path__ = f"{__hyfi_package_name__}.{__config_path__}"
 
 __about__ = AboutConfig()
 _batcher_instance_ = None
 
 
+def __app_name__() -> str:
+    """
+    Returns the name of the App
+
+    Returns:
+        string containing the name of the App
+    """
+
+    return __about__.name
+
+
 def __app_version__() -> str:
     """
     Returns the version of App.
 
     Returns:
         string containing the version of App
     """
 
     return __about__.__version__
 
 
-def __app_path__() -> str:
+def __package_name__() -> str:
+    """
+    Returns the package name of the App
+
+    Returns:
+        string containing the package name of the App
+    """
+
+    return __about__.__package_name__
+
+
+def __package_path__() -> str:
     """
     Returns the path to the App root folder
 
     Returns:
         string containing the path to the App root folder
     """
```

### Comparing `hyfi-1.7.0/src/hyfi/core/config.py` & `hyfi-1.7.1/src/hyfi/core/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,22 @@
     ConfigDict,
     FieldValidationInfo,
     PrivateAttr,
     field_validator,
     model_validator,
 )
 
-from hyfi.about import AboutConfig, __app_name__
-from hyfi.core import __about__, __app_version__, __hydra_config__
+from hyfi.about import AboutConfig
+from hyfi.core import (
+    __about__,
+    __app_name__,
+    __app_version__,
+    __hydra_config__,
+    __package_name__,
+)
 from hyfi.dotenv import DotEnvConfig
 from hyfi.pipeline import PipelineConfig
 from hyfi.project import ProjectConfig
 from hyfi.task import TaskConfig
 from hyfi.utils.envs import ENVs
 from hyfi.utils.logging import LOGGING
 from hyfi.utils.notebooks import NBs
@@ -261,28 +267,38 @@
     def app_name(self):
         """
         Get the name of the application.
 
         Returns:
             The name of the application
         """
-        return self.about.name if self.about else __app_name__
+        return __app_name__()
+
+    @property
+    def package_name(self):
+        """
+        Get the name of the package.
+
+        Returns:
+            The name of the package
+        """
+        return __package_name__()
 
     @property
     def dotenv(self):
         return DotEnvConfig()  # type: ignore
 
     @property
     def osenv(self):
         return os.environ
 
     def print_about(self, **kwargs):
         about = AboutConfig(**kwargs)
-        pkg_name = kwargs.get("__package_name__", about.__package_name__)
-        name = about.name
+        pkg_name = self.package_name
+        name = self.app_name
         print()
         for k, v in about.model_dump().items():
             if k.startswith("_") or k == "version":
                 continue
             print(f"{k:11} : {v}")
         print(f"{'version':11} : {self.app_version}")
         if pkg_name:
```

### Comparing `hyfi-1.7.0/src/hyfi/core/hydra/__init__.py` & `hyfi-1.7.1/src/hyfi/core/hydra/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from hydra._internal.config_search_path_impl import ConfigSearchPathImpl
 from hydra._internal.hydra import Hydra
 from hydra.core.config_search_path import ConfigSearchPath
 from hydra.core.global_hydra import GlobalHydra
 from hydra.core.singleton import Singleton
 from hydra.errors import HydraException
 
-from hyfi.core import __config_module_path__, __config_path__
+from hyfi.core import __config_path__, __hyfi_config_module_path__
 from hyfi.utils.logging import LOGGING
 from hyfi.utils.packages import PKGs
 
 logger = LOGGING.getLogger(__name__)
 
 
 def get_gh_backup() -> Any:
@@ -35,15 +35,15 @@
 def get_caller_config_module_path(
     config_path: Optional[str] = __config_path__,
 ) -> str:
     """Returns the path to the caller module's config folder"""
     caller_module_name = PKGs.get_caller_module_name()
     config_module = caller_module_name.split(".")[0]
     config_module_path = f"{config_module}.{config_path}"
-    if config_module_path == __config_module_path__:
+    if config_module_path == __hyfi_config_module_path__:
         return config_module_path
     # check if the config module is importable
     try:
         __import__(config_module_path)
         return config_module_path
     except ImportError:
         logger.debug("Config module not found: %s", config_module_path)
@@ -121,15 +121,15 @@
     from hydra.core.plugins import Plugins
     from hydra.plugins.search_path_plugin import SearchPathPlugin
 
     search_path = ConfigSearchPathImpl()
     search_path.append("hydra", "pkg://hydra.conf")
 
     # addiing hyfi's config module to the search path should come before the other modules
-    append_search_path("hyfi", f"pkg://{__config_module_path__}", search_path)
+    append_search_path("hyfi", f"pkg://{__hyfi_config_module_path__}", search_path)
 
     if config_module:
         path = (
             config_module
             if config_module.startswith("pkg://")
             else f"pkg://{config_module}"
             if "." in config_module
```

### Comparing `hyfi-1.7.0/src/hyfi/core/hydra/main.py` & `hyfi-1.7.1/src/hyfi/core/hydra/main.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/core/hydra/utils.py` & `hyfi-1.7.1/src/hyfi/core/hydra/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/dotenv/__init__.py` & `hyfi-1.7.1/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/graphics/__init__.py` & `hyfi-1.7.1/src/hyfi/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/graphics/collage.py` & `hyfi-1.7.1/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/graphics/motion.py` & `hyfi-1.7.1/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/graphics/utils.py` & `hyfi-1.7.1/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/joblib/__init__.py` & `hyfi-1.7.1/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/joblib/batch/apply.py` & `hyfi-1.7.1/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.7.1/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.7.1/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/main/__init__.py` & `hyfi-1.7.1/src/hyfi/main/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,21 @@
 import hydra
 from omegaconf import DictConfig, OmegaConf
 
 from hyfi.about import __hyfi_version__
 from hyfi.cached_path import cached_path
 from hyfi.composer import Composer, SpecialKeys
 from hyfi.copier import Copier
-from hyfi.core import __app_path__, __app_version__, __home_path__, __hyfi_path__
+from hyfi.core import (
+    __app_version__,
+    __home_path__,
+    __hyfi_path__,
+    __package_name__,
+    __package_path__,
+)
 from hyfi.core.config import __global_config__, __search_package_path__
 from hyfi.dotenv import DotEnvConfig
 from hyfi.graphics import GRAPHICs
 from hyfi.joblib import BATCHER, JobLibConfig
 from hyfi.pipeline import PIPELINEs
 from hyfi.pipeline.configs import PipeConfig
 from hyfi.project import ProjectConfig
@@ -34,15 +40,16 @@
 from hyfi.workflow import WorkflowConfig
 
 logger = LOGGING.getLogger(__name__)
 
 
 OmegaConf.register_new_resolver("__hyfi_path__", __hyfi_path__)
 OmegaConf.register_new_resolver("__hyfi_version__", __hyfi_version__)
-OmegaConf.register_new_resolver("__app_path__", __app_path__)
+OmegaConf.register_new_resolver("__package_name__", __package_name__)
+OmegaConf.register_new_resolver("__package_path__", __package_path__)
 OmegaConf.register_new_resolver("__app_version__", __app_version__)
 OmegaConf.register_new_resolver("__version__", __app_version__)
 OmegaConf.register_new_resolver("__search_package_path__", __search_package_path__)
 OmegaConf.register_new_resolver("__home_path__", __home_path__)
 OmegaConf.register_new_resolver("today", FUNCs.today)
 OmegaConf.register_new_resolver("to_datetime", FUNCs.strptime)
 OmegaConf.register_new_resolver("iif", lambda cond, t, f: t if cond else f)
@@ -77,17 +84,20 @@
     PIPELINEs,
     PKGs,
 ):
     """Primary class for the hyfi config package"""
 
     config = __global_config__
     SpeicialKeys = SpecialKeys
-    __version__ = __global_config__._version_
+    __version__ = __hyfi_version__()
     __hyfi_path__ = __hyfi_path__()
     __home_path__ = __home_path__()
+    __package_name__ = __package_name__()
+    __package_path__ = __package_path__()
+    __app_version__ = __app_version__()
 
     def __init__(self) -> None:
         raise NotImplementedError("Use one of the static construction functions")
 
     @staticmethod
     def about(**args) -> None:
         """Print the about information"""
```

### Comparing `hyfi-1.7.0/src/hyfi/path/__init__.py` & `hyfi-1.7.1/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/path/base.py` & `hyfi-1.7.1/src/hyfi/path/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/path/batch.py` & `hyfi-1.7.1/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/path/dirnames.py` & `hyfi-1.7.1/src/hyfi/path/dirnames.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/path/task.py` & `hyfi-1.7.1/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/pipe/__init__.py` & `hyfi-1.7.1/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/pipe/datasets.py` & `hyfi-1.7.1/src/hyfi/pipe/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/pipe/test.py` & `hyfi-1.7.1/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/pipeline/__init__.py` & `hyfi-1.7.1/src/hyfi/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/pipeline/configs.py` & `hyfi-1.7.1/src/hyfi/pipeline/configs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/project/__init__.py` & `hyfi-1.7.1/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/task/__init__.py` & `hyfi-1.7.1/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/task/batch.py` & `hyfi-1.7.1/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/utils/conf.py` & `hyfi-1.7.1/src/hyfi/utils/conf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/utils/contexts.py` & `hyfi-1.7.1/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/utils/datasets.py` & `hyfi-1.7.1/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/utils/envs.py` & `hyfi-1.7.1/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/utils/funcs.py` & `hyfi-1.7.1/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/utils/gpumon.py` & `hyfi-1.7.1/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/utils/iolibs.py` & `hyfi-1.7.1/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/utils/logging.py` & `hyfi-1.7.1/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/utils/notebooks.py` & `hyfi-1.7.1/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/utils/packages.py` & `hyfi-1.7.1/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/src/hyfi/workflow/__init__.py` & `hyfi-1.7.1/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.7.0/PKG-INFO` & `hyfi-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.7.0
+Version: 1.7.1
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

