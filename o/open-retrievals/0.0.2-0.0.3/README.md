# Comparing `tmp/open-retrievals-0.0.2.tar.gz` & `tmp/open-retrievals-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-retrievals-0.0.2.tar", last modified: Mon Apr 15 11:13:43 2024, max compression
+gzip compressed data, was "open-retrievals-0.0.3.tar", last modified: Thu May  9 07:24:13 2024, max compression
```

## Comparing `open-retrievals-0.0.2.tar` & `open-retrievals-0.0.3.tar`

### file list

```diff
@@ -1,61 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.787568 open-retrievals-0.0.2/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11346 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-15 11:13:43.787568 open-retrievals-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-15 11:13:43.791568 open-retrievals-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.779568 open-retrievals-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.783568 open-retrievals-0.0.2/src/open_retrievals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-15 11:13:43.000000 open-retrievals-0.0.2/src/open_retrievals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-15 11:13:43.000000 open-retrievals-0.0.2/src/open_retrievals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:13:43.000000 open-retrievals-0.0.2/src/open_retrievals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:13:43.000000 open-retrievals-0.0.2/src/open_retrievals.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-15 11:13:43.000000 open-retrievals-0.0.2/src/open_retrievals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 11:13:43.000000 open-retrievals-0.0.2/src/open_retrievals.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.783568 open-retrievals-0.0.2/src/retrievals/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.783568 open-retrievals-0.0.2/src/retrievals/data/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/data/collator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/data/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.787568 open-retrievals-0.0.2/src/retrievals/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/arcface.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/bce.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/bpr.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/circle.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/cosent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/dice.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/infonce.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/margin_mse.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/pearson_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/r_drop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/simcse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/losses/triplet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.787568 open-retrievals-0.0.2/src/retrievals/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/metrics/mrr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.787568 open-retrievals-0.0.2/src/retrievals/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20893 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/models/embedding_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/models/pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/models/rag.py
--rw-r--r--   0 runner    (1001) docker     (127)     7033 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/models/rerank.py
--rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/models/retrieval_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.787568 open-retrievals-0.0.2/src/retrievals/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/tools/corpus_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/tools/langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/tools/llama_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/tools/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/tools/prompter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:43.787568 open-retrievals-0.0.2/src/retrievals/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/trainer/adversarial.py
--rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/trainer/custom_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/trainer/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-15 11:13:25.000000 open-retrievals-0.0.2/src/retrievals/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:24:13.604039 open-retrievals-0.0.3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11346 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-05-09 07:24:13.604039 open-retrievals-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-09 07:24:13.608039 open-retrievals-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:24:13.596039 open-retrievals-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:24:13.600039 open-retrievals-0.0.3/src/open_retrievals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-05-09 07:24:13.000000 open-retrievals-0.0.3/src/open_retrievals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-09 07:24:13.000000 open-retrievals-0.0.3/src/open_retrievals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:24:13.000000 open-retrievals-0.0.3/src/open_retrievals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:24:13.000000 open-retrievals-0.0.3/src/open_retrievals.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 07:24:13.000000 open-retrievals-0.0.3/src/open_retrievals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 07:24:13.000000 open-retrievals-0.0.3/src/open_retrievals.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:24:13.600039 open-retrievals-0.0.3/src/retrievals/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:24:13.600039 open-retrievals-0.0.3/src/retrievals/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/data/collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/data/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:24:13.604039 open-retrievals-0.0.3/src/retrievals/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/losses/arcface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/losses/bce.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/losses/bpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/losses/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/losses/cosent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/losses/cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/losses/dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/losses/infonce.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/losses/margin_mse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/losses/pearson_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/losses/r_drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/losses/simcse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/losses/triplet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:24:13.604039 open-retrievals-0.0.3/src/retrievals/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/metrics/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/metrics/mrr.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/metrics/ndcg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:24:13.604039 open-retrievals-0.0.3/src/retrievals/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23940 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/models/embedding_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/models/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/models/rag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/models/rerank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/models/retrieval_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:24:13.604039 open-retrievals-0.0.3/src/retrievals/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:24:13.604039 open-retrievals-0.0.3/src/retrievals/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/tools/corpus_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/tools/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/tools/llama_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/tools/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/tools/prompter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:24:13.604039 open-retrievals-0.0.3/src/retrievals/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/trainer/adversarial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/trainer/custom_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/trainer/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-09 07:23:58.000000 open-retrievals-0.0.3/src/retrievals/version.py
```

### Comparing `open-retrievals-0.0.2/LICENSE` & `open-retrievals-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.2/PKG-INFO` & `open-retrievals-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-retrievals
-Version: 0.0.2
+Version: 0.0.3
 Summary: Text Embeddings for Retrieval and RAG based on transformers
 Home-page: https://github.com/LongxingTan/open-retrievals
 Author: Longxing Tan
 Author-email: tanlongxing888@163.com
 License: Apache 2.0 License
 Keywords: NLP retrieval RAG rerank text embedding contrastive
 Platform: UNKNOWN
@@ -260,22 +260,22 @@
 ```
 
 **Search by Cosine similarity/KNN**
 ```python
 from retrievals import AutoModelForEmbedding, AutoModelForRetrieval
 
 query_texts = ['A dog is chasing car.']
-passage_texts = ['A man is playing a guitar.', 'A bee is flying low']
+document_texts = ['A man is playing a guitar.', 'A bee is flying low']
 model_name_or_path = "sentence-transformers/all-MiniLM-L6-v2"
 model = AutoModelForEmbedding(model_name_or_path)
 query_embeddings = model.encode(query_texts, convert_to_tensor=True)
-passage_embeddings = model.encode(passage_texts, convert_to_tensor=True)
+document_embeddings = model.encode(document_texts, convert_to_tensor=True)
 
 matcher = AutoModelForRetrieval(method='cosine')
-dists, indices = matcher.similarity_search(query_embeddings, passage_embeddings, top_k=1)
+dists, indices = matcher.similarity_search(query_embeddings, document_embeddings, top_k=1)
 ```
 
 ## Reference & Acknowledge
 - [sentence-transformers](https://github.com/UKPLab/sentence-transformers)
 - [FlagEmbedding](https://github.com/FlagOpen/FlagEmbedding)
 - [uniem](https://github.com/wangyuxinwhy/uniem)
 - [BCEmbedding](https://github.com/netease-youdao/BCEmbedding)
```

### Comparing `open-retrievals-0.0.2/README.md` & `open-retrievals-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -236,22 +236,22 @@
 ```
 
 **Search by Cosine similarity/KNN**
 ```python
 from retrievals import AutoModelForEmbedding, AutoModelForRetrieval
 
 query_texts = ['A dog is chasing car.']
-passage_texts = ['A man is playing a guitar.', 'A bee is flying low']
+document_texts = ['A man is playing a guitar.', 'A bee is flying low']
 model_name_or_path = "sentence-transformers/all-MiniLM-L6-v2"
 model = AutoModelForEmbedding(model_name_or_path)
 query_embeddings = model.encode(query_texts, convert_to_tensor=True)
-passage_embeddings = model.encode(passage_texts, convert_to_tensor=True)
+document_embeddings = model.encode(document_texts, convert_to_tensor=True)
 
 matcher = AutoModelForRetrieval(method='cosine')
-dists, indices = matcher.similarity_search(query_embeddings, passage_embeddings, top_k=1)
+dists, indices = matcher.similarity_search(query_embeddings, document_embeddings, top_k=1)
 ```
 
 ## Reference & Acknowledge
 - [sentence-transformers](https://github.com/UKPLab/sentence-transformers)
 - [FlagEmbedding](https://github.com/FlagOpen/FlagEmbedding)
 - [uniem](https://github.com/wangyuxinwhy/uniem)
 - [BCEmbedding](https://github.com/netease-youdao/BCEmbedding)
```

### Comparing `open-retrievals-0.0.2/setup.cfg` & `open-retrievals-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.2/setup.py` & `open-retrievals-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.2/src/open_retrievals.egg-info/PKG-INFO` & `open-retrievals-0.0.3/src/open_retrievals.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-retrievals
-Version: 0.0.2
+Version: 0.0.3
 Summary: Text Embeddings for Retrieval and RAG based on transformers
 Home-page: https://github.com/LongxingTan/open-retrievals
 Author: Longxing Tan
 Author-email: tanlongxing888@163.com
 License: Apache 2.0 License
 Keywords: NLP retrieval RAG rerank text embedding contrastive
 Platform: UNKNOWN
@@ -260,22 +260,22 @@
 ```
 
 **Search by Cosine similarity/KNN**
 ```python
 from retrievals import AutoModelForEmbedding, AutoModelForRetrieval
 
 query_texts = ['A dog is chasing car.']
-passage_texts = ['A man is playing a guitar.', 'A bee is flying low']
+document_texts = ['A man is playing a guitar.', 'A bee is flying low']
 model_name_or_path = "sentence-transformers/all-MiniLM-L6-v2"
 model = AutoModelForEmbedding(model_name_or_path)
 query_embeddings = model.encode(query_texts, convert_to_tensor=True)
-passage_embeddings = model.encode(passage_texts, convert_to_tensor=True)
+document_embeddings = model.encode(document_texts, convert_to_tensor=True)
 
 matcher = AutoModelForRetrieval(method='cosine')
