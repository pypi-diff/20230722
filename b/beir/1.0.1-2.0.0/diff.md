# Comparing `tmp/beir-1.0.1.tar.gz` & `tmp/beir-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/beir-1.0.1.tar", last modified: Thu Jun 30 19:01:46 2022, max compression
+gzip compressed data, was "beir-2.0.0.tar", last modified: Fri Jul 21 22:54:01 2023, max compression
```

## Comparing `beir-1.0.1.tar` & `beir-2.0.0.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwx------   0 ukp       (1014) ukp       (1014)        0 2022-06-30 19:01:46.000000 beir-1.0.1/
--rw-------   0 ukp       (1014) ukp       (1014)    11343 2022-03-21 13:13:33.000000 beir-1.0.1/LICENSE
--rw-------   0 ukp       (1014) ukp       (1014)      531 2022-03-21 13:13:33.000000 beir-1.0.1/NOTICE.txt
--rw-------   0 ukp       (1014) ukp       (1014)    17146 2022-06-30 19:01:46.000000 beir-1.0.1/PKG-INFO
--rw-------   0 ukp       (1014) ukp       (1014)    16325 2022-06-30 18:48:50.000000 beir-1.0.1/README.md
-drwx------   0 ukp       (1014) ukp       (1014)        0 2022-06-30 19:01:46.000000 beir-1.0.1/beir/
--rw-------   0 ukp       (1014) ukp       (1014)       35 2021-10-22 19:39:23.000000 beir-1.0.1/beir/__init__.py
-drwx------   0 ukp       (1014) ukp       (1014)        0 2022-06-30 19:01:46.000000 beir-1.0.1/beir/datasets/
--rw-------   0 ukp       (1014) ukp       (1014)        0 2021-10-22 19:39:23.000000 beir-1.0.1/beir/datasets/__init__.py
--rw-------   0 ukp       (1014) ukp       (1014)     4961 2021-10-22 19:39:23.000000 beir-1.0.1/beir/datasets/data_loader.py
--rw-------   0 ukp       (1014) ukp       (1014)     5641 2022-06-30 18:48:50.000000 beir-1.0.1/beir/datasets/data_loader_hf.py
-drwx------   0 ukp       (1014) ukp       (1014)        0 2022-06-30 19:01:46.000000 beir-1.0.1/beir/generation/
--rw-------   0 ukp       (1014) ukp       (1014)       54 2022-03-21 13:13:33.000000 beir-1.0.1/beir/generation/__init__.py
--rw-------   0 ukp       (1014) ukp       (1014)     7748 2022-03-21 13:13:33.000000 beir-1.0.1/beir/generation/generate.py
-drwx------   0 ukp       (1014) ukp       (1014)        0 2022-06-30 19:01:46.000000 beir-1.0.1/beir/generation/models/
--rw-------   0 ukp       (1014) ukp       (1014)       58 2022-03-21 13:13:33.000000 beir-1.0.1/beir/generation/models/__init__.py
--rw-------   0 ukp       (1014) ukp       (1014)     7413 2021-10-22 19:39:23.000000 beir-1.0.1/beir/generation/models/auto_model.py
--rw-------   0 ukp       (1014) ukp       (1014)     3156 2022-03-21 13:13:33.000000 beir-1.0.1/beir/generation/models/tilde.py
--rw-------   0 ukp       (1014) ukp       (1014)      405 2021-10-22 19:39:23.000000 beir-1.0.1/beir/logging.py
-drwx------   0 ukp       (1014) ukp       (1014)        0 2022-06-30 19:01:46.000000 beir-1.0.1/beir/losses/
--rw-------   0 ukp       (1014) ukp       (1014)       72 2021-10-22 19:39:23.000000 beir-1.0.1/beir/losses/__init__.py
--rw-------   0 ukp       (1014) ukp       (1014)     4479 2021-10-22 19:39:23.000000 beir-1.0.1/beir/losses/bpr_loss.py
--rw-------   0 ukp       (1014) ukp       (1014)     1739 2021-10-22 19:39:23.000000 beir-1.0.1/beir/losses/margin_mse_loss.py
-drwx------   0 ukp       (1014) ukp       (1014)        0 2022-06-30 19:01:46.000000 beir-1.0.1/beir/reranking/
--rw-------   0 ukp       (1014) ukp       (1014)       26 2021-10-22 19:39:23.000000 beir-1.0.1/beir/reranking/__init__.py
-drwx------   0 ukp       (1014) ukp       (1014)        0 2022-06-30 19:01:46.000000 beir-1.0.1/beir/reranking/models/
--rw-------   0 ukp       (1014) ukp       (1014)       67 2022-06-30 18:48:50.000000 beir-1.0.1/beir/reranking/models/__init__.py
--rw-------   0 ukp       (1014) ukp       (1014)      525 2022-06-30 18:48:50.000000 beir-1.0.1/beir/reranking/models/cross_encoder.py
--rw-------   0 ukp       (1014) ukp       (1014)     7319 2022-06-30 18:48:50.000000 beir-1.0.1/beir/reranking/models/mono_t5.py
--rw-------   0 ukp       (1014) ukp       (1014)     1923 2021-10-22 19:39:23.000000 beir-1.0.1/beir/reranking/rerank.py
-drwx------   0 ukp       (1014) ukp       (1014)        0 2022-06-30 19:01:46.000000 beir-1.0.1/beir/retrieval/
--rw-------   0 ukp       (1014) ukp       (1014)        0 2021-10-22 19:39:23.000000 beir-1.0.1/beir/retrieval/__init__.py
--rw-------   0 ukp       (1014) ukp       (1014)     4129 2022-03-21 13:13:33.000000 beir-1.0.1/beir/retrieval/custom_metrics.py
--rw-------   0 ukp       (1014) ukp       (1014)     4974 2022-06-30 18:53:57.000000 beir-1.0.1/beir/retrieval/evaluation.py
-drwx------   0 ukp       (1014) ukp       (1014)        0 2022-06-30 19:01:46.000000 beir-1.0.1/beir/retrieval/models/
--rw-------   0 ukp       (1014) ukp       (1014)      229 2022-03-21 13:13:33.000000 beir-1.0.1/beir/retrieval/models/__init__.py
--rw-------   0 ukp       (1014) ukp       (1014)     1613 2021-10-22 19:39:23.000000 beir-1.0.1/beir/retrieval/models/bpr.py
--rw-------   0 ukp       (1014) ukp       (1014)     2244 2021-10-22 19:39:23.000000 beir-1.0.1/beir/retrieval/models/dpr.py
--rw-------   0 ukp       (1014) ukp       (1014)     3296 2022-06-30 18:48:50.000000 beir-1.0.1/beir/retrieval/models/sentence_bert.py
--rw-------   0 ukp       (1014) ukp       (1014)     3571 2021-10-22 19:39:23.000000 beir-1.0.1/beir/retrieval/models/sparta.py
--rw-------   0 ukp       (1014) ukp       (1014)     7672 2022-03-21 13:13:33.000000 beir-1.0.1/beir/retrieval/models/splade.py
--rw-------   0 ukp       (1014) ukp       (1014)     2740 2022-03-21 13:13:33.000000 beir-1.0.1/beir/retrieval/models/tldr.py
--rw-------   0 ukp       (1014) ukp       (1014)     7900 2022-03-21 13:13:33.000000 beir-1.0.1/beir/retrieval/models/unicoil.py
--rw-------   0 ukp       (1014) ukp       (1014)     2113 2022-03-21 13:13:33.000000 beir-1.0.1/beir/retrieval/models/use_qa.py
-drwx------   0 ukp       (1014) ukp       (1014)        0 2022-06-30 19:01:46.000000 beir-1.0.1/beir/retrieval/search/
--rw-------   0 ukp       (1014) ukp       (1014)        0 2021-10-22 19:39:23.000000 beir-1.0.1/beir/retrieval/search/__init__.py
-drwx------   0 ukp       (1014) ukp       (1014)        0 2022-06-30 19:01:46.000000 beir-1.0.1/beir/retrieval/search/dense/
--rw-------   0 ukp       (1014) ukp       (1014)      294 2022-06-30 18:48:50.000000 beir-1.0.1/beir/retrieval/search/dense/__init__.py
--rw-------   0 ukp       (1014) ukp       (1014)     4011 2022-06-30 18:48:50.000000 beir-1.0.1/beir/retrieval/search/dense/exact_search.py
--rw-------   0 ukp       (1014) ukp       (1014)    10872 2022-06-30 18:48:50.000000 beir-1.0.1/beir/retrieval/search/dense/exact_search_multi_gpu.py
--rw-------   0 ukp       (1014) ukp       (1014)     7058 2021-10-22 19:39:23.000000 beir-1.0.1/beir/retrieval/search/dense/faiss_index.py
--rw-------   0 ukp       (1014) ukp       (1014)    18800 2022-06-30 18:48:50.000000 beir-1.0.1/beir/retrieval/search/dense/faiss_search.py
--rw-------   0 ukp       (1014) ukp       (1014)     1890 2022-06-30 18:48:50.000000 beir-1.0.1/beir/retrieval/search/dense/util.py
-drwx------   0 ukp       (1014) ukp       (1014)        0 2022-06-30 19:01:46.000000 beir-1.0.1/beir/retrieval/search/lexical/
--rw-------   0 ukp       (1014) ukp       (1014)       35 2021-10-22 19:39:23.000000 beir-1.0.1/beir/retrieval/search/lexical/__init__.py
--rw-------   0 ukp       (1014) ukp       (1014)     3196 2022-06-30 18:48:50.000000 beir-1.0.1/beir/retrieval/search/lexical/bm25_search.py
--rw-------   0 ukp       (1014) ukp       (1014)     9859 2022-03-21 13:13:33.000000 beir-1.0.1/beir/retrieval/search/lexical/elastic_search.py
-drwx------   0 ukp       (1014) ukp       (1014)        0 2022-06-30 19:01:46.000000 beir-1.0.1/beir/retrieval/search/sparse/
--rw-------   0 ukp       (1014) ukp       (1014)       39 2021-10-22 19:39:23.000000 beir-1.0.1/beir/retrieval/search/sparse/__init__.py
--rw-------   0 ukp       (1014) ukp       (1014)     1759 2022-03-21 13:13:33.000000 beir-1.0.1/beir/retrieval/search/sparse/sparse_search.py
--rw-------   0 ukp       (1014) ukp       (1014)     6676 2021-10-22 19:39:23.000000 beir-1.0.1/beir/retrieval/train.py
--rw-------   0 ukp       (1014) ukp       (1014)     3808 2022-03-21 13:13:33.000000 beir-1.0.1/beir/util.py
-drwx------   0 ukp       (1014) ukp       (1014)        0 2022-06-30 19:01:46.000000 beir-1.0.1/beir.egg-info/
--rw-------   0 ukp       (1014) ukp       (1014)    17146 2022-06-30 19:01:46.000000 beir-1.0.1/beir.egg-info/PKG-INFO
--rw-------   0 ukp       (1014) ukp       (1014)     1636 2022-06-30 19:01:46.000000 beir-1.0.1/beir.egg-info/SOURCES.txt
--rw-------   0 ukp       (1014) ukp       (1014)        1 2022-06-30 19:01:46.000000 beir-1.0.1/beir.egg-info/dependency_links.txt
--rw-------   0 ukp       (1014) ukp       (1014)      129 2022-06-30 19:01:46.000000 beir-1.0.1/beir.egg-info/requires.txt
--rw-------   0 ukp       (1014) ukp       (1014)        5 2022-06-30 19:01:46.000000 beir-1.0.1/beir.egg-info/top_level.txt
--rw-------   0 ukp       (1014) ukp       (1014)       79 2022-06-30 19:01:46.000000 beir-1.0.1/setup.cfg
--rw-------   0 ukp       (1014) ukp       (1014)     1304 2022-06-30 18:54:29.000000 beir-1.0.1/setup.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-07-21 22:54:01.764325 beir-2.0.0/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)    11348 2023-07-21 17:20:59.000000 beir-2.0.0/LICENSE
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      531 2022-04-09 23:18:07.000000 beir-2.0.0/NOTICE.txt
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)    18021 2023-07-21 22:54:01.764325 beir-2.0.0/PKG-INFO
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)    17200 2023-07-21 22:47:39.000000 beir-2.0.0/README.md
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-07-21 22:54:01.760325 beir-2.0.0/beir/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       35 2022-04-09 23:18:07.000000 beir-2.0.0/beir/__init__.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-07-21 22:54:01.760325 beir-2.0.0/beir/datasets/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)        0 2022-04-09 23:18:07.000000 beir-2.0.0/beir/datasets/__init__.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     4961 2022-04-09 23:18:07.000000 beir-2.0.0/beir/datasets/data_loader.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     5641 2023-07-21 17:20:59.000000 beir-2.0.0/beir/datasets/data_loader_hf.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-07-21 22:54:01.760325 beir-2.0.0/beir/generation/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       54 2022-04-09 23:18:07.000000 beir-2.0.0/beir/generation/__init__.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     7748 2022-04-09 23:18:07.000000 beir-2.0.0/beir/generation/generate.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-07-21 22:54:01.760325 beir-2.0.0/beir/generation/models/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       58 2022-04-09 23:18:07.000000 beir-2.0.0/beir/generation/models/__init__.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     7413 2022-04-09 23:18:07.000000 beir-2.0.0/beir/generation/models/auto_model.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3156 2022-04-09 23:18:07.000000 beir-2.0.0/beir/generation/models/tilde.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      405 2022-04-09 23:18:07.000000 beir-2.0.0/beir/logging.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-07-21 22:54:01.760325 beir-2.0.0/beir/losses/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       72 2022-04-09 23:18:07.000000 beir-2.0.0/beir/losses/__init__.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     4479 2022-04-09 23:18:07.000000 beir-2.0.0/beir/losses/bpr_loss.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1739 2022-04-09 23:18:07.000000 beir-2.0.0/beir/losses/margin_mse_loss.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-07-21 22:54:01.760325 beir-2.0.0/beir/reranking/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       26 2022-04-09 23:18:07.000000 beir-2.0.0/beir/reranking/__init__.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-07-21 22:54:01.760325 beir-2.0.0/beir/reranking/models/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       67 2023-07-21 17:20:59.000000 beir-2.0.0/beir/reranking/models/__init__.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      525 2023-07-21 17:20:59.000000 beir-2.0.0/beir/reranking/models/cross_encoder.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     7319 2023-07-21 17:20:59.000000 beir-2.0.0/beir/reranking/models/mono_t5.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1923 2022-04-09 23:18:07.000000 beir-2.0.0/beir/reranking/rerank.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-07-21 22:54:01.760325 beir-2.0.0/beir/retrieval/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)        0 2022-04-09 23:18:07.000000 beir-2.0.0/beir/retrieval/__init__.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     4129 2022-04-09 23:18:07.000000 beir-2.0.0/beir/retrieval/custom_metrics.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     4743 2023-07-21 18:30:00.000000 beir-2.0.0/beir/retrieval/evaluation.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-07-21 22:54:01.760325 beir-2.0.0/beir/retrieval/models/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      229 2022-04-09 23:18:07.000000 beir-2.0.0/beir/retrieval/models/__init__.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1613 2022-04-09 23:18:07.000000 beir-2.0.0/beir/retrieval/models/bpr.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     2244 2022-04-09 23:18:07.000000 beir-2.0.0/beir/retrieval/models/dpr.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3296 2023-07-21 17:20:59.000000 beir-2.0.0/beir/retrieval/models/sentence_bert.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3571 2022-04-09 23:18:07.000000 beir-2.0.0/beir/retrieval/models/sparta.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     7672 2022-04-09 23:18:07.000000 beir-2.0.0/beir/retrieval/models/splade.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     2740 2022-04-09 23:18:07.000000 beir-2.0.0/beir/retrieval/models/tldr.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     7900 2022-04-09 23:18:07.000000 beir-2.0.0/beir/retrieval/models/unicoil.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     2245 2023-07-21 22:47:39.000000 beir-2.0.0/beir/retrieval/models/use_qa.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-07-21 22:54:01.764325 beir-2.0.0/beir/retrieval/search/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       28 2023-07-21 18:11:51.000000 beir-2.0.0/beir/retrieval/search/__init__.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      316 2023-07-21 18:15:51.000000 beir-2.0.0/beir/retrieval/search/base.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-07-21 22:54:01.764325 beir-2.0.0/beir/retrieval/search/dense/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      294 2023-07-21 18:27:25.000000 beir-2.0.0/beir/retrieval/search/dense/__init__.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     4810 2023-07-21 22:24:42.000000 beir-2.0.0/beir/retrieval/search/dense/exact_search.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)    10703 2023-07-21 18:25:59.000000 beir-2.0.0/beir/retrieval/search/dense/exact_search_multi_gpu.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     7058 2023-07-20 20:39:55.000000 beir-2.0.0/beir/retrieval/search/dense/faiss_index.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)    22556 2023-07-21 18:24:48.000000 beir-2.0.0/beir/retrieval/search/dense/faiss_search.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1890 2023-07-21 17:20:59.000000 beir-2.0.0/beir/retrieval/search/dense/util.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-07-21 22:54:01.764325 beir-2.0.0/beir/retrieval/search/lexical/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       35 2023-07-21 18:26:28.000000 beir-2.0.0/beir/retrieval/search/lexical/__init__.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3234 2023-07-21 18:26:36.000000 beir-2.0.0/beir/retrieval/search/lexical/bm25_search.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     9859 2022-04-09 23:18:07.000000 beir-2.0.0/beir/retrieval/search/lexical/elastic_search.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-07-21 22:54:01.764325 beir-2.0.0/beir/retrieval/search/sparse/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       39 2023-07-21 18:27:50.000000 beir-2.0.0/beir/retrieval/search/sparse/__init__.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1777 2023-07-21 18:27:53.000000 beir-2.0.0/beir/retrieval/search/sparse/sparse_search.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     6625 2023-07-21 22:29:01.000000 beir-2.0.0/beir/retrieval/train.py
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     3808 2022-04-09 23:18:07.000000 beir-2.0.0/beir/util.py
+drwxrwxr-x   0 n3thakur  (1017) n3thakur  (1018)        0 2023-07-21 22:54:01.760325 beir-2.0.0/beir.egg-info/
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)    18021 2023-07-21 22:54:01.000000 beir-2.0.0/beir.egg-info/PKG-INFO
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1666 2023-07-21 22:54:01.000000 beir-2.0.0/beir.egg-info/SOURCES.txt
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)        1 2023-07-21 22:54:01.000000 beir-2.0.0/beir.egg-info/dependency_links.txt
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)      129 2023-07-21 22:54:01.000000 beir-2.0.0/beir.egg-info/requires.txt
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)        5 2023-07-21 22:54:01.000000 beir-2.0.0/beir.egg-info/top_level.txt
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)       79 2023-07-21 22:54:01.764325 beir-2.0.0/setup.cfg
+-rw-rw-r--   0 n3thakur  (1017) n3thakur  (1018)     1304 2023-07-21 22:52:29.000000 beir-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `beir-1.0.1/LICENSE` & `beir-2.0.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2020 Nandan Thakur
+   Copyright 2020-2023 Nandan Thakur
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `beir-1.0.1/NOTICE.txt` & `beir-2.0.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/PKG-INFO` & `beir-2.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: beir
-Version: 1.0.1
-Summary: A Heterogeneous Benchmark for Information Retrieval
-Home-page: https://github.com/beir-cellar/beir
-Download-URL: https://github.com/beir-cellar/beir/archive/v1.0.1.zip
-Author: Nandan Thakur
-Author-email: nandant@gmail.com
-License: Apache License 2.0
-Keywords: Information Retrieval Transformer Networks BERT PyTorch IR NLP deep learning
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: tf
-License-File: LICENSE
-License-File: NOTICE.txt
-
 <h1 align="center">
 <img style="vertical-align:middle" width="450" height="180" src="https://raw.githubusercontent.com/benchmarkir/beir/main/images/color_logo_transparent_cropped.png" />
 </h1>
 
 <p align="center">
     <a href="https://github.com/beir-cellar/beir/releases">
         <img alt="GitHub release" src="https://img.shields.io/github/release/beir-cellar/beir.svg">
