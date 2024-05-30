# Comparing `tmp/neural_cherche-1.1.0.tar.gz` & `tmp/neural_cherche-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural_cherche-1.1.0.tar", last modified: Tue Feb 27 16:57:58 2024, max compression
+gzip compressed data, was "neural_cherche-1.3.0.tar", last modified: Thu May 30 21:17:14 2024, max compression
```

## Comparing `neural_cherche-1.1.0.tar` & `neural_cherche-1.3.0.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2024-02-27 16:57:58.330994 neural_cherche-1.1.0/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     1071 2024-02-20 23:47:00.000000 neural_cherche-1.1.0/LICENSE
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     9097 2024-02-27 16:57:58.331097 neural_cherche-1.1.0/PKG-INFO
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     8415 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/README.md
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2024-02-27 16:57:58.325856 neural_cherche-1.1.0/neural_cherche/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       69 2024-02-20 23:47:01.000000 neural_cherche-1.1.0/neural_cherche/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       63 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/__version__.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2024-02-27 16:57:58.327084 neural_cherche-1.1.0/neural_cherche/losses/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      120 2024-02-20 23:47:01.000000 neural_cherche-1.1.0/neural_cherche/losses/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     2794 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/losses/flops.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     2054 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/losses/ranking.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2024-02-27 16:57:58.327913 neural_cherche-1.1.0/neural_cherche/models/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      142 2024-02-20 23:47:01.000000 neural_cherche-1.1.0/neural_cherche/models/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     4127 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/models/base.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     9224 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/models/colbert.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)    10137 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/models/sparse_embed.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)    10951 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/models/splade.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2024-02-27 16:57:58.328225 neural_cherche-1.1.0/neural_cherche/rank/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       52 2024-02-20 23:47:01.000000 neural_cherche-1.1.0/neural_cherche/rank/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     7368 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/rank/colbert.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2024-02-27 16:57:58.329179 neural_cherche-1.1.0/neural_cherche/retrieve/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      195 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/retrieve/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     5887 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/retrieve/colbert.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)    15218 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/retrieve/sparse_embed.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     4512 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/retrieve/splade.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     6729 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/retrieve/tfidf.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2024-02-27 16:57:58.329792 neural_cherche-1.1.0/neural_cherche/train/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      198 2024-02-20 23:47:01.000000 neural_cherche-1.1.0/neural_cherche/train/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     2937 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/train/train_colbert.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     4993 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/train/train_sparse_embed.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     3782 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/train/train_splade.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2024-02-27 16:57:58.330861 neural_cherche-1.1.0/neural_cherche/utils/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      438 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/utils/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     2456 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/utils/colbert_scores.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     8255 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/utils/dense_scores.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     3237 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/utils/evaluate.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      544 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/utils/freeze.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     1844 2024-02-20 23:47:01.000000 neural_cherche-1.1.0/neural_cherche/utils/iter.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     2262 2024-02-27 16:57:03.000000 neural_cherche-1.1.0/neural_cherche/utils/sparse_scores.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2024-02-27 16:57:58.326597 neural_cherche-1.1.0/neural_cherche.egg-info/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     9097 2024-02-27 16:57:58.000000 neural_cherche-1.1.0/neural_cherche.egg-info/PKG-INFO
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     1179 2024-02-27 16:57:58.000000 neural_cherche-1.1.0/neural_cherche.egg-info/SOURCES.txt
--rw-r--r--   0 raphael.sourty   (502) staff       (20)        1 2024-02-27 16:57:58.000000 neural_cherche-1.1.0/neural_cherche.egg-info/dependency_links.txt
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      307 2024-02-27 16:57:58.000000 neural_cherche-1.1.0/neural_cherche.egg-info/requires.txt
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       15 2024-02-27 16:57:58.000000 neural_cherche-1.1.0/neural_cherche.egg-info/top_level.txt
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       79 2024-02-27 16:57:58.331449 neural_cherche-1.1.0/setup.cfg
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     1390 2024-02-20 23:47:01.000000 neural_cherche-1.1.0/setup.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 21:17:14.676685 neural_cherche-1.3.0/
+-rw-r--r--   0 raphael    (502) staff       (20)     1071 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/LICENSE
+-rw-r--r--   0 raphael    (502) staff       (20)    11184 2024-05-30 21:17:14.676570 neural_cherche-1.3.0/PKG-INFO
+-rw-r--r--   0 raphael    (502) staff       (20)     9504 2024-05-30 21:11:56.000000 neural_cherche-1.3.0/README.md
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 21:17:14.668168 neural_cherche-1.3.0/neural_cherche/
+-rw-r--r--   0 raphael    (502) staff       (20)       69 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)       63 2024-05-30 20:50:57.000000 neural_cherche-1.3.0/neural_cherche/__version__.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 21:17:14.669513 neural_cherche-1.3.0/neural_cherche/losses/
+-rw-r--r--   0 raphael    (502) staff       (20)      120 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/losses/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     2794 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/losses/flops.py
+-rw-r--r--   0 raphael    (502) staff       (20)     2054 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/losses/ranking.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 21:17:14.670761 neural_cherche-1.3.0/neural_cherche/models/
+-rw-r--r--   0 raphael    (502) staff       (20)      142 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/models/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4127 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/models/base.py
+-rw-r--r--   0 raphael    (502) staff       (20)     9224 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/models/colbert.py
+-rw-r--r--   0 raphael    (502) staff       (20)    10137 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/models/sparse_embed.py
+-rw-r--r--   0 raphael    (502) staff       (20)    10951 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/models/splade.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 21:17:14.671541 neural_cherche-1.3.0/neural_cherche/rank/
+-rw-r--r--   0 raphael    (502) staff       (20)      105 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/rank/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)    10616 2024-05-24 13:32:45.000000 neural_cherche-1.3.0/neural_cherche/rank/colbert.py
+-rw-r--r--   0 raphael    (502) staff       (20)    11941 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/rank/sparse_embed.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 21:17:14.672947 neural_cherche-1.3.0/neural_cherche/retrieve/
+-rw-r--r--   0 raphael    (502) staff       (20)      230 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/retrieve/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     5808 2024-05-30 20:34:19.000000 neural_cherche-1.3.0/neural_cherche/retrieve/bm25.py
+-rw-r--r--   0 raphael    (502) staff       (20)     6111 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/retrieve/colbert.py
+-rw-r--r--   0 raphael    (502) staff       (20)    15777 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/retrieve/sparse_embed.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4857 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/retrieve/splade.py
+-rw-r--r--   0 raphael    (502) staff       (20)     7034 2024-05-30 20:44:49.000000 neural_cherche-1.3.0/neural_cherche/retrieve/tfidf.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 21:17:14.673782 neural_cherche-1.3.0/neural_cherche/train/
+-rw-r--r--   0 raphael    (502) staff       (20)      198 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/train/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     2937 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/train/train_colbert.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4993 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/train/train_sparse_embed.py
+-rw-r--r--   0 raphael    (502) staff       (20)     3782 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/train/train_splade.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 21:17:14.675103 neural_cherche-1.3.0/neural_cherche/utils/
+-rw-r--r--   0 raphael    (502) staff       (20)      543 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/utils/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     2456 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/utils/colbert_scores.py
+-rw-r--r--   0 raphael    (502) staff       (20)     8255 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/utils/dense_scores.py
+-rw-r--r--   0 raphael    (502) staff       (20)     5487 2024-05-30 20:44:19.000000 neural_cherche-1.3.0/neural_cherche/utils/evaluate.py
+-rw-r--r--   0 raphael    (502) staff       (20)      544 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/utils/freeze.py
+-rw-r--r--   0 raphael    (502) staff       (20)     1844 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/utils/iter.py
+-rw-r--r--   0 raphael    (502) staff       (20)     2262 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/utils/sparse_scores.py
+-rw-r--r--   0 raphael    (502) staff       (20)      208 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/utils/warnings.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 21:17:14.675309 neural_cherche-1.3.0/neural_cherche.egg-info/
+-rw-r--r--   0 raphael    (502) staff       (20)    11184 2024-05-30 21:17:14.000000 neural_cherche-1.3.0/neural_cherche.egg-info/PKG-INFO
+-rw-r--r--   0 raphael    (502) staff       (20)     1280 2024-05-30 21:17:14.000000 neural_cherche-1.3.0/neural_cherche.egg-info/SOURCES.txt
+-rw-r--r--   0 raphael    (502) staff       (20)        1 2024-05-30 21:17:14.000000 neural_cherche-1.3.0/neural_cherche.egg-info/dependency_links.txt
+-rw-r--r--   0 raphael    (502) staff       (20)      404 2024-05-30 21:17:14.000000 neural_cherche-1.3.0/neural_cherche.egg-info/requires.txt
+-rw-r--r--   0 raphael    (502) staff       (20)       15 2024-05-30 21:17:14.000000 neural_cherche-1.3.0/neural_cherche.egg-info/top_level.txt
+-rw-r--r--   0 raphael    (502) staff       (20)       79 2024-05-30 21:17:14.676874 neural_cherche-1.3.0/setup.cfg
+-rw-r--r--   0 raphael    (502) staff       (20)     1507 2024-05-30 21:14:35.000000 neural_cherche-1.3.0/setup.py
```

### Comparing `neural_cherche-1.1.0/LICENSE` & `neural_cherche-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.1.0/PKG-INFO` & `neural_cherche-1.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: neural_cherche
-Version: 1.1.0
-Summary: Sparse Embeddings for Neural Search.
-Home-page: https://github.com/raphaelsty/neural-cherche
-Download-URL: https://github.com/user/neural-cherche/archive/v_01.tar.gz
-Author: Raphael Sourty
-Author-email: raphael.sourty@gmail.com
-Keywords: neural search,information retrieval,semantic search,SparseEmbed,Google Research,Splade,Stanford,ColBERT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: eval
-Provides-Extra: dev
-License-File: LICENSE
-
 <div align="center">
   <h1>Neural-Cherche</h1>
   <p>Neural Search</p>
 </div>
 
 <p align="center"><img width=500 src="docs/img/logo.png"/></p>
 