-dists, indices = matcher.similarity_search(query_embeddings, passage_embeddings, top_k=1)
+dists, indices = matcher.similarity_search(query_embeddings, document_embeddings, top_k=1)
 ```
 
 ## Reference & Acknowledge
 - [sentence-transformers](https://github.com/UKPLab/sentence-transformers)
 - [FlagEmbedding](https://github.com/FlagOpen/FlagEmbedding)
 - [uniem](https://github.com/wangyuxinwhy/uniem)
 - [BCEmbedding](https://github.com/netease-youdao/BCEmbedding)
```

### Comparing `open-retrievals-0.0.2/src/open_retrievals.egg-info/SOURCES.txt` & `open-retrievals-0.0.3/src/open_retrievals.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,24 @@
 src/retrievals/losses/infonce.py
 src/retrievals/losses/margin_mse.py
 src/retrievals/losses/pearson_loss.py
 src/retrievals/losses/r_drop.py
 src/retrievals/losses/simcse.py
 src/retrievals/losses/triplet.py
 src/retrievals/metrics/__init__.py
+src/retrievals/metrics/map.py
 src/retrievals/metrics/mrr.py
+src/retrievals/metrics/ndcg.py
 src/retrievals/models/__init__.py
 src/retrievals/models/embedding_auto.py
 src/retrievals/models/pooling.py
 src/retrievals/models/rag.py
 src/retrievals/models/rerank.py
 src/retrievals/models/retrieval_auto.py
+src/retrievals/pipelines/__init__.py
 src/retrievals/tools/__init__.py
 src/retrievals/tools/corpus_processor.py
 src/retrievals/tools/langchain.py
 src/retrievals/tools/llama_index.py
 src/retrievals/tools/parser.py
 src/retrievals/tools/prompter.py
 src/retrievals/trainer/__init__.py
```

### Comparing `open-retrievals-0.0.2/src/retrievals/data/collator.py` & `open-retrievals-0.0.3/src/retrievals/data/collator.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,120 +4,134 @@
 from transformers import BatchEncoding, DataCollatorWithPadding, PreTrainedTokenizer
 
 
 class PairCollator(DataCollatorWithPadding):
     def __init__(
         self,
         tokenizer,
+        query_key: str = 'query',
+        positive_key: str = 'positive',
         max_length: Optional[int] = None,
         query_max_length: Optional[int] = None,
-        passage_max_length: Optional[int] = None,
+        document_max_length: Optional[int] = None,
     ) -> None:
         self.tokenizer = tokenizer
         if not hasattr(self.tokenizer, "pad_token_id") or self.tokenizer.pad_token is None:
             self.tokenizer.add_special_tokens({"pad_token": "[PAD]"})
 
+        self.query_key = query_key
+        self.positive_key = positive_key
+
         self.query_max_length: int
-        self.passage_max_length: int
+        self.document_max_length: int
         if query_max_length:
             self.query_max_length = query_max_length
         elif max_length:
             self.query_max_length = max_length
-            self.passage_max_length = max_length
+            self.document_max_length = max_length
         else:
             self.query_max_length = tokenizer.model_max_length
-            self.passage_max_length = tokenizer.model_max_length
+            self.document_max_length = tokenizer.model_max_length
 
-        if passage_max_length:
-            self.passage_max_length = passage_max_length
+        if document_max_length:
+            self.document_max_length = document_max_length
 
     def __call__(self, features: List[Dict[str, Any]]) -> Dict[str, Any]:
         assert (
-            'query' in features[0] and 'pos' in features[0]
-        ), "PairCollator should have 'query' and 'pos' keys in features dict"
+            self.query_key in features[0] and self.positive_key in features[0]
+        ), f"PairCollator should have {self.query_key} and {self.positive_key} in features dict, "
+        "you can set the custom key of query_key, positive_key during class init"
 
         query_texts = [feature["query"] for feature in features]
-        pos_texts = [feature["pos"] for feature in features]
+        pos_texts = [feature["positive"] for feature in features]
 
         query_inputs = self.tokenizer(
             query_texts,
             padding=True,
             max_length=self.query_max_length,
             truncation=True,
             return_tensors="pt",
         )
         pos_inputs = self.tokenizer(
             pos_texts,
             padding=True,
-            max_length=self.passage_max_length,
+            max_length=self.document_max_length,
             truncation=True,
             return_tensors="pt",
         )
 
         return {"query": query_inputs, "pos": pos_inputs}
 
 
 class TripletCollator(DataCollatorWithPadding):
     def __init__(
         self,
         tokenizer,
+        query_key: str = 'query',
+        positive_key: str = 'positive',
+        negative_key: Optional[str] = 'negative',
         max_length: Optional[int] = None,
         query_max_length: Optional[int] = None,
-        passage_max_length: Optional[int] = None,
+        document_max_length: Optional[int] = None,
     ) -> None:
         self.tokenizer = tokenizer
         if not hasattr(self.tokenizer, "pad_token_id") or self.tokenizer.pad_token is None:
             self.tokenizer.add_special_tokens({"pad_token": "[PAD]"})
 
+        self.query_key = query_key
+        self.positive_key = positive_key
+        self.negative_key = negative_key
+
         self.query_max_length: int
-        self.passage_max_length: int
+        self.document_max_length: int
         if query_max_length:
             self.query_max_length = query_max_length
         elif max_length:
             self.query_max_length = max_length
-            self.passage_max_length = max_length
+            self.document_max_length = max_length
         else:
             self.query_max_length = tokenizer.model_max_length
-            self.passage_max_length = tokenizer.model_max_length
+            self.document_max_length = tokenizer.model_max_length
 
-        if passage_max_length:
-            self.passage_max_length = passage_max_length
+        if document_max_length:
+            self.document_max_length = document_max_length
 
     def __call__(self, features: List[Dict[str, Any]]) -> Dict[str, Any]:
         assert (
-            'query' in features[0] and 'pos' in features[0] and 'neg' in features[0]
-        ), "TripletCollator should have 'query', 'pos' and 'neg' keys in features dict"
-
-        query_texts = [feature["query"] for feature in features]
-        pos_texts = [feature["pos"] for feature in features]
-        neg_texts = [feature["neg"] for feature in features]
+            self.positive_key in features[0] and self.positive_key in features[0] and self.negative_key in features[0]
+        ), f"TripletCollator should have {self.query_key}, {self.positive_key} and {self.negative_key} in features dict"
+        "you can set the custom key of query_key, positive_key and negative_key during class init"
+
+        query_texts = [feature[self.query_key] for feature in features]
+        pos_texts = [feature[self.positive_key] for feature in features]
+        neg_texts = [feature[self.negative_key] for feature in features]
 
         # if isinstance(query[0], list):
         #     query = sum(query, [])
-        # if isinstance(passage[0], list):
-        #     passage = sum(passage, [])
+        # if isinstance(document[0], list):
+        #     document = sum(document, [])
 
         query_inputs = self.tokenizer(
             query_texts,
             padding=True,
             max_length=self.query_max_length,
             truncation=True,
             return_tensors="pt",
         )
         pos_inputs = self.tokenizer(
             pos_texts,
             padding=True,
-            max_length=self.passage_max_length,
+            max_length=self.document_max_length,
             truncation=True,
             return_tensors="pt",
         )  # ["input_ids"]
         neg_inputs = self.tokenizer(
             neg_texts,
             padding=True,
-            max_length=self.passage_max_length,
+            max_length=self.document_max_length,
             truncation=True,
             return_tensors="pt",
         )  # ["input_ids"]
 
         return {
             "query": query_inputs,
             "pos": pos_inputs,
@@ -125,53 +139,59 @@
         }
 
 
 class RerankCollator(DataCollatorWithPadding):
     def __init__(
         self,
         tokenizer,
+        query_key: str = 'query',
+        document_key: str = 'document',
         max_length: Optional[int] = None,
         query_max_length: Optional[int] = None,
-        passage_max_length: Optional[int] = None,
+        document_max_length: Optional[int] = None,
     ):
         self.tokenizer = tokenizer
         if not hasattr(self.tokenizer, "pad_token_id") or self.tokenizer.pad_token is None:
             self.tokenizer.add_special_tokens({"pad_token": "[PAD]"})
 
+        self.query_key = query_key
+        self.document_key = document_key
+
         self.query_max_length: int
-        self.passage_max_length: int
+        self.document_max_length: int
         if query_max_length:
             self.query_max_length = query_max_length
         elif max_length:
             self.query_max_length = max_length
-            self.passage_max_length = max_length
+            self.document_max_length = max_length
         else:
             self.query_max_length = tokenizer.model_max_length
-            self.passage_max_length = tokenizer.model_max_length
+            self.document_max_length = tokenizer.model_max_length
 
-        if passage_max_length:
-            self.passage_max_length = passage_max_length
+        if document_max_length:
+            self.document_max_length = document_max_length
 
     def __call__(self, features: Union[List[Dict[str, Any]], List]) -> BatchEncoding:
         if isinstance(features[0], dict):
             assert (
-                'query' in features[0] and 'passage' in features[0]
-            ), "RerankCollator should have 'query' and 'passage' keys in features dict, and 'labels' during training"
+                self.query_key in features[0] and self.document_key in features[0]
+            ), f"RerankCollator should have {self.query_key} and {self.document_key} keys in features, "
+            "and 'labels' during training"
             query_texts = [feature["query"] for feature in features]
-            passage_texts = [feature['passage'] for feature in features]
+            document_texts = [feature['document'] for feature in features]
         else:
             query_texts = [feature[0] for feature in features]
