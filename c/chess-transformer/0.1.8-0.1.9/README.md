# Comparing `tmp/chess_transformer-0.1.8.tar.gz` & `tmp/chess_transformer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess_transformer-0.1.8.tar", last modified: Tue May 28 08:55:09 2024, max compression
+gzip compressed data, was "chess_transformer-0.1.9.tar", last modified: Tue May 28 09:08:25 2024, max compression
```

## Comparing `chess_transformer-0.1.8.tar` & `chess_transformer-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:55:09.312162 chess_transformer-0.1.8/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      436 2024-05-28 08:55:09.312162 chess_transformer-0.1.8/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       42 2024-05-27 14:59:07.000000 chess_transformer-0.1.8/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      582 2024-05-28 08:55:06.000000 chess_transformer-0.1.8/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-28 08:55:09.312162 chess_transformer-0.1.8/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:55:09.302162 chess_transformer-0.1.8/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:55:09.302162 chess_transformer-0.1.8/src/chess_transformer/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      125 2024-05-27 15:03:14.000000 chess_transformer-0.1.8/src/chess_transformer/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      302 2024-05-27 18:53:00.000000 chess_transformer-0.1.8/src/chess_transformer/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      342 2024-05-28 08:55:02.000000 chess_transformer-0.1.8/src/chess_transformer/_vocab.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:55:09.312162 chess_transformer-0.1.8/src/chess_transformer/pytorch/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-27 15:05:21.000000 chess_transformer-0.1.8/src/chess_transformer/pytorch/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      378 2024-05-27 19:07:13.000000 chess_transformer-0.1.8/src/chess_transformer/pytorch/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      250 2024-05-27 15:07:20.000000 chess_transformer-0.1.8/src/chess_transformer/pytorch/_loss.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1326 2024-05-27 19:13:32.000000 chess_transformer-0.1.8/src/chess_transformer/pytorch/data.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1166 2024-05-28 08:39:47.000000 chess_transformer-0.1.8/src/chess_transformer/pytorch/decode.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1375 2024-05-27 19:34:27.000000 chess_transformer-0.1.8/src/chess_transformer/pytorch/model.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      909 2024-05-27 19:32:53.000000 chess_transformer-0.1.8/src/chess_transformer/pytorch/pos_enc.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1484 2024-05-27 18:58:37.000000 chess_transformer-0.1.8/src/chess_transformer/samples.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 08:55:09.312162 chess_transformer-0.1.8/src/chess_transformer.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      436 2024-05-28 08:55:09.000000 chess_transformer-0.1.8/src/chess_transformer.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      664 2024-05-28 08:55:09.000000 chess_transformer-0.1.8/src/chess_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-28 08:55:09.000000 chess_transformer-0.1.8/src/chess_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-28 08:55:09.000000 chess_transformer-0.1.8/src/chess_transformer.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-05-28 08:55:09.000000 chess_transformer-0.1.8/src/chess_transformer.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 09:08:25.812159 chess_transformer-0.1.9/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      436 2024-05-28 09:08:25.812159 chess_transformer-0.1.9/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       42 2024-05-27 14:59:07.000000 chess_transformer-0.1.9/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      582 2024-05-28 09:08:20.000000 chess_transformer-0.1.9/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-28 09:08:25.812159 chess_transformer-0.1.9/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 09:08:25.792159 chess_transformer-0.1.9/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 09:08:25.802159 chess_transformer-0.1.9/src/chess_transformer/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      125 2024-05-27 15:03:14.000000 chess_transformer-0.1.9/src/chess_transformer/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      302 2024-05-27 18:53:00.000000 chess_transformer-0.1.9/src/chess_transformer/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      342 2024-05-28 08:55:02.000000 chess_transformer-0.1.9/src/chess_transformer/_vocab.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 09:08:25.802159 chess_transformer-0.1.9/src/chess_transformer/pytorch/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-27 15:05:21.000000 chess_transformer-0.1.9/src/chess_transformer/pytorch/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      378 2024-05-27 19:07:13.000000 chess_transformer-0.1.9/src/chess_transformer/pytorch/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1028 2024-05-28 09:06:59.000000 chess_transformer-0.1.9/src/chess_transformer/pytorch/_loss.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1268 2024-05-28 09:04:15.000000 chess_transformer-0.1.9/src/chess_transformer/pytorch/data.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1166 2024-05-28 08:39:47.000000 chess_transformer-0.1.9/src/chess_transformer/pytorch/decode.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1407 2024-05-28 09:01:57.000000 chess_transformer-0.1.9/src/chess_transformer/pytorch/model.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      909 2024-05-27 19:32:53.000000 chess_transformer-0.1.9/src/chess_transformer/pytorch/pos_enc.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1484 2024-05-27 18:58:37.000000 chess_transformer-0.1.9/src/chess_transformer/samples.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-28 09:08:25.802159 chess_transformer-0.1.9/src/chess_transformer.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      436 2024-05-28 09:08:25.000000 chess_transformer-0.1.9/src/chess_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      664 2024-05-28 09:08:25.000000 chess_transformer-0.1.9/src/chess_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-28 09:08:25.000000 chess_transformer-0.1.9/src/chess_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       54 2024-05-28 09:08:25.000000 chess_transformer-0.1.9/src/chess_transformer.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-05-28 09:08:25.000000 chess_transformer-0.1.9/src/chess_transformer.egg-info/top_level.txt
```

### Comparing `chess_transformer-0.1.8/pyproject.toml` & `chess_transformer-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chess-transformer"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "package_description"
 dependencies = [
   "chess", "jaxtyping", "haskellian", "chess-notation", "chess-utils"
 ]
