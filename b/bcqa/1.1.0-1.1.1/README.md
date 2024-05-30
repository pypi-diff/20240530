# Comparing `tmp/bcqa-1.1.0.tar.gz` & `tmp/bcqa-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcqa-1.1.0.tar", last modified: Thu May 30 20:26:06 2024, max compression
+gzip compressed data, was "bcqa-1.1.1.tar", last modified: Thu May 30 21:24:03 2024, max compression
```

## Comparing `bcqa-1.1.0.tar` & `bcqa-1.1.1.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.402452 bcqa-1.1.0/
--rw-r--r--   0 venky    (100600114) venky    (100600114)     3192 2024-05-30 20:26:06.402452 bcqa-1.1.0/PKG-INFO
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2001 2024-05-30 16:47:11.000000 bcqa-1.1.0/README.md
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.379119 bcqa-1.1.0/bcqa/
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:30:15.000000 bcqa-1.1.0/bcqa/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.379119 bcqa-1.1.0/bcqa/config/
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:46:47.000000 bcqa-1.1.0/bcqa/config/__init__.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)      406 2024-03-12 23:59:30.000000 bcqa-1.1.0/bcqa/config/constants.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.379119 bcqa-1.1.0/bcqa/data/
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:30:31.000000 bcqa-1.1.0/bcqa/data/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.379119 bcqa-1.1.0/bcqa/data/datastructures/
--rw-r--r--   0 venky    (100600114) venky    (100600114)       89 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/data/datastructures/AnnConstants.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)       45 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/data/datastructures/LLmConstants.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/data/datastructures/__init__.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1057 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/data/datastructures/answer.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     6421 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/data/datastructures/dataset.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)      859 2024-05-30 19:02:45.000000 bcqa-1.1.0/bcqa/data/datastructures/evidence.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.382452 bcqa-1.1.0/bcqa/data/datastructures/hyperparameters/
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:25:05.000000 bcqa-1.1.0/bcqa/data/datastructures/hyperparameters/__init__.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)      444 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/data/datastructures/hyperparameters/base.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1801 2024-05-30 19:02:56.000000 bcqa-1.1.0/bcqa/data/datastructures/hyperparameters/dpr.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1028 2024-05-30 19:02:56.000000 bcqa-1.1.0/bcqa/data/datastructures/hyperparameters/tapas.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)      382 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/data/datastructures/question.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)      724 2024-05-30 19:02:56.000000 bcqa-1.1.0/bcqa/data/datastructures/sample.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.382452 bcqa-1.1.0/bcqa/data/loaders/
--rw-r--r--   0 venky    (100600114) venky    (100600114)     3189 2024-05-30 19:02:56.000000 bcqa-1.1.0/bcqa/data/loaders/AmbigQADataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     8869 2024-05-30 19:02:56.000000 bcqa-1.1.0/bcqa/data/loaders/BaseDataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1743 2024-05-30 19:02:56.000000 bcqa-1.1.0/bcqa/data/loaders/DataLoaderFactory.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     3287 2024-05-30 19:03:05.000000 bcqa-1.1.0/bcqa/data/loaders/DprDataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1969 2024-05-30 19:02:56.000000 bcqa-1.1.0/bcqa/data/loaders/FinQADataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/data/loaders/HfDataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2348 2024-05-30 19:02:56.000000 bcqa-1.1.0/bcqa/data/loaders/MusiqueQaDataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2338 2024-05-30 19:02:56.000000 bcqa-1.1.0/bcqa/data/loaders/OTTQADataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     6938 2024-05-30 19:02:56.000000 bcqa-1.1.0/bcqa/data/loaders/ReaderDataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1924 2024-05-30 19:02:14.000000 bcqa-1.1.0/bcqa/data/loaders/RetrieverDataset.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2382 2024-05-30 19:02:56.000000 bcqa-1.1.0/bcqa/data/loaders/StrategyQADataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2385 2024-05-30 19:02:56.000000 bcqa-1.1.0/bcqa/data/loaders/TATQADataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)      569 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/data/loaders/Tokenizer.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2364 2024-05-30 19:02:56.000000 bcqa-1.1.0/bcqa/data/loaders/WikiMultihopQADataLoader.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/data/loaders/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.385786 bcqa-1.1.0/bcqa/evaluation/
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/evaluation/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.385786 bcqa-1.1.0/bcqa/losses/
--rw-r--r--   0 venky    (100600114) venky    (100600114)      126 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/losses/BaseLoss.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1613 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/losses/DprNllLoss.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:30:59.000000 bcqa-1.1.0/bcqa/losses/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.385786 bcqa-1.1.0/bcqa/methods/
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:31:06.000000 bcqa-1.1.0/bcqa/methods/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.385786 bcqa-1.1.0/bcqa/methods/ir/
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:08:55.000000 bcqa-1.1.0/bcqa/methods/ir/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.385786 bcqa-1.1.0/bcqa/methods/ir/dense/
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:13:25.000000 bcqa-1.1.0/bcqa/methods/ir/dense/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.385786 bcqa-1.1.0/bcqa/methods/ir/dense/dpr/
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:13:47.000000 bcqa-1.1.0/bcqa/methods/ir/dense/dpr/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.385786 bcqa-1.1.0/bcqa/methods/ir/dense/dpr/indexer/
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:14:10.000000 bcqa-1.1.0/bcqa/methods/ir/dense/dpr/indexer/__init__.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1699 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/methods/ir/dense/dpr/indexer/annoyIndexer.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1290 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/methods/ir/dense/dpr/indexer/faissIndexer.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)      944 2024-05-30 19:02:56.000000 bcqa-1.1.0/bcqa/methods/ir/dense/dpr/indexer/indexer.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.385786 bcqa-1.1.0/bcqa/methods/ir/dense/dpr/models/
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:14:40.000000 bcqa-1.1.0/bcqa/methods/ir/dense/dpr/models/__init__.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2853 2024-05-30 19:02:56.000000 bcqa-1.1.0/bcqa/methods/ir/dense/dpr/models/bi_encoder.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     6698 2024-05-30 19:02:56.000000 bcqa-1.1.0/bcqa/methods/ir/dense/dpr/models/dpr_sentence_transformers_inference.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.385786 bcqa-1.1.0/bcqa/methods/llms/
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:09:05.000000 bcqa-1.1.0/bcqa/methods/llms/__init__.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)      866 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/methods/llms/flant5_engine.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1067 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/methods/llms/llama_engine.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1248 2024-05-30 19:02:56.000000 bcqa-1.1.0/bcqa/methods/llms/llm_engine_orchestrator.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2214 2024-05-26 07:33:22.000000 bcqa-1.1.0/bcqa/methods/llms/openai_engine.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-13 17:02:58.000000 bcqa-1.1.0/bcqa/methods/utils.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.389119 bcqa-1.1.0/bcqa/metrics/
--rw-r--r--   0 venky    (100600114) venky    (100600114)      601 2024-05-30 19:05:24.000000 bcqa-1.1.0/bcqa/metrics/ExactMatch.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)      624 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/metrics/MetricsBase.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1449 2024-05-30 19:05:30.000000 bcqa-1.1.0/bcqa/metrics/SimilarityMatch.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:31:16.000000 bcqa-1.1.0/bcqa/metrics/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.389119 bcqa-1.1.0/bcqa/metrics/retrieval/
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2657 2024-05-30 19:03:44.000000 bcqa-1.1.0/bcqa/metrics/retrieval/RetrievalMetrics.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:09:40.000000 bcqa-1.1.0/bcqa/metrics/retrieval/__init__.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1139 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/metrics/retrieval/accuracy.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.389119 bcqa-1.1.0/bcqa/re_ranker/
--rw-r--r--   0 venky    (100600114) venky    (100600114)      551 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/re_ranker/CrossEncoder.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1904 2024-05-30 19:02:56.000000 bcqa-1.1.0/bcqa/re_ranker/ReRanker.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:31:29.000000 bcqa-1.1.0/bcqa/re_ranker/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.389119 bcqa-1.1.0/bcqa/retriever/
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1432 2024-05-30 19:06:03.000000 bcqa-1.1.0/bcqa/retriever/ANCE.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2969 2024-05-30 19:02:56.000000 bcqa-1.1.0/bcqa/retriever/Baleen.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)      343 2024-01-07 21:56:32.000000 bcqa-1.1.0/bcqa/retriever/BaseRetriever.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.389119 bcqa-1.1.0/bcqa/retriever/ColBERT/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:11.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.392452 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/
--rw-------   0 venky    (100600114) venky    (100600114)      174 2024-01-15 22:15:14.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.392452 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/data/
--rw-------   0 venky    (100600114) venky    (100600114)       97 2024-01-15 22:15:16.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/data/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     3264 2024-05-27 16:19:05.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/data/collection.py
--rw-------   0 venky    (100600114) venky    (100600114)      421 2024-01-15 22:15:16.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/data/dataset.py
--rw-------   0 venky    (100600114) venky    (100600114)     2788 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/data/examples.py
--rw-------   0 venky    (100600114) venky    (100600114)     4429 2024-05-27 16:20:51.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/data/queries.py
--rw-------   0 venky    (100600114) venky    (100600114)     2846 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/data/ranking.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.392452 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/evaluation/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:12.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/evaluation/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)      973 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/evaluation/load_model.py
--rw-------   0 venky    (100600114) venky    (100600114)     6528 2024-05-27 16:20:37.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/evaluation/loaders.py
--rw-------   0 venky    (100600114) venky    (100600114)     4322 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/evaluation/metrics.py
--rw-------   0 venky    (100600114) venky    (100600114)      286 2024-01-15 22:15:14.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/index.py
--rw-------   0 venky    (100600114) venky    (100600114)    21339 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/index_updater.py
--rw-------   0 venky    (100600114) venky    (100600114)     3236 2024-05-27 16:23:46.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexer.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.392452 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:12.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.392452 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/codecs/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:13.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/codecs/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)    10982 2024-05-27 17:42:56.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual.py
--rw-------   0 venky    (100600114) venky    (100600114)     4931 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual_embeddings.py
--rw-------   0 venky    (100600114) venky    (100600114)     1223 2024-05-27 18:21:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual_embeddings_strided.py
--rw-------   0 venky    (100600114) venky    (100600114)     1866 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/collection_encoder.py
--rw-------   0 venky    (100600114) venky    (100600114)    21552 2024-05-27 17:43:15.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/collection_indexer.py
--rw-------   0 venky    (100600114) venky    (100600114)      878 2024-01-15 22:15:12.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/index_manager.py
--rw-------   0 venky    (100600114) venky    (100600114)     2936 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/index_saver.py
--rw-------   0 venky    (100600114) venky    (100600114)     1995 2024-01-15 22:15:13.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/loaders.py
--rw-------   0 venky    (100600114) venky    (100600114)     1961 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/utils.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.395786 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/infra/
--rw-------   0 venky    (100600114) venky    (100600114)       40 2024-01-15 22:15:15.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/infra/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.395786 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/infra/config/
--rw-------   0 venky    (100600114) venky    (100600114)       45 2024-01-15 22:15:15.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/infra/config/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     4121 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/infra/config/base_config.py
--rw-------   0 venky    (100600114) venky    (100600114)      364 2024-01-15 22:15:15.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/infra/config/config.py
--rw-------   0 venky    (100600114) venky    (100600114)     2430 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/infra/config/core_config.py
--rw-------   0 venky    (100600114) venky    (100600114)     4393 2024-05-27 16:55:49.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/infra/config/settings.py
--rw-------   0 venky    (100600114) venky    (100600114)     4683 2024-05-27 16:24:47.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/infra/launcher.py
--rw-------   0 venky    (100600114) venky    (100600114)      932 2024-01-15 22:15:15.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/infra/provenance.py
--rw-------   0 venky    (100600114) venky    (100600114)     2692 2024-05-27 16:56:04.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/infra/run.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.395786 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:18.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     3977 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/base_colbert.py
--rw-------   0 venky    (100600114) venky    (100600114)     5513 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/checkpoint.py
--rw-------   0 venky    (100600114) venky    (100600114)     7644 2024-05-27 16:20:37.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/colbert.py
--rw-------   0 venky    (100600114) venky    (100600114)     5170 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/hf_colbert.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.395786 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/reranker/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:18.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/reranker/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     1272 2024-01-15 22:15:18.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/reranker/electra.py
--rw-------   0 venky    (100600114) venky    (100600114)      608 2024-01-15 22:15:18.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/reranker/tokenizer.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.395786 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/tokenization/
--rw-------   0 venky    (100600114) venky    (100600114)      244 2024-05-27 16:20:16.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/tokenization/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     2579 2024-05-27 16:20:16.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/tokenization/doc_tokenization.py
--rw-------   0 venky    (100600114) venky    (100600114)     5161 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/tokenization/query_tokenization.py
--rw-------   0 venky    (100600114) venky    (100600114)     2054 2024-01-15 22:15:17.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/tokenization/utils.py
--rw-------   0 venky    (100600114) venky    (100600114)      471 2024-01-18 20:49:04.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/parameters.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.395786 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/ranking/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:16.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/ranking/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.395786 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/search/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:16:50.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/search/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     2111 2024-05-27 18:24:43.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/search/candidate_generation.py
--rw-------   0 venky    (100600114) venky    (100600114)     3152 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/search/index_loader.py
--rw-------   0 venky    (100600114) venky    (100600114)     8853 2024-05-27 18:10:29.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/search/index_storage.py
--rw-------   0 venky    (100600114) venky    (100600114)     7076 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/search/strided_tensor.py
--rw-------   0 venky    (100600114) venky    (100600114)     4181 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/search/strided_tensor_core.py
--rw-------   0 venky    (100600114) venky    (100600114)     5310 2024-05-27 18:20:23.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/searcher.py
--rw-------   0 venky    (100600114) venky    (100600114)     1329 2024-05-27 16:19:05.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/trainer.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.399119 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/training/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:16:49.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/training/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     2072 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/training/eager_batcher.py
--rw-------   0 venky    (100600114) venky    (100600114)     2768 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/training/lazy_batcher.py
--rw-------   0 venky    (100600114) venky    (100600114)     2736 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/training/rerank_batcher.py
--rw-------   0 venky    (100600114) venky    (100600114)     5954 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/training/training.py
--rw-------   0 venky    (100600114) venky    (100600114)     1907 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/training/utils.py
--rw-------   0 venky    (100600114) venky    (100600114)     1568 2024-05-27 16:18:37.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/server.py
--rw-------   0 venky    (100600114) venky    (100600114)     1043 2024-01-15 22:16:52.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/setup.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.399119 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:09.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.399119 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/evaluate/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:09.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/evaluate/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     2955 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/evaluate/annotate_EM.py
--rw-------   0 venky    (100600114) venky    (100600114)     2531 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/evaluate/annotate_EM_helpers.py
--rw-------   0 venky    (100600114) venky    (100600114)     2604 2024-01-15 22:15:09.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/evaluate/evaluate_lotte_rankings.py
--rw-------   0 venky    (100600114) venky    (100600114)     4224 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/evaluate/msmarco_passages.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.399119 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/preprocess/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:09.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/preprocess/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     4808 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/preprocess/docs2passages.py
--rw-------   0 venky    (100600114) venky    (100600114)     2243 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/preprocess/queries_split.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.399119 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/rankings/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:10.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/rankings/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     1386 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/rankings/dev_subsample.py
--rw-------   0 venky    (100600114) venky    (100600114)     1658 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/rankings/merge.py
--rw-------   0 venky    (100600114) venky    (100600114)     1334 2024-01-15 22:15:10.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/rankings/split_by_offset.py
--rw-------   0 venky    (100600114) venky    (100600114)     1754 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/rankings/split_by_queries.py
--rw-------   0 venky    (100600114) venky    (100600114)     1777 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/rankings/tune.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.399119 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/supervision/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:09.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/supervision/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     3942 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/supervision/self_training.py
--rw-------   0 venky    (100600114) venky    (100600114)     5086 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/supervision/triples.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.399119 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/utils/
--rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:10.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/utils/__init__.py
--rw-------   0 venky    (100600114) venky    (100600114)     7071 2024-01-15 22:15:10.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/utils/dpr.py
--rw-------   0 venky    (100600114) venky    (100600114)      744 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/utils/qa_loaders.py
--rw-------   0 venky    (100600114) venky    (100600114)     1949 2024-05-27 16:24:22.000000 bcqa-1.1.0/bcqa/retriever/ColBERT/utility/utils/save_metadata.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)      317 2024-05-30 19:06:38.000000 bcqa-1.1.0/bcqa/retriever/Contriever.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     7626 2024-05-30 19:06:48.000000 bcqa-1.1.0/bcqa/retriever/DenseFullSearch.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     8952 2024-05-30 19:07:00.000000 bcqa-1.1.0/bcqa/retriever/HfRetriever.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)     5096 2024-05-30 19:07:14.000000 bcqa-1.1.0/bcqa/retriever/TCTColBERT.py
--rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:31:38.000000 bcqa-1.1.0/bcqa/retriever/__init__.py
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:26:06.402452 bcqa-1.1.0/bcqa.egg-info/
--rw-r--r--   0 venky    (100600114) venky    (100600114)     3192 2024-05-30 20:26:06.000000 bcqa-1.1.0/bcqa.egg-info/PKG-INFO
--rw-r--r--   0 venky    (100600114) venky    (100600114)     7315 2024-05-30 20:26:06.000000 bcqa-1.1.0/bcqa.egg-info/SOURCES.txt
--rw-r--r--   0 venky    (100600114) venky    (100600114)        1 2024-05-30 20:26:06.000000 bcqa-1.1.0/bcqa.egg-info/dependency_links.txt
--rw-r--r--   0 venky    (100600114) venky    (100600114)      194 2024-05-30 20:26:06.000000 bcqa-1.1.0/bcqa.egg-info/requires.txt
--rw-r--r--   0 venky    (100600114) venky    (100600114)        5 2024-05-30 20:26:06.000000 bcqa-1.1.0/bcqa.egg-info/top_level.txt
--rw-r--r--   0 venky    (100600114) venky    (100600114)       38 2024-05-30 20:26:06.402452 bcqa-1.1.0/setup.cfg
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1430 2024-05-30 20:25:56.000000 bcqa-1.1.0/setup.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.659853 bcqa-1.1.1/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     3192 2024-05-30 21:24:03.659853 bcqa-1.1.1/PKG-INFO
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2001 2024-05-30 16:47:11.000000 bcqa-1.1.1/README.md
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.636519 bcqa-1.1.1/bcqa/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:30:15.000000 bcqa-1.1.1/bcqa/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.639853 bcqa-1.1.1/bcqa/config/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:46:47.000000 bcqa-1.1.1/bcqa/config/__init__.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      406 2024-03-12 23:59:30.000000 bcqa-1.1.1/bcqa/config/constants.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.639853 bcqa-1.1.1/bcqa/data/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:30:31.000000 bcqa-1.1.1/bcqa/data/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.639853 bcqa-1.1.1/bcqa/data/datastructures/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)       89 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/data/datastructures/AnnConstants.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)       45 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/data/datastructures/LLmConstants.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/data/datastructures/__init__.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1057 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/data/datastructures/answer.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     6421 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/data/datastructures/dataset.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      859 2024-05-30 19:02:45.000000 bcqa-1.1.1/bcqa/data/datastructures/evidence.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.639853 bcqa-1.1.1/bcqa/data/datastructures/hyperparameters/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:25:05.000000 bcqa-1.1.1/bcqa/data/datastructures/hyperparameters/__init__.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      444 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/data/datastructures/hyperparameters/base.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1801 2024-05-30 19:02:56.000000 bcqa-1.1.1/bcqa/data/datastructures/hyperparameters/dpr.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1028 2024-05-30 19:02:56.000000 bcqa-1.1.1/bcqa/data/datastructures/hyperparameters/tapas.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      382 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/data/datastructures/question.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      724 2024-05-30 19:02:56.000000 bcqa-1.1.1/bcqa/data/datastructures/sample.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.643186 bcqa-1.1.1/bcqa/data/loaders/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     3189 2024-05-30 19:02:56.000000 bcqa-1.1.1/bcqa/data/loaders/AmbigQADataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     8869 2024-05-30 19:02:56.000000 bcqa-1.1.1/bcqa/data/loaders/BaseDataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1743 2024-05-30 19:02:56.000000 bcqa-1.1.1/bcqa/data/loaders/DataLoaderFactory.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     3287 2024-05-30 19:03:05.000000 bcqa-1.1.1/bcqa/data/loaders/DprDataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1969 2024-05-30 19:02:56.000000 bcqa-1.1.1/bcqa/data/loaders/FinQADataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/data/loaders/HfDataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2348 2024-05-30 19:02:56.000000 bcqa-1.1.1/bcqa/data/loaders/MusiqueQaDataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2338 2024-05-30 19:02:56.000000 bcqa-1.1.1/bcqa/data/loaders/OTTQADataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     6938 2024-05-30 19:02:56.000000 bcqa-1.1.1/bcqa/data/loaders/ReaderDataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1924 2024-05-30 19:02:14.000000 bcqa-1.1.1/bcqa/data/loaders/RetrieverDataset.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2382 2024-05-30 19:02:56.000000 bcqa-1.1.1/bcqa/data/loaders/StrategyQADataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2385 2024-05-30 19:02:56.000000 bcqa-1.1.1/bcqa/data/loaders/TATQADataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      569 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/data/loaders/Tokenizer.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2364 2024-05-30 19:02:56.000000 bcqa-1.1.1/bcqa/data/loaders/WikiMultihopQADataLoader.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/data/loaders/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.643186 bcqa-1.1.1/bcqa/evaluation/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/evaluation/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.643186 bcqa-1.1.1/bcqa/losses/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      126 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/losses/BaseLoss.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1613 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/losses/DprNllLoss.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:30:59.000000 bcqa-1.1.1/bcqa/losses/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.643186 bcqa-1.1.1/bcqa/methods/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:31:06.000000 bcqa-1.1.1/bcqa/methods/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.643186 bcqa-1.1.1/bcqa/methods/ir/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:08:55.000000 bcqa-1.1.1/bcqa/methods/ir/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.643186 bcqa-1.1.1/bcqa/methods/ir/dense/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:13:25.000000 bcqa-1.1.1/bcqa/methods/ir/dense/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.643186 bcqa-1.1.1/bcqa/methods/ir/dense/dpr/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:13:47.000000 bcqa-1.1.1/bcqa/methods/ir/dense/dpr/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.643186 bcqa-1.1.1/bcqa/methods/ir/dense/dpr/indexer/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:14:10.000000 bcqa-1.1.1/bcqa/methods/ir/dense/dpr/indexer/__init__.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1699 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/methods/ir/dense/dpr/indexer/annoyIndexer.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1290 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/methods/ir/dense/dpr/indexer/faissIndexer.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      944 2024-05-30 19:02:56.000000 bcqa-1.1.1/bcqa/methods/ir/dense/dpr/indexer/indexer.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.643186 bcqa-1.1.1/bcqa/methods/ir/dense/dpr/models/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 20:14:40.000000 bcqa-1.1.1/bcqa/methods/ir/dense/dpr/models/__init__.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2853 2024-05-30 19:02:56.000000 bcqa-1.1.1/bcqa/methods/ir/dense/dpr/models/bi_encoder.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     6708 2024-05-30 20:34:23.000000 bcqa-1.1.1/bcqa/methods/ir/dense/dpr/models/dpr_sentence_transformers_inference.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.646519 bcqa-1.1.1/bcqa/methods/llms/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:09:05.000000 bcqa-1.1.1/bcqa/methods/llms/__init__.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      866 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/methods/llms/flant5_engine.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1067 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/methods/llms/llama_engine.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1248 2024-05-30 19:02:56.000000 bcqa-1.1.1/bcqa/methods/llms/llm_engine_orchestrator.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2214 2024-05-26 07:33:22.000000 bcqa-1.1.1/bcqa/methods/llms/openai_engine.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-01-13 17:02:58.000000 bcqa-1.1.1/bcqa/methods/utils.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.646519 bcqa-1.1.1/bcqa/metrics/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      601 2024-05-30 19:05:24.000000 bcqa-1.1.1/bcqa/metrics/ExactMatch.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      624 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/metrics/MetricsBase.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1449 2024-05-30 19:05:30.000000 bcqa-1.1.1/bcqa/metrics/SimilarityMatch.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:31:16.000000 bcqa-1.1.1/bcqa/metrics/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.646519 bcqa-1.1.1/bcqa/metrics/retrieval/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2657 2024-05-30 19:03:44.000000 bcqa-1.1.1/bcqa/metrics/retrieval/RetrievalMetrics.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 19:09:40.000000 bcqa-1.1.1/bcqa/metrics/retrieval/__init__.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1139 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/metrics/retrieval/accuracy.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.646519 bcqa-1.1.1/bcqa/re_ranker/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      551 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/re_ranker/CrossEncoder.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1904 2024-05-30 19:02:56.000000 bcqa-1.1.1/bcqa/re_ranker/ReRanker.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:31:29.000000 bcqa-1.1.1/bcqa/re_ranker/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.646519 bcqa-1.1.1/bcqa/retriever/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1432 2024-05-30 19:06:03.000000 bcqa-1.1.1/bcqa/retriever/ANCE.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2969 2024-05-30 19:02:56.000000 bcqa-1.1.1/bcqa/retriever/Baleen.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      343 2024-01-07 21:56:32.000000 bcqa-1.1.1/bcqa/retriever/BaseRetriever.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.649853 bcqa-1.1.1/bcqa/retriever/ColBERT/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:11.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.649853 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/
+-rw-------   0 venky    (100600114) venky    (100600114)      174 2024-01-15 22:15:14.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.649853 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/data/
+-rw-------   0 venky    (100600114) venky    (100600114)       97 2024-01-15 22:15:16.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/data/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     3264 2024-05-27 16:19:05.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/data/collection.py
+-rw-------   0 venky    (100600114) venky    (100600114)      421 2024-01-15 22:15:16.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/data/dataset.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2788 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/data/examples.py
+-rw-------   0 venky    (100600114) venky    (100600114)     4429 2024-05-27 16:20:51.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/data/queries.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2846 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/data/ranking.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.649853 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/evaluation/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:12.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/evaluation/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)      973 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/evaluation/load_model.py
+-rw-------   0 venky    (100600114) venky    (100600114)     6528 2024-05-27 16:20:37.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/evaluation/loaders.py
+-rw-------   0 venky    (100600114) venky    (100600114)     4322 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/evaluation/metrics.py
+-rw-------   0 venky    (100600114) venky    (100600114)      286 2024-01-15 22:15:14.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/index.py
+-rw-------   0 venky    (100600114) venky    (100600114)    21339 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/index_updater.py
+-rw-------   0 venky    (100600114) venky    (100600114)     3236 2024-05-27 16:23:46.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexer.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.649853 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:12.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.653186 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/codecs/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:13.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/codecs/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)    10982 2024-05-27 17:42:56.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual.py
+-rw-------   0 venky    (100600114) venky    (100600114)     4931 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual_embeddings.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1223 2024-05-27 18:21:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual_embeddings_strided.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1866 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/collection_encoder.py
+-rw-------   0 venky    (100600114) venky    (100600114)    21552 2024-05-27 17:43:15.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/collection_indexer.py
+-rw-------   0 venky    (100600114) venky    (100600114)      878 2024-01-15 22:15:12.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/index_manager.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2936 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/index_saver.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1995 2024-01-15 22:15:13.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/loaders.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1961 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/utils.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.653186 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/infra/
+-rw-------   0 venky    (100600114) venky    (100600114)       40 2024-01-15 22:15:15.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/infra/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.653186 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/infra/config/
+-rw-------   0 venky    (100600114) venky    (100600114)       45 2024-01-15 22:15:15.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/infra/config/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     4121 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/infra/config/base_config.py
+-rw-------   0 venky    (100600114) venky    (100600114)      364 2024-01-15 22:15:15.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/infra/config/config.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2430 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/infra/config/core_config.py
+-rw-------   0 venky    (100600114) venky    (100600114)     4393 2024-05-27 16:55:49.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/infra/config/settings.py
+-rw-------   0 venky    (100600114) venky    (100600114)     4683 2024-05-27 16:24:47.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/infra/launcher.py
+-rw-------   0 venky    (100600114) venky    (100600114)      932 2024-01-15 22:15:15.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/infra/provenance.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2692 2024-05-27 16:56:04.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/infra/run.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.653186 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:18.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     3977 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/base_colbert.py
+-rw-------   0 venky    (100600114) venky    (100600114)     5513 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/checkpoint.py
+-rw-------   0 venky    (100600114) venky    (100600114)     7644 2024-05-27 16:20:37.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/colbert.py
+-rw-------   0 venky    (100600114) venky    (100600114)     5170 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/hf_colbert.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.653186 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/reranker/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:18.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/reranker/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1272 2024-01-15 22:15:18.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/reranker/electra.py
+-rw-------   0 venky    (100600114) venky    (100600114)      608 2024-01-15 22:15:18.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/reranker/tokenizer.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.653186 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/tokenization/
+-rw-------   0 venky    (100600114) venky    (100600114)      244 2024-05-27 16:20:16.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/tokenization/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2579 2024-05-27 16:20:16.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/tokenization/doc_tokenization.py
+-rw-------   0 venky    (100600114) venky    (100600114)     5161 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/tokenization/query_tokenization.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2054 2024-01-15 22:15:17.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/tokenization/utils.py
+-rw-------   0 venky    (100600114) venky    (100600114)      471 2024-01-18 20:49:04.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/parameters.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.653186 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/ranking/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:16.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/ranking/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.656519 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/search/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:16:50.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/search/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2111 2024-05-27 18:24:43.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/search/candidate_generation.py
+-rw-------   0 venky    (100600114) venky    (100600114)     3152 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/search/index_loader.py
+-rw-------   0 venky    (100600114) venky    (100600114)     8853 2024-05-27 18:10:29.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/search/index_storage.py
+-rw-------   0 venky    (100600114) venky    (100600114)     7076 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/search/strided_tensor.py
+-rw-------   0 venky    (100600114) venky    (100600114)     4181 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/search/strided_tensor_core.py
+-rw-------   0 venky    (100600114) venky    (100600114)     5310 2024-05-27 18:20:23.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/searcher.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1329 2024-05-27 16:19:05.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/trainer.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.656519 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/training/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:16:49.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/training/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2072 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/training/eager_batcher.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2768 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/training/lazy_batcher.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2736 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/training/rerank_batcher.py
+-rw-------   0 venky    (100600114) venky    (100600114)     5954 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/training/training.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1907 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/training/utils.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1568 2024-05-27 16:18:37.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/server.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1043 2024-01-15 22:16:52.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/setup.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.656519 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:09.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.656519 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/evaluate/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:09.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/evaluate/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2955 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/evaluate/annotate_EM.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2531 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/evaluate/annotate_EM_helpers.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2604 2024-01-15 22:15:09.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/evaluate/evaluate_lotte_rankings.py
+-rw-------   0 venky    (100600114) venky    (100600114)     4224 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/evaluate/msmarco_passages.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.656519 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/preprocess/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:09.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/preprocess/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     4808 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/preprocess/docs2passages.py
+-rw-------   0 venky    (100600114) venky    (100600114)     2243 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/preprocess/queries_split.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.656519 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/rankings/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:10.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/rankings/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1386 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/rankings/dev_subsample.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1658 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/rankings/merge.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1334 2024-01-15 22:15:10.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/rankings/split_by_offset.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1754 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/rankings/split_by_queries.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1777 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/rankings/tune.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.659853 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/supervision/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:09.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/supervision/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     3942 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/supervision/self_training.py
+-rw-------   0 venky    (100600114) venky    (100600114)     5086 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/supervision/triples.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.659853 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/utils/
+-rw-------   0 venky    (100600114) venky    (100600114)        0 2024-01-15 22:15:10.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/utils/__init__.py
+-rw-------   0 venky    (100600114) venky    (100600114)     7071 2024-01-15 22:15:10.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/utils/dpr.py
+-rw-------   0 venky    (100600114) venky    (100600114)      744 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/utils/qa_loaders.py
+-rw-------   0 venky    (100600114) venky    (100600114)     1949 2024-05-27 16:24:22.000000 bcqa-1.1.1/bcqa/retriever/ColBERT/utility/utils/save_metadata.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      317 2024-05-30 19:06:38.000000 bcqa-1.1.1/bcqa/retriever/Contriever.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     7626 2024-05-30 19:06:48.000000 bcqa-1.1.1/bcqa/retriever/DenseFullSearch.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     8952 2024-05-30 19:07:00.000000 bcqa-1.1.1/bcqa/retriever/HfRetriever.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     5096 2024-05-30 19:07:14.000000 bcqa-1.1.1/bcqa/retriever/TCTColBERT.py
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:31:38.000000 bcqa-1.1.1/bcqa/retriever/__init__.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 21:24:03.659853 bcqa-1.1.1/bcqa.egg-info/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     3192 2024-05-30 21:24:03.000000 bcqa-1.1.1/bcqa.egg-info/PKG-INFO
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     7315 2024-05-30 21:24:03.000000 bcqa-1.1.1/bcqa.egg-info/SOURCES.txt
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        1 2024-05-30 21:24:03.000000 bcqa-1.1.1/bcqa.egg-info/dependency_links.txt
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      194 2024-05-30 21:24:03.000000 bcqa-1.1.1/bcqa.egg-info/requires.txt
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        5 2024-05-30 21:24:03.000000 bcqa-1.1.1/bcqa.egg-info/top_level.txt
+-rw-r--r--   0 venky    (100600114) venky    (100600114)       38 2024-05-30 21:24:03.659853 bcqa-1.1.1/setup.cfg
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1430 2024-05-30 21:23:47.000000 bcqa-1.1.1/setup.py
```

### Comparing `bcqa-1.1.0/PKG-INFO` & `bcqa-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcqa
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Benchmark for Complex Heterogeneous Question answering
 Home-page: https://github.com/VenkteshV/BCQA
 Download-URL: 
 Author: Venktesh V, Deepali Prabhu
 Author-email: venkyviswa12@gmail.com
 License: Apache License 2.0
 Keywords: Information Retrieval Transformer Networks BERT PyTorch Complex Question Answering IR NLP deep learning