-            passage_texts = [feature[1] for feature in features]
+            document_texts = [feature[1] for feature in features]
 
         labels = None
         if 'labels' in features[0].keys():
             labels = [feature['labels'] for feature in features]
 
         batch = self.tokenizer(
-            text=query_texts, text_pair=passage_texts, truncation=True, max_length=self.max_length, return_tensors="pt"
+            text=query_texts, text_pair=document_texts, truncation=True, max_length=self.max_length, return_tensors="pt"
         )
 
         # for key in ['input_ids', 'attention_mask']:
         #     batch[key] = torch.tensor(batch[key], dtype=torch.int64)
 
         if labels is not None:
             batch['labels'] = torch.tensor(batch['labels'], dtype=torch.float32)
```

### Comparing `open-retrievals-0.0.2/src/retrievals/data/dataset.py` & `open-retrievals-0.0.3/src/retrievals/data/dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import os
 import random
-from dataclasses import dataclass
 from typing import Iterable, List, Tuple
 
 import datasets
 from torch.utils.data import Dataset
 from transformers import DataCollatorWithPadding, PreTrainedTokenizer
 
 logger = logging.getLogger(__name__)
@@ -70,11 +69,11 @@
         logger.info("Loaded {} rerank data.".format(len(self.dataset)))
 
     def __len__(self):
         return len(self.dataset)
 
     def __getitem__(self, item):
         query = self.dataset[item]["query"]
-        passage = self.dataset[item]['passage']
+        document = self.dataset[item]['document']
         labels = self.dataset[item]['labels']
-        sample = {"query": query, "passage": passage, "neg": labels}
+        sample = {"query": query, "document": document, "neg": labels}
         return sample
```

### Comparing `open-retrievals-0.0.2/src/retrievals/losses/arcface.py` & `open-retrievals-0.0.3/src/retrievals/losses/arcface.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.2/src/retrievals/losses/bce.py` & `open-retrievals-0.0.3/src/retrievals/losses/bce.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.2/src/retrievals/losses/cosine_similarity.py` & `open-retrievals-0.0.3/src/retrievals/losses/triplet.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,80 @@
 """
-trainable temperature parameter: Text and Code Embeddings by Contrastive Pre-Training
+`FaceNet: A Unified Embedding for Face Recognition and Clustering
+<https://arxiv.org/abs/1503.03832>`_
 """
 
-import logging
+from typing import Optional
 
 import torch
-from torch import nn
+import torch.distributed as dist
+import torch.nn as nn
+import torch.nn.functional as F
 
-logger = logging.getLogger(__name__)
 
+class TripletLoss(nn.Module):
+    """
+    https://omoindrot.github.io/triplet-loss
+    """
 
-class CosineSimilarity(nn.Module):
-    def __init__(self, temperature: float = 0.0, dynamic_temperature=False):
+    def __init__(self, temperature: float = 0.05, negatives_cross_device: bool = False):
         super().__init__()
         self.temperature = temperature
-        self.dynamic_temperature = dynamic_temperature
+        self.negatives_cross_device = negatives_cross_device
+        if self.negatives_cross_device:
+            if not dist.is_initialized():
+                raise ValueError("Cannot do negatives_cross_device without distributed training")
+            self.rank = dist.get_rank()
+            self.world_size = dist.get_world_size()
+
+    def forward(
+        self,
+        query_embeddings: torch.Tensor,
+        pos_embeddings: torch.Tensor,
+        neg_embeddings: torch.Tensor,
+    ):
+        if self.negatives_cross_device:
+            # This gathers both negatives and positives.
+            # It could likely be optimized by only gathering negatives.
+            pos_embeddings = self._dist_gather_tensor(pos_embeddings)
+            neg_embeddings = self._dist_gather_tensor(neg_embeddings)
 
-    def forward(self, query_embeddings: torch.Tensor, passage_embeddings: torch.Tensor):
-        sim_pos_vector = torch.cosine_similarity(query_embeddings, passage_embeddings, dim=-1)
+        sim_pos_vector = torch.cosine_similarity(query_embeddings, pos_embeddings, dim=-1)
         sim_pos_vector = sim_pos_vector / self.temperature
         sim_neg_matrix = torch.cosine_similarity(
             query_embeddings.unsqueeze(1),
-            passage_embeddings.unsqueeze(0),
+            neg_embeddings.unsqueeze(0),
             dim=-1,
         )
         sim_neg_matrix = sim_neg_matrix / self.temperature
         sim_diff_matrix = sim_pos_vector.unsqueeze(1) - sim_neg_matrix
         loss = -torch.log(torch.sigmoid(sim_diff_matrix)).mean()
         return loss
 
-    def get_temperature(self):
-        if not self.dynamic_temperature:
-            return self.temperature
-        return torch.clamp(self.temperature, min=1e-3)
+    def _dist_gather_tensor(self, t: Optional[torch.Tensor]):
+        if t is None:
+            return None
+        t = t.contiguous()
 
+        all_tensors = [torch.empty_like(t) for _ in range(self.world_size)]
+        # All tensors have the same shape, as pooling already applied to them
+        dist.all_gather(all_tensors, t)
 
-class Similarity(nn.Module):
-    """
-    Dot product or cosine similarity
-    """
+        all_tensors[self.rank] = t
+        all_tensors = torch.cat(all_tensors, dim=0)
 
-    def __init__(self, temp=0.05):
+        return all_tensors
+
+
+class TripletCosineSimilarity(nn.Module):
+    def __init__(self, temperature: float = 0, margin: float = 0.50):
         super().__init__()
-        self.temp = temp
-        self.cos = nn.CosineSimilarity(dim=-1)
+        self.temperature = temperature
+        self.margin = margin
+        self.distance_metric = lambda x, y: F.pairwise_distance(x, y, p=2)
+
+    def forward(self, query_embedding: torch.Tensor, pos_embedding: torch.Tensor, neg_embedding: torch.Tensor):
+        distance_pos = self.distance_metric(query_embedding, pos_embedding)
+        distance_neg = self.distance_metric(query_embedding, neg_embedding)
 
-    def forward(self, x, y):
-        return self.cos(x, y) / self.temp
+        losses = F.relu(distance_pos - distance_neg + self.margin)
+        return losses.mean()
```

### Comparing `open-retrievals-0.0.2/src/retrievals/losses/focal_loss.py` & `open-retrievals-0.0.3/src/retrievals/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.2/src/retrievals/losses/infonce.py` & `open-retrievals-0.0.3/src/retrievals/losses/infonce.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,50 +11,59 @@
 import torch.nn as nn
 import torch.nn.functional as F
 
 logger = logging.getLogger(__name__)
 
 
 class InfoNCE(nn.Module):
+    """
+    https://github.com/RElbers/info-nce-pytorch
+    """
+
     def __init__(
         self,
         criterion: Union[nn.Module, Callable, None] = None,
-        scale: float = 1,
+        temperature: float = 0.02,
         negative_mode: str = "unpaired",
     ):
         super().__init__()
         self.criterion = criterion
-        self.scale = scale
+        self.temperature = temperature
         self.negative_mode = negative_mode
 
     def forward(
         self,
         query_embeddings: torch.Tensor,
         positive_embeddings: torch.Tensor,
         negative_embeddings: Optional[torch.Tensor] = None,
     ):
         query_embeddings = F.normalize(query_embeddings, dim=-1)
         positive_embeddings = F.normalize(positive_embeddings, dim=-1)
         device = query_embeddings.device
         if negative_embeddings is None:
-            logits1 = self.scale * query_embeddings @ positive_embeddings.T
+            logits1 = query_embeddings @ positive_embeddings.transpose(-2, -1)
             logits2 = logits1.T
             labels = torch.arange(len(logits1), dtype=torch.long, device=device)
-            loss = (self.criterion(logits1, labels) + self.criterion(logits2, labels)) / 2
+            loss = (
+                self.criterion(logits1 / self.temperature, labels) + self.criterion(logits2 / self.temperature, labels)
+            ) / 2
             return loss
         else:
             negative_embeddings = F.normalize(negative_embeddings, dim=-1)
             positive_logit = torch.sum(query_embeddings * positive_embeddings, dim=1, keepdim=True)
 
             if self.negative_mode == 'unpaired':
                 # Cosine between all query-negative combinations
                 negative_logits = query_embeddings @ negative_embeddings.transpose(-2, -1)
 
             elif self.negative_mode == 'paired':
                 query = query_embeddings.unsqueeze(1)
                 negative_logits = query @ negative_embeddings.transpose(-2, -1)
                 negative_logits = negative_logits.squeeze(1)
 
+            else:
+                raise ValueError(f"negative mode could chose 'unpaired' or 'paired', while got {self.negative_mode}")
+
             # First index in last dimension are the positive samples
             logits = torch.cat([positive_logit, negative_logits], dim=1)
             labels = torch.zeros(len(logits), dtype=torch.long, device=query_embeddings.device)
-            return self.criterion(logits, labels)
+            return self.criterion(logits / self.temperature, labels)
```

### Comparing `open-retrievals-0.0.2/src/retrievals/losses/margin_mse.py` & `open-retrievals-0.0.3/src/retrievals/losses/margin_mse.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.2/src/retrievals/losses/r_drop.py` & `open-retrievals-0.0.3/src/retrievals/losses/r_drop.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.2/src/retrievals/losses/simcse.py` & `open-retrievals-0.0.3/src/retrievals/losses/simcse.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,28 +10,32 @@
 import torch.nn.functional as F
 from torch import nn
 
 logger = logging.getLogger(__name__)
 
 
 class SimCSE(nn.Module):
