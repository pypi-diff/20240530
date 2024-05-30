# Comparing `tmp/ipex_llm-2.1.0b20240529-py3-none-win_amd64.whl.zip` & `tmp/ipex_llm-2.1.0b20240530-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5383358 bytes, number of entries: 202
+Zip file size: 5383060 bytes, number of entries: 202
 -rw-------  2.0 unx     1898 b- defN 24-Mar-25 11:36 ipex_llm/__init__.py
 -rw-------  2.0 unx     6816 b- defN 24-Mar-25 11:36 ipex_llm/convert_model.py
 -rw-------  2.0 unx     3232 b- defN 24-May-07 15:07 ipex_llm/llm_patching.py
 -rw-------  2.0 unx     1177 b- defN 24-Mar-25 11:36 ipex_llm/models.py
 -rw-------  2.0 unx    12466 b- defN 24-May-24 15:08 ipex_llm/optimize.py
 -rw-------  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-chat.ps1
 -rwx------  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-cli.ps1
@@ -40,68 +40,68 @@
 -rw-------  2.0 unx     7225 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/transformersembeddings.py
 -rw-------  2.0 unx     1636 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/__init__.py
 -rw-------  2.0 unx    24438 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/bigdlllm.py
 -rw-------  2.0 unx    10576 b- defN 24-Apr-03 15:07 ipex_llm/langchain/llms/transformersllm.py
 -rw-------  2.0 unx     7379 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/transformerspipelinellm.py
 -rw-------  2.0 unx      874 b- defN 24-May-24 15:08 ipex_llm/langchain/vllm/__init__.py
 -rw-------  2.0 unx     7793 b- defN 24-May-24 15:08 ipex_llm/langchain/vllm/vllm.py
--rw-------  2.0 unx        0 b- defN 24-May-30 00:12 ipex_llm/libs/__init__.py
--rw-------  2.0 unx    36352 b- defN 24-May-30 00:12 ipex_llm/libs/bloom-api.dll
--rw-------  2.0 unx   472064 b- defN 24-May-30 00:12 ipex_llm/libs/bloom.dll
--rw-------  2.0 unx   854016 b- defN 24-May-30 00:12 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
--rw-------  2.0 unx   856576 b- defN 24-May-30 00:12 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
--rw-------  2.0 unx   844800 b- defN 24-May-30 00:12 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
--rw-------  2.0 unx    24576 b- defN 24-May-30 00:12 ipex_llm/libs/gptneox-api.dll
--rw-------  2.0 unx   531968 b- defN 24-May-30 00:12 ipex_llm/libs/gptneox.dll
--rw-------  2.0 unx   498688 b- defN 24-May-30 00:12 ipex_llm/libs/libbloom_avx.dll
--rw-------  2.0 unx   472576 b- defN 24-May-30 00:12 ipex_llm/libs/libbloom_vnni.dll
--rw-------  2.0 unx   559104 b- defN 24-May-30 00:12 ipex_llm/libs/libgptneox_avx.dll
--rw-------  2.0 unx   532992 b- defN 24-May-30 00:12 ipex_llm/libs/libgptneox_vnni.dll
--rw-------  2.0 unx   552960 b- defN 24-May-30 00:12 ipex_llm/libs/libllama_avx.dll
--rw-------  2.0 unx   526848 b- defN 24-May-30 00:12 ipex_llm/libs/libllama_vnni.dll
--rw-------  2.0 unx   590336 b- defN 24-May-30 00:12 ipex_llm/libs/libstarcoder_avx.dll
--rw-------  2.0 unx   564224 b- defN 24-May-30 00:12 ipex_llm/libs/libstarcoder_vnni.dll
--rw-------  2.0 unx    25088 b- defN 24-May-30 00:12 ipex_llm/libs/llama-api.dll
--rw-------  2.0 unx   526336 b- defN 24-May-30 00:12 ipex_llm/libs/llama.dll
--rw-------  2.0 unx   103424 b- defN 24-May-30 00:12 ipex_llm/libs/main-bloom.exe
--rw-------  2.0 unx   726528 b- defN 24-May-30 00:12 ipex_llm/libs/main-chatglm_vnni.exe
--rw-------  2.0 unx    98816 b- defN 24-May-30 00:12 ipex_llm/libs/main-gptneox.exe
--rw-------  2.0 unx    99840 b- defN 24-May-30 00:12 ipex_llm/libs/main-llama.exe
--rw-------  2.0 unx   157696 b- defN 24-May-30 00:12 ipex_llm/libs/main-starcoder.exe
--rw-------  2.0 unx   126464 b- defN 24-May-30 00:12 ipex_llm/libs/quantize-bloom.exe
--rw-------  2.0 unx   127488 b- defN 24-May-30 00:12 ipex_llm/libs/quantize-bloom_vnni.exe
--rw-------  2.0 unx   103936 b- defN 24-May-30 00:12 ipex_llm/libs/quantize-gptneox.exe
--rw-------  2.0 unx   104448 b- defN 24-May-30 00:12 ipex_llm/libs/quantize-gptneox_vnni.exe
--rw-------  2.0 unx   109056 b- defN 24-May-30 00:12 ipex_llm/libs/quantize-llama.exe
--rw-------  2.0 unx   110080 b- defN 24-May-30 00:12 ipex_llm/libs/quantize-llama_vnni.exe
--rw-------  2.0 unx   126976 b- defN 24-May-30 00:12 ipex_llm/libs/quantize-starcoder.exe
--rw-------  2.0 unx   128512 b- defN 24-May-30 00:12 ipex_llm/libs/quantize-starcoder_vnni.exe
--rw-------  2.0 unx    21504 b- defN 24-May-30 00:12 ipex_llm/libs/starcoder-api.dll
--rw-------  2.0 unx   563712 b- defN 24-May-30 00:12 ipex_llm/libs/starcoder.dll
+-rw-------  2.0 unx        0 b- defN 24-May-30 15:07 ipex_llm/libs/__init__.py
+-rw-------  2.0 unx    36352 b- defN 24-May-30 15:07 ipex_llm/libs/bloom-api.dll
+-rw-------  2.0 unx   472064 b- defN 24-May-30 15:07 ipex_llm/libs/bloom.dll
+-rw-------  2.0 unx   854016 b- defN 24-May-30 15:07 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
+-rw-------  2.0 unx   856576 b- defN 24-May-30 15:07 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
+-rw-------  2.0 unx   844800 b- defN 24-May-30 15:07 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
+-rw-------  2.0 unx    24576 b- defN 24-May-30 15:07 ipex_llm/libs/gptneox-api.dll
+-rw-------  2.0 unx   531968 b- defN 24-May-30 15:07 ipex_llm/libs/gptneox.dll
+-rw-------  2.0 unx   498688 b- defN 24-May-30 15:07 ipex_llm/libs/libbloom_avx.dll
+-rw-------  2.0 unx   472576 b- defN 24-May-30 15:07 ipex_llm/libs/libbloom_vnni.dll
+-rw-------  2.0 unx   559104 b- defN 24-May-30 15:07 ipex_llm/libs/libgptneox_avx.dll
+-rw-------  2.0 unx   532992 b- defN 24-May-30 15:07 ipex_llm/libs/libgptneox_vnni.dll
+-rw-------  2.0 unx   552960 b- defN 24-May-30 15:07 ipex_llm/libs/libllama_avx.dll
+-rw-------  2.0 unx   526848 b- defN 24-May-30 15:07 ipex_llm/libs/libllama_vnni.dll
+-rw-------  2.0 unx   590336 b- defN 24-May-30 15:07 ipex_llm/libs/libstarcoder_avx.dll
+-rw-------  2.0 unx   564224 b- defN 24-May-30 15:07 ipex_llm/libs/libstarcoder_vnni.dll
+-rw-------  2.0 unx    25088 b- defN 24-May-30 15:07 ipex_llm/libs/llama-api.dll
+-rw-------  2.0 unx   526336 b- defN 24-May-30 15:07 ipex_llm/libs/llama.dll
+-rw-------  2.0 unx   103424 b- defN 24-May-30 15:07 ipex_llm/libs/main-bloom.exe
+-rw-------  2.0 unx   726528 b- defN 24-May-30 15:07 ipex_llm/libs/main-chatglm_vnni.exe
+-rw-------  2.0 unx    98816 b- defN 24-May-30 15:07 ipex_llm/libs/main-gptneox.exe
+-rw-------  2.0 unx    99840 b- defN 24-May-30 15:07 ipex_llm/libs/main-llama.exe
+-rw-------  2.0 unx   157696 b- defN 24-May-30 15:07 ipex_llm/libs/main-starcoder.exe
+-rw-------  2.0 unx   126464 b- defN 24-May-30 15:07 ipex_llm/libs/quantize-bloom.exe
+-rw-------  2.0 unx   127488 b- defN 24-May-30 15:07 ipex_llm/libs/quantize-bloom_vnni.exe
+-rw-------  2.0 unx   103936 b- defN 24-May-30 15:07 ipex_llm/libs/quantize-gptneox.exe
+-rw-------  2.0 unx   104448 b- defN 24-May-30 15:07 ipex_llm/libs/quantize-gptneox_vnni.exe
+-rw-------  2.0 unx   109056 b- defN 24-May-30 15:07 ipex_llm/libs/quantize-llama.exe
+-rw-------  2.0 unx   110080 b- defN 24-May-30 15:07 ipex_llm/libs/quantize-llama_vnni.exe
+-rw-------  2.0 unx   126976 b- defN 24-May-30 15:07 ipex_llm/libs/quantize-starcoder.exe
+-rw-------  2.0 unx   128512 b- defN 24-May-30 15:07 ipex_llm/libs/quantize-starcoder_vnni.exe
+-rw-------  2.0 unx    21504 b- defN 24-May-30 15:07 ipex_llm/libs/starcoder-api.dll
+-rw-------  2.0 unx   563712 b- defN 24-May-30 15:07 ipex_llm/libs/starcoder.dll
 -rw-------  2.0 unx      874 b- defN 24-Mar-25 11:36 ipex_llm/llamaindex/__init__.py
 -rw-------  2.0 unx     1139 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/__init__.py
 -rw-------  2.0 unx    26314 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/bigdlllm.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/__init__.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/__init__.py
 -rw-------  2.0 unx    10084 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/bigdl_llm_model.py
 -rw-------  2.0 unx    19605 b- defN 24-May-20 15:06 ipex_llm/serving/fastchat/ipex_llm_worker.py
 -rw-------  2.0 unx    16649 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/model_worker.py
 -rw-------  2.0 unx     5918 b- defN 24-May-20 15:06 ipex_llm/serving/fastchat/tgi_api_protocol.py
