# Comparing `tmp/chattts_fork-0.0.1.tar.gz` & `tmp/chattts_fork-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chattts_fork-0.0.1.tar", last modified: Wed May 29 11:04:52 2024, max compression
+gzip compressed data, was "chattts_fork-0.0.2.tar", last modified: Thu May 30 06:50:47 2024, max compression
```

## Comparing `chattts_fork-0.0.1.tar` & `chattts_fork-0.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-05-29 11:04:52.889634 chattts_fork-0.0.1/
-drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-05-29 11:04:52.885634 chattts_fork-0.0.1/ChatTTS/
--rw-rw-r--   0 yihong    (1000) yihong    (1000)       30 2024-05-29 11:04:42.000000 chattts_fork-0.0.1/ChatTTS/__init__.py
--rw-rw-r--   0 yihong    (1000) yihong    (1000)       68 2024-05-29 11:04:42.000000 chattts_fork-0.0.1/ChatTTS/__main__.py
--rw-rw-r--   0 yihong    (1000) yihong    (1000)      987 2024-05-29 11:04:42.000000 chattts_fork-0.0.1/ChatTTS/cli.py
--rw-rw-r--   0 yihong    (1000) yihong    (1000)     7196 2024-05-29 11:04:42.000000 chattts_fork-0.0.1/ChatTTS/core.py
-drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-05-29 11:04:52.885634 chattts_fork-0.0.1/ChatTTS/experimental/
--rw-rw-r--   0 yihong    (1000) yihong    (1000)        0 2024-05-29 11:01:48.000000 chattts_fork-0.0.1/ChatTTS/experimental/__init__.py
--rw-rw-r--   0 yihong    (1000) yihong    (1000)     3438 2024-05-29 11:04:42.000000 chattts_fork-0.0.1/ChatTTS/experimental/llm.py
-drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-05-29 11:04:52.885634 chattts_fork-0.0.1/ChatTTS/infer/
--rw-rw-r--   0 yihong    (1000) yihong    (1000)        0 2024-05-29 11:01:40.000000 chattts_fork-0.0.1/ChatTTS/infer/__init__.py
--rw-rw-r--   0 yihong    (1000) yihong    (1000)     4463 2024-05-29 11:04:42.000000 chattts_fork-0.0.1/ChatTTS/infer/api.py
-drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-05-29 11:04:52.885634 chattts_fork-0.0.1/ChatTTS/model/
--rw-rw-r--   0 yihong    (1000) yihong    (1000)        0 2024-05-29 10:56:35.000000 chattts_fork-0.0.1/ChatTTS/model/__init__.py
--rw-rw-r--   0 yihong    (1000) yihong    (1000)     5112 2024-05-29 11:04:42.000000 chattts_fork-0.0.1/ChatTTS/model/dvae.py
--rw-rw-r--   0 yihong    (1000) yihong    (1000)    12773 2024-05-29 11:04:42.000000 chattts_fork-0.0.1/ChatTTS/model/gpt.py
-drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-05-29 11:04:52.885634 chattts_fork-0.0.1/ChatTTS/utils/
--rw-rw-r--   0 yihong    (1000) yihong    (1000)        0 2024-05-29 11:01:18.000000 chattts_fork-0.0.1/ChatTTS/utils/__init__.py
--rw-rw-r--   0 yihong    (1000) yihong    (1000)      970 2024-05-29 11:04:42.000000 chattts_fork-0.0.1/ChatTTS/utils/gpu_utils.py
--rw-rw-r--   0 yihong    (1000) yihong    (1000)     1797 2024-05-29 11:04:42.000000 chattts_fork-0.0.1/ChatTTS/utils/infer_utils.py
--rw-rw-r--   0 yihong    (1000) yihong    (1000)      380 2024-05-29 11:04:42.000000 chattts_fork-0.0.1/ChatTTS/utils/io_utils.py
--rw-rw-r--   0 yihong    (1000) yihong    (1000)    17529 2024-05-29 10:09:35.000000 chattts_fork-0.0.1/LICENSE
--rw-r--r--   0 yihong    (1000) yihong    (1000)     7039 2024-05-29 11:04:52.889634 chattts_fork-0.0.1/PKG-INFO
--rw-rw-r--   0 yihong    (1000) yihong    (1000)     6204 2024-05-29 10:09:35.000000 chattts_fork-0.0.1/README.md
-drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-05-29 11:04:52.889634 chattts_fork-0.0.1/chattts_fork.egg-info/
--rw-r--r--   0 yihong    (1000) yihong    (1000)     7039 2024-05-29 11:04:52.000000 chattts_fork-0.0.1/chattts_fork.egg-info/PKG-INFO
--rw-rw-r--   0 yihong    (1000) yihong    (1000)      600 2024-05-29 11:04:52.000000 chattts_fork-0.0.1/chattts_fork.egg-info/SOURCES.txt
--rw-rw-r--   0 yihong    (1000) yihong    (1000)        1 2024-05-29 11:04:52.000000 chattts_fork-0.0.1/chattts_fork.egg-info/dependency_links.txt
--rw-rw-r--   0 yihong    (1000) yihong    (1000)       45 2024-05-29 11:04:52.000000 chattts_fork-0.0.1/chattts_fork.egg-info/entry_points.txt
--rw-rw-r--   0 yihong    (1000) yihong    (1000)       91 2024-05-29 11:04:52.000000 chattts_fork-0.0.1/chattts_fork.egg-info/requires.txt
--rw-rw-r--   0 yihong    (1000) yihong    (1000)        8 2024-05-29 11:04:52.000000 chattts_fork-0.0.1/chattts_fork.egg-info/top_level.txt
--rw-rw-r--   0 yihong    (1000) yihong    (1000)       38 2024-05-29 11:04:52.889634 chattts_fork-0.0.1/setup.cfg
--rwxrwxr-x   0 yihong    (1000) yihong    (1000)     1127 2024-05-29 11:00:29.000000 chattts_fork-0.0.1/setup.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-30 06:50:47.407494 chattts_fork-0.0.2/
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-30 06:50:47.385352 chattts_fork-0.0.2/ChatTTS/
+-rw-r--r--   0 hyi        (502) staff       (20)       30 2024-05-30 04:07:50.000000 chattts_fork-0.0.2/ChatTTS/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       68 2024-05-30 04:07:50.000000 chattts_fork-0.0.2/ChatTTS/__main__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1451 2024-05-30 06:42:40.000000 chattts_fork-0.0.2/ChatTTS/cli.py
+-rw-r--r--   0 hyi        (502) staff       (20)     7503 2024-05-30 06:39:43.000000 chattts_fork-0.0.2/ChatTTS/core.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-30 06:50:47.387052 chattts_fork-0.0.2/ChatTTS/experimental/
+-rw-r--r--   0 hyi        (502) staff       (20)        0 2024-05-30 04:07:50.000000 chattts_fork-0.0.2/ChatTTS/experimental/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3438 2024-05-30 04:07:50.000000 chattts_fork-0.0.2/ChatTTS/experimental/llm.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-30 06:50:47.388194 chattts_fork-0.0.2/ChatTTS/infer/
+-rw-r--r--   0 hyi        (502) staff       (20)        0 2024-05-30 04:07:50.000000 chattts_fork-0.0.2/ChatTTS/infer/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     4463 2024-05-30 04:07:50.000000 chattts_fork-0.0.2/ChatTTS/infer/api.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-30 06:50:47.389822 chattts_fork-0.0.2/ChatTTS/model/
+-rw-r--r--   0 hyi        (502) staff       (20)        0 2024-05-30 04:07:50.000000 chattts_fork-0.0.2/ChatTTS/model/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     5112 2024-05-30 04:07:50.000000 chattts_fork-0.0.2/ChatTTS/model/dvae.py
+-rw-r--r--   0 hyi        (502) staff       (20)    12773 2024-05-30 04:07:50.000000 chattts_fork-0.0.2/ChatTTS/model/gpt.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-30 06:50:47.392978 chattts_fork-0.0.2/ChatTTS/utils/
+-rw-r--r--   0 hyi        (502) staff       (20)        0 2024-05-30 04:07:50.000000 chattts_fork-0.0.2/ChatTTS/utils/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1051 2024-05-30 05:55:15.000000 chattts_fork-0.0.2/ChatTTS/utils/gpu_utils.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1797 2024-05-30 04:07:50.000000 chattts_fork-0.0.2/ChatTTS/utils/infer_utils.py
+-rw-r--r--   0 hyi        (502) staff       (20)      380 2024-05-30 04:07:50.000000 chattts_fork-0.0.2/ChatTTS/utils/io_utils.py
+-rw-r--r--   0 hyi        (502) staff       (20)    17529 2024-05-30 04:07:50.000000 chattts_fork-0.0.2/LICENSE
+-rw-r--r--   0 hyi        (502) staff       (20)     7116 2024-05-30 06:50:47.407133 chattts_fork-0.0.2/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)     6281 2024-05-30 05:26:34.000000 chattts_fork-0.0.2/README.md
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-30 06:50:47.406578 chattts_fork-0.0.2/chattts_fork.egg-info/
+-rw-r--r--   0 hyi        (502) staff       (20)     7116 2024-05-30 06:50:47.000000 chattts_fork-0.0.2/chattts_fork.egg-info/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)      600 2024-05-30 06:50:47.000000 chattts_fork-0.0.2/chattts_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        1 2024-05-30 06:50:47.000000 chattts_fork-0.0.2/chattts_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       45 2024-05-30 06:50:47.000000 chattts_fork-0.0.2/chattts_fork.egg-info/entry_points.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       91 2024-05-30 06:50:47.000000 chattts_fork-0.0.2/chattts_fork.egg-info/requires.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        8 2024-05-30 06:50:47.000000 chattts_fork-0.0.2/chattts_fork.egg-info/top_level.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       38 2024-05-30 06:50:47.407556 chattts_fork-0.0.2/setup.cfg
+-rwxr-xr-x   0 hyi        (502) staff       (20)     1127 2024-05-30 06:49:25.000000 chattts_fork-0.0.2/setup.py
```

### Comparing `chattts_fork-0.0.1/ChatTTS/cli.py` & `chattts_fork-0.0.2/ChatTTS/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,45 @@
+import os
+os.environ["PYTORCH_ENABLE_MPS_FALLBACK"] = "1"
+
 from .core import Chat
 import argparse
 import numpy as np
 import wave
 
 
 def main():
     # cli args
     ap = argparse.ArgumentParser(description="Your text to tts")
     ap.add_argument("text", type=str, help="Your text")
     ap.add_argument(
         "-o", "--out-file", help="out file name", default="tts.wav", dest="out_file"
     )
