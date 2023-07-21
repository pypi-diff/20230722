# Comparing `tmp/arize-7.1.0.tar.gz` & `tmp/arize-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arize-7.1.0.tar", last modified: Mon Jun 26 21:01:01 2023, max compression
+gzip compressed data, was "arize-7.2.0.tar", last modified: Fri Jul 21 22:41:29 2023, max compression
```

## Comparing `arize-7.1.0.tar` & `arize-7.2.0.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.283121 arize-7.1.0/
--rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-06-23 05:09:35.000000 arize-7.1.0/LICENSE.md
--rw-r--r--   0 kiko       (501) staff       (20)       65 2023-06-23 05:09:35.000000 arize-7.1.0/MANIFEST.in
--rw-r--r--   0 kiko       (501) staff       (20)    12555 2023-06-26 21:01:01.283336 arize-7.1.0/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-06-23 05:09:35.000000 arize-7.1.0/README.md
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.231870 arize-7.1.0/arize/
--rw-r--r--   0 kiko       (501) staff       (20)       22 2023-06-26 20:59:58.000000 arize-7.1.0/arize/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    31982 2023-06-26 20:59:58.000000 arize-7.1.0/arize/api.py
--rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-06-23 05:09:35.000000 arize-7.1.0/arize/bounded_executor.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.245214 arize-7.1.0/arize/examples/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.1.0/arize/examples/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-06-23 05:09:35.000000 arize-7.1.0/arize/examples/bulk_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-06-23 05:09:35.000000 arize-7.1.0/arize/examples/bulk_client_shap.py
--rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-06-23 05:09:35.000000 arize-7.1.0/arize/examples/client_shap_values.py
--rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-06-23 05:09:35.000000 arize-7.1.0/arize/examples/log_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-06-23 05:09:35.000000 arize-7.1.0/arize/examples/log_pandas_dataframe.py
--rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-06-23 05:09:35.000000 arize-7.1.0/arize/examples/preproduction_client.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.247189 arize-7.1.0/arize/exporter/
--rw-r--r--   0 kiko       (501) staff       (20)      146 2023-06-23 05:09:35.000000 arize-7.1.0/arize/exporter/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.251312 arize-7.1.0/arize/exporter/core/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.1.0/arize/exporter/core/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    10940 2023-06-23 18:59:38.000000 arize-7.1.0/arize/exporter/core/client.py
--rw-r--r--   0 kiko       (501) staff       (20)     1343 2023-06-23 18:59:38.000000 arize-7.1.0/arize/exporter/core/query.py
--rw-r--r--   0 kiko       (501) staff       (20)     3464 2023-06-23 18:59:38.000000 arize-7.1.0/arize/exporter/core/session.py
--rw-r--r--   0 kiko       (501) staff       (20)     2406 2023-06-23 18:59:38.000000 arize-7.1.0/arize/exporter/publicexporter_pb2.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.256106 arize-7.1.0/arize/exporter/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.1.0/arize/exporter/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1422 2023-06-23 18:59:38.000000 arize-7.1.0/arize/exporter/utils/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)      727 2023-06-23 18:59:38.000000 arize-7.1.0/arize/exporter/utils/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)     5793 2023-06-23 18:59:38.000000 arize-7.1.0/arize/exporter/utils/schema_parser.py
--rw-r--r--   0 kiko       (501) staff       (20)      778 2023-06-23 18:59:38.000000 arize-7.1.0/arize/exporter/utils/validation.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.257608 arize-7.1.0/arize/pandas/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.266926 arize-7.1.0/arize/pandas/embeddings/
--rw-r--r--   0 kiko       (501) staff       (20)      124 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/embeddings/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/embeddings/auto_generator.py
--rw-r--r--   0 kiko       (501) staff       (20)     6988 2023-06-23 18:59:38.000000 arize-7.1.0/arize/pandas/embeddings/base_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      213 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/embeddings/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     2023 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/embeddings/cv_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      753 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/embeddings/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)      571 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/embeddings/models.py
--rw-r--r--   0 kiko       (501) staff       (20)     3675 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/embeddings/nlp_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)     5853 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/embeddings/tabular_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      412 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/embeddings/usecases.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.267733 arize-7.1.0/arize/pandas/generative/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/generative/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.270194 arize-7.1.0/arize/pandas/generative/llm_evaluation/
--rw-r--r--   0 kiko       (501) staff       (20)      160 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/generative/llm_evaluation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      183 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/generative/llm_evaluation/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)    12178 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/generative/llm_evaluation/hf_metrics.py
--rw-r--r--   0 kiko       (501) staff       (20)    22779 2023-06-23 18:59:38.000000 arize-7.1.0/arize/pandas/logger.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.271744 arize-7.1.0/arize/pandas/surrogate_explainer/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/surrogate_explainer/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     5090 2023-06-23 18:59:38.000000 arize-7.1.0/arize/pandas/surrogate_explainer/mimic.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.274302 arize-7.1.0/arize/pandas/validation/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/validation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    26601 2023-06-23 05:09:35.000000 arize-7.1.0/arize/pandas/validation/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)    70456 2023-06-23 18:59:38.000000 arize-7.1.0/arize/pandas/validation/validator.py
--rw-r--r--   0 kiko       (501) staff       (20)    50975 2023-06-26 20:59:58.000000 arize-7.1.0/arize/public_pb2.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.280500 arize-7.1.0/arize/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.1.0/arize/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      619 2023-06-23 05:09:35.000000 arize-7.1.0/arize/utils/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-06-23 05:09:35.000000 arize-7.1.0/arize/utils/logging.py
--rw-r--r--   0 kiko       (501) staff       (20)     5725 2023-06-23 05:09:35.000000 arize-7.1.0/arize/utils/model_mapping.json
--rw-r--r--   0 kiko       (501) staff       (20)    24659 2023-06-23 18:59:38.000000 arize-7.1.0/arize/utils/types.py
--rw-r--r--   0 kiko       (501) staff       (20)     7620 2023-06-23 05:09:35.000000 arize-7.1.0/arize/utils/utils.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.237134 arize-7.1.0/arize.egg-info/
--rw-r--r--   0 kiko       (501) staff       (20)    12555 2023-06-26 21:01:01.000000 arize-7.1.0/arize.egg-info/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)     1879 2023-06-26 21:01:01.000000 arize-7.1.0/arize.egg-info/SOURCES.txt
--rw-r--r--   0 kiko       (501) staff       (20)        1 2023-06-26 21:01:01.000000 arize-7.1.0/arize.egg-info/dependency_links.txt
--rw-r--r--   0 kiko       (501) staff       (20)      429 2023-06-26 21:01:01.000000 arize-7.1.0/arize.egg-info/requires.txt
--rw-r--r--   0 kiko       (501) staff       (20)        6 2023-06-26 21:01:01.000000 arize-7.1.0/arize.egg-info/top_level.txt
--rw-r--r--   0 kiko       (501) staff       (20)      167 2023-06-23 05:09:35.000000 arize-7.1.0/pyproject.toml
--rw-r--r--   0 kiko       (501) staff       (20)     1517 2023-06-26 21:01:01.284280 arize-7.1.0/setup.cfg
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 21:01:01.282373 arize-7.1.0/tests/
--rw-r--r--   0 kiko       (501) staff       (20)    59500 2023-06-26 20:59:58.000000 arize-7.1.0/tests/test_api.py
--rw-r--r--   0 kiko       (501) staff       (20)      952 2023-06-23 05:09:35.000000 arize-7.1.0/tests/test_utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.251542 arize-7.2.0/
+-rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-06-23 05:09:35.000000 arize-7.2.0/LICENSE.md
+-rw-r--r--   0 kiko       (501) staff       (20)       65 2023-06-23 05:09:35.000000 arize-7.2.0/MANIFEST.in
+-rw-r--r--   0 kiko       (501) staff       (20)    12555 2023-07-21 22:41:29.251891 arize-7.2.0/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-06-23 05:09:35.000000 arize-7.2.0/README.md
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.182958 arize-7.2.0/arize/
+-rw-r--r--   0 kiko       (501) staff       (20)       22 2023-07-21 22:31:43.000000 arize-7.2.0/arize/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    32195 2023-07-21 22:31:43.000000 arize-7.2.0/arize/api.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-06-23 05:09:35.000000 arize-7.2.0/arize/bounded_executor.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.200987 arize-7.2.0/arize/examples/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.2.0/arize/examples/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-06-23 05:09:35.000000 arize-7.2.0/arize/examples/bulk_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-06-23 05:09:35.000000 arize-7.2.0/arize/examples/bulk_client_shap.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-06-23 05:09:35.000000 arize-7.2.0/arize/examples/client_shap_values.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-06-23 05:09:35.000000 arize-7.2.0/arize/examples/log_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-06-23 05:09:35.000000 arize-7.2.0/arize/examples/log_pandas_dataframe.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-06-23 05:09:35.000000 arize-7.2.0/arize/examples/preproduction_client.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.202793 arize-7.2.0/arize/exporter/
+-rw-r--r--   0 kiko       (501) staff       (20)      146 2023-06-23 05:09:35.000000 arize-7.2.0/arize/exporter/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.206128 arize-7.2.0/arize/exporter/core/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.2.0/arize/exporter/core/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    10940 2023-06-30 17:46:28.000000 arize-7.2.0/arize/exporter/core/client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1343 2023-06-30 17:46:28.000000 arize-7.2.0/arize/exporter/core/query.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3464 2023-06-30 17:46:28.000000 arize-7.2.0/arize/exporter/core/session.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2406 2023-07-18 18:29:39.000000 arize-7.2.0/arize/exporter/publicexporter_pb2.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.210171 arize-7.2.0/arize/exporter/utils/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.2.0/arize/exporter/utils/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1422 2023-06-30 17:46:28.000000 arize-7.2.0/arize/exporter/utils/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)      727 2023-06-30 17:46:28.000000 arize-7.2.0/arize/exporter/utils/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5793 2023-06-30 17:46:28.000000 arize-7.2.0/arize/exporter/utils/schema_parser.py
+-rw-r--r--   0 kiko       (501) staff       (20)      778 2023-06-30 17:46:28.000000 arize-7.2.0/arize/exporter/utils/validation.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.211445 arize-7.2.0/arize/pandas/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.221576 arize-7.2.0/arize/pandas/embeddings/
+-rw-r--r--   0 kiko       (501) staff       (20)      124 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/embeddings/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/embeddings/auto_generator.py
+-rw-r--r--   0 kiko       (501) staff       (20)     6988 2023-06-30 17:46:28.000000 arize-7.2.0/arize/pandas/embeddings/base_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      213 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/embeddings/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2023 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/embeddings/cv_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      753 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/embeddings/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)      571 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/embeddings/models.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3675 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/embeddings/nlp_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5853 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/embeddings/tabular_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      412 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/embeddings/usecases.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.222708 arize-7.2.0/arize/pandas/generative/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/generative/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.226607 arize-7.2.0/arize/pandas/generative/llm_evaluation/
+-rw-r--r--   0 kiko       (501) staff       (20)      160 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/generative/llm_evaluation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      183 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/generative/llm_evaluation/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)    12178 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/generative/llm_evaluation/hf_metrics.py
+-rw-r--r--   0 kiko       (501) staff       (20)    24029 2023-07-21 22:31:43.000000 arize-7.2.0/arize/pandas/logger.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.229801 arize-7.2.0/arize/pandas/surrogate_explainer/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/surrogate_explainer/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5090 2023-06-30 17:46:28.000000 arize-7.2.0/arize/pandas/surrogate_explainer/mimic.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.234976 arize-7.2.0/arize/pandas/validation/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.2.0/arize/pandas/validation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    26601 2023-07-21 00:34:26.000000 arize-7.2.0/arize/pandas/validation/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)    70724 2023-07-21 22:31:43.000000 arize-7.2.0/arize/pandas/validation/validator.py
+-rw-r--r--   0 kiko       (501) staff       (20)    50975 2023-07-18 18:29:39.000000 arize-7.2.0/arize/public_pb2.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.247833 arize-7.2.0/arize/utils/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.2.0/arize/utils/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      743 2023-07-21 22:31:43.000000 arize-7.2.0/arize/utils/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1163 2023-07-21 22:31:43.000000 arize-7.2.0/arize/utils/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-06-23 05:09:35.000000 arize-7.2.0/arize/utils/logging.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5725 2023-06-23 05:09:35.000000 arize-7.2.0/arize/utils/model_mapping.json
+-rw-r--r--   0 kiko       (501) staff       (20)    24659 2023-06-30 17:46:28.000000 arize-7.2.0/arize/utils/types.py
+-rw-r--r--   0 kiko       (501) staff       (20)     7620 2023-06-23 05:09:35.000000 arize-7.2.0/arize/utils/utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.188408 arize-7.2.0/arize.egg-info/
+-rw-r--r--   0 kiko       (501) staff       (20)    12555 2023-07-21 22:41:29.000000 arize-7.2.0/arize.egg-info/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)     1901 2023-07-21 22:41:29.000000 arize-7.2.0/arize.egg-info/SOURCES.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        1 2023-07-21 22:41:29.000000 arize-7.2.0/arize.egg-info/dependency_links.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      429 2023-07-21 22:41:29.000000 arize-7.2.0/arize.egg-info/requires.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        6 2023-07-21 22:41:29.000000 arize-7.2.0/arize.egg-info/top_level.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      167 2023-06-23 05:09:35.000000 arize-7.2.0/pyproject.toml
+-rw-r--r--   0 kiko       (501) staff       (20)     1517 2023-07-21 22:41:29.254223 arize-7.2.0/setup.cfg
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-07-21 22:41:29.250500 arize-7.2.0/tests/
+-rw-r--r--   0 kiko       (501) staff       (20)    61734 2023-07-21 22:31:43.000000 arize-7.2.0/tests/test_api.py
+-rw-r--r--   0 kiko       (501) staff       (20)      952 2023-06-23 05:09:35.000000 arize-7.2.0/tests/test_utils.py
```

### Comparing `arize-7.1.0/LICENSE.md` & `arize-7.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/PKG-INFO` & `arize-7.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.1.0
+Version: 7.2.0
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.1.0/README.md` & `arize-7.2.0/README.md`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/api.py` & `arize-7.2.0/arize/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # type: ignore[pb2]
 import concurrent.futures as cf
+import os
 import time
 from typing import Dict, Optional, Tuple, Union
 
 from arize.pandas.validation.errors import InvalidAdditionalHeaders
 from arize.utils.constants import (
+    API_KEY_ENVVAR_NAME,
     MAX_FUTURE_YEARS_FROM_CURRENT_TIME,
     MAX_PAST_YEARS_FROM_CURRENT_TIME,
     MAX_PREDICTION_ID_LEN,
     MAX_TAG_LENGTH,
     MIN_PREDICTION_ID_LEN,
+    SPACE_KEY_ENVVAR_NAME,
 )
 from arize.utils.logging import logger
 from google.protobuf.json_format import MessageToDict
 from google.protobuf.wrappers_pb2 import BoolValue, DoubleValue
 from requests_futures.sessions import FuturesSession
 
 from . import public_pb2 as pb2
 from .__init__ import __version__
 from .bounded_executor import BoundedExecutor
+from .utils.errors import AuthError
 from .utils.types import (
     CATEGORICAL_MODEL_TYPES,
     NUMERIC_MODEL_TYPES,
     Embedding,
     Environments,
     ModelTypes,
     ObjectDetectionLabel,
@@ -60,16 +64,16 @@
 class Client:
     """
     Arize API Client to log model predictions and actuals to the Arize AI platform
     """
 
     def __init__(
         self,
-        api_key: str,
-        space_key: str,
+        api_key: Optional[str] = None,
+        space_key: Optional[str] = None,
         uri: Optional[str] = "https://api.arize.com/v1",
         max_workers: Optional[int] = 8,
         max_queue_bound: Optional[int] = 5000,
         timeout: Optional[int] = 200,
         additional_headers: Optional[Dict[str, str]] = None,
     ) -> None:
         """
@@ -89,19 +93,21 @@
                 generated for publishing to Arize. Defaults to 5000.
             timeout (int, optional): How long to wait for the server to send data before giving
                 up. Defaults to 200.
             additional_headers (Dict[str, str], optional): Dictionary of additional headers to
                 append to request
         """
 
-        if not isinstance(space_key, str):
-            raise TypeError(f"space_key {space_key} is type {type(space_key)}, but must be a str")
-        self._uri = f"{uri}/log"
+        api_key = api_key or os.getenv(API_KEY_ENVVAR_NAME)
+        space_key = space_key or os.getenv(SPACE_KEY_ENVVAR_NAME)
+        if api_key is None or space_key is None:
+            raise AuthError(api_key, space_key)
         self._api_key = api_key
         self._space_key = space_key
+        self._uri = f"{uri}/log"
         self._timeout = timeout
         self._session = FuturesSession(executor=BoundedExecutor(max_queue_bound, max_workers))
         # Grpc-Metadata prefix is required to pass non-standard md through via grpc-gateway
         self._headers = {
             "authorization": api_key,
             "Grpc-Metadata-space": space_key,
             "Grpc-Metadata-sdk-language": "python",
```