--rw-------  2.0 unx    27062 b- defN 24-May-20 15:06 ipex_llm/serving/fastchat/tgi_api_server.py
+-rw-------  2.0 unx    24418 b- defN 24-May-30 15:06 ipex_llm/serving/fastchat/tgi_api_server.py
 -rw-------  2.0 unx    11093 b- defN 24-May-27 15:06 ipex_llm/serving/fastchat/vllm_worker.py
 -rw-------  2.0 unx     1005 b- defN 24-Mar-25 11:36 ipex_llm/transformers/__init__.py
 -rw-------  2.0 unx     1209 b- defN 24-May-28 15:07 ipex_llm/transformers/bmm.py
--rw-------  2.0 unx    76077 b- defN 24-May-24 15:08 ipex_llm/transformers/convert.py
+-rw-------  2.0 unx    76127 b- defN 24-May-30 15:06 ipex_llm/transformers/convert.py
 -rw-------  2.0 unx    14334 b- defN 24-Apr-26 15:08 ipex_llm/transformers/convert_ipex.py
 -rw-------  2.0 unx     4607 b- defN 24-May-28 15:07 ipex_llm/transformers/embedding.py
 -rw-------  2.0 unx     4247 b- defN 24-Apr-29 15:08 ipex_llm/transformers/kv.py
 -rw-------  2.0 unx     3289 b- defN 24-Apr-18 12:34 ipex_llm/transformers/lisa.py
 -rw-------  2.0 unx     6893 b- defN 24-May-24 15:08 ipex_llm/transformers/loader.py
 -rw-------  2.0 unx    15562 b- defN 24-May-16 02:22 ipex_llm/transformers/lookup.py
--rw-------  2.0 unx    40985 b- defN 24-May-30 00:11 ipex_llm/transformers/low_bit_linear.py
+-rw-------  2.0 unx    40895 b- defN 24-May-30 15:06 ipex_llm/transformers/low_bit_linear.py
 -rw-------  2.0 unx    39002 b- defN 24-May-28 15:07 ipex_llm/transformers/model.py
 -rw-------  2.0 unx     6921 b- defN 24-Mar-25 11:36 ipex_llm/transformers/modelling_bigdl.py
 -rw-------  2.0 unx    15520 b- defN 24-May-07 15:07 ipex_llm/transformers/qlora.py
 -rw-------  2.0 unx    16567 b- defN 24-Mar-25 11:36 ipex_llm/transformers/relora.py
 -rw-------  2.0 unx    56660 b- defN 24-May-08 15:07 ipex_llm/transformers/speculative.py
 -rw-------  2.0 unx     4842 b- defN 24-May-24 15:08 ipex_llm/transformers/streamer.py
 -rw-------  2.0 unx    10799 b- defN 24-May-27 15:06 ipex_llm/transformers/training_patch.py
@@ -189,16 +189,16 @@
 -rw-------  2.0 unx     6944 b- defN 24-May-24 15:08 ipex_llm/vllm/cpu/entrypoints/openai/api_server.py
 -rw-------  2.0 unx      585 b- defN 24-May-24 15:08 ipex_llm/vllm/xpu/__init__.py
 -rw-------  2.0 unx    18506 b- defN 24-May-24 15:08 ipex_llm/vllm/xpu/ipex_llm_gpu_executor.py
 -rw-------  2.0 unx     7172 b- defN 24-May-24 15:08 ipex_llm/vllm/xpu/model_convert.py
 -rw-------  2.0 unx      747 b- defN 24-May-24 15:08 ipex_llm/vllm/xpu/engine/__init__.py
 -rw-------  2.0 unx     5953 b- defN 24-May-24 15:08 ipex_llm/vllm/xpu/engine/engine.py
 -rw-------  2.0 unx    10568 b- defN 24-May-24 15:08 ipex_llm/vllm/xpu/entrypoints/openai/api_server.py
--rwxr-xr-x  2.0 unx     2578 b- defN 24-May-24 15:08 ipex_llm-2.1.0b20240529.data/scripts/ipex-llm-init.bat
--rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240529.data/scripts/llm-chat.ps1
--rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240529.data/scripts/llm-cli.ps1
--rw-------  2.0 unx     5495 b- defN 24-May-30 00:12 ipex_llm-2.1.0b20240529.dist-info/METADATA
--rw-------  2.0 unx       98 b- defN 24-May-30 00:12 ipex_llm-2.1.0b20240529.dist-info/WHEEL
--rw-------  2.0 unx       61 b- defN 24-May-30 00:12 ipex_llm-2.1.0b20240529.dist-info/entry_points.txt
--rw-------  2.0 unx        9 b- defN 24-May-30 00:12 ipex_llm-2.1.0b20240529.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    19167 b- defN 24-May-30 00:12 ipex_llm-2.1.0b20240529.dist-info/RECORD
-202 files, 13352382 bytes uncompressed, 5352728 bytes compressed:  59.9%
+-rwxr-xr-x  2.0 unx     2578 b- defN 24-May-24 15:08 ipex_llm-2.1.0b20240530.data/scripts/ipex-llm-init.bat
+-rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240530.data/scripts/llm-chat.ps1
+-rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240530.data/scripts/llm-cli.ps1
+-rw-------  2.0 unx     5495 b- defN 24-May-30 15:07 ipex_llm-2.1.0b20240530.dist-info/METADATA
+-rw-------  2.0 unx       98 b- defN 24-May-30 15:07 ipex_llm-2.1.0b20240530.dist-info/WHEEL
+-rw-------  2.0 unx       61 b- defN 24-May-30 15:07 ipex_llm-2.1.0b20240530.dist-info/entry_points.txt
+-rw-------  2.0 unx        9 b- defN 24-May-30 15:07 ipex_llm-2.1.0b20240530.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    19167 b- defN 24-May-30 15:07 ipex_llm-2.1.0b20240530.dist-info/RECORD
+202 files, 13349698 bytes uncompressed, 5352430 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -576,32 +576,32 @@
 
 Filename: ipex_llm/vllm/xpu/engine/engine.py
 Comment: 
 
 Filename: ipex_llm/vllm/xpu/entrypoints/openai/api_server.py
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240529.data/scripts/ipex-llm-init.bat
+Filename: ipex_llm-2.1.0b20240530.data/scripts/ipex-llm-init.bat
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240529.data/scripts/llm-chat.ps1
+Filename: ipex_llm-2.1.0b20240530.data/scripts/llm-chat.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240529.data/scripts/llm-cli.ps1
+Filename: ipex_llm-2.1.0b20240530.data/scripts/llm-cli.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240529.dist-info/METADATA
+Filename: ipex_llm-2.1.0b20240530.dist-info/METADATA
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240529.dist-info/WHEEL
+Filename: ipex_llm-2.1.0b20240530.dist-info/WHEEL
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240529.dist-info/entry_points.txt
+Filename: ipex_llm-2.1.0b20240530.dist-info/entry_points.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240529.dist-info/top_level.txt
+Filename: ipex_llm-2.1.0b20240530.dist-info/top_level.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240529.dist-info/RECORD
+Filename: ipex_llm-2.1.0b20240530.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipex_llm/libs/bloom-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800036cc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 29 15:02:40 2024
+Time/Date		Thu May 30 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000003200
 SizeOfInitializedData	0000000000005e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000036cc
@@ -6375,16 +6375,16 @@
    180005621:	push   %rdx
    180005622:	add    %al,0x1(%rax)
    180005628:	pop    %rax
    180005629:	push   %rdx
    18000562a:	add    %al,0x1(%rax)
    180005630:	add    %al,(%rax)
    180005632:	add    %al,(%rax)
-   180005634:	nop
-   180005635:	rex.XB push %r15
+   180005634:	adc    $0x95,%al
+   180005636:	pop    %rax
    180005637:	data16 add %al,(%rax)
    18000563a:	add    %al,(%rax)
    18000563c:	or     $0xe0000000,%eax
    180005641:	add    (%rax),%al
    180005643:	add    %cl,(%rcx,%rbx,2)
    180005646:	add    %al,(%rax)
    180005648:	or     $0x3f,%al
```

## ipex_llm/libs/bloom.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800558b8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 29 15:02:40 2024
+Time/Date		Thu May 30 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000055e00
 SizeOfInitializedData	00000000000bf200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000558b8
@@ -112267,17 +112267,17 @@
    18005e83a:	add    $0x180,%eax
    18005e83f:	add    %dh,0x76(%rax)
    18005e842:	add    $0x180,%eax
    18005e847:	add    %bh,0x76(%rax)
    18005e84a:	add    $0x180,%eax
    18005e84f:	add    %al,(%rax)
    18005e851:	add    %al,(%rax)
-   18005e853:	add    %dl,0x665743(%rax)
-   18005e859:	add    %al,(%rax)
-   18005e85b:	add    %cl,0x50000000(%rip)        # 0x1d005e861
+   18005e853:	add    %dl,0x6658(,%rdx,4)
+   18005e85a:	add    %al,(%rax)
+   18005e85c:	or     $0x50000000,%eax
    18005e861:	add    (%rax),%eax
    18005e863:	add    %ah,(%rax)
    18005e865:	repnz add $0x5e42000,%eax
 	...
    18005e87f:	add    %dl,0x18005f5(%rax)
    18005e885:	add    %al,(%rax)
    18005e887:	add    %bl,0x18005f5(%rax)
```

## ipex_llm/libs/gptneox-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002cbc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 29 15:02:40 2024
+Time/Date		Thu May 30 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002600
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002cbc
@@ -5058,16 +5058,16 @@
    1800049c0:	cmp    %al,0x0(%rdx)
    1800049c3:	addb   $0x0,(%rcx)
    1800049c6:	add    %al,(%rax)
    1800049c8:	rex
    1800049c9:	rex.X add %al,0x1(%rax)
    1800049d0:	add    %al,(%rax)
    1800049d2:	add    %al,(%rax)
-   1800049d4:	nop
-   1800049d5:	rex.XB push %r15
+   1800049d4:	adc    $0x95,%al
+   1800049d6:	pop    %rax
    1800049d7:	data16 add %al,(%rax)
    1800049da:	add    %al,(%rax)
    1800049dc:	or     $0xe0000000,%eax
    1800049e1:	add    (%rax),%al
    1800049e3:	add    %ah,0x0(%rsp,%rcx,2)
    1800049e7:	add    %ah,0x0(%rsi,%rsi,1)
 	...
