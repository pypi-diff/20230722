# Comparing `tmp/hyfi-1.6.4.tar.gz` & `tmp/hyfi-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.6.4.tar", max compression
+gzip compressed data, was "hyfi-1.7.0.tar", max compression
```

## Comparing `hyfi-1.6.4.tar` & `hyfi-1.7.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0     1071 2023-07-22 07:00:40.388696 hyfi-1.6.4/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-22 07:00:40.388696 hyfi-1.6.4/README.md
--rw-r--r--   0        0        0     4928 2023-07-22 07:01:08.048712 hyfi-1.6.4/pyproject.toml
--rw-r--r--   0        0        0     3703 2023-07-22 07:00:40.392696 hyfi-1.6.4/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     3586 2023-07-22 07:00:40.392696 hyfi-1.6.4/src/hyfi/__click__.py
--rw-r--r--   0        0        0      886 2023-07-22 07:00:40.392696 hyfi-1.6.4/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-22 07:01:07.972712 hyfi-1.6.4/src/hyfi/_version.py
--rw-r--r--   0        0        0     3315 2023-07-22 07:00:40.392696 hyfi-1.6.4/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7292 2023-07-22 07:00:40.392696 hyfi-1.6.4/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-22 07:00:40.392696 hyfi-1.6.4/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-22 07:00:40.392696 hyfi-1.6.4/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-22 07:00:40.392696 hyfi-1.6.4/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-22 07:00:40.392696 hyfi-1.6.4/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-22 07:00:40.392696 hyfi-1.6.4/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-22 07:00:40.392696 hyfi-1.6.4/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-22 07:00:40.392696 hyfi-1.6.4/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-22 07:00:40.392696 hyfi-1.6.4/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-22 07:00:40.392696 hyfi-1.6.4/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-22 07:00:40.392696 hyfi-1.6.4/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-22 07:00:40.392696 hyfi-1.6.4/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-22 07:00:40.392696 hyfi-1.6.4/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-22 07:00:40.392696 hyfi-1.6.4/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-22 07:00:40.392696 hyfi-1.6.4/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    24378 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     7328 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/composer/base.py
--rw-r--r--   0        0        0     1933 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/composer/pydantic.py
--rw-r--r--   0        0        0        0 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      262 2023-07-22 07:01:07.972712 hyfi-1.6.4/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      588 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       44 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       60 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      160 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      209 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      662 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/copier/__init__.yaml
--rw-r--r--   0        0        0      709 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0     1128 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      132 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      926 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       72 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      846 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0       91 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      286 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      424 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      159 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/pipe/dataset_load_from_disk.yaml
--rw-r--r--   0        0        0      213 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/pipe/dataset_sample.yaml
--rw-r--r--   0        0        0      113 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/pipe/dataset_save_to_disk.yaml
--rw-r--r--   0        0        0       69 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      746 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       38 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      142 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      329 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      132 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0     6984 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0      948 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/core/__init__.py
--rw-r--r--   0        0        0    10050 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/core/config.py
--rw-r--r--   0        0        0     5357 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/core/hydra/__init__.py
--rw-r--r--   0        0        0     3029 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/core/hydra/main.py
--rw-r--r--   0        0        0     5695 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/core/hydra/utils.py
--rw-r--r--   0        0        0     5911 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0     3517 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4209 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13823 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    18823 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     4359 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     4092 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/path/base.py
--rw-r--r--   0        0        0      533 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      594 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     1484 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1323 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/pipe/datasets.py
--rw-r--r--   0        0        0     1455 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8129 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     3207 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5854 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/py.typed
--rw-r--r--   0        0        0     3656 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     7131 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-22 07:00:40.396696 hyfi-1.6.4/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0    12742 2023-07-22 07:00:40.400696 hyfi-1.6.4/src/hyfi/utils/conf.py
--rw-r--r--   0        0        0     1314 2023-07-22 07:00:40.400696 hyfi-1.6.4/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30131 2023-07-22 07:00:40.400696 hyfi-1.6.4/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     9036 2023-07-22 07:00:40.400696 hyfi-1.6.4/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-22 07:00:40.400696 hyfi-1.6.4/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     4930 2023-07-22 07:00:40.400696 hyfi-1.6.4/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    23279 2023-07-22 07:00:40.400696 hyfi-1.6.4/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-22 07:00:40.400696 hyfi-1.6.4/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-22 07:00:40.400696 hyfi-1.6.4/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     7164 2023-07-22 07:00:40.400696 hyfi-1.6.4/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-22 07:00:40.400696 hyfi-1.6.4/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     1116 2023-07-22 07:00:40.400696 hyfi-1.6.4/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-22 11:48:50.261604 hyfi-1.7.0/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-22 11:48:50.261604 hyfi-1.7.0/README.md
+-rw-r--r--   0        0        0     4853 2023-07-22 11:49:17.081513 hyfi-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4149 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     3586 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      886 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-22 11:49:17.005514 hyfi-1.7.0/src/hyfi/_version.py
+-rw-r--r--   0        0        0     3460 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7292 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    24378 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     7328 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/composer/base.py
+-rw-r--r--   0        0        0     1933 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/composer/pydantic.py
+-rw-r--r--   0        0        0        0 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      588 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       44 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       60 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      160 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      209 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      662 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/copier/__init__.yaml
+-rw-r--r--   0        0        0      709 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0     1128 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      132 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      955 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      868 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      286 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      424 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      159 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipe/dataset_load_from_disk.yaml
+-rw-r--r--   0        0        0      213 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipe/dataset_sample.yaml
+-rw-r--r--   0        0        0      113 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipe/dataset_save_to_disk.yaml
+-rw-r--r--   0        0        0       69 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      746 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       38 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      329 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      132 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0     6984 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     1321 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/core/__init__.py
+-rw-r--r--   0        0        0    10016 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/core/config.py
+-rw-r--r--   0        0        0     5467 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/core/hydra/__init__.py
+-rw-r--r--   0        0        0     3266 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/core/hydra/main.py
+-rw-r--r--   0        0        0     5695 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/core/hydra/utils.py
+-rw-r--r--   0        0        0     5911 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0     3517 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-22 11:48:50.265604 hyfi-1.7.0/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4209 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    19063 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     4359 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     4092 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/path/base.py
+-rw-r--r--   0        0        0      533 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      594 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     1484 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1323 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/pipe/datasets.py
+-rw-r--r--   0        0        0     1455 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8129 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     3207 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5854 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/py.typed
+-rw-r--r--   0        0        0     3656 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     7131 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0    12742 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/conf.py
+-rw-r--r--   0        0        0     1314 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30131 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     9036 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     4930 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    23279 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     7164 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     1116 2023-07-22 11:48:50.269604 hyfi-1.7.0/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.7.0/PKG-INFO
```

### Comparing `hyfi-1.6.4/LICENSE` & `hyfi-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/README.md` & `hyfi-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/pyproject.toml` & `hyfi-1.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.6.4"
+version = "1.7.0"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
@@ -200,15 +200,14 @@
 write_to_template = '__version__ = "{version}"'
 tag_regex = '^(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$'
 
 [tool.semantic_release]
 branch = "main"
 version_variable = "src/hyfi/_version.py:__version__"
 version_toml = "pyproject.toml:tool.poetry.version"