+    ap.add_argument("--use-seed", help="use seed", action="store_true", dest="use_seed")
+    ap.add_argument(
+        "-s", "--seed", help="out file name", default=None, dest="seed"
+    )
 
     args = ap.parse_args()
     out_file = args.out_file
     text = args.text
     if not text:
         raise ValueError("text is empty")
+
     chat = Chat()
-    chat.load_models()
+    try:
+        chat.load_models()
+    except Exception as e:
+        # this is a tricky for most newbies do not now the args for cli
+        print("The model maybe broke will load again")
+        chat.load_models(force_redownload=True)
     texts = [
         text,
     ]
+
     wavs = chat.infer(texts, use_decoder=True)
     audio_data = np.array(wavs[0], dtype=np.float32)
     sample_rate = 24000
     audio_data = (audio_data * 32767).astype(np.int16)
 
     with wave.open(out_file, "w") as wf:
         wf.setnchannels(1)  # Mono channel
```

### Comparing `chattts_fork-0.0.1/ChatTTS/core.py` & `chattts_fork-0.0.2/ChatTTS/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 import os
+import sys
+import platform
 import logging
 from omegaconf import OmegaConf
 
+# Amazing WTF things to check if it is m1(m2,m3) chip
+# we need to change the environment variable before torch import
+if sys.platform == 'darwin' and platform.machine() == 'arm64':
+    os.environ["PYTORCH_ENABLE_MPS_FALLBACK"] = "1"
+
 import torch
 from vocos import Vocos
 from ChatTTS.model.dvae import DVAE
 from ChatTTS.model.gpt import GPT_warpper
 from ChatTTS.utils.gpu_utils import select_device
 from ChatTTS.utils.io_utils import get_latest_modified_file
 from ChatTTS.infer.api import refine_text, infer_code