```

## ipex_llm/libs/gptneox.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005d018
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 29 15:02:41 2024
+Time/Date		Thu May 30 15:02:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005d800
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005d018
@@ -123663,19 +123663,17 @@
    1800660fd:	add    %al,(%rax)
    1800660ff:	add    %bh,0x18005f6(%rax)
    180066105:	add    %al,(%rax)
    180066107:	add    %al,%al
    180066109:	testb  $0x0,0x180(%rip)        # 0x180066290
    180066110:	add    %al,(%rax)
    180066112:	add    %al,(%rax)
-   180066114:	xchg   %eax,%ecx
-   180066115:	rex.XB push %r15
-   180066117:	data16 add %al,(%rax)
-   18006611a:	add    %al,(%rax)
-   18006611c:	or     $0x50000000,%eax
+   180066114:	adc    $0x665895,%eax
+   180066119:	add    %al,(%rax)
+   18006611b:	add    %cl,0x50000000(%rip)        # 0x1d0066121
    180066121:	add    (%rax),%eax
    180066123:	add    %al,0x59840006(%rbp,%rbp,2)
    18006612a:	(bad)
 	...
    18006617f:	add    %bh,%al
    180066181:	jo     0x180066189
    180066183:	addb   $0x0,(%rcx)
```

## ipex_llm/libs/libbloom_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005bb78
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 29 15:03:48 2024
+Time/Date		Thu May 30 15:03:47 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c000
 SizeOfInitializedData	00000000000bf800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005bb78
@@ -117919,16 +117919,16 @@
    18006476a:	add    $0x180,%eax
    18006476f:	add    %dh,-0x2a(%rax)
    180064772:	add    $0x180,%eax
    180064777:	add    %bh,-0x2a(%rax)
    18006477a:	add    $0x180,%eax
    18006477f:	add    %al,(%rax)
    180064781:	add    %al,(%rax)
-   180064783:	add    %dl,%ah
-   180064785:	rex.XB push %r15
+   180064783:	add    %dl,-0x6b(%rbx)
+   180064786:	pop    %rax
    180064787:	data16 add %al,(%rax)
    18006478a:	add    %al,(%rax)
    18006478c:	or     $0x50000000,%eax
    180064791:	add    (%rax),%eax
    180064793:	add    %ah,-0x5ffff9af(%rax)
    180064799:	rex.RB (bad)
 	...
```

## ipex_llm/libs/libbloom_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180055ac8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 29 15:03:04 2024
+Time/Date		Thu May 30 15:03:04 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000056000
 SizeOfInitializedData	00000000000bf200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000055ac8
@@ -112386,17 +112386,20 @@
    18005e81a:	add    $0x180,%eax
    18005e81f:	add    %dh,0x76(%rax)
    18005e822:	add    $0x180,%eax
    18005e827:	add    %bh,0x76(%rax)
    18005e82a:	add    $0x180,%eax
    18005e82f:	add    %al,(%rax)
    18005e831:	add    %al,(%rax)
-   18005e833:	add    %ch,0x665743(%rax)
-   18005e839:	add    %al,(%rax)
-   18005e83b:	add    %cl,0x50000000(%rip)        # 0x1d005e841
+   18005e833:	add    %ch,(%rax)
+   18005e835:	xchg   %eax,%ebp
+   18005e836:	pop    %rax
+   18005e837:	data16 add %al,(%rax)
+   18005e83a:	add    %al,(%rax)
+   18005e83c:	or     $0x50000000,%eax
    18005e841:	add    (%rax),%eax
    18005e843:	add    %ah,(%rax)
    18005e845:	repnz add $0x5e62000,%eax
 	...
    18005e87f:	add    %dl,0x18005f5(%rax)
    18005e885:	add    %al,(%rax)
    18005e887:	add    %bl,0x18005f5(%rax)
```

## ipex_llm/libs/libgptneox_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180063368
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 29 15:03:49 2024
+Time/Date		Thu May 30 15:03:47 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063c00
 SizeOfInitializedData	00000000000c6a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000063368
@@ -129327,15 +129327,17 @@
    18006c037:	add    %al,%al
    18006c039:	push   %rsi
    18006c03a:	(bad)
    18006c03b:	addb   $0x0,(%rcx)
    18006c03e:	add    %al,(%rax)
    18006c040:	add    %al,(%rax)
    18006c042:	add    %al,(%rax)
-   18006c044:	{rex2 0x43} push %r15
+   18006c044:	push   %rbx
+   18006c045:	xchg   %eax,%ebp
+   18006c046:	pop    %rax
    18006c047:	data16 add %al,(%rax)
    18006c04a:	add    %al,(%rax)
    18006c04c:	or     $0x50000000,%eax
    18006c051:	add    (%rax),%eax
    18006c053:	add    %al,-0x437bfffa(%rsp,%rcx,8)
    18006c05a:	(bad)
 	...
```

## ipex_llm/libs/libgptneox_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005d228
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 29 15:03:05 2024
+Time/Date		Thu May 30 15:03:04 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005da00
 SizeOfInitializedData	00000000000c6600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005d228
@@ -123791,17 +123791,17 @@
    1800660dd:	add    %al,(%rax)
    1800660df:	add    %bh,0x18005f6(%rax)
    1800660e5:	add    %al,(%rax)
    1800660e7:	add    %al,%al
    1800660e9:	testb  $0x0,0x180(%rip)        # 0x180066270
    1800660f0:	add    %al,(%rax)
    1800660f2:	add    %al,(%rax)
-   1800660f4:	test   $0x665743,%eax
-   1800660f9:	add    %al,(%rax)
-   1800660fb:	add    %cl,0x50000000(%rip)        # 0x1d0066101
+   1800660f4:	sub    %dl,0x6658(%rbp)
+   1800660fa:	add    %al,(%rax)
+   1800660fc:	or     $0x50000000,%eax
    180066101:	add    (%rax),%eax
    180066103:	add    %al,0x5b840006(%rbp,%rbp,2)
    18006610a:	(bad)
 	...
    18006617f:	add    %bh,%al
    180066181:	jo     0x180066189
    180066183:	addb   $0x0,(%rcx)
```

## ipex_llm/libs/libllama_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180062078
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 29 15:03:49 2024
+Time/Date		Thu May 30 15:03:47 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000062800
 SizeOfInitializedData	00000000000c6600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000062078
@@ -128050,15 +128050,17 @@
    18006b114:	add    %eax,(%rax)
    18006b116:	add    %al,(%rax)
    18006b118:	rolb   $1,0x6(%rsi)
    18006b11b:	addb   $0x0,(%rcx)
    18006b11e:	add    %al,(%rax)
    18006b120:	add    %al,(%rax)
    18006b122:	add    %al,(%rax)
-   18006b124:	{rex2 0x43} push %r15
+   18006b124:	push   %rbx
+   18006b125:	xchg   %eax,%ebp
+   18006b126:	pop    %rax
    18006b127:	data16 add %al,(%rax)
    18006b12a:	add    %al,(%rax)
    18006b12c:	or     $0x50000000,%eax
    18006b131:	add    (%rax),%eax
    18006b133:	add    %al,-0x7ffff943(%rax)
    18006b139:	test   $0x6,%eax
 	...
```

## ipex_llm/libs/libllama_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005bf38
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 29 15:03:05 2024
+Time/Date		Thu May 30 15:03:04 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c600
 SizeOfInitializedData	00000000000c6200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005bf38
@@ -122524,17 +122524,20 @@
    1800651c0:	enter  $0x5e6,$0x80
    1800651c4:	add    %eax,(%rax)
    1800651c6:	add    %al,(%rax)
    1800651c8:	shl    $1,%dh
    1800651ca:	add    $0x180,%eax
    1800651cf:	add    %al,(%rax)
    1800651d1:	add    %al,(%rax)
-   1800651d3:	add    %ch,0x665743(%rcx)
-   1800651d9:	add    %al,(%rax)
-   1800651db:	add    %cl,0x50000000(%rip)        # 0x1d00651e1
+   1800651d3:	add    %ch,(%rax)
+   1800651d5:	xchg   %eax,%ebp
+   1800651d6:	pop    %rax
+   1800651d7:	data16 add %al,(%rax)
+   1800651da:	add    %al,(%rax)
+   1800651dc:	or     $0x50000000,%eax
    1800651e1:	add    (%rax),%eax
    1800651e3:	add    %al,(%rax)
    1800651e5:	pop    %rsi
    1800651e6:	(bad)
    1800651e7:	add    %al,(%rax)
    1800651e9:	rex.W (bad)
 	...
```

## ipex_llm/libs/libstarcoder_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800694d8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 29 15:03:48 2024
+Time/Date		Thu May 30 15:03:47 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000069c00
 SizeOfInitializedData	00000000000c8400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000694d8
@@ -138525,16 +138525,17 @@
    180072c85:	add    %al,(%rax)
    180072c87:	add    %al,%al
    180072c89:	mov    $0x6,%dh
    180072c8b:	addb   $0x0,(%rcx)
    180072c8e:	add    %al,(%rax)
    180072c90:	add    %al,(%rax)
    180072c92:	add    %al,(%rax)
-   180072c94:	(bad)
-   180072c95:	rex.XB push %r15
+   180072c94:	push   %rbx
+   180072c95:	xchg   %eax,%ebp
+   180072c96:	pop    %rax
    180072c97:	data16 add %al,(%rax)
    180072c9a:	add    %al,(%rax)
    180072c9c:	or     $0x50000000,%eax
    180072ca1:	add    (%rax),%eax
    180072ca3:	add    %dl,0x3e(%rax)
    180072ca6:	(bad)
    180072ca7:	add    %dl,0x2e(%rax)
```

## ipex_llm/libs/libstarcoder_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180063428
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 29 15:03:04 2024
+Time/Date		Thu May 30 15:03:04 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063a00
 SizeOfInitializedData	00000000000c8000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000063428
@@ -133117,17 +133117,15 @@
    18006cd57:	add    %al,%al
    18006cd59:	push   %rsi
    18006cd5a:	(bad)
    18006cd5b:	addb   $0x0,(%rcx)
    18006cd5e:	add    %al,(%rax)
    18006cd60:	add    %al,(%rax)
    18006cd62:	add    %al,(%rax)
-   18006cd64:	test   $0x43,%al
-   18006cd66:	push   %rdi
-   18006cd67:	data16 add %al,(%rax)
+   18006cd64:	sub    %dl,0x6658(%rbp)
    18006cd6a:	add    %al,(%rax)
    18006cd6c:	or     $0x50000000,%eax
    18006cd71:	add    (%rax),%eax
    18006cd73:	add    %dl,%al
    18006cd75:	fiadds (%rsi)
    18006cd77:	add    %dl,%al
    18006cd79:	int3
```

## ipex_llm/libs/llama-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002dac
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 29 15:02:40 2024
+Time/Date		Thu May 30 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002800
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002dac
@@ -5355,16 +5355,16 @@
    180004a20:	cmp    %al,0x0(%rdx)
    180004a23:	addb   $0x0,(%rcx)
    180004a26:	add    %al,(%rax)
    180004a28:	rex
    180004a29:	rex.X add %al,0x1(%rax)
    180004a30:	add    %al,(%rax)
    180004a32:	add    %al,(%rax)