-version_pattern = 'src/hyfi/conf/about/__init__.yaml:version: "{version}"'
 version_source = "tag"
 commit_version_number = true                                               # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
 changelog_file = "CHANGELOG.md"
```

### Comparing `hyfi-1.6.4/src/hyfi/__cli__.py` & `hyfi-1.7.0/src/hyfi/__cli__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Command line interface for HyFI"""
 import os
 import sys
-from typing import Optional
+from typing import List, Optional
 
 import hydra
 from omegaconf import DictConfig
 
+from hyfi.about import __package_name__
 from hyfi.core import (
     __about__,
     __config_name__,
     __config_path__,
     __hydra_version_base__,
 )
 from hyfi.core.config import HyfiConfig
@@ -58,49 +59,59 @@
 
     HyFI.terminate()
 
 
 def hyfi_main(
     config_path: Optional[str] = __config_path__,
     config_name: Optional[str] = __config_name__,
+    overrides: Optional[List[str]] = None,
 ) -> None:
     """
     Main function for the command line interface of Hydra
 
     Args:
         config_path: The config path, a directory where Hydra will search for
                         config files. This path is added to Hydra's searchpath.
                         Relative paths are interpreted relative to the declaring python
                         file. Alternatively, you can use the prefix `pkg://` to specify
                         a python package to add to the searchpath.
                         If config_path is None no directory is added to the Config search path.
         config_name: The name of the config (usually the file name without the .yaml extension)
     """
     if search_path := __about__.user_config_path:
-        logger.debug("Adding `%s` to Hydra's config search path", search_path)
         sys.argv.append(f"--config-dir={search_path}")
     if config_path is None:
         config_path = __about__.config_path
+    if __about__.__package_name__ != __package_name__:
+        overrides = overrides or []
+        override = f"about={__about__.__package_name__}"
+        if override not in overrides:
+            overrides.append(override)
+            logger.debug(
+                "Overriding `about` config group with `%s`", __about__.__package_name__
+            )
     hyfi_hydra_main(
         config_path=config_path,
         config_name=config_name,
         version_base=__hydra_version_base__,
+        overrides=overrides,
     )(cli_main)()
 
 
 def hydra_main(
     config_path: Optional[str] = __config_path__,
     config_name: Optional[str] = __config_name__,
+    overrides: Optional[List[str]] = None,
 ) -> None:
     """
     Main function for the command line interface of Hydra
 
     Args:
         config_path: The config path, a directory where Hydra will search for
                         config files. This path is added to Hydra's searchpath.
                         Relative paths are interpreted relative to the declaring python
                         file. Alternatively, you can use the prefix `pkg://` to specify
                         a python package to add to the searchpath.
                         If config_path is None no directory is added to the Config search path.
         config_name: The name of the config (usually the file name without the .yaml extension)
     """
-    hyfi_main(config_path, config_name)
+    hyfi_main(config_path, config_name, overrides)
```

### Comparing `hyfi-1.6.4/src/hyfi/__click__.py` & `hyfi-1.7.0/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/__init__.py` & `hyfi-1.7.0/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/about/__init__.py` & `hyfi-1.7.0/src/hyfi/about/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,38 +2,39 @@
 
 It defines the AboutConfig class, which is a Pydantic BaseModel that contains
 metadata about the package, such as its name, version, authors, and license.
 It also defines the model_config attribute, which is a ConfigDict that allows
 extra configuration options to be added to the AboutConfig instance.
 """
 import os