@@ -106,61 +88,91 @@
     if (step + 1) % 1000 == 0:
         # Save the model every 1000 steps
         model.save_pretrained("checkpoint")
 ```
 
 ## Retrieval
 
-Here is how to use the fine-tuned ColBERT model to retrieve documents:
+Here is how to use the fine-tuned ColBERT model to re-rank documents:
 
 ```python
-from neural_cherche import models, retrieve
 import torch
+from lenlp import sparse
 
-batch_size = 32
+from neural_cherche import models, rank, retrieve
 
 documents = [
-    {"id": 0, "document": "Food"},
-    {"id": 1, "document": "Sports"},
-    {"id": 2, "document": "Cinema"},
+    {"id": "doc1", "title": "Paris", "text": "Paris is the capital of France."},
+    {"id": "doc2", "title": "Montreal", "text": "Montreal is the largest city in Quebec."},
+    {"id": "doc3", "title": "Bordeaux", "text": "Bordeaux in Southwestern France."},
 ]
 
+retriever = retrieve.BM25(
+    key="id",
+    on=["title", "text"],
+    count_vectorizer=sparse.CountVectorizer(
+        normalize=True, ngram_range=(3, 5), analyzer="char_wb", stop_words=[]
+    ),
+    k1=1.5,
+    b=0.75,
+    epsilon=0.0,
+)
+
 model = models.ColBERT(
     model_name_or_path="raphaelsty/neural-cherche-colbert",
-    device="cuda" if torch.cuda.is_available() else "cpu", # or mps
+    device="cuda" if torch.cuda.is_available() else "cpu",  # or mps
 )
 