```

### Comparing `chess_transformer-0.1.8/src/chess_transformer/pytorch/data.py` & `chess_transformer-0.1.9/src/chess_transformer/pytorch/data.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,17 +20,16 @@
   input_ids = [vocab[tok] for tok in tokens]
   return Sample(torch.tensor(input_ids), ends, torch.tensor(labs))
 
 def collate_fn(batch: Sequence[Sample], pad_token_id: int, ignore_idx: int = -100) -> Batch:
 
   input_ids, ends, labs = I.unzip(batch)
   batch_size = len(input_ids)
-  max_input_len = max(len(x) for x in input_ids)
-  max_lab_len = max(len(x) for x in labs)
-  padded_input_ids = torch.full((batch_size, max_input_len), fill_value=pad_token_id)
-  padded_labs = torch.full((batch_size, max_lab_len, 5), fill_value=ignore_idx)
+  max_len = max(len(x) for x in input_ids)
+  padded_input_ids = torch.full((batch_size, max_len), fill_value=pad_token_id)
+  padded_labs = torch.full((batch_size, max_len, 5), fill_value=ignore_idx)
 
   for i in range(batch_size):
     padded_input_ids[i, :len(input_ids[i])] = input_ids[i]
     padded_labs[i, :len(labs[i])] = labs[i]
 
   return Batch(padded_input_ids, ends, padded_labs)
```

### Comparing `chess_transformer-0.1.8/src/chess_transformer/pytorch/decode.py` & `chess_transformer-0.1.9/src/chess_transformer/pytorch/decode.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.8/src/chess_transformer/pytorch/model.py` & `chess_transformer-0.1.9/src/chess_transformer/pytorch/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Sequence
+from typing import Sequence, Protocol
 from jaxtyping import Int, Float
 import torch
 from torch import nn, Tensor
 from transformers import BertConfig, BertModel
 from .pos_enc import segment_encoding, positional_encoding
 
 class ChessBERT(nn.Module):
@@ -36,8 +36,9 @@
       segment_encoding(input_ids.size(1), ends=ends, encoding=self.pos_enc)
       for ends in word_ends
     ])
     embedded: Float[Tensor, 'batch seq_len hidden_size'] = self.embedding(input_ids)
     x: Float[Tensor, 'batch seq_len hidden_size'] = embedded + pos_enc
     y = self.bert(inputs_embeds=x)
     seq_output = y.last_hidden_state
+    return seq_output
     return self.fc(seq_output)
```

### Comparing `chess_transformer-0.1.8/src/chess_transformer/pytorch/pos_enc.py` & `chess_transformer-0.1.9/src/chess_transformer/pytorch/pos_enc.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.8/src/chess_transformer/samples.py` & `chess_transformer-0.1.9/src/chess_transformer/samples.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.8/src/chess_transformer.egg-info/SOURCES.txt` & `chess_transformer-0.1.9/src/chess_transformer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