-    def __init__(self, criterion: Union[nn.Module, Callable], temperature: float = 0.05):
+    def __init__(
+        self, criterion: Union[nn.Module, Callable], temperature: float = 0.05, dynamic_temperature: bool = False
+    ):
         super().__init__()
-        # TODO: dynamic_temperature
         self.criterion = criterion
         self.temperature = temperature
+        if dynamic_temperature:
+            # TODO: dynamic_temperature
+            self.temperature = nn.Parameter(torch.tensor(temperature))
 
     def forward(
         self,
         query_embeddings: torch.Tensor,
         pos_embeddings: torch.Tensor,
         neg_embeddings: Optional[torch.Tensor] = None,
     ):
         y_true = torch.arange(0, query_embeddings.size(0), device=query_embeddings.device)
 
         sim = F.cosine_similarity(query_embeddings.unsqueeze(1), pos_embeddings.unsqueeze(0), dim=2)
-        # sim = sim - torch.eye(y_pred.shape[0], device=device) * 1e12
+        # sim = sim - torch.eye(pos_embeddings.shape[0], device=query_embeddings.device) * 1e12
 
         sim = sim / self.temperature
         loss = self.criterion(sim, y_true)
         loss = torch.mean(loss)
         return loss
```

### Comparing `open-retrievals-0.0.2/src/retrievals/metrics/mrr.py` & `open-retrievals-0.0.3/src/retrievals/metrics/mrr.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.2/src/retrievals/models/embedding_auto.py` & `open-retrievals-0.0.3/src/retrievals/models/embedding_auto.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import logging
 from typing import Any, Callable, Dict, Iterable, List, Literal, Optional, Tuple, Union
 
-import faiss
 import numpy as np
+import pandas as pd
 import torch
 import torch.nn as nn
 from numpy import ndarray
 from torch.utils.data import DataLoader
 from tqdm.autonotebook import trange
 from transformers import (
     AutoConfig,
     AutoModel,
     AutoTokenizer,
     BatchEncoding,
     GenerationConfig,
 )
 
-from src.retrievals.models.pooling import AutoPooling
+from .pooling import AutoPooling
 
 logger = logging.getLogger(__name__)
 
 
 def get_device_name() -> Literal["mps", "cuda", "cpu"]:
     """
     Returns the name of the device where this module is running on.
@@ -64,55 +64,69 @@
     show_progress: bool = False
 
     def __init__(
         self,
         model_name_or_path: str,
         pretrained: bool = True,
         config_path: Optional[str] = None,
-        pooling_method: str = "cls",
+        pooling_method: Optional[str] = "cls",
         normalize_embeddings: bool = False,
         max_length: Optional[int] = None,
         loss_fn: Optional[Callable] = None,
         query_instruction: Optional[str] = None,
-        passage_instruction: Optional[str] = None,
+        document_instruction: Optional[str] = None,
+        hidden_dropout_prob: float = 0.1,
+        attention_dropout_prob: float = 0.1,
         generation_args: Dict = None,
         use_fp16: bool = False,
         use_lora: bool = False,
         lora_config=None,
         device: Optional[str] = None,
         trust_remote_code: bool = True,
+        **kwargs,
     ):
         super().__init__()
 
         self.tokenizer = AutoTokenizer.from_pretrained(
             model_name_or_path, return_tensors=False, trust_remote_code=trust_remote_code
         )
 
+        if config_path:
+            self.config = AutoConfig.from_pretrained(
+                config_path, output_hidden_states=True, trust_remote_code=trust_remote_code
+            )
+        elif hidden_dropout_prob > 0 or attention_dropout_prob > 0:
+            self.config = AutoConfig.from_pretrained(
+                model_name_or_path, output_hidden_states=True, trust_remote_code=trust_remote_code
+            )
+            self.config.update(
+                {"hidden_dropout_prob": hidden_dropout_prob, "attention_probs_dropout_prob": attention_dropout_prob}
+            )
+
         if pretrained:
-            self.model = AutoModel.from_pretrained(model_name_or_path, trust_remote_code=trust_remote_code)
+            self.model = AutoModel.from_pretrained(
+                model_name_or_path, config=self.config, trust_remote_code=trust_remote_code, **kwargs
+            )
         else:
-            if config_path is None:
-                self.config = AutoConfig.from_pretrained(
-                    model_name_or_path, output_hidden_states=True, trust_remote_code=trust_remote_code
-                )
-                self.model = AutoModel.from_config(self.config)
+            self.model = AutoModel.from_config(self.config)
         self.loss_fn = loss_fn
 
         if max_length is None:
             if (
                 hasattr(self.model, "config")
                 and hasattr(self.model.config, "max_position_embeddings")
                 and hasattr(self.tokenizer, "model_max_length")
             ):
                 max_length = min(self.model.config.max_position_embeddings, self.tokenizer.model_max_length)
 
         self.max_length = max_length
 
         if use_fp16:
             self.model.half()
+
         if use_lora:
             # peft config and wrapping
             from peft import LoraConfig, TaskType, get_peft_model
 
             if not lora_config:
                 raise ValueError("If use_lora is true, please provide a valid lora_config")
             self.model = get_peft_model(self.model, lora_config)
@@ -120,21 +134,21 @@
 
         if device is None:
             self.device = get_device_name()
         else:
             self.device = device
 
         self.normalize_embeddings = normalize_embeddings
-        self.pooling = AutoPooling(pooling_method)
+        self.pooling = AutoPooling(pooling_method) if pooling_method else None
 
         # self.fc = nn.Linear(768, 1)
         # self._init_weights(self.fc)
 
         self.query_instruction = query_instruction
-        self.passage_instruction = passage_instruction
+        self.document_instruction = document_instruction
         if generation_args is not None:
             generation_config = self.model.generation_config.to_dict()
             generation_config.update(generation_args)
             generation_config.update({"pad_token_id": self.tokenizer.pad_token_id})
             self.model.generation_config = GenerationConfig(**generation_config)
 
     def _init_weights(self, module: nn.Module):
@@ -172,23 +186,32 @@
         else:
             outputs = dict()
             loss_output = self.loss_fn(embeddings, labels)
             outputs["loss"] = loss_output["loss"]
             outputs["sentence_embedding"] = loss_output["sentence_embedding"]
             return outputs
 
-    def forward_from_loader(self, inputs):
+    def forward_from_loader(self, inputs, without_pooling: bool = False):
         model_output = self.model(inputs['input_ids'], inputs['attention_mask'])
-        if self.pooling is not None:
-            embeddings = self.pooling(model_output[0], inputs["attention_mask"])
+        if self.pooling is not None and not without_pooling:
+            if 'last_hidden_state' in model_output:
+                last_hidden_state = model_output['last_hidden_state']
+            elif 'hidden_states' not in model_output:
+                last_hidden_state = model_output[0]
+            else:
+                hidden_states = model_output['hidden_states']
+                # last_hidden_state = torch.cat([hidden_states[0], hidden_states[-1]])
+                last_hidden_state = (hidden_states[0] + hidden_states[-1]) / 2.0
+            embeddings = self.pooling(last_hidden_state, inputs["attention_mask"])
 
             if self.normalize_embeddings:
                 embeddings = torch.nn.functional.normalize(embeddings, p=2, dim=1)
 
             return embeddings
+        return model_output
 
     def forward_from_text(self, texts):
         batch_dict = self.tokenizer(
             texts,
             max_length=self.max_length,
             return_attention_mask=False,
             padding=False,
@@ -217,27 +240,27 @@
                 show_progress_bar=show_progress_bar,
                 output_value=output_value,
                 convert_to_numpy=convert_to_numpy,
                 convert_to_tensor=convert_to_tensor,
                 device=device,
                 normalize_embeddings=normalize_embeddings,
             )
-        elif isinstance(inputs, (str, List, Tuple)):
+        elif isinstance(inputs, (str, List, Tuple, pd.Series)):
             return self.encode_from_text(
                 sentences=inputs,
                 batch_size=batch_size,
                 show_progress_bar=show_progress_bar,
                 output_value=output_value,
                 convert_to_numpy=convert_to_numpy,
                 convert_to_tensor=convert_to_tensor,
                 device=device,
                 normalize_embeddings=normalize_embeddings,
             )
         else:
-            raise ValueError
+            raise ValueError(f'Input type: {type(inputs)}')
 
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         """Compute doc embeddings using a HuggingFace transformer model."""
         embeddings = self.encode(texts, show_progress_bar=self.show_progress, **self.encode_kwargs)
         return embeddings.tolist()
 
     def embed_query(self, text: str) -> List[float]:
@@ -259,15 +282,15 @@
                 embeddings = embeddings.detach()
                 if normalize_embeddings:
                     embeddings = torch.nn.functional.normalize(embeddings, p=2, dim=1)
                 if convert_to_numpy:
                     embeddings = embeddings.cpu()
                 all_embeddings.append(embeddings)
         if convert_to_numpy:
-            all_embeddings = np.asarray([emb.numpy() for emb in all_embeddings])
+            all_embeddings = np.concatenate([emb.numpy() for emb in all_embeddings], axis=0)
         else:
             all_embeddings = torch.concat(all_embeddings)
         return all_embeddings
 
     def encode_from_text(
         self,
         sentences: Union[str, List[str]],
@@ -377,14 +400,16 @@
 
         if input_was_string:
             all_embeddings = all_embeddings[0]
 
         return all_embeddings
 
     def build_index(self, inputs: BatchEncoding, batch_size: int = 128, use_gpu: bool = True):
+        import faiss
+
         embeddings = self.encode(inputs, batch_size=batch_size)
         embeddings = np.asarray(embeddings, dtype=np.float32)
         index = faiss.IndexFlatL2(len(embeddings[0]))
         if use_gpu:
             co = faiss.GpuMultipleClonerOptions()
             co.shard = True
             co.useFloat16 = True
@@ -434,14 +459,21 @@
         elif not hasattr(text, "__len__"):  # Object has no len() method
             return 1
         elif len(text) == 0 or isinstance(text[0], int):  # Empty string or list of ints
             return len(text)
         else:
             return sum([len(t) for t in text])  # Sum of length of individual strings
 
+    # @property
+    # def __dict__(self):
+    #     return self.model.__dict__
+
+    # def __getattr__(self, name):
+    #     return getattr(self.model, name)
+
 
 class PairwiseModel(AutoModelForEmbedding):
     """Pairwise Model wrapper
     - bi_encoder
     - cross_encoder
     - poly_encoder
     support: query + pos pair, or query + pos + neg triplet