### Comparing `arize-7.1.0/arize/bounded_executor.py` & `arize-7.2.0/arize/bounded_executor.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/examples/bulk_client.py` & `arize-7.2.0/arize/examples/bulk_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/examples/bulk_client_shap.py` & `arize-7.2.0/arize/examples/bulk_client_shap.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/examples/client_shap_values.py` & `arize-7.2.0/arize/examples/client_shap_values.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/examples/log_client.py` & `arize-7.2.0/arize/examples/log_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/examples/log_pandas_dataframe.py` & `arize-7.2.0/arize/examples/log_pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/examples/preproduction_client.py` & `arize-7.2.0/arize/examples/preproduction_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/exporter/core/client.py` & `arize-7.2.0/arize/exporter/core/client.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/exporter/core/query.py` & `arize-7.2.0/arize/exporter/core/query.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/exporter/core/session.py` & `arize-7.2.0/arize/exporter/core/session.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/exporter/publicexporter_pb2.py` & `arize-7.2.0/arize/exporter/publicexporter_pb2.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/exporter/utils/constants.py` & `arize-7.2.0/arize/exporter/utils/constants.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/exporter/utils/errors.py` & `arize-7.2.0/arize/exporter/utils/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/exporter/utils/schema_parser.py` & `arize-7.2.0/arize/exporter/utils/schema_parser.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/exporter/utils/validation.py` & `arize-7.2.0/arize/exporter/utils/validation.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/pandas/embeddings/auto_generator.py` & `arize-7.2.0/arize/pandas/embeddings/auto_generator.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/pandas/embeddings/base_generators.py` & `arize-7.2.0/arize/pandas/embeddings/base_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/pandas/embeddings/cv_generators.py` & `arize-7.2.0/arize/pandas/embeddings/cv_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/pandas/embeddings/errors.py` & `arize-7.2.0/arize/pandas/embeddings/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/pandas/embeddings/models.py` & `arize-7.2.0/arize/pandas/embeddings/models.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/pandas/embeddings/nlp_generators.py` & `arize-7.2.0/arize/pandas/embeddings/nlp_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/pandas/embeddings/tabular_generators.py` & `arize-7.2.0/arize/pandas/embeddings/tabular_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/pandas/generative/llm_evaluation/hf_metrics.py` & `arize-7.2.0/arize/pandas/generative/llm_evaluation/hf_metrics.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/pandas/logger.py` & `arize-7.2.0/arize/pandas/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # type: ignore[pb2]
 import base64
