# Comparing `tmp/bcqa-1.0.5.tar.gz` & `tmp/bcqa-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcqa-1.0.5.tar", last modified: Thu May 30 18:47:17 2024, max compression
+gzip compressed data, was "bcqa-1.0.6.tar", last modified: Thu May 30 19:07:42 2024, max compression
```

## Comparing `bcqa-1.0.5.tar` & `bcqa-1.0.6.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.499933 bcqa-1.0.5/
--rw-r--r--   0 venky    (100600114) venky    (100600114)     3192 2024-05-30 18:47:17.499933 bcqa-1.0.5/PKG-INFO
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2001 2024-05-30 16:47:11.000000 bcqa-1.0.5/README.md
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.479933 bcqa-1.0.5/bcqa/
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:30:15.000000 bcqa-1.0.5/bcqa/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.483267 bcqa-1.0.5/bcqa/config/
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:46:47.000000 bcqa-1.0.5/bcqa/config/__init__.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)      406 2024-03-12 23:59:30.000000 bcqa-1.0.5/bcqa/config/constants.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.483267 bcqa-1.0.5/bcqa/data/
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:30:31.000000 bcqa-1.0.5/bcqa/data/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.483267 bcqa-1.0.5/bcqa/data/datastructures/
--rw-r--r--   0 venky    (100600114) venky    (100600114)       89 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/data/datastructures/AnnConstants.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)       45 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/data/datastructures/LLmConstants.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/data/datastructures/__init__.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1057 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/data/datastructures/answer.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     6421 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/data/datastructures/dataset.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)      854 2024-05-27 13:02:54.000000 bcqa-1.0.5/bcqa/data/datastructures/evidence.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)      382 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/data/datastructures/question.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)      709 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/data/datastructures/sample.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.486600 bcqa-1.0.5/bcqa/data/loaders/
--rw-r--r--   0 venky    (100600114) venky    (100600114)     3159 2024-05-27 13:02:54.000000 bcqa-1.0.5/bcqa/data/loaders/AmbigQADataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     8834 2024-05-27 13:02:54.000000 bcqa-1.0.5/bcqa/data/loaders/BaseDataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1703 2024-05-27 13:02:54.000000 bcqa-1.0.5/bcqa/data/loaders/DataLoaderFactory.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     3242 2024-05-27 13:02:54.000000 bcqa-1.0.5/bcqa/data/loaders/DprDataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1934 2024-05-27 21:03:57.000000 bcqa-1.0.5/bcqa/data/loaders/FinQADataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/data/loaders/HfDataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2313 2024-05-27 13:02:54.000000 bcqa-1.0.5/bcqa/data/loaders/MusiqueQaDataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2303 2024-05-27 13:02:54.000000 bcqa-1.0.5/bcqa/data/loaders/OTTQADataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     6913 2024-05-27 13:02:54.000000 bcqa-1.0.5/bcqa/data/loaders/ReaderDataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1894 2024-05-27 13:02:54.000000 bcqa-1.0.5/bcqa/data/loaders/RetrieverDataset.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2347 2024-05-27 13:02:54.000000 bcqa-1.0.5/bcqa/data/loaders/StrategyQADataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2345 2024-05-27 13:02:54.000000 bcqa-1.0.5/bcqa/data/loaders/TATQADataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)      569 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/data/loaders/Tokenizer.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2329 2024-05-27 13:02:54.000000 bcqa-1.0.5/bcqa/data/loaders/WikiMultihopQADataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/data/loaders/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.486600 bcqa-1.0.5/bcqa/evaluation/
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/evaluation/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.486600 bcqa-1.0.5/bcqa/losses/
--rw-r--r--   0 venky    (100600114) venky    (100600114)      126 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/losses/BaseLoss.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1613 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/losses/DprNllLoss.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:30:59.000000 bcqa-1.0.5/bcqa/losses/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.486600 bcqa-1.0.5/bcqa/methods/
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:31:06.000000 bcqa-1.0.5/bcqa/methods/__init__.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-13 17:02:58.000000 bcqa-1.0.5/bcqa/methods/utils.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.486600 bcqa-1.0.5/bcqa/metrics/
--rw-r--r--   0 venky    (100600114) venky    (100600114)      596 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/metrics/ExactMatch.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)      624 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/metrics/MetricsBase.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1444 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/metrics/SimilarityMatch.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:31:16.000000 bcqa-1.0.5/bcqa/metrics/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.486600 bcqa-1.0.5/bcqa/re_ranker/
--rw-r--r--   0 venky    (100600114) venky    (100600114)      551 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/re_ranker/CrossEncoder.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1894 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/re_ranker/ReRanker.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:31:29.000000 bcqa-1.0.5/bcqa/re_ranker/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.489933 bcqa-1.0.5/bcqa/retriever/
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1407 2024-03-12 23:59:03.000000 bcqa-1.0.5/bcqa/retriever/ANCE.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2954 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/retriever/Baleen.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)      343 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/retriever/BaseRetriever.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.489933 bcqa-1.0.5/bcqa/retriever/ColBERT/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:11.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.489933 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/
--rw-------   0 venky    (100600114) venky    (100600114)      174 2024-01-15 22:15:14.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.489933 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/data/
--rw-------   0 venky    (100600114) venky    (100600114)       97 2024-01-15 22:15:16.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/data/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     3264 2024-05-27 16:19:05.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/data/collection.py
--rw-------   0 venky    (100600114) venky    (100600114)      421 2024-01-15 22:15:16.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/data/dataset.py
--rw-------   0 venky    (100600114) venky    (100600114)     2788 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/data/examples.py
--rw-------   0 venky    (100600114) venky    (100600114)     4429 2024-05-27 16:20:51.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/data/queries.py
--rw-------   0 venky    (100600114) venky    (100600114)     2846 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/data/ranking.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.489933 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/evaluation/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:12.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/evaluation/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)      973 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/evaluation/load_model.py
--rw-------   0 venky    (100600114) venky    (100600114)     6528 2024-05-27 16:20:37.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/evaluation/loaders.py
--rw-------   0 venky    (100600114) venky    (100600114)     4322 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/evaluation/metrics.py
--rw-------   0 venky    (100600114) venky    (100600114)      286 2024-01-15 22:15:14.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/index.py
--rw-------   0 venky    (100600114) venky    (100600114)    21339 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/index_updater.py
--rw-------   0 venky    (100600114) venky    (100600114)     3236 2024-05-27 16:23:46.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexer.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.493267 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:12.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.493267 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/codecs/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:13.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/codecs/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)    10982 2024-05-27 17:42:56.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual.py
--rw-------   0 venky    (100600114) venky    (100600114)     4931 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual_embeddings.py
--rw-------   0 venky    (100600114) venky    (100600114)     1223 2024-05-27 18:21:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual_embeddings_strided.py
--rw-------   0 venky    (100600114) venky    (100600114)     1866 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/collection_encoder.py
--rw-------   0 venky    (100600114) venky    (100600114)    21552 2024-05-27 17:43:15.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/collection_indexer.py
--rw-------   0 venky    (100600114) venky    (100600114)      878 2024-01-15 22:15:12.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/index_manager.py
--rw-------   0 venky    (100600114) venky    (100600114)     2936 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/index_saver.py
--rw-------   0 venky    (100600114) venky    (100600114)     1995 2024-01-15 22:15:13.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/loaders.py
--rw-------   0 venky    (100600114) venky    (100600114)     1961 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/utils.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.493267 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/infra/
--rw-------   0 venky    (100600114) venky    (100600114)       40 2024-01-15 22:15:15.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/infra/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.493267 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/infra/config/
--rw-------   0 venky    (100600114) venky    (100600114)       45 2024-01-15 22:15:15.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/infra/config/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     4121 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/infra/config/base_config.py
--rw-------   0 venky    (100600114) venky    (100600114)      364 2024-01-15 22:15:15.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/infra/config/config.py
--rw-------   0 venky    (100600114) venky    (100600114)     2430 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/infra/config/core_config.py
--rw-------   0 venky    (100600114) venky    (100600114)     4393 2024-05-27 16:55:49.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/infra/config/settings.py
--rw-------   0 venky    (100600114) venky    (100600114)     4683 2024-05-27 16:24:47.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/infra/launcher.py
--rw-------   0 venky    (100600114) venky    (100600114)      932 2024-01-15 22:15:15.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/infra/provenance.py
--rw-------   0 venky    (100600114) venky    (100600114)     2692 2024-05-27 16:56:04.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/infra/run.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.493267 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:18.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     3977 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/base_colbert.py
--rw-------   0 venky    (100600114) venky    (100600114)     5513 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/checkpoint.py
--rw-------   0 venky    (100600114) venky    (100600114)     7644 2024-05-27 16:20:37.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/colbert.py
--rw-------   0 venky    (100600114) venky    (100600114)     5170 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/hf_colbert.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.493267 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/reranker/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:18.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/reranker/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     1272 2024-01-15 22:15:18.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/reranker/electra.py
--rw-------   0 venky    (100600114) venky    (100600114)      608 2024-01-15 22:15:18.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/reranker/tokenizer.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.496600 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/tokenization/
--rw-------   0 venky    (100600114) venky    (100600114)      244 2024-05-27 16:20:16.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/tokenization/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     2579 2024-05-27 16:20:16.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/tokenization/doc_tokenization.py
--rw-------   0 venky    (100600114) venky    (100600114)     5161 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/tokenization/query_tokenization.py
--rw-------   0 venky    (100600114) venky    (100600114)     2054 2024-01-15 22:15:17.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/tokenization/utils.py
--rw-------   0 venky    (100600114) venky    (100600114)      471 2024-01-18 20:49:04.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/parameters.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.496600 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/ranking/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:16.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/ranking/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.496600 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/search/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:16:50.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/search/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     2111 2024-05-27 18:24:43.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/search/candidate_generation.py
--rw-------   0 venky    (100600114) venky    (100600114)     3152 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/search/index_loader.py
--rw-------   0 venky    (100600114) venky    (100600114)     8853 2024-05-27 18:10:29.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/search/index_storage.py
--rw-------   0 venky    (100600114) venky    (100600114)     7076 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/search/strided_tensor.py
--rw-------   0 venky    (100600114) venky    (100600114)     4181 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/search/strided_tensor_core.py
--rw-------   0 venky    (100600114) venky    (100600114)     5310 2024-05-27 18:20:23.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/searcher.py
--rw-------   0 venky    (100600114) venky    (100600114)     1329 2024-05-27 16:19:05.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/trainer.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.496600 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/training/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:16:49.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/training/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     2072 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/training/eager_batcher.py
--rw-------   0 venky    (100600114) venky    (100600114)     2768 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/training/lazy_batcher.py
--rw-------   0 venky    (100600114) venky    (100600114)     2736 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/training/rerank_batcher.py
--rw-------   0 venky    (100600114) venky    (100600114)     5954 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/training/training.py
--rw-------   0 venky    (100600114) venky    (100600114)     1907 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/training/utils.py
--rw-------   0 venky    (100600114) venky    (100600114)     1568 2024-05-27 16:18:37.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/server.py
--rw-------   0 venky    (100600114) venky    (100600114)     1043 2024-01-15 22:16:52.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/setup.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.496600 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:09.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.496600 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/evaluate/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:09.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/evaluate/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     2955 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/evaluate/annotate_EM.py
--rw-------   0 venky    (100600114) venky    (100600114)     2531 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/evaluate/annotate_EM_helpers.py
--rw-------   0 venky    (100600114) venky    (100600114)     2604 2024-01-15 22:15:09.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/evaluate/evaluate_lotte_rankings.py
--rw-------   0 venky    (100600114) venky    (100600114)     4224 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/evaluate/msmarco_passages.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.499933 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/preprocess/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:09.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/preprocess/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     4808 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/preprocess/docs2passages.py
--rw-------   0 venky    (100600114) venky    (100600114)     2243 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/preprocess/queries_split.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.499933 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/rankings/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:10.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/rankings/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     1386 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/rankings/dev_subsample.py
--rw-------   0 venky    (100600114) venky    (100600114)     1658 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/rankings/merge.py
--rw-------   0 venky    (100600114) venky    (100600114)     1334 2024-01-15 22:15:10.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/rankings/split_by_offset.py
--rw-------   0 venky    (100600114) venky    (100600114)     1754 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/rankings/split_by_queries.py
--rw-------   0 venky    (100600114) venky    (100600114)     1777 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/rankings/tune.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.499933 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/supervision/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:09.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/supervision/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     3942 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/supervision/self_training.py
--rw-------   0 venky    (100600114) venky    (100600114)     5086 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/supervision/triples.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.499933 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/utils/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:10.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/utils/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     7071 2024-01-15 22:15:10.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/utils/dpr.py
--rw-------   0 venky    (100600114) venky    (100600114)      744 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/utils/qa_loaders.py
--rw-------   0 venky    (100600114) venky    (100600114)     1949 2024-05-27 16:24:22.000000 bcqa-1.0.5/bcqa/retriever/ColBERT/utility/utils/save_metadata.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)      307 2024-01-07 21:56:32.000000 bcqa-1.0.5/bcqa/retriever/Contriever.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     7601 2024-04-18 15:41:50.000000 bcqa-1.0.5/bcqa/retriever/DenseFullSearch.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     8927 2024-03-12 23:59:03.000000 bcqa-1.0.5/bcqa/retriever/HfRetriever.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     5071 2024-05-27 17:14:43.000000 bcqa-1.0.5/bcqa/retriever/TCTColBERT.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:31:38.000000 bcqa-1.0.5/bcqa/retriever/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:47:17.499933 bcqa-1.0.5/bcqa.egg-info/
--rw-r--r--   0 venky    (100600114) venky    (100600114)     3192 2024-05-30 18:47:17.000000 bcqa-1.0.5/bcqa.egg-info/PKG-INFO
--rw-r--r--   0 venky    (100600114) venky    (100600114)     6368 2024-05-30 18:47:17.000000 bcqa-1.0.5/bcqa.egg-info/SOURCES.txt
--rw-r--r--   0 venky    (100600114) venky    (100600114)        1 2024-05-30 18:47:17.000000 bcqa-1.0.5/bcqa.egg-info/dependency_links.txt
--rw-r--r--   0 venky    (100600114) venky    (100600114)      194 2024-05-30 18:47:17.000000 bcqa-1.0.5/bcqa.egg-info/requires.txt
--rw-r--r--   0 venky    (100600114) venky    (100600114)        5 2024-05-30 18:47:17.000000 bcqa-1.0.5/bcqa.egg-info/top_level.txt
--rw-r--r--   0 venky    (100600114) venky    (100600114)       38 2024-05-30 18:47:17.499933 bcqa-1.0.5/setup.cfg
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1430 2024-05-30 18:47:02.000000 bcqa-1.0.5/setup.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.019103 bcqa-1.0.6/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     3192 2024-05-30 19:07:42.019103 bcqa-1.0.6/PKG-INFO
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2001 2024-05-30 16:47:11.000000 bcqa-1.0.6/README.md
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:41.999103 bcqa-1.0.6/bcqa/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:30:15.000000 bcqa-1.0.6/bcqa/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.002437 bcqa-1.0.6/bcqa/config/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:46:47.000000 bcqa-1.0.6/bcqa/config/__init__.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      406 2024-03-12 23:59:30.000000 bcqa-1.0.6/bcqa/config/constants.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.002437 bcqa-1.0.6/bcqa/data/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:30:31.000000 bcqa-1.0.6/bcqa/data/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.002437 bcqa-1.0.6/bcqa/data/datastructures/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)       89 2024-01-07 21:56:32.000000 bcqa-1.0.6/bcqa/data/datastructures/AnnConstants.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)       45 2024-01-07 21:56:32.000000 bcqa-1.0.6/bcqa/data/datastructures/LLmConstants.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-07 21:56:32.000000 bcqa-1.0.6/bcqa/data/datastructures/__init__.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1057 2024-01-07 21:56:32.000000 bcqa-1.0.6/bcqa/data/datastructures/answer.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     6421 2024-01-07 21:56:32.000000 bcqa-1.0.6/bcqa/data/datastructures/dataset.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      859 2024-05-30 19:02:45.000000 bcqa-1.0.6/bcqa/data/datastructures/evidence.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      382 2024-01-07 21:56:32.000000 bcqa-1.0.6/bcqa/data/datastructures/question.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      724 2024-05-30 19:02:56.000000 bcqa-1.0.6/bcqa/data/datastructures/sample.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.005770 bcqa-1.0.6/bcqa/data/loaders/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     3189 2024-05-30 19:02:56.000000 bcqa-1.0.6/bcqa/data/loaders/AmbigQADataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     8869 2024-05-30 19:02:56.000000 bcqa-1.0.6/bcqa/data/loaders/BaseDataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1743 2024-05-30 19:02:56.000000 bcqa-1.0.6/bcqa/data/loaders/DataLoaderFactory.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     3287 2024-05-30 19:03:05.000000 bcqa-1.0.6/bcqa/data/loaders/DprDataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1969 2024-05-30 19:02:56.000000 bcqa-1.0.6/bcqa/data/loaders/FinQADataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-07 21:56:32.000000 bcqa-1.0.6/bcqa/data/loaders/HfDataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2348 2024-05-30 19:02:56.000000 bcqa-1.0.6/bcqa/data/loaders/MusiqueQaDataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2338 2024-05-30 19:02:56.000000 bcqa-1.0.6/bcqa/data/loaders/OTTQADataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     6938 2024-05-30 19:02:56.000000 bcqa-1.0.6/bcqa/data/loaders/ReaderDataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1924 2024-05-30 19:02:14.000000 bcqa-1.0.6/bcqa/data/loaders/RetrieverDataset.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2382 2024-05-30 19:02:56.000000 bcqa-1.0.6/bcqa/data/loaders/StrategyQADataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2385 2024-05-30 19:02:56.000000 bcqa-1.0.6/bcqa/data/loaders/TATQADataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      569 2024-01-07 21:56:32.000000 bcqa-1.0.6/bcqa/data/loaders/Tokenizer.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2364 2024-05-30 19:02:56.000000 bcqa-1.0.6/bcqa/data/loaders/WikiMultihopQADataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-07 21:56:32.000000 bcqa-1.0.6/bcqa/data/loaders/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.005770 bcqa-1.0.6/bcqa/evaluation/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-07 21:56:32.000000 bcqa-1.0.6/bcqa/evaluation/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.005770 bcqa-1.0.6/bcqa/losses/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      126 2024-01-07 21:56:32.000000 bcqa-1.0.6/bcqa/losses/BaseLoss.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1613 2024-01-07 21:56:32.000000 bcqa-1.0.6/bcqa/losses/DprNllLoss.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:30:59.000000 bcqa-1.0.6/bcqa/losses/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.005770 bcqa-1.0.6/bcqa/methods/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:31:06.000000 bcqa-1.0.6/bcqa/methods/__init__.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-13 17:02:58.000000 bcqa-1.0.6/bcqa/methods/utils.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.009103 bcqa-1.0.6/bcqa/metrics/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      601 2024-05-30 19:05:24.000000 bcqa-1.0.6/bcqa/metrics/ExactMatch.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      624 2024-01-07 21:56:32.000000 bcqa-1.0.6/bcqa/metrics/MetricsBase.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1449 2024-05-30 19:05:30.000000 bcqa-1.0.6/bcqa/metrics/SimilarityMatch.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:31:16.000000 bcqa-1.0.6/bcqa/metrics/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.009103 bcqa-1.0.6/bcqa/re_ranker/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      551 2024-01-07 21:56:32.000000 bcqa-1.0.6/bcqa/re_ranker/CrossEncoder.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1904 2024-05-30 19:02:56.000000 bcqa-1.0.6/bcqa/re_ranker/ReRanker.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:31:29.000000 bcqa-1.0.6/bcqa/re_ranker/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.009103 bcqa-1.0.6/bcqa/retriever/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1432 2024-05-30 19:06:03.000000 bcqa-1.0.6/bcqa/retriever/ANCE.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2969 2024-05-30 19:02:56.000000 bcqa-1.0.6/bcqa/retriever/Baleen.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      343 2024-01-07 21:56:32.000000 bcqa-1.0.6/bcqa/retriever/BaseRetriever.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.009103 bcqa-1.0.6/bcqa/retriever/ColBERT/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:11.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.012437 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/
+-rw-------   0 venky    (100600114) venky    (100600114)      174 2024-01-15 22:15:14.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.012437 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/data/
+-rw-------   0 venky    (100600114) venky    (100600114)       97 2024-01-15 22:15:16.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/data/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     3264 2024-05-27 16:19:05.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/data/collection.py
+-rw-------   0 venky    (100600114) venky    (100600114)      421 2024-01-15 22:15:16.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/data/dataset.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2788 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/data/examples.py
+-rw-------   0 venky    (100600114) venky    (100600114)     4429 2024-05-27 16:20:51.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/data/queries.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2846 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/data/ranking.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.012437 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/evaluation/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:12.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/evaluation/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)      973 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/evaluation/load_model.py
+-rw-------   0 venky    (100600114) venky    (100600114)     6528 2024-05-27 16:20:37.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/evaluation/loaders.py
+-rw-------   0 venky    (100600114) venky    (100600114)     4322 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/evaluation/metrics.py
+-rw-------   0 venky    (100600114) venky    (100600114)      286 2024-01-15 22:15:14.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/index.py
+-rw-------   0 venky    (100600114) venky    (100600114)    21339 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/index_updater.py
+-rw-------   0 venky    (100600114) venky    (100600114)     3236 2024-05-27 16:23:46.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexer.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.012437 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:12.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.012437 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/codecs/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:13.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/codecs/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)    10982 2024-05-27 17:42:56.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual.py
+-rw-------   0 venky    (100600114) venky    (100600114)     4931 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual_embeddings.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1223 2024-05-27 18:21:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual_embeddings_strided.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1866 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/collection_encoder.py
+-rw-------   0 venky    (100600114) venky    (100600114)    21552 2024-05-27 17:43:15.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/collection_indexer.py
+-rw-------   0 venky    (100600114) venky    (100600114)      878 2024-01-15 22:15:12.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/index_manager.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2936 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/index_saver.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1995 2024-01-15 22:15:13.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/loaders.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1961 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/utils.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.012437 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/infra/
+-rw-------   0 venky    (100600114) venky    (100600114)       40 2024-01-15 22:15:15.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/infra/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.015770 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/infra/config/
+-rw-------   0 venky    (100600114) venky    (100600114)       45 2024-01-15 22:15:15.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/infra/config/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     4121 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/infra/config/base_config.py
+-rw-------   0 venky    (100600114) venky    (100600114)      364 2024-01-15 22:15:15.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/infra/config/config.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2430 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/infra/config/core_config.py
+-rw-------   0 venky    (100600114) venky    (100600114)     4393 2024-05-27 16:55:49.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/infra/config/settings.py
+-rw-------   0 venky    (100600114) venky    (100600114)     4683 2024-05-27 16:24:47.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/infra/launcher.py
+-rw-------   0 venky    (100600114) venky    (100600114)      932 2024-01-15 22:15:15.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/infra/provenance.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2692 2024-05-27 16:56:04.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/infra/run.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.015770 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:18.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     3977 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/base_colbert.py
+-rw-------   0 venky    (100600114) venky    (100600114)     5513 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/checkpoint.py
+-rw-------   0 venky    (100600114) venky    (100600114)     7644 2024-05-27 16:20:37.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/colbert.py
+-rw-------   0 venky    (100600114) venky    (100600114)     5170 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/hf_colbert.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.015770 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/reranker/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:18.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/reranker/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1272 2024-01-15 22:15:18.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/reranker/electra.py
+-rw-------   0 venky    (100600114) venky    (100600114)      608 2024-01-15 22:15:18.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/reranker/tokenizer.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.015770 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/tokenization/
+-rw-------   0 venky    (100600114) venky    (100600114)      244 2024-05-27 16:20:16.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/tokenization/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2579 2024-05-27 16:20:16.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/tokenization/doc_tokenization.py
+-rw-------   0 venky    (100600114) venky    (100600114)     5161 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/tokenization/query_tokenization.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2054 2024-01-15 22:15:17.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/tokenization/utils.py
+-rw-------   0 venky    (100600114) venky    (100600114)      471 2024-01-18 20:49:04.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/parameters.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.015770 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/ranking/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:16.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/ranking/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.015770 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/search/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:16:50.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/search/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2111 2024-05-27 18:24:43.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/search/candidate_generation.py
+-rw-------   0 venky    (100600114) venky    (100600114)     3152 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/search/index_loader.py
+-rw-------   0 venky    (100600114) venky    (100600114)     8853 2024-05-27 18:10:29.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/search/index_storage.py
+-rw-------   0 venky    (100600114) venky    (100600114)     7076 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/search/strided_tensor.py
+-rw-------   0 venky    (100600114) venky    (100600114)     4181 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/search/strided_tensor_core.py
+-rw-------   0 venky    (100600114) venky    (100600114)     5310 2024-05-27 18:20:23.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/searcher.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1329 2024-05-27 16:19:05.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/trainer.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.019103 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/training/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:16:49.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/training/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2072 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/training/eager_batcher.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2768 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/training/lazy_batcher.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2736 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/training/rerank_batcher.py
+-rw-------   0 venky    (100600114) venky    (100600114)     5954 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/training/training.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1907 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/training/utils.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1568 2024-05-27 16:18:37.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/server.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1043 2024-01-15 22:16:52.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/setup.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.019103 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:09.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.019103 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/evaluate/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:09.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/evaluate/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2955 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/evaluate/annotate_EM.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2531 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/evaluate/annotate_EM_helpers.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2604 2024-01-15 22:15:09.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/evaluate/evaluate_lotte_rankings.py
+-rw-------   0 venky    (100600114) venky    (100600114)     4224 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/evaluate/msmarco_passages.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.019103 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/preprocess/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:09.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/preprocess/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     4808 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/preprocess/docs2passages.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2243 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/preprocess/queries_split.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.019103 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/rankings/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:10.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/rankings/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1386 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/rankings/dev_subsample.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1658 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/rankings/merge.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1334 2024-01-15 22:15:10.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/rankings/split_by_offset.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1754 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/rankings/split_by_queries.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1777 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/rankings/tune.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.019103 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/supervision/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:09.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/supervision/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     3942 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/supervision/self_training.py
+-rw-------   0 venky    (100600114) venky    (100600114)     5086 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/supervision/triples.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.019103 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/utils/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:10.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/utils/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     7071 2024-01-15 22:15:10.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/utils/dpr.py
+-rw-------   0 venky    (100600114) venky    (100600114)      744 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/utils/qa_loaders.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1949 2024-05-27 16:24:22.000000 bcqa-1.0.6/bcqa/retriever/ColBERT/utility/utils/save_metadata.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      317 2024-05-30 19:06:38.000000 bcqa-1.0.6/bcqa/retriever/Contriever.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     7626 2024-05-30 19:06:48.000000 bcqa-1.0.6/bcqa/retriever/DenseFullSearch.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     8952 2024-05-30 19:07:00.000000 bcqa-1.0.6/bcqa/retriever/HfRetriever.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     5096 2024-05-30 19:07:14.000000 bcqa-1.0.6/bcqa/retriever/TCTColBERT.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:31:38.000000 bcqa-1.0.6/bcqa/retriever/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:07:42.019103 bcqa-1.0.6/bcqa.egg-info/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     3192 2024-05-30 19:07:41.000000 bcqa-1.0.6/bcqa.egg-info/PKG-INFO
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     6368 2024-05-30 19:07:41.000000 bcqa-1.0.6/bcqa.egg-info/SOURCES.txt
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        1 2024-05-30 19:07:41.000000 bcqa-1.0.6/bcqa.egg-info/dependency_links.txt
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      194 2024-05-30 19:07:41.000000 bcqa-1.0.6/bcqa.egg-info/requires.txt
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        5 2024-05-30 19:07:41.000000 bcqa-1.0.6/bcqa.egg-info/top_level.txt
+-rw-r--r--   0 venky    (100600114) venky    (100600114)       38 2024-05-30 19:07:42.022437 bcqa-1.0.6/setup.cfg
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1430 2024-05-30 19:07:34.000000 bcqa-1.0.6/setup.py
```

### Comparing `bcqa-1.0.5/PKG-INFO` & `bcqa-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcqa
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Benchmark for Complex Heterogeneous Question answering
 Home-page: https://github.com/VenkteshV/BCQA
 Download-URL: 
 Author: Venktesh V, Deepali Prabhu
 Author-email: venkyviswa12@gmail.com
 License: Apache License 2.0
 Keywords: Information Retrieval Transformer Networks BERT PyTorch Complex Question Answering IR NLP deep learning
