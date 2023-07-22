# Comparing `tmp/pynidm-4.0.0.tar.gz` & `tmp/pynidm-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynidm-4.0.0.tar", last modified: Tue May 30 18:26:26 2023, max compression
+gzip compressed data, was "pynidm-4.1.0.tar", last modified: Sat Jul 22 19:10:05 2023, max compression
```

## Comparing `pynidm-4.0.0.tar` & `pynidm-4.1.0.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.452654 pynidm-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-05-30 18:23:55.000000 pynidm-4.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-30 18:23:22.000000 pynidm-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 18:23:22.000000 pynidm-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    28540 2023-05-30 18:26:26.452654 pynidm-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27721 2023-05-30 18:23:22.000000 pynidm-4.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.424654 pynidm-4.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-30 18:23:22.000000 pynidm-4.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-30 18:23:22.000000 pynidm-4.0.0/docs/REST_API_definition.openapi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-30 18:23:22.000000 pynidm-4.0.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.420654 pynidm-4.0.0/docs/manuscripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.424654 pynidm-4.0.0/docs/manuscripts/linreg_joss/
--rw-r--r--   0 runner    (1001) docker     (123)    33017 2023-05-30 18:23:22.000000 pynidm-4.0.0/docs/manuscripts/linreg_joss/fig-1.png
--rw-r--r--   0 runner    (1001) docker     (123)    22892 2023-05-30 18:23:22.000000 pynidm-4.0.0/docs/manuscripts/linreg_joss/fig-2.png
--rw-r--r--   0 runner    (1001) docker     (123)    62098 2023-05-30 18:23:22.000000 pynidm-4.0.0/docs/manuscripts/linreg_joss/fig-3.png
--rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-05-30 18:23:22.000000 pynidm-4.0.0/docs/manuscripts/linreg_joss/fig-4.png
--rw-r--r--   0 runner    (1001) docker     (123)    22801 2023-05-30 18:23:22.000000 pynidm-4.0.0/docs/manuscripts/linreg_joss/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)    15968 2023-05-30 18:23:22.000000 pynidm-4.0.0/docs/manuscripts/linreg_joss/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-30 18:23:22.000000 pynidm-4.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.424654 pynidm-4.0.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-30 18:23:22.000000 pynidm-4.0.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    35260 2023-05-30 18:23:22.000000 pynidm-4.0.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-30 18:23:22.000000 pynidm-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-30 18:26:26.452654 pynidm-4.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.420654 pynidm-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.428654 pynidm-4.0.0/src/nidm/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.428654 pynidm-4.0.0/src/nidm/core/
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/core/BIDS_Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    27786 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/core/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.432654 pynidm-4.0.0/src/nidm/core/cde_dir/
--rw-r--r--   0 runner    (1001) docker     (123)   114047 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/core/cde_dir/ants_cde.ttl
--rw-r--r--   0 runner    (1001) docker     (123)  1762832 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/core/cde_dir/fs_cde.ttl
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/core/cde_dir/fsl_cde.ttl
--rw-r--r--   0 runner    (1001) docker     (123)    15051 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/core/dot.py
--rw-r--r--   0 runner    (1001) docker     (123)    32283 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/core/provone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.432654 pynidm-4.0.0/src/nidm/core/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/core/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30556 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/core/serializers/provonerdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.440654 pynidm-4.0.0/src/nidm/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/Acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/AcquisitionObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/AssessmentAcquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/AssessmentObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/CDE.py
--rw-r--r--   0 runner    (1001) docker     (123)    23391 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/Core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/DataElement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/DemographicsObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/Derivative.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/DerivativeObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/MRAcquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/MRObject.py
--rw-r--r--   0 runner    (1001) docker     (123)    19843 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/Navigate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/PETAcquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/PETObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/Project.py
--rw-r--r--   0 runner    (1001) docker     (123)    55218 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/Query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/Session.py
--rw-r--r--   0 runner    (1001) docker     (123)   132960 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.444654 pynidm-4.0.0/src/nidm/experiment/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/agent.ttl
--rwxr-xr-x   0 runner    (1001) docker     (123)    65168 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/bidsmri2nidm.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/click_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/click_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/csv2nidm.py
--rw-r--r--   0 runner    (1001) docker     (123)    40521 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/nidm2bids.py
--rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/nidm_affinity_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16230 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/nidm_agglomerative_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/nidm_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/nidm_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    22214 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/nidm_gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    24780 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/nidm_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    32494 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/nidm_linreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/nidm_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/nidm_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/nidm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/nidm_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/nidm_visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)    38609 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/repronim_simple2_brainvolumes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/repronim_simple2_query.txt
--rw-r--r--   0 runner    (1001) docker     (123)    37953 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/rest_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/experiment/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.444654 pynidm-4.0.0/src/nidm/terms/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/terms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.444654 pynidm-4.0.0/src/nidm/terms/imports/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/terms/imports/crypto_import.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/terms/imports/dc_import.ttl
--rw-r--r--   0 runner    (1001) docker     (123)    21156 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/terms/imports/iao_import.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/terms/imports/nfo_import.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/terms/imports/nlx_import.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/terms/imports/obi_import.ttl
--rw-r--r--   0 runner    (1001) docker     (123)    32076 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/terms/imports/ontoneurolog_instruments_import.ttl
--rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/terms/imports/pato_import.ttl
--rw-r--r--   0 runner    (1001) docker     (123)    68790 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/terms/imports/prov-o
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/terms/imports/prv_import.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/terms/imports/qibo_import.ttl
--rw-r--r--   0 runner    (1001) docker     (123)    43335 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/terms/imports/sio_import.ttl
--rw-r--r--   0 runner    (1001) docker     (123)    29175 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/terms/imports/stato_import.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.448654 pynidm-4.0.0/src/nidm/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/workflows/ProcessExecution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/workflows/ProcessSpecification.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-30 18:23:22.000000 pynidm-4.0.0/src/nidm/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.448654 pynidm-4.0.0/src/pynidm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28540 2023-05-30 18:26:26.000000 pynidm-4.0.0/src/pynidm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-30 18:26:26.000000 pynidm-4.0.0/src/pynidm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:26:26.000000 pynidm-4.0.0/src/pynidm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-30 18:26:26.000000 pynidm-4.0.0/src/pynidm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-30 18:26:26.000000 pynidm-4.0.0/src/pynidm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 18:26:26.000000 pynidm-4.0.0/src/pynidm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.424654 pynidm-4.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.448654 pynidm-4.0.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/core/test_provone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.452654 pynidm-4.0.0/tests/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/create_testfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/read_nidm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/termsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/test_experiment_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/test_load_nidmowl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/test_map_vars_to_terms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/test_navigate.py
--rw-r--r--   0 runner    (1001) docker     (123)   260961 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/test_nidm.png
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/test_nidm.ttl
--rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.452654 pynidm-4.0.0/tests/experiment/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/tools/test_nidm_lingreg.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/tools/test_nidm_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    26479 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/tools/test_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/tools/test_rest_dataelements.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/tools/test_rest_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/experiment/tools/test_rest_subjects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:26:26.452654 pynidm-4.0.0/tests/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-30 18:23:22.000000 pynidm-4.0.0/tests/workflows/test_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-30 18:23:22.000000 pynidm-4.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.749708 pynidm-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-07-22 19:09:51.000000 pynidm-4.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-22 19:09:34.000000 pynidm-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-22 19:09:34.000000 pynidm-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    28540 2023-07-22 19:10:05.749708 pynidm-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27721 2023-07-22 19:09:34.000000 pynidm-4.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.729706 pynidm-4.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-22 19:09:34.000000 pynidm-4.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-22 19:09:34.000000 pynidm-4.1.0/docs/REST_API_definition.openapi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-22 19:09:34.000000 pynidm-4.1.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.725706 pynidm-4.1.0/docs/manuscripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.729706 pynidm-4.1.0/docs/manuscripts/linreg_joss/
+-rw-r--r--   0 runner    (1001) docker     (123)    33017 2023-07-22 19:09:34.000000 pynidm-4.1.0/docs/manuscripts/linreg_joss/fig-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22892 2023-07-22 19:09:34.000000 pynidm-4.1.0/docs/manuscripts/linreg_joss/fig-2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62098 2023-07-22 19:09:34.000000 pynidm-4.1.0/docs/manuscripts/linreg_joss/fig-3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-07-22 19:09:34.000000 pynidm-4.1.0/docs/manuscripts/linreg_joss/fig-4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22801 2023-07-22 19:09:34.000000 pynidm-4.1.0/docs/manuscripts/linreg_joss/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)    15968 2023-07-22 19:09:34.000000 pynidm-4.1.0/docs/manuscripts/linreg_joss/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-22 19:09:34.000000 pynidm-4.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.729706 pynidm-4.1.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-07-22 19:09:34.000000 pynidm-4.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35260 2023-07-22 19:09:34.000000 pynidm-4.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-22 19:09:34.000000 pynidm-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-22 19:10:05.749708 pynidm-4.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.725706 pynidm-4.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.729706 pynidm-4.1.0/src/nidm/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.733707 pynidm-4.1.0/src/nidm/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/core/BIDS_Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27786 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/core/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.737707 pynidm-4.1.0/src/nidm/core/cde_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)   114047 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/core/cde_dir/ants_cde.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)  1762832 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/core/cde_dir/fs_cde.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/core/cde_dir/fsl_cde.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)    15051 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/core/dot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32283 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/core/provone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.737707 pynidm-4.1.0/src/nidm/core/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/core/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30556 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/core/serializers/provonerdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.737707 pynidm-4.1.0/src/nidm/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/Acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/AcquisitionObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/AssessmentAcquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/AssessmentObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/CDE.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23391 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/Core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/DataElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/DemographicsObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/Derivative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/DerivativeObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/MRAcquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/MRObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19843 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/Navigate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/PETAcquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/PETObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/Project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55218 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/Query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/Session.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132960 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.741707 pynidm-4.1.0/src/nidm/experiment/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/agent.ttl
+-rwxr-xr-x   0 runner    (1001) docker     (123)    68069 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/bidsmri2nidm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/click_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/click_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/csv2nidm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40521 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/nidm2bids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/nidm_affinity_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16230 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/nidm_agglomerative_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/nidm_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/nidm_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22214 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/nidm_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24780 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/nidm_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32494 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/nidm_linreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/nidm_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/nidm_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/nidm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/nidm_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/nidm_visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38609 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/repronim_simple2_brainvolumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/repronim_simple2_query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    37953 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/rest_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/experiment/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.741707 pynidm-4.1.0/src/nidm/terms/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/terms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.745707 pynidm-4.1.0/src/nidm/terms/imports/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/terms/imports/crypto_import.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/terms/imports/dc_import.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)    21156 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/terms/imports/iao_import.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/terms/imports/nfo_import.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/terms/imports/nlx_import.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/terms/imports/obi_import.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)    32076 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/terms/imports/ontoneurolog_instruments_import.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/terms/imports/pato_import.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)    68790 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/terms/imports/prov-o
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/terms/imports/prv_import.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/terms/imports/qibo_import.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)    43335 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/terms/imports/sio_import.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)    29175 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/terms/imports/stato_import.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.745707 pynidm-4.1.0/src/nidm/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/workflows/ProcessExecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/workflows/ProcessSpecification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-22 19:09:34.000000 pynidm-4.1.0/src/nidm/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.745707 pynidm-4.1.0/src/pynidm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28540 2023-07-22 19:10:05.000000 pynidm-4.1.0/src/pynidm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-22 19:10:05.000000 pynidm-4.1.0/src/pynidm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 19:10:05.000000 pynidm-4.1.0/src/pynidm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-22 19:10:05.000000 pynidm-4.1.0/src/pynidm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-22 19:10:05.000000 pynidm-4.1.0/src/pynidm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-22 19:10:05.000000 pynidm-4.1.0/src/pynidm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.729706 pynidm-4.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.745707 pynidm-4.1.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/core/test_provone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.749708 pynidm-4.1.0/tests/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/create_testfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/read_nidm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/termsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/test_experiment_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/test_load_nidmowl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/test_map_vars_to_terms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/test_navigate.py
+-rw-r--r--   0 runner    (1001) docker     (123)   260961 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/test_nidm.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/test_nidm.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.749708 pynidm-4.1.0/tests/experiment/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/tools/test_nidm_lingreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/tools/test_nidm_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26479 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/tools/test_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/tools/test_rest_dataelements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/tools/test_rest_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/experiment/tools/test_rest_subjects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:10:05.749708 pynidm-4.1.0/tests/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-22 19:09:34.000000 pynidm-4.1.0/tests/workflows/test_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-22 19:09:34.000000 pynidm-4.1.0/tox.ini
```

### Comparing `pynidm-4.0.0/CHANGELOG.md` & `pynidm-4.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+# v4.1.0 (Sat Jul 22 2023)
+
+#### 🚀 Enhancement
+
+- updated nidm model to collections of entities [#378](https://github.com/incf-nidash/PyNIDM/pull/378) ([@dbkeator](https://github.com/dbkeator))
+
+#### Authors: 1
+
+- David Keator ([@dbkeator](https://github.com/dbkeator))
+
+---
+
 # v4.0.0 (Tue May 30 2023)
 
 #### 💥 Breaking Change
 
 - [gh-actions](deps): Bump codespell-project/actions-codespell from 1 to 2 [#375](https://github.com/incf-nidash/PyNIDM/pull/375) ([@dependabot[bot]](https://github.com/dependabot[bot]))
 
 #### 🐛 Bug Fix
```

### Comparing `pynidm-4.0.0/LICENSE` & `pynidm-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/PKG-INFO` & `pynidm-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynidm
-Version: 4.0.0
+Version: 4.1.0
 Summary: PYNIDM: a Python NIDM library and tools
 Home-page: https://github.com/incf-nidash/PyNIDM
 Author: INCF-NIDASH developers
 Author-email: incf-nidash-nidm@googlegroups.com
 Maintainer: INCF-NIDASH developers
 Maintainer-email: incf-nidash-nidm@googlegroups.com
 License: Apache-2.0
```

### Comparing `pynidm-4.0.0/README.rst` & `pynidm-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/docs/Makefile` & `pynidm-4.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/docs/REST_API_definition.openapi.yaml` & `pynidm-4.1.0/docs/REST_API_definition.openapi.yaml`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/docs/make.bat` & `pynidm-4.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/docs/manuscripts/linreg_joss/fig-1.png` & `pynidm-4.1.0/docs/manuscripts/linreg_joss/fig-1.png`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/docs/manuscripts/linreg_joss/fig-2.png` & `pynidm-4.1.0/docs/manuscripts/linreg_joss/fig-2.png`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/docs/manuscripts/linreg_joss/fig-3.png` & `pynidm-4.1.0/docs/manuscripts/linreg_joss/fig-3.png`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/docs/manuscripts/linreg_joss/fig-4.png` & `pynidm-4.1.0/docs/manuscripts/linreg_joss/fig-4.png`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/docs/manuscripts/linreg_joss/paper.bib` & `pynidm-4.1.0/docs/manuscripts/linreg_joss/paper.bib`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/docs/manuscripts/linreg_joss/paper.md` & `pynidm-4.1.0/docs/manuscripts/linreg_joss/paper.md`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/docs/source/conf.py` & `pynidm-4.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/docs/source/index.rst` & `pynidm-4.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/setup.cfg` & `pynidm-4.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/core/BIDS_Constants.py` & `pynidm-4.1.0/src/nidm/core/BIDS_Constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """ BIDS Terms -> NIDM-Exp Mappings
 @author: David Keator <dbkeator@uci.edu>
 """
 from . import Constants
 
 # BIDS dataset_description -> NIDM constants mappings
 dataset_description = {
-    "BIDSVersion": Constants.NIDM_PROJECT_IDENTIFIER,
+    "BIDSVersion": Constants.BIDS["BIDSVersion"],
     "Name": Constants.NIDM_PROJECT_NAME,
     "Procedure": Constants.NIDM_PROJECT_DESCRIPTION,
     "License": Constants.NIDM_PROJECT_LICENSE,
     "ReferencesAndLinks": Constants.NIDM_PROJECT_REFERENCES,
     "Authors": Constants.NIDM_AUTHOR,
     "DatasetDOI": Constants.NIDM_DOI,
     "Funding": Constants.NIDM_FUNDING,
```

### Comparing `pynidm-4.0.0/src/nidm/core/Constants.py` & `pynidm-4.1.0/src/nidm/core/Constants.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/core/cde_dir/ants_cde.ttl` & `pynidm-4.1.0/src/nidm/core/cde_dir/ants_cde.ttl`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/core/cde_dir/fs_cde.ttl` & `pynidm-4.1.0/src/nidm/core/cde_dir/fs_cde.ttl`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/core/cde_dir/fsl_cde.ttl` & `pynidm-4.1.0/src/nidm/core/cde_dir/fsl_cde.ttl`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/core/dot.py` & `pynidm-4.1.0/src/nidm/core/dot.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/core/provone.py` & `pynidm-4.1.0/src/nidm/core/provone.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/core/serializers/__init__.py` & `pynidm-4.1.0/src/nidm/core/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/core/serializers/provonerdf.py` & `pynidm-4.1.0/src/nidm/core/serializers/provonerdf.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/Acquisition.py` & `pynidm-4.1.0/src/nidm/experiment/Acquisition.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/AcquisitionObject.py` & `pynidm-4.1.0/src/nidm/experiment/AcquisitionObject.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/AssessmentAcquisition.py` & `pynidm-4.1.0/src/nidm/experiment/AssessmentAcquisition.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/AssessmentObject.py` & `pynidm-4.1.0/src/nidm/experiment/AssessmentObject.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/CDE.py` & `pynidm-4.1.0/src/nidm/experiment/CDE.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/Core.py` & `pynidm-4.1.0/src/nidm/experiment/Core.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/DataElement.py` & `pynidm-4.1.0/src/nidm/experiment/DataElement.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/DemographicsObject.py` & `pynidm-4.1.0/src/nidm/experiment/DemographicsObject.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/Derivative.py` & `pynidm-4.1.0/src/nidm/experiment/Derivative.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/DerivativeObject.py` & `pynidm-4.1.0/src/nidm/experiment/DerivativeObject.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/MRAcquisition.py` & `pynidm-4.1.0/src/nidm/experiment/MRAcquisition.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/MRObject.py` & `pynidm-4.1.0/src/nidm/experiment/MRObject.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/Navigate.py` & `pynidm-4.1.0/src/nidm/experiment/Navigate.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/PETAcquisition.py` & `pynidm-4.1.0/src/nidm/experiment/PETAcquisition.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/PETObject.py` & `pynidm-4.1.0/src/nidm/experiment/PETObject.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/Project.py` & `pynidm-4.1.0/src/nidm/experiment/Project.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,13 +126,14 @@
             # add session to self.sessions list
             self._dataelements.extend([dataelement])
             # create links in graph
             # session.add_attributes({str("dct:isPartOf"):self})
             # dataelement.add_attributes({pm.QualifiedName(pm.Namespace("dct", Constants.DCT), 'isPartOf'): self})
             return True
 
+
     def __str__(self):
         return "NIDM-Experiment Project Class"
 
     sessions = property(get_sessions, add_sessions)
     derivatives = property(get_derivatives, add_derivatives)
     dataelements = property(get_dataelements, add_dataelements)
```

### Comparing `pynidm-4.0.0/src/nidm/experiment/Query.py` & `pynidm-4.1.0/src/nidm/experiment/Query.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/Session.py` & `pynidm-4.1.0/src/nidm/experiment/Session.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/Utils.py` & `pynidm-4.1.0/src/nidm/experiment/Utils.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/__init__.py` & `pynidm-4.1.0/src/nidm/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/agent.ttl` & `pynidm-4.1.0/src/nidm/experiment/tools/agent.ttl`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/bidsmri2nidm.py` & `pynidm-4.1.0/src/nidm/experiment/tools/bidsmri2nidm.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     Session,
 )
 from nidm.experiment.Utils import (
     add_attributes_with_cde,
     addGitAnnexSources,
     map_variables_to_terms,
 )
+from nidm.experiment.Core import getUUID
 
 
 def getRelPathToBIDS(filepath, bids_root):
     """
     This function returns a relative file link that is relative to the BIDS root directory.
 
     :param filename: absolute path + file
@@ -226,24 +227,25 @@
                 with open(
                     os.path.join(directory, ".bidsignore"), "a", encoding="utf-8"
                 ) as text_file:
                     print(filename_to_add, file=text_file)
 
 
 def addimagingsessions(
-    bids_layout, subject_id, session, participant, directory, img_session=None
+    bids_layout, subject_id, session, participant, directory, collection, img_session=None
 ):
     """
     This function adds imaging acquistions to the NIDM file and deals with BIDS structures potentially having
     separate ses-* directories or not
     :param bids_layout:
     :param subject_id:
-    :param session:
+    :param session: nidm session
     :param participant:
-    :param directory:
+    :param directory: BIDS directory
+    :param collection: prov:collection to add imaging acquisition objects to for BIDS dataset
     :param img_session:
     :return:
     """
     for file_tpl in bids_layout.get(
         subject=subject_id, session=img_session, extension=[".nii", ".nii.gz"]
     ):
         # create an acquisition activity
@@ -277,14 +279,18 @@
                 person=participant[subject_id]["person"],
                 role=Constants.NIDM_PARTICIPANT,
             )
 
         if file_tpl.entities["datatype"] == "anat":
             # do something with anatomicals
             acq_obj = MRObject(acq)
+
+            # Modified 7/22/23 to add acq_entity to collection
+            session.graph.hadMember(collection, acq_obj)
+
             # add image contrast type
             if file_tpl.entities["suffix"] in BIDS_Constants.scans:
                 acq_obj.add_attributes(
                     {
                         Constants.NIDM_IMAGE_CONTRAST_TYPE: BIDS_Constants.scans[
                             file_tpl.entities["suffix"]
                         ]
@@ -421,14 +427,18 @@
                         acq_obj.add_attributes(
                             {BIDS_Constants.json_keys[key]: dataset[key]}
                         )
 
         elif file_tpl.entities["datatype"] == "func":
             # do something with functionals
             acq_obj = MRObject(acq)
+
+            # Modified 7/22/23 to add acq_entity to collection
+            session.graph.hadMember(collection, acq_obj)
+
             # add image contrast type
             if file_tpl.entities["suffix"] in BIDS_Constants.scans:
                 acq_obj.add_attributes(
                     {
                         Constants.NIDM_IMAGE_CONTRAST_TYPE: BIDS_Constants.scans[
                             file_tpl.entities["suffix"]
                         ]
@@ -542,14 +552,17 @@
                 )
             # if there is an events file then this is task-based so create an acquisition object for the task file and link
             if events_file:
                 # for now create acquisition object and link it to the associated scan
                 events_obj = AcquisitionObject(acq)
                 # add prov type, task name as prov:label, and link to filename of events file
 
+                # Modified 7/22/23 to add acq_entity to collection
+                session.graph.hadMember(collection, events_obj)
+
                 events_obj.add_attributes(
                     {
                         PROV_TYPE: Constants.NIDM_MRI_BOLD_EVENTS,
                         BIDS_Constants.json_keys["TaskName"]: json_data["TaskName"],
                         Constants.NIDM_FILENAME: getRelPathToBIDS(
                             events_file[0].filename, directory
                         ),
@@ -622,14 +635,18 @@
                             {BIDS_Constants.json_keys[key]: dataset[key]}
                         )
 
         # DBK added for ASL support 3/16/21
         # WIP: Waiting for pybids > 0.12.4 to support perfusion scans
         elif file_tpl.entities["datatype"] == "perf":
             acq_obj = MRObject(acq)
+
+            # Modified 7/22/23 to add acq_entity to collection
+            session.graph.hadMember(collection, acq_obj)
+
             # add image contrast type
             if file_tpl.entities["suffix"] in BIDS_Constants.scans:
                 acq_obj.add_attributes(
                     {
                         Constants.NIDM_IMAGE_CONTRAST_TYPE: BIDS_Constants.scans[
                             file_tpl.entities["suffix"]
                         ]
@@ -721,14 +738,18 @@
 
         # WIP support B0 maps...waiting for pybids > 0.12.4
         # elif file_tpl.entities['datatype'] == 'fmap':
 
         elif file_tpl.entities["datatype"] == "dwi":
             # do stuff with with dwi scans...
             acq_obj = MRObject(acq)
+
+            # Modified 7/22/23 to add acq_entity to collection
+            session.graph.hadMember(collection, acq_obj)
+
             # add image contrast type
             if file_tpl.entities["suffix"] in BIDS_Constants.scans:
                 acq_obj.add_attributes(
                     {
                         Constants.NIDM_IMAGE_CONTRAST_TYPE: BIDS_Constants.scans[
                             file_tpl.entities["suffix"]
                         ]
@@ -815,14 +836,18 @@
                                     ]: json_data.info[key]
                                 }
                             )
             # for bval and bvec files, what to do with those?
 
             # for now, create new generic acquisition objects, link the files, and associate with the one for the DWI scan?
             acq_obj_bval = AcquisitionObject(acq)
+
+            # Modified 7/22/23 to add acq_entity to collection
+            session.graph.hadMember(collection, acq_obj_bval)
+
             acq_obj_bval.add_attributes({PROV_TYPE: BIDS_Constants.scans["bval"]})
             # add file link to bval files
             acq_obj_bval.add_attributes(
                 {
                     Constants.NIDM_FILENAME: getRelPathToBIDS(
                         join(
                             file_tpl.dirname,
@@ -870,14 +895,18 @@
                 )
             else:
                 logging.info(
                     "WARNING file %s doesn't exist! No SHA512 sum stored in NIDM files...",
                     join(directory, file_tpl.dirname, file_tpl.filename),
                 )
             acq_obj_bvec = AcquisitionObject(acq)
+
+            # Modified 7/22/23 to add acq_entity to collection
+            session.graph.hadMember(collection, acq_obj_bvec)
+
             acq_obj_bvec.add_attributes({PROV_TYPE: BIDS_Constants.scans["bvec"]})
             # add file link to bvec files
             acq_obj_bvec.add_attributes(
                 {
                     Constants.NIDM_FILENAME: getRelPathToBIDS(
                         join(
                             file_tpl.dirname,
@@ -953,30 +982,48 @@
             "Error: BIDS directory %s does not exist!", os.path.join(directory)
         )
         sys.exit(-1)
 
     # create project / nidm-exp doc
     project = Project()
 
+    # 7/22/23 - Modified to create collection of AcquisitionObjects (prov:Entity) to
+    # essentially model the BIDS dataset that we're using to convert data into the
+    # NIDM representation
+    provgraph = project.getGraph()
+    collection = provgraph.collection(Constants.NIIRI[getUUID()])
+    # 7/22/23 add type as bids:Dataset
+    collection.add_attributes({PROV_TYPE: QualifiedName(
+                                Namespace("bids", Constants.BIDS), "Dataset"
+                            )})
+
     # if there are git annex sources then add them
     num_sources = addGitAnnexSources(obj=project.get_uuid(), bids_root=directory)
     # else just add the local path to the dataset
-    if num_sources == 0:
-        project.add_attributes({Constants.PROV["Location"]: "file:/" + directory})
+    #if num_sources == 0:
+        # 7/22/23 - modified to add location attribute to collection of acquisition objects
+    #    collection.add_attributes({Constants.PROV["Location"]: "file:/" + directory})
 
     # add various attributes if they exist in BIDS dataset description file
     for key in dataset:
         # if key from dataset_description file is mapped to term in BIDS_Constants.py then add to NIDM object
         if key in BIDS_Constants.dataset_description:
-            if type(dataset[key]) is list:
+            if key == "Name":
+                # 7/22/23 - modified to add BIDS "Name" attribute to project
                 project.add_attributes(
                     {BIDS_Constants.dataset_description[key]: "".join(dataset[key])}
                 )
+            elif type(dataset[key]) is list:
+                # 7/22/23 - modified to add attributes to collection of acquisition objects
+                collection.add_attributes(
+                    {BIDS_Constants.dataset_description[key]: "".join(dataset[key])}
+                )
             else:
-                project.add_attributes(
+                # 7/22/23 - modified to add attributes to collection of acquisition objects
+                collection.add_attributes(
                     {BIDS_Constants.dataset_description[key]: dataset[key]}
                 )
 
             # added special case to include DOI of project in hash for data element UUIDs to prevent collisions with
             # similar data elements from other projects and make the bids2nidm conversion deterministic in the sense
             # that if you re-convert the same dataset to NIDM, the data element UUIDs will remain the same.
             if key == "DatasetDOI":
@@ -1110,14 +1157,18 @@
 
                 # add session and keep track if it for later using subjid
                 session[subjid] = Session(project)
                 # add acquisition activity
                 acq = AssessmentAcquisition(session=session[subjid])
                 # add acquisition entity
                 acq_entity = AssessmentObject(acquisition=acq)
+
+                # Modified 7/22/23 to add acq_entity to collection
+                provgraph.hadMember(collection,acq_entity)
+
                 # create participant dictionary indexed by subjid to get agen UUIDs for later use
                 participant[subjid] = {}
                 # add agent for this participant to the graph
                 participant[subjid]["person"] = acq.add_person(
                     attributes=({Constants.NIDM_SUBJECTID: row["participant_id"]})
                 )
 
@@ -1150,14 +1201,18 @@
                         }
                     )
 
                 # if there's a participant.json sidecar file then create an entity and
                 # associate it with all the assessment entities
                 if os.path.isfile(os.path.join(directory, "participants.json")):
                     json_sidecar = AcquisitionObject(acquisition=acq)
+
+                    # Modified 7/22/23 to add acq_entity to collection
+                    provgraph.hadMember(collection, json_sidecar)
+
                     json_sidecar.add_attributes(
                         {
                             PROV_TYPE: QualifiedName(
                                 Namespace("bids", Constants.BIDS), "sidecar_file"
                             ),
                             Constants.NIDM_FILENAME: getRelPathToBIDS(
                                 os.path.join(directory, "participants.json"), directory
@@ -1291,23 +1346,25 @@
                 ses.add_attributes({Constants.BIDS["session_number"]: img_session})
                 addimagingsessions(
                     bids_layout=bids_layout,
                     subject_id=subject_id,
                     session=ses,
                     participant=participant,
                     directory=directory,
+                    collection=collection,
                     img_session=img_session,
                 )
         # else we have no ses-* directories in the BIDS layout
         addimagingsessions(
             bids_layout=bids_layout,
             subject_id=subject_id,
             session=Session(project),
             participant=participant,
             directory=directory,
+            collection=collection,
         )
 
     # Added temporarily to support phenotype files
     # for each *.tsv / *.json file pair in the phenotypes directory
     # WIP: ADD VARIABLE -> TERM MAPPING HERE
     cde_pheno = []
     for tsv_file in glob.glob(os.path.join(directory, "phenotype", "*.tsv")):
@@ -1399,17 +1456,20 @@
                 # add acquisition object
                 acq = AssessmentAcquisition(session=session[subjid[1]])
                 # add qualified association with person
                 acq.add_qualified_association(
                     person=participant[subjid[1]]["person"],
                     role=Constants.NIDM_PARTICIPANT,
                 )
-                # add acquisition enttity and associate it with the acquisition activity
+                # add acquisition entity and associate it with the acquisition activity
                 acq_entity = AssessmentObject(acquisition=acq)
 
+                # Modified 7/22/23 to add acq_entity to collection
+                provgraph.hadMember(collection, acq_entity)
+
                 for key, value in row.items():
                     if not value:
                         continue
                     # we're using participant_id in NIDM in agent so don't add to assessment as a triple.
                     # BIDS phenotype files seem to have an index column with no column header variable name so skip those
                     if (not key == "participant_id") and (key != ""):
                         add_attributes_with_cde(
@@ -1425,29 +1485,34 @@
                 )
 
                 # if there are git annex sources for participants.tsv file then add them
                 num_sources = addGitAnnexSources(
                     obj=acq_entity.get_uuid(), bids_root=directory
                 )
                 # else just add the local path to the dataset
-                if num_sources == 0:
-                    acq_entity.add_attributes(
-                        {Constants.PROV["Location"]: "file:/" + tsv_file}
-                    )
+                # 7/22/23 commented out to not add local source if no gitAnnex source found
+                #if num_sources == 0:
+                #    acq_entity.add_attributes(
+                #        {Constants.PROV["Location"]: "file:/" + tsv_file}
+                #    )
 
                 # link associated JSON file if it exists
                 data_dict = os.path.join(
                     directory,
                     "phenotype",
                     os.path.splitext(os.path.basename(tsv_file))[0] + ".json",
                 )
                 if os.path.isfile(data_dict):
                     # if file exists, create a new entity and associate it with the appropriate activity  and a used relationship
                     # with the TSV-related entity
                     json_entity = AcquisitionObject(acquisition=acq)
+
+                    # Modified 7/22/23 to add json_entity to collection
+                    provgraph.hadMember(collection, json_entity)
+
                     json_entity.add_attributes(
                         {
                             PROV_TYPE: Constants.BIDS["sidecar_file"],
                             Constants.NIDM_FILENAME: getRelPathToBIDS(
                                 data_dict, directory
                             ),
                         }
@@ -1457,18 +1522,19 @@
                     # if there are git annex sources for participants.tsv file then add them
                     num_sources = addGitAnnexSources(
                         obj=json_entity.get_uuid(),
                         filepath=data_dict,
                         bids_root=directory,
                     )
                     # else just add the local path to the dataset
-                    if num_sources == 0:
-                        json_entity.add_attributes(
-                            {Constants.PROV["Location"]: "file:/" + data_dict}
-                        )
+                    # 7/22/23 commented out so local source file isn't stored if no gitAnnex sources
+                    #if num_sources == 0:
+                    #    json_entity.add_attributes(
+                    #        {Constants.PROV["Location"]: "file:/" + data_dict}
+                    #    )
 
                     # connect json_entity with acq_entity
                     acq_entity.add_attributes(
                         {Constants.PROV["wasInfluencedBy"]: json_entity.get_uuid()}
                     )
             # append cde_tmp to cde_pheno list for later inclusion in NIDM graph
             cde_pheno.append(cde_tmp)
```

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/csv2nidm.py` & `pynidm-4.1.0/src/nidm/experiment/tools/csv2nidm.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/nidm2bids.py` & `pynidm-4.1.0/src/nidm/experiment/tools/nidm2bids.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/nidm_affinity_propagation.py` & `pynidm-4.1.0/src/nidm/experiment/tools/nidm_affinity_propagation.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/nidm_agglomerative_clustering.py` & `pynidm-4.1.0/src/nidm/experiment/tools/nidm_agglomerative_clustering.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/nidm_concat.py` & `pynidm-4.1.0/src/nidm/experiment/tools/nidm_concat.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/nidm_convert.py` & `pynidm-4.1.0/src/nidm/experiment/tools/nidm_convert.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/nidm_gmm.py` & `pynidm-4.1.0/src/nidm/experiment/tools/nidm_gmm.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/nidm_kmeans.py` & `pynidm-4.1.0/src/nidm/experiment/tools/nidm_kmeans.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/nidm_linreg.py` & `pynidm-4.1.0/src/nidm/experiment/tools/nidm_linreg.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/nidm_merge.py` & `pynidm-4.1.0/src/nidm/experiment/tools/nidm_merge.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/nidm_query.py` & `pynidm-4.1.0/src/nidm/experiment/tools/nidm_query.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/nidm_utils.py` & `pynidm-4.1.0/src/nidm/experiment/tools/nidm_utils.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/nidm_visualize.py` & `pynidm-4.1.0/src/nidm/experiment/tools/nidm_visualize.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/repronim_simple2_brainvolumes.py` & `pynidm-4.1.0/src/nidm/experiment/tools/repronim_simple2_brainvolumes.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/repronim_simple2_query.txt` & `pynidm-4.1.0/src/nidm/experiment/tools/repronim_simple2_query.txt`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/rest.py` & `pynidm-4.1.0/src/nidm/experiment/tools/rest.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/rest_statistics.py` & `pynidm-4.1.0/src/nidm/experiment/tools/rest_statistics.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/experiment/tools/utils.py` & `pynidm-4.1.0/src/nidm/experiment/tools/utils.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/terms/imports/crypto_import.ttl` & `pynidm-4.1.0/src/nidm/terms/imports/crypto_import.ttl`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/terms/imports/dc_import.ttl` & `pynidm-4.1.0/src/nidm/terms/imports/dc_import.ttl`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/terms/imports/iao_import.ttl` & `pynidm-4.1.0/src/nidm/terms/imports/iao_import.ttl`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/terms/imports/nfo_import.ttl` & `pynidm-4.1.0/src/nidm/terms/imports/nfo_import.ttl`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/terms/imports/nlx_import.ttl` & `pynidm-4.1.0/src/nidm/terms/imports/nlx_import.ttl`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/terms/imports/obi_import.ttl` & `pynidm-4.1.0/src/nidm/terms/imports/obi_import.ttl`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/terms/imports/ontoneurolog_instruments_import.ttl` & `pynidm-4.1.0/src/nidm/terms/imports/ontoneurolog_instruments_import.ttl`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/terms/imports/pato_import.ttl` & `pynidm-4.1.0/src/nidm/terms/imports/pato_import.ttl`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/terms/imports/prov-o` & `pynidm-4.1.0/src/nidm/terms/imports/prov-o`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/terms/imports/prv_import.ttl` & `pynidm-4.1.0/src/nidm/terms/imports/prv_import.ttl`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/terms/imports/qibo_import.ttl` & `pynidm-4.1.0/src/nidm/terms/imports/qibo_import.ttl`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/terms/imports/sio_import.ttl` & `pynidm-4.1.0/src/nidm/terms/imports/sio_import.ttl`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/terms/imports/stato_import.ttl` & `pynidm-4.1.0/src/nidm/terms/imports/stato_import.ttl`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/workflows/ProcessExecution.py` & `pynidm-4.1.0/src/nidm/workflows/ProcessExecution.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/nidm/workflows/ProcessSpecification.py` & `pynidm-4.1.0/src/nidm/workflows/ProcessSpecification.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/src/pynidm.egg-info/PKG-INFO` & `pynidm-4.1.0/src/pynidm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynidm
-Version: 4.0.0
+Version: 4.1.0
 Summary: PYNIDM: a Python NIDM library and tools
 Home-page: https://github.com/incf-nidash/PyNIDM
 Author: INCF-NIDASH developers
 Author-email: incf-nidash-nidm@googlegroups.com
 Maintainer: INCF-NIDASH developers
 Maintainer-email: incf-nidash-nidm@googlegroups.com
 License: Apache-2.0
```

### Comparing `pynidm-4.0.0/src/pynidm.egg-info/SOURCES.txt` & `pynidm-4.1.0/src/pynidm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/tests/core/test_provone.py` & `pynidm-4.1.0/tests/core/test_provone.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/tests/experiment/conftest.py` & `pynidm-4.1.0/tests/experiment/conftest.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/tests/experiment/create_testfile.py` & `pynidm-4.1.0/tests/experiment/create_testfile.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/tests/experiment/read_nidm.py` & `pynidm-4.1.0/tests/experiment/read_nidm.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/tests/experiment/termsearch.py` & `pynidm-4.1.0/tests/experiment/termsearch.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/tests/experiment/test_experiment.py` & `pynidm-4.1.0/tests/experiment/test_experiment.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/tests/experiment/test_experiment_basic.py` & `pynidm-4.1.0/tests/experiment/test_experiment_basic.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/tests/experiment/test_map_vars_to_terms.py` & `pynidm-4.1.0/tests/experiment/test_map_vars_to_terms.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/tests/experiment/test_navigate.py` & `pynidm-4.1.0/tests/experiment/test_navigate.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/tests/experiment/test_nidm.png` & `pynidm-4.1.0/tests/experiment/test_nidm.png`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/tests/experiment/test_nidm.ttl` & `pynidm-4.1.0/tests/experiment/test_nidm.ttl`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/tests/experiment/test_query.py` & `pynidm-4.1.0/tests/experiment/test_query.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/tests/experiment/tools/test_nidm_lingreg.py` & `pynidm-4.1.0/tests/experiment/tools/test_nidm_lingreg.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/tests/experiment/tools/test_rest.py` & `pynidm-4.1.0/tests/experiment/tools/test_rest.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/tests/experiment/tools/test_rest_dataelements.py` & `pynidm-4.1.0/tests/experiment/tools/test_rest_dataelements.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/tests/experiment/tools/test_rest_statistics.py` & `pynidm-4.1.0/tests/experiment/tools/test_rest_statistics.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/tests/experiment/tools/test_rest_subjects.py` & `pynidm-4.1.0/tests/experiment/tools/test_rest_subjects.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/tests/workflows/test_workflows.py` & `pynidm-4.1.0/tests/workflows/test_workflows.py`

 * *Files identical despite different names*

### Comparing `pynidm-4.0.0/tox.ini` & `pynidm-4.1.0/tox.ini`

 * *Files identical despite different names*

