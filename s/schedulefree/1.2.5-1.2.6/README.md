# Comparing `tmp/schedulefree-1.2.5.tar.gz` & `tmp/schedulefree-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schedulefree-1.2.5.tar", last modified: Mon Apr 22 19:59:49 2024, max compression
+gzip compressed data, was "schedulefree-1.2.6.tar", last modified: Thu May 30 14:50:22 2024, max compression
```

## Comparing `schedulefree-1.2.5.tar` & `schedulefree-1.2.6.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2024-04-22 19:59:49.450132 schedulefree-1.2.5/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)    11356 2024-04-01 19:27:30.000000 schedulefree-1.2.5/LICENSE
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     7043 2024-04-22 19:59:49.451430 schedulefree-1.2.5/PKG-INFO
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6585 2024-04-22 19:53:22.000000 schedulefree-1.2.5/README.md
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      303 2024-04-01 19:31:49.000000 schedulefree-1.2.5/pyproject.toml
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2024-04-22 19:59:49.431153 schedulefree-1.2.5/schedulefree/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      420 2024-04-05 14:54:15.000000 schedulefree-1.2.5/schedulefree/__init__.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     7534 2024-04-22 19:58:50.000000 schedulefree-1.2.5/schedulefree/adamw_schedulefree.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6964 2024-04-22 19:58:50.000000 schedulefree-1.2.5/schedulefree/adamw_schedulefree_closure.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6411 2024-04-22 19:58:50.000000 schedulefree-1.2.5/schedulefree/sgd_schedulefree.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5994 2024-04-22 19:58:50.000000 schedulefree-1.2.5/schedulefree/sgd_schedulefree_closure.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5600 2024-04-22 19:58:50.000000 schedulefree-1.2.5/schedulefree/test_schedulefree.py
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2024-04-22 19:59:49.446770 schedulefree-1.2.5/schedulefree.egg-info/
--rw-r--r--   0 adefazio (1185200101) adefazio (1185200101)     7043 2024-04-22 19:59:49.000000 schedulefree-1.2.5/schedulefree.egg-info/PKG-INFO
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      406 2024-04-22 19:59:49.000000 schedulefree-1.2.5/schedulefree.egg-info/SOURCES.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)        1 2024-04-22 19:59:49.000000 schedulefree-1.2.5/schedulefree.egg-info/dependency_links.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       13 2024-04-22 19:59:49.000000 schedulefree-1.2.5/schedulefree.egg-info/top_level.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       79 2024-04-22 19:59:49.454855 schedulefree-1.2.5/setup.cfg
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      891 2024-04-22 19:59:19.000000 schedulefree-1.2.5/setup.py
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2024-05-30 14:50:22.215736 schedulefree-1.2.6/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)    11356 2024-04-01 19:27:30.000000 schedulefree-1.2.6/LICENSE
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     7602 2024-05-30 14:50:22.217119 schedulefree-1.2.6/PKG-INFO
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     7144 2024-05-28 14:26:57.000000 schedulefree-1.2.6/README.md
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      303 2024-04-01 19:31:49.000000 schedulefree-1.2.6/pyproject.toml
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2024-05-30 14:50:22.199146 schedulefree-1.2.6/schedulefree/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      489 2024-05-28 14:28:16.000000 schedulefree-1.2.6/schedulefree/__init__.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     7676 2024-05-30 14:47:37.000000 schedulefree-1.2.6/schedulefree/adamw_schedulefree.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     7028 2024-05-30 14:47:37.000000 schedulefree-1.2.6/schedulefree/adamw_schedulefree_closure.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6559 2024-05-28 14:51:53.000000 schedulefree-1.2.6/schedulefree/adamw_schedulefree_reference.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     8870 2024-05-28 14:22:34.000000 schedulefree-1.2.6/schedulefree/adamw_schedulefree_reference_check.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6553 2024-05-30 14:47:37.000000 schedulefree-1.2.6/schedulefree/sgd_schedulefree.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6058 2024-05-30 14:47:37.000000 schedulefree-1.2.6/schedulefree/sgd_schedulefree_closure.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6405 2024-05-28 14:57:07.000000 schedulefree-1.2.6/schedulefree/test_schedulefree.py
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2024-05-30 14:50:22.212710 schedulefree-1.2.6/schedulefree.egg-info/
+-rw-r--r--   0 adefazio (1185200101) adefazio (1185200101)     7602 2024-05-30 14:50:22.000000 schedulefree-1.2.6/schedulefree.egg-info/PKG-INFO
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      502 2024-05-30 14:50:22.000000 schedulefree-1.2.6/schedulefree.egg-info/SOURCES.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)        1 2024-05-30 14:50:22.000000 schedulefree-1.2.6/schedulefree.egg-info/dependency_links.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       13 2024-05-30 14:50:22.000000 schedulefree-1.2.6/schedulefree.egg-info/top_level.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       79 2024-05-30 14:50:22.220198 schedulefree-1.2.6/setup.cfg
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      891 2024-05-30 14:47:37.000000 schedulefree-1.2.6/setup.py
```

### Comparing `schedulefree-1.2.5/LICENSE` & `schedulefree-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `schedulefree-1.2.5/PKG-INFO` & `schedulefree-1.2.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,55 @@
-Metadata-Version: 2.1
-Name: schedulefree
-Version: 1.2.5
-Summary: Schedule Free Learning in PyTorch
-Home-page: https://github.com/facebookresearch/schedule_free
-Author: Aaron Defazio
-Author-email: adefazio@meta.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Schedule-Free Learning - A New Way to Train
+# Schedule-Free Learning
 Schedule-Free Optimizers in PyTorch.
 
-Authors: Aaron Defazio, Xingyu Yang, Konstantin Mishchenko, Ashok Cutkosky, Harsh Mehta, Ahmed Khaled
+Preprint: [The Road Less Scheduled](https://arxiv.org/abs/2405.15682)
+
+Authors: Aaron Defazio, Xingyu (Alice) Yang, Harsh Mehta, Konstantin Mishchenko, Ahmed Khaled, Ashok Cutkosky
 
 **TLDR** Faster training without schedules - no need to specify the stopping time/steps in advance!
 
 ``` pip install schedulefree ```
 
 Primary implementations are `SGDScheduleFree` and `AdamWScheduleFree`.
 
 ## Approach
-Schedule-Free learning replaces the momentum of an underlying optimizer with a combination of interpolation and averaging. In the case of gradient descent, the Schedule-free update is:
+Schedule-Free learning replaces the momentum of an underlying optimizer with a combination of interpolation and averaging. In the case of gradient descent, the Schedule-Free update is:
 
 $$
 \begin{align*}
 y_{t} & = (1-\beta)z_{t} + \beta x_{t},\\
 z_{t+1} & =z_{t}-\gamma\nabla f(y_{t}),\\
-x_{t+1} & =\left(1-\frac{1}{t}\right)x_{t}+\frac{1}{t}z_{t+1},
+x_{t+1} & =\left(1-\frac{1}{t+1}\right)x_{t}+\frac{1}{t+1}z_{t+1},
 \end{align*}
 $$
 
 Here $x$ is the sequence that evaluations of test/val loss should occur at, which differs from the primary iterates $z$ and the gradient evaluation locations $y$. The updates to $z$ correspond to the underlying optimizer, in this case a simple gradient step.
 
-As the name suggests, Schedule-free learning does not require a decreasing learning rate schedule, yet typically out-performs, or at worst matches, SOTA schedules such as cosine-decay and linear decay. Only two sequences need to be stored at a time (the third can be computed from the other two on the fly) so this method has the same memory requirements as the base optimizer (parameter buffer + momentum).
+As the name suggests, Schedule-Free learning does not require a decreasing learning rate schedule, yet typically out-performs, or at worst matches, SOTA schedules such as cosine-decay and linear decay. Only two sequences need to be stored at a time (the third can be computed from the other two on the fly) so this method has the same memory requirements as the base optimizer (parameter buffer + momentum).
 
 We provide both AdamW and SGD versions in this repo.
 
 ## How to Use
-Since our optimizer uses two different points for gradient calls and test/val loss calculations, it's necessary to switch the param buffer between the two during training. This is done by calling `optimizer.train()` at the same place you call `model.train()` and `optimizer.eval()` at the same place you call `model.eval()`.
+Since our optimizer uses two different points for gradient calls and test/val loss calculations, it's necessary to switch the param buffer between the two during training. This is done by calling `optimizer.train()` at the same place you call `model.train()` and `optimizer.eval()` at the same place you call `model.eval()`. The optimizer should also be placed in eval mode when storing checkpoints.
 
 If your code supports PyTorch Optimizer step closures, you can use the closure forms of the optimizers, which do not require the `.train()` and `.eval()` calls.
 
+## Paper
+If you use Schedule-Free training in your work, please cite our [preprint](https://arxiv.org/abs/2405.15682) as:
+```
+@misc{defazio2024road,
+      title={The Road Less Scheduled}, 
+      author={Aaron Defazio and Xingyu Yang and Harsh Mehta and Konstantin Mishchenko and Ahmed Khaled and Ashok Cutkosky},
+      year={2024},
+      eprint={2405.15682},
+      archivePrefix={arXiv},
+      primaryClass={cs.LG}
+}
+```
+
 ### Examples
 Examples of using the `schedulefree` package can be found in the `examples` folder. These include:
 - [Image classification (MNIST) using Convnets](./examples/mnist/)*
 - More examples to be added
 
 *Example is modified from [Pytorch Examples Repo](https://github.com/pytorch/examples).
```