+import os
+import shutil
 import tempfile
 from typing import Dict, List, Optional
 
 import pandas as pd
 import pandas.api.types as ptypes
 import pyarrow as pa
 import requests
 
 from .. import public_pb2 as pb2
 from ..__init__ import __version__
+from ..utils.constants import API_KEY_ENVVAR_NAME, SPACE_KEY_ENVVAR_NAME
+from ..utils.errors import AuthError
 from ..utils.logging import logger
 from ..utils.types import (
     CATEGORICAL_MODEL_TYPES,
     NUMERIC_MODEL_TYPES,
     Environments,
     Metrics,
     ModelTypes,
@@ -28,16 +32,16 @@
     """
     Arize API Client to log predictions and actuals to the Arize platform from
     pandas.DataFrames
     """
 
     def __init__(
         self,
-        api_key: str,
-        space_key: str,
+        api_key: Optional[str] = None,
+        space_key: Optional[str] = None,
         uri: Optional[str] = "https://api.arize.com/v1",
         additional_headers: Optional[Dict[str, str]] = None,
     ) -> None:
         """
         Initializes the Arize Client
 
         Arguments:
@@ -47,14 +51,18 @@
             space_key (str): Arize provided identifier to connect records to spaces. Located on
                 the data upload page.
             uri (str, optional): URI endpoint to send your records to Arize AI. Defaults to
                 "https://api.arize.com/v1".
             additional_headers (Dict[str, str], optional): Dictionary of additional headers to
                 append to request
         """
+        api_key = api_key or os.getenv(API_KEY_ENVVAR_NAME)
+        space_key = space_key or os.getenv(SPACE_KEY_ENVVAR_NAME)
+        if api_key is None or space_key is None:
+            raise AuthError(api_key, space_key)
         self._api_key = api_key
         self._space_key = space_key
         self._files_uri = uri + "/pandas_arrow"
         self._headers = {
             "authorization": self._api_key,
             "space": self._space_key,
             "sdk-language": "python",
@@ -414,31 +422,43 @@
         base64_schema = base64.b64encode(s.SerializeToString())
 
         # limit the potential size of http headers to under 64 kilobytes
         if len(base64_schema) > 63000:
             raise ValueError("The schema (after removing unnecessary columns) is too large.")
 
         if path is None:
-            f = tempfile.NamedTemporaryFile()
-            tmp_file = f.name
+            tmp_dir = tempfile.mkdtemp()
+            fd, tmp_file = tempfile.mkstemp(dir=tmp_dir)
+            # This way of handling temp files is not ideal, but necessary for it to work
+            # for Windows machines. A Windows corner case is on exiting a tempfile context manager,
+            # PermissionError can be thrown if non-writable files are placed into a
+            # tempfile.TemporaryDirectory. Python 3.10 fixed this issue by adding argument
+            # TemporaryDirectory(ignore_cleanup_errors=True). See code that will work well across
+            # operating systems: https://www.scivision.dev/python-tempfile-permission-error-windows/
         else:
             tmp_file = path
 
         try:
             if verbose:
                 logger.info("Writing table to temporary file: ", tmp_file)
             writer = pa.ipc.new_stream(tmp_file, pa_schema)
             writer.write_table(ta, max_chunksize=65536)
             writer.close()
             if verbose:
                 logger.info("Sending file to Arize")
             response = self._post_file(tmp_file, base64_schema, sync, timeout)
         finally:
             if path is None:
-                f.close()
+                # NOTE: This try-catch should also be updated/removed when
+                # Python >=3.10 is required, see comment above
+                try:
+                    os.close(fd)
+                    shutil.rmtree(tmp_dir)
+                except PermissionError:
+                    pass
 
         try:
             logger.info(f"Success! Check out your data at {reconstruct_url(response)}")
 
             if not schema.has_prediction_columns():
                 logger.warning(
                     "Logging actuals without any predictions may result in "
```

### Comparing `arize-7.1.0/arize/pandas/surrogate_explainer/mimic.py` & `arize-7.2.0/arize/pandas/surrogate_explainer/mimic.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/pandas/validation/errors.py` & `arize-7.2.0/arize/pandas/validation/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/pandas/validation/validator.py` & `arize-7.2.0/arize/pandas/validation/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1219,16 +1219,17 @@
     def _check_value_tag(dataframe: pd.DataFrame, schema: Schema) -> List[err.InvalidTagLength]:
         if schema.tag_column_names is not None and len(dataframe):
             wrong_tag_cols = []
             for col in schema.tag_column_names:
                 # This is to be defensive, validate_params should guarantee that this column is in
                 # the dataframe, via _check_missing_columns, and return an error before reaching this
                 # block if not
-                if col in dataframe.columns:
-                    max_tag_len = len(str(dataframe[col].agg(["max"])["max"]))
+                # Checks max tag length when any values in a column are strings
+                if col in dataframe.columns and dataframe[col].map(type).eq(str).any():
+                    max_tag_len = dataframe[col].apply(_check_value_tag_string_length_helper).max()
                     if max_tag_len > MAX_TAG_LENGTH:
                         wrong_tag_cols.append(col)
             if wrong_tag_cols:
                 return [err.InvalidTagLength(wrong_tag_cols)]
         return []
 
     @staticmethod
@@ -1598,14 +1599,21 @@
             if sc_col_name is not None:
                 error = _check_value_bounding_boxes_scores_helper(dataframe[sc_col_name])
                 if error is not None:
                     errors.append(error)
         return errors
 
 
+def _check_value_tag_string_length_helper(x):
+    if isinstance(x, str):
+        return len(x)
+    else:
+        return 0
+
+
 def _check_value_bounding_boxes_coordinates_helper(
     coordinates_col: pd.Series,
 ) -> Union[err.InvalidBoundingBoxesCoordinates, None]:
     def check(boxes):
         # We allow for zero boxes. None coordinates list is not allowed (will break following tests:
         # 'NoneType is not iterable')
         if boxes is None:
```

### Comparing `arize-7.1.0/arize/public_pb2.py` & `arize-7.2.0/arize/public_pb2.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/utils/logging.py` & `arize-7.2.0/arize/utils/logging.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/utils/model_mapping.json` & `arize-7.2.0/arize/utils/model_mapping.json`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/utils/types.py` & `arize-7.2.0/arize/utils/types.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize/utils/utils.py` & `arize-7.2.0/arize/utils/utils.py`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/arize.egg-info/PKG-INFO` & `arize-7.2.0/arize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.1.0
+Version: 7.2.0
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.1.0/arize.egg-info/SOURCES.txt` & `arize-7.2.0/arize.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -49,13 +49,14 @@
 arize/pandas/surrogate_explainer/__init__.py
 arize/pandas/surrogate_explainer/mimic.py
 arize/pandas/validation/__init__.py
 arize/pandas/validation/errors.py
 arize/pandas/validation/validator.py
 arize/utils/__init__.py
 arize/utils/constants.py
+arize/utils/errors.py
 arize/utils/logging.py
 arize/utils/model_mapping.json
 arize/utils/types.py
 arize/utils/utils.py
 tests/test_api.py
 tests/test_utils.py
```

### Comparing `arize-7.1.0/setup.cfg` & `arize-7.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `arize-7.1.0/tests/test_api.py` & `arize-7.2.0/tests/test_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+import os
 import time
 from pathlib import Path
 
 import arize.public_pb2 as pb2
 import numpy as np
 import pandas as pd
 import pytest
 from arize import __version__ as arize_version
 from arize.api import Client, Embedding
 from arize.pandas.validation.errors import InvalidAdditionalHeaders
 from arize.utils.constants import (
+    API_KEY_ENVVAR_NAME,
     MAX_FUTURE_YEARS_FROM_CURRENT_TIME,
     MAX_PAST_YEARS_FROM_CURRENT_TIME,
     MAX_PREDICTION_ID_LEN,
     MAX_TAG_LENGTH,
     MIN_PREDICTION_ID_LEN,
+    SPACE_KEY_ENVVAR_NAME,
 )
+from arize.utils.errors import AuthError
 from arize.utils.types import (
     Environments,
     ModelTypes,
     ObjectDetectionLabel,
     RankingActualLabel,
     RankingPredictionLabel,
 )
@@ -1543,9 +1547,63 @@
         "Grpc-Metadata-language-version": get_python_version(),
         "Grpc-Metadata-sdk-version": arize_version,
         "JWT": "FAKE_VALUE",
     }
     assert c._headers == expected
 
 
+def test_invalid_client_auth_passed_vars():
+    with pytest.raises(AuthError) as excinfo:
+        _ = Client()
+    assert excinfo.value.__str__() == AuthError(None, None).error_message()
+    assert "Missing: ['api_key', 'space_key']" in str(excinfo.value)
+
+    with pytest.raises(AuthError) as excinfo:
+        _ = Client(space_key=inputs["space_key"])
+    assert excinfo.value.__str__() == AuthError(None, inputs["space_key"]).error_message()
+    assert "Missing: ['api_key']" in str(excinfo.value)
+
+    with pytest.raises(AuthError) as excinfo:
+        _ = Client(api_key=inputs["api_key"])
+    assert excinfo.value.__str__() == AuthError(inputs["api_key"], None).error_message()
+    assert "Missing: ['space_key']" in str(excinfo.value)
+
+    # acceptable input
+    try:
+        _ = Client(space_key=inputs["space_key"], api_key=inputs["api_key"])
+    except Exception:
+        pytest.fail("Unexpected error!")
+
+
+def test_invalid_client_auth_environment_vars():
+    with pytest.raises(AuthError) as excinfo:
+        _ = Client()
+    assert excinfo.value.__str__() == AuthError(None, None).error_message()
+    assert "Missing: ['api_key', 'space_key']" in str(excinfo.value)
+
+    os.environ[SPACE_KEY_ENVVAR_NAME] = inputs["space_key"]
+    with pytest.raises(AuthError) as excinfo:
+        c = Client()
+        assert c._space_key == inputs["space_key"]
+    assert excinfo.value.__str__() == AuthError(None, inputs["space_key"]).error_message()
+    assert "Missing: ['api_key']" in str(excinfo.value)
+
+    os.environ.pop(SPACE_KEY_ENVVAR_NAME)
+    os.environ[API_KEY_ENVVAR_NAME] = inputs["api_key"]
+    with pytest.raises(AuthError) as excinfo:
+        c = Client()
+        assert c._api_key == inputs["api_key"]
+    assert excinfo.value.__str__() == AuthError(inputs["api_key"], None).error_message()
+    assert "Missing: ['space_key']" in str(excinfo.value)
+
+    # acceptable input
+    os.environ[SPACE_KEY_ENVVAR_NAME] = inputs["space_key"]
+    try:
+        c = Client()
+    except Exception:
+        pytest.fail("Unexpected error!")
+    assert c._space_key == inputs["space_key"]
+    assert c._api_key == inputs["api_key"]
+
+
 if __name__ == "__main__":
     raise SystemExit(pytest.main([__file__]))
```

### Comparing `arize-7.1.0/tests/test_utils.py` & `arize-7.2.0/tests/test_utils.py`

 * *Files identical despite different names*

