# Comparing `tmp/lycoris_lora-3.0.0.dev4.tar.gz` & `tmp/lycoris_lora-3.0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-3.0.0.dev4.tar", last modified: Sat May 25 03:29:41 2024, max compression
+gzip compressed data, was "lycoris_lora-3.0.0.dev5.tar", last modified: Thu May 30 12:51:50 2024, max compression
```

## Comparing `lycoris_lora-3.0.0.dev4.tar` & `lycoris_lora-3.0.0.dev5.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 03:29:41.523151 lycoris_lora-3.0.0.dev4/
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-3.0.0.dev4/LICENSE.md
--rw-rw-rw-   0        0        0      444 2024-05-25 03:29:41.522152 lycoris_lora-3.0.0.dev4/PKG-INFO
--rw-rw-rw-   0        0        0    12433 2024-05-15 08:22:33.000000 lycoris_lora-3.0.0.dev4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 03:29:41.494119 lycoris_lora-3.0.0.dev4/lycoris/
--rw-rw-rw-   0        0        0      588 2024-05-18 10:27:24.000000 lycoris_lora-3.0.0.dev4/lycoris/__init__.py
--rw-rw-rw-   0        0        0     2537 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev4/lycoris/config.py
-drwxrwxrwx   0        0        0        0 2024-05-25 03:29:41.496122 lycoris_lora-3.0.0.dev4/lycoris/functional/
--rw-rw-rw-   0        0        0      251 2024-05-17 14:23:10.000000 lycoris_lora-3.0.0.dev4/lycoris/functional/__init__.py
--rw-rw-rw-   0        0        0     2429 2024-05-18 15:09:35.000000 lycoris_lora-3.0.0.dev4/lycoris/functional/general.py
--rw-rw-rw-   0        0        0     3354 2024-05-17 14:23:10.000000 lycoris_lora-3.0.0.dev4/lycoris/functional/locon.py
--rw-rw-rw-   0        0        0     5259 2024-05-17 12:55:00.000000 lycoris_lora-3.0.0.dev4/lycoris/functional/loha.py
--rw-rw-rw-   0        0        0    31780 2024-05-18 10:06:20.000000 lycoris_lora-3.0.0.dev4/lycoris/kohya.py
--rw-rw-rw-   0        0        0     1053 2024-02-05 11:33:20.000000 lycoris_lora-3.0.0.dev4/lycoris/logging.py
-drwxrwxrwx   0        0        0        0 2024-05-25 03:29:41.502122 lycoris_lora-3.0.0.dev4/lycoris/modules/
--rw-rw-rw-   0        0        0     4201 2024-05-03 13:52:01.000000 lycoris_lora-3.0.0.dev4/lycoris/modules/__init__.py
--rw-rw-rw-   0        0        0     9576 2024-05-24 08:45:31.000000 lycoris_lora-3.0.0.dev4/lycoris/modules/base.py
--rw-rw-rw-   0        0        0     8349 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev4/lycoris/modules/boft.py
--rw-rw-rw-   0        0        0     7743 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev4/lycoris/modules/diag_oft.py
--rw-rw-rw-   0        0        0     4395 2024-05-03 12:40:31.000000 lycoris_lora-3.0.0.dev4/lycoris/modules/dylora.py
--rw-rw-rw-   0        0        0     6439 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev4/lycoris/modules/full.py
--rw-rw-rw-   0        0        0     9077 2024-05-25 03:28:17.000000 lycoris_lora-3.0.0.dev4/lycoris/modules/glora.py
--rw-rw-rw-   0        0        0     6144 2024-05-25 03:27:52.000000 lycoris_lora-3.0.0.dev4/lycoris/modules/ia3.py
--rw-rw-rw-   0        0        0    11601 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev4/lycoris/modules/locon.py
--rw-rw-rw-   0        0        0    11372 2024-05-25 03:26:29.000000 lycoris_lora-3.0.0.dev4/lycoris/modules/loha.py
--rw-rw-rw-   0        0        0    16571 2024-05-25 03:28:25.000000 lycoris_lora-3.0.0.dev4/lycoris/modules/lokr.py
--rw-rw-rw-   0        0        0     3557 2024-05-18 09:12:34.000000 lycoris_lora-3.0.0.dev4/lycoris/modules/norms.py
-drwxrwxrwx   0        0        0        0 2024-05-25 03:29:41.504126 lycoris_lora-3.0.0.dev4/lycoris/utils/
--rw-rw-rw-   0        0        0    23287 2024-03-23 07:38:25.000000 lycoris_lora-3.0.0.dev4/lycoris/utils/__init__.py
--rw-rw-rw-   0        0        0      497 2024-03-13 17:06:13.000000 lycoris_lora-3.0.0.dev4/lycoris/utils/bnb.py
--rw-rw-rw-   0        0        0     1078 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev4/lycoris/utils/logger.py
--rw-rw-rw-   0        0        0      190 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev4/lycoris/utils/preset.py
--rw-rw-rw-   0        0        0      251 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev4/lycoris/utils/xformers_utils.py
--rw-rw-rw-   0        0        0    18779 2024-05-15 08:22:10.000000 lycoris_lora-3.0.0.dev4/lycoris/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-05-25 03:29:41.522152 lycoris_lora-3.0.0.dev4/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      444 2024-05-25 03:29:41.000000 lycoris_lora-3.0.0.dev4/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      879 2024-05-25 03:29:41.000000 lycoris_lora-3.0.0.dev4/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 03:29:41.000000 lycoris_lora-3.0.0.dev4/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-11-06 13:42:23.000000 lycoris_lora-3.0.0.dev4/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2024-05-25 03:29:41.000000 lycoris_lora-3.0.0.dev4/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-25 03:29:41.000000 lycoris_lora-3.0.0.dev4/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 03:29:41.523151 lycoris_lora-3.0.0.dev4/setup.cfg
--rw-rw-rw-   0        0        0      567 2024-05-25 03:29:37.000000 lycoris_lora-3.0.0.dev4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:51:50.220299 lycoris_lora-3.0.0.dev5/
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-3.0.0.dev5/LICENSE.md
+-rw-rw-rw-   0        0        0      465 2024-05-30 12:51:50.219298 lycoris_lora-3.0.0.dev5/PKG-INFO
+-rw-rw-rw-   0        0        0    12433 2024-05-15 08:22:33.000000 lycoris_lora-3.0.0.dev5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 12:51:50.192653 lycoris_lora-3.0.0.dev5/lycoris/
+-rw-rw-rw-   0        0        0      588 2024-05-18 10:27:24.000000 lycoris_lora-3.0.0.dev5/lycoris/__init__.py
+-rw-rw-rw-   0        0        0     2537 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev5/lycoris/config.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:51:50.194652 lycoris_lora-3.0.0.dev5/lycoris/functional/
+-rw-rw-rw-   0        0        0      251 2024-05-17 14:23:10.000000 lycoris_lora-3.0.0.dev5/lycoris/functional/__init__.py
+-rw-rw-rw-   0        0        0     2499 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev5/lycoris/functional/general.py
+-rw-rw-rw-   0        0        0     3186 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev5/lycoris/functional/locon.py
+-rw-rw-rw-   0        0        0     6387 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev5/lycoris/functional/loha.py
+-rw-rw-rw-   0        0        0    31398 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev5/lycoris/kohya.py
+-rw-rw-rw-   0        0        0     1053 2024-02-05 11:33:20.000000 lycoris_lora-3.0.0.dev5/lycoris/logging.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:51:50.199285 lycoris_lora-3.0.0.dev5/lycoris/modules/
+-rw-rw-rw-   0        0        0     4461 2024-05-30 12:50:16.000000 lycoris_lora-3.0.0.dev5/lycoris/modules/__init__.py
+-rw-rw-rw-   0        0        0     9568 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev5/lycoris/modules/base.py
+-rw-rw-rw-   0        0        0     8349 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev5/lycoris/modules/boft.py
+-rw-rw-rw-   0        0        0     7743 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev5/lycoris/modules/diag_oft.py
+-rw-rw-rw-   0        0        0     7032 2024-05-25 08:12:37.000000 lycoris_lora-3.0.0.dev5/lycoris/modules/dylora.py
+-rw-rw-rw-   0        0        0     6439 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev5/lycoris/modules/full.py
+-rw-rw-rw-   0        0        0     9077 2024-05-25 03:28:17.000000 lycoris_lora-3.0.0.dev5/lycoris/modules/glora.py
+-rw-rw-rw-   0        0        0     5963 2024-05-25 03:59:59.000000 lycoris_lora-3.0.0.dev5/lycoris/modules/ia3.py
+-rw-rw-rw-   0        0        0    11562 2024-05-26 12:02:29.000000 lycoris_lora-3.0.0.dev5/lycoris/modules/locon.py
+-rw-rw-rw-   0        0        0    11372 2024-05-25 03:26:29.000000 lycoris_lora-3.0.0.dev5/lycoris/modules/loha.py
+-rw-rw-rw-   0        0        0    16571 2024-05-25 03:28:25.000000 lycoris_lora-3.0.0.dev5/lycoris/modules/lokr.py
+-rw-rw-rw-   0        0        0     3557 2024-05-18 09:12:34.000000 lycoris_lora-3.0.0.dev5/lycoris/modules/norms.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:51:50.202284 lycoris_lora-3.0.0.dev5/lycoris/utils/
+-rw-rw-rw-   0        0        0    24042 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev5/lycoris/utils/__init__.py
+-rw-rw-rw-   0        0        0      497 2024-03-13 17:06:13.000000 lycoris_lora-3.0.0.dev5/lycoris/utils/bnb.py
+-rw-rw-rw-   0        0        0      102 2024-05-25 08:12:37.000000 lycoris_lora-3.0.0.dev5/lycoris/utils/general.py
+-rw-rw-rw-   0        0        0     1078 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev5/lycoris/utils/logger.py
+-rw-rw-rw-   0        0        0      190 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev5/lycoris/utils/preset.py
+-rw-rw-rw-   0        0        0      251 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev5/lycoris/utils/xformers_utils.py
+-rw-rw-rw-   0        0        0    18777 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev5/lycoris/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:51:50.218298 lycoris_lora-3.0.0.dev5/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      465 2024-05-30 12:51:50.000000 lycoris_lora-3.0.0.dev5/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      904 2024-05-30 12:51:50.000000 lycoris_lora-3.0.0.dev5/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 12:51:50.000000 lycoris_lora-3.0.0.dev5/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-11-06 13:42:23.000000 lycoris_lora-3.0.0.dev5/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       23 2024-05-30 12:51:50.000000 lycoris_lora-3.0.0.dev5/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-30 12:51:50.000000 lycoris_lora-3.0.0.dev5/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 12:51:50.220299 lycoris_lora-3.0.0.dev5/setup.cfg
+-rw-rw-rw-   0        0        0      540 2024-05-25 08:12:50.000000 lycoris_lora-3.0.0.dev5/setup.py
```

### Comparing `lycoris_lora-3.0.0.dev4/LICENSE.md` & `lycoris_lora-3.0.0.dev5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev4/README.md` & `lycoris_lora-3.0.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/__init__.py` & `lycoris_lora-3.0.0.dev5/lycoris/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/config.py` & `lycoris_lora-3.0.0.dev5/lycoris/config.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/functional/general.py` & `lycoris_lora-3.0.0.dev5/lycoris/functional/general.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 
+FUNC_LIST = [None, None, F.linear, F.conv1d, F.conv2d, F.conv3d]
+
+
 def rebuild_tucker(t, wa, wb):
     rebuild2 = torch.einsum("i j ..., i p, j r -> p r ...", t, wa, wb)
     return rebuild2
 
 
 def factorization(dimension: int, factor: int = -1) -> tuple[int, int]:
     """
```

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/functional/locon.py` & `lycoris_lora-3.0.0.dev5/lycoris/functional/locon.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 import math
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-from .general import rebuild_tucker
+from .general import rebuild_tucker, FUNC_LIST
 
 
 def lora_weight_gen(org_weight, rank, tucker=True):
     """### lora_weight_gen
 
     Args:
-        out_dim (int): output dimension
-        in_dim (int): input dimension
+        org_weight (torch.Tensor): the weight tensor
         rank (int): low rank
 
     Returns:
-        torch.Tensor: down proj weight
-        torch.Tensor: up proj weight
-        torch.Tensor(optional): mid proj weight
+        torch.Tensor: down, up[, mid]
     """
     out_dim, in_dim, *k = org_weight.shape
     if k and tucker:
         down = torch.empty(rank, in_dim, *(1 for _ in k))
         up = torch.empty(out_dim, rank, *(1 for _ in k))
         mid = torch.empty(rank, rank, *k)
         nn.init.kaiming_uniform_(down, a=math.sqrt(5))
@@ -41,49 +38,45 @@
     """### lora_diff_weight
 
     Get ΔW = BA, where BA is low rank decomposition
 
     Args:
         d (torch.Tensor): weight of down proj linear/conv layer
         u (torch.Tensor): weight of up proj linear/conv layer
-        m (torch.Tensor, optional): weight of mid proj linear/conv layer, \
-            for tucker deomposition
+        m (torch.Tensor, optional): middle weight of tucker decomposition
         gamma (float, optional): scale factor, normally alpha/rank here
 
     Returns:
         torch.Tensor: ΔW
     """
-    assert d.size(0) == u.size(1)
     R, I, *k = d.shape
     O, R, *_ = u.shape
     u = u * gamma
 
     if m is None:
         result = u.reshape(-1, u.size(1)) @ d.reshape(d.size(0), -1)
     else:
         R, R, *k = m.shape
         u = u.reshape(u.size(0), -1).transpose(0, 1)
         d = d.reshape(d.size(0), -1)
         result = rebuild_tucker(m, u, d)
     return result.reshape(O, I, *k)
 
 
-FUNC_LIST = [None, None, F.linear, F.conv1d, F.conv2d, F.conv3d]
-
-
 def lora_bypass_forward_diff(x, d, u, m=None, gamma=1.0, extra_args={}):
     """### lora_bypass_forward_diff
 
     Args:
         x (torch.Tensor): input tensor
         d (torch.Tensor): weight of down proj linear/conv layer
         u (torch.Tensor): weight of up proj linear/conv layer
