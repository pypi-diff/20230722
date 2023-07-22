# Comparing `tmp/bytetrade-recommend-model-sdk-0.0.26.tar.gz` & `tmp/bytetrade-recommend-model-sdk-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.26.tar", last modified: Mon Jul 17 01:45:56 2023, max compression
+gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.27.tar", last modified: Sat Jul 22 02:13:46 2023, max compression
```

## Comparing `bytetrade-recommend-model-sdk-0.0.26.tar` & `bytetrade-recommend-model-sdk-0.0.27.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.104727 bytetrade-recommend-model-sdk-0.0.26/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.26/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-17 01:45:56.104727 bytetrade-recommend-model-sdk-0.0.26/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.26/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/bytetrade_recommend_model_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-17 01:45:56.000000 bytetrade-recommend-model-sdk-0.0.26/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2178 2023-07-17 01:45:56.000000 bytetrade-recommend-model-sdk-0.0.26/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-17 01:45:56.000000 bytetrade-recommend-model-sdk-0.0.26/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-07-17 01:45:56.000000 bytetrade-recommend-model-sdk-0.0.26/bytetrade_recommend_model_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-17 01:45:56.000000 bytetrade-recommend-model-sdk-0.0.26/bytetrade_recommend_model_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/embeddings/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/embeddings/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3875 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/embeddings/bert_embedding.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/embeddings/embedding_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/embeddings/word2vec_embedding.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/config/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/config/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/config/content_similar_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      396 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/config/dnn_click_predictor_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/config/mind_base_config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4244 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2719 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/eval/__init_.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/eval/eval_operation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11667 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/exp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/exp/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11826 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/experiment_enum.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14888 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/model/content_similar_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2330 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.100727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/proto_class/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/proto_class/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19923 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/proto_class/embedding_pb2.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.104727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/recommend/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/recommend/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4976 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/recommend/recommend_common_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/recommend/recommend_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/recommend/time_weight_decay_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.104727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2508 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/resources/model_management.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 01:45:56.104727 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/tools/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/tools/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5147 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/tools/aws_s3_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10416 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/tools/common_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33591 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/tools/model_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-17 01:45:56.104727 bytetrade-recommend-model-sdk-0.0.26/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.26/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.691041 bytetrade-recommend-model-sdk-0.0.27/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.27/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-22 02:13:46.691041 bytetrade-recommend-model-sdk-0.0.27/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.27/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.683041 bytetrade-recommend-model-sdk-0.0.27/bytetrade_recommend_model_sdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-22 02:13:46.000000 bytetrade-recommend-model-sdk-0.0.27/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2178 2023-07-22 02:13:46.000000 bytetrade-recommend-model-sdk-0.0.27/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-22 02:13:46.000000 bytetrade-recommend-model-sdk-0.0.27/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-07-22 02:13:46.000000 bytetrade-recommend-model-sdk-0.0.27/bytetrade_recommend_model_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-22 02:13:46.000000 bytetrade-recommend-model-sdk-0.0.27/bytetrade_recommend_model_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.683041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/embeddings/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/embeddings/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3875 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/embeddings/bert_embedding.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/embeddings/embedding_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/embeddings/word2vec_embedding.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/config/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/config/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/config/content_similar_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      396 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/config/dnn_click_predictor_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/config/mind_base_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4244 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2719 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/eval/__init_.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/eval/eval_operation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11667 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/exp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/exp/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11826 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/experiment_enum.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14888 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/model/content_similar_model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2330 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/proto_class/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/proto_class/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23340 2023-07-21 09:10:35.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/proto_class/embedding_pb2.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/recommend/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/recommend/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4976 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/recommend/recommend_common_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/recommend/recommend_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/recommend/time_weight_decay_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.687041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2508 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/resources/model_management.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 02:13:46.691041 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/tools/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/tools/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5148 2023-07-21 12:55:09.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/tools/aws_s3_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10416 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/tools/common_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36818 2023-07-21 12:58:15.000000 bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/tools/model_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-22 02:13:46.691041 bytetrade-recommend-model-sdk-0.0.27/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-07-22 01:51:32.000000 bytetrade-recommend-model-sdk-0.0.27/setup.py
```

### Comparing `bytetrade-recommend-model-sdk-0.0.26/README.md` & `bytetrade-recommend-model-sdk-0.0.27/README.md`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt` & `bytetrade-recommend-model-sdk-0.0.27/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/embeddings/bert_embedding.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/embeddings/bert_embedding.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/embeddings/embedding_tool.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/embeddings/embedding_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/embeddings/word2vec_embedding.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/embeddings/word2vec_embedding.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/config/content_similar_config.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/config/content_similar_config.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/eval/eval_operation.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/eval/eval_operation.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/model/content_similar_model.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/model/content_similar_model.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/proto_class/embedding_pb2.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/proto_class/embedding_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='embedding.proto',
   package='',
   syntax='proto3',
   serialized_options=None,
-  serialized_pb=_b('\n\x0f\x65mbedding.proto\"\xb5\x01\n\x07\x41rticle\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tfull_text\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\x12\x12\x14\n\x0cpublished_at\x18\x04 \x01(\x12\x12\r\n\x05title\x18\x05 \x01(\t\x12\x0e\n\x06\x61uthor\x18\x06 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x07 \x01(\t\x12\x0f\n\x07\x66\x65\x65\x64_id\x18\x08 \x01(\x04\x12\x0c\n\x04hash\x18\t \x01(\t\x12\x11\n\timage_url\x18\n \x01(\t\"\x83\x01\n\tEmbedding\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x15\n\rmodel_version\x18\x03 \x01(\t\x12\x12\n\nembeddings\x18\x04 \x03(\x02\x12*\n\x10subdocembeddings\x18\x05 \x03(\x0b\x32\x10.SubdocEmbedding\";\n\x0fSubdocEmbedding\x12\x14\n\x0csubdoc_index\x18\x01 \x01(\r\x12\x12\n\nembeddings\x18\x02 \x03(\x02\"K\n\rLatestPackage\x12\x1a\n\x08\x61rticles\x18\x01 \x03(\x0b\x32\x08.Article\x12\x1e\n\nembeddings\x18\x02 \x03(\x0b\x32\n.Embedding\",\n\x0e\x41rticlePackage\x12\x1a\n\x08\x61rticles\x18\x01 \x03(\x0b\x32\x08.Article\"2\n\x10\x45mbeddingPakcage\x12\x1e\n\nembeddings\x18\x01 \x03(\x0b\x32\n.Embedding\"\xc1\x01\n\x04\x46\x65\x65\x64\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x10\n\x08\x66\x65\x65\x64_url\x18\x02 \x01(\t\x12\x10\n\x08site_url\x18\x03 \x01(\t\x12\r\n\x05title\x18\x04 \x01(\t\x12\x13\n\x0b\x63\x61tegory_id\x18\x05 \x01(\x03\x12\x16\n\x0e\x63\x61tegory_title\x18\x06 \x01(\t\x12\x0f\n\x07icon_id\x18\x07 \x01(\x03\x12\x11\n\ticon_type\x18\x08 \x01(\t\x12\x14\n\x0cicon_content\x18\t \x01(\x0c\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\"#\n\x0b\x46\x65\x65\x64Package\x12\x14\n\x05\x66\x65\x65\x64s\x18\x01 \x03(\x0b\x32\x05.Feedb\x06proto3')
+  serialized_pb=_b('\n\x0f\x65mbedding.proto\"\xb5\x01\n\x07\x41rticle\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tfull_text\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\x12\x12\x14\n\x0cpublished_at\x18\x04 \x01(\x12\x12\r\n\x05title\x18\x05 \x01(\t\x12\x0e\n\x06\x61uthor\x18\x06 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x07 \x01(\t\x12\x0f\n\x07\x66\x65\x65\x64_id\x18\x08 \x01(\x04\x12\x0c\n\x04hash\x18\t \x01(\t\x12\x11\n\timage_url\x18\n \x01(\t\"\x83\x01\n\tEmbedding\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x15\n\rmodel_version\x18\x03 \x01(\t\x12\x12\n\nembeddings\x18\x04 \x03(\x02\x12*\n\x10subdocembeddings\x18\x05 \x03(\x0b\x32\x10.SubdocEmbedding\";\n\x0fSubdocEmbedding\x12\x14\n\x0csubdoc_index\x18\x01 \x01(\r\x12\x12\n\nembeddings\x18\x02 \x03(\x02\"K\n\rLatestPackage\x12\x1a\n\x08\x61rticles\x18\x01 \x03(\x0b\x32\x08.Article\x12\x1e\n\nembeddings\x18\x02 \x03(\x0b\x32\n.Embedding\",\n\x0e\x41rticlePackage\x12\x1a\n\x08\x61rticles\x18\x01 \x03(\x0b\x32\x08.Article\"2\n\x10\x45mbeddingPakcage\x12\x1e\n\nembeddings\x18\x01 \x03(\x0b\x32\n.Embedding\"\xc1\x01\n\x04\x46\x65\x65\x64\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x10\n\x08\x66\x65\x65\x64_url\x18\x02 \x01(\t\x12\x10\n\x08site_url\x18\x03 \x01(\t\x12\r\n\x05title\x18\x04 \x01(\t\x12\x13\n\x0b\x63\x61tegory_id\x18\x05 \x01(\x03\x12\x16\n\x0e\x63\x61tegory_title\x18\x06 \x01(\t\x12\x0f\n\x07icon_id\x18\x07 \x01(\x03\x12\x11\n\ticon_type\x18\x08 \x01(\t\x12\x14\n\x0cicon_content\x18\t \x01(\x0c\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\"#\n\x0b\x46\x65\x65\x64Package\x12\x14\n\x05\x66\x65\x65\x64s\x18\x01 \x03(\x0b\x32\x05.Feed\"A\n\x11KeywordSortedInfo\x12\x0c\n\x04urls\x18\x01 \x03(\t\x12\r\n\x05\x66\x65\x65\x64s\x18\x02 \x03(\x03\x12\x0f\n\x07keyword\x18\x03 \x01(\t\"M\n\x18KeywordSortedInfoPackage\x12\x31\n\x15keyword_sortinfo_list\x18\x01 \x03(\x0b\x32\x12.KeywordSortedInfob\x06proto3')
 )
 
 
 
 
 _ARTICLE = _descriptor.Descriptor(
   name='Article',
@@ -436,28 +436,107 @@
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=769,
   serialized_end=804,
 )
 
+
+_KEYWORDSORTEDINFO = _descriptor.Descriptor(
+  name='KeywordSortedInfo',
+  full_name='KeywordSortedInfo',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='urls', full_name='KeywordSortedInfo.urls', index=0,
+      number=1, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='feeds', full_name='KeywordSortedInfo.feeds', index=1,
+      number=2, type=3, cpp_type=2, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='keyword', full_name='KeywordSortedInfo.keyword', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=806,
+  serialized_end=871,
+)
+
+
+_KEYWORDSORTEDINFOPACKAGE = _descriptor.Descriptor(
+  name='KeywordSortedInfoPackage',
+  full_name='KeywordSortedInfoPackage',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='keyword_sortinfo_list', full_name='KeywordSortedInfoPackage.keyword_sortinfo_list', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=873,
+  serialized_end=950,
+)
+
 _EMBEDDING.fields_by_name['subdocembeddings'].message_type = _SUBDOCEMBEDDING
 _LATESTPACKAGE.fields_by_name['articles'].message_type = _ARTICLE
 _LATESTPACKAGE.fields_by_name['embeddings'].message_type = _EMBEDDING
 _ARTICLEPACKAGE.fields_by_name['articles'].message_type = _ARTICLE
 _EMBEDDINGPAKCAGE.fields_by_name['embeddings'].message_type = _EMBEDDING
 _FEEDPACKAGE.fields_by_name['feeds'].message_type = _FEED
+_KEYWORDSORTEDINFOPACKAGE.fields_by_name['keyword_sortinfo_list'].message_type = _KEYWORDSORTEDINFO
 DESCRIPTOR.message_types_by_name['Article'] = _ARTICLE
 DESCRIPTOR.message_types_by_name['Embedding'] = _EMBEDDING
 DESCRIPTOR.message_types_by_name['SubdocEmbedding'] = _SUBDOCEMBEDDING
 DESCRIPTOR.message_types_by_name['LatestPackage'] = _LATESTPACKAGE
 DESCRIPTOR.message_types_by_name['ArticlePackage'] = _ARTICLEPACKAGE
 DESCRIPTOR.message_types_by_name['EmbeddingPakcage'] = _EMBEDDINGPAKCAGE
 DESCRIPTOR.message_types_by_name['Feed'] = _FEED
 DESCRIPTOR.message_types_by_name['FeedPackage'] = _FEEDPACKAGE
+DESCRIPTOR.message_types_by_name['KeywordSortedInfo'] = _KEYWORDSORTEDINFO
+DESCRIPTOR.message_types_by_name['KeywordSortedInfoPackage'] = _KEYWORDSORTEDINFOPACKAGE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 Article = _reflection.GeneratedProtocolMessageType('Article', (_message.Message,), dict(
   DESCRIPTOR = _ARTICLE,
   __module__ = 'embedding_pb2'
   # @@protoc_insertion_point(class_scope:Article)
   ))
@@ -508,9 +587,23 @@
 FeedPackage = _reflection.GeneratedProtocolMessageType('FeedPackage', (_message.Message,), dict(
   DESCRIPTOR = _FEEDPACKAGE,
   __module__ = 'embedding_pb2'
   # @@protoc_insertion_point(class_scope:FeedPackage)
   ))
 _sym_db.RegisterMessage(FeedPackage)
 
+KeywordSortedInfo = _reflection.GeneratedProtocolMessageType('KeywordSortedInfo', (_message.Message,), dict(
+  DESCRIPTOR = _KEYWORDSORTEDINFO,
+  __module__ = 'embedding_pb2'
+  # @@protoc_insertion_point(class_scope:KeywordSortedInfo)
+  ))
+_sym_db.RegisterMessage(KeywordSortedInfo)
+
+KeywordSortedInfoPackage = _reflection.GeneratedProtocolMessageType('KeywordSortedInfoPackage', (_message.Message,), dict(
+  DESCRIPTOR = _KEYWORDSORTEDINFOPACKAGE,
+  __module__ = 'embedding_pb2'
+  # @@protoc_insertion_point(class_scope:KeywordSortedInfoPackage)
+  ))
+_sym_db.RegisterMessage(KeywordSortedInfoPackage)
+
 
 # @@protoc_insertion_point(module_scope)
```

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/recommend/recommend_common_util.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/recommend/recommend_common_util.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/recommend/recommend_tool.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/recommend/recommend_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/recommend/time_weight_decay_tool.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/recommend/time_weight_decay_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/resources/model_management.json` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/resources/model_management.json`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/tools/aws_s3_tool.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/tools/aws_s3_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from recommend_model_sdk.tools.common_tool import CommonTool
 
 class AWSS3Tool:
     def __init__(self) -> None:
         self.__client = boto3.client('s3')
         self.__common_tool = CommonTool()
         self.__logger = self.__common_tool.get_logger()