```

### Comparing `bcqa-1.1.0/README.md` & `bcqa-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/data/datastructures/answer.py` & `bcqa-1.1.1/bcqa/data/datastructures/answer.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/data/datastructures/dataset.py` & `bcqa-1.1.1/bcqa/data/datastructures/dataset.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/data/datastructures/evidence.py` & `bcqa-1.1.1/bcqa/data/datastructures/evidence.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/data/datastructures/hyperparameters/dpr.py` & `bcqa-1.1.1/bcqa/data/datastructures/hyperparameters/dpr.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/data/datastructures/hyperparameters/tapas.py` & `bcqa-1.1.1/bcqa/data/datastructures/hyperparameters/tapas.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/data/datastructures/sample.py` & `bcqa-1.1.1/bcqa/data/datastructures/sample.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/data/loaders/AmbigQADataLoader.py` & `bcqa-1.1.1/bcqa/data/loaders/AmbigQADataLoader.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/data/loaders/BaseDataLoader.py` & `bcqa-1.1.1/bcqa/data/loaders/BaseDataLoader.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/data/loaders/DataLoaderFactory.py` & `bcqa-1.1.1/bcqa/data/loaders/DataLoaderFactory.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/data/loaders/DprDataLoader.py` & `bcqa-1.1.1/bcqa/data/loaders/DprDataLoader.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/data/loaders/FinQADataLoader.py` & `bcqa-1.1.1/bcqa/data/loaders/FinQADataLoader.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/data/loaders/MusiqueQaDataLoader.py` & `bcqa-1.1.1/bcqa/data/loaders/MusiqueQaDataLoader.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/data/loaders/OTTQADataLoader.py` & `bcqa-1.1.1/bcqa/data/loaders/OTTQADataLoader.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/data/loaders/ReaderDataLoader.py` & `bcqa-1.1.1/bcqa/data/loaders/ReaderDataLoader.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/data/loaders/RetrieverDataset.py` & `bcqa-1.1.1/bcqa/data/loaders/RetrieverDataset.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/data/loaders/StrategyQADataLoader.py` & `bcqa-1.1.1/bcqa/data/loaders/StrategyQADataLoader.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/data/loaders/TATQADataLoader.py` & `bcqa-1.1.1/bcqa/data/loaders/TATQADataLoader.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/data/loaders/Tokenizer.py` & `bcqa-1.1.1/bcqa/data/loaders/Tokenizer.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/data/loaders/WikiMultihopQADataLoader.py` & `bcqa-1.1.1/bcqa/data/loaders/WikiMultihopQADataLoader.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/losses/DprNllLoss.py` & `bcqa-1.1.1/bcqa/losses/DprNllLoss.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/methods/ir/dense/dpr/indexer/annoyIndexer.py` & `bcqa-1.1.1/bcqa/methods/ir/dense/dpr/indexer/annoyIndexer.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/methods/ir/dense/dpr/indexer/faissIndexer.py` & `bcqa-1.1.1/bcqa/methods/ir/dense/dpr/indexer/faissIndexer.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/methods/ir/dense/dpr/indexer/indexer.py` & `bcqa-1.1.1/bcqa/methods/ir/dense/dpr/indexer/indexer.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/methods/ir/dense/dpr/models/bi_encoder.py` & `bcqa-1.1.1/bcqa/methods/ir/dense/dpr/models/bi_encoder.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/methods/ir/dense/dpr/models/dpr_sentence_transformers_inference.py` & `bcqa-1.1.1/bcqa/methods/ir/dense/dpr/models/dpr_sentence_transformers_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import List
 import torch
 import heapq
 from sentence_transformers import SentenceTransformer, util
 from bcqa.data.datastructures.evidence import Evidence
 from bcqa.data.datastructures.hyperparameters.dpr import DenseHyperParams
 from bcqa.data.datastructures.question import Question
