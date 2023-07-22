# Comparing `tmp/hyfi-1.6.0.tar.gz` & `tmp/hyfi-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.6.0.tar", max compression
+gzip compressed data, was "hyfi-1.6.1.tar", max compression
```

## Comparing `hyfi-1.6.0.tar` & `hyfi-1.6.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0     1071 2023-07-22 04:04:18.022894 hyfi-1.6.0/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-22 04:04:18.022894 hyfi-1.6.0/README.md
--rw-r--r--   0        0        0     4928 2023-07-22 04:04:45.178858 hyfi-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     3701 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     3586 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/__click__.py
--rw-r--r--   0        0        0      886 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-22 04:04:45.102858 hyfi-1.6.0/src/hyfi/_version.py
--rw-r--r--   0        0        0     3314 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7292 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    24378 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     7328 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/composer/base.py
--rw-r--r--   0        0        0     1933 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/composer/pydantic.py
--rw-r--r--   0        0        0        0 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      262 2023-07-22 04:04:45.102858 hyfi-1.6.0/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      588 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       44 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       60 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      160 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      209 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      662 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/copier/__init__.yaml
--rw-r--r--   0        0        0      709 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      209 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      132 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      926 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       72 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      846 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0       91 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      286 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      424 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      159 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/pipe/dataset_load_from_disk.yaml
--rw-r--r--   0        0        0      213 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/pipe/dataset_sample.yaml
--rw-r--r--   0        0        0      113 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/pipe/dataset_save_to_disk.yaml
--rw-r--r--   0        0        0       69 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      746 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       38 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      142 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      329 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      132 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0     6984 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0      948 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/core/__init__.py
--rw-r--r--   0        0        0    10050 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/core/config.py
--rw-r--r--   0        0        0     4661 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/core/hydra/__init__.py
--rw-r--r--   0        0        0     3029 2023-07-22 04:04:18.026894 hyfi-1.6.0/src/hyfi/core/hydra/main.py
--rw-r--r--   0        0        0     5193 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/core/hydra/utils.py
--rw-r--r--   0        0        0     5911 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0     3517 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4209 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13823 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    18823 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     4359 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     4092 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/path/base.py
--rw-r--r--   0        0        0      533 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      594 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     1484 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1323 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/pipe/datasets.py
--rw-r--r--   0        0        0     1455 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8129 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     3207 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5854 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/py.typed
--rw-r--r--   0        0        0     3656 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     7131 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0    12742 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/utils/conf.py
--rw-r--r--   0        0        0     1314 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30131 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     9036 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     4930 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    23279 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     7164 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     1116 2023-07-22 04:04:18.030894 hyfi-1.6.0/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-22 05:04:08.564763 hyfi-1.6.1/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-22 05:04:08.564763 hyfi-1.6.1/README.md
+-rw-r--r--   0        0        0     4928 2023-07-22 05:04:35.053688 hyfi-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3701 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     3586 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      886 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-22 05:04:34.973686 hyfi-1.6.1/src/hyfi/_version.py
+-rw-r--r--   0        0        0     3315 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7292 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    24378 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     7328 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/composer/base.py
+-rw-r--r--   0        0        0     1933 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/composer/pydantic.py
+-rw-r--r--   0        0        0        0 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      262 2023-07-22 05:04:34.973686 hyfi-1.6.1/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      588 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       44 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       60 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      160 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      209 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      662 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/conf/copier/__init__.yaml
+-rw-r--r--   0        0        0      709 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      209 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      132 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      926 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-22 05:04:08.568763 hyfi-1.6.1/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      846 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      286 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      424 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      159 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/conf/pipe/dataset_load_from_disk.yaml
+-rw-r--r--   0        0        0      213 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/conf/pipe/dataset_sample.yaml
+-rw-r--r--   0        0        0      113 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/conf/pipe/dataset_save_to_disk.yaml
+-rw-r--r--   0        0        0       69 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      746 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       38 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      329 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      132 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0     6984 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0      948 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/core/__init__.py
+-rw-r--r--   0        0        0    10050 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/core/config.py
+-rw-r--r--   0        0        0     4649 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/core/hydra/__init__.py
+-rw-r--r--   0        0        0     3029 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/core/hydra/main.py
+-rw-r--r--   0        0        0     5699 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/core/hydra/utils.py
+-rw-r--r--   0        0        0     5911 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0     3517 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4209 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    18823 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     4359 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     4092 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/path/base.py
+-rw-r--r--   0        0        0      533 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      594 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     1484 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1323 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/pipe/datasets.py
+-rw-r--r--   0        0        0     1455 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8129 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     3207 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5854 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/py.typed
+-rw-r--r--   0        0        0     3656 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     7131 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0    12742 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/utils/conf.py
+-rw-r--r--   0        0        0     1314 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30131 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     9036 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     4930 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    23279 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     7164 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     1116 2023-07-22 05:04:08.572763 hyfi-1.6.1/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.6.1/PKG-INFO
```

### Comparing `hyfi-1.6.0/LICENSE` & `hyfi-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/README.md` & `hyfi-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/pyproject.toml` & `hyfi-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.6.0"
+version = "1.6.1"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-1.6.0/src/hyfi/__cli__.py` & `hyfi-1.6.1/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/__click__.py` & `hyfi-1.6.1/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/__init__.py` & `hyfi-1.6.1/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/about/__init__.py` & `hyfi-1.6.1/src/hyfi/about/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,12 +85,12 @@
         if os.path.isdir(search_path):
             self.__user_config_path__ = (
                 search_path
                 if os.path.isabs(search_path)
                 else os.path.join(os.getcwd(), search_path)
             )
         else:
