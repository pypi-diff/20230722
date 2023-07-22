# Comparing `tmp/dcnum-0.11.2.tar.gz` & `tmp/dcnum-0.11.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.11.2.tar", last modified: Thu Jun 29 22:42:43 2023, max compression
+gzip compressed data, was "dcnum-0.11.3.tar", last modified: Sat Jul 22 08:57:23 2023, max compression
```

## Comparing `dcnum-0.11.2.tar` & `dcnum-0.11.3.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.257078 dcnum-0.11.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.249078 dcnum-0.11.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.249078 dcnum-0.11.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-29 22:42:34.000000 dcnum-0.11.2/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-29 22:42:34.000000 dcnum-0.11.2/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-29 22:42:34.000000 dcnum-0.11.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-29 22:42:34.000000 dcnum-0.11.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-29 22:42:34.000000 dcnum-0.11.2/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-29 22:42:34.000000 dcnum-0.11.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-29 22:42:43.257078 dcnum-0.11.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-29 22:42:34.000000 dcnum-0.11.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.249078 dcnum-0.11.2/dcnum/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 22:42:43.000000 dcnum-0.11.2/dcnum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.249078 dcnum-0.11.2/dcnum/feat/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/event_extractor_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.249078 dcnum-0.11.2/dcnum/feat/feat_background/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_background/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_background/bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_background/bg_sparse_median.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.249078 dcnum-0.11.2/dcnum/feat/feat_brightness/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_brightness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_brightness/bright_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_brightness/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.253078 dcnum-0.11.2/dcnum/feat/feat_moments/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_moments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_moments/ct_opencv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_moments/mt_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.253078 dcnum-0.11.2/dcnum/feat/feat_texture/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_texture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_texture/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/feat_texture/tex_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/feat/queue_event_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.253078 dcnum-0.11.2/dcnum/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/meta/ppid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.253078 dcnum-0.11.2/dcnum/read/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/read/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/read/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/read/hdf5_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.253078 dcnum-0.11.2/dcnum/segm/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/segm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/segm/segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/segm/segmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/segm/segmenter_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/segm/segmenter_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/segm/segmenter_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.253078 dcnum-0.11.2/dcnum/write/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/write/deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/write/queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-29 22:42:34.000000 dcnum-0.11.2/dcnum/write/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.249078 dcnum-0.11.2/dcnum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-29 22:42:43.000000 dcnum-0.11.2/dcnum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-29 22:42:43.000000 dcnum-0.11.2/dcnum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 22:42:43.000000 dcnum-0.11.2/dcnum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-29 22:42:43.000000 dcnum-0.11.2/dcnum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 22:42:43.000000 dcnum-0.11.2/dcnum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.253078 dcnum-0.11.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-29 22:42:34.000000 dcnum-0.11.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.253078 dcnum-0.11.2/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-29 22:42:34.000000 dcnum-0.11.2/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-29 22:42:34.000000 dcnum-0.11.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-29 22:42:34.000000 dcnum-0.11.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-29 22:42:34.000000 dcnum-0.11.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 22:42:43.257078 dcnum-0.11.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.257078 dcnum-0.11.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:42:43.257078 dcnum-0.11.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_feat_background_bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_feat_brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_feat_haralick.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_feat_moments_based.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_ppid.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_ppid_segm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_read_concat_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_read_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_segmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_write_deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-29 22:42:34.000000 dcnum-0.11.2/tests/test_write_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:23.137631 dcnum-0.11.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:23.125631 dcnum-0.11.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:23.125631 dcnum-0.11.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-22 08:57:15.000000 dcnum-0.11.3/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-22 08:57:15.000000 dcnum-0.11.3/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-22 08:57:15.000000 dcnum-0.11.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-22 08:57:15.000000 dcnum-0.11.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-22 08:57:15.000000 dcnum-0.11.3/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-22 08:57:15.000000 dcnum-0.11.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-22 08:57:23.137631 dcnum-0.11.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-22 08:57:15.000000 dcnum-0.11.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:23.125631 dcnum-0.11.3/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-22 08:57:23.000000 dcnum-0.11.3/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:23.129631 dcnum-0.11.3/dcnum/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/feat/event_extractor_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:23.129631 dcnum-0.11.3/dcnum/feat/feat_background/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/feat/feat_background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/feat/feat_background/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/feat/feat_background/bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/feat/feat_background/bg_sparse_median.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:23.129631 dcnum-0.11.3/dcnum/feat/feat_brightness/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/feat/feat_brightness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/feat/feat_brightness/bright_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/feat/feat_brightness/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:23.129631 dcnum-0.11.3/dcnum/feat/feat_moments/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/feat/feat_moments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/feat/feat_moments/ct_opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/feat/feat_moments/mt_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:23.129631 dcnum-0.11.3/dcnum/feat/feat_texture/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/feat/feat_texture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/feat/feat_texture/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/feat/feat_texture/tex_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/feat/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/feat/queue_event_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:23.129631 dcnum-0.11.3/dcnum/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/meta/ppid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:23.129631 dcnum-0.11.3/dcnum/read/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/read/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/read/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12147 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/read/hdf5_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:23.133631 dcnum-0.11.3/dcnum/segm/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/segm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/segm/segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/segm/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/segm/segmenter_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/segm/segmenter_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/segm/segmenter_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:23.133631 dcnum-0.11.3/dcnum/write/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/write/deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/write/queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-22 08:57:15.000000 dcnum-0.11.3/dcnum/write/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:23.125631 dcnum-0.11.3/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-22 08:57:23.000000 dcnum-0.11.3/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-22 08:57:23.000000 dcnum-0.11.3/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 08:57:23.000000 dcnum-0.11.3/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-22 08:57:23.000000 dcnum-0.11.3/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 08:57:23.000000 dcnum-0.11.3/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:23.133631 dcnum-0.11.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-22 08:57:15.000000 dcnum-0.11.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:23.133631 dcnum-0.11.3/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-22 08:57:15.000000 dcnum-0.11.3/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-22 08:57:15.000000 dcnum-0.11.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-22 08:57:15.000000 dcnum-0.11.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-22 08:57:15.000000 dcnum-0.11.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 08:57:23.137631 dcnum-0.11.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:23.133631 dcnum-0.11.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-22 08:57:15.000000 dcnum-0.11.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 08:57:23.137631 dcnum-0.11.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-07-22 08:57:15.000000 dcnum-0.11.3/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-07-22 08:57:15.000000 dcnum-0.11.3/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-22 08:57:15.000000 dcnum-0.11.3/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-22 08:57:15.000000 dcnum-0.11.3/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-22 08:57:15.000000 dcnum-0.11.3/tests/test_feat_background_bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-22 08:57:15.000000 dcnum-0.11.3/tests/test_feat_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-22 08:57:15.000000 dcnum-0.11.3/tests/test_feat_haralick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-22 08:57:15.000000 dcnum-0.11.3/tests/test_feat_moments_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-22 08:57:15.000000 dcnum-0.11.3/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-22 08:57:15.000000 dcnum-0.11.3/tests/test_ppid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-22 08:57:15.000000 dcnum-0.11.3/tests/test_ppid_segm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-22 08:57:15.000000 dcnum-0.11.3/tests/test_read_concat_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-22 08:57:15.000000 dcnum-0.11.3/tests/test_read_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-22 08:57:15.000000 dcnum-0.11.3/tests/test_segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-22 08:57:15.000000 dcnum-0.11.3/tests/test_segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-22 08:57:15.000000 dcnum-0.11.3/tests/test_write_deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-22 08:57:15.000000 dcnum-0.11.3/tests/test_write_writer.py
```

### Comparing `dcnum-0.11.2/.github/workflows/check.yml` & `dcnum-0.11.3/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/.github/workflows/deploy_pypi.yml` & `dcnum-0.11.3/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/.gitignore` & `dcnum-0.11.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/CHANGELOG` & `dcnum-0.11.3/CHANGELOG`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+0.11.3
+ - fix: make sure values in tables dictionary are one-dimensional
 0.11.2
  - meta: increment pipeline ID (texture feature computation)
  - fix: HDF5Data was not pickable
  - fix: HDF5Data did not properly handle tables
  - enh: add context manager for CPUSegmenter
  - enh: record and log execution time of segmentation and feature extraction
  - enh: properly handle border case for computing contour-moments
```