-        m (torch.Tensor, optional): weight of mid proj linear/conv layer, \
-            for tucker deomposition
+        m (torch.Tensor, optional): middle weight of tucker decomposition
         gamma (float, optional): scale factor, normally alpha/rank here
+        extra_args (dict, optional): extra args for forward func, \
+            e.g. padding, stride for Conv1/2/3d
 
     Returns:
         torch.Tensor: output tensor
     """
     if m is not None:
         down = FUNC_LIST[d.dim()](x, d)
         mid = FUNC_LIST[d.dim()](down, m, **extra_args)
```

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/functional/loha.py` & `lycoris_lora-3.0.0.dev5/lycoris/functional/loha.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+import math
+
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
+from .general import FUNC_LIST
+
 
 class HadaWeight(torch.autograd.Function):
     @staticmethod
     def forward(ctx, w1d, w1u, w2d, w2u, scale=torch.tensor(1)):
         ctx.save_for_backward(w1d, w1u, w2d, w2u, scale)
         diff_weight = ((w1u @ w1d) * (w2u @ w2d)) * scale
         return diff_weight
@@ -75,79 +79,111 @@
     return HadaWeight.apply(w1d, w1u, w2d, w2u, scale)
 
 
 def make_weight_tucker(t1, w1d, w1u, t2, w2d, w2u, scale):
     return HadaWeightTucker.apply(t1, w1d, w1u, t2, w2d, w2u, scale)
 
 
+def loha_weight_gen(org_weight, rank, tucker=True):
+    """### loha_weight_gen
+
+    Args:
+        org_weight (torch.Tensor): the weight tensor
+        rank (int): low rank
+
+    Returns:
+        torch.Tensor: w1d, w2d, w1u, w2u[, t1, t2]
+    """
+    out_dim, in_dim, *k = org_weight.shape
+    if k and tucker:
+        w1d = torch.empty(rank, in_dim)
+        w1u = torch.empty(rank, out_dim)
+        t1 = torch.empty(rank, rank, *k)
+        w2d = torch.empty(rank, in_dim)
+        w2u = torch.empty(rank, out_dim)
+        t2 = torch.empty(rank, rank, *k)
+        nn.init.normal_(w1d, std=1)
+        nn.init.constant_(w1u, 0)
+        nn.init.normal_(w2d, std=1)
+        nn.init.normal_(w2u, std=0.1)
+        nn.init.normal_(t1, std=0.1)
+        nn.init.normal_(t2, std=0.1)
+        return w1d, w2d, w1u, w2u, t1, t2
+    else:
+        w1d = torch.empty(rank, in_dim)
+        w1u = torch.empty(rank, out_dim)
+        w2d = torch.empty(rank, in_dim)
+        w2u = torch.empty(rank, out_dim)
+        nn.init.normal_(w1d, std=1)
+        nn.init.constant_(w1u, 0)
+        nn.init.normal_(w2d, std=1)
+        nn.init.normal_(w2u, std=0.1)
+        return w1d, w2d, w1u, w2u
+
+
 def loha_diff_weight(w1d, w1u, w2d, w2u, t1=None, t2=None, gamma=1.0):
     """### loha_diff_weight
 
     Get ΔW = BA, where BA is low rank decomposition
 
     Args:
         w1d, w2d (torch.Tensor): weight of down proj linear/conv layer
         w1u, w2u (torch.Tensor): weight of up proj linear/conv layer