@@ -97,49 +104,49 @@
         if not device:
             device = select_device(4096)
             self.logger.log(logging.INFO, f"use {device}")
 
         if vocos_config_path:
             vocos = Vocos.from_hparams(vocos_config_path).to(device).eval()
             assert vocos_ckpt_path, "vocos_ckpt_path should not be None"
-            vocos.load_state_dict(torch.load(vocos_ckpt_path))
+            vocos.load_state_dict(torch.load(vocos_ckpt_path, map_location=device))
             self.pretrain_models["vocos"] = vocos
             self.logger.log(logging.INFO, "vocos loaded.")
 
         if dvae_config_path:
             cfg = OmegaConf.load(dvae_config_path)
             dvae = DVAE(**cfg).to(device).eval()
             assert dvae_ckpt_path, "dvae_ckpt_path should not be None"
-            dvae.load_state_dict(torch.load(dvae_ckpt_path, map_location="cpu"))
+            dvae.load_state_dict(torch.load(dvae_ckpt_path, map_location=device))
             self.pretrain_models["dvae"] = dvae
             self.logger.log(logging.INFO, "dvae loaded.")
 
         if gpt_config_path:
             cfg = OmegaConf.load(gpt_config_path)
             gpt = GPT_warpper(**cfg).to(device).eval()
             assert gpt_ckpt_path, "gpt_ckpt_path should not be None"