-   180004a34:	nop
-   180004a35:	rex.XB push %r15
+   180004a34:	adc    $0x95,%al
+   180004a36:	pop    %rax
    180004a37:	data16 add %al,(%rax)
    180004a3a:	add    %al,(%rax)
    180004a3c:	or     $0xe0000000,%eax
    180004a41:	add    (%rax),%al
    180004a43:	add    %ah,%ah
    180004a45:	rex.WR add %r8b,(%rax)
    180004a48:	in     $0x38,%al
```

## ipex_llm/libs/llama.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005bd28
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 29 15:02:41 2024
+Time/Date		Thu May 30 15:02:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c400
 SizeOfInitializedData	00000000000c6200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005bd28
@@ -122360,15 +122360,15 @@
    1800651e0:	enter  $0x5e6,$0x80
    1800651e4:	add    %eax,(%rax)
    1800651e6:	add    %al,(%rax)
    1800651e8:	shl    $1,%dh
    1800651ea:	add    $0x180,%eax
    1800651ef:	add    %al,(%rax)
    1800651f1:	add    %al,(%rax)
-   1800651f3:	add    %dl,0x665743(%rcx)
+   1800651f3:	add    %dl,0x665895(%rip)        # 0x1806caa8e
    1800651f9:	add    %al,(%rax)
    1800651fb:	add    %cl,0x50000000(%rip)        # 0x1d0065201
    180065201:	add    (%rax),%eax
    180065203:	add    %al,-0x7ffff9a2(%rax)
    180065209:	rex.RX (bad)
 	...
    18006527f:	add    %dh,%al
```

## ipex_llm/libs/main-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001045c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Wed May 29 15:02:40 2024
+Time/Date		Thu May 30 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010800
 SizeOfInitializedData	0000000000008e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001045c
@@ -25509,16 +25509,16 @@
    140014ab0:	enter  $0x125,$0x40
    140014ab4:	add    %eax,(%rax)
    140014ab6:	add    %al,(%rax)
    140014ab8:	shlb   $1,0x14001(%rip)        # 0x140028abf
    140014abe:	add    %al,(%rax)
    140014ac0:	add    %al,(%rax)
    140014ac2:	add    %al,(%rax)
-   140014ac4:	nop
-   140014ac5:	rex.XB push %r15
+   140014ac4:	adc    $0x95,%al
+   140014ac6:	pop    %rax
    140014ac7:	data16 add %al,(%rax)
    140014aca:	add    %al,(%rax)
    140014acc:	or     $0x20000000,%eax
    140014ad1:	add    (%rax),%eax
    140014ad3:	add    %cl,%ah
    140014ad5:	push   %rsp
    140014ad6:	add    %eax,(%rax)
```

## ipex_llm/libs/main-chatglm_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400836cc
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Wed May 29 15:03:38 2024
+Time/Date		Thu May 30 15:03:37 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000087c00
 SizeOfInitializedData	00000000000cc000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000836cc
@@ -189033,16 +189033,16 @@
    140093fa5:	add    %al,(%rax)
    140093fa7:	add    %al,(%rax)
    140093fa9:	cltd
    140093faa:	or     %al,0x1(%rax)
    140093fad:	add    %al,(%rax)
    140093faf:	add    %al,(%rax)
    140093fb1:	add    %al,(%rax)
-   140093fb3:	add    %cl,%dl
-   140093fb5:	rex.XB push %r15
+   140093fb3:	add    %cl,-0x6b(%rcx)
+   140093fb6:	pop    %rax
    140093fb7:	data16 add %al,(%rax)
    140093fba:	add    %al,(%rax)
    140093fbc:	or     $0xcc000000,%eax
    140093fc1:	add    (%rax),%eax
    140093fc3:	add    %dl,(%rax)
    140093fc5:	je     0x140093fd0
    140093fc7:	add    %dl,(%rax)
```

## ipex_llm/libs/main-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000ef6c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Wed May 29 15:02:40 2024
+Time/Date		Thu May 30 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f200
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000ef6c
@@ -24136,16 +24136,16 @@
    140013edf:	add    %ch,%al
    140013ee1:	adc    $0x14001,%eax
    140013ee6:	add    %al,(%rax)
    140013ee8:	lock adc $0x14001,%eax
    140013eee:	add    %al,(%rax)
    140013ef0:	add    %al,(%rax)
    140013ef2:	add    %al,(%rax)
-   140013ef4:	nop
-   140013ef5:	rex.XB push %r15
+   140013ef4:	adc    $0x95,%al
+   140013ef6:	pop    %rax
    140013ef7:	data16 add %al,(%rax)
    140013efa:	add    %al,(%rax)
    140013efc:	or     $0x90000000,%eax
    140013f01:	add    (%rax),%eax
    140013f03:	add    %ch,0x1(%rcx,%rcx,2)
    140013f07:	add    %ch,0x1(%rdi,%rbp,1)
 	...
```

## ipex_llm/libs/main-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000f32c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Wed May 29 15:02:40 2024
+Time/Date		Thu May 30 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f600
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000f32c
@@ -24679,16 +24679,16 @@
    140013faf:	add    %ch,%al
    140013fb1:	adc    $0x14001,%eax
    140013fb6:	add    %al,(%rax)
    140013fb8:	lock adc $0x14001,%eax
    140013fbe:	add    %al,(%rax)
    140013fc0:	add    %al,(%rax)
    140013fc2:	add    %al,(%rax)
-   140013fc4:	nop
-   140013fc5:	rex.XB push %r15
+   140013fc4:	adc    $0x95,%al
+   140013fc6:	pop    %rax
    140013fc7:	data16 add %al,(%rax)
    140013fca:	add    %al,(%rax)
    140013fcc:	or     $0x90000000,%eax
    140013fd1:	add    (%rax),%eax
    140013fd3:	add    %ch,%ah
    140013fd5:	add    %rax,(%r8)
    140013fd8:	in     (%dx),%al
```

## ipex_llm/libs/main-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001a85c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Wed May 29 15:02:40 2024
+Time/Date		Thu May 30 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000001b000
 SizeOfInitializedData	000000000000bc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001a85c
@@ -40341,17 +40341,17 @@
    14001f111:	movb   $0x40,(%rcx)
    14001f114:	add    %eax,(%rax)
    14001f116:	add    %al,(%rax)
    14001f118:	push   $0x14001c6
    14001f11d:	add    %al,(%rax)
    14001f11f:	add    %al,(%rax)
    14001f121:	add    %al,(%rax)
-   14001f123:	add    %dl,0x665743(%rax)
-   14001f129:	add    %al,(%rax)
-   14001f12b:	add    %cl,0x20000000(%rip)        # 0x16001f131
+   14001f123:	add    %dl,0x6658(,%rdx,4)
+   14001f12a:	add    %al,(%rax)
+   14001f12c:	or     $0x20000000,%eax
    14001f131:	add    (%rax),%eax
    14001f133:	add    %dl,(%rbx,%rax,1)
    14001f136:	add    (%rax),%al
    14001f138:	adc    $0xf7,%al
    14001f13a:	add    %eax,(%rax)
 	...
    14001f180:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013918
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Wed May 29 15:02:40 2024
+Time/Date		Thu May 30 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013a00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013918
@@ -32234,17 +32234,17 @@
    140019225:	add    %al,(%rax)
    140019227:	add    %al,(%rax)
    140019229:	push   %rbp
    14001922a:	add    %eax,0x1(%rax)
    14001922d:	add    %al,(%rax)
    14001922f:	add    %al,(%rax)
    140019231:	add    %al,(%rax)
-   140019233:	add    %dl,0x665743(%rax)
-   140019239:	add    %al,(%rax)
-   14001923b:	add    %cl,0x20000000(%rip)        # 0x160019241
+   140019233:	add    %dl,0x6658(,%rdx,4)
+   14001923a:	add    %al,(%rax)
+   14001923c:	or     $0x20000000,%eax
    140019241:	add    (%rax),%eax
    140019243:	add    %dh,%al
    140019245:	movabs 0x18ff00001,%eax
 	...
    14001927e:	add    %al,(%rax)
    140019280:	add    %eax,(%rax)
 	...
```

## ipex_llm/libs/quantize-bloom_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013b28
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Wed May 29 15:03:04 2024
+Time/Date		Thu May 30 15:03:03 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ad000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013b28
@@ -32372,17 +32372,20 @@
    140019205:	add    %al,(%rax)
    140019207:	add    %al,(%rax)
    140019209:	push   %rbp
    14001920a:	add    %eax,0x1(%rax)
    14001920d:	add    %al,(%rax)
    14001920f:	add    %al,(%rax)
    140019211:	add    %al,(%rax)
-   140019213:	add    %ch,0x665743(%rax)
-   140019219:	add    %al,(%rax)
-   14001921b:	add    %cl,0x20000000(%rip)        # 0x160019221
+   140019213:	add    %ah,(%rdi)
+   140019215:	xchg   %eax,%ebp
+   140019216:	pop    %rax
+   140019217:	data16 add %al,(%rax)
+   14001921a:	add    %al,(%rax)
+   14001921c:	or     $0x20000000,%eax
    140019221:	add    (%rax),%eax
    140019223:	add    %dh,%al
    140019225:	movabs 0x191f00001,%eax
 	...
    14001927e:	add    %al,(%rax)
    140019280:	add    %eax,(%rax)
 	...
```

## ipex_llm/libs/quantize-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010988
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Wed May 29 15:02:39 2024
+Time/Date		Thu May 30 15:02:43 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010a00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010988
@@ -27181,17 +27181,20 @@
    140016020:	push   $0x1400123
    140016025:	add    %al,(%rax)
    140016027:	add    %dh,0x23(%rax)
    14001602a:	add    %eax,0x1(%rax)
    14001602d:	add    %al,(%rax)
    14001602f:	add    %al,(%rax)
    140016031:	add    %al,(%rax)
-   140016033:	add    %cl,0x665743(%rdi)
-   140016039:	add    %al,(%rax)
-   14001603b:	add    %cl,-0x70000000(%rip)        # 0xd0016041
+   140016033:	add    %dl,(%rbx)
+   140016035:	xchg   %eax,%ebp
+   140016036:	pop    %rax
+   140016037:	data16 add %al,(%rax)
+   14001603a:	add    %al,(%rax)
+   14001603c:	or     $0x90000000,%eax
    140016041:	add    (%rax),%eax
    140016043:	add    %ch,%al
    140016045:	add    %eax,%gs:(%rax)
    140016048:	call   0x1400161a0
 	...
    14001607d:	add    %al,(%rax)
    14001607f:	add    %bl,0x1400169(%rax)