@@ -452,65 +484,69 @@
         model_name_or_path: str,
         pooling_method: str = "cls",
         normalize_embeddings: bool = False,
         query_instruction: Optional[str] = None,
         use_fp16: bool = False,
         cross_encoder: bool = False,
         poly_encoder: bool = False,
-        temperature: float = 0,
-        dynamic_temperature: bool = False,
         loss_fn: Union[nn.Module, Callable] = None,
+        **kwargs,
     ) -> None:
         super().__init__(
             model_name_or_path=model_name_or_path,
             pooling_method=pooling_method,
             normalize_embeddings=normalize_embeddings,
             query_instruction=query_instruction,
             use_fp16=use_fp16,
             loss_fn=None,
+            **kwargs,
         )
         if loss_fn is not None:
-            logger.warning("loss_fn in Pairwise embed model, which will be ignored")
+            logger.warning("loss_fn in Pairwise model will be ignored")
 
         self.cross_encoder = cross_encoder
-        self.temperature = temperature
-        self.dynamic_temperature = dynamic_temperature
 
     def forward(
         self,
-        inputs: List[torch.Tensor],
+        inputs,
         labels: Optional[torch.LongTensor] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
     ):
-        input1 = inputs[0]
-        input2 = inputs[1]
-        if len(inputs) == 3:
-            input3 = inputs[2]
-
-        if self.cross_encoder:
-            ids1, mask1 = input1
-            ids2, mask2 = input2
-            ids = torch.cat([ids1, ids2], dim=0)
-            mask = torch.cat([mask1, mask2], dim=0)
-
-            transformer_out = super().forward({"input_ids": ids, "attention_mask": mask})
-            pooled_output = self.pooling(transformer_out[0], mask)
-            pooled_output1 = pooled_output[: len(ids1), :]
-            pooled_output2 = pooled_output[len(ids1) :, :]
-            return pooled_output1, pooled_output2
-        else:
-            # bi-encoder, pooling in each
-            pooled_output1 = super().forward(input1)
-            pooled_output2 = super().forward(input2)
+        if len(inputs) > 1 and len(inputs) <= 3:
+            input1 = inputs[0]
+            input2 = inputs[1]
             if len(inputs) == 3:
-                pooled_output3 = super().forward(input3)
-                return pooled_output1, pooled_output2, pooled_output3
-            return pooled_output1, pooled_output2
+                input3 = inputs[2]
+
+            if self.cross_encoder:
+                ids1, mask1 = input1['input_ids'], input1['attention_mask']
+                ids2, mask2 = input2['input_ids'], input2['attention_mask']
+                ids = torch.cat([ids1, ids2], dim=0)
+                mask = torch.cat([mask1, mask2], dim=0)
+
+                transformer_out = super().forward_from_loader(
+                    {"input_ids": ids, "attention_mask": mask}, without_pooling=True
+                )
+                pooled_output = self.pooling(transformer_out[0], mask)
+                pooled_output1 = pooled_output[: len(ids1), :]
+                pooled_output2 = pooled_output[len(ids1) :, :]
+                return pooled_output1, pooled_output2
+            else:
+                # bi-encoder, pooling in each
+                pooled_output1 = super().forward(input1)
+                pooled_output2 = super().forward(input2)
+                if len(inputs) == 3:
+                    pooled_output3 = super().forward(input3)
+                    return pooled_output1, pooled_output2, pooled_output3
+                return pooled_output1, pooled_output2
+        else:
+            pooled_output = super(PairwiseModel, self).forward(inputs)
+            return pooled_output
 
 
 def unsorted_segment_mean(data: torch.Tensor, segment_ids: torch.Tensor, num_segments: int) -> torch.Tensor:
     result_shape = (num_segments, data.size(1))
     segment_ids = segment_ids.unsqueeze(-1).expand(-1, data.size(1))
     result = data.new_full(result_shape, 0)  # init empty result tensor
     count = data.new_full(result_shape, 0)
@@ -520,19 +556,58 @@
 
 
 class ListwiseModel(AutoModelForEmbedding):
     """
     segment_id
     """
 
-    def __init__(self, **kwargs) -> None:
-        super().__init__(**kwargs)
+    def __init__(
+        self,
+        model_name_or_path: str,
+        pooling_method: str = "cls",
+        listwise_pooling: bool = False,
+        num_segments: Optional[int] = None,
+        normalize_embeddings: bool = False,
+        query_instruction: Optional[str] = None,
+        use_fp16: bool = False,
+        loss_fn: Union[nn.Module, Callable] = None,
+        **kwargs,
+    ) -> None:
+        super().__init__(
+            model_name_or_path=model_name_or_path,
+            pooling_method=pooling_method,
+            normalize_embeddings=normalize_embeddings,
+            query_instruction=query_instruction,
+            use_fp16=use_fp16,
+            loss_fn=loss_fn,
+            **kwargs,
+        )
+        self.pooling_method = pooling_method
+        self.num_segments = num_segments
 
     def forward(
         self,
         inputs,
         labels: Optional[torch.LongTensor] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
     ):
-        return
+        encoding = super().forward(inputs)
+
+        res = dict()
+        if self.pooling_method == 'unsorted_segment_mean':
+            encoding = unsorted_segment_mean(
+                encoding, segment_ids=inputs['segment_ids'], num_segments=self.num_segments
+            )
+            res['pred'] = self.fc(encoding[:, 1:])
+        else:
+            encodings = []
+            for i in range(self.num_segments):
+                mask_ = (inputs['segment_ids'] == i + 1).int()
+                encoding_ = self.pooling(encoding, mask_)
+                encoding_ = self.fc(encoding_)
+                encodings.append(encoding_)
+            res['pred'] = torch.stack(encodings, 1)
+
+        res['pred'] = res['pred'].squeeze(-1)
+        return res
```

### Comparing `open-retrievals-0.0.2/src/retrievals/models/pooling.py` & `open-retrievals-0.0.3/src/retrievals/models/pooling.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Any
-
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 
 class AutoPooling(nn.Module):
     def __init__(self, pooling_method: str, **kwargs) -> None:
@@ -28,35 +26,26 @@
         super().__init__()
 
     def forward(self, last_hidden_state: torch.Tensor, attention_mask: torch.Tensor) -> torch.Tensor:
         """
         last hidden state: First element of model_output contains all token embeddings
         """
         # last_hidden_state = model_output[0]
-        attention_mask = attention_mask.unsqueeze(-1).expand(last_hidden_state.size()).float()
+        attention_mask = attention_mask.unsqueeze(-1).float()
         sum_embeddings = torch.sum(last_hidden_state * attention_mask, 1)
         sum_mask = torch.clamp(attention_mask.sum(1), min=1e-9)
         mean_embeddings = sum_embeddings / sum_mask
         return mean_embeddings
 
 
-class AttentionPooling(nn.Module):
-    def __init__(self):
-        super(AttentionPooling, self).__init__()
-
-    def forward(self, last_hidden_state: torch.Tensor, attention_mask: torch.Tensor) -> torch.Tensor:
-        return last_hidden_state[:, 0, :]
-
-
 class ClsTokenPooling(nn.Module):
     """CLS Pooling"""
 
     def __init__(self):
         super().__init__()
-        self.feat_mult = 1
 
     def forward(
         self,
         last_hidden_state: torch.Tensor,
         attention_mask: torch.Tensor,
     ) -> torch.Tensor:
         # Take embeddings of first token per sample
@@ -86,14 +75,22 @@
             emb = last_hidden_state[
                 torch.arange(batch_size, device=last_hidden_state.device),
                 sequence_lengths,
             ]
         return emb
 
 