### Comparing `dcnum-0.11.2/LICENSE` & `dcnum-0.11.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/PKG-INFO` & `dcnum-0.11.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.11.2
+Version: 0.11.3
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.11.2/README.rst` & `dcnum-0.11.3/README.rst`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum/feat/event_extractor_manager_thread.py` & `dcnum-0.11.3/dcnum/feat/event_extractor_manager_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum/feat/feat_background/base.py` & `dcnum-0.11.3/dcnum/feat/feat_background/base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum/feat/feat_background/bg_roll_median.py` & `dcnum-0.11.3/dcnum/feat/feat_background/bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum/feat/feat_background/bg_sparse_median.py` & `dcnum-0.11.3/dcnum/feat/feat_background/bg_sparse_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum/feat/feat_brightness/bright_all.py` & `dcnum-0.11.3/dcnum/feat/feat_brightness/bright_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum/feat/feat_moments/mt_legacy.py` & `dcnum-0.11.3/dcnum/feat/feat_moments/mt_legacy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum/feat/feat_texture/tex_all.py` & `dcnum-0.11.3/dcnum/feat/feat_texture/tex_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum/feat/gate.py` & `dcnum-0.11.3/dcnum/feat/gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum/feat/queue_event_extractor.py` & `dcnum-0.11.3/dcnum/feat/queue_event_extractor.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum/meta/ppid.py` & `dcnum-0.11.3/dcnum/meta/ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum/read/cache.py` & `dcnum-0.11.3/dcnum/read/cache.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum/read/hdf5_data.py` & `dcnum-0.11.3/dcnum/read/hdf5_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                     alog = list(h5["logs"][key])
                     if isinstance(alog[0], bytes):
                         alog = [ll.decode("utf") for ll in alog]
                     self.logs[key] = alog
                 for tab in h5.get("tables", []):
                     tabdict = {}
                     for tkey in h5["tables"][tab].dtype.fields.keys():
-                        tabdict[tkey] = h5["tables"][tab][tkey]
+                        tabdict[tkey] = np.squeeze(h5["tables"][tab][tkey])
                     self.tables[tab] = tabdict
 
         if state["pixel_size"] is not None:
             self.pixel_size = state["pixel_size"]
         else:
             # Set known pixel size if possible
             did = self.meta.get("setup:identifier", "EMPTY")
```