-            gpt.load_state_dict(torch.load(gpt_ckpt_path, map_location="cpu"))
+            gpt.load_state_dict(torch.load(gpt_ckpt_path, map_location=device))
             self.pretrain_models["gpt"] = gpt
             spk_stat_path = os.path.join(os.path.dirname(gpt_ckpt_path), "spk_stat.pt")
             assert os.path.exists(
                 spk_stat_path
             ), f"Missing spk_stat.pt: {spk_stat_path}"
-            self.pretrain_models["spk_stat"] = torch.load(spk_stat_path).to(device)
+            self.pretrain_models["spk_stat"] = torch.load(spk_stat_path, map_location=device).to(device)
             self.logger.log(logging.INFO, "gpt loaded.")
 
         if decoder_config_path:
             cfg = OmegaConf.load(decoder_config_path)
             decoder = DVAE(**cfg).to(device).eval()
             assert decoder_ckpt_path, "decoder_ckpt_path should not be None"
-            decoder.load_state_dict(torch.load(decoder_ckpt_path, map_location="cpu"))
+            decoder.load_state_dict(torch.load(decoder_ckpt_path, map_location=device))
             self.pretrain_models["decoder"] = decoder
             self.logger.log(logging.INFO, "decoder loaded.")
 
         if tokenizer_path:
-            tokenizer = torch.load(tokenizer_path, map_location="cpu")
+            tokenizer = torch.load(tokenizer_path, map_location=device)
             tokenizer.padding_side = "left"
             self.pretrain_models["tokenizer"] = tokenizer
             self.logger.log(logging.INFO, "tokenizer loaded.")
 
         self.check_model()
 
     def infer(
@@ -183,15 +190,14 @@
                 for i in result["hiddens"]
             ]
         else:
             mel_spec = [
                 self.pretrain_models["dvae"](i[None].permute(0, 2, 1))
                 for i in result["ids"]
             ]
-
         wav = [self.pretrain_models["vocos"].decode(i).cpu().numpy() for i in mel_spec]
 
         return wav
 
     def sample_random_speaker(
         self,
     ):
```

### Comparing `chattts_fork-0.0.1/ChatTTS/experimental/llm.py` & `chattts_fork-0.0.2/ChatTTS/experimental/llm.py`

 * *Files identical despite different names*

### Comparing `chattts_fork-0.0.1/ChatTTS/infer/api.py` & `chattts_fork-0.0.2/ChatTTS/infer/api.py`

 * *Files identical despite different names*

### Comparing `chattts_fork-0.0.1/ChatTTS/model/dvae.py` & `chattts_fork-0.0.2/ChatTTS/model/dvae.py`

 * *Files identical despite different names*

### Comparing `chattts_fork-0.0.1/ChatTTS/model/gpt.py` & `chattts_fork-0.0.2/ChatTTS/model/gpt.py`

 * *Files identical despite different names*

### Comparing `chattts_fork-0.0.1/ChatTTS/utils/gpu_utils.py` & `chattts_fork-0.0.2/ChatTTS/utils/gpu_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,12 +15,14 @@
         free_memory_mb = max_free_memory / (1024 * 1024)
         if free_memory_mb < min_memory:
             logger.log(
                 logging.WARNING,
                 f"GPU {selected_gpu} has {round(free_memory_mb, 2)} MB memory left.",
             )
             device = torch.device("cpu")
+    elif torch.backends.mps.is_available():
+        device = torch.device('mps')
     else:
         logger.log(logging.WARNING, f"No GPU found, use CPU instead")
         device = torch.device("cpu")
 
     return device