+class AttentionPooling(nn.Module):
+    def __init__(self):
+        super(AttentionPooling, self).__init__()
+
+    def forward(self, last_hidden_state: torch.Tensor, attention_mask: torch.Tensor) -> torch.Tensor:
+        return last_hidden_state[:, 0, :]
+
+
 class WeightedLayerPooling(nn.Module):
     def __init__(self, num_hidden_layers: int, layer_start: int = 4, layer_weights=None):
         super().__init__()
         self.layer_start = layer_start
         self.num_hidden_layers = num_hidden_layers
         self.layer_weights = (
             layer_weights
@@ -114,21 +111,19 @@
     """
 
     def __init__(self, dim, p: int = 3, eps: float = 1e-6):
         super(GeMText, self).__init__()
         self.dim = dim
         self.p = nn.Parameter(torch.ones(1) * p)
         self.eps = eps
-        self.feat_mult = 1
 
     def forward(
         self,
         x: torch.Tensor,
         attention_mask: torch.Tensor,
-        input_ids: torch.Tensor,
     ) -> torch.Tensor:
         attention_mask_expanded = attention_mask.unsqueeze(-1).expand(x.shape)
         x = (x.clamp(min=self.eps) * attention_mask_expanded).pow(self.p).sum(self.dim)
         ret = x / attention_mask_expanded.sum(self.dim).clip(min=self.eps)
         ret = ret.pow(1 / self.p)
         return ret
```

### Comparing `open-retrievals-0.0.2/src/retrievals/models/rag.py` & `open-retrievals-0.0.3/src/retrievals/models/rag.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.2/src/retrievals/models/rerank.py` & `open-retrievals-0.0.3/src/retrievals/models/rerank.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from transformers import (
     AutoConfig,
     AutoModel,
     AutoModelForSequenceClassification,
     AutoTokenizer,
 )
 
-from src.retrievals.data.collator import RerankCollator
-from src.retrievals.models.embedding_auto import get_device_name
-from src.retrievals.models.pooling import AutoPooling
+from ..data.collator import RerankCollator
+from .embedding_auto import get_device_name
+from .pooling import AutoPooling
 
 logger = logging.getLogger(__name__)
 
 
 class RerankModel(nn.Module):
     def __init__(
         self,
@@ -85,40 +85,44 @@
             if module.padding_idx is not None:
                 module.weight.data[module.padding_idx].zero_()
         elif isinstance(module, nn.LayerNorm):
             module.bias.data.zero_()
             module.weight.data.fill_(1.0)
 
     def encode(self, input_ids: torch.Tensor, attention_mask: torch.Tensor) -> torch.Tensor:
-        outputs = self.model(input_ids, attention_mask, output_hidden_states=False)
-        encoder_layer = outputs.last_hidden_state
-        embeddings = self.pooling(encoder_layer, attention_mask)
+        outputs = self.model(input_ids, attention_mask, output_hidden_states=True)
+        if hasattr(outputs, 'last_hidden_state'):
+            hidden_state = outputs.last_hidden_state
+            embeddings = self.pooling(hidden_state, attention_mask)
+        else:
+            hidden_state = outputs.hidden_states[1]
+            embeddings = self.pooling(hidden_state, attention_mask)
         return embeddings
 
     def forward(
         self,
         input_ids: torch.Tensor,
-        attention_mask: torch.Tensor,
+        attention_mask: Optional[torch.Tensor] = None,
         labels: Optional[torch.Tensor] = None,
-        return_dict: Optional[bool] = False,
+        return_dict: Optional[bool] = True,
         **kwargs,
     ) -> Union[Dict[str, torch.Tensor], torch.Tensor]:
         features = self.encode(input_ids=input_ids, attention_mask=attention_mask)
         logits = self.classifier(features).reshape(-1)
 
         if return_dict:
             outputs_dict = dict()
             outputs_dict['logits'] = logits
 
         if labels is not None:
             if not self.loss_fn:
                 logger.warning('loss_fn is not setup, use BCEWithLogitsLoss')
                 self.loss_fn = nn.BCEWithLogitsLoss(reduction='mean')
 
-            loss = self.loss_fn(logits, labels)
+            loss = self.loss_fn(logits, labels.float())
             if return_dict:
                 outputs_dict['loss'] = loss
                 return outputs_dict
             else:
                 return logits, loss
         else:
             return logits
@@ -141,51 +145,51 @@
 
         if not data_collator:
             data_collator = RerankCollator(tokenizer=self.tokenizer)
 
         with torch.no_grad():
             scores_list: List = []
             for i in range(0, len(text), batch_size):
-                text_batch = [{'query': text[i], 'passage': text_pair[i]} for i in range(i, i + batch_size)]
+                text_batch = [{'query': text[i], 'document': text_pair[i]} for i in range(i, i + batch_size)]
                 batch = data_collator(text_batch)
                 scores = (
                     self.model(batch['input_ids'], batch['attention_mask'], return_dict=True).logits.view(-1).float()
                 )
                 scores = torch.sigmoid(scores)
                 scores_list.extend(scores.cpu().numpy().tolist())
 
         return scores_list
 
     def rerank(
         self,
         query: Union[List[str], str],
-        passages: List[str],
+        document: List[str],
         data_collator: Optional[RerankCollator] = None,
         batch_size: int = 32,
         show_progress_bar: bool = None,
         return_dict: bool = True,
         **kwargs,
     ):
-        merge_scores = self.compute_score(query, passages, data_collator, batch_size, show_progress_bar)
+        merge_scores = self.compute_score(query, document, data_collator, batch_size, show_progress_bar)
 
         merge_scores_argsort = np.argsort(merge_scores)[::-1]
-        sorted_passages = []
+        sorted_document = []
         sorted_scores = []
         for mid in merge_scores_argsort:
             sorted_scores.append(merge_scores[mid])
-            sorted_passages.append(passages[mid])
+            sorted_document.append(document[mid])
 
         if return_dict:
             return {
-                'rerank_passages': sorted_passages,
+                'rerank_document': sorted_document,
                 'rerank_scores': sorted_scores,
                 'rerank_ids': merge_scores_argsort.tolist(),
             }
         else:
-            return sorted_passages
+            return sorted_document
 
     def save(self, path: str):
         """
         Saves all model and tokenizer to path
         """
         if path is None:
             return
```

### Comparing `open-retrievals-0.0.2/src/retrievals/models/retrieval_auto.py` & `open-retrievals-0.0.3/src/retrievals/models/retrieval_auto.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,97 +1,134 @@
 import logging
-from typing import Optional, Union
+from typing import Literal, Optional, Union
 
-import faiss
 import numpy as np
 import pandas as pd
 import torch
 from sklearn.neighbors import NearestNeighbors
 from tqdm import tqdm
 from tqdm.autonotebook import trange
 
 logger = logging.getLogger(__name__)
 
 
 class AutoModelForRetrieval(object):
-    def __init__(self, method: str = "cosine") -> None:
+    def __init__(self, method: Literal['cosine', 'knn', None] = "cosine") -> None:
         super().__init__()
         self.method = method
 
     def similarity_search(
         self,
         query_embed: torch.Tensor,
-        passage_embed: Optional[torch.Tensor] = None,
+        document_embed: Optional[torch.Tensor] = None,
         index_path: Optional[str] = None,
         top_k: int = 1,
         batch_size: int = -1,
         convert_to_numpy: bool = True,
-        convert_to_pandas: bool = False,
         **kwargs,
     ):
-        if passage_embed is None and index_path is None:
-            logging.warning('Please provide passage_embed for knn/tensor search or index_path for faiss search')
+        self.top_k = top_k
+        if document_embed is None and index_path is None:
+            logging.warning('Please provide document_embed for knn/tensor search or index_path for faiss search')
             return
         if index_path is not None:
+            import faiss
+
             faiss_index = faiss.read_index(index_path)
             dists, indices = faiss_search(
                 query_embeddings=query_embed,
                 faiss_index=faiss_index,
                 top_k=top_k,
                 batch_size=batch_size,
             )
 
         elif self.method == "knn":
             neighbors_model = NearestNeighbors(n_neighbors=top_k, metric="cosine", n_jobs=-1)
-            neighbors_model.fit(passage_embed)
+            neighbors_model.fit(document_embed)
             dists, indices = neighbors_model.kneighbors(query_embed)
 
         elif self.method == "cosine":
             dists, indices = cosine_similarity_search(
-                query_embed, passage_embed, top_k=top_k, batch_size=batch_size, convert_to_numpy=convert_to_numpy
+                query_embed, document_embed, top_k=top_k, batch_size=batch_size, convert_to_numpy=convert_to_numpy
             )
 
         else:
             raise ValueError(f"Only cosine and knn method are supported by similarity_search, while get {self.method}")
 
-        if not convert_to_pandas:
-            return dists, indices
+        return dists, indices
+
+    def get_pandas_candidate(self, query_ids, document_ids, dists, indices):
+        if isinstance(query_ids, pd.Series):
+            query_ids = query_ids.values
+        if isinstance(document_ids, pd.Series):
+            document_ids = document_ids.values
+
+        retrieval = {
+            'query_id': np.repeat(query_ids, self.top_k),
+            'document_id': document_ids[indices.ravel()],
+            'score': dists.ravel(),
+        }
+        return pd.DataFrame(retrieval)
+
+    def get_rerank_data(self, pred_df):
+        logger.info('Generate rerank samples based on the retrieval prediction with: query_id, document_ids, pred_ids')
+
+        samples = []
+        for _, row in tqdm(pred_df.iterrows(), total=len(pred_df)):
+            query_id = row['query_id']
+            document_ids = row['document_ids']
+            if pd.isna(row['pred_ids']):
+                print(' Error 1 , no pred_ids ...')
+                continue
+            else:
+                pred_ids_list = row['pred_ids'].split()
 
-        retrieval = dict({'query': [], 'passage': [], 'labels': []})
-        return pd.from_dict(retrieval)
+            if pd.isna(document_ids):
+                print(' Error 2 , no label document_ids ...')
+                for id in pred_ids_list:
+                    samples.append({'query_id': query_id, 'document_id': id, 'label': 0})
+            else:
+                documents = document_ids.split()
+                for id in pred_ids_list:
+                    if id not in documents:
+                        samples.append({'query_id': query_id, 'document_id': id, 'label': 0})
+                    else:
+                        samples.append({'query_id': query_id, 'document_id': id, 'label': 1})
+
+        return pd.DataFrame(samples)
 
 
 class EnsembleRetriever(object):
     def __init__(self, retrievers, weights=None):
         pass
 
 
 def cosine_similarity_search(
     query_embed: torch.Tensor,
-    passage_embed: torch.Tensor,
+    document_embed: torch.Tensor,
     top_k: int = 1,
     batch_size: int = 128,
     penalty: bool = True,
     temperature: float = 0,
     convert_to_numpy: bool = True,
     show_progress_bar: bool = None,
 ):
     if len(query_embed.size()) == 1:
         query_embed = query_embed.view(1, -1)
-    assert query_embed.size()[1] == passage_embed.size()[1], (
-        f"The embed Shape of query_embed and passage_embed should be same, "
-        f"while received query {query_embed.size()} and passage {passage_embed.size()}"
+    assert query_embed.size()[1] == document_embed.size()[1], (
+        f"The embed Shape of query_embed and document_embed should be same, "
+        f"while received query {query_embed.size()} and document {document_embed.size()}"
     )
     chunk = batch_size if batch_size > 0 else len(query_embed)
     embeddings_chunks = query_embed.split(chunk)
 
     dists = []
     indices = []
     for idx in trange(0, len(embeddings_chunks), desc="Batches", disable=not show_progress_bar):
-        cos_sim_chunk = torch.matmul(embeddings_chunks[idx], passage_embed.transpose(0, 1))
+        cos_sim_chunk = torch.matmul(embeddings_chunks[idx], document_embed.transpose(0, 1))
         cos_sim_chunk = torch.nan_to_num(cos_sim_chunk, nan=0.0)
         # if penalty:
         #     pen = ((contents["old_source_count"].values==0) & (contents["old_nonsource_count"].values==1))
         #     cos_sim_chunk = cos_sim_chunk.clamp(0,1) ** torch.Tensor((1 + pen*0.5).reshape(1,-1)).to(DEVICE)
         #     cos_sim_chunk = cos_sim_chunk.clamp(0,1) ** torch.Tensor((1-(contents["old_count"].values==0)*0.1).
         #     reshape(1,-1)).to(DEVICE)
         if temperature:
@@ -106,15 +143,15 @@
         dists = dists.numpy()
         indices = indices.numpy()
     return dists, indices
 
 
 def faiss_search(
     query_embeddings,
-    faiss_index: faiss.Index,
+    faiss_index,
     top_k: int = 100,
     batch_size: int = 128,
     max_length: int = 512,
 ):
     """
     1. Encode queries into dense embeddings;
     2. Search through faiss index
@@ -133,61 +170,7 @@
         score, index = faiss_index.search(query_embedding.astype(np.float32), k=top_k)
         all_scores.append(score)
         all_indices.append(index)
 
     all_scores = np.concatenate(all_scores, axis=0)
     all_indices = np.concatenate(all_indices, axis=0)
     return all_scores, all_indices
-
-
-class FaissIndex:
-    def __init__(self, device) -> None:
-        if isinstance(device, torch.device):
-            if device.index is None:
-                device = "cpu"
-            else:
-                device = device.index
-        self.device = device
-
-    def build(self, encoded_corpus, index_factory, metric):
-        if metric == "l2":
-            metric = faiss.METRIC_L2
-        elif metric in ["ip", "cos"]:
-            metric = faiss.METRIC_INNER_PRODUCT
-        else:
-            raise NotImplementedError(f"Metric {metric} not implemented!")
-
-        index = faiss.index_factory(encoded_corpus.shape[1], index_factory, metric)
-
-        if self.device != "cpu":
-            co = faiss.GpuClonerOptions()
-            co.useFloat16 = True
-            # logger.info("using fp16 on GPU...")
-            index = faiss.index_cpu_to_gpu(faiss.StandardGpuResources(), self.device, index, co)
-
-        logging.info("training index...")
-        index.train(encoded_corpus)
-        logging.info("adding embeddings...")
-        index.add(encoded_corpus)
-        self.index = index
-        return index
-
-    def load(self, index_path):
-        logging.info(f"loading index from {index_path}...")
-        index = faiss.read_index(index_path)
-        if self.device != "cpu":
-            co = faiss.GpuClonerOptions()
-            co.useFloat16 = True
-            index = faiss.index_cpu_to_gpu(faiss.StandardGpuResources(), self.device, index, co)
-        self.index = index
-        return index
-
-    def save(self, index_path):
-        logging.info(f"saving index at {index_path}...")
-        if isinstance(self.index, faiss.GpuIndex):
-            index = faiss.index_gpu_to_cpu(self.index)
-        else:
-            index = self.index
-        faiss.write_index(index, index_path)
-
-    def search(self, query, hits):
-        return self.index.search(query, k=hits)
```

### Comparing `open-retrievals-0.0.2/src/retrievals/tools/langchain.py` & `open-retrievals-0.0.3/src/retrievals/tools/langchain.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     MarkdownHeaderTextSplitter,
     MarkdownTextSplitter,
 )
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.pydantic_v1 import Extra, root_validator
 