```

### Comparing `bcqa-1.0.5/README.md` & `bcqa-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/data/datastructures/answer.py` & `bcqa-1.0.6/bcqa/data/datastructures/answer.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/data/datastructures/dataset.py` & `bcqa-1.0.6/bcqa/data/datastructures/dataset.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/data/datastructures/evidence.py` & `bcqa-1.0.6/bcqa/data/datastructures/evidence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 
 import pandas as pd
 
-from config.constants import Separators
+from bcqa.config.constants import Separators
 
 
 class Evidence:
     def __init__(self, text: str, idx=None, title: str = None):
         self._text = text
         self._idx = idx
         self._title = title
```

### Comparing `bcqa-1.0.5/bcqa/data/datastructures/sample.py` & `bcqa-1.0.6/bcqa/data/datastructures/sample.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 
 from typing import Optional
 
-from data.datastructures.answer import Answer, AmbigNQAnswer
-from data.datastructures.evidence import Evidence
-from data.datastructures.question import Question
+from bcqa.data.datastructures.answer import Answer, AmbigNQAnswer
+from bcqa.data.datastructures.evidence import Evidence
+from bcqa.data.datastructures.question import Question
 
 
 class Sample:
     def __init__(self, idx, question: Question, answer: Answer, evidences: Optional[Evidence] = None):
         self.question = question
         self.evidences = evidences
         self.answer = answer