-            logger.info(
+            logger.debug(
                 "The user configuration directory does not exist: %s", search_path
             )
             self.__user_config_path__ = ""
         return self.__user_config_path__
```

### Comparing `hyfi-1.6.0/src/hyfi/batch/__init__.py` & `hyfi-1.6.1/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/cached_path/__init__.py` & `hyfi-1.6.1/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.6.1/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/cached_path/cache_file.py` & `hyfi-1.6.1/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/cached_path/common.py` & `hyfi-1.6.1/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/cached_path/file_lock.py` & `hyfi-1.6.1/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/cached_path/meta.py` & `hyfi-1.6.1/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/cached_path/progress.py` & `hyfi-1.6.1/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.6.1/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.6.1/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.6.1/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.6.1/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.6.1/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/cached_path/testing.py` & `hyfi-1.6.1/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/cached_path/util.py` & `hyfi-1.6.1/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/composer/__init__.py` & `hyfi-1.6.1/src/hyfi/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/composer/base.py` & `hyfi-1.6.1/src/hyfi/composer/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/composer/pydantic.py` & `hyfi-1.6.1/src/hyfi/composer/pydantic.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/conf/batch/__init__.yaml` & `hyfi-1.6.1/src/hyfi/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/conf/copier/__init__.yaml` & `hyfi-1.6.1/src/hyfi/conf/copier/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.6.1/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.6.1/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.6.1/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.6.1/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.6.1/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/copier/__init__.py` & `hyfi-1.6.1/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/core/__init__.py` & `hyfi-1.6.1/src/hyfi/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/core/config.py` & `hyfi-1.6.1/src/hyfi/core/config.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/core/hydra/__init__.py` & `hyfi-1.6.1/src/hyfi/core/hydra/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,28 +30,28 @@
         del Singleton._instances[GlobalHydra]
     else:
         Singleton._instances[GlobalHydra] = _gh_backup
 
 
 def get_caller_config_module_path(
     config_path: Optional[str] = __config_path__,
-) -> Optional[str]:
+) -> str:
     """Returns the path to the caller module's config folder"""
     caller_module_name = PKGs.get_caller_module_name()
     config_module = caller_module_name.split(".")[0]
     config_module_path = f"{config_module}.{config_path}"
     if config_module_path == __config_module_path__:
         return config_module_path
     # check if the config module is importable
     try:
         __import__(config_module_path)
         return config_module_path
     except ImportError:
         logger.debug("Config module not found: %s", config_module_path)