-from src.retrievals.models.embedding_auto import AutoModelForEmbedding
-from src.retrievals.models.rerank import RerankModel
+from ..models.embedding_auto import AutoModelForEmbedding
+from ..models.rerank import RerankModel
 
 
 class LangchainEmbedding(AutoModelForEmbedding, Embeddings):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `open-retrievals-0.0.2/src/retrievals/tools/llama_index.py` & `open-retrievals-0.0.3/src/retrievals/tools/llama_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from llama_index.bridge.pydantic import Field, PrivateAttr
 from llama_index.callbacks import CBEventType, EventPayload
 from llama_index.postprocessor.types import BaseNodePostprocessor
 from llama_index.schema import MetadataMode, NodeWithScore, QueryBundle
 from llama_index.utils import infer_torch_device
 
-from src.retrievals import RerankModel
+from ..models.rerank import RerankModel
 
 
 class LlamaIndexReranker(BaseNodePostprocessor):
     model: str = Field(ddescription="Sentence transformer model name.")
     top_n: int = Field(description="Number of nodes to return sorted by score.")
     _model: Any = PrivateAttr()
```

### Comparing `open-retrievals-0.0.2/src/retrievals/tools/parser.py` & `open-retrievals-0.0.3/src/retrievals/tools/parser.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.2/src/retrievals/tools/prompter.py` & `open-retrievals-0.0.3/src/retrievals/tools/prompter.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.2/src/retrievals/trainer/adversarial.py` & `open-retrievals-0.0.3/src/retrievals/trainer/adversarial.py`

 * *Files identical despite different names*

### Comparing `open-retrievals-0.0.2/src/retrievals/trainer/custom_trainer.py` & `open-retrievals-0.0.3/src/retrievals/trainer/custom_trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 import gc
 import logging
 import math
 import time
-from typing import Callable, Dict, List, Optional, Tuple, Union
+from typing import Callable, Dict, List, Literal, Optional, Tuple, Union
 
 import numpy as np
 import torch
+
+# from accelerate import Accelerator
+# from accelerate.logging import get_logger
+# from accelerate.utils import set_seed
 from torch import nn
 from tqdm import tqdm
 
+from .adversarial import AWP, EMA, FGM
+
 logger = logging.getLogger(__name__)
 
 
 def train_fn(
-    epoch,
-    model,
+    epoch: int,
+    model: nn.Module,
     train_loader,
     optimizer,
-    criterion=None,
+    criterion: Optional[Callable] = None,
     apex: bool = False,
     gradient_accumulation_steps: int = 1,
     max_grad_norm: float = 1,
     data_collator=None,
     batch_scheduler=None,
     fgm=None,
     awp=None,
     ema_inst=None,
     print_freq: int = 100,
     wandb: bool = False,
     device: str = "cuda",
+    teacher=None,
+    teacher_loss: Optional[Callable] = None,
     **kwargs,
 ):
+    start = time.time()
     model.train()
     scaler = torch.cuda.amp.GradScaler(enabled=apex)
     losses = AverageMeter()
-    start = time.time()
     global_step = 0
     save_step = int(len(train_loader) / 1)
 
     # loss_list = []
     # metrics_list = []
 
     for step, (inputs, labels) in enumerate(train_loader):
@@ -59,68 +67,79 @@
             if criterion is None:
                 preds = model(inputs, labels)
             else:
                 preds = model(inputs)
             if isinstance(preds, dict) and "loss" in preds:
                 loss = preds["loss"]
             else:
-                loss = criterion(preds[0], preds[1])
+                if isinstance(inputs, dict) and 'weights' in inputs:
+                    loss = criterion(preds[0], labels, inputs['weights'])
+                else:
+                    loss = criterion(preds[0], preds[1])
+
+        if teacher:
+            with torch.no_grad():
+                teacher_output = teacher(inputs)
+                loss_distill = teacher_loss(preds, teacher_output)
+                loss = loss_distill
 
         if gradient_accumulation_steps > 1:
             loss = loss / gradient_accumulation_steps