```

## ipex_llm/libs/quantize-gptneox_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010b98
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Wed May 29 15:03:03 2024
+Time/Date		Thu May 30 15:03:02 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010c00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010b98
@@ -27311,17 +27311,20 @@
    140016000:	push   $0x1400123
    140016005:	add    %al,(%rax)
    140016007:	add    %dh,0x23(%rax)
    14001600a:	add    %eax,0x1(%rax)
    14001600d:	add    %al,(%rax)
    14001600f:	add    %al,(%rax)
    140016011:	add    %al,(%rax)
-   140016013:	add    %ah,0x665743(%rdi)
-   140016019:	add    %al,(%rax)
-   14001601b:	add    %cl,-0x70000000(%rip)        # 0xd0016021
+   140016013:	add    %ah,(%rsi)
+   140016015:	xchg   %eax,%ebp
+   140016016:	pop    %rax
+   140016017:	data16 add %al,(%rax)
+   14001601a:	add    %al,(%rax)
+   14001601c:	or     $0x90000000,%eax
    140016021:	add    (%rax),%eax
    140016023:	add    %ch,%al
    140016025:	add    %eax,%gs:(%rax)
    140016028:	call   0x140016182
 	...
    14001607d:	add    %al,(%rax)
    14001607f:	add    %bl,0x1400169(%rax)
```

## ipex_llm/libs/quantize-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400118e8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Wed May 29 15:02:39 2024
+Time/Date		Thu May 30 15:02:43 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011800
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000118e8
@@ -28460,17 +28460,20 @@
    1400170ed:	add    %al,(%rax)
    1400170ef:	add    %cl,0x1400133(%rax)
    1400170f5:	add    %al,(%rax)
    1400170f7:	add    %dl,0x1400133(%rax)
    1400170fd:	add    %al,(%rax)
    1400170ff:	add    %al,(%rax)
    140017101:	add    %al,(%rax)
-   140017103:	add    %cl,0x665743(%rdi)
-   140017109:	add    %al,(%rax)
-   14001710b:	add    %cl,-0x70000000(%rip)        # 0xd0017111
+   140017103:	add    %dl,(%rbx)
+   140017105:	xchg   %eax,%ebp
+   140017106:	pop    %rax
+   140017107:	data16 add %al,(%rax)
+   14001710a:	add    %al,(%rax)
+   14001710c:	or     $0x90000000,%eax
    140017111:	add    (%rax),%eax
    140017113:	add    %ch,%ah
    140017115:	jbe    0x140017118
    140017117:	add    %ch,%ah
    140017119:	(bad)
 	...
    14001717e:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-llama_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140011af8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Wed May 29 15:03:03 2024
+Time/Date		Thu May 30 15:03:02 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011c00
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000011af8
@@ -28609,17 +28609,20 @@
    1400170cd:	add    %al,(%rax)
    1400170cf:	add    %cl,0x1400133(%rax)
    1400170d5:	add    %al,(%rax)
    1400170d7:	add    %dl,0x1400133(%rax)
    1400170dd:	add    %al,(%rax)
    1400170df:	add    %al,(%rax)
    1400170e1:	add    %al,(%rax)
-   1400170e3:	add    %ah,0x665743(%rdi)
-   1400170e9:	add    %al,(%rax)
-   1400170eb:	add    %cl,-0x70000000(%rip)        # 0xd00170f1
+   1400170e3:	add    %ah,(%rsi)
+   1400170e5:	xchg   %eax,%ebp
+   1400170e6:	pop    %rax
+   1400170e7:	data16 add %al,(%rax)
+   1400170ea:	add    %al,(%rax)
+   1400170ec:	or     $0x90000000,%eax
    1400170f1:	add    (%rax),%eax
    1400170f3:	add    %ch,0x1(%rsi,%rsi,2)
    1400170f7:	add    %ch,0x1(%rsi,%riz,2)
    1400170fb:	add    %al,(%rax)
    1400170fd:	add    %al,(%rax)
    1400170ff:	add    %ah,(%rax)
    140017101:	jp     0x140017104
```

## ipex_llm/libs/quantize-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013c70
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Wed May 29 15:02:40 2024
+Time/Date		Thu May 30 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013c70
@@ -32579,17 +32579,17 @@
    140019325:	add    %al,(%rax)
    140019327:	add    %al,(%rax)
    140019329:	push   %rbp
    14001932a:	add    %eax,0x1(%rax)
    14001932d:	add    %al,(%rax)
    14001932f:	add    %al,(%rax)
    140019331:	add    %al,(%rax)
-   140019333:	add    %dl,0x665743(%rax)
-   140019339:	add    %al,(%rax)
-   14001933b:	add    %cl,0x20000000(%rip)        # 0x160019341
+   140019333:	add    %dl,0x6658(,%rdx,4)
+   14001933a:	add    %al,(%rax)
+   14001933c:	or     $0x20000000,%eax
    140019341:	add    (%rax),%eax
    140019343:	add    %bh,%ah
    140019345:	movabs %al,0x192fc0001
 	...
    14001937e:	add    %al,(%rax)
    140019380:	add    %eax,(%rax)
 	...
```

## ipex_llm/libs/quantize-starcoder_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013e80
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Wed May 29 15:03:04 2024
+Time/Date		Thu May 30 15:03:03 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013e00
 SizeOfInitializedData	00000000000ad200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013e80
@@ -32702,17 +32702,20 @@
    140019305:	add    %al,(%rax)
    140019307:	add    %al,(%rax)
    140019309:	push   %rbp
    14001930a:	add    %eax,0x1(%rax)
    14001930d:	add    %al,(%rax)
    14001930f:	add    %al,(%rax)
    140019311:	add    %al,(%rax)
-   140019313:	add    %ch,0x665743(%rax)
-   140019319:	add    %al,(%rax)
-   14001931b:	add    %cl,0x20000000(%rip)        # 0x160019321
+   140019313:	add    %ah,(%rdi)
+   140019315:	xchg   %eax,%ebp
+   140019316:	pop    %rax
+   140019317:	data16 add %al,(%rax)
+   14001931a:	add    %al,(%rax)
+   14001931c:	or     $0x20000000,%eax
    140019321:	add    (%rax),%eax
    140019323:	add    %bh,%ah
    140019325:	movabs %al,0x194fc0001
 	...
    14001937e:	add    %al,(%rax)
    140019380:	add    %eax,(%rax)
 	...
```

## ipex_llm/libs/starcoder-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018000277c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 29 15:02:40 2024
+Time/Date		Thu May 30 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002200
 SizeOfInitializedData	0000000000003400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000277c
@@ -4028,16 +4028,16 @@
    1800045f0:	cmp    %al,0x0(%rdx)
    1800045f3:	addb   $0x0,(%rcx)
    1800045f6:	add    %al,(%rax)
    1800045f8:	rex
    1800045f9:	rex.X add %al,0x1(%rax)
    180004600:	add    %al,(%rax)
    180004602:	add    %al,(%rax)
-   180004604:	nop
-   180004605:	rex.XB push %r15
+   180004604:	adc    $0x95,%al
+   180004606:	pop    %rax
    180004607:	data16 add %al,(%rax)
    18000460a:	add    %al,(%rax)
    18000460c:	or     $0xe0000000,%eax
    180004611:	add    (%rax),%al
    180004613:	add    %ah,%ah
    180004615:	rex.W add %al,(%rax)
    180004618:	in     $0x2e,%al
```

## ipex_llm/libs/starcoder.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180063218
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 29 15:02:40 2024
+Time/Date		Thu May 30 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063800
 SizeOfInitializedData	00000000000c8000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000063218
@@ -133011,16 +133011,16 @@
    18006cd77:	add    %al,%al
    18006cd79:	push   %rsi
    18006cd7a:	(bad)
    18006cd7b:	addb   $0x0,(%rcx)
    18006cd7e:	add    %al,(%rax)
    18006cd80:	add    %al,(%rax)
    18006cd82:	add    %al,(%rax)
-   18006cd84:	nop
-   18006cd85:	rex.XB push %r15
+   18006cd84:	adc    $0x95,%al
+   18006cd86:	pop    %rax
    18006cd87:	data16 add %al,(%rax)
    18006cd8a:	add    %al,(%rax)
    18006cd8c:	or     $0x50000000,%eax
    18006cd91:	add    (%rax),%eax
    18006cd93:	add    %dl,-0x21(%rax)
    18006cd96:	(bad)
    18006cd97:	add    %dl,-0x35(%rax)
```

## ipex_llm/serving/fastchat/tgi_api_server.py

```diff
@@ -603,73 +603,14 @@
                 continue
             yield f"data: {json.dumps(chunk.model_dump(exclude_unset=True), ensure_ascii=False)}\n\n"
     # There is not "content" field in the last delta message, so exclude_none to exclude field "content".
     for finish_chunk in finish_stream_events:
         yield f"data: {json.dumps(chunk.model_dump(exclude_unset=True), ensure_ascii=False)}\n\n"
     yield "data: [DONE]\n\n"
 