### Comparing `dcnum-0.11.2/dcnum/segm/segm_thresh.py` & `dcnum-0.11.3/dcnum/segm/segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum/segm/segmenter.py` & `dcnum-0.11.3/dcnum/segm/segmenter.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum/segm/segmenter_cpu.py` & `dcnum-0.11.3/dcnum/segm/segmenter_cpu.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum/segm/segmenter_gpu.py` & `dcnum-0.11.3/dcnum/segm/segmenter_gpu.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum/segm/segmenter_manager_thread.py` & `dcnum-0.11.3/dcnum/segm/segmenter_manager_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum/write/deque_writer_thread.py` & `dcnum-0.11.3/dcnum/write/deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum/write/queue_collector_thread.py` & `dcnum-0.11.3/dcnum/write/queue_collector_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum/write/writer.py` & `dcnum-0.11.3/dcnum/write/writer.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/dcnum.egg-info/PKG-INFO` & `dcnum-0.11.3/dcnum.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.11.2
+Version: 0.11.3
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.11.2/dcnum.egg-info/SOURCES.txt` & `dcnum-0.11.3/dcnum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/docs/conf.py` & `dcnum-0.11.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/docs/extensions/github_changelog.py` & `dcnum-0.11.3/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/pyproject.toml` & `dcnum-0.11.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/tests/conftest.py` & `dcnum-0.11.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip` & `dcnum-0.11.3/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `dcnum-0.11.3/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/tests/helper_methods.py` & `dcnum-0.11.3/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/tests/test_feat_background_bg_roll_median.py` & `dcnum-0.11.3/tests/test_feat_background_bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/tests/test_feat_brightness.py` & `dcnum-0.11.3/tests/test_feat_brightness.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/tests/test_feat_haralick.py` & `dcnum-0.11.3/tests/test_feat_haralick.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/tests/test_feat_moments_based.py` & `dcnum-0.11.3/tests/test_feat_moments_based.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/tests/test_ppid.py` & `dcnum-0.11.3/tests/test_ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/tests/test_read_concat_hdf5.py` & `dcnum-0.11.3/tests/test_read_concat_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/tests/test_read_hdf5.py` & `dcnum-0.11.3/tests/test_read_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/tests/test_segm_thresh.py` & `dcnum-0.11.3/tests/test_segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/tests/test_segmenter.py` & `dcnum-0.11.3/tests/test_segmenter.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/tests/test_write_deque_writer_thread.py` & `dcnum-0.11.3/tests/test_write_deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.2/tests/test_write_writer.py` & `dcnum-0.11.3/tests/test_write_writer.py`

 * *Files identical despite different names*