+
         losses.update(loss.item(), batch_size)
         scaler.scale(loss).backward()
 
         # if isinstance(preds, dict):
         #     acc = (preds["feature"].softmax(dim=1) * (labels > 0)).sum(axis=1).mean()
         # else:
         #     acc = (preds.softmax(dim=1) * (labels > 0)).sum(axis=1).mean()
         # acc = acc.detach().cpu().item()
         # acc_list.append(acc)
 
+        # ---------------------fgm-------------
         if fgm:
             fgm.attack(epsilon=1.0)  # embedding被修改
             with torch.cuda.amp.autocast(enabled=apex):
                 preds = model(inputs)
                 if isinstance(preds, dict) and "loss" in preds:
                     loss_avg = preds["loss"]
                 else:
                     loss_avg = criterion(preds, labels)
             if gradient_accumulation_steps > 1:
                 loss_avg = loss_avg / gradient_accumulation_steps
             losses.update(loss_avg.item(), batch_size)
             scaler.scale(loss_avg).backward()
             fgm.restore()  # 恢复Embedding参数
-        # ---------------------fgm-------------
 
         grad_norm = torch.nn.utils.clip_grad_norm_(model.parameters(), max_grad_norm)
+
         if (step + 1) % gradient_accumulation_steps == 0:
             scaler.step(optimizer)
             scaler.update()
 
             if ema_inst:
                 ema_inst.update()
 
             optimizer.zero_grad()
             global_step += 1
             if batch_scheduler:
                 batch_scheduler.step()
 
-        if step % print_freq == 0 or step == (len(train_loader) - 1):
+        if step % print_freq == 0 or (step + 1) == len(train_loader):
             print(
                 "Epoch: [{0}][{1}/{2}] "
                 "Elapsed {remain:s} "
                 "Loss: {loss.val:.4f}({loss.avg:.4f}) "
                 "Grad: {grad_norm:.4f}  "
                 "LR: {lr:.8f}  "
                 # "ACC: {acc: .4f}"
                 .format(
                     epoch + 1,
                     step,
-                    len(train_loader),
+                    len(train_loader) - 1,
                     remain=timeSince(start, float(step + 1) / len(train_loader)),
                     loss=losses,
                     grad_norm=grad_norm,
                     lr=batch_scheduler.get_lr()[0] if batch_scheduler else optimizer.param_groups[0]["lr"],
                     # acc=np.mean(acc_list),
                 )
             )
@@ -166,15 +185,15 @@
         batch_size = labels.size(0)
         with torch.cuda.amp.autocast(enabled=apex):
             try:
                 preds = model(inputs, labels=labels)
             except ValueError:
                 preds = model(inputs)
             else:
-                print('inputs of model should be with or without labels')
+                logger.warning('inputs of model should be with or without labels')
 
             if isinstance(preds, dict) and "loss" in preds:
                 loss = preds["loss"]
                 pred = preds["output"]
             else:
                 loss = criterion(preds, labels)
                 pred = preds
@@ -219,47 +238,69 @@
             y_preds = model(inputs)
         preds.append(y_preds.sigmoid().squeeze().to("cpu").numpy().reshape(-1))
     predictions = np.concatenate(preds)
     return predictions
 
 
 class CustomTrainer(object):
-    def __init__(self, model: Union[str, nn.Module], device=None, apex=False, teacher=None):
+    def __init__(self, model: Union[nn.Module], device: Optional[str] = None, apex: bool = False, teacher=None):
         if not device:
             device = "cuda" if torch.cuda.is_available() else "cpu"
         self.device = device
         self.model = model
-        self.teacher = teacher
         self.apex = apex
-        self.train_step = train_fn
-        self.valid_step = valid_fn
+        self.train_fn = train_fn
+        self.valid_fn = valid_fn
+        if teacher:
+            self.teacher = teacher.eval()
+            self.teacher_loss = torch.nn.MSELoss()
 
     def train(
         self,
         train_loader,
         optimizer,
         epochs=10,
         criterion=None,
         scheduler=None,
         valid_loader=None,
         eval_metrics=None,
         data_collator=None,
         max_grad_norm=10,
+        use_fgm: bool = False,
+        use_awp: bool = False,
+        ema_decay: float = 0,
+        dynamic_margin_fn: Optional[Callable] = None,
+        gradient_checkpointing: bool = False,
+        resume_from_checkpoint: Optional[Union[str, bool]] = None,
         **kwargs,
     ):
-        # best_score = 0
-        # fgm = FGM(model)
-        # awp = None
-        # ema_inst = EMA(model, 0.999)
-        # ema_inst.register()
+        logger.info('-------START TO TRAIN-------')
+        if resume_from_checkpoint is not None:
+            checkpoint = torch.load(resume_from_checkpoint)
+            self.model.load_state_dict(checkpoint)
+
+        if use_fgm:
+            logger.info('[FGM] Use FGM adversarial')
+            fgm = FGM(self.model.to(self.device))
+        elif use_awp:
+            logger.info('[AWP] Use AWP adversarial')
+            awp = AWP(self.model.to(self.device), optimizer)
+
+        if ema_decay > 0:
+            logger.info('[EMA] Use EMA while training')
+            ema_inst = EMA(self.model.to(self.device), ema_decay)
+            ema_inst.register()
+
+        if gradient_checkpointing:
+            self.model.gradient_checkpointing_enable()
 
         for epoch in range(epochs):
-            if "dynamic_margin" in kwargs.keys():
-                margin = min(0.1 + epoch * 0.02, 0.4)
-                logger.info(f"Epoch: {epoch}, Margin: {margin}")
+            if dynamic_margin_fn:
+                margin = dynamic_margin_fn(epoch)
+                logger.info(f"[Dynamic margin] Epoch: {epoch}, Margin: {margin}")
                 if criterion:
                     criterion.set_margin(margin)
                 elif self.model.loss_fn is not None:
                     self.model.loss_fn.set_margin(margin)
                 else:
                     raise ValueError(
                         'dynamic margin is True, but criterion of trainer and loss_fn of model are both none'
@@ -267,31 +308,34 @@
 
             # lr = scheduler(optimizer, epoch)
 
             # 放在这里, 是因为前面的set_margin也会产生新的参数位于cpu
             # 如果把参数直接放在cuda, 则导致parameter里没有出现该参数，无法分别设置学习率
             self.model = self.model.to(self.device)
             optimizer.zero_grad()
-            self.train_step(
+            self.train_fn(
                 epoch=epoch,
                 train_loader=train_loader,
                 model=self.model,
                 criterion=criterion,
                 optimizer=optimizer,
                 batch_scheduler=scheduler,
+                fgm=fgm if use_fgm else None,
+                awp=awp if use_awp else None,
+                ema_inst=ema_inst if ema_decay > 0 else None,
                 apex=self.apex,
                 gradient_accumulation_steps=1,
                 max_grad_norm=max_grad_norm,
                 valid_loader=valid_loader,
                 data_collator=data_collator,
                 device=self.device,
             )
 
             if valid_loader is not None:
-                self.valid_step(
+                self.valid_fn(
                     epoch=epoch,
                     valid_loader=valid_loader,
                     model=self.model,
                     criterion=criterion,
                     eval_metrics=eval_metrics,
                     apex=self.apex,
                     device=self.device,
```

### Comparing `open-retrievals-0.0.2/src/retrievals/trainer/trainer.py` & `open-retrievals-0.0.3/src/retrievals/trainer/trainer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import logging
-import math
 import os
-import time
-from dataclasses import dataclass, field
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import torch.nn as nn
 from transformers import Trainer
+from transformers.modeling_outputs import SequenceClassifierOutput
 from transformers.modeling_utils import PreTrainedModel
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.trainer_callback import TrainerCallback
 from transformers.trainer_utils import EvalPrediction
 
-from src.retrievals.losses.triplet import TripletLoss
+from ..losses.triplet import TripletLoss
 
 logger = logging.getLogger(__name__)
 
 
 class RetrievalTrainer(Trainer):
     def __init__(self, loss_fn, **kwargs):
         super().__init__(**kwargs)
@@ -53,12 +51,18 @@
 class RerankTrainer(Trainer):
     def __init__(self, loss_fn=None, **kwargs):
         super().__init__(**kwargs)
         if not loss_fn:
             loss_fn = nn.BCEWithLogitsLoss()
         self.loss_fn = loss_fn
 
-    def compute_loss(self, model, inputs, **kwargs):
-        return
+    def compute_loss(self, model, inputs, return_outputs=False, **kwargs):
+        outputs: dict = model(**inputs)
+        loss = outputs['loss']
+        return (loss, outputs) if return_outputs else loss
 
     def _save(self, output_dir: Optional[str] = None, state_dict=None):
-        pass
+        output_dir = output_dir if output_dir is not None else self.args.output_dir
+        os.makedirs(output_dir, exist_ok=True)
+
+        self.model.model.save_pretrained(output_dir)
+        self.model.tokenizer.save_pretrained(output_dir)
```

### Comparing `open-retrievals-0.0.2/src/retrievals/version.py` & `open-retrievals-0.0.3/src/retrievals/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Longxing Tan.
 
 import sys
 
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 short_version = __version__
 
 
 def parse_version_info(version_str):
     """Parse a version string into a tuple.
 
     Args:
```

