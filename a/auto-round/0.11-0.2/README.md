# Comparing `tmp/auto_round-0.11.tar.gz` & `tmp/auto_round-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_round-0.11.tar", last modified: Mon Mar 25 11:43:43 2024, max compression
+gzip compressed data, was "dist/auto_round-0.2.tar", last modified: Wed May 29 16:52:36 2024, max compression
```

## Comparing `auto_round-0.11.tar` & `auto_round-0.2.tar`

### file list

```diff
@@ -1,34 +1,39 @@
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-03-25 11:43:43.475982 auto_round-0.11/
--rw-rw-r--   0 test      (1000) test      (1000)    10172 2024-03-08 07:32:51.000000 auto_round-0.11/LICENSE
--rw-rw-r--   0 test      (1000) test      (1000)    14624 2024-03-25 11:43:43.475982 auto_round-0.11/PKG-INFO
--rw-rw-r--   0 test      (1000) test      (1000)    13903 2024-03-25 11:42:57.000000 auto_round-0.11/README.md
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-03-25 11:43:43.475982 auto_round-0.11/auto_round/
--rw-rw-r--   0 test      (1000) test      (1000)      679 2024-03-08 07:32:51.000000 auto_round-0.11/auto_round/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)    56201 2024-03-25 11:42:57.000000 auto_round-0.11/auto_round/autoround.py
--rw-rw-r--   0 test      (1000) test      (1000)     5664 2024-03-08 07:32:51.000000 auto_round-0.11/auto_round/calib_dataset.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-03-25 11:43:43.475982 auto_round-0.11/auto_round/export/
--rw-rw-r--   0 test      (1000) test      (1000)      746 2024-03-08 07:32:51.000000 auto_round-0.11/auto_round/export/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)    10356 2024-03-08 07:32:51.000000 auto_round-0.11/auto_round/export/export_to_autogptq.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-03-25 11:43:43.475982 auto_round-0.11/auto_round/export/export_to_itrex/
--rw-rw-r--   0 test      (1000) test      (1000)      672 2024-03-08 07:32:51.000000 auto_round-0.11/auto_round/export/export_to_itrex/__init__.py
--rw-rw-r--   0 test      (1000) test      (1000)     8838 2024-03-08 07:32:51.000000 auto_round-0.11/auto_round/export/export_to_itrex/config.py
--rw-rw-r--   0 test      (1000) test      (1000)     5912 2024-03-25 11:42:57.000000 auto_round-0.11/auto_round/export/export_to_itrex/export.py
--rw-rw-r--   0 test      (1000) test      (1000)    14884 2024-03-08 07:32:51.000000 auto_round-0.11/auto_round/export/export_to_itrex/model_wrapper.py
--rw-rw-r--   0 test      (1000) test      (1000)     1031 2024-03-08 07:32:51.000000 auto_round-0.11/auto_round/export/register.py
--rw-rw-r--   0 test      (1000) test      (1000)    14977 2024-03-08 07:32:51.000000 auto_round-0.11/auto_round/sign_sgd.py
--rw-rw-r--   0 test      (1000) test      (1000)    22647 2024-03-25 11:42:57.000000 auto_round-0.11/auto_round/utils.py
--rw-rw-r--   0 test      (1000) test      (1000)      731 2024-03-25 11:42:57.000000 auto_round-0.11/auto_round/version.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-03-25 11:43:43.475982 auto_round-0.11/auto_round.egg-info/
--rw-rw-r--   0 test      (1000) test      (1000)    14624 2024-03-25 11:43:43.000000 auto_round-0.11/auto_round.egg-info/PKG-INFO
--rw-rw-r--   0 test      (1000) test      (1000)      744 2024-03-25 11:43:43.000000 auto_round-0.11/auto_round.egg-info/SOURCES.txt
--rw-rw-r--   0 test      (1000) test      (1000)        1 2024-03-25 11:43:43.000000 auto_round-0.11/auto_round.egg-info/dependency_links.txt
--rw-rw-r--   0 test      (1000) test      (1000)       74 2024-03-25 11:43:43.000000 auto_round-0.11/auto_round.egg-info/requires.txt
--rw-rw-r--   0 test      (1000) test      (1000)       11 2024-03-25 11:43:43.000000 auto_round-0.11/auto_round.egg-info/top_level.txt
--rw-rw-r--   0 test      (1000) test      (1000)     2242 2024-03-08 07:32:51.000000 auto_round-0.11/pyproject.toml
--rw-rw-r--   0 test      (1000) test      (1000)      102 2024-03-25 11:43:43.475982 auto_round-0.11/setup.cfg
--rw-rw-r--   0 test      (1000) test      (1000)     1487 2024-03-08 07:32:51.000000 auto_round-0.11/setup.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-03-25 11:43:43.475982 auto_round-0.11/test/
--rw-rw-r--   0 test      (1000) test      (1000)     1312 2024-03-08 07:32:51.000000 auto_round-0.11/test/test_autoopt.py
--rw-rw-r--   0 test      (1000) test      (1000)     4054 2024-03-08 07:32:51.000000 auto_round-0.11/test/test_autoround.py
--rw-rw-r--   0 test      (1000) test      (1000)     3481 2024-03-08 07:32:51.000000 auto_round-0.11/test/test_autoround_export.py
--rw-rw-r--   0 test      (1000) test      (1000)     5375 2024-03-08 07:32:51.000000 auto_round-0.11/third-party-programs.txt
+drwxrwxr-x   0 suyueche  (1162) suyueche  (1163)        0 2024-05-29 16:52:36.022160 auto_round-0.2/
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)    10172 2024-05-29 16:51:49.000000 auto_round-0.2/LICENSE
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)    19427 2024-05-29 16:52:36.023161 auto_round-0.2/PKG-INFO
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)    17005 2024-05-29 16:51:49.000000 auto_round-0.2/README.md
+drwxrwxr-x   0 suyueche  (1162) suyueche  (1163)        0 2024-05-29 16:52:35.979161 auto_round-0.2/auto_round/
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)      678 2024-05-29 16:51:49.000000 auto_round-0.2/auto_round/__init__.py
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)    18380 2024-05-29 16:51:49.000000 auto_round-0.2/auto_round/auto_quantizer.py
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)    72813 2024-05-29 16:51:49.000000 auto_round-0.2/auto_round/autoround.py
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)    11233 2024-05-29 16:51:49.000000 auto_round-0.2/auto_round/calib_dataset.py
+drwxrwxr-x   0 suyueche  (1162) suyueche  (1163)        0 2024-05-29 16:52:35.996161 auto_round-0.2/auto_round/export/
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)      829 2024-05-29 16:51:49.000000 auto_round-0.2/auto_round/export/__init__.py
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)    10773 2024-05-29 16:51:49.000000 auto_round-0.2/auto_round/export/export_to_autogptq.py
+drwxrwxr-x   0 suyueche  (1162) suyueche  (1163)        0 2024-05-29 16:52:36.000161 auto_round-0.2/auto_round/export/export_to_autoround/
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)      647 2024-05-29 16:51:49.000000 auto_round-0.2/auto_round/export/export_to_autoround/__init__.py
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)     7660 2024-05-29 16:51:49.000000 auto_round-0.2/auto_round/export/export_to_autoround/export_to_autoround.py
+drwxrwxr-x   0 suyueche  (1162) suyueche  (1163)        0 2024-05-29 16:52:36.011160 auto_round-0.2/auto_round/export/export_to_itrex/
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)      672 2024-05-29 16:51:49.000000 auto_round-0.2/auto_round/export/export_to_itrex/__init__.py
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)    11672 2024-05-29 16:51:49.000000 auto_round-0.2/auto_round/export/export_to_itrex/config.py
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)     9016 2024-05-29 16:51:49.000000 auto_round-0.2/auto_round/export/export_to_itrex/export.py
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)    14884 2024-05-29 16:51:49.000000 auto_round-0.2/auto_round/export/export_to_itrex/model_wrapper.py
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)     1031 2024-05-29 16:51:49.000000 auto_round-0.2/auto_round/export/register.py
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)    14989 2024-05-29 16:51:49.000000 auto_round-0.2/auto_round/sign_sgd.py
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)     2102 2024-05-29 16:51:49.000000 auto_round-0.2/auto_round/special_model_handler.py
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)    26216 2024-05-29 16:51:49.000000 auto_round-0.2/auto_round/utils.py
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)      730 2024-05-29 16:51:49.000000 auto_round-0.2/auto_round/version.py
+drwxrwxr-x   0 suyueche  (1162) suyueche  (1163)        0 2024-05-29 16:52:35.989161 auto_round-0.2/auto_round.egg-info/
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)    19427 2024-05-29 16:52:35.000000 auto_round-0.2/auto_round.egg-info/PKG-INFO
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)      932 2024-05-29 16:52:35.000000 auto_round-0.2/auto_round.egg-info/SOURCES.txt
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)        1 2024-05-29 16:52:35.000000 auto_round-0.2/auto_round.egg-info/dependency_links.txt
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)       74 2024-05-29 16:52:35.000000 auto_round-0.2/auto_round.egg-info/requires.txt
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)       11 2024-05-29 16:52:35.000000 auto_round-0.2/auto_round.egg-info/top_level.txt
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)      102 2024-05-29 16:52:36.026160 auto_round-0.2/setup.cfg
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)     1487 2024-05-29 16:51:49.000000 auto_round-0.2/setup.py
+drwxrwxr-x   0 suyueche  (1162) suyueche  (1163)        0 2024-05-29 16:52:36.021160 auto_round-0.2/test/
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)     1333 2024-05-29 16:51:49.000000 auto_round-0.2/test/test_autoopt.py
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)     4768 2024-05-29 16:51:49.000000 auto_round-0.2/test/test_autoround.py
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)     3482 2024-05-29 16:51:49.000000 auto_round-0.2/test/test_autoround_export.py
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)     2552 2024-05-29 16:51:49.000000 auto_round-0.2/test/test_calib_dataset.py
+-rw-rw-r--   0 suyueche  (1162) suyueche  (1163)     5375 2024-05-29 16:51:49.000000 auto_round-0.2/third-party-programs.txt
```

### Comparing `auto_round-0.11/LICENSE` & `auto_round-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_round-0.11/PKG-INFO` & `auto_round-0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,218 +1,219 @@
-Metadata-Version: 2.1
-Name: auto_round
-Version: 0.11
-Summary: Repository of AutoRound: Advanced Weight-Only Quantization Algorithm for LLMs
-Home-page: https://github.com/intel/auto-round
-Author: Intel AIPT Team
-Author-email: wenhua.cheng@intel.com, weiwei1.zhang@intel.com
-License: Apache 2.0
-Keywords: quantization,auto-around,LLM,SignRound
-Platform: UNKNOWN
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: third-party-programs.txt
-
 <div align="center">
 
 AutoRound
 ===========================
 <h3> Advanced Weight-Only Quantization Algorithm for LLMs</h3>
 
 [![python](https://img.shields.io/badge/python-3.8%2B-blue)](https://github.com/intel/auto-round)
-[![version](https://img.shields.io/badge/release-0.1-green)](https://github.com/intel/auto-round)
+[![version](https://img.shields.io/badge/release-0.2-green)](https://github.com/intel/auto-round)
 [![license](https://img.shields.io/badge/license-Apache%202-blue)](https://github.com/intel/auto-round/blob/main/LICENSE)
 ---
 <div align="left">
 
-AutoRound is an advanced weight-only quantization algorithm for low-bits LLM inference. It's tailored for a wide range of models and consistently delivers noticeable improvements, often significantly outperforming SignRound with the cost of more tuning time for quantization.
+AutoRound is an advanced weight-only quantization algorithm for low-bits LLM inference. It's tailored for a wide range
+of models and consistently delivers noticeable improvements, often significantly outperforming SignRound with the cost
+of more tuning time for quantization.
+
+Our method adopts sign gradient descent to fine-tune rounding values and minmax values of weights in just 200 steps,
+which competes impressively against recent methods without introducing any additional inference overhead. The below
+image presents an overview of AutoRound.
+
+<div align="center">
+
+![](docs/imgs/autoround_overview.png)
+
+<div align="left">
+
+## What's New
+
+* [2024/05] Check out our updated paper on [arxiv](https://arxiv.org/pdf/2309.05516v4)
+* [2024/05] AutoRound supports lm-head quantization, saving 0.7G for LLaMA3-8B at W4G128.
+* [2024/05] AutoRound performs well
+  in [low_bit_open_llm_leaderboard](https://huggingface.co/spaces/Intel/low_bit_open_llm_leaderboard)
 
 ## Prerequisites
+
 - Python 3.9 or higher
 
 ## Installation
+
 ### Build from Source
+
 ```bash
 pip install -r requirements.txt
 python setup.py install
 ```
+
 ### Install from pypi
+
 ```bash
 pip install auto-round
 ```
-## Usage of Tuning
 
-### On CPU/ Gaudi2/ GPU
+## Model quantization
+
+### Gaudi2/ CPU/ GPU
+
+We found a significant accuracy discrepancy with the qdq model using the AutoGPTQ GPU backend with asymmetric
+quantization in some scenarios. Please switch to symmetric quantization to alleviate this issue.
 
 ```python
-import torch
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
-tuning_device = "cuda:0"  ## or "cpu", "hpu"
-dtype = "auto" if tuning_device != "hpu" else torch.bfloat16
 model_name = "meta-llama/Llama-2-7b-hf"
-model = AutoModelForCausalLM.from_pretrained(model_name, torch_dtype=dtype, trust_remote_code=True)
+model = AutoModelForCausalLM.from_pretrained(model_name, torch_dtype="auto", trust_remote_code=True)
 tokenizer = AutoTokenizer.from_pretrained(model_name, trust_remote_code=True)
 
 from auto_round import AutoRound
 
 bits, group_size, sym = 4, 128, False
-autoround = AutoRound(model, tokenizer, bits=bits, group_size=group_size, sym=sym, device=tuning_device)
+##device:Optional["auto", None, "hpu", "cpu", "cuda"]
+autoround = AutoRound(model, tokenizer, bits=bits, group_size=group_size, sym=sym, device=None)
 autoround.quantize()
 output_dir = "./tmp_autoround"
 autoround.save_quantized(output_dir)
 ```
 
-
-
-## Model inference
-Please run the tuning code first
-
-
-
-### Intel CPU
-```python
-# Please save the quantized model in 'itrex' format first, then refer to the ITREX tutorial for more details on inference with the INT4 model.
-# (https://github.com/intel/intel-extension-for-transformers/tree/main/intel_extension_for_transformers/llm/runtime/neural_speed)
-from intel_extension_for_transformers.transformers import AutoModelForCausalLM, WeightOnlyQuantConfig
-from transformers import AutoTokenizer
-
-quantized_model_path = "./tmp_autoround"
-scheme = "sym" if sym else "asym"
-woq_config = WeightOnlyQuantConfig(
-    group_size=group_size, scheme=scheme, use_autoround=True
-)  ##only supports 4 bits currently
-prompt = "There is a girl who likes adventure,"
-tokenizer = AutoTokenizer.from_pretrained(quantized_model_path, trust_remote_code=True)
-inputs = tokenizer(prompt, return_tensors="pt").input_ids
-model = AutoModelForCausalLM.from_pretrained(
-    quantized_model_path, quantization_config=woq_config, trust_remote_code=True, device="cpu"
-)
-outputs = model.generate(inputs, max_new_tokens=50)
-print(tokenizer.decode(outputs[0]))
-```
-
-
-### GPU
-```python
-from transformers import AutoModelForCausalLM, AutoTokenizer
-
-quantized_model_path = "./tmp_autoround"
-model = AutoModelForCausalLM.from_pretrained(quantized_model_path, device_map="auto", trust_remote_code=True)
-tokenizer = AutoTokenizer.from_pretrained(quantized_model_path, use_fast=True)
-text = "There is a girl who likes adventure,"
-inputs = tokenizer(text, return_tensors="pt").to(model.device)
-print(tokenizer.decode(model.generate(**inputs, max_new_tokens=50)[0]))
-```
-
 <details>
   <summary>Detailed Hyperparameters</summary>
 
 - `model`: The PyTorch model to be quantized.
-            
-- `tokenizer`: An optional tokenizer for processing input data. If none is provided, a dataloader must be supplied.
-  
+
+- `tokenizer`: An optional tokenizer for processing input data. If none, a dataset must be provided.
+
 - `bits (int)`: Number of bits for quantization (default is 4).
-  
+
 - `group_size (int)`: Size of the quantization group (default is 128).
 
-- `sym (bool)`: Whether to use symmetric quantization.
-  
-- `use_quant_input (bool)`: Whether to use the output of the previous quantized block as the input for the current block (default is True).
-  
+- `sym (bool)`: Whether to use symmetric quantization (default is False).
+
+- `enable_quanted_input (bool)`: Whether to use the output of the previous quantized block as the input for the current
+  block for tuning (default is True).
+
 - `enable_minmax_tuning (bool)`: Whether to enable weight min-max tuning (default is True).
-  
+
 - `iters (int)`: Number of tuning iterations (default is 200).
-  
+
 - `lr (float)`: The learning rate for rounding value (default is None, it will be set to 1.0/iters automatically).
-  
+
 - `minmax_lr (float)`: The learning rate for min-max tuning (default is None, it will be set to lr automatically).
-  
+
 - `n_samples (int)`: Number of samples for tuning (default is 512).
-  
+
 - `seqlen (int)`: Data length of the sequence for tuning (default is 2048).
-  
+
 - `batch_size (int)`: Batch size for training (default is 8).
 
-- `scale_dtype (str)`: The data type of quantization scale to be used (default is "float32"), different kernels have different choices.
-  
+- `scale_dtype (str)`: The data type of quantization scale to be used (default is "float16"), different kernels have
+  different choices.
+
 - `amp (bool)`: Whether to use automatic mixed precision (default is True).
-  
+
 - `n_blocks (int)`: Packing several blocks as one for tuning together (default is 1).
-  
+
 - `gradient_accumulate_steps (int)`: Number of gradient accumulation steps (default is 1).
-  
-- `low_gpu_mem_usage (bool)`: Whether to save GPU memory at the cost of a little tuning time (default is True).
-  
-- `dataset (str)`: The default dataset name for tuning (default is "NeelNanda/pile-10k").
-  
-- `dataset_split (str)`: The split of the dataset to be used for tuning (default is "train").
-  
-- `dataloader`: The dataloader for tuning data.
-  
-- `weight_config (dict)`: Configuration for weight quantization (default is an empty dictionary), mainly for mixed bits or mixed precision.
-  
+
+- `low_gpu_mem_usage (bool)`: Whether to save GPU memory at the cost of ~20% more tuning time (default is True).
+
+- `dataset Union[str, list, tuple, torch.utils.data.DataLoader]`: The dataset name for tuning (default is "
+  NeelNanda/pile-10k"). Local json file and combination of datasets have been supported, e.g. "
+  ./tmp.json,NeelNanda/pile-10k:train, mbpp:train+validation+test"
+
+- `weight_config (dict)`: Configuration for weight quantization (default is an empty dictionary), mainly for mixed bits
+  or mixed precision.
+
 - `device`: The device to be used for tuning. The default is set to 'auto', allowing for automatic detection.
 
 </details>
 
+## Model inference
+
+Please run the quantization code first.
 
-## Support List
+### CPU
+
+```python
+##Install the latest https://github.com/intel/intel-extension-for-transformers from source first.
+from intel_extension_for_transformers.transformers import AutoModelForCausalLM
+from transformers import AutoTokenizer
+
+quantized_model_path = "./tmp_autoround"
+model = AutoModelForCausalLM.from_pretrained(quantized_model_path, device_map="auto", trust_remote_code=True)
+tokenizer = AutoTokenizer.from_pretrained(quantized_model_path, use_fast=True)
+text = "There is a girl who likes adventure,"
+inputs = tokenizer(text, return_tensors="pt").to(model.device)
+print(tokenizer.decode(model.generate(**inputs, max_new_tokens=50)[0]))
+```
 
-| Model                    | Supported                                                                                                                                                                                                                                                          |
-|--------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| Intel/neural-chat-7b-v3-3 | [HF-int4-model](https://huggingface.co/Intel/neural-chat-7b-v3-3-int4-inc), [accuracy](./docs/neural-chat-7b-v3-3-acc.md), [recipe](./examples/language-modeling/scripts/neural-chat-7b-v3-3.sh), [example](./examples/language-modeling/)                         |
-| Intel/neural-chat-7b-v3-1 | [HF-int4-model](https://huggingface.co/Intel/neural-chat-7b-v3-1-int4-inc), [accuracy](./docs/neural-chat-7b-v3-1-acc.md), [recipe](./examples/language-modeling/scripts/neural-chat-7b-v3-1.sh), [example](./examples/language-modeling/)                         |
-| mistralai/Mistral-7B-v0.1 | [HF-int4-model](https://huggingface.co/Intel/Mistral-7B-v0.1-int4-inc), [accuracy](./docs/Mistral-7B-v0.1-acc.md), [recipe](./examples/language-modeling/scripts/Mistral-7B-v0.1.sh), [example](./examples/language-modeling/)                                     |
-| google/gemma-7b          | [HF-int4-model](https://huggingface.co/Intel/gemma-7b-int4-inc) under review, [accuracy](./docs/gemma-7b-acc.md), [recipe](./examples/language-modeling/scripts/gemma-7b.sh),  [example](./examples/language-modeling/)                                            |
-| google/gemma-7b-it       | [HF-int4-model](https://huggingface.co/Intel/gemma-7b-it-int4-inc) under review, [accuracy](./docs/gemma-7b-it-acc.md), [recipe](./examples/language-modeling/scripts/gemma-7b-it.sh), [example](./examples/language-modeling/)                                    |                                            |
-  mistralai/Mixtral-8x7B-Instruct-v0.1 | [HF-int4-model](https://huggingface.co/Intel/Mistral-7B-v0.1-int4-inc) under review, [accuracy](./docs/Mixtral-8x7B-Instruct-v0.1-acc.md), [recipe](./examples/language-modeling/scripts/Mixtral-8x7B-Instruct-v0.1.sh),  [example](./examples/language-modeling/) |
-| mistralai/Mixtral-8x7B-v0.1 | [HF-int4-model](https://huggingface.co/Intel/Mixtral-8x7B-v0.1-int4-inc) under review, [accuracy](./docs/Mixtral-8x7B-v0.1-acc.md), [recipe](./examples/language-modeling/scripts/Mixtral-8x7B-v0.1.sh), [example](./examples/language-modeling/)                  |
-| microsoft/phi-2          | [HF-int4-model](https://huggingface.co/Intel/phi-2-int4-inc) under review, [accuracy](./docs/phi-2-acc.md), [recipe](./examples/language-modeling/scripts/phi-2.sh), [example](./examples/language-modeling/)                                                      |
-| meta-llama/Llama-2-7b-chat-hf | [accuracy](./docs/Llama-2-7b-chat-hf-acc.md), [recipe](./examples/language-modeling/scripts/Llama-2-7b-chat-hf.sh), [example](./examples/language-modeling/)                                                                                                                    |
-| Salesforce/codegen25-7b-multi | [example](./examples/code-generation)                                                                                                                                                                                                                              |
-| EleutherAI/gpt-j-6b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| huggyllama/llama-7b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| meta-llama/Llama-2-7b-hf | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| facebook/opt-6.7b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| tiiuae/falcon-7b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| mosaicml/mpt-7b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| bigscience/bloom-7b1 | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| baichuan-inc/Baichuan-7B | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| Qwen/Qwen-7B | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| THUDM/chatglm3-6b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| MBZUAI/LaMini-GPT-124M | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| EleutherAI/gpt-neo-125m | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| databricks/dolly-v2-3b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| stabilityai/stablelm-base-alpha-3b | [example](./examples/language-modeling/)
+### GPU
 
+```python
+from transformers import AutoModelForCausalLM, AutoTokenizer
+##from auto_round.auto_quantizer import AutoHfQuantizer ## uncomment it for models with quantized lm-head
+
+quantized_model_path = "./tmp_autoround"
+model = AutoModelForCausalLM.from_pretrained(quantized_model_path, device_map="auto", trust_remote_code=True)
+tokenizer = AutoTokenizer.from_pretrained(quantized_model_path, use_fast=True)
+text = "There is a girl who likes adventure,"
+inputs = tokenizer(text, return_tensors="pt").to(model.device)
+print(tokenizer.decode(model.generate(**inputs, max_new_tokens=50)[0]))
+```
 
+## Support List
 
+| Model                                | Supported                                                                                                                                                                                                                                                                                                           |
+|--------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Intel/neural-chat-7b-v3-3            | [HF-int4-model](https://huggingface.co/Intel/neural-chat-7b-v3-3-int4-inc), [accuracy](./docs/neural-chat-7b-v3-3-acc.md), [recipe](./examples/language-modeling/scripts/neural-chat-7b-v3-3.sh), [example](./examples/language-modeling/)                                                                          |
+| Intel/neural-chat-7b-v3-1            | [HF-int4-model](https://huggingface.co/Intel/neural-chat-7b-v3-1-int4-inc), [accuracy](./docs/neural-chat-7b-v3-1-acc.md), [recipe](./examples/language-modeling/scripts/neural-chat-7b-v3-1.sh), [example](./examples/language-modeling/)                                                                          |
+| mistralai/Mistral-7B-v0.1            | [HF-int4-model-lmhead](https://huggingface.co/Intel/Mistral-7B-v0.1-int4-inc-lmhead),[HF-int4-model](https://huggingface.co/Intel/Mistral-7B-v0.1-int4-inc), [accuracy](./docs/Mistral-7B-v0.1-acc.md), [recipe](./examples/language-modeling/scripts/Mistral-7B-v0.1.sh), [example](./examples/language-modeling/) |
+| microsoft/phi-2                      | [HF-int4-sym-model](https://huggingface.co/Intel/phi-2-int4-inc), [accuracy](./docs/phi-2-acc.md), [recipe](./examples/language-modeling/scripts/phi-2.sh), [example](./examples/language-modeling/)                                                                                                                
+| google/gemma-2b                      | [HF-int4-model](https://huggingface.co/Intel/gemma-2b-int4-inc), [accuracy](./docs/gemma-2b-acc.md), [recipe](./examples/language-modeling/scripts/gemma-2b.sh),  [example](./examples/language-modeling/)                                                                                                          
+| tiiuae/falcon-7b                     | [HF-int4-model-G64](https://huggingface.co/Intel/falcon-7b-int4-inc), [accuracy](./docs/falcon-7b-acc.md), [recipe](./examples/language-modeling/scripts/falcon-7b.sh), [example](./examples/language-modeling/)                                                                                                    |
+| mistralai/Mistral-7B-Instruct-v0.2   | [HF-int4-model](https://huggingface.co/Intel/Mistral-7B-Instruct-v0.2-int4-inc) (under review), [accuracy](./docs/Mistral-7B-Instruct-v0.2-acc.md), [recipe](./examples/language-modeling/scripts/Mistral-7B-Instruct-v0.2.sh),  [example](./examples/language-modeling/)                                           |
+| google/gemma-7b                      | [HF-int4-model](https://huggingface.co/Intel/gemma-7b-int4-inc) (under review), [accuracy](./docs/gemma-7b-acc.md), [recipe](./examples/language-modeling/scripts/gemma-7b.sh),  [example](./examples/language-modeling/)                                                                                           |
+| mistralai/Mixtral-8x7B-Instruct-v0.1 | [HF-int4-model](https://huggingface.co/Intel/Mixtral-8x7B-Instruct-v0.1-int4-inc) (under review), [accuracy](./docs/Mixtral-8x7B-Instruct-v0.1-acc.md), [recipe](./examples/language-modeling/scripts/Mixtral-8x7B-Instruct-v0.1.sh),  [example](./examples/language-modeling/)                                     |
+| mistralai/Mixtral-8x7B-v0.1          | [HF-int4-model](https://huggingface.co/Intel/Mixtral-8x7B-v0.1-int4-inc) (under review), [accuracy](./docs/Mixtral-8x7B-v0.1-acc.md), [recipe](./examples/language-modeling/scripts/Mixtral-8x7B-v0.1.sh), [example](./examples/language-modeling/)                                                                 |
+| meta-llama/Meta-Llama-3-8B-Instruct  | [accuracy](./docs/Meta-Llama-3-8B-Instruct-acc.md), [recipe](./examples/language-modeling/scripts/Meta-Llama-3-8B-Instruct.sh), [example](./examples/language-modeling/)                                                                                                                                            |
+| meta-llama/Llama-2-7b-chat-hf        | [accuracy](./docs/Llama-2-7b-chat-hf-acc.md), [recipe](./examples/language-modeling/scripts/Llama-2-7b-chat-hf.sh), [example](./examples/language-modeling/)                                                                                                                                                        |
+| Qwen/Qwen1.5-7B-Chat                 | [accuracy](./docs/Qwen1.5-7B-Chat-acc.md), [sym recipe](./examples/language-modeling/scripts/Qwen1.5-7B-Chat-sym.sh), [asym recipe ](./examples/language-modeling/scripts/Qwen1.5-7B-Chat-asym.sh), [example](./examples/language-modeling/)                                                                        |
+| baichuan-inc/Baichuan2-7B-Chat       | [accuracy](./docs/baichuan2-7b-chat-acc.md), [recipe](./examples/language-modeling/scripts/baichuan2-7b-chat.sh), [example](./examples/language-modeling/)                                                                                                                                                          |
+| 01-ai/Yi-6B-Chat                     | [accuracy](./docs/Yi-6B-Chat-acc.md), [recipe](./examples/language-modeling/scripts/Yi-6B-Chat.sh), [example](./examples/language-modeling/)                                                                                                                                                                        |
+| facebook/opt-2.7b                    | [accuracy](./docs/opt-2.7b-acc.md), [recipe](./examples/language-modeling/scripts/opt-2.7b.sh), [example](./examples/language-modeling/)                                                                                                                                                                            |
+| bigscience/bloom-3b                  | [accuracy](./docs/bloom-3B-acc.md), [recipe](./examples/language-modeling/scripts/bloom-3b.sh), [example](./examples/language-modeling/)                                                                                                                                                                            |
+| EleutherAI/gpt-j-6b                  | [accuracy](./docs/gpt-j-6B-acc.md), [recipe](./examples/language-modeling/scripts/gpt-j-6b.sh), [example](./examples/language-modeling/)                                                                                                                                                                            |
+| Salesforce/codegen25-7b-multi        | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+| huggyllama/llama-7b                  | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+| mosaicml/mpt-7b                      | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+| THUDM/chatglm3-6b                    | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+| MBZUAI/LaMini-GPT-124M               | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+| EleutherAI/gpt-neo-125m              | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+| databricks/dolly-v2-3b               | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+| stabilityai/stablelm-base-alpha-3b   | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            
 
 ## Comparison with other methods
 
-We provide a [comprehensive analysis](docs/acc.md) with other methods in our accuracy data section. Notably, our approach has outperformed GPTQ with a score of 30/32 and AWQ with a score of 27/32 across llamv1/llamav2/mistral-7b on W4G-1, W4G128, W3G128, W2G128.  And the tuning costs are comparable.
+We provide a [comprehensive analysis](docs/acc.md) with other methods in our accuracy data section. In summary, our
+approach achieved superior performance compared to GPTQ, scoring 30/32, AWQ with 27/32, HQQ with 15/16, and OmniQuant
+with a perfect score of 16/16 across llamv1/llamav2/mistral-7b on W4G-1, W4G128, W3G128, and W2G128, based on the
+average accuracies of 11 zero-shot tasks.
 
 ## Tips
-1 Consider increasing tuning steps to achieve better results, albeit with increased tuning time. 
 
-2 Setting 'use_quant_input' to False has been observed to occasionally yield improved results.
+1 Consider increasing tuning steps to achieve better results, albeit with increased tuning time.
+
+2 Setting 'enable_quanted_input' to False has been observed to occasionally yield improved results.
 
 3 Setting 'minmax_lr' to 2.0/iters has been observed to occasionally yield improved results.
 
 ## Reference
+
 If you find SignRound useful for your research, please cite our paper:
+
 ```bash
 @article{cheng2023optimize,
   title={Optimize Weight Rounding via Signed Gradient Descent for the Quantization of LLMs},
-  author={Cheng, Wenhua and Zhang, Weiwei and Shen, Haihao and Cai, Yiyang and He, Xin and Lv, Kaokao},
+  author={Cheng, Wenhua and Zhang, Weiwei and Shen, Haihao and Cai, Yiyang and He, Xin and Lv, Kaokao and Liu, Yi},
   journal={arXiv preprint arXiv:2309.05516},
   year={2023}
 }
 ```
-
-
```

### Comparing `auto_round-0.11/README.md` & `auto_round-0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,197 +1,236 @@
-<div align="center">
-
-AutoRound
-===========================
-<h3> Advanced Weight-Only Quantization Algorithm for LLMs</h3>
-
-[![python](https://img.shields.io/badge/python-3.8%2B-blue)](https://github.com/intel/auto-round)
-[![version](https://img.shields.io/badge/release-0.1-green)](https://github.com/intel/auto-round)
-[![license](https://img.shields.io/badge/license-Apache%202-blue)](https://github.com/intel/auto-round/blob/main/LICENSE)
----
-<div align="left">
-
-AutoRound is an advanced weight-only quantization algorithm for low-bits LLM inference. It's tailored for a wide range of models and consistently delivers noticeable improvements, often significantly outperforming SignRound with the cost of more tuning time for quantization.
-
-## Prerequisites
-- Python 3.9 or higher
-
-## Installation
-### Build from Source
-```bash
-pip install -r requirements.txt
-python setup.py install
-```
-### Install from pypi
-```bash
-pip install auto-round
-```
-## Usage of Tuning
-
-### On CPU/ Gaudi2/ GPU
-
-```python
-import torch
-from transformers import AutoModelForCausalLM, AutoTokenizer
-
-tuning_device = "cuda:0"  ## or "cpu", "hpu"
-dtype = "auto" if tuning_device != "hpu" else torch.bfloat16
-model_name = "meta-llama/Llama-2-7b-hf"
-model = AutoModelForCausalLM.from_pretrained(model_name, torch_dtype=dtype, trust_remote_code=True)
-tokenizer = AutoTokenizer.from_pretrained(model_name, trust_remote_code=True)
-
-from auto_round import AutoRound
-
-bits, group_size, sym = 4, 128, False
-autoround = AutoRound(model, tokenizer, bits=bits, group_size=group_size, sym=sym, device=tuning_device)
-autoround.quantize()
-output_dir = "./tmp_autoround"
-autoround.save_quantized(output_dir)
-```
-
-
-
-## Model inference
-Please run the tuning code first
-
-
-
-### Intel CPU
-```python
-# Please save the quantized model in 'itrex' format first, then refer to the ITREX tutorial for more details on inference with the INT4 model.
-# (https://github.com/intel/intel-extension-for-transformers/tree/main/intel_extension_for_transformers/llm/runtime/neural_speed)
-from intel_extension_for_transformers.transformers import AutoModelForCausalLM, WeightOnlyQuantConfig
-from transformers import AutoTokenizer
-
-quantized_model_path = "./tmp_autoround"
-scheme = "sym" if sym else "asym"
-woq_config = WeightOnlyQuantConfig(
-    group_size=group_size, scheme=scheme, use_autoround=True
-)  ##only supports 4 bits currently
-prompt = "There is a girl who likes adventure,"
-tokenizer = AutoTokenizer.from_pretrained(quantized_model_path, trust_remote_code=True)
-inputs = tokenizer(prompt, return_tensors="pt").input_ids
-model = AutoModelForCausalLM.from_pretrained(
-    quantized_model_path, quantization_config=woq_config, trust_remote_code=True, device="cpu"
-)
-outputs = model.generate(inputs, max_new_tokens=50)
-print(tokenizer.decode(outputs[0]))
-```
-
-
-### GPU
-```python
-from transformers import AutoModelForCausalLM, AutoTokenizer
-
-quantized_model_path = "./tmp_autoround"
-model = AutoModelForCausalLM.from_pretrained(quantized_model_path, device_map="auto", trust_remote_code=True)
-tokenizer = AutoTokenizer.from_pretrained(quantized_model_path, use_fast=True)
-text = "There is a girl who likes adventure,"
-inputs = tokenizer(text, return_tensors="pt").to(model.device)
-print(tokenizer.decode(model.generate(**inputs, max_new_tokens=50)[0]))
-```
-
-<details>
-  <summary>Detailed Hyperparameters</summary>
-
-- `model`: The PyTorch model to be quantized.
-            
-- `tokenizer`: An optional tokenizer for processing input data. If none is provided, a dataloader must be supplied.
-  
-- `bits (int)`: Number of bits for quantization (default is 4).
-  
-- `group_size (int)`: Size of the quantization group (default is 128).
-
-- `sym (bool)`: Whether to use symmetric quantization.
-  
-- `use_quant_input (bool)`: Whether to use the output of the previous quantized block as the input for the current block (default is True).
-  
-- `enable_minmax_tuning (bool)`: Whether to enable weight min-max tuning (default is True).
-  
-- `iters (int)`: Number of tuning iterations (default is 200).
-  
-- `lr (float)`: The learning rate for rounding value (default is None, it will be set to 1.0/iters automatically).
-  
-- `minmax_lr (float)`: The learning rate for min-max tuning (default is None, it will be set to lr automatically).
-  
-- `n_samples (int)`: Number of samples for tuning (default is 512).
-  
-- `seqlen (int)`: Data length of the sequence for tuning (default is 2048).
-  
-- `batch_size (int)`: Batch size for training (default is 8).
-
-- `scale_dtype (str)`: The data type of quantization scale to be used (default is "float32"), different kernels have different choices.
-  
-- `amp (bool)`: Whether to use automatic mixed precision (default is True).
-  
-- `n_blocks (int)`: Packing several blocks as one for tuning together (default is 1).
-  
-- `gradient_accumulate_steps (int)`: Number of gradient accumulation steps (default is 1).
-  
-- `low_gpu_mem_usage (bool)`: Whether to save GPU memory at the cost of a little tuning time (default is True).
-  
-- `dataset (str)`: The default dataset name for tuning (default is "NeelNanda/pile-10k").
-  
-- `dataset_split (str)`: The split of the dataset to be used for tuning (default is "train").
-  
-- `dataloader`: The dataloader for tuning data.
-  
-- `weight_config (dict)`: Configuration for weight quantization (default is an empty dictionary), mainly for mixed bits or mixed precision.
-  
-- `device`: The device to be used for tuning. The default is set to 'auto', allowing for automatic detection.
-
-</details>
-
-
-## Support List
-
-| Model                    | Supported                                                                                                                                                                                                                                                          |
-|--------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| Intel/neural-chat-7b-v3-3 | [HF-int4-model](https://huggingface.co/Intel/neural-chat-7b-v3-3-int4-inc), [accuracy](./docs/neural-chat-7b-v3-3-acc.md), [recipe](./examples/language-modeling/scripts/neural-chat-7b-v3-3.sh), [example](./examples/language-modeling/)                         |
-| Intel/neural-chat-7b-v3-1 | [HF-int4-model](https://huggingface.co/Intel/neural-chat-7b-v3-1-int4-inc), [accuracy](./docs/neural-chat-7b-v3-1-acc.md), [recipe](./examples/language-modeling/scripts/neural-chat-7b-v3-1.sh), [example](./examples/language-modeling/)                         |
-| mistralai/Mistral-7B-v0.1 | [HF-int4-model](https://huggingface.co/Intel/Mistral-7B-v0.1-int4-inc), [accuracy](./docs/Mistral-7B-v0.1-acc.md), [recipe](./examples/language-modeling/scripts/Mistral-7B-v0.1.sh), [example](./examples/language-modeling/)                                     |
-| google/gemma-7b          | [HF-int4-model](https://huggingface.co/Intel/gemma-7b-int4-inc) under review, [accuracy](./docs/gemma-7b-acc.md), [recipe](./examples/language-modeling/scripts/gemma-7b.sh),  [example](./examples/language-modeling/)                                            |
-| google/gemma-7b-it       | [HF-int4-model](https://huggingface.co/Intel/gemma-7b-it-int4-inc) under review, [accuracy](./docs/gemma-7b-it-acc.md), [recipe](./examples/language-modeling/scripts/gemma-7b-it.sh), [example](./examples/language-modeling/)                                    |                                            |
-  mistralai/Mixtral-8x7B-Instruct-v0.1 | [HF-int4-model](https://huggingface.co/Intel/Mistral-7B-v0.1-int4-inc) under review, [accuracy](./docs/Mixtral-8x7B-Instruct-v0.1-acc.md), [recipe](./examples/language-modeling/scripts/Mixtral-8x7B-Instruct-v0.1.sh),  [example](./examples/language-modeling/) |
-| mistralai/Mixtral-8x7B-v0.1 | [HF-int4-model](https://huggingface.co/Intel/Mixtral-8x7B-v0.1-int4-inc) under review, [accuracy](./docs/Mixtral-8x7B-v0.1-acc.md), [recipe](./examples/language-modeling/scripts/Mixtral-8x7B-v0.1.sh), [example](./examples/language-modeling/)                  |
-| microsoft/phi-2          | [HF-int4-model](https://huggingface.co/Intel/phi-2-int4-inc) under review, [accuracy](./docs/phi-2-acc.md), [recipe](./examples/language-modeling/scripts/phi-2.sh), [example](./examples/language-modeling/)                                                      |
-| meta-llama/Llama-2-7b-chat-hf | [accuracy](./docs/Llama-2-7b-chat-hf-acc.md), [recipe](./examples/language-modeling/scripts/Llama-2-7b-chat-hf.sh), [example](./examples/language-modeling/)                                                                                                                    |
-| Salesforce/codegen25-7b-multi | [example](./examples/code-generation)                                                                                                                                                                                                                              |
-| EleutherAI/gpt-j-6b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| huggyllama/llama-7b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| meta-llama/Llama-2-7b-hf | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| facebook/opt-6.7b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| tiiuae/falcon-7b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| mosaicml/mpt-7b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| bigscience/bloom-7b1 | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| baichuan-inc/Baichuan-7B | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| Qwen/Qwen-7B | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| THUDM/chatglm3-6b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| MBZUAI/LaMini-GPT-124M | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| EleutherAI/gpt-neo-125m | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| databricks/dolly-v2-3b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| stabilityai/stablelm-base-alpha-3b | [example](./examples/language-modeling/)
-
-
-
-
-## Comparison with other methods
-
-We provide a [comprehensive analysis](docs/acc.md) with other methods in our accuracy data section. Notably, our approach has outperformed GPTQ with a score of 30/32 and AWQ with a score of 27/32 across llamv1/llamav2/mistral-7b on W4G-1, W4G128, W3G128, W2G128.  And the tuning costs are comparable.
-
-## Tips
-1 Consider increasing tuning steps to achieve better results, albeit with increased tuning time. 
-
-2 Setting 'use_quant_input' to False has been observed to occasionally yield improved results.
-
-3 Setting 'minmax_lr' to 2.0/iters has been observed to occasionally yield improved results.
-
-## Reference
-If you find SignRound useful for your research, please cite our paper:
-```bash
-@article{cheng2023optimize,
-  title={Optimize Weight Rounding via Signed Gradient Descent for the Quantization of LLMs},
-  author={Cheng, Wenhua and Zhang, Weiwei and Shen, Haihao and Cai, Yiyang and He, Xin and Lv, Kaokao},
-  journal={arXiv preprint arXiv:2309.05516},
-  year={2023}
-}
-```
+Metadata-Version: 2.1
+Name: auto_round
+Version: 0.2
+Summary: Repository of AutoRound: Advanced Weight-Only Quantization Algorithm for LLMs
+Home-page: https://github.com/intel/auto-round
+Author: Intel AIPT Team
+Author-email: wenhua.cheng@intel.com, weiwei1.zhang@intel.com
+License: Apache 2.0
+Description: <div align="center">
+        
+        AutoRound
+        ===========================
+        <h3> Advanced Weight-Only Quantization Algorithm for LLMs</h3>
+        
+        [![python](https://img.shields.io/badge/python-3.8%2B-blue)](https://github.com/intel/auto-round)
+        [![version](https://img.shields.io/badge/release-0.2-green)](https://github.com/intel/auto-round)
+        [![license](https://img.shields.io/badge/license-Apache%202-blue)](https://github.com/intel/auto-round/blob/main/LICENSE)
+        ---
+        <div align="left">
+        
+        AutoRound is an advanced weight-only quantization algorithm for low-bits LLM inference. It's tailored for a wide range
+        of models and consistently delivers noticeable improvements, often significantly outperforming SignRound with the cost
+        of more tuning time for quantization.
+        
+        Our method adopts sign gradient descent to fine-tune rounding values and minmax values of weights in just 200 steps,
+        which competes impressively against recent methods without introducing any additional inference overhead. The below
+        image presents an overview of AutoRound.
+        
+        <div align="center">
+        
+        ![](docs/imgs/autoround_overview.png)
+        
+        <div align="left">
+        
+        ## What's New
+        
+        * [2024/05] Check out our updated paper on [arxiv](https://arxiv.org/pdf/2309.05516v4)
+        * [2024/05] AutoRound supports lm-head quantization, saving 0.7G for LLaMA3-8B at W4G128.
+        * [2024/05] AutoRound performs well
+          in [low_bit_open_llm_leaderboard](https://huggingface.co/spaces/Intel/low_bit_open_llm_leaderboard)
+        
+        ## Prerequisites
+        
+        - Python 3.9 or higher
+        
+        ## Installation
+        
+        ### Build from Source
+        
+        ```bash
+        pip install -r requirements.txt
+        python setup.py install
+        ```
+        
+        ### Install from pypi
+        
+        ```bash
+        pip install auto-round
+        ```
+        
+        ## Model quantization
+        
+        ### Gaudi2/ CPU/ GPU
+        
+        We found a significant accuracy discrepancy with the qdq model using the AutoGPTQ GPU backend with asymmetric
+        quantization in some scenarios. Please switch to symmetric quantization to alleviate this issue.
+        
+        ```python
+        from transformers import AutoModelForCausalLM, AutoTokenizer
+        
+        model_name = "meta-llama/Llama-2-7b-hf"
+        model = AutoModelForCausalLM.from_pretrained(model_name, torch_dtype="auto", trust_remote_code=True)
+        tokenizer = AutoTokenizer.from_pretrained(model_name, trust_remote_code=True)
+        
+        from auto_round import AutoRound
+        
+        bits, group_size, sym = 4, 128, False
+        ##device:Optional["auto", None, "hpu", "cpu", "cuda"]
+        autoround = AutoRound(model, tokenizer, bits=bits, group_size=group_size, sym=sym, device=None)
+        autoround.quantize()
+        output_dir = "./tmp_autoround"
+        autoround.save_quantized(output_dir)
+        ```
+        
+        <details>
+          <summary>Detailed Hyperparameters</summary>
+        
+        - `model`: The PyTorch model to be quantized.
+        
+        - `tokenizer`: An optional tokenizer for processing input data. If none, a dataset must be provided.
+        
+        - `bits (int)`: Number of bits for quantization (default is 4).
+        
+        - `group_size (int)`: Size of the quantization group (default is 128).
+        
+        - `sym (bool)`: Whether to use symmetric quantization (default is False).
+        
+        - `enable_quanted_input (bool)`: Whether to use the output of the previous quantized block as the input for the current
+          block for tuning (default is True).
+        
+        - `enable_minmax_tuning (bool)`: Whether to enable weight min-max tuning (default is True).
+        
+        - `iters (int)`: Number of tuning iterations (default is 200).
+        
+        - `lr (float)`: The learning rate for rounding value (default is None, it will be set to 1.0/iters automatically).
+        
+        - `minmax_lr (float)`: The learning rate for min-max tuning (default is None, it will be set to lr automatically).
+        
+        - `n_samples (int)`: Number of samples for tuning (default is 512).
+        
+        - `seqlen (int)`: Data length of the sequence for tuning (default is 2048).
+        
+        - `batch_size (int)`: Batch size for training (default is 8).
+        
+        - `scale_dtype (str)`: The data type of quantization scale to be used (default is "float16"), different kernels have
+          different choices.
+        
+        - `amp (bool)`: Whether to use automatic mixed precision (default is True).
+        
+        - `n_blocks (int)`: Packing several blocks as one for tuning together (default is 1).
+        
+        - `gradient_accumulate_steps (int)`: Number of gradient accumulation steps (default is 1).
+        
+        - `low_gpu_mem_usage (bool)`: Whether to save GPU memory at the cost of ~20% more tuning time (default is True).
+        
+        - `dataset Union[str, list, tuple, torch.utils.data.DataLoader]`: The dataset name for tuning (default is "
+          NeelNanda/pile-10k"). Local json file and combination of datasets have been supported, e.g. "
+          ./tmp.json,NeelNanda/pile-10k:train, mbpp:train+validation+test"
+        
+        - `weight_config (dict)`: Configuration for weight quantization (default is an empty dictionary), mainly for mixed bits
+          or mixed precision.
+        
+        - `device`: The device to be used for tuning. The default is set to 'auto', allowing for automatic detection.
+        
+        </details>
+        
+        ## Model inference
+        
+        Please run the quantization code first.
+        
+        ### CPU
+        
+        ```python
+        ##Install the latest https://github.com/intel/intel-extension-for-transformers from source first.
+        from intel_extension_for_transformers.transformers import AutoModelForCausalLM
+        from transformers import AutoTokenizer
+        
+        quantized_model_path = "./tmp_autoround"
+        model = AutoModelForCausalLM.from_pretrained(quantized_model_path, device_map="auto", trust_remote_code=True)
+        tokenizer = AutoTokenizer.from_pretrained(quantized_model_path, use_fast=True)
+        text = "There is a girl who likes adventure,"
+        inputs = tokenizer(text, return_tensors="pt").to(model.device)
+        print(tokenizer.decode(model.generate(**inputs, max_new_tokens=50)[0]))
+        ```
+        
+        ### GPU
+        
+        ```python
+        from transformers import AutoModelForCausalLM, AutoTokenizer
+        ##from auto_round.auto_quantizer import AutoHfQuantizer ## uncomment it for models with quantized lm-head
+        
+        quantized_model_path = "./tmp_autoround"
+        model = AutoModelForCausalLM.from_pretrained(quantized_model_path, device_map="auto", trust_remote_code=True)
+        tokenizer = AutoTokenizer.from_pretrained(quantized_model_path, use_fast=True)
+        text = "There is a girl who likes adventure,"
+        inputs = tokenizer(text, return_tensors="pt").to(model.device)
+        print(tokenizer.decode(model.generate(**inputs, max_new_tokens=50)[0]))
+        ```
+        
+        ## Support List
+        
+        | Model                                | Supported                                                                                                                                                                                                                                                                                                           |
+        |--------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+        | Intel/neural-chat-7b-v3-3            | [HF-int4-model](https://huggingface.co/Intel/neural-chat-7b-v3-3-int4-inc), [accuracy](./docs/neural-chat-7b-v3-3-acc.md), [recipe](./examples/language-modeling/scripts/neural-chat-7b-v3-3.sh), [example](./examples/language-modeling/)                                                                          |
+        | Intel/neural-chat-7b-v3-1            | [HF-int4-model](https://huggingface.co/Intel/neural-chat-7b-v3-1-int4-inc), [accuracy](./docs/neural-chat-7b-v3-1-acc.md), [recipe](./examples/language-modeling/scripts/neural-chat-7b-v3-1.sh), [example](./examples/language-modeling/)                                                                          |
+        | mistralai/Mistral-7B-v0.1            | [HF-int4-model-lmhead](https://huggingface.co/Intel/Mistral-7B-v0.1-int4-inc-lmhead),[HF-int4-model](https://huggingface.co/Intel/Mistral-7B-v0.1-int4-inc), [accuracy](./docs/Mistral-7B-v0.1-acc.md), [recipe](./examples/language-modeling/scripts/Mistral-7B-v0.1.sh), [example](./examples/language-modeling/) |
+        | microsoft/phi-2                      | [HF-int4-sym-model](https://huggingface.co/Intel/phi-2-int4-inc), [accuracy](./docs/phi-2-acc.md), [recipe](./examples/language-modeling/scripts/phi-2.sh), [example](./examples/language-modeling/)                                                                                                                
+        | google/gemma-2b                      | [HF-int4-model](https://huggingface.co/Intel/gemma-2b-int4-inc), [accuracy](./docs/gemma-2b-acc.md), [recipe](./examples/language-modeling/scripts/gemma-2b.sh),  [example](./examples/language-modeling/)                                                                                                          
+        | tiiuae/falcon-7b                     | [HF-int4-model-G64](https://huggingface.co/Intel/falcon-7b-int4-inc), [accuracy](./docs/falcon-7b-acc.md), [recipe](./examples/language-modeling/scripts/falcon-7b.sh), [example](./examples/language-modeling/)                                                                                                    |
+        | mistralai/Mistral-7B-Instruct-v0.2   | [HF-int4-model](https://huggingface.co/Intel/Mistral-7B-Instruct-v0.2-int4-inc) (under review), [accuracy](./docs/Mistral-7B-Instruct-v0.2-acc.md), [recipe](./examples/language-modeling/scripts/Mistral-7B-Instruct-v0.2.sh),  [example](./examples/language-modeling/)                                           |
+        | google/gemma-7b                      | [HF-int4-model](https://huggingface.co/Intel/gemma-7b-int4-inc) (under review), [accuracy](./docs/gemma-7b-acc.md), [recipe](./examples/language-modeling/scripts/gemma-7b.sh),  [example](./examples/language-modeling/)                                                                                           |
+        | mistralai/Mixtral-8x7B-Instruct-v0.1 | [HF-int4-model](https://huggingface.co/Intel/Mixtral-8x7B-Instruct-v0.1-int4-inc) (under review), [accuracy](./docs/Mixtral-8x7B-Instruct-v0.1-acc.md), [recipe](./examples/language-modeling/scripts/Mixtral-8x7B-Instruct-v0.1.sh),  [example](./examples/language-modeling/)                                     |
+        | mistralai/Mixtral-8x7B-v0.1          | [HF-int4-model](https://huggingface.co/Intel/Mixtral-8x7B-v0.1-int4-inc) (under review), [accuracy](./docs/Mixtral-8x7B-v0.1-acc.md), [recipe](./examples/language-modeling/scripts/Mixtral-8x7B-v0.1.sh), [example](./examples/language-modeling/)                                                                 |
+        | meta-llama/Meta-Llama-3-8B-Instruct  | [accuracy](./docs/Meta-Llama-3-8B-Instruct-acc.md), [recipe](./examples/language-modeling/scripts/Meta-Llama-3-8B-Instruct.sh), [example](./examples/language-modeling/)                                                                                                                                            |
+        | meta-llama/Llama-2-7b-chat-hf        | [accuracy](./docs/Llama-2-7b-chat-hf-acc.md), [recipe](./examples/language-modeling/scripts/Llama-2-7b-chat-hf.sh), [example](./examples/language-modeling/)                                                                                                                                                        |
+        | Qwen/Qwen1.5-7B-Chat                 | [accuracy](./docs/Qwen1.5-7B-Chat-acc.md), [sym recipe](./examples/language-modeling/scripts/Qwen1.5-7B-Chat-sym.sh), [asym recipe ](./examples/language-modeling/scripts/Qwen1.5-7B-Chat-asym.sh), [example](./examples/language-modeling/)                                                                        |
+        | baichuan-inc/Baichuan2-7B-Chat       | [accuracy](./docs/baichuan2-7b-chat-acc.md), [recipe](./examples/language-modeling/scripts/baichuan2-7b-chat.sh), [example](./examples/language-modeling/)                                                                                                                                                          |
+        | 01-ai/Yi-6B-Chat                     | [accuracy](./docs/Yi-6B-Chat-acc.md), [recipe](./examples/language-modeling/scripts/Yi-6B-Chat.sh), [example](./examples/language-modeling/)                                                                                                                                                                        |
+        | facebook/opt-2.7b                    | [accuracy](./docs/opt-2.7b-acc.md), [recipe](./examples/language-modeling/scripts/opt-2.7b.sh), [example](./examples/language-modeling/)                                                                                                                                                                            |
+        | bigscience/bloom-3b                  | [accuracy](./docs/bloom-3B-acc.md), [recipe](./examples/language-modeling/scripts/bloom-3b.sh), [example](./examples/language-modeling/)                                                                                                                                                                            |
+        | EleutherAI/gpt-j-6b                  | [accuracy](./docs/gpt-j-6B-acc.md), [recipe](./examples/language-modeling/scripts/gpt-j-6b.sh), [example](./examples/language-modeling/)                                                                                                                                                                            |
+        | Salesforce/codegen25-7b-multi        | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+        | huggyllama/llama-7b                  | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+        | mosaicml/mpt-7b                      | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+        | THUDM/chatglm3-6b                    | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+        | MBZUAI/LaMini-GPT-124M               | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+        | EleutherAI/gpt-neo-125m              | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+        | databricks/dolly-v2-3b               | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+        | stabilityai/stablelm-base-alpha-3b   | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            
+        
+        ## Comparison with other methods
+        
+        We provide a [comprehensive analysis](docs/acc.md) with other methods in our accuracy data section. In summary, our
+        approach achieved superior performance compared to GPTQ, scoring 30/32, AWQ with 27/32, HQQ with 15/16, and OmniQuant
+        with a perfect score of 16/16 across llamv1/llamav2/mistral-7b on W4G-1, W4G128, W3G128, and W2G128, based on the
+        average accuracies of 11 zero-shot tasks.
+        
+        ## Tips
+        
+        1 Consider increasing tuning steps to achieve better results, albeit with increased tuning time.
+        
+        2 Setting 'enable_quanted_input' to False has been observed to occasionally yield improved results.
+        
+        3 Setting 'minmax_lr' to 2.0/iters has been observed to occasionally yield improved results.
+        
+        ## Reference
+        
+        If you find SignRound useful for your research, please cite our paper:
+        
+        ```bash
+        @article{cheng2023optimize,
+          title={Optimize Weight Rounding via Signed Gradient Descent for the Quantization of LLMs},
+          author={Cheng, Wenhua and Zhang, Weiwei and Shen, Haihao and Cai, Yiyang and He, Xin and Lv, Kaokao and Liu, Yi},
+          journal={arXiv preprint arXiv:2309.05516},
+          year={2023}
+        }
+        ```
+        
+Keywords: quantization,auto-around,LLM,SignRound
+Platform: UNKNOWN
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
```

### Comparing `auto_round-0.11/auto_round/__init__.py` & `auto_round-0.2/auto_round/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from .autoround import AutoRound, AutoAdamRound, AutoOPTRound
-from .version import __version__
+from .version import __version__
```

### Comparing `auto_round-0.11/auto_round/autoround.py` & `auto_round-0.2/auto_round/autoround.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,37 +11,41 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import copy
 import time
+from typing import Optional, Union
 
 import torch
+import transformers
+from torch import autocast
 
+from .calib_dataset import get_dataloader
+from .special_model_handler import check_hidden_state_dim, check_share_attention_mask
 from .utils import (
     CpuInfo,
     block_forward,
     check_is_cpu,
     check_to_quantized,
     collect_minmax_scale,
     collect_round_v,
+    convert_dtype_str2torch,
     detect_device,
-    get_batch_dim,
     get_block_names,
     get_module,
     get_scale_shape,
     htcore,
     is_optimum_habana_available,
-    is_share_attention_mask_model,
     logger,
-    move_input_to_device,
     quant_weight,
     sampling_inputs,
     set_module,
+    to_device,
 )
 
 
 class WrapperLinear(torch.nn.Module):
     def __init__(self, orig_layer, enable_minmax_tuning=True):
         """A wrapper module for linear layers that enables quantization and min-max tuning of weights.
 
@@ -61,30 +65,33 @@
         """
         super(WrapperLinear, self).__init__()
         self.orig_layer = orig_layer
         self.num_bits = self.orig_layer.bits
         self.group_size = self.orig_layer.group_size
         self.scale_dtype = self.orig_layer.scale_dtype
         self.sym = self.orig_layer.sym
+        weight_dtype = self.orig_layer.weight.dtype
+        weight_dtype = torch.float32  ##TODO revert the change to check the accuracy
         self.value = torch.nn.Parameter(
-            torch.zeros(self.orig_layer.weight.shape, device=self.orig_layer.weight.device), requires_grad=True
+            torch.zeros(self.orig_layer.weight.shape, device=self.orig_layer.weight.device, dtype=weight_dtype),
+            requires_grad=True,
         )
         self.enable_minmax_tuning = enable_minmax_tuning
         shape = get_scale_shape(self.orig_layer.weight, self.group_size)
-
+        weight_dtype = self.orig_layer.weight.dtype
         if self.enable_minmax_tuning:
             self.min_scale = torch.nn.Parameter(
-                torch.zeros(shape, device=self.orig_layer.weight.device), requires_grad=True
+                torch.zeros(shape, device=self.orig_layer.weight.device, dtype=weight_dtype), requires_grad=True
             )
             self.max_scale = torch.nn.Parameter(
-                torch.zeros(shape, device=self.orig_layer.weight.device), requires_grad=True
+                torch.zeros(shape, device=self.orig_layer.weight.device, dtype=weight_dtype), requires_grad=True
             )
         else:
-            self.min_scale = torch.tensor(0, device=self.orig_layer.weight.device)
-            self.max_scale = torch.tensor(0, device=self.orig_layer.weight.device)
+            self.min_scale = torch.tensor(0, device=self.orig_layer.weight.device, dtype=weight_dtype)
+            self.max_scale = torch.tensor(0, device=self.orig_layer.weight.device, dtype=weight_dtype)
 
     def unwrapper(self, v, min_scale, max_scale):
         """Unwrapper the layer to the original layer.
 
         Args:
         - v (torch.Tensor): The rounding v parameter for quantization.
         - min_scale (torch.nn.Parameter or torch.Tensor): The minimum scale for min-max tuning.
@@ -165,27 +172,37 @@
         - max_scale (torch.nn.Parameter or torch.Tensor): The maximum scale for min-max tuning.
         """
         super(WrapperTransformerConv1d, self).__init__()
         self.orig_layer = orig_layer
         self.num_bits = self.orig_layer.bits
         self.group_size = self.orig_layer.group_size
         self.sym = self.orig_layer.sym
+        self.scale_dtype = self.orig_layer.scale_dtype
+        weight_dtype = self.orig_layer.weight.dtype
+        weight_dtype = torch.float32  ##TODO revert the change to check the accuracy
+
         device = self.orig_layer.weight.device
         self.weight_t = self.orig_layer.weight.t()
-        self.value = torch.nn.Parameter(torch.zeros(self.weight_t.shape, device=device), requires_grad=True)
+        self.value = torch.nn.Parameter(
+            torch.zeros(self.weight_t.shape, device=device, dtype=weight_dtype), requires_grad=True
+        )
         shape = get_scale_shape(self.weight_t, self.group_size)
 
         if enable_minmax_tuning:
-            self.min_scale = torch.nn.Parameter(torch.zeros(shape, device=device), requires_grad=True)
-            self.max_scale = torch.nn.Parameter(torch.zeros(shape, device=device), requires_grad=True)
+            self.min_scale = torch.nn.Parameter(
+                torch.zeros(shape, device=device, dtype=weight_dtype), requires_grad=True
+            )
+            self.max_scale = torch.nn.Parameter(
+                torch.zeros(shape, device=device, dtype=weight_dtype), requires_grad=True
+            )
         else:
-            self.min_scale = torch.tensor(0, device=device)
-            self.max_scale = torch.tensor(0, device=device)
+            self.min_scale = torch.tensor(0, device=device, dtype=weight_dtype)
+            self.max_scale = torch.tensor(0, device=device, dtype=weight_dtype)
 
-    def unwrapper(self, v, min_scale, max_scale):
+    def unwrapper(self, v=0, min_scale=0, max_scale=0):
         """Unwrapper the layer to the original conv1d layer.
 
         Args:
         - v (torch.Tensor): The scaling parameter for quantization.
         - min_scale (torch.nn.Parameter or torch.Tensor): The minimum scale for min-max tuning.
         - max_scale (torch.nn.Parameter or torch.Tensor): The maximum scale for min-max tuning.
 
@@ -270,44 +287,65 @@
             if not check_to_quantized(m):
                 unquantized_layers.append(n)
                 continue
             new_m = WrapperLinear(m, enable_minmax_tuning=enable_minmax_tuning)
             set_module(block, n, new_m)
             quantized_layers.append(n)
 
-        try:
-            import transformers
+        if isinstance(m, transformers.modeling_utils.Conv1D):
+            if not check_to_quantized(m):
+                unquantized_layers.append(n)
+                continue
+            new_m = WrapperTransformerConv1d(m, enable_minmax_tuning=enable_minmax_tuning)
+            set_module(block, n, new_m)
+            quantized_layers.append(n)
 
-            if isinstance(m, transformers.modeling_utils.Conv1D):
-                if not check_to_quantized(m):
-                    unquantized_layers.append(n)
-                    continue
-                new_m = WrapperTransformerConv1d(m, enable_minmax_tuning=enable_minmax_tuning)
-                set_module(block, n, new_m)
-                quantized_layers.append(n)
-        except:
-            pass
     return quantized_layers, unquantized_layers
 
 
 @torch.no_grad()
+def unwrapper_layer(model, layer, layer_name, v=0, min_scale=0, max_scale=0):
+    """Unwraps the WrapperLinear and WrapperTransformerConv1d modules in the given block.
+
+    Args:
+    block: The input block containing wrapped modules to be unwrapped.
+    vs: A dictionary of scaling parameters for the wrapped modules.
+    min_scales: A dictionary of minimum scaling values for the wrapped modules.
+    max_scales: A dictionary of maximum scaling values for the wrapped modules.
+    """
+
+    if hasattr(layer, "orig_layer"):
+
+        if isinstance(min_scale, torch.Tensor):
+            min_scale = torch.clamp(min_scale, -1, 0)
+            max_scale = torch.clamp(max_scale, -1, 0)
+
+        else:
+            min_scale = torch.tensor(0)
+            max_scale = torch.tensor(0)
+        orig_layer = layer.unwrapper(v, min_scale, max_scale)
+        orig_layer = orig_layer.to("cpu")
+        set_module(model, layer_name, orig_layer)
+
+
+@torch.no_grad()
 def unwrapper_block(block, vs, min_scales, max_scales):
     """Unwraps the WrapperLinear and WrapperTransformerConv1d modules in the given block.
 
     Args:
     block: The input block containing wrapped modules to be unwrapped.
     vs: A dictionary of scaling parameters for the wrapped modules.
     min_scales: A dictionary of minimum scaling values for the wrapped modules.
     max_scales: A dictionary of maximum scaling values for the wrapped modules.
     """
     for n, m in block.named_modules():
         if hasattr(m, "orig_layer"):
             v = 0
-            min_scale = 0
-            max_scale = 0
+            min_scale = torch.tensor(0)
+            max_scale = torch.tensor(0)
             if isinstance(vs, dict):
                 v = vs[n]
             if isinstance(min_scales, dict):
                 min_scale = min_scales[n]
                 min_scale = torch.clamp(min_scale, -1, 0)
             if isinstance(max_scales, dict):
                 max_scale = max_scales[n]
@@ -339,19 +377,17 @@
                    ...
                }
         enable_full_range (bool): Whether to enable full range quantization (default is False).
         batch_size (int): Batch size for training (default is 8).
         amp (bool): Whether to use automatic mixed precision (default is True).
         device: The device to be used for tuning (default is "auto").
         lr_scheduler: The learning rate scheduler to be used.
-        dataloader: The dataloader for input data (to be supported in future).
-        dataset_name (str): The default dataset name (default is "NeelNanda/pile-10k").
-        dataset_split (str): The split of the dataset to be used (default is "train").
-        use_quant_input (bool): Whether to use the output of the previous quantized block as the input for the current
-                                block (default is True).
+        dataset (str): The default dataset name (default is "NeelNanda/pile-10k").
+        enable_quanted_input (bool): Whether to use the output of the previous quantized block as
+                                the input for the current block (default is True).
         enable_minmax_tuning (bool): Whether to enable weight min-max tuning (default is True).
         lr (float): The learning rate (default is None, will be set to 1.0/iters).
         minmax_lr (float): The learning rate for min-max tuning (default is None, it will be set to lr automatically).
         low_gpu_mem_usage (bool): Whether to use low GPU memory (default is True).
         iters (int): Number of iterations (default is 200).
         seqlen (int): Data length of the sequence for tuning (default is 2048).
         n_samples (int): Number of samples (default is 512).
@@ -360,15 +396,14 @@
         n_blocks (int): Number of blocks (default is 1).
         gradient_accumulate_steps (int): Number of gradient accumulation steps (default is 1).
         not_use_best_mse (bool): Whether to use mean squared error (default is False).
         dynamic_max_gap (int): The dynamic maximum gap (default is -1).
         data_type (str): The data type to be used (default is "int").
         scale_dtype (str): The data type of quantization scale to be used (default is "float32"), different kernels
                            have different choices.
-        **kwargs: Additional keyword arguments.
 
     Returns:
         The quantized model.
     """
 
     def __init__(
         self,
@@ -379,97 +414,59 @@
         sym: bool = False,
         weight_config: dict = {},
         enable_full_range: bool = False,  ##for symmetric, TODO support later
         batch_size: int = 8,
         amp: bool = True,
         device=None,
         lr_scheduler=None,
-        dataloader=None,  ## to support later
-        dataset: str = "NeelNanda/pile-10k",
-        dataset_split: str = "train",
-        use_quant_input: bool = True,
+        dataset: Union[str, list, tuple, torch.utils.data.DataLoader] = "NeelNanda/pile-10k",
+        enable_quanted_input: bool = True,
         enable_minmax_tuning: bool = True,
         lr: float = None,
         minmax_lr: float = None,
         low_gpu_mem_usage: bool = True,
         iters: int = 200,
         seqlen: int = 2048,
         n_samples: int = 512,
         sampler: str = "rand",
         seed: int = 42,
         n_blocks: int = 1,
         gradient_accumulate_steps: int = 1,
         not_use_best_mse: bool = False,
         dynamic_max_gap: int = -1,
-        data_type: str = "int",  ##only support data_type
-        scale_dtype: str = "fp32",
+        data_type: str = "int",  ##only support int for now
+        scale_dtype: str = "fp16",
         **kwargs,
     ):
+        self.quantized = False
         self.model_orig_dtype = model.dtype
         self.model = model.eval().to("cpu")
         self.amp = amp
-        self.use_quant_input = use_quant_input
+        self.enable_quanted_input = enable_quanted_input
         self.enable_minmax_tuning = enable_minmax_tuning
         self.n_samples = n_samples
         self.n_blocks = n_blocks
         self.bits = bits
         self.group_size = group_size
         self.sym = sym
         self.low_gpu_mem_usage = low_gpu_mem_usage
         self.data_type = data_type
-        self.supported_types = [torch.nn.Linear]
-        try:
-            import transformers
-
-            self.supported_types.append(transformers.modeling_utils.Conv1D)
-        except:
-            pass
+        self.supported_types = [torch.nn.Linear, transformers.modeling_utils.Conv1D]
         self.weight_config = weight_config
-        self.dataset_split = dataset_split
         self.seed = seed
         self.tokenizer = tokenizer
         self.seqlen = seqlen
         self.train_bs = batch_size
         self.n_blocks = n_blocks
         self.device = detect_device(device)
-
-        if scale_dtype == "fp16" or scale_dtype == "float16":
-            self.scale_dtype = torch.float16
-        elif scale_dtype == "bf16" or scale_dtype == "bfloat16":
-            self.scale_dtype = torch.bfloat16
-        else:
-            self.scale_dtype = torch.float32
-
-        self.amp_dtype = torch.float16
-        if self.model.dtype != torch.float32:
-            self.amp_dtype = self.model.dtype
-        if self.device == "cpu":
-            self.amp_dtype = torch.bfloat16
-            self.amp_device_type = "cpu"
-
-        if "hpu" in self.device:
-            self.amp_dtype = torch.bfloat16
-
-            self.amp_device_type = "hpu"
-        if "cuda" in self.device:
-            self.amp_device_type = "cuda"
-
-        if self.amp:
-            if self.device == "cpu" and not CpuInfo().bf16:
-                self.amp = False
-                self.model = self.model.to(torch.float32)
-                logger.warning("amp is set to FALSE as the current" "device does not support the 'bf16' data type.")
-            else:
-                self.model = self.model.to(self.amp_dtype)
-        else:
-            self.model = self.model.to(torch.float32)
+        self.scale_dtype = convert_dtype_str2torch(scale_dtype)
+        self.set_amp_dtype()
+        self.cache_device = torch.device("cpu") if self.low_gpu_mem_usage else device
         logger.info(f"using {self.model.dtype} for quantization tuning")
-        self.dataset_name = dataset
-
-        self.dataloader = dataloader
+        self.dataset = dataset
         self.iters = iters
         if self.iters <= 0:
             logger.warning("iters must be positive, reset it to 200")
             self.iters = 200
         self.lr = lr
         if self.lr is None:
             self.lr = 1.0 / self.iters
@@ -478,134 +475,254 @@
             self.minmax_lr = self.lr
 
         self.sampler = sampler
         self.gradient_accumulate_steps = gradient_accumulate_steps
         self.not_use_best_mse = not_use_best_mse
         self.dynamic_max_gap = dynamic_max_gap
         self.enable_full_range = enable_full_range
-        assert self.enable_full_range is False, "only support enable_full_range=False currently"
         self.lr_scheduler = lr_scheduler
         self.set_layerwise_config(self.weight_config)
         self.optimizer = self.get_optimizer(None)
-        self.check_configs()
+        self.share_attention_mask_flag = None
+        self.hidden_dim_flag = None
         torch.set_printoptions(precision=3, sci_mode=True)
+
+        self.check_configs()
+        serialization_keys = [
+            "bits",
+            "group_size",
+            "sym",
+            "data_type",
+            "enable_quanted_input",
+            "enable_minmax_tuning",
+            "data_type",
+            "seqlen",
+            "train_bs",
+            "scale_dtype",
+            "lr",
+            "minmax_lr",
+            "gradient_accumulate_steps",
+            "iters",
+            "amp",
+            "n_samples",
+            "low_gpu_mem_usage",
+        ]
+        if isinstance(dataset, str):
+            serialization_keys.append("dataset")
+        self.serialization_dict = {}
+        for key in serialization_keys:
+            self.serialization_dict[key] = getattr(self, key)
+        from .version import __version__
+
+        self.serialization_dict["autoround_version"] = __version__
+        if "scale_dtype" in self.serialization_dict.keys():
+            self.serialization_dict["scale_dtype"] = str(self.serialization_dict["scale_dtype"])
         if is_optimum_habana_available():
             logger.info("Optimum Habana is available, import htcore explicitly.")
             import habana_frameworks.torch.core as htcore  # pylint: disable=E0401
             import habana_frameworks.torch.hpu as hthpu  # pylint: disable=E0401
 
-    def get_optimizer(self, optimizer):
-        """Returns the specified optimizer. In SignRound, we fix the optimizer.
+    def check_configs(self):
+        """Checks if the configurations are valid.
 
-        Args:
-        optimizer: The optimizer to be used.
+        Raises:
+        AssertionError: If any of the configurations are invalid.
+        """
+        assert isinstance(self.model, torch.nn.Module)
+        assert self.bits > 0, "bits must be positive"
+        assert self.group_size == -1 or self.group_size >= 1, "only supports positive group_size or -1(per channel)"
+        assert self.train_bs > 0, "batch size must be positive"
+        assert self.iters > 0, "iters must be positive"
+        assert self.seqlen > 0, "seqlen must be positive"
+        assert self.n_blocks > 0, "n_blocks must be positive"
+        assert self.gradient_accumulate_steps > 0, "gradient accumulate step must be positive"
+        assert self.enable_full_range is False, "only support enable_full_range=False currently"
+        # assert self.tokenizer != None or self.dataloader != None
+
+    def quantize(self):
+        """Quantize the model and return the quantized model along with weight configurations.
+        the entry of AutoRound.
 
         Returns:
-        The specified optimizer.
+        The quantized model and weight configurations.
         """
-        from auto_round.sign_sgd import SGD
+        # logger.info("cache block input")
+        block_names = get_block_names(self.model)
+        if len(block_names) == 0:
+            logger.warning("could not find blocks, exit with original model")
+            return self.model, self.weight_config
 
-        return SGD
+        if self.amp:
+            self.model = self.model.to(self.amp_dtype)
 
-    def get_scaler(self):
-        """Returns scaler, in SignRound, no need to use scaler."""
-        return None
+        layer_names = self.get_quantized_layer_names_outside_blocks()
+        self.start_time = time.time()
+        all_inputs = self.try_cache_inter_data_gpucpu([block_names[0]], self.n_samples, layer_names=layer_names)
+        del self.inputs
+        inputs = all_inputs[block_names[0]]
 
-    def scale_loss_and_backward(self, scaler, loss):
-        """Scales the loss and performs backward pass.
+        all_inputs.pop(block_names[0])
+        self.inputs = None
+        del self.inputs
+        if "input_ids" in inputs.keys():
+            total_samples = len(inputs["input_ids"])
+            self.n_samples = total_samples
+            if total_samples < self.train_bs:
+                self.train_bs = total_samples
+                logger.warning(f"force the train batch size to {total_samples} ")
+
+        self.model = self.model.to("cpu")
+        torch.cuda.empty_cache()
+        self.quant_blocks(
+            self.model,
+            inputs,
+            block_names,
+            n_blocks=self.n_blocks,
+            device=self.device,
+        )
+
+        self.quant_layers(layer_names, all_inputs)
+
+        self.dump_data_to_weight_config()
+
+        end_time = time.time()
+        cost_time = end_time - self.start_time
+        logger.info(f"quantization tuning time {cost_time}")
+
+        ## dump a summary
+        quantized_layers = []
+        unquantized_layers = []
+        for n, m in self.model.named_modules():
+            if isinstance(m, tuple(self.supported_types)):
+                if self.weight_config[n]["bits"] == 16:
+                    unquantized_layers.append(n)
+                else:
+                    quantized_layers.append(n)
+        summary_info = (
+            f"Summary: quantized {len(quantized_layers)}/{len(quantized_layers) + len(unquantized_layers)} in the model"
+        )
+        if len(unquantized_layers) > 0:
+            summary_info += f",  {unquantized_layers} have not been quantized"
+        logger.info(summary_info)
+
+        self.quantized = True
+        ##self.model = self.model.to(self.model_orig_dtype)##keep it as amp dtype
+        return self.model, self.weight_config
 
+    def dump_data_to_weight_config(self):
+        """
+        dump quantization scale and zp to  weight configuration
         Args:
-        scaler: The scaler to be used.
-        loss: The loss to be scaled.
 
         Returns:
-        The scaled loss.
+            None
         """
-        scale_loss = loss * 1000
-        scale_loss.backward()
-        if is_optimum_habana_available():
-            htcore.mark_step()
-        return scale_loss
+        for n, m in self.model.named_modules():
+            if n not in self.weight_config.keys():
+                continue
+            if hasattr(m, "scale"):
+                self.weight_config[n]["scale"] = m.scale
+                self.weight_config[n]["zp"] = m.zp
+                if self.group_size <= 0:
+                    self.weight_config[n]["g_idx"] = torch.tensor(
+                        [0 for i in range(m.weight.shape[1])], dtype=torch.int32, device="cpu"
+                    )
+                else:
+                    self.weight_config[n]["g_idx"] = torch.tensor(
+                        [i // self.group_size for i in range(m.weight.shape[1])], dtype=torch.int32, device="cpu"
+                    )
+                delattr(m, "scale")
+                delattr(m, "zp")
+            else:
+                self.weight_config[n]["data_type"] = "float"
+                if self.amp_dtype == torch.bfloat16:
+                    self.weight_config[n]["data_type"] = "bfloat"
+                self.weight_config[n]["bits"] = 16
+                self.weight_config[n]["group_size"] = None
+                self.weight_config[n]["sym"] = None
 
-    def step(self, scaler, optimizer, lr_schedule):
-        """Performs a step in the optimization process.
+    def quant_layers(self, layer_names, layer_inputs):
+        """Quantizes specified layers based on inputs and configuration.
 
         Args:
-        scaler: The scaler to be used.
-        optimizer: The optimizer for the step.
-        lr_schedule: The learning rate schedule.
+            layer_names (list): List of layer names to quantize.
+            layer_inputs (dict): Dictionary mapping layer names to input data.
 
         Returns:
-        None
+            None
         """
-        optimizer.step()
-        # for hpu
-        if is_optimum_habana_available():
-            htcore.mark_step()
-        optimizer.zero_grad()
-        lr_schedule.step()
-
-    def check_configs(self):
-        """Checks if the configurations are valid.
+        ##TODO currently we take all the layers outside blocks as post block layers which is not optimal
+        if len(layer_names) == 0:
+            return
+        q_layer_inputs = None
+        if self.enable_quanted_input:
+            q_layer_inputs = self.try_cache_inter_data_gpucpu([], self.n_samples, layer_names=layer_names)
 
-        Raises:
-        AssertionError: If any of the configurations are invalid.
-        """
-        assert isinstance(self.model, torch.nn.Module)
-        assert self.bits > 0, "bits must be positive"
-        assert self.group_size == -1 or self.group_size >= 1, "only supports positive group_size or -1(per channel)"
-        assert self.train_bs > 0, "batch size must be positive"
-        assert self.iters > 0, "iters must be positive"
-        assert self.seqlen > 0, "seqlen must be positive"
-        assert self.n_blocks > 0, "n_blocks must be positive"
-        assert self.gradient_accumulate_steps > 0, "gradient accumulate step must be positive"
-        # assert self.tokenizer != None or self.dataloader != None
+        self.model = self.model.to("cpu")
+        torch.cuda.empty_cache()
+        for layer_name in layer_names:
+            layer_input = layer_inputs[layer_name]
+            layer_input = to_device(layer_input, self.cache_device)
+            q_layer_input = q_layer_inputs[layer_name] if self.enable_quanted_input else None
+            q_layer_input = to_device(q_layer_input, self.cache_device)
+            self.quant_layer(layer_name, layer_input, q_layer_input, device=self.device)
+            for i in range(len(layer_input)):
+                layer_input[i] = None
+                if q_layer_input is not None:
+                    q_layer_input[i] = None
+            torch.cuda.empty_cache()
 
     def set_layerwise_config(self, weight_config):
         """Sets the layer-wise configuration based on the provided weight_config.
+           By default, only quantize layers in blocks.
 
         Args:
         weight_config: The weight configuration.
 
         Returns:
         None
         """
+        layers_in_blocks = self.get_layer_names_in_block()
         for n, m in self.model.named_modules():
-            is_supported_type = False
-            for supported_type in self.supported_types:
-                if isinstance(m, supported_type):
-                    is_supported_type = True
-                    break
-            if not is_supported_type:
+            if not isinstance(m, tuple(self.supported_types)):
                 continue
-            if n not in weight_config.keys():
+            if n not in weight_config.keys() and n in layers_in_blocks:
                 weight_config[n] = {}
                 weight_config[n]["data_type"] = self.data_type
                 weight_config[n]["bits"] = self.bits
                 weight_config[n]["group_size"] = self.group_size
                 weight_config[n]["sym"] = self.sym
-            else:
+                weight_config[n]["scale_dtype"] = self.scale_dtype
+            elif n in weight_config.keys():
                 if "data_type" not in weight_config[n].keys():
                     weight_config[n]["data_type"] = self.data_type
                 if "bits" not in weight_config[n].keys():
                     weight_config[n]["bits"] = self.bits
                 if "group_size" not in weight_config[n].keys():
                     weight_config[n]["group_size"] = self.group_size
                 if "sym" not in weight_config[n].keys():
                     weight_config[n]["sym"] = self.sym
-            weight_config[n]["scale_dtype"] = self.scale_dtype
+                if "scale_dtype" not in weight_config[n].keys():
+                    weight_config[n]["scale_dtype"] = self.scale_dtype
+            else:
+                weight_config[n] = {}
+                weight_config[n]["data_type"] = "float"
+                weight_config[n]["bits"] = 16
+                weight_config[n]["group_size"] = self.group_size
+                weight_config[n]["sym"] = self.sym
+                weight_config[n]["scale_dtype"] = self.scale_dtype
 
             m.data_type = weight_config[n]["data_type"]
             m.bits = weight_config[n]["bits"]
             m.group_size = weight_config[n]["group_size"]
             m.sym = weight_config[n]["sym"]
             m.scale_dtype = weight_config[n]["scale_dtype"]
 
     @torch.no_grad()
-    def get_block_outputs(self, block, input_ids, input_others, bs, device, cache_device, batch_dim):
+    def get_block_outputs(self, block, input_ids, input_others, bs, device, cache_device):
         """Compute the output of a given block of the model for a given input.
 
         Args:
         block: The block of the model.
         input_ids: The input tensor containing tokenized input ids.
         input_others: A dictionary containing additional input data.
         bs: The batch size for computing the output.
@@ -614,218 +731,418 @@
         batch_dim: The batch dimension of the output tensor.
 
         Returns:
         The output tensor of the block.
         """
 
         output = []
-        share_attention_mask_flag = is_share_attention_mask_model(self.model)
         for i in range(0, self.n_samples, bs):
             end_index = min(self.n_samples, i + bs)
             indices = torch.arange(i, end_index).to(torch.long)
             tmp_input_ids, tmp_input_others = sampling_inputs(
-                input_ids, input_others, indices, self.seqlen, share_attention_mask_flag=share_attention_mask_flag
+                input_ids, input_others, indices, self.seqlen, self.share_attention_mask_flag, self.input_dim
             )
-            tmp_output = block_forward(
-                block, tmp_input_ids, tmp_input_others, self.amp, self.amp_dtype, self.amp_device_type, device
-            ).to(cache_device)
-            output.append(tmp_output)
-        output = torch.cat(output, dim=batch_dim)
+            tmp_output = block_forward(block, tmp_input_ids, tmp_input_others, self.amp, self.amp_dtype, device).to(
+                cache_device
+            )
+            output.extend(list(torch.split(tmp_output, 1, dim=self.input_dim)))
         torch.cuda.empty_cache()
+
         return output
 
     @torch.no_grad()
-    def calib(self, n_samples):
+    def calib(self, n_samples, bs):
         """Perform calibration for quantization.
 
         This method calibrates the model for quantization by processing a specified
         number of samples from the calibration dataset. It ensures that the data is
         properly formatted and feeds it to the model. If the number of samples processed
         is less than the specified number, it logs a warning. If no samples are processed,
         it logs an error and exits.
         Args:
             n_samples (int): The number of samples to use for calibration.
+            bs (int): The number of samples to use for calibration
         """
-        if self.dataloader is None:
-            from .calib_dataset import CALIB_DATASETS
 
-            get_dataloader = CALIB_DATASETS.get(self.dataset_name, CALIB_DATASETS["NeelNanda/pile-10k"])
+        if isinstance(self.dataset, str):
+            dataset = self.dataset.replace(" ", "")  ##remove all whitespaces
             self.dataloader = get_dataloader(
                 self.tokenizer,
                 self.seqlen,
-                seed=self.seed,
-                bs=self.train_bs,
-                split=self.dataset_split,
-                dataset_name=self.dataset_name,
+                dataset,
+                self.seed,
+                bs,
+                self.n_samples,
             )
-
-        self.start_time = time.time()
+        else:
+            self.dataloader = self.dataset
         total_cnt = 0
         for data in self.dataloader:
             if data is None:
                 continue
             if isinstance(data, torch.Tensor):
-                data_new = data.to(self.model.device)
-                input_ids = data_new
+                input_ids = data.to(self.model.device)
+                data_new = input_ids
+
+            elif isinstance(data, str):
+                if self.tokenizer is None:
+                    logger.error("please provide tokenizer for string input")
+                    exit()
+                data = self.tokenizer(data, truncation=True, max_length=self.seqlen, return_tensors="pt").data
+                data_new = {}
+                for key in data.keys():
+                    data_new[key] = data[key].to(self.model.device)
+                input_ids = data_new["input_ids"]
             else:
                 data_new = {}
                 for key in data.keys():
                     data_new[key] = data[key].to(self.model.device)
                 input_ids = data_new["input_ids"]
-            # if input_ids.shape[-1] < self.seqlen:
-            #     continue
-            if total_cnt + input_ids.shape[0] > n_samples:
-                input_ids = input_ids[: n_samples - total_cnt, ...]
+            if input_ids.shape[-1] < self.seqlen:
+                continue
+
             try:
                 if isinstance(data_new, torch.Tensor):
                     self.model(data_new)
-                elif isinstance(data_new, dict):
+                else:
                     self.model(**data_new)
             except NotImplementedError:
                 pass
             except Exception as error:
                 logger.error(error)
             total_cnt += input_ids.shape[0]
             if total_cnt >= n_samples:
                 break
         if total_cnt == 0:
             logger.error(
                 f"no data has been cached, please provide more data with sequence length >={self.seqlen} in the "
-                f"dataloader or decease the sequence length"
+                f"dataset or decease the sequence length"
             )
             exit()
         elif total_cnt < n_samples:
             logger.warning(
                 f"Insufficient number of samples collected may affect the quantification. "
-                f"Effective samples size:{total_cnt}, Target sample size:{n_samples}"
+                f"Valid samples size:{total_cnt}, Target sample size:{n_samples}"
             )
 
     @torch.no_grad()
-    def cache_block_input(self, block_name, n_samples):
-        """Save the inputs of the first block for calibration.
+    def try_cache_inter_data_gpucpu(self, block_names, n_samples, layer_names=[], last_cache_name=None):
+        """Attempts to cache intermediate data on GPU，if failed, then using CPU.
+
+        Args:
+            block_names (list): List of block names to cache data for.
+            n_samples (int): Number of samples to use for caching.
+            layer_names (list, optional): List of layer names to cache data for. Defaults to [].
+            last_cache_name (str, optional): Name of the last cache. Defaults to None.
+
+        Returns:
+            all_inputs: Cached intermediate data.
+
+        Raises:
+            Exception: If caching on GPU fails, switches to CPU and caches there.
+        """
+        try:
+            self.model = self.model.to(self.device)
+            all_inputs = self.cache_inter_data(
+                block_names, n_samples, layer_names=layer_names, last_cache_name=last_cache_name
+            )
+            self.model = self.model.to("cpu")
+            torch.cuda.empty_cache()
+        except:
+            logger.info("switch to cpu to cache inputs")
+            self.model = self.model.to("cpu")
+            torch.cuda.empty_cache()
+            all_inputs = self.cache_inter_data(
+                block_names, n_samples, layer_names=layer_names, last_cache_name=last_cache_name
+            )
+        return all_inputs
+
+    @torch.no_grad()
+    def cache_inter_data(self, block_names, n_samples, layer_names=[], last_cache_name=None):
+        """Save the inputs of block_name for calibration. For layers, we cache both of inputs and output.
 
         This method temporarily replaces the forward method of the model to capture
         the inputs passing through the specified block. It then calibrates the model
         using a specified number of samples. Finally, it restores the original forward
         method and returns the inputs for the specified block.
         Args:
-            block_name (str): The name of the block for which inputs are to be saved.
+            block_names (list): The names of the blocks for which inputs are to be saved.
+            layer_names (list):The names of the layers for which inputs are to be saved.
             n_samples (int): The number of samples to use for calibration.
+            last_cache_name (str, optional): The name of the last layer to be cached,
+                                       we could break the forward in this layer to save time
+
         Returns:
             dict: A dictionary containing the inputs for the specified block.
         """
         self.inputs = {}
-        self.tmp_block_name = block_name
+        self.to_cached_layers = block_names + layer_names
+        tmp_dtype = None
+        ## have bug if block name is not the first block
+        if (len(block_names) > 1 or len(layer_names) > 0) and self.low_gpu_mem_usage:
+            tmp_dtype = self.model.dtype
+            self.model = self.model.to(torch.bfloat16) if self.amp else self.model.to(torch.float32)
+
+        self.last_cache_name = last_cache_name
+        if last_cache_name is None and len(block_names) + len(layer_names) == 1:
+            self.last_cache_name = block_names[0] if len(block_names) == 1 else layer_names[0]
+        calib_bs = self.train_bs
+        self.hook_handles = []
         self._replace_forward()
-        self.calib(n_samples)
+        self.calib(n_samples, calib_bs)
         self._recover_forward()
-        res = self.inputs[self.tmp_block_name]
-        del self.tmp_block_name
+        res = self.inputs
+        del self.last_cache_name
+        del self.to_cached_layers
+        if tmp_dtype is not None:
+            self.model = self.model.to(tmp_dtype)
+
         return res
 
     @torch.no_grad()
-    def get_forward_func(self, name):
+    def get_block_forward_func(self, name):
         """Gets the forward function.
 
         Args:
             name (str): The name of the function.
         Returns:
             function: The forward function.
         """
 
-        def forward(_, hidden_states, *positional_args, **kwargs):
-            dim = int((hasattr(self.model, "config") and "chatglm" in self.model.config.model_type))
-            share_attention_mask_flag = is_share_attention_mask_model(self.model)
+        def forward(m, hidden_states, *positional_args, **kwargs):
+            """Rewrite forward function, process and collect input data.
+
+            Args:
+                hidden_states (torch.Tensor): The hidden states tensor.
+                *positional_args: Variable number of positional arguments.
+                **kwargs: Variable number of keyword arguments.
+
+            Returns:
+                NotImplementedError: Getting the first layer inputs and then raise the error to save runtime.
+            """
+            if self.share_attention_mask_flag is None:
+                self.input_dim = check_hidden_state_dim(self.model, positional_args)
+                self.share_attention_mask_flag = check_share_attention_mask(self.model, hidden_states, **kwargs)
             if name in self.inputs:
-                data = torch.cat([self.inputs[name]["input_ids"], hidden_states.to("cpu")], dim=dim)
-                self.inputs[name]["input_ids"] = data
+                self.inputs[name]["input_ids"].extend(list(torch.split(hidden_states.to("cpu"), 1, dim=self.input_dim)))
             else:
                 self.inputs[name] = {}
-                self.inputs[name]["input_ids"] = hidden_states.to("cpu")
+                self.inputs[name]["input_ids"] = list(torch.split(hidden_states.to("cpu"), 1, dim=self.input_dim))
 
             if "positional_inputs" not in self.inputs[name]:
                 self.inputs[name]["positional_inputs"] = []
             for idx, item in enumerate(positional_args):
-                self.inputs[name]["positional_inputs"] = move_input_to_device(positional_args)
+                self.inputs[name]["positional_inputs"] = to_device(positional_args)
 
             for key in kwargs.keys():
-                if isinstance(kwargs[key], torch.Tensor) or isinstance(kwargs[key], list) or (key == "alibi"):
+                if isinstance(kwargs[key], torch.Tensor) or isinstance(kwargs[key], list) \
+                        or (key == "alibi") or (key == "attention_mask"):
                     if "attention_mask" in key:
                         if key not in self.inputs[name].keys():
                             self.inputs[name][key] = None
-                        if (not share_attention_mask_flag) and kwargs[key] is not None:
-                            if self.inputs[name][key] is not None:
-                                self.inputs[name][key] = torch.cat(
-                                    [self.inputs[name][key], kwargs[key].to("cpu")], dim=0
-                                )
+                        if kwargs[key] is not None:
+                            if (not self.share_attention_mask_flag) and self.inputs[name][key] is not None:
+                                self.inputs[name][key].extend(list(torch.split(kwargs[key].to("cpu"), 1, dim=0)))
                             else:
-                                self.inputs[name][key] = kwargs[key].to("cpu")
+                                self.inputs[name][key] = list(torch.split(kwargs[key].to("cpu"), 1, dim=0))
                     elif "alibi" in key:
                         if key not in self.inputs[name].keys():
                             self.inputs[name][key] = None
                         if isinstance(kwargs[key], torch.Tensor):
                             alibi = kwargs[key]
                             batch = kwargs["attention_mask"].shape[0]
                             alibi = alibi.reshape(batch, -1, alibi.shape[1], alibi.shape[2])
-                            if (not share_attention_mask_flag) and self.inputs[name][key] is not None:
-                                self.inputs[name][key] = torch.cat([self.inputs[name][key], alibi.to("cpu")], dim=0)
+                            if (not self.share_attention_mask_flag) and self.inputs[name][key] is not None:
+                                self.inputs[name][key].extend(list(torch.split(alibi.to("cpu"), 1, dim=0)))
                             else:
-                                self.inputs[name][key] = alibi.to("cpu")
+                                self.inputs[name][key] = list(torch.split(alibi.to("cpu"), 1, dim=0))
                     elif key not in self.inputs[name].keys():
-                        self.inputs[name][key] = move_input_to_device(kwargs[key], device=torch.device("cpu"))
-            raise NotImplementedError
+                        self.inputs[name][key] = to_device(kwargs[key], device=torch.device("cpu"))
+            if name == self.last_cache_name:
+                raise NotImplementedError
+            else:
+                return m.orig_forward(hidden_states, *positional_args, **kwargs)
 
         return forward
 
+    @torch.no_grad()
+    def _get_cache_data_hook_for_layer(self, name):
+        """A forward hook to save input max of a module
+        :param name: the module name
+        :return: A hook function."""
+
+        def cache_input_hook(module, inputs, outputs):
+            input = inputs
+            if isinstance(inputs, tuple) or isinstance(input, list):
+                input = inputs[0]
+            if name in self.inputs:
+                self.inputs[name].extend(list(torch.split(input.to("cpu"), 1, dim=0)))
+            else:
+                self.inputs[name] = list(torch.split(input.to("cpu"), 1, dim=0))
+
+        return cache_input_hook
+
     def _recover_forward(self):
         """Recovers the forward function."""
         for n, m in self.model.named_modules():
-            if n == self.tmp_block_name:
+            if hasattr(m, "orig_forward"):
                 m.forward = m.orig_forward
                 delattr(m, "orig_forward")
-                break
+        for hook_handle in self.hook_handles:
+            hook_handle.remove()
+        self.hook_handles = []
 
     def _replace_forward(self):
         """Replaces the forward function."""
         from functools import partial
 
         for n, m in self.model.named_modules():
-            if n == self.tmp_block_name:
+            if n in self.to_cached_layers and not isinstance(m, tuple(self.supported_types)):  ##block
                 m.orig_forward = m.forward
-                m.forward = partial(self.get_forward_func(n), m)
-                break
+                m.forward = partial(self.get_block_forward_func(n), m)
+            elif n in self.to_cached_layers:  ##linear layer or conv1d layer
+                hook_func = self._get_cache_data_hook_for_layer(n)
+                hook_handle = m.register_forward_hook(hook_func)
+                self.hook_handles.append(hook_handle)
+
+    def quant_layer(self, layer_name, inputs, q_inputs=None, device=torch.device("cpu")):
+        """Quantize a specific layer of the model using the provided inputs.
+
+        Args:
+            layer_name (str): The name of the layer to quantize.
+            inputs (torch.Tensor): Input data for quantization.
+            q_inputs (torch.Tensor, optional): Quantized input data. Defaults to None.
+            device (torch.device, optional): The device to use for quantization. Defaults to torch.device("cpu").
+
+        Returns:
+            None
+        """
+        logger.info(f"quantizing layer {layer_name}")
+        layer = get_module(self.model, layer_name)
+        layer = layer.to(device)
+        for i in range(len(inputs)):
+            inputs[i] = inputs[i].to(layer.weight.dtype)
+            if q_inputs is not None:
+                q_inputs[i] = q_inputs[i].to(layer.weight.dtype)
+
+        wrapper_linear = WrapperLinear(layer, self.enable_minmax_tuning).to(device)
+        round_params = []
+        minmax_params = []
+        round_params.append(wrapper_linear.value)
+        minmax_params.append(wrapper_linear.min_scale)
+        minmax_params.append(wrapper_linear.max_scale)
+        if self.enable_minmax_tuning:
+            optimizer = self.optimizer(
+                [{"params": round_params}, {"params": minmax_params, "lr": self.minmax_lr}], lr=self.lr, weight_decay=0
+            )
+        else:
+            optimizer = self.optimizer(round_params, lr=self.lr, weight_decay=0)
+
+        if self.lr_scheduler is None:
+            lr_schedule = torch.optim.lr_scheduler.LinearLR(
+                optimizer, start_factor=1.0, end_factor=0.0, total_iters=self.iters, verbose=False
+            )
+        else:
+            lr_schedule = copy.deepcopy(self.lr_scheduler)
+        n_samples = len(inputs)
+        last_best_iter = 0
+        best_loss = torch.finfo(torch.float).max
+        mse_loss = torch.nn.MSELoss().to(device)
+        scaler = self.get_scaler()  # pylint: disable=assignment-from-none
+        init_loss = None
+        best_v, best_min_scale, best_max_scale = torch.tensor(0), torch.tensor(0), torch.tensor(0)
+        gradient_accumulate_steps = self.train_bs  ##Force to low gpu
+        train_bs = 1  ##Force to low gpu
+        pick_samples = train_bs * gradient_accumulate_steps
+
+        if self.sampler != "rand":
+            whole_indices = torch.randperm(n_samples)[:pick_samples]
+        for i in range(self.iters):
+            total_loss = 0
+            if self.sampler == "rand":
+                whole_indices = torch.randperm(n_samples)[:pick_samples]
+            for tmp_step in range(gradient_accumulate_steps):
+                org_input = None
+                indices = whole_indices[tmp_step * train_bs : (tmp_step + 1) * train_bs]
+                if q_inputs is not None:
+                    current_input = [q_inputs[i] for i in indices]
+                    current_input = torch.cat(current_input, dim=0).to(device)
+                    org_input = [inputs[i] for i in indices]
+                    org_input = torch.cat(org_input, dim=0).to(device)
+                else:
+                    current_input = [inputs[i] for i in indices]
+                    current_input = torch.cat(current_input, dim=0).to(device)
+                    org_input = current_input
+                with torch.no_grad():
+                    current_output = layer(org_input)
+
+                if self.amp:
+                    with autocast(device_type=device.split(":")[0], dtype=self.amp_dtype):
+                        output_q = wrapper_linear(current_input)  # pylint: disable=not-callable
+                        loss = mse_loss(output_q, current_output)  # pylint: disable=not-callable
+                else:
+                    output_q = wrapper_linear(current_input)  # pylint: disable=not-callable
+                    loss = mse_loss(  # pylint: disable=not-callable
+                        output_q.to(torch.float32), current_output.to(torch.float32)
+                    )
+                total_loss += loss.item() / gradient_accumulate_steps
+
+                self.scale_loss_and_backward(scaler, loss)
+            if i == 0:
+                init_loss = total_loss
+
+            if total_loss < best_loss:
+                best_loss = total_loss
+                if not self.not_use_best_mse:
+                    best_v = copy.deepcopy(wrapper_linear.value.data)
+                    best_min_scale = copy.deepcopy(torch.clamp(wrapper_linear.min_scale.data, -1, 0))
+                    best_max_scale = copy.deepcopy(torch.clamp(wrapper_linear.max_scale.data, -1, 0))
+
+                    last_best_iter = i
+            if self.not_use_best_mse and i == self.iters - 1:
+                best_v = copy.deepcopy(wrapper_linear.value.data)
+                best_min_scale = copy.deepcopy(torch.clamp(wrapper_linear.min_scale.data, -1, 0))
+                best_max_scale = copy.deepcopy(torch.clamp(wrapper_linear.max_scale.data, -1, 0))
+
+            if not self.not_use_best_mse:
+                if self.dynamic_max_gap > 0 and i - last_best_iter >= self.dynamic_max_gap:
+                    break
+            self.step(scaler, optimizer, lr_schedule)
+
+        last_loss = total_loss
+        best_iter = self.iters
+        if not self.not_use_best_mse:
+            last_loss = best_loss
+            best_iter = last_best_iter
+        with torch.no_grad():
+            unwrapper_layer(self.model, wrapper_linear, layer_name, best_v, best_min_scale, best_max_scale)
+        dump_info = f"quantized {layer_name},  loss iter 0: {init_loss:.6f} -> iter {best_iter}: {last_loss:.6f}"
+        logger.info(dump_info)
 
     def quant_block(self, block, input_ids, input_others, q_input=None, device=torch.device("cpu")):
         """Quantize the weights of a given block of the model.
 
         Args:
         block: The block of the model to be quantized.
         input_ids: The input tensor containing tokenized input ids.
         input_others: A dictionary containing additional input data.
         q_input: The quantized input tensor.
         device: The device for quantization.
 
         Returns:
-        Tuple: (q_outputs, output) if self.use_quant_input is True, else (None, output)
+        Tuple: (q_outputs, output) if self.enable_quanted_input is True, else (None, output)
         """
-        from torch.amp import autocast
 
-        share_attention_mask_flag = is_share_attention_mask_model(self.model)
-        batch_dim = get_batch_dim(input_others)
-        if not self.low_gpu_mem_usage and input_ids.device != device:
-            input_ids = move_input_to_device(input_ids, device)
-            input_others = move_input_to_device(input_others, device)
-        cache_device = device
-        if self.low_gpu_mem_usage:
-            cache_device = "cpu"
-        output = self.get_block_outputs(block, input_ids, input_others, self.train_bs, device, cache_device, batch_dim)
+        output = self.get_block_outputs(block, input_ids, input_others, self.train_bs, device, self.cache_device)
 
         if q_input is not None:
-            input_ids = q_input.to(cache_device)
-
+            for i in range(len(input_ids)):
+                input_ids[i] = None
+            input_ids = q_input
+        torch.cuda.empty_cache()
         quantized_layer_names, unquantized_layer_names = wrapper_block(block, self.enable_minmax_tuning)
 
         round_params = []
         minmax_params = []
         for n, m in block.named_modules():
             if hasattr(m, "orig_layer"):
                 round_params.append(m.value)
@@ -842,74 +1159,59 @@
         if self.lr_scheduler is None:
             lr_schedule = torch.optim.lr_scheduler.LinearLR(
                 optimizer, start_factor=1.0, end_factor=0.0, total_iters=self.iters, verbose=False
             )
         else:
             lr_schedule = copy.deepcopy(self.lr_scheduler)
 
-        pick_samples = self.train_bs
-        if len(input_ids.shape) == 3:
-            n_samples = input_ids.shape[batch_dim]
-        else:
-            n_samples = input_ids.shape[0] // self.seqlen
+        pick_samples = self.train_bs * self.gradient_accumulate_steps
+        n_samples = len(input_ids)
         if self.sampler != "rand":
-            indices = torch.randperm(n_samples)[:pick_samples]
+            whole_indices = torch.randperm(n_samples)[:pick_samples]
         last_best_iter = 0
         best_loss = torch.finfo(torch.float).max
         mse_loss = torch.nn.MSELoss().to(device)
         scaler = self.get_scaler()  # pylint: disable=assignment-from-none
         init_loss = None
+        best_v, best_min_scale, best_max_scale = torch.tensor(0), torch.tensor(0), torch.tensor(0)
         for i in range(self.iters):
-            if self.sampler == "rand":
-                indices = torch.randperm(n_samples)[:pick_samples]
-
             total_loss = 0
-            for _ in range(self.gradient_accumulate_steps):
+            if self.sampler == "rand":
+                whole_indices = torch.randperm(n_samples)[:pick_samples]
+            for tmp_step in range(self.gradient_accumulate_steps):
+                indices = whole_indices[tmp_step * self.train_bs : (tmp_step + 1) * self.train_bs]
                 current_input_ids, current_input_others = sampling_inputs(
                     input_ids,
                     input_others,
                     indices,
                     seqlen=self.seqlen,
-                    share_attention_mask_flag=share_attention_mask_flag,
+                    share_attention_mask_flag=self.share_attention_mask_flag,
+                    input_dim=self.input_dim,
                 )
-                if len(input_ids.shape) == 3:
-                    if batch_dim == 0:
-                        current_output = output[indices, :, :]
-                    elif batch_dim == 1:
-                        current_output = output[:, indices, :]
-                    else:
-                        current_output = output[:, :, indices]
-                else:
-                    current_output = output.view(n_samples, self.seqlen, -1)
-                    current_output = current_output[indices, :, :]
-                    current_output = current_output.reshape(-1, current_output.shape[-1])
-                current_output = move_input_to_device(current_output, device)
+
+                current_output = [output[i] for i in indices]
+                current_output = torch.cat(current_output, dim=self.input_dim)
+
+                current_output = to_device(current_output, device)
 
                 output_q = block_forward(
-                    block,
-                    current_input_ids,
-                    current_input_others,
-                    self.amp,
-                    self.amp_dtype,
-                    self.amp_device_type,
-                    device,
+                    block, current_input_ids, current_input_others, self.amp, self.amp_dtype, device
                 )
                 if self.amp and not check_is_cpu(device):
-                    with autocast(device_type=self.amp_device_type, dtype=self.amp_dtype):
+                    with autocast(device_type=device.split(":")[0], dtype=self.amp_dtype):
                         loss = mse_loss(output_q, current_output)  # pylint: disable=not-callable
                 else:
                     loss = mse_loss(  # pylint: disable=not-callable
                         output_q.to(torch.float32), current_output.to(torch.float32)
                     )
 
                 total_loss += loss.item() / self.gradient_accumulate_steps
-                if i == 0:
-                    init_loss = total_loss
-
                 self.scale_loss_and_backward(scaler, loss)
+            if i == 0:
+                init_loss = total_loss
 
             if total_loss < best_loss:
                 best_loss = total_loss
                 if not self.not_use_best_mse:
                     # print(f"get better result at iter {i}, the loss is {total_loss}", flush=True)
                     best_v = collect_round_v(block)
                     best_min_scale, best_max_scale = collect_minmax_scale(block)
@@ -931,27 +1233,34 @@
         dump_info = (
             f"quantized {len(quantized_layer_names)}/{(len(quantized_layer_names) + len(unquantized_layer_names))} "
             f"layers in the block, loss iter 0: {init_loss:.6f} -> iter {best_iter}: {last_loss:.6f}"
         )
         logger.info(dump_info)
         if len(unquantized_layer_names) != 0:
             logger.info(f"{unquantized_layer_names} have not been quantized")
+        with torch.no_grad():
+            unwrapper_block(block, best_v, best_min_scale, best_max_scale)
+        if self.enable_quanted_input:
 
-        unwrapper_block(block, best_v, best_min_scale, best_max_scale)
-        if self.use_quant_input:
             q_outputs = self.get_block_outputs(
-                block, input_ids, input_others, self.train_bs, device, cache_device, batch_dim
+                block, input_ids, input_others, self.train_bs, device, cache_device=self.cache_device
             )
+            for i in range(len(input_ids)):
+                input_ids[i] = None
+            torch.cuda.empty_cache()
 
             return q_outputs, output
 
         else:
+            for i in range(len(input_ids)):
+                input_ids[i] = None
+            torch.cuda.empty_cache()
             return None, output
 
-    def qdq_weight_round(
+    def quant_blocks(
         self,
         model: torch.nn.Module,
         inputs,
         block_names,
         n_blocks=1,
         device=torch.device("cpu"),
     ):
@@ -971,14 +1280,30 @@
         torch.cuda.empty_cache()
         for n, m in model.named_parameters():
             m.requires_grad_(False)
         input_ids = inputs["input_ids"]
         inputs.pop("input_ids", None)
         input_others = inputs
         torch.cuda.empty_cache()
+        input_ids = to_device(input_ids, self.cache_device)
+        input_others = to_device(input_others, self.cache_device)
+        ## as in calibration phase, we may use bf16 for calibration due to low_gpu_memory usage
+        tmp_dtype = self.amp_dtype if self.amp else torch.float32
+        for i in range(len(input_ids)):
+            input_ids[i] = input_ids[i].to(tmp_dtype)
+
+        for key in input_others.keys():
+            if isinstance(input_others[key], torch.Tensor) and (
+                input_others[key].dtype == torch.float16 or input_others[key].dtype == torch.bfloat16
+            ):
+                input_others[key] = input_others[key].to(tmp_dtype)
+            elif isinstance(input_others[key], list):
+                for i in range(len(input_others[key])):
+                    input_others[key][i].to(tmp_dtype)
+
         for i in range(0, len(block_names), n_blocks):
             if n_blocks == 1:
                 n = block_names[i]
                 logger.info(f"quantizing {i + 1}/{len(block_names)}, {n}")
                 m = get_module(model, n)
             else:
                 names = block_names[i : i + n_blocks]
@@ -991,135 +1316,183 @@
             q_input, input_ids = self.quant_block(
                 m,
                 input_ids,
                 input_others,
                 q_input=q_input,
                 device=device,
             )
-            m.to("cpu")
+            m = m.to("cpu")
             torch.cuda.empty_cache()
 
         del q_input
         del input_ids
         del input_others
         del inputs
 
         torch.cuda.empty_cache()
 
     def save_quantized(self, output_dir=None, format="auto_gptq", inplace=True, **kwargs):
+        """Save the quantized model to the specified output directory in the specified format.
+
+        Args:
+            output_dir (str, optional): The directory to save the quantized model. Defaults to None.
+            format (str, optional): The format in which to save the model. Defaults to "auto_gptq".
+            inplace (bool, optional): Whether to modify the model in place. Defaults to True.
+            **kwargs: Additional keyword arguments specific to the export format.
+
+        Returns:
+            object: The compressed model object.
+        """
         if not self.quantized:
             logger.warning("please run autoround.quantize first")
             return
         from auto_round.export import EXPORT_FORMAT
 
         if format not in EXPORT_FORMAT:
             logger.error(f"export format only supports {EXPORT_FORMAT.keys()}")
             exit()
         save_quantized_as_format = EXPORT_FORMAT.get(format)
-        compressed_model = save_quantized_as_format(
+        compressed_model = save_quantized_as_format(  ##TODO refine the code
             output_dir,
             model=self.model,
             weight_config=self.weight_config,
             inplace=inplace,
             bits=self.bits,
             group_size=self.group_size,
             sym=self.sym,
             iters=self.iters,
             lr=self.lr,
             minmax_lr=self.minmax_lr,
             enable_minmax_tuning=self.enable_minmax_tuning,
-            use_quant_input=self.use_quant_input,
+            enable_quanted_input=self.enable_quanted_input,
             scale_dtype=self.scale_dtype,
             tokenizer=self.tokenizer,
             supported_types=self.supported_types,
+            data_type=self.data_type,
+            serialization_dict=self.serialization_dict,
             **kwargs,
         )
         return compressed_model
 
-    def quantize(self):
-        """Quantize the model and return the quantized model along with weight configurations.
+    def get_layer_names_in_block(self): ##TODO consolidate with utils
+        """Retrieves the names of layers within each block of the model.
 
         Returns:
-        The quantized model and weight configurations.
+            list: A list of strings, where each string is the name of a layer
+                  within a block of the model.
         """
-        # logger.info("cache block input")
+        for n, m in self.model.named_modules():
+            if isinstance(m, tuple(self.supported_types)):
+                m.tmp_name = n
+        layers_in_block = []
         block_names = get_block_names(self.model)
-        if len(block_names) == 0:
-            logger.warning("could not find blocks, exit with original model")
-            return
-        if self.amp:
-            self.model = self.model.to(self.amp_dtype)
-        if not self.low_gpu_mem_usage:
-            self.model = self.model.to(self.device)
-        inputs = self.cache_block_input(block_names[0], self.n_samples)
-        del self.inputs
-        if "input_ids" in inputs.keys():
-            dim = int((hasattr(self.model, "config") and "chatglm" in self.model.config.model_type))
-            total_samples = inputs["input_ids"].shape[dim]
-            self.n_samples = total_samples
-            if total_samples < self.train_bs:
-                self.train_bs = total_samples
-                logger.warning(f"force the train batch size to {total_samples} ")
-        self.model = self.model.to("cpu")
-        torch.cuda.empty_cache()
-        self.qdq_weight_round(
-            self.model,
-            inputs,
-            block_names,
-            n_blocks=self.n_blocks,
-            device=self.device,
-        )
+        for block_name in block_names:
+            block = get_module(self.model, block_name)
+            for n, m in block.named_modules():
+                if hasattr(m, "tmp_name"):
+                    layers_in_block.append(m.tmp_name)
         for n, m in self.model.named_modules():
-            if n in self.weight_config.keys():
-                if hasattr(m, "scale"):
-                    self.weight_config[n]["scale"] = m.scale
-                    self.weight_config[n]["zp"] = m.zp
-                    if self.group_size <= 0:
-                        self.weight_config[n]["g_idx"] = torch.tensor(
-                            [0 for i in range(m.weight.shape[1])], dtype=torch.int32, device="cpu"
-                        )
-                    else:
-                        self.weight_config[n]["g_idx"] = torch.tensor(
-                            [i // self.group_size for i in range(m.weight.shape[1])], dtype=torch.int32, device="cpu"
-                        )
-                    delattr(m, "scale")
-                    delattr(m, "zp")
-                else:
-                    self.weight_config[n]["data_type"] = "float"
-                    if self.amp_dtype == torch.bfloat16:
-                        self.weight_config[n]["data_type"] = "bfloat"
-                    self.weight_config[n]["bits"] = 16
-                    self.weight_config[n]["group_size"] = None
-                    self.weight_config[n]["sym"] = None
+            if hasattr(m, "tmp_name"):
+                delattr(m, "tmp_name")
+        return layers_in_block
 
-        end_time = time.time()
-        cost_time = end_time - self.start_time
-        logger.info(f"quantization tuning time {cost_time}")
-        ## dump a summary
-        quantized_layers = []
-        unquantized_layers = []
-        for n, m in self.model.named_modules():
-            if isinstance(m, tuple(self.supported_types)):
-                if self.weight_config[n]["bits"] == 16:
-                    unquantized_layers.append(n)
-                else:
-                    quantized_layers.append(n)
-        summary_info = (
-            f"Summary: quantized {len(quantized_layers)}/{len(quantized_layers) + len(unquantized_layers)} in the model"
-        )
-        if len(unquantized_layers) > 0:
-            summary_info += f",  {unquantized_layers} have not been quantized"
+    def get_quantized_layer_names_outside_blocks(self):
+        """Gets the names of quantized layers outside blocks in the model.
 
-        logger.info(summary_info)
-        if len(unquantized_layers) > 0:
-            logger.info(f"Summary: {unquantized_layers} have not been quantized")
+        Returns:
+            list: List of layer names outside blocks.
+        """
+        if self.weight_config is None or len(self.weight_config) == 0:
+            return []
 
-        self.quantized = True
-        self.model = self.model.to(self.model_orig_dtype)
-        return self.model, self.weight_config
+        layer_names = []
+        all_layers_in_block = self.get_layer_names_in_block()
+
+        for key in self.weight_config.keys():
+            if key in all_layers_in_block:
+                continue
+            layer = get_module(self.model, key)
+            if layer is None:
+                logger.error(f"could not find layer {key} in the model, exit...")
+                exit()
+            if isinstance(layer, tuple(self.supported_types)) and check_to_quantized(self.weight_config[key]):
+                layer_names.append(key)
+
+        return layer_names
+
+    def set_amp_dtype(self):
+        self.amp_dtype = torch.float16
+        if self.model.dtype != torch.float32:
+            self.amp_dtype = self.model.dtype
+        if self.device == "cpu" or "hpu" in self.device:
+            self.amp_dtype = torch.bfloat16
+        if self.amp:
+            if self.device == "cpu" and not CpuInfo().bf16:
+                self.amp = False
+                self.amp_dtype = torch.float32
+                self.model = self.model.to(torch.float32)
+                logger.warning(
+                    f"amp is set to FALSE as the current {self.device} device does not support the 'bf16' data type."
+                )
+            else:
+                self.model = self.model.to(self.amp_dtype)
+        else:
+            self.amp_dtype = torch.float32
+            self.model = self.model.to(torch.float32)
+
+    def get_optimizer(self, optimizer):
+        """Returns the specified optimizer. In SignRound, we fix the optimizer.
+
+        Args:
+        optimizer: The optimizer to be used.
+
+        Returns:
+        The specified optimizer.
+        """
+        from auto_round.sign_sgd import SignSGD
+
+        return SignSGD
+
+    def get_scaler(self):
+        """Returns scaler, in SignRound, no need to use scaler."""
+        return None
+
+    def scale_loss_and_backward(self, scaler, loss):
+        """Scales the loss and performs backward pass.
+
+        Args:
+        scaler: The scaler to be used.
+        loss: The loss to be scaled.
+
+        Returns:
+        The scaled loss.
+        """
+        scale_loss = loss * 1000
+        scale_loss.backward()
+        if is_optimum_habana_available():
+            htcore.mark_step()
+        return scale_loss
+
+    def step(self, scaler, optimizer, lr_schedule):
+        """Performs a step in the optimization process.
+
+        Args:
+        scaler: The scaler to be used.
+        optimizer: The optimizer for the step.
+        lr_schedule: The learning rate schedule.
+
+        Returns:
+        None
+        """
+        optimizer.step()
+        # for hpu
+        if is_optimum_habana_available():
+            htcore.mark_step()
+        optimizer.zero_grad()
+        lr_schedule.step()
 
 
 class AutoOPTRound(AutoRound):
     """Class for automatic rounding-based quantization with optimizers like adamw of a PyTorch model.
 
     Args:
         model: The PyTorch model to be quantized.
@@ -1129,18 +1502,16 @@
         sym (bool): Whether sym to be used (default is False).
         weight_config (dict): Configuration for weight quantization (default is an empty dictionary).
         enable_full_range (bool): Whether to enable full range quantization (default is False).
         batch_size (int): Batch size for training (default is 8).
         amp (bool): Whether to use automatic mixed precision (default is True).
         device: The device to be used for training (default is "auto").
         lr_scheduler: The learning rate scheduler to be used.
-        dataloader: The dataloader for input data (to be supported in future).
-        dataset_name (str): The default dataset name (default is "NeelNanda/pile-10k").
-        dataset_split (str): The split of the dataset to be used (default is "train").
-        use_quant_input (bool): Whether to use quantized input data (default is True).
+        dataset: The default dataset name (default is "NeelNanda/pile-10k").
+        enable_quanted_input (bool): Whether to use quantized input data (default is True).
         enable_minmax_tuning (bool): Whether to enable min-max tuning (default is True).
         lr (float): The learning rate (default is 0.005).
         minmax_lr (float): The learning rate for min-max tuning (default is None).
         low_gpu_mem_usage (bool): Whether to use low GPU memory (default is True).
         iters (int): Number of iterations (default is 200).
         seqlen (int): Length of the sequence.
         n_samples (int): Number of samples (default is 512).
@@ -1149,15 +1520,14 @@
         n_blocks (int): Number of blocks (default is 1).
         gradient_accumulate_steps (int): Number of gradient accumulation steps (default is 1).
         not_use_best_mse (bool): Whether to use mean squared error (default is False).
         dynamic_max_gap (int): The dynamic maximum gap (default is -1).
         data_type (str): The data type to be used (default is "int").
         scale_dtype (str): The data type of quantization scale to be used (default is "float32"), different kernels
                            have different choices.
-        optimizer: string or object
         **kwargs: Additional keyword arguments.
 
     Returns:
         The quantized model.
     """
 
     def __init__(
@@ -1169,33 +1539,31 @@
         sym: bool = False,
         weight_config: dict = {},
         enable_full_range: bool = False,
         batch_size: int = 8,
         amp: bool = True,
         device="auto",
         lr_scheduler=None,
-        dataloader=None,
-        dataset: str = "NeelNanda/pile-10k",
-        dataset_split: str = "train",
-        use_quant_input: bool = True,
+        dataset: Union[str, list, tuple, torch.utils.data.DataLoader] = "NeelNanda/pile-10k",
+        enable_quanted_input: bool = True,
         enable_minmax_tuning: bool = True,
         lr: float = None,
         minmax_lr: float = None,
         low_gpu_mem_usage: bool = True,
         iters: int = 200,
         seqlen: int = 2048,
         n_samples: int = 512,
         sampler: str = "rand",
         seed: int = 42,
         n_blocks: int = 1,
         gradient_accumulate_steps: int = 1,
         not_use_best_mse: bool = False,
         dynamic_max_gap: int = -1,
         data_type: str = "int",
-        scale_dtype: str = "fp32",
+        scale_dtype: str = "fp16",
         optimizer="AdamW",
         **kwargs,
     ):
         super(AutoOPTRound, self).__init__(
             model,
             tokenizer,
             bits,
@@ -1203,18 +1571,16 @@
             sym,
             weight_config,
             enable_full_range,
             batch_size,
             amp,
             device,
             lr_scheduler,
-            dataloader,
             dataset,
-            dataset_split,
-            use_quant_input,
+            enable_quanted_input,
             enable_minmax_tuning,
             lr,
             minmax_lr,
             low_gpu_mem_usage,
             iters,
             seqlen,
             n_samples,
@@ -1238,15 +1604,15 @@
             optimizer = getattr(torch.optim, optimizer)
         else:
             optimizer = optimizer
         return optimizer
 
     def get_scaler(self):
         scaler = None
-        if self.amp and not check_is_cpu(self.device) and self.amp_device_type != "hpu":
+        if self.amp and not check_is_cpu(self.device):
             from torch.cuda.amp import GradScaler
 
             scaler = GradScaler(init_scale=1024, growth_interval=100000)
         return scaler
 
     def scale_loss_and_backward(self, scaler, loss):
         if scaler is not None:
@@ -1283,18 +1649,17 @@
         sym (str): Whether symmetric quantization to be used (default is False).
         weight_config (dict): Configuration for weight quantization (default is an empty dictionary).
         enable_full_range (bool): Whether to enable full range quantization (default is False).
         batch_size (int): Batch size for training (default is 8).
         amp (bool): Whether to use automatic mixed precision (default is True).
         device: The device to be used for training (default is "auto").
         lr_scheduler: The learning rate scheduler to be used.
-        dataloader: The dataloader for input data (to be supported in future).
-        dataset_name (str): The default dataset name (default is "NeelNanda/pile-10k").
-        dataset_split (str): The split of the dataset to be used (default is "train").
-        use_quant_input (bool): Whether to use quantized input data (default is True).
+        dataset (Union[str, list, tuple, torch.utils.data.DataLoader]):
+                The default dataset name (default is "NeelNanda/pile-10k").
+        enable_quanted_input (bool): Whether to use quantized input data (default is True).
         enable_minmax_tuning (bool): Whether to enable min-max tuning (default is True).
         lr (float): The learning rate (default is 0.005).
         minmax_lr (float): The learning rate for min-max tuning (default is None).
         low_gpu_mem_usage (bool): Whether to use low GPU memory (default is True).
         iters (int): Number of iterations (default is 200).
         seqlen (int): Length of the sequence.
         n_samples (int): Number of samples (default is 512).
@@ -1304,15 +1669,14 @@
         gradient_accumulate_steps (int): Number of gradient accumulation steps (default is 1).
         not_use_best_mse (bool): Whether to use mean squared error (default is False).
         dynamic_max_gap (int): The dynamic maximum gap (default is -1).
         data_type (str): The data type to be used (default is "int").
         optimizer: string or object
         scale_dtype (str): The data type of quantization scale to be used (default is "float32"), different kernels
                            have different choices.
-        **kwargs: Additional keyword arguments.
 
     Returns:
         The quantized model.
     """
 
     def __init__(
         self,
@@ -1323,33 +1687,31 @@
         sym: bool = False,
         weight_config: dict = {},
         enable_full_range: bool = False,
         batch_size: int = 8,
         amp: bool = True,
         device="auto",
         lr_scheduler=None,
-        dataloader=None,
-        dataset: str = "NeelNanda/pile-10k",
-        dataset_split: str = "train",
-        use_quant_input: bool = True,
+        dataset: Union[str, list, tuple, torch.utils.data.DataLoader] = "NeelNanda/pile-10k",
+        enable_quanted_input: bool = True,
         enable_minmax_tuning: bool = True,
         lr: float = None,
         minmax_lr: float = None,
         low_gpu_mem_usage: bool = True,
         iters: int = 200,
         seqlen: int = 2048,
         n_samples: int = 512,
         sampler: str = "rand",
         seed: int = 42,
         n_blocks: int = 1,
         gradient_accumulate_steps: int = 1,
         not_use_best_mse: bool = False,
         dynamic_max_gap: int = -1,
         data_type: str = "int",
-        scale_dtype: str = "fp32",
+        scale_dtype: str = "fp16",
         optimizer="AdamW",
         **kwargs,
     ):
         super(AutoAdamRound, self).__init__(
             model,
             tokenizer,
             bits,
@@ -1357,18 +1719,16 @@
             sym,
             weight_config,
             enable_full_range,
             batch_size,
             amp,
             device,
             lr_scheduler,
-            dataloader,
             dataset,
-            dataset_split,
-            use_quant_input,
+            enable_quanted_input,
             enable_minmax_tuning,
             lr,
             minmax_lr,
             low_gpu_mem_usage,
             iters,
             seqlen,
             n_samples,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `auto_round-0.11/auto_round/export/__init__.py` & `auto_round-0.2/auto_round/export/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,7 +11,10 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .register import EXPORT_FORMAT
 from .export_to_autogptq import save_quantized_as_autogptq
 from .export_to_itrex import save_quantized_as_itrex, QuantConfig
+from .export_to_autoround.export_to_autoround import save_quantized_as_autoround
+
+
```

### Comparing `auto_round-0.11/auto_round/export/export_to_autogptq.py` & `auto_round-0.2/auto_round/export/export_to_autogptq.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,28 +42,30 @@
 # SOFTWARE.
 import torch
 from safetensors.torch import save_file as safe_save
 
 from auto_round.export.register import register_format
 from auto_round.utils import check_to_quantized, get_block_names, get_module, logger
 
+from ..utils import convert_dtype_torch2str_hf
+
 
 @register_format("auto_gptq")
 def save_quantized_as_autogptq(output_dir, use_triton=True, inplace=True, **kwargs):
     """Export the model to autogptq format to easily leverage cuda kernel."""
     model = kwargs["model"]
     weight_config = kwargs["weight_config"]
     sym = kwargs["sym"]
     bits = kwargs["bits"]
     group_size = kwargs["group_size"]
     iters = kwargs["iters"]
     lr = kwargs["lr"]
     minmax_lr = kwargs["minmax_lr"]
     enable_minmax_tuning = kwargs["enable_minmax_tuning"]
-    use_quant_input = kwargs["use_quant_input"]
+    enable_quanted_input = kwargs["enable_quanted_input"]
     scale_dtype = kwargs["scale_dtype"]
     tokenizer = kwargs["tokenizer"]
     supported_types = kwargs["supported_types"]
 
     logger.info("Saving quantized model to autogptq format, this may take a while...")
     if tokenizer is not None:
         tokenizer.save_pretrained(output_dir)
@@ -80,15 +82,15 @@
                 break
         if not is_supported_type:
             continue
         if not check_to_quantized(m):
             all_to_quantized = False
         else:
             modules_in_block_to_quantize.append(n)
-    modules_in_block_to_quantize = [modules_in_block_to_quantize]  ##align with autogptq
+    modules_in_block_to_quantize = [modules_in_block_to_quantize]
     if all_to_quantized:
         modules_in_block_to_quantize = None
 
     if inplace:
         compressed_model = model.to("cpu")
     else:
         compressed_model = copy.deepcopy(model.to("cpu"))
@@ -96,36 +98,40 @@
     from auto_gptq.modeling._utils import pack_model
 
     if bits == 3 or use_triton is False:
         if bits == 3 and use_triton is True:
             logger.warning("triton does not support 3 bits, reset it to False")
         quantizers = {}
         for key in weight_config:
+            if key == "lm_head":  ##TODO remove this after pr 87 is merged
+                continue
             info = weight_config[key]
             if not check_to_quantized(info):
                 continue
-            quantizers[key] = (None, info["scale"], info["zp"], info["g_idx"])
+            ##force to float32 to be compatible with torch 2.0
+            quantizers[key] = (None, info["scale"], info["zp"].to(torch.float32), info["g_idx"])
         pack_model(
             compressed_model,
             quantizers,
             bits,
             group_size,
             use_cuda_fp16=True,
             desc_act=False,
             force_layer_back_to_cpu=True,
             use_triton=False,
         )
     else:
         quantizers = {}
         for key in weight_config:
+            if key == "lm_head":  ##TODO remove this after pr 87 is merged
+                continue
             info = weight_config[key]
             if not check_to_quantized(info):
                 continue
-            info["zp"] = info["zp"].to(torch.float32)
-            quantizers[key] = (None, info["scale"].to(torch.float32), info["zp"], info["g_idx"])
+            quantizers[key] = (None, info["scale"].to(torch.float32), info["zp"].to(torch.float32), info["g_idx"])
         pack_model(
             compressed_model,
             quantizers,
             bits,
             group_size,
             use_cuda_fp16=True,
             desc_act=False,
@@ -141,36 +147,36 @@
         bits=bits,
         group_size=group_size,
         sym=sym,
         iters=iters,
         lr=lr,
         minmax_lr=minmax_lr,
         enable_minmax_tuning=enable_minmax_tuning,
-        use_quant_input=use_quant_input,
+        enable_quanted_input=enable_quanted_input,
         scale_dtype=scale_dtype,
         use_safetensors=True,
         modules_in_block_to_quantize=modules_in_block_to_quantize,
     )
 
 
 def _save_quantized_to_autogptq(
-    model,
-    save_dir: str,
-    bits=4,
-    group_size=128,
-    sym=False,
-    iters=200,
-    lr=5e-3,
-    minmax_lr=5e-3,
-    enable_minmax_tuning=True,
-    use_quant_input=True,
-    use_safetensors: bool = True,
-    scale_dtype=torch.float32,
-    safetensors_metadata: Optional[Dict[str, str]] = None,
-    modules_in_block_to_quantize=None,
+        model,
+        save_dir: str,
+        bits=4,
+        group_size=128,
+        sym=False,
+        iters=200,
+        lr=5e-3,
+        minmax_lr=5e-3,
+        enable_minmax_tuning=True,
+        enable_quanted_input=True,
+        use_safetensors: bool = True,
+        scale_dtype=torch.float32,
+        safetensors_metadata: Optional[Dict[str, str]] = None,
+        modules_in_block_to_quantize=None,
 ):
     """Save quantized model and configs to local disk for cuda."""
     os.makedirs(save_dir, exist_ok=True)
     model.to("cpu")
 
     model_base_name = "model"
     if use_safetensors:
@@ -219,16 +225,16 @@
         safetensors_metadata["autoround_version"] = str(__version__)
         safetensors_metadata["bits"] = str(bits)
         safetensors_metadata["group_size"] = str(group_size)
         safetensors_metadata["iters"] = str(iters)
         safetensors_metadata["lr"] = str(lr)
         safetensors_metadata["minmax_lr"] = str(minmax_lr)
         safetensors_metadata["enable_minmax_tuning"] = str(enable_minmax_tuning)
-        safetensors_metadata["use_quant_input"] = str(use_quant_input)
-        safetensors_metadata["scale_dtype"] = str(scale_dtype)
+        safetensors_metadata["enable_quanted_input"] = str(enable_quanted_input)
+        safetensors_metadata["scale_dtype"] = convert_dtype_torch2str_hf(scale_dtype)
         safe_save(state_dict, join(save_dir, model_save_name), safetensors_metadata)
     else:
         model_save_name = model_base_name + ".bin"
         torch.save(model.state_dict(), join(save_dir, model_save_name))
 
     from auto_gptq.modeling._base import BaseQuantizeConfig
 
@@ -246,16 +252,16 @@
     config_dict = quantization_config.to_dict()
     config_dict["quant_method"] = "intel/auto-round"
     config_dict["autoround_version"] = __version__
     config_dict["iters"] = iters
     config_dict["lr"] = lr
     config_dict["minmax_lr"] = minmax_lr
     config_dict["enable_minmax_tuning"] = enable_minmax_tuning
-    config_dict["use_quant_input"] = use_quant_input
-    config_dict["scale_dtype"] = str(scale_dtype)
+    config_dict["enable_quanted_input"] = enable_quanted_input
+    config_dict["scale_dtype"] = convert_dtype_torch2str_hf(scale_dtype)
     if modules_in_block_to_quantize is not None:
         config_dict["modules_in_block_to_quantize"] = modules_in_block_to_quantize
 
     with open(join(save_dir, "quantize_config.json"), "w", encoding="utf-8") as f:
         json.dump(config_dict, f, indent=2)
 
     config_dict["quant_method"] = "gptq"  ##hf transformers could only recognize this value
```

### Comparing `auto_round-0.11/auto_round/export/export_to_itrex/__init__.py` & `auto_round-0.2/auto_round/export/export_to_itrex/__init__.py`

 * *Files identical despite different names*

### Comparing `auto_round-0.11/auto_round/export/export_to_itrex/config.py` & `auto_round-0.2/auto_round/export/export_to_itrex/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,68 +21,118 @@
 import os
 from dataclasses import dataclass, field
 from typing import Any, Dict, Tuple, Union
 
 import torch
 from transformers import PretrainedConfig
 
-from auto_round.utils import logger
+from auto_round.utils import convert_dtype_str2torch, convert_dtype_torch2str, logger
 
 QUANT_CONFIG = "quantize_config.json"
 
 
 class QuantConfig(PretrainedConfig):
-    """A brief quantization configuration for reference when performing model dequantization."""
+    """A brief quantization configuration for reference when performing model de-quantization."""
 
     def __init__(
         self,
         bits=4,
-        scale_dtype="torch.float32",
+        scale_dtype="fp32",
         group_size=128,
         sym=False,
         quant_method="autoround",
         model_name_or_path=None,
         model_file_base_name="model",
         enable_minmax_tuning=True,
         iters=1000,
         lr=0.001,
         minmax_lr=0.001,
-        use_quant_input=True,
+        enable_quanted_input=True,
+        compute_dtype=None,
         **kwargs,
     ):
         self.bits = bits
         self.group_size = group_size
-        self.scale_dtype = scale_dtype
+        self.scale_dtype = convert_dtype_torch2str(scale_dtype)
         self.sym = sym
         self.quant_method = quant_method
         self.model_name_or_path = model_name_or_path
         self.model_file_base_name = model_file_base_name
         self.enable_minmax_tuning = enable_minmax_tuning
         self.iters = iters
         self.lr = lr
         self.minmax_lr = minmax_lr
-        self.use_quant_input = use_quant_input
+        self.enable_quanted_input = enable_quanted_input
+        self.compute_dtype = convert_dtype_torch2str(compute_dtype)
 
-        ### Redundant parameters, will be removed later. ###
-        self.damp_percent = 0.01
-        self.desc_act = False
-        self.true_sequential = False
-        self.quant_method = "gptq"
+        if "export_to_xpu" not in kwargs or not kwargs["export_to_xpu"]:
+            ### Redundant parameters, will be removed later. ###
+            self.damp_percent = 0.01
+            self.desc_act = False
+            self.true_sequential = False
+            self.quant_method = "gptq"
+        else:
+            ### XPU special parameters. ###
+            self.weight_dtype = "int4_fullrange"  # Due to ipex format limitations. Actually, it's int4_clip.
 
     def post_init(self):
-        r"""
-        Safety checker that arguments are correct - also replaces some NoneType arguments with their default values.
-        """
+        r"""Safety checker for CPU that arguments are correct
+        also replaces some NoneType arguments with their default values."""
 
-        if self.scale_dtype not in ["torch.float32", "torch.float16", "torch.bfloat16"]:
+        if self.scale_dtype not in ["fp32", "fp16", "bf16"]:
             raise ValueError("scale_dtype must be 'fp32', 'fp16' or 'bf16'.")
 
         if self.group_size not in [-1, 32, 128]:
             raise ValueError("group_size must be an integer in [-1, 32, 128]")
 
+    def post_init_xpu(self):
+        r"""
+        Safety checker for XPU that arguments are correct
+        - also replaces some NoneType arguments with their default values.
+        """
+
+        if self.compute_dtype is not None and self.compute_dtype not in ["fp16"]:
+            raise ValueError("compute_dtype must be 'fp16'.")
+        elif self.compute_dtype is None:
+            self.compute_dtype = "fp16"
+
+        if self.bits is None:
+            self.bits = 4
+        elif self.bits not in [4]:
+            raise ValueError(f"Only support quantization to [4] bits but found {self.bits}")
+
+        if self.weight_dtype is None:
+            self.weight_dtype = "int4_fullrange"
+
+        elif self.weight_dtype not in [
+            "int4_fullrange",
+        ]:
+            raise ValueError(f"weight_dtype must be a string in 'int4_fullrange', but get {self.weight_dtype}.")
+
+        if self.scale_dtype is not None and self.scale_dtype not in ["fp16"]:
+            raise ValueError("scale_dtype must be a string in 'fp16'")
+        elif self.scale_dtype is None:
+            self.scale_dtype = "fp16"
+
+        # if not isinstance(self.use_double_quant, bool):
+        #     raise ValueError("use_double_quant must be a boolean")
+
+        # if self.use_double_quant and not isinstance(self.double_quant_dtype, str):
+        #     raise ValueError("double_quant_dtype must be a string")
+
+        # if self.use_double_quant and not isinstance(self.scale_dtype, str):
+        #     raise ValueError("scale_dtype must be a string")
+
+        if not isinstance(self.group_size, int):
+            raise ValueError("group_size must be a int")
+
+        if self.sym is not True:
+            raise ValueError("asym is not support, only support 'sym' now!")
+        self.use_neural_speed = False
+
     def quantization_method(self):
         r"""This method returns the quantization method used for the model."""
         return self.quant_method
 
     @classmethod
     def from_dict(cls, config_dict, return_unused_kwargs=False, **kwargs):
         """Instantiates a [`QuantConfig`] from a Python dictionary of parameters.
@@ -225,7 +275,29 @@
             )
 
     @classmethod
     def get_config_dict(
         cls, pretrained_model_name_or_path: Union[str, os.PathLike], **kwargs
     ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         return super().get_config_dict(pretrained_model_name_or_path, _configuration_file=QUANT_CONFIG, **kwargs)
+
+    def remove_redundant_parameters(self):
+        remove_parameters = [
+            "calib_dataloader",
+            "dataset",
+            "scheme",
+            "tokenizer",
+            "use_neural_speed",
+            "enable_quanted_input",
+            "layer_wise",
+            "nsamples",
+            "lr",
+            "minmax_lr",
+            "iters",
+            "enable_quanted_input",
+            "model_file_base_name",
+            "enable_minmax_tuning",
+            "model_name_or_path",
+        ]
+        for parameter in remove_parameters:
+            if hasattr(self, parameter):
+                delattr(self, parameter)
```

### Comparing `auto_round-0.11/auto_round/export/export_to_itrex/export.py` & `auto_round-0.2/auto_round/export/export_to_itrex/export.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import copy
 import json
 import os
 from os.path import isdir, isfile, join
 from typing import Dict, List, Optional, Union
 
 import torch
+import transformers
 from safetensors.torch import save_file as safe_save
 
 from auto_round.export.register import register_format
 from auto_round.utils import get_module, logger, quant_weight_w_scale, set_module
 
 from .config import QuantConfig
 from .model_wrapper import WeightOnlyLinear
@@ -36,33 +37,82 @@
     sym = kwargs["sym"]
     bits = kwargs["bits"]
     group_size = kwargs["group_size"]
     iters = kwargs["iters"]
     lr = kwargs["lr"]
     minmax_lr = kwargs["minmax_lr"]
     enable_minmax_tuning = kwargs["enable_minmax_tuning"]
-    use_quant_input = kwargs["use_quant_input"]
+    enable_quanted_input = kwargs["enable_quanted_input"]
     scale_dtype = kwargs["scale_dtype"]
     tokenizer = kwargs["tokenizer"]
 
     compressed_model = pack_model(model, weight_config, inplace=inplace)
     if output_dir is None:
         return compressed_model
     quantize_config = QuantConfig(
         bits=bits,
         group_size=group_size,
         sym=sym,
         iters=iters,
         lr=lr,
         minmax_lr=minmax_lr,
         enable_minmax_tuning=enable_minmax_tuning,
-        use_quant_input=use_quant_input,
-        scale_dtype=str(scale_dtype),
+        enable_quanted_input=enable_quanted_input,
+        scale_dtype=scale_dtype,
     )
     if quantize_config is not None:
+        quantize_config.post_init()
+        config = compressed_model.config
+        setattr(config, "quantization_config", quantize_config.to_dict())
+        config.save_pretrained(output_dir)
+        quantize_config.save_pretrained(output_dir)
+    try:
+        compressed_model.save_pretrained(output_dir, safe_serialization=True)
+        if tokenizer is not None:
+            tokenizer.save_pretrained(output_dir)
+        logger.info("Saved config file and weights of quantized model to {}.".format(output_dir))
+    except IOError as e:  # pragma: no cover
+        logger.error("Fail to save configure file and weights due to {}.".format(e))
+    return compressed_model
+
+
+@register_format("itrex_xpu")
+def save_quantized_as_itrex_xpu(output_dir, inplace=True, **kwargs):
+    """Save configure file and weights for CPU backend inference."""
+    model = kwargs["model"]
+    weight_config = kwargs["weight_config"]
+    sym = kwargs["sym"]
+    bits = kwargs["bits"]
+    group_size = kwargs["group_size"]
+    iters = kwargs["iters"]
+    lr = kwargs["lr"]
+    minmax_lr = kwargs["minmax_lr"]
+    enable_minmax_tuning = kwargs["enable_minmax_tuning"]
+    enable_quanted_input = kwargs["enable_quanted_input"]
+    scale_dtype = kwargs["scale_dtype"]
+    tokenizer = kwargs["tokenizer"]
+
+    compressed_model = pack_model(inplace=inplace, **kwargs)
+    if output_dir is None:
+        return compressed_model
+    quantize_config = QuantConfig(
+        bits=bits,
+        group_size=group_size,
+        sym=sym,
+        iters=iters,
+        lr=lr,
+        minmax_lr=minmax_lr,
+        enable_minmax_tuning=enable_minmax_tuning,
+        enable_quanted_input=enable_quanted_input,
+        scale_dtype=scale_dtype,
+        export_to_xpu=True,
+    )
+    if quantize_config is not None:
+        quantize_config.post_init_xpu()
+        quantize_config.remove_redundant_parameters()
         config = compressed_model.config
         setattr(config, "quantization_config", quantize_config.to_dict())
         config.save_pretrained(output_dir)
         quantize_config.save_pretrained(output_dir)
     try:
         compressed_model.save_pretrained(output_dir, safe_serialization=True)
         if tokenizer is not None:
@@ -78,14 +128,15 @@
     weight_config: Union[str, dict],
     enable_full_range=False,
     compression_dtype=torch.int32,
     compression_dim=1,
     device="cpu",
     use_optimum_format=True,
     inplace=False,
+    **kwargs,
 ):
     """Convert Linear to WeightOnlyLinear for low memory inference.
 
     Args:
         weight_config (str|dict): qconfig dict or Path of qconfig.json.
         enable_full_range (bool, optional): Whether to leverage the full compression range
                                             under symmetric quantization. Defaults to False.
@@ -97,14 +148,21 @@
         use_optimum_format (bool, optional): use the popular huggingface compression format.
             1: compression_dim: weight = 1, zeros = 0 and both are transposed.
             2: zeros -= 1 before compression. Why we need it?
             3: g_idx: use same number for one group instead of recording the channel order.
             4. parameter name changed, such as 'packed_weight' -> 'qweight'.
             5. zeros is always needed even for sym.
         inplace (bool, optional): Compress the model in place, or copy the model and compress it.
+
+    xpu args:
+        compression_dtype=torch.int8,
+        compression_dim=0,
+        use_optimum_format=False,
+        scale_dtype=convert_dtype_str2torch(config.scale_dtype),
+        device="xpu",
     """
     if inplace:
         compressed_model = model
     else:
         compressed_model = copy.deepcopy(model)
     if isinstance(weight_config, str):
         with open(weight_config, "r") as f:
@@ -123,31 +181,48 @@
         m = get_module(compressed_model, k)
         fp_weight = m.weight.data
         scale, zp = v["scale"], v["zp"]
         convert_dtype = scale_dtype
         if not isinstance(scale, torch.Tensor):
             scale = torch.tensor(scale, dtype=convert_dtype)
             zp = torch.tensor(zp, dtype=torch.int32)
+            if device == "xpu":
+                scale = torch.tensor(v["scale"], dtype=torch.float32)
+                zp = None if sym else torch.tensor(v["zp"], dtype=torch.int32)
         else:
             if not inplace:
                 scale = scale.clone()
                 zp = zp.clone()
-            scale = scale.to(dtype=convert_dtype)
-            zp = zp.to(dtype=torch.int32)
+            if device == "xpu":
+                # Please note that for XPU, the scale data type is forcibly set to fp32
+                scale = scale.to(dtype=torch.float32)
+                zp = None if sym else zp.to(dtype=torch.int32)
+            else:
+                scale = scale.to(dtype=convert_dtype)
+                zp = zp.to(dtype=torch.int32)
+        if isinstance(m, transformers.modeling_utils.Conv1D):
+            fp_weight = fp_weight.t_().contiguous()
         int_weight = quant_weight_w_scale(fp_weight, scale, zp, group_size, fp_weight.device)
+        if isinstance(m, torch.nn.Linear):
+            in_features = m.in_features
+            out_features = m.out_features
+        elif isinstance(m, transformers.modeling_utils.Conv1D):
+            in_features = m.weight.shape[0]
+            out_features = m.weight.shape[1]
         int_weight = int_weight.type(torch.int32)
         new_module = WeightOnlyLinear(
-            m.in_features,
-            m.out_features,
+            in_features,
+            out_features,
             num_bits,
             group_size,
             dtype=dtype,
             scale_dtype=scale_dtype,
             zp=zp is not None,
             bias=m.bias is not None,
-            device=device,
-            use_optimum_format=True,
+            device="cuda" if device == "xpu" else device,
+            compression_dtype=compression_dtype,
+            compression_dim=compression_dim,
+            use_optimum_format=use_optimum_format,  # xpu is False
         )
         new_module.pack(int_weight, scale, zp, m.bias)
         set_module(compressed_model, k, new_module)
-
     return compressed_model
```

### Comparing `auto_round-0.11/auto_round/export/export_to_itrex/model_wrapper.py` & `auto_round-0.2/auto_round/export/export_to_itrex/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `auto_round-0.11/auto_round/export/register.py` & `auto_round-0.2/auto_round/export/register.py`

 * *Files identical despite different names*

### Comparing `auto_round-0.11/auto_round/sign_sgd.py` & `auto_round-0.2/auto_round/sign_sgd.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 import torch
 from torch import Tensor
 from torch.optim.optimizer import Optimizer
 
-__all__ = ["SGD", "sgd"]
+__all__ = ["SignSGD", "sgd"]
 
 
 class _RequiredParameter(object):
     """Singleton class representing a required parameter for an Optimizer."""
 
     def __repr__(self):
         return "<required parameter>"
@@ -121,15 +121,15 @@
         finally:
             torch.set_grad_enabled(prev_grad)
         return ret
 
     return _use_grad
 
 
-class SGD(Optimizer):
+class SignSGD(Optimizer):
     r"""Implements stochastic gradient descent (optionally with momentum).
 
     .. math::
        \begin{aligned}
             &\rule{110mm}{0.4pt}                                                                 \\
             &\textbf{input}      : \gamma \text{ (lr)}, \: \theta_0 \text{ (params)}, \: f(\theta)
                 \text{ (objective)}, \: \lambda \text{ (weight decay)},                          \\
@@ -238,15 +238,15 @@
             nesterov=nesterov,
             maximize=maximize,
             foreach=foreach,
             differentiable=differentiable,
         )
         if nesterov and (momentum <= 0 or dampening != 0):
             raise ValueError("Nesterov momentum requires a momentum and zero dampening")
-        super(SGD, self).__init__(params, defaults)
+        super(SignSGD, self).__init__(params, defaults)
 
     def __setstate__(self, state):
         super().__setstate__(state)
         for group in self.param_groups:
             group.setdefault("nesterov", False)
             group.setdefault("maximize", False)
             group.setdefault("foreach", None)
```

### Comparing `auto_round-0.11/auto_round/utils.py` & `auto_round-0.2/auto_round/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,34 +9,36 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
-import importlib
 import logging
+import os
 import subprocess
 from collections import UserDict
 
 # for cpu usage
 import cpuinfo
+import numpy as np
 import psutil
 import torch
 from torch.amp import autocast
 
-SHARE_ATTENTION_MASK_LIST = ["Baichuan2-13B-Base", "Baichuan2-13B-Chat"]
-
 logger = logging.getLogger("autoround")
 logger.setLevel(logging.INFO)
+logger.propagate = False
 fh = logging.StreamHandler()
 fh_formatter = logging.Formatter("%(asctime)s %(levelname)s %(filename)s L%(lineno)d: %(message)s", "%Y-%m-%d %H:%M:%S")
 fh.setFormatter(fh_formatter)
 logger.addHandler(fh)
 
+import importlib
+import transformers
 
 class LazyImport(object):
     """Lazy import python module till use."""
 
     def __init__(self, module_name):
         """Init LazyImport object.
 
@@ -62,24 +64,24 @@
         function_name = self.module_name.split(".")[-1]
         module_name = self.module_name.split(f".{function_name}")[0]
         self.module = importlib.import_module(module_name)
         function = getattr(self.module, function_name)
         return function(*args, **kwargs)
 
 
-def is_optimum_habana_available():
+auto_gptq = LazyImport("auto_gptq")
+htcore = LazyImport("habana_frameworks.torch.core")
 
+
+def is_optimum_habana_available():
     from transformers.utils.import_utils import is_optimum_available
 
     return is_optimum_available() and importlib.util.find_spec("optimum.habana") is not None
 
 
-htcore = LazyImport("habana_frameworks.torch.core")
-
-
 def round_ste(x: torch.Tensor):
     """Straight-Through Estimator for rounding.
     This function is adapted from omniquant.
 
     Args:
         x: torch.Tensor
 
@@ -99,26 +101,24 @@
         min_scale: Minimum scale coefficient for weight
         max_scale: Maximum scale coefficient for weight
 
     Returns:
         Quantized and dequantized weight, scale, zero-point
     """
     maxq = torch.tensor(2**num_bits - 1)
-    zeros = torch.zeros(weight.shape[0], device=weight.device, dtype=scale_dtype)
-    # zeros = torch.zeros(weight.shape[0], device=weight.device)
     if isinstance(min_scale, torch.Tensor):
-        wmin_tmp = torch.minimum(weight.min(1)[0], zeros)
-        wmax_tmp = torch.maximum(weight.max(1)[0], zeros)
+        wmin_tmp = torch.clamp(weight.min(1)[0], max=0)
+        wmax_tmp = torch.clamp(weight.max(1)[0], min=0)
         wmin_tmp *= min_scale + 1.0
         wmax_tmp *= max_scale + 1.0
         wmax = torch.maximum(wmax_tmp, wmin_tmp)
         wmin = torch.minimum(wmax_tmp, wmin_tmp)
     else:
-        wmin = torch.minimum(weight.min(1)[0], zeros)
-        wmax = torch.maximum(weight.max(1)[0], zeros)
+        wmin = torch.clamp(weight.min(1)[0], max=0)
+        wmax = torch.clamp(weight.max(1)[0], min=0)
 
     tmp = (wmin == 0) & (wmax == 0)
     wmin[tmp] = -1
     wmax[tmp] = +1
     scale = ((wmax - wmin) / maxq).to(scale_dtype)
     zp = round_ste(-wmin / scale)
     scale = scale.unsqueeze(dim=-1)
@@ -138,25 +138,24 @@
         min_scale: Minimum scale coefficient for weight
         max_scale: Maximum scale coefficient for weight
 
     Returns:
         Quantized and dequantized weight, scale, zero-point
     """
     maxq = torch.tensor(2**num_bits - 1)
-    zeros = torch.zeros(weight.shape[0], device=weight.device, dtype=scale_dtype)
     if isinstance(min_scale, torch.Tensor):
-        wmin_tmp = torch.minimum(weight.min(1)[0], zeros)
-        wmax_tmp = torch.maximum(weight.max(1)[0], zeros)
+        wmin_tmp = torch.clamp(weight.min(1)[0], max=0)
+        wmax_tmp = torch.clamp(weight.max(1)[0], min=0)
         wmin_tmp *= min_scale + 1.0
         wmax_tmp *= max_scale + 1.0
         wmax = torch.maximum(wmax_tmp, wmin_tmp)
         wmin = torch.minimum(wmax_tmp, wmin_tmp)
     else:
-        wmin = torch.minimum(weight.min(1)[0], zeros)
-        wmax = torch.maximum(weight.max(1)[0], zeros)
+        wmin = torch.clamp(weight.min(1)[0], max=0)
+        wmax = torch.clamp(weight.max(1)[0], min=0)
     wmax_new = torch.max(wmin.abs(), wmax)
     tmp = wmin < 0
     wmin_new = wmin.clone()  ##must clone, otherwise inplace backward will occur
     if torch.any(tmp):
         wmin_new[tmp] = -wmax_new[tmp]
 
     tmp = (wmin_new == 0) & (wmax_new == 0)
@@ -286,17 +285,15 @@
 
     Args:
         module (torch.nn.Module): original model
         key (str): module name to be replaced
     """
     name_list = key.split(".")
     for name in name_list:
-        if hasattr(module, name):
-            module = getattr(module, name)
-            module = module
+        module = getattr(module, name, None)
     return module
 
 
 def set_module(model, key, new_module):
     """Set new module into model by key name.
 
     Args:
@@ -305,16 +302,14 @@
         new_module (torch.nn.Module): new module to be inserted
     """
     module = model
     name_list = key.split(".")
     for name in name_list[:-1]:
         if hasattr(module, name):
             module = getattr(module, name)
-        else:
-            module = module
     setattr(module, name_list[-1], new_module)
 
 
 def get_scale_shape(weight, group_size):
     """Computes the shape of the scale tensor for quantization based on the weight tensor and group size.
 
     Args:
@@ -328,34 +323,42 @@
         shape = weight.shape[0]
     else:
         shape = weight.shape[0] * ((weight.shape[1] + group_size - 1) // group_size)
 
     return shape
 
 
-def move_input_to_device(input, device=torch.device("cpu")):
+def to_device(input, device=torch.device("cpu")):
     """Moves input data to the specified device.
 
     Args:
     input: The input data to be moved.
     device: The target device.
 
     Returns:
     The input data on the specified device.
     """
+    if input is None:
+        return None
     if isinstance(input, torch.Tensor):
         return input.to(device)
     if isinstance(input, dict) or isinstance(input, UserDict):
         for inp in input.keys():
-            input[inp] = move_input_to_device(input[inp], device)
+            input[inp] = to_device(input[inp], device)
+
     elif isinstance(input, list) or isinstance(input, tuple):
+        if len(input) == 0:
+            return input
         input_res = []
         for inp in input:
-            input_res.append(move_input_to_device(inp, device))
+            input_res.append(to_device(inp, device))
+        if isinstance(input, tuple):
+            input_res = tuple(input_res)
         input = input_res
+
     return input
 
 
 def check_is_cpu(device):
     """Check if the device is a CPU.
 
     Args:
@@ -420,72 +423,45 @@
         if hasattr(m, "orig_layer"):
             min_scales[n] = copy.deepcopy(torch.clamp(m.min_scale.data, -1, 0))
             max_scales[n] = copy.deepcopy(torch.clamp(m.max_scale.data, -1, 0))
     return min_scales, max_scales
 
 
 @torch.no_grad()
-def get_batch_dim(input_others):
-    """Gets the batch dimension based on the input positional inputs.
-
-    Args:
-    input_others: A dictionary containing input data.
-
-    Returns:
-    dim: The batch dimension.
-    """
-    dim = int(len(input_others["positional_inputs"]) > 0)
-    return dim
-
-
-def sampling_inputs(input_ids, input_others, indices, seqlen, share_attention_mask_flag=False):
+def sampling_inputs(input_ids, input_others, indices, seqlen, share_attention_mask_flag=False, input_dim=0):
     """Samples inputs based on the given indices and sequence length.
 
     Args:
-    input_ids: The input tensor containing IDs.
+    input_ids: The list of input tensor containing  input_ids.
     input_others: A dictionary containing other input data.
     indices: The indices to sample from the input.
     seqlen: The sequence length.
 
     Returns:
     current_input_ids: The sampled input IDs.
     current_input_others: The sampled other input data.
     """
-    if len(input_ids.shape) == 3:
-        if int(len(input_others["positional_inputs"]) > 0):
-            current_input_ids = input_ids[:, indices, :]
-        else:
-            current_input_ids = input_ids[indices, :, :]
-    else:
-        n_samples = input_ids.shape[0] // seqlen
-        current_input_ids = input_ids.view(n_samples, seqlen, -1)
-        current_input_ids = current_input_ids[indices, :, :]
-        current_input_ids = current_input_ids.reshape(-1, input.shape[-1])
+    current_input_ids = [input_ids[i] for i in indices]
+    current_input_ids = torch.cat(current_input_ids, dim=input_dim)
 
     current_input_others = {"positional_inputs": input_others["positional_inputs"]}
     for key in input_others.keys():
-        if not share_attention_mask_flag and "attention_mask" in key or "alibi" in key:
+        if not share_attention_mask_flag and ("attention_mask" in key or "alibi" in key):
             current_input_others[key] = None
             if input_others[key] is not None:
-                current_input_others[key] = input_others[key][indices, ...]
+                current_input_others[key] = [input_others[key][i] for i in indices]
+                current_input_others[key] = torch.cat(current_input_others[key], dim=0)
+
         else:
             current_input_others[key] = input_others[key]
 
     return current_input_ids, current_input_others
 
 
-def block_forward(
-    block,
-    input_ids,
-    input_others,
-    amp=False,
-    amp_dtype=torch.bfloat16,
-    amp_device_type="hpu",
-    device=torch.device("cpu"),
-):
+def block_forward(block, input_ids, input_others, amp=False, amp_dtype=torch.float16, device=torch.device("cpu")):
     """Performs a forward pass through a block with the given inputs.
 
     Args:
     block: The block to perform the forward pass on.
     input_ids: The input IDs.
     input_others: A dictionary containing other input data.
     amp: A boolean indicating whether to use automatic mixed precision.
@@ -493,41 +469,34 @@
     device: The target device.
 
     Returns:
     output: The output of the forward pass.
     """
     if input_ids.device != device:
         # input_ids, input_others = move_to_device(input_ids, input_others, device)
-        input_ids = move_input_to_device(input_ids, device)
-        input_others = move_input_to_device(input_others, device)
+        input_ids = to_device(input_ids, device)
+        input_others = to_device(input_others, device)
+    input_tuple = input_others.pop("positional_inputs", None)
     if "alibi" in input_others.keys():
-        attention_mask = input_others["attention_mask"]
-        alibi = input_others["alibi"]
+        alibi = input_others.pop("alibi")
         if alibi is not None:
             alibi = alibi.reshape(-1, alibi.shape[2], alibi.shape[3])
-        if amp and not check_is_cpu(device):
-            with autocast(device_type=amp_device_type, dtype=amp_dtype):  # pragma: no cover
+        if amp:
+            with autocast(device_type=device.split(":")[0], dtype=amp_dtype):  # pragma: no cover
                 output = block(
-                    input_ids, attention_mask=attention_mask, alibi=alibi
+                    input_ids, alibi=alibi, *input_tuple, **input_others
                 )  ##TODO is this correct for all models with alibi?
-        elif amp and check_is_cpu(device):
-            with torch.autocast(device_type=amp_device_type, dtype=torch.bfloat16):
-                output = block(input_ids, attention_mask=attention_mask, alibi=alibi)
         else:
-            output = block(input_ids, attention_mask=attention_mask, alibi=alibi)
+            output = block(input_ids, alibi=alibi, *input_tuple, **input_others)
     else:
-        input_tuple = input_others.pop("positional_inputs", None)
-        if amp and not check_is_cpu(device):
-            with autocast(device_type=amp_device_type, dtype=amp_dtype):  # pragma: no cover
-                output = block.forward(input_ids, *input_tuple, **input_others)
-        elif amp and check_is_cpu(device):
-            with torch.autocast(device_type=amp_device_type, dtype=torch.bfloat16):
-                output = block.forward(input_ids, *input_tuple, **input_others)
+        if amp:
+            with autocast(device_type=device.split(":")[0], dtype=amp_dtype):  # pragma: no cover
+                output = block(input_ids, *input_tuple, **input_others)
         else:
-            output = block.forward(input_ids, *input_tuple, **input_others)
+            output = block(input_ids, *input_tuple, **input_others)
     if isinstance(output, list) or isinstance(output, tuple):
         output = output[0]
     return output
 
 
 def check_to_quantized(config):
     if isinstance(config, dict):
@@ -536,26 +505,14 @@
         return True
     else:
         if config.bits > 8 or "fp" in config.data_type or "float" in config.data_type:
             return False
         return True
 
 
-def is_share_attention_mask_model(model):
-    model_name = None
-    if not hasattr(model, "config") or not hasattr(model.config, "_name_or_path"):
-        logger.warn("Unable to get model name via config, assumed to be a normal model.")
-        return True
-    model_name = model.config._name_or_path
-    for key in SHARE_ATTENTION_MASK_LIST:
-        if key in model_name:
-            return True
-    return False
-
-
 def detect_device(device=None):
     def is_valid_digit(s):
         try:
             num = int(s)
             return 0 <= num
         except:
             return False
@@ -571,15 +528,15 @@
         elif is_optimum_habana_available():
             device = torch.device("hpu")
             logger.info("Using HPU device")
         # Use CPU as a fallback
         else:
             device = torch.device("cpu")
             logger.info("Using CPU device")
-        if dev_idx is not None:
+        if dev_idx is not None and str(device) != "cpu":
             device = str(device) + f":{dev_idx}"
         return str(device)
     elif isinstance(device, torch.device):
         device = str(device)
     return device
 
 
@@ -643,7 +600,165 @@
             universal_newlines=False,
         ) as proc:
             proc.wait()
             if proc.stdout:
                 for line in proc.stdout:
                     return int(line.decode("utf-8", errors="ignore").strip())
         return 0
+
+
+def is_local_path(path):
+    """Checks if a given path exists locally.
+
+    Args:
+        path (str): The path to check.
+
+    Returns:
+        bool: True if the path exists locally, False otherwise.
+    """
+    return os.path.exists(path)
+
+
+def convert_dtype_str2torch(str_dtype):
+    """Converts a string dtype to its corresponding PyTorch dtype.
+
+    Args:
+        str_dtype (str): The string representation of the dtype.
+
+    Returns:
+        torch.dtype: The PyTorch dtype.
+
+    Raises:
+        AssertionError: If the input str_dtype is unsupported.
+    """
+    if isinstance(str_dtype, torch.dtype) or str_dtype is None:
+        return str_dtype
+    if str_dtype == "int8":
+        return torch.int8
+    elif str_dtype == "fp32" or str_dtype == "float32" or str_dtype == "auto":
+        return torch.float
+    elif str_dtype == "fp16" or str_dtype == "float16":
+        return torch.float16
+    elif str_dtype == "bf16" or str_dtype == "bfloat16":
+        return torch.bfloat16
+    else:
+        assert False, "Unsupported str dtype {} to torch dtype".format(str_dtype)
+
+
+def convert_dtype_torch2str(dtype):
+    """Converts a PyTorch dtype to its corresponding string representation.
+
+    Args:
+        dtype: PyTorch dtype or str. The dtype to convert.
+
+    Returns:
+        str: The string representation of the dtype.
+
+    Raises:
+        AssertionError: If the input dtype is unsupported.
+    """
+    if isinstance(dtype, str) or dtype is None:
+        return dtype
+    if dtype == torch.int8:
+        return "int8"
+    elif dtype == torch.float:
+        return "fp32"
+    elif dtype == torch.float16:
+        return "fp16"
+    elif dtype == torch.bfloat16:
+        return "bf16"
+    elif isinstance(dtype, str) and dtype in ["int8", "fp32", "fp16", "bf16"]:
+        return dtype
+    else:
+        assert False, "Unsupported pytorch dtype {} to str dtype".format(dtype)
+
+
+def convert_dtype_torch2str_hf(dtype):
+    """Converts a PyTorch dtype to its corresponding huggingface string dtype, e.g. torch.float32 -> 'float32'.
+
+    Args:
+        dtype: PyTorch dtype or str. The dtype to convert.
+
+    Returns:
+         str: The string representation of the dtype.
+
+    Raises:
+        AssertionError: If the input str_dtype is unsupported.
+    """
+    if dtype is None:
+        return dtype
+    if isinstance(dtype, str):
+        if "float" not in dtype and "int" not in dtype:
+            dtype = convert_dtype_str2torch(dtype)
+        else:
+            return dtype
+    str_dtype = str(dtype)
+    if "." not in str_dtype:
+        assert False, "Unsupported pytorch dtype {} to huggingface str dtype".format(dtype)
+    str_dtype = str_dtype.split(".")[1]
+    return str_dtype
+
+
+def check_memory_availability(device, inputs, weight, org_seqlen, org_bs):
+    """Checks the availability of memory on the specified device for processing inputs using a given weight tensor.
+
+    Args:
+        device (str): The device type ('cuda' for GPU or 'hpu' for HPU).
+        inputs (torch.Tensor): Input tensor.
+        weight (torch.Tensor): Weight tensor.
+        org_seqlen (int): Original sequence length.
+        org_bs (int): Original batch size.
+
+    Returns:
+        tuple: A tuple containing availability status (bool), modified sequence length (int),
+               and modified batch size (int).
+    """
+    weight_memory = weight.numel() * weight.element_size()
+    if "cuda" in device:
+        current_gpu_index = torch.cuda.current_device()
+        total_memory = torch.cuda.get_device_properties(current_gpu_index).total_memory
+        used_memory = torch.cuda.memory_allocated(current_gpu_index)
+        free_space = total_memory - used_memory
+    elif "hpu" in device:
+        current_hpu_index = torch.hpu.current_device()
+        free_space = torch.hpu.memory_reserved(current_hpu_index)
+    else:
+        return True, org_seqlen, org_bs
+
+    free_space = free_space - weight_memory * 10  # for min_max_scale & grad usage
+    seqlen = org_seqlen
+    bs = org_bs
+    in_feature = weight.shape[1]
+    out_feature = weight.shape[0]
+    while seqlen >= 128:
+        input_size = bs * seqlen * in_feature
+        output_size = bs * seqlen * out_feature
+        input_output_memory = 2 * (input_size * inputs.element_size() + output_size * inputs.element_size())
+        if input_output_memory < free_space:
+            return True, seqlen, bs
+        seqlen = seqlen // 2
+        bs = 1
+
+    return False, seqlen, bs
+
+
+def get_layer_names_in_block(model, supported_types=[torch.nn.Linear, transformers.modeling_utils.Conv1D]):
+    """Retrieves the names of layers within each block of the model.
+
+    Returns:
+        list: A list of strings, where each string is the name of a layer
+              within a block of the model.
+    """
+    for n, m in model.named_modules():
+        if isinstance(m, tuple(supported_types)):
+            m.tmp_name = n
+    layers_in_block = []
+    block_names = get_block_names(model)
+    for block_name in block_names:
+        block = get_module(model, block_name)
+        for n, m in block.named_modules():
+            if hasattr(m, "tmp_name"):
+                layers_in_block.append(m.tmp_name)
+    for n, m in model.named_modules():
+        if hasattr(m, "tmp_name"):
+            delattr(m, "tmp_name")
+    return layers_in_block
```

### Comparing `auto_round-0.11/auto_round/version.py` & `auto_round-0.2/auto_round/export/export_to_autoround/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# Copyright (c) 2023 Intel Corporation
+# Copyright (c) 2024 Intel Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Intel® auto-round: An open-source Python library
-supporting popular model weight only compression based on signround."""
 
-__version__ = "0.11"
+from .export_to_autoround import save_quantized_as_autoround
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `auto_round-0.11/auto_round.egg-info/PKG-INFO` & `auto_round-0.2/auto_round.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,218 +1,236 @@
 Metadata-Version: 2.1
 Name: auto-round
-Version: 0.11
+Version: 0.2
 Summary: Repository of AutoRound: Advanced Weight-Only Quantization Algorithm for LLMs
 Home-page: https://github.com/intel/auto-round
 Author: Intel AIPT Team
 Author-email: wenhua.cheng@intel.com, weiwei1.zhang@intel.com
 License: Apache 2.0
+Description: <div align="center">
+        
+        AutoRound
+        ===========================
+        <h3> Advanced Weight-Only Quantization Algorithm for LLMs</h3>
+        
+        [![python](https://img.shields.io/badge/python-3.8%2B-blue)](https://github.com/intel/auto-round)
+        [![version](https://img.shields.io/badge/release-0.2-green)](https://github.com/intel/auto-round)
+        [![license](https://img.shields.io/badge/license-Apache%202-blue)](https://github.com/intel/auto-round/blob/main/LICENSE)
+        ---
+        <div align="left">
+        
+        AutoRound is an advanced weight-only quantization algorithm for low-bits LLM inference. It's tailored for a wide range
+        of models and consistently delivers noticeable improvements, often significantly outperforming SignRound with the cost
+        of more tuning time for quantization.
+        
+        Our method adopts sign gradient descent to fine-tune rounding values and minmax values of weights in just 200 steps,
+        which competes impressively against recent methods without introducing any additional inference overhead. The below
+        image presents an overview of AutoRound.
+        
+        <div align="center">
+        
+        ![](docs/imgs/autoround_overview.png)
+        
+        <div align="left">
+        
+        ## What's New
+        
+        * [2024/05] Check out our updated paper on [arxiv](https://arxiv.org/pdf/2309.05516v4)
+        * [2024/05] AutoRound supports lm-head quantization, saving 0.7G for LLaMA3-8B at W4G128.
+        * [2024/05] AutoRound performs well
+          in [low_bit_open_llm_leaderboard](https://huggingface.co/spaces/Intel/low_bit_open_llm_leaderboard)
+        
+        ## Prerequisites
+        
+        - Python 3.9 or higher
+        
+        ## Installation
+        
+        ### Build from Source
+        
+        ```bash
+        pip install -r requirements.txt
+        python setup.py install
+        ```
+        
+        ### Install from pypi
+        
+        ```bash
+        pip install auto-round
+        ```
+        
+        ## Model quantization
+        
+        ### Gaudi2/ CPU/ GPU
+        
+        We found a significant accuracy discrepancy with the qdq model using the AutoGPTQ GPU backend with asymmetric
+        quantization in some scenarios. Please switch to symmetric quantization to alleviate this issue.
+        
+        ```python
+        from transformers import AutoModelForCausalLM, AutoTokenizer
+        
+        model_name = "meta-llama/Llama-2-7b-hf"
+        model = AutoModelForCausalLM.from_pretrained(model_name, torch_dtype="auto", trust_remote_code=True)
+        tokenizer = AutoTokenizer.from_pretrained(model_name, trust_remote_code=True)
+        
+        from auto_round import AutoRound
+        
+        bits, group_size, sym = 4, 128, False
+        ##device:Optional["auto", None, "hpu", "cpu", "cuda"]
+        autoround = AutoRound(model, tokenizer, bits=bits, group_size=group_size, sym=sym, device=None)
+        autoround.quantize()
+        output_dir = "./tmp_autoround"
+        autoround.save_quantized(output_dir)
+        ```
+        
+        <details>
+          <summary>Detailed Hyperparameters</summary>
+        
+        - `model`: The PyTorch model to be quantized.
+        
+        - `tokenizer`: An optional tokenizer for processing input data. If none, a dataset must be provided.
+        
+        - `bits (int)`: Number of bits for quantization (default is 4).
+        
+        - `group_size (int)`: Size of the quantization group (default is 128).
+        
+        - `sym (bool)`: Whether to use symmetric quantization (default is False).
+        
+        - `enable_quanted_input (bool)`: Whether to use the output of the previous quantized block as the input for the current
+          block for tuning (default is True).
+        
+        - `enable_minmax_tuning (bool)`: Whether to enable weight min-max tuning (default is True).
+        
+        - `iters (int)`: Number of tuning iterations (default is 200).
+        
+        - `lr (float)`: The learning rate for rounding value (default is None, it will be set to 1.0/iters automatically).
+        
+        - `minmax_lr (float)`: The learning rate for min-max tuning (default is None, it will be set to lr automatically).
+        
+        - `n_samples (int)`: Number of samples for tuning (default is 512).
+        
+        - `seqlen (int)`: Data length of the sequence for tuning (default is 2048).
+        
+        - `batch_size (int)`: Batch size for training (default is 8).
+        
+        - `scale_dtype (str)`: The data type of quantization scale to be used (default is "float16"), different kernels have
+          different choices.
+        
+        - `amp (bool)`: Whether to use automatic mixed precision (default is True).
+        
+        - `n_blocks (int)`: Packing several blocks as one for tuning together (default is 1).
+        
+        - `gradient_accumulate_steps (int)`: Number of gradient accumulation steps (default is 1).
+        
+        - `low_gpu_mem_usage (bool)`: Whether to save GPU memory at the cost of ~20% more tuning time (default is True).
+        
+        - `dataset Union[str, list, tuple, torch.utils.data.DataLoader]`: The dataset name for tuning (default is "
+          NeelNanda/pile-10k"). Local json file and combination of datasets have been supported, e.g. "
+          ./tmp.json,NeelNanda/pile-10k:train, mbpp:train+validation+test"
+        
+        - `weight_config (dict)`: Configuration for weight quantization (default is an empty dictionary), mainly for mixed bits
+          or mixed precision.
+        
+        - `device`: The device to be used for tuning. The default is set to 'auto', allowing for automatic detection.
+        
+        </details>
+        
+        ## Model inference
+        
+        Please run the quantization code first.
+        
+        ### CPU
+        
+        ```python
+        ##Install the latest https://github.com/intel/intel-extension-for-transformers from source first.
+        from intel_extension_for_transformers.transformers import AutoModelForCausalLM
+        from transformers import AutoTokenizer
+        
+        quantized_model_path = "./tmp_autoround"
+        model = AutoModelForCausalLM.from_pretrained(quantized_model_path, device_map="auto", trust_remote_code=True)
+        tokenizer = AutoTokenizer.from_pretrained(quantized_model_path, use_fast=True)
+        text = "There is a girl who likes adventure,"
+        inputs = tokenizer(text, return_tensors="pt").to(model.device)
+        print(tokenizer.decode(model.generate(**inputs, max_new_tokens=50)[0]))
+        ```
+        
+        ### GPU
+        
+        ```python
+        from transformers import AutoModelForCausalLM, AutoTokenizer
+        ##from auto_round.auto_quantizer import AutoHfQuantizer ## uncomment it for models with quantized lm-head
+        
+        quantized_model_path = "./tmp_autoround"
+        model = AutoModelForCausalLM.from_pretrained(quantized_model_path, device_map="auto", trust_remote_code=True)
+        tokenizer = AutoTokenizer.from_pretrained(quantized_model_path, use_fast=True)
+        text = "There is a girl who likes adventure,"
+        inputs = tokenizer(text, return_tensors="pt").to(model.device)
+        print(tokenizer.decode(model.generate(**inputs, max_new_tokens=50)[0]))
+        ```
+        
+        ## Support List
+        
+        | Model                                | Supported                                                                                                                                                                                                                                                                                                           |
+        |--------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+        | Intel/neural-chat-7b-v3-3            | [HF-int4-model](https://huggingface.co/Intel/neural-chat-7b-v3-3-int4-inc), [accuracy](./docs/neural-chat-7b-v3-3-acc.md), [recipe](./examples/language-modeling/scripts/neural-chat-7b-v3-3.sh), [example](./examples/language-modeling/)                                                                          |
+        | Intel/neural-chat-7b-v3-1            | [HF-int4-model](https://huggingface.co/Intel/neural-chat-7b-v3-1-int4-inc), [accuracy](./docs/neural-chat-7b-v3-1-acc.md), [recipe](./examples/language-modeling/scripts/neural-chat-7b-v3-1.sh), [example](./examples/language-modeling/)                                                                          |
+        | mistralai/Mistral-7B-v0.1            | [HF-int4-model-lmhead](https://huggingface.co/Intel/Mistral-7B-v0.1-int4-inc-lmhead),[HF-int4-model](https://huggingface.co/Intel/Mistral-7B-v0.1-int4-inc), [accuracy](./docs/Mistral-7B-v0.1-acc.md), [recipe](./examples/language-modeling/scripts/Mistral-7B-v0.1.sh), [example](./examples/language-modeling/) |
+        | microsoft/phi-2                      | [HF-int4-sym-model](https://huggingface.co/Intel/phi-2-int4-inc), [accuracy](./docs/phi-2-acc.md), [recipe](./examples/language-modeling/scripts/phi-2.sh), [example](./examples/language-modeling/)                                                                                                                
+        | google/gemma-2b                      | [HF-int4-model](https://huggingface.co/Intel/gemma-2b-int4-inc), [accuracy](./docs/gemma-2b-acc.md), [recipe](./examples/language-modeling/scripts/gemma-2b.sh),  [example](./examples/language-modeling/)                                                                                                          
+        | tiiuae/falcon-7b                     | [HF-int4-model-G64](https://huggingface.co/Intel/falcon-7b-int4-inc), [accuracy](./docs/falcon-7b-acc.md), [recipe](./examples/language-modeling/scripts/falcon-7b.sh), [example](./examples/language-modeling/)                                                                                                    |
+        | mistralai/Mistral-7B-Instruct-v0.2   | [HF-int4-model](https://huggingface.co/Intel/Mistral-7B-Instruct-v0.2-int4-inc) (under review), [accuracy](./docs/Mistral-7B-Instruct-v0.2-acc.md), [recipe](./examples/language-modeling/scripts/Mistral-7B-Instruct-v0.2.sh),  [example](./examples/language-modeling/)                                           |
+        | google/gemma-7b                      | [HF-int4-model](https://huggingface.co/Intel/gemma-7b-int4-inc) (under review), [accuracy](./docs/gemma-7b-acc.md), [recipe](./examples/language-modeling/scripts/gemma-7b.sh),  [example](./examples/language-modeling/)                                                                                           |
+        | mistralai/Mixtral-8x7B-Instruct-v0.1 | [HF-int4-model](https://huggingface.co/Intel/Mixtral-8x7B-Instruct-v0.1-int4-inc) (under review), [accuracy](./docs/Mixtral-8x7B-Instruct-v0.1-acc.md), [recipe](./examples/language-modeling/scripts/Mixtral-8x7B-Instruct-v0.1.sh),  [example](./examples/language-modeling/)                                     |
+        | mistralai/Mixtral-8x7B-v0.1          | [HF-int4-model](https://huggingface.co/Intel/Mixtral-8x7B-v0.1-int4-inc) (under review), [accuracy](./docs/Mixtral-8x7B-v0.1-acc.md), [recipe](./examples/language-modeling/scripts/Mixtral-8x7B-v0.1.sh), [example](./examples/language-modeling/)                                                                 |
+        | meta-llama/Meta-Llama-3-8B-Instruct  | [accuracy](./docs/Meta-Llama-3-8B-Instruct-acc.md), [recipe](./examples/language-modeling/scripts/Meta-Llama-3-8B-Instruct.sh), [example](./examples/language-modeling/)                                                                                                                                            |
+        | meta-llama/Llama-2-7b-chat-hf        | [accuracy](./docs/Llama-2-7b-chat-hf-acc.md), [recipe](./examples/language-modeling/scripts/Llama-2-7b-chat-hf.sh), [example](./examples/language-modeling/)                                                                                                                                                        |
+        | Qwen/Qwen1.5-7B-Chat                 | [accuracy](./docs/Qwen1.5-7B-Chat-acc.md), [sym recipe](./examples/language-modeling/scripts/Qwen1.5-7B-Chat-sym.sh), [asym recipe ](./examples/language-modeling/scripts/Qwen1.5-7B-Chat-asym.sh), [example](./examples/language-modeling/)                                                                        |
+        | baichuan-inc/Baichuan2-7B-Chat       | [accuracy](./docs/baichuan2-7b-chat-acc.md), [recipe](./examples/language-modeling/scripts/baichuan2-7b-chat.sh), [example](./examples/language-modeling/)                                                                                                                                                          |
+        | 01-ai/Yi-6B-Chat                     | [accuracy](./docs/Yi-6B-Chat-acc.md), [recipe](./examples/language-modeling/scripts/Yi-6B-Chat.sh), [example](./examples/language-modeling/)                                                                                                                                                                        |
+        | facebook/opt-2.7b                    | [accuracy](./docs/opt-2.7b-acc.md), [recipe](./examples/language-modeling/scripts/opt-2.7b.sh), [example](./examples/language-modeling/)                                                                                                                                                                            |
+        | bigscience/bloom-3b                  | [accuracy](./docs/bloom-3B-acc.md), [recipe](./examples/language-modeling/scripts/bloom-3b.sh), [example](./examples/language-modeling/)                                                                                                                                                                            |
+        | EleutherAI/gpt-j-6b                  | [accuracy](./docs/gpt-j-6B-acc.md), [recipe](./examples/language-modeling/scripts/gpt-j-6b.sh), [example](./examples/language-modeling/)                                                                                                                                                                            |
+        | Salesforce/codegen25-7b-multi        | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+        | huggyllama/llama-7b                  | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+        | mosaicml/mpt-7b                      | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+        | THUDM/chatglm3-6b                    | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+        | MBZUAI/LaMini-GPT-124M               | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+        | EleutherAI/gpt-neo-125m              | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+        | databricks/dolly-v2-3b               | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            |
+        | stabilityai/stablelm-base-alpha-3b   | [example](./examples/language-modeling/)                                                                                                                                                                                                                                                                            
+        
+        ## Comparison with other methods
+        
+        We provide a [comprehensive analysis](docs/acc.md) with other methods in our accuracy data section. In summary, our
+        approach achieved superior performance compared to GPTQ, scoring 30/32, AWQ with 27/32, HQQ with 15/16, and OmniQuant
+        with a perfect score of 16/16 across llamv1/llamav2/mistral-7b on W4G-1, W4G128, W3G128, and W2G128, based on the
+        average accuracies of 11 zero-shot tasks.
+        
+        ## Tips
+        
+        1 Consider increasing tuning steps to achieve better results, albeit with increased tuning time.
+        
+        2 Setting 'enable_quanted_input' to False has been observed to occasionally yield improved results.
+        
+        3 Setting 'minmax_lr' to 2.0/iters has been observed to occasionally yield improved results.
+        
+        ## Reference
+        
+        If you find SignRound useful for your research, please cite our paper:
+        
+        ```bash
+        @article{cheng2023optimize,
+          title={Optimize Weight Rounding via Signed Gradient Descent for the Quantization of LLMs},
+          author={Cheng, Wenhua and Zhang, Weiwei and Shen, Haihao and Cai, Yiyang and He, Xin and Lv, Kaokao and Liu, Yi},
+          journal={arXiv preprint arXiv:2309.05516},
+          year={2023}
+        }
+        ```
+        
 Keywords: quantization,auto-around,LLM,SignRound
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: third-party-programs.txt
-
-<div align="center">
-
-AutoRound
-===========================
-<h3> Advanced Weight-Only Quantization Algorithm for LLMs</h3>
-
-[![python](https://img.shields.io/badge/python-3.8%2B-blue)](https://github.com/intel/auto-round)
-[![version](https://img.shields.io/badge/release-0.1-green)](https://github.com/intel/auto-round)
-[![license](https://img.shields.io/badge/license-Apache%202-blue)](https://github.com/intel/auto-round/blob/main/LICENSE)
----
-<div align="left">
-
-AutoRound is an advanced weight-only quantization algorithm for low-bits LLM inference. It's tailored for a wide range of models and consistently delivers noticeable improvements, often significantly outperforming SignRound with the cost of more tuning time for quantization.
-
-## Prerequisites
-- Python 3.9 or higher
-
-## Installation
-### Build from Source
-```bash
-pip install -r requirements.txt
-python setup.py install
-```
-### Install from pypi
-```bash
-pip install auto-round
-```
-## Usage of Tuning
-
-### On CPU/ Gaudi2/ GPU
-
-```python
-import torch
-from transformers import AutoModelForCausalLM, AutoTokenizer
-
-tuning_device = "cuda:0"  ## or "cpu", "hpu"
-dtype = "auto" if tuning_device != "hpu" else torch.bfloat16
-model_name = "meta-llama/Llama-2-7b-hf"
-model = AutoModelForCausalLM.from_pretrained(model_name, torch_dtype=dtype, trust_remote_code=True)
-tokenizer = AutoTokenizer.from_pretrained(model_name, trust_remote_code=True)
-
-from auto_round import AutoRound
-
-bits, group_size, sym = 4, 128, False
-autoround = AutoRound(model, tokenizer, bits=bits, group_size=group_size, sym=sym, device=tuning_device)
-autoround.quantize()
-output_dir = "./tmp_autoround"
-autoround.save_quantized(output_dir)
-```
-
-
-
-## Model inference
-Please run the tuning code first
-
-
-
-### Intel CPU
-```python
-# Please save the quantized model in 'itrex' format first, then refer to the ITREX tutorial for more details on inference with the INT4 model.
-# (https://github.com/intel/intel-extension-for-transformers/tree/main/intel_extension_for_transformers/llm/runtime/neural_speed)
-from intel_extension_for_transformers.transformers import AutoModelForCausalLM, WeightOnlyQuantConfig
-from transformers import AutoTokenizer
-
-quantized_model_path = "./tmp_autoround"
-scheme = "sym" if sym else "asym"
-woq_config = WeightOnlyQuantConfig(
-    group_size=group_size, scheme=scheme, use_autoround=True
-)  ##only supports 4 bits currently
-prompt = "There is a girl who likes adventure,"
-tokenizer = AutoTokenizer.from_pretrained(quantized_model_path, trust_remote_code=True)
-inputs = tokenizer(prompt, return_tensors="pt").input_ids
-model = AutoModelForCausalLM.from_pretrained(
-    quantized_model_path, quantization_config=woq_config, trust_remote_code=True, device="cpu"
-)
-outputs = model.generate(inputs, max_new_tokens=50)
-print(tokenizer.decode(outputs[0]))
-```
-
-
-### GPU
-```python
-from transformers import AutoModelForCausalLM, AutoTokenizer
-
-quantized_model_path = "./tmp_autoround"
-model = AutoModelForCausalLM.from_pretrained(quantized_model_path, device_map="auto", trust_remote_code=True)
-tokenizer = AutoTokenizer.from_pretrained(quantized_model_path, use_fast=True)
-text = "There is a girl who likes adventure,"
-inputs = tokenizer(text, return_tensors="pt").to(model.device)
-print(tokenizer.decode(model.generate(**inputs, max_new_tokens=50)[0]))
-```
-
-<details>
-  <summary>Detailed Hyperparameters</summary>
-
-- `model`: The PyTorch model to be quantized.
-            
-- `tokenizer`: An optional tokenizer for processing input data. If none is provided, a dataloader must be supplied.
-  
-- `bits (int)`: Number of bits for quantization (default is 4).
-  
-- `group_size (int)`: Size of the quantization group (default is 128).
-
-- `sym (bool)`: Whether to use symmetric quantization.
-  
-- `use_quant_input (bool)`: Whether to use the output of the previous quantized block as the input for the current block (default is True).
-  
-- `enable_minmax_tuning (bool)`: Whether to enable weight min-max tuning (default is True).
-  
-- `iters (int)`: Number of tuning iterations (default is 200).
-  
-- `lr (float)`: The learning rate for rounding value (default is None, it will be set to 1.0/iters automatically).
-  
-- `minmax_lr (float)`: The learning rate for min-max tuning (default is None, it will be set to lr automatically).
-  
-- `n_samples (int)`: Number of samples for tuning (default is 512).
-  
-- `seqlen (int)`: Data length of the sequence for tuning (default is 2048).
-  
-- `batch_size (int)`: Batch size for training (default is 8).
-
-- `scale_dtype (str)`: The data type of quantization scale to be used (default is "float32"), different kernels have different choices.
-  
-- `amp (bool)`: Whether to use automatic mixed precision (default is True).
-  
-- `n_blocks (int)`: Packing several blocks as one for tuning together (default is 1).
-  
-- `gradient_accumulate_steps (int)`: Number of gradient accumulation steps (default is 1).
-  
-- `low_gpu_mem_usage (bool)`: Whether to save GPU memory at the cost of a little tuning time (default is True).
-  
-- `dataset (str)`: The default dataset name for tuning (default is "NeelNanda/pile-10k").
-  
-- `dataset_split (str)`: The split of the dataset to be used for tuning (default is "train").
-  
-- `dataloader`: The dataloader for tuning data.
-  
-- `weight_config (dict)`: Configuration for weight quantization (default is an empty dictionary), mainly for mixed bits or mixed precision.
-  
-- `device`: The device to be used for tuning. The default is set to 'auto', allowing for automatic detection.
-
-</details>
-
-
-## Support List
-
-| Model                    | Supported                                                                                                                                                                                                                                                          |
-|--------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| Intel/neural-chat-7b-v3-3 | [HF-int4-model](https://huggingface.co/Intel/neural-chat-7b-v3-3-int4-inc), [accuracy](./docs/neural-chat-7b-v3-3-acc.md), [recipe](./examples/language-modeling/scripts/neural-chat-7b-v3-3.sh), [example](./examples/language-modeling/)                         |
-| Intel/neural-chat-7b-v3-1 | [HF-int4-model](https://huggingface.co/Intel/neural-chat-7b-v3-1-int4-inc), [accuracy](./docs/neural-chat-7b-v3-1-acc.md), [recipe](./examples/language-modeling/scripts/neural-chat-7b-v3-1.sh), [example](./examples/language-modeling/)                         |
-| mistralai/Mistral-7B-v0.1 | [HF-int4-model](https://huggingface.co/Intel/Mistral-7B-v0.1-int4-inc), [accuracy](./docs/Mistral-7B-v0.1-acc.md), [recipe](./examples/language-modeling/scripts/Mistral-7B-v0.1.sh), [example](./examples/language-modeling/)                                     |
-| google/gemma-7b          | [HF-int4-model](https://huggingface.co/Intel/gemma-7b-int4-inc) under review, [accuracy](./docs/gemma-7b-acc.md), [recipe](./examples/language-modeling/scripts/gemma-7b.sh),  [example](./examples/language-modeling/)                                            |
-| google/gemma-7b-it       | [HF-int4-model](https://huggingface.co/Intel/gemma-7b-it-int4-inc) under review, [accuracy](./docs/gemma-7b-it-acc.md), [recipe](./examples/language-modeling/scripts/gemma-7b-it.sh), [example](./examples/language-modeling/)                                    |                                            |
-  mistralai/Mixtral-8x7B-Instruct-v0.1 | [HF-int4-model](https://huggingface.co/Intel/Mistral-7B-v0.1-int4-inc) under review, [accuracy](./docs/Mixtral-8x7B-Instruct-v0.1-acc.md), [recipe](./examples/language-modeling/scripts/Mixtral-8x7B-Instruct-v0.1.sh),  [example](./examples/language-modeling/) |
-| mistralai/Mixtral-8x7B-v0.1 | [HF-int4-model](https://huggingface.co/Intel/Mixtral-8x7B-v0.1-int4-inc) under review, [accuracy](./docs/Mixtral-8x7B-v0.1-acc.md), [recipe](./examples/language-modeling/scripts/Mixtral-8x7B-v0.1.sh), [example](./examples/language-modeling/)                  |
-| microsoft/phi-2          | [HF-int4-model](https://huggingface.co/Intel/phi-2-int4-inc) under review, [accuracy](./docs/phi-2-acc.md), [recipe](./examples/language-modeling/scripts/phi-2.sh), [example](./examples/language-modeling/)                                                      |
-| meta-llama/Llama-2-7b-chat-hf | [accuracy](./docs/Llama-2-7b-chat-hf-acc.md), [recipe](./examples/language-modeling/scripts/Llama-2-7b-chat-hf.sh), [example](./examples/language-modeling/)                                                                                                                    |
-| Salesforce/codegen25-7b-multi | [example](./examples/code-generation)                                                                                                                                                                                                                              |
-| EleutherAI/gpt-j-6b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| huggyllama/llama-7b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| meta-llama/Llama-2-7b-hf | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| facebook/opt-6.7b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| tiiuae/falcon-7b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| mosaicml/mpt-7b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| bigscience/bloom-7b1 | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| baichuan-inc/Baichuan-7B | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| Qwen/Qwen-7B | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| THUDM/chatglm3-6b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| MBZUAI/LaMini-GPT-124M | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| EleutherAI/gpt-neo-125m | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| databricks/dolly-v2-3b | [example](./examples/language-modeling/)                                                                                                                                                                                                                           |
-| stabilityai/stablelm-base-alpha-3b | [example](./examples/language-modeling/)
-
-
-
-
-## Comparison with other methods
-
-We provide a [comprehensive analysis](docs/acc.md) with other methods in our accuracy data section. Notably, our approach has outperformed GPTQ with a score of 30/32 and AWQ with a score of 27/32 across llamv1/llamav2/mistral-7b on W4G-1, W4G128, W3G128, W2G128.  And the tuning costs are comparable.
-
-## Tips
-1 Consider increasing tuning steps to achieve better results, albeit with increased tuning time. 
-
-2 Setting 'use_quant_input' to False has been observed to occasionally yield improved results.
-
-3 Setting 'minmax_lr' to 2.0/iters has been observed to occasionally yield improved results.
-
-## Reference
-If you find SignRound useful for your research, please cite our paper:
-```bash
-@article{cheng2023optimize,
-  title={Optimize Weight Rounding via Signed Gradient Descent for the Quantization of LLMs},
-  author={Cheng, Wenhua and Zhang, Weiwei and Shen, Haihao and Cai, Yiyang and He, Xin and Lv, Kaokao},
-  journal={arXiv preprint arXiv:2309.05516},
-  year={2023}
-}
-```
-
-
```

### Comparing `auto_round-0.11/auto_round.egg-info/SOURCES.txt` & `auto_round-0.2/auto_round.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 LICENSE
 README.md
-pyproject.toml
 setup.cfg
 setup.py
 third-party-programs.txt
 auto_round/__init__.py
+auto_round/auto_quantizer.py
 auto_round/autoround.py
 auto_round/calib_dataset.py
 auto_round/sign_sgd.py
+auto_round/special_model_handler.py
 auto_round/utils.py
 auto_round/version.py
 auto_round.egg-info/PKG-INFO
 auto_round.egg-info/SOURCES.txt
 auto_round.egg-info/dependency_links.txt
 auto_round.egg-info/requires.txt
 auto_round.egg-info/top_level.txt
 auto_round/export/__init__.py
 auto_round/export/export_to_autogptq.py
 auto_round/export/register.py
+auto_round/export/export_to_autoround/__init__.py
+auto_round/export/export_to_autoround/export_to_autoround.py
 auto_round/export/export_to_itrex/__init__.py
 auto_round/export/export_to_itrex/config.py
 auto_round/export/export_to_itrex/export.py
 auto_round/export/export_to_itrex/model_wrapper.py
 test/test_autoopt.py
 test/test_autoround.py
-test/test_autoround_export.py
+test/test_autoround_export.py
+test/test_calib_dataset.py
```

### Comparing `auto_round-0.11/setup.py` & `auto_round-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `auto_round-0.11/test/test_autoopt.py` & `auto_round-0.2/test/test_autoopt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 import shutil
 import sys
 import unittest
 
-sys.path.insert(0, ".")
+sys.path.insert(0, "..")
 import torch
 import transformers
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 from auto_round import AutoOPTRound
 
 
@@ -38,14 +38,15 @@
         autoround = AutoOPTRound(
             self.model,
             self.tokenizer,
             bits=bits,
             group_size=group_size,
             sym=sym,
             iters=2,
-            dataloader=self.llm_dataloader,
+            seqlen=10,
+            dataset=self.llm_dataloader,
         )
         autoround.quantize()
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `auto_round-0.11/test/test_autoround.py` & `auto_round-0.2/test/test_autoround.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 import shutil
 import sys
 import unittest
 
-sys.path.insert(0, ".")
+sys.path.insert(0, "..")
 import torch
 import transformers
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 from auto_round import AutoRound
 
 
@@ -38,15 +38,16 @@
         autoround = AutoRound(
             self.model,
             self.tokenizer,
             bits=bits,
             group_size=group_size,
             sym=sym,
             iters=2,
-            dataloader=self.llm_dataloader,
+            seqlen=2,
+            dataset=self.llm_dataloader,
         )
         autoround.quantize()
         if torch.cuda.is_available():
             autoround.save_quantized(output_dir="./saved", inplace=False)
         autoround.save_quantized(output_dir="./saved", inplace=False, format="itrex")
 
     def test_sym(self):
@@ -54,96 +55,121 @@
         autoround = AutoRound(
             self.model,
             self.tokenizer,
             bits=bits,
             group_size=group_size,
             sym=sym,
             iters=2,
-            dataloader=self.llm_dataloader,
+            seqlen=10,
+            dataset=self.llm_dataloader,
         )
         autoround.quantize()
 
     def test_w4g1(self):
         bits, group_size, sym = 4, -1, True
         autoround = AutoRound(
             self.model,
             self.tokenizer,
             bits=bits,
             group_size=group_size,
             sym=sym,
             iters=2,
-            dataloader=self.llm_dataloader,
+            seqlen=10,
+            dataset=self.llm_dataloader,
         )
         autoround.quantize()
 
     def test_w3g128(self):
         bits, group_size, sym = 3, 128, True
         autoround = AutoRound(
             self.model,
             self.tokenizer,
             bits=bits,
             group_size=group_size,
             sym=sym,
             iters=2,
-            dataloader=self.llm_dataloader,
+            seqlen=10,
+            dataset=self.llm_dataloader,
         )
         autoround.quantize()
 
     def test_w2g128(self):
         bits, group_size, sym = 2, 128, True
         autoround = AutoRound(
             self.model,
             self.tokenizer,
             bits=bits,
             group_size=group_size,
             sym=sym,
             iters=2,
-            dataloader=self.llm_dataloader,
+            seqlen=10,
+            dataset=self.llm_dataloader,
         )
         autoround.quantize()
 
-    def test_disable_use_quant_input(self):
+    def test_disable_enable_quanted_input(self):
         bits, group_size, sym = 4, -1, True
         autoround = AutoRound(
             self.model,
             self.tokenizer,
             bits=bits,
             group_size=group_size,
             sym=sym,
             iters=2,
-            use_quant_input=False,
-            dataloader=self.llm_dataloader,
+            seqlen=10,
+            enable_quanted_input=False,
+            dataset=self.llm_dataloader,
         )
         autoround.quantize()
 
     def test_disable_minmax_tuning(self):
         bits, group_size, sym = 4, -1, True
         autoround = AutoRound(
             self.model,
             self.tokenizer,
             bits=bits,
             group_size=group_size,
             sym=sym,
             iters=2,
+            seqlen=10,
             enable_minmax_tuning=False,
-            dataloader=self.llm_dataloader,
+            dataset=self.llm_dataloader,
         )
         autoround.quantize()
 
     def test_signround(self):
         bits, group_size, sym = 4, -1, False
         autoround = AutoRound(
             self.model,
             self.tokenizer,
             bits=bits,
             group_size=group_size,
             sym=sym,
             iters=2,
+            seqlen=10,
             enable_minmax_tuning=False,
-            use_quant_input=False,
-            dataloader=self.llm_dataloader,
+            enable_quanted_input=False,
+            dataset=self.llm_dataloader,
+        )
+        autoround.quantize()
+
+    def test_lm_head(self):
+        bits, group_size, sym = 4, -1, False
+        weight_config = {"lm_head": {"data_type": "int"}}
+        autoround = AutoRound(
+            self.model,
+            self.tokenizer,
+            bits=bits,
+            group_size=group_size,
+            sym=sym,
+            iters=2,
+            seqlen=10,
+            enable_minmax_tuning=False,
+            enable_quanted_input=False,
+            dataset=self.llm_dataloader,
+            weight_config=weight_config,
         )
         autoround.quantize()
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `auto_round-0.11/test/test_autoround_export.py` & `auto_round-0.2/test/test_autoround_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 import shutil
 import sys
 import unittest
 
-sys.path.insert(0, ".")
+sys.path.insert(0, "..")
 import torch
 import transformers
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 from auto_round import AutoRound
```

### Comparing `auto_round-0.11/third-party-programs.txt` & `auto_round-0.2/third-party-programs.txt`

 * *Files identical despite different names*