```

### Comparing `chattts_fork-0.0.1/ChatTTS/utils/infer_utils.py` & `chattts_fork-0.0.2/ChatTTS/utils/infer_utils.py`

 * *Files identical despite different names*

### Comparing `chattts_fork-0.0.1/LICENSE` & `chattts_fork-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chattts_fork-0.0.1/PKG-INFO` & `chattts_fork-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chattts-fork
-Version: 0.0.1
+Version: 0.0.2
 Summary: fork from https://github.com/2noise/ChatTTS to PYPI
 Home-page: https://github.com/yihong0618/ChatTTS
 Author: lich99 CH.Li, yihong0618
 Author-email: zouzou0208@gmail.com
 License: # Attribution-NonCommercial-NoDerivatives 4.0 International
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -21,14 +21,19 @@
 Requires-Dist: vector_quantize_pytorch
 Requires-Dist: transformers~=4.41.1
 Requires-Dist: vocos
 
 # ChatTTS
 [**English**](./README.md) | [**中文简体**](./README_CN.md)
 
+# For this fork
+
+- pip3 install chattts-fork
+- chattts "哈哈" -o test.wav
+
 ChatTTS is a text-to-speech model designed specifically for dialogue scenario such as LLM assistant. It supports both English and Chinese languages. Our model is trained with 100,000+ hours composed of chinese and english. The open-source version on HuggingFace is a 40,000 hours pre trained model without SFT.
 
 For formal inquiries about model and roadmap, please contact us at open-source@2noise.com. You could join our QQ group: 808364215 for discussion. Adding github issues is always welcomed.
 
 ---
 ## Highlights
 1. **Conversational TTS**: ChatTTS is optimized for dialogue-based tasks, enabling natural and expressive speech synthesis. It supports multiple speakers, facilitating interactive conversations.
```

### Comparing `chattts_fork-0.0.1/README.md` & `chattts_fork-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # ChatTTS
 [**English**](./README.md) | [**中文简体**](./README_CN.md)
 
+# For this fork
+
+- pip3 install chattts-fork
+- chattts "哈哈" -o test.wav
+
 ChatTTS is a text-to-speech model designed specifically for dialogue scenario such as LLM assistant. It supports both English and Chinese languages. Our model is trained with 100,000+ hours composed of chinese and english. The open-source version on HuggingFace is a 40,000 hours pre trained model without SFT.
 
 For formal inquiries about model and roadmap, please contact us at open-source@2noise.com. You could join our QQ group: 808364215 for discussion. Adding github issues is always welcomed.
 
 ---
 ## Highlights
 1. **Conversational TTS**: ChatTTS is optimized for dialogue-based tasks, enabling natural and expressive speech synthesis. It supports multiple speakers, facilitating interactive conversations.
```

### Comparing `chattts_fork-0.0.1/chattts_fork.egg-info/PKG-INFO` & `chattts_fork-0.0.2/chattts_fork.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chattts-fork
-Version: 0.0.1
+Version: 0.0.2
 Summary: fork from https://github.com/2noise/ChatTTS to PYPI
 Home-page: https://github.com/yihong0618/ChatTTS
 Author: lich99 CH.Li, yihong0618
 Author-email: zouzou0208@gmail.com
 License: # Attribution-NonCommercial-NoDerivatives 4.0 International
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -21,14 +21,19 @@
 Requires-Dist: vector_quantize_pytorch
 Requires-Dist: transformers~=4.41.1
 Requires-Dist: vocos
 
 # ChatTTS
 [**English**](./README.md) | [**中文简体**](./README_CN.md)
 
+# For this fork
+
+- pip3 install chattts-fork
+- chattts "哈哈" -o test.wav
+
 ChatTTS is a text-to-speech model designed specifically for dialogue scenario such as LLM assistant. It supports both English and Chinese languages. Our model is trained with 100,000+ hours composed of chinese and english. The open-source version on HuggingFace is a 40,000 hours pre trained model without SFT.
 
 For formal inquiries about model and roadmap, please contact us at open-source@2noise.com. You could join our QQ group: 808364215 for discussion. Adding github issues is always welcomed.
 
 ---
 ## Highlights
 1. **Conversational TTS**: ChatTTS is optimized for dialogue-based tasks, enabling natural and expressive speech synthesis. It supports multiple speakers, facilitating interactive conversations.
```

### Comparing `chattts_fork-0.0.1/chattts_fork.egg-info/SOURCES.txt` & `chattts_fork-0.0.2/chattts_fork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chattts_fork-0.0.1/setup.py` & `chattts_fork-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from setuptools import setup, find_packages
 
 setup(
     name="chattts-fork",
     description="fork from https://github.com/2noise/ChatTTS to PYPI",
-    version="0.0.1",
+    version="0.0.2",
     license="# Attribution-NonCommercial-NoDerivatives 4.0 International",
     author="lich99 CH.Li, yihong0618",
     author_email="zouzou0208@gmail.com",
     url="https://github.com/yihong0618/ChatTTS",
     packages=find_packages(),
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
```

