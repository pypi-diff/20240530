# Comparing `tmp/rotary_embedding_torch-0.6.1.tar.gz` & `tmp/rotary_embedding_torch-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotary_embedding_torch-0.6.1.tar", last modified: Sat May 11 15:32:54 2024, max compression
+gzip compressed data, was "rotary_embedding_torch-0.6.2.tar", last modified: Thu May 30 21:14:12 2024, max compression
```

## Comparing `rotary_embedding_torch-0.6.1.tar` & `rotary_embedding_torch-0.6.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:32:54.135856 rotary_embedding_torch-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-11 15:32:49.000000 rotary_embedding_torch-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-11 15:32:54.131856 rotary_embedding_torch-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-11 15:32:49.000000 rotary_embedding_torch-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:32:54.131856 rotary_embedding_torch-0.6.1/rotary_embedding_torch/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-11 15:32:49.000000 rotary_embedding_torch-0.6.1/rotary_embedding_torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-05-11 15:32:49.000000 rotary_embedding_torch-0.6.1/rotary_embedding_torch/rotary_embedding_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:32:54.131856 rotary_embedding_torch-0.6.1/rotary_embedding_torch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-11 15:32:54.000000 rotary_embedding_torch-0.6.1/rotary_embedding_torch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-11 15:32:54.000000 rotary_embedding_torch-0.6.1/rotary_embedding_torch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 15:32:54.000000 rotary_embedding_torch-0.6.1/rotary_embedding_torch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-11 15:32:54.000000 rotary_embedding_torch-0.6.1/rotary_embedding_torch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-11 15:32:54.000000 rotary_embedding_torch-0.6.1/rotary_embedding_torch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 15:32:54.135856 rotary_embedding_torch-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-11 15:32:49.000000 rotary_embedding_torch-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:14:12.382393 rotary_embedding_torch-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-30 21:14:08.000000 rotary_embedding_torch-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-30 21:14:12.382393 rotary_embedding_torch-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-30 21:14:08.000000 rotary_embedding_torch-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:14:12.382393 rotary_embedding_torch-0.6.2/rotary_embedding_torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-30 21:14:08.000000 rotary_embedding_torch-0.6.2/rotary_embedding_torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-05-30 21:14:08.000000 rotary_embedding_torch-0.6.2/rotary_embedding_torch/rotary_embedding_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:14:12.382393 rotary_embedding_torch-0.6.2/rotary_embedding_torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-30 21:14:12.000000 rotary_embedding_torch-0.6.2/rotary_embedding_torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-30 21:14:12.000000 rotary_embedding_torch-0.6.2/rotary_embedding_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 21:14:12.000000 rotary_embedding_torch-0.6.2/rotary_embedding_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 21:14:12.000000 rotary_embedding_torch-0.6.2/rotary_embedding_torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 21:14:12.000000 rotary_embedding_torch-0.6.2/rotary_embedding_torch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 21:14:12.382393 rotary_embedding_torch-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-30 21:14:08.000000 rotary_embedding_torch-0.6.2/setup.py
```

### Comparing `rotary_embedding_torch-0.6.1/LICENSE` & `rotary_embedding_torch-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rotary_embedding_torch-0.6.1/PKG-INFO` & `rotary_embedding_torch-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotary-embedding-torch
-Version: 0.6.1
+Version: 0.6.2
 Summary: Rotary Embedding - Pytorch
 Home-page: https://github.com/lucidrains/rotary-embedding-torch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,positional embedding
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rotary_embedding_torch-0.6.1/README.md` & `rotary_embedding_torch-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `rotary_embedding_torch-0.6.1/rotary_embedding_torch/rotary_embedding_torch.py` & `rotary_embedding_torch-0.6.2/rotary_embedding_torch/rotary_embedding_torch.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,26 +30,30 @@
     x = rearrange(x, '... (d r) -> ... d r', r = 2)
     x1, x2 = x.unbind(dim = -1)
     x = torch.stack((-x2, x1), dim = -1)
     return rearrange(x, '... d r -> ... (d r)')
 
 @autocast(enabled = False)
 def apply_rotary_emb(freqs, t, start_index = 0, scale = 1., seq_dim = -2):
+    dtype = t.dtype
+
     if t.ndim == 3:
         seq_len = t.shape[seq_dim]
-        freqs = freqs[-seq_len:].to(t)
+        freqs = freqs[-seq_len:]
 
     rot_dim = freqs.shape[-1]
     end_index = start_index + rot_dim
 
     assert rot_dim <= t.shape[-1], f'feature dimension {t.shape[-1]} is not of sufficient size to rotate in all the positions {rot_dim}'
 
     t_left, t, t_right = t[..., :start_index], t[..., start_index:end_index], t[..., end_index:]
     t = (t * freqs.cos() * scale) + (rotate_half(t) * freqs.sin() * scale)
-    return torch.cat((t_left, t, t_right), dim = -1)
+    out = torch.cat((t_left, t, t_right), dim = -1)
+
+    return out.type(dtype)
 
 # learned rotation helpers
 
 def apply_learned_rotations(rotations, t, start_index = 0, freq_ranges = None):
     if exists(freq_ranges):
         rotations = einsum('..., f -> ... f', rotations, freq_ranges)
         rotations = rearrange(rotations, '... r f -> ... (r f)')
```

### Comparing `rotary_embedding_torch-0.6.1/rotary_embedding_torch.egg-info/PKG-INFO` & `rotary_embedding_torch-0.6.2/rotary_embedding_torch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotary-embedding-torch
-Version: 0.6.1
+Version: 0.6.2
 Summary: Rotary Embedding - Pytorch
 Home-page: https://github.com/lucidrains/rotary-embedding-torch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,positional embedding
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rotary_embedding_torch-0.6.1/setup.py` & `rotary_embedding_torch-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'rotary-embedding-torch',
   packages = find_packages(),
-  version = '0.6.1',
+  version = '0.6.2',
   license='MIT',
   description = 'Rotary Embedding - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/rotary-embedding-torch',
   keywords = [
```