-async def generate_completion_stream_generator(
-    request: CompletionRequest, n: int, worker_addr: str
-):
-    model_name = request.model
-    id = f"cmpl-{shortuuid.random()}"
-    finish_stream_events = []
-    for text in request.prompt:
-        for i in range(n):
-            previous_text = ""
-            gen_params = await get_gen_params(
-                request.model,
-                worker_addr,
-                text,
-                temperature=request.temperature,
-                top_p=request.top_p,
-                top_k=request.top_k,
-                presence_penalty=request.presence_penalty,
-                frequency_penalty=request.frequency_penalty,
-                max_tokens=request.max_tokens,
-                logprobs=request.logprobs,
-                echo=request.echo,
-                stop=request.stop,
-            )
-            async for content in generate_completion_stream(gen_params, worker_addr):
-                if content["error_code"] != 0:
-                    yield f"data: {json.dumps(chunk.model_dump(exclude_unset=True), ensure_ascii=False)}\n\n"
-                    yield "data: [DONE]\n\n"
-                    return
-                decoded_unicode = content["text"].replace("\ufffd", "")
-                delta_text = decoded_unicode[len(previous_text) :]
-                previous_text = (
-                    decoded_unicode
-                    if len(decoded_unicode) > len(previous_text)
-                    else previous_text
-                )
-                # todo: index is not apparent
-                choice_data = CompletionResponseStreamChoice(
-                    index=i,
-                    text=delta_text,
-                    logprobs=create_openai_logprobs(content.get("logprobs", None)),
-                    finish_reason=content.get("finish_reason", None),
-                )
-                chunk = CompletionStreamResponse(
-                    id=id,
-                    object="text_completion",
-                    choices=[choice_data],
-                    model=model_name,
-                )
-                if len(delta_text) == 0:
-                    if content.get("finish_reason", None) is not None:
-                        finish_stream_events.append(chunk)
-                    continue
-                yield f"data: {json.dumps(chunk.model_dump(exclude_unset=True), ensure_ascii=False)}\n\n"
-    # There is not "content" field in the last delta message, so exclude_none to exclude field "content".
-    for finish_chunk in finish_stream_events:
-        yield f"data: {json.dumps(chunk.model_dump(exclude_unset=True), ensure_ascii=False)}\n\n"
-    yield "data: [DONE]\n\n"
-
-
 async def generate_completion_stream(payload: Dict[str, Any], worker_addr: str):
     controller_address = app_settings.controller_address
     async with httpx.AsyncClient() as client:
         delimiter = b"\0"
         async with client.stream(
             "POST",
             worker_addr + "/worker_generate_stream",
```

## ipex_llm/transformers/convert.py

```diff
@@ -49,14 +49,15 @@
 from ipex_llm.utils.common import invalidInputError
 from typing import List, Optional, Tuple, Union
 from types import MethodType
 import subprocess
 import sys
 
 _IS_VLLM_AVAILABLE = None
+_USE_VLLM = False
 
 
 def is_auto_gptq_available():
     return importlib.util.find_spec("auto_gptq") is not None
 
 
 def is_auto_awq_available():
@@ -72,14 +73,18 @@
     if 'vllm' in installed_packages:
         _IS_VLLM_AVAILABLE = True
     else:
         _IS_VLLM_AVAILABLE = False
     return _IS_VLLM_AVAILABLE
 
 
+def get_use_vllm():
+    return _USE_VLLM
+
+
 def is_torch_distributed_initialized():
     return torch.distributed.is_initialized()
 
 
 def is_module_in_classes(module, classes):
     return any(isinstance(module, cls) for cls in classes)
 
@@ -115,22 +120,23 @@
 def is_gptq_linear(module):
     return is_auto_gptq_available() and \
         (isinstance(module, QuantLinearCuda) or isinstance(module, QuantLinearCudaOld))
 
 
 def is_linear_module(module):
 
+    global _USE_VLLM
+
     in_features = None
     out_features = None
     mp_group = None
 
     is_awq = is_auto_awq_available() and isinstance(module, WQLinear_GEMM)
-
     if is_vllm_available():
-        # TODO: add tensor parallel feature later
+        # Only convert vllm modules
         from vllm.model_executor.layers.linear import (
             ColumnParallelLinear, RowParallelLinear, QKVParallelLinear, MergedColumnParallelLinear
         )
         from vllm.model_executor.parallel_utils.parallel_state import (
             get_tensor_model_parallel_group,
             get_tensor_model_parallel_world_size
         )
@@ -144,24 +150,17 @@
             mp_group = None
             tp_size = get_tensor_model_parallel_world_size()
             if isinstance(module, RowParallelLinear) and tp_size >= 2:
                 mp_group = get_tensor_model_parallel_group()
                 in_features = module.input_size_per_partition
             elif isinstance(module, ColumnParallelLinear) and tp_size >= 2:
                 out_features = module.output_size_per_partition
-        else:
-            # Also check for Linear module
-            if isinstance(module, nn.Linear) or is_awq:
-                in_features = module.in_features
-                out_features = module.out_features
-                mp_group = None
-                result = True
-            else:
-                result = False
-    elif is_gptq_linear(module):
+            _USE_VLLM = True
+            return result, (in_features, out_features, mp_group)
+    if is_gptq_linear(module):
         in_features = module.infeatures
         out_features = module.outfeatures
         mp_group = None
         result = True
     elif isinstance(module, nn.Linear) or is_awq:
         in_features = module.in_features
         out_features = module.out_features
@@ -484,28 +483,33 @@
 def replace_with_low_bit_linear_for_module(model, qtype, module_name=None,
                                            modules_to_not_convert=None, current_key_name=None,
                                            convert_shape_only=False, torch_dtype="auto"):
     from ipex_llm.transformers.low_bit_linear import LowBitLinear, FP4Params, \
         FP16Linear, BF16Linear
     has_been_replaced = False
 
+    splits = []
     if "." in module_name:
         splits = module_name.split(".")
-    parent_module = getattr(model, splits[0])
-
-    if "lm_head" not in module_name:
-        for split in splits[1:-2]:
-            new_module = getattr(parent_module, split)
-            parent_module = new_module
-        module = getattr(parent_module, splits[-2])
-        module_name = splits[-2]
+    if not splits:
+        invalidInputError(False,
+                          "Please provide a valid module_name with hierarchical structure")
     else:
-        module = parent_module
-        parent_module = model
-        module_name = splits[0]
+        parent_module = getattr(model, splits[0])
+
+        if "lm_head" not in module_name:
+            for split in splits[1:-2]:
+                new_module = getattr(parent_module, split)
+                parent_module = new_module
+            module = getattr(parent_module, splits[-2])
+            module_name = splits[-2]
+        else:
+            module = parent_module
+            parent_module = model
+            module_name = splits[0]
 
     if current_key_name is None:
         current_key_name = []
 
     if modules_to_not_convert is None:
         modules_to_not_convert = []
```

## ipex_llm/transformers/low_bit_linear.py

```diff
@@ -49,15 +49,15 @@
 import torch.nn.functional as F
 from torch import Tensor, device, dtype, nn
 from operator import mul
 from functools import reduce
 from ipex_llm.transformers.xpu_customize_fwd import custom_fwd, custom_bwd
 from ipex_llm.transformers.utils import get_autocast_dtype, get_xpu_device_type, \
     get_ipex_version
-from ipex_llm.transformers.convert import is_deepspeed_available, is_vllm_available
+from ipex_llm.transformers.convert import is_deepspeed_available, get_use_vllm
 
 T = TypeVar("T", bound="torch.nn.Module")
 
 import ipex_llm.ggml.model.llama.llama_cpp as ggml
 import ctypes
 from ipex_llm.ggml.quantize import ggml_tensor_qtype
 
@@ -733,20 +733,19 @@
                     else:
                         result = xe_linear.forward_new(x_2d, self.weight.data, self.weight.qtype,
                                                        input_seq_size)
                 if do_empty_cache:
                     torch.xpu.empty_cache()
             result = result.view(new_shape)
             if self.mp_group is not None:
-                # FIXME: the user may install both vllm and deepspeed
-                if is_deepspeed_available():
+                if get_use_vllm():
+                    torch.distributed.all_reduce(result, group=self.mp_group)
+                elif is_deepspeed_available():
                     from deepspeed import comm as dist
                     dist.inference_all_reduce(result, group=self.mp_group)
-                elif is_vllm_available():
-                    torch.distributed.all_reduce(result, group=self.mp_group)
                 else:
                     invalidInputError(False, "mp_group is not None, but no supported backend found")
             if self.bias is not None:
                 result += self.bias
         else:
             # CPU logic
             # todo may need to set a different number on different platforms
@@ -818,19 +817,19 @@
                 result = F.linear(x, self.weight, self.bias)
             else:
                 if self.weight_type == 1:
                     self.weight = self.weight.transpose(0, 1).contiguous()
                     self.weight_type = 2
                 result = torch.ops.torch_ipex.matmul_bias_out(x, self.weight, self.bias)
             if self.mp_group is not None:
-                if is_deepspeed_available():
+                if get_use_vllm():
+                    torch.distributed.all_reduce(result, group=self.mp_group)
+                elif is_deepspeed_available():
                     from deepspeed import comm as dist
                     dist.inference_all_reduce(result, group=self.mp_group)
-                elif is_vllm_available():
-                    torch.distributed.all_reduce(result, group=self.mp_group)
                 else:
                     invalidInputError(False, "mp_group is not None, but no supported backend found")
             return result
         else:
             if self.in_len == 4096 and self.weight_type != 3 or \
                     self.in_len == 11008 and self.weight_type != 1:
                 # convert weight first to use esimd fp16 kernel
@@ -855,19 +854,19 @@
                 import xe_batch
                 result = xe_batch.batch_forward(x_2d, self.weight.data,
                                                 self.qtype)
 
             new_shape = x_shape[:-1] + (self.out_len,)
             result = result.view(new_shape)
             if self.mp_group is not None:
-                if is_deepspeed_available():
+                if get_use_vllm():
+                    torch.distributed.all_reduce(result, group=self.mp_group)
+                elif is_deepspeed_available():
                     from deepspeed import comm as dist
                     dist.inference_all_reduce(result, group=self.mp_group)
-                elif is_vllm_available():
-                    torch.distributed.all_reduce(result, group=self.mp_group)
                 else:
                     invalidInputError(False, "mp_group is not None, but no supported backend found")
             if self.bias is not None:
                 result += self.bias
 
             return result.to(x.dtype)
```

## Comparing `ipex_llm-2.1.0b20240529.data/scripts/ipex-llm-init.bat` & `ipex_llm-2.1.0b20240530.data/scripts/ipex-llm-init.bat`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240529.data/scripts/llm-chat.ps1` & `ipex_llm-2.1.0b20240530.data/scripts/llm-chat.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240529.data/scripts/llm-cli.ps1` & `ipex_llm-2.1.0b20240530.data/scripts/llm-cli.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240529.dist-info/METADATA` & `ipex_llm-2.1.0b20240530.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipex-llm
-Version: 2.1.0b20240529
+Version: 2.1.0b20240530
 Summary: Large Language Model Develop Toolkit
 Home-page: https://github.com/intel-analytics/ipex-llm
 Author: BigDL Authors
 Author-email: bigdl-user-group@googlegroups.com
 License: Apache License, Version 2.0
 Platform: windows
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,15 +22,15 @@
 Requires-Dist: tokenizers (==0.15.2) ; extra == 'all'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'all'
 Requires-Dist: tabulate ; extra == 'all'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'all'
 Requires-Dist: torch (==2.1.2+cpu) ; (platform_system == "Linux") and extra == 'all'
 Requires-Dist: torch (==2.1.2) ; (platform_system == "Windows") and extra == 'all'
 Provides-Extra: cpp
-Requires-Dist: bigdl-core-cpp (==2.5.0b20240529) ; extra == 'cpp'
+Requires-Dist: bigdl-core-cpp (==2.5.0b20240530) ; extra == 'cpp'
 Requires-Dist: dpcpp-cpp-rt (==2024.0.2) ; (platform_system == "Windows") and extra == 'cpp'
 Requires-Dist: mkl-dpcpp (==2024.0.0) ; (platform_system == "Windows") and extra == 'cpp'
 Requires-Dist: onednn (==2024.0.0) ; (platform_system == "Windows") and extra == 'cpp'
 Provides-Extra: llama-index
 Requires-Dist: py-cpuinfo ; extra == 'llama-index'
 Requires-Dist: protobuf ; extra == 'llama-index'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'llama-index'
@@ -58,34 +58,34 @@
 Requires-Dist: tokenizers (==0.15.2) ; extra == 'xpu'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu'
 Requires-Dist: tabulate ; extra == 'xpu'
 Requires-Dist: setuptools (<70.0.0) ; extra == 'xpu'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240529) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-batch-21 (==2.5.0b20240529) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-addons-21 (==2.5.0b20240529) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240530) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-batch-21 (==2.5.0b20240530) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-addons-21 (==2.5.0b20240530) ; extra == 'xpu'
 Provides-Extra: xpu-2-1
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-1'
 Requires-Dist: protobuf ; extra == 'xpu-2-1'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-1'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-1'
 Requires-Dist: transformers (==4.36.2) ; extra == 'xpu-2-1'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-1'
 Requires-Dist: tokenizers (==0.15.2) ; extra == 'xpu-2-1'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-1'
 Requires-Dist: tabulate ; extra == 'xpu-2-1'
 Requires-Dist: setuptools (<70.0.0) ; extra == 'xpu-2-1'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240529) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-batch-21 (==2.5.0b20240529) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-addons-21 (==2.5.0b20240529) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240530) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-batch-21 (==2.5.0b20240530) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-addons-21 (==2.5.0b20240530) ; extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-1'
 Requires-Dist: dpcpp-cpp-rt (==2024.0.2) ; (platform_system == "Windows") and extra == 'xpu-2-1'
 Requires-Dist: mkl-dpcpp (==2024.0.0) ; (platform_system == "Windows") and extra == 'xpu-2-1'
 Requires-Dist: onednn (==2024.0.0) ; (platform_system == "Windows") and extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu'
 Requires-Dist: dpcpp-cpp-rt (==2024.0.2) ; (platform_system == "Windows") and extra == 'xpu'
 Requires-Dist: mkl-dpcpp (==2024.0.0) ; (platform_system == "Windows") and extra == 'xpu'
```

## Comparing `ipex_llm-2.1.0b20240529.dist-info/RECORD` & `ipex_llm-2.1.0b20240530.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -40,67 +40,67 @@
 ipex_llm/langchain/llms/__init__.py,sha256=vBCl9JF45vnk9CWBG1k8lp8J6F8OCR9UY2E-idkkm5Y,1636
 ipex_llm/langchain/llms/bigdlllm.py,sha256=FAZG6cAIJhRgbxm16gMq-cyBwLe-u165zE7yyxD7r9E,24438
 ipex_llm/langchain/llms/transformersllm.py,sha256=7eaIkJi1CbTCSgNxBCoZTe-o_5FYjD1GTYPWpn0Ccr4,10576
 ipex_llm/langchain/llms/transformerspipelinellm.py,sha256=vm522YPPwWxxAPVvQBtxRfBinC4hIbXdKW6VjHDaFXY,7379
 ipex_llm/langchain/vllm/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/langchain/vllm/vllm.py,sha256=6dxc-ZISZQrJilEa_HA827l75Dv9rcHpY_G6FdJ8BVs,7793
 ipex_llm/libs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ipex_llm/libs/bloom-api.dll,sha256=CXxyfQy7eBiJ5fT94n0mvp-qFxIBo0ADxum8iD86ML0,36352
-ipex_llm/libs/bloom.dll,sha256=WjnsuOxMVzW2FY9Z5jDBjzRNrr7K3IR2DC2h0BoX-1Y,472064
-ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=j3QguFm-PmqY86M9-vMRXblL98cfWUNUTZqs0Fg_zdI,854016
-ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=fdPnQQw7jx0xMw4-CQf_PLYErdLbLr_wugLX1_hZBPg,856576
-ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=6QQ5IeKPBgJqQR39RYDL_LZkBfiJQMi6fyNpnM86kv8,844800
-ipex_llm/libs/gptneox-api.dll,sha256=_fxWC1S5d_QXXcL3w1OL9_tZXYRgm2D9p8uVb2TvebA,24576
-ipex_llm/libs/gptneox.dll,sha256=Jtr7NLkm11Egx_xIJo6f9mm8vDPiRDMM_OxnKQu-xMA,531968
-ipex_llm/libs/libbloom_avx.dll,sha256=RXI33IZlRgcsUB3FkJhaft95y_TEu6hr3LI0PZJ3D2c,498688
-ipex_llm/libs/libbloom_vnni.dll,sha256=TgXb3CqSaDghFXh3jpN4ZqSpezn5SUb1qIFqnbwokok,472576
-ipex_llm/libs/libgptneox_avx.dll,sha256=AgW0PiyM8opPFzjEOE_A5BRZf5uDu9M6z6rUHm9m6cI,559104
-ipex_llm/libs/libgptneox_vnni.dll,sha256=zpCE0YQ_OSyjQ7dMgwXSD-jxJ2NBOfBOZABnYuZtp3U,532992
-ipex_llm/libs/libllama_avx.dll,sha256=HC88MLfrw4B2fQ5KN0nsquHOAVf3esnZN4yrTcRxENA,552960
-ipex_llm/libs/libllama_vnni.dll,sha256=n-O0ifd9kvHLCjeMrsXfkpE6mde-6JlBbt_5NxeLAxk,526848
-ipex_llm/libs/libstarcoder_avx.dll,sha256=L-WYsrI4OPzqXGHJuX6HE-6NZ8B_wRIaaTEo-DYssJI,590336
-ipex_llm/libs/libstarcoder_vnni.dll,sha256=EVjb1x1Xa2fD9MDCmLuwwWFPqVuNeImPSFCVp9koI2Q,564224
-ipex_llm/libs/llama-api.dll,sha256=GWfrJfLqWdJGaq8tZTCzl-AxDN_VZ8yGX-ZffCsH2t8,25088
-ipex_llm/libs/llama.dll,sha256=iSdhjAZfvbEEB7vHqpYJyl_-ZT8gSvDUCVM7i2PbQxg,526336
-ipex_llm/libs/main-bloom.exe,sha256=bxWK7X_AnQAAk6g2cw9JtgvINrL2ZZIuDIhuAK9Bf18,103424
-ipex_llm/libs/main-chatglm_vnni.exe,sha256=_tQfEM5nR-bBu9gXHuV8jlKObWctr0uwUa6ScAZb6kA,726528
-ipex_llm/libs/main-gptneox.exe,sha256=kPxDy-MwdqZu7h4Ut0wCzL3f_ayMEGQZV22cI2qsTHI,98816
-ipex_llm/libs/main-llama.exe,sha256=qHfyftbosjPgCCFUTRwOkA9fduSTquF7EzaNBYxR4cc,99840
-ipex_llm/libs/main-starcoder.exe,sha256=gfuR05Oyxh9mnvB-WauQyQizQXjX5_bj94qGLgEvFWk,157696
-ipex_llm/libs/quantize-bloom.exe,sha256=mVgRuEsVBotiPuJVndcIzem6PYwOTfQF-E3HF6S6I_A,126464
-ipex_llm/libs/quantize-bloom_vnni.exe,sha256=yLnVoqW42t6qwF8DZ25CxPdqKOvXzfymzrbkan7s_OY,127488
-ipex_llm/libs/quantize-gptneox.exe,sha256=JLw-NskblIedZaXrryyIPEltt8pPwwLJqTLzjs4ONig,103936
-ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=lueHhXsVnK1OTfDu0iq2yY4N4A9byVN52hhCHa74gbw,104448
-ipex_llm/libs/quantize-llama.exe,sha256=cYGx1lnce7ZrX2GMiwpjxrxtkx91QLgSNu5z9THLS_k,109056
-ipex_llm/libs/quantize-llama_vnni.exe,sha256=z-BBWPSg2i0AkncxYBwbkeecrPaT0f4pFme87qbB6jk,110080
-ipex_llm/libs/quantize-starcoder.exe,sha256=EkiSDQ0XFZaceBZMcqch06gK2ELzDFBTVqVYG7NP8oo,126976
-ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=YyYQeo5t41QqcyZmJmlJQMtbh_UYCX04gzcGplx2Mdk,128512
-ipex_llm/libs/starcoder-api.dll,sha256=0Kv29oasYQY3BUuTCImTaFejrGGgec3J3kxdqHjzgPM,21504
-ipex_llm/libs/starcoder.dll,sha256=HpvCFrguvNxIDtzOUoRYBVHW1NchFaAsBABH-uSPX4k,563712
+ipex_llm/libs/bloom-api.dll,sha256=XmCnjI5IDfs8mnIn27eXu9NDfTIugh_nxgeSKgaay08,36352
+ipex_llm/libs/bloom.dll,sha256=FcJnuYL-uJ-KmsIonbcUtJXZFZuYGytT_S6tqqY75hs,472064
+ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=-tvct_e1zGDBZ_RdjJ8Bv9LWvwFZJBNGNGDjCx36Xm4,854016
+ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=f3-HHvNvBo_qcSJwlwtP5jqQu-fH4zvp8ckc4_yLGZw,856576
+ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=7w4IlnOFrG1Ixp1-03E4IHgDgUBlZ6AVWO99rVJ3XcA,844800
+ipex_llm/libs/gptneox-api.dll,sha256=UBouwGkMX1_hOQwtV4F8s5GYzVP3ls4iG-c62j4xpDw,24576
+ipex_llm/libs/gptneox.dll,sha256=fTBH3K3ns7TEkZgHRh0dfAK1O_RBic6H-kmxuwWIfjY,531968
+ipex_llm/libs/libbloom_avx.dll,sha256=N8cbpDeKx1eyTNfmC_8MKG4VmMmjQrzsmOAGX09KOMk,498688
+ipex_llm/libs/libbloom_vnni.dll,sha256=YOo7nWlR5RYNlYdG_s196jlAd15yF00zRtft0cyzQd4,472576
+ipex_llm/libs/libgptneox_avx.dll,sha256=GlscI-MdcKdGTnuUXgHO290M0Y4LOw-ym94W8r99vAI,559104
+ipex_llm/libs/libgptneox_vnni.dll,sha256=wgnySI6frz4V1-THtImdr7NVVrv-a3I5GHLIaM6P3oQ,532992
+ipex_llm/libs/libllama_avx.dll,sha256=n6ATuGbj0R9LuXzkoT7VtlQhE2Xkvx5rJW4q5NujkEE,552960
+ipex_llm/libs/libllama_vnni.dll,sha256=CIEszEbeMGeKWlnt-SGouUhDN86onKl7ByhO3b4n9xk,526848
+ipex_llm/libs/libstarcoder_avx.dll,sha256=J-uSLEMeYy1-BrtTwYEa_KITKPH4asCQvnkpywS1N4U,590336
+ipex_llm/libs/libstarcoder_vnni.dll,sha256=iHqXA_fMmcwwyLYMkYzyh2vuS82HwS03XiEjyF7NfQY,564224
+ipex_llm/libs/llama-api.dll,sha256=vuP3M6Bt6HSeOzLnUVnFF0ImfGozRzP6b2XQ3OgNXrc,25088
+ipex_llm/libs/llama.dll,sha256=HNbhO9A6_FWSMtKRpDoi2SW4erVu9X3VGvWeSDaTSj0,526336
+ipex_llm/libs/main-bloom.exe,sha256=3nFNRpKoadFysOXAiO4xB4IdUWJldJdTADOD_anXE98,103424
+ipex_llm/libs/main-chatglm_vnni.exe,sha256=EJE43cah698-z3elH-NhBtgYahSB7Lc50U7upRwDtgQ,726528
+ipex_llm/libs/main-gptneox.exe,sha256=MNopq5l732JMjxL2ZZjLqE89FSPOPO6xb8UDBWeVTE8,98816
+ipex_llm/libs/main-llama.exe,sha256=R-p0_lQ1QsMbWbayy2twliQKRSD0faNhaJlrx6DVEu4,99840
+ipex_llm/libs/main-starcoder.exe,sha256=MHQStyg8GLaww0xYFybV3d5BTq3_Laj_IK5-sgbujyU,157696
+ipex_llm/libs/quantize-bloom.exe,sha256=Sc9nJtI_janaigoywxTAIUYrQj_BzROAv7sYjyhSZRE,126464
+ipex_llm/libs/quantize-bloom_vnni.exe,sha256=9OfyR85e6sp6LLiCh-uZvtIyEZUefTMVZ8DXpWsDTvQ,127488
+ipex_llm/libs/quantize-gptneox.exe,sha256=npZ9-vbvXlpRhcHmwsAUmT4Kv-8cB0MWgActIGxDtSg,103936
+ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=F-k0spLR0NK7vrHpwOl2VYR0fZziL7S6boVbfWufLr4,104448
+ipex_llm/libs/quantize-llama.exe,sha256=k3hLlsFb2A6JC_c2Ul0pM1PMLNZyWf9wJyqaBJk0ti8,109056
+ipex_llm/libs/quantize-llama_vnni.exe,sha256=llm6RiPy2xiV1fYGMyjEgiVfbSnwVVgGA1a1Qjitwkc,110080
+ipex_llm/libs/quantize-starcoder.exe,sha256=O40pQGqakxCghOPHcqp2R1UESMkBLj3mPaUV7IjEagA,126976
+ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=qyHzxq8shkaQXHdbFlDmECZHvZCSMd7rFv6tdGNsZEc,128512
+ipex_llm/libs/starcoder-api.dll,sha256=UsHCVSkQS1w2zjnt4XPTcC-JP0Pb4JjNpS1NoqtPT-8,21504
+ipex_llm/libs/starcoder.dll,sha256=54nNOlqEFJdcjeSCJSNYg4x6yL_VG5AJk5OqCY9haeI,563712
 ipex_llm/llamaindex/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/llamaindex/llms/__init__.py,sha256=KP1lEdGqDuxPoxL1ZSH25Pm2kKMPJBWUTLR0ckSLMIU,1139
 ipex_llm/llamaindex/llms/bigdlllm.py,sha256=FQBzq1KOjfc6uofTXAha3O7TqpJkNfOFepXQmOVlbnI,26314
 ipex_llm/serving/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/bigdl_llm_model.py,sha256=NXEN_3EPmcP3dDnvug4MokEXXE2zVUnENgBYxfubqic,10084
 ipex_llm/serving/fastchat/ipex_llm_worker.py,sha256=-nDeJIrGneosxjidzcQBMMkByLsRAM8kV70F5v8Kl10,19605
 ipex_llm/serving/fastchat/model_worker.py,sha256=qJSLyWNkP6z70ysq4AV5SqHzXPJJiX2tz7AORB6jEvM,16649
 ipex_llm/serving/fastchat/tgi_api_protocol.py,sha256=brT3k3-V0NJrU4fRqUwWjC0O3iOitdttDfduXXEefh0,5918
-ipex_llm/serving/fastchat/tgi_api_server.py,sha256=2RNVAhd3tH4yH7F7WootcKg9usXaK0OZ6SdTUamrI_I,27062
+ipex_llm/serving/fastchat/tgi_api_server.py,sha256=agNTAEiZPSuj3dEdIdYKwkoY0cXOUDX06DiM9VP2knQ,24418
 ipex_llm/serving/fastchat/vllm_worker.py,sha256=Jk-GDgM79IJYf_puWH90hTussiQUhUQF_TS7eT8J-W4,11093
 ipex_llm/transformers/__init__.py,sha256=8zrY1AGBb2_AeKGDWHY4PCJyzelYA4KwahD54jPoiPg,1005
 ipex_llm/transformers/bmm.py,sha256=qQ_6Hw2dptT_xCL-1PYHoDRzCZzMpNV63V9TAh5SYjs,1209
-ipex_llm/transformers/convert.py,sha256=PCswNYn-ztT0esTy9SP1QrYeIDhC1MzA-7_YNnyo8xk,76077
+ipex_llm/transformers/convert.py,sha256=ySwrpB997yAHf_qkjPBG3Q5oYZFb6wYQLP6UlfGnDZ0,76127
 ipex_llm/transformers/convert_ipex.py,sha256=iKXo0n8fVFTOA2fNYYrByMFK0dovL-kLd2sVDk88AlQ,14334
 ipex_llm/transformers/embedding.py,sha256=XYbFlP0gbLkxa_Q2aXiEFdHbK0H2WYo8JNNOWLbd-a4,4607
 ipex_llm/transformers/kv.py,sha256=PDdcXWElpiPvzVJQdkkx6Vez0mhROW4K59sngYaX0yY,4247
 ipex_llm/transformers/lisa.py,sha256=F5WxbtXQ7RdKulj83h_2DnEIgKiKGZf7zvOmg6QBl2s,3289
 ipex_llm/transformers/loader.py,sha256=cOgX93xOC-4dt01GTJ5wyd7PjZ8S43r4mctkR2YxVuw,6893
 ipex_llm/transformers/lookup.py,sha256=OBFFNkuSHP9lK6ePTnNFieKs4_vRs83mECrJj0_XoCU,15562
-ipex_llm/transformers/low_bit_linear.py,sha256=_KDj1pbEV6J6FWIPNHuqy9NwtuCmuzAg7zRXjdTnJv0,40985
+ipex_llm/transformers/low_bit_linear.py,sha256=dvVy9gvfrZ9qPkq-ACLl2jmcRhsXrtC3EWfCLM7LDjQ,40895
 ipex_llm/transformers/model.py,sha256=2FCIFGz2dFgxhNLcRHMVyLwBhyOLyEoumtRTS5OB0xQ,39002
 ipex_llm/transformers/modelling_bigdl.py,sha256=AqbRwpSAiHmKUo2FGOiwKtytlh-35NWb6eDy7YyNzoo,6921
 ipex_llm/transformers/qlora.py,sha256=Zo-XeDvTjw_Yzc7Pc3GtyV29SQuy_Zongl1B4iYQID8,15520
 ipex_llm/transformers/relora.py,sha256=-dYzUV0P-IhO2jFdnzN9-v_sFzJpRj3ZwN9eCJzOoCw,16567
 ipex_llm/transformers/speculative.py,sha256=AEda893ENQVFSAjGYLyDLglpCwD7aaCEbL_YMiR5PT4,56660
 ipex_llm/transformers/streamer.py,sha256=RrVlLblzCOtABRUpaMXAyaMnCGgLUtAi_YesLumRbww,4842
 ipex_llm/transformers/training_patch.py,sha256=oxMkUtqyvqJiprw6dE3skkYfD1HOmUlH9N0hBkbn0G0,10799
@@ -188,15 +188,15 @@
 ipex_llm/vllm/cpu/entrypoints/openai/api_server.py,sha256=NIeHHB8IcqmyA83sZEdKPhVM3vpJBupFuTFOuW2nj-Q,6944
 ipex_llm/vllm/xpu/__init__.py,sha256=zBSG6nzrVF5QnpR6_f7kPhBFeowTE9gaZ7D5m98E7_w,585
 ipex_llm/vllm/xpu/ipex_llm_gpu_executor.py,sha256=3lfClSuMWg6tfDmi_kCAI9zmc9_N5DINL-ZS6UHs0N0,18506
 ipex_llm/vllm/xpu/model_convert.py,sha256=lriPO5Ife5lMU6q5US4N6l9Y-iQmZa1fNGFPLXoVTuM,7172
 ipex_llm/vllm/xpu/engine/__init__.py,sha256=mzPVAyZdbvfzBQi-wxZh1sbme_NElPMmtrJ9C2zh8Us,747
 ipex_llm/vllm/xpu/engine/engine.py,sha256=6cRzT1UUoqbcaeLh-PigsRv881QavHIWUvHlB5miy3A,5953
 ipex_llm/vllm/xpu/entrypoints/openai/api_server.py,sha256=uIujXmuoKAcOcx5dz8DhnXpqpIlCgPz-4k-SfYKSvS0,10568
-ipex_llm-2.1.0b20240529.data/scripts/ipex-llm-init.bat,sha256=HPtCYuDYwEatq7dAwOvdfVcHYCpAVdbj75K1qh0vQek,2578
-ipex_llm-2.1.0b20240529.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
-ipex_llm-2.1.0b20240529.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
-ipex_llm-2.1.0b20240529.dist-info/METADATA,sha256=pV1BEAlYc0_pNv3nCxbwRuSLBwKB2TxkFyE-CNCsyTs,5495
-ipex_llm-2.1.0b20240529.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-ipex_llm-2.1.0b20240529.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
-ipex_llm-2.1.0b20240529.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
-ipex_llm-2.1.0b20240529.dist-info/RECORD,,
+ipex_llm-2.1.0b20240530.data/scripts/ipex-llm-init.bat,sha256=HPtCYuDYwEatq7dAwOvdfVcHYCpAVdbj75K1qh0vQek,2578
+ipex_llm-2.1.0b20240530.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
+ipex_llm-2.1.0b20240530.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
+ipex_llm-2.1.0b20240530.dist-info/METADATA,sha256=fk51HAbOuySRLPvpQRQfd35dF54hVefUpnoYA6FDr_o,5495
+ipex_llm-2.1.0b20240530.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+ipex_llm-2.1.0b20240530.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
+ipex_llm-2.1.0b20240530.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
+ipex_llm-2.1.0b20240530.dist-info/RECORD,,
```