### Comparing `schedulefree-1.2.5/README.md` & `schedulefree-1.2.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,69 @@
-# Schedule-Free Learning - A New Way to Train
+Metadata-Version: 2.1
+Name: schedulefree
+Version: 1.2.6
+Summary: Schedule Free Learning in PyTorch
+Home-page: https://github.com/facebookresearch/schedule_free
+Author: Aaron Defazio
+Author-email: adefazio@meta.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Schedule-Free Learning
 Schedule-Free Optimizers in PyTorch.
 
-Authors: Aaron Defazio, Xingyu Yang, Konstantin Mishchenko, Ashok Cutkosky, Harsh Mehta, Ahmed Khaled
+Preprint: [The Road Less Scheduled](https://arxiv.org/abs/2405.15682)
+
+Authors: Aaron Defazio, Xingyu (Alice) Yang, Harsh Mehta, Konstantin Mishchenko, Ahmed Khaled, Ashok Cutkosky
 
 **TLDR** Faster training without schedules - no need to specify the stopping time/steps in advance!
 
 ``` pip install schedulefree ```
 
 Primary implementations are `SGDScheduleFree` and `AdamWScheduleFree`.
 
 ## Approach
-Schedule-Free learning replaces the momentum of an underlying optimizer with a combination of interpolation and averaging. In the case of gradient descent, the Schedule-free update is:
+Schedule-Free learning replaces the momentum of an underlying optimizer with a combination of interpolation and averaging. In the case of gradient descent, the Schedule-Free update is:
 
 $$
 \begin{align*}
 y_{t} & = (1-\beta)z_{t} + \beta x_{t},\\
 z_{t+1} & =z_{t}-\gamma\nabla f(y_{t}),\\
-x_{t+1} & =\left(1-\frac{1}{t}\right)x_{t}+\frac{1}{t}z_{t+1},
+x_{t+1} & =\left(1-\frac{1}{t+1}\right)x_{t}+\frac{1}{t+1}z_{t+1},
 \end{align*}
 $$
 
 Here $x$ is the sequence that evaluations of test/val loss should occur at, which differs from the primary iterates $z$ and the gradient evaluation locations $y$. The updates to $z$ correspond to the underlying optimizer, in this case a simple gradient step.
 
-As the name suggests, Schedule-free learning does not require a decreasing learning rate schedule, yet typically out-performs, or at worst matches, SOTA schedules such as cosine-decay and linear decay. Only two sequences need to be stored at a time (the third can be computed from the other two on the fly) so this method has the same memory requirements as the base optimizer (parameter buffer + momentum).
+As the name suggests, Schedule-Free learning does not require a decreasing learning rate schedule, yet typically out-performs, or at worst matches, SOTA schedules such as cosine-decay and linear decay. Only two sequences need to be stored at a time (the third can be computed from the other two on the fly) so this method has the same memory requirements as the base optimizer (parameter buffer + momentum).
 
 We provide both AdamW and SGD versions in this repo.
 
 ## How to Use
-Since our optimizer uses two different points for gradient calls and test/val loss calculations, it's necessary to switch the param buffer between the two during training. This is done by calling `optimizer.train()` at the same place you call `model.train()` and `optimizer.eval()` at the same place you call `model.eval()`.
+Since our optimizer uses two different points for gradient calls and test/val loss calculations, it's necessary to switch the param buffer between the two during training. This is done by calling `optimizer.train()` at the same place you call `model.train()` and `optimizer.eval()` at the same place you call `model.eval()`. The optimizer should also be placed in eval mode when storing checkpoints.
 
 If your code supports PyTorch Optimizer step closures, you can use the closure forms of the optimizers, which do not require the `.train()` and `.eval()` calls.
 
+## Paper
+If you use Schedule-Free training in your work, please cite our [preprint](https://arxiv.org/abs/2405.15682) as:
+```
+@misc{defazio2024road,
+      title={The Road Less Scheduled}, 
+      author={Aaron Defazio and Xingyu Yang and Harsh Mehta and Konstantin Mishchenko and Ahmed Khaled and Ashok Cutkosky},
+      year={2024},
+      eprint={2405.15682},
+      archivePrefix={arXiv},
+      primaryClass={cs.LG}
+}
+```
+
 ### Examples
 Examples of using the `schedulefree` package can be found in the `examples` folder. These include:
 - [Image classification (MNIST) using Convnets](./examples/mnist/)*
 - More examples to be added
 
 *Example is modified from [Pytorch Examples Repo](https://github.com/pytorch/examples).
```

### Comparing `schedulefree-1.2.5/schedulefree/adamw_schedulefree.py` & `schedulefree-1.2.6/schedulefree/adamw_schedulefree.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     r"""
     Schedule-Free AdamW
     As the name suggests, no scheduler is needed with this optimizer. 
     To add warmup, rather than using a learning rate schedule you can just
     set the warmup_steps parameter.
     
     This optimizer requires that .train() and .eval() be called before the
-    beginning of training and evaluation respectively.
+    beginning of training and evaluation respectively. The optimizer should
+    also be placed in eval mode when saving checkpoints.
     
     Arguments:
         params (iterable): 
             Iterable of parameters to optimize or dicts defining 
             parameter groups.
         lr (float): 
             Learning rate parameter (default 0.0025)
@@ -34,26 +35,26 @@
         r (float): Use polynomial weighting in the average 
             with power r (default 0).
         weight_lr_power (float): During warmup, the weights in the average will
             be equal to lr raised to this power. Set to 0 for no weighting
             (default 2.0).
         foreach (bool): Use a foreach-backed implementation of the optimizer.
             Should be significantly faster, but will have higher peak memory
-            usage (default True).
+            usage (default True if supported in your PyTorch version).
     """
     def __init__(self,
                  params, 
                  lr=0.0025, 
                  betas=(0.9, 0.999), 
                  eps=1e-8,
                  weight_decay=0,
                  warmup_steps=0,
                  r=0.0,
                  weight_lr_power=2.0,
-                 foreach=True
+                 foreach=hasattr(torch, "_foreach_mul_")
                  ):
 
         defaults = dict(lr=lr, 
                         betas=betas, 
                         eps=eps,
                         r=r,
                         k=0,
```

### Comparing `schedulefree-1.2.5/schedulefree/adamw_schedulefree_closure.py` & `schedulefree-1.2.6/schedulefree/adamw_schedulefree_closure.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,25 +33,25 @@
         r (float): Use polynomial weighting in the average 
             with power r (default 0).
         weight_lr_power (float): During warmup, the weights in the average will
             be equal to lr raised to this power. Set to 0 for no weighting
             (default 2.0).
         foreach (bool): Use a foreach-backed implementation of the optimizer.
             Should be significantly faster, but will have higher peak memory
-            usage (default True).
+            usage (default True if supported in your PyTorch version).
     """
     def __init__(self, params,
                  lr=0.0025,
                  betas=(0.9, 0.999),
                  eps=1e-8,
                  weight_decay=0,
                  warmup_steps=0,
                  r=0,
                  weight_lr_power=2.0,
-                 foreach=True
+                 foreach=hasattr(torch, "_foreach_mul_")
                  ):
         defaults = dict(lr=lr,
                         betas=betas,
                         eps=eps,
                         r=r,
                         k=0,
                         weight_sum=0.0,
```

### Comparing `schedulefree-1.2.5/schedulefree/sgd_schedulefree.py` & `schedulefree-1.2.6/schedulefree/sgd_schedulefree.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     r"""
     Schedule-Free SGD
     As the name suggests, no scheduler is needed with this optimizer. 
     To add warmup, rather than using a learning rate schedule you can just
     set the warmup_steps parameter.
 
     This optimizer requires that .train() and .eval() be called before the
-    beginning of training and evaluation respectively.
+    beginning of training and evaluation respectively. The optimizer should
+    also be placed in eval mode when saving checkpoints.
     
     Arguments:
         params (iterable): 
             Iterable of parameters to optimize or dicts defining 
             parameter groups.
         lr (float): 
             Learning rate parameter (default 1.0)
@@ -30,25 +31,25 @@
         r (float): Use polynomial weighting in the average 
             with power r (default 0).
         weight_lr_power (float): During warmup, the weights in the average will
             be equal to lr raised to this power. Set to 0 for no weighting
             (default 2.0).
         foreach (bool): Use a foreach-backed implementation of the optimizer.
             Should be significantly faster, but will have higher peak memory
-            usage (default True).
+            usage (default True if supported in your PyTorch version).
     """
     def __init__(self,
                  params, 
                  lr=1.0, 
                  momentum=0.9, 
                  weight_decay=0,
                  warmup_steps=0,
                  r=0.0,
                  weight_lr_power=2,
-                 foreach=True,
+                 foreach=hasattr(torch, "_foreach_mul_"),
                  ):
         if lr < 0.0:
             raise ValueError("Invalid learning rate: {}".format(lr))
         if weight_decay < 0.0:
             raise ValueError("Invalid weight_decay value: {}".format(weight_decay))
         if momentum <= 0 or momentum >= 1:
             raise ValueError("Momentum must be between 0 and 1 exclusive: {}".format(momentum))
```

### Comparing `schedulefree-1.2.5/schedulefree/sgd_schedulefree_closure.py` & `schedulefree-1.2.6/schedulefree/sgd_schedulefree_closure.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,25 +30,25 @@
         r (float): Use polynomial weighting in the average 
             with power r (default 0).
         weight_lr_power (float): During warmup, the weights in the average will
             be equal to lr raised to this power. Set to 0 for no weighting
             (default 2.0).
         foreach (bool): Use a foreach-backed implementation of the optimizer.
             Should be significantly faster, but will have higher peak memory
-            usage (default True).
+            usage (default True if supported in your PyTorch version).
     """
     def __init__(self,
                  params,
                  lr=1.0,
                  weight_decay=0,
                  momentum=0.9,
                  warmup_steps=0,
                  r=0.0,
                  weight_lr_power=2.0,
-                 foreach=True
+                 foreach=hasattr(torch, "_foreach_mul_")
                  ):
         if lr < 0.0:
             raise ValueError("Invalid learning rate: {}".format(lr))
         if weight_decay < 0.0:
             raise ValueError("Invalid weight_decay value: {}".format(weight_decay))
         if momentum <= 0 or momentum >= 1:
             raise ValueError("Momentum must be between 0 and 1 exclusive: {}".format(momentum))
```

### Comparing `schedulefree-1.2.5/schedulefree/test_schedulefree.py` & `schedulefree-1.2.6/schedulefree/test_schedulefree.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 # 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 import torch
-from schedulefree import SGDScheduleFree, SGDScheduleFreeClosure, AdamWScheduleFree, AdamWScheduleFreeClosure
+from schedulefree import SGDScheduleFree, SGDScheduleFreeClosure, AdamWScheduleFree, AdamWScheduleFreeClosure, AdamWScheduleFreeReference
 
 def test_schedulefree_sgd():
     decay = 0.5
     warmup = 5
     weight_closure = torch.randn(3, 2).cuda().requires_grad_()
     weight = torch.clone(weight_closure.data).requires_grad_()
     optimizer_closure = SGDScheduleFreeClosure([weight_closure], lr=0.3, warmup_steps=warmup, weight_decay=decay)
@@ -41,66 +41,73 @@
                 assert torch.allclose(z, z_closure)
  
 def test_schedulefree_adam():
     decay = 0.5
     warmup = 5
     weight_closure = torch.randn(3, 2).cuda().requires_grad_()
     weight = torch.clone(weight_closure.data).requires_grad_()
+    weight_reference = torch.clone(weight_closure.data).requires_grad_()
     optimizer_closure = AdamWScheduleFreeClosure([weight_closure], lr=0.3, warmup_steps=warmup, weight_decay=decay)
     optimizer = AdamWScheduleFree([weight], lr=0.3, warmup_steps=warmup, weight_decay=decay)
+    optimizer_reference = AdamWScheduleFreeReference([weight_reference], lr=0.3, warmup_steps=warmup, weight_decay=decay)
 
     for step_idx in range(50):
         print(step_idx)
         optimizer.train()
+        optimizer_reference.train()
         grad = torch.rand_like(weight)
 
         weight.grad = torch.clone(grad)
+        weight_reference.grad = torch.clone(grad)
 
         def closure():
             weight_closure.grad = torch.clone(grad)
 
         optimizer.step()
         optimizer_closure.step(closure=closure)
+        optimizer_reference.step()
 
         optimizer.eval()
+        optimizer_reference.eval()
 
-        for group_closure, group in zip(optimizer_closure.param_groups, optimizer.param_groups):
-            for p_closure, p in zip(group_closure['params'], group['params']):
+        for group_closure, group, group_reference in zip(optimizer_closure.param_groups, optimizer.param_groups, optimizer_reference.param_groups):
+            for p_closure, p, p_reference in zip(group_closure['params'], group['params'], group_reference['params']):
                 state_closure = optimizer_closure.state[p_closure]
                 state = optimizer.state[p]
+                state_reference = optimizer_reference.state[p_reference]
+
                 z_closure = state_closure['z']
                 z = state['z']
-
-                #print(f"p: {p}")
-                #print(f"p: {p_closure}")
-
-
-                #print(f"z: {z}")
-                #print(f"z: {z_closure}")
+                z_reference = state_reference['z']
 
                 assert torch.allclose(p, p_closure)
+                assert torch.allclose(p, p_reference)
                 assert torch.allclose(z, z_closure)
+                assert torch.allclose(z, z_reference)
  
         optimizer.train()
+        optimizer_reference.train()
 
-        for group_closure, group in zip(optimizer_closure.param_groups, optimizer.param_groups):
-            for p_closure, p in zip(group_closure['params'], group['params']):
+        for group_closure, group, group_reference in zip(optimizer_closure.param_groups, optimizer.param_groups, optimizer_reference.param_groups):
+            for p_closure, p, p_reference in zip(group_closure['params'], group['params'], group_reference['params']):
                 state_closure = optimizer_closure.state[p_closure]
                 state = optimizer.state[p]
+                state_reference = optimizer_reference.state[p_reference]
 
                 z_closure = state_closure['z']
+                z = state['z']
+                z_reference = state_reference['z']
 
                 # Extrapolate p.data to equal y
                 y = p.data
                 y_closure = p_closure.lerp(end=z_closure, weight=1-0.9)
 
-                #print(f"y: {y}")
-                #print(f"y closure: {y_closure}")
 
                 assert torch.allclose(y, y_closure)
+                assert torch.allclose(y, p_reference.data)
 
 def test_foreach():
     decay = 0.5
     warmup = 5
     weight_foreach = torch.randn(3, 2).cuda().requires_grad_()
     weight_foreach2 = torch.randn(1, 1).cuda().requires_grad_()
     weight_foreach_nograd = torch.randn(1, 2).cuda().requires_grad_()
```

### Comparing `schedulefree-1.2.5/schedulefree.egg-info/PKG-INFO` & `schedulefree-1.2.6/schedulefree.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,69 @@
 Metadata-Version: 2.1
 Name: schedulefree
-Version: 1.2.5
+Version: 1.2.6
 Summary: Schedule Free Learning in PyTorch
 Home-page: https://github.com/facebookresearch/schedule_free
 Author: Aaron Defazio
 Author-email: adefazio@meta.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Schedule-Free Learning - A New Way to Train
+# Schedule-Free Learning
 Schedule-Free Optimizers in PyTorch.
 
-Authors: Aaron Defazio, Xingyu Yang, Konstantin Mishchenko, Ashok Cutkosky, Harsh Mehta, Ahmed Khaled
+Preprint: [The Road Less Scheduled](https://arxiv.org/abs/2405.15682)
+
+Authors: Aaron Defazio, Xingyu (Alice) Yang, Harsh Mehta, Konstantin Mishchenko, Ahmed Khaled, Ashok Cutkosky
 
 **TLDR** Faster training without schedules - no need to specify the stopping time/steps in advance!
 
 ``` pip install schedulefree ```
 
 Primary implementations are `SGDScheduleFree` and `AdamWScheduleFree`.
 
 ## Approach
-Schedule-Free learning replaces the momentum of an underlying optimizer with a combination of interpolation and averaging. In the case of gradient descent, the Schedule-free update is:
+Schedule-Free learning replaces the momentum of an underlying optimizer with a combination of interpolation and averaging. In the case of gradient descent, the Schedule-Free update is:
 
 $$
 \begin{align*}
 y_{t} & = (1-\beta)z_{t} + \beta x_{t},\\
 z_{t+1} & =z_{t}-\gamma\nabla f(y_{t}),\\
-x_{t+1} & =\left(1-\frac{1}{t}\right)x_{t}+\frac{1}{t}z_{t+1},
+x_{t+1} & =\left(1-\frac{1}{t+1}\right)x_{t}+\frac{1}{t+1}z_{t+1},
 \end{align*}
 $$
 
 Here $x$ is the sequence that evaluations of test/val loss should occur at, which differs from the primary iterates $z$ and the gradient evaluation locations $y$. The updates to $z$ correspond to the underlying optimizer, in this case a simple gradient step.
 
-As the name suggests, Schedule-free learning does not require a decreasing learning rate schedule, yet typically out-performs, or at worst matches, SOTA schedules such as cosine-decay and linear decay. Only two sequences need to be stored at a time (the third can be computed from the other two on the fly) so this method has the same memory requirements as the base optimizer (parameter buffer + momentum).
+As the name suggests, Schedule-Free learning does not require a decreasing learning rate schedule, yet typically out-performs, or at worst matches, SOTA schedules such as cosine-decay and linear decay. Only two sequences need to be stored at a time (the third can be computed from the other two on the fly) so this method has the same memory requirements as the base optimizer (parameter buffer + momentum).
 
 We provide both AdamW and SGD versions in this repo.
 
 ## How to Use
-Since our optimizer uses two different points for gradient calls and test/val loss calculations, it's necessary to switch the param buffer between the two during training. This is done by calling `optimizer.train()` at the same place you call `model.train()` and `optimizer.eval()` at the same place you call `model.eval()`.
+Since our optimizer uses two different points for gradient calls and test/val loss calculations, it's necessary to switch the param buffer between the two during training. This is done by calling `optimizer.train()` at the same place you call `model.train()` and `optimizer.eval()` at the same place you call `model.eval()`. The optimizer should also be placed in eval mode when storing checkpoints.
 
 If your code supports PyTorch Optimizer step closures, you can use the closure forms of the optimizers, which do not require the `.train()` and `.eval()` calls.
 
+## Paper
+If you use Schedule-Free training in your work, please cite our [preprint](https://arxiv.org/abs/2405.15682) as:
+```
+@misc{defazio2024road,
+      title={The Road Less Scheduled}, 
+      author={Aaron Defazio and Xingyu Yang and Harsh Mehta and Konstantin Mishchenko and Ahmed Khaled and Ashok Cutkosky},
+      year={2024},
+      eprint={2405.15682},
+      archivePrefix={arXiv},
+      primaryClass={cs.LG}
+}
+```
+
 ### Examples
 Examples of using the `schedulefree` package can be found in the `examples` folder. These include:
 - [Image classification (MNIST) using Convnets](./examples/mnist/)*
 - More examples to be added
 
 *Example is modified from [Pytorch Examples Repo](https://github.com/pytorch/examples).
```

### Comparing `schedulefree-1.2.5/setup.py` & `schedulefree-1.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="schedulefree",
-    version="1.2.5",
+    version="1.2.6",
     author="Aaron Defazio",
     author_email="adefazio@meta.com",
     description="Schedule Free Learning in PyTorch",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/facebookresearch/schedule_free",
     packages=setuptools.find_packages(),
```

