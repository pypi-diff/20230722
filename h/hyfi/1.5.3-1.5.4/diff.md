# Comparing `tmp/hyfi-1.5.3.tar.gz` & `tmp/hyfi-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.5.3.tar", max compression
+gzip compressed data, was "hyfi-1.5.4.tar", max compression
```

## Comparing `hyfi-1.5.3.tar` & `hyfi-1.5.4.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0     1071 2023-07-21 20:56:29.475244 hyfi-1.5.3/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-21 20:56:29.475244 hyfi-1.5.3/README.md
--rw-r--r--   0        0        0     4928 2023-07-21 20:56:55.783770 hyfi-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     2793 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     3586 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/__click__.py
--rw-r--r--   0        0        0      715 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-21 20:56:55.703768 hyfi-1.5.3/src/hyfi/_version.py
--rw-r--r--   0        0        0     3314 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7292 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    24378 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     7328 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/composer/base.py
--rw-r--r--   0        0        0     1933 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/composer/pydantic.py
--rw-r--r--   0        0        0        0 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      262 2023-07-21 20:56:55.703768 hyfi-1.5.3/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      588 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       44 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       60 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      160 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      209 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      662 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/copier/__init__.yaml
--rw-r--r--   0        0        0      709 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      209 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      132 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      926 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       72 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      846 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0       91 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      286 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      424 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0       69 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      746 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       38 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      142 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      329 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      132 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0     6984 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0      865 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/core/__init__.py
--rw-r--r--   0        0        0    10050 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/core/config.py
--rw-r--r--   0        0        0     3480 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/core/hydra.py
--rw-r--r--   0        0        0     5911 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0     3517 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4209 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-21 20:56:29.483244 hyfi-1.5.3/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13823 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    18823 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     4359 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     4092 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/path/base.py
--rw-r--r--   0        0        0      533 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      594 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     1484 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1455 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8129 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     3207 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5854 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/py.typed
--rw-r--r--   0        0        0     3656 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     7131 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0    12742 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/conf.py
--rw-r--r--   0        0        0     1314 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30131 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     9036 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     4930 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    23279 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     6955 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     1116 2023-07-21 20:56:29.487244 hyfi-1.5.3/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-21 22:06:29.999867 hyfi-1.5.4/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-21 22:06:29.999867 hyfi-1.5.4/README.md
+-rw-r--r--   0        0        0     4928 2023-07-21 22:06:55.060706 hyfi-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2793 2023-07-21 22:06:30.003867 hyfi-1.5.4/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     3586 2023-07-21 22:06:30.003867 hyfi-1.5.4/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      715 2023-07-21 22:06:30.003867 hyfi-1.5.4/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-21 22:06:54.980703 hyfi-1.5.4/src/hyfi/_version.py
+-rw-r--r--   0        0        0     3314 2023-07-21 22:06:30.003867 hyfi-1.5.4/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7292 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    24378 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     7328 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/composer/base.py
+-rw-r--r--   0        0        0     1933 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/composer/pydantic.py
+-rw-r--r--   0        0        0        0 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      262 2023-07-21 22:06:54.980703 hyfi-1.5.4/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      588 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       44 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       60 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      160 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      209 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      662 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/copier/__init__.yaml
+-rw-r--r--   0        0        0      709 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      209 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      132 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      926 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      846 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      286 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      424 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0       69 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      746 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       38 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      329 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      132 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0     6984 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0      943 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/core/__init__.py
+-rw-r--r--   0        0        0    10050 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/core/config.py
+-rw-r--r--   0        0        0     3630 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/core/hydra.py
+-rw-r--r--   0        0        0     5911 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0     3517 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4209 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    18823 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     4359 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     4092 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/path/base.py
+-rw-r--r--   0        0        0      533 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      594 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     1484 2023-07-21 22:06:30.007867 hyfi-1.5.4/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1455 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8129 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     3207 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5854 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/py.typed
+-rw-r--r--   0        0        0     3656 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     7131 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0    12742 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/utils/conf.py
+-rw-r--r--   0        0        0     1314 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30131 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     9036 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     4930 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    23279 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     7164 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     1116 2023-07-21 22:06:30.011867 hyfi-1.5.4/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.5.4/PKG-INFO
```

### Comparing `hyfi-1.5.3/LICENSE` & `hyfi-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/README.md` & `hyfi-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/pyproject.toml` & `hyfi-1.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.5.3"
+version = "1.5.4"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-1.5.3/src/hyfi/__cli__.py` & `hyfi-1.5.4/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/__click__.py` & `hyfi-1.5.4/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/__init__.py` & `hyfi-1.5.4/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/about/__init__.py` & `hyfi-1.5.4/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/batch/__init__.py` & `hyfi-1.5.4/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/cached_path/__init__.py` & `hyfi-1.5.4/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.5.4/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/cached_path/cache_file.py` & `hyfi-1.5.4/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/cached_path/common.py` & `hyfi-1.5.4/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/cached_path/file_lock.py` & `hyfi-1.5.4/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/cached_path/meta.py` & `hyfi-1.5.4/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/cached_path/progress.py` & `hyfi-1.5.4/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.5.4/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.5.4/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.5.4/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.5.4/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.5.4/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/cached_path/testing.py` & `hyfi-1.5.4/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/cached_path/util.py` & `hyfi-1.5.4/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/composer/__init__.py` & `hyfi-1.5.4/src/hyfi/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/composer/base.py` & `hyfi-1.5.4/src/hyfi/composer/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/composer/pydantic.py` & `hyfi-1.5.4/src/hyfi/composer/pydantic.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/conf/batch/__init__.yaml` & `hyfi-1.5.4/src/hyfi/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/conf/copier/__init__.yaml` & `hyfi-1.5.4/src/hyfi/conf/copier/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.5.4/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.5.4/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.5.4/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.5.4/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.5.4/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/copier/__init__.py` & `hyfi-1.5.4/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/core/__init__.py` & `hyfi-1.5.4/src/hyfi/core/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from pathlib import Path
 
 from pydantic import BaseModel
 