+        t1, t2 (torch.Tensor, optional): middle weight of tucker decomposition
         gamma (float, optional): scale factor, normally alpha/rank here
 
     Returns:
         torch.Tensor: ΔW
     """
     if t1 is not None and t2 is not None:
-        assert w1d.size(0) == t1.size(1)
-        assert w1u.size(0) == t1.size(0)
-        assert w2d.size(0) == t2.size(1)
-        assert w2u.size(0) == t2.size(0)
         R, I = w1d.shape
         R, O = w1u.shape
         R, R, *k = t1.shape
         result = make_weight_tucker(t1, w1d, w1u, t2, w2d, w2u, gamma)
     else:
-        assert w1d.size(0) == w1u.size(1)
-        assert w2d.size(0) == w2u.size(1)
         R, I, *k = w1d.shape
         O, R, *_ = w1u.shape
         w1d = w1d.reshape(w1d.size(0), -1)
         w1u = w1u.reshape(-1, w1u.size(1))
         w2d = w2d.reshape(w2d.size(0), -1)
         w2u = w1u.reshape(-1, w2u.size(1))
         result = make_weight(w1d, w1u, w2d, w2u, gamma)
 
     result = result.reshape(O, I, *k)
     return result
 
 
-FUNC_LIST = [None, None, F.linear, F.conv1d, F.conv2d, F.conv3d]
-
-
 def loha_bypass_forward_diff(
     x, w1d, w1u, w2d, w2u, t1=None, t2=None, gamma=1.0, extra_args={}
 ):
     """### loha_bypass_forward_diff
 
     Args:
         x (torch.Tensor): input tensor
         w1d, w2d (torch.Tensor): weight of up proj linear/conv layer
         w1u, w2u (torch.Tensor): weight of down proj linear/conv layer
         gamma (float, optional): scale factor, normally alpha/rank here