-    return None
+    return ""
 
 
 _UNSPECIFIED_: Any = object()
 
 
 class initialize_config:
     """
```

### Comparing `hyfi-1.6.0/src/hyfi/core/hydra/main.py` & `hyfi-1.6.1/src/hyfi/core/hydra/main.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/core/hydra/utils.py` & `hyfi-1.6.1/src/hyfi/core/hydra/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 )
 from hydra.core.config_search_path import SearchPathQuery
 from hydra.core.utils import validate_config_path
 from hydra.errors import SearchPathException
 from hydra.types import TaskFunction
 
 from hyfi.core import __config_module_path__
+from hyfi.core.hydra import get_caller_config_module_path
 
 log = logging.getLogger(__name__)
 
 
 def _run_hydra(
     args: argparse.Namespace,
     args_parser: argparse.ArgumentParser,
@@ -53,45 +54,58 @@
 
     validate_config_path(config_path)
 
     search_path = create_automatic_config_search_path(
         calling_file, calling_module, config_path
     )
 
-    def add_hyfi_conf() -> None:
-        if (
-            calling_module
-            and calling_module.split(".")[0] == __config_module_path__.split(".")[0]
-        ):
-            log.debug("Calling module is hyfi")
-        else:
-            log.debug(
-                "Calling module is not hyfi, adding hyfi to the config search path"
-            )
-            search_path.prepend(
-                provider="hyfi",
-                path=f"pkg://{__config_module_path__}",
-            )
-
-    run_and_report(add_hyfi_conf)
-
     def add_conf_dir() -> None:
         if args.config_dir is not None:
             abs_config_dir = os.path.abspath(args.config_dir)
             if not os.path.isdir(abs_config_dir):
                 raise SearchPathException(
                     f"Additional config directory '{abs_config_dir}' not found"
                 )
             search_path.prepend(
                 provider="command-line",
                 path=f"file://{abs_config_dir}",
                 anchor=SearchPathQuery(provider="schema"),
             )
 
     run_and_report(add_conf_dir)
+
+    def add_hyfi_conf() -> None:
+        path = f"pkg://{__config_module_path__}"
+        for sp_item in search_path.get_path():
+            if sp_item.path == path:
+                log.debug("HyFI config path already in search path")
+                return
+        log.debug("Adding hyfi to the config search path")
+        search_path.prepend(
+            provider="hyfi",
+            path=path,
+        )
+
+    run_and_report(add_hyfi_conf)
+
+    def add_caller_conf() -> None:
+        caller_config_path = get_caller_config_module_path()
+        path = f"pkg://{caller_config_path}"
+        for sp_item in search_path.get_path():
+            if sp_item.path == path:
+                log.debug("Caller config path already in search path")
+                return
+        log.debug("Adding %s to the config search path", caller_config_path)
+        search_path.prepend(
+            provider="caller",
+            path=path,
+        )
+
+    run_and_report(add_caller_conf)
+
     hydra = run_and_report(
         lambda: Hydra.create_main_hydra2(
             task_name=task_name, config_search_path=search_path
         )
     )
 
     try:
```

### Comparing `hyfi-1.6.0/src/hyfi/dotenv/__init__.py` & `hyfi-1.6.1/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/graphics/__init__.py` & `hyfi-1.6.1/src/hyfi/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/graphics/collage.py` & `hyfi-1.6.1/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/graphics/motion.py` & `hyfi-1.6.1/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/graphics/utils.py` & `hyfi-1.6.1/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/joblib/__init__.py` & `hyfi-1.6.1/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/joblib/batch/apply.py` & `hyfi-1.6.1/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.6.1/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.6.1/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/main/__init__.py` & `hyfi-1.6.1/src/hyfi/main/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/path/__init__.py` & `hyfi-1.6.1/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/path/base.py` & `hyfi-1.6.1/src/hyfi/path/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/path/batch.py` & `hyfi-1.6.1/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/path/dirnames.py` & `hyfi-1.6.1/src/hyfi/path/dirnames.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/path/task.py` & `hyfi-1.6.1/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/pipe/__init__.py` & `hyfi-1.6.1/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/pipe/datasets.py` & `hyfi-1.6.1/src/hyfi/pipe/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/pipe/test.py` & `hyfi-1.6.1/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/pipeline/__init__.py` & `hyfi-1.6.1/src/hyfi/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/pipeline/configs.py` & `hyfi-1.6.1/src/hyfi/pipeline/configs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/project/__init__.py` & `hyfi-1.6.1/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/task/__init__.py` & `hyfi-1.6.1/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/task/batch.py` & `hyfi-1.6.1/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/utils/conf.py` & `hyfi-1.6.1/src/hyfi/utils/conf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/utils/contexts.py` & `hyfi-1.6.1/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/utils/datasets.py` & `hyfi-1.6.1/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/utils/envs.py` & `hyfi-1.6.1/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/utils/funcs.py` & `hyfi-1.6.1/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/utils/gpumon.py` & `hyfi-1.6.1/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/utils/iolibs.py` & `hyfi-1.6.1/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/utils/logging.py` & `hyfi-1.6.1/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/utils/notebooks.py` & `hyfi-1.6.1/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/utils/packages.py` & `hyfi-1.6.1/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/src/hyfi/workflow/__init__.py` & `hyfi-1.6.1/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.6.0/PKG-INFO` & `hyfi-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.6.0
+Version: 1.6.1
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