-retriever = retrieve.ColBERT(
+ranker = rank.ColBERT(
     key="id",
-    on=["document"], # the field to search on, can be a list of fields
+    on=["title", "text"],
     model=model,
 )
 
 documents_embeddings = retriever.encode_documents(
     documents=documents,
-    batch_size=batch_size,
 )
 
-retriever = retriever.add(
+retriever.add(
     documents_embeddings=documents_embeddings,
 )
 ```
 
 Now we can retrieve documents using the fine-tuned model:
 
 ```python
+queries = ["Paris", "Montreal", "Bordeaux"]
+
 queries_embeddings = retriever.encode_queries(
-    queries=["Food", "Sports", "Cinema"], # list of queries
-    batch_size=batch_size,
+    queries=queries,
 )
 
-scores = retriever(
+ranker_queries_embeddings = ranker.encode_queries(
+    queries=queries,
+)
+
+candidates = retriever(
     queries_embeddings=queries_embeddings,
-    batch_size=batch_size,
-    k=10, # number of documents to retrieve
+    batch_size=32,
+    k=100,  # number of documents to retrieve
+)
+
+# Compute embeddings of the candidates with the ranker model.
+# Note, we could also pre-compute all the embeddings.
+ranker_documents_embeddings = ranker.encode_candidates_documents(
+    candidates=candidates,
+    documents=documents,
+    batch_size=32,
+)
+
+scores = ranker(
+    queries_embeddings=ranker_queries_embeddings,
+    documents_embeddings=ranker_documents_embeddings,
+    documents=candidates,
+    batch_size=32,
 )
 
 scores
 ```
 
 ```python
 [[{'id': 0, 'similarity': 22.825355529785156},
@@ -170,18 +182,15 @@
   {'id': 0, 'similarity': 9.9658203125},
   {'id': 2, 'similarity': 7.308732509613037}],
  [{'id': 1, 'similarity': 6.4031805992126465},
   {'id': 0, 'similarity': 5.601611137390137},
   {'id': 2, 'similarity': 5.599479675292969}]]
 ```
 
-Please note that neural-cherche provide documentation to use [ColBERT as a ranker](https://raphaelsty.github.io/neural-cherche/retrieve/colbert/) which is much more efficient.
-
-
-Neural-Cherche also provides a `SparseEmbed`, a `SPLADE`, a `TFIDF` retriever and a `ColBERT` ranker which can be used to re-order output of a retriever. For more information, please refer to the [documentation](https://raphaelsty.github.io/neural-cherche/).
+Neural-Cherche provides a `SparseEmbed`, a `SPLADE`, a `TFIDF`, a `BM25` retriever and a `ColBERT` ranker which can be used to re-order output of a retriever. For more information, please refer to the [documentation](https://raphaelsty.github.io/neural-cherche/).
 
 ### Pre-trained Models
 
 We provide pre-trained checkpoints specifically designed for neural-cherche: [raphaelsty/neural-cherche-sparse-embed](https://huggingface.co/raphaelsty/neural-cherche-sparse-embed) and [raphaelsty/neural-cherche-colbert](https://huggingface.co/raphaelsty/neural-cherche-colbert). Those checkpoints are fine-tuned on a subset of the MS-MARCO dataset and would benefit from being fine-tuned on your specific dataset. You can fine-tune ColBERT from any Sentence Transformer pre-trained checkpoint in order to fit your specific language. You should use a MLM based-checkpoint to fine-tune SparseEmbed.
 
 <table class="tg">
 <thead>
@@ -198,17 +207,24 @@
     <td class="tg-rvyq">ndcg@10</td>
     <td class="tg-rvyq">hits@10</td>
     <td class="tg-rvyq">hits@1</td>
   </tr>
   <tr>
     <td class="tg-c3ow">TfIdf</td>
     <td class="tg-c3ow">-</td>
-    <td class="tg-c3ow">0,61</td>
-    <td class="tg-c3ow">0,85</td>
-    <td class="tg-c3ow">0,47</td>
+    <td class="tg-c3ow">0,62</td>
+    <td class="tg-c3ow">0,86</td>
+    <td class="tg-c3ow">0,50</td>
+  </tr>
+  <tr>
+    <td class="tg-c3ow">BM25</td>
+    <td class="tg-c3ow">-</td>
+    <td class="tg-c3ow">0,69</td>
+    <td class="tg-c3ow">0,92</td>
+    <td class="tg-c3ow">0,56</td>
   </tr>
   <tr>
     <td class="tg-c3ow">SparseEmbed</td>
     <td class="tg-c3ow">raphaelsty/neural-cherche-sparse-embed</td>
     <td class="tg-c3ow">0,62</td>
     <td class="tg-c3ow">0,87</td>
     <td class="tg-c3ow">0,48</td>
@@ -230,20 +246,28 @@
   <tr>
     <td class="tg-c3ow">TfIDF Retriever + ColBERT Ranker</td>
     <td class="tg-c3ow">raphaelsty/neural-cherche-colbert</td>
     <td class="tg-7btt">0,71</td>
     <td class="tg-7btt">0,94</td>
     <td class="tg-7btt">0,59</td>
   </tr>
+  <tr>
+    <td class="tg-c3ow">BM25 Retriever + ColBERT Ranker</td>
+    <td class="tg-c3ow">raphaelsty/neural-cherche-colbert</td>
+    <td class="tg-7btt">0,72</td>
+    <td class="tg-7btt">0,95</td>
+    <td class="tg-7btt">0,59</td>
+  </tr>
 </tbody>
 </table>
 
 ### Neural-Cherche Contributors
 
 - [Benjamin Clavié](https://github.com/bclavie)
+- [Arthur Satouf](https://github.com/arthur-75)
 
 ## References
 
 - *[SPLADE: Sparse Lexical and Expansion Model for First Stage Ranking](https://arxiv.org/abs/2107.05720)* authored by Thibault Formal, Benjamin Piwowarski, Stéphane Clinchant, SIGIR 2021.
 
 - *[SPLADE v2: Sparse Lexical and Expansion Model for Information Retrieval](https://arxiv.org/abs/2109.10086)* authored by Thibault Formal, Carlos Lassance, Benjamin Piwowarski, Stéphane Clinchant, SIGIR 2022.
```

#### html2text {}

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1 Name: neural_cherche Version: 1.1.0 Summary: Sparse
-Embeddings for Neural Search. Home-page: https://github.com/raphaelsty/neural-
-cherche Download-URL: https://github.com/user/neural-cherche/archive/
-v_01.tar.gz Author: Raphael Sourty Author-email: raphael.sourty@gmail.com
-Keywords: neural search,information retrieval,semantic
-search,SparseEmbed,Google Research,Splade,Stanford,ColBERT Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown Provides-Extra: eval Provides-Extra:
-dev License-File: LICENSE
                          ************ NNeeuurraall--CChheerrcchhee ************
                                  Neural Search
                               [docs/img/logo.png]
                            _[_d_o_c_u_m_e_n_t_a_t_i_o_n_]_[_l_i_c_e_n_s_e_]
 Neural-Cherche is a library designed to fine-tune neural search models such as
 Splade, ColBERT, and SparseEmbed on a specific dataset. Neural-Cherche also
 provide classes to run efficient inference on a fine-tuned retriever or ranker.
@@ -40,69 +30,80 @@
 "positive document", "negative document"), ] for step, (anchor, positive,
 negative) in enumerate(utils.iter( X, epochs=1, # number of epochs
 batch_size=8, # number of triples per batch shuffle=True )): loss =
 train.train_colbert( model=model, optimizer=optimizer, anchor=anchor,
 positive=positive, negative=negative, step=step,
 gradient_accumulation_steps=50, ) if (step + 1) % 1000 == 0: # Save the model
 every 1000 steps model.save_pretrained("checkpoint") ``` ## Retrieval Here is
-how to use the fine-tuned ColBERT model to retrieve documents: ```python from
-neural_cherche import models, retrieve import torch batch_size = 32 documents =
-[ {"id": 0, "document": "Food"}, {"id": 1, "document": "Sports"}, {"id": 2,
-"document": "Cinema"}, ] model = models.ColBERT
-( model_name_or_path="raphaelsty/neural-cherche-colbert", device="cuda" if
-torch.cuda.is_available() else "cpu", # or mps ) retriever = retrieve.ColBERT
-( key="id", on=["document"], # the field to search on, can be a list of fields
-model=model, ) documents_embeddings = retriever.encode_documents
-( documents=documents, batch_size=batch_size, ) retriever = retriever.add
-( documents_embeddings=documents_embeddings, ) ``` Now we can retrieve
-documents using the fine-tuned model: ```python queries_embeddings =
-retriever.encode_queries( queries=["Food", "Sports", "Cinema"], # list of
-queries batch_size=batch_size, ) scores = retriever
-( queries_embeddings=queries_embeddings, batch_size=batch_size, k=10, # number
-of documents to retrieve ) scores ``` ```python [[{'id': 0, 'similarity':
+how to use the fine-tuned ColBERT model to re-rank documents: ```python import
+torch from lenlp import sparse from neural_cherche import models, rank,
+retrieve documents = [ {"id": "doc1", "title": "Paris", "text": "Paris is the
+capital of France."}, {"id": "doc2", "title": "Montreal", "text": "Montreal is
+the largest city in Quebec."}, {"id": "doc3", "title": "Bordeaux", "text":
+"Bordeaux in Southwestern France."}, ] retriever = retrieve.BM25( key="id", on=
+["title", "text"], count_vectorizer=sparse.CountVectorizer( normalize=True,
+ngram_range=(3, 5), analyzer="char_wb", stop_words=[] ), k1=1.5, b=0.75,
+epsilon=0.0, ) model = models.ColBERT( model_name_or_path="raphaelsty/neural-
+cherche-colbert", device="cuda" if torch.cuda.is_available() else "cpu", # or
+mps ) ranker = rank.ColBERT( key="id", on=["title", "text"], model=model, )
+documents_embeddings = retriever.encode_documents( documents=documents, )
+retriever.add( documents_embeddings=documents_embeddings, ) ``` Now we can
+retrieve documents using the fine-tuned model: ```python queries = ["Paris",
+"Montreal", "Bordeaux"] queries_embeddings = retriever.encode_queries
+( queries=queries, ) ranker_queries_embeddings = ranker.encode_queries
+( queries=queries, ) candidates = retriever
+( queries_embeddings=queries_embeddings, batch_size=32, k=100, # number of
+documents to retrieve ) # Compute embeddings of the candidates with the ranker
+model. # Note, we could also pre-compute all the embeddings.
+ranker_documents_embeddings = ranker.encode_candidates_documents
+( candidates=candidates, documents=documents, batch_size=32, ) scores = ranker
+( queries_embeddings=ranker_queries_embeddings,
+documents_embeddings=ranker_documents_embeddings, documents=candidates,
+batch_size=32, ) scores ``` ```python [[{'id': 0, 'similarity':
 22.825355529785156}, {'id': 1, 'similarity': 11.201947212219238}, {'id': 2,
 'similarity': 10.748161315917969}], [{'id': 1, 'similarity':
 23.21628189086914}, {'id': 0, 'similarity': 9.9658203125}, {'id': 2,
 'similarity': 7.308732509613037}], [{'id': 1, 'similarity':
 6.4031805992126465}, {'id': 0, 'similarity': 5.601611137390137}, {'id': 2,
-'similarity': 5.599479675292969}]] ``` Please note that neural-cherche provide
-documentation to use [ColBERT as a ranker](https://raphaelsty.github.io/neural-
-cherche/retrieve/colbert/) which is much more efficient. Neural-Cherche also
-provides a `SparseEmbed`, a `SPLADE`, a `TFIDF` retriever and a `ColBERT`
-ranker which can be used to re-order output of a retriever. For more
-information, please refer to the [documentation](https://raphaelsty.github.io/
-neural-cherche/). ### Pre-trained Models We provide pre-trained checkpoints
-specifically designed for neural-cherche: [raphaelsty/neural-cherche-sparse-
-embed](https://huggingface.co/raphaelsty/neural-cherche-sparse-embed) and
-[raphaelsty/neural-cherche-colbert](https://huggingface.co/raphaelsty/neural-
-cherche-colbert). Those checkpoints are fine-tuned on a subset of the MS-MARCO
-dataset and would benefit from being fine-tuned on your specific dataset. You
-can fine-tune ColBERT from any Sentence Transformer pre-trained checkpoint in
-order to fit your specific language. You should use a MLM based-checkpoint to
-fine-tune SparseEmbed.
+'similarity': 5.599479675292969}]] ``` Neural-Cherche provides a `SparseEmbed`,
+a `SPLADE`, a `TFIDF`, a `BM25` retriever and a `ColBERT` ranker which can be
+used to re-order output of a retriever. For more information, please refer to
+the [documentation](https://raphaelsty.github.io/neural-cherche/). ### Pre-
+trained Models We provide pre-trained checkpoints specifically designed for
+neural-cherche: [raphaelsty/neural-cherche-sparse-embed](https://
+huggingface.co/raphaelsty/neural-cherche-sparse-embed) and [raphaelsty/neural-
+cherche-colbert](https://huggingface.co/raphaelsty/neural-cherche-colbert).
+Those checkpoints are fine-tuned on a subset of the MS-MARCO dataset and would
+benefit from being fine-tuned on your specific dataset. You can fine-tune
+ColBERT from any Sentence Transformer pre-trained checkpoint in order to fit
+your specific language. You should use a MLM based-checkpoint to fine-tune
+SparseEmbed.
                                                      sscciiffaacctt ddaattaasseett
 model                     HuggingFace Checkpoint     ndcg@10 hits@10 hits@1
-TfIdf                     -                          0,61    0,85    0,47
+TfIdf                     -                          0,62    0,86    0,50
+BM25                      -                          0,69    0,92    0,56
 SparseEmbed               raphaelsty/neural-cherche- 0,62    0,87    0,48
                           sparse-embed
 Sentence Transformer      sentence-transformers/all- 0,66    0,89    0,53
                           mpnet-base-v2
 ColBERT                   raphaelsty/neural-cherche- 0,70    0,92    0,58
                           colbert
 TfIDF Retriever + ColBERT raphaelsty/neural-cherche- 0,71    0,94    0,59
 Ranker                    colbert
+BM25 Retriever + ColBERT  raphaelsty/neural-cherche- 0,72    0,95    0,59
+Ranker                    colbert
 ### Neural-Cherche Contributors - [Benjamin ClaviÃ©](https://github.com/
-bclavie) ## References - *[SPLADE: Sparse Lexical and Expansion Model for First
-Stage Ranking](https://arxiv.org/abs/2107.05720)* authored by Thibault Formal,
-Benjamin Piwowarski, StÃ©phane Clinchant, SIGIR 2021. - *[SPLADE v2: Sparse
-Lexical and Expansion Model for Information Retrieval](https://arxiv.org/abs/
-2109.10086)* authored by Thibault Formal, Carlos Lassance, Benjamin Piwowarski,
-StÃ©phane Clinchant, SIGIR 2022. - *[SparseEmbed: Learning Sparse Lexical
-Representations with Contextual Embeddings for Retrieval](https://
-research.google/pubs/pub52289/)* authored by Weize Kong, Jeffrey M. Dudek,
-Cheng Li, Mingyang Zhang, and Mike Bendersky, SIGIR 2023. - *[ColBERT:
-Efficient and Effective Passage Search via Contextualized Late Interaction over
-BERT](https://arxiv.org/abs/2004.12832)* authored by Omar Khattab, Matei
-Zaharia, SIGIR 2020. ## License This Python library is licensed under the MIT
-open-source license, and the splade model is licensed as non-commercial only by
-the authors. SparseEmbed and ColBERT are fully open-source including commercial
-usage.
+bclavie) - [Arthur Satouf](https://github.com/arthur-75) ## References - *
+[SPLADE: Sparse Lexical and Expansion Model for First Stage Ranking](https://
+arxiv.org/abs/2107.05720)* authored by Thibault Formal, Benjamin Piwowarski,
+StÃ©phane Clinchant, SIGIR 2021. - *[SPLADE v2: Sparse Lexical and Expansion
+Model for Information Retrieval](https://arxiv.org/abs/2109.10086)* authored by
+Thibault Formal, Carlos Lassance, Benjamin Piwowarski, StÃ©phane Clinchant,
+SIGIR 2022. - *[SparseEmbed: Learning Sparse Lexical Representations with
+Contextual Embeddings for Retrieval](https://research.google/pubs/pub52289/)*
+authored by Weize Kong, Jeffrey M. Dudek, Cheng Li, Mingyang Zhang, and Mike
+Bendersky, SIGIR 2023. - *[ColBERT: Efficient and Effective Passage Search via
+Contextualized Late Interaction over BERT](https://arxiv.org/abs/2004.12832)*
+authored by Omar Khattab, Matei Zaharia, SIGIR 2020. ## License This Python
+library is licensed under the MIT open-source license, and the splade model is
+licensed as non-commercial only by the authors. SparseEmbed and ColBERT are
+fully open-source including commercial usage.
```

### Comparing `neural_cherche-1.1.0/neural_cherche/losses/flops.py` & `neural_cherche-1.3.0/neural_cherche/losses/flops.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.1.0/neural_cherche/losses/ranking.py` & `neural_cherche-1.3.0/neural_cherche/losses/ranking.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.1.0/neural_cherche/models/base.py` & `neural_cherche-1.3.0/neural_cherche/models/base.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.1.0/neural_cherche/models/colbert.py` & `neural_cherche-1.3.0/neural_cherche/models/colbert.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.1.0/neural_cherche/models/sparse_embed.py` & `neural_cherche-1.3.0/neural_cherche/models/sparse_embed.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.1.0/neural_cherche/models/splade.py` & `neural_cherche-1.3.0/neural_cherche/models/splade.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.1.0/neural_cherche/rank/colbert.py` & `neural_cherche-1.3.0/neural_cherche/retrieve/colbert.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import torch
 
 from .. import models, utils
+from ..rank import ColBERT as ColBERTRanker
 
 __all__ = ["ColBERT"]
 
 
-class ColBERT:
-    """ColBERT ranker.
+class ColBERT(ColBERTRanker):
+    """ColBERT retriever.
 
     Parameters
     ----------
     key
         Document unique identifier.
     on
         Document texts.
     model
         ColBERT model.
+    device
+        Device to use, default is model device.
 
     Examples
     --------
-    >>> from neural_cherche import models, rank
+    >>> from neural_cherche import models, retrieve
     >>> from pprint import pprint
     >>> import torch
 
     >>> _ = torch.manual_seed(42)
 
     >>> encoder = models.ColBERT(
     ...     model_name_or_path="raphaelsty/neural-cherche-colbert",
@@ -34,143 +37,90 @@
     ...     {"id": 0, "document": "Food"},
     ...     {"id": 1, "document": "Sports"},
     ...     {"id": 2, "document": "Cinema"},
     ... ]
 
     >>> queries = ["Food", "Sports", "Cinema"]
 
-    >>> ranker = rank.ColBERT(
+    >>> retriever = retrieve.ColBERT(
     ...    key="id",
     ...    on=["document"],
     ...    model=encoder,
     ... )
 
-    >>> queries_embeddings = ranker.encode_queries(
-    ...     queries=queries,
+    >>> documents_embeddings = retriever.encode_documents(
+    ...     documents=documents,
     ...     batch_size=3,
     ... )
 
-    >>> documents_embeddings = ranker.encode_documents(
-    ...     documents=documents,
+    >>> retriever = retriever.add(
+    ...     documents_embeddings=documents_embeddings,
+    ... )
+
+    >>> queries_embeddings = retriever.encode_queries(
+    ...     queries=queries,
     ...     batch_size=3,
     ... )
 
-    >>> scores = ranker(
-    ...     documents=[documents for _ in queries],
+    >>> scores = retriever(
     ...     queries_embeddings=queries_embeddings,
-    ...     documents_embeddings=documents_embeddings,
     ...     batch_size=3,
     ...     tqdm_bar=True,
     ...     k=3,
     ... )
 
     >>> pprint(scores)
-    [[{'document': 'Food', 'id': 0, 'similarity': 4.7243194580078125},
-      {'document': 'Cinema', 'id': 2, 'similarity': 2.403003692626953},
-      {'document': 'Sports', 'id': 1, 'similarity': 2.286036252975464}],
-     [{'document': 'Sports', 'id': 1, 'similarity': 4.792296886444092},
-      {'document': 'Cinema', 'id': 2, 'similarity': 2.6001152992248535},
-      {'document': 'Food', 'id': 0, 'similarity': 2.312016487121582}],
-     [{'document': 'Cinema', 'id': 2, 'similarity': 5.069696426391602},
-      {'document': 'Sports', 'id': 1, 'similarity': 2.5587477684020996},
-      {'document': 'Food', 'id': 0, 'similarity': 2.4474282264709473}]]
+    [[{'id': 0, 'similarity': 4.7243194580078125},
+      {'id': 2, 'similarity': 2.403003692626953},
+      {'id': 1, 'similarity': 2.286036252975464}],
+     [{'id': 1, 'similarity': 4.792296886444092},
+      {'id': 2, 'similarity': 2.6001152992248535},
+      {'id': 0, 'similarity': 2.312016487121582}],
+     [{'id': 2, 'similarity': 5.069696426391602},
+      {'id': 1, 'similarity': 2.5587477684020996},
+      {'id': 0, 'similarity': 2.4474282264709473}]]
 
     """
 
     def __init__(
         self,
         key: str,
         on: list[str],
         model: models.ColBERT,
+        device: str = None,
     ) -> None:
         self.key = key
         self.on = on if isinstance(on, list) else [on]
         self.model = model
-        self.device = self.model.device
+        self.documents = []
+        self.documents_embeddings = {}
+        self.device = device if device is not None else self.model.device
 
-    def encode_documents(
+    def add(
         self,
-        documents: list[str],
-        batch_size: int = 32,
-        tqdm_bar: bool = True,
-        query_mode: bool = False,
-        **kwargs,
-    ) -> dict[str, torch.Tensor]:
-        """Encode documents.
+        documents_embeddings: dict[str, torch.Tensor],
+    ) -> "ColBERT":
+        """Add documents embeddings.
 
         Parameters
         ----------
+        documents_embeddings
+            Documents embeddings.
         documents
             Documents.
-        batch_size
-            Batch size.
-        tqdm_bar
-            Show tqdm bar.
-        """
-        # Documents embeddings must be composed of more tokens than queries embeddings
-        embeddings = self.encode_queries(
-            queries=[
-                " ".join([document[field] for field in self.on])
-                for document in documents
-            ],
-            batch_size=batch_size,
-            tqdm_bar=tqdm_bar,
-            query_mode=query_mode,
-            **kwargs,
-        )
-
-        return {
-            document[self.key]: embedding
-            for document, embedding in zip(documents, embeddings.values())
-        }
-
-    def encode_queries(
-        self,
-        queries: list[str],
-        batch_size: int = 32,
-        tqdm_bar: bool = True,
-        query_mode: bool = True,
-        **kwargs,
-    ) -> dict[str, torch.Tensor]:
-        """Encode queries.
-
-        Parameters
-        ----------
-        queries
-            Queries.
-        batch_size
-            Batch size.
-        tqdm_bar
-            Show tqdm bar.
         """
-        embeddings = {}
-
-        for batch_texts in utils.batchify(
-            X=queries, batch_size=batch_size, tqdm_bar=tqdm_bar
-        ):
-            batch_embeddings = self.model.encode(
-                texts=batch_texts,
-                query_mode=query_mode,
-                **kwargs,
-            )
-
-            batch_embeddings = (
-                batch_embeddings["embeddings"].cpu().detach().numpy().astype("float32")
-            )
-
-            for query, embedding in zip(batch_texts, batch_embeddings):
-                embeddings[query] = embedding
-
-        return embeddings
+        for document_key, tokens_embeddings in documents_embeddings.items():
+            if document_key not in self.documents_embeddings:
+                self.documents.append({self.key: document_key})
+                self.documents_embeddings[document_key] = tokens_embeddings
+        return self
 
     def __call__(
         self,
-        documents: list[list[dict]],
         queries_embeddings: dict[str, torch.Tensor],
-        documents_embeddings: dict[str, torch.Tensor],
         batch_size: int = 32,
         tqdm_bar: bool = True,
         k: int = None,
     ) -> list[list[str]]:
         """Rank documents  givent queries.
 
         Parameters
@@ -188,34 +138,40 @@
         tqdm_bar
             Show tqdm bar.
         k
             Number of documents to retrieve.
         """
         scores = []
 
-        for (query, query_embedding), query_documents in zip(
-            queries_embeddings.items(), documents
-        ):
+        bar = utils.batchify(
+            X=[query_embedding for query_embedding in queries_embeddings.values()],
+            batch_size=1,
+            tqdm_bar=tqdm_bar,
+            desc=f"{self.__class__.__name__} retriever",
+        )
+
+        for query_embedding in bar:
+            query_embedding = query_embedding[0]
             query_scores = []
 
             embedding_query = torch.tensor(
-                query_embedding,
+                data=query_embedding,
                 device=self.device,
                 dtype=torch.float32,
             )
 
             for batch_query_documents in utils.batchify(
-                X=query_documents,
+                X=self.documents,
                 batch_size=batch_size,
-                tqdm_bar=tqdm_bar,
+                tqdm_bar=False,
             ):
                 embeddings_batch_documents = torch.stack(
-                    [
+                    tensors=[
                         torch.tensor(
-                            documents_embeddings[document[self.key]],
+                            data=self.documents_embeddings[document[self.key]],
                             device=self.device,
                             dtype=torch.float32,
                         )
                         for document in batch_query_documents
                     ],
                     dim=0,
                 )
@@ -226,17 +182,17 @@
                     embeddings_batch_documents,
                 )
 
                 query_scores.append(
                     query_documents_scores.max(dim=2).values.sum(axis=1)
                 )
 
-            scores.append(torch.cat(query_scores, dim=0))
+            scores.append(torch.cat(tensors=query_scores, dim=0))
 
-        return self._rank(scores=scores, documents=documents, k=k)
+        return self._rank(scores=scores, documents=self.documents, k=k)
 
     def _rank(
         self, scores: torch.Tensor, documents: list[list[dict]], k: int
     ) -> list[list[dict]]:
         """Rank documents by scores.
 
         Parameters
@@ -246,24 +202,22 @@
         documents
             Documents.
         k
             Number of documents to retrieve.
         """
         ranked = []
 
-        for query_scores, query_documents in zip(scores, documents):
+        for query_scores in scores:
             top_k = torch.topk(
                 input=query_scores,
-                k=min(k, len(query_documents))
-                if k is not None
-                else len(query_documents),
+                k=min(k, len(documents)) if k is not None else len(documents),
                 dim=-1,
             )
 
             ranked.append(
                 [
-                    {**query_documents[indice], "similarity": similarity}
+                    {**documents[indice], "similarity": similarity}
                     for indice, similarity in zip(top_k.indices, top_k.values.tolist())
                 ]
             )
 
         return ranked
```

### Comparing `neural_cherche-1.1.0/neural_cherche/retrieve/colbert.py` & `neural_cherche-1.3.0/neural_cherche/retrieve/tfidf.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,219 +1,219 @@
-import torch
-import tqdm
+import numpy as np
+from lenlp import sparse
+from scipy.sparse import csc_matrix, csr_matrix, hstack, vstack
 
-from .. import models, utils
-from ..rank import ColBERT as ColBERTRanker
+from .. import utils
 
-__all__ = ["ColBERT"]
+__all__ = ["TfIdf"]
 
 
-class ColBERT(ColBERTRanker):
-    """ColBERT retriever.
+class TfIdf:
+    """TfIdf retriever based on cosine similarities.
 
     Parameters
     ----------
     key
-        Document unique identifier.
+        Field identifier of each document.
     on
-        Document texts.
-    model
-        ColBERT model.
+        Fields to use to match the query to the documents.
+    documents
+        Documents in TFIdf retriever are static. The retriever must be reseted to index new
+        documents.
+    k
+        Number of documents to retrieve. Default is `None`, i.e all documents that match the query
+        will be retrieved.
+    tfidf
+        TfidfVectorizer class of Sklearn to create a custom TfIdf retriever.
 
     Examples
     --------
-    >>> from neural_cherche import models, retrieve
+    >>> from neural_cherche import retrieve
     >>> from pprint import pprint
-    >>> import torch
-
-    >>> _ = torch.manual_seed(42)
-
-    >>> encoder = models.ColBERT(
-    ...     model_name_or_path="raphaelsty/neural-cherche-colbert",
-    ...     device="mps",
-    ... )
 
     >>> documents = [
     ...     {"id": 0, "document": "Food"},
     ...     {"id": 1, "document": "Sports"},
     ...     {"id": 2, "document": "Cinema"},
     ... ]
 
     >>> queries = ["Food", "Sports", "Cinema"]
 
-    >>> retriever = retrieve.ColBERT(
-    ...    key="id",
-    ...    on=["document"],
-    ...    model=encoder,
+    >>> retriever = retrieve.TfIdf(
+    ...     key="id",
+    ...     on=["document"],
     ... )
 
     >>> documents_embeddings = retriever.encode_documents(
-    ...     documents=documents,
-    ...     batch_size=3,
+    ...     documents=documents
     ... )
 
     >>> retriever = retriever.add(
     ...     documents_embeddings=documents_embeddings,
     ... )
 
     >>> queries_embeddings = retriever.encode_queries(
-    ...     queries=queries,
-    ...     batch_size=3,
+    ...     queries=queries
     ... )
 
     >>> scores = retriever(
     ...     queries_embeddings=queries_embeddings,
-    ...     batch_size=3,
-    ...     tqdm_bar=True,
-    ...     k=3,
+    ...     k=4
+    ... )
+
+    >>> queries_embeddings = retriever.encode_queries(
+    ...     queries=["hello world", "hello world"]
     ... )
 
     >>> pprint(scores)
-    [[{'id': 0, 'similarity': 4.7243194580078125},
-      {'id': 2, 'similarity': 2.403003692626953},
-      {'id': 1, 'similarity': 2.286036252975464}],
-     [{'id': 1, 'similarity': 4.792296886444092},
-      {'id': 2, 'similarity': 2.6001152992248535},
-      {'id': 0, 'similarity': 2.312016487121582}],
-     [{'id': 2, 'similarity': 5.069696426391602},
-      {'id': 1, 'similarity': 2.5587477684020996},
-      {'id': 0, 'similarity': 2.4474282264709473}]]
+    [[{'id': 0, 'similarity': 1.0}],
+     [{'id': 1, 'similarity': 0.9999999999999999}],
+     [{'id': 2, 'similarity': 0.9999999999999999}]]
+
+    References
+    ----------
+    1. [sklearn.feature_extraction.text.TfidfVectorizer](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html)
+    2. [Python: tf-idf-cosine: to find document similarity](https://stackoverflow.com/questions/12118720/python-tf-idf-cosine-to-find-document-similarity)
 
     """
 
     def __init__(
         self,
         key: str,
         on: list[str],
-        model: models.ColBERT,
+        tfidf: sparse.TfidfVectorizer = None,
+        fit: bool = True,
     ) -> None:
         self.key = key
-        self.on = on if isinstance(on, list) else [on]
-        self.model = model
-        self.device = self.model.device
+        self.on = [on] if isinstance(on, str) else on
+
+        self.vectorizer = (
+            sparse.TfidfVectorizer(normalize=True, ngram_range=(3, 5), analyzer="char")
+            if tfidf is None
+            else tfidf
+        )
+
+        self.matrix = None
+        self.fit = fit
         self.documents = []
-        self.documents_embeddings = {}
+        self.n_documents = 0
 
-    def add(
-        self,
-        documents_embeddings: dict[str, torch.Tensor],
-    ) -> "ColBERT":
-        """Add documents embeddings.
+    def encode_documents(self, documents: list[dict]) -> dict[str, csr_matrix]:
+        """Encode queries into sparse matrix.
 
         Parameters
         ----------
-        documents_embeddings
-            Documents embeddings.
         documents
-            Documents.
-        """
-        for document_key, tokens_embeddings in documents_embeddings.items():
-            if document_key not in self.documents_embeddings:
-                self.documents.append({self.key: document_key})
-                self.documents_embeddings[document_key] = tokens_embeddings
-        return self
+            Documents to encode.
 
-    def __call__(
-        self,
-        queries_embeddings: dict[str, torch.Tensor],
-        batch_size: int = 32,
-        tqdm_bar: bool = True,
-        k: int = None,
-    ) -> list[list[str]]:
-        """Rank documents  givent queries.
+        """
+        content = [
+            " ".join([doc.get(field, "") for field in self.on]) for doc in documents
+        ]
+
+        matrix = None
+        if self.fit:
+            matrix = self.vectorizer.fit_transform(raw_documents=content)
+            self.fit = False
+
+        # matrix is a csr matrix of shape (n_documents, n_features)
+        if matrix is None:
+            matrix = self.vectorizer.transform(raw_documents=content)
+        return {document[self.key]: row for document, row in zip(documents, matrix)}
+
+    def encode_queries(
+        self, queries: list[str], warn_duplicates: bool = True
+    ) -> dict[str, csr_matrix]:
+        """Encode queries into sparse matrix.
 
         Parameters
         ----------
         queries
-            Queries.
-        documents
-            Documents.
-        queries_embeddings
-            Queries embeddings.
-        documents_embeddings
-            Documents embeddings.
-        batch_size
-            Batch size.
-        tqdm_bar
-            Show tqdm bar.
-        k
-            Number of documents to retrieve.
+            Queries to encode.
+
         """
-        scores = []
+        if self.fit:
+            raise ValueError("You must call the `encode_documents` method first.")
 
-        bar = (
-            tqdm.tqdm(iterable=queries_embeddings.items(), position=0)
-            if tqdm_bar
-            else queries_embeddings.items()
-        )
+        # matrix is a csr matrix of shape (n_queries, n_features)
+        matrix = self.vectorizer.transform(raw_documents=queries)
+        embeddings = {query: row for query, row in zip(queries, matrix)}
 
-        for query, query_embedding in bar:
-            query_scores = []
+        if len(embeddings) != len(queries) and warn_duplicates:
+            utils.duplicates_queries_warning()
 
-            embedding_query = torch.tensor(
-                data=query_embedding,
-                device=self.device,
-                dtype=torch.float32,
-            )
-
-            for batch_query_documents in utils.batchify(
-                X=self.documents,
-                batch_size=batch_size,
-                tqdm_bar=False,
-            ):
-                embeddings_batch_documents = torch.stack(
-                    tensors=[
-                        torch.tensor(
-                            data=self.documents_embeddings[document[self.key]],
-                            device=self.device,
-                            dtype=torch.float32,
-                        )
-                        for document in batch_query_documents
-                    ],
-                    dim=0,
-                )
+        return embeddings
 
-                query_documents_scores = torch.einsum(
-                    "sh,bth->bst",
-                    embedding_query,
-                    embeddings_batch_documents,
-                )
-
-                query_scores.append(
-                    query_documents_scores.max(dim=2).values.sum(axis=1)
-                )
+    def add(
+        self,
+        documents_embeddings: dict[str, csr_matrix],
+    ) -> "TfIdf":
+        """Add new documents to the TFIDF retriever. The tfidf won't be refitted."""
+        matrix = vstack(blocks=[row for row in documents_embeddings.values()]).T.tocsr()
+
+        for document_key in documents_embeddings:
+            self.documents.append({self.key: document_key})
+
+        self.n_documents += len(documents_embeddings)
+        self.matrix = (
+            matrix if self.matrix is None else hstack(blocks=(self.matrix, matrix))
+        )
 
-            scores.append(torch.cat(tensors=query_scores, dim=0))
+        return self
 
-        return self._rank(scores=scores, documents=self.documents, k=k)
+    def top_k(self, similarities: csc_matrix, k: int) -> tuple[list, list]:
+        """Return the top k documents for each query."""
+        matchs, scores = [], []
+        for row in similarities:
+            _k = min(row.data.shape[0] - 1, k)
+            ind = np.argpartition(a=row.data, kth=_k, axis=0)[:k]
+            similarity = np.take_along_axis(arr=row.data, indices=ind, axis=0)
+            indices = np.take_along_axis(arr=row.indices, indices=ind, axis=0)
+            ind = np.argsort(a=similarity, axis=0)
+            scores.append(-1 * np.take_along_axis(arr=similarity, indices=ind, axis=0))
+            matchs.append(np.take_along_axis(arr=indices, indices=ind, axis=0))
+        return matchs, scores
 
-    def _rank(
-        self, scores: torch.Tensor, documents: list[list[dict]], k: int
+    def __call__(
+        self,
+        queries_embeddings: dict[str, csr_matrix],
+        k: int = None,
+        batch_size: int = 2000,
+        tqdm_bar: bool = True,
     ) -> list[list[dict]]:
-        """Rank documents by scores.
+        """Retrieve documents from batch of queries.
 
         Parameters
         ----------
-        scores
-            Scores.
-        documents
-            Documents.
+        queries_embeddings
+            Queries embeddings.
         k
-            Number of documents to retrieve.
+            Number of documents to retrieve. Default is `None`, i.e all documents that match the
+            query will be retrieved.
+        batch_size
+            Batch size to use to retrieve documents.
         """
+        k = k if k is not None else self.n_documents
+
         ranked = []
 
-        for query_scores in scores:
-            top_k = torch.topk(
-                input=query_scores,
-                k=min(k, len(documents)) if k is not None else len(documents),
-                dim=-1,
-            )
-
-            ranked.append(
-                [
-                    {**documents[indice], "similarity": similarity}
-                    for indice, similarity in zip(top_k.indices, top_k.values.tolist())
-                ]
-            )
+        for batch_embeddings in utils.batchify(
+            list(queries_embeddings.values()),
+            batch_size=batch_size,
+            desc=f"{self.__class__.__name__} retriever",
+            tqdm_bar=tqdm_bar,
+        ):
+            # self.matrix is a csr matrix of shape (n_features, n_documents)
+            # Transform output a csr matrix of shape (n_queries, n_features)
+            similarities = -1 * vstack(blocks=batch_embeddings).dot(self.matrix)
+            batch_match, batch_similarities = self.top_k(similarities=similarities, k=k)
+
+            for match, similarities in zip(batch_match, batch_similarities):
+                ranked.append(
+                    [
+                        {**self.documents[idx], "similarity": similarity}
+                        for idx, similarity in zip(match, similarities)
+                        if similarity > 0
+                    ]
+                )
 
         return ranked
```

### Comparing `neural_cherche-1.1.0/neural_cherche/retrieve/sparse_embed.py` & `neural_cherche-1.3.0/neural_cherche/retrieve/sparse_embed.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 from .. import models, utils
 from .tfidf import TfIdf
 
 __all__ = ["SparseEmbed"]
 
 
 class SparseEmbed(TfIdf):
-    """Retriever class.
+    """SparseEmbed retriever.
 
     Parameters
     ----------
     key
         Document unique identifier.
     on
         Document texts.
     model
-        SparsEmbed model.
+        SparseEmbed model.
 
     Examples
     --------
     >>> from neural_cherche import models, retrieve
     >>> from pprint import pprint
     >>> import torch
 
@@ -85,14 +85,15 @@
 
     def __init__(
         self,
         key: str,
         on: list[str],
         model: models.SparseEmbed,
         tokenizer_parallelism: str = "false",
+        device: str = None,
     ) -> None:
         super().__init__(
             key=key,
             on=on,
         )
 
         self.model = model
@@ -100,21 +101,24 @@
         # TfIdf Retriever.
         self.fit = True
 
         # Documents embeddings and activations store.
         self.documents_embeddings, self.documents_activations = [], []
 
         os.environ["TOKENIZERS_PARALLELISM"] = tokenizer_parallelism
+        self.device = device if device is not None else self.model.device
 
     def encode_queries(
         self,
         queries: list[str],
         batch_size: int = 32,
         tqdm_bar: bool = True,
         query_mode: bool = True,
+        warn_duplicates: bool = True,
+        desc: str = "embeddings queries",
         **kwargs,
     ) -> dict[str, dict[str, torch.Tensor]]:
         """Encode queries.
 
         Parameters
         ----------
         queries
@@ -125,15 +129,15 @@
             Display a tqdm bar.
         """
         embeddings = collections.defaultdict(dict)
 
         for batch in utils.batchify(
             queries,
             batch_size=batch_size,
-            desc=f"{self.__class__.__name__} encoder",
+            desc=f"{self.__class__.__name__} {desc}",
             tqdm_bar=tqdm_bar,
         ):
             queries_embeddings = self.model.encode(
                 texts=batch,
                 query_mode=query_mode,
                 **kwargs,
             )
@@ -153,37 +157,42 @@
                 queries_embeddings["activations"],
                 queries_embeddings["embeddings"],
             ):
                 embeddings[query]["sparse_activations"] = csr_matrix(sparse_activations)
                 embeddings[query]["activations"] = activations
                 embeddings[query]["embeddings"] = tokens_embeddings
 
+        if len(embeddings) != len(queries) and warn_duplicates:
+            utils.duplicates_queries_warning()
+
         return embeddings
 
     def encode_documents(
         self,
         documents: list[dict],
         batch_size: int = 32,
         tqdm_bar: bool = True,
         query_mode: bool = False,
+        desc: str = "embeddings documents",
         **kwargs,
     ) -> dict[str, dict[str, torch.Tensor]]:
         """Encode documents.
 
         Parameters
         ----------
         documents
             List of documents to encode.
         """
         embeddings = collections.defaultdict(dict)
 
         for batch in utils.batchify(
-            documents,
+            X=documents,
             batch_size=batch_size,
             tqdm_bar=tqdm_bar,
+            desc=f"{self.__class__.__name__} {desc}",
         ):
             documents_embeddings = self.model.encode(
                 texts=[
                     " ".join([doc.get(field, "") for field in self.on]) for doc in batch
                 ],
                 query_mode=query_mode,
                 **kwargs,
@@ -236,17 +245,18 @@
         ).T.tocsr()
 
         self.matrix = matrix if self.matrix is None else hstack((self.matrix, matrix))
 
         for key, embeddings in documents_embeddings.items():
             self.documents_embeddings.append(
                 {
-                    token.item(): token_embedding
+                    token: token_embedding
                     for token, token_embedding in zip(
-                        embeddings["activations"], embeddings["embeddings"]
+                        embeddings["activations"],
+                        embeddings["embeddings"],
                     )
                 }
             )
             self.documents_activations.append(embeddings["activations"])
 
         for key in documents_embeddings:
             self.documents.append({self.key: key})
@@ -285,24 +295,22 @@
             batch_size=batch_size,
             desc=f"{self.__class__.__name__} retriever",
             tqdm_bar=tqdm_bar,
         ):
             embeddings = {
                 "activations": torch.stack(
                     tensors=[
-                        torch.tensor(
-                            data=query["activations"], device=self.model.device
-                        )
+                        torch.tensor(data=query["activations"], device=self.device)
                         for query in queries_batch
                     ],
                     dim=0,
                 ),
                 "embeddings": torch.stack(
                     tensors=[
-                        torch.tensor(data=query["embeddings"], device=self.model.device)
+                        torch.tensor(data=query["embeddings"], device=self.device)
                         for query in queries_batch
                     ],
                     dim=0,
                 ),
                 "sparse_activations": vstack(
                     blocks=[query["sparse_activations"] for query in queries_batch]
                 ),
@@ -326,39 +334,41 @@
         Parameters
         ----------
         embeddings
             Input embeddings.
         k
             Number of documents to retrieve.
         """
-        similarities = -1 * embeddings["sparse_activations"].dot(self.matrix)
-        sparse_matchs, _ = self.top_k(similarities=similarities, k=k)
+        sparse_matchs = [
+            activations.indices
+            for activations in (embeddings["sparse_activations"].dot(self.matrix))
+        ]
 
         documents_activations = [
             [
                 torch.tensor(
-                    data=self.documents_activations[document], device=self.model.device
+                    data=self.documents_activations[document], device=self.device
                 )
                 for document in query_matchs
             ]
             for query_matchs in sparse_matchs
         ]
 
         intersections = self._get_intersection(
             queries_activations=embeddings["activations"],
             documents_activations=documents_activations,
         )
 
         queries_embeddings = [
             {
-                token.item(): token_embedding
+                token: token_embedding
                 for token, token_embedding in zip(query_activations, query_embeddings)
             }
             for query_activations, query_embeddings in zip(
-                embeddings["activations"],
+                embeddings["activations"].tolist(),
                 embeddings["embeddings"],
             )
         ]
 
         dense_scores = self._get_scores(
             queries_embeddings=queries_embeddings,
             documents_embeddings=[
@@ -391,14 +401,18 @@
         for query_scores, query_sparse_matchs in zip(dense_scores, sparse_matchs):
             query_scores, query_matchs = torch.topk(
                 input=query_scores,
                 k=min(k, query_scores.shape[0]),
                 dim=-1,
             )
 
+            if len(query_scores) == 0:
+                ranked.append([])
+                continue
+
             query_matchs = np.take(
                 a=query_sparse_matchs, indices=query_matchs.cpu().detach().numpy()
             )
 
             query_scores = query_scores.tolist()
 
             ranked.append(
@@ -466,15 +480,15 @@
                 if len(intersection) > 0:
                     query_documents_scores.append(
                         torch.sum(
                             input=torch.stack(
                                 tensors=[
                                     torch.tensor(
                                         data=document_embedding[token],
-                                        device=self.model.device,
+                                        device=self.device,
                                     )
                                     for token in intersection
                                 ],
                                 dim=0,
                             )
                             * torch.stack(
                                 tensors=[
@@ -483,15 +497,19 @@
                                 dim=0,
                             )
                         )
                     )
 
                 else:
                     query_documents_scores.append(
-                        torch.tensor(data=0.0, device=self.model.device)
+                        torch.tensor(data=0.0, device=self.device)
                     )
 
+            if not query_documents_scores:
+                queries_documents_scores.append([])
+                continue
+
             queries_documents_scores.append(
                 torch.stack(tensors=query_documents_scores, dim=0)
             )
 
         return queries_documents_scores
```

### Comparing `neural_cherche-1.1.0/neural_cherche/retrieve/splade.py` & `neural_cherche-1.3.0/neural_cherche/retrieve/splade.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 
     def encode_documents(
         self,
         documents: list[dict],
         batch_size: int = 32,
         tqdm_bar: bool = True,
         query_mode: bool = False,
+        desc: str = "documents embeddings",
         **kwargs,
     ) -> dict[str, csr_matrix]:
         """Encode queries into sparse matrix.
 
         Parameters
         ----------
         documents
@@ -116,14 +117,15 @@
         """
         documents_embeddings = {}
 
         for batch_documents in utils.batchify(
             documents,
             batch_size=batch_size,
             tqdm_bar=tqdm_bar,
+            desc=f"{self.__class__.__name__} {desc}",
         ):
             embeddings = self.model.encode(
                 [
                     " ".join([doc.get(field, "") for field in self.on])
                     for doc in batch_documents
                 ],
                 query_mode=query_mode,
@@ -140,14 +142,16 @@
 
     def encode_queries(
         self,
         queries: list[str],
         batch_size: int = 32,
         tqdm_bar: bool = True,
         query_mode: bool = True,
+        desc: str = "queries embeddings",
+        warn_duplicates: bool = True,
         **kwargs,
     ) -> dict[str, csr_matrix]:
         """Encode queries into sparse matrix.
 
         Parameters
         ----------
         documents
@@ -160,21 +164,25 @@
         """
         queries_embeddings = {}
 
         for batch_queries in utils.batchify(
             queries,
             batch_size=batch_size,
             tqdm_bar=tqdm_bar,
+            desc=f"{self.__class__.__name__}  {desc}",
         ):
             embeddings = self.model.encode(
                 batch_queries,
                 query_mode=query_mode,
                 **kwargs,
             )
 
             sparse_activations = csr_matrix(
                 embeddings["sparse_activations"].detach().cpu()
             )
             for query, sparse_activation in zip(batch_queries, sparse_activations):
                 queries_embeddings[query] = sparse_activation
 
+        if len(embeddings) != len(queries) and warn_duplicates:
+            utils.duplicates_queries_warning()
+
         return queries_embeddings
```

### Comparing `neural_cherche-1.1.0/neural_cherche/train/train_colbert.py` & `neural_cherche-1.3.0/neural_cherche/train/train_colbert.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.1.0/neural_cherche/train/train_sparse_embed.py` & `neural_cherche-1.3.0/neural_cherche/train/train_sparse_embed.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.1.0/neural_cherche/train/train_splade.py` & `neural_cherche-1.3.0/neural_cherche/train/train_splade.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.1.0/neural_cherche/utils/colbert_scores.py` & `neural_cherche-1.3.0/neural_cherche/utils/colbert_scores.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.1.0/neural_cherche/utils/dense_scores.py` & `neural_cherche-1.3.0/neural_cherche/utils/dense_scores.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.1.0/neural_cherche/utils/freeze.py` & `neural_cherche-1.3.0/neural_cherche/utils/freeze.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.1.0/neural_cherche/utils/iter.py` & `neural_cherche-1.3.0/neural_cherche/utils/iter.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.1.0/neural_cherche/utils/sparse_scores.py` & `neural_cherche-1.3.0/neural_cherche/utils/sparse_scores.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.1.0/neural_cherche.egg-info/SOURCES.txt` & `neural_cherche-1.3.0/neural_cherche.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,26 @@
 neural_cherche/models/__init__.py
 neural_cherche/models/base.py
 neural_cherche/models/colbert.py
 neural_cherche/models/sparse_embed.py
 neural_cherche/models/splade.py
 neural_cherche/rank/__init__.py
 neural_cherche/rank/colbert.py
+neural_cherche/rank/sparse_embed.py
 neural_cherche/retrieve/__init__.py
+neural_cherche/retrieve/bm25.py
 neural_cherche/retrieve/colbert.py
 neural_cherche/retrieve/sparse_embed.py
 neural_cherche/retrieve/splade.py
 neural_cherche/retrieve/tfidf.py
 neural_cherche/train/__init__.py
 neural_cherche/train/train_colbert.py
 neural_cherche/train/train_sparse_embed.py
 neural_cherche/train/train_splade.py
 neural_cherche/utils/__init__.py
 neural_cherche/utils/colbert_scores.py
 neural_cherche/utils/dense_scores.py
 neural_cherche/utils/evaluate.py
 neural_cherche/utils/freeze.py
 neural_cherche/utils/iter.py
-neural_cherche/utils/sparse_scores.py
+neural_cherche/utils/sparse_scores.py
+neural_cherche/utils/warnings.py
```

### Comparing `neural_cherche-1.1.0/setup.py` & `neural_cherche-1.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import setuptools
 
 from neural_cherche.__version__ import __version__
 
-with open("README.md", "r", encoding="utf-8") as fh:
+with open(file="README.md", mode="r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 base_packages = [
     "torch >= 1.13",
     "tqdm >= 4.66",
     "transformers >= 4.34.0",
     "sentence-transformers >= 2.2.2",
+    "lenlp >= 1.0.3",
 ]
 
+
 eval = ["ranx >= 0.3.16", "beir >= 2.0.0"]
 
-dev = ["mkdocs-material == 9.2.8"]
+dev = [
+    "mkdocs-material == 9.2.8",
+    "mkdocs-awesome-pages-plugin == 2.9.2",
+    " mkdocs-jupyter == 0.24.7",
+]
 
 setuptools.setup(
     name="neural_cherche",
     version=f"{__version__}",
     license="",
     author="Raphael Sourty",
     author_email="raphael.sourty@gmail.com",
```