+        extra_args (dict, optional): extra args for forward func, \
+            e.g. padding, stride for Conv1/2/3d
 
     Returns:
         torch.Tensor: output tensor
     """
     diff_w = loha_diff_weight(w1d, w1u, w2d, w2u, t1, t2, gamma)
     return FUNC_LIST[w1d.dim() if t1 is None else t1.dim()](x, diff_w, **extra_args)
 
 
 if __name__ == "__main__":
     w = torch.randn(128, 128, 3, 3, 3)
-    a = torch.randn(16, 128) * 0.01
-    b = torch.randn(16, 128) * 0.01
-    m = torch.randn(16, 16, 3, 3, 3) * 0.01
+    w1d, w2d, w1u, w2u, t1, t2 = loha_weight_gen(
+        w, 4, tucker=True
+    )
+    w1u += 0.01
     extra_args = {"padding": 1}
 
     x = torch.randn(1, 128, 8, 8, 8)
     y = FUNC_LIST[w.dim()](x, w, **extra_args)
-    diff_w = loha_diff_weight(a, b, a, b, m, m, 1)
-    diff_y = loha_bypass_forward_diff(x, a, b, a, b, m, m, 1, extra_args)
+    diff_w = loha_diff_weight(w1d, w2d, w1u, w2u, t1, t2, 1)
+    diff_y = loha_bypass_forward_diff(x, w1d, w2d, w1u, w2u, t1, t2, 1, extra_args)
 
     print(F.mse_loss(y, y + diff_y))
     print(F.mse_loss(w, w + diff_w))
```

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/kohya.py` & `lycoris_lora-3.0.0.dev5/lycoris/kohya.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,14 @@
-# network module for kohya
-# reference:
-# https://github.com/microsoft/LoRA/blob/main/loralib/layers.py
-# https://github.com/cloneofsimo/lora/blob/master/lora_diffusion/lora.py
-# https://github.com/kohya-ss/sd-scripts/blob/main/networks/lora.py
-
 import os
 import re
 from typing import List
 
 import torch
 
-from library.train_util import *
+from .utils import precalculate_safetensors_hashes
 from .wrapper import LycorisNetwork
 from .modules.locon import LoConModule
 from .modules.loha import LohaModule
 from .modules.ia3 import IA3Module
 from .modules.lokr import LokrModule
 from .modules.dylora import DyLoraModule
 from .modules.glora import GLoRAModule
@@ -146,18 +140,14 @@
             weight_decompose=weight_decompose,
             full_matrix=full_matrix,
             bypass_mode=bypass_mode,
             rs_lora=rs_lora,
             unbalanced_factorization=unbalanced_factorization,
         )
 
-    if algo == "dylora":
-        # dylora didn't support scale weight norm yet
-        delattr(type(network), "apply_max_norm_regularization")
-
     return network
 
 
 def create_network_from_weights(
     multiplier,
     file,
     vae,
```

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/logging.py` & `lycoris_lora-3.0.0.dev5/lycoris/logging.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/modules/__init__.py` & `lycoris_lora-3.0.0.dev5/lycoris/modules/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 import torch
 import torch.nn as nn
 
-from .full import FullModule
-from .norms import NormModule
 from .locon import LoConModule
 from .loha import LohaModule
-from .lokr import LokrModule, factorization
+from .lokr import LokrModule
+from .full import FullModule
+from .norms import NormModule
+from .diag_oft import DiagOFTModule
+from .boft import ButterflyOFTModule
+from .glora import GLoRAModule
+from .dylora import DyLoraModule
 from .ia3 import IA3Module
 
+from ..functional.general import factorization
+
 
 @torch.no_grad()
 def make_module(lyco_type, params, lora_name, orig_module):
     module = None
     if lyco_type == "locon":
         up, down, mid, alpha, dora_scale = params
         module = LoConModule(
@@ -47,20 +53,22 @@
         if t1 is not None:
             module.hada_t1.copy_(t1)
             module.hada_t2.copy_(t2)
         if dora_scale is not None:
             module.dora_scale.copy_(dora_scale)
     elif lyco_type == "kron":
         w1, w1a, w1b, w2, w2a, w2b, _, t2, alpha, dora_scale = params
+        full_matrix=False
         if w1a is not None:
             lora_dim = w1a.size(1)
         elif w2a is not None:
             lora_dim = w2a.size(1)
         else:
-            lora_dim = 10000000000000
+            full_matrix = True
+            lora_dim = 1
 
         if w1 is None:
             out_dim = w1a.size(0)
             in_dim = w1b.size(1)
         else:
             out_dim, in_dim = w1.shape
 
@@ -87,14 +95,15 @@
             1,
             lora_dim,
             float(alpha),
             use_tucker=t2 is not None,
             decompose_both=w1 is None and w2 is None,
             factor=factor,
             weight_decompose=dora_scale is not None,
+            full_matrix=full_matrix,
         )
         if w1 is not None:
             module.lokr_w1.copy_(w1)
         else:
             module.lokr_w1_a.copy_(w1a)
             module.lokr_w1_b.copy_(w1b)
         if w2 is not None:
```

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/modules/base.py` & `lycoris_lora-3.0.0.dev5/lycoris/modules/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,15 @@
         raise NotImplementedError
 
     def get_merged_weight(self, multiplier=1.0, shape=None, device=None):
         raise NotImplementedError
 
     @torch.no_grad()
     def apply_max_norm(self, max_norm, device=None):
-        raise NotImplementedError
+        return None, None
 
     def bypass_forward_diff(self, x, scale=1):
         raise NotImplementedError
 
     def bypass_forward(self, x, scale=1):
         raise NotImplementedError
```

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/modules/boft.py` & `lycoris_lora-3.0.0.dev5/lycoris/modules/boft.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/modules/diag_oft.py` & `lycoris_lora-3.0.0.dev5/lycoris/modules/diag_oft.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/modules/full.py` & `lycoris_lora-3.0.0.dev5/lycoris/modules/full.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/modules/glora.py` & `lycoris_lora-3.0.0.dev5/lycoris/modules/glora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/modules/ia3.py` & `lycoris_lora-3.0.0.dev5/lycoris/modules/ia3.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,15 @@
             rank_dropout,
             module_dropout,
             rank_dropout_scale,
             bypass_mode,
         )
         if self.module_type not in self.support_module:
             raise ValueError(f"{self.module_type} is not supported in IA^3 algo.")
-        self.lora_dim = lora_dim
-        self.tucker = False
-        self.rs_lora = rs_lora
 
-        self.shape = org_module.weight.shape
         if self.module_type.startswith("conv"):
             self.isconv = True
             in_dim = org_module.in_channels
             out_dim = org_module.out_channels
             if train_on_input:
                 train_dim = in_dim
             else:
@@ -69,16 +65,14 @@
             else:
                 train_dim = out_dim
 
             self.weight = nn.Parameter(torch.empty(train_dim))
 
         # Need more experiences on init method
         torch.nn.init.constant_(self.weight, 0)
-
-        self.multiplier = multiplier
         self.train_input = train_on_input
         self.register_buffer("on_input", torch.tensor(int(train_on_input)))
 
     def apply_to(self):
         self.org_forward = self.org_module[0].forward
         self.org_module[0].forward = self.forward
```

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/modules/locon.py` & `lycoris_lora-3.0.0.dev5/lycoris/modules/locon.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,20 +150,20 @@
             self.scalar.data.copy_(torch.ones_like(self.scalar))
         else:
             self.register_buffer(
                 "scalar", torch.ones_like(self.scalar), persistent=False
             )
 
     def make_weight(self, device=None):
-        wa = self.lora_up.weight.to(device)
-        wb = self.lora_down.weight.to(device)
+        wa = self.lora_up.weight
+        wb = self.lora_down.weight
         if self.tucker:
-            t = self.lora_mid.weight.to(device)
-            wa = wa.reshape(wa.size(0), -1).transpose(0, 1)
-            wb = wb.reshape(wb.size(0), -1)
+            t = self.lora_mid.weight
+            wa = wa.view(wa.size(0), -1).transpose(0, 1)
+            wb = wb.view(wb.size(0), -1)
             weight = rebuild_tucker(t, wa, wb)
         else:
             weight = wa.view(wa.size(0), -1) @ wb.view(wb.size(0), -1)
 
         weight = weight.view(self.shape)
         if self.training and self.rank_dropout:
             drop = (torch.rand(weight.size(0), device=device) > self.rank_dropout).to(
```

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/modules/loha.py` & `lycoris_lora-3.0.0.dev5/lycoris/modules/loha.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/modules/lokr.py` & `lycoris_lora-3.0.0.dev5/lycoris/modules/lokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/modules/norms.py` & `lycoris_lora-3.0.0.dev5/lycoris/modules/norms.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/utils/__init__.py` & `lycoris_lora-3.0.0.dev5/lycoris/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,48 @@
 import re
+import hashlib
+from io import BytesIO
 from typing import Dict, Tuple, Union
 
 import numpy as np
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-
 import torch.linalg as linalg
 
+import safetensors.torch
+
 from tqdm import tqdm
+from .general import *
+
+
+def load_bytes_in_safetensors(tensors):
+    bytes = safetensors.torch.save(tensors)
+    b = BytesIO(bytes)
+
+    b.seek(0)
+    header = b.read(8)
+    n = int.from_bytes(header, "little")
+
+    offset = n + 8
+    b.seek(offset)
+
+    return b.read()
+
+
+def precalculate_safetensors_hashes(state_dict):
+    # calculate each tensor one by one to reduce memory usage
+    hash_sha256 = hashlib.sha256()
+    for tensor in state_dict.values():
+        single_tensor_sd = {"tensor": tensor}
+        bytes_for_tensor = load_bytes_in_safetensors(single_tensor_sd)
+        hash_sha256.update(bytes_for_tensor)
+
+    return f"0x{hash_sha256.hexdigest()}"
 
 
 def str_bool(val):
     return str(val).lower() != "false"
 
 
 def default(val, d):
```

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/utils/logger.py` & `lycoris_lora-3.0.0.dev5/lycoris/utils/logger.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev4/lycoris/wrapper.py` & `lycoris_lora-3.0.0.dev5/lycoris/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,19 +464,20 @@
     def merge_to(self, weight=1.0):
         for lora in self.loras:
             lora.merge_to(weight)
 
     def apply_max_norm_regularization(self, max_norm_value, device):
         key_scaled = 0
         norms = []
-        for model in self.loras:
-            if hasattr(model, "apply_max_norm"):
-                scaled, norm = model.apply_max_norm(max_norm_value, device)
-                norms.append(norm)
-                key_scaled += scaled
+        for module in self.loras:
+            scaled, norm = module.apply_max_norm(max_norm_value, device)
+            if scaled is None:
+                continue
+            norms.append(norm)
+            key_scaled += scaled
 
         if key_scaled == 0:
             return key_scaled, 0, 0
 
         return key_scaled, sum(norms) / len(norms), max(norms)
 
     def enable_gradient_checkpointing(self):
```

### Comparing `lycoris_lora-3.0.0.dev4/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-3.0.0.dev5/lycoris_lora.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 lycoris/modules/ia3.py
 lycoris/modules/locon.py
 lycoris/modules/loha.py
 lycoris/modules/lokr.py
 lycoris/modules/norms.py
 lycoris/utils/__init__.py
 lycoris/utils/bnb.py
+lycoris/utils/general.py
 lycoris/utils/logger.py
 lycoris/utils/preset.py
 lycoris/utils/xformers_utils.py
 lycoris_lora.egg-info/PKG-INFO
 lycoris_lora.egg-info/SOURCES.txt
 lycoris_lora.egg-info/dependency_links.txt
 lycoris_lora.egg-info/not-zip-safe
```

### Comparing `lycoris_lora-3.0.0.dev4/setup.py` & `lycoris_lora-3.0.0.dev5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="lycoris_lora",
     packages=find_packages(),
-    version="3.0.0.dev4",
+    version="3.0.0.dev5",
     url="https://github.com/KohakuBlueleaf/LyCORIS",
     description="Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion",
     author="Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao",
     author_email="apolloyeh0123@gmail.com",
     zip_safe=False,
-    install_requires=[
-        "torch",
-        "einops",
-        "toml",
-    ],
+    install_requires=["torch", "einops", "toml", "tqdm"],
     python_requires=">=3.10",
 )
```