+
     
     def upload_file(self,local_path,bucket_name,key):
         response = self.__client.upload_file(local_path,bucket_name,key)
         return response
     
     def get_file_size(self,s3_bucket, s3_object_key):
         meta_data = self.__client.head_object(Bucket=s3_bucket, Key=s3_object_key)
```

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/tools/common_tool.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/tools/common_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.26/recommend_model_sdk/tools/model_tool.py` & `bytetrade-recommend-model-sdk-0.0.27/recommend_model_sdk/tools/model_tool.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,14 +26,18 @@
         self.__model_dict = self.__validate_model_management_file(self.__model_management_file)
         self.__awss3tool = AWSS3Tool()
         self.__model_name_to_infer_method = dict()
         self.__model_name_to_infer_method["word2vec_google"] = self.word2vec_calculate_embedding
         self.__model_name_to_infer_method["bert"] = self.bert_calculate_embedding
         self.__model_root_dir = model_root_dir
         self.__latest_support_package_number = set([1000,5000,10000])
+        self.__keyword_sortinfo_package_recent_article_number = 1000
+        self.__keyword_sortinfo_package_top_k = 100
+        self.__default_bucket = "gpu-model-data"
+
 
     
     def get_valid_model_and_version(self):
         model_name_to_valid_version_list = dict()
         for current_model_name, current_model_version_dict in self.__model_dict.items():
             for current_version_name,current_model_detail in current_model_version_dict.items():
                 if current_model_detail["active"]:
@@ -300,15 +304,15 @@
             for current_field in feed_field_set:
                 if current_field not in current_feed:
                     current_feed[current_field] = None
             all_feed_id_to_feed[current_feed['id']] = current_feed
                 
         return all_feed_id_to_feed
         
-    
+
     def download_latest_article_embedding_package(self,model_name,model_version,latest_number,publish_time=None):
         """_summary_
 
         Args:
             model_name (_type_): _description_
             model_version (_type_): _description_
             latest_number (_type_): _description_
@@ -424,22 +428,15 @@
             for current_url,current_article in url_to_article_dict.items():
 
                 if current_article['published_at'] > start_time_timestamp:
                     filter_url_to_article_dict[current_url] = current_article
                     filter_url_to_embedding_dict[current_url] = url_to_embedding_dict[current_url]
             return filter_url_to_article_dict,filter_url_to_embedding_dict
         else:
-            return url_to_article_dict,url_to_embedding_dict
-        
-            
-            
-            
-                
-        
-        
+            return url_to_article_dict,url_to_embedding_dict  
     
     def init_model(self,model_name,model_version):
         nltk.download('stopwords')
         return self.download(model_name,model_version,self.__model_root_dir)
         
     def download(self,model_name,model_version,directory):
         if isinstance(directory,str) is False:
@@ -519,15 +516,15 @@
             if os.path.exists(last_formt_dst_file) is False:
                 return False
         return True
                 
                 
     def download_increment_package(self,model_name,model_version,package_key,publish_time=None):
         """_summary_
-
+        download increment embedding package
         Args:
             model_name (_type_): _description_
             model_version (_type_): _description_
             latest_number (_type_): _description_
             start_time (_type_, optional): _description_. Defaults to None.
 
         Raises:
@@ -639,10 +636,57 @@
                 if current_article['published_at'] > start_time_timestamp:
                     filter_url_to_article_dict[current_url] = current_article
                     filter_url_to_embedding_dict[current_url] = url_to_embedding_dict[current_url]
             return filter_url_to_article_dict,filter_url_to_embedding_dict
         else:
             return url_to_article_dict,url_to_embedding_dict
         
-            
-            
-              
+    def get_keyword_sortinfo_package_name(self):
+        package_name = f'keyword_sortinfo_package_recent_article_{self.__keyword_sortinfo_package_recent_article_number}_tok_k_{self.__keyword_sortinfo_package_top_k}'
+        return package_name 
+    
+    def download_keyword_sortinfo_package(self):
+        """_summary_
+        """
+        package_key = self.get_keyword_sortinfo_package_name()
+        # article_field_set = set(['url', 'full_text', 'created_at', 'published_at', 'title', 'author', 'content', 'feed_id', 'hash','image_url'])
+    
+        keyword_sortinfo_package_dir = os.path.join(self.__model_root_dir, 'sortinfo_package')
+        if os.path.exists(keyword_sortinfo_package_dir) is False or os.path.isdir(keyword_sortinfo_package_dir) is False:
+            os.makedirs(keyword_sortinfo_package_dir)
+        current_sortinfo_package_path = os.path.join(keyword_sortinfo_package_dir,package_key)
+                        
+        current_bucket_name = self.__default_bucket
+        
+        need_redownload = False
+        if os.path.exists(current_sortinfo_package_path) is False:
+            self.__logger.debug(f'current_sortinfo_package_path {current_sortinfo_package_path}  not exist')
+            need_redownload = True
+        else:
+            exist_protobuf_compress_hash = self.__common_tool.calculate_md5_for_big_file(current_sortinfo_package_path)
+            self.__logger.debug(f'current_embedding_path {current_sortinfo_package_path} does  exist ,exist file hash {exist_protobuf_compress_hash}')
+            response_header = self.__awss3tool.get_object_header(current_bucket_name, package_key)
+            if ("ResponseMetadata" not in response_header or 
+                "HTTPStatusCode" not in response_header["ResponseMetadata"] or
+                response_header["ResponseMetadata"]["HTTPStatusCode"] != 200):
+                raise ValueError(f'current_bucket { current_bucket_name} key {package_key} not exist')
+            if response_header["Metadata"]["md5_digest"] != exist_protobuf_compress_hash:
+                need_redownload = True
+                
+        if need_redownload:
+            result = self.__awss3tool.get_object_byte(current_bucket_name,package_key)
+            if result["success"] is False:
+                raise ValueError(f"download embedding package fail result {result}")
+            current_package_compress_byte = result["bytes"]
+            with open(current_sortinfo_package_path,'wb') as f:
+                f.write(current_package_compress_byte)
+            self.__logger.debug(f'need_download {current_sortinfo_package_path}')
+        else:
+            with open(current_sortinfo_package_path,'rb') as f:
+                current_package_compress_byte = f.read()
+        
+        decompress_bytes = zlib.decompress(current_package_compress_byte)
+        current_latest_package = rec_proto_embebding.KeywordSortedInfoPackage()
+        current_latest_package.ParseFromString(decompress_bytes)
+        
+        keyword_sortinfo_dict = MessageToDict(current_latest_package,preserving_proto_field_name=True)
+        return keyword_sortinfo_dict["keyword_sortinfo_list"]
```

### Comparing `bytetrade-recommend-model-sdk-0.0.26/setup.py` & `bytetrade-recommend-model-sdk-0.0.27/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 sys.path.append(os.path.dirname(__file__) + "/recommend-model")
 
 
 
 
 setup(
     name="bytetrade-recommend-model-sdk",
-    version="0.0.26",
+    version="0.0.27",
     # packages=find_packages(exclude="unit_test"),
     install_requires=[
         "pandas==2.0.0",
         "gensim==4.3.1",
         "protobuf==3.20.1",
         "nltk==3.8.1",
         "boto3"
```