@@ -70,19 +48,22 @@
 
 ## :beers: What is it?
 
 **BEIR** is a **heterogeneous benchmark** containing diverse IR tasks. It also provides a **common and easy framework** for evaluation of your NLP-based retrieval models within the benchmark.
 
 For **an overview**, checkout our **new wiki** page: [https://github.com/beir-cellar/beir/wiki](https://github.com/beir-cellar/beir/wiki).
 
-For **models and datasets**, checkout out **HuggingFace (HF)** page: [https://huggingface.co/BeIR](https://huggingface.co/BeIR).
+For **models and datasets**, checkout out **Hugging Face (HF)** page: [https://huggingface.co/BeIR](https://huggingface.co/BeIR).
+
+For **Leaderboard**, checkout out **Eval AI** page: [https://eval.ai/web/challenges/challenge-page/1897](https://eval.ai/web/challenges/challenge-page/1897).
 
 For more information, checkout out our publications:
 
 - [BEIR: A Heterogenous Benchmark for Zero-shot Evaluation of Information Retrieval Models](https://openreview.net/forum?id=wCu6T5xFjeJ) (NeurIPS 2021, Datasets and Benchmarks Track)
+- [Resources for Brewing BEIR: Reproducible Reference Models and an Official Leaderboard](https://arxiv.org/abs/2306.07471) (Arxiv 2023)
 
 ## :beers: Installation
 
 Install via pip:
 
 ```python
 pip install beir
@@ -144,23 +125,23 @@
 ndcg, _map, recall, precision = retriever.evaluate(qrels, results, retriever.k_values)
 ```
 
 ## :beers: Available Datasets
 
 Command to generate md5hash using Terminal:  ``md5sum filename.zip``.
 
-You can view all datasets available **[here](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/)** or on **[HuggingFace](https://huggingface.co/BeIR)**.
+You can view all datasets available **[here](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/)** or on **[Hugging Face](https://huggingface.co/BeIR)**.
 
 
 | Dataset   | Website| BEIR-Name | Public? | Type | Queries  | Corpus | Rel D/Q | Down-load | md5 |
 | -------- | -----| ---------| ------- | --------- | ----------- | ---------| ---------| :----------: | :------:|
 | MSMARCO    | [Homepage](https://microsoft.github.io/msmarco/)| ``msmarco`` | ✅ | ``train``<br>``dev``<br>``test``|  6,980   |  8.84M     |    1.1 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/msmarco.zip) | ``444067daf65d982533ea17ebd59501e4`` |
 | TREC-COVID |  [Homepage](https://ir.nist.gov/covidSubmit/index.html)| ``trec-covid``| ✅ | ``test``| 50|  171K| 493.5 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/trec-covid.zip) | ``ce62140cb23feb9becf6270d0d1fe6d1`` |
 | NFCorpus   | [Homepage](https://www.cl.uni-heidelberg.de/statnlpgroup/nfcorpus/) | ``nfcorpus`` | ✅ |``train``<br>``dev``<br>``test``|  323     |  3.6K     |  38.2 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/nfcorpus.zip) | ``a89dba18a62ef92f7d323ec890a0d38d`` |
-| BioASQ     | [Homepage](http://bioasq.org) | ``bioasq``| ❌ | ``train``<br>``test`` | 500 |  14.91M    |  8.05 | No | [How to Reproduce?](https://github.com/beir-cellar/beir/blob/main/examples/dataset#2-bioasq) |
+| BioASQ     | [Homepage](http://bioasq.org) | ``bioasq``| ❌ | ``train``<br>``test`` | 500 |  14.91M    |  4.7 | No | [How to Reproduce?](https://github.com/beir-cellar/beir/blob/main/examples/dataset#2-bioasq) |
 | NQ         | [Homepage](https://ai.google.com/research/NaturalQuestions) | ``nq``| ✅ | ``train``<br>``test``| 3,452   |  2.68M  |  1.2 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/nq.zip) | ``d4d3d2e48787a744b6f6e691ff534307`` |
 | HotpotQA   | [Homepage](https://hotpotqa.github.io) | ``hotpotqa``| ✅ |``train``<br>``dev``<br>``test``|  7,405   |  5.23M  |  2.0 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/hotpotqa.zip)  | ``f412724f78b0d91183a0e86805e16114`` |
 | FiQA-2018  | [Homepage](https://sites.google.com/view/fiqa/) | ``fiqa`` | ✅ | ``train``<br>``dev``<br>``test``|  648     |  57K    |  2.6 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/fiqa.zip)  | ``17918ed23cd04fb15047f73e6c3bd9d9`` |
 | Signal-1M(RT) | [Homepage](https://research.signal-ai.com/datasets/signal1m-tweetir.html)| ``signal1m`` | ❌ | ``test``| 97   |  2.86M  |  19.6 | No | [How to Reproduce?](https://github.com/beir-cellar/beir/blob/main/examples/dataset#4-signal-1m) |
 | TREC-NEWS  | [Homepage](https://trec.nist.gov/data/news2019.html) | ``trec-news`` | ❌ | ``test``| 57    |  595K    |  19.6 | No | [How to Reproduce?](https://github.com/beir-cellar/beir/blob/main/examples/dataset#1-trec-news) |
 | Robust04 | [Homepage](https://trec.nist.gov/data/robust/04.guidelines.html) | ``robust04``| ❌ | ``test``| 249  |  528K  |  69.9 |  No  |  [How to Reproduce?](https://github.com/beir-cellar/beir/blob/main/examples/dataset#3-robust04)  |
 | ArguAna    | [Homepage](http://argumentation.bplaced.net/arguana/data) | ``arguana``| ✅ |``test`` | 1,406     |  8.67K    |  1.0 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/arguana.zip)  | ``8ad3e3c2a5867cdced806d6503f29b99`` |
@@ -202,15 +183,15 @@
 ### Miscellaneous
 
 - [BEIR Leaderboard](https://github.com/beir-cellar/beir/wiki/Leaderboard)
 - [Couse Material on IR](https://github.com/beir-cellar/beir/wiki/Course-material-on-ir)
 
 ## :beers: Disclaimer
 
-Similar to Tensorflow [datasets](https://github.com/tensorflow/datasets) or HuggingFace's [datasets](https://github.com/huggingface/datasets) library, we just downloaded and prepared public datasets. We only distribute these datasets in a specific format, but we do not vouch for their quality or fairness, or claim that you have license to use the dataset. It remains the user's responsibility to determine whether you as a user have permission to use the dataset under the dataset's license and to cite the right owner of the dataset.
+Similar to Tensorflow [datasets](https://github.com/tensorflow/datasets) or Hugging Face's [datasets](https://github.com/huggingface/datasets) library, we just downloaded and prepared public datasets. We only distribute these datasets in a specific format, but we do not vouch for their quality or fairness, or claim that you have license to use the dataset. It remains the user's responsibility to determine whether you as a user have permission to use the dataset under the dataset's license and to cite the right owner of the dataset.
 
 If you're a dataset owner and wish to update any part of it, or do not want your dataset to be included in this library, feel free to post an issue here or make a pull request!
 
 If you're a dataset owner and wish to include your dataset or model in this library, feel free to post an issue here or make a pull request!
 
 ## :beers: Citing & Authors
 
@@ -223,29 +204,41 @@
     author={Nandan Thakur and Nils Reimers and Andreas R{\"u}ckl{\'e} and Abhishek Srivastava and Iryna Gurevych},
     booktitle={Thirty-fifth Conference on Neural Information Processing Systems Datasets and Benchmarks Track (Round 2)},
     year={2021},
     url={https://openreview.net/forum?id=wCu6T5xFjeJ}
 }
 ```
 
+If you use any baseline score from the BEIR leaderboard, feel free to cite our publication [Resources for Brewing BEIR: Reproducible Reference Models and an Official Leaderboard](https://arxiv.org/abs/2306.07471)
+```
+@misc{kamalloo2023resources,
+      title={Resources for Brewing BEIR: Reproducible Reference Models and an Official Leaderboard}, 
+      author={Ehsan Kamalloo and Nandan Thakur and Carlos Lassance and Xueguang Ma and Jheng-Hong Yang and Jimmy Lin},
+      year={2023},
+      eprint={2306.07471},
+      archivePrefix={arXiv},
+      primaryClass={cs.IR}
+}
+```
+
 The main contributors of this repository are:
 - [Nandan Thakur](https://github.com/Nthakur20), Personal Website: [nandan-thakur.com](https://nandan-thakur.com)
 
 Contact person: Nandan Thakur, [nandant@gmail.com](mailto:nandant@gmail.com)
 
 Don't hesitate to send us an e-mail or report an issue, if something is broken (and it shouldn't be) or if you have further questions.
 
 > This repository contains experimental software and is published for the sole purpose of giving additional background details on the respective publication.
 
 ## :beers: Collaboration
 
 The BEIR Benchmark has been made possible due to a collaborative effort of the following universities and organizations:
 - [UKP Lab, Technical University of Darmstadt](http://www.ukp.tu-darmstadt.de/)
 - [University of Waterloo](https://uwaterloo.ca/)
-- [HuggingFace](https://huggingface.co/)
+- [Hugging Face](https://huggingface.co/)
 
 ## :beers: Contributors
 
 Thanks go to all these wonderful collaborations for their contribution towards the BEIR benchmark:
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
@@ -260,9 +253,7 @@
     <td align="center"><a href="https://www.linkedin.com/in/abhesrivas"><img src="https://avatars.githubusercontent.com/u/19344566?v=4" width="100px;" alt=""/><br /><sub><b>Abhishek Srivastava</b></sub></a></td>
   </tr>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 <!-- ALL-CONTRIBUTORS-LIST:END -->
-
-
```

#### html2text {}

```diff
@@ -1,48 +1,41 @@
-Metadata-Version: 2.1 Name: beir Version: 1.0.1 Summary: A Heterogeneous
-Benchmark for Information Retrieval Home-page: https://github.com/beir-cellar/
-beir Download-URL: https://github.com/beir-cellar/beir/archive/v1.0.1.zip
-Author: Nandan Thakur Author-email: nandant@gmail.com License: Apache License
-2.0 Keywords: Information Retrieval Transformer Networks BERT PyTorch IR NLP
-deep learning Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Programming Language :: Python
-:: 3.6 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
-tf License-File: LICENSE License-File: NOTICE.txt
     ****** [https://raw.githubusercontent.com/benchmarkir/beir/main/images/
                   color_logo_transparent_cropped.png] ******
   [GitHub_release] [Build] [License] [Open_In_Colab] [Downloads] [Downloads]
  *** Paper | Installation | Quick_Example | Datasets | Wiki | Hugging_Face ***
  **** [./images/ukp.png] [./images/tu-darmstadt.png] [./images/uwaterloo.png]
                                      ****
                           **** [./images/HF.png] ****
 ## :beers: What is it? **BEIR** is a **heterogeneous benchmark** containing
 diverse IR tasks. It also provides a **common and easy framework** for
 evaluation of your NLP-based retrieval models within the benchmark. For **an
 overview**, checkout our **new wiki** page: [https://github.com/beir-cellar/
 beir/wiki](https://github.com/beir-cellar/beir/wiki). For **models and
-datasets**, checkout out **HuggingFace (HF)** page: [https://huggingface.co/
-BeIR](https://huggingface.co/BeIR). For more information, checkout out our
-publications: - [BEIR: A Heterogenous Benchmark for Zero-shot Evaluation of
+datasets**, checkout out **Hugging Face (HF)** page: [https://huggingface.co/
+BeIR](https://huggingface.co/BeIR). For **Leaderboard**, checkout out **Eval
+AI** page: [https://eval.ai/web/challenges/challenge-page/1897](https://
+eval.ai/web/challenges/challenge-page/1897). For more information, checkout out
+our publications: - [BEIR: A Heterogenous Benchmark for Zero-shot Evaluation of
 Information Retrieval Models](https://openreview.net/forum?id=wCu6T5xFjeJ)
-(NeurIPS 2021, Datasets and Benchmarks Track) ## :beers: Installation Install
-via pip: ```python pip install beir ``` If you want to build from source, use:
-```python $ git clone https://github.com/beir-cellar/beir.git $ cd beir $ pip
-install -e . ``` Tested with python versions 3.6 and 3.7 ## :beers: Features -
-Preprocess your own IR dataset or use one of the already-preprocessed 17
-benchmark datasets - Wide settings included, covers diverse benchmarks useful
-for both academia and industry - Includes well-known retrieval architectures
-(lexical, dense, sparse and reranking-based) - Add and evaluate your own model
-in a easy framework using different state-of-the-art evaluation metrics ## :
-beers: Quick Example For other example codes, please refer to our **[Examples
-and Tutorials](https://github.com/beir-cellar/beir/wiki/Examples-and-
-tutorials)** Wiki page. ```python from beir import util, LoggingHandler from
-beir.retrieval import models from beir.datasets.data_loader import
-GenericDataLoader from beir.retrieval.evaluation import EvaluateRetrieval from
+(NeurIPS 2021, Datasets and Benchmarks Track) - [Resources for Brewing BEIR:
+Reproducible Reference Models and an Official Leaderboard](https://arxiv.org/
+abs/2306.07471) (Arxiv 2023) ## :beers: Installation Install via pip: ```python
+pip install beir ``` If you want to build from source, use: ```python $ git
+clone https://github.com/beir-cellar/beir.git $ cd beir $ pip install -e . ```
+Tested with python versions 3.6 and 3.7 ## :beers: Features - Preprocess your
+own IR dataset or use one of the already-preprocessed 17 benchmark datasets -
+Wide settings included, covers diverse benchmarks useful for both academia and
+industry - Includes well-known retrieval architectures (lexical, dense, sparse
+and reranking-based) - Add and evaluate your own model in a easy framework
+using different state-of-the-art evaluation metrics ## :beers: Quick Example
+For other example codes, please refer to our **[Examples and Tutorials](https:/
+/github.com/beir-cellar/beir/wiki/Examples-and-tutorials)** Wiki page.
+```python from beir import util, LoggingHandler from beir.retrieval import
+models from beir.datasets.data_loader import GenericDataLoader from
+beir.retrieval.evaluation import EvaluateRetrieval from
 beir.retrieval.search.dense import DenseRetrievalExactSearch as DRES import
 logging import pathlib, os #### Just some code to print debug information to
 stdout logging.basicConfig(format='%(asctime)s - %(message)s', datefmt='%Y-%m-
 %d %H:%M:%S', level=logging.INFO, handlers=[LoggingHandler()]) #### /print
 debug information to stdout #### Download scifact.zip dataset and unzip the
 dataset dataset = "scifact" url = "https://public.ukp.informatik.tu-
 darmstadt.de/thakur/BEIR/datasets/{}.zip".format(dataset) out_dir =
@@ -54,35 +47,35 @@
 distilbert-base-tas-b"), batch_size=16) retriever = EvaluateRetrieval(model,
 score_function="dot") # or "cos_sim" for cosine similarity results =
 retriever.retrieve(corpus, queries) #### Evaluate your model with NDCG@k,
 MAP@K, Recall@K and Precision@K where k = [1,3,5,10,100,1000] ndcg, _map,
 recall, precision = retriever.evaluate(qrels, results, retriever.k_values) ```
 ## :beers: Available Datasets Command to generate md5hash using Terminal:
 ``md5sum filename.zip``. You can view all datasets available **[here](https://
-public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/)** or on **
-[HuggingFace](https://huggingface.co/BeIR)**. | Dataset | Website| BEIR-Name |
-Public? | Type | Queries | Corpus | Rel D/Q | Down-load | md5 | | -------- | --
----| ---------| ------- | --------- | ----------- | ---------| ---------| :----
-------: | :------:| | MSMARCO | [Homepage](https://microsoft.github.io/msmarco/
-)| ``msmarco`` | â | ``train``
+public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/)** or on **[Hugging
+Face](https://huggingface.co/BeIR)**. | Dataset | Website| BEIR-Name | Public?
+| Type | Queries | Corpus | Rel D/Q | Down-load | md5 | | -------- | -----| ---
+------| ------- | --------- | ----------- | ---------| ---------| :----------:
+| :------:| | MSMARCO | [Homepage](https://microsoft.github.io/msmarco/)|
+``msmarco`` | â | ``train``
 ``dev``
 ``test``| 6,980 | 8.84M | 1.1 | [Link](https://public.ukp.informatik.tu-
 darmstadt.de/thakur/BEIR/datasets/msmarco.zip) |
 ``444067daf65d982533ea17ebd59501e4`` | | TREC-COVID | [Homepage](https://
 ir.nist.gov/covidSubmit/index.html)| ``trec-covid``| â | ``test``| 50| 171K|
 493.5 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/
 datasets/trec-covid.zip) | ``ce62140cb23feb9becf6270d0d1fe6d1`` | | NFCorpus |
 [Homepage](https://www.cl.uni-heidelberg.de/statnlpgroup/nfcorpus/) |
 ``nfcorpus`` | â |``train``
 ``dev``
 ``test``| 323 | 3.6K | 38.2 | [Link](https://public.ukp.informatik.tu-
 darmstadt.de/thakur/BEIR/datasets/nfcorpus.zip) |
 ``a89dba18a62ef92f7d323ec890a0d38d`` | | BioASQ | [Homepage](http://bioasq.org)
 | ``bioasq``| â | ``train``
-``test`` | 500 | 14.91M | 8.05 | No | [How to Reproduce?](https://github.com/
+``test`` | 500 | 14.91M | 4.7 | No | [How to Reproduce?](https://github.com/
 beir-cellar/beir/blob/main/examples/dataset#2-bioasq) | | NQ | [Homepage]
 (https://ai.google.com/research/NaturalQuestions) | ``nq``| â | ``train``
 ``test``| 3,452 | 2.68M | 1.2 | [Link](https://public.ukp.informatik.tu-
 darmstadt.de/thakur/BEIR/datasets/nq.zip) |
 ``d4d3d2e48787a744b6f6e691ff534307`` | | HotpotQA | [Homepage](https://
 hotpotqa.github.io) | ``hotpotqa``| â |``train``
 ``dev``
@@ -149,15 +142,15 @@
 custom-dataset) ### Models - [Models Available](https://github.com/beir-cellar/
 beir/wiki/Models-available) - [Evaluate your Custom Model](https://github.com/
 beir-cellar/beir/wiki/Evaluate-your-custom-model) ### Metrics - [Metrics
 Available](https://github.com/beir-cellar/beir/wiki/Metrics-available) ###
 Miscellaneous - [BEIR Leaderboard](https://github.com/beir-cellar/beir/wiki/
 Leaderboard) - [Couse Material on IR](https://github.com/beir-cellar/beir/wiki/
 Course-material-on-ir) ## :beers: Disclaimer Similar to Tensorflow [datasets]
-(https://github.com/tensorflow/datasets) or HuggingFace's [datasets](https://
+(https://github.com/tensorflow/datasets) or Hugging Face's [datasets](https://
 github.com/huggingface/datasets) library, we just downloaded and prepared
 public datasets. We only distribute these datasets in a specific format, but we
 do not vouch for their quality or fairness, or claim that you have license to
 use the dataset. It remains the user's responsibility to determine whether you
 as a user have permission to use the dataset under the dataset's license and to
 cite the right owner of the dataset. If you're a dataset owner and wish to
 update any part of it, or do not want your dataset to be included in this
@@ -168,25 +161,32 @@
 Heterogenous Benchmark for Zero-shot Evaluation of Information Retrieval
 Models](https://arxiv.org/abs/2104.08663): ``` @inproceedings{ thakur2021beir,
 title={{BEIR}: A Heterogeneous Benchmark for Zero-shot Evaluation of
 Information Retrieval Models}, author={Nandan Thakur and Nils Reimers and
 Andreas R{\"u}ckl{\'e} and Abhishek Srivastava and Iryna Gurevych}, booktitle=
 {Thirty-fifth Conference on Neural Information Processing Systems Datasets and
 Benchmarks Track (Round 2)}, year={2021}, url={https://openreview.net/
-forum?id=wCu6T5xFjeJ} } ``` The main contributors of this repository are: -
+forum?id=wCu6T5xFjeJ} } ``` If you use any baseline score from the BEIR
+leaderboard, feel free to cite our publication [Resources for Brewing BEIR:
+Reproducible Reference Models and an Official Leaderboard](https://arxiv.org/
+abs/2306.07471) ``` @misc{kamalloo2023resources, title={Resources for Brewing
+BEIR: Reproducible Reference Models and an Official Leaderboard}, author={Ehsan
+Kamalloo and Nandan Thakur and Carlos Lassance and Xueguang Ma and Jheng-Hong
+Yang and Jimmy Lin}, year={2023}, eprint={2306.07471}, archivePrefix={arXiv},
+primaryClass={cs.IR} } ``` The main contributors of this repository are: -
 [Nandan Thakur](https://github.com/Nthakur20), Personal Website: [nandan-
 thakur.com](https://nandan-thakur.com) Contact person: Nandan Thakur,
 [nandant@gmail.com](mailto:nandant@gmail.com) Don't hesitate to send us an e-
 mail or report an issue, if something is broken (and it shouldn't be) or if you
 have further questions. > This repository contains experimental software and is
 published for the sole purpose of giving additional background details on the
 respective publication. ## :beers: Collaboration The BEIR Benchmark has been
 made possible due to a collaborative effort of the following universities and
 organizations: - [UKP Lab, Technical University of Darmstadt](http://
 www.ukp.tu-darmstadt.de/) - [University of Waterloo](https://uwaterloo.ca/) -
-[HuggingFace](https://huggingface.co/) ## :beers: Contributors Thanks go to all
-these wonderful collaborations for their contribution towards the BEIR
+[Hugging Face](https://huggingface.co/) ## :beers: Contributors Thanks go to
+all these wonderful collaborations for their contribution towards the BEIR
 benchmark:
 
 Nandan_Thakur Nils_Reimers  Iryna   Jimmy_Lin   Andreas_RÃ¼cklÃ� Abhishek
                            Gurevych                                Srivastava
```

### Comparing `beir-1.0.1/README.md` & `beir-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: beir
+Version: 2.0.0
+Summary: A Heterogeneous Benchmark for Information Retrieval
+Home-page: https://github.com/beir-cellar/beir
+Author: Nandan Thakur
+Author-email: nandant@gmail.com
+License: Apache License 2.0
+Download-URL: https://github.com/beir-cellar/beir/archive/v2.0.0.zip
+Keywords: Information Retrieval Transformer Networks BERT PyTorch IR NLP deep learning
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: tf
+License-File: LICENSE
+License-File: NOTICE.txt
+
 <h1 align="center">
 <img style="vertical-align:middle" width="450" height="180" src="https://raw.githubusercontent.com/benchmarkir/beir/main/images/color_logo_transparent_cropped.png" />
 </h1>
 
 <p align="center">
     <a href="https://github.com/beir-cellar/beir/releases">
         <img alt="GitHub release" src="https://img.shields.io/github/release/beir-cellar/beir.svg">
@@ -48,19 +70,22 @@
 
 ## :beers: What is it?
 
 **BEIR** is a **heterogeneous benchmark** containing diverse IR tasks. It also provides a **common and easy framework** for evaluation of your NLP-based retrieval models within the benchmark.
 
 For **an overview**, checkout our **new wiki** page: [https://github.com/beir-cellar/beir/wiki](https://github.com/beir-cellar/beir/wiki).
 
-For **models and datasets**, checkout out **HuggingFace (HF)** page: [https://huggingface.co/BeIR](https://huggingface.co/BeIR).
+For **models and datasets**, checkout out **Hugging Face (HF)** page: [https://huggingface.co/BeIR](https://huggingface.co/BeIR).
+
+For **Leaderboard**, checkout out **Eval AI** page: [https://eval.ai/web/challenges/challenge-page/1897](https://eval.ai/web/challenges/challenge-page/1897).
 
 For more information, checkout out our publications:
 
 - [BEIR: A Heterogenous Benchmark for Zero-shot Evaluation of Information Retrieval Models](https://openreview.net/forum?id=wCu6T5xFjeJ) (NeurIPS 2021, Datasets and Benchmarks Track)
+- [Resources for Brewing BEIR: Reproducible Reference Models and an Official Leaderboard](https://arxiv.org/abs/2306.07471) (Arxiv 2023)
 
 ## :beers: Installation
 
 Install via pip:
 
 ```python
 pip install beir
@@ -122,23 +147,23 @@
 ndcg, _map, recall, precision = retriever.evaluate(qrels, results, retriever.k_values)
 ```
 
 ## :beers: Available Datasets
 
 Command to generate md5hash using Terminal:  ``md5sum filename.zip``.
 
-You can view all datasets available **[here](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/)** or on **[HuggingFace](https://huggingface.co/BeIR)**.
+You can view all datasets available **[here](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/)** or on **[Hugging Face](https://huggingface.co/BeIR)**.
 
 
 | Dataset   | Website| BEIR-Name | Public? | Type | Queries  | Corpus | Rel D/Q | Down-load | md5 |
 | -------- | -----| ---------| ------- | --------- | ----------- | ---------| ---------| :----------: | :------:|
 | MSMARCO    | [Homepage](https://microsoft.github.io/msmarco/)| ``msmarco`` | ✅ | ``train``<br>``dev``<br>``test``|  6,980   |  8.84M     |    1.1 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/msmarco.zip) | ``444067daf65d982533ea17ebd59501e4`` |
 | TREC-COVID |  [Homepage](https://ir.nist.gov/covidSubmit/index.html)| ``trec-covid``| ✅ | ``test``| 50|  171K| 493.5 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/trec-covid.zip) | ``ce62140cb23feb9becf6270d0d1fe6d1`` |
 | NFCorpus   | [Homepage](https://www.cl.uni-heidelberg.de/statnlpgroup/nfcorpus/) | ``nfcorpus`` | ✅ |``train``<br>``dev``<br>``test``|  323     |  3.6K     |  38.2 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/nfcorpus.zip) | ``a89dba18a62ef92f7d323ec890a0d38d`` |
-| BioASQ     | [Homepage](http://bioasq.org) | ``bioasq``| ❌ | ``train``<br>``test`` | 500 |  14.91M    |  8.05 | No | [How to Reproduce?](https://github.com/beir-cellar/beir/blob/main/examples/dataset#2-bioasq) |
+| BioASQ     | [Homepage](http://bioasq.org) | ``bioasq``| ❌ | ``train``<br>``test`` | 500 |  14.91M    |  4.7 | No | [How to Reproduce?](https://github.com/beir-cellar/beir/blob/main/examples/dataset#2-bioasq) |
 | NQ         | [Homepage](https://ai.google.com/research/NaturalQuestions) | ``nq``| ✅ | ``train``<br>``test``| 3,452   |  2.68M  |  1.2 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/nq.zip) | ``d4d3d2e48787a744b6f6e691ff534307`` |
 | HotpotQA   | [Homepage](https://hotpotqa.github.io) | ``hotpotqa``| ✅ |``train``<br>``dev``<br>``test``|  7,405   |  5.23M  |  2.0 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/hotpotqa.zip)  | ``f412724f78b0d91183a0e86805e16114`` |
 | FiQA-2018  | [Homepage](https://sites.google.com/view/fiqa/) | ``fiqa`` | ✅ | ``train``<br>``dev``<br>``test``|  648     |  57K    |  2.6 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/fiqa.zip)  | ``17918ed23cd04fb15047f73e6c3bd9d9`` |
 | Signal-1M(RT) | [Homepage](https://research.signal-ai.com/datasets/signal1m-tweetir.html)| ``signal1m`` | ❌ | ``test``| 97   |  2.86M  |  19.6 | No | [How to Reproduce?](https://github.com/beir-cellar/beir/blob/main/examples/dataset#4-signal-1m) |
 | TREC-NEWS  | [Homepage](https://trec.nist.gov/data/news2019.html) | ``trec-news`` | ❌ | ``test``| 57    |  595K    |  19.6 | No | [How to Reproduce?](https://github.com/beir-cellar/beir/blob/main/examples/dataset#1-trec-news) |
 | Robust04 | [Homepage](https://trec.nist.gov/data/robust/04.guidelines.html) | ``robust04``| ❌ | ``test``| 249  |  528K  |  69.9 |  No  |  [How to Reproduce?](https://github.com/beir-cellar/beir/blob/main/examples/dataset#3-robust04)  |
 | ArguAna    | [Homepage](http://argumentation.bplaced.net/arguana/data) | ``arguana``| ✅ |``test`` | 1,406     |  8.67K    |  1.0 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/arguana.zip)  | ``8ad3e3c2a5867cdced806d6503f29b99`` |
@@ -180,15 +205,15 @@
 ### Miscellaneous
 
 - [BEIR Leaderboard](https://github.com/beir-cellar/beir/wiki/Leaderboard)
 - [Couse Material on IR](https://github.com/beir-cellar/beir/wiki/Course-material-on-ir)
 
 ## :beers: Disclaimer
 
-Similar to Tensorflow [datasets](https://github.com/tensorflow/datasets) or HuggingFace's [datasets](https://github.com/huggingface/datasets) library, we just downloaded and prepared public datasets. We only distribute these datasets in a specific format, but we do not vouch for their quality or fairness, or claim that you have license to use the dataset. It remains the user's responsibility to determine whether you as a user have permission to use the dataset under the dataset's license and to cite the right owner of the dataset.
+Similar to Tensorflow [datasets](https://github.com/tensorflow/datasets) or Hugging Face's [datasets](https://github.com/huggingface/datasets) library, we just downloaded and prepared public datasets. We only distribute these datasets in a specific format, but we do not vouch for their quality or fairness, or claim that you have license to use the dataset. It remains the user's responsibility to determine whether you as a user have permission to use the dataset under the dataset's license and to cite the right owner of the dataset.
 
 If you're a dataset owner and wish to update any part of it, or do not want your dataset to be included in this library, feel free to post an issue here or make a pull request!
 
 If you're a dataset owner and wish to include your dataset or model in this library, feel free to post an issue here or make a pull request!
 
 ## :beers: Citing & Authors
 
@@ -201,29 +226,41 @@
     author={Nandan Thakur and Nils Reimers and Andreas R{\"u}ckl{\'e} and Abhishek Srivastava and Iryna Gurevych},
     booktitle={Thirty-fifth Conference on Neural Information Processing Systems Datasets and Benchmarks Track (Round 2)},
     year={2021},
     url={https://openreview.net/forum?id=wCu6T5xFjeJ}
 }
 ```
 
+If you use any baseline score from the BEIR leaderboard, feel free to cite our publication [Resources for Brewing BEIR: Reproducible Reference Models and an Official Leaderboard](https://arxiv.org/abs/2306.07471)
+```
+@misc{kamalloo2023resources,
+      title={Resources for Brewing BEIR: Reproducible Reference Models and an Official Leaderboard}, 
+      author={Ehsan Kamalloo and Nandan Thakur and Carlos Lassance and Xueguang Ma and Jheng-Hong Yang and Jimmy Lin},
+      year={2023},
+      eprint={2306.07471},
+      archivePrefix={arXiv},
+      primaryClass={cs.IR}
+}
+```
+
 The main contributors of this repository are:
 - [Nandan Thakur](https://github.com/Nthakur20), Personal Website: [nandan-thakur.com](https://nandan-thakur.com)
 
 Contact person: Nandan Thakur, [nandant@gmail.com](mailto:nandant@gmail.com)
 
 Don't hesitate to send us an e-mail or report an issue, if something is broken (and it shouldn't be) or if you have further questions.
 
 > This repository contains experimental software and is published for the sole purpose of giving additional background details on the respective publication.
 
 ## :beers: Collaboration
 
 The BEIR Benchmark has been made possible due to a collaborative effort of the following universities and organizations:
 - [UKP Lab, Technical University of Darmstadt](http://www.ukp.tu-darmstadt.de/)
 - [University of Waterloo](https://uwaterloo.ca/)
-- [HuggingFace](https://huggingface.co/)
+- [Hugging Face](https://huggingface.co/)
 
 ## :beers: Contributors
 
 Thanks go to all these wonderful collaborations for their contribution towards the BEIR benchmark:
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
@@ -238,7 +275,9 @@
     <td align="center"><a href="https://www.linkedin.com/in/abhesrivas"><img src="https://avatars.githubusercontent.com/u/19344566?v=4" width="100px;" alt=""/><br /><sub><b>Abhishek Srivastava</b></sub></a></td>
   </tr>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 <!-- ALL-CONTRIBUTORS-LIST:END -->
+
+
```

#### html2text {}

```diff
@@ -1,37 +1,52 @@
+Metadata-Version: 2.1 Name: beir Version: 2.0.0 Summary: A Heterogeneous
+Benchmark for Information Retrieval Home-page: https://github.com/beir-cellar/
+beir Author: Nandan Thakur Author-email: nandant@gmail.com License: Apache
+License 2.0 Download-URL: https://github.com/beir-cellar/beir/archive/
+v2.0.0.zip Keywords: Information Retrieval Transformer Networks BERT PyTorch IR
+NLP deep learning Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Programming Language :: Python
+:: 3.6 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
+tf License-File: LICENSE License-File: NOTICE.txt
     ****** [https://raw.githubusercontent.com/benchmarkir/beir/main/images/
                   color_logo_transparent_cropped.png] ******
   [GitHub_release] [Build] [License] [Open_In_Colab] [Downloads] [Downloads]
  *** Paper | Installation | Quick_Example | Datasets | Wiki | Hugging_Face ***
  **** [./images/ukp.png] [./images/tu-darmstadt.png] [./images/uwaterloo.png]
                                      ****
                           **** [./images/HF.png] ****
 ## :beers: What is it? **BEIR** is a **heterogeneous benchmark** containing
 diverse IR tasks. It also provides a **common and easy framework** for
 evaluation of your NLP-based retrieval models within the benchmark. For **an
 overview**, checkout our **new wiki** page: [https://github.com/beir-cellar/
 beir/wiki](https://github.com/beir-cellar/beir/wiki). For **models and
-datasets**, checkout out **HuggingFace (HF)** page: [https://huggingface.co/
-BeIR](https://huggingface.co/BeIR). For more information, checkout out our
-publications: - [BEIR: A Heterogenous Benchmark for Zero-shot Evaluation of
+datasets**, checkout out **Hugging Face (HF)** page: [https://huggingface.co/
+BeIR](https://huggingface.co/BeIR). For **Leaderboard**, checkout out **Eval
+AI** page: [https://eval.ai/web/challenges/challenge-page/1897](https://
+eval.ai/web/challenges/challenge-page/1897). For more information, checkout out
+our publications: - [BEIR: A Heterogenous Benchmark for Zero-shot Evaluation of
 Information Retrieval Models](https://openreview.net/forum?id=wCu6T5xFjeJ)
-(NeurIPS 2021, Datasets and Benchmarks Track) ## :beers: Installation Install
-via pip: ```python pip install beir ``` If you want to build from source, use:
-```python $ git clone https://github.com/beir-cellar/beir.git $ cd beir $ pip
-install -e . ``` Tested with python versions 3.6 and 3.7 ## :beers: Features -
-Preprocess your own IR dataset or use one of the already-preprocessed 17
-benchmark datasets - Wide settings included, covers diverse benchmarks useful
-for both academia and industry - Includes well-known retrieval architectures
-(lexical, dense, sparse and reranking-based) - Add and evaluate your own model
-in a easy framework using different state-of-the-art evaluation metrics ## :
-beers: Quick Example For other example codes, please refer to our **[Examples
-and Tutorials](https://github.com/beir-cellar/beir/wiki/Examples-and-
-tutorials)** Wiki page. ```python from beir import util, LoggingHandler from
-beir.retrieval import models from beir.datasets.data_loader import
-GenericDataLoader from beir.retrieval.evaluation import EvaluateRetrieval from
+(NeurIPS 2021, Datasets and Benchmarks Track) - [Resources for Brewing BEIR:
+Reproducible Reference Models and an Official Leaderboard](https://arxiv.org/
+abs/2306.07471) (Arxiv 2023) ## :beers: Installation Install via pip: ```python
+pip install beir ``` If you want to build from source, use: ```python $ git
+clone https://github.com/beir-cellar/beir.git $ cd beir $ pip install -e . ```
+Tested with python versions 3.6 and 3.7 ## :beers: Features - Preprocess your
+own IR dataset or use one of the already-preprocessed 17 benchmark datasets -
+Wide settings included, covers diverse benchmarks useful for both academia and
+industry - Includes well-known retrieval architectures (lexical, dense, sparse
+and reranking-based) - Add and evaluate your own model in a easy framework
+using different state-of-the-art evaluation metrics ## :beers: Quick Example
+For other example codes, please refer to our **[Examples and Tutorials](https:/
+/github.com/beir-cellar/beir/wiki/Examples-and-tutorials)** Wiki page.
+```python from beir import util, LoggingHandler from beir.retrieval import
+models from beir.datasets.data_loader import GenericDataLoader from
+beir.retrieval.evaluation import EvaluateRetrieval from
 beir.retrieval.search.dense import DenseRetrievalExactSearch as DRES import
 logging import pathlib, os #### Just some code to print debug information to
 stdout logging.basicConfig(format='%(asctime)s - %(message)s', datefmt='%Y-%m-
 %d %H:%M:%S', level=logging.INFO, handlers=[LoggingHandler()]) #### /print
 debug information to stdout #### Download scifact.zip dataset and unzip the
 dataset dataset = "scifact" url = "https://public.ukp.informatik.tu-
 darmstadt.de/thakur/BEIR/datasets/{}.zip".format(dataset) out_dir =
@@ -43,35 +58,35 @@
 distilbert-base-tas-b"), batch_size=16) retriever = EvaluateRetrieval(model,
 score_function="dot") # or "cos_sim" for cosine similarity results =
 retriever.retrieve(corpus, queries) #### Evaluate your model with NDCG@k,
 MAP@K, Recall@K and Precision@K where k = [1,3,5,10,100,1000] ndcg, _map,
 recall, precision = retriever.evaluate(qrels, results, retriever.k_values) ```
 ## :beers: Available Datasets Command to generate md5hash using Terminal:
 ``md5sum filename.zip``. You can view all datasets available **[here](https://
-public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/)** or on **
-[HuggingFace](https://huggingface.co/BeIR)**. | Dataset | Website| BEIR-Name |
-Public? | Type | Queries | Corpus | Rel D/Q | Down-load | md5 | | -------- | --
----| ---------| ------- | --------- | ----------- | ---------| ---------| :----
-------: | :------:| | MSMARCO | [Homepage](https://microsoft.github.io/msmarco/
-)| ``msmarco`` | â | ``train``
+public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/)** or on **[Hugging
+Face](https://huggingface.co/BeIR)**. | Dataset | Website| BEIR-Name | Public?
+| Type | Queries | Corpus | Rel D/Q | Down-load | md5 | | -------- | -----| ---
+------| ------- | --------- | ----------- | ---------| ---------| :----------:
+| :------:| | MSMARCO | [Homepage](https://microsoft.github.io/msmarco/)|
+``msmarco`` | â | ``train``
 ``dev``
 ``test``| 6,980 | 8.84M | 1.1 | [Link](https://public.ukp.informatik.tu-
 darmstadt.de/thakur/BEIR/datasets/msmarco.zip) |
 ``444067daf65d982533ea17ebd59501e4`` | | TREC-COVID | [Homepage](https://
 ir.nist.gov/covidSubmit/index.html)| ``trec-covid``| â | ``test``| 50| 171K|
 493.5 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/
 datasets/trec-covid.zip) | ``ce62140cb23feb9becf6270d0d1fe6d1`` | | NFCorpus |
 [Homepage](https://www.cl.uni-heidelberg.de/statnlpgroup/nfcorpus/) |
 ``nfcorpus`` | â |``train``
 ``dev``
 ``test``| 323 | 3.6K | 38.2 | [Link](https://public.ukp.informatik.tu-
 darmstadt.de/thakur/BEIR/datasets/nfcorpus.zip) |
 ``a89dba18a62ef92f7d323ec890a0d38d`` | | BioASQ | [Homepage](http://bioasq.org)
 | ``bioasq``| â | ``train``
-``test`` | 500 | 14.91M | 8.05 | No | [How to Reproduce?](https://github.com/
+``test`` | 500 | 14.91M | 4.7 | No | [How to Reproduce?](https://github.com/
 beir-cellar/beir/blob/main/examples/dataset#2-bioasq) | | NQ | [Homepage]
 (https://ai.google.com/research/NaturalQuestions) | ``nq``| â | ``train``
 ``test``| 3,452 | 2.68M | 1.2 | [Link](https://public.ukp.informatik.tu-
 darmstadt.de/thakur/BEIR/datasets/nq.zip) |
 ``d4d3d2e48787a744b6f6e691ff534307`` | | HotpotQA | [Homepage](https://
 hotpotqa.github.io) | ``hotpotqa``| â |``train``
 ``dev``
@@ -138,15 +153,15 @@
 custom-dataset) ### Models - [Models Available](https://github.com/beir-cellar/
 beir/wiki/Models-available) - [Evaluate your Custom Model](https://github.com/
 beir-cellar/beir/wiki/Evaluate-your-custom-model) ### Metrics - [Metrics
 Available](https://github.com/beir-cellar/beir/wiki/Metrics-available) ###
 Miscellaneous - [BEIR Leaderboard](https://github.com/beir-cellar/beir/wiki/
 Leaderboard) - [Couse Material on IR](https://github.com/beir-cellar/beir/wiki/
 Course-material-on-ir) ## :beers: Disclaimer Similar to Tensorflow [datasets]
-(https://github.com/tensorflow/datasets) or HuggingFace's [datasets](https://
+(https://github.com/tensorflow/datasets) or Hugging Face's [datasets](https://
 github.com/huggingface/datasets) library, we just downloaded and prepared
 public datasets. We only distribute these datasets in a specific format, but we
 do not vouch for their quality or fairness, or claim that you have license to
 use the dataset. It remains the user's responsibility to determine whether you
 as a user have permission to use the dataset under the dataset's license and to
 cite the right owner of the dataset. If you're a dataset owner and wish to
 update any part of it, or do not want your dataset to be included in this
@@ -157,25 +172,32 @@
 Heterogenous Benchmark for Zero-shot Evaluation of Information Retrieval
 Models](https://arxiv.org/abs/2104.08663): ``` @inproceedings{ thakur2021beir,
 title={{BEIR}: A Heterogeneous Benchmark for Zero-shot Evaluation of
 Information Retrieval Models}, author={Nandan Thakur and Nils Reimers and
 Andreas R{\"u}ckl{\'e} and Abhishek Srivastava and Iryna Gurevych}, booktitle=
 {Thirty-fifth Conference on Neural Information Processing Systems Datasets and
 Benchmarks Track (Round 2)}, year={2021}, url={https://openreview.net/
-forum?id=wCu6T5xFjeJ} } ``` The main contributors of this repository are: -
+forum?id=wCu6T5xFjeJ} } ``` If you use any baseline score from the BEIR
+leaderboard, feel free to cite our publication [Resources for Brewing BEIR:
+Reproducible Reference Models and an Official Leaderboard](https://arxiv.org/
+abs/2306.07471) ``` @misc{kamalloo2023resources, title={Resources for Brewing
+BEIR: Reproducible Reference Models and an Official Leaderboard}, author={Ehsan
+Kamalloo and Nandan Thakur and Carlos Lassance and Xueguang Ma and Jheng-Hong
+Yang and Jimmy Lin}, year={2023}, eprint={2306.07471}, archivePrefix={arXiv},
+primaryClass={cs.IR} } ``` The main contributors of this repository are: -
 [Nandan Thakur](https://github.com/Nthakur20), Personal Website: [nandan-
 thakur.com](https://nandan-thakur.com) Contact person: Nandan Thakur,
 [nandant@gmail.com](mailto:nandant@gmail.com) Don't hesitate to send us an e-
 mail or report an issue, if something is broken (and it shouldn't be) or if you
 have further questions. > This repository contains experimental software and is
 published for the sole purpose of giving additional background details on the
 respective publication. ## :beers: Collaboration The BEIR Benchmark has been
 made possible due to a collaborative effort of the following universities and
 organizations: - [UKP Lab, Technical University of Darmstadt](http://
 www.ukp.tu-darmstadt.de/) - [University of Waterloo](https://uwaterloo.ca/) -
-[HuggingFace](https://huggingface.co/) ## :beers: Contributors Thanks go to all
-these wonderful collaborations for their contribution towards the BEIR
+[Hugging Face](https://huggingface.co/) ## :beers: Contributors Thanks go to
+all these wonderful collaborations for their contribution towards the BEIR
 benchmark:
 
 Nandan_Thakur Nils_Reimers  Iryna   Jimmy_Lin   Andreas_RÃ¼cklÃ� Abhishek
                            Gurevych                                Srivastava
```

### Comparing `beir-1.0.1/beir/datasets/data_loader.py` & `beir-2.0.0/beir/datasets/data_loader.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/datasets/data_loader_hf.py` & `beir-2.0.0/beir/datasets/data_loader_hf.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/generation/generate.py` & `beir-2.0.0/beir/generation/generate.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/generation/models/auto_model.py` & `beir-2.0.0/beir/generation/models/auto_model.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/generation/models/tilde.py` & `beir-2.0.0/beir/generation/models/tilde.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/losses/bpr_loss.py` & `beir-2.0.0/beir/losses/bpr_loss.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/losses/margin_mse_loss.py` & `beir-2.0.0/beir/losses/margin_mse_loss.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/reranking/models/cross_encoder.py` & `beir-2.0.0/beir/reranking/models/cross_encoder.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/reranking/models/mono_t5.py` & `beir-2.0.0/beir/reranking/models/mono_t5.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/reranking/rerank.py` & `beir-2.0.0/beir/reranking/rerank.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/retrieval/custom_metrics.py` & `beir-2.0.0/beir/retrieval/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/retrieval/evaluation.py` & `beir-2.0.0/beir/retrieval/evaluation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import pytrec_eval
 import logging
-from typing import Type, List, Dict, Union, Tuple
-from .search.dense import DenseRetrievalExactSearch as DRES
-from .search.dense import DenseRetrievalFaissSearch as DRFS
-from .search.lexical import BM25Search as BM25
-from .search.sparse import SparseSearch as SS
+from typing import List, Dict, Tuple
+from .search.base import BaseSearch
 from .custom_metrics import mrr, recall_cap, hole, top_k_accuracy
 
 logger = logging.getLogger(__name__)
 
 class EvaluateRetrieval:
     
-    def __init__(self, retriever: Union[Type[DRES], Type[DRFS], Type[BM25], Type[SS]] = None, k_values: List[int] = [1,3,5,10,100,1000], score_function: str = "cos_sim"):
+    def __init__(self, retriever: BaseSearch = None, k_values: List[int] = [1,3,5,10,100,1000], score_function: str = "cos_sim"):
         self.k_values = k_values
         self.top_k = max(k_values)
         self.retriever = retriever
         self.score_function = score_function
             
     def retrieve(self, corpus: Dict[str, Dict[str, str]], queries: Dict[str, str], **kwargs) -> Dict[str, Dict[str, float]]:
         if not self.retriever:
```

### Comparing `beir-1.0.1/beir/retrieval/models/bpr.py` & `beir-2.0.0/beir/retrieval/models/bpr.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/retrieval/models/dpr.py` & `beir-2.0.0/beir/retrieval/models/dpr.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/retrieval/models/sentence_bert.py` & `beir-2.0.0/beir/retrieval/models/sentence_bert.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/retrieval/models/sparta.py` & `beir-2.0.0/beir/retrieval/models/sparta.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/retrieval/models/splade.py` & `beir-2.0.0/beir/retrieval/models/splade.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/retrieval/models/tldr.py` & `beir-2.0.0/beir/retrieval/models/tldr.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/retrieval/models/unicoil.py` & `beir-2.0.0/beir/retrieval/models/unicoil.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/retrieval/models/use_qa.py` & `beir-2.0.0/beir/retrieval/models/use_qa.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import numpy as np
 import importlib.util
 from typing import List, Dict
 from tqdm.autonotebook import trange
 
-if importlib.util.find_spec("tensorflow") is not None:
+if importlib.util.find_spec("tensorflow") is not None \
+    and importlib.util.find_spec("tensorflow_hub") is not None \
+    and importlib.util.find_spec("tensorflow_text") is not None:
     import tensorflow as tf
     import tensorflow_hub as hub
     import tensorflow_text
 
 class UseQA:
     def __init__(self, hub_url=None, **kwargs):
         self.initialisation()
@@ -45,8 +47,8 @@
 
             embeddings_c = self.model.signatures['response_encoder'](
                 input=tf.constant(titles),
                 context=tf.constant(texts))
             for emb in embeddings_c["outputs"]:
                 output.append(emb)
                     
-        return np.asarray(output)
+        return np.asarray(output)
```

### Comparing `beir-1.0.1/beir/retrieval/search/dense/exact_search_multi_gpu.py` & `beir-2.0.0/beir/retrieval/search/dense/exact_search_multi_gpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+from .. import BaseSearch
 from .util import cos_sim, dot_score
 from sentence_transformers import SentenceTransformer
 from torch.utils.data import DataLoader
-from datasets import Features, Value, Sequence
+from datasets import Features, Value
 from datasets.utils.filelock import FileLock
 from datasets import Array2D, Dataset
 from tqdm.autonotebook import tqdm
-from datetime import datetime
-from typing import Dict, List, Tuple
+from typing import Dict, List
 
 import logging
 import torch
 import math
 import queue
 import os
 import time
@@ -38,28 +38,26 @@
             )
 
         def _compute(self, cos_scores_top_k_values, cos_scores_top_k_idx, batch_index):
             for i in range(len(batch_index) - 1, -1, -1):
                 if batch_index[i] == -1:
                     del cos_scores_top_k_values[i]
                     del cos_scores_top_k_idx[i]
-            batch_index = [e for e in batch_index if e != -1]
-            batch_index = np.repeat(batch_index, len(cos_scores_top_k_values[0]))
             cos_scores_top_k_values = np.concatenate(cos_scores_top_k_values, axis=0)
             cos_scores_top_k_idx = np.concatenate(cos_scores_top_k_idx, axis=0)
-            return cos_scores_top_k_values, cos_scores_top_k_idx, batch_index[:len(cos_scores_top_k_values)]
+            return cos_scores_top_k_values, cos_scores_top_k_idx
 
         def warmup(self):
             """
             Add dummy batch to acquire filelocks for all processes and avoid getting errors
             """
             self.add_batch(cos_scores_top_k_values=torch.ones((1, 1, self.len_queries), dtype=torch.float32), cos_scores_top_k_idx=torch.ones((1, 1, self.len_queries), dtype=torch.int32), batch_index=-torch.ones(1, dtype=torch.int32))
 
 #Parent class for any dense model
-class DenseRetrievalParallelExactSearch:
+class DenseRetrievalParallelExactSearch(BaseSearch):
     
     def __init__(self, model, batch_size: int = 128, corpus_chunk_size: int = None, target_devices: List[str] = None, **kwargs):
         #model is class that provides encode_corpus() and encode_queries()
         self.model = model
         self.batch_size = batch_size
         if target_devices is None:
             if torch.cuda.is_available():
@@ -67,28 +65,28 @@
             else:
                 logger.info("CUDA is not available. Start 4 CPU worker")
                 target_devices = ['cpu']*1 # 4
         self.target_devices = target_devices  # PyTorch target devices, e.g. cuda:0, cuda:1... If None, all available CUDA devices will be used, or 4 CPU processes
         self.score_functions = {'cos_sim': cos_sim, 'dot': dot_score}
         self.score_function_desc = {'cos_sim': "Cosine Similarity", 'dot': "Dot Product"}
         self.corpus_chunk_size = corpus_chunk_size
-        self.show_progress_bar = True #TODO: implement no progress bar if false
-        self.convert_to_tensor = True
+        self.show_progress_bar = kwargs.get("show_progress_bar", True)
+        self.convert_to_tensor = kwargs.get("convert_to_tensor", True)
         self.results = {}
 
         self.query_embeddings = {}
         self.top_k = None
         self.score_function = None
         self.sort_corpus = True
         self.experiment_id = "exact_search_multi_gpu" # f"test_{datetime.now().strftime('%Y-%m-%d_%H-%M-%S')}"
     
     def search(self, 
                corpus: Dataset, 
                queries: Dataset, 
-               top_k: List[int], 
+               top_k: int, 
                score_function: str,
                **kwargs) -> Dict[str, Dict[str, float]]:
         #Create embeddings for all queries using model.encode_queries()
         #Runs semantic search against the corpus embeddings
         #Returns a ranked list with the corpus ids
         if score_function not in self.score_functions:
             raise ValueError("score function: {} must be either (cos_sim) for cosine similarity or (dot) for dot product".format(score_function))
@@ -143,16 +141,15 @@
 
         # Gather all results
         DummyMetric.len_queries = len(queries)
         metric = DummyMetric(experiment_id=self.experiment_id, num_process=len(self.target_devices), process_id=0)
         metric.filelock = FileLock(os.path.join(metric.data_dir, f"{metric.experiment_id}-{metric.num_process}-{metric.process_id}.arrow.lock"))
         metric.cache_file_name = os.path.join(metric.data_dir, f"{metric.experiment_id}-{metric.num_process}-{metric.process_id}.arrow")
 
-        cos_scores_top_k_values, cos_scores_top_k_idx, chunk_ids = metric.compute()
-        cos_scores_top_k_idx = (cos_scores_top_k_idx.T + chunk_ids * self.corpus_chunk_size).T
+        cos_scores_top_k_values, cos_scores_top_k_idx = metric.compute()
 
         # sort similar docs for each query by cosine similarity and keep only top_k
         sorted_idx = np.argsort(cos_scores_top_k_values, axis=0)[::-1]
         sorted_idx = sorted_idx[:self.top_k+1]
         cos_scores_top_k_values = np.take_along_axis(cos_scores_top_k_values, sorted_idx, axis=0)
         cos_scores_top_k_idx = np.take_along_axis(cos_scores_top_k_idx, sorted_idx, axis=0)
 
@@ -192,14 +189,17 @@
                     cos_scores[torch.isnan(cos_scores)] = -1
 
                     #Get top-k values
                     cos_scores_top_k_values, cos_scores_top_k_idx = torch.topk(cos_scores, min(self.top_k+1, len(cos_scores[1])), dim=1, largest=True, sorted=False)
                     cos_scores_top_k_values = cos_scores_top_k_values.T.unsqueeze(0).detach()
                     cos_scores_top_k_idx = cos_scores_top_k_idx.T.unsqueeze(0).detach()
 
+                    # correct sentence ids
+                    cos_scores_top_k_idx += id * self.corpus_chunk_size
+
                     # Store results in an Apache Arrow table
                     metric.add_batch(cos_scores_top_k_values=cos_scores_top_k_values, cos_scores_top_k_idx=cos_scores_top_k_idx, batch_index=[id]*len(cos_scores_top_k_values))
 
                     # Alarm that process finished processing a batch
                     results_queue.put(None)
                 except queue.Empty:
                     break
```

### Comparing `beir-1.0.1/beir/retrieval/search/dense/faiss_index.py` & `beir-2.0.0/beir/retrieval/search/dense/faiss_index.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/retrieval/search/dense/faiss_search.py` & `beir-2.0.0/beir/retrieval/search/dense/faiss_search.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from .util import cos_sim, dot_score, normalize, save_dict_to_tsv, load_tsv_to_dict
+from .. import BaseSearch
+from .util import save_dict_to_tsv, load_tsv_to_dict
 from .faiss_index import FaissBinaryIndex, FaissTrainIndex, FaissHNSWIndex, FaissIndex
 import logging
-import sys
-import torch
 import faiss
 import numpy as np
 import os
-from typing import Dict, List
+from typing import Dict
 from tqdm.autonotebook import tqdm
 
 logger = logging.getLogger(__name__)
 
 #Parent class for any faiss search
-class DenseRetrievalFaissSearch:
+class DenseRetrievalFaissSearch(BaseSearch):
     
-    def __init__(self, model, batch_size: int = 128, corpus_chunk_size: int = 50000, **kwargs):
+    def __init__(self, model, batch_size: int = 128, corpus_chunk_size: int = 50000, use_gpu: bool = False, **kwargs):
         self.model = model
         self.batch_size = batch_size
         self.corpus_chunk_size = corpus_chunk_size
         self.score_functions = ['cos_sim','dot']
         self.mapping_tsv_keys = ["beir-docid", "faiss-docid"]
         self.faiss_index = None
+        self.use_gpu = use_gpu
+        self.single_gpu = faiss.StandardGpuResources() if use_gpu else None
         self.dim_size = 0
         self.results = {}
         self.mapping = {}
         self.rev_mapping = {}
     
     def _create_mapping_ids(self, corpus_ids):
         if not all(isinstance(doc_id, int) for doc_id in corpus_ids):
@@ -69,15 +70,15 @@
         normalize_embeddings = True if score_function == "cos_sim" else False
 
         logger.info("Encoding Corpus in batches... Warning: This might take a while!")
 
         itr = range(0, len(corpus), self.corpus_chunk_size)
 
         for batch_num, corpus_start_idx in enumerate(itr):
-            logger.info("Encoding Batch {}/{}...".format(batch_num+1, len(itr)))
+            logger.info("Encoding Batch {}/{}. Normalize: {}...".format(batch_num+1, len(itr), normalize_embeddings))
             corpus_end_idx = min(corpus_start_idx + self.corpus_chunk_size, len(corpus))
             
             #Encode chunk of corpus    
             sub_corpus_embeddings = self.model.encode_corpus(
                 corpus[corpus_start_idx:corpus_end_idx],
                 batch_size=self.batch_size,
                 show_progress_bar=True, 
@@ -101,23 +102,26 @@
     def search(self, 
                corpus: Dict[str, Dict[str, str]],
                queries: Dict[str, str], 
                top_k: int,
                score_function = str, **kwargs) -> Dict[str, Dict[str, float]]:
         
         assert score_function in self.score_functions
+        normalize_embeddings = True if score_function == "cos_sim" else False
 
         if not self.faiss_index: self.index(corpus, score_function)
 
-        logger.info("Encoding Queries...")
         query_ids = list(queries.keys())
         queries = [queries[qid] for qid in queries]
+        logger.info("Computing Query Embeddings. Normalize: {}...".format(normalize_embeddings))
         query_embeddings = self.model.encode_queries(
-            queries, show_progress_bar=True, batch_size=self.batch_size)
-
+            queries, show_progress_bar=True, 
+            batch_size=self.batch_size, 
+            normalize_embeddings=normalize_embeddings)
+        
         faiss_scores, faiss_doc_ids = self.faiss_index.search(query_embeddings, top_k, **kwargs)
         
         for idx in range(len(query_ids)):
             scores = [float(score) for score in faiss_scores[idx]]
             if len(self.rev_mapping) != 0:
                 doc_ids = [self.rev_mapping[doc_id] for doc_id in faiss_doc_ids[idx]]
             else:
@@ -169,15 +173,20 @@
         self.code_size = code_size
         self.similarity_metric = similarity_metric
         self.use_rotation = use_rotation
     
     def load(self, input_dir: str, prefix: str = "my-index", ext: str = "pq"):
         input_faiss_path, passage_ids = super()._load(input_dir, prefix, ext)
         base_index = faiss.read_index(input_faiss_path)
-        self.faiss_index = FaissTrainIndex(base_index, passage_ids)
+        if self.use_gpu:
+            logger.info("Moving Faiss Index from CPU to GPU...")
+            gpu_base_index = faiss.index_cpu_to_gpu(self.single_gpu, 0, base_index)
+            self.faiss_index = FaissTrainIndex(gpu_base_index, passage_ids)
+        else:
+            self.faiss_index = FaissTrainIndex(base_index, passage_ids)
 
     def index(self, corpus: Dict[str, Dict[str, str]], score_function: str = None, **kwargs):
         faiss_ids, corpus_embeddings = super()._index(corpus, score_function, **kwargs)  
 
         logger.info("Using Product Quantization (PQ) in Flat mode!")
         logger.info("Parameters Used: num_of_centroids: {} ".format(self.num_of_centroids))
         logger.info("Parameters Used: code_size: {}".format(self.code_size))          
@@ -185,16 +194,22 @@
         base_index = faiss.IndexPQ(self.dim_size, self.num_of_centroids, self.code_size, self.similarity_metric)
 
         if self.use_rotation:
             logger.info("Rotating data before encoding it with a product quantizer...")
             logger.info("Creating OPQ Matrix...")
             opq_matrix = faiss.OPQMatrix(self.dim_size, self.code_size)
             base_index = faiss.IndexPreTransform(opq_matrix, base_index)
-
-        self.faiss_index = FaissTrainIndex.build(faiss_ids, corpus_embeddings, base_index)
+        
+        if self.use_gpu:
+            logger.info("Moving Faiss Index from CPU to GPU...")
+            gpu_base_index = faiss.index_cpu_to_gpu(self.single_gpu, 0, base_index)
+            self.faiss_index = FaissTrainIndex.build(faiss_ids, corpus_embeddings, gpu_base_index)
+        
+        else:
+            self.faiss_index = FaissTrainIndex.build(faiss_ids, corpus_embeddings, base_index)
 
     def save(self, output_dir: str, prefix: str = "my-index", ext: str = "pq"):
         super().save(output_dir, prefix, ext)
     
     def search(self, 
             corpus: Dict[str, Dict[str, str]],
             queries: Dict[str, str], 
@@ -215,28 +230,39 @@
         self.hnsw_ef_search = hnsw_ef_search
         self.hnsw_ef_construction = hnsw_ef_construction
         self.similarity_metric = similarity_metric
     
     def load(self, input_dir: str, prefix: str = "my-index", ext: str = "hnsw"):
         input_faiss_path, passage_ids = super()._load(input_dir, prefix, ext)
         base_index = faiss.read_index(input_faiss_path)
-        self.faiss_index = FaissHNSWIndex(base_index, passage_ids)
+        if self.use_gpu:
+            logger.info("Moving Faiss Index from CPU to GPU...")
+            gpu_base_index = faiss.index_cpu_to_gpu(self.single_gpu, 0, base_index)
+            self.faiss_index = FaissHNSWIndex(gpu_base_index, passage_ids)
+        else:
+            self.faiss_index = FaissHNSWIndex(base_index, passage_ids)
+
     
     def index(self, corpus: Dict[str, Dict[str, str]], score_function: str = None, **kwargs):
         faiss_ids, corpus_embeddings = super()._index(corpus, score_function, **kwargs)
 
         logger.info("Using Approximate Nearest Neighbours (HNSW) in Flat Mode!")
         logger.info("Parameters Required: hnsw_store_n: {}".format(self.hnsw_store_n))
         logger.info("Parameters Required: hnsw_ef_search: {}".format(self.hnsw_ef_search))
         logger.info("Parameters Required: hnsw_ef_construction: {}".format(self.hnsw_ef_construction))
         
         base_index = faiss.IndexHNSWFlat(self.dim_size + 1, self.hnsw_store_n, self.similarity_metric)
         base_index.hnsw.efSearch = self.hnsw_ef_search
         base_index.hnsw.efConstruction = self.hnsw_ef_construction
-        self.faiss_index = FaissHNSWIndex.build(faiss_ids, corpus_embeddings, base_index)
+        if self.use_gpu:
+            logger.info("Moving Faiss Index from CPU to GPU...")
+            gpu_base_index = faiss.index_cpu_to_gpu(self.single_gpu, 0, base_index)
+            self.faiss_index = FaissHNSWIndex.build(faiss_ids, corpus_embeddings, gpu_base_index)
+        else:
+            self.faiss_index = FaissHNSWIndex.build(faiss_ids, corpus_embeddings, base_index)
 
     def save(self, output_dir: str, prefix: str = "my-index", ext: str = "hnsw"):
         super().save(output_dir, prefix, ext)
     
     def search(self, 
             corpus: Dict[str, Dict[str, str]],
             queries: Dict[str, str], 
@@ -293,20 +319,30 @@
     def get_index_name(self):
         return "hnswsq_faiss_index"
 
 class FlatIPFaissSearch(DenseRetrievalFaissSearch):
     def load(self, input_dir: str, prefix: str = "my-index", ext: str = "flat"):
         input_faiss_path, passage_ids = super()._load(input_dir, prefix, ext)
         base_index = faiss.read_index(input_faiss_path)
-        self.faiss_index = FaissIndex(base_index, passage_ids)
+        if self.use_gpu:
+            logger.info("Moving Faiss Index from CPU to GPU...")
+            gpu_base_index = faiss.index_cpu_to_gpu(self.single_gpu, 0, base_index)
+            self.faiss_index = FaissIndex(gpu_base_index, passage_ids)
+        else:
+            self.faiss_index = FaissIndex(base_index, passage_ids)
 
     def index(self, corpus: Dict[str, Dict[str, str]], score_function: str = None, **kwargs):
         faiss_ids, corpus_embeddings = super()._index(corpus, score_function, **kwargs)
         base_index = faiss.IndexFlatIP(self.dim_size)
-        self.faiss_index = FaissIndex.build(faiss_ids, corpus_embeddings, base_index)
+        if self.use_gpu:
+            logger.info("Moving Faiss Index from CPU to GPU...")
+            gpu_base_index = faiss.index_cpu_to_gpu(self.single_gpu, 0, base_index)
+            self.faiss_index = FaissIndex.build(faiss_ids, corpus_embeddings, gpu_base_index)
+        else:
+            self.faiss_index = FaissIndex.build(faiss_ids, corpus_embeddings, base_index)
 
     def save(self, output_dir: str, prefix: str = "my-index", ext: str = "flat"):
         super().save(output_dir, prefix, ext)
     
     def search(self, 
             corpus: Dict[str, Dict[str, str]],
             queries: Dict[str, str], 
@@ -316,31 +352,53 @@
         return super().search(corpus, queries, top_k, score_function, **kwargs)
     
     def get_index_name(self):
         return "flat_faiss_index"
 
 class PCAFaissSearch(DenseRetrievalFaissSearch):
     def __init__(self, model, base_index: faiss.Index, output_dimension: int, batch_size: int = 128, 
-                corpus_chunk_size: int = 50000, **kwargs):
+                corpus_chunk_size: int = 50000, pca_matrix = None, random_rotation: bool = False, 
+                eigen_power: float = 0.0, **kwargs):
         super(PCAFaissSearch, self).__init__(model, batch_size, corpus_chunk_size, **kwargs)
         self.base_index = base_index
         self.output_dim = output_dimension
+        self.pca_matrix = pca_matrix
+        self.random_rotation = random_rotation
+        self.eigen_power = eigen_power
 
     def load(self, input_dir: str, prefix: str = "my-index", ext: str = "pca"):
         input_faiss_path, passage_ids = super()._load(input_dir, prefix, ext)
         base_index = faiss.read_index(input_faiss_path)
-        self.faiss_index = FaissTrainIndex(base_index, passage_ids)
+        if self.use_gpu:
+            logger.info("Moving Faiss Index from CPU to GPU...")
+            gpu_base_index = faiss.index_cpu_to_gpu(self.single_gpu, 0, base_index)
+            self.faiss_index = FaissTrainIndex(gpu_base_index, passage_ids)
+        else:
+            self.faiss_index = FaissTrainIndex(base_index, passage_ids)
+
 
     def index(self, corpus: Dict[str, Dict[str, str]], score_function: str = None, **kwargs):
         faiss_ids, corpus_embeddings = super()._index(corpus, score_function, **kwargs)
         logger.info("Creating PCA Matrix...")
         logger.info("Input Dimension: {}, Output Dimension: {}".format(self.dim_size, self.output_dim))
-        pca_matrix = faiss.PCAMatrix(self.dim_size, self.output_dim, 0, True)
+        pca_matrix = faiss.PCAMatrix(self.dim_size, self.output_dim, self.eigen_power, self.random_rotation)
+        logger.info("Random Rotation in PCA Matrix is set to: {}".format(self.random_rotation))
+        logger.info("Whitening in PCA Matrix is set to: {}".format(self.eigen_power))
+        if self.pca_matrix is not None:
+            pca_matrix = pca_matrix.copy_from(self.pca_matrix)
+        self.pca_matrix = pca_matrix
+        
+        # Final index
         final_index = faiss.IndexPreTransform(pca_matrix, self.base_index)
-        self.faiss_index = FaissTrainIndex.build(faiss_ids, corpus_embeddings, final_index)
+        if self.use_gpu:
+            logger.info("Moving Faiss Index from CPU to GPU...")
+            gpu_base_index = faiss.index_cpu_to_gpu(self.single_gpu, 0, final_index)
+            self.faiss_index = FaissTrainIndex.build(faiss_ids, corpus_embeddings, gpu_base_index)
+        else:
+            self.faiss_index = FaissTrainIndex.build(faiss_ids, corpus_embeddings, final_index)
 
     def save(self, output_dir: str, prefix: str = "my-index", ext: str = "pca"):
         super().save(output_dir, prefix, ext)
     
     def search(self, 
             corpus: Dict[str, Dict[str, str]],
             queries: Dict[str, str], 
@@ -358,25 +416,35 @@
         super(SQFaissSearch, self).__init__(model, batch_size, corpus_chunk_size, **kwargs)
         self.similarity_metric = similarity_metric
         self.qname = quantizer_type
 
     def load(self, input_dir: str, prefix: str = "my-index", ext: str = "sq"):
         input_faiss_path, passage_ids = super()._load(input_dir, prefix, ext)
         base_index = faiss.read_index(input_faiss_path)
-        self.faiss_index = FaissTrainIndex(base_index, passage_ids)
+        if self.use_gpu:
+            logger.info("Moving Faiss Index from CPU to GPU...")
+            gpu_base_index = faiss.index_cpu_to_gpu(self.single_gpu, 0, base_index)
+            self.faiss_index = FaissTrainIndex(gpu_base_index, passage_ids)
+        else:
+            self.faiss_index = FaissTrainIndex(base_index, passage_ids)
 
     def index(self, corpus: Dict[str, Dict[str, str]], score_function: str = None, **kwargs):
         faiss_ids, corpus_embeddings = super()._index(corpus, score_function, **kwargs)
 
         logger.info("Using Scalar Quantizer in Flat Mode!")
         logger.info("Parameters Used: quantizer_type: {}".format(self.qname))
 
         qtype = getattr(faiss.ScalarQuantizer, self.qname)
         base_index = faiss.IndexScalarQuantizer(self.dim_size, qtype, self.similarity_metric)
-        self.faiss_index = FaissTrainIndex.build(faiss_ids, corpus_embeddings, base_index)
+        if self.use_gpu:
+            logger.info("Moving Faiss Index from CPU to GPU...")
+            gpu_base_index = faiss.index_cpu_to_gpu(self.single_gpu, 0, base_index)
+            self.faiss_index = FaissTrainIndex.build(faiss_ids, corpus_embeddings, gpu_base_index)
+        else:
+            self.faiss_index = FaissTrainIndex.build(faiss_ids, corpus_embeddings, base_index)
 
     def save(self, output_dir: str, prefix: str = "my-index", ext: str = "sq"):
         super().save(output_dir, prefix, ext)
     
     def search(self, 
             corpus: Dict[str, Dict[str, str]],
             queries: Dict[str, str],
```

### Comparing `beir-1.0.1/beir/retrieval/search/dense/util.py` & `beir-2.0.0/beir/retrieval/search/dense/util.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/retrieval/search/lexical/bm25_search.py` & `beir-2.0.0/beir/retrieval/search/lexical/bm25_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from .. import BaseSearch
 from .elastic_search import ElasticSearch
 import tqdm
 import time
 from typing import List, Dict
 
 def sleep(seconds):
     if seconds: time.sleep(seconds) 
 
-class BM25Search:
+class BM25Search(BaseSearch):
     def __init__(self, index_name: str, hostname: str = "localhost", keys: Dict[str, str] = {"title": "title", "body": "txt"}, language: str = "english",
                  batch_size: int = 128, timeout: int = 100, retry_on_timeout: bool = True, maxsize: int = 24, number_of_shards: int = "default", 
                  initialize: bool = True, sleep_for: int = 2):
         self.results = {}
         self.batch_size = batch_size
         self.initialize = initialize
         self.sleep_for = sleep_for
```

### Comparing `beir-1.0.1/beir/retrieval/search/lexical/elastic_search.py` & `beir-2.0.0/beir/retrieval/search/lexical/elastic_search.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir/retrieval/search/sparse/sparse_search.py` & `beir-2.0.0/beir/retrieval/search/sparse/sparse_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from .. import BaseSearch
 from tqdm.autonotebook import trange
-from typing import List, Dict, Union, Tuple
+from typing import Dict
 import logging
 import numpy as np
 
 logger = logging.getLogger(__name__)
 
-class SparseSearch:
+class SparseSearch(BaseSearch):
     
     def __init__(self, model, batch_size: int = 16, **kwargs):
         self.model = model
         self.batch_size = batch_size
         self.sparse_matrix = None
         self.results = {}
```

### Comparing `beir-1.0.1/beir/retrieval/train.py` & `beir-2.0.0/beir/retrieval/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from sentence_transformers import SentenceTransformer, SentencesDataset, models, datasets
+from sentence_transformers import SentenceTransformer, SentencesDataset, datasets
 from sentence_transformers.evaluation import SentenceEvaluator, SequentialEvaluator, InformationRetrievalEvaluator
 from sentence_transformers.readers import InputExample
 from transformers import AdamW
 from torch import nn
 from torch.utils.data import DataLoader
 from torch.optim import Optimizer
 from tqdm.autonotebook import trange
-from typing import Dict, Type, List, Callable, Iterable, Tuple
+from typing import Dict, List, Callable, Iterable, Tuple
 import logging
 import time
-import difflib
+import random
 
 logger = logging.getLogger(__name__)
 
 class TrainRetriever:
     
-    def __init__(self, model: Type[SentenceTransformer], batch_size: int = 64):
+    def __init__(self, model: SentenceTransformer, batch_size: int = 64):
         self.model = model
         self.batch_size = batch_size
 
     def load_train(self, corpus: Dict[str, Dict[str, str]], queries: Dict[str, str], 
-                   qrels: Dict[str, Dict[str, int]]) -> List[Type[InputExample]]:
+                   qrels: Dict[str, Dict[str, int]]) -> List[InputExample]:
         
         query_ids = list(queries.keys())
         train_samples = []
 
         for idx, start_idx in enumerate(trange(0, len(query_ids), self.batch_size, desc='Adding Input Examples')):
             query_ids_batch = query_ids[start_idx:start_idx+self.batch_size]
             for query_id in query_ids_batch:
@@ -36,36 +36,36 @@
                             train_samples.append(InputExample(guid=idx, texts=[s1, s2], label=1))
                         except KeyError:
                             logging.error("Error: Key {} not present in corpus!".format(corpus_id))
 
         logger.info("Loaded {} training pairs.".format(len(train_samples)))
         return train_samples
 
-    def load_train_triplets(self, triplets: List[Tuple[str, str, str]]) -> List[Type[InputExample]]:        
+    def load_train_triplets(self, triplets: List[Tuple[str, str, str]]) -> List[InputExample]:        
         
         train_samples = []
 
         for idx, start_idx in enumerate(trange(0, len(triplets), self.batch_size, desc='Adding Input Examples')):
             triplets_batch = triplets[start_idx:start_idx+self.batch_size]
             for triplet in triplets_batch:
                 guid = None
                 train_samples.append(InputExample(guid=guid, texts=triplet))
 
         logger.info("Loaded {} training pairs.".format(len(train_samples)))
         return train_samples
     
-    def prepare_train(self, train_dataset: List[Type[InputExample]], shuffle: bool = True, dataset_present: bool = False) -> DataLoader:
+    def prepare_train(self, train_dataset: List[InputExample], shuffle: bool = True, dataset_present: bool = False) -> DataLoader:
         
         if not dataset_present: 
             train_dataset = SentencesDataset(train_dataset, model=self.model)
         
         train_dataloader = DataLoader(train_dataset, shuffle=shuffle, batch_size=self.batch_size)
         return train_dataloader
     
-    def prepare_train_triplets(self, train_dataset: List[Type[InputExample]]) -> DataLoader:
+    def prepare_train_triplets(self, train_dataset: List[InputExample]) -> DataLoader:
         
         train_dataloader = datasets.NoDuplicatesDataLoader(train_dataset, batch_size=self.batch_size)
         return train_dataloader
     
     def load_ir_evaluator(self, corpus: Dict[str, Dict[str, str]], queries: Dict[str, str], 
                  qrels: Dict[str, Dict[str, int]], max_corpus_size: int = None, name: str = "eval") -> SentenceEvaluator:
 
@@ -113,15 +113,15 @@
     def fit(self, 
             train_objectives: Iterable[Tuple[DataLoader, nn.Module]],
             evaluator: SentenceEvaluator = None,
             epochs: int = 1,
             steps_per_epoch = None,
             scheduler: str = 'WarmupLinear',
             warmup_steps: int = 10000,
-            optimizer_class: Type[Optimizer] = AdamW,
+            optimizer_class: Optimizer = AdamW,
             optimizer_params : Dict[str, object]= {'lr': 2e-5, 'eps': 1e-6, 'correct_bias': False},
             weight_decay: float = 0.01,
             evaluation_steps: int = 0,
             output_path: str = None,
             save_best_model: bool = True,
             max_grad_norm: float = 1,
             use_amp: bool = False,
```

### Comparing `beir-1.0.1/beir/util.py` & `beir-2.0.0/beir/util.py`

 * *Files identical despite different names*

### Comparing `beir-1.0.1/beir.egg-info/PKG-INFO` & `beir-2.0.0/beir.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: beir
-Version: 1.0.1
+Version: 2.0.0
 Summary: A Heterogeneous Benchmark for Information Retrieval
 Home-page: https://github.com/beir-cellar/beir
-Download-URL: https://github.com/beir-cellar/beir/archive/v1.0.1.zip
 Author: Nandan Thakur
 Author-email: nandant@gmail.com
 License: Apache License 2.0
+Download-URL: https://github.com/beir-cellar/beir/archive/v2.0.0.zip
 Keywords: Information Retrieval Transformer Networks BERT PyTorch IR NLP deep learning
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -70,19 +70,22 @@
 
 ## :beers: What is it?
 
 **BEIR** is a **heterogeneous benchmark** containing diverse IR tasks. It also provides a **common and easy framework** for evaluation of your NLP-based retrieval models within the benchmark.
 
 For **an overview**, checkout our **new wiki** page: [https://github.com/beir-cellar/beir/wiki](https://github.com/beir-cellar/beir/wiki).
 
-For **models and datasets**, checkout out **HuggingFace (HF)** page: [https://huggingface.co/BeIR](https://huggingface.co/BeIR).
+For **models and datasets**, checkout out **Hugging Face (HF)** page: [https://huggingface.co/BeIR](https://huggingface.co/BeIR).
+
+For **Leaderboard**, checkout out **Eval AI** page: [https://eval.ai/web/challenges/challenge-page/1897](https://eval.ai/web/challenges/challenge-page/1897).
 
 For more information, checkout out our publications:
 
 - [BEIR: A Heterogenous Benchmark for Zero-shot Evaluation of Information Retrieval Models](https://openreview.net/forum?id=wCu6T5xFjeJ) (NeurIPS 2021, Datasets and Benchmarks Track)
+- [Resources for Brewing BEIR: Reproducible Reference Models and an Official Leaderboard](https://arxiv.org/abs/2306.07471) (Arxiv 2023)
 
 ## :beers: Installation
 
 Install via pip:
 
 ```python
 pip install beir
@@ -144,23 +147,23 @@
 ndcg, _map, recall, precision = retriever.evaluate(qrels, results, retriever.k_values)
 ```
 
 ## :beers: Available Datasets
 
 Command to generate md5hash using Terminal:  ``md5sum filename.zip``.
 
-You can view all datasets available **[here](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/)** or on **[HuggingFace](https://huggingface.co/BeIR)**.
+You can view all datasets available **[here](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/)** or on **[Hugging Face](https://huggingface.co/BeIR)**.
 
 
 | Dataset   | Website| BEIR-Name | Public? | Type | Queries  | Corpus | Rel D/Q | Down-load | md5 |
 | -------- | -----| ---------| ------- | --------- | ----------- | ---------| ---------| :----------: | :------:|
 | MSMARCO    | [Homepage](https://microsoft.github.io/msmarco/)| ``msmarco`` | ✅ | ``train``<br>``dev``<br>``test``|  6,980   |  8.84M     |    1.1 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/msmarco.zip) | ``444067daf65d982533ea17ebd59501e4`` |
 | TREC-COVID |  [Homepage](https://ir.nist.gov/covidSubmit/index.html)| ``trec-covid``| ✅ | ``test``| 50|  171K| 493.5 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/trec-covid.zip) | ``ce62140cb23feb9becf6270d0d1fe6d1`` |
 | NFCorpus   | [Homepage](https://www.cl.uni-heidelberg.de/statnlpgroup/nfcorpus/) | ``nfcorpus`` | ✅ |``train``<br>``dev``<br>``test``|  323     |  3.6K     |  38.2 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/nfcorpus.zip) | ``a89dba18a62ef92f7d323ec890a0d38d`` |
-| BioASQ     | [Homepage](http://bioasq.org) | ``bioasq``| ❌ | ``train``<br>``test`` | 500 |  14.91M    |  8.05 | No | [How to Reproduce?](https://github.com/beir-cellar/beir/blob/main/examples/dataset#2-bioasq) |
+| BioASQ     | [Homepage](http://bioasq.org) | ``bioasq``| ❌ | ``train``<br>``test`` | 500 |  14.91M    |  4.7 | No | [How to Reproduce?](https://github.com/beir-cellar/beir/blob/main/examples/dataset#2-bioasq) |
 | NQ         | [Homepage](https://ai.google.com/research/NaturalQuestions) | ``nq``| ✅ | ``train``<br>``test``| 3,452   |  2.68M  |  1.2 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/nq.zip) | ``d4d3d2e48787a744b6f6e691ff534307`` |
 | HotpotQA   | [Homepage](https://hotpotqa.github.io) | ``hotpotqa``| ✅ |``train``<br>``dev``<br>``test``|  7,405   |  5.23M  |  2.0 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/hotpotqa.zip)  | ``f412724f78b0d91183a0e86805e16114`` |
 | FiQA-2018  | [Homepage](https://sites.google.com/view/fiqa/) | ``fiqa`` | ✅ | ``train``<br>``dev``<br>``test``|  648     |  57K    |  2.6 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/fiqa.zip)  | ``17918ed23cd04fb15047f73e6c3bd9d9`` |
 | Signal-1M(RT) | [Homepage](https://research.signal-ai.com/datasets/signal1m-tweetir.html)| ``signal1m`` | ❌ | ``test``| 97   |  2.86M  |  19.6 | No | [How to Reproduce?](https://github.com/beir-cellar/beir/blob/main/examples/dataset#4-signal-1m) |
 | TREC-NEWS  | [Homepage](https://trec.nist.gov/data/news2019.html) | ``trec-news`` | ❌ | ``test``| 57    |  595K    |  19.6 | No | [How to Reproduce?](https://github.com/beir-cellar/beir/blob/main/examples/dataset#1-trec-news) |
 | Robust04 | [Homepage](https://trec.nist.gov/data/robust/04.guidelines.html) | ``robust04``| ❌ | ``test``| 249  |  528K  |  69.9 |  No  |  [How to Reproduce?](https://github.com/beir-cellar/beir/blob/main/examples/dataset#3-robust04)  |
 | ArguAna    | [Homepage](http://argumentation.bplaced.net/arguana/data) | ``arguana``| ✅ |``test`` | 1,406     |  8.67K    |  1.0 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/arguana.zip)  | ``8ad3e3c2a5867cdced806d6503f29b99`` |
@@ -202,15 +205,15 @@
 ### Miscellaneous
 
 - [BEIR Leaderboard](https://github.com/beir-cellar/beir/wiki/Leaderboard)
 - [Couse Material on IR](https://github.com/beir-cellar/beir/wiki/Course-material-on-ir)
 
 ## :beers: Disclaimer
 
-Similar to Tensorflow [datasets](https://github.com/tensorflow/datasets) or HuggingFace's [datasets](https://github.com/huggingface/datasets) library, we just downloaded and prepared public datasets. We only distribute these datasets in a specific format, but we do not vouch for their quality or fairness, or claim that you have license to use the dataset. It remains the user's responsibility to determine whether you as a user have permission to use the dataset under the dataset's license and to cite the right owner of the dataset.
+Similar to Tensorflow [datasets](https://github.com/tensorflow/datasets) or Hugging Face's [datasets](https://github.com/huggingface/datasets) library, we just downloaded and prepared public datasets. We only distribute these datasets in a specific format, but we do not vouch for their quality or fairness, or claim that you have license to use the dataset. It remains the user's responsibility to determine whether you as a user have permission to use the dataset under the dataset's license and to cite the right owner of the dataset.
 
 If you're a dataset owner and wish to update any part of it, or do not want your dataset to be included in this library, feel free to post an issue here or make a pull request!
 
 If you're a dataset owner and wish to include your dataset or model in this library, feel free to post an issue here or make a pull request!
 
 ## :beers: Citing & Authors
 
@@ -223,29 +226,41 @@
     author={Nandan Thakur and Nils Reimers and Andreas R{\"u}ckl{\'e} and Abhishek Srivastava and Iryna Gurevych},
     booktitle={Thirty-fifth Conference on Neural Information Processing Systems Datasets and Benchmarks Track (Round 2)},
     year={2021},
     url={https://openreview.net/forum?id=wCu6T5xFjeJ}
 }
 ```
 
+If you use any baseline score from the BEIR leaderboard, feel free to cite our publication [Resources for Brewing BEIR: Reproducible Reference Models and an Official Leaderboard](https://arxiv.org/abs/2306.07471)
+```
+@misc{kamalloo2023resources,
+      title={Resources for Brewing BEIR: Reproducible Reference Models and an Official Leaderboard}, 
+      author={Ehsan Kamalloo and Nandan Thakur and Carlos Lassance and Xueguang Ma and Jheng-Hong Yang and Jimmy Lin},
+      year={2023},
+      eprint={2306.07471},
+      archivePrefix={arXiv},
+      primaryClass={cs.IR}
+}
+```
+
 The main contributors of this repository are:
 - [Nandan Thakur](https://github.com/Nthakur20), Personal Website: [nandan-thakur.com](https://nandan-thakur.com)
 
 Contact person: Nandan Thakur, [nandant@gmail.com](mailto:nandant@gmail.com)
 
 Don't hesitate to send us an e-mail or report an issue, if something is broken (and it shouldn't be) or if you have further questions.
 
 > This repository contains experimental software and is published for the sole purpose of giving additional background details on the respective publication.
 
 ## :beers: Collaboration
 
 The BEIR Benchmark has been made possible due to a collaborative effort of the following universities and organizations:
 - [UKP Lab, Technical University of Darmstadt](http://www.ukp.tu-darmstadt.de/)
 - [University of Waterloo](https://uwaterloo.ca/)
-- [HuggingFace](https://huggingface.co/)
+- [Hugging Face](https://huggingface.co/)
 
 ## :beers: Contributors
 
 Thanks go to all these wonderful collaborations for their contribution towards the BEIR benchmark:
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: beir Version: 1.0.1 Summary: A Heterogeneous
+Metadata-Version: 2.1 Name: beir Version: 2.0.0 Summary: A Heterogeneous
 Benchmark for Information Retrieval Home-page: https://github.com/beir-cellar/
-beir Download-URL: https://github.com/beir-cellar/beir/archive/v1.0.1.zip
-Author: Nandan Thakur Author-email: nandant@gmail.com License: Apache License
-2.0 Keywords: Information Retrieval Transformer Networks BERT PyTorch IR NLP
-deep learning Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
+beir Author: Nandan Thakur Author-email: nandant@gmail.com License: Apache
+License 2.0 Download-URL: https://github.com/beir-cellar/beir/archive/
+v2.0.0.zip Keywords: Information Retrieval Transformer Networks BERT PyTorch IR
+NLP deep learning Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3.6 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
 tf License-File: LICENSE License-File: NOTICE.txt
     ****** [https://raw.githubusercontent.com/benchmarkir/beir/main/images/
                   color_logo_transparent_cropped.png] ******
@@ -17,32 +17,36 @@
                                      ****
                           **** [./images/HF.png] ****
 ## :beers: What is it? **BEIR** is a **heterogeneous benchmark** containing
 diverse IR tasks. It also provides a **common and easy framework** for
 evaluation of your NLP-based retrieval models within the benchmark. For **an
 overview**, checkout our **new wiki** page: [https://github.com/beir-cellar/
 beir/wiki](https://github.com/beir-cellar/beir/wiki). For **models and
-datasets**, checkout out **HuggingFace (HF)** page: [https://huggingface.co/
-BeIR](https://huggingface.co/BeIR). For more information, checkout out our
-publications: - [BEIR: A Heterogenous Benchmark for Zero-shot Evaluation of
+datasets**, checkout out **Hugging Face (HF)** page: [https://huggingface.co/
+BeIR](https://huggingface.co/BeIR). For **Leaderboard**, checkout out **Eval
+AI** page: [https://eval.ai/web/challenges/challenge-page/1897](https://
+eval.ai/web/challenges/challenge-page/1897). For more information, checkout out
+our publications: - [BEIR: A Heterogenous Benchmark for Zero-shot Evaluation of
 Information Retrieval Models](https://openreview.net/forum?id=wCu6T5xFjeJ)
-(NeurIPS 2021, Datasets and Benchmarks Track) ## :beers: Installation Install
-via pip: ```python pip install beir ``` If you want to build from source, use:
-```python $ git clone https://github.com/beir-cellar/beir.git $ cd beir $ pip
-install -e . ``` Tested with python versions 3.6 and 3.7 ## :beers: Features -
-Preprocess your own IR dataset or use one of the already-preprocessed 17
-benchmark datasets - Wide settings included, covers diverse benchmarks useful
-for both academia and industry - Includes well-known retrieval architectures
-(lexical, dense, sparse and reranking-based) - Add and evaluate your own model
-in a easy framework using different state-of-the-art evaluation metrics ## :
-beers: Quick Example For other example codes, please refer to our **[Examples
-and Tutorials](https://github.com/beir-cellar/beir/wiki/Examples-and-
-tutorials)** Wiki page. ```python from beir import util, LoggingHandler from
-beir.retrieval import models from beir.datasets.data_loader import
-GenericDataLoader from beir.retrieval.evaluation import EvaluateRetrieval from
+(NeurIPS 2021, Datasets and Benchmarks Track) - [Resources for Brewing BEIR:
+Reproducible Reference Models and an Official Leaderboard](https://arxiv.org/
+abs/2306.07471) (Arxiv 2023) ## :beers: Installation Install via pip: ```python
+pip install beir ``` If you want to build from source, use: ```python $ git
+clone https://github.com/beir-cellar/beir.git $ cd beir $ pip install -e . ```
+Tested with python versions 3.6 and 3.7 ## :beers: Features - Preprocess your
+own IR dataset or use one of the already-preprocessed 17 benchmark datasets -
+Wide settings included, covers diverse benchmarks useful for both academia and
+industry - Includes well-known retrieval architectures (lexical, dense, sparse
+and reranking-based) - Add and evaluate your own model in a easy framework
+using different state-of-the-art evaluation metrics ## :beers: Quick Example
+For other example codes, please refer to our **[Examples and Tutorials](https:/
+/github.com/beir-cellar/beir/wiki/Examples-and-tutorials)** Wiki page.
+```python from beir import util, LoggingHandler from beir.retrieval import
+models from beir.datasets.data_loader import GenericDataLoader from
+beir.retrieval.evaluation import EvaluateRetrieval from
 beir.retrieval.search.dense import DenseRetrievalExactSearch as DRES import
 logging import pathlib, os #### Just some code to print debug information to
 stdout logging.basicConfig(format='%(asctime)s - %(message)s', datefmt='%Y-%m-
 %d %H:%M:%S', level=logging.INFO, handlers=[LoggingHandler()]) #### /print
 debug information to stdout #### Download scifact.zip dataset and unzip the
 dataset dataset = "scifact" url = "https://public.ukp.informatik.tu-
 darmstadt.de/thakur/BEIR/datasets/{}.zip".format(dataset) out_dir =
@@ -54,35 +58,35 @@
 distilbert-base-tas-b"), batch_size=16) retriever = EvaluateRetrieval(model,
 score_function="dot") # or "cos_sim" for cosine similarity results =
 retriever.retrieve(corpus, queries) #### Evaluate your model with NDCG@k,
 MAP@K, Recall@K and Precision@K where k = [1,3,5,10,100,1000] ndcg, _map,
 recall, precision = retriever.evaluate(qrels, results, retriever.k_values) ```
 ## :beers: Available Datasets Command to generate md5hash using Terminal:
 ``md5sum filename.zip``. You can view all datasets available **[here](https://
-public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/)** or on **
-[HuggingFace](https://huggingface.co/BeIR)**. | Dataset | Website| BEIR-Name |
-Public? | Type | Queries | Corpus | Rel D/Q | Down-load | md5 | | -------- | --
----| ---------| ------- | --------- | ----------- | ---------| ---------| :----
-------: | :------:| | MSMARCO | [Homepage](https://microsoft.github.io/msmarco/
-)| ``msmarco`` | â | ``train``
+public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/)** or on **[Hugging
+Face](https://huggingface.co/BeIR)**. | Dataset | Website| BEIR-Name | Public?
+| Type | Queries | Corpus | Rel D/Q | Down-load | md5 | | -------- | -----| ---
+------| ------- | --------- | ----------- | ---------| ---------| :----------:
+| :------:| | MSMARCO | [Homepage](https://microsoft.github.io/msmarco/)|
+``msmarco`` | â | ``train``
 ``dev``
 ``test``| 6,980 | 8.84M | 1.1 | [Link](https://public.ukp.informatik.tu-
 darmstadt.de/thakur/BEIR/datasets/msmarco.zip) |
 ``444067daf65d982533ea17ebd59501e4`` | | TREC-COVID | [Homepage](https://
 ir.nist.gov/covidSubmit/index.html)| ``trec-covid``| â | ``test``| 50| 171K|
 493.5 | [Link](https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/
 datasets/trec-covid.zip) | ``ce62140cb23feb9becf6270d0d1fe6d1`` | | NFCorpus |
 [Homepage](https://www.cl.uni-heidelberg.de/statnlpgroup/nfcorpus/) |
 ``nfcorpus`` | â |``train``
 ``dev``
 ``test``| 323 | 3.6K | 38.2 | [Link](https://public.ukp.informatik.tu-
 darmstadt.de/thakur/BEIR/datasets/nfcorpus.zip) |
 ``a89dba18a62ef92f7d323ec890a0d38d`` | | BioASQ | [Homepage](http://bioasq.org)
 | ``bioasq``| â | ``train``
-``test`` | 500 | 14.91M | 8.05 | No | [How to Reproduce?](https://github.com/
+``test`` | 500 | 14.91M | 4.7 | No | [How to Reproduce?](https://github.com/
 beir-cellar/beir/blob/main/examples/dataset#2-bioasq) | | NQ | [Homepage]
 (https://ai.google.com/research/NaturalQuestions) | ``nq``| â | ``train``
 ``test``| 3,452 | 2.68M | 1.2 | [Link](https://public.ukp.informatik.tu-
 darmstadt.de/thakur/BEIR/datasets/nq.zip) |
 ``d4d3d2e48787a744b6f6e691ff534307`` | | HotpotQA | [Homepage](https://
 hotpotqa.github.io) | ``hotpotqa``| â |``train``
 ``dev``
@@ -149,15 +153,15 @@
 custom-dataset) ### Models - [Models Available](https://github.com/beir-cellar/
 beir/wiki/Models-available) - [Evaluate your Custom Model](https://github.com/
 beir-cellar/beir/wiki/Evaluate-your-custom-model) ### Metrics - [Metrics
 Available](https://github.com/beir-cellar/beir/wiki/Metrics-available) ###
 Miscellaneous - [BEIR Leaderboard](https://github.com/beir-cellar/beir/wiki/
 Leaderboard) - [Couse Material on IR](https://github.com/beir-cellar/beir/wiki/
 Course-material-on-ir) ## :beers: Disclaimer Similar to Tensorflow [datasets]
-(https://github.com/tensorflow/datasets) or HuggingFace's [datasets](https://
+(https://github.com/tensorflow/datasets) or Hugging Face's [datasets](https://
 github.com/huggingface/datasets) library, we just downloaded and prepared
 public datasets. We only distribute these datasets in a specific format, but we
 do not vouch for their quality or fairness, or claim that you have license to
 use the dataset. It remains the user's responsibility to determine whether you
 as a user have permission to use the dataset under the dataset's license and to
 cite the right owner of the dataset. If you're a dataset owner and wish to
 update any part of it, or do not want your dataset to be included in this
@@ -168,25 +172,32 @@
 Heterogenous Benchmark for Zero-shot Evaluation of Information Retrieval
 Models](https://arxiv.org/abs/2104.08663): ``` @inproceedings{ thakur2021beir,
 title={{BEIR}: A Heterogeneous Benchmark for Zero-shot Evaluation of
 Information Retrieval Models}, author={Nandan Thakur and Nils Reimers and
 Andreas R{\"u}ckl{\'e} and Abhishek Srivastava and Iryna Gurevych}, booktitle=
 {Thirty-fifth Conference on Neural Information Processing Systems Datasets and
 Benchmarks Track (Round 2)}, year={2021}, url={https://openreview.net/
-forum?id=wCu6T5xFjeJ} } ``` The main contributors of this repository are: -
+forum?id=wCu6T5xFjeJ} } ``` If you use any baseline score from the BEIR
+leaderboard, feel free to cite our publication [Resources for Brewing BEIR:
+Reproducible Reference Models and an Official Leaderboard](https://arxiv.org/
+abs/2306.07471) ``` @misc{kamalloo2023resources, title={Resources for Brewing
+BEIR: Reproducible Reference Models and an Official Leaderboard}, author={Ehsan
+Kamalloo and Nandan Thakur and Carlos Lassance and Xueguang Ma and Jheng-Hong
+Yang and Jimmy Lin}, year={2023}, eprint={2306.07471}, archivePrefix={arXiv},
+primaryClass={cs.IR} } ``` The main contributors of this repository are: -
 [Nandan Thakur](https://github.com/Nthakur20), Personal Website: [nandan-
 thakur.com](https://nandan-thakur.com) Contact person: Nandan Thakur,
 [nandant@gmail.com](mailto:nandant@gmail.com) Don't hesitate to send us an e-
 mail or report an issue, if something is broken (and it shouldn't be) or if you
 have further questions. > This repository contains experimental software and is
 published for the sole purpose of giving additional background details on the
 respective publication. ## :beers: Collaboration The BEIR Benchmark has been
 made possible due to a collaborative effort of the following universities and
 organizations: - [UKP Lab, Technical University of Darmstadt](http://
 www.ukp.tu-darmstadt.de/) - [University of Waterloo](https://uwaterloo.ca/) -
-[HuggingFace](https://huggingface.co/) ## :beers: Contributors Thanks go to all
-these wonderful collaborations for their contribution towards the BEIR
+[Hugging Face](https://huggingface.co/) ## :beers: Contributors Thanks go to
+all these wonderful collaborations for their contribution towards the BEIR
 benchmark:
 
 Nandan_Thakur Nils_Reimers  Iryna   Jimmy_Lin   Andreas_RÃ¼cklÃ� Abhishek
                            Gurevych                                Srivastava
```

### Comparing `beir-1.0.1/beir.egg-info/SOURCES.txt` & `beir-2.0.0/beir.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 beir/retrieval/models/sentence_bert.py
 beir/retrieval/models/sparta.py
 beir/retrieval/models/splade.py
 beir/retrieval/models/tldr.py
 beir/retrieval/models/unicoil.py
 beir/retrieval/models/use_qa.py
 beir/retrieval/search/__init__.py
+beir/retrieval/search/base.py
 beir/retrieval/search/dense/__init__.py
 beir/retrieval/search/dense/exact_search.py
 beir/retrieval/search/dense/exact_search_multi_gpu.py
 beir/retrieval/search/dense/faiss_index.py
 beir/retrieval/search/dense/faiss_search.py
 beir/retrieval/search/dense/util.py
 beir/retrieval/search/lexical/__init__.py
```