-from methods.ir.dense.dpr.indexer.indexer import AnnSearch
-from metrics.SimilarityMatch import SimilarityMetric
+from bcqa.methods.ir.dense.dpr.indexer.indexer import AnnSearch
+from bcqa.metrics.SimilarityMatch import SimilarityMetric
 
 import gzip
 import logging
 
 logger = logging.getLogger(__name__)
```

### Comparing `bcqa-1.1.0/bcqa/methods/llms/flant5_engine.py` & `bcqa-1.1.1/bcqa/methods/llms/flant5_engine.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/methods/llms/llama_engine.py` & `bcqa-1.1.1/bcqa/methods/llms/llama_engine.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/methods/llms/llm_engine_orchestrator.py` & `bcqa-1.1.1/bcqa/methods/llms/llm_engine_orchestrator.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/methods/llms/openai_engine.py` & `bcqa-1.1.1/bcqa/methods/llms/openai_engine.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/metrics/ExactMatch.py` & `bcqa-1.1.1/bcqa/metrics/ExactMatch.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/metrics/MetricsBase.py` & `bcqa-1.1.1/bcqa/metrics/MetricsBase.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/metrics/SimilarityMatch.py` & `bcqa-1.1.1/bcqa/metrics/SimilarityMatch.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/metrics/retrieval/RetrievalMetrics.py` & `bcqa-1.1.1/bcqa/metrics/retrieval/RetrievalMetrics.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/metrics/retrieval/accuracy.py` & `bcqa-1.1.1/bcqa/metrics/retrieval/accuracy.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/re_ranker/CrossEncoder.py` & `bcqa-1.1.1/bcqa/re_ranker/CrossEncoder.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/re_ranker/ReRanker.py` & `bcqa-1.1.1/bcqa/re_ranker/ReRanker.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ANCE.py` & `bcqa-1.1.1/bcqa/retriever/ANCE.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/Baleen.py` & `bcqa-1.1.1/bcqa/retriever/Baleen.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/data/collection.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/data/collection.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/data/examples.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/data/examples.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/data/queries.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/data/queries.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/data/ranking.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/data/ranking.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/evaluation/load_model.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/evaluation/load_model.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/evaluation/loaders.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/evaluation/loaders.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/evaluation/metrics.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/index_updater.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/index_updater.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexer.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexer.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual_embeddings.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual_embeddings.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual_embeddings_strided.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/codecs/residual_embeddings_strided.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/collection_encoder.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/collection_encoder.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/collection_indexer.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/collection_indexer.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/index_manager.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/index_manager.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/index_saver.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/index_saver.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/loaders.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/loaders.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/indexing/utils.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/indexing/utils.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/infra/config/base_config.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/infra/config/base_config.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/infra/config/core_config.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/infra/config/core_config.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/infra/config/settings.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/infra/config/settings.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/infra/launcher.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/infra/launcher.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/infra/provenance.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/infra/provenance.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/infra/run.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/infra/run.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/base_colbert.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/base_colbert.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/checkpoint.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/checkpoint.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/colbert.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/colbert.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/hf_colbert.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/hf_colbert.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/reranker/electra.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/reranker/electra.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/reranker/tokenizer.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/reranker/tokenizer.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/tokenization/doc_tokenization.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/tokenization/doc_tokenization.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/tokenization/query_tokenization.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/tokenization/query_tokenization.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/modeling/tokenization/utils.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/modeling/tokenization/utils.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/search/candidate_generation.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/search/candidate_generation.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/search/index_loader.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/search/index_loader.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/search/index_storage.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/search/index_storage.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/search/strided_tensor.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/search/strided_tensor.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/search/strided_tensor_core.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/search/strided_tensor_core.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/searcher.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/searcher.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/trainer.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/trainer.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/training/eager_batcher.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/training/eager_batcher.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/training/lazy_batcher.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/training/lazy_batcher.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/training/rerank_batcher.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/training/rerank_batcher.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/training/training.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/training/training.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/colbert/training/utils.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/colbert/training/utils.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/server.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/server.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/setup.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/setup.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/utility/evaluate/annotate_EM.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/utility/evaluate/annotate_EM.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/utility/evaluate/annotate_EM_helpers.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/utility/evaluate/annotate_EM_helpers.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/utility/evaluate/evaluate_lotte_rankings.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/utility/evaluate/evaluate_lotte_rankings.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/utility/evaluate/msmarco_passages.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/utility/evaluate/msmarco_passages.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/utility/preprocess/docs2passages.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/utility/preprocess/docs2passages.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/utility/preprocess/queries_split.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/utility/preprocess/queries_split.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/utility/rankings/dev_subsample.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/utility/rankings/dev_subsample.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/utility/rankings/merge.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/utility/rankings/merge.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/utility/rankings/split_by_offset.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/utility/rankings/split_by_offset.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/utility/rankings/split_by_queries.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/utility/rankings/split_by_queries.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/utility/rankings/tune.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/utility/rankings/tune.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/utility/supervision/self_training.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/utility/supervision/self_training.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/utility/supervision/triples.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/utility/supervision/triples.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/utility/utils/dpr.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/utility/utils/dpr.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/utility/utils/qa_loaders.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/utility/utils/qa_loaders.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/ColBERT/utility/utils/save_metadata.py` & `bcqa-1.1.1/bcqa/retriever/ColBERT/utility/utils/save_metadata.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/DenseFullSearch.py` & `bcqa-1.1.1/bcqa/retriever/DenseFullSearch.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/HfRetriever.py` & `bcqa-1.1.1/bcqa/retriever/HfRetriever.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa/retriever/TCTColBERT.py` & `bcqa-1.1.1/bcqa/retriever/TCTColBERT.py`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/bcqa.egg-info/PKG-INFO` & `bcqa-1.1.1/bcqa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcqa
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Benchmark for Complex Heterogeneous Question answering
 Home-page: https://github.com/VenkteshV/BCQA
 Download-URL: 
 Author: Venktesh V, Deepali Prabhu
 Author-email: venkyviswa12@gmail.com
 License: Apache License 2.0
 Keywords: Information Retrieval Transformer Networks BERT PyTorch Complex Question Answering IR NLP deep learning
```

### Comparing `bcqa-1.1.0/bcqa.egg-info/SOURCES.txt` & `bcqa-1.1.1/bcqa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bcqa-1.1.0/setup.py` & `bcqa-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 optional_packages = {
     "tf" : ['tensorflow>=2.2.0', 'tensorflow-text', 'tensorflow-hub']
 }
 
 setup(
     name="bcqa",
-    version="1.1.0",
+    version="1.1.1",
     author="Venktesh V, Deepali Prabhu",
     author_email="venkyviswa12@gmail.com",
     description="A Benchmark for Complex Heterogeneous Question answering",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="Apache License 2.0",
     url="https://github.com/VenkteshV/BCQA",
```

