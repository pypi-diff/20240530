# Comparing `tmp/sae_lens-3.1.0.tar.gz` & `tmp/sae_lens-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-3.1.0.tar", max compression
+gzip compressed data, was "sae_lens-3.1.1.tar", max compression
```

## Comparing `sae_lens-3.1.0.tar` & `sae_lens-3.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1069 2024-05-29 15:03:40.110520 sae_lens-3.1.0/LICENSE
--rw-r--r--   0        0        0     3381 2024-05-29 15:03:40.110520 sae_lens-3.1.0/README.md
--rw-r--r--   0        0        0     2068 2024-05-29 15:03:41.446527 sae_lens-3.1.0/pyproject.toml
--rw-r--r--   0        0        0      898 2024-05-29 15:03:41.446527 sae_lens-3.1.0/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0     3320 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0    12561 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/analysis/hooked_sae_transformer.py
--rw-r--r--   0        0        0    17062 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    20406 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     4052 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/batching.py
--rw-r--r--   0        0        0     6047 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/cache_activations_runner.py
--rw-r--r--   0        0        0    24486 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/config.py
--rw-r--r--   0        0        0    16161 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/dashboard_runner.py
--rw-r--r--   0        0        0     7966 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/evals.py
--rw-r--r--   0        0        0     1320 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/load_model.py
--rw-r--r--   0        0        0     5383 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/pretokenize_runner.py
--rw-r--r--   0        0        0     4833 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/pretrained_saes.yaml
--rw-r--r--   0        0        0    15822 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/sae.py
--rw-r--r--   0        0        0     6972 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/sae_training_runner.py
--rw-r--r--   0        0        0        0 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/toolkit/__init__.py
--rw-r--r--   0        0        0     6506 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/toolkit/pretrained_sae_loaders.py
--rw-r--r--   0        0        0     4752 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0     1143 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/toolkit/pretrained_saes_directory.py
--rw-r--r--   0        0        0     1783 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/toy_model_runner.py
--rw-r--r--   0        0        0        0 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/training/__init__.py
--rw-r--r--   0        0        0    21723 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     3779 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     5585 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/training/optim.py
--rw-r--r--   0        0        0    14674 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/training/sae_trainer.py
--rw-r--r--   0        0        0    18456 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0     4850 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/training/train_toy_sae.py
--rw-r--r--   0        0        0    15495 2024-05-29 15:03:40.122521 sae_lens-3.1.0/sae_lens/training/training_sae.py
--rw-r--r--   0        0        0     5024 1970-01-01 00:00:00.000000 sae_lens-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-29 20:19:45.909911 sae_lens-3.1.1/LICENSE
+-rw-r--r--   0        0        0     3381 2024-05-29 20:19:45.909911 sae_lens-3.1.1/README.md
+-rw-r--r--   0        0        0     2068 2024-05-29 20:19:47.329921 sae_lens-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0      898 2024-05-29 20:19:47.329921 sae_lens-3.1.1/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:19:45.917911 sae_lens-3.1.1/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0     3320 2024-05-29 20:19:45.917911 sae_lens-3.1.1/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0    12561 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/analysis/hooked_sae_transformer.py
+-rw-r--r--   0        0        0    17062 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    20406 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     4052 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/batching.py
+-rw-r--r--   0        0        0     6047 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/cache_activations_runner.py
+-rw-r--r--   0        0        0    24486 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/config.py
+-rw-r--r--   0        0        0    16161 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/dashboard_runner.py
+-rw-r--r--   0        0        0     7966 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/evals.py
+-rw-r--r--   0        0        0     1320 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/load_model.py
+-rw-r--r--   0        0        0     5383 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/pretokenize_runner.py
+-rw-r--r--   0        0        0     4833 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/pretrained_saes.yaml
+-rw-r--r--   0        0        0    14128 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/sae.py
+-rw-r--r--   0        0        0     6972 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/sae_training_runner.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/toolkit/__init__.py
+-rw-r--r--   0        0        0     8087 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/toolkit/pretrained_sae_loaders.py
+-rw-r--r--   0        0        0     4752 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0     1143 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/toolkit/pretrained_saes_directory.py
+-rw-r--r--   0        0        0     1783 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/toy_model_runner.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0    21723 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     3779 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     5585 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/training/optim.py
+-rw-r--r--   0        0        0    14674 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/training/sae_trainer.py
+-rw-r--r--   0        0        0    18456 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0     4850 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/training/train_toy_sae.py
+-rw-r--r--   0        0        0    15495 2024-05-29 20:19:45.921911 sae_lens-3.1.1/sae_lens/training/training_sae.py
+-rw-r--r--   0        0        0     5024 1970-01-01 00:00:00.000000 sae_lens-3.1.1/PKG-INFO
```

### Comparing `sae_lens-3.1.0/LICENSE` & `sae_lens-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/README.md` & `sae_lens-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/pyproject.toml` & `sae_lens-3.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sae-lens"
-version = "3.1.0"
+version = "3.1.1"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 include = ["pretrained_saes.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `sae_lens-3.1.0/sae_lens/__init__.py` & `sae_lens-3.1.1/sae_lens/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.1.0"
+__version__ = "3.1.1"
 
 
 from .analysis.hooked_sae_transformer import HookedSAETransformer
 from .cache_activations_runner import CacheActivationsRunner
 from .config import (
     CacheActivationsRunnerConfig,
     LanguageModelSAERunnerConfig,
```

### Comparing `sae_lens-3.1.0/sae_lens/analysis/feature_statistics.py` & `sae_lens-3.1.1/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/analysis/hooked_sae_transformer.py` & `sae_lens-3.1.1/sae_lens/analysis/hooked_sae_transformer.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/analysis/neuronpedia_integration.py` & `sae_lens-3.1.1/sae_lens/analysis/neuronpedia_integration.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-3.1.1/sae_lens/analysis/neuronpedia_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/analysis/tsea.py` & `sae_lens-3.1.1/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/batching.py` & `sae_lens-3.1.1/sae_lens/batching.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/cache_activations_runner.py` & `sae_lens-3.1.1/sae_lens/cache_activations_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/config.py` & `sae_lens-3.1.1/sae_lens/config.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/dashboard_runner.py` & `sae_lens-3.1.1/sae_lens/dashboard_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/evals.py` & `sae_lens-3.1.1/sae_lens/evals.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/load_model.py` & `sae_lens-3.1.1/sae_lens/load_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/pretokenize_runner.py` & `sae_lens-3.1.1/sae_lens/pretokenize_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/pretrained_saes.yaml` & `sae_lens-3.1.1/sae_lens/pretrained_saes.yaml`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/sae.py` & `sae_lens-3.1.1/sae_lens/sae.py`

 * *Files 6% similar despite different names*

```diff
@@ -341,54 +341,14 @@
         cfg_dict, state_dict, log_sparsities = conversion_loader(
             repo_id=hf_repo_id,
             folder_name=hf_path,
             device=device,
             force_download=False,
         )
 
-        if "prepend_bos" not in cfg_dict:
-            # default to True for backwards compatibility
-            cfg_dict["prepend_bos"] = True
-
-        if "apply_b_dec_to_input" not in cfg_dict:
-            # default to True for backwards compatibility
-            cfg_dict["apply_b_dec_to_input"] = True
-
-        if "finetuning_scaling_factor" not in cfg_dict:
-            # default to False for backwards compatibility
-            cfg_dict["finetuning_scaling_factor"] = False
-
-        if "sae_lens_training_version" not in cfg_dict:
-            cfg_dict["sae_lens_training_version"] = None
-
-        if "activation_fn" not in cfg_dict:
-            cfg_dict["activation_fn_str"] = "relu"
-
-        if "normalize_activations" not in cfg_dict:
-            cfg_dict["normalize_activations"] = False
-
-        if "scaling_factor" in state_dict:
-            # we were adding it anyway for a period of time but are no longer doing so.
-            # so we should delete it if
-            if torch.allclose(
-                state_dict["scaling_factor"],
-                torch.ones_like(state_dict["scaling_factor"]),
-            ):
-                del state_dict["scaling_factor"]
-                cfg_dict["finetuning_scaling_factor"] = False
-            else:
-                assert cfg_dict[
-                    "finetuning_scaling_factor"
-                ], "Scaling factor is present but finetuning_scaling_factor is False."
-                state_dict["finetuning_scaling_factor"] = state_dict["scaling_factor"]
-                del state_dict["scaling_factor"]
-        else:
-            # it's there and it's not all 1's, we should use it.
-            cfg_dict["finetuning_scaling_factor"] = False
-
         sae = cls(SAEConfig.from_dict(cfg_dict))
         sae.load_state_dict(state_dict)
 
         return sae, cfg_dict, log_sparsities
 
     def get_name(self):
         sae_name = f"sae_{self.cfg.model_name}_{self.cfg.hook_name}_{self.cfg.d_sae}"
```

### Comparing `sae_lens-3.1.0/sae_lens/sae_training_runner.py` & `sae_lens-3.1.1/sae_lens/sae_training_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/toolkit/pretrained_saes.py` & `sae_lens-3.1.1/sae_lens/toolkit/pretrained_saes.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/toolkit/pretrained_saes_directory.py` & `sae_lens-3.1.1/sae_lens/toolkit/pretrained_saes_directory.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/toy_model_runner.py` & `sae_lens-3.1.1/sae_lens/toy_model_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/training/activations_store.py` & `sae_lens-3.1.1/sae_lens/training/activations_store.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/training/geometric_median.py` & `sae_lens-3.1.1/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/training/optim.py` & `sae_lens-3.1.1/sae_lens/training/optim.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/training/sae_trainer.py` & `sae_lens-3.1.1/sae_lens/training/sae_trainer.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/training/toy_models.py` & `sae_lens-3.1.1/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/training/train_toy_sae.py` & `sae_lens-3.1.1/sae_lens/training/train_toy_sae.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/sae_lens/training/training_sae.py` & `sae_lens-3.1.1/sae_lens/training/training_sae.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.1.0/PKG-INFO` & `sae_lens-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 3.1.0
+Version: 3.1.1
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