```

### Comparing `bcqa-1.0.5/bcqa/data/loaders/AmbigQADataLoader.py` & `bcqa-1.0.6/bcqa/data/loaders/AmbigQADataLoader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from config.constants import Split
-from data.datastructures.answer import AmbigNQAnswer, Answer
-from data.datastructures.question import Question
-from data.datastructures.evidence import Evidence
-from data.datastructures.sample import AmbigNQSample
-from data.loaders.BaseDataLoader import GenericDataLoader
+from bcqa.config.constants import Split
+from bcqa.data.datastructures.answer import AmbigNQAnswer, Answer
+from bcqa.data.datastructures.question import Question
+from bcqa.data.datastructures.evidence import Evidence
+from bcqa.data.datastructures.sample import AmbigNQSample
+from bcqa.data.loaders.BaseDataLoader import GenericDataLoader
 import tqdm
 
 class AmbigQADataLoader(GenericDataLoader):
     def __init__(
         self,
         dataset: str,
         tokenizer="bert-base-uncased",
```

### Comparing `bcqa-1.0.5/bcqa/data/loaders/BaseDataLoader.py` & `bcqa-1.0.6/bcqa/data/loaders/BaseDataLoader.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 import os
 from typing import List
 import zipfile
 
 from torch.utils.data import DataLoader, RandomSampler, SequentialSampler
 from tqdm import tqdm
 
-from config.constants import DataTypes, Separators, Split
-from data.datastructures.answer import Answer
-from data.datastructures.dataset import PassageDataset, QADataset
-from data.datastructures.evidence import Evidence, TableEvidence
-from data.datastructures.question import Question
-from data.datastructures.sample import Sample
-from data.loaders.Tokenizer import Tokenizer
+from bcqa.config.constants import DataTypes, Separators, Split
+from bcqa.data.datastructures.answer import Answer
+from bcqa.data.datastructures.dataset import PassageDataset, QADataset
+from bcqa.data.datastructures.evidence import Evidence, TableEvidence
+from bcqa.data.datastructures.question import Question
+from bcqa.data.datastructures.sample import Sample
+from bcqa.data.loaders.Tokenizer import Tokenizer
 
 
 class GenericDataLoader(DataLoader):
     def __init__(
         self,
         dataset: str,
         tokenizer: str = "bert-base-uncased",
```

### Comparing `bcqa-1.0.5/bcqa/data/loaders/DataLoaderFactory.py` & `bcqa-1.0.6/bcqa/data/loaders/DataLoaderFactory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from config.constants import Dataset, Split
-from data.loaders.AmbigQADataLoader import AmbigQADataLoader
-from data.loaders.FinQADataLoader import FinQADataLoader
-from data.loaders.MusiqueQaDataLoader import MusiqueQADataLoader
+from bcqa.config.constants import Dataset, Split
+from bcqa.data.loaders.AmbigQADataLoader import AmbigQADataLoader
+from bcqa.data.loaders.FinQADataLoader import FinQADataLoader
+from bcqa.data.loaders.MusiqueQaDataLoader import MusiqueQADataLoader
 
-from data.loaders.OTTQADataLoader import OTTQADataLoader
-from data.loaders.TATQADataLoader import TATQADataLoader
-from data.loaders.WikiMultihopQADataLoader import WikiMultihopQADataLoader
-from data.loaders.StrategyQADataLoader import StrategyQADataLoader
+from bcqa.data.loaders.OTTQADataLoader import OTTQADataLoader
+from bcqa.data.loaders.TATQADataLoader import TATQADataLoader
+from bcqa.data.loaders.WikiMultihopQADataLoader import WikiMultihopQADataLoader
+from bcqa.data.loaders.StrategyQADataLoader import StrategyQADataLoader
 
 
 
 class DataLoaderFactory:
     def __int__(self):
         pass
```

### Comparing `bcqa-1.0.5/bcqa/data/loaders/DprDataLoader.py` & `bcqa-1.0.6/bcqa/data/loaders/DprDataLoader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
 import numpy as np
 import random
 import uuid
-from config.constants import Split
-from data.datastructures.answer import AmbigNQAnswer
-from data.datastructures.dataset import DprDataset
-from data.datastructures.question import Question
-from data.datastructures.evidence import Evidence
+from bcqa.config.constants import Split
+from bcqa.data.datastructures.answer import AmbigNQAnswer
+from bcqa.data.datastructures.dataset import DprDataset
+from bcqa.data.datastructures.question import Question
+from bcqa.data.datastructures.evidence import Evidence
 
-from data.datastructures.sample import Sample, AmbigNQSample
-from data.loaders.Tokenizer import Tokenizer
-from data.datastructures.hyperparameters.dpr import DenseHyperParams
+from bcqa.data.datastructures.sample import Sample, AmbigNQSample
+from bcqa.data.loaders.Tokenizer import Tokenizer
+from bcqa.data.datastructures.hyperparameters.dpr import DenseHyperParams
 
-from data.loaders.BaseDataLoader import GenericDataLoader
+from bcqa.data.loaders.BaseDataLoader import GenericDataLoader
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class DprDataLoader(GenericDataLoader):
     def __init__(self, dataset: str, tokenizer="bert-base-uncased", config_path='test_config.ini', config=None,
```

### Comparing `bcqa-1.0.5/bcqa/data/loaders/FinQADataLoader.py` & `bcqa-1.0.6/bcqa/data/loaders/FinQADataLoader.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import os
-from config.constants import Split
-from data.datastructures.answer import Answer
-from data.datastructures.dataset import DprDataset
-from data.datastructures.evidence import Evidence, TableEvidence
-from data.datastructures.question import Question
-from data.datastructures.sample import Sample
-from data.loaders.BaseDataLoader import GenericDataLoader
+from bcqa.config.constants import Split
+from bcqa.data.datastructures.answer import Answer
+from bcqa.data.datastructures.dataset import DprDataset
+from bcqa.data.datastructures.evidence import Evidence, TableEvidence
+from bcqa.data.datastructures.question import Question
+from bcqa.data.datastructures.sample import Sample
+from bcqa.data.loaders.BaseDataLoader import GenericDataLoader
 
 
 class FinQADataLoader(GenericDataLoader):
     def __init__(self, dataset: str, tokenizer="bert-base-uncased", config_path='test_config.ini', split=Split.TRAIN,
                  batch_size=None, corpus=None):
         super().__init__(dataset, tokenizer, config_path, split, batch_size)
```

### Comparing `bcqa-1.0.5/bcqa/data/loaders/MusiqueQaDataLoader.py` & `bcqa-1.0.6/bcqa/data/loaders/WikiMultihopQADataLoader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 import json
 import os
 import tqdm
-from config.constants import Split
-from data.datastructures.answer import Answer
-from data.datastructures.dataset import DprDataset
-from data.datastructures.evidence import Evidence
-from data.datastructures.question import Question
-from data.datastructures.sample import Sample
-from data.loaders.BaseDataLoader import GenericDataLoader
+from typing import List
+from bcqa.config.constants import Split
+from bcqa.data.datastructures.answer import Answer
+from bcqa.data.datastructures.dataset import DprDataset
+from bcqa.data.datastructures.evidence import Evidence
+from bcqa.data.datastructures.question import Question
+from bcqa.data.datastructures.sample import Sample
+from bcqa.data.loaders.BaseDataLoader import GenericDataLoader
 
 
-class MusiqueQADataLoader(GenericDataLoader):
+class WikiMultihopQADataLoader(GenericDataLoader):
     def __init__(self, dataset: str, tokenizer="bert-base-uncased", config_path='test_config.ini', split=Split.TRAIN,
                  batch_size=None, corpus=None):
         self.corpus = corpus
         self.titles = [self.corpus[idx].title().split(" - ")[0] for idx,_ in enumerate(self.corpus)]
         print(self.titles[100],self.corpus[100].title())
         super().__init__(dataset, tokenizer, config_path, split, batch_size)
 
 
     def load_raw_dataset(self, split=Split.TRAIN):
         dataset = self.load_json(split)
         print(len(dataset))
-        for  query_index, data in enumerate(tqdm.tqdm(dataset)):
-            if len(data["paragraphs"]) == 0:
-                data["paragraphs"] = ['some random title', ['some random stuff']]
-            for evidence_set in data["paragraphs"]:
-                title = evidence_set["title"]
+        for  query_index, data in enumerate(tqdm.tqdm(dataset[:1200])):
+            if len(data["context"]) == 0:
+                data["context"] = ['some random title', ['some random stuff']]
+            for evidence_set in data["context"]:
+                title = evidence_set[0]
                 #for evidence in evidence_set[1]:
-                evidence = evidence_set["paragraph_text"]
+                evidence = " ".join(evidence_set[1])
                 #print(list(self.titles).index(title.split(" - ")[0]))
                 self.raw_data.append(
-                    Sample(query_index, Question(data["question"],idx=data["id"]), Answer(data["answer"]),
+                    Sample(query_index, Question(data["question"],idx=data["_id"]), Answer(data["answer"]),
                             Evidence(text=evidence, 
                                     idx=list(self.titles).index(title.split(" - ")[0]),title=title)
                 ))
 
-
     def load_tokenized(self):
         if self.tokenized_path and os.path.exists(self.tokenized_path):
             self.logger.info("Loading DPR data from {}".format(self.tokenized_path))
             with open(self.tokenized_path, "r") as f:
                 ip_ids, ip_attention, evidence_ids, evidence_attention = json.load(f)
         else:
             ip_ids, ip_attention = self.tokenize_questions()
```

### Comparing `bcqa-1.0.5/bcqa/data/loaders/OTTQADataLoader.py` & `bcqa-1.0.6/bcqa/data/loaders/OTTQADataLoader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 import os
 
 from tqdm import tqdm
-from config.constants import Split
-from data.datastructures.answer import Answer
-from data.datastructures.dataset import DprDataset
-from data.datastructures.evidence import Evidence, TableEvidence
-from data.datastructures.question import Question
-from data.datastructures.sample import Sample
-from data.loaders.BaseDataLoader import GenericDataLoader
+from bcqa.config.constants import Split
+from bcqa.data.datastructures.answer import Answer
+from bcqa.data.datastructures.dataset import DprDataset
+from bcqa.data.datastructures.evidence import Evidence, TableEvidence
+from bcqa.data.datastructures.question import Question
+from bcqa.data.datastructures.sample import Sample
+from bcqa.data.loaders.BaseDataLoader import GenericDataLoader
 
 
 class OTTQADataLoader(GenericDataLoader):
     def __init__(self, dataset: str, tokenizer="bert-base-uncased", config_path='test_config.ini', split=Split.TRAIN,
                  batch_size=None, corpus = None):
         super().__init__(dataset, tokenizer, config_path, split, batch_size)
```

### Comparing `bcqa-1.0.5/bcqa/data/loaders/ReaderDataLoader.py` & `bcqa-1.0.6/bcqa/data/loaders/ReaderDataLoader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from collections import defaultdict
 import configparser
 import json
 
 import tqdm
-from config.constants import Split
-from data.datastructures.dataset import ReaderDataset
-from data.loaders.BaseDataLoader import PassageDataLoader
-from data.loaders.DataLoaderFactory import DataLoaderFactory
-from data.loaders.Tokenizer import Tokenizer
+from bcqa.config.constants import Split
+from bcqa.data.datastructures.dataset import ReaderDataset
+from bcqa.data.loaders.BaseDataLoader import PassageDataLoader
+from bcqa.data.loaders.DataLoaderFactory import DataLoaderFactory
+from bcqa.data.loaders.Tokenizer import Tokenizer
 from torch.utils.data import RandomSampler, SequentialSampler
 
 
 class ReaderDataLoader(DataLoaderFactory):
     def __init__(self, dataset:str,passage_dataset:str,config_path,split:Split, batch_size=32,tokenizer="bert-base-uncased"):
         self.split = split
         self.config = configparser.ConfigParser()
```

### Comparing `bcqa-1.0.5/bcqa/data/loaders/RetrieverDataset.py` & `bcqa-1.0.6/bcqa/data/loaders/RetrieverDataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import configparser
 from typing import Dict, List
 
-from config.constants import Split
-from data.datastructures.evidence import Evidence
-from data.datastructures.question import Question
-from data.loaders.BaseDataLoader import PassageDataLoader
-from data.loaders.DataLoaderFactory import DataLoaderFactory
+from bcqa.config.constants import Split
+from bcqa.data.datastructures.evidence import Evidence
+from bcqa.data.datastructures.question import Question
+from bcqa.data.loaders.BaseDataLoader import PassageDataLoader
+from bcqa.data.loaders.DataLoaderFactory import DataLoaderFactory
 
-from data.loaders.Tokenizer import Tokenizer
+from bcqa.data.loaders.Tokenizer import Tokenizer
 
 
 class RetrieverDataset:
     def __init__(self, dataset:str,passage_dataset:str,config_path,split:Split, batch_size=32,tokenizer="bert-base-uncased"):
         self.split = split
         self.config = configparser.ConfigParser()
         self.config.read(config_path)
```

### Comparing `bcqa-1.0.5/bcqa/data/loaders/StrategyQADataLoader.py` & `bcqa-1.0.6/bcqa/data/loaders/StrategyQADataLoader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import os
 import tqdm
-from config.constants import Split
-from data.datastructures.answer import Answer
-from data.datastructures.dataset import DprDataset
-from data.datastructures.evidence import Evidence
-from data.datastructures.question import Question
-from data.datastructures.sample import Sample
-from data.loaders.BaseDataLoader import GenericDataLoader
+from bcqa.config.constants import Split
+from bcqa.data.datastructures.answer import Answer
+from bcqa.data.datastructures.dataset import DprDataset
+from bcqa.data.datastructures.evidence import Evidence
+from bcqa.data.datastructures.question import Question
+from bcqa.data.datastructures.sample import Sample
+from bcqa.data.loaders.BaseDataLoader import GenericDataLoader
 
 
 class StrategyQADataLoader(GenericDataLoader):
     def __init__(self, dataset: str, tokenizer="bert-base-uncased", config_path='test_config.ini', split=Split.TRAIN,
                  batch_size=None, corpus=None):
         self.corpus = corpus
         self.titles = [self.corpus[idx].title() for idx,_ in enumerate(self.corpus)]
```

### Comparing `bcqa-1.0.5/bcqa/data/loaders/TATQADataLoader.py` & `bcqa-1.0.6/bcqa/data/loaders/TATQADataLoader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import os
-from config.constants import Split
-from data.datastructures.answer import Answer
-from data.datastructures.dataset import DprDataset
-from data.datastructures.evidence import Evidence, TableEvidence
-from data.datastructures.question import Question
-from data.datastructures.sample import Sample
-from data.loaders.BaseDataLoader import GenericDataLoader
-from config.constants import DataTypes
+from bcqa.config.constants import Split
+from bcqa.data.datastructures.answer import Answer
+from bcqa.data.datastructures.dataset import DprDataset
+from bcqa.data.datastructures.evidence import Evidence, TableEvidence
+from bcqa.data.datastructures.question import Question
+from bcqa.data.datastructures.sample import Sample
+from bcqa.data.loaders.BaseDataLoader import GenericDataLoader
+from bcqa.config.constants import DataTypes
 
 
 class TATQADataLoader(GenericDataLoader):
     def __init__(self, dataset: str, tokenizer="bert-base-uncased", config_path='test_config.ini', split=Split.TRAIN,
                  batch_size=None, corpus=None):
         super().__init__(dataset, tokenizer, config_path, split, batch_size)
         self.corpus = corpus
```

### Comparing `bcqa-1.0.5/bcqa/data/loaders/Tokenizer.py` & `bcqa-1.0.6/bcqa/data/loaders/Tokenizer.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/data/loaders/WikiMultihopQADataLoader.py` & `bcqa-1.0.6/bcqa/data/loaders/MusiqueQaDataLoader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 import json
 import os
 import tqdm
-from typing import List
-from config.constants import Split
-from data.datastructures.answer import Answer
-from data.datastructures.dataset import DprDataset
-from data.datastructures.evidence import Evidence
-from data.datastructures.question import Question
-from data.datastructures.sample import Sample
-from data.loaders.BaseDataLoader import GenericDataLoader
+from bcqa.config.constants import Split
+from bcqa.data.datastructures.answer import Answer
+from bcqa.data.datastructures.dataset import DprDataset
+from bcqa.data.datastructures.evidence import Evidence
+from bcqa.data.datastructures.question import Question
+from bcqa.data.datastructures.sample import Sample
+from bcqa.data.loaders.BaseDataLoader import GenericDataLoader
 
 
-class WikiMultihopQADataLoader(GenericDataLoader):
+class MusiqueQADataLoader(GenericDataLoader):
     def __init__(self, dataset: str, tokenizer="bert-base-uncased", config_path='test_config.ini', split=Split.TRAIN,
                  batch_size=None, corpus=None):
         self.corpus = corpus
         self.titles = [self.corpus[idx].title().split(" - ")[0] for idx,_ in enumerate(self.corpus)]
         print(self.titles[100],self.corpus[100].title())
         super().__init__(dataset, tokenizer, config_path, split, batch_size)
 
 
     def load_raw_dataset(self, split=Split.TRAIN):
         dataset = self.load_json(split)
         print(len(dataset))
-        for  query_index, data in enumerate(tqdm.tqdm(dataset[:1200])):
-            if len(data["context"]) == 0:
-                data["context"] = ['some random title', ['some random stuff']]
-            for evidence_set in data["context"]:
-                title = evidence_set[0]
+        for  query_index, data in enumerate(tqdm.tqdm(dataset)):
+            if len(data["paragraphs"]) == 0:
+                data["paragraphs"] = ['some random title', ['some random stuff']]
+            for evidence_set in data["paragraphs"]:
+                title = evidence_set["title"]
                 #for evidence in evidence_set[1]:
-                evidence = " ".join(evidence_set[1])
+                evidence = evidence_set["paragraph_text"]
                 #print(list(self.titles).index(title.split(" - ")[0]))
                 self.raw_data.append(
-                    Sample(query_index, Question(data["question"],idx=data["_id"]), Answer(data["answer"]),
+                    Sample(query_index, Question(data["question"],idx=data["id"]), Answer(data["answer"]),
                             Evidence(text=evidence, 
                                     idx=list(self.titles).index(title.split(" - ")[0]),title=title)
                 ))
 
+
     def load_tokenized(self):
         if self.tokenized_path and os.path.exists(self.tokenized_path):
             self.logger.info("Loading DPR data from {}".format(self.tokenized_path))
             with open(self.tokenized_path, "r") as f:
                 ip_ids, ip_attention, evidence_ids, evidence_attention = json.load(f)
         else:
             ip_ids, ip_attention = self.tokenize_questions()
```

### Comparing `bcqa-1.0.5/bcqa/losses/DprNllLoss.py` & `bcqa-1.0.6/bcqa/losses/DprNllLoss.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/metrics/ExactMatch.py` & `bcqa-1.0.6/bcqa/metrics/ExactMatch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from metrics.MetricsBase import Metric
+from bcqa.metrics.MetricsBase import Metric
 
 
 class ExactMatch(Metric):
     def name(self):
         return "Exact Match"    
     def evaluate(self,answers1, answers2):
         if type(answers1)==list:
```

### Comparing `bcqa-1.0.5/bcqa/metrics/MetricsBase.py` & `bcqa-1.0.6/bcqa/metrics/MetricsBase.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/metrics/SimilarityMatch.py` & `bcqa-1.0.6/bcqa/metrics/SimilarityMatch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import torch
-from metrics.MetricsBase import Metric
+from bcqa.metrics.MetricsBase import Metric
 
 class SimilarityMetric(Metric):
 
     def name(self):
         return "None"  
 
     def normalize_embedding(self,embeddings):
```

### Comparing `bcqa-1.0.5/bcqa/re_ranker/CrossEncoder.py` & `bcqa-1.0.6/bcqa/re_ranker/CrossEncoder.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/re_ranker/ReRanker.py` & `bcqa-1.0.6/bcqa/re_ranker/ReRanker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from typing import List, Dict
-from data.datastructures.question import Question
-from data.datastructures.evidence import Evidence
+from bcqa.data.datastructures.question import Question
+from bcqa.data.datastructures.evidence import Evidence
 
 from re_ranker.CrossEncoder import CrossEncoder
 class Reranker:
     
     def __init__(self, model_name, batch_size: int = 128, **kwargs):
         self.cross_encoder = CrossEncoder(model_name)
         self.batch_size = batch_size
```

### Comparing `bcqa-1.0.5/bcqa/retriever/ANCE.py` & `bcqa-1.0.6/bcqa/retriever/ANCE.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from configparser import ConfigParser
 import heapq
 from typing import Dict, List, Union
 import numpy as np
 
 from torch import Tensor
 import torch
-from data.datastructures.evidence import Evidence
-from data.datastructures.hyperparameters.dpr import DenseHyperParams
-from data.datastructures.question import Question
-from metrics.SimilarityMatch import SimilarityMetric
-from retriever.BaseRetriever import BaseRetriver
+from bcqa.data.datastructures.evidence import Evidence
+from bcqa.data.datastructures.hyperparameters.dpr import DenseHyperParams
+from bcqa.data.datastructures.question import Question
+from bcqa.metrics.SimilarityMatch import SimilarityMetric
+from bcqa.retriever.BaseRetriever import BaseRetriver
 from sentence_transformers import SentenceTransformer
 import logging
 
 from retriever.DenseFullSearch import DenseFullSearch
 
 
 class ANCE(DenseFullSearch):
```

### Comparing `bcqa-1.0.5/bcqa/retriever/Baleen.py` & `bcqa-1.0.6/bcqa/retriever/Baleen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from retriever.ColBERT.baleen.condenser.condense import Condenser
 from retriever.ColBERT.baleen.hop_searcher import HopSearcher
 from retriever.ColBERT.baleen.engine import Baleen
-from data.datastructures.hyperparameters.dpr import DenseHyperParams
+from bcqa.data.datastructures.hyperparameters.dpr import DenseHyperParams
 from retriever.HfRetriever import HfRetriever
 from .ColBERT.colbert import Indexer, Searcher
 from .ColBERT.colbert.infra import Run, RunConfig, ColBERTConfig
 from .ColBERT.colbert.data import Queries, Collection
-from data.datastructures.evidence import Evidence
-from data.datastructures.question import Question
+from bcqa.data.datastructures.evidence import Evidence
+from bcqa.data.datastructures.question import Question
 import os
 from metrics.SimilarityMatch import SimilarityMetric
 import logging
 import tqdm
 from typing import List,Dict
 
 class BaleenRetriever():
```

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/data/collection.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/data/collection.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/data/examples.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/data/examples.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/data/queries.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/data/queries.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/data/ranking.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/data/ranking.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/evaluation/load_model.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/evaluation/load_model.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/evaluation/loaders.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/evaluation/loaders.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/evaluation/metrics.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/index_updater.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/index_updater.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexer.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexer.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual_embeddings.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual_embeddings.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual_embeddings_strided.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual_embeddings_strided.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/collection_encoder.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/collection_encoder.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/collection_indexer.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/collection_indexer.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/index_manager.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/index_manager.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/index_saver.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/index_saver.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/loaders.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/loaders.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/indexing/utils.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/indexing/utils.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/infra/config/base_config.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/infra/config/base_config.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/infra/config/core_config.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/infra/config/core_config.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/infra/config/settings.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/infra/config/settings.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/infra/launcher.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/infra/launcher.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/infra/provenance.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/infra/provenance.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/infra/run.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/infra/run.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/base_colbert.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/base_colbert.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/checkpoint.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/checkpoint.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/colbert.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/colbert.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/hf_colbert.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/hf_colbert.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/reranker/electra.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/reranker/electra.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/reranker/tokenizer.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/reranker/tokenizer.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/tokenization/doc_tokenization.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/tokenization/doc_tokenization.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/tokenization/query_tokenization.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/tokenization/query_tokenization.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/modeling/tokenization/utils.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/modeling/tokenization/utils.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/search/candidate_generation.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/search/candidate_generation.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/search/index_loader.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/search/index_loader.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/search/index_storage.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/search/index_storage.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/search/strided_tensor.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/search/strided_tensor.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/search/strided_tensor_core.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/search/strided_tensor_core.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/searcher.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/searcher.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/trainer.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/trainer.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/training/eager_batcher.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/training/eager_batcher.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/training/lazy_batcher.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/training/lazy_batcher.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/training/rerank_batcher.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/training/rerank_batcher.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/training/training.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/training/training.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/colbert/training/utils.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/colbert/training/utils.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/server.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/server.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/setup.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/setup.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/utility/evaluate/annotate_EM.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/utility/evaluate/annotate_EM.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/utility/evaluate/annotate_EM_helpers.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/utility/evaluate/annotate_EM_helpers.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/utility/evaluate/evaluate_lotte_rankings.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/utility/evaluate/evaluate_lotte_rankings.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/utility/evaluate/msmarco_passages.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/utility/evaluate/msmarco_passages.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/utility/preprocess/docs2passages.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/utility/preprocess/docs2passages.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/utility/preprocess/queries_split.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/utility/preprocess/queries_split.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/utility/rankings/dev_subsample.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/utility/rankings/dev_subsample.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/utility/rankings/merge.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/utility/rankings/merge.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/utility/rankings/split_by_offset.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/utility/rankings/split_by_offset.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/utility/rankings/split_by_queries.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/utility/rankings/split_by_queries.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/utility/rankings/tune.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/utility/rankings/tune.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/utility/supervision/self_training.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/utility/supervision/self_training.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/utility/supervision/triples.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/utility/supervision/triples.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/utility/utils/dpr.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/utility/utils/dpr.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/utility/utils/qa_loaders.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/utility/utils/qa_loaders.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/ColBERT/utility/utils/save_metadata.py` & `bcqa-1.0.6/bcqa/retriever/ColBERT/utility/utils/save_metadata.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/bcqa/retriever/DenseFullSearch.py` & `bcqa-1.0.6/bcqa/retriever/DenseFullSearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import heapq
 from typing import Dict, List, Union, Tuple, Any
 import numpy as np
 import os
 import joblib
 from torch import Tensor
 import torch
-from data.datastructures.evidence import Evidence
-from data.datastructures.question import Question
-from metrics.SimilarityMatch import SimilarityMetric
-from retriever.BaseRetriever import BaseRetriver
+from bcqa.data.datastructures.evidence import Evidence
+from bcqa.data.datastructures.question import Question
+from bcqa.metrics.SimilarityMatch import SimilarityMetric
+from bcqa.retriever.BaseRetriever import BaseRetriver
 from sentence_transformers import SentenceTransformer
 import logging
-from data.datastructures.hyperparameters.dpr import DenseHyperParams
+from bcqa.data.datastructures.hyperparameters.dpr import DenseHyperParams
 
 
 
 class DenseFullSearch(BaseRetriver):
 
     def __init__(self,config=DenseHyperParams) -> None:
         super().__init__()
```

### Comparing `bcqa-1.0.5/bcqa/retriever/HfRetriever.py` & `bcqa-1.0.6/bcqa/retriever/HfRetriever.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 import numpy as np
 import os
 import heapq
 import joblib
 from torch import Tensor
 import torch
 from tqdm import tqdm
-from data.datastructures.evidence import Evidence
-from data.datastructures.question import Question
-from metrics.SimilarityMatch import SimilarityMetric
-from retriever.BaseRetriever import BaseRetriver
+from bcqa.data.datastructures.evidence import Evidence
+from bcqa.data.datastructures.question import Question
+from bcqa.metrics.SimilarityMatch import SimilarityMetric
+from bcqa.retriever.BaseRetriever import BaseRetriver
 from sentence_transformers import SentenceTransformer
 from transformers import AutoTokenizer, AutoModel
 import logging
-from data.datastructures.hyperparameters.dpr import DenseHyperParams
+from bcqa.data.datastructures.hyperparameters.dpr import DenseHyperParams
 
 class HfRetriever(BaseRetriver):
 
     def __init__(self,config=DenseHyperParams) -> None:
         super().__init__()
         self.config = config
         #print("self.config.query_encoder_path",self.config.query_encoder_path)
```

### Comparing `bcqa-1.0.5/bcqa/retriever/TCTColBERT.py` & `bcqa-1.0.6/bcqa/retriever/TCTColBERT.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 
 
-from data.datastructures.hyperparameters.dpr import DenseHyperParams
-from retriever.HfRetriever import HfRetriever
+from bcqa.data.datastructures.hyperparameters.dpr import DenseHyperParams
+from bcqa.retriever.HfRetriever import HfRetriever
 from .ColBERT.colbert import Indexer, Searcher
 from .ColBERT.colbert.infra import Run, RunConfig, ColBERTConfig
 from .ColBERT.colbert.data import Queries, Collection
-from data.datastructures.evidence import Evidence
-from data.datastructures.question import Question
-from metrics.SimilarityMatch import SimilarityMetric
+from bcqa.data.datastructures.evidence import Evidence
+from bcqa.data.datastructures.question import Question
+from bcqa.metrics.SimilarityMatch import SimilarityMetric
 import logging
 import tqdm
 import heapq
 from typing import List,Dict
 
 
 class TCTColBERT():
```

### Comparing `bcqa-1.0.5/bcqa.egg-info/PKG-INFO` & `bcqa-1.0.6/bcqa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcqa
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Benchmark for Complex Heterogeneous Question answering
 Home-page: https://github.com/VenkteshV/BCQA
 Download-URL: 
 Author: Venktesh V, Deepali Prabhu
 Author-email: venkyviswa12@gmail.com
 License: Apache License 2.0
 Keywords: Information Retrieval Transformer Networks BERT PyTorch Complex Question Answering IR NLP deep learning
```

### Comparing `bcqa-1.0.5/bcqa.egg-info/SOURCES.txt` & `bcqa-1.0.6/bcqa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.5/setup.py` & `bcqa-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 optional_packages = {
     "tf" : ['tensorflow>=2.2.0', 'tensorflow-text', 'tensorflow-hub']
 }
 
 setup(
     name="bcqa",
-    version="1.0.5",
+    version="1.0.6",
     author="Venktesh V, Deepali Prabhu",
     author_email="venkyviswa12@gmail.com",
     description="A Benchmark for Complex Heterogeneous Question answering",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="Apache License 2.0",
     url="https://github.com/VenkteshV/BCQA",
```