+from pathlib import Path
 
 from pydantic import BaseModel, ConfigDict
 
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
 
 __package_name__: str = "hyfi"
+__package_path__: str = Path(__file__).parent.parent.as_posix()
 __app_name__: str = "HyFI"
 __authors__: str = "Young Joon Lee <entelecheia@hotmail.com>"
 __description__: str = (
     "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 )
 __homepage__: str = "https://hyfi.entelecheia.ai"
 __license__: str = "MIT"
 
 
-def __version__() -> str:
+def __hyfi_version__() -> str:
     """
-    Returns the version of Hyfi. It is used to determine the version of Hyfi.
-
+    Returns the version of HyFI.
 
     Returns:
-        string containing the version of
+        string containing the version of HyFI
     """
     from hyfi._version import __version__
 
     return __version__
 
 
 class AboutConfig(BaseModel):
@@ -50,22 +51,24 @@
         version (str): The version number of the package.
         model_config (ConfigDict): A ConfigDict that allows extra configuration
             options to be added to the AboutConfig instance.
     """
 
     _config_group_: str = "about"
     __package_name__: str = __package_name__
+    __package_path__: str = __package_path__
     __user_config_path__: str = "config"
+    __version__: str = __hyfi_version__()
 
     name: str = __app_name__
     authors: str = __authors__
     description: str = __description__
     homepage: str = __homepage__
     license: str = __license__
-    version: str = __version__()
+    version: str = __hyfi_version__()
 
     model_config = ConfigDict(extra="allow")  # type: ignore
 
     @property
     def config_module(self) -> str:
         """Returns the name of the configuration module."""
         return f"{self.__package_name__}.conf"
```

### Comparing `hyfi-1.6.4/src/hyfi/batch/__init__.py` & `hyfi-1.7.0/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/cached_path/__init__.py` & `hyfi-1.7.0/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.7.0/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/cached_path/cache_file.py` & `hyfi-1.7.0/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/cached_path/common.py` & `hyfi-1.7.0/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/cached_path/file_lock.py` & `hyfi-1.7.0/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/cached_path/meta.py` & `hyfi-1.7.0/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/cached_path/progress.py` & `hyfi-1.7.0/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.7.0/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.7.0/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.7.0/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.7.0/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.7.0/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/cached_path/testing.py` & `hyfi-1.7.0/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/cached_path/util.py` & `hyfi-1.7.0/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/composer/__init__.py` & `hyfi-1.7.0/src/hyfi/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/composer/base.py` & `hyfi-1.7.0/src/hyfi/composer/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/composer/pydantic.py` & `hyfi-1.7.0/src/hyfi/composer/pydantic.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/conf/batch/__init__.yaml` & `hyfi-1.7.0/src/hyfi/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/conf/copier/__init__.yaml` & `hyfi-1.7.0/src/hyfi/conf/copier/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.7.0/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.7.0/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.7.0/src/hyfi/conf/mode/__init__.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # @package _global_
 debug_mode: false
 resolve: true
 verbose: false
+version: ${__app_version__:}
 ignore_warnings: true
 logging_level: WARNING
 hydra_log_dir: ${oc.select:project.global_hyfi_root, ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}}}/${oc.select:project.global_workspace_name, ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},.hyfi}}/logs/hydra
 
 hydra:
   job:
     name: ${oc.select:project.project_name, ${oc.select:task.project.project_name, ${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi}}}
```

### Comparing `hyfi-1.6.4/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.7.0/src/hyfi/conf/path/__init__.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # This file defines the path variables used in the project.
 # internal paths for hyfi
 defaults:
   - dirnames: __init__
 
 home: ${__home_path__:}
 hyfi: ${__hyfi_path__:}
+app: ${__app_path__:}
 resources: ${alt:${oc.env:HYFI_RESOURCE_DIR,null},${.hyfi}/resources}
 runtime: ${get_original_cwd:}
 # global paths
 global_hyfi_root: ${oc.select:..global_hyfi_root,${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}}}
 global_workspace_name: ${oc.select:..global_workspace_name,${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},.hyfi}}
 # project specific paths
 project_name: ${oc.select:..project_name,${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi}}
```

### Comparing `hyfi-1.6.4/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.7.0/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/copier/__init__.py` & `hyfi-1.7.0/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/core/config.py` & `hyfi-1.7.0/src/hyfi/core/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     ConfigDict,
     FieldValidationInfo,
     PrivateAttr,
     field_validator,
     model_validator,
 )
 
-from hyfi.about import AboutConfig, __app_name__, __version__
-from hyfi.core import __about__, __hydra_config__
+from hyfi.about import AboutConfig, __app_name__
+from hyfi.core import __about__, __app_version__, __hydra_config__
 from hyfi.dotenv import DotEnvConfig
 from hyfi.pipeline import PipelineConfig
 from hyfi.project import ProjectConfig
 from hyfi.task import TaskConfig
 from hyfi.utils.envs import ENVs
 from hyfi.utils.logging import LOGGING
 from hyfi.utils.notebooks import NBs
@@ -46,15 +46,15 @@
     copier: Optional[DictConfig] = None
     project: Optional[ProjectConfig] = None
     pipeline: Optional[PipelineConfig] = None
     task: Optional[TaskConfig] = None
     workflow: Optional[WorkflowConfig] = None
     tasks: Optional[List[str]] = None
 
-    _version_: str = PrivateAttr(__version__())
+    _version_: str = PrivateAttr(__app_version__())
     _initilized_: bool = PrivateAttr(False)
 
     model_config = ConfigDict(
         arbitrary_types_allowed=True,
         validate_assignment=True,
         extra="allow",
     )  # type: ignore
@@ -251,15 +251,15 @@
         """
         Get the version of the application.
 
 
         Returns:
             The version of the application
         """
-        return self.about.version if self.about else __version__()
+        return __app_version__()
 
     @property
     def app_name(self):
         """
         Get the name of the application.
 
         Returns:
@@ -277,27 +277,26 @@
 
     def print_about(self, **kwargs):
         about = AboutConfig(**kwargs)
         pkg_name = kwargs.get("__package_name__", about.__package_name__)
         name = about.name
         print()
         for k, v in about.model_dump().items():
-            if k.startswith("_"):
+            if k.startswith("_") or k == "version":
                 continue
             print(f"{k:11} : {v}")
+        print(f"{'version':11} : {self.app_version}")
         if pkg_name:
             print(f"\nExecute `{pkg_name} --help` to see what you can do with {name}")
 
     def get_project_path(self, path_name: str) -> str:
         if self.project and self.project.path:
             return str(self.project.path.get_path(path_name))
         return ""
 
 
 __global_config__ = HyfiConfig()
-if __global_config__.about:
-    __global_config__.about.version = __version__()
 
 
 def __search_package_path__():
     """Global HyFI config path for the package to search for."""
     return __global_config__.hyfi_config_path
```

### Comparing `hyfi-1.6.4/src/hyfi/core/hydra/__init__.py` & `hyfi-1.7.0/src/hyfi/core/hydra/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
     def __repr__(self) -> str:
         return "hyfi.core.hydra.initialize_config()"
 
 
 def append_search_path(provider: str, path: str, search_path: ConfigSearchPath) -> None:
     if not path:
-        logger.debug("Not adding empty path to Hydra's config search path")
+        logger.debug("Not adding empty path to Hydra's config search path for `%s`", provider)
         return
     for sp_item in search_path.get_path():
         if sp_item.path == path:
             logger.debug(
                 "Not adding `%s` to Hydra's config search path, it was already added by `%s`",
                 path,
                 sp_item.provider,
@@ -120,26 +120,27 @@
 ) -> ConfigSearchPath:
     from hydra.core.plugins import Plugins
     from hydra.plugins.search_path_plugin import SearchPathPlugin
 
     search_path = ConfigSearchPathImpl()
     search_path.append("hydra", "pkg://hydra.conf")
 
+    # addiing hyfi's config module to the search path should come before the other modules
+    append_search_path("hyfi", f"pkg://{__config_module_path__}", search_path)
+
     if config_module:
         path = (
             config_module
             if config_module.startswith("pkg://")
             else f"pkg://{config_module}"
             if "." in config_module
             else ""
         )
         append_search_path("main", path, search_path)
 
-    append_search_path("hyfi", f"pkg://{__config_module_path__}", search_path)
-
     if caller_config_module := get_caller_config_module_path():
         append_search_path("caller", f"pkg://{caller_config_module}", search_path)
 
     if search_path_dir is not None and os.path.isdir(search_path_dir):
         append_search_path("user", f"file://{search_path_dir}", search_path)
 
     search_path_plugins = Plugins.instance().discover(SearchPathPlugin)
```

### Comparing `hyfi-1.6.4/src/hyfi/core/hydra/main.py` & `hyfi-1.7.0/src/hyfi/core/hydra/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Facebook, Inc. and its affiliates. All Rights Reserved
 import functools
 from textwrap import dedent
-from typing import Any, Callable, Optional
+from typing import Any, Callable, List, Optional
 
 from hydra import version
 from hydra._internal.deprecation_warning import deprecation_warning
 from hydra._internal.utils import get_args_parser
 from hydra.core.utils import _flush_loggers
 from hydra.main import _get_rerun_conf
 from hydra.types import TaskFunction
@@ -16,14 +16,15 @@
 _UNSPECIFIED_: Any = object()
 
 
 def main(
     config_path: Optional[str] = _UNSPECIFIED_,
     config_name: Optional[str] = None,
     version_base: Optional[str] = _UNSPECIFIED_,
+    overrides: Optional[List[str]] = None,
 ) -> Callable[[TaskFunction], Any]:
     """
     :param config_path: The config path, a directory where Hydra will search for
                         config files. This path is added to Hydra's searchpath.
                         Relative paths are interpreted relative to the declaring python
                         file. Alternatively, you can use the prefix `pkg://` to specify
                         a python package to add to the searchpath.
@@ -53,14 +54,18 @@
     def main_decorator(task_function: TaskFunction) -> Callable[[], None]:
         @functools.wraps(task_function)
         def decorated_main(cfg_passthrough: Optional[DictConfig] = None) -> Any:
             if cfg_passthrough is not None:
                 return task_function(cfg_passthrough)
             args_parser = get_args_parser()
             args = args_parser.parse_args()
+            if overrides and not args.overrides:
+                args.overrides = overrides
+            elif overrides and args.overrides:
+                args.overrides.extend(overrides)
             if args.experimental_rerun is not None:
                 cfg = _get_rerun_conf(args.experimental_rerun, args.overrides)
                 task_function(cfg)
                 _flush_loggers()
             else:
                 # no return value from run_hydra() as it may sometime actually run the task_function
                 # multiple times (--multirun)
```

### Comparing `hyfi-1.6.4/src/hyfi/core/hydra/utils.py` & `hyfi-1.7.0/src/hyfi/core/hydra/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/dotenv/__init__.py` & `hyfi-1.7.0/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/graphics/__init__.py` & `hyfi-1.7.0/src/hyfi/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/graphics/collage.py` & `hyfi-1.7.0/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/graphics/motion.py` & `hyfi-1.7.0/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/graphics/utils.py` & `hyfi-1.7.0/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/joblib/__init__.py` & `hyfi-1.7.0/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/joblib/batch/apply.py` & `hyfi-1.7.0/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.7.0/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.7.0/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/main/__init__.py` & `hyfi-1.7.0/src/hyfi/main/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 import os
 import random
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import hydra
 from omegaconf import DictConfig, OmegaConf
 
-from hyfi.about import __version__
+from hyfi.about import __hyfi_version__
 from hyfi.cached_path import cached_path
 from hyfi.composer import Composer, SpecialKeys
 from hyfi.copier import Copier
-from hyfi.core import __home_path__, __hyfi_path__
+from hyfi.core import __app_path__, __app_version__, __home_path__, __hyfi_path__
 from hyfi.core.config import __global_config__, __search_package_path__
 from hyfi.dotenv import DotEnvConfig
 from hyfi.graphics import GRAPHICs
 from hyfi.joblib import BATCHER, JobLibConfig
 from hyfi.pipeline import PIPELINEs
 from hyfi.pipeline.configs import PipeConfig
 from hyfi.project import ProjectConfig
@@ -33,15 +33,18 @@
 from hyfi.utils.packages import PKGs
 from hyfi.workflow import WorkflowConfig
 
 logger = LOGGING.getLogger(__name__)
 
 
 OmegaConf.register_new_resolver("__hyfi_path__", __hyfi_path__)
-OmegaConf.register_new_resolver("__version__", __version__)
+OmegaConf.register_new_resolver("__hyfi_version__", __hyfi_version__)
+OmegaConf.register_new_resolver("__app_path__", __app_path__)
+OmegaConf.register_new_resolver("__app_version__", __app_version__)
+OmegaConf.register_new_resolver("__version__", __app_version__)
 OmegaConf.register_new_resolver("__search_package_path__", __search_package_path__)
 OmegaConf.register_new_resolver("__home_path__", __home_path__)
 OmegaConf.register_new_resolver("today", FUNCs.today)
 OmegaConf.register_new_resolver("to_datetime", FUNCs.strptime)
 OmegaConf.register_new_resolver("iif", lambda cond, t, f: t if cond else f)
 OmegaConf.register_new_resolver("alt", lambda val, alt: val or alt)
 OmegaConf.register_new_resolver("randint", random.randint, use_cache=True)
```

### Comparing `hyfi-1.6.4/src/hyfi/path/__init__.py` & `hyfi-1.7.0/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/path/base.py` & `hyfi-1.7.0/src/hyfi/path/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/path/batch.py` & `hyfi-1.7.0/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/path/dirnames.py` & `hyfi-1.7.0/src/hyfi/path/dirnames.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/path/task.py` & `hyfi-1.7.0/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/pipe/__init__.py` & `hyfi-1.7.0/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/pipe/datasets.py` & `hyfi-1.7.0/src/hyfi/pipe/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/pipe/test.py` & `hyfi-1.7.0/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/pipeline/__init__.py` & `hyfi-1.7.0/src/hyfi/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/pipeline/configs.py` & `hyfi-1.7.0/src/hyfi/pipeline/configs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/project/__init__.py` & `hyfi-1.7.0/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/task/__init__.py` & `hyfi-1.7.0/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/task/batch.py` & `hyfi-1.7.0/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/utils/conf.py` & `hyfi-1.7.0/src/hyfi/utils/conf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/utils/contexts.py` & `hyfi-1.7.0/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/utils/datasets.py` & `hyfi-1.7.0/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/utils/envs.py` & `hyfi-1.7.0/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/utils/funcs.py` & `hyfi-1.7.0/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/utils/gpumon.py` & `hyfi-1.7.0/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/utils/iolibs.py` & `hyfi-1.7.0/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/utils/logging.py` & `hyfi-1.7.0/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/utils/notebooks.py` & `hyfi-1.7.0/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/utils/packages.py` & `hyfi-1.7.0/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/src/hyfi/workflow/__init__.py` & `hyfi-1.7.0/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.4/PKG-INFO` & `hyfi-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.6.4
+Version: 1.7.0
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