-from hyfi.about import AboutConfig
+from hyfi.about import AboutConfig, __package_name__
 from hyfi.utils.logging import LOGGING
 
 logger = LOGGING.getLogger(__name__)
 
 __hydra_version_base__ = "1.2"
 __hydra_default_config_group_value__ = "__init__"
 __config_path__ = "conf"
 __config_name__ = "config"
+__config_module__ = f"{__package_name__}.{__config_path__}"
 
 __about__ = AboutConfig()
 _batcher_instance_ = None
 
 
 class HydraConfig(BaseModel):
     """Global configuration for Hydra"""
```

### Comparing `hyfi-1.5.3/src/hyfi/core/config.py` & `hyfi-1.5.4/src/hyfi/core/config.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/core/hydra.py` & `hyfi-1.5.4/src/hyfi/core/hydra.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from hydra._internal.config_search_path_impl import ConfigSearchPathImpl
 from hydra._internal.hydra import Hydra
 from hydra.core.config_search_path import ConfigSearchPath
 from hydra.core.global_hydra import GlobalHydra
 from hydra.core.singleton import Singleton
 from hydra.errors import HydraException
 
+from hyfi.core import __config_module__
+
 
 def get_gh_backup() -> Any:
     if GlobalHydra in Singleton._instances:
         return copy.deepcopy(Singleton._instances[GlobalHydra])
     else:
         return None
 
@@ -83,14 +85,17 @@
 
     search_path = ConfigSearchPathImpl()
     search_path.append("hydra", "pkg://hydra.conf")
 
     if config_module is not None:
         search_path.append("main", f"pkg://{config_module}")
 
+    if config_module != __config_module__:
+        search_path.append("hyfi", f"pkg://{__config_module__}")
+
     if search_path_dir is not None and os.path.isdir(search_path_dir):
         search_path.append("hyfi", f"file://{search_path_dir}")
 
     search_path_plugins = Plugins.instance().discover(SearchPathPlugin)
     for spp in search_path_plugins:
         plugin = spp()
         assert isinstance(plugin, SearchPathPlugin)
```

### Comparing `hyfi-1.5.3/src/hyfi/dotenv/__init__.py` & `hyfi-1.5.4/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/graphics/__init__.py` & `hyfi-1.5.4/src/hyfi/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/graphics/collage.py` & `hyfi-1.5.4/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/graphics/motion.py` & `hyfi-1.5.4/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/graphics/utils.py` & `hyfi-1.5.4/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/joblib/__init__.py` & `hyfi-1.5.4/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/joblib/batch/apply.py` & `hyfi-1.5.4/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.5.4/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.5.4/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/main/__init__.py` & `hyfi-1.5.4/src/hyfi/main/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/path/__init__.py` & `hyfi-1.5.4/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/path/base.py` & `hyfi-1.5.4/src/hyfi/path/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/path/batch.py` & `hyfi-1.5.4/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/path/dirnames.py` & `hyfi-1.5.4/src/hyfi/path/dirnames.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/path/task.py` & `hyfi-1.5.4/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/pipe/__init__.py` & `hyfi-1.5.4/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/pipe/test.py` & `hyfi-1.5.4/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/pipeline/__init__.py` & `hyfi-1.5.4/src/hyfi/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/pipeline/configs.py` & `hyfi-1.5.4/src/hyfi/pipeline/configs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/project/__init__.py` & `hyfi-1.5.4/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/task/__init__.py` & `hyfi-1.5.4/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/task/batch.py` & `hyfi-1.5.4/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/utils/conf.py` & `hyfi-1.5.4/src/hyfi/utils/conf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/utils/contexts.py` & `hyfi-1.5.4/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/utils/datasets.py` & `hyfi-1.5.4/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/utils/envs.py` & `hyfi-1.5.4/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/utils/funcs.py` & `hyfi-1.5.4/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/utils/gpumon.py` & `hyfi-1.5.4/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/utils/iolibs.py` & `hyfi-1.5.4/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/utils/logging.py` & `hyfi-1.5.4/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/utils/notebooks.py` & `hyfi-1.5.4/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/src/hyfi/utils/packages.py` & `hyfi-1.5.4/src/hyfi/utils/packages.py`

 * *Files 3% similar despite different names*

```diff
@@ -197,7 +197,12 @@
             logger.error(f"Error getting source: {e}")
             return ""
 
     @staticmethod
     def viewsource(obj: str) -> None:
         """Print the source code of the object."""
         print(PKGs.getsource(obj))
+
+    @staticmethod
+    def get_caller_module_name() -> str:
+        """Get the name of the module that called this function."""
+        return inspect.getmodule(inspect.stack()[2][0]).__name__  # type: ignore
```

### Comparing `hyfi-1.5.3/src/hyfi/workflow/__init__.py` & `hyfi-1.5.4/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.5.3/PKG-INFO` & `hyfi-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.5.3
+Version: 1.5.4
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

